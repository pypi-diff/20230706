# Comparing `tmp/cryspy_editor-1.6.9.tar.gz` & `tmp/cryspy_editor-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryspy_editor-1.6.9.tar", last modified: Fri Dec  2 15:02:28 2022, max compression
+gzip compressed data, was "cryspy_editor-1.7.0.tar", last modified: Thu Jul  6 15:19:15 2023, max compression
```

## Comparing `cryspy_editor-1.6.9.tar` & `cryspy_editor-1.7.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2022-12-02 15:02:28.642730 cryspy_editor-1.6.9/
--rw-rw-rw-   0        0        0     1090 2021-10-19 16:23:12.000000 cryspy_editor-1.6.9/LICENSE
--rw-rw-rw-   0        0        0       90 2020-09-15 11:31:18.000000 cryspy_editor-1.6.9/MANIFEST.in
--rw-rw-rw-   0        0        0      736 2022-12-02 15:02:28.640722 cryspy_editor-1.6.9/PKG-INFO
--rw-rw-rw-   0        0        0       43 2021-10-19 16:23:12.000000 cryspy_editor-1.6.9/README.md
-drwxrwxrwx   0        0        0        0 2022-12-02 15:02:28.545212 cryspy_editor-1.6.9/cryspy_editor/
--rw-rw-rw-   0        0        0      166 2022-12-02 15:01:31.000000 cryspy_editor-1.6.9/cryspy_editor/__init__.py
--rw-rw-rw-   0        0        0     1048 2022-05-05 11:54:19.000000 cryspy_editor-1.6.9/cryspy_editor/__main__.py
--rw-rw-rw-   0        0        0    37319 2022-12-02 15:00:59.000000 cryspy_editor-1.6.9/cryspy_editor/ceditor.py
--rw-rw-rw-   0        0        0     4193 2022-05-17 14:09:19.000000 cryspy_editor-1.6.9/cryspy_editor/cl_thread.py
-drwxrwxrwx   0        0        0        0 2022-12-02 15:02:28.624042 cryspy_editor-1.6.9/cryspy_editor/f_icon/
--rw-rw-rw-   0        0        0        0 2019-09-13 14:30:22.000000 cryspy_editor-1.6.9/cryspy_editor/f_icon/__init__.py
--rw-rw-rw-   0        0        0  2345529 2020-09-15 10:04:31.000000 cryspy_editor-1.6.9/cryspy_editor/f_icon/calc.gif
--rw-rw-rw-   0        0        0    29962 2019-09-13 14:30:22.000000 cryspy_editor-1.6.9/cryspy_editor/f_icon/calc_rcif.png
--rw-rw-rw-   0        0        0    98264 2020-08-24 11:04:57.000000 cryspy_editor-1.6.9/cryspy_editor/f_icon/flip.png
--rw-rw-rw-   0        0        0    10108 2020-06-02 21:21:38.000000 cryspy_editor-1.6.9/cryspy_editor/f_icon/graph.png
--rw-rw-rw-   0        0        0   113548 2019-11-07 23:29:40.000000 cryspy_editor-1.6.9/cryspy_editor/f_icon/icon.png
--rw-rw-rw-   0        0        0    39486 2022-04-13 12:41:34.000000 cryspy_editor-1.6.9/cryspy_editor/f_icon/logo.png
--rw-rw-rw-   0        0        0    26227 2019-11-07 22:20:40.000000 cryspy_editor-1.6.9/cryspy_editor/f_icon/new.png
--rw-rw-rw-   0        0        0    49862 2019-11-07 22:17:52.000000 cryspy_editor-1.6.9/cryspy_editor/f_icon/open.png
--rw-rw-rw-   0        0        0   143269 2019-09-13 14:30:22.000000 cryspy_editor-1.6.9/cryspy_editor/f_icon/open_folder.png
--rw-rw-rw-   0        0        0  3988101 2020-12-27 13:01:23.000000 cryspy_editor-1.6.9/cryspy_editor/f_icon/pm.gif
--rw-rw-rw-   0        0        0    43680 2020-08-23 19:18:18.000000 cryspy_editor-1.6.9/cryspy_editor/f_icon/refresh.png
--rw-rw-rw-   0        0        0    25022 2019-11-07 22:56:40.000000 cryspy_editor-1.6.9/cryspy_editor/f_icon/save.png
--rw-rw-rw-   0        0        0    64331 2019-11-05 11:24:32.000000 cryspy_editor-1.6.9/cryspy_editor/f_icon/save_.png
--rw-rw-rw-   0        0        0    41818 2019-11-07 23:03:38.000000 cryspy_editor-1.6.9/cryspy_editor/f_icon/save_as.png
--rw-rw-rw-   0        0        0    51960 2019-11-05 11:25:28.000000 cryspy_editor-1.6.9/cryspy_editor/f_icon/save_as_.png
--rw-rw-rw-   0        0        0    99105 2019-11-06 23:02:14.000000 cryspy_editor-1.6.9/cryspy_editor/f_icon/to_cryspy.png
--rw-rw-rw-   0        0        0   178186 2019-11-05 11:29:32.000000 cryspy_editor-1.6.9/cryspy_editor/f_icon/to_cryspy_.png
--rw-rw-rw-   0        0        0   108844 2020-01-07 15:47:24.000000 cryspy_editor-1.6.9/cryspy_editor/f_icon/to_magref.png
--rw-rw-rw-   0        0        0    53109 2019-11-08 13:27:48.000000 cryspy_editor-1.6.9/cryspy_editor/f_icon/to_mem.png
--rw-rw-rw-   0        0        0    94484 2019-11-06 22:42:32.000000 cryspy_editor-1.6.9/cryspy_editor/f_icon/to_rhochi.png
--rw-rw-rw-   0        0        0   168743 2019-11-05 11:22:48.000000 cryspy_editor-1.6.9/cryspy_editor/f_icon/to_rhochi_.png
--rw-rw-rw-   0        0        0   104476 2019-11-06 22:40:08.000000 cryspy_editor-1.6.9/cryspy_editor/f_icon/to_star.png
--rw-rw-rw-   0        0        0   111744 2019-11-05 11:27:06.000000 cryspy_editor-1.6.9/cryspy_editor/f_icon/to_star_.png
-drwxrwxrwx   0        0        0        0 2022-12-02 15:02:28.638073 cryspy_editor-1.6.9/cryspy_editor/widgets/
--rw-rw-rw-   0        0        0        0 2020-03-06 09:15:20.000000 cryspy_editor-1.6.9/cryspy_editor/widgets/__init__.py
--rw-rw-rw-   0        0        0     7842 2022-04-29 16:32:34.000000 cryspy_editor-1.6.9/cryspy_editor/widgets/cryspy_objects.py
--rw-rw-rw-   0        0        0     1808 2022-02-08 10:47:56.000000 cryspy_editor-1.6.9/cryspy_editor/widgets/matplotlib.py
--rw-rw-rw-   0        0        0     1214 2022-02-08 10:47:50.000000 cryspy_editor-1.6.9/cryspy_editor/widgets/w_editcif.py
--rw-rw-rw-   0        0        0    12691 2022-04-29 16:59:23.000000 cryspy_editor-1.6.9/cryspy_editor/widgets/w_function.py
--rw-rw-rw-   0        0        0     3109 2022-10-21 13:03:13.000000 cryspy_editor-1.6.9/cryspy_editor/widgets/w_object_panel.py
-drwxrwxrwx   0        0        0        0 2022-12-02 15:02:28.555329 cryspy_editor-1.6.9/cryspy_editor.egg-info/
--rw-rw-rw-   0        0        0      736 2022-12-02 15:02:28.000000 cryspy_editor-1.6.9/cryspy_editor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1327 2022-12-02 15:02:28.000000 cryspy_editor-1.6.9/cryspy_editor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-02 15:02:28.000000 cryspy_editor-1.6.9/cryspy_editor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2022-12-02 15:02:28.000000 cryspy_editor-1.6.9/cryspy_editor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-12-02 15:02:28.000000 cryspy_editor-1.6.9/cryspy_editor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-02 15:02:28.642730 cryspy_editor-1.6.9/setup.cfg
--rw-rw-rw-   0        0        0     2815 2022-12-02 15:01:55.000000 cryspy_editor-1.6.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:19:15.197919 cryspy_editor-1.7.0/
+-rw-rw-rw-   0        0        0     1090 2021-10-19 16:23:12.000000 cryspy_editor-1.7.0/LICENSE
+-rw-rw-rw-   0        0        0       90 2020-09-15 11:31:18.000000 cryspy_editor-1.7.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      704 2023-07-06 15:19:15.197919 cryspy_editor-1.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0       43 2021-10-19 16:23:12.000000 cryspy_editor-1.7.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 15:19:15.115775 cryspy_editor-1.7.0/cryspy_editor/
+-rw-rw-rw-   0        0        0      166 2023-07-06 15:18:51.000000 cryspy_editor-1.7.0/cryspy_editor/__init__.py
+-rw-rw-rw-   0        0        0     1048 2022-05-05 11:54:19.000000 cryspy_editor-1.7.0/cryspy_editor/__main__.py
+-rw-rw-rw-   0        0        0    38932 2023-03-15 12:56:40.000000 cryspy_editor-1.7.0/cryspy_editor/ceditor.py
+-rw-rw-rw-   0        0        0     4193 2022-05-17 14:09:19.000000 cryspy_editor-1.7.0/cryspy_editor/cl_thread.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:19:15.185963 cryspy_editor-1.7.0/cryspy_editor/f_icon/
+-rw-rw-rw-   0        0        0        0 2019-09-13 14:30:22.000000 cryspy_editor-1.7.0/cryspy_editor/f_icon/__init__.py
+-rw-rw-rw-   0        0        0  2345529 2020-09-15 10:04:31.000000 cryspy_editor-1.7.0/cryspy_editor/f_icon/calc.gif
+-rw-rw-rw-   0        0        0    29962 2019-09-13 14:30:22.000000 cryspy_editor-1.7.0/cryspy_editor/f_icon/calc_rcif.png
+-rw-rw-rw-   0        0        0    98264 2020-08-24 11:04:57.000000 cryspy_editor-1.7.0/cryspy_editor/f_icon/flip.png
+-rw-rw-rw-   0        0        0    10108 2020-06-02 21:21:38.000000 cryspy_editor-1.7.0/cryspy_editor/f_icon/graph.png
+-rw-rw-rw-   0        0        0   113548 2019-11-07 23:29:40.000000 cryspy_editor-1.7.0/cryspy_editor/f_icon/icon.png
+-rw-rw-rw-   0        0        0    39486 2022-04-13 12:41:34.000000 cryspy_editor-1.7.0/cryspy_editor/f_icon/logo.png
+-rw-rw-rw-   0        0        0    26227 2019-11-07 22:20:40.000000 cryspy_editor-1.7.0/cryspy_editor/f_icon/new.png
+-rw-rw-rw-   0        0        0    49862 2019-11-07 22:17:52.000000 cryspy_editor-1.7.0/cryspy_editor/f_icon/open.png
+-rw-rw-rw-   0        0        0   143269 2019-09-13 14:30:22.000000 cryspy_editor-1.7.0/cryspy_editor/f_icon/open_folder.png
+-rw-rw-rw-   0        0        0  3988101 2020-12-27 13:01:23.000000 cryspy_editor-1.7.0/cryspy_editor/f_icon/pm.gif
+-rw-rw-rw-   0        0        0    43680 2020-08-23 19:18:18.000000 cryspy_editor-1.7.0/cryspy_editor/f_icon/refresh.png
+-rw-rw-rw-   0        0        0    25022 2019-11-07 22:56:40.000000 cryspy_editor-1.7.0/cryspy_editor/f_icon/save.png
+-rw-rw-rw-   0        0        0    64331 2019-11-05 11:24:32.000000 cryspy_editor-1.7.0/cryspy_editor/f_icon/save_.png
+-rw-rw-rw-   0        0        0    41818 2019-11-07 23:03:38.000000 cryspy_editor-1.7.0/cryspy_editor/f_icon/save_as.png
+-rw-rw-rw-   0        0        0    51960 2019-11-05 11:25:28.000000 cryspy_editor-1.7.0/cryspy_editor/f_icon/save_as_.png
+-rw-rw-rw-   0        0        0    99105 2019-11-06 23:02:14.000000 cryspy_editor-1.7.0/cryspy_editor/f_icon/to_cryspy.png
+-rw-rw-rw-   0        0        0   178186 2019-11-05 11:29:32.000000 cryspy_editor-1.7.0/cryspy_editor/f_icon/to_cryspy_.png
+-rw-rw-rw-   0        0        0   108844 2020-01-07 15:47:24.000000 cryspy_editor-1.7.0/cryspy_editor/f_icon/to_magref.png
+-rw-rw-rw-   0        0        0    53109 2019-11-08 13:27:48.000000 cryspy_editor-1.7.0/cryspy_editor/f_icon/to_mem.png
+-rw-rw-rw-   0        0        0    94484 2019-11-06 22:42:32.000000 cryspy_editor-1.7.0/cryspy_editor/f_icon/to_rhochi.png
+-rw-rw-rw-   0        0        0   168743 2019-11-05 11:22:48.000000 cryspy_editor-1.7.0/cryspy_editor/f_icon/to_rhochi_.png
+-rw-rw-rw-   0        0        0   104476 2019-11-06 22:40:08.000000 cryspy_editor-1.7.0/cryspy_editor/f_icon/to_star.png
+-rw-rw-rw-   0        0        0   111744 2019-11-05 11:27:06.000000 cryspy_editor-1.7.0/cryspy_editor/f_icon/to_star_.png
+drwxrwxrwx   0        0        0        0 2023-07-06 15:19:15.195904 cryspy_editor-1.7.0/cryspy_editor/widgets/
+-rw-rw-rw-   0        0        0        0 2020-03-06 09:15:20.000000 cryspy_editor-1.7.0/cryspy_editor/widgets/__init__.py
+-rw-rw-rw-   0        0        0     5803 2023-03-15 12:58:04.000000 cryspy_editor-1.7.0/cryspy_editor/widgets/cryspy_objects.py
+-rw-rw-rw-   0        0        0     1808 2022-02-08 10:47:56.000000 cryspy_editor-1.7.0/cryspy_editor/widgets/matplotlib.py
+-rw-rw-rw-   0        0        0     1214 2022-02-08 10:47:50.000000 cryspy_editor-1.7.0/cryspy_editor/widgets/w_editcif.py
+-rw-rw-rw-   0        0        0     9442 2023-03-15 12:27:18.000000 cryspy_editor-1.7.0/cryspy_editor/widgets/w_function.py
+-rw-rw-rw-   0        0        0     3109 2022-10-21 13:03:13.000000 cryspy_editor-1.7.0/cryspy_editor/widgets/w_object_panel.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:19:15.125712 cryspy_editor-1.7.0/cryspy_editor.egg-info/
+-rw-rw-rw-   0        0        0      704 2023-07-06 15:19:14.000000 cryspy_editor-1.7.0/cryspy_editor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1327 2023-07-06 15:19:15.000000 cryspy_editor-1.7.0/cryspy_editor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 15:19:14.000000 cryspy_editor-1.7.0/cryspy_editor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-06 15:19:14.000000 cryspy_editor-1.7.0/cryspy_editor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-06 15:19:14.000000 cryspy_editor-1.7.0/cryspy_editor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 15:19:15.197919 cryspy_editor-1.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     2815 2023-07-06 15:18:35.000000 cryspy_editor-1.7.0/setup.py
```

### Comparing `cryspy_editor-1.6.9/LICENSE` & `cryspy_editor-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cryspy_editor-1.6.9/PKG-INFO` & `cryspy_editor-1.7.0/cryspy_editor.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 Metadata-Version: 2.1
-Name: cryspy_editor
-Version: 1.6.9
+Name: cryspy-editor
+Version: 1.7.0
 Summary: Editor of CRYSPY files
 Home-page:  
 Author: Iurii Kibalin
 Author-email: yurikibalin@outlook.com
 License: MIT License
 Keywords: STAR,CrysPy,RhoChi,MEM
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `cryspy_editor-1.6.9/cryspy_editor/__main__.py` & `cryspy_editor-1.7.0/cryspy_editor/__main__.py`

 * *Files identical despite different names*

