# Comparing `tmp/looker_deployer-0.3.8.tar.gz` & `tmp/looker_deployer-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "looker_deployer-0.3.8.tar", last modified: Fri Oct  7 20:56:18 2022, max compression
+gzip compressed data, was "looker_deployer-0.3.9.tar", last modified: Mon Feb 20 21:19:11 2023, max compression
```

## Comparing `looker_deployer-0.3.8.tar` & `looker_deployer-0.3.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 20:56:18.614195 looker_deployer-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-10-07 20:56:05.000000 looker_deployer-0.3.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)    23584 2022-10-07 20:56:18.614195 looker_deployer-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    23228 2022-10-07 20:56:05.000000 looker_deployer-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 20:56:18.610195 looker_deployer-0.3.8/looker_deployer/
--rw-r--r--   0 runner    (1001) docker     (121)      575 2022-10-07 20:56:05.000000 looker_deployer-0.3.8/looker_deployer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12394 2022-10-07 20:56:05.000000 looker_deployer-0.3.8/looker_deployer/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 20:56:18.610195 looker_deployer-0.3.8/looker_deployer/commands/
--rw-r--r--   0 runner    (1001) docker     (121)      575 2022-10-07 20:56:05.000000 looker_deployer-0.3.8/looker_deployer/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9640 2022-10-07 20:56:05.000000 looker_deployer-0.3.8/looker_deployer/commands/deploy_boards.py
--rw-r--r--   0 runner    (1001) docker     (121)     4002 2022-10-07 20:56:05.000000 looker_deployer-0.3.8/looker_deployer/commands/deploy_code.py
--rw-r--r--   0 runner    (1001) docker     (121)     3294 2022-10-07 20:56:05.000000 looker_deployer-0.3.8/looker_deployer/commands/deploy_connections.py
--rw-r--r--   0 runner    (1001) docker     (121)    12645 2022-10-07 20:56:05.000000 looker_deployer-0.3.8/looker_deployer/commands/deploy_content.py
--rw-r--r--   0 runner    (1001) docker     (121)     3374 2022-10-07 20:56:05.000000 looker_deployer-0.3.8/looker_deployer/commands/deploy_content_export.py
--rw-r--r--   0 runner    (1001) docker     (121)     4457 2022-10-07 20:56:05.000000 looker_deployer-0.3.8/looker_deployer/commands/deploy_group_in_group.py
--rw-r--r--   0 runner    (1001) docker     (121)     3386 2022-10-07 20:56:05.000000 looker_deployer-0.3.8/looker_deployer/commands/deploy_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)     3760 2022-10-07 20:56:05.000000 looker_deployer-0.3.8/looker_deployer/commands/deploy_model_sets.py
--rw-r--r--   0 runner    (1001) docker     (121)     4448 2022-10-07 20:56:05.000000 looker_deployer-0.3.8/looker_deployer/commands/deploy_permission_sets.py
--rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-10-07 20:56:05.000000 looker_deployer-0.3.8/looker_deployer/commands/deploy_role_to_group.py
--rw-r--r--   0 runner    (1001) docker     (121)     3911 2022-10-07 20:56:05.000000 looker_deployer-0.3.8/looker_deployer/commands/deploy_roles.py
--rw-r--r--   0 runner    (1001) docker     (121)     6226 2022-10-07 20:56:05.000000 looker_deployer-0.3.8/looker_deployer/commands/deploy_user_attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 20:56:18.614195 looker_deployer-0.3.8/looker_deployer/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      575 2022-10-07 20:56:05.000000 looker_deployer-0.3.8/looker_deployer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2384 2022-10-07 20:56:05.000000 looker_deployer-0.3.8/looker_deployer/utils/deploy_logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     1578 2022-10-07 20:56:05.000000 looker_deployer-0.3.8/looker_deployer/utils/get_client.py
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-10-07 20:56:05.000000 looker_deployer-0.3.8/looker_deployer/utils/match_by_key.py
--rw-r--r--   0 runner    (1001) docker     (121)      714 2022-10-07 20:56:05.000000 looker_deployer-0.3.8/looker_deployer/utils/parse_ini.py
--rw-r--r--   0 runner    (1001) docker     (121)      598 2022-10-07 20:56:05.000000 looker_deployer-0.3.8/looker_deployer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 20:56:18.610195 looker_deployer-0.3.8/looker_deployer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    23584 2022-10-07 20:56:18.000000 looker_deployer-0.3.8/looker_deployer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1116 2022-10-07 20:56:18.000000 looker_deployer-0.3.8/looker_deployer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-07 20:56:18.000000 looker_deployer-0.3.8/looker_deployer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-10-07 20:56:18.000000 looker_deployer-0.3.8/looker_deployer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-10-07 20:56:18.000000 looker_deployer-0.3.8/looker_deployer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-10-07 20:56:18.000000 looker_deployer-0.3.8/looker_deployer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-07 20:56:18.614195 looker_deployer-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1354 2022-10-07 20:56:05.000000 looker_deployer-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 21:19:11.678456 looker_deployer-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-02-20 21:19:09.000000 looker_deployer-0.3.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    23584 2023-02-20 21:19:11.678456 looker_deployer-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23228 2023-02-20 21:19:09.000000 looker_deployer-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 21:19:11.674456 looker_deployer-0.3.9/looker_deployer/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-02-20 21:19:09.000000 looker_deployer-0.3.9/looker_deployer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12642 2023-02-20 21:19:09.000000 looker_deployer-0.3.9/looker_deployer/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 21:19:11.674456 looker_deployer-0.3.9/looker_deployer/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-02-20 21:19:09.000000 looker_deployer-0.3.9/looker_deployer/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-02-20 21:19:09.000000 looker_deployer-0.3.9/looker_deployer/commands/deploy_boards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-02-20 21:19:09.000000 looker_deployer-0.3.9/looker_deployer/commands/deploy_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-02-20 21:19:09.000000 looker_deployer-0.3.9/looker_deployer/commands/deploy_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12645 2023-02-20 21:19:09.000000 looker_deployer-0.3.9/looker_deployer/commands/deploy_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-02-20 21:19:09.000000 looker_deployer-0.3.9/looker_deployer/commands/deploy_content_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-02-20 21:19:09.000000 looker_deployer-0.3.9/looker_deployer/commands/deploy_group_in_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-02-20 21:19:09.000000 looker_deployer-0.3.9/looker_deployer/commands/deploy_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-02-20 21:19:09.000000 looker_deployer-0.3.9/looker_deployer/commands/deploy_model_sets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-02-20 21:19:09.000000 looker_deployer-0.3.9/looker_deployer/commands/deploy_permission_sets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-02-20 21:19:09.000000 looker_deployer-0.3.9/looker_deployer/commands/deploy_role_to_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-02-20 21:19:09.000000 looker_deployer-0.3.9/looker_deployer/commands/deploy_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-02-20 21:19:09.000000 looker_deployer-0.3.9/looker_deployer/commands/deploy_user_attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 21:19:11.678456 looker_deployer-0.3.9/looker_deployer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-02-20 21:19:09.000000 looker_deployer-0.3.9/looker_deployer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-02-20 21:19:09.000000 looker_deployer-0.3.9/looker_deployer/utils/deploy_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-02-20 21:19:09.000000 looker_deployer-0.3.9/looker_deployer/utils/get_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-02-20 21:19:09.000000 looker_deployer-0.3.9/looker_deployer/utils/match_by_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-02-20 21:19:09.000000 looker_deployer-0.3.9/looker_deployer/utils/parse_ini.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-02-20 21:19:09.000000 looker_deployer-0.3.9/looker_deployer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 21:19:11.674456 looker_deployer-0.3.9/looker_deployer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23584 2023-02-20 21:19:11.000000 looker_deployer-0.3.9/looker_deployer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-02-20 21:19:11.000000 looker_deployer-0.3.9/looker_deployer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 21:19:11.000000 looker_deployer-0.3.9/looker_deployer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-20 21:19:11.000000 looker_deployer-0.3.9/looker_deployer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-20 21:19:11.000000 looker_deployer-0.3.9/looker_deployer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-20 21:19:11.000000 looker_deployer-0.3.9/looker_deployer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 21:19:11.678456 looker_deployer-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-02-20 21:19:09.000000 looker_deployer-0.3.9/setup.py
```

### Comparing `looker_deployer-0.3.8/LICENSE.txt` & `looker_deployer-0.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `looker_deployer-0.3.8/PKG-INFO` & `looker_deployer-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: looker_deployer
-Version: 0.3.8
+Version: 0.3.9
 Summary: A Looker Deployment Tool
 Home-page: UNKNOWN
 Author: Looker Open Source
 Author-email: looker-open-source@google.com
 License: Apache License 2.0
 Keywords: Looker Deployer
 Platform: UNKNOWN
-Requires-Python: >=3.6.0, <3.10
+Requires-Python: >=3.6.0, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Looker Deployer
 
 ![badge](https://github.com/looker-open-source/looker_deployer/workflows/python_application/badge.svg)
```

