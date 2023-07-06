# Comparing `tmp/odoo-tools-0.1.7.tar.gz` & `tmp/odoo-tools-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo-tools-0.1.7.tar", last modified: Sat Mar  4 02:23:26 2023, max compression
+gzip compressed data, was "odoo-tools-0.1.9.tar", last modified: Thu Jul  6 20:57:20 2023, max compression
```

## Comparing `odoo-tools-0.1.7.tar` & `odoo-tools-0.1.9.tar`

### file list

```diff
@@ -1,174 +1,189 @@
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.189932 odoo-tools-0.1.7/
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)    35149 2023-03-01 02:33:28.000000 odoo-tools-0.1.7/LICENSE.txt
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     2329 2023-03-04 02:23:26.189932 odoo-tools-0.1.7/PKG-INFO
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1692 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/README.md
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.178932 odoo-tools-0.1.7/odoo_tools/
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1277 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/odoo_tools/__init__.py
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.180932 odoo-tools-0.1.7/odoo_tools/api/
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)        1 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/odoo_tools/api/__init__.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     6488 2023-02-22 18:58:08.000000 odoo-tools-0.1.7/odoo_tools/api/context.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)    10580 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/odoo_tools/api/db.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)    14302 2022-11-09 22:14:46.000000 odoo-tools-0.1.7/odoo_tools/api/environment.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)    13566 2022-11-15 01:05:34.000000 odoo-tools-0.1.7/odoo_tools/api/management.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     4278 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/odoo_tools/api/modules.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)    19949 2022-11-15 01:05:34.000000 odoo-tools-0.1.7/odoo_tools/api/objects.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     2642 2023-03-03 04:28:15.000000 odoo-tools-0.1.7/odoo_tools/api/services.py
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.180932 odoo-tools-0.1.7/odoo_tools/app/
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)       41 2023-03-01 02:33:28.000000 odoo-tools-0.1.7/odoo_tools/app/__init__.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1223 2023-03-01 02:33:28.000000 odoo-tools-0.1.7/odoo_tools/app/application.py
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.181932 odoo-tools-0.1.7/odoo_tools/app/mixins/
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 01:10:03.000000 odoo-tools-0.1.7/odoo_tools/app/mixins/__init__.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1584 2023-03-01 02:33:28.000000 odoo-tools-0.1.7/odoo_tools/app/mixins/app.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     4464 2023-03-01 02:33:28.000000 odoo-tools-0.1.7/odoo_tools/app/mixins/dispatchers.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     8226 2023-03-01 02:33:28.000000 odoo-tools-0.1.7/odoo_tools/app/mixins/http.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)    18545 2023-03-01 02:33:28.000000 odoo-tools-0.1.7/odoo_tools/app/mixins/request.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     2606 2023-03-01 02:33:28.000000 odoo-tools-0.1.7/odoo_tools/app/mixins/routers.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     7323 2023-03-01 02:33:28.000000 odoo-tools-0.1.7/odoo_tools/app/mixins/routing.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1243 2023-03-01 02:33:28.000000 odoo-tools-0.1.7/odoo_tools/app/mixins/sessions.py
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.181932 odoo-tools-0.1.7/odoo_tools/app/plugins/
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)       43 2023-03-01 02:33:28.000000 odoo-tools-0.1.7/odoo_tools/app/plugins/__init__.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     5418 2023-03-01 02:33:28.000000 odoo-tools-0.1.7/odoo_tools/app/plugins/base.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     6590 2023-03-01 02:33:28.000000 odoo-tools-0.1.7/odoo_tools/app/plugins/logging.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)      458 2023-03-01 02:33:28.000000 odoo-tools-0.1.7/odoo_tools/app/utils.py
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.181932 odoo-tools-0.1.7/odoo_tools/cli/
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)        0 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/odoo_tools/cli/__init__.py
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.182932 odoo-tools-0.1.7/odoo_tools/cli/click/
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)        1 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/odoo_tools/cli/click/__init__.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1052 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/odoo_tools/cli/click/config.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     2513 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/odoo_tools/cli/click/db.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1951 2023-03-01 02:33:28.000000 odoo-tools-0.1.7/odoo_tools/cli/click/entrypoint.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)      189 2022-11-10 22:29:45.000000 odoo-tools-0.1.7/odoo_tools/cli/click/gen.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     4079 2023-03-02 00:04:03.000000 odoo-tools-0.1.7/odoo_tools/cli/click/manage.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     7125 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/odoo_tools/cli/click/module.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1858 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/odoo_tools/cli/click/path.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)      417 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/odoo_tools/cli/click/platform.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     2546 2023-03-04 02:04:06.000000 odoo-tools-0.1.7/odoo_tools/cli/click/services.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)      936 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/odoo_tools/cli/click/shell.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     5288 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/odoo_tools/cli/click/users.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)      690 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/odoo_tools/cli/click/utils.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)      746 2022-11-09 22:17:33.000000 odoo-tools-0.1.7/odoo_tools/cli/odot.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)      983 2022-11-15 01:05:35.000000 odoo-tools-0.1.7/odoo_tools/cli/registry.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     2590 2023-02-22 18:58:08.000000 odoo-tools-0.1.7/odoo_tools/compat.py
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.183932 odoo-tools-0.1.7/odoo_tools/configuration/
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)        0 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/odoo_tools/configuration/__init__.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     3395 2023-03-03 20:04:34.000000 odoo-tools-0.1.7/odoo_tools/configuration/git.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     2149 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/odoo_tools/configuration/misc.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     7795 2022-11-15 01:05:34.000000 odoo-tools-0.1.7/odoo_tools/configuration/odoo.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)      656 2022-11-10 21:24:35.000000 odoo-tools-0.1.7/odoo_tools/configuration/pip.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1173 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/odoo_tools/db.py
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.183932 odoo-tools-0.1.7/odoo_tools/docker/
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)        0 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/odoo_tools/docker/__init__.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1397 2023-02-22 18:58:08.000000 odoo-tools-0.1.7/odoo_tools/docker/sudo_entrypoint.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     9365 2023-01-28 00:56:10.000000 odoo-tools-0.1.7/odoo_tools/docker/user_entrypoint.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)      486 2023-01-19 22:31:18.000000 odoo-tools-0.1.7/odoo_tools/entrypoints.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     7588 2023-02-22 18:58:08.000000 odoo-tools-0.1.7/odoo_tools/env.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)      230 2022-11-09 22:14:46.000000 odoo-tools-0.1.7/odoo_tools/exceptions.py
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.183932 odoo-tools-0.1.7/odoo_tools/modules/
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)      172 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/odoo_tools/modules/__init__.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1834 2023-03-02 00:04:02.000000 odoo-tools-0.1.7/odoo_tools/modules/assets.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     2957 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/odoo_tools/modules/render.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)    11041 2022-11-09 22:14:46.000000 odoo-tools-0.1.7/odoo_tools/modules/search.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)    10854 2023-03-01 22:15:21.000000 odoo-tools-0.1.7/odoo_tools/modules/translate.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)      343 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/odoo_tools/odoo.py
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.176932 odoo-tools-0.1.7/odoo_tools/overlays/
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.176932 odoo-tools-0.1.7/odoo_tools/overlays/common/
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.183932 odoo-tools-0.1.7/odoo_tools/overlays/common/odoo/
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.176932 odoo-tools-0.1.7/odoo_tools/overlays/common/odoo/addons/
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.176932 odoo-tools-0.1.7/odoo_tools/overlays/common/odoo/addons/base/
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.184932 odoo-tools-0.1.7/odoo_tools/overlays/common/odoo/addons/base/models/
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)      136 2023-03-01 02:33:28.000000 odoo-tools-0.1.7/odoo_tools/overlays/common/odoo/addons/base/models/ir_http.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     7883 2023-03-01 02:33:28.000000 odoo-tools-0.1.7/odoo_tools/overlays/common/odoo/http.py
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.184932 odoo-tools-0.1.7/odoo_tools/overlays/common/odoo/modules/
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)       36 2023-03-01 02:33:28.000000 odoo-tools-0.1.7/odoo_tools/overlays/common/odoo/modules/module.py
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.176932 odoo-tools-0.1.7/odoo_tools/overlays/v14/
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.184932 odoo-tools-0.1.7/odoo_tools/overlays/v14/odoo/
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.176932 odoo-tools-0.1.7/odoo_tools/overlays/v14/odoo/addons/
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.176932 odoo-tools-0.1.7/odoo_tools/overlays/v14/odoo/addons/base/
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.184932 odoo-tools-0.1.7/odoo_tools/overlays/v14/odoo/addons/base/models/
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)      245 2023-03-01 02:33:28.000000 odoo-tools-0.1.7/odoo_tools/overlays/v14/odoo/addons/base/models/ir_http.py
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.176932 odoo-tools-0.1.7/odoo_tools/overlays/v14/odoo/addons/http_routing/
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.184932 odoo-tools-0.1.7/odoo_tools/overlays/v14/odoo/addons/http_routing/models/
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     4178 2023-03-01 02:33:28.000000 odoo-tools-0.1.7/odoo_tools/overlays/v14/odoo/addons/http_routing/models/ir_http.py
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.176932 odoo-tools-0.1.7/odoo_tools/overlays/v14/odoo/addons/website/
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.184932 odoo-tools-0.1.7/odoo_tools/overlays/v14/odoo/addons/website/models/
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)      549 2023-03-01 02:33:28.000000 odoo-tools-0.1.7/odoo_tools/overlays/v14/odoo/addons/website/models/ir_http.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1824 2023-03-01 02:33:28.000000 odoo-tools-0.1.7/odoo_tools/overlays/v14/odoo/addons/website/models/ir_qweb.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)       90 2023-03-01 02:33:28.000000 odoo-tools-0.1.7/odoo_tools/overlays/v14/odoo/http.py
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.176932 odoo-tools-0.1.7/odoo_tools/overlays/v15/
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.184932 odoo-tools-0.1.7/odoo_tools/overlays/v15/odoo/
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.177932 odoo-tools-0.1.7/odoo_tools/overlays/v15/odoo/addons/
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.176932 odoo-tools-0.1.7/odoo_tools/overlays/v15/odoo/addons/base/
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.184932 odoo-tools-0.1.7/odoo_tools/overlays/v15/odoo/addons/base/models/
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)      245 2023-03-01 02:33:28.000000 odoo-tools-0.1.7/odoo_tools/overlays/v15/odoo/addons/base/models/ir_http.py
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.177932 odoo-tools-0.1.7/odoo_tools/overlays/v15/odoo/addons/http_routing/
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.184932 odoo-tools-0.1.7/odoo_tools/overlays/v15/odoo/addons/http_routing/models/
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     4120 2023-03-01 02:33:28.000000 odoo-tools-0.1.7/odoo_tools/overlays/v15/odoo/addons/http_routing/models/ir_http.py
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.177932 odoo-tools-0.1.7/odoo_tools/overlays/v15/odoo/addons/website/
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.185932 odoo-tools-0.1.7/odoo_tools/overlays/v15/odoo/addons/website/models/
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)      549 2023-03-01 02:33:28.000000 odoo-tools-0.1.7/odoo_tools/overlays/v15/odoo/addons/website/models/ir_http.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1824 2023-03-01 02:33:28.000000 odoo-tools-0.1.7/odoo_tools/overlays/v15/odoo/addons/website/models/ir_qweb.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)       90 2023-03-01 02:33:28.000000 odoo-tools-0.1.7/odoo_tools/overlays/v15/odoo/http.py
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.185932 odoo-tools-0.1.7/odoo_tools/packages/
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)       21 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/odoo_tools/packages/map-15.toml
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)       21 2022-11-09 22:16:35.000000 odoo-tools-0.1.7/odoo_tools/packages/map-16.toml
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     2268 2023-03-01 02:33:28.000000 odoo-tools-0.1.7/odoo_tools/patch.py
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.185932 odoo-tools-0.1.7/odoo_tools/requirements/
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)      658 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/odoo_tools/requirements/requirements-10.0.txt
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)      907 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/odoo_tools/requirements/requirements-11.0.txt
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)      980 2023-02-02 00:23:13.000000 odoo-tools-0.1.7/odoo_tools/requirements/requirements-12.0.txt
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)      910 2023-02-02 00:23:13.000000 odoo-tools-0.1.7/odoo_tools/requirements/requirements-13.0.txt
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1019 2023-02-02 00:23:13.000000 odoo-tools-0.1.7/odoo_tools/requirements/requirements-14.0.txt
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1474 2023-02-02 00:23:13.000000 odoo-tools-0.1.7/odoo_tools/requirements/requirements-15.0.txt
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1620 2023-02-02 00:23:13.000000 odoo-tools-0.1.7/odoo_tools/requirements/requirements-16.0.txt
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)      679 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/odoo_tools/requirements/requirements-9.0.txt
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.186932 odoo-tools-0.1.7/odoo_tools/services/
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)        0 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/odoo_tools/services/__init__.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     3205 2023-03-02 23:33:00.000000 odoo-tools-0.1.7/odoo_tools/services/fields.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1042 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/odoo_tools/services/models.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)    11250 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/odoo_tools/services/objects.py
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.186932 odoo-tools-0.1.7/odoo_tools/utilities/
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)        0 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/odoo_tools/utilities/__init__.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     4568 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/odoo_tools/utilities/config.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)      896 2022-11-09 22:14:46.000000 odoo-tools-0.1.7/odoo_tools/utilities/loaders.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)      965 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/odoo_tools/utilities/logging.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)        1 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/odoo_tools/utilities/modules.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     2223 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/odoo_tools/utilities/requirements.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     4921 2023-02-22 18:58:08.000000 odoo-tools-0.1.7/odoo_tools/utils.py
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.179932 odoo-tools-0.1.7/odoo_tools.egg-info/
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     2329 2023-03-04 02:23:26.000000 odoo-tools-0.1.7/odoo_tools.egg-info/PKG-INFO
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     4133 2023-03-04 02:23:26.000000 odoo-tools-0.1.7/odoo_tools.egg-info/SOURCES.txt
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)        1 2023-03-04 02:23:26.000000 odoo-tools-0.1.7/odoo_tools.egg-info/dependency_links.txt
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)      633 2023-03-04 02:23:26.000000 odoo-tools-0.1.7/odoo_tools.egg-info/entry_points.txt
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)      275 2023-03-04 02:23:26.000000 odoo-tools-0.1.7/odoo_tools.egg-info/requires.txt
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)       17 2023-03-04 02:23:26.000000 odoo-tools-0.1.7/odoo_tools.egg-info/top_level.txt
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)      202 2023-03-04 02:23:26.189932 odoo-tools-0.1.7/setup.cfg
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     3012 2023-03-04 01:23:16.000000 odoo-tools-0.1.7/setup.py
-drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-03-04 02:23:26.189932 odoo-tools-0.1.7/tests/
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)        0 2023-02-22 23:23:59.000000 odoo-tools-0.1.7/tests/__init__.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     2599 2023-02-22 18:59:48.000000 odoo-tools-0.1.7/tests/fixtures.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)      771 2022-11-15 01:05:37.000000 odoo-tools-0.1.7/tests/test_api_context.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     4623 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/tests/test_api_db.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     4398 2022-11-15 01:05:34.000000 odoo-tools-0.1.7/tests/test_api_objects.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1718 2022-11-15 01:05:35.000000 odoo-tools-0.1.7/tests/test_api_services.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)    31647 2022-11-15 01:05:35.000000 odoo-tools-0.1.7/tests/test_cli.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1937 2022-11-15 01:05:35.000000 odoo-tools-0.1.7/tests/test_command_registry.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1969 2023-02-22 18:58:08.000000 odoo-tools-0.1.7/tests/test_compat.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     4220 2022-11-15 01:05:37.000000 odoo-tools-0.1.7/tests/test_config_utilities.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     3153 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/tests/test_configuration_git.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     8745 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/tests/test_db.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)      959 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/tests/test_entrypoint.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     6738 2022-11-11 02:55:35.000000 odoo-tools-0.1.7/tests/test_env.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     3494 2023-02-22 18:58:08.000000 odoo-tools-0.1.7/tests/test_envvars.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1304 2022-11-15 01:05:33.000000 odoo-tools-0.1.7/tests/test_manage.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     5425 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/tests/test_manifest.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)      835 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/tests/test_module_search.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     2287 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/tests/test_modules.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)    13320 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/tests/test_odoo_entrypoint.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     2678 2022-11-15 01:05:37.000000 odoo-tools-0.1.7/tests/test_odoo_git.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     2869 2022-11-15 01:05:37.000000 odoo-tools-0.1.7/tests/test_odoo_release.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1046 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/tests/test_rendering_description.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1693 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/tests/test_requirements.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     3217 2023-03-03 04:44:35.000000 odoo-tools-0.1.7/tests/test_services.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)      403 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/tests/test_trans.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     3908 2023-02-22 18:58:08.000000 odoo-tools-0.1.7/tests/test_utils.py
--rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1384 2022-09-26 19:08:21.000000 odoo-tools-0.1.7/tests/utils.py
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.443339 odoo-tools-0.1.9/
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)    35149 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/LICENSE.txt
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     2329 2023-07-06 20:57:20.443339 odoo-tools-0.1.9/PKG-INFO
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1692 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/README.md
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.411339 odoo-tools-0.1.9/odoo_tools/
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1277 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/odoo_tools/__init__.py
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.414339 odoo-tools-0.1.9/odoo_tools/api/
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)        1 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/odoo_tools/api/__init__.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     6488 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/api/context.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)    10580 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/odoo_tools/api/db.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)    14318 2023-07-06 20:21:41.000000 odoo-tools-0.1.9/odoo_tools/api/environment.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)    13566 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/api/management.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     4278 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/odoo_tools/api/modules.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)    19949 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/api/objects.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     2642 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/api/services.py
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.414339 odoo-tools-0.1.9/odoo_tools/app/
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)       41 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/app/__init__.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1223 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/app/application.py
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.416339 odoo-tools-0.1.9/odoo_tools/app/mixins/
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)        0 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/app/mixins/__init__.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1584 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/app/mixins/app.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     4464 2023-07-06 14:00:13.000000 odoo-tools-0.1.9/odoo_tools/app/mixins/dispatchers.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     8226 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/app/mixins/http.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)    18545 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/app/mixins/request.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     2606 2023-07-06 14:00:13.000000 odoo-tools-0.1.9/odoo_tools/app/mixins/routers.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     7323 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/app/mixins/routing.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1243 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/app/mixins/sessions.py
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.416339 odoo-tools-0.1.9/odoo_tools/app/plugins/
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)       43 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/app/plugins/__init__.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     5418 2023-07-06 19:34:29.000000 odoo-tools-0.1.9/odoo_tools/app/plugins/base.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     6590 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/app/plugins/logging.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      458 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/app/utils.py
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.417339 odoo-tools-0.1.9/odoo_tools/cli/
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)        0 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/odoo_tools/cli/__init__.py
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.420339 odoo-tools-0.1.9/odoo_tools/cli/click/
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)        1 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/odoo_tools/cli/click/__init__.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1052 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/odoo_tools/cli/click/config.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     2513 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/odoo_tools/cli/click/db.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1951 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/cli/click/entrypoint.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      189 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/cli/click/gen.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     4079 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/cli/click/manage.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     7431 2023-07-06 20:21:41.000000 odoo-tools-0.1.9/odoo_tools/cli/click/module.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1858 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/odoo_tools/cli/click/path.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      433 2023-07-06 20:21:41.000000 odoo-tools-0.1.9/odoo_tools/cli/click/platform.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     2546 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/cli/click/services.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      936 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/odoo_tools/cli/click/shell.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     5288 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/odoo_tools/cli/click/users.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      690 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/odoo_tools/cli/click/utils.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      746 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/cli/odot.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      983 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/cli/registry.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     2590 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/compat.py
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.420339 odoo-tools-0.1.9/odoo_tools/configuration/
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)        0 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/odoo_tools/configuration/__init__.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     3395 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/configuration/git.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     2149 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/odoo_tools/configuration/misc.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     7823 2023-07-06 20:34:39.000000 odoo-tools-0.1.9/odoo_tools/configuration/odoo.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      656 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/configuration/pip.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1173 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/odoo_tools/db.py
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.424339 odoo-tools-0.1.9/odoo_tools/docker/
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)        0 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/odoo_tools/docker/__init__.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1397 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/docker/sudo_entrypoint.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     9365 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/docker/user_entrypoint.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      486 2023-01-19 22:31:18.000000 odoo-tools-0.1.9/odoo_tools/entrypoints.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     7588 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/env.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      230 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/exceptions.py
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.425339 odoo-tools-0.1.9/odoo_tools/modules/
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      172 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/odoo_tools/modules/__init__.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1834 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/modules/assets.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     2957 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/odoo_tools/modules/render.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)    11041 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/modules/search.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)    10854 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/modules/translate.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      343 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/odoo_tools/odoo.py
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.408339 odoo-tools-0.1.9/odoo_tools/overlays/
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.407339 odoo-tools-0.1.9/odoo_tools/overlays/common/
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.425339 odoo-tools-0.1.9/odoo_tools/overlays/common/odoo/
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.425339 odoo-tools-0.1.9/odoo_tools/overlays/common/odoo/__pycache__/
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     6504 2023-03-31 04:55:09.000000 odoo-tools-0.1.9/odoo_tools/overlays/common/odoo/__pycache__/http.cpython-38.pyc
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.407339 odoo-tools-0.1.9/odoo_tools/overlays/common/odoo/addons/
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.407339 odoo-tools-0.1.9/odoo_tools/overlays/common/odoo/addons/base/
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.425339 odoo-tools-0.1.9/odoo_tools/overlays/common/odoo/addons/base/models/
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.426339 odoo-tools-0.1.9/odoo_tools/overlays/common/odoo/addons/base/models/__pycache__/
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      367 2023-03-30 22:40:06.000000 odoo-tools-0.1.9/odoo_tools/overlays/common/odoo/addons/base/models/__pycache__/ir_http.cpython-38.pyc
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      136 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/overlays/common/odoo/addons/base/models/ir_http.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     7883 2023-07-06 14:00:13.000000 odoo-tools-0.1.9/odoo_tools/overlays/common/odoo/http.py
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.426339 odoo-tools-0.1.9/odoo_tools/overlays/common/odoo/modules/
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.426339 odoo-tools-0.1.9/odoo_tools/overlays/common/odoo/modules/__pycache__/
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      284 2023-03-30 22:39:58.000000 odoo-tools-0.1.9/odoo_tools/overlays/common/odoo/modules/__pycache__/module.cpython-38.pyc
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)       36 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/overlays/common/odoo/modules/module.py
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.408339 odoo-tools-0.1.9/odoo_tools/overlays/v14/
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.426339 odoo-tools-0.1.9/odoo_tools/overlays/v14/odoo/
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.408339 odoo-tools-0.1.9/odoo_tools/overlays/v14/odoo/addons/
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.408339 odoo-tools-0.1.9/odoo_tools/overlays/v14/odoo/addons/base/
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.427339 odoo-tools-0.1.9/odoo_tools/overlays/v14/odoo/addons/base/models/
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      245 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/overlays/v14/odoo/addons/base/models/ir_http.py
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.408339 odoo-tools-0.1.9/odoo_tools/overlays/v14/odoo/addons/http_routing/
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.427339 odoo-tools-0.1.9/odoo_tools/overlays/v14/odoo/addons/http_routing/models/
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     4178 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/overlays/v14/odoo/addons/http_routing/models/ir_http.py
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.408339 odoo-tools-0.1.9/odoo_tools/overlays/v14/odoo/addons/website/
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.427339 odoo-tools-0.1.9/odoo_tools/overlays/v14/odoo/addons/website/models/
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      549 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/overlays/v14/odoo/addons/website/models/ir_http.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1824 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/overlays/v14/odoo/addons/website/models/ir_qweb.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)       90 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/overlays/v14/odoo/http.py
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.408339 odoo-tools-0.1.9/odoo_tools/overlays/v15/
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.428339 odoo-tools-0.1.9/odoo_tools/overlays/v15/odoo/
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.428339 odoo-tools-0.1.9/odoo_tools/overlays/v15/odoo/__pycache__/
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      220 2023-03-30 22:39:58.000000 odoo-tools-0.1.9/odoo_tools/overlays/v15/odoo/__pycache__/http.cpython-38.pyc
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.409339 odoo-tools-0.1.9/odoo_tools/overlays/v15/odoo/addons/
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.408339 odoo-tools-0.1.9/odoo_tools/overlays/v15/odoo/addons/base/
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.428339 odoo-tools-0.1.9/odoo_tools/overlays/v15/odoo/addons/base/models/
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.428339 odoo-tools-0.1.9/odoo_tools/overlays/v15/odoo/addons/base/models/__pycache__/
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      505 2023-03-30 22:40:06.000000 odoo-tools-0.1.9/odoo_tools/overlays/v15/odoo/addons/base/models/__pycache__/ir_http.cpython-38.pyc
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      245 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/overlays/v15/odoo/addons/base/models/ir_http.py
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.409339 odoo-tools-0.1.9/odoo_tools/overlays/v15/odoo/addons/http_routing/
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.429340 odoo-tools-0.1.9/odoo_tools/overlays/v15/odoo/addons/http_routing/models/
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.429340 odoo-tools-0.1.9/odoo_tools/overlays/v15/odoo/addons/http_routing/models/__pycache__/
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     2190 2023-03-30 22:40:06.000000 odoo-tools-0.1.9/odoo_tools/overlays/v15/odoo/addons/http_routing/models/__pycache__/ir_http.cpython-38.pyc
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     4120 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/overlays/v15/odoo/addons/http_routing/models/ir_http.py
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.409339 odoo-tools-0.1.9/odoo_tools/overlays/v15/odoo/addons/website/
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.429340 odoo-tools-0.1.9/odoo_tools/overlays/v15/odoo/addons/website/models/
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.430339 odoo-tools-0.1.9/odoo_tools/overlays/v15/odoo/addons/website/models/__pycache__/
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      685 2023-03-30 22:40:07.000000 odoo-tools-0.1.9/odoo_tools/overlays/v15/odoo/addons/website/models/__pycache__/ir_http.cpython-38.pyc
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1466 2023-03-30 22:40:07.000000 odoo-tools-0.1.9/odoo_tools/overlays/v15/odoo/addons/website/models/__pycache__/ir_qweb.cpython-38.pyc
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      549 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/overlays/v15/odoo/addons/website/models/ir_http.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1824 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/overlays/v15/odoo/addons/website/models/ir_qweb.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)       90 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/overlays/v15/odoo/http.py
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.430339 odoo-tools-0.1.9/odoo_tools/packages/
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)       21 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/odoo_tools/packages/map-15.toml
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)       21 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/packages/map-16.toml
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     2268 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/patch.py
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.435339 odoo-tools-0.1.9/odoo_tools/requirements/
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      658 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/odoo_tools/requirements/requirements-10.0.txt
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      907 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/odoo_tools/requirements/requirements-11.0.txt
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      980 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/requirements/requirements-12.0.txt
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      896 2023-07-06 20:34:55.000000 odoo-tools-0.1.9/odoo_tools/requirements/requirements-13.0.txt
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1019 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/requirements/requirements-14.0.txt
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1474 2023-07-06 20:21:41.000000 odoo-tools-0.1.9/odoo_tools/requirements/requirements-15.0.txt
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1620 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/requirements/requirements-16.0.txt
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      679 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/odoo_tools/requirements/requirements-9.0.txt
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.436339 odoo-tools-0.1.9/odoo_tools/services/
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)        0 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/odoo_tools/services/__init__.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     3205 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/services/fields.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1042 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/odoo_tools/services/models.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)    11250 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/odoo_tools/services/objects.py
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.437339 odoo-tools-0.1.9/odoo_tools/utilities/
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)        0 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/odoo_tools/utilities/__init__.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     4568 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/odoo_tools/utilities/config.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      896 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/utilities/loaders.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      965 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/odoo_tools/utilities/logging.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)        1 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/odoo_tools/utilities/modules.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     2223 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/odoo_tools/utilities/requirements.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     4921 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/odoo_tools/utils.py
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.412339 odoo-tools-0.1.9/odoo_tools.egg-info/
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     2329 2023-07-06 20:57:20.000000 odoo-tools-0.1.9/odoo_tools.egg-info/PKG-INFO
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     4764 2023-07-06 20:57:20.000000 odoo-tools-0.1.9/odoo_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)        1 2023-07-06 20:57:20.000000 odoo-tools-0.1.9/odoo_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      633 2023-07-06 20:57:20.000000 odoo-tools-0.1.9/odoo_tools.egg-info/entry_points.txt
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      275 2023-07-06 20:57:20.000000 odoo-tools-0.1.9/odoo_tools.egg-info/requires.txt
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)       17 2023-07-06 20:57:20.000000 odoo-tools-0.1.9/odoo_tools.egg-info/top_level.txt
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      202 2023-07-06 20:57:20.444339 odoo-tools-0.1.9/setup.cfg
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     3012 2023-07-06 20:50:21.000000 odoo-tools-0.1.9/setup.py
+drwxr-xr-x   0 llacroix  (1000) llacroix  (1000)        0 2023-07-06 20:57:20.443339 odoo-tools-0.1.9/tests/
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)        0 2023-02-22 23:23:59.000000 odoo-tools-0.1.9/tests/__init__.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     2599 2023-07-06 20:21:41.000000 odoo-tools-0.1.9/tests/fixtures.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      771 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/tests/test_api_context.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     4623 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/tests/test_api_db.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     4398 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/tests/test_api_objects.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1718 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/tests/test_api_services.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)    31647 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/tests/test_cli.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1937 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/tests/test_command_registry.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1969 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/tests/test_compat.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     4220 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/tests/test_config_utilities.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     3153 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/tests/test_configuration_git.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     8745 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/tests/test_db.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      959 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/tests/test_entrypoint.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     7107 2023-07-06 20:21:41.000000 odoo-tools-0.1.9/tests/test_env.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     3494 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/tests/test_envvars.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1304 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/tests/test_manage.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     5425 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/tests/test_manifest.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      835 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/tests/test_module_search.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     2287 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/tests/test_modules.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)    13320 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/tests/test_odoo_entrypoint.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     2678 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/tests/test_odoo_git.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     2869 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/tests/test_odoo_release.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1046 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/tests/test_rendering_description.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1693 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/tests/test_requirements.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     3217 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/tests/test_services.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)      403 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/tests/test_trans.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     3908 2023-03-07 00:04:42.000000 odoo-tools-0.1.9/tests/test_utils.py
+-rw-r--r--   0 llacroix  (1000) llacroix  (1000)     1384 2022-09-26 19:08:21.000000 odoo-tools-0.1.9/tests/utils.py
```

### Comparing `odoo-tools-0.1.7/LICENSE.txt` & `odoo-tools-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/PKG-INFO` & `odoo-tools-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-tools
-Version: 0.1.7
+Version: 0.1.9
 Summary: Odoo Tools
 Home-page: https://odoo-tools.readthedocs.io
 Author: Loïc Faure-Lacroix <lamerstar@gmail.com>
 Author-email: lamerstar@gmail.com
 License: GPL3
 Project-URL: Source, https://github.com/llacroix/odoo-tools
 Project-URL: Documentation, https://odoo-tools.readthedocs.io
