# Comparing `tmp/pyfixest-0.6.tar.gz` & `tmp/pyfixest-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfixest-0.6.tar", max compression
+gzip compressed data, was "pyfixest-0.6.5.tar", max compression
```

## Comparing `pyfixest-0.6.tar` & `pyfixest-0.6.5.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1096 2022-11-19 12:53:04.921992 pyfixest-0.6/LICENSE.md
--rw-r--r--   0        0        0       26 2023-03-16 21:51:51.234748 pyfixest-0.6/pyfixest/__init__.py
--rw-r--r--   0        0        0    20564 2023-05-21 16:38:34.330335 pyfixest-0.6/pyfixest/feols.py
--rw-r--r--   0        0        0    44096 2023-05-21 16:38:34.332330 pyfixest-0.6/pyfixest/fixest.py
--rw-r--r--   0        0        0    19550 2023-05-21 16:38:34.319816 pyfixest-0.6/pyfixest/FormulaParser.py
--rw-r--r--   0        0        0     3426 2023-04-27 19:03:35.062476 pyfixest-0.6/pyfixest/ssc_utils.py
--rw-r--r--   0        0        0     1312 2023-05-21 16:38:34.333327 pyfixest-0.6/pyfixest/utils.py
--rw-r--r--   0        0        0      894 2023-05-21 16:38:34.334501 pyfixest-0.6/pyproject.toml
--rw-r--r--   0        0        0     2684 2023-05-21 16:38:31.130088 pyfixest-0.6/readme.md
--rw-r--r--   0        0        0     3566 1970-01-01 00:00:00.000000 pyfixest-0.6/PKG-INFO
+-rw-r--r--   0        0        0     1096 2022-11-19 12:53:04.921992 pyfixest-0.6.5/LICENSE.md
+-rw-r--r--   0        0        0       26 2023-03-16 21:51:51.234748 pyfixest-0.6.5/pyfixest/__init__.py
+-rw-r--r--   0        0        0     4330 2023-06-22 18:59:48.885238 pyfixest-0.6.5/pyfixest/demean.py
+-rw-r--r--   0        0        0    21004 2023-07-06 20:11:17.320736 pyfixest-0.6.5/pyfixest/feols.py
+-rw-r--r--   0        0        0    45465 2023-06-22 18:59:48.886235 pyfixest-0.6.5/pyfixest/fixest.py
+-rw-r--r--   0        0        0    20302 2023-06-04 20:23:08.754381 pyfixest-0.6.5/pyfixest/FormulaParser.py
+-rw-r--r--   0        0        0     3426 2023-04-27 19:03:35.062476 pyfixest-0.6.5/pyfixest/ssc_utils.py
+-rw-r--r--   0        0        0     1312 2023-06-04 20:23:04.808444 pyfixest-0.6.5/pyfixest/utils.py
+-rw-r--r--   0        0        0      939 2023-07-06 20:11:17.322020 pyfixest-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0     2617 2023-06-04 20:23:08.766777 pyfixest-0.6.5/readme.md
+-rw-r--r--   0        0        0     3573 1970-01-01 00:00:00.000000 pyfixest-0.6.5/PKG-INFO
```

### Comparing `pyfixest-0.6/LICENSE.md` & `pyfixest-0.6.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyfixest-0.6/pyfixest/feols.py` & `pyfixest-0.6.5/pyfixest/feols.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import warnings
 
-from wildboottest.wildboottest import WildboottestCL, WildboottestHC
 from importlib import import_module
 from typing import Union, List, Dict
 from scipy.stats import norm, t
 from pyfixest.ssc_utils import get_ssc
 
 
 class Feols:
@@ -136,15 +135,15 @@
         -------
         None
 
         '''
 
         _check_vcov_input(vcov, self.data)
 
-        self.vcov_type, self.vcov_type_detail, self.is_clustered, self.clustervar = _deparse_vcov_input(vcov, self.has_fixef)
+        self.vcov_type, self.vcov_type_detail, self.is_clustered, self.clustervar = _deparse_vcov_input(vcov, self.has_fixef, self.is_iv)
 
         if self.is_iv:
             if self.vcov_type in ["CRV3"]:
                 raise ValueError("CRV3 inference is not supported for IV regressions.")
 
         # compute vcov
         if self.vcov_type == 'iid':
@@ -391,14 +390,19 @@
         bootstrap_type (str, optional):A string of length one. Allows to choose the bootstrap type
                             to be run. Either '11', '31', '13' or '33'. '11' by default. Defaults to '11'.
         seed (Union[str, None], optional): Option to provide a random seed. Defaults to None.
 
         Returns: a pd.DataFrame with bootstrapped t-statistic and p-value
         '''
 
