# Comparing `tmp/geomanager-0.0.1.tar.gz` & `tmp/geomanager-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomanager-0.0.1.tar", last modified: Tue Jul  4 07:36:50 2023, max compression
+gzip compressed data, was "geomanager-0.0.2.tar", last modified: Thu Jul  6 13:48:50 2023, max compression
```

## Comparing `geomanager-0.0.1.tar` & `geomanager-0.0.2.tar`

### file list

```diff
@@ -1,132 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.640030 geomanager-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-04 07:36:26.000000 geomanager-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-07-04 07:36:50.640030 geomanager-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-07-04 07:36:26.000000 geomanager-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.628029 geomanager-0.0.1/geomanager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    18234 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    39310 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.624029 geomanager-0.0.1/geomanager/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.624029 geomanager-0.0.1/geomanager/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.628029 geomanager-0.0.1/geomanager/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    13802 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.624029 geomanager-0.0.1/geomanager/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.628029 geomanager-0.0.1/geomanager/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12664 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.632029 geomanager-0.0.1/geomanager/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    50516 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/migrations/0002_geomanagersettings_logo_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/migrations/0003_alter_colorvalue_label_alter_colorvalue_threshold_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/migrations/0004_alter_dataset_can_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.632029 geomanager-0.0.1/geomanager/models/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/models/aoi.py
--rw-r--r--   0 runner    (1001) docker     (123)    20079 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/models/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/models/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    24496 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/models/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/models/tile_gl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11450 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/models/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/panels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.624029 geomanager-0.0.1/geomanager/samples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.632029 geomanager-0.0.1/geomanager/samples/basemaps/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/samples/basemaps/basemaps.json
--rw-r--r--   0 runner    (1001) docker     (123)    26170 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/samples/basemaps/style.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.632029 geomanager-0.0.1/geomanager/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/serializers/aoi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/serializers/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/serializers/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/serializers/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/serializers/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/serializers/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.628029 geomanager-0.0.1/geomanager/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.624029 geomanager-0.0.1/geomanager/static/django_large_image/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.624029 geomanager-0.0.1/geomanager/static/django_large_image/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.624029 geomanager-0.0.1/geomanager/static/django_large_image/js/geojs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.632029 geomanager-0.0.1/geomanager/static/django_large_image/js/geojs/1.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/static/django_large_image/js/geojs/1.8.3/geo.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.628029 geomanager-0.0.1/geomanager/static/geomanager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.632029 geomanager-0.0.1/geomanager/static/geomanager/css/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/static/geomanager/css/preview-map.css
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/static/geomanager/css/upload.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.632029 geomanager-0.0.1/geomanager/static/geomanager/css/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)    70412 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/static/geomanager/css/vendor/maplibre-gl.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.632029 geomanager-0.0.1/geomanager/static/geomanager/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15210 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/static/geomanager/images/geomapviewer-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.632029 geomanager-0.0.1/geomanager/static/geomanager/js/
--rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/static/geomanager/js/add-multiple.js
--rw-r--r--   0 runner    (1001) docker     (123)    29056 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/static/geomanager/js/colorbrewer.js
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/static/geomanager/js/mbt_source_extra.js
--rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/static/geomanager/js/raster-preview.js
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/static/geomanager/js/raster_style_extra.js
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/static/geomanager/js/vector-preview.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.636029 geomanager-0.0.1/geomanager/static/geomanager/js/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/static/geomanager/js/vendor/d3-format.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   745424 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/static/geomanager/js/vendor/maplibre-gl.js
--rw-r--r--   0 runner    (1001) docker     (123)   542509 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/static/geomanager/js/vendor/ol.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.636029 geomanager-0.0.1/geomanager/static/geomanager/js/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/static/geomanager/js/widgets/icon_chooser.js
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/static/geomanager/js/widgets/raster_style_widget.js
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/static/geomanager/js/wms-preview.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.628029 geomanager-0.0.1/geomanager/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.628029 geomanager-0.0.1/geomanager/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.628029 geomanager-0.0.1/geomanager/templates/admin/geomanager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.636029 geomanager-0.0.1/geomanager/templates/admin/geomanager/layerrasterfile/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/templates/admin/geomanager/layerrasterfile/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.636029 geomanager-0.0.1/geomanager/templates/django_nextjs/
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/templates/django_nextjs/mapviewer.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.636029 geomanager-0.0.1/geomanager/templates/geomanager/
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/templates/geomanager/boundary_loader.html
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/templates/geomanager/raster_edit_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/templates/geomanager/raster_preview.html
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/templates/geomanager/raster_upload.html
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/templates/geomanager/vector_edit_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/templates/geomanager/vector_preview.html
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/templates/geomanager/vector_upload.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.636029 geomanager-0.0.1/geomanager/templates/geomanager/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/templates/geomanager/widgets/raster_style_widget.html
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/templates/geomanager/wms_preview.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.636029 geomanager-0.0.1/geomanager/templates/modeladmin/
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/templates/modeladmin/index_without_custom_create.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.640030 geomanager-0.0.1/geomanager/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/utils/boundary_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/utils/countries.py
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/utils/raster_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/utils/tile_gl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/utils/vector_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.640030 geomanager-0.0.1/geomanager/views/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/views/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/views/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/views/nextjs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/views/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    20188 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/views/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/views/tile_gl.py
--rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/views/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.640030 geomanager-0.0.1/geomanager/viewsets/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/viewsets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/viewsets/aoi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/viewsets/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/viewsets/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/viewsets/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)    22707 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/wagtail_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-04 07:36:26.000000 geomanager-0.0.1/geomanager/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 07:36:50.628029 geomanager-0.0.1/geomanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-07-04 07:36:50.000000 geomanager-0.0.1/geomanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-07-04 07:36:50.000000 geomanager-0.0.1/geomanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 07:36:50.000000 geomanager-0.0.1/geomanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-04 07:36:50.000000 geomanager-0.0.1/geomanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-04 07:36:50.000000 geomanager-0.0.1/geomanager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-04 07:36:26.000000 geomanager-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-04 07:36:50.640030 geomanager-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:50.013260 geomanager-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-06 13:48:27.000000 geomanager-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-07-06 13:48:50.013260 geomanager-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-06 13:48:27.000000 geomanager-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:49.993259 geomanager-0.0.2/geomanager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18234 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39310 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:49.997259 geomanager-0.0.2/geomanager/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    50516 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/migrations/0002_geomanagersettings_logo_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/migrations/0003_alter_colorvalue_label_alter_colorvalue_threshold_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/migrations/0004_alter_dataset_can_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/migrations/0005_delete_countryboundary_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:49.997259 geomanager-0.0.2/geomanager/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/models/aoi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/models/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/models/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24496 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/models/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/models/tile_gl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10290 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/models/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/panels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:49.989259 geomanager-0.0.2/geomanager/samples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:49.997259 geomanager-0.0.2/geomanager/samples/basemaps/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/samples/basemaps/basemaps.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26170 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/samples/basemaps/style.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:50.001259 geomanager-0.0.2/geomanager/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/serializers/aoi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/serializers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/serializers/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/serializers/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/serializers/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/serializers/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:49.989259 geomanager-0.0.2/geomanager/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:49.989259 geomanager-0.0.2/geomanager/static/django_large_image/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:49.989259 geomanager-0.0.2/geomanager/static/django_large_image/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:49.989259 geomanager-0.0.2/geomanager/static/django_large_image/js/geojs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:50.001259 geomanager-0.0.2/geomanager/static/django_large_image/js/geojs/1.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/static/django_large_image/js/geojs/1.8.3/geo.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:49.989259 geomanager-0.0.2/geomanager/static/geomanager/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:50.001259 geomanager-0.0.2/geomanager/static/geomanager/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/static/geomanager/css/preview-map.css
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/static/geomanager/css/upload.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:50.001259 geomanager-0.0.2/geomanager/static/geomanager/css/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)    70412 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/static/geomanager/css/vendor/maplibre-gl.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:50.001259 geomanager-0.0.2/geomanager/static/geomanager/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15210 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/static/geomanager/images/geomapviewer-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:50.005259 geomanager-0.0.2/geomanager/static/geomanager/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/static/geomanager/js/add-multiple.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29056 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/static/geomanager/js/colorbrewer.js
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/static/geomanager/js/mbt_source_extra.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/static/geomanager/js/raster-preview.js
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/static/geomanager/js/raster_style_extra.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/static/geomanager/js/vector-preview.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:50.005259 geomanager-0.0.2/geomanager/static/geomanager/js/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/static/geomanager/js/vendor/d3-format.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   745424 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/static/geomanager/js/vendor/maplibre-gl.js
+-rw-r--r--   0 runner    (1001) docker     (123)   542509 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/static/geomanager/js/vendor/ol.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:50.005259 geomanager-0.0.2/geomanager/static/geomanager/js/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/static/geomanager/js/widgets/icon_chooser.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/static/geomanager/js/widgets/raster_style_widget.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/static/geomanager/js/wms-preview.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:49.989259 geomanager-0.0.2/geomanager/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:49.989259 geomanager-0.0.2/geomanager/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:49.989259 geomanager-0.0.2/geomanager/templates/admin/geomanager/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:50.005259 geomanager-0.0.2/geomanager/templates/admin/geomanager/layerrasterfile/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/templates/admin/geomanager/layerrasterfile/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:50.005259 geomanager-0.0.2/geomanager/templates/django_nextjs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/templates/django_nextjs/mapviewer.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:50.009259 geomanager-0.0.2/geomanager/templates/geomanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/templates/geomanager/raster_edit_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/templates/geomanager/raster_preview.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/templates/geomanager/raster_upload.html
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/templates/geomanager/vector_edit_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/templates/geomanager/vector_preview.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/templates/geomanager/vector_upload.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:50.009259 geomanager-0.0.2/geomanager/templates/geomanager/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/templates/geomanager/widgets/raster_style_widget.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/templates/geomanager/wms_preview.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:50.009259 geomanager-0.0.2/geomanager/templates/modeladmin/
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/templates/modeladmin/index_without_custom_create.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:50.009259 geomanager-0.0.2/geomanager/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/utils/raster_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/utils/tile_gl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/utils/vector_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:50.013260 geomanager-0.0.2/geomanager/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/views/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/views/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/views/nextjs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/views/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20493 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/views/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/views/tile_gl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11577 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/views/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:50.013260 geomanager-0.0.2/geomanager/viewsets/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/viewsets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/viewsets/aoi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/viewsets/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/viewsets/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/viewsets/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23126 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-06 13:48:27.000000 geomanager-0.0.2/geomanager/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:48:49.997259 geomanager-0.0.2/geomanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-07-06 13:48:49.000000 geomanager-0.0.2/geomanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-06 13:48:49.000000 geomanager-0.0.2/geomanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 13:48:49.000000 geomanager-0.0.2/geomanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-06 13:48:49.000000 geomanager-0.0.2/geomanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 13:48:49.000000 geomanager-0.0.2/geomanager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-06 13:48:27.000000 geomanager-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-06 13:48:50.017259 geomanager-0.0.2/setup.cfg
```

### Comparing `geomanager-0.0.1/PKG-INFO` & `geomanager-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomanager
-Version: 0.0.1
+Version: 0.0.2
 Summary: Wagtail based Geospatial Data Manager
 Home-page: https://github.com/wmo-raf/geomanager
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -97,37 +97,36 @@
 pip install geomanager
 ```
 
 The following packages will be automatically installed when installing `geomanager`, if not already installed.
 
 - wagtail>=4.2.2
 - django_extensions>=3.2.1
-- django-countries>=7.5.1
 - wagtail_color_panel>=1.4.1
 - wagtailfontawesomesvg>=0.0.3,
 - django_json_widget>=1.1.1
 - django_nextjs>= 2.2.2
 - django-allauth>=0.54.0
 - django-large-image>=0.9.0
 - large-image-source-gdal>=1.20.6
 - large-image-source-pil>=1.20.6
 - large-image-source-tiff>=1.20.6
 - django-filter>=22.1
-- geopandas>=0.12.2
 - cftime>=1.6.2
 - netCDF4>=1.6.3
 - rasterio>=1.3.6
 - rio-cogeo>=3.5.1
 - xarray>=2023.3.0
 - rioxarray>=0.14.0
 - shapely>=2.0.1
 - djangorestframework-simplejwt>=5.2.2
 - wagtail-humanitarian-icons>=1.0.3
 - wagtail-icon-chooser>=0.0.1
 - matplotlib>=3.7.1
+- wagtail-cache>=2.2.0
 
 # Usage
 
 Make sure the following are all added to your `INSTALLED_APPS` in your Wagtail `settings`
 
 ````python
 INSTALLED_APPS = [
@@ -138,19 +137,19 @@
     'django_json_widget',
     'django_nextjs',
     "django_filters",
     "wagtail_color_panel",
     "wagtail_adminsortable",
     "wagtailhumanitarianicons",
     "wagtailiconchooser",
-    "django_countries",
     "django_extensions",
     "wagtailfontawesomesvg"
     "allauth",
     "allauth.account",
+    "wagtailcache",
 
     "wagtail.contrib.modeladmin",
     "wagtail.contrib.settings",
     "rest_framework",
     "django.contrib.gis",
 
     ...
@@ -170,14 +169,20 @@
 urlpatterns = [
     ...
     path("", include("geomanager.urls")),
     ...
 ]
 ```
 