### Comparing `cryspy_editor-1.6.9/cryspy_editor/ceditor.py` & `cryspy_editor-1.7.0/cryspy_editor/ceditor.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,20 @@
 L_ITEM_CLS = L_ITEM_CLASS
 
 
 from cryspy_editor.widgets.w_function import WFunction
 from cryspy_editor.widgets.w_object_panel import WObjectPanel
 from cryspy_editor.widgets.w_editcif import WEditCif
 from cryspy_editor.widgets.matplotlib import Graph
-from cryspy_editor.widgets.cryspy_objects import cryspy_procedures_to_dictionary, check_function_to_auto_run, check_function_for_procedure
+from cryspy_editor.widgets.cryspy_objects import \
+    cryspy_procedures_to_dictionary, \
+    check_function_to_auto_run, \
+    check_function_for_procedure, \
+    get_plot_functions_for_data_loop_item, \
+    check_function_reserved_for_cryspy_editor
 
 from cryspy_editor.cl_thread import CThread
 
 from cryspy import __version__ as cryspy_version
 from cryspy_editor import __version__ as cryspy_editor_version
 
 
@@ -59,14 +64,16 @@
                 for obj_name in dir(module):
                     if not((obj_name.startswith("__") or (obj_name in ["Callable", ]))):
                         obj = getattr(module, obj_name)
 
                         if hasattr(obj, "__call__"):
                             if check_function_for_procedure(obj): # 
                                 l_func_external.append(obj)