+        try:
+            from wildboottest.wildboottest import WildboottestCL, WildboottestHC
+        except ImportError:
+            print("Module 'wildboottest' not found. Please install 'wildboottest'. Note that it 'wildboottest 'requires Python < 3.11 due to its dependency on 'numba'.")
+
         if self.is_iv:
             raise ValueError("Wild cluster bootstrap is not supported with IV estimation.")
         if self.has_fixef:
             raise ValueError("Wild cluster bootstrap is not supported with fixed effects.")
 
         xnames = self.coefnames.to_list()
         Y = self.Y.flatten()
@@ -494,22 +498,23 @@
     if isinstance(vcov, list):
         assert all(isinstance(v, str) for v in vcov), "vcov list must contain strings"
         assert all(v in data.columns for v in vcov), "vcov list must contain columns in the data"
     if isinstance(vcov, str):
         assert vcov in ["iid", "hetero", "HC1", "HC2", "HC3"], "vcov string must be iid, hetero, HC1, HC2, or HC3"
 
 
-def _deparse_vcov_input(vcov, has_fixef):
+def _deparse_vcov_input(vcov, has_fixef, is_iv):
 
     '''
     Deparse the vcov argument passed to the Feols class.
 
     Args:
         vcov (dict, str, list): The vcov argument passed to the Feols class.
         has_fixef (bool): Whether the regression has fixed effects.
+        is_iv (bool): Whether the regression is an IV regression.
     Returns:
         vcov_type (str): The type of vcov to be used. Either "iid", "hetero", or "CRV"
         vcov_type_detail (str, list): The type of vcov to be used, with more detail. Either "iid", "hetero", "HC1", "HC2", "HC3", "CRV1", or "CRV3"
         is_clustered (bool): Whether the vcov is clustered.
         clustervar (str): The name of the cluster variable.
     '''
 
@@ -528,14 +533,16 @@
         is_clustered = False
     elif vcov_type_detail in ["hetero", "HC1", "HC2", "HC3"]:
         vcov_type = "hetero"
         is_clustered = False
         if vcov_type_detail in ["HC2", "HC3"]:
             if has_fixef:
                 raise ValueError("HC2 and HC3 inference types are not supported for regressions with fixed effects.")
+            if is_iv:
+                raise ValueError("HC2 and HC3 inference types are not supported for IV regressions.")
     elif vcov_type_detail in ["CRV1", "CRV3"]:
         vcov_type = "CRV"
         is_clustered = True
 
     if is_clustered:
         clustervar = list(vcov.values())[0]
     else:
```

### Comparing `pyfixest-0.6/pyfixest/fixest.py` & `pyfixest-0.6.5/pyfixest/fixest.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 from formulaic import model_matrix
 
 from pyfixest.feols import Feols
 from pyfixest.FormulaParser import FixestFormulaParser, _flatten_list
 from pyfixest.ssc_utils import ssc
 
 
+class DepvarIsNotNumericError(Exception):
+    pass
+
+
 class Fixest:
 
     def __init__(self, data: pd.DataFrame) -> None:
         '''
         A class for fixed effects regression modeling.
         Args:
             data: The input pd.DataFrame for the object.
@@ -29,32 +33,40 @@
         self.model_res = dict()
 
     def _clean_fe(self, data, fval):
 
         fval_list = fval.split("+")
 
         # find interacted fixed effects via "^"
-        interacted_fes = [
-            x for x in fval_list if len(x.split('^')) > 1]
+        interacted_fes = [x for x in fval_list if len(x.split('^')) > 1]
+            
+        varying_slopes = [x for x in fval_list if len(x.split('/')) > 1]
 
         for x in interacted_fes:
             vars = x.split("^")
             data[x] = data[vars].apply(lambda x: '^'.join(
                 x.dropna().astype(str)) if x.notna().all() else np.nan, axis=1)
-
+        
         fe = data[fval_list]
         # all fes to factors / categories
-        fe = fe.apply(lambda x: pd.factorize(x)[0])
 
+        if varying_slopes != []: 
+          
+            for x in varying_slopes: 
+                mm_vs = model_matrix("-1 + " + x, data)
+            
+            fe = pd.concat([fe, mm_vs], axis = 1)
+        
         fe_na = fe.isna().any(axis=1)
+        fe = fe.apply(lambda x: pd.factorize(x)[0])
         fe = fe.to_numpy()
 
         return fe, fe_na
 
-    def _demean(self, data: pd.DataFrame, fval: str, ivars: List[str], drop_ref: str) -> None:
+    def _demean_model(self, data: pd.DataFrame, fval: str, ivars: List[str], drop_ref: str) -> None:
         '''
         Demean all regressions for a specification of fixed effects.
 
         Args:
             data: The input pd.DataFrame for the object. Either self.data or a subset thereof (for split sample estimation).
             fval: A specification of fixed effects. A string indicating the fixed effects to be demeaned,
                 such as "X4" or "X3 + X2".
