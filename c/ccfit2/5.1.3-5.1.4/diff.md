# Comparing `tmp/ccfit2-5.1.3.tar.gz` & `tmp/ccfit2-5.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccfit2-5.1.3.tar", last modified: Wed Jun 28 13:09:39 2023, max compression
+gzip compressed data, was "ccfit2-5.1.4.tar", last modified: Thu Jul  6 12:09:32 2023, max compression
```

## Comparing `ccfit2-5.1.3.tar` & `ccfit2-5.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 13:09:39.868527 ccfit2-5.1.3/
--rw-rw-rw-   0 root         (0) root         (0)    35075 2023-06-28 13:09:09.000000 ccfit2-5.1.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1132 2023-06-28 13:09:39.868527 ccfit2-5.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      501 2023-06-28 13:09:09.000000 ccfit2-5.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 13:09:39.867610 ccfit2-5.1.3/ccfit2/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-28 13:09:09.000000 ccfit2-5.1.3/ccfit2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-28 13:09:37.000000 ccfit2-5.1.3/ccfit2/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)   132398 2023-06-28 13:09:09.000000 ccfit2-5.1.3/ccfit2/ac.py
--rw-rw-rw-   0 root         (0) root         (0)    69434 2023-06-28 13:09:09.000000 ccfit2-5.1.3/ccfit2/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    61106 2023-06-28 13:09:09.000000 ccfit2-5.1.3/ccfit2/dc.py
--rw-rw-rw-   0 root         (0) root         (0)    23311 2023-06-28 13:09:09.000000 ccfit2-5.1.3/ccfit2/gui.py
--rw-rw-rw-   0 root         (0) root         (0)   171342 2023-06-28 13:09:09.000000 ccfit2-5.1.3/ccfit2/relaxation.py
--rw-rw-rw-   0 root         (0) root         (0)     1756 2023-06-28 13:09:09.000000 ccfit2-5.1.3/ccfit2/stats.py
--rw-rw-rw-   0 root         (0) root         (0)    10668 2023-06-28 13:09:09.000000 ccfit2-5.1.3/ccfit2/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    21023 2023-06-28 13:09:09.000000 ccfit2-5.1.3/ccfit2/waveform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 13:09:39.868527 ccfit2-5.1.3/ccfit2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1132 2023-06-28 13:09:39.000000 ccfit2-5.1.3/ccfit2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      390 2023-06-28 13:09:39.000000 ccfit2-5.1.3/ccfit2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 13:09:39.000000 ccfit2-5.1.3/ccfit2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2023-06-28 13:09:39.000000 ccfit2-5.1.3/ccfit2.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      133 2023-06-28 13:09:39.000000 ccfit2-5.1.3/ccfit2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-28 13:09:39.000000 ccfit2-5.1.3/ccfit2.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-06-28 13:09:09.000000 ccfit2-5.1.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 13:09:39.870360 ccfit2-5.1.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1544 2023-06-28 13:09:37.000000 ccfit2-5.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:09:32.286707 ccfit2-5.1.4/
+-rw-rw-rw-   0 root         (0) root         (0)    35075 2023-07-06 12:09:02.000000 ccfit2-5.1.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-07-06 12:09:32.286707 ccfit2-5.1.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      501 2023-07-06 12:09:02.000000 ccfit2-5.1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:09:32.284717 ccfit2-5.1.4/ccfit2/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-06 12:09:02.000000 ccfit2-5.1.4/ccfit2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-07-06 12:09:29.000000 ccfit2-5.1.4/ccfit2/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)   132412 2023-07-06 12:09:02.000000 ccfit2-5.1.4/ccfit2/ac.py
+-rw-rw-rw-   0 root         (0) root         (0)    69815 2023-07-06 12:09:02.000000 ccfit2-5.1.4/ccfit2/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    61138 2023-07-06 12:09:02.000000 ccfit2-5.1.4/ccfit2/dc.py
+-rw-rw-rw-   0 root         (0) root         (0)    23311 2023-07-06 12:09:02.000000 ccfit2-5.1.4/ccfit2/gui.py
+-rw-rw-rw-   0 root         (0) root         (0)   171346 2023-07-06 12:09:02.000000 ccfit2-5.1.4/ccfit2/relaxation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1756 2023-07-06 12:09:02.000000 ccfit2-5.1.4/ccfit2/stats.py
+-rw-rw-rw-   0 root         (0) root         (0)    10668 2023-07-06 12:09:02.000000 ccfit2-5.1.4/ccfit2/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    21023 2023-07-06 12:09:02.000000 ccfit2-5.1.4/ccfit2/waveform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:09:32.286707 ccfit2-5.1.4/ccfit2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-07-06 12:09:32.000000 ccfit2-5.1.4/ccfit2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      390 2023-07-06 12:09:32.000000 ccfit2-5.1.4/ccfit2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 12:09:32.000000 ccfit2-5.1.4/ccfit2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       95 2023-07-06 12:09:32.000000 ccfit2-5.1.4/ccfit2.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      133 2023-07-06 12:09:32.000000 ccfit2-5.1.4/ccfit2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-06 12:09:32.000000 ccfit2-5.1.4/ccfit2.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-07-06 12:09:02.000000 ccfit2-5.1.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 12:09:32.286707 ccfit2-5.1.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1544 2023-07-06 12:09:29.000000 ccfit2-5.1.4/setup.py
```

### Comparing `ccfit2-5.1.3/LICENSE` & `ccfit2-5.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ccfit2-5.1.3/PKG-INFO` & `ccfit2-5.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccfit2
-Version: 5.1.3
+Version: 5.1.4
 Summary: CCFIT2 is a program for fitting AC and DC magnetisation data
 Home-page: https://gitlab.com/chilton-group/cc-fit2
 Author: Daniel Reta
 Author-email: danielreta1@gmail.com
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/cc-fit2/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/cc-fit2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ccfit2-5.1.3/ccfit2/ac.py` & `ccfit2-5.1.4/ccfit2/ac.py`

 * *Files 0% similar despite different names*

```diff
@@ -2592,15 +2592,15 @@
         try:
             s = float(s.strip())
             if s < 0:
                 # print(
                 #   f'Negative Susceptibility {s} emu, skipping'
                 # )
                 s = np.NaN
-        except TypeError:
+        except (TypeError, ValueError):
             s = np.NaN
 
         return s
 
     @classmethod
     def from_file(cls, file: str, mass: float, mw: float,
                   header_indices: dict | str = 'find',
```

### Comparing `ccfit2-5.1.3/ccfit2/cli.py` & `ccfit2-5.1.4/ccfit2/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -955,30 +955,38 @@
             print('Fixed parameters are:')
             print(model.fix_vars)
             print()
         # Fit model
         model.fit_to(experiment)
 
         # Plot decay with fit
-        if uargs.decay_plots in ['on', 'show', 'save']:
-            file_name = 'fitted_decay_{:.2f}K_{:.1f}Oe{}'.format(
-                experiment.rep_temperature,
-                experiment.dc_fields[-1],
-                PFF
-            )
+        if model.fit_status:
+            if uargs.decay_plots in ['on', 'show', 'save']:
+                file_name = 'fitted_decay_{:.2f}K_{:.1f}Oe{}'.format(
+                    experiment.rep_temperature,
+                    experiment.dc_fields[-1],
+                    PFF
+                )
 
-            file_name = os.path.join(user_cfg.results_dir, file_name)
-            dc.plot_fitted_decay(
-                experiment=experiment, model=model,
-                show=_SHOW_CONV[uargs.decay_plots],
-                save=_SAVE_CONV[uargs.decay_plots],
-                save_name=file_name, x_scale=uargs.plot_axes[0],
-                y_scale=uargs.plot_axes[1],
-                show_params=uargs.hide_params
-            )
+                file_name = os.path.join(user_cfg.results_dir, file_name)
+                dc.plot_fitted_decay(
+                    experiment=experiment, model=model,
+                    show=_SHOW_CONV[uargs.decay_plots],
+                    save=_SAVE_CONV[uargs.decay_plots],
+                    save_name=file_name, x_scale=uargs.plot_axes[0],
+                    y_scale=uargs.plot_axes[1],
+                    show_params=uargs.hide_params
+                )
+        else:
+            ut.cprint(
+                        '\n Cannot save/show plot fot T = {} K and {} Oe as fit has failed'.format( # noqa
+                            model.temperature, model.dc_field
+                        ),
+                        'black_yellowbg'
+                )
 
     base_filename = 'dc_{}_'.format(model.NAME.lower().replace(' ', '_'))
     base_filename = os.path.join(user_cfg.results_dir, base_filename)
 
     # Save parameters to file
     dc.write_model_params(
         models,
```

### Comparing `ccfit2-5.1.3/ccfit2/dc.py` & `ccfit2-5.1.4/ccfit2/dc.py`

 * *Files 0% similar despite different names*

```diff
@@ -872,16 +872,16 @@
         self.temperature = experiment.rep_temperature
         self.dc_field = experiment.dc_fields[-1]
         self.meas_dc_field = experiment.meas_dc_fields[-1]
 
         if curr_fit.status == 0:
             if verbose:
                 ut.cprint(
-                    '\n Fit at {} K failed - Too many iterations'.format(
-                        self.temperature
+                    '\n Fit at {} K and {} Oe failed - Too many iterations'.format( # noqa
+                        self.temperature, self.dc_field
                     ),
                     'black_yellowbg'
                 )
 
             # Set fitted values
             self.final_var_values = {
                 name: value
```

### Comparing `ccfit2-5.1.3/ccfit2/gui.py` & `ccfit2-5.1.4/ccfit2/gui.py`

 * *Files identical despite different names*

### Comparing `ccfit2-5.1.3/ccfit2/relaxation.py` & `ccfit2-5.1.4/ccfit2/relaxation.py`

 * *Files 0% similar despite different names*

```diff
@@ -5937,4773 +5937,4774 @@
 00017300: 0a20 2020 2020 2020 2027 4427 3a20 7227  .        'D': r'
 00017310: 733c 7375 703e 2d31 3c2f 7375 703e 204b  s<sup>-1</sup> K
 00017320: 3c73 7570 3e2d 313c 2f73 7570 3e27 0a20  <sup>-1</sup>'. 
 00017330: 2020 207d 0a0a 2020 2020 233a 204d 6f64     }..    #: Mod
 00017340: 656c 2070 6172 616d 6574 6572 2062 6f75  el parameter bou
 00017350: 6e64 730a 2020 2020 424f 554e 4453 203d  nds.    BOUNDS =
 00017360: 207b 0a20 2020 2020 2020 2027 4427 3a20   {.        'D': 
-00017370: 5b2d 3330 2c20 302e 5d0a 2020 2020 7d0a  [-30, 0.].    }.
-00017380: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
-00017390: 6f64 0a20 2020 2064 6566 2073 6574 5f69  od.    def set_i
-000173a0: 6e69 7469 616c 5f76 616c 7328 7061 7261  nitial_vals(para
-000173b0: 6d5f 6469 6374 3a20 6469 6374 5b73 7472  m_dict: dict[str
-000173c0: 2c20 7374 7220 7c20 666c 6f61 745d 2920  , str | float]) 
-000173d0: 2d3e 2064 6963 745b 7374 722c 2066 6c6f  -> dict[str, flo
-000173e0: 6174 5d3a 2023 206e 6f71 610a 2020 2020  at]: # noqa.    
-000173f0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-00017400: 5365 7473 2067 7565 7373 2076 616c 7565  Sets guess value
-00017410: 7320 666f 7220 7061 7261 6d65 7465 7273  s for parameters
-00017420: 2069 6620 7265 7175 6573 7465 6420 6279   if requested by
-00017430: 2075 7365 720a 0a20 2020 2020 2020 2050   user..        P
-00017440: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-00017450: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-00017460: 2020 2020 2070 6172 616d 5f64 6963 743a       param_dict:
-00017470: 2064 6963 745b 7374 722c 2073 7472 207c   dict[str, str |
-00017480: 2066 6c6f 6174 5d0a 2020 2020 2020 2020   float].        
-00017490: 2020 2020 4b65 7973 2061 7265 2066 6974      Keys are fit
-000174a0: 2f66 6978 2070 6172 616d 6574 6572 206e  /fix parameter n
-000174b0: 616d 6573 2028 7365 6520 636c 6173 732e  ames (see class.
-000174c0: 5041 524e 414d 4553 295c 6e0a 2020 2020  PARNAMES)\n.    
-000174d0: 2020 2020 2020 2020 5661 6c75 6573 2061          Values a
-000174e0: 7265 2065 6974 6865 7220 666c 6f61 7420  re either float 
-000174f0: 2861 6374 7561 6c20 7661 6c75 6529 206f  (actual value) o
-00017500: 7220 7468 6520 7374 7269 6e67 2027 6775  r the string 'gu
-00017510: 6573 7327 0a0a 2020 2020 2020 2020 5265  ess'..        Re
-00017520: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
-00017530: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6469  -----.        di
-00017540: 6374 5b73 7472 2c20 666c 6f61 745d 0a20  ct[str, float]. 
-00017550: 2020 2020 2020 2020 2020 204b 6579 7320             Keys 
-00017560: 6172 6520 6669 742f 6669 7820 7061 7261  are fit/fix para
-00017570: 6d65 7465 7220 6e61 6d65 7320 2873 6565  meter names (see
-00017580: 2063 6c61 7373 2e50 4152 4e41 4d45 5329   class.PARNAMES)
-00017590: 5c6e 0a20 2020 2020 2020 2020 2020 2056  \n.            V
-000175a0: 616c 7565 7320 6172 6520 666c 6f61 7420  alues are float 
-000175b0: 2861 6374 7561 6c20 7661 6c75 6529 2077  (actual value) w
-000175c0: 6869 6368 2061 7265 2069 6e69 7469 616c  hich are initial
-000175d0: 2076 616c 7565 7320 6f66 0a20 2020 2020   values of.     
-000175e0: 2020 2020 2020 2070 6172 616d 6574 6572         parameter
-000175f0: 0a20 2020 2020 2020 2027 2727 0a0a 2020  .        '''..  
-00017600: 2020 2020 2020 2320 4d61 6b65 2063 6f70        # Make cop
-00017610: 792c 2061 6e79 2073 7472 2076 616c 7565  y, any str value
-00017620: 7320 7769 6c6c 2062 6520 7265 706c 6163  s will be replac
-00017630: 6564 0a20 2020 2020 2020 206e 6577 5f70  ed.        new_p
-00017640: 6172 616d 5f64 6963 7420 3d20 636f 7079  aram_dict = copy
-00017650: 2e63 6f70 7928 7061 7261 6d5f 6469 6374  .copy(param_dict
-00017660: 290a 0a20 2020 2020 2020 2023 2047 7565  )..        # Gue
-00017670: 7373 6573 0a20 2020 2020 2020 2067 7565  sses.        gue
-00017680: 7373 6469 6374 203d 207b 0a20 2020 2020  ssdict = {.     
-00017690: 2020 2020 2020 2027 4427 3a20 2d32 0a20         'D': -2. 
-000176a0: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
-000176b0: 2020 2320 5265 706c 6163 6520 2767 7565    # Replace 'gue
-000176c0: 7373 2720 7769 7468 2072 656c 6576 616e  ss' with relevan
-000176d0: 7420 6775 6573 730a 2020 2020 2020 2020  t guess.        
-000176e0: 666f 7220 7661 722c 2076 616c 2069 6e20  for var, val in 
-000176f0: 7061 7261 6d5f 6469 6374 2e69 7465 6d73  param_dict.items
-00017700: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00017710: 6966 2076 616c 203d 3d20 2767 7565 7373  if val == 'guess
-00017720: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
-00017730: 2020 206e 6577 5f70 6172 616d 5f64 6963     new_param_dic
-00017740: 745b 7661 725d 203d 2067 7565 7373 6469  t[var] = guessdi
-00017750: 6374 5b76 6172 5d0a 0a20 2020 2020 2020  ct[var]..       
-00017760: 2072 6574 7572 6e20 6e65 775f 7061 7261   return new_para
-00017770: 6d5f 6469 6374 0a0a 2020 2020 4073 7461  m_dict..    @sta
-00017780: 7469 636d 6574 686f 640a 2020 2020 6465  ticmethod.    de
-00017790: 6620 6d6f 6465 6c28 7061 7261 6d65 7465  f model(paramete
-000177a0: 7273 3a20 6469 6374 5b73 7472 2c20 666c  rs: dict[str, fl
-000177b0: 6f61 745d 2c0a 2020 2020 2020 2020 2020  oat],.          
-000177c0: 2020 2020 7465 6d70 6572 6174 7572 6573      temperatures
-000177d0: 3a20 6e70 742e 4172 7261 794c 696b 6529  : npt.ArrayLike)
-000177e0: 202d 3e20 6e70 742e 4e44 4172 7261 793a   -> npt.NDArray:
-000177f0: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-00017800: 2020 2020 2045 7661 6c75 6174 6573 206c       Evaluates l
-00017810: 6f67 3130 2844 6972 6563 7429 206d 6f64  og10(Direct) mod
-00017820: 656c 206f 6620 6c6f 6731 3028 7265 6c61  el of log10(rela
-00017830: 7861 7469 6f6e 2072 6174 6529 0a20 2020  xation rate).   
-00017840: 2020 2020 2075 7369 6e67 2070 726f 7669       using provi
-00017850: 6465 6420 7061 7261 6d65 7465 7220 616e  ded parameter an
-00017860: 6420 7465 6d70 6572 6174 7572 6520 7661  d temperature va
-00017870: 6c75 6573 2e0a 0a20 2020 2020 2020 2050  lues...        P
-00017880: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-00017890: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-000178a0: 2020 2020 2070 6172 616d 6574 6572 733a       parameters:
-000178b0: 2064 6963 745b 7374 722c 2066 6c6f 6174   dict[str, float
-000178c0: 5d0a 2020 2020 2020 2020 2020 2020 5061  ].            Pa
-000178d0: 7261 6d65 7465 7273 2074 6f20 7573 6520  rameters to use 
-000178e0: 696e 206d 6f64 656c 2066 756e 6374 696f  in model functio
-000178f0: 6e2c 206b 6579 7320 6172 6520 6769 7665  n, keys are give
-00017900: 6e20 696e 0a20 2020 2020 2020 2020 2020  n in.           
-00017910: 2063 6c61 7373 2e50 4152 4e41 4d45 530a   class.PARNAMES.
-00017920: 2020 2020 2020 2020 7465 6d70 6572 6174          temperat
-00017930: 7572 6573 3a20 6172 7261 795f 6c69 6b65  ures: array_like
-00017940: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
-00017950: 7065 7261 7475 7265 2076 616c 7565 7320  perature values 
-00017960: 284b 2920 6174 2077 6869 6368 206d 6f64  (K) at which mod
-00017970: 656c 2066 756e 6374 696f 6e20 6973 2065  el function is e
-00017980: 7661 6c75 6174 6564 0a0a 2020 2020 2020  valuated..      
-00017990: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
-000179a0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
-000179b0: 2020 6e64 6172 7261 7920 6f66 2066 6c6f    ndarray of flo
-000179c0: 6174 730a 2020 2020 2020 2020 2020 2020  ats.            
-000179d0: 6c6f 6731 3028 5265 6c61 7861 7469 6f6e  log10(Relaxation
-000179e0: 2072 6174 6529 2061 7320 6120 6675 6e63   rate) as a func
-000179f0: 7469 6f6e 206f 6620 7465 6d70 6572 6174  tion of temperat
-00017a00: 7572 650a 0a20 2020 2020 2020 2027 2727  ure..        '''
-00017a10: 0a0a 2020 2020 2020 2020 6420 3d20 7061  ..        d = pa
-00017a20: 7261 6d65 7465 7273 5b27 4427 5d0a 0a20  rameters['D'].. 
-00017a30: 2020 2020 2020 206c 6f67 7261 7465 203d         lograte =
-00017a40: 206e 702e 6c6f 6731 3028 3130 2a2a 6420   np.log10(10**d 
-00017a50: 2a20 6e70 2e61 7361 7272 6179 2874 656d  * np.asarray(tem
-00017a60: 7065 7261 7475 7265 7329 290a 0a20 2020  peratures))..   
-00017a70: 2020 2020 2072 6574 7572 6e20 6c6f 6772       return logr
-00017a80: 6174 650a 0a0a 636c 6173 7320 4d75 6c74  ate...class Mult
-00017a90: 694c 6f67 5461 7554 4d6f 6465 6c28 293a  iLogTauTModel():
-00017aa0: 0a20 2020 2027 2727 0a20 2020 2054 616b  .    '''.    Tak
-00017ab0: 6573 206d 756c 7469 706c 6520 4c6f 6754  es multiple LogT
-00017ac0: 6175 544d 6f64 656c 206f 626a 6563 7473  auTModel objects
-00017ad0: 2061 6e64 2063 6f6d 6269 6e65 7320 696e   and combines in
-00017ae0: 746f 2061 2073 696e 676c 6520 6f62 6a65  to a single obje
-00017af0: 6374 0a0a 2020 2020 5061 7261 6d65 7465  ct..    Paramete
-00017b00: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-00017b10: 2d0a 2020 2020 6669 745f 7661 7273 3a20  -.    fit_vars: 
-00017b20: 6c69 7374 5b64 6963 745b 7374 722c 2066  list[dict[str, f
-00017b30: 6c6f 6174 207c 2073 7472 5d5d 0a20 2020  loat | str]].   
-00017b40: 2020 2020 204c 6973 7420 6f66 2066 6974       List of fit
-00017b50: 2064 6963 7473 2c20 7769 7468 206b 6579   dicts, with key
-00017b60: 7320 6173 2050 4152 4e41 4d45 5320 6f66  s as PARNAMES of
-00017b70: 2065 6163 6820 4c6f 6754 6175 544d 6f64   each LogTauTMod
-00017b80: 656c 0a20 2020 2020 2020 2061 6e64 2076  el.        and v
-00017b90: 616c 7565 7320 6173 2065 6974 6865 7220  alues as either 
-00017ba0: 7468 6520 7374 7269 6e67 2027 6775 6573  the string 'gues
-00017bb0: 7327 206f 7220 6120 666c 6f61 7420 7661  s' or a float va
-00017bc0: 6c75 650a 2020 2020 6669 785f 7661 7273  lue.    fix_vars
-00017bd0: 3a20 6c69 7374 5b64 6963 745b 7374 722c  : list[dict[str,
-00017be0: 2066 6c6f 6174 207c 2073 7472 5d5d 0a20   float | str]]. 
-00017bf0: 2020 2020 2020 204c 6973 7420 6f66 2066         List of f
-00017c00: 6978 2064 6963 7473 2c20 7769 7468 206b  ix dicts, with k
-00017c10: 6579 7320 6173 2050 4152 4e41 4d45 5320  eys as PARNAMES 
-00017c20: 6f66 2065 6163 6820 4c6f 6754 6175 544d  of each LogTauTM
-00017c30: 6f64 656c 0a20 2020 2020 2020 2061 6e64  odel.        and
-00017c40: 2076 616c 7565 7320 6173 2065 6974 6865   values as eithe
-00017c50: 7220 7468 6520 7374 7269 6e67 2027 6775  r the string 'gu
-00017c60: 6573 7327 206f 7220 6120 666c 6f61 7420  ess' or a float 
-00017c70: 7661 6c75 650a 2020 2020 6c6f 676d 6f64  value.    logmod
-00017c80: 656c 733a 206c 6973 745b 4c6f 6754 6175  els: list[LogTau
-00017c90: 544d 6f64 656c 5d0a 2020 2020 2020 2020  TModel].        
-00017ca0: 4c69 7374 206f 6620 756e 696e 7374 616e  List of uninstan
-00017cb0: 7469 6174 6564 204c 6f67 5461 7554 4d6f  tiated LogTauTMo
-00017cc0: 6465 6c20 6f62 6a65 6374 730a 0a20 2020  del objects..   
-00017cd0: 2041 7474 7269 6275 7465 730a 2020 2020   Attributes.    
-00017ce0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 206c  ----------.    l
-00017cf0: 6f67 6d6f 6465 6c73 3a20 6c69 7374 5b4c  ogmodels: list[L
-00017d00: 6f67 5461 7554 4d6f 6465 6c5d 0a20 2020  ogTauTModel].   
-00017d10: 2020 2020 204c 6973 7420 6f66 204c 6f67       List of Log
-00017d20: 5461 7554 4d6f 6465 6c20 6f62 6a65 6374  TauTModel object
-00017d30: 730a 2020 2020 4e41 4d45 3a20 7374 720a  s.    NAME: str.
-00017d40: 2020 2020 2020 2020 4e61 6d65 7320 6f66          Names of
-00017d50: 2065 6163 6820 4c6f 6754 6175 544d 6f64   each LogTauTMod
-00017d60: 656c 2063 6f6e 6361 7465 6e61 7465 640a  el concatenated.
-00017d70: 2020 2020 2727 270a 0a20 2020 2064 6566      '''..    def
-00017d80: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-00017d90: 6c6f 676d 6f64 656c 733a 206c 6973 745b  logmodels: list[
-00017da0: 4c6f 6754 6175 544d 6f64 656c 5d2c 0a20  LogTauTModel],. 
-00017db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017dc0: 6669 745f 7661 7273 3a20 6c69 7374 5b64  fit_vars: list[d
-00017dd0: 6963 745b 7374 722c 2066 6c6f 6174 207c  ict[str, float |
-00017de0: 2073 7472 5d5d 2c0a 2020 2020 2020 2020   str]],.        
-00017df0: 2020 2020 2020 2020 2066 6978 5f76 6172           fix_var
-00017e00: 733a 206c 6973 745b 6469 6374 5b73 7472  s: list[dict[str
-00017e10: 2c20 666c 6f61 7420 7c20 7374 725d 5d29  , float | str]])
-00017e20: 202d 3e20 4e6f 6e65 3a0a 0a20 2020 2020   -> None:..     
-00017e30: 2020 2023 2049 6e73 7461 6e74 6961 7465     # Instantiate
-00017e40: 2065 6163 6820 6c6f 676d 6f64 656c 2061   each logmodel a
-00017e50: 6e64 2063 7265 6174 6520 6c69 7374 206f  nd create list o
-00017e60: 6620 696e 7374 616e 7469 6174 6564 206c  f instantiated l
-00017e70: 6f67 6d6f 6465 6c73 0a20 2020 2020 2020  ogmodels.       
-00017e80: 2073 656c 662e 6c6f 676d 6f64 656c 7320   self.logmodels 
-00017e90: 3d20 7365 6c66 2e70 726f 6365 7373 5f66  = self.process_f
-00017ea0: 6974 6669 7828 6669 745f 7661 7273 2c20  itfix(fit_vars, 
-00017eb0: 6669 785f 7661 7273 2c20 6c6f 676d 6f64  fix_vars, logmod
-00017ec0: 656c 7329 0a0a 2020 2020 2020 2020 7365  els)..        se
-00017ed0: 6c66 2e4e 414d 4520 3d20 5b6c 6f67 6d6f  lf.NAME = [logmo
-00017ee0: 6465 6c2e 4e41 4d45 2066 6f72 206c 6f67  del.NAME for log
-00017ef0: 6d6f 6465 6c20 696e 206c 6f67 6d6f 6465  model in logmode
-00017f00: 6c73 5d0a 2020 2020 2020 2020 7365 6c66  ls].        self
-00017f10: 2e4e 414d 4520 3d20 2727 2e6a 6f69 6e28  .NAME = ''.join(
-00017f20: 5b27 7b7d 2b27 2e66 6f72 6d61 7428 6e61  ['{}+'.format(na
-00017f30: 6d65 2920 666f 7220 6e61 6d65 2069 6e20  me) for name in 
-00017f40: 7365 6c66 2e4e 414d 455d 295b 3a2d 315d  self.NAME])[:-1]
-00017f50: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-00017f60: 6669 745f 7374 6174 7573 203d 2046 616c  fit_status = Fal
-00017f70: 7365 0a0a 2020 2020 2020 2020 7265 7475  se..        retu
-00017f80: 726e 0a0a 2020 2020 4070 726f 7065 7274  rn..    @propert
-00017f90: 790a 2020 2020 6465 6620 6669 745f 7374  y.    def fit_st
-00017fa0: 6174 7573 2873 656c 6629 202d 3e20 626f  atus(self) -> bo
-00017fb0: 6f6c 3a0a 2020 2020 2020 2020 2754 7275  ol:.        'Tru
-00017fc0: 6520 6966 2066 6974 2073 7563 6365 7373  e if fit success
-00017fd0: 6675 6c2c 2065 6c73 6520 4661 6c73 6527  ful, else False'
-00017fe0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00017ff0: 7365 6c66 2e5f 6669 745f 7374 6174 7573  self._fit_status
-00018000: 0a0a 2020 2020 4066 6974 5f73 7461 7475  ..    @fit_statu
-00018010: 732e 7365 7474 6572 0a20 2020 2064 6566  s.setter.    def
-00018020: 2066 6974 5f73 7461 7475 7328 7365 6c66   fit_status(self
-00018030: 2c20 7661 6c75 6529 3a0a 2020 2020 2020  , value):.      
-00018040: 2020 6966 2074 7970 6528 7661 6c75 6529    if type(value)
-00018050: 203d 3d20 626f 6f6c 3a0a 2020 2020 2020   == bool:.      
-00018060: 2020 2020 2020 7365 6c66 2e5f 6669 745f        self._fit_
-00018070: 7374 6174 7573 203d 2076 616c 7565 0a20  status = value. 
-00018080: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00018090: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
-000180a0: 7970 6545 7272 6f72 0a20 2020 2020 2020  ypeError.       
-000180b0: 2072 6574 7572 6e0a 0a20 2020 2040 7374   return..    @st
-000180c0: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
-000180d0: 6566 2070 726f 6365 7373 5f66 6974 6669  ef process_fitfi
-000180e0: 7828 6669 745f 7661 7273 3a20 6c69 7374  x(fit_vars: list
-000180f0: 5b64 6963 745b 7374 722c 2066 6c6f 6174  [dict[str, float
-00018100: 207c 2073 7472 5d5d 2c0a 2020 2020 2020   | str]],.      
+00017370: 5b2d 3330 2c20 6e70 2e69 6e66 5d0a 2020  [-30, np.inf].  
+00017380: 2020 7d0a 0a20 2020 2040 7374 6174 6963    }..    @static
+00017390: 6d65 7468 6f64 0a20 2020 2064 6566 2073  method.    def s
+000173a0: 6574 5f69 6e69 7469 616c 5f76 616c 7328  et_initial_vals(
+000173b0: 7061 7261 6d5f 6469 6374 3a20 6469 6374  param_dict: dict
+000173c0: 5b73 7472 2c20 7374 7220 7c20 666c 6f61  [str, str | floa
+000173d0: 745d 2920 2d3e 2064 6963 745b 7374 722c  t]) -> dict[str,
+000173e0: 2066 6c6f 6174 5d3a 2023 206e 6f71 610a   float]: # noqa.
+000173f0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+00017400: 2020 2020 5365 7473 2067 7565 7373 2076      Sets guess v
+00017410: 616c 7565 7320 666f 7220 7061 7261 6d65  alues for parame
+00017420: 7465 7273 2069 6620 7265 7175 6573 7465  ters if requeste
+00017430: 6420 6279 2075 7365 720a 0a20 2020 2020  d by user..     
+00017440: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00017450: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+00017460: 0a20 2020 2020 2020 2070 6172 616d 5f64  .        param_d
+00017470: 6963 743a 2064 6963 745b 7374 722c 2073  ict: dict[str, s
+00017480: 7472 207c 2066 6c6f 6174 5d0a 2020 2020  tr | float].    
+00017490: 2020 2020 2020 2020 4b65 7973 2061 7265          Keys are
+000174a0: 2066 6974 2f66 6978 2070 6172 616d 6574   fit/fix paramet
+000174b0: 6572 206e 616d 6573 2028 7365 6520 636c  er names (see cl
+000174c0: 6173 732e 5041 524e 414d 4553 295c 6e0a  ass.PARNAMES)\n.
+000174d0: 2020 2020 2020 2020 2020 2020 5661 6c75              Valu
+000174e0: 6573 2061 7265 2065 6974 6865 7220 666c  es are either fl
+000174f0: 6f61 7420 2861 6374 7561 6c20 7661 6c75  oat (actual valu
+00017500: 6529 206f 7220 7468 6520 7374 7269 6e67  e) or the string
+00017510: 2027 6775 6573 7327 0a0a 2020 2020 2020   'guess'..      
+00017520: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+00017530: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+00017540: 2020 6469 6374 5b73 7472 2c20 666c 6f61    dict[str, floa
+00017550: 745d 0a20 2020 2020 2020 2020 2020 204b  t].            K
+00017560: 6579 7320 6172 6520 6669 742f 6669 7820  eys are fit/fix 
+00017570: 7061 7261 6d65 7465 7220 6e61 6d65 7320  parameter names 
+00017580: 2873 6565 2063 6c61 7373 2e50 4152 4e41  (see class.PARNA
+00017590: 4d45 5329 5c6e 0a20 2020 2020 2020 2020  MES)\n.         
+000175a0: 2020 2056 616c 7565 7320 6172 6520 666c     Values are fl
+000175b0: 6f61 7420 2861 6374 7561 6c20 7661 6c75  oat (actual valu
+000175c0: 6529 2077 6869 6368 2061 7265 2069 6e69  e) which are ini
+000175d0: 7469 616c 2076 616c 7565 7320 6f66 0a20  tial values of. 
+000175e0: 2020 2020 2020 2020 2020 2070 6172 616d             param
+000175f0: 6574 6572 0a20 2020 2020 2020 2027 2727  eter.        '''
+00017600: 0a0a 2020 2020 2020 2020 2320 4d61 6b65  ..        # Make
+00017610: 2063 6f70 792c 2061 6e79 2073 7472 2076   copy, any str v
+00017620: 616c 7565 7320 7769 6c6c 2062 6520 7265  alues will be re
+00017630: 706c 6163 6564 0a20 2020 2020 2020 206e  placed.        n
+00017640: 6577 5f70 6172 616d 5f64 6963 7420 3d20  ew_param_dict = 
+00017650: 636f 7079 2e63 6f70 7928 7061 7261 6d5f  copy.copy(param_
+00017660: 6469 6374 290a 0a20 2020 2020 2020 2023  dict)..        #
+00017670: 2047 7565 7373 6573 0a20 2020 2020 2020   Guesses.       
+00017680: 2067 7565 7373 6469 6374 203d 207b 0a20   guessdict = {. 
+00017690: 2020 2020 2020 2020 2020 2027 4427 3a20             'D': 
+000176a0: 2d32 0a20 2020 2020 2020 207d 0a0a 2020  -2.        }..  
+000176b0: 2020 2020 2020 2320 5265 706c 6163 6520        # Replace 
+000176c0: 2767 7565 7373 2720 7769 7468 2072 656c  'guess' with rel
+000176d0: 6576 616e 7420 6775 6573 730a 2020 2020  evant guess.    
+000176e0: 2020 2020 666f 7220 7661 722c 2076 616c      for var, val
+000176f0: 2069 6e20 7061 7261 6d5f 6469 6374 2e69   in param_dict.i
+00017700: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
+00017710: 2020 2020 6966 2076 616c 203d 3d20 2767      if val == 'g
+00017720: 7565 7373 273a 0a20 2020 2020 2020 2020  uess':.         
+00017730: 2020 2020 2020 206e 6577 5f70 6172 616d         new_param
+00017740: 5f64 6963 745b 7661 725d 203d 2067 7565  _dict[var] = gue
+00017750: 7373 6469 6374 5b76 6172 5d0a 0a20 2020  ssdict[var]..   
+00017760: 2020 2020 2072 6574 7572 6e20 6e65 775f       return new_
+00017770: 7061 7261 6d5f 6469 6374 0a0a 2020 2020  param_dict..    
+00017780: 4073 7461 7469 636d 6574 686f 640a 2020  @staticmethod.  
+00017790: 2020 6465 6620 6d6f 6465 6c28 7061 7261    def model(para
+000177a0: 6d65 7465 7273 3a20 6469 6374 5b73 7472  meters: dict[str
+000177b0: 2c20 666c 6f61 745d 2c0a 2020 2020 2020  , float],.      
+000177c0: 2020 2020 2020 2020 7465 6d70 6572 6174          temperat
+000177d0: 7572 6573 3a20 6e70 742e 4172 7261 794c  ures: npt.ArrayL
+000177e0: 696b 6529 202d 3e20 6e70 742e 4e44 4172  ike) -> npt.NDAr
+000177f0: 7261 793a 0a20 2020 2020 2020 2027 2727  ray:.        '''
+00017800: 0a20 2020 2020 2020 2045 7661 6c75 6174  .        Evaluat
+00017810: 6573 206c 6f67 3130 2844 6972 6563 7429  es log10(Direct)
+00017820: 206d 6f64 656c 206f 6620 6c6f 6731 3028   model of log10(
+00017830: 7265 6c61 7861 7469 6f6e 2072 6174 6529  relaxation rate)
+00017840: 0a20 2020 2020 2020 2075 7369 6e67 2070  .        using p
+00017850: 726f 7669 6465 6420 7061 7261 6d65 7465  rovided paramete
+00017860: 7220 616e 6420 7465 6d70 6572 6174 7572  r and temperatur
+00017870: 6520 7661 6c75 6573 2e0a 0a20 2020 2020  e values...     
+00017880: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00017890: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+000178a0: 0a20 2020 2020 2020 2070 6172 616d 6574  .        paramet
+000178b0: 6572 733a 2064 6963 745b 7374 722c 2066  ers: dict[str, f
+000178c0: 6c6f 6174 5d0a 2020 2020 2020 2020 2020  loat].          
+000178d0: 2020 5061 7261 6d65 7465 7273 2074 6f20    Parameters to 
+000178e0: 7573 6520 696e 206d 6f64 656c 2066 756e  use in model fun
+000178f0: 6374 696f 6e2c 206b 6579 7320 6172 6520  ction, keys are 
+00017900: 6769 7665 6e20 696e 0a20 2020 2020 2020  given in.       
+00017910: 2020 2020 2063 6c61 7373 2e50 4152 4e41       class.PARNA
+00017920: 4d45 530a 2020 2020 2020 2020 7465 6d70  MES.        temp
+00017930: 6572 6174 7572 6573 3a20 6172 7261 795f  eratures: array_
+00017940: 6c69 6b65 0a20 2020 2020 2020 2020 2020  like.           
+00017950: 2074 656d 7065 7261 7475 7265 2076 616c   temperature val
+00017960: 7565 7320 284b 2920 6174 2077 6869 6368  ues (K) at which
+00017970: 206d 6f64 656c 2066 756e 6374 696f 6e20   model function 
+00017980: 6973 2065 7661 6c75 6174 6564 0a0a 2020  is evaluated..  
+00017990: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
+000179a0: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
+000179b0: 2020 2020 2020 6e64 6172 7261 7920 6f66        ndarray of
+000179c0: 2066 6c6f 6174 730a 2020 2020 2020 2020   floats.        
+000179d0: 2020 2020 6c6f 6731 3028 5265 6c61 7861      log10(Relaxa
+000179e0: 7469 6f6e 2072 6174 6529 2061 7320 6120  tion rate) as a 
+000179f0: 6675 6e63 7469 6f6e 206f 6620 7465 6d70  function of temp
+00017a00: 6572 6174 7572 650a 0a20 2020 2020 2020  erature..       
+00017a10: 2027 2727 0a0a 2020 2020 2020 2020 6420   '''..        d 
+00017a20: 3d20 7061 7261 6d65 7465 7273 5b27 4427  = parameters['D'
+00017a30: 5d0a 0a20 2020 2020 2020 206c 6f67 7261  ]..        logra
+00017a40: 7465 203d 206e 702e 6c6f 6731 3028 3130  te = np.log10(10
+00017a50: 2a2a 6420 2a20 6e70 2e61 7361 7272 6179  **d * np.asarray
+00017a60: 2874 656d 7065 7261 7475 7265 7329 290a  (temperatures)).
+00017a70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00017a80: 6c6f 6772 6174 650a 0a0a 636c 6173 7320  lograte...class 
+00017a90: 4d75 6c74 694c 6f67 5461 7554 4d6f 6465  MultiLogTauTMode
+00017aa0: 6c28 293a 0a20 2020 2027 2727 0a20 2020  l():.    '''.   
+00017ab0: 2054 616b 6573 206d 756c 7469 706c 6520   Takes multiple 
+00017ac0: 4c6f 6754 6175 544d 6f64 656c 206f 626a  LogTauTModel obj
+00017ad0: 6563 7473 2061 6e64 2063 6f6d 6269 6e65  ects and combine
+00017ae0: 7320 696e 746f 2061 2073 696e 676c 6520  s into a single 
+00017af0: 6f62 6a65 6374 0a0a 2020 2020 5061 7261  object..    Para
+00017b00: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
+00017b10: 2d2d 2d2d 2d0a 2020 2020 6669 745f 7661  -----.    fit_va
+00017b20: 7273 3a20 6c69 7374 5b64 6963 745b 7374  rs: list[dict[st
+00017b30: 722c 2066 6c6f 6174 207c 2073 7472 5d5d  r, float | str]]
+00017b40: 0a20 2020 2020 2020 204c 6973 7420 6f66  .        List of
+00017b50: 2066 6974 2064 6963 7473 2c20 7769 7468   fit dicts, with
+00017b60: 206b 6579 7320 6173 2050 4152 4e41 4d45   keys as PARNAME
+00017b70: 5320 6f66 2065 6163 6820 4c6f 6754 6175  S of each LogTau
+00017b80: 544d 6f64 656c 0a20 2020 2020 2020 2061  TModel.        a
+00017b90: 6e64 2076 616c 7565 7320 6173 2065 6974  nd values as eit
+00017ba0: 6865 7220 7468 6520 7374 7269 6e67 2027  her the string '
+00017bb0: 6775 6573 7327 206f 7220 6120 666c 6f61  guess' or a floa
+00017bc0: 7420 7661 6c75 650a 2020 2020 6669 785f  t value.    fix_
+00017bd0: 7661 7273 3a20 6c69 7374 5b64 6963 745b  vars: list[dict[
+00017be0: 7374 722c 2066 6c6f 6174 207c 2073 7472  str, float | str
+00017bf0: 5d5d 0a20 2020 2020 2020 204c 6973 7420  ]].        List 
+00017c00: 6f66 2066 6978 2064 6963 7473 2c20 7769  of fix dicts, wi
+00017c10: 7468 206b 6579 7320 6173 2050 4152 4e41  th keys as PARNA
+00017c20: 4d45 5320 6f66 2065 6163 6820 4c6f 6754  MES of each LogT
+00017c30: 6175 544d 6f64 656c 0a20 2020 2020 2020  auTModel.       
+00017c40: 2061 6e64 2076 616c 7565 7320 6173 2065   and values as e
+00017c50: 6974 6865 7220 7468 6520 7374 7269 6e67  ither the string
+00017c60: 2027 6775 6573 7327 206f 7220 6120 666c   'guess' or a fl
+00017c70: 6f61 7420 7661 6c75 650a 2020 2020 6c6f  oat value.    lo
+00017c80: 676d 6f64 656c 733a 206c 6973 745b 4c6f  gmodels: list[Lo
+00017c90: 6754 6175 544d 6f64 656c 5d0a 2020 2020  gTauTModel].    
+00017ca0: 2020 2020 4c69 7374 206f 6620 756e 696e      List of unin
+00017cb0: 7374 616e 7469 6174 6564 204c 6f67 5461  stantiated LogTa
+00017cc0: 7554 4d6f 6465 6c20 6f62 6a65 6374 730a  uTModel objects.
+00017cd0: 0a20 2020 2041 7474 7269 6275 7465 730a  .    Attributes.
+00017ce0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00017cf0: 2020 206c 6f67 6d6f 6465 6c73 3a20 6c69     logmodels: li
+00017d00: 7374 5b4c 6f67 5461 7554 4d6f 6465 6c5d  st[LogTauTModel]
+00017d10: 0a20 2020 2020 2020 204c 6973 7420 6f66  .        List of
+00017d20: 204c 6f67 5461 7554 4d6f 6465 6c20 6f62   LogTauTModel ob
+00017d30: 6a65 6374 730a 2020 2020 4e41 4d45 3a20  jects.    NAME: 
+00017d40: 7374 720a 2020 2020 2020 2020 4e61 6d65  str.        Name
+00017d50: 7320 6f66 2065 6163 6820 4c6f 6754 6175  s of each LogTau
+00017d60: 544d 6f64 656c 2063 6f6e 6361 7465 6e61  TModel concatena
+00017d70: 7465 640a 2020 2020 2727 270a 0a20 2020  ted.    '''..   
+00017d80: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+00017d90: 6c66 2c20 6c6f 676d 6f64 656c 733a 206c  lf, logmodels: l
+00017da0: 6973 745b 4c6f 6754 6175 544d 6f64 656c  ist[LogTauTModel
+00017db0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00017dc0: 2020 2020 6669 745f 7661 7273 3a20 6c69      fit_vars: li
+00017dd0: 7374 5b64 6963 745b 7374 722c 2066 6c6f  st[dict[str, flo
+00017de0: 6174 207c 2073 7472 5d5d 2c0a 2020 2020  at | str]],.    
+00017df0: 2020 2020 2020 2020 2020 2020 2066 6978               fix
+00017e00: 5f76 6172 733a 206c 6973 745b 6469 6374  _vars: list[dict
+00017e10: 5b73 7472 2c20 666c 6f61 7420 7c20 7374  [str, float | st
+00017e20: 725d 5d29 202d 3e20 4e6f 6e65 3a0a 0a20  r]]) -> None:.. 
+00017e30: 2020 2020 2020 2023 2049 6e73 7461 6e74         # Instant
+00017e40: 6961 7465 2065 6163 6820 6c6f 676d 6f64  iate each logmod
+00017e50: 656c 2061 6e64 2063 7265 6174 6520 6c69  el and create li
+00017e60: 7374 206f 6620 696e 7374 616e 7469 6174  st of instantiat
+00017e70: 6564 206c 6f67 6d6f 6465 6c73 0a20 2020  ed logmodels.   
+00017e80: 2020 2020 2073 656c 662e 6c6f 676d 6f64       self.logmod
+00017e90: 656c 7320 3d20 7365 6c66 2e70 726f 6365  els = self.proce
+00017ea0: 7373 5f66 6974 6669 7828 6669 745f 7661  ss_fitfix(fit_va
+00017eb0: 7273 2c20 6669 785f 7661 7273 2c20 6c6f  rs, fix_vars, lo
+00017ec0: 676d 6f64 656c 7329 0a0a 2020 2020 2020  gmodels)..      
+00017ed0: 2020 7365 6c66 2e4e 414d 4520 3d20 5b6c    self.NAME = [l
+00017ee0: 6f67 6d6f 6465 6c2e 4e41 4d45 2066 6f72  ogmodel.NAME for
+00017ef0: 206c 6f67 6d6f 6465 6c20 696e 206c 6f67   logmodel in log
+00017f00: 6d6f 6465 6c73 5d0a 2020 2020 2020 2020  models].        
+00017f10: 7365 6c66 2e4e 414d 4520 3d20 2727 2e6a  self.NAME = ''.j
+00017f20: 6f69 6e28 5b27 7b7d 2b27 2e66 6f72 6d61  oin(['{}+'.forma
+00017f30: 7428 6e61 6d65 2920 666f 7220 6e61 6d65  t(name) for name
+00017f40: 2069 6e20 7365 6c66 2e4e 414d 455d 295b   in self.NAME])[
+00017f50: 3a2d 315d 0a0a 2020 2020 2020 2020 7365  :-1]..        se
+00017f60: 6c66 2e5f 6669 745f 7374 6174 7573 203d  lf._fit_status =
+00017f70: 2046 616c 7365 0a0a 2020 2020 2020 2020   False..        
+00017f80: 7265 7475 726e 0a0a 2020 2020 4070 726f  return..    @pro
+00017f90: 7065 7274 790a 2020 2020 6465 6620 6669  perty.    def fi
+00017fa0: 745f 7374 6174 7573 2873 656c 6629 202d  t_status(self) -
+00017fb0: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
+00017fc0: 2754 7275 6520 6966 2066 6974 2073 7563  'True if fit suc
+00017fd0: 6365 7373 6675 6c2c 2065 6c73 6520 4661  cessful, else Fa
+00017fe0: 6c73 6527 0a20 2020 2020 2020 2072 6574  lse'.        ret
+00017ff0: 7572 6e20 7365 6c66 2e5f 6669 745f 7374  urn self._fit_st
+00018000: 6174 7573 0a0a 2020 2020 4066 6974 5f73  atus..    @fit_s
+00018010: 7461 7475 732e 7365 7474 6572 0a20 2020  tatus.setter.   
+00018020: 2064 6566 2066 6974 5f73 7461 7475 7328   def fit_status(
+00018030: 7365 6c66 2c20 7661 6c75 6529 3a0a 2020  self, value):.  
+00018040: 2020 2020 2020 6966 2074 7970 6528 7661        if type(va
+00018050: 6c75 6529 203d 3d20 626f 6f6c 3a0a 2020  lue) == bool:.  
+00018060: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00018070: 6669 745f 7374 6174 7573 203d 2076 616c  fit_status = val
+00018080: 7565 0a20 2020 2020 2020 2065 6c73 653a  ue.        else:
+00018090: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+000180a0: 7365 2054 7970 6545 7272 6f72 0a20 2020  se TypeError.   
+000180b0: 2020 2020 2072 6574 7572 6e0a 0a20 2020       return..   
+000180c0: 2040 7374 6174 6963 6d65 7468 6f64 0a20   @staticmethod. 
+000180d0: 2020 2064 6566 2070 726f 6365 7373 5f66     def process_f
+000180e0: 6974 6669 7828 6669 745f 7661 7273 3a20  itfix(fit_vars: 
+000180f0: 6c69 7374 5b64 6963 745b 7374 722c 2066  list[dict[str, f
+00018100: 6c6f 6174 207c 2073 7472 5d5d 2c0a 2020  loat | str]],.  
 00018110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018120: 2066 6978 5f76 6172 733a 206c 6973 745b   fix_vars: list[
-00018130: 6469 6374 5b73 7472 2c20 666c 6f61 7420  dict[str, float 
-00018140: 7c20 7374 725d 5d2c 0a20 2020 2020 2020  | str]],.       
+00018120: 2020 2020 2066 6978 5f76 6172 733a 206c       fix_vars: l
+00018130: 6973 745b 6469 6374 5b73 7472 2c20 666c  ist[dict[str, fl
+00018140: 6f61 7420 7c20 7374 725d 5d2c 0a20 2020  oat | str]],.   
 00018150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018160: 6c6f 676d 6f64 656c 733a 206c 6973 745b  logmodels: list[
-00018170: 4c6f 6754 6175 544d 6f64 656c 5d29 202d  LogTauTModel]) -
-00018180: 3e20 6c69 7374 5b4c 6f67 5461 7554 4d6f  > list[LogTauTMo
-00018190: 6465 6c5d 3a0a 2020 2020 2020 2020 2727  del]:.        ''
-000181a0: 270a 2020 2020 2020 2020 4173 736f 6369  '.        Associ
-000181b0: 6174 6573 2066 6974 2061 6e64 2066 6978  ates fit and fix
-000181c0: 2064 6963 7473 2077 6974 6820 6120 6c69   dicts with a li
-000181d0: 7374 206f 6620 6c6f 676d 6f64 656c 7320  st of logmodels 
-000181e0: 6279 2069 6e73 7461 6e74 6961 7469 6e67  by instantiating
-000181f0: 0a20 2020 2020 2020 2065 6163 6820 6c6f  .        each lo
-00018200: 676d 6f64 656c 2077 6974 6820 7468 6520  gmodel with the 
-00018210: 7370 6563 6966 6965 6420 7061 7261 6d65  specified parame
-00018220: 7465 7273 0a0a 2020 2020 2020 2020 5061  ters..        Pa
-00018230: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-00018240: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 0a20 2020   ----------..   
-00018250: 2020 2020 2066 6974 5f76 6172 733a 206c       fit_vars: l
-00018260: 6973 745b 6469 6374 5b73 7472 2c20 666c  ist[dict[str, fl
-00018270: 6f61 7420 7c20 7374 725d 5d0a 2020 2020  oat | str]].    
-00018280: 2020 2020 2020 2020 4c69 7374 206f 6620          List of 
-00018290: 6669 7420 6469 6374 732c 2077 6974 6820  fit dicts, with 
-000182a0: 6b65 7973 2061 7320 5041 524e 414d 4553  keys as PARNAMES
-000182b0: 206f 6620 6561 6368 204c 6f67 5461 7554   of each LogTauT
-000182c0: 4d6f 6465 6c0a 2020 2020 2020 2020 2020  Model.          
-000182d0: 2020 616e 6420 7661 6c75 6573 2061 7320    and values as 
-000182e0: 6569 7468 6572 2074 6865 2073 7472 696e  either the strin
-000182f0: 6720 2767 7565 7373 2720 6f72 2061 2066  g 'guess' or a f
-00018300: 6c6f 6174 2076 616c 7565 0a20 2020 2020  loat value.     
-00018310: 2020 2066 6978 5f76 6172 733a 206c 6973     fix_vars: lis
-00018320: 745b 6469 6374 5b73 7472 2c20 666c 6f61  t[dict[str, floa
-00018330: 7420 7c20 7374 725d 5d0a 2020 2020 2020  t | str]].      
-00018340: 2020 2020 2020 4c69 7374 206f 6620 6669        List of fi
-00018350: 7820 6469 6374 732c 2077 6974 6820 6b65  x dicts, with ke
-00018360: 7973 2061 7320 5041 524e 414d 4553 206f  ys as PARNAMES o
-00018370: 6620 6561 6368 204c 6f67 5461 7554 4d6f  f each LogTauTMo
-00018380: 6465 6c0a 2020 2020 2020 2020 2020 2020  del.            
-00018390: 616e 6420 7661 6c75 6573 2061 7320 6569  and values as ei
-000183a0: 7468 6572 2074 6865 2073 7472 696e 6720  ther the string 
-000183b0: 2767 7565 7373 2720 6f72 2061 2066 6c6f  'guess' or a flo
-000183c0: 6174 2076 616c 7565 0a20 2020 2020 2020  at value.       
-000183d0: 206c 6f67 6d6f 6465 6c73 3a20 6c69 7374   logmodels: list
-000183e0: 5b4c 6f67 5461 7554 4d6f 6465 6c5d 0a20  [LogTauTModel]. 
-000183f0: 2020 2020 2020 2020 2020 204c 6973 7420             List 
-00018400: 6f66 2075 6e69 6e73 7461 6e74 6961 7465  of uninstantiate
-00018410: 6420 4c6f 6754 6175 544d 6f64 656c 206f  d LogTauTModel o
-00018420: 626a 6563 7473 0a0a 2020 2020 2020 2020  bjects..        
-00018430: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
-00018440: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00018450: 6c69 7374 5b4c 6f67 5461 7554 4d6f 6465  list[LogTauTMode
-00018460: 6c5d 0a20 2020 2020 2020 2020 2020 2049  l].            I
-00018470: 6e73 7461 6e74 6961 7465 6420 4c6f 6754  nstantiated LogT
-00018480: 6175 544d 6f64 656c 7320 7769 7468 2066  auTModels with f
-00018490: 6974 2061 6e64 2066 6978 2064 6963 7473  it and fix dicts
-000184a0: 2061 7070 6c69 6564 0a20 2020 2020 2020   applied.       
-000184b0: 2027 2727 0a0a 2020 2020 2020 2020 6d61   '''..        ma
-000184c0: 726b 6564 203d 205b 4661 6c73 655d 202a  rked = [False] *
-000184d0: 206c 656e 2866 6974 5f76 6172 7329 0a0a   len(fit_vars)..
-000184e0: 2020 2020 2020 2020 696e 7374 616e 7469          instanti
-000184f0: 6174 6564 5f6d 6f64 656c 7320 3d20 5b5d  ated_models = []
-00018500: 0a0a 2020 2020 2020 2020 666f 7220 6c6f  ..        for lo
-00018510: 676d 6f64 656c 2069 6e20 6c6f 676d 6f64  gmodel in logmod
-00018520: 656c 733a 0a20 2020 2020 2020 2020 2020  els:.           
-00018530: 2066 6f72 2069 742c 2028 6669 7476 6172   for it, (fitvar
-00018540: 5f73 6574 2c20 6669 785f 7661 725f 7365  _set, fix_var_se
-00018550: 7429 2069 6e20 656e 756d 6572 6174 6528  t) in enumerate(
-00018560: 7a69 7028 6669 745f 7661 7273 2c20 6669  zip(fit_vars, fi
-00018570: 785f 7661 7273 2929 3a20 2320 6e6f 7161  x_vars)): # noqa
-00018580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018590: 2069 6620 6d61 726b 6564 5b69 745d 3a0a   if marked[it]:.
-000185a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000185b0: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
-000185c0: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-000185d0: 6620 616c 6c28 5b6b 2069 6e20 6c6f 676d  f all([k in logm
-000185e0: 6f64 656c 2e50 4152 4e41 4d45 5320 666f  odel.PARNAMES fo
-000185f0: 7220 6b20 696e 2066 6974 7661 725f 7365  r k in fitvar_se
-00018600: 742e 6b65 7973 2829 5d29 3a20 2320 6e6f  t.keys()]): # no
-00018610: 7161 0a20 2020 2020 2020 2020 2020 2020  qa.             
-00018620: 2020 2020 2020 2069 6620 616c 6c28 5b6b         if all([k
-00018630: 2069 6e20 6c6f 676d 6f64 656c 2e50 4152   in logmodel.PAR
-00018640: 4e41 4d45 5320 666f 7220 6b20 696e 2066  NAMES for k in f
-00018650: 6978 5f76 6172 5f73 6574 2e6b 6579 7328  ix_var_set.keys(
-00018660: 295d 2920 6f72 206e 6f74 206c 656e 2866  )]) or not len(f
-00018670: 6978 5f76 6172 5f73 6574 293a 2023 206e  ix_var_set): # n
-00018680: 6f71 610a 2020 2020 2020 2020 2020 2020  oqa.            
-00018690: 2020 2020 2020 2020 2020 2020 696e 7374              inst
-000186a0: 616e 7469 6174 6564 5f6d 6f64 656c 732e  antiated_models.
-000186b0: 6170 7065 6e64 280a 2020 2020 2020 2020  append(.        
+00018160: 2020 2020 6c6f 676d 6f64 656c 733a 206c      logmodels: l
+00018170: 6973 745b 4c6f 6754 6175 544d 6f64 656c  ist[LogTauTModel
+00018180: 5d29 202d 3e20 6c69 7374 5b4c 6f67 5461  ]) -> list[LogTa
+00018190: 7554 4d6f 6465 6c5d 3a0a 2020 2020 2020  uTModel]:.      
+000181a0: 2020 2727 270a 2020 2020 2020 2020 4173    '''.        As
+000181b0: 736f 6369 6174 6573 2066 6974 2061 6e64  sociates fit and
+000181c0: 2066 6978 2064 6963 7473 2077 6974 6820   fix dicts with 
+000181d0: 6120 6c69 7374 206f 6620 6c6f 676d 6f64  a list of logmod
+000181e0: 656c 7320 6279 2069 6e73 7461 6e74 6961  els by instantia
+000181f0: 7469 6e67 0a20 2020 2020 2020 2065 6163  ting.        eac
+00018200: 6820 6c6f 676d 6f64 656c 2077 6974 6820  h logmodel with 
+00018210: 7468 6520 7370 6563 6966 6965 6420 7061  the specified pa
+00018220: 7261 6d65 7465 7273 0a0a 2020 2020 2020  rameters..      
+00018230: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00018240: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+00018250: 0a20 2020 2020 2020 2066 6974 5f76 6172  .        fit_var
+00018260: 733a 206c 6973 745b 6469 6374 5b73 7472  s: list[dict[str
+00018270: 2c20 666c 6f61 7420 7c20 7374 725d 5d0a  , float | str]].
+00018280: 2020 2020 2020 2020 2020 2020 4c69 7374              List
+00018290: 206f 6620 6669 7420 6469 6374 732c 2077   of fit dicts, w
+000182a0: 6974 6820 6b65 7973 2061 7320 5041 524e  ith keys as PARN
+000182b0: 414d 4553 206f 6620 6561 6368 204c 6f67  AMES of each Log
+000182c0: 5461 7554 4d6f 6465 6c0a 2020 2020 2020  TauTModel.      
+000182d0: 2020 2020 2020 616e 6420 7661 6c75 6573        and values
+000182e0: 2061 7320 6569 7468 6572 2074 6865 2073   as either the s
+000182f0: 7472 696e 6720 2767 7565 7373 2720 6f72  tring 'guess' or
+00018300: 2061 2066 6c6f 6174 2076 616c 7565 0a20   a float value. 
+00018310: 2020 2020 2020 2066 6978 5f76 6172 733a         fix_vars:
+00018320: 206c 6973 745b 6469 6374 5b73 7472 2c20   list[dict[str, 
+00018330: 666c 6f61 7420 7c20 7374 725d 5d0a 2020  float | str]].  
+00018340: 2020 2020 2020 2020 2020 4c69 7374 206f            List o
+00018350: 6620 6669 7820 6469 6374 732c 2077 6974  f fix dicts, wit
+00018360: 6820 6b65 7973 2061 7320 5041 524e 414d  h keys as PARNAM
+00018370: 4553 206f 6620 6561 6368 204c 6f67 5461  ES of each LogTa
+00018380: 7554 4d6f 6465 6c0a 2020 2020 2020 2020  uTModel.        
+00018390: 2020 2020 616e 6420 7661 6c75 6573 2061      and values a
+000183a0: 7320 6569 7468 6572 2074 6865 2073 7472  s either the str
+000183b0: 696e 6720 2767 7565 7373 2720 6f72 2061  ing 'guess' or a
+000183c0: 2066 6c6f 6174 2076 616c 7565 0a20 2020   float value.   
+000183d0: 2020 2020 206c 6f67 6d6f 6465 6c73 3a20       logmodels: 
+000183e0: 6c69 7374 5b4c 6f67 5461 7554 4d6f 6465  list[LogTauTMode
+000183f0: 6c5d 0a20 2020 2020 2020 2020 2020 204c  l].            L
+00018400: 6973 7420 6f66 2075 6e69 6e73 7461 6e74  ist of uninstant
+00018410: 6961 7465 6420 4c6f 6754 6175 544d 6f64  iated LogTauTMod
+00018420: 656c 206f 626a 6563 7473 0a0a 2020 2020  el objects..    
+00018430: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+00018440: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+00018450: 2020 2020 6c69 7374 5b4c 6f67 5461 7554      list[LogTauT
+00018460: 4d6f 6465 6c5d 0a20 2020 2020 2020 2020  Model].         
+00018470: 2020 2049 6e73 7461 6e74 6961 7465 6420     Instantiated 
+00018480: 4c6f 6754 6175 544d 6f64 656c 7320 7769  LogTauTModels wi
+00018490: 7468 2066 6974 2061 6e64 2066 6978 2064  th fit and fix d
+000184a0: 6963 7473 2061 7070 6c69 6564 0a20 2020  icts applied.   
+000184b0: 2020 2020 2027 2727 0a0a 2020 2020 2020       '''..      
+000184c0: 2020 6d61 726b 6564 203d 205b 4661 6c73    marked = [Fals
+000184d0: 655d 202a 206c 656e 2866 6974 5f76 6172  e] * len(fit_var
+000184e0: 7329 0a0a 2020 2020 2020 2020 696e 7374  s)..        inst
+000184f0: 616e 7469 6174 6564 5f6d 6f64 656c 7320  antiated_models 
+00018500: 3d20 5b5d 0a0a 2020 2020 2020 2020 666f  = []..        fo
+00018510: 7220 6c6f 676d 6f64 656c 2069 6e20 6c6f  r logmodel in lo
+00018520: 676d 6f64 656c 733a 0a20 2020 2020 2020  gmodels:.       
+00018530: 2020 2020 2066 6f72 2069 742c 2028 6669       for it, (fi
+00018540: 7476 6172 5f73 6574 2c20 6669 785f 7661  tvar_set, fix_va
+00018550: 725f 7365 7429 2069 6e20 656e 756d 6572  r_set) in enumer
+00018560: 6174 6528 7a69 7028 6669 745f 7661 7273  ate(zip(fit_vars
+00018570: 2c20 6669 785f 7661 7273 2929 3a20 2320  , fix_vars)): # 
+00018580: 6e6f 7161 0a20 2020 2020 2020 2020 2020  noqa.           
+00018590: 2020 2020 2069 6620 6d61 726b 6564 5b69       if marked[i
+000185a0: 745d 3a0a 2020 2020 2020 2020 2020 2020  t]:.            
+000185b0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+000185c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000185d0: 2065 6c69 6620 616c 6c28 5b6b 2069 6e20   elif all([k in 
+000185e0: 6c6f 676d 6f64 656c 2e50 4152 4e41 4d45  logmodel.PARNAME
+000185f0: 5320 666f 7220 6b20 696e 2066 6974 7661  S for k in fitva
+00018600: 725f 7365 742e 6b65 7973 2829 5d29 3a20  r_set.keys()]): 
+00018610: 2320 6e6f 7161 0a20 2020 2020 2020 2020  # noqa.         
+00018620: 2020 2020 2020 2020 2020 2069 6620 616c             if al
+00018630: 6c28 5b6b 2069 6e20 6c6f 676d 6f64 656c  l([k in logmodel
+00018640: 2e50 4152 4e41 4d45 5320 666f 7220 6b20  .PARNAMES for k 
+00018650: 696e 2066 6978 5f76 6172 5f73 6574 2e6b  in fix_var_set.k
+00018660: 6579 7328 295d 2920 6f72 206e 6f74 206c  eys()]) or not l
+00018670: 656e 2866 6978 5f76 6172 5f73 6574 293a  en(fix_var_set):
+00018680: 2023 206e 6f71 610a 2020 2020 2020 2020   # noqa.        
+00018690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000186a0: 696e 7374 616e 7469 6174 6564 5f6d 6f64  instantiated_mod
+000186b0: 656c 732e 6170 7065 6e64 280a 2020 2020  els.append(.    
 000186c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000186d0: 2020 2020 6c6f 676d 6f64 656c 2866 6974      logmodel(fit
-000186e0: 7661 725f 7365 742c 2066 6978 5f76 6172  var_set, fix_var
-000186f0: 5f73 6574 290a 2020 2020 2020 2020 2020  _set).          
-00018700: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00018710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018720: 2020 2020 2020 2020 6d61 726b 6564 5b69          marked[i
-00018730: 745d 203d 2054 7275 650a 0a20 2020 2020  t] = True..     
-00018740: 2020 2072 6574 7572 6e20 696e 7374 616e     return instan
-00018750: 7469 6174 6564 5f6d 6f64 656c 730a 0a20  tiated_models.. 
-00018760: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
-00018770: 2020 2020 6465 6620 7265 7369 6475 616c      def residual
-00018780: 5f66 726f 6d5f 666c 6f61 745f 6c69 7374  _from_float_list
-00018790: 2863 6c73 2c20 6e65 775f 7661 6c73 3a20  (cls, new_vals: 
-000187a0: 6e70 742e 4172 7261 794c 696b 652c 0a20  npt.ArrayLike,. 
-000187b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000186d0: 2020 2020 2020 2020 6c6f 676d 6f64 656c          logmodel
+000186e0: 2866 6974 7661 725f 7365 742c 2066 6978  (fitvar_set, fix
+000186f0: 5f76 6172 5f73 6574 290a 2020 2020 2020  _var_set).      
+00018700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018710: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00018720: 2020 2020 2020 2020 2020 2020 6d61 726b              mark
+00018730: 6564 5b69 745d 203d 2054 7275 650a 0a20  ed[it] = True.. 
+00018740: 2020 2020 2020 2072 6574 7572 6e20 696e         return in
+00018750: 7374 616e 7469 6174 6564 5f6d 6f64 656c  stantiated_model
+00018760: 730a 0a20 2020 2040 636c 6173 736d 6574  s..    @classmet
+00018770: 686f 640a 2020 2020 6465 6620 7265 7369  hod.    def resi
+00018780: 6475 616c 5f66 726f 6d5f 666c 6f61 745f  dual_from_float_
+00018790: 6c69 7374 2863 6c73 2c20 6e65 775f 7661  list(cls, new_va
+000187a0: 6c73 3a20 6e70 742e 4172 7261 794c 696b  ls: npt.ArrayLik
+000187b0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
 000187c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000187d0: 6c6f 676d 6f64 656c 733a 206c 6973 745b  logmodels: list[
-000187e0: 4c6f 6754 6175 544d 6f64 656c 5d2c 0a20  LogTauTModel],. 
-000187f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000187d0: 2020 2020 6c6f 676d 6f64 656c 733a 206c      logmodels: l
+000187e0: 6973 745b 4c6f 6754 6175 544d 6f64 656c  ist[LogTauTModel
+000187f0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
 00018800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018810: 7465 6d70 6572 6174 7572 6573 3a20 6e70  temperatures: np
-00018820: 742e 4172 7261 794c 696b 652c 0a20 2020  t.ArrayLike,.   
-00018830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018840: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00018850: 6772 6174 653a 206e 7074 2e41 7272 6179  grate: npt.Array
-00018860: 4c69 6b65 2c0a 2020 2020 2020 2020 2020  Like,.          
+00018810: 2020 2020 7465 6d70 6572 6174 7572 6573      temperatures
+00018820: 3a20 6e70 742e 4172 7261 794c 696b 652c  : npt.ArrayLike,
+00018830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018850: 2020 6c6f 6772 6174 653a 206e 7074 2e41    lograte: npt.A
+00018860: 7272 6179 4c69 6b65 2c0a 2020 2020 2020  rrayLike,.      
 00018870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018880: 2020 2020 2020 2073 6967 6d61 3a20 6e70         sigma: np
-00018890: 742e 4172 7261 794c 696b 6520 3d20 5b5d  t.ArrayLike = []
-000188a0: 2920 2d3e 206e 7074 2e4e 4441 7272 6179  ) -> npt.NDArray
-000188b0: 3a0a 2020 2020 2020 2020 2727 270a 2020  :.        '''.  
-000188c0: 2020 2020 2020 5772 6170 7065 7220 666f        Wrapper fo
-000188d0: 7220 6072 6573 6964 7561 6c73 6020 6d65  r `residuals` me
-000188e0: 7468 6f64 2c20 7461 6b65 7320 6e65 7720  thod, takes new 
-000188f0: 7661 6c75 6573 2066 726f 6d20 6669 7474  values from fitt
-00018900: 696e 6720 726f 7574 696e 650a 2020 2020  ing routine.    
-00018910: 2020 2020 7768 6963 6820 7072 6f76 6964      which provid
-00018920: 6573 206c 6973 745b 666c 6f61 745d 2c20  es list[float], 
-00018930: 746f 2063 6f6e 7374 7275 6374 206e 6577  to construct new
-00018940: 2066 6974 5f76 6172 7320 6469 6374 2c20   fit_vars dict, 
-00018950: 7468 656e 0a20 2020 2020 2020 2072 756e  then.        run
-00018960: 7320 6072 6573 6964 7561 6c73 6020 6d65  s `residuals` me
-00018970: 7468 6f64 2e0a 0a20 2020 2020 2020 2050  thod...        P
-00018980: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-00018990: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-000189a0: 2020 2020 206e 6577 5f76 616c 733a 2061       new_vals: a
-000189b0: 7272 6179 5f6c 696b 650a 2020 2020 2020  rray_like.      
-000189c0: 2020 2020 2020 5468 6973 2069 7465 7261        This itera
-000189d0: 7469 6f6e 2773 2066 6974 2070 6172 616d  tion's fit param
-000189e0: 6574 6572 2076 616c 7565 7320 7072 6f76  eter values prov
-000189f0: 6964 6564 2062 7920 6c65 6173 745f 7371  ided by least_sq
-00018a00: 7561 7265 730a 2020 2020 2020 2020 2020  uares.          
-00018a10: 2020 7468 6973 2068 6173 2074 6865 2073    this has the s
-00018a20: 616d 6520 6f72 6465 7220 6174 2066 6974  ame order at fit
-00018a30: 5f76 6172 732e 6b65 7973 0a20 2020 2020  _vars.keys.     
-00018a40: 2020 206c 6f67 6d6f 6465 6c73 3a20 6c69     logmodels: li
-00018a50: 7374 5b4c 6f67 5461 7554 4d6f 6465 6c5d  st[LogTauTModel]
-00018a60: 0a20 2020 2020 2020 2020 2020 204d 6f64  .            Mod
-00018a70: 656c 7320 746f 2075 7365 0a20 2020 2020  els to use.     
-00018a80: 2020 2074 656d 7065 7261 7475 7265 733a     temperatures:
-00018a90: 2061 7272 6179 5f6c 696b 650a 2020 2020   array_like.    
-00018aa0: 2020 2020 2020 2020 5465 6d70 6572 6174          Temperat
-00018ab0: 7572 6520 7661 6c75 6573 2028 4b29 2061  ure values (K) a
-00018ac0: 7420 7768 6963 6820 6d6f 6465 6c20 6675  t which model fu
-00018ad0: 6e63 7469 6f6e 2069 7320 6576 616c 7561  nction is evalua
-00018ae0: 7465 640a 2020 2020 2020 2020 6c6f 6772  ted.        logr
-00018af0: 6174 653a 2061 7272 6179 5f6c 696b 650a  ate: array_like.
-00018b00: 2020 2020 2020 2020 2020 2020 5472 7565              True
-00018b10: 2028 6578 7065 7269 6d65 6e74 616c 2920   (experimental) 
-00018b20: 7661 6c75 6573 206f 6620 6c6f 6731 3028  values of log10(
-00018b30: 7265 6c61 7861 7469 6f6e 2072 6174 6529  relaxation rate)
-00018b40: 0a20 2020 2020 2020 2073 6967 6d61 3a20  .        sigma: 
-00018b50: 6172 7261 795f 6c69 6b65 0a20 2020 2020  array_like.     
-00018b60: 2020 2020 2020 2053 7461 6e64 6172 6420         Standard 
-00018b70: 6465 7669 6174 696f 6e20 6f66 2074 6175  deviation of tau
-00018b80: 2069 6e20 6c6f 6773 7061 6365 0a0a 2020   in logspace..  
-00018b90: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
-00018ba0: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
-00018bb0: 2020 2020 2020 6e64 6172 7261 7920 6f66        ndarray of
-00018bc0: 2066 6c6f 6174 730a 2020 2020 2020 2020   floats.        
-00018bd0: 2020 2020 5265 7369 6475 616c 730a 2020      Residuals.  
-00018be0: 2020 2020 2020 2727 270a 0a20 2020 2020        '''..     
-00018bf0: 2020 2023 2053 7761 7020 6669 7420 7661     # Swap fit va
-00018c00: 6c75 6573 2066 6f72 206e 6577 2076 616c  lues for new val
-00018c10: 7565 7320 6672 6f6d 2066 6974 2072 6f75  ues from fit rou
-00018c20: 7469 6e65 0a20 2020 2020 2020 206e 6577  tine.        new
-00018c30: 5f66 6974 5f76 6172 7320 3d20 5b5d 0a0a  _fit_vars = []..
-00018c40: 2020 2020 2020 2020 6974 203d 2030 0a20          it = 0. 
-00018c50: 2020 2020 2020 2066 6f72 206c 6f67 6d6f         for logmo
-00018c60: 6465 6c20 696e 206c 6f67 6d6f 6465 6c73  del in logmodels
-00018c70: 3a0a 2020 2020 2020 2020 2020 2020 6e65  :.            ne
-00018c80: 775f 6469 6374 203d 207b 7d0a 2020 2020  w_dict = {}.    
-00018c90: 2020 2020 2020 2020 666f 7220 6e61 6d65          for name
-00018ca0: 2069 6e20 6c6f 676d 6f64 656c 2e66 6974   in logmodel.fit
-00018cb0: 5f76 6172 732e 6b65 7973 2829 3a0a 2020  _vars.keys():.  
-00018cc0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-00018cd0: 775f 6469 6374 5b6e 616d 655d 203d 206e  w_dict[name] = n
-00018ce0: 6577 5f76 616c 735b 6974 5d0a 2020 2020  ew_vals[it].    
-00018cf0: 2020 2020 2020 2020 2020 2020 6974 202b              it +
-00018d00: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
-00018d10: 6e65 775f 6669 745f 7661 7273 2e61 7070  new_fit_vars.app
-00018d20: 656e 6428 6e65 775f 6469 6374 290a 0a20  end(new_dict).. 
-00018d30: 2020 2020 2020 2072 6573 6964 7561 6c73         residuals
-00018d40: 203d 2063 6c73 2e72 6573 6964 7561 6c73   = cls.residuals
-00018d50: 280a 2020 2020 2020 2020 2020 2020 6c6f  (.            lo
-00018d60: 676d 6f64 656c 732c 206e 6577 5f66 6974  gmodels, new_fit
-00018d70: 5f76 6172 732c 2074 656d 7065 7261 7475  _vars, temperatu
-00018d80: 7265 732c 206c 6f67 7261 7465 0a20 2020  res, lograte.   
-00018d90: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00018da0: 6966 206c 656e 2873 6967 6d61 293a 0a20  if len(sigma):. 
-00018db0: 2020 2020 2020 2020 2020 2072 6573 6964             resid
-00018dc0: 7561 6c73 202f 3d20 7369 676d 610a 0a20  uals /= sigma.. 
-00018dd0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00018de0: 7369 6475 616c 730a 0a20 2020 2040 7374  siduals..    @st
-00018df0: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
-00018e00: 6566 2072 6573 6964 7561 6c73 286c 6f67  ef residuals(log
-00018e10: 6d6f 6465 6c73 3a20 6c69 7374 5b4c 6f67  models: list[Log
-00018e20: 5461 7554 4d6f 6465 6c5d 2c0a 2020 2020  TauTModel],.    
-00018e30: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-00018e40: 775f 6669 745f 7661 7273 3a20 6c69 7374  w_fit_vars: list
-00018e50: 5b64 6963 745b 7374 722c 2066 6c6f 6174  [dict[str, float
-00018e60: 5d5d 2c0a 2020 2020 2020 2020 2020 2020  ]],.            
-00018e70: 2020 2020 2020 7465 6d70 6572 6174 7572        temperatur
-00018e80: 6573 3a20 6e70 742e 4172 7261 794c 696b  es: npt.ArrayLik
-00018e90: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00018ea0: 2020 2020 2074 7275 655f 6c6f 6772 6174       true_lograt
-00018eb0: 653a 206e 7074 2e41 7272 6179 4c69 6b65  e: npt.ArrayLike
-00018ec0: 2920 2d3e 206e 7074 2e4e 4441 7272 6179  ) -> npt.NDArray
-00018ed0: 3a0a 2020 2020 2020 2020 2727 270a 2020  :.        '''.  
-00018ee0: 2020 2020 2020 4361 6c63 756c 6174 6573        Calculates
-00018ef0: 2064 6966 6665 7265 6e63 6520 6265 7477   difference betw
-00018f00: 6565 6e20 6578 7065 7269 6d65 6e74 616c  een experimental
-00018f10: 206c 6f67 3130 2874 6175 5e2d 3129 0a20   log10(tau^-1). 
-00018f20: 2020 2020 2020 2061 6e64 206c 6f67 3130         and log10
-00018f30: 2874 6175 5e2d 3129 206f 6274 6169 6e65  (tau^-1) obtaine
-00018f40: 6420 6672 6f6d 2074 6865 2073 756d 206f  d from the sum o
-00018f50: 6620 7468 6520 7072 6f76 6964 6564 206c  f the provided l
-00018f60: 6f67 6d6f 6465 6c73 0a20 2020 2020 2020  ogmodels.       
-00018f70: 2075 7369 6e67 2074 6865 2070 726f 7669   using the provi
-00018f80: 6465 6420 6669 7420 7661 7269 6162 6c65  ded fit variable
-00018f90: 2076 616c 7565 7320 6174 2070 726f 7669   values at provi
-00018fa0: 6465 6420 7465 6d70 6572 6174 7572 6573  ded temperatures
-00018fb0: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-00018fc0: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-00018fd0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00018fe0: 6c6f 676d 6f64 656c 733a 206c 6973 745b  logmodels: list[
-00018ff0: 4c6f 6754 6175 544d 6f64 656c 5d0a 2020  LogTauTModel].  
-00019000: 2020 2020 2020 2020 2020 4c6f 6754 6175            LogTau
-00019010: 544d 6f64 656c 7320 7768 6963 6820 7769  TModels which wi
-00019020: 6c6c 2062 6520 6576 616c 7561 7465 640a  ll be evaluated.
-00019030: 2020 2020 2020 2020 6e65 775f 6669 745f          new_fit_
-00019040: 7661 7273 3a20 6c69 7374 5b64 6963 745b  vars: list[dict[
-00019050: 7374 722c 2066 6c6f 6174 5d5d 0a20 2020  str, float]].   
-00019060: 2020 2020 2020 2020 2066 6974 2064 6963           fit dic
-00019070: 7473 2066 6f72 2065 6163 6820 4c6f 6754  ts for each LogT
-00019080: 6175 544d 6f64 656c 2c20 6d75 7374 2068  auTModel, must h
-00019090: 6176 6520 7361 6d65 206f 7264 6572 2061  ave same order a
-000190a0: 7320 6c6f 676d 6f64 656c 0a20 2020 2020  s logmodel.     
-000190b0: 2020 2020 2020 2069 6620 6e6f 2076 6172         if no var
-000190c0: 7320 746f 2066 6974 2066 6f72 2074 6861  s to fit for tha
-000190d0: 7420 6d6f 6465 6c2c 2074 6865 6e20 656d  t model, then em
-000190e0: 7074 7920 6469 6374 2069 7320 6769 7665  pty dict is give
-000190f0: 6e0a 2020 2020 2020 2020 7465 6d70 6572  n.        temper
-00019100: 6174 7572 6573 3a20 6172 7261 795f 6c69  atures: array_li
-00019110: 6b65 0a20 2020 2020 2020 2020 2020 2045  ke.            E
-00019120: 7870 6572 696d 656e 7461 6c20 7465 6d70  xperimental temp
-00019130: 6572 6174 7572 6573 2028 4b29 0a20 2020  eratures (K).   
-00019140: 2020 2020 2074 7275 655f 6c6f 6772 6174       true_lograt
-00019150: 653a 2061 7272 6179 5f6c 696b 650a 2020  e: array_like.  
-00019160: 2020 2020 2020 2020 2020 4578 7065 7269            Experi
-00019170: 6d65 6e74 616c 204c 6f67 3130 2872 6174  mental Log10(rat
-00019180: 6529 730a 0a20 2020 2020 2020 2052 6574  e)s..        Ret
-00019190: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
-000191a0: 2d2d 2d2d 0a20 2020 2020 2020 206e 6461  ----.        nda
-000191b0: 7272 6179 206f 6620 666c 6f61 7473 0a20  rray of floats. 
-000191c0: 2020 2020 2020 2020 2020 204c 6f67 3130             Log10
-000191d0: 2872 6174 6529 5f74 7269 616c 202d 204c  (rate)_trial - L
-000191e0: 6f67 3130 2872 6174 6529 5f65 7870 2066  og10(rate)_exp f
-000191f0: 6f72 2065 6163 6820 7465 6d70 6572 6174  or each temperat
-00019200: 7572 650a 2020 2020 2020 2020 2727 270a  ure.        '''.
-00019210: 0a20 2020 2020 2020 2023 2043 616c 6375  .        # Calcu
-00019220: 6c61 7465 206d 6f64 656c 206c 6f67 3130  late model log10
-00019230: 2872 656c 6178 6174 696f 6e20 7261 7465  (relaxation rate
-00019240: 2920 7573 696e 6720 7061 7261 6d65 7465  ) using paramete
-00019250: 7273 0a20 2020 2020 2020 2023 2061 7320  rs.        # as 
-00019260: 7375 6d20 6f66 2063 6f6e 7472 6962 7574  sum of contribut
-00019270: 696f 6e73 2066 726f 6d20 6561 6368 2070  ions from each p
-00019280: 726f 6365 7373 0a20 2020 2020 2020 2074  rocess.        t
-00019290: 7269 616c 5f6c 6f67 7261 7465 203d 206e  rial_lograte = n
-000192a0: 702e 7a65 726f 7328 6c65 6e28 7465 6d70  p.zeros(len(temp
-000192b0: 6572 6174 7572 6573 2929 0a0a 2020 2020  eratures))..    
-000192c0: 2020 2020 666f 7220 6c6f 676d 6f64 656c      for logmodel
-000192d0: 2c20 6669 745f 7661 7273 2069 6e20 7a69  , fit_vars in zi
-000192e0: 7028 6c6f 676d 6f64 656c 732c 206e 6577  p(logmodels, new
-000192f0: 5f66 6974 5f76 6172 7329 3a0a 2020 2020  _fit_vars):.    
-00019300: 2020 2020 2020 2020 616c 6c5f 7661 7273          all_vars
-00019310: 203d 207b 2a2a 6c6f 676d 6f64 656c 2e66   = {**logmodel.f
-00019320: 6978 5f76 6172 732c 202a 2a66 6974 5f76  ix_vars, **fit_v
-00019330: 6172 737d 0a20 2020 2020 2020 2020 2020  ars}.           
-00019340: 2074 7269 616c 5f6c 6f67 7261 7465 202b   trial_lograte +
-00019350: 3d20 3130 2a2a 6c6f 676d 6f64 656c 2e6d  = 10**logmodel.m
-00019360: 6f64 656c 2861 6c6c 5f76 6172 732c 2074  odel(all_vars, t
-00019370: 656d 7065 7261 7475 7265 7329 0a0a 2020  emperatures)..  
-00019380: 2020 2020 2020 2320 7375 6d20 696e 206c        # sum in l
-00019390: 696e 6561 7220 7370 6163 652c 2074 6865  inear space, the
-000193a0: 6e20 7461 6b65 206c 6f67 0a20 2020 2020  n take log.     
-000193b0: 2020 2074 7269 616c 5f6c 6f67 7261 7465     trial_lograte
-000193c0: 203d 206e 702e 6c6f 6731 3028 7472 6961   = np.log10(tria
-000193d0: 6c5f 6c6f 6772 6174 6529 0a0a 2020 2020  l_lograte)..    
-000193e0: 2020 2020 7265 7369 6475 616c 7320 3d20      residuals = 
-000193f0: 7472 6961 6c5f 6c6f 6772 6174 6520 2d20  trial_lograte - 
-00019400: 7472 7565 5f6c 6f67 7261 7465 0a0a 2020  true_lograte..  
-00019410: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-00019420: 6964 7561 6c73 0a0a 2020 2020 6465 6620  iduals..    def 
-00019430: 6669 745f 746f 2873 656c 662c 2064 6174  fit_to(self, dat
-00019440: 6173 6574 3a20 5461 7554 4461 7461 7365  aset: TauTDatase
-00019450: 742c 2076 6572 626f 7365 3a20 626f 6f6c  t, verbose: bool
-00019460: 203d 2054 7275 6529 202d 3e20 4e6f 6e65   = True) -> None
-00019470: 3a0a 2020 2020 2020 2020 2727 270a 2020  :.        '''.  
-00019480: 2020 2020 2020 4669 7473 206d 6f64 656c        Fits model
-00019490: 2074 6f20 4461 7461 7365 740a 0a20 2020   to Dataset..   
-000194a0: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-000194b0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-000194c0: 2d2d 0a20 2020 2020 2020 2064 6174 6173  --.        datas
-000194d0: 6574 3a20 5461 7554 4461 7461 7365 740a  et: TauTDataset.
-000194e0: 2020 2020 2020 2020 2020 2020 4461 7461              Data
-000194f0: 7365 7420 746f 2077 6869 6368 2061 206d  set to which a m
-00019500: 6f64 656c 206f 6620 7261 7465 2076 7320  odel of rate vs 
-00019510: 7465 6d70 6572 6174 7572 6520 7769 6c6c  temperature will
-00019520: 2062 6520 6669 7474 6564 0a20 2020 2020   be fitted.     
-00019530: 2020 2076 6572 626f 7365 3a20 626f 6f6c     verbose: bool
-00019540: 2c20 6465 6661 756c 7420 5472 7565 0a20  , default True. 
-00019550: 2020 2020 2020 2020 2020 2049 6620 5472             If Tr
-00019560: 7565 2c20 7072 696e 7473 2069 6e66 6f72  ue, prints infor
-00019570: 6d61 7469 6f6e 2074 6f20 7465 726d 696e  mation to termin
-00019580: 616c 0a0a 2020 2020 2020 2020 5265 7475  al..        Retu
-00019590: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
-000195a0: 2d2d 2d0a 2020 2020 2020 2020 4e6f 6e65  ---.        None
-000195b0: 0a20 2020 2020 2020 2027 2727 0a0a 2020  .        '''..  
-000195c0: 2020 2020 2020 2320 496e 6974 6961 6c20        # Initial 
-000195d0: 6775 6573 7320 6973 2061 206c 6973 7420  guess is a list 
-000195e0: 6f66 2066 6974 7661 7273 2076 616c 7565  of fitvars value
-000195f0: 730a 2020 2020 2020 2020 6775 6573 7320  s.        guess 
-00019600: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
-00019610: 7661 6c75 6520 666f 7220 6c6f 676d 6f64  value for logmod
-00019620: 656c 2069 6e20 7365 6c66 2e6c 6f67 6d6f  el in self.logmo
-00019630: 6465 6c73 0a20 2020 2020 2020 2020 2020  dels.           
-00019640: 2066 6f72 2076 616c 7565 2069 6e20 6c6f   for value in lo
-00019650: 676d 6f64 656c 2e66 6974 5f76 6172 732e  gmodel.fit_vars.
-00019660: 7661 6c75 6573 2829 0a20 2020 2020 2020  values().       
-00019670: 205d 0a0a 2020 2020 2020 2020 626f 756e   ]..        boun
-00019680: 6473 203d 206e 702e 6172 7261 7928 5b0a  ds = np.array([.
-00019690: 2020 2020 2020 2020 2020 2020 6c6f 676d              logm
-000196a0: 6f64 656c 2e42 4f55 4e44 535b 6e61 6d65  odel.BOUNDS[name
-000196b0: 5d20 666f 7220 6c6f 676d 6f64 656c 2069  ] for logmodel i
-000196c0: 6e20 7365 6c66 2e6c 6f67 6d6f 6465 6c73  n self.logmodels
-000196d0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-000196e0: 206e 616d 6520 696e 206c 6f67 6d6f 6465   name in logmode
-000196f0: 6c2e 6669 745f 7661 7273 2e6b 6579 7328  l.fit_vars.keys(
-00019700: 290a 2020 2020 2020 2020 5d29 2e54 0a0a  ).        ]).T..
-00019710: 2020 2020 2020 2020 6375 7272 5f66 6974          curr_fit
-00019720: 203d 206c 6561 7374 5f73 7175 6172 6573   = least_squares
-00019730: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
-00019740: 6c66 2e72 6573 6964 7561 6c5f 6672 6f6d  lf.residual_from
-00019750: 5f66 6c6f 6174 5f6c 6973 742c 0a20 2020  _float_list,.   
-00019760: 2020 2020 2020 2020 2061 7267 733d 5b0a           args=[.
-00019770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019780: 7365 6c66 2e6c 6f67 6d6f 6465 6c73 2c0a  self.logmodels,.
-00019790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000197a0: 6461 7461 7365 742e 7465 6d70 6572 6174  dataset.temperat
-000197b0: 7572 6573 2c0a 2020 2020 2020 2020 2020  ures,.          
-000197c0: 2020 2020 2020 6e70 2e6c 6f67 3130 2864        np.log10(d
-000197d0: 6174 6173 6574 2e72 6174 6573 292c 0a20  ataset.rates),. 
-000197e0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-000197f0: 6174 6173 6574 2e6c 6f67 7261 7465 5f70  ataset.lograte_p
-00019800: 6d0a 2020 2020 2020 2020 2020 2020 5d2c  m.            ],
-00019810: 0a20 2020 2020 2020 2020 2020 2078 303d  .            x0=
-00019820: 6775 6573 732c 0a20 2020 2020 2020 2020  guess,.         
-00019830: 2020 2062 6f75 6e64 733d 626f 756e 6473     bounds=bounds
-00019840: 2c0a 2020 2020 2020 2020 2020 2020 6a61  ,.            ja
-00019850: 633d 2733 2d70 6f69 6e74 270a 2020 2020  c='3-point'.    
-00019860: 2020 2020 290a 0a20 2020 2020 2020 2069      )..        i
-00019870: 6620 6375 7272 5f66 6974 2e73 7461 7475  f curr_fit.statu
-00019880: 7320 3d3d 2030 3a0a 2020 2020 2020 2020  s == 0:.        
-00019890: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
-000198a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000198b0: 7574 2e63 7072 696e 7428 0a20 2020 2020  ut.cprint(.     
-000198c0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000198d0: 5c6e 2046 6974 2066 6169 6c65 6420 2d20  \n Fit failed - 
-000198e0: 546f 6f20 6d61 6e79 2069 7465 7261 7469  Too many iterati
-000198f0: 6f6e 7327 2c0a 2020 2020 2020 2020 2020  ons',.          
-00019900: 2020 2020 2020 2020 2020 2762 6c61 636b            'black
-00019910: 5f79 656c 6c6f 7762 6727 0a20 2020 2020  _yellowbg'.     
-00019920: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-00019930: 2020 2020 2020 2020 2020 6e5f 6669 7474            n_fitt
-00019940: 6564 5f70 6172 7320 3d20 6e70 2e73 756d  ed_pars = np.sum
-00019950: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00019960: 2020 5b6c 656e 286c 6f67 6d6f 6465 6c2e    [len(logmodel.
-00019970: 6669 745f 7661 7273 2e6b 6579 7328 2929  fit_vars.keys())
-00019980: 2066 6f72 206c 6f67 6d6f 6465 6c20 696e   for logmodel in
-00019990: 2073 656c 662e 6c6f 676d 6f64 656c 735d   self.logmodels]
-000199a0: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-000199b0: 2020 2020 2020 2020 2020 2020 7374 6465              stde
-000199c0: 7620 3d20 5b6e 702e 6e61 6e5d 202a 206e  v = [np.nan] * n
-000199d0: 5f66 6974 7465 645f 7061 7273 0a20 2020  _fitted_pars.   
-000199e0: 2020 2020 2020 2020 2073 656c 662e 6669           self.fi
-000199f0: 745f 7374 6174 7573 203d 2046 616c 7365  t_status = False
-00019a00: 0a20 2020 2020 2020 2065 6c73 653a 0a0a  .        else:..
-00019a10: 2020 2020 2020 2020 2020 2020 7374 6465              stde
-00019a20: 762c 206e 6f5f 7374 6465 7620 3d20 7374  v, no_stdev = st
-00019a30: 6174 732e 7376 645f 7374 6465 7628 6375  ats.svd_stdev(cu
-00019a40: 7272 5f66 6974 290a 0a20 2020 2020 2020  rr_fit)..       
-00019a50: 2020 2020 2073 656c 662e 6669 745f 7374       self.fit_st
-00019a60: 6174 7573 203d 2054 7275 650a 0a20 2020  atus = True..   
-00019a70: 2020 2020 2023 2041 6464 2070 6172 616d       # Add param
-00019a80: 6574 6572 732c 2073 7461 7475 7320 616e  eters, status an
-00019a90: 6420 7374 6465 7620 746f 2065 6163 6820  d stdev to each 
-00019aa0: 4c6f 6754 6175 544d 6f64 656c 0a20 2020  LogTauTModel.   
-00019ab0: 2020 2020 2069 7420 3d20 300a 2020 2020       it = 0.    
-00019ac0: 2020 2020 666f 7220 6c6f 676d 6f64 656c      for logmodel
-00019ad0: 2069 6e20 7365 6c66 2e6c 6f67 6d6f 6465   in self.logmode
-00019ae0: 6c73 3a0a 0a20 2020 2020 2020 2020 2020  ls:..           
-00019af0: 2023 204e 616d 6520 6f66 2066 6974 7465   # Name of fitte
-00019b00: 6420 7661 7269 6162 6c65 7320 696e 2074  d variables in t
-00019b10: 6869 7320 6c6f 676d 6f64 656c 0a20 2020  his logmodel.   
-00019b20: 2020 2020 2020 2020 2066 6974 5f76 6172           fit_var
-00019b30: 5f6e 616d 6573 203d 206c 6f67 6d6f 6465  _names = logmode
-00019b40: 6c2e 6669 745f 7661 7273 2e6b 6579 7328  l.fit_vars.keys(
-00019b50: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
-00019b60: 4e75 6d62 6572 206f 6620 7061 7261 6d65  Number of parame
-00019b70: 7465 7273 2066 6f72 2074 6869 7320 6c6f  ters for this lo
-00019b80: 676d 6f64 656c 0a20 2020 2020 2020 2020  gmodel.         
-00019b90: 2020 206e 5f70 6172 7320 3d20 6c65 6e28     n_pars = len(
-00019ba0: 6669 745f 7661 725f 6e61 6d65 7329 0a0a  fit_var_names)..
-00019bb0: 2020 2020 2020 2020 2020 2020 2320 5365              # Se
-00019bc0: 7420 6561 6368 2073 7461 6e64 6172 6420  t each standard 
-00019bd0: 6465 7669 6174 696f 6e0a 2020 2020 2020  deviation.      
-00019be0: 2020 2020 2020 5f73 7464 6576 203d 2073        _stdev = s
-00019bf0: 7464 6576 5b69 743a 2069 7420 2b20 6e5f  tdev[it: it + n_
-00019c00: 7061 7273 5d0a 2020 2020 2020 2020 2020  pars].          
-00019c10: 2020 6c6f 676d 6f64 656c 2e66 6974 5f73    logmodel.fit_s
-00019c20: 7464 6576 203d 207b 0a20 2020 2020 2020  tdev = {.       
-00019c30: 2020 2020 2020 2020 206c 6162 656c 3a20           label: 
-00019c40: 7661 6c0a 2020 2020 2020 2020 2020 2020  val.            
-00019c50: 2020 2020 666f 7220 6c61 6265 6c2c 2076      for label, v
-00019c60: 616c 2069 6e20 7a69 7028 0a20 2020 2020  al in zip(.     
-00019c70: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00019c80: 6974 5f76 6172 5f6e 616d 6573 2c20 5f73  it_var_names, _s
-00019c90: 7464 6576 0a20 2020 2020 2020 2020 2020  tdev.           
-00019ca0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00019cb0: 2020 207d 0a0a 2020 2020 2020 2020 2020     }..          
-00019cc0: 2020 2320 5265 706f 7274 2073 696e 6775    # Report singu
-00019cd0: 6c61 7220 7661 6c75 6573 3d30 206f 6620  lar values=0 of 
-00019ce0: 4a61 636f 6269 616e 0a20 2020 2020 2020  Jacobian.       
-00019cf0: 2020 2020 2023 2061 6e64 2069 6e64 6963       # and indic
-00019d00: 6174 6520 7468 6174 2073 7464 5f64 6576  ate that std_dev
-00019d10: 2063 616e 6e6f 7420 6265 2063 616c 6375   cannot be calcu
-00019d20: 6c61 7465 640a 2020 2020 2020 2020 2020  lated.          
-00019d30: 2020 7369 6e67 7320 3d20 6e6f 5f73 7464    sings = no_std
-00019d40: 6576 5b69 743a 2069 7420 2b20 6e5f 7061  ev[it: it + n_pa
-00019d50: 7273 5d0a 2020 2020 2020 2020 2020 2020  rs].            
-00019d60: 666f 7220 7061 722c 2073 6920 696e 207a  for par, si in z
-00019d70: 6970 2866 6974 5f76 6172 5f6e 616d 6573  ip(fit_var_names
-00019d80: 2c20 7369 6e67 7329 3a0a 2020 2020 2020  , sings):.      
-00019d90: 2020 2020 2020 2020 2020 6966 2076 6572            if ver
-00019da0: 626f 7365 2061 6e64 206e 6f74 2073 693a  bose and not si:
-00019db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019dc0: 2020 2020 2075 742e 6370 7269 6e74 280a       ut.cprint(.
-00019dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019de0: 2020 2020 2020 2020 6627 5761 726e 696e          f'Warnin
-00019df0: 673a 204a 6163 6f62 6961 6e20 6973 2064  g: Jacobian is d
-00019e00: 6567 656e 6572 6174 6520 666f 7220 7b70  egenerate for {p
-00019e10: 6172 7d2c 2073 7461 6e64 6172 6420 6465  ar}, standard de
-00019e20: 7669 6174 696f 6e20 6361 6e6e 6f74 2062  viation cannot b
-00019e30: 6520 666f 756e 642c 2061 6e64 2069 7320  e found, and is 
-00019e40: 7365 7420 746f 207a 6572 6f5c 6e27 2c20  set to zero\n', 
-00019e50: 2320 6e6f 7161 0a20 2020 2020 2020 2020  # noqa.         
-00019e60: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00019e70: 626c 6163 6b5f 7965 6c6c 6f77 6267 270a  black_yellowbg'.
-00019e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019e90: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
-00019ea0: 2020 2023 2053 6574 2066 696e 616c 2066     # Set final f
-00019eb0: 6974 7465 6420 7661 6c75 6573 0a20 2020  itted values.   
-00019ec0: 2020 2020 2020 2020 205f 7661 6c73 203d           _vals =
-00019ed0: 2063 7572 725f 6669 742e 785b 6974 3a20   curr_fit.x[it: 
-00019ee0: 6974 202b 206e 5f70 6172 735d 0a20 2020  it + n_pars].   
-00019ef0: 2020 2020 2020 2020 206c 6f67 6d6f 6465           logmode
-00019f00: 6c2e 6669 6e61 6c5f 7661 725f 7661 6c75  l.final_var_valu
-00019f10: 6573 203d 207b 0a20 2020 2020 2020 2020  es = {.         
-00019f20: 2020 2020 2020 206e 616d 653a 2076 616c         name: val
-00019f30: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
-00019f40: 2020 2066 6f72 206e 616d 652c 2076 616c     for name, val
-00019f50: 7565 2069 6e20 7a69 7028 6669 745f 7661  ue in zip(fit_va
-00019f60: 725f 6e61 6d65 732c 205f 7661 6c73 290a  r_names, _vals).
-00019f70: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00019f80: 2020 2020 2020 2020 2020 2320 616e 6420            # and 
-00019f90: 6669 7865 6420 7661 6c75 6573 0a20 2020  fixed values.   
-00019fa0: 2020 2020 2020 2020 2066 6f72 206b 6579           for key
-00019fb0: 2c20 7661 6c20 696e 206c 6f67 6d6f 6465  , val in logmode
-00019fc0: 6c2e 6669 785f 7661 7273 2e69 7465 6d73  l.fix_vars.items
-00019fd0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00019fe0: 2020 2020 6c6f 676d 6f64 656c 2e66 696e      logmodel.fin
-00019ff0: 616c 5f76 6172 5f76 616c 7565 735b 6b65  al_var_values[ke
-0001a000: 795d 203d 2076 616c 0a0a 2020 2020 2020  y] = val..      
-0001a010: 2020 2020 2020 6974 202b 3d20 6e5f 7061        it += n_pa
-0001a020: 7273 0a0a 2020 2020 2020 2020 7265 7475  rs..        retu
-0001a030: 726e 0a0a 0a63 6c61 7373 2046 6974 5769  rn...class FitWi
-0001a040: 6e64 6f77 2851 7457 6964 6765 7473 2e51  ndow(QtWidgets.Q
-0001a050: 4d61 696e 5769 6e64 6f77 293a 0a20 2020  MainWindow):.   
-0001a060: 2027 2727 0a20 2020 2049 6e74 6572 6163   '''.    Interac
-0001a070: 7469 7665 2046 6974 2057 696e 646f 7720  tive Fit Window 
-0001a080: 666f 7220 7261 7465 2076 7320 7465 6d70  for rate vs temp
-0001a090: 6572 6174 7572 652f 6669 656c 6420 6461  erature/field da
-0001a0a0: 7461 2066 6974 7469 6e67 0a20 2020 2027  ta fitting.    '
-0001a0b0: 2727 0a0a 2020 2020 6465 6620 5f5f 696e  ''..    def __in
-0001a0c0: 6974 5f5f 2873 656c 662c 2064 6174 6173  it__(self, datas
-0001a0d0: 6574 3a20 5461 7554 4461 7461 7365 7420  et: TauTDataset 
-0001a0e0: 7c20 5461 7548 4461 7461 7365 742c 2075  | TauHDataset, u
-0001a0f0: 7365 6c3a 206f 626a 6563 742c 0a20 2020  sel: object,.   
-0001a100: 2020 2020 2020 2020 2020 2020 2020 7375                su
-0001a110: 7070 6f72 7465 645f 6d6f 6465 6c73 3a20  pported_models: 
-0001a120: 6c69 7374 2c0a 2020 2020 2020 2020 2020  list,.          
-0001a130: 2020 2020 2020 2077 6964 6765 745f 6465         widget_de
-0001a140: 6661 756c 7473 3a20 6469 6374 5b73 7472  faults: dict[str
-0001a150: 2c20 6469 6374 5b73 7472 2c20 666c 6f61  , dict[str, floa
-0001a160: 745d 5d20 3d20 6775 692e 7769 6467 6574  t]] = gui.widget
-0001a170: 5f64 6566 6175 6c74 732c 2023 206e 6f71  _defaults, # noq
-0001a180: 610a 2020 2020 2020 2020 2020 2020 2020  a.              
-0001a190: 2020 202a 6172 6773 2c20 2a2a 6b77 6172     *args, **kwar
-0001a1a0: 6773 293a 0a0a 2020 2020 2020 2020 7375  gs):..        su
-0001a1b0: 7065 7228 4669 7457 696e 646f 772c 2073  per(FitWindow, s
-0001a1c0: 656c 6629 2e5f 5f69 6e69 745f 5f28 2a61  elf).__init__(*a
-0001a1d0: 7267 732c 202a 2a6b 7761 7267 7329 0a0a  rgs, **kwargs)..
-0001a1e0: 2020 2020 2020 2020 2320 4164 6420 7368          # Add sh
-0001a1f0: 6f72 7463 7574 2074 6f20 7072 6573 7320  ortcut to press 
-0001a200: 7120 746f 2071 7569 740a 2020 2020 2020  q to quit.      
-0001a210: 2020 7365 6c66 2e65 7869 745f 7368 6f72    self.exit_shor
-0001a220: 7463 7574 203d 2051 7457 6964 6765 7473  tcut = QtWidgets
-0001a230: 2e51 5368 6f72 7463 7574 2851 7447 7569  .QShortcut(QtGui
-0001a240: 2e51 4b65 7953 6571 7565 6e63 6528 2771  .QKeySequence('q
-0001a250: 2729 2c20 7365 6c66 290a 2020 2020 2020  '), self).      
-0001a260: 2020 7365 6c66 2e65 7869 745f 7368 6f72    self.exit_shor
-0001a270: 7463 7574 2e61 6374 6976 6174 6564 2e63  tcut.activated.c
-0001a280: 6f6e 6e65 6374 280a 2020 2020 2020 2020  onnect(.        
-0001a290: 2020 2020 6c61 6d62 6461 3a20 7365 6c66      lambda: self
-0001a2a0: 2e63 6c6f 7365 2829 0a20 2020 2020 2020  .close().       
-0001a2b0: 2029 0a0a 2020 2020 2020 2020 7365 6c66   )..        self
-0001a2c0: 2e73 6574 5769 6e64 6f77 5469 746c 6528  .setWindowTitle(
-0001a2d0: 2749 6e74 6572 6163 7469 7665 2052 656c  'Interactive Rel
-0001a2e0: 6178 6174 696f 6e20 5072 6f66 696c 6527  axation Profile'
-0001a2f0: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-0001a300: 7365 7441 7474 7269 6275 7465 2851 7443  setAttribute(QtC
-0001a310: 6f72 652e 5174 2e57 415f 4465 6c65 7465  ore.Qt.WA_Delete
-0001a320: 4f6e 436c 6f73 6529 0a20 2020 2020 2020  OnClose).       
-0001a330: 2073 656c 662e 7365 7453 7479 6c65 5368   self.setStyleSh
-0001a340: 6565 7428 0a20 2020 2020 2020 2020 2020  eet(.           
-0001a350: 2027 2727 0a20 2020 2020 2020 2020 2020   '''.           
-0001a360: 2051 4d61 696e 5769 6e64 6f77 207b 0a20   QMainWindow {. 
-0001a370: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-0001a380: 6163 6b67 726f 756e 642d 636f 6c6f 723a  ackground-color:
-0001a390: 2077 6869 7465 0a20 2020 2020 2020 2020   white.         
-0001a3a0: 2020 207d 0a0a 2020 2020 2020 2020 2020     }..          
-0001a3b0: 2020 5143 6865 636b 426f 7820 7b0a 2020    QCheckBox {.  
-0001a3c0: 2020 2020 2020 2020 2020 2020 2020 7370                sp
-0001a3d0: 6163 696e 673a 2035 7078 3b0a 2020 2020  acing: 5px;.    
-0001a3e0: 2020 2020 2020 2020 2020 2020 666f 6e74              font
-0001a3f0: 2d73 697a 653a 3135 7078 3b0a 2020 2020  -size:15px;.    
-0001a400: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-0001a410: 2020 2020 2020 5153 6c69 6465 723a 3a67        QSlider::g
-0001a420: 726f 6f76 653a 686f 7269 7a6f 6e74 616c  roove:horizontal
-0001a430: 207b 0a20 2020 2020 2020 2020 2020 2062   {.            b
-0001a440: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
-0001a450: 2023 6262 623b 0a20 2020 2020 2020 2020   #bbb;.         
-0001a460: 2020 2062 6163 6b67 726f 756e 643a 2077     background: w
-0001a470: 6869 7465 3b0a 2020 2020 2020 2020 2020  hite;.          
-0001a480: 2020 6865 6967 6874 3a20 3130 7078 3b0a    height: 10px;.
-0001a490: 2020 2020 2020 2020 2020 2020 626f 7264              bord
-0001a4a0: 6572 2d72 6164 6975 733a 2034 7078 3b0a  er-radius: 4px;.
-0001a4b0: 2020 2020 2020 2020 2020 2020 7d0a 0a20              }.. 
-0001a4c0: 2020 2020 2020 2020 2020 2051 536c 6964             QSlid
-0001a4d0: 6572 3a3a 7375 622d 7061 6765 3a68 6f72  er::sub-page:hor
-0001a4e0: 697a 6f6e 7461 6c20 7b0a 2020 2020 2020  izontal {.      
-0001a4f0: 2020 2020 2020 6261 636b 6772 6f75 6e64        background
-0001a500: 3a20 716c 696e 6561 7267 7261 6469 656e  : qlineargradien
-0001a510: 7428 7831 3a20 302c 2079 313a 2030 2c20  t(x1: 0, y1: 0, 
-0001a520: 2020 2078 323a 2030 2c20 7932 3a20 312c     x2: 0, y2: 1,
-0001a530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a540: 2073 746f 703a 2030 2023 3636 652c 2073   stop: 0 #66e, s
-0001a550: 746f 703a 2031 2023 6262 6629 3b0a 2020  top: 1 #bbf);.  
-0001a560: 2020 2020 2020 2020 2020 6261 636b 6772            backgr
-0001a570: 6f75 6e64 3a20 716c 696e 6561 7267 7261  ound: qlineargra
-0001a580: 6469 656e 7428 7831 3a20 302c 2079 313a  dient(x1: 0, y1:
-0001a590: 2030 2e32 2c20 7832 3a20 312c 2079 323a   0.2, x2: 1, y2:
-0001a5a0: 2031 2c0a 2020 2020 2020 2020 2020 2020   1,.            
-0001a5b0: 2020 2020 7374 6f70 3a20 3020 2362 6266      stop: 0 #bbf
-0001a5c0: 2c20 7374 6f70 3a20 3120 2335 3566 293b  , stop: 1 #55f);
-0001a5d0: 0a20 2020 2020 2020 2020 2020 2062 6f72  .            bor
-0001a5e0: 6465 723a 2031 7078 2073 6f6c 6964 2023  der: 1px solid #
-0001a5f0: 3737 373b 0a20 2020 2020 2020 2020 2020  777;.           
-0001a600: 2068 6569 6768 743a 2031 3070 783b 0a20   height: 10px;. 
-0001a610: 2020 2020 2020 2020 2020 2062 6f72 6465             borde
-0001a620: 722d 7261 6469 7573 3a20 3470 783b 0a20  r-radius: 4px;. 
-0001a630: 2020 2020 2020 2020 2020 207d 0a0a 2020             }..  
-0001a640: 2020 2020 2020 2020 2020 5153 6c69 6465            QSlide
-0001a650: 723a 3a61 6464 2d70 6167 653a 686f 7269  r::add-page:hori
-0001a660: 7a6f 6e74 616c 207b 0a20 2020 2020 2020  zontal {.       
-0001a670: 2020 2020 2062 6163 6b67 726f 756e 643a       background:
-0001a680: 2023 6666 663b 0a20 2020 2020 2020 2020   #fff;.         
-0001a690: 2020 2062 6f72 6465 723a 2031 7078 2073     border: 1px s
-0001a6a0: 6f6c 6964 2023 3737 373b 0a20 2020 2020  olid #777;.     
-0001a6b0: 2020 2020 2020 2068 6569 6768 743a 2031         height: 1
-0001a6c0: 3070 783b 0a20 2020 2020 2020 2020 2020  0px;.           
-0001a6d0: 2062 6f72 6465 722d 7261 6469 7573 3a20   border-radius: 
-0001a6e0: 3470 783b 0a20 2020 2020 2020 2020 2020  4px;.           
-0001a6f0: 207d 0a0a 2020 2020 2020 2020 2020 2020   }..            
-0001a700: 5153 6c69 6465 723a 3a68 616e 646c 653a  QSlider::handle:
-0001a710: 686f 7269 7a6f 6e74 616c 207b 0a20 2020  horizontal {.   
-0001a720: 2020 2020 2020 2020 2062 6163 6b67 726f           backgro
-0001a730: 756e 643a 2071 6c69 6e65 6172 6772 6164  und: qlineargrad
-0001a740: 6965 6e74 2878 313a 302c 2079 313a 302c  ient(x1:0, y1:0,
-0001a750: 2078 323a 312c 2079 323a 312c 0a20 2020   x2:1, y2:1,.   
-0001a760: 2020 2020 2020 2020 2020 2020 2073 746f               sto
-0001a770: 703a 3020 2365 6565 2c20 7374 6f70 3a31  p:0 #eee, stop:1
-0001a780: 2023 6363 6329 3b0a 2020 2020 2020 2020   #ccc);.        
-0001a790: 2020 2020 626f 7264 6572 3a20 3170 7820      border: 1px 
-0001a7a0: 736f 6c69 6420 2337 3737 3b0a 2020 2020  solid #777;.    
-0001a7b0: 2020 2020 2020 2020 7769 6474 683a 2031          width: 1
-0001a7c0: 3370 783b 0a20 2020 2020 2020 2020 2020  3px;.           
-0001a7d0: 206d 6172 6769 6e2d 746f 703a 202d 3270   margin-top: -2p
-0001a7e0: 783b 0a20 2020 2020 2020 2020 2020 206d  x;.            m
-0001a7f0: 6172 6769 6e2d 626f 7474 6f6d 3a20 2d32  argin-bottom: -2
-0001a800: 7078 3b0a 2020 2020 2020 2020 2020 2020  px;.            
-0001a810: 626f 7264 6572 2d72 6164 6975 733a 2034  border-radius: 4
-0001a820: 7078 3b0a 2020 2020 2020 2020 2020 2020  px;.            
-0001a830: 7d0a 0a20 2020 2020 2020 2020 2020 2051  }..            Q
-0001a840: 536c 6964 6572 3a3a 6861 6e64 6c65 3a68  Slider::handle:h
-0001a850: 6f72 697a 6f6e 7461 6c3a 686f 7665 7220  orizontal:hover 
-0001a860: 7b0a 2020 2020 2020 2020 2020 2020 6261  {.            ba
-0001a870: 636b 6772 6f75 6e64 3a20 716c 696e 6561  ckground: qlinea
-0001a880: 7267 7261 6469 656e 7428 7831 3a30 2c20  rgradient(x1:0, 
-0001a890: 7931 3a30 2c20 7832 3a31 2c20 7932 3a31  y1:0, x2:1, y2:1
-0001a8a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001a8b0: 2020 7374 6f70 3a30 2023 6666 662c 2073    stop:0 #fff, s
-0001a8c0: 746f 703a 3120 2364 6464 293b 0a20 2020  top:1 #ddd);.   
-0001a8d0: 2020 2020 2020 2020 2062 6f72 6465 723a           border:
-0001a8e0: 2031 7078 2073 6f6c 6964 2023 3434 343b   1px solid #444;
-0001a8f0: 0a20 2020 2020 2020 2020 2020 2062 6f72  .            bor
-0001a900: 6465 722d 7261 6469 7573 3a20 3470 783b  der-radius: 4px;
-0001a910: 0a20 2020 2020 2020 2020 2020 207d 0a0a  .            }..
-0001a920: 2020 2020 2020 2020 2020 2020 5153 6c69              QSli
-0001a930: 6465 723a 3a73 7562 2d70 6167 653a 686f  der::sub-page:ho
-0001a940: 7269 7a6f 6e74 616c 3a64 6973 6162 6c65  rizontal:disable
-0001a950: 6420 7b0a 2020 2020 2020 2020 2020 2020  d {.            
-0001a960: 6261 636b 6772 6f75 6e64 3a20 2362 6262  background: #bbb
-0001a970: 3b0a 2020 2020 2020 2020 2020 2020 626f  ;.            bo
-0001a980: 7264 6572 2d63 6f6c 6f72 3a20 2339 3939  rder-color: #999
-0001a990: 3b0a 2020 2020 2020 2020 2020 2020 7d0a  ;.            }.
-0001a9a0: 0a20 2020 2020 2020 2020 2020 2051 536c  .            QSl
-0001a9b0: 6964 6572 3a3a 6164 642d 7061 6765 3a68  ider::add-page:h
-0001a9c0: 6f72 697a 6f6e 7461 6c3a 6469 7361 626c  orizontal:disabl
-0001a9d0: 6564 207b 0a20 2020 2020 2020 2020 2020  ed {.           
-0001a9e0: 2062 6163 6b67 726f 756e 643a 2023 6565   background: #ee
-0001a9f0: 653b 0a20 2020 2020 2020 2020 2020 2062  e;.            b
-0001aa00: 6f72 6465 722d 636f 6c6f 723a 2023 3939  order-color: #99
-0001aa10: 393b 0a20 2020 2020 2020 2020 2020 207d  9;.            }
-0001aa20: 0a0a 2020 2020 2020 2020 2020 2020 5153  ..            QS
-0001aa30: 6c69 6465 723a 3a68 616e 646c 653a 686f  lider::handle:ho
-0001aa40: 7269 7a6f 6e74 616c 3a64 6973 6162 6c65  rizontal:disable
-0001aa50: 6420 7b0a 2020 2020 2020 2020 2020 2020  d {.            
-0001aa60: 6261 636b 6772 6f75 6e64 3a20 2365 6565  background: #eee
-0001aa70: 3b0a 2020 2020 2020 2020 2020 2020 626f  ;.            bo
-0001aa80: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
-0001aa90: 2361 6161 3b0a 2020 2020 2020 2020 2020  #aaa;.          
-0001aaa0: 2020 626f 7264 6572 2d72 6164 6975 733a    border-radius:
-0001aab0: 2034 7078 3b0a 2020 2020 2020 2020 2020   4px;.          
-0001aac0: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-0001aad0: 2727 270a 2020 2020 2020 2020 290a 0a20  '''.        ).. 
-0001aae0: 2020 2020 2020 2023 2053 6574 2064 6566         # Set def
-0001aaf0: 6175 6c74 206d 696e 2c20 6d61 782c 2069  ault min, max, i
-0001ab00: 6e69 742c 2061 6e64 2073 7465 7020 7661  nit, and step va
-0001ab10: 6c75 6573 206f 6620 736c 6964 6572 7320  lues of sliders 
-0001ab20: 616e 6420 7465 7874 2062 6f78 6573 0a20  and text boxes. 
-0001ab30: 2020 2020 2020 2073 656c 662e 6465 6661         self.defa
-0001ab40: 756c 7473 203d 2077 6964 6765 745f 6465  ults = widget_de
-0001ab50: 6661 756c 7473 0a0a 2020 2020 2020 2020  faults..        
-0001ab60: 2320 4469 6374 696f 6e61 7279 2066 6f72  # Dictionary for
-0001ab70: 2074 6963 6b62 6f78 2077 6964 6765 7473   tickbox widgets
-0001ab80: 0a20 2020 2020 2020 2073 656c 662e 7469  .        self.ti
-0001ab90: 636b 6469 6374 203d 207b 0a20 2020 2020  ckdict = {.     
-0001aba0: 2020 2020 2020 206d 6f64 656c 2e4e 414d         model.NAM
-0001abb0: 452e 6c6f 7765 7228 293a 204e 6f6e 650a  E.lower(): None.
-0001abc0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0001abd0: 6d6f 6465 6c20 696e 2073 7570 706f 7274  model in support
-0001abe0: 6564 5f6d 6f64 656c 730a 2020 2020 2020  ed_models.      
-0001abf0: 2020 7d0a 0a20 2020 2020 2020 2023 2044    }..        # D
-0001ac00: 6963 7469 6f6e 6172 7920 666f 7220 7061  ictionary for pa
-0001ac10: 7261 6d65 7465 7220 736c 6964 6572 2c20  rameter slider, 
-0001ac20: 656e 7472 792c 2061 6e64 2066 6974 6669  entry, and fitfi
-0001ac30: 7820 7769 6467 6574 730a 2020 2020 2020  x widgets.      
-0001ac40: 2020 7365 6c66 2e77 6964 6765 7464 6963    self.widgetdic
-0001ac50: 7420 3d20 7b0a 2020 2020 2020 2020 2020  t = {.          
-0001ac60: 2020 6d6f 6465 6c2e 4e41 4d45 2e6c 6f77    model.NAME.low
-0001ac70: 6572 2829 3a20 7b0a 2020 2020 2020 2020  er(): {.        
-0001ac80: 2020 2020 2020 2020 7061 726e 616d 653a          parname:
-0001ac90: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-0001aca0: 2020 2020 2020 2027 736c 6964 6572 273a         'slider':
-0001acb0: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-0001acc0: 2020 2020 2020 2020 2020 2027 6666 5f74             'ff_t
-0001acd0: 6f67 676c 6527 3a20 4e6f 6e65 2c0a 2020  oggle': None,.  
-0001ace0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001acf0: 2020 2765 6e74 7279 273a 204e 6f6e 650a    'entry': None.
-0001ad00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ad10: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-0001ad20: 2020 666f 7220 7061 726e 616d 6520 696e    for parname in
-0001ad30: 206d 6f64 656c 2e50 4152 4e41 4d45 530a   model.PARNAMES.
-0001ad40: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-0001ad50: 2020 2020 2020 2020 2020 666f 7220 6d6f            for mo
-0001ad60: 6465 6c20 696e 2073 7570 706f 7274 6564  del in supported
-0001ad70: 5f6d 6f64 656c 730a 2020 2020 2020 2020  _models.        
-0001ad80: 7d0a 0a20 2020 2020 2020 2023 204d 696e  }..        # Min
-0001ad90: 696d 756d 2057 696e 646f 7720 7369 7a65  imum Window size
-0001ada0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-0001adb0: 744d 696e 696d 756d 5369 7a65 2851 7443  tMinimumSize(QtC
-0001adc0: 6f72 652e 5153 697a 6528 3132 3030 2c20  ore.QSize(1200, 
-0001add0: 3730 3029 290a 0a20 2020 2020 2020 2023  700))..        #
-0001ade0: 204d 616b 6520 7769 6467 6574 7320 666f   Make widgets fo
-0001adf0: 7220 656e 7469 7265 2077 696e 646f 770a  r entire window.
-0001ae00: 2020 2020 2020 2020 7365 6c66 2e77 6964          self.wid
-0001ae10: 6765 7420 3d20 5174 5769 6467 6574 732e  get = QtWidgets.
-0001ae20: 5157 6964 6765 7428 7061 7265 6e74 3d73  QWidget(parent=s
-0001ae30: 656c 6629 0a20 2020 2020 2020 2073 656c  elf).        sel
-0001ae40: 662e 7365 7443 656e 7472 616c 5769 6467  f.setCentralWidg
-0001ae50: 6574 2873 656c 662e 7769 6467 6574 290a  et(self.widget).
-0001ae60: 2020 2020 2020 2020 626f 745f 726f 775f          bot_row_
-0001ae70: 7769 6467 6574 203d 2051 7457 6964 6765  widget = QtWidge
-0001ae80: 7473 2e51 5769 6467 6574 2873 656c 662e  ts.QWidget(self.
-0001ae90: 7769 6467 6574 290a 2020 2020 2020 2020  widget).        
-0001aea0: 746f 705f 726f 775f 7769 6467 6574 203d  top_row_widget =
-0001aeb0: 2051 7457 6964 6765 7473 2e51 5769 6467   QtWidgets.QWidg
-0001aec0: 6574 2873 656c 662e 7769 6467 6574 290a  et(self.widget).
-0001aed0: 2020 2020 2020 2020 7268 735f 636f 6c5f          rhs_col_
-0001aee0: 7769 6467 6574 203d 2051 7457 6964 6765  widget = QtWidge
-0001aef0: 7473 2e51 5769 6467 6574 2874 6f70 5f72  ts.QWidget(top_r
-0001af00: 6f77 5f77 6964 6765 7429 0a0a 2020 2020  ow_widget)..    
-0001af10: 2020 2020 7268 735f 636f 6c5f 7363 726f      rhs_col_scro
-0001af20: 6c6c 203d 2051 7457 6964 6765 7473 2e51  ll = QtWidgets.Q
-0001af30: 5363 726f 6c6c 4172 6561 2872 6873 5f63  ScrollArea(rhs_c
-0001af40: 6f6c 5f77 6964 6765 7429 0a20 2020 2020  ol_widget).     
-0001af50: 2020 2072 6873 5f63 6f6c 5f73 6372 6f6c     rhs_col_scrol
-0001af60: 6c2e 7365 7456 6572 7469 6361 6c53 6372  l.setVerticalScr
-0001af70: 6f6c 6c42 6172 506f 6c69 6379 280a 2020  ollBarPolicy(.  
-0001af80: 2020 2020 2020 2020 2020 5174 436f 7265            QtCore
-0001af90: 2e51 742e 5363 726f 6c6c 4261 7241 6c77  .Qt.ScrollBarAlw
-0001afa0: 6179 734f 6e0a 2020 2020 2020 2020 290a  aysOn.        ).
-0001afb0: 2020 2020 2020 2020 7268 735f 636f 6c5f          rhs_col_
-0001afc0: 7363 726f 6c6c 2e73 6574 486f 7269 7a6f  scroll.setHorizo
-0001afd0: 6e74 616c 5363 726f 6c6c 4261 7250 6f6c  ntalScrollBarPol
-0001afe0: 6963 7928 0a20 2020 2020 2020 2020 2020  icy(.           
-0001aff0: 2051 7443 6f72 652e 5174 2e53 6372 6f6c   QtCore.Qt.Scrol
-0001b000: 6c42 6172 416c 7761 7973 4f66 660a 2020  lBarAlwaysOff.  
-0001b010: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0001b020: 7268 735f 636f 6c5f 7363 726f 6c6c 2e73  rhs_col_scroll.s
-0001b030: 6574 5769 6467 6574 5265 7369 7a61 626c  etWidgetResizabl
-0001b040: 6528 5472 7565 290a 0a20 2020 2020 2020  e(True)..       
-0001b050: 2073 6372 6f6c 6c5f 636f 6e74 6169 6e65   scroll_containe
-0001b060: 7220 3d20 5174 5769 6467 6574 732e 5157  r = QtWidgets.QW
-0001b070: 6964 6765 7428 7268 735f 636f 6c5f 7363  idget(rhs_col_sc
-0001b080: 726f 6c6c 290a 2020 2020 2020 2020 7268  roll).        rh
-0001b090: 735f 636f 6c5f 7363 726f 6c6c 2e73 6574  s_col_scroll.set
-0001b0a0: 5769 6467 6574 2873 6372 6f6c 6c5f 636f  Widget(scroll_co
-0001b0b0: 6e74 6169 6e65 7229 0a0a 2020 2020 2020  ntainer)..      
-0001b0c0: 2020 6c68 735f 636f 6c5f 7769 6467 6574    lhs_col_widget
-0001b0d0: 203d 2051 7457 6964 6765 7473 2e51 5769   = QtWidgets.QWi
-0001b0e0: 6467 6574 2874 6f70 5f72 6f77 5f77 6964  dget(top_row_wid
-0001b0f0: 6765 7429 0a0a 2020 2020 2020 2020 2320  get)..        # 
-0001b100: 4c48 5320 636f 6c75 6d6e 202d 2070 6c6f  LHS column - plo
-0001b110: 7420 6f6e 6c79 0a20 2020 2020 2020 206c  t only.        l
-0001b120: 6873 5f63 6f6c 5f6c 6179 6f75 7420 3d20  hs_col_layout = 
-0001b130: 5174 5769 6467 6574 732e 5156 426f 784c  QtWidgets.QVBoxL
-0001b140: 6179 6f75 7428 6c68 735f 636f 6c5f 7769  ayout(lhs_col_wi
-0001b150: 6467 6574 290a 0a20 2020 2020 2020 2023  dget)..        #
-0001b160: 206d 616b 6520 7067 6670 6c6f 7473 2070   make pgfplots p
-0001b170: 6c6f 7420 7769 6467 6574 0a20 2020 2020  lot widget.     
-0001b180: 2020 2073 656c 662e 706c 6f74 5f77 6964     self.plot_wid
-0001b190: 6765 7420 3d20 7067 2e50 6c6f 7457 6964  get = pg.PlotWid
-0001b1a0: 6765 7428 0a20 2020 2020 2020 2020 2020  get(.           
-0001b1b0: 2070 6172 656e 743d 6c68 735f 636f 6c5f   parent=lhs_col_
-0001b1c0: 7769 6467 6574 0a20 2020 2020 2020 2029  widget.        )
-0001b1d0: 0a20 2020 2020 2020 2023 2041 6464 2070  .        # Add p
-0001b1e0: 6c6f 7420 746f 206c 6566 7420 636f 6c75  lot to left colu
-0001b1f0: 6d6e 0a20 2020 2020 2020 206c 6873 5f63  mn.        lhs_c
-0001b200: 6f6c 5f6c 6179 6f75 742e 6164 6457 6964  ol_layout.addWid
-0001b210: 6765 7428 7365 6c66 2e70 6c6f 745f 7769  get(self.plot_wi
-0001b220: 6467 6574 290a 0a20 2020 2020 2020 2023  dget)..        #
-0001b230: 2053 6574 206c 6f67 6c6f 6720 6178 6573   Set loglog axes
-0001b240: 0a20 2020 2020 2020 2073 656c 662e 706c  .        self.pl
-0001b250: 6f74 5f77 6964 6765 742e 7365 744c 6f67  ot_widget.setLog
-0001b260: 4d6f 6465 2854 7275 652c 2054 7275 6529  Mode(True, True)
-0001b270: 0a0a 2020 2020 2020 2020 2320 5365 7420  ..        # Set 
-0001b280: 7768 6974 6520 706c 6f74 2062 6163 6b67  white plot backg
-0001b290: 726f 756e 640a 2020 2020 2020 2020 7365  round.        se
-0001b2a0: 6c66 2e70 6c6f 745f 7769 6467 6574 2e73  lf.plot_widget.s
-0001b2b0: 6574 4261 636b 6772 6f75 6e64 2827 7727  etBackground('w'
-0001b2c0: 290a 0a20 2020 2020 2020 2023 2053 656c  )..        # Sel
-0001b2d0: 6563 7420 6569 7468 6572 2066 6965 6c64  ect either field
-0001b2e0: 206f 7220 7465 6d70 6572 6174 7572 6520   or temperature 
-0001b2f0: 6173 2078 2064 6174 6120 6261 7365 6420  as x data based 
-0001b300: 6f6e 2064 6174 6173 6574 2074 7970 650a  on dataset type.
-0001b310: 2020 2020 2020 2020 2320 616e 6420 7365          # and se
-0001b320: 7420 7820 6c61 6265 6c20 6f66 2070 6c6f  t x label of plo
-0001b330: 740a 2020 2020 2020 2020 6966 2069 7369  t.        if isi
-0001b340: 6e73 7461 6e63 6528 6461 7461 7365 742c  nstance(dataset,
-0001b350: 2054 6175 4844 6174 6173 6574 293a 0a20   TauHDataset):. 
-0001b360: 2020 2020 2020 2020 2020 2078 5f76 616c             x_val
-0001b370: 7320 3d20 636f 7079 2e63 6f70 7928 6461  s = copy.copy(da
-0001b380: 7461 7365 742e 6669 656c 6473 290a 2020  taset.fields).  
-0001b390: 2020 2020 2020 2020 2020 2320 5368 6966            # Shif
-0001b3a0: 7420 616c 6c20 6461 7461 2074 6f20 6265  t all data to be
-0001b3b0: 636f 6d65 2064 6566 696e 6564 2069 6e20  come defined in 
-0001b3c0: 6c6f 6731 3020 7370 6163 650a 2020 2020  log10 space.    
-0001b3d0: 2020 2020 2020 2020 2320 5468 6973 2073          # This s
-0001b3e0: 6869 6674 206d 7573 7420 6f6e 6c79 2062  hift must only b
-0001b3f0: 6520 6170 706c 6965 6420 7768 656e 2070  e applied when p
-0001b400: 6c6f 7474 696e 672c 206e 6f74 0a20 2020  lotting, not.   
-0001b410: 2020 2020 2020 2020 2023 2077 6865 6e20           # when 
-0001b420: 6361 6c63 756c 6174 696e 6720 7468 6520  calculating the 
-0001b430: 7661 6c75 6573 206f 6620 7468 6520 6675  values of the fu
-0001b440: 6e63 7469 6f6e 0a20 2020 2020 2020 2020  nction.         
-0001b450: 2020 2069 6620 616e 7928 7661 6c20 3c20     if any(val < 
-0001b460: 6e70 2e66 696e 666f 2866 6c6f 6174 292e  np.finfo(float).
-0001b470: 6570 7320 666f 7220 7661 6c20 696e 2078  eps for val in x
-0001b480: 5f76 616c 7329 3a0a 2020 2020 2020 2020  _vals):.        
-0001b490: 2020 2020 2020 2020 7365 6c66 2e6c 6f67          self.log
-0001b4a0: 7368 6966 7420 3d20 312e 0a20 2020 2020  shift = 1..     
-0001b4b0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0001b4c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0001b4d0: 662e 6c6f 6773 6869 6674 203d 2030 2e0a  f.logshift = 0..
-0001b4e0: 2020 2020 2020 2020 2020 2020 785f 7661              x_va
-0001b4f0: 6c73 202b 3d20 7365 6c66 2e6c 6f67 7368  ls += self.logsh
-0001b500: 6966 740a 2020 2020 2020 2020 2020 2020  ift.            
-0001b510: 7365 6c66 2e70 6c6f 745f 7769 6467 6574  self.plot_widget
-0001b520: 2e73 6574 4c61 6265 6c28 2762 6f74 746f  .setLabel('botto
-0001b530: 6d27 2c20 2746 6965 6c64 2028 4f65 2927  m', 'Field (Oe)'
-0001b540: 290a 0a20 2020 2020 2020 2065 6c69 6620  )..        elif 
-0001b550: 6973 696e 7374 616e 6365 2864 6174 6173  isinstance(datas
-0001b560: 6574 2c20 5461 7554 4461 7461 7365 7429  et, TauTDataset)
-0001b570: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0001b580: 6c66 2e6c 6f67 7368 6966 7420 3d20 302e  lf.logshift = 0.
-0001b590: 0a20 2020 2020 2020 2020 2020 2078 5f76  .            x_v
-0001b5a0: 616c 7320 3d20 636f 7079 2e63 6f70 7928  als = copy.copy(
-0001b5b0: 6461 7461 7365 742e 7465 6d70 6572 6174  dataset.temperat
-0001b5c0: 7572 6573 290a 2020 2020 2020 2020 2020  ures).          
-0001b5d0: 2020 7365 6c66 2e70 6c6f 745f 7769 6467    self.plot_widg
-0001b5e0: 6574 2e73 6574 4c61 6265 6c28 2762 6f74  et.setLabel('bot
-0001b5f0: 746f 6d27 2c20 2754 656d 7065 7261 7475  tom', 'Temperatu
-0001b600: 7265 2028 4b29 2729 0a0a 2020 2020 2020  re (K)')..      
-0001b610: 2020 2320 4578 7065 7269 6d65 6e74 616c    # Experimental
-0001b620: 2064 6174 610a 2020 2020 2020 2020 7365   data.        se
-0001b630: 6c66 2e65 7870 203d 2073 656c 662e 706c  lf.exp = self.pl
-0001b640: 6f74 5f77 6964 6765 742e 706c 6f74 280a  ot_widget.plot(.
-0001b650: 2020 2020 2020 2020 2020 2020 6e70 2e61              np.a
-0001b660: 7272 6179 2878 5f76 616c 7329 2c0a 2020  rray(x_vals),.  
-0001b670: 2020 2020 2020 2020 2020 6e70 2e61 7272            np.arr
-0001b680: 6179 2864 6174 6173 6574 2e72 6174 6573  ay(dataset.rates
-0001b690: 292c 0a20 2020 2020 2020 2020 2020 2070  ),.            p
-0001b6a0: 656e 3d4e 6f6e 652c 0a20 2020 2020 2020  en=None,.       
-0001b6b0: 2020 2020 2073 796d 626f 6c3d 2778 272c       symbol='x',
-0001b6c0: 0a20 2020 2020 2020 2020 2020 2073 796d  .            sym
-0001b6d0: 626f 6c42 7275 7368 3d28 302c 2030 2c20  bolBrush=(0, 0, 
-0001b6e0: 3029 0a20 2020 2020 2020 2029 0a0a 2020  0).        )..  
-0001b6f0: 2020 2020 2020 2320 4669 6e64 206e 6963        # Find nic
-0001b700: 6520 792d 6178 6973 206c 696d 6974 730a  e y-axis limits.
-0001b710: 2020 2020 2020 2020 795f 6c6f 7765 722c          y_lower,
-0001b720: 2079 5f75 7070 6572 203d 2067 7569 2e63   y_upper = gui.c
-0001b730: 616c 635f 795f 7261 7465 5f6c 696d 7328  alc_y_rate_lims(
-0001b740: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-0001b750: 6173 6574 2e72 6174 6573 2c0a 2020 2020  aset.rates,.    
-0001b760: 2020 2020 2020 2020 6e70 2e61 7272 6179          np.array
-0001b770: 2864 6174 6173 6574 2e72 6174 655f 706d  (dataset.rate_pm
-0001b780: 290a 2020 2020 2020 2020 290a 0a20 2020  ).        )..   
-0001b790: 2020 2020 2023 2043 6c69 7020 7468 656d       # Clip them
-0001b7a0: 2061 7420 7365 6e73 6962 6c65 2076 616c   at sensible val
-0001b7b0: 7565 730a 2020 2020 2020 2020 5b79 5f6c  ues.        [y_l
-0001b7c0: 6f77 6572 2c20 795f 7570 7065 725d 203d  ower, y_upper] =
-0001b7d0: 206e 702e 636c 6970 285b 795f 6c6f 7765   np.clip([y_lowe
-0001b7e0: 722c 2079 5f75 7070 6572 5d2c 2031 452d  r, y_upper], 1E-
-0001b7f0: 3130 2c20 3145 3130 290a 0a20 2020 2020  10, 1E10)..     
-0001b800: 2020 2023 2061 6e64 2073 6574 2076 616c     # and set val
-0001b810: 7565 730a 2020 2020 2020 2020 7365 6c66  ues.        self
-0001b820: 2e70 6c6f 745f 7769 6467 6574 2e73 6574  .plot_widget.set
-0001b830: 5952 616e 6765 280a 2020 2020 2020 2020  YRange(.        
-0001b840: 2020 2020 6e70 2e6c 6f67 3130 2879 5f6c      np.log10(y_l
-0001b850: 6f77 6572 292c 0a20 2020 2020 2020 2020  ower),.         
-0001b860: 2020 206e 702e 6c6f 6731 3028 795f 7570     np.log10(y_up
-0001b870: 7065 7229 2c0a 2020 2020 2020 2020 2020  per),.          
-0001b880: 2020 7061 6464 696e 673d 300a 2020 2020    padding=0.    
-0001b890: 2020 2020 290a 0a20 2020 2020 2020 2023      )..        #
-0001b8a0: 2041 6464 2065 7870 6572 696d 656e 7461   Add experimenta
-0001b8b0: 6c20 6572 726f 7262 6172 730a 2020 2020  l errorbars.    
-0001b8c0: 2020 2020 6966 206c 656e 2864 6174 6173      if len(datas
-0001b8d0: 6574 2e6c 6f67 7261 7465 5f70 6d29 3a0a  et.lograte_pm):.
-0001b8e0: 2020 2020 2020 2020 2020 2020 6572 7220              err 
-0001b8f0: 3d20 7067 2e45 7272 6f72 4261 7249 7465  = pg.ErrorBarIte
-0001b900: 6d28 0a20 2020 2020 2020 2020 2020 2020  m(.             
-0001b910: 2020 2078 3d6e 702e 6c6f 6731 3028 785f     x=np.log10(x_
-0001b920: 7661 6c73 292c 0a20 2020 2020 2020 2020  vals),.         
-0001b930: 2020 2020 2020 2079 3d6e 702e 6c6f 6731         y=np.log1
-0001b940: 3028 6461 7461 7365 742e 7261 7465 7329  0(dataset.rates)
-0001b950: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001b960: 2020 746f 703d 6461 7461 7365 742e 6c6f    top=dataset.lo
-0001b970: 6772 6174 655f 706d 2c0a 2020 2020 2020  grate_pm,.      
-0001b980: 2020 2020 2020 2020 2020 626f 7474 6f6d            bottom
-0001b990: 3d64 6174 6173 6574 2e6c 6f67 7261 7465  =dataset.lograte
-0001b9a0: 5f70 6d2c 0a20 2020 2020 2020 2020 2020  _pm,.           
-0001b9b0: 2020 2020 2062 6561 6d3d 302e 3030 350a       beam=0.005.
-0001b9c0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0001b9d0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-0001b9e0: 6c6f 745f 7769 6467 6574 2e61 6464 4974  lot_widget.addIt
-0001b9f0: 656d 2865 7272 290a 0a20 2020 2020 2020  em(err)..       
-0001ba00: 2023 2041 7869 7320 6c61 6265 6c73 0a20   # Axis labels. 
-0001ba10: 2020 2020 2020 2073 656c 662e 706c 6f74         self.plot
-0001ba20: 5f77 6964 6765 742e 7365 744c 6162 656c  _widget.setLabel
-0001ba30: 2827 6c65 6674 272c 2027 5261 7465 2028  ('left', 'Rate (
-0001ba40: 733c 7375 703e 2d31 3c2f 7375 703e 2927  s<sup>-1</sup>)'
-0001ba50: 290a 0a20 2020 2020 2020 2023 2053 6574  )..        # Set
-0001ba60: 2064 6963 7469 6f6e 6172 7920 6f66 2054   dictionary of T
-0001ba70: 7275 6520 2866 6974 2920 616e 6420 4661  rue (fit) and Fa
-0001ba80: 6c73 6520 2866 6978 2920 666f 7220 6561  lse (fix) for ea
-0001ba90: 6368 0a20 2020 2020 2020 2023 2070 6172  ch.        # par
-0001baa0: 616d 6574 6572 206f 6620 616c 6c20 6176  ameter of all av
-0001bab0: 6169 6c61 626c 6520 6d6f 6465 6c73 0a20  ailable models. 
-0001bac0: 2020 2020 2020 2075 7365 6c2e 6669 7420         usel.fit 
-0001bad0: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
-0001bae0: 7061 726e 616d 653a 2054 7275 650a 2020  parname: True.  
-0001baf0: 2020 2020 2020 2020 2020 666f 7220 6d6f            for mo
-0001bb00: 6465 6c20 696e 2073 7570 706f 7274 6564  del in supported
-0001bb10: 5f6d 6f64 656c 730a 2020 2020 2020 2020  _models.        
-0001bb20: 2020 2020 666f 7220 7061 726e 616d 6520      for parname 
-0001bb30: 696e 206d 6f64 656c 2e50 4152 4e41 4d45  in model.PARNAME
-0001bb40: 530a 2020 2020 2020 2020 7d0a 0a20 2020  S.        }..   
-0001bb50: 2020 2020 2023 2053 6574 2075 7365 7220       # Set user 
-0001bb60: 7365 6c65 6374 696f 6e20 6f62 6a65 6374  selection object
-0001bb70: 2061 6e64 2073 7570 706f 7274 6564 206d   and supported m
-0001bb80: 6f64 656c 730a 2020 2020 2020 2020 7365  odels.        se
-0001bb90: 6c66 2e75 7365 6c20 3d20 7573 656c 0a20  lf.usel = usel. 
-0001bba0: 2020 2020 2020 2073 656c 662e 7375 7070         self.supp
-0001bbb0: 6f72 7465 645f 6d6f 6465 6c73 203d 2073  orted_models = s
-0001bbc0: 7570 706f 7274 6564 5f6d 6f64 656c 730a  upported_models.
-0001bbd0: 0a20 2020 2020 2020 2023 2043 616c 6375  .        # Calcu
-0001bbe0: 6c61 7465 2065 6163 6820 6d6f 6465 6c20  late each model 
-0001bbf0: 6675 6e63 7469 6f6e 2061 6e64 2070 6c6f  function and plo
-0001bc00: 740a 2020 2020 2020 2020 2320 4e6f 7465  t.        # Note
-0001bc10: 2069 6620 7368 6966 7420 6973 2061 7070   if shift is app
-0001bc20: 6c69 6564 2074 6865 6e20 7468 6573 6520  lied then these 
-0001bc30: 7661 6c75 6573 0a20 2020 2020 2020 2023  values.        #
-0001bc40: 206d 7573 7420 6265 2074 6865 2074 7275   must be the tru
-0001bc50: 6520 7820 7661 7269 6162 6c65 7320 6173  e x variables as
-0001bc60: 2074 6865 7920 7769 6c6c 2062 6520 7573   they will be us
-0001bc70: 6564 2074 6f20 636f 6d70 7574 650a 2020  ed to compute.  
-0001bc80: 2020 2020 2020 2320 7468 6520 6d6f 6465        # the mode
-0001bc90: 6c20 7661 6c75 6573 0a20 2020 2020 2020  l values.       
-0001bca0: 2073 656c 662e 785f 6772 6964 203d 206e   self.x_grid = n
-0001bcb0: 702e 6c69 6e73 7061 6365 280a 2020 2020  p.linspace(.    
-0001bcc0: 2020 2020 2020 2020 6e70 2e6d 696e 2878          np.min(x
-0001bcd0: 5f76 616c 7320 2d20 7365 6c66 2e6c 6f67  _vals - self.log
-0001bce0: 7368 6966 7429 2c0a 2020 2020 2020 2020  shift),.        
-0001bcf0: 2020 2020 6e70 2e6d 6178 2878 5f76 616c      np.max(x_val
-0001bd00: 7320 2d20 7365 6c66 2e6c 6f67 7368 6966  s - self.logshif
-0001bd10: 7429 2c0a 2020 2020 2020 2020 2020 2020  t),.            
-0001bd20: 3130 3030 0a20 2020 2020 2020 2029 0a0a  1000.        )..
-0001bd30: 2020 2020 2020 2020 2320 5375 6d20 6f66          # Sum of
-0001bd40: 2061 6c6c 206d 6f64 656c 732c 2073 6574   all models, set
-0001bd50: 2074 6f20 7a65 726f 2069 6e69 7469 616c   to zero initial
-0001bd60: 6c79 0a20 2020 2020 2020 2074 6f74 616c  ly.        total
-0001bd70: 5f72 6174 6573 203d 206e 702e 7a65 726f  _rates = np.zero
-0001bd80: 7328 6e70 2e73 6861 7065 2873 656c 662e  s(np.shape(self.
-0001bd90: 785f 6772 6964 2929 0a0a 2020 2020 2020  x_grid))..      
-0001bda0: 2020 2320 4469 6374 696f 6e61 7279 206f    # Dictionary o
-0001bdb0: 6620 706c 6f74 730a 2020 2020 2020 2020  f plots.        
-0001bdc0: 2320 6b65 7973 2061 7265 206d 6f64 656c  # keys are model
-0001bdd0: 2e4e 414d 452e 6c6f 7765 7228 292c 2076  .NAME.lower(), v
-0001bde0: 616c 7565 7320 6172 6520 706c 6f74 5f77  alues are plot_w
-0001bdf0: 6964 6765 742e 706c 6f74 0a20 2020 2020  idget.plot.     
-0001be00: 2020 2073 656c 662e 6d6f 6465 6c5f 706c     self.model_pl
-0001be10: 6f74 7320 3d20 7b7d 0a0a 2020 2020 2020  ots = {}..      
-0001be20: 2020 2320 4c69 7374 206f 6620 6e69 6365    # List of nice
-0001be30: 2063 6f6c 6f72 730a 2020 2020 2020 2020   colors.        
-0001be40: 636f 6c6f 7273 203d 206d 636f 6c6f 7273  colors = mcolors
-0001be50: 2e54 4142 4c45 4155 5f43 4f4c 4f52 532e  .TABLEAU_COLORS.
-0001be60: 7661 6c75 6573 2829 0a0a 2020 2020 2020  values()..      
-0001be70: 2020 2320 4c6f 6f70 206f 7665 7220 616c    # Loop over al
-0001be80: 6c20 706f 7373 6962 6c65 206d 6f64 656c  l possible model
-0001be90: 732c 2063 616c 6375 6c61 7465 206d 6f64  s, calculate mod
-0001bea0: 656c 2076 616c 7565 730a 2020 2020 2020  el values.      
-0001beb0: 2020 2320 6174 2072 616e 6765 206f 6620    # at range of 
-0001bec0: 7465 6d70 6572 6174 7572 6573 2061 6e64  temperatures and
-0001bed0: 2070 6c6f 740a 2020 2020 2020 2020 2320   plot.        # 
-0001bee0: 7468 656e 2061 6464 2074 6f20 6172 7261  then add to arra
-0001bef0: 7920 6f66 2074 6f74 616c 2072 6174 6573  y of total rates
-0001bf00: 0a20 2020 2020 2020 2066 6f72 2063 6f6c  .        for col
-0001bf10: 6f72 2c20 6d6f 6465 6c20 696e 207a 6970  or, model in zip
-0001bf20: 2863 6f6c 6f72 732c 2073 7570 706f 7274  (colors, support
-0001bf30: 6564 5f6d 6f64 656c 7329 3a0a 0a20 2020  ed_models):..   
-0001bf40: 2020 2020 2020 2020 2023 2047 6574 2069           # Get i
-0001bf50: 6e69 7469 616c 2076 616c 7565 730a 2020  nitial values.  
-0001bf60: 2020 2020 2020 2020 2020 696e 6974 6961            initia
-0001bf70: 6c73 203d 206d 6f64 656c 2e73 6574 5f69  ls = model.set_i
-0001bf80: 6e69 7469 616c 5f76 616c 7328 0a20 2020  nitial_vals(.   
-0001bf90: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
-0001bfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bfb0: 2020 2070 6172 3a20 7365 6c66 2e64 6566     par: self.def
-0001bfc0: 6175 6c74 735b 6d6f 6465 6c2e 4e41 4d45  aults[model.NAME
-0001bfd0: 5d5b 7061 725d 5b27 7661 6c69 6e69 7427  ][par]['valinit'
-0001bfe0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0001bff0: 2020 2020 2020 666f 7220 7061 7220 696e        for par in
-0001c000: 206d 6f64 656c 2e50 4152 4e41 4d45 530a   model.PARNAMES.
-0001c010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c020: 7d0a 2020 2020 2020 2020 2020 2020 290a  }.            ).
-0001c030: 2020 2020 2020 2020 2020 2020 2320 4361              # Ca
-0001c040: 6c63 756c 6174 6520 7261 7465 730a 2020  lculate rates.  
-0001c050: 2020 2020 2020 2020 2020 7261 7465 7320            rates 
-0001c060: 3d20 3130 2a2a 286d 6f64 656c 2e6d 6f64  = 10**(model.mod
-0001c070: 656c 2869 6e69 7469 616c 732c 2073 656c  el(initials, sel
-0001c080: 662e 785f 6772 6964 2929 0a20 2020 2020  f.x_grid)).     
-0001c090: 2020 2020 2020 2023 2061 6e64 2061 6464         # and add
-0001c0a0: 2074 6f20 746f 7461 6c20 6f66 2061 6c6c   to total of all
-0001c0b0: 206d 6f64 656c 730a 2020 2020 2020 2020   models.        
-0001c0c0: 2020 2020 746f 7461 6c5f 7261 7465 7320      total_rates 
-0001c0d0: 2b3d 2072 6174 6573 0a20 2020 2020 2020  += rates.       
-0001c0e0: 2020 2020 2023 2050 6c6f 7420 7468 6973       # Plot this
-0001c0f0: 206d 6f64 656c 0a20 2020 2020 2020 2020   model.         
-0001c100: 2020 205f 706c 6f74 203d 2073 656c 662e     _plot = self.
-0001c110: 706c 6f74 5f77 6964 6765 742e 706c 6f74  plot_widget.plot
-0001c120: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0001c130: 2020 7365 6c66 2e78 5f67 7269 6420 2b20    self.x_grid + 
-0001c140: 7365 6c66 2e6c 6f67 7368 6966 742c 0a20  self.logshift,. 
-0001c150: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0001c160: 6174 6573 2c0a 2020 2020 2020 2020 2020  ates,.          
-0001c170: 2020 2020 2020 7065 6e3d 7b27 7769 6474        pen={'widt
-0001c180: 6827 3a20 322e 352c 2027 636f 6c6f 7227  h': 2.5, 'color'
-0001c190: 3a20 636f 6c6f 722c 2027 7374 796c 6527  : color, 'style'
-0001c1a0: 3a20 5174 436f 7265 2e51 742e 4461 7368  : QtCore.Qt.Dash
-0001c1b0: 4c69 6e65 7d0a 2020 2020 2020 2020 2020  Line}.          
-0001c1c0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0001c1d0: 2320 616e 6420 7374 6f72 6520 696e 2064  # and store in d
-0001c1e0: 6963 7420 6f66 2061 6c6c 2070 6c6f 7473  ict of all plots
-0001c1f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0001c200: 662e 6d6f 6465 6c5f 706c 6f74 735b 6d6f  f.model_plots[mo
-0001c210: 6465 6c2e 4e41 4d45 2e6c 6f77 6572 2829  del.NAME.lower()
-0001c220: 5d20 3d20 5f70 6c6f 740a 2020 2020 2020  ] = _plot.      
-0001c230: 2020 2020 2020 2320 5265 6d6f 7665 2066        # Remove f
-0001c240: 726f 6d20 6163 7475 616c 2070 6c6f 7420  rom actual plot 
-0001c250: 7769 6467 6574 0a20 2020 2020 2020 2020  widget.         
-0001c260: 2020 2023 2073 696e 6365 206e 6f20 6d6f     # since no mo
-0001c270: 6465 6c73 2061 7265 2076 6973 6962 6c65  dels are visible
-0001c280: 2069 6e69 7469 616c 6c79 0a20 2020 2020   initially.     
-0001c290: 2020 2020 2020 2023 2050 6c6f 7473 2061         # Plots a
-0001c2a0: 7265 2072 652d 6164 6465 6420 7769 7468  re re-added with
-0001c2b0: 206d 6f64 656c 2063 6865 636b 626f 7865   model checkboxe
-0001c2c0: 730a 2020 2020 2020 2020 2020 2020 7365  s.            se
-0001c2d0: 6c66 2e70 6c6f 745f 7769 6467 6574 2e72  lf.plot_widget.r
-0001c2e0: 656d 6f76 6549 7465 6d28 5f70 6c6f 7429  emoveItem(_plot)
-0001c2f0: 0a0a 2020 2020 2020 2020 2320 506c 6f74  ..        # Plot
-0001c300: 2073 756d 206f 6620 616c 6c20 6d6f 6465   sum of all mode
-0001c310: 6c73 0a20 2020 2020 2020 2073 656c 662e  ls.        self.
-0001c320: 746f 7420 3d20 7365 6c66 2e70 6c6f 745f  tot = self.plot_
-0001c330: 7769 6467 6574 2e70 6c6f 7428 0a20 2020  widget.plot(.   
-0001c340: 2020 2020 2020 2020 2073 656c 662e 785f           self.x_
-0001c350: 6772 6964 202b 2073 656c 662e 6c6f 6773  grid + self.logs
-0001c360: 6869 6674 2c0a 2020 2020 2020 2020 2020  hift,.          
-0001c370: 2020 746f 7461 6c5f 7261 7465 732c 0a20    total_rates,. 
-0001c380: 2020 2020 2020 2020 2020 2070 656e 3d7b             pen={
-0001c390: 2777 6964 7468 273a 2032 2e35 2c20 2763  'width': 2.5, 'c
-0001c3a0: 6f6c 6f72 273a 2027 7265 6427 7d0a 2020  olor': 'red'}.  
-0001c3b0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0001c3c0: 7365 6c66 2e70 6c6f 745f 7769 6467 6574  self.plot_widget
-0001c3d0: 2e72 656d 6f76 6549 7465 6d28 7365 6c66  .removeItem(self
-0001c3e0: 2e74 6f74 290a 0a20 2020 2020 2020 2023  .tot)..        #
-0001c3f0: 2053 746f 7261 6765 206f 626a 6563 7420   Storage object 
-0001c400: 666f 7220 6669 6e61 6c20 7061 7261 6d65  for final parame
-0001c410: 7465 7220 7661 6c75 6573 0a20 2020 2020  ter values.     
-0001c420: 2020 2023 2053 6574 2061 6c6c 2069 6e69     # Set all ini
-0001c430: 7469 616c 2076 616c 7565 7320 6465 6661  tial values defa
-0001c440: 756c 7473 0a20 2020 2020 2020 2073 656c  ults.        sel
-0001c450: 662e 7061 7273 746f 7265 203d 2074 7970  f.parstore = typ
-0001c460: 6528 0a20 2020 2020 2020 2020 2020 2027  e(.            '
-0001c470: 6f62 6a27 2c0a 2020 2020 2020 2020 2020  obj',.          
-0001c480: 2020 286f 626a 6563 742c 292c 0a20 2020    (object,),.   
-0001c490: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
-0001c4a0: 2020 2020 2020 2020 2020 2070 6172 3a20             par: 
-0001c4b0: 7365 6c66 2e64 6566 6175 6c74 735b 6d6f  self.defaults[mo
-0001c4c0: 6465 6c2e 4e41 4d45 5d5b 7061 725d 5b27  del.NAME][par]['
-0001c4d0: 7661 6c69 6e69 7427 5d0a 2020 2020 2020  valinit'].      
-0001c4e0: 2020 2020 2020 2020 2020 666f 7220 6d6f            for mo
-0001c4f0: 6465 6c20 696e 2073 7570 706f 7274 6564  del in supported
-0001c500: 5f6d 6f64 656c 730a 2020 2020 2020 2020  _models.        
-0001c510: 2020 2020 2020 2020 666f 7220 7061 7220          for par 
-0001c520: 696e 206d 6f64 656c 2e50 4152 4e41 4d45  in model.PARNAME
-0001c530: 530a 2020 2020 2020 2020 2020 2020 7d0a  S.            }.
-0001c540: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-0001c550: 2020 2023 2043 6f6e 7665 7274 206c 6f67     # Convert log
-0001c560: 2074 656d 7065 7261 7475 7265 2074 6963   temperature tic
-0001c570: 6b73 2074 6f20 6c69 6e65 6172 0a20 2020  ks to linear.   
-0001c580: 2020 2020 2061 7820 3d20 7365 6c66 2e70       ax = self.p
-0001c590: 6c6f 745f 7769 6467 6574 2e67 6574 4178  lot_widget.getAx
-0001c5a0: 6973 2827 626f 7474 6f6d 2729 0a20 2020  is('bottom').   
-0001c5b0: 2020 2020 2067 7569 2e63 6f6e 7665 7274       gui.convert
-0001c5c0: 5f6c 6f67 5f74 6963 6b73 5f74 6f5f 6c69  _log_ticks_to_li
-0001c5d0: 6e28 6178 2c20 6e70 2e6c 6f67 3130 2878  n(ax, np.log10(x
-0001c5e0: 5f76 616c 7329 2c20 7368 6966 743d 7365  _vals), shift=se
-0001c5f0: 6c66 2e6c 6f67 7368 6966 7429 0a0a 2020  lf.logshift)..  
-0001c600: 2020 2020 2020 2320 5248 5320 636f 6c75        # RHS colu
-0001c610: 6d6e 206f 6620 7769 6e64 6f77 0a20 2020  mn of window.   
-0001c620: 2020 2020 2023 2054 6869 7320 636f 6e74       # This cont
-0001c630: 6169 6e73 2065 6163 6820 6d6f 6465 6c20  ains each model 
-0001c640: 616e 6420 6974 7320 6173 736f 6369 6174  and its associat
-0001c650: 6564 2070 6172 616d 6574 6572 730a 2020  ed parameters.  
-0001c660: 2020 2020 2020 2320 4561 6368 2070 6172        # Each par
-0001c670: 616d 6574 6572 2069 7320 636f 6e74 726f  ameter is contro
-0001c680: 6c6c 6564 2062 7920 610a 2020 2020 2020  lled by a.      
-0001c690: 2020 2320 736c 6964 6572 732c 2054 6578    # sliders, Tex
-0001c6a0: 7420 656e 7472 792c 2061 6e64 2061 2066  t entry, and a f
-0001c6b0: 6974 2f66 6978 2074 6f67 676c 650a 2020  it/fix toggle.  
-0001c6c0: 2020 2020 2020 636f 6e74 6169 6e65 725f        container_
-0001c6d0: 6c61 796f 7574 203d 2051 7457 6964 6765  layout = QtWidge
-0001c6e0: 7473 2e51 5642 6f78 4c61 796f 7574 2873  ts.QVBoxLayout(s
-0001c6f0: 6372 6f6c 6c5f 636f 6e74 6169 6e65 7229  croll_container)
-0001c700: 0a0a 2020 2020 2020 2020 2320 4c69 7374  ..        # List
-0001c710: 206f 6620 6e75 6d62 6572 206b 6579 2073   of number key s
-0001c720: 686f 7274 6375 7473 2074 6f20 746f 6767  hortcuts to togg
-0001c730: 6c65 206d 6f64 656c 730a 2020 2020 2020  le models.      
-0001c740: 2020 7365 6c66 2e6f 6e5f 6f66 665f 7368    self.on_off_sh
-0001c750: 6f72 7463 7574 203d 205b 5d0a 0a20 2020  ortcut = []..   
-0001c760: 2020 2020 2023 2046 6f72 2065 6163 6820       # For each 
-0001c770: 6d6f 6465 6c2c 206d 616b 6520 6120 626f  model, make a bo
-0001c780: 7820 746f 2063 6f6e 7461 696e 2061 6c6c  x to contain all
-0001c790: 2070 6172 616d 6574 6572 730a 2020 2020   parameters.    
-0001c7a0: 2020 2020 2320 616e 6420 706f 7075 6c61      # and popula
-0001c7b0: 7465 2077 6974 6820 7061 7261 6d65 7465  te with paramete
-0001c7c0: 7273 0a20 2020 2020 2020 2066 6f72 206d  rs.        for m
-0001c7d0: 6974 2c20 6d6f 6465 6c20 696e 2065 6e75  it, model in enu
-0001c7e0: 6d65 7261 7465 2873 7570 706f 7274 6564  merate(supported
-0001c7f0: 5f6d 6f64 656c 7329 3a0a 2020 2020 2020  _models):.      
-0001c800: 2020 2020 2020 6d6f 6465 6c5f 7769 6467        model_widg
-0001c810: 6574 203d 2073 656c 662e 6d61 6b65 5f6d  et = self.make_m
-0001c820: 6f64 656c 626f 7828 6d6f 6465 6c2c 2073  odelbox(model, s
-0001c830: 6372 6f6c 6c5f 636f 6e74 6169 6e65 722c  croll_container,
-0001c840: 206d 6974 202b 2031 290a 0a20 2020 2020   mit + 1)..     
-0001c850: 2020 2020 2020 2023 2041 6464 2074 6869         # Add thi
-0001c860: 7320 6d6f 6465 6c20 746f 2074 6865 2072  s model to the r
-0001c870: 6967 6874 2068 616e 6420 7369 6465 206f  ight hand side o
-0001c880: 6620 7468 6520 7769 6e64 6f77 0a20 2020  f the window.   
-0001c890: 2020 2020 2020 2020 2063 6f6e 7461 696e           contain
-0001c8a0: 6572 5f6c 6179 6f75 742e 6164 6457 6964  er_layout.addWid
-0001c8b0: 6765 7428 6d6f 6465 6c5f 7769 6467 6574  get(model_widget
-0001c8c0: 2c20 6c65 6e28 6d6f 6465 6c2e 5041 524e  , len(model.PARN
-0001c8d0: 414d 4553 2929 0a0a 2020 2020 2020 2020  AMES))..        
-0001c8e0: 2320 4469 7361 626c 6520 6576 6572 7920  # Disable every 
-0001c8f0: 736c 6964 6572 2c20 656e 7472 792c 2061  slider, entry, a
-0001c900: 6e64 2066 6974 2f66 6978 2062 7920 6465  nd fit/fix by de
-0001c910: 6661 756c 740a 2020 2020 2020 2020 2320  fault.        # 
-0001c920: 5468 6973 2069 7320 746f 6767 6c65 6420  This is toggled 
-0001c930: 6279 2074 6865 206d 6f64 656c 2063 6865  by the model che
-0001c940: 636b 626f 7865 730a 2020 2020 2020 2020  ckboxes.        
-0001c950: 666f 7220 6d6f 6465 6c20 696e 2073 7570  for model in sup
-0001c960: 706f 7274 6564 5f6d 6f64 656c 733a 0a20  ported_models:. 
-0001c970: 2020 2020 2020 2020 2020 206d 6f64 656c             model
-0001c980: 6e61 6d65 203d 206d 6f64 656c 2e4e 414d  name = model.NAM
-0001c990: 452e 6c6f 7765 7228 290a 2020 2020 2020  E.lower().      
-0001c9a0: 2020 2020 2020 666f 7220 7061 726e 616d        for parnam
-0001c9b0: 6520 696e 206d 6f64 656c 2e50 4152 4e41  e in model.PARNA
-0001c9c0: 4d45 533a 0a20 2020 2020 2020 2020 2020  MES:.           
-0001c9d0: 2020 2020 2073 656c 662e 7769 6467 6574       self.widget
-0001c9e0: 6469 6374 5b6d 6f64 656c 6e61 6d65 5d5b  dict[modelname][
-0001c9f0: 7061 726e 616d 655d 5b27 736c 6964 6572  parname]['slider
-0001ca00: 275d 2e73 6574 456e 6162 6c65 6428 4661  '].setEnabled(Fa
-0001ca10: 6c73 6529 0a20 2020 2020 2020 2020 2020  lse).           
-0001ca20: 2020 2020 2073 656c 662e 7769 6467 6574       self.widget
-0001ca30: 6469 6374 5b6d 6f64 656c 6e61 6d65 5d5b  dict[modelname][
-0001ca40: 7061 726e 616d 655d 5b27 656e 7472 7927  parname]['entry'
-0001ca50: 5d2e 7365 7445 6e61 626c 6564 2846 616c  ].setEnabled(Fal
-0001ca60: 7365 290a 2020 2020 2020 2020 2020 2020  se).            
-0001ca70: 2020 2020 7365 6c66 2e77 6964 6765 7464      self.widgetd
-0001ca80: 6963 745b 6d6f 6465 6c6e 616d 655d 5b70  ict[modelname][p
-0001ca90: 6172 6e61 6d65 5d5b 2766 665f 746f 6767  arname]['ff_togg
-0001caa0: 6c65 275d 2e73 6574 456e 6162 6c65 6428  le'].setEnabled(
-0001cab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001cac0: 2020 2020 2046 616c 7365 0a20 2020 2020       False.     
-0001cad0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-0001cae0: 2020 2020 2020 636f 6e74 6169 6e65 725f        container_
-0001caf0: 6c61 796f 7574 2e73 6574 416c 6967 6e6d  layout.setAlignm
-0001cb00: 656e 7428 5174 436f 7265 2e51 742e 416c  ent(QtCore.Qt.Al
-0001cb10: 6967 6e56 4365 6e74 6572 290a 2020 2020  ignVCenter).    
-0001cb20: 2020 2020 7363 726f 6c6c 5f63 6f6e 7461      scroll_conta
-0001cb30: 696e 6572 2e73 6574 5369 7a65 506f 6c69  iner.setSizePoli
-0001cb40: 6379 280a 2020 2020 2020 2020 2020 2020  cy(.            
-0001cb50: 5174 5769 6467 6574 732e 5153 697a 6550  QtWidgets.QSizeP
-0001cb60: 6f6c 6963 792e 4d61 7869 6d75 6d2c 0a20  olicy.Maximum,. 
-0001cb70: 2020 2020 2020 2020 2020 2051 7457 6964             QtWid
-0001cb80: 6765 7473 2e51 5369 7a65 506f 6c69 6379  gets.QSizePolicy
-0001cb90: 2e4d 6178 696d 756d 0a20 2020 2020 2020  .Maximum.       
-0001cba0: 2029 0a20 2020 2020 2020 2072 6873 5f63   ).        rhs_c
-0001cbb0: 6f6c 5f73 6372 6f6c 6c2e 7365 744d 696e  ol_scroll.setMin
-0001cbc0: 696d 756d 4865 6967 6874 2835 3735 290a  imumHeight(575).
-0001cbd0: 0a20 2020 2020 2020 2023 2054 6f70 2072  .        # Top r
-0001cbe0: 6f77 0a20 2020 2020 2020 2023 204c 4853  ow.        # LHS
-0001cbf0: 2070 6c6f 742c 2052 4853 2053 6c69 6465   plot, RHS Slide
-0001cc00: 7273 2c20 7465 7874 2c20 6c61 6265 6c73  rs, text, labels
-0001cc10: 0a20 2020 2020 2020 2074 6f70 5f72 6f77  .        top_row
-0001cc20: 5f6c 6179 6f75 7420 3d20 5174 5769 6467  _layout = QtWidg
-0001cc30: 6574 732e 5148 426f 784c 6179 6f75 7428  ets.QHBoxLayout(
-0001cc40: 746f 705f 726f 775f 7769 6467 6574 290a  top_row_widget).
-0001cc50: 2020 2020 2020 2020 746f 705f 726f 775f          top_row_
-0001cc60: 6c61 796f 7574 2e61 6464 5769 6467 6574  layout.addWidget
-0001cc70: 286c 6873 5f63 6f6c 5f77 6964 6765 742c  (lhs_col_widget,
-0001cc80: 2033 290a 2020 2020 2020 2020 746f 705f   3).        top_
-0001cc90: 726f 775f 6c61 796f 7574 2e61 6464 5769  row_layout.addWi
-0001cca0: 6467 6574 2872 6873 5f63 6f6c 5f77 6964  dget(rhs_col_wid
-0001ccb0: 6765 742c 2032 290a 0a20 2020 2020 2020  get, 2)..       
-0001ccc0: 2023 2042 6f74 746f 6d20 726f 770a 2020   # Bottom row.  
-0001ccd0: 2020 2020 2020 2320 4275 7474 6f6e 7320        # Buttons 
-0001cce0: 666f 7220 7265 7365 7420 616e 6420 6669  for reset and fi
-0001ccf0: 740a 2020 2020 2020 2020 7365 6c66 2e66  t.        self.f
-0001cd00: 6974 5f62 746e 5f77 6964 6765 7420 3d20  it_btn_widget = 
-0001cd10: 5174 5769 6467 6574 732e 5150 7573 6842  QtWidgets.QPushB
-0001cd20: 7574 746f 6e28 0a20 2020 2020 2020 2020  utton(.         
-0001cd30: 2020 2070 6172 656e 743d 626f 745f 726f     parent=bot_ro
-0001cd40: 775f 7769 6467 6574 2c0a 2020 2020 2020  w_widget,.      
-0001cd50: 2020 2020 2020 7465 7874 3d27 4669 7427        text='Fit'
-0001cd60: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-0001cd70: 2020 2073 656c 662e 6669 745f 6274 6e5f     self.fit_btn_
-0001cd80: 7769 6467 6574 2e73 6574 5374 796c 6553  widget.setStyleS
-0001cd90: 6865 6574 2827 666f 6e74 2d77 6569 6768  heet('font-weigh
-0001cda0: 743a 2062 6f6c 643b 2729 0a0a 2020 2020  t: bold;')..    
-0001cdb0: 2020 2020 7365 6c66 2e66 6974 5f62 746e      self.fit_btn
-0001cdc0: 5f77 6964 6765 742e 7365 7445 6e61 626c  _widget.setEnabl
-0001cdd0: 6564 2846 616c 7365 290a 2020 2020 2020  ed(False).      
-0001cde0: 2020 7365 6c66 2e66 6974 5f62 746e 5f77    self.fit_btn_w
-0001cdf0: 6964 6765 742e 636c 6963 6b65 642e 636f  idget.clicked.co
-0001ce00: 6e6e 6563 7428 7365 6c66 2e66 6974 290a  nnect(self.fit).
-0001ce10: 2020 2020 2020 2020 7365 6c66 2e66 6974          self.fit
-0001ce20: 5f62 746e 5f77 6964 6765 742e 7365 7453  _btn_widget.setS
-0001ce30: 697a 6550 6f6c 6963 7928 0a20 2020 2020  izePolicy(.     
-0001ce40: 2020 2020 2020 2051 7457 6964 6765 7473         QtWidgets
-0001ce50: 2e51 5369 7a65 506f 6c69 6379 2e46 6978  .QSizePolicy.Fix
-0001ce60: 6564 2c0a 2020 2020 2020 2020 2020 2020  ed,.            
-0001ce70: 5174 5769 6467 6574 732e 5153 697a 6550  QtWidgets.QSizeP
-0001ce80: 6f6c 6963 792e 4669 7865 640a 2020 2020  olicy.Fixed.    
-0001ce90: 2020 2020 290a 2020 2020 2020 2020 7265      ).        re
-0001cea0: 7365 745f 6274 6e5f 7769 6467 6574 203d  set_btn_widget =
-0001ceb0: 2051 7457 6964 6765 7473 2e51 5075 7368   QtWidgets.QPush
-0001cec0: 4275 7474 6f6e 280a 2020 2020 2020 2020  Button(.        
-0001ced0: 2020 2020 7061 7265 6e74 3d62 6f74 5f72      parent=bot_r
-0001cee0: 6f77 5f77 6964 6765 742c 0a20 2020 2020  ow_widget,.     
-0001cef0: 2020 2020 2020 2074 6578 743d 2752 6573         text='Res
-0001cf00: 6574 272c 0a20 2020 2020 2020 2029 0a20  et',.        ). 
-0001cf10: 2020 2020 2020 2072 6573 6574 5f62 746e         reset_btn
-0001cf20: 5f77 6964 6765 742e 7365 7453 7479 6c65  _widget.setStyle
-0001cf30: 5368 6565 7428 2766 6f6e 742d 7765 6967  Sheet('font-weig
-0001cf40: 6874 3a20 626f 6c64 3b27 290a 2020 2020  ht: bold;').    
-0001cf50: 2020 2020 7265 7365 745f 6274 6e5f 7769      reset_btn_wi
-0001cf60: 6467 6574 2e63 6c69 636b 6564 2e63 6f6e  dget.clicked.con
-0001cf70: 6e65 6374 2873 656c 662e 7265 7365 7429  nect(self.reset)
-0001cf80: 0a20 2020 2020 2020 2072 6573 6574 5f62  .        reset_b
-0001cf90: 746e 5f77 6964 6765 742e 7365 7453 697a  tn_widget.setSiz
-0001cfa0: 6550 6f6c 6963 7928 0a20 2020 2020 2020  ePolicy(.       
-0001cfb0: 2020 2020 2051 7457 6964 6765 7473 2e51       QtWidgets.Q
-0001cfc0: 5369 7a65 506f 6c69 6379 2e46 6978 6564  SizePolicy.Fixed
-0001cfd0: 2c0a 2020 2020 2020 2020 2020 2020 5174  ,.            Qt
-0001cfe0: 5769 6467 6574 732e 5153 697a 6550 6f6c  Widgets.QSizePol
-0001cff0: 6963 792e 4669 7865 640a 2020 2020 2020  icy.Fixed.      
-0001d000: 2020 290a 0a20 2020 2020 2020 2023 204d    )..        # M
-0001d010: 6f64 6966 7920 6669 7420 616e 6420 7265  odify fit and re
-0001d020: 7365 7420 6275 7474 6f6e 2074 6578 7420  set button text 
-0001d030: 636f 6c6f 7273 2074 6f20 6c6f 6f6b 2067  colors to look g
-0001d040: 6f6f 6420 6576 656e 0a20 2020 2020 2020  ood even.       
-0001d050: 2023 2069 6e20 4d61 634f 5320 6461 726b   # in MacOS dark
-0001d060: 6d6f 6465 2e0a 2020 2020 2020 2020 7061  mode..        pa
-0001d070: 6c65 7474 6520 3d20 5174 4775 692e 5150  lette = QtGui.QP
-0001d080: 616c 6574 7465 2873 656c 662e 6669 745f  alette(self.fit_
-0001d090: 6274 6e5f 7769 6467 6574 2e70 616c 6574  btn_widget.palet
-0001d0a0: 7465 2829 290a 2020 2020 2020 2020 7061  te()).        pa
-0001d0b0: 6c65 7474 652e 7365 7443 6f6c 6f72 2851  lette.setColor(Q
-0001d0c0: 7447 7569 2e51 5061 6c65 7474 652e 4275  tGui.QPalette.Bu
-0001d0d0: 7474 6f6e 5465 7874 2c20 5174 4775 692e  ttonText, QtGui.
-0001d0e0: 5143 6f6c 6f72 2827 2330 6462 3237 3327  QColor('#0db273'
-0001d0f0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-0001d100: 6669 745f 6274 6e5f 7769 6467 6574 2e73  fit_btn_widget.s
-0001d110: 6574 5061 6c65 7474 6528 7061 6c65 7474  etPalette(palett
-0001d120: 6529 0a20 2020 2020 2020 2070 616c 6574  e).        palet
-0001d130: 7465 2e73 6574 436f 6c6f 7228 5174 4775  te.setColor(QtGu
-0001d140: 692e 5150 616c 6574 7465 2e42 7574 746f  i.QPalette.Butto
-0001d150: 6e54 6578 742c 2051 7447 7569 2e51 436f  nText, QtGui.QCo
-0001d160: 6c6f 7228 2723 3462 3661 6164 2729 290a  lor('#4b6aad')).
-0001d170: 2020 2020 2020 2020 7265 7365 745f 6274          reset_bt
-0001d180: 6e5f 7769 6467 6574 2e73 6574 5061 6c65  n_widget.setPale
-0001d190: 7474 6528 7061 6c65 7474 6529 0a0a 2020  tte(palette)..  
-0001d1a0: 2020 2020 2020 2320 4b65 7962 6f61 7264        # Keyboard
-0001d1b0: 2073 686f 7274 6375 742c 2070 7265 7373   shortcut, press
-0001d1c0: 2066 2074 6f20 6669 7420 6966 2066 6974   f to fit if fit
-0001d1d0: 2062 7574 746f 6e20 6e6f 7420 6772 6579   button not grey
-0001d1e0: 6564 206f 7574 0a20 2020 2020 2020 2073  ed out.        s
-0001d1f0: 656c 662e 6669 745f 7368 6f72 7463 7574  elf.fit_shortcut
-0001d200: 203d 2051 7457 6964 6765 7473 2e51 5368   = QtWidgets.QSh
-0001d210: 6f72 7463 7574 2851 7447 7569 2e51 4b65  ortcut(QtGui.QKe
-0001d220: 7953 6571 7565 6e63 6528 2766 2729 2c20  ySequence('f'), 
-0001d230: 7365 6c66 290a 2020 2020 2020 2020 7365  self).        se
-0001d240: 6c66 2e66 6974 5f73 686f 7274 6375 742e  lf.fit_shortcut.
-0001d250: 6163 7469 7661 7465 642e 636f 6e6e 6563  activated.connec
-0001d260: 7428 0a20 2020 2020 2020 2020 2020 206c  t(.            l
-0001d270: 616d 6264 613a 2073 656c 662e 6b65 7962  ambda: self.keyb
-0001d280: 6f61 7264 5f66 6974 5f63 616c 6c62 6163  oard_fit_callbac
-0001d290: 6b28 290a 2020 2020 2020 2020 290a 0a20  k().        ).. 
-0001d2a0: 2020 2020 2020 2062 6f74 5f72 6f77 5f6c         bot_row_l
-0001d2b0: 6179 6f75 7420 3d20 5174 5769 6467 6574  ayout = QtWidget
-0001d2c0: 732e 5148 426f 784c 6179 6f75 7428 626f  s.QHBoxLayout(bo
-0001d2d0: 745f 726f 775f 7769 6467 6574 290a 2020  t_row_widget).  
-0001d2e0: 2020 2020 2020 626f 745f 726f 775f 6c61        bot_row_la
-0001d2f0: 796f 7574 2e61 6464 5769 6467 6574 2873  yout.addWidget(s
-0001d300: 656c 662e 6669 745f 6274 6e5f 7769 6467  elf.fit_btn_widg
-0001d310: 6574 290a 2020 2020 2020 2020 626f 745f  et).        bot_
-0001d320: 726f 775f 6c61 796f 7574 2e61 6464 5769  row_layout.addWi
-0001d330: 6467 6574 2872 6573 6574 5f62 746e 5f77  dget(reset_btn_w
-0001d340: 6964 6765 7429 0a0a 2020 2020 2020 2020  idget)..        
-0001d350: 2320 4f76 6572 616c 6c20 6170 700a 2020  # Overall app.  
-0001d360: 2020 2020 2020 2320 546f 7020 616e 6420        # Top and 
-0001d370: 426f 7474 6f6d 2072 6f77 730a 2020 2020  Bottom rows.    
-0001d380: 2020 2020 6675 6c6c 5f6c 6179 6f75 7420      full_layout 
-0001d390: 3d20 5174 5769 6467 6574 732e 5156 426f  = QtWidgets.QVBo
-0001d3a0: 784c 6179 6f75 7428 7365 6c66 2e77 6964  xLayout(self.wid
-0001d3b0: 6765 7429 0a20 2020 2020 2020 2066 756c  get).        ful
-0001d3c0: 6c5f 6c61 796f 7574 2e61 6464 5769 6467  l_layout.addWidg
-0001d3d0: 6574 2874 6f70 5f72 6f77 5f77 6964 6765  et(top_row_widge
-0001d3e0: 7429 0a20 2020 2020 2020 2066 756c 6c5f  t).        full_
-0001d3f0: 6c61 796f 7574 2e61 6464 5769 6467 6574  layout.addWidget
-0001d400: 2862 6f74 5f72 6f77 5f77 6964 6765 7429  (bot_row_widget)
-0001d410: 0a0a 2020 2020 2020 2020 2320 5365 7420  ..        # Set 
-0001d420: 6c61 796f 7574 0a20 2020 2020 2020 2073  layout.        s
-0001d430: 656c 662e 7769 6467 6574 2e73 6574 4c61  elf.widget.setLa
-0001d440: 796f 7574 2866 756c 6c5f 6c61 796f 7574  yout(full_layout
-0001d450: 290a 2020 2020 2020 2020 7365 6c66 2e77  ).        self.w
-0001d460: 6964 6765 742e 7365 7453 697a 6550 6f6c  idget.setSizePol
-0001d470: 6963 7928 0a20 2020 2020 2020 2020 2020  icy(.           
-0001d480: 2051 7457 6964 6765 7473 2e51 5369 7a65   QtWidgets.QSize
-0001d490: 506f 6c69 6379 2e45 7870 616e 6469 6e67  Policy.Expanding
-0001d4a0: 2c0a 2020 2020 2020 2020 2020 2020 5174  ,.            Qt
-0001d4b0: 5769 6467 6574 732e 5153 697a 6550 6f6c  Widgets.QSizePol
-0001d4c0: 6963 792e 4578 7061 6e64 696e 670a 2020  icy.Expanding.  
-0001d4d0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-0001d4e0: 2072 6574 7572 6e0a 0a20 2020 2064 6566   return..    def
-0001d4f0: 206b 6579 626f 6172 645f 6669 745f 6361   keyboard_fit_ca
-0001d500: 6c6c 6261 636b 2873 656c 6629 3a0a 2020  llback(self):.  
-0001d510: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-0001d520: 2020 4361 6c6c 6261 636b 2066 6f72 2070    Callback for p
-0001d530: 7265 7373 696e 6720 2766 2720 6b65 792e  ressing 'f' key.
-0001d540: 2052 756e 7320 6669 7420 6275 7474 6f6e   Runs fit button
-0001d550: 2069 6620 6e6f 7420 6772 6579 6564 206f   if not greyed o
-0001d560: 7574 0a20 2020 2020 2020 2027 2727 0a0a  ut.        '''..
-0001d570: 2020 2020 2020 2020 2320 4368 6563 6b20          # Check 
-0001d580: 6669 7420 6275 7474 6f6e 2069 7320 6e6f  fit button is no
-0001d590: 7420 6772 6579 6564 206f 7574 0a20 2020  t greyed out.   
-0001d5a0: 2020 2020 2069 6620 7365 6c66 2e66 6974       if self.fit
-0001d5b0: 5f62 746e 5f77 6964 6765 742e 6973 456e  _btn_widget.isEn
-0001d5c0: 6162 6c65 6428 293a 0a20 2020 2020 2020  abled():.       
-0001d5d0: 2020 2020 2023 2052 756e 2066 6974 2063       # Run fit c
-0001d5e0: 6f64 652c 2074 6869 7320 636c 6f73 6573  ode, this closes
-0001d5f0: 2061 7070 0a20 2020 2020 2020 2020 2020   app.           
-0001d600: 2073 656c 662e 6669 7428 290a 0a20 2020   self.fit()..   
-0001d610: 2020 2020 2072 6574 7572 6e0a 0a20 2020       return..   
-0001d620: 2064 6566 2072 6573 6574 2873 656c 6629   def reset(self)
-0001d630: 3a0a 2020 2020 2020 2020 2727 270a 2020  :.        '''.  
-0001d640: 2020 2020 2020 4361 6c6c 6261 636b 2066        Callback f
-0001d650: 6f72 2052 6573 6574 2062 7574 746f 6e2e  or Reset button.
-0001d660: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-0001d670: 2077 696e 646f 7720 6261 636b 2074 6f20   window back to 
-0001d680: 6f72 6967 696e 616c 206c 6179 6f75 742f  original layout/
-0001d690: 7365 6c65 6374 696f 6e73 0a20 2020 2020  selections.     
-0001d6a0: 2020 2027 2727 0a0a 2020 2020 2020 2020     '''..        
-0001d6b0: 2320 466f 7220 6561 6368 206d 6f64 656c  # For each model
-0001d6c0: 2c20 7265 6d6f 7665 2070 6c6f 742c 2061  , remove plot, a
-0001d6d0: 6e64 2072 6573 6574 2070 6172 616d 6574  nd reset paramet
-0001d6e0: 6572 2076 616c 7565 730a 2020 2020 2020  er values.      
-0001d6f0: 2020 666f 7220 6d6f 6465 6c20 696e 2073    for model in s
-0001d700: 656c 662e 7375 7070 6f72 7465 645f 6d6f  elf.supported_mo
-0001d710: 6465 6c73 3a0a 2020 2020 2020 2020 2020  dels:.          
-0001d720: 2020 6d6f 6465 6c6e 616d 6520 3d20 6d6f    modelname = mo
-0001d730: 6465 6c2e 4e41 4d45 2e6c 6f77 6572 2829  del.NAME.lower()
-0001d740: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-0001d750: 4469 7361 626c 6520 616c 6c20 6d6f 6465  Disable all mode
-0001d760: 6c73 0a20 2020 2020 2020 2020 2020 2073  ls.            s
-0001d770: 656c 662e 7573 656c 2e6d 6f64 656c 735b  elf.usel.models[
-0001d780: 6d6f 6465 6c6e 616d 655d 203d 2046 616c  modelname] = Fal
-0001d790: 7365 0a20 2020 2020 2020 2020 2020 2023  se.            #
-0001d7a0: 2061 6e64 2075 6e74 6963 6b20 6368 6563   and untick chec
-0001d7b0: 6b62 6f78 6573 0a20 2020 2020 2020 2020  kboxes.         
-0001d7c0: 2020 2073 656c 662e 7469 636b 6469 6374     self.tickdict
-0001d7d0: 5b6d 6f64 656c 6e61 6d65 5d2e 7365 7443  [modelname].setC
-0001d7e0: 6865 636b 5374 6174 6528 4661 6c73 6529  heckState(False)
-0001d7f0: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-0001d800: 5265 6d6f 7665 2063 6f72 7265 7370 6f6e  Remove correspon
-0001d810: 6469 6e67 2070 6c6f 740a 2020 2020 2020  ding plot.      
-0001d820: 2020 2020 2020 5f70 6c6f 7420 3d20 7365        _plot = se
-0001d830: 6c66 2e6d 6f64 656c 5f70 6c6f 7473 5b6d  lf.model_plots[m
-0001d840: 6f64 656c 6e61 6d65 5d0a 2020 2020 2020  odelname].      
-0001d850: 2020 2020 2020 7365 6c66 2e70 6c6f 745f        self.plot_
-0001d860: 7769 6467 6574 2e72 656d 6f76 6549 7465  widget.removeIte
-0001d870: 6d28 5f70 6c6f 7429 0a0a 2020 2020 2020  m(_plot)..      
-0001d880: 2020 2020 2020 2320 5265 7365 7420 6561        # Reset ea
-0001d890: 6368 2070 6172 616d 6574 6572 2073 6c69  ch parameter sli
-0001d8a0: 6465 722c 2065 6e74 7279 2c20 616e 6420  der, entry, and 
-0001d8b0: 6669 7466 6978 0a20 2020 2020 2020 2020  fitfix.         
-0001d8c0: 2020 2023 2062 6163 6b20 746f 206f 7269     # back to ori
-0001d8d0: 6769 6e61 6c20 7661 6c75 650a 2020 2020  ginal value.    
-0001d8e0: 2020 2020 2020 2020 666f 7220 7061 726e          for parn
-0001d8f0: 616d 6520 696e 206d 6f64 656c 2e50 4152  ame in model.PAR
-0001d900: 4e41 4d45 533a 0a20 2020 2020 2020 2020  NAMES:.         
-0001d910: 2020 2020 2020 2073 6574 6174 7472 280a         setattr(.
-0001d920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d930: 2020 2020 7365 6c66 2e70 6172 7374 6f72      self.parstor
-0001d940: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0001d950: 2020 2020 2020 2070 6172 6e61 6d65 2c0a         parname,.
-0001d960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d970: 2020 2020 7365 6c66 2e64 6566 6175 6c74      self.default
-0001d980: 735b 6d6f 6465 6c2e 4e41 4d45 5d5b 7061  s[model.NAME][pa
-0001d990: 726e 616d 655d 5b27 7661 6c69 6e69 7427  rname]['valinit'
-0001d9a0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0001d9b0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0001d9c0: 2020 2020 7365 6c66 2e77 6964 6765 7464      self.widgetd
-0001d9d0: 6963 745b 6d6f 6465 6c6e 616d 655d 5b70  ict[modelname][p
-0001d9e0: 6172 6e61 6d65 5d5b 2773 6c69 6465 7227  arname]['slider'
-0001d9f0: 5d2e 7365 7456 616c 7565 280a 2020 2020  ].setValue(.    
+00018880: 2020 2020 2020 2020 2020 2073 6967 6d61             sigma
+00018890: 3a20 6e70 742e 4172 7261 794c 696b 6520  : npt.ArrayLike 
+000188a0: 3d20 5b5d 2920 2d3e 206e 7074 2e4e 4441  = []) -> npt.NDA
+000188b0: 7272 6179 3a0a 2020 2020 2020 2020 2727  rray:.        ''
+000188c0: 270a 2020 2020 2020 2020 5772 6170 7065  '.        Wrappe
+000188d0: 7220 666f 7220 6072 6573 6964 7561 6c73  r for `residuals
+000188e0: 6020 6d65 7468 6f64 2c20 7461 6b65 7320  ` method, takes 
+000188f0: 6e65 7720 7661 6c75 6573 2066 726f 6d20  new values from 
+00018900: 6669 7474 696e 6720 726f 7574 696e 650a  fitting routine.
+00018910: 2020 2020 2020 2020 7768 6963 6820 7072          which pr
+00018920: 6f76 6964 6573 206c 6973 745b 666c 6f61  ovides list[floa
+00018930: 745d 2c20 746f 2063 6f6e 7374 7275 6374  t], to construct
+00018940: 206e 6577 2066 6974 5f76 6172 7320 6469   new fit_vars di
+00018950: 6374 2c20 7468 656e 0a20 2020 2020 2020  ct, then.       
+00018960: 2072 756e 7320 6072 6573 6964 7561 6c73   runs `residuals
+00018970: 6020 6d65 7468 6f64 2e0a 0a20 2020 2020  ` method...     
+00018980: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00018990: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+000189a0: 0a20 2020 2020 2020 206e 6577 5f76 616c  .        new_val
+000189b0: 733a 2061 7272 6179 5f6c 696b 650a 2020  s: array_like.  
+000189c0: 2020 2020 2020 2020 2020 5468 6973 2069            This i
+000189d0: 7465 7261 7469 6f6e 2773 2066 6974 2070  teration's fit p
+000189e0: 6172 616d 6574 6572 2076 616c 7565 7320  arameter values 
+000189f0: 7072 6f76 6964 6564 2062 7920 6c65 6173  provided by leas
+00018a00: 745f 7371 7561 7265 730a 2020 2020 2020  t_squares.      
+00018a10: 2020 2020 2020 7468 6973 2068 6173 2074        this has t
+00018a20: 6865 2073 616d 6520 6f72 6465 7220 6174  he same order at
+00018a30: 2066 6974 5f76 6172 732e 6b65 7973 0a20   fit_vars.keys. 
+00018a40: 2020 2020 2020 206c 6f67 6d6f 6465 6c73         logmodels
+00018a50: 3a20 6c69 7374 5b4c 6f67 5461 7554 4d6f  : list[LogTauTMo
+00018a60: 6465 6c5d 0a20 2020 2020 2020 2020 2020  del].           
+00018a70: 204d 6f64 656c 7320 746f 2075 7365 0a20   Models to use. 
+00018a80: 2020 2020 2020 2074 656d 7065 7261 7475         temperatu
+00018a90: 7265 733a 2061 7272 6179 5f6c 696b 650a  res: array_like.
+00018aa0: 2020 2020 2020 2020 2020 2020 5465 6d70              Temp
+00018ab0: 6572 6174 7572 6520 7661 6c75 6573 2028  erature values (
+00018ac0: 4b29 2061 7420 7768 6963 6820 6d6f 6465  K) at which mode
+00018ad0: 6c20 6675 6e63 7469 6f6e 2069 7320 6576  l function is ev
+00018ae0: 616c 7561 7465 640a 2020 2020 2020 2020  aluated.        
+00018af0: 6c6f 6772 6174 653a 2061 7272 6179 5f6c  lograte: array_l
+00018b00: 696b 650a 2020 2020 2020 2020 2020 2020  ike.            
+00018b10: 5472 7565 2028 6578 7065 7269 6d65 6e74  True (experiment
+00018b20: 616c 2920 7661 6c75 6573 206f 6620 6c6f  al) values of lo
+00018b30: 6731 3028 7265 6c61 7861 7469 6f6e 2072  g10(relaxation r
+00018b40: 6174 6529 0a20 2020 2020 2020 2073 6967  ate).        sig
+00018b50: 6d61 3a20 6172 7261 795f 6c69 6b65 0a20  ma: array_like. 
+00018b60: 2020 2020 2020 2020 2020 2053 7461 6e64             Stand
+00018b70: 6172 6420 6465 7669 6174 696f 6e20 6f66  ard deviation of
+00018b80: 2074 6175 2069 6e20 6c6f 6773 7061 6365   tau in logspace
+00018b90: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00018ba0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00018bb0: 2d0a 2020 2020 2020 2020 6e64 6172 7261  -.        ndarra
+00018bc0: 7920 6f66 2066 6c6f 6174 730a 2020 2020  y of floats.    
+00018bd0: 2020 2020 2020 2020 5265 7369 6475 616c          Residual
+00018be0: 730a 2020 2020 2020 2020 2727 270a 0a20  s.        '''.. 
+00018bf0: 2020 2020 2020 2023 2053 7761 7020 6669         # Swap fi
+00018c00: 7420 7661 6c75 6573 2066 6f72 206e 6577  t values for new
+00018c10: 2076 616c 7565 7320 6672 6f6d 2066 6974   values from fit
+00018c20: 2072 6f75 7469 6e65 0a20 2020 2020 2020   routine.       
+00018c30: 206e 6577 5f66 6974 5f76 6172 7320 3d20   new_fit_vars = 
+00018c40: 5b5d 0a0a 2020 2020 2020 2020 6974 203d  []..        it =
+00018c50: 2030 0a20 2020 2020 2020 2066 6f72 206c   0.        for l
+00018c60: 6f67 6d6f 6465 6c20 696e 206c 6f67 6d6f  ogmodel in logmo
+00018c70: 6465 6c73 3a0a 2020 2020 2020 2020 2020  dels:.          
+00018c80: 2020 6e65 775f 6469 6374 203d 207b 7d0a    new_dict = {}.
+00018c90: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00018ca0: 6e61 6d65 2069 6e20 6c6f 676d 6f64 656c  name in logmodel
+00018cb0: 2e66 6974 5f76 6172 732e 6b65 7973 2829  .fit_vars.keys()
+00018cc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00018cd0: 2020 6e65 775f 6469 6374 5b6e 616d 655d    new_dict[name]
+00018ce0: 203d 206e 6577 5f76 616c 735b 6974 5d0a   = new_vals[it].
+00018cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018d00: 6974 202b 3d20 310a 2020 2020 2020 2020  it += 1.        
+00018d10: 2020 2020 6e65 775f 6669 745f 7661 7273      new_fit_vars
+00018d20: 2e61 7070 656e 6428 6e65 775f 6469 6374  .append(new_dict
+00018d30: 290a 0a20 2020 2020 2020 2072 6573 6964  )..        resid
+00018d40: 7561 6c73 203d 2063 6c73 2e72 6573 6964  uals = cls.resid
+00018d50: 7561 6c73 280a 2020 2020 2020 2020 2020  uals(.          
+00018d60: 2020 6c6f 676d 6f64 656c 732c 206e 6577    logmodels, new
+00018d70: 5f66 6974 5f76 6172 732c 2074 656d 7065  _fit_vars, tempe
+00018d80: 7261 7475 7265 732c 206c 6f67 7261 7465  ratures, lograte
+00018d90: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00018da0: 2020 2020 6966 206c 656e 2873 6967 6d61      if len(sigma
+00018db0: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+00018dc0: 6573 6964 7561 6c73 202f 3d20 7369 676d  esiduals /= sigm
+00018dd0: 610a 0a20 2020 2020 2020 2072 6574 7572  a..        retur
+00018de0: 6e20 7265 7369 6475 616c 730a 0a20 2020  n residuals..   
+00018df0: 2040 7374 6174 6963 6d65 7468 6f64 0a20   @staticmethod. 
+00018e00: 2020 2064 6566 2072 6573 6964 7561 6c73     def residuals
+00018e10: 286c 6f67 6d6f 6465 6c73 3a20 6c69 7374  (logmodels: list
+00018e20: 5b4c 6f67 5461 7554 4d6f 6465 6c5d 2c0a  [LogTauTModel],.
+00018e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018e40: 2020 6e65 775f 6669 745f 7661 7273 3a20    new_fit_vars: 
+00018e50: 6c69 7374 5b64 6963 745b 7374 722c 2066  list[dict[str, f
+00018e60: 6c6f 6174 5d5d 2c0a 2020 2020 2020 2020  loat]],.        
+00018e70: 2020 2020 2020 2020 2020 7465 6d70 6572            temper
+00018e80: 6174 7572 6573 3a20 6e70 742e 4172 7261  atures: npt.Arra
+00018e90: 794c 696b 652c 0a20 2020 2020 2020 2020  yLike,.         
+00018ea0: 2020 2020 2020 2020 2074 7275 655f 6c6f           true_lo
+00018eb0: 6772 6174 653a 206e 7074 2e41 7272 6179  grate: npt.Array
+00018ec0: 4c69 6b65 2920 2d3e 206e 7074 2e4e 4441  Like) -> npt.NDA
+00018ed0: 7272 6179 3a0a 2020 2020 2020 2020 2727  rray:.        ''
+00018ee0: 270a 2020 2020 2020 2020 4361 6c63 756c  '.        Calcul
+00018ef0: 6174 6573 2064 6966 6665 7265 6e63 6520  ates difference 
+00018f00: 6265 7477 6565 6e20 6578 7065 7269 6d65  between experime
+00018f10: 6e74 616c 206c 6f67 3130 2874 6175 5e2d  ntal log10(tau^-
+00018f20: 3129 0a20 2020 2020 2020 2061 6e64 206c  1).        and l
+00018f30: 6f67 3130 2874 6175 5e2d 3129 206f 6274  og10(tau^-1) obt
+00018f40: 6169 6e65 6420 6672 6f6d 2074 6865 2073  ained from the s
+00018f50: 756d 206f 6620 7468 6520 7072 6f76 6964  um of the provid
+00018f60: 6564 206c 6f67 6d6f 6465 6c73 0a20 2020  ed logmodels.   
+00018f70: 2020 2020 2075 7369 6e67 2074 6865 2070       using the p
+00018f80: 726f 7669 6465 6420 6669 7420 7661 7269  rovided fit vari
+00018f90: 6162 6c65 2076 616c 7565 7320 6174 2070  able values at p
+00018fa0: 726f 7669 6465 6420 7465 6d70 6572 6174  rovided temperat
+00018fb0: 7572 6573 0a0a 2020 2020 2020 2020 5061  ures..        Pa
+00018fc0: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+00018fd0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00018fe0: 2020 2020 6c6f 676d 6f64 656c 733a 206c      logmodels: l
+00018ff0: 6973 745b 4c6f 6754 6175 544d 6f64 656c  ist[LogTauTModel
+00019000: 5d0a 2020 2020 2020 2020 2020 2020 4c6f  ].            Lo
+00019010: 6754 6175 544d 6f64 656c 7320 7768 6963  gTauTModels whic
+00019020: 6820 7769 6c6c 2062 6520 6576 616c 7561  h will be evalua
+00019030: 7465 640a 2020 2020 2020 2020 6e65 775f  ted.        new_
+00019040: 6669 745f 7661 7273 3a20 6c69 7374 5b64  fit_vars: list[d
+00019050: 6963 745b 7374 722c 2066 6c6f 6174 5d5d  ict[str, float]]
+00019060: 0a20 2020 2020 2020 2020 2020 2066 6974  .            fit
+00019070: 2064 6963 7473 2066 6f72 2065 6163 6820   dicts for each 
+00019080: 4c6f 6754 6175 544d 6f64 656c 2c20 6d75  LogTauTModel, mu
+00019090: 7374 2068 6176 6520 7361 6d65 206f 7264  st have same ord
+000190a0: 6572 2061 7320 6c6f 676d 6f64 656c 0a20  er as logmodel. 
+000190b0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+000190c0: 2076 6172 7320 746f 2066 6974 2066 6f72   vars to fit for
+000190d0: 2074 6861 7420 6d6f 6465 6c2c 2074 6865   that model, the
+000190e0: 6e20 656d 7074 7920 6469 6374 2069 7320  n empty dict is 
+000190f0: 6769 7665 6e0a 2020 2020 2020 2020 7465  given.        te
+00019100: 6d70 6572 6174 7572 6573 3a20 6172 7261  mperatures: arra
+00019110: 795f 6c69 6b65 0a20 2020 2020 2020 2020  y_like.         
+00019120: 2020 2045 7870 6572 696d 656e 7461 6c20     Experimental 
+00019130: 7465 6d70 6572 6174 7572 6573 2028 4b29  temperatures (K)
+00019140: 0a20 2020 2020 2020 2074 7275 655f 6c6f  .        true_lo
+00019150: 6772 6174 653a 2061 7272 6179 5f6c 696b  grate: array_lik
+00019160: 650a 2020 2020 2020 2020 2020 2020 4578  e.            Ex
+00019170: 7065 7269 6d65 6e74 616c 204c 6f67 3130  perimental Log10
+00019180: 2872 6174 6529 730a 0a20 2020 2020 2020  (rate)s..       
+00019190: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+000191a0: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+000191b0: 206e 6461 7272 6179 206f 6620 666c 6f61   ndarray of floa
+000191c0: 7473 0a20 2020 2020 2020 2020 2020 204c  ts.            L
+000191d0: 6f67 3130 2872 6174 6529 5f74 7269 616c  og10(rate)_trial
+000191e0: 202d 204c 6f67 3130 2872 6174 6529 5f65   - Log10(rate)_e
+000191f0: 7870 2066 6f72 2065 6163 6820 7465 6d70  xp for each temp
+00019200: 6572 6174 7572 650a 2020 2020 2020 2020  erature.        
+00019210: 2727 270a 0a20 2020 2020 2020 2023 2043  '''..        # C
+00019220: 616c 6375 6c61 7465 206d 6f64 656c 206c  alculate model l
+00019230: 6f67 3130 2872 656c 6178 6174 696f 6e20  og10(relaxation 
+00019240: 7261 7465 2920 7573 696e 6720 7061 7261  rate) using para
+00019250: 6d65 7465 7273 0a20 2020 2020 2020 2023  meters.        #
+00019260: 2061 7320 7375 6d20 6f66 2063 6f6e 7472   as sum of contr
+00019270: 6962 7574 696f 6e73 2066 726f 6d20 6561  ibutions from ea
+00019280: 6368 2070 726f 6365 7373 0a20 2020 2020  ch process.     
+00019290: 2020 2074 7269 616c 5f6c 6f67 7261 7465     trial_lograte
+000192a0: 203d 206e 702e 7a65 726f 7328 6c65 6e28   = np.zeros(len(
+000192b0: 7465 6d70 6572 6174 7572 6573 2929 0a0a  temperatures))..
+000192c0: 2020 2020 2020 2020 666f 7220 6c6f 676d          for logm
+000192d0: 6f64 656c 2c20 6669 745f 7661 7273 2069  odel, fit_vars i
+000192e0: 6e20 7a69 7028 6c6f 676d 6f64 656c 732c  n zip(logmodels,
+000192f0: 206e 6577 5f66 6974 5f76 6172 7329 3a0a   new_fit_vars):.
+00019300: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
+00019310: 7661 7273 203d 207b 2a2a 6c6f 676d 6f64  vars = {**logmod
+00019320: 656c 2e66 6978 5f76 6172 732c 202a 2a66  el.fix_vars, **f
+00019330: 6974 5f76 6172 737d 0a20 2020 2020 2020  it_vars}.       
+00019340: 2020 2020 2074 7269 616c 5f6c 6f67 7261       trial_logra
+00019350: 7465 202b 3d20 3130 2a2a 6c6f 676d 6f64  te += 10**logmod
+00019360: 656c 2e6d 6f64 656c 2861 6c6c 5f76 6172  el.model(all_var
+00019370: 732c 2074 656d 7065 7261 7475 7265 7329  s, temperatures)
+00019380: 0a0a 2020 2020 2020 2020 2320 7375 6d20  ..        # sum 
+00019390: 696e 206c 696e 6561 7220 7370 6163 652c  in linear space,
+000193a0: 2074 6865 6e20 7461 6b65 206c 6f67 0a20   then take log. 
+000193b0: 2020 2020 2020 2074 7269 616c 5f6c 6f67         trial_log
+000193c0: 7261 7465 203d 206e 702e 6c6f 6731 3028  rate = np.log10(
+000193d0: 7472 6961 6c5f 6c6f 6772 6174 6529 0a0a  trial_lograte)..
+000193e0: 2020 2020 2020 2020 7265 7369 6475 616c          residual
+000193f0: 7320 3d20 7472 6961 6c5f 6c6f 6772 6174  s = trial_lograt
+00019400: 6520 2d20 7472 7565 5f6c 6f67 7261 7465  e - true_lograte
+00019410: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00019420: 2072 6573 6964 7561 6c73 0a0a 2020 2020   residuals..    
+00019430: 6465 6620 6669 745f 746f 2873 656c 662c  def fit_to(self,
+00019440: 2064 6174 6173 6574 3a20 5461 7554 4461   dataset: TauTDa
+00019450: 7461 7365 742c 2076 6572 626f 7365 3a20  taset, verbose: 
+00019460: 626f 6f6c 203d 2054 7275 6529 202d 3e20  bool = True) -> 
+00019470: 4e6f 6e65 3a0a 2020 2020 2020 2020 2727  None:.        ''
+00019480: 270a 2020 2020 2020 2020 4669 7473 206d  '.        Fits m
+00019490: 6f64 656c 2074 6f20 4461 7461 7365 740a  odel to Dataset.
+000194a0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+000194b0: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+000194c0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2064  ------.        d
+000194d0: 6174 6173 6574 3a20 5461 7554 4461 7461  ataset: TauTData
+000194e0: 7365 740a 2020 2020 2020 2020 2020 2020  set.            
+000194f0: 4461 7461 7365 7420 746f 2077 6869 6368  Dataset to which
+00019500: 2061 206d 6f64 656c 206f 6620 7261 7465   a model of rate
+00019510: 2076 7320 7465 6d70 6572 6174 7572 6520   vs temperature 
+00019520: 7769 6c6c 2062 6520 6669 7474 6564 0a20  will be fitted. 
+00019530: 2020 2020 2020 2076 6572 626f 7365 3a20         verbose: 
+00019540: 626f 6f6c 2c20 6465 6661 756c 7420 5472  bool, default Tr
+00019550: 7565 0a20 2020 2020 2020 2020 2020 2049  ue.            I
+00019560: 6620 5472 7565 2c20 7072 696e 7473 2069  f True, prints i
+00019570: 6e66 6f72 6d61 7469 6f6e 2074 6f20 7465  nformation to te
+00019580: 726d 696e 616c 0a0a 2020 2020 2020 2020  rminal..        
+00019590: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+000195a0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+000195b0: 4e6f 6e65 0a20 2020 2020 2020 2027 2727  None.        '''
+000195c0: 0a0a 2020 2020 2020 2020 2320 496e 6974  ..        # Init
+000195d0: 6961 6c20 6775 6573 7320 6973 2061 206c  ial guess is a l
+000195e0: 6973 7420 6f66 2066 6974 7661 7273 2076  ist of fitvars v
+000195f0: 616c 7565 730a 2020 2020 2020 2020 6775  alues.        gu
+00019600: 6573 7320 3d20 5b0a 2020 2020 2020 2020  ess = [.        
+00019610: 2020 2020 7661 6c75 6520 666f 7220 6c6f      value for lo
+00019620: 676d 6f64 656c 2069 6e20 7365 6c66 2e6c  gmodel in self.l
+00019630: 6f67 6d6f 6465 6c73 0a20 2020 2020 2020  ogmodels.       
+00019640: 2020 2020 2066 6f72 2076 616c 7565 2069       for value i
+00019650: 6e20 6c6f 676d 6f64 656c 2e66 6974 5f76  n logmodel.fit_v
+00019660: 6172 732e 7661 6c75 6573 2829 0a20 2020  ars.values().   
+00019670: 2020 2020 205d 0a0a 2020 2020 2020 2020       ]..        
+00019680: 626f 756e 6473 203d 206e 702e 6172 7261  bounds = np.arra
+00019690: 7928 5b0a 2020 2020 2020 2020 2020 2020  y([.            
+000196a0: 6c6f 676d 6f64 656c 2e42 4f55 4e44 535b  logmodel.BOUNDS[
+000196b0: 6e61 6d65 5d20 666f 7220 6c6f 676d 6f64  name] for logmod
+000196c0: 656c 2069 6e20 7365 6c66 2e6c 6f67 6d6f  el in self.logmo
+000196d0: 6465 6c73 0a20 2020 2020 2020 2020 2020  dels.           
+000196e0: 2066 6f72 206e 616d 6520 696e 206c 6f67   for name in log
+000196f0: 6d6f 6465 6c2e 6669 745f 7661 7273 2e6b  model.fit_vars.k
+00019700: 6579 7328 290a 2020 2020 2020 2020 5d29  eys().        ])
+00019710: 2e54 0a0a 2020 2020 2020 2020 6375 7272  .T..        curr
+00019720: 5f66 6974 203d 206c 6561 7374 5f73 7175  _fit = least_squ
+00019730: 6172 6573 280a 2020 2020 2020 2020 2020  ares(.          
+00019740: 2020 7365 6c66 2e72 6573 6964 7561 6c5f    self.residual_
+00019750: 6672 6f6d 5f66 6c6f 6174 5f6c 6973 742c  from_float_list,
+00019760: 0a20 2020 2020 2020 2020 2020 2061 7267  .            arg
+00019770: 733d 5b0a 2020 2020 2020 2020 2020 2020  s=[.            
+00019780: 2020 2020 7365 6c66 2e6c 6f67 6d6f 6465      self.logmode
+00019790: 6c73 2c0a 2020 2020 2020 2020 2020 2020  ls,.            
+000197a0: 2020 2020 6461 7461 7365 742e 7465 6d70      dataset.temp
+000197b0: 6572 6174 7572 6573 2c0a 2020 2020 2020  eratures,.      
+000197c0: 2020 2020 2020 2020 2020 6e70 2e6c 6f67            np.log
+000197d0: 3130 2864 6174 6173 6574 2e72 6174 6573  10(dataset.rates
+000197e0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+000197f0: 2020 2064 6174 6173 6574 2e6c 6f67 7261     dataset.logra
+00019800: 7465 5f70 6d0a 2020 2020 2020 2020 2020  te_pm.          
+00019810: 2020 5d2c 0a20 2020 2020 2020 2020 2020    ],.           
+00019820: 2078 303d 6775 6573 732c 0a20 2020 2020   x0=guess,.     
+00019830: 2020 2020 2020 2062 6f75 6e64 733d 626f         bounds=bo
+00019840: 756e 6473 2c0a 2020 2020 2020 2020 2020  unds,.          
+00019850: 2020 6a61 633d 2733 2d70 6f69 6e74 270a    jac='3-point'.
+00019860: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00019870: 2020 2069 6620 6375 7272 5f66 6974 2e73     if curr_fit.s
+00019880: 7461 7475 7320 3d3d 2030 3a0a 2020 2020  tatus == 0:.    
+00019890: 2020 2020 2020 2020 6966 2076 6572 626f          if verbo
+000198a0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000198b0: 2020 2020 7574 2e63 7072 696e 7428 0a20      ut.cprint(. 
+000198c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000198d0: 2020 2027 5c6e 2046 6974 2066 6169 6c65     '\n Fit faile
+000198e0: 6420 2d20 546f 6f20 6d61 6e79 2069 7465  d - Too many ite
+000198f0: 7261 7469 6f6e 7327 2c0a 2020 2020 2020  rations',.      
+00019900: 2020 2020 2020 2020 2020 2020 2020 2762                'b
+00019910: 6c61 636b 5f79 656c 6c6f 7762 6727 0a20  lack_yellowbg'. 
+00019920: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00019930: 0a0a 2020 2020 2020 2020 2020 2020 6e5f  ..            n_
+00019940: 6669 7474 6564 5f70 6172 7320 3d20 6e70  fitted_pars = np
+00019950: 2e73 756d 280a 2020 2020 2020 2020 2020  .sum(.          
+00019960: 2020 2020 2020 5b6c 656e 286c 6f67 6d6f        [len(logmo
+00019970: 6465 6c2e 6669 745f 7661 7273 2e6b 6579  del.fit_vars.key
+00019980: 7328 2929 2066 6f72 206c 6f67 6d6f 6465  s()) for logmode
+00019990: 6c20 696e 2073 656c 662e 6c6f 676d 6f64  l in self.logmod
+000199a0: 656c 735d 0a20 2020 2020 2020 2020 2020  els].           
+000199b0: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
+000199c0: 7374 6465 7620 3d20 5b6e 702e 6e61 6e5d  stdev = [np.nan]
+000199d0: 202a 206e 5f66 6974 7465 645f 7061 7273   * n_fitted_pars
+000199e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000199f0: 662e 6669 745f 7374 6174 7573 203d 2046  f.fit_status = F
+00019a00: 616c 7365 0a20 2020 2020 2020 2065 6c73  alse.        els
+00019a10: 653a 0a0a 2020 2020 2020 2020 2020 2020  e:..            
+00019a20: 7374 6465 762c 206e 6f5f 7374 6465 7620  stdev, no_stdev 
+00019a30: 3d20 7374 6174 732e 7376 645f 7374 6465  = stats.svd_stde
+00019a40: 7628 6375 7272 5f66 6974 290a 0a20 2020  v(curr_fit)..   
+00019a50: 2020 2020 2020 2020 2073 656c 662e 6669           self.fi
+00019a60: 745f 7374 6174 7573 203d 2054 7275 650a  t_status = True.
+00019a70: 0a20 2020 2020 2020 2023 2041 6464 2070  .        # Add p
+00019a80: 6172 616d 6574 6572 732c 2073 7461 7475  arameters, statu
+00019a90: 7320 616e 6420 7374 6465 7620 746f 2065  s and stdev to e
+00019aa0: 6163 6820 4c6f 6754 6175 544d 6f64 656c  ach LogTauTModel
+00019ab0: 0a20 2020 2020 2020 2069 7420 3d20 300a  .        it = 0.
+00019ac0: 2020 2020 2020 2020 666f 7220 6c6f 676d          for logm
+00019ad0: 6f64 656c 2069 6e20 7365 6c66 2e6c 6f67  odel in self.log
+00019ae0: 6d6f 6465 6c73 3a0a 0a20 2020 2020 2020  models:..       
+00019af0: 2020 2020 2023 204e 616d 6520 6f66 2066       # Name of f
+00019b00: 6974 7465 6420 7661 7269 6162 6c65 7320  itted variables 
+00019b10: 696e 2074 6869 7320 6c6f 676d 6f64 656c  in this logmodel
+00019b20: 0a20 2020 2020 2020 2020 2020 2066 6974  .            fit
+00019b30: 5f76 6172 5f6e 616d 6573 203d 206c 6f67  _var_names = log
+00019b40: 6d6f 6465 6c2e 6669 745f 7661 7273 2e6b  model.fit_vars.k
+00019b50: 6579 7328 290a 2020 2020 2020 2020 2020  eys().          
+00019b60: 2020 2320 4e75 6d62 6572 206f 6620 7061    # Number of pa
+00019b70: 7261 6d65 7465 7273 2066 6f72 2074 6869  rameters for thi
+00019b80: 7320 6c6f 676d 6f64 656c 0a20 2020 2020  s logmodel.     
+00019b90: 2020 2020 2020 206e 5f70 6172 7320 3d20         n_pars = 
+00019ba0: 6c65 6e28 6669 745f 7661 725f 6e61 6d65  len(fit_var_name
+00019bb0: 7329 0a0a 2020 2020 2020 2020 2020 2020  s)..            
+00019bc0: 2320 5365 7420 6561 6368 2073 7461 6e64  # Set each stand
+00019bd0: 6172 6420 6465 7669 6174 696f 6e0a 2020  ard deviation.  
+00019be0: 2020 2020 2020 2020 2020 5f73 7464 6576            _stdev
+00019bf0: 203d 2073 7464 6576 5b69 743a 2069 7420   = stdev[it: it 
+00019c00: 2b20 6e5f 7061 7273 5d0a 2020 2020 2020  + n_pars].      
+00019c10: 2020 2020 2020 6c6f 676d 6f64 656c 2e66        logmodel.f
+00019c20: 6974 5f73 7464 6576 203d 207b 0a20 2020  it_stdev = {.   
+00019c30: 2020 2020 2020 2020 2020 2020 206c 6162               lab
+00019c40: 656c 3a20 7661 6c0a 2020 2020 2020 2020  el: val.        
+00019c50: 2020 2020 2020 2020 666f 7220 6c61 6265          for labe
+00019c60: 6c2c 2076 616c 2069 6e20 7a69 7028 0a20  l, val in zip(. 
+00019c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019c80: 2020 2066 6974 5f76 6172 5f6e 616d 6573     fit_var_names
+00019c90: 2c20 5f73 7464 6576 0a20 2020 2020 2020  , _stdev.       
+00019ca0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00019cb0: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
+00019cc0: 2020 2020 2020 2320 5265 706f 7274 2073        # Report s
+00019cd0: 696e 6775 6c61 7220 7661 6c75 6573 3d30  ingular values=0
+00019ce0: 206f 6620 4a61 636f 6269 616e 0a20 2020   of Jacobian.   
+00019cf0: 2020 2020 2020 2020 2023 2061 6e64 2069           # and i
+00019d00: 6e64 6963 6174 6520 7468 6174 2073 7464  ndicate that std
+00019d10: 5f64 6576 2063 616e 6e6f 7420 6265 2063  _dev cannot be c
+00019d20: 616c 6375 6c61 7465 640a 2020 2020 2020  alculated.      
+00019d30: 2020 2020 2020 7369 6e67 7320 3d20 6e6f        sings = no
+00019d40: 5f73 7464 6576 5b69 743a 2069 7420 2b20  _stdev[it: it + 
+00019d50: 6e5f 7061 7273 5d0a 2020 2020 2020 2020  n_pars].        
+00019d60: 2020 2020 666f 7220 7061 722c 2073 6920      for par, si 
+00019d70: 696e 207a 6970 2866 6974 5f76 6172 5f6e  in zip(fit_var_n
+00019d80: 616d 6573 2c20 7369 6e67 7329 3a0a 2020  ames, sings):.  
+00019d90: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00019da0: 2076 6572 626f 7365 2061 6e64 206e 6f74   verbose and not
+00019db0: 2073 693a 0a20 2020 2020 2020 2020 2020   si:.           
+00019dc0: 2020 2020 2020 2020 2075 742e 6370 7269           ut.cpri
+00019dd0: 6e74 280a 2020 2020 2020 2020 2020 2020  nt(.            
+00019de0: 2020 2020 2020 2020 2020 2020 6627 5761              f'Wa
+00019df0: 726e 696e 673a 204a 6163 6f62 6961 6e20  rning: Jacobian 
+00019e00: 6973 2064 6567 656e 6572 6174 6520 666f  is degenerate fo
+00019e10: 7220 7b70 6172 7d2c 2073 7461 6e64 6172  r {par}, standar
+00019e20: 6420 6465 7669 6174 696f 6e20 6361 6e6e  d deviation cann
+00019e30: 6f74 2062 6520 666f 756e 642c 2061 6e64  ot be found, and
+00019e40: 2069 7320 7365 7420 746f 207a 6572 6f5c   is set to zero\
+00019e50: 6e27 2c20 2320 6e6f 7161 0a20 2020 2020  n', # noqa.     
+00019e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019e70: 2020 2027 626c 6163 6b5f 7965 6c6c 6f77     'black_yellow
+00019e80: 6267 270a 2020 2020 2020 2020 2020 2020  bg'.            
+00019e90: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00019ea0: 2020 2020 2020 2023 2053 6574 2066 696e         # Set fin
+00019eb0: 616c 2066 6974 7465 6420 7661 6c75 6573  al fitted values
+00019ec0: 0a20 2020 2020 2020 2020 2020 205f 7661  .            _va
+00019ed0: 6c73 203d 2063 7572 725f 6669 742e 785b  ls = curr_fit.x[
+00019ee0: 6974 3a20 6974 202b 206e 5f70 6172 735d  it: it + n_pars]
+00019ef0: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
+00019f00: 6d6f 6465 6c2e 6669 6e61 6c5f 7661 725f  model.final_var_
+00019f10: 7661 6c75 6573 203d 207b 0a20 2020 2020  values = {.     
+00019f20: 2020 2020 2020 2020 2020 206e 616d 653a             name:
+00019f30: 2076 616c 7565 0a20 2020 2020 2020 2020   value.         
+00019f40: 2020 2020 2020 2066 6f72 206e 616d 652c         for name,
+00019f50: 2076 616c 7565 2069 6e20 7a69 7028 6669   value in zip(fi
+00019f60: 745f 7661 725f 6e61 6d65 732c 205f 7661  t_var_names, _va
+00019f70: 6c73 290a 2020 2020 2020 2020 2020 2020  ls).            
+00019f80: 7d0a 2020 2020 2020 2020 2020 2020 2320  }.            # 
+00019f90: 616e 6420 6669 7865 6420 7661 6c75 6573  and fixed values
+00019fa0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00019fb0: 206b 6579 2c20 7661 6c20 696e 206c 6f67   key, val in log
+00019fc0: 6d6f 6465 6c2e 6669 785f 7661 7273 2e69  model.fix_vars.i
+00019fd0: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
+00019fe0: 2020 2020 2020 2020 6c6f 676d 6f64 656c          logmodel
+00019ff0: 2e66 696e 616c 5f76 6172 5f76 616c 7565  .final_var_value
+0001a000: 735b 6b65 795d 203d 2076 616c 0a0a 2020  s[key] = val..  
+0001a010: 2020 2020 2020 2020 2020 6974 202b 3d20            it += 
+0001a020: 6e5f 7061 7273 0a0a 2020 2020 2020 2020  n_pars..        
+0001a030: 7265 7475 726e 0a0a 0a63 6c61 7373 2046  return...class F
+0001a040: 6974 5769 6e64 6f77 2851 7457 6964 6765  itWindow(QtWidge
+0001a050: 7473 2e51 4d61 696e 5769 6e64 6f77 293a  ts.QMainWindow):
+0001a060: 0a20 2020 2027 2727 0a20 2020 2049 6e74  .    '''.    Int
+0001a070: 6572 6163 7469 7665 2046 6974 2057 696e  eractive Fit Win
+0001a080: 646f 7720 666f 7220 7261 7465 2076 7320  dow for rate vs 
+0001a090: 7465 6d70 6572 6174 7572 652f 6669 656c  temperature/fiel
+0001a0a0: 6420 6461 7461 2066 6974 7469 6e67 0a20  d data fitting. 
+0001a0b0: 2020 2027 2727 0a0a 2020 2020 6465 6620     '''..    def 
+0001a0c0: 5f5f 696e 6974 5f5f 2873 656c 662c 2064  __init__(self, d
+0001a0d0: 6174 6173 6574 3a20 5461 7554 4461 7461  ataset: TauTData
+0001a0e0: 7365 7420 7c20 5461 7548 4461 7461 7365  set | TauHDatase
+0001a0f0: 742c 2075 7365 6c3a 206f 626a 6563 742c  t, usel: object,
+0001a100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a110: 2020 7375 7070 6f72 7465 645f 6d6f 6465    supported_mode
+0001a120: 6c73 3a20 6c69 7374 2c0a 2020 2020 2020  ls: list,.      
+0001a130: 2020 2020 2020 2020 2020 2077 6964 6765             widge
+0001a140: 745f 6465 6661 756c 7473 3a20 6469 6374  t_defaults: dict
+0001a150: 5b73 7472 2c20 6469 6374 5b73 7472 2c20  [str, dict[str, 
+0001a160: 666c 6f61 745d 5d20 3d20 6775 692e 7769  float]] = gui.wi
+0001a170: 6467 6574 5f64 6566 6175 6c74 732c 2023  dget_defaults, #
+0001a180: 206e 6f71 610a 2020 2020 2020 2020 2020   noqa.          
+0001a190: 2020 2020 2020 202a 6172 6773 2c20 2a2a         *args, **
+0001a1a0: 6b77 6172 6773 293a 0a0a 2020 2020 2020  kwargs):..      
+0001a1b0: 2020 7375 7065 7228 4669 7457 696e 646f    super(FitWindo
+0001a1c0: 772c 2073 656c 6629 2e5f 5f69 6e69 745f  w, self).__init_
+0001a1d0: 5f28 2a61 7267 732c 202a 2a6b 7761 7267  _(*args, **kwarg
+0001a1e0: 7329 0a0a 2020 2020 2020 2020 2320 4164  s)..        # Ad
+0001a1f0: 6420 7368 6f72 7463 7574 2074 6f20 7072  d shortcut to pr
+0001a200: 6573 7320 7120 746f 2071 7569 740a 2020  ess q to quit.  
+0001a210: 2020 2020 2020 7365 6c66 2e65 7869 745f        self.exit_
+0001a220: 7368 6f72 7463 7574 203d 2051 7457 6964  shortcut = QtWid
+0001a230: 6765 7473 2e51 5368 6f72 7463 7574 2851  gets.QShortcut(Q
+0001a240: 7447 7569 2e51 4b65 7953 6571 7565 6e63  tGui.QKeySequenc
+0001a250: 6528 2771 2729 2c20 7365 6c66 290a 2020  e('q'), self).  
+0001a260: 2020 2020 2020 7365 6c66 2e65 7869 745f        self.exit_
+0001a270: 7368 6f72 7463 7574 2e61 6374 6976 6174  shortcut.activat
+0001a280: 6564 2e63 6f6e 6e65 6374 280a 2020 2020  ed.connect(.    
+0001a290: 2020 2020 2020 2020 6c61 6d62 6461 3a20          lambda: 
+0001a2a0: 7365 6c66 2e63 6c6f 7365 2829 0a20 2020  self.close().   
+0001a2b0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+0001a2c0: 7365 6c66 2e73 6574 5769 6e64 6f77 5469  self.setWindowTi
+0001a2d0: 746c 6528 2749 6e74 6572 6163 7469 7665  tle('Interactive
+0001a2e0: 2052 656c 6178 6174 696f 6e20 5072 6f66   Relaxation Prof
+0001a2f0: 696c 6527 290a 0a20 2020 2020 2020 2073  ile')..        s
+0001a300: 656c 662e 7365 7441 7474 7269 6275 7465  elf.setAttribute
+0001a310: 2851 7443 6f72 652e 5174 2e57 415f 4465  (QtCore.Qt.WA_De
+0001a320: 6c65 7465 4f6e 436c 6f73 6529 0a20 2020  leteOnClose).   
+0001a330: 2020 2020 2073 656c 662e 7365 7453 7479       self.setSty
+0001a340: 6c65 5368 6565 7428 0a20 2020 2020 2020  leSheet(.       
+0001a350: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+0001a360: 2020 2020 2051 4d61 696e 5769 6e64 6f77       QMainWindow
+0001a370: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+0001a380: 2020 2062 6163 6b67 726f 756e 642d 636f     background-co
+0001a390: 6c6f 723a 2077 6869 7465 0a20 2020 2020  lor: white.     
+0001a3a0: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
+0001a3b0: 2020 2020 2020 5143 6865 636b 426f 7820        QCheckBox 
+0001a3c0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+0001a3d0: 2020 7370 6163 696e 673a 2035 7078 3b0a    spacing: 5px;.
+0001a3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a3f0: 666f 6e74 2d73 697a 653a 3135 7078 3b0a  font-size:15px;.
+0001a400: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+0001a410: 2020 2020 2020 2020 2020 5153 6c69 6465            QSlide
+0001a420: 723a 3a67 726f 6f76 653a 686f 7269 7a6f  r::groove:horizo
+0001a430: 6e74 616c 207b 0a20 2020 2020 2020 2020  ntal {.         
+0001a440: 2020 2062 6f72 6465 723a 2031 7078 2073     border: 1px s
+0001a450: 6f6c 6964 2023 6262 623b 0a20 2020 2020  olid #bbb;.     
+0001a460: 2020 2020 2020 2062 6163 6b67 726f 756e         backgroun
+0001a470: 643a 2077 6869 7465 3b0a 2020 2020 2020  d: white;.      
+0001a480: 2020 2020 2020 6865 6967 6874 3a20 3130        height: 10
+0001a490: 7078 3b0a 2020 2020 2020 2020 2020 2020  px;.            
+0001a4a0: 626f 7264 6572 2d72 6164 6975 733a 2034  border-radius: 4
+0001a4b0: 7078 3b0a 2020 2020 2020 2020 2020 2020  px;.            
+0001a4c0: 7d0a 0a20 2020 2020 2020 2020 2020 2051  }..            Q
+0001a4d0: 536c 6964 6572 3a3a 7375 622d 7061 6765  Slider::sub-page
+0001a4e0: 3a68 6f72 697a 6f6e 7461 6c20 7b0a 2020  :horizontal {.  
+0001a4f0: 2020 2020 2020 2020 2020 6261 636b 6772            backgr
+0001a500: 6f75 6e64 3a20 716c 696e 6561 7267 7261  ound: qlineargra
+0001a510: 6469 656e 7428 7831 3a20 302c 2079 313a  dient(x1: 0, y1:
+0001a520: 2030 2c20 2020 2078 323a 2030 2c20 7932   0,    x2: 0, y2
+0001a530: 3a20 312c 0a20 2020 2020 2020 2020 2020  : 1,.           
+0001a540: 2020 2020 2073 746f 703a 2030 2023 3636       stop: 0 #66
+0001a550: 652c 2073 746f 703a 2031 2023 6262 6629  e, stop: 1 #bbf)
+0001a560: 3b0a 2020 2020 2020 2020 2020 2020 6261  ;.            ba
+0001a570: 636b 6772 6f75 6e64 3a20 716c 696e 6561  ckground: qlinea
+0001a580: 7267 7261 6469 656e 7428 7831 3a20 302c  rgradient(x1: 0,
+0001a590: 2079 313a 2030 2e32 2c20 7832 3a20 312c   y1: 0.2, x2: 1,
+0001a5a0: 2079 323a 2031 2c0a 2020 2020 2020 2020   y2: 1,.        
+0001a5b0: 2020 2020 2020 2020 7374 6f70 3a20 3020          stop: 0 
+0001a5c0: 2362 6266 2c20 7374 6f70 3a20 3120 2335  #bbf, stop: 1 #5
+0001a5d0: 3566 293b 0a20 2020 2020 2020 2020 2020  5f);.           
+0001a5e0: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
+0001a5f0: 6964 2023 3737 373b 0a20 2020 2020 2020  id #777;.       
+0001a600: 2020 2020 2068 6569 6768 743a 2031 3070       height: 10p
+0001a610: 783b 0a20 2020 2020 2020 2020 2020 2062  x;.            b
+0001a620: 6f72 6465 722d 7261 6469 7573 3a20 3470  order-radius: 4p
+0001a630: 783b 0a20 2020 2020 2020 2020 2020 207d  x;.            }
+0001a640: 0a0a 2020 2020 2020 2020 2020 2020 5153  ..            QS
+0001a650: 6c69 6465 723a 3a61 6464 2d70 6167 653a  lider::add-page:
+0001a660: 686f 7269 7a6f 6e74 616c 207b 0a20 2020  horizontal {.   
+0001a670: 2020 2020 2020 2020 2062 6163 6b67 726f           backgro
+0001a680: 756e 643a 2023 6666 663b 0a20 2020 2020  und: #fff;.     
+0001a690: 2020 2020 2020 2062 6f72 6465 723a 2031         border: 1
+0001a6a0: 7078 2073 6f6c 6964 2023 3737 373b 0a20  px solid #777;. 
+0001a6b0: 2020 2020 2020 2020 2020 2068 6569 6768             heigh
+0001a6c0: 743a 2031 3070 783b 0a20 2020 2020 2020  t: 10px;.       
+0001a6d0: 2020 2020 2062 6f72 6465 722d 7261 6469       border-radi
+0001a6e0: 7573 3a20 3470 783b 0a20 2020 2020 2020  us: 4px;.       
+0001a6f0: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
+0001a700: 2020 2020 5153 6c69 6465 723a 3a68 616e      QSlider::han
+0001a710: 646c 653a 686f 7269 7a6f 6e74 616c 207b  dle:horizontal {
+0001a720: 0a20 2020 2020 2020 2020 2020 2062 6163  .            bac
+0001a730: 6b67 726f 756e 643a 2071 6c69 6e65 6172  kground: qlinear
+0001a740: 6772 6164 6965 6e74 2878 313a 302c 2079  gradient(x1:0, y
+0001a750: 313a 302c 2078 323a 312c 2079 323a 312c  1:0, x2:1, y2:1,
+0001a760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a770: 2073 746f 703a 3020 2365 6565 2c20 7374   stop:0 #eee, st
+0001a780: 6f70 3a31 2023 6363 6329 3b0a 2020 2020  op:1 #ccc);.    
+0001a790: 2020 2020 2020 2020 626f 7264 6572 3a20          border: 
+0001a7a0: 3170 7820 736f 6c69 6420 2337 3737 3b0a  1px solid #777;.
+0001a7b0: 2020 2020 2020 2020 2020 2020 7769 6474              widt
+0001a7c0: 683a 2031 3370 783b 0a20 2020 2020 2020  h: 13px;.       
+0001a7d0: 2020 2020 206d 6172 6769 6e2d 746f 703a       margin-top:
+0001a7e0: 202d 3270 783b 0a20 2020 2020 2020 2020   -2px;.         
+0001a7f0: 2020 206d 6172 6769 6e2d 626f 7474 6f6d     margin-bottom
+0001a800: 3a20 2d32 7078 3b0a 2020 2020 2020 2020  : -2px;.        
+0001a810: 2020 2020 626f 7264 6572 2d72 6164 6975      border-radiu
+0001a820: 733a 2034 7078 3b0a 2020 2020 2020 2020  s: 4px;.        
+0001a830: 2020 2020 7d0a 0a20 2020 2020 2020 2020      }..         
+0001a840: 2020 2051 536c 6964 6572 3a3a 6861 6e64     QSlider::hand
+0001a850: 6c65 3a68 6f72 697a 6f6e 7461 6c3a 686f  le:horizontal:ho
+0001a860: 7665 7220 7b0a 2020 2020 2020 2020 2020  ver {.          
+0001a870: 2020 6261 636b 6772 6f75 6e64 3a20 716c    background: ql
+0001a880: 696e 6561 7267 7261 6469 656e 7428 7831  ineargradient(x1
+0001a890: 3a30 2c20 7931 3a30 2c20 7832 3a31 2c20  :0, y1:0, x2:1, 
+0001a8a0: 7932 3a31 2c0a 2020 2020 2020 2020 2020  y2:1,.          
+0001a8b0: 2020 2020 2020 7374 6f70 3a30 2023 6666        stop:0 #ff
+0001a8c0: 662c 2073 746f 703a 3120 2364 6464 293b  f, stop:1 #ddd);
+0001a8d0: 0a20 2020 2020 2020 2020 2020 2062 6f72  .            bor
+0001a8e0: 6465 723a 2031 7078 2073 6f6c 6964 2023  der: 1px solid #
+0001a8f0: 3434 343b 0a20 2020 2020 2020 2020 2020  444;.           
+0001a900: 2062 6f72 6465 722d 7261 6469 7573 3a20   border-radius: 
+0001a910: 3470 783b 0a20 2020 2020 2020 2020 2020  4px;.           
+0001a920: 207d 0a0a 2020 2020 2020 2020 2020 2020   }..            
+0001a930: 5153 6c69 6465 723a 3a73 7562 2d70 6167  QSlider::sub-pag
+0001a940: 653a 686f 7269 7a6f 6e74 616c 3a64 6973  e:horizontal:dis
+0001a950: 6162 6c65 6420 7b0a 2020 2020 2020 2020  abled {.        
+0001a960: 2020 2020 6261 636b 6772 6f75 6e64 3a20      background: 
+0001a970: 2362 6262 3b0a 2020 2020 2020 2020 2020  #bbb;.          
+0001a980: 2020 626f 7264 6572 2d63 6f6c 6f72 3a20    border-color: 
+0001a990: 2339 3939 3b0a 2020 2020 2020 2020 2020  #999;.          
+0001a9a0: 2020 7d0a 0a20 2020 2020 2020 2020 2020    }..           
+0001a9b0: 2051 536c 6964 6572 3a3a 6164 642d 7061   QSlider::add-pa
+0001a9c0: 6765 3a68 6f72 697a 6f6e 7461 6c3a 6469  ge:horizontal:di
+0001a9d0: 7361 626c 6564 207b 0a20 2020 2020 2020  sabled {.       
+0001a9e0: 2020 2020 2062 6163 6b67 726f 756e 643a       background:
+0001a9f0: 2023 6565 653b 0a20 2020 2020 2020 2020   #eee;.         
+0001aa00: 2020 2062 6f72 6465 722d 636f 6c6f 723a     border-color:
+0001aa10: 2023 3939 393b 0a20 2020 2020 2020 2020   #999;.         
+0001aa20: 2020 207d 0a0a 2020 2020 2020 2020 2020     }..          
+0001aa30: 2020 5153 6c69 6465 723a 3a68 616e 646c    QSlider::handl
+0001aa40: 653a 686f 7269 7a6f 6e74 616c 3a64 6973  e:horizontal:dis
+0001aa50: 6162 6c65 6420 7b0a 2020 2020 2020 2020  abled {.        
+0001aa60: 2020 2020 6261 636b 6772 6f75 6e64 3a20      background: 
+0001aa70: 2365 6565 3b0a 2020 2020 2020 2020 2020  #eee;.          
+0001aa80: 2020 626f 7264 6572 3a20 3170 7820 736f    border: 1px so
+0001aa90: 6c69 6420 2361 6161 3b0a 2020 2020 2020  lid #aaa;.      
+0001aaa0: 2020 2020 2020 626f 7264 6572 2d72 6164        border-rad
+0001aab0: 6975 733a 2034 7078 3b0a 2020 2020 2020  ius: 4px;.      
+0001aac0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+0001aad0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+0001aae0: 290a 0a20 2020 2020 2020 2023 2053 6574  )..        # Set
+0001aaf0: 2064 6566 6175 6c74 206d 696e 2c20 6d61   default min, ma
+0001ab00: 782c 2069 6e69 742c 2061 6e64 2073 7465  x, init, and ste
+0001ab10: 7020 7661 6c75 6573 206f 6620 736c 6964  p values of slid
+0001ab20: 6572 7320 616e 6420 7465 7874 2062 6f78  ers and text box
+0001ab30: 6573 0a20 2020 2020 2020 2073 656c 662e  es.        self.
+0001ab40: 6465 6661 756c 7473 203d 2077 6964 6765  defaults = widge
+0001ab50: 745f 6465 6661 756c 7473 0a0a 2020 2020  t_defaults..    
+0001ab60: 2020 2020 2320 4469 6374 696f 6e61 7279      # Dictionary
+0001ab70: 2066 6f72 2074 6963 6b62 6f78 2077 6964   for tickbox wid
+0001ab80: 6765 7473 0a20 2020 2020 2020 2073 656c  gets.        sel
+0001ab90: 662e 7469 636b 6469 6374 203d 207b 0a20  f.tickdict = {. 
+0001aba0: 2020 2020 2020 2020 2020 206d 6f64 656c             model
+0001abb0: 2e4e 414d 452e 6c6f 7765 7228 293a 204e  .NAME.lower(): N
+0001abc0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+0001abd0: 666f 7220 6d6f 6465 6c20 696e 2073 7570  for model in sup
+0001abe0: 706f 7274 6564 5f6d 6f64 656c 730a 2020  ported_models.  
+0001abf0: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
+0001ac00: 2023 2044 6963 7469 6f6e 6172 7920 666f   # Dictionary fo
+0001ac10: 7220 7061 7261 6d65 7465 7220 736c 6964  r parameter slid
+0001ac20: 6572 2c20 656e 7472 792c 2061 6e64 2066  er, entry, and f
+0001ac30: 6974 6669 7820 7769 6467 6574 730a 2020  itfix widgets.  
+0001ac40: 2020 2020 2020 7365 6c66 2e77 6964 6765        self.widge
+0001ac50: 7464 6963 7420 3d20 7b0a 2020 2020 2020  tdict = {.      
+0001ac60: 2020 2020 2020 6d6f 6465 6c2e 4e41 4d45        model.NAME
+0001ac70: 2e6c 6f77 6572 2829 3a20 7b0a 2020 2020  .lower(): {.    
+0001ac80: 2020 2020 2020 2020 2020 2020 7061 726e              parn
+0001ac90: 616d 653a 207b 0a20 2020 2020 2020 2020  ame: {.         
+0001aca0: 2020 2020 2020 2020 2020 2027 736c 6964             'slid
+0001acb0: 6572 273a 204e 6f6e 652c 0a20 2020 2020  er': None,.     
+0001acc0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0001acd0: 6666 5f74 6f67 676c 6527 3a20 4e6f 6e65  ff_toggle': None
+0001ace0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001acf0: 2020 2020 2020 2765 6e74 7279 273a 204e        'entry': N
+0001ad00: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+0001ad10: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
+0001ad20: 2020 2020 2020 666f 7220 7061 726e 616d        for parnam
+0001ad30: 6520 696e 206d 6f64 656c 2e50 4152 4e41  e in model.PARNA
+0001ad40: 4d45 530a 2020 2020 2020 2020 2020 2020  MES.            
+0001ad50: 7d0a 2020 2020 2020 2020 2020 2020 666f  }.            fo
+0001ad60: 7220 6d6f 6465 6c20 696e 2073 7570 706f  r model in suppo
+0001ad70: 7274 6564 5f6d 6f64 656c 730a 2020 2020  rted_models.    
+0001ad80: 2020 2020 7d0a 0a20 2020 2020 2020 2023      }..        #
+0001ad90: 204d 696e 696d 756d 2057 696e 646f 7720   Minimum Window 
+0001ada0: 7369 7a65 0a20 2020 2020 2020 2073 656c  size.        sel
+0001adb0: 662e 7365 744d 696e 696d 756d 5369 7a65  f.setMinimumSize
+0001adc0: 2851 7443 6f72 652e 5153 697a 6528 3132  (QtCore.QSize(12
+0001add0: 3030 2c20 3730 3029 290a 0a20 2020 2020  00, 700))..     
+0001ade0: 2020 2023 204d 616b 6520 7769 6467 6574     # Make widget
+0001adf0: 7320 666f 7220 656e 7469 7265 2077 696e  s for entire win
+0001ae00: 646f 770a 2020 2020 2020 2020 7365 6c66  dow.        self
+0001ae10: 2e77 6964 6765 7420 3d20 5174 5769 6467  .widget = QtWidg
+0001ae20: 6574 732e 5157 6964 6765 7428 7061 7265  ets.QWidget(pare
+0001ae30: 6e74 3d73 656c 6629 0a20 2020 2020 2020  nt=self).       
+0001ae40: 2073 656c 662e 7365 7443 656e 7472 616c   self.setCentral
+0001ae50: 5769 6467 6574 2873 656c 662e 7769 6467  Widget(self.widg
+0001ae60: 6574 290a 2020 2020 2020 2020 626f 745f  et).        bot_
+0001ae70: 726f 775f 7769 6467 6574 203d 2051 7457  row_widget = QtW
+0001ae80: 6964 6765 7473 2e51 5769 6467 6574 2873  idgets.QWidget(s
+0001ae90: 656c 662e 7769 6467 6574 290a 2020 2020  elf.widget).    
+0001aea0: 2020 2020 746f 705f 726f 775f 7769 6467      top_row_widg
+0001aeb0: 6574 203d 2051 7457 6964 6765 7473 2e51  et = QtWidgets.Q
+0001aec0: 5769 6467 6574 2873 656c 662e 7769 6467  Widget(self.widg
+0001aed0: 6574 290a 2020 2020 2020 2020 7268 735f  et).        rhs_
+0001aee0: 636f 6c5f 7769 6467 6574 203d 2051 7457  col_widget = QtW
+0001aef0: 6964 6765 7473 2e51 5769 6467 6574 2874  idgets.QWidget(t
+0001af00: 6f70 5f72 6f77 5f77 6964 6765 7429 0a0a  op_row_widget)..
+0001af10: 2020 2020 2020 2020 7268 735f 636f 6c5f          rhs_col_
+0001af20: 7363 726f 6c6c 203d 2051 7457 6964 6765  scroll = QtWidge
+0001af30: 7473 2e51 5363 726f 6c6c 4172 6561 2872  ts.QScrollArea(r
+0001af40: 6873 5f63 6f6c 5f77 6964 6765 7429 0a20  hs_col_widget). 
+0001af50: 2020 2020 2020 2072 6873 5f63 6f6c 5f73         rhs_col_s
+0001af60: 6372 6f6c 6c2e 7365 7456 6572 7469 6361  croll.setVertica
+0001af70: 6c53 6372 6f6c 6c42 6172 506f 6c69 6379  lScrollBarPolicy
+0001af80: 280a 2020 2020 2020 2020 2020 2020 5174  (.            Qt
+0001af90: 436f 7265 2e51 742e 5363 726f 6c6c 4261  Core.Qt.ScrollBa
+0001afa0: 7241 6c77 6179 734f 6e0a 2020 2020 2020  rAlwaysOn.      
+0001afb0: 2020 290a 2020 2020 2020 2020 7268 735f    ).        rhs_
+0001afc0: 636f 6c5f 7363 726f 6c6c 2e73 6574 486f  col_scroll.setHo
+0001afd0: 7269 7a6f 6e74 616c 5363 726f 6c6c 4261  rizontalScrollBa
+0001afe0: 7250 6f6c 6963 7928 0a20 2020 2020 2020  rPolicy(.       
+0001aff0: 2020 2020 2051 7443 6f72 652e 5174 2e53       QtCore.Qt.S
+0001b000: 6372 6f6c 6c42 6172 416c 7761 7973 4f66  crollBarAlwaysOf
+0001b010: 660a 2020 2020 2020 2020 290a 2020 2020  f.        ).    
+0001b020: 2020 2020 7268 735f 636f 6c5f 7363 726f      rhs_col_scro
+0001b030: 6c6c 2e73 6574 5769 6467 6574 5265 7369  ll.setWidgetResi
+0001b040: 7a61 626c 6528 5472 7565 290a 0a20 2020  zable(True)..   
+0001b050: 2020 2020 2073 6372 6f6c 6c5f 636f 6e74       scroll_cont
+0001b060: 6169 6e65 7220 3d20 5174 5769 6467 6574  ainer = QtWidget
+0001b070: 732e 5157 6964 6765 7428 7268 735f 636f  s.QWidget(rhs_co
+0001b080: 6c5f 7363 726f 6c6c 290a 2020 2020 2020  l_scroll).      
+0001b090: 2020 7268 735f 636f 6c5f 7363 726f 6c6c    rhs_col_scroll
+0001b0a0: 2e73 6574 5769 6467 6574 2873 6372 6f6c  .setWidget(scrol
+0001b0b0: 6c5f 636f 6e74 6169 6e65 7229 0a0a 2020  l_container)..  
+0001b0c0: 2020 2020 2020 6c68 735f 636f 6c5f 7769        lhs_col_wi
+0001b0d0: 6467 6574 203d 2051 7457 6964 6765 7473  dget = QtWidgets
+0001b0e0: 2e51 5769 6467 6574 2874 6f70 5f72 6f77  .QWidget(top_row
+0001b0f0: 5f77 6964 6765 7429 0a0a 2020 2020 2020  _widget)..      
+0001b100: 2020 2320 4c48 5320 636f 6c75 6d6e 202d    # LHS column -
+0001b110: 2070 6c6f 7420 6f6e 6c79 0a20 2020 2020   plot only.     
+0001b120: 2020 206c 6873 5f63 6f6c 5f6c 6179 6f75     lhs_col_layou
+0001b130: 7420 3d20 5174 5769 6467 6574 732e 5156  t = QtWidgets.QV
+0001b140: 426f 784c 6179 6f75 7428 6c68 735f 636f  BoxLayout(lhs_co
+0001b150: 6c5f 7769 6467 6574 290a 0a20 2020 2020  l_widget)..     
+0001b160: 2020 2023 206d 616b 6520 7067 6670 6c6f     # make pgfplo
+0001b170: 7473 2070 6c6f 7420 7769 6467 6574 0a20  ts plot widget. 
+0001b180: 2020 2020 2020 2073 656c 662e 706c 6f74         self.plot
+0001b190: 5f77 6964 6765 7420 3d20 7067 2e50 6c6f  _widget = pg.Plo
+0001b1a0: 7457 6964 6765 7428 0a20 2020 2020 2020  tWidget(.       
+0001b1b0: 2020 2020 2070 6172 656e 743d 6c68 735f       parent=lhs_
+0001b1c0: 636f 6c5f 7769 6467 6574 0a20 2020 2020  col_widget.     
+0001b1d0: 2020 2029 0a20 2020 2020 2020 2023 2041     ).        # A
+0001b1e0: 6464 2070 6c6f 7420 746f 206c 6566 7420  dd plot to left 
+0001b1f0: 636f 6c75 6d6e 0a20 2020 2020 2020 206c  column.        l
+0001b200: 6873 5f63 6f6c 5f6c 6179 6f75 742e 6164  hs_col_layout.ad
+0001b210: 6457 6964 6765 7428 7365 6c66 2e70 6c6f  dWidget(self.plo
+0001b220: 745f 7769 6467 6574 290a 0a20 2020 2020  t_widget)..     
+0001b230: 2020 2023 2053 6574 206c 6f67 6c6f 6720     # Set loglog 
+0001b240: 6178 6573 0a20 2020 2020 2020 2073 656c  axes.        sel
+0001b250: 662e 706c 6f74 5f77 6964 6765 742e 7365  f.plot_widget.se
+0001b260: 744c 6f67 4d6f 6465 2854 7275 652c 2054  tLogMode(True, T
+0001b270: 7275 6529 0a0a 2020 2020 2020 2020 2320  rue)..        # 
+0001b280: 5365 7420 7768 6974 6520 706c 6f74 2062  Set white plot b
+0001b290: 6163 6b67 726f 756e 640a 2020 2020 2020  ackground.      
+0001b2a0: 2020 7365 6c66 2e70 6c6f 745f 7769 6467    self.plot_widg
+0001b2b0: 6574 2e73 6574 4261 636b 6772 6f75 6e64  et.setBackground
+0001b2c0: 2827 7727 290a 0a20 2020 2020 2020 2023  ('w')..        #
+0001b2d0: 2053 656c 6563 7420 6569 7468 6572 2066   Select either f
+0001b2e0: 6965 6c64 206f 7220 7465 6d70 6572 6174  ield or temperat
+0001b2f0: 7572 6520 6173 2078 2064 6174 6120 6261  ure as x data ba
+0001b300: 7365 6420 6f6e 2064 6174 6173 6574 2074  sed on dataset t
+0001b310: 7970 650a 2020 2020 2020 2020 2320 616e  ype.        # an
+0001b320: 6420 7365 7420 7820 6c61 6265 6c20 6f66  d set x label of
+0001b330: 2070 6c6f 740a 2020 2020 2020 2020 6966   plot.        if
+0001b340: 2069 7369 6e73 7461 6e63 6528 6461 7461   isinstance(data
+0001b350: 7365 742c 2054 6175 4844 6174 6173 6574  set, TauHDataset
+0001b360: 293a 0a20 2020 2020 2020 2020 2020 2078  ):.            x
+0001b370: 5f76 616c 7320 3d20 636f 7079 2e63 6f70  _vals = copy.cop
+0001b380: 7928 6461 7461 7365 742e 6669 656c 6473  y(dataset.fields
+0001b390: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
+0001b3a0: 5368 6966 7420 616c 6c20 6461 7461 2074  Shift all data t
+0001b3b0: 6f20 6265 636f 6d65 2064 6566 696e 6564  o become defined
+0001b3c0: 2069 6e20 6c6f 6731 3020 7370 6163 650a   in log10 space.
+0001b3d0: 2020 2020 2020 2020 2020 2020 2320 5468              # Th
+0001b3e0: 6973 2073 6869 6674 206d 7573 7420 6f6e  is shift must on
+0001b3f0: 6c79 2062 6520 6170 706c 6965 6420 7768  ly be applied wh
+0001b400: 656e 2070 6c6f 7474 696e 672c 206e 6f74  en plotting, not
+0001b410: 0a20 2020 2020 2020 2020 2020 2023 2077  .            # w
+0001b420: 6865 6e20 6361 6c63 756c 6174 696e 6720  hen calculating 
+0001b430: 7468 6520 7661 6c75 6573 206f 6620 7468  the values of th
+0001b440: 6520 6675 6e63 7469 6f6e 0a20 2020 2020  e function.     
+0001b450: 2020 2020 2020 2069 6620 616e 7928 7661         if any(va
+0001b460: 6c20 3c20 6e70 2e66 696e 666f 2866 6c6f  l < np.finfo(flo
+0001b470: 6174 292e 6570 7320 666f 7220 7661 6c20  at).eps for val 
+0001b480: 696e 2078 5f76 616c 7329 3a0a 2020 2020  in x_vals):.    
+0001b490: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001b4a0: 2e6c 6f67 7368 6966 7420 3d20 312e 0a20  .logshift = 1.. 
+0001b4b0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0001b4c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b4d0: 2073 656c 662e 6c6f 6773 6869 6674 203d   self.logshift =
+0001b4e0: 2030 2e0a 2020 2020 2020 2020 2020 2020   0..            
+0001b4f0: 785f 7661 6c73 202b 3d20 7365 6c66 2e6c  x_vals += self.l
+0001b500: 6f67 7368 6966 740a 2020 2020 2020 2020  ogshift.        
+0001b510: 2020 2020 7365 6c66 2e70 6c6f 745f 7769      self.plot_wi
+0001b520: 6467 6574 2e73 6574 4c61 6265 6c28 2762  dget.setLabel('b
+0001b530: 6f74 746f 6d27 2c20 2746 6965 6c64 2028  ottom', 'Field (
+0001b540: 4f65 2927 290a 0a20 2020 2020 2020 2065  Oe)')..        e
+0001b550: 6c69 6620 6973 696e 7374 616e 6365 2864  lif isinstance(d
+0001b560: 6174 6173 6574 2c20 5461 7554 4461 7461  ataset, TauTData
+0001b570: 7365 7429 3a0a 2020 2020 2020 2020 2020  set):.          
+0001b580: 2020 7365 6c66 2e6c 6f67 7368 6966 7420    self.logshift 
+0001b590: 3d20 302e 0a20 2020 2020 2020 2020 2020  = 0..           
+0001b5a0: 2078 5f76 616c 7320 3d20 636f 7079 2e63   x_vals = copy.c
+0001b5b0: 6f70 7928 6461 7461 7365 742e 7465 6d70  opy(dataset.temp
+0001b5c0: 6572 6174 7572 6573 290a 2020 2020 2020  eratures).      
+0001b5d0: 2020 2020 2020 7365 6c66 2e70 6c6f 745f        self.plot_
+0001b5e0: 7769 6467 6574 2e73 6574 4c61 6265 6c28  widget.setLabel(
+0001b5f0: 2762 6f74 746f 6d27 2c20 2754 656d 7065  'bottom', 'Tempe
+0001b600: 7261 7475 7265 2028 4b29 2729 0a0a 2020  rature (K)')..  
+0001b610: 2020 2020 2020 2320 4578 7065 7269 6d65        # Experime
+0001b620: 6e74 616c 2064 6174 610a 2020 2020 2020  ntal data.      
+0001b630: 2020 7365 6c66 2e65 7870 203d 2073 656c    self.exp = sel
+0001b640: 662e 706c 6f74 5f77 6964 6765 742e 706c  f.plot_widget.pl
+0001b650: 6f74 280a 2020 2020 2020 2020 2020 2020  ot(.            
+0001b660: 6e70 2e61 7272 6179 2878 5f76 616c 7329  np.array(x_vals)
+0001b670: 2c0a 2020 2020 2020 2020 2020 2020 6e70  ,.            np
+0001b680: 2e61 7272 6179 2864 6174 6173 6574 2e72  .array(dataset.r
+0001b690: 6174 6573 292c 0a20 2020 2020 2020 2020  ates),.         
+0001b6a0: 2020 2070 656e 3d4e 6f6e 652c 0a20 2020     pen=None,.   
+0001b6b0: 2020 2020 2020 2020 2073 796d 626f 6c3d           symbol=
+0001b6c0: 2778 272c 0a20 2020 2020 2020 2020 2020  'x',.           
+0001b6d0: 2073 796d 626f 6c42 7275 7368 3d28 302c   symbolBrush=(0,
+0001b6e0: 2030 2c20 3029 0a20 2020 2020 2020 2029   0, 0).        )
+0001b6f0: 0a0a 2020 2020 2020 2020 2320 4669 6e64  ..        # Find
+0001b700: 206e 6963 6520 792d 6178 6973 206c 696d   nice y-axis lim
+0001b710: 6974 730a 2020 2020 2020 2020 795f 6c6f  its.        y_lo
+0001b720: 7765 722c 2079 5f75 7070 6572 203d 2067  wer, y_upper = g
+0001b730: 7569 2e63 616c 635f 795f 7261 7465 5f6c  ui.calc_y_rate_l
+0001b740: 696d 7328 0a20 2020 2020 2020 2020 2020  ims(.           
+0001b750: 2064 6174 6173 6574 2e72 6174 6573 2c0a   dataset.rates,.
+0001b760: 2020 2020 2020 2020 2020 2020 6e70 2e61              np.a
+0001b770: 7272 6179 2864 6174 6173 6574 2e72 6174  rray(dataset.rat
+0001b780: 655f 706d 290a 2020 2020 2020 2020 290a  e_pm).        ).
+0001b790: 0a20 2020 2020 2020 2023 2043 6c69 7020  .        # Clip 
+0001b7a0: 7468 656d 2061 7420 7365 6e73 6962 6c65  them at sensible
+0001b7b0: 2076 616c 7565 730a 2020 2020 2020 2020   values.        
+0001b7c0: 5b79 5f6c 6f77 6572 2c20 795f 7570 7065  [y_lower, y_uppe
+0001b7d0: 725d 203d 206e 702e 636c 6970 285b 795f  r] = np.clip([y_
+0001b7e0: 6c6f 7765 722c 2079 5f75 7070 6572 5d2c  lower, y_upper],
+0001b7f0: 2031 452d 3130 2c20 3145 3130 290a 0a20   1E-10, 1E10).. 
+0001b800: 2020 2020 2020 2023 2061 6e64 2073 6574         # and set
+0001b810: 2076 616c 7565 730a 2020 2020 2020 2020   values.        
+0001b820: 7365 6c66 2e70 6c6f 745f 7769 6467 6574  self.plot_widget
+0001b830: 2e73 6574 5952 616e 6765 280a 2020 2020  .setYRange(.    
+0001b840: 2020 2020 2020 2020 6e70 2e6c 6f67 3130          np.log10
+0001b850: 2879 5f6c 6f77 6572 292c 0a20 2020 2020  (y_lower),.     
+0001b860: 2020 2020 2020 206e 702e 6c6f 6731 3028         np.log10(
+0001b870: 795f 7570 7065 7229 2c0a 2020 2020 2020  y_upper),.      
+0001b880: 2020 2020 2020 7061 6464 696e 673d 300a        padding=0.
+0001b890: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0001b8a0: 2020 2023 2041 6464 2065 7870 6572 696d     # Add experim
+0001b8b0: 656e 7461 6c20 6572 726f 7262 6172 730a  ental errorbars.
+0001b8c0: 2020 2020 2020 2020 6966 206c 656e 2864          if len(d
+0001b8d0: 6174 6173 6574 2e6c 6f67 7261 7465 5f70  ataset.lograte_p
+0001b8e0: 6d29 3a0a 2020 2020 2020 2020 2020 2020  m):.            
+0001b8f0: 6572 7220 3d20 7067 2e45 7272 6f72 4261  err = pg.ErrorBa
+0001b900: 7249 7465 6d28 0a20 2020 2020 2020 2020  rItem(.         
+0001b910: 2020 2020 2020 2078 3d6e 702e 6c6f 6731         x=np.log1
+0001b920: 3028 785f 7661 6c73 292c 0a20 2020 2020  0(x_vals),.     
+0001b930: 2020 2020 2020 2020 2020 2079 3d6e 702e             y=np.
+0001b940: 6c6f 6731 3028 6461 7461 7365 742e 7261  log10(dataset.ra
+0001b950: 7465 7329 2c0a 2020 2020 2020 2020 2020  tes),.          
+0001b960: 2020 2020 2020 746f 703d 6461 7461 7365        top=datase
+0001b970: 742e 6c6f 6772 6174 655f 706d 2c0a 2020  t.lograte_pm,.  
+0001b980: 2020 2020 2020 2020 2020 2020 2020 626f                bo
+0001b990: 7474 6f6d 3d64 6174 6173 6574 2e6c 6f67  ttom=dataset.log
+0001b9a0: 7261 7465 5f70 6d2c 0a20 2020 2020 2020  rate_pm,.       
+0001b9b0: 2020 2020 2020 2020 2062 6561 6d3d 302e           beam=0.
+0001b9c0: 3030 350a 2020 2020 2020 2020 2020 2020  005.            
+0001b9d0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+0001b9e0: 6c66 2e70 6c6f 745f 7769 6467 6574 2e61  lf.plot_widget.a
+0001b9f0: 6464 4974 656d 2865 7272 290a 0a20 2020  ddItem(err)..   
+0001ba00: 2020 2020 2023 2041 7869 7320 6c61 6265       # Axis labe
+0001ba10: 6c73 0a20 2020 2020 2020 2073 656c 662e  ls.        self.
+0001ba20: 706c 6f74 5f77 6964 6765 742e 7365 744c  plot_widget.setL
+0001ba30: 6162 656c 2827 6c65 6674 272c 2027 5261  abel('left', 'Ra
+0001ba40: 7465 2028 733c 7375 703e 2d31 3c2f 7375  te (s<sup>-1</su
+0001ba50: 703e 2927 290a 0a20 2020 2020 2020 2023  p>)')..        #
+0001ba60: 2053 6574 2064 6963 7469 6f6e 6172 7920   Set dictionary 
+0001ba70: 6f66 2054 7275 6520 2866 6974 2920 616e  of True (fit) an
+0001ba80: 6420 4661 6c73 6520 2866 6978 2920 666f  d False (fix) fo
+0001ba90: 7220 6561 6368 0a20 2020 2020 2020 2023  r each.        #
+0001baa0: 2070 6172 616d 6574 6572 206f 6620 616c   parameter of al
+0001bab0: 6c20 6176 6169 6c61 626c 6520 6d6f 6465  l available mode
+0001bac0: 6c73 0a20 2020 2020 2020 2075 7365 6c2e  ls.        usel.
+0001bad0: 6669 7420 3d20 7b0a 2020 2020 2020 2020  fit = {.        
+0001bae0: 2020 2020 7061 726e 616d 653a 2054 7275      parname: Tru
+0001baf0: 650a 2020 2020 2020 2020 2020 2020 666f  e.            fo
+0001bb00: 7220 6d6f 6465 6c20 696e 2073 7570 706f  r model in suppo
+0001bb10: 7274 6564 5f6d 6f64 656c 730a 2020 2020  rted_models.    
+0001bb20: 2020 2020 2020 2020 666f 7220 7061 726e          for parn
+0001bb30: 616d 6520 696e 206d 6f64 656c 2e50 4152  ame in model.PAR
+0001bb40: 4e41 4d45 530a 2020 2020 2020 2020 7d0a  NAMES.        }.
+0001bb50: 0a20 2020 2020 2020 2023 2053 6574 2075  .        # Set u
+0001bb60: 7365 7220 7365 6c65 6374 696f 6e20 6f62  ser selection ob
+0001bb70: 6a65 6374 2061 6e64 2073 7570 706f 7274  ject and support
+0001bb80: 6564 206d 6f64 656c 730a 2020 2020 2020  ed models.      
+0001bb90: 2020 7365 6c66 2e75 7365 6c20 3d20 7573    self.usel = us
+0001bba0: 656c 0a20 2020 2020 2020 2073 656c 662e  el.        self.
+0001bbb0: 7375 7070 6f72 7465 645f 6d6f 6465 6c73  supported_models
+0001bbc0: 203d 2073 7570 706f 7274 6564 5f6d 6f64   = supported_mod
+0001bbd0: 656c 730a 0a20 2020 2020 2020 2023 2043  els..        # C
+0001bbe0: 616c 6375 6c61 7465 2065 6163 6820 6d6f  alculate each mo
+0001bbf0: 6465 6c20 6675 6e63 7469 6f6e 2061 6e64  del function and
+0001bc00: 2070 6c6f 740a 2020 2020 2020 2020 2320   plot.        # 
+0001bc10: 4e6f 7465 2069 6620 7368 6966 7420 6973  Note if shift is
+0001bc20: 2061 7070 6c69 6564 2074 6865 6e20 7468   applied then th
+0001bc30: 6573 6520 7661 6c75 6573 0a20 2020 2020  ese values.     
+0001bc40: 2020 2023 206d 7573 7420 6265 2074 6865     # must be the
+0001bc50: 2074 7275 6520 7820 7661 7269 6162 6c65   true x variable
+0001bc60: 7320 6173 2074 6865 7920 7769 6c6c 2062  s as they will b
+0001bc70: 6520 7573 6564 2074 6f20 636f 6d70 7574  e used to comput
+0001bc80: 650a 2020 2020 2020 2020 2320 7468 6520  e.        # the 
+0001bc90: 6d6f 6465 6c20 7661 6c75 6573 0a20 2020  model values.   
+0001bca0: 2020 2020 2073 656c 662e 785f 6772 6964       self.x_grid
+0001bcb0: 203d 206e 702e 6c69 6e73 7061 6365 280a   = np.linspace(.
+0001bcc0: 2020 2020 2020 2020 2020 2020 6e70 2e6d              np.m
+0001bcd0: 696e 2878 5f76 616c 7320 2d20 7365 6c66  in(x_vals - self
+0001bce0: 2e6c 6f67 7368 6966 7429 2c0a 2020 2020  .logshift),.    
+0001bcf0: 2020 2020 2020 2020 6e70 2e6d 6178 2878          np.max(x
+0001bd00: 5f76 616c 7320 2d20 7365 6c66 2e6c 6f67  _vals - self.log
+0001bd10: 7368 6966 7429 2c0a 2020 2020 2020 2020  shift),.        
+0001bd20: 2020 2020 3130 3030 0a20 2020 2020 2020      1000.       
+0001bd30: 2029 0a0a 2020 2020 2020 2020 2320 5375   )..        # Su
+0001bd40: 6d20 6f66 2061 6c6c 206d 6f64 656c 732c  m of all models,
+0001bd50: 2073 6574 2074 6f20 7a65 726f 2069 6e69   set to zero ini
+0001bd60: 7469 616c 6c79 0a20 2020 2020 2020 2074  tially.        t
+0001bd70: 6f74 616c 5f72 6174 6573 203d 206e 702e  otal_rates = np.
+0001bd80: 7a65 726f 7328 6e70 2e73 6861 7065 2873  zeros(np.shape(s
+0001bd90: 656c 662e 785f 6772 6964 2929 0a0a 2020  elf.x_grid))..  
+0001bda0: 2020 2020 2020 2320 4469 6374 696f 6e61        # Dictiona
+0001bdb0: 7279 206f 6620 706c 6f74 730a 2020 2020  ry of plots.    
+0001bdc0: 2020 2020 2320 6b65 7973 2061 7265 206d      # keys are m
+0001bdd0: 6f64 656c 2e4e 414d 452e 6c6f 7765 7228  odel.NAME.lower(
+0001bde0: 292c 2076 616c 7565 7320 6172 6520 706c  ), values are pl
+0001bdf0: 6f74 5f77 6964 6765 742e 706c 6f74 0a20  ot_widget.plot. 
+0001be00: 2020 2020 2020 2073 656c 662e 6d6f 6465         self.mode
+0001be10: 6c5f 706c 6f74 7320 3d20 7b7d 0a0a 2020  l_plots = {}..  
+0001be20: 2020 2020 2020 2320 4c69 7374 206f 6620        # List of 
+0001be30: 6e69 6365 2063 6f6c 6f72 730a 2020 2020  nice colors.    
+0001be40: 2020 2020 636f 6c6f 7273 203d 206d 636f      colors = mco
+0001be50: 6c6f 7273 2e54 4142 4c45 4155 5f43 4f4c  lors.TABLEAU_COL
+0001be60: 4f52 532e 7661 6c75 6573 2829 0a0a 2020  ORS.values()..  
+0001be70: 2020 2020 2020 2320 4c6f 6f70 206f 7665        # Loop ove
+0001be80: 7220 616c 6c20 706f 7373 6962 6c65 206d  r all possible m
+0001be90: 6f64 656c 732c 2063 616c 6375 6c61 7465  odels, calculate
+0001bea0: 206d 6f64 656c 2076 616c 7565 730a 2020   model values.  
+0001beb0: 2020 2020 2020 2320 6174 2072 616e 6765        # at range
+0001bec0: 206f 6620 7465 6d70 6572 6174 7572 6573   of temperatures
+0001bed0: 2061 6e64 2070 6c6f 740a 2020 2020 2020   and plot.      
+0001bee0: 2020 2320 7468 656e 2061 6464 2074 6f20    # then add to 
+0001bef0: 6172 7261 7920 6f66 2074 6f74 616c 2072  array of total r
+0001bf00: 6174 6573 0a20 2020 2020 2020 2066 6f72  ates.        for
+0001bf10: 2063 6f6c 6f72 2c20 6d6f 6465 6c20 696e   color, model in
+0001bf20: 207a 6970 2863 6f6c 6f72 732c 2073 7570   zip(colors, sup
+0001bf30: 706f 7274 6564 5f6d 6f64 656c 7329 3a0a  ported_models):.
+0001bf40: 0a20 2020 2020 2020 2020 2020 2023 2047  .            # G
+0001bf50: 6574 2069 6e69 7469 616c 2076 616c 7565  et initial value
+0001bf60: 730a 2020 2020 2020 2020 2020 2020 696e  s.            in
+0001bf70: 6974 6961 6c73 203d 206d 6f64 656c 2e73  itials = model.s
+0001bf80: 6574 5f69 6e69 7469 616c 5f76 616c 7328  et_initial_vals(
+0001bf90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001bfa0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+0001bfb0: 2020 2020 2020 2070 6172 3a20 7365 6c66         par: self
+0001bfc0: 2e64 6566 6175 6c74 735b 6d6f 6465 6c2e  .defaults[model.
+0001bfd0: 4e41 4d45 5d5b 7061 725d 5b27 7661 6c69  NAME][par]['vali
+0001bfe0: 6e69 7427 5d0a 2020 2020 2020 2020 2020  nit'].          
+0001bff0: 2020 2020 2020 2020 2020 666f 7220 7061            for pa
+0001c000: 7220 696e 206d 6f64 656c 2e50 4152 4e41  r in model.PARNA
+0001c010: 4d45 530a 2020 2020 2020 2020 2020 2020  MES.            
+0001c020: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
+0001c030: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0001c040: 2320 4361 6c63 756c 6174 6520 7261 7465  # Calculate rate
+0001c050: 730a 2020 2020 2020 2020 2020 2020 7261  s.            ra
+0001c060: 7465 7320 3d20 3130 2a2a 286d 6f64 656c  tes = 10**(model
+0001c070: 2e6d 6f64 656c 2869 6e69 7469 616c 732c  .model(initials,
+0001c080: 2073 656c 662e 785f 6772 6964 2929 0a20   self.x_grid)). 
+0001c090: 2020 2020 2020 2020 2020 2023 2061 6e64             # and
+0001c0a0: 2061 6464 2074 6f20 746f 7461 6c20 6f66   add to total of
+0001c0b0: 2061 6c6c 206d 6f64 656c 730a 2020 2020   all models.    
+0001c0c0: 2020 2020 2020 2020 746f 7461 6c5f 7261          total_ra
+0001c0d0: 7465 7320 2b3d 2072 6174 6573 0a20 2020  tes += rates.   
+0001c0e0: 2020 2020 2020 2020 2023 2050 6c6f 7420           # Plot 
+0001c0f0: 7468 6973 206d 6f64 656c 0a20 2020 2020  this model.     
+0001c100: 2020 2020 2020 205f 706c 6f74 203d 2073         _plot = s
+0001c110: 656c 662e 706c 6f74 5f77 6964 6765 742e  elf.plot_widget.
+0001c120: 706c 6f74 280a 2020 2020 2020 2020 2020  plot(.          
+0001c130: 2020 2020 2020 7365 6c66 2e78 5f67 7269        self.x_gri
+0001c140: 6420 2b20 7365 6c66 2e6c 6f67 7368 6966  d + self.logshif
+0001c150: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
+0001c160: 2020 2072 6174 6573 2c0a 2020 2020 2020     rates,.      
+0001c170: 2020 2020 2020 2020 2020 7065 6e3d 7b27            pen={'
+0001c180: 7769 6474 6827 3a20 322e 352c 2027 636f  width': 2.5, 'co
+0001c190: 6c6f 7227 3a20 636f 6c6f 722c 2027 7374  lor': color, 'st
+0001c1a0: 796c 6527 3a20 5174 436f 7265 2e51 742e  yle': QtCore.Qt.
+0001c1b0: 4461 7368 4c69 6e65 7d0a 2020 2020 2020  DashLine}.      
+0001c1c0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0001c1d0: 2020 2020 2320 616e 6420 7374 6f72 6520      # and store 
+0001c1e0: 696e 2064 6963 7420 6f66 2061 6c6c 2070  in dict of all p
+0001c1f0: 6c6f 7473 0a20 2020 2020 2020 2020 2020  lots.           
+0001c200: 2073 656c 662e 6d6f 6465 6c5f 706c 6f74   self.model_plot
+0001c210: 735b 6d6f 6465 6c2e 4e41 4d45 2e6c 6f77  s[model.NAME.low
+0001c220: 6572 2829 5d20 3d20 5f70 6c6f 740a 2020  er()] = _plot.  
+0001c230: 2020 2020 2020 2020 2020 2320 5265 6d6f            # Remo
+0001c240: 7665 2066 726f 6d20 6163 7475 616c 2070  ve from actual p
+0001c250: 6c6f 7420 7769 6467 6574 0a20 2020 2020  lot widget.     
+0001c260: 2020 2020 2020 2023 2073 696e 6365 206e         # since n
+0001c270: 6f20 6d6f 6465 6c73 2061 7265 2076 6973  o models are vis
+0001c280: 6962 6c65 2069 6e69 7469 616c 6c79 0a20  ible initially. 
+0001c290: 2020 2020 2020 2020 2020 2023 2050 6c6f             # Plo
+0001c2a0: 7473 2061 7265 2072 652d 6164 6465 6420  ts are re-added 
+0001c2b0: 7769 7468 206d 6f64 656c 2063 6865 636b  with model check
+0001c2c0: 626f 7865 730a 2020 2020 2020 2020 2020  boxes.          
+0001c2d0: 2020 7365 6c66 2e70 6c6f 745f 7769 6467    self.plot_widg
+0001c2e0: 6574 2e72 656d 6f76 6549 7465 6d28 5f70  et.removeItem(_p
+0001c2f0: 6c6f 7429 0a0a 2020 2020 2020 2020 2320  lot)..        # 
+0001c300: 506c 6f74 2073 756d 206f 6620 616c 6c20  Plot sum of all 
+0001c310: 6d6f 6465 6c73 0a20 2020 2020 2020 2073  models.        s
+0001c320: 656c 662e 746f 7420 3d20 7365 6c66 2e70  elf.tot = self.p
+0001c330: 6c6f 745f 7769 6467 6574 2e70 6c6f 7428  lot_widget.plot(
+0001c340: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0001c350: 662e 785f 6772 6964 202b 2073 656c 662e  f.x_grid + self.
+0001c360: 6c6f 6773 6869 6674 2c0a 2020 2020 2020  logshift,.      
+0001c370: 2020 2020 2020 746f 7461 6c5f 7261 7465        total_rate
+0001c380: 732c 0a20 2020 2020 2020 2020 2020 2070  s,.            p
+0001c390: 656e 3d7b 2777 6964 7468 273a 2032 2e35  en={'width': 2.5
+0001c3a0: 2c20 2763 6f6c 6f72 273a 2027 7265 6427  , 'color': 'red'
+0001c3b0: 7d0a 2020 2020 2020 2020 290a 2020 2020  }.        ).    
+0001c3c0: 2020 2020 7365 6c66 2e70 6c6f 745f 7769      self.plot_wi
+0001c3d0: 6467 6574 2e72 656d 6f76 6549 7465 6d28  dget.removeItem(
+0001c3e0: 7365 6c66 2e74 6f74 290a 0a20 2020 2020  self.tot)..     
+0001c3f0: 2020 2023 2053 746f 7261 6765 206f 626a     # Storage obj
+0001c400: 6563 7420 666f 7220 6669 6e61 6c20 7061  ect for final pa
+0001c410: 7261 6d65 7465 7220 7661 6c75 6573 0a20  rameter values. 
+0001c420: 2020 2020 2020 2023 2053 6574 2061 6c6c         # Set all
+0001c430: 2069 6e69 7469 616c 2076 616c 7565 7320   initial values 
+0001c440: 6465 6661 756c 7473 0a20 2020 2020 2020  defaults.       
+0001c450: 2073 656c 662e 7061 7273 746f 7265 203d   self.parstore =
+0001c460: 2074 7970 6528 0a20 2020 2020 2020 2020   type(.         
+0001c470: 2020 2027 6f62 6a27 2c0a 2020 2020 2020     'obj',.      
+0001c480: 2020 2020 2020 286f 626a 6563 742c 292c        (object,),
+0001c490: 0a20 2020 2020 2020 2020 2020 207b 0a20  .            {. 
+0001c4a0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0001c4b0: 6172 3a20 7365 6c66 2e64 6566 6175 6c74  ar: self.default
+0001c4c0: 735b 6d6f 6465 6c2e 4e41 4d45 5d5b 7061  s[model.NAME][pa
+0001c4d0: 725d 5b27 7661 6c69 6e69 7427 5d0a 2020  r]['valinit'].  
+0001c4e0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0001c4f0: 7220 6d6f 6465 6c20 696e 2073 7570 706f  r model in suppo
+0001c500: 7274 6564 5f6d 6f64 656c 730a 2020 2020  rted_models.    
+0001c510: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0001c520: 7061 7220 696e 206d 6f64 656c 2e50 4152  par in model.PAR
+0001c530: 4e41 4d45 530a 2020 2020 2020 2020 2020  NAMES.          
+0001c540: 2020 7d0a 2020 2020 2020 2020 290a 0a20    }.        ).. 
+0001c550: 2020 2020 2020 2023 2043 6f6e 7665 7274         # Convert
+0001c560: 206c 6f67 2074 656d 7065 7261 7475 7265   log temperature
+0001c570: 2074 6963 6b73 2074 6f20 6c69 6e65 6172   ticks to linear
+0001c580: 0a20 2020 2020 2020 2061 7820 3d20 7365  .        ax = se
+0001c590: 6c66 2e70 6c6f 745f 7769 6467 6574 2e67  lf.plot_widget.g
+0001c5a0: 6574 4178 6973 2827 626f 7474 6f6d 2729  etAxis('bottom')
+0001c5b0: 0a20 2020 2020 2020 2067 7569 2e63 6f6e  .        gui.con
+0001c5c0: 7665 7274 5f6c 6f67 5f74 6963 6b73 5f74  vert_log_ticks_t
+0001c5d0: 6f5f 6c69 6e28 6178 2c20 6e70 2e6c 6f67  o_lin(ax, np.log
+0001c5e0: 3130 2878 5f76 616c 7329 2c20 7368 6966  10(x_vals), shif
+0001c5f0: 743d 7365 6c66 2e6c 6f67 7368 6966 7429  t=self.logshift)
+0001c600: 0a0a 2020 2020 2020 2020 2320 5248 5320  ..        # RHS 
+0001c610: 636f 6c75 6d6e 206f 6620 7769 6e64 6f77  column of window
+0001c620: 0a20 2020 2020 2020 2023 2054 6869 7320  .        # This 
+0001c630: 636f 6e74 6169 6e73 2065 6163 6820 6d6f  contains each mo
+0001c640: 6465 6c20 616e 6420 6974 7320 6173 736f  del and its asso
+0001c650: 6369 6174 6564 2070 6172 616d 6574 6572  ciated parameter
+0001c660: 730a 2020 2020 2020 2020 2320 4561 6368  s.        # Each
+0001c670: 2070 6172 616d 6574 6572 2069 7320 636f   parameter is co
+0001c680: 6e74 726f 6c6c 6564 2062 7920 610a 2020  ntrolled by a.  
+0001c690: 2020 2020 2020 2320 736c 6964 6572 732c        # sliders,
+0001c6a0: 2054 6578 7420 656e 7472 792c 2061 6e64   Text entry, and
+0001c6b0: 2061 2066 6974 2f66 6978 2074 6f67 676c   a fit/fix toggl
+0001c6c0: 650a 2020 2020 2020 2020 636f 6e74 6169  e.        contai
+0001c6d0: 6e65 725f 6c61 796f 7574 203d 2051 7457  ner_layout = QtW
+0001c6e0: 6964 6765 7473 2e51 5642 6f78 4c61 796f  idgets.QVBoxLayo
+0001c6f0: 7574 2873 6372 6f6c 6c5f 636f 6e74 6169  ut(scroll_contai
+0001c700: 6e65 7229 0a0a 2020 2020 2020 2020 2320  ner)..        # 
+0001c710: 4c69 7374 206f 6620 6e75 6d62 6572 206b  List of number k
+0001c720: 6579 2073 686f 7274 6375 7473 2074 6f20  ey shortcuts to 
+0001c730: 746f 6767 6c65 206d 6f64 656c 730a 2020  toggle models.  
+0001c740: 2020 2020 2020 7365 6c66 2e6f 6e5f 6f66        self.on_of
+0001c750: 665f 7368 6f72 7463 7574 203d 205b 5d0a  f_shortcut = [].
+0001c760: 0a20 2020 2020 2020 2023 2046 6f72 2065  .        # For e
+0001c770: 6163 6820 6d6f 6465 6c2c 206d 616b 6520  ach model, make 
+0001c780: 6120 626f 7820 746f 2063 6f6e 7461 696e  a box to contain
+0001c790: 2061 6c6c 2070 6172 616d 6574 6572 730a   all parameters.
+0001c7a0: 2020 2020 2020 2020 2320 616e 6420 706f          # and po
+0001c7b0: 7075 6c61 7465 2077 6974 6820 7061 7261  pulate with para
+0001c7c0: 6d65 7465 7273 0a20 2020 2020 2020 2066  meters.        f
+0001c7d0: 6f72 206d 6974 2c20 6d6f 6465 6c20 696e  or mit, model in
+0001c7e0: 2065 6e75 6d65 7261 7465 2873 7570 706f   enumerate(suppo
+0001c7f0: 7274 6564 5f6d 6f64 656c 7329 3a0a 2020  rted_models):.  
+0001c800: 2020 2020 2020 2020 2020 6d6f 6465 6c5f            model_
+0001c810: 7769 6467 6574 203d 2073 656c 662e 6d61  widget = self.ma
+0001c820: 6b65 5f6d 6f64 656c 626f 7828 6d6f 6465  ke_modelbox(mode
+0001c830: 6c2c 2073 6372 6f6c 6c5f 636f 6e74 6169  l, scroll_contai
+0001c840: 6e65 722c 206d 6974 202b 2031 290a 0a20  ner, mit + 1).. 
+0001c850: 2020 2020 2020 2020 2020 2023 2041 6464             # Add
+0001c860: 2074 6869 7320 6d6f 6465 6c20 746f 2074   this model to t
+0001c870: 6865 2072 6967 6874 2068 616e 6420 7369  he right hand si
+0001c880: 6465 206f 6620 7468 6520 7769 6e64 6f77  de of the window
+0001c890: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+0001c8a0: 7461 696e 6572 5f6c 6179 6f75 742e 6164  tainer_layout.ad
+0001c8b0: 6457 6964 6765 7428 6d6f 6465 6c5f 7769  dWidget(model_wi
+0001c8c0: 6467 6574 2c20 6c65 6e28 6d6f 6465 6c2e  dget, len(model.
+0001c8d0: 5041 524e 414d 4553 2929 0a0a 2020 2020  PARNAMES))..    
+0001c8e0: 2020 2020 2320 4469 7361 626c 6520 6576      # Disable ev
+0001c8f0: 6572 7920 736c 6964 6572 2c20 656e 7472  ery slider, entr
+0001c900: 792c 2061 6e64 2066 6974 2f66 6978 2062  y, and fit/fix b
+0001c910: 7920 6465 6661 756c 740a 2020 2020 2020  y default.      
+0001c920: 2020 2320 5468 6973 2069 7320 746f 6767    # This is togg
+0001c930: 6c65 6420 6279 2074 6865 206d 6f64 656c  led by the model
+0001c940: 2063 6865 636b 626f 7865 730a 2020 2020   checkboxes.    
+0001c950: 2020 2020 666f 7220 6d6f 6465 6c20 696e      for model in
+0001c960: 2073 7570 706f 7274 6564 5f6d 6f64 656c   supported_model
+0001c970: 733a 0a20 2020 2020 2020 2020 2020 206d  s:.            m
+0001c980: 6f64 656c 6e61 6d65 203d 206d 6f64 656c  odelname = model
+0001c990: 2e4e 414d 452e 6c6f 7765 7228 290a 2020  .NAME.lower().  
+0001c9a0: 2020 2020 2020 2020 2020 666f 7220 7061            for pa
+0001c9b0: 726e 616d 6520 696e 206d 6f64 656c 2e50  rname in model.P
+0001c9c0: 4152 4e41 4d45 533a 0a20 2020 2020 2020  ARNAMES:.       
+0001c9d0: 2020 2020 2020 2020 2073 656c 662e 7769           self.wi
+0001c9e0: 6467 6574 6469 6374 5b6d 6f64 656c 6e61  dgetdict[modelna
+0001c9f0: 6d65 5d5b 7061 726e 616d 655d 5b27 736c  me][parname]['sl
+0001ca00: 6964 6572 275d 2e73 6574 456e 6162 6c65  ider'].setEnable
+0001ca10: 6428 4661 6c73 6529 0a20 2020 2020 2020  d(False).       
+0001ca20: 2020 2020 2020 2020 2073 656c 662e 7769           self.wi
+0001ca30: 6467 6574 6469 6374 5b6d 6f64 656c 6e61  dgetdict[modelna
+0001ca40: 6d65 5d5b 7061 726e 616d 655d 5b27 656e  me][parname]['en
+0001ca50: 7472 7927 5d2e 7365 7445 6e61 626c 6564  try'].setEnabled
+0001ca60: 2846 616c 7365 290a 2020 2020 2020 2020  (False).        
+0001ca70: 2020 2020 2020 2020 7365 6c66 2e77 6964          self.wid
+0001ca80: 6765 7464 6963 745b 6d6f 6465 6c6e 616d  getdict[modelnam
+0001ca90: 655d 5b70 6172 6e61 6d65 5d5b 2766 665f  e][parname]['ff_
+0001caa0: 746f 6767 6c65 275d 2e73 6574 456e 6162  toggle'].setEnab
+0001cab0: 6c65 6428 0a20 2020 2020 2020 2020 2020  led(.           
+0001cac0: 2020 2020 2020 2020 2046 616c 7365 0a20           False. 
+0001cad0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0001cae0: 0a0a 2020 2020 2020 2020 636f 6e74 6169  ..        contai
+0001caf0: 6e65 725f 6c61 796f 7574 2e73 6574 416c  ner_layout.setAl
+0001cb00: 6967 6e6d 656e 7428 5174 436f 7265 2e51  ignment(QtCore.Q
+0001cb10: 742e 416c 6967 6e56 4365 6e74 6572 290a  t.AlignVCenter).
+0001cb20: 2020 2020 2020 2020 7363 726f 6c6c 5f63          scroll_c
+0001cb30: 6f6e 7461 696e 6572 2e73 6574 5369 7a65  ontainer.setSize
+0001cb40: 506f 6c69 6379 280a 2020 2020 2020 2020  Policy(.        
+0001cb50: 2020 2020 5174 5769 6467 6574 732e 5153      QtWidgets.QS
+0001cb60: 697a 6550 6f6c 6963 792e 4d61 7869 6d75  izePolicy.Maximu
+0001cb70: 6d2c 0a20 2020 2020 2020 2020 2020 2051  m,.            Q
+0001cb80: 7457 6964 6765 7473 2e51 5369 7a65 506f  tWidgets.QSizePo
+0001cb90: 6c69 6379 2e4d 6178 696d 756d 0a20 2020  licy.Maximum.   
+0001cba0: 2020 2020 2029 0a20 2020 2020 2020 2072       ).        r
+0001cbb0: 6873 5f63 6f6c 5f73 6372 6f6c 6c2e 7365  hs_col_scroll.se
+0001cbc0: 744d 696e 696d 756d 4865 6967 6874 2835  tMinimumHeight(5
+0001cbd0: 3735 290a 0a20 2020 2020 2020 2023 2054  75)..        # T
+0001cbe0: 6f70 2072 6f77 0a20 2020 2020 2020 2023  op row.        #
+0001cbf0: 204c 4853 2070 6c6f 742c 2052 4853 2053   LHS plot, RHS S
+0001cc00: 6c69 6465 7273 2c20 7465 7874 2c20 6c61  liders, text, la
+0001cc10: 6265 6c73 0a20 2020 2020 2020 2074 6f70  bels.        top
+0001cc20: 5f72 6f77 5f6c 6179 6f75 7420 3d20 5174  _row_layout = Qt
+0001cc30: 5769 6467 6574 732e 5148 426f 784c 6179  Widgets.QHBoxLay
+0001cc40: 6f75 7428 746f 705f 726f 775f 7769 6467  out(top_row_widg
+0001cc50: 6574 290a 2020 2020 2020 2020 746f 705f  et).        top_
+0001cc60: 726f 775f 6c61 796f 7574 2e61 6464 5769  row_layout.addWi
+0001cc70: 6467 6574 286c 6873 5f63 6f6c 5f77 6964  dget(lhs_col_wid
+0001cc80: 6765 742c 2033 290a 2020 2020 2020 2020  get, 3).        
+0001cc90: 746f 705f 726f 775f 6c61 796f 7574 2e61  top_row_layout.a
+0001cca0: 6464 5769 6467 6574 2872 6873 5f63 6f6c  ddWidget(rhs_col
+0001ccb0: 5f77 6964 6765 742c 2032 290a 0a20 2020  _widget, 2)..   
+0001ccc0: 2020 2020 2023 2042 6f74 746f 6d20 726f       # Bottom ro
+0001ccd0: 770a 2020 2020 2020 2020 2320 4275 7474  w.        # Butt
+0001cce0: 6f6e 7320 666f 7220 7265 7365 7420 616e  ons for reset an
+0001ccf0: 6420 6669 740a 2020 2020 2020 2020 7365  d fit.        se
+0001cd00: 6c66 2e66 6974 5f62 746e 5f77 6964 6765  lf.fit_btn_widge
+0001cd10: 7420 3d20 5174 5769 6467 6574 732e 5150  t = QtWidgets.QP
+0001cd20: 7573 6842 7574 746f 6e28 0a20 2020 2020  ushButton(.     
+0001cd30: 2020 2020 2020 2070 6172 656e 743d 626f         parent=bo
+0001cd40: 745f 726f 775f 7769 6467 6574 2c0a 2020  t_row_widget,.  
+0001cd50: 2020 2020 2020 2020 2020 7465 7874 3d27            text='
+0001cd60: 4669 7427 0a20 2020 2020 2020 2029 0a20  Fit'.        ). 
+0001cd70: 2020 2020 2020 2073 656c 662e 6669 745f         self.fit_
+0001cd80: 6274 6e5f 7769 6467 6574 2e73 6574 5374  btn_widget.setSt
+0001cd90: 796c 6553 6865 6574 2827 666f 6e74 2d77  yleSheet('font-w
+0001cda0: 6569 6768 743a 2062 6f6c 643b 2729 0a0a  eight: bold;')..
+0001cdb0: 2020 2020 2020 2020 7365 6c66 2e66 6974          self.fit
+0001cdc0: 5f62 746e 5f77 6964 6765 742e 7365 7445  _btn_widget.setE
+0001cdd0: 6e61 626c 6564 2846 616c 7365 290a 2020  nabled(False).  
+0001cde0: 2020 2020 2020 7365 6c66 2e66 6974 5f62        self.fit_b
+0001cdf0: 746e 5f77 6964 6765 742e 636c 6963 6b65  tn_widget.clicke
+0001ce00: 642e 636f 6e6e 6563 7428 7365 6c66 2e66  d.connect(self.f
+0001ce10: 6974 290a 2020 2020 2020 2020 7365 6c66  it).        self
+0001ce20: 2e66 6974 5f62 746e 5f77 6964 6765 742e  .fit_btn_widget.
+0001ce30: 7365 7453 697a 6550 6f6c 6963 7928 0a20  setSizePolicy(. 
+0001ce40: 2020 2020 2020 2020 2020 2051 7457 6964             QtWid
+0001ce50: 6765 7473 2e51 5369 7a65 506f 6c69 6379  gets.QSizePolicy
+0001ce60: 2e46 6978 6564 2c0a 2020 2020 2020 2020  .Fixed,.        
+0001ce70: 2020 2020 5174 5769 6467 6574 732e 5153      QtWidgets.QS
+0001ce80: 697a 6550 6f6c 6963 792e 4669 7865 640a  izePolicy.Fixed.
+0001ce90: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0001cea0: 2020 7265 7365 745f 6274 6e5f 7769 6467    reset_btn_widg
+0001ceb0: 6574 203d 2051 7457 6964 6765 7473 2e51  et = QtWidgets.Q
+0001cec0: 5075 7368 4275 7474 6f6e 280a 2020 2020  PushButton(.    
+0001ced0: 2020 2020 2020 2020 7061 7265 6e74 3d62          parent=b
+0001cee0: 6f74 5f72 6f77 5f77 6964 6765 742c 0a20  ot_row_widget,. 
+0001cef0: 2020 2020 2020 2020 2020 2074 6578 743d             text=
+0001cf00: 2752 6573 6574 272c 0a20 2020 2020 2020  'Reset',.       
+0001cf10: 2029 0a20 2020 2020 2020 2072 6573 6574   ).        reset
+0001cf20: 5f62 746e 5f77 6964 6765 742e 7365 7453  _btn_widget.setS
+0001cf30: 7479 6c65 5368 6565 7428 2766 6f6e 742d  tyleSheet('font-
+0001cf40: 7765 6967 6874 3a20 626f 6c64 3b27 290a  weight: bold;').
+0001cf50: 2020 2020 2020 2020 7265 7365 745f 6274          reset_bt
+0001cf60: 6e5f 7769 6467 6574 2e63 6c69 636b 6564  n_widget.clicked
+0001cf70: 2e63 6f6e 6e65 6374 2873 656c 662e 7265  .connect(self.re
+0001cf80: 7365 7429 0a20 2020 2020 2020 2072 6573  set).        res
+0001cf90: 6574 5f62 746e 5f77 6964 6765 742e 7365  et_btn_widget.se
+0001cfa0: 7453 697a 6550 6f6c 6963 7928 0a20 2020  tSizePolicy(.   
+0001cfb0: 2020 2020 2020 2020 2051 7457 6964 6765           QtWidge
+0001cfc0: 7473 2e51 5369 7a65 506f 6c69 6379 2e46  ts.QSizePolicy.F
+0001cfd0: 6978 6564 2c0a 2020 2020 2020 2020 2020  ixed,.          
+0001cfe0: 2020 5174 5769 6467 6574 732e 5153 697a    QtWidgets.QSiz
+0001cff0: 6550 6f6c 6963 792e 4669 7865 640a 2020  ePolicy.Fixed.  
+0001d000: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0001d010: 2023 204d 6f64 6966 7920 6669 7420 616e   # Modify fit an
+0001d020: 6420 7265 7365 7420 6275 7474 6f6e 2074  d reset button t
+0001d030: 6578 7420 636f 6c6f 7273 2074 6f20 6c6f  ext colors to lo
+0001d040: 6f6b 2067 6f6f 6420 6576 656e 0a20 2020  ok good even.   
+0001d050: 2020 2020 2023 2069 6e20 4d61 634f 5320       # in MacOS 
+0001d060: 6461 726b 6d6f 6465 2e0a 2020 2020 2020  darkmode..      
+0001d070: 2020 7061 6c65 7474 6520 3d20 5174 4775    palette = QtGu
+0001d080: 692e 5150 616c 6574 7465 2873 656c 662e  i.QPalette(self.
+0001d090: 6669 745f 6274 6e5f 7769 6467 6574 2e70  fit_btn_widget.p
+0001d0a0: 616c 6574 7465 2829 290a 2020 2020 2020  alette()).      
+0001d0b0: 2020 7061 6c65 7474 652e 7365 7443 6f6c    palette.setCol
+0001d0c0: 6f72 2851 7447 7569 2e51 5061 6c65 7474  or(QtGui.QPalett
+0001d0d0: 652e 4275 7474 6f6e 5465 7874 2c20 5174  e.ButtonText, Qt
+0001d0e0: 4775 692e 5143 6f6c 6f72 2827 2330 6462  Gui.QColor('#0db
+0001d0f0: 3237 3327 2929 0a20 2020 2020 2020 2073  273')).        s
+0001d100: 656c 662e 6669 745f 6274 6e5f 7769 6467  elf.fit_btn_widg
+0001d110: 6574 2e73 6574 5061 6c65 7474 6528 7061  et.setPalette(pa
+0001d120: 6c65 7474 6529 0a20 2020 2020 2020 2070  lette).        p
+0001d130: 616c 6574 7465 2e73 6574 436f 6c6f 7228  alette.setColor(
+0001d140: 5174 4775 692e 5150 616c 6574 7465 2e42  QtGui.QPalette.B
+0001d150: 7574 746f 6e54 6578 742c 2051 7447 7569  uttonText, QtGui
+0001d160: 2e51 436f 6c6f 7228 2723 3462 3661 6164  .QColor('#4b6aad
+0001d170: 2729 290a 2020 2020 2020 2020 7265 7365  ')).        rese
+0001d180: 745f 6274 6e5f 7769 6467 6574 2e73 6574  t_btn_widget.set
+0001d190: 5061 6c65 7474 6528 7061 6c65 7474 6529  Palette(palette)
+0001d1a0: 0a0a 2020 2020 2020 2020 2320 4b65 7962  ..        # Keyb
+0001d1b0: 6f61 7264 2073 686f 7274 6375 742c 2070  oard shortcut, p
+0001d1c0: 7265 7373 2066 2074 6f20 6669 7420 6966  ress f to fit if
+0001d1d0: 2066 6974 2062 7574 746f 6e20 6e6f 7420   fit button not 
+0001d1e0: 6772 6579 6564 206f 7574 0a20 2020 2020  greyed out.     
+0001d1f0: 2020 2073 656c 662e 6669 745f 7368 6f72     self.fit_shor
+0001d200: 7463 7574 203d 2051 7457 6964 6765 7473  tcut = QtWidgets
+0001d210: 2e51 5368 6f72 7463 7574 2851 7447 7569  .QShortcut(QtGui
+0001d220: 2e51 4b65 7953 6571 7565 6e63 6528 2766  .QKeySequence('f
+0001d230: 2729 2c20 7365 6c66 290a 2020 2020 2020  '), self).      
+0001d240: 2020 7365 6c66 2e66 6974 5f73 686f 7274    self.fit_short
+0001d250: 6375 742e 6163 7469 7661 7465 642e 636f  cut.activated.co
+0001d260: 6e6e 6563 7428 0a20 2020 2020 2020 2020  nnect(.         
+0001d270: 2020 206c 616d 6264 613a 2073 656c 662e     lambda: self.
+0001d280: 6b65 7962 6f61 7264 5f66 6974 5f63 616c  keyboard_fit_cal
+0001d290: 6c62 6163 6b28 290a 2020 2020 2020 2020  lback().        
+0001d2a0: 290a 0a20 2020 2020 2020 2062 6f74 5f72  )..        bot_r
+0001d2b0: 6f77 5f6c 6179 6f75 7420 3d20 5174 5769  ow_layout = QtWi
+0001d2c0: 6467 6574 732e 5148 426f 784c 6179 6f75  dgets.QHBoxLayou
+0001d2d0: 7428 626f 745f 726f 775f 7769 6467 6574  t(bot_row_widget
+0001d2e0: 290a 2020 2020 2020 2020 626f 745f 726f  ).        bot_ro
+0001d2f0: 775f 6c61 796f 7574 2e61 6464 5769 6467  w_layout.addWidg
+0001d300: 6574 2873 656c 662e 6669 745f 6274 6e5f  et(self.fit_btn_
+0001d310: 7769 6467 6574 290a 2020 2020 2020 2020  widget).        
+0001d320: 626f 745f 726f 775f 6c61 796f 7574 2e61  bot_row_layout.a
+0001d330: 6464 5769 6467 6574 2872 6573 6574 5f62  ddWidget(reset_b
+0001d340: 746e 5f77 6964 6765 7429 0a0a 2020 2020  tn_widget)..    
+0001d350: 2020 2020 2320 4f76 6572 616c 6c20 6170      # Overall ap
+0001d360: 700a 2020 2020 2020 2020 2320 546f 7020  p.        # Top 
+0001d370: 616e 6420 426f 7474 6f6d 2072 6f77 730a  and Bottom rows.
+0001d380: 2020 2020 2020 2020 6675 6c6c 5f6c 6179          full_lay
+0001d390: 6f75 7420 3d20 5174 5769 6467 6574 732e  out = QtWidgets.
+0001d3a0: 5156 426f 784c 6179 6f75 7428 7365 6c66  QVBoxLayout(self
+0001d3b0: 2e77 6964 6765 7429 0a20 2020 2020 2020  .widget).       
+0001d3c0: 2066 756c 6c5f 6c61 796f 7574 2e61 6464   full_layout.add
+0001d3d0: 5769 6467 6574 2874 6f70 5f72 6f77 5f77  Widget(top_row_w
+0001d3e0: 6964 6765 7429 0a20 2020 2020 2020 2066  idget).        f
+0001d3f0: 756c 6c5f 6c61 796f 7574 2e61 6464 5769  ull_layout.addWi
+0001d400: 6467 6574 2862 6f74 5f72 6f77 5f77 6964  dget(bot_row_wid
+0001d410: 6765 7429 0a0a 2020 2020 2020 2020 2320  get)..        # 
+0001d420: 5365 7420 6c61 796f 7574 0a20 2020 2020  Set layout.     
+0001d430: 2020 2073 656c 662e 7769 6467 6574 2e73     self.widget.s
+0001d440: 6574 4c61 796f 7574 2866 756c 6c5f 6c61  etLayout(full_la
+0001d450: 796f 7574 290a 2020 2020 2020 2020 7365  yout).        se
+0001d460: 6c66 2e77 6964 6765 742e 7365 7453 697a  lf.widget.setSiz
+0001d470: 6550 6f6c 6963 7928 0a20 2020 2020 2020  ePolicy(.       
+0001d480: 2020 2020 2051 7457 6964 6765 7473 2e51       QtWidgets.Q
+0001d490: 5369 7a65 506f 6c69 6379 2e45 7870 616e  SizePolicy.Expan
+0001d4a0: 6469 6e67 2c0a 2020 2020 2020 2020 2020  ding,.          
+0001d4b0: 2020 5174 5769 6467 6574 732e 5153 697a    QtWidgets.QSiz
+0001d4c0: 6550 6f6c 6963 792e 4578 7061 6e64 696e  ePolicy.Expandin
+0001d4d0: 670a 2020 2020 2020 2020 290a 0a20 2020  g.        )..   
+0001d4e0: 2020 2020 2072 6574 7572 6e0a 0a20 2020       return..   
+0001d4f0: 2064 6566 206b 6579 626f 6172 645f 6669   def keyboard_fi
+0001d500: 745f 6361 6c6c 6261 636b 2873 656c 6629  t_callback(self)
+0001d510: 3a0a 2020 2020 2020 2020 2727 270a 2020  :.        '''.  
+0001d520: 2020 2020 2020 4361 6c6c 6261 636b 2066        Callback f
+0001d530: 6f72 2070 7265 7373 696e 6720 2766 2720  or pressing 'f' 
+0001d540: 6b65 792e 2052 756e 7320 6669 7420 6275  key. Runs fit bu
+0001d550: 7474 6f6e 2069 6620 6e6f 7420 6772 6579  tton if not grey
+0001d560: 6564 206f 7574 0a20 2020 2020 2020 2027  ed out.        '
+0001d570: 2727 0a0a 2020 2020 2020 2020 2320 4368  ''..        # Ch
+0001d580: 6563 6b20 6669 7420 6275 7474 6f6e 2069  eck fit button i
+0001d590: 7320 6e6f 7420 6772 6579 6564 206f 7574  s not greyed out
+0001d5a0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0001d5b0: 2e66 6974 5f62 746e 5f77 6964 6765 742e  .fit_btn_widget.
+0001d5c0: 6973 456e 6162 6c65 6428 293a 0a20 2020  isEnabled():.   
+0001d5d0: 2020 2020 2020 2020 2023 2052 756e 2066           # Run f
+0001d5e0: 6974 2063 6f64 652c 2074 6869 7320 636c  it code, this cl
+0001d5f0: 6f73 6573 2061 7070 0a20 2020 2020 2020  oses app.       
+0001d600: 2020 2020 2073 656c 662e 6669 7428 290a       self.fit().
+0001d610: 0a20 2020 2020 2020 2072 6574 7572 6e0a  .        return.
+0001d620: 0a20 2020 2064 6566 2072 6573 6574 2873  .    def reset(s
+0001d630: 656c 6629 3a0a 2020 2020 2020 2020 2727  elf):.        ''
+0001d640: 270a 2020 2020 2020 2020 4361 6c6c 6261  '.        Callba
+0001d650: 636b 2066 6f72 2052 6573 6574 2062 7574  ck for Reset but
+0001d660: 746f 6e2e 0a20 2020 2020 2020 2052 6574  ton..        Ret
+0001d670: 7572 6e73 2077 696e 646f 7720 6261 636b  urns window back
+0001d680: 2074 6f20 6f72 6967 696e 616c 206c 6179   to original lay
+0001d690: 6f75 742f 7365 6c65 6374 696f 6e73 0a20  out/selections. 
+0001d6a0: 2020 2020 2020 2027 2727 0a0a 2020 2020         '''..    
+0001d6b0: 2020 2020 2320 466f 7220 6561 6368 206d      # For each m
+0001d6c0: 6f64 656c 2c20 7265 6d6f 7665 2070 6c6f  odel, remove plo
+0001d6d0: 742c 2061 6e64 2072 6573 6574 2070 6172  t, and reset par
+0001d6e0: 616d 6574 6572 2076 616c 7565 730a 2020  ameter values.  
+0001d6f0: 2020 2020 2020 666f 7220 6d6f 6465 6c20        for model 
+0001d700: 696e 2073 656c 662e 7375 7070 6f72 7465  in self.supporte
+0001d710: 645f 6d6f 6465 6c73 3a0a 2020 2020 2020  d_models:.      
+0001d720: 2020 2020 2020 6d6f 6465 6c6e 616d 6520        modelname 
+0001d730: 3d20 6d6f 6465 6c2e 4e41 4d45 2e6c 6f77  = model.NAME.low
+0001d740: 6572 2829 0a0a 2020 2020 2020 2020 2020  er()..          
+0001d750: 2020 2320 4469 7361 626c 6520 616c 6c20    # Disable all 
+0001d760: 6d6f 6465 6c73 0a20 2020 2020 2020 2020  models.         
+0001d770: 2020 2073 656c 662e 7573 656c 2e6d 6f64     self.usel.mod
+0001d780: 656c 735b 6d6f 6465 6c6e 616d 655d 203d  els[modelname] =
+0001d790: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
+0001d7a0: 2020 2023 2061 6e64 2075 6e74 6963 6b20     # and untick 
+0001d7b0: 6368 6563 6b62 6f78 6573 0a20 2020 2020  checkboxes.     
+0001d7c0: 2020 2020 2020 2073 656c 662e 7469 636b         self.tick
+0001d7d0: 6469 6374 5b6d 6f64 656c 6e61 6d65 5d2e  dict[modelname].
+0001d7e0: 7365 7443 6865 636b 5374 6174 6528 4661  setCheckState(Fa
+0001d7f0: 6c73 6529 0a0a 2020 2020 2020 2020 2020  lse)..          
+0001d800: 2020 2320 5265 6d6f 7665 2063 6f72 7265    # Remove corre
+0001d810: 7370 6f6e 6469 6e67 2070 6c6f 740a 2020  sponding plot.  
+0001d820: 2020 2020 2020 2020 2020 5f70 6c6f 7420            _plot 
+0001d830: 3d20 7365 6c66 2e6d 6f64 656c 5f70 6c6f  = self.model_plo
+0001d840: 7473 5b6d 6f64 656c 6e61 6d65 5d0a 2020  ts[modelname].  
+0001d850: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+0001d860: 6c6f 745f 7769 6467 6574 2e72 656d 6f76  lot_widget.remov
+0001d870: 6549 7465 6d28 5f70 6c6f 7429 0a0a 2020  eItem(_plot)..  
+0001d880: 2020 2020 2020 2020 2020 2320 5265 7365            # Rese
+0001d890: 7420 6561 6368 2070 6172 616d 6574 6572  t each parameter
+0001d8a0: 2073 6c69 6465 722c 2065 6e74 7279 2c20   slider, entry, 
+0001d8b0: 616e 6420 6669 7466 6978 0a20 2020 2020  and fitfix.     
+0001d8c0: 2020 2020 2020 2023 2062 6163 6b20 746f         # back to
+0001d8d0: 206f 7269 6769 6e61 6c20 7661 6c75 650a   original value.
+0001d8e0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0001d8f0: 7061 726e 616d 6520 696e 206d 6f64 656c  parname in model
+0001d900: 2e50 4152 4e41 4d45 533a 0a20 2020 2020  .PARNAMES:.     
+0001d910: 2020 2020 2020 2020 2020 2073 6574 6174             setat
+0001d920: 7472 280a 2020 2020 2020 2020 2020 2020  tr(.            
+0001d930: 2020 2020 2020 2020 7365 6c66 2e70 6172          self.par
+0001d940: 7374 6f72 652c 0a20 2020 2020 2020 2020  store,.         
+0001d950: 2020 2020 2020 2020 2020 2070 6172 6e61             parna
+0001d960: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
+0001d970: 2020 2020 2020 2020 7365 6c66 2e64 6566          self.def
+0001d980: 6175 6c74 735b 6d6f 6465 6c2e 4e41 4d45  aults[model.NAME
+0001d990: 5d5b 7061 726e 616d 655d 5b27 7661 6c69  ][parname]['vali
+0001d9a0: 6e69 7427 5d0a 2020 2020 2020 2020 2020  nit'].          
+0001d9b0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0001d9c0: 2020 2020 2020 2020 7365 6c66 2e77 6964          self.wid
+0001d9d0: 6765 7464 6963 745b 6d6f 6465 6c6e 616d  getdict[modelnam
+0001d9e0: 655d 5b70 6172 6e61 6d65 5d5b 2773 6c69  e][parname]['sli
+0001d9f0: 6465 7227 5d2e 7365 7456 616c 7565 280a  der'].setValue(.
 0001da00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001da10: 696e 7428 7365 6c66 2e64 6566 6175 6c74  int(self.default
-0001da20: 735b 6d6f 6465 6c2e 4e41 4d45 5d5b 7061  s[model.NAME][pa
-0001da30: 726e 616d 655d 5b27 7661 6c69 6e69 7427  rname]['valinit'
-0001da40: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-0001da50: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0001da60: 2020 2020 2073 656c 662e 7769 6467 6574       self.widget
-0001da70: 6469 6374 5b6d 6f64 656c 6e61 6d65 5d5b  dict[modelname][
-0001da80: 7061 726e 616d 655d 5b27 656e 7472 7927  parname]['entry'
-0001da90: 5d2e 7365 7456 616c 7565 280a 2020 2020  ].setValue(.    
+0001da10: 2020 2020 696e 7428 7365 6c66 2e64 6566      int(self.def
+0001da20: 6175 6c74 735b 6d6f 6465 6c2e 4e41 4d45  aults[model.NAME
+0001da30: 5d5b 7061 726e 616d 655d 5b27 7661 6c69  ][parname]['vali
+0001da40: 6e69 7427 5d29 0a20 2020 2020 2020 2020  nit']).         
+0001da50: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0001da60: 2020 2020 2020 2020 2073 656c 662e 7769           self.wi
+0001da70: 6467 6574 6469 6374 5b6d 6f64 656c 6e61  dgetdict[modelna
+0001da80: 6d65 5d5b 7061 726e 616d 655d 5b27 656e  me][parname]['en
+0001da90: 7472 7927 5d2e 7365 7456 616c 7565 280a  try'].setValue(.
 0001daa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dab0: 7365 6c66 2e64 6566 6175 6c74 735b 6d6f  self.defaults[mo
-0001dac0: 6465 6c2e 4e41 4d45 5d5b 7061 726e 616d  del.NAME][parnam
-0001dad0: 655d 5b27 7661 6c69 6e69 7427 5d0a 2020  e]['valinit'].  
-0001dae0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0001daf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001db00: 7365 6c66 2e77 6964 6765 7464 6963 745b  self.widgetdict[
-0001db10: 6d6f 6465 6c6e 616d 655d 5b70 6172 6e61  modelname][parna
-0001db20: 6d65 5d5b 2766 665f 746f 6767 6c65 275d  me]['ff_toggle']
-0001db30: 2e73 6574 5465 7874 280a 2020 2020 2020  .setText(.      
-0001db40: 2020 2020 2020 2020 2020 2020 2020 2746                'F
-0001db50: 7265 6527 0a20 2020 2020 2020 2020 2020  ree'.           
-0001db60: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-0001db70: 2320 5265 6d6f 7665 2074 6f74 616c 206d  # Remove total m
-0001db80: 6f64 656c 2070 6c6f 740a 2020 2020 2020  odel plot.      
-0001db90: 2020 7365 6c66 2e70 6c6f 745f 7769 6467    self.plot_widg
-0001dba0: 6574 2e72 656d 6f76 6549 7465 6d28 7365  et.removeItem(se
-0001dbb0: 6c66 2e74 6f74 290a 0a20 2020 2020 2020  lf.tot)..       
-0001dbc0: 2072 6574 7572 6e0a 0a20 2020 2064 6566   return..    def
-0001dbd0: 2066 6974 2873 656c 6629 3a0a 2020 2020   fit(self):.    
-0001dbe0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-0001dbf0: 4361 6c6c 6261 636b 2066 6f72 2046 6974  Callback for Fit
-0001dc00: 2062 7574 746f 6e2e 0a20 2020 2020 2020   button..       
-0001dc10: 2043 6f6c 6c65 6374 7320 7661 7269 6162   Collects variab
-0001dc20: 6c65 2076 616c 7565 7320 6f66 2065 6163  le values of eac
-0001dc30: 6820 6d6f 6465 6c20 616e 6420 6173 7365  h model and asse
-0001dc40: 6d62 6c65 7320 696e 746f 2066 6974 2f66  mbles into fit/f
-0001dc50: 6978 0a20 2020 2020 2020 2064 6963 7469  ix.        dicti
-0001dc60: 6f6e 6172 6965 732c 2074 6865 6e20 636c  onaries, then cl
-0001dc70: 6f73 6573 2074 6865 2077 696e 646f 772e  oses the window.
-0001dc80: 0a20 2020 2020 2020 2027 2727 0a0a 2020  .        '''..  
-0001dc90: 2020 2020 2020 6c6e 616d 655f 746f 5f6d        lname_to_m
-0001dca0: 6f64 656c 203d 207b 0a20 2020 2020 2020  odel = {.       
-0001dcb0: 2020 2020 206d 6f64 656c 2e4e 414d 452e       model.NAME.
-0001dcc0: 6c6f 7765 7228 293a 206d 6f64 656c 0a20  lower(): model. 
-0001dcd0: 2020 2020 2020 2020 2020 2066 6f72 206d             for m
-0001dce0: 6f64 656c 2069 6e20 7365 6c66 2e73 7570  odel in self.sup
-0001dcf0: 706f 7274 6564 5f6d 6f64 656c 730a 2020  ported_models.  
-0001dd00: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
-0001dd10: 2023 2043 6f6c 6c65 6374 2076 6172 6961   # Collect varia
-0001dd20: 626c 6573 206f 6620 6561 6368 206d 6f64  bles of each mod
-0001dd30: 656c 2c20 6966 2074 6861 7420 6d6f 6465  el, if that mode
-0001dd40: 6c20 6973 2065 6e61 626c 6564 0a20 2020  l is enabled.   
-0001dd50: 2020 2020 2023 2061 6e64 2061 7373 6967       # and assig
-0001dd60: 6e20 746f 2066 6974 206f 7220 6669 780a  n to fit or fix.
-0001dd70: 2020 2020 2020 2020 666f 7220 6d6f 6465          for mode
-0001dd80: 6c6e 616d 652c 2065 6e61 626c 6564 2069  lname, enabled i
-0001dd90: 6e20 7365 6c66 2e75 7365 6c2e 6d6f 6465  n self.usel.mode
-0001dda0: 6c73 2e69 7465 6d73 2829 3a0a 2020 2020  ls.items():.    
-0001ddb0: 2020 2020 2020 2020 5f66 6974 5f76 6172          _fit_var
-0001ddc0: 7320 3d20 6469 6374 2829 0a20 2020 2020  s = dict().     
-0001ddd0: 2020 2020 2020 205f 6669 785f 7661 7273         _fix_vars
-0001dde0: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-0001ddf0: 2020 2020 2020 6966 2065 6e61 626c 6564        if enabled
-0001de00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001de10: 2020 6d6f 6465 6c20 3d20 6c6e 616d 655f    model = lname_
-0001de20: 746f 5f6d 6f64 656c 5b6d 6f64 656c 6e61  to_model[modelna
-0001de30: 6d65 5d0a 2020 2020 2020 2020 2020 2020  me].            
-0001de40: 2020 2020 666f 7220 6e61 6d65 2069 6e20      for name in 
-0001de50: 6d6f 6465 6c2e 5041 524e 414d 4553 3a0a  model.PARNAMES:.
-0001de60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001de70: 2020 2020 6966 2073 656c 662e 7573 656c      if self.usel
-0001de80: 2e66 6974 5b6e 616d 655d 3a0a 2020 2020  .fit[name]:.    
+0001dab0: 2020 2020 7365 6c66 2e64 6566 6175 6c74      self.default
+0001dac0: 735b 6d6f 6465 6c2e 4e41 4d45 5d5b 7061  s[model.NAME][pa
+0001dad0: 726e 616d 655d 5b27 7661 6c69 6e69 7427  rname]['valinit'
+0001dae0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0001daf0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0001db00: 2020 2020 7365 6c66 2e77 6964 6765 7464      self.widgetd
+0001db10: 6963 745b 6d6f 6465 6c6e 616d 655d 5b70  ict[modelname][p
+0001db20: 6172 6e61 6d65 5d5b 2766 665f 746f 6767  arname]['ff_togg
+0001db30: 6c65 275d 2e73 6574 5465 7874 280a 2020  le'].setText(.  
+0001db40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001db50: 2020 2746 7265 6527 0a20 2020 2020 2020    'Free'.       
+0001db60: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+0001db70: 2020 2020 2320 5265 6d6f 7665 2074 6f74      # Remove tot
+0001db80: 616c 206d 6f64 656c 2070 6c6f 740a 2020  al model plot.  
+0001db90: 2020 2020 2020 7365 6c66 2e70 6c6f 745f        self.plot_
+0001dba0: 7769 6467 6574 2e72 656d 6f76 6549 7465  widget.removeIte
+0001dbb0: 6d28 7365 6c66 2e74 6f74 290a 0a20 2020  m(self.tot)..   
+0001dbc0: 2020 2020 2072 6574 7572 6e0a 0a20 2020       return..   
+0001dbd0: 2064 6566 2066 6974 2873 656c 6629 3a0a   def fit(self):.
+0001dbe0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+0001dbf0: 2020 2020 4361 6c6c 6261 636b 2066 6f72      Callback for
+0001dc00: 2046 6974 2062 7574 746f 6e2e 0a20 2020   Fit button..   
+0001dc10: 2020 2020 2043 6f6c 6c65 6374 7320 7661       Collects va
+0001dc20: 7269 6162 6c65 2076 616c 7565 7320 6f66  riable values of
+0001dc30: 2065 6163 6820 6d6f 6465 6c20 616e 6420   each model and 
+0001dc40: 6173 7365 6d62 6c65 7320 696e 746f 2066  assembles into f
+0001dc50: 6974 2f66 6978 0a20 2020 2020 2020 2064  it/fix.        d
+0001dc60: 6963 7469 6f6e 6172 6965 732c 2074 6865  ictionaries, the
+0001dc70: 6e20 636c 6f73 6573 2074 6865 2077 696e  n closes the win
+0001dc80: 646f 772e 0a20 2020 2020 2020 2027 2727  dow..        '''
+0001dc90: 0a0a 2020 2020 2020 2020 6c6e 616d 655f  ..        lname_
+0001dca0: 746f 5f6d 6f64 656c 203d 207b 0a20 2020  to_model = {.   
+0001dcb0: 2020 2020 2020 2020 206d 6f64 656c 2e4e           model.N
+0001dcc0: 414d 452e 6c6f 7765 7228 293a 206d 6f64  AME.lower(): mod
+0001dcd0: 656c 0a20 2020 2020 2020 2020 2020 2066  el.            f
+0001dce0: 6f72 206d 6f64 656c 2069 6e20 7365 6c66  or model in self
+0001dcf0: 2e73 7570 706f 7274 6564 5f6d 6f64 656c  .supported_model
+0001dd00: 730a 2020 2020 2020 2020 7d0a 0a20 2020  s.        }..   
+0001dd10: 2020 2020 2023 2043 6f6c 6c65 6374 2076       # Collect v
+0001dd20: 6172 6961 626c 6573 206f 6620 6561 6368  ariables of each
+0001dd30: 206d 6f64 656c 2c20 6966 2074 6861 7420   model, if that 
+0001dd40: 6d6f 6465 6c20 6973 2065 6e61 626c 6564  model is enabled
+0001dd50: 0a20 2020 2020 2020 2023 2061 6e64 2061  .        # and a
+0001dd60: 7373 6967 6e20 746f 2066 6974 206f 7220  ssign to fit or 
+0001dd70: 6669 780a 2020 2020 2020 2020 666f 7220  fix.        for 
+0001dd80: 6d6f 6465 6c6e 616d 652c 2065 6e61 626c  modelname, enabl
+0001dd90: 6564 2069 6e20 7365 6c66 2e75 7365 6c2e  ed in self.usel.
+0001dda0: 6d6f 6465 6c73 2e69 7465 6d73 2829 3a0a  models.items():.
+0001ddb0: 2020 2020 2020 2020 2020 2020 5f66 6974              _fit
+0001ddc0: 5f76 6172 7320 3d20 6469 6374 2829 0a20  _vars = dict(). 
+0001ddd0: 2020 2020 2020 2020 2020 205f 6669 785f             _fix_
+0001dde0: 7661 7273 203d 2064 6963 7428 290a 2020  vars = dict().  
+0001ddf0: 2020 2020 2020 2020 2020 6966 2065 6e61            if ena
+0001de00: 626c 6564 3a0a 2020 2020 2020 2020 2020  bled:.          
+0001de10: 2020 2020 2020 6d6f 6465 6c20 3d20 6c6e        model = ln
+0001de20: 616d 655f 746f 5f6d 6f64 656c 5b6d 6f64  ame_to_model[mod
+0001de30: 656c 6e61 6d65 5d0a 2020 2020 2020 2020  elname].        
+0001de40: 2020 2020 2020 2020 666f 7220 6e61 6d65          for name
+0001de50: 2069 6e20 6d6f 6465 6c2e 5041 524e 414d   in model.PARNAM
+0001de60: 4553 3a0a 2020 2020 2020 2020 2020 2020  ES:.            
+0001de70: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0001de80: 7573 656c 2e66 6974 5b6e 616d 655d 3a0a  usel.fit[name]:.
 0001de90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dea0: 2020 2020 5f66 6974 5f76 6172 735b 6e61      _fit_vars[na
-0001deb0: 6d65 5d20 3d20 6765 7461 7474 7228 7365  me] = getattr(se
-0001dec0: 6c66 2e70 6172 7374 6f72 652c 206e 616d  lf.parstore, nam
-0001ded0: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-0001dee0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0001def0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001df00: 2020 2020 205f 6669 785f 7661 7273 5b6e       _fix_vars[n
-0001df10: 616d 655d 203d 2067 6574 6174 7472 2873  ame] = getattr(s
-0001df20: 656c 662e 7061 7273 746f 7265 2c20 6e61  elf.parstore, na
-0001df30: 6d65 290a 0a20 2020 2020 2020 2020 2020  me)..           
-0001df40: 2020 2020 2073 656c 662e 7573 656c 2e66       self.usel.f
-0001df50: 6974 5f76 6172 732e 6170 7065 6e64 285f  it_vars.append(_
-0001df60: 6669 745f 7661 7273 290a 2020 2020 2020  fit_vars).      
-0001df70: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-0001df80: 7365 6c2e 6669 785f 7661 7273 2e61 7070  sel.fix_vars.app
-0001df90: 656e 6428 5f66 6978 5f76 6172 7329 0a0a  end(_fix_vars)..
-0001dfa0: 2020 2020 2020 2020 2320 5365 7420 2768          # Set 'h
-0001dfb0: 6173 2070 726f 6772 616d 2062 6565 6e20  as program been 
-0001dfc0: 6578 6974 6564 2720 666c 6167 2074 6f20  exited' flag to 
-0001dfd0: 6661 6c73 650a 2020 2020 2020 2020 7365  false.        se
-0001dfe0: 6c66 2e75 7365 6c2e 6578 6974 6564 203d  lf.usel.exited =
-0001dff0: 2046 616c 7365 0a0a 2020 2020 2020 2020   False..        
-0001e000: 2320 436c 6f73 6520 7468 6520 7769 6e64  # Close the wind
-0001e010: 6f77 0a20 2020 2020 2020 2073 656c 662e  ow.        self.
-0001e020: 636c 6f73 6528 290a 2020 2020 2020 2020  close().        
-0001e030: 7265 7475 726e 0a0a 2020 2020 6465 6620  return..    def 
-0001e040: 7570 6461 7465 5f6d 6f64 656c 706c 6f74  update_modelplot
-0001e050: 2873 656c 662c 2076 616c 7565 2c20 7061  (self, value, pa
-0001e060: 726e 616d 652c 206d 6f64 656c 3a20 4c6f  rname, model: Lo
-0001e070: 6754 6175 544d 6f64 656c 293a 0a0a 2020  gTauTModel):..  
-0001e080: 2020 2020 2020 2320 5365 7420 6e65 7720        # Set new 
-0001e090: 7061 7261 6d65 7465 7220 7661 6c75 650a  parameter value.
-0001e0a0: 2020 2020 2020 2020 7365 7461 7474 7228          setattr(
-0001e0b0: 7365 6c66 2e70 6172 7374 6f72 652c 2070  self.parstore, p
-0001e0c0: 6172 6e61 6d65 2c20 666c 6f61 7428 7661  arname, float(va
-0001e0d0: 6c75 6529 290a 0a20 2020 2020 2020 2070  lue))..        p
-0001e0e0: 6172 616d 6574 6572 7320 3d20 6d6f 6465  arameters = mode
-0001e0f0: 6c2e 7365 745f 696e 6974 6961 6c5f 7661  l.set_initial_va
-0001e100: 6c73 280a 2020 2020 2020 2020 2020 2020  ls(.            
-0001e110: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-0001e120: 2020 7061 726e 616d 653a 2067 6574 6174    parname: getat
-0001e130: 7472 2873 656c 662e 7061 7273 746f 7265  tr(self.parstore
-0001e140: 2c20 7061 726e 616d 6529 0a20 2020 2020  , parname).     
-0001e150: 2020 2020 2020 2020 2020 2066 6f72 2070             for p
-0001e160: 6172 6e61 6d65 2069 6e20 6d6f 6465 6c2e  arname in model.
-0001e170: 5041 524e 414d 4553 0a20 2020 2020 2020  PARNAMES.       
-0001e180: 2020 2020 207d 0a20 2020 2020 2020 2029       }.        )
-0001e190: 0a0a 2020 2020 2020 2020 6e65 775f 7261  ..        new_ra
-0001e1a0: 7465 7320 3d20 3130 2a2a 6d6f 6465 6c2e  tes = 10**model.
-0001e1b0: 6d6f 6465 6c28 7061 7261 6d65 7465 7273  model(parameters
-0001e1c0: 2c20 7365 6c66 2e78 5f67 7269 6429 0a0a  , self.x_grid)..
-0001e1d0: 2020 2020 2020 2020 5f70 6c6f 7420 3d20          _plot = 
-0001e1e0: 7365 6c66 2e6d 6f64 656c 5f70 6c6f 7473  self.model_plots
-0001e1f0: 5b6d 6f64 656c 2e4e 414d 452e 6c6f 7765  [model.NAME.lowe
-0001e200: 7228 295d 0a20 2020 2020 2020 205f 706c  r()].        _pl
-0001e210: 6f74 2e73 6574 4461 7461 2873 656c 662e  ot.setData(self.
-0001e220: 785f 6772 6964 202b 2073 656c 662e 6c6f  x_grid + self.lo
-0001e230: 6773 6869 6674 2c20 6e65 775f 7261 7465  gshift, new_rate
-0001e240: 7329 0a0a 2020 2020 2020 2020 2320 5570  s)..        # Up
-0001e250: 6461 7465 2074 6f74 616c 2070 6c6f 7420  date total plot 
-0001e260: 6173 2073 756d 206f 6620 616c 6c20 6d6f  as sum of all mo
-0001e270: 6465 6c73 0a20 2020 2020 2020 2023 2075  dels.        # u
-0001e280: 7365 2079 6461 7461 206f 6620 6561 6368  se ydata of each
-0001e290: 206d 6f64 656c 0a20 2020 2020 2020 2074   model.        t
-0001e2a0: 6f74 616c 5f72 6174 6573 203d 206e 702e  otal_rates = np.
-0001e2b0: 7a65 726f 7328 7365 6c66 2e78 5f67 7269  zeros(self.x_gri
-0001e2c0: 642e 7368 6170 6529 0a20 2020 2020 2020  d.shape).       
-0001e2d0: 2074 6f74 616c 5f72 6174 6573 202b 3d20   total_rates += 
-0001e2e0: 6e70 2e73 756d 280a 2020 2020 2020 2020  np.sum(.        
-0001e2f0: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
-0001e300: 2020 2020 2020 5f70 6c6f 742e 7944 6174        _plot.yDat
-0001e310: 610a 2020 2020 2020 2020 2020 2020 2020  a.              
-0001e320: 2020 666f 7220 6e61 6d65 2c20 5f70 6c6f    for name, _plo
-0001e330: 7420 696e 2073 656c 662e 6d6f 6465 6c5f  t in self.model_
-0001e340: 706c 6f74 732e 6974 656d 7328 290a 2020  plots.items().  
-0001e350: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0001e360: 2073 656c 662e 7573 656c 2e6d 6f64 656c   self.usel.model
-0001e370: 735b 6e61 6d65 5d0a 2020 2020 2020 2020  s[name].        
-0001e380: 2020 2020 5d2c 0a20 2020 2020 2020 2020      ],.         
-0001e390: 2020 2061 7869 733d 300a 2020 2020 2020     axis=0.      
-0001e3a0: 2020 290a 2020 2020 2020 2020 7365 6c66    ).        self
-0001e3b0: 2e74 6f74 2e73 6574 4461 7461 2873 656c  .tot.setData(sel
-0001e3c0: 662e 785f 6772 6964 202b 2073 656c 662e  f.x_grid + self.
-0001e3d0: 6c6f 6773 6869 6674 2c20 746f 7461 6c5f  logshift, total_
-0001e3e0: 7261 7465 7329 0a0a 2020 2020 2020 2020  rates)..        
-0001e3f0: 7265 7475 726e 0a0a 2020 2020 6465 6620  return..    def 
-0001e400: 746f 6767 6c65 5f70 6c6f 7428 7365 6c66  toggle_plot(self
-0001e410: 2c20 7661 6c3a 2069 6e74 2c0a 2020 2020  , val: int,.    
+0001dea0: 2020 2020 2020 2020 5f66 6974 5f76 6172          _fit_var
+0001deb0: 735b 6e61 6d65 5d20 3d20 6765 7461 7474  s[name] = getatt
+0001dec0: 7228 7365 6c66 2e70 6172 7374 6f72 652c  r(self.parstore,
+0001ded0: 206e 616d 6529 0a20 2020 2020 2020 2020   name).         
+0001dee0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0001def0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001df00: 2020 2020 2020 2020 205f 6669 785f 7661           _fix_va
+0001df10: 7273 5b6e 616d 655d 203d 2067 6574 6174  rs[name] = getat
+0001df20: 7472 2873 656c 662e 7061 7273 746f 7265  tr(self.parstore
+0001df30: 2c20 6e61 6d65 290a 0a20 2020 2020 2020  , name)..       
+0001df40: 2020 2020 2020 2020 2073 656c 662e 7573           self.us
+0001df50: 656c 2e66 6974 5f76 6172 732e 6170 7065  el.fit_vars.appe
+0001df60: 6e64 285f 6669 745f 7661 7273 290a 2020  nd(_fit_vars).  
+0001df70: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0001df80: 6c66 2e75 7365 6c2e 6669 785f 7661 7273  lf.usel.fix_vars
+0001df90: 2e61 7070 656e 6428 5f66 6978 5f76 6172  .append(_fix_var
+0001dfa0: 7329 0a0a 2020 2020 2020 2020 2320 5365  s)..        # Se
+0001dfb0: 7420 2768 6173 2070 726f 6772 616d 2062  t 'has program b
+0001dfc0: 6565 6e20 6578 6974 6564 2720 666c 6167  een exited' flag
+0001dfd0: 2074 6f20 6661 6c73 650a 2020 2020 2020   to false.      
+0001dfe0: 2020 7365 6c66 2e75 7365 6c2e 6578 6974    self.usel.exit
+0001dff0: 6564 203d 2046 616c 7365 0a0a 2020 2020  ed = False..    
+0001e000: 2020 2020 2320 436c 6f73 6520 7468 6520      # Close the 
+0001e010: 7769 6e64 6f77 0a20 2020 2020 2020 2073  window.        s
+0001e020: 656c 662e 636c 6f73 6528 290a 2020 2020  elf.close().    
+0001e030: 2020 2020 7265 7475 726e 0a0a 2020 2020      return..    
+0001e040: 6465 6620 7570 6461 7465 5f6d 6f64 656c  def update_model
+0001e050: 706c 6f74 2873 656c 662c 2076 616c 7565  plot(self, value
+0001e060: 2c20 7061 726e 616d 652c 206d 6f64 656c  , parname, model
+0001e070: 3a20 4c6f 6754 6175 544d 6f64 656c 293a  : LogTauTModel):
+0001e080: 0a0a 2020 2020 2020 2020 2320 5365 7420  ..        # Set 
+0001e090: 6e65 7720 7061 7261 6d65 7465 7220 7661  new parameter va
+0001e0a0: 6c75 650a 2020 2020 2020 2020 7365 7461  lue.        seta
+0001e0b0: 7474 7228 7365 6c66 2e70 6172 7374 6f72  ttr(self.parstor
+0001e0c0: 652c 2070 6172 6e61 6d65 2c20 666c 6f61  e, parname, floa
+0001e0d0: 7428 7661 6c75 6529 290a 0a20 2020 2020  t(value))..     
+0001e0e0: 2020 2070 6172 616d 6574 6572 7320 3d20     parameters = 
+0001e0f0: 6d6f 6465 6c2e 7365 745f 696e 6974 6961  model.set_initia
+0001e100: 6c5f 7661 6c73 280a 2020 2020 2020 2020  l_vals(.        
+0001e110: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+0001e120: 2020 2020 2020 7061 726e 616d 653a 2067        parname: g
+0001e130: 6574 6174 7472 2873 656c 662e 7061 7273  etattr(self.pars
+0001e140: 746f 7265 2c20 7061 726e 616d 6529 0a20  tore, parname). 
+0001e150: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0001e160: 6f72 2070 6172 6e61 6d65 2069 6e20 6d6f  or parname in mo
+0001e170: 6465 6c2e 5041 524e 414d 4553 0a20 2020  del.PARNAMES.   
+0001e180: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+0001e190: 2020 2029 0a0a 2020 2020 2020 2020 6e65     )..        ne
+0001e1a0: 775f 7261 7465 7320 3d20 3130 2a2a 6d6f  w_rates = 10**mo
+0001e1b0: 6465 6c2e 6d6f 6465 6c28 7061 7261 6d65  del.model(parame
+0001e1c0: 7465 7273 2c20 7365 6c66 2e78 5f67 7269  ters, self.x_gri
+0001e1d0: 6429 0a0a 2020 2020 2020 2020 5f70 6c6f  d)..        _plo
+0001e1e0: 7420 3d20 7365 6c66 2e6d 6f64 656c 5f70  t = self.model_p
+0001e1f0: 6c6f 7473 5b6d 6f64 656c 2e4e 414d 452e  lots[model.NAME.
+0001e200: 6c6f 7765 7228 295d 0a20 2020 2020 2020  lower()].       
+0001e210: 205f 706c 6f74 2e73 6574 4461 7461 2873   _plot.setData(s
+0001e220: 656c 662e 785f 6772 6964 202b 2073 656c  elf.x_grid + sel
+0001e230: 662e 6c6f 6773 6869 6674 2c20 6e65 775f  f.logshift, new_
+0001e240: 7261 7465 7329 0a0a 2020 2020 2020 2020  rates)..        
+0001e250: 2320 5570 6461 7465 2074 6f74 616c 2070  # Update total p
+0001e260: 6c6f 7420 6173 2073 756d 206f 6620 616c  lot as sum of al
+0001e270: 6c20 6d6f 6465 6c73 0a20 2020 2020 2020  l models.       
+0001e280: 2023 2075 7365 2079 6461 7461 206f 6620   # use ydata of 
+0001e290: 6561 6368 206d 6f64 656c 0a20 2020 2020  each model.     
+0001e2a0: 2020 2074 6f74 616c 5f72 6174 6573 203d     total_rates =
+0001e2b0: 206e 702e 7a65 726f 7328 7365 6c66 2e78   np.zeros(self.x
+0001e2c0: 5f67 7269 642e 7368 6170 6529 0a20 2020  _grid.shape).   
+0001e2d0: 2020 2020 2074 6f74 616c 5f72 6174 6573       total_rates
+0001e2e0: 202b 3d20 6e70 2e73 756d 280a 2020 2020   += np.sum(.    
+0001e2f0: 2020 2020 2020 2020 5b0a 2020 2020 2020          [.      
+0001e300: 2020 2020 2020 2020 2020 5f70 6c6f 742e            _plot.
+0001e310: 7944 6174 610a 2020 2020 2020 2020 2020  yData.          
+0001e320: 2020 2020 2020 666f 7220 6e61 6d65 2c20        for name, 
+0001e330: 5f70 6c6f 7420 696e 2073 656c 662e 6d6f  _plot in self.mo
+0001e340: 6465 6c5f 706c 6f74 732e 6974 656d 7328  del_plots.items(
+0001e350: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001e360: 2020 6966 2073 656c 662e 7573 656c 2e6d    if self.usel.m
+0001e370: 6f64 656c 735b 6e61 6d65 5d0a 2020 2020  odels[name].    
+0001e380: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
+0001e390: 2020 2020 2020 2061 7869 733d 300a 2020         axis=0.  
+0001e3a0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0001e3b0: 7365 6c66 2e74 6f74 2e73 6574 4461 7461  self.tot.setData
+0001e3c0: 2873 656c 662e 785f 6772 6964 202b 2073  (self.x_grid + s
+0001e3d0: 656c 662e 6c6f 6773 6869 6674 2c20 746f  elf.logshift, to
+0001e3e0: 7461 6c5f 7261 7465 7329 0a0a 2020 2020  tal_rates)..    
+0001e3f0: 2020 2020 7265 7475 726e 0a0a 2020 2020      return..    
+0001e400: 6465 6620 746f 6767 6c65 5f70 6c6f 7428  def toggle_plot(
+0001e410: 7365 6c66 2c20 7661 6c3a 2069 6e74 2c0a  self, val: int,.
 0001e420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e430: 6d6f 6465 6c3a 204c 6f67 5461 7554 4d6f  model: LogTauTMo
-0001e440: 6465 6c20 7c20 4c6f 6754 6175 484d 6f64  del | LogTauHMod
-0001e450: 656c 2920 2d3e 204e 6f6e 653a 0a20 2020  el) -> None:.   
-0001e460: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-0001e470: 2043 616c 6c62 6163 6b20 666f 7220 746f   Callback for to
-0001e480: 6767 6c69 6e67 206d 6f64 656c 2063 6865  ggling model che
-0001e490: 636b 626f 7865 730a 0a20 2020 2020 2020  ckboxes..       
-0001e4a0: 2043 616c 6375 6c61 7465 7320 6d6f 6465   Calculates mode
-0001e4b0: 6c20 6461 7461 2c20 6164 6473 2f64 656c  l data, adds/del
-0001e4c0: 6574 6573 206c 696e 6520 6672 6f6d 2070  etes line from p
-0001e4d0: 6c6f 740a 2020 2020 2020 2020 616e 6420  lot.        and 
-0001e4e0: 7570 6461 7465 7320 746f 7461 6c20 6d6f  updates total mo
-0001e4f0: 6465 6c20 706c 6f74 0a20 2020 2020 2020  del plot.       
-0001e500: 2027 2727 0a0a 2020 2020 2020 2020 6d6f   '''..        mo
-0001e510: 6465 6c6e 616d 6520 3d20 6d6f 6465 6c2e  delname = model.
-0001e520: 4e41 4d45 2e6c 6f77 6572 2829 0a0a 2020  NAME.lower()..  
-0001e530: 2020 2020 2020 2320 436f 6e76 6572 7420        # Convert 
-0001e540: 7661 6c20 746f 2062 6f6f 6c0a 2020 2020  val to bool.    
-0001e550: 2020 2020 7661 6c20 3d20 626f 6f6c 2876      val = bool(v
-0001e560: 616c 202f 2032 290a 0a20 2020 2020 2020  al / 2)..       
-0001e570: 2023 2055 7064 6174 6520 6c69 7374 206f   # Update list o
-0001e580: 6620 6d6f 6465 6c73 0a20 2020 2020 2020  f models.       
-0001e590: 2073 656c 662e 7573 656c 2e6d 6f64 656c   self.usel.model
-0001e5a0: 735b 6d6f 6465 6c6e 616d 655d 203d 2076  s[modelname] = v
-0001e5b0: 616c 0a0a 2020 2020 2020 2020 2320 5570  al..        # Up
-0001e5c0: 6461 7465 206d 6f64 656c 2076 616c 7565  date model value
-0001e5d0: 7320 616e 6420 706c 6f74 2064 6174 6120  s and plot data 
-0001e5e0: 666f 7220 6561 6368 206d 6f64 656c 2c20  for each model, 
-0001e5f0: 616e 6420 666f 7220 746f 7461 6c0a 2020  and for total.  
-0001e600: 2020 2020 2020 666f 7220 7061 726e 616d        for parnam
-0001e610: 6520 696e 206d 6f64 656c 2e50 4152 4e41  e in model.PARNA
-0001e620: 4d45 533a 0a20 2020 2020 2020 2020 2020  MES:.           
-0001e630: 2073 656c 662e 7570 6461 7465 5f6d 6f64   self.update_mod
-0001e640: 656c 706c 6f74 280a 2020 2020 2020 2020  elplot(.        
-0001e650: 2020 2020 2020 2020 6765 7461 7474 7228          getattr(
-0001e660: 7365 6c66 2e70 6172 7374 6f72 652c 2070  self.parstore, p
-0001e670: 6172 6e61 6d65 292c 0a20 2020 2020 2020  arname),.       
-0001e680: 2020 2020 2020 2020 2070 6172 6e61 6d65           parname
-0001e690: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001e6a0: 2020 6d6f 6465 6c0a 2020 2020 2020 2020    model.        
-0001e6b0: 2020 2020 290a 0a20 2020 2020 2020 2023      )..        #
-0001e6c0: 2053 656c 6563 7420 6d6f 6465 6c20 706c   Select model pl
-0001e6d0: 6f74 2074 6f20 746f 6767 6c65 0a20 2020  ot to toggle.   
-0001e6e0: 2020 2020 205f 706c 6f74 203d 2073 656c       _plot = sel
-0001e6f0: 662e 6d6f 6465 6c5f 706c 6f74 735b 6d6f  f.model_plots[mo
-0001e700: 6465 6c6e 616d 655d 0a0a 2020 2020 2020  delname]..      
-0001e710: 2020 2320 4164 6420 6261 636b 2069 6e20    # Add back in 
-0001e720: 706c 6f74 0a20 2020 2020 2020 2069 6620  plot.        if 
-0001e730: 7661 6c3a 0a20 2020 2020 2020 2020 2020  val:.           
-0001e740: 2073 656c 662e 706c 6f74 5f77 6964 6765   self.plot_widge
-0001e750: 742e 7265 6d6f 7665 4974 656d 285f 706c  t.removeItem(_pl
-0001e760: 6f74 290a 2020 2020 2020 2020 2020 2020  ot).            
-0001e770: 7365 6c66 2e70 6c6f 745f 7769 6467 6574  self.plot_widget
-0001e780: 2e61 6464 4974 656d 285f 706c 6f74 290a  .addItem(_plot).
-0001e790: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0001e7a0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-0001e7b0: 6c6f 745f 7769 6467 6574 2e72 656d 6f76  lot_widget.remov
-0001e7c0: 6549 7465 6d28 5f70 6c6f 7429 0a0a 2020  eItem(_plot)..  
-0001e7d0: 2020 2020 2020 2320 456e 6162 6c65 2074        # Enable t
-0001e7e0: 6f74 616c 2070 6c6f 7420 6966 203e 2031  otal plot if > 1
-0001e7f0: 206d 6f64 656c 0a20 2020 2020 2020 2023   model.        #
-0001e800: 2061 6e64 2065 6e61 626c 6520 6669 7420   and enable fit 
-0001e810: 6275 7474 6f6e 2069 6620 3e20 3020 6d6f  button if > 0 mo
-0001e820: 6465 6c73 0a20 2020 2020 2020 206e 5f6d  dels.        n_m
-0001e830: 6f64 656c 7320 3d20 6e70 2e73 756d 285b  odels = np.sum([
-0001e840: 7661 6c20 666f 7220 7661 6c20 696e 2073  val for val in s
-0001e850: 656c 662e 7573 656c 2e6d 6f64 656c 732e  elf.usel.models.
-0001e860: 7661 6c75 6573 2829 5d29 0a20 2020 2020  values()]).     
-0001e870: 2020 2069 6620 6e5f 6d6f 6465 6c73 203d     if n_models =
-0001e880: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-0001e890: 2073 656c 662e 6669 745f 6274 6e5f 7769   self.fit_btn_wi
-0001e8a0: 6467 6574 2e73 6574 456e 6162 6c65 6428  dget.setEnabled(
-0001e8b0: 4661 6c73 6529 0a20 2020 2020 2020 2065  False).        e
-0001e8c0: 6c69 6620 6e5f 6d6f 6465 6c73 203d 3d20  lif n_models == 
-0001e8d0: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
-0001e8e0: 656c 662e 6669 745f 6274 6e5f 7769 6467  elf.fit_btn_widg
-0001e8f0: 6574 2e73 6574 456e 6162 6c65 6428 5472  et.setEnabled(Tr
-0001e900: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
-0001e910: 7365 6c66 2e70 6c6f 745f 7769 6467 6574  self.plot_widget
-0001e920: 2e72 656d 6f76 6549 7465 6d28 7365 6c66  .removeItem(self
-0001e930: 2e74 6f74 290a 2020 2020 2020 2020 656c  .tot).        el
-0001e940: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0001e950: 7365 6c66 2e66 6974 5f62 746e 5f77 6964  self.fit_btn_wid
-0001e960: 6765 742e 7365 7445 6e61 626c 6564 2854  get.setEnabled(T
-0001e970: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
-0001e980: 2073 656c 662e 706c 6f74 5f77 6964 6765   self.plot_widge
-0001e990: 742e 7265 6d6f 7665 4974 656d 2873 656c  t.removeItem(sel
-0001e9a0: 662e 746f 7429 0a20 2020 2020 2020 2020  f.tot).         
-0001e9b0: 2020 2073 656c 662e 706c 6f74 5f77 6964     self.plot_wid
-0001e9c0: 6765 742e 6164 6449 7465 6d28 7365 6c66  get.addItem(self
-0001e9d0: 2e74 6f74 290a 0a20 2020 2020 2020 2023  .tot)..        #
-0001e9e0: 2045 6e61 626c 652f 4469 7361 626c 6520   Enable/Disable 
-0001e9f0: 736c 6964 6572 2c20 6368 6563 6b62 6f78  slider, checkbox
-0001ea00: 2c20 616e 6420 6669 7466 6978 0a20 2020  , and fitfix.   
-0001ea10: 2020 2020 2066 6f72 2070 6172 6e61 6d65       for parname
-0001ea20: 2069 6e20 6d6f 6465 6c2e 5041 524e 414d   in model.PARNAM
-0001ea30: 4553 3a0a 2020 2020 2020 2020 2020 2020  ES:.            
-0001ea40: 7365 6c66 2e77 6964 6765 7464 6963 745b  self.widgetdict[
-0001ea50: 6d6f 6465 6c6e 616d 655d 5b70 6172 6e61  modelname][parna
-0001ea60: 6d65 5d5b 2773 6c69 6465 7227 5d2e 7365  me]['slider'].se
-0001ea70: 7445 6e61 626c 6564 2876 616c 290a 2020  tEnabled(val).  
-0001ea80: 2020 2020 2020 2020 2020 7365 6c66 2e77            self.w
-0001ea90: 6964 6765 7464 6963 745b 6d6f 6465 6c6e  idgetdict[modeln
-0001eaa0: 616d 655d 5b70 6172 6e61 6d65 5d5b 2765  ame][parname]['e
-0001eab0: 6e74 7279 275d 2e73 6574 456e 6162 6c65  ntry'].setEnable
-0001eac0: 6428 7661 6c29 0a20 2020 2020 2020 2020  d(val).         
-0001ead0: 2020 2073 656c 662e 7769 6467 6574 6469     self.widgetdi
-0001eae0: 6374 5b6d 6f64 656c 6e61 6d65 5d5b 7061  ct[modelname][pa
-0001eaf0: 726e 616d 655d 5b27 6666 5f74 6f67 676c  rname]['ff_toggl
-0001eb00: 6527 5d2e 7365 7445 6e61 626c 6564 2876  e'].setEnabled(v
-0001eb10: 616c 290a 0a20 2020 2020 2020 2072 6574  al)..        ret
-0001eb20: 7572 6e0a 0a20 2020 2064 6566 206d 616b  urn..    def mak
-0001eb30: 655f 6d6f 6465 6c62 6f78 2873 656c 662c  e_modelbox(self,
-0001eb40: 206d 6f64 656c 3a20 4c6f 6754 6175 544d   model: LogTauTM
-0001eb50: 6f64 656c 2c20 7061 7265 6e74 2c20 696e  odel, parent, in
-0001eb60: 6465 783a 2069 6e74 293a 0a20 2020 2020  dex: int):.     
-0001eb70: 2020 2027 2727 0a20 2020 2020 2020 2043     '''.        C
-0001eb80: 7265 6174 6573 2077 6964 6765 7420 666f  reates widget fo
-0001eb90: 7220 6120 6769 7665 6e20 6d6f 6465 6c2c  r a given model,
-0001eba0: 2063 6f6e 7461 696e 696e 6720 6120 6368   containing a ch
-0001ebb0: 6563 6b62 6f78 2074 6f20 746f 6767 6c65  eckbox to toggle
-0001ebc0: 0a20 2020 2020 2020 2074 6865 206d 6f64  .        the mod
-0001ebd0: 656c 2c20 616e 6420 6120 726f 7720 6f66  el, and a row of
-0001ebe0: 2069 6e74 6572 6163 7469 7665 2077 6964   interactive wid
-0001ebf0: 6765 7473 2066 6f72 2065 6163 6820 7061  gets for each pa
-0001ec00: 7261 6d65 7465 7220 6f66 2074 6865 0a20  rameter of the. 
-0001ec10: 2020 2020 2020 206d 6f64 656c 0a20 2020         model.   
-0001ec20: 2020 2020 2027 2727 0a0a 2020 2020 2020       '''..      
-0001ec30: 2020 2320 5769 6467 6574 2066 6f72 2074    # Widget for t
-0001ec40: 6869 7320 6d6f 6465 6c0a 2020 2020 2020  his model.      
-0001ec50: 2020 6d6f 6465 6c5f 7769 6467 6574 203d    model_widget =
-0001ec60: 2051 7457 6964 6765 7473 2e51 5769 6467   QtWidgets.QWidg
-0001ec70: 6574 2870 6172 656e 743d 7061 7265 6e74  et(parent=parent
-0001ec80: 290a 2020 2020 2020 2020 6d6f 6465 6c5f  ).        model_
-0001ec90: 6c61 796f 7574 203d 2051 7457 6964 6765  layout = QtWidge
-0001eca0: 7473 2e51 4842 6f78 4c61 796f 7574 286d  ts.QHBoxLayout(m
-0001ecb0: 6f64 656c 5f77 6964 6765 7429 0a0a 2020  odel_widget)..  
-0001ecc0: 2020 2020 2020 2320 4372 6561 7465 2074        # Create t
-0001ecd0: 6963 6b62 6f78 2074 6f20 746f 6767 6c65  ickbox to toggle
-0001ece0: 2074 6869 7320 7769 6467 6574 0a20 2020   this widget.   
-0001ecf0: 2020 2020 2074 6963 6b62 6f78 5f77 6964       tickbox_wid
-0001ed00: 6765 7420 3d20 5174 5769 6467 6574 732e  get = QtWidgets.
-0001ed10: 5143 6865 636b 426f 7828 0a20 2020 2020  QCheckBox(.     
-0001ed20: 2020 2020 2020 2070 6172 656e 743d 6d6f         parent=mo
-0001ed30: 6465 6c5f 7769 6467 6574 2c0a 2020 2020  del_widget,.    
-0001ed40: 2020 2020 2020 2020 7465 7874 3d6d 6f64          text=mod
-0001ed50: 656c 2e4e 414d 452e 7265 706c 6163 6528  el.NAME.replace(
-0001ed60: 2742 726f 6e73 2d56 616e 2d56 6c65 636b  'Brons-Van-Vleck
-0001ed70: 272c 2027 4256 5627 292c 0a0a 2020 2020  ', 'BVV'),..    
-0001ed80: 2020 2020 290a 0a20 2020 2020 2020 2023      )..        #
-0001ed90: 2041 6464 2074 6963 6b62 6f78 2074 6f20   Add tickbox to 
-0001eda0: 7468 6973 206d 6f64 656c 0a20 2020 2020  this model.     
-0001edb0: 2020 206d 6f64 656c 5f6c 6179 6f75 742e     model_layout.
-0001edc0: 6164 6457 6964 6765 7428 7469 636b 626f  addWidget(tickbo
-0001edd0: 785f 7769 6467 6574 290a 0a20 2020 2020  x_widget)..     
-0001ede0: 2020 2023 2041 6464 2074 6f20 6469 6374     # Add to dict
-0001edf0: 696f 6e61 7279 206f 6620 616c 6c20 7469  ionary of all ti
-0001ee00: 636b 626f 7865 732c 2069 6e64 6578 6564  ckboxes, indexed
-0001ee10: 2062 7920 6d6f 6465 6c2e 4e41 4d45 2e6c   by model.NAME.l
-0001ee20: 6f77 6572 2829 0a20 2020 2020 2020 2073  ower().        s
-0001ee30: 656c 662e 7469 636b 6469 6374 5b6d 6f64  elf.tickdict[mod
-0001ee40: 656c 2e4e 414d 452e 6c6f 7765 7228 295d  el.NAME.lower()]
-0001ee50: 203d 2074 6963 6b62 6f78 5f77 6964 6765   = tickbox_widge
-0001ee60: 740a 0a20 2020 2020 2020 2023 2057 6865  t..        # Whe
-0001ee70: 6e20 746f 6767 6c65 642c 2070 6c6f 7420  n toggled, plot 
-0001ee80: 7468 6973 206d 6f64 656c 0a20 2020 2020  this model.     
-0001ee90: 2020 2074 6963 6b62 6f78 5f77 6964 6765     tickbox_widge
-0001eea0: 742e 7374 6174 6543 6861 6e67 6564 2e63  t.stateChanged.c
-0001eeb0: 6f6e 6e65 6374 280a 2020 2020 2020 2020  onnect(.        
-0001eec0: 2020 2020 6c61 6d62 6461 2076 616c 3a20      lambda val: 
-0001eed0: 7365 6c66 2e74 6f67 676c 655f 706c 6f74  self.toggle_plot
-0001eee0: 2876 616c 2c20 6d6f 6465 6c29 0a20 2020  (val, model).   
-0001eef0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-0001ef00: 2320 4164 6420 6162 696c 6974 7920 746f  # Add ability to
-0001ef10: 2074 6f67 676c 6520 6d6f 6465 6c20 7573   toggle model us
-0001ef20: 696e 6720 6e75 6d62 6572 206b 6579 0a20  ing number key. 
-0001ef30: 2020 2020 2020 206f 6e5f 6f66 665f 7368         on_off_sh
-0001ef40: 6f72 7463 7574 203d 2051 7457 6964 6765  ortcut = QtWidge
-0001ef50: 7473 2e51 5368 6f72 7463 7574 280a 2020  ts.QShortcut(.  
-0001ef60: 2020 2020 2020 2020 2020 5174 4775 692e            QtGui.
-0001ef70: 514b 6579 5365 7175 656e 6365 2827 7b3a  QKeySequence('{:
-0001ef80: 647d 272e 666f 726d 6174 2869 6e64 6578  d}'.format(index
-0001ef90: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
-0001efa0: 7365 6c66 0a20 2020 2020 2020 2029 0a20  self.        ). 
-0001efb0: 2020 2020 2020 206f 6e5f 6f66 665f 7368         on_off_sh
-0001efc0: 6f72 7463 7574 2e61 6374 6976 6174 6564  ortcut.activated
-0001efd0: 2e63 6f6e 6e65 6374 280a 2020 2020 2020  .connect(.      
-0001efe0: 2020 2020 2020 6c61 6d62 6461 3a20 7469        lambda: ti
-0001eff0: 636b 626f 785f 7769 6467 6574 2e74 6f67  ckbox_widget.tog
-0001f000: 676c 6528 290a 2020 2020 2020 2020 290a  gle().        ).
-0001f010: 2020 2020 2020 2020 7365 6c66 2e6f 6e5f          self.on_
-0001f020: 6f66 665f 7368 6f72 7463 7574 2e61 7070  off_shortcut.app
-0001f030: 656e 6428 6f6e 5f6f 6666 5f73 686f 7274  end(on_off_short
-0001f040: 6375 7429 0a0a 2020 2020 2020 2020 2320  cut)..        # 
-0001f050: 4372 6561 7465 2063 6f6e 7461 696e 6572  Create container
-0001f060: 2077 6964 6765 7420 666f 7220 616c 6c20   widget for all 
-0001f070: 7061 7261 6d65 7465 7220 726f 7773 0a20  parameter rows. 
-0001f080: 2020 2020 2020 2072 6873 5f77 6964 6765         rhs_widge
-0001f090: 7420 3d20 5174 5769 6467 6574 732e 5157  t = QtWidgets.QW
-0001f0a0: 6964 6765 7428 7061 7265 6e74 3d6d 6f64  idget(parent=mod
-0001f0b0: 656c 5f77 6964 6765 7429 0a20 2020 2020  el_widget).     
-0001f0c0: 2020 2072 6873 5f6c 6179 6f75 7420 3d20     rhs_layout = 
-0001f0d0: 5174 5769 6467 6574 732e 5156 426f 784c  QtWidgets.QVBoxL
-0001f0e0: 6179 6f75 7428 7268 735f 7769 6467 6574  ayout(rhs_widget
-0001f0f0: 290a 0a20 2020 2020 2020 2023 204d 616b  )..        # Mak
-0001f100: 6520 736c 6964 6572 2c20 7465 7874 626f  e slider, textbo
-0001f110: 782c 2061 6e64 2066 6974 2f66 6978 2074  x, and fit/fix t
-0001f120: 6f67 676c 6520 666f 7220 6561 6368 0a20  oggle for each. 
-0001f130: 2020 2020 2020 2023 2070 6172 616d 6574         # paramet
-0001f140: 6572 206f 6620 7468 6520 6375 7272 656e  er of the curren
-0001f150: 7420 6d6f 6465 6c0a 2020 2020 2020 2020  t model.        
-0001f160: 666f 7220 7061 726e 616d 6520 696e 206d  for parname in m
-0001f170: 6f64 656c 2e50 4152 4e41 4d45 533a 0a0a  odel.PARNAMES:..
-0001f180: 2020 2020 2020 2020 2020 2020 2320 4465              # De
-0001f190: 6661 756c 7420 7061 7261 6d65 7465 7220  fault parameter 
-0001f1a0: 7661 6c75 6573 0a20 2020 2020 2020 2020  values.         
-0001f1b0: 2020 205f 6465 6661 756c 7473 203d 2073     _defaults = s
-0001f1c0: 656c 662e 6465 6661 756c 7473 5b6d 6f64  elf.defaults[mod
-0001f1d0: 656c 2e4e 414d 455d 5b70 6172 6e61 6d65  el.NAME][parname
-0001f1e0: 5d0a 0a20 2020 2020 2020 2020 2020 2023  ]..            #
-0001f1f0: 204e 616d 6520 616e 6420 556e 6974 7320   Name and Units 
-0001f200: 6173 2073 7472 696e 670a 2020 2020 2020  as string.      
-0001f210: 2020 2020 2020 5f6e 755f 7374 7269 6e67        _nu_string
-0001f220: 203d 2027 7b7d 2028 7b7d 2927 2e66 6f72   = '{} ({})'.for
-0001f230: 6d61 7428 0a20 2020 2020 2020 2020 2020  mat(.           
-0001f240: 2020 2020 206d 6f64 656c 2e56 4152 4e41       model.VARNA
-0001f250: 4d45 535f 4854 4d4c 5b70 6172 6e61 6d65  MES_HTML[parname
-0001f260: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-0001f270: 2020 206d 6f64 656c 2e55 4e49 5453 5f48     model.UNITS_H
-0001f280: 544d 4c5b 7061 726e 616d 655d 0a20 2020  TML[parname].   
-0001f290: 2020 2020 2020 2020 2029 2e72 6570 6c61           ).repla
-0001f2a0: 6365 2827 2829 272c 2027 2729 0a0a 2020  ce('()', '')..  
-0001f2b0: 2020 2020 2020 2020 2020 2320 4361 6c6c            # Call
-0001f2c0: 6261 636b 2066 6f72 2069 6e74 6572 6163  back for interac
-0001f2d0: 7469 6f6e 2077 6974 6820 736c 6964 6572  tion with slider
-0001f2e0: 2c20 7465 7874 626f 782e 2e2e 0a20 2020  , textbox....   
-0001f2f0: 2020 2020 2020 2020 2063 6220 3d20 7061           cb = pa
-0001f300: 7274 6961 6c28 7365 6c66 2e75 7064 6174  rtial(self.updat
-0001f310: 655f 6d6f 6465 6c70 6c6f 742c 206d 6f64  e_modelplot, mod
-0001f320: 656c 3d6d 6f64 656c 2c20 7061 726e 616d  el=model, parnam
-0001f330: 653d 7061 726e 616d 6529 0a0a 2020 2020  e=parname)..    
-0001f340: 2020 2020 2020 2020 2320 4d61 6b65 2072          # Make r
-0001f350: 6f77 206f 6620 7769 6467 6574 7320 666f  ow of widgets fo
-0001f360: 7220 7468 6973 2070 6172 616d 6574 6572  r this parameter
-0001f370: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
-0001f380: 626f 785f 7769 6467 6574 2c20 7061 7262  box_widget, parb
-0001f390: 6f78 5f6c 6179 6f75 7420 3d20 7365 6c66  ox_layout = self
-0001f3a0: 2e6d 616b 655f 7061 7262 6f78 280a 2020  .make_parbox(.  
-0001f3b0: 2020 2020 2020 2020 2020 2020 2020 6362                cb
-0001f3c0: 2c20 7061 726e 616d 652c 205f 6e75 5f73  , parname, _nu_s
-0001f3d0: 7472 696e 672c 205f 6465 6661 756c 7473  tring, _defaults
-0001f3e0: 2c20 6d6f 6465 6c5f 7769 6467 6574 2c0a  , model_widget,.
-0001f3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f400: 6d6f 6465 6c2e 4e41 4d45 2e6c 6f77 6572  model.NAME.lower
-0001f410: 2829 0a20 2020 2020 2020 2020 2020 2029  ().            )
-0001f420: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-0001f430: 616e 6420 6164 6420 746f 2074 6865 206d  and add to the m
-0001f440: 6f64 656c 2773 2062 6f78 206f 6620 7061  odel's box of pa
-0001f450: 7261 6d65 7465 720a 2020 2020 2020 2020  rameter.        
-0001f460: 2020 2020 7268 735f 6c61 796f 7574 2e61      rhs_layout.a
-0001f470: 6464 5769 6467 6574 2870 6172 626f 785f  ddWidget(parbox_
-0001f480: 7769 6467 6574 290a 0a20 2020 2020 2020  widget)..       
-0001f490: 2023 2053 6574 2065 7870 616e 7369 6f6e   # Set expansion
-0001f4a0: 2062 6568 6176 696f 7572 2061 6e64 2063   behaviour and c
-0001f4b0: 656e 7465 7269 6e67 206f 6620 7769 6467  entering of widg
-0001f4c0: 6574 730a 2020 2020 2020 2020 7268 735f  ets.        rhs_
-0001f4d0: 6c61 796f 7574 2e73 6574 416c 6967 6e6d  layout.setAlignm
-0001f4e0: 656e 7428 5174 436f 7265 2e51 742e 416c  ent(QtCore.Qt.Al
-0001f4f0: 6967 6e56 4365 6e74 6572 290a 2020 2020  ignVCenter).    
-0001f500: 2020 2020 7268 735f 7769 6467 6574 2e73      rhs_widget.s
-0001f510: 6574 5369 7a65 506f 6c69 6379 280a 2020  etSizePolicy(.  
-0001f520: 2020 2020 2020 2020 2020 5174 5769 6467            QtWidg
-0001f530: 6574 732e 5153 697a 6550 6f6c 6963 792e  ets.QSizePolicy.
-0001f540: 4669 7865 642c 0a20 2020 2020 2020 2020  Fixed,.         
-0001f550: 2020 2051 7457 6964 6765 7473 2e51 5369     QtWidgets.QSi
-0001f560: 7a65 506f 6c69 6379 2e46 6978 6564 0a20  zePolicy.Fixed. 
-0001f570: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0001f580: 2074 6963 6b62 6f78 5f77 6964 6765 742e   tickbox_widget.
-0001f590: 7365 7453 697a 6550 6f6c 6963 7928 0a20  setSizePolicy(. 
-0001f5a0: 2020 2020 2020 2020 2020 2051 7457 6964             QtWid
-0001f5b0: 6765 7473 2e51 5369 7a65 506f 6c69 6379  gets.QSizePolicy
-0001f5c0: 2e46 6978 6564 2c0a 2020 2020 2020 2020  .Fixed,.        
-0001f5d0: 2020 2020 5174 5769 6467 6574 732e 5153      QtWidgets.QS
-0001f5e0: 697a 6550 6f6c 6963 792e 4669 7865 640a  izePolicy.Fixed.
-0001f5f0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-0001f600: 2020 2072 6873 5f6c 6179 6f75 742e 7365     rhs_layout.se
-0001f610: 7453 7061 6369 6e67 2830 290a 2020 2020  tSpacing(0).    
-0001f620: 2020 2020 7268 735f 6c61 796f 7574 2e61      rhs_layout.a
-0001f630: 6464 5374 7265 7463 6828 3429 0a0a 2020  ddStretch(4)..  
-0001f640: 2020 2020 2020 2320 4164 6420 7061 7261        # Add para
-0001f650: 6d65 7465 7220 726f 7773 2074 6f20 7468  meter rows to th
-0001f660: 6973 206d 6f64 656c 0a20 2020 2020 2020  is model.       
-0001f670: 206d 6f64 656c 5f6c 6179 6f75 742e 6164   model_layout.ad
-0001f680: 6457 6964 6765 7428 7268 735f 7769 6467  dWidget(rhs_widg
-0001f690: 6574 290a 0a20 2020 2020 2020 2023 2061  et)..        # a
-0001f6a0: 6e64 2073 6574 2061 6c69 676e 6d65 6e74  nd set alignment
-0001f6b0: 206f 6620 7468 6520 6d6f 6465 6c0a 2020   of the model.  
-0001f6c0: 2020 2020 2020 6d6f 6465 6c5f 6c61 796f        model_layo
-0001f6d0: 7574 2e73 6574 416c 6967 6e6d 656e 7428  ut.setAlignment(
-0001f6e0: 5174 436f 7265 2e51 742e 416c 6967 6e54  QtCore.Qt.AlignT
-0001f6f0: 6f70 290a 0a20 2020 2020 2020 2072 6574  op)..        ret
-0001f700: 7572 6e20 6d6f 6465 6c5f 7769 6467 6574  urn model_widget
-0001f710: 0a0a 2020 2020 6465 6620 6e6f 745f 6966  ..    def not_if
-0001f720: 7928 7365 6c66 2c20 7061 726e 616d 653a  y(self, parname:
-0001f730: 2073 7472 293a 0a20 2020 2020 2020 2027   str):.        '
-0001f740: 2727 0a20 2020 2020 2020 2053 7769 7463  ''.        Switc
-0001f750: 6865 7320 6669 7420 6469 6374 696f 6e61  hes fit dictiona
-0001f760: 7279 2065 6e74 7279 2054 7275 6520 3c2d  ry entry True <-
-0001f770: 2d3e 2046 616c 7365 0a20 2020 2020 2020  -> False.       
-0001f780: 2066 6f72 2074 6865 2070 726f 7669 6465   for the provide
-0001f790: 6420 7061 726e 616d 650a 2020 2020 2020  d parname.      
-0001f7a0: 2020 2727 270a 2020 2020 2020 2020 7365    '''.        se
-0001f7b0: 6c66 2e75 7365 6c2e 6669 745b 7061 726e  lf.usel.fit[parn
-0001f7c0: 616d 655d 203d 206e 6f74 2073 656c 662e  ame] = not self.
-0001f7d0: 7573 656c 2e66 6974 5b70 6172 6e61 6d65  usel.fit[parname
-0001f7e0: 5d0a 0a20 2020 2064 6566 206d 616b 655f  ]..    def make_
-0001f7f0: 7061 7262 6f78 2873 656c 662c 2063 623a  parbox(self, cb:
-0001f800: 2070 6172 7469 616c 2c20 7061 726e 616d   partial, parnam
-0001f810: 653a 2073 7472 2c20 5f6e 755f 7374 7269  e: str, _nu_stri
-0001f820: 6e67 3a20 7374 722c 0a20 2020 2020 2020  ng: str,.       
-0001f830: 2020 2020 2020 2020 2020 2020 2064 6566               def
-0001f840: 6175 6c74 733a 2064 6963 745b 7374 722c  aults: dict[str,
-0001f850: 2066 6c6f 6174 5d2c 206f 705f 7061 723a   float], op_par:
-0001f860: 2051 7457 6964 6765 7473 2e51 5769 6467   QtWidgets.QWidg
-0001f870: 6574 2c0a 2020 2020 2020 2020 2020 2020  et,.            
-0001f880: 2020 2020 2020 2020 6d6f 6465 6c6e 616d          modelnam
-0001f890: 653a 2073 7472 293a 0a20 2020 2020 2020  e: str):.       
-0001f8a0: 2027 2727 0a20 2020 2020 2020 2043 7265   '''.        Cre
-0001f8b0: 6174 6573 2073 6574 206f 6620 7769 6467  ates set of widg
-0001f8c0: 6574 7320 666f 7220 6120 7369 6e67 6c65  ets for a single
-0001f8d0: 2070 6172 616d 6574 6572 206f 6620 6120   parameter of a 
-0001f8e0: 6d6f 6465 6c2e 5c6e 0a20 2020 2020 2020  model.\n.       
-0001f8f0: 2043 6f6e 7461 696e 7320 3220 726f 7773   Contains 2 rows
-0001f900: 2c20 7570 7065 7220 6973 206c 6162 656c  , upper is label
-0001f910: 2061 6e64 2075 6e69 7473 2061 7320 7374   and units as st
-0001f920: 7269 6e67 2c20 616e 6420 6c6f 7765 720a  ring, and lower.
-0001f930: 2020 2020 2020 2020 6973 2073 6c69 6465          is slide
-0001f940: 722c 2074 6578 7465 6e74 7279 2028 646f  r, textentry (do
-0001f950: 7562 6c65 7370 696e 626f 7829 2c20 616e  ublespinbox), an
-0001f960: 6420 6669 742f 6669 7820 746f 6767 6c65  d fit/fix toggle
-0001f970: 2062 7574 746f 6e2e 0a0a 2020 2020 2020   button...      
-0001f980: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-0001f990: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
-0001f9a0: 2020 2020 2020 2020 6362 3a20 6675 6e63          cb: func
-0001f9b0: 746f 6f6c 732e 7061 7274 6961 6c0a 2020  tools.partial.  
-0001f9c0: 2020 2020 2020 2020 2020 5061 7274 6961            Partia
-0001f9d0: 6c2d 6c79 2069 6e73 7461 6e74 6961 7465  l-ly instantiate
-0001f9e0: 6420 6361 6c6c 6261 636b 2077 6869 6368  d callback which
-0001f9f0: 2077 696c 6c20 6265 2066 6972 6564 2077   will be fired w
-0001fa00: 6865 6e0a 2020 2020 2020 2020 2020 2020  hen.            
-0001fa10: 7769 6467 6574 7320 6f66 2074 6869 7320  widgets of this 
-0001fa20: 7061 7261 6d65 7465 7220 6172 6520 696e  parameter are in
-0001fa30: 7465 7261 6374 6564 2077 6974 682e 0a20  teracted with.. 
-0001fa40: 2020 2020 2020 2070 6172 6e61 6d65 3a20         parname: 
-0001fa50: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
-0001fa60: 5374 7269 6e67 206e 616d 6520 6f66 2070  String name of p
-0001fa70: 6172 616d 6574 6572 2075 7365 6420 6173  arameter used as
-0001fa80: 206b 6579 2069 6e0a 2020 2020 2020 2020   key in.        
-0001fa90: 2020 2020 7365 6c66 2e77 6964 6765 7464      self.widgetd
-0001faa0: 6963 745b 7769 6467 6574 6469 6374 5d0a  ict[widgetdict].
-0001fab0: 2020 2020 2020 2020 5f6e 755f 7374 7269          _nu_stri
-0001fac0: 6e67 3a20 7374 720a 2020 2020 2020 2020  ng: str.        
-0001fad0: 2020 2020 5374 7269 6e67 206e 616d 6520      String name 
-0001fae0: 6f66 2070 6172 616d 6574 6572 2061 6e64  of parameter and
-0001faf0: 2075 6e69 7473 2075 7365 6420 6173 2074   units used as t
-0001fb00: 6974 6c65 206f 6620 7468 6973 2070 6172  itle of this par
-0001fb10: 616d 6574 6572 0a20 2020 2020 2020 2064  ameter.        d
-0001fb20: 6566 6175 6c74 733a 2064 6963 745b 7374  efaults: dict[st
-0001fb30: 722c 2066 6c6f 6174 5d0a 2020 2020 2020  r, float].      
-0001fb40: 2020 2020 2020 4465 6661 756c 7420 7661        Default va
-0001fb50: 6c75 6573 206f 6620 7468 6973 2070 6172  lues of this par
-0001fb60: 616d 6574 6572 2c20 6b65 7973 2061 7265  ameter, keys are
-0001fb70: 206d 696e 2c20 6d61 782c 2076 616c 696e   min, max, valin
-0001fb80: 6974 2c20 7374 6570 0a20 2020 2020 2020  it, step.       
-0001fb90: 206f 705f 7061 723a 2051 7457 6964 6765   op_par: QtWidge
-0001fba0: 7473 2e51 5769 6467 6574 0a20 2020 2020  ts.QWidget.     
-0001fbb0: 2020 2020 2020 2050 6172 656e 7420 7769         Parent wi
-0001fbc0: 6467 6574 0a20 2020 2020 2020 206d 6f64  dget.        mod
-0001fbd0: 656c 6e61 6d65 3a20 7374 720a 2020 2020  elname: str.    
-0001fbe0: 2020 2020 2020 2020 5374 7269 6e67 206e          String n
-0001fbf0: 616d 6520 6f66 206d 6f64 656c 2075 7365  ame of model use
-0001fc00: 6420 6173 206b 6579 2069 6e20 7365 6c66  d as key in self
-0001fc10: 2e77 6964 6765 7464 6963 740a 2020 2020  .widgetdict.    
-0001fc20: 2020 2020 2727 270a 0a20 2020 2020 2020      '''..       
-0001fc30: 2023 2057 6964 6765 7420 666f 7220 7468   # Widget for th
-0001fc40: 6973 2070 6172 616d 6574 6572 2773 2072  is parameter's r
-0001fc50: 6f77 206f 6620 7769 6467 6574 730a 2020  ow of widgets.  
-0001fc60: 2020 2020 2020 6f6e 655f 7061 7261 6d5f        one_param_
-0001fc70: 7769 6467 6574 203d 2051 7457 6964 6765  widget = QtWidge
-0001fc80: 7473 2e51 5769 6467 6574 2870 6172 656e  ts.QWidget(paren
-0001fc90: 743d 6f70 5f70 6172 290a 2020 2020 2020  t=op_par).      
-0001fca0: 2020 6f6e 655f 7061 7261 6d5f 6c61 796f    one_param_layo
-0001fcb0: 7574 203d 2051 7457 6964 6765 7473 2e51  ut = QtWidgets.Q
-0001fcc0: 5642 6f78 4c61 796f 7574 286f 6e65 5f70  VBoxLayout(one_p
-0001fcd0: 6172 616d 5f77 6964 6765 7429 0a0a 2020  aram_widget)..  
-0001fce0: 2020 2020 2020 2320 466f 7220 6c61 6265        # For labe
-0001fcf0: 6c20 616e 6420 756e 6974 730a 2020 2020  l and units.    
-0001fd00: 2020 2020 746f 705f 626f 7877 6964 6765      top_boxwidge
-0001fd10: 7420 3d20 5174 5769 6467 6574 732e 5157  t = QtWidgets.QW
-0001fd20: 6964 6765 7428 7061 7265 6e74 3d6f 6e65  idget(parent=one
-0001fd30: 5f70 6172 616d 5f77 6964 6765 7429 0a20  _param_widget). 
-0001fd40: 2020 2020 2020 2074 6f70 5f62 6f78 6c61         top_boxla
-0001fd50: 796f 7574 203d 2051 7457 6964 6765 7473  yout = QtWidgets
-0001fd60: 2e51 4842 6f78 4c61 796f 7574 2874 6f70  .QHBoxLayout(top
-0001fd70: 5f62 6f78 7769 6467 6574 290a 0a20 2020  _boxwidget)..   
-0001fd80: 2020 2020 2023 2046 6f72 2069 6e74 6572       # For inter
-0001fd90: 6163 7469 7665 2077 6964 6765 7473 0a20  active widgets. 
-0001fda0: 2020 2020 2020 2062 6f74 5f62 6f78 7769         bot_boxwi
-0001fdb0: 6467 6574 203d 2051 7457 6964 6765 7473  dget = QtWidgets
-0001fdc0: 2e51 5769 6467 6574 2870 6172 656e 743d  .QWidget(parent=
-0001fdd0: 6f6e 655f 7061 7261 6d5f 7769 6467 6574  one_param_widget
-0001fde0: 290a 2020 2020 2020 2020 626f 745f 626f  ).        bot_bo
-0001fdf0: 786c 6179 6f75 7420 3d20 5174 5769 6467  xlayout = QtWidg
-0001fe00: 6574 732e 5148 426f 784c 6179 6f75 7428  ets.QHBoxLayout(
-0001fe10: 626f 745f 626f 7877 6964 6765 7429 0a0a  bot_boxwidget)..
-0001fe20: 2020 2020 2020 2020 2320 4164 6420 6c61          # Add la
-0001fe30: 6265 6c20 616e 6420 756e 6974 730a 2020  bel and units.  
-0001fe40: 2020 2020 2020 6e61 6d65 5f75 6e69 7473        name_units
-0001fe50: 203d 2051 7457 6964 6765 7473 2e51 4c61   = QtWidgets.QLa
-0001fe60: 6265 6c28 5f6e 755f 7374 7269 6e67 290a  bel(_nu_string).
-0001fe70: 2020 2020 2020 2020 6e61 6d65 5f75 6e69          name_uni
-0001fe80: 7473 2e73 6574 466f 6e74 2851 7447 7569  ts.setFont(QtGui
-0001fe90: 2e51 466f 6e74 2827 4172 6961 6c27 2c20  .QFont('Arial', 
-0001fea0: 3131 2929 0a0a 2020 2020 2020 2020 6e61  11))..        na
-0001feb0: 6d65 5f75 6e69 7473 2e73 6574 5369 7a65  me_units.setSize
-0001fec0: 506f 6c69 6379 280a 2020 2020 2020 2020  Policy(.        
-0001fed0: 2020 2020 5174 5769 6467 6574 732e 5153      QtWidgets.QS
-0001fee0: 697a 6550 6f6c 6963 792e 4669 7865 642c  izePolicy.Fixed,
-0001fef0: 0a20 2020 2020 2020 2020 2020 2051 7457  .            QtW
-0001ff00: 6964 6765 7473 2e51 5369 7a65 506f 6c69  idgets.QSizePoli
-0001ff10: 6379 2e46 6978 6564 0a20 2020 2020 2020  cy.Fixed.       
-0001ff20: 2029 0a0a 2020 2020 2020 2020 746f 705f   )..        top_
-0001ff30: 626f 786c 6179 6f75 742e 6164 6457 6964  boxlayout.addWid
-0001ff40: 6765 7428 6e61 6d65 5f75 6e69 7473 290a  get(name_units).
-0001ff50: 0a20 2020 2020 2020 2023 2043 7265 6174  .        # Creat
-0001ff60: 6520 736c 6964 6572 0a20 2020 2020 2020  e slider.       
-0001ff70: 2073 6c69 6465 7220 3d20 5174 5769 6467   slider = QtWidg
-0001ff80: 6574 732e 5153 6c69 6465 7228 0a20 2020  ets.QSlider(.   
-0001ff90: 2020 2020 2020 2020 206f 7269 656e 7461           orienta
-0001ffa0: 7469 6f6e 3d51 7443 6f72 652e 5174 2e48  tion=QtCore.Qt.H
-0001ffb0: 6f72 697a 6f6e 7461 6c2c 0a20 2020 2020  orizontal,.     
-0001ffc0: 2020 2020 2020 2070 6172 656e 743d 626f         parent=bo
-0001ffd0: 745f 626f 7877 6964 6765 740a 2020 2020  t_boxwidget.    
-0001ffe0: 2020 2020 290a 0a20 2020 2020 2020 2023      )..        #
-0001fff0: 2053 6361 6c65 2061 6c6c 2073 6c69 6465   Scale all slide
-00020000: 7220 6e75 6d62 6572 7320 6279 2074 6869  r numbers by thi
-00020010: 7320 746f 206d 616b 6520 696e 746f 2066  s to make into f
-00020020: 6c6f 6174 730a 2020 2020 2020 2020 736c  loats.        sl
-00020030: 6964 6572 5f73 6361 6c65 203d 2031 4535  ider_scale = 1E5
-00020040: 0a0a 2020 2020 2020 2020 736c 6964 6572  ..        slider
-00020050: 2e73 6574 4d69 6e69 6d75 6d28 696e 7428  .setMinimum(int(
-00020060: 6465 6661 756c 7473 5b27 6d69 6e27 5d20  defaults['min'] 
-00020070: 2a20 736c 6964 6572 5f73 6361 6c65 2929  * slider_scale))
-00020080: 0a20 2020 2020 2020 2073 6c69 6465 722e  .        slider.
-00020090: 7365 744d 6178 696d 756d 2869 6e74 2864  setMaximum(int(d
-000200a0: 6566 6175 6c74 735b 276d 6178 275d 202a  efaults['max'] *
-000200b0: 2073 6c69 6465 725f 7363 616c 6529 290a   slider_scale)).
-000200c0: 2020 2020 2020 2020 736c 6964 6572 2e73          slider.s
-000200d0: 6574 5661 6c75 6528 696e 7428 6465 6661  etValue(int(defa
-000200e0: 756c 7473 5b27 7661 6c69 6e69 7427 5d20  ults['valinit'] 
-000200f0: 2a20 736c 6964 6572 5f73 6361 6c65 2929  * slider_scale))
-00020100: 0a20 2020 2020 2020 2073 6c69 6465 722e  .        slider.
-00020110: 7365 7453 696e 676c 6553 7465 7028 696e  setSingleStep(in
-00020120: 7428 6465 6661 756c 7473 5b27 7374 6570  t(defaults['step
-00020130: 275d 202a 2073 6c69 6465 725f 7363 616c  '] * slider_scal
-00020140: 6529 290a 0a20 2020 2020 2020 2073 656c  e))..        sel
-00020150: 662e 7769 6467 6574 6469 6374 5b6d 6f64  f.widgetdict[mod
-00020160: 656c 6e61 6d65 2e6c 6f77 6572 2829 5d5b  elname.lower()][
-00020170: 7061 726e 616d 655d 5b27 736c 6964 6572  parname]['slider
-00020180: 275d 203d 2073 6c69 6465 720a 0a20 2020  '] = slider..   
-00020190: 2020 2020 2023 2041 6464 2073 6c69 6465       # Add slide
-000201a0: 7220 746f 206c 6179 6f75 740a 2020 2020  r to layout.    
-000201b0: 2020 2020 626f 745f 626f 786c 6179 6f75      bot_boxlayou
-000201c0: 742e 6164 6457 6964 6765 7428 736c 6964  t.addWidget(slid
-000201d0: 6572 290a 0a20 2020 2020 2020 2023 2043  er)..        # C
-000201e0: 7265 6174 6520 7465 7874 2065 6e74 7279  reate text entry
-000201f0: 2028 446f 7562 6c65 5370 696e 426f 7829   (DoubleSpinBox)
-00020200: 0a20 2020 2020 2020 2065 6e74 7279 203d  .        entry =
-00020210: 2051 7457 6964 6765 7473 2e51 446f 7562   QtWidgets.QDoub
-00020220: 6c65 5370 696e 426f 7828 7061 7265 6e74  leSpinBox(parent
-00020230: 3d62 6f74 5f62 6f78 7769 6467 6574 290a  =bot_boxwidget).
-00020240: 2020 2020 2020 2020 656e 7472 792e 7365          entry.se
-00020250: 7444 6563 696d 616c 7328 696e 7428 6465  tDecimals(int(de
-00020260: 6661 756c 7473 5b27 6465 6369 6d61 6c73  faults['decimals
-00020270: 275d 2929 0a20 2020 2020 2020 2065 6e74  '])).        ent
-00020280: 7279 2e73 6574 4275 7474 6f6e 5379 6d62  ry.setButtonSymb
-00020290: 6f6c 7328 5174 5769 6467 6574 732e 5144  ols(QtWidgets.QD
-000202a0: 6f75 626c 6553 7069 6e42 6f78 2e4e 6f42  oubleSpinBox.NoB
-000202b0: 7574 746f 6e73 290a 2020 2020 2020 2020  uttons).        
-000202c0: 656e 7472 792e 7365 744b 6579 626f 6172  entry.setKeyboar
-000202d0: 6454 7261 636b 696e 6728 4661 6c73 6529  dTracking(False)
-000202e0: 0a20 2020 2020 2020 2065 6e74 7279 2e73  .        entry.s
-000202f0: 6574 4d69 6e69 6d75 6d28 6465 6661 756c  etMinimum(defaul
-00020300: 7473 5b27 6d69 6e27 5d29 0a20 2020 2020  ts['min']).     
-00020310: 2020 2065 6e74 7279 2e73 6574 4d61 7869     entry.setMaxi
-00020320: 6d75 6d28 6465 6661 756c 7473 5b27 6d61  mum(defaults['ma
-00020330: 7827 5d29 0a20 2020 2020 2020 2065 6e74  x']).        ent
-00020340: 7279 2e73 6574 5661 6c75 6528 6465 6661  ry.setValue(defa
-00020350: 756c 7473 5b27 7661 6c69 6e69 7427 5d29  ults['valinit'])
-00020360: 0a20 2020 2020 2020 2065 6e74 7279 2e73  .        entry.s
-00020370: 6574 5369 6e67 6c65 5374 6570 2864 6566  etSingleStep(def
-00020380: 6175 6c74 735b 2773 7465 7027 5d29 0a0a  aults['step'])..
-00020390: 2020 2020 2020 2020 7365 6c66 2e77 6964          self.wid
-000203a0: 6765 7464 6963 745b 6d6f 6465 6c6e 616d  getdict[modelnam
-000203b0: 652e 6c6f 7765 7228 295d 5b70 6172 6e61  e.lower()][parna
-000203c0: 6d65 5d5b 2765 6e74 7279 275d 203d 2065  me]['entry'] = e
-000203d0: 6e74 7279 0a0a 2020 2020 2020 2020 2320  ntry..        # 
-000203e0: 4164 6420 646f 7562 6c65 7370 696e 626f  Add doublespinbo
-000203f0: 7820 746f 206c 6179 6f75 740a 2020 2020  x to layout.    
-00020400: 2020 2020 626f 745f 626f 786c 6179 6f75      bot_boxlayou
-00020410: 742e 6164 6457 6964 6765 7428 656e 7472  t.addWidget(entr
-00020420: 7929 0a0a 2020 2020 2020 2020 2320 4372  y)..        # Cr
-00020430: 6561 7465 2066 6974 2f66 6978 2074 6f67  eate fit/fix tog
-00020440: 676c 6520 6275 7474 6f6e 0a20 2020 2020  gle button.     
-00020450: 2020 2066 665f 746f 6767 6c65 203d 2051     ff_toggle = Q
-00020460: 7457 6964 6765 7473 2e51 5075 7368 4275  tWidgets.QPushBu
-00020470: 7474 6f6e 2827 4672 6565 272c 2070 6172  tton('Free', par
-00020480: 656e 743d 626f 745f 626f 7877 6964 6765  ent=bot_boxwidge
-00020490: 7429 0a0a 2020 2020 2020 2020 7365 6c66  t)..        self
-000204a0: 2e77 6964 6765 7464 6963 745b 6d6f 6465  .widgetdict[mode
-000204b0: 6c6e 616d 652e 6c6f 7765 7228 295d 5b70  lname.lower()][p
-000204c0: 6172 6e61 6d65 5d5b 2766 665f 746f 6767  arname]['ff_togg
-000204d0: 6c65 275d 203d 2066 665f 746f 6767 6c65  le'] = ff_toggle
-000204e0: 0a0a 2020 2020 2020 2020 6666 7377 203d  ..        ffsw =
-000204f0: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
-00020500: 4672 6565 273a 2027 4669 7865 6427 2c0a  Free': 'Fixed',.
-00020510: 2020 2020 2020 2020 2020 2020 2746 6978              'Fix
-00020520: 6564 273a 2027 4672 6565 272c 0a20 2020  ed': 'Free',.   
-00020530: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
-00020540: 2320 4361 6c6c 6261 636b 2066 6f72 2074  # Callback for t
-00020550: 6578 740a 2020 2020 2020 2020 6666 5f74  ext.        ff_t
-00020560: 6f67 676c 652e 636c 6963 6b65 642e 636f  oggle.clicked.co
-00020570: 6e6e 6563 7428 0a20 2020 2020 2020 2020  nnect(.         
-00020580: 2020 206c 616d 6264 6120 5f3a 2066 665f     lambda _: ff_
-00020590: 746f 6767 6c65 2e73 6574 5465 7874 2866  toggle.setText(f
-000205a0: 6673 775b 6666 5f74 6f67 676c 652e 7465  fsw[ff_toggle.te
-000205b0: 7874 2829 5d29 0a20 2020 2020 2020 2029  xt()]).        )
-000205c0: 0a0a 2020 2020 2020 2020 2320 4361 6c6c  ..        # Call
-000205d0: 6261 636b 2066 6f72 2066 6974 2f66 6978  back for fit/fix
-000205e0: 206f 6620 7468 6973 2070 6172 616d 6574   of this paramet
-000205f0: 6572 0a20 2020 2020 2020 2066 665f 746f  er.        ff_to
-00020600: 6767 6c65 2e63 6c69 636b 6564 2e63 6f6e  ggle.clicked.con
-00020610: 6e65 6374 280a 2020 2020 2020 2020 2020  nect(.          
-00020620: 2020 6c61 6d62 6461 205f 3a20 7365 6c66    lambda _: self
-00020630: 2e6e 6f74 5f69 6679 2870 6172 6e61 6d65  .not_ify(parname
-00020640: 290a 2020 2020 2020 2020 290a 0a20 2020  ).        )..   
-00020650: 2020 2020 2023 2043 6f6e 6e65 6374 2066       # Connect f
-00020660: 6974 2f66 6978 2074 6f20 736c 6964 6572  it/fix to slider
-00020670: 2061 6e64 2074 6578 7465 6e74 7279 0a20   and textentry. 
-00020680: 2020 2020 2020 2073 6c69 6465 722e 7661         slider.va
-00020690: 6c75 6543 6861 6e67 6564 2e63 6f6e 6e65  lueChanged.conne
-000206a0: 6374 286c 616d 6264 6120 7661 6c3a 2063  ct(lambda val: c
-000206b0: 6228 7661 6c20 2a20 736c 6964 6572 5f73  b(val * slider_s
-000206c0: 6361 6c65 2a2a 2d31 2929 0a20 2020 2020  cale**-1)).     
-000206d0: 2020 2073 6c69 6465 722e 7661 6c75 6543     slider.valueC
-000206e0: 6861 6e67 6564 2e63 6f6e 6e65 6374 280a  hanged.connect(.
-000206f0: 2020 2020 2020 2020 2020 2020 6c61 6d62              lamb
-00020700: 6461 2076 616c 3a20 656e 7472 792e 7365  da val: entry.se
-00020710: 7456 616c 7565 2876 616c 202a 2073 6c69  tValue(val * sli
-00020720: 6465 725f 7363 616c 652a 2a2d 3129 0a20  der_scale**-1). 
-00020730: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00020740: 2065 6e74 7279 2e76 616c 7565 4368 616e   entry.valueChan
-00020750: 6765 642e 636f 6e6e 6563 7428 6362 290a  ged.connect(cb).
-00020760: 2020 2020 2020 2020 656e 7472 792e 7661          entry.va
-00020770: 6c75 6543 6861 6e67 6564 2e63 6f6e 6e65  lueChanged.conne
-00020780: 6374 280a 2020 2020 2020 2020 2020 2020  ct(.            
-00020790: 6c61 6d62 6461 2076 616c 3a20 736c 6964  lambda val: slid
-000207a0: 6572 2e73 6574 5661 6c75 6528 696e 7428  er.setValue(int(
-000207b0: 7661 6c20 2a20 736c 6964 6572 5f73 6361  val * slider_sca
-000207c0: 6c65 2929 0a20 2020 2020 2020 2029 0a0a  le)).        )..
-000207d0: 2020 2020 2020 2020 2320 4164 6420 6669          # Add fi
-000207e0: 742f 6669 7820 746f 206c 6179 6f75 740a  t/fix to layout.
-000207f0: 2020 2020 2020 2020 626f 745f 626f 786c          bot_boxl
-00020800: 6179 6f75 742e 6164 6457 6964 6765 7428  ayout.addWidget(
-00020810: 6666 5f74 6f67 676c 6529 0a0a 2020 2020  ff_toggle)..    
-00020820: 2020 2020 746f 705f 626f 7877 6964 6765      top_boxwidge
-00020830: 742e 7365 7453 697a 6550 6f6c 6963 7928  t.setSizePolicy(
-00020840: 0a20 2020 2020 2020 2020 2020 2051 7457  .            QtW
-00020850: 6964 6765 7473 2e51 5369 7a65 506f 6c69  idgets.QSizePoli
-00020860: 6379 2e46 6978 6564 2c0a 2020 2020 2020  cy.Fixed,.      
-00020870: 2020 2020 2020 5174 5769 6467 6574 732e        QtWidgets.
-00020880: 5153 697a 6550 6f6c 6963 792e 4669 7865  QSizePolicy.Fixe
-00020890: 640a 2020 2020 2020 2020 290a 2020 2020  d.        ).    
-000208a0: 2020 2020 626f 745f 626f 7877 6964 6765      bot_boxwidge
-000208b0: 742e 7365 7453 697a 6550 6f6c 6963 7928  t.setSizePolicy(
-000208c0: 0a20 2020 2020 2020 2020 2020 2051 7457  .            QtW
-000208d0: 6964 6765 7473 2e51 5369 7a65 506f 6c69  idgets.QSizePoli
-000208e0: 6379 2e46 6978 6564 2c0a 2020 2020 2020  cy.Fixed,.      
-000208f0: 2020 2020 2020 5174 5769 6467 6574 732e        QtWidgets.
-00020900: 5153 697a 6550 6f6c 6963 792e 4669 7865  QSizePolicy.Fixe
-00020910: 640a 2020 2020 2020 2020 290a 2020 2020  d.        ).    
-00020920: 2020 2020 746f 705f 626f 786c 6179 6f75      top_boxlayou
-00020930: 742e 7365 7441 6c69 676e 6d65 6e74 2851  t.setAlignment(Q
-00020940: 7443 6f72 652e 5174 2e41 6c69 676e 4843  tCore.Qt.AlignHC
-00020950: 656e 7465 7229 0a0a 2020 2020 2020 2020  enter)..        
-00020960: 6f6e 655f 7061 7261 6d5f 6c61 796f 7574  one_param_layout
-00020970: 2e61 6464 5769 6467 6574 2874 6f70 5f62  .addWidget(top_b
-00020980: 6f78 7769 6467 6574 290a 2020 2020 2020  oxwidget).      
-00020990: 2020 6f6e 655f 7061 7261 6d5f 6c61 796f    one_param_layo
-000209a0: 7574 2e61 6464 5769 6467 6574 2862 6f74  ut.addWidget(bot
-000209b0: 5f62 6f78 7769 6467 6574 290a 0a20 2020  _boxwidget)..   
-000209c0: 2020 2020 206f 6e65 5f70 6172 616d 5f6c       one_param_l
-000209d0: 6179 6f75 742e 7365 7443 6f6e 7465 6e74  ayout.setContent
-000209e0: 734d 6172 6769 6e73 2830 2c20 302c 2030  sMargins(0, 0, 0
-000209f0: 2c20 3029 0a20 2020 2020 2020 206f 6e65  , 0).        one
-00020a00: 5f70 6172 616d 5f6c 6179 6f75 742e 7365  _param_layout.se
-00020a10: 7453 7061 6369 6e67 2832 290a 2020 2020  tSpacing(2).    
-00020a20: 2020 2020 6f6e 655f 7061 7261 6d5f 6c61      one_param_la
-00020a30: 796f 7574 2e61 6464 5374 7265 7463 6828  yout.addStretch(
-00020a40: 3129 0a20 2020 2020 2020 206f 6e65 5f70  1).        one_p
-00020a50: 6172 616d 5f6c 6179 6f75 742e 7365 7441  aram_layout.setA
-00020a60: 6c69 676e 6d65 6e74 2851 7443 6f72 652e  lignment(QtCore.
-00020a70: 5174 2e41 6c69 676e 5643 656e 7465 7229  Qt.AlignVCenter)
-00020a80: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00020a90: 206f 6e65 5f70 6172 616d 5f77 6964 6765   one_param_widge
-00020aa0: 742c 206f 6e65 5f70 6172 616d 5f6c 6179  t, one_param_lay
-00020ab0: 6f75 740a 0a0a 6465 6620 696e 7465 7261  out...def intera
-00020ac0: 6374 6976 655f 6669 7474 696e 6728 6461  ctive_fitting(da
-00020ad0: 7461 7365 743a 2054 6175 5444 6174 6173  taset: TauTDatas
-00020ae0: 6574 207c 2054 6175 4844 6174 6173 6574  et | TauHDataset
-00020af0: 2c20 6170 702c 0a20 2020 2020 2020 2020  , app,.         
-00020b00: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00020b10: 6f64 656c 5f6f 7074 3a20 7374 7220 7c20  odel_opt: str | 
-00020b20: 6c69 7374 5b4c 6f67 5461 7554 4d6f 6465  list[LogTauTMode
-00020b30: 6c20 7c20 4c6f 6754 6175 484d 6f64 656c  l | LogTauHModel
-00020b40: 5d20 3d20 2766 726f 6d5f 6461 7461 7365  ] = 'from_datase
-00020b50: 7427 2920 2d3e 2074 7570 6c65 5b6c 6973  t') -> tuple[lis
-00020b60: 745b 4c6f 6754 6175 544d 6f64 656c 207c  t[LogTauTModel |
-00020b70: 204c 6f67 5461 7548 4d6f 6465 6c5d 2c20   LogTauHModel], 
-00020b80: 6c69 7374 5b64 6963 745b 7374 722c 2066  list[dict[str, f
-00020b90: 6c6f 6174 5d5d 2c20 6c69 7374 5b64 6963  loat]], list[dic
-00020ba0: 745b 7374 722c 2066 6c6f 6174 5d5d 2c20  t[str, float]], 
-00020bb0: 626f 6f6c 5d3a 2023 206e 6f71 610a 2020  bool]: # noqa.  
-00020bc0: 2020 2727 270a 2020 2020 4372 6561 7465    '''.    Create
-00020bd0: 7320 7174 2077 696e 646f 7720 666f 7220  s qt window for 
-00020be0: 7573 6572 2074 6f20 696e 7465 7261 6374  user to interact
-00020bf0: 6976 656c 7920 6669 7420 6d6f 6465 6c73  ively fit models
-00020c00: 2074 6f20 7265 6c61 7861 7469 6f6e 0a20   to relaxation. 
-00020c10: 2020 2064 6174 610a 0a20 2020 2050 6172     data..    Par
-00020c20: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-00020c30: 2d2d 2d2d 2d2d 0a20 2020 2064 6174 6173  ------.    datas
-00020c40: 6574 3a20 5461 7554 4461 7461 7365 7420  et: TauTDataset 
-00020c50: 7c20 5461 7548 4461 7461 7365 740a 2020  | TauHDataset.  
-00020c60: 2020 2020 2020 4461 7461 7365 7420 746f        Dataset to
-00020c70: 2070 6c6f 740a 2020 2020 6170 703a 2051   plot.    app: Q
-00020c80: 7457 6964 6765 7473 2e51 4170 706c 6963  tWidgets.QApplic
-00020c90: 6174 696f 6e0a 2020 2020 2020 2020 4170  ation.        Ap
-00020ca0: 706c 6963 6174 696f 6e20 7573 6564 2062  plication used b
-00020cb0: 7920 6375 7272 656e 7420 7072 6f67 7261  y current progra
-00020cc0: 6d0a 2020 2020 2020 2020 4372 6561 7465  m.        Create
-00020cd0: 2077 6974 6820 6061 7070 3d51 7457 6964   with `app=QtWid
-00020ce0: 6765 7473 2e51 4170 706c 6963 6174 696f  gets.QApplicatio
-00020cf0: 6e28 5b5d 2960 0a20 2020 206d 6f64 656c  n([])`.    model
-00020d00: 5f6f 7074 3a20 7374 7220 7c20 6c69 7374  _opt: str | list
-00020d10: 5b4c 6f67 5461 7554 4d6f 6465 6c20 7c20  [LogTauTModel | 
-00020d20: 4c6f 6754 6175 484d 6f64 656c 5d20 6465  LogTauHModel] de
-00020d30: 6661 756c 7420 2766 726f 6d5f 6461 7461  fault 'from_data
-00020d40: 7365 7427 200a 2020 2020 2020 2020 4c69  set' .        Li
-00020d50: 7374 206f 6620 6d6f 6465 6c73 2074 6f20  st of models to 
-00020d60: 6f66 6665 7220 746f 2075 7365 722c 2069  offer to user, i
-00020d70: 6620 2766 726f 6d5f 6461 7461 7365 7427  f 'from_dataset'
-00020d80: 2077 696c 6c20 6765 6e65 7261 7465 0a20   will generate. 
-00020d90: 2020 2020 2020 2061 206c 6973 7420 6261         a list ba
-00020da0: 7365 6420 6f6e 2074 6865 2064 6174 6173  sed on the datas
-00020db0: 6574 2070 726f 7669 6465 640a 0a20 2020  et provided..   
-00020dc0: 2052 6574 7572 6e73 0a20 2020 202d 2d2d   Returns.    ---
-00020dd0: 2d2d 2d2d 0a20 2020 206c 6973 745b 4c6f  ----.    list[Lo
-00020de0: 6754 6175 544d 6f64 656c 207c 204c 6f67  gTauTModel | Log
-00020df0: 5461 7548 4d6f 6465 6c5d 0a20 2020 2020  TauHModel].     
-00020e00: 2020 204d 6f64 656c 7320 7365 6c65 6374     Models select
-00020e10: 6564 2062 7920 7573 6572 0a20 2020 206c  ed by user.    l
-00020e20: 6973 745b 6469 6374 5b73 7472 2c20 666c  ist[dict[str, fl
-00020e30: 6f61 745d 5d0a 2020 2020 2020 2020 6669  oat]].        fi
-00020e40: 745f 7661 7273 2064 6963 7473 2c20 6f6e  t_vars dicts, on
-00020e50: 6520 7065 7220 6d6f 6465 6c0a 2020 2020  e per model.    
-00020e60: 6c69 7374 5b64 6963 745b 7374 722c 2066  list[dict[str, f
-00020e70: 6c6f 6174 5d5d 0a20 2020 2020 2020 2066  loat]].        f
-00020e80: 6978 5f76 6172 7320 6469 6374 732c 206f  ix_vars dicts, o
-00020e90: 6e65 2070 6572 206d 6f64 656c 0a20 2020  ne per model.   
-00020ea0: 2062 6f6f 6c0a 2020 2020 2020 2020 5472   bool.        Tr
-00020eb0: 7565 2069 6620 7573 6572 2068 6173 2065  ue if user has e
-00020ec0: 7869 7465 6420 7769 6e64 6f77 2069 6e73  xited window ins
-00020ed0: 7465 6164 206f 6620 6669 7474 696e 670a  tead of fitting.
-00020ee0: 2020 2020 2020 2020 656c 7365 2046 616c          else Fal
-00020ef0: 7365 0a20 2020 2027 2727 2023 206e 6f71  se.    ''' # noq
-00020f00: 610a 0a20 2020 2069 6620 6d6f 6465 6c5f  a..    if model_
-00020f10: 6f70 7420 3d3d 2027 6672 6f6d 5f64 6174  opt == 'from_dat
-00020f20: 6173 6574 273a 0a20 2020 2020 2020 2069  aset':.        i
-00020f30: 6620 6973 696e 7374 616e 6365 2864 6174  f isinstance(dat
-00020f40: 6173 6574 2c20 5461 7554 4461 7461 7365  aset, TauTDatase
-00020f50: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-00020f60: 6d6f 6465 6c5f 6f70 7420 3d20 5b0a 2020  model_opt = [.  
-00020f70: 2020 2020 2020 2020 2020 2020 2020 4c6f                Lo
-00020f80: 674f 7262 6163 684d 6f64 656c 2c0a 2020  gOrbachModel,.  
-00020f90: 2020 2020 2020 2020 2020 2020 2020 4c6f                Lo
-00020fa0: 6752 616d 616e 4d6f 6465 6c2c 0a20 2020  gRamanModel,.   
-00020fb0: 2020 2020 2020 2020 2020 2020 204c 6f67               Log
-00020fc0: 5154 4d4d 6f64 656c 2c0a 2020 2020 2020  QTMModel,.      
-00020fd0: 2020 2020 2020 2020 2020 4c6f 6744 6972            LogDir
-00020fe0: 6563 744d 6f64 656c 0a20 2020 2020 2020  ectModel.       
-00020ff0: 2020 2020 205d 0a20 2020 2020 2020 2065       ].        e
-00021000: 6c69 6620 6973 696e 7374 616e 6365 2864  lif isinstance(d
-00021010: 6174 6173 6574 2c20 5461 7548 4461 7461  ataset, TauHData
-00021020: 7365 7429 3a0a 2020 2020 2020 2020 2020  set):.          
-00021030: 2020 6d6f 6465 6c5f 6f70 7420 3d20 5b0a    model_opt = [.
-00021040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021050: 4c6f 6746 4451 544d 4d6f 6465 6c2c 0a20  LogFDQTMModel,. 
-00021060: 2020 2020 2020 2020 2020 2020 2020 204c                 L
-00021070: 6f67 5261 6d61 6e49 494d 6f64 656c 2c0a  ogRamanIIModel,.
-00021080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021090: 4c6f 6742 5656 5261 6d61 6e49 494d 6f64  LogBVVRamanIIMod
-000210a0: 656c 2c0a 2020 2020 2020 2020 2020 2020  el,.            
-000210b0: 2020 2020 4c6f 6743 6f6e 7374 616e 744d      LogConstantM
-000210c0: 6f64 656c 2c0a 2020 2020 2020 2020 2020  odel,.          
-000210d0: 2020 2020 2020 4c6f 6742 5656 436f 6e73        LogBVVCons
-000210e0: 7461 6e74 4d6f 6465 6c2c 0a20 2020 2020  tantModel,.     
-000210f0: 2020 2020 2020 205d 0a0a 2020 2020 7573         ]..    us
-00021100: 656c 203d 2074 7970 6528 276f 626a 272c  el = type('obj',
-00021110: 2028 6f62 6a65 6374 2c29 2c20 7b0a 2020   (object,), {.  
-00021120: 2020 2020 2020 276d 6f64 656c 7327 3a20        'models': 
-00021130: 7b0a 2020 2020 2020 2020 2020 2020 6d6f  {.            mo
-00021140: 6465 6c2e 4e41 4d45 2e6c 6f77 6572 2829  del.NAME.lower()
-00021150: 3a20 4661 6c73 650a 2020 2020 2020 2020  : False.        
-00021160: 2020 2020 666f 7220 6d6f 6465 6c20 696e      for model in
-00021170: 206d 6f64 656c 5f6f 7074 0a20 2020 2020   model_opt.     
-00021180: 2020 207d 2c0a 2020 2020 2020 2020 2766     },.        'f
-00021190: 6974 5f76 6172 7327 3a20 5b5d 2c0a 2020  it_vars': [],.  
-000211a0: 2020 2020 2020 2766 6978 5f76 6172 7327        'fix_vars'
-000211b0: 3a20 5b5d 2c0a 2020 2020 2020 2020 2766  : [],.        'f
-000211c0: 6978 273a 205b 5d2c 0a20 2020 2020 2020  ix': [],.       
-000211d0: 2027 6578 6974 6564 273a 2054 7275 650a   'exited': True.
-000211e0: 2020 2020 7d29 0a0a 2020 2020 7061 7261      })..    para
-000211f0: 6d5f 7769 6e64 6f77 203d 2046 6974 5769  m_window = FitWi
-00021200: 6e64 6f77 280a 2020 2020 2020 2020 6461  ndow(.        da
-00021210: 7461 7365 742c 0a20 2020 2020 2020 2075  taset,.        u
-00021220: 7365 6c2c 0a20 2020 2020 2020 206d 6f64  sel,.        mod
-00021230: 656c 5f6f 7074 2c0a 2020 2020 2020 2020  el_opt,.        
-00021240: 6775 692e 7769 6467 6574 5f64 6566 6175  gui.widget_defau
-00021250: 6c74 730a 2020 2020 290a 2020 2020 7061  lts.    ).    pa
-00021260: 7261 6d5f 7769 6e64 6f77 2e73 686f 7728  ram_window.show(
-00021270: 290a 0a20 2020 2061 7070 2e65 7865 6328  )..    app.exec(
-00021280: 290a 0a20 2020 206e 616d 655f 746f 5f6d  )..    name_to_m
-00021290: 6f64 656c 203d 207b 0a20 2020 2020 2020  odel = {.       
-000212a0: 206d 6f64 656c 2e4e 414d 452e 6c6f 7765   model.NAME.lowe
-000212b0: 7228 293a 206d 6f64 656c 0a20 2020 2020  r(): model.     
-000212c0: 2020 2066 6f72 206d 6f64 656c 2069 6e20     for model in 
-000212d0: 6d6f 6465 6c5f 6f70 740a 2020 2020 7d0a  model_opt.    }.
-000212e0: 0a20 2020 2072 5f6d 6f64 656c 7320 3d20  .    r_models = 
-000212f0: 5b0a 2020 2020 2020 2020 6e61 6d65 5f74  [.        name_t
-00021300: 6f5f 6d6f 6465 6c5b 6e61 6d65 5d0a 2020  o_model[name].  
-00021310: 2020 2020 2020 666f 7220 6e61 6d65 2069        for name i
-00021320: 6e20 7573 656c 2e6d 6f64 656c 730a 2020  n usel.models.  
-00021330: 2020 5d0a 0a20 2020 2072 6574 7572 6e20    ]..    return 
-00021340: 725f 6d6f 6465 6c73 2c20 7573 656c 2e66  r_models, usel.f
-00021350: 6974 5f76 6172 732c 2075 7365 6c2e 6669  it_vars, usel.fi
-00021360: 785f 7661 7273 2c20 7573 656c 2e65 7869  x_vars, usel.exi
-00021370: 7465 640a 0a0a 6465 6620 706c 6f74 5f66  ted...def plot_f
-00021380: 6974 7465 645f 7469 6d65 7328 6461 7461  itted_times(data
-00021390: 7365 743a 2054 6175 5444 6174 6173 6574  set: TauTDataset
-000213a0: 207c 2054 6175 4844 6174 6173 6574 2c0a   | TauHDataset,.
-000213b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000213c0: 2020 2020 2020 6d6f 6465 6c3a 204c 6f67        model: Log
-000213d0: 5461 7554 4d6f 6465 6c20 7c20 4d75 6c74  TauTModel | Mult
-000213e0: 694c 6f67 5461 7554 4d6f 6465 6c20 7c20  iLogTauTModel | 
-000213f0: 4c6f 6754 6175 484d 6f64 656c 207c 204d  LogTauHModel | M
-00021400: 756c 7469 4c6f 6754 6175 484d 6f64 656c  ultiLogTauHModel
-00021410: 2c20 2320 6e6f 7161 0a20 2020 2020 2020  , # noqa.       
-00021420: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00021430: 686f 773a 2062 6f6f 6c20 3d20 5472 7565  how: bool = True
-00021440: 2c20 7361 7665 3a20 626f 6f6c 203d 2046  , save: bool = F
-00021450: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
-00021460: 2020 2020 2020 2020 2020 2020 7361 7665              save
-00021470: 5f6e 616d 653a 2073 7472 203d 2027 6669  _name: str = 'fi
-00021480: 7474 6564 5f72 6174 6573 2e70 6e67 272c  tted_rates.png',
-00021490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000214a0: 2020 2020 2020 2076 6572 626f 7365 3a20         verbose: 
-000214b0: 626f 6f6c 203d 2054 7275 652c 0a20 2020  bool = True,.   
-000214c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000214d0: 2020 2073 686f 775f 7061 7261 6d73 3a20     show_params: 
-000214e0: 626f 6f6c 203d 2054 7275 6529 202d 3e20  bool = True) -> 
-000214f0: 7475 706c 655b 706c 742e 4669 6775 7265  tuple[plt.Figure
-00021500: 2c20 706c 742e 4178 6573 5d3a 0a20 2020  , plt.Axes]:.   
-00021510: 2027 2727 0a20 2020 2050 6c6f 7473 2065   '''.    Plots e
-00021520: 7870 6572 696d 656e 7461 6c20 616e 6420  xperimental and 
-00021530: 6669 7474 6564 2028 6d6f 6465 6c29 2072  fitted (model) r
-00021540: 656c 6178 6174 696f 6e20 7261 7465 2061  elaxation rate a
-00021550: 735c 6e0a 2020 2020 6c6e 2874 6175 2920  s\n.    ln(tau) 
-00021560: 7673 2031 2f78 7661 7220 7768 6572 6520  vs 1/xvar where 
-00021570: 7876 6172 2069 7320 5420 6f72 2048 2e0a  xvar is T or H..
-00021580: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
-00021590: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-000215a0: 2020 2064 6174 6173 6574 3a20 5461 7554     dataset: TauT
-000215b0: 4461 7461 7365 7420 7c20 5461 7548 4461  Dataset | TauHDa
-000215c0: 7461 7365 740a 2020 2020 2020 2020 4461  taset.        Da
-000215d0: 7461 7365 7420 746f 2070 6c6f 740a 2020  taset to plot.  
-000215e0: 2020 6d6f 6465 6c3a 204c 6f67 5461 7554    model: LogTauT
-000215f0: 4d6f 6465 6c20 7c20 4d75 6c74 694c 6f67  Model | MultiLog
-00021600: 5461 7554 4d6f 6465 6c20 7c20 4c6f 6754  TauTModel | LogT
-00021610: 6175 484d 6f64 656c 207c 204d 756c 7469  auHModel | Multi
-00021620: 4c6f 6754 6175 484d 6f64 656c 0a20 2020  LogTauHModel.   
-00021630: 2020 2020 204d 6f64 656c 2028 6669 7474       Model (fitt
-00021640: 6564 2920 746f 2070 6c6f 740a 2020 2020  ed) to plot.    
-00021650: 7368 6f77 3a20 626f 6f6c 2c20 6465 6661  show: bool, defa
-00021660: 756c 7420 5472 7565 0a20 2020 2020 2020  ult True.       
-00021670: 2049 6620 5472 7565 2c20 7368 6f77 2070   If True, show p
-00021680: 6c6f 7420 6f6e 2073 6372 6565 6e0a 2020  lot on screen.  
-00021690: 2020 7361 7665 3a20 626f 6f6c 2c20 6465    save: bool, de
-000216a0: 6661 756c 7420 4661 6c73 650a 2020 2020  fault False.    
-000216b0: 2020 2020 4966 2054 7275 652c 2073 6176      If True, sav
-000216c0: 6520 706c 6f74 2074 6f20 6669 6c65 2060  e plot to file `
-000216d0: 7361 7665 5f6e 616d 6560 0a20 2020 2073  save_name`.    s
-000216e0: 6176 655f 6e61 6d65 3a20 7374 722c 2064  ave_name: str, d
-000216f0: 6566 6175 6c74 203d 2027 6669 7474 6564  efault = 'fitted
-00021700: 5f72 6174 6573 2e70 6e67 270a 2020 2020  _rates.png'.    
-00021710: 2020 2020 4966 2073 6176 6520 6973 2054      If save is T
-00021720: 7275 652c 2077 696c 6c20 7361 7665 2070  rue, will save p
-00021730: 6c6f 7420 746f 2074 6869 7320 6669 6c65  lot to this file
-00021740: 6e61 6d65 0a20 2020 2076 6572 626f 7365  name.    verbose
-00021750: 3a20 626f 6f6c 2c20 6465 6661 756c 7420  : bool, default 
-00021760: 5472 7565 0a20 2020 2020 2020 2049 6620  True.        If 
-00021770: 5472 7565 2c20 706c 6f74 2066 696c 6520  True, plot file 
-00021780: 6c6f 6361 7469 6f6e 2069 7320 7772 6974  location is writ
-00021790: 7465 6e20 746f 2074 6572 6d69 6e61 6c0a  ten to terminal.
-000217a0: 2020 2020 7368 6f77 5f70 6172 616d 733a      show_params:
-000217b0: 2062 6f6f 6c2c 2064 6566 6175 6c74 2054   bool, default T
-000217c0: 7275 650a 2020 2020 2020 2020 4966 2054  rue.        If T
-000217d0: 7275 652c 2073 686f 7773 2066 6974 7465  rue, shows fitte
-000217e0: 6420 7061 7261 6d65 7465 7273 206f 6e20  d parameters on 
-000217f0: 706c 6f74 0a0a 2020 2020 5265 7475 726e  plot..    Return
-00021800: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
-00021810: 2020 706c 742e 4669 6775 7265 0a20 2020    plt.Figure.   
-00021820: 2020 2020 204d 6174 706c 6f74 6c69 6220       Matplotlib 
-00021830: 6669 6775 7265 206f 626a 6563 740a 2020  figure object.  
-00021840: 2020 706c 742e 4178 6573 0a20 2020 2020    plt.Axes.     
-00021850: 2020 204d 6174 706c 6f74 6c69 6220 6178     Matplotlib ax
-00021860: 6973 206f 626a 6563 740a 2020 2020 2727  is object.    ''
-00021870: 270a 0a20 2020 2069 6620 7368 6f77 5f70  '..    if show_p
-00021880: 6172 616d 733a 0a20 2020 2020 2020 2066  arams:.        f
-00021890: 6967 7369 7a65 203d 2028 362c 2036 290a  igsize = (6, 6).
-000218a0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000218b0: 2020 6669 6773 697a 6520 3d20 2836 2c20    figsize = (6, 
-000218c0: 352e 3529 0a0a 2020 2020 2320 4372 6561  5.5)..    # Crea
-000218d0: 7465 2066 6967 7572 6520 616e 6420 6178  te figure and ax
-000218e0: 6573 0a20 2020 2066 6967 2c20 6178 203d  es.    fig, ax =
-000218f0: 2070 6c74 2e73 7562 706c 6f74 7328 0a20   plt.subplots(. 
-00021900: 2020 2020 2020 2031 2c0a 2020 2020 2020         1,.      
-00021910: 2020 312c 0a20 2020 2020 2020 2073 6861    1,.        sha
-00021920: 7265 783d 5472 7565 2c0a 2020 2020 2020  rex=True,.      
-00021930: 2020 7368 6172 6579 3d54 7275 652c 0a20    sharey=True,. 
-00021940: 2020 2020 2020 2066 6967 7369 7a65 3d66         figsize=f
-00021950: 6967 7369 7a65 2c0a 2020 2020 2020 2020  igsize,.        
-00021960: 6e75 6d3d 2746 6974 7465 6420 7265 6c61  num='Fitted rela
-00021970: 7861 7469 6f6e 2070 726f 6669 6c65 270a  xation profile'.
-00021980: 2020 2020 290a 0a20 2020 205f 706c 6f74      )..    _plot
-00021990: 5f66 6974 7465 645f 7469 6d65 7328 6461  _fitted_times(da
-000219a0: 7461 7365 742c 206d 6f64 656c 2c20 6669  taset, model, fi
-000219b0: 672c 2061 782c 2073 686f 775f 7061 7261  g, ax, show_para
-000219c0: 6d73 3d73 686f 775f 7061 7261 6d73 290a  ms=show_params).
-000219d0: 0a20 2020 2066 6967 2e74 6967 6874 5f6c  .    fig.tight_l
-000219e0: 6179 6f75 7428 290a 0a20 2020 2069 6620  ayout()..    if 
-000219f0: 7368 6f77 3a0a 2020 2020 2020 2020 706c  show:.        pl
-00021a00: 742e 7368 6f77 2829 0a0a 2020 2020 6966  t.show()..    if
-00021a10: 2073 6176 653a 0a20 2020 2020 2020 2066   save:.        f
-00021a20: 6967 2e73 6176 6566 6967 2873 6176 655f  ig.savefig(save_
-00021a30: 6e61 6d65 2c20 6470 693d 3530 3029 0a20  name, dpi=500). 
-00021a40: 2020 2020 2020 2069 6620 7665 7262 6f73         if verbos
-00021a50: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
-00021a60: 6620 6973 696e 7374 616e 6365 2864 6174  f isinstance(dat
-00021a70: 6173 6574 2c20 2854 6175 5444 6174 6173  aset, (TauTDatas
-00021a80: 6574 2929 3a0a 2020 2020 2020 2020 2020  et)):.          
-00021a90: 2020 2020 2020 5f78 7661 7220 3d20 2754        _xvar = 'T
-00021aa0: 270a 2020 2020 2020 2020 2020 2020 656c  '.            el
-00021ab0: 6966 2069 7369 6e73 7461 6e63 6528 6461  if isinstance(da
-00021ac0: 7461 7365 742c 2028 5461 7548 4461 7461  taset, (TauHData
-00021ad0: 7365 7429 293a 0a20 2020 2020 2020 2020  set)):.         
-00021ae0: 2020 2020 2020 205f 7876 6172 203d 2027         _xvar = '
-00021af0: 4827 0a20 2020 2020 2020 2020 2020 2075  H'.            u
-00021b00: 742e 6370 7269 6e74 280a 2020 2020 2020  t.cprint(.      
-00021b10: 2020 2020 2020 2020 2020 6627 5c6e 2046            f'\n F
-00021b20: 6974 7465 6420 6c6e 28cf 8429 2076 7320  itted ln(..) vs 
-00021b30: 312f 7b5f 7876 6172 7d20 706c 6f74 2073  1/{_xvar} plot s
-00021b40: 6176 6564 2074 6f20 5c6e 207b 7361 7665  aved to \n {save
-00021b50: 5f6e 616d 657d 5c6e 272c 2023 206e 6f71  _name}\n', # noq
-00021b60: 610a 2020 2020 2020 2020 2020 2020 2020  a.              
-00021b70: 2020 2763 7961 6e27 0a20 2020 2020 2020    'cyan'.       
-00021b80: 2020 2020 2029 0a0a 2020 2020 7265 7475       )..    retu
-00021b90: 726e 2066 6967 2c20 6178 0a0a 0a64 6566  rn fig, ax...def
-00021ba0: 2070 6c6f 745f 7469 6d65 7328 6461 7461   plot_times(data
-00021bb0: 7365 743a 2054 6175 5444 6174 6173 6574  set: TauTDataset
-00021bc0: 207c 2054 6175 4844 6174 6173 6574 2c20   | TauHDataset, 
-00021bd0: 7368 6f77 3a20 626f 6f6c 203d 2054 7275  show: bool = Tru
-00021be0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00021bf0: 2020 7361 7665 3a20 626f 6f6c 203d 2046    save: bool = F
-00021c00: 616c 7365 2c20 7361 7665 5f6e 616d 653a  alse, save_name:
-00021c10: 2073 7472 203d 2027 7265 6c61 7861 7469   str = 'relaxati
-00021c20: 6f6e 5f74 696d 6573 2e70 6e67 272c 0a20  on_times.png',. 
-00021c30: 2020 2020 2020 2020 2020 2020 2020 7665                ve
-00021c40: 7262 6f73 653a 2062 6f6f 6c20 3d20 5472  rbose: bool = Tr
-00021c50: 7565 2920 2d3e 2074 7570 6c65 5b70 6c74  ue) -> tuple[plt
-00021c60: 2e46 6967 7572 652c 2070 6c74 2e41 7865  .Figure, plt.Axe
-00021c70: 735d 3a0a 2020 2020 2727 270a 2020 2020  s]:.    '''.    
-00021c80: 506c 6f74 7320 6578 7065 7269 6d65 6e74  Plots experiment
-00021c90: 616c 2072 656c 6178 6174 696f 6e20 7469  al relaxation ti
-00021ca0: 6d65 2061 735c 6e0a 2020 2020 6c6e 2874  me as\n.    ln(t
-00021cb0: 6175 2920 7673 2031 2f78 7661 7220 7768  au) vs 1/xvar wh
-00021cc0: 6572 6520 7876 6172 2069 7320 5420 6f72  ere xvar is T or
-00021cd0: 2048 2e0a 0a20 2020 2050 6172 616d 6574   H...    Paramet
-00021ce0: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
-00021cf0: 2d2d 0a20 2020 2064 6174 6173 6574 3a20  --.    dataset: 
-00021d00: 5461 7554 4461 7461 7365 7420 7c20 5461  TauTDataset | Ta
-00021d10: 7548 4461 7461 7365 740a 2020 2020 2020  uHDataset.      
-00021d20: 2020 4461 7461 7365 7420 746f 2070 6c6f    Dataset to plo
-00021d30: 740a 2020 2020 7368 6f77 3a20 626f 6f6c  t.    show: bool
-00021d40: 2c20 6465 6661 756c 7420 5472 7565 0a20  , default True. 
-00021d50: 2020 2020 2020 2049 6620 5472 7565 2c20         If True, 
-00021d60: 7368 6f77 2070 6c6f 7420 6f6e 2073 6372  show plot on scr
-00021d70: 6565 6e0a 2020 2020 7361 7665 3a20 626f  een.    save: bo
-00021d80: 6f6c 2c20 6465 6661 756c 7420 4661 6c73  ol, default Fals
-00021d90: 650a 2020 2020 2020 2020 4966 2054 7275  e.        If Tru
-00021da0: 652c 2073 6176 6520 706c 6f74 2074 6f20  e, save plot to 
-00021db0: 6669 6c65 2060 7361 7665 5f6e 616d 6560  file `save_name`
-00021dc0: 0a20 2020 2073 6176 655f 6e61 6d65 3a20  .    save_name: 
-00021dd0: 7374 722c 2064 6566 6175 6c74 2027 7265  str, default 're
-00021de0: 6c61 7861 7469 6f6e 5f74 696d 6573 2e70  laxation_times.p
-00021df0: 6e67 270a 2020 2020 2020 2020 4966 2073  ng'.        If s
-00021e00: 6176 6520 6973 2054 7275 652c 2077 696c  ave is True, wil
-00021e10: 6c20 7361 7665 2070 6c6f 7420 746f 2074  l save plot to t
-00021e20: 6869 7320 6669 6c65 6e61 6d65 0a20 2020  his filename.   
-00021e30: 2076 6572 626f 7365 3a20 626f 6f6c 2c20   verbose: bool, 
-00021e40: 6465 6661 756c 7420 5472 7565 0a20 2020  default True.   
-00021e50: 2020 2020 2049 6620 5472 7565 2c20 706c       If True, pl
-00021e60: 6f74 2066 696c 6520 6c6f 6361 7469 6f6e  ot file location
-00021e70: 2069 7320 7772 6974 7465 6e20 746f 2074   is written to t
-00021e80: 6572 6d69 6e61 6c0a 0a20 2020 2052 6574  erminal..    Ret
-00021e90: 7572 6e73 0a20 2020 202d 2d2d 2d2d 2d2d  urns.    -------
-00021ea0: 0a20 2020 2070 6c74 2e46 6967 7572 650a  .    plt.Figure.
-00021eb0: 2020 2020 2020 2020 4d61 7470 6c6f 746c          Matplotl
-00021ec0: 6962 2066 6967 7572 6520 6f62 6a65 6374  ib figure object
-00021ed0: 0a20 2020 2070 6c74 2e41 7865 730a 2020  .    plt.Axes.  
-00021ee0: 2020 2020 2020 4d61 7470 6c6f 746c 6962        Matplotlib
-00021ef0: 2061 7869 7320 6f62 6a65 6374 0a20 2020   axis object.   
-00021f00: 2027 2727 0a0a 2020 2020 2320 4372 6561   '''..    # Crea
-00021f10: 7465 2066 6967 7572 6520 616e 6420 6178  te figure and ax
-00021f20: 6573 0a20 2020 2066 6967 2c20 6178 203d  es.    fig, ax =
-00021f30: 2070 6c74 2e73 7562 706c 6f74 7328 0a20   plt.subplots(. 
-00021f40: 2020 2020 2020 2031 2c0a 2020 2020 2020         1,.      
-00021f50: 2020 312c 0a20 2020 2020 2020 2073 6861    1,.        sha
-00021f60: 7265 783d 5472 7565 2c0a 2020 2020 2020  rex=True,.      
-00021f70: 2020 7368 6172 6579 3d54 7275 652c 0a20    sharey=True,. 
-00021f80: 2020 2020 2020 2066 6967 7369 7a65 3d28         figsize=(
-00021f90: 362c 2035 2e35 292c 0a20 2020 2020 2020  6, 5.5),.       
-00021fa0: 206e 756d 3d27 4669 7474 6564 2072 656c   num='Fitted rel
-00021fb0: 6178 6174 696f 6e20 7072 6f66 696c 6527  axation profile'
-00021fc0: 0a20 2020 2029 0a0a 2020 2020 6966 2069  .    )..    if i
-00021fd0: 7369 6e73 7461 6e63 6528 6461 7461 7365  sinstance(datase
-00021fe0: 742c 2054 6175 4844 6174 6173 6574 293a  t, TauHDataset):
-00021ff0: 0a20 2020 2020 2020 2078 5f76 616c 7320  .        x_vals 
-00022000: 3d20 636f 7079 2e63 6f70 7928 6461 7461  = copy.copy(data
-00022010: 7365 742e 6669 656c 6473 290a 2020 2020  set.fields).    
-00022020: 2020 2020 6178 2e73 6574 5f78 6c61 6265      ax.set_xlabe
-00022030: 6c28 7227 312f 4820 245c 6c65 6674 285c  l(r'1/H $\left(\
-00022040: 6d61 7468 7265 6775 6c61 727b 4f65 7d5e  mathregular{Oe}^
-00022050: 5c6d 6174 6872 6567 756c 6172 7b2d 317d  \mathregular{-1}
-00022060: 5c72 6967 6874 2924 2729 0a20 2020 2065  \right)$').    e
-00022070: 6c69 6620 6973 696e 7374 616e 6365 2864  lif isinstance(d
-00022080: 6174 6173 6574 2c20 5461 7554 4461 7461  ataset, TauTData
-00022090: 7365 7429 3a0a 2020 2020 2020 2020 785f  set):.        x_
-000220a0: 7661 6c73 203d 2063 6f70 792e 636f 7079  vals = copy.copy
-000220b0: 2864 6174 6173 6574 2e74 656d 7065 7261  (dataset.tempera
-000220c0: 7475 7265 7329 0a20 2020 2020 2020 2061  tures).        a
-000220d0: 782e 7365 745f 786c 6162 656c 2872 2731  x.set_xlabel(r'1
-000220e0: 2f54 2024 5c6c 6566 7428 5c6d 6174 6872  /T $\left(\mathr
-000220f0: 6567 756c 6172 7b4b 7d5e 5c6d 6174 6872  egular{K}^\mathr
-00022100: 6567 756c 6172 7b2d 317d 5c72 6967 6874  egular{-1}\right
-00022110: 2924 2729 0a0a 2020 2020 2320 4164 6420  )$')..    # Add 
-00022120: 756e 6365 7274 6169 6e74 6965 7320 6173  uncertainties as
-00022130: 2065 7272 6f72 6261 7273 0a20 2020 2069   errorbars.    i
-00022140: 6620 6c65 6e28 6461 7461 7365 742e 7261  f len(dataset.ra
-00022150: 7465 5f70 6d29 3a0a 0a20 2020 2020 2020  te_pm):..       
-00022160: 2023 2043 616c 6375 6c61 7465 2074 696d   # Calculate tim
-00022170: 6520 6572 726f 7262 6172 730a 2020 2020  e errorbars.    
-00022180: 2020 2020 7469 6d65 7320 3d20 312e 202f      times = 1. /
-00022190: 2064 6174 6173 6574 2e72 6174 6573 0a20   dataset.rates. 
-000221a0: 2020 2020 2020 206d 696e 5f74 696d 6520         min_time 
-000221b0: 3d20 312e 202f 2028 6461 7461 7365 742e  = 1. / (dataset.
-000221c0: 7261 7465 7320 2b20 6461 7461 7365 742e  rates + dataset.
-000221d0: 7261 7465 5f70 6d5b 312c 203a 5d29 0a20  rate_pm[1, :]). 
-000221e0: 2020 2020 2020 206d 6178 5f74 696d 6520         max_time 
-000221f0: 3d20 312e 202f 2028 6461 7461 7365 742e  = 1. / (dataset.
-00022200: 7261 7465 7320 2d20 6461 7461 7365 742e  rates - dataset.
-00022210: 7261 7465 5f70 6d5b 302c 203a 5d29 0a0a  rate_pm[0, :])..
-00022220: 2020 2020 2020 2020 6c6e 5f6d 696e 5f74          ln_min_t
-00022230: 696d 6520 3d20 6e70 2e6c 6f67 286d 696e  ime = np.log(min
-00022240: 5f74 696d 6529 0a20 2020 2020 2020 206c  _time).        l
-00022250: 6e5f 6d61 785f 7469 6d65 203d 206e 702e  n_max_time = np.
-00022260: 6c6f 6728 6d61 785f 7469 6d65 290a 0a20  log(max_time).. 
-00022270: 2020 2020 2020 206c 6e5f 7469 6d65 5f70         ln_time_p
-00022280: 6c75 7320 3d20 6c6e 5f6d 6178 5f74 696d  lus = ln_max_tim
-00022290: 6520 2d20 6e70 2e6c 6f67 2874 696d 6573  e - np.log(times
-000222a0: 290a 2020 2020 2020 2020 6c6e 5f74 696d  ).        ln_tim
-000222b0: 655f 6d69 6e75 7320 3d20 6e70 2e6c 6f67  e_minus = np.log
-000222c0: 2874 696d 6573 2920 2d20 6c6e 5f6d 696e  (times) - ln_min
-000222d0: 5f74 696d 650a 0a20 2020 2020 2020 206c  _time..        l
-000222e0: 6e74 696d 655f 6d70 203d 206e 702e 6172  ntime_mp = np.ar
-000222f0: 7261 7928 5b6c 6e5f 7469 6d65 5f6d 696e  ray([ln_time_min
-00022300: 7573 2c20 6c6e 5f74 696d 655f 706c 7573  us, ln_time_plus
-00022310: 5d29 0a0a 2020 2020 2020 2020 6178 2e65  ])..        ax.e
-00022320: 7272 6f72 6261 7228 0a20 2020 2020 2020  rrorbar(.       
-00022330: 2020 2020 2031 2e20 2f20 785f 7661 6c73       1. / x_vals
-00022340: 2c0a 2020 2020 2020 2020 2020 2020 6e70  ,.            np
-00022350: 2e6c 6f67 2874 696d 6573 292c 0a20 2020  .log(times),.   
-00022360: 2020 2020 2020 2020 2079 6572 723d 6c6e           yerr=ln
-00022370: 7469 6d65 5f6d 702c 0a20 2020 2020 2020  time_mp,.       
-00022380: 2020 2020 206d 6172 6b65 723d 276f 272c       marker='o',
-00022390: 0a20 2020 2020 2020 2020 2020 206c 773d  .            lw=
-000223a0: 302c 0a20 2020 2020 2020 2020 2020 2065  0,.            e
-000223b0: 6c69 6e65 7769 6474 683d 312e 352c 0a20  linewidth=1.5,. 
-000223c0: 2020 2020 2020 2020 2020 2066 696c 6c73             fills
-000223d0: 7479 6c65 3d27 6e6f 6e65 272c 0a20 2020  tyle='none',.   
-000223e0: 2020 2020 2020 2020 2063 6f6c 6f72 3d27           color='
-000223f0: 626c 6163 6b27 0a20 2020 2020 2020 2029  black'.        )
-00022400: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-00022410: 2020 2061 782e 706c 6f74 280a 2020 2020     ax.plot(.    
-00022420: 2020 2020 2020 2020 312e 202f 2078 5f76          1. / x_v
-00022430: 616c 732c 0a20 2020 2020 2020 2020 2020  als,.           
-00022440: 206e 702e 6c6f 6728 312e 202f 2064 6174   np.log(1. / dat
-00022450: 6173 6574 2e72 6174 6573 292c 0a20 2020  aset.rates),.   
-00022460: 2020 2020 2020 2020 206d 6172 6b65 723d           marker=
-00022470: 276f 272c 0a20 2020 2020 2020 2020 2020  'o',.           
-00022480: 206c 773d 302c 0a20 2020 2020 2020 2020   lw=0,.         
-00022490: 2020 2066 696c 6c73 7479 6c65 3d27 6e6f     fillstyle='no
-000224a0: 6e65 272c 0a20 2020 2020 2020 2020 2020  ne',.           
-000224b0: 2063 6f6c 6f72 3d27 626c 6163 6b27 0a20   color='black'. 
-000224c0: 2020 2020 2020 2029 0a0a 2020 2020 2320         )..    # 
-000224d0: 456e 6162 6c65 206d 696e 6f72 2074 6963  Enable minor tic
-000224e0: 6b73 0a20 2020 2061 782e 7961 7869 732e  ks.    ax.yaxis.
-000224f0: 7365 745f 6d69 6e6f 725f 6c6f 6361 746f  set_minor_locato
-00022500: 7228 4175 746f 4d69 6e6f 724c 6f63 6174  r(AutoMinorLocat
-00022510: 6f72 2829 290a 2020 2020 6178 2e78 6178  or()).    ax.xax
-00022520: 6973 2e73 6574 5f6d 696e 6f72 5f6c 6f63  is.set_minor_loc
-00022530: 6174 6f72 2841 7574 6f4d 696e 6f72 4c6f  ator(AutoMinorLo
-00022540: 6361 746f 7228 2929 0a0a 2020 2020 6178  cator())..    ax
-00022550: 2e73 6574 5f79 6c61 6265 6c28 7227 245c  .set_ylabel(r'$\
-00022560: 6c6e 5c6c 6566 745b 5c74 6175 5c72 6967  ln\left[\tau\rig
-00022570: 6874 5d24 2024 5c6c 6566 7428 5c6c 6e5c  ht]$ $\left(\ln\
-00022580: 6c65 6674 5b5c 6d61 7468 7265 6775 6c61  left[\mathregula
-00022590: 727b 737d 5e5c 6d61 7468 7265 6775 6c61  r{s}^\mathregula
-000225a0: 727b 2d31 7d5c 7269 6768 745d 5c72 6967  r{-1}\right]\rig
-000225b0: 6874 2924 2729 2023 206e 6f71 610a 0a20  ht)$') # noqa.. 
-000225c0: 2020 2066 6967 2e74 6967 6874 5f6c 6179     fig.tight_lay
-000225d0: 6f75 7428 290a 0a20 2020 2069 6620 7368  out()..    if sh
-000225e0: 6f77 3a0a 2020 2020 2020 2020 706c 742e  ow:.        plt.
-000225f0: 7368 6f77 2829 0a0a 2020 2020 6966 2073  show()..    if s
-00022600: 6176 653a 0a20 2020 2020 2020 2066 6967  ave:.        fig
-00022610: 2e73 6176 6566 6967 2873 6176 655f 6e61  .savefig(save_na
-00022620: 6d65 2c20 6470 693d 3530 3029 0a20 2020  me, dpi=500).   
-00022630: 2020 2020 2069 6620 7665 7262 6f73 653a       if verbose:
-00022640: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00022650: 6973 696e 7374 616e 6365 2864 6174 6173  isinstance(datas
-00022660: 6574 2c20 2854 6175 5444 6174 6173 6574  et, (TauTDataset
-00022670: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
-00022680: 2020 2020 5f78 7661 7220 3d20 2754 270a      _xvar = 'T'.
-00022690: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-000226a0: 2069 7369 6e73 7461 6e63 6528 6461 7461   isinstance(data
-000226b0: 7365 742c 2028 5461 7548 4461 7461 7365  set, (TauHDatase
-000226c0: 7429 293a 0a20 2020 2020 2020 2020 2020  t)):.           
-000226d0: 2020 2020 205f 7876 6172 203d 2027 4827       _xvar = 'H'
-000226e0: 0a20 2020 2020 2020 2020 2020 2075 742e  .            ut.
-000226f0: 6370 7269 6e74 280a 2020 2020 2020 2020  cprint(.        
-00022700: 2020 2020 2020 2020 6627 5c6e 2046 6974          f'\n Fit
-00022710: 7465 6420 6c6e 2874 6175 2920 7673 2031  ted ln(tau) vs 1
-00022720: 2f7b 5f78 7661 727d 2070 6c6f 7420 7361  /{_xvar} plot sa
-00022730: 7665 6420 746f 205c 6e20 7b73 6176 655f  ved to \n {save_
-00022740: 6e61 6d65 7d5c 6e27 2c20 2320 6e6f 7161  name}\n', # noqa
-00022750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022760: 2027 6379 616e 270a 2020 2020 2020 2020   'cyan'.        
-00022770: 2020 2020 290a 0a20 2020 2072 6574 7572      )..    retur
-00022780: 6e20 6669 672c 2061 780a 0a0a 6465 6620  n fig, ax...def 
-00022790: 5f70 6c6f 745f 6669 7474 6564 5f74 696d  _plot_fitted_tim
-000227a0: 6573 2864 6174 6173 6574 3a20 5461 7554  es(dataset: TauT
-000227b0: 4461 7461 7365 7420 7c20 5461 7548 4461  Dataset | TauHDa
-000227c0: 7461 7365 742c 0a20 2020 2020 2020 2020  taset,.         
-000227d0: 2020 2020 2020 2020 2020 2020 2020 6d6f                mo
-000227e0: 6465 6c3a 204c 6f67 5461 7554 4d6f 6465  del: LogTauTMode
-000227f0: 6c20 7c20 4d75 6c74 694c 6f67 5461 7554  l | MultiLogTauT
-00022800: 4d6f 6465 6c20 7c20 4c6f 6754 6175 484d  Model | LogTauHM
-00022810: 6f64 656c 207c 204d 756c 7469 4c6f 6754  odel | MultiLogT
-00022820: 6175 484d 6f64 656c 2c20 2320 6e6f 7161  auHModel, # noqa
-00022830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022840: 2020 2020 2020 2020 6669 673a 2070 6c74          fig: plt
-00022850: 2e46 6967 7572 652c 2061 783a 2070 6c74  .Figure, ax: plt
-00022860: 2e41 7865 732c 0a20 2020 2020 2020 2020  .Axes,.         
-00022870: 2020 2020 2020 2020 2020 2020 2020 7368                sh
-00022880: 6f77 5f70 6172 616d 733a 2062 6f6f 6c20  ow_params: bool 
-00022890: 3d20 5472 7565 293a 0a20 2020 2027 2727  = True):.    '''
-000228a0: 0a20 2020 2050 6c6f 7473 2065 7870 6572  .    Plots exper
-000228b0: 696d 656e 7461 6c20 616e 6420 6669 7474  imental and fitt
-000228c0: 6564 2028 6d6f 6465 6c29 2072 656c 6178  ed (model) relax
-000228d0: 6174 696f 6e20 7261 7465 2061 735c 6e0a  ation rate as\n.
-000228e0: 2020 2020 6c6e 2874 6175 2920 7673 2031      ln(tau) vs 1
-000228f0: 2f78 7661 7220 7768 6572 6520 7876 6172  /xvar where xvar
-00022900: 2069 7320 5420 6f72 2048 2e0a 0a20 2020   is T or H...   
-00022910: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-00022920: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064  ----------.    d
-00022930: 6174 6173 6574 3a20 5461 7554 4461 7461  ataset: TauTData
-00022940: 7365 7420 7c20 5461 7548 4461 7461 7365  set | TauHDatase
-00022950: 740a 2020 2020 2020 2020 4461 7461 7365  t.        Datase
-00022960: 7420 746f 2070 6c6f 740a 2020 2020 6d6f  t to plot.    mo
-00022970: 6465 6c3a 204c 6f67 5461 7554 4d6f 6465  del: LogTauTMode
-00022980: 6c20 7c20 4d75 6c74 694c 6f67 5461 7554  l | MultiLogTauT
-00022990: 4d6f 6465 6c20 7c20 4c6f 6754 6175 484d  Model | LogTauHM
-000229a0: 6f64 656c 207c 204d 756c 7469 4c6f 6754  odel | MultiLogT
-000229b0: 6175 484d 6f64 656c 0a20 2020 2020 2020  auHModel.       
-000229c0: 204d 6f64 656c 2028 6669 7474 6564 2920   Model (fitted) 
-000229d0: 746f 2070 6c6f 740a 2020 2020 6669 673a  to plot.    fig:
-000229e0: 2070 6c74 2e46 6967 7572 650a 2020 2020   plt.Figure.    
-000229f0: 2020 2020 4d61 7470 6c6f 746c 6962 2046      Matplotlib F
-00022a00: 6967 7572 6520 6f62 6a65 6374 2075 7365  igure object use
-00022a10: 6420 666f 7220 706c 6f74 0a20 2020 2061  d for plot.    a
-00022a20: 783a 2070 6c74 2e41 7865 730a 2020 2020  x: plt.Axes.    
-00022a30: 2020 2020 4d61 7470 6c6f 746c 6962 2041      Matplotlib A
-00022a40: 7869 7320 6f62 6a65 6374 2075 7365 6420  xis object used 
-00022a50: 666f 7220 706c 6f74 0a20 2020 2073 686f  for plot.    sho
-00022a60: 775f 7061 7261 6d73 3a20 626f 6f6c 2c20  w_params: bool, 
-00022a70: 6465 6661 756c 7420 5472 7565 0a20 2020  default True.   
-00022a80: 2020 2020 2049 6620 5472 7565 2c20 7368       If True, sh
-00022a90: 6f77 7320 6669 7474 6564 2070 6172 616d  ows fitted param
-00022aa0: 6574 6572 7320 6f6e 2070 6c6f 740a 0a20  eters on plot.. 
-00022ab0: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
-00022ac0: 2d2d 2d2d 2d2d 0a20 2020 204e 6f6e 650a  ------.    None.
-00022ad0: 2020 2020 2727 270a 0a20 2020 2069 6620      '''..    if 
-00022ae0: 6973 696e 7374 616e 6365 2864 6174 6173  isinstance(datas
-00022af0: 6574 2c20 5461 7548 4461 7461 7365 7429  et, TauHDataset)
-00022b00: 3a0a 2020 2020 2020 2020 785f 7661 6c73  :.        x_vals
-00022b10: 203d 2063 6f70 792e 636f 7079 2864 6174   = copy.copy(dat
-00022b20: 6173 6574 2e66 6965 6c64 7329 0a20 2020  aset.fields).   
-00022b30: 2020 2020 2061 782e 7365 745f 786c 6162       ax.set_xlab
-00022b40: 656c 2872 2731 2f48 2024 5c6c 6566 7428  el(r'1/H $\left(
-00022b50: 5c6d 6174 6872 6567 756c 6172 7b4f 657d  \mathregular{Oe}
-00022b60: 5e5c 6d61 7468 7265 6775 6c61 727b 2d31  ^\mathregular{-1
-00022b70: 7d5c 7269 6768 7429 2427 290a 2020 2020  }\right)$').    
-00022b80: 2020 2020 785f 7479 7065 203d 2027 6669      x_type = 'fi
-00022b90: 656c 6427 0a20 2020 2065 6c69 6620 6973  eld'.    elif is
-00022ba0: 696e 7374 616e 6365 2864 6174 6173 6574  instance(dataset
-00022bb0: 2c20 5461 7554 4461 7461 7365 7429 3a0a  , TauTDataset):.
-00022bc0: 2020 2020 2020 2020 785f 7661 6c73 203d          x_vals =
-00022bd0: 2063 6f70 792e 636f 7079 2864 6174 6173   copy.copy(datas
-00022be0: 6574 2e74 656d 7065 7261 7475 7265 7329  et.temperatures)
-00022bf0: 0a20 2020 2020 2020 2061 782e 7365 745f  .        ax.set_
-00022c00: 786c 6162 656c 2872 2731 2f54 2024 5c6c  xlabel(r'1/T $\l
-00022c10: 6566 7428 5c6d 6174 6872 6567 756c 6172  eft(\mathregular
-00022c20: 7b4b 7d5e 5c6d 6174 6872 6567 756c 6172  {K}^\mathregular
-00022c30: 7b2d 317d 5c72 6967 6874 2924 2729 0a20  {-1}\right)$'). 
-00022c40: 2020 2020 2020 2078 5f74 7970 6520 3d20         x_type = 
-00022c50: 2774 656d 7065 7261 7475 7265 270a 0a20  'temperature'.. 
-00022c60: 2020 2023 2041 6464 2075 6e63 6572 7461     # Add uncerta
-00022c70: 696e 7469 6573 2061 7320 6572 726f 7262  inties as errorb
-00022c80: 6172 730a 2020 2020 6966 206c 656e 2864  ars.    if len(d
-00022c90: 6174 6173 6574 2e72 6174 655f 706d 293a  ataset.rate_pm):
-00022ca0: 0a0a 2020 2020 2020 2020 2320 4361 6c63  ..        # Calc
-00022cb0: 756c 6174 6520 7469 6d65 2065 7272 6f72  ulate time error
-00022cc0: 6261 7273 0a20 2020 2020 2020 2074 696d  bars.        tim
-00022cd0: 6573 203d 2031 2e20 2f20 6461 7461 7365  es = 1. / datase
-00022ce0: 742e 7261 7465 730a 2020 2020 2020 2020  t.rates.        
-00022cf0: 6d69 6e5f 7469 6d65 203d 2031 2e20 2f20  min_time = 1. / 
-00022d00: 2864 6174 6173 6574 2e72 6174 6573 202b  (dataset.rates +
-00022d10: 2064 6174 6173 6574 2e72 6174 655f 706d   dataset.rate_pm
-00022d20: 5b31 2c20 3a5d 290a 2020 2020 2020 2020  [1, :]).        
-00022d30: 6d61 785f 7469 6d65 203d 2031 2e20 2f20  max_time = 1. / 
-00022d40: 2864 6174 6173 6574 2e72 6174 6573 202d  (dataset.rates -
-00022d50: 2064 6174 6173 6574 2e72 6174 655f 706d   dataset.rate_pm
-00022d60: 5b30 2c20 3a5d 290a 0a20 2020 2020 2020  [0, :])..       
-00022d70: 206c 6e5f 6d69 6e5f 7469 6d65 203d 206e   ln_min_time = n
-00022d80: 702e 6c6f 6728 6d69 6e5f 7469 6d65 290a  p.log(min_time).
-00022d90: 2020 2020 2020 2020 6c6e 5f6d 6178 5f74          ln_max_t
-00022da0: 696d 6520 3d20 6e70 2e6c 6f67 286d 6178  ime = np.log(max
-00022db0: 5f74 696d 6529 0a0a 2020 2020 2020 2020  _time)..        
-00022dc0: 6c6e 5f74 696d 655f 706c 7573 203d 206c  ln_time_plus = l
-00022dd0: 6e5f 6d61 785f 7469 6d65 202d 206e 702e  n_max_time - np.
-00022de0: 6c6f 6728 7469 6d65 7329 0a20 2020 2020  log(times).     
-00022df0: 2020 206c 6e5f 7469 6d65 5f6d 696e 7573     ln_time_minus
-00022e00: 203d 206e 702e 6c6f 6728 7469 6d65 7329   = np.log(times)
-00022e10: 202d 206c 6e5f 6d69 6e5f 7469 6d65 0a0a   - ln_min_time..
-00022e20: 2020 2020 2020 2020 6c6e 7469 6d65 5f6d          lntime_m
-00022e30: 7020 3d20 6e70 2e61 7272 6179 285b 6c6e  p = np.array([ln
-00022e40: 5f74 696d 655f 6d69 6e75 732c 206c 6e5f  _time_minus, ln_
-00022e50: 7469 6d65 5f70 6c75 735d 290a 0a20 2020  time_plus])..   
-00022e60: 2020 2020 2061 782e 6572 726f 7262 6172       ax.errorbar
-00022e70: 280a 2020 2020 2020 2020 2020 2020 312e  (.            1.
-00022e80: 202f 2078 5f76 616c 732c 0a20 2020 2020   / x_vals,.     
-00022e90: 2020 2020 2020 206e 702e 6c6f 6728 7469         np.log(ti
-00022ea0: 6d65 7329 2c0a 2020 2020 2020 2020 2020  mes),.          
-00022eb0: 2020 7965 7272 3d6c 6e74 696d 655f 6d70    yerr=lntime_mp
-00022ec0: 2c0a 2020 2020 2020 2020 2020 2020 6d61  ,.            ma
-00022ed0: 726b 6572 3d27 6f27 2c0a 2020 2020 2020  rker='o',.      
-00022ee0: 2020 2020 2020 6c77 3d30 2c0a 2020 2020        lw=0,.    
-00022ef0: 2020 2020 2020 2020 656c 696e 6577 6964          elinewid
-00022f00: 7468 3d31 2e35 2c0a 2020 2020 2020 2020  th=1.5,.        
-00022f10: 2020 2020 6669 6c6c 7374 796c 653d 276e      fillstyle='n
-00022f20: 6f6e 6527 2c0a 2020 2020 2020 2020 2020  one',.          
-00022f30: 2020 6c61 6265 6c3d 2745 7870 6572 696d    label='Experim
-00022f40: 656e 7427 2c0a 2020 2020 2020 2020 2020  ent',.          
-00022f50: 2020 636f 6c6f 723d 2762 6c61 636b 270a    color='black'.
-00022f60: 2020 2020 2020 2020 290a 2020 2020 656c          ).    el
-00022f70: 7365 3a0a 2020 2020 2020 2020 6178 2e70  se:.        ax.p
-00022f80: 6c6f 7428 0a20 2020 2020 2020 2020 2020  lot(.           
-00022f90: 2031 2e20 2f20 785f 7661 6c73 2c0a 2020   1. / x_vals,.  
-00022fa0: 2020 2020 2020 2020 2020 6e70 2e6c 6f67            np.log
-00022fb0: 2831 2e20 2f20 6461 7461 7365 742e 7261  (1. / dataset.ra
-00022fc0: 7465 7329 2c0a 2020 2020 2020 2020 2020  tes),.          
-00022fd0: 2020 6d61 726b 6572 3d27 6f27 2c0a 2020    marker='o',.  
-00022fe0: 2020 2020 2020 2020 2020 6c77 3d30 2c0a            lw=0,.
-00022ff0: 2020 2020 2020 2020 2020 2020 6669 6c6c              fill
-00023000: 7374 796c 653d 276e 6f6e 6527 2c0a 2020  style='none',.  
-00023010: 2020 2020 2020 2020 2020 6c61 6265 6c3d            label=
-00023020: 2745 7870 6572 696d 656e 7427 2c0a 2020  'Experiment',.  
-00023030: 2020 2020 2020 2020 2020 636f 6c6f 723d            color=
-00023040: 2762 6c61 636b 270a 2020 2020 2020 2020  'black'.        
-00023050: 290a 0a20 2020 2078 5f76 6172 735f 6772  )..    x_vars_gr
-00023060: 6964 203d 206e 702e 6c69 6e73 7061 6365  id = np.linspace
-00023070: 280a 2020 2020 2020 2020 6e70 2e6d 696e  (.        np.min
-00023080: 2878 5f76 616c 7329 2c0a 2020 2020 2020  (x_vals),.      
-00023090: 2020 6e70 2e6d 6178 2878 5f76 616c 7329    np.max(x_vals)
-000230a0: 2c0a 2020 2020 2020 2020 3130 3030 0a20  ,.        1000. 
-000230b0: 2020 2029 0a0a 2020 2020 6966 2074 7970     )..    if typ
-000230c0: 6528 6d6f 6465 6c29 2069 6e20 5b4d 756c  e(model) in [Mul
-000230d0: 7469 4c6f 6754 6175 544d 6f64 656c 2c20  tiLogTauTModel, 
-000230e0: 4d75 6c74 694c 6f67 5461 7548 4d6f 6465  MultiLogTauHMode
-000230f0: 6c5d 3a0a 2020 2020 2020 2020 6c6f 676d  l]:.        logm
-00023100: 6f64 656c 7320 3d20 6d6f 6465 6c2e 6c6f  odels = model.lo
-00023110: 676d 6f64 656c 730a 2020 2020 656c 7365  gmodels.    else
-00023120: 3a0a 2020 2020 2020 2020 6c6f 676d 6f64  :.        logmod
-00023130: 656c 7320 3d20 5b6d 6f64 656c 5d0a 0a20  els = [model].. 
-00023140: 2020 2066 6f72 206c 6f67 6d6f 6465 6c20     for logmodel 
-00023150: 696e 206c 6f67 6d6f 6465 6c73 3a0a 0a20  in logmodels:.. 
-00023160: 2020 2020 2020 2069 6620 7479 7065 286c         if type(l
-00023170: 6f67 6d6f 6465 6c29 2069 7320 4c6f 674f  ogmodel) is LogO
-00023180: 7262 6163 684d 6f64 656c 3a0a 2020 2020  rbachModel:.    
-00023190: 2020 2020 2020 2020 6c61 6265 6c5f 6669          label_fi
-000231a0: 7420 3d20 275c 6e46 6974 2077 6974 6827  t = '\nFit with'
-000231b0: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
-000231c0: 656c 5f66 6974 202b 3d20 275c 6e27 202b  el_fit += '\n' +
-000231d0: 2072 277b 7d20 7b3a 362e 3266 7d20 7327   r'{} {:6.2f} s'
-000231e0: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
-000231f0: 2020 2020 2020 2020 206c 6f67 6d6f 6465           logmode
-00023200: 6c2e 5641 524e 414d 4553 5f4d 4d5b 2775  l.VARNAMES_MM['u
-00023210: 5f65 6666 275d 2c0a 2020 2020 2020 2020  _eff'],.        
-00023220: 2020 2020 2020 2020 6c6f 676d 6f64 656c          logmodel
-00023230: 2e66 696e 616c 5f76 6172 5f76 616c 7565  .final_var_value
-00023240: 735b 2775 5f65 6666 275d 0a20 2020 2020  s['u_eff'].     
-00023250: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00023260: 2020 2020 206c 6162 656c 5f66 6974 202b       label_fit +
-00023270: 3d20 275c 6e27 202b 2072 277b 7d20 7b3a  = '\n' + r'{} {:
-00023280: 3034 2e33 657d 272e 666f 726d 6174 280a  04.3e}'.format(.
-00023290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000232a0: 6c6f 676d 6f64 656c 2e56 4152 4e41 4d45  logmodel.VARNAME
-000232b0: 535f 4d4d 5b27 4127 5d2c 206c 6f67 6d6f  S_MM['A'], logmo
-000232c0: 6465 6c2e 6669 6e61 6c5f 7661 725f 7661  del.final_var_va
-000232d0: 6c75 6573 5b27 4127 5d0a 2020 2020 2020  lues['A'].      
-000232e0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000232f0: 656c 6966 2074 7970 6528 6c6f 676d 6f64  elif type(logmod
-00023300: 656c 2920 6973 204c 6f67 5261 6d61 6e4d  el) is LogRamanM
-00023310: 6f64 656c 3a0a 2020 2020 2020 2020 2020  odel:.          
-00023320: 2020 6c61 6265 6c5f 6669 7420 3d20 275c    label_fit = '\
-00023330: 6e46 6974 2077 6974 6827 0a20 2020 2020  nFit with'.     
-00023340: 2020 2020 2020 206c 6162 656c 5f66 6974         label_fit
-00023350: 202b 3d20 275c 6e27 202b 2072 277b 7d20   += '\n' + r'{} 
-00023360: 7b3a 362e 3266 7d20 7327 2e66 6f72 6d61  {:6.2f} s'.forma
-00023370: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-00023380: 2020 206c 6f67 6d6f 6465 6c2e 5641 524e     logmodel.VARN
-00023390: 414d 4553 5f4d 4d5b 2752 275d 2c20 6c6f  AMES_MM['R'], lo
-000233a0: 676d 6f64 656c 2e66 696e 616c 5f76 6172  gmodel.final_var
-000233b0: 5f76 616c 7565 735b 2752 275d 0a20 2020  _values['R'].   
-000233c0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-000233d0: 2020 2020 2020 206c 6162 656c 5f66 6974         label_fit
-000233e0: 202b 3d20 275c 6e27 202b 2072 277b 7d20   += '\n' + r'{} 
-000233f0: 7b3a 3034 2e33 657d 272e 666f 726d 6174  {:04.3e}'.format
-00023400: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00023410: 2020 6c6f 676d 6f64 656c 2e56 4152 4e41    logmodel.VARNA
-00023420: 4d45 535f 4d4d 5b27 6e27 5d2c 206c 6f67  MES_MM['n'], log
-00023430: 6d6f 6465 6c2e 6669 6e61 6c5f 7661 725f  model.final_var_
-00023440: 7661 6c75 6573 5b27 6e27 5d0a 2020 2020  values['n'].    
-00023450: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00023460: 2020 656c 6966 2074 7970 6528 6c6f 676d    elif type(logm
-00023470: 6f64 656c 2920 6973 204c 6f67 5154 4d4d  odel) is LogQTMM
-00023480: 6f64 656c 3a0a 2020 2020 2020 2020 2020  odel:.          
-00023490: 2020 6c61 6265 6c5f 6669 7420 3d20 275c    label_fit = '\
-000234a0: 6e46 6974 2077 6974 6827 0a20 2020 2020  nFit with'.     
-000234b0: 2020 2020 2020 206c 6162 656c 5f66 6974         label_fit
-000234c0: 202b 3d20 275c 6e27 202b 2072 277b 7d20   += '\n' + r'{} 
-000234d0: 7b3a 362e 3266 7d20 7327 2e66 6f72 6d61  {:6.2f} s'.forma
-000234e0: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-000234f0: 2020 206c 6f67 6d6f 6465 6c2e 5641 524e     logmodel.VARN
-00023500: 414d 4553 5f4d 4d5b 2751 275d 2c20 6c6f  AMES_MM['Q'], lo
-00023510: 676d 6f64 656c 2e66 696e 616c 5f76 6172  gmodel.final_var
-00023520: 5f76 616c 7565 735b 2751 275d 0a20 2020  _values['Q'].   
-00023530: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00023540: 2020 2065 6c69 6620 7479 7065 286c 6f67     elif type(log
-00023550: 6d6f 6465 6c29 2069 7320 4c6f 6744 6972  model) is LogDir
-00023560: 6563 744d 6f64 656c 3a0a 2020 2020 2020  ectModel:.      
-00023570: 2020 2020 2020 6c61 6265 6c5f 6669 7420        label_fit 
-00023580: 3d20 275c 6e46 6974 2077 6974 6827 0a20  = '\nFit with'. 
-00023590: 2020 2020 2020 2020 2020 206c 6162 656c             label
-000235a0: 5f66 6974 202b 3d20 275c 6e27 202b 2072  _fit += '\n' + r
-000235b0: 277b 7d20 7b3a 362e 3266 7d20 7327 2e66  '{} {:6.2f} s'.f
-000235c0: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
-000235d0: 2020 2020 2020 206c 6f67 6d6f 6465 6c2e         logmodel.
-000235e0: 5641 524e 414d 4553 5f4d 4d5b 2744 275d  VARNAMES_MM['D']
-000235f0: 2c20 6c6f 676d 6f64 656c 2e66 696e 616c  , logmodel.final
-00023600: 5f76 6172 5f76 616c 7565 735b 2744 275d  _var_values['D']
-00023610: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00023620: 2020 2020 2020 206d 6f64 656c 5f72 6174         model_rat
-00023630: 6573 203d 2031 302a 2a6c 6f67 6d6f 6465  es = 10**logmode
-00023640: 6c2e 6d6f 6465 6c28 0a20 2020 2020 2020  l.model(.       
-00023650: 2020 2020 206c 6f67 6d6f 6465 6c2e 6669       logmodel.fi
-00023660: 6e61 6c5f 7661 725f 7661 6c75 6573 2c0a  nal_var_values,.
-00023670: 2020 2020 2020 2020 2020 2020 785f 7661              x_va
-00023680: 7273 5f67 7269 642c 0a20 2020 2020 2020  rs_grid,.       
-00023690: 2029 0a0a 2020 2020 2020 2020 6178 2e70   )..        ax.p
-000236a0: 6c6f 7428 0a20 2020 2020 2020 2020 2020  lot(.           
-000236b0: 2031 2e20 2f20 6e70 2e61 7272 6179 2878   1. / np.array(x
-000236c0: 5f76 6172 735f 6772 6964 292c 0a20 2020  _vars_grid),.   
-000236d0: 2020 2020 2020 2020 206e 702e 6c6f 6728           np.log(
-000236e0: 312e 202f 206e 702e 6172 7261 7928 6d6f  1. / np.array(mo
-000236f0: 6465 6c5f 7261 7465 7329 292c 0a20 2020  del_rates)),.   
-00023700: 2020 2020 2020 2020 206c 773d 312e 352c           lw=1.5,
-00023710: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
-00023720: 656c 3d6c 6f67 6d6f 6465 6c2e 4e41 4d45  el=logmodel.NAME
-00023730: 2c0a 2020 2020 2020 2020 2020 2020 6c73  ,.            ls
-00023740: 3d27 2d2d 270a 2020 2020 2020 2020 290a  ='--'.        ).
-00023750: 0a20 2020 2069 6620 7479 7065 286d 6f64  .    if type(mod
-00023760: 656c 2920 696e 205b 4d75 6c74 694c 6f67  el) in [MultiLog
-00023770: 5461 7554 4d6f 6465 6c2c 204d 756c 7469  TauTModel, Multi
-00023780: 4c6f 6754 6175 484d 6f64 656c 5d20 616e  LogTauHModel] an
-00023790: 6420 6c65 6e28 6c6f 676d 6f64 656c 7329  d len(logmodels)
-000237a0: 203e 2031 3a20 2320 6e6f 7161 0a20 2020   > 1: # noqa.   
-000237b0: 2020 2020 2074 6f74 616c 203d 206e 702e       total = np.
-000237c0: 7a65 726f 7328 6c65 6e28 785f 7661 7273  zeros(len(x_vars
-000237d0: 5f67 7269 6429 290a 0a20 2020 2020 2020  _grid))..       
-000237e0: 2066 6f72 206c 6f67 6d6f 6465 6c20 696e   for logmodel in
-000237f0: 206c 6f67 6d6f 6465 6c73 3a0a 2020 2020   logmodels:.    
-00023800: 2020 2020 2020 2020 746f 7461 6c20 2b3d          total +=
-00023810: 2031 302a 2a6c 6f67 6d6f 6465 6c2e 6d6f   10**logmodel.mo
-00023820: 6465 6c28 0a20 2020 2020 2020 2020 2020  del(.           
-00023830: 2020 2020 206c 6f67 6d6f 6465 6c2e 6669       logmodel.fi
-00023840: 6e61 6c5f 7661 725f 7661 6c75 6573 2c0a  nal_var_values,.
-00023850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023860: 785f 7661 7273 5f67 7269 642c 0a20 2020  x_vars_grid,.   
-00023870: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-00023880: 2020 2020 6178 2e70 6c6f 7428 0a20 2020      ax.plot(.   
-00023890: 2020 2020 2020 2020 2031 2e20 2f20 785f           1. / x_
-000238a0: 7661 7273 5f67 7269 642c 0a20 2020 2020  vars_grid,.     
-000238b0: 2020 2020 2020 206e 702e 6c6f 6728 312e         np.log(1.
-000238c0: 202f 2074 6f74 616c 292c 0a20 2020 2020   / total),.     
-000238d0: 2020 2020 2020 206c 773d 312e 352c 0a20         lw=1.5,. 
-000238e0: 2020 2020 2020 2020 2020 206c 6162 656c             label
-000238f0: 3d27 546f 7461 6c27 2c0a 2020 2020 2020  ='Total',.      
-00023900: 2020 2020 2020 636f 6c6f 723d 2772 6564        color='red
-00023910: 270a 2020 2020 2020 2020 290a 0a20 2020  '.        )..   
-00023920: 2023 2045 6e61 626c 6520 6d69 6e6f 7220   # Enable minor 
-00023930: 7469 636b 730a 2020 2020 6178 2e79 6178  ticks.    ax.yax
-00023940: 6973 2e73 6574 5f6d 696e 6f72 5f6c 6f63  is.set_minor_loc
-00023950: 6174 6f72 2841 7574 6f4d 696e 6f72 4c6f  ator(AutoMinorLo
-00023960: 6361 746f 7228 2929 0a20 2020 2061 782e  cator()).    ax.
-00023970: 7861 7869 732e 7365 745f 6d69 6e6f 725f  xaxis.set_minor_
-00023980: 6c6f 6361 746f 7228 4175 746f 4d69 6e6f  locator(AutoMino
-00023990: 724c 6f63 6174 6f72 2829 290a 0a20 2020  rLocator())..   
-000239a0: 2065 7870 7265 7373 696f 6e20 3d20 2727   expression = ''
-000239b0: 0a0a 2020 2020 666f 7220 6c6f 676d 6f64  ..    for logmod
-000239c0: 656c 2069 6e20 6c6f 676d 6f64 656c 733a  el in logmodels:
-000239d0: 0a20 2020 2020 2020 2066 6f72 2069 742c  .        for it,
-000239e0: 206e 616d 6520 696e 2065 6e75 6d65 7261   name in enumera
-000239f0: 7465 286c 6f67 6d6f 6465 6c2e 5041 524e  te(logmodel.PARN
-00023a00: 414d 4553 293a 0a20 2020 2020 2020 2020  AMES):.         
-00023a10: 2020 2065 7870 7265 7373 696f 6e20 2b3d     expression +=
-00023a20: 2027 7b7d 203d 207b 3a2e 3366 7d20 272e   '{} = {:.3f} '.
-00023a30: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
-00023a40: 2020 2020 2020 2020 6c6f 676d 6f64 656c          logmodel
-00023a50: 2e56 4152 4e41 4d45 535f 4d4d 5b6e 616d  .VARNAMES_MM[nam
-00023a60: 655d 2c0a 2020 2020 2020 2020 2020 2020  e],.            
-00023a70: 2020 2020 6c6f 676d 6f64 656c 2e66 696e      logmodel.fin
-00023a80: 616c 5f76 6172 5f76 616c 7565 735b 6e61  al_var_values[na
-00023a90: 6d65 5d2c 0a20 2020 2020 2020 2020 2020  me],.           
-00023aa0: 2029 0a20 2020 2020 2020 2020 2020 2069   ).            i
-00023ab0: 6620 6e61 6d65 2069 6e20 6c6f 676d 6f64  f name in logmod
-00023ac0: 656c 2e66 6974 5f76 6172 732e 6b65 7973  el.fit_vars.keys
-00023ad0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00023ae0: 2020 2020 6578 7072 6573 7369 6f6e 202b      expression +
-00023af0: 3d20 7227 245c 706d 2420 270a 2020 2020  = r'$\pm$ '.    
-00023b00: 2020 2020 2020 2020 2020 2020 6578 7072              expr
-00023b10: 6573 7369 6f6e 202b 3d20 277b 3a2e 3366  ession += '{:.3f
-00023b20: 7d20 272e 666f 726d 6174 286c 6f67 6d6f  } '.format(logmo
-00023b30: 6465 6c2e 6669 745f 7374 6465 765b 6e61  del.fit_stdev[na
-00023b40: 6d65 5d29 0a20 2020 2020 2020 2020 2020  me]).           
-00023b50: 2065 7870 7265 7373 696f 6e20 2b3d 2027   expression += '
-00023b60: 7b7d 2020 2020 272e 666f 726d 6174 286c  {}    '.format(l
-00023b70: 6f67 6d6f 6465 6c2e 554e 4954 535f 4d4d  ogmodel.UNITS_MM
-00023b80: 5b6e 616d 655d 290a 2020 2020 2020 2020  [name]).        
-00023b90: 2020 2020 6966 2069 7420 3d3d 2031 2061      if it == 1 a
-00023ba0: 6e64 206c 656e 286c 6f67 6d6f 6465 6c2e  nd len(logmodel.
-00023bb0: 6669 745f 7661 7273 2e6b 6579 7328 2929  fit_vars.keys())
-00023bc0: 203e 2032 3a0a 2020 2020 2020 2020 2020   > 2:.          
-00023bd0: 2020 2020 2020 6578 7072 6573 7369 6f6e        expression
-00023be0: 202b 3d20 275c 6e27 0a20 2020 2020 2020   += '\n'.       
-00023bf0: 2065 7870 7265 7373 696f 6e20 2b3d 2027   expression += '
-00023c00: 5c6e 270a 0a20 2020 2069 6620 7368 6f77  \n'..    if show
-00023c10: 5f70 6172 616d 733a 0a20 2020 2020 2020  _params:.       
-00023c20: 2061 782e 7465 7874 280a 2020 2020 2020   ax.text(.      
-00023c30: 2020 2020 2020 302e 302c 2031 2e30 322c        0.0, 1.02,
-00023c40: 2073 3d65 7870 7265 7373 696f 6e2c 2066   s=expression, f
-00023c50: 6f6e 7473 697a 653d 3130 2c20 7472 616e  ontsize=10, tran
-00023c60: 7366 6f72 6d3d 6178 2e74 7261 6e73 4178  sform=ax.transAx
-00023c70: 6573 0a20 2020 2020 2020 2029 0a0a 2020  es.        )..  
-00023c80: 2020 6966 2078 5f74 7970 6520 3d3d 2027    if x_type == '
-00023c90: 6669 656c 6427 3a0a 2020 2020 2020 2020  field':.        
-00023ca0: 6178 2e6c 6567 656e 6428 0a20 2020 2020  ax.legend(.     
-00023cb0: 2020 2020 2020 2066 6f6e 7473 697a 653d         fontsize=
-00023cc0: 2731 3027 2c20 6e75 6d70 6f69 6e74 733d  '10', numpoints=
-00023cd0: 312c 206e 636f 6c3d 312c 2066 7261 6d65  1, ncol=1, frame
-00023ce0: 6f6e 3d46 616c 7365 0a20 2020 2020 2020  on=False.       
-00023cf0: 2029 0a20 2020 2065 6c73 653a 0a20 2020   ).    else:.   
-00023d00: 2020 2020 2061 782e 6c65 6765 6e64 280a       ax.legend(.
-00023d10: 2020 2020 2020 2020 2020 2020 6c6f 633d              loc=
-00023d20: 276c 6f77 6572 2072 6967 6874 272c 2066  'lower right', f
-00023d30: 6f6e 7473 697a 653d 2731 3027 2c20 6e75  ontsize='10', nu
-00023d40: 6d70 6f69 6e74 733d 312c 206e 636f 6c3d  mpoints=1, ncol=
-00023d50: 312c 0a20 2020 2020 2020 2020 2020 2066  1,.            f
-00023d60: 7261 6d65 6f6e 3d46 616c 7365 0a20 2020  rameon=False.   
-00023d70: 2020 2020 2029 0a0a 2020 2020 6178 2e73       )..    ax.s
-00023d80: 6574 5f79 6c61 6265 6c28 7227 245c 6c6e  et_ylabel(r'$\ln
-00023d90: 5c6c 6566 745b 5c74 6175 5c72 6967 6874  \left[\tau\right
-00023da0: 5d24 2028 245c 6c6e 5c6c 6566 745b 5c6d  ]$ ($\ln\left[\m
-00023db0: 6174 6872 6567 756c 6172 7b73 7d5e 5c6d  athregular{s}^\m
-00023dc0: 6174 6872 6567 756c 6172 7b2d 317d 5c72  athregular{-1}\r
-00023dd0: 6967 6874 5d24 2927 2920 2320 6e6f 7161  ight]$)') # noqa
-00023de0: 0a0a 2020 2020 7265 7475 726e 0a0a 0a64  ..    return...d
-00023df0: 6566 2070 6c6f 745f 6669 7474 6564 5f72  ef plot_fitted_r
-00023e00: 6174 6573 2864 6174 6173 6574 3a20 5461  ates(dataset: Ta
-00023e10: 7554 4461 7461 7365 7420 7c20 5461 7548  uTDataset | TauH
-00023e20: 4461 7461 7365 742c 0a20 2020 2020 2020  Dataset,.       
-00023e30: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00023e40: 6f64 656c 3a20 4c6f 6754 6175 544d 6f64  odel: LogTauTMod
-00023e50: 656c 207c 204d 756c 7469 4c6f 6754 6175  el | MultiLogTau
-00023e60: 544d 6f64 656c 207c 204c 6f67 5461 7548  TModel | LogTauH
-00023e70: 4d6f 6465 6c20 7c20 4d75 6c74 694c 6f67  Model | MultiLog
-00023e80: 5461 7548 4d6f 6465 6c2c 2023 206e 6f71  TauHModel, # noq
-00023e90: 610a 2020 2020 2020 2020 2020 2020 2020  a.              
-00023ea0: 2020 2020 2020 2020 7368 6f77 3a20 626f          show: bo
-00023eb0: 6f6c 203d 2054 7275 652c 2073 6176 653a  ol = True, save:
-00023ec0: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
-00023ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023ee0: 2020 2020 2073 6176 655f 6e61 6d65 3a20       save_name: 
-00023ef0: 7374 7220 3d20 2766 6974 7465 645f 7261  str = 'fitted_ra
-00023f00: 7465 732e 706e 6727 2c0a 2020 2020 2020  tes.png',.      
+0001e430: 2020 2020 6d6f 6465 6c3a 204c 6f67 5461      model: LogTa
+0001e440: 7554 4d6f 6465 6c20 7c20 4c6f 6754 6175  uTModel | LogTau
+0001e450: 484d 6f64 656c 2920 2d3e 204e 6f6e 653a  HModel) -> None:
+0001e460: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
+0001e470: 2020 2020 2043 616c 6c62 6163 6b20 666f       Callback fo
+0001e480: 7220 746f 6767 6c69 6e67 206d 6f64 656c  r toggling model
+0001e490: 2063 6865 636b 626f 7865 730a 0a20 2020   checkboxes..   
+0001e4a0: 2020 2020 2043 616c 6375 6c61 7465 7320       Calculates 
+0001e4b0: 6d6f 6465 6c20 6461 7461 2c20 6164 6473  model data, adds
+0001e4c0: 2f64 656c 6574 6573 206c 696e 6520 6672  /deletes line fr
+0001e4d0: 6f6d 2070 6c6f 740a 2020 2020 2020 2020  om plot.        
+0001e4e0: 616e 6420 7570 6461 7465 7320 746f 7461  and updates tota
+0001e4f0: 6c20 6d6f 6465 6c20 706c 6f74 0a20 2020  l model plot.   
+0001e500: 2020 2020 2027 2727 0a0a 2020 2020 2020       '''..      
+0001e510: 2020 6d6f 6465 6c6e 616d 6520 3d20 6d6f    modelname = mo
+0001e520: 6465 6c2e 4e41 4d45 2e6c 6f77 6572 2829  del.NAME.lower()
+0001e530: 0a0a 2020 2020 2020 2020 2320 436f 6e76  ..        # Conv
+0001e540: 6572 7420 7661 6c20 746f 2062 6f6f 6c0a  ert val to bool.
+0001e550: 2020 2020 2020 2020 7661 6c20 3d20 626f          val = bo
+0001e560: 6f6c 2876 616c 202f 2032 290a 0a20 2020  ol(val / 2)..   
+0001e570: 2020 2020 2023 2055 7064 6174 6520 6c69       # Update li
+0001e580: 7374 206f 6620 6d6f 6465 6c73 0a20 2020  st of models.   
+0001e590: 2020 2020 2073 656c 662e 7573 656c 2e6d       self.usel.m
+0001e5a0: 6f64 656c 735b 6d6f 6465 6c6e 616d 655d  odels[modelname]
+0001e5b0: 203d 2076 616c 0a0a 2020 2020 2020 2020   = val..        
+0001e5c0: 2320 5570 6461 7465 206d 6f64 656c 2076  # Update model v
+0001e5d0: 616c 7565 7320 616e 6420 706c 6f74 2064  alues and plot d
+0001e5e0: 6174 6120 666f 7220 6561 6368 206d 6f64  ata for each mod
+0001e5f0: 656c 2c20 616e 6420 666f 7220 746f 7461  el, and for tota
+0001e600: 6c0a 2020 2020 2020 2020 666f 7220 7061  l.        for pa
+0001e610: 726e 616d 6520 696e 206d 6f64 656c 2e50  rname in model.P
+0001e620: 4152 4e41 4d45 533a 0a20 2020 2020 2020  ARNAMES:.       
+0001e630: 2020 2020 2073 656c 662e 7570 6461 7465       self.update
+0001e640: 5f6d 6f64 656c 706c 6f74 280a 2020 2020  _modelplot(.    
+0001e650: 2020 2020 2020 2020 2020 2020 6765 7461              geta
+0001e660: 7474 7228 7365 6c66 2e70 6172 7374 6f72  ttr(self.parstor
+0001e670: 652c 2070 6172 6e61 6d65 292c 0a20 2020  e, parname),.   
+0001e680: 2020 2020 2020 2020 2020 2020 2070 6172               par
+0001e690: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
+0001e6a0: 2020 2020 2020 6d6f 6465 6c0a 2020 2020        model.    
+0001e6b0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0001e6c0: 2020 2023 2053 656c 6563 7420 6d6f 6465     # Select mode
+0001e6d0: 6c20 706c 6f74 2074 6f20 746f 6767 6c65  l plot to toggle
+0001e6e0: 0a20 2020 2020 2020 205f 706c 6f74 203d  .        _plot =
+0001e6f0: 2073 656c 662e 6d6f 6465 6c5f 706c 6f74   self.model_plot
+0001e700: 735b 6d6f 6465 6c6e 616d 655d 0a0a 2020  s[modelname]..  
+0001e710: 2020 2020 2020 2320 4164 6420 6261 636b        # Add back
+0001e720: 2069 6e20 706c 6f74 0a20 2020 2020 2020   in plot.       
+0001e730: 2069 6620 7661 6c3a 0a20 2020 2020 2020   if val:.       
+0001e740: 2020 2020 2073 656c 662e 706c 6f74 5f77       self.plot_w
+0001e750: 6964 6765 742e 7265 6d6f 7665 4974 656d  idget.removeItem
+0001e760: 285f 706c 6f74 290a 2020 2020 2020 2020  (_plot).        
+0001e770: 2020 2020 7365 6c66 2e70 6c6f 745f 7769      self.plot_wi
+0001e780: 6467 6574 2e61 6464 4974 656d 285f 706c  dget.addItem(_pl
+0001e790: 6f74 290a 2020 2020 2020 2020 656c 7365  ot).        else
+0001e7a0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0001e7b0: 6c66 2e70 6c6f 745f 7769 6467 6574 2e72  lf.plot_widget.r
+0001e7c0: 656d 6f76 6549 7465 6d28 5f70 6c6f 7429  emoveItem(_plot)
+0001e7d0: 0a0a 2020 2020 2020 2020 2320 456e 6162  ..        # Enab
+0001e7e0: 6c65 2074 6f74 616c 2070 6c6f 7420 6966  le total plot if
+0001e7f0: 203e 2031 206d 6f64 656c 0a20 2020 2020   > 1 model.     
+0001e800: 2020 2023 2061 6e64 2065 6e61 626c 6520     # and enable 
+0001e810: 6669 7420 6275 7474 6f6e 2069 6620 3e20  fit button if > 
+0001e820: 3020 6d6f 6465 6c73 0a20 2020 2020 2020  0 models.       
+0001e830: 206e 5f6d 6f64 656c 7320 3d20 6e70 2e73   n_models = np.s
+0001e840: 756d 285b 7661 6c20 666f 7220 7661 6c20  um([val for val 
+0001e850: 696e 2073 656c 662e 7573 656c 2e6d 6f64  in self.usel.mod
+0001e860: 656c 732e 7661 6c75 6573 2829 5d29 0a20  els.values()]). 
+0001e870: 2020 2020 2020 2069 6620 6e5f 6d6f 6465         if n_mode
+0001e880: 6c73 203d 3d20 303a 0a20 2020 2020 2020  ls == 0:.       
+0001e890: 2020 2020 2073 656c 662e 6669 745f 6274       self.fit_bt
+0001e8a0: 6e5f 7769 6467 6574 2e73 6574 456e 6162  n_widget.setEnab
+0001e8b0: 6c65 6428 4661 6c73 6529 0a20 2020 2020  led(False).     
+0001e8c0: 2020 2065 6c69 6620 6e5f 6d6f 6465 6c73     elif n_models
+0001e8d0: 203d 3d20 313a 0a20 2020 2020 2020 2020   == 1:.         
+0001e8e0: 2020 2073 656c 662e 6669 745f 6274 6e5f     self.fit_btn_
+0001e8f0: 7769 6467 6574 2e73 6574 456e 6162 6c65  widget.setEnable
+0001e900: 6428 5472 7565 290a 2020 2020 2020 2020  d(True).        
+0001e910: 2020 2020 7365 6c66 2e70 6c6f 745f 7769      self.plot_wi
+0001e920: 6467 6574 2e72 656d 6f76 6549 7465 6d28  dget.removeItem(
+0001e930: 7365 6c66 2e74 6f74 290a 2020 2020 2020  self.tot).      
+0001e940: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0001e950: 2020 2020 7365 6c66 2e66 6974 5f62 746e      self.fit_btn
+0001e960: 5f77 6964 6765 742e 7365 7445 6e61 626c  _widget.setEnabl
+0001e970: 6564 2854 7275 6529 0a20 2020 2020 2020  ed(True).       
+0001e980: 2020 2020 2073 656c 662e 706c 6f74 5f77       self.plot_w
+0001e990: 6964 6765 742e 7265 6d6f 7665 4974 656d  idget.removeItem
+0001e9a0: 2873 656c 662e 746f 7429 0a20 2020 2020  (self.tot).     
+0001e9b0: 2020 2020 2020 2073 656c 662e 706c 6f74         self.plot
+0001e9c0: 5f77 6964 6765 742e 6164 6449 7465 6d28  _widget.addItem(
+0001e9d0: 7365 6c66 2e74 6f74 290a 0a20 2020 2020  self.tot)..     
+0001e9e0: 2020 2023 2045 6e61 626c 652f 4469 7361     # Enable/Disa
+0001e9f0: 626c 6520 736c 6964 6572 2c20 6368 6563  ble slider, chec
+0001ea00: 6b62 6f78 2c20 616e 6420 6669 7466 6978  kbox, and fitfix
+0001ea10: 0a20 2020 2020 2020 2066 6f72 2070 6172  .        for par
+0001ea20: 6e61 6d65 2069 6e20 6d6f 6465 6c2e 5041  name in model.PA
+0001ea30: 524e 414d 4553 3a0a 2020 2020 2020 2020  RNAMES:.        
+0001ea40: 2020 2020 7365 6c66 2e77 6964 6765 7464      self.widgetd
+0001ea50: 6963 745b 6d6f 6465 6c6e 616d 655d 5b70  ict[modelname][p
+0001ea60: 6172 6e61 6d65 5d5b 2773 6c69 6465 7227  arname]['slider'
+0001ea70: 5d2e 7365 7445 6e61 626c 6564 2876 616c  ].setEnabled(val
+0001ea80: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+0001ea90: 6c66 2e77 6964 6765 7464 6963 745b 6d6f  lf.widgetdict[mo
+0001eaa0: 6465 6c6e 616d 655d 5b70 6172 6e61 6d65  delname][parname
+0001eab0: 5d5b 2765 6e74 7279 275d 2e73 6574 456e  ]['entry'].setEn
+0001eac0: 6162 6c65 6428 7661 6c29 0a20 2020 2020  abled(val).     
+0001ead0: 2020 2020 2020 2073 656c 662e 7769 6467         self.widg
+0001eae0: 6574 6469 6374 5b6d 6f64 656c 6e61 6d65  etdict[modelname
+0001eaf0: 5d5b 7061 726e 616d 655d 5b27 6666 5f74  ][parname]['ff_t
+0001eb00: 6f67 676c 6527 5d2e 7365 7445 6e61 626c  oggle'].setEnabl
+0001eb10: 6564 2876 616c 290a 0a20 2020 2020 2020  ed(val)..       
+0001eb20: 2072 6574 7572 6e0a 0a20 2020 2064 6566   return..    def
+0001eb30: 206d 616b 655f 6d6f 6465 6c62 6f78 2873   make_modelbox(s
+0001eb40: 656c 662c 206d 6f64 656c 3a20 4c6f 6754  elf, model: LogT
+0001eb50: 6175 544d 6f64 656c 2c20 7061 7265 6e74  auTModel, parent
+0001eb60: 2c20 696e 6465 783a 2069 6e74 293a 0a20  , index: int):. 
+0001eb70: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+0001eb80: 2020 2043 7265 6174 6573 2077 6964 6765     Creates widge
+0001eb90: 7420 666f 7220 6120 6769 7665 6e20 6d6f  t for a given mo
+0001eba0: 6465 6c2c 2063 6f6e 7461 696e 696e 6720  del, containing 
+0001ebb0: 6120 6368 6563 6b62 6f78 2074 6f20 746f  a checkbox to to
+0001ebc0: 6767 6c65 0a20 2020 2020 2020 2074 6865  ggle.        the
+0001ebd0: 206d 6f64 656c 2c20 616e 6420 6120 726f   model, and a ro
+0001ebe0: 7720 6f66 2069 6e74 6572 6163 7469 7665  w of interactive
+0001ebf0: 2077 6964 6765 7473 2066 6f72 2065 6163   widgets for eac
+0001ec00: 6820 7061 7261 6d65 7465 7220 6f66 2074  h parameter of t
+0001ec10: 6865 0a20 2020 2020 2020 206d 6f64 656c  he.        model
+0001ec20: 0a20 2020 2020 2020 2027 2727 0a0a 2020  .        '''..  
+0001ec30: 2020 2020 2020 2320 5769 6467 6574 2066        # Widget f
+0001ec40: 6f72 2074 6869 7320 6d6f 6465 6c0a 2020  or this model.  
+0001ec50: 2020 2020 2020 6d6f 6465 6c5f 7769 6467        model_widg
+0001ec60: 6574 203d 2051 7457 6964 6765 7473 2e51  et = QtWidgets.Q
+0001ec70: 5769 6467 6574 2870 6172 656e 743d 7061  Widget(parent=pa
+0001ec80: 7265 6e74 290a 2020 2020 2020 2020 6d6f  rent).        mo
+0001ec90: 6465 6c5f 6c61 796f 7574 203d 2051 7457  del_layout = QtW
+0001eca0: 6964 6765 7473 2e51 4842 6f78 4c61 796f  idgets.QHBoxLayo
+0001ecb0: 7574 286d 6f64 656c 5f77 6964 6765 7429  ut(model_widget)
+0001ecc0: 0a0a 2020 2020 2020 2020 2320 4372 6561  ..        # Crea
+0001ecd0: 7465 2074 6963 6b62 6f78 2074 6f20 746f  te tickbox to to
+0001ece0: 6767 6c65 2074 6869 7320 7769 6467 6574  ggle this widget
+0001ecf0: 0a20 2020 2020 2020 2074 6963 6b62 6f78  .        tickbox
+0001ed00: 5f77 6964 6765 7420 3d20 5174 5769 6467  _widget = QtWidg
+0001ed10: 6574 732e 5143 6865 636b 426f 7828 0a20  ets.QCheckBox(. 
+0001ed20: 2020 2020 2020 2020 2020 2070 6172 656e             paren
+0001ed30: 743d 6d6f 6465 6c5f 7769 6467 6574 2c0a  t=model_widget,.
+0001ed40: 2020 2020 2020 2020 2020 2020 7465 7874              text
+0001ed50: 3d6d 6f64 656c 2e4e 414d 452e 7265 706c  =model.NAME.repl
+0001ed60: 6163 6528 2742 726f 6e73 2d56 616e 2d56  ace('Brons-Van-V
+0001ed70: 6c65 636b 272c 2027 4256 5627 292c 0a0a  leck', 'BVV'),..
+0001ed80: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0001ed90: 2020 2023 2041 6464 2074 6963 6b62 6f78     # Add tickbox
+0001eda0: 2074 6f20 7468 6973 206d 6f64 656c 0a20   to this model. 
+0001edb0: 2020 2020 2020 206d 6f64 656c 5f6c 6179         model_lay
+0001edc0: 6f75 742e 6164 6457 6964 6765 7428 7469  out.addWidget(ti
+0001edd0: 636b 626f 785f 7769 6467 6574 290a 0a20  ckbox_widget).. 
+0001ede0: 2020 2020 2020 2023 2041 6464 2074 6f20         # Add to 
+0001edf0: 6469 6374 696f 6e61 7279 206f 6620 616c  dictionary of al
+0001ee00: 6c20 7469 636b 626f 7865 732c 2069 6e64  l tickboxes, ind
+0001ee10: 6578 6564 2062 7920 6d6f 6465 6c2e 4e41  exed by model.NA
+0001ee20: 4d45 2e6c 6f77 6572 2829 0a20 2020 2020  ME.lower().     
+0001ee30: 2020 2073 656c 662e 7469 636b 6469 6374     self.tickdict
+0001ee40: 5b6d 6f64 656c 2e4e 414d 452e 6c6f 7765  [model.NAME.lowe
+0001ee50: 7228 295d 203d 2074 6963 6b62 6f78 5f77  r()] = tickbox_w
+0001ee60: 6964 6765 740a 0a20 2020 2020 2020 2023  idget..        #
+0001ee70: 2057 6865 6e20 746f 6767 6c65 642c 2070   When toggled, p
+0001ee80: 6c6f 7420 7468 6973 206d 6f64 656c 0a20  lot this model. 
+0001ee90: 2020 2020 2020 2074 6963 6b62 6f78 5f77         tickbox_w
+0001eea0: 6964 6765 742e 7374 6174 6543 6861 6e67  idget.stateChang
+0001eeb0: 6564 2e63 6f6e 6e65 6374 280a 2020 2020  ed.connect(.    
+0001eec0: 2020 2020 2020 2020 6c61 6d62 6461 2076          lambda v
+0001eed0: 616c 3a20 7365 6c66 2e74 6f67 676c 655f  al: self.toggle_
+0001eee0: 706c 6f74 2876 616c 2c20 6d6f 6465 6c29  plot(val, model)
+0001eef0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+0001ef00: 2020 2020 2320 4164 6420 6162 696c 6974      # Add abilit
+0001ef10: 7920 746f 2074 6f67 676c 6520 6d6f 6465  y to toggle mode
+0001ef20: 6c20 7573 696e 6720 6e75 6d62 6572 206b  l using number k
+0001ef30: 6579 0a20 2020 2020 2020 206f 6e5f 6f66  ey.        on_of
+0001ef40: 665f 7368 6f72 7463 7574 203d 2051 7457  f_shortcut = QtW
+0001ef50: 6964 6765 7473 2e51 5368 6f72 7463 7574  idgets.QShortcut
+0001ef60: 280a 2020 2020 2020 2020 2020 2020 5174  (.            Qt
+0001ef70: 4775 692e 514b 6579 5365 7175 656e 6365  Gui.QKeySequence
+0001ef80: 2827 7b3a 647d 272e 666f 726d 6174 2869  ('{:d}'.format(i
+0001ef90: 6e64 6578 2929 2c0a 2020 2020 2020 2020  ndex)),.        
+0001efa0: 2020 2020 7365 6c66 0a20 2020 2020 2020      self.       
+0001efb0: 2029 0a20 2020 2020 2020 206f 6e5f 6f66   ).        on_of
+0001efc0: 665f 7368 6f72 7463 7574 2e61 6374 6976  f_shortcut.activ
+0001efd0: 6174 6564 2e63 6f6e 6e65 6374 280a 2020  ated.connect(.  
+0001efe0: 2020 2020 2020 2020 2020 6c61 6d62 6461            lambda
+0001eff0: 3a20 7469 636b 626f 785f 7769 6467 6574  : tickbox_widget
+0001f000: 2e74 6f67 676c 6528 290a 2020 2020 2020  .toggle().      
+0001f010: 2020 290a 2020 2020 2020 2020 7365 6c66    ).        self
+0001f020: 2e6f 6e5f 6f66 665f 7368 6f72 7463 7574  .on_off_shortcut
+0001f030: 2e61 7070 656e 6428 6f6e 5f6f 6666 5f73  .append(on_off_s
+0001f040: 686f 7274 6375 7429 0a0a 2020 2020 2020  hortcut)..      
+0001f050: 2020 2320 4372 6561 7465 2063 6f6e 7461    # Create conta
+0001f060: 696e 6572 2077 6964 6765 7420 666f 7220  iner widget for 
+0001f070: 616c 6c20 7061 7261 6d65 7465 7220 726f  all parameter ro
+0001f080: 7773 0a20 2020 2020 2020 2072 6873 5f77  ws.        rhs_w
+0001f090: 6964 6765 7420 3d20 5174 5769 6467 6574  idget = QtWidget
+0001f0a0: 732e 5157 6964 6765 7428 7061 7265 6e74  s.QWidget(parent
+0001f0b0: 3d6d 6f64 656c 5f77 6964 6765 7429 0a20  =model_widget). 
+0001f0c0: 2020 2020 2020 2072 6873 5f6c 6179 6f75         rhs_layou
+0001f0d0: 7420 3d20 5174 5769 6467 6574 732e 5156  t = QtWidgets.QV
+0001f0e0: 426f 784c 6179 6f75 7428 7268 735f 7769  BoxLayout(rhs_wi
+0001f0f0: 6467 6574 290a 0a20 2020 2020 2020 2023  dget)..        #
+0001f100: 204d 616b 6520 736c 6964 6572 2c20 7465   Make slider, te
+0001f110: 7874 626f 782c 2061 6e64 2066 6974 2f66  xtbox, and fit/f
+0001f120: 6978 2074 6f67 676c 6520 666f 7220 6561  ix toggle for ea
+0001f130: 6368 0a20 2020 2020 2020 2023 2070 6172  ch.        # par
+0001f140: 616d 6574 6572 206f 6620 7468 6520 6375  ameter of the cu
+0001f150: 7272 656e 7420 6d6f 6465 6c0a 2020 2020  rrent model.    
+0001f160: 2020 2020 666f 7220 7061 726e 616d 6520      for parname 
+0001f170: 696e 206d 6f64 656c 2e50 4152 4e41 4d45  in model.PARNAME
+0001f180: 533a 0a0a 2020 2020 2020 2020 2020 2020  S:..            
+0001f190: 2320 4465 6661 756c 7420 7061 7261 6d65  # Default parame
+0001f1a0: 7465 7220 7661 6c75 6573 0a20 2020 2020  ter values.     
+0001f1b0: 2020 2020 2020 205f 6465 6661 756c 7473         _defaults
+0001f1c0: 203d 2073 656c 662e 6465 6661 756c 7473   = self.defaults
+0001f1d0: 5b6d 6f64 656c 2e4e 414d 455d 5b70 6172  [model.NAME][par
+0001f1e0: 6e61 6d65 5d0a 0a20 2020 2020 2020 2020  name]..         
+0001f1f0: 2020 2023 204e 616d 6520 616e 6420 556e     # Name and Un
+0001f200: 6974 7320 6173 2073 7472 696e 670a 2020  its as string.  
+0001f210: 2020 2020 2020 2020 2020 5f6e 755f 7374            _nu_st
+0001f220: 7269 6e67 203d 2027 7b7d 2028 7b7d 2927  ring = '{} ({})'
+0001f230: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
+0001f240: 2020 2020 2020 2020 206d 6f64 656c 2e56           model.V
+0001f250: 4152 4e41 4d45 535f 4854 4d4c 5b70 6172  ARNAMES_HTML[par
+0001f260: 6e61 6d65 5d2c 0a20 2020 2020 2020 2020  name],.         
+0001f270: 2020 2020 2020 206d 6f64 656c 2e55 4e49         model.UNI
+0001f280: 5453 5f48 544d 4c5b 7061 726e 616d 655d  TS_HTML[parname]
+0001f290: 0a20 2020 2020 2020 2020 2020 2029 2e72  .            ).r
+0001f2a0: 6570 6c61 6365 2827 2829 272c 2027 2729  eplace('()', '')
+0001f2b0: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0001f2c0: 4361 6c6c 6261 636b 2066 6f72 2069 6e74  Callback for int
+0001f2d0: 6572 6163 7469 6f6e 2077 6974 6820 736c  eraction with sl
+0001f2e0: 6964 6572 2c20 7465 7874 626f 782e 2e2e  ider, textbox...
+0001f2f0: 0a20 2020 2020 2020 2020 2020 2063 6220  .            cb 
+0001f300: 3d20 7061 7274 6961 6c28 7365 6c66 2e75  = partial(self.u
+0001f310: 7064 6174 655f 6d6f 6465 6c70 6c6f 742c  pdate_modelplot,
+0001f320: 206d 6f64 656c 3d6d 6f64 656c 2c20 7061   model=model, pa
+0001f330: 726e 616d 653d 7061 726e 616d 6529 0a0a  rname=parname)..
+0001f340: 2020 2020 2020 2020 2020 2020 2320 4d61              # Ma
+0001f350: 6b65 2072 6f77 206f 6620 7769 6467 6574  ke row of widget
+0001f360: 7320 666f 7220 7468 6973 2070 6172 616d  s for this param
+0001f370: 6574 6572 0a20 2020 2020 2020 2020 2020  eter.           
+0001f380: 2070 6172 626f 785f 7769 6467 6574 2c20   parbox_widget, 
+0001f390: 7061 7262 6f78 5f6c 6179 6f75 7420 3d20  parbox_layout = 
+0001f3a0: 7365 6c66 2e6d 616b 655f 7061 7262 6f78  self.make_parbox
+0001f3b0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0001f3c0: 2020 6362 2c20 7061 726e 616d 652c 205f    cb, parname, _
+0001f3d0: 6e75 5f73 7472 696e 672c 205f 6465 6661  nu_string, _defa
+0001f3e0: 756c 7473 2c20 6d6f 6465 6c5f 7769 6467  ults, model_widg
+0001f3f0: 6574 2c0a 2020 2020 2020 2020 2020 2020  et,.            
+0001f400: 2020 2020 6d6f 6465 6c2e 4e41 4d45 2e6c      model.NAME.l
+0001f410: 6f77 6572 2829 0a20 2020 2020 2020 2020  ower().         
+0001f420: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
+0001f430: 2020 2320 616e 6420 6164 6420 746f 2074    # and add to t
+0001f440: 6865 206d 6f64 656c 2773 2062 6f78 206f  he model's box o
+0001f450: 6620 7061 7261 6d65 7465 720a 2020 2020  f parameter.    
+0001f460: 2020 2020 2020 2020 7268 735f 6c61 796f          rhs_layo
+0001f470: 7574 2e61 6464 5769 6467 6574 2870 6172  ut.addWidget(par
+0001f480: 626f 785f 7769 6467 6574 290a 0a20 2020  box_widget)..   
+0001f490: 2020 2020 2023 2053 6574 2065 7870 616e       # Set expan
+0001f4a0: 7369 6f6e 2062 6568 6176 696f 7572 2061  sion behaviour a
+0001f4b0: 6e64 2063 656e 7465 7269 6e67 206f 6620  nd centering of 
+0001f4c0: 7769 6467 6574 730a 2020 2020 2020 2020  widgets.        
+0001f4d0: 7268 735f 6c61 796f 7574 2e73 6574 416c  rhs_layout.setAl
+0001f4e0: 6967 6e6d 656e 7428 5174 436f 7265 2e51  ignment(QtCore.Q
+0001f4f0: 742e 416c 6967 6e56 4365 6e74 6572 290a  t.AlignVCenter).
+0001f500: 2020 2020 2020 2020 7268 735f 7769 6467          rhs_widg
+0001f510: 6574 2e73 6574 5369 7a65 506f 6c69 6379  et.setSizePolicy
+0001f520: 280a 2020 2020 2020 2020 2020 2020 5174  (.            Qt
+0001f530: 5769 6467 6574 732e 5153 697a 6550 6f6c  Widgets.QSizePol
+0001f540: 6963 792e 4669 7865 642c 0a20 2020 2020  icy.Fixed,.     
+0001f550: 2020 2020 2020 2051 7457 6964 6765 7473         QtWidgets
+0001f560: 2e51 5369 7a65 506f 6c69 6379 2e46 6978  .QSizePolicy.Fix
+0001f570: 6564 0a20 2020 2020 2020 2029 0a20 2020  ed.        ).   
+0001f580: 2020 2020 2074 6963 6b62 6f78 5f77 6964       tickbox_wid
+0001f590: 6765 742e 7365 7453 697a 6550 6f6c 6963  get.setSizePolic
+0001f5a0: 7928 0a20 2020 2020 2020 2020 2020 2051  y(.            Q
+0001f5b0: 7457 6964 6765 7473 2e51 5369 7a65 506f  tWidgets.QSizePo
+0001f5c0: 6c69 6379 2e46 6978 6564 2c0a 2020 2020  licy.Fixed,.    
+0001f5d0: 2020 2020 2020 2020 5174 5769 6467 6574          QtWidget
+0001f5e0: 732e 5153 697a 6550 6f6c 6963 792e 4669  s.QSizePolicy.Fi
+0001f5f0: 7865 640a 2020 2020 2020 2020 290a 0a20  xed.        ).. 
+0001f600: 2020 2020 2020 2072 6873 5f6c 6179 6f75         rhs_layou
+0001f610: 742e 7365 7453 7061 6369 6e67 2830 290a  t.setSpacing(0).
+0001f620: 2020 2020 2020 2020 7268 735f 6c61 796f          rhs_layo
+0001f630: 7574 2e61 6464 5374 7265 7463 6828 3429  ut.addStretch(4)
+0001f640: 0a0a 2020 2020 2020 2020 2320 4164 6420  ..        # Add 
+0001f650: 7061 7261 6d65 7465 7220 726f 7773 2074  parameter rows t
+0001f660: 6f20 7468 6973 206d 6f64 656c 0a20 2020  o this model.   
+0001f670: 2020 2020 206d 6f64 656c 5f6c 6179 6f75       model_layou
+0001f680: 742e 6164 6457 6964 6765 7428 7268 735f  t.addWidget(rhs_
+0001f690: 7769 6467 6574 290a 0a20 2020 2020 2020  widget)..       
+0001f6a0: 2023 2061 6e64 2073 6574 2061 6c69 676e   # and set align
+0001f6b0: 6d65 6e74 206f 6620 7468 6520 6d6f 6465  ment of the mode
+0001f6c0: 6c0a 2020 2020 2020 2020 6d6f 6465 6c5f  l.        model_
+0001f6d0: 6c61 796f 7574 2e73 6574 416c 6967 6e6d  layout.setAlignm
+0001f6e0: 656e 7428 5174 436f 7265 2e51 742e 416c  ent(QtCore.Qt.Al
+0001f6f0: 6967 6e54 6f70 290a 0a20 2020 2020 2020  ignTop)..       
+0001f700: 2072 6574 7572 6e20 6d6f 6465 6c5f 7769   return model_wi
+0001f710: 6467 6574 0a0a 2020 2020 6465 6620 6e6f  dget..    def no
+0001f720: 745f 6966 7928 7365 6c66 2c20 7061 726e  t_ify(self, parn
+0001f730: 616d 653a 2073 7472 293a 0a20 2020 2020  ame: str):.     
+0001f740: 2020 2027 2727 0a20 2020 2020 2020 2053     '''.        S
+0001f750: 7769 7463 6865 7320 6669 7420 6469 6374  witches fit dict
+0001f760: 696f 6e61 7279 2065 6e74 7279 2054 7275  ionary entry Tru
+0001f770: 6520 3c2d 2d3e 2046 616c 7365 0a20 2020  e <--> False.   
+0001f780: 2020 2020 2066 6f72 2074 6865 2070 726f       for the pro
+0001f790: 7669 6465 6420 7061 726e 616d 650a 2020  vided parname.  
+0001f7a0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+0001f7b0: 2020 7365 6c66 2e75 7365 6c2e 6669 745b    self.usel.fit[
+0001f7c0: 7061 726e 616d 655d 203d 206e 6f74 2073  parname] = not s
+0001f7d0: 656c 662e 7573 656c 2e66 6974 5b70 6172  elf.usel.fit[par
+0001f7e0: 6e61 6d65 5d0a 0a20 2020 2064 6566 206d  name]..    def m
+0001f7f0: 616b 655f 7061 7262 6f78 2873 656c 662c  ake_parbox(self,
+0001f800: 2063 623a 2070 6172 7469 616c 2c20 7061   cb: partial, pa
+0001f810: 726e 616d 653a 2073 7472 2c20 5f6e 755f  rname: str, _nu_
+0001f820: 7374 7269 6e67 3a20 7374 722c 0a20 2020  string: str,.   
+0001f830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f840: 2064 6566 6175 6c74 733a 2064 6963 745b   defaults: dict[
+0001f850: 7374 722c 2066 6c6f 6174 5d2c 206f 705f  str, float], op_
+0001f860: 7061 723a 2051 7457 6964 6765 7473 2e51  par: QtWidgets.Q
+0001f870: 5769 6467 6574 2c0a 2020 2020 2020 2020  Widget,.        
+0001f880: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
+0001f890: 6c6e 616d 653a 2073 7472 293a 0a20 2020  lname: str):.   
+0001f8a0: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+0001f8b0: 2043 7265 6174 6573 2073 6574 206f 6620   Creates set of 
+0001f8c0: 7769 6467 6574 7320 666f 7220 6120 7369  widgets for a si
+0001f8d0: 6e67 6c65 2070 6172 616d 6574 6572 206f  ngle parameter o
+0001f8e0: 6620 6120 6d6f 6465 6c2e 5c6e 0a20 2020  f a model.\n.   
+0001f8f0: 2020 2020 2043 6f6e 7461 696e 7320 3220       Contains 2 
+0001f900: 726f 7773 2c20 7570 7065 7220 6973 206c  rows, upper is l
+0001f910: 6162 656c 2061 6e64 2075 6e69 7473 2061  abel and units a
+0001f920: 7320 7374 7269 6e67 2c20 616e 6420 6c6f  s string, and lo
+0001f930: 7765 720a 2020 2020 2020 2020 6973 2073  wer.        is s
+0001f940: 6c69 6465 722c 2074 6578 7465 6e74 7279  lider, textentry
+0001f950: 2028 646f 7562 6c65 7370 696e 626f 7829   (doublespinbox)
+0001f960: 2c20 616e 6420 6669 742f 6669 7820 746f  , and fit/fix to
+0001f970: 6767 6c65 2062 7574 746f 6e2e 0a0a 2020  ggle button...  
+0001f980: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+0001f990: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+0001f9a0: 2d2d 2d0a 2020 2020 2020 2020 6362 3a20  ---.        cb: 
+0001f9b0: 6675 6e63 746f 6f6c 732e 7061 7274 6961  functools.partia
+0001f9c0: 6c0a 2020 2020 2020 2020 2020 2020 5061  l.            Pa
+0001f9d0: 7274 6961 6c2d 6c79 2069 6e73 7461 6e74  rtial-ly instant
+0001f9e0: 6961 7465 6420 6361 6c6c 6261 636b 2077  iated callback w
+0001f9f0: 6869 6368 2077 696c 6c20 6265 2066 6972  hich will be fir
+0001fa00: 6564 2077 6865 6e0a 2020 2020 2020 2020  ed when.        
+0001fa10: 2020 2020 7769 6467 6574 7320 6f66 2074      widgets of t
+0001fa20: 6869 7320 7061 7261 6d65 7465 7220 6172  his parameter ar
+0001fa30: 6520 696e 7465 7261 6374 6564 2077 6974  e interacted wit
+0001fa40: 682e 0a20 2020 2020 2020 2070 6172 6e61  h..        parna
+0001fa50: 6d65 3a20 7374 720a 2020 2020 2020 2020  me: str.        
+0001fa60: 2020 2020 5374 7269 6e67 206e 616d 6520      String name 
+0001fa70: 6f66 2070 6172 616d 6574 6572 2075 7365  of parameter use
+0001fa80: 6420 6173 206b 6579 2069 6e0a 2020 2020  d as key in.    
+0001fa90: 2020 2020 2020 2020 7365 6c66 2e77 6964          self.wid
+0001faa0: 6765 7464 6963 745b 7769 6467 6574 6469  getdict[widgetdi
+0001fab0: 6374 5d0a 2020 2020 2020 2020 5f6e 755f  ct].        _nu_
+0001fac0: 7374 7269 6e67 3a20 7374 720a 2020 2020  string: str.    
+0001fad0: 2020 2020 2020 2020 5374 7269 6e67 206e          String n
+0001fae0: 616d 6520 6f66 2070 6172 616d 6574 6572  ame of parameter
+0001faf0: 2061 6e64 2075 6e69 7473 2075 7365 6420   and units used 
+0001fb00: 6173 2074 6974 6c65 206f 6620 7468 6973  as title of this
+0001fb10: 2070 6172 616d 6574 6572 0a20 2020 2020   parameter.     
+0001fb20: 2020 2064 6566 6175 6c74 733a 2064 6963     defaults: dic
+0001fb30: 745b 7374 722c 2066 6c6f 6174 5d0a 2020  t[str, float].  
+0001fb40: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
+0001fb50: 7420 7661 6c75 6573 206f 6620 7468 6973  t values of this
+0001fb60: 2070 6172 616d 6574 6572 2c20 6b65 7973   parameter, keys
+0001fb70: 2061 7265 206d 696e 2c20 6d61 782c 2076   are min, max, v
+0001fb80: 616c 696e 6974 2c20 7374 6570 0a20 2020  alinit, step.   
+0001fb90: 2020 2020 206f 705f 7061 723a 2051 7457       op_par: QtW
+0001fba0: 6964 6765 7473 2e51 5769 6467 6574 0a20  idgets.QWidget. 
+0001fbb0: 2020 2020 2020 2020 2020 2050 6172 656e             Paren
+0001fbc0: 7420 7769 6467 6574 0a20 2020 2020 2020  t widget.       
+0001fbd0: 206d 6f64 656c 6e61 6d65 3a20 7374 720a   modelname: str.
+0001fbe0: 2020 2020 2020 2020 2020 2020 5374 7269              Stri
+0001fbf0: 6e67 206e 616d 6520 6f66 206d 6f64 656c  ng name of model
+0001fc00: 2075 7365 6420 6173 206b 6579 2069 6e20   used as key in 
+0001fc10: 7365 6c66 2e77 6964 6765 7464 6963 740a  self.widgetdict.
+0001fc20: 2020 2020 2020 2020 2727 270a 0a20 2020          '''..   
+0001fc30: 2020 2020 2023 2057 6964 6765 7420 666f       # Widget fo
+0001fc40: 7220 7468 6973 2070 6172 616d 6574 6572  r this parameter
+0001fc50: 2773 2072 6f77 206f 6620 7769 6467 6574  's row of widget
+0001fc60: 730a 2020 2020 2020 2020 6f6e 655f 7061  s.        one_pa
+0001fc70: 7261 6d5f 7769 6467 6574 203d 2051 7457  ram_widget = QtW
+0001fc80: 6964 6765 7473 2e51 5769 6467 6574 2870  idgets.QWidget(p
+0001fc90: 6172 656e 743d 6f70 5f70 6172 290a 2020  arent=op_par).  
+0001fca0: 2020 2020 2020 6f6e 655f 7061 7261 6d5f        one_param_
+0001fcb0: 6c61 796f 7574 203d 2051 7457 6964 6765  layout = QtWidge
+0001fcc0: 7473 2e51 5642 6f78 4c61 796f 7574 286f  ts.QVBoxLayout(o
+0001fcd0: 6e65 5f70 6172 616d 5f77 6964 6765 7429  ne_param_widget)
+0001fce0: 0a0a 2020 2020 2020 2020 2320 466f 7220  ..        # For 
+0001fcf0: 6c61 6265 6c20 616e 6420 756e 6974 730a  label and units.
+0001fd00: 2020 2020 2020 2020 746f 705f 626f 7877          top_boxw
+0001fd10: 6964 6765 7420 3d20 5174 5769 6467 6574  idget = QtWidget
+0001fd20: 732e 5157 6964 6765 7428 7061 7265 6e74  s.QWidget(parent
+0001fd30: 3d6f 6e65 5f70 6172 616d 5f77 6964 6765  =one_param_widge
+0001fd40: 7429 0a20 2020 2020 2020 2074 6f70 5f62  t).        top_b
+0001fd50: 6f78 6c61 796f 7574 203d 2051 7457 6964  oxlayout = QtWid
+0001fd60: 6765 7473 2e51 4842 6f78 4c61 796f 7574  gets.QHBoxLayout
+0001fd70: 2874 6f70 5f62 6f78 7769 6467 6574 290a  (top_boxwidget).
+0001fd80: 0a20 2020 2020 2020 2023 2046 6f72 2069  .        # For i
+0001fd90: 6e74 6572 6163 7469 7665 2077 6964 6765  nteractive widge
+0001fda0: 7473 0a20 2020 2020 2020 2062 6f74 5f62  ts.        bot_b
+0001fdb0: 6f78 7769 6467 6574 203d 2051 7457 6964  oxwidget = QtWid
+0001fdc0: 6765 7473 2e51 5769 6467 6574 2870 6172  gets.QWidget(par
+0001fdd0: 656e 743d 6f6e 655f 7061 7261 6d5f 7769  ent=one_param_wi
+0001fde0: 6467 6574 290a 2020 2020 2020 2020 626f  dget).        bo
+0001fdf0: 745f 626f 786c 6179 6f75 7420 3d20 5174  t_boxlayout = Qt
+0001fe00: 5769 6467 6574 732e 5148 426f 784c 6179  Widgets.QHBoxLay
+0001fe10: 6f75 7428 626f 745f 626f 7877 6964 6765  out(bot_boxwidge
+0001fe20: 7429 0a0a 2020 2020 2020 2020 2320 4164  t)..        # Ad
+0001fe30: 6420 6c61 6265 6c20 616e 6420 756e 6974  d label and unit
+0001fe40: 730a 2020 2020 2020 2020 6e61 6d65 5f75  s.        name_u
+0001fe50: 6e69 7473 203d 2051 7457 6964 6765 7473  nits = QtWidgets
+0001fe60: 2e51 4c61 6265 6c28 5f6e 755f 7374 7269  .QLabel(_nu_stri
+0001fe70: 6e67 290a 2020 2020 2020 2020 6e61 6d65  ng).        name
+0001fe80: 5f75 6e69 7473 2e73 6574 466f 6e74 2851  _units.setFont(Q
+0001fe90: 7447 7569 2e51 466f 6e74 2827 4172 6961  tGui.QFont('Aria
+0001fea0: 6c27 2c20 3131 2929 0a0a 2020 2020 2020  l', 11))..      
+0001feb0: 2020 6e61 6d65 5f75 6e69 7473 2e73 6574    name_units.set
+0001fec0: 5369 7a65 506f 6c69 6379 280a 2020 2020  SizePolicy(.    
+0001fed0: 2020 2020 2020 2020 5174 5769 6467 6574          QtWidget
+0001fee0: 732e 5153 697a 6550 6f6c 6963 792e 4669  s.QSizePolicy.Fi
+0001fef0: 7865 642c 0a20 2020 2020 2020 2020 2020  xed,.           
+0001ff00: 2051 7457 6964 6765 7473 2e51 5369 7a65   QtWidgets.QSize
+0001ff10: 506f 6c69 6379 2e46 6978 6564 0a20 2020  Policy.Fixed.   
+0001ff20: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+0001ff30: 746f 705f 626f 786c 6179 6f75 742e 6164  top_boxlayout.ad
+0001ff40: 6457 6964 6765 7428 6e61 6d65 5f75 6e69  dWidget(name_uni
+0001ff50: 7473 290a 0a20 2020 2020 2020 2023 2043  ts)..        # C
+0001ff60: 7265 6174 6520 736c 6964 6572 0a20 2020  reate slider.   
+0001ff70: 2020 2020 2073 6c69 6465 7220 3d20 5174       slider = Qt
+0001ff80: 5769 6467 6574 732e 5153 6c69 6465 7228  Widgets.QSlider(
+0001ff90: 0a20 2020 2020 2020 2020 2020 206f 7269  .            ori
+0001ffa0: 656e 7461 7469 6f6e 3d51 7443 6f72 652e  entation=QtCore.
+0001ffb0: 5174 2e48 6f72 697a 6f6e 7461 6c2c 0a20  Qt.Horizontal,. 
+0001ffc0: 2020 2020 2020 2020 2020 2070 6172 656e             paren
+0001ffd0: 743d 626f 745f 626f 7877 6964 6765 740a  t=bot_boxwidget.
+0001ffe0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0001fff0: 2020 2023 2053 6361 6c65 2061 6c6c 2073     # Scale all s
+00020000: 6c69 6465 7220 6e75 6d62 6572 7320 6279  lider numbers by
+00020010: 2074 6869 7320 746f 206d 616b 6520 696e   this to make in
+00020020: 746f 2066 6c6f 6174 730a 2020 2020 2020  to floats.      
+00020030: 2020 736c 6964 6572 5f73 6361 6c65 203d    slider_scale =
+00020040: 2031 4535 0a0a 2020 2020 2020 2020 736c   1E5..        sl
+00020050: 6964 6572 2e73 6574 4d69 6e69 6d75 6d28  ider.setMinimum(
+00020060: 696e 7428 6465 6661 756c 7473 5b27 6d69  int(defaults['mi
+00020070: 6e27 5d20 2a20 736c 6964 6572 5f73 6361  n'] * slider_sca
+00020080: 6c65 2929 0a20 2020 2020 2020 2073 6c69  le)).        sli
+00020090: 6465 722e 7365 744d 6178 696d 756d 2869  der.setMaximum(i
+000200a0: 6e74 2864 6566 6175 6c74 735b 276d 6178  nt(defaults['max
+000200b0: 275d 202a 2073 6c69 6465 725f 7363 616c  '] * slider_scal
+000200c0: 6529 290a 2020 2020 2020 2020 736c 6964  e)).        slid
+000200d0: 6572 2e73 6574 5661 6c75 6528 696e 7428  er.setValue(int(
+000200e0: 6465 6661 756c 7473 5b27 7661 6c69 6e69  defaults['valini
+000200f0: 7427 5d20 2a20 736c 6964 6572 5f73 6361  t'] * slider_sca
+00020100: 6c65 2929 0a20 2020 2020 2020 2073 6c69  le)).        sli
+00020110: 6465 722e 7365 7453 696e 676c 6553 7465  der.setSingleSte
+00020120: 7028 696e 7428 6465 6661 756c 7473 5b27  p(int(defaults['
+00020130: 7374 6570 275d 202a 2073 6c69 6465 725f  step'] * slider_
+00020140: 7363 616c 6529 290a 0a20 2020 2020 2020  scale))..       
+00020150: 2073 656c 662e 7769 6467 6574 6469 6374   self.widgetdict
+00020160: 5b6d 6f64 656c 6e61 6d65 2e6c 6f77 6572  [modelname.lower
+00020170: 2829 5d5b 7061 726e 616d 655d 5b27 736c  ()][parname]['sl
+00020180: 6964 6572 275d 203d 2073 6c69 6465 720a  ider'] = slider.
+00020190: 0a20 2020 2020 2020 2023 2041 6464 2073  .        # Add s
+000201a0: 6c69 6465 7220 746f 206c 6179 6f75 740a  lider to layout.
+000201b0: 2020 2020 2020 2020 626f 745f 626f 786c          bot_boxl
+000201c0: 6179 6f75 742e 6164 6457 6964 6765 7428  ayout.addWidget(
+000201d0: 736c 6964 6572 290a 0a20 2020 2020 2020  slider)..       
+000201e0: 2023 2043 7265 6174 6520 7465 7874 2065   # Create text e
+000201f0: 6e74 7279 2028 446f 7562 6c65 5370 696e  ntry (DoubleSpin
+00020200: 426f 7829 0a20 2020 2020 2020 2065 6e74  Box).        ent
+00020210: 7279 203d 2051 7457 6964 6765 7473 2e51  ry = QtWidgets.Q
+00020220: 446f 7562 6c65 5370 696e 426f 7828 7061  DoubleSpinBox(pa
+00020230: 7265 6e74 3d62 6f74 5f62 6f78 7769 6467  rent=bot_boxwidg
+00020240: 6574 290a 2020 2020 2020 2020 656e 7472  et).        entr
+00020250: 792e 7365 7444 6563 696d 616c 7328 696e  y.setDecimals(in
+00020260: 7428 6465 6661 756c 7473 5b27 6465 6369  t(defaults['deci
+00020270: 6d61 6c73 275d 2929 0a20 2020 2020 2020  mals'])).       
+00020280: 2065 6e74 7279 2e73 6574 4275 7474 6f6e   entry.setButton
+00020290: 5379 6d62 6f6c 7328 5174 5769 6467 6574  Symbols(QtWidget
+000202a0: 732e 5144 6f75 626c 6553 7069 6e42 6f78  s.QDoubleSpinBox
+000202b0: 2e4e 6f42 7574 746f 6e73 290a 2020 2020  .NoButtons).    
+000202c0: 2020 2020 656e 7472 792e 7365 744b 6579      entry.setKey
+000202d0: 626f 6172 6454 7261 636b 696e 6728 4661  boardTracking(Fa
+000202e0: 6c73 6529 0a20 2020 2020 2020 2065 6e74  lse).        ent
+000202f0: 7279 2e73 6574 4d69 6e69 6d75 6d28 6465  ry.setMinimum(de
+00020300: 6661 756c 7473 5b27 6d69 6e27 5d29 0a20  faults['min']). 
+00020310: 2020 2020 2020 2065 6e74 7279 2e73 6574         entry.set
+00020320: 4d61 7869 6d75 6d28 6465 6661 756c 7473  Maximum(defaults
+00020330: 5b27 6d61 7827 5d29 0a20 2020 2020 2020  ['max']).       
+00020340: 2065 6e74 7279 2e73 6574 5661 6c75 6528   entry.setValue(
+00020350: 6465 6661 756c 7473 5b27 7661 6c69 6e69  defaults['valini
+00020360: 7427 5d29 0a20 2020 2020 2020 2065 6e74  t']).        ent
+00020370: 7279 2e73 6574 5369 6e67 6c65 5374 6570  ry.setSingleStep
+00020380: 2864 6566 6175 6c74 735b 2773 7465 7027  (defaults['step'
+00020390: 5d29 0a0a 2020 2020 2020 2020 7365 6c66  ])..        self
+000203a0: 2e77 6964 6765 7464 6963 745b 6d6f 6465  .widgetdict[mode
+000203b0: 6c6e 616d 652e 6c6f 7765 7228 295d 5b70  lname.lower()][p
+000203c0: 6172 6e61 6d65 5d5b 2765 6e74 7279 275d  arname]['entry']
+000203d0: 203d 2065 6e74 7279 0a0a 2020 2020 2020   = entry..      
+000203e0: 2020 2320 4164 6420 646f 7562 6c65 7370    # Add doublesp
+000203f0: 696e 626f 7820 746f 206c 6179 6f75 740a  inbox to layout.
+00020400: 2020 2020 2020 2020 626f 745f 626f 786c          bot_boxl
+00020410: 6179 6f75 742e 6164 6457 6964 6765 7428  ayout.addWidget(
+00020420: 656e 7472 7929 0a0a 2020 2020 2020 2020  entry)..        
+00020430: 2320 4372 6561 7465 2066 6974 2f66 6978  # Create fit/fix
+00020440: 2074 6f67 676c 6520 6275 7474 6f6e 0a20   toggle button. 
+00020450: 2020 2020 2020 2066 665f 746f 6767 6c65         ff_toggle
+00020460: 203d 2051 7457 6964 6765 7473 2e51 5075   = QtWidgets.QPu
+00020470: 7368 4275 7474 6f6e 2827 4672 6565 272c  shButton('Free',
+00020480: 2070 6172 656e 743d 626f 745f 626f 7877   parent=bot_boxw
+00020490: 6964 6765 7429 0a0a 2020 2020 2020 2020  idget)..        
+000204a0: 7365 6c66 2e77 6964 6765 7464 6963 745b  self.widgetdict[
+000204b0: 6d6f 6465 6c6e 616d 652e 6c6f 7765 7228  modelname.lower(
+000204c0: 295d 5b70 6172 6e61 6d65 5d5b 2766 665f  )][parname]['ff_
+000204d0: 746f 6767 6c65 275d 203d 2066 665f 746f  toggle'] = ff_to
+000204e0: 6767 6c65 0a0a 2020 2020 2020 2020 6666  ggle..        ff
+000204f0: 7377 203d 207b 0a20 2020 2020 2020 2020  sw = {.         
+00020500: 2020 2027 4672 6565 273a 2027 4669 7865     'Free': 'Fixe
+00020510: 6427 2c0a 2020 2020 2020 2020 2020 2020  d',.            
+00020520: 2746 6978 6564 273a 2027 4672 6565 272c  'Fixed': 'Free',
+00020530: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
+00020540: 2020 2020 2320 4361 6c6c 6261 636b 2066      # Callback f
+00020550: 6f72 2074 6578 740a 2020 2020 2020 2020  or text.        
+00020560: 6666 5f74 6f67 676c 652e 636c 6963 6b65  ff_toggle.clicke
+00020570: 642e 636f 6e6e 6563 7428 0a20 2020 2020  d.connect(.     
+00020580: 2020 2020 2020 206c 616d 6264 6120 5f3a         lambda _:
+00020590: 2066 665f 746f 6767 6c65 2e73 6574 5465   ff_toggle.setTe
+000205a0: 7874 2866 6673 775b 6666 5f74 6f67 676c  xt(ffsw[ff_toggl
+000205b0: 652e 7465 7874 2829 5d29 0a20 2020 2020  e.text()]).     
+000205c0: 2020 2029 0a0a 2020 2020 2020 2020 2320     )..        # 
+000205d0: 4361 6c6c 6261 636b 2066 6f72 2066 6974  Callback for fit
+000205e0: 2f66 6978 206f 6620 7468 6973 2070 6172  /fix of this par
+000205f0: 616d 6574 6572 0a20 2020 2020 2020 2066  ameter.        f
+00020600: 665f 746f 6767 6c65 2e63 6c69 636b 6564  f_toggle.clicked
+00020610: 2e63 6f6e 6e65 6374 280a 2020 2020 2020  .connect(.      
+00020620: 2020 2020 2020 6c61 6d62 6461 205f 3a20        lambda _: 
+00020630: 7365 6c66 2e6e 6f74 5f69 6679 2870 6172  self.not_ify(par
+00020640: 6e61 6d65 290a 2020 2020 2020 2020 290a  name).        ).
+00020650: 0a20 2020 2020 2020 2023 2043 6f6e 6e65  .        # Conne
+00020660: 6374 2066 6974 2f66 6978 2074 6f20 736c  ct fit/fix to sl
+00020670: 6964 6572 2061 6e64 2074 6578 7465 6e74  ider and textent
+00020680: 7279 0a20 2020 2020 2020 2073 6c69 6465  ry.        slide
+00020690: 722e 7661 6c75 6543 6861 6e67 6564 2e63  r.valueChanged.c
+000206a0: 6f6e 6e65 6374 286c 616d 6264 6120 7661  onnect(lambda va
+000206b0: 6c3a 2063 6228 7661 6c20 2a20 736c 6964  l: cb(val * slid
+000206c0: 6572 5f73 6361 6c65 2a2a 2d31 2929 0a20  er_scale**-1)). 
+000206d0: 2020 2020 2020 2073 6c69 6465 722e 7661         slider.va
+000206e0: 6c75 6543 6861 6e67 6564 2e63 6f6e 6e65  lueChanged.conne
+000206f0: 6374 280a 2020 2020 2020 2020 2020 2020  ct(.            
+00020700: 6c61 6d62 6461 2076 616c 3a20 656e 7472  lambda val: entr
+00020710: 792e 7365 7456 616c 7565 2876 616c 202a  y.setValue(val *
+00020720: 2073 6c69 6465 725f 7363 616c 652a 2a2d   slider_scale**-
+00020730: 3129 0a20 2020 2020 2020 2029 0a20 2020  1).        ).   
+00020740: 2020 2020 2065 6e74 7279 2e76 616c 7565       entry.value
+00020750: 4368 616e 6765 642e 636f 6e6e 6563 7428  Changed.connect(
+00020760: 6362 290a 2020 2020 2020 2020 656e 7472  cb).        entr
+00020770: 792e 7661 6c75 6543 6861 6e67 6564 2e63  y.valueChanged.c
+00020780: 6f6e 6e65 6374 280a 2020 2020 2020 2020  onnect(.        
+00020790: 2020 2020 6c61 6d62 6461 2076 616c 3a20      lambda val: 
+000207a0: 736c 6964 6572 2e73 6574 5661 6c75 6528  slider.setValue(
+000207b0: 696e 7428 7661 6c20 2a20 736c 6964 6572  int(val * slider
+000207c0: 5f73 6361 6c65 2929 0a20 2020 2020 2020  _scale)).       
+000207d0: 2029 0a0a 2020 2020 2020 2020 2320 4164   )..        # Ad
+000207e0: 6420 6669 742f 6669 7820 746f 206c 6179  d fit/fix to lay
+000207f0: 6f75 740a 2020 2020 2020 2020 626f 745f  out.        bot_
+00020800: 626f 786c 6179 6f75 742e 6164 6457 6964  boxlayout.addWid
+00020810: 6765 7428 6666 5f74 6f67 676c 6529 0a0a  get(ff_toggle)..
+00020820: 2020 2020 2020 2020 746f 705f 626f 7877          top_boxw
+00020830: 6964 6765 742e 7365 7453 697a 6550 6f6c  idget.setSizePol
+00020840: 6963 7928 0a20 2020 2020 2020 2020 2020  icy(.           
+00020850: 2051 7457 6964 6765 7473 2e51 5369 7a65   QtWidgets.QSize
+00020860: 506f 6c69 6379 2e46 6978 6564 2c0a 2020  Policy.Fixed,.  
+00020870: 2020 2020 2020 2020 2020 5174 5769 6467            QtWidg
+00020880: 6574 732e 5153 697a 6550 6f6c 6963 792e  ets.QSizePolicy.
+00020890: 4669 7865 640a 2020 2020 2020 2020 290a  Fixed.        ).
+000208a0: 2020 2020 2020 2020 626f 745f 626f 7877          bot_boxw
+000208b0: 6964 6765 742e 7365 7453 697a 6550 6f6c  idget.setSizePol
+000208c0: 6963 7928 0a20 2020 2020 2020 2020 2020  icy(.           
+000208d0: 2051 7457 6964 6765 7473 2e51 5369 7a65   QtWidgets.QSize
+000208e0: 506f 6c69 6379 2e46 6978 6564 2c0a 2020  Policy.Fixed,.  
+000208f0: 2020 2020 2020 2020 2020 5174 5769 6467            QtWidg
+00020900: 6574 732e 5153 697a 6550 6f6c 6963 792e  ets.QSizePolicy.
+00020910: 4669 7865 640a 2020 2020 2020 2020 290a  Fixed.        ).
+00020920: 2020 2020 2020 2020 746f 705f 626f 786c          top_boxl
+00020930: 6179 6f75 742e 7365 7441 6c69 676e 6d65  ayout.setAlignme
+00020940: 6e74 2851 7443 6f72 652e 5174 2e41 6c69  nt(QtCore.Qt.Ali
+00020950: 676e 4843 656e 7465 7229 0a0a 2020 2020  gnHCenter)..    
+00020960: 2020 2020 6f6e 655f 7061 7261 6d5f 6c61      one_param_la
+00020970: 796f 7574 2e61 6464 5769 6467 6574 2874  yout.addWidget(t
+00020980: 6f70 5f62 6f78 7769 6467 6574 290a 2020  op_boxwidget).  
+00020990: 2020 2020 2020 6f6e 655f 7061 7261 6d5f        one_param_
+000209a0: 6c61 796f 7574 2e61 6464 5769 6467 6574  layout.addWidget
+000209b0: 2862 6f74 5f62 6f78 7769 6467 6574 290a  (bot_boxwidget).
+000209c0: 0a20 2020 2020 2020 206f 6e65 5f70 6172  .        one_par
+000209d0: 616d 5f6c 6179 6f75 742e 7365 7443 6f6e  am_layout.setCon
+000209e0: 7465 6e74 734d 6172 6769 6e73 2830 2c20  tentsMargins(0, 
+000209f0: 302c 2030 2c20 3029 0a20 2020 2020 2020  0, 0, 0).       
+00020a00: 206f 6e65 5f70 6172 616d 5f6c 6179 6f75   one_param_layou
+00020a10: 742e 7365 7453 7061 6369 6e67 2832 290a  t.setSpacing(2).
+00020a20: 2020 2020 2020 2020 6f6e 655f 7061 7261          one_para
+00020a30: 6d5f 6c61 796f 7574 2e61 6464 5374 7265  m_layout.addStre
+00020a40: 7463 6828 3129 0a20 2020 2020 2020 206f  tch(1).        o
+00020a50: 6e65 5f70 6172 616d 5f6c 6179 6f75 742e  ne_param_layout.
+00020a60: 7365 7441 6c69 676e 6d65 6e74 2851 7443  setAlignment(QtC
+00020a70: 6f72 652e 5174 2e41 6c69 676e 5643 656e  ore.Qt.AlignVCen
+00020a80: 7465 7229 0a0a 2020 2020 2020 2020 7265  ter)..        re
+00020a90: 7475 726e 206f 6e65 5f70 6172 616d 5f77  turn one_param_w
+00020aa0: 6964 6765 742c 206f 6e65 5f70 6172 616d  idget, one_param
+00020ab0: 5f6c 6179 6f75 740a 0a0a 6465 6620 696e  _layout...def in
+00020ac0: 7465 7261 6374 6976 655f 6669 7474 696e  teractive_fittin
+00020ad0: 6728 6461 7461 7365 743a 2054 6175 5444  g(dataset: TauTD
+00020ae0: 6174 6173 6574 207c 2054 6175 4844 6174  ataset | TauHDat
+00020af0: 6173 6574 2c20 6170 702c 0a20 2020 2020  aset, app,.     
+00020b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020b10: 2020 206d 6f64 656c 5f6f 7074 3a20 7374     model_opt: st
+00020b20: 7220 7c20 6c69 7374 5b4c 6f67 5461 7554  r | list[LogTauT
+00020b30: 4d6f 6465 6c20 7c20 4c6f 6754 6175 484d  Model | LogTauHM
+00020b40: 6f64 656c 5d20 3d20 2766 726f 6d5f 6461  odel] = 'from_da
+00020b50: 7461 7365 7427 2920 2d3e 2074 7570 6c65  taset') -> tuple
+00020b60: 5b6c 6973 745b 4c6f 6754 6175 544d 6f64  [list[LogTauTMod
+00020b70: 656c 207c 204c 6f67 5461 7548 4d6f 6465  el | LogTauHMode
+00020b80: 6c5d 2c20 6c69 7374 5b64 6963 745b 7374  l], list[dict[st
+00020b90: 722c 2066 6c6f 6174 5d5d 2c20 6c69 7374  r, float]], list
+00020ba0: 5b64 6963 745b 7374 722c 2066 6c6f 6174  [dict[str, float
+00020bb0: 5d5d 2c20 626f 6f6c 5d3a 2023 206e 6f71  ]], bool]: # noq
+00020bc0: 610a 2020 2020 2727 270a 2020 2020 4372  a.    '''.    Cr
+00020bd0: 6561 7465 7320 7174 2077 696e 646f 7720  eates qt window 
+00020be0: 666f 7220 7573 6572 2074 6f20 696e 7465  for user to inte
+00020bf0: 7261 6374 6976 656c 7920 6669 7420 6d6f  ractively fit mo
+00020c00: 6465 6c73 2074 6f20 7265 6c61 7861 7469  dels to relaxati
+00020c10: 6f6e 0a20 2020 2064 6174 610a 0a20 2020  on.    data..   
+00020c20: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00020c30: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064  ----------.    d
+00020c40: 6174 6173 6574 3a20 5461 7554 4461 7461  ataset: TauTData
+00020c50: 7365 7420 7c20 5461 7548 4461 7461 7365  set | TauHDatase
+00020c60: 740a 2020 2020 2020 2020 4461 7461 7365  t.        Datase
+00020c70: 7420 746f 2070 6c6f 740a 2020 2020 6170  t to plot.    ap
+00020c80: 703a 2051 7457 6964 6765 7473 2e51 4170  p: QtWidgets.QAp
+00020c90: 706c 6963 6174 696f 6e0a 2020 2020 2020  plication.      
+00020ca0: 2020 4170 706c 6963 6174 696f 6e20 7573    Application us
+00020cb0: 6564 2062 7920 6375 7272 656e 7420 7072  ed by current pr
+00020cc0: 6f67 7261 6d0a 2020 2020 2020 2020 4372  ogram.        Cr
+00020cd0: 6561 7465 2077 6974 6820 6061 7070 3d51  eate with `app=Q
+00020ce0: 7457 6964 6765 7473 2e51 4170 706c 6963  tWidgets.QApplic
+00020cf0: 6174 696f 6e28 5b5d 2960 0a20 2020 206d  ation([])`.    m
+00020d00: 6f64 656c 5f6f 7074 3a20 7374 7220 7c20  odel_opt: str | 
+00020d10: 6c69 7374 5b4c 6f67 5461 7554 4d6f 6465  list[LogTauTMode
+00020d20: 6c20 7c20 4c6f 6754 6175 484d 6f64 656c  l | LogTauHModel
+00020d30: 5d20 6465 6661 756c 7420 2766 726f 6d5f  ] default 'from_
+00020d40: 6461 7461 7365 7427 200a 2020 2020 2020  dataset' .      
+00020d50: 2020 4c69 7374 206f 6620 6d6f 6465 6c73    List of models
+00020d60: 2074 6f20 6f66 6665 7220 746f 2075 7365   to offer to use
+00020d70: 722c 2069 6620 2766 726f 6d5f 6461 7461  r, if 'from_data
+00020d80: 7365 7427 2077 696c 6c20 6765 6e65 7261  set' will genera
+00020d90: 7465 0a20 2020 2020 2020 2061 206c 6973  te.        a lis
+00020da0: 7420 6261 7365 6420 6f6e 2074 6865 2064  t based on the d
+00020db0: 6174 6173 6574 2070 726f 7669 6465 640a  ataset provided.
+00020dc0: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
+00020dd0: 202d 2d2d 2d2d 2d2d 0a20 2020 206c 6973   -------.    lis
+00020de0: 745b 4c6f 6754 6175 544d 6f64 656c 207c  t[LogTauTModel |
+00020df0: 204c 6f67 5461 7548 4d6f 6465 6c5d 0a20   LogTauHModel]. 
+00020e00: 2020 2020 2020 204d 6f64 656c 7320 7365         Models se
+00020e10: 6c65 6374 6564 2062 7920 7573 6572 0a20  lected by user. 
+00020e20: 2020 206c 6973 745b 6469 6374 5b73 7472     list[dict[str
+00020e30: 2c20 666c 6f61 745d 5d0a 2020 2020 2020  , float]].      
+00020e40: 2020 6669 745f 7661 7273 2064 6963 7473    fit_vars dicts
+00020e50: 2c20 6f6e 6520 7065 7220 6d6f 6465 6c0a  , one per model.
+00020e60: 2020 2020 6c69 7374 5b64 6963 745b 7374      list[dict[st
+00020e70: 722c 2066 6c6f 6174 5d5d 0a20 2020 2020  r, float]].     
+00020e80: 2020 2066 6978 5f76 6172 7320 6469 6374     fix_vars dict
+00020e90: 732c 206f 6e65 2070 6572 206d 6f64 656c  s, one per model
+00020ea0: 0a20 2020 2062 6f6f 6c0a 2020 2020 2020  .    bool.      
+00020eb0: 2020 5472 7565 2069 6620 7573 6572 2068    True if user h
+00020ec0: 6173 2065 7869 7465 6420 7769 6e64 6f77  as exited window
+00020ed0: 2069 6e73 7465 6164 206f 6620 6669 7474   instead of fitt
+00020ee0: 696e 670a 2020 2020 2020 2020 656c 7365  ing.        else
+00020ef0: 2046 616c 7365 0a20 2020 2027 2727 2023   False.    ''' #
+00020f00: 206e 6f71 610a 0a20 2020 2069 6620 6d6f   noqa..    if mo
+00020f10: 6465 6c5f 6f70 7420 3d3d 2027 6672 6f6d  del_opt == 'from
+00020f20: 5f64 6174 6173 6574 273a 0a20 2020 2020  _dataset':.     
+00020f30: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00020f40: 2864 6174 6173 6574 2c20 5461 7554 4461  (dataset, TauTDa
+00020f50: 7461 7365 7429 3a0a 2020 2020 2020 2020  taset):.        
+00020f60: 2020 2020 6d6f 6465 6c5f 6f70 7420 3d20      model_opt = 
+00020f70: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+00020f80: 2020 4c6f 674f 7262 6163 684d 6f64 656c    LogOrbachModel
+00020f90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00020fa0: 2020 4c6f 6752 616d 616e 4d6f 6465 6c2c    LogRamanModel,
+00020fb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020fc0: 204c 6f67 5154 4d4d 6f64 656c 2c0a 2020   LogQTMModel,.  
+00020fd0: 2020 2020 2020 2020 2020 2020 2020 4c6f                Lo
+00020fe0: 6744 6972 6563 744d 6f64 656c 0a20 2020  gDirectModel.   
+00020ff0: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
+00021000: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
+00021010: 6365 2864 6174 6173 6574 2c20 5461 7548  ce(dataset, TauH
+00021020: 4461 7461 7365 7429 3a0a 2020 2020 2020  Dataset):.      
+00021030: 2020 2020 2020 6d6f 6465 6c5f 6f70 7420        model_opt 
+00021040: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
+00021050: 2020 2020 4c6f 6746 4451 544d 4d6f 6465      LogFDQTMMode
+00021060: 6c2c 0a20 2020 2020 2020 2020 2020 2020  l,.             
+00021070: 2020 204c 6f67 5261 6d61 6e49 494d 6f64     LogRamanIIMod
+00021080: 656c 2c0a 2020 2020 2020 2020 2020 2020  el,.            
+00021090: 2020 2020 4c6f 6742 5656 5261 6d61 6e49      LogBVVRamanI
+000210a0: 494d 6f64 656c 2c0a 2020 2020 2020 2020  IModel,.        
+000210b0: 2020 2020 2020 2020 4c6f 6743 6f6e 7374          LogConst
+000210c0: 616e 744d 6f64 656c 2c0a 2020 2020 2020  antModel,.      
+000210d0: 2020 2020 2020 2020 2020 4c6f 6742 5656            LogBVV
+000210e0: 436f 6e73 7461 6e74 4d6f 6465 6c2c 0a20  ConstantModel,. 
+000210f0: 2020 2020 2020 2020 2020 205d 0a0a 2020             ]..  
+00021100: 2020 7573 656c 203d 2074 7970 6528 276f    usel = type('o
+00021110: 626a 272c 2028 6f62 6a65 6374 2c29 2c20  bj', (object,), 
+00021120: 7b0a 2020 2020 2020 2020 276d 6f64 656c  {.        'model
+00021130: 7327 3a20 7b0a 2020 2020 2020 2020 2020  s': {.          
+00021140: 2020 6d6f 6465 6c2e 4e41 4d45 2e6c 6f77    model.NAME.low
+00021150: 6572 2829 3a20 4661 6c73 650a 2020 2020  er(): False.    
+00021160: 2020 2020 2020 2020 666f 7220 6d6f 6465          for mode
+00021170: 6c20 696e 206d 6f64 656c 5f6f 7074 0a20  l in model_opt. 
+00021180: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00021190: 2020 2766 6974 5f76 6172 7327 3a20 5b5d    'fit_vars': []
+000211a0: 2c0a 2020 2020 2020 2020 2766 6978 5f76  ,.        'fix_v
+000211b0: 6172 7327 3a20 5b5d 2c0a 2020 2020 2020  ars': [],.      
+000211c0: 2020 2766 6978 273a 205b 5d2c 0a20 2020    'fix': [],.   
+000211d0: 2020 2020 2027 6578 6974 6564 273a 2054       'exited': T
+000211e0: 7275 650a 2020 2020 7d29 0a0a 2020 2020  rue.    })..    
+000211f0: 7061 7261 6d5f 7769 6e64 6f77 203d 2046  param_window = F
+00021200: 6974 5769 6e64 6f77 280a 2020 2020 2020  itWindow(.      
+00021210: 2020 6461 7461 7365 742c 0a20 2020 2020    dataset,.     
+00021220: 2020 2075 7365 6c2c 0a20 2020 2020 2020     usel,.       
+00021230: 206d 6f64 656c 5f6f 7074 2c0a 2020 2020   model_opt,.    
+00021240: 2020 2020 6775 692e 7769 6467 6574 5f64      gui.widget_d
+00021250: 6566 6175 6c74 730a 2020 2020 290a 2020  efaults.    ).  
+00021260: 2020 7061 7261 6d5f 7769 6e64 6f77 2e73    param_window.s
+00021270: 686f 7728 290a 0a20 2020 2061 7070 2e65  how()..    app.e
+00021280: 7865 6328 290a 0a20 2020 206e 616d 655f  xec()..    name_
+00021290: 746f 5f6d 6f64 656c 203d 207b 0a20 2020  to_model = {.   
+000212a0: 2020 2020 206d 6f64 656c 2e4e 414d 452e       model.NAME.
+000212b0: 6c6f 7765 7228 293a 206d 6f64 656c 0a20  lower(): model. 
+000212c0: 2020 2020 2020 2066 6f72 206d 6f64 656c         for model
+000212d0: 2069 6e20 6d6f 6465 6c5f 6f70 740a 2020   in model_opt.  
+000212e0: 2020 7d0a 0a20 2020 2072 5f6d 6f64 656c    }..    r_model
+000212f0: 7320 3d20 5b0a 2020 2020 2020 2020 6e61  s = [.        na
+00021300: 6d65 5f74 6f5f 6d6f 6465 6c5b 6e61 6d65  me_to_model[name
+00021310: 5d0a 2020 2020 2020 2020 666f 7220 6e61  ].        for na
+00021320: 6d65 2069 6e20 7573 656c 2e6d 6f64 656c  me in usel.model
+00021330: 730a 2020 2020 5d0a 0a20 2020 2072 6574  s.    ]..    ret
+00021340: 7572 6e20 725f 6d6f 6465 6c73 2c20 7573  urn r_models, us
+00021350: 656c 2e66 6974 5f76 6172 732c 2075 7365  el.fit_vars, use
+00021360: 6c2e 6669 785f 7661 7273 2c20 7573 656c  l.fix_vars, usel
+00021370: 2e65 7869 7465 640a 0a0a 6465 6620 706c  .exited...def pl
+00021380: 6f74 5f66 6974 7465 645f 7469 6d65 7328  ot_fitted_times(
+00021390: 6461 7461 7365 743a 2054 6175 5444 6174  dataset: TauTDat
+000213a0: 6173 6574 207c 2054 6175 4844 6174 6173  aset | TauHDatas
+000213b0: 6574 2c0a 2020 2020 2020 2020 2020 2020  et,.            
+000213c0: 2020 2020 2020 2020 2020 6d6f 6465 6c3a            model:
+000213d0: 204c 6f67 5461 7554 4d6f 6465 6c20 7c20   LogTauTModel | 
+000213e0: 4d75 6c74 694c 6f67 5461 7554 4d6f 6465  MultiLogTauTMode
+000213f0: 6c20 7c20 4c6f 6754 6175 484d 6f64 656c  l | LogTauHModel
+00021400: 207c 204d 756c 7469 4c6f 6754 6175 484d   | MultiLogTauHM
+00021410: 6f64 656c 2c20 2320 6e6f 7161 0a20 2020  odel, # noqa.   
+00021420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021430: 2020 2073 686f 773a 2062 6f6f 6c20 3d20     show: bool = 
+00021440: 5472 7565 2c20 7361 7665 3a20 626f 6f6c  True, save: bool
+00021450: 203d 2046 616c 7365 2c0a 2020 2020 2020   = False,.      
+00021460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021470: 7361 7665 5f6e 616d 653a 2073 7472 203d  save_name: str =
+00021480: 2027 6669 7474 6564 5f72 6174 6573 2e70   'fitted_rates.p
+00021490: 6e67 272c 0a20 2020 2020 2020 2020 2020  ng',.           
+000214a0: 2020 2020 2020 2020 2020 2076 6572 626f             verbo
+000214b0: 7365 3a20 626f 6f6c 203d 2054 7275 652c  se: bool = True,
+000214c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000214d0: 2020 2020 2020 2073 686f 775f 7061 7261         show_para
+000214e0: 6d73 3a20 626f 6f6c 203d 2054 7275 6529  ms: bool = True)
+000214f0: 202d 3e20 7475 706c 655b 706c 742e 4669   -> tuple[plt.Fi
+00021500: 6775 7265 2c20 706c 742e 4178 6573 5d3a  gure, plt.Axes]:
+00021510: 0a20 2020 2027 2727 0a20 2020 2050 6c6f  .    '''.    Plo
+00021520: 7473 2065 7870 6572 696d 656e 7461 6c20  ts experimental 
+00021530: 616e 6420 6669 7474 6564 2028 6d6f 6465  and fitted (mode
+00021540: 6c29 2072 656c 6178 6174 696f 6e20 7261  l) relaxation ra
+00021550: 7465 2061 735c 6e0a 2020 2020 6c6e 2874  te as\n.    ln(t
+00021560: 6175 2920 7673 2031 2f78 7661 7220 7768  au) vs 1/xvar wh
+00021570: 6572 6520 7876 6172 2069 7320 5420 6f72  ere xvar is T or
+00021580: 2048 2e0a 0a20 2020 2050 6172 616d 6574   H...    Paramet
+00021590: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
+000215a0: 2d2d 0a20 2020 2064 6174 6173 6574 3a20  --.    dataset: 
+000215b0: 5461 7554 4461 7461 7365 7420 7c20 5461  TauTDataset | Ta
+000215c0: 7548 4461 7461 7365 740a 2020 2020 2020  uHDataset.      
+000215d0: 2020 4461 7461 7365 7420 746f 2070 6c6f    Dataset to plo
+000215e0: 740a 2020 2020 6d6f 6465 6c3a 204c 6f67  t.    model: Log
+000215f0: 5461 7554 4d6f 6465 6c20 7c20 4d75 6c74  TauTModel | Mult
+00021600: 694c 6f67 5461 7554 4d6f 6465 6c20 7c20  iLogTauTModel | 
+00021610: 4c6f 6754 6175 484d 6f64 656c 207c 204d  LogTauHModel | M
+00021620: 756c 7469 4c6f 6754 6175 484d 6f64 656c  ultiLogTauHModel
+00021630: 0a20 2020 2020 2020 204d 6f64 656c 2028  .        Model (
+00021640: 6669 7474 6564 2920 746f 2070 6c6f 740a  fitted) to plot.
+00021650: 2020 2020 7368 6f77 3a20 626f 6f6c 2c20      show: bool, 
+00021660: 6465 6661 756c 7420 5472 7565 0a20 2020  default True.   
+00021670: 2020 2020 2049 6620 5472 7565 2c20 7368       If True, sh
+00021680: 6f77 2070 6c6f 7420 6f6e 2073 6372 6565  ow plot on scree
+00021690: 6e0a 2020 2020 7361 7665 3a20 626f 6f6c  n.    save: bool
+000216a0: 2c20 6465 6661 756c 7420 4661 6c73 650a  , default False.
+000216b0: 2020 2020 2020 2020 4966 2054 7275 652c          If True,
+000216c0: 2073 6176 6520 706c 6f74 2074 6f20 6669   save plot to fi
+000216d0: 6c65 2060 7361 7665 5f6e 616d 6560 0a20  le `save_name`. 
+000216e0: 2020 2073 6176 655f 6e61 6d65 3a20 7374     save_name: st
+000216f0: 722c 2064 6566 6175 6c74 203d 2027 6669  r, default = 'fi
+00021700: 7474 6564 5f72 6174 6573 2e70 6e67 270a  tted_rates.png'.
+00021710: 2020 2020 2020 2020 4966 2073 6176 6520          If save 
+00021720: 6973 2054 7275 652c 2077 696c 6c20 7361  is True, will sa
+00021730: 7665 2070 6c6f 7420 746f 2074 6869 7320  ve plot to this 
+00021740: 6669 6c65 6e61 6d65 0a20 2020 2076 6572  filename.    ver
+00021750: 626f 7365 3a20 626f 6f6c 2c20 6465 6661  bose: bool, defa
+00021760: 756c 7420 5472 7565 0a20 2020 2020 2020  ult True.       
+00021770: 2049 6620 5472 7565 2c20 706c 6f74 2066   If True, plot f
+00021780: 696c 6520 6c6f 6361 7469 6f6e 2069 7320  ile location is 
+00021790: 7772 6974 7465 6e20 746f 2074 6572 6d69  written to termi
+000217a0: 6e61 6c0a 2020 2020 7368 6f77 5f70 6172  nal.    show_par
+000217b0: 616d 733a 2062 6f6f 6c2c 2064 6566 6175  ams: bool, defau
+000217c0: 6c74 2054 7275 650a 2020 2020 2020 2020  lt True.        
+000217d0: 4966 2054 7275 652c 2073 686f 7773 2066  If True, shows f
+000217e0: 6974 7465 6420 7061 7261 6d65 7465 7273  itted parameters
+000217f0: 206f 6e20 706c 6f74 0a0a 2020 2020 5265   on plot..    Re
+00021800: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
+00021810: 2d0a 2020 2020 706c 742e 4669 6775 7265  -.    plt.Figure
+00021820: 0a20 2020 2020 2020 204d 6174 706c 6f74  .        Matplot
+00021830: 6c69 6220 6669 6775 7265 206f 626a 6563  lib figure objec
+00021840: 740a 2020 2020 706c 742e 4178 6573 0a20  t.    plt.Axes. 
+00021850: 2020 2020 2020 204d 6174 706c 6f74 6c69         Matplotli
+00021860: 6220 6178 6973 206f 626a 6563 740a 2020  b axis object.  
+00021870: 2020 2727 270a 0a20 2020 2069 6620 7368    '''..    if sh
+00021880: 6f77 5f70 6172 616d 733a 0a20 2020 2020  ow_params:.     
+00021890: 2020 2066 6967 7369 7a65 203d 2028 362c     figsize = (6,
+000218a0: 2036 290a 2020 2020 656c 7365 3a0a 2020   6).    else:.  
+000218b0: 2020 2020 2020 6669 6773 697a 6520 3d20        figsize = 
+000218c0: 2836 2c20 352e 3529 0a0a 2020 2020 2320  (6, 5.5)..    # 
+000218d0: 4372 6561 7465 2066 6967 7572 6520 616e  Create figure an
+000218e0: 6420 6178 6573 0a20 2020 2066 6967 2c20  d axes.    fig, 
+000218f0: 6178 203d 2070 6c74 2e73 7562 706c 6f74  ax = plt.subplot
+00021900: 7328 0a20 2020 2020 2020 2031 2c0a 2020  s(.        1,.  
+00021910: 2020 2020 2020 312c 0a20 2020 2020 2020        1,.       
+00021920: 2073 6861 7265 783d 5472 7565 2c0a 2020   sharex=True,.  
+00021930: 2020 2020 2020 7368 6172 6579 3d54 7275        sharey=Tru
+00021940: 652c 0a20 2020 2020 2020 2066 6967 7369  e,.        figsi
+00021950: 7a65 3d66 6967 7369 7a65 2c0a 2020 2020  ze=figsize,.    
+00021960: 2020 2020 6e75 6d3d 2746 6974 7465 6420      num='Fitted 
+00021970: 7265 6c61 7861 7469 6f6e 2070 726f 6669  relaxation profi
+00021980: 6c65 270a 2020 2020 290a 0a20 2020 205f  le'.    )..    _
+00021990: 706c 6f74 5f66 6974 7465 645f 7469 6d65  plot_fitted_time
+000219a0: 7328 6461 7461 7365 742c 206d 6f64 656c  s(dataset, model
+000219b0: 2c20 6669 672c 2061 782c 2073 686f 775f  , fig, ax, show_
+000219c0: 7061 7261 6d73 3d73 686f 775f 7061 7261  params=show_para
+000219d0: 6d73 290a 0a20 2020 2066 6967 2e74 6967  ms)..    fig.tig
+000219e0: 6874 5f6c 6179 6f75 7428 290a 0a20 2020  ht_layout()..   
+000219f0: 2069 6620 7368 6f77 3a0a 2020 2020 2020   if show:.      
+00021a00: 2020 706c 742e 7368 6f77 2829 0a0a 2020    plt.show()..  
+00021a10: 2020 6966 2073 6176 653a 0a20 2020 2020    if save:.     
+00021a20: 2020 2066 6967 2e73 6176 6566 6967 2873     fig.savefig(s
+00021a30: 6176 655f 6e61 6d65 2c20 6470 693d 3530  ave_name, dpi=50
+00021a40: 3029 0a20 2020 2020 2020 2069 6620 7665  0).        if ve
+00021a50: 7262 6f73 653a 0a20 2020 2020 2020 2020  rbose:.         
+00021a60: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00021a70: 2864 6174 6173 6574 2c20 2854 6175 5444  (dataset, (TauTD
+00021a80: 6174 6173 6574 2929 3a0a 2020 2020 2020  ataset)):.      
+00021a90: 2020 2020 2020 2020 2020 5f78 7661 7220            _xvar 
+00021aa0: 3d20 2754 270a 2020 2020 2020 2020 2020  = 'T'.          
+00021ab0: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
+00021ac0: 6528 6461 7461 7365 742c 2028 5461 7548  e(dataset, (TauH
+00021ad0: 4461 7461 7365 7429 293a 0a20 2020 2020  Dataset)):.     
+00021ae0: 2020 2020 2020 2020 2020 205f 7876 6172             _xvar
+00021af0: 203d 2027 4827 0a20 2020 2020 2020 2020   = 'H'.         
+00021b00: 2020 2075 742e 6370 7269 6e74 280a 2020     ut.cprint(.  
+00021b10: 2020 2020 2020 2020 2020 2020 2020 6627                f'
+00021b20: 5c6e 2046 6974 7465 6420 6c6e 28cf 8429  \n Fitted ln(..)
+00021b30: 2076 7320 312f 7b5f 7876 6172 7d20 706c   vs 1/{_xvar} pl
+00021b40: 6f74 2073 6176 6564 2074 6f20 5c6e 207b  ot saved to \n {
+00021b50: 7361 7665 5f6e 616d 657d 5c6e 272c 2023  save_name}\n', #
+00021b60: 206e 6f71 610a 2020 2020 2020 2020 2020   noqa.          
+00021b70: 2020 2020 2020 2763 7961 6e27 0a20 2020        'cyan'.   
+00021b80: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+00021b90: 7265 7475 726e 2066 6967 2c20 6178 0a0a  return fig, ax..
+00021ba0: 0a64 6566 2070 6c6f 745f 7469 6d65 7328  .def plot_times(
+00021bb0: 6461 7461 7365 743a 2054 6175 5444 6174  dataset: TauTDat
+00021bc0: 6173 6574 207c 2054 6175 4844 6174 6173  aset | TauHDatas
+00021bd0: 6574 2c20 7368 6f77 3a20 626f 6f6c 203d  et, show: bool =
+00021be0: 2054 7275 652c 0a20 2020 2020 2020 2020   True,.         
+00021bf0: 2020 2020 2020 7361 7665 3a20 626f 6f6c        save: bool
+00021c00: 203d 2046 616c 7365 2c20 7361 7665 5f6e   = False, save_n
+00021c10: 616d 653a 2073 7472 203d 2027 7265 6c61  ame: str = 'rela
+00021c20: 7861 7469 6f6e 5f74 696d 6573 2e70 6e67  xation_times.png
+00021c30: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00021c40: 2020 7665 7262 6f73 653a 2062 6f6f 6c20    verbose: bool 
+00021c50: 3d20 5472 7565 2920 2d3e 2074 7570 6c65  = True) -> tuple
+00021c60: 5b70 6c74 2e46 6967 7572 652c 2070 6c74  [plt.Figure, plt
+00021c70: 2e41 7865 735d 3a0a 2020 2020 2727 270a  .Axes]:.    '''.
+00021c80: 2020 2020 506c 6f74 7320 6578 7065 7269      Plots experi
+00021c90: 6d65 6e74 616c 2072 656c 6178 6174 696f  mental relaxatio
+00021ca0: 6e20 7469 6d65 2061 735c 6e0a 2020 2020  n time as\n.    
+00021cb0: 6c6e 2874 6175 2920 7673 2031 2f78 7661  ln(tau) vs 1/xva
+00021cc0: 7220 7768 6572 6520 7876 6172 2069 7320  r where xvar is 
+00021cd0: 5420 6f72 2048 2e0a 0a20 2020 2050 6172  T or H...    Par
+00021ce0: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
+00021cf0: 2d2d 2d2d 2d2d 0a20 2020 2064 6174 6173  ------.    datas
+00021d00: 6574 3a20 5461 7554 4461 7461 7365 7420  et: TauTDataset 
+00021d10: 7c20 5461 7548 4461 7461 7365 740a 2020  | TauHDataset.  
+00021d20: 2020 2020 2020 4461 7461 7365 7420 746f        Dataset to
+00021d30: 2070 6c6f 740a 2020 2020 7368 6f77 3a20   plot.    show: 
+00021d40: 626f 6f6c 2c20 6465 6661 756c 7420 5472  bool, default Tr
+00021d50: 7565 0a20 2020 2020 2020 2049 6620 5472  ue.        If Tr
+00021d60: 7565 2c20 7368 6f77 2070 6c6f 7420 6f6e  ue, show plot on
+00021d70: 2073 6372 6565 6e0a 2020 2020 7361 7665   screen.    save
+00021d80: 3a20 626f 6f6c 2c20 6465 6661 756c 7420  : bool, default 
+00021d90: 4661 6c73 650a 2020 2020 2020 2020 4966  False.        If
+00021da0: 2054 7275 652c 2073 6176 6520 706c 6f74   True, save plot
+00021db0: 2074 6f20 6669 6c65 2060 7361 7665 5f6e   to file `save_n
+00021dc0: 616d 6560 0a20 2020 2073 6176 655f 6e61  ame`.    save_na
+00021dd0: 6d65 3a20 7374 722c 2064 6566 6175 6c74  me: str, default
+00021de0: 2027 7265 6c61 7861 7469 6f6e 5f74 696d   'relaxation_tim
+00021df0: 6573 2e70 6e67 270a 2020 2020 2020 2020  es.png'.        
+00021e00: 4966 2073 6176 6520 6973 2054 7275 652c  If save is True,
+00021e10: 2077 696c 6c20 7361 7665 2070 6c6f 7420   will save plot 
+00021e20: 746f 2074 6869 7320 6669 6c65 6e61 6d65  to this filename
+00021e30: 0a20 2020 2076 6572 626f 7365 3a20 626f  .    verbose: bo
+00021e40: 6f6c 2c20 6465 6661 756c 7420 5472 7565  ol, default True
+00021e50: 0a20 2020 2020 2020 2049 6620 5472 7565  .        If True
+00021e60: 2c20 706c 6f74 2066 696c 6520 6c6f 6361  , plot file loca
+00021e70: 7469 6f6e 2069 7320 7772 6974 7465 6e20  tion is written 
+00021e80: 746f 2074 6572 6d69 6e61 6c0a 0a20 2020  to terminal..   
+00021e90: 2052 6574 7572 6e73 0a20 2020 202d 2d2d   Returns.    ---
+00021ea0: 2d2d 2d2d 0a20 2020 2070 6c74 2e46 6967  ----.    plt.Fig
+00021eb0: 7572 650a 2020 2020 2020 2020 4d61 7470  ure.        Matp
+00021ec0: 6c6f 746c 6962 2066 6967 7572 6520 6f62  lotlib figure ob
+00021ed0: 6a65 6374 0a20 2020 2070 6c74 2e41 7865  ject.    plt.Axe
+00021ee0: 730a 2020 2020 2020 2020 4d61 7470 6c6f  s.        Matplo
+00021ef0: 746c 6962 2061 7869 7320 6f62 6a65 6374  tlib axis object
+00021f00: 0a20 2020 2027 2727 0a0a 2020 2020 2320  .    '''..    # 
+00021f10: 4372 6561 7465 2066 6967 7572 6520 616e  Create figure an
+00021f20: 6420 6178 6573 0a20 2020 2066 6967 2c20  d axes.    fig, 
+00021f30: 6178 203d 2070 6c74 2e73 7562 706c 6f74  ax = plt.subplot
+00021f40: 7328 0a20 2020 2020 2020 2031 2c0a 2020  s(.        1,.  
+00021f50: 2020 2020 2020 312c 0a20 2020 2020 2020        1,.       
+00021f60: 2073 6861 7265 783d 5472 7565 2c0a 2020   sharex=True,.  
+00021f70: 2020 2020 2020 7368 6172 6579 3d54 7275        sharey=Tru
+00021f80: 652c 0a20 2020 2020 2020 2066 6967 7369  e,.        figsi
+00021f90: 7a65 3d28 362c 2035 2e35 292c 0a20 2020  ze=(6, 5.5),.   
+00021fa0: 2020 2020 206e 756d 3d27 4669 7474 6564       num='Fitted
+00021fb0: 2072 656c 6178 6174 696f 6e20 7072 6f66   relaxation prof
+00021fc0: 696c 6527 0a20 2020 2029 0a0a 2020 2020  ile'.    )..    
+00021fd0: 6966 2069 7369 6e73 7461 6e63 6528 6461  if isinstance(da
+00021fe0: 7461 7365 742c 2054 6175 4844 6174 6173  taset, TauHDatas
+00021ff0: 6574 293a 0a20 2020 2020 2020 2078 5f76  et):.        x_v
+00022000: 616c 7320 3d20 636f 7079 2e63 6f70 7928  als = copy.copy(
+00022010: 6461 7461 7365 742e 6669 656c 6473 290a  dataset.fields).
+00022020: 2020 2020 2020 2020 6178 2e73 6574 5f78          ax.set_x
+00022030: 6c61 6265 6c28 7227 312f 4820 245c 6c65  label(r'1/H $\le
+00022040: 6674 285c 6d61 7468 7265 6775 6c61 727b  ft(\mathregular{
+00022050: 4f65 7d5e 5c6d 6174 6872 6567 756c 6172  Oe}^\mathregular
+00022060: 7b2d 317d 5c72 6967 6874 2924 2729 0a20  {-1}\right)$'). 
+00022070: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
+00022080: 6365 2864 6174 6173 6574 2c20 5461 7554  ce(dataset, TauT
+00022090: 4461 7461 7365 7429 3a0a 2020 2020 2020  Dataset):.      
+000220a0: 2020 785f 7661 6c73 203d 2063 6f70 792e    x_vals = copy.
+000220b0: 636f 7079 2864 6174 6173 6574 2e74 656d  copy(dataset.tem
+000220c0: 7065 7261 7475 7265 7329 0a20 2020 2020  peratures).     
+000220d0: 2020 2061 782e 7365 745f 786c 6162 656c     ax.set_xlabel
+000220e0: 2872 2731 2f54 2024 5c6c 6566 7428 5c6d  (r'1/T $\left(\m
+000220f0: 6174 6872 6567 756c 6172 7b4b 7d5e 5c6d  athregular{K}^\m
+00022100: 6174 6872 6567 756c 6172 7b2d 317d 5c72  athregular{-1}\r
+00022110: 6967 6874 2924 2729 0a0a 2020 2020 2320  ight)$')..    # 
+00022120: 4164 6420 756e 6365 7274 6169 6e74 6965  Add uncertaintie
+00022130: 7320 6173 2065 7272 6f72 6261 7273 0a20  s as errorbars. 
+00022140: 2020 2069 6620 6c65 6e28 6461 7461 7365     if len(datase
+00022150: 742e 7261 7465 5f70 6d29 3a0a 0a20 2020  t.rate_pm):..   
+00022160: 2020 2020 2023 2043 616c 6375 6c61 7465       # Calculate
+00022170: 2074 696d 6520 6572 726f 7262 6172 730a   time errorbars.
+00022180: 2020 2020 2020 2020 7469 6d65 7320 3d20          times = 
+00022190: 312e 202f 2064 6174 6173 6574 2e72 6174  1. / dataset.rat
+000221a0: 6573 0a20 2020 2020 2020 206d 696e 5f74  es.        min_t
+000221b0: 696d 6520 3d20 312e 202f 2028 6461 7461  ime = 1. / (data
+000221c0: 7365 742e 7261 7465 7320 2b20 6461 7461  set.rates + data
+000221d0: 7365 742e 7261 7465 5f70 6d5b 312c 203a  set.rate_pm[1, :
+000221e0: 5d29 0a20 2020 2020 2020 206d 6178 5f74  ]).        max_t
+000221f0: 696d 6520 3d20 312e 202f 2028 6461 7461  ime = 1. / (data
+00022200: 7365 742e 7261 7465 7320 2d20 6461 7461  set.rates - data
+00022210: 7365 742e 7261 7465 5f70 6d5b 302c 203a  set.rate_pm[0, :
+00022220: 5d29 0a0a 2020 2020 2020 2020 6c6e 5f6d  ])..        ln_m
+00022230: 696e 5f74 696d 6520 3d20 6e70 2e6c 6f67  in_time = np.log
+00022240: 286d 696e 5f74 696d 6529 0a20 2020 2020  (min_time).     
+00022250: 2020 206c 6e5f 6d61 785f 7469 6d65 203d     ln_max_time =
+00022260: 206e 702e 6c6f 6728 6d61 785f 7469 6d65   np.log(max_time
+00022270: 290a 0a20 2020 2020 2020 206c 6e5f 7469  )..        ln_ti
+00022280: 6d65 5f70 6c75 7320 3d20 6c6e 5f6d 6178  me_plus = ln_max
+00022290: 5f74 696d 6520 2d20 6e70 2e6c 6f67 2874  _time - np.log(t
+000222a0: 696d 6573 290a 2020 2020 2020 2020 6c6e  imes).        ln
+000222b0: 5f74 696d 655f 6d69 6e75 7320 3d20 6e70  _time_minus = np
+000222c0: 2e6c 6f67 2874 696d 6573 2920 2d20 6c6e  .log(times) - ln
+000222d0: 5f6d 696e 5f74 696d 650a 0a20 2020 2020  _min_time..     
+000222e0: 2020 206c 6e74 696d 655f 6d70 203d 206e     lntime_mp = n
+000222f0: 702e 6172 7261 7928 5b6c 6e5f 7469 6d65  p.array([ln_time
+00022300: 5f6d 696e 7573 2c20 6c6e 5f74 696d 655f  _minus, ln_time_
+00022310: 706c 7573 5d29 0a0a 2020 2020 2020 2020  plus])..        
+00022320: 6178 2e65 7272 6f72 6261 7228 0a20 2020  ax.errorbar(.   
+00022330: 2020 2020 2020 2020 2031 2e20 2f20 785f           1. / x_
+00022340: 7661 6c73 2c0a 2020 2020 2020 2020 2020  vals,.          
+00022350: 2020 6e70 2e6c 6f67 2874 696d 6573 292c    np.log(times),
+00022360: 0a20 2020 2020 2020 2020 2020 2079 6572  .            yer
+00022370: 723d 6c6e 7469 6d65 5f6d 702c 0a20 2020  r=lntime_mp,.   
+00022380: 2020 2020 2020 2020 206d 6172 6b65 723d           marker=
+00022390: 276f 272c 0a20 2020 2020 2020 2020 2020  'o',.           
+000223a0: 206c 773d 302c 0a20 2020 2020 2020 2020   lw=0,.         
+000223b0: 2020 2065 6c69 6e65 7769 6474 683d 312e     elinewidth=1.
+000223c0: 352c 0a20 2020 2020 2020 2020 2020 2066  5,.            f
+000223d0: 696c 6c73 7479 6c65 3d27 6e6f 6e65 272c  illstyle='none',
+000223e0: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
+000223f0: 6f72 3d27 626c 6163 6b27 0a20 2020 2020  or='black'.     
+00022400: 2020 2029 0a20 2020 2065 6c73 653a 0a20     ).    else:. 
+00022410: 2020 2020 2020 2061 782e 706c 6f74 280a         ax.plot(.
+00022420: 2020 2020 2020 2020 2020 2020 312e 202f              1. /
+00022430: 2078 5f76 616c 732c 0a20 2020 2020 2020   x_vals,.       
+00022440: 2020 2020 206e 702e 6c6f 6728 312e 202f       np.log(1. /
+00022450: 2064 6174 6173 6574 2e72 6174 6573 292c   dataset.rates),
+00022460: 0a20 2020 2020 2020 2020 2020 206d 6172  .            mar
+00022470: 6b65 723d 276f 272c 0a20 2020 2020 2020  ker='o',.       
+00022480: 2020 2020 206c 773d 302c 0a20 2020 2020       lw=0,.     
+00022490: 2020 2020 2020 2066 696c 6c73 7479 6c65         fillstyle
+000224a0: 3d27 6e6f 6e65 272c 0a20 2020 2020 2020  ='none',.       
+000224b0: 2020 2020 2063 6f6c 6f72 3d27 626c 6163       color='blac
+000224c0: 6b27 0a20 2020 2020 2020 2029 0a0a 2020  k'.        )..  
+000224d0: 2020 2320 456e 6162 6c65 206d 696e 6f72    # Enable minor
+000224e0: 2074 6963 6b73 0a20 2020 2061 782e 7961   ticks.    ax.ya
+000224f0: 7869 732e 7365 745f 6d69 6e6f 725f 6c6f  xis.set_minor_lo
+00022500: 6361 746f 7228 4175 746f 4d69 6e6f 724c  cator(AutoMinorL
+00022510: 6f63 6174 6f72 2829 290a 2020 2020 6178  ocator()).    ax
+00022520: 2e78 6178 6973 2e73 6574 5f6d 696e 6f72  .xaxis.set_minor
+00022530: 5f6c 6f63 6174 6f72 2841 7574 6f4d 696e  _locator(AutoMin
+00022540: 6f72 4c6f 6361 746f 7228 2929 0a0a 2020  orLocator())..  
+00022550: 2020 6178 2e73 6574 5f79 6c61 6265 6c28    ax.set_ylabel(
+00022560: 7227 245c 6c6e 5c6c 6566 745b 5c74 6175  r'$\ln\left[\tau
+00022570: 5c72 6967 6874 5d24 2024 5c6c 6566 7428  \right]$ $\left(
+00022580: 5c6c 6e5c 6c65 6674 5b5c 6d61 7468 7265  \ln\left[\mathre
+00022590: 6775 6c61 727b 737d 5e5c 6d61 7468 7265  gular{s}^\mathre
+000225a0: 6775 6c61 727b 2d31 7d5c 7269 6768 745d  gular{-1}\right]
+000225b0: 5c72 6967 6874 2924 2729 2023 206e 6f71  \right)$') # noq
+000225c0: 610a 0a20 2020 2066 6967 2e74 6967 6874  a..    fig.tight
+000225d0: 5f6c 6179 6f75 7428 290a 0a20 2020 2069  _layout()..    i
+000225e0: 6620 7368 6f77 3a0a 2020 2020 2020 2020  f show:.        
+000225f0: 706c 742e 7368 6f77 2829 0a0a 2020 2020  plt.show()..    
+00022600: 6966 2073 6176 653a 0a20 2020 2020 2020  if save:.       
+00022610: 2066 6967 2e73 6176 6566 6967 2873 6176   fig.savefig(sav
+00022620: 655f 6e61 6d65 2c20 6470 693d 3530 3029  e_name, dpi=500)
+00022630: 0a20 2020 2020 2020 2069 6620 7665 7262  .        if verb
+00022640: 6f73 653a 0a20 2020 2020 2020 2020 2020  ose:.           
+00022650: 2069 6620 6973 696e 7374 616e 6365 2864   if isinstance(d
+00022660: 6174 6173 6574 2c20 2854 6175 5444 6174  ataset, (TauTDat
+00022670: 6173 6574 2929 3a0a 2020 2020 2020 2020  aset)):.        
+00022680: 2020 2020 2020 2020 5f78 7661 7220 3d20          _xvar = 
+00022690: 2754 270a 2020 2020 2020 2020 2020 2020  'T'.            
+000226a0: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
+000226b0: 6461 7461 7365 742c 2028 5461 7548 4461  dataset, (TauHDa
+000226c0: 7461 7365 7429 293a 0a20 2020 2020 2020  taset)):.       
+000226d0: 2020 2020 2020 2020 205f 7876 6172 203d           _xvar =
+000226e0: 2027 4827 0a20 2020 2020 2020 2020 2020   'H'.           
+000226f0: 2075 742e 6370 7269 6e74 280a 2020 2020   ut.cprint(.    
+00022700: 2020 2020 2020 2020 2020 2020 6627 5c6e              f'\n
+00022710: 2046 6974 7465 6420 6c6e 2874 6175 2920   Fitted ln(tau) 
+00022720: 7673 2031 2f7b 5f78 7661 727d 2070 6c6f  vs 1/{_xvar} plo
+00022730: 7420 7361 7665 6420 746f 205c 6e20 7b73  t saved to \n {s
+00022740: 6176 655f 6e61 6d65 7d5c 6e27 2c20 2320  ave_name}\n', # 
+00022750: 6e6f 7161 0a20 2020 2020 2020 2020 2020  noqa.           
+00022760: 2020 2020 2027 6379 616e 270a 2020 2020       'cyan'.    
+00022770: 2020 2020 2020 2020 290a 0a20 2020 2072          )..    r
+00022780: 6574 7572 6e20 6669 672c 2061 780a 0a0a  eturn fig, ax...
+00022790: 6465 6620 5f70 6c6f 745f 6669 7474 6564  def _plot_fitted
+000227a0: 5f74 696d 6573 2864 6174 6173 6574 3a20  _times(dataset: 
+000227b0: 5461 7554 4461 7461 7365 7420 7c20 5461  TauTDataset | Ta
+000227c0: 7548 4461 7461 7365 742c 0a20 2020 2020  uHDataset,.     
+000227d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000227e0: 2020 6d6f 6465 6c3a 204c 6f67 5461 7554    model: LogTauT
+000227f0: 4d6f 6465 6c20 7c20 4d75 6c74 694c 6f67  Model | MultiLog
+00022800: 5461 7554 4d6f 6465 6c20 7c20 4c6f 6754  TauTModel | LogT
+00022810: 6175 484d 6f64 656c 207c 204d 756c 7469  auHModel | Multi
+00022820: 4c6f 6754 6175 484d 6f64 656c 2c20 2320  LogTauHModel, # 
+00022830: 6e6f 7161 0a20 2020 2020 2020 2020 2020  noqa.           
+00022840: 2020 2020 2020 2020 2020 2020 6669 673a              fig:
+00022850: 2070 6c74 2e46 6967 7572 652c 2061 783a   plt.Figure, ax:
+00022860: 2070 6c74 2e41 7865 732c 0a20 2020 2020   plt.Axes,.     
+00022870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022880: 2020 7368 6f77 5f70 6172 616d 733a 2062    show_params: b
+00022890: 6f6f 6c20 3d20 5472 7565 293a 0a20 2020  ool = True):.   
+000228a0: 2027 2727 0a20 2020 2050 6c6f 7473 2065   '''.    Plots e
+000228b0: 7870 6572 696d 656e 7461 6c20 616e 6420  xperimental and 
+000228c0: 6669 7474 6564 2028 6d6f 6465 6c29 2072  fitted (model) r
+000228d0: 656c 6178 6174 696f 6e20 7261 7465 2061  elaxation rate a
+000228e0: 735c 6e0a 2020 2020 6c6e 2874 6175 2920  s\n.    ln(tau) 
+000228f0: 7673 2031 2f78 7661 7220 7768 6572 6520  vs 1/xvar where 
+00022900: 7876 6172 2069 7320 5420 6f72 2048 2e0a  xvar is T or H..
+00022910: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
+00022920: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00022930: 2020 2064 6174 6173 6574 3a20 5461 7554     dataset: TauT
+00022940: 4461 7461 7365 7420 7c20 5461 7548 4461  Dataset | TauHDa
+00022950: 7461 7365 740a 2020 2020 2020 2020 4461  taset.        Da
+00022960: 7461 7365 7420 746f 2070 6c6f 740a 2020  taset to plot.  
+00022970: 2020 6d6f 6465 6c3a 204c 6f67 5461 7554    model: LogTauT
+00022980: 4d6f 6465 6c20 7c20 4d75 6c74 694c 6f67  Model | MultiLog
+00022990: 5461 7554 4d6f 6465 6c20 7c20 4c6f 6754  TauTModel | LogT
+000229a0: 6175 484d 6f64 656c 207c 204d 756c 7469  auHModel | Multi
+000229b0: 4c6f 6754 6175 484d 6f64 656c 0a20 2020  LogTauHModel.   
+000229c0: 2020 2020 204d 6f64 656c 2028 6669 7474       Model (fitt
+000229d0: 6564 2920 746f 2070 6c6f 740a 2020 2020  ed) to plot.    
+000229e0: 6669 673a 2070 6c74 2e46 6967 7572 650a  fig: plt.Figure.
+000229f0: 2020 2020 2020 2020 4d61 7470 6c6f 746c          Matplotl
+00022a00: 6962 2046 6967 7572 6520 6f62 6a65 6374  ib Figure object
+00022a10: 2075 7365 6420 666f 7220 706c 6f74 0a20   used for plot. 
+00022a20: 2020 2061 783a 2070 6c74 2e41 7865 730a     ax: plt.Axes.
+00022a30: 2020 2020 2020 2020 4d61 7470 6c6f 746c          Matplotl
+00022a40: 6962 2041 7869 7320 6f62 6a65 6374 2075  ib Axis object u
+00022a50: 7365 6420 666f 7220 706c 6f74 0a20 2020  sed for plot.   
+00022a60: 2073 686f 775f 7061 7261 6d73 3a20 626f   show_params: bo
+00022a70: 6f6c 2c20 6465 6661 756c 7420 5472 7565  ol, default True
+00022a80: 0a20 2020 2020 2020 2049 6620 5472 7565  .        If True
+00022a90: 2c20 7368 6f77 7320 6669 7474 6564 2070  , shows fitted p
+00022aa0: 6172 616d 6574 6572 7320 6f6e 2070 6c6f  arameters on plo
+00022ab0: 740a 0a20 2020 2052 6574 7572 6e73 0a20  t..    Returns. 
+00022ac0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 204e     -------.    N
+00022ad0: 6f6e 650a 2020 2020 2727 270a 0a20 2020  one.    '''..   
+00022ae0: 2069 6620 6973 696e 7374 616e 6365 2864   if isinstance(d
+00022af0: 6174 6173 6574 2c20 5461 7548 4461 7461  ataset, TauHData
+00022b00: 7365 7429 3a0a 2020 2020 2020 2020 785f  set):.        x_
+00022b10: 7661 6c73 203d 2063 6f70 792e 636f 7079  vals = copy.copy
+00022b20: 2864 6174 6173 6574 2e66 6965 6c64 7329  (dataset.fields)
+00022b30: 0a20 2020 2020 2020 2061 782e 7365 745f  .        ax.set_
+00022b40: 786c 6162 656c 2872 2731 2f48 2024 5c6c  xlabel(r'1/H $\l
+00022b50: 6566 7428 5c6d 6174 6872 6567 756c 6172  eft(\mathregular
+00022b60: 7b4f 657d 5e5c 6d61 7468 7265 6775 6c61  {Oe}^\mathregula
+00022b70: 727b 2d31 7d5c 7269 6768 7429 2427 290a  r{-1}\right)$').
+00022b80: 2020 2020 2020 2020 785f 7479 7065 203d          x_type =
+00022b90: 2027 6669 656c 6427 0a20 2020 2065 6c69   'field'.    eli
+00022ba0: 6620 6973 696e 7374 616e 6365 2864 6174  f isinstance(dat
+00022bb0: 6173 6574 2c20 5461 7554 4461 7461 7365  aset, TauTDatase
+00022bc0: 7429 3a0a 2020 2020 2020 2020 785f 7661  t):.        x_va
+00022bd0: 6c73 203d 2063 6f70 792e 636f 7079 2864  ls = copy.copy(d
+00022be0: 6174 6173 6574 2e74 656d 7065 7261 7475  ataset.temperatu
+00022bf0: 7265 7329 0a20 2020 2020 2020 2061 782e  res).        ax.
+00022c00: 7365 745f 786c 6162 656c 2872 2731 2f54  set_xlabel(r'1/T
+00022c10: 2024 5c6c 6566 7428 5c6d 6174 6872 6567   $\left(\mathreg
+00022c20: 756c 6172 7b4b 7d5e 5c6d 6174 6872 6567  ular{K}^\mathreg
+00022c30: 756c 6172 7b2d 317d 5c72 6967 6874 2924  ular{-1}\right)$
+00022c40: 2729 0a20 2020 2020 2020 2078 5f74 7970  ').        x_typ
+00022c50: 6520 3d20 2774 656d 7065 7261 7475 7265  e = 'temperature
+00022c60: 270a 0a20 2020 2023 2041 6464 2075 6e63  '..    # Add unc
+00022c70: 6572 7461 696e 7469 6573 2061 7320 6572  ertainties as er
+00022c80: 726f 7262 6172 730a 2020 2020 6966 206c  rorbars.    if l
+00022c90: 656e 2864 6174 6173 6574 2e72 6174 655f  en(dataset.rate_
+00022ca0: 706d 293a 0a0a 2020 2020 2020 2020 2320  pm):..        # 
+00022cb0: 4361 6c63 756c 6174 6520 7469 6d65 2065  Calculate time e
+00022cc0: 7272 6f72 6261 7273 0a20 2020 2020 2020  rrorbars.       
+00022cd0: 2074 696d 6573 203d 2031 2e20 2f20 6461   times = 1. / da
+00022ce0: 7461 7365 742e 7261 7465 730a 2020 2020  taset.rates.    
+00022cf0: 2020 2020 6d69 6e5f 7469 6d65 203d 2031      min_time = 1
+00022d00: 2e20 2f20 2864 6174 6173 6574 2e72 6174  . / (dataset.rat
+00022d10: 6573 202b 2064 6174 6173 6574 2e72 6174  es + dataset.rat
+00022d20: 655f 706d 5b31 2c20 3a5d 290a 2020 2020  e_pm[1, :]).    
+00022d30: 2020 2020 6d61 785f 7469 6d65 203d 2031      max_time = 1
+00022d40: 2e20 2f20 2864 6174 6173 6574 2e72 6174  . / (dataset.rat
+00022d50: 6573 202d 2064 6174 6173 6574 2e72 6174  es - dataset.rat
+00022d60: 655f 706d 5b30 2c20 3a5d 290a 0a20 2020  e_pm[0, :])..   
+00022d70: 2020 2020 206c 6e5f 6d69 6e5f 7469 6d65       ln_min_time
+00022d80: 203d 206e 702e 6c6f 6728 6d69 6e5f 7469   = np.log(min_ti
+00022d90: 6d65 290a 2020 2020 2020 2020 6c6e 5f6d  me).        ln_m
+00022da0: 6178 5f74 696d 6520 3d20 6e70 2e6c 6f67  ax_time = np.log
+00022db0: 286d 6178 5f74 696d 6529 0a0a 2020 2020  (max_time)..    
+00022dc0: 2020 2020 6c6e 5f74 696d 655f 706c 7573      ln_time_plus
+00022dd0: 203d 206c 6e5f 6d61 785f 7469 6d65 202d   = ln_max_time -
+00022de0: 206e 702e 6c6f 6728 7469 6d65 7329 0a20   np.log(times). 
+00022df0: 2020 2020 2020 206c 6e5f 7469 6d65 5f6d         ln_time_m
+00022e00: 696e 7573 203d 206e 702e 6c6f 6728 7469  inus = np.log(ti
+00022e10: 6d65 7329 202d 206c 6e5f 6d69 6e5f 7469  mes) - ln_min_ti
+00022e20: 6d65 0a0a 2020 2020 2020 2020 6c6e 7469  me..        lnti
+00022e30: 6d65 5f6d 7020 3d20 6e70 2e61 7272 6179  me_mp = np.array
+00022e40: 285b 6c6e 5f74 696d 655f 6d69 6e75 732c  ([ln_time_minus,
+00022e50: 206c 6e5f 7469 6d65 5f70 6c75 735d 290a   ln_time_plus]).
+00022e60: 0a20 2020 2020 2020 2061 782e 6572 726f  .        ax.erro
+00022e70: 7262 6172 280a 2020 2020 2020 2020 2020  rbar(.          
+00022e80: 2020 312e 202f 2078 5f76 616c 732c 0a20    1. / x_vals,. 
+00022e90: 2020 2020 2020 2020 2020 206e 702e 6c6f             np.lo
+00022ea0: 6728 7469 6d65 7329 2c0a 2020 2020 2020  g(times),.      
+00022eb0: 2020 2020 2020 7965 7272 3d6c 6e74 696d        yerr=lntim
+00022ec0: 655f 6d70 2c0a 2020 2020 2020 2020 2020  e_mp,.          
+00022ed0: 2020 6d61 726b 6572 3d27 6f27 2c0a 2020    marker='o',.  
+00022ee0: 2020 2020 2020 2020 2020 6c77 3d30 2c0a            lw=0,.
+00022ef0: 2020 2020 2020 2020 2020 2020 656c 696e              elin
+00022f00: 6577 6964 7468 3d31 2e35 2c0a 2020 2020  ewidth=1.5,.    
+00022f10: 2020 2020 2020 2020 6669 6c6c 7374 796c          fillstyl
+00022f20: 653d 276e 6f6e 6527 2c0a 2020 2020 2020  e='none',.      
+00022f30: 2020 2020 2020 6c61 6265 6c3d 2745 7870        label='Exp
+00022f40: 6572 696d 656e 7427 2c0a 2020 2020 2020  eriment',.      
+00022f50: 2020 2020 2020 636f 6c6f 723d 2762 6c61        color='bla
+00022f60: 636b 270a 2020 2020 2020 2020 290a 2020  ck'.        ).  
+00022f70: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00022f80: 6178 2e70 6c6f 7428 0a20 2020 2020 2020  ax.plot(.       
+00022f90: 2020 2020 2031 2e20 2f20 785f 7661 6c73       1. / x_vals
+00022fa0: 2c0a 2020 2020 2020 2020 2020 2020 6e70  ,.            np
+00022fb0: 2e6c 6f67 2831 2e20 2f20 6461 7461 7365  .log(1. / datase
+00022fc0: 742e 7261 7465 7329 2c0a 2020 2020 2020  t.rates),.      
+00022fd0: 2020 2020 2020 6d61 726b 6572 3d27 6f27        marker='o'
+00022fe0: 2c0a 2020 2020 2020 2020 2020 2020 6c77  ,.            lw
+00022ff0: 3d30 2c0a 2020 2020 2020 2020 2020 2020  =0,.            
+00023000: 6669 6c6c 7374 796c 653d 276e 6f6e 6527  fillstyle='none'
+00023010: 2c0a 2020 2020 2020 2020 2020 2020 6c61  ,.            la
+00023020: 6265 6c3d 2745 7870 6572 696d 656e 7427  bel='Experiment'
+00023030: 2c0a 2020 2020 2020 2020 2020 2020 636f  ,.            co
+00023040: 6c6f 723d 2762 6c61 636b 270a 2020 2020  lor='black'.    
+00023050: 2020 2020 290a 0a20 2020 2078 5f76 6172      )..    x_var
+00023060: 735f 6772 6964 203d 206e 702e 6c69 6e73  s_grid = np.lins
+00023070: 7061 6365 280a 2020 2020 2020 2020 6e70  pace(.        np
+00023080: 2e6d 696e 2878 5f76 616c 7329 2c0a 2020  .min(x_vals),.  
+00023090: 2020 2020 2020 6e70 2e6d 6178 2878 5f76        np.max(x_v
+000230a0: 616c 7329 2c0a 2020 2020 2020 2020 3130  als),.        10
+000230b0: 3030 0a20 2020 2029 0a0a 2020 2020 6966  00.    )..    if
+000230c0: 2074 7970 6528 6d6f 6465 6c29 2069 6e20   type(model) in 
+000230d0: 5b4d 756c 7469 4c6f 6754 6175 544d 6f64  [MultiLogTauTMod
+000230e0: 656c 2c20 4d75 6c74 694c 6f67 5461 7548  el, MultiLogTauH
+000230f0: 4d6f 6465 6c5d 3a0a 2020 2020 2020 2020  Model]:.        
+00023100: 6c6f 676d 6f64 656c 7320 3d20 6d6f 6465  logmodels = mode
+00023110: 6c2e 6c6f 676d 6f64 656c 730a 2020 2020  l.logmodels.    
+00023120: 656c 7365 3a0a 2020 2020 2020 2020 6c6f  else:.        lo
+00023130: 676d 6f64 656c 7320 3d20 5b6d 6f64 656c  gmodels = [model
+00023140: 5d0a 0a20 2020 2066 6f72 206c 6f67 6d6f  ]..    for logmo
+00023150: 6465 6c20 696e 206c 6f67 6d6f 6465 6c73  del in logmodels
+00023160: 3a0a 0a20 2020 2020 2020 2069 6620 7479  :..        if ty
+00023170: 7065 286c 6f67 6d6f 6465 6c29 2069 7320  pe(logmodel) is 
+00023180: 4c6f 674f 7262 6163 684d 6f64 656c 3a0a  LogOrbachModel:.
+00023190: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
+000231a0: 6c5f 6669 7420 3d20 275c 6e46 6974 2077  l_fit = '\nFit w
+000231b0: 6974 6827 0a20 2020 2020 2020 2020 2020  ith'.           
+000231c0: 206c 6162 656c 5f66 6974 202b 3d20 275c   label_fit += '\
+000231d0: 6e27 202b 2072 277b 7d20 7b3a 362e 3266  n' + r'{} {:6.2f
+000231e0: 7d20 7327 2e66 6f72 6d61 7428 0a20 2020  } s'.format(.   
+000231f0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+00023200: 6d6f 6465 6c2e 5641 524e 414d 4553 5f4d  model.VARNAMES_M
+00023210: 4d5b 2775 5f65 6666 275d 2c0a 2020 2020  M['u_eff'],.    
+00023220: 2020 2020 2020 2020 2020 2020 6c6f 676d              logm
+00023230: 6f64 656c 2e66 696e 616c 5f76 6172 5f76  odel.final_var_v
+00023240: 616c 7565 735b 2775 5f65 6666 275d 0a20  alues['u_eff']. 
+00023250: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00023260: 2020 2020 2020 2020 206c 6162 656c 5f66           label_f
+00023270: 6974 202b 3d20 275c 6e27 202b 2072 277b  it += '\n' + r'{
+00023280: 7d20 7b3a 3034 2e33 657d 272e 666f 726d  } {:04.3e}'.form
+00023290: 6174 280a 2020 2020 2020 2020 2020 2020  at(.            
+000232a0: 2020 2020 6c6f 676d 6f64 656c 2e56 4152      logmodel.VAR
+000232b0: 4e41 4d45 535f 4d4d 5b27 4127 5d2c 206c  NAMES_MM['A'], l
+000232c0: 6f67 6d6f 6465 6c2e 6669 6e61 6c5f 7661  ogmodel.final_va
+000232d0: 725f 7661 6c75 6573 5b27 4127 5d0a 2020  r_values['A'].  
+000232e0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+000232f0: 2020 2020 656c 6966 2074 7970 6528 6c6f      elif type(lo
+00023300: 676d 6f64 656c 2920 6973 204c 6f67 5261  gmodel) is LogRa
+00023310: 6d61 6e4d 6f64 656c 3a0a 2020 2020 2020  manModel:.      
+00023320: 2020 2020 2020 6c61 6265 6c5f 6669 7420        label_fit 
+00023330: 3d20 275c 6e46 6974 2077 6974 6827 0a20  = '\nFit with'. 
+00023340: 2020 2020 2020 2020 2020 206c 6162 656c             label
+00023350: 5f66 6974 202b 3d20 275c 6e27 202b 2072  _fit += '\n' + r
+00023360: 277b 7d20 7b3a 362e 3266 7d20 7327 2e66  '{} {:6.2f} s'.f
+00023370: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
+00023380: 2020 2020 2020 206c 6f67 6d6f 6465 6c2e         logmodel.
+00023390: 5641 524e 414d 4553 5f4d 4d5b 2752 275d  VARNAMES_MM['R']
+000233a0: 2c20 6c6f 676d 6f64 656c 2e66 696e 616c  , logmodel.final
+000233b0: 5f76 6172 5f76 616c 7565 735b 2752 275d  _var_values['R']
+000233c0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+000233d0: 2020 2020 2020 2020 2020 206c 6162 656c             label
+000233e0: 5f66 6974 202b 3d20 275c 6e27 202b 2072  _fit += '\n' + r
+000233f0: 277b 7d20 7b3a 3034 2e33 657d 272e 666f  '{} {:04.3e}'.fo
+00023400: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
+00023410: 2020 2020 2020 6c6f 676d 6f64 656c 2e56        logmodel.V
+00023420: 4152 4e41 4d45 535f 4d4d 5b27 6e27 5d2c  ARNAMES_MM['n'],
+00023430: 206c 6f67 6d6f 6465 6c2e 6669 6e61 6c5f   logmodel.final_
+00023440: 7661 725f 7661 6c75 6573 5b27 6e27 5d0a  var_values['n'].
+00023450: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00023460: 2020 2020 2020 656c 6966 2074 7970 6528        elif type(
+00023470: 6c6f 676d 6f64 656c 2920 6973 204c 6f67  logmodel) is Log
+00023480: 5154 4d4d 6f64 656c 3a0a 2020 2020 2020  QTMModel:.      
+00023490: 2020 2020 2020 6c61 6265 6c5f 6669 7420        label_fit 
+000234a0: 3d20 275c 6e46 6974 2077 6974 6827 0a20  = '\nFit with'. 
+000234b0: 2020 2020 2020 2020 2020 206c 6162 656c             label
+000234c0: 5f66 6974 202b 3d20 275c 6e27 202b 2072  _fit += '\n' + r
+000234d0: 277b 7d20 7b3a 362e 3266 7d20 7327 2e66  '{} {:6.2f} s'.f
+000234e0: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
+000234f0: 2020 2020 2020 206c 6f67 6d6f 6465 6c2e         logmodel.
+00023500: 5641 524e 414d 4553 5f4d 4d5b 2751 275d  VARNAMES_MM['Q']
+00023510: 2c20 6c6f 676d 6f64 656c 2e66 696e 616c  , logmodel.final
+00023520: 5f76 6172 5f76 616c 7565 735b 2751 275d  _var_values['Q']
+00023530: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00023540: 2020 2020 2020 2065 6c69 6620 7479 7065         elif type
+00023550: 286c 6f67 6d6f 6465 6c29 2069 7320 4c6f  (logmodel) is Lo
+00023560: 6744 6972 6563 744d 6f64 656c 3a0a 2020  gDirectModel:.  
+00023570: 2020 2020 2020 2020 2020 6c61 6265 6c5f            label_
+00023580: 6669 7420 3d20 275c 6e46 6974 2077 6974  fit = '\nFit wit
+00023590: 6827 0a20 2020 2020 2020 2020 2020 206c  h'.            l
+000235a0: 6162 656c 5f66 6974 202b 3d20 275c 6e27  abel_fit += '\n'
+000235b0: 202b 2072 277b 7d20 7b3a 362e 3266 7d20   + r'{} {:6.2f} 
+000235c0: 7327 2e66 6f72 6d61 7428 0a20 2020 2020  s'.format(.     
+000235d0: 2020 2020 2020 2020 2020 206c 6f67 6d6f             logmo
+000235e0: 6465 6c2e 5641 524e 414d 4553 5f4d 4d5b  del.VARNAMES_MM[
+000235f0: 2744 275d 2c20 6c6f 676d 6f64 656c 2e66  'D'], logmodel.f
+00023600: 696e 616c 5f76 6172 5f76 616c 7565 735b  inal_var_values[
+00023610: 2744 275d 0a20 2020 2020 2020 2020 2020  'D'].           
+00023620: 2029 0a20 2020 2020 2020 206d 6f64 656c   ).        model
+00023630: 5f72 6174 6573 203d 2031 302a 2a6c 6f67  _rates = 10**log
+00023640: 6d6f 6465 6c2e 6d6f 6465 6c28 0a20 2020  model.model(.   
+00023650: 2020 2020 2020 2020 206c 6f67 6d6f 6465           logmode
+00023660: 6c2e 6669 6e61 6c5f 7661 725f 7661 6c75  l.final_var_valu
+00023670: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
+00023680: 785f 7661 7273 5f67 7269 642c 0a20 2020  x_vars_grid,.   
+00023690: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+000236a0: 6178 2e70 6c6f 7428 0a20 2020 2020 2020  ax.plot(.       
+000236b0: 2020 2020 2031 2e20 2f20 6e70 2e61 7272       1. / np.arr
+000236c0: 6179 2878 5f76 6172 735f 6772 6964 292c  ay(x_vars_grid),
+000236d0: 0a20 2020 2020 2020 2020 2020 206e 702e  .            np.
+000236e0: 6c6f 6728 312e 202f 206e 702e 6172 7261  log(1. / np.arra
+000236f0: 7928 6d6f 6465 6c5f 7261 7465 7329 292c  y(model_rates)),
+00023700: 0a20 2020 2020 2020 2020 2020 206c 773d  .            lw=
+00023710: 312e 352c 0a20 2020 2020 2020 2020 2020  1.5,.           
+00023720: 206c 6162 656c 3d6c 6f67 6d6f 6465 6c2e   label=logmodel.
+00023730: 4e41 4d45 2c0a 2020 2020 2020 2020 2020  NAME,.          
+00023740: 2020 6c73 3d27 2d2d 270a 2020 2020 2020    ls='--'.      
+00023750: 2020 290a 0a20 2020 2069 6620 7479 7065    )..    if type
+00023760: 286d 6f64 656c 2920 696e 205b 4d75 6c74  (model) in [Mult
+00023770: 694c 6f67 5461 7554 4d6f 6465 6c2c 204d  iLogTauTModel, M
+00023780: 756c 7469 4c6f 6754 6175 484d 6f64 656c  ultiLogTauHModel
+00023790: 5d20 616e 6420 6c65 6e28 6c6f 676d 6f64  ] and len(logmod
+000237a0: 656c 7329 203e 2031 3a20 2320 6e6f 7161  els) > 1: # noqa
+000237b0: 0a20 2020 2020 2020 2074 6f74 616c 203d  .        total =
+000237c0: 206e 702e 7a65 726f 7328 6c65 6e28 785f   np.zeros(len(x_
+000237d0: 7661 7273 5f67 7269 6429 290a 0a20 2020  vars_grid))..   
+000237e0: 2020 2020 2066 6f72 206c 6f67 6d6f 6465       for logmode
+000237f0: 6c20 696e 206c 6f67 6d6f 6465 6c73 3a0a  l in logmodels:.
+00023800: 2020 2020 2020 2020 2020 2020 746f 7461              tota
+00023810: 6c20 2b3d 2031 302a 2a6c 6f67 6d6f 6465  l += 10**logmode
+00023820: 6c2e 6d6f 6465 6c28 0a20 2020 2020 2020  l.model(.       
+00023830: 2020 2020 2020 2020 206c 6f67 6d6f 6465           logmode
+00023840: 6c2e 6669 6e61 6c5f 7661 725f 7661 6c75  l.final_var_valu
+00023850: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
+00023860: 2020 2020 785f 7661 7273 5f67 7269 642c      x_vars_grid,
+00023870: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+00023880: 2020 2020 2020 2020 6178 2e70 6c6f 7428          ax.plot(
+00023890: 0a20 2020 2020 2020 2020 2020 2031 2e20  .            1. 
+000238a0: 2f20 785f 7661 7273 5f67 7269 642c 0a20  / x_vars_grid,. 
+000238b0: 2020 2020 2020 2020 2020 206e 702e 6c6f             np.lo
+000238c0: 6728 312e 202f 2074 6f74 616c 292c 0a20  g(1. / total),. 
+000238d0: 2020 2020 2020 2020 2020 206c 773d 312e             lw=1.
+000238e0: 352c 0a20 2020 2020 2020 2020 2020 206c  5,.            l
+000238f0: 6162 656c 3d27 546f 7461 6c27 2c0a 2020  abel='Total',.  
+00023900: 2020 2020 2020 2020 2020 636f 6c6f 723d            color=
+00023910: 2772 6564 270a 2020 2020 2020 2020 290a  'red'.        ).
+00023920: 0a20 2020 2023 2045 6e61 626c 6520 6d69  .    # Enable mi
+00023930: 6e6f 7220 7469 636b 730a 2020 2020 6178  nor ticks.    ax
+00023940: 2e79 6178 6973 2e73 6574 5f6d 696e 6f72  .yaxis.set_minor
+00023950: 5f6c 6f63 6174 6f72 2841 7574 6f4d 696e  _locator(AutoMin
+00023960: 6f72 4c6f 6361 746f 7228 2929 0a20 2020  orLocator()).   
+00023970: 2061 782e 7861 7869 732e 7365 745f 6d69   ax.xaxis.set_mi
+00023980: 6e6f 725f 6c6f 6361 746f 7228 4175 746f  nor_locator(Auto
+00023990: 4d69 6e6f 724c 6f63 6174 6f72 2829 290a  MinorLocator()).
+000239a0: 0a20 2020 2065 7870 7265 7373 696f 6e20  .    expression 
+000239b0: 3d20 2727 0a0a 2020 2020 666f 7220 6c6f  = ''..    for lo
+000239c0: 676d 6f64 656c 2069 6e20 6c6f 676d 6f64  gmodel in logmod
+000239d0: 656c 733a 0a20 2020 2020 2020 2066 6f72  els:.        for
+000239e0: 2069 742c 206e 616d 6520 696e 2065 6e75   it, name in enu
+000239f0: 6d65 7261 7465 286c 6f67 6d6f 6465 6c2e  merate(logmodel.
+00023a00: 5041 524e 414d 4553 293a 0a20 2020 2020  PARNAMES):.     
+00023a10: 2020 2020 2020 2065 7870 7265 7373 696f         expressio
+00023a20: 6e20 2b3d 2027 7b7d 203d 207b 3a2e 3366  n += '{} = {:.3f
+00023a30: 7d20 272e 666f 726d 6174 280a 2020 2020  } '.format(.    
+00023a40: 2020 2020 2020 2020 2020 2020 6c6f 676d              logm
+00023a50: 6f64 656c 2e56 4152 4e41 4d45 535f 4d4d  odel.VARNAMES_MM
+00023a60: 5b6e 616d 655d 2c0a 2020 2020 2020 2020  [name],.        
+00023a70: 2020 2020 2020 2020 6c6f 676d 6f64 656c          logmodel
+00023a80: 2e66 696e 616c 5f76 6172 5f76 616c 7565  .final_var_value
+00023a90: 735b 6e61 6d65 5d2c 0a20 2020 2020 2020  s[name],.       
+00023aa0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00023ab0: 2020 2069 6620 6e61 6d65 2069 6e20 6c6f     if name in lo
+00023ac0: 676d 6f64 656c 2e66 6974 5f76 6172 732e  gmodel.fit_vars.
+00023ad0: 6b65 7973 2829 3a0a 2020 2020 2020 2020  keys():.        
+00023ae0: 2020 2020 2020 2020 6578 7072 6573 7369          expressi
+00023af0: 6f6e 202b 3d20 7227 245c 706d 2420 270a  on += r'$\pm$ '.
+00023b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023b10: 6578 7072 6573 7369 6f6e 202b 3d20 277b  expression += '{
+00023b20: 3a2e 3366 7d20 272e 666f 726d 6174 286c  :.3f} '.format(l
+00023b30: 6f67 6d6f 6465 6c2e 6669 745f 7374 6465  ogmodel.fit_stde
+00023b40: 765b 6e61 6d65 5d29 0a20 2020 2020 2020  v[name]).       
+00023b50: 2020 2020 2065 7870 7265 7373 696f 6e20       expression 
+00023b60: 2b3d 2027 7b7d 2020 2020 272e 666f 726d  += '{}    '.form
+00023b70: 6174 286c 6f67 6d6f 6465 6c2e 554e 4954  at(logmodel.UNIT
+00023b80: 535f 4d4d 5b6e 616d 655d 290a 2020 2020  S_MM[name]).    
+00023b90: 2020 2020 2020 2020 6966 2069 7420 3d3d          if it ==
+00023ba0: 2031 2061 6e64 206c 656e 286c 6f67 6d6f   1 and len(logmo
+00023bb0: 6465 6c2e 6669 745f 7661 7273 2e6b 6579  del.fit_vars.key
+00023bc0: 7328 2929 203e 2032 3a0a 2020 2020 2020  s()) > 2:.      
+00023bd0: 2020 2020 2020 2020 2020 6578 7072 6573            expres
+00023be0: 7369 6f6e 202b 3d20 275c 6e27 0a20 2020  sion += '\n'.   
+00023bf0: 2020 2020 2065 7870 7265 7373 696f 6e20       expression 
+00023c00: 2b3d 2027 5c6e 270a 0a20 2020 2069 6620  += '\n'..    if 
+00023c10: 7368 6f77 5f70 6172 616d 733a 0a20 2020  show_params:.   
+00023c20: 2020 2020 2061 782e 7465 7874 280a 2020       ax.text(.  
+00023c30: 2020 2020 2020 2020 2020 302e 302c 2031            0.0, 1
+00023c40: 2e30 322c 2073 3d65 7870 7265 7373 696f  .02, s=expressio
+00023c50: 6e2c 2066 6f6e 7473 697a 653d 3130 2c20  n, fontsize=10, 
+00023c60: 7472 616e 7366 6f72 6d3d 6178 2e74 7261  transform=ax.tra
+00023c70: 6e73 4178 6573 0a20 2020 2020 2020 2029  nsAxes.        )
+00023c80: 0a0a 2020 2020 6966 2078 5f74 7970 6520  ..    if x_type 
+00023c90: 3d3d 2027 6669 656c 6427 3a0a 2020 2020  == 'field':.    
+00023ca0: 2020 2020 6178 2e6c 6567 656e 6428 0a20      ax.legend(. 
+00023cb0: 2020 2020 2020 2020 2020 2066 6f6e 7473             fonts
+00023cc0: 697a 653d 2731 3027 2c20 6e75 6d70 6f69  ize='10', numpoi
+00023cd0: 6e74 733d 312c 206e 636f 6c3d 312c 2066  nts=1, ncol=1, f
+00023ce0: 7261 6d65 6f6e 3d46 616c 7365 0a20 2020  rameon=False.   
+00023cf0: 2020 2020 2029 0a20 2020 2065 6c73 653a       ).    else:
+00023d00: 0a20 2020 2020 2020 2061 782e 6c65 6765  .        ax.lege
+00023d10: 6e64 280a 2020 2020 2020 2020 2020 2020  nd(.            
+00023d20: 6c6f 633d 276c 6f77 6572 2072 6967 6874  loc='lower right
+00023d30: 272c 2066 6f6e 7473 697a 653d 2731 3027  ', fontsize='10'
+00023d40: 2c20 6e75 6d70 6f69 6e74 733d 312c 206e  , numpoints=1, n
+00023d50: 636f 6c3d 312c 0a20 2020 2020 2020 2020  col=1,.         
+00023d60: 2020 2066 7261 6d65 6f6e 3d46 616c 7365     frameon=False
+00023d70: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00023d80: 6178 2e73 6574 5f79 6c61 6265 6c28 7227  ax.set_ylabel(r'
+00023d90: 245c 6c6e 5c6c 6566 745b 5c74 6175 5c72  $\ln\left[\tau\r
+00023da0: 6967 6874 5d24 2028 245c 6c6e 5c6c 6566  ight]$ ($\ln\lef
+00023db0: 745b 5c6d 6174 6872 6567 756c 6172 7b73  t[\mathregular{s
+00023dc0: 7d5e 5c6d 6174 6872 6567 756c 6172 7b2d  }^\mathregular{-
+00023dd0: 317d 5c72 6967 6874 5d24 2927 2920 2320  1}\right]$)') # 
+00023de0: 6e6f 7161 0a0a 2020 2020 7265 7475 726e  noqa..    return
+00023df0: 0a0a 0a64 6566 2070 6c6f 745f 6669 7474  ...def plot_fitt
+00023e00: 6564 5f72 6174 6573 2864 6174 6173 6574  ed_rates(dataset
+00023e10: 3a20 5461 7554 4461 7461 7365 7420 7c20  : TauTDataset | 
+00023e20: 5461 7548 4461 7461 7365 742c 0a20 2020  TauHDataset,.   
+00023e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023e40: 2020 206d 6f64 656c 3a20 4c6f 6754 6175     model: LogTau
+00023e50: 544d 6f64 656c 207c 204d 756c 7469 4c6f  TModel | MultiLo
+00023e60: 6754 6175 544d 6f64 656c 207c 204c 6f67  gTauTModel | Log
+00023e70: 5461 7548 4d6f 6465 6c20 7c20 4d75 6c74  TauHModel | Mult
+00023e80: 694c 6f67 5461 7548 4d6f 6465 6c2c 2023  iLogTauHModel, #
+00023e90: 206e 6f71 610a 2020 2020 2020 2020 2020   noqa.          
+00023ea0: 2020 2020 2020 2020 2020 2020 7368 6f77              show
+00023eb0: 3a20 626f 6f6c 203d 2054 7275 652c 2073  : bool = True, s
+00023ec0: 6176 653a 2062 6f6f 6c20 3d20 4661 6c73  ave: bool = Fals
+00023ed0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00023ee0: 2020 2020 2020 2020 2073 6176 655f 6e61           save_na
+00023ef0: 6d65 3a20 7374 7220 3d20 2766 6974 7465  me: str = 'fitte
+00023f00: 645f 7261 7465 732e 706e 6727 2c0a 2020  d_rates.png',.  
 00023f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023f20: 7665 7262 6f73 653a 2062 6f6f 6c20 3d20  verbose: bool = 
-00023f30: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-00023f40: 2020 2020 2020 2020 2020 2020 7368 6f77              show
-00023f50: 5f70 6172 616d 733a 2062 6f6f 6c20 3d20  _params: bool = 
-00023f60: 5472 7565 2920 2d3e 2074 7570 6c65 5b70  True) -> tuple[p
-00023f70: 6c74 2e46 6967 7572 652c 2070 6c74 2e41  lt.Figure, plt.A
-00023f80: 7865 735d 3a0a 2020 2020 2727 270a 2020  xes]:.    '''.  
-00023f90: 2020 506c 6f74 7320 6578 7065 7269 6d65    Plots experime
-00023fa0: 6e74 616c 2061 6e64 2066 6974 7465 6420  ntal and fitted 
-00023fb0: 286d 6f64 656c 2920 7265 6c61 7861 7469  (model) relaxati
-00023fc0: 6f6e 2072 6174 6520 6173 5c6e 0a20 2020  on rate as\n.   
-00023fd0: 2072 6174 6520 7673 2078 7661 7220 7768   rate vs xvar wh
-00023fe0: 6572 6520 7876 6172 2069 7320 5420 6f72  ere xvar is T or
-00023ff0: 2048 2e20 5769 7468 206c 6f67 206c 6f67   H. With log log
-00024000: 2073 6361 6c65 2e0a 0a20 2020 2050 6172   scale...    Par
-00024010: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-00024020: 2d2d 2d2d 2d2d 0a20 2020 2064 6174 6173  ------.    datas
-00024030: 6574 3a20 5461 7554 4461 7461 7365 7420  et: TauTDataset 
-00024040: 7c20 5461 7548 4461 7461 7365 740a 2020  | TauHDataset.  
-00024050: 2020 2020 2020 4461 7461 7365 7420 746f        Dataset to
-00024060: 2070 6c6f 740a 2020 2020 6d6f 6465 6c3a   plot.    model:
-00024070: 204c 6f67 5461 7554 4d6f 6465 6c20 7c20   LogTauTModel | 
-00024080: 4d75 6c74 694c 6f67 5461 7554 4d6f 6465  MultiLogTauTMode
-00024090: 6c20 7c20 4c6f 6754 6175 484d 6f64 656c  l | LogTauHModel
-000240a0: 207c 204d 756c 7469 4c6f 6754 6175 484d   | MultiLogTauHM
-000240b0: 6f64 656c 0a20 2020 2020 2020 204d 6f64  odel.        Mod
-000240c0: 656c 2028 6669 7474 6564 2920 746f 2070  el (fitted) to p
-000240d0: 6c6f 740a 2020 2020 7368 6f77 3a20 626f  lot.    show: bo
-000240e0: 6f6c 2c20 6465 6661 756c 7420 5472 7565  ol, default True
-000240f0: 0a20 2020 2020 2020 2049 6620 5472 7565  .        If True
-00024100: 2c20 7368 6f77 2070 6c6f 7420 6f6e 2073  , show plot on s
-00024110: 6372 6565 6e0a 2020 2020 7361 7665 3a20  creen.    save: 
-00024120: 626f 6f6c 2c20 6465 6661 756c 7420 4661  bool, default Fa
-00024130: 6c73 650a 2020 2020 2020 2020 4966 2054  lse.        If T
-00024140: 7275 652c 2073 6176 6520 706c 6f74 2074  rue, save plot t
-00024150: 6f20 6669 6c65 2060 7361 7665 5f6e 616d  o file `save_nam
-00024160: 6560 0a20 2020 2073 6176 655f 6e61 6d65  e`.    save_name
-00024170: 3a20 7374 722c 2064 6566 6175 6c74 203d  : str, default =
-00024180: 2027 6669 7474 6564 5f72 6174 6573 2e70   'fitted_rates.p
-00024190: 6e67 270a 2020 2020 2020 2020 4966 2073  ng'.        If s
-000241a0: 6176 6520 6973 2054 7275 652c 2077 696c  ave is True, wil
-000241b0: 6c20 7361 7665 2070 6c6f 7420 746f 2074  l save plot to t
-000241c0: 6869 7320 6669 6c65 6e61 6d65 0a20 2020  his filename.   
-000241d0: 2076 6572 626f 7365 3a20 626f 6f6c 2c20   verbose: bool, 
-000241e0: 6465 6661 756c 7420 5472 7565 0a20 2020  default True.   
-000241f0: 2020 2020 2049 6620 5472 7565 2c20 706c       If True, pl
-00024200: 6f74 2066 696c 6520 6c6f 6361 7469 6f6e  ot file location
-00024210: 2069 7320 7772 6974 7465 6e20 746f 2074   is written to t
-00024220: 6572 6d69 6e61 6c0a 2020 2020 7368 6f77  erminal.    show
-00024230: 5f70 6172 616d 733a 2062 6f6f 6c2c 2064  _params: bool, d
-00024240: 6566 6175 6c74 2054 7275 650a 2020 2020  efault True.    
-00024250: 2020 2020 4966 2054 7275 652c 2073 686f      If True, sho
-00024260: 7773 2066 6974 7465 6420 7061 7261 6d65  ws fitted parame
-00024270: 7465 7273 206f 6e20 706c 6f74 0a0a 2020  ters on plot..  
-00024280: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
-00024290: 2d2d 2d2d 2d0a 2020 2020 706c 742e 4669  -----.    plt.Fi
-000242a0: 6775 7265 0a20 2020 2020 2020 204d 6174  gure.        Mat
-000242b0: 706c 6f74 6c69 6220 6669 6775 7265 206f  plotlib figure o
-000242c0: 626a 6563 740a 2020 2020 706c 742e 4178  bject.    plt.Ax
-000242d0: 6573 0a20 2020 2020 2020 204d 6174 706c  es.        Matpl
-000242e0: 6f74 6c69 6220 6178 6973 206f 626a 6563  otlib axis objec
-000242f0: 740a 2020 2020 2727 270a 0a20 2020 2069  t.    '''..    i
-00024300: 6620 7368 6f77 5f70 6172 616d 733a 0a20  f show_params:. 
-00024310: 2020 2020 2020 2066 6967 7369 7a65 203d         figsize =
-00024320: 2028 362c 2036 290a 2020 2020 656c 7365   (6, 6).    else
-00024330: 3a0a 2020 2020 2020 2020 6669 6773 697a  :.        figsiz
-00024340: 6520 3d20 2836 2c20 352e 3529 0a0a 2020  e = (6, 5.5)..  
-00024350: 2020 2320 4372 6561 7465 2066 6967 7572    # Create figur
-00024360: 6520 616e 6420 6178 6573 0a20 2020 2066  e and axes.    f
-00024370: 6967 2c20 6178 203d 2070 6c74 2e73 7562  ig, ax = plt.sub
-00024380: 706c 6f74 7328 0a20 2020 2020 2020 2031  plots(.        1
-00024390: 2c0a 2020 2020 2020 2020 312c 0a20 2020  ,.        1,.   
-000243a0: 2020 2020 2073 6861 7265 783d 5472 7565       sharex=True
-000243b0: 2c0a 2020 2020 2020 2020 7368 6172 6579  ,.        sharey
-000243c0: 3d54 7275 652c 0a20 2020 2020 2020 2066  =True,.        f
-000243d0: 6967 7369 7a65 3d66 6967 7369 7a65 2c0a  igsize=figsize,.
-000243e0: 2020 2020 2020 2020 6e75 6d3d 2746 6974          num='Fit
-000243f0: 7465 6420 7265 6c61 7861 7469 6f6e 2070  ted relaxation p
-00024400: 726f 6669 6c65 270a 2020 2020 290a 0a20  rofile'.    ).. 
-00024410: 2020 205f 706c 6f74 5f66 6974 7465 645f     _plot_fitted_
-00024420: 7261 7465 7328 6461 7461 7365 742c 206d  rates(dataset, m
-00024430: 6f64 656c 2c20 6669 672c 2061 782c 2073  odel, fig, ax, s
-00024440: 686f 775f 7061 7261 6d73 3d73 686f 775f  how_params=show_
-00024450: 7061 7261 6d73 290a 0a20 2020 2066 6967  params)..    fig
-00024460: 2e74 6967 6874 5f6c 6179 6f75 7428 290a  .tight_layout().
-00024470: 0a20 2020 2077 6172 6e69 6e67 732e 7369  .    warnings.si
-00024480: 6d70 6c65 6669 6c74 6572 2827 6967 6e6f  mplefilter('igno
-00024490: 7265 272c 2055 7365 7257 6172 6e69 6e67  re', UserWarning
-000244a0: 290a 2020 2020 6966 2073 686f 773a 0a20  ).    if show:. 
-000244b0: 2020 2020 2020 2070 6c74 2e73 686f 7728         plt.show(
-000244c0: 290a 0a20 2020 2069 6620 7361 7665 3a0a  )..    if save:.
-000244d0: 2020 2020 2020 2020 6669 672e 7361 7665          fig.save
-000244e0: 6669 6728 7361 7665 5f6e 616d 652c 2064  fig(save_name, d
-000244f0: 7069 3d35 3030 290a 2020 2020 2020 2020  pi=500).        
-00024500: 6966 2076 6572 626f 7365 3a0a 2020 2020  if verbose:.    
-00024510: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-00024520: 7461 6e63 6528 6461 7461 7365 742c 2028  tance(dataset, (
-00024530: 5461 7554 4461 7461 7365 7429 293a 0a20  TauTDataset)):. 
-00024540: 2020 2020 2020 2020 2020 2020 2020 205f                 _
-00024550: 7876 6172 203d 2027 5427 0a20 2020 2020  xvar = 'T'.     
-00024560: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
-00024570: 7374 616e 6365 2864 6174 6173 6574 2c20  stance(dataset, 
-00024580: 2854 6175 4844 6174 6173 6574 2929 3a0a  (TauHDataset)):.
-00024590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000245a0: 5f78 7661 7220 3d20 2748 270a 2020 2020  _xvar = 'H'.    
-000245b0: 2020 2020 2020 2020 7574 2e63 7072 696e          ut.cprin
-000245c0: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-000245d0: 2020 2066 275c 6e20 4669 7474 6564 20cf     f'\n Fitted .
-000245e0: 84e2 81bb c2b9 2076 7320 7b5f 7876 6172  ...... vs {_xvar
-000245f0: 7d20 706c 6f74 2073 6176 6564 2074 6f20  } plot saved to 
-00024600: 5c6e 207b 7361 7665 5f6e 616d 657d 5c6e  \n {save_name}\n
-00024610: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-00024620: 2020 2027 6379 616e 270a 2020 2020 2020     'cyan'.      
-00024630: 2020 2020 2020 290a 2020 2020 7761 726e        ).    warn
-00024640: 696e 6773 2e73 696d 706c 6566 696c 7465  ings.simplefilte
-00024650: 7228 2764 6566 6175 6c74 272c 2055 7365  r('default', Use
-00024660: 7257 6172 6e69 6e67 290a 0a20 2020 2072  rWarning)..    r
-00024670: 6574 7572 6e20 6669 672c 2061 780a 0a0a  eturn fig, ax...
-00024680: 6465 6620 7174 5f70 6c6f 745f 6669 7474  def qt_plot_fitt
-00024690: 6564 5f72 6174 6573 2861 7070 3a20 5174  ed_rates(app: Qt
-000246a0: 5769 6467 6574 732e 5141 7070 6c69 6361  Widgets.QApplica
-000246b0: 7469 6f6e 2c0a 2020 2020 2020 2020 2020  tion,.          
-000246c0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-000246d0: 6174 6173 6574 3a20 5461 7554 4461 7461  ataset: TauTData
-000246e0: 7365 7420 7c20 5461 7548 4461 7461 7365  set | TauHDatase
-000246f0: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
-00024700: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
-00024710: 6c3a 204c 6f67 5461 7554 4d6f 6465 6c20  l: LogTauTModel 
-00024720: 7c20 4d75 6c74 694c 6f67 5461 7554 4d6f  | MultiLogTauTMo
-00024730: 6465 6c20 7c20 4c6f 6754 6175 484d 6f64  del | LogTauHMod
-00024740: 656c 207c 204d 756c 7469 4c6f 6754 6175  el | MultiLogTau
-00024750: 484d 6f64 656c 2c20 2320 6e6f 7161 0a20  HModel, # noqa. 
-00024760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024770: 2020 2020 2020 2020 7361 7665 3a20 626f          save: bo
-00024780: 6f6c 203d 2046 616c 7365 2c20 7368 6f77  ol = False, show
-00024790: 3a20 626f 6f6c 203d 2054 7275 652c 0a20  : bool = True,. 
-000247a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000247b0: 2020 2020 2020 2020 7361 7665 5f6e 616d          save_nam
-000247c0: 653a 2073 7472 203d 2027 6669 7474 6564  e: str = 'fitted
-000247d0: 5f72 6174 6573 2e70 6e67 272c 0a20 2020  _rates.png',.   
-000247e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000247f0: 2020 2020 2020 7665 7262 6f73 653a 2062        verbose: b
-00024800: 6f6f 6c20 3d20 5472 7565 2c0a 2020 2020  ool = True,.    
+00023f20: 2020 2020 7665 7262 6f73 653a 2062 6f6f      verbose: boo
+00023f30: 6c20 3d20 5472 7565 2c0a 2020 2020 2020  l = True,.      
+00023f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023f50: 7368 6f77 5f70 6172 616d 733a 2062 6f6f  show_params: boo
+00023f60: 6c20 3d20 5472 7565 2920 2d3e 2074 7570  l = True) -> tup
+00023f70: 6c65 5b70 6c74 2e46 6967 7572 652c 2070  le[plt.Figure, p
+00023f80: 6c74 2e41 7865 735d 3a0a 2020 2020 2727  lt.Axes]:.    ''
+00023f90: 270a 2020 2020 506c 6f74 7320 6578 7065  '.    Plots expe
+00023fa0: 7269 6d65 6e74 616c 2061 6e64 2066 6974  rimental and fit
+00023fb0: 7465 6420 286d 6f64 656c 2920 7265 6c61  ted (model) rela
+00023fc0: 7861 7469 6f6e 2072 6174 6520 6173 5c6e  xation rate as\n
+00023fd0: 0a20 2020 2072 6174 6520 7673 2078 7661  .    rate vs xva
+00023fe0: 7220 7768 6572 6520 7876 6172 2069 7320  r where xvar is 
+00023ff0: 5420 6f72 2048 2e20 5769 7468 206c 6f67  T or H. With log
+00024000: 206c 6f67 2073 6361 6c65 2e0a 0a20 2020   log scale...   
+00024010: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00024020: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064  ----------.    d
+00024030: 6174 6173 6574 3a20 5461 7554 4461 7461  ataset: TauTData
+00024040: 7365 7420 7c20 5461 7548 4461 7461 7365  set | TauHDatase
+00024050: 740a 2020 2020 2020 2020 4461 7461 7365  t.        Datase
+00024060: 7420 746f 2070 6c6f 740a 2020 2020 6d6f  t to plot.    mo
+00024070: 6465 6c3a 204c 6f67 5461 7554 4d6f 6465  del: LogTauTMode
+00024080: 6c20 7c20 4d75 6c74 694c 6f67 5461 7554  l | MultiLogTauT
+00024090: 4d6f 6465 6c20 7c20 4c6f 6754 6175 484d  Model | LogTauHM
+000240a0: 6f64 656c 207c 204d 756c 7469 4c6f 6754  odel | MultiLogT
+000240b0: 6175 484d 6f64 656c 0a20 2020 2020 2020  auHModel.       
+000240c0: 204d 6f64 656c 2028 6669 7474 6564 2920   Model (fitted) 
+000240d0: 746f 2070 6c6f 740a 2020 2020 7368 6f77  to plot.    show
+000240e0: 3a20 626f 6f6c 2c20 6465 6661 756c 7420  : bool, default 
+000240f0: 5472 7565 0a20 2020 2020 2020 2049 6620  True.        If 
+00024100: 5472 7565 2c20 7368 6f77 2070 6c6f 7420  True, show plot 
+00024110: 6f6e 2073 6372 6565 6e0a 2020 2020 7361  on screen.    sa
+00024120: 7665 3a20 626f 6f6c 2c20 6465 6661 756c  ve: bool, defaul
+00024130: 7420 4661 6c73 650a 2020 2020 2020 2020  t False.        
+00024140: 4966 2054 7275 652c 2073 6176 6520 706c  If True, save pl
+00024150: 6f74 2074 6f20 6669 6c65 2060 7361 7665  ot to file `save
+00024160: 5f6e 616d 6560 0a20 2020 2073 6176 655f  _name`.    save_
+00024170: 6e61 6d65 3a20 7374 722c 2064 6566 6175  name: str, defau
+00024180: 6c74 203d 2027 6669 7474 6564 5f72 6174  lt = 'fitted_rat
+00024190: 6573 2e70 6e67 270a 2020 2020 2020 2020  es.png'.        
+000241a0: 4966 2073 6176 6520 6973 2054 7275 652c  If save is True,
+000241b0: 2077 696c 6c20 7361 7665 2070 6c6f 7420   will save plot 
+000241c0: 746f 2074 6869 7320 6669 6c65 6e61 6d65  to this filename
+000241d0: 0a20 2020 2076 6572 626f 7365 3a20 626f  .    verbose: bo
+000241e0: 6f6c 2c20 6465 6661 756c 7420 5472 7565  ol, default True
+000241f0: 0a20 2020 2020 2020 2049 6620 5472 7565  .        If True
+00024200: 2c20 706c 6f74 2066 696c 6520 6c6f 6361  , plot file loca
+00024210: 7469 6f6e 2069 7320 7772 6974 7465 6e20  tion is written 
+00024220: 746f 2074 6572 6d69 6e61 6c0a 2020 2020  to terminal.    
+00024230: 7368 6f77 5f70 6172 616d 733a 2062 6f6f  show_params: boo
+00024240: 6c2c 2064 6566 6175 6c74 2054 7275 650a  l, default True.
+00024250: 2020 2020 2020 2020 4966 2054 7275 652c          If True,
+00024260: 2073 686f 7773 2066 6974 7465 6420 7061   shows fitted pa
+00024270: 7261 6d65 7465 7273 206f 6e20 706c 6f74  rameters on plot
+00024280: 0a0a 2020 2020 5265 7475 726e 730a 2020  ..    Returns.  
+00024290: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 706c    -------.    pl
+000242a0: 742e 4669 6775 7265 0a20 2020 2020 2020  t.Figure.       
+000242b0: 204d 6174 706c 6f74 6c69 6220 6669 6775   Matplotlib figu
+000242c0: 7265 206f 626a 6563 740a 2020 2020 706c  re object.    pl
+000242d0: 742e 4178 6573 0a20 2020 2020 2020 204d  t.Axes.        M
+000242e0: 6174 706c 6f74 6c69 6220 6178 6973 206f  atplotlib axis o
+000242f0: 626a 6563 740a 2020 2020 2727 270a 0a20  bject.    '''.. 
+00024300: 2020 2069 6620 7368 6f77 5f70 6172 616d     if show_param
+00024310: 733a 0a20 2020 2020 2020 2066 6967 7369  s:.        figsi
+00024320: 7a65 203d 2028 362c 2036 290a 2020 2020  ze = (6, 6).    
+00024330: 656c 7365 3a0a 2020 2020 2020 2020 6669  else:.        fi
+00024340: 6773 697a 6520 3d20 2836 2c20 352e 3529  gsize = (6, 5.5)
+00024350: 0a0a 2020 2020 2320 4372 6561 7465 2066  ..    # Create f
+00024360: 6967 7572 6520 616e 6420 6178 6573 0a20  igure and axes. 
+00024370: 2020 2066 6967 2c20 6178 203d 2070 6c74     fig, ax = plt
+00024380: 2e73 7562 706c 6f74 7328 0a20 2020 2020  .subplots(.     
+00024390: 2020 2031 2c0a 2020 2020 2020 2020 312c     1,.        1,
+000243a0: 0a20 2020 2020 2020 2073 6861 7265 783d  .        sharex=
+000243b0: 5472 7565 2c0a 2020 2020 2020 2020 7368  True,.        sh
+000243c0: 6172 6579 3d54 7275 652c 0a20 2020 2020  arey=True,.     
+000243d0: 2020 2066 6967 7369 7a65 3d66 6967 7369     figsize=figsi
+000243e0: 7a65 2c0a 2020 2020 2020 2020 6e75 6d3d  ze,.        num=
+000243f0: 2746 6974 7465 6420 7265 6c61 7861 7469  'Fitted relaxati
+00024400: 6f6e 2070 726f 6669 6c65 270a 2020 2020  on profile'.    
+00024410: 290a 0a20 2020 205f 706c 6f74 5f66 6974  )..    _plot_fit
+00024420: 7465 645f 7261 7465 7328 6461 7461 7365  ted_rates(datase
+00024430: 742c 206d 6f64 656c 2c20 6669 672c 2061  t, model, fig, a
+00024440: 782c 2073 686f 775f 7061 7261 6d73 3d73  x, show_params=s
+00024450: 686f 775f 7061 7261 6d73 290a 0a20 2020  how_params)..   
+00024460: 2066 6967 2e74 6967 6874 5f6c 6179 6f75   fig.tight_layou
+00024470: 7428 290a 0a20 2020 2077 6172 6e69 6e67  t()..    warning
+00024480: 732e 7369 6d70 6c65 6669 6c74 6572 2827  s.simplefilter('
+00024490: 6967 6e6f 7265 272c 2055 7365 7257 6172  ignore', UserWar
+000244a0: 6e69 6e67 290a 2020 2020 6966 2073 686f  ning).    if sho
+000244b0: 773a 0a20 2020 2020 2020 2070 6c74 2e73  w:.        plt.s
+000244c0: 686f 7728 290a 0a20 2020 2069 6620 7361  how()..    if sa
+000244d0: 7665 3a0a 2020 2020 2020 2020 6669 672e  ve:.        fig.
+000244e0: 7361 7665 6669 6728 7361 7665 5f6e 616d  savefig(save_nam
+000244f0: 652c 2064 7069 3d35 3030 290a 2020 2020  e, dpi=500).    
+00024500: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
+00024510: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00024520: 7369 6e73 7461 6e63 6528 6461 7461 7365  sinstance(datase
+00024530: 742c 2028 5461 7554 4461 7461 7365 7429  t, (TauTDataset)
+00024540: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00024550: 2020 205f 7876 6172 203d 2027 5427 0a20     _xvar = 'T'. 
+00024560: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00024570: 6973 696e 7374 616e 6365 2864 6174 6173  isinstance(datas
+00024580: 6574 2c20 2854 6175 4844 6174 6173 6574  et, (TauHDataset
+00024590: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+000245a0: 2020 2020 5f78 7661 7220 3d20 2748 270a      _xvar = 'H'.
+000245b0: 2020 2020 2020 2020 2020 2020 7574 2e63              ut.c
+000245c0: 7072 696e 7428 0a20 2020 2020 2020 2020  print(.         
+000245d0: 2020 2020 2020 2066 275c 6e20 4669 7474         f'\n Fitt
+000245e0: 6564 20cf 84e2 81bb c2b9 2076 7320 7b5f  ed ....... vs {_
+000245f0: 7876 6172 7d20 706c 6f74 2073 6176 6564  xvar} plot saved
+00024600: 2074 6f20 5c6e 207b 7361 7665 5f6e 616d   to \n {save_nam
+00024610: 657d 5c6e 272c 0a20 2020 2020 2020 2020  e}\n',.         
+00024620: 2020 2020 2020 2027 6379 616e 270a 2020         'cyan'.  
+00024630: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00024640: 7761 726e 696e 6773 2e73 696d 706c 6566  warnings.simplef
+00024650: 696c 7465 7228 2764 6566 6175 6c74 272c  ilter('default',
+00024660: 2055 7365 7257 6172 6e69 6e67 290a 0a20   UserWarning).. 
+00024670: 2020 2072 6574 7572 6e20 6669 672c 2061     return fig, a
+00024680: 780a 0a0a 6465 6620 7174 5f70 6c6f 745f  x...def qt_plot_
+00024690: 6669 7474 6564 5f72 6174 6573 2861 7070  fitted_rates(app
+000246a0: 3a20 5174 5769 6467 6574 732e 5141 7070  : QtWidgets.QApp
+000246b0: 6c69 6361 7469 6f6e 2c0a 2020 2020 2020  lication,.      
+000246c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000246d0: 2020 2064 6174 6173 6574 3a20 5461 7554     dataset: TauT
+000246e0: 4461 7461 7365 7420 7c20 5461 7548 4461  Dataset | TauHDa
+000246f0: 7461 7365 742c 0a20 2020 2020 2020 2020  taset,.         
+00024700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024710: 6d6f 6465 6c3a 204c 6f67 5461 7554 4d6f  model: LogTauTMo
+00024720: 6465 6c20 7c20 4d75 6c74 694c 6f67 5461  del | MultiLogTa
+00024730: 7554 4d6f 6465 6c20 7c20 4c6f 6754 6175  uTModel | LogTau
+00024740: 484d 6f64 656c 207c 204d 756c 7469 4c6f  HModel | MultiLo
+00024750: 6754 6175 484d 6f64 656c 2c20 2320 6e6f  gTauHModel, # no
+00024760: 7161 0a20 2020 2020 2020 2020 2020 2020  qa.             
+00024770: 2020 2020 2020 2020 2020 2020 7361 7665              save
+00024780: 3a20 626f 6f6c 203d 2046 616c 7365 2c20  : bool = False, 
+00024790: 7368 6f77 3a20 626f 6f6c 203d 2054 7275  show: bool = Tru
+000247a0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+000247b0: 2020 2020 2020 2020 2020 2020 7361 7665              save
+000247c0: 5f6e 616d 653a 2073 7472 203d 2027 6669  _name: str = 'fi
+000247d0: 7474 6564 5f72 6174 6573 2e70 6e67 272c  tted_rates.png',
+000247e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000247f0: 2020 2020 2020 2020 2020 7665 7262 6f73            verbos
+00024800: 653a 2062 6f6f 6c20 3d20 5472 7565 2c0a  e: bool = True,.
 00024810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024820: 2020 2020 2073 686f 775f 7061 7261 6d73       show_params
-00024830: 3a20 626f 6f6c 203d 2054 7275 6529 202d  : bool = True) -
-00024840: 3e20 4e6f 6e65 3a0a 2020 2020 2727 270a  > None:.    '''.
-00024850: 2020 2020 506c 6f74 7320 6578 7065 7269      Plots experi
-00024860: 6d65 6e74 616c 2061 6e64 2066 6974 7465  mental and fitte
-00024870: 6420 286d 6f64 656c 2920 7265 6c61 7861  d (model) relaxa
-00024880: 7469 6f6e 2072 6174 6520 6173 5c6e 0a20  tion rate as\n. 
-00024890: 2020 2072 6174 6520 7673 2078 7661 7220     rate vs xvar 
-000248a0: 7768 6572 6520 7876 6172 2069 7320 5420  where xvar is T 
-000248b0: 6f72 2048 2e20 5769 7468 206c 6f67 206c  or H. With log l
-000248c0: 6f67 2073 6361 6c65 2e0a 0a20 2020 2050  og scale...    P
-000248d0: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
-000248e0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064 6174  --------.    dat
-000248f0: 6173 6574 3a20 5461 7554 4461 7461 7365  aset: TauTDatase
-00024900: 7420 7c20 5461 7548 4461 7461 7365 740a  t | TauHDataset.
-00024910: 2020 2020 2020 2020 4461 7461 7365 7420          Dataset 
-00024920: 746f 2070 6c6f 740a 2020 2020 6d6f 6465  to plot.    mode
-00024930: 6c3a 204c 6f67 5461 7554 4d6f 6465 6c20  l: LogTauTModel 
-00024940: 7c20 4d75 6c74 694c 6f67 5461 7554 4d6f  | MultiLogTauTMo
-00024950: 6465 6c20 7c20 4c6f 6754 6175 484d 6f64  del | LogTauHMod
-00024960: 656c 207c 204d 756c 7469 4c6f 6754 6175  el | MultiLogTau
-00024970: 484d 6f64 656c 0a20 2020 2020 2020 204d  HModel.        M
-00024980: 6f64 656c 2028 6669 7474 6564 2920 746f  odel (fitted) to
-00024990: 2070 6c6f 740a 2020 2020 7368 6f77 3a20   plot.    show: 
-000249a0: 626f 6f6c 2c20 6465 6661 756c 7420 5472  bool, default Tr
-000249b0: 7565 0a20 2020 2020 2020 2049 6620 5472  ue.        If Tr
-000249c0: 7565 2c20 7368 6f77 2070 6c6f 7420 6f6e  ue, show plot on
-000249d0: 2073 6372 6565 6e0a 2020 2020 7361 7665   screen.    save
-000249e0: 3a20 626f 6f6c 2c20 6465 6661 756c 7420  : bool, default 
-000249f0: 4661 6c73 650a 2020 2020 2020 2020 4966  False.        If
-00024a00: 2054 7275 652c 2073 6176 6520 706c 6f74   True, save plot
-00024a10: 2074 6f20 6669 6c65 2060 7361 7665 5f6e   to file `save_n
-00024a20: 616d 6560 0a20 2020 2073 6176 655f 6e61  ame`.    save_na
-00024a30: 6d65 3a20 7374 722c 2064 6566 6175 6c74  me: str, default
-00024a40: 2027 6669 7474 6564 5f72 6174 6573 2e70   'fitted_rates.p
-00024a50: 6e67 270a 2020 2020 2020 2020 4966 2073  ng'.        If s
-00024a60: 6176 6520 6973 2054 7275 652c 2077 696c  ave is True, wil
-00024a70: 6c20 7361 7665 2070 6c6f 7420 746f 2074  l save plot to t
-00024a80: 6869 7320 6669 6c65 6e61 6d65 0a20 2020  his filename.   
-00024a90: 2076 6572 626f 7365 3a20 626f 6f6c 2c20   verbose: bool, 
-00024aa0: 6465 6661 756c 7420 5472 7565 0a20 2020  default True.   
-00024ab0: 2020 2020 2049 6620 5472 7565 2c20 706c       If True, pl
-00024ac0: 6f74 2066 696c 6520 6c6f 6361 7469 6f6e  ot file location
-00024ad0: 2069 7320 7772 6974 7465 6e20 746f 2074   is written to t
-00024ae0: 6572 6d69 6e61 6c0a 2020 2020 7368 6f77  erminal.    show
-00024af0: 5f70 6172 616d 733a 2062 6f6f 6c2c 2064  _params: bool, d
-00024b00: 6566 6175 6c74 2054 7275 650a 2020 2020  efault True.    
-00024b10: 2020 2020 4966 2054 7275 652c 2073 686f      If True, sho
-00024b20: 7773 2066 6974 7465 6420 7061 7261 6d65  ws fitted parame
-00024b30: 7465 7273 206f 6e20 706c 6f74 0a0a 2020  ters on plot..  
-00024b40: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
-00024b50: 2d2d 2d2d 2d0a 2020 2020 4e6f 6e65 0a20  -----.    None. 
-00024b60: 2020 2027 2727 0a0a 2020 2020 7769 6e64     '''..    wind
-00024b70: 6f77 203d 2067 7569 2e4d 6174 706c 6f74  ow = gui.Matplot
-00024b80: 6c69 6257 696e 646f 7728 290a 0a20 2020  libWindow()..   
-00024b90: 2077 696e 646f 772e 7365 7457 696e 646f   window.setWindo
-00024ba0: 7754 6974 6c65 2827 4669 7474 6564 2072  wTitle('Fitted r
-00024bb0: 656c 6178 6174 696f 6e20 7072 6f66 696c  elaxation profil
-00024bc0: 6527 290a 0a20 2020 2023 2041 6464 2070  e')..    # Add p
-00024bd0: 6c6f 740a 2020 2020 5f70 6c6f 745f 6669  lot.    _plot_fi
-00024be0: 7474 6564 5f72 6174 6573 280a 2020 2020  tted_rates(.    
-00024bf0: 2020 2020 6461 7461 7365 742c 206d 6f64      dataset, mod
-00024c00: 656c 2c20 7769 6e64 6f77 2e73 632e 6669  el, window.sc.fi
-00024c10: 672c 2077 696e 646f 772e 7363 2e61 782c  g, window.sc.ax,
-00024c20: 2073 686f 775f 7061 7261 6d73 3d73 686f   show_params=sho
-00024c30: 775f 7061 7261 6d73 0a20 2020 2029 0a0a  w_params.    )..
-00024c40: 2020 2020 7761 726e 696e 6773 2e73 696d      warnings.sim
-00024c50: 706c 6566 696c 7465 7228 2769 676e 6f72  plefilter('ignor
-00024c60: 6527 2c20 5573 6572 5761 726e 696e 6729  e', UserWarning)
-00024c70: 0a20 2020 2023 2053 6176 6520 706c 6f74  .    # Save plot
-00024c80: 0a20 2020 2069 6620 7361 7665 3a0a 2020  .    if save:.  
-00024c90: 2020 2020 2020 7769 6e64 6f77 2e73 632e        window.sc.
-00024ca0: 6669 672e 7361 7665 6669 6728 7361 7665  fig.savefig(save
-00024cb0: 5f6e 616d 652c 2064 7069 3d33 3030 290a  _name, dpi=300).
-00024cc0: 2020 2020 2020 2020 6966 2076 6572 626f          if verbo
-00024cd0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00024ce0: 6966 2069 7369 6e73 7461 6e63 6528 6461  if isinstance(da
-00024cf0: 7461 7365 742c 2028 5461 7554 4461 7461  taset, (TauTData
-00024d00: 7365 7429 293a 0a20 2020 2020 2020 2020  set)):.         
-00024d10: 2020 2020 2020 205f 7876 6172 203d 2027         _xvar = '
-00024d20: 5427 0a20 2020 2020 2020 2020 2020 2065  T'.            e
-00024d30: 6c69 6620 6973 696e 7374 616e 6365 2864  lif isinstance(d
-00024d40: 6174 6173 6574 2c20 2854 6175 4844 6174  ataset, (TauHDat
-00024d50: 6173 6574 2929 3a0a 2020 2020 2020 2020  aset)):.        
-00024d60: 2020 2020 2020 2020 5f78 7661 7220 3d20          _xvar = 
-00024d70: 2748 270a 2020 2020 2020 2020 2020 2020  'H'.            
-00024d80: 7574 2e63 7072 696e 7428 0a20 2020 2020  ut.cprint(.     
-00024d90: 2020 2020 2020 2020 2020 2066 275c 6e20             f'\n 
-00024da0: 4669 7474 6564 20cf 84e2 81bb c2b9 2076  Fitted ....... v
-00024db0: 7320 7b5f 7876 6172 7d20 706c 6f74 2073  s {_xvar} plot s
-00024dc0: 6176 6564 2074 6f20 5c6e 207b 7361 7665  aved to \n {save
-00024dd0: 5f6e 616d 657d 5c6e 272c 0a20 2020 2020  _name}\n',.     
-00024de0: 2020 2020 2020 2020 2020 2027 6379 616e             'cyan
-00024df0: 270a 2020 2020 2020 2020 2020 2020 290a  '.            ).
-00024e00: 0a20 2020 2069 6620 7368 6f77 3a0a 2020  .    if show:.  
-00024e10: 2020 2020 2020 7769 6e64 6f77 2e73 686f        window.sho
-00024e20: 7728 290a 2020 2020 2020 2020 2320 4361  w().        # Ca
-00024e30: 6c6c 2074 7769 6365 2065 6c73 6520 6974  ll twice else it
-00024e40: 2077 6f6e 7420 776f 726b 210a 2020 2020   wont work!.    
-00024e50: 2020 2020 7769 6e64 6f77 2e73 632e 6669      window.sc.fi
-00024e60: 672e 7469 6768 745f 6c61 796f 7574 2829  g.tight_layout()
-00024e70: 0a20 2020 2020 2020 2077 696e 646f 772e  .        window.
-00024e80: 7363 2e66 6967 2e74 6967 6874 5f6c 6179  sc.fig.tight_lay
-00024e90: 6f75 7428 290a 2020 2020 2020 2020 6170  out().        ap
-00024ea0: 702e 6578 6563 5f28 290a 0a20 2020 2077  p.exec_()..    w
-00024eb0: 6172 6e69 6e67 732e 7369 6d70 6c65 6669  arnings.simplefi
-00024ec0: 6c74 6572 2827 6465 6661 756c 7427 2c20  lter('default', 
-00024ed0: 5573 6572 5761 726e 696e 6729 0a0a 2020  UserWarning)..  
-00024ee0: 2020 7265 7475 726e 0a0a 0a64 6566 205f    return...def _
-00024ef0: 706c 6f74 5f66 6974 7465 645f 7261 7465  plot_fitted_rate
-00024f00: 7328 6461 7461 7365 743a 2054 6175 5444  s(dataset: TauTD
-00024f10: 6174 6173 6574 207c 2054 6175 4844 6174  ataset | TauHDat
-00024f20: 6173 6574 2c0a 2020 2020 2020 2020 2020  aset,.          
-00024f30: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
-00024f40: 656c 3a20 4c6f 6754 6175 544d 6f64 656c  el: LogTauTModel
-00024f50: 207c 204d 756c 7469 4c6f 6754 6175 544d   | MultiLogTauTM
-00024f60: 6f64 656c 207c 204c 6f67 5461 7548 4d6f  odel | LogTauHMo
-00024f70: 6465 6c20 7c20 4d75 6c74 694c 6f67 5461  del | MultiLogTa
-00024f80: 7548 4d6f 6465 6c2c 2023 206e 6f71 610a  uHModel, # noqa.
-00024f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024fa0: 2020 2020 2020 2066 6967 3a20 706c 742e         fig: plt.
-00024fb0: 4669 6775 7265 2c20 6178 3a20 706c 742e  Figure, ax: plt.
-00024fc0: 4178 6573 2c0a 2020 2020 2020 2020 2020  Axes,.          
-00024fd0: 2020 2020 2020 2020 2020 2020 2073 686f               sho
-00024fe0: 775f 7061 7261 6d73 3a20 626f 6f6c 203d  w_params: bool =
-00024ff0: 2054 7275 6529 3a0a 2020 2020 2727 270a   True):.    '''.
-00025000: 2020 2020 506c 6f74 7320 6578 7065 7269      Plots experi
-00025010: 6d65 6e74 616c 2061 6e64 2066 6974 7465  mental and fitte
-00025020: 6420 286d 6f64 656c 2920 7265 6c61 7861  d (model) relaxa
-00025030: 7469 6f6e 2072 6174 6520 6173 5c6e 0a20  tion rate as\n. 
-00025040: 2020 2072 6174 6520 7673 2078 7661 7220     rate vs xvar 
-00025050: 7768 6572 6520 7876 6172 2069 7320 5420  where xvar is T 
-00025060: 6f72 2048 2e20 5769 7468 206c 6f67 206c  or H. With log l
-00025070: 6f67 2073 6361 6c65 2e0a 0a20 2020 2050  og scale...    P
-00025080: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
-00025090: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064 6174  --------.    dat
-000250a0: 6173 6574 3a20 5461 7554 4461 7461 7365  aset: TauTDatase
-000250b0: 7420 7c20 5461 7548 4461 7461 7365 740a  t | TauHDataset.
-000250c0: 2020 2020 2020 2020 4461 7461 7365 7420          Dataset 
-000250d0: 746f 2070 6c6f 740a 2020 2020 6d6f 6465  to plot.    mode
-000250e0: 6c3a 204c 6f67 5461 7554 4d6f 6465 6c20  l: LogTauTModel 
-000250f0: 7c20 4d75 6c74 694c 6f67 5461 7554 4d6f  | MultiLogTauTMo
-00025100: 6465 6c20 7c20 4c6f 6754 6175 484d 6f64  del | LogTauHMod
-00025110: 656c 207c 204d 756c 7469 4c6f 6754 6175  el | MultiLogTau
-00025120: 484d 6f64 656c 0a20 2020 2020 2020 204d  HModel.        M
-00025130: 6f64 656c 2028 6669 7474 6564 2920 746f  odel (fitted) to
-00025140: 2070 6c6f 740a 2020 2020 6669 673a 2070   plot.    fig: p
-00025150: 6c74 2e46 6967 7572 650a 2020 2020 2020  lt.Figure.      
-00025160: 2020 4d61 7470 6c6f 746c 6962 2046 6967    Matplotlib Fig
-00025170: 7572 6520 6f62 6a65 6374 2075 7365 6420  ure object used 
-00025180: 666f 7220 706c 6f74 0a20 2020 2061 783a  for plot.    ax:
-00025190: 2070 6c74 2e41 7865 730a 2020 2020 2020   plt.Axes.      
-000251a0: 2020 4d61 7470 6c6f 746c 6962 2041 7869    Matplotlib Axi
-000251b0: 7320 6f62 6a65 6374 2075 7365 6420 666f  s object used fo
-000251c0: 7220 706c 6f74 0a20 2020 2073 686f 775f  r plot.    show_
-000251d0: 7061 7261 6d73 3a20 626f 6f6c 2c20 6465  params: bool, de
-000251e0: 6661 756c 7420 5472 7565 0a20 2020 2020  fault True.     
-000251f0: 2020 2049 6620 5472 7565 2c20 7368 6f77     If True, show
-00025200: 7320 6669 7474 6564 2070 6172 616d 6574  s fitted paramet
-00025210: 6572 7320 6f6e 2070 6c6f 740a 0a20 2020  ers on plot..   
-00025220: 2052 6574 7572 6e73 0a20 2020 202d 2d2d   Returns.    ---
-00025230: 2d2d 2d2d 0a20 2020 204e 6f6e 650a 2020  ----.    None.  
-00025240: 2020 2727 270a 0a20 2020 2069 6620 6973    '''..    if is
-00025250: 696e 7374 616e 6365 2864 6174 6173 6574  instance(dataset
-00025260: 2c20 5461 7548 4461 7461 7365 7429 3a0a  , TauHDataset):.
-00025270: 2020 2020 2020 2020 785f 7661 6c73 203d          x_vals =
-00025280: 2063 6f70 792e 636f 7079 2864 6174 6173   copy.copy(datas
-00025290: 6574 2e66 6965 6c64 7329 0a20 2020 2020  et.fields).     
-000252a0: 2020 2078 5f74 7970 6520 3d20 2766 6965     x_type = 'fie
-000252b0: 6c64 270a 2020 2020 2020 2020 6178 2e73  ld'.        ax.s
-000252c0: 6574 5f78 6c61 6265 6c28 7227 4669 656c  et_xlabel(r'Fiel
-000252d0: 6420 284f 6529 2729 0a20 2020 2065 6c69  d (Oe)').    eli
-000252e0: 6620 6973 696e 7374 616e 6365 2864 6174  f isinstance(dat
-000252f0: 6173 6574 2c20 5461 7554 4461 7461 7365  aset, TauTDatase
-00025300: 7429 3a0a 2020 2020 2020 2020 785f 7661  t):.        x_va
-00025310: 6c73 203d 2063 6f70 792e 636f 7079 2864  ls = copy.copy(d
-00025320: 6174 6173 6574 2e74 656d 7065 7261 7475  ataset.temperatu
-00025330: 7265 7329 0a20 2020 2020 2020 2078 5f74  res).        x_t
-00025340: 7970 6520 3d20 2774 656d 7065 7261 7475  ype = 'temperatu
-00025350: 7265 270a 2020 2020 2020 2020 6178 2e73  re'.        ax.s
-00025360: 6574 5f78 6c61 6265 6c28 7227 5465 6d70  et_xlabel(r'Temp
-00025370: 6572 6174 7572 6520 284b 2927 290a 0a20  erature (K)').. 
-00025380: 2020 2023 2041 6464 2075 6e63 6572 7461     # Add uncerta
-00025390: 696e 7469 6573 2061 7320 6572 726f 7262  inties as errorb
-000253a0: 6172 730a 2020 2020 6966 206c 656e 2864  ars.    if len(d
-000253b0: 6174 6173 6574 2e72 6174 655f 706d 293a  ataset.rate_pm):
-000253c0: 0a20 2020 2020 2020 2061 782e 6572 726f  .        ax.erro
-000253d0: 7262 6172 280a 2020 2020 2020 2020 2020  rbar(.          
-000253e0: 2020 785f 7661 6c73 2c0a 2020 2020 2020    x_vals,.      
-000253f0: 2020 2020 2020 6461 7461 7365 742e 7261        dataset.ra
-00025400: 7465 732c 0a20 2020 2020 2020 2020 2020  tes,.           
-00025410: 2079 6572 723d 6461 7461 7365 742e 7261   yerr=dataset.ra
-00025420: 7465 5f70 6d2c 0a20 2020 2020 2020 2020  te_pm,.         
-00025430: 2020 206d 6172 6b65 723d 276f 272c 0a20     marker='o',. 
-00025440: 2020 2020 2020 2020 2020 206c 773d 302c             lw=0,
-00025450: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-00025460: 6e65 7769 6474 683d 312e 352c 0a20 2020  newidth=1.5,.   
-00025470: 2020 2020 2020 2020 2066 696c 6c73 7479           fillsty
-00025480: 6c65 3d27 6e6f 6e65 272c 0a20 2020 2020  le='none',.     
-00025490: 2020 2020 2020 206c 6162 656c 3d27 4578         label='Ex
-000254a0: 7065 7269 6d65 6e74 272c 0a20 2020 2020  periment',.     
-000254b0: 2020 2020 2020 2063 6f6c 6f72 3d27 626c         color='bl
-000254c0: 6163 6b27 0a20 2020 2020 2020 2029 0a20  ack'.        ). 
-000254d0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000254e0: 2061 782e 706c 6f74 280a 2020 2020 2020   ax.plot(.      
-000254f0: 2020 2020 2020 785f 7661 6c73 2c0a 2020        x_vals,.  
-00025500: 2020 2020 2020 2020 2020 6461 7461 7365            datase
-00025510: 742e 7261 7465 732c 0a20 2020 2020 2020  t.rates,.       
-00025520: 2020 2020 206d 6172 6b65 723d 276f 272c       marker='o',
-00025530: 0a20 2020 2020 2020 2020 2020 206c 773d  .            lw=
-00025540: 302c 0a20 2020 2020 2020 2020 2020 2066  0,.            f
-00025550: 696c 6c73 7479 6c65 3d27 6e6f 6e65 272c  illstyle='none',
-00025560: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
-00025570: 656c 3d27 4578 7065 7269 6d65 6e74 272c  el='Experiment',
-00025580: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
-00025590: 6f72 3d27 626c 6163 6b27 0a20 2020 2020  or='black'.     
-000255a0: 2020 2029 0a0a 2020 2020 785f 7661 7273     )..    x_vars
-000255b0: 5f67 7269 6420 3d20 6e70 2e6c 696e 7370  _grid = np.linsp
-000255c0: 6163 6528 0a20 2020 2020 2020 206e 702e  ace(.        np.
-000255d0: 6d69 6e28 785f 7661 6c73 292c 0a20 2020  min(x_vals),.   
-000255e0: 2020 2020 206e 702e 6d61 7828 785f 7661       np.max(x_va
-000255f0: 6c73 292c 0a20 2020 2020 2020 2035 3030  ls),.        500
-00025600: 300a 2020 2020 290a 0a20 2020 2069 6620  0.    )..    if 
-00025610: 7479 7065 286d 6f64 656c 2920 696e 205b  type(model) in [
-00025620: 4d75 6c74 694c 6f67 5461 7554 4d6f 6465  MultiLogTauTMode
-00025630: 6c2c 204d 756c 7469 4c6f 6754 6175 484d  l, MultiLogTauHM
-00025640: 6f64 656c 5d3a 0a20 2020 2020 2020 206c  odel]:.        l
-00025650: 6f67 6d6f 6465 6c73 203d 206d 6f64 656c  ogmodels = model
-00025660: 2e6c 6f67 6d6f 6465 6c73 0a20 2020 2065  .logmodels.    e
-00025670: 6c73 653a 0a20 2020 2020 2020 206c 6f67  lse:.        log
-00025680: 6d6f 6465 6c73 203d 205b 6d6f 6465 6c5d  models = [model]
-00025690: 0a0a 2020 2020 666f 7220 6c6f 676d 6f64  ..    for logmod
-000256a0: 656c 2069 6e20 6c6f 676d 6f64 656c 733a  el in logmodels:
-000256b0: 0a0a 2020 2020 2020 2020 6966 2074 7970  ..        if typ
-000256c0: 6528 6c6f 676d 6f64 656c 2920 6973 204c  e(logmodel) is L
-000256d0: 6f67 4f72 6261 6368 4d6f 6465 6c3a 0a20  ogOrbachModel:. 
-000256e0: 2020 2020 2020 2020 2020 206c 6162 656c             label
-000256f0: 5f66 6974 203d 2027 5c6e 4669 7420 7769  _fit = '\nFit wi
-00025700: 7468 270a 2020 2020 2020 2020 2020 2020  th'.            
-00025710: 6c61 6265 6c5f 6669 7420 2b3d 2027 5c6e  label_fit += '\n
-00025720: 2720 2b20 7227 7b7d 207b 3a36 2e32 667d  ' + r'{} {:6.2f}
-00025730: 2073 272e 666f 726d 6174 280a 2020 2020   s'.format(.    
-00025740: 2020 2020 2020 2020 2020 2020 6c6f 676d              logm
-00025750: 6f64 656c 2e56 4152 4e41 4d45 535f 4d4d  odel.VARNAMES_MM
-00025760: 5b27 755f 6566 6627 5d2c 0a20 2020 2020  ['u_eff'],.     
-00025770: 2020 2020 2020 2020 2020 206c 6f67 6d6f             logmo
-00025780: 6465 6c2e 6669 6e61 6c5f 7661 725f 7661  del.final_var_va
-00025790: 6c75 6573 5b27 755f 6566 6627 5d0a 2020  lues['u_eff'].  
-000257a0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-000257b0: 2020 2020 2020 2020 6c61 6265 6c5f 6669          label_fi
-000257c0: 7420 2b3d 2027 5c6e 2720 2b20 7227 7b7d  t += '\n' + r'{}
-000257d0: 207b 3a30 342e 3365 7d27 2e66 6f72 6d61   {:04.3e}'.forma
-000257e0: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-000257f0: 2020 206c 6f67 6d6f 6465 6c2e 5641 524e     logmodel.VARN
-00025800: 414d 4553 5f4d 4d5b 2741 275d 2c20 6c6f  AMES_MM['A'], lo
-00025810: 676d 6f64 656c 2e66 696e 616c 5f76 6172  gmodel.final_var
-00025820: 5f76 616c 7565 735b 2741 275d 0a20 2020  _values['A'].   
-00025830: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00025840: 2020 2065 6c69 6620 7479 7065 286c 6f67     elif type(log
-00025850: 6d6f 6465 6c29 2069 7320 4c6f 6752 616d  model) is LogRam
-00025860: 616e 4d6f 6465 6c3a 0a20 2020 2020 2020  anModel:.       
-00025870: 2020 2020 206c 6162 656c 5f66 6974 203d       label_fit =
-00025880: 2027 5c6e 4669 7420 7769 7468 270a 2020   '\nFit with'.  
-00025890: 2020 2020 2020 2020 2020 6c61 6265 6c5f            label_
-000258a0: 6669 7420 2b3d 2027 5c6e 2720 2b20 7227  fit += '\n' + r'
-000258b0: 7b7d 207b 3a36 2e32 667d 2073 272e 666f  {} {:6.2f} s'.fo
-000258c0: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
-000258d0: 2020 2020 2020 6c6f 676d 6f64 656c 2e56        logmodel.V
-000258e0: 4152 4e41 4d45 535f 4d4d 5b27 5227 5d2c  ARNAMES_MM['R'],
-000258f0: 206c 6f67 6d6f 6465 6c2e 6669 6e61 6c5f   logmodel.final_
-00025900: 7661 725f 7661 6c75 6573 5b27 5227 5d0a  var_values['R'].
-00025910: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00025920: 2020 2020 2020 2020 2020 6c61 6265 6c5f            label_
-00025930: 6669 7420 2b3d 2027 5c6e 2720 2b20 7227  fit += '\n' + r'
-00025940: 7b7d 207b 3a30 342e 3365 7d27 2e66 6f72  {} {:04.3e}'.for
-00025950: 6d61 7428 0a20 2020 2020 2020 2020 2020  mat(.           
-00025960: 2020 2020 206c 6f67 6d6f 6465 6c2e 5641       logmodel.VA
-00025970: 524e 414d 4553 5f4d 4d5b 276e 275d 2c20  RNAMES_MM['n'], 
-00025980: 6c6f 676d 6f64 656c 2e66 696e 616c 5f76  logmodel.final_v
-00025990: 6172 5f76 616c 7565 735b 276e 275d 0a20  ar_values['n']. 
-000259a0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-000259b0: 2020 2020 2065 6c69 6620 7479 7065 286c       elif type(l
-000259c0: 6f67 6d6f 6465 6c29 2069 7320 4c6f 6751  ogmodel) is LogQ
-000259d0: 544d 4d6f 6465 6c3a 0a20 2020 2020 2020  TMModel:.       
-000259e0: 2020 2020 206c 6162 656c 5f66 6974 203d       label_fit =
-000259f0: 2027 5c6e 4669 7420 7769 7468 270a 2020   '\nFit with'.  
-00025a00: 2020 2020 2020 2020 2020 6c61 6265 6c5f            label_
-00025a10: 6669 7420 2b3d 2027 5c6e 2720 2b20 7227  fit += '\n' + r'
-00025a20: 7b7d 207b 3a36 2e32 667d 2073 272e 666f  {} {:6.2f} s'.fo
-00025a30: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
-00025a40: 2020 2020 2020 6c6f 676d 6f64 656c 2e56        logmodel.V
-00025a50: 4152 4e41 4d45 535f 4d4d 5b27 5127 5d2c  ARNAMES_MM['Q'],
-00025a60: 206c 6f67 6d6f 6465 6c2e 6669 6e61 6c5f   logmodel.final_
-00025a70: 7661 725f 7661 6c75 6573 5b27 5127 5d0a  var_values['Q'].
-00025a80: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00025a90: 2020 2020 2020 656c 6966 2074 7970 6528        elif type(
-00025aa0: 6c6f 676d 6f64 656c 2920 6973 204c 6f67  logmodel) is Log
-00025ab0: 4469 7265 6374 4d6f 6465 6c3a 0a20 2020  DirectModel:.   
-00025ac0: 2020 2020 2020 2020 206c 6162 656c 5f66           label_f
-00025ad0: 6974 203d 2027 5c6e 4669 7420 7769 7468  it = '\nFit with
-00025ae0: 270a 2020 2020 2020 2020 2020 2020 6c61  '.            la
-00025af0: 6265 6c5f 6669 7420 2b3d 2027 5c6e 2720  bel_fit += '\n' 
-00025b00: 2b20 7227 7b7d 207b 3a36 2e32 667d 2073  + r'{} {:6.2f} s
-00025b10: 272e 666f 726d 6174 280a 2020 2020 2020  '.format(.      
-00025b20: 2020 2020 2020 2020 2020 6c6f 676d 6f64            logmod
-00025b30: 656c 2e56 4152 4e41 4d45 535f 4d4d 5b27  el.VARNAMES_MM['
-00025b40: 4427 5d2c 206c 6f67 6d6f 6465 6c2e 6669  D'], logmodel.fi
-00025b50: 6e61 6c5f 7661 725f 7661 6c75 6573 5b27  nal_var_values['
-00025b60: 4427 5d0a 2020 2020 2020 2020 2020 2020  D'].            
-00025b70: 290a 2020 2020 2020 2020 6d6f 6465 6c5f  ).        model_
-00025b80: 7261 7465 7320 3d20 3130 2a2a 6c6f 676d  rates = 10**logm
-00025b90: 6f64 656c 2e6d 6f64 656c 280a 2020 2020  odel.model(.    
-00025ba0: 2020 2020 2020 2020 6c6f 676d 6f64 656c          logmodel
-00025bb0: 2e66 696e 616c 5f76 6172 5f76 616c 7565  .final_var_value
-00025bc0: 732c 0a20 2020 2020 2020 2020 2020 2078  s,.            x
-00025bd0: 5f76 6172 735f 6772 6964 2c0a 2020 2020  _vars_grid,.    
-00025be0: 2020 2020 290a 0a20 2020 2020 2020 2061      )..        a
-00025bf0: 782e 706c 6f74 280a 2020 2020 2020 2020  x.plot(.        
-00025c00: 2020 2020 6e70 2e61 7272 6179 2878 5f76      np.array(x_v
-00025c10: 6172 735f 6772 6964 292c 0a20 2020 2020  ars_grid),.     
-00025c20: 2020 2020 2020 206e 702e 6172 7261 7928         np.array(
-00025c30: 6d6f 6465 6c5f 7261 7465 7329 2c0a 2020  model_rates),.  
-00025c40: 2020 2020 2020 2020 2020 6c77 3d31 2e35            lw=1.5
-00025c50: 2c0a 2020 2020 2020 2020 2020 2020 6c61  ,.            la
-00025c60: 6265 6c3d 6c6f 676d 6f64 656c 2e4e 414d  bel=logmodel.NAM
-00025c70: 452c 0a20 2020 2020 2020 2020 2020 206c  E,.            l
-00025c80: 733d 272d 2d27 0a20 2020 2020 2020 2029  s='--'.        )
-00025c90: 0a0a 2020 2020 6966 2074 7970 6528 6d6f  ..    if type(mo
-00025ca0: 6465 6c29 2069 6e20 5b4d 756c 7469 4c6f  del) in [MultiLo
-00025cb0: 6754 6175 544d 6f64 656c 2c20 4d75 6c74  gTauTModel, Mult
-00025cc0: 694c 6f67 5461 7548 4d6f 6465 6c5d 2061  iLogTauHModel] a
-00025cd0: 6e64 206c 656e 286c 6f67 6d6f 6465 6c73  nd len(logmodels
-00025ce0: 2920 3e20 313a 2023 206e 6f71 610a 2020  ) > 1: # noqa.  
-00025cf0: 2020 2020 2020 746f 7461 6c20 3d20 6e70        total = np
-00025d00: 2e7a 6572 6f73 286c 656e 2878 5f76 6172  .zeros(len(x_var
-00025d10: 735f 6772 6964 2929 0a0a 2020 2020 2020  s_grid))..      
-00025d20: 2020 666f 7220 6c6f 676d 6f64 656c 2069    for logmodel i
-00025d30: 6e20 6c6f 676d 6f64 656c 733a 0a20 2020  n logmodels:.   
-00025d40: 2020 2020 2020 2020 2074 6f74 616c 202b           total +
-00025d50: 3d20 3130 2a2a 6c6f 676d 6f64 656c 2e6d  = 10**logmodel.m
-00025d60: 6f64 656c 280a 2020 2020 2020 2020 2020  odel(.          
-00025d70: 2020 2020 2020 6c6f 676d 6f64 656c 2e66        logmodel.f
-00025d80: 696e 616c 5f76 6172 5f76 616c 7565 732c  inal_var_values,
-00025d90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00025da0: 2078 5f76 6172 735f 6772 6964 2c0a 2020   x_vars_grid,.  
-00025db0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-00025dc0: 2020 2020 2061 782e 706c 6f74 280a 2020       ax.plot(.  
-00025dd0: 2020 2020 2020 2020 2020 785f 7661 7273            x_vars
-00025de0: 5f67 7269 642c 0a20 2020 2020 2020 2020  _grid,.         
-00025df0: 2020 2074 6f74 616c 2c0a 2020 2020 2020     total,.      
-00025e00: 2020 2020 2020 6c77 3d31 2e35 2c0a 2020        lw=1.5,.  
-00025e10: 2020 2020 2020 2020 2020 6c61 6265 6c3d            label=
-00025e20: 2754 6f74 616c 272c 0a20 2020 2020 2020  'Total',.       
-00025e30: 2020 2020 2063 6f6c 6f72 3d27 7265 6427       color='red'
-00025e40: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-00025e50: 6966 2078 5f74 7970 6520 3d3d 2027 6669  if x_type == 'fi
-00025e60: 656c 6427 3a0a 2020 2020 2020 2020 6966  eld':.        if
-00025e70: 2061 6e79 2876 616c 203c 206e 702e 6669   any(val < np.fi
-00025e80: 6e66 6f28 666c 6f61 7429 2e65 7073 2066  nfo(float).eps f
-00025e90: 6f72 2076 616c 2069 6e20 785f 7661 6c73  or val in x_vals
-00025ea0: 293a 0a20 2020 2020 2020 2020 2020 2061  ):.            a
-00025eb0: 782e 7365 745f 7873 6361 6c65 280a 2020  x.set_xscale(.  
-00025ec0: 2020 2020 2020 2020 2020 2020 2020 2773                's
-00025ed0: 796d 6c6f 6727 2c0a 2020 2020 2020 2020  ymlog',.        
-00025ee0: 2020 2020 2020 2020 6c69 6e74 6872 6573          linthres
-00025ef0: 683d 6775 692e 6361 6c63 5f6c 696e 7468  h=gui.calc_linth
-00025f00: 7265 7368 2878 5f76 616c 7329 2c0a 2020  resh(x_vals),.  
-00025f10: 2020 2020 2020 2020 2020 2020 2020 6c69                li
-00025f20: 6e73 6361 6c65 3d67 7569 2e63 616c 635f  nscale=gui.calc_
-00025f30: 6c69 6e73 6361 6c65 2878 5f76 616c 7329  linscale(x_vals)
-00025f40: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00025f50: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00025f60: 2020 2020 2020 2020 2061 782e 7365 745f           ax.set_
-00025f70: 7873 6361 6c65 2827 6c6f 6727 290a 2020  xscale('log').  
-00025f80: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00025f90: 6178 2e73 6574 5f78 7363 616c 6528 276c  ax.set_xscale('l
-00025fa0: 6f67 2729 0a20 2020 2061 782e 7365 745f  og').    ax.set_
-00025fb0: 7973 6361 6c65 2827 6c6f 6727 290a 0a20  yscale('log').. 
-00025fc0: 2020 2067 7569 2e66 6f72 6d61 745f 7261     gui.format_ra
-00025fd0: 7465 5f78 5f79 5f61 7865 7328 0a20 2020  te_x_y_axes(.   
-00025fe0: 2020 2020 2061 782c 0a20 2020 2020 2020       ax,.       
-00025ff0: 2064 6174 6173 6574 2e72 6174 6573 2c0a   dataset.rates,.
-00026000: 2020 2020 2020 2020 785f 7661 6c73 2c0a          x_vals,.
-00026010: 2020 2020 2020 2020 6e70 2e61 6273 2864          np.abs(d
-00026020: 6174 6173 6574 2e72 6174 655f 706d 292c  ataset.rate_pm),
-00026030: 0a20 2020 2020 2020 2078 5f74 7970 653d  .        x_type=
-00026040: 785f 7479 7065 0a20 2020 2029 0a0a 2020  x_type.    )..  
-00026050: 2020 6578 7072 6573 7369 6f6e 203d 2027    expression = '
-00026060: 270a 0a20 2020 2066 6f72 206c 6f67 6d6f  '..    for logmo
-00026070: 6465 6c20 696e 206c 6f67 6d6f 6465 6c73  del in logmodels
-00026080: 3a0a 2020 2020 2020 2020 666f 7220 6974  :.        for it
-00026090: 2c20 6e61 6d65 2069 6e20 656e 756d 6572  , name in enumer
-000260a0: 6174 6528 6c6f 676d 6f64 656c 2e50 4152  ate(logmodel.PAR
-000260b0: 4e41 4d45 5329 3a0a 2020 2020 2020 2020  NAMES):.        
-000260c0: 2020 2020 6578 7072 6573 7369 6f6e 202b      expression +
-000260d0: 3d20 277b 7d20 3d20 7b3a 2e33 667d 2027  = '{} = {:.3f} '
-000260e0: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
-000260f0: 2020 2020 2020 2020 206c 6f67 6d6f 6465           logmode
-00026100: 6c2e 5641 524e 414d 4553 5f4d 4d5b 6e61  l.VARNAMES_MM[na
-00026110: 6d65 5d2c 0a20 2020 2020 2020 2020 2020  me],.           
-00026120: 2020 2020 206c 6f67 6d6f 6465 6c2e 6669       logmodel.fi
-00026130: 6e61 6c5f 7661 725f 7661 6c75 6573 5b6e  nal_var_values[n
-00026140: 616d 655d 2c0a 2020 2020 2020 2020 2020  ame],.          
-00026150: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00026160: 6966 206e 616d 6520 696e 206c 6f67 6d6f  if name in logmo
-00026170: 6465 6c2e 6669 745f 7661 7273 2e6b 6579  del.fit_vars.key
-00026180: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
-00026190: 2020 2020 2065 7870 7265 7373 696f 6e20       expression 
-000261a0: 2b3d 2072 2724 5c70 6d24 2027 0a20 2020  += r'$\pm$ '.   
-000261b0: 2020 2020 2020 2020 2020 2020 2065 7870               exp
-000261c0: 7265 7373 696f 6e20 2b3d 2027 7b3a 2e33  ression += '{:.3
-000261d0: 667d 2027 2e66 6f72 6d61 7428 6c6f 676d  f} '.format(logm
-000261e0: 6f64 656c 2e66 6974 5f73 7464 6576 5b6e  odel.fit_stdev[n
-000261f0: 616d 655d 290a 2020 2020 2020 2020 2020  ame]).          
-00026200: 2020 6578 7072 6573 7369 6f6e 202b 3d20    expression += 
-00026210: 277b 7d20 2020 2027 2e66 6f72 6d61 7428  '{}    '.format(
-00026220: 6c6f 676d 6f64 656c 2e55 4e49 5453 5f4d  logmodel.UNITS_M
-00026230: 4d5b 6e61 6d65 5d29 0a20 2020 2020 2020  M[name]).       
-00026240: 2020 2020 2069 6620 6974 203d 3d20 3120       if it == 1 
-00026250: 616e 6420 6c65 6e28 6c6f 676d 6f64 656c  and len(logmodel
-00026260: 2e66 6974 5f76 6172 732e 6b65 7973 2829  .fit_vars.keys()
-00026270: 2920 3e20 323a 0a20 2020 2020 2020 2020  ) > 2:.         
-00026280: 2020 2020 2020 2065 7870 7265 7373 696f         expressio
-00026290: 6e20 2b3d 2027 5c6e 270a 2020 2020 2020  n += '\n'.      
-000262a0: 2020 6578 7072 6573 7369 6f6e 202b 3d20    expression += 
-000262b0: 275c 6e27 0a0a 2020 2020 6966 2073 686f  '\n'..    if sho
-000262c0: 775f 7061 7261 6d73 3a0a 2020 2020 2020  w_params:.      
-000262d0: 2020 6178 2e74 6578 7428 0a20 2020 2020    ax.text(.     
-000262e0: 2020 2020 2020 2030 2e30 2c20 312e 3032         0.0, 1.02
-000262f0: 2c20 733d 6578 7072 6573 7369 6f6e 2c20  , s=expression, 
-00026300: 666f 6e74 7369 7a65 3d31 302c 2074 7261  fontsize=10, tra
-00026310: 6e73 666f 726d 3d61 782e 7472 616e 7341  nsform=ax.transA
-00026320: 7865 730a 2020 2020 2020 2020 290a 0a20  xes.        ).. 
-00026330: 2020 2069 6620 785f 7479 7065 203d 3d20     if x_type == 
-00026340: 2766 6965 6c64 273a 0a20 2020 2020 2020  'field':.       
-00026350: 2061 782e 6c65 6765 6e64 280a 2020 2020   ax.legend(.    
-00026360: 2020 2020 2020 2020 666f 6e74 7369 7a65          fontsize
-00026370: 3d27 3130 272c 206e 756d 706f 696e 7473  ='10', numpoints
-00026380: 3d31 2c20 6e63 6f6c 3d31 2c20 6672 616d  =1, ncol=1, fram
-00026390: 656f 6e3d 4661 6c73 650a 2020 2020 2020  eon=False.      
-000263a0: 2020 290a 2020 2020 656c 7365 3a0a 2020    ).    else:.  
-000263b0: 2020 2020 2020 6178 2e6c 6567 656e 6428        ax.legend(
-000263c0: 0a20 2020 2020 2020 2020 2020 206c 6f63  .            loc
-000263d0: 3d27 7570 7065 7220 6c65 6674 272c 2066  ='upper left', f
-000263e0: 6f6e 7473 697a 653d 2731 3027 2c20 6e75  ontsize='10', nu
-000263f0: 6d70 6f69 6e74 733d 312c 206e 636f 6c3d  mpoints=1, ncol=
-00026400: 312c 2066 7261 6d65 6f6e 3d46 616c 7365  1, frameon=False
-00026410: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-00026420: 6178 2e73 6574 5f79 6c61 6265 6c28 7227  ax.set_ylabel(r'
-00026430: 5261 7465 2028 7324 5e5c 6d61 7468 7265  Rate (s$^\mathre
-00026440: 6775 6c61 727b 2d31 7d24 2927 290a 0a20  gular{-1}$)').. 
-00026450: 2020 2072 6574 7572 6e0a 0a0a 6465 6620     return...def 
-00026460: 706c 6f74 5f72 6174 6573 2864 6174 6173  plot_rates(datas
-00026470: 6574 3a20 5461 7554 4461 7461 7365 7420  et: TauTDataset 
-00026480: 7c20 5461 7548 4461 7461 7365 742c 2073  | TauHDataset, s
-00026490: 686f 773a 2062 6f6f 6c20 3d20 5472 7565  how: bool = True
-000264a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000264b0: 2073 6176 653a 2062 6f6f 6c20 3d20 4661   save: bool = Fa
-000264c0: 6c73 652c 2073 6176 655f 6e61 6d65 3a20  lse, save_name: 
-000264d0: 7374 7220 3d20 2772 656c 6178 6174 696f  str = 'relaxatio
-000264e0: 6e5f 7261 7465 732e 706e 6727 2c0a 2020  n_rates.png',.  
-000264f0: 2020 2020 2020 2020 2020 2020 2076 6572               ver
-00026500: 626f 7365 3a20 626f 6f6c 203d 2054 7275  bose: bool = Tru
-00026510: 6529 202d 3e20 7475 706c 655b 706c 742e  e) -> tuple[plt.
-00026520: 4669 6775 7265 2c20 706c 742e 4178 6573  Figure, plt.Axes
-00026530: 5d3a 0a20 2020 2027 2727 0a20 2020 2050  ]:.    '''.    P
-00026540: 6c6f 7473 2065 7870 6572 696d 656e 7461  lots experimenta
-00026550: 6c20 7265 6c61 7861 7469 6f6e 2072 6174  l relaxation rat
-00026560: 6520 7673 2066 6965 6c64 2f74 656d 7065  e vs field/tempe
-00026570: 7261 7475 7265 2061 6e64 0a20 2020 2064  rature and.    d
-00026580: 6973 706c 6179 7320 6f6e 2073 6372 6565  isplays on scree
-00026590: 6e2e 0a0a 2020 2020 5061 7261 6d65 7465  n...    Paramete
-000265a0: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-000265b0: 2d0a 2020 2020 6461 7461 7365 743a 2054  -.    dataset: T
-000265c0: 6175 5444 6174 6173 6574 207c 2054 6175  auTDataset | Tau
-000265d0: 4844 6174 6173 6574 0a20 2020 2020 2020  HDataset.       
-000265e0: 2044 6174 6173 6574 2074 6f20 706c 6f74   Dataset to plot
-000265f0: 0a20 2020 2073 686f 773a 2062 6f6f 6c2c  .    show: bool,
-00026600: 2064 6566 6175 6c74 2054 7275 650a 2020   default True.  
-00026610: 2020 2020 2020 4966 2054 7275 652c 2073        If True, s
-00026620: 686f 7720 706c 6f74 206f 6e20 7363 7265  how plot on scre
-00026630: 656e 0a20 2020 2073 6176 653a 2062 6f6f  en.    save: boo
-00026640: 6c2c 2064 6566 6175 6c74 2046 616c 7365  l, default False
-00026650: 0a20 2020 2020 2020 2049 6620 5472 7565  .        If True
-00026660: 2c20 7361 7665 2070 6c6f 7420 746f 2066  , save plot to f
-00026670: 696c 6520 6073 6176 655f 6e61 6d65 600a  ile `save_name`.
-00026680: 2020 2020 7361 7665 5f6e 616d 653a 2073      save_name: s
-00026690: 7472 2c20 6465 6661 756c 7420 2772 656c  tr, default 'rel
-000266a0: 6178 6174 696f 6e5f 7261 7465 732e 706e  axation_rates.pn
-000266b0: 6727 0a20 2020 2020 2020 2049 6620 7361  g'.        If sa
-000266c0: 7665 2069 7320 5472 7565 2c20 7769 6c6c  ve is True, will
-000266d0: 2073 6176 6520 706c 6f74 2074 6f20 7468   save plot to th
-000266e0: 6973 2066 696c 656e 616d 650a 2020 2020  is filename.    
-000266f0: 7665 7262 6f73 653a 2062 6f6f 6c2c 2064  verbose: bool, d
-00026700: 6566 6175 6c74 2054 7275 650a 2020 2020  efault True.    
-00026710: 2020 2020 4966 2054 7275 652c 2070 6c6f      If True, plo
-00026720: 7420 6669 6c65 206c 6f63 6174 696f 6e20  t file location 
-00026730: 6973 2077 7269 7474 656e 2074 6f20 7465  is written to te
-00026740: 726d 696e 616c 0a0a 2020 2020 5265 7475  rminal..    Retu
-00026750: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
-00026760: 2020 2020 706c 742e 4669 6775 7265 0a20      plt.Figure. 
-00026770: 2020 2020 2020 204d 6174 706c 6f74 6c69         Matplotli
-00026780: 6220 6669 6775 7265 206f 626a 6563 740a  b figure object.
-00026790: 2020 2020 706c 742e 4178 6573 0a20 2020      plt.Axes.   
-000267a0: 2020 2020 204d 6174 706c 6f74 6c69 6220       Matplotlib 
-000267b0: 6178 6973 206f 626a 6563 740a 2020 2020  axis object.    
-000267c0: 2727 270a 0a20 2020 2023 2043 7265 6174  '''..    # Creat
-000267d0: 6520 6669 6775 7265 2061 6e64 2061 7865  e figure and axe
-000267e0: 730a 2020 2020 6669 672c 2061 7820 3d20  s.    fig, ax = 
-000267f0: 706c 742e 7375 6270 6c6f 7473 280a 2020  plt.subplots(.  
-00026800: 2020 2020 2020 312c 0a20 2020 2020 2020        1,.       
-00026810: 2031 2c0a 2020 2020 2020 2020 7368 6172   1,.        shar
-00026820: 6578 3d54 7275 652c 0a20 2020 2020 2020  ex=True,.       
-00026830: 2073 6861 7265 793d 5472 7565 2c0a 2020   sharey=True,.  
-00026840: 2020 2020 2020 6669 6773 697a 653d 2836        figsize=(6
-00026850: 2c20 352e 3529 2c0a 2020 2020 2020 2020  , 5.5),.        
-00026860: 6e75 6d3d 2746 6974 7465 6420 7265 6c61  num='Fitted rela
-00026870: 7861 7469 6f6e 2070 726f 6669 6c65 270a  xation profile'.
-00026880: 2020 2020 290a 0a20 2020 2069 6620 6973      )..    if is
-00026890: 696e 7374 616e 6365 2864 6174 6173 6574  instance(dataset
-000268a0: 2c20 5461 7548 4461 7461 7365 7429 3a0a  , TauHDataset):.
-000268b0: 2020 2020 2020 2020 785f 7661 6c73 203d          x_vals =
-000268c0: 2063 6f70 792e 636f 7079 2864 6174 6173   copy.copy(datas
-000268d0: 6574 2e66 6965 6c64 7329 0a20 2020 2020  et.fields).     
-000268e0: 2020 2078 5f74 7970 6520 3d20 2766 6965     x_type = 'fie
-000268f0: 6c64 270a 2020 2020 2020 2020 6178 2e73  ld'.        ax.s
-00026900: 6574 5f78 6c61 6265 6c28 7227 4669 656c  et_xlabel(r'Fiel
-00026910: 6420 284f 6529 2729 0a20 2020 2065 6c69  d (Oe)').    eli
-00026920: 6620 6973 696e 7374 616e 6365 2864 6174  f isinstance(dat
-00026930: 6173 6574 2c20 5461 7554 4461 7461 7365  aset, TauTDatase
-00026940: 7429 3a0a 2020 2020 2020 2020 785f 7661  t):.        x_va
-00026950: 6c73 203d 2063 6f70 792e 636f 7079 2864  ls = copy.copy(d
-00026960: 6174 6173 6574 2e74 656d 7065 7261 7475  ataset.temperatu
-00026970: 7265 7329 0a20 2020 2020 2020 2078 5f74  res).        x_t
-00026980: 7970 6520 3d20 2774 656d 7065 7261 7475  ype = 'temperatu
-00026990: 7265 270a 2020 2020 2020 2020 6178 2e73  re'.        ax.s
-000269a0: 6574 5f78 6c61 6265 6c28 7227 5465 6d70  et_xlabel(r'Temp
-000269b0: 6572 6174 7572 6520 284b 2927 290a 0a20  erature (K)').. 
-000269c0: 2020 2023 2041 6464 2075 6e63 6572 7461     # Add uncerta
-000269d0: 696e 7469 6573 2061 7320 6572 726f 7262  inties as errorb
-000269e0: 6172 730a 2020 2020 6966 206c 656e 2864  ars.    if len(d
-000269f0: 6174 6173 6574 2e72 6174 655f 706d 293a  ataset.rate_pm):
-00026a00: 0a20 2020 2020 2020 2061 782e 6572 726f  .        ax.erro
-00026a10: 7262 6172 280a 2020 2020 2020 2020 2020  rbar(.          
-00026a20: 2020 785f 7661 6c73 2c0a 2020 2020 2020    x_vals,.      
-00026a30: 2020 2020 2020 6461 7461 7365 742e 7261        dataset.ra
-00026a40: 7465 732c 0a20 2020 2020 2020 2020 2020  tes,.           
-00026a50: 2079 6572 723d 6461 7461 7365 742e 7261   yerr=dataset.ra
-00026a60: 7465 5f70 6d2c 0a20 2020 2020 2020 2020  te_pm,.         
-00026a70: 2020 206d 6172 6b65 723d 276f 272c 0a20     marker='o',. 
-00026a80: 2020 2020 2020 2020 2020 206c 773d 302c             lw=0,
-00026a90: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-00026aa0: 6e65 7769 6474 683d 312e 352c 0a20 2020  newidth=1.5,.   
-00026ab0: 2020 2020 2020 2020 2066 696c 6c73 7479           fillsty
-00026ac0: 6c65 3d27 6e6f 6e65 272c 0a20 2020 2020  le='none',.     
-00026ad0: 2020 2020 2020 2063 6f6c 6f72 3d27 626c         color='bl
-00026ae0: 6163 6b27 0a20 2020 2020 2020 2029 0a20  ack'.        ). 
-00026af0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00026b00: 2061 782e 706c 6f74 280a 2020 2020 2020   ax.plot(.      
-00026b10: 2020 2020 2020 785f 7661 6c73 2c0a 2020        x_vals,.  
-00026b20: 2020 2020 2020 2020 2020 6461 7461 7365            datase
-00026b30: 742e 7261 7465 732c 0a20 2020 2020 2020  t.rates,.       
-00026b40: 2020 2020 206d 6172 6b65 723d 276f 272c       marker='o',
-00026b50: 0a20 2020 2020 2020 2020 2020 206c 773d  .            lw=
-00026b60: 302c 0a20 2020 2020 2020 2020 2020 2066  0,.            f
-00026b70: 696c 6c73 7479 6c65 3d27 6e6f 6e65 272c  illstyle='none',
-00026b80: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
-00026b90: 6f72 3d27 626c 6163 6b27 0a20 2020 2020  or='black'.     
-00026ba0: 2020 2029 0a0a 2020 2020 6966 2078 5f74     )..    if x_t
-00026bb0: 7970 6520 3d3d 2027 6669 656c 6427 3a0a  ype == 'field':.
-00026bc0: 2020 2020 2020 2020 6966 2061 6e79 2876          if any(v
-00026bd0: 616c 203c 206e 702e 6669 6e66 6f28 666c  al < np.finfo(fl
-00026be0: 6f61 7429 2e65 7073 2066 6f72 2076 616c  oat).eps for val
-00026bf0: 2069 6e20 785f 7661 6c73 293a 0a20 2020   in x_vals):.   
-00026c00: 2020 2020 2020 2020 2061 782e 7365 745f           ax.set_
-00026c10: 7873 6361 6c65 280a 2020 2020 2020 2020  xscale(.        
-00026c20: 2020 2020 2020 2020 2773 796d 6c6f 6727          'symlog'
-00026c30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00026c40: 2020 6c69 6e74 6872 6573 683d 6775 692e    linthresh=gui.
-00026c50: 6361 6c63 5f6c 696e 7468 7265 7368 2878  calc_linthresh(x
-00026c60: 5f76 616c 7329 2c0a 2020 2020 2020 2020  _vals),.        
-00026c70: 2020 2020 2020 2020 6c69 6e73 6361 6c65          linscale
-00026c80: 3d67 7569 2e63 616c 635f 6c69 6e73 6361  =gui.calc_linsca
-00026c90: 6c65 2878 5f76 616c 7329 0a20 2020 2020  le(x_vals).     
-00026ca0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00026cb0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00026cc0: 2020 2061 782e 7365 745f 7873 6361 6c65     ax.set_xscale
-00026cd0: 2827 6c6f 6727 290a 2020 2020 656c 7365  ('log').    else
-00026ce0: 3a0a 2020 2020 2020 2020 6178 2e73 6574  :.        ax.set
-00026cf0: 5f78 7363 616c 6528 276c 6f67 2729 0a20  _xscale('log'). 
-00026d00: 2020 2061 782e 7365 745f 7973 6361 6c65     ax.set_yscale
-00026d10: 2827 6c6f 6727 290a 0a20 2020 2061 782e  ('log')..    ax.
-00026d20: 7365 745f 796c 6162 656c 2872 2752 6174  set_ylabel(r'Rat
-00026d30: 6520 2873 245e 5c6d 6174 6872 6567 756c  e (s$^\mathregul
-00026d40: 6172 7b2d 317d 2429 2729 0a0a 2020 2020  ar{-1}$)')..    
-00026d50: 6966 206c 656e 2864 6174 6173 6574 2e6c  if len(dataset.l
-00026d60: 6f67 7261 7465 5f70 6d29 3a0a 2020 2020  ograte_pm):.    
-00026d70: 2020 2020 616c 6c5f 6461 7461 203d 205b      all_data = [
-00026d80: 0a20 2020 2020 2020 2020 2020 206e 702e  .            np.
-00026d90: 6c6f 6731 3028 6461 7461 7365 742e 7261  log10(dataset.ra
-00026da0: 7465 7329 202b 2064 6174 6173 6574 2e6c  tes) + dataset.l
-00026db0: 6f67 7261 7465 5f70 6d0a 2020 2020 2020  ograte_pm.      
-00026dc0: 2020 5d0a 2020 2020 2020 2020 616c 6c5f    ].        all_
-00026dd0: 6461 7461 202b 3d20 5b0a 2020 2020 2020  data += [.      
-00026de0: 2020 2020 2020 6e70 2e6c 6f67 3130 2864        np.log10(d
-00026df0: 6174 6173 6574 2e72 6174 6573 2920 2d20  ataset.rates) - 
-00026e00: 6461 7461 7365 742e 6c6f 6772 6174 655f  dataset.lograte_
-00026e10: 706d 0a20 2020 2020 2020 205d 0a20 2020  pm.        ].   
-00026e20: 2065 6c73 653a 0a20 2020 2020 2020 2061   else:.        a
-00026e30: 6c6c 5f64 6174 6120 3d20 5b0a 2020 2020  ll_data = [.    
-00026e40: 2020 2020 2020 2020 6e70 2e6c 6f67 3130          np.log10
-00026e50: 2864 6174 6173 6574 2e72 6174 6573 290a  (dataset.rates).
-00026e60: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-00026e70: 2020 616c 6c5f 6461 7461 202b 3d20 5b0a    all_data += [.
-00026e80: 2020 2020 2020 2020 2020 2020 6e70 2e6c              np.l
-00026e90: 6f67 3130 2864 6174 6173 6574 2e72 6174  og10(dataset.rat
-00026ea0: 6573 290a 2020 2020 2020 2020 5d0a 0a20  es).        ].. 
-00026eb0: 2020 2067 7569 2e66 6f72 6d61 745f 7261     gui.format_ra
-00026ec0: 7465 5f78 5f79 5f61 7865 7328 0a20 2020  te_x_y_axes(.   
-00026ed0: 2020 2020 2061 782c 0a20 2020 2020 2020       ax,.       
-00026ee0: 2064 6174 6173 6574 2e72 6174 6573 2c0a   dataset.rates,.
-00026ef0: 2020 2020 2020 2020 785f 7661 6c73 2c0a          x_vals,.
-00026f00: 2020 2020 2020 2020 6e70 2e61 6273 2864          np.abs(d
-00026f10: 6174 6173 6574 2e72 6174 655f 706d 292c  ataset.rate_pm),
-00026f20: 0a20 2020 2020 2020 2078 5f74 7970 653d  .        x_type=
-00026f30: 785f 7479 7065 0a20 2020 2029 0a0a 2020  x_type.    )..  
-00026f40: 2020 2320 5365 7420 7820 7469 636b 2066    # Set x tick f
-00026f50: 6f72 6d61 7474 696e 670a 2020 2020 6775  ormatting.    gu
-00026f60: 692e 7365 745f 7261 7465 5f78 7469 636b  i.set_rate_xtick
-00026f70: 5f66 6f72 6d61 7474 696e 6728 6178 2c20  _formatting(ax, 
-00026f80: 785f 7661 6c73 2c20 785f 7479 7065 3d78  x_vals, x_type=x
-00026f90: 5f74 7970 6529 0a0a 2020 2020 6669 672e  _type)..    fig.
-00026fa0: 7469 6768 745f 6c61 796f 7574 2829 0a0a  tight_layout()..
-00026fb0: 2020 2020 2320 5375 7070 7265 7373 2073      # Suppress s
-00026fc0: 796d 6c6f 6720 7761 726e 696e 670a 2020  ymlog warning.  
-00026fd0: 2020 7761 726e 696e 6773 2e73 696d 706c    warnings.simpl
-00026fe0: 6566 696c 7465 7228 2769 676e 6f72 6527  efilter('ignore'
-00026ff0: 2c20 5573 6572 5761 726e 696e 6729 0a0a  , UserWarning)..
-00027000: 2020 2020 6966 2073 6176 653a 0a20 2020      if save:.   
-00027010: 2020 2020 2070 6c74 2e73 6176 6566 6967       plt.savefig
-00027020: 2873 6176 655f 6e61 6d65 290a 2020 2020  (save_name).    
-00027030: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
-00027040: 2020 2020 2020 2020 2020 2020 7574 2e63              ut.c
-00027050: 7072 696e 7428 0a20 2020 2020 2020 2020  print(.         
-00027060: 2020 2020 2020 2066 275c 6e20 5265 6c61         f'\n Rela
-00027070: 7861 7469 6f6e 2070 6c6f 7420 7361 7665  xation plot save
-00027080: 6420 746f 205c 6e20 7b73 6176 655f 6e61  d to \n {save_na
-00027090: 6d65 7d5c 6e27 2c0a 2020 2020 2020 2020  me}\n',.        
-000270a0: 2020 2020 2020 2020 2763 7961 6e27 0a20          'cyan'. 
-000270b0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-000270c0: 2069 6620 7368 6f77 3a0a 2020 2020 2020   if show:.      
-000270d0: 2020 706c 742e 7368 6f77 2829 0a0a 2020    plt.show()..  
-000270e0: 2020 2320 5265 656e 6162 6c65 2073 796d    # Reenable sym
-000270f0: 6c6f 6720 7761 726e 696e 670a 2020 2020  log warning.    
-00027100: 7761 726e 696e 6773 2e73 696d 706c 6566  warnings.simplef
-00027110: 696c 7465 7228 2764 6566 6175 6c74 272c  ilter('default',
-00027120: 2055 7365 7257 6172 6e69 6e67 290a 0a20   UserWarning).. 
-00027130: 2020 2072 6574 7572 6e20 6669 672c 2061     return fig, a
-00027140: 780a 0a0a 6465 6620 706c 6f74 5f72 6174  x...def plot_rat
-00027150: 655f 7265 7369 6475 616c 7328 6461 7461  e_residuals(data
-00027160: 7365 743a 2054 6175 5444 6174 6173 6574  set: TauTDataset
-00027170: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00027180: 2020 2020 2020 2020 2020 6d6f 6465 6c3a            model:
-00027190: 204c 6f67 5461 7554 4d6f 6465 6c20 7c20   LogTauTModel | 
-000271a0: 4d75 6c74 694c 6f67 5461 7554 4d6f 6465  MultiLogTauTMode
-000271b0: 6c20 7c20 4c6f 6754 6175 484d 6f64 656c  l | LogTauHModel
-000271c0: 207c 204d 756c 7469 4c6f 6754 6175 484d   | MultiLogTauHM
-000271d0: 6f64 656c 2c20 2320 6e6f 7161 0a20 2020  odel, # noqa.   
-000271e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000271f0: 2020 2020 2073 6176 653a 2062 6f6f 6c20       save: bool 
-00027200: 3d20 4661 6c73 652c 2073 686f 773a 2062  = False, show: b
-00027210: 6f6f 6c20 3d20 5472 7565 2c0a 2020 2020  ool = True,.    
+00024820: 2020 2020 2020 2020 2073 686f 775f 7061           show_pa
+00024830: 7261 6d73 3a20 626f 6f6c 203d 2054 7275  rams: bool = Tru
+00024840: 6529 202d 3e20 4e6f 6e65 3a0a 2020 2020  e) -> None:.    
+00024850: 2727 270a 2020 2020 506c 6f74 7320 6578  '''.    Plots ex
+00024860: 7065 7269 6d65 6e74 616c 2061 6e64 2066  perimental and f
+00024870: 6974 7465 6420 286d 6f64 656c 2920 7265  itted (model) re
+00024880: 6c61 7861 7469 6f6e 2072 6174 6520 6173  laxation rate as
+00024890: 5c6e 0a20 2020 2072 6174 6520 7673 2078  \n.    rate vs x
+000248a0: 7661 7220 7768 6572 6520 7876 6172 2069  var where xvar i
+000248b0: 7320 5420 6f72 2048 2e20 5769 7468 206c  s T or H. With l
+000248c0: 6f67 206c 6f67 2073 6361 6c65 2e0a 0a20  og log scale... 
+000248d0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+000248e0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+000248f0: 2064 6174 6173 6574 3a20 5461 7554 4461   dataset: TauTDa
+00024900: 7461 7365 7420 7c20 5461 7548 4461 7461  taset | TauHData
+00024910: 7365 740a 2020 2020 2020 2020 4461 7461  set.        Data
+00024920: 7365 7420 746f 2070 6c6f 740a 2020 2020  set to plot.    
+00024930: 6d6f 6465 6c3a 204c 6f67 5461 7554 4d6f  model: LogTauTMo
+00024940: 6465 6c20 7c20 4d75 6c74 694c 6f67 5461  del | MultiLogTa
+00024950: 7554 4d6f 6465 6c20 7c20 4c6f 6754 6175  uTModel | LogTau
+00024960: 484d 6f64 656c 207c 204d 756c 7469 4c6f  HModel | MultiLo
+00024970: 6754 6175 484d 6f64 656c 0a20 2020 2020  gTauHModel.     
+00024980: 2020 204d 6f64 656c 2028 6669 7474 6564     Model (fitted
+00024990: 2920 746f 2070 6c6f 740a 2020 2020 7368  ) to plot.    sh
+000249a0: 6f77 3a20 626f 6f6c 2c20 6465 6661 756c  ow: bool, defaul
+000249b0: 7420 5472 7565 0a20 2020 2020 2020 2049  t True.        I
+000249c0: 6620 5472 7565 2c20 7368 6f77 2070 6c6f  f True, show plo
+000249d0: 7420 6f6e 2073 6372 6565 6e0a 2020 2020  t on screen.    
+000249e0: 7361 7665 3a20 626f 6f6c 2c20 6465 6661  save: bool, defa
+000249f0: 756c 7420 4661 6c73 650a 2020 2020 2020  ult False.      
+00024a00: 2020 4966 2054 7275 652c 2073 6176 6520    If True, save 
+00024a10: 706c 6f74 2074 6f20 6669 6c65 2060 7361  plot to file `sa
+00024a20: 7665 5f6e 616d 6560 0a20 2020 2073 6176  ve_name`.    sav
+00024a30: 655f 6e61 6d65 3a20 7374 722c 2064 6566  e_name: str, def
+00024a40: 6175 6c74 2027 6669 7474 6564 5f72 6174  ault 'fitted_rat
+00024a50: 6573 2e70 6e67 270a 2020 2020 2020 2020  es.png'.        
+00024a60: 4966 2073 6176 6520 6973 2054 7275 652c  If save is True,
+00024a70: 2077 696c 6c20 7361 7665 2070 6c6f 7420   will save plot 
+00024a80: 746f 2074 6869 7320 6669 6c65 6e61 6d65  to this filename
+00024a90: 0a20 2020 2076 6572 626f 7365 3a20 626f  .    verbose: bo
+00024aa0: 6f6c 2c20 6465 6661 756c 7420 5472 7565  ol, default True
+00024ab0: 0a20 2020 2020 2020 2049 6620 5472 7565  .        If True
+00024ac0: 2c20 706c 6f74 2066 696c 6520 6c6f 6361  , plot file loca
+00024ad0: 7469 6f6e 2069 7320 7772 6974 7465 6e20  tion is written 
+00024ae0: 746f 2074 6572 6d69 6e61 6c0a 2020 2020  to terminal.    
+00024af0: 7368 6f77 5f70 6172 616d 733a 2062 6f6f  show_params: boo
+00024b00: 6c2c 2064 6566 6175 6c74 2054 7275 650a  l, default True.
+00024b10: 2020 2020 2020 2020 4966 2054 7275 652c          If True,
+00024b20: 2073 686f 7773 2066 6974 7465 6420 7061   shows fitted pa
+00024b30: 7261 6d65 7465 7273 206f 6e20 706c 6f74  rameters on plot
+00024b40: 0a0a 2020 2020 5265 7475 726e 730a 2020  ..    Returns.  
+00024b50: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 4e6f    -------.    No
+00024b60: 6e65 0a20 2020 2027 2727 0a0a 2020 2020  ne.    '''..    
+00024b70: 7769 6e64 6f77 203d 2067 7569 2e4d 6174  window = gui.Mat
+00024b80: 706c 6f74 6c69 6257 696e 646f 7728 290a  plotlibWindow().
+00024b90: 0a20 2020 2077 696e 646f 772e 7365 7457  .    window.setW
+00024ba0: 696e 646f 7754 6974 6c65 2827 4669 7474  indowTitle('Fitt
+00024bb0: 6564 2072 656c 6178 6174 696f 6e20 7072  ed relaxation pr
+00024bc0: 6f66 696c 6527 290a 0a20 2020 2023 2041  ofile')..    # A
+00024bd0: 6464 2070 6c6f 740a 2020 2020 5f70 6c6f  dd plot.    _plo
+00024be0: 745f 6669 7474 6564 5f72 6174 6573 280a  t_fitted_rates(.
+00024bf0: 2020 2020 2020 2020 6461 7461 7365 742c          dataset,
+00024c00: 206d 6f64 656c 2c20 7769 6e64 6f77 2e73   model, window.s
+00024c10: 632e 6669 672c 2077 696e 646f 772e 7363  c.fig, window.sc
+00024c20: 2e61 782c 2073 686f 775f 7061 7261 6d73  .ax, show_params
+00024c30: 3d73 686f 775f 7061 7261 6d73 0a20 2020  =show_params.   
+00024c40: 2029 0a0a 2020 2020 7761 726e 696e 6773   )..    warnings
+00024c50: 2e73 696d 706c 6566 696c 7465 7228 2769  .simplefilter('i
+00024c60: 676e 6f72 6527 2c20 5573 6572 5761 726e  gnore', UserWarn
+00024c70: 696e 6729 0a20 2020 2023 2053 6176 6520  ing).    # Save 
+00024c80: 706c 6f74 0a20 2020 2069 6620 7361 7665  plot.    if save
+00024c90: 3a0a 2020 2020 2020 2020 7769 6e64 6f77  :.        window
+00024ca0: 2e73 632e 6669 672e 7361 7665 6669 6728  .sc.fig.savefig(
+00024cb0: 7361 7665 5f6e 616d 652c 2064 7069 3d33  save_name, dpi=3
+00024cc0: 3030 290a 2020 2020 2020 2020 6966 2076  00).        if v
+00024cd0: 6572 626f 7365 3a0a 2020 2020 2020 2020  erbose:.        
+00024ce0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00024cf0: 6528 6461 7461 7365 742c 2028 5461 7554  e(dataset, (TauT
+00024d00: 4461 7461 7365 7429 293a 0a20 2020 2020  Dataset)):.     
+00024d10: 2020 2020 2020 2020 2020 205f 7876 6172             _xvar
+00024d20: 203d 2027 5427 0a20 2020 2020 2020 2020   = 'T'.         
+00024d30: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
+00024d40: 6365 2864 6174 6173 6574 2c20 2854 6175  ce(dataset, (Tau
+00024d50: 4844 6174 6173 6574 2929 3a0a 2020 2020  HDataset)):.    
+00024d60: 2020 2020 2020 2020 2020 2020 5f78 7661              _xva
+00024d70: 7220 3d20 2748 270a 2020 2020 2020 2020  r = 'H'.        
+00024d80: 2020 2020 7574 2e63 7072 696e 7428 0a20      ut.cprint(. 
+00024d90: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00024da0: 275c 6e20 4669 7474 6564 20cf 84e2 81bb  '\n Fitted .....
+00024db0: c2b9 2076 7320 7b5f 7876 6172 7d20 706c  .. vs {_xvar} pl
+00024dc0: 6f74 2073 6176 6564 2074 6f20 5c6e 207b  ot saved to \n {
+00024dd0: 7361 7665 5f6e 616d 657d 5c6e 272c 0a20  save_name}\n',. 
+00024de0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00024df0: 6379 616e 270a 2020 2020 2020 2020 2020  cyan'.          
+00024e00: 2020 290a 0a20 2020 2069 6620 7368 6f77    )..    if show
+00024e10: 3a0a 2020 2020 2020 2020 7769 6e64 6f77  :.        window
+00024e20: 2e73 686f 7728 290a 2020 2020 2020 2020  .show().        
+00024e30: 2320 4361 6c6c 2074 7769 6365 2065 6c73  # Call twice els
+00024e40: 6520 6974 2077 6f6e 7420 776f 726b 210a  e it wont work!.
+00024e50: 2020 2020 2020 2020 7769 6e64 6f77 2e73          window.s
+00024e60: 632e 6669 672e 7469 6768 745f 6c61 796f  c.fig.tight_layo
+00024e70: 7574 2829 0a20 2020 2020 2020 2077 696e  ut().        win
+00024e80: 646f 772e 7363 2e66 6967 2e74 6967 6874  dow.sc.fig.tight
+00024e90: 5f6c 6179 6f75 7428 290a 2020 2020 2020  _layout().      
+00024ea0: 2020 6170 702e 6578 6563 5f28 290a 0a20    app.exec_().. 
+00024eb0: 2020 2077 6172 6e69 6e67 732e 7369 6d70     warnings.simp
+00024ec0: 6c65 6669 6c74 6572 2827 6465 6661 756c  lefilter('defaul
+00024ed0: 7427 2c20 5573 6572 5761 726e 696e 6729  t', UserWarning)
+00024ee0: 0a0a 2020 2020 7265 7475 726e 0a0a 0a64  ..    return...d
+00024ef0: 6566 205f 706c 6f74 5f66 6974 7465 645f  ef _plot_fitted_
+00024f00: 7261 7465 7328 6461 7461 7365 743a 2054  rates(dataset: T
+00024f10: 6175 5444 6174 6173 6574 207c 2054 6175  auTDataset | Tau
+00024f20: 4844 6174 6173 6574 2c0a 2020 2020 2020  HDataset,.      
+00024f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024f40: 206d 6f64 656c 3a20 4c6f 6754 6175 544d   model: LogTauTM
+00024f50: 6f64 656c 207c 204d 756c 7469 4c6f 6754  odel | MultiLogT
+00024f60: 6175 544d 6f64 656c 207c 204c 6f67 5461  auTModel | LogTa
+00024f70: 7548 4d6f 6465 6c20 7c20 4d75 6c74 694c  uHModel | MultiL
+00024f80: 6f67 5461 7548 4d6f 6465 6c2c 2023 206e  ogTauHModel, # n
+00024f90: 6f71 610a 2020 2020 2020 2020 2020 2020  oqa.            
+00024fa0: 2020 2020 2020 2020 2020 2066 6967 3a20             fig: 
+00024fb0: 706c 742e 4669 6775 7265 2c20 6178 3a20  plt.Figure, ax: 
+00024fc0: 706c 742e 4178 6573 2c0a 2020 2020 2020  plt.Axes,.      
+00024fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024fe0: 2073 686f 775f 7061 7261 6d73 3a20 626f   show_params: bo
+00024ff0: 6f6c 203d 2054 7275 6529 3a0a 2020 2020  ol = True):.    
+00025000: 2727 270a 2020 2020 506c 6f74 7320 6578  '''.    Plots ex
+00025010: 7065 7269 6d65 6e74 616c 2061 6e64 2066  perimental and f
+00025020: 6974 7465 6420 286d 6f64 656c 2920 7265  itted (model) re
+00025030: 6c61 7861 7469 6f6e 2072 6174 6520 6173  laxation rate as
+00025040: 5c6e 0a20 2020 2072 6174 6520 7673 2078  \n.    rate vs x
+00025050: 7661 7220 7768 6572 6520 7876 6172 2069  var where xvar i
+00025060: 7320 5420 6f72 2048 2e20 5769 7468 206c  s T or H. With l
+00025070: 6f67 206c 6f67 2073 6361 6c65 2e0a 0a20  og log scale... 
+00025080: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00025090: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+000250a0: 2064 6174 6173 6574 3a20 5461 7554 4461   dataset: TauTDa
+000250b0: 7461 7365 7420 7c20 5461 7548 4461 7461  taset | TauHData
+000250c0: 7365 740a 2020 2020 2020 2020 4461 7461  set.        Data
+000250d0: 7365 7420 746f 2070 6c6f 740a 2020 2020  set to plot.    
+000250e0: 6d6f 6465 6c3a 204c 6f67 5461 7554 4d6f  model: LogTauTMo
+000250f0: 6465 6c20 7c20 4d75 6c74 694c 6f67 5461  del | MultiLogTa
+00025100: 7554 4d6f 6465 6c20 7c20 4c6f 6754 6175  uTModel | LogTau
+00025110: 484d 6f64 656c 207c 204d 756c 7469 4c6f  HModel | MultiLo
+00025120: 6754 6175 484d 6f64 656c 0a20 2020 2020  gTauHModel.     
+00025130: 2020 204d 6f64 656c 2028 6669 7474 6564     Model (fitted
+00025140: 2920 746f 2070 6c6f 740a 2020 2020 6669  ) to plot.    fi
+00025150: 673a 2070 6c74 2e46 6967 7572 650a 2020  g: plt.Figure.  
+00025160: 2020 2020 2020 4d61 7470 6c6f 746c 6962        Matplotlib
+00025170: 2046 6967 7572 6520 6f62 6a65 6374 2075   Figure object u
+00025180: 7365 6420 666f 7220 706c 6f74 0a20 2020  sed for plot.   
+00025190: 2061 783a 2070 6c74 2e41 7865 730a 2020   ax: plt.Axes.  
+000251a0: 2020 2020 2020 4d61 7470 6c6f 746c 6962        Matplotlib
+000251b0: 2041 7869 7320 6f62 6a65 6374 2075 7365   Axis object use
+000251c0: 6420 666f 7220 706c 6f74 0a20 2020 2073  d for plot.    s
+000251d0: 686f 775f 7061 7261 6d73 3a20 626f 6f6c  how_params: bool
+000251e0: 2c20 6465 6661 756c 7420 5472 7565 0a20  , default True. 
+000251f0: 2020 2020 2020 2049 6620 5472 7565 2c20         If True, 
+00025200: 7368 6f77 7320 6669 7474 6564 2070 6172  shows fitted par
+00025210: 616d 6574 6572 7320 6f6e 2070 6c6f 740a  ameters on plot.
+00025220: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
+00025230: 202d 2d2d 2d2d 2d2d 0a20 2020 204e 6f6e   -------.    Non
+00025240: 650a 2020 2020 2727 270a 0a20 2020 2069  e.    '''..    i
+00025250: 6620 6973 696e 7374 616e 6365 2864 6174  f isinstance(dat
+00025260: 6173 6574 2c20 5461 7548 4461 7461 7365  aset, TauHDatase
+00025270: 7429 3a0a 2020 2020 2020 2020 785f 7661  t):.        x_va
+00025280: 6c73 203d 2063 6f70 792e 636f 7079 2864  ls = copy.copy(d
+00025290: 6174 6173 6574 2e66 6965 6c64 7329 0a20  ataset.fields). 
+000252a0: 2020 2020 2020 2078 5f74 7970 6520 3d20         x_type = 
+000252b0: 2766 6965 6c64 270a 2020 2020 2020 2020  'field'.        
+000252c0: 6178 2e73 6574 5f78 6c61 6265 6c28 7227  ax.set_xlabel(r'
+000252d0: 4669 656c 6420 284f 6529 2729 0a20 2020  Field (Oe)').   
+000252e0: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+000252f0: 2864 6174 6173 6574 2c20 5461 7554 4461  (dataset, TauTDa
+00025300: 7461 7365 7429 3a0a 2020 2020 2020 2020  taset):.        
+00025310: 785f 7661 6c73 203d 2063 6f70 792e 636f  x_vals = copy.co
+00025320: 7079 2864 6174 6173 6574 2e74 656d 7065  py(dataset.tempe
+00025330: 7261 7475 7265 7329 0a20 2020 2020 2020  ratures).       
+00025340: 2078 5f74 7970 6520 3d20 2774 656d 7065   x_type = 'tempe
+00025350: 7261 7475 7265 270a 2020 2020 2020 2020  rature'.        
+00025360: 6178 2e73 6574 5f78 6c61 6265 6c28 7227  ax.set_xlabel(r'
+00025370: 5465 6d70 6572 6174 7572 6520 284b 2927  Temperature (K)'
+00025380: 290a 0a20 2020 2023 2041 6464 2075 6e63  )..    # Add unc
+00025390: 6572 7461 696e 7469 6573 2061 7320 6572  ertainties as er
+000253a0: 726f 7262 6172 730a 2020 2020 6966 206c  rorbars.    if l
+000253b0: 656e 2864 6174 6173 6574 2e72 6174 655f  en(dataset.rate_
+000253c0: 706d 293a 0a20 2020 2020 2020 2061 782e  pm):.        ax.
+000253d0: 6572 726f 7262 6172 280a 2020 2020 2020  errorbar(.      
+000253e0: 2020 2020 2020 785f 7661 6c73 2c0a 2020        x_vals,.  
+000253f0: 2020 2020 2020 2020 2020 6461 7461 7365            datase
+00025400: 742e 7261 7465 732c 0a20 2020 2020 2020  t.rates,.       
+00025410: 2020 2020 2079 6572 723d 6461 7461 7365       yerr=datase
+00025420: 742e 7261 7465 5f70 6d2c 0a20 2020 2020  t.rate_pm,.     
+00025430: 2020 2020 2020 206d 6172 6b65 723d 276f         marker='o
+00025440: 272c 0a20 2020 2020 2020 2020 2020 206c  ',.            l
+00025450: 773d 302c 0a20 2020 2020 2020 2020 2020  w=0,.           
+00025460: 2065 6c69 6e65 7769 6474 683d 312e 352c   elinewidth=1.5,
+00025470: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
+00025480: 6c73 7479 6c65 3d27 6e6f 6e65 272c 0a20  lstyle='none',. 
+00025490: 2020 2020 2020 2020 2020 206c 6162 656c             label
+000254a0: 3d27 4578 7065 7269 6d65 6e74 272c 0a20  ='Experiment',. 
+000254b0: 2020 2020 2020 2020 2020 2063 6f6c 6f72             color
+000254c0: 3d27 626c 6163 6b27 0a20 2020 2020 2020  ='black'.       
+000254d0: 2029 0a20 2020 2065 6c73 653a 0a20 2020   ).    else:.   
+000254e0: 2020 2020 2061 782e 706c 6f74 280a 2020       ax.plot(.  
+000254f0: 2020 2020 2020 2020 2020 785f 7661 6c73            x_vals
+00025500: 2c0a 2020 2020 2020 2020 2020 2020 6461  ,.            da
+00025510: 7461 7365 742e 7261 7465 732c 0a20 2020  taset.rates,.   
+00025520: 2020 2020 2020 2020 206d 6172 6b65 723d           marker=
+00025530: 276f 272c 0a20 2020 2020 2020 2020 2020  'o',.           
+00025540: 206c 773d 302c 0a20 2020 2020 2020 2020   lw=0,.         
+00025550: 2020 2066 696c 6c73 7479 6c65 3d27 6e6f     fillstyle='no
+00025560: 6e65 272c 0a20 2020 2020 2020 2020 2020  ne',.           
+00025570: 206c 6162 656c 3d27 4578 7065 7269 6d65   label='Experime
+00025580: 6e74 272c 0a20 2020 2020 2020 2020 2020  nt',.           
+00025590: 2063 6f6c 6f72 3d27 626c 6163 6b27 0a20   color='black'. 
+000255a0: 2020 2020 2020 2029 0a0a 2020 2020 785f         )..    x_
+000255b0: 7661 7273 5f67 7269 6420 3d20 6e70 2e6c  vars_grid = np.l
+000255c0: 696e 7370 6163 6528 0a20 2020 2020 2020  inspace(.       
+000255d0: 206e 702e 6d69 6e28 785f 7661 6c73 292c   np.min(x_vals),
+000255e0: 0a20 2020 2020 2020 206e 702e 6d61 7828  .        np.max(
+000255f0: 785f 7661 6c73 292c 0a20 2020 2020 2020  x_vals),.       
+00025600: 2035 3030 300a 2020 2020 290a 0a20 2020   5000.    )..   
+00025610: 2069 6620 7479 7065 286d 6f64 656c 2920   if type(model) 
+00025620: 696e 205b 4d75 6c74 694c 6f67 5461 7554  in [MultiLogTauT
+00025630: 4d6f 6465 6c2c 204d 756c 7469 4c6f 6754  Model, MultiLogT
+00025640: 6175 484d 6f64 656c 5d3a 0a20 2020 2020  auHModel]:.     
+00025650: 2020 206c 6f67 6d6f 6465 6c73 203d 206d     logmodels = m
+00025660: 6f64 656c 2e6c 6f67 6d6f 6465 6c73 0a20  odel.logmodels. 
+00025670: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00025680: 206c 6f67 6d6f 6465 6c73 203d 205b 6d6f   logmodels = [mo
+00025690: 6465 6c5d 0a0a 2020 2020 666f 7220 6c6f  del]..    for lo
+000256a0: 676d 6f64 656c 2069 6e20 6c6f 676d 6f64  gmodel in logmod
+000256b0: 656c 733a 0a0a 2020 2020 2020 2020 6966  els:..        if
+000256c0: 2074 7970 6528 6c6f 676d 6f64 656c 2920   type(logmodel) 
+000256d0: 6973 204c 6f67 4f72 6261 6368 4d6f 6465  is LogOrbachMode
+000256e0: 6c3a 0a20 2020 2020 2020 2020 2020 206c  l:.            l
+000256f0: 6162 656c 5f66 6974 203d 2027 5c6e 4669  abel_fit = '\nFi
+00025700: 7420 7769 7468 270a 2020 2020 2020 2020  t with'.        
+00025710: 2020 2020 6c61 6265 6c5f 6669 7420 2b3d      label_fit +=
+00025720: 2027 5c6e 2720 2b20 7227 7b7d 207b 3a36   '\n' + r'{} {:6
+00025730: 2e32 667d 2073 272e 666f 726d 6174 280a  .2f} s'.format(.
+00025740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025750: 6c6f 676d 6f64 656c 2e56 4152 4e41 4d45  logmodel.VARNAME
+00025760: 535f 4d4d 5b27 755f 6566 6627 5d2c 0a20  S_MM['u_eff'],. 
+00025770: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00025780: 6f67 6d6f 6465 6c2e 6669 6e61 6c5f 7661  ogmodel.final_va
+00025790: 725f 7661 6c75 6573 5b27 755f 6566 6627  r_values['u_eff'
+000257a0: 5d0a 2020 2020 2020 2020 2020 2020 290a  ].            ).
+000257b0: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
+000257c0: 6c5f 6669 7420 2b3d 2027 5c6e 2720 2b20  l_fit += '\n' + 
+000257d0: 7227 7b7d 207b 3a30 342e 3365 7d27 2e66  r'{} {:04.3e}'.f
+000257e0: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
+000257f0: 2020 2020 2020 206c 6f67 6d6f 6465 6c2e         logmodel.
+00025800: 5641 524e 414d 4553 5f4d 4d5b 2741 275d  VARNAMES_MM['A']
+00025810: 2c20 6c6f 676d 6f64 656c 2e66 696e 616c  , logmodel.final
+00025820: 5f76 6172 5f76 616c 7565 735b 2741 275d  _var_values['A']
+00025830: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00025840: 2020 2020 2020 2065 6c69 6620 7479 7065         elif type
+00025850: 286c 6f67 6d6f 6465 6c29 2069 7320 4c6f  (logmodel) is Lo
+00025860: 6752 616d 616e 4d6f 6465 6c3a 0a20 2020  gRamanModel:.   
+00025870: 2020 2020 2020 2020 206c 6162 656c 5f66           label_f
+00025880: 6974 203d 2027 5c6e 4669 7420 7769 7468  it = '\nFit with
+00025890: 270a 2020 2020 2020 2020 2020 2020 6c61  '.            la
+000258a0: 6265 6c5f 6669 7420 2b3d 2027 5c6e 2720  bel_fit += '\n' 
+000258b0: 2b20 7227 7b7d 207b 3a36 2e32 667d 2073  + r'{} {:6.2f} s
+000258c0: 272e 666f 726d 6174 280a 2020 2020 2020  '.format(.      
+000258d0: 2020 2020 2020 2020 2020 6c6f 676d 6f64            logmod
+000258e0: 656c 2e56 4152 4e41 4d45 535f 4d4d 5b27  el.VARNAMES_MM['
+000258f0: 5227 5d2c 206c 6f67 6d6f 6465 6c2e 6669  R'], logmodel.fi
+00025900: 6e61 6c5f 7661 725f 7661 6c75 6573 5b27  nal_var_values['
+00025910: 5227 5d0a 2020 2020 2020 2020 2020 2020  R'].            
+00025920: 290a 2020 2020 2020 2020 2020 2020 6c61  ).            la
+00025930: 6265 6c5f 6669 7420 2b3d 2027 5c6e 2720  bel_fit += '\n' 
+00025940: 2b20 7227 7b7d 207b 3a30 342e 3365 7d27  + r'{} {:04.3e}'
+00025950: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
+00025960: 2020 2020 2020 2020 206c 6f67 6d6f 6465           logmode
+00025970: 6c2e 5641 524e 414d 4553 5f4d 4d5b 276e  l.VARNAMES_MM['n
+00025980: 275d 2c20 6c6f 676d 6f64 656c 2e66 696e  '], logmodel.fin
+00025990: 616c 5f76 6172 5f76 616c 7565 735b 276e  al_var_values['n
+000259a0: 275d 0a20 2020 2020 2020 2020 2020 2029  '].            )
+000259b0: 0a20 2020 2020 2020 2065 6c69 6620 7479  .        elif ty
+000259c0: 7065 286c 6f67 6d6f 6465 6c29 2069 7320  pe(logmodel) is 
+000259d0: 4c6f 6751 544d 4d6f 6465 6c3a 0a20 2020  LogQTMModel:.   
+000259e0: 2020 2020 2020 2020 206c 6162 656c 5f66           label_f
+000259f0: 6974 203d 2027 5c6e 4669 7420 7769 7468  it = '\nFit with
+00025a00: 270a 2020 2020 2020 2020 2020 2020 6c61  '.            la
+00025a10: 6265 6c5f 6669 7420 2b3d 2027 5c6e 2720  bel_fit += '\n' 
+00025a20: 2b20 7227 7b7d 207b 3a36 2e32 667d 2073  + r'{} {:6.2f} s
+00025a30: 272e 666f 726d 6174 280a 2020 2020 2020  '.format(.      
+00025a40: 2020 2020 2020 2020 2020 6c6f 676d 6f64            logmod
+00025a50: 656c 2e56 4152 4e41 4d45 535f 4d4d 5b27  el.VARNAMES_MM['
+00025a60: 5127 5d2c 206c 6f67 6d6f 6465 6c2e 6669  Q'], logmodel.fi
+00025a70: 6e61 6c5f 7661 725f 7661 6c75 6573 5b27  nal_var_values['
+00025a80: 5127 5d0a 2020 2020 2020 2020 2020 2020  Q'].            
+00025a90: 290a 2020 2020 2020 2020 656c 6966 2074  ).        elif t
+00025aa0: 7970 6528 6c6f 676d 6f64 656c 2920 6973  ype(logmodel) is
+00025ab0: 204c 6f67 4469 7265 6374 4d6f 6465 6c3a   LogDirectModel:
+00025ac0: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
+00025ad0: 656c 5f66 6974 203d 2027 5c6e 4669 7420  el_fit = '\nFit 
+00025ae0: 7769 7468 270a 2020 2020 2020 2020 2020  with'.          
+00025af0: 2020 6c61 6265 6c5f 6669 7420 2b3d 2027    label_fit += '
+00025b00: 5c6e 2720 2b20 7227 7b7d 207b 3a36 2e32  \n' + r'{} {:6.2
+00025b10: 667d 2073 272e 666f 726d 6174 280a 2020  f} s'.format(.  
+00025b20: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00025b30: 676d 6f64 656c 2e56 4152 4e41 4d45 535f  gmodel.VARNAMES_
+00025b40: 4d4d 5b27 4427 5d2c 206c 6f67 6d6f 6465  MM['D'], logmode
+00025b50: 6c2e 6669 6e61 6c5f 7661 725f 7661 6c75  l.final_var_valu
+00025b60: 6573 5b27 4427 5d0a 2020 2020 2020 2020  es['D'].        
+00025b70: 2020 2020 290a 2020 2020 2020 2020 6d6f      ).        mo
+00025b80: 6465 6c5f 7261 7465 7320 3d20 3130 2a2a  del_rates = 10**
+00025b90: 6c6f 676d 6f64 656c 2e6d 6f64 656c 280a  logmodel.model(.
+00025ba0: 2020 2020 2020 2020 2020 2020 6c6f 676d              logm
+00025bb0: 6f64 656c 2e66 696e 616c 5f76 6172 5f76  odel.final_var_v
+00025bc0: 616c 7565 732c 0a20 2020 2020 2020 2020  alues,.         
+00025bd0: 2020 2078 5f76 6172 735f 6772 6964 2c0a     x_vars_grid,.
+00025be0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00025bf0: 2020 2061 782e 706c 6f74 280a 2020 2020     ax.plot(.    
+00025c00: 2020 2020 2020 2020 6e70 2e61 7272 6179          np.array
+00025c10: 2878 5f76 6172 735f 6772 6964 292c 0a20  (x_vars_grid),. 
+00025c20: 2020 2020 2020 2020 2020 206e 702e 6172             np.ar
+00025c30: 7261 7928 6d6f 6465 6c5f 7261 7465 7329  ray(model_rates)
+00025c40: 2c0a 2020 2020 2020 2020 2020 2020 6c77  ,.            lw
+00025c50: 3d31 2e35 2c0a 2020 2020 2020 2020 2020  =1.5,.          
+00025c60: 2020 6c61 6265 6c3d 6c6f 676d 6f64 656c    label=logmodel
+00025c70: 2e4e 414d 452c 0a20 2020 2020 2020 2020  .NAME,.         
+00025c80: 2020 206c 733d 272d 2d27 0a20 2020 2020     ls='--'.     
+00025c90: 2020 2029 0a0a 2020 2020 6966 2074 7970     )..    if typ
+00025ca0: 6528 6d6f 6465 6c29 2069 6e20 5b4d 756c  e(model) in [Mul
+00025cb0: 7469 4c6f 6754 6175 544d 6f64 656c 2c20  tiLogTauTModel, 
+00025cc0: 4d75 6c74 694c 6f67 5461 7548 4d6f 6465  MultiLogTauHMode
+00025cd0: 6c5d 2061 6e64 206c 656e 286c 6f67 6d6f  l] and len(logmo
+00025ce0: 6465 6c73 2920 3e20 313a 2023 206e 6f71  dels) > 1: # noq
+00025cf0: 610a 2020 2020 2020 2020 746f 7461 6c20  a.        total 
+00025d00: 3d20 6e70 2e7a 6572 6f73 286c 656e 2878  = np.zeros(len(x
+00025d10: 5f76 6172 735f 6772 6964 2929 0a0a 2020  _vars_grid))..  
+00025d20: 2020 2020 2020 666f 7220 6c6f 676d 6f64        for logmod
+00025d30: 656c 2069 6e20 6c6f 676d 6f64 656c 733a  el in logmodels:
+00025d40: 0a20 2020 2020 2020 2020 2020 2074 6f74  .            tot
+00025d50: 616c 202b 3d20 3130 2a2a 6c6f 676d 6f64  al += 10**logmod
+00025d60: 656c 2e6d 6f64 656c 280a 2020 2020 2020  el.model(.      
+00025d70: 2020 2020 2020 2020 2020 6c6f 676d 6f64            logmod
+00025d80: 656c 2e66 696e 616c 5f76 6172 5f76 616c  el.final_var_val
+00025d90: 7565 732c 0a20 2020 2020 2020 2020 2020  ues,.           
+00025da0: 2020 2020 2078 5f76 6172 735f 6772 6964       x_vars_grid
+00025db0: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+00025dc0: 0a20 2020 2020 2020 2061 782e 706c 6f74  .        ax.plot
+00025dd0: 280a 2020 2020 2020 2020 2020 2020 785f  (.            x_
+00025de0: 7661 7273 5f67 7269 642c 0a20 2020 2020  vars_grid,.     
+00025df0: 2020 2020 2020 2074 6f74 616c 2c0a 2020         total,.  
+00025e00: 2020 2020 2020 2020 2020 6c77 3d31 2e35            lw=1.5
+00025e10: 2c0a 2020 2020 2020 2020 2020 2020 6c61  ,.            la
+00025e20: 6265 6c3d 2754 6f74 616c 272c 0a20 2020  bel='Total',.   
+00025e30: 2020 2020 2020 2020 2063 6f6c 6f72 3d27           color='
+00025e40: 7265 6427 0a20 2020 2020 2020 2029 0a0a  red'.        )..
+00025e50: 2020 2020 6966 2078 5f74 7970 6520 3d3d      if x_type ==
+00025e60: 2027 6669 656c 6427 3a0a 2020 2020 2020   'field':.      
+00025e70: 2020 6966 2061 6e79 2876 616c 203c 206e    if any(val < n
+00025e80: 702e 6669 6e66 6f28 666c 6f61 7429 2e65  p.finfo(float).e
+00025e90: 7073 2066 6f72 2076 616c 2069 6e20 785f  ps for val in x_
+00025ea0: 7661 6c73 293a 0a20 2020 2020 2020 2020  vals):.         
+00025eb0: 2020 2061 782e 7365 745f 7873 6361 6c65     ax.set_xscale
+00025ec0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00025ed0: 2020 2773 796d 6c6f 6727 2c0a 2020 2020    'symlog',.    
+00025ee0: 2020 2020 2020 2020 2020 2020 6c69 6e74              lint
+00025ef0: 6872 6573 683d 6775 692e 6361 6c63 5f6c  hresh=gui.calc_l
+00025f00: 696e 7468 7265 7368 2878 5f76 616c 7329  inthresh(x_vals)
+00025f10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00025f20: 2020 6c69 6e73 6361 6c65 3d67 7569 2e63    linscale=gui.c
+00025f30: 616c 635f 6c69 6e73 6361 6c65 2878 5f76  alc_linscale(x_v
+00025f40: 616c 7329 0a20 2020 2020 2020 2020 2020  als).           
+00025f50: 2029 0a20 2020 2020 2020 2065 6c73 653a   ).        else:
+00025f60: 0a20 2020 2020 2020 2020 2020 2061 782e  .            ax.
+00025f70: 7365 745f 7873 6361 6c65 2827 6c6f 6727  set_xscale('log'
+00025f80: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
+00025f90: 2020 2020 6178 2e73 6574 5f78 7363 616c      ax.set_xscal
+00025fa0: 6528 276c 6f67 2729 0a20 2020 2061 782e  e('log').    ax.
+00025fb0: 7365 745f 7973 6361 6c65 2827 6c6f 6727  set_yscale('log'
+00025fc0: 290a 0a20 2020 2067 7569 2e66 6f72 6d61  )..    gui.forma
+00025fd0: 745f 7261 7465 5f78 5f79 5f61 7865 7328  t_rate_x_y_axes(
+00025fe0: 0a20 2020 2020 2020 2061 782c 0a20 2020  .        ax,.   
+00025ff0: 2020 2020 2064 6174 6173 6574 2e72 6174       dataset.rat
+00026000: 6573 2c0a 2020 2020 2020 2020 785f 7661  es,.        x_va
+00026010: 6c73 2c0a 2020 2020 2020 2020 6e70 2e61  ls,.        np.a
+00026020: 6273 2864 6174 6173 6574 2e72 6174 655f  bs(dataset.rate_
+00026030: 706d 292c 0a20 2020 2020 2020 2078 5f74  pm),.        x_t
+00026040: 7970 653d 785f 7479 7065 0a20 2020 2029  ype=x_type.    )
+00026050: 0a0a 2020 2020 6578 7072 6573 7369 6f6e  ..    expression
+00026060: 203d 2027 270a 0a20 2020 2066 6f72 206c   = ''..    for l
+00026070: 6f67 6d6f 6465 6c20 696e 206c 6f67 6d6f  ogmodel in logmo
+00026080: 6465 6c73 3a0a 2020 2020 2020 2020 666f  dels:.        fo
+00026090: 7220 6974 2c20 6e61 6d65 2069 6e20 656e  r it, name in en
+000260a0: 756d 6572 6174 6528 6c6f 676d 6f64 656c  umerate(logmodel
+000260b0: 2e50 4152 4e41 4d45 5329 3a0a 2020 2020  .PARNAMES):.    
+000260c0: 2020 2020 2020 2020 6578 7072 6573 7369          expressi
+000260d0: 6f6e 202b 3d20 277b 7d20 3d20 7b3a 2e33  on += '{} = {:.3
+000260e0: 667d 2027 2e66 6f72 6d61 7428 0a20 2020  f} '.format(.   
+000260f0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+00026100: 6d6f 6465 6c2e 5641 524e 414d 4553 5f4d  model.VARNAMES_M
+00026110: 4d5b 6e61 6d65 5d2c 0a20 2020 2020 2020  M[name],.       
+00026120: 2020 2020 2020 2020 206c 6f67 6d6f 6465           logmode
+00026130: 6c2e 6669 6e61 6c5f 7661 725f 7661 6c75  l.final_var_valu
+00026140: 6573 5b6e 616d 655d 2c0a 2020 2020 2020  es[name],.      
+00026150: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00026160: 2020 2020 6966 206e 616d 6520 696e 206c      if name in l
+00026170: 6f67 6d6f 6465 6c2e 6669 745f 7661 7273  ogmodel.fit_vars
+00026180: 2e6b 6579 7328 293a 0a20 2020 2020 2020  .keys():.       
+00026190: 2020 2020 2020 2020 2065 7870 7265 7373           express
+000261a0: 696f 6e20 2b3d 2072 2724 5c70 6d24 2027  ion += r'$\pm$ '
+000261b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000261c0: 2065 7870 7265 7373 696f 6e20 2b3d 2027   expression += '
+000261d0: 7b3a 2e33 667d 2027 2e66 6f72 6d61 7428  {:.3f} '.format(
+000261e0: 6c6f 676d 6f64 656c 2e66 6974 5f73 7464  logmodel.fit_std
+000261f0: 6576 5b6e 616d 655d 290a 2020 2020 2020  ev[name]).      
+00026200: 2020 2020 2020 6578 7072 6573 7369 6f6e        expression
+00026210: 202b 3d20 277b 7d20 2020 2027 2e66 6f72   += '{}    '.for
+00026220: 6d61 7428 6c6f 676d 6f64 656c 2e55 4e49  mat(logmodel.UNI
+00026230: 5453 5f4d 4d5b 6e61 6d65 5d29 0a20 2020  TS_MM[name]).   
+00026240: 2020 2020 2020 2020 2069 6620 6974 203d           if it =
+00026250: 3d20 3120 616e 6420 6c65 6e28 6c6f 676d  = 1 and len(logm
+00026260: 6f64 656c 2e66 6974 5f76 6172 732e 6b65  odel.fit_vars.ke
+00026270: 7973 2829 2920 3e20 323a 0a20 2020 2020  ys()) > 2:.     
+00026280: 2020 2020 2020 2020 2020 2065 7870 7265             expre
+00026290: 7373 696f 6e20 2b3d 2027 5c6e 270a 2020  ssion += '\n'.  
+000262a0: 2020 2020 2020 6578 7072 6573 7369 6f6e        expression
+000262b0: 202b 3d20 275c 6e27 0a0a 2020 2020 6966   += '\n'..    if
+000262c0: 2073 686f 775f 7061 7261 6d73 3a0a 2020   show_params:.  
+000262d0: 2020 2020 2020 6178 2e74 6578 7428 0a20        ax.text(. 
+000262e0: 2020 2020 2020 2020 2020 2030 2e30 2c20             0.0, 
+000262f0: 312e 3032 2c20 733d 6578 7072 6573 7369  1.02, s=expressi
+00026300: 6f6e 2c20 666f 6e74 7369 7a65 3d31 302c  on, fontsize=10,
+00026310: 2074 7261 6e73 666f 726d 3d61 782e 7472   transform=ax.tr
+00026320: 616e 7341 7865 730a 2020 2020 2020 2020  ansAxes.        
+00026330: 290a 0a20 2020 2069 6620 785f 7479 7065  )..    if x_type
+00026340: 203d 3d20 2766 6965 6c64 273a 0a20 2020   == 'field':.   
+00026350: 2020 2020 2061 782e 6c65 6765 6e64 280a       ax.legend(.
+00026360: 2020 2020 2020 2020 2020 2020 666f 6e74              font
+00026370: 7369 7a65 3d27 3130 272c 206e 756d 706f  size='10', numpo
+00026380: 696e 7473 3d31 2c20 6e63 6f6c 3d31 2c20  ints=1, ncol=1, 
+00026390: 6672 616d 656f 6e3d 4661 6c73 650a 2020  frameon=False.  
+000263a0: 2020 2020 2020 290a 2020 2020 656c 7365        ).    else
+000263b0: 3a0a 2020 2020 2020 2020 6178 2e6c 6567  :.        ax.leg
+000263c0: 656e 6428 0a20 2020 2020 2020 2020 2020  end(.           
+000263d0: 206c 6f63 3d27 7570 7065 7220 6c65 6674   loc='upper left
+000263e0: 272c 2066 6f6e 7473 697a 653d 2731 3027  ', fontsize='10'
+000263f0: 2c20 6e75 6d70 6f69 6e74 733d 312c 206e  , numpoints=1, n
+00026400: 636f 6c3d 312c 2066 7261 6d65 6f6e 3d46  col=1, frameon=F
+00026410: 616c 7365 0a20 2020 2020 2020 2029 0a0a  alse.        )..
+00026420: 2020 2020 6178 2e73 6574 5f79 6c61 6265      ax.set_ylabe
+00026430: 6c28 7227 5261 7465 2028 7324 5e5c 6d61  l(r'Rate (s$^\ma
+00026440: 7468 7265 6775 6c61 727b 2d31 7d24 2927  thregular{-1}$)'
+00026450: 290a 0a20 2020 2072 6574 7572 6e0a 0a0a  )..    return...
+00026460: 6465 6620 706c 6f74 5f72 6174 6573 2864  def plot_rates(d
+00026470: 6174 6173 6574 3a20 5461 7554 4461 7461  ataset: TauTData
+00026480: 7365 7420 7c20 5461 7548 4461 7461 7365  set | TauHDatase
+00026490: 742c 2073 686f 773a 2062 6f6f 6c20 3d20  t, show: bool = 
+000264a0: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+000264b0: 2020 2020 2073 6176 653a 2062 6f6f 6c20       save: bool 
+000264c0: 3d20 4661 6c73 652c 2073 6176 655f 6e61  = False, save_na
+000264d0: 6d65 3a20 7374 7220 3d20 2772 656c 6178  me: str = 'relax
+000264e0: 6174 696f 6e5f 7261 7465 732e 706e 6727  ation_rates.png'
+000264f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00026500: 2076 6572 626f 7365 3a20 626f 6f6c 203d   verbose: bool =
+00026510: 2054 7275 6529 202d 3e20 7475 706c 655b   True) -> tuple[
+00026520: 706c 742e 4669 6775 7265 2c20 706c 742e  plt.Figure, plt.
+00026530: 4178 6573 5d3a 0a20 2020 2027 2727 0a20  Axes]:.    '''. 
+00026540: 2020 2050 6c6f 7473 2065 7870 6572 696d     Plots experim
+00026550: 656e 7461 6c20 7265 6c61 7861 7469 6f6e  ental relaxation
+00026560: 2072 6174 6520 7673 2066 6965 6c64 2f74   rate vs field/t
+00026570: 656d 7065 7261 7475 7265 2061 6e64 0a20  emperature and. 
+00026580: 2020 2064 6973 706c 6179 7320 6f6e 2073     displays on s
+00026590: 6372 6565 6e2e 0a0a 2020 2020 5061 7261  creen...    Para
+000265a0: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
+000265b0: 2d2d 2d2d 2d0a 2020 2020 6461 7461 7365  -----.    datase
+000265c0: 743a 2054 6175 5444 6174 6173 6574 207c  t: TauTDataset |
+000265d0: 2054 6175 4844 6174 6173 6574 0a20 2020   TauHDataset.   
+000265e0: 2020 2020 2044 6174 6173 6574 2074 6f20       Dataset to 
+000265f0: 706c 6f74 0a20 2020 2073 686f 773a 2062  plot.    show: b
+00026600: 6f6f 6c2c 2064 6566 6175 6c74 2054 7275  ool, default Tru
+00026610: 650a 2020 2020 2020 2020 4966 2054 7275  e.        If Tru
+00026620: 652c 2073 686f 7720 706c 6f74 206f 6e20  e, show plot on 
+00026630: 7363 7265 656e 0a20 2020 2073 6176 653a  screen.    save:
+00026640: 2062 6f6f 6c2c 2064 6566 6175 6c74 2046   bool, default F
+00026650: 616c 7365 0a20 2020 2020 2020 2049 6620  alse.        If 
+00026660: 5472 7565 2c20 7361 7665 2070 6c6f 7420  True, save plot 
+00026670: 746f 2066 696c 6520 6073 6176 655f 6e61  to file `save_na
+00026680: 6d65 600a 2020 2020 7361 7665 5f6e 616d  me`.    save_nam
+00026690: 653a 2073 7472 2c20 6465 6661 756c 7420  e: str, default 
+000266a0: 2772 656c 6178 6174 696f 6e5f 7261 7465  'relaxation_rate
+000266b0: 732e 706e 6727 0a20 2020 2020 2020 2049  s.png'.        I
+000266c0: 6620 7361 7665 2069 7320 5472 7565 2c20  f save is True, 
+000266d0: 7769 6c6c 2073 6176 6520 706c 6f74 2074  will save plot t
+000266e0: 6f20 7468 6973 2066 696c 656e 616d 650a  o this filename.
+000266f0: 2020 2020 7665 7262 6f73 653a 2062 6f6f      verbose: boo
+00026700: 6c2c 2064 6566 6175 6c74 2054 7275 650a  l, default True.
+00026710: 2020 2020 2020 2020 4966 2054 7275 652c          If True,
+00026720: 2070 6c6f 7420 6669 6c65 206c 6f63 6174   plot file locat
+00026730: 696f 6e20 6973 2077 7269 7474 656e 2074  ion is written t
+00026740: 6f20 7465 726d 696e 616c 0a0a 2020 2020  o terminal..    
+00026750: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
+00026760: 2d2d 2d0a 2020 2020 706c 742e 4669 6775  ---.    plt.Figu
+00026770: 7265 0a20 2020 2020 2020 204d 6174 706c  re.        Matpl
+00026780: 6f74 6c69 6220 6669 6775 7265 206f 626a  otlib figure obj
+00026790: 6563 740a 2020 2020 706c 742e 4178 6573  ect.    plt.Axes
+000267a0: 0a20 2020 2020 2020 204d 6174 706c 6f74  .        Matplot
+000267b0: 6c69 6220 6178 6973 206f 626a 6563 740a  lib axis object.
+000267c0: 2020 2020 2727 270a 0a20 2020 2023 2043      '''..    # C
+000267d0: 7265 6174 6520 6669 6775 7265 2061 6e64  reate figure and
+000267e0: 2061 7865 730a 2020 2020 6669 672c 2061   axes.    fig, a
+000267f0: 7820 3d20 706c 742e 7375 6270 6c6f 7473  x = plt.subplots
+00026800: 280a 2020 2020 2020 2020 312c 0a20 2020  (.        1,.   
+00026810: 2020 2020 2031 2c0a 2020 2020 2020 2020       1,.        
+00026820: 7368 6172 6578 3d54 7275 652c 0a20 2020  sharex=True,.   
+00026830: 2020 2020 2073 6861 7265 793d 5472 7565       sharey=True
+00026840: 2c0a 2020 2020 2020 2020 6669 6773 697a  ,.        figsiz
+00026850: 653d 2836 2c20 352e 3529 2c0a 2020 2020  e=(6, 5.5),.    
+00026860: 2020 2020 6e75 6d3d 2746 6974 7465 6420      num='Fitted 
+00026870: 7265 6c61 7861 7469 6f6e 2070 726f 6669  relaxation profi
+00026880: 6c65 270a 2020 2020 290a 0a20 2020 2069  le'.    )..    i
+00026890: 6620 6973 696e 7374 616e 6365 2864 6174  f isinstance(dat
+000268a0: 6173 6574 2c20 5461 7548 4461 7461 7365  aset, TauHDatase
+000268b0: 7429 3a0a 2020 2020 2020 2020 785f 7661  t):.        x_va
+000268c0: 6c73 203d 2063 6f70 792e 636f 7079 2864  ls = copy.copy(d
+000268d0: 6174 6173 6574 2e66 6965 6c64 7329 0a20  ataset.fields). 
+000268e0: 2020 2020 2020 2078 5f74 7970 6520 3d20         x_type = 
+000268f0: 2766 6965 6c64 270a 2020 2020 2020 2020  'field'.        
+00026900: 6178 2e73 6574 5f78 6c61 6265 6c28 7227  ax.set_xlabel(r'
+00026910: 4669 656c 6420 284f 6529 2729 0a20 2020  Field (Oe)').   
+00026920: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+00026930: 2864 6174 6173 6574 2c20 5461 7554 4461  (dataset, TauTDa
+00026940: 7461 7365 7429 3a0a 2020 2020 2020 2020  taset):.        
+00026950: 785f 7661 6c73 203d 2063 6f70 792e 636f  x_vals = copy.co
+00026960: 7079 2864 6174 6173 6574 2e74 656d 7065  py(dataset.tempe
+00026970: 7261 7475 7265 7329 0a20 2020 2020 2020  ratures).       
+00026980: 2078 5f74 7970 6520 3d20 2774 656d 7065   x_type = 'tempe
+00026990: 7261 7475 7265 270a 2020 2020 2020 2020  rature'.        
+000269a0: 6178 2e73 6574 5f78 6c61 6265 6c28 7227  ax.set_xlabel(r'
+000269b0: 5465 6d70 6572 6174 7572 6520 284b 2927  Temperature (K)'
+000269c0: 290a 0a20 2020 2023 2041 6464 2075 6e63  )..    # Add unc
+000269d0: 6572 7461 696e 7469 6573 2061 7320 6572  ertainties as er
+000269e0: 726f 7262 6172 730a 2020 2020 6966 206c  rorbars.    if l
+000269f0: 656e 2864 6174 6173 6574 2e72 6174 655f  en(dataset.rate_
+00026a00: 706d 293a 0a20 2020 2020 2020 2061 782e  pm):.        ax.
+00026a10: 6572 726f 7262 6172 280a 2020 2020 2020  errorbar(.      
+00026a20: 2020 2020 2020 785f 7661 6c73 2c0a 2020        x_vals,.  
+00026a30: 2020 2020 2020 2020 2020 6461 7461 7365            datase
+00026a40: 742e 7261 7465 732c 0a20 2020 2020 2020  t.rates,.       
+00026a50: 2020 2020 2079 6572 723d 6461 7461 7365       yerr=datase
+00026a60: 742e 7261 7465 5f70 6d2c 0a20 2020 2020  t.rate_pm,.     
+00026a70: 2020 2020 2020 206d 6172 6b65 723d 276f         marker='o
+00026a80: 272c 0a20 2020 2020 2020 2020 2020 206c  ',.            l
+00026a90: 773d 302c 0a20 2020 2020 2020 2020 2020  w=0,.           
+00026aa0: 2065 6c69 6e65 7769 6474 683d 312e 352c   elinewidth=1.5,
+00026ab0: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
+00026ac0: 6c73 7479 6c65 3d27 6e6f 6e65 272c 0a20  lstyle='none',. 
+00026ad0: 2020 2020 2020 2020 2020 2063 6f6c 6f72             color
+00026ae0: 3d27 626c 6163 6b27 0a20 2020 2020 2020  ='black'.       
+00026af0: 2029 0a20 2020 2065 6c73 653a 0a20 2020   ).    else:.   
+00026b00: 2020 2020 2061 782e 706c 6f74 280a 2020       ax.plot(.  
+00026b10: 2020 2020 2020 2020 2020 785f 7661 6c73            x_vals
+00026b20: 2c0a 2020 2020 2020 2020 2020 2020 6461  ,.            da
+00026b30: 7461 7365 742e 7261 7465 732c 0a20 2020  taset.rates,.   
+00026b40: 2020 2020 2020 2020 206d 6172 6b65 723d           marker=
+00026b50: 276f 272c 0a20 2020 2020 2020 2020 2020  'o',.           
+00026b60: 206c 773d 302c 0a20 2020 2020 2020 2020   lw=0,.         
+00026b70: 2020 2066 696c 6c73 7479 6c65 3d27 6e6f     fillstyle='no
+00026b80: 6e65 272c 0a20 2020 2020 2020 2020 2020  ne',.           
+00026b90: 2063 6f6c 6f72 3d27 626c 6163 6b27 0a20   color='black'. 
+00026ba0: 2020 2020 2020 2029 0a0a 2020 2020 6966         )..    if
+00026bb0: 2078 5f74 7970 6520 3d3d 2027 6669 656c   x_type == 'fiel
+00026bc0: 6427 3a0a 2020 2020 2020 2020 6966 2061  d':.        if a
+00026bd0: 6e79 2876 616c 203c 206e 702e 6669 6e66  ny(val < np.finf
+00026be0: 6f28 666c 6f61 7429 2e65 7073 2066 6f72  o(float).eps for
+00026bf0: 2076 616c 2069 6e20 785f 7661 6c73 293a   val in x_vals):
+00026c00: 0a20 2020 2020 2020 2020 2020 2061 782e  .            ax.
+00026c10: 7365 745f 7873 6361 6c65 280a 2020 2020  set_xscale(.    
+00026c20: 2020 2020 2020 2020 2020 2020 2773 796d              'sym
+00026c30: 6c6f 6727 2c0a 2020 2020 2020 2020 2020  log',.          
+00026c40: 2020 2020 2020 6c69 6e74 6872 6573 683d        linthresh=
+00026c50: 6775 692e 6361 6c63 5f6c 696e 7468 7265  gui.calc_linthre
+00026c60: 7368 2878 5f76 616c 7329 2c0a 2020 2020  sh(x_vals),.    
+00026c70: 2020 2020 2020 2020 2020 2020 6c69 6e73              lins
+00026c80: 6361 6c65 3d67 7569 2e63 616c 635f 6c69  cale=gui.calc_li
+00026c90: 6e73 6361 6c65 2878 5f76 616c 7329 0a20  nscale(x_vals). 
+00026ca0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00026cb0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00026cc0: 2020 2020 2020 2061 782e 7365 745f 7873         ax.set_xs
+00026cd0: 6361 6c65 2827 6c6f 6727 290a 2020 2020  cale('log').    
+00026ce0: 656c 7365 3a0a 2020 2020 2020 2020 6178  else:.        ax
+00026cf0: 2e73 6574 5f78 7363 616c 6528 276c 6f67  .set_xscale('log
+00026d00: 2729 0a20 2020 2061 782e 7365 745f 7973  ').    ax.set_ys
+00026d10: 6361 6c65 2827 6c6f 6727 290a 0a20 2020  cale('log')..   
+00026d20: 2061 782e 7365 745f 796c 6162 656c 2872   ax.set_ylabel(r
+00026d30: 2752 6174 6520 2873 245e 5c6d 6174 6872  'Rate (s$^\mathr
+00026d40: 6567 756c 6172 7b2d 317d 2429 2729 0a0a  egular{-1}$)')..
+00026d50: 2020 2020 6966 206c 656e 2864 6174 6173      if len(datas
+00026d60: 6574 2e6c 6f67 7261 7465 5f70 6d29 3a0a  et.lograte_pm):.
+00026d70: 2020 2020 2020 2020 616c 6c5f 6461 7461          all_data
+00026d80: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
+00026d90: 206e 702e 6c6f 6731 3028 6461 7461 7365   np.log10(datase
+00026da0: 742e 7261 7465 7329 202b 2064 6174 6173  t.rates) + datas
+00026db0: 6574 2e6c 6f67 7261 7465 5f70 6d0a 2020  et.lograte_pm.  
+00026dc0: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
+00026dd0: 616c 6c5f 6461 7461 202b 3d20 5b0a 2020  all_data += [.  
+00026de0: 2020 2020 2020 2020 2020 6e70 2e6c 6f67            np.log
+00026df0: 3130 2864 6174 6173 6574 2e72 6174 6573  10(dataset.rates
+00026e00: 2920 2d20 6461 7461 7365 742e 6c6f 6772  ) - dataset.logr
+00026e10: 6174 655f 706d 0a20 2020 2020 2020 205d  ate_pm.        ]
+00026e20: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00026e30: 2020 2061 6c6c 5f64 6174 6120 3d20 5b0a     all_data = [.
+00026e40: 2020 2020 2020 2020 2020 2020 6e70 2e6c              np.l
+00026e50: 6f67 3130 2864 6174 6173 6574 2e72 6174  og10(dataset.rat
+00026e60: 6573 290a 2020 2020 2020 2020 5d0a 2020  es).        ].  
+00026e70: 2020 2020 2020 616c 6c5f 6461 7461 202b        all_data +
+00026e80: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
+00026e90: 6e70 2e6c 6f67 3130 2864 6174 6173 6574  np.log10(dataset
+00026ea0: 2e72 6174 6573 290a 2020 2020 2020 2020  .rates).        
+00026eb0: 5d0a 0a20 2020 2067 7569 2e66 6f72 6d61  ]..    gui.forma
+00026ec0: 745f 7261 7465 5f78 5f79 5f61 7865 7328  t_rate_x_y_axes(
+00026ed0: 0a20 2020 2020 2020 2061 782c 0a20 2020  .        ax,.   
+00026ee0: 2020 2020 2064 6174 6173 6574 2e72 6174       dataset.rat
+00026ef0: 6573 2c0a 2020 2020 2020 2020 785f 7661  es,.        x_va
+00026f00: 6c73 2c0a 2020 2020 2020 2020 6e70 2e61  ls,.        np.a
+00026f10: 6273 2864 6174 6173 6574 2e72 6174 655f  bs(dataset.rate_
+00026f20: 706d 292c 0a20 2020 2020 2020 2078 5f74  pm),.        x_t
+00026f30: 7970 653d 785f 7479 7065 0a20 2020 2029  ype=x_type.    )
+00026f40: 0a0a 2020 2020 2320 5365 7420 7820 7469  ..    # Set x ti
+00026f50: 636b 2066 6f72 6d61 7474 696e 670a 2020  ck formatting.  
+00026f60: 2020 6775 692e 7365 745f 7261 7465 5f78    gui.set_rate_x
+00026f70: 7469 636b 5f66 6f72 6d61 7474 696e 6728  tick_formatting(
+00026f80: 6178 2c20 785f 7661 6c73 2c20 785f 7479  ax, x_vals, x_ty
+00026f90: 7065 3d78 5f74 7970 6529 0a0a 2020 2020  pe=x_type)..    
+00026fa0: 6669 672e 7469 6768 745f 6c61 796f 7574  fig.tight_layout
+00026fb0: 2829 0a0a 2020 2020 2320 5375 7070 7265  ()..    # Suppre
+00026fc0: 7373 2073 796d 6c6f 6720 7761 726e 696e  ss symlog warnin
+00026fd0: 670a 2020 2020 7761 726e 696e 6773 2e73  g.    warnings.s
+00026fe0: 696d 706c 6566 696c 7465 7228 2769 676e  implefilter('ign
+00026ff0: 6f72 6527 2c20 5573 6572 5761 726e 696e  ore', UserWarnin
+00027000: 6729 0a0a 2020 2020 6966 2073 6176 653a  g)..    if save:
+00027010: 0a20 2020 2020 2020 2070 6c74 2e73 6176  .        plt.sav
+00027020: 6566 6967 2873 6176 655f 6e61 6d65 290a  efig(save_name).
+00027030: 2020 2020 2020 2020 6966 2076 6572 626f          if verbo
+00027040: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00027050: 7574 2e63 7072 696e 7428 0a20 2020 2020  ut.cprint(.     
+00027060: 2020 2020 2020 2020 2020 2066 275c 6e20             f'\n 
+00027070: 5265 6c61 7861 7469 6f6e 2070 6c6f 7420  Relaxation plot 
+00027080: 7361 7665 6420 746f 205c 6e20 7b73 6176  saved to \n {sav
+00027090: 655f 6e61 6d65 7d5c 6e27 2c0a 2020 2020  e_name}\n',.    
+000270a0: 2020 2020 2020 2020 2020 2020 2763 7961              'cya
+000270b0: 6e27 0a20 2020 2020 2020 2020 2020 2029  n'.            )
+000270c0: 0a20 2020 2069 6620 7368 6f77 3a0a 2020  .    if show:.  
+000270d0: 2020 2020 2020 706c 742e 7368 6f77 2829        plt.show()
+000270e0: 0a0a 2020 2020 2320 5265 656e 6162 6c65  ..    # Reenable
+000270f0: 2073 796d 6c6f 6720 7761 726e 696e 670a   symlog warning.
+00027100: 2020 2020 7761 726e 696e 6773 2e73 696d      warnings.sim
+00027110: 706c 6566 696c 7465 7228 2764 6566 6175  plefilter('defau
+00027120: 6c74 272c 2055 7365 7257 6172 6e69 6e67  lt', UserWarning
+00027130: 290a 0a20 2020 2072 6574 7572 6e20 6669  )..    return fi
+00027140: 672c 2061 780a 0a0a 6465 6620 706c 6f74  g, ax...def plot
+00027150: 5f72 6174 655f 7265 7369 6475 616c 7328  _rate_residuals(
+00027160: 6461 7461 7365 743a 2054 6175 5444 6174  dataset: TauTDat
+00027170: 6173 6574 2c0a 2020 2020 2020 2020 2020  aset,.          
+00027180: 2020 2020 2020 2020 2020 2020 2020 6d6f                mo
+00027190: 6465 6c3a 204c 6f67 5461 7554 4d6f 6465  del: LogTauTMode
+000271a0: 6c20 7c20 4d75 6c74 694c 6f67 5461 7554  l | MultiLogTauT
+000271b0: 4d6f 6465 6c20 7c20 4c6f 6754 6175 484d  Model | LogTauHM
+000271c0: 6f64 656c 207c 204d 756c 7469 4c6f 6754  odel | MultiLogT
+000271d0: 6175 484d 6f64 656c 2c20 2320 6e6f 7161  auHModel, # noqa
+000271e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000271f0: 2020 2020 2020 2020 2073 6176 653a 2062           save: b
+00027200: 6f6f 6c20 3d20 4661 6c73 652c 2073 686f  ool = False, sho
+00027210: 773a 2062 6f6f 6c20 3d20 5472 7565 2c0a  w: bool = True,.
 00027220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027230: 2020 2020 7361 7665 5f6e 616d 653a 2073      save_name: s
-00027240: 7472 203d 2027 6d6f 6465 6c5f 7265 7369  tr = 'model_resi
-00027250: 6475 616c 5f74 6175 2e70 6e67 272c 0a20  dual_tau.png',. 
-00027260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027270: 2020 2020 2020 2076 6572 626f 7365 3a20         verbose: 
-00027280: 626f 6f6c 203d 2054 7275 6529 202d 3e20  bool = True) -> 
-00027290: 7475 706c 655b 706c 742e 4669 6775 7265  tuple[plt.Figure
-000272a0: 2c20 706c 742e 4178 6573 5d3a 0a20 2020  , plt.Axes]:.   
-000272b0: 2027 2727 0a20 2020 2050 6c6f 7473 2064   '''.    Plots d
-000272c0: 6966 6665 7265 6e63 6520 6f66 206c 6f67  ifference of log
-000272d0: 3130 2865 7870 6572 696d 656e 7429 2061  10(experiment) a
-000272e0: 6e64 206c 6f67 3130 286d 6f64 656c 2920  nd log10(model) 
-000272f0: 7265 6c61 7861 7469 6f6e 2072 6174 6573  relaxation rates
-00027300: 0a20 2020 2028 6c6f 6731 3028 6578 7065  .    (log10(expe
-00027310: 7269 6d65 6e74 5f72 6174 6529 202d 206c  riment_rate) - l
-00027320: 6f67 3130 286d 6f64 656c 5f72 6174 6529  og10(model_rate)
-00027330: 2076 7320 5465 6d70 6572 6174 7572 6520   vs Temperature 
-00027340: 6f72 2046 6965 6c64 290a 0a20 2020 2050  or Field)..    P
-00027350: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
-00027360: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064 6174  --------.    dat
-00027370: 6173 6574 3a20 5461 7554 4461 7461 7365  aset: TauTDatase
-00027380: 7420 7c20 5461 7548 4461 7461 7365 740a  t | TauHDataset.
-00027390: 2020 2020 2020 2020 4461 7461 7365 7420          Dataset 
-000273a0: 746f 2070 6c6f 740a 2020 2020 6d6f 6465  to plot.    mode
-000273b0: 6c3a 204c 6f67 5461 7554 4d6f 6465 6c20  l: LogTauTModel 
-000273c0: 7c20 4d75 6c74 694c 6f67 5461 7554 4d6f  | MultiLogTauTMo
-000273d0: 6465 6c20 7c20 4c6f 6754 6175 484d 6f64  del | LogTauHMod
-000273e0: 656c 207c 204d 756c 7469 4c6f 6754 6175  el | MultiLogTau
-000273f0: 484d 6f64 656c 0a20 2020 2020 2020 204d  HModel.        M
-00027400: 6f64 656c 2028 6669 7474 6564 2920 746f  odel (fitted) to
-00027410: 2070 6c6f 740a 2020 2020 7368 6f77 3a20   plot.    show: 
-00027420: 626f 6f6c 2c20 6465 6661 756c 7420 5472  bool, default Tr
-00027430: 7565 0a20 2020 2020 2020 2049 6620 5472  ue.        If Tr
-00027440: 7565 2c20 7368 6f77 2070 6c6f 7420 6f6e  ue, show plot on
-00027450: 2073 6372 6565 6e0a 2020 2020 7361 7665   screen.    save
-00027460: 3a20 626f 6f6c 2c20 6465 6661 756c 7420  : bool, default 
-00027470: 4661 6c73 650a 2020 2020 2020 2020 4966  False.        If
-00027480: 2054 7275 652c 2073 6176 6520 706c 6f74   True, save plot
-00027490: 2074 6f20 6669 6c65 2060 7361 7665 5f6e   to file `save_n
-000274a0: 616d 6560 0a20 2020 2073 6176 655f 6e61  ame`.    save_na
-000274b0: 6d65 3a20 7374 722c 2064 6566 6175 6c74  me: str, default
-000274c0: 2027 6d6f 6465 6c5f 7265 7369 6475 616c   'model_residual
-000274d0: 5f74 6175 2e70 6e67 270a 2020 2020 2020  _tau.png'.      
-000274e0: 2020 4966 2073 6176 6520 6973 2054 7275    If save is Tru
-000274f0: 652c 2077 696c 6c20 7361 7665 2070 6c6f  e, will save plo
-00027500: 7420 746f 2074 6869 7320 6669 6c65 6e61  t to this filena
-00027510: 6d65 0a20 2020 2076 6572 626f 7365 3a20  me.    verbose: 
-00027520: 626f 6f6c 2c20 6465 6661 756c 7420 5472  bool, default Tr
-00027530: 7565 0a20 2020 2020 2020 2049 6620 5472  ue.        If Tr
-00027540: 7565 2c20 706c 6f74 2066 696c 6520 6c6f  ue, plot file lo
-00027550: 6361 7469 6f6e 2069 7320 7772 6974 7465  cation is writte
-00027560: 6e20 746f 2074 6572 6d69 6e61 6c0a 0a20  n to terminal.. 
-00027570: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
-00027580: 2d2d 2d2d 2d2d 0a20 2020 2070 6c74 2e46  ------.    plt.F
-00027590: 6967 7572 650a 2020 2020 2020 2020 4d61  igure.        Ma
-000275a0: 7470 6c6f 746c 6962 2066 6967 7572 6520  tplotlib figure 
-000275b0: 6f62 6a65 6374 0a20 2020 2070 6c74 2e41  object.    plt.A
-000275c0: 7865 730a 2020 2020 2020 2020 4d61 7470  xes.        Matp
-000275d0: 6c6f 746c 6962 2061 7869 7320 6f62 6a65  lotlib axis obje
-000275e0: 6374 0a20 2020 2027 2727 0a20 2020 2023  ct.    '''.    #
-000275f0: 2043 7265 6174 6520 6669 6775 7265 2061   Create figure a
-00027600: 6e64 2061 7865 730a 2020 2020 6669 672c  nd axes.    fig,
-00027610: 2061 7820 3d20 706c 742e 7375 6270 6c6f   ax = plt.subplo
-00027620: 7473 280a 2020 2020 2020 2020 312c 0a20  ts(.        1,. 
-00027630: 2020 2020 2020 2031 2c0a 2020 2020 2020         1,.      
-00027640: 2020 6669 6773 697a 653d 5b36 2c20 365d    figsize=[6, 6]
-00027650: 2c0a 2020 2020 2020 2020 6e75 6d3d 2752  ,.        num='R
-00027660: 6573 6964 7561 6c73 270a 2020 2020 290a  esiduals'.    ).
-00027670: 0a20 2020 205f 706c 6f74 5f72 6174 655f  .    _plot_rate_
-00027680: 7265 7369 6475 616c 7328 6461 7461 7365  residuals(datase
-00027690: 742c 206d 6f64 656c 2c20 6178 290a 0a20  t, model, ax).. 
-000276a0: 2020 2066 6967 2e74 6967 6874 5f6c 6179     fig.tight_lay
-000276b0: 6f75 7428 290a 0a20 2020 2077 6172 6e69  out()..    warni
-000276c0: 6e67 732e 7369 6d70 6c65 6669 6c74 6572  ngs.simplefilter
-000276d0: 2827 6967 6e6f 7265 272c 2055 7365 7257  ('ignore', UserW
-000276e0: 6172 6e69 6e67 290a 2020 2020 2320 5361  arning).    # Sa
-000276f0: 7665 2070 6c6f 740a 2020 2020 6966 2073  ve plot.    if s
-00027700: 6176 653a 0a20 2020 2020 2020 2070 6c74  ave:.        plt
-00027710: 2e73 6176 6566 6967 2873 6176 655f 6e61  .savefig(save_na
-00027720: 6d65 2c20 6470 693d 3330 3029 0a20 2020  me, dpi=300).   
-00027730: 2020 2020 2069 6620 7665 7262 6f73 653a       if verbose:
-00027740: 0a20 2020 2020 2020 2020 2020 2075 742e  .            ut.
-00027750: 6370 7269 6e74 280a 2020 2020 2020 2020  cprint(.        
-00027760: 2020 2020 2020 2020 6627 5c6e 2052 6174          f'\n Rat
-00027770: 6520 7265 7369 6475 616c 7320 706c 6f74  e residuals plot
-00027780: 2073 6176 6564 2074 6f20 5c6e 207b 7361   saved to \n {sa
-00027790: 7665 5f6e 616d 657d 5c6e 272c 0a20 2020  ve_name}\n',.   
-000277a0: 2020 2020 2020 2020 2020 2020 2027 6379               'cy
-000277b0: 616e 270a 2020 2020 2020 2020 2020 2020  an'.            
-000277c0: 290a 2020 2020 6966 2073 686f 773a 0a20  ).    if show:. 
-000277d0: 2020 2020 2020 2070 6c74 2e73 686f 7728         plt.show(
-000277e0: 290a 2020 2020 7761 726e 696e 6773 2e73  ).    warnings.s
-000277f0: 696d 706c 6566 696c 7465 7228 2764 6566  implefilter('def
-00027800: 6175 6c74 272c 2055 7365 7257 6172 6e69  ault', UserWarni
-00027810: 6e67 290a 0a20 2020 2072 6574 7572 6e20  ng)..    return 
-00027820: 6669 672c 2061 780a 0a0a 6465 6620 7174  fig, ax...def qt
-00027830: 5f70 6c6f 745f 7261 7465 5f72 6573 6964  _plot_rate_resid
-00027840: 7561 6c73 2861 7070 3a20 5174 5769 6467  uals(app: QtWidg
-00027850: 6574 732e 5141 7070 6c69 6361 7469 6f6e  ets.QApplication
-00027860: 2c20 6461 7461 7365 743a 2054 6175 5444  , dataset: TauTD
-00027870: 6174 6173 6574 2c0a 2020 2020 2020 2020  ataset,.        
+00027230: 2020 2020 2020 2020 7361 7665 5f6e 616d          save_nam
+00027240: 653a 2073 7472 203d 2027 6d6f 6465 6c5f  e: str = 'model_
+00027250: 7265 7369 6475 616c 5f74 6175 2e70 6e67  residual_tau.png
+00027260: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00027270: 2020 2020 2020 2020 2020 2076 6572 626f             verbo
+00027280: 7365 3a20 626f 6f6c 203d 2054 7275 6529  se: bool = True)
+00027290: 202d 3e20 7475 706c 655b 706c 742e 4669   -> tuple[plt.Fi
+000272a0: 6775 7265 2c20 706c 742e 4178 6573 5d3a  gure, plt.Axes]:
+000272b0: 0a20 2020 2027 2727 0a20 2020 2050 6c6f  .    '''.    Plo
+000272c0: 7473 2064 6966 6665 7265 6e63 6520 6f66  ts difference of
+000272d0: 206c 6f67 3130 2865 7870 6572 696d 656e   log10(experimen
+000272e0: 7429 2061 6e64 206c 6f67 3130 286d 6f64  t) and log10(mod
+000272f0: 656c 2920 7265 6c61 7861 7469 6f6e 2072  el) relaxation r
+00027300: 6174 6573 0a20 2020 2028 6c6f 6731 3028  ates.    (log10(
+00027310: 6578 7065 7269 6d65 6e74 5f72 6174 6529  experiment_rate)
+00027320: 202d 206c 6f67 3130 286d 6f64 656c 5f72   - log10(model_r
+00027330: 6174 6529 2076 7320 5465 6d70 6572 6174  ate) vs Temperat
+00027340: 7572 6520 6f72 2046 6965 6c64 290a 0a20  ure or Field).. 
+00027350: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00027360: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00027370: 2064 6174 6173 6574 3a20 5461 7554 4461   dataset: TauTDa
+00027380: 7461 7365 7420 7c20 5461 7548 4461 7461  taset | TauHData
+00027390: 7365 740a 2020 2020 2020 2020 4461 7461  set.        Data
+000273a0: 7365 7420 746f 2070 6c6f 740a 2020 2020  set to plot.    
+000273b0: 6d6f 6465 6c3a 204c 6f67 5461 7554 4d6f  model: LogTauTMo
+000273c0: 6465 6c20 7c20 4d75 6c74 694c 6f67 5461  del | MultiLogTa
+000273d0: 7554 4d6f 6465 6c20 7c20 4c6f 6754 6175  uTModel | LogTau
+000273e0: 484d 6f64 656c 207c 204d 756c 7469 4c6f  HModel | MultiLo
+000273f0: 6754 6175 484d 6f64 656c 0a20 2020 2020  gTauHModel.     
+00027400: 2020 204d 6f64 656c 2028 6669 7474 6564     Model (fitted
+00027410: 2920 746f 2070 6c6f 740a 2020 2020 7368  ) to plot.    sh
+00027420: 6f77 3a20 626f 6f6c 2c20 6465 6661 756c  ow: bool, defaul
+00027430: 7420 5472 7565 0a20 2020 2020 2020 2049  t True.        I
+00027440: 6620 5472 7565 2c20 7368 6f77 2070 6c6f  f True, show plo
+00027450: 7420 6f6e 2073 6372 6565 6e0a 2020 2020  t on screen.    
+00027460: 7361 7665 3a20 626f 6f6c 2c20 6465 6661  save: bool, defa
+00027470: 756c 7420 4661 6c73 650a 2020 2020 2020  ult False.      
+00027480: 2020 4966 2054 7275 652c 2073 6176 6520    If True, save 
+00027490: 706c 6f74 2074 6f20 6669 6c65 2060 7361  plot to file `sa
+000274a0: 7665 5f6e 616d 6560 0a20 2020 2073 6176  ve_name`.    sav
+000274b0: 655f 6e61 6d65 3a20 7374 722c 2064 6566  e_name: str, def
+000274c0: 6175 6c74 2027 6d6f 6465 6c5f 7265 7369  ault 'model_resi
+000274d0: 6475 616c 5f74 6175 2e70 6e67 270a 2020  dual_tau.png'.  
+000274e0: 2020 2020 2020 4966 2073 6176 6520 6973        If save is
+000274f0: 2054 7275 652c 2077 696c 6c20 7361 7665   True, will save
+00027500: 2070 6c6f 7420 746f 2074 6869 7320 6669   plot to this fi
+00027510: 6c65 6e61 6d65 0a20 2020 2076 6572 626f  lename.    verbo
+00027520: 7365 3a20 626f 6f6c 2c20 6465 6661 756c  se: bool, defaul
+00027530: 7420 5472 7565 0a20 2020 2020 2020 2049  t True.        I
+00027540: 6620 5472 7565 2c20 706c 6f74 2066 696c  f True, plot fil
+00027550: 6520 6c6f 6361 7469 6f6e 2069 7320 7772  e location is wr
+00027560: 6974 7465 6e20 746f 2074 6572 6d69 6e61  itten to termina
+00027570: 6c0a 0a20 2020 2052 6574 7572 6e73 0a20  l..    Returns. 
+00027580: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2070     -------.    p
+00027590: 6c74 2e46 6967 7572 650a 2020 2020 2020  lt.Figure.      
+000275a0: 2020 4d61 7470 6c6f 746c 6962 2066 6967    Matplotlib fig
+000275b0: 7572 6520 6f62 6a65 6374 0a20 2020 2070  ure object.    p
+000275c0: 6c74 2e41 7865 730a 2020 2020 2020 2020  lt.Axes.        
+000275d0: 4d61 7470 6c6f 746c 6962 2061 7869 7320  Matplotlib axis 
+000275e0: 6f62 6a65 6374 0a20 2020 2027 2727 0a20  object.    '''. 
+000275f0: 2020 2023 2043 7265 6174 6520 6669 6775     # Create figu
+00027600: 7265 2061 6e64 2061 7865 730a 2020 2020  re and axes.    
+00027610: 6669 672c 2061 7820 3d20 706c 742e 7375  fig, ax = plt.su
+00027620: 6270 6c6f 7473 280a 2020 2020 2020 2020  bplots(.        
+00027630: 312c 0a20 2020 2020 2020 2031 2c0a 2020  1,.        1,.  
+00027640: 2020 2020 2020 6669 6773 697a 653d 5b36        figsize=[6
+00027650: 2c20 365d 2c0a 2020 2020 2020 2020 6e75  , 6],.        nu
+00027660: 6d3d 2752 6573 6964 7561 6c73 270a 2020  m='Residuals'.  
+00027670: 2020 290a 0a20 2020 205f 706c 6f74 5f72    )..    _plot_r
+00027680: 6174 655f 7265 7369 6475 616c 7328 6461  ate_residuals(da
+00027690: 7461 7365 742c 206d 6f64 656c 2c20 6178  taset, model, ax
+000276a0: 290a 0a20 2020 2066 6967 2e74 6967 6874  )..    fig.tight
+000276b0: 5f6c 6179 6f75 7428 290a 0a20 2020 2077  _layout()..    w
+000276c0: 6172 6e69 6e67 732e 7369 6d70 6c65 6669  arnings.simplefi
+000276d0: 6c74 6572 2827 6967 6e6f 7265 272c 2055  lter('ignore', U
+000276e0: 7365 7257 6172 6e69 6e67 290a 2020 2020  serWarning).    
+000276f0: 2320 5361 7665 2070 6c6f 740a 2020 2020  # Save plot.    
+00027700: 6966 2073 6176 653a 0a20 2020 2020 2020  if save:.       
+00027710: 2070 6c74 2e73 6176 6566 6967 2873 6176   plt.savefig(sav
+00027720: 655f 6e61 6d65 2c20 6470 693d 3330 3029  e_name, dpi=300)
+00027730: 0a20 2020 2020 2020 2069 6620 7665 7262  .        if verb
+00027740: 6f73 653a 0a20 2020 2020 2020 2020 2020  ose:.           
+00027750: 2075 742e 6370 7269 6e74 280a 2020 2020   ut.cprint(.    
+00027760: 2020 2020 2020 2020 2020 2020 6627 5c6e              f'\n
+00027770: 2052 6174 6520 7265 7369 6475 616c 7320   Rate residuals 
+00027780: 706c 6f74 2073 6176 6564 2074 6f20 5c6e  plot saved to \n
+00027790: 207b 7361 7665 5f6e 616d 657d 5c6e 272c   {save_name}\n',
+000277a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000277b0: 2027 6379 616e 270a 2020 2020 2020 2020   'cyan'.        
+000277c0: 2020 2020 290a 2020 2020 6966 2073 686f      ).    if sho
+000277d0: 773a 0a20 2020 2020 2020 2070 6c74 2e73  w:.        plt.s
+000277e0: 686f 7728 290a 2020 2020 7761 726e 696e  how().    warnin
+000277f0: 6773 2e73 696d 706c 6566 696c 7465 7228  gs.simplefilter(
+00027800: 2764 6566 6175 6c74 272c 2055 7365 7257  'default', UserW
+00027810: 6172 6e69 6e67 290a 0a20 2020 2072 6574  arning)..    ret
+00027820: 7572 6e20 6669 672c 2061 780a 0a0a 6465  urn fig, ax...de
+00027830: 6620 7174 5f70 6c6f 745f 7261 7465 5f72  f qt_plot_rate_r
+00027840: 6573 6964 7561 6c73 2861 7070 3a20 5174  esiduals(app: Qt
+00027850: 5769 6467 6574 732e 5141 7070 6c69 6361  Widgets.QApplica
+00027860: 7469 6f6e 2c20 6461 7461 7365 743a 2054  tion, dataset: T
+00027870: 6175 5444 6174 6173 6574 2c0a 2020 2020  auTDataset,.    
 00027880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027890: 2020 206d 6f64 656c 3a20 4c6f 6754 6175     model: LogTau
-000278a0: 544d 6f64 656c 207c 204d 756c 7469 4c6f  TModel | MultiLo
-000278b0: 6754 6175 544d 6f64 656c 207c 204c 6f67  gTauTModel | Log
-000278c0: 5461 7548 4d6f 6465 6c20 7c20 4d75 6c74  TauHModel | Mult
-000278d0: 694c 6f67 5461 7548 4d6f 6465 6c2c 2023  iLogTauHModel, #
-000278e0: 206e 6f71 610a 2020 2020 2020 2020 2020   noqa.          
+00027890: 2020 2020 2020 206d 6f64 656c 3a20 4c6f         model: Lo
+000278a0: 6754 6175 544d 6f64 656c 207c 204d 756c  gTauTModel | Mul
+000278b0: 7469 4c6f 6754 6175 544d 6f64 656c 207c  tiLogTauTModel |
+000278c0: 204c 6f67 5461 7548 4d6f 6465 6c20 7c20   LogTauHModel | 
+000278d0: 4d75 6c74 694c 6f67 5461 7548 4d6f 6465  MultiLogTauHMode
+000278e0: 6c2c 2023 206e 6f71 610a 2020 2020 2020  l, # noqa.      
 000278f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027900: 2073 6176 653a 2062 6f6f 6c20 3d20 4661   save: bool = Fa
-00027910: 6c73 652c 2073 686f 773a 2062 6f6f 6c20  lse, show: bool 
-00027920: 3d20 5472 7565 2c0a 2020 2020 2020 2020  = True,.        
+00027900: 2020 2020 2073 6176 653a 2062 6f6f 6c20       save: bool 
+00027910: 3d20 4661 6c73 652c 2073 686f 773a 2062  = False, show: b
+00027920: 6f6f 6c20 3d20 5472 7565 2c0a 2020 2020  ool = True,.    
 00027930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027940: 2020 2073 6176 655f 6e61 6d65 3a20 7374     save_name: st
-00027950: 7220 3d20 276d 6f64 656c 5f72 6573 6964  r = 'model_resid
-00027960: 7561 6c5f 7461 752e 706e 6727 2c0a 2020  ual_tau.png',.  
-00027970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027980: 2020 2020 2020 2020 2076 6572 626f 7365           verbose
-00027990: 3a20 626f 6f6c 203d 2054 7275 6529 202d  : bool = True) -
-000279a0: 3e20 4e6f 6e65 3a0a 2020 2020 2727 270a  > None:.    '''.
-000279b0: 2020 2020 506c 6f74 7320 6469 6666 6572      Plots differ
-000279c0: 656e 6365 206f 6620 6c6f 6731 3028 6578  ence of log10(ex
-000279d0: 7065 7269 6d65 6e74 2920 616e 6420 6c6f  periment) and lo
-000279e0: 6731 3028 6d6f 6465 6c29 2072 656c 6178  g10(model) relax
-000279f0: 6174 696f 6e20 7261 7465 730a 2020 2020  ation rates.    
-00027a00: 696e 2061 2071 7420 7769 6e64 6f77 2075  in a qt window u
-00027a10: 7369 6e67 206d 6174 706c 6f74 6c69 620a  sing matplotlib.
-00027a20: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
-00027a30: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00027a40: 2020 2061 7070 3a20 5174 5769 6467 6574     app: QtWidget
-00027a50: 732e 5141 7070 6c69 6361 7469 6f6e 0a20  s.QApplication. 
-00027a60: 2020 2020 2020 2041 7070 6c69 6361 7469         Applicati
-00027a70: 6f6e 2075 7365 6420 6279 2063 7572 7265  on used by curre
-00027a80: 6e74 2070 726f 6772 616d 0a20 2020 2020  nt program.     
-00027a90: 2020 2043 7265 6174 6520 7769 7468 2060     Create with `
-00027aa0: 6170 703d 5174 5769 6467 6574 732e 5141  app=QtWidgets.QA
-00027ab0: 7070 6c69 6361 7469 6f6e 285b 5d29 600a  pplication([])`.
-00027ac0: 2020 2020 6461 7461 7365 743a 2054 6175      dataset: Tau
-00027ad0: 5444 6174 6173 6574 207c 2054 6175 4844  TDataset | TauHD
-00027ae0: 6174 6173 6574 0a20 2020 2020 2020 2044  ataset.        D
-00027af0: 6174 6173 6574 2074 6f20 706c 6f74 0a20  ataset to plot. 
-00027b00: 2020 206d 6f64 656c 3a20 4c6f 6754 6175     model: LogTau
-00027b10: 544d 6f64 656c 207c 204d 756c 7469 4c6f  TModel | MultiLo
-00027b20: 6754 6175 544d 6f64 656c 207c 204c 6f67  gTauTModel | Log
-00027b30: 5461 7548 4d6f 6465 6c20 7c20 4d75 6c74  TauHModel | Mult
-00027b40: 694c 6f67 5461 7548 4d6f 6465 6c0a 2020  iLogTauHModel.  
-00027b50: 2020 2020 2020 4d6f 6465 6c20 2866 6974        Model (fit
-00027b60: 7465 6429 2074 6f20 706c 6f74 0a20 2020  ted) to plot.   
-00027b70: 2073 686f 773a 2062 6f6f 6c2c 2064 6566   show: bool, def
-00027b80: 6175 6c74 2054 7275 650a 2020 2020 2020  ault True.      
-00027b90: 2020 4966 2054 7275 652c 2073 686f 7720    If True, show 
-00027ba0: 706c 6f74 206f 6e20 7363 7265 656e 0a20  plot on screen. 
-00027bb0: 2020 2073 6176 653a 2062 6f6f 6c2c 2064     save: bool, d
-00027bc0: 6566 6175 6c74 2046 616c 7365 0a20 2020  efault False.   
-00027bd0: 2020 2020 2049 6620 5472 7565 2c20 7361       If True, sa
-00027be0: 7665 2070 6c6f 7420 746f 2066 696c 6520  ve plot to file 
-00027bf0: 6073 6176 655f 6e61 6d65 600a 2020 2020  `save_name`.    
-00027c00: 7361 7665 5f6e 616d 653a 2073 7472 2c20  save_name: str, 
-00027c10: 6465 6661 756c 7420 276d 6f64 656c 5f72  default 'model_r
-00027c20: 6573 6964 7561 6c5f 7461 752e 706e 6727  esidual_tau.png'
-00027c30: 0a20 2020 2020 2020 2049 6620 7361 7665  .        If save
-00027c40: 2069 7320 5472 7565 2c20 7769 6c6c 2073   is True, will s
-00027c50: 6176 6520 706c 6f74 2074 6f20 7468 6973  ave plot to this
-00027c60: 2066 696c 656e 616d 650a 2020 2020 7665   filename.    ve
-00027c70: 7262 6f73 653a 2062 6f6f 6c2c 2064 6566  rbose: bool, def
-00027c80: 6175 6c74 2054 7275 650a 2020 2020 2020  ault True.      
-00027c90: 2020 4966 2054 7275 652c 2070 6c6f 7420    If True, plot 
-00027ca0: 6669 6c65 206c 6f63 6174 696f 6e20 6973  file location is
-00027cb0: 2077 7269 7474 656e 2074 6f20 7465 726d   written to term
-00027cc0: 696e 616c 0a0a 2020 2020 5265 7475 726e  inal..    Return
-00027cd0: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
-00027ce0: 2020 4e6f 6e65 0a20 2020 2027 2727 0a0a    None.    '''..
-00027cf0: 2020 2020 7769 6e64 6f77 203d 2067 7569      window = gui
-00027d00: 2e4d 6174 706c 6f74 6c69 6257 696e 646f  .MatplotlibWindo
-00027d10: 7728 290a 2020 2020 7769 6e64 6f77 2e73  w().    window.s
-00027d20: 6574 5769 6e64 6f77 5469 746c 6528 2752  etWindowTitle('R
-00027d30: 6573 6964 7561 6c73 2729 0a0a 2020 2020  esiduals')..    
-00027d40: 5f70 6c6f 745f 7261 7465 5f72 6573 6964  _plot_rate_resid
-00027d50: 7561 6c73 2864 6174 6173 6574 2c20 6d6f  uals(dataset, mo
-00027d60: 6465 6c2c 2077 696e 646f 772e 7363 2e61  del, window.sc.a
-00027d70: 7829 0a0a 2020 2020 2320 5361 7665 2070  x)..    # Save p
-00027d80: 6c6f 740a 2020 2020 6966 2073 6176 653a  lot.    if save:
-00027d90: 0a20 2020 2020 2020 2077 696e 646f 772e  .        window.
-00027da0: 7363 2e66 6967 2e73 6176 6566 6967 2873  sc.fig.savefig(s
-00027db0: 6176 655f 6e61 6d65 2c20 6470 693d 3330  ave_name, dpi=30
-00027dc0: 3029 0a20 2020 2020 2020 2069 6620 7665  0).        if ve
-00027dd0: 7262 6f73 653a 0a20 2020 2020 2020 2020  rbose:.         
-00027de0: 2020 2075 742e 6370 7269 6e74 280a 2020     ut.cprint(.  
-00027df0: 2020 2020 2020 2020 2020 2020 2020 6627                f'
-00027e00: 5c6e 2052 6174 6520 7265 7369 6475 616c  \n Rate residual
-00027e10: 7320 706c 6f74 2073 6176 6564 2074 6f20  s plot saved to 
-00027e20: 5c6e 207b 7361 7665 5f6e 616d 657d 5c6e  \n {save_name}\n
-00027e30: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-00027e40: 2020 2027 6379 616e 270a 2020 2020 2020     'cyan'.      
-00027e50: 2020 2020 2020 290a 0a20 2020 2077 6172        )..    war
-00027e60: 6e69 6e67 732e 7369 6d70 6c65 6669 6c74  nings.simplefilt
-00027e70: 6572 2827 6967 6e6f 7265 272c 2055 7365  er('ignore', Use
-00027e80: 7257 6172 6e69 6e67 290a 2020 2020 6966  rWarning).    if
-00027e90: 2073 686f 773a 0a20 2020 2020 2020 2077   show:.        w
-00027ea0: 696e 646f 772e 7368 6f77 2829 0a20 2020  indow.show().   
-00027eb0: 2020 2020 2023 2043 616c 6c20 7477 6963       # Call twic
-00027ec0: 6520 656c 7365 2069 7420 776f 6e74 2077  e else it wont w
-00027ed0: 6f72 6b21 0a20 2020 2020 2020 2077 696e  ork!.        win
-00027ee0: 646f 772e 7363 2e66 6967 2e74 6967 6874  dow.sc.fig.tight
-00027ef0: 5f6c 6179 6f75 7428 290a 2020 2020 2020  _layout().      
-00027f00: 2020 7769 6e64 6f77 2e73 632e 6669 672e    window.sc.fig.
-00027f10: 7469 6768 745f 6c61 796f 7574 2829 0a20  tight_layout(). 
-00027f20: 2020 2020 2020 2061 7070 2e65 7865 635f         app.exec_
-00027f30: 2829 0a20 2020 2077 6172 6e69 6e67 732e  ().    warnings.
-00027f40: 7369 6d70 6c65 6669 6c74 6572 2827 6967  simplefilter('ig
-00027f50: 6e6f 7265 272c 2055 7365 7257 6172 6e69  nore', UserWarni
-00027f60: 6e67 290a 0a20 2020 2072 6574 7572 6e0a  ng)..    return.
-00027f70: 0a0a 6465 6620 5f70 6c6f 745f 7261 7465  ..def _plot_rate
-00027f80: 5f72 6573 6964 7561 6c73 2864 6174 6173  _residuals(datas
-00027f90: 6574 3a20 5461 7554 4461 7461 7365 7420  et: TauTDataset 
-00027fa0: 7c20 5461 7548 4461 7461 7365 742c 0a20  | TauHDataset,. 
-00027fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027fc0: 2020 2020 2020 2020 6d6f 6465 6c3a 204c          model: L
-00027fd0: 6f67 5461 7554 4d6f 6465 6c20 7c20 4d75  ogTauTModel | Mu
-00027fe0: 6c74 694c 6f67 5461 7554 4d6f 6465 6c20  ltiLogTauTModel 
-00027ff0: 7c20 4c6f 6754 6175 484d 6f64 656c 207c  | LogTauHModel |
-00028000: 204d 756c 7469 4c6f 6754 6175 484d 6f64   MultiLogTauHMod
-00028010: 656c 2c20 2320 6e6f 7161 0a20 2020 2020  el, # noqa.     
+00027940: 2020 2020 2020 2073 6176 655f 6e61 6d65         save_name
+00027950: 3a20 7374 7220 3d20 276d 6f64 656c 5f72  : str = 'model_r
+00027960: 6573 6964 7561 6c5f 7461 752e 706e 6727  esidual_tau.png'
+00027970: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00027980: 2020 2020 2020 2020 2020 2020 2076 6572               ver
+00027990: 626f 7365 3a20 626f 6f6c 203d 2054 7275  bose: bool = Tru
+000279a0: 6529 202d 3e20 4e6f 6e65 3a0a 2020 2020  e) -> None:.    
+000279b0: 2727 270a 2020 2020 506c 6f74 7320 6469  '''.    Plots di
+000279c0: 6666 6572 656e 6365 206f 6620 6c6f 6731  fference of log1
+000279d0: 3028 6578 7065 7269 6d65 6e74 2920 616e  0(experiment) an
+000279e0: 6420 6c6f 6731 3028 6d6f 6465 6c29 2072  d log10(model) r
+000279f0: 656c 6178 6174 696f 6e20 7261 7465 730a  elaxation rates.
+00027a00: 2020 2020 696e 2061 2071 7420 7769 6e64      in a qt wind
+00027a10: 6f77 2075 7369 6e67 206d 6174 706c 6f74  ow using matplot
+00027a20: 6c69 620a 0a20 2020 2050 6172 616d 6574  lib..    Paramet
+00027a30: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
+00027a40: 2d2d 0a20 2020 2061 7070 3a20 5174 5769  --.    app: QtWi
+00027a50: 6467 6574 732e 5141 7070 6c69 6361 7469  dgets.QApplicati
+00027a60: 6f6e 0a20 2020 2020 2020 2041 7070 6c69  on.        Appli
+00027a70: 6361 7469 6f6e 2075 7365 6420 6279 2063  cation used by c
+00027a80: 7572 7265 6e74 2070 726f 6772 616d 0a20  urrent program. 
+00027a90: 2020 2020 2020 2043 7265 6174 6520 7769         Create wi
+00027aa0: 7468 2060 6170 703d 5174 5769 6467 6574  th `app=QtWidget
+00027ab0: 732e 5141 7070 6c69 6361 7469 6f6e 285b  s.QApplication([
+00027ac0: 5d29 600a 2020 2020 6461 7461 7365 743a  ])`.    dataset:
+00027ad0: 2054 6175 5444 6174 6173 6574 207c 2054   TauTDataset | T
+00027ae0: 6175 4844 6174 6173 6574 0a20 2020 2020  auHDataset.     
+00027af0: 2020 2044 6174 6173 6574 2074 6f20 706c     Dataset to pl
+00027b00: 6f74 0a20 2020 206d 6f64 656c 3a20 4c6f  ot.    model: Lo
+00027b10: 6754 6175 544d 6f64 656c 207c 204d 756c  gTauTModel | Mul
+00027b20: 7469 4c6f 6754 6175 544d 6f64 656c 207c  tiLogTauTModel |
+00027b30: 204c 6f67 5461 7548 4d6f 6465 6c20 7c20   LogTauHModel | 
+00027b40: 4d75 6c74 694c 6f67 5461 7548 4d6f 6465  MultiLogTauHMode
+00027b50: 6c0a 2020 2020 2020 2020 4d6f 6465 6c20  l.        Model 
+00027b60: 2866 6974 7465 6429 2074 6f20 706c 6f74  (fitted) to plot
+00027b70: 0a20 2020 2073 686f 773a 2062 6f6f 6c2c  .    show: bool,
+00027b80: 2064 6566 6175 6c74 2054 7275 650a 2020   default True.  
+00027b90: 2020 2020 2020 4966 2054 7275 652c 2073        If True, s
+00027ba0: 686f 7720 706c 6f74 206f 6e20 7363 7265  how plot on scre
+00027bb0: 656e 0a20 2020 2073 6176 653a 2062 6f6f  en.    save: boo
+00027bc0: 6c2c 2064 6566 6175 6c74 2046 616c 7365  l, default False
+00027bd0: 0a20 2020 2020 2020 2049 6620 5472 7565  .        If True
+00027be0: 2c20 7361 7665 2070 6c6f 7420 746f 2066  , save plot to f
+00027bf0: 696c 6520 6073 6176 655f 6e61 6d65 600a  ile `save_name`.
+00027c00: 2020 2020 7361 7665 5f6e 616d 653a 2073      save_name: s
+00027c10: 7472 2c20 6465 6661 756c 7420 276d 6f64  tr, default 'mod
+00027c20: 656c 5f72 6573 6964 7561 6c5f 7461 752e  el_residual_tau.
+00027c30: 706e 6727 0a20 2020 2020 2020 2049 6620  png'.        If 
+00027c40: 7361 7665 2069 7320 5472 7565 2c20 7769  save is True, wi
+00027c50: 6c6c 2073 6176 6520 706c 6f74 2074 6f20  ll save plot to 
+00027c60: 7468 6973 2066 696c 656e 616d 650a 2020  this filename.  
+00027c70: 2020 7665 7262 6f73 653a 2062 6f6f 6c2c    verbose: bool,
+00027c80: 2064 6566 6175 6c74 2054 7275 650a 2020   default True.  
+00027c90: 2020 2020 2020 4966 2054 7275 652c 2070        If True, p
+00027ca0: 6c6f 7420 6669 6c65 206c 6f63 6174 696f  lot file locatio
+00027cb0: 6e20 6973 2077 7269 7474 656e 2074 6f20  n is written to 
+00027cc0: 7465 726d 696e 616c 0a0a 2020 2020 5265  terminal..    Re
+00027cd0: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
+00027ce0: 2d0a 2020 2020 4e6f 6e65 0a20 2020 2027  -.    None.    '
+00027cf0: 2727 0a0a 2020 2020 7769 6e64 6f77 203d  ''..    window =
+00027d00: 2067 7569 2e4d 6174 706c 6f74 6c69 6257   gui.MatplotlibW
+00027d10: 696e 646f 7728 290a 2020 2020 7769 6e64  indow().    wind
+00027d20: 6f77 2e73 6574 5769 6e64 6f77 5469 746c  ow.setWindowTitl
+00027d30: 6528 2752 6573 6964 7561 6c73 2729 0a0a  e('Residuals')..
+00027d40: 2020 2020 5f70 6c6f 745f 7261 7465 5f72      _plot_rate_r
+00027d50: 6573 6964 7561 6c73 2864 6174 6173 6574  esiduals(dataset
+00027d60: 2c20 6d6f 6465 6c2c 2077 696e 646f 772e  , model, window.
+00027d70: 7363 2e61 7829 0a0a 2020 2020 2320 5361  sc.ax)..    # Sa
+00027d80: 7665 2070 6c6f 740a 2020 2020 6966 2073  ve plot.    if s
+00027d90: 6176 653a 0a20 2020 2020 2020 2077 696e  ave:.        win
+00027da0: 646f 772e 7363 2e66 6967 2e73 6176 6566  dow.sc.fig.savef
+00027db0: 6967 2873 6176 655f 6e61 6d65 2c20 6470  ig(save_name, dp
+00027dc0: 693d 3330 3029 0a20 2020 2020 2020 2069  i=300).        i
+00027dd0: 6620 7665 7262 6f73 653a 0a20 2020 2020  f verbose:.     
+00027de0: 2020 2020 2020 2075 742e 6370 7269 6e74         ut.cprint
+00027df0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00027e00: 2020 6627 5c6e 2052 6174 6520 7265 7369    f'\n Rate resi
+00027e10: 6475 616c 7320 706c 6f74 2073 6176 6564  duals plot saved
+00027e20: 2074 6f20 5c6e 207b 7361 7665 5f6e 616d   to \n {save_nam
+00027e30: 657d 5c6e 272c 0a20 2020 2020 2020 2020  e}\n',.         
+00027e40: 2020 2020 2020 2027 6379 616e 270a 2020         'cyan'.  
+00027e50: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+00027e60: 2077 6172 6e69 6e67 732e 7369 6d70 6c65   warnings.simple
+00027e70: 6669 6c74 6572 2827 6967 6e6f 7265 272c  filter('ignore',
+00027e80: 2055 7365 7257 6172 6e69 6e67 290a 2020   UserWarning).  
+00027e90: 2020 6966 2073 686f 773a 0a20 2020 2020    if show:.     
+00027ea0: 2020 2077 696e 646f 772e 7368 6f77 2829     window.show()
+00027eb0: 0a20 2020 2020 2020 2023 2043 616c 6c20  .        # Call 
+00027ec0: 7477 6963 6520 656c 7365 2069 7420 776f  twice else it wo
+00027ed0: 6e74 2077 6f72 6b21 0a20 2020 2020 2020  nt work!.       
+00027ee0: 2077 696e 646f 772e 7363 2e66 6967 2e74   window.sc.fig.t
+00027ef0: 6967 6874 5f6c 6179 6f75 7428 290a 2020  ight_layout().  
+00027f00: 2020 2020 2020 7769 6e64 6f77 2e73 632e        window.sc.
+00027f10: 6669 672e 7469 6768 745f 6c61 796f 7574  fig.tight_layout
+00027f20: 2829 0a20 2020 2020 2020 2061 7070 2e65  ().        app.e
+00027f30: 7865 635f 2829 0a20 2020 2077 6172 6e69  xec_().    warni
+00027f40: 6e67 732e 7369 6d70 6c65 6669 6c74 6572  ngs.simplefilter
+00027f50: 2827 6967 6e6f 7265 272c 2055 7365 7257  ('ignore', UserW
+00027f60: 6172 6e69 6e67 290a 0a20 2020 2072 6574  arning)..    ret
+00027f70: 7572 6e0a 0a0a 6465 6620 5f70 6c6f 745f  urn...def _plot_
+00027f80: 7261 7465 5f72 6573 6964 7561 6c73 2864  rate_residuals(d
+00027f90: 6174 6173 6574 3a20 5461 7554 4461 7461  ataset: TauTData
+00027fa0: 7365 7420 7c20 5461 7548 4461 7461 7365  set | TauHDatase
+00027fb0: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
+00027fc0: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
+00027fd0: 6c3a 204c 6f67 5461 7554 4d6f 6465 6c20  l: LogTauTModel 
+00027fe0: 7c20 4d75 6c74 694c 6f67 5461 7554 4d6f  | MultiLogTauTMo
+00027ff0: 6465 6c20 7c20 4c6f 6754 6175 484d 6f64  del | LogTauHMod
+00028000: 656c 207c 204d 756c 7469 4c6f 6754 6175  el | MultiLogTau
+00028010: 484d 6f64 656c 2c20 2320 6e6f 7161 0a20  HModel, # noqa. 
 00028020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028030: 2020 2020 6178 3a20 706c 742e 4178 6573      ax: plt.Axes
-00028040: 2920 2d3e 204e 6f6e 653a 0a20 2020 2027  ) -> None:.    '
-00028050: 2727 0a20 2020 2050 6c6f 7473 2064 6966  ''.    Plots dif
-00028060: 6665 7265 6e63 6520 6f66 206c 6f67 3130  ference of log10
-00028070: 2865 7870 6572 696d 656e 7429 2061 6e64  (experiment) and
-00028080: 206c 6f67 3130 286d 6f64 656c 2920 7265   log10(model) re
-00028090: 6c61 7861 7469 6f6e 2072 6174 6573 0a20  laxation rates. 
-000280a0: 2020 206f 6e74 6f20 6120 6769 7665 6e20     onto a given 
-000280b0: 6669 6775 7265 2061 6e64 2061 7869 730a  figure and axis.
-000280c0: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
-000280d0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-000280e0: 2020 206d 6f64 656c 733a 206c 6973 745b     models: list[
-000280f0: 4c6f 6754 6175 544d 6f64 656c 207c 204d  LogTauTModel | M
-00028100: 756c 7469 4c6f 6754 6175 544d 6f64 656c  ultiLogTauTModel
-00028110: 207c 204c 6f67 5461 7548 4d6f 6465 6c20   | LogTauHModel 
-00028120: 7c20 4d75 6c74 694c 6f67 5461 7548 4d6f  | MultiLogTauHMo
-00028130: 6465 6c5d 0a20 2020 2020 2020 204d 6f64  del].        Mod
-00028140: 656c 732c 206f 6e65 2070 6572 2074 656d  els, one per tem
-00028150: 7065 7261 7475 7265 0a20 2020 2066 696c  perature.    fil
-00028160: 655f 6e61 6d65 3a20 7374 720a 2020 2020  e_name: str.    
-00028170: 2020 2020 4e61 6d65 206f 6620 6f75 7470      Name of outp
-00028180: 7574 2066 696c 650a 2020 2020 6178 3a20  ut file.    ax: 
-00028190: 706c 742e 4178 6573 0a20 2020 2020 2020  plt.Axes.       
-000281a0: 204d 6174 706c 6f74 6c69 6220 4178 6973   Matplotlib Axis
-000281b0: 206f 626a 6563 7420 7573 6564 2066 6f72   object used for
-000281c0: 2070 6c6f 740a 0a20 2020 2052 6574 7572   plot..    Retur
-000281d0: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
-000281e0: 2020 204e 6f6e 650a 2020 2020 2727 2720     None.    ''' 
-000281f0: 2320 6e6f 7161 0a0a 2020 2020 6966 2069  # noqa..    if i
-00028200: 7369 6e73 7461 6e63 6528 6461 7461 7365  sinstance(datase
-00028210: 742c 2054 6175 4844 6174 6173 6574 293a  t, TauHDataset):
-00028220: 0a20 2020 2020 2020 2078 5f74 7970 6520  .        x_type 
-00028230: 3d20 2766 6965 6c64 270a 2020 2020 2020  = 'field'.      
-00028240: 2020 785f 7661 6c73 203d 2063 6f70 792e    x_vals = copy.
-00028250: 636f 7079 2864 6174 6173 6574 2e66 6965  copy(dataset.fie
-00028260: 6c64 7329 0a20 2020 2020 2020 2061 782e  lds).        ax.
-00028270: 7365 745f 786c 6162 656c 2872 2746 6965  set_xlabel(r'Fie
-00028280: 6c64 2028 4f65 2927 290a 2020 2020 656c  ld (Oe)').    el
-00028290: 6966 2069 7369 6e73 7461 6e63 6528 6461  if isinstance(da
-000282a0: 7461 7365 742c 2054 6175 5444 6174 6173  taset, TauTDatas
-000282b0: 6574 293a 0a20 2020 2020 2020 2078 5f74  et):.        x_t
-000282c0: 7970 6520 3d20 2774 656d 7065 7261 7475  ype = 'temperatu
-000282d0: 7265 270a 2020 2020 2020 2020 785f 7661  re'.        x_va
-000282e0: 6c73 203d 2063 6f70 792e 636f 7079 2864  ls = copy.copy(d
-000282f0: 6174 6173 6574 2e74 656d 7065 7261 7475  ataset.temperatu
-00028300: 7265 7329 0a20 2020 2020 2020 2061 782e  res).        ax.
-00028310: 7365 745f 786c 6162 656c 2872 2754 656d  set_xlabel(r'Tem
-00028320: 7065 7261 7475 7265 2028 4b29 2729 0a0a  perature (K)')..
-00028330: 2020 2020 2320 4164 6420 6164 6469 7469      # Add additi
-00028340: 6f6e 616c 2073 6574 206f 6620 6178 6573  onal set of axes
-00028350: 2074 6f20 6372 6561 7465 2027 7a65 726f   to create 'zero
-00028360: 2720 6c69 6e65 0a20 2020 2061 7832 203d  ' line.    ax2 =
-00028370: 2061 782e 7477 696e 7928 290a 2020 2020   ax.twiny().    
-00028380: 6178 322e 6765 745f 7961 7869 7328 292e  ax2.get_yaxis().
-00028390: 7365 745f 7669 7369 626c 6528 4661 6c73  set_visible(Fals
-000283a0: 6529 0a20 2020 2061 7832 2e73 6574 5f79  e).    ax2.set_y
-000283b0: 7469 636b 7328 5b5d 290a 2020 2020 6178  ticks([]).    ax
-000283c0: 322e 7365 745f 7874 6963 6b73 285b 5d29  2.set_xticks([])
-000283d0: 0a20 2020 2061 7832 2e73 7069 6e65 735b  .    ax2.spines[
-000283e0: 2762 6f74 746f 6d27 5d2e 7365 745f 706f  'bottom'].set_po
-000283f0: 7369 7469 6f6e 2828 277a 6572 6f27 2929  sition(('zero'))
-00028400: 0a0a 2020 2020 6966 2074 7970 6528 6d6f  ..    if type(mo
-00028410: 6465 6c29 2069 6e20 5b4d 756c 7469 4c6f  del) in [MultiLo
-00028420: 6754 6175 544d 6f64 656c 2c20 4d75 6c74  gTauTModel, Mult
-00028430: 694c 6f67 5461 7548 4d6f 6465 6c5d 3a0a  iLogTauHModel]:.
-00028440: 2020 2020 2020 2020 6c6f 676d 6f64 656c          logmodel
-00028450: 7320 3d20 6d6f 6465 6c2e 6c6f 676d 6f64  s = model.logmod
-00028460: 656c 730a 2020 2020 656c 7365 3a0a 2020  els.    else:.  
-00028470: 2020 2020 2020 6c6f 676d 6f64 656c 7320        logmodels 
-00028480: 3d20 5b6d 6f64 656c 5d0a 0a20 2020 206d  = [model]..    m
-00028490: 6f64 656c 5f72 6174 6520 3d20 6e70 2e7a  odel_rate = np.z
-000284a0: 6572 6f73 286c 656e 2878 5f76 616c 7329  eros(len(x_vals)
-000284b0: 290a 0a20 2020 2066 6f72 206c 6f67 6d6f  )..    for logmo
-000284c0: 6465 6c20 696e 206c 6f67 6d6f 6465 6c73  del in logmodels
-000284d0: 3a0a 2020 2020 2020 2020 6d6f 6465 6c5f  :.        model_
-000284e0: 7261 7465 202b 3d20 3130 2a2a 6c6f 676d  rate += 10**logm
-000284f0: 6f64 656c 2e6d 6f64 656c 280a 2020 2020  odel.model(.    
-00028500: 2020 2020 2020 2020 6c6f 676d 6f64 656c          logmodel
-00028510: 2e66 696e 616c 5f76 6172 5f76 616c 7565  .final_var_value
-00028520: 732c 0a20 2020 2020 2020 2020 2020 2078  s,.            x
-00028530: 5f76 616c 732c 0a20 2020 2020 2020 2029  _vals,.        )
-00028540: 0a0a 2020 2020 6d6f 6465 6c5f 6c6f 6772  ..    model_logr
-00028550: 6174 6520 3d20 6e70 2e6c 6f67 3130 286d  ate = np.log10(m
-00028560: 6f64 656c 5f72 6174 6529 0a0a 2020 2020  odel_rate)..    
-00028570: 2320 506c 6f74 2072 6573 6964 7561 6c73  # Plot residuals
-00028580: 0a20 2020 2069 6620 6c65 6e28 6461 7461  .    if len(data
-00028590: 7365 742e 6c6f 6772 6174 655f 706d 293a  set.lograte_pm):
-000285a0: 0a20 2020 2020 2020 2061 782e 6572 726f  .        ax.erro
-000285b0: 7262 6172 280a 2020 2020 2020 2020 2020  rbar(.          
-000285c0: 2020 785f 7661 6c73 2c0a 2020 2020 2020    x_vals,.      
-000285d0: 2020 2020 2020 6e70 2e6c 6f67 3130 2864        np.log10(d
-000285e0: 6174 6173 6574 2e72 6174 6573 2920 2d20  ataset.rates) - 
-000285f0: 6d6f 6465 6c5f 6c6f 6772 6174 652c 0a20  model_lograte,. 
-00028600: 2020 2020 2020 2020 2020 2079 6572 723d             yerr=
-00028610: 6461 7461 7365 742e 6c6f 6772 6174 655f  dataset.lograte_
-00028620: 706d 2c0a 2020 2020 2020 2020 2020 2020  pm,.            
-00028630: 666d 743d 2762 2e27 0a20 2020 2020 2020  fmt='b.'.       
-00028640: 2029 0a20 2020 2065 6c73 653a 0a20 2020   ).    else:.   
-00028650: 2020 2020 2061 782e 706c 6f74 280a 2020       ax.plot(.  
-00028660: 2020 2020 2020 2020 2020 785f 7661 6c73            x_vals
-00028670: 2c0a 2020 2020 2020 2020 2020 2020 6e70  ,.            np
-00028680: 2e6c 6f67 3130 2864 6174 6173 6574 2e72  .log10(dataset.r
-00028690: 6174 6573 2920 2d20 6d6f 6465 6c5f 6c6f  ates) - model_lo
-000286a0: 6772 6174 652c 0a20 2020 2020 2020 2020  grate,.         
-000286b0: 2020 2063 6f6c 6f72 3d27 6227 2c0a 2020     color='b',.  
-000286c0: 2020 2020 2020 2020 2020 6d61 726b 6572            marker
-000286d0: 3d27 6f27 2c0a 2020 2020 2020 2020 2020  ='o',.          
-000286e0: 2020 6c77 3d30 2c0a 2020 2020 2020 2020    lw=0,.        
-000286f0: 2020 2020 6669 6c6c 7374 796c 653d 276e      fillstyle='n
-00028700: 6f6e 6527 2c0a 2020 2020 2020 2020 2020  one',.          
-00028710: 2020 6c61 6265 6c3d 2745 7870 6572 696d    label='Experim
-00028720: 656e 7427 0a20 2020 2020 2020 2029 0a20  ent'.        ). 
-00028730: 2020 2023 2053 6574 206c 6f67 2073 6361     # Set log sca
-00028740: 6c65 206f 6e20 7820 6178 6973 0a20 2020  le on x axis.   
-00028750: 2069 6620 785f 7479 7065 203d 3d20 2766   if x_type == 'f
-00028760: 6965 6c64 273a 0a20 2020 2020 2020 2069  ield':.        i
-00028770: 6620 616e 7928 7661 6c20 3c20 6e70 2e66  f any(val < np.f
-00028780: 696e 666f 2866 6c6f 6174 292e 6570 7320  info(float).eps 
-00028790: 666f 7220 7661 6c20 696e 2078 5f76 616c  for val in x_val
-000287a0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-000287b0: 6178 2e73 6574 5f78 7363 616c 6528 0a20  ax.set_xscale(. 
-000287c0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000287d0: 7379 6d6c 6f67 272c 0a20 2020 2020 2020  symlog',.       
-000287e0: 2020 2020 2020 2020 206c 696e 7468 7265           linthre
-000287f0: 7368 3d67 7569 2e63 616c 635f 6c69 6e74  sh=gui.calc_lint
-00028800: 6872 6573 6828 785f 7661 6c73 292c 0a20  hresh(x_vals),. 
-00028810: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00028820: 696e 7363 616c 653d 6775 692e 6361 6c63  inscale=gui.calc
-00028830: 5f6c 696e 7363 616c 6528 785f 7661 6c73  _linscale(x_vals
-00028840: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
-00028850: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00028860: 2020 2020 2020 2020 2020 6178 2e73 6574            ax.set
-00028870: 5f78 7363 616c 6528 276c 6f67 2729 0a20  _xscale('log'). 
-00028880: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00028890: 2061 782e 7365 745f 7873 6361 6c65 2827   ax.set_xscale('
-000288a0: 6c6f 6727 290a 0a20 2020 2023 2053 6574  log')..    # Set
-000288b0: 2066 6f72 6d61 7474 696e 6720 666f 7220   formatting for 
-000288c0: 7920 6178 6973 206d 616a 6f72 2074 6963  y axis major tic
-000288d0: 6b73 0a20 2020 2061 782e 7961 7869 732e  ks.    ax.yaxis.
-000288e0: 7365 745f 6d61 6a6f 725f 666f 726d 6174  set_major_format
-000288f0: 7465 7228 5363 616c 6172 466f 726d 6174  ter(ScalarFormat
-00028900: 7465 7228 2929 0a0a 2020 2020 2320 4164  ter())..    # Ad
-00028910: 6420 6d69 6e6f 7220 7469 636b 7320 746f  d minor ticks to
-00028920: 2079 2061 7869 7320 7769 7468 206e 6f20   y axis with no 
-00028930: 6c61 6265 6c73 0a20 2020 2061 782e 7961  labels.    ax.ya
-00028940: 7869 732e 7365 745f 6d69 6e6f 725f 6c6f  xis.set_minor_lo
-00028950: 6361 746f 7228 4175 746f 4d69 6e6f 724c  cator(AutoMinorL
-00028960: 6f63 6174 6f72 2829 290a 0a20 2020 2023  ocator())..    #
-00028970: 2053 796d 6d65 7472 6973 6520 7920 6178   Symmetrise y ax
-00028980: 6973 206c 696d 6974 7320 6261 7365 6420  is limits based 
-00028990: 6f6e 206d 6178 2061 6273 2065 7272 6f72  on max abs error
-000289a0: 0a20 2020 2069 6620 6c65 6e28 6461 7461  .    if len(data
-000289b0: 7365 742e 6c6f 6772 6174 655f 706d 293a  set.lograte_pm):
-000289c0: 0a20 2020 2020 2020 2061 6c6c 5f64 6174  .        all_dat
-000289d0: 6120 3d20 5b0a 2020 2020 2020 2020 2020  a = [.          
-000289e0: 2020 6e70 2e6c 6f67 3130 2864 6174 6173    np.log10(datas
-000289f0: 6574 2e72 6174 6573 2920 2d20 6d6f 6465  et.rates) - mode
-00028a00: 6c5f 6c6f 6772 6174 6520 2b20 6461 7461  l_lograte + data
-00028a10: 7365 742e 6c6f 6772 6174 655f 706d 0a20  set.lograte_pm. 
-00028a20: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-00028a30: 2061 6c6c 5f64 6174 6120 2b3d 205b 0a20   all_data += [. 
-00028a40: 2020 2020 2020 2020 2020 206e 702e 6c6f             np.lo
-00028a50: 6731 3028 6461 7461 7365 742e 7261 7465  g10(dataset.rate
-00028a60: 7329 202d 206d 6f64 656c 5f6c 6f67 7261  s) - model_logra
-00028a70: 7465 202d 2064 6174 6173 6574 2e6c 6f67  te - dataset.log
-00028a80: 7261 7465 5f70 6d0a 2020 2020 2020 2020  rate_pm.        
-00028a90: 5d0a 2020 2020 656c 7365 3a0a 2020 2020  ].    else:.    
-00028aa0: 2020 2020 616c 6c5f 6461 7461 203d 205b      all_data = [
-00028ab0: 0a20 2020 2020 2020 2020 2020 206e 702e  .            np.
-00028ac0: 6c6f 6731 3028 6461 7461 7365 742e 7261  log10(dataset.ra
-00028ad0: 7465 7329 202d 206d 6f64 656c 5f6c 6f67  tes) - model_log
-00028ae0: 7261 7465 0a20 2020 2020 2020 205d 0a20  rate.        ]. 
-00028af0: 2020 2020 2020 2061 6c6c 5f64 6174 6120         all_data 
-00028b00: 2b3d 205b 0a20 2020 2020 2020 2020 2020  += [.           
-00028b10: 206e 702e 6c6f 6731 3028 6461 7461 7365   np.log10(datase
-00028b20: 742e 7261 7465 7329 202d 206d 6f64 656c  t.rates) - model
-00028b30: 5f6c 6f67 7261 7465 0a20 2020 2020 2020  _lograte.       
-00028b40: 205d 0a0a 2020 2020 7469 636b 732c 206d   ]..    ticks, m
-00028b50: 6178 7661 6c20 3d20 6775 692e 6d69 6e5f  axval = gui.min_
-00028b60: 6d61 785f 7469 636b 735f 7769 7468 5f7a  max_ticks_with_z
-00028b70: 6572 6f28 616c 6c5f 6461 7461 2c20 3529  ero(all_data, 5)
-00028b80: 0a20 2020 2061 782e 7365 745f 7974 6963  .    ax.set_ytic
-00028b90: 6b73 2874 6963 6b73 290a 0a20 2020 2061  ks(ticks)..    a
-00028ba0: 782e 7365 745f 796c 696d 285b 2d20 6d61  x.set_ylim([- ma
-00028bb0: 7876 616c 202a 2031 2e31 2c20 2b20 6d61  xval * 1.1, + ma
-00028bc0: 7876 616c 202a 2031 2e31 5d29 0a0a 2020  xval * 1.1])..  
-00028bd0: 2020 2320 4178 6973 206c 6162 656c 730a    # Axis labels.
-00028be0: 2020 2020 6178 2e73 6574 5f79 6c61 6265      ax.set_ylabe
-00028bf0: 6c28 0a20 2020 2020 2020 2072 2724 5c6c  l(.        r'$\l
-00028c00: 6f67 5f5c 6d61 7468 7265 6775 6c61 727b  og_\mathregular{
-00028c10: 3130 7d5c 6c65 6674 5b5c 7461 755e 5c6d  10}\left[\tau^\m
-00028c20: 6174 6872 6567 756c 6172 7b2d 317d 5f7b  athregular{-1}_{
-00028c30: 5c6d 6174 6872 6567 756c 6172 7b65 7870  \mathregular{exp
-00028c40: 7d7d 5c72 6967 6874 5d20 2d20 5c6c 6f67  }}\right] - \log
-00028c50: 5f5c 6d61 7468 7265 6775 6c61 727b 3130  _\mathregular{10
-00028c60: 7d5c 6c65 6674 5b5c 7461 755e 5c6d 6174  }\left[\tau^\mat
-00028c70: 6872 6567 756c 6172 7b2d 317d 5f7b 5c6d  hregular{-1}_{\m
-00028c80: 6174 6872 6567 756c 6172 7b66 6974 7d7d  athregular{fit}}
-00028c90: 5c72 6967 6874 5d24 2020 245c 6c65 6674  \right]$  $\left
-00028ca0: 285c 6c6f 675f 5c6d 6174 6872 6567 756c  (\log_\mathregul
-00028cb0: 6172 7b31 307d 5c6c 6566 745b 5c6d 6174  ar{10}\left[\mat
-00028cc0: 6872 6567 756c 6172 7b73 7d5e 5c6d 6174  hregular{s}^\mat
-00028cd0: 6872 6567 756c 6172 7b2d 317d 5c72 6967  hregular{-1}\rig
-00028ce0: 6874 5d5c 7269 6768 7429 2427 2023 206e  ht]\right)$' # n
-00028cf0: 6f71 610a 2020 2020 290a 0a20 2020 2023  oqa.    )..    #
-00028d00: 2053 6574 2078 2074 6963 6b20 666f 726d   Set x tick form
-00028d10: 6174 7469 6e67 0a20 2020 2067 7569 2e73  atting.    gui.s
-00028d20: 6574 5f72 6174 655f 7874 6963 6b5f 666f  et_rate_xtick_fo
-00028d30: 726d 6174 7469 6e67 2861 782c 2078 5f76  rmatting(ax, x_v
-00028d40: 616c 732c 2078 5f74 7970 653d 785f 7479  als, x_type=x_ty
-00028d50: 7065 290a 0a20 2020 2072 6574 7572 6e0a  pe)..    return.
-00028d60: 0a0a 6465 6620 7772 6974 655f 6d6f 6465  ..def write_mode
-00028d70: 6c5f 7061 7261 6d73 286d 6f64 656c 3a20  l_params(model: 
-00028d80: 4c6f 6754 6175 544d 6f64 656c 207c 204d  LogTauTModel | M
-00028d90: 756c 7469 4c6f 6754 6175 544d 6f64 656c  ultiLogTauTModel
-00028da0: 207c 204c 6f67 5461 7548 4d6f 6465 6c20   | LogTauHModel 
-00028db0: 7c20 4d75 6c74 694c 6f67 5461 7548 4d6f  | MultiLogTauHMo
-00028dc0: 6465 6c2c 2023 206e 6f71 610a 2020 2020  del, # noqa.    
+00028030: 2020 2020 2020 2020 6178 3a20 706c 742e          ax: plt.
+00028040: 4178 6573 2920 2d3e 204e 6f6e 653a 0a20  Axes) -> None:. 
+00028050: 2020 2027 2727 0a20 2020 2050 6c6f 7473     '''.    Plots
+00028060: 2064 6966 6665 7265 6e63 6520 6f66 206c   difference of l
+00028070: 6f67 3130 2865 7870 6572 696d 656e 7429  og10(experiment)
+00028080: 2061 6e64 206c 6f67 3130 286d 6f64 656c   and log10(model
+00028090: 2920 7265 6c61 7861 7469 6f6e 2072 6174  ) relaxation rat
+000280a0: 6573 0a20 2020 206f 6e74 6f20 6120 6769  es.    onto a gi
+000280b0: 7665 6e20 6669 6775 7265 2061 6e64 2061  ven figure and a
+000280c0: 7869 730a 0a20 2020 2050 6172 616d 6574  xis..    Paramet
+000280d0: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
+000280e0: 2d2d 0a20 2020 206d 6f64 656c 733a 206c  --.    models: l
+000280f0: 6973 745b 4c6f 6754 6175 544d 6f64 656c  ist[LogTauTModel
+00028100: 207c 204d 756c 7469 4c6f 6754 6175 544d   | MultiLogTauTM
+00028110: 6f64 656c 207c 204c 6f67 5461 7548 4d6f  odel | LogTauHMo
+00028120: 6465 6c20 7c20 4d75 6c74 694c 6f67 5461  del | MultiLogTa
+00028130: 7548 4d6f 6465 6c5d 0a20 2020 2020 2020  uHModel].       
+00028140: 204d 6f64 656c 732c 206f 6e65 2070 6572   Models, one per
+00028150: 2074 656d 7065 7261 7475 7265 0a20 2020   temperature.   
+00028160: 2066 696c 655f 6e61 6d65 3a20 7374 720a   file_name: str.
+00028170: 2020 2020 2020 2020 4e61 6d65 206f 6620          Name of 
+00028180: 6f75 7470 7574 2066 696c 650a 2020 2020  output file.    
+00028190: 6178 3a20 706c 742e 4178 6573 0a20 2020  ax: plt.Axes.   
+000281a0: 2020 2020 204d 6174 706c 6f74 6c69 6220       Matplotlib 
+000281b0: 4178 6973 206f 626a 6563 7420 7573 6564  Axis object used
+000281c0: 2066 6f72 2070 6c6f 740a 0a20 2020 2052   for plot..    R
+000281d0: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
+000281e0: 2d2d 0a20 2020 204e 6f6e 650a 2020 2020  --.    None.    
+000281f0: 2727 2720 2320 6e6f 7161 0a0a 2020 2020  ''' # noqa..    
+00028200: 6966 2069 7369 6e73 7461 6e63 6528 6461  if isinstance(da
+00028210: 7461 7365 742c 2054 6175 4844 6174 6173  taset, TauHDatas
+00028220: 6574 293a 0a20 2020 2020 2020 2078 5f74  et):.        x_t
+00028230: 7970 6520 3d20 2766 6965 6c64 270a 2020  ype = 'field'.  
+00028240: 2020 2020 2020 785f 7661 6c73 203d 2063        x_vals = c
+00028250: 6f70 792e 636f 7079 2864 6174 6173 6574  opy.copy(dataset
+00028260: 2e66 6965 6c64 7329 0a20 2020 2020 2020  .fields).       
+00028270: 2061 782e 7365 745f 786c 6162 656c 2872   ax.set_xlabel(r
+00028280: 2746 6965 6c64 2028 4f65 2927 290a 2020  'Field (Oe)').  
+00028290: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
+000282a0: 6528 6461 7461 7365 742c 2054 6175 5444  e(dataset, TauTD
+000282b0: 6174 6173 6574 293a 0a20 2020 2020 2020  ataset):.       
+000282c0: 2078 5f74 7970 6520 3d20 2774 656d 7065   x_type = 'tempe
+000282d0: 7261 7475 7265 270a 2020 2020 2020 2020  rature'.        
+000282e0: 785f 7661 6c73 203d 2063 6f70 792e 636f  x_vals = copy.co
+000282f0: 7079 2864 6174 6173 6574 2e74 656d 7065  py(dataset.tempe
+00028300: 7261 7475 7265 7329 0a20 2020 2020 2020  ratures).       
+00028310: 2061 782e 7365 745f 786c 6162 656c 2872   ax.set_xlabel(r
+00028320: 2754 656d 7065 7261 7475 7265 2028 4b29  'Temperature (K)
+00028330: 2729 0a0a 2020 2020 2320 4164 6420 6164  ')..    # Add ad
+00028340: 6469 7469 6f6e 616c 2073 6574 206f 6620  ditional set of 
+00028350: 6178 6573 2074 6f20 6372 6561 7465 2027  axes to create '
+00028360: 7a65 726f 2720 6c69 6e65 0a20 2020 2061  zero' line.    a
+00028370: 7832 203d 2061 782e 7477 696e 7928 290a  x2 = ax.twiny().
+00028380: 2020 2020 6178 322e 6765 745f 7961 7869      ax2.get_yaxi
+00028390: 7328 292e 7365 745f 7669 7369 626c 6528  s().set_visible(
+000283a0: 4661 6c73 6529 0a20 2020 2061 7832 2e73  False).    ax2.s
+000283b0: 6574 5f79 7469 636b 7328 5b5d 290a 2020  et_yticks([]).  
+000283c0: 2020 6178 322e 7365 745f 7874 6963 6b73    ax2.set_xticks
+000283d0: 285b 5d29 0a20 2020 2061 7832 2e73 7069  ([]).    ax2.spi
+000283e0: 6e65 735b 2762 6f74 746f 6d27 5d2e 7365  nes['bottom'].se
+000283f0: 745f 706f 7369 7469 6f6e 2828 277a 6572  t_position(('zer
+00028400: 6f27 2929 0a0a 2020 2020 6966 2074 7970  o'))..    if typ
+00028410: 6528 6d6f 6465 6c29 2069 6e20 5b4d 756c  e(model) in [Mul
+00028420: 7469 4c6f 6754 6175 544d 6f64 656c 2c20  tiLogTauTModel, 
+00028430: 4d75 6c74 694c 6f67 5461 7548 4d6f 6465  MultiLogTauHMode
+00028440: 6c5d 3a0a 2020 2020 2020 2020 6c6f 676d  l]:.        logm
+00028450: 6f64 656c 7320 3d20 6d6f 6465 6c2e 6c6f  odels = model.lo
+00028460: 676d 6f64 656c 730a 2020 2020 656c 7365  gmodels.    else
+00028470: 3a0a 2020 2020 2020 2020 6c6f 676d 6f64  :.        logmod
+00028480: 656c 7320 3d20 5b6d 6f64 656c 5d0a 0a20  els = [model].. 
+00028490: 2020 206d 6f64 656c 5f72 6174 6520 3d20     model_rate = 
+000284a0: 6e70 2e7a 6572 6f73 286c 656e 2878 5f76  np.zeros(len(x_v
+000284b0: 616c 7329 290a 0a20 2020 2066 6f72 206c  als))..    for l
+000284c0: 6f67 6d6f 6465 6c20 696e 206c 6f67 6d6f  ogmodel in logmo
+000284d0: 6465 6c73 3a0a 2020 2020 2020 2020 6d6f  dels:.        mo
+000284e0: 6465 6c5f 7261 7465 202b 3d20 3130 2a2a  del_rate += 10**
+000284f0: 6c6f 676d 6f64 656c 2e6d 6f64 656c 280a  logmodel.model(.
+00028500: 2020 2020 2020 2020 2020 2020 6c6f 676d              logm
+00028510: 6f64 656c 2e66 696e 616c 5f76 6172 5f76  odel.final_var_v
+00028520: 616c 7565 732c 0a20 2020 2020 2020 2020  alues,.         
+00028530: 2020 2078 5f76 616c 732c 0a20 2020 2020     x_vals,.     
+00028540: 2020 2029 0a0a 2020 2020 6d6f 6465 6c5f     )..    model_
+00028550: 6c6f 6772 6174 6520 3d20 6e70 2e6c 6f67  lograte = np.log
+00028560: 3130 286d 6f64 656c 5f72 6174 6529 0a0a  10(model_rate)..
+00028570: 2020 2020 2320 506c 6f74 2072 6573 6964      # Plot resid
+00028580: 7561 6c73 0a20 2020 2069 6620 6c65 6e28  uals.    if len(
+00028590: 6461 7461 7365 742e 6c6f 6772 6174 655f  dataset.lograte_
+000285a0: 706d 293a 0a20 2020 2020 2020 2061 782e  pm):.        ax.
+000285b0: 6572 726f 7262 6172 280a 2020 2020 2020  errorbar(.      
+000285c0: 2020 2020 2020 785f 7661 6c73 2c0a 2020        x_vals,.  
+000285d0: 2020 2020 2020 2020 2020 6e70 2e6c 6f67            np.log
+000285e0: 3130 2864 6174 6173 6574 2e72 6174 6573  10(dataset.rates
+000285f0: 2920 2d20 6d6f 6465 6c5f 6c6f 6772 6174  ) - model_lograt
+00028600: 652c 0a20 2020 2020 2020 2020 2020 2079  e,.            y
+00028610: 6572 723d 6461 7461 7365 742e 6c6f 6772  err=dataset.logr
+00028620: 6174 655f 706d 2c0a 2020 2020 2020 2020  ate_pm,.        
+00028630: 2020 2020 666d 743d 2762 2e27 0a20 2020      fmt='b.'.   
+00028640: 2020 2020 2029 0a20 2020 2065 6c73 653a       ).    else:
+00028650: 0a20 2020 2020 2020 2061 782e 706c 6f74  .        ax.plot
+00028660: 280a 2020 2020 2020 2020 2020 2020 785f  (.            x_
+00028670: 7661 6c73 2c0a 2020 2020 2020 2020 2020  vals,.          
+00028680: 2020 6e70 2e6c 6f67 3130 2864 6174 6173    np.log10(datas
+00028690: 6574 2e72 6174 6573 2920 2d20 6d6f 6465  et.rates) - mode
+000286a0: 6c5f 6c6f 6772 6174 652c 0a20 2020 2020  l_lograte,.     
+000286b0: 2020 2020 2020 2063 6f6c 6f72 3d27 6227         color='b'
+000286c0: 2c0a 2020 2020 2020 2020 2020 2020 6d61  ,.            ma
+000286d0: 726b 6572 3d27 6f27 2c0a 2020 2020 2020  rker='o',.      
+000286e0: 2020 2020 2020 6c77 3d30 2c0a 2020 2020        lw=0,.    
+000286f0: 2020 2020 2020 2020 6669 6c6c 7374 796c          fillstyl
+00028700: 653d 276e 6f6e 6527 2c0a 2020 2020 2020  e='none',.      
+00028710: 2020 2020 2020 6c61 6265 6c3d 2745 7870        label='Exp
+00028720: 6572 696d 656e 7427 0a20 2020 2020 2020  eriment'.       
+00028730: 2029 0a20 2020 2023 2053 6574 206c 6f67   ).    # Set log
+00028740: 2073 6361 6c65 206f 6e20 7820 6178 6973   scale on x axis
+00028750: 0a20 2020 2069 6620 785f 7479 7065 203d  .    if x_type =
+00028760: 3d20 2766 6965 6c64 273a 0a20 2020 2020  = 'field':.     
+00028770: 2020 2069 6620 616e 7928 7661 6c20 3c20     if any(val < 
+00028780: 6e70 2e66 696e 666f 2866 6c6f 6174 292e  np.finfo(float).
+00028790: 6570 7320 666f 7220 7661 6c20 696e 2078  eps for val in x
+000287a0: 5f76 616c 7329 3a0a 2020 2020 2020 2020  _vals):.        
+000287b0: 2020 2020 6178 2e73 6574 5f78 7363 616c      ax.set_xscal
+000287c0: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
+000287d0: 2020 2027 7379 6d6c 6f67 272c 0a20 2020     'symlog',.   
+000287e0: 2020 2020 2020 2020 2020 2020 206c 696e               lin
+000287f0: 7468 7265 7368 3d67 7569 2e63 616c 635f  thresh=gui.calc_
+00028800: 6c69 6e74 6872 6573 6828 785f 7661 6c73  linthresh(x_vals
+00028810: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00028820: 2020 206c 696e 7363 616c 653d 6775 692e     linscale=gui.
+00028830: 6361 6c63 5f6c 696e 7363 616c 6528 785f  calc_linscale(x_
+00028840: 7661 6c73 290a 2020 2020 2020 2020 2020  vals).          
+00028850: 2020 290a 2020 2020 2020 2020 656c 7365    ).        else
+00028860: 3a0a 2020 2020 2020 2020 2020 2020 6178  :.            ax
+00028870: 2e73 6574 5f78 7363 616c 6528 276c 6f67  .set_xscale('log
+00028880: 2729 0a20 2020 2065 6c73 653a 0a20 2020  ').    else:.   
+00028890: 2020 2020 2061 782e 7365 745f 7873 6361       ax.set_xsca
+000288a0: 6c65 2827 6c6f 6727 290a 0a20 2020 2023  le('log')..    #
+000288b0: 2053 6574 2066 6f72 6d61 7474 696e 6720   Set formatting 
+000288c0: 666f 7220 7920 6178 6973 206d 616a 6f72  for y axis major
+000288d0: 2074 6963 6b73 0a20 2020 2061 782e 7961   ticks.    ax.ya
+000288e0: 7869 732e 7365 745f 6d61 6a6f 725f 666f  xis.set_major_fo
+000288f0: 726d 6174 7465 7228 5363 616c 6172 466f  rmatter(ScalarFo
+00028900: 726d 6174 7465 7228 2929 0a0a 2020 2020  rmatter())..    
+00028910: 2320 4164 6420 6d69 6e6f 7220 7469 636b  # Add minor tick
+00028920: 7320 746f 2079 2061 7869 7320 7769 7468  s to y axis with
+00028930: 206e 6f20 6c61 6265 6c73 0a20 2020 2061   no labels.    a
+00028940: 782e 7961 7869 732e 7365 745f 6d69 6e6f  x.yaxis.set_mino
+00028950: 725f 6c6f 6361 746f 7228 4175 746f 4d69  r_locator(AutoMi
+00028960: 6e6f 724c 6f63 6174 6f72 2829 290a 0a20  norLocator()).. 
+00028970: 2020 2023 2053 796d 6d65 7472 6973 6520     # Symmetrise 
+00028980: 7920 6178 6973 206c 696d 6974 7320 6261  y axis limits ba
+00028990: 7365 6420 6f6e 206d 6178 2061 6273 2065  sed on max abs e
+000289a0: 7272 6f72 0a20 2020 2069 6620 6c65 6e28  rror.    if len(
+000289b0: 6461 7461 7365 742e 6c6f 6772 6174 655f  dataset.lograte_
+000289c0: 706d 293a 0a20 2020 2020 2020 2061 6c6c  pm):.        all
+000289d0: 5f64 6174 6120 3d20 5b0a 2020 2020 2020  _data = [.      
+000289e0: 2020 2020 2020 6e70 2e6c 6f67 3130 2864        np.log10(d
+000289f0: 6174 6173 6574 2e72 6174 6573 2920 2d20  ataset.rates) - 
+00028a00: 6d6f 6465 6c5f 6c6f 6772 6174 6520 2b20  model_lograte + 
+00028a10: 6461 7461 7365 742e 6c6f 6772 6174 655f  dataset.lograte_
+00028a20: 706d 0a20 2020 2020 2020 205d 0a20 2020  pm.        ].   
+00028a30: 2020 2020 2061 6c6c 5f64 6174 6120 2b3d       all_data +=
+00028a40: 205b 0a20 2020 2020 2020 2020 2020 206e   [.            n
+00028a50: 702e 6c6f 6731 3028 6461 7461 7365 742e  p.log10(dataset.
+00028a60: 7261 7465 7329 202d 206d 6f64 656c 5f6c  rates) - model_l
+00028a70: 6f67 7261 7465 202d 2064 6174 6173 6574  ograte - dataset
+00028a80: 2e6c 6f67 7261 7465 5f70 6d0a 2020 2020  .lograte_pm.    
+00028a90: 2020 2020 5d0a 2020 2020 656c 7365 3a0a      ].    else:.
+00028aa0: 2020 2020 2020 2020 616c 6c5f 6461 7461          all_data
+00028ab0: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
+00028ac0: 206e 702e 6c6f 6731 3028 6461 7461 7365   np.log10(datase
+00028ad0: 742e 7261 7465 7329 202d 206d 6f64 656c  t.rates) - model
+00028ae0: 5f6c 6f67 7261 7465 0a20 2020 2020 2020  _lograte.       
+00028af0: 205d 0a20 2020 2020 2020 2061 6c6c 5f64   ].        all_d
+00028b00: 6174 6120 2b3d 205b 0a20 2020 2020 2020  ata += [.       
+00028b10: 2020 2020 206e 702e 6c6f 6731 3028 6461       np.log10(da
+00028b20: 7461 7365 742e 7261 7465 7329 202d 206d  taset.rates) - m
+00028b30: 6f64 656c 5f6c 6f67 7261 7465 0a20 2020  odel_lograte.   
+00028b40: 2020 2020 205d 0a0a 2020 2020 7469 636b       ]..    tick
+00028b50: 732c 206d 6178 7661 6c20 3d20 6775 692e  s, maxval = gui.
+00028b60: 6d69 6e5f 6d61 785f 7469 636b 735f 7769  min_max_ticks_wi
+00028b70: 7468 5f7a 6572 6f28 616c 6c5f 6461 7461  th_zero(all_data
+00028b80: 2c20 3529 0a20 2020 2061 782e 7365 745f  , 5).    ax.set_
+00028b90: 7974 6963 6b73 2874 6963 6b73 290a 0a20  yticks(ticks).. 
+00028ba0: 2020 2061 782e 7365 745f 796c 696d 285b     ax.set_ylim([
+00028bb0: 2d20 6d61 7876 616c 202a 2031 2e31 2c20  - maxval * 1.1, 
+00028bc0: 2b20 6d61 7876 616c 202a 2031 2e31 5d29  + maxval * 1.1])
+00028bd0: 0a0a 2020 2020 2320 4178 6973 206c 6162  ..    # Axis lab
+00028be0: 656c 730a 2020 2020 6178 2e73 6574 5f79  els.    ax.set_y
+00028bf0: 6c61 6265 6c28 0a20 2020 2020 2020 2072  label(.        r
+00028c00: 2724 5c6c 6f67 5f5c 6d61 7468 7265 6775  '$\log_\mathregu
+00028c10: 6c61 727b 3130 7d5c 6c65 6674 5b5c 7461  lar{10}\left[\ta
+00028c20: 755e 5c6d 6174 6872 6567 756c 6172 7b2d  u^\mathregular{-
+00028c30: 317d 5f7b 5c6d 6174 6872 6567 756c 6172  1}_{\mathregular
+00028c40: 7b65 7870 7d7d 5c72 6967 6874 5d20 2d20  {exp}}\right] - 
+00028c50: 5c6c 6f67 5f5c 6d61 7468 7265 6775 6c61  \log_\mathregula
+00028c60: 727b 3130 7d5c 6c65 6674 5b5c 7461 755e  r{10}\left[\tau^
+00028c70: 5c6d 6174 6872 6567 756c 6172 7b2d 317d  \mathregular{-1}
+00028c80: 5f7b 5c6d 6174 6872 6567 756c 6172 7b66  _{\mathregular{f
+00028c90: 6974 7d7d 5c72 6967 6874 5d24 2020 245c  it}}\right]$  $\
+00028ca0: 6c65 6674 285c 6c6f 675f 5c6d 6174 6872  left(\log_\mathr
+00028cb0: 6567 756c 6172 7b31 307d 5c6c 6566 745b  egular{10}\left[
+00028cc0: 5c6d 6174 6872 6567 756c 6172 7b73 7d5e  \mathregular{s}^
+00028cd0: 5c6d 6174 6872 6567 756c 6172 7b2d 317d  \mathregular{-1}
+00028ce0: 5c72 6967 6874 5d5c 7269 6768 7429 2427  \right]\right)$'
+00028cf0: 2023 206e 6f71 610a 2020 2020 290a 0a20   # noqa.    ).. 
+00028d00: 2020 2023 2053 6574 2078 2074 6963 6b20     # Set x tick 
+00028d10: 666f 726d 6174 7469 6e67 0a20 2020 2067  formatting.    g
+00028d20: 7569 2e73 6574 5f72 6174 655f 7874 6963  ui.set_rate_xtic
+00028d30: 6b5f 666f 726d 6174 7469 6e67 2861 782c  k_formatting(ax,
+00028d40: 2078 5f76 616c 732c 2078 5f74 7970 653d   x_vals, x_type=
+00028d50: 785f 7479 7065 290a 0a20 2020 2072 6574  x_type)..    ret
+00028d60: 7572 6e0a 0a0a 6465 6620 7772 6974 655f  urn...def write_
+00028d70: 6d6f 6465 6c5f 7061 7261 6d73 286d 6f64  model_params(mod
+00028d80: 656c 3a20 4c6f 6754 6175 544d 6f64 656c  el: LogTauTModel
+00028d90: 207c 204d 756c 7469 4c6f 6754 6175 544d   | MultiLogTauTM
+00028da0: 6f64 656c 207c 204c 6f67 5461 7548 4d6f  odel | LogTauHMo
+00028db0: 6465 6c20 7c20 4d75 6c74 694c 6f67 5461  del | MultiLogTa
+00028dc0: 7548 4d6f 6465 6c2c 2023 206e 6f71 610a  uHModel, # noqa.
 00028dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028de0: 2020 2066 696c 655f 6e61 6d65 3a20 7374     file_name: st
-00028df0: 722c 2076 6572 626f 7365 3a20 626f 6f6c  r, verbose: bool
-00028e00: 203d 2054 7275 6529 202d 3e20 4e6f 6e65   = True) -> None
-00028e10: 3a0a 2020 2020 2727 270a 2020 2020 5772  :.    '''.    Wr
-00028e20: 6974 6573 2066 6974 7465 6420 616e 6420  ites fitted and 
-00028e30: 6669 7865 6420 7061 7261 6d65 7465 7273  fixed parameters
-00028e40: 206f 6620 6d6f 6465 6c28 7329 2074 6f20   of model(s) to 
-00028e50: 6669 6c65 0a0a 2020 2020 5061 7261 6d65  file..    Parame
-00028e60: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
-00028e70: 2d2d 2d0a 2020 2020 6d6f 6465 6c73 3a20  ---.    models: 
-00028e80: 6c69 7374 5b4c 6f67 5461 7554 4d6f 6465  list[LogTauTMode
-00028e90: 6c20 7c20 4d75 6c74 694c 6f67 5461 7554  l | MultiLogTauT
-00028ea0: 4d6f 6465 6c20 7c20 4c6f 6754 6175 484d  Model | LogTauHM
-00028eb0: 6f64 656c 207c 204d 756c 7469 4c6f 6754  odel | MultiLogT
-00028ec0: 6175 484d 6f64 656c 5d0a 2020 2020 2020  auHModel].      
-00028ed0: 2020 4d6f 6465 6c73 2c20 6f6e 6520 7065    Models, one pe
-00028ee0: 7220 7465 6d70 6572 6174 7572 650a 2020  r temperature.  
-00028ef0: 2020 6669 6c65 5f6e 616d 653a 2073 7472    file_name: str
-00028f00: 0a20 2020 2020 2020 204e 616d 6520 6f66  .        Name of
-00028f10: 206f 7574 7075 7420 6669 6c65 0a20 2020   output file.   
-00028f20: 2076 6572 626f 7365 3a20 626f 6f6c 2c20   verbose: bool, 
-00028f30: 6465 6661 756c 7420 5472 7565 0a20 2020  default True.   
-00028f40: 2020 2020 2049 6620 5472 7565 2c20 6f75       If True, ou
-00028f50: 7470 7574 2066 696c 6520 6c6f 6361 7469  tput file locati
-00028f60: 6f6e 2069 7320 7772 6974 7465 6e20 746f  on is written to
-00028f70: 2074 6572 6d69 6e61 6c0a 0a20 2020 2052   terminal..    R
-00028f80: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
-00028f90: 2d2d 0a20 2020 204e 6f6e 650a 2020 2020  --.    None.    
-00028fa0: 2727 2720 2320 6e6f 7161 0a0a 2020 2020  ''' # noqa..    
-00028fb0: 6966 2074 7970 6528 6d6f 6465 6c29 2069  if type(model) i
-00028fc0: 6e20 5b4d 756c 7469 4c6f 6754 6175 544d  n [MultiLogTauTM
-00028fd0: 6f64 656c 2c20 4d75 6c74 694c 6f67 5461  odel, MultiLogTa
-00028fe0: 7548 4d6f 6465 6c5d 3a0a 2020 2020 2020  uHModel]:.      
-00028ff0: 2020 6c6f 676d 6f64 656c 7320 3d20 6d6f    logmodels = mo
-00029000: 6465 6c2e 6c6f 676d 6f64 656c 730a 2020  del.logmodels.  
-00029010: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00029020: 6c6f 676d 6f64 656c 7320 3d20 5b6d 6f64  logmodels = [mod
-00029030: 656c 5d0a 0a20 2020 2066 203d 206f 7065  el]..    f = ope
-00029040: 6e28 6669 6c65 5f6e 616d 652c 2027 7727  n(file_name, 'w'
-00029050: 2c20 656e 636f 6469 6e67 3d27 7574 662d  , encoding='utf-
-00029060: 3827 290a 0a20 2020 2023 2057 7269 7465  8')..    # Write
-00029070: 2065 6163 6820 7465 726d 2773 206e 616d   each term's nam
-00029080: 652c 2066 6974 2076 6172 732c 2073 7464  e, fit vars, std
-00029090: 6576 2c20 616e 6420 6669 7820 7661 7273  ev, and fix vars
-000290a0: 0a20 2020 2066 6f72 206c 6f67 6d6f 6465  .    for logmode
-000290b0: 6c20 696e 206c 6f67 6d6f 6465 6c73 3a0a  l in logmodels:.
-000290c0: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
-000290d0: 277b 7d5c 6e27 2e66 6f72 6d61 7428 6c6f  '{}\n'.format(lo
-000290e0: 676d 6f64 656c 2e4e 414d 4529 290a 2020  gmodel.NAME)).  
-000290f0: 2020 2020 2020 6966 206c 656e 286c 6f67        if len(log
-00029100: 6d6f 6465 6c2e 6669 745f 7661 7273 2e6b  model.fit_vars.k
-00029110: 6579 7328 2929 3a0a 2020 2020 2020 2020  eys()):.        
-00029120: 2020 2020 662e 7772 6974 6528 2746 6974      f.write('Fit
-00029130: 7465 6420 5465 726d 733a 2056 616c 7565  ted Terms: Value
-00029140: 2061 6e64 2053 7461 6e64 6172 6420 4465   and Standard De
-00029150: 7669 6174 696f 6e3a 5c6e 2729 0a20 2020  viation:\n').   
-00029160: 2020 2020 2020 2020 2066 6f72 206e 616d           for nam
-00029170: 6520 696e 206c 6f67 6d6f 6465 6c2e 6669  e in logmodel.fi
-00029180: 745f 7661 7273 2e6b 6579 7328 293a 0a20  t_vars.keys():. 
-00029190: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000291a0: 2e77 7269 7465 2827 7b3a 3e36 7d20 7b3a  .write('{:>6} {:
-000291b0: 2031 2e38 457d 207b 3a20 312e 3845 7d20   1.8E} {: 1.8E} 
-000291c0: 7b7d 5c6e 272e 666f 726d 6174 280a 2020  {}\n'.format(.  
-000291d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000291e0: 2020 6e61 6d65 2c0a 2020 2020 2020 2020    name,.        
-000291f0: 2020 2020 2020 2020 2020 2020 6c6f 676d              logm
-00029200: 6f64 656c 2e66 696e 616c 5f76 6172 5f76  odel.final_var_v
-00029210: 616c 7565 735b 6e61 6d65 5d2c 0a20 2020  alues[name],.   
-00029220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029230: 206c 6f67 6d6f 6465 6c2e 6669 745f 7374   logmodel.fit_st
-00029240: 6465 765b 6e61 6d65 5d2c 0a20 2020 2020  dev[name],.     
-00029250: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00029260: 6f67 6d6f 6465 6c2e 554e 4954 535b 6e61  ogmodel.UNITS[na
-00029270: 6d65 5d0a 2020 2020 2020 2020 2020 2020  me].            
-00029280: 2020 2020 2929 0a20 2020 2020 2020 2069      )).        i
-00029290: 6620 6c65 6e28 6c6f 676d 6f64 656c 2e66  f len(logmodel.f
-000292a0: 6978 5f76 6172 732e 6b65 7973 2829 293a  ix_vars.keys()):
-000292b0: 0a20 2020 2020 2020 2020 2020 2066 2e77  .            f.w
-000292c0: 7269 7465 2827 4669 7865 6420 5465 726d  rite('Fixed Term
-000292d0: 733a 2056 616c 7565 735c 6e27 290a 2020  s: Values\n').  
-000292e0: 2020 2020 2020 2020 2020 666f 7220 6e61            for na
-000292f0: 6d65 2069 6e20 6c6f 676d 6f64 656c 2e66  me in logmodel.f
-00029300: 6978 5f76 6172 732e 6b65 7973 2829 3a0a  ix_vars.keys():.
-00029310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029320: 662e 7772 6974 6528 277b 3a3e 367d 207b  f.write('{:>6} {
-00029330: 3a20 312e 3845 7d20 7b7d 5c6e 272e 666f  : 1.8E} {}\n'.fo
-00029340: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
-00029350: 2020 2020 2020 2020 2020 6e61 6d65 2c0a            name,.
-00029360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029370: 2020 2020 6c6f 676d 6f64 656c 2e66 696e      logmodel.fin
-00029380: 616c 5f76 6172 5f76 616c 7565 735b 6e61  al_var_values[na
-00029390: 6d65 5d2c 0a20 2020 2020 2020 2020 2020  me],.           
-000293a0: 2020 2020 2020 2020 206c 6f67 6d6f 6465           logmode
-000293b0: 6c2e 554e 4954 535b 6e61 6d65 5d0a 2020  l.UNITS[name].  
-000293c0: 2020 2020 2020 2020 2020 2020 2020 2929                ))
-000293d0: 0a20 2020 2020 2020 2066 2e77 7269 7465  .        f.write
-000293e0: 2827 5c6e 2729 0a0a 2020 2020 6966 2076  ('\n')..    if v
-000293f0: 6572 626f 7365 3a0a 2020 2020 2020 2020  erbose:.        
-00029400: 7574 2e63 7072 696e 7428 0a20 2020 2020  ut.cprint(.     
-00029410: 2020 2020 2020 2027 5c6e 2052 656c 6178         '\n Relax
-00029420: 6174 696f 6e20 4d6f 6465 6c20 7061 7261  ation Model para
-00029430: 6d65 7465 7273 2077 7269 7474 656e 2074  meters written t
-00029440: 6f20 5c6e 207b 7d5c 6e27 2e66 6f72 6d61  o \n {}\n'.forma
-00029450: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-00029460: 2020 2066 696c 655f 6e61 6d65 0a20 2020     file_name.   
-00029470: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
-00029480: 2020 2020 2020 2020 2763 7961 6e27 0a20          'cyan'. 
-00029490: 2020 2020 2020 2029 0a0a 2020 2020 7265         )..    re
-000294a0: 7475 726e 0a0a 0a64 6566 2077 7269 7465  turn...def write
-000294b0: 5f6d 6f64 656c 5f64 6174 6128 6461 7461  _model_data(data
-000294c0: 7365 743a 2054 6175 5444 6174 6173 6574  set: TauTDataset
-000294d0: 207c 2054 6175 4844 6174 6173 6574 2c0a   | TauHDataset,.
-000294e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000294f0: 2020 2020 206d 6f64 656c 3a20 4c6f 6754       model: LogT
-00029500: 6175 544d 6f64 656c 207c 204d 756c 7469  auTModel | Multi
-00029510: 4c6f 6754 6175 544d 6f64 656c 207c 204c  LogTauTModel | L
-00029520: 6f67 5461 7548 4d6f 6465 6c20 7c20 4d75  ogTauHModel | Mu
-00029530: 6c74 694c 6f67 5461 7548 4d6f 6465 6c2c  ltiLogTauHModel,
-00029540: 2023 206e 6f71 610a 2020 2020 2020 2020   # noqa.        
-00029550: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-00029560: 655f 6e61 6d65 3a20 7374 722c 2076 6572  e_name: str, ver
-00029570: 626f 7365 3a20 626f 6f6c 203d 2054 7275  bose: bool = Tru
-00029580: 6529 202d 3e20 4e6f 6e65 3a0a 2020 2020  e) -> None:.    
-00029590: 2727 270a 2020 2020 4372 6561 7465 7320  '''.    Creates 
-000295a0: 6669 6c65 2063 6f6e 7461 696e 696e 6720  file containing 
-000295b0: 7261 7465 2076 7320 7465 6d70 6572 6174  rate vs temperat
-000295c0: 7572 652f 6669 656c 6420 6361 6c63 756c  ure/field calcul
-000295d0: 6174 6564 2075 7369 6e67 206d 6f64 656c  ated using model
-000295e0: 0a20 2020 2070 6172 616d 6574 6572 730a  .    parameters.
-000295f0: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
-00029600: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00029610: 2020 2064 6174 6173 6574 3a20 5461 7554     dataset: TauT
-00029620: 4461 7461 7365 7420 7c20 5461 7548 4461  Dataset | TauHDa
-00029630: 7461 7365 740a 2020 2020 2020 2020 4461  taset.        Da
-00029640: 7461 7365 7420 746f 2077 6869 6368 2061  taset to which a
-00029650: 206d 6f64 656c 2077 6173 2073 7563 6365   model was succe
-00029660: 7373 6675 6c6c 7920 6669 7474 6564 2028  ssfully fitted (
-00029670: 692e 652e 2066 6974 5f73 7461 7475 733d  i.e. fit_status=
-00029680: 5472 7565 290a 2020 2020 6d6f 6465 6c3a  True).    model:
-00029690: 204c 6f67 5461 7554 4d6f 6465 6c20 7c20   LogTauTModel | 
-000296a0: 4d75 6c74 694c 6f67 5461 7554 4d6f 6465  MultiLogTauTMode
-000296b0: 6c20 7c20 4c6f 6754 6175 484d 6f64 656c  l | LogTauHModel
-000296c0: 207c 204d 756c 7469 4c6f 6754 6175 484d   | MultiLogTauHM
-000296d0: 6f64 656c 0a20 2020 2020 2020 204d 6f64  odel.        Mod
-000296e0: 656c 2077 6869 6368 2068 6173 2062 6565  el which has bee
-000296f0: 6e20 6669 7474 6564 2074 6f20 6461 7461  n fitted to data
-00029700: 7365 740a 2020 2020 6669 6c65 5f6e 616d  set.    file_nam
-00029710: 653a 2073 7472 0a20 2020 2020 2020 204e  e: str.        N
-00029720: 616d 6520 6f66 206f 7574 7075 7420 6669  ame of output fi
-00029730: 6c65 0a20 2020 2076 6572 626f 7365 3a20  le.    verbose: 
-00029740: 626f 6f6c 2c20 6465 6661 756c 7420 5472  bool, default Tr
-00029750: 7565 0a20 2020 2020 2020 2049 6620 5472  ue.        If Tr
-00029760: 7565 2c20 6f75 7470 7574 2066 696c 6520  ue, output file 
-00029770: 6c6f 6361 7469 6f6e 2069 7320 7772 6974  location is writ
-00029780: 7465 6e20 746f 2074 6572 6d69 6e61 6c0a  ten to terminal.
-00029790: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
-000297a0: 202d 2d2d 2d2d 2d2d 0a20 2020 204e 6f6e   -------.    Non
-000297b0: 650a 2020 2020 2727 270a 0a20 2020 2069  e.    '''..    i
-000297c0: 6620 6e6f 7420 6d6f 6465 6c2e 6669 745f  f not model.fit_
-000297d0: 7374 6174 7573 3a0a 2020 2020 2020 2020  status:.        
-000297e0: 7265 7475 726e 0a0a 2020 2020 6966 2069  return..    if i
-000297f0: 7369 6e73 7461 6e63 6528 6461 7461 7365  sinstance(datase
-00029800: 742c 2054 6175 4844 6174 6173 6574 293a  t, TauHDataset):
-00029810: 0a20 2020 2020 2020 2078 5f76 616c 7320  .        x_vals 
-00029820: 3d20 636f 7079 2e63 6f70 7928 6461 7461  = copy.copy(data
-00029830: 7365 742e 6669 656c 6473 290a 2020 2020  set.fields).    
-00029840: 2020 2020 785f 7661 725f 6c61 6265 6c20      x_var_label 
-00029850: 3d20 2748 2028 4f65 2927 0a0a 2020 2020  = 'H (Oe)'..    
-00029860: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
-00029870: 6461 7461 7365 742c 2054 6175 5444 6174  dataset, TauTDat
-00029880: 6173 6574 293a 0a20 2020 2020 2020 2078  aset):.        x
-00029890: 5f76 616c 7320 3d20 636f 7079 2e63 6f70  _vals = copy.cop
-000298a0: 7928 6461 7461 7365 742e 7465 6d70 6572  y(dataset.temper
-000298b0: 6174 7572 6573 290a 2020 2020 2020 2020  atures).        
-000298c0: 785f 7661 725f 6c61 6265 6c20 3d20 2754  x_var_label = 'T
-000298d0: 2028 4b29 270a 0a20 2020 2069 6620 7479   (K)'..    if ty
-000298e0: 7065 286d 6f64 656c 2920 696e 205b 4d75  pe(model) in [Mu
-000298f0: 6c74 694c 6f67 5461 7554 4d6f 6465 6c2c  ltiLogTauTModel,
-00029900: 204d 756c 7469 4c6f 6754 6175 484d 6f64   MultiLogTauHMod
-00029910: 656c 5d3a 0a20 2020 2020 2020 206c 6f67  el]:.        log
-00029920: 6d6f 6465 6c73 203d 206d 6f64 656c 2e6c  models = model.l
-00029930: 6f67 6d6f 6465 6c73 0a20 2020 2065 6c73  ogmodels.    els
-00029940: 653a 0a20 2020 2020 2020 206c 6f67 6d6f  e:.        logmo
-00029950: 6465 6c73 203d 205b 6d6f 6465 6c5d 0a0a  dels = [model]..
-00029960: 2020 2020 6620 3d20 6f70 656e 2866 696c      f = open(fil
-00029970: 655f 6e61 6d65 2c20 2777 272c 2065 6e63  e_name, 'w', enc
-00029980: 6f64 696e 673d 2775 7466 2d38 2729 0a0a  oding='utf-8')..
-00029990: 2020 2020 785f 7661 7273 5f67 7269 6420      x_vars_grid 
-000299a0: 3d20 6e70 2e6c 696e 7370 6163 6528 0a20  = np.linspace(. 
-000299b0: 2020 2020 2020 206e 702e 6d69 6e28 785f         np.min(x_
-000299c0: 7661 6c73 292c 0a20 2020 2020 2020 206e  vals),.        n
-000299d0: 702e 6d61 7828 785f 7661 6c73 292c 0a20  p.max(x_vals),. 
-000299e0: 2020 2020 2020 2031 3030 300a 2020 2020         1000.    
-000299f0: 290a 0a20 2020 2066 2e77 7269 7465 2827  )..    f.write('
-00029a00: 7b3a 3e39 7d20 272e 666f 726d 6174 2878  {:>9} '.format(x
-00029a10: 5f76 6172 5f6c 6162 656c 2929 0a20 2020  _var_label)).   
-00029a20: 2066 6f72 206c 6f67 6d6f 6465 6c20 696e   for logmodel in
-00029a30: 206c 6f67 6d6f 6465 6c73 3a0a 2020 2020   logmodels:.    
-00029a40: 2020 2020 662e 7772 6974 6528 277b 3a3e      f.write('{:>
-00029a50: 377d 2072 6174 6520 272e 666f 726d 6174  7} rate '.format
-00029a60: 286c 6f67 6d6f 6465 6c2e 4e41 4d45 2929  (logmodel.NAME))
-00029a70: 0a20 2020 2069 6620 6c65 6e28 6c6f 676d  .    if len(logm
-00029a80: 6f64 656c 7329 203e 2031 3a0a 2020 2020  odels) > 1:.    
-00029a90: 2020 2020 662e 7772 6974 6528 2720 2054      f.write('  T
-00029aa0: 6f74 616c 2072 6174 6520 2873 5e2d 3129  otal rate (s^-1)
-00029ab0: 2729 0a20 2020 2066 2e77 7269 7465 2827  ').    f.write('
-00029ac0: 5c6e 2729 0a0a 2020 2020 666f 7220 6772  \n')..    for gr
-00029ad0: 6964 5f70 7420 696e 2078 5f76 6172 735f  id_pt in x_vars_
-00029ae0: 6772 6964 3a0a 2020 2020 2020 2020 662e  grid:.        f.
-00029af0: 7772 6974 6528 277b 3a20 392e 3566 7d20  write('{: 9.5f} 
-00029b00: 272e 666f 726d 6174 2867 7269 645f 7074  '.format(grid_pt
-00029b10: 2929 0a20 2020 2020 2020 2074 6f74 616c  )).        total
-00029b20: 203d 2030 2e0a 2020 2020 2020 2020 666f   = 0..        fo
-00029b30: 7220 6c6f 676d 6f64 656c 2069 6e20 6c6f  r logmodel in lo
-00029b40: 676d 6f64 656c 733a 0a20 2020 2020 2020  gmodels:.       
-00029b50: 2020 2020 2072 6174 6520 3d20 3130 2a2a       rate = 10**
-00029b60: 6c6f 676d 6f64 656c 2e6d 6f64 656c 280a  logmodel.model(.
-00029b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029b80: 6c6f 676d 6f64 656c 2e66 696e 616c 5f76  logmodel.final_v
-00029b90: 6172 5f76 616c 7565 732c 0a20 2020 2020  ar_values,.     
-00029ba0: 2020 2020 2020 2020 2020 205b 6772 6964             [grid
-00029bb0: 5f70 745d 0a20 2020 2020 2020 2020 2020  _pt].           
-00029bc0: 2029 5b30 5d0a 2020 2020 2020 2020 2020   )[0].          
-00029bd0: 2020 662e 7772 6974 6528 277b 3a2e 3645    f.write('{:.6E
-00029be0: 7d20 272e 666f 726d 6174 2872 6174 6529  } '.format(rate)
-00029bf0: 290a 2020 2020 2020 2020 2020 2020 746f  ).            to
-00029c00: 7461 6c20 2b3d 2072 6174 650a 2020 2020  tal += rate.    
-00029c10: 2020 2020 6966 206c 656e 286c 6f67 6d6f      if len(logmo
-00029c20: 6465 6c73 2920 3e20 313a 0a20 2020 2020  dels) > 1:.     
-00029c30: 2020 2020 2020 2066 2e77 7269 7465 2827         f.write('
-00029c40: 7b3a 2e36 457d 272e 666f 726d 6174 2874  {:.6E}'.format(t
-00029c50: 6f74 616c 2929 0a20 2020 2020 2020 2066  otal)).        f
-00029c60: 2e77 7269 7465 2827 5c6e 2729 0a0a 2020  .write('\n')..  
-00029c70: 2020 6966 2076 6572 626f 7365 3a0a 2020    if verbose:.  
-00029c80: 2020 2020 2020 7574 2e63 7072 696e 7428        ut.cprint(
-00029c90: 0a20 2020 2020 2020 2020 2020 2027 5c6e  .            '\n
-00029ca0: 2052 656c 6178 6174 696f 6e20 6d6f 6465   Relaxation mode
-00029cb0: 6c20 cf84 e281 bbc2 b920 7673 207b 7d20  l ....... vs {} 
-00029cc0: 7772 6974 7465 6e20 746f 205c 6e20 7b7d  written to \n {}
-00029cd0: 5c6e 272e 666f 726d 6174 280a 2020 2020  \n'.format(.    
-00029ce0: 2020 2020 2020 2020 2020 2020 785f 7661              x_va
-00029cf0: 725f 6c61 6265 6c5b 305d 2c0a 2020 2020  r_label[0],.    
-00029d00: 2020 2020 2020 2020 2020 2020 6669 6c65              file
-00029d10: 5f6e 616d 650a 2020 2020 2020 2020 2020  _name.          
-00029d20: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
-00029d30: 2027 6379 616e 270a 2020 2020 2020 2020   'cyan'.        
-00029d40: 290a 0a20 2020 2072 6574 7572 6e0a       )..    return.
+00028de0: 2020 2020 2020 2066 696c 655f 6e61 6d65         file_name
+00028df0: 3a20 7374 722c 2076 6572 626f 7365 3a20  : str, verbose: 
+00028e00: 626f 6f6c 203d 2054 7275 6529 202d 3e20  bool = True) -> 
+00028e10: 4e6f 6e65 3a0a 2020 2020 2727 270a 2020  None:.    '''.  
+00028e20: 2020 5772 6974 6573 2066 6974 7465 6420    Writes fitted 
+00028e30: 616e 6420 6669 7865 6420 7061 7261 6d65  and fixed parame
+00028e40: 7465 7273 206f 6620 6d6f 6465 6c28 7329  ters of model(s)
+00028e50: 2074 6f20 6669 6c65 0a0a 2020 2020 5061   to file..    Pa
+00028e60: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
+00028e70: 2d2d 2d2d 2d2d 2d0a 2020 2020 6d6f 6465  -------.    mode
+00028e80: 6c73 3a20 6c69 7374 5b4c 6f67 5461 7554  ls: list[LogTauT
+00028e90: 4d6f 6465 6c20 7c20 4d75 6c74 694c 6f67  Model | MultiLog
+00028ea0: 5461 7554 4d6f 6465 6c20 7c20 4c6f 6754  TauTModel | LogT
+00028eb0: 6175 484d 6f64 656c 207c 204d 756c 7469  auHModel | Multi
+00028ec0: 4c6f 6754 6175 484d 6f64 656c 5d0a 2020  LogTauHModel].  
+00028ed0: 2020 2020 2020 4d6f 6465 6c73 2c20 6f6e        Models, on
+00028ee0: 6520 7065 7220 7465 6d70 6572 6174 7572  e per temperatur
+00028ef0: 650a 2020 2020 6669 6c65 5f6e 616d 653a  e.    file_name:
+00028f00: 2073 7472 0a20 2020 2020 2020 204e 616d   str.        Nam
+00028f10: 6520 6f66 206f 7574 7075 7420 6669 6c65  e of output file
+00028f20: 0a20 2020 2076 6572 626f 7365 3a20 626f  .    verbose: bo
+00028f30: 6f6c 2c20 6465 6661 756c 7420 5472 7565  ol, default True
+00028f40: 0a20 2020 2020 2020 2049 6620 5472 7565  .        If True
+00028f50: 2c20 6f75 7470 7574 2066 696c 6520 6c6f  , output file lo
+00028f60: 6361 7469 6f6e 2069 7320 7772 6974 7465  cation is writte
+00028f70: 6e20 746f 2074 6572 6d69 6e61 6c0a 0a20  n to terminal.. 
+00028f80: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
+00028f90: 2d2d 2d2d 2d2d 0a20 2020 204e 6f6e 650a  ------.    None.
+00028fa0: 2020 2020 2727 2720 2320 6e6f 7161 0a0a      ''' # noqa..
+00028fb0: 2020 2020 6966 2074 7970 6528 6d6f 6465      if type(mode
+00028fc0: 6c29 2069 6e20 5b4d 756c 7469 4c6f 6754  l) in [MultiLogT
+00028fd0: 6175 544d 6f64 656c 2c20 4d75 6c74 694c  auTModel, MultiL
+00028fe0: 6f67 5461 7548 4d6f 6465 6c5d 3a0a 2020  ogTauHModel]:.  
+00028ff0: 2020 2020 2020 6c6f 676d 6f64 656c 7320        logmodels 
+00029000: 3d20 6d6f 6465 6c2e 6c6f 676d 6f64 656c  = model.logmodel
+00029010: 730a 2020 2020 656c 7365 3a0a 2020 2020  s.    else:.    
+00029020: 2020 2020 6c6f 676d 6f64 656c 7320 3d20      logmodels = 
+00029030: 5b6d 6f64 656c 5d0a 0a20 2020 2066 203d  [model]..    f =
+00029040: 206f 7065 6e28 6669 6c65 5f6e 616d 652c   open(file_name,
+00029050: 2027 7727 2c20 656e 636f 6469 6e67 3d27   'w', encoding='
+00029060: 7574 662d 3827 290a 0a20 2020 2023 2057  utf-8')..    # W
+00029070: 7269 7465 2065 6163 6820 7465 726d 2773  rite each term's
+00029080: 206e 616d 652c 2066 6974 2076 6172 732c   name, fit vars,
+00029090: 2073 7464 6576 2c20 616e 6420 6669 7820   stdev, and fix 
+000290a0: 7661 7273 0a20 2020 2066 6f72 206c 6f67  vars.    for log
+000290b0: 6d6f 6465 6c20 696e 206c 6f67 6d6f 6465  model in logmode
+000290c0: 6c73 3a0a 2020 2020 2020 2020 662e 7772  ls:.        f.wr
+000290d0: 6974 6528 277b 7d5c 6e27 2e66 6f72 6d61  ite('{}\n'.forma
+000290e0: 7428 6c6f 676d 6f64 656c 2e4e 414d 4529  t(logmodel.NAME)
+000290f0: 290a 2020 2020 2020 2020 6966 206c 656e  ).        if len
+00029100: 286c 6f67 6d6f 6465 6c2e 6669 745f 7661  (logmodel.fit_va
+00029110: 7273 2e6b 6579 7328 2929 3a0a 2020 2020  rs.keys()):.    
+00029120: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
+00029130: 2746 6974 7465 6420 5465 726d 733a 2056  'Fitted Terms: V
+00029140: 616c 7565 2061 6e64 2053 7461 6e64 6172  alue and Standar
+00029150: 6420 4465 7669 6174 696f 6e3a 5c6e 2729  d Deviation:\n')
+00029160: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00029170: 206e 616d 6520 696e 206c 6f67 6d6f 6465   name in logmode
+00029180: 6c2e 6669 745f 7661 7273 2e6b 6579 7328  l.fit_vars.keys(
+00029190: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000291a0: 2020 2066 2e77 7269 7465 2827 7b3a 3e36     f.write('{:>6
+000291b0: 7d20 7b3a 2031 2e38 457d 207b 3a20 312e  } {: 1.8E} {: 1.
+000291c0: 3845 7d20 7b7d 5c6e 272e 666f 726d 6174  8E} {}\n'.format
+000291d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000291e0: 2020 2020 2020 6e61 6d65 2c0a 2020 2020        name,.    
+000291f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029200: 6c6f 676d 6f64 656c 2e66 696e 616c 5f76  logmodel.final_v
+00029210: 6172 5f76 616c 7565 735b 6e61 6d65 5d2c  ar_values[name],
+00029220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00029230: 2020 2020 206c 6f67 6d6f 6465 6c2e 6669       logmodel.fi
+00029240: 745f 7374 6465 765b 6e61 6d65 5d2c 0a20  t_stdev[name],. 
+00029250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029260: 2020 206c 6f67 6d6f 6465 6c2e 554e 4954     logmodel.UNIT
+00029270: 535b 6e61 6d65 5d0a 2020 2020 2020 2020  S[name].        
+00029280: 2020 2020 2020 2020 2929 0a20 2020 2020          )).     
+00029290: 2020 2069 6620 6c65 6e28 6c6f 676d 6f64     if len(logmod
+000292a0: 656c 2e66 6978 5f76 6172 732e 6b65 7973  el.fix_vars.keys
+000292b0: 2829 293a 0a20 2020 2020 2020 2020 2020  ()):.           
+000292c0: 2066 2e77 7269 7465 2827 4669 7865 6420   f.write('Fixed 
+000292d0: 5465 726d 733a 2056 616c 7565 735c 6e27  Terms: Values\n'
+000292e0: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
+000292f0: 7220 6e61 6d65 2069 6e20 6c6f 676d 6f64  r name in logmod
+00029300: 656c 2e66 6978 5f76 6172 732e 6b65 7973  el.fix_vars.keys
+00029310: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00029320: 2020 2020 662e 7772 6974 6528 277b 3a3e      f.write('{:>
+00029330: 367d 207b 3a20 312e 3845 7d20 7b7d 5c6e  6} {: 1.8E} {}\n
+00029340: 272e 666f 726d 6174 280a 2020 2020 2020  '.format(.      
+00029350: 2020 2020 2020 2020 2020 2020 2020 6e61                na
+00029360: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
+00029370: 2020 2020 2020 2020 6c6f 676d 6f64 656c          logmodel
+00029380: 2e66 696e 616c 5f76 6172 5f76 616c 7565  .final_var_value
+00029390: 735b 6e61 6d65 5d2c 0a20 2020 2020 2020  s[name],.       
+000293a0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+000293b0: 6d6f 6465 6c2e 554e 4954 535b 6e61 6d65  model.UNITS[name
+000293c0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+000293d0: 2020 2929 0a20 2020 2020 2020 2066 2e77    )).        f.w
+000293e0: 7269 7465 2827 5c6e 2729 0a0a 2020 2020  rite('\n')..    
+000293f0: 6966 2076 6572 626f 7365 3a0a 2020 2020  if verbose:.    
+00029400: 2020 2020 7574 2e63 7072 696e 7428 0a20      ut.cprint(. 
+00029410: 2020 2020 2020 2020 2020 2027 5c6e 2052             '\n R
+00029420: 656c 6178 6174 696f 6e20 4d6f 6465 6c20  elaxation Model 
+00029430: 7061 7261 6d65 7465 7273 2077 7269 7474  parameters writt
+00029440: 656e 2074 6f20 5c6e 207b 7d5c 6e27 2e66  en to \n {}\n'.f
+00029450: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
+00029460: 2020 2020 2020 2066 696c 655f 6e61 6d65         file_name
+00029470: 0a20 2020 2020 2020 2020 2020 2029 2c0a  .            ),.
+00029480: 2020 2020 2020 2020 2020 2020 2763 7961              'cya
+00029490: 6e27 0a20 2020 2020 2020 2029 0a0a 2020  n'.        )..  
+000294a0: 2020 7265 7475 726e 0a0a 0a64 6566 2077    return...def w
+000294b0: 7269 7465 5f6d 6f64 656c 5f64 6174 6128  rite_model_data(
+000294c0: 6461 7461 7365 743a 2054 6175 5444 6174  dataset: TauTDat
+000294d0: 6173 6574 207c 2054 6175 4844 6174 6173  aset | TauHDatas
+000294e0: 6574 2c0a 2020 2020 2020 2020 2020 2020  et,.            
+000294f0: 2020 2020 2020 2020 206d 6f64 656c 3a20           model: 
+00029500: 4c6f 6754 6175 544d 6f64 656c 207c 204d  LogTauTModel | M
+00029510: 756c 7469 4c6f 6754 6175 544d 6f64 656c  ultiLogTauTModel
+00029520: 207c 204c 6f67 5461 7548 4d6f 6465 6c20   | LogTauHModel 
+00029530: 7c20 4d75 6c74 694c 6f67 5461 7548 4d6f  | MultiLogTauHMo
+00029540: 6465 6c2c 2023 206e 6f71 610a 2020 2020  del, # noqa.    
+00029550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029560: 2066 696c 655f 6e61 6d65 3a20 7374 722c   file_name: str,
+00029570: 2076 6572 626f 7365 3a20 626f 6f6c 203d   verbose: bool =
+00029580: 2054 7275 6529 202d 3e20 4e6f 6e65 3a0a   True) -> None:.
+00029590: 2020 2020 2727 270a 2020 2020 4372 6561      '''.    Crea
+000295a0: 7465 7320 6669 6c65 2063 6f6e 7461 696e  tes file contain
+000295b0: 696e 6720 7261 7465 2076 7320 7465 6d70  ing rate vs temp
+000295c0: 6572 6174 7572 652f 6669 656c 6420 6361  erature/field ca
+000295d0: 6c63 756c 6174 6564 2075 7369 6e67 206d  lculated using m
+000295e0: 6f64 656c 0a20 2020 2070 6172 616d 6574  odel.    paramet
+000295f0: 6572 730a 0a20 2020 2050 6172 616d 6574  ers..    Paramet
+00029600: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
+00029610: 2d2d 0a20 2020 2064 6174 6173 6574 3a20  --.    dataset: 
+00029620: 5461 7554 4461 7461 7365 7420 7c20 5461  TauTDataset | Ta
+00029630: 7548 4461 7461 7365 740a 2020 2020 2020  uHDataset.      
+00029640: 2020 4461 7461 7365 7420 746f 2077 6869    Dataset to whi
+00029650: 6368 2061 206d 6f64 656c 2077 6173 2073  ch a model was s
+00029660: 7563 6365 7373 6675 6c6c 7920 6669 7474  uccessfully fitt
+00029670: 6564 2028 692e 652e 2066 6974 5f73 7461  ed (i.e. fit_sta
+00029680: 7475 733d 5472 7565 290a 2020 2020 6d6f  tus=True).    mo
+00029690: 6465 6c3a 204c 6f67 5461 7554 4d6f 6465  del: LogTauTMode
+000296a0: 6c20 7c20 4d75 6c74 694c 6f67 5461 7554  l | MultiLogTauT
+000296b0: 4d6f 6465 6c20 7c20 4c6f 6754 6175 484d  Model | LogTauHM
+000296c0: 6f64 656c 207c 204d 756c 7469 4c6f 6754  odel | MultiLogT
+000296d0: 6175 484d 6f64 656c 0a20 2020 2020 2020  auHModel.       
+000296e0: 204d 6f64 656c 2077 6869 6368 2068 6173   Model which has
+000296f0: 2062 6565 6e20 6669 7474 6564 2074 6f20   been fitted to 
+00029700: 6461 7461 7365 740a 2020 2020 6669 6c65  dataset.    file
+00029710: 5f6e 616d 653a 2073 7472 0a20 2020 2020  _name: str.     
+00029720: 2020 204e 616d 6520 6f66 206f 7574 7075     Name of outpu
+00029730: 7420 6669 6c65 0a20 2020 2076 6572 626f  t file.    verbo
+00029740: 7365 3a20 626f 6f6c 2c20 6465 6661 756c  se: bool, defaul
+00029750: 7420 5472 7565 0a20 2020 2020 2020 2049  t True.        I
+00029760: 6620 5472 7565 2c20 6f75 7470 7574 2066  f True, output f
+00029770: 696c 6520 6c6f 6361 7469 6f6e 2069 7320  ile location is 
+00029780: 7772 6974 7465 6e20 746f 2074 6572 6d69  written to termi
+00029790: 6e61 6c0a 0a20 2020 2052 6574 7572 6e73  nal..    Returns
+000297a0: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
+000297b0: 204e 6f6e 650a 2020 2020 2727 270a 0a20   None.    '''.. 
+000297c0: 2020 2069 6620 6e6f 7420 6d6f 6465 6c2e     if not model.
+000297d0: 6669 745f 7374 6174 7573 3a0a 2020 2020  fit_status:.    
+000297e0: 2020 2020 7265 7475 726e 0a0a 2020 2020      return..    
+000297f0: 6966 2069 7369 6e73 7461 6e63 6528 6461  if isinstance(da
+00029800: 7461 7365 742c 2054 6175 4844 6174 6173  taset, TauHDatas
+00029810: 6574 293a 0a20 2020 2020 2020 2078 5f76  et):.        x_v
+00029820: 616c 7320 3d20 636f 7079 2e63 6f70 7928  als = copy.copy(
+00029830: 6461 7461 7365 742e 6669 656c 6473 290a  dataset.fields).
+00029840: 2020 2020 2020 2020 785f 7661 725f 6c61          x_var_la
+00029850: 6265 6c20 3d20 2748 2028 4f65 2927 0a0a  bel = 'H (Oe)'..
+00029860: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
+00029870: 6e63 6528 6461 7461 7365 742c 2054 6175  nce(dataset, Tau
+00029880: 5444 6174 6173 6574 293a 0a20 2020 2020  TDataset):.     
+00029890: 2020 2078 5f76 616c 7320 3d20 636f 7079     x_vals = copy
+000298a0: 2e63 6f70 7928 6461 7461 7365 742e 7465  .copy(dataset.te
+000298b0: 6d70 6572 6174 7572 6573 290a 2020 2020  mperatures).    
+000298c0: 2020 2020 785f 7661 725f 6c61 6265 6c20      x_var_label 
+000298d0: 3d20 2754 2028 4b29 270a 0a20 2020 2069  = 'T (K)'..    i
+000298e0: 6620 7479 7065 286d 6f64 656c 2920 696e  f type(model) in
+000298f0: 205b 4d75 6c74 694c 6f67 5461 7554 4d6f   [MultiLogTauTMo
+00029900: 6465 6c2c 204d 756c 7469 4c6f 6754 6175  del, MultiLogTau
+00029910: 484d 6f64 656c 5d3a 0a20 2020 2020 2020  HModel]:.       
+00029920: 206c 6f67 6d6f 6465 6c73 203d 206d 6f64   logmodels = mod
+00029930: 656c 2e6c 6f67 6d6f 6465 6c73 0a20 2020  el.logmodels.   
+00029940: 2065 6c73 653a 0a20 2020 2020 2020 206c   else:.        l
+00029950: 6f67 6d6f 6465 6c73 203d 205b 6d6f 6465  ogmodels = [mode
+00029960: 6c5d 0a0a 2020 2020 6620 3d20 6f70 656e  l]..    f = open
+00029970: 2866 696c 655f 6e61 6d65 2c20 2777 272c  (file_name, 'w',
+00029980: 2065 6e63 6f64 696e 673d 2775 7466 2d38   encoding='utf-8
+00029990: 2729 0a0a 2020 2020 785f 7661 7273 5f67  ')..    x_vars_g
+000299a0: 7269 6420 3d20 6e70 2e6c 696e 7370 6163  rid = np.linspac
+000299b0: 6528 0a20 2020 2020 2020 206e 702e 6d69  e(.        np.mi
+000299c0: 6e28 785f 7661 6c73 292c 0a20 2020 2020  n(x_vals),.     
+000299d0: 2020 206e 702e 6d61 7828 785f 7661 6c73     np.max(x_vals
+000299e0: 292c 0a20 2020 2020 2020 2031 3030 300a  ),.        1000.
+000299f0: 2020 2020 290a 0a20 2020 2066 2e77 7269      )..    f.wri
+00029a00: 7465 2827 7b3a 3e39 7d20 272e 666f 726d  te('{:>9} '.form
+00029a10: 6174 2878 5f76 6172 5f6c 6162 656c 2929  at(x_var_label))
+00029a20: 0a20 2020 2066 6f72 206c 6f67 6d6f 6465  .    for logmode
+00029a30: 6c20 696e 206c 6f67 6d6f 6465 6c73 3a0a  l in logmodels:.
+00029a40: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
+00029a50: 277b 3a3e 377d 2072 6174 6520 272e 666f  '{:>7} rate '.fo
+00029a60: 726d 6174 286c 6f67 6d6f 6465 6c2e 4e41  rmat(logmodel.NA
+00029a70: 4d45 2929 0a20 2020 2069 6620 6c65 6e28  ME)).    if len(
+00029a80: 6c6f 676d 6f64 656c 7329 203e 2031 3a0a  logmodels) > 1:.
+00029a90: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
+00029aa0: 2720 2054 6f74 616c 2072 6174 6520 2873  '  Total rate (s
+00029ab0: 5e2d 3129 2729 0a20 2020 2066 2e77 7269  ^-1)').    f.wri
+00029ac0: 7465 2827 5c6e 2729 0a0a 2020 2020 666f  te('\n')..    fo
+00029ad0: 7220 6772 6964 5f70 7420 696e 2078 5f76  r grid_pt in x_v
+00029ae0: 6172 735f 6772 6964 3a0a 2020 2020 2020  ars_grid:.      
+00029af0: 2020 662e 7772 6974 6528 277b 3a20 392e    f.write('{: 9.
+00029b00: 3566 7d20 272e 666f 726d 6174 2867 7269  5f} '.format(gri
+00029b10: 645f 7074 2929 0a20 2020 2020 2020 2074  d_pt)).        t
+00029b20: 6f74 616c 203d 2030 2e0a 2020 2020 2020  otal = 0..      
+00029b30: 2020 666f 7220 6c6f 676d 6f64 656c 2069    for logmodel i
+00029b40: 6e20 6c6f 676d 6f64 656c 733a 0a20 2020  n logmodels:.   
+00029b50: 2020 2020 2020 2020 2072 6174 6520 3d20           rate = 
+00029b60: 3130 2a2a 6c6f 676d 6f64 656c 2e6d 6f64  10**logmodel.mod
+00029b70: 656c 280a 2020 2020 2020 2020 2020 2020  el(.            
+00029b80: 2020 2020 6c6f 676d 6f64 656c 2e66 696e      logmodel.fin
+00029b90: 616c 5f76 6172 5f76 616c 7565 732c 0a20  al_var_values,. 
+00029ba0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+00029bb0: 6772 6964 5f70 745d 0a20 2020 2020 2020  grid_pt].       
+00029bc0: 2020 2020 2029 5b30 5d0a 2020 2020 2020       )[0].      
+00029bd0: 2020 2020 2020 662e 7772 6974 6528 277b        f.write('{
+00029be0: 3a2e 3645 7d20 272e 666f 726d 6174 2872  :.6E} '.format(r
+00029bf0: 6174 6529 290a 2020 2020 2020 2020 2020  ate)).          
+00029c00: 2020 746f 7461 6c20 2b3d 2072 6174 650a    total += rate.
+00029c10: 2020 2020 2020 2020 6966 206c 656e 286c          if len(l
+00029c20: 6f67 6d6f 6465 6c73 2920 3e20 313a 0a20  ogmodels) > 1:. 
+00029c30: 2020 2020 2020 2020 2020 2066 2e77 7269             f.wri
+00029c40: 7465 2827 7b3a 2e36 457d 272e 666f 726d  te('{:.6E}'.form
+00029c50: 6174 2874 6f74 616c 2929 0a20 2020 2020  at(total)).     
+00029c60: 2020 2066 2e77 7269 7465 2827 5c6e 2729     f.write('\n')
+00029c70: 0a0a 2020 2020 6966 2076 6572 626f 7365  ..    if verbose
+00029c80: 3a0a 2020 2020 2020 2020 7574 2e63 7072  :.        ut.cpr
+00029c90: 696e 7428 0a20 2020 2020 2020 2020 2020  int(.           
+00029ca0: 2027 5c6e 2052 656c 6178 6174 696f 6e20   '\n Relaxation 
+00029cb0: 6d6f 6465 6c20 cf84 e281 bbc2 b920 7673  model ....... vs
+00029cc0: 207b 7d20 7772 6974 7465 6e20 746f 205c   {} written to \
+00029cd0: 6e20 7b7d 5c6e 272e 666f 726d 6174 280a  n {}\n'.format(.
+00029ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029cf0: 785f 7661 725f 6c61 6265 6c5b 305d 2c0a  x_var_label[0],.
+00029d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029d10: 6669 6c65 5f6e 616d 650a 2020 2020 2020  file_name.      
+00029d20: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
+00029d30: 2020 2020 2027 6379 616e 270a 2020 2020       'cyan'.    
+00029d40: 2020 2020 290a 0a20 2020 2072 6574 7572      )..    retur
+00029d50: 6e0a                                     n.
```

### Comparing `ccfit2-5.1.3/ccfit2/stats.py` & `ccfit2-5.1.4/ccfit2/stats.py`

 * *Files identical despite different names*

### Comparing `ccfit2-5.1.3/ccfit2/utils.py` & `ccfit2-5.1.4/ccfit2/utils.py`

 * *Files identical despite different names*

### Comparing `ccfit2-5.1.3/ccfit2/waveform.py` & `ccfit2-5.1.4/ccfit2/waveform.py`

 * *Files identical despite different names*

### Comparing `ccfit2-5.1.3/ccfit2.egg-info/PKG-INFO` & `ccfit2-5.1.4/ccfit2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccfit2
-Version: 5.1.3
+Version: 5.1.4
 Summary: CCFIT2 is a program for fitting AC and DC magnetisation data
 Home-page: https://gitlab.com/chilton-group/cc-fit2
 Author: Daniel Reta
 Author-email: danielreta1@gmail.com
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/cc-fit2/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/cc-fit2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ccfit2-5.1.3/setup.py` & `ccfit2-5.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 # DO NOT EDIT THIS NUMBER!
 # IT IS AUTOMATICALLY CHANGED BY python-semantic-release
-__version__ = "5.1.3"
+__version__ = "5.1.4"
 
 setuptools.setup(
     name='ccfit2',
     version=__version__,
     author='Daniel Reta',
     author_email='danielreta1@gmail.com',
     description='CCFIT2 is a program for fitting AC and DC magnetisation data', # noqa
```

