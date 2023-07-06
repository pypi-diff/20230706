# Comparing `tmp/django-subadmin-3.2.1.tar.gz` & `tmp/django-subadmin-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-subadmin-3.2.1.tar", last modified: Wed Jul  6 23:21:25 2022, max compression
+gzip compressed data, was "django-subadmin-3.2.2.tar", last modified: Thu Jul  6 09:46:00 2023, max compression
```

## Comparing `django-subadmin-3.2.1.tar` & `django-subadmin-3.2.2.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 mpagon     (501) staff       (20)        0 2022-07-06 23:21:25.000000 django-subadmin-3.2.1/
--rw-r--r--   0 mpagon     (501) staff       (20)     1545 2022-07-06 23:17:43.000000 django-subadmin-3.2.1/CHANGELOG.md
--rw-r--r--   0 mpagon     (501) staff       (20)     1085 2020-04-11 12:31:01.000000 django-subadmin-3.2.1/LICENSE
--rw-r--r--   0 mpagon     (501) staff       (20)      144 2020-04-11 12:31:01.000000 django-subadmin-3.2.1/MANIFEST.in
--rw-r--r--   0 mpagon     (501) staff       (20)     7222 2022-07-06 23:21:25.000000 django-subadmin-3.2.1/PKG-INFO
--rw-r--r--   0 mpagon     (501) staff       (20)     5384 2020-04-11 21:07:17.000000 django-subadmin-3.2.1/README.md
-drwxr-xr-x   0 mpagon     (501) staff       (20)        0 2022-07-06 23:21:25.000000 django-subadmin-3.2.1/django_subadmin.egg-info/
--rw-r--r--   0 mpagon     (501) staff       (20)     7222 2022-07-06 23:21:25.000000 django-subadmin-3.2.1/django_subadmin.egg-info/PKG-INFO
--rw-r--r--   0 mpagon     (501) staff       (20)      734 2022-07-06 23:21:25.000000 django-subadmin-3.2.1/django_subadmin.egg-info/SOURCES.txt
--rw-r--r--   0 mpagon     (501) staff       (20)        1 2022-07-06 23:21:25.000000 django-subadmin-3.2.1/django_subadmin.egg-info/dependency_links.txt
--rw-r--r--   0 mpagon     (501) staff       (20)        1 2020-05-17 10:15:51.000000 django-subadmin-3.2.1/django_subadmin.egg-info/not-zip-safe
--rw-r--r--   0 mpagon     (501) staff       (20)        9 2022-07-06 23:21:25.000000 django-subadmin-3.2.1/django_subadmin.egg-info/top_level.txt
--rw-r--r--   0 mpagon     (501) staff       (20)       38 2022-07-06 23:21:25.000000 django-subadmin-3.2.1/setup.cfg
--rw-r--r--   0 mpagon     (501) staff       (20)     1593 2022-07-06 23:14:39.000000 django-subadmin-3.2.1/setup.py
-drwxr-xr-x   0 mpagon     (501) staff       (20)        0 2022-07-06 23:21:25.000000 django-subadmin-3.2.1/subadmin/
--rw-r--r--   0 mpagon     (501) staff       (20)    23209 2022-07-06 23:16:29.000000 django-subadmin-3.2.1/subadmin/__init__.py
-drwxr-xr-x   0 mpagon     (501) staff       (20)        0 2022-07-06 23:21:25.000000 django-subadmin-3.2.1/subadmin/templates/
-drwxr-xr-x   0 mpagon     (501) staff       (20)        0 2022-07-06 23:21:25.000000 django-subadmin-3.2.1/subadmin/templates/subadmin/
--rw-r--r--   0 mpagon     (501) staff       (20)      313 2020-04-11 12:31:01.000000 django-subadmin-3.2.1/subadmin/templates/subadmin/breadcrumbs.html
--rw-r--r--   0 mpagon     (501) staff       (20)     1047 2020-04-11 12:31:01.000000 django-subadmin-3.2.1/subadmin/templates/subadmin/change_form.html
--rw-r--r--   0 mpagon     (501) staff       (20)      569 2020-04-11 12:31:01.000000 django-subadmin-3.2.1/subadmin/templates/subadmin/change_list.html
--rw-r--r--   0 mpagon     (501) staff       (20)      421 2020-04-11 12:31:01.000000 django-subadmin-3.2.1/subadmin/templates/subadmin/delete_confirmation.html
--rw-r--r--   0 mpagon     (501) staff       (20)      338 2020-04-11 12:31:01.000000 django-subadmin-3.2.1/subadmin/templates/subadmin/delete_selected_confirmation.html
--rw-r--r--   0 mpagon     (501) staff       (20)      418 2020-04-11 12:31:01.000000 django-subadmin-3.2.1/subadmin/templates/subadmin/object_history.html
--rw-r--r--   0 mpagon     (501) staff       (20)      266 2020-04-11 12:31:01.000000 django-subadmin-3.2.1/subadmin/templates/subadmin/parent_change_form.html
--rw-r--r--   0 mpagon     (501) staff       (20)      791 2020-04-11 12:31:01.000000 django-subadmin-3.2.1/subadmin/templates/subadmin/submit_line.html
-drwxr-xr-x   0 mpagon     (501) staff       (20)        0 2022-07-06 23:21:25.000000 django-subadmin-3.2.1/subadmin/templatetags/
--rw-r--r--   0 mpagon     (501) staff       (20)        1 2020-04-11 12:31:01.000000 django-subadmin-3.2.1/subadmin/templatetags/__init__.py
--rw-r--r--   0 mpagon     (501) staff       (20)     1920 2022-06-28 09:47:42.000000 django-subadmin-3.2.1/subadmin/templatetags/subadmin_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:46:00.194272 django-subadmin-3.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:46:00.190272 django-subadmin-3.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:46:00.190272 django-subadmin-3.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/.github/workflows/publish_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-07-06 09:46:00.194272 django-subadmin-3.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:46:00.190272 django-subadmin-3.2.2/django_subadmin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-07-06 09:46:00.000000 django-subadmin-3.2.2/django_subadmin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-06 09:46:00.000000 django-subadmin-3.2.2/django_subadmin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 09:46:00.000000 django-subadmin-3.2.2/django_subadmin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 09:46:00.000000 django-subadmin-3.2.2/django_subadmin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 09:46:00.194272 django-subadmin-3.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:46:00.190272 django-subadmin-3.2.2/subadmin/
+-rw-r--r--   0 runner    (1001) docker     (123)    23209 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/subadmin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:46:00.190272 django-subadmin-3.2.2/subadmin/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:46:00.194272 django-subadmin-3.2.2/subadmin/templates/subadmin/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/subadmin/templates/subadmin/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/subadmin/templates/subadmin/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/subadmin/templates/subadmin/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/subadmin/templates/subadmin/delete_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/subadmin/templates/subadmin/delete_selected_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/subadmin/templates/subadmin/object_history.html
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/subadmin/templates/subadmin/parent_change_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/subadmin/templates/subadmin/submit_line.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:46:00.194272 django-subadmin-3.2.2/subadmin/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/subadmin/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-06 09:45:50.000000 django-subadmin-3.2.2/subadmin/templatetags/subadmin_tags.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-subadmin-3.2.1/LICENSE` & `django-subadmin-3.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-subadmin-3.2.1/PKG-INFO` & `django-subadmin-3.2.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,137 +1,136 @@
 Metadata-Version: 2.1
 Name: django-subadmin