@@ -102,39 +114,41 @@
                 fml = depvar2 + " ~ " + covar2
 
                 if self.is_iv:
                     instruments2 = dict2fe_iv.get(depvar)[0]
                     endogvar_list = list(set(covar2.split("+")) - set(instruments2.split("+")))#[0]
                     instrument_list = list(set(instruments2.split("+")) - set(covar2.split("+")))#[0]
 
-                    #if len(instrument_list) > 1 or len(endogvar_list) > 1:
-                    #    raise ValueError("Currently, IV estimation is only supported with one endogeneous variable and one instrument.")
-
                     fml2 = "+".join(instrument_list) + "+" + fml
-                    rhs, lhs = model_matrix(fml2, data)
 
-                    Y = rhs[[depvar]]
-                    I = rhs[instrument_list]
-                    X = lhs
                 else:
-                    Y, X = model_matrix(fml, data)
+                    fml2 = fml
+
+                lhs, rhs = model_matrix(fml2, data)
+
+                untransformed_depvar = _find_untransformed_depvar(depvar2)
 
+                Y = lhs[[depvar]]
+                X = rhs
+                if self.is_iv:
+                    I = lhs[instrument_list]
+
+                # get NA index before converting Y to numpy array
                 na_index = list(set(data.index) - set(Y.index))
 
+                # drop variables before collecting variable names
                 if self.ivars is not None:
                     if drop_ref is not None:
                         X = X.drop(drop_ref, axis=1)
 
                 y_names = list(Y.columns)
                 x_names = list(X.columns)
                 yxz_names = list(y_names) + list(x_names)
                 if self.is_iv:
                     iv_names = list(I.columns)
-                    #z_varnames = list(set(x_names) - set([endogvar]))
-                    #z_varnames.append(instrument)
                     x_names_copy = x_names.copy()
                     x_names_copy = [x for x in x_names_copy if x not in endogvar_list]
                     z_names = x_names_copy + instrument_list
                     cols = yxz_names + iv_names
                 else:
                     iv_names = None
                     z_names = None
@@ -144,36 +158,29 @@
                     self.icovars = [s for s in x_names if s.startswith(
                         ivars[0]) and s.endswith(ivars[1])]
                 else:
                     self.icovars = None
 
 
                 Y = Y.to_numpy()
-                #if Y.ndim != 1:
-                #    Y = Y.reshape((len(Y), 1))
-                #.reshape((len(Y), 1))
                 X = X.to_numpy()
                 if self.is_iv:
                     I = I.to_numpy()
-                    #if I.ndim != 1:
-                    #    I = I.reshape((len(I), 1))
 
                 if Y.shape[1] > 1:
                     raise ValueError(
                         "Dependent variable must be a single column. Please make sure that the dependent variable" + depvar2 + "is of a numeric type (int or float).")
 
                 # variant 1: if there are fixed effects to be projected out
                 if fe is not None:
                     na_index = (na_index + fe_na)
                     fe2 = np.delete(fe, na_index, axis=0)
                     # drop intercept
                     intercept_index = x_names.index("Intercept")
                     X = np.delete(X, intercept_index, axis = 1)
-                    #if self.is_iv:
-                    #    I = np.delete(I, intercept_index, axis = 1)
                     x_names.remove("Intercept")
                     yxz_names.remove("Intercept")
                     if self.is_iv:
                         z_names.remove("Intercept")
                         cols.remove("Intercept")
 
                     # check if variables have already been demeaned
