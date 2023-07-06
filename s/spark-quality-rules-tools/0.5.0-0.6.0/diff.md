# Comparing `tmp/spark_quality_rules_tools-0.5.0.tar.gz` & `tmp/spark_quality_rules_tools-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_quality_rules_tools-0.5.0.tar", last modified: Mon Jul  3 14:59:55 2023, max compression
+gzip compressed data, was "spark_quality_rules_tools-0.6.0.tar", last modified: Thu Jul  6 08:07:32 2023, max compression
```

## Comparing `spark_quality_rules_tools-0.5.0.tar` & `spark_quality_rules_tools-0.6.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 14:59:55.784552 spark_quality_rules_tools-0.5.0/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.5.0/LICENSE
--rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4041 2023-07-03 14:59:55.785553 spark_quality_rules_tools-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.5.0/README.md
--rw-rw-rw-   0        0        0      685 2023-07-01 22:58:24.000000 spark_quality_rules_tools-0.5.0/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-07-03 14:59:55.786553 spark_quality_rules_tools-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1210 2023-07-03 14:59:45.000000 spark_quality_rules_tools-0.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 14:59:55.732541 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/
--rw-rw-rw-   0        0        0     2550 2023-07-02 03:08:37.000000 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 14:59:55.756546 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    49664 2023-07-03 14:59:45.000000 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-07-03 14:59:55.775551 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/utils/color.py
--rw-rw-rw-   0        0        0     2138 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/utils/resolve.py
-drwxrwxrwx   0        0        0        0 2023-07-03 14:59:55.784552 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/utils/resource/
--rw-rw-rw-   0        0        0      532 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/utils/resource/resolve_edge.conf
--rw-rw-rw-   0        0        0      742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf
--rw-rw-rw-   0        0        0    25817 2023-07-02 01:22:13.000000 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/utils/resource/rules.json
--rw-rw-rw-   0        0        0     3742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/utils/rules.py
-drwxrwxrwx   0        0        0        0 2023-07-03 14:59:55.755546 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools.egg-info/
--rw-rw-rw-   0        0        0     4041 2023-07-03 14:59:55.000000 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      784 2023-07-03 14:59:55.000000 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 14:59:55.000000 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      205 2023-07-03 14:59:55.000000 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-07-03 14:59:55.000000 spark_quality_rules_tools-0.5.0/spark_quality_rules_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 08:07:32.135801 spark_quality_rules_tools-0.6.0/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4041 2023-07-06 08:07:32.135801 spark_quality_rules_tools-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.6.0/README.md
+-rw-rw-rw-   0        0        0      685 2023-07-06 02:24:33.000000 spark_quality_rules_tools-0.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-07-06 08:07:32.136802 spark_quality_rules_tools-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1210 2023-07-06 08:07:00.000000 spark_quality_rules_tools-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 08:07:32.087791 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/
+-rw-rw-rw-   0        0        0     2790 2023-07-06 07:26:52.000000 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 08:07:32.109798 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    56427 2023-07-06 07:47:24.000000 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-07-06 08:07:32.125799 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/utils/color.py
+-rw-rw-rw-   0        0        0     2138 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/utils/resolve.py
+drwxrwxrwx   0        0        0        0 2023-07-06 08:07:32.134803 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/utils/resource/
+-rw-rw-rw-   0        0        0      532 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/utils/resource/resolve_edge.conf
+-rw-rw-rw-   0        0        0      742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf
+-rw-rw-rw-   0        0        0    25809 2023-07-06 02:34:48.000000 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/utils/resource/rules.json
+-rw-rw-rw-   0        0        0     3920 2023-07-06 05:59:35.000000 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/utils/rules.py
+drwxrwxrwx   0        0        0        0 2023-07-06 08:07:32.108797 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools.egg-info/
+-rw-rw-rw-   0        0        0     4041 2023-07-06 08:07:32.000000 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      784 2023-07-06 08:07:32.000000 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 08:07:32.000000 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      205 2023-07-06 08:07:32.000000 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-07-06 08:07:32.000000 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools.egg-info/top_level.txt
```

### Comparing `spark_quality_rules_tools-0.5.0/LICENSE` & `spark_quality_rules_tools-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.5.0/PKG-INFO` & `spark_quality_rules_tools-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_quality_rules_tools
-Version: 0.5.0
+Version: 0.6.0
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.5.0/README.md` & `spark_quality_rules_tools-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.5.0/pyproject.toml` & `spark_quality_rules_tools-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 findspark = "2.0.1"
 pyspark = "3.1.1"
 pandas = "2.0.1"
 numpy = "1.24.3"
 pyarrow = "12.0.0"
 setuptools = "58.2.0"
 wheel = "0.40.0"
