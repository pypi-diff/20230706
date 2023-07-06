# Comparing `tmp/curcheck_manager-1.0.0.tar.gz` & `tmp/curcheck_manager-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curcheck_manager-1.0.0.tar", max compression
+gzip compressed data, was "curcheck_manager-1.0.1.tar", max compression
```

## Comparing `curcheck_manager-1.0.0.tar` & `curcheck_manager-1.0.1.tar`

### file list

```diff
@@ -1,65 +1,45 @@
--rw-r--r--   0        0        0       89 2023-02-10 12:25:51.143879 curcheck_manager-1.0.0/curcheck_manager/__main__.py
--rw-r--r--   0        0        0     1027 2023-06-27 11:06:16.235087 curcheck_manager-1.0.0/curcheck_manager/app.py
--rw-r--r--   0        0        0      525 2023-06-24 17:25:28.673796 curcheck_manager-1.0.0/curcheck_manager/config.py
--rw-r--r--   0        0        0      173 2023-06-27 10:54:24.846875 curcheck_manager-1.0.0/curcheck_manager/context.py
--rw-r--r--   0        0        0       78 2023-03-08 07:24:30.482519 curcheck_manager-1.0.0/curcheck_manager/enums.py
--rw-r--r--   0        0        0     1998 2023-06-27 11:10:43.105873 curcheck_manager-1.0.0/curcheck_manager/generator.py
--rw-r--r--   0        0        0        0 2023-02-10 13:56:06.325380 curcheck_manager-1.0.0/curcheck_manager/templates/full/app/__init__.py
--rw-r--r--   0        0        0       53 2023-02-11 09:02:53.545791 curcheck_manager-1.0.0/curcheck_manager/templates/full/app/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-02-10 13:56:38.157436 curcheck_manager-1.0.0/curcheck_manager/templates/full/app/{{ cookiecutter.app_name }}/__init__.py
--rw-r--r--   0        0        0      168 2023-03-05 20:23:17.902824 curcheck_manager-1.0.0/curcheck_manager/templates/full/app/{{ cookiecutter.app_name }}/models.py
--rw-r--r--   0        0        0      253 2023-06-23 08:56:09.139441 curcheck_manager-1.0.0/curcheck_manager/templates/full/app/{{ cookiecutter.app_name }}/views.py
--rw-r--r--   0        0        0       61 2023-02-11 08:05:26.713003 curcheck_manager-1.0.0/curcheck_manager/templates/full/project/cookiecutter.json
--rw-r--r--   0        0        0       28 2023-06-23 09:02:15.026394 curcheck_manager-1.0.0/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/env.env
--rw-r--r--   0        0        0      296 2023-03-05 20:23:17.853251 curcheck_manager-1.0.0/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/main.py
--rw-r--r--   0        0        0      115 2023-03-05 20:23:17.860255 curcheck_manager-1.0.0/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-05 20:23:17.861256 curcheck_manager-1.0.0/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/readme.md
--rw-r--r--   0        0        0        0 2023-03-05 20:23:17.863563 curcheck_manager-1.0.0/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/requirements.txt
--rw-r--r--   0        0        0        0 2023-03-05 20:23:17.872723 curcheck_manager-1.0.0/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/__init__.py
--rw-r--r--   0        0        0      169 2023-03-06 19:32:52.986600 curcheck_manager-1.0.0/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      576 2023-03-06 19:32:52.987595 curcheck_manager-1.0.0/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/__pycache__/app.cpython-310.pyc
--rw-r--r--   0        0        0      314 2023-03-05 20:23:17.871723 curcheck_manager-1.0.0/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/app.py
--rw-r--r--   0        0        0      178 2023-06-23 08:52:42.460993 curcheck_manager-1.0.0/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/apps/__init__.py
--rw-r--r--   0        0        0      358 2023-06-23 09:03:07.407853 curcheck_manager-1.0.0/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/apps/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2023-03-05 20:23:17.904817 curcheck_manager-1.0.0/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/apps/main/__init__.py
--rw-r--r--   0        0        0      179 2023-03-07 18:08:39.524514 curcheck_manager-1.0.0/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/apps/main/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      535 2023-03-07 18:08:39.526513 curcheck_manager-1.0.0/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/apps/main/__pycache__/handlers.cpython-310.pyc
--rw-r--r--   0        0        0      460 2023-03-07 18:21:52.928046 curcheck_manager-1.0.0/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/apps/main/__pycache__/models.cpython-310.pyc
--rw-r--r--   0        0        0      497 2023-06-23 09:03:07.418843 curcheck_manager-1.0.0/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/apps/main/__pycache__/views.cpython-310.pyc
--rw-r--r--   0        0        0      168 2023-03-05 20:23:17.902824 curcheck_manager-1.0.0/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/apps/main/models.py
--rw-r--r--   0        0        0      253 2023-06-23 08:56:09.139441 curcheck_manager-1.0.0/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/apps/main/views.py
--rw-r--r--   0        0        0        0 2023-03-05 20:23:17.944825 curcheck_manager-1.0.0/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/__init__.py
--rw-r--r--   0        0        0      174 2023-03-06 19:32:52.989596 curcheck_manager-1.0.0/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      644 2023-06-23 09:00:43.741842 curcheck_manager-1.0.0/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/__pycache__/bot_app.cpython-310.pyc
--rw-r--r--   0        0        0      793 2023-03-07 18:21:52.788334 curcheck_manager-1.0.0/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/__pycache__/db.cpython-310.pyc
--rw-r--r--   0        0        0      742 2023-06-23 09:03:07.329815 curcheck_manager-1.0.0/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/__pycache__/settings.cpython-310.pyc
--rw-r--r--   0        0        0      423 2023-06-23 08:46:09.993536 curcheck_manager-1.0.0/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/bot_app.py
--rw-r--r--   0        0        0      678 2023-03-05 20:23:17.927821 curcheck_manager-1.0.0/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/db.py
--rw-r--r--   0        0        0      954 2023-03-07 18:21:52.931053 curcheck_manager-1.0.0/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/models/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0      659 2023-03-07 18:21:52.940062 curcheck_manager-1.0.0/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/models/__pycache__/timestamp.cpython-310.pyc
--rw-r--r--   0        0        0      408 2023-03-05 20:23:17.953810 curcheck_manager-1.0.0/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/models/base.py
--rw-r--r--   0        0        0      349 2023-03-05 20:23:17.962097 curcheck_manager-1.0.0/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/models/timestamp.py
--rw-r--r--   0        0        0      298 2023-06-23 09:03:04.582318 curcheck_manager-1.0.0/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/settings.py
--rw-r--r--   0        0        0      289 2023-03-05 20:23:17.942824 curcheck_manager-1.0.0/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/tortoise_orm.py
--rw-r--r--   0        0        0       61 2023-06-24 13:39:32.178390 curcheck_manager-1.0.0/curcheck_manager/templates/mini/project/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-06-27 08:26:16.394398 curcheck_manager-1.0.0/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/env.env
--rw-r--r--   0        0        0      824 2023-06-27 08:37:09.075765 curcheck_manager-1.0.0/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/main.py
--rw-r--r--   0        0        0      451 2023-06-27 08:37:25.751801 curcheck_manager-1.0.0/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/__pycache__/models.cpython-310.pyc
--rw-r--r--   0        0        0      493 2023-06-27 08:37:25.686786 curcheck_manager-1.0.0/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/__pycache__/router.cpython-310.pyc
--rw-r--r--   0        0        0      611 2023-06-27 08:37:24.122976 curcheck_manager-1.0.0/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/core/__pycache__/db.cpython-310.pyc
--rw-r--r--   0        0        0      747 2023-06-27 08:37:24.359974 curcheck_manager-1.0.0/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/core/__pycache__/settings.cpython-310.pyc
--rw-r--r--   0        0        0      368 2023-06-27 08:37:24.356973 curcheck_manager-1.0.0/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/core/__pycache__/tortoise_orm.cpython-310.pyc
--rw-r--r--   0        0        0      337 2023-06-27 08:35:30.708961 curcheck_manager-1.0.0/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/core/db.py
--rw-r--r--   0        0        0      954 2023-03-07 18:21:52.931053 curcheck_manager-1.0.0/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/core/models/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0      659 2023-03-07 18:21:52.940062 curcheck_manager-1.0.0/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/core/models/__pycache__/timestamp.cpython-310.pyc
--rw-r--r--   0        0        0      408 2023-03-05 20:23:17.953810 curcheck_manager-1.0.0/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/core/models/base.py
--rw-r--r--   0        0        0      349 2023-03-05 20:23:17.962097 curcheck_manager-1.0.0/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/core/models/timestamp.py
--rw-r--r--   0        0        0      298 2023-06-27 08:27:46.134954 curcheck_manager-1.0.0/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/core/settings.py
--rw-r--r--   0        0        0      263 2023-06-27 08:31:54.772473 curcheck_manager-1.0.0/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/core/tortoise_orm.py
--rw-r--r--   0        0        0      168 2023-06-27 08:32:07.404070 curcheck_manager-1.0.0/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/models.py
--rw-r--r--   0        0        0      253 2023-06-27 08:28:02.541201 curcheck_manager-1.0.0/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/router.py
--rw-r--r--   0        0        0     1085 2023-06-20 20:30:32.324512 curcheck_manager-1.0.0/LICENSE
--rw-r--r--   0        0        0      582 2023-06-21 20:45:36.411756 curcheck_manager-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       59 2023-06-27 11:11:21.093016 curcheck_manager-1.0.0/README.md
--rw-r--r--   0        0        0     1953 1970-01-01 00:00:00.000000 curcheck_manager-1.0.0/setup.py
--rw-r--r--   0        0        0      839 1970-01-01 00:00:00.000000 curcheck_manager-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       89 2023-02-10 12:25:51.143879 curcheck_manager-1.0.1/curcheck_manager/__main__.py
+-rw-r--r--   0        0        0     1027 2023-06-27 11:06:16.235087 curcheck_manager-1.0.1/curcheck_manager/app.py
+-rw-r--r--   0        0        0      525 2023-06-24 17:25:28.673796 curcheck_manager-1.0.1/curcheck_manager/config.py
+-rw-r--r--   0        0        0      173 2023-06-27 10:54:24.846875 curcheck_manager-1.0.1/curcheck_manager/context.py
+-rw-r--r--   0        0        0       78 2023-03-08 07:24:30.482519 curcheck_manager-1.0.1/curcheck_manager/enums.py
+-rw-r--r--   0        0        0     1998 2023-06-27 11:10:43.105873 curcheck_manager-1.0.1/curcheck_manager/generator.py
+-rw-r--r--   0        0        0        0 2023-02-10 13:56:06.325380 curcheck_manager-1.0.1/curcheck_manager/templates/full/app/__init__.py
+-rw-r--r--   0        0        0       53 2023-02-11 09:02:53.545791 curcheck_manager-1.0.1/curcheck_manager/templates/full/app/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-02-10 13:56:38.157436 curcheck_manager-1.0.1/curcheck_manager/templates/full/app/{{ cookiecutter.app_name }}/__init__.py
+-rw-r--r--   0        0        0      168 2023-03-05 20:23:17.902824 curcheck_manager-1.0.1/curcheck_manager/templates/full/app/{{ cookiecutter.app_name }}/models.py
+-rw-r--r--   0        0        0      253 2023-06-23 08:56:09.139441 curcheck_manager-1.0.1/curcheck_manager/templates/full/app/{{ cookiecutter.app_name }}/views.py
+-rw-r--r--   0        0        0       61 2023-02-11 08:05:26.713003 curcheck_manager-1.0.1/curcheck_manager/templates/full/project/cookiecutter.json
+-rw-r--r--   0        0        0       28 2023-06-23 09:02:15.026394 curcheck_manager-1.0.1/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/env.env
+-rw-r--r--   0        0        0      296 2023-03-05 20:23:17.853251 curcheck_manager-1.0.1/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/main.py
+-rw-r--r--   0        0        0      115 2023-03-05 20:23:17.860255 curcheck_manager-1.0.1/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-05 20:23:17.861256 curcheck_manager-1.0.1/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/readme.md
+-rw-r--r--   0        0        0        0 2023-03-05 20:23:17.863563 curcheck_manager-1.0.1/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/requirements.txt
+-rw-r--r--   0        0        0        0 2023-03-05 20:23:17.872723 curcheck_manager-1.0.1/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/__init__.py
+-rw-r--r--   0        0        0      314 2023-03-05 20:23:17.871723 curcheck_manager-1.0.1/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/app.py
+-rw-r--r--   0        0        0      178 2023-06-23 08:52:42.460993 curcheck_manager-1.0.1/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/apps/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-05 20:23:17.904817 curcheck_manager-1.0.1/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/apps/main/__init__.py
+-rw-r--r--   0        0        0      168 2023-03-05 20:23:17.902824 curcheck_manager-1.0.1/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/apps/main/models.py
+-rw-r--r--   0        0        0      253 2023-06-23 08:56:09.139441 curcheck_manager-1.0.1/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/apps/main/views.py
+-rw-r--r--   0        0        0        0 2023-03-05 20:23:17.944825 curcheck_manager-1.0.1/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/__init__.py
+-rw-r--r--   0        0        0      423 2023-06-23 08:46:09.993536 curcheck_manager-1.0.1/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/bot_app.py
+-rw-r--r--   0        0        0      678 2023-03-05 20:23:17.927821 curcheck_manager-1.0.1/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/db.py
+-rw-r--r--   0        0        0      408 2023-03-05 20:23:17.953810 curcheck_manager-1.0.1/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/models/base.py
+-rw-r--r--   0        0        0      349 2023-03-05 20:23:17.962097 curcheck_manager-1.0.1/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/models/timestamp.py
+-rw-r--r--   0        0        0      298 2023-06-23 09:03:04.582318 curcheck_manager-1.0.1/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/settings.py
+-rw-r--r--   0        0        0      289 2023-03-05 20:23:17.942824 curcheck_manager-1.0.1/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/tortoise_orm.py
+-rw-r--r--   0        0        0       61 2023-06-24 13:39:32.178390 curcheck_manager-1.0.1/curcheck_manager/templates/mini/project/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-06-27 08:26:16.394398 curcheck_manager-1.0.1/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/env.env
+-rw-r--r--   0        0        0      824 2023-06-27 08:37:09.075765 curcheck_manager-1.0.1/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/main.py
+-rw-r--r--   0        0        0      337 2023-06-27 08:35:30.708961 curcheck_manager-1.0.1/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/core/db.py
+-rw-r--r--   0        0        0      408 2023-03-05 20:23:17.953810 curcheck_manager-1.0.1/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/core/models/base.py
+-rw-r--r--   0        0        0      349 2023-03-05 20:23:17.962097 curcheck_manager-1.0.1/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/core/models/timestamp.py
+-rw-r--r--   0        0        0      298 2023-06-27 08:27:46.134954 curcheck_manager-1.0.1/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/core/settings.py
+-rw-r--r--   0        0        0      263 2023-06-27 08:31:54.772473 curcheck_manager-1.0.1/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/core/tortoise_orm.py
+-rw-r--r--   0        0        0      168 2023-06-27 08:32:07.404070 curcheck_manager-1.0.1/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/models.py
+-rw-r--r--   0        0        0      253 2023-06-27 08:28:02.541201 curcheck_manager-1.0.1/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/router.py
+-rw-r--r--   0        0        0     1085 2023-06-27 11:18:05.861249 curcheck_manager-1.0.1/LICENSE
+-rw-r--r--   0        0        0      574 2023-07-06 21:18:02.296903 curcheck_manager-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-06-27 11:11:21.093016 curcheck_manager-1.0.1/README.md
+-rw-r--r--   0        0        0     1945 1970-01-01 00:00:00.000000 curcheck_manager-1.0.1/setup.py
+-rw-r--r--   0        0        0      838 1970-01-01 00:00:00.000000 curcheck_manager-1.0.1/PKG-INFO
```

### Comparing `curcheck_manager-1.0.0/curcheck_manager/app.py` & `curcheck_manager-1.0.1/curcheck_manager/app.py`

 * *Files identical despite different names*

### Comparing `curcheck_manager-1.0.0/curcheck_manager/config.py` & `curcheck_manager-1.0.1/curcheck_manager/config.py`

 * *Files identical despite different names*

### Comparing `curcheck_manager-1.0.0/curcheck_manager/generator.py` & `curcheck_manager-1.0.1/curcheck_manager/generator.py`

 * *Files identical despite different names*

### Comparing `curcheck_manager-1.0.0/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/db.py` & `curcheck_manager-1.0.1/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/db.py`

 * *Files identical despite different names*

### Comparing `curcheck_manager-1.0.0/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/main.py` & `curcheck_manager-1.0.1/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/main.py`

 * *Files identical despite different names*

### Comparing `curcheck_manager-1.0.0/LICENSE` & `curcheck_manager-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `curcheck_manager-1.0.0/pyproject.toml` & `curcheck_manager-1.0.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "curcheck-manager"
-version = "1.0.0"
+version = "1.0.1"
 description = "Managing curcheck projects"
 authors = ["BulatXam <Khamdbulat@yandex.ru>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 pydantic=">=1.10.4"
 click=">=8.1.3"
 cookiecutter=">=2.1.1"
-curcheck=">=1.1.3b"
+curcheck=">=1.1.4"
 changecode=">=0.0.1b"
 loguru=">=0.6.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.2"
 
 [tool.poetry.scripts]
-curcheckmanager = 'curcheck_manager.app:cli'
+curcheck = 'curcheck_manager.app:cli'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `curcheck_manager-1.0.0/setup.py` & `curcheck_manager-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,24 +26,24 @@
 {'': ['*'],
  'curcheck_manager': ['templates/full/project/*', 'templates/mini/project/*']}
 
 install_requires = \
 ['changecode>=0.0.1b',
  'click>=8.1.3',
  'cookiecutter>=2.1.1',
- 'curcheck>=1.1.3b',
+ 'curcheck>=1.1.4',
  'loguru>=0.6.0',
  'pydantic>=1.10.4']
 
 entry_points = \