@@ -214,61 +221,174 @@
                     else:
                         # not data demeaned yet for NA combination
                         algorithm = pyhdfe.create(
                             ids=fe2,
                             residualize_method='map',
                             drop_singletons=self.drop_singletons,
                         )
-                        # n_singletons = algorithm.singletons
-                        # if n_singletons is not None:
-                        #    print(f'{n_singletons} columns are dropped due to singleton fixed effects.')
+
                         if self.drop_singletons == True and algorithm.singletons != 0 and algorithm.singletons is not None:
-                            print(
-                                algorithm.singletons, "columns are dropped due to singleton fixed effects.")
+                            print(algorithm.singletons, "columns are dropped due to singleton fixed effects.")
                             dropped_singleton_indices = (
                                 np.where(algorithm._singleton_indices))[0].tolist()
                             na_index += dropped_singleton_indices
 
                         YXZ_demeaned = algorithm.residualize(YXZ)
                         YXZ_demeaned = pd.DataFrame(YXZ_demeaned)
 
-                        #if self.is_iv:
-                        #    cols += iv_names
-
                         YXZ_demeaned.columns = cols
 
                     lookup_demeaned_data[na_index_str] = [
                         algorithm, YXZ_demeaned]
 
                 else:
                     # if no fixed effects
                     if self.is_iv:
                         YXZ = np.concatenate([Y, X, I], axis=1)
                     else:
                         YXZ = np.concatenate([Y, X], axis=1)
 
                     YXZ_demeaned = pd.DataFrame(YXZ)
 
-                    #if self.is_iv:
-                    #    cols += list(iv_names)
-
                     YXZ_demeaned.columns = cols
 
-                YXZ_dict[fml] = YXZ_demeaned#[cols]
+                YXZ_dict[fml] = YXZ_demeaned
                 na_dict[fml] = na_index
                 var_dict[fml] = dict({
                     'y_names': y_names,
                     'x_names': x_names,
                     'iv_names': iv_names,
                     'z_names': z_names
                 })
 
 
         return YXZ_dict, na_dict, var_dict
 
