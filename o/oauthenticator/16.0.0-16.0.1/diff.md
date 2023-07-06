# Comparing `tmp/oauthenticator-16.0.0.tar.gz` & `tmp/oauthenticator-16.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oauthenticator-16.0.0.tar", last modified: Wed Jul  5 09:29:59 2023, max compression
+gzip compressed data, was "oauthenticator-16.0.1.tar", last modified: Wed Jul  5 19:35:55 2023, max compression
```

## Comparing `oauthenticator-16.0.0.tar` & `oauthenticator-16.0.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:29:59.984432 oauthenticator-16.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-05 09:29:59.984432 oauthenticator-16.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:29:59.980432 oauthenticator-16.0.0/oauthenticator/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/auth0.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/azuread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/bitbucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    13306 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/cilogon.py
--rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    12847 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    14952 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/globus.py
--rw-r--r--   0 runner    (1001) docker     (123)    10979 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/google.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/mediawiki.py
--rw-r--r--   0 runner    (1001) docker     (123)    36900 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/okpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/openshift.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:29:59.984432 oauthenticator-16.0.0/oauthenticator/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/schemas/cilogon-schema.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:29:59.984432 oauthenticator-16.0.0/oauthenticator/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/tests/mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/tests/test_auth0.py
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/tests/test_azuread.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/tests/test_bitbucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    14935 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/tests/test_cilogon.py
--rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/tests/test_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)    12203 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/tests/test_gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    18529 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/tests/test_globus.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/tests/test_google.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/tests/test_mediawiki.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/tests/test_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/tests/test_okpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/tests/test_openshift.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:29:59.984432 oauthenticator-16.0.0/oauthenticator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-05 09:29:59.000000 oauthenticator-16.0.0/oauthenticator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-05 09:29:59.000000 oauthenticator-16.0.0/oauthenticator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 09:29:59.000000 oauthenticator-16.0.0/oauthenticator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-05 09:29:59.000000 oauthenticator-16.0.0/oauthenticator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-05 09:29:59.000000 oauthenticator-16.0.0/oauthenticator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-05 09:29:59.000000 oauthenticator-16.0.0/oauthenticator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 09:29:59.984432 oauthenticator-16.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:35:55.615785 oauthenticator-16.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-05 19:35:55.615785 oauthenticator-16.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:35:55.615785 oauthenticator-16.0.1/oauthenticator/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/oauthenticator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/oauthenticator/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/oauthenticator/auth0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/oauthenticator/azuread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/oauthenticator/bitbucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13306 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/oauthenticator/cilogon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/oauthenticator/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12847 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/oauthenticator/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/oauthenticator/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14952 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/oauthenticator/globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10979 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/oauthenticator/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/oauthenticator/mediawiki.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37380 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/oauthenticator/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/oauthenticator/okpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/oauthenticator/openshift.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:35:55.615785 oauthenticator-16.0.1/oauthenticator/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/oauthenticator/schemas/cilogon-schema.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:35:55.615785 oauthenticator-16.0.1/oauthenticator/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/oauthenticator/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/oauthenticator/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/oauthenticator/tests/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/oauthenticator/tests/test_auth0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/oauthenticator/tests/test_azuread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/oauthenticator/tests/test_bitbucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14935 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/oauthenticator/tests/test_cilogon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/oauthenticator/tests/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/oauthenticator/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12203 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/oauthenticator/tests/test_gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18529 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/oauthenticator/tests/test_globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/oauthenticator/tests/test_google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/oauthenticator/tests/test_mediawiki.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/oauthenticator/tests/test_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/oauthenticator/tests/test_okpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/oauthenticator/tests/test_openshift.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:35:55.615785 oauthenticator-16.0.1/oauthenticator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-05 19:35:55.000000 oauthenticator-16.0.1/oauthenticator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-05 19:35:55.000000 oauthenticator-16.0.1/oauthenticator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 19:35:55.000000 oauthenticator-16.0.1/oauthenticator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-05 19:35:55.000000 oauthenticator-16.0.1/oauthenticator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-05 19:35:55.000000 oauthenticator-16.0.1/oauthenticator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-05 19:35:55.000000 oauthenticator-16.0.1/oauthenticator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 19:35:55.615785 oauthenticator-16.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-07-05 19:35:45.000000 oauthenticator-16.0.1/setup.py
```

### Comparing `oauthenticator-16.0.0/CONTRIBUTING.md` & `oauthenticator-16.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.0/LICENSE` & `oauthenticator-16.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.0/PKG-INFO` & `oauthenticator-16.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oauthenticator
-Version: 16.0.0
+Version: 16.0.1
 Summary: OAuthenticator: Authenticate JupyterHub users with common OAuth providers
 Home-page: https://jupyter.org
 Author: Jupyter Development Team
 Author-email: jupyter@googlegroups.com
 License: BSD
 Keywords: Interactive,Interpreter,Shell,Web
 Platform: Linux