-Version: 3.2.1
+Version: 3.2.2
 Summary: A special kind of ModelAdmin that allows it to be nested within another ModelAdmin
-Home-page: https://github.com/inueni/django-subadmin/
-Author: Mitja Pagon
-Author-email: mitja@inueni.com
+Author-email: Mitja Pagon <mitja@inueni.com>
 License: MIT
-Description: # django-subadmin
-        
-        `django-subadmin` provides a special kind of `ModelAdmin`, called `SubAdmin`, that allows it to be nested within another `ModelAdmin` instance. Similar to django's built-in `InlineModelAdmin`, it allows editing of related objects, but instead of doing it inline, it gives you a full `ModelAdmin` as sub-admin of parent `ModelAdmin`. Like `InlineModelAdmin` it works on models related by `ForeignKey`. Multiple `SubAdmin` instances can be nested within a single `ModelAdmin` or `SubAdmin` allowing for multi-level nesting.
-        
-        ### Suported Python and Django releases
-        
-        Current release of `django-subadmin` is **2.0.1** and it supports Python 3 only and Django versions 2.0 and up (including Django 3.0).
-        
-        There is also a *legacy* **1.9.3** release with support for Python 2.7 and Django versions 1.9, 1.10 and 1.11. This release is **no longer maintained and supported**, but it's made available for legacy applications.
-        
-        #### Verison numbering
-        
-        django-subadmin versions follow Django version numbers. django-subadmin major and minor version numbers equal the minimal compatible django release.
-        
-        ## Installation
-        
-        The easiest and recommended way to install `django-subadmin` is from [PyPI](https://pypi.python.org/pypi/django-subadmin)
-        
-        ```
-        pip install django-subadmin
-        ```
-        
-        You need to add `subadmin` to `INSTALLED_APPS` in your projects `settings.py`, otherwise `django` will not be able to find the necessary templates and template tags.
-        
-        ```
-        # settings.py
-        
-        INSTALLED_APPS = (
-            ...
-            'subadmin',
-            ...
-        )
-        ```
-        
-        ## Example Usage
-        
-        Sometimes things are best explained by an example. Let's say you have two related models.
-        
-        ```python
-        # models.py
-        
-        class MailingList(models.Model):
-            name = models.CharField(max_length=100)
-        
-        
-        class Subscriber(models.Model):
-            mailing_list = models.ForeignKey(MailingList)
-            username = models.CharField(max_length=100)
-        ```
-        
-        If you wish to display only subscribers belonging to a particular mailing list in django admin, your only options is to use `InlineModelAdmin`, which is not very practical when dealing with large number of related objects, plus, you loose all the cool functionality of `ModelAdmin` like searching, filtering, pagination, etc ...
-        
-        This is where `SubAdmin` comes in.
-        
-        ```python
-        # admin.py
-        
-        from subadmin import SubAdmin, RootSubAdmin
-        from .models import MailingList, Subscriber
-        
-        # Instead of admin.ModelAdmin we subclass SubAdmin,
-        # we also set model attribute
-        
-        class SubscriberSubAdmin(SubAdmin): 
-            model = Subscriber
-            list_display = ('username',)
-        
-        
-        # Since this is the top level model admin, which will be registred with admin.site,
-        # we subclass RootSubAdmin and set subadmins attribute
-        
-        class MailingListAdmin(RootSubAdmin):
-            list_display = ('name',)
-        
-            subadmins = [SubscriberSubAdmin]
-            
-        
-        admin.site.register(MailingList, MailingListAdmin)
-        ```
-        
-        With just a few lines of code you get a fully functional `ModelAdmin`, that will automatically pull in just the relevant related objects, based on `ForeignKey` relation between the two models, it will also auto set `ForeignKey` fields for nested relations and exclude them from change form when adding and editing objects on subadmin.
-        
-        
-        ### Caveats
-        
-        In order to properly support unique field validation (see Issue #7), `SubAdmin` will inject a small mixin into the form. This is done in the `get_form` method and if you override this method in your own classes, make sure to call `super()` or `perp_subadmin_form()` directly. See `subadmin` source code for more details.
-        
-        Also, the injected mixin `SubAdminFormMixin` overrides `validate_unique` on the form. If your custom form overrides this method as well, have a look at `subadmin` source code for ways in which it differs from stock `ModelForm` implementation and adjust your code as neccesarry.
-        
-        
-        ### Screenshots
-        
-        ![alt text](https://github.com/inueni/django-subadmin-example/raw/master/screenshots/subadmin_screenshot_1.png?raw=true)
-        
-         `SubAdmin` instances are accesible from edit view of the `ModelAdmin` instance they are nested in. In the screenshot above you can see links to _Subscribers_ and _Messages_ subadmins (marked with red rectangle) for `MailingList` instance _Mailing list 5_.
-        
-        ---
-        
-        ![alt text](https://github.com/inueni/django-subadmin-example/raw/master/screenshots/subadmin_screenshot_2.png?raw=true)
-        
-         `SubAdmin` looks and behaves just like a regular `ModelAdmin`, but looking at breadcrumbs (marked with red rectangle), you can see it is nested within another `ModelAdmin`. Displayed `Subscribers` are limited to those related to `MailingList` instance _Mailing list 5_.
-        
-        ---
-        
-         ![alt text](https://github.com/inueni/django-subadmin-example/raw/master/screenshots/subadmin_screenshot_3.png?raw=true)
-        
-        When adding or editing objects with `SubAdmin`, `ForeignKey` fields to parent instances are removed from the form and automatically set when saving. In this example `mailing_list` field is removed and value is set to parent `MailingList` instance _Mailing list 5_.
-        
-        > If you want to see it in action, or get a more in-depth look at how to set everything up, check out <https://github.com/inueni/django-subadmin-example>.
-        
-        ## Stability
-        
-        `django-subadmin` has evolved from code that has been running on production servers since early 2014 without any issues. The code is provided **as-is** and the developers bear no responsibility for any issues stemming from it's use.
-        
-Keywords: django admin modeladmin foreignkey related field
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/inueni/django-subadmin/
+Project-URL: Bug Tracker, https://github.com/inueni/django-subadmin/issues
+Project-URL: Changelog, https://github.com/inueni/django-subadmin/releases
+Keywords: django,admin,modeladmin,foreignkey,related field
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4
-Requires-Python: >=3
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# django-subadmin
+
+`django-subadmin` provides a special kind of `ModelAdmin`, called `SubAdmin`, that allows it to be nested within another `ModelAdmin` instance. Similar to django's built-in `InlineModelAdmin`, it allows editing of related objects, but instead of doing it inline, it gives you a full `ModelAdmin` as sub-admin of parent `ModelAdmin`. Like `InlineModelAdmin` it works on models related by `ForeignKey`. Multiple `SubAdmin` instances can be nested within a single `ModelAdmin` or `SubAdmin` allowing for multi-level nesting.
+
+### Suported Python and Django releases
+
+Current release of `django-subadmin` supports Django versions 3.2 and up (including Django 4).
+
+#### Verison numbering
+
+django-subadmin versions follow Django version numbers. django-subadmin major and minor version numbers equal the minimal compatible django release.
+
+## Installation
+
+The easiest and recommended way to install `django-subadmin` is from [PyPI](https://pypi.python.org/pypi/django-subadmin)
+
+```
+pip install django-subadmin
+```
+
+You need to add `subadmin` to `INSTALLED_APPS` in your projects `settings.py`, otherwise `django` will not be able to find the necessary templates and template tags.
+
+```
+# settings.py
+
+INSTALLED_APPS = (
+    ...
+    'subadmin',
+    ...
+)
+```
+
+## Example Usage
+
+Sometimes things are best explained by an example. Let's say you have two related models.
+
+```python
+# models.py
+
+class MailingList(models.Model):
+    name = models.CharField(max_length=100)
+
+
+class Subscriber(models.Model):
+    mailing_list = models.ForeignKey(MailingList)
+    username = models.CharField(max_length=100)
+```
+
+If you wish to display only subscribers belonging to a particular mailing list in django admin, your only options is to use `InlineModelAdmin`, which is not very practical when dealing with large number of related objects, plus, you loose all the cool functionality of `ModelAdmin` like searching, filtering, pagination, etc ...
+
+This is where `SubAdmin` comes in.
+
+```python
+# admin.py
+
+from subadmin import SubAdmin, RootSubAdmin
+from .models import MailingList, Subscriber
+
+# Instead of admin.ModelAdmin we subclass SubAdmin,
+# we also set model attribute
+
+class SubscriberSubAdmin(SubAdmin): 
+    model = Subscriber
+    list_display = ('username',)
+
+
+# Since this is the top level model admin, which will be registred with admin.site,
+# we subclass RootSubAdmin and set subadmins attribute
+
+class MailingListAdmin(RootSubAdmin):
+    list_display = ('name',)
+
+    subadmins = [SubscriberSubAdmin]
+    
+
+admin.site.register(MailingList, MailingListAdmin)
+```
+
+With just a few lines of code you get a fully functional `ModelAdmin`, that will automatically pull in just the relevant related objects, based on `ForeignKey` relation between the two models, it will also auto set `ForeignKey` fields for nested relations and exclude them from change form when adding and editing objects on subadmin.
+
+
+### Caveats
+
+In order to properly support unique field validation (see Issue #7), `SubAdmin` will inject a small mixin into the form. This is done in the `get_form` method and if you override this method in your own classes, make sure to call `super()` or `perp_subadmin_form()` directly. See `subadmin` source code for more details.
+
+Also, the injected mixin `SubAdminFormMixin` overrides `validate_unique` on the form. If your custom form overrides this method as well, have a look at `subadmin` source code for ways in which it differs from stock `ModelForm` implementation and adjust your code as neccesarry.
+
+
+### Screenshots
+
+![alt text](https://github.com/inueni/django-subadmin-example/raw/master/screenshots/subadmin_screenshot_1.png?raw=true)
+
+ `SubAdmin` instances are accesible from edit view of the `ModelAdmin` instance they are nested in. In the screenshot above you can see links to _Subscribers_ and _Messages_ subadmins (marked with red rectangle) for `MailingList` instance _Mailing list 5_.
+
+---
+
+![alt text](https://github.com/inueni/django-subadmin-example/raw/master/screenshots/subadmin_screenshot_2.png?raw=true)
+
+ `SubAdmin` looks and behaves just like a regular `ModelAdmin`, but looking at breadcrumbs (marked with red rectangle), you can see it is nested within another `ModelAdmin`. Displayed `Subscribers` are limited to those related to `MailingList` instance _Mailing list 5_.
+
+---
+
+ ![alt text](https://github.com/inueni/django-subadmin-example/raw/master/screenshots/subadmin_screenshot_3.png?raw=true)
+
+When adding or editing objects with `SubAdmin`, `ForeignKey` fields to parent instances are removed from the form and automatically set when saving. In this example `mailing_list` field is removed and value is set to parent `MailingList` instance _Mailing list 5_.
+
+> If you want to see it in action, or get a more in-depth look at how to set everything up, check out <https://github.com/inueni/django-subadmin-example>.
+
+## Stability
+
+`django-subadmin` has evolved from code that has been running on production servers since early 2014 without any issues. The code is provided **as-is** and the developers bear no responsibility for any issues stemming from it's use.
```

### Comparing `django-subadmin-3.2.1/README.md` & `django-subadmin-3.2.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # django-subadmin
 
 `django-subadmin` provides a special kind of `ModelAdmin`, called `SubAdmin`, that allows it to be nested within another `ModelAdmin` instance. Similar to django's built-in `InlineModelAdmin`, it allows editing of related objects, but instead of doing it inline, it gives you a full `ModelAdmin` as sub-admin of parent `ModelAdmin`. Like `InlineModelAdmin` it works on models related by `ForeignKey`. Multiple `SubAdmin` instances can be nested within a single `ModelAdmin` or `SubAdmin` allowing for multi-level nesting.
 
 ### Suported Python and Django releases
 
-Current release of `django-subadmin` is **2.0.1** and it supports Python 3 only and Django versions 2.0 and up (including Django 3.0).
-
-There is also a *legacy* **1.9.3** release with support for Python 2.7 and Django versions 1.9, 1.10 and 1.11. This release is **no longer maintained and supported**, but it's made available for legacy applications.
+Current release of `django-subadmin` supports Django versions 3.2 and up (including Django 4).
 
 #### Verison numbering
 
 django-subadmin versions follow Django version numbers. django-subadmin major and minor version numbers equal the minimal compatible django release.
 
 ## Installation
```

### Comparing `django-subadmin-3.2.1/django_subadmin.egg-info/PKG-INFO` & `django-subadmin-3.2.2/django_subadmin.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,137 +1,136 @@
 Metadata-Version: 2.1
 Name: django-subadmin
-Version: 3.2.1
+Version: 3.2.2
 Summary: A special kind of ModelAdmin that allows it to be nested within another ModelAdmin
-Home-page: https://github.com/inueni/django-subadmin/
-Author: Mitja Pagon
-Author-email: mitja@inueni.com
+Author-email: Mitja Pagon <mitja@inueni.com>
 License: MIT
-Description: # django-subadmin
-        
-        `django-subadmin` provides a special kind of `ModelAdmin`, called `SubAdmin`, that allows it to be nested within another `ModelAdmin` instance. Similar to django's built-in `InlineModelAdmin`, it allows editing of related objects, but instead of doing it inline, it gives you a full `ModelAdmin` as sub-admin of parent `ModelAdmin`. Like `InlineModelAdmin` it works on models related by `ForeignKey`. Multiple `SubAdmin` instances can be nested within a single `ModelAdmin` or `SubAdmin` allowing for multi-level nesting.
-        
-        ### Suported Python and Django releases
-        
-        Current release of `django-subadmin` is **2.0.1** and it supports Python 3 only and Django versions 2.0 and up (including Django 3.0).
-        
-        There is also a *legacy* **1.9.3** release with support for Python 2.7 and Django versions 1.9, 1.10 and 1.11. This release is **no longer maintained and supported**, but it's made available for legacy applications.
-        
-        #### Verison numbering
-        
-        django-subadmin versions follow Django version numbers. django-subadmin major and minor version numbers equal the minimal compatible django release.
-        
-        ## Installation
-        
-        The easiest and recommended way to install `django-subadmin` is from [PyPI](https://pypi.python.org/pypi/django-subadmin)
-        
-        ```
-        pip install django-subadmin
-        ```
-        
-        You need to add `subadmin` to `INSTALLED_APPS` in your projects `settings.py`, otherwise `django` will not be able to find the necessary templates and template tags.
-        
-        ```
-        # settings.py
-        
-        INSTALLED_APPS = (
-            ...
-            'subadmin',
-            ...
-        )
-        ```
-        
-        ## Example Usage
-        
-        Sometimes things are best explained by an example. Let's say you have two related models.
-        
-        ```python
-        # models.py
-        
-        class MailingList(models.Model):
-            name = models.CharField(max_length=100)
-        
-        
-        class Subscriber(models.Model):
-            mailing_list = models.ForeignKey(MailingList)
-            username = models.CharField(max_length=100)
-        ```
-        
-        If you wish to display only subscribers belonging to a particular mailing list in django admin, your only options is to use `InlineModelAdmin`, which is not very practical when dealing with large number of related objects, plus, you loose all the cool functionality of `ModelAdmin` like searching, filtering, pagination, etc ...
-        
-        This is where `SubAdmin` comes in.
-        
-        ```python
-        # admin.py
-        
-        from subadmin import SubAdmin, RootSubAdmin
-        from .models import MailingList, Subscriber
-        
-        # Instead of admin.ModelAdmin we subclass SubAdmin,
-        # we also set model attribute
-        
-        class SubscriberSubAdmin(SubAdmin): 
-            model = Subscriber
-            list_display = ('username',)
-        
-        
-        # Since this is the top level model admin, which will be registred with admin.site,
-        # we subclass RootSubAdmin and set subadmins attribute
-        
-        class MailingListAdmin(RootSubAdmin):
-            list_display = ('name',)
-        
-            subadmins = [SubscriberSubAdmin]
-            
-        
-        admin.site.register(MailingList, MailingListAdmin)
-        ```
-        
-        With just a few lines of code you get a fully functional `ModelAdmin`, that will automatically pull in just the relevant related objects, based on `ForeignKey` relation between the two models, it will also auto set `ForeignKey` fields for nested relations and exclude them from change form when adding and editing objects on subadmin.
-        
-        
-        ### Caveats
-        
-        In order to properly support unique field validation (see Issue #7), `SubAdmin` will inject a small mixin into the form. This is done in the `get_form` method and if you override this method in your own classes, make sure to call `super()` or `perp_subadmin_form()` directly. See `subadmin` source code for more details.
-        
-        Also, the injected mixin `SubAdminFormMixin` overrides `validate_unique` on the form. If your custom form overrides this method as well, have a look at `subadmin` source code for ways in which it differs from stock `ModelForm` implementation and adjust your code as neccesarry.
-        
-        
-        ### Screenshots
-        
-        ![alt text](https://github.com/inueni/django-subadmin-example/raw/master/screenshots/subadmin_screenshot_1.png?raw=true)
-        
-         `SubAdmin` instances are accesible from edit view of the `ModelAdmin` instance they are nested in. In the screenshot above you can see links to _Subscribers_ and _Messages_ subadmins (marked with red rectangle) for `MailingList` instance _Mailing list 5_.
-        
-        ---
-        
-        ![alt text](https://github.com/inueni/django-subadmin-example/raw/master/screenshots/subadmin_screenshot_2.png?raw=true)
-        
-         `SubAdmin` looks and behaves just like a regular `ModelAdmin`, but looking at breadcrumbs (marked with red rectangle), you can see it is nested within another `ModelAdmin`. Displayed `Subscribers` are limited to those related to `MailingList` instance _Mailing list 5_.
-        
-        ---
-        
-         ![alt text](https://github.com/inueni/django-subadmin-example/raw/master/screenshots/subadmin_screenshot_3.png?raw=true)
-        
-        When adding or editing objects with `SubAdmin`, `ForeignKey` fields to parent instances are removed from the form and automatically set when saving. In this example `mailing_list` field is removed and value is set to parent `MailingList` instance _Mailing list 5_.
-        
-        > If you want to see it in action, or get a more in-depth look at how to set everything up, check out <https://github.com/inueni/django-subadmin-example>.
-        
-        ## Stability
-        
-        `django-subadmin` has evolved from code that has been running on production servers since early 2014 without any issues. The code is provided **as-is** and the developers bear no responsibility for any issues stemming from it's use.
-        
-Keywords: django admin modeladmin foreignkey related field
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/inueni/django-subadmin/
+Project-URL: Bug Tracker, https://github.com/inueni/django-subadmin/issues
+Project-URL: Changelog, https://github.com/inueni/django-subadmin/releases
+Keywords: django,admin,modeladmin,foreignkey,related field
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4
-Requires-Python: >=3
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# django-subadmin
+
+`django-subadmin` provides a special kind of `ModelAdmin`, called `SubAdmin`, that allows it to be nested within another `ModelAdmin` instance. Similar to django's built-in `InlineModelAdmin`, it allows editing of related objects, but instead of doing it inline, it gives you a full `ModelAdmin` as sub-admin of parent `ModelAdmin`. Like `InlineModelAdmin` it works on models related by `ForeignKey`. Multiple `SubAdmin` instances can be nested within a single `ModelAdmin` or `SubAdmin` allowing for multi-level nesting.
+
+### Suported Python and Django releases
+
+Current release of `django-subadmin` supports Django versions 3.2 and up (including Django 4).
+
+#### Verison numbering
+
+django-subadmin versions follow Django version numbers. django-subadmin major and minor version numbers equal the minimal compatible django release.
+
+## Installation
+
+The easiest and recommended way to install `django-subadmin` is from [PyPI](https://pypi.python.org/pypi/django-subadmin)
+
+```
+pip install django-subadmin
+```
+
+You need to add `subadmin` to `INSTALLED_APPS` in your projects `settings.py`, otherwise `django` will not be able to find the necessary templates and template tags.
+
+```
+# settings.py
+
+INSTALLED_APPS = (
+    ...
+    'subadmin',
+    ...
+)
+```
+
+## Example Usage
+
+Sometimes things are best explained by an example. Let's say you have two related models.
+
+```python
+# models.py
+
+class MailingList(models.Model):
+    name = models.CharField(max_length=100)
+
+
+class Subscriber(models.Model):
+    mailing_list = models.ForeignKey(MailingList)
+    username = models.CharField(max_length=100)
+```
+
+If you wish to display only subscribers belonging to a particular mailing list in django admin, your only options is to use `InlineModelAdmin`, which is not very practical when dealing with large number of related objects, plus, you loose all the cool functionality of `ModelAdmin` like searching, filtering, pagination, etc ...
+
+This is where `SubAdmin` comes in.
+
+```python
+# admin.py
+
+from subadmin import SubAdmin, RootSubAdmin
+from .models import MailingList, Subscriber
+
+# Instead of admin.ModelAdmin we subclass SubAdmin,
+# we also set model attribute
+
+class SubscriberSubAdmin(SubAdmin): 
+    model = Subscriber
+    list_display = ('username',)
+
+
+# Since this is the top level model admin, which will be registred with admin.site,
+# we subclass RootSubAdmin and set subadmins attribute
+
+class MailingListAdmin(RootSubAdmin):
+    list_display = ('name',)
+
+    subadmins = [SubscriberSubAdmin]
+    
+
+admin.site.register(MailingList, MailingListAdmin)
+```
+
+With just a few lines of code you get a fully functional `ModelAdmin`, that will automatically pull in just the relevant related objects, based on `ForeignKey` relation between the two models, it will also auto set `ForeignKey` fields for nested relations and exclude them from change form when adding and editing objects on subadmin.
+
+
+### Caveats
+
+In order to properly support unique field validation (see Issue #7), `SubAdmin` will inject a small mixin into the form. This is done in the `get_form` method and if you override this method in your own classes, make sure to call `super()` or `perp_subadmin_form()` directly. See `subadmin` source code for more details.
+
+Also, the injected mixin `SubAdminFormMixin` overrides `validate_unique` on the form. If your custom form overrides this method as well, have a look at `subadmin` source code for ways in which it differs from stock `ModelForm` implementation and adjust your code as neccesarry.
+
+
+### Screenshots
+
+![alt text](https://github.com/inueni/django-subadmin-example/raw/master/screenshots/subadmin_screenshot_1.png?raw=true)
+
+ `SubAdmin` instances are accesible from edit view of the `ModelAdmin` instance they are nested in. In the screenshot above you can see links to _Subscribers_ and _Messages_ subadmins (marked with red rectangle) for `MailingList` instance _Mailing list 5_.
+
+---
+
+![alt text](https://github.com/inueni/django-subadmin-example/raw/master/screenshots/subadmin_screenshot_2.png?raw=true)
+
+ `SubAdmin` looks and behaves just like a regular `ModelAdmin`, but looking at breadcrumbs (marked with red rectangle), you can see it is nested within another `ModelAdmin`. Displayed `Subscribers` are limited to those related to `MailingList` instance _Mailing list 5_.
+
+---
+
+ ![alt text](https://github.com/inueni/django-subadmin-example/raw/master/screenshots/subadmin_screenshot_3.png?raw=true)
+
+When adding or editing objects with `SubAdmin`, `ForeignKey` fields to parent instances are removed from the form and automatically set when saving. In this example `mailing_list` field is removed and value is set to parent `MailingList` instance _Mailing list 5_.
+
+> If you want to see it in action, or get a more in-depth look at how to set everything up, check out <https://github.com/inueni/django-subadmin-example>.
+
+## Stability
+
+`django-subadmin` has evolved from code that has been running on production servers since early 2014 without any issues. The code is provided **as-is** and the developers bear no responsibility for any issues stemming from it's use.
```

### Comparing `django-subadmin-3.2.1/django_subadmin.egg-info/SOURCES.txt` & `django-subadmin-3.2.2/django_subadmin.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-CHANGELOG.md
+.gitignore
 LICENSE
-MANIFEST.in
 README.md
-setup.py
+pyproject.toml
+.github/workflows/publish.yml
+.github/workflows/publish_test.yml
 django_subadmin.egg-info/PKG-INFO
 django_subadmin.egg-info/SOURCES.txt
 django_subadmin.egg-info/dependency_links.txt
-django_subadmin.egg-info/not-zip-safe
 django_subadmin.egg-info/top_level.txt
 subadmin/__init__.py
 subadmin/templates/subadmin/breadcrumbs.html
 subadmin/templates/subadmin/change_form.html
 subadmin/templates/subadmin/change_list.html
 subadmin/templates/subadmin/delete_confirmation.html
 subadmin/templates/subadmin/delete_selected_confirmation.html
```

### Comparing `django-subadmin-3.2.1/subadmin/__init__.py` & `django-subadmin-3.2.2/subadmin/__init__.py`

 * *Files identical despite different names*

### Comparing `django-subadmin-3.2.1/subadmin/templates/subadmin/change_form.html` & `django-subadmin-3.2.2/subadmin/templates/subadmin/change_form.html`

 * *Files identical despite different names*

### Comparing `django-subadmin-3.2.1/subadmin/templates/subadmin/change_list.html` & `django-subadmin-3.2.2/subadmin/templates/subadmin/change_list.html`

 * *Files identical despite different names*

### Comparing `django-subadmin-3.2.1/subadmin/templates/subadmin/submit_line.html` & `django-subadmin-3.2.2/subadmin/templates/subadmin/submit_line.html`

 * *Files identical despite different names*

### Comparing `django-subadmin-3.2.1/subadmin/templatetags/subadmin_tags.py` & `django-subadmin-3.2.2/subadmin/templatetags/subadmin_tags.py`

 * *Files identical despite different names*