-{'console_scripts': ['curcheckmanager = curcheck_manager.app:cli']}
+{'console_scripts': ['curcheck = curcheck_manager.app:cli']}
 
 setup_kwargs = {
     'name': 'curcheck-manager',
-    'version': '1.0.0',
+    'version': '1.0.1',
     'description': 'Managing curcheck projects',
     'long_description': '# Curcheck-manager\n___\n\n\nManager for curcheck library\n',
     'author': 'BulatXam',
     'author_email': 'Khamdbulat@yandex.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `curcheck_manager-1.0.0/PKG-INFO` & `curcheck_manager-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curcheck-manager
-Version: 1.0.0
+Version: 1.0.1
 Summary: Managing curcheck projects
 License: MIT
 Author: BulatXam
 Author-email: Khamdbulat@yandex.ru
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: changecode (>=0.0.1b)
 Requires-Dist: click (>=8.1.3)
 Requires-Dist: cookiecutter (>=2.1.1)
-Requires-Dist: curcheck (>=1.1.3b)
+Requires-Dist: curcheck (>=1.1.4)
 Requires-Dist: loguru (>=0.6.0)
 Requires-Dist: pydantic (>=1.10.4)
 Description-Content-Type: text/markdown
 
 # Curcheck-manager
 ___
```