-spark-dataframe-tools = "^0.2.0"
 color-tools = "^0.0.2"
 pyhocon = "^0.3.60"
 tqdm = "^4.65.0"
 prettytable = "^3.8.0"
+spark-dataframe-tools = "^0.4.0"
 
 
 [tool.poetry.group.dev.dependencies]
 jupyterlab = "^4.0.0"
 twine = "^4.0.2"
 
 [build-system]
```

### Comparing `spark_quality_rules_tools-0.5.0/setup.py` & `spark_quality_rules_tools-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_quality_rules_tools',
     packages=find_packages(),
-    version='0.5.0',
+    version='0.6.0',
     description='spark_quality_rules_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_quality_rules_tools/',
     download_url='https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip',
```

### Comparing `spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/__init__.py` & `spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 from spark_quality_rules_tools.functions.generator import dq_creating_directory_sandbox
 from spark_quality_rules_tools.functions.generator import dq_download_jar
 from spark_quality_rules_tools.functions.generator import dq_extract_parameters_artifactory
 from spark_quality_rules_tools.functions.generator import dq_extract_parameters_file
 from spark_quality_rules_tools.functions.generator import dq_path_workspace
+from spark_quality_rules_tools.functions.generator import dq_searching_rules
 from spark_quality_rules_tools.functions.generator import dq_run_sandbox_artifactory
 from spark_quality_rules_tools.functions.generator import dq_run_sandbox_file
 from spark_quality_rules_tools.functions.generator import dq_run_sandbox_file_with_rules
 from spark_quality_rules_tools.functions.generator import dq_spark_session
 from spark_quality_rules_tools.functions.generator import dq_validate_artifactory
 from spark_quality_rules_tools.functions.generator import dq_validate_artifactory_with_rules
 from spark_quality_rules_tools.functions.generator import dq_validate_conf_artifactory
 from spark_quality_rules_tools.functions.generator import dq_validate_conf_file
 from spark_quality_rules_tools.functions.generator import dq_validate_file
 from spark_quality_rules_tools.functions.generator import dq_validate_file_with_rules
 from spark_quality_rules_tools.functions.generator import dq_get_rules_list
 from spark_quality_rules_tools.functions.generator import dq_generated_rules
