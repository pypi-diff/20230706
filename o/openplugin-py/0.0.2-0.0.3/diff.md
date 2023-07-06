# Comparing `tmp/openplugin-py-0.0.2.tar.gz` & `tmp/openplugin-py-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openplugin-py-0.0.2.tar", last modified: Sun Jul  2 15:55:14 2023, max compression
+gzip compressed data, was "openplugin-py-0.0.3.tar", last modified: Thu Jul  6 10:01:27 2023, max compression
```

## Comparing `openplugin-py-0.0.2.tar` & `openplugin-py-0.0.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-02 15:55:14.594420 openplugin-py-0.0.2/
--rw-r--r--   0 4paradigm   (501) staff       (20)    11357 2023-06-28 13:02:04.000000 openplugin-py-0.0.2/LICENSE
--rw-r--r--   0 4paradigm   (501) staff       (20)     3244 2023-07-02 15:55:14.594259 openplugin-py-0.0.2/PKG-INFO
--rw-r--r--   0 4paradigm   (501) staff       (20)     2163 2023-07-02 15:40:39.000000 openplugin-py-0.0.2/README.md
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-02 15:55:14.590229 openplugin-py-0.0.2/openplugin/
--rw-r--r--   0 4paradigm   (501) staff       (20)     1114 2023-07-02 15:40:49.000000 openplugin-py-0.0.2/openplugin/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-02 15:55:14.590595 openplugin-py-0.0.2/openplugin/cli/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:37:33.000000 openplugin-py-0.0.2/openplugin/cli/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3080 2023-07-02 15:52:03.000000 openplugin-py-0.0.2/openplugin/cli/cli.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-02 15:55:14.590816 openplugin-py-0.0.2/openplugin/install/
--rw-r--r--   0 4paradigm   (501) staff       (20)     2464 2023-07-02 15:52:06.000000 openplugin-py-0.0.2/openplugin/install/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-02 15:55:14.591053 openplugin-py-0.0.2/openplugin/run/
--rw-r--r--   0 4paradigm   (501) staff       (20)     3342 2023-07-02 14:58:56.000000 openplugin-py-0.0.2/openplugin/run/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-02 15:55:14.592049 openplugin-py-0.0.2/openplugin/template/
--rw-r--r--   0 4paradigm   (501) staff       (20)      876 2023-07-02 15:52:03.000000 openplugin-py-0.0.2/openplugin/template/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1192 2023-07-02 15:52:03.000000 openplugin-py-0.0.2/openplugin/template/base_template.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      901 2023-07-02 15:52:03.000000 openplugin-py-0.0.2/openplugin/template/json_template.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      901 2023-07-02 15:52:03.000000 openplugin-py-0.0.2/openplugin/template/utils.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      902 2023-07-02 15:52:03.000000 openplugin-py-0.0.2/openplugin/template/yaml_template.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-02 15:55:14.593178 openplugin-py-0.0.2/openplugin/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:58:04.000000 openplugin-py-0.0.2/openplugin/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    17531 2023-06-30 09:22:51.000000 openplugin-py-0.0.2/openplugin/utils/app_util.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      915 2023-06-30 09:22:51.000000 openplugin-py-0.0.2/openplugin/utils/errors.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1868 2023-06-30 09:22:51.000000 openplugin-py-0.0.2/openplugin/utils/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-02 15:55:14.594042 openplugin-py-0.0.2/openplugin_py.egg-info/
--rw-r--r--   0 4paradigm   (501) staff       (20)     3244 2023-07-02 15:55:14.000000 openplugin-py-0.0.2/openplugin_py.egg-info/PKG-INFO
--rw-r--r--   0 4paradigm   (501) staff       (20)      662 2023-07-02 15:55:14.000000 openplugin-py-0.0.2/openplugin_py.egg-info/SOURCES.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)        1 2023-07-02 15:55:14.000000 openplugin-py-0.0.2/openplugin_py.egg-info/dependency_links.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       46 2023-07-02 15:55:14.000000 openplugin-py-0.0.2/openplugin_py.egg-info/entry_points.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)      167 2023-07-02 15:55:14.000000 openplugin-py-0.0.2/openplugin_py.egg-info/requires.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       11 2023-07-02 15:55:14.000000 openplugin-py-0.0.2/openplugin_py.egg-info/top_level.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       38 2023-07-02 15:55:14.594466 openplugin-py-0.0.2/setup.cfg
--rw-r--r--   0 4paradigm   (501) staff       (20)     2869 2023-06-30 09:40:35.000000 openplugin-py-0.0.2/setup.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-06 10:01:27.218741 openplugin-py-0.0.3/
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11357 2023-06-28 13:02:04.000000 openplugin-py-0.0.3/LICENSE
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3621 2023-07-06 10:01:27.218600 openplugin-py-0.0.3/PKG-INFO
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2540 2023-07-06 09:48:54.000000 openplugin-py-0.0.3/README.md
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-06 10:01:27.213482 openplugin-py-0.0.3/openplugin/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1114 2023-07-06 06:46:44.000000 openplugin-py-0.0.3/openplugin/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-06 10:01:27.213860 openplugin-py-0.0.3/openplugin/cli/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:37:33.000000 openplugin-py-0.0.3/openplugin/cli/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3080 2023-07-02 15:52:03.000000 openplugin-py-0.0.3/openplugin/cli/cli.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-06 10:01:27.214234 openplugin-py-0.0.3/openplugin/install/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3559 2023-07-06 09:33:01.000000 openplugin-py-0.0.3/openplugin/install/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-06 10:01:27.214622 openplugin-py-0.0.3/openplugin/run/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3342 2023-07-02 14:58:56.000000 openplugin-py-0.0.3/openplugin/run/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-06 10:01:27.216258 openplugin-py-0.0.3/openplugin/template/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      876 2023-07-02 15:52:03.000000 openplugin-py-0.0.3/openplugin/template/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1192 2023-07-02 15:52:03.000000 openplugin-py-0.0.3/openplugin/template/base_template.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      901 2023-07-02 15:52:03.000000 openplugin-py-0.0.3/openplugin/template/json_template.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      901 2023-07-02 15:52:03.000000 openplugin-py-0.0.3/openplugin/template/utils.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      902 2023-07-02 15:52:03.000000 openplugin-py-0.0.3/openplugin/template/yaml_template.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-06 10:01:27.217484 openplugin-py-0.0.3/openplugin/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:58:04.000000 openplugin-py-0.0.3/openplugin/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    17531 2023-06-30 09:22:51.000000 openplugin-py-0.0.3/openplugin/utils/app_util.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      915 2023-06-30 09:22:51.000000 openplugin-py-0.0.3/openplugin/utils/errors.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2314 2023-07-06 09:30:48.000000 openplugin-py-0.0.3/openplugin/utils/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-06 10:01:27.218408 openplugin-py-0.0.3/openplugin_py.egg-info/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3621 2023-07-06 10:01:27.000000 openplugin-py-0.0.3/openplugin_py.egg-info/PKG-INFO
+-rw-r--r--   0 4paradigm   (501) staff       (20)      662 2023-07-06 10:01:27.000000 openplugin-py-0.0.3/openplugin_py.egg-info/SOURCES.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)        1 2023-07-06 10:01:27.000000 openplugin-py-0.0.3/openplugin_py.egg-info/dependency_links.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       46 2023-07-06 10:01:27.000000 openplugin-py-0.0.3/openplugin_py.egg-info/entry_points.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)      167 2023-07-06 10:01:27.000000 openplugin-py-0.0.3/openplugin_py.egg-info/requires.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       11 2023-07-06 10:01:27.000000 openplugin-py-0.0.3/openplugin_py.egg-info/top_level.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       38 2023-07-06 10:01:27.218786 openplugin-py-0.0.3/setup.cfg
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2869 2023-06-30 09:40:35.000000 openplugin-py-0.0.3/setup.py
```

### Comparing `openplugin-py-0.0.2/LICENSE` & `openplugin-py-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.2/PKG-INFO` & `openplugin-py-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openplugin-py
-Version: 0.0.2
+Version: 0.0.3
 Summary: Toolkit and Collection for Plugins of Large Language Models
 Home-page: https://github.com/OpenRL-Lab/openplugin
 Author: openrl contributors
 Author-email: huangsy1314@163.com
 Project-URL: Code, https://github.com/OpenRL-Lab/openplugin
 Project-URL: Documentation, https://openplugin.readthedocs.io/
 Keywords: LLM plugin toolkit