+    def _demean_all_models(self, fixef_keys, ivars, drop_ref, estimate_full_model, estimate_split_model):
+
+        '''
+        demean multiple models. essentially, the function loops
+        over all split var and fixed effects variables and demeans the
+        specified dependend variables and covariates
+        Args:
+            fixef_keys: fixed effect variables
+            ivars: interaction variables
+            drop_ref: drop reference category
+            estimate_full_model: boolean, whether to estimate the full model
+            estimate_split_model: boolean, whether to estimate the split model
+        '''
+
+        if estimate_full_model:
+            for _, fval in enumerate(fixef_keys):
+                self.demeaned_data_dict[fval] = []
+                self.dropped_data_dict[fval] = []
+                self.yxz_name_dict[fval] = []
+                data = self.data
+                demeaned_data, dropped_data, yxz_name_dict= self._demean_model(
+                    data, fval, ivars, drop_ref)
+                self.demeaned_data_dict[fval].append(demeaned_data)
+                self.dropped_data_dict[fval].append(dropped_data)
+                self.yxz_name_dict[fval].append(yxz_name_dict)
+
+        if estimate_split_model:
+            for _, fval in enumerate(fixef_keys):
+                self.demeaned_data_dict[fval] = []
+                self.dropped_data_dict[fval] = []
+                self.yxz_name_dict[fval] = []
+                for x in self.split_categories:
+                    sub_data = self.data[x == self.splitvar]
+                    demeaned_data, dropped_data, yxz_name_dict = self._demean_model(
+                        sub_data, fval, ivars, drop_ref)
+                    self.demeaned_data_dict[fval].append(demeaned_data)
+                    self.dropped_data_dict[fval].append(dropped_data)
+                    self.yxz_name_dict[fval].append(yxz_name_dict)
+
+    def _estimate_all_models(self, vcov):
+
+        # estimate models based on demeaned model matrix and dependent variables
+        for _, fval in enumerate(self.fml_dict.keys()):
+            model_splits = self.demeaned_data_dict[fval]
+            for x, _ in enumerate(model_splits):
+                model_frames = model_splits[x]
+                for _, fml in enumerate(model_frames):
+
+                    # get the (demeaned) model frame. key is fml without fixed effects
+                    model_frame = model_frames[fml]
+
+                    # update formula with fixed effect. fval is "0" for no fixed effect
+                    if fval == "0":
+                        fml2 = fml
+                    else:
+                        fml2 = fml + "|" + fval
+
+                    # formula log: add information on sample split
+                    if self.splitvar is not None:
+                        split_log = str(self.split_categories[x])
+                        full_fml = fml2 + "| split =" + split_log
+                    else:
+                        split_log = None
+                        full_fml = fml2
+
+                    name_dict = self.yxz_name_dict[fval][0][fml]
+                    depvar_name = name_dict["y_names"]
+                    xvar_names = name_dict["x_names"]
+                    if name_dict["z_names"] is None:
+                        zvar_names = name_dict["x_names"]
+                    else:
+                        zvar_names = name_dict["z_names"]
+
+                    Y = model_frame[depvar_name]
+                    X = model_frame[xvar_names]
+                    Z = model_frame[zvar_names]
+
+                    colnames = X.columns
+                    zcolnames = Z.columns
+
+                    Y = Y.to_numpy()
+                    X = X.to_numpy()
+                    Z = Z.to_numpy()
+
+                    N = X.shape[0]
+                    k = X.shape[1]
+
+                    # check for multicollinearity
+                    _multicollinearity_checks(X, Z, self.ivars, fml2)
+
+                    FEOLS = Feols(Y, X, Z)
+                    FEOLS.is_iv = self.is_iv
+                    FEOLS.fml = fml2
+                    FEOLS.ssc_dict = self.ssc_dict
+                    if self.is_iv:
+                        FEOLS.get_fit(estimator = "2sls")
+                    else:
+                        FEOLS.get_fit(estimator = "ols")
+                    FEOLS.na_index = self.dropped_data_dict[fval][x][fml]
+                    FEOLS.data = self.data.iloc[~self.data.index.isin(
+                        FEOLS.na_index), :]
+                    FEOLS.N = N
+                    FEOLS.k = k
+                    if fval != "0":
+                        FEOLS.has_fixef = True
+                        FEOLS.fixef = fval
+                    else:
+                        FEOLS.has_fixef = False
+
+                    vcov_type = _get_vcov_type(vcov, fval)
+
+                    FEOLS.vcov_log = vcov_type
+                    FEOLS.split_log = x
+                    FEOLS.get_vcov(vcov=vcov_type)
+                    FEOLS.get_inference()
+                    FEOLS.coefnames = colnames
+                    if self.icovars is not None:
+                        FEOLS.icovars = self.icovars
+                    self.model_res[full_fml] = FEOLS
+
+
+
     def feols(self, fml: str, vcov: Union[None, str, Dict[str, str]] = None, ssc=ssc(), fixef_rm: str = "none") -> None:
         '''
         Method for fixed effects regression modeling using the PyHDFE package for projecting out fixed effects.
         Args:
             fml (str): A three-sided formula string using fixest formula syntax. Supported syntax includes:
                 The syntax is as follows: "Y ~ X1 + X2 | FE1 + FE2 | X1 ~ Z1" where:
 
@@ -314,14 +434,21 @@
                 fml = 'Y1 + Y2 ~ X1 + X2'
             Stepwise regressions (sw and sw0):
                 fml = 'Y1 + Y2 ~ sw(X1, X2, X3)'
             Cumulative stepwise regressions (csw and csw0):
                 fml = 'Y1 + Y2 ~ csw(X1, X2, X3) '
             Combinations:
                 fml = 'Y1 + Y2 ~ csw(X1, X2, X3) | sw(X4, X5) + X6'
+
+        Details:
+            The method proceeds in the following steps:
+            1. Parse the formula using the FixestFormulaParser class.
+            2. Create a dictionary of formulas for each dependent variable.
+            3. demean all models and store the data
+            4. fit all models
         '''
 
         self.fml = fml.replace(" ", "")
         self.split = None
 
         # deparse formula, at least partially
         fxst_fml = FixestFormulaParser(fml)
@@ -383,137 +510,45 @@
         self.yxz_name_dict = dict()
 
         estimate_full_model = True
         estimate_split_model = False
         # currently no fsplit allowed
         fsplit = None
 
