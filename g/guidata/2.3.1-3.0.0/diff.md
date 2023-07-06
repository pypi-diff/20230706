# Comparing `tmp/guidata-2.3.1.tar.gz` & `tmp/guidata-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guidata-2.3.1.tar", last modified: Tue Nov 15 09:48:18 2022, max compression
+gzip compressed data, was "guidata-3.0.0.tar", last modified: Thu Jul  6 16:25:04 2023, max compression
```

## Comparing `guidata-2.3.1.tar` & `guidata-3.0.0.tar`

### file list

```diff
@@ -1,192 +1,210 @@
-drwxrwxrwx   0        0        0        0 2022-11-15 09:48:18.419304 guidata-2.3.1/
--rw-rw-rw-   0        0        0    16699 2022-11-15 09:24:08.000000 guidata-2.3.1/CHANGELOG.md
--rw-rw-rw-   0        0        0    21603 2022-08-21 14:03:05.000000 guidata-2.3.1/Licence_CeCILL_V2-en.txt
--rw-rw-rw-   0        0        0      229 2022-08-21 14:03:05.000000 guidata-2.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2506 2022-11-15 09:48:18.419304 guidata-2.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     2399 2022-11-15 09:25:43.000000 guidata-2.3.1/README.md
-drwxrwxrwx   0        0        0        0 2022-11-15 09:48:18.165827 guidata-2.3.1/doc/
-drwxrwxrwx   0        0        0        0 2022-11-15 09:48:18.165827 guidata-2.3.1/doc/_static/
--rw-rw-rw-   0        0        0     7886 2022-08-21 14:03:05.000000 guidata-2.3.1/doc/_static/favicon.ico
--rw-rw-rw-   0        0        0      642 2022-08-21 14:03:05.000000 guidata-2.3.1/doc/basic_example.py
--rw-rw-rw-   0        0        0     7128 2022-08-21 14:03:05.000000 guidata-2.3.1/doc/conf.py
--rw-rw-rw-   0        0        0      514 2022-08-21 14:03:05.000000 guidata-2.3.1/doc/development.rst
--rw-rw-rw-   0        0        0     2220 2022-08-21 14:03:05.000000 guidata-2.3.1/doc/examples.rst
-drwxrwxrwx   0        0        0        0 2022-11-15 09:48:18.165827 guidata-2.3.1/doc/images/
--rw-rw-rw-   0        0        0     6291 2022-08-21 14:03:05.000000 guidata-2.3.1/doc/images/basic_example.png
--rw-rw-rw-   0        0        0     3437 2022-08-21 14:03:05.000000 guidata-2.3.1/doc/images/guidata.png
-drwxrwxrwx   0        0        0        0 2022-11-15 09:48:18.182328 guidata-2.3.1/doc/images/screenshots/
--rw-rw-rw-   0        0        0    63004 2022-08-21 14:03:05.000000 guidata-2.3.1/doc/images/screenshots/__init__.png
--rw-rw-rw-   0        0        0     7689 2022-08-21 14:03:05.000000 guidata-2.3.1/doc/images/screenshots/activable_dataset.png
--rw-rw-rw-   0        0        0    40397 2022-08-21 14:03:05.000000 guidata-2.3.1/doc/images/screenshots/all_features.png
--rw-rw-rw-   0        0        0    34204 2022-08-21 14:03:05.000000 guidata-2.3.1/doc/images/screenshots/all_items.png
--rw-rw-rw-   0        0        0    10281 2022-08-21 14:03:05.000000 guidata-2.3.1/doc/images/screenshots/bool_selector.png
--rw-rw-rw-   0        0        0    67487 2022-08-21 14:03:05.000000 guidata-2.3.1/doc/images/screenshots/datasetgroup.png
--rw-rw-rw-   0        0        0    19333 2022-08-21 14:03:05.000000 guidata-2.3.1/doc/images/screenshots/editgroupbox.png
--rw-rw-rw-   0        0        0      782 2022-08-21 14:03:05.000000 guidata-2.3.1/doc/index.rst
--rw-rw-rw-   0        0        0     1072 2022-08-21 14:03:05.000000 guidata-2.3.1/doc/installation.rst
--rw-rw-rw-   0        0        0     2125 2022-08-21 14:03:05.000000 guidata-2.3.1/doc/overview.rst
-drwxrwxrwx   0        0        0        0 2022-11-15 09:48:18.182328 guidata-2.3.1/doc/reference/
--rw-rw-rw-   0        0        0       51 2022-08-21 14:03:05.000000 guidata-2.3.1/doc/reference/configtools.rst
--rw-rw-rw-   0        0        0       47 2022-08-21 14:03:05.000000 guidata-2.3.1/doc/reference/dataset.rst
--rw-rw-rw-   0        0        0       51 2022-08-21 14:03:05.000000 guidata-2.3.1/doc/reference/disthelpers.rst
--rw-rw-rw-   0        0        0      176 2022-08-21 14:03:05.000000 guidata-2.3.1/doc/reference/index.rst
--rw-rw-rw-   0        0        0       49 2022-08-21 14:03:05.000000 guidata-2.3.1/doc/reference/qthelpers.rst
--rw-rw-rw-   0        0        0       50 2022-08-21 14:03:05.000000 guidata-2.3.1/doc/reference/userconfig.rst
--rw-rw-rw-   0        0        0       45 2022-08-21 14:03:05.000000 guidata-2.3.1/doc/reference/utils.rst
-drwxrwxrwx   0        0        0        0 2022-11-15 09:48:18.214571 guidata-2.3.1/guidata/
--rw-rw-rw-   0        0        0    27125 2022-11-15 09:24:42.000000 guidata-2.3.1/guidata/__init__.py
--rw-rw-rw-   0        0        0    11108 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/config.py
--rw-rw-rw-   0        0        0     9061 2022-11-14 19:09:17.000000 guidata-2.3.1/guidata/configtools.py
-drwxrwxrwx   0        0        0        0 2022-11-15 09:48:18.246773 guidata-2.3.1/guidata/dataset/
--rw-rw-rw-   0        0        0      611 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/dataset/__init__.py
--rw-rw-rw-   0        0        0    27318 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/dataset/dataitems.py
--rw-rw-rw-   0        0        0    30048 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/dataset/datatypes.py
--rw-rw-rw-   0        0        0    36813 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/dataset/qtitemwidgets.py
--rw-rw-rw-   0        0        0    20892 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/dataset/qtwidgets.py
--rw-rw-rw-   0        0        0      874 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/dataset/textedit.py
--rw-rw-rw-   0        0        0    37596 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/disthelpers.py
--rw-rw-rw-   0        0        0     6408 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/encoding.py
-drwxrwxrwx   0        0        0        0 2022-11-15 09:48:18.246773 guidata-2.3.1/guidata/external/
--rw-rw-rw-   0        0        0        1 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/external/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-15 09:48:18.261278 guidata-2.3.1/guidata/external/darkdetect/
--rw-rw-rw-   0        0        0     1289 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/external/darkdetect/__init__.py
--rw-rw-rw-   0        0        0      377 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/external/darkdetect/_dummy.py
--rw-rw-rw-   0        0        0      890 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/external/darkdetect/_linux_detect.py
--rw-rw-rw-   0        0        0     2212 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/external/darkdetect/_mac_detect.py
--rw-rw-rw-   0        0        0     1257 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/external/darkdetect/_windows_detect.py
--rw-rw-rw-   0        0        0     4079 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/gettext_helpers.py
--rw-rw-rw-   0        0        0     7461 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/guitest.py
--rw-rw-rw-   0        0        0    12629 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/hdf5io.py
-drwxrwxrwx   0        0        0        0 2022-11-15 09:48:18.292613 guidata-2.3.1/guidata/images/
--rw-rw-rw-   0        0        0      785 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/apply.png
--rw-rw-rw-   0        0        0     1123 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/arredit.png
--rw-rw-rw-   0        0        0      721 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/busy.png
--rw-rw-rw-   0        0        0      689 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/cell_edit.png
--rw-rw-rw-   0        0        0      830 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/copy.png
--rw-rw-rw-   0        0        0      722 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/delete.png
--rw-rw-rw-   0        0        0      911 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/dictedit.png
--rw-rw-rw-   0        0        0      735 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/dtype.png
--rw-rw-rw-   0        0        0      929 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/edit.png
-drwxrwxrwx   0        0        0        0 2022-11-15 09:48:18.308245 guidata-2.3.1/guidata/images/editors/
--rw-rw-rw-   0        0        0      911 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/editors/copywop.png
--rw-rw-rw-   0        0        0      929 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/editors/edit.png
--rw-rw-rw-   0        0        0     1001 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/editors/edit_add.png
--rw-rw-rw-   0        0        0     1777 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/editors/editclear.png
--rw-rw-rw-   0        0        0     1048 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/editors/editcopy.png
--rw-rw-rw-   0        0        0      824 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/editors/editcut.png
--rw-rw-rw-   0        0        0     1453 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/editors/editdelete.png
--rw-rw-rw-   0        0        0     1295 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/editors/editpaste.png
--rw-rw-rw-   0        0        0     2248 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/editors/fileimport.png
--rw-rw-rw-   0        0        0     1144 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/editors/filesave.png
--rw-rw-rw-   0        0        0      727 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/editors/imshow.png
--rw-rw-rw-   0        0        0      525 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/editors/insert.png
--rw-rw-rw-   0        0        0      515 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/editors/plot.png
--rw-rw-rw-   0        0        0      689 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/editors/rename.png
--rw-rw-rw-   0        0        0     1184 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/editors/selectall.png
--rw-rw-rw-   0        0        0     1164 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/exit.png
--rw-rw-rw-   0        0        0      165 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/expander_down.png
--rw-rw-rw-   0        0        0      432 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/expander_right.png
--rw-rw-rw-   0        0        0      530 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/file.png
--rw-rw-rw-   0        0        0     1424 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/fileclose.png
--rw-rw-rw-   0        0        0     1556 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/fileimport.png
--rw-rw-rw-   0        0        0      463 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/filenew.png
--rw-rw-rw-   0        0        0     1539 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/fileopen.png
--rw-rw-rw-   0        0        0     1144 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/filesave.png
--rw-rw-rw-   0        0        0     1443 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/filesaveas.png
-drwxrwxrwx   0        0        0        0 2022-11-15 09:48:18.323871 guidata-2.3.1/guidata/images/filetypes/
--rw-rw-rw-   0        0        0     1601 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/filetypes/doc.png
--rw-rw-rw-   0        0        0     1512 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/filetypes/gif.png
--rw-rw-rw-   0        0        0     1848 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/filetypes/html.png
--rw-rw-rw-   0        0        0     1512 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/filetypes/jpg.png
--rw-rw-rw-   0        0        0     1543 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/filetypes/pdf.png
--rw-rw-rw-   0        0        0     1512 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/filetypes/png.png
--rw-rw-rw-   0        0        0     1439 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/filetypes/pps.png
--rw-rw-rw-   0        0        0     1428 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/filetypes/ps.png
--rw-rw-rw-   0        0        0     1577 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/filetypes/tar.png
--rw-rw-rw-   0        0        0     1577 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/filetypes/tgz.png
--rw-rw-rw-   0        0        0     1512 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/filetypes/tif.png
--rw-rw-rw-   0        0        0     1801 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/filetypes/txt.png
--rw-rw-rw-   0        0        0     1237 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/filetypes/xls.png
--rw-rw-rw-   0        0        0     1577 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/filetypes/zip.png
--rw-rw-rw-   0        0        0    19333 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/guidata.svg
--rw-rw-rw-   0        0        0      356 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/max.png
--rw-rw-rw-   0        0        0      351 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/min.png
--rw-rw-rw-   0        0        0      331 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/none.png
--rw-rw-rw-   0        0        0      531 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/not_found.png
--rw-rw-rw-   0        0        0      887 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/python.png
--rw-rw-rw-   0        0        0      888 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/quickview.png
--rw-rw-rw-   0        0        0     1599 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/save_all.png
--rw-rw-rw-   0        0        0      744 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/selection.png
--rw-rw-rw-   0        0        0     2445 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/settings.png
--rw-rw-rw-   0        0        0      361 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/shape.png
--rw-rw-rw-   0        0        0      354 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/xmax.png
--rw-rw-rw-   0        0        0      353 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/images/xmin.png
--rw-rw-rw-   0        0        0     7969 2022-11-14 16:49:47.000000 guidata-2.3.1/guidata/jsonio.py
-drwxrwxrwx   0        0        0        0 2022-11-15 09:48:18.118859 guidata-2.3.1/guidata/locale/
-drwxrwxrwx   0        0        0        0 2022-11-15 09:48:18.118859 guidata-2.3.1/guidata/locale/fr/
-drwxrwxrwx   0        0        0        0 2022-11-15 09:48:18.323871 guidata-2.3.1/guidata/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0        0        0    10218 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/locale/fr/LC_MESSAGES/guidata.mo
--rw-rw-rw-   0        0        0    21530 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/locale/fr/LC_MESSAGES/guidata.po
--rw-rw-rw-   0        0        0     9180 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/qthelpers.py
--rw-rw-rw-   0        0        0     4408 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/qtwidgets.py
-drwxrwxrwx   0        0        0        0 2022-11-15 09:48:18.355122 guidata-2.3.1/guidata/tests/
--rw-rw-rw-   0        0        0      422 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/tests/__init__.py
--rw-rw-rw-   0        0        0     1576 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/tests/activable_dataset.py
--rw-rw-rw-   0        0        0     1047 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/tests/activable_items.py
--rw-rw-rw-   0        0        0     4477 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/tests/all_features.py
--rw-rw-rw-   0        0        0     3471 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/tests/all_items.py
--rw-rw-rw-   0        0        0     1875 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/tests/bool_selector.py
--rw-rw-rw-   0        0        0     1937 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/tests/callbacks.py
--rw-rw-rw-   0        0        0     1496 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/tests/config.py
--rw-rw-rw-   0        0        0     1442 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/tests/data.py
--rw-rw-rw-   0        0        0      798 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/tests/datasetgroup.py
--rw-rw-rw-   0        0        0      811 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/tests/disthelpers.py
--rw-rw-rw-   0        0        0     5711 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/tests/editgroupbox.py
--rw-rw-rw-   0        0        0     1424 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/tests/inheritance.py
--rw-rw-rw-   0        0        0     1237 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/tests/item_order.py
--rw-rw-rw-   0        0        0     1146 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/tests/loadsave_hdf5.py
--rw-rw-rw-   0        0        0      935 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/tests/loadsave_json.py
--rw-rw-rw-   0        0        0     1287 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/tests/rotatedlabel.py
--rw-rw-rw-   0        0        0     2377 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/tests/test_arrayeditor.py
--rw-rw-rw-   0        0        0      618 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/tests/test_codeeditor.py
--rw-rw-rw-   0        0        0     3790 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/tests/test_collectionseditor.py
--rw-rw-rw-   0        0        0      630 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/tests/test_console.py
--rw-rw-rw-   0        0        0     1784 2022-11-15 09:12:03.000000 guidata-2.3.1/guidata/tests/test_dataframeeditor.py
--rw-rw-rw-   0        0        0      600 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/tests/test_importwizard.py
--rw-rw-rw-   0        0        0     1294 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/tests/test_objecteditor.py
--rw-rw-rw-   0        0        0      671 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/tests/text.py
--rw-rw-rw-   0        0        0      436 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/tests/translations.py
--rw-rw-rw-   0        0        0      605 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/tests/userconfig_app.py
--rw-rw-rw-   0        0        0    13187 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/userconfig.py
--rw-rw-rw-   0        0        0     4544 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/userconfigio.py
--rw-rw-rw-   0        0        0    15234 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/utils.py
-drwxrwxrwx   0        0        0        0 2022-11-15 09:48:18.387562 guidata-2.3.1/guidata/widgets/
--rw-rw-rw-   0        0        0      698 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/widgets/__init__.py
--rw-rw-rw-   0        0        0    33275 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/widgets/arrayeditor.py
--rw-rw-rw-   0        0        0    13476 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/widgets/codeeditor.py
--rw-rw-rw-   0        0        0    55301 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/widgets/collectionseditor.py
-drwxrwxrwx   0        0        0        0 2022-11-15 09:48:18.419304 guidata-2.3.1/guidata/widgets/console/
--rw-rw-rw-   0        0        0     3252 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/widgets/console/__init__.py
--rw-rw-rw-   0        0        0    59175 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/widgets/console/base.py
--rw-rw-rw-   0        0        0    12726 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/widgets/console/calltip.py
--rw-rw-rw-   0        0        0    12068 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/widgets/console/dochelpers.py
--rw-rw-rw-   0        0        0    15449 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/widgets/console/internalshell.py
--rw-rw-rw-   0        0        0    12580 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/widgets/console/interpreter.py
--rw-rw-rw-   0        0        0    30741 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/widgets/console/mixins.py
--rw-rw-rw-   0        0        0    33059 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/widgets/console/shell.py
--rw-rw-rw-   0        0        0     4099 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/widgets/console/terminal.py
--rw-rw-rw-   0        0        0    32563 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/widgets/dataframeeditor.py
--rw-rw-rw-   0        0        0    24184 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/widgets/importwizard.py
--rw-rw-rw-   0        0        0    23460 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/widgets/nsview.py
--rw-rw-rw-   0        0        0     2920 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/widgets/objecteditor.py
--rw-rw-rw-   0        0        0    62527 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/widgets/syntaxhighlighters.py
--rw-rw-rw-   0        0        0     4022 2022-08-21 14:03:05.000000 guidata-2.3.1/guidata/widgets/texteditor.py
-drwxrwxrwx   0        0        0        0 2022-11-15 09:48:18.233595 guidata-2.3.1/guidata.egg-info/
--rw-rw-rw-   0        0        0     2506 2022-11-15 09:48:17.000000 guidata-2.3.1/guidata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5031 2022-11-15 09:48:18.000000 guidata-2.3.1/guidata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-15 09:48:17.000000 guidata-2.3.1/guidata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2022-11-15 09:48:17.000000 guidata-2.3.1/guidata.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2022-11-15 09:48:17.000000 guidata-2.3.1/guidata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-11-15 09:48:17.000000 guidata-2.3.1/guidata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-15 09:48:18.419304 guidata-2.3.1/setup.cfg
--rw-rw-rw-   0        0        0     5585 2022-11-15 09:25:52.000000 guidata-2.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 16:25:03.453874 guidata-3.0.0/
+-rw-rw-rw-   0        0        0    18426 2023-07-06 14:11:58.000000 guidata-3.0.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1563 2023-07-06 12:28:58.000000 guidata-3.0.0/LICENSE
+-rw-rw-rw-   0        0        0      186 2023-07-06 16:11:07.000000 guidata-3.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3359 2023-07-06 16:25:03.454875 guidata-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2218 2023-07-06 12:34:12.000000 guidata-3.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 16:25:02.845870 guidata-3.0.0/doc/
+drwxrwxrwx   0        0        0        0 2023-07-06 16:25:02.847869 guidata-3.0.0/doc/_static/
+-rw-rw-rw-   0        0        0    97375 2023-06-30 10:35:52.000000 guidata-3.0.0/doc/_static/favicon.ico
+-rw-rw-rw-   0        0        0      734 2023-06-12 16:28:37.000000 guidata-3.0.0/doc/basic_example.py
+-rw-rw-rw-   0        0        0     1253 2023-07-06 14:41:46.000000 guidata-3.0.0/doc/conf.py
+drwxrwxrwx   0        0        0        0 2023-07-06 16:25:02.863871 guidata-3.0.0/doc/dev/
+-rw-rw-rw-   0        0        0     1839 2023-07-06 07:59:24.000000 guidata-3.0.0/doc/dev/contribute.rst
+-rw-rw-rw-   0        0        0      975 2023-07-06 12:59:03.000000 guidata-3.0.0/doc/dev/howto.rst
+-rw-rw-rw-   0        0        0      123 2023-07-06 12:57:35.000000 guidata-3.0.0/doc/dev/index.rst
+-rw-rw-rw-   0        0        0     1186 2023-07-06 13:32:10.000000 guidata-3.0.0/doc/dev/v2_to_v3.rst
+-rw-rw-rw-   0        0        0     1631 2023-07-06 14:12:31.000000 guidata-3.0.0/doc/examples.rst
+drwxrwxrwx   0        0        0        0 2023-07-06 16:25:02.884868 guidata-3.0.0/doc/images/
+-rw-rw-rw-   0        0        0     4718 2023-07-06 12:12:29.000000 guidata-3.0.0/doc/images/basic_example.png
+-rw-rw-rw-   0        0        0    16573 2023-07-06 15:02:39.000000 guidata-3.0.0/doc/images/guidata-banner.png
+-rw-rw-rw-   0        0        0     6176 2023-06-30 10:38:57.000000 guidata-3.0.0/doc/images/guidata-vertical.png
+-rw-rw-rw-   0        0        0    14799 2023-07-06 12:21:56.000000 guidata-3.0.0/doc/images/layout_example.png
+drwxrwxrwx   0        0        0        0 2023-07-06 16:25:02.926867 guidata-3.0.0/doc/images/screenshots/
+-rw-rw-rw-   0        0        0    78499 2023-07-06 12:13:38.000000 guidata-3.0.0/doc/images/screenshots/__init__.png
+-rw-rw-rw-   0        0        0     4765 2023-07-06 12:14:34.000000 guidata-3.0.0/doc/images/screenshots/activable_dataset.png
+-rw-rw-rw-   0        0        0    31447 2023-07-06 12:15:25.000000 guidata-3.0.0/doc/images/screenshots/all_features.png
+-rw-rw-rw-   0        0        0    37993 2023-07-06 12:15:56.000000 guidata-3.0.0/doc/images/screenshots/all_items.png
+-rw-rw-rw-   0        0        0     8866 2023-07-06 12:16:16.000000 guidata-3.0.0/doc/images/screenshots/bool_selector.png
+-rw-rw-rw-   0        0        0    32420 2023-07-06 12:16:41.000000 guidata-3.0.0/doc/images/screenshots/datasetgroup.png
+-rw-rw-rw-   0        0        0    20345 2023-07-06 12:17:05.000000 guidata-3.0.0/doc/images/screenshots/editgroupbox.png
+-rw-rw-rw-   0        0        0      900 2023-07-06 12:56:58.000000 guidata-3.0.0/doc/index.rst
+-rw-rw-rw-   0        0        0      507 2023-07-06 12:07:32.000000 guidata-3.0.0/doc/installation.rst
+-rw-rw-rw-   0        0        0     1731 2023-07-06 12:22:51.000000 guidata-3.0.0/doc/overview.rst
+drwxrwxrwx   0        0        0        0 2023-07-06 16:25:02.934867 guidata-3.0.0/doc/reference/
+drwxrwxrwx   0        0        0        0 2023-07-06 16:25:02.974873 guidata-3.0.0/doc/reference/dataset/
+-rw-rw-rw-   0        0        0       43 2023-06-30 13:46:46.000000 guidata-3.0.0/doc/reference/dataset/dataitems.rst
+-rw-rw-rw-   0        0        0       43 2023-06-30 13:46:54.000000 guidata-3.0.0/doc/reference/dataset/datatypes.rst
+-rw-rw-rw-   0        0        0      137 2023-07-06 12:24:53.000000 guidata-3.0.0/doc/reference/dataset/index.rst
+-rw-rw-rw-   0        0        0       43 2023-06-30 13:46:30.000000 guidata-3.0.0/doc/reference/dataset/qtwidgets.rst
+-rw-rw-rw-   0        0        0       33 2023-06-30 12:46:29.000000 guidata-3.0.0/doc/reference/guitest.rst
+-rw-rw-rw-   0        0        0      133 2023-07-06 12:24:40.000000 guidata-3.0.0/doc/reference/index.rst
+-rw-rw-rw-   0        0        0      130 2023-06-30 12:45:12.000000 guidata-3.0.0/doc/reference/utils.rst
+-rw-rw-rw-   0        0        0      120 2023-06-30 10:49:38.000000 guidata-3.0.0/doc/reference/widgets.rst
+drwxrwxrwx   0        0        0        0 2023-07-06 16:25:02.993870 guidata-3.0.0/guidata/
+-rw-rw-rw-   0        0        0     3004 2023-07-06 14:12:41.000000 guidata-3.0.0/guidata/__init__.py
+-rw-rw-rw-   0        0        0    11296 2023-07-06 14:12:49.000000 guidata-3.0.0/guidata/config.py
+-rw-rw-rw-   0        0        0    14144 2023-07-06 12:39:33.000000 guidata-3.0.0/guidata/configtools.py
+drwxrwxrwx   0        0        0        0 2023-07-06 16:25:03.026870 guidata-3.0.0/guidata/dataset/
+-rw-rw-rw-   0        0        0      535 2023-07-06 12:39:33.000000 guidata-3.0.0/guidata/dataset/__init__.py
+-rw-rw-rw-   0        0        0    33232 2023-07-06 12:39:43.000000 guidata-3.0.0/guidata/dataset/dataitems.py
+-rw-rw-rw-   0        0        0    34658 2023-07-06 14:12:57.000000 guidata-3.0.0/guidata/dataset/datatypes.py
+-rw-rw-rw-   0        0        0    23498 2023-07-06 12:39:33.000000 guidata-3.0.0/guidata/dataset/hdf5io.py
+-rw-rw-rw-   0        0        0    11586 2023-07-06 12:40:58.000000 guidata-3.0.0/guidata/dataset/iniio.py
+-rw-rw-rw-   0        0        0     8371 2023-06-30 12:40:36.000000 guidata-3.0.0/guidata/dataset/jsonio.py
+-rw-rw-rw-   0        0        0    40201 2023-07-06 12:39:33.000000 guidata-3.0.0/guidata/dataset/qtitemwidgets.py
+-rw-rw-rw-   0        0        0    23426 2023-07-06 12:39:33.000000 guidata-3.0.0/guidata/dataset/qtwidgets.py
+-rw-rw-rw-   0        0        0      820 2023-07-06 12:39:33.000000 guidata-3.0.0/guidata/dataset/textedit.py
+-rw-rw-rw-   0        0        0     6093 2023-07-06 12:40:25.000000 guidata-3.0.0/guidata/env.py
+drwxrwxrwx   0        0        0        0 2023-07-06 16:25:03.029869 guidata-3.0.0/guidata/external/
+-rw-rw-rw-   0        0        0        1 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/external/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 16:25:03.042874 guidata-3.0.0/guidata/external/darkdetect/
+-rw-rw-rw-   0        0        0     1289 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/external/darkdetect/__init__.py
+-rw-rw-rw-   0        0        0      377 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/external/darkdetect/_dummy.py
+-rw-rw-rw-   0        0        0      890 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/external/darkdetect/_linux_detect.py
+-rw-rw-rw-   0        0        0     2212 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/external/darkdetect/_mac_detect.py
+-rw-rw-rw-   0        0        0     1257 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/external/darkdetect/_windows_detect.py
+-rw-rw-rw-   0        0        0   361592 2023-07-06 16:24:46.000000 guidata-3.0.0/guidata/guidata.chm
+-rw-rw-rw-   0        0        0    11264 2023-07-06 14:13:06.000000 guidata-3.0.0/guidata/guitest.py
+drwxrwxrwx   0        0        0        0 2023-07-06 16:25:03.128870 guidata-3.0.0/guidata/images/
+-rw-rw-rw-   0        0        0      785 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/apply.png
+-rw-rw-rw-   0        0        0     1123 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/arredit.png
+-rw-rw-rw-   0        0        0      721 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/busy.png
+-rw-rw-rw-   0        0        0      689 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/cell_edit.png
+-rw-rw-rw-   0        0        0      830 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/copy.png
+-rw-rw-rw-   0        0        0      722 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/delete.png
+-rw-rw-rw-   0        0        0      911 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/dictedit.png
+-rw-rw-rw-   0        0        0      735 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/dtype.png
+-rw-rw-rw-   0        0        0      929 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/edit.png
+drwxrwxrwx   0        0        0        0 2023-07-06 16:25:03.172872 guidata-3.0.0/guidata/images/editors/
+-rw-rw-rw-   0        0        0      911 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/editors/copywop.png
+-rw-rw-rw-   0        0        0      929 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/editors/edit.png
+-rw-rw-rw-   0        0        0     1001 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/editors/edit_add.png
+-rw-rw-rw-   0        0        0     1777 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/editors/editclear.png
+-rw-rw-rw-   0        0        0     1048 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/editors/editcopy.png
+-rw-rw-rw-   0        0        0      824 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/editors/editcut.png
+-rw-rw-rw-   0        0        0     1453 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/editors/editdelete.png
+-rw-rw-rw-   0        0        0     1295 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/editors/editpaste.png
+-rw-rw-rw-   0        0        0     2248 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/editors/fileimport.png
+-rw-rw-rw-   0        0        0     1144 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/editors/filesave.png
+-rw-rw-rw-   0        0        0      727 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/editors/imshow.png
+-rw-rw-rw-   0        0        0      525 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/editors/insert.png
+-rw-rw-rw-   0        0        0      515 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/editors/plot.png
+-rw-rw-rw-   0        0        0      689 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/editors/rename.png
+-rw-rw-rw-   0        0        0     1184 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/editors/selectall.png
+-rw-rw-rw-   0        0        0     1164 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/exit.png
+-rw-rw-rw-   0        0        0      165 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/expander_down.png
+-rw-rw-rw-   0        0        0      432 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/expander_right.png
+-rw-rw-rw-   0        0        0      530 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/file.png
+-rw-rw-rw-   0        0        0     1424 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/fileclose.png
+-rw-rw-rw-   0        0        0     1556 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/fileimport.png
+-rw-rw-rw-   0        0        0      463 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filenew.png
+-rw-rw-rw-   0        0        0     1539 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/fileopen.png
+-rw-rw-rw-   0        0        0     1144 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filesave.png
+-rw-rw-rw-   0        0        0     1443 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filesaveas.png
+drwxrwxrwx   0        0        0        0 2023-07-06 16:25:03.255873 guidata-3.0.0/guidata/images/filetypes/
+-rw-rw-rw-   0        0        0     1601 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filetypes/doc.png
+-rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filetypes/gif.png
+-rw-rw-rw-   0        0        0     1848 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filetypes/html.png
+-rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filetypes/jpg.png
+-rw-rw-rw-   0        0        0     1543 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filetypes/pdf.png
+-rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filetypes/png.png
+-rw-rw-rw-   0        0        0     1439 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filetypes/pps.png
+-rw-rw-rw-   0        0        0     1428 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filetypes/ps.png
+-rw-rw-rw-   0        0        0     1577 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filetypes/tar.png
+-rw-rw-rw-   0        0        0     1577 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filetypes/tgz.png
+-rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filetypes/tif.png
+-rw-rw-rw-   0        0        0     1801 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filetypes/txt.png
+-rw-rw-rw-   0        0        0     1237 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filetypes/xls.png
+-rw-rw-rw-   0        0        0     1577 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filetypes/zip.png
+-rw-rw-rw-   0        0        0    16434 2023-07-06 15:03:14.000000 guidata-3.0.0/guidata/images/guidata-banner.svg
+-rw-rw-rw-   0        0        0    16406 2023-06-30 10:39:39.000000 guidata-3.0.0/guidata/images/guidata-vertical.svg
+-rw-rw-rw-   0        0        0    15818 2023-06-30 10:21:40.000000 guidata-3.0.0/guidata/images/guidata.svg
+-rw-rw-rw-   0        0        0      356 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/max.png
+-rw-rw-rw-   0        0        0      351 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/min.png
+-rw-rw-rw-   0        0        0      331 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/none.png
+-rw-rw-rw-   0        0        0      531 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/not_found.png
+-rw-rw-rw-   0        0        0      887 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/python.png
+-rw-rw-rw-   0        0        0      888 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/quickview.png
+-rw-rw-rw-   0        0        0     1599 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/save_all.png
+-rw-rw-rw-   0        0        0      744 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/selection.png
+-rw-rw-rw-   0        0        0     2445 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/settings.png
+-rw-rw-rw-   0        0        0      361 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/shape.png
+-rw-rw-rw-   0        0        0      354 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/xmax.png
+-rw-rw-rw-   0        0        0      353 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/xmin.png
+drwxrwxrwx   0        0        0        0 2023-07-06 16:25:03.257873 guidata-3.0.0/guidata/locale/
+drwxrwxrwx   0        0        0        0 2023-07-06 16:25:02.792868 guidata-3.0.0/guidata/locale/fr/
+drwxrwxrwx   0        0        0        0 2023-07-06 16:25:03.261873 guidata-3.0.0/guidata/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0    10186 2023-06-29 17:09:10.000000 guidata-3.0.0/guidata/locale/fr/LC_MESSAGES/guidata.mo
+-rw-rw-rw-   0        0        0    20765 2023-06-29 17:09:05.000000 guidata-3.0.0/guidata/locale/fr/LC_MESSAGES/guidata.po
+-rw-rw-rw-   0        0        0    16593 2023-06-29 17:08:15.000000 guidata-3.0.0/guidata/locale/guidata.pot
+-rw-rw-rw-   0        0        0    20476 2023-07-06 12:39:28.000000 guidata-3.0.0/guidata/qthelpers.py
+drwxrwxrwx   0        0        0        0 2023-07-06 16:25:03.359874 guidata-3.0.0/guidata/tests/
+-rw-rw-rw-   0        0        0      368 2023-07-06 12:39:33.000000 guidata-3.0.0/guidata/tests/__init__.py
+-rw-rw-rw-   0        0        0     1709 2023-06-30 14:48:32.000000 guidata-3.0.0/guidata/tests/_all_tests.py
+-rw-rw-rw-   0        0        0      469 2023-06-29 14:36:29.000000 guidata-3.0.0/guidata/tests/conftest.py
+-rw-rw-rw-   0        0        0     1724 2023-07-06 14:13:35.000000 guidata-3.0.0/guidata/tests/test_activable_dataset.py
+-rw-rw-rw-   0        0        0     1153 2023-07-06 14:13:43.000000 guidata-3.0.0/guidata/tests/test_activable_items.py
+-rw-rw-rw-   0        0        0     4858 2023-07-06 14:13:50.000000 guidata-3.0.0/guidata/tests/test_all_features.py
+-rw-rw-rw-   0        0        0     3577 2023-07-06 14:13:57.000000 guidata-3.0.0/guidata/tests/test_all_items.py
+-rw-rw-rw-   0        0        0     2601 2023-07-06 14:14:03.000000 guidata-3.0.0/guidata/tests/test_arrayeditor.py
+-rw-rw-rw-   0        0        0     1932 2023-07-06 14:14:10.000000 guidata-3.0.0/guidata/tests/test_bool_selector.py
+-rw-rw-rw-   0        0        0     2049 2023-07-06 14:14:16.000000 guidata-3.0.0/guidata/tests/test_callbacks.py
+-rw-rw-rw-   0        0        0      652 2023-07-06 14:14:23.000000 guidata-3.0.0/guidata/tests/test_codeeditor.py
+-rw-rw-rw-   0        0        0     3794 2023-07-06 14:14:29.000000 guidata-3.0.0/guidata/tests/test_collectionseditor.py
+-rw-rw-rw-   0        0        0     1068 2023-07-06 12:39:33.000000 guidata-3.0.0/guidata/tests/test_config.py
+-rw-rw-rw-   0        0        0      598 2023-07-06 14:14:35.000000 guidata-3.0.0/guidata/tests/test_console.py
+-rw-rw-rw-   0        0        0     1413 2023-07-06 14:14:42.000000 guidata-3.0.0/guidata/tests/test_data.py
+-rw-rw-rw-   0        0        0     1944 2023-07-06 14:14:58.000000 guidata-3.0.0/guidata/tests/test_dataframeeditor.py
+-rw-rw-rw-   0        0        0      869 2023-07-06 12:39:33.000000 guidata-3.0.0/guidata/tests/test_datasetgroup.py
+-rw-rw-rw-   0        0        0      962 2023-07-06 12:41:46.000000 guidata-3.0.0/guidata/tests/test_disthelpers.py
+-rw-rw-rw-   0        0        0     6011 2023-07-06 14:15:08.000000 guidata-3.0.0/guidata/tests/test_editgroupbox.py
+-rw-rw-rw-   0        0        0      779 2023-07-06 14:15:14.000000 guidata-3.0.0/guidata/tests/test_importwizard.py
+-rw-rw-rw-   0        0        0     1511 2023-07-06 14:15:21.000000 guidata-3.0.0/guidata/tests/test_inheritance.py
+-rw-rw-rw-   0        0        0     1321 2023-07-06 14:15:27.000000 guidata-3.0.0/guidata/tests/test_item_order.py
+-rw-rw-rw-   0        0        0     1112 2023-07-06 12:39:33.000000 guidata-3.0.0/guidata/tests/test_loadsave_hdf5.py
+-rw-rw-rw-   0        0        0     1046 2023-07-06 12:39:33.000000 guidata-3.0.0/guidata/tests/test_loadsave_json.py
+-rw-rw-rw-   0        0        0     1446 2023-07-06 14:15:35.000000 guidata-3.0.0/guidata/tests/test_objecteditor.py
+-rw-rw-rw-   0        0        0     1361 2023-07-06 14:15:41.000000 guidata-3.0.0/guidata/tests/test_rotatedlabel.py
+-rw-rw-rw-   0        0        0      818 2023-07-06 14:15:48.000000 guidata-3.0.0/guidata/tests/test_text.py
+-rw-rw-rw-   0        0        0      493 2023-07-06 12:40:58.000000 guidata-3.0.0/guidata/tests/test_translations.py
+-rw-rw-rw-   0        0        0      778 2023-06-29 14:26:00.000000 guidata-3.0.0/guidata/tests/test_userconfig_app.py
+-rw-rw-rw-   0        0        0    14759 2023-05-22 12:48:41.000000 guidata-3.0.0/guidata/userconfig.py
+drwxrwxrwx   0        0        0        0 2023-07-06 16:25:03.383872 guidata-3.0.0/guidata/utils/
+-rw-rw-rw-   0        0        0     2868 2023-07-06 12:39:33.000000 guidata-3.0.0/guidata/utils/__init__.py
+-rw-rw-rw-   0        0        0    43150 2023-07-06 12:41:24.000000 guidata-3.0.0/guidata/utils/disthelpers.py
+-rw-rw-rw-   0        0        0     6408 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/utils/encoding.py
+-rw-rw-rw-   0        0        0     2364 2023-07-06 12:05:00.000000 guidata-3.0.0/guidata/utils/genreqs.py
+-rw-rw-rw-   0        0        0     4025 2023-07-06 12:39:27.000000 guidata-3.0.0/guidata/utils/gettext_helpers.py
+-rw-rw-rw-   0        0        0     9067 2023-07-06 12:39:33.000000 guidata-3.0.0/guidata/utils/misc.py
+drwxrwxrwx   0        0        0        0 2023-07-06 16:25:03.419872 guidata-3.0.0/guidata/widgets/
+-rw-rw-rw-   0        0        0      729 2023-07-06 12:41:42.000000 guidata-3.0.0/guidata/widgets/__init__.py
+-rw-rw-rw-   0        0        0    33274 2023-06-30 13:14:39.000000 guidata-3.0.0/guidata/widgets/arrayeditor.py
+-rw-rw-rw-   0        0        0    13477 2023-06-30 14:48:54.000000 guidata-3.0.0/guidata/widgets/codeeditor.py
+-rw-rw-rw-   0        0        0    55310 2023-06-30 12:28:15.000000 guidata-3.0.0/guidata/widgets/collectionseditor.py
+drwxrwxrwx   0        0        0        0 2023-07-06 16:25:03.451874 guidata-3.0.0/guidata/widgets/console/
+-rw-rw-rw-   0        0        0     3257 2023-06-30 12:22:39.000000 guidata-3.0.0/guidata/widgets/console/__init__.py
+-rw-rw-rw-   0        0        0    59019 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/widgets/console/base.py
+-rw-rw-rw-   0        0        0    12513 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/widgets/console/calltip.py
+-rw-rw-rw-   0        0        0    11610 2023-06-30 15:04:24.000000 guidata-3.0.0/guidata/widgets/console/dochelpers.py
+-rw-rw-rw-   0        0        0    15411 2023-06-30 14:59:03.000000 guidata-3.0.0/guidata/widgets/console/internalshell.py
+-rw-rw-rw-   0        0        0    12585 2023-06-30 12:28:06.000000 guidata-3.0.0/guidata/widgets/console/interpreter.py
+-rw-rw-rw-   0        0        0    30662 2023-06-30 12:40:32.000000 guidata-3.0.0/guidata/widgets/console/mixins.py
+-rw-rw-rw-   0        0        0    33285 2023-07-06 14:15:58.000000 guidata-3.0.0/guidata/widgets/console/shell.py
+-rw-rw-rw-   0        0        0     4099 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/widgets/console/terminal.py
+-rw-rw-rw-   0        0        0    32563 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/widgets/dataframeeditor.py
+-rw-rw-rw-   0        0        0     3644 2023-07-06 12:41:23.000000 guidata-3.0.0/guidata/widgets/dockable.py
+-rw-rw-rw-   0        0        0    24121 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/widgets/importwizard.py
+-rw-rw-rw-   0        0        0    23460 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/widgets/nsview.py
+-rw-rw-rw-   0        0        0     3351 2023-06-30 13:19:03.000000 guidata-3.0.0/guidata/widgets/objecteditor.py
+-rw-rw-rw-   0        0        0     2122 2023-07-06 12:41:23.000000 guidata-3.0.0/guidata/widgets/rotatedlabel.py
+-rw-rw-rw-   0        0        0    62527 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/widgets/syntaxhighlighters.py
+-rw-rw-rw-   0        0        0     4022 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/widgets/texteditor.py
+drwxrwxrwx   0        0        0        0 2023-07-06 16:25:03.005872 guidata-3.0.0/guidata.egg-info/
+-rw-rw-rw-   0        0        0     3359 2023-07-06 16:25:02.000000 guidata-3.0.0/guidata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5585 2023-07-06 16:25:02.000000 guidata-3.0.0/guidata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 16:25:02.000000 guidata-3.0.0/guidata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2023-07-06 16:25:02.000000 guidata-3.0.0/guidata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-06 16:25:02.000000 guidata-3.0.0/guidata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       84 2023-07-06 15:51:24.000000 guidata-3.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1312 2023-07-06 16:25:04.088819 guidata-3.0.0/setup.cfg
```

### Comparing `guidata-2.3.1/CHANGELOG.md` & `guidata-3.0.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,44 @@
 # guidata Releases #
 
+## Version 3.0.0 ##
+
+New major release:
+
+* New BSD 3-Clause License
+* Black code formatting on all Python files
+* New automated test suite:
+  * Added module `guidata.env` to handle execution environment
+  * Added support for an "unattended" execution mode (Qt loop is bypassed)
+  * Added support for pytest fixtures
+  * Added support for coverage testing: 70% coverage to date
+* Documentation was entirely rewritten using Sphinx
+* Reorganized modules:
+  * Moved `guidata.hd5io` to `guidata.dataset.hdf5io`
+  * Moved `guidata.jsonio` to `guidata.dataset.jsonio`
+  * Renamed `guidata.userconfigio` to `guidata.dataset.iniio`
+  * New package `guidata.utils` for utility functions:
+    * Removed deprecated or unused functions in old `guidata.utils` module
+    * Moved old `guidata.utils` module to `guidata.utils.misc`, except the
+      functions `update_dataset` and `restore_dataset` which are still in
+      `guidata.utils` (root module)
+    * Moved `guidata.encoding` to `guidata.utils.encoding`
+    * Moved `guidata.gettext_helpers` to `guidata.utils.gettext_helpers`
+  * Splitted `guidata.qtwidgets` in two modules:
+    * `guidata.widgets.dockable` for dockable widgets
+    * `guidata.widgets.rotatedlabel` for rotated label
+* Other changes:
+  * `guidata.guitest`:
+    * Added support for subpackages
+    * New comment directive (``# guitest: show``) to add test module to test suite or
+      to show test module in test launcher (this replaces the old ``SHOW = True`` line)
+  * `guidata.dataset.datatypes.DataSet`: new `create` class method for concise
+    dataset creation, allowing to create a dataset with a single line of code by
+    passing default item values as keyword arguments
+
 ## Version 2.3.1 ##
 
 Bug fixes:
 
 * Fixed critical compatibility issue with Python 3.11 (`codeset` argument was removed
   from `gettext.translation` function)
 * Fixed support for `DateTimeItem` and `DateItem` objects serializing (HDF5 and JSON)
```

### Comparing `guidata-2.3.1/README.md` & `guidata-3.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,56 @@
 # guidata: Automatic GUI generation for easy dataset editing and display with Python
 
 [![license](https://img.shields.io/pypi/l/guidata.svg)](./LICENSE)
 [![pypi version](https://img.shields.io/pypi/v/guidata.svg)](https://pypi.org/project/guidata/)
-[![PyPI status](https://img.shields.io/pypi/status/guidata.svg)](https://github.com/PierreRaybaut/guidata)
+[![PyPI status](https://img.shields.io/pypi/status/guidata.svg)](https://github.com/CODRA-Ingenierie-Informatique/guidata/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/guidata.svg)](https://pypi.python.org/pypi/guidata/)
 [![download count](https://img.shields.io/conda/dn/conda-forge/guidata.svg)](https://www.anaconda.com/download/)
 
 Simple example of ``guidata`` datasets embedded in an application window:
 
 <img src="https://raw.githubusercontent.com/PierreRaybaut/guidata/master/doc/images/screenshots/editgroupbox.png">
 
 See [documentation](https://guidata.readthedocs.io/en/latest/) for more details on
 the library and [changelog](CHANGELOG.md) for recent history of changes.
 
-Copyright © 2009-2022 CEA, Pierre Raybaut, licensed under the terms of the
-CECILL License (see ``Licence_CeCILL_V2-en.txt``).
+Copyrights and licensing:
+
+* Copyright © 2023 [CEA](https://www.cea.fr), [Codra](https://codra.net/), [Pierre Raybaut](https://github.com/PierreRaybaut).
+* Licensed under the terms of the BSD 3-Clause (see [LICENSE](LICENSE)).
 
 ## Overview
 
 Based on the Qt library, ``guidata`` is a Python library generating graphical user
 interfaces for easy dataset editing and display. It also provides helpers and
 application development tools for Qt (PyQt5, PySide2, PyQt6, PySide6).
 
 Generate GUIs to edit and display all kind of objects:
 
-- integers, floats, strings ;
-- ndarrays (NumPy's n-dimensional arrays) ;
-- etc.
+* integers, floats, strings ;
+* ndarrays (NumPy's n-dimensional arrays) ;
+* etc.
 
 Application development tools:
 
-- configuration management
-- internationalization (``gettext``)
-- deployment tools
-- HDF5 I/O helpers
-- misc. utils
+* configuration management
+* internationalization (``gettext``)
+* deployment tools
+* HDF5 I/O helpers
+* misc. utils
 
 ## Dependencies
 
 ### Requirements
 
-- Python >= 3.7
-- [PyQt5](https://pypi.python.org/pypi/PyQt5) >=5.5 or [PySide2](https://pypi.python.org/pypi/PySide2) >=5.11
-- [QtPy](https://pypi.org/project/QtPy/) >= 1.3
-
-### Optional Python modules
-
-- [h5py](https://pypi.python.org/pypi/h5py) (HDF5 files I/O)
-- [cx_Freeze](https://pypi.python.org/pypi/cx_Freeze) or [py2exe](https://pypi.python.org/pypi/py2exe) (application deployment on Windows platforms)
-
-### Other optional modules
-
-gettext (text translation support)
-
-### Recommended modules
-
-[guiqwt](https://pypi.python.org/pypi/guiqwt) >= 4.3 is a set of tools for curve and image plotting based on `guidata`.
+* Python 3.7+
+* [PyQt5](https://pypi.python.org/pypi/PyQt5) (Python Qt bindings)
+* [QtPy](https://pypi.org/project/QtPy/) (abstraction layer for Python-Qt binding libraries)
+* [h5py](https://pypi.org/project/h5py/) (interface to the HDF5 data format)
+* [NumPy](https://pypi.org/project/numpy/) (operations on multidimensional arrays)
 
 ## Installation
 
 ### From the source package
 
 ```bash
 python setup.py install
```

### Comparing `guidata-2.3.1/doc/basic_example.py` & `guidata-3.0.0/doc/basic_example.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # -*- coding: utf-8 -*-
 
-# Note: the two following lines are not required
-#       if a QApplication has already been created
 import guidata
+import guidata.dataset.dataitems as di
+import guidata.dataset.datatypes as dt
 
+# Note: the following line is not required if a QApplication has already been created
 _app = guidata.qapplication()
 
-import guidata.dataset.datatypes as dt
-import guidata.dataset.dataitems as di
-
 
 class Processing(dt.DataSet):
     """Example"""
 
     a = di.FloatItem("Parameter #1", default=2.3)
     b = di.IntItem("Parameter #2", min=0, max=10, default=5)
     type = di.ChoiceItem("Processing algorithm", ("type 1", "type 2", "type 3"))
 
 
 param = Processing()
 param.edit()
 print(param)  # Showing param contents
 param.b = 4  # Modifying item value
 param.view()
+
+# Alternative way for creating a DataSet instance:
+param = Processing.create(a=7.323, b=4)
+print(param)
```

### Comparing `guidata-2.3.1/doc/overview.rst` & `guidata-3.0.0/doc/overview.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,38 @@
 Overview
 ========
 
-When developping scientific software, from the simplest script to the 
-most complex application, one systematically needs to manipulate data sets 
+When developping scientific software, from the simplest script to the
+most complex application, one systematically needs to manipulate data sets
 (e.g. parameters for a data processing feature).
-These data sets may consist of various data types: real numbers (e.g. physical 
-quantities), integers (e.g. array indexes), strings (e.g. filenames), 
+These data sets may consist of various data types: real numbers (e.g. physical
+quantities), integers (e.g. array indexes), strings (e.g. filenames),
 booleans (e.g. enable/disable an option), and so on.
 
 Most of the time, the programmer will need the following features:
 
-    * allow the user to enter each parameter through a graphical user interface,
-      using widgets which are adapted to data types (e.g. a single combo box or 
-      check boxes are suitable for presenting an option selection among 
-      multiple choices)
-
-    * entered values have to be stored by the program with a convention which 
-      is again adapted to data types (e.g. when storing a combo box selection 
-      value, should we store the option string, the list index or an 
-      associated key?)
-
-    * using the stored values easily (e.g. for data processing) by regrouping 
-      parameters in data structures
-      
-    * showing the stored values in a dialog box or within a graphical user 
-      interface layout, again with widgets adapted to data types
+* allow the user to enter each parameter through a graphical user interface,
+  using widgets which are adapted to data types (e.g. a single combo box or
+  check boxes are suitable for presenting an option selection among
+  multiple choices)
+
+* entered values have to be stored by the program with a convention which
+  is again adapted to data types (e.g. when storing a combo box selection
+  value, should we store the option string, the list index or an
+  associated key?)
 
-This library aims to provide these features thanks to automatic graphical user 
-interface generation for data set editing and display. Widgets inside GUIs are 
-automatically generated depending on each data item type.
+* using the stored values easily (e.g. for data processing) by regrouping
+  parameters in data structures
+
+* showing the stored values in a dialog box or within a graphical user
+  interface layout, again with widgets adapted to data types
 
-The `guidata` library also provides the following features:
+This library aims to provide these features thanks to automatic graphical user
+interface generation for data set editing and display. Widgets inside GUIs are
+automatically generated depending on each data item type.
 
-    * :py:mod:`guidata.qthelpers`: Qt helpers
-    * :py:mod:`guidata.disthelpers`: `py2ex` helpers
-    * :py:mod:`guidata.userconfig`: `.ini` configuration management helpers 
-      (based on Python standard module :py:mod:`ConfigParser`)
-    * :py:mod:`guidata.configtools`: library/application data management
-    * :py:mod:`guidata.gettext_helpers`: translation helpers 
-      (based on the GNU tool `gettext`)
-    * :py:mod:`guidata.guitest`: automatic GUI-based test launcher
-    * :py:mod:`guidata.utils`: miscelleneous utilities
+The :mod:`guidata` library also provides the following features:
 
+* :py:mod:`guidata.qthelpers`: Qt helpers
+* :py:mod:`guidata.configtools`: library/application data management
+* :py:mod:`guidata.guitest`: automatic GUI-based test launcher
+* :py:mod:`guidata.utils`: utilities
```

### Comparing `guidata-2.3.1/guidata/config.py` & `guidata-3.0.0/guidata/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright © 2009-2010 CEA
-# Pierre Raybaut
-# Licensed under the terms of the CECILL License
-# (see guidata/__init__.py for details)
+# Licensed under the terms of the BSD 3-Clause
+# (see guidata/LICENSE for details)
 
 """
 Handle *guidata* module configuration
 (options, images and icons)
 """
 
 import os.path as osp
 
 from guidata.configtools import add_image_module_path, get_translation
 from guidata.userconfig import UserConfig
 
-
+APP_NAME = "guidata"
 APP_PATH = osp.dirname(__file__)
 add_image_module_path("guidata", "images")
 _ = get_translation("guidata")
 
 
 def gen_mono_font_settings(size, other_settings=None):
     """Generate mono font settings"""
@@ -31,15 +29,21 @@
             "font/family/mac": "Monaco",
             "font/size": size,
         }
     )
     return settings
 
 
+def get_old_log_fname(fname):
+    """Return old log fname from current log fname"""
+    return osp.splitext(fname)[0] + ".1.log"
+
+
 DEFAULTS = {
+    "faulthandler": {"enabled": False, "log_path": f".{APP_NAME}_faulthandler.log"},
     "arrayeditor": gen_mono_font_settings(9),
     "dicteditor": gen_mono_font_settings(9),
     "texteditor": gen_mono_font_settings(9),
     "codeeditor": gen_mono_font_settings(10),
     "console": gen_mono_font_settings(
         9,
         {
@@ -102,15 +106,15 @@
         "idle/comment": ("#dd0000", False, True),
         "idle/string": ("#00aa00", False, False),
         "idle/number": ("#924900", False, False),
         "idle/instance": ("#777777", True, True),
         # ---- Monokai ----
         "monokai/name": "Monokai",
         #      Name              Color     Bold  Italic
-        "monokai/background": "#121212",
+        "monokai/background": "#1f1f1f",
         "monokai/currentline": "#484848",
         "monokai/currentcell": "#3d3d3d",
         "monokai/occurrence": "#666666",
         "monokai/ctrlclick": "#0000ff",
         "monokai/sideareas": "#2a2b24",
         "monokai/matched_p": "#688060",
         "monokai/unmatched_p": "#bd6e76",
@@ -178,15 +182,15 @@
         "spyder/comment": ("#adadad", False, True),
         "spyder/string": ("#00aa00", False, False),
         "spyder/number": ("#800000", False, False),
         "spyder/instance": ("#924900", False, True),
         # ---- Spyder/Dark ----
         "spyder/dark/name": "Spyder Dark",
         #           Name             Color     Bold  Italic
-        "spyder/dark/background": "#121212",
+        "spyder/dark/background": "#1f1f1f",
         "spyder/dark/currentline": "#2b2b43",
         "spyder/dark/currentcell": "#31314e",
         "spyder/dark/occurrence": "#abab67",
         "spyder/dark/ctrlclick": "#0000ff",
         "spyder/dark/sideareas": "#282828",
         "spyder/dark/matched_p": "#009800",
         "spyder/dark/unmatched_p": "#c80000",
@@ -197,15 +201,15 @@
         "spyder/dark/comment": ("#7f7f7f", False, False),
         "spyder/dark/string": ("#11a642", False, True),
         "spyder/dark/number": ("#c80000", False, False),
         "spyder/dark/instance": ("#be5f00", False, True),
         # ---- Zenburn ----
         "zenburn/name": "Zenburn",
         #        Name            Color     Bold  Italic
-        "zenburn/background": "#121212",
+        "zenburn/background": "#1f1f1f",
         "zenburn/currentline": "#333333",
         "zenburn/currentcell": "#2c2c2c",
         "zenburn/occurrence": "#7a738f",
         "zenburn/ctrlclick": "#0000ff",
         "zenburn/sideareas": "#3f3f3f",
         "zenburn/matched_p": "#688060",
         "zenburn/unmatched_p": "#bd6e76",
@@ -235,15 +239,15 @@
         "solarized/light/comment": ("#93a1a1", False, True),
         "solarized/light/string": ("#2aa198", False, False),
         "solarized/light/number": ("#cb4b16", False, False),
         "solarized/light/instance": ("#b58900", False, True),
         # ---- Solarized Dark ----
         "solarized/dark/name": "Solarized Dark",
         #        Name            Color     Bold  Italic
-        "solarized/dark/background": "#121212",
+        "solarized/dark/background": "#1f1f1f",
         "solarized/dark/currentline": "#083f4d",
         "solarized/dark/currentcell": "#073642",
         "solarized/dark/occurrence": "#657b83",
         "solarized/dark/ctrlclick": "#d33682",
         "solarized/dark/sideareas": "#073642",
         "solarized/dark/matched_p": "#93a1a1",
         "solarized/dark/unmatched_p": "#dc322f",
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `guidata-2.3.1/guidata/configtools.py` & `guidata-3.0.0/guidata/configtools.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,61 +1,111 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright © 2009-2010 CEA
-# Pierre Raybaut
-# Licensed under the terms of the CECILL License
-# (see guidata/__init__.py for details)
+# Licensed under the terms of the BSD 3-Clause
+# (see guidata/LICENSE for details)
 
 """
-configtools
------------
+Configuration related functions
+-------------------------------
 
-The ``guidata.configtools`` module provides configuration related tools.
+Access configured options
+^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. autofunction:: get_icon
+
+.. autofunction:: get_image_file_path
+
+.. autofunction:: get_image_label
+
+.. autofunction:: get_image_layout
+
+.. autofunction:: get_family
+
+.. autofunction:: get_font
+
+.. autofunction:: get_pen
+
+.. autofunction:: get_brush
+
+Add image paths
+^^^^^^^^^^^^^^^
+
+.. autofunction:: add_image_path
+
+.. autofunction:: add_image_module_path
 """
 
+from __future__ import annotations
+
 import gettext
 import os
 import os.path as osp
 import sys
+from collections.abc import Callable
+from typing import TYPE_CHECKING
+
+from guidata.utils.misc import decode_fs_string, get_module_path
+
+if TYPE_CHECKING:
+    from qtpy import QtCore as QC
+    from qtpy import QtGui as QG
+    from qtpy import QtWidgets as QW
 
-from guidata.utils import decode_fs_string, get_module_path
+    from guidata.userconfig import UserConfig
 
 IMG_PATH = []
 
 
-def get_module_data_path(modname, relpath=None):
+def get_module_data_path(modname: str, relpath: str | None = None) -> str:
     """Return module *modname* data path
-    Handles py2exe/cx_Freeze distributions"""
+    Handles py2exe/cx_Freeze distributions
+
+    Args:
+        modname (str): module name
+        relpath (str, optional): relative path to module data directory
+
+    Returns:
+        str: module data path
+    """
     datapath = getattr(sys.modules[modname], "DATAPATH", "")
     if not datapath:
         datapath = get_module_path(modname)
         parentdir = osp.normpath(osp.join(datapath, osp.pardir))
         if osp.isfile(parentdir):
             # Parent directory is not a directory but the 'library.zip' file:
             # this is either a py2exe or a cx_Freeze distribution
             datapath = osp.abspath(osp.join(osp.join(parentdir, osp.pardir), modname))
     if relpath is not None:
         datapath = osp.abspath(osp.join(datapath, relpath))
     return datapath
 
 
-def get_translation(modname, dirname=None):
-    """Return translation callback for module *modname*"""
+def get_translation(modname: str, dirname: str | None = None) -> Callable[[str], str]:
+    """Return translation callback for module *modname*
+
+    Args:
+        modname (str): module name
+        dirname (str, optional): module directory
+
+    Returns:
+        Callable[[str], str]: translation callback
+    """
     if dirname is None:
         dirname = modname
     # fixup environment var LANG in case it's unknown
     if "LANG" not in os.environ:
         import locale  # Warning: 2to3 false alarm ('import' fixer)
 
         lang = locale.getdefaultlocale()[0]
         if lang is not None:
             os.environ["LANG"] = lang
     try:
         modlocpath = get_module_locale_path(dirname)
         try:
+            # pylint: disable=unexpected-keyword-arg
             _trans = gettext.translation(modname, modlocpath, codeset="utf-8")
         except TypeError:
             # Python >= 3.11 (codeset argument has been removed)
             _trans = gettext.translation(modname, modlocpath)
         lgettext = _trans.gettext
 
         def translate_gettext(x):
@@ -72,51 +122,78 @@
             if not isinstance(x, str):
                 return str(x, "utf-8")
             return x
 
         return translate_dumb
 
 
-def get_module_locale_path(modname):
-    """Return module *modname* gettext translation path"""
+def get_module_locale_path(modname: str) -> str:
+    """Return module *modname* gettext translation path
+
+    Args:
+        modname (str): module name
+
+    Returns:
+        str: module gettext translation path
+    """
     localepath = getattr(sys.modules[modname], "LOCALEPATH", "")
     if not localepath:
         localepath = get_module_data_path(modname, relpath="locale")
     return localepath
 
 
-def add_image_path(path, subfolders=True):
-    """Append image path (opt. with its subfolders) to global list IMG_PATH"""
+def add_image_path(path: str, subfolders: bool = True) -> None:
+    """Append image path (opt. with its subfolders) to global list IMG_PATH
+
+    Args:
+        path (str): image path
+        subfolders (bool, optional): include subfolders
+    """
     if not isinstance(path, str):
         path = decode_fs_string(path)
     global IMG_PATH
     IMG_PATH.append(path)
     if subfolders:
         for fileobj in os.listdir(path):
             pth = osp.join(path, fileobj)
             if osp.isdir(pth):
                 IMG_PATH.append(pth)
 
 
-def add_image_module_path(modname, relpath, subfolders=True):
+def add_image_module_path(modname: str, relpath: str, subfolders: bool = True) -> None:
     """
     Appends image data path relative to a module name.
     Used to add module local data that resides in a module directory
     but will be shipped under sys.prefix / share/ ...
 
     modname must be the name of an already imported module as found in
     sys.modules
+
+    Args:
+        modname (str): module name
+        relpath (str): relative path to module data directory
+        subfolders (bool, optional): include subfolders
     """
     add_image_path(get_module_data_path(modname, relpath=relpath), subfolders)
 
 
-def get_image_file_path(name, default="not_found.png"):
+def get_image_file_path(name: str, default: str = "not_found.png") -> str:
     """
     Return the absolute path to image with specified name
     name, default: filenames with extensions
+
+    Args:
+        name (str): name of the image
+        default (str, optional): default image name. Defaults to "not_found.png".
+
+    Raises:
+        RuntimeError: if image file not found
+
+    Returns:
+        str: absolute path to image
     """
     for pth in IMG_PATH:
         full_path = osp.join(pth, name)
         if osp.isfile(full_path):
             return osp.abspath(full_path)
     if default is not None:
         try:
@@ -126,51 +203,78 @@
     else:
         raise RuntimeError()
 
 
 ICON_CACHE = {}
 
 
-def get_icon(name, default="not_found.png"):
+def get_icon(name: str, default: str = "not_found.png") -> QG.QIcon:
     """
     Construct a QIcon from the file with specified name
     name, default: filenames with extensions
+
+    Args:
+        name (str): name of the icon
+        default (str, optional): default icon name. Defaults to "not_found.png".
+
+    Returns:
+        QG.QIcon: icon
     """
     try:
         return ICON_CACHE[name]
     except KeyError:
-        from qtpy import QtGui as QG
+        # Importing Qt here because this module should be independent from it
+        from qtpy import QtGui as QG  # pylint: disable=import-outside-toplevel
 
         icon = QG.QIcon(get_image_file_path(name, default))
         ICON_CACHE[name] = icon
         return icon
 
 
-def get_image_label(name, default="not_found.png"):
+def get_image_label(name, default="not_found.png") -> QW.QLabel:
     """
     Construct a QLabel from the file with specified name
     name, default: filenames with extensions
-    """
-    from qtpy import QtGui as QG
-    from qtpy import QtWidgets as QW
+
+    Args:
+        name (str): name of the icon
+        default (str, optional): default icon name. Defaults to "not_found.png".
+
+    Returns:
+        QW.QLabel: label
+    """
+    # Importing Qt here because this module should be independent from it
+    from qtpy import QtGui as QG  # pylint: disable=import-outside-toplevel
+    from qtpy import QtWidgets as QW  # pylint: disable=import-outside-toplevel
 
     label = QW.QLabel()
     pixmap = QG.QPixmap(get_image_file_path(name, default))
     label.setPixmap(pixmap)
     return label
 
 
-def get_image_layout(imagename, text="", tooltip="", alignment=None):
+def get_image_layout(
+    imagename: str, text: str = "", tooltip: str = "", alignment: QC.Qt.Alignment = None
+) -> tuple[QW.QHBoxLayout, QW.QLabel]:
     """
     Construct a QHBoxLayout including image from the file with specified name,
     left-aligned text [with specified tooltip]
-    Return (layout, label)
-    """
-    from qtpy import QtCore as QC
-    from qtpy import QtWidgets as QW
+
+    Args:
+        imagename (str): name of the icon
+        text (str, optional): text to display. Defaults to "".
+        tooltip (str, optional): tooltip to display. Defaults to "".
+        alignment (QC.Qt.Alignment, optional): alignment of the text. Defaults to None.
+
+    Returns:
+        tuple[QW.QHBoxLayout, QW.QLabel]: layout, label
+    """
+    # Importing Qt here because this module should be independent from it
+    from qtpy import QtCore as QC  # pylint: disable=import-outside-toplevel
+    from qtpy import QtWidgets as QW  # pylint: disable=import-outside-toplevel
 
     if alignment is None:
         alignment = QC.Qt.AlignLeft
     layout = QW.QHBoxLayout()
     if alignment in (QC.Qt.AlignCenter, QC.Qt.AlignRight):
         layout.addStretch()
     layout.addWidget(get_image_label(imagename))
@@ -178,17 +282,25 @@
     label.setToolTip(tooltip)
     layout.addWidget(label)
     if alignment in (QC.Qt.AlignCenter, QC.Qt.AlignLeft):
         layout.addStretch()
     return (layout, label)
 
 
-def font_is_installed(font):
-    """Check if font is installed"""
-    from qtpy import QtGui as QG
+def font_is_installed(font: str) -> list[str]:
+    """Check if font is installed
+
+    Args:
+        font (str): font name
+
+    Returns:
+        list[str]: list of installed fonts
+    """
+    # Importing Qt here because this module should be independent from it
+    from qtpy import QtGui as QG  # pylint: disable=import-outside-toplevel
 
     return [fam for fam in QG.QFontDatabase().families() if str(fam) == font]
 
 
 MONOSPACE = [
     "Cascadia Code PL",
     "Cascadia Mono PL",
@@ -203,33 +315,49 @@
     "Courier",
     "monospace",
     "Fixed",
     "Terminal",
 ]
 
 
-def get_family(families):
-    """Return the first installed font family in family list"""
+def get_family(families: str | list[str]) -> str:
+    """Return the first installed font family in family list
+
+    Args:
+        families (str|list[str]): font family or list of font families
+
+    Returns:
+        str: first installed font family
+    """
     if not isinstance(families, list):
         families = [families]
     for family in families:
         if font_is_installed(family):
             return family
     else:
         print("Warning: None of the following fonts is installed: %r" % families)
         return ""
 
 
-def get_font(conf, section, option=""):
+def get_font(conf: UserConfig, section: str, option: str = "") -> QG.QFont:
     """
     Construct a QFont from the specified configuration file entry
     conf: UserConfig instance
     section [, option]: configuration entry
+
+    Args:
+        conf (UserConfig): UserConfig instance
+        section (str): configuration entry
+        option (str, optional): configuration entry. Defaults to "".
+
+    Returns:
+        QG.QFont: font
     """
-    from qtpy import QtGui as QG
+    # Importing Qt here because this module should be independent from it
+    from qtpy import QtGui as QG  # pylint: disable=import-outside-toplevel
 
     if not option:
         option = "font"
     if "font" not in option:
         option += "/font"
     font = QG.QFont()
     if conf.has_option(section, option + "/family/nt"):
@@ -251,45 +379,81 @@
     if conf.get(section, option + "/bold", False):
         font.setWeight(QG.QFont.Bold)
     else:
         font.setWeight(QG.QFont.Normal)
     return font
 
 
-def get_pen(conf, section, option="", color="black", width=1, style="SolidLine"):
+def get_pen(
+    conf: UserConfig,
+    section: str,
+    option: str = "",
+    color: str = "black",
+    width: int = 1,
+    style: str = "SolidLine",
+) -> QG.QPen:
     """
     Construct a QPen from the specified configuration file entry
     conf: UserConfig instance
     section [, option]: configuration entry
     [color]: default color
     [width]: default width
     [style]: default style
-    """
-    from qtpy import QtCore as QC
-    from qtpy import QtGui as QG
+
+    Args:
+        conf (UserConfig): UserConfig instance
+        section (str): configuration entry
+        option (str, optional): configuration entry. Defaults to "".
+        color (str, optional): default color. Defaults to "black".
+        width (int, optional): default width. Defaults to 1.
+        style (str, optional): default style. Defaults to "SolidLine".
+
+    Returns:
+        QG.QPen: pen
+    """
+    # Importing Qt here because this module should be independent from it
+    from qtpy import QtCore as QC  # pylint: disable=import-outside-toplevel
+    from qtpy import QtGui as QG  # pylint: disable=import-outside-toplevel
 
     if "pen" not in option:
         option += "/pen"
     color = conf.get(section, option + "/color", color)
     color = QG.QColor(color)
     width = conf.get(section, option + "/width", width)
     style_name = conf.get(section, option + "/style", style)
     style = getattr(QC.Qt, style_name)
     return QG.QPen(color, width, style)
 
 
-def get_brush(conf, section, option="", color="black", alpha=1.0):
+def get_brush(
+    conf: UserConfig,
+    section: str,
+    option: str = "",
+    color: str = "black",
+    alpha: float = 1.0,
+) -> QG.QBrush:
     """
     Construct a QBrush from the specified configuration file entry
     conf: UserConfig instance
     section [, option]: configuration entry
     [color]: default color
     [alpha]: default alpha-channel
+
+    Args:
+        conf (UserConfig): UserConfig instance
+        section (str): configuration entry
+        option (str, optional): configuration entry. Defaults to "".
+        color (str, optional): default color. Defaults to "black".
+        alpha (float, optional): default alpha-channel. Defaults to 1.0.
+
+    Returns:
+        QG.QBrush: brush
     """
-    from qtpy import QtGui as QG
+    # Importing Qt here because this module should be independent from it
+    from qtpy import QtGui as QG  # pylint: disable=import-outside-toplevel
 
     if "brush" not in option:
         option += "/brush"
     color = conf.get(section, option + "/color", color)
     color = QG.QColor(color)
     alpha = conf.get(section, option + "/alphaF", alpha)
     color.setAlphaF(alpha)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `guidata-2.3.1/guidata/dataset/__init__.py` & `guidata-3.0.0/guidata/dataset/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright © 2009-2010 CEA
-# Pierre Raybaut
-# Licensed under the terms of the CECILL License
-# (see guidata/__init__.py for details)
+# Licensed under the terms of the BSD 3-Clause
+# (see guidata/LICENSE for details)
 
 """
 dataset
 =======
 
-The ``guidata.dataset`` package provides the core features for data set 
+The ``guidata.dataset`` package provides the core features for data set
 display and editing with automatically generated graphical user interfaces.
 
 .. automodule:: guidata.dataset.dataitems
    :members:
-       
+
 .. automodule:: guidata.dataset.datatypes
    :members:
-       
+
 .. automodule:: guidata.dataset.qtitemwidgets
    :members:
-       
+
 .. automodule:: guidata.dataset.qtwidgets
    :members:
 """
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `guidata-2.3.1/guidata/dataset/dataitems.py` & `guidata-3.0.0/guidata/dataset/dataitems.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,147 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright © 2009-2010 CEA
-# Pierre Raybaut
-# Licensed under the terms of the CECILL License
-# (see guidata/__init__.py for details)
+# Licensed under the terms of the BSD 3-Clause
+# (see guidata/LICENSE for details)
 
 """
-dataset.dataitems
-=================
+Data items
+----------
 
-The ``guidata.dataset.dataitems`` module contains implementation for
-concrete DataItems.
+Numeric items
+^^^^^^^^^^^^^
+
+.. autoclass:: FloatItem
+    :members:
+
+.. autoclass:: IntItem
+    :members:
+
+.. autoclass:: FloatArrayItem
+    :members:
+
+Text items
+^^^^^^^^^^
+
+.. autoclass:: StringItem
+    :members:
+
+.. autoclass:: TextItem
+    :members:
+
+Date and time items
+^^^^^^^^^^^^^^^^^^^
+
+.. autoclass:: DateItem
+    :members:
+
+.. autoclass:: DateTimeItem
+    :members:
+
+Color items
+^^^^^^^^^^^
+
+.. autoclass:: ColorItem
+    :members:
+
+File items
+^^^^^^^^^^
+
+.. autoclass:: FileSaveItem
+    :members:
+
+.. autoclass:: FileOpenItem
+    :members:
+
+.. autoclass:: FilesOpenItem
+    :members:
+
+.. autoclass:: DirectoryItem
+    :members:
+
+Choice items
+^^^^^^^^^^^^
+
+.. autoclass:: BoolItem
+    :members:
+
+.. autoclass:: ChoiceItem
+    :members:
+
+.. autoclass:: MultipleChoiceItem
+    :members:
+
+.. autoclass:: ImageChoiceItem
+    :members:
+
+Other items
+^^^^^^^^^^^
+
+.. autoclass:: ButtonItem
+    :members:
+
+.. autoclass:: DictItem
+    :members:
+
+.. autoclass:: FontFamilyItem
+    :members:
 """
 
+import collections.abc
+import datetime
 import os
 import re
-import datetime
-import collections.abc
+from typing import TYPE_CHECKING, Any, Callable, List, Optional, Tuple, Type, Union
 
-from guidata.dataset.datatypes import DataItem, ItemProperty
-from guidata.utils import utf8_to_unicode, add_extension
 from guidata.config import _
+from guidata.dataset.datatypes import DataItem, DataSet, ItemProperty
+from guidata.dataset.iniio import UserConfigReader, UserConfigWriter
+from guidata.qthelpers import exec_dialog
+from numpy import ndarray
+
+if TYPE_CHECKING:  # pragma: no cover
+    from guidata.dataset.hdf5io import HDF5Reader, HDF5Writer
+    from guidata.dataset.jsonio import JSONReader, JSONWriter
 
 
 class NumericTypeItem(DataItem):
     """
     Numeric data item
+    * label [string]: name
+    * default [int]: default value (optional)
+    * min [int]: minimum value (optional)
+    * max [int]: maximum value (optional)
+    * nonzero [bool]: if True, zero is not a valid value (optional)
+    * unit [string]: physical unit (optional)
+    * even [bool]: if True, even values are valid, if False,
+        odd values are valid if None (default), ignored (optional)
+    * slider [bool]: if True, shows a slider widget right after the line
+        edit widget (default is False)
+    * help [string]: text shown in tooltip (optional)
+    * check [bool]: if False, value is not checked (optional, default=True)
     """
 
-    type = None
+    type: Callable = None
 
     def __init__(
         self,
-        label,
-        default=None,
-        min=None,
-        max=None,
-        nonzero=None,
-        unit="",
-        help="",
-        check=True,
-    ):
+        label: str,
+        default: Optional[Union[float, int]] = None,
+        min: Optional[Union[float, int]] = None,
+        max: Optional[Union[float, int]] = None,
+        nonzero: Optional[bool] = None,
+        unit: str = "",
+        help: str = "",
+        check: bool = True,
+    ) -> None:
         DataItem.__init__(self, label, default=default, help=help)
         self.set_prop("data", min=min, max=max, nonzero=nonzero, check_value=check)
         self.set_prop("display", unit=unit)
 
-    def get_auto_help(self, instance):
+    def get_auto_help(self, instance: DataSet) -> str:
         """Override DataItem method"""
         auto_help = {int: _("integer"), float: _("float")}[self.type]
         _min = self.get_prop_value("data", instance, "min")
         _max = self.get_prop_value("data", instance, "max")
         nonzero = self.get_prop_value("data", instance, "nonzero")
         unit = self.get_prop_value("display", instance, "unit")
         if _min is not None and _max is not None:
@@ -60,25 +152,27 @@
             auto_help += _(" lower than ") + str(_max)
         if nonzero:
             auto_help += ", " + _("non zero")
         if unit:
             auto_help += ", %s %s" % (_("unit:"), unit)
         return auto_help
 
-    def format_string(self, instance, value, fmt, func):
+    def format_string(
+        self, instance: "DataSet", value: Union[float, int], fmt: str, func: Callable
+    ) -> str:
         """Override DataItem method"""
         text = fmt % (func(value),)
         # We add directly the unit to 'text' (instead of adding it
         # to 'fmt') to avoid string formatting error if '%' is in unit
         unit = self.get_prop_value("display", instance, "unit", "")
         if unit:
             text += " " + unit
         return text
 
-    def check_value(self, value):
+    def check_value(self, value: Union[float, int]) -> bool:
         """Override DataItem method"""
         if not self.get_prop("data", "check_value", True):
             return True
         if not isinstance(value, self.type):
             return False
         if self.get_prop("data", "nonzero") and value == 0:
             return False
@@ -88,15 +182,15 @@
                 return False
         _max = self.get_prop("data", "max")
         if _max is not None:
             if value > _max:
                 return False
         return True
 
-    def from_string(self, value):
+    def from_string(self, value: str) -> Optional[Any]:
         """Override DataItem method"""
         # String may contains numerical operands:
         if re.match(r"^([\d\(\)\+/\-\*.]|e)+$", value):
             try:
                 return self.type(eval(value))
             except:
                 pass
@@ -119,39 +213,41 @@
         * check [bool]: if False, value is not checked (optional, default=True)
     """
 
     type = float
 
     def __init__(
         self,
-        label,
-        default=None,
-        min=None,
-        max=None,
-        nonzero=None,
-        unit="",
-        step=0.1,
-        slider=False,
-        help="",
-        check=True,
-    ):
-        super(FloatItem, self).__init__(
+        label: str,
+        default: Optional[float] = None,
+        min: Optional[float] = None,
+        max: Optional[float] = None,
+        nonzero: Optional[bool] = None,
+        unit: str = "",
+        step: float = 0.1,
+        slider: bool = False,
+        help: str = "",
+        check: bool = True,
+    ) -> None:
+        super().__init__(
             label,
             default=default,
             min=min,
             max=max,
             nonzero=nonzero,
             unit=unit,
             help=help,
             check=check,
         )
         self.set_prop("display", slider=slider)
         self.set_prop("data", step=step)
 
-    def get_value_from_reader(self, reader):
+    def get_value_from_reader(
+        self, reader: Union["HDF5Reader", "JSONReader", "UserConfigReader"]
+    ) -> float:
         """Reads value from the reader object, inside the try...except
         statement defined in the base item `deserialize` method"""
         return reader.read_float()
 
 
 class IntItem(NumericTypeItem):
     """
@@ -170,64 +266,66 @@
         * check [bool]: if False, value is not checked (optional, default=True)
     """
 
     type = int
 
     def __init__(
         self,
-        label,
-        default=None,
-        min=None,
-        max=None,
-        nonzero=None,
-        unit="",
-        even=None,
-        slider=False,
-        help="",
-        check=True,
-    ):
-        super(IntItem, self).__init__(
+        label: str,
+        default: Optional[int] = None,
+        min: Optional[int] = None,
+        max: Optional[int] = None,
+        nonzero: Optional[bool] = None,
+        unit: str = "",
+        even: Optional[bool] = None,
+        slider: bool = False,
+        help: str = "",
+        check: bool = True,
+    ) -> None:
+        super().__init__(
             label,
             default=default,
             min=min,
             max=max,
             nonzero=nonzero,
             unit=unit,
             help=help,
             check=check,
         )
         self.set_prop("data", even=even)
         self.set_prop("display", slider=slider)
 
-    def get_auto_help(self, instance):
+    def get_auto_help(self, instance: "DataSet") -> str:
         """Override DataItem method"""
-        auto_help = super(IntItem, self).get_auto_help(instance)
+        auto_help = super().get_auto_help(instance)
         even = self.get_prop_value("data", instance, "even")
         if even is not None:
             if even:
                 auto_help += ", " + _("even")
             else:
                 auto_help += ", " + _("odd")
         return auto_help
 
-    def check_value(self, value):
+    def check_value(self, value: Any) -> bool:
         """Override DataItem method"""
         if not self.get_prop("data", "check_value", True):
             return True
-        valid = super(IntItem, self).check_value(value)
+        valid = super().check_value(value)
         if not valid:
             return False
         even = self.get_prop("data", "even")
         if even is not None:
             is_even = value // 2 == value / 2.0
             if (even and not is_even) or (not even and is_even):
                 return False
         return True
 
-    def get_value_from_reader(self, reader):
+    def get_value_from_reader(
+        self, reader: Union["HDF5Reader", "JSONReader", "UserConfigReader"]
+    ) -> Any:
         """Reads value from the reader object, inside the try...except
         statement defined in the base item `deserialize` method"""
         return reader.read_int()
 
 
 class StringItem(DataItem):
     """
@@ -235,33 +333,42 @@
         * label [string]: name
         * default [string]: default value (optional)
         * help [string]: text shown in tooltip (optional)
         * notempty [bool]: if True, empty string is not a valid value (opt.)
         * wordwrap [bool]: toggle word wrapping (optional)
     """
 
-    type = (str,)
+    type: Any = str
 
-    def __init__(self, label, default=None, notempty=None, wordwrap=False, help=""):
+    def __init__(
+        self,
+        label: str,
+        default: Optional[str] = None,
+        notempty: Optional[bool] = None,
+        wordwrap: bool = False,
+        help: str = "",
+    ) -> None:
         DataItem.__init__(self, label, default=default, help=help)
         self.set_prop("data", notempty=notempty)
         self.set_prop("display", wordwrap=wordwrap)
 
-    def check_value(self, value):
+    def check_value(self, value: Any) -> bool:
         """Override DataItem method"""
         notempty = self.get_prop("data", "notempty")
         if notempty and not value:
             return False
         return True
 
-    def from_string(self, value):
+    def from_string(self, value: str) -> str:
         """Override DataItem method"""
         return value
 
-    def get_value_from_reader(self, reader):
+    def get_value_from_reader(
+        self, reader: Union["HDF5Reader", "JSONReader", "UserConfigReader"]
+    ) -> Any:
         """Reads value from the reader object, inside the try...except
         statement defined in the base item `deserialize` method"""
         return reader.read_unicode()
 
 
 class TextItem(StringItem):
     """
@@ -269,15 +376,22 @@
         * label [string]: name
         * default [string]: default value (optional)
         * help [string]: text shown in tooltip (optional)
         * notempty [bool]: if True, empty string is not a valid value (opt.)
         * wordwrap [bool]: toggle word wrapping (optional)
     """
 
-    def __init__(self, label, default=None, notempty=None, wordwrap=True, help=""):
+    def __init__(
+        self,
+        label: str,
+        default: Optional[str] = None,
+        notempty: Optional[bool] = None,
+        wordwrap: bool = True,
+        help: str = "",
+    ) -> None:
         StringItem.__init__(
             self,
             label,
             default=default,
             notempty=notempty,
             wordwrap=wordwrap,
             help=help,
@@ -292,19 +406,28 @@
         * default [string]: default value (optional)
         * help [string]: text shown in tooltip (optional)
         * check [bool]: if False, value is not checked (optional, default=True)
     """
 
     type = bool
 
-    def __init__(self, text="", label="", default=None, help="", check=True):
+    def __init__(
+        self,
+        text: str = "",
+        label: str = "",
+        default: Optional[bool] = None,
+        help: str = "",
+        check: bool = True,
+    ) -> None:
         DataItem.__init__(self, label, default=default, help=help, check=check)
         self.set_prop("display", text=text)
 
-    def get_value_from_reader(self, reader):
+    def get_value_from_reader(
+        self, reader: Union["HDF5Reader", "JSONReader", "UserConfigReader"]
+    ) -> bool:
         """Reads value from the reader object, inside the try...except
         statement defined in the base item `deserialize` method"""
         return reader.read_bool()
 
 
 class DateItem(DataItem):
     """
@@ -315,39 +438,49 @@
         * help [string]: text shown in tooltip (optional)
     """
 
     type = datetime.date
 
 
 class DateTimeItem(DateItem):
+    """
+    Construct a date time data item.
+        * text [string]: form's field name (optional)
+        * label [string]: name
+        * default [datetime.date]: default value (optional)
+        * help [string]: text shown in tooltip (optional)
+    """
+
     pass
 
 
 class ColorItem(StringItem):
     """
     Construct a color data item
         * label [string]: name
         * default [string]: default value (optional)
         * help [string]: text shown in tooltip (optional)
         * check [bool]: if False, value is not checked (optional, default=True)
 
     Color values are encoded as hexadecimal strings or Qt color names
     """
 
-    def check_value(self, value):
+    def check_value(self, value: str) -> bool:
         """Override DataItem method"""
         if not self.get_prop("data", "check_value", True):
             return True
         if not isinstance(value, self.type):
             return False
         from guidata.qthelpers import text_to_qcolor
 
         return text_to_qcolor(value).isValid()
 
-    def get_value_from_reader(self, reader):
+    def get_value_from_reader(
+        self, reader: Union["HDF5Reader", "JSONReader", "UserConfigReader"]
+    ) -> str:
         """Reads value from the reader object, inside the try...except
         statement defined in the base item `deserialize` method"""
         # Using read_str converts `numpy.string_` to `str` -- otherwise,
         # when passing the string to a QColor Qt object, any numpy.string_ will
         # be interpreted as no color (black)
         return reader.read_str()
 
@@ -361,63 +494,73 @@
         * basedir [string]: default base directory (optional)
         * help [string]: text shown in tooltip (optional)
         * check [bool]: if False, value is not checked (optional, default=True)
     """
 
     def __init__(
         self,
-        label,
-        formats="*",
-        default=None,
-        basedir=None,
-        all_files_first=False,
-        help="",
-        check=True,
-    ):
+        label: str,
+        formats: Union[Tuple[str, ...], str] = "*",
+        default: Optional[Union[List[str], str]] = None,
+        basedir: Optional[str] = None,
+        all_files_first: bool = False,
+        help: str = "",
+        check: bool = True,
+    ) -> None:
         DataItem.__init__(self, label, default=default, help=help, check=check)
         if isinstance(formats, str):
-            formats = [formats]
+            formats = [formats]  # type:ignore
         self.set_prop("data", formats=formats)
         self.set_prop("data", basedir=basedir)
         self.set_prop("data", all_files_first=all_files_first)
 
-    def get_auto_help(self, instance):
+    def get_auto_help(self, instance: "DataSet") -> str:
         """Override DataItem method"""
         formats = self.get_prop("data", "formats")
         return (
             _("all file types")
             if formats == ["*"]
             else _("supported file types:") + " *.%s" % ", *.".join(formats)
         )
 
-    def check_value(self, value):
+    def check_value(self, value: str) -> bool:
         """Override DataItem method"""
         if not self.get_prop("data", "check_value", True):
             return True
         if not isinstance(value, self.type):
             return False
         return len(value) > 0
 
-    def from_string(self, value):
+    def from_string(self, value) -> str:
         """Override DataItem method"""
-        return add_extension(self, value)
+        return self.add_extension(value)
+
+    def add_extension(self, value) -> str:
+        """Add extension to filename
+        `value`: possible value for data item"""
+        value = str(value)
+        formats = self.get_prop("data", "formats")
+        if len(formats) == 1 and formats[0] != "*":
+            if not value.endswith("." + formats[0]) and len(value) > 0:
+                return value + "." + formats[0]
+        return value
 
 
 class FileOpenItem(FileSaveItem):
     """
     Construct a path data item for a file to be opened
         * label [string]: name
         * formats [string (or string list)]: wildcard filter
         * default [string]: default value (optional)
         * basedir [string]: default base directory (optional)
         * help [string]: text shown in tooltip (optional)
         * check [bool]: if False, value is not checked (optional, default=True)
     """
 
-    def check_value(self, value):
+    def check_value(self, value: str) -> bool:
         """Override DataItem method"""
         if not self.get_prop("data", "check_value", True):
             return True
         if not isinstance(value, self.type):
             return False
         return os.path.exists(value) and os.path.isfile(value)
 
@@ -433,84 +576,95 @@
         * check [bool]: if False, value is not checked (optional, default=True)
     """
 
     type = list
 
     def __init__(
         self,
-        label,
-        formats="*",
-        default=None,
-        basedir=None,
-        all_files_first=False,
-        help="",
-        check=True,
-    ):
+        label: str,
+        formats: str = "*",
+        default: Optional[Union[List[str], str]] = None,
+        basedir: Optional[str] = None,
+        all_files_first: bool = False,
+        help: str = "",
+        check: bool = True,
+    ) -> None:
         if isinstance(default, str):
             default = [default]
         FileSaveItem.__init__(
             self,
             label,
             formats=formats,
             default=default,
             basedir=basedir,
             all_files_first=all_files_first,
             help=help,
             check=check,
         )
 
-    def check_value(self, value):
+    def check_value(self, value: str) -> bool:
         """Override DataItem method"""
         if not self.get_prop("data", "check_value", True):
             return True
         if value is None:
             return False
         allexist = True
         for path in value:
             allexist = allexist and os.path.exists(path) and os.path.isfile(path)
         return allexist
 
-    def from_string(self, value):
+    def from_string(self, value: Any) -> List[str]:  # type:ignore
         """Override DataItem method"""
         if value.endswith("']") or value.endswith('"]'):
             value = eval(value)
         else:
             value = [value]
-        return [add_extension(self, path) for path in value]
+        return [self.add_extension(path) for path in value]
 
-    def serialize(self, instance, writer):
+    def serialize(
+        self,
+        instance: "DataSet",
+        writer: Union["HDF5Writer", "JSONWriter", "UserConfigWriter"],
+    ) -> None:
         """Serialize this item"""
         value = self.get_value(instance)
         writer.write_sequence([fname.encode("utf-8") for fname in value])
 
-    def get_value_from_reader(self, reader):
+    def get_value_from_reader(
+        self, reader: Union["HDF5Reader", "JSONReader", "UserConfigReader"]
+    ) -> List[str]:
         """Reads value from the reader object, inside the try...except
         statement defined in the base item `deserialize` method"""
         return [fname for fname in reader.read_sequence()]
 
 
 class DirectoryItem(StringItem):
     """
     Construct a path data item for a directory.
         * label [string]: name
         * default [string]: default value (optional)
         * help [string]: text shown in tooltip (optional)
         * check [bool]: if False, value is not checked (optional, default=True)
     """
 
-    def check_value(self, value):
+    def check_value(self, value: str) -> bool:
         """Override DataItem method"""
         if not self.get_prop("data", "check_value", True):
             return True
         if not isinstance(value, self.type):
             return False
         return os.path.exists(value) and os.path.isdir(value)
 
 
-class FirstChoice(object):
+class FirstChoice:
+    """
+    Special object that means the default value of a ChoiceItem
+    is the first item.
+    """
+
     pass
 
 
 class ChoiceItem(DataItem):
     """
     Construct a data item for a list of choices.
         * label [string]: name
@@ -522,48 +676,50 @@
         * help [string]: text shown in tooltip (optional)
         * check [bool]: if False, value is not checked (optional, default=True)
         * radio [bool]: if True, shows radio buttons instead of a combo box
           (default is False)
     """
 
     def __init__(
-        self, label, choices, default=FirstChoice, help="", check=True, radio=False
-    ):
-        if isinstance(choices, collections.abc.Callable):
+        self,
+        label: str,
+        choices: Any,
+        default: Optional[Union[Tuple[()], Type[FirstChoice], int]] = FirstChoice,
+        help: str = "",
+        check: bool = True,
+        radio: bool = False,
+    ) -> None:
+        _choices_data: Any
+        if isinstance(choices, collections.abc.Callable):  # type:ignore
             _choices_data = ItemProperty(choices)
         else:
             _choices_data = []
             for idx, choice in enumerate(choices):
                 _choices_data.append(self._normalize_choice(idx, choice))
-        if default is FirstChoice and not isinstance(choices, collections.abc.Callable):
+        if default is FirstChoice and not isinstance(
+            choices, collections.abc.Callable  # type:ignore
+        ):
             default = _choices_data[0][0]
         elif default is FirstChoice:
             default = None
         DataItem.__init__(self, label, default=default, help=help, check=check)
         self.set_prop("data", choices=_choices_data)
         self.set_prop("display", radio=radio)
 
-    def _normalize_choice(self, idx, choice_tuple):
+    def _normalize_choice(
+        self, idx: int, choice_tuple: Tuple[Any, ...]
+    ) -> Union[Tuple[int, str, None], Tuple[str, str, None]]:
         if isinstance(choice_tuple, tuple):
             key, value = choice_tuple
         else:
             key = idx
             value = choice_tuple
-
-        if isinstance(value, str):
-            value = utf8_to_unicode(value)
         return (key, value, None)
 
-    #    def _choices(self, item):
-    #        _choices_data = self.get_prop("data", "choices")
-    #        if callable(_choices_data):
-    #            return _choices_data(self, item)
-    #        return _choices_data
-
-    def get_string_value(self, instance):
+    def get_string_value(self, instance: "DataSet") -> str:
         """Override DataItem method"""
         value = self.get_value(instance)
         choices = self.get_prop_value("data", instance, "choices")
         # print "ShowChoiceWidget:", choices, value
         for choice in choices:
             if choice[0] == value:
                 return str(choice[1])
@@ -577,58 +733,77 @@
         * label [string]: name
         * choices [list or tuple]: string list or (key, label) list
         * default [-]: default label or default key (optional)
         * help [string]: text shown in tooltip (optional)
         * check [bool]: if False, value is not checked (optional, default=True)
     """
 
-    def __init__(self, label, choices, default=(), help="", check=True):
+    def __init__(
+        self,
+        label: str,
+        choices: List[str],
+        default: Tuple[()] = (),
+        help: str = "",
+        check: bool = True,
+    ) -> None:
         ChoiceItem.__init__(self, label, choices, default, help, check=check)
         self.set_prop("display", shape=(1, -1))
 
-    def horizontal(self, row_nb=1):
+    def horizontal(self, row_nb: int = 1) -> "MultipleChoiceItem":
         """
         Method to arange choice list horizontally on `n` rows
 
         Example:
         nb = MultipleChoiceItem("Number", ['1', '2', '3'] ).horizontal(2)
         """
         self.set_prop("display", shape=(row_nb, -1))
         return self
 
-    def vertical(self, col_nb=1):
+    def vertical(self, col_nb: int = 1) -> "MultipleChoiceItem":
         """
         Method to arange choice list vertically on `n` columns
 
         Example:
         nb = MultipleChoiceItem("Number", ['1', '2', '3'] ).vertical(2)
         """
         self.set_prop("display", shape=(-1, col_nb))
         return self
 
-    def serialize(self, instance, writer):
+    def serialize(
+        self,
+        instance: "DataSet",
+        writer: Union["HDF5Writer", "JSONWriter", "UserConfigWriter"],
+    ) -> None:
         """Serialize this item"""
         value = self.get_value(instance)
         seq = []
         _choices = self.get_prop_value("data", instance, "choices")
         for key, _label, _img in _choices:
             seq.append(key in value)
         writer.write_sequence(seq)
 
-    def deserialize(self, instance, reader):
+    def deserialize(
+        self,
+        instance: "DataSet",
+        reader: Union["HDF5Reader", "JSONReader", "UserConfigReader"],
+    ) -> None:
         """Deserialize this item"""
-        flags = reader.read_sequence()
-        # We could have trouble with objects providing their own choice
-        # function which depend on not yet deserialized values
-        _choices = self.get_prop_value("data", instance, "choices")
-        value = []
-        for idx, flag in enumerate(flags):
-            if flag:
-                value.append(_choices[idx][0])
-        self.__set__(instance, value)
+        try:
+            flags = reader.read_sequence()
+        except KeyError:
+            self.set_default(instance)
+        else:
+            # We could have trouble with objects providing their own choice
+            # function which depend on not yet deserialized values
+            _choices = self.get_prop_value("data", instance, "choices")
+            value = []
+            for idx, flag in enumerate(flags):
+                if flag:
+                    value.append(_choices[idx][0])
+            self.__set__(instance, value)
 
 
 class ImageChoiceItem(ChoiceItem):
     """
     Construct a data item for a list of choices with images
         * label [string]: name
         * choices [list, tuple or function]: (label, image) list or
@@ -637,24 +812,23 @@
           icon path, a QIcon instance or a function of one argument (key)
           returning a QIcon instance
         * default [-]: default label or default key (optional)
         * help [string]: text shown in tooltip (optional)
         * check [bool]: if False, value is not checked (optional, default=True)
     """
 
-    def _normalize_choice(self, idx, choice_tuple):
+    def _normalize_choice(
+        self, idx: int, choice_tuple: Tuple[Any, ...]
+    ) -> Tuple[Any, Any, Any]:
         assert isinstance(choice_tuple, tuple)
         if len(choice_tuple) == 3:
             key, value, img = choice_tuple
         else:
             key = idx
             value, img = choice_tuple
-
-        if isinstance(value, str):
-            value = utf8_to_unicode(value)
         return (key, value, img)
 
 
 class FloatArrayItem(DataItem):
     """
     Construct a float array data item
         * label [string]: name
@@ -665,26 +839,28 @@
         * large [bool]: view all float of the array
         * minmax [string]: "all" (default), "columns", "rows"
         * check [bool]: if False, value is not checked (optional, default=True)
     """
 
     def __init__(
         self,
-        label,
-        default=None,
-        help="",
-        format="%.3f",
-        transpose=False,
-        minmax="all",
-        check=True,
-    ):
+        label: str,
+        default: Optional[ndarray] = None,
+        help: str = "",
+        format: str = "%.3f",
+        transpose: bool = False,
+        minmax: str = "all",
+        check: bool = True,
+    ) -> None:
         DataItem.__init__(self, label, default=default, help=help, check=check)
         self.set_prop("display", format=format, transpose=transpose, minmax=minmax)
 
-    def format_string(self, instance, value, fmt, func):
+    def format_string(
+        self, instance: "DataSet", value: Any, fmt: str, func: Callable
+    ) -> str:
         """Override DataItem method"""
         larg = self.get_prop_value("display", instance, "large", False)
         fmt = self.get_prop_value("display", instance, "format", "%s")
         unit = self.get_prop_value("display", instance, "unit", "")
         v = func(value)
         if larg:
             text = "= ["
@@ -695,20 +871,26 @@
             text = "~= " + fmt % v.mean()
             text += " [" + fmt % v.min()
             text += " .. " + fmt % v.max()
             text += "]"
         text += " %s" % unit
         return str(text)
 
-    def serialize(self, instance, writer):
+    def serialize(
+        self,
+        instance: "DataSet",
+        writer: Union["HDF5Writer", "JSONWriter", "UserConfigWriter"],
+    ) -> None:
         """Serialize this item"""
         value = self.get_value(instance)
         writer.write_array(value)
 
-    def get_value_from_reader(self, reader):
+    def get_value_from_reader(
+        self, reader: Union["HDF5Reader", "JSONReader", "UserConfigReader"]
+    ) -> Any:
         """Reads value from the reader object, inside the try...except
         statement defined in the base item `deserialize` method"""
         return reader.read_array()
 
 
 class ButtonItem(DataItem):
     """
@@ -726,45 +908,69 @@
         * help [string]: text shown in button's tooltip (optional)
         * check [bool]: if False, value is not checked (optional, default=True)
 
     The value of this item is unspecified but is passed to the callback along
     with the whole dataset. The value is assigned the callback`s return value.
     """
 
-    def __init__(self, label, callback, icon=None, default=None, help="", check=True):
+    def __init__(
+        self,
+        label: str,
+        callback: Callable,
+        icon: Optional[str] = None,
+        default: Optional[Any] = None,
+        help: str = "",
+        check: bool = True,
+    ) -> None:
         DataItem.__init__(self, label, default=default, help=help, check=check)
         self.set_prop("display", callback=callback)
         self.set_prop("display", icon=icon)
 
-    def serialize(self, instance, writer):
+    def serialize(
+        self,
+        instance: "DataSet",
+        writer: Union["HDF5Writer", "JSONWriter", "UserConfigWriter"],
+    ) -> Any:
         pass
 
-    def deserialize(self, instance, reader):
+    def deserialize(
+        self,
+        instance: "DataSet",
+        reader: Union["HDF5Reader", "JSONReader", "UserConfigReader"],
+    ) -> Any:
         pass
 
 
 class DictItem(ButtonItem):
     """
     Construct a dictionary data item
         * label [string]: name
         * default [dict]: default value (optional)
         * help [string]: text shown in tooltip (optional)
         * check [bool]: if False, value is not checked (optional, default=True)
     """
 
-    def __init__(self, label, default=None, help="", check=True):
-        def dictedit(instance, item, value, parent):
+    def __init__(
+        self,
+        label: str,
+        default: Optional[dict] = None,
+        help: str = "",
+        check: bool = True,
+    ) -> None:
+        def dictedit(
+            instance: "DataSet", item: "DataItem", value: Any, parent: object
+        ) -> Any:
             from guidata.widgets.collectionseditor import CollectionsEditor
 
             editor = CollectionsEditor(parent)
             value_was_none = value is None
             if value_was_none:
                 value = {}
             editor.setup(value)
-            if editor.exec_():
+            if exec_dialog(editor):
                 return editor.get_value()
             else:
                 if value_was_none:
                     return
                 return value
 
         ButtonItem.__init__(
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `guidata-2.3.1/guidata/dataset/datatypes.py` & `guidata-3.0.0/guidata/dataset/datatypes.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,76 +1,135 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright © 2009-2010 CEA
-# Pierre Raybaut
-# Licensed under the terms of the CECILL License
-# (see guidata/__init__.py for details)
+# Licensed under the terms of the BSD 3-Clause
+# (see guidata/LICENSE for details)
 
 """
-dataset.datatypes
-=================
+Data sets
+---------
 
-The ``guidata.dataset.datatypes`` module contains implementation for
-DataSets (DataSet, DataSetGroup, ...) and related objects (ItemProperty,
-ValueProp, ...).
+Defining data sets
+^^^^^^^^^^^^^^^^^^
+
+.. autoclass:: DataSet
+    :members:
+
+.. autoclass:: DataSetGroup
+    :members:
+
+.. autoclass:: ActivableDataSet
+    :members:
+
+Grouping items
+^^^^^^^^^^^^^^
+
+.. autoclass:: BeginGroup
+    :members:
+
+.. autoclass:: EndGroup
+    :members:
+
+.. autoclass:: BeginTabGroup
+    :members:
+
+.. autoclass:: EndTabGroup
+    :members:
+
+Handling item properties
+^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. autoclass:: FormatProp
+    :members:
+
+.. autoclass:: GetAttrProp
+    :members:
+
+.. autoclass:: ValueProp
+    :members:
+
+.. autoclass:: NotProp
+    :members:
+
+.. autoclass:: FuncProp
+    :members:
 """
 
 # pylint: disable-msg=W0622
 # pylint: disable-msg=W0212
 
-import sys
-import re
 import collections.abc
-
-from guidata.utils import utf8_to_unicode, update_dataset
-
+import re
+import sys
+from abc import abstractmethod
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Tuple,
+    Type,
+    Union,
+)
+
+from guidata.dataset.iniio import UserConfigReader, UserConfigWriter
+from guidata.qthelpers import exec_dialog
+from guidata.userconfig import UserConfig
+from guidata.utils import update_dataset
+from qtpy.QtWidgets import QWidget
 
 DEBUG_DESERIALIZE = False
 
+if TYPE_CHECKING:  # pragma: no cover
+    from guidata.dataset.hdf5io import HDF5Reader, HDF5Writer
+    from guidata.dataset.jsonio import JSONReader, JSONWriter
+    from guidata.dataset.qtwidgets import DataSetEditDialog
+
 
 class NoDefault:
     pass
 
 
-class ItemProperty(object):
-    def __init__(self, callable=None):
+class ItemProperty:
+    def __init__(self, callable: Callable) -> None:
         self.callable = callable
 
-    def __call__(self, instance, item, value):
+    def __call__(self, instance: "DataSet", item: Any, value: Any) -> Any:
         """Evaluate the value of the property given, the instance,
         the item and the value maintained in the instance by the item"""
         return self.callable(instance, item, value)
 
-    def set(self, instance, item, value):
+    def set(self, instance: "DataSet", item: Any, value: Any) -> Any:
         """Sets the value of the property given an instance, item and value
         Depending on implementation the value will be stored either on the
         instance, item or self
         """
         raise NotImplementedError
 
 
 FMT_GROUPS = re.compile(r"(?<!%)%\((\w+)\)")
 
 
 class FormatProp(ItemProperty):
     """A Property that returns a string to help
     custom read-only representation of items"""
 
-    def __init__(self, fmt, ignore_error=True):
+    def __init__(self, fmt: str, ignore_error: Optional[bool] = True) -> None:
         """fmt is a format string
         it can contain a single anonymous substition or
         several named substitions.
         """
         self.fmt = fmt
         self.ignore_error = ignore_error
         self.attrs = FMT_GROUPS.findall(fmt)
 
-    def __call__(self, instance, item, value):
+    def __call__(self, instance: "DataSet", item: "DataItem", value: Any) -> Any:
         if not self.attrs:
-            return self.fmt % value
+            return self.fmt.format(value)
         dic = {}
         for attr in self.attrs:
             dic[attr] = getattr(instance, attr)
         try:
             return self.fmt % dic
         except TypeError:
             if not self.ignore_error:
@@ -78,502 +137,526 @@
                 raise
 
 
 class GetAttrProp(ItemProperty):
     """A property that matches the value of
     an instance's attribute"""
 
-    def __init__(self, attr):
+    def __init__(self, attr: str) -> None:
         self.attr = attr
 
-    def __call__(self, instance, item, value):
+    def __call__(self, instance: "DataSet", item: "DataItem", value: Any) -> Any:
         val = getattr(instance, self.attr)
         return val
 
-    def set(self, instance, item, value):
+    def set(self, instance: "DataSet", item: "DataItem", value: Any) -> None:
         setattr(instance, self.attr, value)
 
 
 class ValueProp(ItemProperty):
     """A property that retrieves a value stored elsewhere"""
 
-    def __init__(self, value):
+    def __init__(self, value: Any) -> None:
         self.value = value
 
-    def __call__(self, instance, item, value):
+    def __call__(self, instance: "DataSet", item: "DataItem", value: Any) -> Any:
         return self.value
 
-    def set(self, instance, item, value):
+    def set(self, instance: "DataSet", item: "DataItem", value: Any) -> None:
         self.value = value
 
 
 class NotProp(ItemProperty):
     """Not property"""
 
-    def __init__(self, prop):
+    def __init__(self, prop: ItemProperty):
         self.property = prop
 
-    def __call__(self, instance, item, value):
+    def __call__(self, instance: "DataSet", item: "DataItem", value: Any) -> Any:
         return not self.property(instance, item, value)
 
-    def set(self, instance, item, value):
+    def set(self, instance: "DataSet", item: "DataItem", value: Any) -> None:
         self.property.set(instance, item, not value)
 
 
 class FuncProp(ItemProperty):
     """An 'operator property'
     prop: ItemProperty instance
     func: function
     invfunc: inverse function (optional)
     """
 
-    def __init__(self, prop, func, invfunc=None):
+    def __init__(
+        self,
+        prop: ItemProperty,
+        func: Callable,
+        invfunc: Optional[Callable] = None,
+    ) -> None:
         self.property = prop
         self.function = func
         if invfunc is None:
             invfunc = func
         self.inverse_function = invfunc
 
-    def __call__(self, instance, item, value):
+    def __call__(self, instance: "DataSet", item: "DataItem", value: Any) -> Any:
         return self.function(self.property(instance, item, value))
 
-    def set(self, instance, item, value):
+    def set(self, instance: "DataSet", item: "DataItem", value: Any) -> None:
         self.property.set(instance, item, self.inverse_function(value))
 
 
-class DataItem(object):
+class DataItem:
     """
     DataSet data item
 
     `label` : string
     `default` : any type, optional
     `help` : string Text displayed on data item's tooltip
     """
 
     count = 0
 
-    def __init__(self, label, default=None, help="", check=True):
+    def __init__(
+        self,
+        label: str,
+        default: Optional[Any] = None,
+        help: Optional[str] = "",
+        check: Optional[bool] = True,
+    ) -> None:
         self._order = DataItem.count
         DataItem.count += 1
-        self._name = None
+        self._name: Optional[str] = None
         self._default = default
-        self._help = utf8_to_unicode(help)
-        self._props = {}  # a dict realm->dict containing realm-specific properties
-        self.set_prop(
-            "display", col=0, colspan=None, row=None, label=utf8_to_unicode(label)
-        )
+        self._help = help
+        self._props: Dict[
+            Any, Any
+        ] = {}  # a dict realm->dict containing realm-specific properties
+        self.set_prop("display", col=0, colspan=None, row=None, label=label)
         self.set_prop("data", check_value=check)
 
-    def get_prop(self, realm, name, default=NoDefault):
+    def get_prop(self, realm: str, name: str, default: Any = NoDefault) -> Any:
         """Get one property of this item"""
         prop = self._props.get(realm)
         if not prop:
             prop = {}
         if default is NoDefault:
             return prop[name]
         return prop.get(name, default)
 
-    def get_prop_value(self, realm, instance, name, default=NoDefault):
+    def get_prop_value(
+        self, realm: str, instance: "DataSet", name: str, default: Any = NoDefault
+    ) -> Any:
         value = self.get_prop(realm, name, default)
         if isinstance(value, ItemProperty):
             return value(instance, self, self.get_value(instance))
         else:
             return value
 
-    def set_prop(self, realm, **kwargs):
+    def set_prop(self, realm: str, **kwargs) -> "DataItem":
         """Set one or several properties using
         the syntax set_prop(name1=value1, ..., nameX=valueX)
 
         it returns self so that we can assign to the result like this:
 
         item = Item().set_prop(x=y)
         """
         prop = self._props.get(realm)
         if not prop:
             prop = {}
             self._props[realm] = prop
         prop.update(kwargs)
         return self
 
-    def set_pos(self, col=0, colspan=None, row=None):
+    def set_pos(
+        self, col: int = 0, colspan: Optional[int] = None, row: Optional[int] = None
+    ) -> "DataItem":
         """
         Set data item's position on a GUI layout
         """
         self.set_prop("display", col=col, colspan=colspan, row=row)
         return self
 
-    def __str__(self):
-        return self._name + ": " + self.__class__.__name__
+    def __str__(self) -> str:
+        return "%s : %s" % (self._name, self.__class__.__name__)
 
-    def get_help(self, instance):
+    def get_help(self, instance: "DataSet") -> str:
         """
         Return data item's tooltip
         """
-        auto_help = utf8_to_unicode(self.get_auto_help(instance))
+        auto_help = self.get_auto_help(instance)
         help = self._help
         if auto_help:
             if help:
                 help = help + "\n(" + auto_help + ")"
             else:
                 help = auto_help.capitalize()
         return help
 
-    def get_auto_help(self, instance):
+    def get_auto_help(self, instance: "DataSet") -> str:
         """
         Return the automatically generated part of data item's tooltip
         """
         return ""
 
-    def format_string(self, instance, value, fmt, func):
+    def format_string(self, instance: Any, value: Any, fmt: str, func: Callable) -> str:
         """Apply format to string representation of the item's value"""
         return fmt % (func(value),)
 
-    def get_string_value(self, instance):
+    def get_string_value(self, instance: "DataSet") -> str:
         """
         Return a formatted unicode representation of the item's value
         obeying 'display' or 'repr' properties
         """
         value = self.get_value(instance)
         repval = self.get_prop_value("display", instance, "repr", None)
         if repval is not None:
             return repval
         else:
             fmt = self.get_prop_value("display", instance, "format", "%s")
             func = self.get_prop_value("display", instance, "func", lambda x: x)
-            if isinstance(fmt, collections.abc.Callable) and value is not None:
+            if (
+                isinstance(fmt, collections.abc.Callable)  # type:ignore
+                and value is not None
+            ):
                 return fmt(func(value))
             if value is not None:
                 text = self.format_string(instance, value, fmt, func)
             else:
                 text = ""
             return text
 
-    def set_name(self, new_name):
+    def set_name(self, new_name: str) -> None:
         """
         Set data item's name
         """
         self._name = new_name
 
-    def set_help(self, new_help):
+    def set_help(self, new_help: str) -> None:
         """
         Set data item's help text
         """
         self._help = new_help
 
-    def set_from_string(self, instance, string_value):
+    def set_from_string(self, instance: "DataSet", string_value: str) -> None:
         """
         Set data item's value from specified string
         """
         value = self.from_string(string_value)
         self.__set__(instance, value)
 
-    def set_default(self, instance):
+    def set_default(self, instance: "DataSet") -> None:
         """
         Set data item's value to default
         """
         self.__set__(instance, self._default)
 
-    def accept(self, visitor):
+    def accept(self, visitor: object) -> None:
         """
         This is the visitor pattern's accept function.
         It calls the corresponding visit_MYCLASS method
         of the visitor object.
 
         Python's allow a generic base class implementation of
         this method so there's no need to write an accept function
         for each derived class unless you need to override the
         default behavior
         """
         funcname = "visit_" + self.__class__.__name__
         func = getattr(visitor, funcname)
         func(self)
 
-    def __set__(self, instance, value):
-        setattr(instance, "_" + self._name, value)
+    def __set__(self, instance: Any, value: Any):
+        setattr(instance, "_%s" % (self._name), value)
 
-    def __get__(self, instance, klass):
+    def __get__(self, instance: Any, klass: type) -> Optional[Any]:
         if instance is not None:
-            return getattr(instance, "_" + self._name, self._default)
+            return getattr(instance, "_%s" % (self._name), self._default)
         else:
             return self
 
-    def get_value(self, instance):
+    def get_value(self, instance: Any) -> Any:
         """
         Return data item's value
         """
         return self.__get__(instance, instance.__class__)
 
-    def check_item(self, instance):
+    def check_item(self, instance: Any) -> Any:
         """
         Check data item's current value (calling method check_value)
         """
-        value = getattr(instance, "_" + self._name)
+        value = getattr(instance, "_%s" % (self._name))
         return self.check_value(value)
 
-    def check_value(self, instance, value):
+    def check_value(self, value: Any) -> Any:
         """
         Check if `value` is valid for this data item
         """
         raise NotImplementedError()
 
-    def from_string(self, instance, string_value):
+    def from_string(self, string_value: str) -> Any:
         """
         Transform string into valid data item's value
         """
         raise NotImplementedError()
 
-    def bind(self, instance):
+    def bind(self, instance: "DataSet") -> "DataItemVariable":
         """
         Return a DataItemVariable instance bound to the data item
         """
         return DataItemVariable(self, instance)
 
-    def serialize(self, instance, writer):
+    def serialize(
+        self,
+        instance: "DataSet",
+        writer: Union["HDF5Writer", "JSONWriter", "UserConfigWriter"],
+    ) -> None:
         """Serialize this item using the writer object
 
         this is a default implementation that should work for
         everything but new datatypes
         """
         value = self.get_value(instance)
         writer.write(value)
 
-    def get_value_from_reader(self, reader):
+    def get_value_from_reader(
+        self, reader: Union["HDF5Reader", "JSONReader", "UserConfigReader"]
+    ) -> Any:
         """Reads value from the reader object, inside the try...except
         statement defined in the base item `deserialize` method
 
         This method is reimplemented in some child classes"""
         return reader.read_any()
 
-    def deserialize(self, instance, reader):
+    def deserialize(
+        self,
+        instance: Any,
+        reader: Union["HDF5Reader", "JSONReader", "UserConfigReader"],
+    ) -> None:
         """Deserialize this item using the reader object
 
         Default base implementation supposes the reader can
         detect expected datatype from the stream
         """
         try:
             value = self.get_value_from_reader(reader)
+        except KeyError:
+            self.set_default(instance)
+            return
         except RuntimeError as e:
             if DEBUG_DESERIALIZE:
                 import traceback
 
                 print("DEBUG_DESERIALIZE enabled in datatypes.py", file=sys.stderr)
                 traceback.print_stack()
                 print(e, file=sys.stderr)
             self.set_default(instance)
             return
         self.__set__(instance, value)
 
 
-class Obj(object):
+class Obj:
     """An object that helps build default instances for
     ObjectItems"""
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs) -> None:
         self.__dict__.update(kwargs)
 
 
 class ObjectItem(DataItem):
     """Simple helper class implementing default
     for composite objects"""
 
-    klass = None
+    klass: Optional[Type] = None
 
-    def set_default(self, instance):
+    def set_default(self, instance: "DataSet") -> None:
         """Make a copy of the default value"""
-        value = self.klass()
-        if self._default is not None:
-            update_dataset(value, self._default)
-        self.__set__(instance, value)
-
-    def deserialize(self, instance, reader):
+        if self.klass is not None:
+            value = self.klass()
+            if self._default is not None:
+                update_dataset(value, self._default)
+            self.__set__(instance, value)
+
+    def deserialize(
+        self,
+        instance: "DataSet",
+        reader: Union["HDF5Reader", "JSONReader", "UserConfigReader"],
+    ) -> None:
         """Deserialize this item using the reader object
 
         We build a new default object and deserialize it
         """
-        value = self.klass()
-        value.deserialize(reader)
-        self.__set__(instance, value)
+        if self.klass is not None:
+            value = self.klass()
+            value.deserialize(reader)
+            self.__set__(instance, value)
 
 
-class DataItemProxy(object):
+class DataItemProxy:
     """
     Proxy for DataItem objects
 
     This class is needed to construct GroupItem class
     (see module guidata.qtwidgets)
     """
 
-    def __init__(self, item):
+    def __init__(self, item: "DataItem"):
         self.item = item
 
     def __str__(self):
         return self.item._name + "_proxy: " + self.__class__.__name__
 
-    def get_help(self, instance):
+    def get_help(self, instance: "DataSet") -> str:
         """DataItem method proxy"""
         return self.item.get_help(instance)
 
-    def get_auto_help(self, instance):
+    def get_auto_help(self, instance: "DataSet") -> str:
         """DataItem method proxy"""
         return self.item.get_auto_help(instance)
 
-    def get_string_value(self, instance):
+    def get_string_value(self, instance: "DataSet") -> str:
         """DataItem method proxy"""
         return self.item.get_string_value(instance)
 
-    def set_from_string(self, instance, string_value):
+    def set_from_string(self, instance: "DataSet", string_value: str) -> None:
         """DataItem method proxy"""
-        return self.item.set_from_string(instance, string_value)
+        self.item.set_from_string(instance, string_value)
 
-    def set_default(self, instance):
+    def set_default(self, instance: "DataSet") -> None:
         """DataItem method proxy"""
-        return self.item.set_default(instance)
+        self.item.set_default(instance)
 
-    def accept(self, visitor):
+    def __set__(self, instance: Any, value: Any):
+        pass
+
+    def accept(self, visitor: "object") -> None:
         """DataItem method proxy"""
-        return self.item.accept(visitor)
+        self.item.accept(visitor)
 
-    def get_value(self, instance):
+    def get_value(self, instance: "DataItem") -> Any:
         """DataItem method proxy"""
         return self.item.get_value(instance)
 
-    def check_item(self, instance):
+    def check_item(self, instance: "DataItem") -> Any:
         """DataItem method proxy"""
         return self.item.check_item(instance)
 
-    def check_value(self, instance, value):
+    def check_value(self, value: Any) -> Any:
         """DataItem method proxy"""
-        return self.item.check_value(instance, value)
+        return self.item.check_value(value)
 
-    def from_string(self, instance, string_value):
+    def from_string(self, string_value: str) -> Any:
         """DataItem method proxy"""
-        return self.item.from_string(instance, string_value)
+        return self.item.from_string(string_value)
 
-    def get_prop(self, realm, name, default=NoDefault):
+    def get_prop(self, realm: str, name: str, default=NoDefault) -> Any:
         """DataItem method proxy"""
         return self.item.get_prop(realm, name, default)
 
-    def get_prop_value(self, realm, instance, name, default=NoDefault):
+    def get_prop_value(
+        self, realm, instance: "DataSet", name: str, default: Any = NoDefault
+    ) -> Any:
         """DataItem method proxy"""
         return self.item.get_prop_value(realm, instance, name, default)
 
-    def set_prop(self, realm, **kwargs):
+    def set_prop(self, realm: str, **kwargs) -> "DataItem":
         """DataItem method proxy"""
         return self.item.set_prop(realm, **kwargs)
 
-    def bind(self, instance):
+    def bind(self, instance: "DataSet") -> "DataItemVariable":
         """DataItem method proxy"""
         return DataItemVariable(self, instance)
 
 
-#    def __getattr__(self, name):
-#        assert name in ["min_equals_max", "get_min", "get_max",
-#                        "_formats", "_text", "_choices", "_shape",
-#                        "_format", "_label", "_xy"]
-#        val = getattr(self.item, name)
-#        if callable(val):
-#            return bind(val, self.instance)
-#        else:
-#            return val
-
-
-class DataItemVariable(object):
+class DataItemVariable:
     """An instance of a DataItemVariable represent a binding between
     an item and a dataset.
 
     could be called a bound property.
 
     since DataItem instances are class attributes they need to have a
     DataSet instance to store their value. This class binds the two
     together.
     """
 
-    def __init__(self, item, instance):
+    def __init__(
+        self,
+        item: "DataItem",
+        instance: "DataSet",
+    ):
         self.item = item
         self.instance = instance
 
-    def get_prop_value(self, realm, name, default=NoDefault):
+    def get_prop_value(self, realm: str, name: str, default: object = NoDefault) -> Any:
         """DataItem method proxy"""
         return self.item.get_prop_value(realm, self.instance, name, default)
 
-    def get_prop(self, realm, name, default=NoDefault):
+    def get_prop(
+        self, realm: str, name: str, default: Optional[type] = NoDefault
+    ) -> Any:
         """DataItem method proxy"""
         return self.item.get_prop(realm, name, default)
 
-    #    def set_prop(self, realm, **kwargs):
-    #        """DataItem method proxy"""
-    #        self.item.set_prop(realm, **kwargs)
-    #
-    #    def __getattr__(self, name):
-    #        assert name in ["min_equals_max", "get_min", "get_max",
-    #                        "_formats","_text", "_choices", "_shape",
-    #                        "_format", "_label", "_xy"]
-    #        val = getattr(self.item, name)
-    #        if callable(val):
-    #            return bind(val, self.instance)
-    #        else:
-    #            return val
-    def get_help(self):
+    def get_help(self) -> str:
         """Re-implement DataItem method"""
         return self.item.get_help(self.instance)
 
-    def get_auto_help(self):
+    def get_auto_help(self) -> str:
         """Re-implement DataItem method"""
         # XXX incohérent ?
         return self.item.get_auto_help(self.instance)
 
-    def get_string_value(self):
+    def get_string_value(self) -> str:
         """
         Return a unicode representation of the item's value
         obeying 'display' or 'repr' properties
         """
         return self.item.get_string_value(self.instance)
 
-    def set_default(self):
+    def set_default(self) -> None:
         """Re-implement DataItem method"""
         return self.item.set_default(self.instance)
 
-    def get(self):
+    def get(self) -> Any:
         """Re-implement DataItem method"""
         return self.item.get_value(self.instance)
 
-    def set(self, value):
+    def set(self, value: Any) -> None:
         """Re-implement DataItem method"""
         return self.item.__set__(self.instance, value)
 
-    def set_from_string(self, string_value):
+    def set_from_string(self, string_value) -> None:
         """Re-implement DataItem method"""
         return self.item.set_from_string(self.instance, string_value)
 
-    def check_item(self):
+    def check_item(self) -> Any:
         """Re-implement DataItem method"""
         return self.item.check_item(self.instance)
 
-    def check_value(self, value):
+    def check_value(self, value) -> Any:
         """Re-implement DataItem method"""
         return self.item.check_value(value)
 
-    def from_string(self, string_value):
+    def from_string(self, string_value: str) -> Any:
         """Re-implement DataItem method"""
         return self.item.from_string(string_value)
 
-    def label(self):
+    def label(self) -> str:
         """Re-implement DataItem method"""
         return self.item.get_prop("display", "label")
 
 
 class DataSetMeta(type):
     """
     DataSet metaclass
 
     Create class attribute `_items`: list of the DataSet class attributes,
     created in the same order as these attributes were written
     """
 
-    def __new__(cls, name, bases, dct):
+    def __new__(cls: Type, name: str, bases: Any, dct: Dict[str, Any]) -> Type:
         items = {}
         for base in bases:
             if getattr(base, "__metaclass__", None) is DataSetMeta:
                 for item in base._items:
                     items[item._name] = item
 
         for attrname, value in list(dct.items()):
@@ -587,202 +670,247 @@
         dct["_items"] = items_list
         return type.__new__(cls, name, bases, dct)
 
 
 Meta_Py3Compat = DataSetMeta("Meta_Py3Compat", (object,), {})
 
 
-class DataSet(Meta_Py3Compat):
+class DataSet(metaclass=DataSetMeta):
     """
     Construct a DataSet object is a set of DataItem objects
         * title [string]
         * comment [string]: text shown on the top of the first data item
         * icon [QIcon or string]: icon show on the button (optional)
           (string: icon filename as in guidata/guiqwt image search paths)
     """
 
+    _items: List["DataItem"]
     __metaclass__ = DataSetMeta  # keep it even with Python 3 (see DataSetMeta)
 
-    def __init__(self, title=None, comment=None, icon=""):
-        self.__title = title
+    def __init__(
+        self,
+        title: Optional[str] = None,
+        comment: Optional[str] = None,
+        icon: str = "",
+    ):
         self.__comment = comment
         self.__icon = icon
         comp_title, comp_comment = self._compute_title_and_comment()
-        if title is None:
+        if title:
+            self.__title = title
+        else:
             self.__title = comp_title
         if comment is None:
             self.__comment = comp_comment
         self.__changed = False
         # Set default values
         self.set_defaults()
 
+    @classmethod
+    def create(cls, **kwargs) -> "DataSet":
+        """Create a new instance of the DataSet class
+
+        Args:
+            \*\*kwargs: keyword arguments to set the DataItem values
+
+        Returns:
+            DataSet instance
+        """
+        instance = cls()
+        for item in instance._items:
+            name = item._name
+            if name in kwargs:
+                setattr(instance, name, kwargs[name])
+        return instance
+
     def _get_translation(self):
         """We try to find the translation function (_) from the module
         this class was created in
 
         This function is unused but could be useful to translate strings that
         cannot be translated at the time they are created.
         """
         module = sys.modules[self.__class__.__module__]
         if hasattr(module, "_"):
             return module._
         else:
             return lambda x: x
 
-    def _compute_title_and_comment(self):
+    def _compute_title_and_comment(self) -> Tuple[str, Optional[str]]:
         """
         Private method to compute title and comment of the data set
         """
         comp_title = self.__class__.__name__
         comp_comment = None
         if self.__doc__:
-            doc_lines = utf8_to_unicode(self.__doc__).splitlines()
+            doc_lines = self.__doc__.splitlines()
             # Remove empty lines at the begining of comment
             while doc_lines and not doc_lines[0].strip():
                 del doc_lines[0]
             if doc_lines:
                 comp_title = doc_lines.pop(0).strip()
             if doc_lines:
                 comp_comment = "\n".join([x.strip() for x in doc_lines])
         return comp_title, comp_comment
 
-    def get_title(self):
+    def get_title(self) -> str:
         """
         Return data set title
         """
         return self.__title
 
-    def get_comment(self):
+    def get_comment(self) -> Optional[str]:
         """
         Return data set comment
         """
         return self.__comment
 
-    def get_icon(self):
+    def get_icon(self) -> Optional[str]:
         """
         Return data set icon
         """
         return self.__icon
 
-    def set_defaults(self):
+    def set_defaults(self) -> None:
         """Set default values"""
         for item in self._items:
             item.set_default(self)
 
     def __str__(self):
         return self.to_string(debug=False)
 
-    def check(self):
+    def check(self) -> List[str]:
         """
         Check the dataset item values
         """
         errors = []
         for item in self._items:
-            if not item.check_item(self):
+            if not item.check_item(self) and item._name is not None:
                 errors.append(item._name)
         return errors
 
-    def text_edit(self):
+    def text_edit(self) -> None:
         """
         Edit data set with text input only
         """
         from guidata.dataset import textedit
 
         self.accept(textedit.TextEditVisitor(self))
 
-    def edit(self, parent=None, apply=None, size=None):
+    def edit(
+        self,
+        parent: Optional[QWidget] = None,
+        apply: Optional[Callable] = None,
+        size: Optional[Any] = None,
+    ) -> "DataSetEditDialog":
         """
         Open a dialog box to edit data set
             * parent: parent widget (default is None, meaning no parent)
             * apply: apply callback (default is None)
             * size: dialog size (QSize object or integer tuple (width, height))
         """
         from guidata.dataset.qtwidgets import DataSetEditDialog
 
-        win = DataSetEditDialog(
+        dial = DataSetEditDialog(
             self, icon=self.__icon, parent=parent, apply=apply, size=size
         )
-        return win.exec_()
+        return exec_dialog(dial)
 
-    def view(self, parent=None, size=None):
+    def view(self, parent: Optional[QWidget] = None, size: Optional[Any] = None):
         """
         Open a dialog box to view data set
             * parent: parent widget (default is None, meaning no parent)
             * size: dialog size (QSize object or integer tuple (width, height))
         """
         from guidata.dataset.qtwidgets import DataSetShowDialog
 
-        win = DataSetShowDialog(self, icon=self.__icon, parent=parent, size=size)
-        return win.exec_()
+        dial = DataSetShowDialog(self, icon=self.__icon, parent=parent, size=size)
+        return exec_dialog(dial)
 
-    def to_string(self, debug=False, indent=None, align=False):
+    def to_string(
+        self,
+        debug: Optional[bool] = False,
+        indent: Optional[str] = None,
+        align: Optional[bool] = False,
+        show_hidden: Optional[bool] = True,
+    ):
         """
         Return readable string representation of the data set
         If debug is True, add more details on data items
         """
         if indent is None:
             indent = "\n    "
-        txt = self.__title + ":"
+        txt = "%s:" % (self.__title)
 
         def _get_label(item):
             if debug:
                 return item._name
             else:
                 return item.get_prop_value("display", self, "label")
 
         length = 0
         if align:
             for item in self._items:
                 item_length = len(_get_label(item))
                 if item_length > length:
                     length = item_length
         for item in self._items:
+            try:
+                hide = item.get_prop_value("display", self, "hide")
+                if not show_hidden and hide is True:
+                    continue
+            except KeyError:
+                pass
             if isinstance(item, ObjectItem):
                 composite_dataset = item.get_value(self)
                 txt += indent + composite_dataset.to_string(
                     debug=debug, indent=indent + "  "
                 )
                 continue
             elif isinstance(item, BeginGroup):
-                txt += indent + item._name + ":"
+                txt += "%s%s:" % (indent, item._name)
                 indent += "  "
                 continue
             elif isinstance(item, EndGroup):
                 indent = indent[:-2]
                 continue
-            value = getattr(self, "_" + item._name)
+            value = getattr(self, "_%s" % (item._name))
             if value is None:
                 value_str = "-"
             else:
                 value_str = item.get_string_value(self)
             if debug:
                 label = item._name
             else:
                 label = item.get_prop_value("display", self, "label")
-            if length:
+            if length and label is not None:
                 label = label.ljust(length)
-            txt += indent + label + ": " + value_str
+            txt += "%s%s: %s" % (indent, label, value_str)
             if debug:
                 txt += " (" + item.__class__.__name__ + ")"
         return txt
 
-    def accept(self, vis):
+    def accept(self, vis: object) -> None:
         """
         helper function that passes the visitor to the accept methods of all
         the items in this dataset
         """
         for item in self._items:
             item.accept(vis)
 
-    def serialize(self, writer):
+    def serialize(
+        self, writer: Union["HDF5Writer", "JSONWriter", "UserConfigWriter"]
+    ) -> None:
         for item in self._items:
             with writer.group(item._name):
                 item.serialize(self, writer)
 
-    def deserialize(self, reader):
+    def deserialize(
+        self, reader: Union["HDF5Reader", "JSONReader", "UserConfigReader"]
+    ) -> None:
         for item in self._items:
             with reader.group(item._name):
                 try:
                     item.deserialize(self, reader)
                 except RuntimeError as error:
                     if DEBUG_DESERIALIZE:
                         import traceback
@@ -790,28 +918,28 @@
                         print(
                             "DEBUG_DESERIALIZE enabled in datatypes.py", file=sys.stderr
                         )
                         traceback.print_stack()
                         print(error, file=sys.stderr)
                     item.set_default(self)
 
-    def read_config(self, conf, section, option):
-        from guidata.userconfigio import UserConfigReader
+    def read_config(self, conf: "UserConfig", section: str, option: str) -> None:
+        from guidata.dataset.iniio import UserConfigReader
 
         reader = UserConfigReader(conf, section, option)
         self.deserialize(reader)
 
-    def write_config(self, conf, section, option):
-        from guidata.userconfigio import UserConfigWriter
+    def write_config(self, conf: "UserConfig", section: str, option: str) -> None:
+        from guidata.dataset.iniio import UserConfigWriter
 
         writer = UserConfigWriter(conf, section, option)
         self.serialize(writer)
 
     @classmethod
-    def set_global_prop(klass, realm, **kwargs):
+    def set_global_prop(klass, realm: str, **kwargs) -> None:
         for item in klass._items:
             item.set_prop(realm, **kwargs)
 
 
 class ActivableDataSet(DataSet):
     """
     An ActivableDataSet instance must have an "enable" class attribute which
@@ -820,153 +948,175 @@
     """
 
     _ro = True  # default *instance* attribute value
     _active = True
     _ro_prop = GetAttrProp("_ro")
     _active_prop = GetAttrProp("_active")
 
-    def __init__(self, title=None, comment=None, icon=""):
+    @property
+    @abstractmethod
+    def enable(self) -> "DataItem":
+        ...
+
+    def __init__(
+        self,
+        title: Optional[str] = None,
+        comment: Optional[str] = None,
+        icon: str = "",
+    ):
         DataSet.__init__(self, title, comment, icon)
 
     #        self.set_readonly()
 
     @classmethod
-    def active_setup(klass):
+    def active_setup(cls) -> None:
         """
         This class method must be called after the child class definition
         in order to setup the dataset active state
         """
-        klass.set_global_prop("display", active=klass._active_prop)
-        klass.enable.set_prop(
-            "display", active=True, hide=klass._ro_prop, store=klass._active_prop
+        cls.set_global_prop("display", active=cls._active_prop)
+        cls.enable.set_prop(  # type:ignore
+            "display", active=True, hide=cls._ro_prop, store=cls._active_prop
         )
 
-    def set_readonly(self):
+    def set_readonly(self) -> None:
         """
         The dataset is now in read-only mode, i.e. all data items are disabled
         """
         self._ro = True
         self._active = self.enable
 
-    def set_writeable(self):
+    def set_writeable(self) -> None:
         """
         The dataset is now in read/write mode, i.e. all data items are enabled
         """
         self._ro = False
         self._active = self.enable
 
 
-class DataSetGroup(object):
+class DataSetGroup:
     """
     Construct a DataSetGroup object, used to group several datasets together
         * datasets [list of DataSet objects]
         * title [string]
         * icon [QIcon or string]: icon show on the button (optional)
           (string: icon filename as in guidata/guiqwt image search paths)
 
     This class tries to mimics the DataSet interface.
 
     The GUI should represent it as a notebook with one page for each
     contained dataset.
     """
 
-    def __init__(self, datasets, title=None, icon=""):
+    def __init__(
+        self, datasets: List["DataSet"], title: Optional[str] = None, icon: str = ""
+    ) -> None:
         self.__icon = icon
         self.datasets = datasets
         if title:
             self.__title = title
         else:
             self.__title = self.__class__.__name__
 
-    def __str__(self):
+    def __str__(self) -> str:
         return "\n".join([dataset.__str__() for dataset in self.datasets])
 
-    def get_title(self):
+    def get_title(self) -> str:
         """
         Return data set group title
         """
         return self.__title
 
-    def get_comment(self):
+    def get_comment(self) -> None:
         """
         Return data set group comment --> not implemented (will return None)
         """
         return None
 
-    def check(self):
+    def get_icon(self) -> Union[str, None]:
+        """
+        Return data set icon
+        """
+        return self.__icon
+
+    def check(self) -> List[List[str]]:
         """
         Check data set group items
         """
         return [dataset.check() for dataset in self.datasets]
 
-    def text_edit(self):
+    def text_edit(self) -> None:
         """
         Edit data set with text input only
         """
         raise NotImplementedError()
 
-    def edit(self, parent=None, apply=None):
+    def edit(
+        self, parent: Optional[QWidget] = None, apply: Optional[Callable] = None
+    ) -> int:
         """
         Open a dialog box to edit data set
         """
         from guidata.dataset.qtwidgets import DataSetGroupEditDialog
 
-        win = DataSetGroupEditDialog(self, icon=self.__icon, parent=parent, apply=apply)
-        return win.exec_()
+        dial = DataSetGroupEditDialog(
+            self, icon=self.__icon, parent=parent, apply=apply
+        )
+        return exec_dialog(dial)
 
-    def accept(self, vis):
+    def accept(self, vis: object) -> None:
         """
         helper function that passes the visitor to the accept methods of all
         the items in this dataset
         """
         for dataset in self.datasets:
             dataset.accept(vis)
 
 
 class GroupItem(DataItemProxy):
     """GroupItem proxy"""
 
-    def __init__(self, item):
+    def __init__(self, item: "DataItem") -> None:
         DataItemProxy.__init__(self, item)
-        self.group = []
+        self.group: List[Any] = []
 
 
 class BeginGroup(DataItem):
     """
     Data item which does not represent anything
     but a begin flag to define a data set group
     """
 
-    def serialize(self, instance, writer):
+    def serialize(self, instance, writer) -> None:
         pass
 
-    def deserialize(self, instance, reader):
+    def deserialize(self, instance, reader) -> None:
         pass
 
-    def get_group(self):
+    def get_group(self) -> "GroupItem":
         return GroupItem(self)
 
 
 class EndGroup(DataItem):
     """
     Data item which does not represent anything
     but an end flag to define a data set group
     """
 
-    def serialize(self, instance, writer):
+    def serialize(self, instance, writer) -> None:
         pass
 
-    def deserialize(self, instance, reader):
+    def deserialize(self, instance, reader) -> None:
         pass
 
 
 class TabGroupItem(GroupItem):
     pass
 
 
 class BeginTabGroup(BeginGroup):
-    def get_group(self):
+    def get_group(self) -> "TabGroupItem":
         return TabGroupItem(self)
 
 
 class EndTabGroup(EndGroup):
     pass
```

### Comparing `guidata-2.3.1/guidata/dataset/qtitemwidgets.py` & `guidata-3.0.0/guidata/dataset/qtitemwidgets.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,173 +1,188 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright © 2009-2010 CEA
-# Pierre Raybaut
-# Licensed under the terms of the CECILL License
-# (see guidata/__init__.py for details)
+# Licensed under the terms of the BSD 3-Clause
+# (see guidata/LICENSE for details)
 
 """
 dataset.qtitemwidgets
 =====================
 
 Widget factories used to edit data items
 (factory registration is done in guidata.dataset.qtwidgets)
 (data item types are defined in guidata.dataset.datatypes)
 
 There is one widget type for each data item type.
 Example: ChoiceWidget <--> ChoiceItem, ImageChoiceItem
 """
-
+import collections.abc
+import datetime
 import os
 import os.path as osp
 import sys
-import numpy
-import collections.abc
-import datetime
+from abc import abstractmethod
+from typing import TYPE_CHECKING, Any, Callable, List, Optional, Protocol
 
+import numpy
+from qtpy.compat import getexistingdirectory
+from qtpy.QtCore import Qt, QVariant
+from qtpy.QtGui import QColor, QIcon, QPixmap
 from qtpy.QtWidgets import (
-    QHBoxLayout,
-    QGridLayout,
-    QColorDialog,
-    QPushButton,
-    QLineEdit,
+    QAbstractButton,
     QCheckBox,
+    QColorDialog,
     QComboBox,
-    QTabWidget,
-    QGroupBox,
+    QDateEdit,
     QDateTimeEdit,
-    QLabel,
-    QTextEdit,
     QFrame,
-    QDateEdit,
-    QSlider,
+    QGridLayout,
+    QGroupBox,
+    QHBoxLayout,
+    QLabel,
+    QLineEdit,
+    QPushButton,
     QRadioButton,
+    QSlider,
+    QTabWidget,
+    QTextEdit,
     QVBoxLayout,
+    QWidget,
 )
-from qtpy.QtGui import QColor, QIcon, QPixmap
-from qtpy.QtCore import Qt, Signal
-from qtpy.compat import getexistingdirectory
 
-from guidata.utils import update_dataset, restore_dataset, utf8_to_unicode
-from guidata.qthelpers import text_to_qcolor, get_std_icon
-from guidata.configtools import get_icon, get_image_layout, get_image_file_path
 from guidata.config import _
+from guidata.configtools import get_icon, get_image_file_path, get_image_layout
+from guidata.dataset.datatypes import DataItemVariable
+from guidata.qthelpers import get_std_icon, text_to_qcolor
+from guidata.utils import restore_dataset, update_dataset
 from guidata.widgets.arrayeditor import ArrayEditor
 
 # ========================== <!> IMPORTANT <!> =================================
 #
 # In this module, `item` is an instance of DataItemVariable (not DataItem)
 # (see guidata.datatypes for details)
 #
 # ========================== <!> IMPORTANT <!> =================================
 
 # XXX: consider providing an interface here...
 
+if TYPE_CHECKING:  # pragma: no cover
+    from guidata.dataset.qtwidgets import DataSetEditLayout
+
 
-class AbstractDataSetWidget(object):
+class AbstractDataSetWidget:
     """
     Base class for 'widgets' handled by `DataSetEditLayout` and it's derived
     classes.
 
     This is a generic representation of an input (or display) widget that
     has a label and one or more entry field.
 
     `DataSetEditLayout` uses a registry of *Item* to *Widget* mapping in order
     to automatically create a GUI for a `DataSet` structure
     """
 
     READ_ONLY = False
 
-    def __init__(self, item, parent_layout):
+    def __init__(
+        self, item: "DataItemVariable", parent_layout: "DataSetEditLayout"
+    ) -> None:
         """Derived constructors should create the necessary widgets
         The base class keeps a reference to item and parent
         """
         self.item = item
         self.parent_layout = parent_layout
-        self.group = None  # Layout/Widget grouping items
-        self.label = None
+        self.group: Any = None  # Layout/Widget grouping items
+        self.label: Optional[QLabel] = None
         self.build_mode = False
 
-    def place_label(self, layout, row, column):
+    def place_label(self, layout: QGridLayout, row: int, column: int) -> None:
         """
         Place item label on layout at specified position (row, column)
         """
         label_text = self.item.get_prop_value("display", "label")
         unit = self.item.get_prop_value("display", "unit", "")
         if unit and not self.READ_ONLY:
             label_text += " (%s)" % unit
         self.label = QLabel(label_text)
         self.label.setToolTip(self.item.get_help())
         layout.addWidget(self.label, row, column)
 
     def place_on_grid(
-        self, layout, row, label_column, widget_column, row_span=1, column_span=1
-    ):
+        self,
+        layout: QGridLayout,
+        row: int,
+        label_column: int,
+        widget_column: int,
+        row_span: int = 1,
+        column_span: int = 1,
+    ) -> None:
         """
         Place widget on layout at specified position
         """
         self.place_label(layout, row, label_column)
         layout.addWidget(self.group, row, widget_column, row_span, column_span)
 
-    def is_active(self):
+    def is_active(self) -> bool:
         """
         Return True if associated item is active
         """
         return self.item.get_prop_value("display", "active", True)
 
-    def check(self):
+    def check(self) -> bool:
         """
         Item validator
         """
         return True
 
-    def set(self):
+    def set(self) -> None:
         """
         Update data item value from widget contents
         """
         # XXX: consider using item.set instead of item.set_from_string...
         self.item.set_from_string(self.value())
 
-    def get(self):
+    def get(self) -> Any:
         """
         Update widget contents from data item value
         """
         pass
 
-    def value(self):
+    def value(self) -> Any:
         """
         Returns the widget's current value
         """
         return None
 
-    def set_state(self):
+    def set_state(self) -> None:
         """
         Update the visual status of the widget
         """
         active = self.is_active()
         if self.group:
             self.group.setEnabled(active)
         if self.label:
             self.label.setEnabled(active)
 
-    def notify_value_change(self):
+    def notify_value_change(self) -> None:
         """
         Notify parent layout that widget value has changed
         """
         if not self.build_mode:
             self.parent_layout.widget_value_changed()
 
 
 class GroupWidget(AbstractDataSetWidget):
     """
     GroupItem widget
     """
 
-    def __init__(self, item, parent_layout):
-        super(GroupWidget, self).__init__(item, parent_layout)
+    def __init__(
+        self, item: "DataItemVariable", parent_layout: "DataSetEditLayout"
+    ) -> None:
+        super().__init__(item, parent_layout)
         embedded = item.get_prop_value("display", "embedded", False)
         if not embedded:
             self.group = QGroupBox(item.get_prop_value("display", "label"))
         else:
             self.group = QFrame()
         self.layout = QGridLayout()
         EditLayoutClass = parent_layout.__class__
@@ -176,391 +191,468 @@
             item.instance,
             self.layout,
             item.item.group,
             change_callback=self.notify_value_change,
         )
         self.group.setLayout(self.layout)
 
-    def get(self):
+    def get(self) -> None:
         """Override AbstractDataSetWidget method"""
         self.edit.update_widgets()
 
-    def set(self):
+    def set(self) -> None:
         """Override AbstractDataSetWidget method"""
         self.edit.accept_changes()
 
-    def check(self):
+    def check(self) -> bool:
         """Override AbstractDataSetWidget method"""
         return self.edit.check_all_values()
 
     def place_on_grid(
-        self, layout, row, label_column, widget_column, row_span=1, column_span=1
-    ):
+        self,
+        layout: QGridLayout,
+        row: int,
+        label_column: int,
+        widget_column: int,
+        row_span: int = 1,
+        column_span: int = 1,
+    ) -> None:
         """Override AbstractDataSetWidget method"""
         layout.addWidget(self.group, row, label_column, row_span, column_span + 1)
 
 
 class TabGroupWidget(AbstractDataSetWidget):
-    def __init__(self, item, parent_layout):
-        super(TabGroupWidget, self).__init__(item, parent_layout)
+    def __init__(
+        self, item_var: "DataItemVariable", parent_layout: "DataSetEditLayout"
+    ) -> None:
+        super().__init__(item_var, parent_layout)
         self.tabs = QTabWidget()
-        items = item.item.group
+        items = item_var.item.group
         self.widgets = []
         for item in items:
             if item.get_prop_value("display", parent_layout.instance, "hide", False):
                 continue
             item.set_prop("display", embedded=True)
             widget = parent_layout.build_widget(item)
             frame = QFrame()
             label = widget.item.get_prop_value("display", "label")
             icon = widget.item.get_prop_value("display", "icon", None)
             if icon is not None:
                 self.tabs.addTab(frame, get_icon(icon), label)
             else:
                 self.tabs.addTab(frame, label)
             layout = QGridLayout()
-            layout.setAlignment(Qt.AlignTop)
+            layout.setAlignment(Qt.AlignTop)  # type:ignore
             frame.setLayout(layout)
             widget.place_on_grid(layout, 0, 0, 1)
             try:
                 widget.get()
             except Exception:
                 print("Error building item :", item.item._name)
                 raise
             self.widgets.append(widget)
 
-    def get(self):
+    def get(self) -> Any:
         """Override AbstractDataSetWidget method"""
         for widget in self.widgets:
             widget.get()
 
-    def set(self):
+    def set(self) -> Any:
         """Override AbstractDataSetWidget method"""
         for widget in self.widgets:
             widget.set()
 
-    def check(self):
+    def check(self) -> bool:
         """Override AbstractDataSetWidget method"""
         return True
 
     def place_on_grid(
-        self, layout, row, label_column, widget_column, row_span=1, column_span=1
-    ):
+        self,
+        layout: QGridLayout,
+        row: int,
+        label_column: int,
+        widget_column: int,
+        row_span: int = 1,
+        column_span: int = 1,
+    ) -> None:
         """Override AbstractDataSetWidget method"""
         layout.addWidget(self.tabs, row, label_column, row_span, column_span + 1)
 
 
+def _display_callback(widget: AbstractDataSetWidget, value):
+    """Handling of display callback"""
+    cb = widget.item.get_prop_value("display", "callback", None)
+    if cb is not None:
+        if widget.build_mode:
+            widget.set()
+        else:
+            widget.parent_layout.update_dataitems()
+        cb(widget.item.instance, widget.item.item, value)
+        widget.parent_layout.update_widgets(except_this_one=widget)
+
+
 class LineEditWidget(AbstractDataSetWidget):
     """
     QLineEdit-based widget
     """
 
-    def __init__(self, item, parent_layout):
-        super(LineEditWidget, self).__init__(item, parent_layout)
+    def __init__(
+        self, item: "DataItemVariable", parent_layout: "DataSetEditLayout"
+    ) -> None:
+        super().__init__(item, parent_layout)
         self.edit = self.group = QLineEdit()
         self.edit.setToolTip(item.get_help())
-        if hasattr(item, "min_equals_max") and item.min_equals_max():
-            if item.check_item():
-                self.edit.setEnabled(False)
-            self.edit.setToolTip(_("Value is forced to %d") % item.get_max())
-        self.edit.textChanged.connect(self.line_edit_changed)
+        self.edit.textChanged.connect(self.line_edit_changed)  # type:ignore
 
-    def get(self):
+    def get(self) -> None:
         """Override AbstractDataSetWidget method"""
         value = self.item.get()
         old_value = str(self.value())
         if value is not None:
             if isinstance(value, QColor):  # if item is a ColorItem object
                 value = value.name()
-            uvalue = utf8_to_unicode(value)
-            if uvalue != old_value:
-                self.edit.setText(utf8_to_unicode(value))
+            value = str(value)
+            if value != old_value:
+                self.edit.setText(value)
         else:
             self.line_edit_changed(value)
 
-    def line_edit_changed(self, qvalue):
+    def line_edit_changed(self, qvalue: Optional[QVariant]) -> None:
         """QLineEdit validator"""
         if qvalue is not None:
             value = self.item.from_string(str(qvalue))
         else:
             value = None
         if not self.item.check_value(value):
             self.edit.setStyleSheet("background-color:rgb(255, 175, 90);")
         else:
             self.edit.setStyleSheet("")
-            cb = self.item.get_prop_value("display", "callback", None)
-            if cb is not None:
-                if self.build_mode:
-                    self.set()
-                else:
-                    self.parent_layout.update_dataitems()
-                cb(self.item.instance, self.item.item, value)
-                self.parent_layout.update_widgets(except_this_one=self)
+            _display_callback(self, value)
         self.update(value)
         self.notify_value_change()
 
-    def update(self, value):
+    def update(self, value: Any) -> None:
         """Override AbstractDataSetWidget method"""
         cb = self.item.get_prop_value("display", "value_callback", None)
         if cb is not None:
             cb(value)
 
-    def value(self):
+    def value(self) -> str:
         return str(self.edit.text())
 
-    def check(self):
+    def check(self) -> Any:
         """Override AbstractDataSetWidget method"""
         value = self.item.from_string(str(self.edit.text()))
         return self.item.check_value(value)
 
 
 class TextEditWidget(AbstractDataSetWidget):
     """
     QTextEdit-based widget
     """
 
-    def __init__(self, item, parent_layout):
-        super(TextEditWidget, self).__init__(item, parent_layout)
+    def __init__(
+        self, item: "DataItemVariable", parent_layout: "DataSetEditLayout"
+    ) -> None:
+        super().__init__(item, parent_layout)
         self.edit = self.group = QTextEdit()
         self.edit.setToolTip(item.get_help())
-        if hasattr(item, "min_equals_max") and item.min_equals_max():
-            if item.check_item():
-                self.edit.setEnabled(False)
-            self.edit.setToolTip(_("Value is forced to %d") % item.get_max())
-        self.edit.textChanged.connect(self.text_changed)
+        self.edit.textChanged.connect(self.text_changed)  # type:ignore
 
-    def __get_text(self):
+    def __get_text(self) -> str:
         """Get QTextEdit text, replacing UTF-8 EOL chars by os.linesep"""
         return str(self.edit.toPlainText()).replace("\u2029", os.linesep)
 
-    def get(self):
+    def get(self) -> None:
         """Override AbstractDataSetWidget method"""
         value = self.item.get()
         if value is not None:
-            self.edit.setPlainText(utf8_to_unicode(value))
+            self.edit.setPlainText(value)
         self.text_changed()
 
-    def text_changed(self):
+    def text_changed(self) -> None:
         """QLineEdit validator"""
         value = self.item.from_string(self.__get_text())
         if not self.item.check_value(value):
             self.edit.setStyleSheet("background-color:rgb(255, 175, 90);")
         else:
             self.edit.setStyleSheet("")
         self.update(value)
         self.notify_value_change()
 
-    def update(self, value):
+    def update(self, value: Any) -> Any:
         """Override AbstractDataSetWidget method"""
         pass
 
-    def value(self):
+    def value(self) -> str:
+        """
+        Returns the widget's current value
+
+        :rtype str:
+        """
         return self.edit.toPlainText()
 
-    def check(self):
+    def check(self) -> Any:
         """Override AbstractDataSetWidget method"""
         value = self.item.from_string(self.__get_text())
         return self.item.check_value(value)
 
 
 class CheckBoxWidget(AbstractDataSetWidget):
     """
     BoolItem widget
     """
 
-    def __init__(self, item, parent_layout):
-        super(CheckBoxWidget, self).__init__(item, parent_layout)
+    def __init__(
+        self, item: "DataItemVariable", parent_layout: "DataSetEditLayout"
+    ) -> None:
+        super().__init__(item, parent_layout)
         self.checkbox = QCheckBox(self.item.get_prop_value("display", "text"))
         self.checkbox.setToolTip(item.get_help())
         self.group = self.checkbox
 
         self.store = self.item.get_prop("display", "store", None)
-        self.checkbox.stateChanged.connect(self.state_changed)
+        self.checkbox.stateChanged.connect(self.state_changed)  # type:ignore
 
-    def get(self):
+    def get(self) -> None:
         """Override AbstractDataSetWidget method"""
         value = self.item.get()
         if value is not None:
             self.checkbox.setChecked(value)
 
-    def set(self):
+    def set(self) -> None:
         """Override AbstractDataSetWidget method"""
         self.item.set(self.value())
 
-    def value(self):
+    def value(self) -> bool:
         return self.checkbox.isChecked()
 
     def place_on_grid(
-        self, layout, row, label_column, widget_column, row_span=1, column_span=1
-    ):
+        self,
+        layout: "QGridLayout",
+        row: int,
+        label_column: int,
+        widget_column: int,
+        row_span: int = 1,
+        column_span: int = 1,
+    ) -> None:
         """Override AbstractDataSetWidget method"""
         if not self.item.get_prop_value("display", "label"):
             widget_column = label_column
             column_span += 1
         else:
             self.place_label(layout, row, label_column)
         layout.addWidget(self.group, row, widget_column, row_span, column_span)
 
-    def state_changed(self, state):
+    def state_changed(self, state: bool) -> None:
         self.notify_value_change()
         if self.store:
             self.do_store(state)
 
-    def do_store(self, state):
+    def do_store(self, state: bool) -> None:
         self.store.set(self.item.instance, self.item.item, state)
         self.parent_layout.refresh_widgets()
 
 
 class DateWidget(AbstractDataSetWidget):
     """
     DateItem widget
     """
 
-    def __init__(self, item, parent_layout):
-        super(DateWidget, self).__init__(item, parent_layout)
+    def __init__(
+        self, item: "DataItemVariable", parent_layout: "DataSetEditLayout"
+    ) -> None:
+        super().__init__(item, parent_layout)
         self.dateedit = self.group = QDateEdit()
         self.dateedit.setToolTip(item.get_help())
-        self.dateedit.dateTimeChanged.connect(lambda value: self.notify_value_change())
+        self.dateedit.dateTimeChanged.connect(self.date_changed)
 
-    def get(self):
+    def date_changed(self, value):
+        """Date changed"""
+        _display_callback(self, value)
+        self.notify_value_change()
+
+    def get(self) -> None:
         """Override AbstractDataSetWidget method"""
         value = self.item.get()
         if value:
             if not isinstance(value, datetime.date):
                 value = datetime.date.fromordinal(value)
             self.dateedit.setDate(value)
 
-    def set(self):
+    def set(self) -> None:
         """Override AbstractDataSetWidget method"""
         self.item.set(self.value())
 
-    def value(self):
+    def value(self) -> datetime:  # type:ignore
+        """
+        Returns the widget's current value
+
+        :rtype date:
+        """
+        """
+        Returns the widget's current value
+
+        :rtype date:
+        """
         try:
             return self.dateedit.date().toPyDate()
         except AttributeError:
-            return self.dateedit.dateTime().toPython().date()  # PySide
+            return self.dateedit.dateTime().toPython().date()  # type:ignore # PySide
 
 
 class DateTimeWidget(AbstractDataSetWidget):
     """
     DateTimeItem widget
     """
 
-    def __init__(self, item, parent_layout):
-        super(DateTimeWidget, self).__init__(item, parent_layout)
+    def __init__(
+        self, item: "DataItemVariable", parent_layout: "DataSetEditLayout"
+    ) -> None:
+        super().__init__(item, parent_layout)
         self.dateedit = self.group = QDateTimeEdit()
         self.dateedit.setCalendarPopup(True)
         self.dateedit.setToolTip(item.get_help())
-        self.dateedit.dateTimeChanged.connect(lambda value: self.notify_value_change())
+        self.dateedit.dateTimeChanged.connect(  # type:ignore
+            lambda value: self.notify_value_change()
+        )
+
+    def date_changed(self, value):
+        """Date changed"""
+        _display_callback(self, value)
+        self.notify_value_change()
 
     def get(self):
         """Override AbstractDataSetWidget method"""
         value = self.item.get()
         if value:
             if not isinstance(value, datetime.datetime):
                 value = datetime.datetime.fromtimestamp(value)
             self.dateedit.setDateTime(value)
 
-    def set(self):
+    def set(self) -> None:
         """Override AbstractDataSetWidget method"""
         self.item.set(self.value())
 
-    def value(self):
+    def value(self) -> datetime:  # type:ignore
         try:
             return self.dateedit.dateTime().toPyDateTime()
         except AttributeError:
-            return self.dateedit.dateTime().toPython()  # PySide
+            return self.dateedit.dateTime().toPython()  # type:ignore # PySide
 
 
 class GroupLayout(QHBoxLayout):
-    def __init__(self):
+    def __init__(self) -> None:
         QHBoxLayout.__init__(self)
-        self.widgets = []
+        self.widgets: List["QWidget"] = []
 
-    def addWidget(self, widget):
+    def addWidget(self, widget: "QWidget") -> None:  # type:ignore
         QHBoxLayout.addWidget(self, widget)
         self.widgets.append(widget)
 
-    def setEnabled(self, state):
+    def setEnabled(self, state: bool) -> None:
         for widget in self.widgets:
             widget.setEnabled(state)
 
 
-class HLayoutMixin(object):
-    def __init__(self, item, parent_layout):
-        super(HLayoutMixin, self).__init__(item, parent_layout)
+class HasGroupProtocol(Protocol):
+    @property
+    def group(self):
+        pass
+
+    def place_label(self, layout: QGridLayout, row: int, column: int) -> None:
+        pass
+
+
+class HLayoutMixin:
+    def __init__(
+        self: "HasGroupProtocol",
+        item: "DataItemVariable",
+        parent_layout: "DataSetEditLayout",
+    ) -> None:
+        super().__init__(item, parent_layout)  # type:ignore
         old_group = self.group
         self.group = GroupLayout()
         self.group.addWidget(old_group)
 
     def place_on_grid(
-        self, layout, row, label_column, widget_column, row_span=1, column_span=1
+        self: "HasGroupProtocol",
+        layout: "QGridLayout",
+        row: int,
+        label_column: int,
+        widget_column: int,
+        row_span: int = 1,
+        column_span: int = 1,
     ):
         """Override AbstractDataSetWidget method"""
         self.place_label(layout, row, label_column)
         layout.addLayout(self.group, row, widget_column, row_span, column_span)
 
 
 class ColorWidget(HLayoutMixin, LineEditWidget):
     """
     ColorItem widget
     """
 
-    def __init__(self, item, parent_layout):
-        super(ColorWidget, self).__init__(item, parent_layout)
+    def __init__(
+        self, item: "DataItemVariable", parent_layout: "DataSetEditLayout"
+    ) -> None:
+        super().__init__(item, parent_layout)
         self.button = QPushButton("")
         self.button.setMaximumWidth(32)
-        self.button.clicked.connect(self.select_color)
+        self.button.clicked.connect(self.select_color)  # type:ignore
         self.group.addWidget(self.button)
 
-    def update(self, value):
+    def update(self, value: str) -> None:
         """Reimplement LineEditWidget method"""
         LineEditWidget.update(self, value)
         color = text_to_qcolor(value)
         if color.isValid():
             bitmap = QPixmap(16, 16)
             bitmap.fill(color)
             icon = QIcon(bitmap)
         else:
             icon = get_icon("not_found")
         self.button.setIcon(icon)
 
-    def select_color(self):
+    def select_color(self) -> None:
         """Open a color selection dialog box"""
         color = text_to_qcolor(self.edit.text())
         if not color.isValid():
-            color = Qt.gray
+            color = Qt.gray  # type:ignore
         color = QColorDialog.getColor(color, self.parent_layout.parent)
         if color.isValid():
             value = color.name()
             self.edit.setText(value)
             self.update(value)
             self.notify_value_change()
 
 
 class SliderWidget(HLayoutMixin, LineEditWidget):
     """
     IntItem with Slider
     """
 
-    DATA_TYPE = int
+    DATA_TYPE: type = int
 
-    def __init__(self, item, parent_layout):
-        super(SliderWidget, self).__init__(item, parent_layout)
+    def __init__(
+        self, item: DataItemVariable, parent_layout: "DataSetEditLayout"
+    ) -> None:
+        super().__init__(item, parent_layout)
         self.slider = self.vmin = self.vmax = None
         if item.get_prop_value("display", "slider"):
             self.vmin = item.get_prop_value("data", "min")
             self.vmax = item.get_prop_value("data", "max")
             assert (
                 self.vmin is not None and self.vmax is not None
             ), "SliderWidget requires that item min/max have been defined"
             self.slider = QSlider()
-            self.slider.setOrientation(Qt.Horizontal)
+            self.slider.setOrientation(Qt.Horizontal)  # type:ignore
             self.setup_slider(item)
-            self.slider.valueChanged.connect(self.value_changed)
+            self.slider.valueChanged.connect(self.value_changed)  # type:ignore
             self.group.addWidget(self.slider)
 
     def value_to_slider(self, value):
         return value
 
     def slider_to_value(self, value):
         return value
@@ -584,15 +676,15 @@
 
 
 class FloatSliderWidget(SliderWidget):
     """
     FloatItem with Slider
     """
 
-    DATA_TYPE = float
+    DATA_TYPE: type = float
 
     def value_to_slider(self, value):
         return int((value - self.vmin) * 100 / (self.vmax - self.vmin))
 
     def slider_to_value(self, value):
         return value * (self.vmax - self.vmin) / 100 + self.vmin
 
@@ -614,46 +706,52 @@
 
 
 class FileWidget(HLayoutMixin, LineEditWidget):
     """
     File path item widget
     """
 
-    def __init__(self, item, parent_layout, filedialog):
-        super(FileWidget, self).__init__(item, parent_layout)
+    def __init__(
+        self,
+        item: "DataItemVariable",
+        parent_layout: "DataSetEditLayout",
+        filedialog: Callable,
+    ) -> None:
+        super().__init__(item, parent_layout)
         self.filedialog = filedialog
         button = QPushButton()
         fmt = item.get_prop_value("data", "formats")
         button.setIcon(get_icon("%s.png" % fmt[0].lower(), default="file.png"))
-        button.clicked.connect(self.select_file)
+        button.clicked.connect(self.select_file)  # type:ignore
         self.group.addWidget(button)
         self.basedir = item.get_prop_value("data", "basedir")
         self.all_files_first = item.get_prop_value("data", "all_files_first")
 
-    def select_file(self):
+    def select_file(self) -> None:
         """Open a file selection dialog box"""
         fname = self.item.from_string(str(self.edit.text()))
         if isinstance(fname, list):
             fname = osp.dirname(fname[0])
         parent = self.parent_layout.parent
         _temp = sys.stdout
-        sys.stdout = None
+        sys.stdout = None  # type:ignore
         if len(fname) == 0:
             fname = self.basedir
         _formats = self.item.get_prop_value("data", "formats")
         formats = [str(format).lower() for format in _formats]
         filter_lines = [
             (_("%s files") + " (*.%s)") % (format.upper(), format) for format in formats
         ]
         all_filter = _("All supported files") + " (*.%s)" % " *.".join(formats)
         if len(formats) > 1:
             if self.all_files_first:
                 filter_lines.insert(0, all_filter)
             else:
                 filter_lines.append(all_filter)
+
         if fname is None:
             fname = ""
         child_title = _get_child_title_func(parent)
         fname, _filter = self.filedialog(
             parent, child_title(self.item), fname, "\n".join(filter_lines)
         )
         sys.stdout = _temp
@@ -664,70 +762,67 @@
 
 
 class DirectoryWidget(HLayoutMixin, LineEditWidget):
     """
     Directory path item widget
     """
 
-    def __init__(self, item, parent_layout):
-        super(DirectoryWidget, self).__init__(item, parent_layout)
+    def __init__(
+        self, item: "DataItemVariable", parent_layout: "DataSetEditLayout"
+    ) -> None:
+        super().__init__(item, parent_layout)
         button = QPushButton()
         button.setIcon(get_std_icon("DirOpenIcon"))
-        button.clicked.connect(self.select_directory)
+        button.clicked.connect(self.select_directory)  # type:ignore
         self.group.addWidget(button)
 
-    def select_directory(self):
+    def select_directory(self) -> None:
         """Open a directory selection dialog box"""
         value = self.item.from_string(str(self.edit.text()))
         parent = self.parent_layout.parent
         child_title = _get_child_title_func(parent)
         dname = getexistingdirectory(parent, child_title(self.item), value)
         if dname:
             self.edit.setText(dname)
 
 
 class ChoiceWidget(AbstractDataSetWidget):
     """
     Choice item widget
     """
 
-    def __init__(self, item, parent_layout):
-        super(ChoiceWidget, self).__init__(item, parent_layout)
+    def __init__(
+        self, item: "DataItemVariable", parent_layout: "DataSetEditLayout"
+    ) -> None:
+        super().__init__(item, parent_layout)
         self._first_call = True
         self.is_radio = item.get_prop_value("display", "radio")
         self.store = self.item.get_prop("display", "store", None)
         if self.is_radio:
             self.group = QGroupBox()
             self.group.setToolTip(item.get_help())
             self.vbox = QVBoxLayout()
             self.group.setLayout(self.vbox)
-            self._buttons = []
+            self._buttons: List["QAbstractButton"] = []
         else:
             self.combobox = self.group = QComboBox()
             self.combobox.setToolTip(item.get_help())
-            self.combobox.currentIndexChanged.connect(self.index_changed)
+            self.combobox.currentIndexChanged.connect(self.index_changed)  # type:ignore
 
-    def index_changed(self, index):
+    def index_changed(self, index: int) -> None:
         if self.store:
             self.store.set(self.item.instance, self.item.item, self.value())
             self.parent_layout.refresh_widgets()
-        cb = self.item.get_prop_value("display", "callback", None)
-        if cb is not None:
-            if self.build_mode:
-                self.set()
-            else:
-                self.parent_layout.update_dataitems()
-            cb(self.item.instance, self.item.item, self.value())
-            self.parent_layout.update_widgets(except_this_one=self)
+        _display_callback(self, self.value())
         self.notify_value_change()
 
-    def initialize_widget(self):
+    def initialize_widget(self) -> None:
         if self.is_radio:
             for button in self._buttons:
-                button.toggled.disconnect(self.index_changed)
+                button.toggled.disconnect(self.index_changed)  # type:ignore
                 self.vbox.removeWidget(button)
                 button.deleteLater()
             self._buttons = []
         else:
             self.combobox.blockSignals(True)
             while self.combobox.count():
                 self.combobox.removeItem(0)
@@ -736,50 +831,51 @@
             if self.is_radio:
                 button = QRadioButton(lbl, self.group)
             if img:
                 if isinstance(img, str):
                     if not osp.isfile(img):
                         img = get_image_file_path(img)
                     img = QIcon(img)
-                elif isinstance(img, collections.abc.Callable):
+                elif isinstance(img, collections.abc.Callable):  # type:ignore
                     img = img(key)
                 if self.is_radio:
                     button.setIcon(img)
                 else:
                     self.combobox.addItem(img, lbl)
             elif not self.is_radio:
                 self.combobox.addItem(lbl)
             if self.is_radio:
                 self._buttons.append(button)
                 self.vbox.addWidget(button)
-                button.toggled.connect(self.index_changed)
+                button.toggled.connect(self.index_changed)  # type:ignore
         if not self.is_radio:
             self.combobox.blockSignals(False)
 
-    def set_widget_value(self, idx):
+    def set_widget_value(self, idx: int) -> None:
         if self.is_radio:
             for button in self._buttons:
                 button.blockSignals(True)
             self._buttons[idx].setChecked(True)
             for button in self._buttons:
                 button.blockSignals(False)
         else:
             self.combobox.blockSignals(True)
             self.combobox.setCurrentIndex(idx)
             self.combobox.blockSignals(False)
 
-    def get_widget_value(self):
+    def get_widget_value(self) -> Optional[int]:
         if self.is_radio:
             for index, widget in enumerate(self._buttons):
                 if widget.isChecked():
                     return index
+            return None  # TODO:Faire comme ca ?
         else:
             return self.combobox.currentIndex()
 
-    def get(self):
+    def get(self) -> None:
         """Override AbstractDataSetWidget method"""
         self.initialize_widget()
         value = self.item.get()
         if value is not None:
             idx = 0
             _choices = self.item.get_prop_value("data", "choices")
             for key, _val, _img in _choices:
@@ -787,35 +883,37 @@
                     break
                 idx += 1
             self.set_widget_value(idx)
             if self._first_call:
                 self.index_changed(idx)
                 self._first_call = False
 
-    def set(self):
+    def set(self) -> None:
         """Override AbstractDataSetWidget method"""
         try:
             value = self.value()
         except IndexError:
             return
         self.item.set(value)
 
-    def value(self):
+    def value(self) -> Any:
         index = self.get_widget_value()
         choices = self.item.get_prop_value("data", "choices")
         return choices[index][0]
 
 
 class MultipleChoiceWidget(AbstractDataSetWidget):
     """
     Multiple choice item widget
     """
 
-    def __init__(self, item, parent_layout):
-        super(MultipleChoiceWidget, self).__init__(item, parent_layout)
+    def __init__(
+        self, item: "DataItemVariable", parent_layout: "DataSetEditLayout"
+    ) -> None:
+        super().__init__(item, parent_layout)
         self.groupbox = self.group = QGroupBox(item.get_prop_value("display", "label"))
         layout = QGridLayout()
         self.boxes = []
         nx, ny = item.get_prop_value("display", "shape")
         cx, cy = 0, 0
         _choices = item.get_prop_value("data", "choices")
         for _, choice, _img in _choices:
@@ -830,49 +928,57 @@
                 cx += 1
                 if cx >= nx:
                     cx = 0
                     cy += 1
             self.boxes.append(checkbox)
         self.groupbox.setLayout(layout)
 
-    def get(self):
+    def get(self) -> None:
         """Override AbstractDataSetWidget method"""
         value = self.item.get()
         _choices = self.item.get_prop_value("data", "choices")
         for (i, _choice, _img), checkbox in zip(_choices, self.boxes):
             if value is not None and i in value:
                 checkbox.setChecked(True)
 
-    def set(self):
+    def set(self) -> None:
         """Override AbstractDataSetWidget method"""
         _choices = self.item.get_prop_value("data", "choices")
         choices = [_choices[i][0] for i in self.value()]
         self.item.set(choices)
 
-    def value(self):
+    def value(self) -> List[int]:
         return [i for i, w in enumerate(self.boxes) if w.isChecked()]
 
     def place_on_grid(
-        self, layout, row, label_column, widget_column, row_span=1, column_span=1
-    ):
+        self,
+        layout: "QGridLayout",
+        row: int,
+        label_column: int,
+        widget_column: int,
+        row_span: int = 1,
+        column_span: int = 1,
+    ) -> None:
         """Override AbstractDataSetWidget method"""
         layout.addWidget(self.group, row, label_column, row_span, column_span + 1)
 
 
 class FloatArrayWidget(AbstractDataSetWidget):
     """
     FloatArrayItem widget
     """
 
-    def __init__(self, item, parent_layout):
-        super(FloatArrayWidget, self).__init__(item, parent_layout)
+    def __init__(
+        self, item: "DataItemVariable", parent_layout: "DataSetEditLayout"
+    ) -> None:
+        super().__init__(item, parent_layout)
         _label = item.get_prop_value("display", "label")
         self.groupbox = self.group = QGroupBox(_label)
         self.layout = QGridLayout()
-        self.layout.setAlignment(Qt.AlignLeft)
+        self.layout.setAlignment(Qt.AlignLeft)  # type:ignore
         self.groupbox.setLayout(self.layout)
 
         self.first_line, self.dim_label = get_image_layout(
             "shape.png", _("Number of rows x Number of columns")
         )
         edit_button = QPushButton(get_icon("arredit.png"), "")
         edit_button.setToolTip(_("Edit array contents"))
@@ -885,39 +991,39 @@
         )
         self.layout.addLayout(self.min_line, 1, 0)
         self.max_line, self.max_label = get_image_layout(
             "max.png", _("Largest element in array")
         )
         self.layout.addLayout(self.max_line, 2, 0)
 
-        edit_button.clicked.connect(self.edit_array)
-        self.arr = None  # le tableau si il a été modifié
+        edit_button.clicked.connect(self.edit_array)  # type:ignore
+        self.arr = numpy.array([])  # le tableau si il a été modifié
         self.instance = None
 
         self.dtype_line, self.dtype_label = get_image_layout("dtype.png", "")
         self.first_line.insertSpacing(2, 5)
         self.first_line.insertLayout(3, self.dtype_line)
 
-    def edit_array(self):
+    def edit_array(self) -> None:
         """Open an array editor dialog"""
         parent = self.parent_layout.parent
         label = self.item.get_prop_value("display", "label")
         editor = ArrayEditor(parent)
         if editor.setup_and_check(self.arr, title=label):
-            if editor.exec_():
+            if editor.exec():
                 self.update(self.arr)
 
-    def get(self):
+    def get(self) -> None:
         """Override AbstractDataSetWidget method"""
         self.arr = numpy.array(self.item.get(), copy=False)
         if self.item.get_prop_value("display", "transpose"):
             self.arr = self.arr.T
         self.update(self.arr)
 
-    def update(self, arr):
+    def update(self, arr: numpy.ndarray) -> None:
         """Override AbstractDataSetWidget method"""
         shape = arr.shape
         if len(shape) == 1:
             shape = (1,) + shape
         dim = " x ".join([str(d) for d in shape])
         self.dim_label.setText(dim)
 
@@ -945,128 +1051,155 @@
         except (TypeError, IndexError):
             mint, maxt = "-", "-"
         self.min_label.setText(mint)
         self.max_label.setText(maxt)
         typestr = str(arr.dtype)
         self.dtype_label.setText("-" if typestr == "object" else typestr)
 
-    def set(self):
+    def set(self) -> None:
         """Override AbstractDataSetWidget method"""
         if self.item.get_prop_value("display", "transpose"):
             value = self.value().T
         else:
             value = self.value()
         self.item.set(value)
 
-    def value(self):
+    def value(self) -> numpy.ndarray:
         return self.arr
 
     def place_on_grid(
-        self, layout, row, label_column, widget_column, row_span=1, column_span=1
-    ):
+        self,
+        layout: "QGridLayout",
+        row: int,
+        label_column: int,
+        widget_column: int,
+        row_span: int = 1,
+        column_span: int = 1,
+    ) -> None:
         """Override AbstractDataSetWidget method"""
         layout.addWidget(self.group, row, label_column, row_span, column_span + 1)
 
 
 class ButtonWidget(AbstractDataSetWidget):
     """
     BoolItem widget
     """
 
-    def __init__(self, item, parent_layout):
-        super(ButtonWidget, self).__init__(item, parent_layout)
+    def __init__(
+        self, item: "DataItemVariable", parent_layout: "DataSetEditLayout"
+    ) -> None:
+        super().__init__(item, parent_layout)
         _label = self.item.get_prop_value("display", "label")
         self.button = self.group = QPushButton(_label)
         self.button.setToolTip(item.get_help())
         _icon = self.item.get_prop_value("display", "icon")
         if _icon is not None:
             if isinstance(_icon, str):
                 _icon = get_icon(_icon)
             self.button.setIcon(_icon)
-        self.button.clicked.connect(self.clicked)
+        self.button.clicked.connect(self.clicked)  # type:ignore
         self.cb_value = None
 
-    def get(self):
+    def get(self) -> None:
         """Override AbstractDataSetWidget method"""
         self.cb_value = self.item.get()
 
-    def set(self):
+    def set(self) -> None:
         """Override AbstractDataSetWidget method"""
         self.item.set(self.value())
 
-    def value(self):
+    def value(self) -> Optional[Any]:
         return self.cb_value
 
     def place_on_grid(
-        self, layout, row, label_column, widget_column, row_span=1, column_span=1
+        self,
+        layout: "QGridLayout",
+        row: int,
+        label_column: int,
+        widget_column: int,
+        row_span: int = 1,
+        column_span: int = 1,
     ):
         """Override AbstractDataSetWidget method"""
         layout.addWidget(self.group, row, label_column, row_span, column_span + 1)
 
-    def clicked(self, *args):
+    def clicked(self, *args) -> None:
         self.parent_layout.update_dataitems()
         callback = self.item.get_prop_value("display", "callback")
         self.cb_value = callback(
             self.item.instance, self.item.item, self.cb_value, self.button.parent()
         )
         self.set()
         self.parent_layout.update_widgets()
 
 
 class DataSetWidget(AbstractDataSetWidget):
     """
     DataSet widget
     """
 
-    def __init__(self, item, parent_layout):
-        super(DataSetWidget, self).__init__(item, parent_layout)
+    @property
+    @abstractmethod
+    def klass(self) -> type:
+        pass
+
+    def __init__(
+        self, item: "DataItemVariable", parent_layout: "DataSetEditLayout"
+    ) -> None:
+        super().__init__(item, parent_layout)
         self.dataset = self.klass()
         # Création du layout contenant les champs d'édition du signal
         embedded = item.get_prop_value("display", "embedded", False)
         if not embedded:
             self.group = QGroupBox(item.get_prop_value("display", "label"))
         else:
             self.group = QFrame()
         self.layout = QGridLayout()
         self.group.setLayout(self.layout)
         EditLayoutClass = parent_layout.__class__
         self.edit = EditLayoutClass(
             self.parent_layout.parent, self.dataset, self.layout
         )
 
-    def get(self):
+    def get(self) -> None:
         """Override AbstractDataSetWidget method"""
         self.get_dataset()
         for widget in self.edit.widgets:
             widget.get()
 
-    def set(self):
+    def set(self) -> None:
         """Override AbstractDataSetWidget method"""
         for widget in self.edit.widgets:
             widget.set()
         self.set_dataset()
 
-    def get_dataset(self):
+    def get_dataset(self) -> None:
         """update's internal parameter representation
         from the item's stored value
 
         default behavior uses update_dataset and assumes
         internal dataset class is the same as item's value
         class"""
         item = self.item.get()
         update_dataset(self.dataset, item)
 
-    def set_dataset(self):
+    def set_dataset(self) -> None:
         """update the item's value from the internal
         data representation
 
         default behavior uses restore_dataset and assumes
         internal dataset class is the same as item's value
         class"""
         item = self.item.get()
         restore_dataset(self.dataset, item)
 
     def place_on_grid(
-        self, layout, row, label_column, widget_column, row_span=1, column_span=1
-    ):
+        self,
+        layout: "QGridLayout",
+        row: int,
+        label_column: int,
+        widget_column: int,
+        row_span: int = 1,
+        column_span: int = 1,
+    ) -> None:
         """Override AbstractDataSetWidget method"""
         layout.addWidget(self.group, row, label_column, row_span, column_span + 1)
```

### Comparing `guidata-2.3.1/guidata/dataset/qtwidgets.py` & `guidata-3.0.0/guidata/dataset/qtwidgets.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,135 +1,173 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright © 2009-2010 CEA
-# Pierre Raybaut
-# Licensed under the terms of the CECILL License
-# (see guidata/__init__.py for details)
+# Licensed under the terms of the BSD 3-Clause
+# (see guidata/LICENSE for details)
 
 """
-dataset.qtwidgets
-=================
+Qt widgets for data sets
+------------------------
 
-Dialog boxes used to edit data sets:
-    DataSetEditDialog
-    DataSetGroupEditDialog
-    DataSetShowDialog
-
-...and layouts:
-    GroupItem
-    DataSetEditLayout
-    DataSetShowLayout
+Dialog boxes for DataSet editing and showing
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. autoclass:: DataSetEditDialog
+    :show-inheritance:
+    :members:
+
+.. autoclass:: DataSetShowDialog
+    :show-inheritance:
+    :members:
+
+.. autoclass:: DataSetGroupEditDialog
+    :show-inheritance:
+    :members:
+
+Layouts for DataSet editing and showing
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. autoclass:: DataSetEditLayout
+    :show-inheritance:
+    :members:
+
+.. autoclass:: DataSetShowLayout
+    :show-inheritance:
+    :members:
 """
 
+from typing import *
+
+from qtpy.compat import getopenfilename, getopenfilenames, getsavefilename
+from qtpy.QtCore import QRect, QSize, Qt, Signal
+from qtpy.QtGui import QBrush, QColor, QIcon, QPainter, QPicture
 from qtpy.QtWidgets import (
+    QAbstractButton,
+    QApplication,
     QDialog,
-    QMessageBox,
     QDialogButtonBox,
-    QWidget,
-    QVBoxLayout,
     QGridLayout,
+    QGroupBox,
     QLabel,
+    QMessageBox,
+    QPushButton,
     QSpacerItem,
     QTabWidget,
-    QApplication,
-    QGroupBox,
-    QPushButton,
+    QVBoxLayout,
+    QWidget,
 )
-from qtpy.QtGui import QColor, QIcon, QPainter, QPicture, QBrush
-from qtpy.QtCore import Qt, QRect, QSize, Signal
-from qtpy.compat import getopenfilename, getopenfilenames, getsavefilename
 
-from guidata.configtools import get_icon
 from guidata.config import _
-
-from guidata.dataset.datatypes import BeginGroup, EndGroup, GroupItem, TabGroupItem
+from guidata.configtools import get_icon
+from guidata.dataset.datatypes import (
+    BeginGroup,
+    DataItem,
+    DataItemVariable,
+    DataSet,
+    EndGroup,
+    GroupItem,
+    TabGroupItem,
+)
 from guidata.qthelpers import win32_fix_title_bar_background
 
+if TYPE_CHECKING:  # pragma: no cover
+    from guidata.dataset.datatypes import DataSetGroup
+
 
 class DataSetEditDialog(QDialog):
     """
     Dialog box for DataSet editing
     """
 
     def __init__(
-        self, instance, icon="", parent=None, apply=None, wordwrap=True, size=None
-    ):
+        self,
+        instance: Union["DataSet", "DataSetGroup"],
+        icon: Union[str, QIcon] = "",
+        parent: Optional[QWidget] = None,
+        apply: Optional[Callable] = None,
+        wordwrap: bool = True,
+        size: Optional[Union[QSize, Tuple[int, int]]] = None,
+    ) -> None:
         QDialog.__init__(self, parent)
         win32_fix_title_bar_background(self)
         self.wordwrap = wordwrap
         self.apply_func = apply
-        self.layout = QVBoxLayout()
+        self._layout = QVBoxLayout()
         if instance.get_comment():
             label = QLabel(instance.get_comment())
             label.setWordWrap(wordwrap)
-            self.layout.addWidget(label)
+            self._layout.addWidget(label)
         self.instance = instance
-        self.edit_layout = []
+        self.edit_layout: List["DataSetEditLayout"] = []
 
         self.setup_instance(instance)
 
         if apply is not None:
-            apply_button = QDialogButtonBox.Apply
+            apply_button = QDialogButtonBox.Apply  # type:ignore
         else:
-            apply_button = QDialogButtonBox.NoButton
+            apply_button = QDialogButtonBox.NoButton  # type:ignore
         bbox = QDialogButtonBox(
-            QDialogButtonBox.Ok | QDialogButtonBox.Cancel | apply_button
+            QDialogButtonBox.Ok | QDialogButtonBox.Cancel | apply_button  # type:ignore
         )
         self.bbox = bbox
-        bbox.accepted.connect(self.accept)
-        bbox.rejected.connect(self.reject)
-        bbox.clicked.connect(self.button_clicked)
-        self.layout.addWidget(bbox)
+        bbox.accepted.connect(self.accept)  # type:ignore
+        bbox.rejected.connect(self.reject)  # type:ignore
+        bbox.clicked.connect(self.button_clicked)  # type:ignore
+        self._layout.addWidget(bbox)
 
-        self.setLayout(self.layout)
+        self.setLayout(self._layout)
 
         if parent is None:
             if not isinstance(icon, QIcon):
                 icon = get_icon(icon, default="guidata.svg")
-            self.setWindowIcon(icon)
+            self.setWindowIcon(icon)  # type:ignore
 
         self.setModal(True)
         self.setWindowTitle(instance.get_title())
 
         if size is not None:
             if isinstance(size, QSize):
                 self.resize(size)
             else:
                 self.resize(*size)
 
-    def button_clicked(self, button):
+    def button_clicked(self, button: "QAbstractButton") -> None:
         role = self.bbox.buttonRole(button)
-        if role == QDialogButtonBox.ApplyRole and self.apply_func is not None:
+        if (
+            role == QDialogButtonBox.ApplyRole  # type:ignore
+            and self.apply_func is not None
+        ):
             if self.check():
                 for edl in self.edit_layout:
                     edl.accept_changes()
                 self.apply_func(self.instance)
 
-    def setup_instance(self, instance):
+    def setup_instance(self, instance: Any) -> None:
         """Construct main layout"""
         grid = QGridLayout()
-        grid.setAlignment(Qt.AlignTop)
-        self.layout.addLayout(grid)
+        grid.setAlignment(Qt.AlignTop)  # type:ignore
+        self._layout.addLayout(grid)
         self.edit_layout.append(self.layout_factory(instance, grid))
 
-    def layout_factory(self, instance, grid):
+    def layout_factory(
+        self, instance: "DataSet", grid: "QGridLayout"
+    ) -> "DataSetEditLayout":
         """A factory method that produces instances of DataSetEditLayout
 
         or derived classes (see DataSetShowDialog)
         """
         return DataSetEditLayout(self, instance, grid)
 
-    def child_title(self, item):
+    def child_title(self, item: "DataItemVariable") -> str:
         """Return data item title combined with QApplication title"""
         app_name = QApplication.applicationName()
         if not app_name:
             app_name = self.instance.get_title()
         return "%s - %s" % (app_name, item.label())
 
-    def check(self):
+    def check(self) -> bool:
         is_ok = True
         for edl in self.edit_layout:
             if not edl.check_all_values():
                 is_ok = False
         if not is_ok:
             QMessageBox.warning(
                 self,
@@ -137,38 +175,39 @@
                 _("Some required entries are incorrect")
                 + "\n"
                 + _("Please check highlighted fields."),
             )
             return False
         return True
 
-    def accept(self):
+    def accept(self) -> None:
         """Validate inputs"""
         if self.check():
             for edl in self.edit_layout:
                 edl.accept_changes()
             QDialog.accept(self)
 
 
 class DataSetGroupEditDialog(DataSetEditDialog):
     """
     Tabbed dialog box for DataSet editing
     """
 
-    def setup_instance(self, instance):
+    def setup_instance(self, instance: "DataSetGroup") -> None:
         """Override DataSetEditDialog method"""
         from guidata.dataset.datatypes import DataSetGroup
 
         assert isinstance(instance, DataSetGroup)
         tabs = QTabWidget()
         #        tabs.setUsesScrollButtons(False)
-        self.layout.addWidget(tabs)
+        self._layout.addWidget(tabs)
         for dataset in instance.datasets:
             layout = QVBoxLayout()
-            layout.setAlignment(Qt.AlignTop)
+
+            layout.setAlignment(Qt.AlignmentFlag.AlignTop)
             if dataset.get_comment():
                 label = QLabel(dataset.get_comment())
                 label.setWordWrap(self.wordwrap)
                 layout.addWidget(label)
             grid = QGridLayout()
             self.edit_layout.append(self.layout_factory(dataset, grid))
             layout.addLayout(grid)
@@ -176,72 +215,78 @@
             page.setLayout(layout)
             if dataset.get_icon():
                 tabs.addTab(page, get_icon(dataset.get_icon()), dataset.get_title())
             else:
                 tabs.addTab(page, dataset.get_title())
 
 
-class DataSetEditLayout(object):
+class DataSetEditLayout:
     """
     Layout in which data item widgets are placed
     """
 
-    _widget_factory = {}
+    _widget_factory: Dict[Any, Any] = {}
 
     @classmethod
-    def register(cls, item_type, factory):
+    def register(cls: Type, item_type: Type, factory: Any) -> None:
         """Register a factory for a new item_type"""
         cls._widget_factory[item_type] = factory
 
     def __init__(
-        self, parent, instance, layout, items=None, first_line=0, change_callback=None
-    ):
+        self,
+        parent: Optional[QWidget],
+        instance: "DataSet",
+        layout: QGridLayout,
+        items: Optional[List["DataItem"]] = None,
+        first_line: int = 0,
+        change_callback: Optional[Callable] = None,
+    ) -> None:
         self.parent = parent
         self.instance = instance
         self.layout = layout
         self.first_line = first_line
         self.change_callback = change_callback
-        self.widgets = []
-        self.linenos = {}  # prochaine ligne à remplir par colonne
-        self.items_pos = {}
+        self.widgets: List["AbstractDataSetWidget"] = []
+        # self.linenos = {}  # prochaine ligne à remplir par colonne
+        self.items_pos: Dict["DataItem", List[int]] = {}
         if not items:
             items = self.instance._items
-        items = self.transform_items(items)
+        items = self.transform_items(items)  # type:ignore
         self.setup_layout(items)
 
-    def transform_items(self, items):
+    def transform_items(self, items: List["DataItem"]) -> List["DataItem"]:
         """
         Handle group of items: transform items into a GroupItem instance
         if they are located between BeginGroup and EndGroup
         """
-        item_lists = [[]]
+        item_lists: Any = [[]]
         for item in items:
             if isinstance(item, BeginGroup):
-                item = item.get_group()
-                item_lists[-1].append(item)
-                item_lists.append(item.group)
+                group_item = item.get_group()
+                item_lists[-1].append(group_item)
+                item_lists.append(group_item.group)
             elif isinstance(item, EndGroup):
                 item_lists.pop()
             else:
                 item_lists[-1].append(item)
         assert len(item_lists) == 1
         return item_lists[-1]
 
-    def check_all_values(self):
+    def check_all_values(self) -> bool:
         """Check input of all widgets"""
         for widget in self.widgets:
             if widget.is_active() and not widget.check():
                 return False
         return True
 
-    def accept_changes(self):
+    def accept_changes(self) -> None:
         """Accept changes made to widget inputs"""
         self.update_dataitems()
 
-    def setup_layout(self, items):
+    def setup_layout(self, items: List["DataItem"]) -> None:
         """Place items on layout"""
 
         def last_col(col, span):
             """Return last column (which depends on column span)"""
             if not span:
                 return col
             else:
@@ -253,15 +298,15 @@
                     item.get_prop("display", "col"), item.get_prop("display", "colspan")
                 )
                 for item in items
             ]
         )
 
         # Check if specified rows are consistent
-        sorted_items = [None] * len(items)
+        sorted_items: List[Optional[DataItem]] = [None] * len(items)
         rows = []
         other_items = []
         for item in items:
             row = item.get_prop("display", "row")
             if row is not None:
                 if row in rows:
                     raise ValueError(
@@ -271,22 +316,22 @@
                     raise ValueError(
                         "Out of range row index (%d) for item %r" % (row, item._name)
                     )
                 rows.append(row)
                 sorted_items[row] = item
             else:
                 other_items.append(item)
-        for idx, line in enumerate(sorted_items[:]):
-            if line is None:
+        for idx, item in enumerate(sorted_items[:]):  # type:ignore
+            if item is None:
                 sorted_items[idx] = other_items.pop(0)
 
         self.items_pos = {}
         line = self.first_line - 1
         last_item = [-1, 0, colmax]
-        for item in sorted_items:
+        for item in sorted_items:  # type:ignore
             col = item.get_prop("display", "col")
             colspan = item.get_prop("display", "colspan")
             if colspan is None:
                 colspan = colmax - col + 1
             if col <= last_item[1]:
                 # on passe à la ligne si la colonne de debut de cet item
                 #  est avant la colonne de debut de l'item précédent
@@ -301,96 +346,101 @@
             if hide:
                 continue
             widget = self.build_widget(item)
             self.add_row(widget)
 
         self.refresh_widgets()
 
-    def build_widget(self, item):
+    def build_widget(self, item: "DataItem") -> "DataSetShowWidget":
         factory = self._widget_factory[type(item)]
         widget = factory(item.bind(self.instance), self)
         self.widgets.append(widget)
         return widget
 
-    def add_row(self, widget):
+    def add_row(self, widget: "DataSetShowWidget") -> None:
         """Add widget to row"""
         item = widget.item
         line, col, span = self.items_pos[item.item]
         if col > 0:
             self.layout.addItem(QSpacerItem(20, 1), line, col * 3 - 1)
 
         widget.place_on_grid(self.layout, line, col * 3, col * 3 + 1, 1, 3 * span - 2)
         try:
             widget.get()
         except Exception:
             print("Error building item :", item.item._name)
             raise
 
-    def refresh_widgets(self):
+    def refresh_widgets(self) -> None:
         """Refresh the status of all widgets"""
         for widget in self.widgets:
             widget.set_state()
 
-    def update_dataitems(self):
+    def update_dataitems(self) -> None:
         """Refresh the content of all data items"""
         for widget in self.widgets:
             if widget.is_active():
                 widget.set()
 
-    def update_widgets(self, except_this_one=None):
+    def update_widgets(
+        self, except_this_one: Optional[Union[QWidget, "AbstractDataSetWidget"]] = None
+    ) -> None:
         """Refresh the content of all widgets"""
         for widget in self.widgets:
             if widget is not except_this_one:
                 widget.get()
 
-    def widget_value_changed(self):
+    def widget_value_changed(self) -> None:
         """Method called when any widget's value has changed"""
         if self.change_callback is not None:
             self.change_callback()
 
 
+from typing import Any
+
+from guidata.dataset.dataitems import (
+    BoolItem,
+    ButtonItem,
+    ChoiceItem,
+    ColorItem,
+    DateItem,
+    DateTimeItem,
+    DictItem,
+    DirectoryItem,
+    FileOpenItem,
+    FileSaveItem,
+    FilesOpenItem,
+    FloatArrayItem,
+    FloatItem,
+    ImageChoiceItem,
+    IntItem,
+    MultipleChoiceItem,
+    StringItem,
+    TextItem,
+)
+
 # Enregistrement des correspondances avec les widgets
 from guidata.dataset.qtitemwidgets import (
-    LineEditWidget,
-    TextEditWidget,
+    AbstractDataSetWidget,
+    ButtonWidget,
     CheckBoxWidget,
+    ChoiceWidget,
     ColorWidget,
-    FileWidget,
+    DateTimeWidget,
+    DateWidget,
     DirectoryWidget,
-    ChoiceWidget,
-    MultipleChoiceWidget,
+    FileWidget,
     FloatArrayWidget,
+    FloatSliderWidget,
     GroupWidget,
-    AbstractDataSetWidget,
-    ButtonWidget,
-    TabGroupWidget,
-    DateWidget,
-    DateTimeWidget,
+    LineEditWidget,
+    MultipleChoiceWidget,
     SliderWidget,
-    FloatSliderWidget,
-)
-from guidata.dataset.dataitems import (
-    FloatItem,
-    StringItem,
-    TextItem,
-    IntItem,
-    BoolItem,
-    ColorItem,
-    FileOpenItem,
-    FilesOpenItem,
-    FileSaveItem,
-    DirectoryItem,
-    ChoiceItem,
-    ImageChoiceItem,
-    MultipleChoiceItem,
-    FloatArrayItem,
-    ButtonItem,
-    DateItem,
-    DateTimeItem,
-    DictItem,
+    TabGroupWidget,
+    TextEditWidget,
 )
 
 DataSetEditLayout.register(GroupItem, GroupWidget)
 DataSetEditLayout.register(TabGroupItem, TabGroupWidget)
 DataSetEditLayout.register(FloatItem, LineEditWidget)
 DataSetEditLayout.register(StringItem, LineEditWidget)
 DataSetEditLayout.register(TextItem, TextEditWidget)
@@ -425,43 +475,47 @@
 
 
 class DataSetShowWidget(AbstractDataSetWidget):
     """Read-only base widget"""
 
     READ_ONLY = True
 
-    def __init__(self, item, parent_layout):
+    def __init__(
+        self, item: "DataItemVariable", parent_layout: "DataSetEditLayout"
+    ) -> None:
         AbstractDataSetWidget.__init__(self, item, parent_layout)
         self.group = QLabel()
         wordwrap = item.get_prop_value("display", "wordwrap", False)
         self.group.setWordWrap(wordwrap)
         self.group.setToolTip(item.get_help())
         self.group.setStyleSheet(LABEL_CSS)
-        self.group.setTextInteractionFlags(Qt.TextSelectableByMouse)
+        self.group.setTextInteractionFlags(Qt.TextSelectableByMouse)  # type:ignore
         # self.group.setEnabled(False)
 
-    def get(self):
+    def get(self) -> None:
         """Override AbstractDataSetWidget method"""
         self.set_state()
         text = self.item.get_string_value()
         self.group.setText(text)
 
-    def set(self):
+    def set(self) -> Any:
         """Read only..."""
         pass
 
 
 class ShowColorWidget(DataSetShowWidget):
     """Read-only color item widget"""
 
-    def __init__(self, item, parent_layout):
+    def __init__(
+        self, item: "DataItemVariable", parent_layout: "DataSetEditLayout"
+    ) -> None:
         DataSetShowWidget.__init__(self, item, parent_layout)
-        self.picture = None
+        self.picture: Optional[QPicture] = None
 
-    def get(self):
+    def get(self) -> None:
         """Override AbstractDataSetWidget method"""
         value = self.item.get()
         if value is not None:
             color = QColor(value)
             self.picture = QPicture()
             painter = QPainter()
             painter.begin(self.picture)
@@ -470,25 +524,31 @@
             self.group.setPicture(self.picture)
 
 
 class ShowBooleanWidget(DataSetShowWidget):
     """Read-only bool item widget"""
 
     def place_on_grid(
-        self, layout, row, label_column, widget_column, row_span=1, column_span=1
+        self,
+        layout: QGridLayout,
+        row: int,
+        label_column: int,
+        widget_column,
+        row_span: int = 1,
+        column_span: int = 1,
     ):
         """Override AbstractDataSetWidget method"""
         if not self.item.get_prop_value("display", "label"):
             widget_column = label_column
             column_span += 1
         else:
             self.place_label(layout, row, label_column)
         layout.addWidget(self.group, row, widget_column, row_span, column_span)
 
-    def get(self):
+    def get(self) -> None:
         """Override AbstractDataSetWidget method"""
         DataSetShowWidget.get(self)
         text = self.item.get_prop_value("display", "text")
         self.group.setText(text)
         font = self.group.font()
         value = self.item.get()
         state = bool(value)
@@ -502,15 +562,15 @@
 
     _widget_factory = {}
 
 
 class DataSetShowDialog(DataSetEditDialog):
     """Read-only dialog box"""
 
-    def layout_factory(self, instance, grid):
+    def layout_factory(self, instance: DataSet, grid: QGridLayout) -> DataSetShowLayout:
         """Override DataSetEditDialog method"""
         return DataSetShowLayout(self, instance, grid)
 
 
 DataSetShowLayout.register(GroupItem, GroupWidget)
 DataSetShowLayout.register(TabGroupItem, TabGroupWidget)
 DataSetShowLayout.register(FloatItem, DataSetShowWidget)
@@ -525,39 +585,42 @@
 DataSetShowLayout.register(FilesOpenItem, DataSetShowWidget)
 DataSetShowLayout.register(FileSaveItem, DataSetShowWidget)
 DataSetShowLayout.register(DirectoryItem, DataSetShowWidget)
 DataSetShowLayout.register(ChoiceItem, DataSetShowWidget)
 DataSetShowLayout.register(ImageChoiceItem, DataSetShowWidget)
 DataSetShowLayout.register(MultipleChoiceItem, DataSetShowWidget)
 DataSetShowLayout.register(FloatArrayItem, DataSetShowWidget)
+DataSetShowLayout.register(DictItem, DataSetShowWidget)
 
 
 class DataSetShowGroupBox(QGroupBox):
     """Group box widget showing a read-only DataSet"""
 
-    def __init__(self, label, klass, wordwrap=False, **kwargs):
+    def __init__(
+        self, label: QLabel, klass: Type, wordwrap: bool = False, **kwargs
+    ) -> None:
         QGroupBox.__init__(self, label)
-        self.apply_button = None
+        self.apply_button: Optional[QPushButton] = None
         self.klass = klass
         self.dataset = klass(**kwargs)
-        self.layout = QVBoxLayout()
+        self._layout = QVBoxLayout()
         if self.dataset.get_comment():
             label = QLabel(self.dataset.get_comment())
             label.setWordWrap(wordwrap)
-            self.layout.addWidget(label)
+            self._layout.addWidget(label)
         self.grid_layout = QGridLayout()
-        self.layout.addLayout(self.grid_layout)
-        self.setLayout(self.layout)
+        self._layout.addLayout(self.grid_layout)
+        self.setLayout(self._layout)
         self.edit = self.get_edit_layout()
 
-    def get_edit_layout(self):
+    def get_edit_layout(self) -> DataSetEditLayout:
         """Return edit layout"""
         return DataSetShowLayout(self, self.dataset, self.grid_layout)
 
-    def get(self):
+    def get(self) -> None:
         """Update group box contents from data item values"""
         for widget in self.edit.widgets:
             widget.build_mode = True
             widget.get()
             widget.build_mode = False
 
 
@@ -572,57 +635,60 @@
     """
 
     #: Signal emitted when Apply button is clicked
     SIG_APPLY_BUTTON_CLICKED = Signal()
 
     def __init__(
         self,
-        label,
-        klass,
-        button_text=None,
-        button_icon=None,
-        show_button=True,
-        wordwrap=False,
+        label: QLabel,
+        klass: Type,
+        button_text: Optional[str] = None,
+        button_icon: Optional[Union[QIcon, str]] = None,
+        show_button: bool = True,
+        wordwrap: bool = False,
         **kwargs
     ):
         DataSetShowGroupBox.__init__(self, label, klass, wordwrap=wordwrap, **kwargs)
         if show_button:
             if button_text is None:
                 button_text = _("Apply")
             if button_icon is None:
-                button_icon = get_icon("apply.png")
+                Qbutton_icon = get_icon("apply.png")
             elif isinstance(button_icon, str):
-                button_icon = get_icon(button_icon)
-            self.apply_button = applyb = QPushButton(button_icon, button_text, self)
-            applyb.clicked.connect(self.set)
+                Qbutton_icon = get_icon(button_icon)
+            self.apply_button = applyb = QPushButton(Qbutton_icon, button_text, self)
+            applyb.clicked.connect(self.set)  # type:ignore
             layout = self.edit.layout
-            layout.addWidget(applyb, layout.rowCount(), 0, 1, -1, Qt.AlignRight)
+            layout.addWidget(
+                applyb, layout.rowCount(), 0, 1, -1, Qt.AlignRight  # type:ignore
+            )
 
-    def get_edit_layout(self):
+    def get_edit_layout(self) -> DataSetEditLayout:
         """Return edit layout"""
         return DataSetEditLayout(
             self, self.dataset, self.grid_layout, change_callback=self.change_callback
         )
 
-    def change_callback(self):
+    def change_callback(self) -> None:
         """Method called when any widget's value has changed"""
         self.set_apply_button_state(True)
 
-    def set(self):
+    def set(self, check=True) -> None:
         """Update data item values from layout contents"""
         for widget in self.edit.widgets:
-            if widget.is_active() and widget.check():
-                widget.set()
+            if widget.is_active():
+                if not check or widget.check():
+                    widget.set()
         self.SIG_APPLY_BUTTON_CLICKED.emit()
         self.set_apply_button_state(False)
 
-    def set_apply_button_state(self, state):
+    def set_apply_button_state(self, state: bool) -> None:
         """Set apply button enable/disable state"""
         if self.apply_button is not None:
             self.apply_button.setEnabled(state)
 
-    def child_title(self, item):
+    def child_title(self, item: "DataItemVariable") -> str:
         """Return data item title combined with QApplication title"""
         app_name = QApplication.applicationName()
         if not app_name:
             app_name = str(self.title())
         return "%s - %s" % (app_name, item.label())
```

### Comparing `guidata-2.3.1/guidata/disthelpers.py` & `guidata-3.0.0/guidata/utils/disthelpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,156 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright © 2009-2011 CEA
-# Pierre Raybaut
-# Licensed under the terms of the CECILL License
-# (see guidata/__init__.py for details)
+# Licensed under the terms of the BSD 3-Clause
+# (see guidata/LICENSE for details)
 
 # pylint: disable=W0613
 
 """
 disthelpers
 -----------
 
 The ``guidata.disthelpers`` module provides helper functions for Python
 package distribution on Microsoft Windows platforms with ``py2exe`` or on
 all platforms thanks to ``cx_Freeze``.
 """
 
-import sys
+import atexit
+import importlib
+import importlib.machinery
+import inspect
 import os
 import os.path as osp
 import shutil
+import sys
 import traceback
-import atexit
-import imp
-from subprocess import Popen, PIPE
 import warnings
+from subprocess import PIPE, Popen
+
+if os.name == "nt":
+    try:
+        import py2exe  # Patching distutils -- analysis:ignore
+
+        PY2EXE_INSTALLED = True
+    except ImportError:
+        PY2EXE_INSTALLED = False
+
+try:
+    import cx_Freeze
+
+    CX_FREEZE_INSTALLED = True
+
+    # Workaround against duplicated ddl files
+    # https://github.com/anthony-tuininga/cx_Freeze/issues/366
+    # https://github.com/anthony-tuininga/cx_Freeze/pull/400
+    def _CopyFile(self, source, target, copyDependentFiles, includeMode=False):
+        normalizedSource = os.path.normcase(os.path.normpath(source))
+        normalizedTarget = os.path.normcase(os.path.normpath(target))
+        if normalizedTarget in self.filesCopied:
+            return
+        if normalizedSource == normalizedTarget:
+            return
+        self._RemoveFile(target)
+        targetDir = os.path.dirname(target)
+        self._CreateDirectory(targetDir)
+        if not self.silent:
+            sys.stdout.write("copying %s -> %s\n" % (source, target))
+        shutil.copyfile(source, target)
+        shutil.copystat(source, target)
+        if includeMode:
+            shutil.copymode(source, target)
+        self.filesCopied[normalizedTarget] = None
+        if copyDependentFiles and source not in self.finder.excludeDependentFiles:
+            for source in self._GetDependentFiles(source):
+                target = os.path.join(self.targetDir, os.path.basename(source))
+                self._CopyFile(source, target, copyDependentFiles)
+
+    from cx_Freeze import freezer
+
+    freezer.Freezer._CopyFile = _CopyFile
+except ImportError:
+    CX_FREEZE_INSTALLED = False
 
 # Local imports
 from guidata.configtools import get_module_path
 
 
 # ==============================================================================
+# modules management
+# ==============================================================================
+def atexit_deletion(path):
+    """
+    Function to call each time user want to delete file/folder at script end. To use with atexit.register()
+
+    :param path: the absolute path of the file/folder to delete
+    :type path: str
+    """
+
+    # We check if path really exists
+    if os.path.exists(path):
+        # We check if path is a file or a folder to use the right command
+        try:
+            if os.path.isfile(path):
+                os.remove(path)
+            else:
+                shutil.rmtree(path)
+        except:
+            print("Error during deleting path {0}".format(path))
+            traceback.print_exc()
+        else:
+            print("Path {0} deleting with success".format(path))
+    else:
+        print("file/folder {0} is not existing".format(path))
+
+
+def get_package_data(name, extlist, exclude_dirs=[]):
+    """
+    Return data files for package *name* with extensions in *extlist*
+    (search recursively in package directories)
+    """
+    assert isinstance(extlist, (list, tuple))
+    flist = []
+    # Workaround to replace os.path.relpath (not available until Python 2.6):
+    offset = len(name) + len(os.pathsep)
+    for dirpath, _dirnames, filenames in os.walk(name):
+        if dirpath not in exclude_dirs:
+            for fname in filenames:
+                if osp.splitext(fname)[1].lower() in extlist:
+                    flist.append(osp.join(dirpath, fname)[offset:])
+    return flist
+
+
+def get_subpackages(name):
+    """Return subpackages of package *name*"""
+    splist = []
+    for dirpath, _dirnames, _filenames in os.walk(name):
+        if osp.isfile(osp.join(dirpath, "__init__.py")):
+            splist.append(".".join(dirpath.split(os.sep)))
+    return splist
+
+
+def cythonize_all(relpath):
+    """Cythonize all Cython modules in relative path"""
+    from Cython.Compiler import Main
+
+    for fname in os.listdir(relpath):
+        if osp.splitext(fname)[1] == ".pyx":
+            Main.compile(osp.join(relpath, fname))
+
+
+# This is a list of module extensions (.pyd, .cp36-win_amd64.pyd, ...)
+# used to detect if a filename refers to a module
+# and to get the module from the filename.
+# The list is sorted by length in descending order
+# so that .cp36-win64.pyd like extensions are tested before .pyd.
+_MODULE_SUFFIXES = importlib.machinery.all_suffixes()
+_MODULE_SUFFIXES.sort(key=len, reverse=True)
+
+
+# ==============================================================================
 # Dependency management
 # ==============================================================================
 def get_changeset(path, rev=None):
     """Return Mercurial repository *path* revision number"""
     args = ["hg", "parent"]
     if rev is not None:
         args += ["--rev", str(rev)]
@@ -114,14 +230,19 @@
         # Python 2.6-2.7, 3.0-3.2 were built with Visual Studio 9.0.21022.8
         # (i.e. Visual C++ 2008, not Visual C++ 2008 SP1!)
         return "9.0.21022.8"
     elif python_version in ("3.3", "3.4"):
         # Python 3.3+ were built with Visual Studio 10.0.30319.1
         # (i.e. Visual C++ 2010)
         return "10.0"
+    elif python_version in ("3.5", "3.6"):
+        # Python 3.5+ were built with Visual Studio 14
+        # (i.e. Visual Studio 2015)
+        return "14.0"
+    # TODO : Add missing python versions
     else:
         raise RuntimeError("Unsupported Python version %s" % python_version)
 
 
 def get_dll_architecture(path):
     """Return DLL architecture (32 or 64bit) using Microsoft dumpbin.exe"""
     os.environ[
@@ -148,15 +269,15 @@
 
 def get_msvc_dlls(msvc_version, architecture=None, check_architecture=False):
     """Get the list of Microsoft Visual C++ DLLs associated to
     architecture and Python version, create the manifest file.
 
     architecture: integer (32 or 64) -- if None, take the Python build arch
     python_version: X.Y"""
-    current_architecture = 64 if sys.maxsize > 2 ** 32 else 32
+    current_architecture = 64 if sys.maxsize > 2**32 else 32
     if architecture is None:
         architecture = current_architecture
     assert architecture in (32, 64)
 
     filelist = []
 
     msvc_major = msvc_version.split(".")[0]
@@ -174,26 +295,26 @@
 
         for group, dll_list in groups.items():
             dlls = ""
             for dll in dll_list:
                 dlls += '    <file name="%s" />%s' % (dll, os.linesep)
 
             manifest = """<?xml version="1.0" encoding="UTF-8" standalone="yes"?>
-<!-- Copyright (c) Microsoft Corporation.  All rights reserved. -->
-<assembly xmlns="urn:schemas-microsoft-com:asm.v1" manifestVersion="1.0">
-    <noInheritable/>
-    <assemblyIdentity
-        type="%(atype)s"
-        name="Microsoft.VC90.%(group)s"
-        version="%(version)s"
-        processorArchitecture="%(arch)s"
-        publicKeyToken="%(key)s"
-    />
-%(dlls)s</assembly>
-""" % dict(
+            <!-- Copyright (c) Microsoft Corporation.  All rights reserved. -->
+            <assembly xmlns="urn:schemas-microsoft-com:asm.v1" manifestVersion="1.0">
+                <noInheritable/>
+                <assemblyIdentity
+                    type="%(atype)s"
+                    name="Microsoft.VC90.%(group)s"
+                    version="%(version)s"
+                    processorArchitecture="%(arch)s"
+                    publicKeyToken="%(key)s"
+                />
+            %(dlls)s</assembly>
+            """ % dict(
                 version=msvc_version,
                 key=key,
                 atype=atype,
                 arch=arch,
                 group=group,
                 dlls=dlls,
             )
@@ -394,14 +515,28 @@
         self.bin_path_excludes = self.DEFAULT_BIN_PATH_EXCLUDES
         self.msvc = os.name == "nt"
         self._py2exe_is_loaded = False
         self._pyqt_added = False
         self._pyside_added = False
         # Attributes relative to cx_Freeze:
         self.executables = []
+        self.include_msvcr = False
+        self.module_import_func_dict = {
+            "PyQt5": self.add_pyqt,
+            "PySide": self.add_pyside,
+            "scipy": self.add_module_dir,
+            "matplotlib": self.add_matplotlib,
+            "h5py": self.add_h5py,
+            "docutils": self.add_doc_module,
+            "rst2pdf": self.add_doc_module,
+            "sphinx": self.add_doc_module,
+            "pygments": self.add_pygments,
+            "zmq": self.add_zmq,
+            "zmq": self.add_guidata,
+        }
 
     @property
     def target_dir(self):
         """Return target directory (default: 'dist')"""
         dirname = self._target_dir
         if dirname is None:
             return "dist"
@@ -425,14 +560,15 @@
         includes=None,
         excludes=None,
         bin_includes=None,
         bin_excludes=None,
         bin_path_includes=None,
         bin_path_excludes=None,
         msvc=None,
+        include_msvcr=False,
     ):
         """Setup distribution object
 
         Notes:
           * bin_path_excludes is specific to cx_Freeze (ignored if it's None)
           * if msvc is None, it's set to True by default on Windows
             platforms, False on non-Windows platforms
@@ -466,23 +602,24 @@
                 self.data_files += create_msvc_data_files()
             except IOError:
                 print(
                     "Setting the msvc option to False " "will avoid this error",
                     file=sys.stderr,
                 )
                 raise
+        self.include_msvcr = include_msvcr
         # cx_Freeze:
         self.add_executable(self.script, self.target_name, icon=self.icon)
 
     def add_text_data_file(self, filename, contents):
         """Create temporary data file *filename* with *contents*
         and add it to *data_files*"""
         open(filename, "wb").write(bytes(contents, "utf-8"))
         self.data_files += [("", (filename,))]
-        _remove_later(filename)
+        atexit.register(atexit_deletion, os.path.abspath(filename))
 
     def add_data_file(self, filename, destdir=""):
         self.data_files += [(destdir, (filename,))]
 
     # ------ Adding packages
     def add_pyqt(self):
         """Include module PyQt5 to the distribution"""
@@ -492,17 +629,17 @@
         self._pyqt_added = True
 
         import PyQt5 as PyQt
 
         qtver = 5
         self.includes += [
             "sip",
-            "PyQt%d.Qt" % qtver,
-            "PyQt%d.QtSvg" % qtver,
-            "PyQt%d.QtNetwork" % qtver,
+            f"PyQt{qtver}.Qt",
+            f"PyQt{qtver}.QtSvg",
+            f"PyQt{qtver}.QtNetwork",
         ]
 
         pyqt_path = osp.dirname(PyQt.__file__)
 
         # Configuring PyQt
         conf = os.linesep.join(["[Paths]", "Prefix = .", "Binaries = ."])
         self.add_text_data_file("qt.conf", conf)
@@ -539,15 +676,15 @@
                 # there must be a manifest file as well...
                 # ...congrats to Microsoft for this great simplification!
                 filelist.append(vc90man_pyqt)
             self.data_files.append(
                 (dirpath[len(pyqt_path) + len(os.pathsep) :], filelist)
             )
         if self.msvc:
-            atexit.register(remove_dir, pyqt_tmp)
+            atexit.register(atexit_deletion, os.path.abspath(pyqt_tmp))
 
         # Including french translation
         fr_trans = osp.join(pyqt_path, "translations", "qt_fr.qm")
         if osp.exists(fr_trans):
             self.data_files.append(("translations", (fr_trans,)))
 
     def add_pyside(self):
@@ -623,15 +760,15 @@
         fr_trans = osp.join(pyside_path, "translations", "qt_fr.qm")
         if osp.exists(fr_trans):
             self.data_files.append(("translations", (fr_trans,)))
 
     def add_qt_bindings(self):
         """Include Qt bindings, i.e. PyQt or PySide"""
         try:
-            imp.find_module("PyQt5")
+            importlib.find_module("PyQt5")
             self.add_modules("PyQt5")
         except ImportError:
             self.add_modules("PySide")
 
     def add_matplotlib(self):
         """Include module Matplotlib to the distribution"""
         if "matplotlib" in self.excludes:
@@ -661,99 +798,103 @@
                 ".ppm",
                 ".npy",
                 ".afm",
                 ".ttf",
             ),
         )
 
+    def add_h5py(self):
+        self.add_module_dir("h5py")
+        if self.bin_path_excludes is not None and os.name == "nt":
+            # Specific to cx_Freeze on Windows: avoid including a zlib dll
+            # built with another version of Microsoft Visual Studio
+            self.bin_path_excludes += [
+                r"C:\Program Files",
+                r"C:\Program Files (x86)",
+            ]
+            self.data_files.append(  # necessary for cx_Freeze only
+                ("", (osp.join(get_module_path("h5py"), "zlib1.dll"),))
+            )
+
+    def add_doc_module(self, module_name):
+        self.includes += [
+            "docutils.writers.null",
+            "docutils.languages.en",
+            "docutils.languages.fr",
+        ]
+        if module_name == "rst2pdf":
+            self.add_module_data_files(
+                "rst2pdf", ("styles",), (".json", ".style"), copy_to_root=True
+            )
+        if module_name == "sphinx":
+            import sphinx.ext
+
+            for fname in os.listdir(osp.dirname(sphinx.ext.__file__)):
+                if osp.splitext(fname)[1] == ".py":
+                    modname = "sphinx.ext.%s" % osp.splitext(fname)[0]
+                    self.includes.append(modname)
+
+    def add_pygments(self):
+        self.includes += [
+            "pygments",
+            "pygments.formatters",
+            "pygments.lexers",
+            "pygments.lexers.agile",
+        ]
+
+    def add_zmq(self):
+        # FIXME: this is not working, yet... (missing DLL)
+        self.includes += [
+            "zmq",
+            "zmq.core._poll",
+            "zmq.core._version",
+            "zmq.core.constants",
+            "zmq.core.context",
+            "zmq.core.device",
+            "zmq.core.error",
+            "zmq.core.message",
+            "zmq.core.socket",
+            "zmq.core.stopwatch",
+        ]
+        if os.name == "nt":
+            self.bin_includes += ["libzmq.dll"]
+
+    def add_guidata(self):
+        self.add_module_data_files(
+            "guidata", ("images",), (".png", ".svg"), copy_to_root=False
+        )
+        self.add_qt_bindings()
+
     def add_modules(self, *module_names):
         """Include module *module_name*"""
+        # TODO: Add support for PyQt6
         for module_name in module_names:
-            print("Configuring module '%s'" % module_name)
-            # TODO: Add support for PyQt6
-            if module_name == "PyQt5":
-                self.add_pyqt()
-            elif module_name == "PySide":
-                self.add_pyside()
-            elif module_name == "scipy":
-                self.add_module_dir("scipy")
-            elif module_name == "matplotlib":
-                self.add_matplotlib()
-            elif module_name == "h5py":
-                self.add_module_dir("h5py")
-                if self.bin_path_excludes is not None and os.name == "nt":
-                    # Specific to cx_Freeze on Windows: avoid including a zlib dll
-                    # built with another version of Microsoft Visual Studio
-                    self.bin_path_excludes += [
-                        r"C:\Program Files",
-                        r"C:\Program Files (x86)",
-                    ]
-                    self.data_files.append(  # necessary for cx_Freeze only
-                        ("", (osp.join(get_module_path("h5py"), "zlib1.dll"),))
-                    )
-            elif module_name in ("docutils", "rst2pdf", "sphinx"):
-                self.includes += [
-                    "docutils.writers.null",
-                    "docutils.languages.en",
-                    "docutils.languages.fr",
-                ]
-                if module_name == "rst2pdf":
-                    self.add_module_data_files(
-                        "rst2pdf", ("styles",), (".json", ".style"), copy_to_root=True
-                    )
-                if module_name == "sphinx":
-                    import sphinx.ext
-
-                    for fname in os.listdir(osp.dirname(sphinx.ext.__file__)):
-                        if osp.splitext(fname)[1] == ".py":
-                            modname = "sphinx.ext.%s" % osp.splitext(fname)[0]
-                            self.includes.append(modname)
-            elif module_name == "pygments":
-                self.includes += [
-                    "pygments",
-                    "pygments.formatters",
-                    "pygments.lexers",
-                    "pygments.lexers.agile",
-                ]
-            elif module_name == "zmq":
-                # FIXME: this is not working, yet... (missing DLL)
-                self.includes += [
-                    "zmq",
-                    "zmq.core._poll",
-                    "zmq.core._version",
-                    "zmq.core.constants",
-                    "zmq.core.context",
-                    "zmq.core.device",
-                    "zmq.core.error",
-                    "zmq.core.message",
-                    "zmq.core.socket",
-                    "zmq.core.stopwatch",
-                ]
-                if os.name == "nt":
-                    self.bin_includes += ["libzmq.dll"]
-            elif module_name == "guidata":
-                self.add_module_data_files(
-                    "guidata", ("images",), (".png", ".svg"), copy_to_root=False
-                )
-                self.add_qt_bindings()
-            elif module_name == "guiqwt":
-                self.add_module_data_files(
-                    "guiqwt", ("images",), (".png", ".svg"), copy_to_root=False
-                )
-                if os.name == "nt":
-                    # Specific to cx_Freeze: including manually MinGW DLLs
-                    self.bin_includes += ["libgcc_s_dw2-1.dll", "libstdc++-6.dll"]
+            print(f"Configuring module '{module_name}'")
+            if module_name in self.module_import_func_dict.keys():
+                func = self.module_import_func_dict[module_name]
+                if not inspect.getargspec().args:
+                    func()
+                else:
+                    func(module_name)
             else:
                 try:
                     # Modules based on the same scheme as guidata and guiqwt
                     self.add_module_data_files(
                         module_name, ("images",), (".png", ".svg"), copy_to_root=False
                     )
                 except IOError:
-                    raise RuntimeError("Module not supported: %s" % module_name)
+                    raise RuntimeError(f"Module not supported:{module_name}")
+            # XXX: guiqwt ref, delete ?
+            # if module_name == "guiqwt":
+            #     self.add_module_data_files(
+            #         "guiqwt", ("images",), (".png", ".svg"), copy_to_root=False
+            #     )
+            #     if os.name == "nt":
+            #         # Specific to cx_Freeze: including manually MinGW DLLs
+            #         self.bin_includes += ["libgcc_s_dw2-1.dll", "libstdc++-6.dll"]
 
     def add_module_data_dir(
         self,
         module_name,
         data_dir_name,
         extensions,
         copy_to_root=True,
@@ -765,15 +906,15 @@
         and add them to *data_files*
         *extensions*: list of file extensions, e.g. ('.png', '.svg')
         """
         module_dir = get_module_path(module_name)
         nstrip = len(module_dir) + len(osp.sep)
         data_dir = osp.join(module_dir, data_dir_name)
         if not osp.isdir(data_dir):
-            raise IOError("Directory not found: %s" % data_dir)
+            raise IOError(f"Directory not found: {data_dir}")
         for dirpath, _dirnames, filenames in os.walk(data_dir):
             dirname = dirpath[nstrip:]
             if osp.basename(dirpath) in exclude_dirs:
                 continue
             if not copy_to_root:
                 dirname = osp.join(module_name, dirname)
             pathlist = [
@@ -802,15 +943,18 @@
             dirname = osp.join(module_name, dirpath[nstrip:])
             for filename in filenames:
                 ext = osp.splitext(filename)[1].lower()
                 if ext in (".py", ".pyd"):
                     if filename == "__init__.py":
                         fn = dirname
                     else:
-                        fn = osp.splitext(osp.join(dirname, filename))[0]
+                        for suffix in _MODULE_SUFFIXES:
+                            if filename.endswith(suffix):
+                                fn = osp.join(dirname, filename[: -len(suffix)])
+                                break
                     if fn.endswith(os.sep):
                         fn = fn[:-1]
                     modname = ".".join(fn.split(os.sep))
                     self.includes += [modname]
                     if verbose:
                         print("  + ", modname)
 
@@ -825,40 +969,45 @@
     ):
         """
         Collect data files for module *module_name* and add them to *data_files*
         *data_dir_names*: list of dirnames, e.g. ('images', )
         *extensions*: list of file extensions, e.g. ('.png', '.svg')
         """
         print(
-            "Adding module '%s' data files in %s (%s)"
-            % (module_name, ", ".join(data_dir_names), ", ".join(extensions))
+            "Adding module '{}' data files in {} ({})".format(
+                module_name,
+                ", ".join(data_dir_names),
+                ", ".join(extensions),
+            )
         )
         module_dir = get_module_path(module_name)
         for data_dir_name in data_dir_names:
             self.add_module_data_dir(
                 module_name,
                 data_dir_name,
                 extensions,
                 copy_to_root,
                 verbose,
                 exclude_dirs,
             )
         translation_file = osp.join(
-            module_dir, "locale", "fr", "LC_MESSAGES", "%s.mo" % module_name
+            module_dir, "locale", "fr", "LC_MESSAGES", f"{module_name}.mo"
         )
         if osp.isfile(translation_file):
             self.data_files.append(
                 (
                     osp.join(module_name, "locale", "fr", "LC_MESSAGES"),
                     (translation_file,),
                 )
             )
             print(
-                "Adding module '%s' translation file: %s"
-                % (module_name, osp.basename(translation_file))
+                "Adding module '{}' translation file: {}".format(
+                    module_name,
+                    osp.basename(translation_file),
+                )
             )
 
     def build(self, library, cleanup=True, create_archive=None):
         """Build executable with given library.
 
         library:
             * 'py2exe': deploy using the `py2exe` library
@@ -889,15 +1038,15 @@
         """Create a ZIP archive
 
         option:
             * 'add': add target directory to a ZIP archive
             * 'move': move target directory to a ZIP archive
         """
         name = self.target_dir
-        os.system('zip "%s.zip" -r "%s"' % (name, name))
+        os.system(f'python -m zipfile -c "{name}.zip" "{name}"')
         if option == "move":
             shutil.rmtree(name)
 
     def build_py2exe(
         self,
         cleanup=True,
         compressed=2,
@@ -911,16 +1060,20 @@
         cleanup: remove 'build/dist' directories before building distribution
 
         create_archive (requires the executable `zip`):
             * None or False: do nothing
             * 'add': add target directory to a ZIP archive
             * 'move': move target directory to a ZIP archive
         """
+        if not PY2EXE_INSTALLED:
+            raise RuntimeError(
+                "You must install py2exe in order to build the executable"
+            )
+
         from distutils.core import setup
-        import py2exe  # Patching distutils -- analysis:ignore
 
         self._py2exe_is_loaded = True
         if cleanup:
             self.__cleanup()
         sys.argv += ["py2exe"]
         options = dict(
             compressed=compressed,
@@ -951,14 +1104,16 @@
         )
         if create_archive:
             self.__create_archive(create_archive)
 
     def add_executable(self, script, target_name, icon=None):
         """Add executable to the cx_Freeze distribution
         Not supported for py2exe"""
+        if not CX_FREEZE_INSTALLED:
+            return
         from cx_Freeze import Executable
 
         base = None
         if script.endswith(".pyw") and os.name == "nt":
             base = "win32gui"
         self.executables += [
             Executable(script, base=base, icon=icon, targetName=target_name)
@@ -970,19 +1125,21 @@
         cleanup: remove 'build/dist' directories before building distribution
 
         create_archive (requires the executable `zip`):
             * None or False: do nothing
             * 'add': add target directory to a ZIP archive
             * 'move': move target directory to a ZIP archive
         """
+        if not CX_FREEZE_INSTALLED:
+            raise RuntimeError(
+                "You must install cx_Freeze in order to build the executable"
+            )
         assert not self._py2exe_is_loaded, "cx_Freeze can't be executed after py2exe"
-        from cx_Freeze import setup
-
         # ===== Monkey-patching cx_Freeze (backported from v5.0 dev) ===========
-        from cx_Freeze import hooks
+        from cx_Freeze import hooks, setup
 
         def load_h5py(finder, module):
             """h5py module has a number of implicit imports"""
             finder.IncludeModule("h5py.defs")
             finder.IncludeModule("h5py.utils")
             finder.IncludeModule("h5py._proxy")
             try:
@@ -1004,24 +1161,29 @@
         hooks.load_scipy = load_scipy
         # ===== Monkey-patching cx_Freeze for Scipy ============================
 
         if cleanup:
             self.__cleanup()
         sys.argv += ["build"]
         excv = "3" if sys.version[0] == "2" else "2"
-        self.excludes += ["sympy.mpmath.libmp.exec_py%s" % excv]
+        self.excludes += [f"sympy.mpmath.libmp.exec_py{excv}"]
+        self.excludes += [f"PyQt4.uic.port_v{excv}"]
         build_exe = dict(
             include_files=to_include_files(self.data_files),
             includes=self.includes,
             excludes=self.excludes,
             bin_excludes=self.bin_excludes,
             bin_includes=self.bin_includes,
             bin_path_includes=self.bin_path_includes,
             bin_path_excludes=self.bin_path_excludes,
             build_exe=self.target_dir,
+            optimize=0,
+            zip_include_packages="*",
+            zip_exclude_packages=["numpy", "pandas"],
+            include_msvcr=self.include_msvcr,
         )
         setup(
             name=self.name,
             version=self.version,
             description=self.description,
             executables=self.executables,
             options=dict(build_exe=build_exe),
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `guidata-2.3.1/guidata/encoding.py` & `guidata-3.0.0/guidata/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/external/darkdetect/__init__.py` & `guidata-3.0.0/guidata/external/darkdetect/__init__.py`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/external/darkdetect/_linux_detect.py` & `guidata-3.0.0/guidata/external/darkdetect/_linux_detect.py`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/external/darkdetect/_mac_detect.py` & `guidata-3.0.0/guidata/external/darkdetect/_mac_detect.py`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/external/darkdetect/_windows_detect.py` & `guidata-3.0.0/guidata/external/darkdetect/_windows_detect.py`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/gettext_helpers.py` & `guidata-3.0.0/guidata/utils/gettext_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright © 2009-2010 CEA
-# Pierre Raybaut
-# Licensed under the terms of the CECILL License
-# (see guidata/__init__.py for details)
+# Licensed under the terms of the BSD 3-Clause
+# (see guidata/LICENSE for details)
 
-import sys
 import os
 import os.path as osp
 import subprocess
+import sys
 
 if os.name == "nt":
     # Find pygettext.py source on a windows install
     pygettext = ["python", osp.join(sys.prefix, "Tools", "i18n", "pygettext.py")]
     msgfmt = ["python", osp.join(sys.prefix, "Tools", "i18n", "msgfmt.py")]
 else:
     pygettext = ["pygettext"]
```

### Comparing `guidata-2.3.1/guidata/guitest.py` & `guidata-3.0.0/guidata/guitest.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,222 +1,351 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright © 2009-2010 CEA
-# Pierre Raybaut
-# Licensed under the terms of the CECILL License
-# (see guidata/__init__.py for details)
+# Licensed under the terms of the BSD 3-Clause
+# (see guidata/LICENSE for details)
 
 """
 GUI-based test launcher
+-----------------------
+
+Overview
+^^^^^^^^
+
+This module provides a GUI-based test launcher for any Python package.
+
+Usage example::
+
+    import your_package
+
+    from guidata.guitest import run_testlauncher
+    run_testlauncher(your_package)
+
+Reference/API
+^^^^^^^^^^^^^
+
+.. autofunction:: run_testlauncher
+
+.. autoclass:: TestModule
+
+.. autofunction:: get_tests
+
 """
 
-import sys
+from __future__ import annotations
+
 import os
 import os.path as osp
+import re
 import subprocess
+import sys
 import traceback
+from types import ModuleType
 
-# Local imports
-from qtpy.QtWidgets import (
-    QWidget,
-    QVBoxLayout,
-    QSplitter,
-    QListWidget,
-    QPushButton,
-    QLabel,
-    QGroupBox,
-    QHBoxLayout,
-    QShortcut,
-    QMainWindow,
-    QFrame,
-)
-from qtpy.QtGui import QKeySequence, QColor
-from qtpy.QtCore import Qt, QSize
+from qtpy import QtCore as QC
+from qtpy import QtGui as QG
+from qtpy import QtWidgets as QW
 
-from guidata.config import _
-from guidata.configtools import get_icon
+from guidata.config import CONF, _
+from guidata.configtools import get_font, get_icon
 from guidata.qthelpers import get_std_icon, win32_fix_title_bar_background
 from guidata.widgets.codeeditor import CodeEditor
 
 
-def get_test_package(package):
-    """Return test package for package"""
+def get_test_package(package) -> str:
+    """Return test package for package
+
+    Args:
+        package (module): package to test
+
+    Returns:
+        str: test package
+    """
     test_package_name = "%s.tests" % package.__name__
     _temp = __import__(test_package_name)
     return sys.modules[test_package_name]
 
 
-def get_tests(package):
-    """Retrieve test scripts from test package"""
+def get_tests(package, category: str) -> list[TestModule]:
+    """Retrieve test scripts from test package
+
+    Args:
+        package (module): package to test
+        category (str): test category (values: "all", "visible", "batch")
+
+    Returns:
+        list[TestModule]: list of test modules
+    """
+    assert category in ("all", "visible", "batch")
     tests = []
     test_package = get_test_package(package)
     test_path = osp.dirname(osp.realpath(test_package.__file__))
-    for fname in sorted(os.listdir(test_path)):
-        path = osp.join(test_path, fname)
-        if fname.endswith((".py", ".pyw")) and not fname.startswith("_"):
-            test = TestModule(test_package, path)
-            if test.is_visible():
-                tests.append(test)
+    # Iterate over test scripts recursively within test package:
+    for root, _dirs, files in os.walk(test_path):
+        for fname in files:
+            path = osp.join(root, fname)
+            if fname.endswith((".py", ".pyw")) and not fname.startswith("_"):
+                test = TestModule(test_package, path)
+                if (
+                    category == "all"
+                    or (category == "visible" and test.is_visible())
+                    or (category == "batch" and not test.is_skipped())
+                ):
+                    tests.append(test)
     return tests
 
 
-class TestModule(object):
-    """Object representing a test module (Python script)"""
+class TestModule:
+    """Object representing a test module (Python script)
+
+    Args:
+        test_package (module): test package
+        path (str): test module path
+    """
 
-    def __init__(self, test_package, path):
+    def __init__(self, test_package, path: str) -> None:
         self.path = path
+        test_package_path = osp.dirname(osp.realpath(test_package.__file__))
+        self.name = osp.relpath(self.path, test_package_path)
         module_name, _ext = osp.splitext(osp.basename(path))
+        subpkgname = test_package.__name__
+        if len(self.name.split(os.sep)) > 1:
+            subpkgname += "." + ".".join(self.name.split(os.sep)[:-1])
         try:
             self.error_msg = ""
-            _temp = __import__(test_package.__name__, fromlist=[module_name])
+            _temp = __import__(subpkgname, fromlist=[module_name])
             self.module = getattr(_temp, module_name)
         except ImportError:
             self.error_msg = traceback.format_exc()
             self.module = None
+        self.__is_visible = False
+        self.__is_skipped = False
+        self.__contents = ""
+        self.__read_contents()
+
+    def __read_contents(self) -> str:
+        """Read test module contents"""
+        with open(self.path, "r", encoding="utf-8") as fdesc:
+            lines = fdesc.readlines()
+        startline = 0
+        for lineno, line in enumerate(lines):
+            if re.match(r"^#[ ]*guitest[ ]*:", line.strip()):
+                if "show" in line:
+                    self.__is_visible = True
+                    startline = lineno + 1
+                if "skip" in line:
+                    self.__is_skipped = True
+        self.__contents = "".join(lines[startline:]).strip()
+
+    def is_visible(self) -> bool:
+        """Returns True if test module is visible"""
+        return self.__is_visible
+
+    def is_skipped(self) -> bool:
+        """Returns True if test module is skipped"""
+        return self.__is_skipped
+
+    def get_contents(self) -> str:
+        """Returns test module contents"""
+        return self.__contents
 
-    def is_visible(self):
-        """Returns True if this script is intended to be shown in test launcher"""
-        return self.module is None or (
-            hasattr(self.module, "SHOW") and self.module.SHOW
-        )
-
-    def is_valid(self):
+    def is_valid(self) -> bool:
         """Returns True if test module is valid and can be executed"""
         return self.module is not None
 
-    def get_description(self):
+    def get_description(self) -> str:
         """Returns test module description"""
         if self.is_valid():
             doc = self.module.__doc__
             if doc is None or not doc.strip():
                 return _("No description available")
             lines = doc.strip().splitlines()
             fmt = "<span style='color: #2222FF'><b>%s</b></span>"
             lines[0] = fmt % lines[0]
             return "<br>".join(lines)
         return self.error_msg
 
-    def run(self, args="", timeout=None):
-        """Run test script"""
+    def run(self, args: str = "", timeout: int = None) -> None:
+        """Run test script
+
+        Args:
+            args (str, optional): arguments to pass to the script
+            timeout (int, optional): timeout in seconds
+        """
         # Keep the same sys.path environment in child process:
         # (useful when the program is executed from Spyder, for example)
         os.environ["PYTHONPATH"] = os.pathsep.join(sys.path)
 
         command = [sys.executable, '"' + self.path + '"']
         if args:
             command.append(args)
         proc = subprocess.Popen(" ".join(command), shell=True)
         if timeout is not None:
             proc.wait(timeout)
 
 
-class TestPropertiesWidget(QWidget):
-    """Test module properties panel"""
+class TestPropertiesWidget(QW.QWidget):
+    """Test module properties panel
 
-    def __init__(self, parent):
-        QWidget.__init__(self, parent)
-        self.lbl_icon = QLabel()
+    Args:
+        parent (QWidget, optional): parent widget
+    """
+
+    def __init__(self, parent: QW.QWidget = None) -> None:
+        super().__init__(parent)
+        self.lbl_icon = QW.QLabel()
         self.lbl_icon.setFixedWidth(32)
-        self.desc_label = QLabel()
-        self.desc_label.setTextInteractionFlags(Qt.TextSelectableByMouse)
+        self.desc_label = QW.QLabel()
+        self.desc_label.setTextInteractionFlags(QC.Qt.TextSelectableByMouse)
         self.desc_label.setWordWrap(True)
-        group_desc = QGroupBox(_("Description"), self)
-        layout = QHBoxLayout()
+        group_desc = QW.QGroupBox(_("Description"), self)
+        layout = QW.QHBoxLayout()
         for label in (self.lbl_icon, self.desc_label):
-            label.setAlignment(Qt.AlignTop)
+            label.setAlignment(QC.Qt.AlignTop)
             layout.addWidget(label)
         group_desc.setLayout(layout)
 
-        self.editor = CodeEditor(self, columns=85, rows=30, language="python")
+        font = get_font(CONF, "codeeditor")
+        font.setPointSize(9)
+        self.editor = CodeEditor(
+            self, columns=85, rows=30, language="python", font=font
+        )
+        self.editor.setFont(font)
         self.editor.setReadOnly(True)
-        self.desc_label.setFont(self.editor.font())
+        self.desc_label.setFont(font)
 
-        vlayout = QVBoxLayout()
+        vlayout = QW.QVBoxLayout()
         vlayout.addWidget(group_desc)
         vlayout.addWidget(self.editor)
         self.setLayout(vlayout)
 
-    def set_item(self, test):
-        """Set current item"""
+    def set_item(self, test: TestModule) -> None:
+        """Set current item
+
+        Args:
+            test (TestModule): test module
+        """
         self.desc_label.setText(test.get_description())
-        self.editor.set_text_from_file(test.path)
+        self.editor.setPlainText(test.get_contents())
         txt = "Information" if test.is_valid() else "Critical"
         self.lbl_icon.setPixmap(get_std_icon("MessageBox" + txt).pixmap(24, 24))
 
 
-class TestMainView(QSplitter):
-    """Test launcher main view"""
+class TestMainView(QW.QSplitter):
+    """Test launcher main view
+
+    Args:
+        package (module): test package
+        parent (QWidget, optional): parent widget
+    """
 
     def __init__(self, package, parent=None):
-        QSplitter.__init__(self, parent)
-        self.tests = get_tests(package)
+        super().__init__(parent)
+        self.tests = get_tests(package, category="visible")
 
-        listgroup = QFrame()
+        listgroup = QW.QFrame()
         self.addWidget(listgroup)
         self.props = TestPropertiesWidget(self)
         font = self.props.editor.font()
         self.addWidget(self.props)
 
-        vlayout = QVBoxLayout()
+        vlayout = QW.QVBoxLayout()
         self.run_button = self.create_run_button(font)
         self.listw = self.create_test_listwidget(font)
         vlayout.addWidget(self.listw)
         vlayout.addWidget(self.run_button)
         listgroup.setLayout(vlayout)
 
         self.setStretchFactor(1, 1)
-        self.props.set_item(self.tests[0])
 
-    def create_test_listwidget(self, font):
-        """Create and setup test list widget"""
-        listw = QListWidget(self)
-        listw.addItems([osp.basename(test.path) for test in self.tests])
+        enabled = len(self.tests) > 0
+        self.run_button.setEnabled(enabled)
+        if enabled:
+            self.props.set_item(self.tests[0])
+
+    def create_test_listwidget(self, font: QG.QFont) -> QW.QListWidget:
+        """Create and setup test list widget
+
+        Args:
+            font (QFont): font to use
+
+        Returns:
+            QListWidget: test list widget
+        """
+        listw = QW.QListWidget(self)
+        listw.addItems([test.name for test in self.tests])
         for index in range(listw.count()):
             item = listw.item(index)
-            item.setSizeHint(QSize(1, 25))
+            item.setSizeHint(QC.QSize(1, 25))
             if not self.tests[index].is_valid():
-                item.setForeground(QColor("#FF3333"))
+                item.setForeground(QG.QColor("#FF3333"))
         listw.setFont(font)
         listw.currentRowChanged.connect(self.current_row_changed)
         listw.itemActivated.connect(self.run_current_script)
         listw.setCurrentRow(0)
         return listw
 
-    def create_run_button(self, font):
-        """Create and setup run button"""
-        btn = QPushButton(get_icon("apply.png"), _("Run this script"), self)
+    def create_run_button(self, font: QG.QFont) -> QW.QPushButton:
+        """Create and setup run button
+
+        Args:
+            font (QFont): font to use
+
+        Returns:
+            QPushButton: run button
+        """
+        btn = QW.QPushButton(get_icon("apply.png"), _("Run this script"), self)
         btn.setFont(font)
         btn.clicked.connect(self.run_current_script)
         return btn
 
-    def current_row_changed(self, row):
-        """Current list widget row has changed"""
+    def current_row_changed(self, row: int) -> None:
+        """Current list widget row has changed
+
+        Args:
+            row (int): row index
+        """
         current_test = self.tests[row]
         self.props.set_item(current_test)
         self.run_button.setEnabled(current_test.is_valid())
 
-    def run_current_script(self):
+    def run_current_script(self) -> None:
         """Run current script"""
         self.tests[self.listw.currentRow()].run()
 
 
-class TestLauncherWindow(QMainWindow):
-    """Test launcher main window"""
+class TestLauncherWindow(QW.QMainWindow):
+    """Test launcher main window
 
-    def __init__(self, package, parent=None):
-        QMainWindow.__init__(self, parent)
+    Args:
+        package (module): test package
+        parent (QWidget, optional): parent widget
+    """
+
+    def __init__(self, package, parent: QW.QWidget = None) -> None:
+        super().__init__(parent)
         win32_fix_title_bar_background(self)
         self.setWindowTitle(_("Tests - %s module") % package.__name__)
         self.setWindowIcon(get_icon("%s.svg" % package.__name__, "guidata.svg"))
         self.mainview = TestMainView(package, self)
         self.setCentralWidget(self.mainview)
-        QShortcut(QKeySequence("Escape"), self, self.close)
-
+        QW.QShortcut(QG.QKeySequence("Escape"), self, self.close)
 
-def run_testlauncher(package):
-    """Run test launcher"""
-    from guidata import qapplication
+    def show(self):
+        """Show window"""
+        super().show()
+        if not self.mainview.tests:
+            msg = _("No test found in this package.")
+            QW.QMessageBox.critical(self, _("Error"), msg)
+
+
+def run_testlauncher(package: ModuleType) -> None:
+    """Run test launcher
+
+    Args:
+        package (module): test package
+    """
+    from guidata import qapplication  # pylint: disable=import-outside-toplevel
 
     app = qapplication()
     win = TestLauncherWindow(package)
     win.show()
     app.exec_()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `guidata-2.3.1/guidata/hdf5io.py` & `guidata-3.0.0/guidata/widgets/console/interpreter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,392 +1,352 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright © 2009-2010 CEA
-# Pierre Raybaut
-# Licensed under the terms of the CECILL License
-# (see guidata/__init__.py for details)
-
-"""
-Reader and Writer for the serialization of DataSets into HDF5 files
-"""
-
+# Copyright © Spyder Project Contributors
+# Licensed under the terms of the MIT License
+# (see spyder/__init__.py for details)
+
+"""Shell Interpreter"""
+
+import atexit
+import ctypes
+import os
+import os.path as osp
+import pydoc
+import re
 import sys
-from uuid import uuid1
-
-import h5py
-import numpy as np
-
-from guidata.utils import utf8_to_unicode
-from guidata.userconfigio import BaseIOHandler, WriterMixin
-
-
-class TypeConverter(object):
-    def __init__(self, to_type, from_type=None):
-        self._to_type = to_type
-        if from_type:
-            self._from_type = from_type
-        else:
-            self._from_type = to_type
+import threading
+from code import InteractiveConsole
 
-    def to_hdf(self, value):
-        try:
-            return self._to_type(value)
-        except:
-            print("ERR", repr(value), file=sys.stderr)
-            raise
+from guidata.utils.misc import getcwd_or_home, remove_backslashes, run_shell_command
+from guidata.widgets.console.dochelpers import isdefined
 
-    def from_hdf(self, value):
-        return self._from_type(value)
+sys.path.insert(0, "")
 
 
-unicode_hdf = TypeConverter(lambda x: x.encode("utf-8"), lambda x: str(x, "utf-8"))
-int_hdf = TypeConverter(int)
-
-
-class Attr(object):
-    """Helper class representing class attribute that
-    should be saved/restored to/from a corresponding HDF5 attribute
-
-    hdf_name : name of the attribute in the HDF5 file
-    struct_name : name of the attribute in the object (default to hdf_name)
-    type : attribute type (guess it if None)
-    optional : indicates whether we should fail if the attribute is not present
-    """
-
-    def __init__(self, hdf_name, struct_name=None, type=None, optional=False):
-        self.hdf_name = hdf_name
-        if struct_name is None:
-            struct_name = hdf_name
-        self.struct_name = struct_name
-        self.type = type
-        self.optional = optional
-
-    def get_value(self, struct):
-        if self.optional:
-            return getattr(struct, self.struct_name, None)
-        else:
-            return getattr(struct, self.struct_name)
+def guess_filename(filename):
+    """Guess filename"""
+    if osp.isfile(filename):
+        return filename
+    if not filename.endswith(".py"):
+        filename += ".py"
+    for path in [getcwd_or_home()] + sys.path:
+        fname = osp.join(path, filename)
+        if osp.isfile(fname):
+            return fname
+        elif osp.isfile(fname + ".py"):
+            return fname + ".py"
+        elif osp.isfile(fname + ".pyw"):
+            return fname + ".pyw"
+    return filename
 
-    def set_value(self, struct, value):
-        setattr(struct, self.struct_name, value)
 
-    def save(self, group, struct):
-        value = self.get_value(struct)
-        if self.optional and value is None:
-            # print ".-", self.hdf_name, value
-            if self.hdf_name in group.attrs:
-                del group.attrs[self.hdf_name]
-            return
-        if self.type is not None:
-            value = self.type.to_hdf(value)
-        # print ".", self.hdf_name, value, self.optional
-        try:
-            group.attrs[self.hdf_name] = value
-        except:
-            print("ERROR saving:", repr(value), "into", self.hdf_name, file=sys.stderr)
-            raise
+class Interpreter(InteractiveConsole, threading.Thread):
+    """Interpreter, executed in a separate thread"""
 
-    def load(self, group, struct):
-        # print "LoadAttr:", group, self.hdf_name
-        if self.optional:
-            if self.hdf_name not in group.attrs:
-                self.set_value(struct, None)
-                return
-        try:
-            value = group.attrs[self.hdf_name]
-        except KeyError:
-            raise KeyError("Unable to locate attribute %s" % self.hdf_name)
-        if self.type is not None:
-            value = self.type.from_hdf(value)
-        self.set_value(struct, value)
-
-
-def createdset(group, name, value):
-    group.create_dataset(
-        name,
-        compression=None,
-        # compression_opts=3,
-        data=value,
-    )
-
-
-class Dset(Attr):
-    """
-    Generic load/save for an hdf5 dataset:
-    scalar=float -> used to convert the value when it is scalar
-    """
+    p1 = ">>> "
+    p2 = "... "
 
     def __init__(
-        self, hdf_name, struct_name=None, type=None, scalar=None, optional=False
+        self, namespace=None, exitfunc=None, Output=None, WidgetProxy=None, debug=False
     ):
-        Attr.__init__(self, hdf_name, struct_name, type, optional)
-        self.scalar = scalar
-
-    def save(self, group, struct):
-        value = self.get_value(struct)
-        if isinstance(value, float):
-            value = np.float64(value)
-        elif isinstance(value, int):
-            value = np.int32(value)
-        if value is None or value.size == 0:
-            value = np.array([0.0])
-        if value.shape == ():
-            value = value.reshape((1,))
-        group.require_dataset(
-            self.hdf_name,
-            shape=value.shape,
-            dtype=value.dtype,
-            data=value,
-            compression="gzip",
-            compression_opts=1,
-        )
-
-    def load(self, group, struct):
-        if self.optional:
-            if self.hdf_name not in group:
-                self.set_value(struct, None)
-                return
-        try:
-            value = group[self.hdf_name][...]
-        except KeyError:
-            raise KeyError("Unable to locate dataset %s" % self.hdf_name)
-        if self.scalar is not None:
-            value = self.scalar(value)
-        self.set_value(struct, value)
-
-
-class Dlist(Dset):
-    def get_value(self, struct):
-        return np.array(getattr(struct, self.struct_name))
-
-    def set_value(self, struct, value):
-        setattr(struct, self.struct_name, list(value))
-
-
-# ==============================================================================
-# Base HDF5 Store object: do not break API compatibility here as this class is
-# used in various critical projects for saving/loading application data
-# ==============================================================================
-class H5Store(object):
-    def __init__(self, filename):
-        self.filename = filename
-        self.h5 = None
-
-    def open(self, mode="a"):
-        """Open an hdf5 file"""
-        if self.h5:
-            return self.h5
-        try:
-            self.h5 = h5py.File(self.filename, mode=mode)
-        except Exception:
-            print(
-                "Error trying to load:",
-                self.filename,
-                "in mode:",
-                mode,
-                file=sys.stderr,
-            )
-            raise
-        return self.h5
-
-    def close(self):
-        if self.h5:
-            self.h5.close()
-        self.h5 = None
-
-    def generic_save(self, parent, source, structure):
-        """save the data from source into the file using 'structure'
-        as a descriptor.
-
-        structure is a list of Attribute Descriptor (Attr, Dset, Dlist or anything
-        with a save interface) that describe the conversion of data and the name
-        of the attribute in the source and in the file
         """
-        for instr in structure:
-            instr.save(parent, source)
-
-    def generic_load(self, parent, dest, structure):
-        """load the data from the file into dest using 'structure'
-        as a descriptor.
-
-        structure is the same as in generic_save
+        namespace: locals send to InteractiveConsole object
+        commands: list of commands executed at startup
         """
-        for instr in structure:
-            try:
-                instr.load(parent, dest)
-            except Exception:
-                print("Error loading HDF5 item:", instr.hdf_name, file=sys.stderr)
-                raise
-
-
-# ==============================================================================
-# HDF5 reader/writer: do not break API compatibility here as this class is
-# used in various critical projects for saving/loading application data and
-# in guiqwt for saving/loading plot items.
-# ==============================================================================
-class HDF5Handler(H5Store, BaseIOHandler):
-    """Base HDF5 I/O Handler object"""
+        InteractiveConsole.__init__(self, namespace)
+        threading.Thread.__init__(self)
 
-    def __init__(self, filename):
-        H5Store.__init__(self, filename)
-        self.option = []
+        self._id = None
 
-    def get_parent_group(self):
-        parent = self.h5
-        for option in self.option[:-1]:
-            parent = parent.require_group(option)
-        return parent
+        self.exit_flag = False
+        self.debug = debug
 
+        # Execution Status
+        self.more = False
+
+        if exitfunc is not None:
+            atexit.register(exitfunc)
+
+        self.namespace = self.locals
+        self.namespace["__name__"] = "__main__"
+        self.namespace["execfile"] = self.execfile
+        self.namespace["runfile"] = self.runfile
+        self.namespace["raw_input"] = self.raw_input_replacement
+        self.namespace["help"] = self.help_replacement
+
+        # Capture all interactive input/output
+        self.initial_stdout = sys.stdout
+        self.initial_stderr = sys.stderr
+        self.initial_stdin = sys.stdin
+
+        # Create communication pipes
+        pr, pw = os.pipe()
+        self.stdin_read = os.fdopen(pr, "r")
+        self.stdin_write = os.fdopen(pw, "wb", 0)
+        self.stdout_write = Output()
+        self.stderr_write = Output()
+
+        self.input_condition = threading.Condition()
+        self.widget_proxy = WidgetProxy(self.input_condition)
+
+        self.redirect_stds()
+
+    # ------ Standard input/output
+    def redirect_stds(self):
+        """Redirects stds"""
+        if not self.debug:
+            sys.stdout = self.stdout_write
+            sys.stderr = self.stderr_write
+            sys.stdin = self.stdin_read
+
+    def restore_stds(self):
+        """Restore stds"""
+        if not self.debug:
+            sys.stdout = self.initial_stdout
+            sys.stderr = self.initial_stderr
+            sys.stdin = self.initial_stdin
+
+    def raw_input_replacement(self, prompt=""):
+        """For raw_input builtin function emulation"""
+        self.widget_proxy.wait_input(prompt)
+        self.input_condition.acquire()
+        while not self.widget_proxy.data_available():
+            self.input_condition.wait()
+        inp = self.widget_proxy.input_data
+        self.input_condition.release()
+        return inp
+
+    def help_replacement(self, text=None, interactive=False):
+        """For help builtin function emulation"""
+        if text is not None and not interactive:
+            return pydoc.help(text)
+        elif text is None:
+            pyver = "%d.%d" % (sys.version_info[0], sys.version_info[1])
+            self.write(
+                """
+Welcome to Python %s!  This is the online help utility.
+
+If this is your first time using Python, you should definitely check out
+the tutorial on the Internet at https://www.python.org/about/gettingstarted/
+
+Enter the name of any module, keyword, or topic to get help on writing
+Python programs and using Python modules.  To quit this help utility and
+return to the interpreter, just type "quit".
+
+To get a list of available modules, keywords, or topics, type "modules",
+"keywords", or "topics".  Each module also comes with a one-line summary
+of what it does; to list the modules whose summaries contain a given word
+such as "spam", type "modules spam".
+"""
+                % pyver
+            )
+        else:
+            text = text.strip()
+            try:
+                eval("pydoc.help(%s)" % text)
+            except (NameError, SyntaxError):
+                print(
+                    "no Python documentation found for '%r'" % text
+                )  # spyder: test-skip
+        self.write(os.linesep)
+        self.widget_proxy.new_prompt("help> ")
+        inp = self.raw_input_replacement()
+        if inp.strip():
+            self.help_replacement(inp, interactive=True)
+        else:
+            self.write(
+                """
+You are now leaving help and returning to the Python interpreter.
+If you want to ask for help on a particular object directly from the
+interpreter, you can type "help(object)".  Executing "help('string')"
+has the same effect as typing a particular string at the help> prompt.
+"""
+            )
 
-class HDF5Writer(HDF5Handler, WriterMixin):
-    """Writer for HDF5 files"""
-
-    def __init__(self, filename):
-        super(HDF5Writer, self).__init__(filename)
-        self.open("w")
-
-    def write_any(self, val):
-        group = self.get_parent_group()
-        group.attrs[self.option[-1]] = val
+    def run_command(self, cmd, new_prompt=True):
+        """Run command in interpreter"""
+        if cmd == "exit()":
+            self.exit_flag = True
+            self.write("\n")
+            return
+        # -- Special commands type I
+        #    (transformed into commands executed in the interpreter)
+        # ? command
+        special_pattern = r"^%s (?:r\')?(?:u\')?\"?\'?([a-zA-Z0-9_\.]+)"
+        run_match = re.match(special_pattern % "run", cmd)
+        help_match = re.match(r"^([a-zA-Z0-9_\.]+)\?$", cmd)
+        cd_match = re.match(r"^\!cd \"?\'?([a-zA-Z0-9_ \.]+)", cmd)
+        if help_match:
+            cmd = "help(%s)" % help_match.group(1)
+        # run command
+        elif run_match:
+            filename = guess_filename(run_match.groups()[0])
+            cmd = "runfile('%s', args=None)" % remove_backslashes(filename)
+        # !cd system command
+        elif cd_match:
+            cmd = 'import os; os.chdir(r"%s")' % cd_match.groups()[0].strip()
+        # -- End of Special commands type I
+
+        # -- Special commands type II
+        #    (don't need code execution in interpreter)
+        xedit_match = re.match(special_pattern % "xedit", cmd)
+        edit_match = re.match(special_pattern % "edit", cmd)
+        clear_match = re.match(r"^clear ([a-zA-Z0-9_, ]+)", cmd)
+        # (external) edit command
+        if xedit_match:
+            filename = guess_filename(xedit_match.groups()[0])
+            self.widget_proxy.edit(filename, external_editor=True)
+        # local edit command
+        elif edit_match:
+            filename = guess_filename(edit_match.groups()[0])
+            if osp.isfile(filename):
+                self.widget_proxy.edit(filename)
+            else:
+                self.stderr_write.write("No such file or directory: %s\n" % filename)
+        # remove reference (equivalent to MATLAB's clear command)
+        elif clear_match:
+            varnames = clear_match.groups()[0].replace(" ", "").split(",")
+            for varname in varnames:
+                try:
+                    self.namespace.pop(varname)
+                except KeyError:
+                    pass
+        # Execute command
+        elif cmd.startswith("!"):
+            # System ! command
+            pipe = run_shell_command(cmd[1:])
+            out = pipe.stdout.read()
+            err = pipe.stderr.read()
+            try:
+                out = out.decode("cp437")
+            except UnicodeDecodeError:
+                out = out.decode(erros="ignore")
+            try:
+                err = err.decode("cp437")
+            except UnicodeDecodeError:
+                err = err.decode(erros="ignore")
+            if err:
+                self.stderr_write.write(err)
+            if out:
+                self.stdout_write.write(out)
+            self.stdout_write.write("\n")
+            self.more = False
+        # -- End of Special commands type II
+        else:
+            # Command executed in the interpreter
+            #            self.widget_proxy.set_readonly(True)
+            self.more = self.push(cmd)
+        #            self.widget_proxy.set_readonly(False)
+
+        if new_prompt:
+            self.widget_proxy.new_prompt(self.p2 if self.more else self.p1)
+        if not self.more:
+            self.resetbuffer()
+
+    def run(self):
+        """Wait for input and run it"""
+        while not self.exit_flag:
+            self.run_line()
 
-    write_int = write_float = write_any
+    def run_line(self):
+        """
 
-    def write_bool(self, val):
-        self.write_int(int(val))
+        :return:
+        """
+        line = self.stdin_read.readline()
+        if self.exit_flag:
+            return
+        # Remove last character which is always '\n':
+        self.run_command(line[:-1])
 
-    write_str = write_any
+    def get_thread_id(self):
+        """Return thread id"""
+        if self._id is None:
+            for thread_id, obj in list(threading._active.items()):
+                if obj is self:
+                    self._id = thread_id
+        return self._id
 
-    def write_unicode(self, val):
-        group = self.get_parent_group()
-        group.attrs[self.option[-1]] = val.encode("utf-8")
+    def raise_keyboard_interrupt(self):
+        """
 
-    write_unicode = write_str
+        :return:
+        """
+        if self.isAlive():
+            ctypes.pythonapi.PyThreadState_SetAsyncExc(
+                self.get_thread_id(), ctypes.py_object(KeyboardInterrupt)
+            )
+            return True
+        else:
+            return False
 
-    def write_array(self, val):
-        group = self.get_parent_group()
-        group[self.option[-1]] = val
+    def closing(self):
+        """Actions to be done before restarting this interpreter"""
+        pass
+
+    def execfile(self, filename):
+        """Exec filename"""
+        source = open(filename, "r").read()
+        try:
+            try:
+                name = filename.encode("ascii")
+            except UnicodeEncodeError:
+                name = "<executed_script>"
+            code = compile(source, name, "exec")
+        except (OverflowError, SyntaxError):
+            InteractiveConsole.showsyntaxerror(self, filename)
+        else:
+            self.runcode(code)
 
-    write_sequence = write_any
+    def runfile(self, filename, args=None):
+        """
+        Run filename
+        args: command line arguments (string)
+        """
+        if args is not None and not isinstance(args, str):
+            raise TypeError("expected a character buffer object")
+        self.namespace["__file__"] = filename
+        sys.argv = [filename]
+        if args is not None:
+            for arg in args.split():
+                sys.argv.append(arg)
+        self.execfile(filename)
+        sys.argv = [""]
+        self.namespace.pop("__file__")
 
-    def write_none(self):
-        group = self.get_parent_group()
-        group.attrs[self.option[-1]] = ""
+    def eval(self, text):
+        """
+        Evaluate text and return (obj, valid)
+        where *obj* is the object represented by *text*
+        and *valid* is True if object evaluation did not raise any exception
+        """
+        assert isinstance(text, str)
+        try:
+            return eval(text, self.locals), True
+        except:
+            return None, False
 
-    def write_object_list(self, seq, group_name):
-        """Write object sequence in group.
-        Objects must implement the DataSet-like `serialize` method"""
-        with self.group(group_name):
-            if seq is None:
-                self.write_none()
-            else:
-                ids = []
-                for obj in seq:
-                    guid = bytes(str(uuid1()), "utf-8")
-                    ids.append(guid)
-                    with self.group(guid):
-                        if obj is None:
-                            self.write_none()
-                        else:
-                            obj.serialize(self)
-                self.write(ids, "IDs")
-
-
-class HDF5Reader(HDF5Handler):
-    """Reader for HDF5 files"""
-
-    def __init__(self, filename):
-        super(HDF5Reader, self).__init__(filename)
-        self.open("r")
-
-    def read(self, group_name=None, func=None, instance=None):
-        """Read value within current group or group_name.
-
-        Optional argument `instance` is an object which
-        implements the DataSet-like `deserialize` method."""
-        if group_name:
-            self.begin(group_name)
-        if instance is None:
-            if func is None:
-                func = self.read_any
-            val = func()
-        else:
-            group = self.get_parent_group()
-            if group_name in group.attrs:
-                # This is an attribute (not a group), meaning that
-                # the object was None when deserializing it
-                val = None
-            else:
-                instance.deserialize(self)
-                val = instance
-        if group_name:
-            self.end(group_name)
-        return val
-
-    def read_any(self):
-        group = self.get_parent_group()
-        value = group.attrs[self.option[-1]]
-        if isinstance(value, bytes):
-            return value.decode("utf-8")
-        else:
-            return value
+    def is_defined(self, objtxt, force_import=False):
+        """Return True if object is defined"""
+        return isdefined(objtxt, force_import=force_import, namespace=self.locals)
+
+    # ===========================================================================
+    # InteractiveConsole API
+    # ===========================================================================
+    def push(self, line):
+        """
+        Push a line of source text to the interpreter
 
-    def read_bool(self):
-        val = self.read_any()
-        if val != "":
-            return bool(val)
-
-    def read_int(self):
-        val = self.read_any()
-        if val != "":
-            return int(val)
-
-    def read_float(self):
-        val = self.read_any()
-        if val != "":
-            return float(val)
-
-    read_unicode = read_str = read_any
-
-    def read_array(self):
-        group = self.get_parent_group()
-        return group[self.option[-1]][...]
-
-    def read_sequence(self):
-        group = self.get_parent_group()
-        return list(group.attrs[self.option[-1]])
-
-    def read_object_list(self, group_name, klass, progress_callback=None):
-        """Read object sequence in group.
-        Objects must implement the DataSet-like `deserialize` method.
-        `klass` is the object class which constructor requires no argument.
-
-        progress_callback: if not None, this function is called with
-        an integer argument (progress: 0 --> 100). Function returns the
-        `cancel` state (True: progress dialog has been canceled, False
-        otherwise)
+        The line should not have a trailing newline; it may have internal
+        newlines. The line is appended to a buffer and the interpreter’s
+        runsource() method is called with the concatenated contents of the
+        buffer as source. If this indicates that the command was executed
+        or invalid, the buffer is reset; otherwise, the command is incomplete,
+        and the buffer is left as it was after the line was appended.
+        The return value is True if more input is required, False if the line
+        was dealt with in some way (this is the same as runsource()).
         """
-        with self.group(group_name):
-            try:
-                ids = self.read("IDs", func=self.read_sequence)
-            except ValueError:
-                # None was saved instead of list of objects
-                self.end("IDs")
-                return
-            seq = []
-            count = len(ids)
-            for idx, name in enumerate(ids):
-                if progress_callback is not None:
-                    if progress_callback(int(100 * float(idx) / count)):
-                        break
-                with self.group(name):
-                    group = self.get_parent_group()
-                    if name in group.attrs:
-                        # This is an attribute (not a group), meaning that
-                        # the object was None when deserializing it
-                        obj = None
-                    else:
-                        obj = klass()
-                        obj.deserialize(self)
-                seq.append(obj)
-        return seq
+        return InteractiveConsole.push(self, "#coding=utf-8\n" + line)
 
-    read_none = read_any
+    def resetbuffer(self):
+        """Remove any unhandled source text from the input buffer"""
+        InteractiveConsole.resetbuffer(self)
```

### Comparing `guidata-2.3.1/guidata/images/apply.png` & `guidata-3.0.0/guidata/images/apply.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/arredit.png` & `guidata-3.0.0/guidata/images/arredit.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/busy.png` & `guidata-3.0.0/guidata/images/busy.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/cell_edit.png` & `guidata-3.0.0/guidata/images/cell_edit.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/copy.png` & `guidata-3.0.0/guidata/images/copy.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/delete.png` & `guidata-3.0.0/guidata/images/delete.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/dictedit.png` & `guidata-3.0.0/guidata/images/dictedit.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/dtype.png` & `guidata-3.0.0/guidata/images/dtype.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/edit.png` & `guidata-3.0.0/guidata/images/edit.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/editors/copywop.png` & `guidata-3.0.0/guidata/images/editors/copywop.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/editors/edit.png` & `guidata-3.0.0/guidata/images/editors/edit.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/editors/edit_add.png` & `guidata-3.0.0/guidata/images/editors/edit_add.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/editors/editclear.png` & `guidata-3.0.0/guidata/images/editors/editclear.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/editors/editcopy.png` & `guidata-3.0.0/guidata/images/editors/editcopy.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/editors/editcut.png` & `guidata-3.0.0/guidata/images/editors/editcut.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/editors/editdelete.png` & `guidata-3.0.0/guidata/images/editors/editdelete.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/editors/editpaste.png` & `guidata-3.0.0/guidata/images/editors/editpaste.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/editors/fileimport.png` & `guidata-3.0.0/guidata/images/editors/fileimport.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/editors/filesave.png` & `guidata-3.0.0/guidata/images/editors/filesave.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/editors/imshow.png` & `guidata-3.0.0/guidata/images/editors/imshow.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/editors/insert.png` & `guidata-3.0.0/guidata/images/editors/insert.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/editors/plot.png` & `guidata-3.0.0/guidata/images/editors/plot.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/editors/rename.png` & `guidata-3.0.0/guidata/images/editors/rename.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/editors/selectall.png` & `guidata-3.0.0/guidata/images/editors/selectall.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/exit.png` & `guidata-3.0.0/guidata/images/exit.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/file.png` & `guidata-3.0.0/guidata/images/file.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/fileclose.png` & `guidata-3.0.0/guidata/images/fileclose.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/fileimport.png` & `guidata-3.0.0/guidata/images/fileimport.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/fileopen.png` & `guidata-3.0.0/guidata/images/fileopen.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/filesave.png` & `guidata-3.0.0/guidata/images/filesave.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/filesaveas.png` & `guidata-3.0.0/guidata/images/filesaveas.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/filetypes/doc.png` & `guidata-3.0.0/guidata/images/filetypes/doc.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/filetypes/gif.png` & `guidata-3.0.0/guidata/images/filetypes/gif.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/filetypes/html.png` & `guidata-3.0.0/guidata/images/filetypes/html.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/filetypes/jpg.png` & `guidata-3.0.0/guidata/images/filetypes/jpg.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/filetypes/pdf.png` & `guidata-3.0.0/guidata/images/filetypes/pdf.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/filetypes/png.png` & `guidata-3.0.0/guidata/images/filetypes/png.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/filetypes/pps.png` & `guidata-3.0.0/guidata/images/filetypes/pps.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/filetypes/ps.png` & `guidata-3.0.0/guidata/images/filetypes/ps.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/filetypes/tar.png` & `guidata-3.0.0/guidata/images/filetypes/tar.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/filetypes/tgz.png` & `guidata-3.0.0/guidata/images/filetypes/tgz.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/filetypes/tif.png` & `guidata-3.0.0/guidata/images/filetypes/tif.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/filetypes/txt.png` & `guidata-3.0.0/guidata/images/filetypes/txt.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/filetypes/xls.png` & `guidata-3.0.0/guidata/images/filetypes/xls.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/filetypes/zip.png` & `guidata-3.0.0/guidata/images/filetypes/zip.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/guidata.svg` & `guidata-3.0.0/guidata/images/guidata-vertical.svg`

 * *Files 23% similar despite different names*

```diff
@@ -1,1209 +1,1026 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
 00000020: 462d 3822 2073 7461 6e64 616c 6f6e 653d  F-8" standalone=
-00000030: 226e 6f22 3f3e 0d0a 3c21 2d2d 2043 7265  "no"?>..<!-- Cre
-00000040: 6174 6564 2077 6974 6820 496e 6b73 6361  ated with Inksca
-00000050: 7065 2028 6874 7470 3a2f 2f77 7777 2e69  pe (http://www.i
-00000060: 6e6b 7363 6170 652e 6f72 672f 2920 2d2d  nkscape.org/) --
-00000070: 3e0d 0a0d 0a3c 7376 670d 0a20 2020 786d  >....<svg..   xm
-00000080: 6c6e 733a 6f73 623d 2268 7474 703a 2f2f  lns:osb="http://
-00000090: 7777 772e 6f70 656e 7377 6174 6368 626f  www.openswatchbo
-000000a0: 6f6b 2e6f 7267 2f75 7269 2f32 3030 392f  ok.org/uri/2009/
-000000b0: 6f73 6222 0d0a 2020 2078 6d6c 6e73 3a64  osb"..   xmlns:d
-000000c0: 633d 2268 7474 703a 2f2f 7075 726c 2e6f  c="http://purl.o
-000000d0: 7267 2f64 632f 656c 656d 656e 7473 2f31  rg/dc/elements/1
-000000e0: 2e31 2f22 0d0a 2020 2078 6d6c 6e73 3a63  .1/"..   xmlns:c
-000000f0: 633d 2268 7474 703a 2f2f 6372 6561 7469  c="http://creati
-00000100: 7665 636f 6d6d 6f6e 732e 6f72 672f 6e73  vecommons.org/ns
-00000110: 2322 0d0a 2020 2078 6d6c 6e73 3a72 6466  #"..   xmlns:rdf
-00000120: 3d22 6874 7470 3a2f 2f77 7777 2e77 332e  ="http://www.w3.
-00000130: 6f72 672f 3139 3939 2f30 322f 3232 2d72  org/1999/02/22-r
-00000140: 6466 2d73 796e 7461 782d 6e73 2322 0d0a  df-syntax-ns#"..
-00000150: 2020 2078 6d6c 6e73 3a73 7667 3d22 6874     xmlns:svg="ht
-00000160: 7470 3a2f 2f77 7777 2e77 332e 6f72 672f  tp://www.w3.org/
-00000170: 3230 3030 2f73 7667 220d 0a20 2020 786d  2000/svg"..   xm
-00000180: 6c6e 733d 2268 7474 703a 2f2f 7777 772e  lns="http://www.
-00000190: 7733 2e6f 7267 2f32 3030 302f 7376 6722  w3.org/2000/svg"
-000001a0: 0d0a 2020 2078 6d6c 6e73 3a78 6c69 6e6b  ..   xmlns:xlink
-000001b0: 3d22 6874 7470 3a2f 2f77 7777 2e77 332e  ="http://www.w3.
-000001c0: 6f72 672f 3139 3939 2f78 6c69 6e6b 220d  org/1999/xlink".
-000001d0: 0a20 2020 786d 6c6e 733a 736f 6469 706f  .   xmlns:sodipo
-000001e0: 6469 3d22 6874 7470 3a2f 2f73 6f64 6970  di="http://sodip
-000001f0: 6f64 692e 736f 7572 6365 666f 7267 652e  odi.sourceforge.
-00000200: 6e65 742f 4454 442f 736f 6469 706f 6469  net/DTD/sodipodi
-00000210: 2d30 2e64 7464 220d 0a20 2020 786d 6c6e  -0.dtd"..   xmln
-00000220: 733a 696e 6b73 6361 7065 3d22 6874 7470  s:inkscape="http
-00000230: 3a2f 2f77 7777 2e69 6e6b 7363 6170 652e  ://www.inkscape.
-00000240: 6f72 672f 6e61 6d65 7370 6163 6573 2f69  org/namespaces/i
-00000250: 6e6b 7363 6170 6522 0d0a 2020 2076 6572  nkscape"..   ver
-00000260: 7369 6f6e 3d22 312e 3022 0d0a 2020 2077  sion="1.0"..   w
-00000270: 6964 7468 3d22 3135 332e 3536 3538 3322  idth="153.56583"
-00000280: 0d0a 2020 2068 6569 6768 743d 2231 3533  ..   height="153
-00000290: 2e35 3635 3833 220d 0a20 2020 6964 3d22  .56583"..   id="
-000002a0: 7376 6732 220d 0a20 2020 736f 6469 706f  svg2"..   sodipo
-000002b0: 6469 3a76 6572 7369 6f6e 3d22 302e 3332  di:version="0.32
-000002c0: 220d 0a20 2020 696e 6b73 6361 7065 3a76  "..   inkscape:v
-000002d0: 6572 7369 6f6e 3d22 302e 3438 2e32 2072  ersion="0.48.2 r
-000002e0: 3938 3139 220d 0a20 2020 736f 6469 706f  9819"..   sodipo
-000002f0: 6469 3a64 6f63 6e61 6d65 3d22 6775 6964  di:docname="guid
-00000300: 6174 612e 7376 6722 0d0a 2020 2069 6e6b  ata.svg"..   ink
-00000310: 7363 6170 653a 6f75 7470 7574 5f65 7874  scape:output_ext
-00000320: 656e 7369 6f6e 3d22 6f72 672e 696e 6b73  ension="org.inks
-00000330: 6361 7065 2e6f 7574 7075 742e 7376 672e  cape.output.svg.
-00000340: 696e 6b73 6361 7065 220d 0a20 2020 696e  inkscape"..   in
-00000350: 6b73 6361 7065 3a65 7870 6f72 742d 6669  kscape:export-fi
-00000360: 6c65 6e61 6d65 3d22 443a 5c31 3238 2e70  lename="D:\128.p
-00000370: 6e67 220d 0a20 2020 696e 6b73 6361 7065  ng"..   inkscape
-00000380: 3a65 7870 6f72 742d 7864 7069 3d22 3238  :export-xdpi="28
-00000390: 2e30 3931 3835 3222 0d0a 2020 2069 6e6b  .091852"..   ink
-000003a0: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
-000003b0: 693d 2232 382e 3039 3138 3532 223e 0d0a  i="28.091852">..
-000003c0: 2020 3c6d 6574 6164 6174 610d 0a20 2020    <metadata..   
-000003d0: 2020 6964 3d22 6d65 7461 6461 7461 3231    id="metadata21
-000003e0: 3933 223e 0d0a 2020 2020 3c72 6466 3a52  93">..    <rdf:R
-000003f0: 4446 3e0d 0a20 2020 2020 203c 6363 3a57  DF>..      <cc:W
-00000400: 6f72 6b0d 0a20 2020 2020 2020 2020 7264  ork..         rd
-00000410: 663a 6162 6f75 743d 2222 3e0d 0a20 2020  f:about="">..   
-00000420: 2020 2020 203c 6463 3a66 6f72 6d61 743e       <dc:format>
-00000430: 696d 6167 652f 7376 672b 786d 6c3c 2f64  image/svg+xml</d
-00000440: 633a 666f 726d 6174 3e0d 0a20 2020 2020  c:format>..     
-00000450: 2020 203c 6463 3a74 7970 650d 0a20 2020     <dc:type..   
-00000460: 2020 2020 2020 2020 7264 663a 7265 736f          rdf:reso
-00000470: 7572 6365 3d22 6874 7470 3a2f 2f70 7572  urce="http://pur
-00000480: 6c2e 6f72 672f 6463 2f64 636d 6974 7970  l.org/dc/dcmityp
-00000490: 652f 5374 696c 6c49 6d61 6765 2220 2f3e  e/StillImage" />
-000004a0: 0d0a 2020 2020 2020 2020 3c64 633a 7469  ..        <dc:ti
-000004b0: 746c 653e 3c2f 6463 3a74 6974 6c65 3e0d  tle></dc:title>.
-000004c0: 0a20 2020 2020 203c 2f63 633a 576f 726b  .      </cc:Work
-000004d0: 3e0d 0a20 2020 203c 2f72 6466 3a52 4446  >..    </rdf:RDF
-000004e0: 3e0d 0a20 203c 2f6d 6574 6164 6174 613e  >..  </metadata>
-000004f0: 0d0a 2020 3c73 6f64 6970 6f64 693a 6e61  ..  <sodipodi:na
-00000500: 6d65 6476 6965 770d 0a20 2020 2020 696e  medview..     in
-00000510: 6b73 6361 7065 3a77 696e 646f 772d 6865  kscape:window-he
-00000520: 6967 6874 3d22 3734 3422 0d0a 2020 2020  ight="744"..    
-00000530: 2069 6e6b 7363 6170 653a 7769 6e64 6f77   inkscape:window
-00000540: 2d77 6964 7468 3d22 3132 3830 220d 0a20  -width="1280".. 
-00000550: 2020 2020 696e 6b73 6361 7065 3a70 6167      inkscape:pag
-00000560: 6573 6861 646f 773d 2232 220d 0a20 2020  eshadow="2"..   
-00000570: 2020 696e 6b73 6361 7065 3a70 6167 656f    inkscape:pageo
-00000580: 7061 6369 7479 3d22 302e 3022 0d0a 2020  pacity="0.0"..  
-00000590: 2020 2062 6f72 6465 726f 7061 6369 7479     borderopacity
-000005a0: 3d22 312e 3022 0d0a 2020 2020 2062 6f72  ="1.0"..     bor
-000005b0: 6465 7263 6f6c 6f72 3d22 2336 3636 3636  dercolor="#66666
-000005c0: 3622 0d0a 2020 2020 2070 6167 6563 6f6c  6"..     pagecol
-000005d0: 6f72 3d22 2366 6666 6666 6622 0d0a 2020  or="#ffffff"..  
-000005e0: 2020 2069 643d 2262 6173 6522 0d0a 2020     id="base"..  
-000005f0: 2020 2069 6e6b 7363 6170 653a 7a6f 6f6d     inkscape:zoom
-00000600: 3d22 312e 3835 3238 3038 3722 0d0a 2020  ="1.8528087"..  
-00000610: 2020 2069 6e6b 7363 6170 653a 6378 3d22     inkscape:cx="
-00000620: 2d31 342e 3033 3139 3734 220d 0a20 2020  -14.031974"..   
-00000630: 2020 696e 6b73 6361 7065 3a63 793d 2236    inkscape:cy="6
-00000640: 322e 3734 3833 3036 220d 0a20 2020 2020  2.748306"..     
-00000650: 696e 6b73 6361 7065 3a77 696e 646f 772d  inkscape:window-
-00000660: 783d 2232 3422 0d0a 2020 2020 2069 6e6b  x="24"..     ink
-00000670: 7363 6170 653a 7769 6e64 6f77 2d79 3d22  scape:window-y="
-00000680: 3931 220d 0a20 2020 2020 696e 6b73 6361  91"..     inksca
-00000690: 7065 3a63 7572 7265 6e74 2d6c 6179 6572  pe:current-layer
-000006a0: 3d22 7376 6732 220d 0a20 2020 2020 7368  ="svg2"..     sh
-000006b0: 6f77 6772 6964 3d22 6661 6c73 6522 0d0a  owgrid="false"..
-000006c0: 2020 2020 2066 6974 2d6d 6172 6769 6e2d       fit-margin-
-000006d0: 746f 703d 2230 220d 0a20 2020 2020 6669  top="0"..     fi
-000006e0: 742d 6d61 7267 696e 2d6c 6566 743d 2230  t-margin-left="0
-000006f0: 220d 0a20 2020 2020 6669 742d 6d61 7267  "..     fit-marg
-00000700: 696e 2d72 6967 6874 3d22 3022 0d0a 2020  in-right="0"..  
-00000710: 2020 2066 6974 2d6d 6172 6769 6e2d 626f     fit-margin-bo
-00000720: 7474 6f6d 3d22 3022 0d0a 2020 2020 2069  ttom="0"..     i
-00000730: 6e6b 7363 6170 653a 7769 6e64 6f77 2d6d  nkscape:window-m
-00000740: 6178 696d 697a 6564 3d22 3022 202f 3e0d  aximized="0" />.
-00000750: 0a20 203c 6465 6673 0d0a 2020 2020 2069  .  <defs..     i
-00000760: 643d 2264 6566 7334 223e 0d0a 2020 2020  d="defs4">..    
-00000770: 3c6c 696e 6561 7247 7261 6469 656e 740d  <linearGradient.
-00000780: 0a20 2020 2020 2020 6964 3d22 6c69 6e65  .       id="line
-00000790: 6172 4772 6164 6965 6e74 3739 3332 220d  arGradient7932".
-000007a0: 0a20 2020 2020 2020 6f73 623a 7061 696e  .       osb:pain
-000007b0: 743d 2273 6f6c 6964 223e 0d0a 2020 2020  t="solid">..    
-000007c0: 2020 3c73 746f 700d 0a20 2020 2020 2020    <stop..       
-000007d0: 2020 7374 796c 653d 2273 746f 702d 636f    style="stop-co
-000007e0: 6c6f 723a 2361 3061 3061 303b 7374 6f70  lor:#a0a0a0;stop
-000007f0: 2d6f 7061 6369 7479 3a31 3b22 0d0a 2020  -opacity:1;"..  
-00000800: 2020 2020 2020 206f 6666 7365 743d 2230         offset="0
-00000810: 220d 0a20 2020 2020 2020 2020 6964 3d22  "..         id="
-00000820: 7374 6f70 3739 3334 2220 2f3e 0d0a 2020  stop7934" />..  
-00000830: 2020 3c2f 6c69 6e65 6172 4772 6164 6965    </linearGradie
-00000840: 6e74 3e0d 0a20 2020 203c 6c69 6e65 6172  nt>..    <linear
-00000850: 4772 6164 6965 6e74 0d0a 2020 2020 2020  Gradient..      
-00000860: 2069 643d 226c 696e 6561 7247 7261 6469   id="linearGradi
-00000870: 656e 7436 3438 3122 3e0d 0a20 2020 2020  ent6481">..     
-00000880: 203c 7374 6f70 0d0a 2020 2020 2020 2020   <stop..        
-00000890: 2069 643d 2273 746f 7036 3438 3322 0d0a   id="stop6483"..
-000008a0: 2020 2020 2020 2020 206f 6666 7365 743d           offset=
-000008b0: 2230 220d 0a20 2020 2020 2020 2020 7374  "0"..         st
-000008c0: 796c 653d 2273 746f 702d 636f 6c6f 723a  yle="stop-color:
-000008d0: 2335 6139 6664 343b 7374 6f70 2d6f 7061  #5a9fd4;stop-opa
-000008e0: 6369 7479 3a31 2220 2f3e 0d0a 2020 2020  city:1" />..    
-000008f0: 2020 3c73 746f 700d 0a20 2020 2020 2020    <stop..       
-00000900: 2020 6964 3d22 7374 6f70 3634 3835 220d    id="stop6485".
-00000910: 0a20 2020 2020 2020 2020 6f66 6673 6574  .         offset
-00000920: 3d22 3122 0d0a 2020 2020 2020 2020 2073  ="1"..         s
-00000930: 7479 6c65 3d22 7374 6f70 2d63 6f6c 6f72  tyle="stop-color
-00000940: 3a23 3330 3639 3938 3b73 746f 702d 6f70  :#306998;stop-op
-00000950: 6163 6974 793a 3122 202f 3e0d 0a20 2020  acity:1" />..   
-00000960: 203c 2f6c 696e 6561 7247 7261 6469 656e   </linearGradien
-00000970: 743e 0d0a 2020 2020 3c6d 6172 6b65 720d  t>..    <marker.
-00000980: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-00000990: 3a73 746f 636b 6964 3d22 4172 726f 7732  :stockid="Arrow2
-000009a0: 4d65 6e64 220d 0a20 2020 2020 2020 6f72  Mend"..       or
-000009b0: 6965 6e74 3d22 6175 746f 220d 0a20 2020  ient="auto"..   
-000009c0: 2020 2020 7265 6659 3d22 3022 0d0a 2020      refY="0"..  
-000009d0: 2020 2020 2072 6566 583d 2230 220d 0a20       refX="0".. 
-000009e0: 2020 2020 2020 6964 3d22 4172 726f 7732        id="Arrow2
-000009f0: 4d65 6e64 220d 0a20 2020 2020 2020 7374  Mend"..       st
-00000a00: 796c 653d 226f 7665 7266 6c6f 773a 7669  yle="overflow:vi
-00000a10: 7369 626c 6522 3e0d 0a20 2020 2020 203c  sible">..      <
-00000a20: 7061 7468 0d0a 2020 2020 2020 2020 2069  path..         i
-00000a30: 643d 2270 6174 6833 3930 3822 0d0a 2020  d="path3908"..  
-00000a40: 2020 2020 2020 2073 7479 6c65 3d22 666f         style="fo
-00000a50: 6e74 2d73 697a 653a 3132 7078 3b66 696c  nt-size:12px;fil
-00000a60: 6c2d 7275 6c65 3a65 7665 6e6f 6464 3b73  l-rule:evenodd;s
-00000a70: 7472 6f6b 652d 7769 6474 683a 302e 3632  troke-width:0.62
-00000a80: 353b 7374 726f 6b65 2d6c 696e 656a 6f69  5;stroke-linejoi
-00000a90: 6e3a 726f 756e 6422 0d0a 2020 2020 2020  n:round"..      
-00000aa0: 2020 2064 3d22 4d20 382e 3731 3835 3837     d="M 8.718587
-00000ab0: 382c 342e 3033 3337 3335 3220 2d32 2e32  8,4.0337352 -2.2
-00000ac0: 3037 3238 3935 2c30 2e30 3136 3031 3332  072895,0.0160132
-00000ad0: 3620 382e 3731 3835 3838 342c 2d34 2e30  6 8.7185884,-4.0
-00000ae0: 3031 3730 3738 2063 202d 312e 3734 3534  017078 c -1.7454
-00000af0: 3938 342c 322e 3337 3230 3630 3920 2d31  984,2.3720609 -1
-00000b00: 2e37 3335 3434 3038 2c35 2e36 3137 3435  .7354408,5.61745
-00000b10: 3139 202d 3665 2d37 2c38 2e30 3335 3434  19 -6e-7,8.03544
-00000b20: 3320 7a22 0d0a 2020 2020 2020 2020 2074  3 z"..         t
-00000b30: 7261 6e73 666f 726d 3d22 7363 616c 6528  ransform="scale(
-00000b40: 2d30 2e36 2c2d 302e 3629 220d 0a20 2020  -0.6,-0.6)"..   
-00000b50: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
-00000b60: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
-00000b70: 7265 3d22 3022 202f 3e0d 0a20 2020 203c  re="0" />..    <
-00000b80: 2f6d 6172 6b65 723e 0d0a 2020 2020 3c6d  /marker>..    <m
-00000b90: 6172 6b65 720d 0a20 2020 2020 2020 696e  arker..       in
-00000ba0: 6b73 6361 7065 3a73 746f 636b 6964 3d22  kscape:stockid="
-00000bb0: 4172 726f 7731 5365 6e64 220d 0a20 2020  Arrow1Send"..   
-00000bc0: 2020 2020 6f72 6965 6e74 3d22 6175 746f      orient="auto
-00000bd0: 220d 0a20 2020 2020 2020 7265 6659 3d22  "..       refY="
-00000be0: 3022 0d0a 2020 2020 2020 2072 6566 583d  0"..       refX=
-00000bf0: 2230 220d 0a20 2020 2020 2020 6964 3d22  "0"..       id="
-00000c00: 4172 726f 7731 5365 6e64 220d 0a20 2020  Arrow1Send"..   
-00000c10: 2020 2020 7374 796c 653d 226f 7665 7266      style="overf
-00000c20: 6c6f 773a 7669 7369 626c 6522 3e0d 0a20  low:visible">.. 
-00000c30: 2020 2020 203c 7061 7468 0d0a 2020 2020       <path..    
-00000c40: 2020 2020 2069 643d 2270 6174 6833 3839       id="path389
-00000c50: 3622 0d0a 2020 2020 2020 2020 2064 3d22  6"..         d="
-00000c60: 4d20 302c 3020 352c 2d35 202d 3132 2e35  M 0,0 5,-5 -12.5
-00000c70: 2c30 2035 2c35 2030 2c30 207a 220d 0a20  ,0 5,5 0,0 z".. 
-00000c80: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
-00000c90: 696c 6c2d 7275 6c65 3a65 7665 6e6f 6464  ill-rule:evenodd
-00000ca0: 3b73 7472 6f6b 653a 2330 3030 3030 303b  ;stroke:#000000;
-00000cb0: 7374 726f 6b65 2d77 6964 7468 3a31 7074  stroke-width:1pt
-00000cc0: 3b6d 6172 6b65 722d 7374 6172 743a 6e6f  ;marker-start:no
-00000cd0: 6e65 220d 0a20 2020 2020 2020 2020 7472  ne"..         tr
-00000ce0: 616e 7366 6f72 6d3d 226d 6174 7269 7828  ansform="matrix(
-00000cf0: 2d30 2e32 2c30 2c30 2c2d 302e 322c 2d31  -0.2,0,0,-0.2,-1
-00000d00: 2e32 2c30 2922 0d0a 2020 2020 2020 2020  .2,0)"..        
-00000d10: 2069 6e6b 7363 6170 653a 636f 6e6e 6563   inkscape:connec
-00000d20: 746f 722d 6375 7276 6174 7572 653d 2230  tor-curvature="0
-00000d30: 2220 2f3e 0d0a 2020 2020 3c2f 6d61 726b  " />..    </mark
-00000d40: 6572 3e0d 0a20 2020 203c 6d61 726b 6572  er>..    <marker
-00000d50: 0d0a 2020 2020 2020 2069 6e6b 7363 6170  ..       inkscap
-00000d60: 653a 7374 6f63 6b69 643d 2241 7272 6f77  e:stockid="Arrow
-00000d70: 314d 656e 6422 0d0a 2020 2020 2020 206f  1Mend"..       o
-00000d80: 7269 656e 743d 2261 7574 6f22 0d0a 2020  rient="auto"..  
-00000d90: 2020 2020 2072 6566 593d 2230 220d 0a20       refY="0".. 
-00000da0: 2020 2020 2020 7265 6658 3d22 3022 0d0a        refX="0"..
-00000db0: 2020 2020 2020 2069 643d 2241 7272 6f77         id="Arrow
-00000dc0: 314d 656e 6422 0d0a 2020 2020 2020 2073  1Mend"..       s
-00000dd0: 7479 6c65 3d22 6f76 6572 666c 6f77 3a76  tyle="overflow:v
-00000de0: 6973 6962 6c65 223e 0d0a 2020 2020 2020  isible">..      
-00000df0: 3c70 6174 680d 0a20 2020 2020 2020 2020  <path..         
-00000e00: 6964 3d22 7061 7468 3338 3930 220d 0a20  id="path3890".. 
-00000e10: 2020 2020 2020 2020 643d 224d 2030 2c30          d="M 0,0
-00000e20: 2035 2c2d 3520 2d31 322e 352c 3020 352c   5,-5 -12.5,0 5,
-00000e30: 3520 302c 3020 7a22 0d0a 2020 2020 2020  5 0,0 z"..      
-00000e40: 2020 2073 7479 6c65 3d22 6669 6c6c 2d72     style="fill-r
-00000e50: 756c 653a 6576 656e 6f64 643b 7374 726f  ule:evenodd;stro
-00000e60: 6b65 3a23 3030 3030 3030 3b73 7472 6f6b  ke:#000000;strok
-00000e70: 652d 7769 6474 683a 3170 743b 6d61 726b  e-width:1pt;mark
-00000e80: 6572 2d73 7461 7274 3a6e 6f6e 6522 0d0a  er-start:none"..
-00000e90: 2020 2020 2020 2020 2074 7261 6e73 666f           transfo
-00000ea0: 726d 3d22 6d61 7472 6978 282d 302e 342c  rm="matrix(-0.4,
-00000eb0: 302c 302c 2d30 2e34 2c2d 342c 3029 220d  0,0,-0.4,-4,0)".
-00000ec0: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-00000ed0: 7065 3a63 6f6e 6e65 6374 6f72 2d63 7572  pe:connector-cur
-00000ee0: 7661 7475 7265 3d22 3022 202f 3e0d 0a20  vature="0" />.. 
-00000ef0: 2020 203c 2f6d 6172 6b65 723e 0d0a 2020     </marker>..  
-00000f00: 2020 3c6d 6172 6b65 720d 0a20 2020 2020    <marker..     
-00000f10: 2020 696e 6b73 6361 7065 3a73 746f 636b    inkscape:stock
-00000f20: 6964 3d22 4172 726f 7732 4c65 6e64 220d  id="Arrow2Lend".
-00000f30: 0a20 2020 2020 2020 6f72 6965 6e74 3d22  .       orient="
-00000f40: 6175 746f 220d 0a20 2020 2020 2020 7265  auto"..       re
-00000f50: 6659 3d22 3022 0d0a 2020 2020 2020 2072  fY="0"..       r
-00000f60: 6566 583d 2230 220d 0a20 2020 2020 2020  efX="0"..       
-00000f70: 6964 3d22 4172 726f 7732 4c65 6e64 220d  id="Arrow2Lend".
-00000f80: 0a20 2020 2020 2020 7374 796c 653d 226f  .       style="o
-00000f90: 7665 7266 6c6f 773a 7669 7369 626c 6522  verflow:visible"
-00000fa0: 3e0d 0a20 2020 2020 203c 7061 7468 0d0a  >..      <path..
-00000fb0: 2020 2020 2020 2020 2069 643d 2270 6174           id="pat
-00000fc0: 6833 3930 3222 0d0a 2020 2020 2020 2020  h3902"..        
-00000fd0: 2073 7479 6c65 3d22 666f 6e74 2d73 697a   style="font-siz
-00000fe0: 653a 3132 7078 3b66 696c 6c2d 7275 6c65  e:12px;fill-rule
-00000ff0: 3a65 7665 6e6f 6464 3b73 7472 6f6b 652d  :evenodd;stroke-
-00001000: 7769 6474 683a 302e 3632 353b 7374 726f  width:0.625;stro
-00001010: 6b65 2d6c 696e 656a 6f69 6e3a 726f 756e  ke-linejoin:roun
-00001020: 6422 0d0a 2020 2020 2020 2020 2064 3d22  d"..         d="
-00001030: 4d20 382e 3731 3835 3837 382c 342e 3033  M 8.7185878,4.03
-00001040: 3337 3335 3220 2d32 2e32 3037 3238 3935  37352 -2.2072895
-00001050: 2c30 2e30 3136 3031 3332 3620 382e 3731  ,0.01601326 8.71
-00001060: 3835 3838 342c 2d34 2e30 3031 3730 3738  85884,-4.0017078
-00001070: 2063 202d 312e 3734 3534 3938 342c 322e   c -1.7454984,2.
-00001080: 3337 3230 3630 3920 2d31 2e37 3335 3434  3720609 -1.73544
-00001090: 3038 2c35 2e36 3137 3435 3139 202d 3665  08,5.6174519 -6e
-000010a0: 2d37 2c38 2e30 3335 3434 3320 7a22 0d0a  -7,8.035443 z"..
-000010b0: 2020 2020 2020 2020 2074 7261 6e73 666f           transfo
-000010c0: 726d 3d22 6d61 7472 6978 282d 312e 312c  rm="matrix(-1.1,
-000010d0: 302c 302c 2d31 2e31 2c2d 312e 312c 3029  0,0,-1.1,-1.1,0)
-000010e0: 220d 0a20 2020 2020 2020 2020 696e 6b73  "..         inks
-000010f0: 6361 7065 3a63 6f6e 6e65 6374 6f72 2d63  cape:connector-c
-00001100: 7572 7661 7475 7265 3d22 3022 202f 3e0d  urvature="0" />.
-00001110: 0a20 2020 203c 2f6d 6172 6b65 723e 0d0a  .    </marker>..
-00001120: 2020 2020 3c6c 696e 6561 7247 7261 6469      <linearGradi
-00001130: 656e 740d 0a20 2020 2020 2020 6964 3d22  ent..       id="
-00001140: 6c69 6e65 6172 4772 6164 6965 6e74 3338  linearGradient38
-00001150: 3132 223e 0d0a 2020 2020 2020 3c73 746f  12">..      <sto
-00001160: 700d 0a20 2020 2020 2020 2020 7374 796c  p..         styl
-00001170: 653d 2273 746f 702d 636f 6c6f 723a 2366  e="stop-color:#f
-00001180: 3066 3066 303b 7374 6f70 2d6f 7061 6369  0f0f0;stop-opaci
-00001190: 7479 3a31 3b22 0d0a 2020 2020 2020 2020  ty:1;"..        
-000011a0: 206f 6666 7365 743d 2230 220d 0a20 2020   offset="0"..   
-000011b0: 2020 2020 2020 6964 3d22 7374 6f70 3338        id="stop38
-000011c0: 3134 2220 2f3e 0d0a 2020 2020 2020 3c73  14" />..      <s
-000011d0: 746f 700d 0a20 2020 2020 2020 2020 7374  top..         st
-000011e0: 796c 653d 2273 746f 702d 636f 6c6f 723a  yle="stop-color:
-000011f0: 2366 6666 6666 663b 7374 6f70 2d6f 7061  #ffffff;stop-opa
-00001200: 6369 7479 3a31 3b22 0d0a 2020 2020 2020  city:1;"..      
-00001210: 2020 206f 6666 7365 743d 2231 220d 0a20     offset="1".. 
-00001220: 2020 2020 2020 2020 6964 3d22 7374 6f70          id="stop
-00001230: 3338 3136 2220 2f3e 0d0a 2020 2020 3c2f  3816" />..    </
-00001240: 6c69 6e65 6172 4772 6164 6965 6e74 3e0d  linearGradient>.
-00001250: 0a20 2020 203c 6c69 6e65 6172 4772 6164  .    <linearGrad
-00001260: 6965 6e74 0d0a 2020 2020 2020 2069 643d  ient..       id=
-00001270: 226c 696e 6561 7247 7261 6469 656e 7433  "linearGradient3
-00001280: 3830 3222 0d0a 2020 2020 2020 206f 7362  802"..       osb
-00001290: 3a70 6169 6e74 3d22 736f 6c69 6422 3e0d  :paint="solid">.
-000012a0: 0a20 2020 2020 203c 7374 6f70 0d0a 2020  .      <stop..  
+00000030: 226e 6f22 3f3e 0a3c 212d 2d20 4372 6561  "no"?>.<!-- Crea
+00000040: 7465 6420 7769 7468 2049 6e6b 7363 6170  ted with Inkscap
+00000050: 6520 2868 7474 703a 2f2f 7777 772e 696e  e (http://www.in
+00000060: 6b73 6361 7065 2e6f 7267 2f29 202d 2d3e  kscape.org/) -->
+00000070: 0a0a 3c73 7667 0a20 2020 7665 7273 696f  ..<svg.   versio
+00000080: 6e3d 2231 2e30 220a 2020 2077 6964 7468  n="1.0".   width
+00000090: 3d22 3238 3022 0a20 2020 6865 6967 6874  ="280".   height
+000000a0: 3d22 3234 3022 0a20 2020 6964 3d22 7376  ="240".   id="sv
+000000b0: 6732 220a 2020 2073 6f64 6970 6f64 693a  g2".   sodipodi:
+000000c0: 7665 7273 696f 6e3d 2230 2e33 3222 0a20  version="0.32". 
+000000d0: 2020 696e 6b73 6361 7065 3a76 6572 7369    inkscape:versi
+000000e0: 6f6e 3d22 312e 322e 3220 2837 3332 6130  on="1.2.2 (732a0
+000000f0: 3164 6136 332c 2032 3032 322d 3132 2d30  1da63, 2022-12-0
+00000100: 3929 220a 2020 2073 6f64 6970 6f64 693a  9)".   sodipodi:
+00000110: 646f 636e 616d 653d 2267 7569 6461 7461  docname="guidata
+00000120: 2d76 6572 7469 6361 6c2e 7376 6722 0a20  -vertical.svg". 
+00000130: 2020 696e 6b73 6361 7065 3a6f 7574 7075    inkscape:outpu
+00000140: 745f 6578 7465 6e73 696f 6e3d 226f 7267  t_extension="org
+00000150: 2e69 6e6b 7363 6170 652e 6f75 7470 7574  .inkscape.output
+00000160: 2e73 7667 2e69 6e6b 7363 6170 6522 0a20  .svg.inkscape". 
+00000170: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
+00000180: 742d 6669 6c65 6e61 6d65 3d22 2e2e 5c2e  t-filename="..\.
+00000190: 2e5c 646f 635c 696d 6167 6573 5c67 7569  .\doc\images\gui
+000001a0: 6461 7461 2d76 6572 7469 6361 6c2e 706e  data-vertical.pn
+000001b0: 6722 0a20 2020 696e 6b73 6361 7065 3a65  g".   inkscape:e
+000001c0: 7870 6f72 742d 7864 7069 3d22 3432 2e38  xport-xdpi="42.8
+000001d0: 3537 3134 3322 0a20 2020 696e 6b73 6361  57143".   inksca
+000001e0: 7065 3a65 7870 6f72 742d 7964 7069 3d22  pe:export-ydpi="
+000001f0: 3432 2e38 3537 3134 3322 0a20 2020 786d  42.857143".   xm
+00000200: 6c6e 733a 696e 6b73 6361 7065 3d22 6874  lns:inkscape="ht
+00000210: 7470 3a2f 2f77 7777 2e69 6e6b 7363 6170  tp://www.inkscap
+00000220: 652e 6f72 672f 6e61 6d65 7370 6163 6573  e.org/namespaces
+00000230: 2f69 6e6b 7363 6170 6522 0a20 2020 786d  /inkscape".   xm
+00000240: 6c6e 733a 736f 6469 706f 6469 3d22 6874  lns:sodipodi="ht
+00000250: 7470 3a2f 2f73 6f64 6970 6f64 692e 736f  tp://sodipodi.so
+00000260: 7572 6365 666f 7267 652e 6e65 742f 4454  urceforge.net/DT
+00000270: 442f 736f 6469 706f 6469 2d30 2e64 7464  D/sodipodi-0.dtd
+00000280: 220a 2020 2078 6d6c 6e73 3a78 6c69 6e6b  ".   xmlns:xlink
+00000290: 3d22 6874 7470 3a2f 2f77 7777 2e77 332e  ="http://www.w3.
+000002a0: 6f72 672f 3139 3939 2f78 6c69 6e6b 220a  org/1999/xlink".
+000002b0: 2020 2078 6d6c 6e73 3d22 6874 7470 3a2f     xmlns="http:/
+000002c0: 2f77 7777 2e77 332e 6f72 672f 3230 3030  /www.w3.org/2000
+000002d0: 2f73 7667 220a 2020 2078 6d6c 6e73 3a73  /svg".   xmlns:s
+000002e0: 7667 3d22 6874 7470 3a2f 2f77 7777 2e77  vg="http://www.w
+000002f0: 332e 6f72 672f 3230 3030 2f73 7667 220a  3.org/2000/svg".
+00000300: 2020 2078 6d6c 6e73 3a72 6466 3d22 6874     xmlns:rdf="ht
+00000310: 7470 3a2f 2f77 7777 2e77 332e 6f72 672f  tp://www.w3.org/
+00000320: 3139 3939 2f30 322f 3232 2d72 6466 2d73  1999/02/22-rdf-s
+00000330: 796e 7461 782d 6e73 2322 0a20 2020 786d  yntax-ns#".   xm
+00000340: 6c6e 733a 6363 3d22 6874 7470 3a2f 2f63  lns:cc="http://c
+00000350: 7265 6174 6976 6563 6f6d 6d6f 6e73 2e6f  reativecommons.o
+00000360: 7267 2f6e 7323 220a 2020 2078 6d6c 6e73  rg/ns#".   xmlns
+00000370: 3a64 633d 2268 7474 703a 2f2f 7075 726c  :dc="http://purl
+00000380: 2e6f 7267 2f64 632f 656c 656d 656e 7473  .org/dc/elements
+00000390: 2f31 2e31 2f22 3e0a 2020 3c6d 6574 6164  /1.1/">.  <metad
+000003a0: 6174 610a 2020 2020 2069 643d 226d 6574  ata.     id="met
+000003b0: 6164 6174 6132 3139 3322 3e0a 2020 2020  adata2193">.    
+000003c0: 3c72 6466 3a52 4446 3e0a 2020 2020 2020  <rdf:RDF>.      
+000003d0: 3c63 633a 576f 726b 0a20 2020 2020 2020  <cc:Work.       
+000003e0: 2020 7264 663a 6162 6f75 743d 2222 3e0a    rdf:about="">.
+000003f0: 2020 2020 2020 2020 3c64 633a 666f 726d          <dc:form
+00000400: 6174 3e69 6d61 6765 2f73 7667 2b78 6d6c  at>image/svg+xml
+00000410: 3c2f 6463 3a66 6f72 6d61 743e 0a20 2020  </dc:format>.   
+00000420: 2020 2020 203c 6463 3a74 7970 650a 2020       <dc:type.  
+00000430: 2020 2020 2020 2020 2072 6466 3a72 6573           rdf:res
+00000440: 6f75 7263 653d 2268 7474 703a 2f2f 7075  ource="http://pu
+00000450: 726c 2e6f 7267 2f64 632f 6463 6d69 7479  rl.org/dc/dcmity
+00000460: 7065 2f53 7469 6c6c 496d 6167 6522 202f  pe/StillImage" /
+00000470: 3e0a 2020 2020 2020 3c2f 6363 3a57 6f72  >.      </cc:Wor
+00000480: 6b3e 0a20 2020 203c 2f72 6466 3a52 4446  k>.    </rdf:RDF
+00000490: 3e0a 2020 3c2f 6d65 7461 6461 7461 3e0a  >.  </metadata>.
+000004a0: 2020 3c73 6f64 6970 6f64 693a 6e61 6d65    <sodipodi:name
+000004b0: 6476 6965 770a 2020 2020 2069 6e6b 7363  dview.     inksc
+000004c0: 6170 653a 7769 6e64 6f77 2d68 6569 6768  ape:window-heigh
+000004d0: 743d 2231 3031 3722 0a20 2020 2020 696e  t="1017".     in
+000004e0: 6b73 6361 7065 3a77 696e 646f 772d 7769  kscape:window-wi
+000004f0: 6474 683d 2231 3932 3022 0a20 2020 2020  dth="1920".     
+00000500: 696e 6b73 6361 7065 3a70 6167 6573 6861  inkscape:pagesha
+00000510: 646f 773d 2232 220a 2020 2020 2069 6e6b  dow="2".     ink
+00000520: 7363 6170 653a 7061 6765 6f70 6163 6974  scape:pageopacit
+00000530: 793d 2230 2e30 220a 2020 2020 2062 6f72  y="0.0".     bor
+00000540: 6465 726f 7061 6369 7479 3d22 312e 3022  deropacity="1.0"
+00000550: 0a20 2020 2020 626f 7264 6572 636f 6c6f  .     bordercolo
+00000560: 723d 2223 3636 3636 3636 220a 2020 2020  r="#666666".    
+00000570: 2070 6167 6563 6f6c 6f72 3d22 2366 6666   pagecolor="#fff
+00000580: 6666 6622 0a20 2020 2020 6964 3d22 6261  fff".     id="ba
+00000590: 7365 220a 2020 2020 2069 6e6b 7363 6170  se".     inkscap
+000005a0: 653a 7a6f 6f6d 3d22 322e 3832 3834 3237  e:zoom="2.828427
+000005b0: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
+000005c0: 6378 3d22 3138 302e 3133 3534 3622 0a20  cx="180.13546". 
+000005d0: 2020 2020 696e 6b73 6361 7065 3a63 793d      inkscape:cy=
+000005e0: 2231 3337 2e31 3738 3732 220a 2020 2020  "137.17872".    
+000005f0: 2069 6e6b 7363 6170 653a 7769 6e64 6f77   inkscape:window
+00000600: 2d78 3d22 3139 3132 220a 2020 2020 2069  -x="1912".     i
+00000610: 6e6b 7363 6170 653a 7769 6e64 6f77 2d79  nkscape:window-y
+00000620: 3d22 2d38 220a 2020 2020 2069 6e6b 7363  ="-8".     inksc
+00000630: 6170 653a 6375 7272 656e 742d 6c61 7965  ape:current-laye
+00000640: 723d 2273 7667 3222 0a20 2020 2020 7368  r="svg2".     sh
+00000650: 6f77 6772 6964 3d22 6661 6c73 6522 0a20  owgrid="false". 
+00000660: 2020 2020 6669 742d 6d61 7267 696e 2d74      fit-margin-t
+00000670: 6f70 3d22 3022 0a20 2020 2020 6669 742d  op="0".     fit-
+00000680: 6d61 7267 696e 2d6c 6566 743d 2230 220a  margin-left="0".
+00000690: 2020 2020 2066 6974 2d6d 6172 6769 6e2d       fit-margin-
+000006a0: 7269 6768 743d 2230 220a 2020 2020 2066  right="0".     f
+000006b0: 6974 2d6d 6172 6769 6e2d 626f 7474 6f6d  it-margin-bottom
+000006c0: 3d22 3022 0a20 2020 2020 696e 6b73 6361  ="0".     inksca
+000006d0: 7065 3a77 696e 646f 772d 6d61 7869 6d69  pe:window-maximi
+000006e0: 7a65 643d 2231 220a 2020 2020 2069 6e6b  zed="1".     ink
+000006f0: 7363 6170 653a 7368 6f77 7061 6765 7368  scape:showpagesh
+00000700: 6164 6f77 3d22 3222 0a20 2020 2020 696e  adow="2".     in
+00000710: 6b73 6361 7065 3a70 6167 6563 6865 636b  kscape:pagecheck
+00000720: 6572 626f 6172 643d 2274 7275 6522 0a20  erboard="true". 
+00000730: 2020 2020 696e 6b73 6361 7065 3a64 6573      inkscape:des
+00000740: 6b63 6f6c 6f72 3d22 2364 3164 3164 3122  kcolor="#d1d1d1"
+00000750: 202f 3e0a 2020 3c64 6566 730a 2020 2020   />.  <defs.    
+00000760: 2069 643d 2264 6566 7334 223e 0a20 2020   id="defs4">.   
+00000770: 203c 6d61 726b 6572 0a20 2020 2020 2020   <marker.       
+00000780: 696e 6b73 6361 7065 3a73 746f 636b 6964  inkscape:stockid
+00000790: 3d22 4172 726f 7732 4d65 6e64 220a 2020  ="Arrow2Mend".  
+000007a0: 2020 2020 206f 7269 656e 743d 2261 7574       orient="aut
+000007b0: 6f22 0a20 2020 2020 2020 7265 6659 3d22  o".       refY="
+000007c0: 3022 0a20 2020 2020 2020 7265 6658 3d22  0".       refX="
+000007d0: 3022 0a20 2020 2020 2020 6964 3d22 4172  0".       id="Ar
+000007e0: 726f 7732 4d65 6e64 220a 2020 2020 2020  row2Mend".      
+000007f0: 2073 7479 6c65 3d22 6f76 6572 666c 6f77   style="overflow
+00000800: 3a76 6973 6962 6c65 223e 0a20 2020 2020  :visible">.     
+00000810: 203c 7061 7468 0a20 2020 2020 2020 2020   <path.         
+00000820: 6964 3d22 7061 7468 3339 3038 220a 2020  id="path3908".  
+00000830: 2020 2020 2020 2073 7479 6c65 3d22 666f         style="fo
+00000840: 6e74 2d73 697a 653a 3132 7078 3b66 696c  nt-size:12px;fil
+00000850: 6c2d 7275 6c65 3a65 7665 6e6f 6464 3b73  l-rule:evenodd;s
+00000860: 7472 6f6b 652d 7769 6474 683a 302e 3632  troke-width:0.62
+00000870: 353b 7374 726f 6b65 2d6c 696e 656a 6f69  5;stroke-linejoi
+00000880: 6e3a 726f 756e 6422 0a20 2020 2020 2020  n:round".       
+00000890: 2020 643d 224d 2038 2e37 3138 3538 3738    d="M 8.7185878
+000008a0: 2c34 2e30 3333 3733 3532 202d 322e 3230  ,4.0337352 -2.20
+000008b0: 3732 3839 352c 302e 3031 3630 3133 3236  72895,0.01601326
+000008c0: 2038 2e37 3138 3538 3834 2c2d 342e 3030   8.7185884,-4.00
+000008d0: 3137 3037 3820 6320 2d31 2e37 3435 3439  17078 c -1.74549
+000008e0: 3834 2c32 2e33 3732 3036 3039 202d 312e  84,2.3720609 -1.
+000008f0: 3733 3534 3430 382c 352e 3631 3734 3531  7354408,5.617451
+00000900: 3920 2d36 652d 372c 382e 3033 3534 3433  9 -6e-7,8.035443
+00000910: 207a 220a 2020 2020 2020 2020 2074 7261   z".         tra
+00000920: 6e73 666f 726d 3d22 7363 616c 6528 2d30  nsform="scale(-0
+00000930: 2e36 2922 0a20 2020 2020 2020 2020 696e  .6)".         in
+00000940: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
+00000950: 2d63 7572 7661 7475 7265 3d22 3022 202f  -curvature="0" /
+00000960: 3e0a 2020 2020 3c2f 6d61 726b 6572 3e0a  >.    </marker>.
+00000970: 2020 2020 3c6d 6172 6b65 720a 2020 2020      <marker.    
+00000980: 2020 2069 6e6b 7363 6170 653a 7374 6f63     inkscape:stoc
+00000990: 6b69 643d 2241 7272 6f77 3153 656e 6422  kid="Arrow1Send"
+000009a0: 0a20 2020 2020 2020 6f72 6965 6e74 3d22  .       orient="
+000009b0: 6175 746f 220a 2020 2020 2020 2072 6566  auto".       ref
+000009c0: 593d 2230 220a 2020 2020 2020 2072 6566  Y="0".       ref
+000009d0: 583d 2230 220a 2020 2020 2020 2069 643d  X="0".       id=
+000009e0: 2241 7272 6f77 3153 656e 6422 0a20 2020  "Arrow1Send".   
+000009f0: 2020 2020 7374 796c 653d 226f 7665 7266      style="overf
+00000a00: 6c6f 773a 7669 7369 626c 6522 3e0a 2020  low:visible">.  
+00000a10: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
+00000a20: 2020 2069 643d 2270 6174 6833 3839 3622     id="path3896"
+00000a30: 0a20 2020 2020 2020 2020 643d 224d 2030  .         d="M 0
+00000a40: 2c30 2035 2c2d 3520 2d31 322e 352c 3020  ,0 5,-5 -12.5,0 
+00000a50: 352c 3520 5a22 0a20 2020 2020 2020 2020  5,5 Z".         
+00000a60: 7374 796c 653d 2266 696c 6c2d 7275 6c65  style="fill-rule
+00000a70: 3a65 7665 6e6f 6464 3b73 7472 6f6b 653a  :evenodd;stroke:
+00000a80: 2330 3030 3030 303b 7374 726f 6b65 2d77  #000000;stroke-w
+00000a90: 6964 7468 3a31 7074 3b6d 6172 6b65 722d  idth:1pt;marker-
+00000aa0: 7374 6172 743a 6e6f 6e65 220a 2020 2020  start:none".    
+00000ab0: 2020 2020 2074 7261 6e73 666f 726d 3d22       transform="
+00000ac0: 6d61 7472 6978 282d 302e 322c 302c 302c  matrix(-0.2,0,0,
+00000ad0: 2d30 2e32 2c2d 312e 322c 3029 220a 2020  -0.2,-1.2,0)".  
+00000ae0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00000af0: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
+00000b00: 7572 653d 2230 2220 2f3e 0a20 2020 203c  ure="0" />.    <
+00000b10: 2f6d 6172 6b65 723e 0a20 2020 203c 6d61  /marker>.    <ma
+00000b20: 726b 6572 0a20 2020 2020 2020 696e 6b73  rker.       inks
+00000b30: 6361 7065 3a73 746f 636b 6964 3d22 4172  cape:stockid="Ar
+00000b40: 726f 7731 4d65 6e64 220a 2020 2020 2020  row1Mend".      
+00000b50: 206f 7269 656e 743d 2261 7574 6f22 0a20   orient="auto". 
+00000b60: 2020 2020 2020 7265 6659 3d22 3022 0a20        refY="0". 
+00000b70: 2020 2020 2020 7265 6658 3d22 3022 0a20        refX="0". 
+00000b80: 2020 2020 2020 6964 3d22 4172 726f 7731        id="Arrow1
+00000b90: 4d65 6e64 220a 2020 2020 2020 2073 7479  Mend".       sty
+00000ba0: 6c65 3d22 6f76 6572 666c 6f77 3a76 6973  le="overflow:vis
+00000bb0: 6962 6c65 223e 0a20 2020 2020 203c 7061  ible">.      <pa
+00000bc0: 7468 0a20 2020 2020 2020 2020 6964 3d22  th.         id="
+00000bd0: 7061 7468 3338 3930 220a 2020 2020 2020  path3890".      
+00000be0: 2020 2064 3d22 4d20 302c 3020 352c 2d35     d="M 0,0 5,-5
+00000bf0: 202d 3132 2e35 2c30 2035 2c35 205a 220a   -12.5,0 5,5 Z".
+00000c00: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+00000c10: 6669 6c6c 2d72 756c 653a 6576 656e 6f64  fill-rule:evenod
+00000c20: 643b 7374 726f 6b65 3a23 3030 3030 3030  d;stroke:#000000
+00000c30: 3b73 7472 6f6b 652d 7769 6474 683a 3170  ;stroke-width:1p
+00000c40: 743b 6d61 726b 6572 2d73 7461 7274 3a6e  t;marker-start:n
+00000c50: 6f6e 6522 0a20 2020 2020 2020 2020 7472  one".         tr
+00000c60: 616e 7366 6f72 6d3d 226d 6174 7269 7828  ansform="matrix(
+00000c70: 2d30 2e34 2c30 2c30 2c2d 302e 342c 2d34  -0.4,0,0,-0.4,-4
+00000c80: 2c30 2922 0a20 2020 2020 2020 2020 696e  ,0)".         in
+00000c90: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
+00000ca0: 2d63 7572 7661 7475 7265 3d22 3022 202f  -curvature="0" /
+00000cb0: 3e0a 2020 2020 3c2f 6d61 726b 6572 3e0a  >.    </marker>.
+00000cc0: 2020 2020 3c6d 6172 6b65 720a 2020 2020      <marker.    
+00000cd0: 2020 2069 6e6b 7363 6170 653a 7374 6f63     inkscape:stoc
+00000ce0: 6b69 643d 2241 7272 6f77 324c 656e 6422  kid="Arrow2Lend"
+00000cf0: 0a20 2020 2020 2020 6f72 6965 6e74 3d22  .       orient="
+00000d00: 6175 746f 220a 2020 2020 2020 2072 6566  auto".       ref
+00000d10: 593d 2230 220a 2020 2020 2020 2072 6566  Y="0".       ref
+00000d20: 583d 2230 220a 2020 2020 2020 2069 643d  X="0".       id=
+00000d30: 2241 7272 6f77 324c 656e 6422 0a20 2020  "Arrow2Lend".   
+00000d40: 2020 2020 7374 796c 653d 226f 7665 7266      style="overf
+00000d50: 6c6f 773a 7669 7369 626c 6522 3e0a 2020  low:visible">.  
+00000d60: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
+00000d70: 2020 2069 643d 2270 6174 6833 3930 3222     id="path3902"
+00000d80: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
+00000d90: 2266 6f6e 742d 7369 7a65 3a31 3270 783b  "font-size:12px;
+00000da0: 6669 6c6c 2d72 756c 653a 6576 656e 6f64  fill-rule:evenod
+00000db0: 643b 7374 726f 6b65 2d77 6964 7468 3a30  d;stroke-width:0
+00000dc0: 2e36 3235 3b73 7472 6f6b 652d 6c69 6e65  .625;stroke-line
+00000dd0: 6a6f 696e 3a72 6f75 6e64 220a 2020 2020  join:round".    
+00000de0: 2020 2020 2064 3d22 4d20 382e 3731 3835       d="M 8.7185
+00000df0: 3837 382c 342e 3033 3337 3335 3220 2d32  878,4.0337352 -2
+00000e00: 2e32 3037 3238 3935 2c30 2e30 3136 3031  .2072895,0.01601
+00000e10: 3332 3620 382e 3731 3835 3838 342c 2d34  326 8.7185884,-4
+00000e20: 2e30 3031 3730 3738 2063 202d 312e 3734  .0017078 c -1.74
+00000e30: 3534 3938 342c 322e 3337 3230 3630 3920  54984,2.3720609 
+00000e40: 2d31 2e37 3335 3434 3038 2c35 2e36 3137  -1.7354408,5.617
+00000e50: 3435 3139 202d 3665 2d37 2c38 2e30 3335  4519 -6e-7,8.035
+00000e60: 3434 3320 7a22 0a20 2020 2020 2020 2020  443 z".         
+00000e70: 7472 616e 7366 6f72 6d3d 226d 6174 7269  transform="matri
+00000e80: 7828 2d31 2e31 2c30 2c30 2c2d 312e 312c  x(-1.1,0,0,-1.1,
+00000e90: 2d31 2e31 2c30 2922 0a20 2020 2020 2020  -1.1,0)".       
+00000ea0: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
+00000eb0: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
+00000ec0: 3022 202f 3e0a 2020 2020 3c2f 6d61 726b  0" />.    </mark
+00000ed0: 6572 3e0a 2020 2020 3c6c 696e 6561 7247  er>.    <linearG
+00000ee0: 7261 6469 656e 740a 2020 2020 2020 2069  radient.       i
+00000ef0: 643d 226c 696e 6561 7247 7261 6469 656e  d="linearGradien
+00000f00: 7433 3831 3222 3e0a 2020 2020 2020 3c73  t3812">.      <s
+00000f10: 746f 700a 2020 2020 2020 2020 2073 7479  top.         sty
+00000f20: 6c65 3d22 7374 6f70 2d63 6f6c 6f72 3a23  le="stop-color:#
+00000f30: 6432 6432 6432 3b73 746f 702d 6f70 6163  d2d2d2;stop-opac
+00000f40: 6974 793a 313b 220a 2020 2020 2020 2020  ity:1;".        
+00000f50: 206f 6666 7365 743d 2230 220a 2020 2020   offset="0".    
+00000f60: 2020 2020 2069 643d 2273 746f 7033 3831       id="stop381
+00000f70: 3422 202f 3e0a 2020 2020 2020 3c73 746f  4" />.      <sto
+00000f80: 700a 2020 2020 2020 2020 2073 7479 6c65  p.         style
+00000f90: 3d22 7374 6f70 2d63 6f6c 6f72 3a23 6666  ="stop-color:#ff
+00000fa0: 6666 6666 3b73 746f 702d 6f70 6163 6974  ffff;stop-opacit
+00000fb0: 793a 313b 220a 2020 2020 2020 2020 206f  y:1;".         o
+00000fc0: 6666 7365 743d 2231 220a 2020 2020 2020  ffset="1".      
+00000fd0: 2020 2069 643d 2273 746f 7033 3831 3622     id="stop3816"
+00000fe0: 202f 3e0a 2020 2020 3c2f 6c69 6e65 6172   />.    </linear
+00000ff0: 4772 6164 6965 6e74 3e0a 2020 2020 3c6c  Gradient>.    <l
+00001000: 696e 6561 7247 7261 6469 656e 740a 2020  inearGradient.  
+00001010: 2020 2020 2069 643d 226c 696e 6561 7247       id="linearG
+00001020: 7261 6469 656e 7433 3830 3222 0a20 2020  radient3802".   
+00001030: 2020 2020 696e 6b73 6361 7065 3a73 7761      inkscape:swa
+00001040: 7463 683d 2273 6f6c 6964 223e 0a20 2020  tch="solid">.   
+00001050: 2020 203c 7374 6f70 0a20 2020 2020 2020     <stop.       
+00001060: 2020 7374 796c 653d 2273 746f 702d 636f    style="stop-co
+00001070: 6c6f 723a 2338 3038 3038 303b 7374 6f70  lor:#808080;stop
+00001080: 2d6f 7061 6369 7479 3a31 3b22 0a20 2020  -opacity:1;".   
+00001090: 2020 2020 2020 6f66 6673 6574 3d22 3022        offset="0"
+000010a0: 0a20 2020 2020 2020 2020 6964 3d22 7374  .         id="st
+000010b0: 6f70 3338 3034 2220 2f3e 0a20 2020 203c  op3804" />.    <
+000010c0: 2f6c 696e 6561 7247 7261 6469 656e 743e  /linearGradient>
+000010d0: 0a20 2020 203c 6c69 6e65 6172 4772 6164  .    <linearGrad
+000010e0: 6965 6e74 0a20 2020 2020 2020 6964 3d22  ient.       id="
+000010f0: 6c69 6e65 6172 4772 6164 6965 6e74 3333  linearGradient33
+00001100: 3530 223e 0a20 2020 2020 203c 7374 6f70  50">.      <stop
+00001110: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
+00001120: 2273 746f 702d 636f 6c6f 723a 2330 3063  "stop-color:#00c
+00001130: 6232 623b 7374 6f70 2d6f 7061 6369 7479  b2b;stop-opacity
+00001140: 3a30 2e32 3437 3933 3338 383b 220a 2020  :0.24793388;".  
+00001150: 2020 2020 2020 206f 6666 7365 743d 2230         offset="0
+00001160: 220a 2020 2020 2020 2020 2069 643d 2273  ".         id="s
+00001170: 746f 7033 3335 3222 202f 3e0a 2020 2020  top3352" />.    
+00001180: 2020 3c73 746f 700a 2020 2020 2020 2020    <stop.        
+00001190: 2073 7479 6c65 3d22 7374 6f70 2d63 6f6c   style="stop-col
+000011a0: 6f72 3a23 3030 6362 3262 3b73 746f 702d  or:#00cb2b;stop-
+000011b0: 6f70 6163 6974 793a 313b 220a 2020 2020  opacity:1;".    
+000011c0: 2020 2020 206f 6666 7365 743d 2231 220a       offset="1".
+000011d0: 2020 2020 2020 2020 2069 643d 2273 746f           id="sto
+000011e0: 7033 3335 3422 202f 3e0a 2020 2020 3c2f  p3354" />.    </
+000011f0: 6c69 6e65 6172 4772 6164 6965 6e74 3e0a  linearGradient>.
+00001200: 2020 2020 3c6c 696e 6561 7247 7261 6469      <linearGradi
+00001210: 656e 740a 2020 2020 2020 2069 643d 226c  ent.       id="l
+00001220: 696e 6561 7247 7261 6469 656e 7433 3334  inearGradient334
+00001230: 3222 3e0a 2020 2020 2020 3c73 746f 700a  2">.      <stop.
+00001240: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+00001250: 7374 6f70 2d63 6f6c 6f72 3a23 3030 3561  stop-color:#005a
+00001260: 3835 3b73 746f 702d 6f70 6163 6974 793a  85;stop-opacity:
+00001270: 313b 220a 2020 2020 2020 2020 206f 6666  1;".         off
+00001280: 7365 743d 2230 220a 2020 2020 2020 2020  set="0".        
+00001290: 2069 643d 2273 746f 7033 3334 3422 202f   id="stop3344" /
+000012a0: 3e0a 2020 2020 2020 3c73 746f 700a 2020  >.      <stop.  
 000012b0: 2020 2020 2020 2073 7479 6c65 3d22 7374         style="st
-000012c0: 6f70 2d63 6f6c 6f72 3a23 3830 3830 3830  op-color:#808080
-000012d0: 3b73 746f 702d 6f70 6163 6974 793a 313b  ;stop-opacity:1;
-000012e0: 220d 0a20 2020 2020 2020 2020 6f66 6673  "..         offs
-000012f0: 6574 3d22 3022 0d0a 2020 2020 2020 2020  et="0"..        
-00001300: 2069 643d 2273 746f 7033 3830 3422 202f   id="stop3804" /
-00001310: 3e0d 0a20 2020 203c 2f6c 696e 6561 7247  >..    </linearG
-00001320: 7261 6469 656e 743e 0d0a 2020 2020 3c6c  radient>..    <l
-00001330: 696e 6561 7247 7261 6469 656e 740d 0a20  inearGradient.. 
-00001340: 2020 2020 2020 6964 3d22 6c69 6e65 6172        id="linear
-00001350: 4772 6164 6965 6e74 3333 3530 223e 0d0a  Gradient3350">..
-00001360: 2020 2020 2020 3c73 746f 700d 0a20 2020        <stop..   
-00001370: 2020 2020 2020 7374 796c 653d 2273 746f        style="sto
-00001380: 702d 636f 6c6f 723a 2330 3063 6232 623b  p-color:#00cb2b;
-00001390: 7374 6f70 2d6f 7061 6369 7479 3a30 2e32  stop-opacity:0.2
-000013a0: 3437 3933 3338 383b 220d 0a20 2020 2020  4793388;"..     
-000013b0: 2020 2020 6f66 6673 6574 3d22 3022 0d0a      offset="0"..
-000013c0: 2020 2020 2020 2020 2069 643d 2273 746f           id="sto
-000013d0: 7033 3335 3222 202f 3e0d 0a20 2020 2020  p3352" />..     
-000013e0: 203c 7374 6f70 0d0a 2020 2020 2020 2020   <stop..        
-000013f0: 2073 7479 6c65 3d22 7374 6f70 2d63 6f6c   style="stop-col
-00001400: 6f72 3a23 3030 6362 3262 3b73 746f 702d  or:#00cb2b;stop-
-00001410: 6f70 6163 6974 793a 313b 220d 0a20 2020  opacity:1;"..   
-00001420: 2020 2020 2020 6f66 6673 6574 3d22 3122        offset="1"
-00001430: 0d0a 2020 2020 2020 2020 2069 643d 2273  ..         id="s
-00001440: 746f 7033 3335 3422 202f 3e0d 0a20 2020  top3354" />..   
-00001450: 203c 2f6c 696e 6561 7247 7261 6469 656e   </linearGradien
-00001460: 743e 0d0a 2020 2020 3c6c 696e 6561 7247  t>..    <linearG
-00001470: 7261 6469 656e 740d 0a20 2020 2020 2020  radient..       
-00001480: 6964 3d22 6c69 6e65 6172 4772 6164 6965  id="linearGradie
-00001490: 6e74 3333 3432 223e 0d0a 2020 2020 2020  nt3342">..      
-000014a0: 3c73 746f 700d 0a20 2020 2020 2020 2020  <stop..         
-000014b0: 7374 796c 653d 2273 746f 702d 636f 6c6f  style="stop-colo
-000014c0: 723a 2330 3035 6138 353b 7374 6f70 2d6f  r:#005a85;stop-o
-000014d0: 7061 6369 7479 3a31 3b22 0d0a 2020 2020  pacity:1;"..    
-000014e0: 2020 2020 206f 6666 7365 743d 2230 220d       offset="0".
-000014f0: 0a20 2020 2020 2020 2020 6964 3d22 7374  .         id="st
-00001500: 6f70 3333 3434 2220 2f3e 0d0a 2020 2020  op3344" />..    
-00001510: 2020 3c73 746f 700d 0a20 2020 2020 2020    <stop..       
-00001520: 2020 7374 796c 653d 2273 746f 702d 636f    style="stop-co
-00001530: 6c6f 723a 2330 3035 6138 353b 7374 6f70  lor:#005a85;stop
-00001540: 2d6f 7061 6369 7479 3a30 2e37 3532 3036  -opacity:0.75206
-00001550: 3631 343b 220d 0a20 2020 2020 2020 2020  614;"..         
-00001560: 6f66 6673 6574 3d22 3122 0d0a 2020 2020  offset="1"..    
-00001570: 2020 2020 2069 643d 2273 746f 7033 3334       id="stop334
-00001580: 3622 202f 3e0d 0a20 2020 203c 2f6c 696e  6" />..    </lin
-00001590: 6561 7247 7261 6469 656e 743e 0d0a 2020  earGradient>..  
-000015a0: 2020 3c6c 696e 6561 7247 7261 6469 656e    <linearGradien
-000015b0: 740d 0a20 2020 2020 2020 6964 3d22 6c69  t..       id="li
-000015c0: 6e65 6172 4772 6164 6965 6e74 3333 3130  nearGradient3310
-000015d0: 223e 0d0a 2020 2020 2020 3c73 746f 700d  ">..      <stop.
-000015e0: 0a20 2020 2020 2020 2020 6964 3d22 7374  .         id="st
-000015f0: 6f70 3333 3132 220d 0a20 2020 2020 2020  op3312"..       
-00001600: 2020 6f66 6673 6574 3d22 3022 0d0a 2020    offset="0"..  
-00001610: 2020 2020 2020 2073 7479 6c65 3d22 7374         style="st
-00001620: 6f70 2d63 6f6c 6f72 3a23 6165 3032 3032  op-color:#ae0202
-00001630: 3b73 746f 702d 6f70 6163 6974 793a 313b  ;stop-opacity:1;
-00001640: 2220 2f3e 0d0a 2020 2020 2020 3c73 746f  " />..      <sto
-00001650: 700d 0a20 2020 2020 2020 2020 6964 3d22  p..         id="
-00001660: 7374 6f70 3333 3134 220d 0a20 2020 2020  stop3314"..     
-00001670: 2020 2020 6f66 6673 6574 3d22 3122 0d0a      offset="1"..
-00001680: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
-00001690: 7374 6f70 2d63 6f6c 6f72 3a23 6234 3735  stop-color:#b475
-000016a0: 3735 3b73 746f 702d 6f70 6163 6974 793a  75;stop-opacity:
-000016b0: 313b 2220 2f3e 0d0a 2020 2020 3c2f 6c69  1;" />..    </li
-000016c0: 6e65 6172 4772 6164 6965 6e74 3e0d 0a20  nearGradient>.. 
-000016d0: 2020 203c 696e 6b73 6361 7065 3a70 6572     <inkscape:per
-000016e0: 7370 6563 7469 7665 0d0a 2020 2020 2020  spective..      
-000016f0: 2073 6f64 6970 6f64 693a 7479 7065 3d22   sodipodi:type="
-00001700: 696e 6b73 6361 7065 3a70 6572 7370 3364  inkscape:persp3d
-00001710: 220d 0a20 2020 2020 2020 696e 6b73 6361  "..       inksca
-00001720: 7065 3a76 705f 783d 2230 203a 2037 312e  pe:vp_x="0 : 71.
-00001730: 3838 3734 3937 203a 2031 220d 0a20 2020  887497 : 1"..   
-00001740: 2020 2020 696e 6b73 6361 7065 3a76 705f      inkscape:vp_
-00001750: 793d 2230 203a 2031 3030 3020 3a20 3022  y="0 : 1000 : 0"
-00001760: 0d0a 2020 2020 2020 2069 6e6b 7363 6170  ..       inkscap
-00001770: 653a 7670 5f7a 3d22 3438 362e 3034 3939  e:vp_z="486.0499
-00001780: 3920 3a20 3731 2e38 3837 3439 3720 3a20  9 : 71.887497 : 
-00001790: 3122 0d0a 2020 2020 2020 2069 6e6b 7363  1"..       inksc
-000017a0: 6170 653a 7065 7273 7033 642d 6f72 6967  ape:persp3d-orig
-000017b0: 696e 3d22 3234 332e 3032 3439 3920 3a20  in="243.02499 : 
-000017c0: 3437 2e39 3234 3939 3820 3a20 3122 0d0a  47.924998 : 1"..
-000017d0: 2020 2020 2020 2069 643d 2270 6572 7370         id="persp
-000017e0: 6563 7469 7665 3437 2220 2f3e 0d0a 2020  ective47" />..  
-000017f0: 2020 3c6c 696e 6561 7247 7261 6469 656e    <linearGradien
-00001800: 740d 0a20 2020 2020 2020 6964 3d22 6c69  t..       id="li
-00001810: 6e65 6172 4772 6164 6965 6e74 3237 3935  nearGradient2795
-00001820: 223e 0d0a 2020 2020 2020 3c73 746f 700d  ">..      <stop.
-00001830: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
-00001840: 2273 746f 702d 636f 6c6f 723a 2362 3862  "stop-color:#b8b
-00001850: 3862 383b 7374 6f70 2d6f 7061 6369 7479  8b8;stop-opacity
-00001860: 3a30 2e34 3938 3033 3932 3222 0d0a 2020  :0.49803922"..  
-00001870: 2020 2020 2020 206f 6666 7365 743d 2230         offset="0
-00001880: 220d 0a20 2020 2020 2020 2020 6964 3d22  "..         id="
-00001890: 7374 6f70 3237 3937 2220 2f3e 0d0a 2020  stop2797" />..  
-000018a0: 2020 2020 3c73 746f 700d 0a20 2020 2020      <stop..     
-000018b0: 2020 2020 7374 796c 653d 2273 746f 702d      style="stop-
-000018c0: 636f 6c6f 723a 2337 6637 6637 663b 7374  color:#7f7f7f;st
-000018d0: 6f70 2d6f 7061 6369 7479 3a30 220d 0a20  op-opacity:0".. 
-000018e0: 2020 2020 2020 2020 6f66 6673 6574 3d22          offset="
-000018f0: 3122 0d0a 2020 2020 2020 2020 2069 643d  1"..         id=
-00001900: 2273 746f 7032 3739 3922 202f 3e0d 0a20  "stop2799" />.. 
-00001910: 2020 203c 2f6c 696e 6561 7247 7261 6469     </linearGradi
-00001920: 656e 743e 0d0a 2020 2020 3c6c 696e 6561  ent>..    <linea
-00001930: 7247 7261 6469 656e 740d 0a20 2020 2020  rGradient..     
-00001940: 2020 6964 3d22 6c69 6e65 6172 4772 6164    id="linearGrad
-00001950: 6965 6e74 3237 3837 223e 0d0a 2020 2020  ient2787">..    
-00001960: 2020 3c73 746f 700d 0a20 2020 2020 2020    <stop..       
-00001970: 2020 7374 796c 653d 2273 746f 702d 636f    style="stop-co
-00001980: 6c6f 723a 2337 6637 6637 663b 7374 6f70  lor:#7f7f7f;stop
-00001990: 2d6f 7061 6369 7479 3a30 2e35 220d 0a20  -opacity:0.5".. 
-000019a0: 2020 2020 2020 2020 6f66 6673 6574 3d22          offset="
-000019b0: 3022 0d0a 2020 2020 2020 2020 2069 643d  0"..         id=
-000019c0: 2273 746f 7032 3738 3922 202f 3e0d 0a20  "stop2789" />.. 
-000019d0: 2020 2020 203c 7374 6f70 0d0a 2020 2020       <stop..    
-000019e0: 2020 2020 2073 7479 6c65 3d22 7374 6f70       style="stop
-000019f0: 2d63 6f6c 6f72 3a23 3766 3766 3766 3b73  -color:#7f7f7f;s
-00001a00: 746f 702d 6f70 6163 6974 793a 3022 0d0a  top-opacity:0"..
-00001a10: 2020 2020 2020 2020 206f 6666 7365 743d           offset=
-00001a20: 2231 220d 0a20 2020 2020 2020 2020 6964  "1"..         id
-00001a30: 3d22 7374 6f70 3237 3931 2220 2f3e 0d0a  ="stop2791" />..
-00001a40: 2020 2020 3c2f 6c69 6e65 6172 4772 6164      </linearGrad
-00001a50: 6965 6e74 3e0d 0a20 2020 203c 6c69 6e65  ient>..    <line
-00001a60: 6172 4772 6164 6965 6e74 0d0a 2020 2020  arGradient..    
-00001a70: 2020 2069 643d 226c 696e 6561 7247 7261     id="linearGra
-00001a80: 6469 656e 7433 3637 3622 3e0d 0a20 2020  dient3676">..   
-00001a90: 2020 203c 7374 6f70 0d0a 2020 2020 2020     <stop..      
-00001aa0: 2020 2073 7479 6c65 3d22 7374 6f70 2d63     style="stop-c
-00001ab0: 6f6c 6f72 3a23 6232 6232 6232 3b73 746f  olor:#b2b2b2;sto
-00001ac0: 702d 6f70 6163 6974 793a 302e 3522 0d0a  p-opacity:0.5"..
-00001ad0: 2020 2020 2020 2020 206f 6666 7365 743d           offset=
-00001ae0: 2230 220d 0a20 2020 2020 2020 2020 6964  "0"..         id
-00001af0: 3d22 7374 6f70 3336 3738 2220 2f3e 0d0a  ="stop3678" />..
-00001b00: 2020 2020 2020 3c73 746f 700d 0a20 2020        <stop..   
-00001b10: 2020 2020 2020 7374 796c 653d 2273 746f        style="sto
-00001b20: 702d 636f 6c6f 723a 2362 3362 3362 333b  p-color:#b3b3b3;
-00001b30: 7374 6f70 2d6f 7061 6369 7479 3a30 220d  stop-opacity:0".
-00001b40: 0a20 2020 2020 2020 2020 6f66 6673 6574  .         offset
-00001b50: 3d22 3122 0d0a 2020 2020 2020 2020 2069  ="1"..         i
-00001b60: 643d 2273 746f 7033 3638 3022 202f 3e0d  d="stop3680" />.
-00001b70: 0a20 2020 203c 2f6c 696e 6561 7247 7261  .    </linearGra
-00001b80: 6469 656e 743e 0d0a 2020 2020 3c6c 696e  dient>..    <lin
-00001b90: 6561 7247 7261 6469 656e 740d 0a20 2020  earGradient..   
-00001ba0: 2020 2020 6964 3d22 6c69 6e65 6172 4772      id="linearGr
-00001bb0: 6164 6965 6e74 3332 3336 223e 0d0a 2020  adient3236">..  
-00001bc0: 2020 2020 3c73 746f 700d 0a20 2020 2020      <stop..     
-00001bd0: 2020 2020 7374 796c 653d 2273 746f 702d      style="stop-
-00001be0: 636f 6c6f 723a 2366 3466 3466 343b 7374  color:#f4f4f4;st
-00001bf0: 6f70 2d6f 7061 6369 7479 3a31 220d 0a20  op-opacity:1".. 
-00001c00: 2020 2020 2020 2020 6f66 6673 6574 3d22          offset="
-00001c10: 3022 0d0a 2020 2020 2020 2020 2069 643d  0"..         id=
-00001c20: 2273 746f 7033 3234 3422 202f 3e0d 0a20  "stop3244" />.. 
-00001c30: 2020 2020 203c 7374 6f70 0d0a 2020 2020       <stop..    
-00001c40: 2020 2020 2073 7479 6c65 3d22 7374 6f70       style="stop
-00001c50: 2d63 6f6c 6f72 3a23 6666 6666 6666 3b73  -color:#ffffff;s
-00001c60: 746f 702d 6f70 6163 6974 793a 3122 0d0a  top-opacity:1"..
-00001c70: 2020 2020 2020 2020 206f 6666 7365 743d           offset=
-00001c80: 2231 220d 0a20 2020 2020 2020 2020 6964  "1"..         id
-00001c90: 3d22 7374 6f70 3332 3430 2220 2f3e 0d0a  ="stop3240" />..
-00001ca0: 2020 2020 3c2f 6c69 6e65 6172 4772 6164      </linearGrad
-00001cb0: 6965 6e74 3e0d 0a20 2020 203c 6c69 6e65  ient>..    <line
-00001cc0: 6172 4772 6164 6965 6e74 0d0a 2020 2020  arGradient..    
-00001cd0: 2020 2069 643d 226c 696e 6561 7247 7261     id="linearGra
-00001ce0: 6469 656e 7434 3637 3122 3e0d 0a20 2020  dient4671">..   
-00001cf0: 2020 203c 7374 6f70 0d0a 2020 2020 2020     <stop..      
-00001d00: 2020 2073 7479 6c65 3d22 7374 6f70 2d63     style="stop-c
-00001d10: 6f6c 6f72 3a23 6666 6434 3362 3b73 746f  olor:#ffd43b;sto
-00001d20: 702d 6f70 6163 6974 793a 3122 0d0a 2020  p-opacity:1"..  
-00001d30: 2020 2020 2020 206f 6666 7365 743d 2230         offset="0
-00001d40: 220d 0a20 2020 2020 2020 2020 6964 3d22  "..         id="
-00001d50: 7374 6f70 3436 3733 2220 2f3e 0d0a 2020  stop4673" />..  
-00001d60: 2020 2020 3c73 746f 700d 0a20 2020 2020      <stop..     
-00001d70: 2020 2020 7374 796c 653d 2273 746f 702d      style="stop-
-00001d80: 636f 6c6f 723a 2366 6665 3837 333b 7374  color:#ffe873;st
-00001d90: 6f70 2d6f 7061 6369 7479 3a31 220d 0a20  op-opacity:1".. 
-00001da0: 2020 2020 2020 2020 6f66 6673 6574 3d22          offset="
-00001db0: 3122 0d0a 2020 2020 2020 2020 2069 643d  1"..         id=
-00001dc0: 2273 746f 7034 3637 3522 202f 3e0d 0a20  "stop4675" />.. 
-00001dd0: 2020 203c 2f6c 696e 6561 7247 7261 6469     </linearGradi
-00001de0: 656e 743e 0d0a 2020 2020 3c6c 696e 6561  ent>..    <linea
-00001df0: 7247 7261 6469 656e 740d 0a20 2020 2020  rGradient..     
-00001e00: 2020 6964 3d22 6c69 6e65 6172 4772 6164    id="linearGrad
-00001e10: 6965 6e74 3436 3839 223e 0d0a 2020 2020  ient4689">..    
-00001e20: 2020 3c73 746f 700d 0a20 2020 2020 2020    <stop..       
-00001e30: 2020 7374 796c 653d 2273 746f 702d 636f    style="stop-co
-00001e40: 6c6f 723a 2335 6139 6664 343b 7374 6f70  lor:#5a9fd4;stop
-00001e50: 2d6f 7061 6369 7479 3a31 220d 0a20 2020  -opacity:1"..   
-00001e60: 2020 2020 2020 6f66 6673 6574 3d22 3022        offset="0"
-00001e70: 0d0a 2020 2020 2020 2020 2069 643d 2273  ..         id="s
-00001e80: 746f 7034 3639 3122 202f 3e0d 0a20 2020  top4691" />..   
-00001e90: 2020 203c 7374 6f70 0d0a 2020 2020 2020     <stop..      
-00001ea0: 2020 2073 7479 6c65 3d22 7374 6f70 2d63     style="stop-c
-00001eb0: 6f6c 6f72 3a23 3330 3639 3938 3b73 746f  olor:#306998;sto
-00001ec0: 702d 6f70 6163 6974 793a 3122 0d0a 2020  p-opacity:1"..  
-00001ed0: 2020 2020 2020 206f 6666 7365 743d 2231         offset="1
-00001ee0: 220d 0a20 2020 2020 2020 2020 6964 3d22  "..         id="
-00001ef0: 7374 6f70 3436 3933 2220 2f3e 0d0a 2020  stop4693" />..  
-00001f00: 2020 3c2f 6c69 6e65 6172 4772 6164 6965    </linearGradie
-00001f10: 6e74 3e0d 0a20 2020 203c 6c69 6e65 6172  nt>..    <linear
-00001f20: 4772 6164 6965 6e74 0d0a 2020 2020 2020  Gradient..      
-00001f30: 2078 313d 2232 3234 2e32 3339 3936 220d   x1="224.23996".
-00001f40: 0a20 2020 2020 2020 7931 3d22 3134 342e  .       y1="144.
-00001f50: 3735 3731 3722 0d0a 2020 2020 2020 2078  75717"..       x
-00001f60: 323d 222d 3635 2e33 3038 3530 3222 0d0a  2="-65.308502"..
-00001f70: 2020 2020 2020 2079 323d 2231 3434 2e37         y2="144.7
-00001f80: 3537 3137 220d 0a20 2020 2020 2020 6964  5717"..       id
-00001f90: 3d22 6c69 6e65 6172 4772 6164 6965 6e74  ="linearGradient
-00001fa0: 3239 3837 220d 0a20 2020 2020 2020 786c  2987"..       xl
-00001fb0: 696e 6b3a 6872 6566 3d22 236c 696e 6561  ink:href="#linea
-00001fc0: 7247 7261 6469 656e 7434 3637 3122 0d0a  rGradient4671"..
-00001fd0: 2020 2020 2020 2067 7261 6469 656e 7455         gradientU
-00001fe0: 6e69 7473 3d22 7573 6572 5370 6163 654f  nits="userSpaceO
-00001ff0: 6e55 7365 220d 0a20 2020 2020 2020 6772  nUse"..       gr
-00002000: 6164 6965 6e74 5472 616e 7366 6f72 6d3d  adientTransform=
-00002010: 2274 7261 6e73 6c61 7465 2831 3030 2e32  "translate(100.2
-00002020: 3730 322c 3939 2e36 3131 3136 2922 202f  702,99.61116)" /
-00002030: 3e0d 0a20 2020 203c 6c69 6e65 6172 4772  >..    <linearGr
-00002040: 6164 6965 6e74 0d0a 2020 2020 2020 2078  adient..       x
-00002050: 313d 2231 3732 2e39 3432 3038 220d 0a20  1="172.94208".. 
-00002060: 2020 2020 2020 7931 3d22 3737 2e34 3735        y1="77.475
-00002070: 3938 3322 0d0a 2020 2020 2020 2078 323d  983"..       x2=
-00002080: 2232 362e 3637 3032 3938 220d 0a20 2020  "26.670298"..   
-00002090: 2020 2020 7932 3d22 3736 2e33 3133 3133      y2="76.31313
-000020a0: 3322 0d0a 2020 2020 2020 2069 643d 226c  3"..       id="l
-000020b0: 696e 6561 7247 7261 6469 656e 7432 3939  inearGradient299
-000020c0: 3022 0d0a 2020 2020 2020 2078 6c69 6e6b  0"..       xlink
-000020d0: 3a68 7265 663d 2223 6c69 6e65 6172 4772  :href="#linearGr
-000020e0: 6164 6965 6e74 3436 3839 220d 0a20 2020  adient4689"..   
-000020f0: 2020 2020 6772 6164 6965 6e74 556e 6974      gradientUnit
-00002100: 733d 2275 7365 7253 7061 6365 4f6e 5573  s="userSpaceOnUs
-00002110: 6522 0d0a 2020 2020 2020 2067 7261 6469  e"..       gradi
-00002120: 656e 7454 7261 6e73 666f 726d 3d22 7472  entTransform="tr
-00002130: 616e 736c 6174 6528 3130 302e 3237 3032  anslate(100.2702
-00002140: 2c39 392e 3631 3131 3629 2220 2f3e 0d0a  ,99.61116)" />..
-00002150: 2020 2020 3c6c 696e 6561 7247 7261 6469      <linearGradi
-00002160: 656e 740d 0a20 2020 2020 2020 7831 3d22  ent..       x1="
-00002170: 3137 322e 3934 3230 3822 0d0a 2020 2020  172.94208"..    
-00002180: 2020 2079 313d 2237 372e 3437 3539 3833     y1="77.475983
-00002190: 220d 0a20 2020 2020 2020 7832 3d22 3236  "..       x2="26
-000021a0: 2e36 3730 3239 3822 0d0a 2020 2020 2020  .670298"..      
-000021b0: 2079 323d 2237 362e 3331 3331 3333 220d   y2="76.313133".
-000021c0: 0a20 2020 2020 2020 6964 3d22 6c69 6e65  .       id="line
-000021d0: 6172 4772 6164 6965 6e74 3235 3837 220d  arGradient2587".
-000021e0: 0a20 2020 2020 2020 786c 696e 6b3a 6872  .       xlink:hr
-000021f0: 6566 3d22 236c 696e 6561 7247 7261 6469  ef="#linearGradi
-00002200: 656e 7434 3638 3922 0d0a 2020 2020 2020  ent4689"..      
-00002210: 2067 7261 6469 656e 7455 6e69 7473 3d22   gradientUnits="
-00002220: 7573 6572 5370 6163 654f 6e55 7365 220d  userSpaceOnUse".
-00002230: 0a20 2020 2020 2020 6772 6164 6965 6e74  .       gradient
-00002240: 5472 616e 7366 6f72 6d3d 2274 7261 6e73  Transform="trans
-00002250: 6c61 7465 2831 3030 2e32 3730 322c 3939  late(100.2702,99
-00002260: 2e36 3131 3136 2922 202f 3e0d 0a20 2020  .61116)" />..   
-00002270: 203c 6c69 6e65 6172 4772 6164 6965 6e74   <linearGradient
-00002280: 0d0a 2020 2020 2020 2078 313d 2232 3234  ..       x1="224
-00002290: 2e32 3339 3936 220d 0a20 2020 2020 2020  .23996"..       
-000022a0: 7931 3d22 3134 342e 3735 3731 3722 0d0a  y1="144.75717"..
-000022b0: 2020 2020 2020 2078 323d 222d 3635 2e33         x2="-65.3
-000022c0: 3038 3530 3222 0d0a 2020 2020 2020 2079  08502"..       y
-000022d0: 323d 2231 3434 2e37 3537 3137 220d 0a20  2="144.75717".. 
-000022e0: 2020 2020 2020 6964 3d22 6c69 6e65 6172        id="linear
-000022f0: 4772 6164 6965 6e74 3235 3839 220d 0a20  Gradient2589".. 
-00002300: 2020 2020 2020 786c 696e 6b3a 6872 6566        xlink:href
-00002310: 3d22 236c 696e 6561 7247 7261 6469 656e  ="#linearGradien
-00002320: 7434 3637 3122 0d0a 2020 2020 2020 2067  t4671"..       g
-00002330: 7261 6469 656e 7455 6e69 7473 3d22 7573  radientUnits="us
-00002340: 6572 5370 6163 654f 6e55 7365 220d 0a20  erSpaceOnUse".. 
-00002350: 2020 2020 2020 6772 6164 6965 6e74 5472        gradientTr
-00002360: 616e 7366 6f72 6d3d 2274 7261 6e73 6c61  ansform="transla
-00002370: 7465 2831 3030 2e32 3730 322c 3939 2e36  te(100.2702,99.6
-00002380: 3131 3136 2922 202f 3e0d 0a20 2020 203c  1116)" />..    <
-00002390: 6c69 6e65 6172 4772 6164 6965 6e74 0d0a  linearGradient..
-000023a0: 2020 2020 2020 2078 313d 2231 3732 2e39         x1="172.9
-000023b0: 3432 3038 220d 0a20 2020 2020 2020 7931  4208"..       y1
-000023c0: 3d22 3737 2e34 3735 3938 3322 0d0a 2020  ="77.475983"..  
-000023d0: 2020 2020 2078 323d 2232 362e 3637 3032       x2="26.6702
-000023e0: 3938 220d 0a20 2020 2020 2020 7932 3d22  98"..       y2="
-000023f0: 3736 2e33 3133 3133 3322 0d0a 2020 2020  76.313133"..    
-00002400: 2020 2069 643d 226c 696e 6561 7247 7261     id="linearGra
-00002410: 6469 656e 7432 3234 3822 0d0a 2020 2020  dient2248"..    
-00002420: 2020 2078 6c69 6e6b 3a68 7265 663d 2223     xlink:href="#
-00002430: 6c69 6e65 6172 4772 6164 6965 6e74 3436  linearGradient46
-00002440: 3839 220d 0a20 2020 2020 2020 6772 6164  89"..       grad
-00002450: 6965 6e74 556e 6974 733d 2275 7365 7253  ientUnits="userS
-00002460: 7061 6365 4f6e 5573 6522 0d0a 2020 2020  paceOnUse"..    
-00002470: 2020 2067 7261 6469 656e 7454 7261 6e73     gradientTrans
-00002480: 666f 726d 3d22 7472 616e 736c 6174 6528  form="translate(
-00002490: 3130 302e 3237 3032 2c39 392e 3631 3131  100.2702,99.6111
-000024a0: 3629 2220 2f3e 0d0a 2020 2020 3c6c 696e  6)" />..    <lin
-000024b0: 6561 7247 7261 6469 656e 740d 0a20 2020  earGradient..   
-000024c0: 2020 2020 7831 3d22 3232 342e 3233 3939      x1="224.2399
-000024d0: 3622 0d0a 2020 2020 2020 2079 313d 2231  6"..       y1="1
-000024e0: 3434 2e37 3537 3137 220d 0a20 2020 2020  44.75717"..     
-000024f0: 2020 7832 3d22 2d36 352e 3330 3835 3032    x2="-65.308502
-00002500: 220d 0a20 2020 2020 2020 7932 3d22 3134  "..       y2="14
-00002510: 342e 3735 3731 3722 0d0a 2020 2020 2020  4.75717"..      
-00002520: 2069 643d 226c 696e 6561 7247 7261 6469   id="linearGradi
-00002530: 656e 7432 3235 3022 0d0a 2020 2020 2020  ent2250"..      
-00002540: 2078 6c69 6e6b 3a68 7265 663d 2223 6c69   xlink:href="#li
-00002550: 6e65 6172 4772 6164 6965 6e74 3436 3731  nearGradient4671
-00002560: 220d 0a20 2020 2020 2020 6772 6164 6965  "..       gradie
-00002570: 6e74 556e 6974 733d 2275 7365 7253 7061  ntUnits="userSpa
-00002580: 6365 4f6e 5573 6522 0d0a 2020 2020 2020  ceOnUse"..      
-00002590: 2067 7261 6469 656e 7454 7261 6e73 666f   gradientTransfo
-000025a0: 726d 3d22 7472 616e 736c 6174 6528 3130  rm="translate(10
-000025b0: 302e 3237 3032 2c39 392e 3631 3131 3629  0.2702,99.61116)
-000025c0: 2220 2f3e 0d0a 2020 2020 3c6c 696e 6561  " />..    <linea
-000025d0: 7247 7261 6469 656e 740d 0a20 2020 2020  rGradient..     
-000025e0: 2020 7831 3d22 3232 342e 3233 3939 3622    x1="224.23996"
-000025f0: 0d0a 2020 2020 2020 2079 313d 2231 3434  ..       y1="144
-00002600: 2e37 3537 3137 220d 0a20 2020 2020 2020  .75717"..       
-00002610: 7832 3d22 2d36 352e 3330 3835 3032 220d  x2="-65.308502".
-00002620: 0a20 2020 2020 2020 7932 3d22 3134 342e  .       y2="144.
-00002630: 3735 3731 3722 0d0a 2020 2020 2020 2069  75717"..       i
-00002640: 643d 226c 696e 6561 7247 7261 6469 656e  d="linearGradien
-00002650: 7432 3235 3522 0d0a 2020 2020 2020 2078  t2255"..       x
-00002660: 6c69 6e6b 3a68 7265 663d 2223 6c69 6e65  link:href="#line
-00002670: 6172 4772 6164 6965 6e74 3436 3731 220d  arGradient4671".
-00002680: 0a20 2020 2020 2020 6772 6164 6965 6e74  .       gradient
-00002690: 556e 6974 733d 2275 7365 7253 7061 6365  Units="userSpace
-000026a0: 4f6e 5573 6522 0d0a 2020 2020 2020 2067  OnUse"..       g
-000026b0: 7261 6469 656e 7454 7261 6e73 666f 726d  radientTransform
-000026c0: 3d22 6d61 7472 6978 2830 2e35 3632 3534  ="matrix(0.56254
-000026d0: 312c 302c 302c 302e 3536 3739 3732 2c2d  1,0,0,0.567972,-
-000026e0: 3131 2e35 3937 342c 2d37 2e36 3039 3534  11.5974,-7.60954
-000026f0: 2922 202f 3e0d 0a20 2020 203c 6c69 6e65  )" />..    <line
-00002700: 6172 4772 6164 6965 6e74 0d0a 2020 2020  arGradient..    
-00002710: 2020 2078 313d 2231 3732 2e39 3432 3038     x1="172.94208
-00002720: 220d 0a20 2020 2020 2020 7931 3d22 3736  "..       y1="76
-00002730: 2e31 3736 3232 3422 0d0a 2020 2020 2020  .176224"..      
-00002740: 2078 323d 2232 362e 3637 3032 3938 220d   x2="26.670298".
-00002750: 0a20 2020 2020 2020 7932 3d22 3736 2e33  .       y2="76.3
-00002760: 3133 3133 3322 0d0a 2020 2020 2020 2069  13133"..       i
-00002770: 643d 226c 696e 6561 7247 7261 6469 656e  d="linearGradien
-00002780: 7432 3235 3822 0d0a 2020 2020 2020 2078  t2258"..       x
-00002790: 6c69 6e6b 3a68 7265 663d 2223 6c69 6e65  link:href="#line
-000027a0: 6172 4772 6164 6965 6e74 3436 3839 220d  arGradient4689".
-000027b0: 0a20 2020 2020 2020 6772 6164 6965 6e74  .       gradient
-000027c0: 556e 6974 733d 2275 7365 7253 7061 6365  Units="userSpace
-000027d0: 4f6e 5573 6522 0d0a 2020 2020 2020 2067  OnUse"..       g
-000027e0: 7261 6469 656e 7454 7261 6e73 666f 726d  radientTransform
-000027f0: 3d22 6d61 7472 6978 2830 2e35 3632 3534  ="matrix(0.56254
-00002800: 312c 302c 302c 302e 3536 3739 3732 2c2d  1,0,0,0.567972,-
-00002810: 3131 2e35 3937 342c 2d37 2e36 3039 3534  11.5974,-7.60954
-00002820: 2922 202f 3e0d 0a20 2020 203c 7261 6469  )" />..    <radi
-00002830: 616c 4772 6164 6965 6e74 0d0a 2020 2020  alGradient..    
-00002840: 2020 2063 783d 2236 312e 3531 3838 3833     cx="61.518883
-00002850: 220d 0a20 2020 2020 2020 6379 3d22 3133  "..       cy="13
-00002860: 322e 3238 3537 3522 0d0a 2020 2020 2020  2.28575"..      
-00002870: 2072 3d22 3239 2e30 3336 3931 3322 0d0a   r="29.036913"..
-00002880: 2020 2020 2020 2066 783d 2236 312e 3531         fx="61.51
-00002890: 3838 3833 220d 0a20 2020 2020 2020 6679  8883"..       fy
-000028a0: 3d22 3133 322e 3238 3537 3522 0d0a 2020  ="132.28575"..  
-000028b0: 2020 2020 2069 643d 2272 6164 6961 6c47       id="radialG
-000028c0: 7261 6469 656e 7432 3830 3122 0d0a 2020  radient2801"..  
-000028d0: 2020 2020 2078 6c69 6e6b 3a68 7265 663d       xlink:href=
-000028e0: 2223 6c69 6e65 6172 4772 6164 6965 6e74  "#linearGradient
-000028f0: 3237 3935 220d 0a20 2020 2020 2020 6772  2795"..       gr
-00002900: 6164 6965 6e74 556e 6974 733d 2275 7365  adientUnits="use
-00002910: 7253 7061 6365 4f6e 5573 6522 0d0a 2020  rSpaceOnUse"..  
-00002920: 2020 2020 2067 7261 6469 656e 7454 7261       gradientTra
-00002930: 6e73 666f 726d 3d22 6d61 7472 6978 2831  nsform="matrix(1
-00002940: 2c30 2c30 2c30 2e31 3737 3936 362c 302c  ,0,0,0.177966,0,
-00002950: 3130 382e 3734 3334 2922 202f 3e0d 0a20  108.7434)" />.. 
-00002960: 2020 203c 6c69 6e65 6172 4772 6164 6965     <linearGradie
-00002970: 6e74 0d0a 2020 2020 2020 2078 313d 2231  nt..       x1="1
-00002980: 3530 2e39 3631 3131 220d 0a20 2020 2020  50.96111"..     
-00002990: 2020 7931 3d22 3139 322e 3335 3137 3622    y1="192.35176"
-000029a0: 0d0a 2020 2020 2020 2078 323d 2231 3132  ..       x2="112
-000029b0: 2e30 3331 3434 220d 0a20 2020 2020 2020  .03144"..       
-000029c0: 7932 3d22 3133 372e 3237 3239 3922 0d0a  y2="137.27299"..
-000029d0: 2020 2020 2020 2069 643d 226c 696e 6561         id="linea
-000029e0: 7247 7261 6469 656e 7431 3437 3522 0d0a  rGradient1475"..
-000029f0: 2020 2020 2020 2078 6c69 6e6b 3a68 7265         xlink:hre
-00002a00: 663d 2223 6c69 6e65 6172 4772 6164 6965  f="#linearGradie
-00002a10: 6e74 3436 3731 220d 0a20 2020 2020 2020  nt4671"..       
-00002a20: 6772 6164 6965 6e74 556e 6974 733d 2275  gradientUnits="u
-00002a30: 7365 7253 7061 6365 4f6e 5573 6522 0d0a  serSpaceOnUse"..
-00002a40: 2020 2020 2020 2067 7261 6469 656e 7454         gradientT
-00002a50: 7261 6e73 666f 726d 3d22 6d61 7472 6978  ransform="matrix
-00002a60: 2830 2e35 3632 3534 312c 302c 302c 302e  (0.562541,0,0,0.
-00002a70: 3536 3739 3732 2c2d 392e 3339 3937 3439  567972,-9.399749
-00002a80: 2c2d 352e 3330 3533 3137 2922 202f 3e0d  ,-5.305317)" />.
-00002a90: 0a20 2020 203c 6c69 6e65 6172 4772 6164  .    <linearGrad
-00002aa0: 6965 6e74 0d0a 2020 2020 2020 2078 313d  ient..       x1=
-00002ab0: 2232 362e 3634 3839 3337 220d 0a20 2020  "26.648937"..   
-00002ac0: 2020 2020 7931 3d22 3230 2e36 3033 3738      y1="20.60378
-00002ad0: 3122 0d0a 2020 2020 2020 2078 323d 2231  1"..       x2="1
-00002ae0: 3335 2e36 3635 3235 220d 0a20 2020 2020  35.66525"..     
-00002af0: 2020 7932 3d22 3131 342e 3339 3736 3722    y2="114.39767"
-00002b00: 0d0a 2020 2020 2020 2069 643d 226c 696e  ..       id="lin
-00002b10: 6561 7247 7261 6469 656e 7431 3437 3822  earGradient1478"
-00002b20: 0d0a 2020 2020 2020 2078 6c69 6e6b 3a68  ..       xlink:h
-00002b30: 7265 663d 2223 6c69 6e65 6172 4772 6164  ref="#linearGrad
-00002b40: 6965 6e74 3436 3839 220d 0a20 2020 2020  ient4689"..     
-00002b50: 2020 6772 6164 6965 6e74 556e 6974 733d    gradientUnits=
-00002b60: 2275 7365 7253 7061 6365 4f6e 5573 6522  "userSpaceOnUse"
-00002b70: 0d0a 2020 2020 2020 2067 7261 6469 656e  ..       gradien
-00002b80: 7454 7261 6e73 666f 726d 3d22 6d61 7472  tTransform="matr
-00002b90: 6978 2830 2e35 3632 3534 312c 302c 302c  ix(0.562541,0,0,
-00002ba0: 302e 3536 3739 3732 2c2d 392e 3339 3937  0.567972,-9.3997
-00002bb0: 3439 2c2d 352e 3330 3533 3137 2922 202f  49,-5.305317)" /
-00002bc0: 3e0d 0a20 2020 203c 7261 6469 616c 4772  >..    <radialGr
-00002bd0: 6164 6965 6e74 0d0a 2020 2020 2020 2063  adient..       c
-00002be0: 783d 2236 312e 3531 3838 3833 220d 0a20  x="61.518883".. 
-00002bf0: 2020 2020 2020 6379 3d22 3133 322e 3238        cy="132.28
-00002c00: 3537 3522 0d0a 2020 2020 2020 2072 3d22  575"..       r="
-00002c10: 3239 2e30 3336 3931 3322 0d0a 2020 2020  29.036913"..    
-00002c20: 2020 2066 783d 2236 312e 3531 3838 3833     fx="61.518883
-00002c30: 220d 0a20 2020 2020 2020 6679 3d22 3133  "..       fy="13
-00002c40: 322e 3238 3537 3522 0d0a 2020 2020 2020  2.28575"..      
-00002c50: 2069 643d 2272 6164 6961 6c47 7261 6469   id="radialGradi
-00002c60: 656e 7431 3438 3022 0d0a 2020 2020 2020  ent1480"..      
-00002c70: 2078 6c69 6e6b 3a68 7265 663d 2223 6c69   xlink:href="#li
-00002c80: 6e65 6172 4772 6164 6965 6e74 3237 3935  nearGradient2795
-00002c90: 220d 0a20 2020 2020 2020 6772 6164 6965  "..       gradie
-00002ca0: 6e74 556e 6974 733d 2275 7365 7253 7061  ntUnits="userSpa
-00002cb0: 6365 4f6e 5573 6522 0d0a 2020 2020 2020  ceOnUse"..      
-00002cc0: 2067 7261 6469 656e 7454 7261 6e73 666f   gradientTransfo
-00002cd0: 726d 3d22 6d61 7472 6978 2832 2e33 3832  rm="matrix(2.382
-00002ce0: 3731 3665 2d38 2c2d 302e 3239 3634 3035  716e-8,-0.296405
-00002cf0: 2c31 2e34 3336 3736 2c34 2e36 3833 3637  ,1.43676,4.68367
-00002d00: 3365 2d37 2c2d 3132 382e 3534 342c 3135  3e-7,-128.544,15
-00002d10: 302e 3532 3032 2922 202f 3e0d 0a20 2020  0.5202)" />..   
-00002d20: 203c 7261 6469 616c 4772 6164 6965 6e74   <radialGradient
-00002d30: 0d0a 2020 2020 2020 2069 6e6b 7363 6170  ..       inkscap
-00002d40: 653a 636f 6c6c 6563 743d 2261 6c77 6179  e:collect="alway
-00002d50: 7322 0d0a 2020 2020 2020 2078 6c69 6e6b  s"..       xlink
-00002d60: 3a68 7265 663d 2223 6c69 6e65 6172 4772  :href="#linearGr
-00002d70: 6164 6965 6e74 3237 3935 220d 0a20 2020  adient2795"..   
-00002d80: 2020 2020 6964 3d22 7261 6469 616c 4772      id="radialGr
-00002d90: 6164 6965 6e74 3234 3231 220d 0a20 2020  adient2421"..   
-00002da0: 2020 2020 6772 6164 6965 6e74 556e 6974      gradientUnit
-00002db0: 733d 2275 7365 7253 7061 6365 4f6e 5573  s="userSpaceOnUs
-00002dc0: 6522 0d0a 2020 2020 2020 2067 7261 6469  e"..       gradi
-00002dd0: 656e 7454 7261 6e73 666f 726d 3d22 6d61  entTransform="ma
-00002de0: 7472 6978 2831 2e37 3439 3035 3635 652d  trix(1.7490565e-
-00002df0: 382c 2d30 2e32 3339 3934 372c 312e 3035  8,-0.239947,1.05
-00002e00: 3436 3638 2c33 2e37 3931 3534 3537 652d  4668,3.7915457e-
-00002e10: 372c 2d37 382e 3130 3934 3239 2c31 3438  7,-78.109429,148
-00002e20: 2e38 3539 3036 2922 0d0a 2020 2020 2020  .85906)"..      
-00002e30: 2063 783d 2236 312e 3531 3838 3833 220d   cx="61.518883".
-00002e40: 0a20 2020 2020 2020 6379 3d22 3133 322e  .       cy="132.
-00002e50: 3238 3537 3522 0d0a 2020 2020 2020 2066  28575"..       f
-00002e60: 783d 2236 312e 3531 3838 3833 220d 0a20  x="61.518883".. 
-00002e70: 2020 2020 2020 6679 3d22 3133 322e 3238        fy="132.28
-00002e80: 3537 3522 0d0a 2020 2020 2020 2072 3d22  575"..       r="
-00002e90: 3239 2e30 3336 3931 3322 202f 3e0d 0a20  29.036913" />.. 
-00002ea0: 2020 203c 6c69 6e65 6172 4772 6164 6965     <linearGradie
-00002eb0: 6e74 0d0a 2020 2020 2020 2069 6e6b 7363  nt..       inksc
-00002ec0: 6170 653a 636f 6c6c 6563 743d 2261 6c77  ape:collect="alw
-00002ed0: 6179 7322 0d0a 2020 2020 2020 2078 6c69  ays"..       xli
-00002ee0: 6e6b 3a68 7265 663d 2223 6c69 6e65 6172  nk:href="#linear
-00002ef0: 4772 6164 6965 6e74 3436 3731 2d38 220d  Gradient4671-8".
-00002f00: 0a20 2020 2020 2020 6964 3d22 6c69 6e65  .       id="line
-00002f10: 6172 4772 6164 6965 6e74 3338 3236 2d36  arGradient3826-6
-00002f20: 220d 0a20 2020 2020 2020 7831 3d22 3336  "..       x1="36
-00002f30: 2e39 3730 3839 3822 0d0a 2020 2020 2020  .970898"..      
-00002f40: 2079 313d 2235 342e 3634 3637 3633 220d   y1="54.646763".
-00002f50: 0a20 2020 2020 2020 7832 3d22 3837 2e37  .       x2="87.7
-00002f60: 3034 3638 3122 0d0a 2020 2020 2020 2079  04681"..       y
-00002f70: 323d 2235 342e 3634 3637 3633 220d 0a20  2="54.646763".. 
-00002f80: 2020 2020 2020 6772 6164 6965 6e74 556e        gradientUn
-00002f90: 6974 733d 2275 7365 7253 7061 6365 4f6e  its="userSpaceOn
-00002fa0: 5573 6522 202f 3e0d 0a20 2020 203c 6c69  Use" />..    <li
-00002fb0: 6e65 6172 4772 6164 6965 6e74 0d0a 2020  nearGradient..  
-00002fc0: 2020 2020 2069 643d 226c 696e 6561 7247       id="linearG
-00002fd0: 7261 6469 656e 7434 3637 312d 3822 3e0d  radient4671-8">.
-00002fe0: 0a20 2020 2020 203c 7374 6f70 0d0a 2020  .      <stop..  
-00002ff0: 2020 2020 2020 2073 7479 6c65 3d22 7374         style="st
-00003000: 6f70 2d63 6f6c 6f72 3a23 6666 6434 3362  op-color:#ffd43b
-00003010: 3b73 746f 702d 6f70 6163 6974 793a 3122  ;stop-opacity:1"
-00003020: 0d0a 2020 2020 2020 2020 206f 6666 7365  ..         offse
-00003030: 743d 2230 220d 0a20 2020 2020 2020 2020  t="0"..         
-00003040: 6964 3d22 7374 6f70 3436 3733 2d38 2220  id="stop4673-8" 
-00003050: 2f3e 0d0a 2020 2020 2020 3c73 746f 700d  />..      <stop.
-00003060: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
-00003070: 2273 746f 702d 636f 6c6f 723a 2366 6665  "stop-color:#ffe
-00003080: 3837 333b 7374 6f70 2d6f 7061 6369 7479  873;stop-opacity
-00003090: 3a31 220d 0a20 2020 2020 2020 2020 6f66  :1"..         of
-000030a0: 6673 6574 3d22 3122 0d0a 2020 2020 2020  fset="1"..      
-000030b0: 2020 2069 643d 2273 746f 7034 3637 352d     id="stop4675-
-000030c0: 3222 202f 3e0d 0a20 2020 203c 2f6c 696e  2" />..    </lin
-000030d0: 6561 7247 7261 6469 656e 743e 0d0a 2020  earGradient>..  
-000030e0: 2020 3c6c 696e 6561 7247 7261 6469 656e    <linearGradien
-000030f0: 740d 0a20 2020 2020 2020 696e 6b73 6361  t..       inksca
-00003100: 7065 3a63 6f6c 6c65 6374 3d22 616c 7761  pe:collect="alwa
-00003110: 7973 220d 0a20 2020 2020 2020 786c 696e  ys"..       xlin
-00003120: 6b3a 6872 6566 3d22 236c 696e 6561 7247  k:href="#linearG
-00003130: 7261 6469 656e 7433 3831 3222 0d0a 2020  radient3812"..  
-00003140: 2020 2020 2069 643d 226c 696e 6561 7247       id="linearG
-00003150: 7261 6469 656e 7433 3831 3822 0d0a 2020  radient3818"..  
-00003160: 2020 2020 2078 313d 2237 382e 3031 3230       x1="78.0120
-00003170: 3234 220d 0a20 2020 2020 2020 7931 3d22  24"..       y1="
-00003180: 3830 2e33 3032 3933 3322 0d0a 2020 2020  80.302933"..    
-00003190: 2020 2078 323d 2231 3234 2e36 3739 3634     x2="124.67964
-000031a0: 220d 0a20 2020 2020 2020 7932 3d22 3238  "..       y2="28
-000031b0: 2e36 3033 3332 3722 0d0a 2020 2020 2020  .603327"..      
-000031c0: 2067 7261 6469 656e 7455 6e69 7473 3d22   gradientUnits="
-000031d0: 7573 6572 5370 6163 654f 6e55 7365 2220  userSpaceOnUse" 
-000031e0: 2f3e 0d0a 2020 2020 3c6c 696e 6561 7247  />..    <linearG
-000031f0: 7261 6469 656e 740d 0a20 2020 2020 2020  radient..       
-00003200: 696e 6b73 6361 7065 3a63 6f6c 6c65 6374  inkscape:collect
-00003210: 3d22 616c 7761 7973 220d 0a20 2020 2020  ="always"..     
-00003220: 2020 786c 696e 6b3a 6872 6566 3d22 236c    xlink:href="#l
-00003230: 696e 6561 7247 7261 6469 656e 7434 3637  inearGradient467
-00003240: 312d 3022 0d0a 2020 2020 2020 2069 643d  1-0"..       id=
-00003250: 226c 696e 6561 7247 7261 6469 656e 7434  "linearGradient4
-00003260: 3039 3722 0d0a 2020 2020 2020 2078 313d  097"..       x1=
-00003270: 222d 3230 352e 3035 3433 3122 0d0a 2020  "-205.05431"..  
-00003280: 2020 2020 2079 313d 2235 352e 3630 3634       y1="55.6064
-00003290: 3431 220d 0a20 2020 2020 2020 7832 3d22  41"..       x2="
-000032a0: 2d36 342e 3830 3632 3539 220d 0a20 2020  -64.806259"..   
-000032b0: 2020 2020 7932 3d22 3535 2e36 3036 3434      y2="55.60644
-000032c0: 3122 0d0a 2020 2020 2020 2067 7261 6469  1"..       gradi
-000032d0: 656e 7455 6e69 7473 3d22 7573 6572 5370  entUnits="userSp
-000032e0: 6163 654f 6e55 7365 2220 2f3e 0d0a 2020  aceOnUse" />..  
-000032f0: 2020 3c6c 696e 6561 7247 7261 6469 656e    <linearGradien
-00003300: 740d 0a20 2020 2020 2020 696e 6b73 6361  t..       inksca
-00003310: 7065 3a63 6f6c 6c65 6374 3d22 616c 7761  pe:collect="alwa
-00003320: 7973 220d 0a20 2020 2020 2020 786c 696e  ys"..       xlin
-00003330: 6b3a 6872 6566 3d22 236c 696e 6561 7247  k:href="#linearG
-00003340: 7261 6469 656e 7434 3638 392d 3922 0d0a  radient4689-9"..
-00003350: 2020 2020 2020 2069 643d 226c 696e 6561         id="linea
-00003360: 7247 7261 6469 656e 7434 3337 3722 0d0a  rGradient4377"..
-00003370: 2020 2020 2020 2067 7261 6469 656e 7455         gradientU
-00003380: 6e69 7473 3d22 7573 6572 5370 6163 654f  nits="userSpaceO
-00003390: 6e55 7365 220d 0a20 2020 2020 2020 6772  nUse"..       gr
-000033a0: 6164 6965 6e74 5472 616e 7366 6f72 6d3d  adientTransform=
-000033b0: 226d 6174 7269 7828 302e 3536 3235 3431  "matrix(0.562541
-000033c0: 2c30 2c30 2c30 2e35 3637 3937 322c 2d39  ,0,0,0.567972,-9
-000033d0: 2e33 3939 3734 392c 2d35 2e33 3035 3331  .399749,-5.30531
-000033e0: 3729 220d 0a20 2020 2020 2020 7831 3d22  7)"..       x1="
-000033f0: 3236 2e36 3438 3933 3722 0d0a 2020 2020  26.648937"..    
-00003400: 2020 2079 313d 2232 302e 3630 3337 3831     y1="20.603781
-00003410: 220d 0a20 2020 2020 2020 7832 3d22 3133  "..       x2="13
-00003420: 352e 3636 3532 3522 0d0a 2020 2020 2020  5.66525"..      
-00003430: 2079 323d 2231 3134 2e33 3937 3637 2220   y2="114.39767" 
-00003440: 2f3e 0d0a 2020 2020 3c6c 696e 6561 7247  />..    <linearG
-00003450: 7261 6469 656e 740d 0a20 2020 2020 2020  radient..       
-00003460: 6964 3d22 6c69 6e65 6172 4772 6164 6965  id="linearGradie
-00003470: 6e74 3436 3839 2d39 223e 0d0a 2020 2020  nt4689-9">..    
-00003480: 2020 3c73 746f 700d 0a20 2020 2020 2020    <stop..       
-00003490: 2020 7374 796c 653d 2273 746f 702d 636f    style="stop-co
-000034a0: 6c6f 723a 2335 6139 6664 343b 7374 6f70  lor:#5a9fd4;stop
-000034b0: 2d6f 7061 6369 7479 3a31 220d 0a20 2020  -opacity:1"..   
-000034c0: 2020 2020 2020 6f66 6673 6574 3d22 3022        offset="0"
-000034d0: 0d0a 2020 2020 2020 2020 2069 643d 2273  ..         id="s
-000034e0: 746f 7034 3639 312d 3422 202f 3e0d 0a20  top4691-4" />.. 
-000034f0: 2020 2020 203c 7374 6f70 0d0a 2020 2020       <stop..    
-00003500: 2020 2020 2073 7479 6c65 3d22 7374 6f70       style="stop
-00003510: 2d63 6f6c 6f72 3a23 3330 3639 3938 3b73  -color:#306998;s
-00003520: 746f 702d 6f70 6163 6974 793a 3122 0d0a  top-opacity:1"..
-00003530: 2020 2020 2020 2020 206f 6666 7365 743d           offset=
-00003540: 2231 220d 0a20 2020 2020 2020 2020 6964  "1"..         id
-00003550: 3d22 7374 6f70 3436 3933 2d36 2220 2f3e  ="stop4693-6" />
-00003560: 0d0a 2020 2020 3c2f 6c69 6e65 6172 4772  ..    </linearGr
-00003570: 6164 6965 6e74 3e0d 0a20 2020 203c 6c69  adient>..    <li
-00003580: 6e65 6172 4772 6164 6965 6e74 0d0a 2020  nearGradient..  
-00003590: 2020 2020 2069 6e6b 7363 6170 653a 636f       inkscape:co
-000035a0: 6c6c 6563 743d 2261 6c77 6179 7322 0d0a  llect="always"..
-000035b0: 2020 2020 2020 2078 6c69 6e6b 3a68 7265         xlink:hre
-000035c0: 663d 2223 6c69 6e65 6172 4772 6164 6965  f="#linearGradie
-000035d0: 6e74 3436 3731 2d30 220d 0a20 2020 2020  nt4671-0"..     
-000035e0: 2020 6964 3d22 6c69 6e65 6172 4772 6164    id="linearGrad
-000035f0: 6965 6e74 3433 3734 220d 0a20 2020 2020  ient4374"..     
-00003600: 2020 6772 6164 6965 6e74 556e 6974 733d    gradientUnits=
-00003610: 2275 7365 7253 7061 6365 4f6e 5573 6522  "userSpaceOnUse"
-00003620: 0d0a 2020 2020 2020 2067 7261 6469 656e  ..       gradien
-00003630: 7454 7261 6e73 666f 726d 3d22 6d61 7472  tTransform="matr
-00003640: 6978 2830 2e35 3632 3534 312c 302c 302c  ix(0.562541,0,0,
-00003650: 302e 3536 3739 3732 2c2d 392e 3339 3937  0.567972,-9.3997
-00003660: 3439 2c2d 352e 3330 3533 3137 2922 0d0a  49,-5.305317)"..
-00003670: 2020 2020 2020 2078 313d 2231 3530 2e39         x1="150.9
-00003680: 3631 3131 220d 0a20 2020 2020 2020 7931  6111"..       y1
-00003690: 3d22 3139 322e 3335 3137 3622 0d0a 2020  ="192.35176"..  
-000036a0: 2020 2020 2078 323d 2231 3132 2e30 3331       x2="112.031
-000036b0: 3434 220d 0a20 2020 2020 2020 7932 3d22  44"..       y2="
-000036c0: 3133 372e 3237 3239 3922 202f 3e0d 0a20  137.27299" />.. 
-000036d0: 2020 203c 6c69 6e65 6172 4772 6164 6965     <linearGradie
-000036e0: 6e74 0d0a 2020 2020 2020 2069 643d 226c  nt..       id="l
-000036f0: 696e 6561 7247 7261 6469 656e 7434 3637  inearGradient467
-00003700: 312d 3022 3e0d 0a20 2020 2020 203c 7374  1-0">..      <st
-00003710: 6f70 0d0a 2020 2020 2020 2020 2073 7479  op..         sty
-00003720: 6c65 3d22 7374 6f70 2d63 6f6c 6f72 3a23  le="stop-color:#
-00003730: 6666 6434 3362 3b73 746f 702d 6f70 6163  ffd43b;stop-opac
-00003740: 6974 793a 3122 0d0a 2020 2020 2020 2020  ity:1"..        
-00003750: 206f 6666 7365 743d 2230 220d 0a20 2020   offset="0"..   
-00003760: 2020 2020 2020 6964 3d22 7374 6f70 3436        id="stop46
-00003770: 3733 2d33 2220 2f3e 0d0a 2020 2020 2020  73-3" />..      
-00003780: 3c73 746f 700d 0a20 2020 2020 2020 2020  <stop..         
-00003790: 7374 796c 653d 2273 746f 702d 636f 6c6f  style="stop-colo
-000037a0: 723a 2366 6665 3837 333b 7374 6f70 2d6f  r:#ffe873;stop-o
-000037b0: 7061 6369 7479 3a31 220d 0a20 2020 2020  pacity:1"..     
-000037c0: 2020 2020 6f66 6673 6574 3d22 3122 0d0a      offset="1"..
-000037d0: 2020 2020 2020 2020 2069 643d 2273 746f           id="sto
-000037e0: 7034 3637 352d 3622 202f 3e0d 0a20 2020  p4675-6" />..   
-000037f0: 203c 2f6c 696e 6561 7247 7261 6469 656e   </linearGradien
-00003800: 743e 0d0a 2020 2020 3c72 6164 6961 6c47  t>..    <radialG
-00003810: 7261 6469 656e 740d 0a20 2020 2020 2020  radient..       
-00003820: 696e 6b73 6361 7065 3a63 6f6c 6c65 6374  inkscape:collect
-00003830: 3d22 616c 7761 7973 220d 0a20 2020 2020  ="always"..     
-00003840: 2020 786c 696e 6b3a 6872 6566 3d22 236c    xlink:href="#l
-00003850: 696e 6561 7247 7261 6469 656e 7432 3739  inearGradient279
-00003860: 352d 3222 0d0a 2020 2020 2020 2069 643d  5-2"..       id=
-00003870: 2272 6164 6961 6c47 7261 6469 656e 7434  "radialGradient4
-00003880: 3337 3022 0d0a 2020 2020 2020 2067 7261  370"..       gra
-00003890: 6469 656e 7455 6e69 7473 3d22 7573 6572  dientUnits="user
-000038a0: 5370 6163 654f 6e55 7365 220d 0a20 2020  SpaceOnUse"..   
-000038b0: 2020 2020 6772 6164 6965 6e74 5472 616e      gradientTran
-000038c0: 7366 6f72 6d3d 226d 6174 7269 7828 312e  sform="matrix(1.
-000038d0: 3734 3930 3536 3565 2d38 2c2d 302e 3233  7490565e-8,-0.23
-000038e0: 3939 3436 3936 2c31 2e30 3534 3636 382c  994696,1.054668,
-000038f0: 332e 3739 3135 3435 3765 2d37 2c2d 3738  3.7915457e-7,-78
-00003900: 2e31 3039 3432 392c 3134 382e 3835 3930  .109429,148.8590
-00003910: 3629 220d 0a20 2020 2020 2020 6378 3d22  6)"..       cx="
-00003920: 3631 2e35 3138 3838 3322 0d0a 2020 2020  61.518883"..    
-00003930: 2020 2063 793d 2231 3332 2e32 3835 3735     cy="132.28575
-00003940: 220d 0a20 2020 2020 2020 6678 3d22 3631  "..       fx="61
-00003950: 2e35 3138 3838 3322 0d0a 2020 2020 2020  .518883"..      
-00003960: 2066 793d 2231 3332 2e32 3835 3735 220d   fy="132.28575".
-00003970: 0a20 2020 2020 2020 723d 2232 392e 3033  .       r="29.03
-00003980: 3639 3133 2220 2f3e 0d0a 2020 2020 3c6c  6913" />..    <l
-00003990: 696e 6561 7247 7261 6469 656e 740d 0a20  inearGradient.. 
-000039a0: 2020 2020 2020 6964 3d22 6c69 6e65 6172        id="linear
-000039b0: 4772 6164 6965 6e74 3237 3935 2d32 223e  Gradient2795-2">
-000039c0: 0d0a 2020 2020 2020 3c73 746f 700d 0a20  ..      <stop.. 
-000039d0: 2020 2020 2020 2020 7374 796c 653d 2273          style="s
-000039e0: 746f 702d 636f 6c6f 723a 2362 3862 3862  top-color:#b8b8b
-000039f0: 383b 7374 6f70 2d6f 7061 6369 7479 3a30  8;stop-opacity:0
-00003a00: 2e34 3938 3033 3932 3222 0d0a 2020 2020  .49803922"..    
-00003a10: 2020 2020 206f 6666 7365 743d 2230 220d       offset="0".
-00003a20: 0a20 2020 2020 2020 2020 6964 3d22 7374  .         id="st
-00003a30: 6f70 3237 3937 2d34 2220 2f3e 0d0a 2020  op2797-4" />..  
-00003a40: 2020 2020 3c73 746f 700d 0a20 2020 2020      <stop..     
-00003a50: 2020 2020 7374 796c 653d 2273 746f 702d      style="stop-
-00003a60: 636f 6c6f 723a 2337 6637 6637 663b 7374  color:#7f7f7f;st
-00003a70: 6f70 2d6f 7061 6369 7479 3a30 220d 0a20  op-opacity:0".. 
-00003a80: 2020 2020 2020 2020 6f66 6673 6574 3d22          offset="
-00003a90: 3122 0d0a 2020 2020 2020 2020 2069 643d  1"..         id=
-00003aa0: 2273 746f 7032 3739 392d 3522 202f 3e0d  "stop2799-5" />.
-00003ab0: 0a20 2020 203c 2f6c 696e 6561 7247 7261  .    </linearGra
-00003ac0: 6469 656e 743e 0d0a 2020 2020 3c72 6164  dient>..    <rad
-00003ad0: 6961 6c47 7261 6469 656e 740d 0a20 2020  ialGradient..   
-00003ae0: 2020 2020 723d 2232 392e 3033 3639 3133      r="29.036913
-00003af0: 220d 0a20 2020 2020 2020 6679 3d22 3133  "..       fy="13
-00003b00: 322e 3238 3537 3522 0d0a 2020 2020 2020  2.28575"..      
-00003b10: 2066 783d 2236 312e 3531 3838 3833 220d   fx="61.518883".
-00003b20: 0a20 2020 2020 2020 6379 3d22 3133 322e  .       cy="132.
-00003b30: 3238 3537 3522 0d0a 2020 2020 2020 2063  28575"..       c
-00003b40: 783d 2236 312e 3531 3838 3833 220d 0a20  x="61.518883".. 
-00003b50: 2020 2020 2020 6772 6164 6965 6e74 5472        gradientTr
-00003b60: 616e 7366 6f72 6d3d 226d 6174 7269 7828  ansform="matrix(
-00003b70: 312e 3734 3930 3536 3565 2d38 2c2d 302e  1.7490565e-8,-0.
-00003b80: 3233 3939 3436 3936 2c31 2e30 3534 3636  23994696,1.05466
-00003b90: 382c 332e 3739 3135 3435 3765 2d37 2c2d  8,3.7915457e-7,-
-00003ba0: 3738 2e31 3039 3432 392c 3134 382e 3835  78.109429,148.85
-00003bb0: 3930 3629 220d 0a20 2020 2020 2020 6772  906)"..       gr
-00003bc0: 6164 6965 6e74 556e 6974 733d 2275 7365  adientUnits="use
-00003bd0: 7253 7061 6365 4f6e 5573 6522 0d0a 2020  rSpaceOnUse"..  
-00003be0: 2020 2020 2069 643d 2272 6164 6961 6c47       id="radialG
-00003bf0: 7261 6469 656e 7434 3431 3622 0d0a 2020  radient4416"..  
-00003c00: 2020 2020 2078 6c69 6e6b 3a68 7265 663d       xlink:href=
-00003c10: 2223 6c69 6e65 6172 4772 6164 6965 6e74  "#linearGradient
-00003c20: 3237 3935 2d32 220d 0a20 2020 2020 2020  2795-2"..       
-00003c30: 696e 6b73 6361 7065 3a63 6f6c 6c65 6374  inkscape:collect
-00003c40: 3d22 616c 7761 7973 2220 2f3e 0d0a 2020  ="always" />..  
-00003c50: 2020 3c72 6164 6961 6c47 7261 6469 656e    <radialGradien
-00003c60: 740d 0a20 2020 2020 2020 696e 6b73 6361  t..       inksca
-00003c70: 7065 3a63 6f6c 6c65 6374 3d22 616c 7761  pe:collect="alwa
-00003c80: 7973 220d 0a20 2020 2020 2020 786c 696e  ys"..       xlin
-00003c90: 6b3a 6872 6566 3d22 236c 696e 6561 7247  k:href="#linearG
-00003ca0: 7261 6469 656e 7432 3739 352d 3222 0d0a  radient2795-2"..
-00003cb0: 2020 2020 2020 2069 643d 2272 6164 6961         id="radia
-00003cc0: 6c47 7261 6469 656e 7434 3435 3822 0d0a  lGradient4458"..
-00003cd0: 2020 2020 2020 2067 7261 6469 656e 7455         gradientU
-00003ce0: 6e69 7473 3d22 7573 6572 5370 6163 654f  nits="userSpaceO
-00003cf0: 6e55 7365 220d 0a20 2020 2020 2020 6772  nUse"..       gr
-00003d00: 6164 6965 6e74 5472 616e 7366 6f72 6d3d  adientTransform=
-00003d10: 226d 6174 7269 7828 312e 3238 3634 3032  "matrix(1.286402
-00003d20: 3665 2d38 2c2d 302e 3137 3634 3737 3039  6e-8,-0.17647709
-00003d30: 2c30 2e37 3735 3639 3131 372c 322e 3738  ,0.77569117,2.78
-00003d40: 3836 3230 3265 2d37 2c2d 3236 2e34 3638  86202e-7,-26.468
-00003d50: 3130 352c 3132 362e 3738 3430 3329 220d  105,126.78403)".
-00003d60: 0a20 2020 2020 2020 6378 3d22 3631 2e35  .       cx="61.5
-00003d70: 3138 3838 3322 0d0a 2020 2020 2020 2063  18883"..       c
-00003d80: 793d 2231 3332 2e32 3835 3735 220d 0a20  y="132.28575".. 
-00003d90: 2020 2020 2020 6678 3d22 3631 2e35 3138        fx="61.518
-00003da0: 3838 3322 0d0a 2020 2020 2020 2066 793d  883"..       fy=
-00003db0: 2231 3332 2e32 3835 3735 220d 0a20 2020  "132.28575"..   
-00003dc0: 2020 2020 723d 2232 392e 3033 3639 3133      r="29.036913
-00003dd0: 2220 2f3e 0d0a 2020 2020 3c6c 696e 6561  " />..    <linea
-00003de0: 7247 7261 6469 656e 740d 0a20 2020 2020  rGradient..     
-00003df0: 2020 696e 6b73 6361 7065 3a63 6f6c 6c65    inkscape:colle
-00003e00: 6374 3d22 616c 7761 7973 220d 0a20 2020  ct="always"..   
-00003e10: 2020 2020 786c 696e 6b3a 6872 6566 3d22      xlink:href="
-00003e20: 236c 696e 6561 7247 7261 6469 656e 7436  #linearGradient6
-00003e30: 3438 3122 0d0a 2020 2020 2020 2069 643d  481"..       id=
-00003e40: 226c 696e 6561 7247 7261 6469 656e 7436  "linearGradient6
-00003e50: 3437 3922 0d0a 2020 2020 2020 2078 313d  479"..       x1=
-00003e60: 222d 3135 382e 3636 3734 220d 0a20 2020  "-158.6674"..   
-00003e70: 2020 2020 7931 3d22 3436 2e31 3437 3833      y1="46.14783
-00003e80: 3522 0d0a 2020 2020 2020 2078 323d 222d  5"..       x2="-
-00003e90: 3738 2e37 3737 3035 3422 0d0a 2020 2020  78.777054"..    
-00003ea0: 2020 2079 323d 2234 362e 3134 3738 3335     y2="46.147835
-00003eb0: 220d 0a20 2020 2020 2020 6772 6164 6965  "..       gradie
-00003ec0: 6e74 556e 6974 733d 2275 7365 7253 7061  ntUnits="userSpa
-00003ed0: 6365 4f6e 5573 6522 0d0a 2020 2020 2020  ceOnUse"..      
-00003ee0: 2067 7261 6469 656e 7454 7261 6e73 666f   gradientTransfo
-00003ef0: 726d 3d22 6d61 7472 6978 2832 2e30 3630  rm="matrix(2.060
-00003f00: 3039 3838 2c30 2c30 2c32 2e30 3630 3039  0988,0,0,2.06009
-00003f10: 3838 2c32 3933 2e33 3532 3832 2c31 352e  88,293.35282,15.
-00003f20: 3432 3535 3237 2922 202f 3e0d 0a20 203c  425527)" />..  <
-00003f30: 2f64 6566 733e 0d0a 2020 3c70 6174 680d  /defs>..  <path.
-00003f40: 0a20 2020 2020 736f 6469 706f 6469 3a74  .     sodipodi:t
-00003f50: 7970 653d 2261 7263 220d 0a20 2020 2020  ype="arc"..     
-00003f60: 7374 796c 653d 2266 696c 6c3a 7572 6c28  style="fill:url(
-00003f70: 236c 696e 6561 7247 7261 6469 656e 7434  #linearGradient4
-00003f80: 3039 3729 3b73 7472 6f6b 653a 6e6f 6e65  097);stroke:none
-00003f90: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
-00003fa0: 313b 6669 6c6c 2d6f 7061 6369 7479 3a31  1;fill-opacity:1
-00003fb0: 2e30 220d 0a20 2020 2020 6964 3d22 7061  .0"..     id="pa
-00003fc0: 7468 3430 3839 220d 0a20 2020 2020 736f  th4089"..     so
-00003fd0: 6469 706f 6469 3a63 783d 222d 3133 342e  dipodi:cx="-134.
-00003fe0: 3933 3032 3822 0d0a 2020 2020 2073 6f64  93028"..     sod
-00003ff0: 6970 6f64 693a 6379 3d22 3535 2e36 3036  ipodi:cy="55.606
-00004000: 3434 3122 0d0a 2020 2020 2073 6f64 6970  441"..     sodip
-00004010: 6f64 693a 7278 3d22 3639 2e36 3234 3032  odi:rx="69.62402
-00004020: 3322 0d0a 2020 2020 2073 6f64 6970 6f64  3"..     sodipod
-00004030: 693a 7279 3d22 3531 2e35 3433 3336 3922  i:ry="51.543369"
-00004040: 0d0a 2020 2020 2064 3d22 6d20 2d36 352e  ..     d="m -65.
-00004050: 3330 3632 3539 2c35 352e 3630 3634 3431  306259,55.606441
-00004060: 2061 2036 392e 3632 3430 3233 2c35 312e   a 69.624023,51.
-00004070: 3534 3333 3639 2030 2031 2031 202d 3133  543369 0 1 1 -13
-00004080: 392e 3234 3830 3531 2c30 2036 392e 3632  9.248051,0 69.62
-00004090: 3430 3233 2c35 312e 3534 3333 3639 2030  4023,51.543369 0
-000040a0: 2031 2031 2031 3339 2e32 3438 3035 312c   1 1 139.248051,
-000040b0: 3020 7a22 0d0a 2020 2020 2074 7261 6e73  0 z"..     trans
-000040c0: 666f 726d 3d22 7472 616e 736c 6174 6528  form="translate(
-000040d0: 3231 312e 3033 3039 362c 382e 3633 3535  211.03096,8.6355
-000040e0: 3338 2922 202f 3e0d 0a20 203c 7061 7468  38)" />..  <path
-000040f0: 0d0a 2020 2020 2069 6e6b 7363 6170 653a  ..     inkscape:
-00004100: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
-00004110: 7572 653d 2230 220d 0a20 2020 2020 643d  ure="0"..     d=
-00004120: 226d 2037 362e 3331 3631 3236 2c32 372e  "m 76.316126,27.
-00004130: 3430 3435 3937 2063 202d 392e 3136 3730  404597 c -9.1670
-00004140: 3039 2c30 2e30 3432 3537 202d 3137 2e39  09,0.04257 -17.9
-00004150: 3231 3238 382c 302e 3832 3434 3032 202d  21288,0.824402 -
-00004160: 3235 2e36 3234 3134 362c 322e 3138 3734  25.624146,2.1874
-00004170: 3234 202d 3232 2e36 3931 3636 2c34 2e30  24 -22.69166,4.0
-00004180: 3038 3837 202d 3236 2e38 3131 3539 352c  0887 -26.811595,
-00004190: 3132 2e33 3939 3738 3720 2d32 362e 3831  12.399787 -26.81
-000041a0: 3135 3935 2c32 372e 3837 3430 3631 206c  1595,27.874061 l
-000041b0: 2030 2c32 302e 3433 3638 3134 2035 332e   0,20.436814 53.
-000041c0: 3632 3331 3836 2c30 2030 2c36 2e38 3132  623186,0 0,6.812
-000041d0: 3236 3920 2d33 2e33 3339 3730 322c 3333  269 -3.339702,33
-000041e0: 2e39 3132 3131 3520 3530 2e37 3430 3930  .912115 50.74090
-000041f0: 312c 2d31 322e 3832 3236 3420 6320 342e  1,-12.82264 c 4.
-00004200: 3933 3536 342c 302e 3130 3538 3420 3131  93564,0.10584 11
-00004210: 2e34 3231 3735 2c2d 362e 3332 3839 3139  .42175,-6.328919
-00004220: 2036 2e31 3539 3532 2c2d 3438 2e33 3338   6.15952,-48.338
-00004230: 3535 3820 302c 2d31 342e 3533 3231 3837  558 0,-14.532187
-00004240: 202d 3132 2e32 3539 3535 2c2d 3235 2e34   -12.25955,-25.4
-00004250: 3438 3639 3820 2d32 362e 3831 3136 312c  48698 -26.81161,
-00004260: 2d32 372e 3837 3430 3631 2043 2039 352e  -27.874061 C 95.
-00004270: 3034 3130 3331 2c32 382e 3035 3836 3220  041031,28.05862 
-00004280: 3835 2e34 3833 3131 322c 3237 2e33 3631  85.483112,27.361
-00004290: 3939 3520 3736 2e33 3136 3132 362c 3237  995 76.316126,27
-000042a0: 2e34 3034 3539 3720 7a20 4d20 3437 2e33  .404597 z M 47.3
-000042b0: 3137 3131 332c 3433 2e38 3431 3534 3320  17113,43.841543 
-000042c0: 6320 352e 3533 3838 3936 2c30 2031 302e  c 5.538896,0 10.
-000042d0: 3036 3231 3435 2c34 2e35 3937 3133 3820  062145,4.597138 
-000042e0: 3130 2e30 3632 3134 352c 3130 2e32 3439  10.062145,10.249
-000042f0: 3635 3220 302c 352e 3633 3234 3835 202d  652 0,5.632485 -
-00004300: 342e 3532 3332 3439 2c31 302e 3138 3731  4.523249,10.1871
-00004310: 3539 202d 3130 2e30 3632 3134 352c 3130  59 -10.062145,10
-00004320: 2e31 3837 3135 3920 2d35 2e35 3538 3738  .187159 -5.55878
-00004330: 372c 2d32 652d 3620 2d31 302e 3036 3231  7,-2e-6 -10.0621
-00004340: 3633 2c2d 342e 3535 3436 3734 202d 3130  63,-4.554674 -10
-00004350: 2e30 3632 3136 332c 2d31 302e 3138 3731  .062163,-10.1871
-00004360: 3539 202d 332e 3265 2d35 2c2d 352e 3635  59 -3.2e-5,-5.65
-00004370: 3235 3134 2034 2e35 3033 3337 362c 2d31  2514 4.503376,-1
-00004380: 302e 3234 3936 3532 2031 302e 3036 3231  0.249652 10.0621
-00004390: 3633 2c2d 3130 2e32 3439 3635 3220 7a22  63,-10.249652 z"
-000043a0: 0d0a 2020 2020 2073 7479 6c65 3d22 6669  ..     style="fi
-000043b0: 6c6c 3a75 726c 2823 6c69 6e65 6172 4772  ll:url(#linearGr
-000043c0: 6164 6965 6e74 3634 3739 293b 6669 6c6c  adient6479);fill
-000043d0: 2d6f 7061 6369 7479 3a31 3b66 696c 6c2d  -opacity:1;fill-
-000043e0: 7275 6c65 3a6e 6f6e 7a65 726f 220d 0a20  rule:nonzero".. 
-000043f0: 2020 2020 6964 3d22 7061 7468 3139 3438      id="path1948
-00004400: 220d 0a20 2020 2020 736f 6469 706f 6469  "..     sodipodi
-00004410: 3a6e 6f64 6574 7970 6573 3d22 7363 7363  :nodetypes="scsc
-00004420: 6363 6363 6363 7373 7373 7373 2220 2f3e  ccccccssssss" />
-00004430: 0d0a 2020 3c70 6174 680d 0a20 2020 2020  ..  <path..     
-00004440: 7374 796c 653d 2266 6f6e 742d 7369 7a65  style="font-size
-00004450: 3a6d 6564 6975 6d3b 666f 6e74 2d73 7479  :medium;font-sty
-00004460: 6c65 3a6e 6f72 6d61 6c3b 666f 6e74 2d76  le:normal;font-v
-00004470: 6172 6961 6e74 3a6e 6f72 6d61 6c3b 666f  ariant:normal;fo
-00004480: 6e74 2d77 6569 6768 743a 6e6f 726d 616c  nt-weight:normal
-00004490: 3b66 6f6e 742d 7374 7265 7463 683a 6e6f  ;font-stretch:no
-000044a0: 726d 616c 3b74 6578 742d 696e 6465 6e74  rmal;text-indent
-000044b0: 3a30 3b74 6578 742d 616c 6967 6e3a 7374  :0;text-align:st
-000044c0: 6172 743b 7465 7874 2d64 6563 6f72 6174  art;text-decorat
-000044d0: 696f 6e3a 6e6f 6e65 3b6c 696e 652d 6865  ion:none;line-he
-000044e0: 6967 6874 3a6e 6f72 6d61 6c3b 6c65 7474  ight:normal;lett
-000044f0: 6572 2d73 7061 6369 6e67 3a6e 6f72 6d61  er-spacing:norma
-00004500: 6c3b 776f 7264 2d73 7061 6369 6e67 3a6e  l;word-spacing:n
-00004510: 6f72 6d61 6c3b 7465 7874 2d74 7261 6e73  ormal;text-trans
-00004520: 666f 726d 3a6e 6f6e 653b 6469 7265 6374  form:none;direct
-00004530: 696f 6e3a 6c74 723b 626c 6f63 6b2d 7072  ion:ltr;block-pr
-00004540: 6f67 7265 7373 696f 6e3a 7462 3b77 7269  ogression:tb;wri
-00004550: 7469 6e67 2d6d 6f64 653a 6c72 2d74 623b  ting-mode:lr-tb;
-00004560: 7465 7874 2d61 6e63 686f 723a 7374 6172  text-anchor:star
-00004570: 743b 6261 7365 6c69 6e65 2d73 6869 6674  t;baseline-shift
-00004580: 3a62 6173 656c 696e 653b 636f 6c6f 723a  :baseline;color:
-00004590: 2330 3030 3030 303b 6669 6c6c 3a23 6462  #000000;fill:#db
-000045a0: 3934 3566 3b66 696c 6c2d 6f70 6163 6974  945f;fill-opacit
-000045b0: 793a 313b 6669 6c6c 2d72 756c 653a 6e6f  y:1;fill-rule:no
-000045c0: 6e7a 6572 6f3b 7374 726f 6b65 3a6e 6f6e  nzero;stroke:non
-000045d0: 653b 7374 726f 6b65 2d77 6964 7468 3a39  e;stroke-width:9
-000045e0: 2e35 3835 3030 3030 3030 3030 3030 3030  .585000000000000
-000045f0: 3930 3b6d 6172 6b65 723a 6e6f 6e65 3b76  90;marker:none;v
-00004600: 6973 6962 696c 6974 793a 7669 7369 626c  isibility:visibl
-00004610: 653b 6469 7370 6c61 793a 696e 6c69 6e65  e;display:inline
-00004620: 3b6f 7665 7266 6c6f 773a 7669 7369 626c  ;overflow:visibl
-00004630: 653b 656e 6162 6c65 2d62 6163 6b67 726f  e;enable-backgro
-00004640: 756e 643a 6163 6375 6d75 6c61 7465 3b66  und:accumulate;f
-00004650: 6f6e 742d 6661 6d69 6c79 3a53 616e 733b  ont-family:Sans;
-00004660: 2d69 6e6b 7363 6170 652d 666f 6e74 2d73  -inkscape-font-s
-00004670: 7065 6369 6669 6361 7469 6f6e 3a53 616e  pecification:San
-00004680: 733b 6f70 6163 6974 793a 313b 7374 726f  s;opacity:1;stro
-00004690: 6b65 2d6f 7061 6369 7479 3a31 3b73 7472  ke-opacity:1;str
-000046a0: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
-000046b0: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
-000046c0: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6c69  y:none;stroke-li
-000046d0: 6e65 6a6f 696e 3a72 6f75 6e64 3b73 7472  nejoin:round;str
-000046e0: 6f6b 652d 6c69 6e65 6361 703a 726f 756e  oke-linecap:roun
-000046f0: 6422 0d0a 2020 2020 2064 3d22 6d20 3737  d"..     d="m 77
-00004700: 2e33 3036 3835 312c 382e 3136 3934 3732  .306851,8.169472
-00004710: 3320 6320 2d34 322e 3531 3035 3531 2c30  3 c -42.510551,0
-00004720: 202d 3737 2e34 3133 3732 312c 3230 2e30   -77.413721,20.0
-00004730: 3636 3234 3637 202d 3737 2e34 3133 3732  662467 -77.41372
-00004740: 312c 3533 2e32 3132 3033 3537 2030 2c38  1,53.2120357 0,8
-00004750: 2e32 3836 3434 3720 322e 3134 3737 3135  .286447 2.147715
-00004760: 362c 3136 2e31 3935 3531 3620 362e 3033  6,16.195516 6.03
-00004770: 3335 3136 332c 3233 2e33 3937 3939 3320  35163,23.397993 
-00004780: 332e 3838 3538 3030 372c 372e 3230 3234  3.8858007,7.2024
-00004790: 3738 2039 2e35 3039 3638 3637 2c31 332e  78 9.5096867,13.
-000047a0: 3639 3833 3633 2031 362e 3436 3230 3236  698363 16.462026
-000047b0: 372c 3139 2e31 3538 3433 3920 362e 3935  7,19.158439 6.95
-000047c0: 3233 3431 2c35 2e34 3630 3038 2031 352e  2341,5.46008 15.
-000047d0: 3233 3331 3336 2c39 2e38 3834 3336 2032  233136,9.88436 2
-000047e0: 342e 3433 3237 3536 2c31 322e 3934 3336  4.432756,12.9436
-000047f0: 3120 392e 3139 3936 3139 2c33 2e30 3539  1 9.199619,3.059
-00004800: 3236 2034 322e 3532 3630 3731 2c33 312e  26 42.526071,31.
-00004810: 3139 3938 3320 3533 2e31 3533 3730 392c  19983 53.153709,
-00004820: 3331 2e31 3939 3833 2035 2e33 3133 3832  31.19983 5.31382
-00004830: 322c 3020 2d32 312e 3132 3134 3732 2c2d  2,0 -21.121472,-
-00004840: 3134 2e30 3535 3733 202d 3138 2e32 3232  14.05573 -18.222
-00004850: 3738 322c 2d32 302e 3932 3933 3520 322e  782,-20.92935 2.
-00004860: 3434 3532 3532 2c2d 352e 3739 3833 3820  445252,-5.79838 
-00004870: 3230 2e33 3634 3330 342c 2d38 2e37 3430  20.364304,-8.740
-00004880: 3835 2032 342e 3936 3536 3734 2c2d 3130  85 24.965674,-10
-00004890: 2e32 3730 3438 2039 2e32 3032 3733 2c2d  .27048 9.20273,-
-000048a0: 332e 3035 3932 3620 3137 2e34 3837 3638  3.05926 17.48768
-000048b0: 2c2d 372e 3438 3335 3320 3234 2e34 3434  ,-7.48353 24.444
-000048c0: 3138 2c2d 3132 2e39 3433 3631 2036 2e39  18,-12.94361 6.9
-000048d0: 3536 352c 2d35 2e34 3630 3037 3620 3132  565,-5.460076 12
-000048e0: 2e35 3834 3534 2c2d 3131 2e39 3535 3936  .58454,-11.95596
-000048f0: 3120 3136 2e34 3733 3436 2c2d 3139 2e31  1 16.47346,-19.1
-00004900: 3538 3433 3920 332e 3838 3839 322c 2d37  58439 3.88892,-7
-00004910: 2e32 3032 3437 3720 362e 3033 3837 312c  .202477 6.03871,
-00004920: 2d31 352e 3131 3135 3436 2036 2e30 3338  -15.111546 6.038
-00004930: 3731 2c2d 3233 2e33 3937 3939 3320 302c  71,-23.397993 0,
-00004940: 2d33 332e 3134 3537 3839 202d 3333 2e38  -33.145789 -33.8
-00004950: 3536 3938 2c2d 3533 2e32 3132 3033 3537  5698,-53.2120357
-00004960: 202d 3736 2e33 3637 3532 392c 2d35 332e   -76.367529,-53.
-00004970: 3231 3230 3335 3720 7a20 6d20 302e 3533  2120357 z m 0.53
-00004980: 3937 3231 2c36 2e36 3331 3230 3037 2063  9721,6.6312007 c
-00004990: 2033 362e 3737 3836 3538 2c30 2036 352e   36.778658,0 65.
-000049a0: 3632 3030 3538 2c31 372e 3433 3831 3031  620058,17.438101
-000049b0: 2036 352e 3632 3030 3538 2c34 362e 3538   65.620058,46.58
-000049c0: 3038 3335 2030 2c37 2e32 3835 3638 3520  0835 0,7.285685 
-000049d0: 2d31 2e38 3730 3035 2c31 342e 3231 3234  -1.87005,14.2124
-000049e0: 3537 202d 352e 3234 3938 2c32 302e 3530  57 -5.2498,20.50
-000049f0: 3434 3138 202d 332e 3337 3937 342c 362e  4418 -3.37974,6.
-00004a00: 3239 3139 3631 202d 382e 3236 3931 382c  291961 -8.26918,
-00004a10: 3131 2e39 3439 3131 3120 2d31 342e 3330  11.949111 -14.30
-00004a20: 3739 352c 3136 2e36 3935 3535 202d 362e  795,16.69555 -6.
-00004a30: 3033 3837 372c 342e 3734 3634 3434 202d  03877,4.746444 -
-00004a40: 3133 2e32 3236 3838 2c38 2e35 3832 3136  13.22688,8.58216
-00004a50: 3420 2d32 312e 3230 3339 362c 3131 2e32  4 -21.20396,11.2
-00004a60: 3331 3238 3420 2d37 2e39 3737 3037 342c  31284 -7.977074,
-00004a70: 322e 3634 3931 3220 2d31 362e 3734 3331  2.64912 -16.7431
-00004a80: 3235 2c34 2e31 3131 3633 202d 3235 2e39  25,4.11163 -25.9
-00004a90: 3337 3739 2c34 2e31 3131 3633 202d 3336  3779,4.11163 -36
-00004aa0: 2e37 3738 3636 332c 3020 2d36 362e 3636  .778663,0 -66.66
-00004ab0: 3632 352c 2d32 332e 3430 3031 3433 202d  625,-23.400143 -
-00004ac0: 3636 2e36 3636 3235 2c2d 3532 2e35 3432  66.66625,-52.542
-00004ad0: 3838 3220 302c 2d32 392e 3134 3237 3334  882 0,-29.142734
-00004ae0: 2033 302e 3936 3730 3239 2c2d 3436 2e35   30.967029,-46.5
-00004af0: 3830 3833 3520 3637 2e37 3435 3639 322c  80835 67.745692,
-00004b00: 2d34 362e 3538 3038 3335 207a 220d 0a20  -46.580835 z".. 
-00004b10: 2020 2020 6964 3d22 7061 7468 3330 3332      id="path3032
-00004b20: 220d 0a20 2020 2020 696e 6b73 6361 7065  "..     inkscape
-00004b30: 3a63 6f6e 6e65 6374 6f72 2d63 7572 7661  :connector-curva
-00004b40: 7475 7265 3d22 3022 0d0a 2020 2020 2073  ture="0"..     s
-00004b50: 6f64 6970 6f64 693a 6e6f 6465 7479 7065  odipodi:nodetype
-00004b60: 733d 2273 7373 7373 7373 7373 7373 7373  s="sssssssssssss
-00004b70: 7373 7373 7373 7322 202f 3e0d 0a3c 2f73  sssssss" />..</s
-00004b80: 7667 3e0d 0a                             vg>..
+000012c0: 6f70 2d63 6f6c 6f72 3a23 3030 3561 3835  op-color:#005a85
+000012d0: 3b73 746f 702d 6f70 6163 6974 793a 302e  ;stop-opacity:0.
+000012e0: 3735 3230 3636 3134 3b22 0a20 2020 2020  75206614;".     
+000012f0: 2020 2020 6f66 6673 6574 3d22 3122 0a20      offset="1". 
+00001300: 2020 2020 2020 2020 6964 3d22 7374 6f70          id="stop
+00001310: 3333 3436 2220 2f3e 0a20 2020 203c 2f6c  3346" />.    </l
+00001320: 696e 6561 7247 7261 6469 656e 743e 0a20  inearGradient>. 
+00001330: 2020 203c 6c69 6e65 6172 4772 6164 6965     <linearGradie
+00001340: 6e74 0a20 2020 2020 2020 6964 3d22 6c69  nt.       id="li
+00001350: 6e65 6172 4772 6164 6965 6e74 3333 3130  nearGradient3310
+00001360: 223e 0a20 2020 2020 203c 7374 6f70 0a20  ">.      <stop. 
+00001370: 2020 2020 2020 2020 6964 3d22 7374 6f70          id="stop
+00001380: 3333 3132 220a 2020 2020 2020 2020 206f  3312".         o
+00001390: 6666 7365 743d 2230 220a 2020 2020 2020  ffset="0".      
+000013a0: 2020 2073 7479 6c65 3d22 7374 6f70 2d63     style="stop-c
+000013b0: 6f6c 6f72 3a23 6165 3032 3032 3b73 746f  olor:#ae0202;sto
+000013c0: 702d 6f70 6163 6974 793a 313b 2220 2f3e  p-opacity:1;" />
+000013d0: 0a20 2020 2020 203c 7374 6f70 0a20 2020  .      <stop.   
+000013e0: 2020 2020 2020 6964 3d22 7374 6f70 3333        id="stop33
+000013f0: 3134 220a 2020 2020 2020 2020 206f 6666  14".         off
+00001400: 7365 743d 2231 220a 2020 2020 2020 2020  set="1".        
+00001410: 2073 7479 6c65 3d22 7374 6f70 2d63 6f6c   style="stop-col
+00001420: 6f72 3a23 6234 3735 3735 3b73 746f 702d  or:#b47575;stop-
+00001430: 6f70 6163 6974 793a 313b 2220 2f3e 0a20  opacity:1;" />. 
+00001440: 2020 203c 2f6c 696e 6561 7247 7261 6469     </linearGradi
+00001450: 656e 743e 0a20 2020 203c 696e 6b73 6361  ent>.    <inksca
+00001460: 7065 3a70 6572 7370 6563 7469 7665 0a20  pe:perspective. 
+00001470: 2020 2020 2020 736f 6469 706f 6469 3a74        sodipodi:t
+00001480: 7970 653d 2269 6e6b 7363 6170 653a 7065  ype="inkscape:pe
+00001490: 7273 7033 6422 0a20 2020 2020 2020 696e  rsp3d".       in
+000014a0: 6b73 6361 7065 3a76 705f 783d 2230 203a  kscape:vp_x="0 :
+000014b0: 2031 3538 2e33 3231 3636 203a 2031 220a   158.32166 : 1".
+000014c0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+000014d0: 7670 5f79 3d22 3020 3a20 3130 3030 203a  vp_y="0 : 1000 :
+000014e0: 2030 220a 2020 2020 2020 2069 6e6b 7363   0".       inksc
+000014f0: 6170 653a 7670 5f7a 3d22 3438 362e 3034  ape:vp_z="486.04
+00001500: 3939 3920 3a20 3135 382e 3332 3136 3620  999 : 158.32166 
+00001510: 3a20 3122 0a20 2020 2020 2020 696e 6b73  : 1".       inks
+00001520: 6361 7065 3a70 6572 7370 3364 2d6f 7269  cape:persp3d-ori
+00001530: 6769 6e3d 2232 3433 2e30 3234 3939 203a  gin="243.02499 :
+00001540: 2031 3334 2e33 3539 3137 203a 2031 220a   134.35917 : 1".
+00001550: 2020 2020 2020 2069 643d 2270 6572 7370         id="persp
+00001560: 6563 7469 7665 3437 2220 2f3e 0a20 2020  ective47" />.   
+00001570: 203c 6c69 6e65 6172 4772 6164 6965 6e74   <linearGradient
+00001580: 0a20 2020 2020 2020 6964 3d22 6c69 6e65  .       id="line
+00001590: 6172 4772 6164 6965 6e74 3237 3935 223e  arGradient2795">
+000015a0: 0a20 2020 2020 203c 7374 6f70 0a20 2020  .      <stop.   
+000015b0: 2020 2020 2020 7374 796c 653d 2273 746f        style="sto
+000015c0: 702d 636f 6c6f 723a 2362 3862 3862 383b  p-color:#b8b8b8;
+000015d0: 7374 6f70 2d6f 7061 6369 7479 3a30 2e34  stop-opacity:0.4
+000015e0: 3938 3033 3932 3222 0a20 2020 2020 2020  9803922".       
+000015f0: 2020 6f66 6673 6574 3d22 3022 0a20 2020    offset="0".   
+00001600: 2020 2020 2020 6964 3d22 7374 6f70 3237        id="stop27
+00001610: 3937 2220 2f3e 0a20 2020 2020 203c 7374  97" />.      <st
+00001620: 6f70 0a20 2020 2020 2020 2020 7374 796c  op.         styl
+00001630: 653d 2273 746f 702d 636f 6c6f 723a 2337  e="stop-color:#7
+00001640: 6637 6637 663b 7374 6f70 2d6f 7061 6369  f7f7f;stop-opaci
+00001650: 7479 3a30 220a 2020 2020 2020 2020 206f  ty:0".         o
+00001660: 6666 7365 743d 2231 220a 2020 2020 2020  ffset="1".      
+00001670: 2020 2069 643d 2273 746f 7032 3739 3922     id="stop2799"
+00001680: 202f 3e0a 2020 2020 3c2f 6c69 6e65 6172   />.    </linear
+00001690: 4772 6164 6965 6e74 3e0a 2020 2020 3c6c  Gradient>.    <l
+000016a0: 696e 6561 7247 7261 6469 656e 740a 2020  inearGradient.  
+000016b0: 2020 2020 2069 643d 226c 696e 6561 7247       id="linearG
+000016c0: 7261 6469 656e 7432 3738 3722 3e0a 2020  radient2787">.  
+000016d0: 2020 2020 3c73 746f 700a 2020 2020 2020      <stop.      
+000016e0: 2020 2073 7479 6c65 3d22 7374 6f70 2d63     style="stop-c
+000016f0: 6f6c 6f72 3a23 3766 3766 3766 3b73 746f  olor:#7f7f7f;sto
+00001700: 702d 6f70 6163 6974 793a 302e 3522 0a20  p-opacity:0.5". 
+00001710: 2020 2020 2020 2020 6f66 6673 6574 3d22          offset="
+00001720: 3022 0a20 2020 2020 2020 2020 6964 3d22  0".         id="
+00001730: 7374 6f70 3237 3839 2220 2f3e 0a20 2020  stop2789" />.   
+00001740: 2020 203c 7374 6f70 0a20 2020 2020 2020     <stop.       
+00001750: 2020 7374 796c 653d 2273 746f 702d 636f    style="stop-co
+00001760: 6c6f 723a 2337 6637 6637 663b 7374 6f70  lor:#7f7f7f;stop
+00001770: 2d6f 7061 6369 7479 3a30 220a 2020 2020  -opacity:0".    
+00001780: 2020 2020 206f 6666 7365 743d 2231 220a       offset="1".
+00001790: 2020 2020 2020 2020 2069 643d 2273 746f           id="sto
+000017a0: 7032 3739 3122 202f 3e0a 2020 2020 3c2f  p2791" />.    </
+000017b0: 6c69 6e65 6172 4772 6164 6965 6e74 3e0a  linearGradient>.
+000017c0: 2020 2020 3c6c 696e 6561 7247 7261 6469      <linearGradi
+000017d0: 656e 740a 2020 2020 2020 2069 643d 226c  ent.       id="l
+000017e0: 696e 6561 7247 7261 6469 656e 7433 3637  inearGradient367
+000017f0: 3622 3e0a 2020 2020 2020 3c73 746f 700a  6">.      <stop.
+00001800: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+00001810: 7374 6f70 2d63 6f6c 6f72 3a23 6232 6232  stop-color:#b2b2
+00001820: 6232 3b73 746f 702d 6f70 6163 6974 793a  b2;stop-opacity:
+00001830: 302e 3522 0a20 2020 2020 2020 2020 6f66  0.5".         of
+00001840: 6673 6574 3d22 3022 0a20 2020 2020 2020  fset="0".       
+00001850: 2020 6964 3d22 7374 6f70 3336 3738 2220    id="stop3678" 
+00001860: 2f3e 0a20 2020 2020 203c 7374 6f70 0a20  />.      <stop. 
+00001870: 2020 2020 2020 2020 7374 796c 653d 2273          style="s
+00001880: 746f 702d 636f 6c6f 723a 2362 3362 3362  top-color:#b3b3b
+00001890: 333b 7374 6f70 2d6f 7061 6369 7479 3a30  3;stop-opacity:0
+000018a0: 220a 2020 2020 2020 2020 206f 6666 7365  ".         offse
+000018b0: 743d 2231 220a 2020 2020 2020 2020 2069  t="1".         i
+000018c0: 643d 2273 746f 7033 3638 3022 202f 3e0a  d="stop3680" />.
+000018d0: 2020 2020 3c2f 6c69 6e65 6172 4772 6164      </linearGrad
+000018e0: 6965 6e74 3e0a 2020 2020 3c6c 696e 6561  ient>.    <linea
+000018f0: 7247 7261 6469 656e 740a 2020 2020 2020  rGradient.      
+00001900: 2069 643d 226c 696e 6561 7247 7261 6469   id="linearGradi
+00001910: 656e 7433 3233 3622 3e0a 2020 2020 2020  ent3236">.      
+00001920: 3c73 746f 700a 2020 2020 2020 2020 2073  <stop.         s
+00001930: 7479 6c65 3d22 7374 6f70 2d63 6f6c 6f72  tyle="stop-color
+00001940: 3a23 6634 6634 6634 3b73 746f 702d 6f70  :#f4f4f4;stop-op
+00001950: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+00001960: 2020 6f66 6673 6574 3d22 3022 0a20 2020    offset="0".   
+00001970: 2020 2020 2020 6964 3d22 7374 6f70 3332        id="stop32
+00001980: 3434 2220 2f3e 0a20 2020 2020 203c 7374  44" />.      <st
+00001990: 6f70 0a20 2020 2020 2020 2020 7374 796c  op.         styl
+000019a0: 653d 2273 746f 702d 636f 6c6f 723a 2366  e="stop-color:#f
+000019b0: 6666 6666 663b 7374 6f70 2d6f 7061 6369  fffff;stop-opaci
+000019c0: 7479 3a31 220a 2020 2020 2020 2020 206f  ty:1".         o
+000019d0: 6666 7365 743d 2231 220a 2020 2020 2020  ffset="1".      
+000019e0: 2020 2069 643d 2273 746f 7033 3234 3022     id="stop3240"
+000019f0: 202f 3e0a 2020 2020 3c2f 6c69 6e65 6172   />.    </linear
+00001a00: 4772 6164 6965 6e74 3e0a 2020 2020 3c6c  Gradient>.    <l
+00001a10: 696e 6561 7247 7261 6469 656e 740a 2020  inearGradient.  
+00001a20: 2020 2020 2069 643d 226c 696e 6561 7247       id="linearG
+00001a30: 7261 6469 656e 7434 3637 3122 3e0a 2020  radient4671">.  
+00001a40: 2020 2020 3c73 746f 700a 2020 2020 2020      <stop.      
+00001a50: 2020 2073 7479 6c65 3d22 7374 6f70 2d63     style="stop-c
+00001a60: 6f6c 6f72 3a23 6666 6434 3362 3b73 746f  olor:#ffd43b;sto
+00001a70: 702d 6f70 6163 6974 793a 3122 0a20 2020  p-opacity:1".   
+00001a80: 2020 2020 2020 6f66 6673 6574 3d22 3022        offset="0"
+00001a90: 0a20 2020 2020 2020 2020 6964 3d22 7374  .         id="st
+00001aa0: 6f70 3436 3733 2220 2f3e 0a20 2020 2020  op4673" />.     
+00001ab0: 203c 7374 6f70 0a20 2020 2020 2020 2020   <stop.         
+00001ac0: 7374 796c 653d 2273 746f 702d 636f 6c6f  style="stop-colo
+00001ad0: 723a 2366 6665 3837 333b 7374 6f70 2d6f  r:#ffe873;stop-o
+00001ae0: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+00001af0: 2020 206f 6666 7365 743d 2231 220a 2020     offset="1".  
+00001b00: 2020 2020 2020 2069 643d 2273 746f 7034         id="stop4
+00001b10: 3637 3522 202f 3e0a 2020 2020 3c2f 6c69  675" />.    </li
+00001b20: 6e65 6172 4772 6164 6965 6e74 3e0a 2020  nearGradient>.  
+00001b30: 2020 3c6c 696e 6561 7247 7261 6469 656e    <linearGradien
+00001b40: 740a 2020 2020 2020 2069 643d 226c 696e  t.       id="lin
+00001b50: 6561 7247 7261 6469 656e 7434 3638 3922  earGradient4689"
+00001b60: 3e0a 2020 2020 2020 3c73 746f 700a 2020  >.      <stop.  
+00001b70: 2020 2020 2020 2073 7479 6c65 3d22 7374         style="st
+00001b80: 6f70 2d63 6f6c 6f72 3a23 3561 3966 6434  op-color:#5a9fd4
+00001b90: 3b73 746f 702d 6f70 6163 6974 793a 3122  ;stop-opacity:1"
+00001ba0: 0a20 2020 2020 2020 2020 6f66 6673 6574  .         offset
+00001bb0: 3d22 3022 0a20 2020 2020 2020 2020 6964  ="0".         id
+00001bc0: 3d22 7374 6f70 3436 3931 2220 2f3e 0a20  ="stop4691" />. 
+00001bd0: 2020 2020 203c 7374 6f70 0a20 2020 2020       <stop.     
+00001be0: 2020 2020 7374 796c 653d 2273 746f 702d      style="stop-
+00001bf0: 636f 6c6f 723a 2333 3036 3939 383b 7374  color:#306998;st
+00001c00: 6f70 2d6f 7061 6369 7479 3a31 220a 2020  op-opacity:1".  
+00001c10: 2020 2020 2020 206f 6666 7365 743d 2231         offset="1
+00001c20: 220a 2020 2020 2020 2020 2069 643d 2273  ".         id="s
+00001c30: 746f 7034 3639 3322 202f 3e0a 2020 2020  top4693" />.    
+00001c40: 3c2f 6c69 6e65 6172 4772 6164 6965 6e74  </linearGradient
+00001c50: 3e0a 2020 2020 3c6c 696e 6561 7247 7261  >.    <linearGra
+00001c60: 6469 656e 740a 2020 2020 2020 2078 313d  dient.       x1=
+00001c70: 2232 3234 2e32 3339 3936 220a 2020 2020  "224.23996".    
+00001c80: 2020 2079 313d 2231 3434 2e37 3537 3137     y1="144.75717
+00001c90: 220a 2020 2020 2020 2078 323d 222d 3635  ".       x2="-65
+00001ca0: 2e33 3038 3530 3222 0a20 2020 2020 2020  .308502".       
+00001cb0: 7932 3d22 3134 342e 3735 3731 3722 0a20  y2="144.75717". 
+00001cc0: 2020 2020 2020 6964 3d22 6c69 6e65 6172        id="linear
+00001cd0: 4772 6164 6965 6e74 3239 3837 220a 2020  Gradient2987".  
+00001ce0: 2020 2020 2078 6c69 6e6b 3a68 7265 663d       xlink:href=
+00001cf0: 2223 6c69 6e65 6172 4772 6164 6965 6e74  "#linearGradient
+00001d00: 3436 3731 220a 2020 2020 2020 2067 7261  4671".       gra
+00001d10: 6469 656e 7455 6e69 7473 3d22 7573 6572  dientUnits="user
+00001d20: 5370 6163 654f 6e55 7365 220a 2020 2020  SpaceOnUse".    
+00001d30: 2020 2067 7261 6469 656e 7454 7261 6e73     gradientTrans
+00001d40: 666f 726d 3d22 7472 616e 736c 6174 6528  form="translate(
+00001d50: 3130 302e 3237 3032 2c39 392e 3631 3131  100.2702,99.6111
+00001d60: 3629 2220 2f3e 0a20 2020 203c 6c69 6e65  6)" />.    <line
+00001d70: 6172 4772 6164 6965 6e74 0a20 2020 2020  arGradient.     
+00001d80: 2020 7831 3d22 3137 322e 3934 3230 3822    x1="172.94208"
+00001d90: 0a20 2020 2020 2020 7931 3d22 3737 2e34  .       y1="77.4
+00001da0: 3735 3938 3322 0a20 2020 2020 2020 7832  75983".       x2
+00001db0: 3d22 3236 2e36 3730 3239 3822 0a20 2020  ="26.670298".   
+00001dc0: 2020 2020 7932 3d22 3736 2e33 3133 3133      y2="76.31313
+00001dd0: 3322 0a20 2020 2020 2020 6964 3d22 6c69  3".       id="li
+00001de0: 6e65 6172 4772 6164 6965 6e74 3239 3930  nearGradient2990
+00001df0: 220a 2020 2020 2020 2078 6c69 6e6b 3a68  ".       xlink:h
+00001e00: 7265 663d 2223 6c69 6e65 6172 4772 6164  ref="#linearGrad
+00001e10: 6965 6e74 3436 3839 220a 2020 2020 2020  ient4689".      
+00001e20: 2067 7261 6469 656e 7455 6e69 7473 3d22   gradientUnits="
+00001e30: 7573 6572 5370 6163 654f 6e55 7365 220a  userSpaceOnUse".
+00001e40: 2020 2020 2020 2067 7261 6469 656e 7454         gradientT
+00001e50: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
+00001e60: 6174 6528 3130 302e 3237 3032 2c39 392e  ate(100.2702,99.
+00001e70: 3631 3131 3629 2220 2f3e 0a20 2020 203c  61116)" />.    <
+00001e80: 6c69 6e65 6172 4772 6164 6965 6e74 0a20  linearGradient. 
+00001e90: 2020 2020 2020 7831 3d22 3137 322e 3934        x1="172.94
+00001ea0: 3230 3822 0a20 2020 2020 2020 7931 3d22  208".       y1="
+00001eb0: 3737 2e34 3735 3938 3322 0a20 2020 2020  77.475983".     
+00001ec0: 2020 7832 3d22 3236 2e36 3730 3239 3822    x2="26.670298"
+00001ed0: 0a20 2020 2020 2020 7932 3d22 3736 2e33  .       y2="76.3
+00001ee0: 3133 3133 3322 0a20 2020 2020 2020 6964  13133".       id
+00001ef0: 3d22 6c69 6e65 6172 4772 6164 6965 6e74  ="linearGradient
+00001f00: 3235 3837 220a 2020 2020 2020 2078 6c69  2587".       xli
+00001f10: 6e6b 3a68 7265 663d 2223 6c69 6e65 6172  nk:href="#linear
+00001f20: 4772 6164 6965 6e74 3436 3839 220a 2020  Gradient4689".  
+00001f30: 2020 2020 2067 7261 6469 656e 7455 6e69       gradientUni
+00001f40: 7473 3d22 7573 6572 5370 6163 654f 6e55  ts="userSpaceOnU
+00001f50: 7365 220a 2020 2020 2020 2067 7261 6469  se".       gradi
+00001f60: 656e 7454 7261 6e73 666f 726d 3d22 7472  entTransform="tr
+00001f70: 616e 736c 6174 6528 3130 302e 3237 3032  anslate(100.2702
+00001f80: 2c39 392e 3631 3131 3629 2220 2f3e 0a20  ,99.61116)" />. 
+00001f90: 2020 203c 6c69 6e65 6172 4772 6164 6965     <linearGradie
+00001fa0: 6e74 0a20 2020 2020 2020 7831 3d22 3232  nt.       x1="22
+00001fb0: 342e 3233 3939 3622 0a20 2020 2020 2020  4.23996".       
+00001fc0: 7931 3d22 3134 342e 3735 3731 3722 0a20  y1="144.75717". 
+00001fd0: 2020 2020 2020 7832 3d22 2d36 352e 3330        x2="-65.30
+00001fe0: 3835 3032 220a 2020 2020 2020 2079 323d  8502".       y2=
+00001ff0: 2231 3434 2e37 3537 3137 220a 2020 2020  "144.75717".    
+00002000: 2020 2069 643d 226c 696e 6561 7247 7261     id="linearGra
+00002010: 6469 656e 7432 3538 3922 0a20 2020 2020  dient2589".     
+00002020: 2020 786c 696e 6b3a 6872 6566 3d22 236c    xlink:href="#l
+00002030: 696e 6561 7247 7261 6469 656e 7434 3637  inearGradient467
+00002040: 3122 0a20 2020 2020 2020 6772 6164 6965  1".       gradie
+00002050: 6e74 556e 6974 733d 2275 7365 7253 7061  ntUnits="userSpa
+00002060: 6365 4f6e 5573 6522 0a20 2020 2020 2020  ceOnUse".       
+00002070: 6772 6164 6965 6e74 5472 616e 7366 6f72  gradientTransfor
+00002080: 6d3d 2274 7261 6e73 6c61 7465 2831 3030  m="translate(100
+00002090: 2e32 3730 322c 3939 2e36 3131 3136 2922  .2702,99.61116)"
+000020a0: 202f 3e0a 2020 2020 3c6c 696e 6561 7247   />.    <linearG
+000020b0: 7261 6469 656e 740a 2020 2020 2020 2078  radient.       x
+000020c0: 313d 2231 3732 2e39 3432 3038 220a 2020  1="172.94208".  
+000020d0: 2020 2020 2079 313d 2237 372e 3437 3539       y1="77.4759
+000020e0: 3833 220a 2020 2020 2020 2078 323d 2232  83".       x2="2
+000020f0: 362e 3637 3032 3938 220a 2020 2020 2020  6.670298".      
+00002100: 2079 323d 2237 362e 3331 3331 3333 220a   y2="76.313133".
+00002110: 2020 2020 2020 2069 643d 226c 696e 6561         id="linea
+00002120: 7247 7261 6469 656e 7432 3234 3822 0a20  rGradient2248". 
+00002130: 2020 2020 2020 786c 696e 6b3a 6872 6566        xlink:href
+00002140: 3d22 236c 696e 6561 7247 7261 6469 656e  ="#linearGradien
+00002150: 7434 3638 3922 0a20 2020 2020 2020 6772  t4689".       gr
+00002160: 6164 6965 6e74 556e 6974 733d 2275 7365  adientUnits="use
+00002170: 7253 7061 6365 4f6e 5573 6522 0a20 2020  rSpaceOnUse".   
+00002180: 2020 2020 6772 6164 6965 6e74 5472 616e      gradientTran
+00002190: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
+000021a0: 2831 3030 2e32 3730 322c 3939 2e36 3131  (100.2702,99.611
+000021b0: 3136 2922 202f 3e0a 2020 2020 3c6c 696e  16)" />.    <lin
+000021c0: 6561 7247 7261 6469 656e 740a 2020 2020  earGradient.    
+000021d0: 2020 2078 313d 2232 3234 2e32 3339 3936     x1="224.23996
+000021e0: 220a 2020 2020 2020 2079 313d 2231 3434  ".       y1="144
+000021f0: 2e37 3537 3137 220a 2020 2020 2020 2078  .75717".       x
+00002200: 323d 222d 3635 2e33 3038 3530 3222 0a20  2="-65.308502". 
+00002210: 2020 2020 2020 7932 3d22 3134 342e 3735        y2="144.75
+00002220: 3731 3722 0a20 2020 2020 2020 6964 3d22  717".       id="
+00002230: 6c69 6e65 6172 4772 6164 6965 6e74 3232  linearGradient22
+00002240: 3530 220a 2020 2020 2020 2078 6c69 6e6b  50".       xlink
+00002250: 3a68 7265 663d 2223 6c69 6e65 6172 4772  :href="#linearGr
+00002260: 6164 6965 6e74 3436 3731 220a 2020 2020  adient4671".    
+00002270: 2020 2067 7261 6469 656e 7455 6e69 7473     gradientUnits
+00002280: 3d22 7573 6572 5370 6163 654f 6e55 7365  ="userSpaceOnUse
+00002290: 220a 2020 2020 2020 2067 7261 6469 656e  ".       gradien
+000022a0: 7454 7261 6e73 666f 726d 3d22 7472 616e  tTransform="tran
+000022b0: 736c 6174 6528 3130 302e 3237 3032 2c39  slate(100.2702,9
+000022c0: 392e 3631 3131 3629 2220 2f3e 0a20 2020  9.61116)" />.   
+000022d0: 203c 6c69 6e65 6172 4772 6164 6965 6e74   <linearGradient
+000022e0: 0a20 2020 2020 2020 7831 3d22 3232 342e  .       x1="224.
+000022f0: 3233 3939 3622 0a20 2020 2020 2020 7931  23996".       y1
+00002300: 3d22 3134 342e 3735 3731 3722 0a20 2020  ="144.75717".   
+00002310: 2020 2020 7832 3d22 2d36 352e 3330 3835      x2="-65.3085
+00002320: 3032 220a 2020 2020 2020 2079 323d 2231  02".       y2="1
+00002330: 3434 2e37 3537 3137 220a 2020 2020 2020  44.75717".      
+00002340: 2069 643d 226c 696e 6561 7247 7261 6469   id="linearGradi
+00002350: 656e 7432 3235 3522 0a20 2020 2020 2020  ent2255".       
+00002360: 786c 696e 6b3a 6872 6566 3d22 236c 696e  xlink:href="#lin
+00002370: 6561 7247 7261 6469 656e 7434 3637 3122  earGradient4671"
+00002380: 0a20 2020 2020 2020 6772 6164 6965 6e74  .       gradient
+00002390: 556e 6974 733d 2275 7365 7253 7061 6365  Units="userSpace
+000023a0: 4f6e 5573 6522 0a20 2020 2020 2020 6772  OnUse".       gr
+000023b0: 6164 6965 6e74 5472 616e 7366 6f72 6d3d  adientTransform=
+000023c0: 226d 6174 7269 7828 302e 3536 3235 3431  "matrix(0.562541
+000023d0: 2c30 2c30 2c30 2e35 3637 3937 322c 2d31  ,0,0,0.567972,-1
+000023e0: 312e 3539 3734 2c2d 372e 3630 3935 3429  1.5974,-7.60954)
+000023f0: 2220 2f3e 0a20 2020 203c 6c69 6e65 6172  " />.    <linear
+00002400: 4772 6164 6965 6e74 0a20 2020 2020 2020  Gradient.       
+00002410: 7831 3d22 3137 322e 3934 3230 3822 0a20  x1="172.94208". 
+00002420: 2020 2020 2020 7931 3d22 3736 2e31 3736        y1="76.176
+00002430: 3232 3422 0a20 2020 2020 2020 7832 3d22  224".       x2="
+00002440: 3236 2e36 3730 3239 3822 0a20 2020 2020  26.670298".     
+00002450: 2020 7932 3d22 3736 2e33 3133 3133 3322    y2="76.313133"
+00002460: 0a20 2020 2020 2020 6964 3d22 6c69 6e65  .       id="line
+00002470: 6172 4772 6164 6965 6e74 3232 3538 220a  arGradient2258".
+00002480: 2020 2020 2020 2078 6c69 6e6b 3a68 7265         xlink:hre
+00002490: 663d 2223 6c69 6e65 6172 4772 6164 6965  f="#linearGradie
+000024a0: 6e74 3436 3839 220a 2020 2020 2020 2067  nt4689".       g
+000024b0: 7261 6469 656e 7455 6e69 7473 3d22 7573  radientUnits="us
+000024c0: 6572 5370 6163 654f 6e55 7365 220a 2020  erSpaceOnUse".  
+000024d0: 2020 2020 2067 7261 6469 656e 7454 7261       gradientTra
+000024e0: 6e73 666f 726d 3d22 6d61 7472 6978 2830  nsform="matrix(0
+000024f0: 2e35 3632 3534 312c 302c 302c 302e 3536  .562541,0,0,0.56
+00002500: 3739 3732 2c2d 3131 2e35 3937 342c 2d37  7972,-11.5974,-7
+00002510: 2e36 3039 3534 2922 202f 3e0a 2020 2020  .60954)" />.    
+00002520: 3c72 6164 6961 6c47 7261 6469 656e 740a  <radialGradient.
+00002530: 2020 2020 2020 2063 783d 2236 312e 3531         cx="61.51
+00002540: 3838 3833 220a 2020 2020 2020 2063 793d  8883".       cy=
+00002550: 2231 3332 2e32 3835 3735 220a 2020 2020  "132.28575".    
+00002560: 2020 2072 3d22 3239 2e30 3336 3931 3322     r="29.036913"
+00002570: 0a20 2020 2020 2020 6678 3d22 3631 2e35  .       fx="61.5
+00002580: 3138 3838 3322 0a20 2020 2020 2020 6679  18883".       fy
+00002590: 3d22 3133 322e 3238 3537 3522 0a20 2020  ="132.28575".   
+000025a0: 2020 2020 6964 3d22 7261 6469 616c 4772      id="radialGr
+000025b0: 6164 6965 6e74 3238 3031 220a 2020 2020  adient2801".    
+000025c0: 2020 2078 6c69 6e6b 3a68 7265 663d 2223     xlink:href="#
+000025d0: 6c69 6e65 6172 4772 6164 6965 6e74 3237  linearGradient27
+000025e0: 3935 220a 2020 2020 2020 2067 7261 6469  95".       gradi
+000025f0: 656e 7455 6e69 7473 3d22 7573 6572 5370  entUnits="userSp
+00002600: 6163 654f 6e55 7365 220a 2020 2020 2020  aceOnUse".      
+00002610: 2067 7261 6469 656e 7454 7261 6e73 666f   gradientTransfo
+00002620: 726d 3d22 6d61 7472 6978 2831 2c30 2c30  rm="matrix(1,0,0
+00002630: 2c30 2e31 3737 3936 362c 302c 3130 382e  ,0.177966,0,108.
+00002640: 3734 3334 2922 202f 3e0a 2020 2020 3c6c  7434)" />.    <l
+00002650: 696e 6561 7247 7261 6469 656e 740a 2020  inearGradient.  
+00002660: 2020 2020 2078 313d 2231 3530 2e39 3631       x1="150.961
+00002670: 3131 220a 2020 2020 2020 2079 313d 2231  11".       y1="1
+00002680: 3932 2e33 3531 3736 220a 2020 2020 2020  92.35176".      
+00002690: 2078 323d 2231 3132 2e30 3331 3434 220a   x2="112.03144".
+000026a0: 2020 2020 2020 2079 323d 2231 3337 2e32         y2="137.2
+000026b0: 3732 3939 220a 2020 2020 2020 2069 643d  7299".       id=
+000026c0: 226c 696e 6561 7247 7261 6469 656e 7431  "linearGradient1
+000026d0: 3437 3522 0a20 2020 2020 2020 786c 696e  475".       xlin
+000026e0: 6b3a 6872 6566 3d22 236c 696e 6561 7247  k:href="#linearG
+000026f0: 7261 6469 656e 7434 3637 3122 0a20 2020  radient4671".   
+00002700: 2020 2020 6772 6164 6965 6e74 556e 6974      gradientUnit
+00002710: 733d 2275 7365 7253 7061 6365 4f6e 5573  s="userSpaceOnUs
+00002720: 6522 0a20 2020 2020 2020 6772 6164 6965  e".       gradie
+00002730: 6e74 5472 616e 7366 6f72 6d3d 226d 6174  ntTransform="mat
+00002740: 7269 7828 302e 3536 3235 3431 2c30 2c30  rix(0.562541,0,0
+00002750: 2c30 2e35 3637 3937 322c 2d39 2e33 3939  ,0.567972,-9.399
+00002760: 3734 392c 2d35 2e33 3035 3331 3729 2220  749,-5.305317)" 
+00002770: 2f3e 0a20 2020 203c 6c69 6e65 6172 4772  />.    <linearGr
+00002780: 6164 6965 6e74 0a20 2020 2020 2020 7831  adient.       x1
+00002790: 3d22 3236 2e36 3438 3933 3722 0a20 2020  ="26.648937".   
+000027a0: 2020 2020 7931 3d22 3230 2e36 3033 3738      y1="20.60378
+000027b0: 3122 0a20 2020 2020 2020 7832 3d22 3133  1".       x2="13
+000027c0: 352e 3636 3532 3522 0a20 2020 2020 2020  5.66525".       
+000027d0: 7932 3d22 3131 342e 3339 3736 3722 0a20  y2="114.39767". 
+000027e0: 2020 2020 2020 6964 3d22 6c69 6e65 6172        id="linear
+000027f0: 4772 6164 6965 6e74 3134 3738 220a 2020  Gradient1478".  
+00002800: 2020 2020 2078 6c69 6e6b 3a68 7265 663d       xlink:href=
+00002810: 2223 6c69 6e65 6172 4772 6164 6965 6e74  "#linearGradient
+00002820: 3436 3839 220a 2020 2020 2020 2067 7261  4689".       gra
+00002830: 6469 656e 7455 6e69 7473 3d22 7573 6572  dientUnits="user
+00002840: 5370 6163 654f 6e55 7365 220a 2020 2020  SpaceOnUse".    
+00002850: 2020 2067 7261 6469 656e 7454 7261 6e73     gradientTrans
+00002860: 666f 726d 3d22 6d61 7472 6978 2830 2e35  form="matrix(0.5
+00002870: 3632 3534 312c 302c 302c 302e 3536 3739  62541,0,0,0.5679
+00002880: 3732 2c2d 392e 3339 3937 3439 2c2d 352e  72,-9.399749,-5.
+00002890: 3330 3533 3137 2922 202f 3e0a 2020 2020  305317)" />.    
+000028a0: 3c72 6164 6961 6c47 7261 6469 656e 740a  <radialGradient.
+000028b0: 2020 2020 2020 2063 783d 2236 312e 3531         cx="61.51
+000028c0: 3838 3833 220a 2020 2020 2020 2063 793d  8883".       cy=
+000028d0: 2231 3332 2e32 3835 3735 220a 2020 2020  "132.28575".    
+000028e0: 2020 2072 3d22 3239 2e30 3336 3931 3322     r="29.036913"
+000028f0: 0a20 2020 2020 2020 6678 3d22 3631 2e35  .       fx="61.5
+00002900: 3138 3838 3322 0a20 2020 2020 2020 6679  18883".       fy
+00002910: 3d22 3133 322e 3238 3537 3522 0a20 2020  ="132.28575".   
+00002920: 2020 2020 6964 3d22 7261 6469 616c 4772      id="radialGr
+00002930: 6164 6965 6e74 3134 3830 220a 2020 2020  adient1480".    
+00002940: 2020 2078 6c69 6e6b 3a68 7265 663d 2223     xlink:href="#
+00002950: 6c69 6e65 6172 4772 6164 6965 6e74 3237  linearGradient27
+00002960: 3935 220a 2020 2020 2020 2067 7261 6469  95".       gradi
+00002970: 656e 7455 6e69 7473 3d22 7573 6572 5370  entUnits="userSp
+00002980: 6163 654f 6e55 7365 220a 2020 2020 2020  aceOnUse".      
+00002990: 2067 7261 6469 656e 7454 7261 6e73 666f   gradientTransfo
+000029a0: 726d 3d22 6d61 7472 6978 2832 2e33 3832  rm="matrix(2.382
+000029b0: 3731 3665 2d38 2c2d 302e 3239 3634 3035  716e-8,-0.296405
+000029c0: 2c31 2e34 3336 3736 2c34 2e36 3833 3637  ,1.43676,4.68367
+000029d0: 3365 2d37 2c2d 3132 382e 3534 342c 3135  3e-7,-128.544,15
+000029e0: 302e 3532 3032 2922 202f 3e0a 2020 2020  0.5202)" />.    
+000029f0: 3c72 6164 6961 6c47 7261 6469 656e 740a  <radialGradient.
+00002a00: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00002a10: 636f 6c6c 6563 743d 2261 6c77 6179 7322  collect="always"
+00002a20: 0a20 2020 2020 2020 786c 696e 6b3a 6872  .       xlink:hr
+00002a30: 6566 3d22 236c 696e 6561 7247 7261 6469  ef="#linearGradi
+00002a40: 656e 7432 3739 3522 0a20 2020 2020 2020  ent2795".       
+00002a50: 6964 3d22 7261 6469 616c 4772 6164 6965  id="radialGradie
+00002a60: 6e74 3234 3231 220a 2020 2020 2020 2067  nt2421".       g
+00002a70: 7261 6469 656e 7455 6e69 7473 3d22 7573  radientUnits="us
+00002a80: 6572 5370 6163 654f 6e55 7365 220a 2020  erSpaceOnUse".  
+00002a90: 2020 2020 2067 7261 6469 656e 7454 7261       gradientTra
+00002aa0: 6e73 666f 726d 3d22 6d61 7472 6978 2831  nsform="matrix(1
+00002ab0: 2e37 3439 3035 3635 652d 382c 2d30 2e32  .7490565e-8,-0.2
+00002ac0: 3339 3934 372c 312e 3035 3436 3638 2c33  39947,1.054668,3
+00002ad0: 2e37 3931 3534 3537 652d 372c 2d37 382e  .7915457e-7,-78.
+00002ae0: 3130 3934 3239 2c31 3438 2e38 3539 3036  109429,148.85906
+00002af0: 2922 0a20 2020 2020 2020 6378 3d22 3631  )".       cx="61
+00002b00: 2e35 3138 3838 3322 0a20 2020 2020 2020  .518883".       
+00002b10: 6379 3d22 3133 322e 3238 3537 3522 0a20  cy="132.28575". 
+00002b20: 2020 2020 2020 6678 3d22 3631 2e35 3138        fx="61.518
+00002b30: 3838 3322 0a20 2020 2020 2020 6679 3d22  883".       fy="
+00002b40: 3133 322e 3238 3537 3522 0a20 2020 2020  132.28575".     
+00002b50: 2020 723d 2232 392e 3033 3639 3133 2220    r="29.036913" 
+00002b60: 2f3e 0a20 2020 203c 6c69 6e65 6172 4772  />.    <linearGr
+00002b70: 6164 6965 6e74 0a20 2020 2020 2020 696e  adient.       in
+00002b80: 6b73 6361 7065 3a63 6f6c 6c65 6374 3d22  kscape:collect="
+00002b90: 616c 7761 7973 220a 2020 2020 2020 2078  always".       x
+00002ba0: 6c69 6e6b 3a68 7265 663d 2223 6c69 6e65  link:href="#line
+00002bb0: 6172 4772 6164 6965 6e74 3436 3731 2d38  arGradient4671-8
+00002bc0: 220a 2020 2020 2020 2069 643d 226c 696e  ".       id="lin
+00002bd0: 6561 7247 7261 6469 656e 7433 3832 362d  earGradient3826-
+00002be0: 3622 0a20 2020 2020 2020 7831 3d22 3336  6".       x1="36
+00002bf0: 2e39 3730 3839 3822 0a20 2020 2020 2020  .970898".       
+00002c00: 7931 3d22 3534 2e36 3436 3736 3322 0a20  y1="54.646763". 
+00002c10: 2020 2020 2020 7832 3d22 3837 2e37 3034        x2="87.704
+00002c20: 3638 3122 0a20 2020 2020 2020 7932 3d22  681".       y2="
+00002c30: 3534 2e36 3436 3736 3322 0a20 2020 2020  54.646763".     
+00002c40: 2020 6772 6164 6965 6e74 556e 6974 733d    gradientUnits=
+00002c50: 2275 7365 7253 7061 6365 4f6e 5573 6522  "userSpaceOnUse"
+00002c60: 202f 3e0a 2020 2020 3c6c 696e 6561 7247   />.    <linearG
+00002c70: 7261 6469 656e 740a 2020 2020 2020 2069  radient.       i
+00002c80: 643d 226c 696e 6561 7247 7261 6469 656e  d="linearGradien
+00002c90: 7434 3637 312d 3822 3e0a 2020 2020 2020  t4671-8">.      
+00002ca0: 3c73 746f 700a 2020 2020 2020 2020 2073  <stop.         s
+00002cb0: 7479 6c65 3d22 7374 6f70 2d63 6f6c 6f72  tyle="stop-color
+00002cc0: 3a23 6666 6434 3362 3b73 746f 702d 6f70  :#ffd43b;stop-op
+00002cd0: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+00002ce0: 2020 6f66 6673 6574 3d22 3022 0a20 2020    offset="0".   
+00002cf0: 2020 2020 2020 6964 3d22 7374 6f70 3436        id="stop46
+00002d00: 3733 2d38 2220 2f3e 0a20 2020 2020 203c  73-8" />.      <
+00002d10: 7374 6f70 0a20 2020 2020 2020 2020 7374  stop.         st
+00002d20: 796c 653d 2273 746f 702d 636f 6c6f 723a  yle="stop-color:
+00002d30: 2366 6665 3837 333b 7374 6f70 2d6f 7061  #ffe873;stop-opa
+00002d40: 6369 7479 3a31 220a 2020 2020 2020 2020  city:1".        
+00002d50: 206f 6666 7365 743d 2231 220a 2020 2020   offset="1".    
+00002d60: 2020 2020 2069 643d 2273 746f 7034 3637       id="stop467
+00002d70: 352d 3222 202f 3e0a 2020 2020 3c2f 6c69  5-2" />.    </li
+00002d80: 6e65 6172 4772 6164 6965 6e74 3e0a 2020  nearGradient>.  
+00002d90: 2020 3c6c 696e 6561 7247 7261 6469 656e    <linearGradien
+00002da0: 740a 2020 2020 2020 2069 6e6b 7363 6170  t.       inkscap
+00002db0: 653a 636f 6c6c 6563 743d 2261 6c77 6179  e:collect="alway
+00002dc0: 7322 0a20 2020 2020 2020 786c 696e 6b3a  s".       xlink:
+00002dd0: 6872 6566 3d22 236c 696e 6561 7247 7261  href="#linearGra
+00002de0: 6469 656e 7433 3831 3222 0a20 2020 2020  dient3812".     
+00002df0: 2020 6964 3d22 6c69 6e65 6172 4772 6164    id="linearGrad
+00002e00: 6965 6e74 3338 3138 220a 2020 2020 2020  ient3818".      
+00002e10: 2078 313d 2237 382e 3031 3230 3234 220a   x1="78.012024".
+00002e20: 2020 2020 2020 2079 313d 2238 302e 3330         y1="80.30
+00002e30: 3239 3333 220a 2020 2020 2020 2078 323d  2933".       x2=
+00002e40: 2231 3234 2e36 3739 3634 220a 2020 2020  "124.67964".    
+00002e50: 2020 2079 323d 2232 382e 3630 3333 3237     y2="28.603327
+00002e60: 220a 2020 2020 2020 2067 7261 6469 656e  ".       gradien
+00002e70: 7455 6e69 7473 3d22 7573 6572 5370 6163  tUnits="userSpac
+00002e80: 654f 6e55 7365 2220 2f3e 0a20 2020 203c  eOnUse" />.    <
+00002e90: 6c69 6e65 6172 4772 6164 6965 6e74 0a20  linearGradient. 
+00002ea0: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
+00002eb0: 6f6c 6c65 6374 3d22 616c 7761 7973 220a  ollect="always".
+00002ec0: 2020 2020 2020 2078 6c69 6e6b 3a68 7265         xlink:hre
+00002ed0: 663d 2223 6c69 6e65 6172 4772 6164 6965  f="#linearGradie
+00002ee0: 6e74 3338 3132 220a 2020 2020 2020 2069  nt3812".       i
+00002ef0: 643d 226c 696e 6561 7247 7261 6469 656e  d="linearGradien
+00002f00: 7434 3039 3722 0a20 2020 2020 2020 7831  t4097".       x1
+00002f10: 3d22 2d32 3035 2e30 3534 3331 220a 2020  ="-205.05431".  
+00002f20: 2020 2020 2079 313d 2235 352e 3630 3634       y1="55.6064
+00002f30: 3431 220a 2020 2020 2020 2078 323d 222d  41".       x2="-
+00002f40: 3634 2e38 3036 3235 3922 0a20 2020 2020  64.806259".     
+00002f50: 2020 7932 3d22 3535 2e36 3036 3434 3122    y2="55.606441"
+00002f60: 0a20 2020 2020 2020 6772 6164 6965 6e74  .       gradient
+00002f70: 556e 6974 733d 2275 7365 7253 7061 6365  Units="userSpace
+00002f80: 4f6e 5573 6522 0a20 2020 2020 2020 6772  OnUse".       gr
+00002f90: 6164 6965 6e74 5472 616e 7366 6f72 6d3d  adientTransform=
+00002fa0: 226d 6174 7269 7828 312e 3039 3531 3533  "matrix(1.095153
+00002fb0: 392c 302c 302c 312e 3033 3135 3236 382c  9,0,0,1.0315268,
+00002fc0: 3238 332e 3739 3331 312c 3134 2e37 3232  283.79311,14.722
+00002fd0: 3734 3629 2220 2f3e 0a20 2020 203c 6c69  746)" />.    <li
+00002fe0: 6e65 6172 4772 6164 6965 6e74 0a20 2020  nearGradient.   
+00002ff0: 2020 2020 696e 6b73 6361 7065 3a63 6f6c      inkscape:col
+00003000: 6c65 6374 3d22 616c 7761 7973 220a 2020  lect="always".  
+00003010: 2020 2020 2078 6c69 6e6b 3a68 7265 663d       xlink:href=
+00003020: 2223 6c69 6e65 6172 4772 6164 6965 6e74  "#linearGradient
+00003030: 3436 3839 220a 2020 2020 2020 2069 643d  4689".       id=
+00003040: 226c 696e 6561 7247 7261 6469 656e 7436  "linearGradient6
+00003050: 3437 3922 0a20 2020 2020 2020 7831 3d22  479".       x1="
+00003060: 2d31 3538 2e36 3637 3422 0a20 2020 2020  -158.6674".     
+00003070: 2020 7931 3d22 3436 2e31 3437 3833 3522    y1="46.147835"
+00003080: 0a20 2020 2020 2020 7832 3d22 2d37 382e  .       x2="-78.
+00003090: 3737 3730 3534 220a 2020 2020 2020 2079  777054".       y
+000030a0: 323d 2234 362e 3134 3738 3335 220a 2020  2="46.147835".  
+000030b0: 2020 2020 2067 7261 6469 656e 7455 6e69       gradientUni
+000030c0: 7473 3d22 7573 6572 5370 6163 654f 6e55  ts="userSpaceOnU
+000030d0: 7365 220a 2020 2020 2020 2067 7261 6469  se".       gradi
+000030e0: 656e 7454 7261 6e73 666f 726d 3d22 6d61  entTransform="ma
+000030f0: 7472 6978 2831 2e37 3739 3830 3739 2c30  trix(1.7798079,0
+00003100: 2c30 2c31 2e37 3739 3830 3739 2c33 3236  ,0,1.7798079,326
+00003110: 2e33 3731 3833 2c33 342e 3535 3539 3833  .37183,34.555983
+00003120: 2922 202f 3e0a 2020 2020 3c6c 696e 6561  )" />.    <linea
+00003130: 7247 7261 6469 656e 740a 2020 2020 2020  rGradient.      
+00003140: 2069 6e6b 7363 6170 653a 636f 6c6c 6563   inkscape:collec
+00003150: 743d 2261 6c77 6179 7322 0a20 2020 2020  t="always".     
+00003160: 2020 786c 696e 6b3a 6872 6566 3d22 236c    xlink:href="#l
+00003170: 696e 6561 7247 7261 6469 656e 7431 3839  inearGradient189
+00003180: 3422 0a20 2020 2020 2020 6964 3d22 6c69  4".       id="li
+00003190: 6e65 6172 4772 6164 6965 6e74 3430 3937  nearGradient4097
+000031a0: 2d34 220a 2020 2020 2020 2078 313d 222d  -4".       x1="-
+000031b0: 3230 352e 3035 3433 3122 0a20 2020 2020  205.05431".     
+000031c0: 2020 7931 3d22 3535 2e36 3036 3434 3122    y1="55.606441"
+000031d0: 0a20 2020 2020 2020 7832 3d22 2d36 342e  .       x2="-64.
+000031e0: 3830 3632 3539 220a 2020 2020 2020 2079  806259".       y
+000031f0: 323d 2235 352e 3630 3634 3431 220a 2020  2="55.606441".  
+00003200: 2020 2020 2067 7261 6469 656e 7455 6e69       gradientUni
+00003210: 7473 3d22 7573 6572 5370 6163 654f 6e55  ts="userSpaceOnU
+00003220: 7365 220a 2020 2020 2020 2067 7261 6469  se".       gradi
+00003230: 656e 7454 7261 6e73 666f 726d 3d22 7472  entTransform="tr
+00003240: 616e 736c 6174 6528 3237 322e 3232 3833  anslate(272.2283
+00003250: 2c31 352e 3638 3739 3031 2922 202f 3e0a  ,15.687901)" />.
+00003260: 2020 2020 3c6c 696e 6561 7247 7261 6469      <linearGradi
+00003270: 656e 740a 2020 2020 2020 2069 643d 226c  ent.       id="l
+00003280: 696e 6561 7247 7261 6469 656e 7431 3839  inearGradient189
+00003290: 3422 3e0a 2020 2020 2020 3c73 746f 700a  4">.      <stop.
+000032a0: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+000032b0: 7374 6f70 2d63 6f6c 6f72 3a23 6666 6633  stop-color:#fff3
+000032c0: 6365 3b73 746f 702d 6f70 6163 6974 793a  ce;stop-opacity:
+000032d0: 313b 220a 2020 2020 2020 2020 206f 6666  1;".         off
+000032e0: 7365 743d 2230 220a 2020 2020 2020 2020  set="0".        
+000032f0: 2069 643d 2273 746f 7031 3839 3022 202f   id="stop1890" /
+00003300: 3e0a 2020 2020 2020 3c73 746f 700a 2020  >.      <stop.  
+00003310: 2020 2020 2020 2073 7479 6c65 3d22 7374         style="st
+00003320: 6f70 2d63 6f6c 6f72 3a23 6666 6538 3733  op-color:#ffe873
+00003330: 3b73 746f 702d 6f70 6163 6974 793a 3122  ;stop-opacity:1"
+00003340: 0a20 2020 2020 2020 2020 6f66 6673 6574  .         offset
+00003350: 3d22 3122 0a20 2020 2020 2020 2020 6964  ="1".         id
+00003360: 3d22 7374 6f70 3138 3932 2220 2f3e 0a20  ="stop1892" />. 
+00003370: 2020 203c 2f6c 696e 6561 7247 7261 6469     </linearGradi
+00003380: 656e 743e 0a20 203c 2f64 6566 733e 0a20  ent>.  </defs>. 
+00003390: 203c 656c 6c69 7073 650a 2020 2020 2073   <ellipse.     s
+000033a0: 7479 6c65 3d22 6669 6c6c 3a75 726c 2823  tyle="fill:url(#
+000033b0: 6c69 6e65 6172 4772 6164 6965 6e74 3430  linearGradient40
+000033c0: 3937 293b 6669 6c6c 2d6f 7061 6369 7479  97);fill-opacity
+000033d0: 3a31 3b73 7472 6f6b 653a 6e6f 6e65 3b73  :1;stroke:none;s
+000033e0: 7472 6f6b 652d 7769 6474 683a 312e 3036  troke-width:1.06
+000033f0: 3238 363b 7374 726f 6b65 2d6f 7061 6369  286;stroke-opaci
+00003400: 7479 3a31 220a 2020 2020 2069 643d 2270  ty:1".     id="p
+00003410: 6174 6834 3038 3922 0a20 2020 2020 6378  ath4089".     cx
+00003420: 3d22 3133 362e 3032 3336 3822 0a20 2020  ="136.02368".   
+00003430: 2020 6379 3d22 3732 2e30 3832 3238 3322    cy="72.082283"
+00003440: 0a20 2020 2020 7278 3d22 3736 2e32 3439  .     rx="76.249
+00003450: 3032 3322 0a20 2020 2020 7279 3d22 3533  023".     ry="53
+00003460: 2e31 3638 3336 3922 202f 3e0a 2020 3c65  .168369" />.  <e
+00003470: 6c6c 6970 7365 0a20 2020 2020 7374 796c  llipse.     styl
+00003480: 653d 2266 696c 6c3a 7572 6c28 236c 696e  e="fill:url(#lin
+00003490: 6561 7247 7261 6469 656e 7434 3039 372d  earGradient4097-
+000034a0: 3429 3b66 696c 6c2d 6f70 6163 6974 793a  4);fill-opacity:
+000034b0: 313b 7374 726f 6b65 3a6e 6f6e 653b 7374  1;stroke:none;st
+000034c0: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
+000034d0: 2020 2020 2069 643d 2270 6174 6834 3038       id="path408
+000034e0: 392d 3222 0a20 2020 2020 6378 3d22 3133  9-2".     cx="13
+000034f0: 372e 3239 3830 3222 0a20 2020 2020 6379  7.29802".     cy
+00003500: 3d22 3731 2e32 3934 3334 3222 0a20 2020  ="71.294342".   
+00003510: 2020 7278 3d22 3639 2e36 3234 3032 3322    rx="69.624023"
+00003520: 0a20 2020 2020 7279 3d22 3531 2e35 3433  .     ry="51.543
+00003530: 3336 3922 202f 3e0a 2020 3c70 6174 680a  369" />.  <path.
+00003540: 2020 2020 2069 6e6b 7363 6170 653a 636f       inkscape:co
+00003550: 6e6e 6563 746f 722d 6375 7276 6174 7572  nnector-curvatur
+00003560: 653d 2230 220a 2020 2020 2064 3d22 6d20  e="0".     d="m 
+00003570: 3133 382e 3836 3434 392c 3434 2e39 3035  138.86449,44.905
+00003580: 3231 3720 6320 2d37 2e39 3139 3737 2c30  217 c -7.91977,0
+00003590: 2e30 3336 3738 202d 3135 2e34 3832 3937  .03678 -15.48297
+000035a0: 2c30 2e37 3132 3233 3720 2d32 322e 3133  ,0.712237 -22.13
+000035b0: 3738 2c31 2e38 3839 3831 202d 3139 2e36  78,1.88981 -19.6
+000035c0: 3034 3330 322c 332e 3436 3334 3335 202d  04302,3.463435 -
+000035d0: 3233 2e31 3633 3639 322c 3130 2e37 3132  23.163692,10.712
+000035e0: 3730 3920 2d32 332e 3136 3336 3932 2c32  709 -23.163692,2
+000035f0: 342e 3038 3136 2076 2031 372e 3635 3632  4.0816 v 17.6562
+00003600: 3432 2068 2034 362e 3332 3733 3732 2076  42 h 46.327372 v
+00003610: 2035 2e38 3835 3431 3220 6c20 2d32 2e38   5.885412 l -2.8
+00003620: 3835 3331 2c32 392e 3239 3831 3339 2034  8531,29.298139 4
+00003630: 332e 3833 3732 362c 2d31 312e 3037 3830  3.83726,-11.0780
+00003640: 3420 6320 342e 3236 3431 312c 302e 3039  4 c 4.26411,0.09
+00003650: 3134 2039 2e38 3637 3734 2c2d 352e 3436  14 9.86774,-5.46
+00003660: 3738 3220 352e 3332 3134 372c 2d34 312e  782 5.32147,-41.
+00003670: 3736 3137 3533 2030 2c2d 3132 2e35 3534  761753 0,-12.554
+00003680: 3938 3120 2d31 302e 3539 3135 352c 2d32  981 -10.59155,-2
+00003690: 312e 3938 3632 3235 202d 3233 2e31 3633  1.986225 -23.163
+000036a0: 372c 2d32 342e 3038 3136 202d 372e 3935  7,-24.0816 -7.95
+000036b0: 3833 352c 2d31 2e33 3234 3737 3120 2d31  835,-1.324771 -1
+000036c0: 362e 3231 3538 352c 2d31 2e39 3236 3631  6.21585,-1.92661
+000036d0: 3520 2d32 342e 3133 3536 2c2d 312e 3838  5 -24.1356,-1.88
+000036e0: 3938 3120 7a20 4d20 3131 332e 3831 312c  981 z M 113.811,
+000036f0: 3539 2e31 3035 3830 3220 6320 342e 3738  59.105802 c 4.78
+00003700: 3532 392c 3020 382e 3639 3331 312c 332e  529,0 8.69311,3.
+00003710: 3937 3136 3635 2038 2e36 3933 3131 2c38  971665 8.69311,8
+00003720: 2e38 3535 3131 3520 302c 342e 3836 3631  .855115 0,4.8661
+00003730: 3436 202d 332e 3930 3738 322c 382e 3830  46 -3.90782,8.80
+00003740: 3131 3235 202d 382e 3639 3331 312c 382e  1125 -8.69311,8.
+00003750: 3830 3131 3235 202d 342e 3830 3234 382c  801125 -4.80248,
+00003760: 2d32 652d 3620 2d38 2e36 3933 3134 2c2d  -2e-6 -8.69314,-
+00003770: 332e 3933 3439 3739 202d 382e 3639 3331  3.934979 -8.6931
+00003780: 342c 2d38 2e38 3031 3132 3520 2d33 652d  4,-8.801125 -3e-
+00003790: 352c 2d34 2e38 3833 3435 2033 2e38 3930  5,-4.88345 3.890
+000037a0: 3636 2c2d 382e 3835 3531 3135 2038 2e36  66,-8.855115 8.6
+000037b0: 3933 3134 2c2d 382e 3835 3531 3135 207a  9314,-8.855115 z
+000037c0: 220a 2020 2020 2073 7479 6c65 3d22 6669  ".     style="fi
+000037d0: 6c6c 3a75 726c 2823 6c69 6e65 6172 4772  ll:url(#linearGr
+000037e0: 6164 6965 6e74 3634 3739 293b 6669 6c6c  adient6479);fill
+000037f0: 2d6f 7061 6369 7479 3a31 3b66 696c 6c2d  -opacity:1;fill-
+00003800: 7275 6c65 3a6e 6f6e 7a65 726f 3b73 7472  rule:nonzero;str
+00003810: 6f6b 652d 7769 6474 683a 302e 3836 3339  oke-width:0.8639
+00003820: 3433 220a 2020 2020 2069 643d 2270 6174  43".     id="pat
+00003830: 6831 3934 3822 0a20 2020 2020 736f 6469  h1948".     sodi
+00003840: 706f 6469 3a6e 6f64 6574 7970 6573 3d22  podi:nodetypes="
+00003850: 7363 7363 6363 6363 6363 7373 7373 7373  scscccccccssssss
+00003860: 2220 2f3e 0a20 203c 7061 7468 0a20 2020  " />.  <path.   
+00003870: 2020 7374 796c 653d 2263 6f6c 6f72 3a23    style="color:#
+00003880: 3030 3030 3030 3b66 6f6e 742d 7374 796c  000000;font-styl
+00003890: 653a 6e6f 726d 616c 3b66 6f6e 742d 7661  e:normal;font-va
+000038a0: 7269 616e 743a 6e6f 726d 616c 3b66 6f6e  riant:normal;fon
+000038b0: 742d 7765 6967 6874 3a6e 6f72 6d61 6c3b  t-weight:normal;
+000038c0: 666f 6e74 2d73 7472 6574 6368 3a6e 6f72  font-stretch:nor
+000038d0: 6d61 6c3b 666f 6e74 2d73 697a 653a 6d65  mal;font-size:me
+000038e0: 6469 756d 3b6c 696e 652d 6865 6967 6874  dium;line-height
+000038f0: 3a6e 6f72 6d61 6c3b 666f 6e74 2d66 616d  :normal;font-fam
+00003900: 696c 793a 5361 6e73 3b2d 696e 6b73 6361  ily:Sans;-inksca
+00003910: 7065 2d66 6f6e 742d 7370 6563 6966 6963  pe-font-specific
+00003920: 6174 696f 6e3a 5361 6e73 3b74 6578 742d  ation:Sans;text-
+00003930: 696e 6465 6e74 3a30 3b74 6578 742d 616c  indent:0;text-al
+00003940: 6967 6e3a 7374 6172 743b 7465 7874 2d64  ign:start;text-d
+00003950: 6563 6f72 6174 696f 6e3a 6e6f 6e65 3b74  ecoration:none;t
+00003960: 6578 742d 6465 636f 7261 7469 6f6e 2d6c  ext-decoration-l
+00003970: 696e 653a 6e6f 6e65 3b6c 6574 7465 722d  ine:none;letter-
+00003980: 7370 6163 696e 673a 6e6f 726d 616c 3b77  spacing:normal;w
+00003990: 6f72 642d 7370 6163 696e 673a 6e6f 726d  ord-spacing:norm
+000039a0: 616c 3b74 6578 742d 7472 616e 7366 6f72  al;text-transfor
+000039b0: 6d3a 6e6f 6e65 3b77 7269 7469 6e67 2d6d  m:none;writing-m
+000039c0: 6f64 653a 6c72 2d74 623b 6469 7265 6374  ode:lr-tb;direct
+000039d0: 696f 6e3a 6c74 723b 6261 7365 6c69 6e65  ion:ltr;baseline
+000039e0: 2d73 6869 6674 3a62 6173 656c 696e 653b  -shift:baseline;
+000039f0: 7465 7874 2d61 6e63 686f 723a 7374 6172  text-anchor:star
+00003a00: 743b 6469 7370 6c61 793a 696e 6c69 6e65  t;display:inline
+00003a10: 3b6f 7665 7266 6c6f 773a 7669 7369 626c  ;overflow:visibl
+00003a20: 653b 7669 7369 6269 6c69 7479 3a76 6973  e;visibility:vis
+00003a30: 6962 6c65 3b66 696c 6c3a 2362 6262 6262  ible;fill:#bbbbb
+00003a40: 623b 6669 6c6c 2d6f 7061 6369 7479 3a31  b;fill-opacity:1
+00003a50: 3b66 696c 6c2d 7275 6c65 3a6e 6f6e 7a65  ;fill-rule:nonze
+00003a60: 726f 3b73 7472 6f6b 653a 6e6f 6e65 3b73  ro;stroke:none;s
+00003a70: 7472 6f6b 652d 7769 6474 683a 392e 3538  troke-width:9.58
+00003a80: 3436 323b 6d61 726b 6572 3a6e 6f6e 653b  462;marker:none;
+00003a90: 656e 6162 6c65 2d62 6163 6b67 726f 756e  enable-backgroun
+00003aa0: 643a 6163 6375 6d75 6c61 7465 220a 2020  d:accumulate".  
+00003ab0: 2020 2064 3d22 6d20 3133 372e 3630 3438     d="m 137.6048
+00003ac0: 362c 3138 2e33 3834 3737 3720 6320 2d35  6,18.384777 c -5
+00003ad0: 352e 3236 3035 3532 2c30 202d 3737 2e34  5.260552,0 -77.4
+00003ae0: 3133 3732 322c 3230 2e30 3636 3234 3620  13722,20.066246 
+00003af0: 2d37 372e 3431 3337 3232 2c35 332e 3231  -77.413722,53.21
+00003b00: 3230 3335 2030 2e37 3839 3338 2c32 372e  2035 0.78938,27.
+00003b10: 3233 3730 3535 2032 342e 3737 3934 362c  237055 24.77946,
+00003b20: 3437 2e36 3934 3136 3820 3436 2e39 3238  47.694168 46.928
+00003b30: 3239 322c 3535 2e35 3030 3034 3820 392e  292,55.500048 9.
+00003b40: 3139 3936 322c 332e 3035 3932 3620 3335  19962,3.05926 35
+00003b50: 2e37 3736 3038 2c33 322e 3934 3938 3320  .77608,32.94983 
+00003b60: 3436 2e34 3033 3731 2c33 322e 3934 3938  46.40371,32.9498
+00003b70: 3320 352e 3331 3338 332c 3020 2d31 392e  3 5.31383,0 -19.
+00003b80: 3230 3933 352c 2d32 302e 3232 3835 3120  20935,-20.22851 
+00003b90: 2d31 332e 3232 3237 382c 2d32 342e 3637  -13.22278,-24.67
+00003ba0: 3933 3520 352e 3434 3532 352c 2d34 2e30  935 5.44525,-4.0
+00003bb0: 3438 3338 2031 332e 3035 3230 312c 2d34  4838 13.05201,-4
+00003bc0: 2e30 3138 3033 2032 382e 3231 3536 382c  .01803 28.21568,
+00003bd0: 2d31 302e 3737 3034 3820 3135 2e31 3633  -10.77048 15.163
+00003be0: 3637 2c2d 362e 3735 3234 3620 3435 2e31  67,-6.75246 45.1
+00003bf0: 3832 3635 2c2d 3235 2e32 3332 3230 3420  8265,-25.232204 
+00003c00: 3435 2e34 3536 3335 2c2d 3533 2e30 3030  45.45635,-53.000
+00003c10: 3034 3820 302c 2d33 332e 3134 3537 3839  048 0,-33.145789
+00003c20: 202d 3231 2e31 3036 3938 2c2d 3533 2e32   -21.10698,-53.2
+00003c30: 3132 3033 3520 2d37 362e 3336 3735 332c  12035 -76.36753,
+00003c40: 2d35 332e 3231 3230 3335 207a 206d 2031  -53.212035 z m 1
+00003c50: 2e30 3339 3732 2c39 2e38 3831 3230 3120  .03972,9.881201 
+00003c60: 6320 3436 2e30 3238 3636 2c30 2e32 3439  c 46.02866,0.249
+00003c70: 3939 3920 3635 2e31 3230 3036 2c31 342e  999 65.12006,14.
+00003c80: 3138 3831 2036 352e 3132 3030 362c 3433  1881 65.12006,43
+00003c90: 2e33 3330 3833 3420 2d31 2e30 3431 3934  .330834 -1.04194
+00003ca0: 2c33 332e 3035 3335 3838 202d 3335 2e39  ,33.053588 -35.9
+00003cb0: 3936 3233 2c34 372e 3238 3830 3638 202d  9623,47.288068 -
+00003cc0: 3636 2e34 3439 352c 3437 2e35 3432 3838  66.4495,47.54288
+00003cd0: 3820 2d33 302e 3435 3332 382c 302e 3235  8 -30.45328,0.25
+00003ce0: 3438 3220 2d36 362e 3931 3632 3532 2c2d  482 -66.916252,-
+00003cf0: 3138 2e34 3030 3135 202d 3636 2e39 3136  18.40015 -66.916
+00003d00: 3235 322c 2d34 372e 3534 3238 3838 2030  252,-47.542888 0
+00003d10: 2c2d 3239 2e31 3432 3733 3620 3232 2e32  ,-29.142736 22.2
+00003d20: 3137 3033 2c2d 3433 2e35 3830 3833 3420  1703,-43.580834 
+00003d30: 3638 2e32 3435 3639 322c 2d34 332e 3333  68.245692,-43.33
+00003d40: 3038 3334 207a 220a 2020 2020 2069 643d  0834 z".     id=
+00003d50: 2270 6174 6833 3033 3222 0a20 2020 2020  "path3032".     
+00003d60: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
+00003d70: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
+00003d80: 0a20 2020 2020 736f 6469 706f 6469 3a6e  .     sodipodi:n
+00003d90: 6f64 6574 7970 6573 3d22 7a63 6373 737a  odetypes="zccssz
+00003da0: 637a 7a63 7a7a 7a22 202f 3e0a 2020 3c74  czzczzz" />.  <t
+00003db0: 6578 740a 2020 2020 2078 6d6c 3a73 7061  ext.     xml:spa
+00003dc0: 6365 3d22 7072 6573 6572 7665 220a 2020  ce="preserve".  
+00003dd0: 2020 2073 7479 6c65 3d22 666f 6e74 2d73     style="font-s
+00003de0: 7479 6c65 3a69 7461 6c69 633b 666f 6e74  tyle:italic;font
+00003df0: 2d77 6569 6768 743a 626f 6c64 3b66 6f6e  -weight:bold;fon
+00003e00: 742d 7369 7a65 3a39 3670 783b 6c69 6e65  t-size:96px;line
+00003e10: 2d68 6569 6768 743a 312e 353b 666f 6e74  -height:1.5;font
+00003e20: 2d66 616d 696c 793a 2743 656e 7475 7279  -family:'Century
+00003e30: 2047 6f74 6869 6327 3b2d 696e 6b73 6361   Gothic';-inksca
+00003e40: 7065 2d66 6f6e 742d 7370 6563 6966 6963  pe-font-specific
+00003e50: 6174 696f 6e3a 2743 656e 7475 7279 2047  ation:'Century G
+00003e60: 6f74 6869 6320 426f 6c64 2049 7461 6c69  othic Bold Itali
+00003e70: 6327 3b6c 6574 7465 722d 7370 6163 696e  c';letter-spacin
+00003e80: 673a 2d34 2e37 3470 783b 6669 6c6c 3a23  g:-4.74px;fill:#
+00003e90: 3830 3830 3830 3b73 7472 6f6b 652d 7769  808080;stroke-wi
+00003ea0: 6474 683a 3133 2e34 3033 220a 2020 2020  dth:13.403".    
+00003eb0: 2078 3d22 3131 2e31 3534 3038 3122 0a20   x="11.154081". 
+00003ec0: 2020 2020 793d 2232 3031 2e34 3837 3722      y="201.4877"
+00003ed0: 0a20 2020 2020 6964 3d22 7465 7874 3338  .     id="text38
+00003ee0: 3022 3e3c 7473 7061 6e0a 2020 2020 2020  0"><tspan.      
+00003ef0: 2073 6f64 6970 6f64 693a 726f 6c65 3d22   sodipodi:role="
+00003f00: 6c69 6e65 220a 2020 2020 2020 2069 643d  line".       id=
+00003f10: 2274 7370 616e 3337 3822 0a20 2020 2020  "tspan378".     
+00003f20: 2020 783d 2231 312e 3135 3430 3831 220a    x="11.154081".
+00003f30: 2020 2020 2020 2079 3d22 3230 312e 3438         y="201.48
+00003f40: 3737 220a 2020 2020 2020 2073 7479 6c65  77".       style
+00003f50: 3d22 666f 6e74 2d73 7479 6c65 3a6e 6f72  ="font-style:nor
+00003f60: 6d61 6c3b 666f 6e74 2d76 6172 6961 6e74  mal;font-variant
+00003f70: 3a6e 6f72 6d61 6c3b 666f 6e74 2d77 6569  :normal;font-wei
+00003f80: 6768 743a 3330 303b 666f 6e74 2d73 7472  ght:300;font-str
+00003f90: 6574 6368 3a6e 6f72 6d61 6c3b 666f 6e74  etch:normal;font
+00003fa0: 2d73 697a 653a 3936 7078 3b66 6f6e 742d  -size:96px;font-
+00003fb0: 6661 6d69 6c79 3a43 6f72 6265 6c3b 2d69  family:Corbel;-i
+00003fc0: 6e6b 7363 6170 652d 666f 6e74 2d73 7065  nkscape-font-spe
+00003fd0: 6369 6669 6361 7469 6f6e 3a27 436f 7262  cification:'Corb
+00003fe0: 656c 204c 6967 6874 273b 6669 6c6c 3a23  el Light';fill:#
+00003ff0: 3830 3830 3830 223e 6775 6964 6174 613c  808080">guidata<
+00004000: 2f74 7370 616e 3e3c 2f74 6578 743e 0a3c  /tspan></text>.<
+00004010: 2f73 7667 3e0a                           /svg>.
```

### Comparing `guidata-2.3.1/guidata/images/not_found.png` & `guidata-3.0.0/guidata/images/not_found.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/python.png` & `guidata-3.0.0/guidata/images/python.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/quickview.png` & `guidata-3.0.0/guidata/images/quickview.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/save_all.png` & `guidata-3.0.0/guidata/images/save_all.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/selection.png` & `guidata-3.0.0/guidata/images/selection.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/images/settings.png` & `guidata-3.0.0/guidata/images/settings.png`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/jsonio.py` & `guidata-3.0.0/guidata/dataset/jsonio.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,24 +14,27 @@
 
 import json
 import os
 from uuid import uuid1
 
 import numpy as np
 
-from guidata.userconfigio import BaseIOHandler, WriterMixin
+from guidata.dataset.iniio import BaseIOHandler, WriterMixin
 
 
 class CustomJSONEncoder(json.JSONEncoder):
     """Custom JSON Encoder"""
 
     def default(self, o):
         """Override JSONEncoder method"""
         if isinstance(o, np.ndarray):
-            return ["array", o.tolist(), str(o.dtype)]
+            olist = o.tolist()
+            if o.dtype in (np.complex64, np.complex128):
+                olist = o.real.tolist() + o.imag.tolist()
+            return ["array", olist, str(o.dtype)]
         if isinstance(o, np.generic):
             if isinstance(o, np.integer):
                 return int(o)
             try:
                 return float(o)
             except ValueError:
                 return str(o)
@@ -49,16 +52,20 @@
     def __iterate_dict(self, obj):
         """Iterate dictionaries"""
         if isinstance(obj, list) and len(obj) == 3:
             family, data, dtypestr = obj
             try:
                 dtype = np.dtype(dtypestr)
                 if family == "array":
+                    if dtype in (np.complex64, np.complex128):
+                        return np.asarray(
+                            data[: len(data) // 2], dtype
+                        ) + 1j * np.asarray(data[len(data) // 2 :], dtype)
                     return np.asarray(data, dtype)
-            except TypeError:
+            except (TypeError, ValueError):
                 pass
         elif isinstance(obj, dict):
             for key, value in list(obj.items()):
                 obj[key] = self.__iterate_dict(value)
         return obj
 
     def object_hook(self, obj: dict):  # pylint: disable=E0202
```

### Comparing `guidata-2.3.1/guidata/locale/fr/LC_MESSAGES/guidata.mo` & `guidata-3.0.0/guidata/locale/fr/LC_MESSAGES/guidata.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,11 +1,11 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2022-06-13 17:10+0200\n"
+"POT-Creation-Date: 2023-06-29 19:08+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: utf-8\n"
@@ -71,17 +71,14 @@
 
 msgid "Arguments"
 msgstr "Arguments"
 
 msgid "Array editor"
 msgstr "Éditeur de tableaux"
 
-msgid "Array is not writeable"
-msgstr "Le tableau n'est pas accessible en écriture"
-
 msgid "Arrays with more than 3 dimensions are not supported"
 msgstr "Les tableaux ayant plus de trois dimensions ne sont pas pris en charge"
 
 msgid "Attribute"
 msgstr "Attribut"
 
 msgid "Axis:"
@@ -140,14 +137,17 @@
 
 msgid "Cut"
 msgstr "Couper"
 
 msgid "Data"
 msgstr "Données"
 
+msgid "DataFrame"
+msgstr "DataFrame"
+
 msgid "Definition:"
 msgstr "Définition :"
 
 msgid "Delete"
 msgstr "Supprimer"
 
 msgid "Description"
@@ -306,14 +306,17 @@
 
 msgid "Next"
 msgstr "Suivant"
 
 msgid "No description available"
 msgstr "Aucune description disponible"
 
+msgid "No test found in this package."
+msgstr "Aucun test trouvé dans ce package."
+
 msgid "Normal text:"
 msgstr "Text normal :"
 
 msgid "Nothing to be imported from clipboard."
 msgstr "Aucune donnée ne peut être importée depuis le presse-papiers."
 
 msgid "NumPy array"
@@ -482,17 +485,14 @@
 
 msgid "Type"
 msgstr "Type"
 
 msgid "Value"
 msgstr "Valeur"
 
-msgid "Value is forced to %d"
-msgstr "La valeur est imposée à %d"
-
 msgid "Value:"
 msgstr "Valeur :"
 
 msgid "Variable Name"
 msgstr "Nom de variable"
 
 msgid "Variable name:"
```

### Comparing `guidata-2.3.1/guidata/locale/fr/LC_MESSAGES/guidata.po` & `guidata-3.0.0/guidata/locale/fr/LC_MESSAGES/guidata.po`

 * *Files 14% similar despite different names*

```diff
@@ -1,816 +1,819 @@
-# -*- coding: utf-8 -*-
-# guidata module translation file
-# Copyright (C) 2009 CEA
-# Pierre Raybaut <pierre.raybaut@cea.fr>, 2009.
-#
-msgid ""
-msgstr ""
-"Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2022-06-13 17:10+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
-"MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
-"Content-Transfer-Encoding: utf-8\n"
-"Generated-By: pygettext.py 1.5\n"
-
-#: guidata\dataset\dataitems.py:50
-msgid "float"
-msgstr "flottant"
-
-#: guidata\dataset\dataitems.py:50
-msgid "integer"
-msgstr "entier"
-
-#: guidata\dataset\dataitems.py:56
-msgid " and "
-msgstr " et "
-
-#: guidata\dataset\dataitems.py:56
-msgid " between "
-msgstr " compris entre "
-
-#: guidata\dataset\dataitems.py:58
-msgid " higher than "
-msgstr " supérieur à "
-
-#: guidata\dataset\dataitems.py:60
-msgid " lower than "
-msgstr " inférieur à "
-
-#: guidata\dataset\dataitems.py:62
-msgid "non zero"
-msgstr "non nul"
-
-#: guidata\dataset\dataitems.py:64
-msgid "unit:"
-msgstr "unité :"
-
-#: guidata\dataset\dataitems.py:207
-msgid "even"
-msgstr "pair"
-
-#: guidata\dataset\dataitems.py:209
-msgid "odd"
-msgstr "impair"
-
-#: guidata\dataset\dataitems.py:387
-msgid "all file types"
-msgstr "tout type de fichier"
-
-#: guidata\dataset\dataitems.py:389
-msgid "supported file types:"
-msgstr "types de fichiers pris en charge : "
-
-#: guidata\dataset\qtitemwidgets.py:264 guidata\dataset\qtitemwidgets.py:328
-msgid "Value is forced to %d"
-msgstr "La valeur est imposée à %d"
-
-#: guidata\dataset\qtitemwidgets.py:645
-msgid "%s files"
-msgstr "Fichiers %s"
-
-#: guidata\dataset\qtitemwidgets.py:647
-msgid "All supported files"
-msgstr "Tous les fichiers pris en charge"
-
-#: guidata\dataset\qtitemwidgets.py:875
-msgid "Number of rows x Number of columns"
-msgstr "Nombre de lignes x Nombre de colonnes"
-
-#: guidata\dataset\qtitemwidgets.py:878
-msgid "Edit array contents"
-msgstr "Modifier le contenu du tableau"
-
-#: guidata\dataset\qtitemwidgets.py:884
-msgid "Smallest element in array"
-msgstr "Valeur minimale du tableau"
-
-#: guidata\dataset\qtitemwidgets.py:888
-msgid "Largest element in array"
-msgstr "Valeur maximale du tableau"
-
-#: guidata\dataset\qtwidgets.py:137 guidata\tests\translations.py:15
-msgid "Some required entries are incorrect"
-msgstr "Les champs surlignés n'ont pas été remplis correctement."
-
-#: guidata\dataset\qtwidgets.py:139
-msgid "Please check highlighted fields."
-msgstr "Veuillez vérifier votre saisie."
-
-#: guidata\dataset\qtwidgets.py:590
-msgid "Apply"
-msgstr "Appliquer"
-
-#: guidata\guitest.py:91
-msgid "No description available"
-msgstr "Aucune description disponible"
-
-#: guidata\guitest.py:122
-msgid "Description"
-msgstr "Description"
-
-#: guidata\guitest.py:186
-msgid "Run this script"
-msgstr "Exécuter ce script"
-
-#: guidata\guitest.py:208
-msgid "Tests - %s module"
-msgstr "Tests - Module %s"
-
-#: guidata\widgets\arrayeditor.py:536 guidata\widgets\collectionseditor.py:837
-#: guidata\widgets\console\shell.py:163 guidata\widgets\dataframeeditor.py:672
-msgid "Copy"
-msgstr "Copier"
-
-#: guidata\widgets\arrayeditor.py:584 guidata\widgets\collectionseditor.py:522
-#: guidata\widgets\collectionseditor.py:1310
-#: guidata\widgets\collectionseditor.py:1323
-msgid "Warning"
-msgstr "Avertissement"
-
-#: guidata\widgets\arrayeditor.py:585
-msgid "It was not possible to copy values for this array"
-msgstr "Impossible de copier les valeurs pour ce tableau"
-
-#: guidata\widgets\arrayeditor.py:627 guidata\widgets\arrayeditor.py:662
-#: guidata\widgets\dataframeeditor.py:785
-#: guidata\widgets\dataframeeditor.py:847
-msgid "Format"
-msgstr "Format"
-
-#: guidata\widgets\arrayeditor.py:632 guidata\widgets\dataframeeditor.py:789
-msgid "Resize"
-msgstr "Ajuster"
-
-#: guidata\widgets\arrayeditor.py:635 guidata\widgets\dataframeeditor.py:793
-msgid "Background color"
-msgstr "Couleur de fond"
-
-#: guidata\widgets\arrayeditor.py:663 guidata\widgets\dataframeeditor.py:848
-msgid "Float formatting"
-msgstr "Format de flottant"
-
-#: guidata\widgets\arrayeditor.py:673
-msgid "Format (%s) is incorrect"
-msgstr "Le format (%s) est incorrect"
-
-#: guidata\widgets\arrayeditor.py:673 guidata\widgets\collectionseditor.py:538
-#: guidata\widgets\dataframeeditor.py:858
-#: guidata\widgets\dataframeeditor.py:862
-msgid "Error"
-msgstr "Erreur"
-
-#: guidata\widgets\arrayeditor.py:711
-msgid "Array is not writeable"
-msgstr "Le tableau n'est pas accessible en écriture"
-
-#: guidata\widgets\arrayeditor.py:719
-msgid "Arrays with more than 3 dimensions are not supported"
-msgstr "Les tableaux ayant plus de trois dimensions ne sont pas pris en charge"
-
-#: guidata\widgets\arrayeditor.py:723
-msgid "The 'xlabels' argument length do no match array column number"
-msgstr ""
-"La taille de l'argument 'xlabels' ne correspond pas au nombre de colonnes du "
-"tableau"
-
-#: guidata\widgets\arrayeditor.py:728
-msgid "The 'ylabels' argument length do no match array row number"
-msgstr ""
-"La taille de l'argument 'ylabels' ne correspond pas au nombre de lignes du "
-"tableau"
-
-#: guidata\widgets\arrayeditor.py:738
-msgid "%s arrays"
-msgstr "les tableaux %s"
-
-#: guidata\widgets\arrayeditor.py:739
-msgid "%s are currently not supported"
-msgstr "Attention: %s ne sont pas pris en charge"
-
-#: guidata\widgets\arrayeditor.py:746
-msgid "NumPy array"
-msgstr "Tableau NumPy"
-
-#: guidata\widgets\arrayeditor.py:748 guidata\widgets\arrayeditor.py:940
-msgid "Array editor"
-msgstr "Éditeur de tableaux"
-
-#: guidata\widgets\arrayeditor.py:750
-msgid "read only"
-msgstr "lecture seule"
-
-#: guidata\widgets\arrayeditor.py:787
-msgid "Record array fields:"
-msgstr "Champs :"
-
-#: guidata\widgets\arrayeditor.py:799
-msgid "Data"
-msgstr "Données"
-
-#: guidata\widgets\arrayeditor.py:799
-msgid "Mask"
-msgstr "Masque"
-
-#: guidata\widgets\arrayeditor.py:799
-msgid "Masked data"
-msgstr "Données masquées"
-
-#: guidata\widgets\arrayeditor.py:810
-msgid "Axis:"
-msgstr "Axe :"
-
-#: guidata\widgets\arrayeditor.py:815
-msgid "Index:"
-msgstr "Indice :"
-
-#: guidata\widgets\arrayeditor.py:828
-msgid "<u>Warning</u>: changes are applied separately"
-msgstr "<u>Attention</u>: les changements sont appliqués séparément"
-
-#: guidata\widgets\arrayeditor.py:830
-msgid ""
-"For performance reasons, changes applied to masked array won't be reflected "
-"in array's data (and vice-versa)."
-msgstr ""
-"Pour des raisons de performance, les changements appliqués au masque ne sont "
-"pas reflétés dans le tableau associé (et vice-versa)."
-
-#: guidata\widgets\arrayeditor.py:841 guidata\widgets\collectionseditor.py:1581
-#: guidata\widgets\dataframeeditor.py:809 guidata\widgets\texteditor.py:79
-msgid "Save and Close"
-msgstr "Enregistrer et Fermer"
-
-#: guidata\widgets\arrayeditor.py:846 guidata\widgets\collectionseditor.py:1586
-#: guidata\widgets\dataframeeditor.py:814 guidata\widgets\texteditor.py:84
-msgid "Close"
-msgstr "Fermer"
-
-#: guidata\widgets\collectionseditor.py:200
-msgid "Index"
-msgstr "Indice"
-
-#: guidata\widgets\collectionseditor.py:202
-msgid "Name"
-msgstr "Nom"
-
-#: guidata\widgets\collectionseditor.py:205
-msgid "Tuple"
-msgstr "Tuple"
-
-#: guidata\widgets\collectionseditor.py:208
-msgid "List"
-msgstr "Liste"
-
-#: guidata\widgets\collectionseditor.py:211
-msgid "Dictionary"
-msgstr "Dictionnaire"
-
-#: guidata\widgets\collectionseditor.py:213
-msgid "Key"
-msgstr "Clé"
-
-#: guidata\widgets\collectionseditor.py:218
-msgid "Attribute"
-msgstr "Attribut"
-
-#: guidata\widgets\collectionseditor.py:221
-msgid "elements"
-msgstr "éléments"
-
-#: guidata\widgets\collectionseditor.py:413
-msgid "Size"
-msgstr "Taille"
-
-#: guidata\widgets\collectionseditor.py:413
-msgid "Type"
-msgstr "Type"
-
-#: guidata\widgets\collectionseditor.py:413
-msgid "Value"
-msgstr "Valeur"
-
-#: guidata\widgets\collectionseditor.py:523
-msgid ""
-"Opening this variable can be slow\n"
-"\n"
-"Do you want to continue anyway?"
-msgstr ""
-"Editer cette variable sera vraisemblablement très long.\n"
-"Souhaitez-vous néanmoins continuer ?"
-
-#: guidata\widgets\collectionseditor.py:539
-msgid ""
-"Spyder was unable to retrieve the value of this variable from the console."
-"<br><br>The error mesage was:<br><i>%s</i>"
-msgstr ""
-
-#: guidata\widgets\collectionseditor.py:759
-msgid "Edit item"
-msgstr "Modifier"
-
-#: guidata\widgets\collectionseditor.py:760
-msgid "<b>Unable to assign data to item.</b><br><br>Error message:<br>%s"
-msgstr ""
-"<b>Impossible d'accéder aux données</b><br><br>Message d'erreur :<br>%s"
-
-#: guidata\widgets\collectionseditor.py:831
-msgid "Resize rows to contents"
-msgstr "Ajuster les colonnes au contenu"
-
-#: guidata\widgets\collectionseditor.py:834
-#: guidata\widgets\console\shell.py:170
-msgid "Paste"
-msgstr "Coller"
-
-#: guidata\widgets\collectionseditor.py:840
-msgid "Edit"
-msgstr "Modifier"
-
-#: guidata\widgets\collectionseditor.py:844
-#: guidata\widgets\collectionseditor.py:1242
-#: guidata\widgets\collectionseditor.py:1261
-msgid "Plot"
-msgstr "Tracer"
-
-#: guidata\widgets\collectionseditor.py:851
-msgid "Histogram"
-msgstr "Histogramme"
-
-#: guidata\widgets\collectionseditor.py:858
-msgid "Show image"
-msgstr "Afficher l'image"
-
-#: guidata\widgets\collectionseditor.py:865
-#: guidata\widgets\collectionseditor.py:1269
-msgid "Save array"
-msgstr "Enregistrer le tableau"
-
-#: guidata\widgets\collectionseditor.py:871
-#: guidata\widgets\collectionseditor.py:1199
-#: guidata\widgets\collectionseditor.py:1208
-msgid "Insert"
-msgstr "Insérer"
-
-#: guidata\widgets\collectionseditor.py:875
-#: guidata\widgets\collectionseditor.py:1136
-msgid "Remove"
-msgstr "Supprimer"
-
-#: guidata\widgets\collectionseditor.py:880
-msgid "Show arrays min/max"
-msgstr "Afficher les min/max des tableaux"
-
-#: guidata\widgets\collectionseditor.py:885
-#: guidata\widgets\collectionseditor.py:1155
-msgid "Rename"
-msgstr "Renommer"
-
-#: guidata\widgets\collectionseditor.py:889
-#: guidata\widgets\collectionseditor.py:1158
-msgid "Duplicate"
-msgstr "Dupliquer"
-
-#: guidata\widgets\collectionseditor.py:1132
-msgid "Do you want to remove the selected item?"
-msgstr "Souhaitez-vous supprimer l'élément sélectionné ?"
-
-#: guidata\widgets\collectionseditor.py:1133
-msgid "Do you want to remove all selected items?"
-msgstr "Souhaitez-vous supprimer les éléments sélectionnés ?"
-
-#: guidata\widgets\collectionseditor.py:1156
-msgid "New variable name:"
-msgstr "Nouveau nom de variable :"
-
-#: guidata\widgets\collectionseditor.py:1159
-msgid "Variable name:"
-msgstr "Nom de variable :"
-
-#: guidata\widgets\collectionseditor.py:1199
-msgid "Key:"
-msgstr "Clé :"
-
-#: guidata\widgets\collectionseditor.py:1208
-msgid "Value:"
-msgstr "Valeur :"
-
-#: guidata\widgets\collectionseditor.py:1228
-msgid "Import error"
-msgstr "Erreur d'import"
-
-#: guidata\widgets\collectionseditor.py:1229
-msgid "Please install <b>matplotlib</b> or <b>guiqwt</b>."
-msgstr "Merci d'installer <b>guiqwt</b> ou <b>matplotlib</b>."
-
-#: guidata\widgets\collectionseditor.py:1243
-msgid "<b>Unable to plot data.</b><br><br>Error message:<br>%s"
-msgstr ""
-"<b>Impossible d'afficher les données</b><br><br>Message d'erreur :<br>%s"
-
-#: guidata\widgets\collectionseditor.py:1262
-msgid "<b>Unable to show image.</b><br><br>Error message:<br>%s"
-msgstr "<b>Impossible d'afficher l'image</b><br><br>Message d'erreur :<br>%s"
-
-#: guidata\widgets\collectionseditor.py:1274
-msgid "NumPy arrays"
-msgstr "Tableaux NumPy"
-
-#: guidata\widgets\collectionseditor.py:1288
-msgid "<b>Unable to save array</b><br><br>Error message:<br>%s"
-msgstr ""
-"<b>Impossible d'enregistrer le tableau</b><br><br>Message d'erreur :<br>%s"
-
-#: guidata\widgets\collectionseditor.py:1311
-msgid "It was not possible to copy this array"
-msgstr "Impossible de copier ce tableau"
-
-#: guidata\widgets\collectionseditor.py:1324
-msgid "It was not possible to copy this dataframe"
-msgstr "Impossible de copier ce DataFrame"
-
-#: guidata\widgets\collectionseditor.py:1346
-msgid "Clipboard contents"
-msgstr "Contenu du presse-papiers"
-
-#: guidata\widgets\collectionseditor.py:1361
-msgid "Import from clipboard"
-msgstr "Importer depuis le presse-papiers"
-
-#: guidata\widgets\collectionseditor.py:1364
-msgid "Empty clipboard"
-msgstr "Presse-papiers vide"
-
-#: guidata\widgets\collectionseditor.py:1364
-msgid "Nothing to be imported from clipboard."
-msgstr "Aucune donnée ne peut être importée depuis le presse-papiers."
-
-#: guidata\widgets\console\internalshell.py:346
-msgid "Help..."
-msgstr "Aide..."
-
-#: guidata\widgets\console\internalshell.py:357
-msgid "Help"
-msgstr "Aide"
-
-#: guidata\widgets\console\internalshell.py:368
-msgid "Shell special commands:"
-msgstr "Commandes spéciales :"
-
-#: guidata\widgets\console\internalshell.py:369
-msgid "Internal editor:"
-msgstr "Éditeur interne :"
-
-#: guidata\widgets\console\internalshell.py:370
-msgid "External editor:"
-msgstr "Éditeur externe :"
-
-#: guidata\widgets\console\internalshell.py:371
-msgid "Run script:"
-msgstr "Exécuter le script :"
-
-#: guidata\widgets\console\internalshell.py:372
-msgid "Remove references:"
-msgstr "Supprimer les références :"
-
-#: guidata\widgets\console\internalshell.py:373
-msgid "System commands:"
-msgstr "Commandes système :"
-
-#: guidata\widgets\console\internalshell.py:374
-msgid "Python help:"
-msgstr "Aide Python :"
-
-#: guidata\widgets\console\internalshell.py:375
-msgid "GUI-based editor:"
-msgstr "Éditeur graphique"
-
-#: guidata\widgets\console\internalshell.py:496
-msgid ""
-"In order to use commands like \"input\" run console with the multithread "
-"option"
-msgstr ""
-"Pour utiliser des commandes du type \"input\" dans la console, utiliser "
-"l'option multithread"
-
-#: guidata\widgets\console\mixins.py:726
-msgid "Arguments"
-msgstr "Arguments"
-
-#: guidata\widgets\console\shell.py:156
-msgid "Cut"
-msgstr "Couper"
-
-#: guidata\widgets\console\shell.py:177
-msgid "Save history log..."
-msgstr "Enregistrer l'historique..."
-
-#: guidata\widgets\console\shell.py:179
-msgid "Save current history log (i.e. all inputs and outputs) in a text file"
-msgstr ""
-"Enregistrer l'historique actuel (c.-à-d. toutes les entrées-sorties) dans un "
-"fichier texte"
-
-#: guidata\widgets\console\shell.py:187
-msgid "Delete"
-msgstr "Supprimer"
-
-#: guidata\widgets\console\shell.py:194
-msgid "Select All"
-msgstr "Sélectionner tout"
-
-#: guidata\widgets\console\shell.py:319
-msgid "Save history log"
-msgstr "Enregistrer l'historique"
-
-#: guidata\widgets\console\shell.py:322
-msgid "History logs"
-msgstr "Historiques"
-
-#: guidata\widgets\console\shell.py:726
-msgid "Copy without prompts"
-msgstr "Copier sans les entêtes"
-
-#: guidata\widgets\console\shell.py:732 guidata\widgets\console\shell.py:734
-msgid "Clear line"
-msgstr "Supprimer la ligne"
-
-#: guidata\widgets\console\shell.py:739
-msgid "Clear shell"
-msgstr "Effacer la console"
-
-#: guidata\widgets\console\shell.py:741
-msgid "Clear shell contents ('cls' command)"
-msgstr "Effacer le contenu de la console (commande 'cls')"
-
-#: guidata\widgets\dataframeeditor.py:335
-msgid ""
-"It is not possible to display this value because\n"
-"an error ocurred while trying to do it"
-msgstr "Impossible d'afficher cette valeur en raison d'une erreur inattendue"
-
-#: guidata\widgets\dataframeeditor.py:679
-msgid "To bool"
-msgstr "Vers booléen"
-
-#: guidata\widgets\dataframeeditor.py:680
-msgid "To complex"
-msgstr "Vers complexe"
-
-#: guidata\widgets\dataframeeditor.py:681
-msgid "To int"
-msgstr "Vers entier"
-
-#: guidata\widgets\dataframeeditor.py:682
-msgid "To float"
-msgstr "Vers flottant"
-
-#: guidata\widgets\dataframeeditor.py:683
-msgid "To str"
-msgstr "Vers chaîne"
-
-#: guidata\widgets\dataframeeditor.py:764
-msgid "%s editor"
-msgstr "Éditeur de %s"
-
-#: guidata\widgets\dataframeeditor.py:799
-msgid "Column min/max"
-msgstr "Min/max de colonne"
-
-#: guidata\widgets\dataframeeditor.py:857
-msgid "Format ({}) is incorrect"
-msgstr "Le format ({}) est incorrect"
-
-#: guidata\widgets\dataframeeditor.py:861
-msgid "Format ({}) should start with '%'"
-msgstr "Le format ({}) ne doit pas commencer par '%'"
-
-#: guidata\widgets\importwizard.py:166 guidata\widgets\importwizard.py:516
-msgid "Import as"
-msgstr "Importer en tant que"
-
-#: guidata\widgets\importwizard.py:168
-msgid "data"
-msgstr "données"
-
-#: guidata\widgets\importwizard.py:172
-msgid "code"
-msgstr "code"
-
-#: guidata\widgets\importwizard.py:175 guidata\widgets\importwizard.py:608
-msgid "text"
-msgstr "texte"
-
-#: guidata\widgets\importwizard.py:187
-msgid "Column separator:"
-msgstr "Séparateur de colonne :"
-
-#: guidata\widgets\importwizard.py:191
-msgid "Tab"
-msgstr "Tab"
-
-#: guidata\widgets\importwizard.py:194
-msgid "Whitespace"
-msgstr "Espace"
-
-#: guidata\widgets\importwizard.py:197 guidata\widgets\importwizard.py:215
-msgid "other"
-msgstr "autre"
-
-#: guidata\widgets\importwizard.py:208
-msgid "Row separator:"
-msgstr "Séparateur de ligne :"
-
-#: guidata\widgets\importwizard.py:212
-msgid "EOL"
-msgstr "EOL"
-
-#: guidata\widgets\importwizard.py:227
-msgid "Additional options"
-msgstr "Options supplémentaires"
-
-#: guidata\widgets\importwizard.py:231
-msgid "Skip rows:"
-msgstr "Sauter des lignes :"
-
-#: guidata\widgets\importwizard.py:241
-msgid "Comments:"
-msgstr "Commentaires :"
-
-#: guidata\widgets\importwizard.py:247
-msgid "Transpose"
-msgstr "Transposer"
-
-#: guidata\widgets\importwizard.py:519
-msgid "array"
-msgstr "tableau"
-
-#: guidata\widgets\importwizard.py:524
-msgid "list"
-msgstr "liste"
-
-#: guidata\widgets\importwizard.py:529
-msgid "DataFrame"
-msgstr ""
-
-#: guidata\widgets\importwizard.py:591 guidata\widgets\importwizard.py:678
-msgid "Import wizard"
-msgstr "Assistant d'importation"
-
-#: guidata\widgets\importwizard.py:596
-msgid "Raw text"
-msgstr "Text brut"
-
-#: guidata\widgets\importwizard.py:599
-msgid "variable_name"
-msgstr "nom_de_variable"
-
-#: guidata\widgets\importwizard.py:610
-msgid "table"
-msgstr "tableau"
-
-#: guidata\widgets\importwizard.py:611
-msgid "Preview"
-msgstr "Aperçu"
-
-#: guidata\widgets\importwizard.py:615
-msgid "Variable Name"
-msgstr "Nom de variable"
-
-#: guidata\widgets\importwizard.py:623
-msgid "Cancel"
-msgstr "Annuler"
-
-#: guidata\widgets\importwizard.py:628
-msgid "Previous"
-msgstr "Précédent"
-
-#: guidata\widgets\importwizard.py:632
-msgid "Next"
-msgstr "Suivant"
-
-#: guidata\widgets\importwizard.py:637
-msgid "Done"
-msgstr "Terminer"
-
-#: guidata\widgets\importwizard.py:679
-msgid ""
-"<b>Unable to proceed to next step</b><br><br>Please check your entries."
-"<br><br>Error message:<br>%s"
-msgstr ""
-"<b>Impossible de passer à l'étape suivante</b><br><br>Merci de vérifier "
-"votre saisie.<br><br>Message d'erreur :<br>%s"
-
-#: guidata\widgets\syntaxhighlighters.py:38
-msgid "Background:"
-msgstr "Fond :"
-
-#: guidata\widgets\syntaxhighlighters.py:39
-msgid "Current line:"
-msgstr "Ligne courante :"
-
-#: guidata\widgets\syntaxhighlighters.py:40
-msgid "Current cell:"
-msgstr "Cellule courante :"
-
-#: guidata\widgets\syntaxhighlighters.py:41
-msgid "Occurrence:"
-msgstr "Occurence :"
-
-#: guidata\widgets\syntaxhighlighters.py:42
-msgid "Link:"
-msgstr "Lien :"
-
-#: guidata\widgets\syntaxhighlighters.py:43
-msgid "Side areas:"
-msgstr "Zone latérale :"
-
-#: guidata\widgets\syntaxhighlighters.py:44
-msgid "Matched <br>parens:"
-msgstr ""
-
-#: guidata\widgets\syntaxhighlighters.py:45
-msgid "Unmatched <br>parens:"
-msgstr ""
-
-#: guidata\widgets\syntaxhighlighters.py:46
-msgid "Normal text:"
-msgstr "Text normal :"
-
-#: guidata\widgets\syntaxhighlighters.py:47
-msgid "Keyword:"
-msgstr "Mot-clé :"
-
-#: guidata\widgets\syntaxhighlighters.py:48
-msgid "Builtin:"
-msgstr "Builtin :"
-
-#: guidata\widgets\syntaxhighlighters.py:49
-msgid "Definition:"
-msgstr "Définition :"
-
-#: guidata\widgets\syntaxhighlighters.py:50
-msgid "Comment:"
-msgstr "Commentaire :"
-
-#: guidata\widgets\syntaxhighlighters.py:51
-msgid "String:"
-msgstr "Chaîne :"
-
-#: guidata\widgets\syntaxhighlighters.py:52
-msgid "Number:"
-msgstr "Nombre :"
-
-#: guidata\widgets\syntaxhighlighters.py:53
-msgid "Instance:"
-msgstr "Instance :"
-
-#: guidata\widgets\texteditor.py:97
-msgid "Text editor"
-msgstr "Éditeur de texte"
-
-#~ msgid "Source code"
-#~ msgstr "Code source"
-
-#~ msgid "Quit"
-#~ msgstr "Quitter"
-
-#~ msgid "Run all tests"
-#~ msgstr "Exécuter tous les tests"
-
-#~ msgid "Open a file"
-#~ msgstr "Ouvrir un fichier"
-
-#~ msgid "All"
-#~ msgstr "Tout"
-
-#~ msgid "Opening "
-#~ msgstr "Ouverture de "
-
-#~ msgid "Array is empty"
-#~ msgstr "Le tableau est vide"
-
-#~ msgid "unknown"
-#~ msgstr "inconnue"
-
-#~ msgid "<b>Unable to retrieve data.</b><br><br>Error message:<br>%s"
-#~ msgstr ""
-#~ "<b>Impossible d'afficher les données</b><br><br>Message d'erreur :<br>%s"
-
-#~ msgid "Truncate values"
-#~ msgstr "Tronquer les valeurs"
-
-#~ msgid "Show collection contents"
-#~ msgstr "Afficher le contenu des séquences"
-
-#~ msgid "Always edit in-place"
-#~ msgstr "Édition en ligne pour tous les types"
-
-#~ msgid "Import as array"
-#~ msgstr "Importer en tant que tableau"
-
-#~ msgid "Progression"
-#~ msgstr "Progression"
+# -*- coding: utf-8 -*-
+# guidata module translation file
+# Copyright (C) 2009 CEA
+# Pierre Raybaut <pierre.raybaut@cea.fr>, 2009.
+#
+msgid ""
+msgstr ""
+"Project-Id-Version: PACKAGE VERSION\n"
+"POT-Creation-Date: 2023-06-29 19:08+0200\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
+"MIME-Version: 1.0\n"
+"Content-Type: text/plain; charset=utf-8\n"
+"Content-Transfer-Encoding: utf-8\n"
+"Generated-By: pygettext.py 1.5\n"
+
+#: guidata\dataset\dataitems.py:70
+msgid "float"
+msgstr "flottant"
+
+#: guidata\dataset\dataitems.py:70
+msgid "integer"
+msgstr "entier"
+
+#: guidata\dataset\dataitems.py:76
+msgid " and "
+msgstr " et "
+
+#: guidata\dataset\dataitems.py:76
+msgid " between "
+msgstr " compris entre "
+
+#: guidata\dataset\dataitems.py:78
+msgid " higher than "
+msgstr " supérieur à "
+
+#: guidata\dataset\dataitems.py:80
+msgid " lower than "
+msgstr " inférieur à "
+
+#: guidata\dataset\dataitems.py:82
+msgid "non zero"
+msgstr "non nul"
+
+#: guidata\dataset\dataitems.py:84
+msgid "unit:"
+msgstr "unité :"
+
+#: guidata\dataset\dataitems.py:231
+msgid "even"
+msgstr "pair"
+
+#: guidata\dataset\dataitems.py:233
+msgid "odd"
+msgstr "impair"
+
+#: guidata\dataset\dataitems.py:448
+msgid "all file types"
+msgstr "tout type de fichier"
+
+#: guidata\dataset\dataitems.py:450
+msgid "supported file types:"
+msgstr "types de fichiers pris en charge : "
+
+#: guidata\dataset\qtitemwidgets.py:756
+msgid "%s files"
+msgstr "Fichiers %s"
+
+#: guidata\dataset\qtitemwidgets.py:758
+msgid "All supported files"
+msgstr "Tous les fichiers pris en charge"
+
+#: guidata\dataset\qtitemwidgets.py:995
+msgid "Number of rows x Number of columns"
+msgstr "Nombre de lignes x Nombre de colonnes"
+
+#: guidata\dataset\qtitemwidgets.py:998
+msgid "Edit array contents"
+msgstr "Modifier le contenu du tableau"
+
+#: guidata\dataset\qtitemwidgets.py:1004
+msgid "Smallest element in array"
+msgstr "Valeur minimale du tableau"
+
+#: guidata\dataset\qtitemwidgets.py:1008
+msgid "Largest element in array"
+msgstr "Valeur maximale du tableau"
+
+#: guidata\dataset\qtwidgets.py:162 guidata\tests\test_translations.py:15
+msgid "Some required entries are incorrect"
+msgstr "Les champs surlignés n'ont pas été remplis correctement."
+
+#: guidata\dataset\qtwidgets.py:164
+msgid "Please check highlighted fields."
+msgstr "Veuillez vérifier votre saisie."
+
+#: guidata\dataset\qtwidgets.py:643
+msgid "Apply"
+msgstr "Appliquer"
+
+#: guidata\guitest.py:137
+msgid "No description available"
+msgstr "Aucune description disponible"
+
+#: guidata\guitest.py:177
+msgid "Description"
+msgstr "Description"
+
+#: guidata\guitest.py:273
+msgid "Run this script"
+msgstr "Exécuter ce script"
+
+#: guidata\guitest.py:304
+msgid "Tests - %s module"
+msgstr "Tests - Module %s"
+
+#: guidata\guitest.py:314
+msgid "No test found in this package."
+msgstr "Aucun test trouvé dans ce package."
+
+#: guidata\guitest.py:315 guidata\widgets\arrayeditor.py:674
+#: guidata\widgets\collectionseditor.py:538
+#: guidata\widgets\dataframeeditor.py:858
+#: guidata\widgets\dataframeeditor.py:862
+msgid "Error"
+msgstr "Erreur"
+
+#: guidata\widgets\arrayeditor.py:537 guidata\widgets\collectionseditor.py:831
+#: guidata\widgets\console\shell.py:147 guidata\widgets\dataframeeditor.py:672
+msgid "Copy"
+msgstr "Copier"
+
+#: guidata\widgets\arrayeditor.py:585 guidata\widgets\collectionseditor.py:522
+#: guidata\widgets\collectionseditor.py:1300
+#: guidata\widgets\collectionseditor.py:1313
+msgid "Warning"
+msgstr "Avertissement"
+
+#: guidata\widgets\arrayeditor.py:586
+msgid "It was not possible to copy values for this array"
+msgstr "Impossible de copier les valeurs pour ce tableau"
+
+#: guidata\widgets\arrayeditor.py:628 guidata\widgets\arrayeditor.py:663
+#: guidata\widgets\dataframeeditor.py:785
+#: guidata\widgets\dataframeeditor.py:847
+msgid "Format"
+msgstr "Format"
+
+#: guidata\widgets\arrayeditor.py:633 guidata\widgets\dataframeeditor.py:789
+msgid "Resize"
+msgstr "Ajuster"
+
+#: guidata\widgets\arrayeditor.py:636 guidata\widgets\dataframeeditor.py:793
+msgid "Background color"
+msgstr "Couleur de fond"
+
+#: guidata\widgets\arrayeditor.py:664 guidata\widgets\dataframeeditor.py:848
+msgid "Float formatting"
+msgstr "Format de flottant"
+
+#: guidata\widgets\arrayeditor.py:674
+msgid "Format (%s) is incorrect"
+msgstr "Le format (%s) est incorrect"
+
+#: guidata\widgets\arrayeditor.py:716
+msgid "Arrays with more than 3 dimensions are not supported"
+msgstr "Les tableaux ayant plus de trois dimensions ne sont pas pris en charge"
+
+#: guidata\widgets\arrayeditor.py:720
+msgid "The 'xlabels' argument length do no match array column number"
+msgstr ""
+"La taille de l'argument 'xlabels' ne correspond pas au nombre de colonnes du "
+"tableau"
+
+#: guidata\widgets\arrayeditor.py:725
+msgid "The 'ylabels' argument length do no match array row number"
+msgstr ""
+"La taille de l'argument 'ylabels' ne correspond pas au nombre de lignes du "
+"tableau"
+
+#: guidata\widgets\arrayeditor.py:735
+msgid "%s arrays"
+msgstr "les tableaux %s"
+
+#: guidata\widgets\arrayeditor.py:736
+msgid "%s are currently not supported"
+msgstr "Attention: %s ne sont pas pris en charge"
+
+#: guidata\widgets\arrayeditor.py:743
+msgid "NumPy array"
+msgstr "Tableau NumPy"
+
+#: guidata\widgets\arrayeditor.py:745 guidata\widgets\arrayeditor.py:937
+msgid "Array editor"
+msgstr "Éditeur de tableaux"
+
+#: guidata\widgets\arrayeditor.py:747
+msgid "read only"
+msgstr "lecture seule"
+
+#: guidata\widgets\arrayeditor.py:784
+msgid "Record array fields:"
+msgstr "Champs :"
+
+#: guidata\widgets\arrayeditor.py:796
+msgid "Data"
+msgstr "Données"
+
+#: guidata\widgets\arrayeditor.py:796
+msgid "Mask"
+msgstr "Masque"
+
+#: guidata\widgets\arrayeditor.py:796
+msgid "Masked data"
+msgstr "Données masquées"
+
+#: guidata\widgets\arrayeditor.py:807
+msgid "Axis:"
+msgstr "Axe :"
+
+#: guidata\widgets\arrayeditor.py:812
+msgid "Index:"
+msgstr "Indice :"
+
+#: guidata\widgets\arrayeditor.py:825
+msgid "<u>Warning</u>: changes are applied separately"
+msgstr "<u>Attention</u>: les changements sont appliqués séparément"
+
+#: guidata\widgets\arrayeditor.py:827
+msgid ""
+"For performance reasons, changes applied to masked array won't be reflected "
+"in array's data (and vice-versa)."
+msgstr ""
+"Pour des raisons de performance, les changements appliqués au masque ne sont "
+"pas reflétés dans le tableau associé (et vice-versa)."
+
+#: guidata\widgets\arrayeditor.py:838 guidata\widgets\collectionseditor.py:1564
+#: guidata\widgets\dataframeeditor.py:809 guidata\widgets\texteditor.py:79
+msgid "Save and Close"
+msgstr "Enregistrer et Fermer"
+
+#: guidata\widgets\arrayeditor.py:843 guidata\widgets\collectionseditor.py:1569
+#: guidata\widgets\dataframeeditor.py:814 guidata\widgets\texteditor.py:84
+msgid "Close"
+msgstr "Fermer"
+
+#: guidata\widgets\collectionseditor.py:201
+msgid "Index"
+msgstr "Indice"
+
+#: guidata\widgets\collectionseditor.py:203
+msgid "Name"
+msgstr "Nom"
+
+#: guidata\widgets\collectionseditor.py:206
+msgid "Tuple"
+msgstr "Tuple"
+
+#: guidata\widgets\collectionseditor.py:209
+msgid "List"
+msgstr "Liste"
+
+#: guidata\widgets\collectionseditor.py:212
+msgid "Dictionary"
+msgstr "Dictionnaire"
+
+#: guidata\widgets\collectionseditor.py:214
+msgid "Key"
+msgstr "Clé"
+
+#: guidata\widgets\collectionseditor.py:219
+msgid "Attribute"
+msgstr "Attribut"
+
+#: guidata\widgets\collectionseditor.py:222
+msgid "elements"
+msgstr "éléments"
+
+#: guidata\widgets\collectionseditor.py:414
+msgid "Size"
+msgstr "Taille"
+
+#: guidata\widgets\collectionseditor.py:414
+msgid "Type"
+msgstr "Type"
+
+#: guidata\widgets\collectionseditor.py:414
+msgid "Value"
+msgstr "Valeur"
+
+#: guidata\widgets\collectionseditor.py:523
+msgid ""
+"Opening this variable can be slow\n"
+"\n"
+"Do you want to continue anyway?"
+msgstr ""
+"Editer cette variable sera vraisemblablement très long.\n"
+"Souhaitez-vous néanmoins continuer ?"
+
+#: guidata\widgets\collectionseditor.py:539
+msgid ""
+"Spyder was unable to retrieve the value of this variable from the console."
+"<br><br>The error mesage was:<br><i>%s</i>"
+msgstr ""
+
+#: guidata\widgets\collectionseditor.py:754
+msgid "Edit item"
+msgstr "Modifier"
+
+#: guidata\widgets\collectionseditor.py:755
+msgid "<b>Unable to assign data to item.</b><br><br>Error message:<br>%s"
+msgstr ""
+"<b>Impossible d'accéder aux données</b><br><br>Message d'erreur :<br>%s"
+
+#: guidata\widgets\collectionseditor.py:825
+msgid "Resize rows to contents"
+msgstr "Ajuster les colonnes au contenu"
+
+#: guidata\widgets\collectionseditor.py:828
+#: guidata\widgets\console\shell.py:154
+msgid "Paste"
+msgstr "Coller"
+
+#: guidata\widgets\collectionseditor.py:834
+msgid "Edit"
+msgstr "Modifier"
+
+#: guidata\widgets\collectionseditor.py:838
+#: guidata\widgets\collectionseditor.py:1232
+#: guidata\widgets\collectionseditor.py:1251
+msgid "Plot"
+msgstr "Tracer"
+
+#: guidata\widgets\collectionseditor.py:845
+msgid "Histogram"
+msgstr "Histogramme"
+
+#: guidata\widgets\collectionseditor.py:852
+msgid "Show image"
+msgstr "Afficher l'image"
+
+#: guidata\widgets\collectionseditor.py:859
+#: guidata\widgets\collectionseditor.py:1259
+msgid "Save array"
+msgstr "Enregistrer le tableau"
+
+#: guidata\widgets\collectionseditor.py:865
+#: guidata\widgets\collectionseditor.py:1189
+#: guidata\widgets\collectionseditor.py:1198
+msgid "Insert"
+msgstr "Insérer"
+
+#: guidata\widgets\collectionseditor.py:869
+#: guidata\widgets\collectionseditor.py:1126
+msgid "Remove"
+msgstr "Supprimer"
+
+#: guidata\widgets\collectionseditor.py:874
+msgid "Show arrays min/max"
+msgstr "Afficher les min/max des tableaux"
+
+#: guidata\widgets\collectionseditor.py:879
+#: guidata\widgets\collectionseditor.py:1145
+msgid "Rename"
+msgstr "Renommer"
+
+#: guidata\widgets\collectionseditor.py:883
+#: guidata\widgets\collectionseditor.py:1148
+msgid "Duplicate"
+msgstr "Dupliquer"
+
+#: guidata\widgets\collectionseditor.py:1122
+msgid "Do you want to remove the selected item?"
+msgstr "Souhaitez-vous supprimer l'élément sélectionné ?"
+
+#: guidata\widgets\collectionseditor.py:1123
+msgid "Do you want to remove all selected items?"
+msgstr "Souhaitez-vous supprimer les éléments sélectionnés ?"
+
+#: guidata\widgets\collectionseditor.py:1146
+msgid "New variable name:"
+msgstr "Nouveau nom de variable :"
+
+#: guidata\widgets\collectionseditor.py:1149
+msgid "Variable name:"
+msgstr "Nom de variable :"
+
+#: guidata\widgets\collectionseditor.py:1189
+msgid "Key:"
+msgstr "Clé :"
+
+#: guidata\widgets\collectionseditor.py:1198
+msgid "Value:"
+msgstr "Valeur :"
+
+#: guidata\widgets\collectionseditor.py:1218
+msgid "Import error"
+msgstr "Erreur d'import"
+
+#: guidata\widgets\collectionseditor.py:1219
+msgid "Please install <b>matplotlib</b> or <b>guiqwt</b>."
+msgstr "Merci d'installer <b>guiqwt</b> ou <b>matplotlib</b>."
+
+#: guidata\widgets\collectionseditor.py:1233
+msgid "<b>Unable to plot data.</b><br><br>Error message:<br>%s"
+msgstr ""
+"<b>Impossible d'afficher les données</b><br><br>Message d'erreur :<br>%s"
+
+#: guidata\widgets\collectionseditor.py:1252
+msgid "<b>Unable to show image.</b><br><br>Error message:<br>%s"
+msgstr "<b>Impossible d'afficher l'image</b><br><br>Message d'erreur :<br>%s"
+
+#: guidata\widgets\collectionseditor.py:1264
+msgid "NumPy arrays"
+msgstr "Tableaux NumPy"
+
+#: guidata\widgets\collectionseditor.py:1278
+msgid "<b>Unable to save array</b><br><br>Error message:<br>%s"
+msgstr ""
+"<b>Impossible d'enregistrer le tableau</b><br><br>Message d'erreur :<br>%s"
+
+#: guidata\widgets\collectionseditor.py:1301
+msgid "It was not possible to copy this array"
+msgstr "Impossible de copier ce tableau"
+
+#: guidata\widgets\collectionseditor.py:1314
+msgid "It was not possible to copy this dataframe"
+msgstr "Impossible de copier ce DataFrame"
+
+#: guidata\widgets\collectionseditor.py:1336
+msgid "Clipboard contents"
+msgstr "Contenu du presse-papiers"
+
+#: guidata\widgets\collectionseditor.py:1351
+msgid "Import from clipboard"
+msgstr "Importer depuis le presse-papiers"
+
+#: guidata\widgets\collectionseditor.py:1354
+msgid "Empty clipboard"
+msgstr "Presse-papiers vide"
+
+#: guidata\widgets\collectionseditor.py:1354
+msgid "Nothing to be imported from clipboard."
+msgstr "Aucune donnée ne peut être importée depuis le presse-papiers."
+
+#: guidata\widgets\console\internalshell.py:299
+msgid "Help..."
+msgstr "Aide..."
+
+#: guidata\widgets\console\internalshell.py:310
+msgid "Help"
+msgstr "Aide"
+
+#: guidata\widgets\console\internalshell.py:320
+msgid "Shell special commands:"
+msgstr "Commandes spéciales :"
+
+#: guidata\widgets\console\internalshell.py:321
+msgid "Internal editor:"
+msgstr "Éditeur interne :"
+
+#: guidata\widgets\console\internalshell.py:322
+msgid "External editor:"
+msgstr "Éditeur externe :"
+
+#: guidata\widgets\console\internalshell.py:323
+msgid "Run script:"
+msgstr "Exécuter le script :"
+
+#: guidata\widgets\console\internalshell.py:324
+msgid "Remove references:"
+msgstr "Supprimer les références :"
+
+#: guidata\widgets\console\internalshell.py:325
+msgid "System commands:"
+msgstr "Commandes système :"
+
+#: guidata\widgets\console\internalshell.py:326
+msgid "Python help:"
+msgstr "Aide Python :"
+
+#: guidata\widgets\console\internalshell.py:327
+msgid "GUI-based editor:"
+msgstr "Éditeur graphique"
+
+#: guidata\widgets\console\internalshell.py:448
+msgid ""
+"In order to use commands like \"input\" run console with the multithread "
+"option"
+msgstr ""
+"Pour utiliser des commandes du type \"input\" dans la console, utiliser "
+"l'option multithread"
+
+#: guidata\widgets\console\mixins.py:714
+msgid "Arguments"
+msgstr "Arguments"
+
+#: guidata\widgets\console\shell.py:140
+msgid "Cut"
+msgstr "Couper"
+
+#: guidata\widgets\console\shell.py:161
+msgid "Save history log..."
+msgstr "Enregistrer l'historique..."
+
+#: guidata\widgets\console\shell.py:163
+msgid "Save current history log (i.e. all inputs and outputs) in a text file"
+msgstr ""
+"Enregistrer l'historique actuel (c.-à-d. toutes les entrées-sorties) dans un "
+"fichier texte"
+
+#: guidata\widgets\console\shell.py:171
+msgid "Delete"
+msgstr "Supprimer"
+
+#: guidata\widgets\console\shell.py:178
+msgid "Select All"
+msgstr "Sélectionner tout"
+
+#: guidata\widgets\console\shell.py:303
+msgid "Save history log"
+msgstr "Enregistrer l'historique"
+
+#: guidata\widgets\console\shell.py:306
+msgid "History logs"
+msgstr "Historiques"
+
+#: guidata\widgets\console\shell.py:710
+msgid "Copy without prompts"
+msgstr "Copier sans les entêtes"
+
+#: guidata\widgets\console\shell.py:718 guidata\widgets\console\shell.py:720
+msgid "Clear line"
+msgstr "Supprimer la ligne"
+
+#: guidata\widgets\console\shell.py:725
+msgid "Clear shell"
+msgstr "Effacer la console"
+
+#: guidata\widgets\console\shell.py:727
+msgid "Clear shell contents ('cls' command)"
+msgstr "Effacer le contenu de la console (commande 'cls')"
+
+#: guidata\widgets\dataframeeditor.py:335
+msgid ""
+"It is not possible to display this value because\n"
+"an error ocurred while trying to do it"
+msgstr "Impossible d'afficher cette valeur en raison d'une erreur inattendue"
+
+#: guidata\widgets\dataframeeditor.py:679
+msgid "To bool"
+msgstr "Vers booléen"
+
+#: guidata\widgets\dataframeeditor.py:680
+msgid "To complex"
+msgstr "Vers complexe"
+
+#: guidata\widgets\dataframeeditor.py:681
+msgid "To int"
+msgstr "Vers entier"
+
+#: guidata\widgets\dataframeeditor.py:682
+msgid "To float"
+msgstr "Vers flottant"
+
+#: guidata\widgets\dataframeeditor.py:683
+msgid "To str"
+msgstr "Vers chaîne"
+
+#: guidata\widgets\dataframeeditor.py:764
+msgid "%s editor"
+msgstr "Éditeur de %s"
+
+#: guidata\widgets\dataframeeditor.py:799
+msgid "Column min/max"
+msgstr "Min/max de colonne"
+
+#: guidata\widgets\dataframeeditor.py:857
+msgid "Format ({}) is incorrect"
+msgstr "Le format ({}) est incorrect"
+
+#: guidata\widgets\dataframeeditor.py:861
+msgid "Format ({}) should start with '%'"
+msgstr "Le format ({}) ne doit pas commencer par '%'"
+
+#: guidata\widgets\importwizard.py:157 guidata\widgets\importwizard.py:507
+msgid "Import as"
+msgstr "Importer en tant que"
+
+#: guidata\widgets\importwizard.py:159
+msgid "data"
+msgstr "données"
+
+#: guidata\widgets\importwizard.py:163
+msgid "code"
+msgstr "code"
+
+#: guidata\widgets\importwizard.py:166 guidata\widgets\importwizard.py:599
+msgid "text"
+msgstr "texte"
+
+#: guidata\widgets\importwizard.py:178
+msgid "Column separator:"
+msgstr "Séparateur de colonne :"
+
+#: guidata\widgets\importwizard.py:182
+msgid "Tab"
+msgstr "Tab"
+
+#: guidata\widgets\importwizard.py:185
+msgid "Whitespace"
+msgstr "Espace"
+
+#: guidata\widgets\importwizard.py:188 guidata\widgets\importwizard.py:206
+msgid "other"
+msgstr "autre"
+
+#: guidata\widgets\importwizard.py:199
+msgid "Row separator:"
+msgstr "Séparateur de ligne :"
+
+#: guidata\widgets\importwizard.py:203
+msgid "EOL"
+msgstr "EOL"
+
+#: guidata\widgets\importwizard.py:218
+msgid "Additional options"
+msgstr "Options supplémentaires"
+
+#: guidata\widgets\importwizard.py:222
+msgid "Skip rows:"
+msgstr "Sauter des lignes :"
+
+#: guidata\widgets\importwizard.py:232
+msgid "Comments:"
+msgstr "Commentaires :"
+
+#: guidata\widgets\importwizard.py:238
+msgid "Transpose"
+msgstr "Transposer"
+
+#: guidata\widgets\importwizard.py:510
+msgid "array"
+msgstr "tableau"
+
+#: guidata\widgets\importwizard.py:515
+msgid "list"
+msgstr "liste"
+
+#: guidata\widgets\importwizard.py:520
+msgid "DataFrame"
+msgstr "DataFrame"
+
+#: guidata\widgets\importwizard.py:582 guidata\widgets\importwizard.py:669
+msgid "Import wizard"
+msgstr "Assistant d'importation"
+
+#: guidata\widgets\importwizard.py:587
+msgid "Raw text"
+msgstr "Text brut"
+
+#: guidata\widgets\importwizard.py:590
+msgid "variable_name"
+msgstr "nom_de_variable"
+
+#: guidata\widgets\importwizard.py:601
+msgid "table"
+msgstr "tableau"
+
+#: guidata\widgets\importwizard.py:602
+msgid "Preview"
+msgstr "Aperçu"
+
+#: guidata\widgets\importwizard.py:606
+msgid "Variable Name"
+msgstr "Nom de variable"
+
+#: guidata\widgets\importwizard.py:614
+msgid "Cancel"
+msgstr "Annuler"
+
+#: guidata\widgets\importwizard.py:619
+msgid "Previous"
+msgstr "Précédent"
+
+#: guidata\widgets\importwizard.py:623
+msgid "Next"
+msgstr "Suivant"
+
+#: guidata\widgets\importwizard.py:628
+msgid "Done"
+msgstr "Terminer"
+
+#: guidata\widgets\importwizard.py:670
+msgid ""
+"<b>Unable to proceed to next step</b><br><br>Please check your entries."
+"<br><br>Error message:<br>%s"
+msgstr ""
+"<b>Impossible de passer à l'étape suivante</b><br><br>Merci de vérifier "
+"votre saisie.<br><br>Message d'erreur :<br>%s"
+
+#: guidata\widgets\syntaxhighlighters.py:38
+msgid "Background:"
+msgstr "Fond :"
+
+#: guidata\widgets\syntaxhighlighters.py:39
+msgid "Current line:"
+msgstr "Ligne courante :"
+
+#: guidata\widgets\syntaxhighlighters.py:40
+msgid "Current cell:"
+msgstr "Cellule courante :"
+
+#: guidata\widgets\syntaxhighlighters.py:41
+msgid "Occurrence:"
+msgstr "Occurence :"
+
+#: guidata\widgets\syntaxhighlighters.py:42
+msgid "Link:"
+msgstr "Lien :"
+
+#: guidata\widgets\syntaxhighlighters.py:43
+msgid "Side areas:"
+msgstr "Zone latérale :"
+
+#: guidata\widgets\syntaxhighlighters.py:44
+msgid "Matched <br>parens:"
+msgstr ""
+
+#: guidata\widgets\syntaxhighlighters.py:45
+msgid "Unmatched <br>parens:"
+msgstr ""
+
+#: guidata\widgets\syntaxhighlighters.py:46
+msgid "Normal text:"
+msgstr "Text normal :"
+
+#: guidata\widgets\syntaxhighlighters.py:47
+msgid "Keyword:"
+msgstr "Mot-clé :"
+
+#: guidata\widgets\syntaxhighlighters.py:48
+msgid "Builtin:"
+msgstr "Builtin :"
+
+#: guidata\widgets\syntaxhighlighters.py:49
+msgid "Definition:"
+msgstr "Définition :"
+
+#: guidata\widgets\syntaxhighlighters.py:50
+msgid "Comment:"
+msgstr "Commentaire :"
+
+#: guidata\widgets\syntaxhighlighters.py:51
+msgid "String:"
+msgstr "Chaîne :"
+
+#: guidata\widgets\syntaxhighlighters.py:52
+msgid "Number:"
+msgstr "Nombre :"
+
+#: guidata\widgets\syntaxhighlighters.py:53
+msgid "Instance:"
+msgstr "Instance :"
+
+#: guidata\widgets\texteditor.py:97
+msgid "Text editor"
+msgstr "Éditeur de texte"
+
+#~ msgid "Value is forced to %d"
+#~ msgstr "La valeur est imposée à %d"
+
+#~ msgid "Array is not writeable"
+#~ msgstr "Le tableau n'est pas accessible en écriture"
+
+#~ msgid "Source code"
+#~ msgstr "Code source"
+
+#~ msgid "Quit"
+#~ msgstr "Quitter"
+
+#~ msgid "Run all tests"
+#~ msgstr "Exécuter tous les tests"
+
+#~ msgid "Open a file"
+#~ msgstr "Ouvrir un fichier"
+
+#~ msgid "All"
+#~ msgstr "Tout"
+
+#~ msgid "Opening "
+#~ msgstr "Ouverture de "
+
+#~ msgid "Array is empty"
+#~ msgstr "Le tableau est vide"
+
+#~ msgid "unknown"
+#~ msgstr "inconnue"
+
+#~ msgid "<b>Unable to retrieve data.</b><br><br>Error message:<br>%s"
+#~ msgstr ""
+#~ "<b>Impossible d'afficher les données</b><br><br>Message d'erreur :<br>%s"
+
+#~ msgid "Truncate values"
+#~ msgstr "Tronquer les valeurs"
+
+#~ msgid "Show collection contents"
+#~ msgstr "Afficher le contenu des séquences"
+
+#~ msgid "Always edit in-place"
+#~ msgstr "Édition en ligne pour tous les types"
+
+#~ msgid "Import as array"
+#~ msgstr "Importer en tant que tableau"
+
+#~ msgid "Progression"
+#~ msgstr "Progression"
```

### Comparing `guidata-2.3.1/guidata/tests/activable_dataset.py` & `guidata-3.0.0/guidata/tests/test_activable_dataset.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,59 +1,61 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright © 2009-2010 CEA
-# Pierre Raybaut
-# Licensed under the terms of the CECILL License
-# (see guidata/__init__.py for details)
+# Licensed under the terms of the BSD 3-Clause
+# (see guidata/LICENSE for details)
 
 """
 ActivableDataSet example
 
 Warning: ActivableDataSet objects were made to be integrated inside GUI layouts.
 So this example with dialog boxes may be confusing.
 --> see tests/editgroupbox.py to understand the activable dataset usage
 """
 
 # When editing, all items are shown.
 # When showing dataset in read-only mode (e.g. inside another layout), all items
 # are shown except the enable item.
 
-SHOW = True  # Show test in GUI-based test launcher
-
+from guidata.dataset.dataitems import BoolItem, ChoiceItem, ColorItem, FloatItem
 from guidata.dataset.datatypes import ActivableDataSet
-from guidata.dataset.dataitems import BoolItem, FloatItem, ChoiceItem, ColorItem
+from guidata.env import execenv
+from guidata.qthelpers import qt_app_context
+
+# guitest: show
 
 
-class ExampleDataSet(ActivableDataSet):
+class Parameters(ActivableDataSet):
     """
     Example
     <b>Activable dataset example</b>
     """
 
+    def __init__(self, title=None, comment=None, icon=""):
+        ActivableDataSet.__init__(self, title, comment, icon)
+
     enable = BoolItem(
         "Enable parameter set",
         help="If disabled, the following parameters will be ignored",
         default=False,
     )
     param0 = ChoiceItem("Param 0", ["choice #1", "choice #2", "choice #3"])
     param1 = FloatItem("Param 1", default=0, min=0)
     param2 = FloatItem("Param 2", default=0.93)
     color = ColorItem("Color", default="red")
 
 
-ExampleDataSet.active_setup()
+Parameters.active_setup()
 
 
-if __name__ == "__main__":
-    # Create QApplication
-    import guidata
+def test_activable_dataset():
+    """Test activable dataset"""
+    with qt_app_context():
+        prm = Parameters()
+        prm.set_writeable()
+        prm.edit()
+        prm.set_readonly()
+        prm.view()
+        execenv.print("OK")
 
-    _app = guidata.qapplication()
 
-    # Editing mode:
-    prm = ExampleDataSet()
-    prm.set_writeable()
-    prm.edit()
-
-    # Showing mode:
-    prm.set_readonly()
-    prm.view()
+if __name__ == "__main__":
+    test_activable_dataset()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `guidata-2.3.1/guidata/tests/activable_items.py` & `guidata-3.0.0/guidata/tests/test_activable_items.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright © 2012 CEA
-# Pierre Raybaut
-# Licensed under the terms of the CECILL License
-# (see guidata/__init__.py for details)
+# Licensed under the terms of the BSD 3-Clause
+# (see guidata/LICENSE for details)
 
 """
-Example with activable items: items which active state is changed depending 
+Example with activable items: items which active state is changed depending
 on another item's value.
 """
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 from guidata.dataset.dataitems import ChoiceItem, FloatItem
-from guidata.dataset.datatypes import DataSet, GetAttrProp, FuncProp
+from guidata.dataset.datatypes import DataSet, FuncProp, GetAttrProp
+from guidata.env import execenv
+from guidata.qthelpers import qt_app_context
 
 choices = (("A", "Choice #1: A"), ("B", "Choice #2: B"), ("C", "Choice #3: C"))
 
 
-class Test(DataSet):
+class Parameters(DataSet):
+    """Example dataset"""
+
     _prop = GetAttrProp("choice")
     choice = ChoiceItem("Choice", choices).set_prop("display", store=_prop)
     x1 = FloatItem("x1")
     x2 = FloatItem("x2").set_prop("display", active=FuncProp(_prop, lambda x: x == "B"))
     x3 = FloatItem("x3").set_prop("display", active=FuncProp(_prop, lambda x: x == "C"))
 
 
-if __name__ == "__main__":
-    # Create QApplication
-    import guidata
+def test_activable_items():
+    """Test activable items"""
+    with qt_app_context():
+        test = Parameters()
+        test.edit()
+        execenv.print("OK")
 
-    _app = guidata.qapplication()
 
-    test = Test()
-    test.edit()
+if __name__ == "__main__":
+    test_activable_items()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `guidata-2.3.1/guidata/tests/all_features.py` & `guidata-3.0.0/guidata/tests/test_all_features.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright © 2009-2010 CEA
-# Pierre Raybaut
-# Licensed under the terms of the CECILL License
-# (see guidata/__init__.py for details)
+# Licensed under the terms of the BSD 3-Clause
+# (see guidata/LICENSE for details)
 
 """
 All guidata item/group features demo
 """
 
+# guitest: show
 
-SHOW = True  # Show test in GUI-based test launcher
+import atexit
+import shutil
+import tempfile
 
-import tempfile, atexit, shutil
 import numpy as np
 
-from guidata.dataset.datatypes import (
-    DataSet,
-    BeginTabGroup,
-    EndTabGroup,
-    BeginGroup,
-    EndGroup,
-    ObjectItem,
-)
 from guidata.dataset.dataitems import (
-    FloatItem,
-    IntItem,
     BoolItem,
     ChoiceItem,
-    MultipleChoiceItem,
-    ImageChoiceItem,
-    FilesOpenItem,
-    StringItem,
-    TextItem,
     ColorItem,
-    FileSaveItem,
-    FileOpenItem,
+    DictItem,
     DirectoryItem,
+    FileOpenItem,
+    FileSaveItem,
+    FilesOpenItem,
     FloatArrayItem,
+    FloatItem,
+    ImageChoiceItem,
+    IntItem,
+    MultipleChoiceItem,
+    StringItem,
+    TextItem,
+)
+from guidata.dataset.datatypes import (
+    BeginGroup,
+    BeginTabGroup,
+    DataSet,
+    EndGroup,
+    EndTabGroup,
+    ObjectItem,
 )
-
-from guidata.dataset.qtwidgets import DataSetEditLayout, DataSetShowLayout
 from guidata.dataset.qtitemwidgets import DataSetWidget
-
+from guidata.dataset.qtwidgets import DataSetEditLayout, DataSetShowLayout
+from guidata.env import execenv
+from guidata.qthelpers import qt_app_context
 
 # Creating temporary files and registering cleanup functions
 TEMPDIR = tempfile.mkdtemp(prefix="test_")
 atexit.register(shutil.rmtree, TEMPDIR)
 FILE_ETA = tempfile.NamedTemporaryFile(suffix=".eta", dir=TEMPDIR)
 atexit.register(FILE_ETA.close)
 FILE_CSV = tempfile.NamedTemporaryFile(suffix=".csv", dir=TEMPDIR)
@@ -68,23 +69,30 @@
     klass = SubDataSet
 
 
 DataSetEditLayout.register(SubDataSetItem, SubDataSetWidget)
 DataSetShowLayout.register(SubDataSetItem, SubDataSetWidget)
 
 
-class TestParameters(DataSet):
+class Parameters(DataSet):
     """
     DataSet test
     The following text is the DataSet 'comment': <br>Plain text or
     <b>rich text<sup>2</sup></b> are both supported,
     as well as special characters (α, β, γ, δ, ...)
     """
 
-    files = SubDataSetItem("files")
+    dict_ = DictItem(
+        "dict_item",
+        {
+            "strings_col": ["a", "b", "c"],
+            "_col": [1, 2.0, 3],
+            "float_col": 1.0,
+        },
+    )
     string = StringItem("String")
     text = TextItem("Text")
     _bg = BeginGroup("A sub group")
     float_slider = FloatItem(
         "Float (with slider)", default=0.5, min=0, max=1, step=0.01, slider=True
     )
     fl1 = FloatItem(
@@ -127,25 +135,32 @@
         .set_prop("display", icon="file.png")
     )
     mchoice3 = MultipleChoiceItem("MC type 3", [str(i) for i in range(10)]).horizontal(
         2
     )
     eg0 = EndTabGroup("group")
     integer_slider = IntItem(
-        "Integer (with slider)", default=5, min=-50, max=100, slider=True
+        "Integer (with slider)", default=5, min=-50, max=-50, slider=True
     )
     integer = IntItem("Integer", default=5, min=3, max=6).set_pos(col=1)
 
 
-if __name__ == "__main__":
-    # Create QApplication
-    import guidata
+def test_all_features():
+    """Test all guidata item/group features"""
+    with qt_app_context():
+        e = Parameters()
+        e.floatarray[:, 0] = np.linspace(-5, 5, 50)
+        execenv.print(e)
+
+        if e.edit():
+            e.edit()
+            execenv.print(e)
+        e.view()
+
+        f = Parameters.create(integer=10101010, string="Using create class method")
+        print(f)
 
-    _app = guidata.qapplication()
+        execenv.print("OK")
 
-    e = TestParameters()
-    e.floatarray[:, 0] = np.linspace(-5, 5, 50)
-    print(e)
-    if e.edit():
-        e.edit()
-        print(e)
-    e.view()
+
+if __name__ == "__main__":
+    test_all_features()
```

### Comparing `guidata-2.3.1/guidata/tests/all_items.py` & `guidata-3.0.0/guidata/tests/test_all_items.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright © 2009-2010 CEA
-# Pierre Raybaut
-# Licensed under the terms of the CECILL License
-# (see guidata/__init__.py for details)
+# Licensed under the terms of the BSD 3-Clause
+# (see guidata/LICENSE for details)
 
 """
 All guidata DataItem objects demo
 
 A DataSet object is a set of parameters of various types (integer, float,
 boolean, string, etc.) which may be edited in a dialog box thanks to the
 'edit' method. Parameters are defined by assigning DataItem objects to a
 DataSet class definition: each parameter type has its own DataItem class
 (IntItem for integers, FloatItem for floats, StringItem for strings, etc.)
 """
 
+# guitest: show
 
-SHOW = True  # Show test in GUI-based test launcher
+import atexit
+import datetime
+import shutil
+import tempfile
 
-import tempfile, atexit, shutil, datetime, numpy as np
+import numpy as np
 
-import guidata.dataset.datatypes as gdt
 import guidata.dataset.dataitems as gdi
-
+import guidata.dataset.datatypes as gdt
+from guidata.env import execenv
+from guidata.qthelpers import qt_app_context
 
 # Creating temporary files and registering cleanup functions
 TEMPDIR = tempfile.mkdtemp(prefix="test_")
 atexit.register(shutil.rmtree, TEMPDIR)
 FILE_ETA = tempfile.NamedTemporaryFile(suffix=".eta", dir=TEMPDIR)
 atexit.register(FILE_ETA.close)
 FILE_CSV = tempfile.NamedTemporaryFile(suffix=".csv", dir=TEMPDIR)
 atexit.register(FILE_CSV.close)
 
 
-class TestParameters(gdt.DataSet):
+class Parameters(gdt.DataSet):
     """
     DataSet test
     The following text is the DataSet 'comment': <br>Plain text or
     <b>rich text<sup>2</sup></b> are both supported,
     as well as special characters (α, β, γ, δ, ...)
     """
 
@@ -83,19 +86,22 @@
             "MC type 2", ["first choice", "second choice", "third choice"]
         )
         .vertical(1)
         .set_pos(col=1)
     )
 
 
-if __name__ == "__main__":
-    # Create QApplication
-    import guidata
+def test_all_items():
+    """Test all DataItem objects"""
+    with qt_app_context():
+        e = Parameters()
+
+        e.floatarray[:, 0] = np.linspace(-5, 5, 50)
+        execenv.print(e)
+        if e.edit():
+            execenv.print(e)
+        e.view()
+        execenv.print("OK")
 
-    _app = guidata.qapplication()
 
-    e = TestParameters()
-    e.floatarray[:, 0] = np.linspace(-5, 5, 50)
-    print(e)
-    if e.edit():
-        print(e)
-    e.view()
+if __name__ == "__main__":
+    test_all_items()
```

### Comparing `guidata-2.3.1/guidata/tests/bool_selector.py` & `guidata-3.0.0/guidata/tests/test_bool_selector.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright © 2009-2010 CEA
-# Pierre Raybaut
-# Licensed under the terms of the CECILL License
-# (see guidata/__init__.py for details)
+# Licensed under the terms of the BSD 3-Clause
+# (see guidata/LICENSE for details)
 
 """
 DataItem groups and group selection
 
 DataSet items may be included in groups (these items are then shown in group
 box widgets in the editing dialog box) and item groups may be enabled/disabled
 using one group parameter (a boolean item).
 """
 
+# guitest: show
 
-SHOW = True  # Show test in GUI-based test launcher
-
-from guidata.dataset.datatypes import DataSet, BeginGroup, EndGroup, ValueProp
 from guidata.dataset.dataitems import BoolItem, FloatItem
+from guidata.dataset.datatypes import BeginGroup, DataSet, EndGroup, ValueProp
+from guidata.env import execenv
+from guidata.qthelpers import qt_app_context
 
 prop1 = ValueProp(False)
 prop2 = ValueProp(False)
 
 
-class GroupSelection(DataSet):
+class Parameters(DataSet):
     """
     Group selection test
     <b>Group selection example:</b>
     """
 
     g1 = BeginGroup("group 1")
     enable1 = BoolItem(
@@ -49,16 +48,18 @@
     param2_1 = FloatItem("Param 2.1", default=0, min=0).set_prop(
         "display", active=prop2
     )
     param2_2 = FloatItem("Param 2.2", default=0.93).set_prop("display", active=prop2)
     _g2 = EndGroup("group 2")
 
 
-if __name__ == "__main__":
-    # Create QApplication
-    import guidata
+def test_bool_selector():
+    """Test bool selector"""
+    with qt_app_context():
+        prm = Parameters()
+        prm.edit()
+        execenv.print(prm)
+        execenv.print("OK")
 
-    _app = guidata.qapplication()
 
-    prm = GroupSelection()
-    prm.edit()
-    print(prm)
+if __name__ == "__main__":
+    test_bool_selector()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `guidata-2.3.1/guidata/tests/callbacks.py` & `guidata-3.0.0/guidata/tests/test_callbacks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright © 2009-2011 CEA
-# Pierre Raybaut
-# Licensed under the terms of the CECILL License
-# (see guidata/__init__.py for details)
+# Licensed under the terms of the BSD 3-Clause
+# (see guidata/LICENSE for details)
 
 """
 Demonstrates how items may trigger callbacks when activated
 """
 
+# guitest: show
 
-SHOW = True  # Show test in GUI-based test launcher
-
-
-from guidata.dataset.datatypes import DataSet
 from guidata.dataset.dataitems import (
     ChoiceItem,
-    StringItem,
-    TextItem,
     ColorItem,
     FloatItem,
+    StringItem,
+    TextItem,
 )
+from guidata.dataset.datatypes import DataSet
+from guidata.env import execenv
+from guidata.qthelpers import qt_app_context
+
 
+class Parameters(DataSet):
+    """Example dataset"""
 
-class TestParameters(DataSet):
     def cb_example(self, item, value):
-        print("\nitem: ", item, "\nvalue:", value)
+        execenv.print("\nitem: ", item, "\nvalue:", value)
         if self.results is None:
             self.results = ""
         self.results += str(value) + "\n"
-        print("results:", self.results)
+        execenv.print("results:", self.results)
 
     def update_x1plusx2(self, item, value):
-        print("\nitem: ", item, "\nvalue:", value)
+        execenv.print("\nitem: ", item, "\nvalue:", value)
         if self.x1 is not None and self.x2 is not None:
             self.x1plusx2 = self.x1 + self.x2
         else:
             self.x1plusx2 = None
 
     string = StringItem("String", default="foobar").set_prop(
         "display", callback=cb_example
@@ -53,18 +53,20 @@
         )
         .set_pos(col=1, colspan=2)
         .set_prop("display", callback=cb_example)
     )
     results = TextItem("Results")
 
 
-if __name__ == "__main__":
-    # Create QApplication
-    import guidata
+def test_callbacks():
+    """Test callbacks"""
+    with qt_app_context():
+        e = Parameters()
+        execenv.print(e)
+        if e.edit():
+            execenv.print(e)
+        e.view()
+        execenv.print("OK")
 
-    _app = guidata.qapplication()
 
-    e = TestParameters()
-    print(e)
-    if e.edit():
-        print(e)
-    e.view()
+if __name__ == "__main__":
+    test_callbacks()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `guidata-2.3.1/guidata/tests/data.py` & `guidata-3.0.0/guidata/tests/test_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright © 2009-2010 CEA
-# Pierre Raybaut
-# Licensed under the terms of the CECILL License
-# (see guidata/__init__.py for details)
+# Licensed under the terms of the BSD 3-Clause
+# (see guidata/LICENSE for details)
 
 """Unit tests"""
 
-SHOW = False  # Do not show test in GUI-based test launcher
 
 import unittest
-from guidata.dataset.datatypes import DataSet
+
 from guidata.dataset.dataitems import FloatItem, IntItem
+from guidata.dataset.datatypes import DataSet
+from guidata.env import execenv
 from guidata.utils import update_dataset
 
 
 class Parameters(DataSet):
+    """Example dataset"""
+
     float1 = FloatItem("float #1", min=1, max=250, help="height in cm")
     float2 = FloatItem("float #2", min=1, max=250, help="width in cm")
     number = IntItem("number", min=3, max=20)
 
 
 class TestCheck(unittest.TestCase):
     def test_range(self):
         """Test range checking of FloatItem"""
         e = Parameters()
         e.float1 = 150.0
         e.float2 = 400.0
         e.number = 4
         errors = e.check()
-        self.assertEquals(errors, ["float2"])
+        self.assertEqual(errors, ["float2"])
 
     def test_typechecking(self):
         """Test type checking of FloatItem"""
         e = Parameters()
         e.float1 = 150
         e.float2 = 400
         e.number = 4.0
         errors = e.check()
-        self.assertEquals(errors, ["float1", "float2", "number"])
+        self.assertEqual(errors, ["float1", "float2", "number"])
 
     def test_update(self):
         e1 = Parameters()
         e2 = Parameters()
         e1.float1 = 23
         update_dataset(e2, e1)
-        self.assertEquals(e2.float1, 23)
+        self.assertEqual(e2.float1, 23)
 
 
 if __name__ == "__main__":
     unittest.main()
+    execenv.print("OK")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `guidata-2.3.1/guidata/tests/disthelpers.py` & `guidata-3.0.0/guidata/tests/test_disthelpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright © 2011 CEA
-# Pierre Raybaut
-# Licensed under the terms of the CECILL License
-# (see guidata/__init__.py for details)
+# Licensed under the terms of the BSD 3-Clause
+# (see guidata/LICENSE for details)
 
 """
 guidata.disthelpers demo
 
 How to create an executable with py2exe or cx_Freeze with less efforts than
 writing a complete setup script.
 """
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 import os.path as osp
 
-from guidata.disthelpers import Distribution
+import pytest
 
-if __name__ == "__main__":
+from guidata.env import execenv
+from guidata.utils.disthelpers import Distribution
+
+
+@pytest.mark.skip(reason="Currently not supporting Python > 3.6")
+def test_disthelpers():
+    """Test disthelpers"""
     dist = Distribution()
     dist.setup(
         name="Application demo",
         version="1.0.0",
         description="Application demo based on editgroupbox.py",
-        script=osp.join(osp.dirname(__file__), "editgroupbox.py"),
+        script=osp.join(osp.dirname(__file__), "test_editgroupbox.py"),
         target_name="demo.exe",
     )
     dist.add_modules("guidata")
     dist.build("cx_Freeze")
+    execenv.print("OK")
+
+
+if __name__ == "__main__":
+    test_disthelpers()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `guidata-2.3.1/guidata/tests/editgroupbox.py` & `guidata-3.0.0/guidata/tests/test_editgroupbox.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright © 2009-2010 CEA
-# Pierre Raybaut
-# Licensed under the terms of the CECILL License
-# (see guidata/__init__.py for details)
+# Licensed under the terms of the BSD 3-Clause
+# (see guidata/LICENSE for details)
 
 """
 DataSetEditGroupBox and DataSetShowGroupBox demo
 
 These group box widgets are intended to be integrated in a GUI application
 layout, showing read-only parameter sets or allowing to edit parameter values.
 """
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 from qtpy.QtWidgets import QMainWindow, QSplitter
 
-from guidata.dataset import datatypes as gdt
-from guidata.dataset import dataitems as gdi
-from guidata.dataset.qtwidgets import DataSetShowGroupBox, DataSetEditGroupBox
 from guidata.configtools import get_icon
+from guidata.dataset import dataitems as gdi
+from guidata.dataset import datatypes as gdt
+from guidata.dataset.qtwidgets import DataSetEditGroupBox, DataSetShowGroupBox
+from guidata.env import execenv
 from guidata.qthelpers import (
-    create_action,
     add_actions,
+    create_action,
     get_std_icon,
+    qt_app_context,
     win32_fix_title_bar_background,
 )
 
 # Local test import:
-from guidata.tests.activable_dataset import ExampleDataSet
+from guidata.tests.test_activable_dataset import Parameters
 
 
 class AnotherDataSet(gdt.DataSet):
     """
     Example 2
     <b>Simple dataset example</b>
     """
@@ -42,14 +42,16 @@
     a_group = gdt.BeginGroup("A group")
     param2 = gdi.FloatItem("Foobar 2", default=0.93)
     param3 = gdi.FloatItem("Foobar 3", default=123)
     _a_group = gdt.EndGroup("A group")
 
 
 class ExampleMultiGroupDataSet(gdt.DataSet):
+    """Example DS with multiple groups"""
+
     param0 = gdi.ChoiceItem("Choice", ["deazdazk", "aeazee", "87575757"])
     param1 = gdi.FloatItem("Foobar 1", default=0, min=0)
     t_group = gdt.BeginTabGroup("T group")
     a_group = gdt.BeginGroup("A group")
     param2 = gdi.FloatItem("Foobar 2", default=0.93)
     dir1 = gdi.DirectoryItem("Directory 1")
     file1 = gdi.FileOpenItem("File 1")
@@ -63,36 +65,40 @@
     param6 = gdi.DateItem("Date")
     param7 = gdi.ColorItem("Color")
     _c_group = gdt.EndGroup("C group")
     _t_group = gdt.EndTabGroup("T group")
 
 
 class OtherDataSet(gdt.DataSet):
+    """Another example dataset"""
+
     title = gdi.StringItem("Title", default="Title")
     icon = gdi.ChoiceItem(
         "Icon",
         (
             ("python.png", "Python"),
             ("guidata.svg", "guidata"),
             ("settings.png", "Settings"),
         ),
     )
     opacity = gdi.FloatItem("Opacity", default=1.0, min=0.1, max=1)
 
 
 class MainWindow(QMainWindow):
+    """Main window"""
+
     def __init__(self):
         QMainWindow.__init__(self)
         win32_fix_title_bar_background(self)
         self.setWindowIcon(get_icon("python.png"))
         self.setWindowTitle("Application example")
 
         # Instantiate dataset-related widgets:
         self.groupbox1 = DataSetShowGroupBox(
-            "Activable dataset", ExampleDataSet, comment=""
+            "Activable dataset", Parameters, comment=""
         )
         self.groupbox2 = DataSetShowGroupBox(
             "Standard dataset", AnotherDataSet, comment=""
         )
         self.groupbox3 = DataSetEditGroupBox(
             "Standard dataset", OtherDataSet, comment=""
         )
@@ -134,39 +140,47 @@
             self, "Edit dataset 4", triggered=self.edit_dataset4
         )
         add_actions(
             edit_menu, (editparam1_action, editparam2_action, editparam4_action)
         )
 
     def update_window(self):
+        """Update window"""
         dataset = self.groupbox3.dataset
         self.setWindowTitle(dataset.title)
         self.setWindowIcon(get_icon(dataset.icon))
         self.setWindowOpacity(dataset.opacity)
 
     def update_groupboxes(self):
+        """Update groupboxes"""
         self.groupbox1.dataset.set_readonly()  # This is an activable dataset
         self.groupbox1.get()
         self.groupbox2.get()
         self.groupbox4.get()
 
     def edit_dataset1(self):
+        """Edit dataset 1"""
         self.groupbox1.dataset.set_writeable()  # This is an activable dataset
         if self.groupbox1.dataset.edit(self):
             self.update_groupboxes()
 
     def edit_dataset2(self):
+        """Edit dataset 2"""
         if self.groupbox2.dataset.edit(self):
             self.update_groupboxes()
 
     def edit_dataset4(self):
+        """Edit dataset 4"""
         if self.groupbox4.dataset.edit(self):
             self.update_groupboxes()
 
 
-if __name__ == "__main__":
-    from guidata import qapplication
+def test_editgroupbox():
+    """Test editgroupbox"""
+    with qt_app_context(exec_loop=True):
+        window = MainWindow()
+        window.show()
+        execenv.print("OK")
+
 
-    app = qapplication()
-    window = MainWindow()
-    window.show()
-    app.exec_()
+if __name__ == "__main__":
+    test_editgroupbox()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `guidata-2.3.1/guidata/tests/inheritance.py` & `guidata-3.0.0/guidata/tests/test_inheritance.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright © 2009-2010 CEA
-# Pierre Raybaut
-# Licensed under the terms of the CECILL License
-# (see guidata/__init__.py for details)
+# Licensed under the terms of the BSD 3-Clause
+# (see guidata/LICENSE for details)
 
 """
 DataSet objects inheritance test
 
 From time to time, it may be useful to derive a DataSet from another. The main
 application is to extend a parameter set with additionnal parameters.
 """
 
+# guitest: show
 
-SHOW = True  # Show test in GUI-based test launcher
-
-import guidata.dataset.datatypes as gdt
 import guidata.dataset.dataitems as gdi
+import guidata.dataset.datatypes as gdt
+from guidata.env import execenv
+from guidata.qthelpers import qt_app_context
 
 
 class OriginalDataset(gdt.DataSet):
     """Original dataset
     This is the original dataset"""
 
     bool = gdi.BoolItem("Boolean")
@@ -35,20 +34,22 @@
 
     bool = gdi.BoolItem("Boolean (modified in derived dataset)")
     a = gdi.FloatItem("Level 1 (added in derived dataset)", default=0)
     b = gdi.FloatItem("Level 2 (added in derived dataset)", default=0)
     c = gdi.FloatItem("Level 3 (added in derived dataset)", default=0)
 
 
-if __name__ == "__main__":
-    # Create QApplication
-    import guidata
+def test_inheritance():
+    """Test DataSet inheritance"""
+    with qt_app_context():
+        e = OriginalDataset()
+        e.edit()
+        execenv.print(e)
+
+        e = DerivedDataset()
+        e.edit()
+        execenv.print(e)
+        execenv.print("OK")
 
-    _app = guidata.qapplication()
 
-    e = OriginalDataset()
-    e.edit()
-    print(e)
-
-    e = DerivedDataset()
-    e.edit()
-    print(e)
+if __name__ == "__main__":
+    test_inheritance()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `guidata-2.3.1/guidata/tests/item_order.py` & `guidata-3.0.0/guidata/tests/test_item_order.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright © 2009-2010 CEA
-# Pierre Raybaut
-# Licensed under the terms of the CECILL License
-# (see guidata/__init__.py for details)
+# Licensed under the terms of the BSD 3-Clause
+# (see guidata/LICENSE for details)
 
 """
 DataSet item order test
 
 From time to time, it may be useful to change the item order,
 for example when deriving a dataset from another.
 """
 
+# guitest: show
 
-SHOW = True  # Show test in GUI-based test launcher
-
-import guidata.dataset.datatypes as gdt
 import guidata.dataset.dataitems as gdi
+import guidata.dataset.datatypes as gdt
+from guidata.env import execenv
+from guidata.qthelpers import qt_app_context
 
 
 class OriginalDataset(gdt.DataSet):
     """Original dataset
     This is the original dataset"""
 
     param1 = gdi.BoolItem("P1 | Boolean")
@@ -33,20 +32,22 @@
     """Derived dataset
     This is the derived dataset, with modified item order"""
 
     param5 = gdi.IntItem("P5 | Int", default=0).set_pos(row=2)
     param6 = gdi.DateItem("P6 | Date", default=0).set_pos(row=4)
 
 
-if __name__ == "__main__":
-    # Create QApplication
-    import guidata
+def test_item_order():
+    """Test DataSet item order"""
+    with qt_app_context():
+        e = OriginalDataset()
+        e.edit()
+        execenv.print(e)
+
+        e = DerivedDataset()
+        e.edit()
+        execenv.print(e)
+        execenv.print("OK")
 
-    _app = guidata.qapplication()
 
-    e = OriginalDataset()
-    e.edit()
-    print(e)
-
-    e = DerivedDataset()
-    e.edit()
-    print(e)
+if __name__ == "__main__":
+    test_item_order()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `guidata-2.3.1/guidata/tests/loadsave_hdf5.py` & `guidata-3.0.0/guidata/tests/test_loadsave_hdf5.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright © 2009-2010 CEA
-# Pierre Raybaut
-# Licensed under the terms of the CECILL License
-# (see guidata/__init__.py for details)
+# Licensed under the terms of the BSD 3-Clause
+# (see guidata/LICENSE for details)
 
 """
 HDF5 I/O demo
 
 DataSet objects may be saved in HDF5 files, a universal hierarchical dataset
 file type. This script shows how to save in and then reload data from a HDF5
 file.
 """
 
-try:
-    import guidata.hdf5io  # @UnusedImport
-
-    hdf5_is_available = True
-except ImportError:
-    hdf5_is_available = False
-
-SHOW = hdf5_is_available  # Show test in GUI-based test launcher
+# guitest: show
 
 import os
 
-from guidata.hdf5io import HDF5Reader, HDF5Writer
-from guidata.tests.all_items import TestParameters
-
-if __name__ == "__main__":
-    # Create QApplication
-    import guidata
-
-    _app = guidata.qapplication()
+from guidata.dataset.hdf5io import HDF5Reader, HDF5Writer
+from guidata.env import execenv
+from guidata.qthelpers import qt_app_context
+from guidata.tests.test_all_items import Parameters
+
+
+def test_loadsave_hdf5():
+    """Test HDF5 I/O"""
+    with qt_app_context():
+        if os.path.exists("test.h5"):
+            os.unlink("test.h5")
+
+        e = Parameters()
+        if execenv.unattended or e.edit():
+            writer = HDF5Writer("test.h5")
+            e.serialize(writer)
+            writer.close()
+
+            e = Parameters()
+            reader = HDF5Reader("test.h5")
+            e.deserialize(reader)
+            reader.close()
+            e.edit()
+        execenv.print("OK")
 
-    if os.path.exists("test.h5"):
-        os.unlink("test.h5")
 
-    e = TestParameters()
-    if e.edit():
-        writer = HDF5Writer("test.h5")
-        e.serialize(writer)
-        writer.close()
-
-        e = TestParameters()
-        reader = HDF5Reader("test.h5")
-        e.deserialize(reader)
-        reader.close()
-        e.edit()
+if __name__ == "__main__":
+    test_loadsave_hdf5()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `guidata-2.3.1/guidata/tests/test_arrayeditor.py` & `guidata-3.0.0/guidata/tests/test_arrayeditor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,79 +1,82 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright © Spyder Project Contributors
 # Licensed under the terms of the MIT License
 
-SHOW = True  # Show test in GUI-based test launcher
 
 """
 Tests for arrayeditor.py
 """
 
+# guitest: show
+
 import numpy as np
 
-# Local imports
-from guidata import qapplication
+from guidata.env import execenv
+from guidata.qthelpers import exec_dialog, qt_app_context
 from guidata.widgets.arrayeditor import ArrayEditor
 
 
 def launch_arrayeditor(data, title="", xlabels=None, ylabels=None):
     """Helper routine to launch an arrayeditor and return its result"""
     dlg = ArrayEditor()
     dlg.setup_and_check(data, title, xlabels=xlabels, ylabels=ylabels)
-    dlg.exec_()
+    exec_dialog(dlg)
     return dlg.get_value()
 
 
 def test_arrayeditor():
     """Test array editor for all supported data types"""
-    for title, data in (
-        ("string array", np.array(["kjrekrjkejr"])),
-        ("unicode array", np.array([u"ñññéáíó"])),
-        (
-            "masked array",
-            np.ma.array([[1, 0], [1, 0]], mask=[[True, False], [False, False]]),
-        ),
-        (
-            "record array",
-            np.zeros(
-                (2, 2),
-                {
-                    "names": ("red", "green", "blue"),
-                    "formats": (np.float32, np.float32, np.float32),
-                },
+    with qt_app_context():
+        for title, data in (
+            ("string array", np.array(["kjrekrjkejr"])),
+            ("unicode array", np.array(["ñññéáíó"])),
+            (
+                "masked array",
+                np.ma.array([[1, 0], [1, 0]], mask=[[True, False], [False, False]]),
+            ),
+            (
+                "record array",
+                np.zeros(
+                    (2, 2),
+                    {
+                        "names": ("red", "green", "blue"),
+                        "formats": (np.float32, np.float32, np.float32),
+                    },
+                ),
+            ),
+            (
+                "record array with titles",
+                np.array(
+                    [(0, 0.0), (0, 0.0), (0, 0.0)],
+                    dtype=[(("title 1", "x"), "|i1"), (("title 2", "y"), ">f4")],
+                ),
             ),
-        ),
-        (
-            "record array with titles",
-            np.array(
-                [(0, 0.0), (0, 0.0), (0, 0.0)],
-                dtype=[(("title 1", "x"), "|i1"), (("title 2", "y"), ">f4")],
+            ("bool array", np.array([True, False, True])),
+            ("int array", np.array([1, 2, 3], dtype="int8")),
+            ("float16 array", np.zeros((5, 5), dtype=np.float16)),
+        ):
+            launch_arrayeditor(data, title)
+        for title, data, xlabels, ylabels in (
+            ("float array", np.random.rand(5, 5), ["a", "b", "c", "d", "e"], None),
+            (
+                "complex array",
+                np.round(np.random.rand(5, 5) * 10)
+                + np.round(np.random.rand(5, 5) * 10) * 1j,
+                np.linspace(-12, 12, 5),
+                np.linspace(-12, 12, 5),
             ),
-        ),
-        ("bool array", np.array([True, False, True])),
-        ("int array", np.array([1, 2, 3], dtype="int8")),
-        ("float16 array", np.zeros((5, 5), dtype=np.float16)),
-    ):
-        launch_arrayeditor(data, title)
-    for title, data, xlabels, ylabels in (
-        ("float array", np.random.rand(5, 5), ["a", "b", "c", "d", "e"], None),
-        (
-            "complex array",
-            np.round(np.random.rand(5, 5) * 10)
-            + np.round(np.random.rand(5, 5) * 10) * 1j,
-            np.linspace(-12, 12, 5),
-            np.linspace(-12, 12, 5),
-        ),
-    ):
-        launch_arrayeditor(data, title, xlabels, ylabels)
-
-    arr = np.zeros((3, 3, 4))
-    arr[0, 0, 0] = 1
-    arr[0, 0, 1] = 2
-    arr[0, 0, 2] = 3
-    launch_arrayeditor(arr, "3D array")
+        ):
+            launch_arrayeditor(data, title, xlabels, ylabels)
+
+        arr = np.zeros((3, 3, 4))
+        arr[0, 0, 0] = 1
+        arr[0, 0, 1] = 2
+        arr[0, 0, 2] = 3
+        launch_arrayeditor(arr, "3D array")
+
+        execenv.print("OK")
 
 
 if __name__ == "__main__":
-    app = qapplication()
     test_arrayeditor()
```

### Comparing `guidata-2.3.1/guidata/tests/test_codeeditor.py` & `guidata-3.0.0/guidata/tests/test_codeeditor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright © Spyder Project Contributors
 # Licensed under the terms of the MIT License
 
-SHOW = True  # Show test in GUI-based test launcher
 
 """
 Tests for codeeditor.py
 """
 
-# Local imports
-from guidata import qapplication
+# guitest: show
+
+from guidata.env import execenv
+from guidata.qthelpers import qt_app_context
 from guidata.widgets import codeeditor
 
 
 def test_codeeditor():
     """Test Code editor."""
-
-    app = qapplication()
-
-    widget = codeeditor.CodeEditor(language="python")
-    widget.set_text_from_file(codeeditor.__file__)
-    widget.resize(800, 600)
-    widget.show()
-    app.exec_()
+    with qt_app_context(exec_loop=True):
+        widget = codeeditor.CodeEditor(language="python")
+        widget.set_text_from_file(codeeditor.__file__)
+        widget.resize(800, 600)
+        widget.show()
+        execenv.print("OK")
 
 
 if __name__ == "__main__":
     test_codeeditor()
```

### Comparing `guidata-2.3.1/guidata/tests/test_collectionseditor.py` & `guidata-3.0.0/guidata/tests/test_collectionseditor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright © Spyder Project Contributors
 # Licensed under the terms of the MIT License
 
-SHOW = True  # Show test in GUI-based test launcher
 
 """
 Tests for collectionseditor.py
 """
 
+# guitest: show
+
 import datetime
-import numpy as np
 
-# Local imports
-from guidata import qapplication
+from guidata.env import execenv
+from guidata.qthelpers import qt_app_context
 from guidata.widgets.collectionseditor import CollectionsEditor
 
 
 def get_test_data():
     """Create test data."""
     import numpy as np
     from PIL import Image
@@ -45,15 +45,15 @@
                 "string_col": ["a", "b", "c", "d"],
                 "int_col": [0, 1, 2, 3],
                 "float_col": [1.1, 2.2, 3.3, 4.4],
                 "bool_col": [True, False, False, True],
             }
         )
 
-    class Foobar(object):
+    class Foobar:
         """ """
 
         def __init__(self):
             self.text = "toto"
             self.testdict = testdict
             self.testdate = testdate
 
@@ -105,17 +105,16 @@
             1000, dtype=[("ID", "f8"), ("param1", "f8", 5000)]
         ),
     }
 
 
 def test_collectionseditor():
     """Test Collections editor."""
-    app = qapplication()
-
-    dialog = CollectionsEditor()
-    dialog.setup(get_test_data())
-    dialog.show()
-    app.exec_()
+    with qt_app_context(exec_loop=True):
+        dialog = CollectionsEditor()
+        dialog.setup(get_test_data())
+        dialog.show()
+        execenv.print("OK")
 
 
 if __name__ == "__main__":
     test_collectionseditor()
```

### Comparing `guidata-2.3.1/guidata/tests/test_dataframeeditor.py` & `guidata-3.0.0/guidata/tests/test_dataframeeditor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,70 +1,72 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright © Spyder Project Contributors
 # Licensed under the terms of the MIT License
 
-SHOW = True  # Show test in GUI-based test launcher
 
 """
 Tests for dataframeeditor.py
 """
 
+# guitest: show
+
 import numpy as np
 from numpy import nan
 from pandas import DataFrame, Series
 from pandas.testing import assert_frame_equal, assert_series_equal
 
-# Local imports
-from guidata import qapplication
+from guidata.env import execenv
+from guidata.qthelpers import exec_dialog, qt_app_context
 from guidata.widgets.dataframeeditor import DataFrameEditor
 
 
-def test_edit(data, title="", parent=None):
-    """Test subroutine"""
-    dlg = DataFrameEditor(parent=parent)
-
-    if dlg.setup_and_check(data, title=title):
-        dlg.exec_()
-        return dlg.get_value()
-    else:
-        import sys
-
-        sys.exit(1)
-
-
 def test_dataframeeditor():
     """DataFrame editor test"""
-    app = qapplication()  # analysis:ignore
 
-    df1 = DataFrame(
-        [
-            [True, "bool"],
-            [1 + 1j, "complex"],
-            ["test", "string"],
-            [1.11, "float"],
-            [1, "int"],
-            [np.random.rand(3, 3), "Unkown type"],
-            ["Large value", 100],
-            ["áéí", "unicode"],
-        ],
-        index=["a", "b", nan, nan, nan, "c", "Test global max", "d"],
-        columns=[nan, "Type"],
-    )
-    out = test_edit(df1)
-    assert_frame_equal(df1, out)
-
-    result = Series([True, "bool"], index=[nan, "Type"], name="a")
-    out = test_edit(df1.iloc[0])
-    assert_series_equal(result, out)
-
-    df1 = DataFrame(np.random.rand(100100, 10))
-    out = test_edit(df1)
-    assert_frame_equal(out, df1)
-
-    series = Series(np.arange(10), name=0)
-    out = test_edit(series)
-    assert_series_equal(series, out)
+    def test_edit(data, title="", parent=None):
+        """Test subroutine"""
+        dlg = DataFrameEditor(parent=parent)
+
+        if dlg.setup_and_check(data, title=title):
+            exec_dialog(dlg)
+            return dlg.get_value()
+        else:
+            import sys
+
+            sys.exit(1)
+
+    with qt_app_context():
+        df1 = DataFrame(
+            [
+                [True, "bool"],
+                [1 + 1j, "complex"],
+                ["test", "string"],
+                [1.11, "float"],
+                [1, "int"],
+                [np.random.rand(3, 3), "Unkown type"],
+                ["Large value", 100],
+                ["áéí", "unicode"],
+            ],
+            index=["a", "b", nan, nan, nan, "c", "Test global max", "d"],
+            columns=[nan, "Type"],
+        )
+        out = test_edit(df1)
+        assert_frame_equal(df1, out)
+
+        result = Series([True, "bool"], index=[nan, "Type"], name="a")
+        out = test_edit(df1.iloc[0])
+        assert_series_equal(result, out)
+
+        df1 = DataFrame(np.random.rand(100100, 10))
+        out = test_edit(df1)
+        assert_frame_equal(out, df1)
+
+        series = Series(np.arange(10), name=0)
+        out = test_edit(series)
+        assert_series_equal(series, out)
+
+        execenv.print("OK")
 
 
 if __name__ == "__main__":
     test_dataframeeditor()
```

### Comparing `guidata-2.3.1/guidata/tests/test_objecteditor.py` & `guidata-3.0.0/guidata/tests/test_objecteditor.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,52 +2,53 @@
 #
 # Copyright © Spyder Project Contributors
 # Licensed under the terms of the MIT License
 """
 Tests for objecteditor.py
 """
 
+# guitest: show
+
 import datetime
 
 import numpy as np
 import PIL.Image
-from guidata import qapplication
-from guidata.widgets.objecteditor import oedit
 
-SHOW = True  # Show test in GUI-based test launcher
+from guidata.env import execenv
+from guidata.qthelpers import qt_app_context
+from guidata.widgets.objecteditor import oedit
 
 
-def test():
+def test_objecteditor():
     """Run object editor test"""
-    data = np.random.randint(255, size=(100, 100)).astype("uint8")
-    image = PIL.Image.fromarray(data)
-    example = {
-        "str": "kjkj kj k j j kj k jkj",
-        "list": [1, 3, 4, "kjkj", None],
-        "dict": {"d": 1, "a": np.random.rand(10, 10), "b": [1, 2]},
-        "float": 1.2233,
-        "array": np.random.rand(10, 10),
-        "image": image,
-        "date": datetime.date(1945, 5, 8),
-        "datetime": datetime.datetime(1945, 5, 8),
-    }
-    image = oedit(image)
-
-    class Foobar(object):
-        """ """
-
-        def __init__(self):
-            self.text = "toto"
-
-    foobar = Foobar()
-    print(oedit(foobar))
-    print(oedit(example))
-    print(oedit(np.random.rand(10, 10)))
-    print(oedit(oedit.__doc__))
-    print(example)
+    with qt_app_context():
+        data = np.random.randint(255, size=(100, 100)).astype("uint8")
+        image = PIL.Image.fromarray(data)
+        example = {
+            "str": "kjkj kj k j j kj k jkj",
+            "list": [1, 3, 4, "kjkj", None],
+            "dict": {"d": 1, "a": np.random.rand(10, 10), "b": [1, 2]},
+            "float": 1.2233,
+            "array": np.random.rand(10, 10),
+            "image": image,
+            "date": datetime.date(1945, 5, 8),
+            "datetime": datetime.datetime(1945, 5, 8),
+        }
+        image = oedit(image)
+
+        class Foobar:
+            """ """
+
+            def __init__(self):
+                self.text = "toto"
+
+        foobar = Foobar()
+        execenv.print(oedit(foobar))
+        execenv.print(oedit(example))
+        execenv.print(oedit(np.random.rand(10, 10)))
+        execenv.print(oedit(oedit.__doc__))
+        execenv.print(example)
+        execenv.print("OK")
 
 
 if __name__ == "__main__":
-    from guidata import qapplication
-
-    app = qapplication()
-    test()
+    test_objecteditor()
```

### Comparing `guidata-2.3.1/guidata/tests/userconfig_app.py` & `guidata-3.0.0/guidata/tests/test_userconfig_app.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,23 +10,32 @@
 [main]
 version = 1.0.0
 
 [a]
 b/f = 1.0
 """
 
-from guidata.dataset import datatypes as gdt
-from guidata.dataset import dataitems as gdi
 from guidata import userconfig
+from guidata.dataset import dataitems as gdi
+from guidata.dataset import datatypes as gdt
+from guidata.env import execenv
 
 
 class DS(gdt.DataSet):
+    """Example dataset"""
+
     f = gdi.FloatItem("F", 1.0)
 
 
-if __name__ == "__main__":
+def test_userconfig_app():
+    """Test userconfig"""
     ds = DS("")
     uc = userconfig.UserConfig({})
     uc.set_application("app", "1.0.0")
     ds.write_config(uc, "a", "b")
 
     print("Settings saved in: ", uc.filename())
+    execenv.print("OK")
+
+
+if __name__ == "__main__":
+    test_userconfig_app()
```

### Comparing `guidata-2.3.1/guidata/userconfig.py` & `guidata-3.0.0/guidata/userconfig.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,121 +32,133 @@
 userconfig
 ----------
 
 The ``guidata.userconfig`` module provides user configuration file (.ini file)
 management features based on ``ConfigParser`` (standard Python library).
 
 It is the exact copy of the open-source package `userconfig` (MIT license).
-
-19/12/2021: Removed Python 2 compatibility
 """
 
-
-__version__ = "1.1.0"
-
+import configparser as cp
 import os
-import re
 import os.path as osp
+import re
 import sys
-import configparser as cp
-
-
-def _check_values(sections):
-    # Checks if all key/value pairs are writable
-    err = False
-    for section, data in list(sections.items()):
-        for key, value in list(data.items()):
-            try:
-                _s = str(value)
-            except Exception as _e:
-                print("Can't convert:")
-                print(section, key, repr(value))
-                err = True
-    if err:
-        assert False
-    else:
-        import traceback
-
-        print("-" * 30)
-        traceback.print_stack()
 
 
-def get_home_dir():
-    """
-    Return user home directory
-    """
+def get_home_dir() -> str:
+    """Return user home directory"""
     try:
-        path = osp.expanduser("~")
-    except:
+        # expanduser() returns a raw byte string which needs to be
+        # decoded with the codec that the OS is using to represent
+        # file paths.
+        path = os.fsdecode(osp.expanduser("~"))
+    except Exception:
         path = ""
-    for env_var in ("HOME", "USERPROFILE", "TMP"):
-        if osp.isdir(path):
-            break
-        path = os.environ.get(env_var, "")
-    if path:
+
+    if osp.isdir(path):
         return path
     else:
-        raise RuntimeError("Please define environment variable $HOME")
+        # Get home from alternative locations
+        for env_var in ("HOME", "USERPROFILE", "TMP"):
+            # os.environ.get() returns a raw byte string which needs to be
+            # decoded with the codec that the OS is using to represent
+            # environment variables.
+            path = os.fsdecode(os.environ.get(env_var, ""))
+            if osp.isdir(path):
+                return path
+            else:
+                path = ""
 
+        if not path:
+            raise RuntimeError(
+                "Please set the environment variable HOME to "
+                "your user/home directory path."
+            )
 
-def get_config_dir():
-    if sys.platform == "win32":
-        # TODO: on windows config files usually go in
-        return get_home_dir()
-    return osp.join(get_home_dir(), ".config")
+
+def get_config_basedir() -> str:
+    """Return user configuration base directory."""
+    if sys.platform.startswith("linux"):
+        # Follow the XDG standard to save settings
+        home = os.environ.get("XDG_CONFIG_HOME", "")
+        if not home:
+            home = osp.join(get_home_dir(), ".config")
+        if not osp.isdir(home):
+            os.makedirs(home)
+        return home
+    return get_home_dir()
 
 
 class NoDefault:
+    """
+    Custom object used to explicitly mark that no default value were
+    provided.
+    """
+
     pass
 
 
 class UserConfig(cp.ConfigParser):
     """
     UserConfig class, based on ConfigParser
     name: name of the config
     options: dictionnary containing options *or* list of tuples
     (section_name, options)
 
-    Note that 'get' and 'set' arguments number and type
+    Note that "get" and "set" arguments number and type
     differ from the overriden methods
     """
 
     default_section_name = "main"
 
     def __init__(self, defaults):
         cp.ConfigParser.__init__(self)
         self.name = "none"
-        self.raw = 0  # 0=substitutions are enabled / 1=raw config parser
+        self.raw = 0  # 0 = substitutions are enabled / 1 = raw config parser
         assert isinstance(defaults, dict)
         for _key, val in list(defaults.items()):
             assert isinstance(val, dict)
         if self.default_section_name not in defaults:
             defaults[self.default_section_name] = {}
         self.defaults = defaults
         self.reset_to_defaults(save=False)
         self.check_default_values()
 
     def update_defaults(self, defaults):
+        """Update the default configuration
+
+        :param defaults: dict section -> dict {option: default value}
+        """
         for key, sectdict in list(defaults.items()):
             if key not in self.defaults:
                 self.defaults[key] = sectdict
             else:
                 self.defaults[key].update(sectdict)
         self.reset_to_defaults(save=False)
 
     def save(self):
+        """Save the configuration."""
         # In any case, the resulting config is saved in config file:
         self.__save()
 
     def set_application(self, name, version, load=True, raw_mode=False):
+        """
+        Set the application name and version
+
+        :param name: name of the application
+        :param version: current version in format "X.Y.Z"
+        :param load: If True, load the configuration from dict
+        :param raw_mode: If True, enable raw mode of ConfigParser
+        """
         self.name = name
         self.raw = 1 if raw_mode else 0
-        if (version is not None) and (re.match("^(\d+).(\d+).(\d+)$", version) is None):
+        if (version is not None) and (re.match(r"^(\d+).(\d+).(\d+)", version) is None):
             raise RuntimeError(
-                "Version number %r is incorrect - must be in X.Y.Z format" % version
+                f"Version number {version!r} is incorrect - must be in X.Y.Z format"
             )
 
         if load:
             # If config file already exists, it overrides Default options:
             self.__load()
             if version != self.get_version(version):
                 # Version has changed -> overwriting .ini file
@@ -170,15 +182,15 @@
                     _check(key + "{}", k)
                     _check(key + "/" + k, v)
             elif isinstance(value, (list, tuple)):
                 for v in value:
                     _check(key + "[]", v)
             else:
                 if not isinstance(value, (bool, int, float, str)):
-                    errors.append("Invalid value for %s: %r" % (key, value))
+                    errors.append(f"Invalid value for {key}: {value}")
 
         for name, section in list(self.defaults.items()):
             assert isinstance(name, str)
             for key, value in list(section.items()):
                 _check(key, value)
         if errors:
             for err in errors:
@@ -216,22 +228,28 @@
     def __save(self):
         """
         Save config into the associated .ini file
         """
         fname = self.filename()
         if osp.isfile(fname):
             os.remove(fname)
+        os.makedirs(osp.dirname(fname), mode=0o700, exist_ok=True)
         with open(fname, "w", encoding="utf-8") as configfile:
             self.write(configfile)
 
-    def filename(self):
-        """
-        Create a .ini filename located in user home directory
-        """
-        return osp.join(get_config_dir(), ".%s.ini" % self.name)
+    def get_path(self, basename: str) -> str:
+        """Return filename path inside configuration directory"""
+        config_dir = osp.join(get_config_basedir(), f".{self.name}")
+        if not osp.isdir(config_dir):
+            os.makedirs(config_dir)
+        return osp.join(config_dir, basename)
+
+    def filename(self) -> str:
+        """Return configuration file name"""
+        return self.get_path(f"{self.name}.ini")
 
     def cleanup(self):
         """
         Remove .ini file associated to config
         """
         os.remove(self.filename())
 
@@ -289,21 +307,21 @@
         if raw is None:
             raw = self.raw
 
         section = self.__check_section_option(section, option)
 
         if not self.has_section(section):
             if default is NoDefault:
-                raise RuntimeError("Unknown section %r" % section)
+                raise RuntimeError(f"Unknown section {section!r}")
             else:
                 self.add_section(section)
 
         if not self.has_option(section, option):
             if default is NoDefault:
-                raise RuntimeError("Unknown option %r/%r" % (section, option))
+                raise RuntimeError(f"Unknown option {section!r}/{option!r}")
             else:
                 self.set(section, option, default)
                 return default
 
         value = cp.ConfigParser.get(self, section, option, raw=raw)
 
         default_value = self.get_default(section, option)
@@ -315,34 +333,42 @@
             value = int(value)
         elif isinstance(default_value, str):
             pass
         else:
             try:
                 # lists, tuples, ...
                 value = eval(value)
-            except:
+            except Exception:
                 pass
+
         return value
 
     def get_section(self, section):
+        """Returns configuration values of the given section.
+
+        The returned dict includes unset default values.
+
+        :param section: section name
+        :return: dict option name -> value
+        """
         sect = self.defaults.get(section, {}).copy()
         for opt in self.options(section):
             sect[opt] = self.get(section, opt)
         return sect
 
     def __set(self, section, option, value, verbose):
         """
         Private set method
         """
         if not self.has_section(section):
             self.add_section(section)
         if not isinstance(value, str):
             value = repr(value)
         if verbose:
-            print("%s[ %s ] = %s" % (section, option, value))
+            print("{}[ {} ] = {}".format(section, option, value))
         cp.ConfigParser.set(self, section, option, value)
 
     def set_default(self, section, option, default_value):
         """
         Set Default value for a given (section, option)
         -> called when a new (section, option) is set and no default exists
         """
@@ -369,13 +395,18 @@
         elif not isinstance(default_value, str):
             value = repr(value)
         self.__set(section, option, value, verbose)
         if save:
             self.__save()
 
     def remove_section(self, section):
+        """Remove the given section and save the configuration."""
         cp.ConfigParser.remove_section(self, section)
         self.__save()
 
     def remove_option(self, section, option):
+        """
+        Remove the given option from the given section
+        and save the configuration.
+        """
         cp.ConfigParser.remove_option(self, section, option)
         self.__save()
```

### Comparing `guidata-2.3.1/guidata/widgets/arrayeditor.py` & `guidata-3.0.0/guidata/widgets/arrayeditor.py`

 * *Files 0% similar despite different names*

```diff
@@ -946,15 +946,15 @@
         QDialog.reject(self)
 
 
 def launch_arrayeditor(data, title="", xlabels=None, ylabels=None):
     """Helper routine to launch an arrayeditor and return its result"""
     dlg = ArrayEditor()
     assert dlg.setup_and_check(data, title, xlabels=xlabels, ylabels=ylabels)
-    dlg.exec_()
+    dlg.exec()
     # dlg.accept()  # trigger slot connected to OK button
     return dlg.get_value()
 
 
 if __name__ == "__main__":
     from guidata import qapplication
```

### Comparing `guidata-2.3.1/guidata/widgets/codeeditor.py` & `guidata-3.0.0/guidata/widgets/codeeditor.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,23 +16,22 @@
 
 # %% This line is for cell execution testing
 # pylint: disable=C0103
 # pylint: disable=R0903
 # pylint: disable=R0911
 # pylint: disable=R0201
 
-from qtpy.QtWidgets import QWidget, QPlainTextEdit
-from qtpy.QtGui import QColor, QPainter
-from qtpy.QtCore import QRect, QSize, Qt
-
 import guidata.widgets.syntaxhighlighters as sh
+from guidata.config import CONF, _
 from guidata.configtools import get_font
-from guidata import encoding
 from guidata.qthelpers import is_dark_mode, win32_fix_title_bar_background
-from guidata.config import CONF, _
+from guidata.utils import encoding
+from qtpy.QtCore import QRect, QSize, Qt
+from qtpy.QtGui import QColor, QPainter
+from qtpy.QtWidgets import QPlainTextEdit, QWidget
 
 
 class LineNumberArea(QWidget):
     """Line number area (on the left side of the text editor widget)"""
 
     def __init__(self, editor):
         QWidget.__init__(self, editor)
@@ -65,15 +64,14 @@
 
     def wheelEvent(self, event):
         """Override Qt method"""
         self.code_editor.wheelEvent(event)
 
 
 class CodeEditor(QPlainTextEdit):
-
     # To have these attrs when early viewportEvent's are triggered
     linenumberarea = None
 
     LANGUAGES = {
         "python": sh.PythonSH,
         "cython": sh.CythonSH,
         "fortran77": sh.Fortran77SH,
@@ -357,8 +355,8 @@
     from guidata import qapplication
 
     app = qapplication()
 
     widget = CodeEditor(columns=80, rows=40)
     widget.set_text_from_file(__file__)
     widget.show()
-    app.exec_()
+    app.exec()
```

### Comparing `guidata-2.3.1/guidata/widgets/collectionseditor.py` & `guidata-3.0.0/guidata/widgets/collectionseditor.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,66 +30,35 @@
 import re
 import sys
 import warnings
 
 import PIL.Image
 from guidata.config import CONF, _
 from guidata.configtools import get_font, get_icon
-from guidata.qthelpers import (
-    add_actions,
-    create_action,
-    mimedata2url,
-    win32_fix_title_bar_background,
-)
-from guidata.utils import getcwd_or_home
+from guidata.qthelpers import (add_actions, create_action, mimedata2url,
+                               win32_fix_title_bar_background)
+from guidata.utils.misc import getcwd_or_home
 from guidata.widgets.importwizard import ImportWizard
-from guidata.widgets.nsview import (
-    DataFrame,
-    DatetimeIndex,
-    FakeObject,
-    Image,
-    MaskedArray,
-    Series,
-    array,
-    display_to_value,
-    get_color_name,
-    get_human_readable_type,
-    get_object_attrs,
-    get_size,
-    get_type_string,
-    is_editable_type,
-    is_known_type,
-    ndarray,
-    np_savetxt,
-    sort_against,
-    try_to_eval,
-    unsorted_unique,
-    value_to_display,
-)
+from guidata.widgets.nsview import (DataFrame, DatetimeIndex, FakeObject,
+                                    Image, MaskedArray, Series, array,
+                                    display_to_value, get_color_name,
+                                    get_human_readable_type, get_object_attrs,
+                                    get_size, get_type_string,
+                                    is_editable_type, is_known_type, ndarray,
+                                    np_savetxt, sort_against, try_to_eval,
+                                    unsorted_unique, value_to_display)
 from guidata.widgets.texteditor import TextEditor
 from qtpy.compat import getsavefilename
-from qtpy.QtCore import QAbstractTableModel, QDateTime, QModelIndex, Qt, Signal, Slot
+from qtpy.QtCore import (QAbstractTableModel, QDateTime, QModelIndex, Qt,
+                         Signal, Slot)
 from qtpy.QtGui import QColor, QKeySequence
-from qtpy.QtWidgets import (
-    QAbstractItemDelegate,
-    QApplication,
-    QDateEdit,
-    QDateTimeEdit,
-    QDialog,
-    QHBoxLayout,
-    QInputDialog,
-    QItemDelegate,
-    QLineEdit,
-    QMenu,
-    QMessageBox,
-    QPushButton,
-    QTableView,
-    QVBoxLayout,
-    QWidget,
-)
+from qtpy.QtWidgets import (QAbstractItemDelegate, QApplication, QDateEdit,
+                            QDateTimeEdit, QDialog, QHBoxLayout, QInputDialog,
+                            QItemDelegate, QLineEdit, QMenu, QMessageBox,
+                            QPushButton, QTableView, QVBoxLayout, QWidget)
 
 if ndarray is not FakeObject:
     from guidata.widgets.arrayeditor import ArrayEditor
 
 if DataFrame is not FakeObject:
     from guidata.widgets.dataframeeditor import DataFrameEditor
 
@@ -113,15 +82,15 @@
         index = 0
         while get_new_name(index) in blacklist:
             index += 1
         name = get_new_name(index)
     return name
 
 
-class ProxyObject(object):
+class ProxyObject:
     """Dictionary proxy to an unknown object."""
 
     def __init__(self, obj):
         """Constructor."""
         self.__obj__ = obj
 
     def __len__(self):
@@ -462,15 +431,14 @@
         self.dataChanged.emit(index, index)
         return True
 
 
 class CollectionsDelegate(QItemDelegate):
     """CollectionsEditor Item Delegate"""
 
-    sig_free_memory = Signal()
 
     def __init__(self, parent=None):
         QItemDelegate.__init__(self, parent)
         self._editors = {}  # keep references on opened editors
 
     def get_value(self, index):
         """
@@ -685,30 +653,25 @@
         data = self._editors[editor_id]
         if not data["readonly"]:
             index = data["model"].get_index_from_key(data["key"])
             value = data["editor"].get_value()
             conv_func = data.get("conv", lambda v: v)
             self.set_value(index, conv_func(value))
         self._editors.pop(editor_id)
-        self.free_memory()
+        editor = self.sender()
+        editor.deleteLater()
 
     def editor_rejected(self, editor_id):
         """
 
         :param editor_id:
         """
         self._editors.pop(editor_id)
-        self.free_memory()
-
-    def free_memory(self):
-        """Free memory after closing an editor."""
-        try:
-            self.sig_free_memory.emit()
-        except RuntimeError:
-            pass
+        editor = self.sender()
+        editor.deleteLater()
 
     def commitAndCloseEditor(self):
         """Overriding method commitAndCloseEditor"""
         editor = self.sender()
         # Avoid a segfault with PyQt5. Variable value won't be changed
         # but at least Spyder won't crash. It seems generated by a bug in sip.
         try:
@@ -787,15 +750,14 @@
 
 class BaseTableView(QTableView):
     """Base collection editor table view"""
 
     sig_option_changed = Signal(str, object)
     sig_files_dropped = Signal(list)
     redirect_stdio = Signal(bool)
-    sig_free_memory = Signal()
 
     def __init__(self, parent):
         QTableView.__init__(self, parent)
         self.array_filename = None
         self.menu = None
         self.empty_ws_menu = None
         self.paste_action = None
@@ -1338,15 +1300,15 @@
         editor = ImportWizard(
             self,
             text,
             title=title,
             contents_title=_("Clipboard contents"),
             varname=fix_reference_name("data", blacklist=list(data.keys())),
         )
-        if editor.exec_():
+        if editor.exec():
             var_name, clip_data = editor.get_data()
             self.new_value(var_name, clip_data)
 
     @Slot()
     def paste(self):
         """Import text/data/code from clipboard"""
         clipboard = QApplication.clipboard()
```

### Comparing `guidata-2.3.1/guidata/widgets/console/__init__.py` & `guidata-3.0.0/guidata/widgets/console/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,20 @@
 
 .. autoclass:: Console
 
 .. autoclass:: DockableConsole
 
 """
 
-from qtpy.QtCore import Qt
-
-from guidata.widgets.console.internalshell import InternalShell
-from guidata.qtwidgets import DockableWidgetMixin
-from guidata.qthelpers import win32_fix_title_bar_background
-from guidata.configtools import get_font
 from guidata.config import CONF, _
+from guidata.configtools import get_font
+from guidata.qthelpers import win32_fix_title_bar_background
+from guidata.widgets.console.internalshell import InternalShell
+from guidata.widgets.dockable import DockableWidgetMixin
+from qtpy.QtCore import Qt
 
 
 class Console(InternalShell):
     """
     Python console that run an interactive shell linked to
     the running process.
```

### Comparing `guidata-2.3.1/guidata/widgets/console/base.py` & `guidata-3.0.0/guidata/widgets/console/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,49 +13,42 @@
 
 
 import os
 import re
 import sys
 from collections import OrderedDict
 
-from qtpy.QtWidgets import (
-    QApplication,
-    QListWidget,
-    QListWidgetItem,
-    QMainWindow,
-    QPlainTextEdit,
-    QTextEdit,
-    QToolTip,
-    QAbstractItemView,
-)
+from qtpy.QtCore import QEvent, QEventLoop, QPoint, Qt, Signal, Slot
 from qtpy.QtGui import (
-    QPalette,
+    QClipboard,
     QColor,
     QFont,
+    QMouseEvent,
+    QPalette,
     QTextCharFormat,
     QTextCursor,
     QTextFormat,
     QTextOption,
-    QClipboard,
-    QMouseEvent,
 )
-from qtpy.QtCore import (
-    QEvent,
-    QEventLoop,
-    QPoint,
-    Signal,
-    Slot,
-    Qt,
+from qtpy.QtWidgets import (
+    QAbstractItemView,
+    QApplication,
+    QListWidget,
+    QListWidgetItem,
+    QMainWindow,
+    QPlainTextEdit,
+    QTextEdit,
+    QToolTip,
 )
 
+from guidata.config import CONF
+from guidata.configtools import get_font, get_icon
 from guidata.widgets.console.calltip import CallTipWidget
 from guidata.widgets.console.mixins import BaseEditMixin
 from guidata.widgets.console.terminal import ANSIEscapeCodeHandler
-from guidata.configtools import get_font, get_icon
-from guidata.config import CONF
 
 
 def insert_text_to(cursor, text, fmt):
     """Helper to print text, taking into account backspaces"""
     while True:
         index = text.find(chr(8))  # backspace
         if index == -1:
@@ -198,24 +191,20 @@
         shift = event.modifiers() & Qt.ShiftModifier
         ctrl = event.modifiers() & Qt.ControlModifier
         modifier = shift or ctrl or alt
         if (
             key in (Qt.Key_Return, Qt.Key_Enter) and self.enter_select
         ) or key == Qt.Key_Tab:
             self.item_selected()
-        elif (
-            key
-            in (
-                Qt.Key_Return,
-                Qt.Key_Enter,
-                Qt.Key_Left,
-                Qt.Key_Right,
-            )
-            or text in (".", ":")
-        ):
+        elif key in (
+            Qt.Key_Return,
+            Qt.Key_Enter,
+            Qt.Key_Left,
+            Qt.Key_Right,
+        ) or text in (".", ":"):
             self.hide()
             self.textedit.keyPressEvent(event)
         elif (
             key
             in (
                 Qt.Key_Up,
                 Qt.Key_Down,
@@ -652,30 +641,30 @@
             text = self.get_text("sof", "eof")
             return (
                 text.replace("\u2028", "\n")
                 .replace("\u2029", "\n")
                 .replace("\u0085", "\n")
             )
         else:
-            return super(TextEditBaseWidget, self).toPlainText()
+            return super().toPlainText()
 
     def keyPressEvent(self, event):
         """
 
         :param event:
         """
         text, key = event.text(), event.key()
         ctrl = event.modifiers() & Qt.ControlModifier
         meta = event.modifiers() & Qt.MetaModifier
         # Use our own copy method for {Ctrl,Cmd}+C to avoid Qt
         # copying text in HTML (See Issue 2285)
         if (ctrl or meta) and key == Qt.Key_C:
             self.copy()
         else:
-            super(TextEditBaseWidget, self).keyPressEvent(event)
+            super().keyPressEvent(event)
 
     # ------Text: get, set, ...
     def get_selection_as_executable_code(self):
         """Return selected text as a processed text,
         to be executable in a Python/IPython interpreter"""
         ls = self.get_line_separator()
```

### Comparing `guidata-2.3.1/guidata/widgets/console/calltip.py` & `guidata-3.0.0/guidata/widgets/console/calltip.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,49 +15,41 @@
 Now located at qtconsole/call_tip_widget.py as part of the
 `Jupyter QtConsole Project <https://github.com/jupyter/qtconsole>`_.
 """
 
 
 from unicodedata import category
 
+from qtpy.QtCore import QBasicTimer, QCoreApplication, QEvent, Qt
+from qtpy.QtGui import QCursor, QPalette
 from qtpy.QtWidgets import (
     QFrame,
     QLabel,
     QPlainTextEdit,
     QStyle,
     QStyleOptionFrame,
     QStylePainter,
     QTextEdit,
     QToolTip,
 )
-from qtpy.QtGui import (
-    QCursor,
-    QPalette,
-)
-from qtpy.QtCore import (
-    QBasicTimer,
-    QEvent,
-    QCoreApplication,
-    Qt,
-)
 
 
 class CallTipWidget(QLabel):
     """Shows call tips by parsing the current text of Q[Plain]TextEdit."""
 
     # --------------------------------------------------------------------------
     # 'QObject' interface
     # --------------------------------------------------------------------------
 
     def __init__(self, text_edit, hide_timer_on=False):
         """Create a call tip manager that is attached to the specified Qt
         text edit widget.
         """
         assert isinstance(text_edit, (QTextEdit, QPlainTextEdit))
-        super(CallTipWidget, self).__init__(None, Qt.ToolTip)
+        super().__init__(None, Qt.ToolTip)
         self.app = QCoreApplication.instance()
 
         self.hide_timer_on = hide_timer_on
         self.tip = None
         self._hide_timer = QBasicTimer()
         self._text_edit = text_edit
 
@@ -101,68 +93,68 @@
                     and self.app.topLevelAt(QCursor.pos()) == self
                 ):
                     self._hide_timer.stop()
 
             elif etype == QEvent.Leave:
                 self._leave_event_hide()
 
-        return super(CallTipWidget, self).eventFilter(obj, event)
+        return super().eventFilter(obj, event)
 
     def timerEvent(self, event):
         """Reimplemented to hide the widget when the hide timer fires."""
         if event.timerId() == self._hide_timer.timerId():
             self._hide_timer.stop()
             self.hide()
 
     # --------------------------------------------------------------------------
     # 'QWidget' interface
     # --------------------------------------------------------------------------
 
     def enterEvent(self, event):
         """Reimplemented to cancel the hide timer."""
-        super(CallTipWidget, self).enterEvent(event)
+        super().enterEvent(event)
         if self._hide_timer.isActive() and self.app.topLevelAt(QCursor.pos()) == self:
             self._hide_timer.stop()
 
     def hideEvent(self, event):
         """Reimplemented to disconnect signal handlers and event filter."""
-        super(CallTipWidget, self).hideEvent(event)
+        super().hideEvent(event)
         self._text_edit.cursorPositionChanged.disconnect(self._cursor_position_changed)
         self._text_edit.removeEventFilter(self)
 
     def leaveEvent(self, event):
         """Reimplemented to start the hide timer."""
-        super(CallTipWidget, self).leaveEvent(event)
+        super().leaveEvent(event)
         self._leave_event_hide()
 
     def mousePressEvent(self, event):
         """
 
         :param event:
         """
-        super(CallTipWidget, self).mousePressEvent(event)
+        super().mousePressEvent(event)
         self.hide()
 
     def paintEvent(self, event):
         """Reimplemented to paint the background panel."""
         painter = QStylePainter(self)
         option = QStyleOptionFrame()
         option.initFrom(self)
         painter.drawPrimitive(QStyle.PE_PanelTipLabel, option)
         painter.end()
 
-        super(CallTipWidget, self).paintEvent(event)
+        super().paintEvent(event)
 
     def setFont(self, font):
         """Reimplemented to allow use of this method as a slot."""
-        super(CallTipWidget, self).setFont(font)
+        super().setFont(font)
 
     def showEvent(self, event):
         """Reimplemented to connect signal handlers and event filter."""
-        super(CallTipWidget, self).showEvent(event)
+        super().showEvent(event)
         self._text_edit.cursorPositionChanged.connect(self._cursor_position_changed)
         self._text_edit.installEventFilter(self)
 
     def focusOutEvent(self, event):
         """Reimplemented to hide it when focus goes out of the main
         window.
         """
```

### Comparing `guidata-2.3.1/guidata/widgets/console/dochelpers.py` & `guidata-3.0.0/guidata/widgets/console/dochelpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     # Most of the time doc will only contain ascii characters, but there are
     # some docstrings that contain non-ascii characters. Not all source files
     # declare their encoding in the first line, so querying for that might not
     # yield anything, either. So assume the most commonly used
     # multi-byte file encoding (which also covers ascii).
     try:
         docstring = str(docstring)
-    except:
+    except:  # pylint: disable=bare-except
         pass
 
     # Doc dict keys
     doc = {"name": "", "argspec": "", "note": "", "docstring": docstring}
 
     if callable(obj):
         try:
@@ -99,33 +99,16 @@
             obj = obj.__func__
         elif hasattr(obj, "__module__"):
             doc["note"] = "Function of %s module" % obj.__module__
         else:
             doc["note"] = "Function"
         doc["name"] = obj.__name__
         if inspect.isfunction(obj):
-            (
-                args,
-                varargs,
-                varkw,
-                defaults,
-                kwonlyargs,
-                kwonlydefaults,
-                annotations,
-            ) = inspect.getfullargspec(obj)
-            doc["argspec"] = inspect.formatargspec(
-                args,
-                varargs,
-                varkw,
-                defaults,
-                kwonlyargs,
-                kwonlydefaults,
-                annotations,
-                formatvalue=lambda o: "=" + repr(o),
-            )
+            sig = inspect.signature(obj)
+            doc["argspec"] = str(sig)
             if name == "<lambda>":
                 doc["name"] = name + " lambda "
                 doc["argspec"] = doc["argspec"][1:-1]  # remove parentheses
         else:
             argspec = getargspecfromtext(doc["docstring"])
             if argspec:
                 doc["argspec"] = argspec
@@ -200,15 +183,15 @@
 getsignaturesfromtext = getsignaturefromtext
 
 
 def getargspecfromtext(text):
     """
     Try to get the formatted argspec of a callable from the first block of its
     docstring
-    
+
     This will return something like
     '(foo, bar, k=1)'
     """
     blocks = text.split("\n\n")
     first_block = blocks[0].strip()
     return getsignaturefromtext(first_block, "")
```

### Comparing `guidata-2.3.1/guidata/widgets/console/internalshell.py` & `guidata-3.0.0/guidata/widgets/console/internalshell.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,29 +17,30 @@
 import builtins
 import os
 import platform
 import sys
 import threading
 from time import time
 
+from qtpy.QtCore import QEventLoop, QObject, Signal, Slot
+from qtpy.QtWidgets import QMessageBox
+
 from guidata.config import CONF, _
 from guidata.qthelpers import create_action, get_std_icon, is_dark_mode
-from guidata.utils import getcwd_or_home, run_program
+from guidata.utils.misc import getcwd_or_home, run_program
 from guidata.widgets.console.dochelpers import getargtxt, getdoc, getobjdir, getsource
 from guidata.widgets.console.interpreter import Interpreter
 from guidata.widgets.console.shell import PythonShellWidget
-from qtpy.QtCore import QEventLoop, QObject, Signal, Slot
-from qtpy.QtWidgets import QMessageBox
 
 
 def create_banner(message):
     """Create internal shell banner"""
     system = platform.system()
     if message is None:
-        bitness = 64 if sys.maxsize > 2 ** 32 else 32
+        bitness = 64 if sys.maxsize > 2**32 else 32
         return "Python %s %dbits [%s]" % (platform.python_version(), bitness, system)
     else:
         return message
 
 
 class SysOutput(QObject):
     """Handle standard I/O queue"""
@@ -276,15 +277,15 @@
     # ------Raw input support
     def wait_input(self, prompt=""):
         """Wait for input (raw_input support)"""
         self.new_prompt(prompt)
         self.setFocus()
         self.input_mode = True
         self.input_loop = QEventLoop()
-        self.input_loop.exec_()
+        self.input_loop.exec()
         self.input_loop = None
 
     def end_input(self, cmd):
         """End of wait_input mode"""
         self.input_mode = False
         self.input_loop.exit()
         self.interpreter.widget_proxy.end_input(cmd)
@@ -319,15 +320,14 @@
                 _("Shell special commands:"),
                 _("Internal editor:"),
                 _("External editor:"),
                 _("Run script:"),
                 _("Remove references:"),
                 _("System commands:"),
                 _("Python help:"),
-                _("GUI-based editor:"),
             ),
         )
 
     def external_editor(self, filename, goto=-1):
         """Edit in an external editor
         Recommended: SciTE (e.g. to go to line where an error did occur)"""
         editor_path = CONF.get("console", "external_editor/path")
@@ -360,15 +360,15 @@
     def on_enter(self, command):
         """on_enter"""
         if self.profile:
             # Simple profiling test
             t0 = time()
             for _ in range(10):
                 self.execute_command(command)
-            self.insert_text(u"\n<Δt>=%dms\n" % (1e2 * (time() - t0)))
+            self.insert_text("\n<Δt>=%dms\n" % (1e2 * (time() - t0)))
             self.new_prompt(self.interpreter.p1)
         else:
             self.execute_command(command)
         self.__flush_eventqueue()
 
     def keyPressEvent(self, event):
         """
```

### Comparing `guidata-2.3.1/guidata/widgets/console/mixins.py` & `guidata-3.0.0/guidata/widgets/console/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,36 +11,28 @@
 IPython console plugin.
 """
 
 
 import os
 import os.path as osp
 import re
-import sre_constants
 import textwrap
 from xml.sax.saxutils import escape
 
-from qtpy.QtWidgets import (
-    QApplication,
-    QToolTip,
-)
-from qtpy.QtGui import (
-    QCursor,
-    QTextCursor,
-    QTextDocument,
-)
-from qtpy.QtCore import Qt, QPoint, QRegularExpression
+from qtpy.QtCore import QPoint, QRegularExpression, Qt
+from qtpy.QtGui import QCursor, QTextCursor, QTextDocument
+from qtpy.QtWidgets import QApplication, QToolTip
 
+from guidata.config import _
+from guidata.utils import encoding
 from guidata.widgets.console.dochelpers import (
     getargspecfromtext,
     getobj,
     getsignaturefromtext,
 )
-from guidata import encoding
-from guidata.config import _
 
 # Order is important:
 EOL_CHARS = (("\r\n", "nt"), ("\n", "posix"), ("\r", "mac"))
 
 
 def get_eol_chars(text):
     """Get text EOL characters"""
@@ -318,15 +310,15 @@
         """
         cursor = self.__select_text(position_from, position_to)
         text = str(cursor.selectedText())
         all_text = position_from == "sof" and position_to == "eof"
         if text and not all_text:
             while text.endswith("\n"):
                 text = text[:-1]
-            while text.endswith(u"\u2029"):
+            while text.endswith("\u2029"):
                 text = text[:-1]
         return text
 
     def get_character(self, position, offset=0):
         """Return character at *position* with the given offset."""
         position = self.get_position(position) + offset
         cursor = self.textCursor()
@@ -417,15 +409,15 @@
         cursor = self.cursorForPosition(coordinates)
         return cursor.blockNumber() - 1
 
     def get_line_at(self, coordinates):
         """Return line at *coordinates* (QPoint)"""
         cursor = self.cursorForPosition(coordinates)
         cursor.select(QTextCursor.BlockUnderCursor)
-        return str(cursor.selectedText()).replace(u"\u2029", "")
+        return str(cursor.selectedText()).replace("\u2029", "")
 
     def get_word_at(self, coordinates):
         """Return word at *coordinates* (QPoint)"""
         cursor = self.cursorForPosition(coordinates)
         cursor.select(QTextCursor.WordUnderCursor)
         return str(cursor.selectedText())
 
@@ -452,15 +444,15 @@
         """
         Return text selected by current text cursor, converted in unicode
 
         Replace the unicode line separator character ``\u2029`` by
         the line separator characters returned by :py:meth:`get_line_separator`
         """
         return str(self.textCursor().selectedText()).replace(
-            u"\u2029", self.get_line_separator()
+            "\u2029", self.get_line_separator()
         )
 
     def remove_selected_text(self):
         """Delete selected text"""
         self.textCursor().removeSelectedText()
 
     def replace(self, text, pattern=None):
@@ -482,15 +474,15 @@
         """Reimplement QTextDocument's find method
 
         Add support for *multiline* regular expressions"""
         pattern = str(regexp.pattern())
         text = str(self.toPlainText())
         try:
             regobj = re.compile(pattern)
-        except sre_constants.error:
+        except re.error:
             return
         if findflag & QTextDocument.FindBackward:
             # Find backward
             offset = min([cursor.selectionEnd(), cursor.selectionStart()])
             text = text[:offset]
             matches = [_m for _m in regobj.finditer(text, 0, offset)]
             if matches:
@@ -534,15 +526,15 @@
             moves += [QTextCursor.End]
 
         if regexp:
             text = str(text)
         else:
             text = re.escape(str(text))
 
-        pattern = QRegularExpression(u"\\b{}\\b".format(text) if words else text)
+        pattern = QRegularExpression("\\b{}\\b".format(text) if words else text)
         if case:
             pattern.setPatternOptions(QRegularExpression.CaseInsensitiveOption)
 
         for move in moves:
             cursor.movePosition(move)
             if regexp and "\\n" in text:
                 # Multiline regular expression
@@ -574,15 +566,15 @@
             source_text = str(self.toPlainText())
 
         try:
             if case:
                 regobj = re.compile(pattern)
             else:
                 regobj = re.compile(pattern, re.IGNORECASE)
-        except sre_constants.error:
+        except re.error:
             return None
 
         number_matches = 0
         for match in regobj.finditer(source_text):
             number_matches += 1
 
         return number_matches
```

### Comparing `guidata-2.3.1/guidata/widgets/console/shell.py` & `guidata-3.0.0/guidata/widgets/console/shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,50 +17,30 @@
 import locale
 import os
 import os.path as osp
 import re
 import sys
 import time
 
-from qtpy.QtWidgets import (
-    QApplication,
-    QToolTip,
-    QMenu,
-)
-from qtpy.QtGui import (
-    QTextCursor,
-    QTextCharFormat,
-    QTextCursor,
-    QKeyEvent,
-)
-from qtpy.QtCore import (
-    QCoreApplication,
-    Qt,
-    QTimer,
-    Signal,
-    Slot,
-    Property,
-)
 from qtpy.compat import getsavefilename
+from qtpy.QtCore import Property, QCoreApplication, Qt, QTimer, Signal, Slot
+from qtpy.QtGui import QKeyEvent, QTextCharFormat, QTextCursor
+from qtpy.QtWidgets import QApplication, QMenu, QToolTip
 
+from guidata.config import CONF, _
+from guidata.configtools import get_icon
+from guidata.qthelpers import add_actions, create_action, keybinding
+from guidata.utils import encoding
+from guidata.widgets.console.base import ConsoleBaseWidget
 from guidata.widgets.console.mixins import (
     BrowseHistoryMixin,
     GetHelpMixin,
     SaveHistoryMixin,
     TracebackLinksMixin,
 )
-from guidata.widgets.console.base import ConsoleBaseWidget
-from guidata.configtools import get_icon
-from guidata import encoding
-from guidata.qthelpers import (
-    add_actions,
-    create_action,
-    keybinding,
-)
-from guidata.config import CONF, _
 
 DEBUG = False
 STDERR = sys.stderr
 
 
 def tuple2keyevent(past_event):
     """Convert tuple into a QKeyEvent instance"""
@@ -91,22 +71,26 @@
     """
 
     redirect_stdio = Signal(bool)
     sig_keyboard_interrupt = Signal()
     execute = Signal(str)
     append_to_history = Signal(str, str)
 
-    def __init__(self, parent, profile=False, initial_message=None):
+    def __init__(self, parent, profile=False, initial_message=None, read_only=False):
         """
         parent : specifies the parent widget
         """
         ConsoleBaseWidget.__init__(self, parent)
         SaveHistoryMixin.__init__(self)
         BrowseHistoryMixin.__init__(self)
 
+        # Read-only console is not the more used case, but it may be useful in
+        # some cases (e.g. when using the console as a log window)
+        self.setReadOnly(read_only)
+
         self.historylog_filename = "history.log"
 
         # Prompt position: tuple (line, index)
         self.current_prompt_pos = None
         self.new_input_line = True
 
         # Context menu
@@ -708,47 +692,47 @@
     INITHISTORY = [
         "# -*- coding: utf-8 -*-",
         "# *** Spyder Python Console History Log ***",
     ]
     SEPARATOR = "%s##---(%s)---" % (os.linesep * 2, time.ctime())
     go_to_error = Signal(str)
 
-    def __init__(self, parent, profile=False, initial_message=None):
-        ShellBaseWidget.__init__(self, parent, profile, initial_message)
+    def __init__(self, parent, profile=False, initial_message=None, read_only=False):
+        ShellBaseWidget.__init__(self, parent, profile, initial_message, read_only)
         TracebackLinksMixin.__init__(self)
         GetHelpMixin.__init__(self)
 
     # ------ Context menu
     def setup_context_menu(self):
         """Reimplements ShellBaseWidget method"""
         ShellBaseWidget.setup_context_menu(self)
         self.copy_without_prompts_action = create_action(
             self,
             _("Copy without prompts"),
             icon=get_icon("copywop.png"),
             triggered=self.copy_without_prompts,
         )
-        clear_line_action = create_action(
-            self,
-            _("Clear line"),
-            icon=get_icon("editdelete.png"),
-            tip=_("Clear line"),
-            triggered=self.clear_line,
-        )
-        clear_action = create_action(
-            self,
-            _("Clear shell"),
-            icon=get_icon("editclear.png"),
-            tip=_("Clear shell contents " "('cls' command)"),
-            triggered=self.clear_terminal,
-        )
-        add_actions(
-            self.menu,
-            (self.copy_without_prompts_action, clear_line_action, clear_action),
-        )
+        actions = [self.copy_without_prompts_action]
+        if not self.isReadOnly():
+            clear_line_action = create_action(
+                self,
+                _("Clear line"),
+                icon=get_icon("editdelete.png"),
+                tip=_("Clear line"),
+                triggered=self.clear_line,
+            )
+            clear_action = create_action(
+                self,
+                _("Clear shell"),
+                icon=get_icon("editclear.png"),
+                tip=_("Clear shell contents " "('cls' command)"),
+                triggered=self.clear_terminal,
+            )
+            actions += [clear_line_action, clear_action]
+        add_actions(self.menu, actions)
 
     def contextMenuEvent(self, event):
         """Reimplements ShellBaseWidget method"""
         state = self.has_selected_text()
         self.copy_without_prompts_action.setEnabled(state)
         ShellBaseWidget.contextMenuEvent(self, event)
```

### Comparing `guidata-2.3.1/guidata/widgets/console/terminal.py` & `guidata-3.0.0/guidata/widgets/console/terminal.py`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/widgets/dataframeeditor.py` & `guidata-3.0.0/guidata/widgets/dataframeeditor.py`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/widgets/importwizard.py` & `guidata-3.0.0/guidata/widgets/importwizard.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,16 @@
 # ----date and datetime objects support
 import datetime
 import io
 from functools import partial as ft_partial
 from itertools import zip_longest
 
 from numpy import nan
-
-from guidata.configtools import get_icon
-from guidata.qthelpers import add_actions, create_action, win32_fix_title_bar_background
-from guidata.config import _
+from qtpy.QtCore import QAbstractTableModel, QModelIndex, Qt, Signal, Slot
+from qtpy.QtGui import QColor, QIntValidator
 from qtpy.QtWidgets import (
     QCheckBox,
     QDialog,
     QFrame,
     QGridLayout,
     QGroupBox,
     QHBoxLayout,
@@ -37,25 +35,18 @@
     QSpacerItem,
     QTableView,
     QTabWidget,
     QTextEdit,
     QVBoxLayout,
     QWidget,
 )
-from qtpy.QtGui import (
-    QColor,
-    QIntValidator,
-)
-from qtpy.QtCore import (
-    QAbstractTableModel,
-    QModelIndex,
-    Qt,
-    Signal,
-    Slot,
-)
+
+from guidata.config import _
+from guidata.configtools import get_icon
+from guidata.qthelpers import add_actions, create_action, win32_fix_title_bar_background
 
 try:
     import pandas as pd
 except:
     pd = None
 
 
@@ -84,22 +75,22 @@
     try:
         return eval(value)
     except (NameError, SyntaxError, ImportError):
         return value
 
 
 # ----Numpy arrays support
-class FakeObject(object):
+class FakeObject:
     """Fake class used in replacement of missing modules"""
 
     pass
 
 
 try:
-    from numpy import ndarray, array
+    from numpy import array, ndarray
 except:
 
     class ndarray(FakeObject):  # analysis:ignore
         """Fake ndarray"""
 
         pass
 
@@ -277,23 +268,23 @@
     def get_as_num(self):
         """Return if numeric type conversion"""
         return self._as_num
 
     def get_col_sep(self):
         """Return the column separator"""
         if self.tab_btn.isChecked():
-            return u"\t"
+            return "\t"
         elif self.ws_btn.isChecked():
             return None
         return str(self.line_edt.text())
 
     def get_row_sep(self):
         """Return the row separator"""
         if self.eol_btn.isChecked():
-            return u"\n"
+            return "\n"
         return str(self.line_edt_row.text())
 
     def get_skiprows(self):
         """Return number of lines to be skipped"""
         return int(str(self.skiprows_edt.text()))
 
     def get_comments(self):
@@ -437,16 +428,16 @@
         add_actions(
             self.opt_menu, (self.str_action, self.int_action, self.float_action)
         )
 
     def _shape_text(
         self,
         text,
-        colsep=u"\t",
-        rowsep=u"\n",
+        colsep="\t",
+        rowsep="\n",
         transpose=False,
         skiprows=0,
         comments="#",
     ):
         """Decode the shape of the given text"""
         assert colsep != rowsep
         out = []
@@ -473,16 +464,16 @@
         if self._model is None:
             return None
         return self._model.get_data()
 
     def process_data(
         self,
         text,
-        colsep=u"\t",
-        rowsep=u"\n",
+        colsep="\t",
+        rowsep="\n",
         transpose=False,
         skiprows=0,
         comments="#",
     ):
         """Put data into table model"""
         data = self._shape_text(text, colsep, rowsep, transpose, skiprows, comments)
         self._model = PreviewTableModel(data)
@@ -539,16 +530,16 @@
         vert_layout.addWidget(type_frame)
         vert_layout.addWidget(self._table_view)
         self.setLayout(vert_layout)
 
     def open_data(
         self,
         text,
-        colsep=u"\t",
-        rowsep=u"\n",
+        colsep="\t",
+        rowsep="\n",
         transpose=False,
         skiprows=0,
         comments="#",
     ):
         """Open clipboard text as table"""
         if pd:
             self.pd_text = text
```

### Comparing `guidata-2.3.1/guidata/widgets/nsview.py` & `guidata-3.0.0/guidata/widgets/nsview.py`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/widgets/objecteditor.py` & `guidata-3.0.0/guidata/widgets/objecteditor.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,29 +10,37 @@
 
 This package provides a generic object editor widget.
 
 .. autofunction:: oedit
 
 """
 
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
 
 import PIL.Image
+from guidata.qthelpers import exec_dialog
 from guidata.widgets.arrayeditor import ArrayEditor
 from guidata.widgets.collectionseditor import CollectionsEditor
 from guidata.widgets.nsview import DataFrame, FakeObject, Series, is_known_type
 from guidata.widgets.texteditor import TextEditor
 from numpy.core.multiarray import ndarray
-from qtpy.QtCore import QObject
 
 try:
     from guidata.widgets.dataframeeditor import DataFrameEditor
 except ImportError:
     DataFrameEditor = FakeObject()
 
 
+if TYPE_CHECKING:
+    import numpy as np
+    from qtpy import QtWidgets as QW
+
+
 def create_dialog(obj, title, parent=None):
     """Creates the editor dialog and returns a tuple (dialog, func) where func
     is the function to be called with the dialog instance as argument, after
     quitting the dialog box
 
     The role of this intermediate function is to allow easy monkey-patching.
     (uschmitt suggested this indirection here so that he can monkey patch
@@ -70,24 +78,31 @@
         :return:
         """
         return conv_func(dialog.get_value())
 
     return dialog, end_func
 
 
-def oedit(obj, title=None, parent=None):
+def oedit(
+    obj: dict | list | tuple | str | np.ndarray,
+    title: str = None,
+    parent: QW.QWidget = None,
+) -> dict | list | tuple | str | np.ndarray:
     """Edit the object 'obj' in a GUI-based editor and return the edited copy
     (if Cancel is pressed, return None)
 
-    The object 'obj' is a container
+    Args:
+        obj (dict | list | tuple | str | np.ndarray): object to edit
+        title (str, optional): dialog title
+        parent (QW.QWidget, optional): parent widget
 
-    Supported container types:
-    dict, list, tuple, str/unicode or numpy.array
+    Returns:
+        dict | list | tuple | str | np.ndarray: edited object
     """
     title = "" if title is None else title
     result = create_dialog(obj, title, parent)
     if result is None:
         return
     dialog, end_func = result
-    if dialog.exec_():
+    if exec_dialog(dialog):
         return end_func(dialog)
     return None
```

### Comparing `guidata-2.3.1/guidata/widgets/syntaxhighlighters.py` & `guidata-3.0.0/guidata/widgets/syntaxhighlighters.py`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata/widgets/texteditor.py` & `guidata-3.0.0/guidata/widgets/texteditor.py`

 * *Files identical despite different names*

### Comparing `guidata-2.3.1/guidata.egg-info/SOURCES.txt` & `guidata-3.0.0/guidata.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,62 @@
 CHANGELOG.md
-Licence_CeCILL_V2-en.txt
+LICENSE
 MANIFEST.in
 README.md
-setup.py
+pyproject.toml
+setup.cfg
 doc/basic_example.py
 doc/conf.py
-doc/development.rst
 doc/examples.rst
 doc/index.rst
 doc/installation.rst
 doc/overview.rst
 doc/_static/favicon.ico
+doc/dev/contribute.rst
+doc/dev/howto.rst
+doc/dev/index.rst
+doc/dev/v2_to_v3.rst
 doc/images/basic_example.png
-doc/images/guidata.png
+doc/images/guidata-banner.png
+doc/images/guidata-vertical.png
+doc/images/layout_example.png
 doc/images/screenshots/__init__.png
 doc/images/screenshots/activable_dataset.png
 doc/images/screenshots/all_features.png
 doc/images/screenshots/all_items.png
 doc/images/screenshots/bool_selector.png
 doc/images/screenshots/datasetgroup.png
 doc/images/screenshots/editgroupbox.png
-doc/reference/configtools.rst
-doc/reference/dataset.rst
-doc/reference/disthelpers.rst
+doc/reference/guitest.rst
 doc/reference/index.rst
-doc/reference/qthelpers.rst
-doc/reference/userconfig.rst
 doc/reference/utils.rst
+doc/reference/widgets.rst
+doc/reference/dataset/dataitems.rst
+doc/reference/dataset/datatypes.rst
+doc/reference/dataset/index.rst
+doc/reference/dataset/qtwidgets.rst
 guidata/__init__.py
 guidata/config.py
 guidata/configtools.py
-guidata/disthelpers.py
-guidata/encoding.py
-guidata/gettext_helpers.py
+guidata/env.py
+guidata/guidata.chm
 guidata/guitest.py
-guidata/hdf5io.py
-guidata/jsonio.py
 guidata/qthelpers.py
-guidata/qtwidgets.py
 guidata/userconfig.py
-guidata/userconfigio.py
-guidata/utils.py
 guidata.egg-info/PKG-INFO
 guidata.egg-info/SOURCES.txt
 guidata.egg-info/dependency_links.txt
-guidata.egg-info/entry_points.txt
 guidata.egg-info/requires.txt
 guidata.egg-info/top_level.txt
 guidata/dataset/__init__.py
 guidata/dataset/dataitems.py
 guidata/dataset/datatypes.py
+guidata/dataset/hdf5io.py
+guidata/dataset/iniio.py
+guidata/dataset/jsonio.py
 guidata/dataset/qtitemwidgets.py
 guidata/dataset/qtwidgets.py
 guidata/dataset/textedit.py
 guidata/external/__init__.py
 guidata/external/darkdetect/__init__.py
 guidata/external/darkdetect/_dummy.py
 guidata/external/darkdetect/_linux_detect.py
@@ -74,14 +77,16 @@
 guidata/images/file.png
 guidata/images/fileclose.png
 guidata/images/fileimport.png
 guidata/images/filenew.png
 guidata/images/fileopen.png
 guidata/images/filesave.png
 guidata/images/filesaveas.png
+guidata/images/guidata-banner.svg
+guidata/images/guidata-vertical.svg
 guidata/images/guidata.svg
 guidata/images/max.png
 guidata/images/min.png
 guidata/images/none.png
 guidata/images/not_found.png
 guidata/images/python.png
 guidata/images/quickview.png
@@ -116,51 +121,62 @@
 guidata/images/filetypes/ps.png
 guidata/images/filetypes/tar.png
 guidata/images/filetypes/tgz.png
 guidata/images/filetypes/tif.png
 guidata/images/filetypes/txt.png
 guidata/images/filetypes/xls.png
 guidata/images/filetypes/zip.png
+guidata/locale/guidata.pot
 guidata/locale/fr/LC_MESSAGES/guidata.mo
 guidata/locale/fr/LC_MESSAGES/guidata.po
 guidata/tests/__init__.py
-guidata/tests/activable_dataset.py
-guidata/tests/activable_items.py
-guidata/tests/all_features.py
-guidata/tests/all_items.py
-guidata/tests/bool_selector.py
-guidata/tests/callbacks.py
-guidata/tests/config.py
-guidata/tests/data.py
-guidata/tests/datasetgroup.py
-guidata/tests/disthelpers.py
-guidata/tests/editgroupbox.py
-guidata/tests/inheritance.py
-guidata/tests/item_order.py
-guidata/tests/loadsave_hdf5.py
-guidata/tests/loadsave_json.py
-guidata/tests/rotatedlabel.py
+guidata/tests/_all_tests.py
+guidata/tests/conftest.py
+guidata/tests/test_activable_dataset.py
+guidata/tests/test_activable_items.py
+guidata/tests/test_all_features.py
+guidata/tests/test_all_items.py
 guidata/tests/test_arrayeditor.py
+guidata/tests/test_bool_selector.py
+guidata/tests/test_callbacks.py
 guidata/tests/test_codeeditor.py
 guidata/tests/test_collectionseditor.py
+guidata/tests/test_config.py
 guidata/tests/test_console.py
+guidata/tests/test_data.py
 guidata/tests/test_dataframeeditor.py
+guidata/tests/test_datasetgroup.py
+guidata/tests/test_disthelpers.py
+guidata/tests/test_editgroupbox.py
 guidata/tests/test_importwizard.py
+guidata/tests/test_inheritance.py
+guidata/tests/test_item_order.py
+guidata/tests/test_loadsave_hdf5.py
+guidata/tests/test_loadsave_json.py
 guidata/tests/test_objecteditor.py
-guidata/tests/text.py
-guidata/tests/translations.py
-guidata/tests/userconfig_app.py
+guidata/tests/test_rotatedlabel.py
+guidata/tests/test_text.py
+guidata/tests/test_translations.py
+guidata/tests/test_userconfig_app.py
+guidata/utils/__init__.py
+guidata/utils/disthelpers.py
+guidata/utils/encoding.py
+guidata/utils/genreqs.py
+guidata/utils/gettext_helpers.py
+guidata/utils/misc.py
 guidata/widgets/__init__.py
 guidata/widgets/arrayeditor.py
 guidata/widgets/codeeditor.py
 guidata/widgets/collectionseditor.py
 guidata/widgets/dataframeeditor.py
+guidata/widgets/dockable.py
 guidata/widgets/importwizard.py
 guidata/widgets/nsview.py
 guidata/widgets/objecteditor.py
+guidata/widgets/rotatedlabel.py
 guidata/widgets/syntaxhighlighters.py
 guidata/widgets/texteditor.py
 guidata/widgets/console/__init__.py
 guidata/widgets/console/base.py
 guidata/widgets/console/calltip.py
 guidata/widgets/console/dochelpers.py
 guidata/widgets/console/internalshell.py
```