### Comparing `looker_deployer-0.3.8/README.md` & `looker_deployer-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `looker_deployer-0.3.8/looker_deployer/__init__.py` & `looker_deployer-0.3.9/looker_deployer/__init__.py`

 * *Files identical despite different names*

### Comparing `looker_deployer-0.3.8/looker_deployer/cli.py` & `looker_deployer-0.3.9/looker_deployer/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -103,27 +103,30 @@
     import_export_subparsers = content_subparser.add_subparsers()
     export_subparser = import_export_subparsers.add_parser("export")
     import_subparser = import_export_subparsers.add_parser("import")
 
     export_subparser.add_argument("--env", required=True, help="What environment to deploy to")
     export_subparser.add_argument("--ini", default=loc, help="ini file to parse for credentials")
     export_subparser.add_argument("--debug", action="store_true", help="set logger to debug for more verbosity")
-    export_subparser.add_argument("--folders", nargs="+", required=True, help="What folders to export content from")
     export_subparser.add_argument("--local-target", required=True, help="Local directory to store content")
+    export_content_group = export_subparser.add_argument_group()
+    export_content_group.add_argument("--folders", nargs="+", help="Folders to fully export")
+    export_content_group.add_argument("--dashboards", nargs="+", help="Dashboards to export")
+    export_content_group.add_argument("--looks", nargs="+", help="Looks to export")
     export_subparser.set_defaults(func=deploy_content_export.main)
 
     import_subparser.add_argument("--env", required=True, help="What environment to deploy to")
     import_subparser.add_argument("--ini", default=loc, help="ini file to parse for credentials")
     import_subparser.add_argument("--debug", action="store_true", help="set logger to debug for more verbosity")
     import_subparser.add_argument("--recursive", action="store_true", help="Should folders deploy recursively")
     import_subparser.add_argument("--target-folder", help="override the default target folder with a custom path")