```

### Comparing `oauthenticator-16.0.0/README.md` & `oauthenticator-16.0.1/README.md`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.0/oauthenticator/auth0.py` & `oauthenticator-16.0.1/oauthenticator/auth0.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.0/oauthenticator/azuread.py` & `oauthenticator-16.0.1/oauthenticator/azuread.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.0/oauthenticator/bitbucket.py` & `oauthenticator-16.0.1/oauthenticator/bitbucket.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.0/oauthenticator/cilogon.py` & `oauthenticator-16.0.1/oauthenticator/cilogon.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.0/oauthenticator/generic.py` & `oauthenticator-16.0.1/oauthenticator/generic.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.0/oauthenticator/github.py` & `oauthenticator-16.0.1/oauthenticator/github.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.0/oauthenticator/gitlab.py` & `oauthenticator-16.0.1/oauthenticator/gitlab.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.0/oauthenticator/globus.py` & `oauthenticator-16.0.1/oauthenticator/globus.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.0/oauthenticator/google.py` & `oauthenticator-16.0.1/oauthenticator/google.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.0/oauthenticator/mediawiki.py` & `oauthenticator-16.0.1/oauthenticator/mediawiki.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.0/oauthenticator/oauth2.py` & `oauthenticator-16.0.1/oauthenticator/oauth2.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,14 +237,29 @@
     callback_handler = OAuthCallbackHandler
     logout_handler = OAuthLogoutHandler
 
     # user_auth_state_key represents the name of the key in the `auth_state`
     # dictionary that user info will be saved
     user_auth_state_key = "oauth_user"
 
+    login_service = Unicode(
+        "OAuth 2.0",
+        config=True,
+        help="""
+        Name of the login service or identity provider that this authenticator
+        is using to authenticate users.
+
+        This config influences the text on a button shown to unauthenticated
+        users before they click it to login, assuming :attr:`auto_login` isn't
+        configured True.
+
+        The login button's text will be "Login with <login_service>".
+        """,
+    )
+
     allow_all = Bool(
         False,
         config=True,
         help="""
         Allow all authenticated users to login.
 
         .. versionadded:: 16.0
```

### Comparing `oauthenticator-16.0.0/oauthenticator/okpy.py` & `oauthenticator-16.0.1/oauthenticator/okpy.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.0/oauthenticator/openshift.py` & `oauthenticator-16.0.1/oauthenticator/openshift.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.0/oauthenticator/schemas/cilogon-schema.yaml` & `oauthenticator-16.0.1/oauthenticator/schemas/cilogon-schema.yaml`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.0/oauthenticator/tests/mocks.py` & `oauthenticator-16.0.1/oauthenticator/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.0/oauthenticator/tests/test_auth0.py` & `oauthenticator-16.0.1/oauthenticator/tests/test_auth0.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.0/oauthenticator/tests/test_azuread.py` & `oauthenticator-16.0.1/oauthenticator/tests/test_azuread.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.0/oauthenticator/tests/test_bitbucket.py` & `oauthenticator-16.0.1/oauthenticator/tests/test_bitbucket.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.0/oauthenticator/tests/test_cilogon.py` & `oauthenticator-16.0.1/oauthenticator/tests/test_cilogon.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.0/oauthenticator/tests/test_generic.py` & `oauthenticator-16.0.1/oauthenticator/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.0/oauthenticator/tests/test_github.py` & `oauthenticator-16.0.1/oauthenticator/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.0/oauthenticator/tests/test_gitlab.py` & `oauthenticator-16.0.1/oauthenticator/tests/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.0/oauthenticator/tests/test_globus.py` & `oauthenticator-16.0.1/oauthenticator/tests/test_globus.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.0/oauthenticator/tests/test_google.py` & `oauthenticator-16.0.1/oauthenticator/tests/test_google.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.0/oauthenticator/tests/test_mediawiki.py` & `oauthenticator-16.0.1/oauthenticator/tests/test_mediawiki.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.0/oauthenticator/tests/test_oauth2.py` & `oauthenticator-16.0.1/oauthenticator/tests/test_oauth2.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.0/oauthenticator/tests/test_okpy.py` & `oauthenticator-16.0.1/oauthenticator/tests/test_okpy.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.0/oauthenticator/tests/test_openshift.py` & `oauthenticator-16.0.1/oauthenticator/tests/test_openshift.py`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.0/oauthenticator.egg-info/PKG-INFO` & `oauthenticator-16.0.1/oauthenticator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oauthenticator
-Version: 16.0.0
+Version: 16.0.1
 Summary: OAuthenticator: Authenticate JupyterHub users with common OAuth providers
 Home-page: https://jupyter.org
 Author: Jupyter Development Team
 Author-email: jupyter@googlegroups.com
 License: BSD
 Keywords: Interactive,Interpreter,Shell,Web
 Platform: Linux
```

### Comparing `oauthenticator-16.0.0/oauthenticator.egg-info/SOURCES.txt` & `oauthenticator-16.0.1/oauthenticator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.0/oauthenticator.egg-info/entry_points.txt` & `oauthenticator-16.0.1/oauthenticator.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oauthenticator-16.0.0/pyproject.toml` & `oauthenticator-16.0.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 #
 # ref: https://github.com/your-tools/tbump#readme
 #
 [tool.tbump]
 github_url = "https://github.com/jupyterhub/oauthenticator"
 
 [tool.tbump.version]
-current = "16.0.0"
+current = "16.0.1"
 regex = '''
     (?P<major>\d+)
     \.
     (?P<minor>\d+)
     \.
     (?P<patch>\d+)
     (?P<pre>((a|b|rc)\d+)|)
```

### Comparing `oauthenticator-16.0.0/setup.py` & `oauthenticator-16.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             "Aborting implicit building of eggs. Use `pip install .` to install from source."
         )
 
 
 setup_args = dict(
     name='oauthenticator',
     packages=find_packages(),
-    version="16.0.0",
+    version="16.0.1",
     description="OAuthenticator: Authenticate JupyterHub users with common OAuth providers",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Jupyter Development Team",
     author_email="jupyter@googlegroups.com",
     url="https://jupyter.org",
     license="BSD",
```