+                            elif check_function_reserved_for_cryspy_editor(obj):
+                                l_func_external.append(obj)
                     else:
                         pass
         except Exception as e:
             print(f"Error at reading external module '{f_name:}'\n", e)
             pass
     return l_func_external
 
@@ -221,14 +228,17 @@
         self.d_setup = {
             "data_file_name": os.path.join(self.dir_prog, ), "data_dir_name": self.dir_prog,
             "file_names_for_external_functions": ""}
         self.f_setup = os.path.join(self.dir_prog, "setup.npy")
         if os.path.isfile(self.f_setup):
             self.d_setup = numpy.load(self.f_setup, allow_pickle='TRUE').item()
 
+        self.functions_plot_data = []
+        self.functions_plot_loop = []
+        self.functions_plot_item = []
         # Thread block        
         self.cthread = CThread(self)
         self.cthread.signal_start.connect(self.run_calculations)
         self.cthread.signal_end.connect(self.end_calculations)
 
         self.setWindowTitle("Cryspy Editor")
         self.init_user_interface()
@@ -390,17 +400,20 @@
         if not("file_names_for_external_functions" in self.d_setup.keys()):
             self.d_setup["file_names_for_external_functions"] = ""
         l_f_name_external_not_checked = self.d_setup["file_names_for_external_functions"].split(";")
         l_f_name_external = [f_name for f_name in l_f_name_external_not_checked if os.path.isfile(f_name)]
         self.d_setup["file_names_for_external_functions"] = ";".join(l_f_name_external)
         numpy.save(self.f_setup, self.d_setup)
         l_func_external = get_external_functions(l_f_name_external)
