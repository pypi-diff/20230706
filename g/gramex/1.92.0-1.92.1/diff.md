# Comparing `tmp/gramex-1.92.0.tar.gz` & `tmp/gramex-1.92.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gramex-1.92.0.tar", last modified: Sun Jul  2 06:18:29 2023, max compression
+gzip compressed data, was "gramex-1.92.1.tar", last modified: Thu Jul  6 20:39:39 2023, max compression
```

## Comparing `gramex-1.92.0.tar` & `gramex-1.92.1.tar`

### file list

```diff
@@ -1,399 +1,399 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:29.158016 gramex-1.92.0/
--rw-rw-rw-   0        0        0     1968 2023-06-17 00:40:29.000000 gramex-1.92.0/.gitignore
--rw-rw-rw-   0        0        0     1274 2022-03-03 08:20:08.000000 gramex-1.92.0/LICENSE
--rw-rw-rw-   0        0        0      641 2023-05-13 04:30:57.000000 gramex-1.92.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2956 2023-07-02 06:18:29.158016 gramex-1.92.0/PKG-INFO
--rw-rw-rw-   0        0        0     1212 2022-09-13 04:40:48.000000 gramex-1.92.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.067998 gramex-1.92.0/gramex/
--rw-rw-rw-   0        0        0    15366 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/__init__.py
--rw-rw-rw-   0        0        0      242 2022-07-03 06:28:06.000000 gramex-1.92.0/gramex/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.116576 gramex-1.92.0/gramex/apps/
--rw-rw-rw-   0        0        0        0 2022-06-20 08:40:01.000000 gramex-1.92.0/gramex/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.120596 gramex-1.92.0/gramex/apps/admin/
--rw-rw-rw-   0        0        0        9 2019-01-01 03:16:23.000000 gramex-1.92.0/gramex/apps/admin/.gitignore
--rw-rw-rw-   0        0        0      129 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/admin/gramex.yaml
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.136304 gramex-1.92.0/gramex/apps/admin2/
--rw-rw-rw-   0        0        0      226 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/admin2/.snyk
--rw-rw-rw-   0        0        0      228 2019-04-01 03:34:34.000000 gramex-1.92.0/gramex/apps/admin2/admin.css
--rw-rw-rw-   0        0        0     3116 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/admin2/gramex.yaml
--rw-rw-rw-   0        0        0    12257 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/admin2/gramexadmin.py
--rw-rw-rw-   0        0        0     8420 2023-04-24 07:27:25.000000 gramex-1.92.0/gramex/apps/admin2/index.html
--rw-rw-rw-   0        0        0     5216 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/admin2/schedule.js
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.153805 gramex-1.92.0/gramex/apps/capture/
--rw-rw-rw-   0        0        0     4061 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/capture/README.md
--rw-rw-rw-   0        0        0     9374 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/capture/capture.js
--rw-rw-rw-   0        0        0    12051 2023-06-25 01:52:25.000000 gramex-1.92.0/gramex/apps/capture/chromecapture.js
--rw-rw-rw-   0        0        0     4197 2020-05-27 03:04:19.000000 gramex-1.92.0/gramex/apps/capture/index.html
--rw-rw-rw-   0        0        0   142301 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/apps/capture/package-lock.json
--rw-rw-rw-   0        0        0      863 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/capture/package.json
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.177013 gramex-1.92.0/gramex/apps/filemanager/
--rw-rw-rw-   0        0        0      305 2022-04-02 07:29:37.000000 gramex-1.92.0/gramex/apps/filemanager/.snyk
--rw-rw-rw-   0        0        0     2845 2022-10-17 06:55:24.000000 gramex-1.92.0/gramex/apps/filemanager/README.html
--rw-rw-rw-   0        0        0      700 2020-05-27 03:04:19.000000 gramex-1.92.0/gramex/apps/filemanager/drivehandler-snippet.html
--rw-rw-rw-   0        0        0      612 2022-10-17 06:55:24.000000 gramex-1.92.0/gramex/apps/filemanager/filemanager-snippet.html
--rw-rw-rw-   0        0        0     2578 2022-02-19 09:58:43.000000 gramex-1.92.0/gramex/apps/filemanager/filemanager.html
--rw-rw-rw-   0        0        0     3068 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/filemanager/filemanager.js
--rw-rw-rw-   0        0        0      926 2022-02-19 09:58:43.000000 gramex-1.92.0/gramex/apps/filemanager/filemanager.py
--rw-rw-rw-   0        0        0      621 2020-05-27 03:04:19.000000 gramex-1.92.0/gramex/apps/filemanager/gramex.yaml
--rw-rw-rw-   0        0        0      914 2020-05-27 03:04:19.000000 gramex-1.92.0/gramex/apps/filemanager/index.html
--rw-rw-rw-   0        0        0      872 2020-05-27 03:04:19.000000 gramex-1.92.0/gramex/apps/filemanager/navbar.html
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:27.910952 gramex-1.92.0/gramex/apps/init/
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.207254 gramex-1.92.0/gramex/apps/init/default/
--rw-rw-rw-   0        0        0      578 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/init/default/.eslintrc.yml
--rw-rw-rw-   0        0        0       71 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/init/default/.flake8
--rw-rw-rw-   0        0        0      756 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/init/default/.gitlab-ci.yml
--rw-rw-rw-   0        0        0      386 2022-02-19 10:03:02.000000 gramex-1.92.0/gramex/apps/init/default/.secrets.yaml
--rw-rw-rw-   0        0        0     1635 2022-02-19 10:03:02.000000 gramex-1.92.0/gramex/apps/init/default/.template.gitignore
--rw-rw-rw-   0        0        0      248 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/init/default/README.template.md
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.209444 gramex-1.92.0/gramex/apps/init/default/assets/
--rw-rw-rw-   0        0        0      519 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/init/default/assets/README.template.md
--rw-rw-rw-   0        0        0     1756 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/init/default/gramex.template.yaml
--rw-rw-rw-   0        0        0      694 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/init/default/index.template.html
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.212767 gramex-1.92.0/gramex/apps/init/default/js/
--rw-rw-rw-   0        0        0      602 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/init/default/js/README.template.md
--rw-rw-rw-   0        0        0     2608 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/init/default/login.template.html
--rw-rw-rw-   0        0        0      352 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/init/default/package.template.json
--rw-rw-rw-   0        0        0       80 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/init/default/style.scss
--rw-rw-rw-   0        0        0     3499 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/init/default/template-navbar.template.html
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.222248 gramex-1.92.0/gramex/apps/init/ide/
--rw-rw-rw-   0        0        0      378 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/init/ide/.gitlab-ci.template.yml
--rw-rw-rw-   0        0        0      244 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/init/ide/gramex.template.yaml
--rw-rw-rw-   0        0        0      738 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/init/ide/index.template.html
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.226244 gramex-1.92.0/gramex/apps/init/minimal/
--rw-rw-rw-   0        0        0      247 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/init/minimal/gramex.template.yaml
--rw-rw-rw-   0        0        0      757 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/init/minimal/index.template.html
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.235256 gramex-1.92.0/gramex/apps/languagetool/
--rw-rw-rw-   0        0        0      709 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/languagetool/README.md
--rw-rw-rw-   0        0        0        0 2022-06-20 08:40:41.000000 gramex-1.92.0/gramex/apps/languagetool/__init__.py
--rw-rw-rw-   0        0        0      788 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/languagetool/gramex.yaml
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.288576 gramex-1.92.0/gramex/apps/logviewer/
--rw-rw-rw-   0        0        0        0 2022-06-20 08:40:32.000000 gramex-1.92.0/gramex/apps/logviewer/__init__.py
--rw-rw-rw-   0        0        0     3466 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/logviewer/config.yaml
--rw-rw-rw-   0        0        0     6291 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/logviewer/gramex.yaml
--rw-rw-rw-   0        0        0     4958 2020-05-27 03:04:19.000000 gramex-1.92.0/gramex/apps/logviewer/index.html
--rw-rw-rw-   0        0        0    13287 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/logviewer/logviewer.py
--rw-rw-rw-   0        0        0      210 2018-12-27 08:44:54.000000 gramex-1.92.0/gramex/apps/logviewer/lv-card-deck.html
--rw-rw-rw-   0        0        0      386 2018-04-14 05:44:28.000000 gramex-1.92.0/gramex/apps/logviewer/lv-card.html
--rw-rw-rw-   0        0        0      526 2018-04-14 05:44:28.000000 gramex-1.92.0/gramex/apps/logviewer/lv-datepicker.html
--rw-rw-rw-   0        0        0      331 2018-04-14 05:44:28.000000 gramex-1.92.0/gramex/apps/logviewer/lv-dropdown.html
--rw-rw-rw-   0        0        0      465 2018-12-27 08:44:54.000000 gramex-1.92.0/gramex/apps/logviewer/lv-filters.html
--rw-rw-rw-   0        0        0      113 2018-04-14 05:44:28.000000 gramex-1.92.0/gramex/apps/logviewer/lv-header.html
--rw-rw-rw-   0        0        0      335 2018-04-14 05:44:28.000000 gramex-1.92.0/gramex/apps/logviewer/lv-kpi.html
--rw-rw-rw-   0        0        0      775 2023-07-02 04:13:13.000000 gramex-1.92.0/gramex/apps/logviewer/package-lock.json
--rw-rw-rw-   0        0        0      179 2021-07-06 10:52:07.000000 gramex-1.92.0/gramex/apps/logviewer/package.json
--rw-rw-rw-   0        0        0     6928 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/logviewer/render.js
--rw-rw-rw-   0        0        0     5390 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/logviewer/script.js
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.293578 gramex-1.92.0/gramex/apps/mail/
--rw-rw-rw-   0        0        0      430 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/mail/gramex.yaml
--rw-rw-rw-   0        0        0     3032 2019-01-15 12:01:13.000000 gramex-1.92.0/gramex/apps/mail/index.html
--rw-rw-rw-   0        0        0      251 2018-03-15 10:39:12.000000 gramex-1.92.0/gramex/apps/mail/mailapp.py
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.296572 gramex-1.92.0/gramex/apps/mlhandler/
--rw-rw-rw-   0        0        0    15225 2022-05-03 15:40:40.000000 gramex-1.92.0/gramex/apps/mlhandler/template.html
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.311128 gramex-1.92.0/gramex/apps/pynode/
--rw-rw-rw-   0        0        0      318 2022-02-19 10:03:03.000000 gramex-1.92.0/gramex/apps/pynode/.snyk
--rw-rw-rw-   0        0        0       47 2018-10-22 05:47:08.000000 gramex-1.92.0/gramex/apps/pynode/README.md
--rw-rw-rw-   0        0        0     4122 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/pynode/index.js
--rw-rw-rw-   0        0        0     2953 2023-07-02 04:13:17.000000 gramex-1.92.0/gramex/apps/pynode/package-lock.json
--rw-rw-rw-   0        0        0      187 2022-07-03 06:28:06.000000 gramex-1.92.0/gramex/apps/pynode/package.json
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.317128 gramex-1.92.0/gramex/apps/smartalerts/
--rw-rw-rw-   0        0        0       89 2018-03-15 10:39:12.000000 gramex-1.92.0/gramex/apps/smartalerts/gramex.yaml
--rw-rw-rw-   0        0        0      429 2018-02-10 11:30:50.000000 gramex-1.92.0/gramex/apps/smartalerts/index.html
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.341135 gramex-1.92.0/gramex/apps/ui/
--rw-rw-rw-   0        0        0      667 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/apps/ui/.snyk
--rw-rw-rw-   0        0        0    13165 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/apps/ui/__init__.py
--rw-rw-rw-   0        0        0      648 2023-04-24 07:13:24.000000 gramex-1.92.0/gramex/apps/ui/bootstrap-theme.scss
--rw-rw-rw-   0        0        0     1056 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/config.yaml
--rw-rw-rw-   0        0        0     2082 2022-11-13 06:15:28.000000 gramex-1.92.0/gramex/apps/ui/gramex.yaml
--rw-rw-rw-   0        0        0    25259 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/gramexui.scss
--rw-rw-rw-   0        0        0   163730 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/apps/ui/package-lock.json
--rw-rw-rw-   0        0        0      265 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/apps/ui/package.json
--rw-rw-rw-   0        0        0     2486 2022-12-05 03:38:51.000000 gramex-1.92.0/gramex/apps/ui/setup.js
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.362659 gramex-1.92.0/gramex/apps/ui/theme/
--rw-rw-rw-   0        0        0    19343 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/bootstrap5.scss
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.471892 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/
--rw-rw-rw-   0        0        0     6324 2022-02-19 10:03:03.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/cerulean.png
--rw-rw-rw-   0        0        0      175 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/cerulean.scss
--rw-rw-rw-   0        0        0     4833 2022-02-19 10:03:03.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/cosmo.png
--rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/cosmo.scss
--rw-rw-rw-   0        0        0     6569 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/cyborg.png
--rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/cyborg.scss
--rw-rw-rw-   0        0        0     5932 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/darkly.png
--rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/darkly.scss
--rw-rw-rw-   0        0        0     5114 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/flatly.png
--rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/flatly.scss
--rw-rw-rw-   0        0        0     5335 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/journal.png
--rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/journal.scss
--rw-rw-rw-   0        0        0     6141 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/litera.png
--rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/litera.scss
--rw-rw-rw-   0        0        0     4958 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/lumen.png
--rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/lumen.scss
--rw-rw-rw-   0        0        0     4818 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/lux.png
--rw-rw-rw-   0        0        0      160 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/lux.scss
--rw-rw-rw-   0        0        0     5791 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/materia.png
--rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/materia.scss
--rw-rw-rw-   0        0        0     5662 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/minty.png
--rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/minty.scss
--rw-rw-rw-   0        0        0     4777 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/pulse.png
--rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/pulse.scss
--rw-rw-rw-   0        0        0     5246 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/sandstone.png
--rw-rw-rw-   0        0        0      178 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/sandstone.scss
--rw-rw-rw-   0        0        0     6213 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/simplex.png
--rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/simplex.scss
--rw-rw-rw-   0        0        0     7371 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/sketchy.png
--rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/sketchy.scss
--rw-rw-rw-   0        0        0     6288 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/slate.png
--rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/slate.scss
--rw-rw-rw-   0        0        0     6158 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/solar.png
--rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/solar.scss
--rw-rw-rw-   0        0        0     6501 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/spacelab.png
--rw-rw-rw-   0        0        0      175 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/spacelab.scss
--rw-rw-rw-   0        0        0     6357 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/superhero.png
--rw-rw-rw-   0        0        0      178 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/superhero.scss
--rw-rw-rw-   0        0        0     5432 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/united.png
--rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/united.scss
--rw-rw-rw-   0        0        0     4842 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/yeti.png
--rw-rw-rw-   0        0        0      163 2022-06-22 13:49:07.000000 gramex-1.92.0/gramex/apps/ui/theme/bootswatch/yeti.scss
--rw-rw-rw-   0        0        0     4573 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/default.png
--rw-rw-rw-   0        0        0       20 2022-02-19 09:58:43.000000 gramex-1.92.0/gramex/apps/ui/theme/default.scss
--rw-rw-rw-   0        0        0      831 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/index.html
--rw-rw-rw-   0        0        0    71063 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/sample.html
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.552981 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/
--rw-rw-rw-   0        0        0     6383 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/blue_voltage.png
--rw-rw-rw-   0        0        0      630 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/blue_voltage.scss
--rw-rw-rw-   0        0        0     6282 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/boldstrap.png
--rw-rw-rw-   0        0        0      478 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/boldstrap.scss
--rw-rw-rw-   0        0        0     6215 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/bootstrap_purple.png
--rw-rw-rw-   0        0        0      268 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/bootstrap_purple.scss
--rw-rw-rw-   0        0        0     6153 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/darkster.png
--rw-rw-rw-   0        0        0     2559 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/darkster.scss
--rw-rw-rw-   0        0        0     5497 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/fresca.png
--rw-rw-rw-   0        0        0      362 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/fresca.scss
--rw-rw-rw-   0        0        0     5525 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/greyson.png
--rw-rw-rw-   0        0        0      571 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/greyson.scss
--rw-rw-rw-   0        0        0     5153 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/hello_kiddie.png
--rw-rw-rw-   0        0        0      621 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/hello_kiddie.scss
--rw-rw-rw-   0        0        0     5523 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/herbie.png
--rw-rw-rw-   0        0        0      480 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/herbie.scss
--rw-rw-rw-   0        0        0     6585 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/hootstrap.png
--rw-rw-rw-   0        0        0      487 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/hootstrap.scss
--rw-rw-rw-   0        0        0     5491 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/lovey.png
--rw-rw-rw-   0        0        0      461 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/lovey.scss
--rw-rw-rw-   0        0        0     6009 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/monotony.png
--rw-rw-rw-   0        0        0      486 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/monotony.scss
--rw-rw-rw-   0        0        0     5546 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/poypull.png
--rw-rw-rw-   0        0        0      541 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/poypull.scss
--rw-rw-rw-   0        0        0     5430 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/signal.png
--rw-rw-rw-   0        0        0      576 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/signal.scss
--rw-rw-rw-   0        0        0     5338 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/tequila.png
--rw-rw-rw-   0        0        0      371 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/ui/theme/themes-guide/tequila.scss
--rw-rw-rw-   0        0        0      801 2022-09-13 04:40:48.000000 gramex-1.92.0/gramex/apps/ui/theme/themes.json
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.686688 gramex-1.92.0/gramex/apps/uifactory/
--rw-rw-rw-   0        0        0      739 2022-11-02 08:06:14.000000 gramex-1.92.0/gramex/apps/uifactory/.eslintrc.js
--rw-rw-rw-   0        0        0       46 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/.gitattributes
--rw-rw-rw-   0        0        0       57 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/.gitignore
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.688688 gramex-1.92.0/gramex/apps/uifactory/assets/
--rw-rw-rw-   0        0        0      432 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/assets/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.690688 gramex-1.92.0/gramex/apps/uifactory/assets/data/
--rw-rw-rw-   0        0        0     1674 2022-09-13 04:40:51.000000 gramex-1.92.0/gramex/apps/uifactory/assets/data/input.json
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.704039 gramex-1.92.0/gramex/apps/uifactory/assets/img/
--rw-rw-rw-   0        0        0      706 2022-06-23 02:35:29.000000 gramex-1.92.0/gramex/apps/uifactory/assets/img/arrows-move.svg
--rw-rw-rw-   0        0        0      496 2022-06-23 02:35:29.000000 gramex-1.92.0/gramex/apps/uifactory/assets/img/clipboard.svg
--rw-rw-rw-   0        0        0      978 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/assets/img/gramener-favicon-blue.png
--rw-rw-rw-   0        0        0      573 2022-06-23 02:35:29.000000 gramex-1.92.0/gramex/apps/uifactory/assets/img/trash.svg
--rw-rw-rw-   0        0        0     6667 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/create.html
--rw-rw-rw-   0        0        0     2673 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/edit.html
--rw-rw-rw-   0        0        0      694 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/field-actions.html
--rw-rw-rw-   0        0        0     4361 2022-11-06 08:24:31.000000 gramex-1.92.0/gramex/apps/uifactory/form_builder.py
--rw-rw-rw-   0        0        0     4749 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/gramex.yaml
--rw-rw-rw-   0        0        0     6274 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/index.html
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.730191 gramex-1.92.0/gramex/apps/uifactory/js/
--rw-rw-rw-   0        0        0      601 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/js/README.md
--rw-rw-rw-   0        0        0      435 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/js/embed.js
--rw-rw-rw-   0        0        0    16411 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/js/fields.js
--rw-rw-rw-   0        0        0     1942 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/js/fork-form.js
--rw-rw-rw-   0        0        0     3080 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/js/index.js
--rw-rw-rw-   0        0        0     9228 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/js/script.js
--rw-rw-rw-   0        0        0      829 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/js/utils.js
--rw-rw-rw-   0        0        0     2776 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/js/viewform.js
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.751263 gramex-1.92.0/gramex/apps/uifactory/modals/
--rw-rw-rw-   0        0        0     1117 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/modals/add-field.html
--rw-rw-rw-   0        0        0     4107 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/modals/embed.html
--rw-rw-rw-   0        0        0      898 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/modals/remove.html
--rw-rw-rw-   0        0        0      952 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/modals/rename.html
--rw-rw-rw-   0        0        0     1323 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/modals/themes.html
--rw-rw-rw-   0        0        0     5781 2023-07-02 04:14:00.000000 gramex-1.92.0/gramex/apps/uifactory/package-lock.json
--rw-rw-rw-   0        0        0      206 2022-03-03 08:20:09.000000 gramex-1.92.0/gramex/apps/uifactory/package.json
--rw-rw-rw-   0        0        0     1548 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/popover-form.html
--rw-rw-rw-   0        0        0     1952 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/sample.html
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.766205 gramex-1.92.0/gramex/apps/uifactory/snippets/
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.768989 gramex-1.92.0/gramex/apps/uifactory/snippets/button/
--rw-rw-rw-   0        0        0     2795 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/snippets/button/bs4-button.js
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.772555 gramex-1.92.0/gramex/apps/uifactory/snippets/checkbox/
--rw-rw-rw-   0        0        0     1225 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/snippets/checkbox/bs4-checkbox.js
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.775554 gramex-1.92.0/gramex/apps/uifactory/snippets/email/
--rw-rw-rw-   0        0        0      604 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/snippets/email/bs4-email.js
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.781701 gramex-1.92.0/gramex/apps/uifactory/snippets/hidden/
--rw-rw-rw-   0        0        0      327 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/snippets/hidden/bs4-hidden.js
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.785738 gramex-1.92.0/gramex/apps/uifactory/snippets/html/
--rw-rw-rw-   0        0        0      292 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/snippets/html/bs4-html.js
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.788725 gramex-1.92.0/gramex/apps/uifactory/snippets/multiselect/
--rw-rw-rw-   0        0        0     4735 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/snippets/multiselect/bs4-multiselect.js
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.790873 gramex-1.92.0/gramex/apps/uifactory/snippets/number/
--rw-rw-rw-   0        0        0      736 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/snippets/number/bs4-number.js
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.796521 gramex-1.92.0/gramex/apps/uifactory/snippets/password/
--rw-rw-rw-   0        0        0      375 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/snippets/password/bs4-password.js
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.800032 gramex-1.92.0/gramex/apps/uifactory/snippets/radio/
--rw-rw-rw-   0        0        0     1034 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/snippets/radio/bs4-radio.js
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.802042 gramex-1.92.0/gramex/apps/uifactory/snippets/range/
--rw-rw-rw-   0        0        0      610 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/snippets/range/bs4-range.js
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.805032 gramex-1.92.0/gramex/apps/uifactory/snippets/select/
--rw-rw-rw-   0        0        0     1617 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/snippets/select/bs4-select.js
--rw-rw-rw-   0        0        0      946 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/snippets/setup.js
--rw-rw-rw-   0        0        0        3 2023-04-17 10:18:07.000000 gramex-1.92.0/gramex/apps/uifactory/snippets/snippets.json
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.808040 gramex-1.92.0/gramex/apps/uifactory/snippets/text/
--rw-rw-rw-   0        0        0      974 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/snippets/text/bs4-text.js
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.812032 gramex-1.92.0/gramex/apps/uifactory/snippets/textarea/
--rw-rw-rw-   0        0        0     1094 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/uifactory/snippets/textarea/bs4-textarea.js
--rw-rw-rw-   0        0        0     1815 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps/uifactory/style.scss
--rw-rw-rw-   0        0        0     2013 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/template-navbar-view-form.html
--rw-rw-rw-   0        0        0     1020 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/template-navbar.html
--rw-rw-rw-   0        0        0      415 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/toast.html
--rw-rw-rw-   0        0        0     6516 2022-02-19 10:03:04.000000 gramex-1.92.0/gramex/apps/uifactory/viewform.html
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.823142 gramex-1.92.0/gramex/apps/update/
--rw-rw-rw-   0        0        0      565 2018-10-30 07:47:04.000000 gramex-1.92.0/gramex/apps/update/README.md
--rw-rw-rw-   0        0        0     2397 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/apps/update/gramex.yaml
--rw-rw-rw-   0        0        0     4593 2022-11-06 08:24:31.000000 gramex-1.92.0/gramex/apps/update/gramexupdate.py
--rw-rw-rw-   0        0        0     3310 2022-03-03 08:20:09.000000 gramex-1.92.0/gramex/apps/update/index.html
--rw-rw-rw-   0        0        0      277 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/apps.yaml
--rw-rw-rw-   0        0        0    58478 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/cache.py
--rw-rw-rw-   0        0        0    35221 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/config.py
--rw-rw-rw-   0        0        0    93430 2023-05-27 08:02:09.000000 gramex-1.92.0/gramex/data.py
--rw-rw-rw-   0        0        0     6408 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/debug.py
--rw-rw-rw-   0        0        0     1825 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/deploy.yaml
--rw-rw-rw-   0        0        0     1466 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/download.vega.js
--rw-rw-rw-   0        0        0    12057 2018-10-22 05:47:08.000000 gramex-1.92.0/gramex/favicon.ico
--rw-rw-rw-   0        0        0    15621 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/gramex.yaml
--rw-rw-rw-   0        0        0     6262 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/gramexfeatures.csv
--rw-rw-rw-   0        0        0    14340 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/gramexsize.csv
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.951295 gramex-1.92.0/gramex/handlers/
--rw-rw-rw-   0        0        0     1368 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/handlers/400.html
--rw-rw-rw-   0        0        0     2081 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/handlers/401.html
--rw-rw-rw-   0        0        0     2483 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/handlers/403.html
--rw-rw-rw-   0        0        0     1399 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/handlers/404.html
--rw-rw-rw-   0        0        0     2163 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/handlers/500.html
--rw-rw-rw-   0        0        0     3085 2023-06-19 14:23:48.000000 gramex-1.92.0/gramex/handlers/__init__.py
--rw-rw-rw-   0        0        0      532 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/handlers/auth.recaptcha.template.html
--rw-rw-rw-   0        0        0     3862 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/handlers/auth.template.html
--rw-rw-rw-   0        0        0    17347 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/handlers/authhandler.py
--rw-rw-rw-   0        0        0    65374 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/handlers/basehandler.py
--rw-rw-rw-   0        0        0    15771 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/handlers/capturehandler.py
--rw-rw-rw-   0        0        0     6643 2023-07-02 04:09:20.000000 gramex-1.92.0/gramex/handlers/chatgpthandler.py
--rw-rw-rw-   0        0        0     1477 2023-06-08 09:04:46.000000 gramex-1.92.0/gramex/handlers/comichandler.py
--rw-rw-rw-   0        0        0     8904 2023-06-17 00:11:07.000000 gramex-1.92.0/gramex/handlers/drivehandler.py
--rw-rw-rw-   0        0        0    14917 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/handlers/filehandler.py
--rw-rw-rw-   0        0        0     1271 2022-07-03 06:28:09.000000 gramex-1.92.0/gramex/handlers/filehandler.template.html
--rw-rw-rw-   0        0        0      198 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/handlers/filterhandler.py
--rw-rw-rw-   0        0        0    13125 2023-06-19 14:23:49.000000 gramex-1.92.0/gramex/handlers/formhandler.py
--rw-rw-rw-   0        0        0     3774 2023-06-08 09:04:46.000000 gramex-1.92.0/gramex/handlers/functionhandler.py
--rw-rw-rw-   0        0        0     6706 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/handlers/jsonhandler.py
--rw-rw-rw-   0        0        0     6838 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/handlers/messagehandler.py
--rw-rw-rw-   0        0        0    16154 2023-06-02 05:59:12.000000 gramex-1.92.0/gramex/handlers/mlhandler.py
--rw-rw-rw-   0        0        0     7492 2023-06-08 09:04:46.000000 gramex-1.92.0/gramex/handlers/modelhandler.py
--rw-rw-rw-   0        0        0     1413 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/handlers/openapiconfig.yaml
--rw-rw-rw-   0        0        0     7326 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/handlers/openapihandler.py
--rw-rw-rw-   0        0        0      818 2023-06-08 09:04:46.000000 gramex-1.92.0/gramex/handlers/pptxhandler.py
--rw-rw-rw-   0        0        0     5145 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/handlers/processhandler.py
--rw-rw-rw-   0        0        0     7882 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/handlers/proxyhandler.py
--rw-rw-rw-   0        0        0     1362 2022-10-17 06:55:24.000000 gramex-1.92.0/gramex/handlers/queryhandler.template.html
--rw-rw-rw-   0        0        0    11338 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/handlers/socialhandler.py
--rw-rw-rw-   0        0        0     9434 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/handlers/uploadhandler.py
--rw-rw-rw-   0        0        0     2121 2022-11-23 03:19:45.000000 gramex-1.92.0/gramex/handlers/websockethandler.py
--rw-rw-rw-   0        0        0     1458 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/http.py
--rw-rw-rw-   0        0        0    35069 2023-06-17 00:40:29.000000 gramex-1.92.0/gramex/install.py
--rw-rw-rw-   0        0        0     2086 2022-09-13 04:40:51.000000 gramex-1.92.0/gramex/license.py
--rw-rw-rw-   0        0        0     2005 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/migrate.py
--rw-rw-rw-   0        0        0    18629 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/ml.py
--rw-rw-rw-   0        0        0    13687 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/ml_api.py
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.969316 gramex-1.92.0/gramex/pptgen/
--rw-rw-rw-   0        0        0     9967 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/pptgen/__init__.py
--rw-rw-rw-   0        0        0    18868 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/pptgen/color.py
--rw-rw-rw-   0        0        0     7779 2018-01-31 16:40:23.000000 gramex-1.92.0/gramex/pptgen/colors.json
--rw-rw-rw-   0        0        0    45490 2022-11-02 08:06:17.000000 gramex-1.92.0/gramex/pptgen/commands.py
--rw-rw-rw-   0        0        0     6351 2018-01-31 16:40:23.000000 gramex-1.92.0/gramex/pptgen/fonts.json
--rw-rw-rw-   0        0        0     1304 2022-11-02 08:06:18.000000 gramex-1.92.0/gramex/pptgen/fontwidth.py
--rw-rw-rw-   0        0        0    26250 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/pptgen/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.978185 gramex-1.92.0/gramex/pptgen2/
--rw-rw-rw-   0        0        0    23438 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/pptgen2/__init__.py
--rw-rw-rw-   0        0        0    34432 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/pptgen2/commands.py
--rw-rw-rw-   0        0        0    12068 2022-11-02 08:06:18.000000 gramex-1.92.0/gramex/pptgen2/config.yaml
--rw-rw-rw-   0        0        0     4278 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/pynode.py
--rw-rw-rw-   0        0        0     2979 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/scale.py
--rw-rw-rw-   0        0        0     1057 2022-11-02 08:06:18.000000 gramex-1.92.0/gramex/secrets.py
--rw-rw-rw-   0        0        0     2508 2022-11-02 08:06:18.000000 gramex-1.92.0/gramex/servicenow.yaml
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:29.000893 gramex-1.92.0/gramex/services/
--rw-rw-rw-   0        0        0    39783 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/services/__init__.py
--rw-rw-rw-   0        0        0    11451 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/services/emailer.py
--rw-rw-rw-   0        0        0     3724 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/services/rediscache.py
--rw-rw-rw-   0        0        0     7164 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/services/scheduler.py
--rw-rw-rw-   0        0        0     3684 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/services/sms.py
--rw-rw-rw-   0        0        0     6385 2023-05-13 04:30:57.000000 gramex-1.92.0/gramex/services/ttlcache.py
--rw-rw-rw-   0        0        0     4521 2023-06-27 08:54:47.000000 gramex-1.92.0/gramex/services/urlcache.py
--rw-rw-rw-   0        0        0     5822 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/services/watcher.py
--rw-rw-rw-   0        0        0     3831 2022-11-02 08:06:18.000000 gramex-1.92.0/gramex/sm_api.py
--rw-rw-rw-   0        0        0     8638 2022-11-02 08:06:18.000000 gramex-1.92.0/gramex/topcause.py
--rw-rw-rw-   0        0        0     8710 2022-11-02 08:06:18.000000 gramex-1.92.0/gramex/transformers.py
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:29.018509 gramex-1.92.0/gramex/transforms/
--rw-rw-rw-   0        0        0      787 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/transforms/__init__.py
--rw-rw-rw-   0        0        0     1658 2022-09-13 04:40:51.000000 gramex-1.92.0/gramex/transforms/auth.py
--rw-rw-rw-   0        0        0     3022 2023-07-02 06:16:31.000000 gramex-1.92.0/gramex/transforms/template.py
--rw-rw-rw-   0        0        0    32960 2023-06-19 14:23:49.000000 gramex-1.92.0/gramex/transforms/transforms.py
--rw-rw-rw-   0        0        0    10095 2023-06-08 09:27:24.000000 gramex-1.92.0/gramex/transforms/twitterstream.py
--rw-rw-rw-   0        0        0     6808 2022-11-13 04:18:56.000000 gramex-1.92.0/gramex/winservice.py
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:28.114595 gramex-1.92.0/gramex.egg-info/
--rw-rw-rw-   0        0        0     2956 2023-07-02 06:18:26.000000 gramex-1.92.0/gramex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    12004 2023-07-02 06:18:27.000000 gramex-1.92.0/gramex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 06:18:26.000000 gramex-1.92.0/gramex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      123 2023-07-02 06:18:26.000000 gramex-1.92.0/gramex.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      953 2023-07-02 06:18:26.000000 gramex-1.92.0/gramex.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-02 06:18:26.000000 gramex-1.92.0/gramex.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6171 2023-07-02 06:16:31.000000 gramex-1.92.0/pyproject.toml
--rw-rw-rw-   0        0        0      503 2023-07-02 06:18:29.178968 gramex-1.92.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-02 06:18:29.156018 gramex-1.92.0/tests/
--rw-rw-rw-   0        0        0     5233 2022-11-06 08:24:18.000000 gramex-1.92.0/tests/test_admin.py
--rw-rw-rw-   0        0        0     9054 2023-04-18 08:45:54.000000 gramex-1.92.0/tests/test_alerts.py
--rw-rw-rw-   0        0        0     3981 2022-11-06 08:24:18.000000 gramex-1.92.0/tests/test_args.py
--rw-rw-rw-   0        0        0    39128 2023-06-19 14:23:49.000000 gramex-1.92.0/tests/test_auth.py
--rw-rw-rw-   0        0        0    14612 2022-11-06 08:24:18.000000 gramex-1.92.0/tests/test_cache.py
--rw-rw-rw-   0        0        0    15062 2023-05-13 04:30:57.000000 gramex-1.92.0/tests/test_capturehandler.py
--rw-rw-rw-   0        0        0     1288 2022-11-06 08:24:19.000000 gramex-1.92.0/tests/test_comichandler.py
--rw-rw-rw-   0        0        0    12571 2023-06-19 14:23:49.000000 gramex-1.92.0/tests/test_drivehandler.py
--rw-rw-rw-   0        0        0    17308 2023-07-02 06:16:31.000000 gramex-1.92.0/tests/test_filehandler.py
--rw-rw-rw-   0        0        0     6797 2023-05-13 04:30:57.000000 gramex-1.92.0/tests/test_filterhandler.py
--rw-rw-rw-   0        0        0    35746 2023-05-27 08:02:33.000000 gramex-1.92.0/tests/test_formhandler.py
--rw-rw-rw-   0        0        0     8784 2022-11-06 08:24:22.000000 gramex-1.92.0/tests/test_functionhandler.py
--rw-rw-rw-   0        0        0     3201 2022-11-06 08:24:22.000000 gramex-1.92.0/tests/test_gramexlog.py
--rw-rw-rw-   0        0        0    19008 2023-06-19 14:23:49.000000 gramex-1.92.0/tests/test_handlers.py
--rw-rw-rw-   0        0        0     1475 2022-11-02 08:06:18.000000 gramex-1.92.0/tests/test_init.py
--rw-rw-rw-   0        0        0     8931 2023-05-13 04:30:57.000000 gramex-1.92.0/tests/test_install.py
--rw-rw-rw-   0        0        0     6361 2022-11-06 08:24:23.000000 gramex-1.92.0/tests/test_jsonhandler.py
--rw-rw-rw-   0        0        0     3896 2022-11-06 08:24:23.000000 gramex-1.92.0/tests/test_ldapauth.py
--rw-rw-rw-   0        0        0     7519 2022-11-02 08:06:18.000000 gramex-1.92.0/tests/test_logviewer.py
--rw-rw-rw-   0        0        0    32878 2022-11-23 04:49:14.000000 gramex-1.92.0/tests/test_mlhandler.py
--rw-rw-rw-   0        0        0     4745 2022-11-02 08:06:18.000000 gramex-1.92.0/tests/test_modelhandler.py
--rw-rw-rw-   0        0        0     7082 2023-05-13 04:30:57.000000 gramex-1.92.0/tests/test_openapihandler.py
--rw-rw-rw-   0        0        0     1411 2022-11-02 08:06:18.000000 gramex-1.92.0/tests/test_pptxhandler.py
--rw-rw-rw-   0        0        0     3530 2022-11-06 08:24:24.000000 gramex-1.92.0/tests/test_processhandler.py
--rw-rw-rw-   0        0        0     3834 2022-11-06 08:24:24.000000 gramex-1.92.0/tests/test_proxyhandler.py
--rw-rw-rw-   0        0        0     1527 2022-11-02 08:06:18.000000 gramex-1.92.0/tests/test_pynode.py
--rw-rw-rw-   0        0        0     1220 2022-11-06 08:24:24.000000 gramex-1.92.0/tests/test_schedule.py
--rw-rw-rw-   0        0        0      757 2022-02-19 10:03:06.000000 gramex-1.92.0/tests/test_secrets.py
--rw-rw-rw-   0        0        0      330 2020-05-27 03:04:19.000000 gramex-1.92.0/tests/test_sms.py
--rw-rw-rw-   0        0        0      180 2017-08-29 07:52:03.000000 gramex-1.92.0/tests/test_subapp.py
--rw-rw-rw-   0        0        0     5382 2022-11-02 08:06:18.000000 gramex-1.92.0/tests/test_subprocess.py
--rw-rw-rw-   0        0        0     2277 2022-11-02 08:06:18.000000 gramex-1.92.0/tests/test_translater.py
--rw-rw-rw-   0        0        0     2895 2022-11-06 08:24:24.000000 gramex-1.92.0/tests/test_twitterresthandler.py
--rw-rw-rw-   0        0        0     2352 2022-11-06 08:24:24.000000 gramex-1.92.0/tests/test_ui.py
--rw-rw-rw-   0        0        0     2359 2022-11-02 08:06:18.000000 gramex-1.92.0/tests/test_update.py
--rw-rw-rw-   0        0        0     6563 2022-11-06 08:24:25.000000 gramex-1.92.0/tests/test_uploadhandler.py
--rw-rw-rw-   0        0        0     1966 2022-11-02 08:06:18.000000 gramex-1.92.0/tests/test_watcher.py
--rw-rw-rw-   0        0        0     2647 2022-11-06 08:24:25.000000 gramex-1.92.0/tests/test_websockethandler.py
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:39.044749 gramex-1.92.1/
+-rw-rw-rw-   0        0        0     1968 2023-06-17 00:40:29.000000 gramex-1.92.1/.gitignore
+-rw-rw-rw-   0        0        0     1274 2022-03-03 08:20:08.000000 gramex-1.92.1/LICENSE
+-rw-rw-rw-   0        0        0      641 2023-05-13 04:30:57.000000 gramex-1.92.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2956 2023-07-06 20:39:39.044749 gramex-1.92.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1212 2022-09-13 04:40:48.000000 gramex-1.92.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:34.634182 gramex-1.92.1/gramex/
+-rw-rw-rw-   0        0        0    15366 2023-07-06 20:38:13.000000 gramex-1.92.1/gramex/__init__.py
+-rw-rw-rw-   0        0        0      242 2022-07-03 06:28:06.000000 gramex-1.92.1/gramex/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:34.691086 gramex-1.92.1/gramex/apps/
+-rw-rw-rw-   0        0        0        0 2022-06-20 08:40:01.000000 gramex-1.92.1/gramex/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:34.699085 gramex-1.92.1/gramex/apps/admin/
+-rw-rw-rw-   0        0        0        9 2019-01-01 03:16:23.000000 gramex-1.92.1/gramex/apps/admin/.gitignore
+-rw-rw-rw-   0        0        0      129 2023-05-13 04:30:57.000000 gramex-1.92.1/gramex/apps/admin/gramex.yaml
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:34.805629 gramex-1.92.1/gramex/apps/admin2/
+-rw-rw-rw-   0        0        0      226 2023-05-13 04:30:57.000000 gramex-1.92.1/gramex/apps/admin2/.snyk
+-rw-rw-rw-   0        0        0      228 2019-04-01 03:34:34.000000 gramex-1.92.1/gramex/apps/admin2/admin.css
+-rw-rw-rw-   0        0        0     3116 2022-11-02 08:06:14.000000 gramex-1.92.1/gramex/apps/admin2/gramex.yaml
+-rw-rw-rw-   0        0        0    12257 2023-05-13 04:30:57.000000 gramex-1.92.1/gramex/apps/admin2/gramexadmin.py
+-rw-rw-rw-   0        0        0     8420 2023-04-24 07:27:25.000000 gramex-1.92.1/gramex/apps/admin2/index.html
+-rw-rw-rw-   0        0        0     5216 2023-05-13 04:30:57.000000 gramex-1.92.1/gramex/apps/admin2/schedule.js
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:34.861933 gramex-1.92.1/gramex/apps/capture/
+-rw-rw-rw-   0        0        0     4061 2022-11-02 08:06:14.000000 gramex-1.92.1/gramex/apps/capture/README.md
+-rw-rw-rw-   0        0        0     9451 2023-07-06 20:38:13.000000 gramex-1.92.1/gramex/apps/capture/capture.js
+-rw-rw-rw-   0        0        0    12060 2023-07-06 20:38:13.000000 gramex-1.92.1/gramex/apps/capture/chromecapture.js
+-rw-rw-rw-   0        0        0     4197 2020-05-27 03:04:19.000000 gramex-1.92.1/gramex/apps/capture/index.html
+-rw-rw-rw-   0        0        0   142301 2023-07-02 06:16:31.000000 gramex-1.92.1/gramex/apps/capture/package-lock.json
+-rw-rw-rw-   0        0        0      863 2023-05-13 04:30:57.000000 gramex-1.92.1/gramex/apps/capture/package.json
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:34.990562 gramex-1.92.1/gramex/apps/filemanager/
+-rw-rw-rw-   0        0        0      305 2022-04-02 07:29:37.000000 gramex-1.92.1/gramex/apps/filemanager/.snyk
+-rw-rw-rw-   0        0        0     2845 2022-10-17 06:55:24.000000 gramex-1.92.1/gramex/apps/filemanager/README.html
+-rw-rw-rw-   0        0        0      700 2020-05-27 03:04:19.000000 gramex-1.92.1/gramex/apps/filemanager/drivehandler-snippet.html
+-rw-rw-rw-   0        0        0      612 2022-10-17 06:55:24.000000 gramex-1.92.1/gramex/apps/filemanager/filemanager-snippet.html
+-rw-rw-rw-   0        0        0     2578 2022-02-19 09:58:43.000000 gramex-1.92.1/gramex/apps/filemanager/filemanager.html
+-rw-rw-rw-   0        0        0     3070 2023-07-06 20:38:13.000000 gramex-1.92.1/gramex/apps/filemanager/filemanager.js
+-rw-rw-rw-   0        0        0      926 2022-02-19 09:58:43.000000 gramex-1.92.1/gramex/apps/filemanager/filemanager.py
+-rw-rw-rw-   0        0        0      621 2020-05-27 03:04:19.000000 gramex-1.92.1/gramex/apps/filemanager/gramex.yaml
+-rw-rw-rw-   0        0        0      914 2020-05-27 03:04:19.000000 gramex-1.92.1/gramex/apps/filemanager/index.html
+-rw-rw-rw-   0        0        0      872 2020-05-27 03:04:19.000000 gramex-1.92.1/gramex/apps/filemanager/navbar.html
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:34.126857 gramex-1.92.1/gramex/apps/init/
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:35.121989 gramex-1.92.1/gramex/apps/init/default/
+-rw-rw-rw-   0        0        0      578 2023-05-13 04:30:57.000000 gramex-1.92.1/gramex/apps/init/default/.eslintrc.yml
+-rw-rw-rw-   0        0        0       71 2022-11-02 08:06:14.000000 gramex-1.92.1/gramex/apps/init/default/.flake8
+-rw-rw-rw-   0        0        0      756 2023-05-13 04:30:57.000000 gramex-1.92.1/gramex/apps/init/default/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0      386 2022-02-19 10:03:02.000000 gramex-1.92.1/gramex/apps/init/default/.secrets.yaml
+-rw-rw-rw-   0        0        0     1635 2022-02-19 10:03:02.000000 gramex-1.92.1/gramex/apps/init/default/.template.gitignore
+-rw-rw-rw-   0        0        0      248 2022-11-02 08:06:14.000000 gramex-1.92.1/gramex/apps/init/default/README.template.md
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:35.130017 gramex-1.92.1/gramex/apps/init/default/assets/
+-rw-rw-rw-   0        0        0      519 2022-11-02 08:06:14.000000 gramex-1.92.1/gramex/apps/init/default/assets/README.template.md
+-rw-rw-rw-   0        0        0     1756 2023-05-13 04:30:57.000000 gramex-1.92.1/gramex/apps/init/default/gramex.template.yaml
+-rw-rw-rw-   0        0        0      694 2023-05-13 04:30:57.000000 gramex-1.92.1/gramex/apps/init/default/index.template.html
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:35.130017 gramex-1.92.1/gramex/apps/init/default/js/
+-rw-rw-rw-   0        0        0      602 2022-11-02 08:06:14.000000 gramex-1.92.1/gramex/apps/init/default/js/README.template.md
+-rw-rw-rw-   0        0        0     2608 2023-05-13 04:30:57.000000 gramex-1.92.1/gramex/apps/init/default/login.template.html
+-rw-rw-rw-   0        0        0      352 2023-05-13 04:30:57.000000 gramex-1.92.1/gramex/apps/init/default/package.template.json
+-rw-rw-rw-   0        0        0       80 2023-05-13 04:30:57.000000 gramex-1.92.1/gramex/apps/init/default/style.scss
+-rw-rw-rw-   0        0        0     3499 2023-05-13 04:30:57.000000 gramex-1.92.1/gramex/apps/init/default/template-navbar.template.html
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:35.171059 gramex-1.92.1/gramex/apps/init/ide/
+-rw-rw-rw-   0        0        0      378 2023-05-13 04:30:57.000000 gramex-1.92.1/gramex/apps/init/ide/.gitlab-ci.template.yml
+-rw-rw-rw-   0        0        0      244 2023-05-13 04:30:57.000000 gramex-1.92.1/gramex/apps/init/ide/gramex.template.yaml
+-rw-rw-rw-   0        0        0      738 2023-05-13 04:30:57.000000 gramex-1.92.1/gramex/apps/init/ide/index.template.html
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:35.202529 gramex-1.92.1/gramex/apps/init/minimal/
+-rw-rw-rw-   0        0        0      247 2023-05-13 04:30:57.000000 gramex-1.92.1/gramex/apps/init/minimal/gramex.template.yaml
+-rw-rw-rw-   0        0        0      757 2023-05-13 04:30:57.000000 gramex-1.92.1/gramex/apps/init/minimal/index.template.html
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:35.219080 gramex-1.92.1/gramex/apps/languagetool/
+-rw-rw-rw-   0        0        0      709 2022-11-02 08:06:14.000000 gramex-1.92.1/gramex/apps/languagetool/README.md
+-rw-rw-rw-   0        0        0        0 2022-06-20 08:40:41.000000 gramex-1.92.1/gramex/apps/languagetool/__init__.py
+-rw-rw-rw-   0        0        0      788 2022-11-02 08:06:14.000000 gramex-1.92.1/gramex/apps/languagetool/gramex.yaml
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:35.414838 gramex-1.92.1/gramex/apps/logviewer/
+-rw-rw-rw-   0        0        0        0 2022-06-20 08:40:32.000000 gramex-1.92.1/gramex/apps/logviewer/__init__.py
+-rw-rw-rw-   0        0        0     3466 2022-11-02 08:06:14.000000 gramex-1.92.1/gramex/apps/logviewer/config.yaml
+-rw-rw-rw-   0        0        0     6291 2022-11-02 08:06:14.000000 gramex-1.92.1/gramex/apps/logviewer/gramex.yaml
+-rw-rw-rw-   0        0        0     4958 2020-05-27 03:04:19.000000 gramex-1.92.1/gramex/apps/logviewer/index.html
+-rw-rw-rw-   0        0        0    13287 2023-07-06 20:35:09.000000 gramex-1.92.1/gramex/apps/logviewer/logviewer.py
+-rw-rw-rw-   0        0        0      210 2018-12-27 08:44:54.000000 gramex-1.92.1/gramex/apps/logviewer/lv-card-deck.html
+-rw-rw-rw-   0        0        0      386 2018-04-14 05:44:28.000000 gramex-1.92.1/gramex/apps/logviewer/lv-card.html
+-rw-rw-rw-   0        0        0      526 2018-04-14 05:44:28.000000 gramex-1.92.1/gramex/apps/logviewer/lv-datepicker.html
+-rw-rw-rw-   0        0        0      331 2018-04-14 05:44:28.000000 gramex-1.92.1/gramex/apps/logviewer/lv-dropdown.html
+-rw-rw-rw-   0        0        0      465 2018-12-27 08:44:54.000000 gramex-1.92.1/gramex/apps/logviewer/lv-filters.html
+-rw-rw-rw-   0        0        0      113 2018-04-14 05:44:28.000000 gramex-1.92.1/gramex/apps/logviewer/lv-header.html
+-rw-rw-rw-   0        0        0      335 2018-04-14 05:44:28.000000 gramex-1.92.1/gramex/apps/logviewer/lv-kpi.html
+-rw-rw-rw-   0        0        0      775 2023-07-02 04:13:13.000000 gramex-1.92.1/gramex/apps/logviewer/package-lock.json
+-rw-rw-rw-   0        0        0      179 2021-07-06 10:52:07.000000 gramex-1.92.1/gramex/apps/logviewer/package.json
+-rw-rw-rw-   0        0        0     6928 2022-11-02 08:06:14.000000 gramex-1.92.1/gramex/apps/logviewer/render.js
+-rw-rw-rw-   0        0        0     5390 2023-05-13 04:30:57.000000 gramex-1.92.1/gramex/apps/logviewer/script.js
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:35.453459 gramex-1.92.1/gramex/apps/mail/
+-rw-rw-rw-   0        0        0      430 2022-11-02 08:06:14.000000 gramex-1.92.1/gramex/apps/mail/gramex.yaml
+-rw-rw-rw-   0        0        0     3032 2019-01-15 12:01:13.000000 gramex-1.92.1/gramex/apps/mail/index.html
+-rw-rw-rw-   0        0        0      251 2018-03-15 10:39:12.000000 gramex-1.92.1/gramex/apps/mail/mailapp.py
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:35.485444 gramex-1.92.1/gramex/apps/mlhandler/
+-rw-rw-rw-   0        0        0    15225 2022-05-03 15:40:40.000000 gramex-1.92.1/gramex/apps/mlhandler/template.html
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:35.518126 gramex-1.92.1/gramex/apps/pynode/
+-rw-rw-rw-   0        0        0      318 2022-02-19 10:03:03.000000 gramex-1.92.1/gramex/apps/pynode/.snyk
+-rw-rw-rw-   0        0        0       47 2018-10-22 05:47:08.000000 gramex-1.92.1/gramex/apps/pynode/README.md
+-rw-rw-rw-   0        0        0     4127 2023-07-06 20:38:13.000000 gramex-1.92.1/gramex/apps/pynode/index.js
+-rw-rw-rw-   0        0        0     2953 2023-07-02 04:13:17.000000 gramex-1.92.1/gramex/apps/pynode/package-lock.json
+-rw-rw-rw-   0        0        0      187 2022-07-03 06:28:06.000000 gramex-1.92.1/gramex/apps/pynode/package.json
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:35.542527 gramex-1.92.1/gramex/apps/smartalerts/
+-rw-rw-rw-   0        0        0       89 2018-03-15 10:39:12.000000 gramex-1.92.1/gramex/apps/smartalerts/gramex.yaml
+-rw-rw-rw-   0        0        0      429 2018-02-10 11:30:50.000000 gramex-1.92.1/gramex/apps/smartalerts/index.html
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:35.618171 gramex-1.92.1/gramex/apps/ui/
+-rw-rw-rw-   0        0        0      667 2023-07-02 06:16:31.000000 gramex-1.92.1/gramex/apps/ui/.snyk
+-rw-rw-rw-   0        0        0    13165 2023-07-02 06:16:31.000000 gramex-1.92.1/gramex/apps/ui/__init__.py
+-rw-rw-rw-   0        0        0      648 2023-04-24 07:13:24.000000 gramex-1.92.1/gramex/apps/ui/bootstrap-theme.scss
+-rw-rw-rw-   0        0        0     1056 2022-11-02 08:06:14.000000 gramex-1.92.1/gramex/apps/ui/config.yaml
+-rw-rw-rw-   0        0        0     2082 2022-11-13 06:15:28.000000 gramex-1.92.1/gramex/apps/ui/gramex.yaml
+-rw-rw-rw-   0        0        0    25271 2023-07-06 20:38:13.000000 gramex-1.92.1/gramex/apps/ui/gramexui.scss
+-rw-rw-rw-   0        0        0   163730 2023-07-06 18:52:16.000000 gramex-1.92.1/gramex/apps/ui/package-lock.json
+-rw-rw-rw-   0        0        0      265 2023-07-02 06:16:31.000000 gramex-1.92.1/gramex/apps/ui/package.json
+-rw-rw-rw-   0        0        0     2490 2023-07-06 20:38:13.000000 gramex-1.92.1/gramex/apps/ui/setup.js
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:35.683283 gramex-1.92.1/gramex/apps/ui/theme/
+-rw-rw-rw-   0        0        0    19355 2023-07-06 20:38:13.000000 gramex-1.92.1/gramex/apps/ui/theme/bootstrap5.scss
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:35.905597 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/
+-rw-rw-rw-   0        0        0     6324 2022-02-19 10:03:03.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/cerulean.png
+-rw-rw-rw-   0        0        0      175 2022-06-22 13:49:07.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/cerulean.scss
+-rw-rw-rw-   0        0        0     4833 2022-02-19 10:03:03.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/cosmo.png
+-rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/cosmo.scss
+-rw-rw-rw-   0        0        0     6569 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/cyborg.png
+-rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/cyborg.scss
+-rw-rw-rw-   0        0        0     5932 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/darkly.png
+-rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/darkly.scss
+-rw-rw-rw-   0        0        0     5114 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/flatly.png
+-rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/flatly.scss
+-rw-rw-rw-   0        0        0     5335 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/journal.png
+-rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/journal.scss
+-rw-rw-rw-   0        0        0     6141 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/litera.png
+-rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/litera.scss
+-rw-rw-rw-   0        0        0     4958 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/lumen.png
+-rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/lumen.scss
+-rw-rw-rw-   0        0        0     4818 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/lux.png
+-rw-rw-rw-   0        0        0      160 2022-06-22 13:49:07.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/lux.scss
+-rw-rw-rw-   0        0        0     5791 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/materia.png
+-rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/materia.scss
+-rw-rw-rw-   0        0        0     5662 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/minty.png
+-rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/minty.scss
+-rw-rw-rw-   0        0        0     4777 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/pulse.png
+-rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/pulse.scss
+-rw-rw-rw-   0        0        0     5246 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/sandstone.png
+-rw-rw-rw-   0        0        0      178 2022-06-22 13:49:07.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/sandstone.scss
+-rw-rw-rw-   0        0        0     6213 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/simplex.png
+-rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/simplex.scss
+-rw-rw-rw-   0        0        0     7371 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/sketchy.png
+-rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/sketchy.scss
+-rw-rw-rw-   0        0        0     6288 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/slate.png
+-rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/slate.scss
+-rw-rw-rw-   0        0        0     6158 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/solar.png
+-rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/solar.scss
+-rw-rw-rw-   0        0        0     6501 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/spacelab.png
+-rw-rw-rw-   0        0        0      175 2022-06-22 13:49:07.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/spacelab.scss
+-rw-rw-rw-   0        0        0     6357 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/superhero.png
+-rw-rw-rw-   0        0        0      178 2022-06-22 13:49:07.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/superhero.scss
+-rw-rw-rw-   0        0        0     5432 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/united.png
+-rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/united.scss
+-rw-rw-rw-   0        0        0     4842 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/yeti.png
+-rw-rw-rw-   0        0        0      163 2022-06-22 13:49:07.000000 gramex-1.92.1/gramex/apps/ui/theme/bootswatch/yeti.scss
+-rw-rw-rw-   0        0        0     4573 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/default.png
+-rw-rw-rw-   0        0        0       20 2022-02-19 09:58:43.000000 gramex-1.92.1/gramex/apps/ui/theme/default.scss
+-rw-rw-rw-   0        0        0      831 2022-11-02 08:06:14.000000 gramex-1.92.1/gramex/apps/ui/theme/index.html
+-rw-rw-rw-   0        0        0    71063 2022-11-02 08:06:14.000000 gramex-1.92.1/gramex/apps/ui/theme/sample.html
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:36.258103 gramex-1.92.1/gramex/apps/ui/theme/themes-guide/
+-rw-rw-rw-   0        0        0     6383 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/themes-guide/blue_voltage.png
+-rw-rw-rw-   0        0        0      630 2022-11-02 08:06:14.000000 gramex-1.92.1/gramex/apps/ui/theme/themes-guide/blue_voltage.scss
+-rw-rw-rw-   0        0        0     6282 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/themes-guide/boldstrap.png
+-rw-rw-rw-   0        0        0      478 2022-11-02 08:06:14.000000 gramex-1.92.1/gramex/apps/ui/theme/themes-guide/boldstrap.scss
+-rw-rw-rw-   0        0        0     6215 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/themes-guide/bootstrap_purple.png
+-rw-rw-rw-   0        0        0      268 2022-11-02 08:06:14.000000 gramex-1.92.1/gramex/apps/ui/theme/themes-guide/bootstrap_purple.scss
+-rw-rw-rw-   0        0        0     6153 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/themes-guide/darkster.png
+-rw-rw-rw-   0        0        0     2559 2022-11-02 08:06:14.000000 gramex-1.92.1/gramex/apps/ui/theme/themes-guide/darkster.scss
+-rw-rw-rw-   0        0        0     5497 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/themes-guide/fresca.png
+-rw-rw-rw-   0        0        0      362 2022-11-02 08:06:14.000000 gramex-1.92.1/gramex/apps/ui/theme/themes-guide/fresca.scss
+-rw-rw-rw-   0        0        0     5525 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/themes-guide/greyson.png
+-rw-rw-rw-   0        0        0      571 2022-11-02 08:06:14.000000 gramex-1.92.1/gramex/apps/ui/theme/themes-guide/greyson.scss
+-rw-rw-rw-   0        0        0     5153 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/themes-guide/hello_kiddie.png
+-rw-rw-rw-   0        0        0      621 2022-11-02 08:06:14.000000 gramex-1.92.1/gramex/apps/ui/theme/themes-guide/hello_kiddie.scss
+-rw-rw-rw-   0        0        0     5523 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/themes-guide/herbie.png
+-rw-rw-rw-   0        0        0      480 2022-11-02 08:06:14.000000 gramex-1.92.1/gramex/apps/ui/theme/themes-guide/herbie.scss
+-rw-rw-rw-   0        0        0     6585 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/themes-guide/hootstrap.png
+-rw-rw-rw-   0        0        0      487 2022-11-02 08:06:14.000000 gramex-1.92.1/gramex/apps/ui/theme/themes-guide/hootstrap.scss
+-rw-rw-rw-   0        0        0     5491 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/themes-guide/lovey.png
+-rw-rw-rw-   0        0        0      461 2022-11-02 08:06:14.000000 gramex-1.92.1/gramex/apps/ui/theme/themes-guide/lovey.scss
+-rw-rw-rw-   0        0        0     6009 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/themes-guide/monotony.png
+-rw-rw-rw-   0        0        0      486 2022-11-02 08:06:14.000000 gramex-1.92.1/gramex/apps/ui/theme/themes-guide/monotony.scss
+-rw-rw-rw-   0        0        0     5546 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/themes-guide/poypull.png
+-rw-rw-rw-   0        0        0      541 2022-11-02 08:06:14.000000 gramex-1.92.1/gramex/apps/ui/theme/themes-guide/poypull.scss
+-rw-rw-rw-   0        0        0     5430 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/themes-guide/signal.png
+-rw-rw-rw-   0        0        0      576 2022-11-02 08:06:14.000000 gramex-1.92.1/gramex/apps/ui/theme/themes-guide/signal.scss
+-rw-rw-rw-   0        0        0     5338 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/ui/theme/themes-guide/tequila.png
+-rw-rw-rw-   0        0        0      371 2022-11-02 08:06:14.000000 gramex-1.92.1/gramex/apps/ui/theme/themes-guide/tequila.scss
+-rw-rw-rw-   0        0        0      801 2022-09-13 04:40:48.000000 gramex-1.92.1/gramex/apps/ui/theme/themes.json
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:36.749694 gramex-1.92.1/gramex/apps/uifactory/
+-rw-rw-rw-   0        0        0      739 2022-11-02 08:06:14.000000 gramex-1.92.1/gramex/apps/uifactory/.eslintrc.js
+-rw-rw-rw-   0        0        0       46 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/uifactory/.gitattributes
+-rw-rw-rw-   0        0        0       57 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/uifactory/.gitignore
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:36.755684 gramex-1.92.1/gramex/apps/uifactory/assets/
+-rw-rw-rw-   0        0        0      432 2022-11-02 08:06:17.000000 gramex-1.92.1/gramex/apps/uifactory/assets/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:36.771824 gramex-1.92.1/gramex/apps/uifactory/assets/data/
+-rw-rw-rw-   0        0        0     1674 2022-09-13 04:40:51.000000 gramex-1.92.1/gramex/apps/uifactory/assets/data/input.json
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:36.828919 gramex-1.92.1/gramex/apps/uifactory/assets/img/
+-rw-rw-rw-   0        0        0      706 2022-06-23 02:35:29.000000 gramex-1.92.1/gramex/apps/uifactory/assets/img/arrows-move.svg
+-rw-rw-rw-   0        0        0      496 2022-06-23 02:35:29.000000 gramex-1.92.1/gramex/apps/uifactory/assets/img/clipboard.svg
+-rw-rw-rw-   0        0        0      978 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/uifactory/assets/img/gramener-favicon-blue.png
+-rw-rw-rw-   0        0        0      573 2022-06-23 02:35:29.000000 gramex-1.92.1/gramex/apps/uifactory/assets/img/trash.svg
+-rw-rw-rw-   0        0        0     6667 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/uifactory/create.html
+-rw-rw-rw-   0        0        0     2673 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/uifactory/edit.html
+-rw-rw-rw-   0        0        0      694 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/uifactory/field-actions.html
+-rw-rw-rw-   0        0        0     4361 2022-11-06 08:24:31.000000 gramex-1.92.1/gramex/apps/uifactory/form_builder.py
+-rw-rw-rw-   0        0        0     4749 2022-11-02 08:06:17.000000 gramex-1.92.1/gramex/apps/uifactory/gramex.yaml
+-rw-rw-rw-   0        0        0     6274 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/uifactory/index.html
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:36.868456 gramex-1.92.1/gramex/apps/uifactory/js/
+-rw-rw-rw-   0        0        0      601 2022-11-02 08:06:17.000000 gramex-1.92.1/gramex/apps/uifactory/js/README.md
+-rw-rw-rw-   0        0        0      436 2023-07-06 20:38:13.000000 gramex-1.92.1/gramex/apps/uifactory/js/embed.js
+-rw-rw-rw-   0        0        0    16411 2022-11-02 08:06:17.000000 gramex-1.92.1/gramex/apps/uifactory/js/fields.js
+-rw-rw-rw-   0        0        0     1943 2023-07-06 20:38:13.000000 gramex-1.92.1/gramex/apps/uifactory/js/fork-form.js
+-rw-rw-rw-   0        0        0     3080 2022-11-02 08:06:17.000000 gramex-1.92.1/gramex/apps/uifactory/js/index.js
+-rw-rw-rw-   0        0        0     9232 2023-07-06 20:38:13.000000 gramex-1.92.1/gramex/apps/uifactory/js/script.js
+-rw-rw-rw-   0        0        0      829 2022-11-02 08:06:17.000000 gramex-1.92.1/gramex/apps/uifactory/js/utils.js
+-rw-rw-rw-   0        0        0     2779 2023-07-06 20:38:13.000000 gramex-1.92.1/gramex/apps/uifactory/js/viewform.js
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:36.975752 gramex-1.92.1/gramex/apps/uifactory/modals/
+-rw-rw-rw-   0        0        0     1117 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/uifactory/modals/add-field.html
+-rw-rw-rw-   0        0        0     4107 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/uifactory/modals/embed.html
+-rw-rw-rw-   0        0        0      898 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/uifactory/modals/remove.html
+-rw-rw-rw-   0        0        0      952 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/uifactory/modals/rename.html
+-rw-rw-rw-   0        0        0     1323 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/uifactory/modals/themes.html
+-rw-rw-rw-   0        0        0     5781 2023-07-02 04:14:00.000000 gramex-1.92.1/gramex/apps/uifactory/package-lock.json
+-rw-rw-rw-   0        0        0      206 2022-03-03 08:20:09.000000 gramex-1.92.1/gramex/apps/uifactory/package.json
+-rw-rw-rw-   0        0        0     1548 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/uifactory/popover-form.html
+-rw-rw-rw-   0        0        0     1952 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/uifactory/sample.html
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:36.991500 gramex-1.92.1/gramex/apps/uifactory/snippets/
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:36.991500 gramex-1.92.1/gramex/apps/uifactory/snippets/button/
+-rw-rw-rw-   0        0        0     2795 2022-11-02 08:06:17.000000 gramex-1.92.1/gramex/apps/uifactory/snippets/button/bs4-button.js
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:36.999466 gramex-1.92.1/gramex/apps/uifactory/snippets/checkbox/
+-rw-rw-rw-   0        0        0     1225 2022-11-02 08:06:17.000000 gramex-1.92.1/gramex/apps/uifactory/snippets/checkbox/bs4-checkbox.js
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:36.999466 gramex-1.92.1/gramex/apps/uifactory/snippets/email/
+-rw-rw-rw-   0        0        0      604 2022-11-02 08:06:17.000000 gramex-1.92.1/gramex/apps/uifactory/snippets/email/bs4-email.js
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:37.006486 gramex-1.92.1/gramex/apps/uifactory/snippets/hidden/
+-rw-rw-rw-   0        0        0      327 2022-11-02 08:06:17.000000 gramex-1.92.1/gramex/apps/uifactory/snippets/hidden/bs4-hidden.js
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:37.020485 gramex-1.92.1/gramex/apps/uifactory/snippets/html/
+-rw-rw-rw-   0        0        0      292 2022-11-02 08:06:17.000000 gramex-1.92.1/gramex/apps/uifactory/snippets/html/bs4-html.js
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:37.023013 gramex-1.92.1/gramex/apps/uifactory/snippets/multiselect/
+-rw-rw-rw-   0        0        0     4735 2022-11-02 08:06:17.000000 gramex-1.92.1/gramex/apps/uifactory/snippets/multiselect/bs4-multiselect.js
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:37.023013 gramex-1.92.1/gramex/apps/uifactory/snippets/number/
+-rw-rw-rw-   0        0        0      736 2022-11-02 08:06:17.000000 gramex-1.92.1/gramex/apps/uifactory/snippets/number/bs4-number.js
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:37.031110 gramex-1.92.1/gramex/apps/uifactory/snippets/password/
+-rw-rw-rw-   0        0        0      375 2022-11-02 08:06:17.000000 gramex-1.92.1/gramex/apps/uifactory/snippets/password/bs4-password.js
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:37.032773 gramex-1.92.1/gramex/apps/uifactory/snippets/radio/
+-rw-rw-rw-   0        0        0     1034 2022-11-02 08:06:17.000000 gramex-1.92.1/gramex/apps/uifactory/snippets/radio/bs4-radio.js
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:37.039290 gramex-1.92.1/gramex/apps/uifactory/snippets/range/
+-rw-rw-rw-   0        0        0      610 2022-11-02 08:06:17.000000 gramex-1.92.1/gramex/apps/uifactory/snippets/range/bs4-range.js
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:37.047610 gramex-1.92.1/gramex/apps/uifactory/snippets/select/
+-rw-rw-rw-   0        0        0     1617 2022-11-02 08:06:17.000000 gramex-1.92.1/gramex/apps/uifactory/snippets/select/bs4-select.js
+-rw-rw-rw-   0        0        0      947 2023-07-06 20:38:13.000000 gramex-1.92.1/gramex/apps/uifactory/snippets/setup.js
+-rw-rw-rw-   0        0        0        3 2023-04-17 10:18:07.000000 gramex-1.92.1/gramex/apps/uifactory/snippets/snippets.json
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:37.049371 gramex-1.92.1/gramex/apps/uifactory/snippets/text/
+-rw-rw-rw-   0        0        0      974 2022-11-02 08:06:17.000000 gramex-1.92.1/gramex/apps/uifactory/snippets/text/bs4-text.js
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:37.056575 gramex-1.92.1/gramex/apps/uifactory/snippets/textarea/
+-rw-rw-rw-   0        0        0     1094 2022-11-02 08:06:17.000000 gramex-1.92.1/gramex/apps/uifactory/snippets/textarea/bs4-textarea.js
+-rw-rw-rw-   0        0        0     1815 2023-05-13 04:30:57.000000 gramex-1.92.1/gramex/apps/uifactory/style.scss
+-rw-rw-rw-   0        0        0     2013 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/uifactory/template-navbar-view-form.html
+-rw-rw-rw-   0        0        0     1020 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/uifactory/template-navbar.html
+-rw-rw-rw-   0        0        0      415 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/uifactory/toast.html
+-rw-rw-rw-   0        0        0     6516 2022-02-19 10:03:04.000000 gramex-1.92.1/gramex/apps/uifactory/viewform.html
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:37.139752 gramex-1.92.1/gramex/apps/update/
+-rw-rw-rw-   0        0        0      565 2018-10-30 07:47:04.000000 gramex-1.92.1/gramex/apps/update/README.md
+-rw-rw-rw-   0        0        0     2397 2022-11-02 08:06:17.000000 gramex-1.92.1/gramex/apps/update/gramex.yaml
+-rw-rw-rw-   0        0        0     4593 2022-11-06 08:24:31.000000 gramex-1.92.1/gramex/apps/update/gramexupdate.py
+-rw-rw-rw-   0        0        0     3310 2022-03-03 08:20:09.000000 gramex-1.92.1/gramex/apps/update/index.html
+-rw-rw-rw-   0        0        0      277 2023-05-13 04:30:57.000000 gramex-1.92.1/gramex/apps.yaml
+-rw-rw-rw-   0        0        0    58478 2023-07-02 06:16:31.000000 gramex-1.92.1/gramex/cache.py
+-rw-rw-rw-   0        0        0    35221 2023-05-13 04:30:57.000000 gramex-1.92.1/gramex/config.py
+-rw-rw-rw-   0        0        0    93430 2023-05-27 08:02:09.000000 gramex-1.92.1/gramex/data.py
+-rw-rw-rw-   0        0        0     6408 2023-06-08 09:27:24.000000 gramex-1.92.1/gramex/debug.py
+-rw-rw-rw-   0        0        0     1825 2022-11-02 08:06:17.000000 gramex-1.92.1/gramex/deploy.yaml
+-rw-rw-rw-   0        0        0     1467 2023-07-06 20:38:13.000000 gramex-1.92.1/gramex/download.vega.js
+-rw-rw-rw-   0        0        0    12057 2018-10-22 05:47:08.000000 gramex-1.92.1/gramex/favicon.ico
+-rw-rw-rw-   0        0        0    15621 2023-07-02 06:16:31.000000 gramex-1.92.1/gramex/gramex.yaml
+-rw-rw-rw-   0        0        0     6262 2023-06-08 09:27:24.000000 gramex-1.92.1/gramex/gramexfeatures.csv
+-rw-rw-rw-   0        0        0    14340 2023-07-02 06:16:31.000000 gramex-1.92.1/gramex/gramexsize.csv
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:37.783238 gramex-1.92.1/gramex/handlers/
+-rw-rw-rw-   0        0        0     1368 2022-11-02 08:06:17.000000 gramex-1.92.1/gramex/handlers/400.html
+-rw-rw-rw-   0        0        0     2081 2022-11-02 08:06:17.000000 gramex-1.92.1/gramex/handlers/401.html
+-rw-rw-rw-   0        0        0     2483 2023-06-08 09:27:24.000000 gramex-1.92.1/gramex/handlers/403.html
+-rw-rw-rw-   0        0        0     1399 2022-11-02 08:06:17.000000 gramex-1.92.1/gramex/handlers/404.html
+-rw-rw-rw-   0        0        0     2163 2022-11-02 08:06:17.000000 gramex-1.92.1/gramex/handlers/500.html
+-rw-rw-rw-   0        0        0     3085 2023-06-19 14:23:48.000000 gramex-1.92.1/gramex/handlers/__init__.py
+-rw-rw-rw-   0        0        0      532 2022-11-02 08:06:17.000000 gramex-1.92.1/gramex/handlers/auth.recaptcha.template.html
+-rw-rw-rw-   0        0        0     3862 2023-05-13 04:30:57.000000 gramex-1.92.1/gramex/handlers/auth.template.html
+-rw-rw-rw-   0        0        0    17347 2023-07-03 02:51:20.000000 gramex-1.92.1/gramex/handlers/authhandler.py
+-rw-rw-rw-   0        0        0    65464 2023-07-06 20:38:13.000000 gramex-1.92.1/gramex/handlers/basehandler.py
+-rw-rw-rw-   0        0        0    15771 2023-06-08 09:27:24.000000 gramex-1.92.1/gramex/handlers/capturehandler.py
+-rw-rw-rw-   0        0        0     6643 2023-07-06 20:35:09.000000 gramex-1.92.1/gramex/handlers/chatgpthandler.py
+-rw-rw-rw-   0        0        0     1477 2023-06-08 09:04:46.000000 gramex-1.92.1/gramex/handlers/comichandler.py
+-rw-rw-rw-   0        0        0     8904 2023-06-17 00:11:07.000000 gramex-1.92.1/gramex/handlers/drivehandler.py
+-rw-rw-rw-   0        0        0    14917 2023-07-02 06:16:31.000000 gramex-1.92.1/gramex/handlers/filehandler.py
+-rw-rw-rw-   0        0        0     1271 2022-07-03 06:28:09.000000 gramex-1.92.1/gramex/handlers/filehandler.template.html
+-rw-rw-rw-   0        0        0      198 2023-05-13 04:30:57.000000 gramex-1.92.1/gramex/handlers/filterhandler.py
+-rw-rw-rw-   0        0        0    13125 2023-06-19 14:23:49.000000 gramex-1.92.1/gramex/handlers/formhandler.py
+-rw-rw-rw-   0        0        0     3774 2023-06-08 09:04:46.000000 gramex-1.92.1/gramex/handlers/functionhandler.py
+-rw-rw-rw-   0        0        0     6706 2023-06-08 09:27:24.000000 gramex-1.92.1/gramex/handlers/jsonhandler.py
+-rw-rw-rw-   0        0        0     6838 2023-05-13 04:30:57.000000 gramex-1.92.1/gramex/handlers/messagehandler.py
+-rw-rw-rw-   0        0        0    16154 2023-06-02 05:59:12.000000 gramex-1.92.1/gramex/handlers/mlhandler.py
+-rw-rw-rw-   0        0        0     7492 2023-06-08 09:04:46.000000 gramex-1.92.1/gramex/handlers/modelhandler.py
+-rw-rw-rw-   0        0        0     1413 2022-11-02 08:06:17.000000 gramex-1.92.1/gramex/handlers/openapiconfig.yaml
+-rw-rw-rw-   0        0        0     7326 2023-07-02 06:16:31.000000 gramex-1.92.1/gramex/handlers/openapihandler.py
+-rw-rw-rw-   0        0        0      818 2023-06-08 09:04:46.000000 gramex-1.92.1/gramex/handlers/pptxhandler.py
+-rw-rw-rw-   0        0        0     5145 2023-06-08 09:27:24.000000 gramex-1.92.1/gramex/handlers/processhandler.py
+-rw-rw-rw-   0        0        0     7882 2023-06-08 09:27:24.000000 gramex-1.92.1/gramex/handlers/proxyhandler.py
+-rw-rw-rw-   0        0        0     1362 2022-10-17 06:55:24.000000 gramex-1.92.1/gramex/handlers/queryhandler.template.html
+-rw-rw-rw-   0        0        0    11338 2023-06-08 09:27:24.000000 gramex-1.92.1/gramex/handlers/socialhandler.py
+-rw-rw-rw-   0        0        0     9434 2023-06-08 09:27:24.000000 gramex-1.92.1/gramex/handlers/uploadhandler.py
+-rw-rw-rw-   0        0        0     2121 2022-11-23 03:19:45.000000 gramex-1.92.1/gramex/handlers/websockethandler.py
+-rw-rw-rw-   0        0        0     1458 2023-05-13 04:30:57.000000 gramex-1.92.1/gramex/http.py
+-rw-rw-rw-   0        0        0    35069 2023-06-17 00:40:29.000000 gramex-1.92.1/gramex/install.py
+-rw-rw-rw-   0        0        0     2086 2022-09-13 04:40:51.000000 gramex-1.92.1/gramex/license.py
+-rw-rw-rw-   0        0        0     2005 2023-05-13 04:30:57.000000 gramex-1.92.1/gramex/migrate.py
+-rw-rw-rw-   0        0        0    18629 2023-06-08 09:27:24.000000 gramex-1.92.1/gramex/ml.py
+-rw-rw-rw-   0        0        0    13687 2022-11-02 08:06:17.000000 gramex-1.92.1/gramex/ml_api.py
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:37.921460 gramex-1.92.1/gramex/pptgen/
+-rw-rw-rw-   0        0        0     9967 2023-06-08 09:27:24.000000 gramex-1.92.1/gramex/pptgen/__init__.py
+-rw-rw-rw-   0        0        0    18868 2023-06-08 09:27:24.000000 gramex-1.92.1/gramex/pptgen/color.py
+-rw-rw-rw-   0        0        0     7779 2018-01-31 16:40:23.000000 gramex-1.92.1/gramex/pptgen/colors.json
+-rw-rw-rw-   0        0        0    45490 2022-11-02 08:06:17.000000 gramex-1.92.1/gramex/pptgen/commands.py
+-rw-rw-rw-   0        0        0     6351 2018-01-31 16:40:23.000000 gramex-1.92.1/gramex/pptgen/fonts.json
+-rw-rw-rw-   0        0        0     1304 2022-11-02 08:06:18.000000 gramex-1.92.1/gramex/pptgen/fontwidth.py
+-rw-rw-rw-   0        0        0    26250 2023-06-08 09:27:24.000000 gramex-1.92.1/gramex/pptgen/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:37.990100 gramex-1.92.1/gramex/pptgen2/
+-rw-rw-rw-   0        0        0    23438 2023-06-08 09:27:24.000000 gramex-1.92.1/gramex/pptgen2/__init__.py
+-rw-rw-rw-   0        0        0    34432 2023-06-08 09:27:24.000000 gramex-1.92.1/gramex/pptgen2/commands.py
+-rw-rw-rw-   0        0        0    12068 2022-11-02 08:06:18.000000 gramex-1.92.1/gramex/pptgen2/config.yaml
+-rw-rw-rw-   0        0        0     4278 2023-06-08 09:27:24.000000 gramex-1.92.1/gramex/pynode.py
+-rw-rw-rw-   0        0        0     2979 2023-06-08 09:27:24.000000 gramex-1.92.1/gramex/scale.py
+-rw-rw-rw-   0        0        0     1057 2022-11-02 08:06:18.000000 gramex-1.92.1/gramex/secrets.py
+-rw-rw-rw-   0        0        0     2508 2022-11-02 08:06:18.000000 gramex-1.92.1/gramex/servicenow.yaml
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:38.140261 gramex-1.92.1/gramex/services/
+-rw-rw-rw-   0        0        0    39783 2023-07-04 08:07:56.000000 gramex-1.92.1/gramex/services/__init__.py
+-rw-rw-rw-   0        0        0    11451 2023-07-02 06:16:31.000000 gramex-1.92.1/gramex/services/emailer.py
+-rw-rw-rw-   0        0        0     3724 2023-07-02 06:16:31.000000 gramex-1.92.1/gramex/services/rediscache.py
+-rw-rw-rw-   0        0        0     7164 2023-05-13 04:30:57.000000 gramex-1.92.1/gramex/services/scheduler.py
+-rw-rw-rw-   0        0        0     3684 2023-06-08 09:27:24.000000 gramex-1.92.1/gramex/services/sms.py
+-rw-rw-rw-   0        0        0     6385 2023-05-13 04:30:57.000000 gramex-1.92.1/gramex/services/ttlcache.py
+-rw-rw-rw-   0        0        0     4521 2023-06-27 08:54:47.000000 gramex-1.92.1/gramex/services/urlcache.py
+-rw-rw-rw-   0        0        0     5822 2023-06-08 09:27:24.000000 gramex-1.92.1/gramex/services/watcher.py
+-rw-rw-rw-   0        0        0     3831 2022-11-02 08:06:18.000000 gramex-1.92.1/gramex/sm_api.py
+-rw-rw-rw-   0        0        0     8638 2022-11-02 08:06:18.000000 gramex-1.92.1/gramex/topcause.py
+-rw-rw-rw-   0        0        0     8710 2022-11-02 08:06:18.000000 gramex-1.92.1/gramex/transformers.py
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:38.261883 gramex-1.92.1/gramex/transforms/
+-rw-rw-rw-   0        0        0      787 2023-07-02 06:16:31.000000 gramex-1.92.1/gramex/transforms/__init__.py
+-rw-rw-rw-   0        0        0     1658 2022-09-13 04:40:51.000000 gramex-1.92.1/gramex/transforms/auth.py
+-rw-rw-rw-   0        0        0     3022 2023-07-02 06:16:31.000000 gramex-1.92.1/gramex/transforms/template.py
+-rw-rw-rw-   0        0        0    32960 2023-06-19 14:23:49.000000 gramex-1.92.1/gramex/transforms/transforms.py
+-rw-rw-rw-   0        0        0    10095 2023-06-08 09:27:24.000000 gramex-1.92.1/gramex/transforms/twitterstream.py
+-rw-rw-rw-   0        0        0     6808 2022-11-13 04:18:56.000000 gramex-1.92.1/gramex/winservice.py
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:34.691086 gramex-1.92.1/gramex.egg-info/
+-rw-rw-rw-   0        0        0     2956 2023-07-06 20:39:31.000000 gramex-1.92.1/gramex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    12004 2023-07-06 20:39:34.000000 gramex-1.92.1/gramex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 20:39:31.000000 gramex-1.92.1/gramex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      123 2023-07-06 20:39:31.000000 gramex-1.92.1/gramex.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      953 2023-07-06 20:39:31.000000 gramex-1.92.1/gramex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-06 20:39:31.000000 gramex-1.92.1/gramex.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6171 2023-07-06 20:38:13.000000 gramex-1.92.1/pyproject.toml
+-rw-rw-rw-   0        0        0      503 2023-07-06 20:39:39.060918 gramex-1.92.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-06 20:39:39.042465 gramex-1.92.1/tests/
+-rw-rw-rw-   0        0        0     5233 2022-11-06 08:24:18.000000 gramex-1.92.1/tests/test_admin.py
+-rw-rw-rw-   0        0        0     9054 2023-04-18 08:45:54.000000 gramex-1.92.1/tests/test_alerts.py
+-rw-rw-rw-   0        0        0     3981 2022-11-06 08:24:18.000000 gramex-1.92.1/tests/test_args.py
+-rw-rw-rw-   0        0        0    39128 2023-06-19 14:23:49.000000 gramex-1.92.1/tests/test_auth.py
+-rw-rw-rw-   0        0        0    14612 2022-11-06 08:24:18.000000 gramex-1.92.1/tests/test_cache.py
+-rw-rw-rw-   0        0        0    15062 2023-05-13 04:30:57.000000 gramex-1.92.1/tests/test_capturehandler.py
+-rw-rw-rw-   0        0        0     1288 2022-11-06 08:24:19.000000 gramex-1.92.1/tests/test_comichandler.py
+-rw-rw-rw-   0        0        0    12571 2023-06-19 14:23:49.000000 gramex-1.92.1/tests/test_drivehandler.py
+-rw-rw-rw-   0        0        0    17308 2023-07-02 06:16:31.000000 gramex-1.92.1/tests/test_filehandler.py
+-rw-rw-rw-   0        0        0     6797 2023-05-13 04:30:57.000000 gramex-1.92.1/tests/test_filterhandler.py
+-rw-rw-rw-   0        0        0    35746 2023-05-27 08:02:33.000000 gramex-1.92.1/tests/test_formhandler.py
+-rw-rw-rw-   0        0        0     8784 2022-11-06 08:24:22.000000 gramex-1.92.1/tests/test_functionhandler.py
+-rw-rw-rw-   0        0        0     3201 2022-11-06 08:24:22.000000 gramex-1.92.1/tests/test_gramexlog.py
+-rw-rw-rw-   0        0        0    19008 2023-06-19 14:23:49.000000 gramex-1.92.1/tests/test_handlers.py
+-rw-rw-rw-   0        0        0     1475 2022-11-02 08:06:18.000000 gramex-1.92.1/tests/test_init.py
+-rw-rw-rw-   0        0        0     8931 2023-05-13 04:30:57.000000 gramex-1.92.1/tests/test_install.py
+-rw-rw-rw-   0        0        0     6361 2022-11-06 08:24:23.000000 gramex-1.92.1/tests/test_jsonhandler.py
+-rw-rw-rw-   0        0        0     3896 2022-11-06 08:24:23.000000 gramex-1.92.1/tests/test_ldapauth.py
+-rw-rw-rw-   0        0        0     7519 2022-11-02 08:06:18.000000 gramex-1.92.1/tests/test_logviewer.py
+-rw-rw-rw-   0        0        0    32878 2022-11-23 04:49:14.000000 gramex-1.92.1/tests/test_mlhandler.py
+-rw-rw-rw-   0        0        0     4745 2022-11-02 08:06:18.000000 gramex-1.92.1/tests/test_modelhandler.py
+-rw-rw-rw-   0        0        0     7082 2023-05-13 04:30:57.000000 gramex-1.92.1/tests/test_openapihandler.py
+-rw-rw-rw-   0        0        0     1411 2022-11-02 08:06:18.000000 gramex-1.92.1/tests/test_pptxhandler.py
+-rw-rw-rw-   0        0        0     3530 2022-11-06 08:24:24.000000 gramex-1.92.1/tests/test_processhandler.py
+-rw-rw-rw-   0        0        0     3834 2022-11-06 08:24:24.000000 gramex-1.92.1/tests/test_proxyhandler.py
+-rw-rw-rw-   0        0        0     1527 2022-11-02 08:06:18.000000 gramex-1.92.1/tests/test_pynode.py
+-rw-rw-rw-   0        0        0     1220 2022-11-06 08:24:24.000000 gramex-1.92.1/tests/test_schedule.py
+-rw-rw-rw-   0        0        0      757 2022-02-19 10:03:06.000000 gramex-1.92.1/tests/test_secrets.py
+-rw-rw-rw-   0        0        0      330 2020-05-27 03:04:19.000000 gramex-1.92.1/tests/test_sms.py
+-rw-rw-rw-   0        0        0      180 2017-08-29 07:52:03.000000 gramex-1.92.1/tests/test_subapp.py
+-rw-rw-rw-   0        0        0     5382 2022-11-02 08:06:18.000000 gramex-1.92.1/tests/test_subprocess.py
+-rw-rw-rw-   0        0        0     2277 2022-11-02 08:06:18.000000 gramex-1.92.1/tests/test_translater.py
+-rw-rw-rw-   0        0        0     2895 2022-11-06 08:24:24.000000 gramex-1.92.1/tests/test_twitterresthandler.py
+-rw-rw-rw-   0        0        0     2352 2022-11-06 08:24:24.000000 gramex-1.92.1/tests/test_ui.py
+-rw-rw-rw-   0        0        0     2359 2022-11-02 08:06:18.000000 gramex-1.92.1/tests/test_update.py
+-rw-rw-rw-   0        0        0     6563 2022-11-06 08:24:25.000000 gramex-1.92.1/tests/test_uploadhandler.py
+-rw-rw-rw-   0        0        0     1966 2022-11-02 08:06:18.000000 gramex-1.92.1/tests/test_watcher.py
+-rw-rw-rw-   0        0        0     2647 2022-11-06 08:24:25.000000 gramex-1.92.1/tests/test_websockethandler.py
```

### Comparing `gramex-1.92.0/.gitignore` & `gramex-1.92.1/.gitignore`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/LICENSE` & `gramex-1.92.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/MANIFEST.in` & `gramex-1.92.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/PKG-INFO` & `gramex-1.92.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gramex
-Version: 1.92.0
+Version: 1.92.1
 Summary: Gramex: Low Code Data Solutions Platform
 Author-email: Anand S <s.anand@gramener.com>, Pratap Vardhan <pratapapvr@gmail.com>, Jaidev Deshpande <jaidev.deshpande@gramener.com>, Bhanu Kamapantula <talk2kish@gmail.com>, Radheya Kale <radheya.kale@gramener.com>, Karmanya Aggarwal <karmanyaaggarwal@gmail.com>, Sandeep Bhat <sandeep.bhat@gramener.com>, Shraddheya Shrivastava <shraddheya.shrivastava@gramener.com>, Sundeep Reddy Mallu <sundeep.mally@gramener.com>
 License: MIT
 Project-URL: Homepage, https://gramener.com/gramex/
 Project-URL: Documentation, https://gramener.com/gramex/guide/
 Project-URL: Repository, https://github.com/gramener/gramex
 Project-URL: Changelog, https://gramener.com/gramex/guide/release/
```

