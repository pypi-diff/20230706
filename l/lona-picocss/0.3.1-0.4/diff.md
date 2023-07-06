# Comparing `tmp/lona-picocss-0.3.1.tar.gz` & `tmp/lona-picocss-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lona-picocss-0.3.1.tar", last modified: Sat May  6 10:08:26 2023, max compression
+gzip compressed data, was "lona-picocss-0.4.tar", last modified: Thu Jul  6 14:38:23 2023, max compression
```

## Comparing `lona-picocss-0.3.1.tar` & `lona-picocss-0.4.tar`

### file list

```diff
@@ -1,139 +1,165 @@
-drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-05-06 10:08:26.427148 lona-picocss-0.3.1/
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1071 2023-02-07 20:21:49.000000 lona-picocss-0.3.1/LICENSE.txt
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     2660 2023-05-06 10:08:26.427148 lona-picocss-0.3.1/PKG-INFO
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      617 2023-02-16 16:11:01.000000 lona-picocss-0.3.1/README.md
-drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-05-06 10:08:26.423148 lona-picocss-0.3.1/lona_picocss/
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     4288 2023-05-06 10:04:39.000000 lona-picocss-0.3.1/lona_picocss/__init__.py
-drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-05-06 10:08:26.423148 lona-picocss-0.3.1/lona_picocss/html/
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      333 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/lona_picocss/html/__init__.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1588 2023-02-25 16:40:44.000000 lona-picocss-0.3.1/lona_picocss/html/base.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1817 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/lona_picocss/html/buttons.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      929 2023-02-25 16:40:44.000000 lona-picocss-0.3.1/lona_picocss/html/cards.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      498 2023-02-25 16:40:44.000000 lona-picocss-0.3.1/lona_picocss/html/generic.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     2866 2023-02-25 16:40:44.000000 lona-picocss-0.3.1/lona_picocss/html/icons.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      472 2023-02-25 16:40:44.000000 lona-picocss-0.3.1/lona_picocss/html/inputs.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      885 2023-02-25 16:40:44.000000 lona-picocss-0.3.1/lona_picocss/html/links.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1837 2023-02-25 16:40:44.000000 lona-picocss-0.3.1/lona_picocss/html/modal.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      701 2023-02-25 16:40:44.000000 lona-picocss-0.3.1/lona_picocss/html/progress.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1706 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/lona_picocss/html/scroller.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1848 2023-02-25 16:40:44.000000 lona-picocss-0.3.1/lona_picocss/html/tabs.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)    10273 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/lona_picocss/settings.py
-drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-05-06 10:08:26.419148 lona-picocss-0.3.1/lona_picocss/static/
-drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-05-06 10:08:26.423148 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/
-drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-05-06 10:08:26.419148 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/
-drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-05-06 10:08:26.423148 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/feather-icons/
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1081 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/feather-icons/LICENSE
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)    60317 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/feather-icons/feather-sprite.svg
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)   158900 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/feather-icons/feather.js
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)    66446 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/feather-icons/feather.js.map
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)    75963 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/feather-icons/feather.min.js
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)    80886 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/feather-icons/feather.min.js.map
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)    53786 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/feather-icons/icons.json
-drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-05-06 10:08:26.423148 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1066 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/LICENSE.md
-drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-05-06 10:08:26.423148 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)    78670 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.classless.css
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)   193178 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.classless.css.map
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)    69329 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.classless.min.css
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)   193408 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.classless.min.css.map
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)    83517 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.css
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)   201166 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.css.map
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)    78207 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.fluid.classless.css
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)   192522 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.fluid.classless.css.map
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)    68998 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.fluid.classless.min.css
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)   192745 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.fluid.classless.min.css.map
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)    73571 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.min.css
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)   201142 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.min.css.map
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)    44881 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.slim.css
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)   112715 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.slim.css.map
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)    40179 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.slim.min.css
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)   113084 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.slim.min.css.map
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      165 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/postcss.config.js
-drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-05-06 10:08:26.427148 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/themes/
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)    27484 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/themes/default.css
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)    58820 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/themes/default.css.map
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)    25324 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/themes/default.min.css
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)    59593 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/themes/default.min.css.map
-drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-05-06 10:08:26.427148 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      135 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/_functions.scss
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1811 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/_variables.scss
-drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-05-06 10:08:26.427148 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/components/
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     2147 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/components/_accordion.scss
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1190 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/components/_card.scss
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     4993 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/components/_dropdown.scss
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     3247 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/components/_modal.scss
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     2802 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/components/_nav.scss
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     2114 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/components/_progress.scss
-drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-05-06 10:08:26.427148 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     5158 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_button.scss
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1670 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_code.scss
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1061 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_embedded.scss
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     6670 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_form-alt-input-types.scss
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     3029 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_form-checkbox-radio.scss
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     9239 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_form.scss
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      701 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_miscs.scss
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1133 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_table.scss
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     4935 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_typography.scss
-drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-05-06 10:08:26.427148 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/layout/
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      940 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_container.scss
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1583 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_document.scss
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      536 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_grid.scss
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      276 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_scroller.scss
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      115 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_section.scss
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1845 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_sectioning.scss
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      248 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/pico.classless.scss
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      370 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/pico.fluid.classless.scss
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1567 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/pico.scss
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1307 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/pico.slim.scss
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      139 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/postcss.config.js
-drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-05-06 10:08:26.427148 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/themes/
-drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-05-06 10:08:26.427148 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     2029 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_colors.scss
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     9649 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_dark.scss
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     9438 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_light.scss
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     5408 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_styles.scss
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      657 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default.scss
-drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-05-06 10:08:26.427148 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1096 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_accessibility.scss
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1038 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_loading.scss
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1034 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_reduce-motion.scss
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     5558 2023-05-04 15:40:58.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_tooltip.scss
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      456 2023-02-25 16:40:44.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/feather-widgets.js
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)    19278 2023-02-06 18:25:40.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/logo.svg
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1051 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/lona-picocss.css
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     3172 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/lona_picocss/static/lona-picocss/picocss-widgets.js
-drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-05-06 10:08:26.419148 lona-picocss-0.3.1/lona_picocss/templates/
-drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-05-06 10:08:26.427148 lona-picocss-0.3.1/lona_picocss/templates/picocss/
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     4604 2023-02-25 16:40:44.000000 lona-picocss-0.3.1/lona_picocss/templates/picocss/base.html
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1734 2023-02-25 16:40:44.000000 lona-picocss-0.3.1/lona_picocss/templates/picocss/color-scheme.css
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      139 2023-02-25 16:40:44.000000 lona-picocss-0.3.1/lona_picocss/templates/picocss/disconnect-message.html
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      108 2023-02-06 22:35:59.000000 lona-picocss-0.3.1/lona_picocss/templates/picocss/footer.html
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1175 2023-02-24 18:33:34.000000 lona-picocss-0.3.1/lona_picocss/templates/picocss/header.html
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)       43 2023-02-25 16:40:44.000000 lona-picocss-0.3.1/lona_picocss/templates/picocss/waiting-for-server-message.html
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1362 2023-02-16 16:11:01.000000 lona-picocss-0.3.1/lona_picocss/themes.py
-drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-05-06 10:08:26.427148 lona-picocss-0.3.1/lona_picocss/views/
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)        0 2023-02-12 19:34:13.000000 lona-picocss-0.3.1/lona_picocss/views/__init__.py
-drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-05-06 10:08:26.427148 lona-picocss-0.3.1/lona_picocss/views/components/
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)        0 2023-02-12 20:14:59.000000 lona-picocss-0.3.1/lona_picocss/views/components/__init__.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1157 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/lona_picocss/views/components/buttons.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1126 2023-02-12 22:30:38.000000 lona-picocss-0.3.1/lona_picocss/views/components/cards.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1285 2023-02-12 23:16:43.000000 lona-picocss-0.3.1/lona_picocss/views/components/forms.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     4268 2023-02-25 16:40:44.000000 lona-picocss-0.3.1/lona_picocss/views/components/icons.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     2598 2023-02-14 21:42:41.000000 lona-picocss-0.3.1/lona_picocss/views/components/modal.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      383 2023-02-12 23:24:26.000000 lona-picocss-0.3.1/lona_picocss/views/components/progress.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      952 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/lona_picocss/views/components/scroller.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      371 2023-02-12 22:46:40.000000 lona-picocss-0.3.1/lona_picocss/views/components/tabs.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     3589 2023-02-12 22:09:51.000000 lona-picocss-0.3.1/lona_picocss/views/components/typography.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     2323 2023-02-25 16:40:44.000000 lona-picocss-0.3.1/lona_picocss/views/error_views.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      469 2023-02-12 19:33:13.000000 lona-picocss-0.3.1/lona_picocss/views/it_works.py
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     7418 2023-02-16 16:11:01.000000 lona-picocss-0.3.1/lona_picocss/views/settings.py
-drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-05-06 10:08:26.423148 lona-picocss-0.3.1/lona_picocss.egg-info/
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     2660 2023-05-06 10:08:26.000000 lona-picocss-0.3.1/lona_picocss.egg-info/PKG-INFO
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     6241 2023-05-06 10:08:26.000000 lona-picocss-0.3.1/lona_picocss.egg-info/SOURCES.txt
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)        1 2023-05-06 10:08:26.000000 lona-picocss-0.3.1/lona_picocss.egg-info/dependency_links.txt
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)      124 2023-05-06 10:08:26.000000 lona-picocss-0.3.1/lona_picocss.egg-info/requires.txt
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)       13 2023-05-06 10:08:26.000000 lona-picocss-0.3.1/lona_picocss.egg-info/top_level.txt
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     1387 2023-05-06 10:04:26.000000 lona-picocss-0.3.1/pyproject.toml
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)       38 2023-05-06 10:08:26.427148 lona-picocss-0.3.1/setup.cfg
-drwxrwxr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-05-06 10:08:26.427148 lona-picocss-0.3.1/tests/
--rw-rw-r--   0 fscherf   (1000) fscherf   (1000)     5610 2023-05-04 17:06:51.000000 lona-picocss-0.3.1/tests/test_screenshots.py
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.032607 lona-picocss-0.4/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1071 2023-05-31 16:56:42.000000 lona-picocss-0.4/LICENSE.txt
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     2690 2023-07-06 14:38:23.032607 lona-picocss-0.4/PKG-INFO
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      652 2023-07-06 14:34:02.000000 lona-picocss-0.4/README.md
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.020606 lona-picocss-0.4/lona_picocss/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1766 2023-07-06 14:36:15.000000 lona-picocss-0.4/lona_picocss/__init__.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      147 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/apps.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     7498 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/color_schemes.py
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.020606 lona-picocss-0.4/lona_picocss/html/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      333 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/html/__init__.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1588 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/html/base.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1817 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/html/buttons.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      929 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/html/cards.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      498 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/html/generic.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     2866 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/html/icons.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      472 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/html/inputs.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      885 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/html/links.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1837 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/html/modal.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      701 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/html/progress.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1706 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/html/scroller.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1848 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/html/tabs.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1881 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/middlewares.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     3613 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/navigation.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     2563 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/routes.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     6028 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/settings.py
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.020606 lona-picocss-0.4/lona_picocss/static/
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.024607 lona-picocss-0.4/lona_picocss/static/lona-picocss/
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.020606 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.024607 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/feather-icons/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1081 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/feather-icons/LICENSE
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    60317 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/feather-icons/feather-sprite.svg
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)   158900 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/feather-icons/feather.js
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    66446 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/feather-icons/feather.js.map
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    75963 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/feather-icons/feather.min.js
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    80886 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/feather-icons/feather.min.js.map
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    53786 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/feather-icons/icons.json
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.024607 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1066 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/LICENSE.md
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.024607 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    78670 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.classless.css
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)   193178 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.classless.css.map
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    69329 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.classless.min.css
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)   193408 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.classless.min.css.map
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    83517 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.css
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)   201166 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.css.map
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    78207 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.fluid.classless.css
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)   192522 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.fluid.classless.css.map
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    68998 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.fluid.classless.min.css
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)   192745 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.fluid.classless.min.css.map
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    73571 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.min.css
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)   201142 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.min.css.map
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    44881 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.slim.css
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)   112715 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.slim.css.map
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    40179 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.slim.min.css
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)   113084 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.slim.min.css.map
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      165 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/postcss.config.js
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.024607 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/themes/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    27484 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/themes/default.css
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    58820 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/themes/default.css.map
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    25324 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/themes/default.min.css
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    59593 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/themes/default.min.css.map
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.028607 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      135 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/_functions.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1811 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/_variables.scss
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.028607 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/components/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     2147 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/components/_accordion.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1190 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/components/_card.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     4993 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/components/_dropdown.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     3247 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/components/_modal.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     2802 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/components/_nav.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     2114 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/components/_progress.scss
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.028607 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     5158 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_button.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1670 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_code.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1061 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_embedded.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     6670 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_form-alt-input-types.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     3029 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_form-checkbox-radio.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     9239 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_form.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      701 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_miscs.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1133 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_table.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     4935 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_typography.scss
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.028607 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/layout/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      940 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_container.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1583 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_document.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      536 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_grid.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      276 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_scroller.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      115 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_section.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1845 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_sectioning.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      248 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/pico.classless.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      370 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/pico.fluid.classless.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1567 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/pico.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1307 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/pico.slim.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      139 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/postcss.config.js
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.028607 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/themes/
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.028607 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     2029 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_colors.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     9649 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_dark.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     9438 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_light.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     5408 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_styles.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      657 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default.scss
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.028607 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1096 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_accessibility.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1038 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_loading.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1034 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_reduce-motion.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     5558 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_tooltip.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      456 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/feather-widgets.js
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    19278 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/logo.svg
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1658 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/lona-picocss.css
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     3172 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/picocss-widgets.js
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.020606 lona-picocss-0.4/lona_picocss/templates/
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.028607 lona-picocss-0.4/lona_picocss/templates/picocss/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)       40 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/picocss/403.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)       36 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/picocss/404.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      349 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/picocss/500.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     4600 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/picocss/base.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1734 2023-06-09 19:36:12.000000 lona-picocss-0.4/lona_picocss/templates/picocss/color-scheme.css
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      139 2023-06-10 13:44:23.000000 lona-picocss-0.4/lona_picocss/templates/picocss/disconnect-message.html
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.028607 lona-picocss-0.4/lona_picocss/templates/picocss/django/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      207 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/picocss/django/403.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      207 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/picocss/django/404.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      379 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/picocss/django/500.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1973 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/picocss/django/base.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      108 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/templates/picocss/footer.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1373 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/picocss/header.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)       43 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/templates/picocss/waiting-for-server-message.html
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.032607 lona-picocss-0.4/lona_picocss/templates/registration/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      261 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/registration/logged_out.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1739 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/registration/login.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      547 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/registration/password_change_done.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1715 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/registration/password_change_form.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      599 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/registration/password_reset_complete.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     2176 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/registration/password_reset_confirm.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1011 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/registration/password_reset_done.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1146 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/registration/password_reset_form.html
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.032607 lona-picocss-0.4/lona_picocss/templatetags/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templatetags/__init__.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      539 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templatetags/lona_picocss_filter.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      459 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/utils.py
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.032607 lona-picocss-0.4/lona_picocss/views/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)       75 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/views/__init__.py
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.032607 lona-picocss-0.4/lona_picocss/views/components/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)        0 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/views/components/__init__.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1157 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/views/components/buttons.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1126 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/views/components/cards.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1285 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/views/components/forms.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     4268 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/views/components/icons.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     2598 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/views/components/modal.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      383 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/views/components/progress.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      952 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/views/components/scroller.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      371 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/views/components/tabs.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     3589 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/views/components/typography.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      546 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/views/django_error_views.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1670 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/views/error_views.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      469 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/views/it_works.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     8056 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/views/settings.py
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.020606 lona-picocss-0.4/lona_picocss.egg-info/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     2690 2023-07-06 14:38:23.000000 lona-picocss-0.4/lona_picocss.egg-info/PKG-INFO
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     7280 2023-07-06 14:38:23.000000 lona-picocss-0.4/lona_picocss.egg-info/SOURCES.txt
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)        1 2023-07-06 14:38:23.000000 lona-picocss-0.4/lona_picocss.egg-info/dependency_links.txt
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      199 2023-07-06 14:38:23.000000 lona-picocss-0.4/lona_picocss.egg-info/requires.txt
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)       13 2023-07-06 14:38:23.000000 lona-picocss-0.4/lona_picocss.egg-info/top_level.txt
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1492 2023-07-06 14:36:06.000000 lona-picocss-0.4/pyproject.toml
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)       38 2023-07-06 14:38:23.032607 lona-picocss-0.4/setup.cfg
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.032607 lona-picocss-0.4/tests/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     8042 2023-07-06 14:34:02.000000 lona-picocss-0.4/tests/test_screenshots.py
```

### Comparing `lona-picocss-0.3.1/LICENSE.txt` & `lona-picocss-0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/PKG-INFO` & `lona-picocss-0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lona-picocss
-Version: 0.3.1
+Version: 0.4
 Summary: Pico.css bindings for Lona
 Author-email: Florian Scherf <mail@florianscherf.de>
 License: MIT License
         
         Copyright (c) 2023 Florian Scherf
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,15 +33,15 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: packaging
-Provides-Extra: testing
+Provides-Extra: test
 License-File: LICENSE.txt
 
 # lona-picocss
 
 ![license MIT](https://img.shields.io/pypi/l/lona-picocss.svg)
 ![Python Version](https://img.shields.io/pypi/pyversions/lona-picocss.svg)
 ![Latest Version](https://img.shields.io/pypi/v/lona-picocss.svg)
@@ -61,7 +61,8 @@
 
 
 ## Topics
 
  - [Getting Started](doc/getting-started.md)
  - [Customization](doc/customization.md)
  - [Components](doc/components.md)
+ - [Django Support](doc/django.md)
```

### Comparing `lona-picocss-0.3.1/README.md` & `lona-picocss-0.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -19,7 +19,8 @@
 
 
 ## Topics
 
  - [Getting Started](doc/getting-started.md)
  - [Customization](doc/customization.md)
  - [Components](doc/components.md)
+ - [Django Support](doc/django.md)
```

### Comparing `lona-picocss-0.3.1/lona_picocss/html/base.py` & `lona-picocss-0.4/lona_picocss/html/base.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/html/buttons.py` & `lona-picocss-0.4/lona_picocss/html/buttons.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/html/cards.py` & `lona-picocss-0.4/lona_picocss/html/cards.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/html/icons.py` & `lona-picocss-0.4/lona_picocss/html/icons.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/html/links.py` & `lona-picocss-0.4/lona_picocss/html/links.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/html/modal.py` & `lona-picocss-0.4/lona_picocss/html/modal.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/html/progress.py` & `lona-picocss-0.4/lona_picocss/html/progress.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/html/scroller.py` & `lona-picocss-0.4/lona_picocss/html/scroller.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/html/tabs.py` & `lona-picocss-0.4/lona_picocss/html/tabs.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/feather-icons/LICENSE` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/feather-icons/LICENSE`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/feather-icons/feather-sprite.svg` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/feather-icons/feather-sprite.svg`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/feather-icons/feather.js` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/feather-icons/feather.js`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/feather-icons/feather.js.map` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/feather-icons/feather.js.map`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/feather-icons/feather.min.js` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/feather-icons/feather.min.js`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/feather-icons/feather.min.js.map` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/feather-icons/feather.min.js.map`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/feather-icons/icons.json` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/feather-icons/icons.json`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/LICENSE.md` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.classless.css` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.classless.css`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.classless.css.map` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.classless.css.map`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.classless.min.css` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.classless.min.css`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.classless.min.css.map` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.classless.min.css.map`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.css` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.css`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.css.map` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.css.map`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.fluid.classless.css` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.fluid.classless.css`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.fluid.classless.css.map` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.fluid.classless.css.map`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.fluid.classless.min.css` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.fluid.classless.min.css`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.fluid.classless.min.css.map` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.fluid.classless.min.css.map`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.min.css` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.min.css`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.min.css.map` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.min.css.map`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.slim.css` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.slim.css`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.slim.css.map` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.slim.css.map`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.slim.min.css` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.slim.min.css`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.slim.min.css.map` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.slim.min.css.map`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/themes/default.css` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/themes/default.css`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/themes/default.css.map` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/themes/default.css.map`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/themes/default.min.css` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/themes/default.min.css`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/css/themes/default.min.css.map` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/themes/default.min.css.map`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/_variables.scss` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/_variables.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/components/_accordion.scss` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/components/_accordion.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/components/_card.scss` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/components/_card.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/components/_dropdown.scss` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/components/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/components/_modal.scss` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/components/_modal.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/components/_nav.scss` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/components/_nav.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/components/_progress.scss` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/components/_progress.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_button.scss` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_button.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_code.scss` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_code.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_embedded.scss` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_embedded.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_form-alt-input-types.scss` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_form-alt-input-types.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_form-checkbox-radio.scss` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_form-checkbox-radio.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_form.scss` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_form.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_miscs.scss` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_miscs.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_table.scss` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_table.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_typography.scss` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_typography.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_container.scss` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_container.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_document.scss` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_document.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_grid.scss` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_grid.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_sectioning.scss` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_sectioning.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/pico.scss` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/pico.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/pico.slim.scss` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/pico.slim.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_colors.scss` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_colors.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_dark.scss` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_dark.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_light.scss` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_light.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_styles.scss` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_styles.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default.scss` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_accessibility.scss` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_accessibility.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_loading.scss` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_loading.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_reduce-motion.scss` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_reduce-motion.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_tooltip.scss` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/logo.svg` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/logo.svg`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/static/lona-picocss/picocss-widgets.js` & `lona-picocss-0.4/lona_picocss/static/lona-picocss/picocss-widgets.js`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/templates/picocss/base.html` & `lona-picocss-0.4/lona_picocss/templates/picocss/base.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-{% set get_theme_data = Lona.import('lona_picocss.themes.get_theme_data') %}
-{% set hex_to_rgba = Lona.import('lona_picocss.themes.hex_to_rgba') %}
-{% set theme_data = get_theme_data(Lona) %}
+{% set get_theme_data = Lona.import('lona_picocss.settings.get_theme_data') %}
+{% set theme_data = get_theme_data(request) %}
 <!doctype html>
 <html data-theme="{{ theme_data.theme_settings.theme }}">
     <head>
         <meta charset="utf-8">
         <meta name="viewport" content="width=device-width, initial-scale=1">
 
         {% if theme_data.theme_settings.theme == 'dark' %}
             <meta name="theme-color" content="#11191F">
         {% elif theme_data.theme_settings.theme == 'light' %}
             <meta name="theme-color" content="#FFFFFF">
         {% endif %}
 
         {{ Lona.load_stylesheets() }}
         <style>
-            {% include "picocss/color-scheme.css" %}
+          {{ theme_data.css_string }}
         </style>
     </head>
     <body{% if theme_data.theme_settings.fluid %} class="fluid"{% endif %}>
         <div
             data-theme="generated"
             {% if theme_data.theme_settings.page_width and not theme_data.theme_settings.fluid %} style="max-width: {{ theme_data.theme_settings.page_width }}" {% endif %}
             {% if not theme_data.theme_settings.fluid %} class="container"{% endif %}>
@@ -46,15 +45,15 @@
                     const auto_reconnect = true;
                 {% else %}
                     const auto_reconnect = false;
                 {% endif %}
 
                 const lona_context = new Lona.LonaContext({
                     target: 'main#lona',
-                    title: '{{ theme_data.theme_settings.title }}',
+                    title: '{{ theme_data.theme_settings.brand }}',
                     update_address_bar: true,
                     update_title: true,
                     follow_redirects: true,
                     follow_http_redirects: true,
                 });
 
                 let first_connect = true;
@@ -95,16 +94,17 @@
                     `;
 
                     if(!auto_reconnect) {
                         return;
                     }
 
                     setTimeout(() => {
-                        lona_context.reconnect();
-
+                        lona_context.reconnect({
+                            create_window: false,
+                        });
                     }, 1000);
                 });
 
                 // waiting for server message
                 lona_context.add_view_timeout_hook((lona_context, lona_window) => {
                     lona_window.set_html(`
                         {% include "picocss/waiting-for-server-message.html" %}
@@ -120,8 +120,8 @@
 
                 // setup
                 lona_context.setup();
                 window['lona_context'] = lona_context;
             });
         </script>
     </body>
-</html>
+</html>
```

#### html2text {}

```diff
@@ -1,10 +1,9 @@
-{% set get_theme_data = Lona.import('lona_picocss.themes.get_theme_data') %} {%
-set hex_to_rgba = Lona.import('lona_picocss.themes.hex_to_rgba') %} {% set
-theme_data = get_theme_data(Lona) %}
+{% set get_theme_data = Lona.import('lona_picocss.settings.get_theme_data') %}
+{% set theme_data = get_theme_data(request) %}
 
  {% if theme_data.theme_settings.theme == 'dark' %}
  {% elif theme_data.theme_settings.theme == 'light' %}
  {% endif %} {{ Lona.load_stylesheets() }}
 % if theme_data.theme_settings.fluid %} class="fluid"{% endif %}>
 % if theme_data.theme_settings.page_width and not
 theme_data.theme_settings.fluid %} style="max-width: {
```

### Comparing `lona-picocss-0.3.1/lona_picocss/templates/picocss/color-scheme.css` & `lona-picocss-0.4/lona_picocss/templates/picocss/color-scheme.css`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/views/components/buttons.py` & `lona-picocss-0.4/lona_picocss/views/components/buttons.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/views/components/cards.py` & `lona-picocss-0.4/lona_picocss/views/components/cards.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/views/components/forms.py` & `lona-picocss-0.4/lona_picocss/views/components/forms.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/views/components/icons.py` & `lona-picocss-0.4/lona_picocss/views/components/icons.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/views/components/modal.py` & `lona-picocss-0.4/lona_picocss/views/components/modal.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/views/components/scroller.py` & `lona-picocss-0.4/lona_picocss/views/components/scroller.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/views/components/typography.py` & `lona-picocss-0.4/lona_picocss/views/components/typography.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.3.1/lona_picocss/views/settings.py` & `lona-picocss-0.4/lona_picocss/views/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,26 +34,36 @@
     def refresh(self):
         return {
             'http_redirect': self.server.reverse('picocss__settings'),
         }
 
     def handle_change(self, input_event):
         name = input_event.node.state['name']
+        value = input_event.node.value
 
-        setattr(self.server.settings, name, input_event.node.value)
+        settings.set(name, value)
+        settings.render_theme()
 
         return self.refresh()
 
-
     def apply(self, input_event):
+        settings.render_theme()
+
         return self.refresh()
 
     def reset(self, input_event):
-        for key, value in settings.DEFAULTS.items():
-            setattr(self.server.settings, key, value)
+        settings.reset()
+        settings.load_lona_settings()
+        settings.render_theme()
+
+        return self.refresh()
+
+    def reset_to_defaults(self, input_event):
+        settings.reset()
+        settings.render_theme()
 
         return self.refresh()
 
     def handle_request(self, request):
         self.set_title('Pico.css Settings')
 
         html = HTML(
@@ -73,14 +83,19 @@
                     Grid(
                         Button(
                             'Reset',
                             secondary=True,
                             handle_click=self.reset,
                         ),
                         Button(
+                            'Reset to defaults',
+                            secondary=True,
+                            handle_click=self.reset_to_defaults,
+                        ),
+                        Button(
                             'Apply',
                             handle_click=self.apply,
                         ),
                     ),
                     Label(
                         'Compiled Settings',
                         Pre(
@@ -106,27 +121,31 @@
         if project_type == 'app':
             settings_prefix = 'app.settings.'
 
         # setup settings
         settings_pre = html.query_selector('pre')
         settings_form = html[2][0]
 
-        for index, name in enumerate(settings.SETTINGS.keys()):
+        for index, name in enumerate(settings.get_names()):
             slug = name[len('PICOCSS_'):].replace('_', '-').lower()
             verbose_name = name[len('PICOCSS_'):].replace('_', ' ').title()
-            default = settings.DEFAULTS[name]
-            values = settings.SETTINGS[name]
-            value = self.server.settings.get(name, default)
+            value = settings.get(name)
+            values = settings.get_default(name, value)
 
-            # object values
-            if name in settings.OBJECT_SETTINGS:
+            # unsupported settings
+            if name in ('PICOCSS_NAVIGATION', ):
                 continue
 
+            # show exceptions
+            if name == 'PICOCSS_SHOW_EXCEPTIONS':
+                if callable(value):
+                    value = True
+
             # string values
-            elif isinstance(values, str):
+            if isinstance(values, str):
                 field = Label(
                     verbose_name,
                     TextInput(
                         value=value,
                         placeholder='not set',
                         bubble_up=True,
                         handle_change=self.handle_change,
@@ -172,15 +191,20 @@
             settings_form.append(field)
 
             if index in self.SPACER:
                 settings_form.append(Br())
                 settings_form.append(Br())
 
             # add config variable to compiled output
-            if value != settings.DEFAULTS[name]:
+            default = settings.get_default(name)
+
+            if isinstance(default, list) and len(default) > 0:
+                default = default[0]
+
+            if value != default:
                 settings_pre.write_line(
                     f'{settings_prefix}{name} = {repr(value)}',
                 )
 
         # empty settings
         if len(settings_pre.nodes) == 0:
             settings_pre.set_text('# nothing to configure\n\n')
```

### Comparing `lona-picocss-0.3.1/lona_picocss.egg-info/PKG-INFO` & `lona-picocss-0.4/lona_picocss.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lona-picocss
-Version: 0.3.1
+Version: 0.4
 Summary: Pico.css bindings for Lona
 Author-email: Florian Scherf <mail@florianscherf.de>
 License: MIT License
         
         Copyright (c) 2023 Florian Scherf
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,15 +33,15 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: packaging
-Provides-Extra: testing
+Provides-Extra: test
 License-File: LICENSE.txt
 
 # lona-picocss
 
 ![license MIT](https://img.shields.io/pypi/l/lona-picocss.svg)
 ![Python Version](https://img.shields.io/pypi/pyversions/lona-picocss.svg)
 ![Latest Version](https://img.shields.io/pypi/v/lona-picocss.svg)
@@ -61,7 +61,8 @@
 
 
 ## Topics
 
  - [Getting Started](doc/getting-started.md)
  - [Customization](doc/customization.md)
  - [Components](doc/components.md)
+ - [Django Support](doc/django.md)
```

### Comparing `lona-picocss-0.3.1/lona_picocss.egg-info/SOURCES.txt` & `lona-picocss-0.4/lona_picocss.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 LICENSE.txt
 README.md
 pyproject.toml
 lona_picocss/__init__.py
+lona_picocss/apps.py
+lona_picocss/color_schemes.py
+lona_picocss/middlewares.py
+lona_picocss/navigation.py
+lona_picocss/routes.py
 lona_picocss/settings.py
-lona_picocss/themes.py
+lona_picocss/utils.py
 lona_picocss.egg-info/PKG-INFO
 lona_picocss.egg-info/SOURCES.txt
 lona_picocss.egg-info/dependency_links.txt
 lona_picocss.egg-info/requires.txt
 lona_picocss.egg-info/top_level.txt
 lona_picocss/html/__init__.py
 lona_picocss/html/base.py
@@ -87,21 +92,39 @@
 lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_dark.scss
 lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_light.scss
 lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_styles.scss
 lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_accessibility.scss
 lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_loading.scss
 lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_reduce-motion.scss
 lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_tooltip.scss
+lona_picocss/templates/picocss/403.html
+lona_picocss/templates/picocss/404.html
+lona_picocss/templates/picocss/500.html
 lona_picocss/templates/picocss/base.html
 lona_picocss/templates/picocss/color-scheme.css
 lona_picocss/templates/picocss/disconnect-message.html
 lona_picocss/templates/picocss/footer.html
 lona_picocss/templates/picocss/header.html
 lona_picocss/templates/picocss/waiting-for-server-message.html
+lona_picocss/templates/picocss/django/403.html
+lona_picocss/templates/picocss/django/404.html
+lona_picocss/templates/picocss/django/500.html
+lona_picocss/templates/picocss/django/base.html
+lona_picocss/templates/registration/logged_out.html
+lona_picocss/templates/registration/login.html
+lona_picocss/templates/registration/password_change_done.html
+lona_picocss/templates/registration/password_change_form.html
+lona_picocss/templates/registration/password_reset_complete.html
+lona_picocss/templates/registration/password_reset_confirm.html
+lona_picocss/templates/registration/password_reset_done.html
+lona_picocss/templates/registration/password_reset_form.html
+lona_picocss/templatetags/__init__.py
+lona_picocss/templatetags/lona_picocss_filter.py
 lona_picocss/views/__init__.py
+lona_picocss/views/django_error_views.py
 lona_picocss/views/error_views.py
 lona_picocss/views/it_works.py
 lona_picocss/views/settings.py
 lona_picocss/views/components/__init__.py
 lona_picocss/views/components/buttons.py
 lona_picocss/views/components/cards.py
 lona_picocss/views/components/forms.py
```

### Comparing `lona-picocss-0.3.1/pyproject.toml` & `lona-picocss-0.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
-version = "0.3.1"
+version = "0.4"
 name = "lona-picocss"
 description = "Pico.css bindings for Lona"
 
 authors = [
   { name="Florian Scherf", email="mail@florianscherf.de" },
 ]
 
@@ -34,20 +34,26 @@
 
 [project.optional-dependencies]
 packaging = [
   "build",
   "twine",
 ]
 
-testing = [
+test = [
   "tox",
   "coverage==7.1.0",
   "pytest==7.2.1",
   "pytest-aiohttp==1.0.4",
-  "playwright==1.30.0",
+  "pytest-django==4.5.2",
+  "playwright==1.34.0",
+
+  # django
+  "lona-django==0.1.1",
+  "aiohttp-wsgi==0.10.0",
+  "django>=3.2,<3.3",
 ]
 
 
 [project.urls]
 "Homepage" = "https://github.com/lona-web-org/lona-picocss"
 "Repository" = "https://github.com/lona-web-org/lona-picocss"
 "Bug Tracker" = "https://github.com/lona-web-org/lona-picocss/issues"
```