-        
-        
+
+        self.functions_plot_data, self.functions_plot_loop, self.functions_plot_item = \
+            get_plot_functions_for_data_loop_item(l_func_external)
+
         d_procedures = cryspy_procedures_to_dictionary(l_func_external)
+        
         for key, functions in sorted(d_procedures.items()):
             menu_cryspy = self.menu_bar.addMenu(key)
             menu_cryspy.setToolTipsVisible(True)
             for func in functions:
                 if key.lower().startswith(func.__name__.split("_")[0].lower()):
                     func_name =  " ".join(func.__name__.split("_")[1:]).lower().strip().title()
                 else:
@@ -579,15 +592,47 @@
                 s_text = f"Fig: {ax[0].title.get_text():}"
             else:
                 s_text = f"Fig: {ax.title.get_text():}"
             if len(s_text) > 20:
                 s_text = s_text[:20] + "..."
             w_item_tabs.addTab(widget, s_text)
             # self.insertTab(0, widget, s_text)
+        if len(l_fig_ax) == 0:
+            fig = None
+            if isinstance(item, DataN):
+                for func in self.functions_plot_data:
+                    fig = func(item)
+                    if fig is not None:
+                        break
+
+            if isinstance(item, LoopN):
+                for func in self.functions_plot_loop:
+                    fig = func(item)
+                    if fig is not None:
+                        break
 