-        self.splitvar, _, estimate_split_model, estimate_full_model = _prepare_split_estimation(
-            self.split,
-            fsplit,
-            self.data,
-            self.var_dict
-        )
+        self.splitvar, _, estimate_split_model, estimate_full_model = _prepare_split_estimation(self.split, fsplit, self.data, self.var_dict)
 
-        if estimate_full_model:
-            for _, fval in enumerate(fixef_keys):
-                self.demeaned_data_dict[fval] = []
-                self.dropped_data_dict[fval] = []
-                self.yxz_name_dict[fval] = []
-                data = self.data
-                demeaned_data, dropped_data, yxz_name_dict= self._demean(
-                    data, fval, ivars, drop_ref)
-                self.demeaned_data_dict[fval].append(demeaned_data)
-                self.dropped_data_dict[fval].append(dropped_data)
-                self.yxz_name_dict[fval].append(yxz_name_dict)
-        # here:
-        if estimate_split_model:
-            for _, fval in enumerate(fixef_keys):
-                self.demeaned_data_dict[fval] = []
-                self.dropped_data_dict[fval] = []
-                self.yxz_name_dict[fval] = []
-                for x in self.split_categories:
-                    sub_data = self.data[x == self.splitvar]
-                    demeaned_data, dropped_data, yxz_name_dict = self._demean(
-                        sub_data, fval, ivars, drop_ref)
-                    self.demeaned_data_dict[fval].append(demeaned_data)
-                    self.dropped_data_dict[fval].append(dropped_data)
-                    self.yxz_name_dict[fval].append(yxz_name_dict)
+        # demean all models: based on fixed effects x split x missing value combinations
+        self._demean_all_models(fixef_keys, ivars, drop_ref, estimate_full_model, estimate_split_model)
 
-        self.is_fixef_multi = False
-        if len(self.fml_dict.keys()) > 1:
-            self.is_fixef_multi = True
-        elif len(self.fml_dict.keys()) == 1:
-            first_key = next(iter(self.fml_dict))
-            if len(self.fml_dict[first_key]) > 1:
-                self.is_fixef_multi = True
+        # create self.is_fixef_multi flag
+        self._is_multiple_estimation()
 
         if self.is_fixef_multi and self.is_iv:
             raise ValueError("Multiple Estimations is currently not supported with IV. This is mostly due to insufficient testing and will be possible with the next release of PyFixest.")
 
-        # estimate models based on demeaned model matrix and dependent variables
-        for _, fval in enumerate(self.fml_dict.keys()):
-            model_splits = self.demeaned_data_dict[fval]
-            for x, _ in enumerate(model_splits):
-                model_frames = model_splits[x]
-                for _, fml in enumerate(model_frames):
-
-                    # get the (demeaned) model frame. key is fml without fixed effects
-                    model_frame = model_frames[fml]
-
-                    # update formula with fixed effect. fval is "0" for no fixed effect
-                    if fval == "0":
-                        fml2 = fml
-                    else:
-                        fml2 = fml + "|" + fval
-
-                    # formula log: add information on sample split
-                    if self.splitvar is not None:
-                        split_log = str(self.split_categories[x])
-                        full_fml = fml2 + "| split =" + split_log
-                    else:
-                        split_log = None
-                        full_fml = fml2
-
-                    name_dict = self.yxz_name_dict[fval][0][fml]
-                    depvar_name = name_dict["y_names"]
-                    xvar_names = name_dict["x_names"]
-                    if name_dict["z_names"] is None:
-                        zvar_names = name_dict["x_names"]
-                    else:
-                        zvar_names = name_dict["z_names"]
-
-                    Y = model_frame[depvar_name]
-                    X = model_frame[xvar_names]
-                    Z = model_frame[zvar_names]
-
-                    colnames = X.columns
-                    zcolnames = Z.columns
+        # estimate all regression models based on demeaned data
+        self._estimate_all_models(vcov = vcov)
 
-                    Y = Y.to_numpy()
-                    X = X.to_numpy()
-                    Z = Z.to_numpy()
+        return self
 
-                    N = X.shape[0]
-                    k = X.shape[1]
 
-                    # check for multicollinearity
-                    _multicollinearity_checks(X, Z, ivars, fml2)
+    def _is_multiple_estimation(self):
 