-    content_group = import_subparser.add_mutually_exclusive_group(required=True)
-    content_group.add_argument("--folders", nargs="+", help="Folders to fully deploy")
-    content_group.add_argument("--dashboards", nargs="+", help="Dashboards to deploy")
-    content_group.add_argument("--looks", nargs="+", help="Looks to deploy")
+    import_content_group = import_subparser.add_mutually_exclusive_group(required=True)
+    import_content_group.add_argument("--folders", nargs="+", help="Folders to fully deploy")
+    import_content_group.add_argument("--dashboards", nargs="+", help="Dashboards to deploy")
+    import_content_group.add_argument("--looks", nargs="+", help="Looks to deploy")
     import_subparser.set_defaults(func=deploy_content.main)
 
 
 def setup_permission_sets_subparser(subparsers):
     permission_sets_subparser = subparsers.add_parser("permission_sets")
     permission_sets_subparser.add_argument("--source", required=True, help="which environment to source the permission sets from")
     permission_sets_subparser.add_argument("--ini", default=loc, help="ini file to parse for credentials")
```

### Comparing `looker_deployer-0.3.8/looker_deployer/commands/__init__.py` & `looker_deployer-0.3.9/looker_deployer/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `looker_deployer-0.3.8/looker_deployer/commands/deploy_boards.py` & `looker_deployer-0.3.9/looker_deployer/commands/deploy_boards.py`

 * *Files identical despite different names*

### Comparing `looker_deployer-0.3.8/looker_deployer/commands/deploy_code.py` & `looker_deployer-0.3.9/looker_deployer/commands/deploy_code.py`

 * *Files identical despite different names*