+            if isinstance(item, ItemN):
+                for func in self.functions_plot_item:
+                    fig = func(item)
+                    if fig is not None:
+                        break
+            if fig is not None:
+                widget = QtWidgets.QWidget(w_item_tabs)
+                layout = QtWidgets.QVBoxLayout()
+                item_plot = Graph(fig, parent=widget)
+                toolbar = item_plot.get_toolbar(parent=widget)
+                layout.addWidget(toolbar)
+                layout.addWidget(item_plot)
+                widget.setLayout(layout)
+                if len(fig.axes) != 0:
+                    s_text = f"Fig: {fig.axes[0].title.get_text():}"
+                if len(s_text) > 20:
+                    s_text = s_text[:20] + "..."
+                w_item_tabs.addTab(widget, s_text)
+            
         # Report tab
         try:
             report_html = item.report_html()
         except Exception as e:
             report_html = ""
             print("ERROR in object_.report_html")
             print(e)
@@ -897,15 +942,7 @@
                 item_cls = set([type(item) for item in item.items])
                 if type(new_item) not in item_cls:
                     item.CLASSES_OPTIONAL = tuple(list(item.CLASSES_OPTIONAL) +
                                                  [type(new_item)])
                     item.CLASSES = tuple(list(item.CLASSES) + [type(new_item)])
             item.add_items([new_item])
             self.renew_w_object_panel()