-                    FEOLS = Feols(Y, X, Z)
-                    FEOLS.is_iv = self.is_iv
-                    FEOLS.fml = fml2
-                    FEOLS.ssc_dict = self.ssc_dict
-                    if self.is_iv:
-                        FEOLS.get_fit(estimator = "2sls")
-                    else:
-                        FEOLS.get_fit(estimator = "ols")
-                    FEOLS.na_index = self.dropped_data_dict[fval][x][fml]
-                    FEOLS.data = self.data.iloc[~self.data.index.isin(
-                        FEOLS.na_index), :]
-                    FEOLS.N = N
-                    FEOLS.k = k
-                    if fval != "0":
-                        FEOLS.has_fixef = True
-                        FEOLS.fixef = fval
-                    else:
-                        FEOLS.has_fixef = False
-
-                    vcov_type = _get_vcov_type(vcov, fval)
+        '''
+        helper method to check if multiple regression models will be estimated
+        '''
 
-                    FEOLS.vcov_log = vcov_type
-                    FEOLS.split_log = x
-                    FEOLS.get_vcov(vcov=vcov_type)
-                    FEOLS.get_inference()
-                    FEOLS.coefnames = colnames
-                    if self.icovars is not None:
-                        FEOLS.icovars = self.icovars
-                    self.model_res[full_fml] = FEOLS
+        self.is_fixef_multi = False
+        if len(self.fml_dict.keys()) > 1:
+            self.is_fixef_multi = True
+        elif len(self.fml_dict.keys()) == 1:
+            first_key = next(iter(self.fml_dict))
+            if len(self.fml_dict[first_key]) > 1:
+                self.is_fixef_multi = True
 
-        return self
 
     def vcov(self, vcov: Union[str, Dict[str, str]]) -> None:
         '''
         Update regression inference "on the fly".
         By calling vcov() on a "Fixest" object, all inference procedures applied
         to the "Fixest" object are replaced with the variance covariance matrix specified via the method.
         Args:
@@ -1075,7 +1110,25 @@
         drop_singletons (bool): Whether to drop singletons.
     '''
 
     if fixef_rm == "singleton":
         return True
     else:
         return False
+
+
+
+def _find_untransformed_depvar(transformed_depvar):
+
+    '''
+    Args:
+        transformed_depvar (str): The transformed depvar
+
+    find untransformed depvar in a formula
+    i.e. if "a" is transormed to "log(a)", then "a" is returned
+    '''
+
+    match = re.search(r'\((.*?)\)', transformed_depvar)
+    if match:
+        return match.group(1)
+    else:
+        return transformed_depvar
```

### Comparing `pyfixest-0.6/pyfixest/FormulaParser.py` & `pyfixest-0.6.5/pyfixest/FormulaParser.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,24 +314,31 @@
     res_s = dict()
     res_s['constant'] = []
 
     for var in var_split:
 
         # Check if this variable contains a switch
         varlist, sw_type = _find_sw(var)
-
+        
         # If there's no switch, just add the variable to the list
         if sw_type is None:
-            res_s['constant'].append(var)
+            if _is_varying_slopes(var):
+                varlist, sw_type = _transform_varying_slopes(var)
+                for x in varlist.split("+"): 
+                    res_s['constant'].append(x)
+            else: 
+                res_s['constant'].append(varlist)
 
-        # If there's a switch, unpack it and add it to the list
+        # If there'_ a switch, unpack it and add it to the list
         else:
             if sw_type in ['sw', 'sw0', 'csw', 'csw0', 'i']:
                 _check_duplicate_key(res_s, sw_type)
                 res_s[sw_type] = varlist
+            elif sw_type == "varying_slopes": 
+                res_s[sw_type] = varlist
             else:
                 raise ValueError("Unsupported switch type")
 
     # Sort the list by type (strings first, then lists)
     #res_s.sort(key=lambda x: 0 if isinstance(x, str) else 1)
 
     return res_s
@@ -519,7 +526,25 @@
         raise DuplicateKeyError("Duplicate key found: " + key + ". Fixed effect syntax i() can only be used once in the input formula.")
     else:
         for key in ['sw', 'csw', 'sw0', 'csw0']:
             if key in my_dict:
                 raise DuplicateKeyError("Duplicate key found: " + key + ". Multiple estimation syntax can only be used once on the rhs of the two-sided formula.")
             else:
                 None
