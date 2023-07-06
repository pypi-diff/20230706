# Comparing `tmp/fractal_client-1.3.1.tar.gz` & `tmp/fractal_client-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_client-1.3.1.tar", max compression
+gzip compressed data, was "fractal_client-1.3.2.tar", max compression
```

## Comparing `fractal_client-1.3.1.tar` & `fractal_client-1.3.2.tar`

### file list

```diff
@@ -1,20 +1,69 @@
--rw-r--r--   0        0        0     1576 2023-06-23 06:18:32.718024 fractal_client-1.3.1/LICENSE
--rw-r--r--   0        0        0     2492 2023-06-23 06:18:32.718024 fractal_client-1.3.1/README.md
--rw-r--r--   0        0        0       22 2023-07-06 08:56:49.429672 fractal_client-1.3.1/fractal/__init__.py
--rw-r--r--   0        0        0      124 2023-06-23 06:18:32.722024 fractal_client-1.3.1/fractal/__main__.py
--rw-r--r--   0        0        0     3448 2023-06-23 06:18:32.722024 fractal_client-1.3.1/fractal/authclient.py
--rw-r--r--   0        0        0     3773 2023-06-23 06:18:32.722024 fractal_client-1.3.1/fractal/client.py
--rw-r--r--   0        0        0    12348 2023-06-23 06:18:32.722024 fractal_client-1.3.1/fractal/cmd/__init__.py
--rw-r--r--   0        0        0     6863 2023-06-23 06:18:32.722024 fractal_client-1.3.1/fractal/cmd/_aux_task_caching.py
--rw-r--r--   0        0        0     5795 2023-06-23 06:18:32.722024 fractal_client-1.3.1/fractal/cmd/_dataset.py
--rw-r--r--   0        0        0     5115 2023-06-23 06:18:32.722024 fractal_client-1.3.1/fractal/cmd/_job.py
--rw-r--r--   0        0        0     4031 2023-06-23 06:18:32.722024 fractal_client-1.3.1/fractal/cmd/_project.py
--rw-r--r--   0        0        0     7260 2023-06-23 06:18:32.722024 fractal_client-1.3.1/fractal/cmd/_task.py
--rw-r--r--   0        0        0     4620 2023-06-23 06:18:32.722024 fractal_client-1.3.1/fractal/cmd/_user.py
--rw-r--r--   0        0        0    10027 2023-06-23 06:18:32.722024 fractal_client-1.3.1/fractal/cmd/_workflow.py
--rw-r--r--   0        0        0     1285 2023-06-23 06:18:32.722024 fractal_client-1.3.1/fractal/config.py
--rw-r--r--   0        0        0     1609 2023-06-23 06:18:32.722024 fractal_client-1.3.1/fractal/interface.py
--rw-r--r--   0        0        0    23932 2023-06-23 06:18:32.722024 fractal_client-1.3.1/fractal/parser.py
--rw-r--r--   0        0        0     1265 2023-06-23 06:18:32.722024 fractal_client-1.3.1/fractal/response.py
--rw-r--r--   0        0        0     1850 2023-07-06 08:56:49.429672 fractal_client-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 fractal_client-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1576 2023-06-23 06:18:32.718024 fractal_client-1.3.2/LICENSE
+-rw-r--r--   0        0        0     2492 2023-06-23 06:18:32.718024 fractal_client-1.3.2/README.md
+-rw-r--r--   0        0        0       22 2023-07-06 09:46:14.837728 fractal_client-1.3.2/fractal/__init__.py
+-rw-r--r--   0        0        0      124 2023-06-23 06:18:32.722024 fractal_client-1.3.2/fractal/__main__.py
+-rw-r--r--   0        0        0     3448 2023-06-23 06:18:32.722024 fractal_client-1.3.2/fractal/authclient.py
+-rw-r--r--   0        0        0     3773 2023-06-23 06:18:32.722024 fractal_client-1.3.2/fractal/client.py
+-rw-r--r--   0        0        0    12348 2023-06-23 06:18:32.722024 fractal_client-1.3.2/fractal/cmd/__init__.py
+-rw-r--r--   0        0        0     6863 2023-06-23 06:18:32.722024 fractal_client-1.3.2/fractal/cmd/_aux_task_caching.py
+-rw-r--r--   0        0        0     5795 2023-06-23 06:18:32.722024 fractal_client-1.3.2/fractal/cmd/_dataset.py
+-rw-r--r--   0        0        0     5115 2023-06-23 06:18:32.722024 fractal_client-1.3.2/fractal/cmd/_job.py
+-rw-r--r--   0        0        0     4031 2023-06-23 06:18:32.722024 fractal_client-1.3.2/fractal/cmd/_project.py
+-rw-r--r--   0        0        0     7260 2023-06-23 06:18:32.722024 fractal_client-1.3.2/fractal/cmd/_task.py
+-rw-r--r--   0        0        0     4620 2023-06-23 06:18:32.722024 fractal_client-1.3.2/fractal/cmd/_user.py
+-rw-r--r--   0        0        0    10027 2023-06-23 06:18:32.722024 fractal_client-1.3.2/fractal/cmd/_workflow.py
+-rw-r--r--   0        0        0       42 2023-07-06 09:45:54.749947 fractal_client-1.3.2/fractal/common/.git
+-rw-r--r--   0        0        0      717 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      364 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/.github/workflows/project-management.yml
+-rw-r--r--   0        0        0       34 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/.gitignore
+-rw-r--r--   0        0        0      620 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1964 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/README.md
+-rw-r--r--   0        0        0        0 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/__init__.py
+-rw-r--r--   0        0        0      149 2023-07-06 09:46:22.653643 fractal_client-1.3.2/fractal/common/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0       57 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/requirements.txt
+-rw-r--r--   0        0        0      614 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/schemas/__init__.py
+-rw-r--r--   0        0        0      411 2023-07-06 09:46:22.189648 fractal_client-1.3.2/fractal/common/schemas/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1753 2023-07-06 09:46:22.221647 fractal_client-1.3.2/fractal/common/schemas/__pycache__/_validators.cpython-310.pyc
+-rw-r--r--   0        0        0     1610 2023-07-06 09:46:22.189648 fractal_client-1.3.2/fractal/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
+-rw-r--r--   0        0        0     4068 2023-07-06 09:46:22.225647 fractal_client-1.3.2/fractal/common/schemas/__pycache__/manifest.cpython-310.pyc
+-rw-r--r--   0        0        0     3537 2023-07-06 09:46:22.229647 fractal_client-1.3.2/fractal/common/schemas/__pycache__/project.cpython-310.pyc
+-rw-r--r--   0        0        0     1165 2023-07-06 09:46:22.233647 fractal_client-1.3.2/fractal/common/schemas/__pycache__/state.cpython-310.pyc
+-rw-r--r--   0        0        0     2705 2023-07-06 09:46:22.233647 fractal_client-1.3.2/fractal/common/schemas/__pycache__/task.cpython-310.pyc
+-rw-r--r--   0        0        0     3292 2023-07-06 09:46:22.237647 fractal_client-1.3.2/fractal/common/schemas/__pycache__/task_collection.cpython-310.pyc
+-rw-r--r--   0        0        0     1202 2023-07-06 09:46:22.237647 fractal_client-1.3.2/fractal/common/schemas/__pycache__/user.cpython-310.pyc
+-rw-r--r--   0        0        0     3882 2023-07-06 09:46:22.589643 fractal_client-1.3.2/fractal/common/schemas/__pycache__/workflow.cpython-310.pyc
+-rw-r--r--   0        0        0     1616 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/schemas/_validators.py
+-rw-r--r--   0        0        0     1117 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/schemas/applyworkflow.py
+-rw-r--r--   0        0        0     3479 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/schemas/manifest.py
+-rw-r--r--   0        0        0     2483 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/schemas/project.py
+-rw-r--r--   0        0        0      673 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/schemas/state.py
+-rw-r--r--   0        0        0     2578 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/schemas/task.py
+-rw-r--r--   0        0        0     2935 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/schemas/task_collection.py
+-rw-r--r--   0        0        0     1216 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/schemas/user.py
+-rw-r--r--   0        0        0     2457 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/schemas/workflow.py
+-rw-r--r--   0        0        0      415 2023-07-06 09:46:22.149648 fractal_client-1.3.2/fractal/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.2.pyc
+-rw-r--r--   0        0        0      606 2023-07-06 09:46:22.181648 fractal_client-1.3.2/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.2.pyc
+-rw-r--r--   0        0        0     3382 2023-07-06 09:46:22.593643 fractal_client-1.3.2/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.2.pyc
+-rw-r--r--   0        0        0     1241 2023-07-06 09:46:22.597643 fractal_client-1.3.2/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.2.pyc
+-rw-r--r--   0        0        0     1164 2023-07-06 09:46:22.597643 fractal_client-1.3.2/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.2.pyc
+-rw-r--r--   0        0        0     1763 2023-07-06 09:46:22.597643 fractal_client-1.3.2/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.2.pyc
+-rw-r--r--   0        0        0     2792 2023-07-06 09:46:22.601643 fractal_client-1.3.2/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.2.pyc
+-rw-r--r--   0        0        0     1335 2023-07-06 09:46:22.601643 fractal_client-1.3.2/fractal/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.2.pyc
+-rw-r--r--   0        0        0     2671 2023-07-06 09:46:22.621643 fractal_client-1.3.2/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.2.pyc
+-rw-r--r--   0        0        0     2911 2023-07-06 09:46:22.625643 fractal_client-1.3.2/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.2.pyc
+-rw-r--r--   0        0        0      139 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/tests/conftest.py
+-rw-r--r--   0        0        0      298 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/tests/test_applyworkflow.py
+-rw-r--r--   0        0        0     2144 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/tests/test_dataset.py
+-rw-r--r--   0        0        0     1420 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/tests/test_manifest.py
+-rw-r--r--   0        0        0      525 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/tests/test_project.py
+-rw-r--r--   0        0        0      551 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/tests/test_state.py
+-rw-r--r--   0        0        0     1190 2023-07-06 09:45:54.765947 fractal_client-1.3.2/fractal/common/tests/test_task.py
+-rw-r--r--   0        0        0      968 2023-07-06 09:45:54.769947 fractal_client-1.3.2/fractal/common/tests/test_task_collection.py
+-rw-r--r--   0        0        0     1499 2023-07-06 09:45:54.769947 fractal_client-1.3.2/fractal/common/tests/test_user.py
+-rw-r--r--   0        0        0     2596 2023-07-06 09:45:54.769947 fractal_client-1.3.2/fractal/common/tests/test_workflow.py
+-rw-r--r--   0        0        0     1285 2023-06-23 06:18:32.722024 fractal_client-1.3.2/fractal/config.py
+-rw-r--r--   0        0        0     1609 2023-06-23 06:18:32.722024 fractal_client-1.3.2/fractal/interface.py
+-rw-r--r--   0        0        0    23932 2023-06-23 06:18:32.722024 fractal_client-1.3.2/fractal/parser.py
+-rw-r--r--   0        0        0     1265 2023-06-23 06:18:32.722024 fractal_client-1.3.2/fractal/response.py
+-rw-r--r--   0        0        0     1850 2023-07-06 09:46:14.837728 fractal_client-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 fractal_client-1.3.2/PKG-INFO
```

### Comparing `fractal_client-1.3.1/LICENSE` & `fractal_client-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.1/README.md` & `fractal_client-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.1/fractal/authclient.py` & `fractal_client-1.3.2/fractal/authclient.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.1/fractal/client.py` & `fractal_client-1.3.2/fractal/client.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.1/fractal/cmd/__init__.py` & `fractal_client-1.3.2/fractal/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.1/fractal/cmd/_aux_task_caching.py` & `fractal_client-1.3.2/fractal/cmd/_aux_task_caching.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.1/fractal/cmd/_dataset.py` & `fractal_client-1.3.2/fractal/cmd/_dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.1/fractal/cmd/_job.py` & `fractal_client-1.3.2/fractal/cmd/_job.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.1/fractal/cmd/_project.py` & `fractal_client-1.3.2/fractal/cmd/_project.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.1/fractal/cmd/_task.py` & `fractal_client-1.3.2/fractal/cmd/_task.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.1/fractal/cmd/_user.py` & `fractal_client-1.3.2/fractal/cmd/_user.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.1/fractal/cmd/_workflow.py` & `fractal_client-1.3.2/fractal/cmd/_workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.1/fractal/config.py` & `fractal_client-1.3.2/fractal/config.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.1/fractal/interface.py` & `fractal_client-1.3.2/fractal/interface.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.1/fractal/parser.py` & `fractal_client-1.3.2/fractal/parser.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.1/fractal/response.py` & `fractal_client-1.3.2/fractal/response.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.1/pyproject.toml` & `fractal_client-1.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-client"
-version = "1.3.1"
+version = "1.3.2"
 description = "Client component of the Fractal analytics platform"
 authors = [
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
 ]
 readme = "README.md"
@@ -43,15 +43,15 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 
 [tool.bumpver]
-current_version = "1.3.1"
+current_version = "1.3.2"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_client-1.3.1/PKG-INFO` & `fractal_client-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-client
-Version: 1.3.1
+Version: 1.3.2
 Summary: Client component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal
 License: BSD-3-Clause
 Author: Tommaso Comparin
 Author-email: tommaso.comparin@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