-
-
-# if __name__=='__main__':
-#     app = QApplication(sys.argv)
-#     f_icon = os.path.join(os.path.dirname(__file__), "f_icon", "logo.png")
-#     app.setWindowIcon(QtGui.QIcon(f_icon))
-#     ex = CMainWindow()
-#     sys.exit(app.exec_())
```

### Comparing `cryspy_editor-1.6.9/cryspy_editor/cl_thread.py` & `cryspy_editor-1.7.0/cryspy_editor/cl_thread.py`

 * *Files identical despite different names*

### Comparing `cryspy_editor-1.6.9/cryspy_editor/f_icon/calc.gif` & `cryspy_editor-1.7.0/cryspy_editor/f_icon/calc.gif`

 * *Files identical despite different names*

### Comparing `cryspy_editor-1.6.9/cryspy_editor/f_icon/calc_rcif.png` & `cryspy_editor-1.7.0/cryspy_editor/f_icon/calc_rcif.png`

 * *Files identical despite different names*

### Comparing `cryspy_editor-1.6.9/cryspy_editor/f_icon/flip.png` & `cryspy_editor-1.7.0/cryspy_editor/f_icon/flip.png`

 * *Files identical despite different names*

### Comparing `cryspy_editor-1.6.9/cryspy_editor/f_icon/graph.png` & `cryspy_editor-1.7.0/cryspy_editor/f_icon/graph.png`

 * *Files identical despite different names*

### Comparing `cryspy_editor-1.6.9/cryspy_editor/f_icon/icon.png` & `cryspy_editor-1.7.0/cryspy_editor/f_icon/icon.png`

 * *Files identical despite different names*

### Comparing `cryspy_editor-1.6.9/cryspy_editor/f_icon/logo.png` & `cryspy_editor-1.7.0/cryspy_editor/f_icon/logo.png`

 * *Files identical despite different names*

### Comparing `cryspy_editor-1.6.9/cryspy_editor/f_icon/new.png` & `cryspy_editor-1.7.0/cryspy_editor/f_icon/new.png`

 * *Files identical despite different names*

### Comparing `cryspy_editor-1.6.9/cryspy_editor/f_icon/open.png` & `cryspy_editor-1.7.0/cryspy_editor/f_icon/open.png`

 * *Files identical despite different names*

### Comparing `cryspy_editor-1.6.9/cryspy_editor/f_icon/open_folder.png` & `cryspy_editor-1.7.0/cryspy_editor/f_icon/open_folder.png`

 * *Files identical despite different names*

### Comparing `cryspy_editor-1.6.9/cryspy_editor/f_icon/pm.gif` & `cryspy_editor-1.7.0/cryspy_editor/f_icon/pm.gif`

 * *Files identical despite different names*

### Comparing `cryspy_editor-1.6.9/cryspy_editor/f_icon/refresh.png` & `cryspy_editor-1.7.0/cryspy_editor/f_icon/refresh.png`

 * *Files identical despite different names*

### Comparing `cryspy_editor-1.6.9/cryspy_editor/f_icon/save.png` & `cryspy_editor-1.7.0/cryspy_editor/f_icon/save.png`

 * *Files identical despite different names*

### Comparing `cryspy_editor-1.6.9/cryspy_editor/f_icon/save_.png` & `cryspy_editor-1.7.0/cryspy_editor/f_icon/save_.png`

 * *Files identical despite different names*

### Comparing `cryspy_editor-1.6.9/cryspy_editor/f_icon/save_as.png` & `cryspy_editor-1.7.0/cryspy_editor/f_icon/save_as.png`

 * *Files identical despite different names*

### Comparing `cryspy_editor-1.6.9/cryspy_editor/f_icon/save_as_.png` & `cryspy_editor-1.7.0/cryspy_editor/f_icon/save_as_.png`

 * *Files identical despite different names*

### Comparing `cryspy_editor-1.6.9/cryspy_editor/f_icon/to_cryspy.png` & `cryspy_editor-1.7.0/cryspy_editor/f_icon/to_cryspy.png`

 * *Files identical despite different names*

### Comparing `cryspy_editor-1.6.9/cryspy_editor/f_icon/to_cryspy_.png` & `cryspy_editor-1.7.0/cryspy_editor/f_icon/to_cryspy_.png`

 * *Files identical despite different names*

### Comparing `cryspy_editor-1.6.9/cryspy_editor/f_icon/to_magref.png` & `cryspy_editor-1.7.0/cryspy_editor/f_icon/to_magref.png`

 * *Files identical despite different names*

### Comparing `cryspy_editor-1.6.9/cryspy_editor/f_icon/to_mem.png` & `cryspy_editor-1.7.0/cryspy_editor/f_icon/to_mem.png`

 * *Files identical despite different names*

### Comparing `cryspy_editor-1.6.9/cryspy_editor/f_icon/to_rhochi.png` & `cryspy_editor-1.7.0/cryspy_editor/f_icon/to_rhochi.png`

 * *Files identical despite different names*

### Comparing `cryspy_editor-1.6.9/cryspy_editor/f_icon/to_rhochi_.png` & `cryspy_editor-1.7.0/cryspy_editor/f_icon/to_rhochi_.png`

 * *Files identical despite different names*

### Comparing `cryspy_editor-1.6.9/cryspy_editor/f_icon/to_star.png` & `cryspy_editor-1.7.0/cryspy_editor/f_icon/to_star.png`

 * *Files identical despite different names*

### Comparing `cryspy_editor-1.6.9/cryspy_editor/f_icon/to_star_.png` & `cryspy_editor-1.7.0/cryspy_editor/f_icon/to_star_.png`

 * *Files identical despite different names*

### Comparing `cryspy_editor-1.6.9/cryspy_editor/widgets/matplotlib.py` & `cryspy_editor-1.7.0/cryspy_editor/widgets/matplotlib.py`

 * *Files identical despite different names*

### Comparing `cryspy_editor-1.6.9/cryspy_editor/widgets/w_editcif.py` & `cryspy_editor-1.7.0/cryspy_editor/widgets/w_editcif.py`

 * *Files identical despite different names*

### Comparing `cryspy_editor-1.6.9/cryspy_editor/widgets/w_function.py` & `cryspy_editor-1.7.0/cryspy_editor/widgets/w_function.py`

 * *Files 25% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         n_var_names = len(l_var_name)
 
         layout = self.layout_func
         del_layout(layout)
 
         self.l_w_arg = []
         self.globaln = None
-        
+
         d_annotations = func.__annotations__
         var_annotations = d_annotations.keys()
 
         flag_first_globaln = False
         flag_in_globaln = globaln is not None
         for _i_var, _var_name in enumerate(l_var_name):
             i_default = _i_var-(n_var_names-n_defaults)
@@ -124,74 +124,18 @@
                     if i_default >= 0:
                         widget.attached_object = l_defaults[i_default]
                         widget.setStyleSheet("")
                 if flag_label:
                     layout.addWidget(QtWidgets.QLabel(_var_name))
                 layout.addWidget(widget)
                 self.l_w_arg.append(widget)
-                
-        
-        # for _i_var, _var_name in enumerate(l_var_name):
-        #     i_default = _i_var-(n_var_names-n_defaults)
-        #     if i_default >= 0:
-        #         s_def = str(l_defaults[i_default]) + " (default)"
-        #     else:
-        #         s_def = "<drop object>"
-        #     if (_var_name != "self"):
-        #         # if _var_name == "d_info":
-        #         #     pass
-        #         # elif ii_h == 0:
-        #         #     pass
-        #         if _var_name != "d_info" :
-        #             flag_special = False
-        #             flag_label = True
-        #             if _var_name in var_annotations:
-        #                 var_type = d_annotations[_var_name]
-        #                 if i_default >= 0:
-        #                     if var_type is bool:
-        #                         widget = QtWidgets.QCheckBox(_var_name)
-        #                         widget.setCheckState(2*l_defaults[i_default])
-        #                         widget.attached_object = l_defaults[i_default]
-        #                         widget.clicked.connect(
-        #                             lambda: setattr(widget, "attached_object",
-        #                                             widget.checkState()//2))
-        #                         flag_special = True
-        #                         flag_label = False
-        #                     # elif var_type is float:
-        #                     #     widget = QtWidgets.QDoubleSpinBox()
-        #                     #     widget.setValue(l_defaults[i_default])
-        #                     #     widget.attached_object = l_defaults[i_default]
-        #                     #     widget.valueChanged.connect(
-        #                     #         lambda: setattr(widget, "attached_object",
-        #                     #                         widget.value()))
-        #                     #     flag_special = True
-        #                     # elif var_type is int:
-        #                     #     widget = QtWidgets.QSpinBox()
-        #                     #     widget.setValue(l_defaults[i_default])
-        #                     #     widget.attached_object = l_defaults[i_default]
-        #                     #     widget.valueChanged.connect(
-        #                     #         lambda: setattr(widget, "attached_object",
-        #                     #                         widget.value()))
-        #                     #     flag_special = True
-
-        #             if not(flag_special):
-        #                 widget = DropLabel(f"{s_def:}")
-        #                 widget.setStyleSheet(
-        #                     "background:lightyellow; border: 2px solid red;")
-        #                 if i_default >= 0:
-        #                     widget.attached_object = l_defaults[i_default]
-        #                     widget.setStyleSheet("")
-        #             if flag_label:
-        #                 layout.addWidget(QtWidgets.QLabel(_var_name))
-        #             layout.addWidget(widget)
-        #             self.l_w_arg.append(widget)
-        #         ii_h += 1
+
         self.function_attached = func
         self.thread_attached = thread
-        
+
         if  len(self.l_w_arg) == 0:
             self.run_function()
             self.w_cb_hide.setCheckState(2)
 
     def is_defined(self):
         """Is defined."""
         return all([w_arg.attached_object is not None
@@ -199,19 +143,19 @@
 
     def run_function(self) -> NoReturn:
         """Run function."""
         func = self.function_attached
         thread = self.thread_attached
         if func is None:
             return
-        
+
         l_w_arg = self.l_w_arg
         self.push_button.setEnabled(False)
         l_x = [_.attached_object for _ in l_w_arg]
-        
+
         if self.globaln is not None:
             t_x = tuple([self.globaln, ] + l_x)
         else:
             t_x = tuple(l_x)
         if thread is None:
             try:
                 func(*t_x)
@@ -263,15 +207,15 @@
             s_cont = type(item).__name__
         else:
             event.ignore()
             return
 
         self.setText(s_cont)
         self.setStyleSheet("")
-        
+
         event.acceptProposedAction()
 
     def convert_to_object(self):
         """Convert to object."""
         text = self.text()
         obj = None
         flag = False
@@ -299,15 +243,15 @@
                 try:
                     obj = float(text)
                     flag = True
                 except Exception:
                     pass
         if not flag:
             obj = str(text)
-        
+
         self.attached_object = obj
         self.setAlignment(QtCore.Qt.AlignRight)
         self.setStyleSheet("")
 
 
 def w_for_function(obj: Callable, layout_11: QtWidgets.QBoxLayout,
                     layout_12: QtWidgets.QBoxLayout,
```