@@ -35,28 +35,36 @@
 
 Toolkit for managing plugins of Large Language Model (LLM). You can install, uninstall, run and list plugins with `op`.
 
 ## Installation
 
 - `pip install openplugin-py` (or clone this repo and `pip install -e .`).
 
+
+## Plugin Store
+
+We provide plugins in [Plugin Store](https://openrl.net/plugin-store/). Users can download these plugins and use them with `op`.
+
 ## Usage
 
 - Check OpenPlugin's version with: `op --version`
 - Check system information: `op --system_info`
-- Install a plugin: `op install <plugin_name>`
-- Uninstall a plugin: `op install <plugin_name>`
+- Install a plugin: `op install <plugin_name>`. You can also install local plugins with `op install ./`.
+- Uninstall a plugin: `op uninstall <plugin_name>`
 - Start a plugin: `op run <plugin_name>`. You can use `-p` to specify the port of the plugin. By default, the port is 5003.
 - List installed plugins: `op list`
 - Reinstall plugin: `op reinstall <plugin_name>`
 
-## An example for using ikun_plugin
+## An example for using QRcode_plugin
 
-- Install ikun_plugin: `op install ikun_plugin`
-- Start ikun_plugin: `op run ikun_plugin -p server_port`
+- Install QRcode_plugin: `op install QRcode_plugin`
+- Or You can install QRcode_plugin from local:
+  - Go to the directory of QRcode_plugin: `cd plugins/QRcode_plugin`
+  - Install QRcode_plugin: `op install ./`
+- Start QRcode_plugin: `op run QRcode_plugin -p server_port`
 - Then you can get the `ai-plugin.json` file via visiting `http://<server_ip>:server_port/ai-plugin.json`
 - You can get the `openaip.yaml` file via visiting `http://<server_ip>:server_port/openaip.yaml`
 
 ## Plugins
 
 We provide some source codes of plugins. You can find them in [plugins](./plugins). 
 We call for contributions of plugins.
```

### Comparing `openplugin-py-0.0.2/README.md` & `openplugin-py-0.0.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -9,28 +9,36 @@
 
 Toolkit for managing plugins of Large Language Model (LLM). You can install, uninstall, run and list plugins with `op`.
 
 ## Installation
 
 - `pip install openplugin-py` (or clone this repo and `pip install -e .`).
 
+
+## Plugin Store
+
+We provide plugins in [Plugin Store](https://openrl.net/plugin-store/). Users can download these plugins and use them with `op`.
+
 ## Usage
 
 - Check OpenPlugin's version with: `op --version`
 - Check system information: `op --system_info`
-- Install a plugin: `op install <plugin_name>`
-- Uninstall a plugin: `op install <plugin_name>`
+- Install a plugin: `op install <plugin_name>`. You can also install local plugins with `op install ./`.
+- Uninstall a plugin: `op uninstall <plugin_name>`
 - Start a plugin: `op run <plugin_name>`. You can use `-p` to specify the port of the plugin. By default, the port is 5003.
 - List installed plugins: `op list`
 - Reinstall plugin: `op reinstall <plugin_name>`
 
-## An example for using ikun_plugin
+## An example for using QRcode_plugin
 
-- Install ikun_plugin: `op install ikun_plugin`
-- Start ikun_plugin: `op run ikun_plugin -p server_port`
+- Install QRcode_plugin: `op install QRcode_plugin`
+- Or You can install QRcode_plugin from local:
+  - Go to the directory of QRcode_plugin: `cd plugins/QRcode_plugin`
+  - Install QRcode_plugin: `op install ./`
+- Start QRcode_plugin: `op run QRcode_plugin -p server_port`
 - Then you can get the `ai-plugin.json` file via visiting `http://<server_ip>:server_port/ai-plugin.json`
 - You can get the `openaip.yaml` file via visiting `http://<server_ip>:server_port/openaip.yaml`
 
 ## Plugins
 
 We provide some source codes of plugins. You can find them in [plugins](./plugins). 
 We call for contributions of plugins.
```

### Comparing `openplugin-py-0.0.2/openplugin/__init__.py` & `openplugin-py-0.0.3/openplugin/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 
 
 __TITLE__ = "openplugin"
-__VERSION__ = "v0.0.2"
+__VERSION__ = "v0.0.3"
 __DESCRIPTION__ = "Toolkit and Collection for Plugins of Large Language Models"
 __AUTHOR__ = "OpenRL Contributors"
 __EMAIL__ = "huangshiyu@4paradigm.com"
 __version__ = __VERSION__
 
 import platform
```

### Comparing `openplugin-py-0.0.2/openplugin/cli/__init__.py` & `openplugin-py-0.0.3/openplugin/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.2/openplugin/cli/cli.py` & `openplugin-py-0.0.3/openplugin/cli/cli.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.2/openplugin/install/__init__.py` & `openplugin-py-0.0.3/openplugin/install/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,28 +12,35 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 import io
+import os
 import shutil
 import zipfile
+import tempfile
 
+from pathlib import Path
 import requests
+import json
 
 from openplugin.utils.util import (
     get_plugin_directory,
     get_plugin_list,
     get_zip_file_url,
+    make_zip_file,
 )
-
-
 # import urllib
 def install_plugin(plugin_name: str) -> bool:
+    if plugin_name == "./":
+        print("Installing current directory as plugin...")
+        return install_local_plugin()
+
     plugin_list = get_plugin_list()
     if plugin_name in plugin_list:
         print("Plugin {} already installed!".format(plugin_name))
         return True
 
     print("Installing plugin: {}...".format(plugin_name))
     zip_file_url = get_zip_file_url(plugin_name)
@@ -48,15 +55,34 @@
         z.extractall(get_plugin_directory())
     except:
         raise ValueError("plugin {} not found".format(plugin_name))
     print("Installed plugin: {}!".format(plugin_name))
     return True
     # urllib.request.urlretrieve(zip_file_url, f'{plugin_name}.zip')
 
+def install_local_plugin() -> bool:
+    info_file = Path("info.json")
+    assert info_file.exists(), "info.json not found"
+    info_dict = json.load(open("info.json", "r"))
+    assert "plugin_name" in info_dict, "plugin_name not found in info.json"
+    plugin_name = info_dict["plugin_name"]
+    print("Installing plugin: {}...".format(plugin_name))
 
+    tempdir = tempfile.mkdtemp()
+    filepath = make_zip_file(dir_to_put_file_in=tempdir,
+                             plugin_directory="./", plugin_name = plugin_name)
+
+    z = zipfile.ZipFile(filepath)
+    plugin_directory = get_plugin_directory()
+    if not plugin_directory.exists():
+        plugin_directory.mkdir(parents=True)
+    print("Extracting plugin to {}".format(plugin_directory / plugin_name))
+    z.extractall(os.path.join(get_plugin_directory(),plugin_name))
+    shutil.rmtree(tempdir, ignore_errors=True)
+    return True
 def uninstall_plugin(plugin_name: str) -> bool:
     plugin_list = get_plugin_list()
     if plugin_name not in plugin_list:
         print("Plugin {} not installed!".format(plugin_name))
         return True
 
     plugin_path = get_plugin_directory() / plugin_name
```

### Comparing `openplugin-py-0.0.2/openplugin/run/__init__.py` & `openplugin-py-0.0.3/openplugin/run/__init__.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.2/openplugin/template/__init__.py` & `openplugin-py-0.0.3/openplugin/template/__init__.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.2/openplugin/template/base_template.py` & `openplugin-py-0.0.3/openplugin/template/base_template.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.2/openplugin/template/json_template.py` & `openplugin-py-0.0.3/openplugin/template/json_template.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.2/openplugin/template/utils.py` & `openplugin-py-0.0.3/openplugin/template/utils.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.2/openplugin/template/yaml_template.py` & `openplugin-py-0.0.3/openplugin/template/yaml_template.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.2/openplugin/utils/__init__.py` & `openplugin-py-0.0.3/openplugin/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.2/openplugin/utils/app_util.py` & `openplugin-py-0.0.3/openplugin/utils/app_util.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.2/openplugin/utils/errors.py` & `openplugin-py-0.0.3/openplugin/utils/errors.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.2/openplugin/utils/util.py` & `openplugin-py-0.0.3/openplugin/utils/util.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,27 +11,28 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
-
+import os
+import shutil
 import platform
 import re
 from pathlib import Path
 from typing import Dict
 
 import numpy as np
 
 import openplugin
 
-
+REMOTE_URL = "https://openrl.net/plugin-store/download"
 def get_zip_file_url(plugin_name: str) -> str:
-    return "https://openrl.net/openplugin/download/{}".format(plugin_name)
+    return "{}/{}".format(REMOTE_URL, plugin_name)
 
 
 def get_plugin_directory() -> Path:
     return Path.home() / ".openplugin" / "plugins"
 
 
 def get_plugin_list():
@@ -39,14 +40,21 @@
     plugin_directory = get_plugin_directory()
     if plugin_directory.is_dir():
         for plugin in plugin_directory.iterdir():
             if plugin.is_dir():
                 plugin_list.append(plugin.name)
     return plugin_list
 
+def make_zip_file(dir_to_put_file_in,plugin_directory,plugin_name):
+    # create a zip file
+    zip_file_name = plugin_name
+    zip_file_parent = Path(plugin_directory).parent
+    zip_file_path = os.path.join(dir_to_put_file_in, zip_file_name)
+    shutil.make_archive(zip_file_path, 'zip', zip_file_parent,plugin_directory)
+    return os.path.join(dir_to_put_file_in, zip_file_name + '.zip')
 
 def get_system_info() -> Dict[str, str]:
     """
     Retrieve system and python env info for the current system.
 
     :return: Dictionary summing up the version for each relevant package
         and a formatted string.
```

### Comparing `openplugin-py-0.0.2/openplugin_py.egg-info/PKG-INFO` & `openplugin-py-0.0.3/openplugin_py.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openplugin-py
-Version: 0.0.2
+Version: 0.0.3
 Summary: Toolkit and Collection for Plugins of Large Language Models
 Home-page: https://github.com/OpenRL-Lab/openplugin
 Author: openrl contributors
 Author-email: huangsy1314@163.com
 Project-URL: Code, https://github.com/OpenRL-Lab/openplugin
 Project-URL: Documentation, https://openplugin.readthedocs.io/
 Keywords: LLM plugin toolkit
@@ -35,28 +35,36 @@
 
 Toolkit for managing plugins of Large Language Model (LLM). You can install, uninstall, run and list plugins with `op`.
 
 ## Installation
 
 - `pip install openplugin-py` (or clone this repo and `pip install -e .`).
 
+
+## Plugin Store
+
+We provide plugins in [Plugin Store](https://openrl.net/plugin-store/). Users can download these plugins and use them with `op`.
+
 ## Usage
 
 - Check OpenPlugin's version with: `op --version`
 - Check system information: `op --system_info`
-- Install a plugin: `op install <plugin_name>`
-- Uninstall a plugin: `op install <plugin_name>`
+- Install a plugin: `op install <plugin_name>`. You can also install local plugins with `op install ./`.
+- Uninstall a plugin: `op uninstall <plugin_name>`
 - Start a plugin: `op run <plugin_name>`. You can use `-p` to specify the port of the plugin. By default, the port is 5003.
 - List installed plugins: `op list`
 - Reinstall plugin: `op reinstall <plugin_name>`
 
-## An example for using ikun_plugin
+## An example for using QRcode_plugin
 
-- Install ikun_plugin: `op install ikun_plugin`
-- Start ikun_plugin: `op run ikun_plugin -p server_port`
+- Install QRcode_plugin: `op install QRcode_plugin`
+- Or You can install QRcode_plugin from local:
+  - Go to the directory of QRcode_plugin: `cd plugins/QRcode_plugin`
+  - Install QRcode_plugin: `op install ./`
+- Start QRcode_plugin: `op run QRcode_plugin -p server_port`
 - Then you can get the `ai-plugin.json` file via visiting `http://<server_ip>:server_port/ai-plugin.json`
 - You can get the `openaip.yaml` file via visiting `http://<server_ip>:server_port/openaip.yaml`
 
 ## Plugins
 
 We provide some source codes of plugins. You can find them in [plugins](./plugins). 
 We call for contributions of plugins.
```

### Comparing `openplugin-py-0.0.2/openplugin_py.egg-info/SOURCES.txt` & `openplugin-py-0.0.3/openplugin_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.2/setup.py` & `openplugin-py-0.0.3/setup.py`

 * *Files identical despite different names*