### Comparing `looker_deployer-0.3.8/looker_deployer/commands/deploy_connections.py` & `looker_deployer-0.3.9/looker_deployer/commands/deploy_connections.py`

 * *Files identical despite different names*

### Comparing `looker_deployer-0.3.8/looker_deployer/commands/deploy_content.py` & `looker_deployer-0.3.9/looker_deployer/commands/deploy_content.py`

 * *Files identical despite different names*

### Comparing `looker_deployer-0.3.8/looker_deployer/commands/deploy_group_in_group.py` & `looker_deployer-0.3.9/looker_deployer/commands/deploy_group_in_group.py`

 * *Files identical despite different names*

### Comparing `looker_deployer-0.3.8/looker_deployer/commands/deploy_groups.py` & `looker_deployer-0.3.9/looker_deployer/commands/deploy_groups.py`

 * *Files identical despite different names*

### Comparing `looker_deployer-0.3.8/looker_deployer/commands/deploy_model_sets.py` & `looker_deployer-0.3.9/looker_deployer/commands/deploy_model_sets.py`

 * *Files identical despite different names*

### Comparing `looker_deployer-0.3.8/looker_deployer/commands/deploy_permission_sets.py` & `looker_deployer-0.3.9/looker_deployer/commands/deploy_permission_sets.py`

 * *Files identical despite different names*

### Comparing `looker_deployer-0.3.8/looker_deployer/commands/deploy_role_to_group.py` & `looker_deployer-0.3.9/looker_deployer/commands/deploy_role_to_group.py`

 * *Files identical despite different names*

### Comparing `looker_deployer-0.3.8/looker_deployer/commands/deploy_roles.py` & `looker_deployer-0.3.9/looker_deployer/commands/deploy_roles.py`

 * *Files identical despite different names*

### Comparing `looker_deployer-0.3.8/looker_deployer/commands/deploy_user_attributes.py` & `looker_deployer-0.3.9/looker_deployer/commands/deploy_user_attributes.py`

 * *Files identical despite different names*

### Comparing `looker_deployer-0.3.8/looker_deployer/utils/__init__.py` & `looker_deployer-0.3.9/looker_deployer/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `looker_deployer-0.3.8/looker_deployer/utils/deploy_logging.py` & `looker_deployer-0.3.9/looker_deployer/utils/deploy_logging.py`

 * *Files identical despite different names*

### Comparing `looker_deployer-0.3.8/looker_deployer/utils/get_client.py` & `looker_deployer-0.3.9/looker_deployer/utils/get_client.py`

 * *Files identical despite different names*

### Comparing `looker_deployer-0.3.8/looker_deployer/utils/parse_ini.py` & `looker_deployer-0.3.9/looker_deployer/utils/parse_ini.py`

 * *Files identical despite different names*

### Comparing `looker_deployer-0.3.8/looker_deployer/version.py` & `looker_deployer-0.3.9/looker_deployer/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.3.8"
+__version__ = "0.3.9"
```

### Comparing `looker_deployer-0.3.8/looker_deployer.egg-info/PKG-INFO` & `looker_deployer-0.3.9/looker_deployer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: looker-deployer
-Version: 0.3.8
+Version: 0.3.9
 Summary: A Looker Deployment Tool
 Home-page: UNKNOWN
 Author: Looker Open Source
 Author-email: looker-open-source@google.com
 License: Apache License 2.0
 Keywords: Looker Deployer
 Platform: UNKNOWN
-Requires-Python: >=3.6.0, <3.10
+Requires-Python: >=3.6.0, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Looker Deployer
 
 ![badge](https://github.com/looker-open-source/looker_deployer/workflows/python_application/badge.svg)
```

### Comparing `looker_deployer-0.3.8/looker_deployer.egg-info/SOURCES.txt` & `looker_deployer-0.3.9/looker_deployer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `looker_deployer-0.3.8/setup.py` & `looker_deployer-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,10 +27,10 @@
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords=["Looker Deployer"],
     license="Apache License 2.0",
     name=NAME,
     packages=["looker_deployer", "looker_deployer/commands", "looker_deployer/utils"],
     entry_points={"console_scripts": ["ldeploy=looker_deployer.cli:main"]},
-    python_requires=">=3.6.0, <3.10",
+    python_requires=">=3.6.0, <3.11",
     version=VERSION
 )
```

