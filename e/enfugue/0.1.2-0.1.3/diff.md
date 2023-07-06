# Comparing `tmp/enfugue-0.1.2.tar.gz` & `tmp/enfugue-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enfugue-0.1.2.tar", last modified: Fri Jun 30 00:34:29 2023, max compression
+gzip compressed data, was "enfugue-0.1.3.tar", last modified: Thu Jul  6 03:42:40 2023, max compression
```

## Comparing `enfugue-0.1.2.tar` & `enfugue-0.1.3.tar`

### file list

```diff
@@ -1,257 +1,259 @@
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.955503 enfugue-0.1.2/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      177 2023-06-30 00:34:29.955503 enfugue-0.1.2/PKG-INFO
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.939504 enfugue-0.1.2/enfugue/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3774 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/__main__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.939504 enfugue-0.1.2/enfugue/api/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      314 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/api/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2186 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/api/config.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.939504 enfugue-0.1.2/enfugue/api/controller/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      690 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/api/controller/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1345 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/api/controller/base.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3638 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/api/controller/downloads.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     9025 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/api/controller/invocation.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    13819 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/api/controller/models.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    17819 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/api/controller/system.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     8447 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/api/downloads.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     8617 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/api/invocations.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    19203 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/api/manager.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    13327 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/api/server.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.939504 enfugue-0.1.2/enfugue/config/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3002 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/config/cms-context.yml
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       75 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/config/database.yml
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      170 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/config/enfugue.yml
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      119 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/config/logging.yml
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2312 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/config/server.yml
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.939504 enfugue-0.1.2/enfugue/database/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      554 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/database/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      130 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/database/base.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      355 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/database/config.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      814 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/database/invocations.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1199 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/database/models.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.943504 enfugue-0.1.2/enfugue/diffusion/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      782 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/constants.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.943504 enfugue-0.1.2/enfugue/diffusion/edge/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/edge/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3971 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/edge/detect.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1348 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/edge/hed.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.943504 enfugue-0.1.2/enfugue/diffusion/edge/mlsd/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      199 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/edge/mlsd/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     9546 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/edge/mlsd/model.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    24714 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/edge/mlsd/util.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    10752 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/engine.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    48134 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/manager.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    66164 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/pipeline.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    54605 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/plan.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    14172 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/process.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.943504 enfugue-0.1.2/enfugue/diffusion/rt/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      317 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/rt/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    12412 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/rt/engine.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.943504 enfugue-0.1.2/enfugue/diffusion/rt/model/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      465 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/rt/model/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5684 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/rt/model/base.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3110 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/rt/model/clip.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    13244 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/rt/model/controlledunet.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7791 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/rt/model/controlnet.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3770 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/rt/model/unet.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2580 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/rt/model/vae.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2671 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/rt/optimizer.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    15776 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/rt/pipeline.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.943504 enfugue-0.1.2/enfugue/diffusion/upscale/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3932 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/upscale/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6806 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/upscale/gfpganer.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    10440 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/util.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      619 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/vision.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      608 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/enfugue.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.943504 enfugue-0.1.2/enfugue/interface/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    12980 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/interface/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4429 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/interface/helpers.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.943504 enfugue-0.1.2/enfugue/partner/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/partner/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4752 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/partner/civitai.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1925 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/server.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.939504 enfugue-0.1.2/enfugue/static/
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.943504 enfugue-0.1.2/enfugue/static/css/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      773 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/css/01-reset.min.css
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      497 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/css/02-variables.min.css
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      279 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/css/03-fonts.min.css
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    12992 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/css/04-base.min.css
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7808 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/css/05-common.min.css
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      989 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/css/06-header.min.css
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4241 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/css/07-main.min.css
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    18052 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/css/08-enfugue.min.css
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    18689 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/css/09-enfugue-nodes.min.css
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.935504 enfugue-0.1.2/enfugue/static/css/vendor/
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.943504 enfugue-0.1.2/enfugue/static/css/vendor/fa/
--rw-r--r--   0 benjamin  (1000) benjamin  (1000)    18620 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/css/vendor/fa/brands.min.css
--rw-r--r--   0 benjamin  (1000) benjamin  (1000)    80651 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/css/vendor/fa/fontawesome.min.css
--rw-r--r--   0 benjamin  (1000) benjamin  (1000)      606 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/css/vendor/fa/regular.min.css
--rw-r--r--   0 benjamin  (1000) benjamin  (1000)      598 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/css/vendor/fa/solid.min.css
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.935504 enfugue-0.1.2/enfugue/static/fonts/
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.935504 enfugue-0.1.2/enfugue/static/fonts/vendor/
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.947503 enfugue-0.1.2/enfugue/static/fonts/vendor/fa/
--rw-r--r--   0 benjamin  (1000) benjamin  (1000)   186112 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/fonts/vendor/fa/fa-brands-400.ttf
--rw-r--r--   0 benjamin  (1000) benjamin  (1000)   107460 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/fonts/vendor/fa/fa-brands-400.woff2
--rw-r--r--   0 benjamin  (1000) benjamin  (1000)    62048 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/fonts/vendor/fa/fa-regular-400.ttf
--rw-r--r--   0 benjamin  (1000) benjamin  (1000)    25096 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/fonts/vendor/fa/fa-regular-400.woff2
--rw-r--r--   0 benjamin  (1000) benjamin  (1000)   397728 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/fonts/vendor/fa/fa-solid-900.ttf
--rw-r--r--   0 benjamin  (1000) benjamin  (1000)   150472 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/fonts/vendor/fa/fa-solid-900.woff2
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.947503 enfugue-0.1.2/enfugue/static/html/
--rw-------   0 benjamin  (1000) benjamin  (1000)      165 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/html/base.html.j2
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.947503 enfugue-0.1.2/enfugue/static/html/body/
--rw-------   0 benjamin  (1000) benjamin  (1000)      187 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/html/body/body-base.html.j2
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.947503 enfugue-0.1.2/enfugue/static/html/body/content/
--rw-------   0 benjamin  (1000) benjamin  (1000)      379 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/html/body/content/content-admin.html.j2
--rw-------   0 benjamin  (1000) benjamin  (1000)      349 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/html/body/content/content-application.html.j2
--rw-------   0 benjamin  (1000) benjamin  (1000)      122 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/html/body/content/content-error.html.j2
--rw-------   0 benjamin  (1000) benjamin  (1000)      297 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/html/body/content/content-external.html.j2
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      876 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/html/body/content/content-login.html.j2
--rw-------   0 benjamin  (1000) benjamin  (1000)      166 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/html/body/content/content-template.html.j2
--rw-------   0 benjamin  (1000) benjamin  (1000)      399 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/html/body/external-base.html.j2
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.947503 enfugue-0.1.2/enfugue/static/html/body/footer/
--rw-------   0 benjamin  (1000) benjamin  (1000)       55 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/html/body/footer/footer-base.html.j2
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      759 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/html/body/footer/footer.html.j2
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.947503 enfugue-0.1.2/enfugue/static/html/body/header/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       55 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/html/body/header/header-base.html.j2
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      140 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/html/body/header/header.html.j2
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.947503 enfugue-0.1.2/enfugue/static/html/head/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2162 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/html/head/head-base.html.j2
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.947503 enfugue-0.1.2/enfugue/static/img/
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.947503 enfugue-0.1.2/enfugue/static/img/brand/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      852 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/img/brand/civit-ai-logo.svg
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1293 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/img/brand/civit-ai.png
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)     1521 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/img/brand/ko-fi.png
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)     1486 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/img/brand/patreon.png
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     9307 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/img/brand/tensorrt.png
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)    63446 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/img/cloud-320.png
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.947503 enfugue-0.1.2/enfugue/static/img/favicon/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    13112 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/img/favicon/favicon-128x128.png
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2235 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/img/favicon/favicon-16x16.png
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    38833 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/img/favicon/favicon-256x256.png
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2827 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/img/favicon/favicon-32x32.png
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)   160675 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/img/favicon/favicon-512x512.png
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4987 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/img/favicon/favicon-64x64.png
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1150 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/img/favicon/favicon.ico
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.947503 enfugue-0.1.2/enfugue/static/js/
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.947503 enfugue-0.1.2/enfugue/static/js/application/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    12929 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/application/index.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.947503 enfugue-0.1.2/enfugue/static/js/base/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3038 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/base/api.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    16960 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/base/builder.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1114 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/base/csv.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     9583 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/base/helpers.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      915 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/base/loader.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      350 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/base/mutex.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      549 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/base/publisher.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3019 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/base/session.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2396 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/base/watcher.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.947503 enfugue-0.1.2/enfugue/static/js/common/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1814 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/common/event-tracker.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4554 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/common/history.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      441 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/common/notify.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      647 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/common/shadowbox.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2469 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/common/tooltip.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.947503 enfugue-0.1.2/enfugue/static/js/config/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      706 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/config/index.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.947503 enfugue-0.1.2/enfugue/static/js/controller/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      845 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/base.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.951503 enfugue-0.1.2/enfugue/static/js/controller/common/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7149 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/common/announcements.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4531 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/common/downloads.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    11935 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/common/invocation.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4771 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/common/model-manager.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6969 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/common/model-picker.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.951503 enfugue-0.1.2/enfugue/static/js/controller/file/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      242 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/file/01-new.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      513 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/file/02-open.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      645 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/file/03-save.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4132 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/file/04-history.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2764 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/file/05-results.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.951503 enfugue-0.1.2/enfugue/static/js/controller/help/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2637 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/help/01-about.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      338 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/help/02-documentation.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      337 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/help/03-discuss.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1298 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/index.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      393 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/menu.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.951503 enfugue-0.1.2/enfugue/static/js/controller/models/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     8688 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/models/01-civitait.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      276 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/models/02-manager.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      259 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/models/03-new.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.951503 enfugue-0.1.2/enfugue/static/js/controller/sidebar/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3562 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/sidebar/01-canvas.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1671 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/sidebar/02-tweaks.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1323 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/sidebar/03-generation.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    11037 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/sidebar/04-upscale.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      900 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/sidebar/05-prompts.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2616 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/sidebar/99-invoke.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.951503 enfugue-0.1.2/enfugue/static/js/controller/system/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3258 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/system/01-settings.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4587 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/system/02-users.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7985 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/system/03-installation.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2601 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/system/04-logs.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.951503 enfugue-0.1.2/enfugue/static/js/controller/toolbar/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      470 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/toolbar/01-load-image.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      317 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/toolbar/02-draw-scribble.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      263 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/toolbar/03-region-prompt.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      670 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/enfugue.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.951503 enfugue-0.1.2/enfugue/static/js/graphics/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      567 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/graphics/colors.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4622 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/graphics/geometry.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1869 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/graphics/paths.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2942 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/graphics/spline.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.951503 enfugue-0.1.2/enfugue/static/js/lang/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      203 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/lang/en.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      256 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/lang/index.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.951503 enfugue-0.1.2/enfugue/static/js/model/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1009 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/model/enfugue.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5772 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/model/index.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.951503 enfugue-0.1.2/enfugue/static/js/view/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3767 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/base.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.951503 enfugue-0.1.2/enfugue/static/js/view/forms/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7044 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/forms/base.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1456 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/forms/classic.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      502 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/forms/confirm.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.955503 enfugue-0.1.2/enfugue/static/js/view/forms/input/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3301 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/forms/input/base.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      472 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/forms/input/bool.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5969 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/forms/input/color.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    11312 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/forms/input/enumerable.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      611 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/forms/input/file.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      450 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/forms/input/misc.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2928 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/forms/input/numeric.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3845 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/forms/input/parent.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      724 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/forms/input/string.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1017 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/forms/input.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     9227 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/image.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3631 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/menu.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.955503 enfugue-0.1.2/enfugue/static/js/view/nodes/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    12845 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/nodes/base.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3427 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/nodes/decorations.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     9870 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/nodes/editor.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    22154 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/nodes/image-editor.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3459 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/nodes/windows.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1512 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/notifications.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4415 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/scribble.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3295 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/status.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    10912 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/table.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.955503 enfugue-0.1.2/enfugue/util/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      275 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/util/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1802 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/util/downloads.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      989 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/util/gpu.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3975 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/util/gputil.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5992 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/util/images.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4280 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/util/installation.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       76 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/util/log.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     8149 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/util/security.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1203 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/util/signature.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1768 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/util/tokens.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.939504 enfugue-0.1.2/enfugue.egg-info/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      177 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue.egg-info/PKG-INFO
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7767 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue.egg-info/SOURCES.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        1 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue.egg-info/dependency_links.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       50 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue.egg-info/entry_points.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1008 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue.egg-info/requires.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        8 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue.egg-info/top_level.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       38 2023-06-30 00:34:29.955503 enfugue-0.1.2/setup.cfg
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2533 2023-06-30 00:34:29.000000 enfugue-0.1.2/setup.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.845198 enfugue-0.1.3/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      202 2023-07-06 03:42:40.841198 enfugue-0.1.3/PKG-INFO
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.829199 enfugue-0.1.3/enfugue/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4606 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/__main__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.829199 enfugue-0.1.3/enfugue/api/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      314 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/api/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2186 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/api/config.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.829199 enfugue-0.1.3/enfugue/api/controller/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      690 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/api/controller/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1345 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/api/controller/base.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3638 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/api/controller/downloads.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    10348 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/api/controller/invocation.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    14784 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/api/controller/models.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    17819 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/api/controller/system.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     8447 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/api/downloads.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     8617 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/api/invocations.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    19203 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/api/manager.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    13881 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/api/server.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.829199 enfugue-0.1.3/enfugue/config/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3002 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/config/cms-context.yml
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       75 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/config/database.yml
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      170 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/config/enfugue.yml
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      119 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/config/logging.yml
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2312 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/config/server.yml
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.829199 enfugue-0.1.3/enfugue/database/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      554 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/database/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      130 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/database/base.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      355 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/database/config.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      814 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/database/invocations.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1199 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/database/models.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.829199 enfugue-0.1.3/enfugue/diffusion/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      782 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/constants.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.829199 enfugue-0.1.3/enfugue/diffusion/edge/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/edge/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4158 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/edge/detect.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1348 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/edge/hed.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.829199 enfugue-0.1.3/enfugue/diffusion/edge/mlsd/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      199 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/edge/mlsd/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     9546 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/edge/mlsd/model.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    24879 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/edge/mlsd/util.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    10752 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/engine.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    48637 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/manager.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    66127 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/pipeline.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    54605 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/plan.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    14172 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/process.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.829199 enfugue-0.1.3/enfugue/diffusion/rt/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      317 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/rt/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    12412 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/rt/engine.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.833199 enfugue-0.1.3/enfugue/diffusion/rt/model/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      465 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/rt/model/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5684 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/rt/model/base.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3110 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/rt/model/clip.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    13244 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/rt/model/controlledunet.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7791 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/rt/model/controlnet.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3770 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/rt/model/unet.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2580 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/rt/model/vae.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2671 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/rt/optimizer.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    15776 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/rt/pipeline.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.833199 enfugue-0.1.3/enfugue/diffusion/upscale/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3932 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/upscale/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6806 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/upscale/gfpganer.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    11443 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/util.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      619 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/diffusion/vision.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1152 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/enfugue.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.833199 enfugue-0.1.3/enfugue/interface/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    12980 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/interface/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4429 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/interface/helpers.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.833199 enfugue-0.1.3/enfugue/partner/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/partner/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4752 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/partner/civitai.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1925 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/server.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.825199 enfugue-0.1.3/enfugue/static/
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.833199 enfugue-0.1.3/enfugue/static/css/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      773 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/css/01-reset.min.css
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      497 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/css/02-variables.min.css
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      279 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/css/03-fonts.min.css
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    12952 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/css/04-base.min.css
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7808 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/css/05-common.min.css
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      989 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/css/06-header.min.css
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4241 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/css/07-main.min.css
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    18592 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/css/08-enfugue.min.css
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    18833 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/css/09-enfugue-nodes.min.css
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.825199 enfugue-0.1.3/enfugue/static/css/vendor/
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.833199 enfugue-0.1.3/enfugue/static/css/vendor/fa/
+-rw-r--r--   0 benjamin  (1000) benjamin  (1000)    18620 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/css/vendor/fa/brands.min.css
+-rw-r--r--   0 benjamin  (1000) benjamin  (1000)    80651 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/css/vendor/fa/fontawesome.min.css
+-rw-r--r--   0 benjamin  (1000) benjamin  (1000)      606 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/css/vendor/fa/regular.min.css
+-rw-r--r--   0 benjamin  (1000) benjamin  (1000)      598 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/css/vendor/fa/solid.min.css
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.825199 enfugue-0.1.3/enfugue/static/fonts/
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.825199 enfugue-0.1.3/enfugue/static/fonts/vendor/
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.833199 enfugue-0.1.3/enfugue/static/fonts/vendor/fa/
+-rw-r--r--   0 benjamin  (1000) benjamin  (1000)   186112 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/fonts/vendor/fa/fa-brands-400.ttf
+-rw-r--r--   0 benjamin  (1000) benjamin  (1000)   107460 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/fonts/vendor/fa/fa-brands-400.woff2
+-rw-r--r--   0 benjamin  (1000) benjamin  (1000)    62048 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/fonts/vendor/fa/fa-regular-400.ttf
+-rw-r--r--   0 benjamin  (1000) benjamin  (1000)    25096 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/fonts/vendor/fa/fa-regular-400.woff2
+-rw-r--r--   0 benjamin  (1000) benjamin  (1000)   397728 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/fonts/vendor/fa/fa-solid-900.ttf
+-rw-r--r--   0 benjamin  (1000) benjamin  (1000)   150472 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/fonts/vendor/fa/fa-solid-900.woff2
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.833199 enfugue-0.1.3/enfugue/static/html/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      165 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/html/base.html.j2
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.833199 enfugue-0.1.3/enfugue/static/html/body/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      187 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/html/body/body-base.html.j2
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.833199 enfugue-0.1.3/enfugue/static/html/body/content/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      379 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/html/body/content/content-admin.html.j2
+-rw-------   0 benjamin  (1000) benjamin  (1000)      349 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/html/body/content/content-application.html.j2
+-rw-------   0 benjamin  (1000) benjamin  (1000)      122 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/html/body/content/content-error.html.j2
+-rw-------   0 benjamin  (1000) benjamin  (1000)      297 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/html/body/content/content-external.html.j2
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      876 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/html/body/content/content-login.html.j2
+-rw-------   0 benjamin  (1000) benjamin  (1000)      166 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/html/body/content/content-template.html.j2
+-rw-------   0 benjamin  (1000) benjamin  (1000)      399 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/html/body/external-base.html.j2
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.833199 enfugue-0.1.3/enfugue/static/html/body/footer/
+-rw-------   0 benjamin  (1000) benjamin  (1000)       55 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/html/body/footer/footer-base.html.j2
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      759 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/html/body/footer/footer.html.j2
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.833199 enfugue-0.1.3/enfugue/static/html/body/header/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       55 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/html/body/header/header-base.html.j2
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      140 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/html/body/header/header.html.j2
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.833199 enfugue-0.1.3/enfugue/static/html/head/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2162 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/html/head/head-base.html.j2
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.833199 enfugue-0.1.3/enfugue/static/img/
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.837198 enfugue-0.1.3/enfugue/static/img/brand/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      852 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/img/brand/civit-ai-logo.svg
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1293 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/img/brand/civit-ai.png
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)     1521 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/img/brand/ko-fi.png
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)     1486 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/img/brand/patreon.png
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     9307 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/img/brand/tensorrt.png
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)    63446 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/img/cloud-320.png
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.837198 enfugue-0.1.3/enfugue/static/img/favicon/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    13112 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/img/favicon/favicon-128x128.png
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2235 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/img/favicon/favicon-16x16.png
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    38833 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/img/favicon/favicon-256x256.png
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2827 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/img/favicon/favicon-32x32.png
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)   160675 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/img/favicon/favicon-512x512.png
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4987 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/img/favicon/favicon-64x64.png
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1150 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/img/favicon/favicon.ico
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.837198 enfugue-0.1.3/enfugue/static/js/
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.837198 enfugue-0.1.3/enfugue/static/js/application/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    12933 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/application/index.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.837198 enfugue-0.1.3/enfugue/static/js/base/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3038 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/base/api.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    16960 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/base/builder.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1114 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/base/csv.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     9701 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/base/helpers.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      915 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/base/loader.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      350 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/base/mutex.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      549 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/base/publisher.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3019 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/base/session.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2396 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/base/watcher.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.837198 enfugue-0.1.3/enfugue/static/js/common/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1814 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/common/event-tracker.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4554 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/common/history.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      441 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/common/notify.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      647 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/common/shadowbox.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2469 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/common/tooltip.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.837198 enfugue-0.1.3/enfugue/static/js/config/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      706 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/config/index.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.837198 enfugue-0.1.3/enfugue/static/js/controller/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      845 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/base.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.837198 enfugue-0.1.3/enfugue/static/js/controller/common/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7149 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/common/announcements.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4531 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/common/downloads.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    12391 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/common/invocation.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4836 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/common/model-manager.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     9067 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/common/model-picker.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.837198 enfugue-0.1.3/enfugue/static/js/controller/file/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      242 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/file/01-new.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      513 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/file/02-open.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      645 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/file/03-save.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4132 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/file/04-history.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2764 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/file/05-results.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.837198 enfugue-0.1.3/enfugue/static/js/controller/help/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2637 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/help/01-about.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      338 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/help/02-documentation.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      337 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/help/03-discuss.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1298 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/index.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      393 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/menu.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.837198 enfugue-0.1.3/enfugue/static/js/controller/models/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     8688 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/models/01-civitait.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      284 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/models/02-manager.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      267 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/models/03-new.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.841198 enfugue-0.1.3/enfugue/static/js/controller/sidebar/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3552 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/sidebar/01-canvas.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1671 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/sidebar/02-tweaks.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1323 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/sidebar/03-generation.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    11037 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/sidebar/04-upscale.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      900 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/sidebar/05-prompts.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2616 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/sidebar/99-invoke.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.841198 enfugue-0.1.3/enfugue/static/js/controller/system/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3258 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/system/01-settings.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4587 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/system/02-users.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     8166 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/system/03-installation.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2601 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/system/04-logs.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.841198 enfugue-0.1.3/enfugue/static/js/controller/toolbar/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      470 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/toolbar/01-load-image.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      317 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/toolbar/02-draw-scribble.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      263 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/controller/toolbar/03-region-prompt.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      670 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/enfugue.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.841198 enfugue-0.1.3/enfugue/static/js/graphics/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      567 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/graphics/colors.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4622 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/graphics/geometry.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1869 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/graphics/paths.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2942 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/graphics/spline.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.841198 enfugue-0.1.3/enfugue/static/js/lang/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      203 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/lang/en.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      256 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/lang/index.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.841198 enfugue-0.1.3/enfugue/static/js/model/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1009 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/model/enfugue.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5772 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/model/index.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.841198 enfugue-0.1.3/enfugue/static/js/view/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3767 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/base.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.841198 enfugue-0.1.3/enfugue/static/js/view/forms/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7044 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/forms/base.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1456 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/forms/classic.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      502 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/forms/confirm.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.841198 enfugue-0.1.3/enfugue/static/js/view/forms/input/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3301 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/forms/input/base.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      472 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/forms/input/bool.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5969 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/forms/input/color.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    11336 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/forms/input/enumerable.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      611 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/forms/input/file.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      450 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/forms/input/misc.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2928 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/forms/input/numeric.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3845 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/forms/input/parent.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      724 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/forms/input/string.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1065 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/forms/input.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     9227 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/image.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3631 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/menu.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.841198 enfugue-0.1.3/enfugue/static/js/view/nodes/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    12845 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/nodes/base.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3427 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/nodes/decorations.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     9870 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/nodes/editor.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    22154 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/nodes/image-editor.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3459 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/nodes/windows.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1512 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/notifications.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4415 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/scribble.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3295 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/status.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    10912 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/static/js/view/table.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.841198 enfugue-0.1.3/enfugue/util/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      275 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/util/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1457 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/util/browser.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1802 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/util/downloads.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      989 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/util/gpu.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3975 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/util/gputil.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5992 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/util/images.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4632 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/util/installation.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       76 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/util/log.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     8149 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/util/security.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1203 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/util/signature.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1768 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/util/tokens.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)        5 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue/version.txt
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-07-06 03:42:40.829199 enfugue-0.1.3/enfugue.egg-info/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      202 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue.egg-info/PKG-INFO
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7811 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue.egg-info/SOURCES.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        1 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue.egg-info/dependency_links.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       50 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue.egg-info/entry_points.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1106 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue.egg-info/requires.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        8 2023-07-06 03:42:40.000000 enfugue-0.1.3/enfugue.egg-info/top_level.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       38 2023-07-06 03:42:40.845198 enfugue-0.1.3/setup.cfg
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2929 2023-07-06 03:42:40.000000 enfugue-0.1.3/setup.py
```

### Comparing `enfugue-0.1.2/enfugue/__main__.py` & `enfugue-0.1.3/enfugue/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -32,25 +32,53 @@
     """
     from enfugue.util import get_version
 
     try:
         enfugue_version = get_version()
     except:
         enfugue_version = "development"
+
     import torch
+    from enfugue.diffusion.util import (
+        get_optimal_device,
+        tensorrt_available,
+        directml_available,
+    )
+
+    device = get_optimal_device()
 
     click.echo(f"Enfugue v.{enfugue_version}")
     click.echo(f"Torch v.{torch.__version__}")
-    click.echo("CUDA {0}".format("available" if torch.cuda.is_available() else "unavailable"))
-    try:
-        import tensorrt
+    click.echo(f"\nAI/ML Capabilities:\n---------------------")
+    click.echo(f"Device type: {device.type}")
 
-        click.echo("TensorRT Supported")
-    except ImportError:
-        click.echo("TensorRT Unsupported")
+    if torch.cuda.is_available():
+        if torch.backends.cuda.is_built():
+            click.echo("CUDA: Ready")
+        else:
+            click.echo("CUDA: Available, but not installed")
+        if tensorrt_available():
+            click.echo("TensorRT: Ready")
+        else:
+            click.echo("TensorRT: Unavailable")
+    else:
+        click.echo("CUDA: Unavailable")
+
+    if directml_available():
+        click.echo("DirectML: Ready")
+    else:
+        click.echo("DirectML: Unavailable")
+
+    if torch.backends.mps.is_available():
+        if torch.backends.mps.is_built():
+            click.echo("MPS: Ready")
+        else:
+            click.echo("MPS: Available, but not installed")
+    else:
+        click.echo("MPS: Unavailable")
 
 
 @main.command(short_help="Dumps a copy of the configuration")
 @click.option("-f", "--filename", help="A file to write to instead of stdout.")
 @click.option(
     "-j", "--json", help="When passed, use JSON instead of YAML.", is_flag=True, default=False
 )
@@ -122,11 +150,11 @@
     print("Goodbye!")
 
 
 try:
     main()
 except Exception as ex:
     print(termcolor.colored(str(ex), "red"))
-    if "--verbose" in sys.argv or "-v" in sys.argv:
+    if "--verbose" in sys.argv or "-v" in sys.argv or os.environ.get("ENFUGUE_DEBUG", "0") == "1":
         print(termcolor.colored(traceback.format_exc(), "red"))
     sys.exit(5)
 sys.exit(0)
```

### Comparing `enfugue-0.1.2/enfugue/api/config.py` & `enfugue-0.1.3/enfugue/api/config.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/api/controller/__init__.py` & `enfugue-0.1.3/enfugue/api/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/api/controller/base.py` & `enfugue-0.1.3/enfugue/api/controller/base.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/api/controller/downloads.py` & `enfugue-0.1.3/enfugue/api/controller/downloads.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/api/controller/invocation.py` & `enfugue-0.1.3/enfugue/api/controller/invocation.py`

 * *Files 11% similar despite different names*

```diff
@@ -47,18 +47,48 @@
             None,
             None,
             None,
             None,
             None,
         )
         model_name = request.parsed.pop("model", None)
+        model_type = request.parsed.pop("model_type", None)
         plan_kwargs: Dict[str, Any] = {}
-        if model_name is not None:
+        if model_name is not None and model_type == "model":
             plan_kwargs = self.get_plan_kwargs_from_model(model_name)
-
+        elif model_name is not None and model_type == "checkpoint":
+            plan_kwargs = {
+                "model": os.path.join(
+                    self.configuration.get(
+                        "enfugue.engine.checkpoint", os.path.join(self.engine_root, "checkpoint")
+                    ),
+                    model_name,
+                ),
+                "lora": [
+                    (
+                        os.path.join(
+                            self.configuration.get(
+                                "enfugue.engine.lora", os.path.join(self.engine_root, "lora")
+                            ),
+                            lora["model"],
+                        ),
+                        float(lora["weight"]),
+                    )
+                    for lora in request.parsed.pop("lora", [])
+                ],
+                "inversion": [
+                    os.path.join(
+                        self.configuration.get(
+                            "enfugue.engine.inversion", os.path.join(self.engine_root, "inversion")
+                        ),
+                        inversion,
+                    )
+                    for inversion in request.parsed.pop("inversion", [])
+                ],
+            }
         plan = DiffusionPlan.from_nodes(**{**plan_kwargs, **request.parsed})
         return self.invoke(request.token.user.id, plan).format()
 
     @handlers.path("^/api/invocation$")
     @handlers.methods("GET")
     @handlers.format()
     @handlers.secured("DiffusionInvocation", "read")
```

### Comparing `enfugue-0.1.2/enfugue/api/controller/models.py` & `enfugue-0.1.3/enfugue/api/controller/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -348,7 +348,29 @@
                     diffusion_model_name=new_model.name, model=inversion
                 )
                 self.database.add(new_inversion)
                 self.database.commit()
             return new_model
         except KeyError as ex:
             raise BadRequestError(f"Missing required parameter {ex}")
+
+    @handlers.path("^/api/model-options$")
+    @handlers.methods("GET")
+    @handlers.format()
+    @handlers.secured("DiffusionModel", "read")
+    def get_all_models(self, request: Request, response: Response) -> List[Dict[str, Any]]:
+        """
+        Gets all checkpoints and model names for the picker.
+        """
+        checkpoints_dir = self.configuration.get(
+            "enfugue.engine.checkpoint", os.path.join(self.engine_root, "checkpoint")
+        )
+        if not os.path.exists(checkpoints_dir):
+            checkpoints = []
+        else:
+            checkpoints = os.listdir(checkpoints_dir)
+        checkpoints.sort(key=lambda item: os.path.getmtime(os.path.join(checkpoints_dir, item)))
+        model_names = self.database.query(self.orm.DiffusionModel.name).all()
+
+        return [{"type": "checkpoint", "name": checkpoint} for checkpoint in checkpoints] + [
+            {"type": "model", "name": model[0]} for model in model_names
+        ]
```

### Comparing `enfugue-0.1.2/enfugue/api/controller/system.py` & `enfugue-0.1.3/enfugue/api/controller/system.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/api/downloads.py` & `enfugue-0.1.3/enfugue/api/downloads.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/api/invocations.py` & `enfugue-0.1.3/enfugue/api/invocations.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/api/manager.py` & `enfugue-0.1.3/enfugue/api/manager.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/api/server.py` & `enfugue-0.1.3/enfugue/api/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import PIL
 import signal
 import requests
 import datetime
+import webbrowser
 
 from typing import Any, Dict, List
 
 from webob import Request, Response
 
 from pibble.api.exceptions import NotFoundError
 from pibble.api.server.webservice.template import TemplateServer
@@ -358,14 +359,25 @@
             """
             Stops the server.
             """
             icon.visible = False
             stop_event.set()
             icon.stop()
 
+        def open_app(icon: pystray.Icon) -> None:
+            """
+            Opens up a browser and navigates to the app
+            """
+            server_config = configuration.get("server", {})
+            scheme = "https" if server_config.get("secure", False) else "http"
+            domain = server_config.get("domain", "127.0.0.1")
+            port = server_config.get("port", 45554)
+            url = f"{scheme}://{domain}:{port}/"
+            webbrowser.open(url)
+
         def setup(icon: pystray.Icon) -> None:
             """
             Starts the server.
             """
             icon.visible = True
             server = cls()
             server.configure_start(signal=False, **configuration)
@@ -374,14 +386,16 @@
             server.stop()
             server.destroy()
 
         static_dir = get_local_static_directory()
         icon_path = configuration.get("enfugue", {}).get("icon", "favicon/favicon-64x64.png")
         icon_image = PIL.Image.open(os.path.join(static_dir, "img", icon_path))
         icon = pystray.Icon("enfugue", icon_image)
-        icon.menu = pystray.Menu(pystray.MenuItem("Quit", stop))
+        icon.menu = pystray.Menu(
+            pystray.MenuItem("Open App", open_app), pystray.MenuItem("Quit", stop)
+        )
         icon.run(setup=setup)
 
 
 server_parents = tuple([EnfugueAPIServerBase] + list(EnfugueAPIControllerBase.enumerate()))
 
 EnfugueAPIServer = type("EnfugueAPIServer", server_parents, {})
```

### Comparing `enfugue-0.1.2/enfugue/config/cms-context.yml` & `enfugue-0.1.3/enfugue/config/cms-context.yml`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/config/server.yml` & `enfugue-0.1.3/enfugue/config/server.yml`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/database/__init__.py` & `enfugue-0.1.3/enfugue/database/__init__.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/database/invocations.py` & `enfugue-0.1.3/enfugue/database/invocations.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/database/models.py` & `enfugue-0.1.3/enfugue/database/models.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/diffusion/constants.py` & `enfugue-0.1.3/enfugue/diffusion/constants.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/diffusion/edge/detect.py` & `enfugue-0.1.3/enfugue/diffusion/edge/detect.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,50 +62,54 @@
         Runs holistically-nested edge detection on an image.
         """
         from enfugue.diffusion.edge.hed import HEDCropLayer  # type: ignore[attr-defined]
 
         width, height = image.size
 
         model = cv2.dnn.readNetFromCaffe(self.hed_prototxt, self.hed_caffemodel)
-        cv2.dnn_registerLayer("Crop", HEDCropLayer)
+        cv2.dnn_registerLayer("Crop", HEDCropLayer) # type: ignore[attr-defined]
 
         cv2_image = ComputerVision.convert_image(image)
         dnn_input = cv2.dnn.blobFromImage(
             cv2_image,
             scalefactor=1.0,
             size=(width, height),
             mean=self.HED_MEAN,
             swapRB=False,
             crop=False,
         )
         model.setInput(dnn_input)
         dnn_output = model.forward()
         output_array = (cv2.cvtColor(dnn_output[0, 0], cv2.COLOR_GRAY2BGR) * 255).astype(np.uint8)
-        cv2.dnn_unregisterLayer("Crop")
+        cv2.dnn_unregisterLayer("Crop") # type: ignore[attr-defined]
         return PIL.Image.fromarray(output_array)
 
     def mlsd(self, image: PIL.Image.Image) -> PIL.Image.Image:
         """
         Runs Mobile Line Segment Detection (MLSD) on an image.
         """
         import torch
+        from enfugue.diffusion.util import get_optimal_device
         from enfugue.diffusion.edge.mlsd import MLSD, pred_lines  # type: ignore[attr-defined]
 
-        if torch.cuda.is_available():
+        device = get_optimal_device()
+        model = MLSD().to(device).eval()
+        """
+        if device.type == "cuda":
+
             model = MLSD().cuda().eval()
-            device = torch.device("cuda")
         else:
             model = MLSD().eval()
-            device = torch.device("cpu")
-
+        device = torch.device(device_type)
+        """
         model.load_state_dict(torch.load(self.mlsd_weights, map_location=device), strict=True)
         cv2_image = ComputerVision.convert_image(image)
         cv2_image = cv2.resize(cv2_image, (512, 512))
         cv2_image = cv2.cvtColor(cv2_image, cv2.COLOR_BGR2RGB)
-        lines = pred_lines(cv2_image, model, [512, 512], 0.1, 20)
+        lines = pred_lines(cv2_image, model, [512, 512], 0.1, 20, device)
         cv2_image = np.zeros((512, 512, 3), np.uint8)
 
         for line in lines:
             cv2.line(
                 cv2_image,
                 (int(line[0]), int(line[1])),
                 (int(line[2]), int(line[3])),
```

### Comparing `enfugue-0.1.2/enfugue/diffusion/edge/hed.py` & `enfugue-0.1.3/enfugue/diffusion/edge/hed.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/diffusion/edge/mlsd/model.py` & `enfugue-0.1.3/enfugue/diffusion/edge/mlsd/model.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/diffusion/edge/mlsd/util.py` & `enfugue-0.1.3/enfugue/diffusion/edge/mlsd/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,22 @@
     ptss = ptss.detach().cpu().numpy()
     scores = scores.detach().cpu().numpy()
     displacement = displacement.detach().cpu().numpy()
     displacement = displacement.transpose((1, 2, 0))
     return ptss, scores, displacement
 
 
-def pred_lines(image, model, input_shape=[512, 512], score_thr=0.10, dist_thr=20.0):
+def pred_lines(
+    image,
+    model,
+    input_shape=[512, 512],
+    score_thr=0.10,
+    dist_thr=20.0,
+    device=None,
+):
     h, w, _ = image.shape
     h_ratio, w_ratio = [h / input_shape[0], w / input_shape[1]]
 
     resized_image = np.concatenate(
         [
             cv2.resize(image, (input_shape[0], input_shape[1]), interpolation=cv2.INTER_AREA),
             np.ones([input_shape[0], input_shape[1], 1]),
@@ -59,15 +66,18 @@
         axis=-1,
     )
 
     resized_image = resized_image.transpose((2, 0, 1))
     batch_image = np.expand_dims(resized_image, axis=0).astype("float32")
     batch_image = (batch_image / 127.5) - 1.0
 
-    batch_image = torch.from_numpy(batch_image).float().cuda()
+    batch_image = torch.from_numpy(batch_image).float()
+    if device:
+        batch_image = batch_image.to(device)
+
     outputs = model(batch_image)
     pts, pts_score, vmap = deccode_output_score_and_ptss(outputs, 200, 3)
     start = vmap[:, :, :2]
     end = vmap[:, :, 2:]
     dist_map = np.sqrt(np.sum((start - end) ** 2, axis=-1))
 
     segments_list = []
@@ -101,14 +111,15 @@
         "inside_ratio": 0.45,
         "w_overlap": 0.0,
         "w_degree": 1.95,
         "w_length": 0.0,
         "w_area": 1.86,
         "w_center": 0.14,
     },
+    device=None,
 ):
     """
     shape = [height, width]
     """
     h, w, _ = image.shape
     original_shape = [h, w]
 
@@ -119,15 +130,18 @@
         ],
         axis=-1,
     )
     resized_image = resized_image.transpose((2, 0, 1))
     batch_image = np.expand_dims(resized_image, axis=0).astype("float32")
     batch_image = (batch_image / 127.5) - 1.0
 
-    batch_image = torch.from_numpy(batch_image).float().cuda()
+    batch_image = torch.from_numpy(batch_image).float()
+    if device:
+        batch_image = batch_image.to(device)
+
     outputs = model(batch_image)
 
     pts, pts_score, vmap = deccode_output_score_and_ptss(outputs, 200, 3)
     start = vmap[:, :, :2]  # (x, y)
     end = vmap[:, :, 2:]  # (x, y)
     dist_map = np.sqrt(np.sum((start - end) ** 2, axis=-1))
```

### Comparing `enfugue-0.1.2/enfugue/diffusion/engine.py` & `enfugue-0.1.3/enfugue/diffusion/engine.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/diffusion/manager.py` & `enfugue-0.1.3/enfugue/diffusion/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import os
 import time
 import torch
 import random
 import datetime
+import traceback
 import threading
 
 from typing import Type, Union, Any, Optional, List, Tuple, Dict, Literal, Callable, TYPE_CHECKING
 from hashlib import md5
 
 from pibble.api.configuration import APIConfiguration
 from pibble.api.exceptions import ConfigurationError
@@ -108,19 +109,23 @@
         Sets a new value for safety checking. Destroys the pipeline.
         """
         if val != getattr(self, "_safe", None):
             self._safe = val
             del self.pipeline
 
     @property
-    def device(self) -> str:
+    def device(self) -> torch.device:
         """
         Gets the device that will be executed on
         """
-        return "cuda" if torch.cuda.is_available() else "cpu"
+        if not hasattr(self, "_device"):
+            from enfugue.diffusion.util import get_optimal_device
+
+            self._device = get_optimal_device()
+        return self._device
 
     @property
     def seed(self) -> int:
         """
         Gets the seed. If there is none, creates a random one once.
         """
         if not hasattr(self, "_seed"):
@@ -180,15 +185,19 @@
 
     @property
     def generator(self) -> torch.Generator:
         """
         Creates the generator once, otherwise returns it.
         """
         if not hasattr(self, "_generator"):
-            self._generator = torch.Generator(device=self.device)
+            try:
+                self._generator = torch.Generator(device=self.device)
+            except RuntimeError:
+                # Unsupported device, go to CPU
+                self._generator = torch.Generator()
             self._generator.manual_seed(self.seed)
         return self._generator
 
     @generator.deleter
     def generator(self) -> None:
         """
         Removes an existing generator.
@@ -676,44 +685,43 @@
     @property
     def model(self) -> str:
         """
         Gets the configured model.
         """
         if not hasattr(self, "_model"):
             self._model = self.configuration.get("enfugue.model", DEFAULT_MODEL)
-            if self._model.startswith("http"):
-                self._model = self.check_download_checkpoint(self._model)
         return self._model
 
     @model.setter
     def model(self, new_model: Optional[str]) -> None:
         """
         Sets a new model. Destroys the pipeline.
         """
         if new_model is None:
             new_model = self.configuration.get("enfugue.model", DEFAULT_MODEL)
         if new_model.startswith("http"):
             new_model = self.check_download_checkpoint(new_model)
-        if self.model != new_model:
+        new_model_name, _ = os.path.splitext(os.path.basename(new_model))
+        if self.model_name != new_model_name:
             del self.pipeline
         self._model = new_model
 
     @property
     def model_name(self) -> str:
         """
         Gets just the basename of the model
         """
         return os.path.splitext(os.path.basename(self.model))[0]
 
     @property
     def dtype(self) -> torch.dtype:
         if not hasattr(self, "_torch_dtype"):
-            if self.device == "cpu":
+            if self.device.type == "cpu":
                 logger.debug("Inferencing on CPU, using BFloat")
-                self._torch_dtype = torch.float
+                self._torch_dtype = torch.bfloat16
             else:
                 configuration_dtype = self.configuration.get("enfugue.dtype", "float16")
                 if configuration_dtype == "float16" or configuration_dtype == "half":
                     self._torch_dtype = torch.half
                 elif configuration_dtype == "float32" or configuration_dtype == "float":
                     self._torch_dtype = torch.float
                 else:
@@ -724,15 +732,15 @@
 
     @dtype.setter
     def dtype(self, new_dtype: Union[str, torch.dtype]) -> None:
         """
         Sets the torch dtype.
         Deletes the pipeline if it's different from the previous one.
         """
-        if self.device == "cpu":
+        if self.device.type == "cpu":
             raise ValueError("CPU-based diffusion can only use bfloat")
         if new_dtype == "float16" or new_dtype == "half":
             new_dtype = torch.half
         elif new_dtype == "float32" or new_dtype == "float":
             new_dtype = torch.float
         else:
             raise ConfigurationError(
@@ -817,29 +825,14 @@
     def inversion_names(self) -> List[str]:
         """
         Gets the basenames of any textual inversions present.
         """
         return [os.path.splitext(os.path.basename(inversion))[0] for inversion in self.inversion]
 
     @property
-    def model_ckpt_path(self) -> str:
-        """
-        Gets the path for a model checkpoint. May be a .ckpt or .safetensors.
-        """
-        ckpt_path = os.path.join(self.engine_checkpoints_dir, f"{self.model}.ckpt")
-        safetensor_path = os.path.join(self.engine_checkpoints_dir, f"{self.model}.safetensors")
-
-        if os.path.exists(ckpt_path):
-            return ckpt_path
-        elif os.path.exists(safetensor_path):
-            return safetensor_path
-        else:
-            raise IOError(f"Unknown model {self.model}")
-
-    @property
     def inpainting(self) -> bool:
         """
         Returns true if the model is an inpainting model.
         """
         return "inpaint" in self.model
 
     @inpainting.setter
@@ -924,22 +917,26 @@
 
     @property
     def pipeline(self) -> EnfugueStableDiffusionPipeline:
         """
         Instantiates the pipeline.
         """
         if not hasattr(self, "_pipeline"):
+            if self.model.startswith("http"):
+                # Base model, make sure it's downloaded here
+                self.model = self.check_download_checkpoint(self.model)
+
             kwargs = {
                 "cache_dir": self.engine_cache_dir,
                 "engine_size": self.size,
                 "chunking_size": self.chunking_size,
                 "requires_safety_checker": self.safe,
-                "controlnet": self.controlnet,
                 "torch_dtype": self.dtype,
             }
+            controlnet = self.controlnet # Load into memory here
 
             if self.use_tensorrt:
                 if "unet" in self.TENSORRT_STAGES:
                     if self.controlnet is None and not self.TENSORRT_ALWAYS_USE_CONTROLLED_UNET:
                         kwargs["unet_engine_dir"] = self.model_tensorrt_unet_dir
                     else:
                         kwargs[
@@ -953,29 +950,39 @@
                     kwargs["clip_engine_dir"] = self.model_tensorrt_clip_dir
                 if not self.safe:
                     kwargs["safety_checker"] = None
                 self.check_create_tensorrt_engine_cache()
                 logger.debug(
                     f"Initializing pipeline from diffusers cache directory at {self.model_tensorrt_dir}. Arguments are {kwargs}"
                 )
-                pipeline = self.pipeline_class.from_pretrained(self.model_tensorrt_dir, **kwargs)
+                pipeline = self.pipeline_class.from_pretrained(
+                    self.model_tensorrt_dir,
+                    controlnet=controlnet,
+                    **kwargs
+                )
             elif self.engine_cache_exists:
                 if not self.safe:
                     kwargs["safety_checker"] = None
                 logger.debug(
                     f"Initializing pipeline from diffusers cache directory at {self.model_tensorrt_dir}. Arguments are {kwargs}"
                 )
-                pipeline = self.pipeline_class.from_pretrained(self.model_tensorrt_dir, **kwargs)
+                pipeline = self.pipeline_class.from_pretrained(
+                    self.model_tensorrt_dir,
+                    controlnet=controlnet,
+                    **kwargs
+                )
             else:
                 kwargs["load_safety_checker"] = self.safe
                 logger.debug(
                     f"Initializing pipeline from checkpoint at {self.model}. Arguments are {kwargs}"
                 )
                 pipeline = self.pipeline_class.from_ckpt(
-                    self.model, num_in_channels=9 if self.inpainting else 4, **kwargs
+                    self.model, num_in_channels=9 if self.inpainting else 4,
+                    controlnet=controlnet,
+                    **kwargs
                 )
             if not self.tensorrt_is_ready:
                 for lora, weight in self.lora:
                     logger.debug(f"Adding LoRA {lora} to pipeline")
                     pipeline.load_lora_weights(lora, multiplier=weight)
                 for inversion in self.inversion:
                     logger.debug(f"Adding textual inversion {inversion} to pipeline")
@@ -1336,16 +1343,24 @@
     ) -> None:
         """
         Creates an inpainting model by merging in the SD 1.5 inpainting model with a non inpainting model.
         """
         from enfugue.diffusion.util import ModelMerger
 
         self.start_keepalive()
-        merger = ModelMerger(
-            self.check_download_checkpoint(DEFAULT_INPAINTING_MODEL),
-            source_checkpoint_path,
-            self.check_download_checkpoint(DEFAULT_MODEL),
-            interpolation="add-difference",
-        )
-        merger.save(target_checkpoint_path)
-        logger.info(f"Saved merged inpainting checkpoint at {target_checkpoint_path}")
+        try:
+            merger = ModelMerger(
+                self.check_download_checkpoint(DEFAULT_INPAINTING_MODEL),
+                source_checkpoint_path,
+                self.check_download_checkpoint(DEFAULT_MODEL),
+                interpolation="add-difference",
+            )
+            merger.save(target_checkpoint_path)
+        except Exception as ex:
+            logger.error(
+                f"Couldn't save merged checkpoint made from {source_checkpoint_path} to {target_checkpoint_path}: {ex}"
+            )
+            logger.error(traceback.format_exc())
+            raise
+        else:
+            logger.info(f"Saved merged inpainting checkpoint at {target_checkpoint_path}")
         self.stop_keepalive()
```

### Comparing `enfugue-0.1.2/enfugue/diffusion/pipeline.py` & `enfugue-0.1.3/enfugue/diffusion/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,28 +135,27 @@
         upcast_attention: Optional[bool] = None,
         extract_ema: Optional[bool] = None,
         num_in_channels: Optional[int] = None,
         **kwargs: Any,
     ) -> EnfugueStableDiffusionPipeline:
         """
         Loads a checkpoint into this pipeline.
-        Diffusers' `from_pretrained` lets us pass arbitrary kwargs in, but `from_ckpt` does not.
+        Diffusers' `from_pretrained` lets us pass arbitrary kwargs in, but `7from_ckpt` does not.
         That's why we override it for this method - most of this is copied from
         https://github.com/huggingface/diffusers/blob/49949f321d9b034440b52e54937fd2df3027bf0a/src/diffusers/pipelines/stable_diffusion/convert_from_ckpt.py
         """
-        device = "cuda" if torch.cuda.is_available() else "cpu"
         if checkpoint_path.endswith("safetensors"):
             from safetensors import safe_open
 
             checkpoint = {}
             with safe_open(checkpoint_path, framework="pt", device="cpu") as f:
                 for key in f.keys():
                     checkpoint[key] = f.get_tensor(key)
         else:
-            checkpoint = torch.load(checkpoint_path, map_location=device)
+            checkpoint = torch.load(checkpoint_path, map_location="cpu")
 
         # Sometimes models don't have the global_step item
         if "global_step" in checkpoint:
             global_step = checkpoint["global_step"]
         else:
             global_step = None
 
@@ -910,15 +909,15 @@
         Executes the denoising loop without chunking.
         """
         if extra_step_kwargs is None:
             extra_step_kwargs = {}
 
         num_steps = len(timesteps)
         num_warmup_steps = num_steps - num_inference_steps * self.scheduler.order
-        logger.debug(f"Denoising image in {num_steps} steps (unchunked)")
+        logger.debug(f"Denoising image on {device} in {num_steps} steps (unchunked)")
 
         for i, t in enumerate(timesteps):
             # expand the latents if we are doing classifier free guidance
             latent_model_input = (
                 torch.cat([latents] * 2) if do_classifier_free_guidance else latents
             )
             latent_model_input = self.scheduler.scale_model_input(latent_model_input, t)
@@ -1065,15 +1064,15 @@
         engine_latent_size = self.engine_size // self.vae_scale_factor
 
         count = torch.zeros_like(latents)
         value = torch.zeros_like(latents)
 
         total_num_steps = num_steps * num_chunks
         logger.debug(
-            f"Denoising image in {total_num_steps} total steps ({num_inference_steps} inference steps * {num_chunks} chunks)"
+            f"Denoising image in {total_num_steps} on {device} in total steps ({num_inference_steps} inference steps * {num_chunks} chunks)"
         )
 
         for i, t in enumerate(timesteps):
             # zero view latents
             count.zero_()
             value.zero_()
```

### Comparing `enfugue-0.1.2/enfugue/diffusion/plan.py` & `enfugue-0.1.3/enfugue/diffusion/plan.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/diffusion/process.py` & `enfugue-0.1.3/enfugue/diffusion/process.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/diffusion/rt/engine.py` & `enfugue-0.1.3/enfugue/diffusion/rt/engine.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/diffusion/rt/model/base.py` & `enfugue-0.1.3/enfugue/diffusion/rt/model/base.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/diffusion/rt/model/clip.py` & `enfugue-0.1.3/enfugue/diffusion/rt/model/clip.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/diffusion/rt/model/controlledunet.py` & `enfugue-0.1.3/enfugue/diffusion/rt/model/controlledunet.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/diffusion/rt/model/controlnet.py` & `enfugue-0.1.3/enfugue/diffusion/rt/model/controlnet.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/diffusion/rt/model/unet.py` & `enfugue-0.1.3/enfugue/diffusion/rt/model/unet.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/diffusion/rt/model/vae.py` & `enfugue-0.1.3/enfugue/diffusion/rt/model/vae.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/diffusion/rt/optimizer.py` & `enfugue-0.1.3/enfugue/diffusion/rt/optimizer.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/diffusion/rt/pipeline.py` & `enfugue-0.1.3/enfugue/diffusion/rt/pipeline.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/diffusion/upscale/__init__.py` & `enfugue-0.1.3/enfugue/diffusion/upscale/__init__.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/diffusion/upscale/gfpganer.py` & `enfugue-0.1.3/enfugue/diffusion/upscale/gfpganer.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/diffusion/util.py` & `enfugue-0.1.3/enfugue/diffusion/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,66 @@
 from __future__ import annotations
 
 import os
 import re
 import numpy as np
 import torch
+import torch.backends
 import safetensors.torch
 
 from typing import Dict, Type, Union, Optional, Literal, cast
 from enfugue.util import logger
 
-__all__ = ["DTypeConverter", "ModelMerger"]
+__all__ = [
+    "tensorrt_available",
+    "mps_available",
+    "directml_available",
+    "get_optimal_device",
+    "DTypeConverter",
+    "ModelMerger",
+]
+
+
+def tensorrt_available() -> bool:
+    """
+    Returns true if TensorRT is available.
+    """
+    try:
+        import tensorrt
+        tensorrt # silence importchecker
+        return True
+    except:
+        return False
+
+
+def directml_available() -> bool:
+    """
+    Returns true if directml is available.
+    """
+    try:
+        import torch_directml
+
+        return True
+    except:
+        return False
+
+
+def get_optimal_device() -> torch.device:
+    """
+    Gets the optimal device based on availability.
+    """
+    if torch.cuda.is_available() and torch.backends.cuda.is_built():
+        return torch.device("cuda")
+    elif directml_available():
+        import torch_directml
+
+        return torch_directml.device()
+    elif torch.backends.mps.is_available() and torch.backends.mps.is_built():
+        return torch.device("mps")
+    return torch.device("cpu")
 
 
 class DTypeConverter:
     """
     This class converts between numpy and torch types.
     """
```

### Comparing `enfugue-0.1.2/enfugue/diffusion/vision.py` & `enfugue-0.1.3/enfugue/diffusion/vision.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/interface/__init__.py` & `enfugue-0.1.3/enfugue/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/interface/helpers.py` & `enfugue-0.1.3/enfugue/interface/helpers.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/partner/civitai.py` & `enfugue-0.1.3/enfugue/partner/civitai.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/server.py` & `enfugue-0.1.3/enfugue/server.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/css/01-reset.min.css` & `enfugue-0.1.3/enfugue/static/css/01-reset.min.css`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/css/04-base.min.css` & `enfugue-0.1.3/enfugue/static/css/04-base.min.css`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-:not(i),:not(i):after,:not(i):before{box-sizing:border-box}*{scrollbar-color:rgba(0,0,0,.25),transparent;scrollbar-width:thin}::-webkit-scrollbar{background:var(--darkest-color);height:14px;width:14px}::-webkit-scrollbar-thumb{background-clip:padding-box;background-color:hsla(0,0%,100%,.25);border:4px solid hsla(0,0%,100%,0);border-radius:7px;box-shadow:inset -1px -1px 0 rgba(0,0,0,.05),inset 1px 1px 0 rgba(0,0,0,.05);height:6px}::-webkit-scrollbar-thumb:hover{background-color:hsla(0,0%,100%,.35)}::-webkit-scrollbar-button{display:none;height:0;width:0}::-webkit-scrollbar-corner{background:var(--darkest-color)}body,html{font-family:var(--body-font),sans-serif;font-size:14px;font-weight:400;height:100%;width:100%}body{align-items:stretch;background-color:var(--darkest-color);display:flex;flex-flow:column nowrap;justify-content:stretch;position:relative}header{flex-grow:0;overflow:visible;z-index:5}header,main{box-sizing:border-box;flex-shrink:0;position:relative;width:100%}main{background-position:50%;background-size:cover;flex-grow:1;overflow:auto}footer{align-items:center;background-color:var(--darker-color);box-sizing:border-box;color:var(--lighter-color);display:flex;flex-flow:column nowrap;flex-grow:0;flex-shrink:0;font-size:8px;gap:4px;justify-content:center;padding:5px 0;position:relative;text-align:center;width:100%}.light-background{background-color:var(--lightest-color)}.semi-strong{font-weight:500}.strong,strong{font-weight:700}.black{font-weight:800}.ultra-black{font-weight:900}.half{margin:0 auto;width:50%}.em,em{font-style:italic}em.note{font-size:.75em;margin-top:2px}h1,h2,h3,h4,h5{font-family:var(--header-font),var(--body-font),sans-serif}h1{border-bottom:4px solid var(--theme-color-secondary);font-size:3rem;font-weight:700;line-height:1em;margin:0 0 1em;text-transform:uppercase}h1,h2{color:var(--theme-color-secondary)}h2{font-size:2rem}h2,h3{font-weight:500}h3{font-size:1.5rem;text-align:center}code,pre{font-family:var(--monospace-font),monospace;font-size:12px}.note{color:var(--theme-color-primary);font-size:.8em}fieldset,form{align-items:stretch;display:flex;gap:1em;justify-content:stretch;position:relative}form{flex-flow:column nowrap;padding:1em 1em 0}fieldset{flex-flow:row wrap}fieldset legend{align-items:center;border-bottom:2px solid var(--theme-color-tertiary);color:var(--theme-color-tertiary);display:flex;flex-flow:row nowrap;font-family:var(--header-font),sans-serif;font-size:16px;font-weight:700;justify-content:space-between;margin:0 0 .5em;padding:0 0 3px;width:100%}fieldset .field-container{align-items:stretch;display:flex;flex-basis:100px;flex-flow:column-reverse nowrap;flex-grow:1}fieldset.collapsed .field-container{display:none}fieldset.collapsible legend{cursor:pointer}fieldset.collapsible legend:after{border-bottom:7px solid transparent;border-right:7px solid var(--theme-color-tertiary);border-top:7px solid transparent;content:"\A";display:inline-block;height:0;transform:rotate(-90deg);transform-origin:center;transition:all .25s ease-in-out;width:0}fieldset.collapsed legend:after{transform:rotate(0deg)}fieldset .field-container goodydata-color-input,fieldset .field-container goodydata-search-list,fieldset .field-container input,fieldset .field-container select,fieldset .field-container textarea{flex-grow:1;margin:0;width:100%}fieldset .field-container.hidden-input-view{display:none}form label{color:var(--theme-color-secondary);display:inline-block;flex-grow:0;font-family:var(--header-font),sans-serif;font-size:14px;font-weight:400;margin-bottom:.25em;min-height:12px}form label.required:after{content:"*"}form .submit-buttons{align-items:stretch;display:flex;flex-flow:row nowrap;gap:1em;justify-content:stretch;margin-top:1em;position:relative}form .submit-buttons>*{flex-basis:100%}form input.cancel{background-color:var(--dark-color);border-color:var(--dark-color)}form input.cancel:not(:disabled):not(.disabled):hover{background-color:transparent;color:#fff}form .error{color:tomato}form p.error:not(:empty){margin:0 0 .5em}form>p.error:not(:empty){margin:1em 0 0}form.inline-form{padding:1em}form.inline-form,form.inline-form fieldset{border:none;flex-basis:100%;flex-flow:row nowrap}form.inline-form input[type=submit]{margin:0}form.inline-form fieldset.field-set-flags{flex-basis:30%;flex-grow:0;flex-shrink:0}form.inline-form fieldset legend{display:none}form.inline-form fieldset .field-container{flex-basis:100%;margin-right:4px}form.inline-form fieldset .field-container:not(.checkbox-input-view) label{display:none}form.embedded-form{background-color:rgba(0,0,0,.01);border:1px solid rgba(0,0,0,.2);margin:.5em;padding:1em}.field-container.checkbox-input-view{align-items:center;background-color:var(--theme-color-primary);border-radius:5px;cursor:pointer;display:flex;flex-flow:row nowrap;padding:0 10px;position:relative;transition:background-color .25s ease-in-out}.field-container.checkbox-input-view label{padding:1em 0}.field-container.checkbox-input-view:after{background-color:var(--lightest-color);bottom:0;left:0;opacity:0;pointer-events:none;position:absolute;right:0;top:0;transition:opacity .25s ease-in-out}.field-container.checkbox-input-view:hover:after{opacity:.1}.field-container.checkbox-input-view label{color:var(--lightest-color);cursor:pointer;display:block;flex-grow:1;margin-top:2.5px}.field-container.checkbox-input-view input{flex-grow:0;flex-shrink:0;height:15px;margin-right:5px;width:15px}form.inline-form fieldset .field-container input:not([type=checkbox]),form.inline-form fieldset .field-container select,form.inline-form fieldset .field-container textarea{margin:0}form.inline-form.show-legend{margin-top:.5em}form.inline-form.show-legend fieldset{align-items:center}form.inline-form.show-legend fieldset legend{display:block;position:absolute;top:-25px;width:calc(100% - 5px)}form.inset-form{background-color:var(--theme-color-secondary);border-radius:5px;margin:1em}form.inset-form fieldset legend{border-color:var(--lightest-color);color:var(--lightest-color)}@keyframes loadingBar{0%{left:1em;right:calc(100% - 2em)}50%{left:1em;right:1em}to{left:calc(100% - 2em);right:1em}}@keyframes loadingBarFull{0%{left:0;right:100%}50%{left:0;right:0}to{left:100%;right:0}}.loading-bar{position:relative}.loading-bar:after,form:after{animation-direction:alternate;animation-duration:.75s;animation-iteration-count:infinite;animation-name:loadingBar;animation-timing-function:ease-in-out;background-color:var(--theme-color-primary);border-radius:10px;bottom:0;content:"\A";height:7px;opacity:0;position:absolute;transition:opacity .15s ease-in-out}.loading-bar.loading:after,form.loading:after{opacity:1}a{color:var(--theme-color-primary);cursor:pointer;text-decoration:underline;transition:color .25s ease-in-out}a:hover{color:var(--theme-color-secondary)}input,select,textarea{background-color:var(--darker-color);border:1px solid #000;border-radius:5px;box-sizing:border-box;color:#fff;margin:0 0 1em;outline:none;padding:10px 15px;transition:all .25s ease-in-out}input,option,select,textarea{font-family:var(--body-font),sans-serif}input{padding:11px 15px}input.search{margin:1em;width:calc(100% - 2em)}input[type=file]{background-image:linear-gradient(to right,var(--theme-color-primary),var(--theme-color-primary));background-position:0;background-repeat:no-repeat;background-size:0 100%}input:disabled,select:disabled,textarea:disabled{color:var(--dark-color)}.button,button,input[type=button],input[type=submit]{background-color:var(--theme-color-primary);border:2px solid var(--theme-color-primary);box-sizing:border-box;color:var(--lightest-color);cursor:pointer;display:inline-block;font-family:var(--header-font),sans-serif;font-size:14px;font-weight:700;padding:.75rem 1.5rem;text-align:center;text-decoration:none;text-transform:uppercase;transition:color .25s ease-in-out,background-color .25s ease-in-out}.border-button,button.border-button,input[type=button].border-button,input[type=submit].border-button{background-color:transparent;border:2px solid var(--theme-color-primary);border-radius:2px;box-sizing:border-box;color:#444;cursor:pointer;display:inline-block;padding:.5em;text-align:center;text-decoration:none;transition:color .25s ease-in-out,border-color .25s ease-in-out}.button.disabled,.button:disabled,button.disabled,button:disabled,input[type=button].disabled,input[type=button]:disabled,input[type=submit].disabled,input[type=submit]:disabled{background-color:var(--darker-color);border-color:var(--dark-color);color:var(--dark-color);cursor:default}.border-button.disabled,.border-button:disabled,button.border-button.disabled,button.border-button:disabled,input[type=button].border-button.disabled,input[type=button].border-button:disabled,input[type=submit].border-button.disabled,input[type=submit].border-button:disabled{cursor:default;opacity:.5}.border-button.active,button.border-button.active,input[type=button].border-button.active,input[type=submit].border-button.active{border-color:var(--theme-color-primary);color:var(--theme-color-primary);cursor:default;opacity:1}.button:not(:disabled):not(.disabled):hover,button:not(:disabled):not(.disabled):hover,input[type=button]:not(:disabled):not(.disabled):hover,input[type=submit]:not(:disabled):not(.disabled):hover{background-color:transparent;color:var(--theme-color-primary)}.border-button:not(:disabled):not(.disabled):hover,button.border-button:not(:disabled):not(.disabled):hover,input[type=button].border-button:not(:disabled):not(.disabled):hover,input[type=submit].border-button:not(:disabled):not(.disabled):hover{border-color:var(--theme-color-primary);color:var(--theme-color-primary)}form ul.list-input-view{display:flex;flex-flow:row wrap;gap:6px}form ul.list-input-view li{background-color:transparent;border:2px solid var(--theme-color-primary);border-radius:5px;color:var(--theme-color-primary);cursor:pointer;font-size:12px;font-weight:700;overflow:hidden;padding:8px 14px;transition:color .25s ease-in-out,background-color .25s ease-in-out}form ul.list-input-view li.selected{background-color:var(--theme-color-primary);color:var(--lightest-color)}.loader{position:relative}.loader:after{backdrop-filter:blur(2px);background-image:url(../img/spinner.svg);background-position:50%;background-repeat:no-repeat;background-size:250px auto;bottom:0;content:"\A";left:0;opacity:0;pointer-events:none;position:absolute;right:0;top:0;transition:opacity .4s ease-out;z-index:100}.loader.loader-cover:after{background-color:var(--lightest-color)}.loader.loading:after{opacity:1;pointer-events:auto}.loader.loader-scaled:after{background-size:75% auto}.loader.button:after{animation-direction:alternate;animation-duration:.75s;animation-iteration-count:infinite;animation-name:loadingBarFull;animation-timing-function:ease-in-out;background-color:var(--theme-color-tertiary);background-image:none;z-index:-1}.loader.button.loading{background:none;cursor:not-allowed}.shadowbox-container{align-items:center;backdrop-filter:blur(5px);background-color:rgba(0,0,0,.8);bottom:0;display:flex;flex-flow:row nowrap;justify-content:center;left:0;opacity:0;pointer-events:none;position:fixed;right:0;top:0;transition:opacity .5s ease-in-out;z-index:5}.shadowbox-container.active{opacity:1;pointer-events:auto}.shadowbox-container .box-container{background-color:#fff;padding:20px;width:calc(100% - 40px);z-index:6}.shadowbox-container .box-container a.close-shadowbox{color:#0146ad;cursor:pointer;display:block;font-size:30px;font-weight:900;margin-right:-5px;margin-top:-21px;padding-right:10px;text-align:right;text-decoration:none;z-index:7}.shadowbox-container iframe{border:none;outline:none;z-index:7}.tooltip-container{background-color:var(--darker-color);border:1px solid var(--light-color);border-radius:5px;color:var(--light-color);font-weight:300;max-width:75vw;opacity:0;padding:10px;pointer-events:none;position:fixed;transition:opacity .25s ease-in-out;white-space:break-spaces;z-index:5}.tooltip-container.active{opacity:1}.tooltip-container>p:not(:last-child){margin-bottom:1em}.notification-container{align-items:center;display:flex;flex-flow:row nowrap;justify-content:center;opacity:1;padding:5px;pointer-events:none;position:fixed;top:0;transition:opacity .5s ease-in-out;width:100%;z-index:6}.notification-container .notification{background-color:var(--darker-color);border:1px solid var(--light-color);border-radius:5px;color:var(--light-color);font-size:12px;font-weight:600;padding:10px}@keyframes slide-background{0%{background-position:0 0}to{background-position:100vw 0}}.sliding-gradient{animation-delay:0s;animation-duration:10s;animation-iteration-count:infinite;animation-name:slide-background;animation-timing-function:linear;background:linear-gradient(to right,var(--theme-color-primary),var(--theme-color-secondary),var(--theme-color-tertiary),var(--theme-color-primary));background-size:100vw 100%}@media (max-width:1024px){h1{font-size:3rem}h2{font-size:2rem}h3{font-size:1.5rem}}@media (max-width:768px){h1{font-size:2.5rem}}
+:not(i),:not(i):after,:not(i):before{box-sizing:border-box}*{scrollbar-color:rgba(0,0,0,.25),transparent;scrollbar-width:thin}::-webkit-scrollbar{background:var(--darkest-color);height:14px;width:14px}::-webkit-scrollbar-thumb{background-clip:padding-box;background-color:hsla(0,0%,100%,.25);border:4px solid hsla(0,0%,100%,0);border-radius:7px;box-shadow:inset -1px -1px 0 rgba(0,0,0,.05),inset 1px 1px 0 rgba(0,0,0,.05);height:6px}::-webkit-scrollbar-thumb:hover{background-color:hsla(0,0%,100%,.35)}::-webkit-scrollbar-button{display:none;height:0;width:0}::-webkit-scrollbar-corner{background:var(--darkest-color)}body,html{font-family:var(--body-font),sans-serif;font-size:14px;font-weight:400;height:100%;width:100%}body{align-items:stretch;background-color:var(--darkest-color);display:flex;flex-flow:column nowrap;justify-content:stretch;position:relative}header{flex-grow:0;overflow:visible;z-index:5}header,main{box-sizing:border-box;flex-shrink:0;position:relative;width:100%}main{background-position:50%;background-size:cover;flex-grow:1;overflow:auto}footer{align-items:center;background-color:var(--darker-color);box-sizing:border-box;color:var(--lighter-color);display:flex;flex-flow:column nowrap;flex-grow:0;flex-shrink:0;font-size:8px;gap:4px;justify-content:center;padding:5px 0;position:relative;text-align:center;width:100%}.light-background{background-color:var(--lightest-color)}.semi-strong{font-weight:500}.strong,strong{font-weight:700}.black{font-weight:800}.ultra-black{font-weight:900}.half{margin:0 auto;width:50%}.em,em{font-style:italic}em.note{font-size:.75em;margin-top:2px}h1,h2,h3,h4,h5{font-family:var(--header-font),var(--body-font),sans-serif}h1{border-bottom:4px solid var(--theme-color-secondary);font-size:3rem;font-weight:700;line-height:1em;margin:0 0 1em;text-transform:uppercase}h1,h2{color:var(--theme-color-secondary)}h2{font-size:2rem}h2,h3{font-weight:500}h3{font-size:1.5rem;text-align:center}code,pre{font-family:var(--monospace-font),monospace;font-size:12px}.note{color:var(--theme-color-primary);font-size:.8em}fieldset,form{align-items:stretch;display:flex;gap:1em;justify-content:stretch;position:relative}form{flex-flow:column nowrap;padding:1em 1em 0}fieldset{flex-flow:row wrap}fieldset legend{align-items:center;border-bottom:2px solid var(--theme-color-tertiary);color:var(--theme-color-tertiary);display:flex;flex-flow:row nowrap;font-family:var(--header-font),sans-serif;font-size:16px;font-weight:700;justify-content:space-between;margin:0 0 .5em;padding:0 0 3px;width:100%}fieldset .field-container{align-items:stretch;display:flex;flex-basis:100px;flex-flow:column-reverse nowrap;flex-grow:1}fieldset.collapsed .field-container{display:none}fieldset.collapsible legend{cursor:pointer}fieldset.collapsible legend:after{border-bottom:7px solid transparent;border-right:7px solid var(--theme-color-tertiary);border-top:7px solid transparent;content:"\A";display:inline-block;height:0;transform:rotate(-90deg);transform-origin:center;transition:all .25s ease-in-out;width:0}fieldset.collapsed legend:after{transform:rotate(0deg)}fieldset .field-container goodydata-color-input,fieldset .field-container goodydata-search-list,fieldset .field-container input,fieldset .field-container select,fieldset .field-container textarea{flex-grow:1;margin:0;width:100%}fieldset .field-container.hidden-input-view{display:none}form label{color:var(--theme-color-secondary);display:inline-block;flex-grow:0;font-family:var(--header-font),sans-serif;font-size:14px;font-weight:400;margin-bottom:.25em;min-height:12px}form label.required:after{content:"*"}form .submit-buttons{align-items:stretch;display:flex;flex-flow:row nowrap;gap:1em;justify-content:stretch;margin-top:1em;position:relative}form .submit-buttons>*{flex-basis:100%}form input.cancel{background-color:var(--dark-color);border-color:var(--dark-color)}form input.cancel:not(:disabled):not(.disabled):hover{background-color:transparent;color:#fff}form .error{color:tomato}form p.error:not(:empty){margin:0 0 .5em}form>p.error:not(:empty){margin:1em 0 0}form.inline-form{padding:1em}form.inline-form,form.inline-form fieldset{border:none;flex-basis:100%;flex-flow:row nowrap}form.inline-form input[type=submit]{margin:0}form.inline-form fieldset.field-set-flags{flex-basis:30%;flex-grow:0;flex-shrink:0}form.inline-form fieldset legend{display:none}form.inline-form fieldset .field-container{flex-basis:100%;margin-right:4px}form.inline-form fieldset .field-container:not(.checkbox-input-view) label{display:none}form.embedded-form{background-color:rgba(0,0,0,.01);border:1px solid rgba(0,0,0,.2);margin:.5em;padding:1em}.field-container.checkbox-input-view{align-items:center;background-color:var(--theme-color-primary);border-radius:5px;cursor:pointer;display:flex;flex-flow:row nowrap;padding:0 10px;position:relative;transition:background-color .25s ease-in-out}.field-container.checkbox-input-view label{padding:1em 0}.field-container.checkbox-input-view:after{background-color:var(--lightest-color);bottom:0;left:0;opacity:0;pointer-events:none;position:absolute;right:0;top:0;transition:opacity .25s ease-in-out}.field-container.checkbox-input-view:hover:after{opacity:.1}.field-container.checkbox-input-view label{color:var(--lightest-color);cursor:pointer;display:block;flex-grow:1;margin-top:2.5px}.field-container.checkbox-input-view input{flex-grow:0;flex-shrink:0;height:15px;margin-right:5px;width:15px}form.inline-form fieldset .field-container input:not([type=checkbox]),form.inline-form fieldset .field-container select,form.inline-form fieldset .field-container textarea{margin:0}form.inline-form.show-legend{margin-top:.5em}form.inline-form.show-legend fieldset{align-items:center}form.inline-form.show-legend fieldset legend{display:block;position:absolute;top:-25px;width:calc(100% - 5px)}form.inset-form{background-color:var(--theme-color-secondary);border-radius:5px;margin:1em}form.inset-form fieldset legend{border-color:var(--lightest-color);color:var(--lightest-color)}@keyframes loadingBar{0%{left:1em;right:calc(100% - 2em)}50%{left:1em;right:1em}to{left:calc(100% - 2em);right:1em}}@keyframes loadingBarFull{0%{left:0;right:100%}50%{left:0;right:0}to{left:100%;right:0}}.loading-bar{position:relative}.loading-bar:after,form:after{animation-direction:alternate;animation-duration:.75s;animation-iteration-count:infinite;animation-name:loadingBar;animation-timing-function:ease-in-out;background-color:var(--theme-color-primary);border-radius:10px;bottom:0;content:"\A";height:7px;opacity:0;position:absolute;transition:opacity .15s ease-in-out}.loading-bar.loading:after,form.loading:after{opacity:1}a{color:var(--theme-color-primary);cursor:pointer;text-decoration:underline;transition:color .25s ease-in-out}a:hover{color:var(--theme-color-secondary)}input,select,textarea{background-color:var(--darker-color);border:1px solid #000;border-radius:5px;box-sizing:border-box;color:#fff;margin:0 0 1em;outline:none;padding:10px 15px;transition:all .25s ease-in-out}input,option,select,textarea{font-family:var(--body-font),sans-serif}input{padding:11px 15px}input.search{margin:1em;width:calc(100% - 2em)}input[type=file]{background-image:linear-gradient(to right,var(--theme-color-primary),var(--theme-color-primary));background-position:0;background-repeat:no-repeat;background-size:0 100%}input:disabled,select:disabled,textarea:disabled{color:var(--dark-color)}.button,button,input[type=button],input[type=submit]{background-color:var(--theme-color-primary);border:2px solid var(--theme-color-primary);box-sizing:border-box;color:var(--lightest-color);cursor:pointer;display:inline-block;font-family:var(--header-font),sans-serif;font-size:14px;font-weight:700;padding:.75rem 1.5rem;text-align:center;text-decoration:none;text-transform:uppercase;transition:color .25s ease-in-out,background-color .25s ease-in-out}.border-button,button.border-button,input[type=button].border-button,input[type=submit].border-button{background-color:transparent;border:2px solid var(--theme-color-primary);border-radius:2px;box-sizing:border-box;color:#444;cursor:pointer;display:inline-block;padding:.5em;text-align:center;text-decoration:none;transition:color .25s ease-in-out,border-color .25s ease-in-out}.button.disabled,.button:disabled,button.disabled,button:disabled,input[type=button].disabled,input[type=button]:disabled,input[type=submit].disabled,input[type=submit]:disabled{background-color:var(--darker-color);border-color:var(--dark-color);color:var(--dark-color);cursor:default}.border-button.disabled,.border-button:disabled,button.border-button.disabled,button.border-button:disabled,input[type=button].border-button.disabled,input[type=button].border-button:disabled,input[type=submit].border-button.disabled,input[type=submit].border-button:disabled{cursor:default;opacity:.5}.border-button.active,button.border-button.active,input[type=button].border-button.active,input[type=submit].border-button.active{border-color:var(--theme-color-primary);color:var(--theme-color-primary);cursor:default;opacity:1}.button:not(:disabled):not(.disabled):hover,button:not(:disabled):not(.disabled):hover,input[type=button]:not(:disabled):not(.disabled):hover,input[type=submit]:not(:disabled):not(.disabled):hover{background-color:transparent;color:var(--theme-color-primary)}.border-button:not(:disabled):not(.disabled):hover,button.border-button:not(:disabled):not(.disabled):hover,input[type=button].border-button:not(:disabled):not(.disabled):hover,input[type=submit].border-button:not(:disabled):not(.disabled):hover{border-color:var(--theme-color-primary);color:var(--theme-color-primary)}form ul.list-input-view{display:flex;flex-flow:row wrap;gap:6px}form ul.list-input-view li{background-color:transparent;border:2px solid var(--theme-color-primary);border-radius:5px;color:var(--theme-color-primary);cursor:pointer;font-size:12px;font-weight:700;overflow:hidden;padding:8px 14px;transition:color .25s ease-in-out,background-color .25s ease-in-out}form ul.list-input-view li.selected{background-color:var(--theme-color-primary);color:var(--lightest-color)}.loader{position:relative}.loader:after{backdrop-filter:blur(2px);background-position:50%;background-repeat:no-repeat;background-size:250px auto;bottom:0;content:"\A";left:0;opacity:0;pointer-events:none;position:absolute;right:0;top:0;transition:opacity .4s ease-out;z-index:100}.loader.loader-cover:after{background-color:var(--lightest-color)}.loader.loading:after{opacity:1;pointer-events:auto}.loader.loader-scaled:after{background-size:75% auto}.loader.button:after{animation-direction:alternate;animation-duration:.75s;animation-iteration-count:infinite;animation-name:loadingBarFull;animation-timing-function:ease-in-out;background-color:var(--theme-color-tertiary);background-image:none;z-index:-1}.loader.button.loading{background:none;cursor:not-allowed}.shadowbox-container{align-items:center;backdrop-filter:blur(5px);background-color:rgba(0,0,0,.8);bottom:0;display:flex;flex-flow:row nowrap;justify-content:center;left:0;opacity:0;pointer-events:none;position:fixed;right:0;top:0;transition:opacity .5s ease-in-out;z-index:5}.shadowbox-container.active{opacity:1;pointer-events:auto}.shadowbox-container .box-container{background-color:#fff;padding:20px;width:calc(100% - 40px);z-index:6}.shadowbox-container .box-container a.close-shadowbox{color:#0146ad;cursor:pointer;display:block;font-size:30px;font-weight:900;margin-right:-5px;margin-top:-21px;padding-right:10px;text-align:right;text-decoration:none;z-index:7}.shadowbox-container iframe{border:none;outline:none;z-index:7}.tooltip-container{background-color:var(--darker-color);border:1px solid var(--light-color);border-radius:5px;color:var(--light-color);font-weight:300;max-width:75vw;opacity:0;padding:10px;pointer-events:none;position:fixed;transition:opacity .25s ease-in-out;white-space:break-spaces;z-index:99}.tooltip-container.active{opacity:1}.tooltip-container>p:not(:last-child){margin-bottom:1em}.notification-container{align-items:center;display:flex;flex-flow:row nowrap;justify-content:center;opacity:1;padding:5px;pointer-events:none;position:fixed;top:0;transition:opacity .5s ease-in-out;width:100%;z-index:6}.notification-container .notification{background-color:var(--darker-color);border:1px solid var(--light-color);border-radius:5px;color:var(--light-color);font-size:12px;font-weight:600;padding:10px}@keyframes slide-background{0%{background-position:0 0}to{background-position:100vw 0}}.sliding-gradient{animation-delay:0s;animation-duration:10s;animation-iteration-count:infinite;animation-name:slide-background;animation-timing-function:linear;background:linear-gradient(to right,var(--theme-color-primary),var(--theme-color-secondary),var(--theme-color-tertiary),var(--theme-color-primary));background-size:100vw 100%}@media (max-width:1024px){h1{font-size:3rem}h2{font-size:2rem}h3{font-size:1.5rem}}@media (max-width:768px){h1{font-size:2.5rem}}
```

### Comparing `enfugue-0.1.2/enfugue/static/css/05-common.min.css` & `enfugue-0.1.3/enfugue/static/css/05-common.min.css`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/css/06-header.min.css` & `enfugue-0.1.3/enfugue/static/css/06-header.min.css`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/css/07-main.min.css` & `enfugue-0.1.3/enfugue/static/css/07-main.min.css`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/css/08-enfugue.min.css` & `enfugue-0.1.3/enfugue/static/css/08-enfugue.min.css`

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
-enfugue-application{display:block;height:100%;left:0;position:absolute;top:0;width:100%}enfugue-application>enfugue-node-editor{bottom:0;height:auto;left:0;position:absolute;right:0;top:35px;width:auto}enfugue-application>enfugue-node-editor.image-editor{bottom:30px;left:40px;right:300px;z-index:3}enfugue-application>enfugue-node-editor.windows{z-index:4}enfugue-menu{align-items:stretch;background-color:var(--dark-color);border-bottom:1px solid rgba(0,0,0,.2);display:flex;flex-flow:row nowrap;height:35px;left:0;line-height:35px;position:absolute;right:0;text-shadow:1px 1px 0 rgba(0,0,0,.2);top:0;z-index:5}enfugue-menu-category{background-color:transparent;border-right:1px solid rgba(0,0,0,.2);cursor:pointer;font-weight:100;width:80px}enfugue-menu-category:hover{background-color:hsla(0,0%,100%,.1)}enfugue-menu>enfugue-menu-category:not(:first-of-type){border-left:1px solid hsla(0,0%,100%,.1)}enfugue-menu-category-header,enfugue-menu-item{font-family:var(--monospace-font),monospace;padding:0 5px}enfugue-menu-item{align-items:center;background-color:var(--dark-color);border-color:hsla(0,0%,100%,.1) rgba(0,0,0,.2) rgba(0,0,0,.2) hsla(0,0%,100%,.1);border-style:solid;border-width:1px;color:var(--theme-color-tertiary);cursor:pointer;display:flex;flex-direction:row-reverse;flex-wrap:nowrap;font-size:14px;font-weight:200;justify-content:space-between;width:150px}enfugue-menu-category:not(.active)>enfugue-menu-item{display:none}enfugue-menu-category>enfugue-menu-item:first-of-type{margin-top:-1px}enfugue-menu-item:hover{color:var(--lightest-color)}enfugue-menu-item.active{border-bottom-color:var(--theme-color-tertiary)}enfugue-menu-item i{font-size:18px}enfugue-sidebar{align-items:stretch;background-color:var(--dark-color);border-bottom:1px solid rgba(0,0,0,.2);border-left:1px solid hsla(0,0%,100%,.1);border-top:1px solid hsla(0,0%,100%,.1);bottom:30px;display:flex;flex-flow:column nowrap;flex-grow:0;flex-shrink:0;justify-content:flex-start;overflow-y:auto;position:absolute;right:0;top:35px;width:300px}enfugue-sidebar::-webkit-scrollbar{background:var(--dark-color)}enfugue-sidebar::-webkit-scrollbar-thumb{background-color:rgba(0,0,0,.55)}enfugue-sidebar::-webkit-scrollbar-thumb:hover{background-color:rgba(0,0,0,.7)}enfugue-sidebar input.invoke{margin:auto 1em 1em}enfugue-sidebar .invoke-loader{margin:-16px 2px 16px;pointer-events:none}enfugue-sidebar .invoke-loader.loading-bar:after{border-bottom-left-radius:4px;border-bottom-right-radius:4px;border-top-left-radius:0;border-top-right-radius:0}enfugue-toolbar{background-color:var(--dark-color);border-right:1px solid rgba(0,0,0,.2);border-top:1px solid hsla(0,0%,100%,.1);bottom:30px;flex-flow:column nowrap;justify-content:flex-start;left:0;padding:0;position:absolute;top:35px;z-index:3}enfugue-toolbar,enfugue-toolbar-item{align-items:center;border-bottom:1px solid rgba(0,0,0,.2);display:flex;width:40px}enfugue-toolbar-item{cursor:pointer;flex-flow:row nowrap;height:40px;justify-content:center;position:relative}enfugue-toolbar enfugue-toolbar-item:not(:first-child){border-top:1px solid hsla(0,0%,100%,.1)}enfugue-toolbar-item>span{display:none}enfugue-toolbar-item>i{font-size:25px}enfugue-toolbar-item:after{background-color:hsla(0,0%,100%,0);bottom:0;content:"\A";display:block;left:0;position:absolute;right:0;top:0}enfugue-toolbar-item:not(.disabled):not(:disabled):hover:after{background-color:hsla(0,0%,100%,.1)}enfugue-toolbar-item:not(.disabled):not(:disabled):active{border-bottom:1px solid rgba(0,0,0,.2)}enfugue-tabbed-view{display:block}enfugue-tabs{align-items:stretch;display:flex;flex-flow:row nowrap;justify-content:stretch}enfugue-tabs enfugue-tab{align-items:center;background-color:transparent;color:var(--theme-color-secondary);cursor:pointer;display:flex;flex-flow:row nowrap;flex-grow:0;font-family:var(--header-font);font-size:15px;font-weight:300;justify-content:center;padding:.75em;transition:background-color .25s ease-in-out,color .25s ease-in-out;transition:all .25s ease-in-out}enfugue-tabs enfugue-tab.active{background-color:var(--theme-color-secondary);color:var(--lightest-color);flex-grow:1;font-weight:700}enfugue-tab-content{border-top:3px solid var(--theme-color-secondary);display:block}enfugue-sidebar-category-header,enfugue-sidebar-item{align-items:center;border-bottom:1px solid rgba(0,0,0,.2);border-top:1px solid hsla(0,0%,100%,.15);color:var(--theme-color-secondary);cursor:pointer;display:flex;flex-direction:row;flex-wrap:nowrap;font-size:14px;font-weight:700;height:45px;padding:0 10px;position:relative;text-transform:uppercase}enfugue-sidebar-category-header:before,enfugue-sidebar-item:before{background-color:#000;bottom:0;content:"\A";display:block;left:0;opacity:0;pointer-events:none;position:absolute;right:0;top:0;transition:opacity .2s ease-in-out}enfugue-sidebar-category-header:hover:before,enfugue-sidebar-item:hover:before{opacity:.1}enfugue-sidebar-category-header:after{content:"\f054";flex-grow:1;font-family:Font Awesome\ 6 Free;font-weight:900;text-align:right}enfugue-sidebar-category.active>enfugue-sidebar-category-header:after{content:"\f078"}enfugue-sidebar-category-header enfugue-sidebar-category-button{cursor:pointer;font-size:16px;margin-left:10px;opacity:.75;transition:opacity .25s ease-in-out}enfugue-sidebar-category-header enfugue-sidebar-category-button:hover{opacity:1}enfugue-sidebar-item{background-color:var(--theme-color-primary);flex-direction:row-reverse}enfugue-menu-item.loading-bar:after,enfugue-sidebar-item.loading-bar:after{bottom:3px;height:5px;margin-left:-5px;margin-right:-5px}enfugue-sidebar-item.disabled{background-color:#aaa}enfugue-sidebar-item i{flex-grow:1;font-size:18px;text-align:right}enfugue-notification-center{bottom:0;display:flex;flex-flow:column-reverse nowrap;justify-content:flex-start;left:66%;pointer-events:none;position:fixed;right:0;top:0;z-index:6}enfugue-notification{backdrop-filter:blur(10px);background-color:rgba(0,0,0,.4);border:1px solid var(--darker-color);border-radius:2px;box-shadow:2px 2px 8px rgba(0,0,0,.3);color:var(--light-color);display:flex;flex-flow:column nowrap;height:150px;margin:1em;padding:1em;pointer-events:auto;position:relative;transition:all .5s ease-in-out}enfugue-notification i{cursor:pointer;font-size:18px;opacity:.75;position:absolute;right:1em;top:11px;transition:opacity .25s ease-in-out}enfugue-notification i:hover{opacity:1}enfugue-notification p{flex-basis:100%;font-size:13px;overflow-y:auto}enfugue-notification.hiding{height:0;margin:0 1em;opacity:0;padding:0 1em}enfugue-notification.hiding,enfugue-notification.hiding p{overflow:hidden}enfugue-notification h2{border-bottom:1px solid var(--lightest-color);color:var(--lightest-color);font-size:24px;font-weight:700;margin-bottom:.5em;text-transform:uppercase}enfugue-notification:not(:last-child){margin-top:0}enfugue-notification.info h2{border-color:rgba(92,184,92,.9);color:rgba(92,184,92,.75)}enfugue-notification.warn h2{border-color:rgba(240,173,78,.9);color:rgba(240,173,78,.75)}enfugue-notification.error h2{border-color:rgba(217,83,79,.9);color:rgba(217,83,79,.75)}enfugue-color-input,enfugue-repeatable-input,enfugue-search-list{align-items:center;background-color:var(--darker-color);border:1px solid #000;border-radius:5px;display:flex;flex-flow:row wrap;gap:5px;outline:none;padding:5px;position:relative;width:100%}enfugue-color-input{flex-flow:row nowrap}enfugue-search-list>enfugue-search-list-selection{align-items:center;background-color:var(--theme-color-primary);border-left:3px solid transparent;border-radius:2px;border-right:3px solid transparent;box-sizing:border-box;color:var(--lightest-color);display:flex;flex-flow:row nowrap;font-size:12px;justify-content:center;opacity:1;padding:5px 10px 5px 5px;position:relative;transition:border-color .1s ease-in-out,opacity .25s ease-in-out}enfugue-search-list>enfugue-search-list-selection span{font-weight:700}enfugue-search-list>enfugue-search-list-selection.dragged{opacity:.5}enfugue-search-list>enfugue-search-list-selection.drop-left{border-left:3px solid var(--dark-color)}enfugue-search-list>enfugue-search-list-selection.drop-right{border-right:3px solid var(--dark-color)}enfugue-search-list>enfugue-search-list-selection>button{background-color:var(--lightest-color);border-radius:20px;border-width:0;color:var(--theme-color-primary);height:15px;line-height:0;margin-right:5px;padding:0;width:15px}enfugue-search-list>enfugue-search-list-selection>button:not(:disabled):not(.disabled):hover{background-color:var(--theme-color-primary);color:var(--lightest-color)}enfugue-color-input>input,enfugue-search-list>input{border:none;flex-grow:1;margin:0;padding:5px}enfugue-color-input>.inline-color-preview{border:1px solid #000;border-radius:5px;cursor:pointer;height:20px;width:20px}enfugue-color-input-helper-view,ul.enfugue-search-list-items{background-color:var(--darker-color);border:1px solid var(--darkest-color);border-bottom-left-radius:5px;border-bottom-right-radius:5px;border-top:none;color:var(--light-color);max-height:400px;max-height:250px;min-height:40px;overflow-y:auto;position:fixed;z-index:10}enfugue-color-input-helper-view .preview-input-container{align-items:stretch;display:flex;flex-flow:row nowrap;gap:5px;justify-content:stretch;padding:5px}enfugue-color-input-helper-view .preview-input-container .preview{align-items:center;display:flex;flex-basis:25%;flex-flow:column nowrap;font-weight:700;gap:1em;justify-content:center;text-transform:uppercase}enfugue-color-input-helper-view .preview-input-container .input-container{align-items:center;display:flex;flex-basis:100%;flex-flow:column nowrap;gap:5px;justify-content:center}enfugue-color-input-helper-view .preview-input-container .input-container .input-part,enfugue-color-input-helper-view .preview-input-container .preview{border:1px solid #ccc;border-radius:5px}enfugue-color-input-helper-view .preview-input-container .input-container .input-part{cursor:pointer;height:30px;position:relative;width:100%}enfugue-color-input-helper-view .preview-input-container .input-container .input-part .indicator{border:1px solid #ccc;bottom:-5px;left:0;margin-left:-5px;pointer-events:none;position:absolute;top:-5px;width:10px}ul.enfugue-search-list-items>li{align-items:center;background-color:var(--darker-color);cursor:pointer;display:flex;flex-flow:row nowrap;font-size:12px;justify-content:flex-start;padding:.5em;position:relative;transition:all .25s ease-in-out}ul.enfugue-search-list-items>li:hover{background-color:var(--darkest-color)}ul.enfugue-search-list-items>li:not(:last-child){border-bottom:1px solid var(--darkest-color)}ul.enfugue-multi-search-list-items>li:before{border:1px solid #ccc;border-radius:2px;color:var(--theme-color-tertiary);content:"\A";display:block;font-weight:700;height:14px;margin-right:4px;padding:0;text-align:center;vertical-align:middle;width:14px}ul.enfugue-multi-search-list-items>li.selected:before{border-color:var(--theme-color-tertiary);content:"✓"}enfugue-repeatable-input input.add-item{flex-grow:0}enfugue-repeatable-input enfugue-repeatable-input-item{display:block;position:relative;width:100%}enfugue-repeatable-input enfugue-repeatable-input-item input.remove-item{border-radius:15px;height:15px;line-height:0;margin:0;padding:0;position:absolute;right:-2px;text-align:center;top:-2px;width:15px}enfugue-repeatable-input enfugue-repeatable-input-item input.remove-item.disabled{opacity:.33}enfugue-repeatable-input.columns{align-items:stretch;flex-flow:column nowrap}enfugue-repeatable-input.columns enfugue-repeatable-input-item{margin-bottom:5px}enfugue-repeatable-input enfugue-repeatable-input-item>form.inset-form{padding:10px}enfugue-repeatable-input enfugue-repeatable-input-item>form.inset-form fieldset:not(:last-child){margin-bottom:10px}enfugue-repeatable-input enfugue-repeatable-input-item>form.inset-form fieldset .field-container:not(:last-child){margin-bottom:5px}enfugue-repeatable-input enfugue-repeatable-input-item>form{gap:0;margin:0;padding:5px}enfugue-repeatable-input.columns input.add-item{width:calc(100% - 5px)}enfugue-repeatable-input.columns input.remove-item{background-color:#000;border-color:#000}enfugue-repeatable-input.columns input.remove-item:not(:disabled):not(.disabled):hover{color:#000}form.model-picker{align-items:center;display:flex;flex-flow:row nowrap;justify-content:center;left:40px;padding:5px 0 0 5px;position:absolute;top:35px;width:auto;z-index:3}form.model-picker fieldset{width:250px}form.model-picker fieldset legend{display:none}form.model-picker div#tensorrt{cursor:pointer;height:22px;margin-left:-64px;position:relative;transition:all .25s ease-in-out}form.model-picker div#tensorrt img{filter:grayscale(100%);height:22px}form.model-picker div#tensorrt:hover img{filter:grayscale(75%)}form.model-picker div#tensorrt.ready img{filter:grayscale(0)}form.model-picker div#tensorrt span.fraction{border-radius:20px;color:#000;display:block;font-size:10px;height:20px;position:absolute;right:13px;text-align:center;top:0;width:20px}form.model-picker div#tensorrt span.fraction:after{background-color:#000;content:"\A";height:1px;left:5px;position:absolute;top:10px;transform:rotate(-62deg);width:10px}form.model-picker div#tensorrt span.fraction>span:first-child{display:block;left:3px;position:absolute;top:2px}form.model-picker div#tensorrt span.fraction>span:last-child{bottom:1px;display:block;position:absolute;right:3px}form.model-picker enfugue-search-list{margin:0}.page-buttons{align-items:center;display:flex;flex-flow:row nowrap;gap:5px;justify-content:stretch;margin:1em;width:calc(100% - 2em)}.page-buttons>*{flex-basis:100%;text-align:center}enfugue-status{align-items:center;color:var(--light-color);display:flex;flex-flow:row nowrap;font-size:10px;font-weight:900;gap:5px;height:100%;justify-content:space-between;padding:0 5px 0 50px;text-shadow:1px 1px 0 rgba(0,0,0,.8);transition:all .25s ease-in-out}enfugue-status-version:before{content:"VERSION: ";font-weight:200}enfugue-status-uptime:before{content:"UPTIME: ";font-weight:200}enfugue-status-gpu-name:before{content:"GPU: ";font-weight:200}enfugue-status-gpu-load:before{color:var(--light-color);content:"LOAD: ";font-weight:200}enfugue-status-gpu-load:after{content:"%";font-weight:200}enfugue-status-gpu-temp:before{color:var(--light-color);content:"TEMP: ";font-weight:200}enfugue-status-gpu-temp:after{content:"°C";font-weight:200}enfugue-status-gpu-memory:before{content:"MEM: ";font-weight:200}enfugue-status-icon{background-color:var(--dark-color);border:1px solid var(--darkest-color);border-radius:14px;display:inline-block;height:14px;width:14px}enfugue-status-gpu-memory{border:1px solid var(--dark-color);border-radius:4px;display:inline-block;padding:4px}enfugue-status-icon.idle{background-color:#999;cursor:not-allowed}enfugue-status-icon.ready{background-color:#4bb543;cursor:pointer}enfugue-status-icon.error{background-color:#f33;cursor:not-allowed}enfugue-status-icon.busy{background-color:#e9d502;cursor:pointer}enfugue-downloads{display:flex;flex-flow:column-reverse nowrap;gap:1em;padding:1em}enfugue-download{display:flex;flex-flow:column nowrap;gap:2px}enfugue-download-name{color:var(--theme-color-secondary);display:block;font-family:var(--header-font);font-size:1.5em}enfugue-download-progress{border-radius:2px;display:block;height:2px;width:100%}enfugue-download-size,enfugue-download-time{display:block;font-weight:300}enfugue-download-status{background-color:rgba(0,0,0,.6);border-radius:22px;color:hsla(0,0%,100%,.8);cursor:pointer;display:block;height:22px;line-height:22px;margin-left:auto;margin-right:-40px;position:relative;text-align:center;width:22px}enfugue-download-count{background-color:var(--dark-color);border-radius:12px;color:var(--light-color);font-size:10px;height:12px;line-height:12px;position:absolute;right:-2px;text-align:center;top:-2px;width:12px}enfugue-download-status.inactive{background:none!important;opacity:.5}enfugue-scribble-view{bottom:0;cursor:default;display:block;left:0;position:absolute;right:0;top:0;z-index:0}enfugue-scribble-view canvas{image-rendering:pixelated;position:relative;z-index:-1}enfugue-model-table-searching{display:block;margin:0;padding:1em 1em 0 0;text-align:right}enfugue-model-table-searching input{margin:0}enfugue-image-inspector{cursor:default;display:block;overflow:hidden;position:relative;text-align:center}enfugue-image-inspector .image-view-container{display:block;max-height:100%;overflow:hidden}enfugue-image-inspector .down,enfugue-image-inspector .left,enfugue-image-inspector .right,enfugue-image-inspector .up{align-items:center;display:flex;flex-flow:row nowrap;justify-content:center;opacity:0;pointer-events:none;position:absolute;transition:all .25s ease-in-out}enfugue-image-inspector .down.active,enfugue-image-inspector .left.active,enfugue-image-inspector .right.active,enfugue-image-inspector .up.active{font-size:40px;opacity:.5}enfugue-image-inspector .up{background-image:linear-gradient(0deg,transparent,#000);height:40px;left:0;right:0;top:0}enfugue-image-inspector .down{background-image:linear-gradient(180deg,transparent,#000);bottom:0;height:40px;left:0;position:absolute;right:0}enfugue-image-inspector .left{background-image:linear-gradient(270deg,transparent,#000);bottom:0;left:0;position:absolute;top:0;width:40px}enfugue-image-inspector .right{background-image:linear-gradient(90deg,transparent,#000);bottom:0;position:absolute;right:0;top:0;width:40px}enfugue-image-details{color:#000;font-family:var(--monospace-font),monospace;font-size:10px;position:absolute;right:5px;text-align:right;text-shadow:1px 1px 0 #fff;top:107px}enfugue-image-browser{box-shadow:0 0 10px rgba(0,0,0,.6);cursor:pointer;height:100px;opacity:.5;position:absolute;right:5px;top:5px;transition:all .25s ease-in-out}enfugue-image-browser:hover{opacity:1}enfugue-image-browser img{height:100%;pointer-events:none}enfugue-image-browser span{border:1px solid #fff;box-shadow:inset 0 0 1px #000;left:0;margin:0;max-height:100%;max-width:100%;padding:0;pointer-events:none;position:absolute;top:0}
+enfugue-application{display:block;height:100%;left:0;position:absolute;top:0;width:100%}enfugue-application>enfugue-node-editor{bottom:0;height:auto;left:0;position:absolute;right:0;top:35px;width:auto}enfugue-application>enfugue-node-editor.image-editor{bottom:30px;left:40px;right:300px;z-index:3}enfugue-application>enfugue-node-editor.windows{z-index:5}enfugue-menu{align-items:stretch;background-color:var(--dark-color);border-bottom:1px solid rgba(0,0,0,.2);display:flex;flex-flow:row nowrap;height:35px;left:0;line-height:35px;position:absolute;right:0;text-shadow:1px 1px 0 rgba(0,0,0,.2);top:0;z-index:6}enfugue-menu-category{background-color:transparent;border-right:1px solid rgba(0,0,0,.2);cursor:pointer;font-weight:100;width:80px}enfugue-menu-category:hover{background-color:hsla(0,0%,100%,.1)}enfugue-menu>enfugue-menu-category:not(:first-of-type){border-left:1px solid hsla(0,0%,100%,.1)}enfugue-menu-category-header,enfugue-menu-item{font-family:var(--monospace-font),monospace;padding:0 5px}enfugue-menu-item{align-items:center;background-color:var(--dark-color);border-color:hsla(0,0%,100%,.1) rgba(0,0,0,.2) rgba(0,0,0,.2) hsla(0,0%,100%,.1);border-style:solid;border-width:1px;color:var(--theme-color-tertiary);cursor:pointer;display:flex;flex-direction:row-reverse;flex-wrap:nowrap;font-size:14px;font-weight:200;justify-content:space-between;width:200px}enfugue-menu-category:not(.active)>enfugue-menu-item{display:none}enfugue-menu-category>enfugue-menu-item:first-of-type{margin-top:-1px}enfugue-menu-item:hover{color:var(--lightest-color)}enfugue-menu-item.active{border-bottom-color:var(--theme-color-tertiary)}enfugue-menu-item i{font-size:18px}enfugue-sidebar{align-items:stretch;background-color:var(--dark-color);border-bottom:1px solid rgba(0,0,0,.2);border-left:1px solid hsla(0,0%,100%,.1);border-top:1px solid hsla(0,0%,100%,.1);bottom:30px;display:flex;flex-flow:column nowrap;flex-grow:0;flex-shrink:0;justify-content:flex-start;overflow-y:auto;position:absolute;right:0;top:35px;width:300px}enfugue-sidebar::-webkit-scrollbar{background:var(--dark-color)}enfugue-sidebar::-webkit-scrollbar-thumb{background-color:rgba(0,0,0,.55)}enfugue-sidebar::-webkit-scrollbar-thumb:hover{background-color:rgba(0,0,0,.7)}enfugue-sidebar input.invoke{margin:auto 1em 1em}enfugue-sidebar .invoke-loader{margin:-16px 2px 16px;pointer-events:none}enfugue-sidebar .invoke-loader.loading-bar:after{border-bottom-left-radius:4px;border-bottom-right-radius:4px;border-top-left-radius:0;border-top-right-radius:0}enfugue-toolbar{background-color:var(--dark-color);border-right:1px solid rgba(0,0,0,.2);border-top:1px solid hsla(0,0%,100%,.1);bottom:30px;flex-flow:column nowrap;justify-content:flex-start;left:0;padding:0;position:absolute;top:35px;z-index:3}enfugue-toolbar,enfugue-toolbar-item{align-items:center;border-bottom:1px solid rgba(0,0,0,.2);display:flex;width:40px}enfugue-toolbar-item{cursor:pointer;flex-flow:row nowrap;height:40px;justify-content:center;position:relative}enfugue-toolbar enfugue-toolbar-item:not(:first-child){border-top:1px solid hsla(0,0%,100%,.1)}enfugue-toolbar-item>span{display:none}enfugue-toolbar-item>i{font-size:25px}enfugue-toolbar-item:after{background-color:hsla(0,0%,100%,0);bottom:0;content:"\A";display:block;left:0;position:absolute;right:0;top:0}enfugue-toolbar-item:not(.disabled):not(:disabled):hover:after{background-color:hsla(0,0%,100%,.1)}enfugue-toolbar-item:not(.disabled):not(:disabled):active{border-bottom:1px solid rgba(0,0,0,.2)}enfugue-tabbed-view{display:block}enfugue-tabs{align-items:stretch;display:flex;flex-flow:row nowrap;justify-content:stretch}enfugue-tabs enfugue-tab{align-items:center;background-color:transparent;color:var(--theme-color-secondary);cursor:pointer;display:flex;flex-flow:row nowrap;flex-grow:0;font-family:var(--header-font);font-size:15px;font-weight:300;justify-content:center;padding:.75em;transition:background-color .25s ease-in-out,color .25s ease-in-out;transition:all .25s ease-in-out}enfugue-tabs enfugue-tab.active{background-color:var(--theme-color-secondary);color:var(--lightest-color);flex-grow:1;font-weight:700}enfugue-tab-content{border-top:3px solid var(--theme-color-secondary);display:block}enfugue-sidebar-category-header,enfugue-sidebar-item{align-items:center;border-bottom:1px solid rgba(0,0,0,.2);border-top:1px solid hsla(0,0%,100%,.15);color:var(--theme-color-secondary);cursor:pointer;display:flex;flex-direction:row;flex-wrap:nowrap;font-size:14px;font-weight:700;height:45px;padding:0 10px;position:relative;text-transform:uppercase}enfugue-sidebar-category-header:before,enfugue-sidebar-item:before{background-color:#000;bottom:0;content:"\A";display:block;left:0;opacity:0;pointer-events:none;position:absolute;right:0;top:0;transition:opacity .2s ease-in-out}enfugue-sidebar-category-header:hover:before,enfugue-sidebar-item:hover:before{opacity:.1}enfugue-sidebar-category-header:after{content:"\f054";flex-grow:1;font-family:Font Awesome\ 6 Free;font-weight:900;text-align:right}enfugue-sidebar-category.active>enfugue-sidebar-category-header:after{content:"\f078"}enfugue-sidebar-category-header enfugue-sidebar-category-button{cursor:pointer;font-size:16px;margin-left:10px;opacity:.75;transition:opacity .25s ease-in-out}enfugue-sidebar-category-header enfugue-sidebar-category-button:hover{opacity:1}enfugue-sidebar-item{background-color:var(--theme-color-primary);flex-direction:row-reverse}enfugue-menu-item.loading-bar:after,enfugue-sidebar-item.loading-bar:after{bottom:3px;height:5px;margin-left:-5px;margin-right:-5px}enfugue-sidebar-item.disabled{background-color:#aaa}enfugue-sidebar-item i{flex-grow:1;font-size:18px;text-align:right}enfugue-notification-center{bottom:0;display:flex;flex-flow:column-reverse nowrap;justify-content:flex-start;left:66%;pointer-events:none;position:fixed;right:0;top:0;z-index:6}enfugue-notification{backdrop-filter:blur(10px);background-color:rgba(0,0,0,.4);border:1px solid var(--darker-color);border-radius:2px;box-shadow:2px 2px 8px rgba(0,0,0,.3);color:var(--light-color);display:flex;flex-flow:column nowrap;height:150px;margin:1em;padding:1em;pointer-events:auto;position:relative;transition:all .5s ease-in-out}enfugue-notification i{cursor:pointer;font-size:18px;opacity:.75;position:absolute;right:1em;top:11px;transition:opacity .25s ease-in-out}enfugue-notification i:hover{opacity:1}enfugue-notification p{flex-basis:100%;font-size:13px;overflow-y:auto}enfugue-notification.hiding{height:0;margin:0 1em;opacity:0;padding:0 1em}enfugue-notification.hiding,enfugue-notification.hiding p{overflow:hidden}enfugue-notification h2{border-bottom:1px solid var(--lightest-color);color:var(--lightest-color);font-size:24px;font-weight:700;margin-bottom:.5em;text-transform:uppercase}enfugue-notification:not(:last-child){margin-top:0}enfugue-notification.info h2{border-color:rgba(92,184,92,.9);color:rgba(92,184,92,.75)}enfugue-notification.warn h2{border-color:rgba(240,173,78,.9);color:rgba(240,173,78,.75)}enfugue-notification.error h2{border-color:rgba(217,83,79,.9);color:rgba(217,83,79,.75)}enfugue-color-input,enfugue-repeatable-input,enfugue-search-list{align-items:center;background-color:var(--darker-color);border:1px solid #000;border-radius:5px;display:flex;flex-flow:row wrap;gap:5px;outline:none;padding:5px;position:relative;width:100%}enfugue-color-input{flex-flow:row nowrap}enfugue-search-list>enfugue-search-list-selection{align-items:center;background-color:var(--theme-color-primary);border-left:3px solid transparent;border-radius:2px;border-right:3px solid transparent;box-sizing:border-box;color:var(--lightest-color);display:flex;flex-flow:row nowrap;font-size:12px;justify-content:center;opacity:1;padding:5px 10px 5px 5px;position:relative;transition:border-color .1s ease-in-out,opacity .25s ease-in-out}enfugue-search-list>enfugue-search-list-selection span{font-weight:700}enfugue-search-list>enfugue-search-list-selection.dragged{opacity:.5}enfugue-search-list>enfugue-search-list-selection.drop-left{border-left:3px solid var(--dark-color)}enfugue-search-list>enfugue-search-list-selection.drop-right{border-right:3px solid var(--dark-color)}enfugue-search-list>enfugue-search-list-selection>button{background-color:var(--lightest-color);border-radius:20px;border-width:0;color:var(--theme-color-primary);height:15px;line-height:0;margin-right:5px;padding:0;width:15px}enfugue-search-list>enfugue-search-list-selection>button:not(:disabled):not(.disabled):hover{background-color:var(--theme-color-primary);color:var(--lightest-color)}enfugue-color-input>input,enfugue-search-list>input{border:none;flex-grow:1;margin:0;padding:5px}enfugue-color-input>.inline-color-preview{border:1px solid #000;border-radius:5px;cursor:pointer;height:20px;width:20px}enfugue-color-input-helper-view,ul.enfugue-search-list-items{background-color:var(--darker-color);border:1px solid var(--darkest-color);border-bottom-left-radius:5px;border-bottom-right-radius:5px;border-top:none;color:var(--light-color);max-height:400px;max-height:250px;min-height:40px;overflow-y:auto;position:fixed;z-index:10}enfugue-color-input-helper-view .preview-input-container{align-items:stretch;display:flex;flex-flow:row nowrap;gap:5px;justify-content:stretch;padding:5px}enfugue-color-input-helper-view .preview-input-container .preview{align-items:center;display:flex;flex-basis:25%;flex-flow:column nowrap;font-weight:700;gap:1em;justify-content:center;text-transform:uppercase}enfugue-color-input-helper-view .preview-input-container .input-container{align-items:center;display:flex;flex-basis:100%;flex-flow:column nowrap;gap:5px;justify-content:center}enfugue-color-input-helper-view .preview-input-container .input-container .input-part,enfugue-color-input-helper-view .preview-input-container .preview{border:1px solid #ccc;border-radius:5px}enfugue-color-input-helper-view .preview-input-container .input-container .input-part{cursor:pointer;height:30px;position:relative;width:100%}enfugue-color-input-helper-view .preview-input-container .input-container .input-part .indicator{border:1px solid #ccc;bottom:-5px;left:0;margin-left:-5px;pointer-events:none;position:absolute;top:-5px;width:10px}ul.enfugue-search-list-items>li{align-items:center;background-color:var(--darker-color);cursor:pointer;display:flex;flex-flow:row nowrap;font-size:12px;justify-content:flex-start;padding:.5em;position:relative;transition:all .25s ease-in-out}ul.enfugue-search-list-items>li:hover{background-color:var(--darkest-color)}ul.enfugue-search-list-items>li:not(:last-child){border-bottom:1px solid var(--darkest-color)}ul.enfugue-multi-search-list-items>li:before{border:1px solid #ccc;border-radius:2px;color:var(--theme-color-tertiary);content:"\A";display:block;font-weight:700;height:14px;margin-right:4px;padding:0;text-align:center;vertical-align:middle;width:14px}ul.enfugue-multi-search-list-items>li.selected:before{border-color:var(--theme-color-tertiary);content:"✓"}enfugue-repeatable-input input.add-item{flex-grow:0}enfugue-repeatable-input enfugue-repeatable-input-item{display:block;position:relative;width:100%}enfugue-repeatable-input enfugue-repeatable-input-item input.remove-item{border-radius:15px;height:15px;line-height:0;margin:0;padding:0;position:absolute;right:-2px;text-align:center;top:-2px;width:15px}enfugue-repeatable-input enfugue-repeatable-input-item input.remove-item.disabled{opacity:.33}enfugue-repeatable-input.columns{align-items:stretch;flex-flow:column nowrap}enfugue-repeatable-input.columns enfugue-repeatable-input-item{margin-bottom:5px}enfugue-repeatable-input enfugue-repeatable-input-item>form.inset-form{padding:10px}enfugue-repeatable-input enfugue-repeatable-input-item>form.inset-form fieldset:not(:last-child){margin-bottom:10px}enfugue-repeatable-input enfugue-repeatable-input-item>form.inset-form fieldset .field-container:not(:last-child){margin-bottom:5px}enfugue-repeatable-input enfugue-repeatable-input-item>form{gap:0;margin:0;padding:5px}enfugue-repeatable-input.columns input.add-item{width:calc(100% - 5px)}enfugue-repeatable-input.columns input.remove-item{background-color:#000;border-color:#000}enfugue-repeatable-input.columns input.remove-item:not(:disabled):not(.disabled):hover{color:#000}form.model-picker{align-items:center;display:flex;flex-flow:row nowrap;justify-content:center;left:40px;max-width:calc(100vw - 400px);padding:5px 0 0 5px;position:absolute;top:35px;width:500px;z-index:3}form.model-picker fieldset{width:100%}form.model-picker fieldset legend{display:none}form.model-picker div#tensorrt{cursor:pointer;height:22px;margin-left:-64px;position:relative;transition:all .25s ease-in-out}form.model-picker div#tensorrt img{filter:grayscale(100%);height:22px}form.model-picker div#tensorrt:hover img{filter:grayscale(75%)}form.model-picker div#tensorrt.ready img{filter:grayscale(0)}form.model-picker div#tensorrt span.fraction{border-radius:20px;color:#000;display:block;font-size:10px;height:20px;position:absolute;right:12.1px;text-align:center;top:0;width:20px}form.model-picker div#tensorrt span.fraction:after{background-color:#000;content:"\A";height:1px;left:5px;position:absolute;top:10px;transform:rotate(-62deg);width:10px}form.model-picker div#tensorrt span.fraction>span:first-child{display:block;left:3px;position:absolute;top:2px}form.model-picker div#tensorrt span.fraction>span:last-child{bottom:1px;display:block;position:absolute;right:3px}form.model-picker enfugue-search-list{margin:0}ul.model-picker-list-input-view>li>span{align-items:center;display:flex;flex-flow:row nowrap;height:100%;justify-content:space-between;width:100%}.additional-weights-form-view{left:35px;max-width:calc(100vw - 380px);opacity:.5;position:absolute;top:75px;transition:opacity .25s ease-in-out;width:520px;z-index:4}.additional-weights-form-view:hover{opacity:1}.additional-weights-form-view legend{flex-direction:row-reverse;justify-content:flex-end}.additional-weights-form-view legend:after{margin-right:10px}.page-buttons{align-items:center;display:flex;flex-flow:row nowrap;gap:5px;justify-content:stretch;margin:1em;width:calc(100% - 2em)}.page-buttons>*{flex-basis:100%;text-align:center}enfugue-status{align-items:center;color:var(--light-color);display:flex;flex-flow:row nowrap;font-size:10px;font-weight:900;gap:5px;height:100%;justify-content:space-between;padding:0 5px 0 50px;text-shadow:1px 1px 0 rgba(0,0,0,.8);transition:all .25s ease-in-out}enfugue-status-version:before{content:"VERSION: ";font-weight:200}enfugue-status-uptime:before{content:"UPTIME: ";font-weight:200}enfugue-status-gpu-name:before{content:"GPU: ";font-weight:200}enfugue-status-gpu-load:before{color:var(--light-color);content:"LOAD: ";font-weight:200}enfugue-status-gpu-load:after{content:"%";font-weight:200}enfugue-status-gpu-temp:before{color:var(--light-color);content:"TEMP: ";font-weight:200}enfugue-status-gpu-temp:after{content:"°C";font-weight:200}enfugue-status-gpu-memory:before{content:"MEM: ";font-weight:200}enfugue-status-icon{background-color:var(--dark-color);border:1px solid var(--darkest-color);border-radius:14px;display:inline-block;height:14px;width:14px}enfugue-status-gpu-memory{border:1px solid var(--dark-color);border-radius:4px;display:inline-block;padding:4px}enfugue-status-icon.idle{background-color:#999;cursor:not-allowed}enfugue-status-icon.ready{background-color:#4bb543;cursor:pointer}enfugue-status-icon.error{background-color:#f33;cursor:not-allowed}enfugue-status-icon.busy{background-color:#e9d502;cursor:pointer}enfugue-downloads{display:flex;flex-flow:column-reverse nowrap;gap:1em;padding:1em}enfugue-download{display:flex;flex-flow:column nowrap;gap:2px}enfugue-download-name{color:var(--theme-color-secondary);display:block;font-family:var(--header-font);font-size:1.5em}enfugue-download-progress{border-radius:2px;display:block;height:2px;width:100%}enfugue-download-size,enfugue-download-time{display:block;font-weight:300}enfugue-download-status{background-color:rgba(0,0,0,.6);border-radius:22px;color:hsla(0,0%,100%,.8);cursor:pointer;display:block;height:22px;line-height:22px;margin-left:auto;margin-right:-40px;position:relative;text-align:center;width:22px}enfugue-download-count{background-color:var(--dark-color);border-radius:12px;color:var(--light-color);font-size:10px;height:12px;line-height:12px;position:absolute;right:-2px;text-align:center;top:-2px;width:12px}enfugue-download-status.inactive{background:none!important;opacity:.5}enfugue-scribble-view{bottom:0;cursor:default;display:block;left:0;position:absolute;right:0;top:0;z-index:0}enfugue-scribble-view canvas{image-rendering:pixelated;position:relative;z-index:-1}enfugue-model-table-searching{display:block;margin:0;padding:1em 1em 0 0;text-align:right}enfugue-model-table-searching input{margin:0}enfugue-image-inspector{cursor:default;display:block;overflow:hidden;position:relative;text-align:center}enfugue-image-inspector .image-view-container{display:block;max-height:100%;overflow:hidden}enfugue-image-inspector .down,enfugue-image-inspector .left,enfugue-image-inspector .right,enfugue-image-inspector .up{align-items:center;display:flex;flex-flow:row nowrap;justify-content:center;opacity:0;pointer-events:none;position:absolute;transition:all .25s ease-in-out}enfugue-image-inspector .down.active,enfugue-image-inspector .left.active,enfugue-image-inspector .right.active,enfugue-image-inspector .up.active{font-size:40px;opacity:.5}enfugue-image-inspector .up{background-image:linear-gradient(0deg,transparent,#000);height:40px;left:0;right:0;top:0}enfugue-image-inspector .down{background-image:linear-gradient(180deg,transparent,#000);bottom:0;height:40px;left:0;position:absolute;right:0}enfugue-image-inspector .left{background-image:linear-gradient(270deg,transparent,#000);bottom:0;left:0;position:absolute;top:0;width:40px}enfugue-image-inspector .right{background-image:linear-gradient(90deg,transparent,#000);bottom:0;position:absolute;right:0;top:0;width:40px}enfugue-image-details{color:#000;font-family:var(--monospace-font),monospace;font-size:10px;position:absolute;right:5px;text-align:right;text-shadow:1px 1px 0 #fff;top:107px}enfugue-image-browser{box-shadow:0 0 10px rgba(0,0,0,.6);cursor:pointer;height:100px;opacity:.5;position:absolute;right:5px;top:5px;transition:all .25s ease-in-out}enfugue-image-browser:hover{opacity:1}enfugue-image-browser img{height:100%;pointer-events:none}enfugue-image-browser span{border:1px solid #fff;box-shadow:inset 0 0 1px #000;left:0;margin:0;max-height:100%;max-width:100%;padding:0;pointer-events:none;position:absolute;top:0}
```

### Comparing `enfugue-0.1.2/enfugue/static/css/09-enfugue-nodes.min.css` & `enfugue-0.1.3/enfugue/static/css/09-enfugue-nodes.min.css`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-enfugue-node-editor,enfugue-nodes{display:block;flex-grow:1;height:100%;overflow:hidden;position:relative;width:100%}enfugue-node-editor{display:block}enfugue-nodes{align-items:center;display:flex;flex-flow:row nowrap;justify-content:center}enfugue-nodes.oversize-x{justify-content:flex-start;overflow-x:auto}enfugue-node-canvas{left:0;position:absolute;top:0;transform-origin:top left}enfugue-node-editor enfugue-node-canvas{background:linear-gradient(to right,var(--dark-color) 0,transparent 1px) 0 0,linear-gradient(to right,var(--darker-color) 0,transparent 1px) 0 0,linear-gradient(to bottom,var(--dark-color) 0,transparent 1px) 0 0,linear-gradient(to bottom,var(--darker-color) 0,transparent 1px) 0 0;background-color:var(--darkest-color);background-position:-.5px -.5px;background-size:64px 64px,8px 8px,64px 64px,8px 8px}enfugue-node-editor enfugue-node-canvas>canvas{pointer-events:none}enfugue-nodes enfugue-node-canvas{position:relative}enfugue-nodes enfugue-node-canvas>canvas{display:none}enfugue-node-editor.windows>enfugue-node-canvas{background:none}enfugue-node-editor-position,enfugue-node-editor-zoom{bottom:5px;color:var(--light-color);font-weight:700;position:absolute;text-transform:uppercase;z-index:3}enfugue-node-editor-position{left:5px}enfugue-node-editor-position-reset,enfugue-node-editor-zoom-reset{background-color:hsla(0,0%,100%,.05);border:1px solid #000;border-radius:2px;cursor:pointer;font-size:12px;padding:2px 4px;transition:background-color .25s ease-in-out}enfugue-node-editor-position-reset:hover,enfugue-node-editor-zoom-reset:hover{background-color:hsla(0,0%,100%,.1)}enfugue-node-editor-position-reset{margin-left:5px}enfugue-node-editor-zoom-reset{margin-right:5px}enfugue-node-editor-zoom{right:5px}enfugue-node-editor-zoom-readout:after{content:"×"}enfugue-node-editor-zoom-in,enfugue-node-editor-zoom-out{cursor:pointer;margin-right:5px}enfugue-node{align-items:stretch;display:flex;flex-flow:row nowrap;justify-content:stretch;padding:10px;pointer-events:all;position:absolute;transition:transform .25s ease-out;z-index:1}enfugue-node.minimized{pointer-events:none;transition:all .25s ease-in}enfugue-node.focused{z-index:2}enfugue-node-container{align-items:stretch;background-color:var(--darkest-color);border:1px solid #000;border-radius:4px;display:block;flex-flow:column nowrap;justify-content:stretch;overflow:hidden;width:100%}enfugue-node.input-output>enfugue-node-container{background-color:#153131;color:var(--lightest-color)}enfugue-node-header,enfugue-windows-toolbar-item{align-items:center;background-color:var(--darker-color);color:var(--lightest-color);display:flex;flex-flow:row nowrap;flex-grow:0;font-size:14px;justify-content:stretch;overflow:hidden;padding:0 5px;transition:background-color .2s ease-in-out,height .2s ease-in-out;z-index:10}enfugue-node.flipped enfugue-node-header{bottom:0}enfugue-windows-toolbar-item{cursor:pointer;height:30px}enfugue-node-header:hover,enfugue-windows-toolbar-item:hover{background-color:var(--dark-color)}enfugue-node-name,enfugue-windows-toolbar-item-name{flex-grow:1;font-family:var(--monospace-font),monospace;margin-right:5px}enfugue-node-button,enfugue-windows-toolbar-item-button{cursor:pointer;flex-grow:0;margin:0 3px;transition:color .25s ease-in-out;z-index:10}enfugue-node-button:hover,enfugue-windows-toolbar-item-button:hover{color:var(--theme-color-primary)}enfugue-windows-toolbar{background-color:var(--dark-color);border-bottom:1px solid rgba(0,0,0,.2);border-top:1px solid hsla(0,0%,100%,.1);bottom:0;display:flex;flex-flow:row wrap;gap:1px;left:0;min-height:30px;pointer-events:all;position:absolute;right:0}enfugue-node-contents{display:block;flex-grow:1;overflow:auto;position:relative;width:100%}enfugue-node-contents h1,enfugue-node-contents h2,enfugue-node-contents h3{margin:1rem 0 0 1rem}enfugue-node-editor.image-editor enfugue-node.hide-header enfugue-node-header{background-color:rgba(0,0,0,.4);background-image:linear-gradient(180deg,rgba(0,0,0,.7),transparent);position:absolute;width:100%}enfugue-node-editor.image-editor enfugue-node.hide-header enfugue-node-header:hover{background-color:rgba(0,0,0,.6)}enfugue-node-editor.image-editor enfugue-node-container{background:transparent;border-radius:0;border-width:0;position:relative}enfugue-node-editor.image-editor enfugue-node:hover enfugue-node-container{background:hsla(0,0%,100%,.02)}enfugue-node-editor.image-editor enfugue-node-contents{overflow:hidden}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view{display:block;height:100%;position:relative;width:100%;z-index:-1}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view .background{background-position:0 0;background-repeat:no-repeat;background-size:auto}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.fit-actual .background{background-size:auto}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.fit-stretch .background{background-size:100% 100%}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.fit-contain .background{background-size:contain}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.fit-cover .background{background-size:cover}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-top-left .background{background-position:0 0}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-top-center .background{background-position:top}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-top-right .background{background-position:100% 0}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-center-left .background{background-position:0}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-center-center .background{background-position:50%}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-center-right .background{background-position:100%}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-bottom-left .background{background-position:0 100%}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-bottom-center .background{background-position:bottom}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-bottom-right .background{background-position:100% 100%}enfugue-node-editor.image-editor enfugue-node-header enfugue-node-button.top-right{transform:rotate(90deg)}enfugue-node-editor.image-editor enfugue-node-header enfugue-node-button.bottom-right{transform:rotate(180deg)}enfugue-node-editor.image-editor enfugue-node-header enfugue-node-button.bottom-left{transform:rotate(270deg)}enfugue-node-editor.image-editor enfugue-node-canvas .current-invocation-image-view{left:0;position:absolute;top:0}enfugue-node-editor.image-editor.zoom-out enfugue-node-canvas .current-invocation-image-view,enfugue-node-editor.image-editor.zoom-out enfugue-node-canvas enfugue-background-image-view{image-rendering:auto}enfugue-node-editor.image-editor.zoom-in enfugue-node-canvas .current-invocation-image-view,enfugue-node-editor.image-editor.zoom-in enfugue-node-canvas enfugue-background-image-view{image-rendering:pixelated}enfugue-node-editor.image-editor enfugue-node-canvas{background:none;border:1px solid var(--dark-color);box-sizing:content-box}enfugue-node-editor.image-editor enfugue-node-canvas enfugue-image-editor-grid{background-color:transparent;background:linear-gradient(90deg,hsla(0,0%,100%,.1) 0,hsla(0,0%,100%,.1) 1px,transparent 0) 0 0,linear-gradient(90deg,hsla(0,0%,100%,.02) 0,hsla(0,0%,100%,.02) 1px,transparent 0) 0 0,linear-gradient(180deg,hsla(0,0%,100%,.1) 0,hsla(0,0%,100%,.1) 1px,transparent 0) 0 0,linear-gradient(180deg,hsla(0,0%,100%,.02) 0,hsla(0,0%,100%,.02) 1px,transparent 0) 0 0;background-position:-.5px -.5px;background-size:64px 64px,8px 8px,64px 64px,8px 8px;height:100%;left:0;opacity:1;pointer-events:none;position:absolute;top:0;transition:.1s ease-in-out;width:100%;z-index:2}enfugue-node-editor.image-editor.has-image enfugue-node-canvas enfugue-image-editor-grid{opacity:0}enfugue-node-editor.image-editor.has-image enfugue-node-canvas:hover enfugue-image-editor-grid{opacity:1}enfugue-node-editor.image-editor.has-image enfugue-node-canvas enfugue-node{display:none}enfugue-node-editor.image-editor enfugue-invocation-loading{border:1px solid var(--dark-color);border-radius:10px;bottom:5px;display:block;height:20px;left:175px;line-height:18px;position:absolute;right:175px;transition:all .25s ease-in-out;z-index:1}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser{align-items:center;bottom:30px;display:flex;flex-flow:row nowrap;gap:5px;justify-content:center;left:175px;position:absolute;right:175px}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser enfugue-invocation-sample{align-items:center;border:1px solid var(--dark-color);border-radius:2px;cursor:pointer;display:flex;flex-flow:row nowrap;height:100px;justify-content:center;opacity:.7;transition:all .25s ease-in-out}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser enfugue-invocation-sample:hover{opacity:.9}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser enfugue-invocation-sample:active{opacity:1}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser enfugue-invocation-sample.no-sample{color:var(--dark-color);font-size:100px;width:100px}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser enfugue-invocation-sample img{max-height:100px}enfugue-node-editor.image-editor enfugue-invocation-stop{background-color:var(--theme-color-primary);border-radius:80px;color:#fff;cursor:not-allowed;display:block;filter:grayscale(100%);font-size:11px;height:40px;line-height:40px;opacity:0;pointer-events:none;position:absolute;right:5px;text-align:center;text-transform:uppercase;top:5px;transition:all .25s ease-in-out;width:40px}enfugue-node-editor.image-editor enfugue-invocation-stop.ready{cursor:pointer;filter:grayscale(50%);opacity:1;pointer-events:all}enfugue-node-editor.image-editor enfugue-invocation-stop.ready:hover{filter:grayscale(25%)}enfugue-node-editor.image-editor enfugue-invocation-stop.ready:active{filter:grayscale(0)}enfugue-node-editor.image-editor enfugue-invocation-loading{align-items:center;display:flex;flex-flow:row nowrap;justify-content:space-between;overflow:hidden}enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-loaded{display:block;height:100%;opacity:0;position:absolute;transition:all .1s linear;z-index:-1}enfugue-node-editor.image-editor enfugue-invocation-loading.loading enfugue-invocation-loaded{opacity:1}enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-duration,enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-iterations,enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-remaining{bottom:0;color:#fff;display:block;font-size:10px;text-shadow:1px 1px 1px #000;top:0}enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-duration{margin-left:5px}enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-iterations{margin-left:5px;margin-right:5px}enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-remaining{margin-right:5px}enfugue-node-editor.image-editor enfugue-node form{font-size:11px;height:0;opacity:0;overflow-y:auto;padding-bottom:1em;position:absolute;top:0;transition:all .25s ease-in-out;width:100%}enfugue-node-editor.image-editor enfugue-node.image-editor-prompt-node-view form{background-color:var(--dark-color)!important;height:100%!important;opacity:1!important;top:0!important}enfugue-node-editor.image-editor enfugue-node.image-editor-image-node-view enfugue-scribble-view{opacity:.5}enfugue-node-editor.image-editor enfugue-node.flipped form{bottom:0;top:auto}enfugue-node-editor.image-editor enfugue-node form input,enfugue-node-editor.image-editor enfugue-node form label,enfugue-node-editor.image-editor enfugue-node form select{color:#fff;font-size:11px}enfugue-node-editor.image-editor enfugue-node form legend{display:none}enfugue-node-editor.image-editor enfugue-node form .field-container{flex-basis:30%}enfugue-node-editor.image-editor enfugue-node form .field-container.checkbox-input-view,enfugue-node-editor.image-editor enfugue-node form .field-container.image-editor-image-anchor-input-view,enfugue-node-editor.image-editor enfugue-node form .field-container.image-editor-image-fit-input-view,enfugue-node-editor.image-editor enfugue-node form .field-container.text-input-view{flex-basis:40%}enfugue-node-editor.image-editor enfugue-node:hover form{background-color:rgba(0,0,0,.4);height:calc(100% - 30px);opacity:1;top:30px}enfugue-node-editor.image-editor enfugue-node.flipped:hover form{bottom:30px;top:auto}enfugue-node-editor.image-editor enfugue-node:hover form:hover{background-color:rgba(0,0,0,.6)}enfugue-node-editor.image-editor enfugue-node-canvas enfugue-toolbar{background-color:transparent;background-image:linear-gradient(90deg,transparent,rgba(0,0,0,.4));border:none;bottom:0;left:auto;right:0;top:0}enfugue-node-editor.image-editor enfugue-node-canvas enfugue-toolbar-item{background:none;border:none;opacity:.5;transition:all .25s ease-in-out}enfugue-node-editor.image-editor enfugue-node-canvas enfugue-toolbar-item:active,enfugue-node-editor.image-editor enfugue-node-canvas enfugue-toolbar-item:hover{border:none;opacity:1}enfugue-node-editor.image-editor enfugue-node-canvas enfugue-toolbar-item:after{display:none}.field-container.checkpoint-input-view,.field-container.multi-inversion-input-view,.field-container.multi-lora-input-view,.field-container.upscale-diffusion-guidance-scale-input-view,.field-container.upscale-diffusion-negative-prompt-input-view,.field-container.upscale-diffusion-prompt-input-view,.field-container.upscale-diffusion-steps-input-view,.field-container.upscale-methods-input-view,fieldset.field-set-directories .field-container,fieldset.field-set-prompts .field-container{flex-basis:100%}fieldset.field-set-prompts .field-container{margin-bottom:1em}.field-container.multi-lora-input-view legend{display:none}.field-container.multi-lora-input-view form .field-container{flex-basis:100%}enfugue-model-table{display:flex;flex-flow:column nowrap;justify-content:space-between}enfugue-model-table-paging{align-items:center;display:flex;flex-flow:row nowrap;justify-content:space-between;padding:5px 1em 0}enfugue-model-table-paging>span{color:var(--theme-color-tertiary);font-size:12px}enfugue-model-table-paging ul{display:flex;flex-flow:row nowrap;gap:5px}enfugue-model-table-paging ul li{align-items:center;background-color:var(--theme-color-tertiary);border-radius:3px;color:#fff;cursor:pointer;display:flex;flex-flow:row nowrap;height:25px;justify-content:center;line-height:25px;position:relative;text-align:center;transition:background-color .25s ease-in-out;width:25px}enfugue-model-table-paging ul li.selected{background-color:var(--theme-color-secondary)}enfugue-model-table-paging ul li span{font-family:var(--monospace-font),monospace}enfugue-model-table ul.include-first li:first-child{margin-right:30px}enfugue-model-table ul.include-first li:first-child:after{color:var(--theme-color-tertiary);content:"…";font-size:16px;left:calc(100% + 11px);position:absolute}enfugue-model-table ul.include-last li:last-child{margin-left:30px}enfugue-model-table ul.include-last li:last-child:after{color:var(--theme-color-tertiary);content:"…";font-size:16px;position:absolute;right:calc(100% + 11px)}enfugue-model-table-paging ul li:before{background-color:#fff;bottom:0;content:"\A";left:0;opacity:0;pointer-events:none;position:absolute;right:0;top:0;transition:opacity .25s ease-in-out}enfugue-model-table-paging ul li:hover:before{opacity:.1}enfugue-invocation-outputs{display:flex;flex-flow:row nowrap;gap:5px}enfugue-model-table.invocation-history tr td:first-child,enfugue-model-table.invocation-history tr td:nth-child(2),enfugue-model-table.invocation-history tr th:first-child,enfugue-model-table.invocation-history tr th:nth-child(2){width:15%}enfugue-model-table.invocation-history tr td:nth-child(3),enfugue-model-table.invocation-history tr th:nth-child(3){width:25%}enfugue-model-table.invocation-history tr td:nth-child(4),enfugue-model-table.invocation-history tr th:nth-child(4){width:35%}div.about-view>p,div.announcements-view>.view>p{line-height:1.1em;margin:1rem 0 0 1rem}div.announcements-view>.view>h3{color:var(--theme-color-tertiary);margin:1rem 0 0 1rem;text-align:left}div.about-view .donate-links{align-items:stretch;display:flex;flex-flow:row nowrap;gap:1em;justify-content:stretch;margin-top:1em;padding:.5em 1em}div.about-view .donate-links a{border-radius:5px;border-style:solid;border-width:2px;color:#fff;display:block;flex-basis:100%;font-weight:900;padding:1em;text-decoration:none;transition:all .25s ease-in-out}div.about-view .donate-links a:before{background-position:50%;background-repeat:no-repeat;background-size:contain;content:"\A";display:inline-block;height:25px;margin-right:10px;vertical-align:middle;width:25px}div.about-view .donate-links a.patreon{background-color:#ee614a;border-color:#ee614a}div.about-view .donate-links a.ko-fi{background-color:#29abe0;border-color:#29abe0}div.about-view .donate-links a.patreon:before{background-image:url(../img/brand/patreon.png)}div.about-view .donate-links a.ko-fi:before{background-image:url(../img/brand/ko-fi.png)}div.about-view .donate-links a:hover{background-color:transparent}div.about-view .donate-links a.patreon:hover{color:#ee614a}div.about-view .donate-links a.ko-fi:hover{color:#29abe0}div.history-view>input{float:right;margin:1em 1em 0 0}table.history-table-view tr td:first-child,table.history-table-view tr th:first-child,table.log-table-view tr td:first-child,table.log-table-view tr th:first-child{width:150px}table.log-table-view tr td:nth-child(2),table.log-table-view tr td:nth-child(3),table.log-table-view tr th:nth-child(2),table.log-table-view tr th:nth-child(3){width:80px}input.new-model-input-view,input.new-user-input-view,input.upload-file-input-view{float:right;margin-right:1em}input.upload-file-input-view{margin-top:1em}input.download-input-view{margin:1em;width:calc(100% - 2em)}enfugue-invocation-outputs enfugue-invocation-output{cursor:pointer}enfugue-invocation-outputs enfugue-invocation-output img{max-height:50px}
+enfugue-node-editor,enfugue-nodes{display:block;flex-grow:1;height:100%;overflow:hidden;position:relative;width:100%}enfugue-node-editor{display:block}enfugue-nodes{align-items:center;display:flex;flex-flow:row nowrap;justify-content:center}enfugue-nodes.oversize-x{justify-content:flex-start;overflow-x:auto}enfugue-node-canvas{left:0;position:absolute;top:0;transform-origin:top left}enfugue-node-editor enfugue-node-canvas{background:linear-gradient(to right,var(--dark-color) 0,transparent 1px) 0 0,linear-gradient(to right,var(--darker-color) 0,transparent 1px) 0 0,linear-gradient(to bottom,var(--dark-color) 0,transparent 1px) 0 0,linear-gradient(to bottom,var(--darker-color) 0,transparent 1px) 0 0;background-color:var(--darkest-color);background-position:-.5px -.5px;background-size:64px 64px,8px 8px,64px 64px,8px 8px}enfugue-node-editor enfugue-node-canvas>canvas{pointer-events:none}enfugue-nodes enfugue-node-canvas{position:relative}enfugue-nodes enfugue-node-canvas>canvas{display:none}enfugue-node-editor.windows>enfugue-node-canvas{background:none}enfugue-node-editor-position,enfugue-node-editor-zoom{bottom:5px;color:var(--light-color);font-weight:700;position:absolute;text-transform:uppercase;z-index:3}enfugue-node-editor-position{left:5px}enfugue-node-editor-position-reset,enfugue-node-editor-zoom-reset{background-color:hsla(0,0%,100%,.05);border:1px solid #000;border-radius:2px;cursor:pointer;font-size:12px;padding:2px 4px;transition:background-color .25s ease-in-out}enfugue-node-editor-position-reset:hover,enfugue-node-editor-zoom-reset:hover{background-color:hsla(0,0%,100%,.1)}enfugue-node-editor-position-reset{margin-left:5px}enfugue-node-editor-zoom-reset{margin-right:5px}enfugue-node-editor-zoom{right:5px}enfugue-node-editor-zoom-readout:after{content:"×"}enfugue-node-editor-zoom-in,enfugue-node-editor-zoom-out{cursor:pointer;margin-right:5px}enfugue-node{align-items:stretch;display:flex;flex-flow:row nowrap;justify-content:stretch;padding:10px;pointer-events:all;position:absolute;transition:transform .25s ease-out;z-index:1}enfugue-node.minimized{pointer-events:none;transition:all .25s ease-in}enfugue-node.focused{z-index:2}enfugue-node-container{align-items:stretch;background-color:var(--darkest-color);border:1px solid #000;border-radius:4px;display:block;flex-flow:column nowrap;justify-content:stretch;overflow:hidden;width:100%}enfugue-node.input-output>enfugue-node-container{background-color:#153131;color:var(--lightest-color)}enfugue-node-header,enfugue-windows-toolbar-item{align-items:center;background-color:var(--darker-color);color:var(--lightest-color);display:flex;flex-flow:row nowrap;flex-grow:0;font-size:14px;justify-content:stretch;overflow:hidden;padding:0 5px;transition:background-color .2s ease-in-out,height .2s ease-in-out;z-index:10}enfugue-node.flipped enfugue-node-header{bottom:0}enfugue-windows-toolbar-item{cursor:pointer;height:30px}enfugue-node-header:hover,enfugue-windows-toolbar-item:hover{background-color:var(--dark-color)}enfugue-node-name,enfugue-windows-toolbar-item-name{flex-grow:1;font-family:var(--monospace-font),monospace;margin-right:5px}enfugue-node-button,enfugue-windows-toolbar-item-button{cursor:pointer;flex-grow:0;margin:0 3px;transition:color .25s ease-in-out;z-index:10}enfugue-node-button:hover,enfugue-windows-toolbar-item-button:hover{color:var(--theme-color-primary)}enfugue-windows-toolbar{background-color:var(--dark-color);border-bottom:1px solid rgba(0,0,0,.2);border-top:1px solid hsla(0,0%,100%,.1);bottom:0;display:flex;flex-flow:row wrap;gap:1px;left:0;min-height:30px;pointer-events:all;position:absolute;right:0}enfugue-node-contents{display:block;flex-grow:1;overflow:auto;position:relative;width:100%}enfugue-node-contents h1,enfugue-node-contents h2,enfugue-node-contents h3{margin:1rem 0 0 1rem}enfugue-node-editor.image-editor enfugue-node.hide-header enfugue-node-header{background-color:rgba(0,0,0,.4);background-image:linear-gradient(180deg,rgba(0,0,0,.7),transparent);position:absolute;width:100%}enfugue-node-editor.image-editor enfugue-node.hide-header enfugue-node-header:hover{background-color:rgba(0,0,0,.6)}enfugue-node-editor.image-editor enfugue-node-container{background:transparent;border-radius:0;border-width:0;position:relative}enfugue-node-editor.image-editor enfugue-node:hover enfugue-node-container{background:hsla(0,0%,100%,.02)}enfugue-node-editor.image-editor enfugue-node-contents{overflow:hidden}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view{display:block;height:100%;position:relative;width:100%;z-index:-1}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view .background{background-position:0 0;background-repeat:no-repeat;background-size:auto}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.fit-actual .background{background-size:auto}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.fit-stretch .background{background-size:100% 100%}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.fit-contain .background{background-size:contain}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.fit-cover .background{background-size:cover}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-top-left .background{background-position:0 0}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-top-center .background{background-position:top}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-top-right .background{background-position:100% 0}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-center-left .background{background-position:0}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-center-center .background{background-position:50%}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-center-right .background{background-position:100%}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-bottom-left .background{background-position:0 100%}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-bottom-center .background{background-position:bottom}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-bottom-right .background{background-position:100% 100%}enfugue-node-editor.image-editor enfugue-node-header enfugue-node-button.top-right{transform:rotate(90deg)}enfugue-node-editor.image-editor enfugue-node-header enfugue-node-button.bottom-right{transform:rotate(180deg)}enfugue-node-editor.image-editor enfugue-node-header enfugue-node-button.bottom-left{transform:rotate(270deg)}enfugue-node-editor.image-editor enfugue-node-canvas .current-invocation-image-view{left:0;position:absolute;top:0}enfugue-node-editor.image-editor.zoom-out enfugue-node-canvas .current-invocation-image-view,enfugue-node-editor.image-editor.zoom-out enfugue-node-canvas enfugue-background-image-view{image-rendering:auto}enfugue-node-editor.image-editor.zoom-in enfugue-node-canvas .current-invocation-image-view,enfugue-node-editor.image-editor.zoom-in enfugue-node-canvas enfugue-background-image-view{image-rendering:pixelated}enfugue-node-editor.image-editor enfugue-node-canvas{background:none;border:1px solid var(--dark-color);box-sizing:content-box}enfugue-node-editor.image-editor enfugue-node-canvas enfugue-image-editor-grid{background-color:transparent;background:linear-gradient(90deg,hsla(0,0%,100%,.1) 0,hsla(0,0%,100%,.1) 1px,transparent 0) 0 0,linear-gradient(90deg,hsla(0,0%,100%,.02) 0,hsla(0,0%,100%,.02) 1px,transparent 0) 0 0,linear-gradient(180deg,hsla(0,0%,100%,.1) 0,hsla(0,0%,100%,.1) 1px,transparent 0) 0 0,linear-gradient(180deg,hsla(0,0%,100%,.02) 0,hsla(0,0%,100%,.02) 1px,transparent 0) 0 0;background-position:-.5px -.5px;background-size:64px 64px,8px 8px,64px 64px,8px 8px;height:100%;left:0;opacity:1;pointer-events:none;position:absolute;top:0;transition:.1s ease-in-out;width:100%;z-index:2}enfugue-node-editor.image-editor.has-image enfugue-node-canvas enfugue-image-editor-grid{opacity:0}enfugue-node-editor.image-editor.has-image enfugue-node-canvas:hover enfugue-image-editor-grid{opacity:1}enfugue-node-editor.image-editor.has-image enfugue-node-canvas enfugue-node{display:none}enfugue-node-editor.image-editor enfugue-invocation-loading{border:1px solid var(--dark-color);border-radius:10px;bottom:5px;display:block;height:20px;left:175px;line-height:18px;position:absolute;right:175px;transition:all .25s ease-in-out;z-index:1}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser{align-items:center;bottom:30px;display:flex;flex-flow:row nowrap;gap:5px;justify-content:center;left:175px;position:absolute;right:175px}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser enfugue-invocation-sample{align-items:center;border:1px solid var(--dark-color);border-radius:2px;cursor:pointer;display:flex;flex-flow:row nowrap;height:100px;justify-content:center;opacity:.7;transition:all .25s ease-in-out}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser enfugue-invocation-sample:hover{opacity:.9}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser enfugue-invocation-sample:active{opacity:1}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser enfugue-invocation-sample.no-sample{color:var(--dark-color);font-size:100px;width:100px}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser enfugue-invocation-sample img{max-height:100px}enfugue-node-editor.image-editor enfugue-invocation-stop{background-color:var(--theme-color-primary);border-radius:80px;color:#fff;cursor:not-allowed;display:block;filter:grayscale(100%);font-size:11px;height:40px;line-height:40px;opacity:0;pointer-events:none;position:absolute;right:5px;text-align:center;text-transform:uppercase;top:5px;transition:all .25s ease-in-out;width:40px}enfugue-node-editor.image-editor enfugue-invocation-stop.ready{cursor:pointer;filter:grayscale(50%);opacity:1;pointer-events:all}enfugue-node-editor.image-editor enfugue-invocation-stop.ready:hover{filter:grayscale(25%)}enfugue-node-editor.image-editor enfugue-invocation-stop.ready:active{filter:grayscale(0)}enfugue-node-editor.image-editor enfugue-invocation-loading{align-items:center;display:flex;flex-flow:row nowrap;justify-content:space-between;overflow:hidden}enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-loaded{display:block;height:100%;opacity:0;position:absolute;transition:all .1s linear;z-index:-1}enfugue-node-editor.image-editor enfugue-invocation-loading.loading enfugue-invocation-loaded{opacity:1}enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-duration,enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-iterations,enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-remaining{bottom:0;color:#fff;display:block;font-size:10px;text-shadow:1px 1px 1px #000;top:0}enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-duration{margin-left:5px}enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-iterations{margin-left:5px;margin-right:5px}enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-remaining{margin-right:5px}enfugue-node-editor.image-editor enfugue-node form{font-size:11px;height:0;opacity:0;overflow-y:auto;padding-bottom:1em;position:absolute;top:0;transition:all .25s ease-in-out;width:100%}enfugue-node-editor.image-editor enfugue-node.image-editor-prompt-node-view form{background-color:var(--dark-color)!important;height:100%!important;opacity:1!important;top:0!important}enfugue-node-editor.image-editor enfugue-node.image-editor-image-node-view enfugue-scribble-view{opacity:.5}enfugue-node-editor.image-editor enfugue-node.flipped form{bottom:0;top:auto}enfugue-node-editor.image-editor enfugue-node form input,enfugue-node-editor.image-editor enfugue-node form label,enfugue-node-editor.image-editor enfugue-node form select{color:#fff;font-size:11px}enfugue-node-editor.image-editor enfugue-node form legend{display:none}enfugue-node-editor.image-editor enfugue-node form .field-container{flex-basis:30%}enfugue-node-editor.image-editor enfugue-node form .field-container.checkbox-input-view,enfugue-node-editor.image-editor enfugue-node form .field-container.image-editor-image-anchor-input-view,enfugue-node-editor.image-editor enfugue-node form .field-container.image-editor-image-fit-input-view,enfugue-node-editor.image-editor enfugue-node form .field-container.text-input-view{flex-basis:40%}enfugue-node-editor.image-editor enfugue-node:hover form{background-color:rgba(0,0,0,.4);height:calc(100% - 30px);opacity:1;top:30px}enfugue-node-editor.image-editor enfugue-node.flipped:hover form{bottom:30px;top:auto}enfugue-node-editor.image-editor enfugue-node:hover form:hover{background-color:rgba(0,0,0,.6)}enfugue-node-editor.image-editor enfugue-node-canvas enfugue-toolbar{background-color:transparent;background-image:linear-gradient(90deg,transparent,rgba(0,0,0,.4));border:none;bottom:0;left:auto;right:0;top:0}enfugue-node-editor.image-editor enfugue-node-canvas enfugue-toolbar-item{background:none;border:none;opacity:.5;transition:all .25s ease-in-out}enfugue-node-editor.image-editor enfugue-node-canvas enfugue-toolbar-item:active,enfugue-node-editor.image-editor enfugue-node-canvas enfugue-toolbar-item:hover{border:none;opacity:1}enfugue-node-editor.image-editor enfugue-node-canvas enfugue-toolbar-item:after{display:none}.field-container.checkpoint-input-view,.field-container.multi-inversion-input-view,.field-container.multi-lora-input-view,.field-container.upscale-diffusion-guidance-scale-input-view,.field-container.upscale-diffusion-negative-prompt-input-view,.field-container.upscale-diffusion-prompt-input-view,.field-container.upscale-diffusion-steps-input-view,.field-container.upscale-methods-input-view,fieldset.field-set-directories .field-container,fieldset.field-set-prompts .field-container{flex-basis:100%}fieldset.field-set-prompts .field-container{margin-bottom:1em}.field-container.multi-lora-input-view legend{display:none}.field-container.multi-lora-input-view form .field-container{flex-basis:100%}enfugue-model-table{display:flex;flex-flow:column nowrap;justify-content:space-between}enfugue-model-table-paging{align-items:center;display:flex;flex-flow:row nowrap;justify-content:space-between;padding:5px 1em 0}enfugue-model-table-paging>span{color:var(--theme-color-tertiary);font-size:12px}enfugue-model-table-paging ul{display:flex;flex-flow:row nowrap;gap:5px}enfugue-model-table-paging ul li{align-items:center;background-color:var(--theme-color-tertiary);border-radius:3px;color:#fff;cursor:pointer;display:flex;flex-flow:row nowrap;height:25px;justify-content:center;line-height:25px;position:relative;text-align:center;transition:background-color .25s ease-in-out;width:25px}enfugue-model-table-paging ul li.selected{background-color:var(--theme-color-secondary)}enfugue-model-table-paging ul li span{font-family:var(--monospace-font),monospace}enfugue-model-table ul.include-first li:first-child{margin-right:30px}enfugue-model-table ul.include-first li:first-child:after{color:var(--theme-color-tertiary);content:"…";font-size:16px;left:calc(100% + 11px);position:absolute}enfugue-model-table ul.include-last li:last-child{margin-left:30px}enfugue-model-table ul.include-last li:last-child:after{color:var(--theme-color-tertiary);content:"…";font-size:16px;position:absolute;right:calc(100% + 11px)}enfugue-model-table-paging ul li:before{background-color:#fff;bottom:0;content:"\A";left:0;opacity:0;pointer-events:none;position:absolute;right:0;top:0;transition:opacity .25s ease-in-out}enfugue-model-table-paging ul li:hover:before{opacity:.1}enfugue-invocation-outputs{display:flex;flex-flow:row nowrap;gap:5px}enfugue-model-table.invocation-history tr td:first-child,enfugue-model-table.invocation-history tr td:nth-child(2),enfugue-model-table.invocation-history tr th:first-child,enfugue-model-table.invocation-history tr th:nth-child(2){width:15%}enfugue-model-table.invocation-history tr td:nth-child(3),enfugue-model-table.invocation-history tr th:nth-child(3){width:25%}enfugue-model-table.invocation-history tr td:nth-child(4),enfugue-model-table.invocation-history tr th:nth-child(4){width:35%}div.about-view>p,div.announcements-view>.view>p{line-height:1.1em;margin:1rem 0 0 1rem}div.announcements-view>.view>h3{color:var(--theme-color-tertiary);margin:1rem 0 0 1rem;text-align:left}div.about-view .donate-links{align-items:stretch;display:flex;flex-flow:row nowrap;gap:1em;justify-content:stretch;margin-top:1em;padding:.5em 1em}div.about-view .donate-links a{border-radius:5px;border-style:solid;border-width:2px;color:#fff;display:block;flex-basis:100%;font-weight:900;padding:1em;text-decoration:none;transition:all .25s ease-in-out}div.about-view .donate-links a:before{background-position:50%;background-repeat:no-repeat;background-size:contain;content:"\A";display:inline-block;height:25px;margin-right:10px;vertical-align:middle;width:25px}div.about-view .donate-links a.patreon{background-color:#ee614a;border-color:#ee614a}div.about-view .donate-links a.ko-fi{background-color:#29abe0;border-color:#29abe0}div.about-view .donate-links a.patreon:before{background-image:url(../img/brand/patreon.png)}div.about-view .donate-links a.ko-fi:before{background-image:url(../img/brand/ko-fi.png)}div.about-view .donate-links a:hover{background-color:transparent}div.about-view .donate-links a.patreon:hover{color:#ee614a}div.about-view .donate-links a.ko-fi:hover{color:#29abe0}div.history-view>input{float:right;margin:1em 1em 0 0}table.history-table-view tr td:first-child,table.history-table-view tr th:first-child,table.log-table-view tr td:first-child,table.log-table-view tr th:first-child{width:150px}table.log-table-view tr td:nth-child(2),table.log-table-view tr td:nth-child(3),table.log-table-view tr th:nth-child(2),table.log-table-view tr th:nth-child(3){width:80px}table.installation-directory-summary-table-view tr td:first-child,table.installation-directory-summary-table-view tr th:first-child{width:250px}input.new-model-input-view,input.new-user-input-view,input.upload-file-input-view{float:right;margin-right:1em}input.upload-file-input-view{margin-top:1em}input.download-input-view{margin:1em;width:calc(100% - 2em)}enfugue-invocation-outputs enfugue-invocation-output{cursor:pointer}enfugue-invocation-outputs enfugue-invocation-output img{max-height:50px}
```

### Comparing `enfugue-0.1.2/enfugue/static/css/vendor/fa/brands.min.css` & `enfugue-0.1.3/enfugue/static/css/vendor/fa/brands.min.css`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/css/vendor/fa/fontawesome.min.css` & `enfugue-0.1.3/enfugue/static/css/vendor/fa/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/css/vendor/fa/regular.min.css` & `enfugue-0.1.3/enfugue/static/css/vendor/fa/regular.min.css`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/css/vendor/fa/solid.min.css` & `enfugue-0.1.3/enfugue/static/css/vendor/fa/solid.min.css`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/fonts/vendor/fa/fa-brands-400.ttf` & `enfugue-0.1.3/enfugue/static/fonts/vendor/fa/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/fonts/vendor/fa/fa-brands-400.woff2` & `enfugue-0.1.3/enfugue/static/fonts/vendor/fa/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/fonts/vendor/fa/fa-regular-400.ttf` & `enfugue-0.1.3/enfugue/static/fonts/vendor/fa/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/fonts/vendor/fa/fa-regular-400.woff2` & `enfugue-0.1.3/enfugue/static/fonts/vendor/fa/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/fonts/vendor/fa/fa-solid-900.ttf` & `enfugue-0.1.3/enfugue/static/fonts/vendor/fa/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/fonts/vendor/fa/fa-solid-900.woff2` & `enfugue-0.1.3/enfugue/static/fonts/vendor/fa/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/html/body/content/content-login.html.j2` & `enfugue-0.1.3/enfugue/static/html/body/content/content-login.html.j2`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/html/body/footer/footer.html.j2` & `enfugue-0.1.3/enfugue/static/html/body/footer/footer.html.j2`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/html/head/head-base.html.j2` & `enfugue-0.1.3/enfugue/static/html/head/head-base.html.j2`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/img/brand/civit-ai-logo.svg` & `enfugue-0.1.3/enfugue/static/img/brand/civit-ai-logo.svg`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/img/brand/civit-ai.png` & `enfugue-0.1.3/enfugue/static/img/brand/civit-ai.png`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/img/brand/ko-fi.png` & `enfugue-0.1.3/enfugue/static/img/brand/ko-fi.png`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/img/brand/patreon.png` & `enfugue-0.1.3/enfugue/static/img/brand/patreon.png`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/img/brand/tensorrt.png` & `enfugue-0.1.3/enfugue/static/img/brand/tensorrt.png`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/img/cloud-320.png` & `enfugue-0.1.3/enfugue/static/img/cloud-320.png`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/img/favicon/favicon-128x128.png` & `enfugue-0.1.3/enfugue/static/img/favicon/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/img/favicon/favicon-16x16.png` & `enfugue-0.1.3/enfugue/static/img/favicon/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/img/favicon/favicon-256x256.png` & `enfugue-0.1.3/enfugue/static/img/favicon/favicon-256x256.png`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/img/favicon/favicon-32x32.png` & `enfugue-0.1.3/enfugue/static/img/favicon/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/img/favicon/favicon-512x512.png` & `enfugue-0.1.3/enfugue/static/img/favicon/favicon-512x512.png`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/img/favicon/favicon-64x64.png` & `enfugue-0.1.3/enfugue/static/img/favicon/favicon-64x64.png`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/img/favicon/favicon.ico` & `enfugue-0.1.3/enfugue/static/img/favicon/favicon.ico`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/application/index.mjs` & `enfugue-0.1.3/enfugue/static/js/application/index.mjs`

 * *Files 0% similar despite different names*

```diff
@@ -1 +1 @@
-import{isEmpty,getQueryParameters,getDataParameters,waitFor,createEvent}from"../base/helpers.mjs";import{Publisher}from"../base/publisher.mjs";import{TooltipHelper}from"../common/tooltip.mjs";import{MenuView,SidebarView,ToolbarView}from"../view/menu.mjs";import{StatusView}from"../view/status.mjs";import{NotificationCenterView}from"../view/notifications.mjs";import{WindowsView}from"../view/nodes/windows.mjs";import{ImageEditorView,ImageEditorNodeView,ImageEditorImageNodeView}from"../view/nodes/image-editor.mjs";import{ImageView}from"../view/image.mjs";import{Model}from"../model/enfugue.mjs";import{ConfirmFormView,YesNoFormView}from"../view/forms/confirm.mjs";import{View}from"../view/base.mjs";import{FormView}from"../view/forms/base.mjs";import{StringInputView}from"../view/forms/input.mjs";import{InvocationController}from"../controller/common/invocation.mjs";import{ModelPickerController}from"../controller/common/model-picker.mjs";import{ModelManagerController}from"../controller/common/model-manager.mjs";import{DownloadsController}from"../controller/common/downloads.mjs";import{AnnouncementsController}from"../controller/common/announcements.mjs";import{HistoryDatabase}from"../common/history.mjs";import{SimpleNotification}from"../common/notify.mjs";class FileNameFormView extends FormView{static fieldSets={"File Name":{filename:{class:StringInputView,config:{required:!0,placeholder:"Please enter a filename."}}}}}class LogoutButtonView extends View{static tagName="i";static className="fa-solid fa-right-from-bracket logout";async logout(){window.location="/logout"}async build(){let t=await super.build();return t.on("click",(()=>this.logout())),t.data("tooltip","Logout"),t}}class Application{static menuCategories={file:"File"};static adminMenuCategories={models:"Models",system:"System"};static filenameFormInputWidth=400;static filenameFormInputHeight=250;static logoShadowRGB=[0,0,0];static logoShadowOpacity=.5;static logoShadowSteps=10;static logoShadowOffset=2;static logoShadowSpread=0;static confirmViewWidth=500;static confirmViewHeight=200;constructor(t){this.config=t,this.publisher=new Publisher}async initialize(){this.tooltips=new TooltipHelper,this.container=document.querySelector(this.config.view.applicationContainer),isEmpty(this.container)?console.error(`Couldn't find application configuration using selector ${this.config.view.applicationContainer}, abandoning initialization.`):(this.model=new Model(this.config),console.log(this.model),this.menu=new MenuView(this.config),this.sidebar=new SidebarView(this.config),this.toolbar=new ToolbarView(this.config),this.windows=new WindowsView(this.config),this.notifications=new NotificationCenterView(this.config),this.history=new HistoryDatabase(this.config.history.size,this.config.debug),this.images=new ImageEditorView(this),this.container.appendChild(await this.menu.render()),this.container.appendChild(await this.sidebar.render()),this.container.appendChild(await this.toolbar.render()),this.container.appendChild(await this.images.render()),this.container.appendChild(await this.windows.render()),this.container.appendChild(await this.notifications.render()),await this.startAnimations(),await this.registerModelControllers(),await this.registerDownloadsControllers(),await this.registerInvocationControllers(),await this.registerMenuControllers(),await this.registerSidebarControllers(),await this.registerToolbarControllers(),await this.startAutosave(),await this.startKeepalive(),await this.startAnnouncements(),await this.registerLogout(),window.onpopstate=t=>this.popState(t),document.addEventListener("paste",(t=>this.onPaste(t))),document.addEventListener("keypress",(t=>this.onKeyPress(t))))}async startAnnouncements(){this.announcements=new AnnouncementsController(this),await this.announcements.initialize()}async startAnimations(){let t=document.querySelector("header h1");isEmpty(t)?console.warn("Can't find header logo, not binding animations."):window.addEventListener("mousemove",(e=>{let[i,o]=[e.clientX/window.innerWidth,e.clientY/window.innerHeight],s=[];for(let t=0;t<this.constructor.logoShadowSteps;t++){let[e,n]=[i*(t+1)*this.constructor.logoShadowOffset,o*(t+1)*this.constructor.logoShadowOffset],a=this.constructor.logoShadowOpacity-t/this.constructor.logoShadowSteps*this.constructor.logoShadowOpacity,r=`rgba(${this.constructor.logoShadowRGB.concat(a.toFixed(2)).join(",")})`;s.push(`${e}px ${n}px ${this.constructor.logoShadowSpread}px ${r}`)}t.style.textShadow=s.join(",")}))}async registerModelControllers(){this.modelManager=new ModelManagerController(this),await this.modelManager.initialize(),this.modelPicker=new ModelPickerController(this),await this.modelPicker.initialize()}async registerDownloadsControllers(){this.downloads=new DownloadsController(this),await this.downloads.initialize()}async registerInvocationControllers(){this.engine=new InvocationController(this),await this.engine.initialize()}getMenuCategories(){let t={...this.constructor.menuCategories};return isEmpty(window.enfugue)||!0!==window.enfugue.admin||(t={...t,...this.constructor.adminMenuCategories}),t.help="Help",t}async registerMenuControllers(){let t=this.getMenuCategories();this.menuControllers={};for(let e in t){let i=t[e];this.menuControllers[e]=[];try{let t=await import(`../controller/${e}/index.autogenerated.mjs`),o=await this.menu.addCategory(i);for(let i of t.Index)try{let t=(await import(`../controller/${e}/${i}`)).MenuController;if(isEmpty(t))throw"Module does not provide a 'MenuController' export.";if(!t.isDisabled()){let i=await o.addItem(t.menuName,t.menuIcon),s=new t(this);await s.initialize(),i.onClick((()=>s.onClick())),this.menuControllers[e].push(s)}}catch(t){console.warn("Couldn't import",e,"menu controller",i,t)}}catch(t){console.warn("Couldn't register controllers for menu",e,t)}}}async registerSidebarControllers(){let t=await import("../controller/sidebar/index.autogenerated.mjs");this.sidebarControllers=[];for(let e of t.Index){let t=(await import(`../controller/sidebar/${e}`)).SidebarController;if(isEmpty(t))throw"Module does not provide a 'SidebarController' export.";let i=new t(this);await i.initialize(),this.sidebarControllers.push(i)}}async registerToolbarControllers(){let t=await import("../controller/toolbar/index.autogenerated.mjs");this.toolbarControllers=[];for(let e of t.Index){let t=(await import(`../controller/toolbar/${e}`)).ToolbarController;if(isEmpty(t))throw"Module does not provide a 'ToolbarController' export.";let i=await this.toolbar.addItem(t.menuName,t.menuIcon),o=new t(this);await o.initialize(),i.onClick((()=>o.onClick())),this.toolbarControllers.push(o)}}async startKeepalive(){const t=this.config.model.status.interval||1e4,e=t=>{"ready"===t?this.publish("engineReady"):"busy"===t?this.publish("engineBusy"):"idle"===t?this.publish("engineIdle"):console.warn("Unknown status",t)};let i=document.querySelector("header");if(isEmpty(i))return void console.warn("No header found on page, not appending status view.");let o=await this.model.get(),s=new StatusView(this.config,o),n=await s.getNode();s.onStatusClicked((async()=>{await this.confirm("Stop engine and terminate any active invocations?")&&(await this.model.post("/invocation/stop"),this.notifications.push("info","Stopped","Engine successfully terminated."))})),e(o.status),i.appendChild(n.render()),setInterval((async()=>{try{let t=await this.model.get();o.status!==t.status&&e(t.status),s.updateStatus(t),o=t}catch{s.updateStatus("error")}}),t);let a=await this.model.get("/invocation"),r=null;for(let t of a)if("processing"===t.status){r=t;break}isEmpty(r)||(isEmpty(r)||isEmpty(r.metadata.tensorrt_build)?(this.notifications.push("info","Active Invocation Found","You have an image currently being generated, beginning monitoring process."),this.engine.canvasInvocation(r.uuid)):this.notifications.push("info","TensorRT Build in Progress",`You have a TensorRT engine build in progress for ${r.metadata.tensorrt_build.model}. You'll receive a notification in this window when it is complete. The engine will remain unavailable until that time.`)),setInterval((async()=>{try{let t,e=await this.model.get("/invocation");for(let i of e)"processing"===i.status&&(null!==r&&r.id===i.id||(t=i)),isEmpty(r)||i.id!==r.id||i.status===r.status||("completed"===i.status?this.publish("invocationComplete",i):this.publish("invocationError",i),r=null);isEmpty(t)||(this.publish("invocationBegin",t),r=t)}catch(t){console.error(t)}}),t)}async registerLogout(){if(!isEmpty(window.enfugue.user)&&"noauth"!==window.enfugue.user){let t=new LogoutButtonView(this.config);document.querySelector("header").appendChild((await t.getNode()).render())}}async startAutosave(){try{let t=await this.history.getCurrentState();isEmpty(t)||(this.setState(t),this.notifications.push("info","Session Restored","Your last autosaved session was successfully loaded."));const e=this.config.model.autosave.interval||3e4;setInterval((()=>this.autosave()),e)}catch(t){console.error(t),this.notifications.push("warning","History Disabled","Couldn't open IndexedDB, history and autosave are disabled.")}}async autosave(t=!0){try{await this.history.setCurrentState(this.getState()),t&&SimpleNotification.notify("Session autosaved!",2e3)}catch(t){console.error("Couldn't autosave",t)}}subscribe(t,e){this.publisher.subscribe(t,e)}unsubscribe(t,e){this.publisher.unsubscribe(t,e)}async publish(t,e=null){this.publisher.publish(t,e)}spawnConfirmForm(t,e,i,o=!0,s=!1){return new Promise((async(n,a)=>{let r,l=!1,h=new t(this.config,i);h.onSubmit((()=>{l=!0,n(!0),o&&r.remove()})),h.onCancel((()=>{l=!0,n(!1),r.remove()})),r=await this.windows.spawnWindow(e,h,this.constructor.confirmViewWidth,this.constructor.confirmViewHeight),r.onClose((()=>{!l&&s?a():n(!1),l=!0}))}))}confirm(t,e=!0){return this.spawnConfirmForm(ConfirmFormView,"Confirm",t,e)}yesNo(t,e=!0){return this.spawnConfirmForm(YesNoFormView,"Yes or No",t,e,!0)}async saveAs(t,e,i,o){let s=new Blob([e],i);return this.saveBlobAs(t,s,o)}async saveBlobAs(t,e,i){i.startsWith(".")||(i=`.${i}`);let o=window.URL.createObjectURL(e),s=new FileNameFormView(this.config),n=await this.windows.spawnWindow(t,s,this.constructor.filenameFormInputWidth,this.constructor.filenameFormInputHeight);s.onCancel((()=>n.close())),s.onSubmit((t=>{let e=t.filename;e.endsWith(i)&&(e=e.substring(0,e.length-i.length));let s=document.createElement("a");s.setAttribute("download",`${e}${i}`),s.href=o,document.body.appendChild(s),window.requestAnimationFrame((()=>{s.dispatchEvent(createEvent("click")),document.body.removeChild(s),n.remove()}))})),n.onClose((()=>window.URL.revokeObjectURL(o)))}async onPaste(t){let e=(t.clipboardData||t.originalEvent.clipboardData).items;for(let t of e)if("file"===t.kind){let e=t.getAsFile(),i=new FileReader;i.onload=t=>this.images.addImageNode(t.target.result,"Pasted Image"),i.readAsDataURL(e)}else t.getAsString((t=>this.onTextPaste(t)))}async onImagePaste(t){let e=new ImageView(this.config,t);await e.waitForLoad(),this.images.addNode(ImageEditorImageNodeView,"Pasted Image",e,0,0,e.width,e.height)}async onTextPaste(t){t.startsWith("<html>")||console.warn("Text paste",t)}getStatefulControllers(){let t=[this.modelPicker].concat(this.toolbarControllers).concat(this.sidebarControllers);for(let e in this.menuControllers)t=t.concat(this.menuControllers[e]);return t}getState(){let t={images:this.images.getState()},e=this.getStatefulControllers();for(let i of e)t={...t,...i.getState()};return t}shouldSaveState(){let t=this.getState();return!(isEmpty(t.prompts)||isEmpty(t.prompts.prompt)&&isEmpty(t.prompts.negativePrompt))||!isEmpty(t.images)}async setState(t,e=!1){!0===e&&this.shouldSaveState()&&(await this.autosave(!1),await this.history.flush(t));let i=this.getStatefulControllers();for(let e of i)await e.setState(t);isEmpty(t.canvas)||(isEmpty(t.canvas.width)||(this.images.width=t.canvas.width),isEmpty(t.canvas.height)||(this.images.height=t.canvas.height)),void 0!==t.images&&null!==t.images&&(this.engine.hideSampleChooser(),this.images.hideCurrentInvocation(),this.images.setState(t.images))}async resetState(t=!0){let e={images:[]},i=this.getStatefulControllers();for(let t of i)e={...e,...t.getDefaultState()};await this.setState(e,t)}async initializeStateFromImage(t,e=!0){try{let i={},o=await this.yesNo("Would you like to keep settings?<br /><br />This will maintain things like prompts and other global settings the same while only changing the dimensions to match the image."),s=this.getStatefulControllers();for(let t of s)i=o?{...i,...t.getState()}:{...i,...t.getDefaultState()};isEmpty(i.canvas)&&(i.canvas={}),i.canvas.width=t.width,i.canvas.height=t.height,i.images=[ImageEditorView.getNodeDataForImage(t)],this.engine.hideSampleChooser(),this.images.hideCurrentInvocation(),this.images.width=t.width,this.images.height=t.height,await this.setState(i,e)}catch(t){}}onKeyPress(t){}async popState(t){}}export{Application};
+import{isEmpty,getQueryParameters,getDataParameters,waitFor,createEvent}from"../base/helpers.mjs";import{Publisher}from"../base/publisher.mjs";import{TooltipHelper}from"../common/tooltip.mjs";import{MenuView,SidebarView,ToolbarView}from"../view/menu.mjs";import{StatusView}from"../view/status.mjs";import{NotificationCenterView}from"../view/notifications.mjs";import{WindowsView}from"../view/nodes/windows.mjs";import{ImageEditorView,ImageEditorNodeView,ImageEditorImageNodeView}from"../view/nodes/image-editor.mjs";import{ImageView}from"../view/image.mjs";import{Model}from"../model/enfugue.mjs";import{ConfirmFormView,YesNoFormView}from"../view/forms/confirm.mjs";import{View}from"../view/base.mjs";import{FormView}from"../view/forms/base.mjs";import{StringInputView}from"../view/forms/input.mjs";import{InvocationController}from"../controller/common/invocation.mjs";import{ModelPickerController}from"../controller/common/model-picker.mjs";import{ModelManagerController}from"../controller/common/model-manager.mjs";import{DownloadsController}from"../controller/common/downloads.mjs";import{AnnouncementsController}from"../controller/common/announcements.mjs";import{HistoryDatabase}from"../common/history.mjs";import{SimpleNotification}from"../common/notify.mjs";class FileNameFormView extends FormView{static fieldSets={"File Name":{filename:{class:StringInputView,config:{required:!0,placeholder:"Please enter a filename."}}}}}class LogoutButtonView extends View{static tagName="i";static className="fa-solid fa-right-from-bracket logout";async logout(){window.location="/logout"}async build(){let t=await super.build();return t.on("click",(()=>this.logout())),t.data("tooltip","Logout"),t}}class Application{static menuCategories={file:"File"};static adminMenuCategories={models:"Models",system:"System"};static filenameFormInputWidth=400;static filenameFormInputHeight=250;static logoShadowRGB=[0,0,0];static logoShadowOpacity=.5;static logoShadowSteps=10;static logoShadowOffset=2;static logoShadowSpread=0;static confirmViewWidth=500;static confirmViewHeight=200;constructor(t){this.config=t,this.publisher=new Publisher}async initialize(){this.tooltips=new TooltipHelper,this.container=document.querySelector(this.config.view.applicationContainer),isEmpty(this.container)?console.error(`Couldn't find application configuration using selector ${this.config.view.applicationContainer}, abandoning initialization.`):(this.model=new Model(this.config),this.menu=new MenuView(this.config),this.sidebar=new SidebarView(this.config),this.toolbar=new ToolbarView(this.config),this.windows=new WindowsView(this.config),this.notifications=new NotificationCenterView(this.config),this.history=new HistoryDatabase(this.config.history.size,this.config.debug),this.images=new ImageEditorView(this),this.container.appendChild(await this.menu.render()),this.container.appendChild(await this.sidebar.render()),this.container.appendChild(await this.toolbar.render()),this.container.appendChild(await this.images.render()),this.container.appendChild(await this.windows.render()),this.container.appendChild(await this.notifications.render()),await this.startAnimations(),await this.registerModelControllers(),await this.registerDownloadsControllers(),await this.registerInvocationControllers(),await this.registerMenuControllers(),await this.registerSidebarControllers(),await this.registerToolbarControllers(),await this.startAutosave(),await this.startKeepalive(),await this.startAnnouncements(),await this.registerLogout(),window.onpopstate=t=>this.popState(t),document.addEventListener("paste",(t=>this.onPaste(t))),document.addEventListener("keypress",(t=>this.onKeyPress(t))))}async startAnnouncements(){this.announcements=new AnnouncementsController(this),await this.announcements.initialize()}async startAnimations(){let t=document.querySelector("header h1");isEmpty(t)?console.warn("Can't find header logo, not binding animations."):window.addEventListener("mousemove",(e=>{let[i,o]=[e.clientX/window.innerWidth,e.clientY/window.innerHeight],s=[];for(let t=0;t<this.constructor.logoShadowSteps;t++){let[e,n]=[i*(t+1)*this.constructor.logoShadowOffset,o*(t+1)*this.constructor.logoShadowOffset],a=this.constructor.logoShadowOpacity-t/this.constructor.logoShadowSteps*this.constructor.logoShadowOpacity,r=`rgba(${this.constructor.logoShadowRGB.concat(a.toFixed(2)).join(",")})`;s.push(`${e}px ${n}px ${this.constructor.logoShadowSpread}px ${r}`)}t.style.textShadow=s.join(",")}))}async registerModelControllers(){this.modelManager=new ModelManagerController(this),await this.modelManager.initialize(),this.modelPicker=new ModelPickerController(this),await this.modelPicker.initialize()}async registerDownloadsControllers(){this.downloads=new DownloadsController(this),await this.downloads.initialize()}async registerInvocationControllers(){this.engine=new InvocationController(this),await this.engine.initialize()}getMenuCategories(){let t={...this.constructor.menuCategories};return isEmpty(window.enfugue)||!0!==window.enfugue.admin||(t={...t,...this.constructor.adminMenuCategories}),t.help="Help",t}async registerMenuControllers(){let t=this.getMenuCategories();this.menuControllers={};for(let e in t){let i=t[e];this.menuControllers[e]=[];try{let t=await import(`../controller/${e}/index.autogenerated.mjs`),o=await this.menu.addCategory(i);for(let i of t.Index)try{let t=(await import(`../controller/${e}/${i}`)).MenuController;if(isEmpty(t))throw"Module does not provide a 'MenuController' export.";if(!t.isDisabled()){let i=await o.addItem(t.menuName,t.menuIcon),s=new t(this);await s.initialize(),i.onClick((()=>s.onClick())),this.menuControllers[e].push(s)}}catch(t){console.warn("Couldn't import",e,"menu controller",i,t)}}catch(t){console.warn("Couldn't register controllers for menu",e,t)}}}async registerSidebarControllers(){let t=await import("../controller/sidebar/index.autogenerated.mjs");this.sidebarControllers=[];for(let e of t.Index){let t=(await import(`../controller/sidebar/${e}`)).SidebarController;if(isEmpty(t))throw"Module does not provide a 'SidebarController' export.";let i=new t(this);await i.initialize(),this.sidebarControllers.push(i)}}async registerToolbarControllers(){let t=await import("../controller/toolbar/index.autogenerated.mjs");this.toolbarControllers=[];for(let e of t.Index){let t=(await import(`../controller/toolbar/${e}`)).ToolbarController;if(isEmpty(t))throw"Module does not provide a 'ToolbarController' export.";let i=await this.toolbar.addItem(t.menuName,t.menuIcon),o=new t(this);await o.initialize(),i.onClick((()=>o.onClick())),this.toolbarControllers.push(o)}}async startKeepalive(){const t=this.config.model.status.interval||1e4,e=t=>{"ready"===t?this.publish("engineReady"):"busy"===t?this.publish("engineBusy"):"idle"===t?this.publish("engineIdle"):console.warn("Unknown status",t)};let i=document.querySelector("header");if(isEmpty(i))return void console.warn("No header found on page, not appending status view.");let o=await this.model.get(),s=new StatusView(this.config,o),n=await s.getNode();s.onStatusClicked((async()=>{await this.confirm("Stop engine and terminate any active invocations?")&&(await this.model.post("/invocation/stop"),this.notifications.push("info","Stopped","Engine successfully terminated."))})),e(o.status),i.appendChild(n.render()),setInterval((async()=>{try{let t=await this.model.get();o.status!==t.status&&e(t.status),s.updateStatus(t),o=t}catch{s.updateStatus("error")}}),t);let a=await this.model.get("/invocation"),r=null;for(let t of a)if("processing"===t.status){r=t;break}isEmpty(r)||(isEmpty(r)||isEmpty(r.metadata)||isEmpty(r.metadata.tensorrt_build)?(this.notifications.push("info","Active Invocation Found","You have an image currently being generated, beginning monitoring process."),this.engine.canvasInvocation(r.uuid)):this.notifications.push("info","TensorRT Build in Progress",`You have a TensorRT engine build in progress for ${r.metadata.tensorrt_build.model}. You'll receive a notification in this window when it is complete. The engine will remain unavailable until that time.`)),setInterval((async()=>{try{let t,e=await this.model.get("/invocation");for(let i of e)"processing"===i.status&&(null!==r&&r.id===i.id||(t=i)),isEmpty(r)||i.id!==r.id||i.status===r.status||("completed"===i.status?this.publish("invocationComplete",i):this.publish("invocationError",i),r=null);isEmpty(t)||(this.publish("invocationBegin",t),r=t)}catch(t){console.error(t)}}),t)}async registerLogout(){if(!isEmpty(window.enfugue.user)&&"noauth"!==window.enfugue.user){let t=new LogoutButtonView(this.config);document.querySelector("header").appendChild((await t.getNode()).render())}}async startAutosave(){try{let t=await this.history.getCurrentState();isEmpty(t)||(this.setState(t),this.notifications.push("info","Session Restored","Your last autosaved session was successfully loaded."));const e=this.config.model.autosave.interval||3e4;setInterval((()=>this.autosave()),e)}catch(t){console.error(t),this.notifications.push("warning","History Disabled","Couldn't open IndexedDB, history and autosave are disabled.")}}async autosave(t=!0){try{await this.history.setCurrentState(this.getState()),t&&SimpleNotification.notify("Session autosaved!",2e3)}catch(t){console.error("Couldn't autosave",t)}}subscribe(t,e){this.publisher.subscribe(t,e)}unsubscribe(t,e){this.publisher.unsubscribe(t,e)}async publish(t,e=null){this.publisher.publish(t,e)}spawnConfirmForm(t,e,i,o=!0,s=!1){return new Promise((async(n,a)=>{let r,l=!1,h=new t(this.config,i);h.onSubmit((()=>{l=!0,n(!0),o&&r.remove()})),h.onCancel((()=>{l=!0,n(!1),r.remove()})),r=await this.windows.spawnWindow(e,h,this.constructor.confirmViewWidth,this.constructor.confirmViewHeight),r.onClose((()=>{!l&&s?a():n(!1),l=!0}))}))}confirm(t,e=!0){return this.spawnConfirmForm(ConfirmFormView,"Confirm",t,e)}yesNo(t,e=!0){return this.spawnConfirmForm(YesNoFormView,"Yes or No",t,e,!0)}async saveAs(t,e,i,o){let s=new Blob([e],{type:i});return this.saveBlobAs(t,s,o)}async saveBlobAs(t,e,i){i.startsWith(".")||(i=`.${i}`);let o=window.URL.createObjectURL(e),s=new FileNameFormView(this.config),n=await this.windows.spawnWindow(t,s,this.constructor.filenameFormInputWidth,this.constructor.filenameFormInputHeight);s.onCancel((()=>n.close())),s.onSubmit((t=>{let e=t.filename;e.endsWith(i)&&(e=e.substring(0,e.length-i.length));let s=document.createElement("a");s.setAttribute("download",`${e}${i}`),s.href=o,document.body.appendChild(s),window.requestAnimationFrame((()=>{s.dispatchEvent(createEvent("click")),document.body.removeChild(s),n.remove()}))})),n.onClose((()=>window.URL.revokeObjectURL(o)))}async onPaste(t){let e=(t.clipboardData||t.originalEvent.clipboardData).items;for(let t of e)if("file"===t.kind){let e=t.getAsFile(),i=new FileReader;i.onload=t=>this.images.addImageNode(t.target.result,"Pasted Image"),i.readAsDataURL(e)}else t.getAsString((t=>this.onTextPaste(t)))}async onImagePaste(t){let e=new ImageView(this.config,t);await e.waitForLoad(),this.images.addNode(ImageEditorImageNodeView,"Pasted Image",e,0,0,e.width,e.height)}async onTextPaste(t){t.startsWith("<html>")||console.warn("Text paste",t)}getStatefulControllers(){let t=[this.modelPicker].concat(this.toolbarControllers).concat(this.sidebarControllers);for(let e in this.menuControllers)t=t.concat(this.menuControllers[e]);return t}getState(){let t={images:this.images.getState()},e=this.getStatefulControllers();for(let i of e)t={...t,...i.getState()};return t}shouldSaveState(){let t=this.getState();return!(isEmpty(t.prompts)||isEmpty(t.prompts.prompt)&&isEmpty(t.prompts.negativePrompt))||!isEmpty(t.images)}async setState(t,e=!1){!0===e&&this.shouldSaveState()&&(await this.autosave(!1),await this.history.flush(t));let i=this.getStatefulControllers();for(let e of i)await e.setState(t);isEmpty(t.canvas)||(isEmpty(t.canvas.width)||(this.images.width=t.canvas.width),isEmpty(t.canvas.height)||(this.images.height=t.canvas.height)),void 0!==t.images&&null!==t.images&&(this.engine.hideSampleChooser(),this.images.hideCurrentInvocation(),this.images.setState(t.images))}async resetState(t=!0){let e={images:[]},i=this.getStatefulControllers();for(let t of i)e={...e,...t.getDefaultState()};await this.setState(e,t)}async initializeStateFromImage(t,e=!0){try{let i={},o=await this.yesNo("Would you like to keep settings?<br /><br />This will maintain things like prompts and other global settings the same while only changing the dimensions to match the image."),s=this.getStatefulControllers();for(let t of s)i=o?{...i,...t.getState()}:{...i,...t.getDefaultState()};isEmpty(i.canvas)&&(i.canvas={}),i.canvas.width=t.width,i.canvas.height=t.height,i.images=[ImageEditorView.getNodeDataForImage(t)],this.engine.hideSampleChooser(),this.images.hideCurrentInvocation(),this.images.width=t.width,this.images.height=t.height,await this.setState(i,e)}catch(t){}}onKeyPress(t){}async popState(t){}}export{Application};
```

### Comparing `enfugue-0.1.2/enfugue/static/js/base/api.mjs` & `enfugue-0.1.3/enfugue/static/js/base/api.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/base/builder.mjs` & `enfugue-0.1.3/enfugue/static/js/base/builder.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/base/csv.mjs` & `enfugue-0.1.3/enfugue/static/js/base/csv.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/base/helpers.mjs` & `enfugue-0.1.3/enfugue/static/js/base/helpers.mjs`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-export let every=e=>{for(let t of e)if(!t)return!1;return!0};export let none=e=>{for(let t of e)if(t)return!1;return!0};export let any=e=>{for(let t of e)if(t)return!0;return!1};export let flatten=e=>e.reduce(((e,t)=>e.concat(Array.isArray(t)?flatten(t):t)),[]);export let strip=e=>{if(isEmpty(e))return e;let t=e.match(/^[\ \t\r\n\'\"]*(.*?)[\ \t\r\n\'\"]*$/);return null===t?"":t[1]};export let sleep=e=>new Promise((t=>{setTimeout(t,e)}));export let waitFor=async(e,t)=>{let r=(t=t||{}).interval||50,o=t.timeout,n=new Date,l=0;for(;!e();)if(await sleep(r),l=new Date-n,!isEmpty(o)&&l>o)throw"Timeout"};export let guessCase=e=>(e=strip(e),/^$/.test(e)?"EMPTY":/^[a-z09]+$/.test(e)?"LOWER":/^[A-Z09]+$/.test(e)?"UPPER":/^[A-Za-z0-9]+(_[A-Za-z0-9]+)+$/.test(e)?"SNAKE":/^[A-Za-z0-9]+(-[A-Za-z0-9]+)+$/.test(e)?"KEBAB":/^[a-z]+([A-Z][a-z0-9]+)+$/.test(e)?"CAMEL":/^([A-Z][a-z0-9]+)+$/.test(e)?"PASCAL":/^(\w+)((\W\w+)+)$/.test(e)?"SENTENCE":"UNKNOWN");export let guessStringParts=e=>{switch(e=strip(e),guessCase(e)){case"SENTENCE":return e.split(" ").map((e=>e.toLowerCase()));case"SNAKE":return e.split("_").map((e=>e.toLowerCase()));case"KEBAB":return e.split("-").map((e=>e.toLowerCase()));case"CAMEL":return e.split(/([A-Z])/g).reduce(((e,t,r)=>0==r||r%2==1?e.concat([t]):e.concat([e.splice(-1)[0]+t])),[]).map((e=>e.toLowerCase()));case"PASCAL":return e.split(/([A-Z])/g).reduce(((e,t,r)=>0==r?e:r%2==1?e.concat([t]):e.concat([e.splice(-1)[0]+t])),[]).map((e=>e.toLowerCase()));default:return[e.toLowerCase()]}};export let kebabCase=(e,t)=>(void 0===t&&(t="-"),guessStringParts(e).join(t));export let snakeCase=(e,t)=>(void 0===t&&(t="_"),guessStringParts(e).join(t));export let camelCase=(e,t)=>(void 0===t&&(t=""),guessStringParts(e).map(((e,t)=>0==t?e:e[0].toUpperCase()+e.substr(1))).join(t));export let pascalCase=(e,t)=>(void 0===t&&(t=""),guessStringParts(e).map((e=>e[0].toUpperCase()+e.substr(1))).join(t));export let titleCase=e=>pascalCase(e," ");export let caseInsensitiveMatch=(e,t)=>e.toLowerCase()===t.toLowerCase()||kebabCase(e)===kebabCase(t);export let truncate=(e,t,r="…")=>e.length<=t?e:e.substring(0,e.lastIndexOf(" ",t))+r;export let set=e=>e.filter(((t,r)=>e.indexOf(t)===r));export let merge=function(){let e=Array.from(arguments),t={...e[0]};for(let r=1;r<e.length;r++){let o=e[r];for(let e in o)void 0===t[e]?t[e]=o[e]:"object"==typeof t[e]&&"object"==typeof o[e]?t[e]=merge(t[e],o[e]):t[e]=o[e]}return t};const mouseEvents=["click","dblclick","mouseenter","mouseleave","mouseup","mousedown","mousemove","mouseover","mouseout","contextmenu"];export let createEvent=e=>"function"==typeof MouseEvent&&mouseEvents.indexOf(e)>-1?new MouseEvent(e):"function"==typeof Event?new Event(e):(()=>{let t=document.createEvent("Event");return t.initEvent(e,!0,!0),t})();export let randomInt=(e,t)=>(void 0===t?0:e)+Math.random()*(void 0===t?e:t-e)|0;export let randomHex=e=>isEmpty(e)?randomInt(16).toString(16):new Array(e).fill(null).map(randomHex).join("");export let randomChoice=e=>e[randomInt(e.length)];export let uuid=()=>`${randomHex(8)}-${randomHex(4)}-4${randomHex(3)}-${randomChoice(["8","9","a","b"])}${randomHex(3)}-${randomHex(12)}`;export let isEquivalent=(e,t)=>{if(typeof e==typeof t){if(Array.isArray(e)&&Array.isArray(t)){if(e.length!==t.length)return!1;for(let r=0;r<e.length;r++)if(!isEquivalent(e[r],t[r]))return!1;return!0}if("object"==typeof e){if(null===e)return null===t;if(null===t)return!1;let r=Object.getOwnPropertyNames(e),o=Object.getOwnPropertyNames(t);if(!isEquivalent(r,o))return!1;for(let o of r)if(!isEquivalent(e[o],t[o]))return!1;return!0}return e===t}return!1};export let getQueryParameters=()=>-1===window.location.href.indexOf("?")?{}:window.location.href.substring(window.location.href.indexOf("?")+1).split("&").reduce(((e,t)=>{let r=t.split("="),o=r[0],n=decodeURIComponent(r[1]).replace("+"," ");return e.hasOwnProperty(o)?(Array.isArray(e[o])||(e[o]=[e[o]]),e[o].push(n)):e[o]=n,e}),{});export let getDataParameters=e=>{let t={};for(let r=0,o=e.attributes,n=o.length;r<n;r++)o[r].nodeName.startsWith("data")&&(t[camelCase(o[r].nodeName.substr(5))]=o[r].nodeValue);return t};export let buildQueryURL=(e,t)=>{let r=e;return-1===e.indexOf("?")&&(r+="?"),r+Object.getOwnPropertyNames(t).map((e=>`${e}=${encodeURIComponent(t[e])}`)).join("&")};export let getQueryURL=e=>buildQueryURL(window.location.href,e);export let isEmpty=e=>null==e||""===e||"null"===e||Array.isArray(e)&&0===e.length||"object"==typeof e&&"Object"===e.constructor.name&&0===Object.getOwnPropertyNames(e).length;export let removeEmpty=e=>{if(Array.isArray(e)){let t=[];for(let r of e)isEmpty(v)||t.push(v);return t}if("object"==typeof e){let t={};for(let r of Object.getOwnPropertyNames(e))isEmpty(e[r])||(t[r]=e[r]);return t}return e};export let deepClone=(e,t=!0)=>{if(null==e)return e;if("function"==typeof e){if(t)throw"Cannot clone functions.";return e}return"boolean"==typeof e?!!e:"number"==typeof e?0+e:"string"==typeof e||e instanceof String?`${e}`:Array.isArray(e)?new Array(e.length).fill(null).map(((t,r)=>deepClone(e[r],!1))):"object"==typeof e||e===Object(e)?"RegExp"===e.constructor.name?e:Object.getOwnPropertyNames(e).reduce(((t,r)=>(t[r]=deepClone(e[r],!1),t)),new Object):(console.warn("Unknown clone type for",e),e)};const byteSuffixes=["B","KB","MB","GB","TB","PB","EB","ZB","YB"];export let humanSize=(e,t)=>{void 0===t&&(t=2);let r=0;for(;e>1e3;)e/=1e3,r++;return`${e.toFixed(t)} ${byteSuffixes[r]}`};const secondsPerMinute=60,secondsPerHour=3600,secondsPerDay=86400;export let humanDuration=(e,t=!0)=>{let r=0,o=0,n=0;e>86400&&(r=Math.floor(e/86400),e-=86400*r),e>3600&&(o=Math.floor(e/3600),e-=3600*o),e>60&&(n=Math.floor(e/60),e-=60*n);let l=`${r} day${1!=r?"s":""}, ${o} hour${1!=o?"s":""}, ${n} minute${1!=n?"s":""}, ${e=Math.floor(e)} second${1!=e?"s":""}`;if(t&&0==r){let e=l.split(", ");return 0==o&&0==n?e.slice(3).join(", "):0==o?e.slice(2).join(", "):e.slice(1).join(", ")}return l};export let getCookies=()=>document.cookie.split(";").reduce(((e,t)=>{let r=strip(t).split("=");return e[r[0]]=r[1],e}),{});export let getCookie=e=>getCookies()[e];export let jaroWinkler=(e,t,r)=>{let o,n,l=0;if(0===e.length||0===t.length)return 0;if(e===t)return 1;let s=Math.floor(Math.max(e.length,t.length)/2)-1,a=new Array(e.length),i=new Array(t.length);for(o=0;o<e.length;o++){let r=o>=s?o-s:0,u=o+s<=t.length-1?o+s:t.length-1;for(n=r;n<=u;n++)if(!0!==a[o]&&!0!==i[n]&&e[o]===t[n]){++l,a[o]=i[n]=!0;break}}if(0===l)return 0;let u=0,p=0;for(o=0;o<e.length;o++)if(!0===a[o]){for(n=u;n<t.length;n++)if(!0===i[n]){u=n+1;break}e[o]!==t[n]&&++p}let c=(l/e.length+l/t.length+(l-p/2)/l)/3,f=0;if(null==r&&(r=.1),c>.7){for(;e[f]===t[f]&&f<4;)++f;c+=f*r*(1-c)}return c};export let getPermutations=e=>{let t,r,o=e.length,n=[e.slice()],l=new Array(o).fill(0),s=1;for(;s<o;)l[s]<s?(t=s%2&&l[s],r=e[s],e[s]=e[t],e[t]=r,++l[s],s=1,n.push(e.slice())):(l[s]=0,++s);return n};export let permutedSentenceJaroWinkler=(e,t)=>{let r=0;for(let o of getPermutations(e.split(" ")))for(let e of getPermutations(t.split(" ")))r=Math.max(r,jaroWinkler(o.join(" "),e.join(" ")));return r};export let ceilingTo=(e,t)=>Math.ceil(e/t)*t;export let floorTo=(e,t)=>Math.floor(e/t)*t;export let roundTo=(e,t)=>Math.round(e/t)*t;export let roundToFactor=(e,t)=>roundTo(e,10**t);export let roundToPrecision=(e,t)=>{return r=10**t,Math.round(e*r)/r;var r};export let clamp=(e,t=0,r=1)=>Math.max(Math.min(isNaN(e)?0:e,r),t);export let parseSelector=e=>{let t={};return e.split(/(?=\.)|(?=#)|(?=\[)/).forEach((e=>{switch(e[0]){case"#":void 0===t.ids&&(t.ids=[]),t.ids.push(e.slice(1));break;case".":void 0===t.classes&&(t.classes=[]),t.classes.push(e.slice(1));break;case"[":void 0===t.attributes&&(t.attributes={});let[r,o]=e.slice(1,-1).split("=");t.attributes[r]=strip(o);break;default:void 0===t.tags&&(t.tags=[]),t.tags.push(e)}})),t};export function*shiftingFrameIterator(e,t){for(let r=0;r<e.length-t+1;r++)yield e.slice(r,r+t)}export function*zip(...e){let t=Math.min(...e.map((e=>e.length)));for(let r=0;r<t;r++)yield e.map((e=>e[r]))}export let hslToRgb=(e,t,r)=>{let o,n,l;if(0===t)o=n=l=r;else{let s=(e,t,r)=>(r<0&&(r+=1),r>1&&(r-=1),r<1/6?e+6*(t-e)*r:r<.5?t:r<2/3?e+(t-e)*(2/3-r)*6:e),a=r<.5?r*(1+t):r+t-r*t,i=2*r-a;o=s(i,a,e+1/3),n=s(i,a,e),l=s(i,a,e-1/3)}return[Math.round(255*o),Math.round(255*n),Math.round(255*l)]};export let rgbToHsl=(e,t,r)=>{e/=255,t/=255,r/=255;let o,n,l=Math.max(e,t,r),s=Math.min(e,t,r),a=(l+s)/2;if(l===s)o=n=0;else{let i=l-s;switch(n=a>.5?i/(2-l-s):i/(l+s),l){case e:o=(t-r)/i+(t<r?6:0);break;case t:o=(r-e)/i+2;break;case r:o=(e-t)/i+4}o/=6}return[o,n,a]};export let rgbToHex=(e,t,r)=>{let o=e=>(e<16?"0":"")+e.toString(16);return`#${o(e)}${o(t)}${o(r)}`};export let hslToHex=(e,t,r)=>rgbToHex(...hslToRgb(e,t,r));export let hexToRgb=e=>(e.startsWith("#")&&(e=e.substr(1)),[parseInt(e.substr(0,2),16),parseInt(e.substr(2,2),16),parseInt(e.substr(4),16)]);export let hexToHsl=e=>rgbToHsl(...hexToRgb(e));const pluralRules=new Intl.PluralRules("en-US",{type:"ordinal"}),suffixes=new Map([["one","st"],["two","nd"],["few","rd"],["other","th"]]);export let formatOrdinal=e=>`${e}${suffixes.get(pluralRules.select(e))}`;export let promptFiles=(e="*",t=!1)=>new Promise(((r,o)=>{let n=document.createElement("input"),l=e=>{window.removeEventListener("mousemove",l),o("No files selected.")};n.type="file",n.multiple=t,n.accept=e,n.onchange=()=>{let e=Array.from(n.files);window.removeEventListener("mousemove",l),r(t?e:e[0])},n.click(),window.addEventListener("mousemove",l)}));export let stripHTML=e=>e.replace(/<[^>]*>?/gm,"");
+export let every=e=>{for(let t of e)if(!t)return!1;return!0};export let none=e=>{for(let t of e)if(t)return!1;return!0};export let any=e=>{for(let t of e)if(t)return!0;return!1};export let flatten=e=>e.reduce(((e,t)=>e.concat(Array.isArray(t)?flatten(t):t)),[]);export let strip=e=>{if(isEmpty(e))return e;let t=e.match(/^[\ \t\r\n\'\"]*(.*?)[\ \t\r\n\'\"]*$/);return null===t?"":t[1]};export let sleep=e=>new Promise((t=>{setTimeout(t,e)}));export let waitFor=async(e,t)=>{let r=(t=t||{}).interval||50,o=t.timeout,n=new Date,l=0;for(;!e();)if(await sleep(r),l=new Date-n,!isEmpty(o)&&l>o)throw"Timeout"};export let guessCase=e=>(e=strip(e),/^$/.test(e)?"EMPTY":/^[a-z09]+$/.test(e)?"LOWER":/^[A-Z09]+$/.test(e)?"UPPER":/^[A-Za-z0-9]+(_[A-Za-z0-9]+)+$/.test(e)?"SNAKE":/^[A-Za-z0-9]+(-[A-Za-z0-9]+)+$/.test(e)?"KEBAB":/^[a-z]+([A-Z][a-z0-9]+)+$/.test(e)?"CAMEL":/^([A-Z][a-z0-9]+)+$/.test(e)?"PASCAL":/^(\w+)((\W\w+)+)$/.test(e)?"SENTENCE":"UNKNOWN");export let guessStringParts=e=>{switch(e=strip(e),guessCase(e)){case"SENTENCE":return e.split(" ").map((e=>e.toLowerCase()));case"SNAKE":return e.split("_").map((e=>e.toLowerCase()));case"KEBAB":return e.split("-").map((e=>e.toLowerCase()));case"CAMEL":return e.split(/([A-Z])/g).reduce(((e,t,r)=>0==r||r%2==1?e.concat([t]):e.concat([e.splice(-1)[0]+t])),[]).map((e=>e.toLowerCase()));case"PASCAL":return e.split(/([A-Z])/g).reduce(((e,t,r)=>0==r?e:r%2==1?e.concat([t]):e.concat([e.splice(-1)[0]+t])),[]).map((e=>e.toLowerCase()));default:return[e.toLowerCase()]}};export let kebabCase=(e,t)=>(void 0===t&&(t="-"),guessStringParts(e).join(t));export let snakeCase=(e,t)=>(void 0===t&&(t="_"),guessStringParts(e).join(t));export let camelCase=(e,t)=>(void 0===t&&(t=""),guessStringParts(e).map(((e,t)=>0==t?e:e[0].toUpperCase()+e.substr(1))).join(t));export let pascalCase=(e,t)=>(void 0===t&&(t=""),guessStringParts(e).map((e=>e[0].toUpperCase()+e.substr(1))).join(t));export let titleCase=e=>pascalCase(e," ");export let caseInsensitiveMatch=(e,t)=>e.toLowerCase()===t.toLowerCase()||kebabCase(e)===kebabCase(t);export let truncate=(e,t,r="…")=>e.length<=t?e:e.substring(0,e.lastIndexOf(" ",t))+r;export let set=e=>e.filter(((t,r)=>e.indexOf(t)===r));export let merge=function(){let e=Array.from(arguments),t={...e[0]};for(let r=1;r<e.length;r++){let o=e[r];for(let e in o)void 0===t[e]?t[e]=o[e]:"object"==typeof t[e]&&"object"==typeof o[e]?t[e]=merge(t[e],o[e]):t[e]=o[e]}return t};const mouseEvents=["click","dblclick","mouseenter","mouseleave","mouseup","mousedown","mousemove","mouseover","mouseout","contextmenu"];export let createEvent=e=>"function"==typeof MouseEvent&&mouseEvents.indexOf(e)>-1?new MouseEvent(e):"function"==typeof Event?new Event(e):(()=>{let t=document.createEvent("Event");return t.initEvent(e,!0,!0),t})();export let randomInt=(e,t)=>(void 0===t?0:e)+Math.random()*(void 0===t?e:t-e)|0;export let randomHex=e=>isEmpty(e)?randomInt(16).toString(16):new Array(e).fill(null).map(randomHex).join("");export let randomChoice=e=>e[randomInt(e.length)];export let uuid=()=>`${randomHex(8)}-${randomHex(4)}-4${randomHex(3)}-${randomChoice(["8","9","a","b"])}${randomHex(3)}-${randomHex(12)}`;export let isEquivalent=(e,t)=>{if(typeof e==typeof t){if(Array.isArray(e)&&Array.isArray(t)){if(e.length!==t.length)return!1;for(let r=0;r<e.length;r++)if(!isEquivalent(e[r],t[r]))return!1;return!0}if("object"==typeof e){if(null===e)return null===t;if(null===t)return!1;let r=Object.getOwnPropertyNames(e),o=Object.getOwnPropertyNames(t);if(!isEquivalent(r,o))return!1;for(let o of r)if(!isEquivalent(e[o],t[o]))return!1;return!0}return e===t}return!1};export let getQueryParameters=()=>-1===window.location.href.indexOf("?")?{}:window.location.href.substring(window.location.href.indexOf("?")+1).split("&").reduce(((e,t)=>{let r=t.split("="),o=r[0],n=decodeURIComponent(r[1]).replace("+"," ");return e.hasOwnProperty(o)?(Array.isArray(e[o])||(e[o]=[e[o]]),e[o].push(n)):e[o]=n,e}),{});export let getDataParameters=e=>{let t={};for(let r=0,o=e.attributes,n=o.length;r<n;r++)o[r].nodeName.startsWith("data")&&(t[camelCase(o[r].nodeName.substr(5))]=o[r].nodeValue);return t};export let buildQueryURL=(e,t)=>{let r=e;return-1===e.indexOf("?")&&(r+="?"),r+Object.getOwnPropertyNames(t).map((e=>`${e}=${encodeURIComponent(t[e])}`)).join("&")};export let getQueryURL=e=>buildQueryURL(window.location.href,e);export let isEmpty=e=>null==e||""===e||"null"===e||Array.isArray(e)&&0===e.length||"object"==typeof e&&"Object"===e.constructor.name&&0===Object.getOwnPropertyNames(e).length;export let removeEmpty=e=>{if(Array.isArray(e)){let t=[];for(let r of e)isEmpty(v)||t.push(v);return t}if("object"==typeof e){let t={};for(let r of Object.getOwnPropertyNames(e))isEmpty(e[r])||(t[r]=e[r]);return t}return e};export let deepClone=(e,t=!0)=>{if(null==e)return e;if("function"==typeof e){if(t)throw"Cannot clone functions.";return e}return"boolean"==typeof e?!!e:"number"==typeof e?0+e:"string"==typeof e||e instanceof String?`${e}`:Array.isArray(e)?new Array(e.length).fill(null).map(((t,r)=>deepClone(e[r],!1))):"object"==typeof e||e===Object(e)?"RegExp"===e.constructor.name?e:Object.getOwnPropertyNames(e).reduce(((t,r)=>(t[r]=deepClone(e[r],!1),t)),new Object):(console.warn("Unknown clone type for",e),e)};const byteSuffixes=["B","KB","MB","GB","TB","PB","EB","ZB","YB"];export let humanSize=(e,t)=>{void 0===t&&(t=2);let r=0;for(;e>1e3;)e/=1e3,r++;return`${e.toFixed(t)} ${byteSuffixes[r]}`};const secondsPerMinute=60,secondsPerHour=3600,secondsPerDay=86400;export let humanDuration=(e,t=!0)=>{let r=0,o=0,n=0;e>86400&&(r=Math.floor(e/86400),e-=86400*r),e>3600&&(o=Math.floor(e/3600),e-=3600*o),e>60&&(n=Math.floor(e/60),e-=60*n);let l=`${r} day${1!=r?"s":""}, ${o} hour${1!=o?"s":""}, ${n} minute${1!=n?"s":""}, ${e=Math.floor(e)} second${1!=e?"s":""}`;if(t&&0==r){let e=l.split(", ");return 0==o&&0==n?e.slice(3).join(", "):0==o?e.slice(2).join(", "):e.slice(1).join(", ")}return l};export let getCookies=()=>document.cookie.split(";").reduce(((e,t)=>{let r=strip(t).split("=");return e[r[0]]=r[1],e}),{});export let getCookie=e=>getCookies()[e];export let jaroWinkler=(e,t,r)=>{let o,n,l=0;if(0===e.length||0===t.length)return 0;if(e===t)return 1;let s=Math.floor(Math.max(e.length,t.length)/2)-1,a=new Array(e.length),i=new Array(t.length);for(o=0;o<e.length;o++){let r=o>=s?o-s:0,u=o+s<=t.length-1?o+s:t.length-1;for(n=r;n<=u;n++)if(!0!==a[o]&&!0!==i[n]&&e[o]===t[n]){++l,a[o]=i[n]=!0;break}}if(0===l)return 0;let u=0,p=0;for(o=0;o<e.length;o++)if(!0===a[o]){for(n=u;n<t.length;n++)if(!0===i[n]){u=n+1;break}e[o]!==t[n]&&++p}let c=(l/e.length+l/t.length+(l-p/2)/l)/3,f=0;if(null==r&&(r=.1),c>.7){for(;e[f]===t[f]&&f<4;)++f;c+=f*r*(1-c)}return c};export let getPermutations=e=>{let t,r,o=e.length,n=[e.slice()],l=new Array(o).fill(0),s=1;for(;s<o;)l[s]<s?(t=s%2&&l[s],r=e[s],e[s]=e[t],e[t]=r,++l[s],s=1,n.push(e.slice())):(l[s]=0,++s);return n};export let permutedSentenceJaroWinkler=(e,t)=>{let r=0;for(let o of getPermutations(e.split(" ")))for(let e of getPermutations(t.split(" ")))r=Math.max(r,jaroWinkler(o.join(" "),e.join(" ")));return r};export let ceilingTo=(e,t)=>Math.ceil(e/t)*t;export let floorTo=(e,t)=>Math.floor(e/t)*t;export let roundTo=(e,t)=>Math.round(e/t)*t;export let roundToFactor=(e,t)=>roundTo(e,10**t);export let roundToPrecision=(e,t)=>{return r=10**t,Math.round(e*r)/r;var r};export let clamp=(e,t=0,r=1)=>Math.max(Math.min(isNaN(e)?0:e,r),t);export let parseSelector=e=>{let t={};return e.split(/(?=\.)|(?=#)|(?=\[)/).forEach((e=>{switch(e[0]){case"#":void 0===t.ids&&(t.ids=[]),t.ids.push(e.slice(1));break;case".":void 0===t.classes&&(t.classes=[]),t.classes.push(e.slice(1));break;case"[":void 0===t.attributes&&(t.attributes={});let[r,o]=e.slice(1,-1).split("=");t.attributes[r]=strip(o);break;default:void 0===t.tags&&(t.tags=[]),t.tags.push(e)}})),t};export function*shiftingFrameIterator(e,t){for(let r=0;r<e.length-t+1;r++)yield e.slice(r,r+t)}export function*zip(...e){let t=Math.min(...e.map((e=>e.length)));for(let r=0;r<t;r++)yield e.map((e=>e[r]))}export let hslToRgb=(e,t,r)=>{let o,n,l;if(0===t)o=n=l=r;else{let s=(e,t,r)=>(r<0&&(r+=1),r>1&&(r-=1),r<1/6?e+6*(t-e)*r:r<.5?t:r<2/3?e+(t-e)*(2/3-r)*6:e),a=r<.5?r*(1+t):r+t-r*t,i=2*r-a;o=s(i,a,e+1/3),n=s(i,a,e),l=s(i,a,e-1/3)}return[Math.round(255*o),Math.round(255*n),Math.round(255*l)]};export let rgbToHsl=(e,t,r)=>{e/=255,t/=255,r/=255;let o,n,l=Math.max(e,t,r),s=Math.min(e,t,r),a=(l+s)/2;if(l===s)o=n=0;else{let i=l-s;switch(n=a>.5?i/(2-l-s):i/(l+s),l){case e:o=(t-r)/i+(t<r?6:0);break;case t:o=(r-e)/i+2;break;case r:o=(e-t)/i+4}o/=6}return[o,n,a]};export let rgbToHex=(e,t,r)=>{let o=e=>(e<16?"0":"")+e.toString(16);return`#${o(e)}${o(t)}${o(r)}`};export let hslToHex=(e,t,r)=>rgbToHex(...hslToRgb(e,t,r));export let hexToRgb=e=>(e.startsWith("#")&&(e=e.substr(1)),[parseInt(e.substr(0,2),16),parseInt(e.substr(2,2),16),parseInt(e.substr(4),16)]);export let hexToHsl=e=>rgbToHsl(...hexToRgb(e));const pluralRules=new Intl.PluralRules("en-US",{type:"ordinal"}),suffixes=new Map([["one","st"],["two","nd"],["few","rd"],["other","th"]]);export let formatOrdinal=e=>`${e}${suffixes.get(pluralRules.select(e))}`;export let promptFiles=(e="*",t=!1)=>new Promise(((r,o)=>{let n=document.createElement("input"),l=e=>{window.removeEventListener("mousemove",l),o("No files selected.")};n.type="file",n.multiple=t,n.accept=e,n.onchange=()=>{let e=Array.from(n.files);window.removeEventListener("mousemove",l),r(t?e:e[0])},n.click(),window.addEventListener("mousemove",l)}));export let stripHTML=e=>e.replace(/<[^>]*>?/gm,"");export let createElementsFromString=e=>{let t=document.createElement("div");return t.innerHTML=e.trim(),t.childNodes};
```

### Comparing `enfugue-0.1.2/enfugue/static/js/base/loader.mjs` & `enfugue-0.1.3/enfugue/static/js/base/loader.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/base/publisher.mjs` & `enfugue-0.1.3/enfugue/static/js/base/publisher.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/base/session.mjs` & `enfugue-0.1.3/enfugue/static/js/base/session.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/base/watcher.mjs` & `enfugue-0.1.3/enfugue/static/js/base/watcher.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/common/event-tracker.mjs` & `enfugue-0.1.3/enfugue/static/js/common/event-tracker.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/common/history.mjs` & `enfugue-0.1.3/enfugue/static/js/common/history.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/common/shadowbox.mjs` & `enfugue-0.1.3/enfugue/static/js/common/shadowbox.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/common/tooltip.mjs` & `enfugue-0.1.3/enfugue/static/js/common/tooltip.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/config/index.mjs` & `enfugue-0.1.3/enfugue/static/js/config/index.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/controller/base.mjs` & `enfugue-0.1.3/enfugue/static/js/controller/base.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/controller/common/announcements.mjs` & `enfugue-0.1.3/enfugue/static/js/controller/common/announcements.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/controller/common/downloads.mjs` & `enfugue-0.1.3/enfugue/static/js/controller/common/downloads.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/controller/common/invocation.mjs` & `enfugue-0.1.3/enfugue/static/js/controller/common/invocation.mjs`

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
-import{ImageInspectorView}from"../../view/image.mjs";import{isEmpty,isEquivalent,waitFor,humanDuration}from"../../base/helpers.mjs";import{ElementBuilder}from"../../base/builder.mjs";import{Controller}from"../base.mjs";const E=new ElementBuilder({invocationLoading:"enfugue-invocation-loading",invocationLoaded:"enfugue-invocation-loaded",invocationDuration:"enfugue-invocation-duration",invocationIterations:"enfugue-invocation-iterations",invocationRemaining:"enfugue-invocation-remaining",invocationSampleChooser:"enfugue-invocation-sample-chooser",invocationSample:"enfugue-invocation-sample",invocationStop:"enfugue-invocation-stop"});class InvocationController extends Controller{static truncatePromptLength=36;constructor(i){super(i),this.kwargs={}}get width(){return this.kwargs.width||this.application.config.model.invocation.width}set width(i){this.width!==i&&this.publish("engineWidthChange",i),this.kwargs.width=i}get height(){return this.kwargs.height||this.application.config.model.invocation.height}set height(i){this.height!==i&&this.publish("engineHeightChange",i),this.kwargs.height=i}get chunkingSize(){return this.kwargs.chunking_size||this.application.config.model.invocation.chunkingSize}set chunkingSize(i){this.chunkingSize!==i&&this.publish("engineChunkingSizeChange",i),this.kwargs.chunking_size=i}get chunkingBlur(){return this.kwargs.chunking_blur||this.application.config.model.invocation.chunkingBlur}set chunkingBlur(i){this.chunkingBlur!==i&&this.publish("engineChunkingBlurChange",i),this.kwargs.chunking_blur=i}get prompt(){return this.kwargs.prompt||""}set prompt(i){this.prompt!==i&&this.publish("enginePromptChange",i),this.kwargs.prompt=i}get negativePrompt(){return this.kwargs.negative_prompt||""}set negativePrompt(i){this.negativePrompt!==i&&this.publish("engineNegativePromptChange",i),this.kwargs.negative_prompt=i}get samples(){return this.kwargs.samples||1}set samples(i){this.samples!==i&&this.publish("engineSamplesChange",i),this.kwargs.samples=i}get seed(){return this.kwargs.seed}set seed(i){this.seed!==i&&this.publish("engineSeedChange",i),this.kwargs.seed=i}get guidanceScale(){return this.kwargs.guidance_scale||this.application.config.model.invocation.guidanceScale}set guidanceScale(i){this.guidanceScale!==i&&this.publish("engineGuidanceScaleChange",i),this.kwargs.guidance_scale=i}get inferenceSteps(){return this.kwargs.num_inference_steps||this.application.config.model.invocation.inferenceSteps}set inferenceSteps(i){this.inferenceSteps!==i&&this.publish("engineInferenceStepsChange",i),this.kwargs.num_inference_steps=i}get model(){return this.kwargs.model}set model(i){this.model!==i&&this.publish("engineModelChange",i),this.kwargs.model=i}get outscale(){return this.kwargs.outscale||1}set outscale(i){this.outscale!==i&&this.publish("engineOutscaleChange",i),this.kwargs.outscale=parseInt(i)}get upscale(){return this.kwargs.upscale}set upscale(i){isEquivalent(this.upscale,i)||this.publish("engineUpscaleChange",i),this.kwargs.upscale=i}get upscaleIterative(){return!0===this.kwargs.upscale_iterative}set upscaleIterative(i){this.upscaleIterative!==i&&this.publish("engineUpscaleIterativeChange",i),this.kwargs.upscale_iterative=i}get upscaleDiffusion(){return!0===this.kwargs.upscale_diffusion}set upscaleDiffusion(i){this.upscaleDiffusion!==i&&this.publish("engineUpscaleDiffusionChange",i),this.kwargs.upscale_diffusion=i}get upscaleDiffusionPrompt(){return this.kwargs.upscale_diffusion_prompt}set upscaleDiffusionPrompt(i){isEquivalent(this.upscaleDiffusionPrompt,i)||this.publish("engineUpscaleDiffusionPromptChange",i),this.kwargs.upscale_diffusion_prompt=i}get upscaleDiffusionNegativePrompt(){return this.kwargs.upscale_diffusion_negative_prompt}set upscaleDiffusionNegativePrompt(i){isEquivalent(this.upscaleDiffusionNegativePrompt,i)||this.publish("engineUpscaleDiffusionNegativePromptChange",i),this.kwargs.upscale_diffusion_negative_prompt=i}get upscaleDiffusionSteps(){return this.kwargs.upscale_diffusion_steps||this.application.config.model.invocation.upscaleDiffusionSteps}set upscaleDiffusionSteps(i){isEquivalent(this.upscaleDiffusionSteps,i)||this.publish("engineUpscaleDiffusionStepsChange",i),this.kwargs.upscale_diffusion_steps=i}get upscaleDiffusionStrength(){return this.kwargs.upscale_diffusion_strength||this.application.config.model.invocation.upscaleDiffusionStrength}set upscaleDiffusionStrength(i){isEquivalent(this.upscaleDiffusionStrength,i)||this.publish("engineUpscaleDiffusionStrengthChange",i),this.kwargs.upscale_diffusion_strength=i}get upscaleDiffusionGuidanceScale(){return this.kwargs.upscale_diffusion_guidance_scale||this.application.config.model.invocation.upscaleDiffusionGuidanceScale}set upscaleDiffusionGuidanceScale(i){isEquivalent(this.upscaleDiffusionGuidanceScale,i)||this.publish("engineUpscaleDiffusionGuidanceScaleChange",i),this.kwargs.upscale_diffusion_guidance_scale=i}get upscaleDiffusionChunkingSize(){return this.kwargs.upscale_diffusion_chunking_size||this.application.config.model.invocation.upscaleDiffusionChunkingSize}set upscaleDiffusionChunkingSize(i){this.upscaleDiffusionChunkingSize!==i&&this.publish("engineUpscaleDiffusionChunkingSizeChange",i),this.kwargs.upscale_diffusion_chunking_size=i}get upscaleDiffusionChunkingBlur(){return this.kwargs.upscale_diffusion_chunking_blur||this.application.config.model.invocation.upscaleDiffusionChunkingBlur}set upscaleDiffusionChunkingBlur(i){this.upscaleDiffusionChunkingBlur!==i&&this.publish("engineUpscaleDiffusionChunkingBlurChange",i),this.kwargs.upscale_diffusion_chunking_blur=i}get upscaleDiffusionScaleChunkingSize(){return!1!==this.kwargs.upscale_diffusion_scale_chunking_size}set upscaleDiffusionScaleChunkingSize(i){this.upscaleDiffusionScaleChunkingSize!==i&&this.publish("engineUpscaleDiffusionScaleChunkingSizeChange",i),this.kwargs.upscale_diffusion_scale_chunking_size=i}get upscaleDiffusionScaleChunkingBlur(){return!1!==this.kwargs.upscale_diffusion_scale_chunking_blur}set upscaleDiffusionScaleChunkingBlur(i){this.upscaleDiffusionScaleChunkingBlur!==i&&this.publish("engineUpscaleDiffusionScaleChunkingBlurChange",i),this.kwargs.upscale_diffusion_scale_chunking_blur=i}get upscaleDiffusionControlnet(){return this.kwargs.upscale_diffusion_controlnet||null}set upscaleDiffusionControlnet(i){isEquivalent(this.upscaleDiffusionControlnet,i)||this.publish("engineUpscaleDiffusionControlnetChange",i),this.kwargs.upscale_diffusion_controlnet=i}async initialize(){this.loadingBar=E.invocationLoading().content(E.invocationLoaded().addClass("sliding-gradient"),E.invocationDuration(),E.invocationIterations(),E.invocationRemaining().hide()),this.invocationSampleChooser=E.invocationSampleChooser().hide(),this.invocationStop=E.invocationStop().content("Stop").on("click",(()=>{this.stopInvocation()})),(await this.images.getNode()).append(this.loadingBar).append(this.invocationSampleChooser).append(this.invocationStop)}hideSampleChooser(){this.invocationSampleChooser.hide()}async invoke(i,e=!1){i=isEmpty(i)?{}:i;let t={...this.kwargs,...i};if(isEmpty(t.prompt))return void this.notify("Error","Missing Prompt","A prompt is required.");let n=await this.application.model.post("invoke",null,null,t);if(this.invocationStop.addClass("ready"),!isEmpty(n.uuid))if(e){let i=t.prompt.substring(0,this.constructor.truncatePromptLength);i.length===this.constructor.truncatePromptLength&&(i+="..."),await this.startDetachedInvocationMonitor(i,n.uuid,parseInt(t.width)||512,parseInt(t.height)||512)}else await this.canvasInvocation(n.uuid),this.invocationStop.removeClass("ready")}async stopInvocation(){if(this.invocationStop.hasClass("ready"))try{await this.application.model.post("/invocation/stop"),this.invocationStop.removeClass("ready"),this.notify("info","Stopped","Successfully stopped engine.")}catch(i){let e=`${i}`;isEmpty(i.detail)?isEmpty(i.title)||(e=i.title):e=i.detail,this.notify("error","Error",`Received an error when stopping. The engine may still be stopped, wait a moment and check again. ${e}`)}}async monitorInvocation(i,e,t,n){const s=this.application.config.model.invocation.interval||1e3,a=this.application.config.model.queue.interval||5e3,o=this.application.config.model.invocation.errors.consecutive||2;void 0===e&&(e=()=>{}),void 0===t&&(t=()=>{}),void 0===n&&(n=()=>{});let u,l,r,c,h,p,g=(new Date).getTime(),f=i=>"queued"===i.status?a:Math.min(Math.max(s,(()=>{let i=u/(h-g),e=isEmpty(r)?i:r/1e3,t=(l-u)/(.75*e+.25*i)-((new Date).getTime()-h);return isNaN(t)&&(t=1/0),n(t,u,l,r,c),t})()/2),a),m=async()=>{let n,s;for(let e=0;e<o;e++)try{n=await this.application.model.get(`/invocation/${i}`)}catch(i){s=i}if(isEmpty(n))return this.notify("error","Invocation Error",`${o} consecutive errors were detected communicating with the server. Please check the server logs. The last error was: ${s}`),void t();if(n.total!==l&&(isEmpty(l)||(g=(new Date).getTime()),l=n.total),n.step!==u&&(u=n.step,h=(new Date).getTime()),n.rate!==r&&(r=n.rate),c=n.duration,!isEmpty(n.images)){let i=n.images.map((i=>`/api/invocation/${i}`)),t="completed"===n.status;e(i,t)}if("error"===n.status)return this.notify("error","Invocation Failed",n.message),void t();"completed"!==n.status&&(p=setTimeout(m,f(n)))};m()}async canvasInvocation(i){let e,t,n,s,a,o,u,l,r,c,h=!1,p=!1,g=(new Date).getTime(),f=g,m=g,d=g,v=0,w=[],k=this.loadingBar.find(E.getCustomTag("invocationLoaded")),C=this.loadingBar.find(E.getCustomTag("invocationDuration")),S=this.loadingBar.find(E.getCustomTag("invocationIterations")),_=this.loadingBar.find(E.getCustomTag("invocationRemaining")),D=()=>{if(isEmpty(o))this.invocationSampleChooser.hide();else if(0===w.length){this.images.setCurrentInvocationImage(o[0]),this.invocationSampleChooser.empty().append(E.invocationSample().class("no-sample").content("×").on("click",(()=>{v=null,this.images.hideCurrentInvocation()})));for(let i in o){let e=E.img().src(o[i]);w.push(e),this.invocationSampleChooser.append(E.invocationSample().content(e).on("click",(()=>{this.images.setCurrentInvocationImage(e.src()),v=i})))}this.invocationSampleChooser.show().render()}else{for(let i in o)w[i].src(o[i]);null!==v&&this.images.setCurrentInvocationImage(o[v])}},y=()=>{let i=(new Date).getTime();if(p)s<100&&s>0?s+=1:(s=100,h=!0);else if(!isEmpty(t)&&t<1/0){let o=i-m,u=t-(i-n),l=o+u;a=u,e=l,s=o/l*100}f=i,(()=>{let i=f-g;if(C.content(humanDuration(i/1e3)),isEmpty(s))k.css("width","100%"),S.hide(),_.show().content("Initializing…");else if(s<100){_.show().content(humanDuration(a/1e3)),k.css("width",`${s.toFixed(2)}%`);let i=r,e="it/s";!isEmpty(i)&&i<1/0?(i<1&&(i=1/i,e="s/it"),S.show().content(`Iteration ${u}/${l} (${i.toFixed(2)} ${e})`)):S.show().content(`Iteration ${u}/${l}`)}else if(h||isEmpty(c))k.css("width","0"),_.empty().hide();else{_.content("Finalizing step…");let i=l/c,e="it/s";i<1&&(i=1/i,e="s/it"),S.content(`${l} Iterations at ${i.toFixed(2)} ${e}`),k.css("width","100%")}})(),h||requestAnimationFrame((()=>y()))};this.loadingBar.addClass("loading"),this.images.hideCurrentInvocation(),this.invocationSampleChooser.empty(),window.requestAnimationFrame((()=>y())),this.monitorInvocation(i,(async(i,e)=>{p=e,i.length>0&&(o=i,D())}),(()=>{p=!0,h=!0,_.empty().hide(),S.empty().hide()}),((i,e,a,o,h)=>{t=i,u!==e&&(d=n),u=e,r=o,c=h,n=(new Date).getTime(),l!==a&&(m=n,isEmpty(l)||(u=0,s=null,d=n)),l=a})),await waitFor((()=>h)),this.loadingBar.removeClass("loading")}async startDetachedInvocationMonitor(i,e,t,n){let s=!1,a=[],o=[];this.monitorInvocation(e,(async(u,l,r)=>{s=!0;for(let s in u){let l=u[s];if(a.length<=s){let u=new ImageInspectorView(this.application.config,l,e),r=await this.spawnWindow(`${i}, sample ${s+1}`,u,t+30,n+90);u.loading(),a.push(r),o.push(u)}else o[s].setImage(l),a[s].setName(`${i}, ${r} elapsed, sample ${s+1}`)}if(l)for(let e in a)a[e].setName(`${i} complete in ${r}, sample ${e+1}`),o[e].doneLoading()}),(()=>s=!0)),await waitFor((()=>!0===s))}}export{InvocationController};
+import{ImageInspectorView}from"../../view/image.mjs";import{isEmpty,isEquivalent,waitFor,humanDuration}from"../../base/helpers.mjs";import{ElementBuilder}from"../../base/builder.mjs";import{Controller}from"../base.mjs";const E=new ElementBuilder({invocationLoading:"enfugue-invocation-loading",invocationLoaded:"enfugue-invocation-loaded",invocationDuration:"enfugue-invocation-duration",invocationIterations:"enfugue-invocation-iterations",invocationRemaining:"enfugue-invocation-remaining",invocationSampleChooser:"enfugue-invocation-sample-chooser",invocationSample:"enfugue-invocation-sample",invocationStop:"enfugue-invocation-stop"});class InvocationController extends Controller{static truncatePromptLength=36;constructor(i){super(i),this.kwargs={}}get width(){return this.kwargs.width||this.application.config.model.invocation.width}set width(i){this.width!==i&&this.publish("engineWidthChange",i),this.kwargs.width=i}get height(){return this.kwargs.height||this.application.config.model.invocation.height}set height(i){this.height!==i&&this.publish("engineHeightChange",i),this.kwargs.height=i}get chunkingSize(){return this.kwargs.chunking_size||this.application.config.model.invocation.chunkingSize}set chunkingSize(i){this.chunkingSize!==i&&this.publish("engineChunkingSizeChange",i),this.kwargs.chunking_size=i}get chunkingBlur(){return this.kwargs.chunking_blur||this.application.config.model.invocation.chunkingBlur}set chunkingBlur(i){this.chunkingBlur!==i&&this.publish("engineChunkingBlurChange",i),this.kwargs.chunking_blur=i}get prompt(){return this.kwargs.prompt||""}set prompt(i){this.prompt!==i&&this.publish("enginePromptChange",i),this.kwargs.prompt=i}get negativePrompt(){return this.kwargs.negative_prompt||""}set negativePrompt(i){this.negativePrompt!==i&&this.publish("engineNegativePromptChange",i),this.kwargs.negative_prompt=i}get samples(){return this.kwargs.samples||1}set samples(i){this.samples!==i&&this.publish("engineSamplesChange",i),this.kwargs.samples=i}get seed(){return this.kwargs.seed}set seed(i){this.seed!==i&&this.publish("engineSeedChange",i),this.kwargs.seed=i}get guidanceScale(){return this.kwargs.guidance_scale||this.application.config.model.invocation.guidanceScale}set guidanceScale(i){this.guidanceScale!==i&&this.publish("engineGuidanceScaleChange",i),this.kwargs.guidance_scale=i}get inferenceSteps(){return this.kwargs.num_inference_steps||this.application.config.model.invocation.inferenceSteps}set inferenceSteps(i){this.inferenceSteps!==i&&this.publish("engineInferenceStepsChange",i),this.kwargs.num_inference_steps=i}get model(){return this.kwargs.model}set model(i){this.model!==i&&this.publish("engineModelChange",i),this.kwargs.model=i}get modelType(){return this.kwargs.model_type||"checkpoint"}set modelType(i){this.modelType!==i&&this.publish("engineModelTypeChange",i),this.kwargs.model_type=i}get outscale(){return this.kwargs.outscale||1}set outscale(i){this.outscale!==i&&this.publish("engineOutscaleChange",i),this.kwargs.outscale=parseInt(i)}get upscale(){return this.kwargs.upscale}set upscale(i){isEquivalent(this.upscale,i)||this.publish("engineUpscaleChange",i),this.kwargs.upscale=i}get upscaleIterative(){return!0===this.kwargs.upscale_iterative}set upscaleIterative(i){this.upscaleIterative!==i&&this.publish("engineUpscaleIterativeChange",i),this.kwargs.upscale_iterative=i}get upscaleDiffusion(){return!0===this.kwargs.upscale_diffusion}set upscaleDiffusion(i){this.upscaleDiffusion!==i&&this.publish("engineUpscaleDiffusionChange",i),this.kwargs.upscale_diffusion=i}get upscaleDiffusionPrompt(){return this.kwargs.upscale_diffusion_prompt}set upscaleDiffusionPrompt(i){isEquivalent(this.upscaleDiffusionPrompt,i)||this.publish("engineUpscaleDiffusionPromptChange",i),this.kwargs.upscale_diffusion_prompt=i}get upscaleDiffusionNegativePrompt(){return this.kwargs.upscale_diffusion_negative_prompt}set upscaleDiffusionNegativePrompt(i){isEquivalent(this.upscaleDiffusionNegativePrompt,i)||this.publish("engineUpscaleDiffusionNegativePromptChange",i),this.kwargs.upscale_diffusion_negative_prompt=i}get upscaleDiffusionSteps(){return this.kwargs.upscale_diffusion_steps||this.application.config.model.invocation.upscaleDiffusionSteps}set upscaleDiffusionSteps(i){isEquivalent(this.upscaleDiffusionSteps,i)||this.publish("engineUpscaleDiffusionStepsChange",i),this.kwargs.upscale_diffusion_steps=i}get upscaleDiffusionStrength(){return this.kwargs.upscale_diffusion_strength||this.application.config.model.invocation.upscaleDiffusionStrength}set upscaleDiffusionStrength(i){isEquivalent(this.upscaleDiffusionStrength,i)||this.publish("engineUpscaleDiffusionStrengthChange",i),this.kwargs.upscale_diffusion_strength=i}get upscaleDiffusionGuidanceScale(){return this.kwargs.upscale_diffusion_guidance_scale||this.application.config.model.invocation.upscaleDiffusionGuidanceScale}set upscaleDiffusionGuidanceScale(i){isEquivalent(this.upscaleDiffusionGuidanceScale,i)||this.publish("engineUpscaleDiffusionGuidanceScaleChange",i),this.kwargs.upscale_diffusion_guidance_scale=i}get upscaleDiffusionChunkingSize(){return this.kwargs.upscale_diffusion_chunking_size||this.application.config.model.invocation.upscaleDiffusionChunkingSize}set upscaleDiffusionChunkingSize(i){this.upscaleDiffusionChunkingSize!==i&&this.publish("engineUpscaleDiffusionChunkingSizeChange",i),this.kwargs.upscale_diffusion_chunking_size=i}get upscaleDiffusionChunkingBlur(){return this.kwargs.upscale_diffusion_chunking_blur||this.application.config.model.invocation.upscaleDiffusionChunkingBlur}set upscaleDiffusionChunkingBlur(i){this.upscaleDiffusionChunkingBlur!==i&&this.publish("engineUpscaleDiffusionChunkingBlurChange",i),this.kwargs.upscale_diffusion_chunking_blur=i}get upscaleDiffusionScaleChunkingSize(){return!1!==this.kwargs.upscale_diffusion_scale_chunking_size}set upscaleDiffusionScaleChunkingSize(i){this.upscaleDiffusionScaleChunkingSize!==i&&this.publish("engineUpscaleDiffusionScaleChunkingSizeChange",i),this.kwargs.upscale_diffusion_scale_chunking_size=i}get upscaleDiffusionScaleChunkingBlur(){return!1!==this.kwargs.upscale_diffusion_scale_chunking_blur}set upscaleDiffusionScaleChunkingBlur(i){this.upscaleDiffusionScaleChunkingBlur!==i&&this.publish("engineUpscaleDiffusionScaleChunkingBlurChange",i),this.kwargs.upscale_diffusion_scale_chunking_blur=i}get upscaleDiffusionControlnet(){return this.kwargs.upscale_diffusion_controlnet||null}set upscaleDiffusionControlnet(i){isEquivalent(this.upscaleDiffusionControlnet,i)||this.publish("engineUpscaleDiffusionControlnetChange",i),this.kwargs.upscale_diffusion_controlnet=i}get inversion(){return this.kwargs.inversion||[]}set inversion(i){isEquivalent(this.inversion,i)||this.publish("engineInversionChange",i),this.kwargs.inversion=i}get lora(){return this.kwargs.lora||[]}set lora(i){isEquivalent(this.lora,i)||this.publish("engineLoraChange",i),this.kwargs.lora=i}async initialize(){this.loadingBar=E.invocationLoading().content(E.invocationLoaded().addClass("sliding-gradient"),E.invocationDuration(),E.invocationIterations(),E.invocationRemaining().hide()),this.invocationSampleChooser=E.invocationSampleChooser().hide(),this.invocationStop=E.invocationStop().content("Stop").on("click",(()=>{this.stopInvocation()})),(await this.images.getNode()).append(this.loadingBar).append(this.invocationSampleChooser).append(this.invocationStop)}hideSampleChooser(){this.invocationSampleChooser.hide()}async invoke(i,e=!1){i=isEmpty(i)?{}:i;let t={...this.kwargs,...i};if(isEmpty(t.prompt))return void this.notify("Error","Missing Prompt","A prompt is required.");let n=await this.application.model.post("invoke",null,null,t);if(this.invocationStop.addClass("ready"),!isEmpty(n.uuid))if(e){let i=t.prompt.substring(0,this.constructor.truncatePromptLength);i.length===this.constructor.truncatePromptLength&&(i+="..."),await this.startDetachedInvocationMonitor(i,n.uuid,parseInt(t.width)||512,parseInt(t.height)||512)}else await this.canvasInvocation(n.uuid),this.invocationStop.removeClass("ready")}async stopInvocation(){if(this.invocationStop.hasClass("ready"))try{await this.application.model.post("/invocation/stop"),this.invocationStop.removeClass("ready"),this.notify("info","Stopped","Successfully stopped engine.")}catch(i){let e=`${i}`;isEmpty(i.detail)?isEmpty(i.title)||(e=i.title):e=i.detail,this.notify("error","Error",`Received an error when stopping. The engine may still be stopped, wait a moment and check again. ${e}`)}}async monitorInvocation(i,e,t,n){const s=this.application.config.model.invocation.interval||1e3,a=this.application.config.model.queue.interval||5e3,o=this.application.config.model.invocation.errors.consecutive||2;void 0===e&&(e=()=>{}),void 0===t&&(t=()=>{}),void 0===n&&(n=()=>{});let r,u,l,h,c,p,g=(new Date).getTime(),f=i=>"queued"===i.status?a:Math.min(Math.max(s,(()=>{let i=r/(c-g),e=isEmpty(l)?i:l/1e3,t=(u-r)/(.75*e+.25*i)-((new Date).getTime()-c);return isNaN(t)&&(t=1/0),n(t,r,u,l,h),t})()/2),a),m=async()=>{let n,s;for(let e=0;e<o;e++)try{n=await this.application.model.get(`/invocation/${i}`)}catch(i){s=i}if(isEmpty(n))return this.notify("error","Invocation Error",`${o} consecutive errors were detected communicating with the server. Please check the server logs. The last error was: ${s}`),void t();if(n.total!==u&&(isEmpty(u)||(g=(new Date).getTime()),u=n.total),n.step!==r&&(r=n.step,c=(new Date).getTime()),n.rate!==l&&(l=n.rate),h=n.duration,!isEmpty(n.images)){let i=n.images.map((i=>`/api/invocation/${i}`)),t="completed"===n.status;e(i,t)}if("error"===n.status)return this.notify("error","Invocation Failed",n.message),void t();"completed"!==n.status&&(p=setTimeout(m,f(n)))};m()}async canvasInvocation(i){let e,t,n,s,a,o,r,u,l,h,c=!1,p=!1,g=(new Date).getTime(),f=g,m=g,d=g,v=0,w=[],k=this.loadingBar.find(E.getCustomTag("invocationLoaded")),C=this.loadingBar.find(E.getCustomTag("invocationDuration")),S=this.loadingBar.find(E.getCustomTag("invocationIterations")),_=this.loadingBar.find(E.getCustomTag("invocationRemaining")),D=()=>{if(isEmpty(o))this.invocationSampleChooser.hide();else if(0===w.length){this.images.setCurrentInvocationImage(o[0]),this.invocationSampleChooser.empty().append(E.invocationSample().class("no-sample").content("×").on("click",(()=>{v=null,this.images.hideCurrentInvocation()})));for(let i in o){let e=E.img().src(o[i]);w.push(e),this.invocationSampleChooser.append(E.invocationSample().content(e).on("click",(()=>{this.images.setCurrentInvocationImage(e.src()),v=i})))}this.invocationSampleChooser.show().render()}else{for(let i in o)w[i].src(o[i]);null!==v&&this.images.setCurrentInvocationImage(o[v])}},y=()=>{let i=(new Date).getTime();if(p)s<100&&s>0?s+=1:(s=100,c=!0);else if(!isEmpty(t)&&t<1/0){let o=i-m,r=t-(i-n),u=o+r;a=r,e=u,s=o/u*100}f=i,(()=>{let i=f-g;if(C.content(humanDuration(i/1e3)),isEmpty(s))k.css("width","100%"),S.hide(),_.show().content("Initializing…");else if(s<100){_.show().content(humanDuration(a/1e3)),k.css("width",`${s.toFixed(2)}%`);let i=l,e="it/s";!isEmpty(i)&&i<1/0?(i<1&&(i=1/i,e="s/it"),S.show().content(`Iteration ${r}/${u} (${i.toFixed(2)} ${e})`)):S.show().content(`Iteration ${r}/${u}`)}else if(c||isEmpty(h))k.css("width","0"),_.empty().hide();else{_.content("Finalizing step…");let i=u/h,e="it/s";i<1&&(i=1/i,e="s/it"),S.content(`${u} Iterations at ${i.toFixed(2)} ${e}`),k.css("width","100%")}})(),c||requestAnimationFrame((()=>y()))};this.loadingBar.addClass("loading"),this.images.hideCurrentInvocation(),this.invocationSampleChooser.empty(),window.requestAnimationFrame((()=>y())),this.monitorInvocation(i,(async(i,e)=>{p=e,i.length>0&&(o=i,D())}),(()=>{p=!0,c=!0,_.empty().hide(),S.empty().hide()}),((i,e,a,o,c)=>{t=i,r!==e&&(d=n),r=e,l=o,h=c,n=(new Date).getTime(),u!==a&&(m=n,isEmpty(u)||(r=0,s=null,d=n)),u=a})),await waitFor((()=>c)),this.loadingBar.removeClass("loading")}async startDetachedInvocationMonitor(i,e,t,n){let s=!1,a=[],o=[];this.monitorInvocation(e,(async(r,u,l)=>{s=!0;for(let s in r){let u=r[s];if(a.length<=s){let r=new ImageInspectorView(this.application.config,u,e),l=await this.spawnWindow(`${i}, sample ${s+1}`,r,t+30,n+90);r.loading(),a.push(l),o.push(r)}else o[s].setImage(u),a[s].setName(`${i}, ${l} elapsed, sample ${s+1}`)}if(u)for(let e in a)a[e].setName(`${i} complete in ${l}, sample ${e+1}`),o[e].doneLoading()}),(()=>s=!0)),await waitFor((()=>!0===s))}}export{InvocationController};
```

### Comparing `enfugue-0.1.2/enfugue/static/js/controller/common/model-manager.mjs` & `enfugue-0.1.3/enfugue/static/js/controller/common/model-manager.mjs`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-import{Controller}from"../base.mjs";import{ParentView}from"../../view/base.mjs";import{FormView}from"../../view/forms/base.mjs";import{TableView,ModelTableView}from"../../view/table.mjs";import{StringInputView,TextInputView,FloatInputView,NumberInputView,FormInputView,RepeatableInputView,SearchListInputView,ButtonInputView}from"../../view/forms/input.mjs";import{isEmpty,deepClone}from"../../base/helpers.mjs";class InversionInputView extends SearchListInputView{}class LoraInputView extends SearchListInputView{}class CheckpointInputView extends SearchListInputView{}class LoraFormView extends FormView{static autoSubmit=!0;static fieldSets={LoRA:{model:{label:"Model",class:LoraInputView,config:{required:!0}},weight:{label:"Weight",class:FloatInputView,config:{min:0,value:1,step:.01,required:!0}}}}}class LoraFormInputView extends FormInputView{static formClass=LoraFormView}class MultiLoraInputView extends RepeatableInputView{static memberClass=LoraFormInputView}class MultiInversionInputView extends RepeatableInputView{static memberClass=InversionInputView}class ModelForm extends FormView{static canCancel=!0;static fieldSets={Name:{name:{class:StringInputView,label:"Name",config:{required:!0}}},Model:{checkpoint:{class:CheckpointInputView,label:"Checkpoint",config:{required:!0}},lora:{class:MultiLoraInputView,label:"LoRA"},inversion:{class:MultiInversionInputView,label:"Textual Inversions"}},Engine:{size:{class:NumberInputView,label:"Size",config:{required:!0,value:512,min:128,max:2048,step:8}}},Prompts:{prompt:{class:TextInputView,label:"Prompt"},negative_prompt:{class:TextInputView,label:"Negative Prompt"}}}}class NewModelInputView extends ButtonInputView{static defaultValue="New Model";static className="new-model-input-view"}class ModelManagerController extends Controller{static modelWindowWidth=400;static modelWindowHeight=1e3;static managerWindowWidth=800;static managerWindowHeight=600;async createManager(){this.tableView=new ModelTableView(this.config,this.model.DiffusionModel),this.buttonView=new NewModelInputView(this.config),this.tableView.setColumns({name:"Name",model:"Model",size:"Size",prompt:"Prompt",negative_prompt:"Negative Prompt"}),this.tableView.setFormatter("size",(e=>`${e}px`)),this.tableView.addButton("Edit","fa-solid fa-edit",(async e=>{let t=e.getAttributes();t.checkpoint=t.model,t.lora=isEmpty(e.lora)?[]:e.lora.map((e=>e.getAttributes())),t.inversion=isEmpty(e.inversion)?[]:e.inversion.map((e=>e.model));let i,o=new ModelForm(this.config,deepClone(t));o.onSubmit((async t=>{try{await this.model.put(`/models/${e.name}`,null,null,t),isEmpty(i)||i.remove(),this.tableView.requery()}catch(e){let t=isEmpty(e)?"Couldn't communicate with server.":isEmpty(e.detail)?`${e}`:e.detail;this.notify("error","Couldn't update model",t),o.enable()}})),o.onCancel((()=>i.remove())),i=await this.spawnWindow(`Edit ${e.name}`,o,this.constructor.modelWindowWidth,this.constructor.modelWindowHeight)})),this.tableView.addButton("Delete","fa-solid fa-trash",(async e=>{try{await this.model.delete(`/models/${e.name}`),this.tableView.requery()}catch(e){let t=isEmpty(e)?"Couldn't communicate with server.":isEmpty(e.detail)?`${e}`:e.detail;this.notify("error","Couldn't delete model",t),modelForm.enable()}})),this.buttonView.onChange((()=>{this.showNewModel()}));let e=new ParentView(this.config);return e.addChild(this.tableView),e.addChild(this.buttonView),e}async createModelForm(){let e=new ModelForm(this.config);return e.onSubmit((async e=>{try{await this.model.post("/models",null,null,e);isEmpty(this.newModelWindow)||(this.newModelWindow.remove(),this.newModelWindow=null),isEmpty(this.managerWindow)||isEmpty(this.tableView)||this.tableView.requery()}catch(e){let t=isEmpty(e)?"Couldn't communicate with server.":isEmpty(e.detail)?`${e}`:e.detail;this.notify("Error","Couldn't create model",t)}})),e.onCancel((()=>{this.newModelWindow.remove(),this.newModelWindow=null})),e}async showNewModel(){isEmpty(this.newModelWindow)?(this.newModelWindow=await this.spawnWindow("New Model",this.createModelForm(),this.constructor.modelWindowWidth,this.constructor.modelWindowHeight),this.newModelWindow.onClose((()=>{delete this.newModelWindow}))):this.newModelWindow.focus()}async showManager(){isEmpty(this.managerWindow)?(this.managerWindow=await this.spawnWindow("Model Manager",this.createManager(),this.constructor.managerWindowWidth,this.constructor.managerWindowHeight),this.managerWindow.onClose((()=>{delete this.managerWindow}))):this.managerWindow.focus()}async initialize(){LoraInputView.defaultOptions=async()=>this.model.get("/lora"),CheckpointInputView.defaultOptions=async()=>this.model.get("/checkpoints"),InversionInputView.defaultOptions=async()=>this.model.get("/inversions")}}export{ModelManagerController};
+import{Controller}from"../base.mjs";import{ParentView}from"../../view/base.mjs";import{FormView}from"../../view/forms/base.mjs";import{TableView,ModelTableView}from"../../view/table.mjs";import{StringInputView,TextInputView,FloatInputView,NumberInputView,FormInputView,RepeatableInputView,SearchListInputView,ButtonInputView}from"../../view/forms/input.mjs";import{isEmpty,deepClone}from"../../base/helpers.mjs";class InversionInputView extends SearchListInputView{}class LoraInputView extends SearchListInputView{}class CheckpointInputView extends SearchListInputView{}class LoraFormView extends FormView{static autoSubmit=!0;static fieldSets={LoRA:{model:{label:"Model",class:LoraInputView,config:{required:!0}},weight:{label:"Weight",class:FloatInputView,config:{min:0,value:1,step:.01,required:!0}}}}}class LoraFormInputView extends FormInputView{static formClass=LoraFormView}class MultiLoraInputView extends RepeatableInputView{static memberClass=LoraFormInputView}class MultiInversionInputView extends RepeatableInputView{static memberClass=InversionInputView}class ModelForm extends FormView{static canCancel=!0;static fieldSets={Name:{name:{class:StringInputView,label:"Name",config:{required:!0}}},Model:{checkpoint:{class:CheckpointInputView,label:"Checkpoint",config:{required:!0}},lora:{class:MultiLoraInputView,label:"LoRA"},inversion:{class:MultiInversionInputView,label:"Textual Inversions"}},Engine:{size:{class:NumberInputView,label:"Size",config:{required:!0,value:512,min:128,max:2048,step:8}}},Prompts:{prompt:{class:TextInputView,label:"Prompt"},negative_prompt:{class:TextInputView,label:"Negative Prompt"}}}}class NewModelInputView extends ButtonInputView{static defaultValue="New Model";static className="new-model-input-view"}class ModelManagerController extends Controller{static modelWindowWidth=400;static modelWindowHeight=1e3;static managerWindowWidth=800;static managerWindowHeight=600;async createManager(){this.tableView=new ModelTableView(this.config,this.model.DiffusionModel),this.buttonView=new NewModelInputView(this.config),this.tableView.setColumns({name:"Name",model:"Model",size:"Size",prompt:"Prompt",negative_prompt:"Negative Prompt"}),this.tableView.setFormatter("size",(e=>`${e}px`)),this.tableView.addButton("Edit","fa-solid fa-edit",(async e=>{let t=e.getAttributes();t.checkpoint=t.model,t.lora=isEmpty(e.lora)?[]:e.lora.map((e=>e.getAttributes())),t.inversion=isEmpty(e.inversion)?[]:e.inversion.map((e=>e.model));let i,o=new ModelForm(this.config,deepClone(t));o.onSubmit((async t=>{try{await this.model.put(`/models/${e.name}`,null,null,t),isEmpty(i)||i.remove(),this.tableView.requery()}catch(e){let t=isEmpty(e)?"Couldn't communicate with server.":isEmpty(e.detail)?`${e}`:e.detail;this.notify("error","Couldn't update model",t),o.enable()}})),o.onCancel((()=>i.remove())),i=await this.spawnWindow(`Edit ${e.name}`,o,this.constructor.modelWindowWidth,this.constructor.modelWindowHeight)})),this.tableView.addButton("Delete","fa-solid fa-trash",(async e=>{try{await this.model.delete(`/models/${e.name}`),this.tableView.requery()}catch(e){let t=isEmpty(e)?"Couldn't communicate with server.":isEmpty(e.detail)?`${e}`:e.detail;this.notify("error","Couldn't delete model",t),modelForm.enable()}})),this.buttonView.onChange((()=>{this.showNewModel()}));let e=new ParentView(this.config);return e.addChild(this.tableView),e.addChild(this.buttonView),e}async createModelForm(){let e=new ModelForm(this.config);return e.onSubmit((async e=>{try{await this.model.post("/models",null,null,e);isEmpty(this.newModelWindow)||(this.newModelWindow.remove(),this.newModelWindow=null),isEmpty(this.managerWindow)||isEmpty(this.tableView)||this.tableView.requery()}catch(e){let t=isEmpty(e)?"Couldn't communicate with server.":isEmpty(e.detail)?`${e}`:e.detail;this.notify("Error","Couldn't create model",t)}})),e.onCancel((()=>{this.newModelWindow.remove(),this.newModelWindow=null})),e}async showNewModel(){isEmpty(this.newModelWindow)?(this.newModelWindow=await this.spawnWindow("New Configuration",this.createModelForm(),this.constructor.modelWindowWidth,this.constructor.modelWindowHeight),this.newModelWindow.onClose((()=>{delete this.newModelWindow}))):this.newModelWindow.focus()}async showManager(){isEmpty(this.managerWindow)?(this.managerWindow=await this.spawnWindow("Model Configuration Manager",this.createManager(),this.constructor.managerWindowWidth,this.constructor.managerWindowHeight),this.managerWindow.onClose((()=>{delete this.managerWindow}))):this.managerWindow.focus()}async initialize(){LoraInputView.defaultOptions=async()=>this.model.get("/lora"),CheckpointInputView.defaultOptions=async()=>this.model.get("/checkpoints"),InversionInputView.defaultOptions=async()=>this.model.get("/inversions")}}export{ModelManagerController,MultiLoraInputView,MultiInversionInputView};
```

### Comparing `enfugue-0.1.2/enfugue/static/js/controller/file/02-open.mjs` & `enfugue-0.1.3/enfugue/static/js/controller/file/02-open.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/controller/file/03-save.mjs` & `enfugue-0.1.3/enfugue/static/js/controller/file/03-save.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/controller/file/04-history.mjs` & `enfugue-0.1.3/enfugue/static/js/controller/file/04-history.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/controller/file/05-results.mjs` & `enfugue-0.1.3/enfugue/static/js/controller/file/05-results.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/controller/help/01-about.mjs` & `enfugue-0.1.3/enfugue/static/js/controller/help/01-about.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/controller/index.mjs` & `enfugue-0.1.3/enfugue/static/js/controller/index.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/controller/models/01-civitait.mjs` & `enfugue-0.1.3/enfugue/static/js/controller/models/01-civitait.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/controller/sidebar/01-canvas.mjs` & `enfugue-0.1.3/enfugue/static/js/controller/sidebar/01-canvas.mjs`

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
-import{isEmpty}from"../../base/helpers.mjs";import{FormView}from"../../view/forms/base.mjs";import{NumberInputView}from"../../view/forms/input.mjs";import{Controller}from"../base.mjs";let defaultWidth=512,defaultHeight=512,defaultChunkingSize=64,defaultChunkingBlur=64;class CanvasForm extends FormView{static collapseFieldSets=!0;static autoSubmit=!0;static fieldSets={Dimensions:{width:{label:"Width",class:NumberInputView,config:{min:64,max:4096,value:defaultWidth,step:8,tooltip:"The width of the canvas in pixels."}},height:{label:"Height",class:NumberInputView,config:{min:64,max:4096,value:defaultHeight,step:8,tooltip:"The height of the canvas in pixels."}},chunkingSize:{label:"Chunk Size",class:NumberInputView,config:{min:0,value:defaultChunkingSize,step:8,tooltip:"<p>The number of pixels to move the frame when doing chunked diffusion.</p><p>When this number is greater than 0, the engine will only ever process a square in the size of the configured model size at once. After each square, the frame will be moved by this many pixels along either the horizontal or vertical axis, and then the image is re-diffused. When this number is 0, chunking is disabled, and the entire canvas will be diffused at once.</p><p>Disabling this (setting it to 0) can have varying visual results, but a guaranteed result is drastically increased VRAM usage for large images. A low number can produce more detailed results, but can be noisy, and takes longer to process. A high number is faster to process, but can have poor results especially along frame boundaries. The recommended value is set by default.</p>"}},chunkingBlur:{label:"Chunk Blur",class:NumberInputView,config:{min:0,value:defaultChunkingBlur,step:8,tooltip:"The number of pixels to feather along the edge of the frame when blending chunked diffusions together. Low numbers can produce less blurry but more noisy results, and can potentially result in visible breaks in the frame. High numbers can help blend frames, but produce blurrier results. The recommended value is set by default."}}}}}class CanvasController extends Controller{getState(){return{canvas:this.canvasForm.values}}getDefaultState(){return{canvas:{width:defaultWidth,height:defaultHeight,chunkingSize:defaultChunkingSize,chunkingBlur:defaultChunkingBlur}}}setState(e){isEmpty(e.canvas)||this.canvasForm.setValues(e.canvas).then((()=>this.canvasForm.submit()))}async initialize(){defaultWidth=this.application.config.model.invocation.width,defaultHeight=this.application.config.model.invocation.height,defaultChunkingSize=this.application.config.model.invocation.chunkingSize,defaultChunkingBlur=this.application.config.model.invocation.chunkingBlur,this.canvasForm=new CanvasForm(this.config),this.canvasForm.onSubmit((async e=>{this.images.width=e.width,this.images.height=e.height,this.engine.width=e.width,this.engine.height=e.height,this.engine.chunkingSize=e.chunkingSize})),this.application.sidebar.addChild(this.canvasForm),this.subscribe("modelPickerChange",(async e=>{let i=this.engine.width,t=this.engine.height,n=!1;if(i<e.size){let i=await this.canvasForm.getInputView("width");i.setValue(e.size),i.setMin(e.size),this.engine.width=e.size,this.images.width=e.size,n=!0}if(t<e.size){let i=await this.canvasForm.getInputView("height");i.setValue(e.size),i.setMin(e.size),this.engine.height=e.size,this.images.height=e.size,n=!0}n&&this.notify("info","Dimensions Changed","The base model specifies a size larger than the current canvas, it has been modified to match.")}))}}export{CanvasController as SidebarController};
+import{isEmpty}from"../../base/helpers.mjs";import{FormView}from"../../view/forms/base.mjs";import{NumberInputView}from"../../view/forms/input.mjs";import{Controller}from"../base.mjs";let defaultWidth=512,defaultHeight=512,defaultChunkingSize=64,defaultChunkingBlur=64;class CanvasForm extends FormView{static collapseFieldSets=!0;static autoSubmit=!0;static fieldSets={Dimensions:{width:{label:"Width",class:NumberInputView,config:{min:64,max:4096,value:defaultWidth,step:8,tooltip:"The width of the canvas in pixels."}},height:{label:"Height",class:NumberInputView,config:{min:64,max:4096,value:defaultHeight,step:8,tooltip:"The height of the canvas in pixels."}},chunkingSize:{label:"Chunk Size",class:NumberInputView,config:{min:0,value:defaultChunkingSize,step:8,tooltip:"<p>The number of pixels to move the frame when doing chunked diffusion.</p><p>When this number is greater than 0, the engine will only ever process a square in the size of the configured model size at once. After each square, the frame will be moved by this many pixels along either the horizontal or vertical axis, and then the image is re-diffused. When this number is 0, chunking is disabled, and the entire canvas will be diffused at once.</p><p>Disabling this (setting it to 0) can have varying visual results, but a guaranteed result is drastically increased VRAM usage for large images. A low number can produce more detailed results, but can be noisy, and takes longer to process. A high number is faster to process, but can have poor results especially along frame boundaries. The recommended value is set by default.</p>"}},chunkingBlur:{label:"Chunk Blur",class:NumberInputView,config:{min:0,value:defaultChunkingBlur,step:8,tooltip:"The number of pixels to feather along the edge of the frame when blending chunked diffusions together. Low numbers can produce less blurry but more noisy results, and can potentially result in visible breaks in the frame. High numbers can help blend frames, but produce blurrier results. The recommended value is set by default."}}}}}class CanvasController extends Controller{getState(){return{canvas:this.canvasForm.values}}getDefaultState(){return{canvas:{width:defaultWidth,height:defaultHeight,chunkingSize:defaultChunkingSize,chunkingBlur:defaultChunkingBlur}}}setState(e){isEmpty(e.canvas)||this.canvasForm.setValues(e.canvas).then((()=>this.canvasForm.submit()))}async initialize(){defaultWidth=this.application.config.model.invocation.width,defaultHeight=this.application.config.model.invocation.height,defaultChunkingSize=this.application.config.model.invocation.chunkingSize,defaultChunkingBlur=this.application.config.model.invocation.chunkingBlur,this.canvasForm=new CanvasForm(this.config),this.canvasForm.onSubmit((async e=>{this.images.width=e.width,this.images.height=e.height,this.engine.width=e.width,this.engine.height=e.height,this.engine.chunkingSize=e.chunkingSize})),this.application.sidebar.addChild(this.canvasForm),this.subscribe("modelPickerChange",(async e=>{let i=this.engine.width,t=this.engine.height,n=!1,s=await this.canvasForm.getInputView("width"),a=await this.canvasForm.getInputView("height");s.setMin(e.size),a.setMin(e.size),i<e.size&&(s.setValue(e.size),this.engine.width=e.size,this.images.width=e.size,n=!0),t<e.size&&(a.setValue(e.size),this.engine.height=e.size,this.images.height=e.size,n=!0),n&&this.notify("info","Dimensions Changed","The base model specifies a size larger than the current canvas, it has been modified to match.")}))}}export{CanvasController as SidebarController};
```

### Comparing `enfugue-0.1.2/enfugue/static/js/controller/sidebar/02-tweaks.mjs` & `enfugue-0.1.3/enfugue/static/js/controller/sidebar/02-tweaks.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/controller/sidebar/03-generation.mjs` & `enfugue-0.1.3/enfugue/static/js/controller/sidebar/03-generation.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/controller/sidebar/04-upscale.mjs` & `enfugue-0.1.3/enfugue/static/js/controller/sidebar/04-upscale.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/controller/sidebar/05-prompts.mjs` & `enfugue-0.1.3/enfugue/static/js/controller/sidebar/05-prompts.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/controller/sidebar/99-invoke.mjs` & `enfugue-0.1.3/enfugue/static/js/controller/sidebar/99-invoke.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/controller/system/01-settings.mjs` & `enfugue-0.1.3/enfugue/static/js/controller/system/01-settings.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/controller/system/02-users.mjs` & `enfugue-0.1.3/enfugue/static/js/controller/system/02-users.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/controller/system/03-installation.mjs` & `enfugue-0.1.3/enfugue/static/js/controller/system/03-installation.mjs`

 * *Files 3% similar despite different names*

```diff
@@ -1 +1 @@
-import{MenuController}from"../menu.mjs";import{ElementBuilder}from"../../base/builder.mjs";import{isEmpty,humanSize}from"../../base/helpers.mjs";import{View,ParentView}from"../../view/base.mjs";import{FormView}from"../../view/forms/base.mjs";import{TableView}from"../../view/table.mjs";import{FileInputView,ButtonInputView,StringInputView}from"../../view/forms/input.mjs";const E=new ElementBuilder;class ChangeDirectoryForm extends FormView{static showCancel=!0;static fieldSets={Directory:{directory:{class:StringInputView,config:{required:!0,placeholder:"C:\\Users\\MyUser\\..."}}}}}class UploadFileFormView extends FormView{static showCancel=!0;static fieldSets={File:{file:{class:FileInputView,config:{required:!0}}}}}class UploadFileButtonInputView extends ButtonInputView{static className="upload-file-input-view";static defaultValue="Upload File"}class InstallationDirectorySummaryTableView extends TableView{static columns={directory:"Directory",location:"Location",items:"Items",bytes:"Total File Size"};static columnFormatters={bytes:t=>humanSize(t)}}class InstallationDirectoryTableView extends TableView{static columns={name:"Name",bytes:"Total File Size"};static columnFormatters={bytes:t=>humanSize(t)}}class TensorRTEngineTableView extends TableView{static columns={model:"Model",type:"Type",size:"Size",lora:"LoRA",inversion:"Inversions",bytes:"File Size",used_by:"Used By"};static columnFormatters={type:(t,e)=>{let i="";return e.model.endsWith("-inpainting")&&(i="Inpainting "),`${i}${{unet:"UNet",controlledunet:"Controlled UNet",clip:"CLIP",vae:"VAE",controlnet:"ControlNet"}[t]}`},size:t=>`${t}px`,bytes:t=>humanSize(t),lora:t=>isEmpty(t)?"None":t.map((t=>t.join(":"))).join("<br />"),inversion:t=>isEmpty(t)?"None":t.map((t=>t.model)).join("<br />"),used_by:t=>isEmpty(t)?"None":t.length<=2?t.join("<br />"):t.slice(0,2).join("<br />")+`<br />…and ${t.length-2} more`}}class TensorRTEngineSummaryTableView extends TableView{static columns={total:"Total Engines",used:"Currently Used",bytes:"Total File Size"};static columnFormatters={total:t=>isEmpty(t)?"None":`${t}`,used:t=>isEmpty(t)?"None":`${t}`,bytes:t=>isEmpty(t)?"0 Bytes":humanSize(t)}}class InstallationSummaryView extends View{constructor(t){super(t.config),this.controller=t,this.summaryTable=new InstallationDirectorySummaryTableView(this.config),this.summaryTable.addButton("Manage","fa-solid fa-list-check",(t=>{this.controller.showDirectoryManager(t.directory)})),this.summaryTable.addButton("Change Directory","fa-solid fa-edit",(t=>{this.controller.showChangeDirectory(t.directory)})),this.engineTable=new TensorRTEngineSummaryTableView(this.config),this.engineTable.addButton("Manage","fa-solid fa-list-check",(()=>{this.controller.showTensorRTManager()}))}async update(){let t=await this.controller.model.get("/installation"),e=await this.controller.model.get("/tensorrt");await this.summaryTable.setData(Object.getOwnPropertyNames(t).map((e=>(console.log(e),{directory:e,location:t[e].path,items:t[e].items,bytes:t[e].bytes}))),!1),await this.engineTable.setData([e.reduce(((t,e)=>(void 0===t.total&&(t.total=0),void 0===t.used&&(t.used=0),void 0===t.bytes&&(t.bytes=0),t.total+=1,t.used+=e.used,t.bytes+=e.bytes,t)),{})],!1)}async build(){let t=await super.build();return await this.update(),t.content(E.h2().content("Weights and Configuration"),await this.summaryTable.getNode(),E.h2().content("TensorRT Engines"),await this.engineTable.getNode())}}class InstallationController extends MenuController{static menuName="Installation";static menuIcon="fa-solid fa-folder-tree";static summaryWindowWidth=600;static summaryWindowHeight=600;static managerWindowWidth=600;static managerWindowHeight=800;static uploadWindowWidth=400;static uploadWindowHeight=250;static changeDirectoryWindowWidth=400;static changeDirectoryWindowHeight=200;static uploadableDirectories=["lora","checkpoint","inversion"];async initialize(){await super.initialize(),this.directoryWindows={}}async showSummaryWindow(){isEmpty(this.summaryWindow)?(this.summaryWindow=await this.spawnWindow("Installation Summary",await this.getSummaryView(),this.constructor.summaryWindowWidth,this.constructor.summaryWindowHeight),this.summaryWindow.onClose((()=>{this.summaryWindow=null}))):this.summaryWindow.focus()}async getSummaryView(){return isEmpty(this.summaryView)?this.summaryView=new InstallationSummaryView(this):this.summaryView.update(),this.summaryView}async showTensorRTManager(){let t=await this.model.get("/tensorrt");if(isEmpty(this.tensorRTManagerWindow)){let e=new TensorRTEngineTableView(this.config,t);e.addButton("Delete","fa-solid fa-trash",(async t=>{let i=`/tensorrt/${t.model}/${t.type}/${t.key}`;try{await this.model.delete(i),this.notify("info","Success","TensorRT engine deleted."),e.setData(await this.model.get("/tensorrt"),!1),isEmpty(this.summaryView)||this.summaryView.update()}catch(t){let e=`${t}`;isEmpty(t.detail)?isEmpty(t.title)||(e=t.title):e=t.detail,this.notify("error","Couldn't Delete",e)}})),this.tensorRTManagerWindow=await this.spawnWindow("TensorRT Engines",e,this.constructor.managerWindowWidth,this.constructor.managerWindowHeight),this.tensorRTManagerWindow.onClose((()=>{this.tensorRTManagerWindow=null}))}else this.tensorRTManagerWindow.content.setData(t,!1),this.tensorRTManagerWindow.focus()}async showUploadFile(t){let e=new UploadFileFormView(this.config),i=await this.spawnWindow(`Upload File to '${t}'`,e,this.constructor.uploadWindowWidth,this.constructor.uploadWindowHeight);e.onSubmit((async s=>{await this.model.multiPart(`/installation/${t}`,null,null,{file:s.file},(async t=>{(await e.getInputView("file")).setProgress(t.loaded/t.total)})),this.notify("info","Uploaded",`File successfully uploaded to '${t}'`),isEmpty(this.summaryView)||this.summaryView.update(),isEmpty(this.directoryWindows[t])||this.directoryWindows[t].content.getChild(0).setData(await this.model.get(`/installation/${t}`),!1),i.remove()})),e.onCancel((()=>{i.remove()}))}async showChangeDirectory(t){let e=new ChangeDirectoryForm(this.config),i=await this.spawnWindow(`Change Filesystem Location for ${t}`,e,this.constructor.changeDirectoryWindowWidth,this.constructor.changeDirectoryWindowHeight);e.onSubmit((async s=>{try{await this.model.post(`/installation/${t}/move`,null,null,{directory:s.directory}),this.notify("info","Changed",`Filesystem Location successfully changed for ${t}`),isEmpty(this.summaryView)||this.summaryView.update(),isEmpty(this.directoryWindows[t])||this.directoryWindows[t].content.getChild(0).setData(await this.model.get(`/installation/${t}`),!1),i.remove()}catch(t){let i=`${t}`;isEmpty(t.detail)?isEmpty(t.title)||(i=t.title):i=t.detail,this.notify("error","Couldn't Change",i),e.enable()}})),e.onCancel((()=>{i.remove()}))}async showDirectoryManager(t){let e=await this.model.get(`/installation/${t}`);if(isEmpty(this.directoryWindows[t])){let i=new InstallationDirectoryTableView(this.config,e);i.addButton("Delete","fa-solid fa-trash",(async e=>{let s=`/installation/${t}/${e.name}`;try{await this.model.delete(s),this.notify("info","Success",`Successfully deleted <strong>${t}/${e.name}</strong>`),i.setData(await this.model.get(`/installation/${t}`),!1),isEmpty(this.summaryView)||this.summaryView.update()}catch(t){let e=`${t}`;isEmpty(t.detail)?isEmpty(t.title)||(e=t.title):e=t.detail,this.notify("error","Couldn't Delete",e)}}));let s=new ParentView(this.config);if(s.addChild(i),-1!==this.constructor.uploadableDirectories.indexOf(t)){let e=new UploadFileButtonInputView(this.config);e.onChange((()=>{this.showUploadFile(t)})),s.addChild(e)}this.directoryWindows[t]=await this.spawnWindow(`Manage Directory '${t}'`,s,this.constructor.managerWindowWidth,this.constructor.managerWindowHeight),this.directoryWindows[t].onClose((()=>{this.directoryWindows[t]=null}))}else this.directoryWindows[t].content.getChild(0).setData(e),this.directoryWindows[t].focus()}async onClick(){this.showSummaryWindow()}}export{InstallationController as MenuController};
+import{MenuController}from"../menu.mjs";import{ElementBuilder}from"../../base/builder.mjs";import{isEmpty,humanSize}from"../../base/helpers.mjs";import{View,ParentView}from"../../view/base.mjs";import{FormView}from"../../view/forms/base.mjs";import{TableView}from"../../view/table.mjs";import{FileInputView,ButtonInputView,StringInputView}from"../../view/forms/input.mjs";const E=new ElementBuilder;class ChangeDirectoryForm extends FormView{static showCancel=!0;static fieldSets={Directory:{directory:{class:StringInputView,config:{required:!0,placeholder:"C:\\Users\\MyUser\\..."}}}}}class UploadFileFormView extends FormView{static showCancel=!0;static fieldSets={File:{file:{class:FileInputView,config:{required:!0}}}}}class UploadFileButtonInputView extends ButtonInputView{static className="upload-file-input-view";static defaultValue="Upload File"}class InstallationDirectorySummaryTableView extends TableView{static className="installation-directory-summary-table-view";static columns={location:"Location",directory:"Directory",items:"Items",bytes:"Total File Size"};static columnFormatters={bytes:t=>humanSize(t)}}class InstallationDirectoryTableView extends TableView{static className="installation-directory-table-view";static columns={name:"Name",bytes:"Total File Size"};static columnFormatters={bytes:t=>humanSize(t)}}class TensorRTEngineTableView extends TableView{static columns={model:"Model",type:"Type",size:"Size",lora:"LoRA",inversion:"Inversions",bytes:"File Size",used_by:"Used By"};static columnFormatters={type:(t,e)=>{let i="";return e.model.endsWith("-inpainting")&&(i="Inpainting "),`${i}${{unet:"UNet",controlledunet:"Controlled UNet",clip:"CLIP",vae:"VAE",controlnet:"ControlNet"}[t]}`},size:t=>`${t}px`,bytes:t=>humanSize(t),lora:t=>isEmpty(t)?"None":t.map((t=>t.join(":"))).join("<br />"),inversion:t=>isEmpty(t)?"None":t.map((t=>t.model)).join("<br />"),used_by:t=>isEmpty(t)?"None":t.length<=2?t.join("<br />"):t.slice(0,2).join("<br />")+`<br />…and ${t.length-2} more`}}class TensorRTEngineSummaryTableView extends TableView{static columns={total:"Total Engines",used:"Currently Used",bytes:"Total File Size"};static columnFormatters={total:t=>isEmpty(t)?"None":`${t}`,used:t=>isEmpty(t)?"None":`${t}`,bytes:t=>isEmpty(t)?"0 Bytes":humanSize(t)}}class InstallationSummaryView extends View{constructor(t){super(t.config),this.controller=t,this.summaryTable=new InstallationDirectorySummaryTableView(this.config),this.summaryTable.addButton("Manage","fa-solid fa-list-check",(t=>{this.controller.showDirectoryManager(t.directory)})),this.summaryTable.addButton("Change Directory","fa-solid fa-edit",(t=>{this.controller.showChangeDirectory(t.directory,t.location)})),this.engineTable=new TensorRTEngineSummaryTableView(this.config),this.engineTable.addButton("Manage","fa-solid fa-list-check",(()=>{this.controller.showTensorRTManager()}))}async update(){let t=await this.controller.model.get("/installation"),e=await this.controller.model.get("/tensorrt");await this.summaryTable.setData(Object.getOwnPropertyNames(t).map((e=>(console.log(e),{directory:e,location:t[e].path,items:t[e].items,bytes:t[e].bytes}))),!1),await this.engineTable.setData([e.reduce(((t,e)=>(void 0===t.total&&(t.total=0),void 0===t.used&&(t.used=0),void 0===t.bytes&&(t.bytes=0),t.total+=1,t.used+=e.used,t.bytes+=e.bytes,t)),{})],!1)}async build(){let t=await super.build();return await this.update(),t.content(E.h2().content("Weights and Configuration"),await this.summaryTable.getNode(),E.h2().content("TensorRT Engines"),await this.engineTable.getNode())}}class InstallationController extends MenuController{static menuName="Installation";static menuIcon="fa-solid fa-folder-tree";static summaryWindowWidth=600;static summaryWindowHeight=600;static managerWindowWidth=600;static managerWindowHeight=800;static uploadWindowWidth=400;static uploadWindowHeight=250;static changeDirectoryWindowWidth=400;static changeDirectoryWindowHeight=200;static uploadableDirectories=["lora","checkpoint","inversion"];async initialize(){await super.initialize(),this.directoryWindows={}}async showSummaryWindow(){isEmpty(this.summaryWindow)?(this.summaryWindow=await this.spawnWindow("Installation Summary",await this.getSummaryView(),this.constructor.summaryWindowWidth,this.constructor.summaryWindowHeight),this.summaryWindow.onClose((()=>{this.summaryWindow=null}))):this.summaryWindow.focus()}async getSummaryView(){return isEmpty(this.summaryView)?this.summaryView=new InstallationSummaryView(this):this.summaryView.update(),this.summaryView}async showTensorRTManager(){let t=await this.model.get("/tensorrt");if(isEmpty(this.tensorRTManagerWindow)){let e=new TensorRTEngineTableView(this.config,t);e.addButton("Delete","fa-solid fa-trash",(async t=>{let i=`/tensorrt/${t.model}/${t.type}/${t.key}`;try{await this.model.delete(i),this.notify("info","Success","TensorRT engine deleted."),e.setData(await this.model.get("/tensorrt"),!1),isEmpty(this.summaryView)||this.summaryView.update()}catch(t){let e=`${t}`;isEmpty(t.detail)?isEmpty(t.title)||(e=t.title):e=t.detail,this.notify("error","Couldn't Delete",e)}})),this.tensorRTManagerWindow=await this.spawnWindow("TensorRT Engines",e,this.constructor.managerWindowWidth,this.constructor.managerWindowHeight),this.tensorRTManagerWindow.onClose((()=>{this.tensorRTManagerWindow=null}))}else this.tensorRTManagerWindow.content.setData(t,!1),this.tensorRTManagerWindow.focus()}async showUploadFile(t){let e=new UploadFileFormView(this.config),i=await this.spawnWindow(`Upload File to '${t}'`,e,this.constructor.uploadWindowWidth,this.constructor.uploadWindowHeight);e.onSubmit((async s=>{await this.model.multiPart(`/installation/${t}`,null,null,{file:s.file},(async t=>{(await e.getInputView("file")).setProgress(t.loaded/t.total)})),this.notify("info","Uploaded",`File successfully uploaded to '${t}'`),isEmpty(this.summaryView)||this.summaryView.update(),isEmpty(this.directoryWindows[t])||this.directoryWindows[t].content.getChild(0).setData(await this.model.get(`/installation/${t}`),!1),i.remove()})),e.onCancel((()=>{i.remove()}))}async showChangeDirectory(t,e){let i=new ChangeDirectoryForm(this.config,{directory:e}),s=await this.spawnWindow(`Change Filesystem Location for ${t}`,i,this.constructor.changeDirectoryWindowWidth,this.constructor.changeDirectoryWindowHeight);i.onSubmit((async e=>{try{await this.model.post(`/installation/${t}/move`,null,null,{directory:e.directory}),this.notify("info","Changed",`Filesystem Location successfully changed for ${t}`),isEmpty(this.summaryView)||this.summaryView.update(),isEmpty(this.directoryWindows[t])||this.directoryWindows[t].content.getChild(0).setData(await this.model.get(`/installation/${t}`),!1),s.remove()}catch(t){let e=`${t}`;isEmpty(t.detail)?isEmpty(t.title)||(e=t.title):e=t.detail,this.notify("error","Couldn't Change",e),i.enable()}})),i.onCancel((()=>{s.remove()}))}async showDirectoryManager(t){let e=await this.model.get(`/installation/${t}`);if(isEmpty(this.directoryWindows[t])){let i=new InstallationDirectoryTableView(this.config,e);i.addButton("Delete","fa-solid fa-trash",(async e=>{let s=`/installation/${t}/${e.name}`;try{await this.model.delete(s),this.notify("info","Success",`Successfully deleted <strong>${t}/${e.name}</strong>`),i.setData(await this.model.get(`/installation/${t}`),!1),isEmpty(this.summaryView)||this.summaryView.update()}catch(t){let e=`${t}`;isEmpty(t.detail)?isEmpty(t.title)||(e=t.title):e=t.detail,this.notify("error","Couldn't Delete",e)}}));let s=new ParentView(this.config);if(s.addClass("installation-summary-view"),s.addChild(i),-1!==this.constructor.uploadableDirectories.indexOf(t)){let e=new UploadFileButtonInputView(this.config);e.onChange((()=>{this.showUploadFile(t)})),s.addChild(e)}this.directoryWindows[t]=await this.spawnWindow(`Manage Directory '${t}'`,s,this.constructor.managerWindowWidth,this.constructor.managerWindowHeight),this.directoryWindows[t].onClose((()=>{this.directoryWindows[t]=null}))}else this.directoryWindows[t].content.getChild(0).setData(e),this.directoryWindows[t].focus()}async onClick(){this.showSummaryWindow()}}export{InstallationController as MenuController};
```

### Comparing `enfugue-0.1.2/enfugue/static/js/controller/system/04-logs.mjs` & `enfugue-0.1.3/enfugue/static/js/controller/system/04-logs.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/enfugue.mjs` & `enfugue-0.1.3/enfugue/static/js/enfugue.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/graphics/colors.mjs` & `enfugue-0.1.3/enfugue/static/js/graphics/colors.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/graphics/geometry.mjs` & `enfugue-0.1.3/enfugue/static/js/graphics/geometry.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/graphics/paths.mjs` & `enfugue-0.1.3/enfugue/static/js/graphics/paths.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/graphics/spline.mjs` & `enfugue-0.1.3/enfugue/static/js/graphics/spline.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/model/enfugue.mjs` & `enfugue-0.1.3/enfugue/static/js/model/enfugue.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/model/index.mjs` & `enfugue-0.1.3/enfugue/static/js/model/index.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/view/base.mjs` & `enfugue-0.1.3/enfugue/static/js/view/base.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/view/forms/base.mjs` & `enfugue-0.1.3/enfugue/static/js/view/forms/base.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/view/forms/classic.mjs` & `enfugue-0.1.3/enfugue/static/js/view/forms/classic.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/view/forms/input/base.mjs` & `enfugue-0.1.3/enfugue/static/js/view/forms/input/base.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/view/forms/input/color.mjs` & `enfugue-0.1.3/enfugue/static/js/view/forms/input/color.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/view/forms/input/enumerable.mjs` & `enfugue-0.1.3/enfugue/static/js/view/forms/input/enumerable.mjs`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-import{isEmpty,jaroWinkler,strip}from"../../../base/helpers.mjs";import{ElementBuilder}from"../../../base/builder.mjs";import{InputView}from"./base.mjs";import{StringInputView}from"./string.mjs";const E=new ElementBuilder({searchList:"enfugue-search-list",searchListItem:"enfugue-search-list-item",searchSelection:"enfugue-search-list-selection",repeatableInput:"enfugue-repeatable-input",repeatableItem:"enfugue-repeatable-input-item"});class EnumerableInputView extends InputView{static defaultOptions={};constructor(t,e,s){super(t,e,s),this.options=this.fieldConfig.options||{},this.sortFunction=this.fieldConfig.sortFunction||((t,e)=>t-e),this.filterFunction=this.fieldConfig.filterFunction||((t,e)=>!1)}setOptions(t){Array.isArray(t)?this.options=t.reduce(((t,e)=>(t[e]=e,t)),{}):this.options=t,void 0!==this.node&&this.rebuildOptions()}async sortOptions(t){this.sortFunction=t,void 0!==this.node&&await this.rebuildOptions()}async filterOptions(t){this.filterFunction=t,void 0!==this.node&&await this.rebuildOptions()}async sortFilterOptions(t,e){this.sortFunction=t,this.filterFunction=e,void 0!==this.node&&await this.rebuildOptions()}async getOptions(){let t=this.options,e=this.constructor.defaultOptions;"function"==typeof t&&(t=await this.options()),Array.isArray(t)&&(t=t.reduce(((t,e)=>(t[e]=e,t)),{})),"function"==typeof e&&(e=await e()),Array.isArray(e)&&(e=e.reduce(((t,e)=>(t[e]=e,t)),{}));let s={...e,...t},i=Object.getOwnPropertyNames(s),a={};i.sort(((t,e)=>this.sortFunction(t,e,s[t],s[e])));for(let t of i)this.filterFunction(t,s[t])||(a[t]=s[t]);return a}buildOptions(t,e){}async rebuildOptions(){void 0!==this.node&&this.buildOptions(this.node,await this.getOptions())}async build(){let t=await super.build();return this.buildOptions(t,await this.getOptions()),t}}class SelectInputView extends EnumerableInputView{static tagName="select";static alwaysShowEmpty=!1;static allowEmpty=!1;async buildOptions(t,e){let s=this.placeholder;isEmpty(s)&&(s="Select One");let i=[];(isEmpty(this.value)||this.constructor.alwaysShowEmpty||this.constructor.allowEmpty)&&i.push(E.option().selected(!0).disabled(!this.constructor.allowEmpty).value("").content(s));for(let t in e){let s=E.option().value(t).content(e[t]);this.value==t&&s.selected(!0),i.push(s)}return t.content(...i)}setValue(t,e){if(void 0!==this.node){this.node.value(t);for(let t of this.node.findAll("option"))t.value()==this.value?t.selected(!0):t.selected(!1)}super.setValue(t,e)}async build(){let t=await super.build();return isEmpty(this.value)||t.value(this.value),t}}class ListInputView extends EnumerableInputView{static tagName="ul";static className="list-input-view";static maximumOptions=1/0;getValue(){return this.value}setValue(t,e){if(super.setValue(t,e),void 0!==this.node)for(let t of this.node.findAll("li"))t.data("value")===this.value?t.addClass("selected"):t.removeClass("selected")}buildOptions(t,e){let s=0,i=[];for(let a in e){let n=E.span().content(e[a]),l=E.li().content(n).data("value",a);if(l.on("click",(e=>{e.stopPropagation(),e.preventDefault();for(let e of t.children())e.removeClass("selected");l.addClass("selected"),this.value=a,this.changed()})),this.value===a&&l.addClass("selected"),i.push(l),s++,s>=this.constructor.maximumOptions)break}return t.content(...i)}}class ListMultiInputView extends ListInputView{static maximumSelected=1/0;static className="list-input-view multi-list-input-view";constructor(t,e,s){super(t,e,s),isEmpty(this.value)&&(this.value=[])}setValue(t,e){if(super.setValue(t,e),isEmpty(this.value)?this.value=[]:Array.isArray(this.value)||(this.value=[this.value]),void 0!==this.node)for(let t of this.node.findAll("li"))-1!==this.value.indexOf(t.data("value"))?t.addClass("selected"):t.removeClass("selected")}buildOptions(t,e){let s=0,i=[];for(let t in e){let a=E.li().content(E.span().content(e[t])).data("value",t);if(a.on("click",(e=>{e.stopPropagation(),e.preventDefault(),a.hasClass("selected")?(this.value=this.value.filter((e=>e!==t)),a.removeClass("selected")):(isEmpty(this.value)&&(this.value=[]),this.value.push(t),a.addClass("selected")),this.changed()})),isEmpty(this.value)&&-1!==this.value.indexOf(t)&&a.addClass("selected"),i.push(a),s++,s>=this.constructor.maximumOptions)break}return t.content(...i)}}class SearchListInputListView extends ListInputView{static maximumOptions=100;static classList=["enfugue-search-list-items"];async build(){let t=await super.build();return t.on("mousewheel",(t=>{t.stopPropagation()})),t}}class SearchListMultiInputListView extends ListMultiInputView{static maximumOptions=100;static classList=["enfugue-search-list-items","enfugue-multi-search-list-items"];async build(){let t=await super.build();return t.on("mousewheel,mouseup",(t=>{t.stopPropagation()})),t}}class SearchListInputView extends EnumerableInputView{static tagName="enfugue-search-list";static placeholder="Start typing to search…";static searchTimeout=250;static filterThreshold=.9;static listInputClass=SearchListInputListView;static stringInputClass=StringInputView;static setClosestOnBlur=!0;static resetListOnFocus=!0;static hideListOnBlur=!0;static hideListOnChange=!0;static populateSearchOnSet=!0;static debounceChangeThreshold=150;constructor(t,e,s){super(t,e,s),this.stringInput=new this.constructor.stringInputClass(t,"autofill",{placeholder:this.constructor.placeholder}),this.stringInput.onInput((t=>this.searchChanged(t))),this.stringInput.onFocus((async()=>{await this.stringInput.getNode();let t=await this.listInput.getNode(),e=this.node.element.getBoundingClientRect(),s=e.x,i=e.y+e.height,a=e.width,n=(e,n,l)=>{s=e,i=n,a=l,t.css({width:`${l}px`,left:`${e}px`,top:`${n}px`})};this.repositionInterval=setInterval((()=>{e=this.node.element.getBoundingClientRect();let t=e.x,l=e.y+e.height,o=e.width;s===t&&i===l&&a===o||n(t,l,o)}),25),document.body.appendChild(t.render()),n(s,i,a),t.css({width:`${e.width}px`,left:`${e.x}px`,top:`${e.y+e.height}px`}),this.listInput.show(),this.constructor.resetListOnFocus&&this.listInput.setValue(null,!1);let l=t=>{this.listInput.hide(),window.removeEventListener("click",l,!1),clearTimeout(this.searchDebounceTimer),clearInterval(this.repositionInterval)};window.addEventListener("click",l,!1)})),this.stringInput.onBlur((async t=>{if(this.constructor.hideListOnBlur){let t=e=>{setTimeout((async()=>{this.listInput.hide(),document.body.removeChild((await this.listInput.getNode()).element)}),100),window.removeEventListener("mouseup",t,!0)};window.addEventListener("mouseup",t,!0),clearTimeout(this.searchDebounceTimer),clearInterval(this.repositionInterval)}if(this.constructor.setClosestOnBlur){let t=strip(this.stringInput.getValue()).toLowerCase();if(isEmpty(t))this.value=null;else{let e=await this.getOptions(),s=Object.getOwnPropertyNames(e);s.sort(((s,i)=>jaroWinkler(e[i].toLowerCase(),t)-jaroWinkler(e[s].toLowerCase(),t))),this.value=s[0],this.stringInput.setValue(e[this.value],!1)}}})),this.listInput=new this.constructor.listInputClass(t,"list",{options:()=>this.getOptions()}),this.listInput.onChange((async()=>{let t=await this.getOptions(),e=this.listInput.getValue();this.value=e,this.constructor.populateSearchOnSet&&this.stringInput.setValue(t[e]),this.constructor.hideListOnChange&&(clearTimeout(this.searchDebounceTimer),clearInterval(this.repositionInterval)),this.changed()})),this.listInput.hide()}disable(){if(clearTimeout(this.searchDebounceTimer),this.stringInput.disable(),this.listInput.disable(),void 0!==this.node)for(let t of this.node.findAll(E.getCustomTag("searchSelection")))t.find("button").disabled(!0)}enable(){if(this.stringInput.enable(),this.listInput.enable(),void 0!==this.node)for(let t of this.node.findAll(E.getCustomTag("searchSelection")))t.find("button").disabled(!1)}setOptions(t){super.setOptions(t),this.listInput.setValue([],!1),this.listInput.setOptions(t)}rebuildOptions(){}buildOptions(){}getValue(){return this.value}setValue(t,e){super.setValue(t,!1);void 0!==this.stringInput&&this.stringInput.setValue(t,!1),e&&this.changed()}searchChanged(t){clearTimeout(this.searchDebounceTimer),this.searchDebounceTimer=setTimeout((()=>{this.search(t)}),this.constructor.searchTimeout)}async search(t){t=strip(t.toLowerCase()),isEmpty(t)?await this.listInput.sortFilterOptions(((t,e)=>t-e),((t,e)=>!1)):await this.listInput.sortFilterOptions(((e,s,i,a)=>jaroWinkler(a.toLowerCase(),t)-jaroWinkler(i.toLowerCase(),t)),((e,s)=>1-jaroWinkler(s.toLowerCase(),t)>=this.constructor.filterThreshold))}async build(){let t=await super.build();return t.append(await this.stringInput.getNode()),t.on("dragover",(e=>{e.preventDefault(),e.stopPropagation();let s=e.target,i=t.findAll(E.getCustomTag("searchSelection")),a=e.offsetX;for(let t of i)t.removeClass("drop-left").removeClass("drop-right");for(;-1===["ENFUGUE-SEARCH-LIST-SELECTION","ENFUGUE-SEARCH-LIST"].indexOf(s.tagName);)a+=s.offsetLeft,s=s.parentElement;if("ENFUGUE-SEARCH-LIST-SELECTION"==s.tagName&&!s.classList.contains("dragged")){let t=s.dataset.selectValue,e=i.filter((e=>e.data("select-value")===t)).shift();a>s.offsetWidth/2?e.addClass("drop-right"):e.addClass("drop-left")}})).on("drop",(e=>{let s=e.target,i=e.dataTransfer.getData("text/plain"),a=e.offsetX,n=t.findAll(E.getCustomTag("searchSelection"));for(let t of n)t.removeClass("drop-left").removeClass("drop-right");for(;-1===["ENFUGUE-SEARCH-LIST-SELECTION","ENFUGUE-SEARCH-LIST"].indexOf(s.tagName);)a+=s.offsetLeft,s=s.parentElement;if("ENFUGUE-SEARCH-LIST-SELECTION"==s.tagName){let e=s.dataset.selectValue;if(i!==e){let l=n.filter((t=>t.data("select-value")===i)).shift(),o=n.filter((t=>t.data("select-value")===e)).shift(),r=this.value.indexOf(i),u=this.value.indexOf(e),h=(l.find("span").getText(),o.find("span").getText(),a>s.offsetWidth/2);t.remove(l),this.value=this.value.filter((t=>t!=i)),!h&&r<u?u--:h&&r>u&&u++,this.value=this.value.slice(0,u).concat([i]).concat(this.value.slice(u)),this.listInput.setValue(this.value,!1),t.insert(u,l),this.changed()}}})),t}async changed(){let t=(new Date).getTime();void 0!==this.lastChange&&t-this.lastChange<this.constructor.debounceChangeThreshold||(await super.changed(),this.lastChange=t)}}class SearchListMultiInputView extends SearchListInputView{static setClosestOnBlur=!1;static resetListOnFocus=!1;static hideListOnBlur=!1;static populateSearchOnSet=!1;static hideListOnChange=!1;static listInputClass=SearchListMultiInputListView;constructor(t,e,s){super(t,e,s),this.onChange((async()=>{let t=this.getValue(),e=await this.getOptions();isEmpty(t)&&(t=[]),void 0!==this.node&&this.node.content(...t.map((t=>{let s=E.searchSelection().data("select-value",t),i=E.button().content("&times;"),a=E.span().content(e[t]);return i.on("click",(t=>{t.preventDefault(),t.stopPropagation(),this.value=this.value.filter((t=>t!==s.data("select-value"))),this.listInput.setValue(this.value,!1),this.changed()})),s.attr("draggable","true").on("dragstart",(e=>{s.addClass("dragged");let i=e.dataTransfer;i.dropEffect="move",i.effectAllowed="move",i.setData("text/plain",t)})).on("dragend",(t=>{s.removeClass("dragged")})),s.content(i,a)})),await this.stringInput.getNode())}))}async build(){let t=await super.build();return t.append(await this.stringInput.getNode()),t}}export{EnumerableInputView,SelectInputView,ListInputView,ListMultiInputView,SearchListInputView,SearchListMultiInputView};
+import{isEmpty,jaroWinkler,strip}from"../../../base/helpers.mjs";import{ElementBuilder}from"../../../base/builder.mjs";import{InputView}from"./base.mjs";import{StringInputView}from"./string.mjs";const E=new ElementBuilder({searchList:"enfugue-search-list",searchListItem:"enfugue-search-list-item",searchSelection:"enfugue-search-list-selection",repeatableInput:"enfugue-repeatable-input",repeatableItem:"enfugue-repeatable-input-item"});class EnumerableInputView extends InputView{static defaultOptions={};constructor(t,e,s){super(t,e,s),this.options=this.fieldConfig.options||{},this.sortFunction=this.fieldConfig.sortFunction||((t,e)=>t-e),this.filterFunction=this.fieldConfig.filterFunction||((t,e)=>!1)}setOptions(t){Array.isArray(t)?this.options=t.reduce(((t,e)=>(t[e]=e,t)),{}):this.options=t,void 0!==this.node&&this.rebuildOptions()}async sortOptions(t){this.sortFunction=t,void 0!==this.node&&await this.rebuildOptions()}async filterOptions(t){this.filterFunction=t,void 0!==this.node&&await this.rebuildOptions()}async sortFilterOptions(t,e){this.sortFunction=t,this.filterFunction=e,void 0!==this.node&&await this.rebuildOptions()}async getOptions(){let t=this.options,e=this.constructor.defaultOptions;"function"==typeof t&&(t=await this.options()),Array.isArray(t)&&(t=t.reduce(((t,e)=>(t[e]=e,t)),{})),"function"==typeof e&&(e=await e()),Array.isArray(e)&&(e=e.reduce(((t,e)=>(t[e]=e,t)),{}));let s={...e,...t},i=Object.getOwnPropertyNames(s),a={};i.sort(((t,e)=>this.sortFunction(t,e,s[t],s[e])));for(let t of i)this.filterFunction(t,s[t])||(a[t]=s[t]);return a}buildOptions(t,e){}async rebuildOptions(){void 0!==this.node&&this.buildOptions(this.node,await this.getOptions())}async build(){let t=await super.build();return this.buildOptions(t,await this.getOptions()),t}}class SelectInputView extends EnumerableInputView{static tagName="select";static alwaysShowEmpty=!1;static allowEmpty=!1;async buildOptions(t,e){let s=this.placeholder;isEmpty(s)&&(s="Select One");let i=[];(isEmpty(this.value)||this.constructor.alwaysShowEmpty||this.constructor.allowEmpty)&&i.push(E.option().selected(!0).disabled(!this.constructor.allowEmpty).value("").content(s));for(let t in e){let s=E.option().value(t).content(e[t]);this.value==t&&s.selected(!0),i.push(s)}return t.content(...i)}setValue(t,e){if(void 0!==this.node){this.node.value(t);for(let t of this.node.findAll("option"))t.value()==this.value?t.selected(!0):t.selected(!1)}super.setValue(t,e)}async build(){let t=await super.build();return isEmpty(this.value)||t.value(this.value),t}}class ListInputView extends EnumerableInputView{static tagName="ul";static className="list-input-view";static maximumOptions=1/0;getValue(){return this.value}setValue(t,e){if(super.setValue(t,e),void 0!==this.node)for(let t of this.node.findAll("li"))t.data("value")===this.value?t.addClass("selected"):t.removeClass("selected")}buildOptions(t,e){let s=0,i=[];for(let a in e){let n=E.span().content(e[a]),l=E.li().content(n).data("value",a);if(l.on("click",(e=>{e.stopPropagation(),e.preventDefault();for(let e of t.children())e.removeClass("selected");l.addClass("selected"),this.value=a,this.changed()})),this.value===a&&l.addClass("selected"),i.push(l),s++,s>=this.constructor.maximumOptions)break}return t.content(...i)}}class ListMultiInputView extends ListInputView{static maximumSelected=1/0;static className="list-input-view multi-list-input-view";constructor(t,e,s){super(t,e,s),isEmpty(this.value)&&(this.value=[])}setValue(t,e){if(super.setValue(t,e),isEmpty(this.value)?this.value=[]:Array.isArray(this.value)||(this.value=[this.value]),void 0!==this.node)for(let t of this.node.findAll("li"))-1!==this.value.indexOf(t.data("value"))?t.addClass("selected"):t.removeClass("selected")}buildOptions(t,e){let s=0,i=[];for(let t in e){let a=E.li().content(E.span().content(e[t])).data("value",t);if(a.on("click",(e=>{e.stopPropagation(),e.preventDefault(),a.hasClass("selected")?(this.value=this.value.filter((e=>e!==t)),a.removeClass("selected")):(isEmpty(this.value)&&(this.value=[]),this.value.push(t),a.addClass("selected")),this.changed()})),isEmpty(this.value)&&-1!==this.value.indexOf(t)&&a.addClass("selected"),i.push(a),s++,s>=this.constructor.maximumOptions)break}return t.content(...i)}}class SearchListInputListView extends ListInputView{static maximumOptions=100;static classList=["enfugue-search-list-items"];async build(){let t=await super.build();return t.on("mousewheel",(t=>{t.stopPropagation()})),t}}class SearchListMultiInputListView extends ListMultiInputView{static maximumOptions=100;static classList=["enfugue-search-list-items","enfugue-multi-search-list-items"];async build(){let t=await super.build();return t.on("mousewheel,mouseup",(t=>{t.stopPropagation()})),t}}class SearchListInputView extends EnumerableInputView{static tagName="enfugue-search-list";static placeholder="Start typing to search…";static searchTimeout=250;static filterThreshold=.9;static listInputClass=SearchListInputListView;static stringInputClass=StringInputView;static setClosestOnBlur=!0;static resetListOnFocus=!0;static hideListOnBlur=!0;static hideListOnChange=!0;static populateSearchOnSet=!0;static debounceChangeThreshold=150;constructor(t,e,s){super(t,e,s),this.stringInput=new this.constructor.stringInputClass(t,"autofill",{placeholder:this.constructor.placeholder}),this.stringInput.onInput((t=>this.searchChanged(t))),this.stringInput.onFocus((async()=>{await this.stringInput.getNode();let t=await this.listInput.getNode(),e=this.node.element.getBoundingClientRect(),s=e.x,i=e.y+e.height,a=e.width,n=(e,n,l)=>{s=e,i=n,a=l,t.css({width:`${l}px`,left:`${e}px`,top:`${n}px`})};this.repositionInterval=setInterval((()=>{e=this.node.element.getBoundingClientRect();let t=e.x,l=e.y+e.height,o=e.width;s===t&&i===l&&a===o||n(t,l,o)}),25),document.body.appendChild(t.render()),n(s,i,a),t.css({width:`${e.width}px`,left:`${e.x}px`,top:`${e.y+e.height}px`}),this.listInput.show(),this.constructor.resetListOnFocus&&this.listInput.setValue(null,!1);let l=t=>{this.listInput.hide(),window.removeEventListener("click",l,!1),clearTimeout(this.searchDebounceTimer),clearInterval(this.repositionInterval)};window.addEventListener("click",l,!1)})),this.stringInput.onBlur((async t=>{if(this.constructor.hideListOnBlur){let t=e=>{setTimeout((async()=>{this.listInput.hide(),document.body.removeChild((await this.listInput.getNode()).element)}),100),window.removeEventListener("mouseup",t,!0)};window.addEventListener("mouseup",t,!0),clearTimeout(this.searchDebounceTimer),clearInterval(this.repositionInterval)}if(this.constructor.setClosestOnBlur){let t=strip(this.stringInput.getValue()).toLowerCase();if(isEmpty(t))this.value=null;else{let e=await this.getOptions(),s=Object.getOwnPropertyNames(e);s.sort(((s,i)=>jaroWinkler(e[i].toLowerCase(),t)-jaroWinkler(e[s].toLowerCase(),t))),this.value=s[0],this.stringInput.setValue(e[this.value],!1)}}})),this.listInput=new this.constructor.listInputClass(t,"list",{options:()=>this.getOptions()}),this.listInput.onChange((async()=>{let t=await this.getOptions(),e=this.listInput.getValue();this.value=e,this.constructor.populateSearchOnSet&&this.stringInput.setValue(t[e]),this.constructor.hideListOnChange&&(clearTimeout(this.searchDebounceTimer),clearInterval(this.repositionInterval)),this.changed()})),this.listInput.hide()}disable(){if(clearTimeout(this.searchDebounceTimer),this.stringInput.disable(),this.listInput.disable(),void 0!==this.node)for(let t of this.node.findAll(E.getCustomTag("searchSelection")))t.find("button").disabled(!0)}enable(){if(this.stringInput.enable(),this.listInput.enable(),void 0!==this.node)for(let t of this.node.findAll(E.getCustomTag("searchSelection")))t.find("button").disabled(!1)}setOptions(t){super.setOptions(t),this.listInput.setValue([],!1),this.listInput.setOptions(t)}rebuildOptions(){}buildOptions(){}getValue(){return this.value}setValue(t,e){super.setValue(t,!1);void 0!==this.stringInput&&this.stringInput.setValue(t,!1),e&&this.changed()}searchChanged(t){clearTimeout(this.searchDebounceTimer),this.searchDebounceTimer=setTimeout((()=>{this.search(t)}),this.constructor.searchTimeout)}async search(t){t=strip(t.toLowerCase()),isEmpty(t)?await this.listInput.sortFilterOptions(((t,e)=>t-e),((t,e)=>!1)):await this.listInput.sortFilterOptions(((e,s,i,a)=>jaroWinkler(a.toLowerCase(),t)-jaroWinkler(i.toLowerCase(),t)),((e,s)=>1-jaroWinkler(s.toLowerCase(),t)>=this.constructor.filterThreshold))}async build(){let t=await super.build();return t.append(await this.stringInput.getNode()),t.on("dragover",(e=>{e.preventDefault(),e.stopPropagation();let s=e.target,i=t.findAll(E.getCustomTag("searchSelection")),a=e.offsetX;for(let t of i)t.removeClass("drop-left").removeClass("drop-right");for(;-1===["ENFUGUE-SEARCH-LIST-SELECTION","ENFUGUE-SEARCH-LIST"].indexOf(s.tagName);)a+=s.offsetLeft,s=s.parentElement;if("ENFUGUE-SEARCH-LIST-SELECTION"==s.tagName&&!s.classList.contains("dragged")){let t=s.dataset.selectValue,e=i.filter((e=>e.data("select-value")===t)).shift();a>s.offsetWidth/2?e.addClass("drop-right"):e.addClass("drop-left")}})).on("drop",(e=>{let s=e.target,i=e.dataTransfer.getData("text/plain"),a=e.offsetX,n=t.findAll(E.getCustomTag("searchSelection"));for(let t of n)t.removeClass("drop-left").removeClass("drop-right");for(;-1===["ENFUGUE-SEARCH-LIST-SELECTION","ENFUGUE-SEARCH-LIST"].indexOf(s.tagName);)a+=s.offsetLeft,s=s.parentElement;if("ENFUGUE-SEARCH-LIST-SELECTION"==s.tagName){let e=s.dataset.selectValue;if(i!==e){let l=n.filter((t=>t.data("select-value")===i)).shift(),o=n.filter((t=>t.data("select-value")===e)).shift(),r=this.value.indexOf(i),u=this.value.indexOf(e),h=(l.find("span").getText(),o.find("span").getText(),a>s.offsetWidth/2);t.remove(l),this.value=this.value.filter((t=>t!=i)),!h&&r<u?u--:h&&r>u&&u++,this.value=this.value.slice(0,u).concat([i]).concat(this.value.slice(u)),this.listInput.setValue(this.value,!1),t.insert(u,l),this.changed()}}})),t}async changed(){let t=(new Date).getTime();void 0!==this.lastChange&&t-this.lastChange<this.constructor.debounceChangeThreshold||(await super.changed(),this.lastChange=t)}}class SearchListMultiInputView extends SearchListInputView{static setClosestOnBlur=!1;static resetListOnFocus=!1;static hideListOnBlur=!1;static populateSearchOnSet=!1;static hideListOnChange=!1;static listInputClass=SearchListMultiInputListView;constructor(t,e,s){super(t,e,s),this.onChange((async()=>{let t=this.getValue(),e=await this.getOptions();isEmpty(t)&&(t=[]),void 0!==this.node&&this.node.content(...t.map((t=>{let s=E.searchSelection().data("select-value",t),i=E.button().content("&times;"),a=E.span().content(e[t]);return i.on("click",(t=>{t.preventDefault(),t.stopPropagation(),this.value=this.value.filter((t=>t!==s.data("select-value"))),this.listInput.setValue(this.value,!1),this.changed()})),s.attr("draggable","true").on("dragstart",(e=>{s.addClass("dragged");let i=e.dataTransfer;i.dropEffect="move",i.effectAllowed="move",i.setData("text/plain",t)})).on("dragend",(t=>{s.removeClass("dragged")})),s.content(i,a)})),await this.stringInput.getNode())}))}async build(){let t=await super.build();return t.append(await this.stringInput.getNode()),t}}export{EnumerableInputView,SelectInputView,ListInputView,ListMultiInputView,SearchListInputView,SearchListInputListView,SearchListMultiInputView};
```

### Comparing `enfugue-0.1.2/enfugue/static/js/view/forms/input/file.mjs` & `enfugue-0.1.3/enfugue/static/js/view/forms/input/file.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/view/forms/input/numeric.mjs` & `enfugue-0.1.3/enfugue/static/js/view/forms/input/numeric.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/view/forms/input/parent.mjs` & `enfugue-0.1.3/enfugue/static/js/view/forms/input/parent.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/view/forms/input/string.mjs` & `enfugue-0.1.3/enfugue/static/js/view/forms/input/string.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/view/forms/input.mjs` & `enfugue-0.1.3/enfugue/static/js/view/forms/input.mjs`

 * *Files 6% similar despite different names*

```diff
@@ -1 +1 @@
-import{InputView}from"./input/base.mjs";import{HiddenInputView,ButtonInputView}from"./input/misc.mjs";import{FileInputView}from"./input/file.mjs";import{CheckboxInputView}from"./input/bool.mjs";import{ColorInputView}from"./input/color.mjs";import{RepeatableInputView,FormInputView}from"./input/parent.mjs";import{StringInputView,TextInputView,PasswordInputView}from"./input/string.mjs";import{NumberInputView,FloatInputView,DateInputView,TimeInputView,DateTimeInputView}from"./input/numeric.mjs";import{EnumerableInputView,SelectInputView,ListInputView,ListMultiInputView,SearchListInputView,SearchListMultiInputView}from"./input/enumerable.mjs";export{InputView,HiddenInputView,ButtonInputView,StringInputView,TextInputView,PasswordInputView,FileInputView,NumberInputView,FloatInputView,DateInputView,TimeInputView,DateTimeInputView,CheckboxInputView,ColorInputView,EnumerableInputView,SelectInputView,ListInputView,ListMultiInputView,SearchListInputView,SearchListMultiInputView,RepeatableInputView,FormInputView};
+import{InputView}from"./input/base.mjs";import{HiddenInputView,ButtonInputView}from"./input/misc.mjs";import{FileInputView}from"./input/file.mjs";import{CheckboxInputView}from"./input/bool.mjs";import{ColorInputView}from"./input/color.mjs";import{RepeatableInputView,FormInputView}from"./input/parent.mjs";import{StringInputView,TextInputView,PasswordInputView}from"./input/string.mjs";import{NumberInputView,FloatInputView,DateInputView,TimeInputView,DateTimeInputView}from"./input/numeric.mjs";import{EnumerableInputView,SelectInputView,ListInputView,ListMultiInputView,SearchListInputView,SearchListInputListView,SearchListMultiInputView}from"./input/enumerable.mjs";export{InputView,HiddenInputView,ButtonInputView,StringInputView,TextInputView,PasswordInputView,FileInputView,NumberInputView,FloatInputView,DateInputView,TimeInputView,DateTimeInputView,CheckboxInputView,ColorInputView,EnumerableInputView,SelectInputView,ListInputView,ListMultiInputView,SearchListInputView,SearchListInputListView,SearchListMultiInputView,RepeatableInputView,FormInputView};
```

### Comparing `enfugue-0.1.2/enfugue/static/js/view/image.mjs` & `enfugue-0.1.3/enfugue/static/js/view/image.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/view/menu.mjs` & `enfugue-0.1.3/enfugue/static/js/view/menu.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/view/nodes/base.mjs` & `enfugue-0.1.3/enfugue/static/js/view/nodes/base.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/view/nodes/decorations.mjs` & `enfugue-0.1.3/enfugue/static/js/view/nodes/decorations.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/view/nodes/editor.mjs` & `enfugue-0.1.3/enfugue/static/js/view/nodes/editor.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/view/nodes/image-editor.mjs` & `enfugue-0.1.3/enfugue/static/js/view/nodes/image-editor.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/view/nodes/windows.mjs` & `enfugue-0.1.3/enfugue/static/js/view/nodes/windows.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/view/notifications.mjs` & `enfugue-0.1.3/enfugue/static/js/view/notifications.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/view/scribble.mjs` & `enfugue-0.1.3/enfugue/static/js/view/scribble.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/view/status.mjs` & `enfugue-0.1.3/enfugue/static/js/view/status.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/static/js/view/table.mjs` & `enfugue-0.1.3/enfugue/static/js/view/table.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/util/downloads.py` & `enfugue-0.1.3/enfugue/util/downloads.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/util/gpu.py` & `enfugue-0.1.3/enfugue/util/gpu.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/util/gputil.py` & `enfugue-0.1.3/enfugue/util/gputil.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/util/images.py` & `enfugue-0.1.3/enfugue/util/images.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/util/installation.py` & `enfugue-0.1.3/enfugue/util/installation.py`

 * *Files 10% similar despite different names*

```diff
@@ -105,14 +105,25 @@
     return configuration
 
 
 def get_version() -> Version:
     """
     Gets the version of enfugue installed.
     """
+    import logging
+    logger = logging.getLogger("enfugue")
+    try:
+        local_install = get_local_installation_directory()
+        version_file = os.path.join(local_install, "version.txt")
+        if os.path.exists(version_file):
+            with open(version_file, "r") as fp:
+                return Version(fp.read())
+    except:
+        pass
+
     from importlib.metadata import version, PackageNotFoundError
 
     try:
         return Version(version("enfugue"))
     except PackageNotFoundError:
         return "development"
```

### Comparing `enfugue-0.1.2/enfugue/util/security.py` & `enfugue-0.1.3/enfugue/util/security.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/util/signature.py` & `enfugue-0.1.3/enfugue/util/signature.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue/util/tokens.py` & `enfugue-0.1.3/enfugue/util/tokens.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.2/enfugue.egg-info/SOURCES.txt` & `enfugue-0.1.3/enfugue.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 setup.py
 enfugue/__init__.py
 enfugue/__main__.py
 enfugue/enfugue.py
 enfugue/server.py
+enfugue/version.txt
 enfugue.egg-info/PKG-INFO
 enfugue.egg-info/SOURCES.txt
 enfugue.egg-info/dependency_links.txt
 enfugue.egg-info/entry_points.txt
 enfugue.egg-info/requires.txt
 enfugue.egg-info/top_level.txt
 enfugue/api/__init__.py
@@ -188,14 +189,15 @@
 enfugue/static/js/view/forms/input/string.mjs
 enfugue/static/js/view/nodes/base.mjs
 enfugue/static/js/view/nodes/decorations.mjs
 enfugue/static/js/view/nodes/editor.mjs
 enfugue/static/js/view/nodes/image-editor.mjs
 enfugue/static/js/view/nodes/windows.mjs
 enfugue/util/__init__.py
+enfugue/util/browser.py
 enfugue/util/downloads.py
 enfugue/util/gpu.py
 enfugue/util/gputil.py
 enfugue/util/images.py
 enfugue/util/installation.py
 enfugue/util/log.py
 enfugue/util/security.py
```

### Comparing `enfugue-0.1.2/enfugue.egg-info/requires.txt` & `enfugue-0.1.3/enfugue.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 cheroot>=9.0.0
 nvidia-pyindex>=1.0.9
-pibble[cherrypy]>=0.5
+pibble[cherrypy]>=0.6
 torch<2.0,>=1.13.1
-numpy>=1.24.0
+numpy>=1.24.3
 colored<1.5,>=1.4
 diffusers<0.17,>=0.16
 albumentations<0.5,>=0.4.3
 opencv-python<4.8,>=4.7.0.72
 pudb==2019.2
 invisible-watermark<0.2,>=0.1
 imageio<3.0,>=2.9
@@ -24,27 +24,32 @@
 tqdm>=4.27
 safetensors<0.4,>=0.3
 realesrgan<0.4,>=0.3
 gfpgan<1.4,>=1.3.8
 backgroundremover<0.3,>=0.2.3
 beautifulsoup4<5,>=4.12
 pystray<0.24,>=0.19
-html2text
+pydantic==1.10.10
+html2text==2020.1.16
 taming-transformers
 clip
 latent-diffusion
 
 [build]
 types-protobuf<5.0,>=4.23.0.1
 types-requests<3.0,>=2.30
 types-setuptools<68.0,>=67.7
 types-urllib3<2.0,>=1.26.25
 types-tabulate<0.10,>=0.9
 types-pyyaml<7.0,>=6.0
 importchecker<3.0,>=2.0
+pyinstaller>=5.13.0
+
+[directml]
+torch-directml==0.1.13.1.dev230413
 
 [tensorrt]
 polygraphy<0.48,>=0.47
 onnx==1.12
 onnxruntime-gpu==1.12.1
 onnx-graphsurgeon==0.3.26
-tensorrt<8.7,>=8.6
+tensorrt<8.7,>=8.6.0
```

### Comparing `enfugue-0.1.2/setup.py` & `enfugue-0.1.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,33 @@
 import os
 from setuptools import setup, find_packages
 
 package_name = "enfugue"
-version_major = "0"
-version_minor = "1"
-version_patch = "2"
+
+# These variables will be replaced during build, but we keep
+# a default version so we can install from the directory itself
+try:
+    version_major = int("0")
+except:
+    version_major = 0
+try:
+    version_minor = int("1")
+except:
+    version_minor = 0
+try:
+    version_patch = int("3")
+except:
+    version_patch = 1
 
 install_requires = [
     "cheroot>=9.0.0",
     "nvidia-pyindex>=1.0.9",
-    "pibble[cherrypy]>=0.5",
+    "pibble[cherrypy]>=0.6",
     "torch>=1.13.1,<2.0",
-    "numpy>=1.24.0",
+    "numpy>=1.24.3",
     "colored>=1.4,<1.5",
     "diffusers>=0.16,<0.17",
     "albumentations>=0.4.3,<0.5",
     "opencv-python>=4.7.0.72,<4.8",
     "pudb==2019.2",
     "invisible-watermark>=0.1,<0.2",
     "imageio>=2.9,<3.0",
@@ -33,36 +45,39 @@
     "tqdm>=4.27",
     "safetensors>=0.3,<0.4",
     "realesrgan>=0.3,<0.4",
     "gfpgan>=1.3.8,<1.4",
     "backgroundremover>=0.2.3,<0.3",
     "beautifulsoup4>=4.12,<5",
     "pystray>=0.19,<0.24",
-    "html2text",
+    "pydantic==1.10.10",
+    "html2text==2020.1.16",
     "taming-transformers",
     "clip",
     "latent-diffusion",
 ]
 
 extras_require = {
+    "directml": ["torch-directml==0.1.13.1.dev230413"],
     "tensorrt": [
         "polygraphy>=0.47,<0.48",
         "onnx==1.12",
         "onnxruntime-gpu==1.12.1",
         "onnx-graphsurgeon==0.3.26",
-        "tensorrt>=8.6,<8.7",
+        "tensorrt>=8.6.0,<8.7",
     ],
     "build": [
         "types-protobuf>=4.23.0.1,<5.0",
         "types-requests>=2.30,<3.0",
         "types-setuptools>=67.7,<68.0",
         "types-urllib3>=1.26.25,<2.0",
         "types-tabulate>=0.9,<0.10",
         "types-pyyaml>=6.0,<7.0",
         "importchecker>=2.0,<3.0",
+        "pyinstaller>=5.13.0"
     ],
 }
 
 packaged_files = []
 
 here = os.path.dirname(os.path.abspath(__file__))
 package_dir = os.path.join(here, package_name)
@@ -77,13 +92,13 @@
 
 setup(
     name=package_name,
     author="Benjamin Paine",
     author_email="painebenjamin@gmail.com",
     version=f"{version_major}.{version_minor}.{version_patch}",
     packages=find_packages("."),
-    package_data={package_name: ["py.typed", *package_data]},
+    package_data={package_name: ["py.typed", "version.txt", *package_data]},
     license="agpl-3.0",
     entry_points={"console_scripts": ["enfugue = enfugue.__main__:main"]},
     install_requires=install_requires,
     extras_require=extras_require,
-)
+)
```