### Comparing `gramex-1.92.0/README.md` & `gramex-1.92.1/README.md`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/__init__.py` & `gramex-1.92.1/gramex/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 gramex install                Install an app
 gramex update                 Update an app
 gramex setup                  Run make, npm install, bower install etc on app
 gramex run                    Run an installed app
 gramex uninstall              Uninstall an app
 '''
 
-__version__ = '1.92.0'
+__version__ = '1.92.1'
 
 paths = AttrDict()  # Paths where configurations are stored
 conf = AttrDict()  # Final merged configurations
 config_layers = ChainConfig()  # Loads all configurations. init() updates it
 appconfig = AttrDict()  # Final app configuration
 
 paths['source'] = Path(__file__).absolute().parent  # Where gramex source code is
```

### Comparing `gramex-1.92.0/gramex/apps/admin2/gramex.yaml` & `gramex-1.92.1/gramex/apps/admin2/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/admin2/gramexadmin.py` & `gramex-1.92.1/gramex/apps/admin2/gramexadmin.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/admin2/index.html` & `gramex-1.92.1/gramex/apps/admin2/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/admin2/schedule.js` & `gramex-1.92.1/gramex/apps/admin2/schedule.js`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/capture/README.md` & `gramex-1.92.1/gramex/apps/capture/README.md`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/capture/capture.js` & `gramex-1.92.1/gramex/apps/capture/capture.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -142,43 +142,46 @@
             console.log("console.log:" + msg);
         };
     }
 
     // Open the page
     console.log("Opening", q.url);
     page.open(q.url, function(status) {
-        setTimeout(function() {
-            error.status = status;
-            if (status == "fail") return callback();
-            // If a selector is specified (for images), set the clipRect.
-            if (q.selector) {
-                var clipRect = page.evaluate(function(selector) {
-                    var query = document.querySelector(selector);
-                    if (query) return query.getBoundingClientRect();
-                }, decodeURIComponent(q.selector));
-                if (clipRect) {
-                    page.clipRect = {
-                        top: clipRect.top,
-                        left: clipRect.left,
-                        width: clipRect.width,
-                        height: clipRect.height,
-                    };
+        setTimeout(
+            function() {
+                error.status = status;
+                if (status == "fail") return callback();
+                // If a selector is specified (for images), set the clipRect.
+                if (q.selector) {
+                    var clipRect = page.evaluate(function(selector) {
+                        var query = document.querySelector(selector);
+                        if (query) return query.getBoundingClientRect();
+                    }, decodeURIComponent(q.selector));
+                    if (clipRect) {
+                        page.clipRect = {
+                            top: clipRect.top,
+                            left: clipRect.left,
+                            width: clipRect.width,
+                            height: clipRect.height,
+                        };
+                    }
                 }
-            }
-            if (q.js) {
-                var js = decodeURIComponent(q.js);
-                if (q.js.match(/^http/)) page.includeJs(js, save);
-                else {
-                    fs.write("inject.js", js, "w");
-                    if (!page.injectJs("inject.js")) console.log("Failed to inject JS");
-                    save();
-                    fs.remove("inject.js");
-                }
-            } else save();
-        }, parseFloat(q.delay || 0));
+                if (q.js) {
+                    var js = decodeURIComponent(q.js);
+                    if (q.js.match(/^http/)) page.includeJs(js, save);
+                    else {
+                        fs.write("inject.js", js, "w");
+                        if (!page.injectJs("inject.js")) console.log("Failed to inject JS");
+                        save();
+                        fs.remove("inject.js");
+                    }
+                } else save();
+            },
+            parseFloat(q.delay || 0),
+        );
     });
 }
 
 var homepage = (function(script) {
     var parts = script.split(/[/\\]/);
     parts[parts.length - 1] = "index.html";
     return parts.join("/");
@@ -194,15 +197,15 @@
     var q = parseUri(
         request.postRaw ?
         "/?" + request.postRaw :
         request.post ?
         "/?" + request.post :
         phantom_version >= "2.0.1" ?
         decodeURIComponent(request.url) :
-        request.url
+        request.url,
     ).queryKey;
     /* eslint-enable indent */
     if (!q.url) {
         response.statusCode = 200;
         response.headers = {
             "Content-Type": "text/html",
             Server: server_version,
@@ -258,15 +261,15 @@
         if (listening) {
             console.log(
                 "PhantomJS:",
                 phantom_version,
                 "capture.js:",
                 version,
                 "port:",
-                port
+                port,
             );
         } else {
             console.log("Could not bind to port", port);
             phantom.exit(1);
         }
     } else {
         render(args, function() {
```

### Comparing `gramex-1.92.0/gramex/apps/capture/chromecapture.js` & `gramex-1.92.1/gramex/apps/capture/chromecapture.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -120,29 +120,29 @@
       width:100%">${s}</div>`;
     }
     if (q.header || q.headerTemplate || q.footer || q.footerTemplate) {
         // For zoom: TODO: https://stackoverflow.com/a/51461829/100904
         // If displayHeaderFooter, headerTemplate and footerTemplate MUST BOTH be present
         pdf_options.displayHeaderFooter = true;
         pdf_options.headerTemplate = template_wrap(
-            q.headerTemplate || templatize(q.header || "")
+            q.headerTemplate || templatize(q.header || ""),
         );
         pdf_options.footerTemplate = template_wrap(
-            q.footerTemplate || templatize(q.footer || "")
+            q.footerTemplate || templatize(q.footer || ""),
         );
         // Increase default margin if header / footer is present
         if (q.header || q.headerTemplate)
             pdf_options.margin.top = pdf_options.margin.top || "2cm";
         if (q.footer || q.footerTemplate)
             pdf_options.margin.bottom = pdf_options.margin.bottom || "2cm";
     }
     // Default to 1cm margin if none was specified
     _.each(
         margin_keys,
-        (key) => (pdf_options.margin[key] = pdf_options.margin[key] || "1cm")
+        (key) => (pdf_options.margin[key] = pdf_options.margin[key] || "1cm"),
     );
     let args = [
         "--no-sandbox",
         "--disable-setuid-sandbox",
         "--ignore-certificate-errors",
     ];
     // If a proxy environment variable is defined, use it
@@ -152,27 +152,27 @@
 
     if (typeof browser == "undefined") browser = await browser_setup(args);
 
     let page = await browser.newPage();
 
     page
         .on("console", (message) =>
-            console.log(`${message.type().toUpperCase()} ${message.text()}`)
+            console.log(`${message.type().toUpperCase()} ${message.text()}`),
         )
         .on("pageerror", (error) => console.log(`ERROR: ${error.message}`))
         .on("response", (response) => {
             if (response.status() >= 400)
                 console.log(
                     `HTTP ${response.status()}: ${response
             .request()
-            .method()} ${response.url()}`
+            .method()} ${response.url()}`,
                 );
         })
         .on("requestfailed", (request) =>
-            console.log(`${request.failure().errorText}: ${request.url()}`)
+            console.log(`${request.failure().errorText}: ${request.url()}`),
         );
 
     // Clear past cookies
     let cookies = await page.cookies(q.url);
     await page.deleteCookie(...cookies);
     // Parse cookies and set them on the page, so that they'll be sent on any
     // requests to this URL. (This overrides the request HTTP header "Cookie")
@@ -242,15 +242,15 @@
             const image_files = [];
             let pages = _.zip(
                 q.selector,
                 q.title,
                 q.title_size,
                 q.x,
                 q.y,
-                q.dpi
+                q.dpi,
             ).entries();
             for (const [index, [selector, title, title_size, x, y, dpi]] of pages) {
                 options.path = target.replace(/\.pptx$/, "." + index + ".png");
                 image_files.push(options.path);
                 await screenshot(page, options, selector);
                 const fmt = pptx_size[q.layout in pptx_size ? q.layout : "4x3"];
                 // 72 points = 1 inch
@@ -302,26 +302,26 @@
 
     let q = Object.assign({
             ext: "pdf",
             media: "screen",
             cookie: req.headers.cookie
         },
         req.query,
-        req.body
+        req.body,
     );
     if (!q.url) return res.sendFile(homepage);
     if (!q.ext.match(/pdf|png|jpg|jpeg|pptx/i))
         return error(400, `Invalid ext=${q.ext}.`);
     q.headers = req.headers;
     render(q)
         .then((info) => {
             if (fs.existsSync(info.path)) {
                 res.setHeader(
                     "Content-Disposition",
-                    "attachment; filename=" + info.file
+                    "attachment; filename=" + info.file,
                 );
                 res.sendFile(info.path, (err) => {
                     if (err) console.error("Error sending file", err);
                     fs.unlinkSync(info.path);
                 });
             } else error(500, `'Missing output file`, info.path);
         })
```

### Comparing `gramex-1.92.0/gramex/apps/capture/index.html` & `gramex-1.92.1/gramex/apps/capture/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/capture/package-lock.json` & `gramex-1.92.1/gramex/apps/capture/package-lock.json`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/capture/package.json` & `gramex-1.92.1/gramex/apps/capture/package.json`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/filemanager/README.html` & `gramex-1.92.1/gramex/apps/filemanager/README.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/filemanager/drivehandler-snippet.html` & `gramex-1.92.1/gramex/apps/filemanager/drivehandler-snippet.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/filemanager/filemanager-snippet.html` & `gramex-1.92.1/gramex/apps/filemanager/filemanager-snippet.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/filemanager/filemanager.html` & `gramex-1.92.1/gramex/apps/filemanager/filemanager.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/filemanager/filemanager.js` & `gramex-1.92.1/gramex/apps/filemanager/filemanager.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -29,23 +29,23 @@
             .on("load", function() {
                 let btn = $(this).find(".uploadbtn").get(0);
                 attach_dropzone(
                     btn,
                     el,
                     el.dataset.src,
                     true,
-                    renderTable.bind(this, el, opts)
+                    renderTable.bind(this, el, opts),
                 );
                 // Attach a dropzone to the whole element
                 attach_dropzone(
                     el,
                     el,
                     el.dataset.src,
                     false,
-                    renderTable.bind(this, el, opts)
+                    renderTable.bind(this, el, opts),
                 );
             })
             .formhandler(opts);
     }
 
     function attach_dropzone(el, parent, url, clickable = true, success = null) {
         try {
```

### Comparing `gramex-1.92.0/gramex/apps/filemanager/filemanager.py` & `gramex-1.92.1/gramex/apps/filemanager/filemanager.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/filemanager/gramex.yaml` & `gramex-1.92.1/gramex/apps/filemanager/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/filemanager/index.html` & `gramex-1.92.1/gramex/apps/filemanager/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/filemanager/navbar.html` & `gramex-1.92.1/gramex/apps/filemanager/navbar.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/init/default/.eslintrc.yml` & `gramex-1.92.1/gramex/apps/init/default/.eslintrc.yml`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/init/default/.gitlab-ci.yml` & `gramex-1.92.1/gramex/apps/init/default/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/init/default/.template.gitignore` & `gramex-1.92.1/gramex/apps/init/default/.template.gitignore`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/init/default/assets/README.template.md` & `gramex-1.92.1/gramex/apps/init/default/assets/README.template.md`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/init/default/gramex.template.yaml` & `gramex-1.92.1/gramex/apps/init/default/gramex.template.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/init/default/index.template.html` & `gramex-1.92.1/gramex/apps/init/default/index.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/init/default/js/README.template.md` & `gramex-1.92.1/gramex/apps/init/default/js/README.template.md`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/init/default/login.template.html` & `gramex-1.92.1/gramex/apps/init/default/login.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/init/default/template-navbar.template.html` & `gramex-1.92.1/gramex/apps/init/default/template-navbar.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/init/ide/index.template.html` & `gramex-1.92.1/gramex/apps/init/ide/index.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/init/minimal/index.template.html` & `gramex-1.92.1/gramex/apps/init/minimal/index.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/languagetool/README.md` & `gramex-1.92.1/gramex/apps/languagetool/README.md`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/languagetool/gramex.yaml` & `gramex-1.92.1/gramex/apps/languagetool/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/logviewer/config.yaml` & `gramex-1.92.1/gramex/apps/logviewer/config.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/logviewer/gramex.yaml` & `gramex-1.92.1/gramex/apps/logviewer/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/logviewer/index.html` & `gramex-1.92.1/gramex/apps/logviewer/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/logviewer/logviewer.py` & `gramex-1.92.1/gramex/apps/logviewer/logviewer.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/logviewer/lv-datepicker.html` & `gramex-1.92.1/gramex/apps/logviewer/lv-datepicker.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/logviewer/package-lock.json` & `gramex-1.92.1/gramex/apps/logviewer/package-lock.json`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/logviewer/render.js` & `gramex-1.92.1/gramex/apps/logviewer/render.js`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/logviewer/script.js` & `gramex-1.92.1/gramex/apps/logviewer/script.js`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/mail/index.html` & `gramex-1.92.1/gramex/apps/mail/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/mlhandler/template.html` & `gramex-1.92.1/gramex/apps/mlhandler/template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/pynode/index.js` & `gramex-1.92.1/gramex/apps/pynode/index.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -17,15 +17,15 @@
         JSON.stringify({
             error: {
                 name: error.name,
                 message: error.message,
                 stack: error.stack,
             },
             result: null,
-        })
+        }),
     );
 }
 
 // Return a function that sends the passed result to the websocket as JSON.
 // If not parseable as JSON, send an error message to the websocket.
 function callback(ws) {
     return (result) => {
@@ -50,15 +50,15 @@
         // Within the code, "this" refers to the context global
         const result = fn.apply(context, values);
         // If the code didn't return anything, return null
         ws.send(
             JSON.stringify({
                 error: null,
                 result: typeof result == "undefined" ? null : result,
-            })
+            }),
         );
     } catch (e) {
         send_error(e, ws);
     }
 }
 
 function main() {
@@ -70,15 +70,15 @@
         // Localhost can be ::::ffff:127.0.0.1 (IPv6) or 127.0.0.1 (IPv4) or '::1'
         verifyClient: (info) =>
             info.req.connection.remoteAddress.match(/\b127.0.0.1$|^::1$/),
     });
 
     // Print a message indicating versions. pynode.py EXPLICITLY checks for this message.
     console.log(
-        `node.js: ${process.version} pynode: ${package.version} port: ${port} pid: ${process.pid} cwd: ${cwd}`
+        `node.js: ${process.version} pynode: ${package.version} port: ${port} pid: ${process.pid} cwd: ${cwd}`,
     );
 
     // Set up the websocket server
     wss.on("connection", (ws) => {
         ws.on("message", (message) => {
             "use strict";
             let exec;
@@ -125,21 +125,21 @@
                     }
                 } else execute(ws, code, args, values);
             } else if (exec.path)
                 send_error({
                         name: "Unsupported argument",
                         message: "path= is not yet supported",
                     },
-                    ws
+                    ws,
                 );
             else
                 send_error({
                         name: "Missing arguments",
                         message: "Need code= or path="
                     },
-                    ws
+                    ws,
                 );
         });
     });
 }
 
 main();
```

### Comparing `gramex-1.92.0/gramex/apps/pynode/package-lock.json` & `gramex-1.92.1/gramex/apps/pynode/package-lock.json`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/.snyk` & `gramex-1.92.1/gramex/apps/ui/.snyk`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/__init__.py` & `gramex-1.92.1/gramex/apps/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/bootstrap-theme.scss` & `gramex-1.92.1/gramex/apps/ui/bootstrap-theme.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/config.yaml` & `gramex-1.92.1/gramex/apps/ui/config.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/gramex.yaml` & `gramex-1.92.1/gramex/apps/ui/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/gramexui.scss` & `gramex-1.92.1/gramex/apps/ui/gramexui.scss`

 * *Files 0% similar despite different names*

```diff
@@ -1059,15 +1059,17 @@
     left: 0;
     pointer-events: none;
     background-image: radial-gradient(circle, #000 10%, transparent 10%);
     background-repeat: no-repeat;
     background-position: 50%;
     opacity: 0;
     transform: scale(10, 10);
-    transition: transform $ripple-duration, opacity $ripple-duration * 2;
+    transition:
+      transform $ripple-duration,
+      opacity $ripple-duration * 2;
   }
   &:active:after {
     transform: scale(0, 0);
     opacity: $ripple-opacity;
     transition: 0s;
   }
 }
```

### Comparing `gramex-1.92.0/gramex/apps/ui/package-lock.json` & `gramex-1.92.1/gramex/apps/ui/package-lock.json`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/setup.js` & `gramex-1.92.1/gramex/apps/ui/setup.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -15,26 +15,26 @@
 // https://bootswatch.com/
 // For each bootswatch/dist/<theme>/ directory, add a theme/bootswatch/<theme>.scss that imports
 // variables.scss and bootswatch.scss files, with Bootstrap sandwiched in-between.
 const bootswatch_root = path.join(
     __dirname,
     "node_modules",
     "bootswatch",
-    "dist"
+    "dist",
 );
 const bootswatch_target = mkdir(theme_dir, "bootswatch");
 fs.readdirSync(bootswatch_root).forEach(function(theme) {
     const target = path.join(bootswatch_target, theme + ".scss");
     fs.writeFileSync(
         target,
         `// https://bootswatch.com/${theme}/
 @import "node_modules/bootswatch/dist/${theme}/variables";
 @import "gramexui";
 @import "node_modules/bootswatch/dist/${theme}/bootswatch";
-`
+`,
     );
     themes.push(`bootswatch/${theme}`);
 });
 
 // http://bootstrap.themes.guide/
 // For each bootstrap-theme/src/<theme>/theme.scss, add a theme/themes-guide/<theme>.scss
 // replacing the @import bootstrap with gramexui
@@ -53,29 +53,29 @@
     if (fs.existsSync(theme_file)) {
         fs.writeFileSync(
             path.join(themes_guide_target, `${dir}.scss`),
             fs
             .readFileSync(theme_file, "utf8")
             .replace('@import "bootstrap";', '@import "gramexui";')
             // Themes Guide disables grid classes. But we want to use them, so kill this line
-            .replace("$enable-grid-classes:false;\n", "") + "\n"
+            .replace("$enable-grid-classes:false;\n", "") + "\n",
         );
         themes.push(`themes-guide/${dir}`);
     }
 });
 execSync("rm -rf bootstrap-themes", {
     cwd: tmp
 });
 
 // Save list of themes
 fs.writeFileSync(
     "theme/themes.json",
     JSON.stringify({
         themes: themes
-    }) + "\n"
+    }) + "\n",
 );
 
 // Utility functions
 // --------------------------------------------------------------------
 function mkdir(...dirs) {
     const dir = path.join(...dirs);
     if (!fs.existsSync(dir)) fs.mkdirSync(dir);
```

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/bootstrap5.scss` & `gramex-1.92.1/gramex/apps/ui/theme/bootstrap5.scss`

 * *Files 1% similar despite different names*

```diff
@@ -838,15 +838,17 @@
     left: 0;
     pointer-events: none;
     background-image: radial-gradient(circle, #000 10%, transparent 10%);
     background-repeat: no-repeat;
     background-position: 50%;
     opacity: 0;
     transform: scale(10, 10);
-    transition: transform $ripple-duration, opacity $ripple-duration * 2;
+    transition:
+      transform $ripple-duration,
+      opacity $ripple-duration * 2;
   }
   &:active:after {
     transform: scale(0, 0);
     opacity: $ripple-opacity;
     transition: 0s;
   }
 }
```

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/cerulean.png` & `gramex-1.92.1/gramex/apps/ui/theme/bootswatch/cerulean.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/cosmo.png` & `gramex-1.92.1/gramex/apps/ui/theme/bootswatch/cosmo.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/cyborg.png` & `gramex-1.92.1/gramex/apps/ui/theme/bootswatch/cyborg.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/darkly.png` & `gramex-1.92.1/gramex/apps/ui/theme/bootswatch/darkly.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/flatly.png` & `gramex-1.92.1/gramex/apps/ui/theme/bootswatch/flatly.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/journal.png` & `gramex-1.92.1/gramex/apps/ui/theme/bootswatch/journal.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/litera.png` & `gramex-1.92.1/gramex/apps/ui/theme/bootswatch/litera.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/lumen.png` & `gramex-1.92.1/gramex/apps/ui/theme/bootswatch/lumen.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/lux.png` & `gramex-1.92.1/gramex/apps/ui/theme/bootswatch/lux.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/materia.png` & `gramex-1.92.1/gramex/apps/ui/theme/bootswatch/materia.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/minty.png` & `gramex-1.92.1/gramex/apps/ui/theme/bootswatch/minty.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/pulse.png` & `gramex-1.92.1/gramex/apps/ui/theme/bootswatch/pulse.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/sandstone.png` & `gramex-1.92.1/gramex/apps/ui/theme/bootswatch/sandstone.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/simplex.png` & `gramex-1.92.1/gramex/apps/ui/theme/bootswatch/simplex.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/sketchy.png` & `gramex-1.92.1/gramex/apps/ui/theme/bootswatch/sketchy.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/slate.png` & `gramex-1.92.1/gramex/apps/ui/theme/bootswatch/slate.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/solar.png` & `gramex-1.92.1/gramex/apps/ui/theme/bootswatch/solar.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/spacelab.png` & `gramex-1.92.1/gramex/apps/ui/theme/bootswatch/spacelab.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/superhero.png` & `gramex-1.92.1/gramex/apps/ui/theme/bootswatch/superhero.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/united.png` & `gramex-1.92.1/gramex/apps/ui/theme/bootswatch/united.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/bootswatch/yeti.png` & `gramex-1.92.1/gramex/apps/ui/theme/bootswatch/yeti.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/default.png` & `gramex-1.92.1/gramex/apps/ui/theme/default.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/index.html` & `gramex-1.92.1/gramex/apps/ui/theme/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/sample.html` & `gramex-1.92.1/gramex/apps/ui/theme/sample.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/blue_voltage.png` & `gramex-1.92.1/gramex/apps/ui/theme/themes-guide/blue_voltage.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/blue_voltage.scss` & `gramex-1.92.1/gramex/apps/ui/theme/themes-guide/blue_voltage.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/boldstrap.png` & `gramex-1.92.1/gramex/apps/ui/theme/themes-guide/boldstrap.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/bootstrap_purple.png` & `gramex-1.92.1/gramex/apps/ui/theme/themes-guide/bootstrap_purple.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/darkster.png` & `gramex-1.92.1/gramex/apps/ui/theme/themes-guide/darkster.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/darkster.scss` & `gramex-1.92.1/gramex/apps/ui/theme/themes-guide/darkster.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/fresca.png` & `gramex-1.92.1/gramex/apps/ui/theme/themes-guide/fresca.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/greyson.png` & `gramex-1.92.1/gramex/apps/ui/theme/themes-guide/greyson.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/greyson.scss` & `gramex-1.92.1/gramex/apps/ui/theme/themes-guide/greyson.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/hello_kiddie.png` & `gramex-1.92.1/gramex/apps/ui/theme/themes-guide/hello_kiddie.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/hello_kiddie.scss` & `gramex-1.92.1/gramex/apps/ui/theme/themes-guide/hello_kiddie.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/herbie.png` & `gramex-1.92.1/gramex/apps/ui/theme/themes-guide/herbie.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/hootstrap.png` & `gramex-1.92.1/gramex/apps/ui/theme/themes-guide/hootstrap.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/lovey.png` & `gramex-1.92.1/gramex/apps/ui/theme/themes-guide/lovey.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/monotony.png` & `gramex-1.92.1/gramex/apps/ui/theme/themes-guide/monotony.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/poypull.png` & `gramex-1.92.1/gramex/apps/ui/theme/themes-guide/poypull.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/poypull.scss` & `gramex-1.92.1/gramex/apps/ui/theme/themes-guide/poypull.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/signal.png` & `gramex-1.92.1/gramex/apps/ui/theme/themes-guide/signal.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/signal.scss` & `gramex-1.92.1/gramex/apps/ui/theme/themes-guide/signal.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/themes-guide/tequila.png` & `gramex-1.92.1/gramex/apps/ui/theme/themes-guide/tequila.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/ui/theme/themes.json` & `gramex-1.92.1/gramex/apps/ui/theme/themes.json`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/.eslintrc.js` & `gramex-1.92.1/gramex/apps/uifactory/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/assets/data/input.json` & `gramex-1.92.1/gramex/apps/uifactory/assets/data/input.json`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/assets/img/arrows-move.svg` & `gramex-1.92.1/gramex/apps/uifactory/assets/img/arrows-move.svg`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/assets/img/gramener-favicon-blue.png` & `gramex-1.92.1/gramex/apps/uifactory/assets/img/gramener-favicon-blue.png`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/assets/img/trash.svg` & `gramex-1.92.1/gramex/apps/uifactory/assets/img/trash.svg`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/create.html` & `gramex-1.92.1/gramex/apps/uifactory/create.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/edit.html` & `gramex-1.92.1/gramex/apps/uifactory/edit.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/field-actions.html` & `gramex-1.92.1/gramex/apps/uifactory/field-actions.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/form_builder.py` & `gramex-1.92.1/gramex/apps/uifactory/form_builder.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/gramex.yaml` & `gramex-1.92.1/gramex/apps/uifactory/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/index.html` & `gramex-1.92.1/gramex/apps/uifactory/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/js/README.md` & `gramex-1.92.1/gramex/apps/uifactory/js/README.md`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/js/fields.js` & `gramex-1.92.1/gramex/apps/uifactory/js/fields.js`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/js/fork-form.js` & `gramex-1.92.1/gramex/apps/uifactory/js/fork-form.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -32,15 +32,15 @@
                 method: !template ? "POST" : "PUT",
                 data: form_details,
                 success: function(response) {
                     if (!template)
                         $(".toast-body").html("Copy successful. Redirecting to new form.");
                     else
                         $(".toast-body").html(
-                            "Selected form is now a template. Refreshing the list."
+                            "Selected form is now a template. Refreshing the list.",
                         );
                     $(".toast").toast("show");
                     setTimeout(function() {
                         // refresh the forms when an existing form is made a template
                         // else redirect to the newly created form after Copy action
                         if (!template)
                             window.location.href = `${base}/create?id=${response.data.inserted[0].id}`;
```

### Comparing `gramex-1.92.0/gramex/apps/uifactory/js/index.js` & `gramex-1.92.1/gramex/apps/uifactory/js/index.js`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/js/script.js` & `gramex-1.92.1/gramex/apps/uifactory/js/script.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -51,15 +51,15 @@
         method: form_details.method,
         data: form_details.data,
         success: function() {
             $(".post-publish").removeClass("d-none");
         },
         error: function() {
             $(".toast-body").html(
-                "Unable to update the form. Please try again later."
+                "Unable to update the form. Please try again later.",
             );
             $(".toast").toast("show");
         },
         complete: function() {
             $icon.fadeOut();
         },
     });
@@ -73,24 +73,24 @@
     $.ajax("publish", {
         method: form_details.method,
         data: form_details.data,
         success: function(response) {
             form_details.id = response.data.inserted[0].id;
             $(".post-publish").removeClass("d-none");
             $(".form-preview-link").html(
-                `<a class="btn btn-info" href="form/${form_details.id}" target="_blank">Preview</a>`
+                `<a class="btn btn-info" href="form/${form_details.id}" target="_blank">Preview</a>`,
             );
             $(".form-view-link").html(
-                `<a class="btn btn-success" href="view/${form_details.id}" target="_blank">View</a>`
+                `<a class="btn btn-success" href="view/${form_details.id}" target="_blank">View</a>`,
             );
             window.location.href = `create?id=${form_details.id}`;
         },
         error: function() {
             $(".toast-body").html(
-                "Unable to publish the form. Please try again later."
+                "Unable to publish the form. Please try again later.",
             );
             $(".toast").toast("show");
         },
         complete: function() {
             $icon.fadeOut();
         },
     });
@@ -116,28 +116,27 @@
     };
 }
 
 $("body")
     .on("click", "#publish-form", function() {
         let _values = {};
         let $icon = $(
-            '<i class="fa fa-spinner fa-2x fa-fw align-middle"></i>'
+            '<i class="fa fa-spinner fa-2x fa-fw align-middle"></i>',
         ).appendTo(this);
         let _md = {
             name: $("#form-name").val() || "Untitled",
             categories: [],
             description: $("#form-description").val().trim() || "Form description",
         };
 
-        $(".edit-properties > input, .edit-properties > input").each(function(
-            ind,
-            item
-        ) {
-            _values[item.id] = item.value;
-        });
+        $(".edit-properties > input, .edit-properties > input").each(
+            function(ind, item) {
+                _values[item.id] = item.value;
+            },
+        );
         $(".user-form > *").removeClass("highlight");
         $(".edit-properties").empty();
 
         let {
             _form,
             _html
         } = prepare_form_values(_values);
```

### Comparing `gramex-1.92.0/gramex/apps/uifactory/js/utils.js` & `gramex-1.92.1/gramex/apps/uifactory/js/utils.js`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/js/viewform.js` & `gramex-1.92.1/gramex/apps/uifactory/js/viewform.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -37,15 +37,15 @@
                 }, 2000);
             },
         });
     })
     .on("submit", "form.analytics", function(e) {
         e.preventDefault();
         let $icon = $(
-            '<i class="fa fa-spinner fa-2x fa-fw align-middle"></i>'
+            '<i class="fa fa-spinner fa-2x fa-fw align-middle"></i>',
         ).appendTo(this);
         let field_vals = {};
         // $.each($('form').serializeArray(), function() { _vals[this.name] = this.value })
         // above line fails for checkboxes with multiple values, hence the following approach
         let groups = _.groupBy($("form").serializeArray(), "name");
         field_vals = _(groups)
             .map((values, _input) => {
@@ -68,26 +68,26 @@
             for (let key in item) {
                 field_vals_obj[key] = item[key];
             }
         });
 
         $.ajax(
             `../analytics/?db=${form_id}&form_id=${form_id}&response=${encodeURIComponent(
-        JSON.stringify(field_vals_obj)
+        JSON.stringify(field_vals_obj),
       )}`, {
                 method: "POST",
                 success: function() {
                     // submit another record
                     $("#view-form").addClass("d-none");
                     $(".post-submission").removeClass("d-none");
                     $(".toast-body").html("Your response has been recorded.");
                     $(".toast").toast("show");
                 },
                 complete: function() {
                     $icon.fadeOut();
                 },
-            }
+            },
         );
     })
     .on("click", "[data-formaction]", function() {
         if ($(this).data("formaction") === "copy") initiate_copy("..", form_id);
     });
```

### Comparing `gramex-1.92.0/gramex/apps/uifactory/modals/add-field.html` & `gramex-1.92.1/gramex/apps/uifactory/modals/add-field.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/modals/embed.html` & `gramex-1.92.1/gramex/apps/uifactory/modals/embed.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/modals/remove.html` & `gramex-1.92.1/gramex/apps/uifactory/modals/remove.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/modals/rename.html` & `gramex-1.92.1/gramex/apps/uifactory/modals/rename.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/modals/themes.html` & `gramex-1.92.1/gramex/apps/uifactory/modals/themes.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/package-lock.json` & `gramex-1.92.1/gramex/apps/uifactory/package-lock.json`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/popover-form.html` & `gramex-1.92.1/gramex/apps/uifactory/popover-form.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/sample.html` & `gramex-1.92.1/gramex/apps/uifactory/sample.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/snippets/button/bs4-button.js` & `gramex-1.92.1/gramex/apps/uifactory/snippets/button/bs4-button.js`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/snippets/checkbox/bs4-checkbox.js` & `gramex-1.92.1/gramex/apps/uifactory/snippets/checkbox/bs4-checkbox.js`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/snippets/email/bs4-email.js` & `gramex-1.92.1/gramex/apps/uifactory/snippets/email/bs4-email.js`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/snippets/multiselect/bs4-multiselect.js` & `gramex-1.92.1/gramex/apps/uifactory/snippets/multiselect/bs4-multiselect.js`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/snippets/number/bs4-number.js` & `gramex-1.92.1/gramex/apps/uifactory/snippets/number/bs4-number.js`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/snippets/radio/bs4-radio.js` & `gramex-1.92.1/gramex/apps/uifactory/snippets/radio/bs4-radio.js`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/snippets/range/bs4-range.js` & `gramex-1.92.1/gramex/apps/uifactory/snippets/range/bs4-range.js`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/snippets/select/bs4-select.js` & `gramex-1.92.1/gramex/apps/uifactory/snippets/select/bs4-select.js`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/snippets/setup.js` & `gramex-1.92.1/gramex/apps/uifactory/snippets/setup.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -22,9 +22,9 @@
             encoding: "utf8",
         });
     });
 
 // Write to snippets.json
 fs.writeFileSync(
     path.join(__dirname, "snippets.json"),
-    JSON.stringify(config) + "\n"
+    JSON.stringify(config) + "\n",
 );
```

### Comparing `gramex-1.92.0/gramex/apps/uifactory/snippets/text/bs4-text.js` & `gramex-1.92.1/gramex/apps/uifactory/snippets/text/bs4-text.js`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/snippets/textarea/bs4-textarea.js` & `gramex-1.92.1/gramex/apps/uifactory/snippets/textarea/bs4-textarea.js`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/style.scss` & `gramex-1.92.1/gramex/apps/uifactory/style.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/template-navbar-view-form.html` & `gramex-1.92.1/gramex/apps/uifactory/template-navbar-view-form.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/template-navbar.html` & `gramex-1.92.1/gramex/apps/uifactory/template-navbar.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/uifactory/viewform.html` & `gramex-1.92.1/gramex/apps/uifactory/viewform.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/update/README.md` & `gramex-1.92.1/gramex/apps/update/README.md`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/update/gramex.yaml` & `gramex-1.92.1/gramex/apps/update/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/update/gramexupdate.py` & `gramex-1.92.1/gramex/apps/update/gramexupdate.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/apps/update/index.html` & `gramex-1.92.1/gramex/apps/update/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/cache.py` & `gramex-1.92.1/gramex/cache.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/config.py` & `gramex-1.92.1/gramex/config.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/data.py` & `gramex-1.92.1/gramex/data.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/debug.py` & `gramex-1.92.1/gramex/debug.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/deploy.yaml` & `gramex-1.92.1/gramex/deploy.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/download.vega.js` & `gramex-1.92.1/gramex/download.vega.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -14,15 +14,15 @@
         id +
         '" style="text-align:center;width:' +
         width +
         "px;height:" +
         height +
         'px">' +
         loading +
-        "</div>"
+        "</div>",
     );
     document.addEventListener("DOMContentLoaded", function() {
         var container = document.getElementById(id);
         try {
             container.spec = {};
             if ("fromjson" in spec) {
                 container.spec.vegam = spec.fromjson;
```

### Comparing `gramex-1.92.0/gramex/favicon.ico` & `gramex-1.92.1/gramex/favicon.ico`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/gramex.yaml` & `gramex-1.92.1/gramex/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/gramexfeatures.csv` & `gramex-1.92.1/gramex/gramexfeatures.csv`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/gramexsize.csv` & `gramex-1.92.1/gramex/gramexsize.csv`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/handlers/400.html` & `gramex-1.92.1/gramex/handlers/400.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/handlers/401.html` & `gramex-1.92.1/gramex/handlers/401.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/handlers/403.html` & `gramex-1.92.1/gramex/handlers/403.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/handlers/404.html` & `gramex-1.92.1/gramex/handlers/404.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/handlers/500.html` & `gramex-1.92.1/gramex/handlers/500.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/handlers/__init__.py` & `gramex-1.92.1/gramex/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/handlers/auth.recaptcha.template.html` & `gramex-1.92.1/gramex/handlers/auth.recaptcha.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/handlers/auth.template.html` & `gramex-1.92.1/gramex/handlers/auth.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/handlers/authhandler.py` & `gramex-1.92.1/gramex/handlers/authhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/handlers/basehandler.py` & `gramex-1.92.1/gramex/handlers/basehandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -983,19 +983,20 @@
             gramex.data.delete(
                 **gramex.service.storelocations.otp, id=['token'], args={'token': [key]}
             )
         # Skip expired tokens
         if row['expire'] <= time.time():
             return None
         # Return the user column parsed as JSON.
-        # Add custom keys from the table to the user object.
+        # Add custom keys from the table to the user object. Don't overwrite NULL values.
         row['user'] = json.loads(row['user'])
         custom_keys = [key for key in row if key not in {'user', 'token', 'expire'}]
         if isinstance(row['user'], dict):
-            row['user'].update({key: row[key] for key in custom_keys})
+            for key in custom_keys:
+                row['user'][key] = row['user'].get(key, None) if row[key] is None else row[key]
         else:
             app_log.warning('Cannot add custom keys to non-dict "user" in: %r', row)
         return row
 
     def revoke_otp(self, key: str) -> Union[str, dict, None]:
         '''Revoke an OTP. Returns the user object from [gramex.handlers.BaseMixin.get_otp][].'''
         return self.get_otp(key, revoke=True)
```

### Comparing `gramex-1.92.0/gramex/handlers/capturehandler.py` & `gramex-1.92.1/gramex/handlers/capturehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/handlers/chatgpthandler.py` & `gramex-1.92.1/gramex/handlers/chatgpthandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/handlers/comichandler.py` & `gramex-1.92.1/gramex/handlers/comichandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/handlers/drivehandler.py` & `gramex-1.92.1/gramex/handlers/drivehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/handlers/filehandler.py` & `gramex-1.92.1/gramex/handlers/filehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/handlers/filehandler.template.html` & `gramex-1.92.1/gramex/handlers/filehandler.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/handlers/formhandler.py` & `gramex-1.92.1/gramex/handlers/formhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/handlers/functionhandler.py` & `gramex-1.92.1/gramex/handlers/functionhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/handlers/jsonhandler.py` & `gramex-1.92.1/gramex/handlers/jsonhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/handlers/messagehandler.py` & `gramex-1.92.1/gramex/handlers/messagehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/handlers/mlhandler.py` & `gramex-1.92.1/gramex/handlers/mlhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/handlers/modelhandler.py` & `gramex-1.92.1/gramex/handlers/modelhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/handlers/openapiconfig.yaml` & `gramex-1.92.1/gramex/handlers/openapiconfig.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/handlers/openapihandler.py` & `gramex-1.92.1/gramex/handlers/openapihandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/handlers/pptxhandler.py` & `gramex-1.92.1/gramex/handlers/pptxhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/handlers/processhandler.py` & `gramex-1.92.1/gramex/handlers/processhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/handlers/proxyhandler.py` & `gramex-1.92.1/gramex/handlers/proxyhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/handlers/queryhandler.template.html` & `gramex-1.92.1/gramex/handlers/queryhandler.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/handlers/socialhandler.py` & `gramex-1.92.1/gramex/handlers/socialhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/handlers/uploadhandler.py` & `gramex-1.92.1/gramex/handlers/uploadhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/handlers/websockethandler.py` & `gramex-1.92.1/gramex/handlers/websockethandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/http.py` & `gramex-1.92.1/gramex/http.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/install.py` & `gramex-1.92.1/gramex/install.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/license.py` & `gramex-1.92.1/gramex/license.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/migrate.py` & `gramex-1.92.1/gramex/migrate.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/ml.py` & `gramex-1.92.1/gramex/ml.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/ml_api.py` & `gramex-1.92.1/gramex/ml_api.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/pptgen/__init__.py` & `gramex-1.92.1/gramex/pptgen/__init__.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/pptgen/color.py` & `gramex-1.92.1/gramex/pptgen/color.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/pptgen/colors.json` & `gramex-1.92.1/gramex/pptgen/colors.json`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/pptgen/commands.py` & `gramex-1.92.1/gramex/pptgen/commands.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/pptgen/fonts.json` & `gramex-1.92.1/gramex/pptgen/fonts.json`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/pptgen/fontwidth.py` & `gramex-1.92.1/gramex/pptgen/fontwidth.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/pptgen/utils.py` & `gramex-1.92.1/gramex/pptgen/utils.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/pptgen2/__init__.py` & `gramex-1.92.1/gramex/pptgen2/__init__.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/pptgen2/commands.py` & `gramex-1.92.1/gramex/pptgen2/commands.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/pptgen2/config.yaml` & `gramex-1.92.1/gramex/pptgen2/config.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/pynode.py` & `gramex-1.92.1/gramex/pynode.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/scale.py` & `gramex-1.92.1/gramex/scale.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/secrets.py` & `gramex-1.92.1/gramex/secrets.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/servicenow.yaml` & `gramex-1.92.1/gramex/servicenow.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/services/__init__.py` & `gramex-1.92.1/gramex/services/__init__.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/services/emailer.py` & `gramex-1.92.1/gramex/services/emailer.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/services/rediscache.py` & `gramex-1.92.1/gramex/services/rediscache.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/services/scheduler.py` & `gramex-1.92.1/gramex/services/scheduler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/services/sms.py` & `gramex-1.92.1/gramex/services/sms.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/services/ttlcache.py` & `gramex-1.92.1/gramex/services/ttlcache.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/services/urlcache.py` & `gramex-1.92.1/gramex/services/urlcache.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/services/watcher.py` & `gramex-1.92.1/gramex/services/watcher.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/sm_api.py` & `gramex-1.92.1/gramex/sm_api.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/topcause.py` & `gramex-1.92.1/gramex/topcause.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/transformers.py` & `gramex-1.92.1/gramex/transformers.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/transforms/__init__.py` & `gramex-1.92.1/gramex/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/transforms/auth.py` & `gramex-1.92.1/gramex/transforms/auth.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/transforms/template.py` & `gramex-1.92.1/gramex/transforms/template.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/transforms/transforms.py` & `gramex-1.92.1/gramex/transforms/transforms.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/transforms/twitterstream.py` & `gramex-1.92.1/gramex/transforms/twitterstream.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex/winservice.py` & `gramex-1.92.1/gramex/winservice.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex.egg-info/PKG-INFO` & `gramex-1.92.1/gramex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gramex
-Version: 1.92.0
+Version: 1.92.1
 Summary: Gramex: Low Code Data Solutions Platform
 Author-email: Anand S <s.anand@gramener.com>, Pratap Vardhan <pratapapvr@gmail.com>, Jaidev Deshpande <jaidev.deshpande@gramener.com>, Bhanu Kamapantula <talk2kish@gmail.com>, Radheya Kale <radheya.kale@gramener.com>, Karmanya Aggarwal <karmanyaaggarwal@gmail.com>, Sandeep Bhat <sandeep.bhat@gramener.com>, Shraddheya Shrivastava <shraddheya.shrivastava@gramener.com>, Sundeep Reddy Mallu <sundeep.mally@gramener.com>
 License: MIT
 Project-URL: Homepage, https://gramener.com/gramex/
 Project-URL: Documentation, https://gramener.com/gramex/guide/
 Project-URL: Repository, https://github.com/gramener/gramex
 Project-URL: Changelog, https://gramener.com/gramex/guide/release/
```

### Comparing `gramex-1.92.0/gramex.egg-info/SOURCES.txt` & `gramex-1.92.1/gramex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/gramex.egg-info/requires.txt` & `gramex-1.92.1/gramex.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/pyproject.toml` & `gramex-1.92.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gramex"
-version = "1.92.0"
+version = "1.92.1"
 description = "Gramex: Low Code Data Solutions Platform"
 # People with 2+ contributions on https://github.com/gramener/gramex/graphs/contributors
 authors = [
     {name = "Anand S", email = "s.anand@gramener.com"},
     {name = "Pratap Vardhan", email = "pratapapvr@gmail.com"},
     {name = "Jaidev Deshpande", email = "jaidev.deshpande@gramener.com"},
     {name = "Bhanu Kamapantula", email = "talk2kish@gmail.com"},
```

### Comparing `gramex-1.92.0/tests/test_admin.py` & `gramex-1.92.1/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_alerts.py` & `gramex-1.92.1/tests/test_alerts.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_args.py` & `gramex-1.92.1/tests/test_args.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_auth.py` & `gramex-1.92.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_cache.py` & `gramex-1.92.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_capturehandler.py` & `gramex-1.92.1/tests/test_capturehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_comichandler.py` & `gramex-1.92.1/tests/test_comichandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_drivehandler.py` & `gramex-1.92.1/tests/test_drivehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_filehandler.py` & `gramex-1.92.1/tests/test_filehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_filterhandler.py` & `gramex-1.92.1/tests/test_filterhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_formhandler.py` & `gramex-1.92.1/tests/test_formhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_functionhandler.py` & `gramex-1.92.1/tests/test_functionhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_gramexlog.py` & `gramex-1.92.1/tests/test_gramexlog.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_handlers.py` & `gramex-1.92.1/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_init.py` & `gramex-1.92.1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_install.py` & `gramex-1.92.1/tests/test_install.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_jsonhandler.py` & `gramex-1.92.1/tests/test_jsonhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_ldapauth.py` & `gramex-1.92.1/tests/test_ldapauth.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_logviewer.py` & `gramex-1.92.1/tests/test_logviewer.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_mlhandler.py` & `gramex-1.92.1/tests/test_mlhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_modelhandler.py` & `gramex-1.92.1/tests/test_modelhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_openapihandler.py` & `gramex-1.92.1/tests/test_openapihandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_pptxhandler.py` & `gramex-1.92.1/tests/test_pptxhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_processhandler.py` & `gramex-1.92.1/tests/test_processhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_proxyhandler.py` & `gramex-1.92.1/tests/test_proxyhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_pynode.py` & `gramex-1.92.1/tests/test_pynode.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_schedule.py` & `gramex-1.92.1/tests/test_schedule.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_secrets.py` & `gramex-1.92.1/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_subprocess.py` & `gramex-1.92.1/tests/test_subprocess.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_translater.py` & `gramex-1.92.1/tests/test_translater.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_twitterresthandler.py` & `gramex-1.92.1/tests/test_twitterresthandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_ui.py` & `gramex-1.92.1/tests/test_ui.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_update.py` & `gramex-1.92.1/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_uploadhandler.py` & `gramex-1.92.1/tests/test_uploadhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_watcher.py` & `gramex-1.92.1/tests/test_watcher.py`

 * *Files identical despite different names*

### Comparing `gramex-1.92.0/tests/test_websockethandler.py` & `gramex-1.92.1/tests/test_websockethandler.py`

 * *Files identical despite different names*

