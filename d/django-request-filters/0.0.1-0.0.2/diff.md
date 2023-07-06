# Comparing `tmp/django_request_filters-0.0.1.tar.gz` & `tmp/django_request_filters-0.0.2.tar.gz`

## Comparing `django_request_filters-0.0.1.tar` & `django_request_filters-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 django_request_filters-0.0.1/.readthedocs.yaml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 django_request_filters-0.0.1/.vscode/settings.json
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 django_request_filters-0.0.1/request_filters/__init__.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 django_request_filters-0.0.1/request_filters/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_request_filters-0.0.1/request_filters/decorators/__init__.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 django_request_filters-0.0.1/request_filters/decorators/ip_check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_request_filters-0.0.1/request_filters/middlewares/__init__.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 django_request_filters-0.0.1/request_filters/middlewares/ip_check.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 django_request_filters-0.0.1/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 django_request_filters-0.0.1/LICENSE
--rw-r--r--   0        0        0     5625 2020-02-02 00:00:00.000000 django_request_filters-0.0.1/README.md
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 django_request_filters-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     6514 2020-02-02 00:00:00.000000 django_request_filters-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 django_request_filters-0.0.2/.readthedocs.yaml
+-rw-r--r--   0        0        0   107725 2020-02-02 00:00:00.000000 django_request_filters-0.0.2/README.pdf
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 django_request_filters-0.0.2/request_filters/__init__.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 django_request_filters-0.0.2/request_filters/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_request_filters-0.0.2/request_filters/decorators/__init__.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 django_request_filters-0.0.2/request_filters/decorators/ip_check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_request_filters-0.0.2/request_filters/middlewares/__init__.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 django_request_filters-0.0.2/request_filters/middlewares/ip_check.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 django_request_filters-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 django_request_filters-0.0.2/LICENSE
+-rw-r--r--   0        0        0     5438 2020-02-02 00:00:00.000000 django_request_filters-0.0.2/README.md
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 django_request_filters-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 django_request_filters-0.0.2/PKG-INFO
```

### Comparing `django_request_filters-0.0.1/.readthedocs.yaml` & `django_request_filters-0.0.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `django_request_filters-0.0.1/request_filters/utils.py` & `django_request_filters-0.0.2/request_filters/utils.py`

 * *Files identical despite different names*

### Comparing `django_request_filters-0.0.1/request_filters/decorators/ip_check.py` & `django_request_filters-0.0.2/request_filters/decorators/ip_check.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         return func(*args, **kwargs)
 
     # copiedFunc = func
     # copiedFunc.__name__ = '_exempt_IPCheckMiddleware'
     return _exempt_IPCheckMiddleware
 
 
-def prevent_anonymous_ip(func, block_vpn=True, block_proxy=True, block_tor=True, block_relay=True):
+def prevent_anonymous_ip(func, block_vpn=setting("BLOCK_VPN", True), block_proxy=setting("BLOCK_PROXY", True), block_tor=setting("BLOCK_TOR", True), block_relay=setting("BLOCK_RELAY", True)):
     def innerFunction(*args, **kwargs):
         request = args[0]
         client_ip, is_routable = get_client_ip(request)
         userIp = getUserIpInfo(client_ip)
         if isAnonymousIP(userIp, block_vpn, block_proxy, block_tor, block_relay):
             if setting('IP_BLOCK_VIEW') is None:
                 return HttpResponse("<h1>We can't allow your request, because you are using VPN or Proxy or Tor or Relay.</h1>", status=418)