+from spark_quality_rules_tools.functions.generator import dq_run_sandbox_archive_path_rules
 from spark_quality_rules_tools.utils import BASE_DIR
 from spark_quality_rules_tools.utils.color import get_color
 from spark_quality_rules_tools.utils.color import get_color_b
 from spark_quality_rules_tools.utils.resolve import get_replace_resolve_parameter
 from spark_quality_rules_tools.utils.rules import get_validate_rules
 
 generator_all = [
     "dq_creating_directory",
     "dq_spark_session",
     "dq_path_workspace",
     "dq_download_jar",
     "dq_get_rules_list",
-    "dq_generated_rules"
+    "dq_generated_rules",
+    "dq_searching_rules"
 ]
 generator_artifactory = [
     "dq_validate_conf_artifactory",
     "dq_extract_parameters_artifactory",
     "dq_run_sandbox_artifactory",
     "dq_validate_rules_artifactory",
     "dq_validate_artifactory",
@@ -40,15 +43,16 @@
 
 generator_file = [
     "dq_validate_conf_file",
     "dq_extract_parameters_file",
     "dq_run_sandbox_file",
     "dq_run_sandbox_file_with_rules"
     "dq_validate_file",
-    "dq_validate_file_with_rules"
+    "dq_validate_file_with_rules",
+    "dq_run_sandbox_archive_path_rules"
 ]
 
 utils_all = [
     "BASE_DIR",
     "get_color",
     "get_color_b",
     "get_replace_resolve_parameter"
```

### Comparing `spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/functions/generator.py` & `spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/functions/generator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,59 @@
+def dq_searching_rules(category_rule=None, table_name=None, rule_id=None, static_id=None, sequence="001"):
+    from spark_quality_rules_tools.utils import BASE_DIR
+    import os
+    import json
+    import ast
+    import sys
+
+    is_windows = sys.platform.startswith('win')
+    json_resource_rules = os.path.join(BASE_DIR, "utils", "resource", "rules.json")
+
+    if is_windows:
+        json_resource_rules = json_resource_rules.replace("\\", "/")
+
+    with open(json_resource_rules) as f:
+        default_rules = json.load(f)
+    rules_config = default_rules.get("rules_config", None)
+    hamu_dict = dict()
+    id_key_dict = dict()
+    rs_dict = dict()
+    for k, v in rules_config.items():
+        for key_name, value_name in v.items():
+            rules_version = value_name[0].get("rules_version")
+            rules_class = str(value_name[0].get("rules_class"))
+            rules_columns = value_name[0].get("rules_columns")
+            if rules_version == rule_id:
+                for rule_name, rule_dtype in rules_columns[0].items():
+                    if rule_dtype[1] == "True":
+                        id_key_dict[rule_name] = "Mandatory"
+                    if rule_dtype[0] == "Boolean" and rule_dtype[2] == "True":
+                        rules_value = True
+                    elif rule_dtype[0] == "Boolean" and rule_dtype[2] == "False":
+                        rules_value = False
+                    elif rule_dtype[0] == "Double" and rule_dtype[2] == "100":
+                        rules_value = ast.literal_eval(rule_dtype[2])
+                    elif rule_dtype[0] == "String" and rule_dtype[2] in ("None", ""):
+                        rules_value = ""
+                    elif rule_dtype[0] == "Array[String]" and rule_dtype[2] in ("None", ""):
+                        rules_value = ["default"]
+                    elif rule_dtype[0] == "Dict" and rule_dtype[2] in ("None", ""):
+                        rules_value = dict(type="", paths="")
+                    else:
+                        rules_value = rule_dtype[2]
+                    rs_dict[rule_name] = rules_value
+                if static_id:
+                    rs_dict["id"] = static_id
+                else:
+                    rs_dict["id"] = f"PE_{category_rule}_{table_name}_{rule_id}_{sequence}"
+                hamu_dict["class"] = rules_class
+                hamu_dict["config"] = rs_dict
+    return hamu_dict, id_key_dict
+
+
 def dq_creating_directory_hdfs(spark=None, path=None):
     from spark_quality_rules_tools import get_color, get_color_b
 
     sc = spark.sparkContext
     fs = spark._jvm.org.apache.hadoop.fs.FileSystem.get(spark._jsc.hadoopConfiguration())
     if path in ("", None):
         raise Exception(f'required variable path')
@@ -704,22 +756,19 @@
     uuaa_name = str(uuaa).upper()
 
     now = datetime.now()
     current_datetime = now.strftime("%Y-%m-%d %H:%M:%S")
     current_datetime_str = now.strftime("%Y%m%d%H%M")
 
     id_split = str(rules_id).split("_")
-    rule_country = str(id_split[0])
-    rule_type = str(id_split[1])
-    rule_id = str(id_split[-2])
-    rule_correlative = str(id_split[-1])
+    table_name = "_".join(id_split[2:-2])
 
     dir_confs_filename = os.path.join(dir_confs_name, uuaa_name, f"{url_conf_name}.txt")
     dir_confs_filename_parameters = os.path.join(dir_confs_name, uuaa_name, f"PARAMS-{url_conf_name}.json")
-    dir_hocons_filename = os.path.join(dir_hocons_name, uuaa_name, f"{url_conf_name}_{rule_country}_{rule_type}_{rule_id}_{rule_correlative}.conf")
+    dir_hocons_filename = os.path.join(dir_hocons_name, uuaa_name, f"{table_name}_ruleid_generated.conf")
 
     if is_windows:
         dir_confs_filename = dir_confs_filename.replace("\\", "/")
         dir_confs_filename_parameters = dir_confs_filename_parameters.replace("\\", "/")
         dir_hocons_filename = dir_hocons_filename.replace("\\", "/")
     os.makedirs(os.path.dirname(dir_hocons_filename), exist_ok=True)
 
@@ -769,19 +818,18 @@
         if 'dataFrameInfo' in info.keys():
             dataframeinfo = info["dataFrameInfo"]
         if 'input' in info.keys():
             input = info["input"]
         if 'rules' in info.keys():
             rules = info["rules"]
             for rule in rules:
-                rule_id = rule.get("config").get("id", None)
-                if rule_id:
+                key_id_rule = rule.get("config").get("id", None)
+                if str(key_id_rule) == str(rules_id):
                     rule_list.append(rule)
         hamu_dict = dict(hammurabi=dict(dataFrameInfo=dataframeinfo, input=input, rules=rule_list))
-
     json_file2 = json.dumps(hamu_dict, indent=4)
     conf2 = ConfigFactory.parse_string(json_file2)
     hocons_file2 = HOCONConverter.convert(conf2, "hocon")
     with open(dir_hocons_filename, "w") as f:
         f.write(hocons_file2)
 
     spark._jvm.org.apache.hadoop.fs.FileSystem.get(spark._jsc.hadoopConfiguration())
@@ -964,66 +1012,31 @@
 
 def dq_generated_rules(rule_id=None,
                        table_name=None,
                        category_rule="MVP"):
     import os
     import sys
     import json
-    import ast
     from pyhocon import ConfigFactory
     from pyhocon.converter import HOCONConverter
     from spark_quality_rules_tools.utils.color import get_color_b, get_color
-    from spark_quality_rules_tools.utils import BASE_DIR
     from prettytable import PrettyTable
 
     is_windows = sys.platform.startswith('win')
     dir_hocons_name = os.getenv('pj_dq_dir_hocons_name')
     uuaa_name = str(table_name.split("_")[1]).upper()
-    json_resource_rules = os.path.join(BASE_DIR, "utils", "resource", "rules.json")
     dir_hocons_filename = os.path.join(dir_hocons_name, uuaa_name, f"{table_name}_{rule_id}_generated.conf")
 
     if is_windows:
-        json_resource_rules = json_resource_rules.replace("\\", "/")
         dir_hocons_filename = dir_hocons_filename.replace("\\", "/")
     os.makedirs(os.path.dirname(dir_hocons_filename), exist_ok=True)
 
-    with open(json_resource_rules) as f:
-        default_rules = json.load(f)
-    rules_config = default_rules.get("rules_config", None)
-    hamu_dict = dict()
     rs_list = list()
-    rs_dict = dict()
-    rs_key = dict()
-    for k, v in rules_config.items():
-        for key_name, value_name in v.items():
-            rules_version = value_name[0].get("rules_version")
-            rules_class = str(value_name[0].get("rules_class"))
-            rules_columns = value_name[0].get("rules_columns")
-            if rules_version == rule_id:
-                for rule_name, rule_value in rules_columns[0].items():
-                    if rule_value[1] == "True":
-                        rs_key[rule_name] = "Mandatory"
-                    if rule_value[0] == "Boolean" and rule_value[2] == "True":
-                        rule_valuex = True
-                    elif rule_value[0] == "Boolean" and rule_value[2] == "False":
-                        rule_valuex = False
-                    elif rule_value[0] == "Double" and rule_value[2] == "100":
-                        rule_valuex = ast.literal_eval(rule_value[2])
-                    elif rule_value[0] == "String" and rule_value[2] in ("None", ""):
-                        rule_valuex = ""
-                    elif rule_value[0] == "Array[String]" and rule_value[2] in ("None", ""):
-                        rule_valuex = ["default"]
-                    elif rule_value[0] == "Dict" and rule_value[2] in ("None", ""):
-                        rule_valuex = dict(type="", paths="")
-                    else:
-                        rule_valuex = rule_value[2]
-                    rs_dict[rule_name] = rule_valuex
-                rs_dict["id"] = f"PE_{category_rule}_{table_name}_{rule_id}_001"
-                hamu_dict["class"] = rules_class
-                hamu_dict["config"] = rs_dict
+    hamu_dict, id_key_dict = dq_searching_rules(category_rule=category_rule, table_name=table_name,
+                                                rule_id=rule_id, static_id=None, sequence="001")
     rs_list.append(hamu_dict)
     json_file2 = json.dumps(rs_list, indent=4)
     conf2 = ConfigFactory.parse_string(json_file2)
     hocons_file2 = HOCONConverter.convert(conf2, "hocon")
     with open(dir_hocons_filename, "w") as f:
         f.write(hocons_file2)
 
@@ -1031,10 +1044,117 @@
     with open(dir_hocons_filename) as f:
         res = f.read()
     print(f"{get_color_b(f'{res}')}")
 
     print(f"{get_color(f'========MANDATORY============')} ")
     t = PrettyTable()
     t.field_names = [get_color_b("DQ NAME"), get_color_b("TYPE")]
-    for key_name, value_name in rs_key.items():
+    for key_name, value_name in id_key_dict.items():
         t.add_row([key_name, value_name])
     print(t)
+
+
+def dq_run_sandbox_archive_path_rules(spark=None, path=None, category_rule="MVP"):
+    import pandas as pd
+    from pyspark.sql.types import StructType, StructField, StringType
+    from pyspark.sql.window import Window
+    from pyspark.sql import functions as func
+    import os
+    import sys
+    from spark_quality_rules_tools.utils.color import get_color_b, get_color
+    import json
+    from pyhocon import ConfigFactory
+    from pyhocon.converter import HOCONConverter
+
+    global dir_hocons_filename
+    is_windows = sys.platform.startswith('win')
+    dir_hocons_name = os.getenv('pj_dq_dir_hocons_name')
+
+    df = pd.read_csv(path, sep=",").fillna("")
+    schema = StructType([
+        StructField("TABLE", StringType(), True),
+        StructField("FIELD", StringType(), True),
+        StructField("SUBPARTITION_ONE", StringType(), True),
+        StructField("SUBPARTITION_TWO", StringType(), True),
+        StructField("VERSION", StringType(), True),
+        StructField("PERIODICITY", StringType(), True),
+        StructField("STATIC_ID", StringType(), True)
+    ])
+    df = spark.createDataFrame(df, schema=schema)
+    df = df.orderBy("TABLE", "FIELD", "SUBPARTITION_ONE", "SUBPARTITION_TWO", "VERSION")
+    df = df.withColumn('ORDEN', func.row_number().over(Window.partitionBy(func.lit('1')).orderBy(func.lit('1'))))
+    windowSpec = Window.partitionBy("TABLE", "FIELD", "SUBPARTITION_ONE", "SUBPARTITION_TWO", "VERSION").orderBy("ORDEN")
+    df = df.withColumn("SEQUENCE", func.row_number().over(windowSpec)).orderBy("ORDEN")
+    table_dict = dict()
+    table_list = list()
+
+    for row in df.collect():
+        table_name = str(row["TABLE"]).strip().lower()
+        field_name = str(row["FIELD"]).strip().lower()
+        subpartition_one = row["SUBPARTITION_ONE"]
+        if subpartition_one not in (None, "", "NaN"):
+            subpartition_one = str(subpartition_one.split("=")[0])
+        subpartition_two = row["SUBPARTITION_TWO"]
+        if subpartition_two not in (None, "", "NaN"):
+            subpartition_two = str(subpartition_two.split("=")[0])
+        rule_id = row["VERSION"]
+        periodicity = str(row["PERIODICITY"]).strip().capitalize()
+        sequence = str(row["SEQUENCE"]).zfill(3)
+        static_id = None if row["STATIC_ID"] in ("", None, "NaN", "Null") else row["STATIC_ID"]
+        uuaa_name = str(table_name.split("_")[1]).lower()
+        uuaa_tag = "".join(table_name.split("_")[2:])
+
+        hamu_dict, id_key_dict = dq_searching_rules(category_rule=category_rule, table_name=table_name,
+                                                    rule_id=rule_id, static_id=static_id, sequence=sequence)
+
+        if 'columns' in hamu_dict["config"].keys():
+            hamu_dict["config"]["columns"] = [field_name]
+        if 'column' in hamu_dict["config"].keys():
+            hamu_dict["config"]["columns"] = field_name
+
+        if table_name not in table_dict.keys():
+            table_dict[table_name] = dict(hammurabi=dict())
+            table_dict[table_name]["hammurabi"]["dataFrameInfo"] = dict()
+            table_dict[table_name]["hammurabi"]["dataFrameInfo"]["cutoffDate"] = "${?CUTOFF_DATE}"
+            table_dict[table_name]["hammurabi"]["dataFrameInfo"]["frequencyRuleExecution"] = periodicity
+            table_dict[table_name]["hammurabi"]["dataFrameInfo"]["physicalTargetName"] = f"/data/master/{uuaa_name}/data/{table_name}"
+            table_dict[table_name]["hammurabi"]["dataFrameInfo"]["subset"] = "cutoff_date='${?CUTOFF_DATE}'"
+            if subpartition_one:
+                table_dict[table_name]["hammurabi"]["dataFrameInfo"]["subset"] = "cutoff_date='${?CUTOFF_DATE}' and " \
+                                                                                 f"{subpartition_one}=" + "'${?SUBPATITION_ONE}'"
+            if subpartition_two:
+                table_dict[table_name]["hammurabi"]["dataFrameInfo"]["subset"] = "cutoff_date='${?CUTOFF_DATE}' and " \
+                                                                                 f"{subpartition_one}=" + "'${?SUBPATITION_ONE}' and " \
+                                                                                                          f"{subpartition_two}=" + "'${?SUBPATITION_TWO}'"
+            table_dict[table_name]["hammurabi"]["dataFrameInfo"]["uuaa"] = uuaa_name
+            table_dict[table_name]["hammurabi"]["Input"] = dict()
+            table_dict[table_name]["hammurabi"]["Input"]["options"] = dict(includeMetadataAndDeleted=True, overrideSchema=True)
+            table_dict[table_name]["hammurabi"]["Input"]["paths"] = [f"/data/master/{uuaa_name}/data/{table_name}"]
+            table_dict[table_name]["hammurabi"]["Input"]["type"] = "parquet"
+            table_dict[table_name]["hammurabi"]["Input"]["schema"] = dict(path="${ARTIFACTORY_UNIQUE_CACHE}/artifactory/${SCHEMAS_REPOSITORY}"
+                                                                               f"/schemas/pe/{uuaa_name}"
+                                                                               f"/master/{uuaa_tag}/latest/{uuaa_tag}.output.schema",
+                                                                          type="parquet")
+
+            table_dict[table_name]["hammurabi"]["rules"] = list()
+        table_dict[table_name]["hammurabi"]["rules"].append(hamu_dict)
+        table_list.append(table_name)
+
+    table_unique_list = list(set(table_list))
+
+    for table in table_unique_list:
+        uuaa_name = str(table.split("_")[1]).upper()
+        table_name = str(table).lower()
+        dir_hocons_filename = os.path.join(dir_hocons_name, uuaa_name, f"{table_name}_archive_generated.conf")
+        if is_windows:
+            dir_hocons_filename = dir_hocons_filename.replace("\\", "/")
+        os.makedirs(os.path.dirname(dir_hocons_filename), exist_ok=True)
+
+        txt_string = table_dict[table]
+        json_file2 = json.dumps(txt_string, indent=4)
+        conf2 = ConfigFactory.parse_string(json_file2)
+        hocons_file2 = HOCONConverter.convert(conf2, "hocon")
+
+        with open(dir_hocons_filename, "w") as f:
+            f.write(hocons_file2)
+
+        print(f"{get_color('HOCON CREATE:')} {get_color_b(dir_hocons_filename)}")
```

### Comparing `spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/utils/resolve.py` & `spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/utils/resolve.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/utils/resource/resolve_edge.conf` & `spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/utils/resource/resolve_edge.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf` & `spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/utils/resource/rules.json` & `spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/utils/resource/rules.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998263888888889%*

 * *Differences: {"'rules_config'": "{'integrity': {'SameValueComparisonRule': {0: {'rules_name': 'Comparison of "*

 * *                   "data values that must fulfill a condition'}}}}"}*

```diff
@@ -1200,15 +1200,15 @@
                             "withRefusals": [
                                 "Boolean",
                                 "False",
                                 "False"
                             ]
                         }
                     ],
-                    "rules_name": "Comparison of related data values that must fulfill a condition",
+                    "rules_name": "Comparison of data values that must fulfill a condition",
                     "rules_version": "5.3"
                 }
             ],
             "ValueComparisonRule": [
                 {
                     "apply_rules_common": true,
                     "rules_class": "com.datio.hammurabi.rules.integrity.ValueComparisonRule",
```

### Comparing `spark_quality_rules_tools-0.5.0/spark_quality_rules_tools/utils/rules.py` & `spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/utils/rules.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     file_conf = ConfigFactory.parse_file(file_conf)
     file_conf = HOCONConverter.to_json(file_conf)
     file_conf = json.loads(file_conf)
     haas_rules = file_conf["hammurabi"]["rules"]
 
     rules_default_properties = default_rules["rules_common_properties"][0]
 
+    key_id_list = list()
     for haas_rule in haas_rules:
         haas_class = str(haas_rule["class"])
         haas_columns = haas_rule["config"]
         haas_rules_type = str(haas_class).split(".")[4]
         haas_rules_class = str(haas_class).split(".")[5]
 
         rules_version = default_rules["rules_config"][haas_rules_type][haas_rules_class][0]["rules_version"]
@@ -42,14 +43,15 @@
 
         t = PrettyTable()
         print(f"type   => {get_color_g(haas_rules_type)}")
         print(f"class  => {get_color_g(haas_rules_class)}")
         print(f"version=> {get_color_g(rules_version)}")
         if "id" in haas_columns.keys():
             print(f"id=> {get_color_g(haas_columns.get('id'))}")
+            key_id_list.append(haas_columns.get('id'))
         else:
             print(f"id=> {get_color_g('No existe parametro ID')}")
 
         t.field_names = [f"Variable", "Value", "Dtype Actual", "Dtype Esperado", "Es Obligatorio"]
         for col in rules_columns_required:
             if "id" in haas_columns.keys():
                 print(f"id=> {get_color_g(rules_columns_all[col])}")
@@ -78,7 +80,10 @@
                 t.add_row([get_color(col),
                            get_color(value),
                            get_color(str(type(value))),
                            get_color(rules_columns_all[col][0]),
                            get_color(rules_columns_all[col][1])
                            ])
         print(t)
+
+    print(f"Total ID: {len(key_id_list)}")
+    print(f"Unique ID: {len(set(key_id_list))}")
```

### Comparing `spark_quality_rules_tools-0.5.0/spark_quality_rules_tools.egg-info/PKG-INFO` & `spark_quality_rules_tools-0.6.0/spark_quality_rules_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-quality-rules-tools
-Version: 0.5.0
+Version: 0.6.0
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.5.0/spark_quality_rules_tools.egg-info/SOURCES.txt` & `spark_quality_rules_tools-0.6.0/spark_quality_rules_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