```

### Comparing `odoo-tools-0.1.7/README.md` & `odoo-tools-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/__init__.py` & `odoo-tools-0.1.9/odoo_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/api/context.py` & `odoo-tools-0.1.9/odoo_tools/api/context.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/api/db.py` & `odoo-tools-0.1.9/odoo_tools/api/db.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/api/environment.py` & `odoo-tools-0.1.9/odoo_tools/api/environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,17 +243,17 @@
                 addons.
         """
         try:
             with self.config(readonly=True) as config:
                 paths = config.get('options', 'addons_path')
 
             config_paths = set(
-                Path(path)
+                Path(path.strip())
                 for path in paths.split(',')
-                if path
+                if path.strip()
             )
 
             if len(config_paths) > 0 and not self.context.force_addons_lookup:
                 return config_paths
 
         except Exception:
             config_paths = set()
```

### Comparing `odoo-tools-0.1.7/odoo_tools/api/management.py` & `odoo-tools-0.1.9/odoo_tools/api/management.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/api/modules.py` & `odoo-tools-0.1.9/odoo_tools/api/modules.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/api/objects.py` & `odoo-tools-0.1.9/odoo_tools/api/objects.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/api/services.py` & `odoo-tools-0.1.9/odoo_tools/api/services.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/app/application.py` & `odoo-tools-0.1.9/odoo_tools/app/application.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/app/mixins/app.py` & `odoo-tools-0.1.9/odoo_tools/app/mixins/app.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/app/mixins/dispatchers.py` & `odoo-tools-0.1.9/odoo_tools/app/mixins/dispatchers.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/app/mixins/http.py` & `odoo-tools-0.1.9/odoo_tools/app/mixins/http.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/app/mixins/request.py` & `odoo-tools-0.1.9/odoo_tools/app/mixins/request.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/app/mixins/routers.py` & `odoo-tools-0.1.9/odoo_tools/app/mixins/routers.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/app/mixins/routing.py` & `odoo-tools-0.1.9/odoo_tools/app/mixins/routing.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/app/mixins/sessions.py` & `odoo-tools-0.1.9/odoo_tools/app/mixins/sessions.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/app/plugins/base.py` & `odoo-tools-0.1.9/odoo_tools/app/plugins/base.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/app/plugins/logging.py` & `odoo-tools-0.1.9/odoo_tools/app/plugins/logging.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/cli/click/config.py` & `odoo-tools-0.1.9/odoo_tools/cli/click/config.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/cli/click/db.py` & `odoo-tools-0.1.9/odoo_tools/cli/click/db.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/cli/click/entrypoint.py` & `odoo-tools-0.1.9/odoo_tools/cli/click/entrypoint.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/cli/click/manage.py` & `odoo-tools-0.1.9/odoo_tools/cli/click/manage.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/cli/click/module.py` & `odoo-tools-0.1.9/odoo_tools/cli/click/module.py`

 * *Files 3% similar despite different names*

```diff
@@ -193,38 +193,45 @@
 @click.option(
     '--auto',
     help="Include auto installed modules",
     is_flag=True
 )
 @click.option(
     '--include-modules',
-    help="Remove logs and warnings.",
+    help="Include dependencies that aren't in the addons_paths.",
     is_flag=True,
     default=False
 )
 @click.option(
     '--quiet',
     help="Remove logs and warnings.",
     is_flag=True,
     default=False
 )
+@click.option(
+    '--exclude-modules',
+    help="Exclude queried modules from the found dependencies.",
+    is_flag=True,
+    default=False
+)
 @click.pass_context
 def show_dependencies(
     ctx,
     only_name,
     csv,
     installable,
     non_installable,
     without_version,
     modules,
     csv_modules,
     path,
     auto,
     quiet,
-    include_modules
+    include_modules,
+    exclude_modules,
 ):
     env = ctx.obj['env']
 
     if path:
         env.context.force_addons_lookup = True
         for _path in path:
             env.context.custom_paths.add(
@@ -274,14 +281,17 @@
             sorted_dependencies.append(modules_kv[dep])
         except KeyError:
             pass
 
     mods = [
         mod.path.name if only_name else str(mod)
         for mod in sorted_dependencies
+        if (
+            exclude_modules and mod.path.name not in check_modules
+        ) or not exclude_modules
     ]
 
     if csv:
         print(",".join(mods), end="")
     else:
         for mod in mods:
             print(mod)
```

### Comparing `odoo-tools-0.1.7/odoo_tools/cli/click/path.py` & `odoo-tools-0.1.9/odoo_tools/cli/click/path.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/cli/click/services.py` & `odoo-tools-0.1.9/odoo_tools/cli/click/services.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/cli/click/shell.py` & `odoo-tools-0.1.9/odoo_tools/cli/click/shell.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/cli/click/users.py` & `odoo-tools-0.1.9/odoo_tools/cli/click/users.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/cli/click/utils.py` & `odoo-tools-0.1.9/odoo_tools/cli/click/utils.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/cli/odot.py` & `odoo-tools-0.1.9/odoo_tools/cli/odot.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/cli/registry.py` & `odoo-tools-0.1.9/odoo_tools/cli/registry.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/compat.py` & `odoo-tools-0.1.9/odoo_tools/compat.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/configuration/git.py` & `odoo-tools-0.1.9/odoo_tools/configuration/git.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/configuration/misc.py` & `odoo-tools-0.1.9/odoo_tools/configuration/misc.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/configuration/odoo.py` & `odoo-tools-0.1.9/odoo_tools/configuration/odoo.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,18 +135,19 @@
         # Ensure setuptools less than 58 is installed for odoo
         # versions from 11 to 13.
         if (
             self.parsed_version.major > 10 and
             self.parsed_version.major < 14
         ):
             new_args = args[:]
+
             new_args += [
-                "setuptools<58"
+                "setuptools <58",
+                "pip <23"
             ]
-
             run(new_args)
 
         args += ['.', '-r', str(self.requirement_file)]
 
         with cd(self.odoo_dir):
             _logger.info("Installing odoo with command: '%s'", " ".join(args))
             run(args)
```

### Comparing `odoo-tools-0.1.7/odoo_tools/configuration/pip.py` & `odoo-tools-0.1.9/odoo_tools/configuration/pip.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/db.py` & `odoo-tools-0.1.9/odoo_tools/db.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/docker/sudo_entrypoint.py` & `odoo-tools-0.1.9/odoo_tools/docker/sudo_entrypoint.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/docker/user_entrypoint.py` & `odoo-tools-0.1.9/odoo_tools/docker/user_entrypoint.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/env.py` & `odoo-tools-0.1.9/odoo_tools/env.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/modules/assets.py` & `odoo-tools-0.1.9/odoo_tools/modules/assets.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/modules/render.py` & `odoo-tools-0.1.9/odoo_tools/modules/render.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/modules/search.py` & `odoo-tools-0.1.9/odoo_tools/modules/search.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/modules/translate.py` & `odoo-tools-0.1.9/odoo_tools/modules/translate.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/overlays/common/odoo/http.py` & `odoo-tools-0.1.9/odoo_tools/overlays/common/odoo/http.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/overlays/v14/odoo/addons/http_routing/models/ir_http.py` & `odoo-tools-0.1.9/odoo_tools/overlays/v14/odoo/addons/http_routing/models/ir_http.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/overlays/v14/odoo/addons/website/models/ir_http.py` & `odoo-tools-0.1.9/odoo_tools/overlays/v14/odoo/addons/website/models/ir_http.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/overlays/v14/odoo/addons/website/models/ir_qweb.py` & `odoo-tools-0.1.9/odoo_tools/overlays/v14/odoo/addons/website/models/ir_qweb.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/overlays/v15/odoo/addons/http_routing/models/ir_http.py` & `odoo-tools-0.1.9/odoo_tools/overlays/v15/odoo/addons/http_routing/models/ir_http.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/overlays/v15/odoo/addons/website/models/ir_http.py` & `odoo-tools-0.1.9/odoo_tools/overlays/v15/odoo/addons/website/models/ir_http.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/overlays/v15/odoo/addons/website/models/ir_qweb.py` & `odoo-tools-0.1.9/odoo_tools/overlays/v15/odoo/addons/website/models/ir_qweb.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/patch.py` & `odoo-tools-0.1.9/odoo_tools/patch.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/requirements/requirements-10.0.txt` & `odoo-tools-0.1.9/odoo_tools/requirements/requirements-10.0.txt`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/requirements/requirements-11.0.txt` & `odoo-tools-0.1.9/odoo_tools/requirements/requirements-11.0.txt`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/requirements/requirements-12.0.txt` & `odoo-tools-0.1.9/odoo_tools/requirements/requirements-12.0.txt`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/requirements/requirements-13.0.txt` & `odoo-tools-0.1.9/odoo_tools/requirements/requirements-13.0.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-setuptools<58
 Babel==2.6.0
 chardet==3.0.4
 decorator==4.3.0
 docutils>=0.14
 ebaysdk==2.1.5
 gevent==1.1.2 ; sys_platform != 'win32' and python_version < '3.7'
 gevent==1.5.0 ; python_version == '3.7'
```

### Comparing `odoo-tools-0.1.7/odoo_tools/requirements/requirements-14.0.txt` & `odoo-tools-0.1.9/odoo_tools/requirements/requirements-14.0.txt`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/requirements/requirements-15.0.txt` & `odoo-tools-0.1.9/odoo_tools/requirements/requirements-15.0.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 pydot==1.4.1
 pyopenssl>=21.0.0
 cryptography<39
 PyPDF2==1.26,<2.0
 pypiwin32 ; sys_platform == 'win32'
 pyserial==3.4
 python-dateutil==2.7.3
-python-ldap==3.4.0 ; sys_platform != 'win32'  # min version = 3.2.0 (Focal with security backports)
+python-ldap>=3.2.0 ; sys_platform != 'win32'  # min version = 3.2.0 (Focal with security backports)
 python-stdnum==1.13
 pytz==2019.3
 pyusb==1.0.2
 qrcode==6.1
 reportlab>=3.5.54 # version < 3.5.54 are not compatible with Pillow 8.1.2 and 3.5.59 is bullseye
 requests>=2.22.0, <3
 urllib3==1.26.5 # indirect / min version = 1.25.8 (Focal with security backports)
```

### Comparing `odoo-tools-0.1.7/odoo_tools/requirements/requirements-16.0.txt` & `odoo-tools-0.1.9/odoo_tools/requirements/requirements-16.0.txt`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/requirements/requirements-9.0.txt` & `odoo-tools-0.1.9/odoo_tools/requirements/requirements-9.0.txt`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/services/fields.py` & `odoo-tools-0.1.9/odoo_tools/services/fields.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/services/models.py` & `odoo-tools-0.1.9/odoo_tools/services/models.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/services/objects.py` & `odoo-tools-0.1.9/odoo_tools/services/objects.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/utilities/config.py` & `odoo-tools-0.1.9/odoo_tools/utilities/config.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/utilities/loaders.py` & `odoo-tools-0.1.9/odoo_tools/utilities/loaders.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/utilities/logging.py` & `odoo-tools-0.1.9/odoo_tools/utilities/logging.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/utilities/requirements.py` & `odoo-tools-0.1.9/odoo_tools/utilities/requirements.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools/utils.py` & `odoo-tools-0.1.9/odoo_tools/utils.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/odoo_tools.egg-info/PKG-INFO` & `odoo-tools-0.1.9/odoo_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-tools
-Version: 0.1.7
+Version: 0.1.9
 Summary: Odoo Tools
 Home-page: https://odoo-tools.readthedocs.io
 Author: Loïc Faure-Lacroix <lamerstar@gmail.com>
 Author-email: lamerstar@gmail.com
 License: GPL3
 Project-URL: Source, https://github.com/llacroix/odoo-tools
 Project-URL: Documentation, https://odoo-tools.readthedocs.io
```

### Comparing `odoo-tools-0.1.7/odoo_tools.egg-info/SOURCES.txt` & `odoo-tools-0.1.9/odoo_tools.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -65,26 +65,34 @@
 odoo_tools/docker/user_entrypoint.py
 odoo_tools/modules/__init__.py
 odoo_tools/modules/assets.py
 odoo_tools/modules/render.py
 odoo_tools/modules/search.py
 odoo_tools/modules/translate.py
 odoo_tools/overlays/common/odoo/http.py
+odoo_tools/overlays/common/odoo/__pycache__/http.cpython-38.pyc
 odoo_tools/overlays/common/odoo/addons/base/models/ir_http.py
+odoo_tools/overlays/common/odoo/addons/base/models/__pycache__/ir_http.cpython-38.pyc
 odoo_tools/overlays/common/odoo/modules/module.py
+odoo_tools/overlays/common/odoo/modules/__pycache__/module.cpython-38.pyc
 odoo_tools/overlays/v14/odoo/http.py
 odoo_tools/overlays/v14/odoo/addons/base/models/ir_http.py
 odoo_tools/overlays/v14/odoo/addons/http_routing/models/ir_http.py
 odoo_tools/overlays/v14/odoo/addons/website/models/ir_http.py
 odoo_tools/overlays/v14/odoo/addons/website/models/ir_qweb.py
 odoo_tools/overlays/v15/odoo/http.py
+odoo_tools/overlays/v15/odoo/__pycache__/http.cpython-38.pyc
 odoo_tools/overlays/v15/odoo/addons/base/models/ir_http.py
+odoo_tools/overlays/v15/odoo/addons/base/models/__pycache__/ir_http.cpython-38.pyc
 odoo_tools/overlays/v15/odoo/addons/http_routing/models/ir_http.py
+odoo_tools/overlays/v15/odoo/addons/http_routing/models/__pycache__/ir_http.cpython-38.pyc
 odoo_tools/overlays/v15/odoo/addons/website/models/ir_http.py
 odoo_tools/overlays/v15/odoo/addons/website/models/ir_qweb.py
+odoo_tools/overlays/v15/odoo/addons/website/models/__pycache__/ir_http.cpython-38.pyc
+odoo_tools/overlays/v15/odoo/addons/website/models/__pycache__/ir_qweb.cpython-38.pyc
 odoo_tools/packages/map-15.toml
 odoo_tools/packages/map-16.toml
 odoo_tools/requirements/requirements-10.0.txt
 odoo_tools/requirements/requirements-11.0.txt
 odoo_tools/requirements/requirements-12.0.txt
 odoo_tools/requirements/requirements-13.0.txt
 odoo_tools/requirements/requirements-14.0.txt
```

### Comparing `odoo-tools-0.1.7/odoo_tools.egg-info/entry_points.txt` & `odoo-tools-0.1.9/odoo_tools.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/setup.py` & `odoo-tools-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     module_path = Path.cwd() / module / path
 
     return find_files(module_path)
 
 
 setuptools.setup(
     name="odoo-tools",
-    version="0.1.7",
+    version="0.1.9",
     author="Loïc Faure-Lacroix <lamerstar@gmail.com>",
     author_email="lamerstar@gmail.com",
     description="Odoo Tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://odoo-tools.readthedocs.io",
     project_urls={
```

### Comparing `odoo-tools-0.1.7/tests/fixtures.py` & `odoo-tools-0.1.9/tests/fixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     options.languages = "fr_CA"
     options.upgrade = False
     options.target = None
     options.cache = None
 
     odoo_version = "{}.0".format(os.environ['TEST_ODOO'])
 
-    release = "20230222"
+    release = "20230601"
 
     env.manage.install_odoo(odoo_version, release=release, opts=options)
 
     try:
         yield env
     finally:
         odoo_cleanup(env)
```

### Comparing `odoo-tools-0.1.7/tests/test_api_context.py` & `odoo-tools-0.1.9/tests/test_api_context.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/tests/test_api_db.py` & `odoo-tools-0.1.9/tests/test_api_db.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/tests/test_api_objects.py` & `odoo-tools-0.1.9/tests/test_api_objects.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/tests/test_api_services.py` & `odoo-tools-0.1.9/tests/test_api_services.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/tests/test_cli.py` & `odoo-tools-0.1.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/tests/test_command_registry.py` & `odoo-tools-0.1.9/tests/test_command_registry.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/tests/test_compat.py` & `odoo-tools-0.1.9/tests/test_compat.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/tests/test_config_utilities.py` & `odoo-tools-0.1.9/tests/test_config_utilities.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/tests/test_configuration_git.py` & `odoo-tools-0.1.9/tests/test_configuration_git.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/tests/test_db.py` & `odoo-tools-0.1.9/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/tests/test_entrypoint.py` & `odoo-tools-0.1.9/tests/test_entrypoint.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/tests/test_env.py` & `odoo-tools-0.1.9/tests/test_env.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,14 +83,29 @@
     paths = env.addons_paths()
     assert paths == {tmp_path}
 
     env.context.force_addons_lookup = True
     assert env.addons_paths() == set()
 
 
+def test_env_config_whitespace_addons_path(tmp_path):
+    env = Environment()
+
+    env.context.odoo_rc = tmp_path / 'odoo.cfg'
+
+    with env.config():
+        env.set_config('addons_path', ",".join([f" {tmp_path}", ""]))
+
+    paths = env.addons_paths()
+    assert paths == {tmp_path}
+
+    env.context.force_addons_lookup = True
+    assert env.addons_paths() == set()
+
+
 def test_invalid_env(tmp_path):
     env = Environment()
 
     assert env.modules.list() == set()
 
     odoo_dir, addons_dir = generate_odoo_dir(tmp_path)
```

### Comparing `odoo-tools-0.1.7/tests/test_envvars.py` & `odoo-tools-0.1.9/tests/test_envvars.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/tests/test_manage.py` & `odoo-tools-0.1.9/tests/test_manage.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/tests/test_manifest.py` & `odoo-tools-0.1.9/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/tests/test_module_search.py` & `odoo-tools-0.1.9/tests/test_module_search.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/tests/test_modules.py` & `odoo-tools-0.1.9/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/tests/test_odoo_entrypoint.py` & `odoo-tools-0.1.9/tests/test_odoo_entrypoint.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/tests/test_odoo_git.py` & `odoo-tools-0.1.9/tests/test_odoo_git.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/tests/test_odoo_release.py` & `odoo-tools-0.1.9/tests/test_odoo_release.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/tests/test_rendering_description.py` & `odoo-tools-0.1.9/tests/test_rendering_description.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/tests/test_requirements.py` & `odoo-tools-0.1.9/tests/test_requirements.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/tests/test_services.py` & `odoo-tools-0.1.9/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/tests/test_utils.py` & `odoo-tools-0.1.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `odoo-tools-0.1.7/tests/utils.py` & `odoo-tools-0.1.9/tests/utils.py`

 * *Files identical despite different names*