```

### Comparing `django_request_filters-0.0.1/request_filters/middlewares/ip_check.py` & `django_request_filters-0.0.2/request_filters/middlewares/ip_check.py`

 * *Files identical despite different names*

### Comparing `django_request_filters-0.0.1/.gitignore` & `django_request_filters-0.0.2/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -153,8 +153,9 @@
 cython_debug/
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-#.idea/
+.idea/
+.vscode/
```

### Comparing `django_request_filters-0.0.1/LICENSE` & `django_request_filters-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_request_filters-0.0.1/README.md` & `django_request_filters-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -26,30 +26,31 @@
    If you want to show your designed page to blocked users, you can follow this step.
 
    * Define a vew function:
 
      ```python
      # For example we defined a view function in views.py
      from django.shortcuts import render
+     from request_filters.decorators.ip_check import exempt_IPCheckMiddleware
 
      @exempt_IPCheckMiddleware
      def blockView(request):
         return render(request, 'block_view.html')
      ```
 
      As we must need to display the view function to blocked users, so the `exempt_IPCheckMiddleware` must be used in that view function.
    * Add the path of the view function in **settings.py**:
 
      ```python
      IP_BLOCK_VIEW = "app_name.views.blockView"
      ```
 
      If you do not defined any view function for blocked users, then by default it will show a simple HTML page contains a text "We can't allow your request, because you are using VPN or Proxy or Tor or Relay." with *status code* 418.
-
 4. Add additional settings in **settings.py** (optional):
+
    * `BLOCK_VPN (optional default: True)`
      If set to `True` all the users want accessing the site with VPN will be disallowed.
      If set to `False`, users can access the site using VPN.
    * `BLOCK_PROXY (optional default: True)`
      If set to `True` all the users want accessing the site with Proxy will be disallowed.
      If set to `False`, users can access the site using Proxy.
    * `BLOCK_TOR (optional default: True)`
@@ -79,33 +80,30 @@
 ```
 
 2. Exempt from some view functions
    Adding the *middleware* will block the anonymous users, so that those users can visit any views.
    If you want to allow anonymous users to visit only some specific views, you can do that by using the `exempt_IPCheckMiddleware` decorator on the view function.
 
    ```python
-   from request_filters.decorators import exempt_IPCheckMiddleware
+   from request_filters.decorators.ip_check import exempt_IPCheckMiddleware
 
    @exempt_IPCheckMiddleware
    def home(request):
         .........
         .........
    ```
 
    Here, for the above code sample, all the users (including anonymous users) can visit the *home view*.
 
 ##### Using only Decorator (Use case 2):
 
-You can also controll uses' request using decorator and without using Middleware. There are two decorators available -
+You can also controll uses' request using decorator and without using Middleware. 
 
-* `exempt_IPCheckMiddleware`
-  Import this decorator by - `from request_filters.decorators import exempt_IPCheckMiddleware`
-  If  you add this decorator in a view function, this view will accessable for all the users (including anonymous users)
 * `prevent_anonymous_ip`
-  Import this decorator by - `from request_filters.decorators import prevent_anonymous_ip`
+  Import this decorator by - `from request_filters.decorators.ip_check import prevent_anonymous_ip`
   If you add this decorator to a view function, this view function will not acessable to anonymous users.
   This decorator has some optional parameter -
   * `block_vpn (optional default: settings.BLOCK_VPN)`
     If set to `True` VPN users can't visit the view function.
     If set to `False`, VPN users can visit the view.
   * `block_proxy (optional default: settings.BLOCK_PROXY)`
     If set to `True` Proxy users can't visit the view function.
```

### Comparing `django_request_filters-0.0.1/pyproject.toml` & `django_request_filters-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
 [project]
 name = "django-request-filters"
 dynamic = ["version"]
 authors = [
   { name="Samiddha Chakrabarti", email="samiddha99@protonmail.com" },
 ]