+# Wagtail Cache Setup
+
+Geomanager depends on the [wagtail-cache](https://github.com/coderedcorp/wagtail-cache) package for caching requests.
+Please have a look at the [wagtail-cache documentation](https://docs.coderedcorp.com/wagtail-cache/) for setup
+instructions
+
 # Including the Map Viewer
 
 This package is the backend component to the frontend [geomapviewer](https://github.com/wmo-raf/geomapviewer).
 
 # Documentation
 
 TODO
```

### Comparing `geomanager-0.0.1/README.md` & `geomanager-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -76,37 +76,36 @@
 pip install geomanager
 ```
 
 The following packages will be automatically installed when installing `geomanager`, if not already installed.
 
 - wagtail>=4.2.2
 - django_extensions>=3.2.1
-- django-countries>=7.5.1
 - wagtail_color_panel>=1.4.1
 - wagtailfontawesomesvg>=0.0.3,
 - django_json_widget>=1.1.1
 - django_nextjs>= 2.2.2
 - django-allauth>=0.54.0
 - django-large-image>=0.9.0
 - large-image-source-gdal>=1.20.6
 - large-image-source-pil>=1.20.6
 - large-image-source-tiff>=1.20.6
 - django-filter>=22.1
-- geopandas>=0.12.2
 - cftime>=1.6.2
 - netCDF4>=1.6.3
 - rasterio>=1.3.6
 - rio-cogeo>=3.5.1
 - xarray>=2023.3.0
 - rioxarray>=0.14.0
 - shapely>=2.0.1
 - djangorestframework-simplejwt>=5.2.2
 - wagtail-humanitarian-icons>=1.0.3
 - wagtail-icon-chooser>=0.0.1
 - matplotlib>=3.7.1
+- wagtail-cache>=2.2.0
 
 # Usage
 
 Make sure the following are all added to your `INSTALLED_APPS` in your Wagtail `settings`
 
 ````python
 INSTALLED_APPS = [
@@ -117,19 +116,19 @@
     'django_json_widget',
     'django_nextjs',
     "django_filters",
     "wagtail_color_panel",
     "wagtail_adminsortable",
     "wagtailhumanitarianicons",
     "wagtailiconchooser",
-    "django_countries",
     "django_extensions",
     "wagtailfontawesomesvg"
     "allauth",
     "allauth.account",
+    "wagtailcache",
 
     "wagtail.contrib.modeladmin",
     "wagtail.contrib.settings",
     "rest_framework",
     "django.contrib.gis",
 
     ...
@@ -149,14 +148,20 @@
 urlpatterns = [
     ...
     path("", include("geomanager.urls")),
     ...
 ]
 ```
 
+# Wagtail Cache Setup
+
+Geomanager depends on the [wagtail-cache](https://github.com/coderedcorp/wagtail-cache) package for caching requests.
+Please have a look at the [wagtail-cache documentation](https://docs.coderedcorp.com/wagtail-cache/) for setup
+instructions
+
 # Including the Map Viewer
 
 This package is the backend component to the frontend [geomapviewer](https://github.com/wmo-raf/geomapviewer).
 
 # Documentation
 
 TODO
```

### Comparing `geomanager-0.0.1/geomanager/apps.py` & `geomanager-0.0.2/geomanager/apps.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/blocks.py` & `geomanager-0.0.2/geomanager/blocks.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/constants.py` & `geomanager-0.0.2/geomanager/constants.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/errors.py` & `geomanager-0.0.2/geomanager/errors.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/fields.py` & `geomanager-0.0.2/geomanager/fields.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/forms.py` & `geomanager-0.0.2/geomanager/forms.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/helpers.py` & `geomanager-0.0.2/geomanager/helpers.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/migrations/0001_initial.py` & `geomanager-0.0.2/geomanager/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/migrations/0002_geomanagersettings_logo_and_more.py` & `geomanager-0.0.2/geomanager/migrations/0002_geomanagersettings_logo_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/migrations/0003_alter_colorvalue_label_alter_colorvalue_threshold_and_more.py` & `geomanager-0.0.2/geomanager/migrations/0003_alter_colorvalue_label_alter_colorvalue_threshold_and_more.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/migrations/0004_alter_dataset_can_clip.py` & `geomanager-0.0.2/geomanager/migrations/0004_alter_dataset_can_clip.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/models/aoi.py` & `geomanager-0.0.2/geomanager/models/aoi.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/models/core.py` & `geomanager-0.0.2/geomanager/models/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import uuid
 
 from django.db import models
 from django.utils.translation import gettext_lazy as _
-from django_countries.fields import CountryField
-from django_countries.widgets import CountrySelectWidget
 from django_extensions.db.models import TimeStampedModel
 from modelcluster.fields import ParentalKey
 from modelcluster.models import ClusterableModel
 from wagtail import blocks
 from wagtail.admin.panels import (
     FieldPanel,
     TabbedInterface,
@@ -367,15 +365,14 @@
                                                     help_text=_(
                                                         "Refresh cap alerts on the map after this minutes. Leave blank "
                                                         "to disable auto refreshing"))
     cap_shown_by_default = models.BooleanField(default=True, verbose_name=_("CAP layer shown by default"),
                                                help_text=_("CAP Layer shown on map by default"))
     cap_metadata = models.ForeignKey(Metadata, on_delete=models.SET_NULL, blank=True, null=True,
                                      verbose_name=_("Metadata"))
-    country = CountryField(blank_label=_("Select Country"), verbose_name=_("country"))
     gadm_version = models.CharField(max_length=50, choices=GADM_VERSION, default="4.1",
                                     verbose_name=_("GADM Boundary Data Version"),
                                     help_text=_(
                                         "It is encouraged to use the latest version. "
                                         "See available versions here: https://gadm.org/old_versions.html"))
     tile_gl_fonts_url = models.URLField(max_length=256,
                                         default="https://fonts.openmaptiles.org/{fontstack}/{range}.pbf",
@@ -422,18 +419,14 @@
             FieldPanel("cap_base_url"),
             FieldPanel("cap_sub_category"),
             FieldPanel("cap_auto_refresh_interval"),
             FieldPanel("cap_shown_by_default"),
             FieldPanel("cap_metadata"),
         ], heading=_("CAP Layer Settings")),
         ObjectList([
-            FieldPanel("country", widget=CountrySelectWidget()),
-            FieldPanel("gadm_version"),
-        ], heading=_("Region Settings")),
-        ObjectList([
             FieldPanel("logo"),
             FieldPanel("navigation"),
         ], heading=_("Branding Settings")),
     ])
 
     @property
     def cap_auto_refresh_interval_milliseconds(self):
```

### Comparing `geomanager-0.0.1/geomanager/models/profile.py` & `geomanager-0.0.2/geomanager/models/profile.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/models/raster.py` & `geomanager-0.0.2/geomanager/models/raster.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/models/tile_gl.py` & `geomanager-0.0.2/geomanager/models/tile_gl.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/models/vector.py` & `geomanager-0.0.2/geomanager/models/vector.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,66 +18,26 @@
 from geomanager.helpers import get_vector_layer_files_url
 from geomanager.models import Dataset
 from geomanager.models.core import BaseLayer
 from geomanager.panels import ReadOnlyFieldPanel
 from geomanager.utils.vector_utils import drop_vector_table
 
 
-class CountryBoundary(TimeStampedModel):
-    name_0 = models.CharField(max_length=100, blank=True, null=True)
-    name_1 = models.CharField(max_length=100, blank=True, null=True)
-    name_2 = models.CharField(max_length=100, blank=True, null=True)
-    gid_0 = models.CharField(max_length=100, blank=True, null=True)
-    gid_1 = models.CharField(max_length=100, blank=True, null=True)
-    gid_2 = models.CharField(max_length=100, blank=True, null=True)
-    level = models.IntegerField(blank=True, null=True)
-    size = models.CharField(max_length=100, blank=True, null=True)
-
-    geom = models.MultiPolygonField(srid=4326)
-
-    class Meta:
-        verbose_name_plural = _("Country Boundaries")
-
-    def __str__(self):
-        return str(self.pk)
-
-    @property
-    def bbox(self):
-        min_x, min_y, max_x, max_y = self.geom.envelope.extent
-        bbox = [min_x, min_y, max_x, max_y]
-        return bbox
-
-    @property
-    def info(self):
-        info = {"iso": self.gid_0}
-
-        if self.level == 0:
-            info.update({"name": self.name_0})
-
-        if self.level == 1:
-            gid_1 = self.gid_1.split(".")[1].split("_")[0]
-            info.update({"id1": gid_1, "name": self.name_1})
-
-        if self.level == 2:
-            gid_1 = self.gid_1.split(".")[1].split("_")[0]
-            gid_2 = self.gid_1.split(".")[1].split("_")[1]
-            info.update({"id1": gid_1, "id2": gid_2, "name": self.name_2})
-
-        return info
-
-
 class Geostore(TimeStampedModel):
     id = models.UUIDField(primary_key=True, default=uuid.uuid4, editable=False)
     iso = models.CharField(max_length=100, blank=True, null=True)
     id1 = models.CharField(max_length=100, blank=True, null=True)
     id2 = models.CharField(max_length=100, blank=True, null=True)
+    id3 = models.CharField(max_length=100, blank=True, null=True)
 
     name_0 = models.CharField(max_length=100, blank=True, null=True)
     name_1 = models.CharField(max_length=100, blank=True, null=True)
     name_2 = models.CharField(max_length=100, blank=True, null=True)
+    name_3 = models.CharField(max_length=100, blank=True, null=True)
+    name_4 = models.CharField(max_length=100, blank=True, null=True)
 
     geom = models.MultiPolygonField(srid=4326)
 
     def __str__(self):
         return self.id.hex
 
     @property
@@ -96,14 +56,17 @@
 
         if self.id1:
             info.update({"id1": self.id1, "name": self.name_1})
 
         if self.id2:
             info.update({"id2": self.id2, "name": self.name_2})
 
+        if self.id3:
+            info.update({"id3": self.id3, "name": self.id3})
+
         return info
 
 
 class VectorLayer(TimeStampedModel, BaseLayer):
     dataset = models.ForeignKey(Dataset, on_delete=models.CASCADE, related_name="vector_layers", verbose_name="dataset")
     render_layers = StreamField([
         ("fill", FillVectorLayerBlock(label=_("Polygon Layer"))),
```

### Comparing `geomanager-0.0.1/geomanager/samples/basemaps/basemaps.json` & `geomanager-0.0.2/geomanager/samples/basemaps/basemaps.json`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/samples/basemaps/style.json` & `geomanager-0.0.2/geomanager/samples/basemaps/style.json`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/serializers/aoi.py` & `geomanager-0.0.2/geomanager/serializers/aoi.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/serializers/auth.py` & `geomanager-0.0.2/geomanager/serializers/auth.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/serializers/core.py` & `geomanager-0.0.2/geomanager/serializers/core.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/serializers/profile.py` & `geomanager-0.0.2/geomanager/serializers/profile.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/serializers/raster.py` & `geomanager-0.0.2/geomanager/serializers/raster.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/serializers/vector.py` & `geomanager-0.0.2/geomanager/serializers/vector.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+from adminboundarymanager.models import AdminBoundary
 from rest_framework import serializers
 
 from geomanager.models.vector import (
     PgVectorTable,
     VectorLayer,
-    CountryBoundary, Geostore
+    Geostore
 )
 from geomanager.utils.vector_utils import create_feature_collection_from_geom
 
 
-class CountrySerializer(serializers.ModelSerializer):
+class AdminBoundarySerializer(serializers.ModelSerializer):
     bbox = serializers.ListField()
 
     class Meta:
-        model = CountryBoundary
+        model = AdminBoundary
         fields = ("level", "name_0", "name_1", "name_2", "gid_0", "gid_1", "gid_2", "size", "bbox")
 
 
 class BoundsFieldSerializer(serializers.Field):
     def to_representation(self, value):
         # Convert the value of the custom field to a string for serialization
         return [float(value) for value in list(value)]
```

### Comparing `geomanager-0.0.1/geomanager/static/geomanager/css/vendor/maplibre-gl.css` & `geomanager-0.0.2/geomanager/static/geomanager/css/vendor/maplibre-gl.css`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/static/geomanager/images/geomapviewer-logo.png` & `geomanager-0.0.2/geomanager/static/geomanager/images/geomapviewer-logo.png`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/static/geomanager/js/add-multiple.js` & `geomanager-0.0.2/geomanager/static/geomanager/js/add-multiple.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/static/geomanager/js/colorbrewer.js` & `geomanager-0.0.2/geomanager/static/geomanager/js/colorbrewer.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/static/geomanager/js/mbt_source_extra.js` & `geomanager-0.0.2/geomanager/static/geomanager/js/mbt_source_extra.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/static/geomanager/js/raster-preview.js` & `geomanager-0.0.2/geomanager/static/geomanager/js/raster-preview.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/static/geomanager/js/raster_style_extra.js` & `geomanager-0.0.2/geomanager/static/geomanager/js/raster_style_extra.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/static/geomanager/js/vector-preview.js` & `geomanager-0.0.2/geomanager/static/geomanager/js/vector-preview.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/static/geomanager/js/vendor/d3-format.min.js` & `geomanager-0.0.2/geomanager/static/geomanager/js/vendor/d3-format.min.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/static/geomanager/js/vendor/maplibre-gl.js` & `geomanager-0.0.2/geomanager/static/geomanager/js/vendor/maplibre-gl.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/static/geomanager/js/vendor/ol.min.js` & `geomanager-0.0.2/geomanager/static/geomanager/js/vendor/ol.min.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/static/geomanager/js/widgets/icon_chooser.js` & `geomanager-0.0.2/geomanager/static/geomanager/js/widgets/icon_chooser.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/static/geomanager/js/widgets/raster_style_widget.js` & `geomanager-0.0.2/geomanager/static/geomanager/js/widgets/raster_style_widget.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/static/geomanager/js/wms-preview.js` & `geomanager-0.0.2/geomanager/static/geomanager/js/wms-preview.js`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/templates/django_nextjs/mapviewer.html` & `geomanager-0.0.2/geomanager/templates/django_nextjs/mapviewer.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/templates/geomanager/raster_edit_form.html` & `geomanager-0.0.2/geomanager/templates/geomanager/raster_edit_form.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/templates/geomanager/raster_preview.html` & `geomanager-0.0.2/geomanager/templates/geomanager/raster_preview.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/templates/geomanager/raster_upload.html` & `geomanager-0.0.2/geomanager/templates/geomanager/raster_upload.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/templates/geomanager/vector_edit_form.html` & `geomanager-0.0.2/geomanager/templates/geomanager/vector_edit_form.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/templates/geomanager/vector_preview.html` & `geomanager-0.0.2/geomanager/templates/geomanager/vector_preview.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/templates/geomanager/vector_upload.html` & `geomanager-0.0.2/geomanager/templates/geomanager/vector_upload.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/templates/geomanager/widgets/raster_style_widget.html` & `geomanager-0.0.2/geomanager/templates/geomanager/widgets/raster_style_widget.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/templates/geomanager/wms_preview.html` & `geomanager-0.0.2/geomanager/templates/geomanager/wms_preview.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/templates/modeladmin/index_without_custom_create.html` & `geomanager-0.0.2/geomanager/templates/modeladmin/index_without_custom_create.html`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/urls.py` & `geomanager-0.0.2/geomanager/urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 from geomanager.views import (
     RasterTileView,
     VectorTileView,
     map_view,
     RegisterView,
     ResetPasswordView,
-    BoundaryVectorTileView,
     tile_gl,
     tile_json_gl,
     style_json_gl,
     get_mapviewer_config,
     GeoJSONPgTableView
 )
 from geomanager.views.auth import (
@@ -32,15 +31,15 @@
     RasterDataGeostoreTimeseriesView
 )
 from geomanager.viewsets import (
     FileImageLayerRasterFileDetailViewSet,
     VectorTableFileDetailViewSet,
     DatasetListViewSet,
     GeostoreViewSet,
-    CountryBoundaryViewSet,
+    AdminBoundaryViewSet,
     MetadataViewSet
 )
 from geomanager.viewsets.aoi import AoiViewSet
 
 router = SimpleRouter(trailing_slash=False)
 
 router.register(r'api/datasets', DatasetListViewSet)
@@ -78,19 +77,19 @@
 
                   # # User Areas of Interest
                   # path('api/aoi/<int:user_id>', get_user_aoi_list, name='get_user_aoi_list'),
                   # path('api/aoi/', create_aoi, name='create_user_aoi'),
                   # path('api/aoi/', create_aoi, name='create_user_aoi'),
 
                   # Country
-                  path(r'api/country', CountryBoundaryViewSet.as_view({"get": "get"}), name="country_list"),
-                  path(r'api/country/<str:gid_0>', CountryBoundaryViewSet.as_view({"get": "get_regions"}),
+                  path(r'api/country', AdminBoundaryViewSet.as_view({"get": "get"}), name="country_list"),
+                  path(r'api/country/<str:gid_0>', AdminBoundaryViewSet.as_view({"get": "get_regions"}),
                        name="country_regions"),
                   path(r'api/country/<str:gid_0>/<str:gid_1>',
-                       CountryBoundaryViewSet.as_view({"get": "get_sub_regions"}),
+                       AdminBoundaryViewSet.as_view({"get": "get_sub_regions"}),
                        name="country_sub_regions"),
 
                   # Geostore
                   path(r'api/geostore/', GeostoreViewSet.as_view({"post": "post"}), name="geostore"),
                   path(r'api/geostore/<uuid:geostore_id>', GeostoreViewSet.as_view({"get": "get"}),
                        name="get_by_geostore"),
                   path(r'api/geostore/admin/<str:gid_0>', GeostoreViewSet.as_view({"get": "get_by_admin"}),
@@ -101,17 +100,14 @@
                        GeostoreViewSet.as_view({"get": "get_by_admin"}),
                        name="get_by_gid2"),
 
                   # Tiles
                   path(r'api/raster-tiles/<int:z>/<int:x>/<int:y>', RasterTileView.as_view(), name="raster_tiles"),
                   path(r'api/vector-tiles/<int:z>/<int:x>/<int:y>', cache_page(3600)(VectorTileView.as_view()),
                        name="vector_tiles"),
-                  path(r'api/boundary-tiles/<int:z>/<int:x>/<int:y>',
-                       BoundaryVectorTileView.as_view(),
-                       name="boundary_tiles"),
 
                   # Data
                   path(r'api/raster-data/pixel', RasterDataPixelView.as_view(), name="raster_data_pixel"),
                   path(r'api/raster-data/pixel/timeseries', RasterDataPixelTimeseriesView.as_view(),
                        name="raster_data_pixel_timeseries"),
 
                   path(r'api/raster-data/geostore', RasterDataGeostoreView.as_view(), name="raster_data_geostore"),
@@ -125,8 +121,9 @@
                   # Tiles GL
                   path(r'api/tile-gl/tile/<str:source_slug>/<int:z>/<int:x>/<int:y>.pbf', tile_gl, name="tile_gl"),
                   path(r'api/tile-gl/tile-json/<str:source_slug>.json', tile_json_gl, name="tile_json_gl"),
                   path(r'api/tile-gl/style/<str:source_slug>.json', style_json_gl, name="style_json_gl"),
 
                   # Additional, standalone URLs from django-large-image
                   path('', include('django_large_image.urls')),
+                  path('', include('adminboundarymanager.urls')),
               ] + router.urls
```

### Comparing `geomanager-0.0.1/geomanager/utils/raster_utils.py` & `geomanager-0.0.2/geomanager/utils/raster_utils.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/utils/tile_gl.py` & `geomanager-0.0.2/geomanager/utils/tile_gl.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/utils/vector_utils.py` & `geomanager-0.0.2/geomanager/utils/vector_utils.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/views/__init__.py` & `geomanager-0.0.2/geomanager/views/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     delete_raster_upload,
     RasterTileView,
     preview_raster_layers,
     preview_wms_layers
 )
 from .tile_gl import tile_gl, tile_json_gl, style_json_gl
 from .vector import (
-    load_boundary,
     upload_vector_file,
     publish_vector,
     delete_vector_upload,
     preview_vector_layers,
     VectorTileView,
-    BoundaryVectorTileView,
     GeoJSONPgTableView
 )
```

### Comparing `geomanager-0.0.1/geomanager/views/auth.py` & `geomanager-0.0.2/geomanager/views/auth.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/views/core.py` & `geomanager-0.0.2/geomanager/views/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,46 @@
+from adminboundarymanager.models import AdminBoundarySettings
 from rest_framework.decorators import api_view
 from rest_framework.response import Response
+from wagtailcache.cache import cache_page
 
 from geomanager.models import Category
 from geomanager.models.core import GeomanagerSettings
 from geomanager.serializers import CategorySerializer
-from geomanager.utils.countries import get_country_info
 
 
 @api_view(['GET'])
+@cache_page
 def get_mapviewer_config(request):
-    settings = GeomanagerSettings.for_request(request)
+    gm_settings = GeomanagerSettings.for_request(request)
+    abm_settings = AdminBoundarySettings.for_request(request)
 
     categories = Category.objects.all()
     categories_data = CategorySerializer(categories, many=True).data
     response = {
         "categories": categories_data,
     }
 
-    if settings.logo:
-        response.update({"logo": request.build_absolute_uri(settings.logo.file.url)})
-
-    if settings.country:
-        country_iso = settings.country.alpha3
-        country_data = {
-            "iso": country_iso
-        }
-        country_info = get_country_info(country_iso)
-        if country_info:
-            country_data.update(**country_info)
-        country_data.update({"name": settings.country.name})
+    if gm_settings.logo:
+        response.update({"logo": request.build_absolute_uri(gm_settings.logo.file.url)})
 
+    if abm_settings.countries_list:
         response.update({
-            "country": country_data
+            "countries": abm_settings.countries_list,
+            "bounds": abm_settings.combined_countries_bounds,
+            "boundaryDataSource": abm_settings.data_source
         })
 
     base_maps_data = []
 
-    tile_gl_source = settings.tile_gl_source
+    tile_gl_source = gm_settings.tile_gl_source
 
     if tile_gl_source:
         # get base maps
-        for base_map in settings.base_maps:
+        for base_map in gm_settings.base_maps:
             data = base_map.block.get_api_representation(base_map.value)
             for key, value in base_map.value.items():
                 if key == "image" and value:
                     data.update({"image": request.build_absolute_uri(value.file.url)})
 
             data.update({"mapStyle": request.build_absolute_uri(tile_gl_source.map_style_url)})
             base_maps_data.append(data)
```

### Comparing `geomanager-0.0.1/geomanager/views/profile.py` & `geomanager-0.0.2/geomanager/views/profile.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/views/raster.py` & `geomanager-0.0.2/geomanager/views/raster.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,30 @@
 from django.core.exceptions import ValidationError, ObjectDoesNotExist
 from django.http import JsonResponse, HttpResponse
 from django.shortcuts import get_object_or_404, render
 from django.template.defaultfilters import filesizeformat
 from django.template.loader import render_to_string
 from django.urls import reverse
 from django.utils import timezone
+from django.utils.decorators import method_decorator
 from django.utils.translation import gettext_lazy as _
 from django_large_image import tilesource
 from large_image.exceptions import TileSourceXYZRangeError
 from rest_framework.request import Request
 from rest_framework.response import Response
 from rest_framework.views import APIView
 from wagtail.admin.auth import (
     user_passes_test,
     user_has_any_page_permission,
     permission_denied
 )
 from wagtail.contrib.modeladmin.helpers import AdminURLHelper
 from wagtail.models import Site
 from wagtail.snippets.permissions import get_permission_name
+from wagtailcache.cache import cache_page
 
 from geomanager.errors import RasterFileNotFound, QueryParamRequired, GeostoreNotFound
 from geomanager.forms import LayerRasterFileForm
 from geomanager.models import (
     Dataset,
     RasterUpload,
     FileImageLayer,
@@ -428,14 +430,15 @@
     def get_raster_geostore_data(self, raster_file, geostore, value_type):
         geostore_data = get_geostore_data(raster_file.file, geostore)
 
     def get_query_param(self, request: Request, key: str, default: Optional[Any] = '') -> str:
         return request.query_params.get(key, str(default))
 
 
+@method_decorator(cache_page, name='get')
 class RasterTileView(RasterDataMixin, APIView):
     # TODO: Validate style query param thoroughly. If not validated, the whole app just exits without warning.
     # TODO: Cache getting layer style. We should not be querying the database each time for style
     def get(self, request, z, x, y):
         try:
             raster_file = self.get_single_raster_file(request)
         except QueryParamRequired as e:
@@ -483,26 +486,28 @@
             raise ValidationError(e)
 
         mime_type = source.getTileMimeType()
 
         return HttpResponse(tile_binary, content_type=mime_type)
 
 
+@method_decorator(cache_page, name='get')
 class RasterDataPixelView(RasterDataMixin, APIView):
     def get(self, request):
         try:
             pixel_data = self.get_pixel_data(request)
         except QueryParamRequired as e:
             return JsonResponse(e.serialize, status=400)
         except RasterFileNotFound as e:
             return JsonResponse({"message": e}, status=404)
 
         return Response(pixel_data)
 
 
+@method_decorator(cache_page, name='get')
 class RasterDataPixelTimeseriesView(RasterDataMixin, APIView):
     def get(self, request):
         try:
             raster_files = self.get_multiple_raster_files(request)
             x_coord, y_coord = self.get_coords(request)
         except QueryParamRequired as e:
             return JsonResponse(e.serialize, status=400)
@@ -514,28 +519,30 @@
         for raster_file in raster_files:
             pixel_data = get_raster_pixel_data(raster_file.file, x_coord, y_coord)
             timeseries_data.append({"date": raster_file.time, "value": pixel_data})
 
         return Response(timeseries_data)
 
 
+@method_decorator(cache_page, name='get')
 class RasterDataGeostoreView(RasterDataMixin, APIView):
     def get(self, request):
         try:
             value_type = self.get_query_param(request, "value_type")
             geostore = self.get_geostore(request)
             raster_file = self.get_single_raster_file(request)
             data = get_geostore_data(raster_file.file, geostore, value_type)
         except QueryParamRequired as e:
             return JsonResponse(e.serialize, status=400)
         except (RasterFileNotFound, GeostoreNotFound) as e:
             return JsonResponse({"message": e}, status=404)
         return Response(data)
 
 
+@method_decorator(cache_page, name='get')
 class RasterDataGeostoreTimeseriesView(RasterDataMixin, APIView):
     def get(self, request):
         try:
             value_type = self.get_query_param(request, "value_type")
             raster_files = self.get_multiple_raster_files(request)
             geostore = self.get_geostore(request)
         except QueryParamRequired as e:
```

### Comparing `geomanager-0.0.1/geomanager/views/tile_gl.py` & `geomanager-0.0.2/geomanager/views/tile_gl.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from django.http import HttpResponse, JsonResponse
 from django.urls import reverse
-from django.views.decorators.cache import cache_control
+from wagtailcache.cache import cache_page
 
 from geomanager.errors import MissingTileError
 from geomanager.models import MBTSource
 from geomanager.utils.tile_gl import center_from_bounds, open_mbtiles
 
 DEFAULT_ZOOM = 13
 DEFAULT_MINZOOM = 7
 DEFAULT_MAXZOOM = 15
 WORLD_BOUNDS = [-180, -85.05112877980659, 180, 85.0511287798066]
 
-MONTH_SECONDS = 60 * 60 * 24 * 30
 
-
-@cache_control(max_age=MONTH_SECONDS)
+@cache_page
 def tile_gl(request, source_slug, z, x, y):
     source = MBTSource.objects.get(slug=source_slug)
     with (open_mbtiles(source.file.path)) as mbtiles:
         try:
             data = mbtiles.tile(z, x, y)
             response = HttpResponse(
                 content=data,
@@ -31,14 +29,15 @@
 
         except MissingTileError:
             return HttpResponse(
                 status=204,
             )
 
 
+@cache_page
 def tile_json_gl(request, source_slug):
     source = MBTSource.objects.get(slug=source_slug)
     with open_mbtiles(source.file.path) as mbtiles:
         metadata = mbtiles.metadata()
 
         # Load valid tilejson keys from the mbtiles metadata
         valid_tilejson_keys = (
@@ -72,25 +71,26 @@
         spec["bounds"] = spec.get("bounds", WORLD_BOUNDS)
         spec["minzoom"] = spec.get("minzoom", DEFAULT_MINZOOM)
         spec["maxzoom"] = spec.get("maxzoom", DEFAULT_MINZOOM)
         spec["center"] = spec.get(
             "center", center_from_bounds(spec["bounds"], DEFAULT_ZOOM)
         )
 
-        # Tile defintions
+        # Tile
         tile_url = request.build_absolute_uri(reverse("tile_gl", args=(source.slug, 0, 0, 0)))
         tile_url = tile_url.replace("/0/0/0.pbf", r"/{z}/{x}/{y}.pbf")
         spec["tiles"] = [tile_url]
 
-        # Version defintion
+        # Version
         spec["tilejson"] = "3.0.0"
 
         return JsonResponse(spec)
 
 
+@cache_page
 def style_json_gl(request, source_slug):
     source = MBTSource.objects.get(slug=source_slug)
     tilejson_url = request.build_absolute_uri(reverse("tile_json_gl", args=[source.slug]))
 
     style_config = source.json_style
 
     style_config["id"] = source.pk
```

### Comparing `geomanager-0.0.1/geomanager/views/vector.py` & `geomanager-0.0.2/geomanager/views/vector.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,99 +1,37 @@
 import os
-import tempfile
 
 from django.conf import settings
 from django.core.exceptions import ObjectDoesNotExist
 from django.db import connection, close_old_connections
 from django.http import JsonResponse, Http404, HttpResponse
-from django.shortcuts import get_object_or_404, render, redirect
+from django.shortcuts import get_object_or_404, render
 from django.template.defaultfilters import filesizeformat
 from django.template.loader import render_to_string
 from django.urls import reverse
+from django.utils.decorators import method_decorator
 from django.utils.translation import gettext_lazy as _
 from django.views import View
-from wagtail.admin import messages
 from wagtail.admin.auth import user_passes_test, user_has_any_page_permission, permission_denied
 from wagtail.contrib.modeladmin.helpers import AdminURLHelper
 from wagtail.models import Site
 from wagtail.snippets.permissions import get_permission_name
+from wagtailcache.cache import cache_page
 
-from geomanager.forms import VectorLayerFileForm, BoundaryUploadForm
+from geomanager.forms import VectorLayerFileForm
 from geomanager.models import Dataset
 from geomanager.models.core import GeomanagerSettings
-from geomanager.models.vector import VectorLayer, VectorUpload, PgVectorTable, CountryBoundary
+from geomanager.models.vector import VectorLayer, VectorUpload, PgVectorTable
 from geomanager.settings import geomanager_settings
-from geomanager.utils.boundary_loader import load_country_boundary
 from geomanager.utils.vector_utils import ogr_db_import
 
 ALLOWED_VECTOR_EXTENSIONS = ["zip", "geojson", "csv"]
 
 
 @user_passes_test(user_has_any_page_permission)
-def load_boundary(request):
-    template = "geomanager/boundary_loader.html"
-
-    lm_settings = GeomanagerSettings.for_request(request)
-    country = lm_settings.country
-    gadm_version = lm_settings.gadm_version
-    context = {"country": country}
-
-    settings_url = reverse(
-        "wagtailsettings:edit",
-        args=[GeomanagerSettings._meta.app_label, GeomanagerSettings._meta.model_name, ],
-    )
-
-    context.update({"settings_url": settings_url})
-
-    if request.POST:
-        form = BoundaryUploadForm(request.POST, request.FILES)
-
-        if form.is_valid():
-            geopackage = form.cleaned_data.get("geopackage")
-            remove_existing = form.cleaned_data.get("remove_existing")
-
-            if not country:
-                form.add_error(None, "Please select a country in layer manager settings and try again")
-
-            with tempfile.NamedTemporaryFile(delete=False, suffix=f"_{geopackage.name}") as temp_file:
-                for chunk in geopackage.chunks():
-                    temp_file.write(chunk)
-
-                try:
-                    load_country_boundary(geopackage_path=temp_file.name,
-                                          country_iso=country.alpha3,
-                                          gadm_version=gadm_version,
-                                          remove_existing=remove_existing)
-                except Exception as e:
-                    form.add_error(None, str(e))
-                    context.update({"form": form, "has_error": True})
-                    countries = CountryBoundary.objects.filter(level=0)
-
-                    if countries.exists():
-                        context.update({"existing_countries": countries})
-
-                    return render(request, template_name=template, context=context)
-
-            messages.success(request, "Boundary data loaded successfully")
-            return redirect(reverse("wagtailadmin_home"))
-        else:
-            context.update({"form": form})
-            return render(request, template_name=template, context=context)
-    else:
-        countries = CountryBoundary.objects.filter(level=0)
-        if countries.exists():
-            context["existing_countries"] = countries
-
-        form = BoundaryUploadForm()
-        context["form"] = form
-
-        return render(request, template_name=template, context=context)
-
-
-@user_passes_test(user_has_any_page_permission)
 def upload_vector_file(request, dataset_id=None, layer_id=None):
     permission = get_permission_name('change', Dataset)
     if not request.user.has_perm(permission):
         return permission_denied(request)
 
     site = Site.objects.get(is_default_site=True)
     layer_manager_settings = GeomanagerSettings.for_site(site)
@@ -310,14 +248,15 @@
         "data_vector_api_base_url": request.build_absolute_uri("/api/vector-data"),
         "vector_tiles_url": base_absolute_url + "/api/vector-tiles/{z}/{x}/{y}",
     }
 
     return render(request, 'geomanager/vector_preview.html', context)
 
 
+@method_decorator(cache_page, name='get')
 class VectorTileView(View):
     def get(self, request, z, x, y):
         table_name = request.GET.get("table_name")
 
         if table_name is None:
             return HttpResponse("Missing table_name query parameter", status=400)
 
@@ -349,43 +288,15 @@
             tile = cursor.fetchone()[0]
             if not len(tile):
                 raise Http404()
 
         return HttpResponse(tile, content_type="application/x-protobuf")
 
 
-class BoundaryVectorTileView(View):
-    def get(self, request, z, x, y):
-        gid_0 = request.GET.get("gid_0")
-        boundary_filter = ""
-        if gid_0:
-            boundary_filter = f"AND t.gid_0='{gid_0}'"
-
-        sql = f"""WITH
-            bounds AS (
-              SELECT ST_TileEnvelope({z}, {x}, {y}) AS geom
-            ),
-            mvtgeom AS (
-              SELECT ST_AsMVTGeom(ST_Transform(t.geom, 3857), bounds.geom) AS geom,
-                *
-              FROM geomanager_countryboundary t, bounds
-              WHERE ST_Intersects(ST_Transform(t.geom, 4326), ST_Transform(bounds.geom, 4326)) {boundary_filter}
-            )
-            SELECT ST_AsMVT(mvtgeom, 'default') FROM mvtgeom;
-            """
-        close_old_connections()
-        with connection.cursor() as cursor:
-            cursor.execute(sql)
-            tile = cursor.fetchone()[0]
-            if not len(tile):
-                raise Http404()
-
-        return HttpResponse(tile, content_type="application/x-protobuf")
-
-
+@method_decorator(cache_page, name='get')
 class GeoJSONPgTableView(View):
     def get(self, request, table_name):
         try:
             vector_table = PgVectorTable.objects.get(table_name=table_name)
         except ObjectDoesNotExist:
             return JsonResponse({"message": f"Table with name: '{table_name}' does not exist"}, status=404)
```

### Comparing `geomanager-0.0.1/geomanager/viewsets/aoi.py` & `geomanager-0.0.2/geomanager/viewsets/aoi.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/viewsets/core.py` & `geomanager-0.0.2/geomanager/viewsets/core.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-from django.urls import reverse
+from adminboundarymanager.models import AdminBoundarySettings
+from django.utils.decorators import method_decorator
 from rest_framework import mixins, viewsets
 from rest_framework.response import Response
+from wagtailcache.cache import cache_page
 
 from geomanager import serializers
 from geomanager.models import Dataset
 from geomanager.models.core import GeomanagerSettings, Metadata
 
 
 class DatasetListViewSet(mixins.ListModelMixin, viewsets.GenericViewSet):
@@ -12,14 +14,15 @@
     serializer_class = serializers.DatasetSerializer
 
     def get_serializer_context(self):
         context = super().get_serializer_context()
         context.update({'request': self.request})
         return context
 
+    @method_decorator(cache_page)
     def list(self, request, *args, **kwargs):
         queryset = self.get_queryset()
         dataset_with_layers = []
 
         icons = []
 
         # get only datasets with layers defined
@@ -41,20 +44,21 @@
                                     icons.append(icon)
 
                 dataset_with_layers.append(dataset)
 
         serializer = self.get_serializer(dataset_with_layers, many=True)
 
         lm_settings = GeomanagerSettings.for_request(request)
+        abm_settings = AdminBoundarySettings.for_request(request)
         datasets = serializer.data
         config = {}
 
         # set boundaries url. This will be used to create base boundary layer
-        boundary_tiles_url = request.build_absolute_uri(reverse("boundary_tiles", args=(0, 0, 0)))
-        boundary_tiles_url = boundary_tiles_url.replace("/0/0/0", r"/{z}/{x}/{y}")
+        boundary_tiles_url = abm_settings.boundary_tiles_url
+        boundary_tiles_url = request.scheme + '://' + request.get_host() + boundary_tiles_url
         config.update({"boundaryTilesUrl": boundary_tiles_url})
 
         # set cap layer configuration. This will be used to create cap layer
         if lm_settings.cap_base_url and lm_settings.cap_sub_category:
             config.update({
                 "capConfig": {
                     "initialVisible": lm_settings.cap_shown_by_default,
@@ -64,10 +68,11 @@
                     "refreshInterval": lm_settings.cap_auto_refresh_interval_milliseconds,
                     "metadata": lm_settings.cap_metadata.pk if lm_settings.cap_metadata else None
                 }})
 
         return Response({"datasets": datasets, "config": config, "icons": icons})
 
 
+@method_decorator(cache_page, name="retrieve")
 class MetadataViewSet(mixins.RetrieveModelMixin, viewsets.GenericViewSet):
     queryset = Metadata.objects.all()
     serializer_class = serializers.MetadataSerialiazer
```

### Comparing `geomanager-0.0.1/geomanager/viewsets/raster.py` & `geomanager-0.0.2/geomanager/viewsets/raster.py`

 * *Files identical despite different names*

### Comparing `geomanager-0.0.1/geomanager/viewsets/vector.py` & `geomanager-0.0.2/geomanager/viewsets/vector.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,54 @@
 import json
 
+from adminboundarymanager.models import AdminBoundary, AdminBoundarySettings
 from django.contrib.gis.geos import GEOSGeometry
 from django.contrib.gis.geos import MultiPolygon
+from django.utils.decorators import method_decorator
 from django_filters.rest_framework import DjangoFilterBackend
 from rest_framework import mixins
 from rest_framework import viewsets
 from rest_framework.decorators import action
 from rest_framework.exceptions import NotFound
 from rest_framework.response import Response
+from wagtailcache.cache import cache_page
 
 from geomanager import serializers
-from geomanager.models import Geostore, CountryBoundary
+from geomanager.models import Geostore
 from geomanager.models.vector import PgVectorTable
-from geomanager.serializers.vector import CountrySerializer, GeostoreSerializer
+from geomanager.serializers.vector import AdminBoundarySerializer, GeostoreSerializer
 
 
 class VectorTableFileDetailViewSet(mixins.ListModelMixin, viewsets.GenericViewSet):
     queryset = PgVectorTable.objects.all()
     serializer_class = serializers.PgVectorTableSerializer
     filter_backends = [DjangoFilterBackend]
     filterset_fields = ["layer"]
 
 
-class CountryBoundaryViewSet(viewsets.ViewSet):
+class AdminBoundaryViewSet(viewsets.ViewSet):
     @action(detail=True, methods=['get'])
+    @method_decorator(cache_page)
     def get(self, request):
-        countries = CountryBoundary.objects.filter(level=0)
-        data = CountrySerializer(countries, many=True).data
+        countries = AdminBoundary.objects.filter(level=0)
+        data = AdminBoundarySerializer(countries, many=True).data
         return Response(data)
 
     @action(detail=True, methods=['get'])
+    @method_decorator(cache_page)
     def get_regions(self, request, gid_0):
-        countries = CountryBoundary.objects.filter(level=1, gid_0=gid_0)
-        data = CountrySerializer(countries, many=True).data
+        countries = AdminBoundary.objects.filter(level=1, gid_0=gid_0)
+        data = AdminBoundarySerializer(countries, many=True).data
         return Response(data)
 
     @action(detail=True, methods=['get'])
+    @method_decorator(cache_page)
     def get_sub_regions(self, request, gid_0, gid_1):
-        countries = CountryBoundary.objects.filter(level=2, gid_0=gid_0, gid_1=gid_1)
-        data = CountrySerializer(countries, many=True).data
+        countries = AdminBoundary.objects.filter(level=2, gid_0=gid_0, gid_1=gid_1)
+        data = AdminBoundarySerializer(countries, many=True).data
         return Response(data)
 
 
 class GeostoreViewSet(viewsets.ViewSet):
     @action(detail=True, methods=['post'])
     def post(self, request):
         # parse the GeoJSON from the POST data
@@ -62,51 +68,63 @@
         geostore.save()
 
         res_data = GeostoreSerializer(geostore).data
 
         return Response(res_data)
 
     @action(detail=True, methods=['get'])
+    @method_decorator(cache_page)
     def get(self, request, geostore_id):
         try:
             geostore = Geostore.objects.get(id=geostore_id)
             res_data = GeostoreSerializer(geostore).data
             return Response(res_data)
         except Geostore.DoesNotExist:
             raise NotFound(detail='Geostore not found')
 
     @action(detail=True, methods=['get'])
+    @method_decorator(cache_page)
     def get_by_admin(self, request, gid_0, gid_1=None, gid_2=None):
+        abm_settings = AdminBoundarySettings.for_request(request)
+        data_source = abm_settings.data_source
 
         simplify_thresh = request.GET.get("thresh")
 
         geostore_filter = {
             "iso": gid_0,
             "id1": None,
             "id2": None,
         }
 
         boundary_filter = {
             "gid_0": gid_0,
             "level": 0
         }
 
-        if gid_1:
-            geostore_filter.update({"id1": gid_1})
-            boundary_filter.update({"gid_1": f"{gid_0}.{gid_1}_1", "level": 1})
-        if gid_2:
-            geostore_filter.update({"id2": gid_2})
-            boundary_filter.update({"gid_2": f"{gid_0}.{gid_1}.{gid_2}_1", "level": 2})
+        if data_source != "gadm41":
+            if gid_1:
+                geostore_filter.update({"id1": gid_1})
+                boundary_filter.update({"gid_1": gid_1, "level": 1})
+            if gid_2:
+                geostore_filter.update({"id2": gid_2})
+                boundary_filter.update({"gid_2": gid_2, "level": 2})
+        else:
+            if gid_1:
+                geostore_filter.update({"id1": gid_1})
+                boundary_filter.update({"gid_1": f"{gid_0}.{gid_1}_1", "level": 1})
+            if gid_2:
+                geostore_filter.update({"id2": gid_2})
+                boundary_filter.update({"gid_2": f"{gid_0}.{gid_1}.{gid_2}_1", "level": 2})
 
         geostore = Geostore.objects.filter(**geostore_filter)
         should_save = False
 
         if not geostore.exists():
             should_save = True
-            geostore = CountryBoundary.objects.filter(**boundary_filter)
+            geostore = AdminBoundary.objects.filter(**boundary_filter)
 
         if not geostore.exists():
             raise NotFound(detail='Geostore not found')
 
         geostore = geostore.first()
 
         geom = geostore.geom
```

### Comparing `geomanager-0.0.1/geomanager/wagtail_hooks.py` & `geomanager-0.0.2/geomanager/wagtail_hooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from adminboundarymanager.models import AdminBoundarySettings
 from django import forms
 from django.core.exceptions import ObjectDoesNotExist
 from django.urls import path, reverse
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext_lazy as _
 from wagtail import hooks
 from wagtail.admin.menu import MenuItem
@@ -26,15 +27,15 @@
     publish_raster,
     delete_raster_upload,
     preview_raster_layers,
     upload_vector_file,
     publish_vector,
     delete_vector_upload,
     preview_vector_layers,
-    preview_wms_layers, load_boundary
+    preview_wms_layers
 )
 
 
 @hooks.register('register_admin_urls')
 def urlconf_geomanager():
     return [
         path('upload-rasters/', upload_raster_file, name='geomanager_upload_rasters'),
@@ -45,17 +46,14 @@
         path('publish-rasters/<int:upload_id>/', publish_raster, name='geomanager_publish_raster'),
         path('delete-raster-upload/<int:upload_id>/', delete_raster_upload, name='geomanager_delete_raster_upload'),
 
         path('preview-raster-layers/<uuid:dataset_id>/', preview_raster_layers,
              name='geomanager_preview_raster_dataset'),
         path('preview-raster-layers/<uuid:dataset_id>/<uuid:layer_id>/', preview_raster_layers,
              name='geomanager_preview_raster_layer'),
-
-        path('load-boundary/', load_boundary, name='geomanager_load_boundary'),
-
         path('upload-vector/', upload_vector_file, name='geomanager_upload_vector'),
         path('upload-vector/<uuid:dataset_id>/', upload_vector_file, name='geomanager_dataset_upload_vector'),
         path('upload-vector/<uuid:dataset_id>/<uuid:layer_id>/', upload_vector_file,
              name='geomanager_dataset_layer_upload_vector'),
 
         path('publish-vector/<int:upload_id>/', publish_vector, name='geomanager_publish_vector'),
         path('delete-vector-upload/<int:upload_id>/', delete_vector_upload, name='geomanager_delete_vector_upload'),
@@ -590,15 +588,26 @@
         CategoryModelAdmin, DatasetModelAdmin, MetadataModelAdmin, FileImageLayerModelAdmin,
         RasterStyleModelAdmin, VectorLayerModelAdmin, WmsLayerModelAdmin, MBTSourceModelAdmin,
         LayerRasterFileModelAdmin, PgVectorTableModelAdmin)
 
     def get_submenu_items(self):
         menu_items = super().get_submenu_items()
 
-        boundary_loader = MenuItem(label=_("Boundary Data"), url=reverse("geomanager_load_boundary"), icon_name="map")
+        try:
+            settings_url = reverse(
+                "wagtailsettings:edit",
+                args=[AdminBoundarySettings._meta.app_label, AdminBoundarySettings._meta.model_name, ],
+            )
+            abm_settings_menu = MenuItem(label=_("Boundary Settings"), url=settings_url, icon_name="cog")
+            menu_items.append(abm_settings_menu)
+        except Exception:
+            pass
+
+        boundary_loader = MenuItem(label=_("Boundary Data"), url=reverse("adminboundarymanager_preview_boundary"),
+                                   icon_name="map")
         menu_items.append(boundary_loader)
 
         try:
             settings_url = reverse(
                 "wagtailsettings:edit",
                 args=[GeomanagerSettings._meta.app_label, GeomanagerSettings._meta.model_name, ],
             )
```

### Comparing `geomanager-0.0.1/geomanager.egg-info/PKG-INFO` & `geomanager-0.0.2/geomanager.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomanager
-Version: 0.0.1
+Version: 0.0.2
 Summary: Wagtail based Geospatial Data Manager
 Home-page: https://github.com/wmo-raf/geomanager
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -97,37 +97,36 @@
 pip install geomanager
 ```
 
 The following packages will be automatically installed when installing `geomanager`, if not already installed.
 
 - wagtail>=4.2.2
 - django_extensions>=3.2.1
-- django-countries>=7.5.1
 - wagtail_color_panel>=1.4.1
 - wagtailfontawesomesvg>=0.0.3,
 - django_json_widget>=1.1.1
 - django_nextjs>= 2.2.2
 - django-allauth>=0.54.0
 - django-large-image>=0.9.0
 - large-image-source-gdal>=1.20.6
 - large-image-source-pil>=1.20.6
 - large-image-source-tiff>=1.20.6
 - django-filter>=22.1
-- geopandas>=0.12.2
 - cftime>=1.6.2
 - netCDF4>=1.6.3
 - rasterio>=1.3.6
 - rio-cogeo>=3.5.1
 - xarray>=2023.3.0
 - rioxarray>=0.14.0
 - shapely>=2.0.1
 - djangorestframework-simplejwt>=5.2.2
 - wagtail-humanitarian-icons>=1.0.3
 - wagtail-icon-chooser>=0.0.1
 - matplotlib>=3.7.1
+- wagtail-cache>=2.2.0
 
 # Usage
 
 Make sure the following are all added to your `INSTALLED_APPS` in your Wagtail `settings`
 
 ````python
 INSTALLED_APPS = [
@@ -138,19 +137,19 @@
     'django_json_widget',
     'django_nextjs',
     "django_filters",
     "wagtail_color_panel",
     "wagtail_adminsortable",
     "wagtailhumanitarianicons",
     "wagtailiconchooser",
-    "django_countries",
     "django_extensions",
     "wagtailfontawesomesvg"
     "allauth",
     "allauth.account",
+    "wagtailcache",
 
     "wagtail.contrib.modeladmin",
     "wagtail.contrib.settings",
     "rest_framework",
     "django.contrib.gis",
 
     ...
@@ -170,14 +169,20 @@
 urlpatterns = [
     ...
     path("", include("geomanager.urls")),
     ...
 ]
 ```
 
+# Wagtail Cache Setup
+
+Geomanager depends on the [wagtail-cache](https://github.com/coderedcorp/wagtail-cache) package for caching requests.
+Please have a look at the [wagtail-cache documentation](https://docs.coderedcorp.com/wagtail-cache/) for setup
+instructions
+
 # Including the Map Viewer
 
 This package is the backend component to the frontend [geomapviewer](https://github.com/wmo-raf/geomapviewer).
 
 # Documentation
 
 TODO
```

### Comparing `geomanager-0.0.1/geomanager.egg-info/SOURCES.txt` & `geomanager-0.0.2/geomanager.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -18,20 +18,19 @@
 geomanager/wagtail_hooks.py
 geomanager/widgets.py
 geomanager.egg-info/PKG-INFO
 geomanager.egg-info/SOURCES.txt
 geomanager.egg-info/dependency_links.txt
 geomanager.egg-info/requires.txt
 geomanager.egg-info/top_level.txt
-geomanager/locale/es/LC_MESSAGES/django.po
-geomanager/locale/fr/LC_MESSAGES/django.po
 geomanager/migrations/0001_initial.py
 geomanager/migrations/0002_geomanagersettings_logo_and_more.py
 geomanager/migrations/0003_alter_colorvalue_label_alter_colorvalue_threshold_and_more.py
 geomanager/migrations/0004_alter_dataset_can_clip.py
+geomanager/migrations/0005_delete_countryboundary_and_more.py
 geomanager/migrations/__init__.py
 geomanager/models/__init__.py
 geomanager/models/aoi.py
 geomanager/models/core.py
 geomanager/models/profile.py
 geomanager/models/raster.py
 geomanager/models/tile_gl.py
@@ -60,27 +59,24 @@
 geomanager/static/geomanager/js/vendor/d3-format.min.js
 geomanager/static/geomanager/js/vendor/maplibre-gl.js
 geomanager/static/geomanager/js/vendor/ol.min.js
 geomanager/static/geomanager/js/widgets/icon_chooser.js
 geomanager/static/geomanager/js/widgets/raster_style_widget.js
 geomanager/templates/admin/geomanager/layerrasterfile/change_form.html
 geomanager/templates/django_nextjs/mapviewer.html
-geomanager/templates/geomanager/boundary_loader.html
 geomanager/templates/geomanager/raster_edit_form.html
 geomanager/templates/geomanager/raster_preview.html
 geomanager/templates/geomanager/raster_upload.html
 geomanager/templates/geomanager/vector_edit_form.html
 geomanager/templates/geomanager/vector_preview.html
 geomanager/templates/geomanager/vector_upload.html
 geomanager/templates/geomanager/wms_preview.html
 geomanager/templates/geomanager/widgets/raster_style_widget.html
 geomanager/templates/modeladmin/index_without_custom_create.html
 geomanager/utils/__init__.py
-geomanager/utils/boundary_loader.py
-geomanager/utils/countries.py
 geomanager/utils/raster_utils.py
 geomanager/utils/tile_gl.py
 geomanager/utils/vector_utils.py
 geomanager/views/__init__.py
 geomanager/views/auth.py
 geomanager/views/core.py
 geomanager/views/nextjs.py
```

### Comparing `geomanager-0.0.1/setup.cfg` & `geomanager-0.0.2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = geomanager
-version = 0.0.1
+version = 0.0.2
 description = Wagtail based Geospatial Data Manager
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/geomanager
 author = Erick Otenyo
 author_email = otenyo.erick@gmail.com
 license = MIT
@@ -23,34 +23,33 @@
 [options]
 packages = find:
 include_package_data = true
 python_requires = >=3.9
 install_requires = 
 	wagtail>=4.2.2
 	django_extensions>=3.2.1
-	django-countries>=7.5.1
 	wagtail_color_panel>=1.4.1
 	wagtail-font-awesome-svg>=0.0.3
 	django_json_widget>=1.1.1
 	django_nextjs>=2.2.2
 	django-allauth>=0.54.0
 	django-large-image>=0.10.0
 	large-image-source-rasterio>=1.22.2
 	large-image-source-pil>=1.22.2
 	django-filter>=22.1
-	geopandas>=0.12.2
 	cftime>=1.6.2
 	netCDF4>=1.6.3
 	rasterio>=1.3.6
 	rio-cogeo>=3.5.1
 	xarray>=2023.3.0
 	rioxarray>=0.14.0
 	shapely>=2.0.1
 	djangorestframework-simplejwt>=5.2.2
 	wagtail-humanitarian-icons>=2.0.0
 	wagtail-icon-chooser>=0.0.1
 	matplotlib>=3.7.1
+	wagtail-cache>=2.2.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