### Comparing `cryspy_editor-1.6.9/cryspy_editor/widgets/w_object_panel.py` & `cryspy_editor-1.7.0/cryspy_editor/widgets/w_object_panel.py`

 * *Files identical despite different names*

### Comparing `cryspy_editor-1.6.9/cryspy_editor.egg-info/PKG-INFO` & `cryspy_editor-1.7.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 Metadata-Version: 2.1
-Name: cryspy-editor
-Version: 1.6.9
+Name: cryspy_editor
+Version: 1.7.0
 Summary: Editor of CRYSPY files
 Home-page:  
 Author: Iurii Kibalin
 Author-email: yurikibalin@outlook.com
 License: MIT License
 Keywords: STAR,CrysPy,RhoChi,MEM
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `cryspy_editor-1.6.9/cryspy_editor.egg-info/SOURCES.txt` & `cryspy_editor-1.7.0/cryspy_editor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cryspy_editor-1.6.9/setup.py` & `cryspy_editor-1.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 
-# Copyright (c) 2018-2019 Iurii Kibalin   
+# Copyright (c) 2018-2023 Iurii Kibalin   
 # https://github.com/ikibalin/cryspy  
 # All rights reserved.
 # 
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are
 # met:
 # 
@@ -38,15 +38,15 @@
 #f_name = os.path.join(os.path.dirname(__file__), "readme.rst")
 #with open(f_name, 'r') as f:
 #    long_description = f.read()
 long_description = ""
 
 setup(
     name='cryspy_editor',
-    version='1.6.9',
+    version='1.7.0',
     description='Editor of CRYSPY files',
     long_description = long_description,
     author='Iurii Kibalin',
     author_email='yurikibalin@outlook.com',
     url = ' ',
     license          = 'MIT License',
     keywords         = 'STAR, CrysPy, RhoChi, MEM',
```