+                
+                
+def _is_varying_slopes(x): 
+          
+    pattern = r'\[.*\]'
+    match = re.search(pattern, x)
+    if match:
+        return True
+    else:
+        return False
+            
+def _transform_varying_slopes(x):
+    parts = x.split('[')
+    a = parts[0]
+    b = parts[1].replace(']', '')
+    transformed_string = f"{a}/{b}"
+    return transformed_string, "varying_slopes"
+
```

### Comparing `pyfixest-0.6/pyfixest/ssc_utils.py` & `pyfixest-0.6.5/pyfixest/ssc_utils.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.6/pyfixest/utils.py` & `pyfixest-0.6.5/pyfixest/utils.py`

 * *Files identical despite different names*

### Comparing `pyfixest-0.6/pyproject.toml` & `pyfixest-0.6.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "pyfixest"
-version = "0.6"
+version = "0.6.5"
 
 description = "Experimental draft package for high dimensional fixed effect estimation. Supports OLS and IV estimation."
 authors = ["Alexander Fischer <alexander-fischer1801@t-online.de>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://s3alfisc.github.io/pyfixest/"
 repository = "https://github.com/s3alfisc/pyfixest"
 
 [tool.poetry.dependencies]
-python=">=3.8,<3.11"
+python=">=3.8"
 pandas="^1.4"
 numpy=">=1.18"
 matplotlib = "^3.7"
 PyHDFE = "^0.1.1"
 scipy = "^1.0.0"
 formulaic = "^0.6.0"
 pytest="^7.0.0"
-wildboottest = ">=0.1.10"
+wildboottest = { version = ">=0.1.10", optional = true, python = "<3.11" }
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 mkdocs-material = "^8.5.10"
 mkdocstrings = "^0.19.0"
```

### Comparing `pyfixest-0.6/readme.md` & `pyfixest-0.6.5/readme.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 ## PyFixest
 
 [![PyPI - Version](https://img.shields.io/pypi/v/pyfixest.svg)](https://pypi.org/project/pyfixest/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyfixest.svg)
-![PyPI - Status](https://img.shields.io/pypi/status/pyfixest.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pyfixest)
 [![image](https://codecov.io/gh/s3alfisc/pyfixest/branch/master/graph/badge.svg)](https://codecov.io/gh/s3alfisc/pyfixest)
 
 This is a draft package (highly experimental!) for a Python clone of the excellent [fixest](https://github.com/lrberge/fixest) package.
 
 Fixed effects are projected out via the [PyHDFE](https://github.com/jeffgortmaker/pyhdfe) package.
```

### Comparing `pyfixest-0.6/PKG-INFO` & `pyfixest-0.6.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: pyfixest
-Version: 0.6
+Version: 0.6.5
 Summary: Experimental draft package for high dimensional fixed effect estimation. Supports OLS and IV estimation.
 Home-page: https://s3alfisc.github.io/pyfixest/
 License: MIT
 Author: Alexander Fischer
 Author-email: alexander-fischer1801@t-online.de
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyHDFE (>=0.1.1,<0.2.0)
 Requires-Dist: formulaic (>=0.6.0,<0.7.0)
 Requires-Dist: matplotlib (>=3.7,<4.0)
 Requires-Dist: numpy (>=1.18)
 Requires-Dist: pandas (>=1.4,<2.0)
 Requires-Dist: pytest (>=7.0.0,<8.0.0)
 Requires-Dist: scipy (>=1.0.0,<2.0.0)
-Requires-Dist: wildboottest (>=0.1.10)
+Requires-Dist: wildboottest (>=0.1.10) ; python_version < "3.11"
 Project-URL: Repository, https://github.com/s3alfisc/pyfixest
 Description-Content-Type: text/markdown
 
 ## PyFixest
 
 [![PyPI - Version](https://img.shields.io/pypi/v/pyfixest.svg)](https://pypi.org/project/pyfixest/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyfixest.svg)
-![PyPI - Status](https://img.shields.io/pypi/status/pyfixest.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pyfixest)
 [![image](https://codecov.io/gh/s3alfisc/pyfixest/branch/master/graph/badge.svg)](https://codecov.io/gh/s3alfisc/pyfixest)
 
 This is a draft package (highly experimental!) for a Python clone of the excellent [fixest](https://github.com/lrberge/fixest) package.
 
 Fixed effects are projected out via the [PyHDFE](https://github.com/jeffgortmaker/pyhdfe) package.
```