+maintainers = [
+  { name="Samiddha Chakrabarti", email="samiddha99@protonmail.com" },
+]
+keywords = ["django", "python", "security", "cybersecurity", "VPN", "Proxy", "TOR", "Relay", "djabgo security"]
 description = "Block the users those are using VPN, Proxy, TOR or Relay."
 dependencies = ["django", "requests", "django-ipware"]
 readme = "README.md"
 requires-python = ">=3.10"
 license = "MIT"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `django_request_filters-0.0.1/PKG-INFO` & `django_request_filters-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: django-request-filters
-Version: 0.0.1
+Version: 0.0.2
 Summary: Block the users those are using VPN, Proxy, TOR or Relay.
 Project-URL: Homepage, https://pypi.org/project/django-request-filters
 Project-URL: Source code, https://github.com/Samiddha99/django-request-filters
 Project-URL: Bug Tracker, https://github.com/Samiddha99/django-request-filters/issues
 Author-email: Samiddha Chakrabarti <samiddha99@protonmail.com>
+Maintainer-email: Samiddha Chakrabarti <samiddha99@protonmail.com>
 License-Expression: MIT
 License-File: LICENSE
+Keywords: Proxy,Relay,TOR,VPN,cybersecurity,djabgo security,django,python,security
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -51,30 +53,31 @@
    If you want to show your designed page to blocked users, you can follow this step.
 
    * Define a vew function:
 
      ```python
      # For example we defined a view function in views.py
      from django.shortcuts import render
+     from request_filters.decorators.ip_check import exempt_IPCheckMiddleware
 
      @exempt_IPCheckMiddleware
      def blockView(request):
         return render(request, 'block_view.html')
      ```
 
      As we must need to display the view function to blocked users, so the `exempt_IPCheckMiddleware` must be used in that view function.
    * Add the path of the view function in **settings.py**:
 
      ```python
      IP_BLOCK_VIEW = "app_name.views.blockView"
      ```
 
      If you do not defined any view function for blocked users, then by default it will show a simple HTML page contains a text "We can't allow your request, because you are using VPN or Proxy or Tor or Relay." with *status code* 418.
-
 4. Add additional settings in **settings.py** (optional):
+
    * `BLOCK_VPN (optional default: True)`
      If set to `True` all the users want accessing the site with VPN will be disallowed.
      If set to `False`, users can access the site using VPN.
    * `BLOCK_PROXY (optional default: True)`
      If set to `True` all the users want accessing the site with Proxy will be disallowed.
      If set to `False`, users can access the site using Proxy.
    * `BLOCK_TOR (optional default: True)`
@@ -104,33 +107,30 @@
 ```
 
 2. Exempt from some view functions
    Adding the *middleware* will block the anonymous users, so that those users can visit any views.
    If you want to allow anonymous users to visit only some specific views, you can do that by using the `exempt_IPCheckMiddleware` decorator on the view function.
 
    ```python
-   from request_filters.decorators import exempt_IPCheckMiddleware
+   from request_filters.decorators.ip_check import exempt_IPCheckMiddleware
 
    @exempt_IPCheckMiddleware
    def home(request):
         .........
         .........
    ```
 
    Here, for the above code sample, all the users (including anonymous users) can visit the *home view*.
 
 ##### Using only Decorator (Use case 2):
 
-You can also controll uses' request using decorator and without using Middleware. There are two decorators available -
+You can also controll uses' request using decorator and without using Middleware. 
 
-* `exempt_IPCheckMiddleware`
-  Import this decorator by - `from request_filters.decorators import exempt_IPCheckMiddleware`
-  If  you add this decorator in a view function, this view will accessable for all the users (including anonymous users)
 * `prevent_anonymous_ip`
-  Import this decorator by - `from request_filters.decorators import prevent_anonymous_ip`
+  Import this decorator by - `from request_filters.decorators.ip_check import prevent_anonymous_ip`
   If you add this decorator to a view function, this view function will not acessable to anonymous users.
   This decorator has some optional parameter -
   * `block_vpn (optional default: settings.BLOCK_VPN)`
     If set to `True` VPN users can't visit the view function.
     If set to `False`, VPN users can visit the view.
   * `block_proxy (optional default: settings.BLOCK_PROXY)`
     If set to `True` Proxy users can't visit the view function.
```

