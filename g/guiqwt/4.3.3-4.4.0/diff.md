# Comparing `tmp/guiqwt-4.3.3.tar.gz` & `tmp/guiqwt-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guiqwt-4.3.3.tar", last modified: Mon Feb 20 09:14:46 2023, max compression
+gzip compressed data, was "guiqwt-4.4.0.tar", last modified: Thu Jul  6 17:58:21 2023, max compression
```

## Comparing `guiqwt-4.3.3.tar` & `guiqwt-4.4.0.tar`

### file list

```diff
@@ -1,315 +1,315 @@
-drwxrwxrwx   0        0        0        0 2023-02-20 09:14:46.456162 guiqwt-4.3.3/
--rw-rw-rw-   0        0        0    36023 2023-02-20 09:12:39.000000 guiqwt-4.3.3/CHANGELOG.md
--rw-rw-rw-   0        0        0    21603 2019-10-08 16:03:22.000000 guiqwt-4.3.3/Licence_CeCILL_V2-en.txt
--rw-rw-rw-   0        0        0      451 2021-02-06 17:38:23.000000 guiqwt-4.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2663 2023-02-20 09:14:46.456162 guiqwt-4.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     2516 2022-08-01 14:49:33.000000 guiqwt-4.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-02-20 09:14:46.023785 guiqwt-4.3.3/doc/
-drwxrwxrwx   0        0        0        0 2023-02-20 09:14:46.023785 guiqwt-4.3.3/doc/_static/
--rw-rw-rw-   0        0        0     7886 2019-10-08 16:03:22.000000 guiqwt-4.3.3/doc/_static/favicon.ico
--rw-rw-rw-   0        0        0     7119 2021-12-19 10:52:19.000000 guiqwt-4.3.3/doc/conf.py
--rw-rw-rw-   0        0        0      512 2021-12-19 10:39:43.000000 guiqwt-4.3.3/doc/development.rst
--rw-rw-rw-   0        0        0     1936 2021-12-19 10:55:25.000000 guiqwt-4.3.3/doc/disthelpers.rst
--rw-rw-rw-   0        0        0     3476 2021-02-06 17:38:23.000000 guiqwt-4.3.3/doc/examples.rst
-drwxrwxrwx   0        0        0        0 2023-02-20 09:14:46.023785 guiqwt-4.3.3/doc/images/
--rw-rw-rw-   0        0        0    32373 2021-02-06 17:38:23.000000 guiqwt-4.3.3/doc/images/curve_widgets.png
--rw-rw-rw-   0        0        0     3360 2019-10-08 16:03:22.000000 guiqwt-4.3.3/doc/images/guiqwt.png
--rw-rw-rw-   0        0        0    49787 2021-02-06 17:38:23.000000 guiqwt-4.3.3/doc/images/image_widgets.png
--rw-rw-rw-   0        0        0    28528 2019-10-08 16:03:22.000000 guiqwt-4.3.3/doc/images/my_plot_manager.png
--rw-rw-rw-   0        0        0   142571 2019-10-08 16:03:22.000000 guiqwt-4.3.3/doc/images/panorama.png
-drwxrwxrwx   0        0        0        0 2023-02-20 09:14:46.077205 guiqwt-4.3.3/doc/images/screenshots/
--rw-rw-rw-   0        0        0    33973 2019-10-08 16:03:22.000000 guiqwt-4.3.3/doc/images/screenshots/__init__.png
--rw-rw-rw-   0        0        0    32219 2019-10-08 16:03:22.000000 guiqwt-4.3.3/doc/images/screenshots/computations.png
--rw-rw-rw-   0        0        0   103911 2019-10-08 16:03:22.000000 guiqwt-4.3.3/doc/images/screenshots/contrast.png
--rw-rw-rw-   0        0        0   123005 2019-10-08 16:03:22.000000 guiqwt-4.3.3/doc/images/screenshots/cross_section.png
--rw-rw-rw-   0        0        0   123510 2019-10-08 16:03:22.000000 guiqwt-4.3.3/doc/images/screenshots/cross_section2.png
--rw-rw-rw-   0        0        0    68152 2021-02-06 17:38:23.000000 guiqwt-4.3.3/doc/images/screenshots/dotarraydemo.png
--rw-rw-rw-   0        0        0    52268 2019-10-08 16:03:22.000000 guiqwt-4.3.3/doc/images/screenshots/fit.png
--rw-rw-rw-   0        0        0    33435 2019-10-08 16:03:22.000000 guiqwt-4.3.3/doc/images/screenshots/get_point.png
--rw-rw-rw-   0        0        0    70160 2019-10-08 16:03:22.000000 guiqwt-4.3.3/doc/images/screenshots/hist2d.png
--rw-rw-rw-   0        0        0   146225 2019-10-08 16:03:22.000000 guiqwt-4.3.3/doc/images/screenshots/image_plot_tools.png
--rw-rw-rw-   0        0        0   114920 2019-10-08 16:03:22.000000 guiqwt-4.3.3/doc/images/screenshots/imagefilter.png
--rw-rw-rw-   0        0        0    73527 2019-10-08 16:03:22.000000 guiqwt-4.3.3/doc/images/screenshots/imagesuperp.png
--rw-rw-rw-   0        0        0   187178 2019-10-08 16:03:22.000000 guiqwt-4.3.3/doc/images/screenshots/imagexy.png
--rw-rw-rw-   0        0        0   100238 2019-10-08 16:03:22.000000 guiqwt-4.3.3/doc/images/screenshots/manager.png
--rw-rw-rw-   0        0        0   123059 2019-10-08 16:03:22.000000 guiqwt-4.3.3/doc/images/screenshots/mandelbrot.png
--rw-rw-rw-   0        0        0    49104 2019-10-08 16:03:22.000000 guiqwt-4.3.3/doc/images/screenshots/pcolor.png
--rw-rw-rw-   0        0        0    80158 2019-10-08 16:03:22.000000 guiqwt-4.3.3/doc/images/screenshots/plot.png
--rw-rw-rw-   0        0        0    66602 2019-10-08 16:03:22.000000 guiqwt-4.3.3/doc/images/screenshots/sift1.png
--rw-rw-rw-   0        0        0   139606 2019-10-08 16:03:22.000000 guiqwt-4.3.3/doc/images/screenshots/sift2.png
--rw-rw-rw-   0        0        0    94356 2019-10-08 16:03:22.000000 guiqwt-4.3.3/doc/images/screenshots/sift3.png
--rw-rw-rw-   0        0        0    47500 2019-10-08 16:03:22.000000 guiqwt-4.3.3/doc/images/screenshots/simple_dialog.png
--rw-rw-rw-   0        0        0    76231 2019-10-08 16:03:22.000000 guiqwt-4.3.3/doc/images/screenshots/simple_window.png
--rw-rw-rw-   0        0        0   391598 2019-10-08 16:03:22.000000 guiqwt-4.3.3/doc/images/screenshots/transform.png
--rw-rw-rw-   0        0        0      824 2021-02-06 17:38:23.000000 guiqwt-4.3.3/doc/index.rst
--rw-rw-rw-   0        0        0     1503 2022-08-01 14:49:33.000000 guiqwt-4.3.3/doc/installation.rst
--rw-rw-rw-   0        0        0     1360 2021-12-19 10:56:36.000000 guiqwt-4.3.3/doc/migrating_from_v2_to_v3.rst
--rw-rw-rw-   0        0        0     5960 2021-02-06 17:38:23.000000 guiqwt-4.3.3/doc/overview.rst
-drwxrwxrwx   0        0        0        0 2023-02-20 09:14:46.108466 guiqwt-4.3.3/doc/reference/
--rw-rw-rw-   0        0        0       36 2021-02-06 17:38:23.000000 guiqwt-4.3.3/doc/reference/annotations.rst
--rw-rw-rw-   0        0        0       33 2021-02-06 17:38:23.000000 guiqwt-4.3.3/doc/reference/baseplot.rst
--rw-rw-rw-   0        0        0       32 2021-02-06 17:38:23.000000 guiqwt-4.3.3/doc/reference/builder.rst
--rw-rw-rw-   0        0        0       38 2021-02-06 17:38:23.000000 guiqwt-4.3.3/doc/reference/cross_section.rst
--rw-rw-rw-   0        0        0       30 2021-02-06 17:38:23.000000 guiqwt-4.3.3/doc/reference/curve.rst
--rw-rw-rw-   0        0        0       34 2021-02-06 17:38:23.000000 guiqwt-4.3.3/doc/reference/histogram.rst
--rw-rw-rw-   0        0        0       30 2021-02-06 17:38:23.000000 guiqwt-4.3.3/doc/reference/image.rst
--rw-rw-rw-   0        0        0      345 2021-02-06 17:38:23.000000 guiqwt-4.3.3/doc/reference/index.rst
--rw-rw-rw-   0        0        0       27 2021-02-06 17:38:23.000000 guiqwt-4.3.3/doc/reference/io.rst
--rw-rw-rw-   0        0        0       30 2021-02-06 17:38:23.000000 guiqwt-4.3.3/doc/reference/label.rst
--rw-rw-rw-   0        0        0       31 2021-02-06 17:38:23.000000 guiqwt-4.3.3/doc/reference/panels.rst
--rw-rw-rw-   0        0        0       29 2021-02-06 17:38:23.000000 guiqwt-4.3.3/doc/reference/plot.rst
--rw-rw-rw-   0        0        0       31 2021-02-06 17:38:23.000000 guiqwt-4.3.3/doc/reference/pyplot.rst
--rw-rw-rw-   0        0        0       31 2021-02-06 17:38:23.000000 guiqwt-4.3.3/doc/reference/shapes.rst
--rw-rw-rw-   0        0        0       32 2021-02-06 17:38:23.000000 guiqwt-4.3.3/doc/reference/signals.rst
--rw-rw-rw-   0        0        0       31 2021-02-06 17:38:23.000000 guiqwt-4.3.3/doc/reference/styles.rst
--rw-rw-rw-   0        0        0       30 2021-02-06 17:38:23.000000 guiqwt-4.3.3/doc/reference/tools.rst
--rw-rw-rw-   0        0        0       36 2021-02-06 17:38:23.000000 guiqwt-4.3.3/doc/reference/widgets_fit.rst
--rw-rw-rw-   0        0        0       45 2021-02-06 17:38:23.000000 guiqwt-4.3.3/doc/reference/widgets_resizedialog.rst
--rw-rw-rw-   0        0        0       43 2021-02-06 17:38:23.000000 guiqwt-4.3.3/doc/reference/widgets_rotatecrop.rst
--rw-rw-rw-   0        0        0      894 2021-12-12 14:59:24.000000 guiqwt-4.3.3/doc/sift.rst
-drwxrwxrwx   0        0        0        0 2023-02-20 09:14:46.155347 guiqwt-4.3.3/guiqwt/
--rw-rw-rw-   0        0        0    26398 2023-02-20 09:01:00.000000 guiqwt-4.3.3/guiqwt/__init__.py
--rw-rw-rw-   0        0        0   421487 2021-12-11 14:47:07.000000 guiqwt-4.3.3/guiqwt/_cm.py
--rw-rw-rw-   0        0        0    24491 2021-12-19 10:52:24.000000 guiqwt-4.3.3/guiqwt/annotations.py
--rw-rw-rw-   0        0        0    34370 2023-02-19 13:53:09.000000 guiqwt-4.3.3/guiqwt/baseplot.py
--rw-rw-rw-   0        0        0    52650 2022-08-01 14:49:33.000000 guiqwt-4.3.3/guiqwt/builder.py
--rw-rw-rw-   0        0        0     3798 2021-03-13 15:31:59.000000 guiqwt-4.3.3/guiqwt/colormap.py
--rw-rw-rw-   0        0        0    33453 2022-08-01 14:49:33.000000 guiqwt-4.3.3/guiqwt/config.py
--rw-rw-rw-   0        0        0    36830 2022-08-01 14:49:33.000000 guiqwt-4.3.3/guiqwt/cross_section.py
--rw-rw-rw-   0        0        0    65700 2022-08-01 14:49:33.000000 guiqwt-4.3.3/guiqwt/curve.py
--rw-rw-rw-   0        0        0     2189 2021-12-19 10:50:52.000000 guiqwt-4.3.3/guiqwt/debug.py
--rw-rw-rw-   0        0        0    25456 2022-08-01 14:49:33.000000 guiqwt-4.3.3/guiqwt/events.py
--rw-rw-rw-   0        0        0     3003 2021-12-11 14:46:59.000000 guiqwt-4.3.3/guiqwt/geometry.py
--rw-rw-rw-   0        0        0    20152 2022-08-01 14:49:33.000000 guiqwt-4.3.3/guiqwt/histogram.py
--rw-rw-rw-   0        0        0   103547 2023-02-19 15:02:26.000000 guiqwt-4.3.3/guiqwt/image.py
-drwxrwxrwx   0        0        0        0 2023-02-20 09:14:46.224362 guiqwt-4.3.3/guiqwt/images/
--rw-rw-rw-   0        0        0      827 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/arrow_down.png
--rw-rw-rw-   0        0        0      828 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/arrow_up.png
--rw-rw-rw-   0        0        0     1095 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/autorefresh.png
--rw-rw-rw-   0        0        0      739 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/axes.png
--rw-rw-rw-   0        0        0      593 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/center.png
--rw-rw-rw-   0        0        0      562 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/contrast.png
--rw-rw-rw-   0        0        0     1227 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/copytoclipboard.png
--rw-rw-rw-   0        0        0      953 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/csapplylut.png
--rw-rw-rw-   0        0        0      426 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/csautoscale.png
--rw-rw-rw-   0        0        0      594 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/csection.png
--rw-rw-rw-   0        0        0      558 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/csection_a.png
--rw-rw-rw-   0        0        0      959 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/csection_oblique.png
--rw-rw-rw-   0        0        0      408 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/csperimage.png
-drwxrwxrwx   0        0        0        0 2023-02-20 09:14:46.224362 guiqwt-4.3.3/guiqwt/images/curvestyles/
--rw-rw-rw-   0        0        0      369 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/curvestyles/dots.png
--rw-rw-rw-   0        0        0      412 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/curvestyles/lines.png
--rw-rw-rw-   0        0        0      384 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/curvestyles/steps.png
--rw-rw-rw-   0        0        0      435 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/curvestyles/sticks.png
-drwxrwxrwx   0        0        0        0 2023-02-20 09:14:46.224362 guiqwt-4.3.3/guiqwt/images/curvetypes/
--rw-rw-rw-   0        0        0      570 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/curvetypes/xfy.png
--rw-rw-rw-   0        0        0      570 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/curvetypes/yfx.png
--rw-rw-rw-   0        0        0      430 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/eliminate_outliers.png
--rw-rw-rw-   0        0        0      882 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/eraser.png
--rw-rw-rw-   0        0        0     1108 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/export.png
--rw-rw-rw-   0        0        0      426 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/font.png
--rw-rw-rw-   0        0        0      432 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/full_range.png
--rw-rw-rw-   0        0        0     1112 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/funct.png
--rw-rw-rw-   0        0        0    15224 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/guiqwt.svg
--rw-rw-rw-   0        0        0      399 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/hcursor.png
--rw-rw-rw-   0        0        0      660 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/hflip.png
--rw-rw-rw-   0        0        0     1041 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/imagestats.png
--rw-rw-rw-   0        0        0      684 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/item_list.png
-drwxrwxrwx   0        0        0        0 2023-02-20 09:14:46.239987 guiqwt-4.3.3/guiqwt/images/items/
--rw-rw-rw-   0        0        0      877 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/items/annotation.png
--rw-rw-rw-   0        0        0      551 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/items/curve.png
--rw-rw-rw-   0        0        0      419 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/items/errorbar.png
--rw-rw-rw-   0        0        0      368 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/items/grid.png
--rw-rw-rw-   0        0        0      387 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/items/histogram.png
--rw-rw-rw-   0        0        0     1104 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/items/histogram2d.png
--rw-rw-rw-   0        0        0     1077 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/items/image.png
--rw-rw-rw-   0        0        0      742 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/items/label.png
--rw-rw-rw-   0        0        0      564 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/items/legend.png
--rw-rw-rw-   0        0        0     2267 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/magnifier.png
-drwxrwxrwx   0        0        0        0 2023-02-20 09:14:46.255611 guiqwt-4.3.3/guiqwt/images/markers/
--rw-rw-rw-   0        0        0      337 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/markers/cross.png
--rw-rw-rw-   0        0        0      420 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/markers/diamond.png
--rw-rw-rw-   0        0        0      468 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/markers/ellipse.png
--rw-rw-rw-   0        0        0      484 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/markers/hexagon.png
--rw-rw-rw-   0        0        0      331 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/markers/point.png
--rw-rw-rw-   0        0        0      363 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/markers/square.png
--rw-rw-rw-   0        0        0      357 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/markers/star.png
--rw-rw-rw-   0        0        0      449 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/markers/triangle_d.png
--rw-rw-rw-   0        0        0      445 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/markers/triangle_l.png
--rw-rw-rw-   0        0        0      438 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/markers/triangle_r.png
--rw-rw-rw-   0        0        0      449 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/markers/triangle_u.png
--rw-rw-rw-   0        0        0      349 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/markers/xcross.png
-drwxrwxrwx   0        0        0        0 2023-02-20 09:14:46.271238 guiqwt-4.3.3/guiqwt/images/markerstyles/
--rw-rw-rw-   0        0        0      343 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/markerstyles/cross_marker.png
--rw-rw-rw-   0        0        0      331 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/markerstyles/horiz_marker.png
--rw-rw-rw-   0        0        0      333 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/markerstyles/vert_marker.png
-drwxrwxrwx   0        0        0        0 2023-02-20 09:14:46.277747 guiqwt-4.3.3/guiqwt/images/mask/
--rw-rw-rw-   0        0        0      619 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/mask/mask_circle.png
--rw-rw-rw-   0        0        0      623 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/mask/mask_circle_outside.png
--rw-rw-rw-   0        0        0      445 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/mask/mask_rectangle.png
--rw-rw-rw-   0        0        0      446 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/mask/mask_rectangle_outside.png
--rw-rw-rw-   0        0        0      411 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/mask/mask_tool.png
--rw-rw-rw-   0        0        0      339 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/move.png
--rw-rw-rw-   0        0        0      644 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/on_curve.png
-drwxrwxrwx   0        0        0        0 2023-02-20 09:14:46.293391 guiqwt-4.3.3/guiqwt/images/patterns/
--rw-rw-rw-   0        0        0      325 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/patterns/bdiagpattern.png
--rw-rw-rw-   0        0        0      311 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/patterns/crosspattern.png
--rw-rw-rw-   0        0        0      303 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/patterns/dense1pattern.png
--rw-rw-rw-   0        0        0      305 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/patterns/dense2pattern.png
--rw-rw-rw-   0        0        0      309 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/patterns/dense3pattern.png
--rw-rw-rw-   0        0        0      300 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/patterns/dense4pattern.png
--rw-rw-rw-   0        0        0      307 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/patterns/dense5pattern.png
--rw-rw-rw-   0        0        0      311 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/patterns/dense6pattern.png
--rw-rw-rw-   0        0        0      308 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/patterns/dense7pattern.png
--rw-rw-rw-   0        0        0      324 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/patterns/diagcrosspattern.png
--rw-rw-rw-   0        0        0      330 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/patterns/fdiagpattern.png
--rw-rw-rw-   0        0        0      306 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/patterns/horpattern.png
--rw-rw-rw-   0        0        0      299 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/patterns/nobrush.png
--rw-rw-rw-   0        0        0      296 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/patterns/solidpattern.png
--rw-rw-rw-   0        0        0      304 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/patterns/verpattern.png
--rw-rw-rw-   0        0        0      442 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/point_selection.png
--rw-rw-rw-   0        0        0      913 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/print.png
--rw-rw-rw-   0        0        0      967 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/refresh.png
-drwxrwxrwx   0        0        0        0 2023-02-20 09:14:46.309019 guiqwt-4.3.3/guiqwt/images/scales/
--rw-rw-rw-   0        0        0      395 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/scales/lin_lin.png
--rw-rw-rw-   0        0        0      402 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/scales/lin_log.png
--rw-rw-rw-   0        0        0      403 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/scales/log_lin.png
--rw-rw-rw-   0        0        0      407 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/scales/log_log.png
-drwxrwxrwx   0        0        0        0 2023-02-20 09:14:46.324638 guiqwt-4.3.3/guiqwt/images/shapes/
--rw-rw-rw-   0        0        0      777 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/shapes/circle.png
--rw-rw-rw-   0        0        0      794 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/shapes/ellipse_shape.png
--rw-rw-rw-   0        0        0      552 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/shapes/freeform.png
--rw-rw-rw-   0        0        0      568 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/shapes/gtaxes.png
--rw-rw-rw-   0        0        0      426 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/shapes/marker.png
--rw-rw-rw-   0        0        0      898 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/shapes/oblique_rectangle.png
--rw-rw-rw-   0        0        0      366 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/shapes/point_shape.png
--rw-rw-rw-   0        0        0      479 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/shapes/polyline.png
--rw-rw-rw-   0        0        0      426 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/shapes/rectangle.png
--rw-rw-rw-   0        0        0      467 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/shapes/segment.png
--rw-rw-rw-   0        0        0    14258 2019-10-08 16:03:22.000000 guiqwt-4.3.3/guiqwt/images/sift.svg
--rw-rw-rw-   0        0        0     1340 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/snapshot.png
-drwxrwxrwx   0        0        0        0 2023-02-20 09:14:46.324638 guiqwt-4.3.3/guiqwt/images/styles/
--rw-rw-rw-   0        0        0      333 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/styles/dash.png
--rw-rw-rw-   0        0        0      338 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/styles/dashdot.png
--rw-rw-rw-   0        0        0      332 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/styles/dashdotdot.png
--rw-rw-rw-   0        0        0      328 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/styles/dot.png
--rw-rw-rw-   0        0        0      328 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/styles/solid.png
--rw-rw-rw-   0        0        0      401 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/trash.png
--rw-rw-rw-   0        0        0      407 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/vcursor.png
--rw-rw-rw-   0        0        0      658 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/vflip.png
--rw-rw-rw-   0        0        0      375 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/xcursor.png
--rw-rw-rw-   0        0        0      417 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/images/xrange.png
--rw-rw-rw-   0        0        0     9529 2021-12-11 14:46:59.000000 guiqwt-4.3.3/guiqwt/interfaces.py
--rw-rw-rw-   0        0        0    21844 2022-09-05 12:23:31.000000 guiqwt-4.3.3/guiqwt/io.py
--rw-rw-rw-   0        0        0    20125 2022-02-26 07:48:18.000000 guiqwt-4.3.3/guiqwt/label.py
-drwxrwxrwx   0        0        0        0 2023-02-20 09:14:46.324638 guiqwt-4.3.3/guiqwt/locale/
-drwxrwxrwx   0        0        0        0 2023-02-20 09:14:45.992555 guiqwt-4.3.3/guiqwt/locale/fr/
-drwxrwxrwx   0        0        0        0 2023-02-20 09:14:46.324638 guiqwt-4.3.3/guiqwt/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0        0        0    30153 2023-02-20 09:04:37.000000 guiqwt-4.3.3/guiqwt/locale/fr/LC_MESSAGES/guiqwt.mo
--rw-rw-rw-   0        0        0    57708 2022-08-01 14:49:33.000000 guiqwt-4.3.3/guiqwt/locale/fr/LC_MESSAGES/guiqwt.po
--rw-rw-rw-   0        0        0    44618 2023-02-20 09:03:54.000000 guiqwt-4.3.3/guiqwt/locale/guiqwt.pot
--rw-rw-rw-   0        0        0     3269 2021-12-11 14:47:00.000000 guiqwt-4.3.3/guiqwt/panels.py
--rw-rw-rw-   0        0        0    48784 2023-02-19 15:02:26.000000 guiqwt-4.3.3/guiqwt/plot.py
--rw-rw-rw-   0        0        0    19841 2023-02-19 15:02:16.000000 guiqwt-4.3.3/guiqwt/pyplot.py
--rw-rw-rw-   0        0        0     3361 2021-12-19 11:05:20.000000 guiqwt-4.3.3/guiqwt/qtdesigner.py
--rw-rw-rw-   0        0        0     5824 2022-04-08 12:35:06.000000 guiqwt-4.3.3/guiqwt/qthelpers.py
--rw-rw-rw-   0        0        0     1852 2021-12-11 14:47:00.000000 guiqwt-4.3.3/guiqwt/scaler.py
--rw-rw-rw-   0        0        0    53858 2022-08-01 14:49:33.000000 guiqwt-4.3.3/guiqwt/shapes.py
--rw-rw-rw-   0        0        0     4452 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/signals.py
--rw-rw-rw-   0        0        0    62787 2022-08-01 14:49:33.000000 guiqwt-4.3.3/guiqwt/styles.py
-drwxrwxrwx   0        0        0        0 2023-02-20 09:14:46.424910 guiqwt-4.3.3/guiqwt/tests/
--rw-rw-rw-   0        0        0      440 2021-12-11 14:47:02.000000 guiqwt-4.3.3/guiqwt/tests/__init__.py
--rw-rw-rw-   0        0        0     4365 2021-12-19 10:58:49.000000 guiqwt-4.3.3/guiqwt/tests/benchmarks.py
--rw-rw-rw-   0        0        0    39666 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/tests/brain.png
--rw-rw-rw-   0        0        0    35354 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/tests/brain_cylinder.png
--rw-rw-rw-   0        0        0     1410 2021-12-19 10:53:01.000000 guiqwt-4.3.3/guiqwt/tests/computations.py
--rw-rw-rw-   0        0        0     1124 2021-12-11 14:47:02.000000 guiqwt-4.3.3/guiqwt/tests/contrast.py
--rw-rw-rw-   0        0        0     1200 2021-12-11 14:47:02.000000 guiqwt-4.3.3/guiqwt/tests/cross_section.py
--rw-rw-rw-   0        0        0     2057 2021-12-11 14:47:02.000000 guiqwt-4.3.3/guiqwt/tests/cross_section_oblique.py
--rw-rw-rw-   0        0        0     1180 2021-12-11 14:47:02.000000 guiqwt-4.3.3/guiqwt/tests/cursors.py
--rw-rw-rw-   0        0        0     1778 2021-12-11 14:47:02.000000 guiqwt-4.3.3/guiqwt/tests/customize_shape_tool.py
--rw-rw-rw-   0        0        0     1013 2021-12-11 14:47:02.000000 guiqwt-4.3.3/guiqwt/tests/dicom_image.py
--rw-rw-rw-   0        0        0     6109 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/tests/dotarraydemo.py
--rw-rw-rw-   0        0        0     2875 2021-12-11 14:47:02.000000 guiqwt-4.3.3/guiqwt/tests/filtertest1.py
--rw-rw-rw-   0        0        0     3626 2021-12-04 15:10:24.000000 guiqwt-4.3.3/guiqwt/tests/filtertest2.py
--rw-rw-rw-   0        0        0      843 2021-12-19 10:51:49.000000 guiqwt-4.3.3/guiqwt/tests/fit.py
--rw-rw-rw-   0        0        0     1189 2021-12-11 14:47:02.000000 guiqwt-4.3.3/guiqwt/tests/fliprotate.py
--rw-rw-rw-   0        0        0      462 2021-12-11 14:47:02.000000 guiqwt-4.3.3/guiqwt/tests/fontparam.py
--rw-rw-rw-   0        0        0     1550 2021-12-19 10:51:28.000000 guiqwt-4.3.3/guiqwt/tests/get_point.py
--rw-rw-rw-   0        0        0     1553 2021-12-19 10:51:38.000000 guiqwt-4.3.3/guiqwt/tests/get_segment.py
--rw-rw-rw-   0        0        0      857 2021-12-11 14:47:02.000000 guiqwt-4.3.3/guiqwt/tests/highprecisionxy.py
--rw-rw-rw-   0        0        0     1244 2021-12-11 14:47:02.000000 guiqwt-4.3.3/guiqwt/tests/hist2d.py
--rw-rw-rw-   0        0        0     1357 2021-12-11 14:47:02.000000 guiqwt-4.3.3/guiqwt/tests/hist2d_func.py
--rw-rw-rw-   0        0        0      730 2022-06-09 15:21:58.000000 guiqwt-4.3.3/guiqwt/tests/histogram.py
--rw-rw-rw-   0        0        0     3082 2023-02-19 14:59:44.000000 guiqwt-4.3.3/guiqwt/tests/image.py
--rw-rw-rw-   0        0        0     1724 2023-02-19 13:01:53.000000 guiqwt-4.3.3/guiqwt/tests/image_coords.py
--rw-rw-rw-   0        0        0     1488 2021-12-19 10:51:49.000000 guiqwt-4.3.3/guiqwt/tests/image_masked.py
--rw-rw-rw-   0        0        0     1902 2021-12-11 14:47:02.000000 guiqwt-4.3.3/guiqwt/tests/image_plot_tools.py
--rw-rw-rw-   0        0        0     1026 2021-12-11 14:47:02.000000 guiqwt-4.3.3/guiqwt/tests/image_rgb.py
--rw-rw-rw-   0        0        0     1671 2021-12-11 14:47:02.000000 guiqwt-4.3.3/guiqwt/tests/imagefilter.py
--rw-rw-rw-   0        0        0     1641 2021-12-11 14:47:02.000000 guiqwt-4.3.3/guiqwt/tests/imagesuperp.py
--rw-rw-rw-   0        0        0     1716 2021-12-19 10:51:38.000000 guiqwt-4.3.3/guiqwt/tests/imagexy.py
--rw-rw-rw-   0        0        0      907 2021-12-11 14:47:02.000000 guiqwt-4.3.3/guiqwt/tests/loadsaveitems_hdf5.py
--rw-rw-rw-   0        0        0     1306 2022-08-01 14:49:33.000000 guiqwt-4.3.3/guiqwt/tests/loadsaveitems_json.py
--rw-rw-rw-   0        0        0     3917 2021-12-19 10:51:38.000000 guiqwt-4.3.3/guiqwt/tests/loadsaveitems_pickle.py
--rw-rw-rw-   0        0        0     2746 2021-12-04 15:10:45.000000 guiqwt-4.3.3/guiqwt/tests/loadtest.py
--rw-rw-rw-   0        0        0     2438 2021-12-04 15:11:01.000000 guiqwt-4.3.3/guiqwt/tests/manager.py
--rw-rw-rw-   0        0        0     2653 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/tests/mandelbrot.py
--rw-rw-rw-   0        0        0   525620 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/tests/mr-brain.dcm
--rw-rw-rw-   0        0        0     2696 2021-12-19 10:51:38.000000 guiqwt-4.3.3/guiqwt/tests/pcolor.py
--rw-rw-rw-   0        0        0     1838 2021-02-06 18:06:49.000000 guiqwt-4.3.3/guiqwt/tests/plot.py
--rw-rw-rw-   0        0        0      971 2021-12-11 14:47:02.000000 guiqwt-4.3.3/guiqwt/tests/plot_log.py
--rw-rw-rw-   0        0        0    14187 2022-08-01 14:49:33.000000 guiqwt-4.3.3/guiqwt/tests/plot_timecurve.py
--rw-rw-rw-   0        0        0      848 2021-12-11 14:47:02.000000 guiqwt-4.3.3/guiqwt/tests/plot_yreverse.py
--rw-rw-rw-   0        0        0      650 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/tests/png_test.py
--rw-rw-rw-   0        0        0     2231 2021-12-19 10:51:27.000000 guiqwt-4.3.3/guiqwt/tests/polygons.py
--rw-rw-rw-   0        0        0     1923 2023-02-19 15:02:16.000000 guiqwt-4.3.3/guiqwt/tests/pyplot.py
--rw-rw-rw-   0        0        0     1069 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/tests/qtdesigner.py
--rw-rw-rw-   0        0        0      993 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/tests/qtdesigner.ui
--rw-rw-rw-   0        0        0      653 2021-12-11 14:47:03.000000 guiqwt-4.3.3/guiqwt/tests/resize.py
--rw-rw-rw-   0        0        0     2846 2021-12-19 10:51:28.000000 guiqwt-4.3.3/guiqwt/tests/rotatecrop.py
--rw-rw-rw-   0        0        0    54632 2022-08-01 14:49:33.000000 guiqwt-4.3.3/guiqwt/tests/sift.py
--rw-rw-rw-   0        0        0     3793 2021-12-11 14:47:03.000000 guiqwt-4.3.3/guiqwt/tests/simple_dialog.py
--rw-rw-rw-   0        0        0     9272 2021-12-19 11:07:19.000000 guiqwt-4.3.3/guiqwt/tests/simple_window.py
--rw-rw-rw-   0        0        0     2958 2021-02-06 17:38:23.000000 guiqwt-4.3.3/guiqwt/tests/styles.py
--rw-rw-rw-   0        0        0     3754 2023-02-19 15:02:26.000000 guiqwt-4.3.3/guiqwt/tests/syncplot.py
--rw-rw-rw-   0        0        0     1338 2021-12-19 10:51:58.000000 guiqwt-4.3.3/guiqwt/tests/test_line.py
--rw-rw-rw-   0        0        0     5388 2022-01-05 14:35:00.000000 guiqwt-4.3.3/guiqwt/tests/transform.py
--rw-rw-rw-   0        0        0    88282 2023-02-09 08:15:33.000000 guiqwt-4.3.3/guiqwt/tools.py
--rw-rw-rw-   0        0        0      749 2021-12-11 14:47:03.000000 guiqwt-4.3.3/guiqwt/transitional.py
-drwxrwxrwx   0        0        0        0 2023-02-20 09:14:46.424910 guiqwt-4.3.3/guiqwt/widgets/
--rw-rw-rw-   0        0        0      578 2019-10-08 16:03:22.000000 guiqwt-4.3.3/guiqwt/widgets/__init__.py
--rw-rw-rw-   0        0        0     8406 2021-12-11 14:47:03.000000 guiqwt-4.3.3/guiqwt/widgets/base.py
--rw-rw-rw-   0        0        0    24367 2022-08-01 14:49:33.000000 guiqwt-4.3.3/guiqwt/widgets/fit.py
--rw-rw-rw-   0        0        0     5169 2022-08-01 14:49:33.000000 guiqwt-4.3.3/guiqwt/widgets/fliprotate.py
--rw-rw-rw-   0        0        0     5064 2021-12-19 10:53:14.000000 guiqwt-4.3.3/guiqwt/widgets/resizedialog.py
--rw-rw-rw-   0        0        0     4550 2021-12-11 14:47:04.000000 guiqwt-4.3.3/guiqwt/widgets/rotatecrop.py
-drwxrwxrwx   0        0        0        0 2023-02-20 09:14:46.155347 guiqwt-4.3.3/guiqwt.egg-info/
--rw-rw-rw-   0        0        0     2663 2023-02-20 09:14:45.000000 guiqwt-4.3.3/guiqwt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8112 2023-02-20 09:14:45.000000 guiqwt-4.3.3/guiqwt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-20 09:14:45.000000 guiqwt-4.3.3/guiqwt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-02-20 09:14:45.000000 guiqwt-4.3.3/guiqwt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      111 2023-02-20 09:14:45.000000 guiqwt-4.3.3/guiqwt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-02-20 09:14:45.000000 guiqwt-4.3.3/guiqwt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      112 2022-08-01 14:49:33.000000 guiqwt-4.3.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-02-20 09:14:46.424910 guiqwt-4.3.3/qtdesigner/
--rw-rw-rw-   0        0        0      446 2019-10-08 16:03:22.000000 guiqwt-4.3.3/qtdesigner/imageplotplugin.py
--rw-rw-rw-   0        0        0      435 2019-10-08 16:03:22.000000 guiqwt-4.3.3/qtdesigner/plotplugin.py
--rw-rw-rw-   0        0        0       42 2023-02-20 09:14:46.456162 guiqwt-4.3.3/setup.cfg
--rw-rw-rw-   0        0        0     8420 2023-02-20 09:09:48.000000 guiqwt-4.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-20 09:14:46.440539 guiqwt-4.3.3/sift/
--rw-rw-rw-   0        0        0     1124 2021-12-12 14:59:49.000000 guiqwt-4.3.3/sift/create_exe.py
--rw-rw-rw-   0        0        0   100952 2019-10-08 16:03:22.000000 guiqwt-4.3.3/sift/sift.ico
--rw-rw-rw-   0        0        0       64 2019-10-08 16:03:22.000000 guiqwt-4.3.3/sift/sift.pyw
-drwxrwxrwx   0        0        0        0 2023-02-20 09:14:46.456162 guiqwt-4.3.3/src/
--rw-rw-rw-   0        0        0     4647 2019-10-08 16:03:22.000000 guiqwt-4.3.3/src/arrays.hpp
--rw-rw-rw-   0        0        0      681 2019-10-08 16:03:22.000000 guiqwt-4.3.3/src/debug.hpp
--rw-rw-rw-   0        0        0   295116 2023-02-20 09:14:32.000000 guiqwt-4.3.3/src/histogram2d.c
--rw-rw-rw-   0        0        0     3434 2019-10-08 16:03:22.000000 guiqwt-4.3.3/src/histogram2d.pyx
--rw-rw-rw-   0        0        0   232562 2023-02-20 09:14:33.000000 guiqwt-4.3.3/src/mandelbrot.c
--rw-rw-rw-   0        0        0     1168 2019-10-08 16:03:22.000000 guiqwt-4.3.3/src/mandelbrot.pyx
--rw-rw-rw-   0        0        0    11581 2021-02-06 17:38:23.000000 guiqwt-4.3.3/src/pcolor.cpp
--rw-rw-rw-   0        0        0     6127 2019-10-08 16:03:22.000000 guiqwt-4.3.3/src/points.hpp
--rw-rw-rw-   0        0        0    22897 2021-02-06 17:38:23.000000 guiqwt-4.3.3/src/scaler.cpp
--rw-rw-rw-   0        0        0     2376 2019-10-08 16:03:22.000000 guiqwt-4.3.3/src/scaler.hpp
--rw-rw-rw-   0        0        0     4137 2022-08-01 14:49:33.000000 guiqwt-4.3.3/src/traits.hpp
+drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.663087 guiqwt-4.4.0/
+-rw-rw-rw-   0        0        0    37564 2023-07-06 17:55:17.000000 guiqwt-4.4.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0    21603 2019-10-08 16:03:22.000000 guiqwt-4.4.0/Licence_CeCILL_V2-en.txt
+-rw-rw-rw-   0        0        0      451 2021-02-06 17:38:23.000000 guiqwt-4.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2640 2023-07-06 17:58:21.663087 guiqwt-4.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2516 2022-08-01 14:49:33.000000 guiqwt-4.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 17:58:20.958638 guiqwt-4.4.0/doc/
+drwxrwxrwx   0        0        0        0 2023-07-06 17:58:20.958638 guiqwt-4.4.0/doc/_static/
+-rw-rw-rw-   0        0        0     7886 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/_static/favicon.ico
+-rw-rw-rw-   0        0        0     7119 2021-12-19 10:52:19.000000 guiqwt-4.4.0/doc/conf.py
+-rw-rw-rw-   0        0        0      512 2021-12-19 10:39:43.000000 guiqwt-4.4.0/doc/development.rst
+-rw-rw-rw-   0        0        0     1942 2023-07-06 13:56:54.000000 guiqwt-4.4.0/doc/disthelpers.rst
+-rw-rw-rw-   0        0        0     2648 2023-07-06 17:17:16.000000 guiqwt-4.4.0/doc/examples.rst
+drwxrwxrwx   0        0        0        0 2023-07-06 17:58:20.958638 guiqwt-4.4.0/doc/images/
+-rw-rw-rw-   0        0        0    32373 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/images/curve_widgets.png
+-rw-rw-rw-   0        0        0     3360 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/guiqwt.png
+-rw-rw-rw-   0        0        0    49787 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/images/image_widgets.png
+-rw-rw-rw-   0        0        0    28528 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/my_plot_manager.png
+-rw-rw-rw-   0        0        0   142571 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/panorama.png
+drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.027667 guiqwt-4.4.0/doc/images/screenshots/
+-rw-rw-rw-   0        0        0    33973 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/__init__.png
+-rw-rw-rw-   0        0        0    32219 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/computations.png
+-rw-rw-rw-   0        0        0   103911 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/contrast.png
+-rw-rw-rw-   0        0        0   123005 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/cross_section.png
+-rw-rw-rw-   0        0        0   123510 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/cross_section2.png
+-rw-rw-rw-   0        0        0    68152 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/images/screenshots/dotarraydemo.png
+-rw-rw-rw-   0        0        0    52268 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/fit.png
+-rw-rw-rw-   0        0        0    33435 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/get_point.png
+-rw-rw-rw-   0        0        0    70160 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/hist2d.png
+-rw-rw-rw-   0        0        0   146225 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/image_plot_tools.png
+-rw-rw-rw-   0        0        0   114920 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/imagefilter.png
+-rw-rw-rw-   0        0        0    73527 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/imagesuperp.png
+-rw-rw-rw-   0        0        0   187178 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/imagexy.png
+-rw-rw-rw-   0        0        0   100238 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/manager.png
+-rw-rw-rw-   0        0        0   123059 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/mandelbrot.png
+-rw-rw-rw-   0        0        0    49104 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/pcolor.png
+-rw-rw-rw-   0        0        0    80158 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/plot.png
+-rw-rw-rw-   0        0        0    66602 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/sift1.png
+-rw-rw-rw-   0        0        0   139606 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/sift2.png
+-rw-rw-rw-   0        0        0    94356 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/sift3.png
+-rw-rw-rw-   0        0        0    47500 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/simple_dialog.png
+-rw-rw-rw-   0        0        0    76231 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/simple_window.png
+-rw-rw-rw-   0        0        0   391598 2019-10-08 16:03:22.000000 guiqwt-4.4.0/doc/images/screenshots/transform.png
+-rw-rw-rw-   0        0        0      824 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/index.rst
+-rw-rw-rw-   0        0        0     1503 2023-07-06 13:43:56.000000 guiqwt-4.4.0/doc/installation.rst
+-rw-rw-rw-   0        0        0     1360 2021-12-19 10:56:36.000000 guiqwt-4.4.0/doc/migrating_from_v2_to_v3.rst
+-rw-rw-rw-   0        0        0     5960 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/overview.rst
+drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.058937 guiqwt-4.4.0/doc/reference/
+-rw-rw-rw-   0        0        0       36 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/annotations.rst
+-rw-rw-rw-   0        0        0       33 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/baseplot.rst
+-rw-rw-rw-   0        0        0       32 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/builder.rst
+-rw-rw-rw-   0        0        0       38 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/cross_section.rst
+-rw-rw-rw-   0        0        0       30 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/curve.rst
+-rw-rw-rw-   0        0        0       34 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/histogram.rst
+-rw-rw-rw-   0        0        0       30 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/image.rst
+-rw-rw-rw-   0        0        0      345 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/index.rst
+-rw-rw-rw-   0        0        0       27 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/io.rst
+-rw-rw-rw-   0        0        0       30 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/label.rst
+-rw-rw-rw-   0        0        0       31 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/panels.rst
+-rw-rw-rw-   0        0        0       29 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/plot.rst
+-rw-rw-rw-   0        0        0       31 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/pyplot.rst
+-rw-rw-rw-   0        0        0       31 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/shapes.rst
+-rw-rw-rw-   0        0        0       32 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/signals.rst
+-rw-rw-rw-   0        0        0       31 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/styles.rst
+-rw-rw-rw-   0        0        0       30 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/tools.rst
+-rw-rw-rw-   0        0        0       36 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/widgets_fit.rst
+-rw-rw-rw-   0        0        0       45 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/widgets_resizedialog.rst
+-rw-rw-rw-   0        0        0       43 2021-02-06 17:38:23.000000 guiqwt-4.4.0/doc/reference/widgets_rotatecrop.rst
+-rw-rw-rw-   0        0        0      903 2023-06-10 14:03:47.000000 guiqwt-4.4.0/doc/sift.rst
+drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.121451 guiqwt-4.4.0/guiqwt/
+-rw-rw-rw-   0        0        0    26398 2023-06-04 08:30:11.000000 guiqwt-4.4.0/guiqwt/__init__.py
+-rw-rw-rw-   0        0        0   421487 2021-12-11 14:47:07.000000 guiqwt-4.4.0/guiqwt/_cm.py
+-rw-rw-rw-   0        0        0    24601 2023-07-06 13:47:44.000000 guiqwt-4.4.0/guiqwt/annotations.py
+-rw-rw-rw-   0        0        0    34502 2023-07-06 13:55:37.000000 guiqwt-4.4.0/guiqwt/baseplot.py
+-rw-rw-rw-   0        0        0    53108 2023-06-04 08:46:35.000000 guiqwt-4.4.0/guiqwt/builder.py
+-rw-rw-rw-   0        0        0     3798 2021-03-13 15:31:59.000000 guiqwt-4.4.0/guiqwt/colormap.py
+-rw-rw-rw-   0        0        0    33453 2023-05-14 09:35:27.000000 guiqwt-4.4.0/guiqwt/config.py
+-rw-rw-rw-   0        0        0    36835 2023-07-06 13:48:38.000000 guiqwt-4.4.0/guiqwt/cross_section.py
+-rw-rw-rw-   0        0        0    65731 2023-07-06 13:49:01.000000 guiqwt-4.4.0/guiqwt/curve.py
+-rw-rw-rw-   0        0        0     2189 2021-12-19 10:50:52.000000 guiqwt-4.4.0/guiqwt/debug.py
+-rw-rw-rw-   0        0        0    25456 2022-08-01 14:49:33.000000 guiqwt-4.4.0/guiqwt/events.py
+-rw-rw-rw-   0        0        0     3003 2021-12-11 14:46:59.000000 guiqwt-4.4.0/guiqwt/geometry.py
+-rw-rw-rw-   0        0        0    20183 2023-07-06 13:49:23.000000 guiqwt-4.4.0/guiqwt/histogram.py
+-rw-rw-rw-   0        0        0   103756 2023-07-06 13:54:21.000000 guiqwt-4.4.0/guiqwt/image.py
+drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.240439 guiqwt-4.4.0/guiqwt/images/
+-rw-rw-rw-   0        0        0      827 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/arrow_down.png
+-rw-rw-rw-   0        0        0      828 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/arrow_up.png
+-rw-rw-rw-   0        0        0     1095 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/autorefresh.png
+-rw-rw-rw-   0        0        0      739 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/axes.png
+-rw-rw-rw-   0        0        0      593 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/center.png
+-rw-rw-rw-   0        0        0      562 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/contrast.png
+-rw-rw-rw-   0        0        0     1227 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/copytoclipboard.png
+-rw-rw-rw-   0        0        0      953 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/csapplylut.png
+-rw-rw-rw-   0        0        0      426 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/csautoscale.png
+-rw-rw-rw-   0        0        0      594 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/csection.png
+-rw-rw-rw-   0        0        0      558 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/csection_a.png
+-rw-rw-rw-   0        0        0      959 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/csection_oblique.png
+-rw-rw-rw-   0        0        0      408 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/csperimage.png
+drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.250516 guiqwt-4.4.0/guiqwt/images/curvestyles/
+-rw-rw-rw-   0        0        0      369 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/curvestyles/dots.png
+-rw-rw-rw-   0        0        0      412 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/curvestyles/lines.png
+-rw-rw-rw-   0        0        0      384 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/curvestyles/steps.png
+-rw-rw-rw-   0        0        0      435 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/curvestyles/sticks.png
+drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.260614 guiqwt-4.4.0/guiqwt/images/curvetypes/
+-rw-rw-rw-   0        0        0      570 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/curvetypes/xfy.png
+-rw-rw-rw-   0        0        0      570 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/curvetypes/yfx.png
+-rw-rw-rw-   0        0        0      430 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/eliminate_outliers.png
+-rw-rw-rw-   0        0        0      882 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/eraser.png
+-rw-rw-rw-   0        0        0     1108 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/export.png
+-rw-rw-rw-   0        0        0      426 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/font.png
+-rw-rw-rw-   0        0        0      432 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/full_range.png
+-rw-rw-rw-   0        0        0     1112 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/funct.png
+-rw-rw-rw-   0        0        0    15224 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/guiqwt.svg
+-rw-rw-rw-   0        0        0      399 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/hcursor.png
+-rw-rw-rw-   0        0        0      660 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/hflip.png
+-rw-rw-rw-   0        0        0     1041 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/imagestats.png
+-rw-rw-rw-   0        0        0      684 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/item_list.png
+drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.299313 guiqwt-4.4.0/guiqwt/images/items/
+-rw-rw-rw-   0        0        0      877 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/items/annotation.png
+-rw-rw-rw-   0        0        0      551 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/items/curve.png
+-rw-rw-rw-   0        0        0      419 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/items/errorbar.png
+-rw-rw-rw-   0        0        0      368 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/items/grid.png
+-rw-rw-rw-   0        0        0      387 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/items/histogram.png
+-rw-rw-rw-   0        0        0     1104 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/items/histogram2d.png
+-rw-rw-rw-   0        0        0     1077 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/items/image.png
+-rw-rw-rw-   0        0        0      742 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/items/label.png
+-rw-rw-rw-   0        0        0      564 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/items/legend.png
+-rw-rw-rw-   0        0        0     2267 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/magnifier.png
+drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.321534 guiqwt-4.4.0/guiqwt/images/markers/
+-rw-rw-rw-   0        0        0      337 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/markers/cross.png
+-rw-rw-rw-   0        0        0      420 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/markers/diamond.png
+-rw-rw-rw-   0        0        0      468 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/markers/ellipse.png
+-rw-rw-rw-   0        0        0      484 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/markers/hexagon.png
+-rw-rw-rw-   0        0        0      331 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/markers/point.png
+-rw-rw-rw-   0        0        0      363 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/markers/square.png
+-rw-rw-rw-   0        0        0      357 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/markers/star.png
+-rw-rw-rw-   0        0        0      449 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/markers/triangle_d.png
+-rw-rw-rw-   0        0        0      445 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/markers/triangle_l.png
+-rw-rw-rw-   0        0        0      438 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/markers/triangle_r.png
+-rw-rw-rw-   0        0        0      449 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/markers/triangle_u.png
+-rw-rw-rw-   0        0        0      349 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/markers/xcross.png
+drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.331605 guiqwt-4.4.0/guiqwt/images/markerstyles/
+-rw-rw-rw-   0        0        0      343 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/markerstyles/cross_marker.png
+-rw-rw-rw-   0        0        0      331 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/markerstyles/horiz_marker.png
+-rw-rw-rw-   0        0        0      333 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/markerstyles/vert_marker.png
+drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.339652 guiqwt-4.4.0/guiqwt/images/mask/
+-rw-rw-rw-   0        0        0      619 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/mask/mask_circle.png
+-rw-rw-rw-   0        0        0      623 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/mask/mask_circle_outside.png
+-rw-rw-rw-   0        0        0      445 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/mask/mask_rectangle.png
+-rw-rw-rw-   0        0        0      446 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/mask/mask_rectangle_outside.png
+-rw-rw-rw-   0        0        0      411 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/mask/mask_tool.png
+-rw-rw-rw-   0        0        0      339 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/move.png
+-rw-rw-rw-   0        0        0      644 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/on_curve.png
+drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.369823 guiqwt-4.4.0/guiqwt/images/patterns/
+-rw-rw-rw-   0        0        0      325 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/patterns/bdiagpattern.png
+-rw-rw-rw-   0        0        0      311 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/patterns/crosspattern.png
+-rw-rw-rw-   0        0        0      303 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/patterns/dense1pattern.png
+-rw-rw-rw-   0        0        0      305 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/patterns/dense2pattern.png
+-rw-rw-rw-   0        0        0      309 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/patterns/dense3pattern.png
+-rw-rw-rw-   0        0        0      300 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/patterns/dense4pattern.png
+-rw-rw-rw-   0        0        0      307 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/patterns/dense5pattern.png
+-rw-rw-rw-   0        0        0      311 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/patterns/dense6pattern.png
+-rw-rw-rw-   0        0        0      308 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/patterns/dense7pattern.png
+-rw-rw-rw-   0        0        0      324 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/patterns/diagcrosspattern.png
+-rw-rw-rw-   0        0        0      330 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/patterns/fdiagpattern.png
+-rw-rw-rw-   0        0        0      306 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/patterns/horpattern.png
+-rw-rw-rw-   0        0        0      299 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/patterns/nobrush.png
+-rw-rw-rw-   0        0        0      296 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/patterns/solidpattern.png
+-rw-rw-rw-   0        0        0      304 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/patterns/verpattern.png
+-rw-rw-rw-   0        0        0      442 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/point_selection.png
+-rw-rw-rw-   0        0        0      913 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/print.png
+-rw-rw-rw-   0        0        0      967 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/refresh.png
+drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.369823 guiqwt-4.4.0/guiqwt/images/scales/
+-rw-rw-rw-   0        0        0      395 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/scales/lin_lin.png
+-rw-rw-rw-   0        0        0      402 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/scales/lin_log.png
+-rw-rw-rw-   0        0        0      403 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/scales/log_lin.png
+-rw-rw-rw-   0        0        0      407 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/scales/log_log.png
+drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.385458 guiqwt-4.4.0/guiqwt/images/shapes/
+-rw-rw-rw-   0        0        0      777 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/shapes/circle.png
+-rw-rw-rw-   0        0        0      794 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/shapes/ellipse_shape.png
+-rw-rw-rw-   0        0        0      552 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/shapes/freeform.png
+-rw-rw-rw-   0        0        0      568 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/shapes/gtaxes.png
+-rw-rw-rw-   0        0        0      426 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/shapes/marker.png
+-rw-rw-rw-   0        0        0      898 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/shapes/oblique_rectangle.png
+-rw-rw-rw-   0        0        0      366 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/shapes/point_shape.png
+-rw-rw-rw-   0        0        0      479 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/shapes/polyline.png
+-rw-rw-rw-   0        0        0      426 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/shapes/rectangle.png
+-rw-rw-rw-   0        0        0      467 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/shapes/segment.png
+-rw-rw-rw-   0        0        0    14258 2019-10-08 16:03:22.000000 guiqwt-4.4.0/guiqwt/images/sift.svg
+-rw-rw-rw-   0        0        0     1340 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/snapshot.png
+drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.401085 guiqwt-4.4.0/guiqwt/images/styles/
+-rw-rw-rw-   0        0        0      333 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/styles/dash.png
+-rw-rw-rw-   0        0        0      338 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/styles/dashdot.png
+-rw-rw-rw-   0        0        0      332 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/styles/dashdotdot.png
+-rw-rw-rw-   0        0        0      328 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/styles/dot.png
+-rw-rw-rw-   0        0        0      328 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/styles/solid.png
+-rw-rw-rw-   0        0        0      401 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/trash.png
+-rw-rw-rw-   0        0        0      407 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/vcursor.png
+-rw-rw-rw-   0        0        0      658 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/vflip.png
+-rw-rw-rw-   0        0        0      375 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/xcursor.png
+-rw-rw-rw-   0        0        0      417 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/images/xrange.png
+-rw-rw-rw-   0        0        0     9529 2021-12-11 14:46:59.000000 guiqwt-4.4.0/guiqwt/interfaces.py
+-rw-rw-rw-   0        0        0    21868 2023-07-06 13:56:01.000000 guiqwt-4.4.0/guiqwt/io.py
+-rw-rw-rw-   0        0        0    20156 2023-07-06 13:50:04.000000 guiqwt-4.4.0/guiqwt/label.py
+drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.414073 guiqwt-4.4.0/guiqwt/locale/
+drwxrwxrwx   0        0        0        0 2023-07-06 17:58:20.927373 guiqwt-4.4.0/guiqwt/locale/fr/
+drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.425824 guiqwt-4.4.0/guiqwt/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0    30153 2023-02-20 09:04:37.000000 guiqwt-4.4.0/guiqwt/locale/fr/LC_MESSAGES/guiqwt.mo
+-rw-rw-rw-   0        0        0    57708 2022-08-01 14:49:33.000000 guiqwt-4.4.0/guiqwt/locale/fr/LC_MESSAGES/guiqwt.po
+-rw-rw-rw-   0        0        0    44618 2023-02-20 09:03:54.000000 guiqwt-4.4.0/guiqwt/locale/guiqwt.pot
+-rw-rw-rw-   0        0        0     3242 2023-07-06 13:50:35.000000 guiqwt-4.4.0/guiqwt/panels.py
+-rw-rw-rw-   0        0        0    48599 2023-07-06 13:50:47.000000 guiqwt-4.4.0/guiqwt/plot.py
+-rw-rw-rw-   0        0        0    19841 2023-02-19 15:02:16.000000 guiqwt-4.4.0/guiqwt/pyplot.py
+-rw-rw-rw-   0        0        0     3361 2021-12-19 11:05:20.000000 guiqwt-4.4.0/guiqwt/qtdesigner.py
+-rw-rw-rw-   0        0        0     5824 2022-04-08 12:35:06.000000 guiqwt-4.4.0/guiqwt/qthelpers.py
+-rw-rw-rw-   0        0        0     1852 2021-12-11 14:47:00.000000 guiqwt-4.4.0/guiqwt/scaler.py
+-rw-rw-rw-   0        0        0    54040 2023-07-06 13:50:11.000000 guiqwt-4.4.0/guiqwt/shapes.py
+-rw-rw-rw-   0        0        0     4530 2023-05-13 07:53:17.000000 guiqwt-4.4.0/guiqwt/signals.py
+-rw-rw-rw-   0        0        0    62787 2022-08-01 14:49:33.000000 guiqwt-4.4.0/guiqwt/styles.py
+drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.614626 guiqwt-4.4.0/guiqwt/tests/
+-rw-rw-rw-   0        0        0      440 2021-12-11 14:47:02.000000 guiqwt-4.4.0/guiqwt/tests/__init__.py
+-rw-rw-rw-   0        0        0     4305 2023-06-10 14:04:27.000000 guiqwt-4.4.0/guiqwt/tests/benchmarks.py
+-rw-rw-rw-   0        0        0    39666 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/tests/brain.png
+-rw-rw-rw-   0        0        0    35354 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/tests/brain_cylinder.png
+-rw-rw-rw-   0        0        0     1374 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/computations.py
+-rw-rw-rw-   0        0        0     1088 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/contrast.py
+-rw-rw-rw-   0        0        0     1164 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/cross_section.py
+-rw-rw-rw-   0        0        0     2021 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/cross_section_oblique.py
+-rw-rw-rw-   0        0        0     1144 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/cursors.py
+-rw-rw-rw-   0        0        0     1742 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/customize_shape_tool.py
+-rw-rw-rw-   0        0        0      977 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/dicom_image.py
+-rw-rw-rw-   0        0        0     6069 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/dotarraydemo.py
+-rw-rw-rw-   0        0        0     2839 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/filtertest1.py
+-rw-rw-rw-   0        0        0     3590 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/filtertest2.py
+-rw-rw-rw-   0        0        0      807 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/fit.py
+-rw-rw-rw-   0        0        0     1153 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/fliprotate.py
+-rw-rw-rw-   0        0        0      401 2023-06-10 14:04:31.000000 guiqwt-4.4.0/guiqwt/tests/fontparam.py
+-rw-rw-rw-   0        0        0     1514 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/get_point.py
+-rw-rw-rw-   0        0        0     1517 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/get_segment.py
+-rw-rw-rw-   0        0        0      801 2023-06-10 14:04:35.000000 guiqwt-4.4.0/guiqwt/tests/highprecisionxy.py
+-rw-rw-rw-   0        0        0     1208 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/hist2d.py
+-rw-rw-rw-   0        0        0     1357 2021-12-11 14:47:02.000000 guiqwt-4.4.0/guiqwt/tests/hist2d_func.py
+-rw-rw-rw-   0        0        0      694 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/histogram.py
+-rw-rw-rw-   0        0        0     3046 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/image.py
+-rw-rw-rw-   0        0        0     1887 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/image_coords.py
+-rw-rw-rw-   0        0        0     1416 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/image_masked.py
+-rw-rw-rw-   0        0        0     1866 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/image_plot_tools.py
+-rw-rw-rw-   0        0        0      954 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/image_rgb.py
+-rw-rw-rw-   0        0        0     1635 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/imagefilter.py
+-rw-rw-rw-   0        0        0     1605 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/imagesuperp.py
+-rw-rw-rw-   0        0        0     1680 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/imagexy.py
+-rw-rw-rw-   0        0        0      879 2023-07-06 13:51:49.000000 guiqwt-4.4.0/guiqwt/tests/loadsaveitems_hdf5.py
+-rw-rw-rw-   0        0        0     1278 2023-07-06 13:51:55.000000 guiqwt-4.4.0/guiqwt/tests/loadsaveitems_json.py
+-rw-rw-rw-   0        0        0     3881 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/loadsaveitems_pickle.py
+-rw-rw-rw-   0        0        0     2710 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/loadtest.py
+-rw-rw-rw-   0        0        0     2402 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/manager.py
+-rw-rw-rw-   0        0        0     2617 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/mandelbrot.py
+-rw-rw-rw-   0        0        0   525620 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/tests/mr-brain.dcm
+-rw-rw-rw-   0        0        0     2660 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/pcolor.py
+-rw-rw-rw-   0        0        0     1802 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/plot.py
+-rw-rw-rw-   0        0        0      908 2023-06-10 14:04:39.000000 guiqwt-4.4.0/guiqwt/tests/plot_log.py
+-rw-rw-rw-   0        0        0    14151 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/plot_timecurve.py
+-rw-rw-rw-   0        0        0      785 2023-06-10 14:04:43.000000 guiqwt-4.4.0/guiqwt/tests/plot_yreverse.py
+-rw-rw-rw-   0        0        0      587 2023-06-10 14:04:47.000000 guiqwt-4.4.0/guiqwt/tests/png_test.py
+-rw-rw-rw-   0        0        0     2195 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/polygons.py
+-rw-rw-rw-   0        0        0     1887 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/pyplot.py
+-rw-rw-rw-   0        0        0     1032 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/qtdesigner.py
+-rw-rw-rw-   0        0        0      993 2021-02-06 17:38:23.000000 guiqwt-4.4.0/guiqwt/tests/qtdesigner.ui
+-rw-rw-rw-   0        0        0      617 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/resize.py
+-rw-rw-rw-   0        0        0     2810 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/rotatecrop.py
+-rw-rw-rw-   0        0        0    54603 2023-07-06 13:52:55.000000 guiqwt-4.4.0/guiqwt/tests/sift.py
+-rw-rw-rw-   0        0        0     3757 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/simple_dialog.py
+-rw-rw-rw-   0        0        0     9236 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/simple_window.py
+-rw-rw-rw-   0        0        0     2895 2023-06-10 14:04:54.000000 guiqwt-4.4.0/guiqwt/tests/styles.py
+-rw-rw-rw-   0        0        0     4809 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/syncplot.py
+-rw-rw-rw-   0        0        0     1280 2023-06-10 14:05:01.000000 guiqwt-4.4.0/guiqwt/tests/test_line.py
+-rw-rw-rw-   0        0        0     5352 2023-06-10 14:05:30.000000 guiqwt-4.4.0/guiqwt/tests/transform.py
+-rw-rw-rw-   0        0        0    88336 2023-06-10 14:03:47.000000 guiqwt-4.4.0/guiqwt/tools.py
+-rw-rw-rw-   0        0        0      749 2021-12-11 14:47:03.000000 guiqwt-4.4.0/guiqwt/transitional.py
+drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.632626 guiqwt-4.4.0/guiqwt/widgets/
+-rw-rw-rw-   0        0        0      578 2019-10-08 16:03:22.000000 guiqwt-4.4.0/guiqwt/widgets/__init__.py
+-rw-rw-rw-   0        0        0     8406 2021-12-11 14:47:03.000000 guiqwt-4.4.0/guiqwt/widgets/base.py
+-rw-rw-rw-   0        0        0    24376 2023-06-10 14:03:47.000000 guiqwt-4.4.0/guiqwt/widgets/fit.py
+-rw-rw-rw-   0        0        0     5169 2022-08-01 14:49:33.000000 guiqwt-4.4.0/guiqwt/widgets/fliprotate.py
+-rw-rw-rw-   0        0        0     5064 2021-12-19 10:53:14.000000 guiqwt-4.4.0/guiqwt/widgets/resizedialog.py
+-rw-rw-rw-   0        0        0     4550 2021-12-11 14:47:04.000000 guiqwt-4.4.0/guiqwt/widgets/rotatecrop.py
+drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.127963 guiqwt-4.4.0/guiqwt.egg-info/
+-rw-rw-rw-   0        0        0     2640 2023-07-06 17:58:20.000000 guiqwt-4.4.0/guiqwt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8112 2023-07-06 17:58:20.000000 guiqwt-4.4.0/guiqwt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 17:58:20.000000 guiqwt-4.4.0/guiqwt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-07-06 17:58:20.000000 guiqwt-4.4.0/guiqwt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      111 2023-07-06 17:58:20.000000 guiqwt-4.4.0/guiqwt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-06 17:58:20.000000 guiqwt-4.4.0/guiqwt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      112 2022-08-01 14:49:33.000000 guiqwt-4.4.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.636625 guiqwt-4.4.0/qtdesigner/
+-rw-rw-rw-   0        0        0      446 2019-10-08 16:03:22.000000 guiqwt-4.4.0/qtdesigner/imageplotplugin.py
+-rw-rw-rw-   0        0        0      435 2019-10-08 16:03:22.000000 guiqwt-4.4.0/qtdesigner/plotplugin.py
+-rw-rw-rw-   0        0        0       42 2023-07-06 17:58:21.663087 guiqwt-4.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     9569 2023-07-06 13:46:26.000000 guiqwt-4.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.642637 guiqwt-4.4.0/sift/
+-rw-rw-rw-   0        0        0     1136 2023-07-06 13:57:01.000000 guiqwt-4.4.0/sift/create_exe.py
+-rw-rw-rw-   0        0        0   100952 2019-10-08 16:03:22.000000 guiqwt-4.4.0/sift/sift.ico
+-rw-rw-rw-   0        0        0       64 2019-10-08 16:03:22.000000 guiqwt-4.4.0/sift/sift.pyw
+drwxrwxrwx   0        0        0        0 2023-07-06 17:58:21.663087 guiqwt-4.4.0/src/
+-rw-rw-rw-   0        0        0     4647 2019-10-08 16:03:22.000000 guiqwt-4.4.0/src/arrays.hpp
+-rw-rw-rw-   0        0        0      681 2019-10-08 16:03:22.000000 guiqwt-4.4.0/src/debug.hpp
+-rw-rw-rw-   0        0        0   298411 2023-07-06 17:58:03.000000 guiqwt-4.4.0/src/histogram2d.c
+-rw-rw-rw-   0        0        0     3434 2019-10-08 16:03:22.000000 guiqwt-4.4.0/src/histogram2d.pyx
+-rw-rw-rw-   0        0        0   235857 2023-07-06 17:58:03.000000 guiqwt-4.4.0/src/mandelbrot.c
+-rw-rw-rw-   0        0        0     1168 2019-10-08 16:03:22.000000 guiqwt-4.4.0/src/mandelbrot.pyx
+-rw-rw-rw-   0        0        0    11581 2021-02-06 17:38:23.000000 guiqwt-4.4.0/src/pcolor.cpp
+-rw-rw-rw-   0        0        0     6127 2019-10-08 16:03:22.000000 guiqwt-4.4.0/src/points.hpp
+-rw-rw-rw-   0        0        0    22897 2021-02-06 17:38:23.000000 guiqwt-4.4.0/src/scaler.cpp
+-rw-rw-rw-   0        0        0     2376 2019-10-08 16:03:22.000000 guiqwt-4.4.0/src/scaler.hpp
+-rw-rw-rw-   0        0        0     4137 2022-08-01 14:49:33.000000 guiqwt-4.4.0/src/traits.hpp
```

### Comparing `guiqwt-4.3.3/CHANGELOG.md` & `guiqwt-4.4.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,30 @@
 # guiqwt Releases #
 
+## Version 4.4.0 ##
+
+Changes:
+
+* guiqwt now requires guidata >=v3.0.
+* tests/syncplot: added image synchronization test
+
+Bug fixes:
+
+* [Issue #107](https://github.com/PierreRaybaut/guiqwt/issues/107) - App with multiple ImageWidgets seg faults about 40+% of the time on startup
+* [Issue #104](https://github.com/PierreRaybaut/guiqwt/issues/104) - TrImageItem will emit a signal when the image is moved but not when resized
+* [Pull Request #103](https://github.com/PierreRaybaut/guiqwt/pull/103) - use np.isnan() to handle if image data contains nan values, by [@RussBerg](https://github.com/RussBerg)
+* [Issue #102](https://github.com/PierreRaybaut/guiqwt/issues/102) - image.py: get_histogram() will fail if image initialized with Nan values
+* [Pull Request #101](https://github.com/PierreRaybaut/guiqwt/pull/101) - corrected arguments names for specifying image center, by [@RussBerg](https://github.com/RussBerg)
+* [Issue #100](https://github.com/PierreRaybaut/guiqwt/issues/100) - Images: changing X-axis direction does not work with autoscale
+* [Issue #99](https://github.com/PierreRaybaut/guiqwt/issues/99) - trimage builder specifies wrong attributes for altering image center
+* [Issue #98](https://github.com/PierreRaybaut/guiqwt/issues/98) - numpy >= 1.20 incompatibilities
+* [Issue #90](https://github.com/PierreRaybaut/guiqwt/issues/90) -  Image visualization: should first pixel be centered at (0,0)
+* Fixed coords inversion in EllipseShape (circle)
+* tests/syncplot: fixed plot rescaling at initialization
+
 ## Version 4.3.3 ##
 
 Bug fixes:
 
 * Fixed Issue #90 / ImageItem's pixels are now centered on their coordinates
 * plot.SubplotWidget w/image related panels: simplify both pyplot and
   syncplot.py test
```

### Comparing `guiqwt-4.3.3/Licence_CeCILL_V2-en.txt` & `guiqwt-4.4.0/Licence_CeCILL_V2-en.txt`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/PKG-INFO` & `guiqwt-4.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: guiqwt
-Version: 4.3.3
+Version: 4.4.0
 Summary: guiqwt is a set of tools for curve and image plotting (extension to PythonQwt)
 Home-page: https://github.com/PierreRaybaut/guiqwt
 Author: Pierre Raybaut
 Author-email: pierre.raybaut@gmail.com
 License: CeCILL V2
-Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
@@ -65,9 +64,7 @@
 .. _NumPy: https://pypi.python.org/pypi/NumPy
 .. _SciPy: https://pypi.python.org/pypi/SciPy
 .. _Pillow: https://pypi.python.org/pypi/Pillow
 
 See the `README`_ and `documentation`_ for more details.
 
 .. _README: https://github.com/PierreRaybaut/guiqwt/blob/master/README.md
-
-
```

### Comparing `guiqwt-4.3.3/README.md` & `guiqwt-4.4.0/README.md`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/_static/favicon.ico` & `guiqwt-4.4.0/doc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/conf.py` & `guiqwt-4.4.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/development.rst` & `guiqwt-4.4.0/doc/development.rst`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/disthelpers.rst` & `guiqwt-4.4.0/doc/disthelpers.rst`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 like `py2exe` or `cx_Freeze`. These tools work as extensions to Python builtin
 `distutils` module and converts Python scripts into executable Windows
 programs which may be executed without requiring a Python installation.
 
 Making such an executable program may be a non trivial task when the script
 dependencies include libraries with data or extensions, such as `PyQt5` or
 `guidata` and `guiqwt`. This task has been considerably simplified thanks to
-the helper functions provided by :py:mod:`guidata.disthelpers`.
+the helper functions provided by :py:mod:`guidata.utils.disthelpers`.
 
 Example
 ~~~~~~~
 
 This example is included in `guiqwt` source package (see the
 ``deployment_example`` folder at source package root directory).
```

### Comparing `guiqwt-4.3.3/doc/images/curve_widgets.png` & `guiqwt-4.4.0/doc/images/curve_widgets.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/images/guiqwt.png` & `guiqwt-4.4.0/doc/images/guiqwt.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/images/image_widgets.png` & `guiqwt-4.4.0/doc/images/image_widgets.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/images/my_plot_manager.png` & `guiqwt-4.4.0/doc/images/my_plot_manager.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/images/panorama.png` & `guiqwt-4.4.0/doc/images/panorama.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/images/screenshots/__init__.png` & `guiqwt-4.4.0/doc/images/screenshots/__init__.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/images/screenshots/computations.png` & `guiqwt-4.4.0/doc/images/screenshots/computations.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/images/screenshots/contrast.png` & `guiqwt-4.4.0/doc/images/screenshots/contrast.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/images/screenshots/cross_section.png` & `guiqwt-4.4.0/doc/images/screenshots/cross_section.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/images/screenshots/cross_section2.png` & `guiqwt-4.4.0/doc/images/screenshots/cross_section2.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/images/screenshots/dotarraydemo.png` & `guiqwt-4.4.0/doc/images/screenshots/dotarraydemo.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/images/screenshots/fit.png` & `guiqwt-4.4.0/doc/images/screenshots/fit.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/images/screenshots/get_point.png` & `guiqwt-4.4.0/doc/images/screenshots/get_point.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/images/screenshots/hist2d.png` & `guiqwt-4.4.0/doc/images/screenshots/hist2d.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/images/screenshots/image_plot_tools.png` & `guiqwt-4.4.0/doc/images/screenshots/image_plot_tools.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/images/screenshots/imagefilter.png` & `guiqwt-4.4.0/doc/images/screenshots/imagefilter.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/images/screenshots/imagesuperp.png` & `guiqwt-4.4.0/doc/images/screenshots/imagesuperp.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/images/screenshots/imagexy.png` & `guiqwt-4.4.0/doc/images/screenshots/imagexy.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/images/screenshots/manager.png` & `guiqwt-4.4.0/doc/images/screenshots/manager.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/images/screenshots/mandelbrot.png` & `guiqwt-4.4.0/doc/images/screenshots/mandelbrot.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/images/screenshots/pcolor.png` & `guiqwt-4.4.0/doc/images/screenshots/pcolor.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/images/screenshots/plot.png` & `guiqwt-4.4.0/doc/images/screenshots/plot.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/images/screenshots/sift1.png` & `guiqwt-4.4.0/doc/images/screenshots/sift1.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/images/screenshots/sift2.png` & `guiqwt-4.4.0/doc/images/screenshots/sift2.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/images/screenshots/sift3.png` & `guiqwt-4.4.0/doc/images/screenshots/sift3.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/images/screenshots/simple_dialog.png` & `guiqwt-4.4.0/doc/images/screenshots/simple_dialog.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/images/screenshots/simple_window.png` & `guiqwt-4.4.0/doc/images/screenshots/simple_window.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/images/screenshots/transform.png` & `guiqwt-4.4.0/doc/images/screenshots/transform.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/index.rst` & `guiqwt-4.4.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/installation.rst` & `guiqwt-4.4.0/doc/installation.rst`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Dependencies
 ------------
 
 Requirements:
     * Python 3.x (x>=7)
     * `PyQt5`_ 5.x (x>=5)
     * `PythonQwt`_ >=0.10
-    * `guidata`_ >=2.3
+    * `guidata`_ >=3.0
     * `QtPy`_ >= 1.3
     * `NumPy`_, `SciPy`_ and `Pillow`_
 
 Optional Python modules:
     * `pydicom`_ >=0.9.3 for DICOM files I/O features
 
 .. _PyQt5: https://pypi.python.org/pypi/PyQt5
```

### Comparing `guiqwt-4.3.3/doc/migrating_from_v2_to_v3.rst` & `guiqwt-4.4.0/doc/migrating_from_v2_to_v3.rst`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/overview.rst` & `guiqwt-4.4.0/doc/overview.rst`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/doc/sift.rst` & `guiqwt-4.4.0/doc/sift.rst`

 * *Files 12% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 counterpart, `Sift` is quite limited in its current implementation. For now,
 its main purpose is to show how to create easily and rapidly your own
 signal/image processing application using ``guidata`` and ``guiqwt``.
 
 .. image:: images/screenshots/sift2.png
 
 .. literalinclude:: ../guiqwt/tests/sift.py
-   :start-after: SHOW
+   :start-after: guitest: show
    :end-before: Workaround for Sphinx v0.6 bug: empty 'end-before' directive
```

### Comparing `guiqwt-4.3.3/guiqwt/__init__.py` & `guiqwt-4.4.0/guiqwt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 .. _PyPI: https://pypi.python.org/pypi/guiqwt
 .. _GitHub: https://github.com/PierreRaybaut/guiqwt
 .. _GoogleGroup: http://groups.google.fr/group/guidata_guiqwt
 """
 
 
-__version__ = "4.3.3"  # Update here *AND* in setup.py!
+__version__ = "4.4.0"  # Update here *AND* in setup.py!
 # (Until setup.py has been fully retrofitted, this manual sync is mandatory)
 
 
 def about(html=True, copyright_only=False):
     """Return text about this package"""
     import sys, os, os.path as osp, platform, guidata, guiqwt, qwt
     from guiqwt.config import _
```

### Comparing `guiqwt-4.3.3/guiqwt/_cm.py` & `guiqwt-4.4.0/guiqwt/_cm.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/annotations.py` & `guiqwt-4.4.0/guiqwt/annotations.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,37 +65,38 @@
    :inherited-members:
 .. autoclass:: AnnotatedCircle
    :members:
    :inherited-members:
 """
 
 import numpy as np
+from guidata.utils import update_dataset
+from guidata.utils.misc import assert_interfaces_valid
 
-from guidata.utils import update_dataset, assert_interfaces_valid
+from guiqwt.baseplot import canvas_to_axes
 
 # Local imports
 from guiqwt.config import CONF, _
-from guiqwt.styles import LabelParam, AnnotationParam
+from guiqwt.geometry import (
+    compute_angle,
+    compute_center,
+    compute_distance,
+    compute_rect_size,
+)
+from guiqwt.interfaces import IBasePlotItem, ISerializableType, IShapeItemType
+from guiqwt.label import DataInfoLabel
 from guiqwt.shapes import (
     AbstractShape,
-    RectangleShape,
     EllipseShape,
-    SegmentShape,
-    PointShape,
     ObliqueRectangleShape,
+    PointShape,
+    RectangleShape,
+    SegmentShape,
 )
-from guiqwt.label import DataInfoLabel
-from guiqwt.interfaces import IBasePlotItem, IShapeItemType, ISerializableType
-from guiqwt.geometry import (
-    compute_center,
-    compute_rect_size,
-    compute_distance,
-    compute_angle,
-)
-from guiqwt.baseplot import canvas_to_axes
+from guiqwt.styles import AnnotationParam, LabelParam
 
 
 class AnnotatedShape(AbstractShape):
     """
     Construct an annotated shape with properties set with
     *annotationparam* (see :py:class:`guiqwt.styles.AnnotationParam`)
     """
@@ -573,14 +574,15 @@
 
     SHAPE_CLASS = EllipseShape
     LABEL_ANCHOR = "C"
 
     def __init__(self, x1=0, y1=0, x2=0, y2=0, annotationparam=None):
         AnnotatedShape.__init__(self, annotationparam)
         self.set_xdiameter(x1, y1, x2, y2)
+        self.shape.switch_to_ellipse()
 
     # ----Public API-------------------------------------------------------------
     def set_xdiameter(self, x0, y0, x1, y1):
         """Set the coordinates of the ellipse's X-axis diameter
         Warning: transform matrix is not applied here"""
         self.shape.set_xdiameter(x0, y0, x1, y1)
         self.set_label_position()
@@ -651,14 +653,15 @@
     Construct an annotated circle with diameter between coordinates
     (x1, y1) and (x2, y2) and properties set with *annotationparam*
     (see :py:class:`guiqwt.styles.AnnotationParam`)
     """
 
     def __init__(self, x1=0, y1=0, x2=0, y2=0, annotationparam=None):
         AnnotatedEllipse.__init__(self, x1, y1, x2, y2, annotationparam)
+        self.shape.switch_to_circle()
 
     def get_tr_diameter(self):
         """Return circle diameter after applying transform matrix"""
         return compute_distance(*self.get_transformed_coords(0, 1))
 
     # ----AnnotatedShape API-------------------------------------------------
     def get_infos(self):
```

### Comparing `guiqwt-4.3.3/guiqwt/baseplot.py` & `guiqwt-4.4.0/guiqwt/baseplot.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,14 +122,17 @@
     AXIS_CONF_OPTIONS = ("axis", "axis", "axis", "axis")
     DEFAULT_ACTIVE_XAXIS = X_BOTTOM
     DEFAULT_ACTIVE_YAXIS = Y_LEFT
 
     #: Signal emitted by plot when an IBasePlotItem object was moved (args: x0, y0, x1, y1)
     SIG_ITEM_MOVED = Signal(object, float, float, float, float)
 
+    #: Signal emitted by plot when an IBasePlotItem handle was moved
+    SIG_ITEM_HANDLE_MOVED = Signal(object)
+
     #: Signal emitted by plot when a shapes.Marker position changes
     SIG_MARKER_CHANGED = Signal(object)
 
     #: Signal emitted by plot when a shapes.Axes position (or the angle) changes
     SIG_AXES_CHANGED = Signal(object)
 
     #: Signal emitted by plot when an annotation.AnnotatedShape position changes
@@ -605,30 +608,30 @@
         items = pickle.load(iofile)
         for item in items:
             self.add_item(item)
 
     def serialize(self, writer, selected=False):
         """
         Save (serializable) items to HDF5 file:
-            * writer: :py:class:`guidata.hdf5io.HDF5Writer` object
+            * writer: :py:class:`guidata.dataset.hdf5io.HDF5Writer` object
             * selected=False: if True, will save only selected items
 
         See also :py:meth:`guiqwt.baseplot.BasePlot.restore_items_from_hdf5`
         """
         if selected:
             items = self.get_selected_items()
         else:
             items = self.items[:]
         items = [item for item in items if ISerializableType in item.types()]
         io.save_items(writer, items)
 
     def deserialize(self, reader):
         """
         Restore items from HDF5 file:
-            * reader: :py:class:`guidata.hdf5io.HDF5Reader` object
+            * reader: :py:class:`guidata.dataset.hdf5io.HDF5Reader` object
 
         See also :py:meth:`guiqwt.baseplot.BasePlot.save_items_to_hdf5`
         """
         for item in io.load_items(reader):
             self.add_item(item)
 
     def set_items(self, *args):
```

### Comparing `guiqwt-4.3.3/guiqwt/builder.py` & `guiqwt-4.4.0/guiqwt/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,70 +53,77 @@
 ~~~~~~~~~
 
 .. autoclass:: PlotItemBuilder
    :members:
 """
 
 import os.path as osp
-from numpy import arange, array, zeros, meshgrid, ndarray
 
-# Local imports
-from guiqwt.config import _, CONF, make_title
+from numpy import arange, array, meshgrid, ndarray, zeros
+
+from guiqwt.annotations import (
+    AnnotatedCircle,
+    AnnotatedEllipse,
+    AnnotatedRectangle,
+    AnnotatedSegment,
+)
 from guiqwt.baseplot import BasePlot
+
+# Local imports
+from guiqwt.config import CONF, _, make_title
 from guiqwt.curve import CurveItem, ErrorBarCurveItem, GridItem
 from guiqwt.histogram import HistogramItem, lut_range_threshold
 from guiqwt.image import (
+    Histogram2DItem,
     ImageItem,
+    MaskedImageItem,
     QuadGridItem,
+    RGBImageItem,
     TrImageItem,
     XYImageItem,
-    Histogram2DItem,
-    RGBImageItem,
-    MaskedImageItem,
+)
+from guiqwt.label import (
+    DataInfoLabel,
+    LabelItem,
+    LegendBoxItem,
+    RangeComputation,
+    RangeComputation2d,
+    RangeInfo,
+    SelectedLegendBoxItem,
 )
 from guiqwt.shapes import (
-    XRangeSelection,
-    RectangleShape,
     EllipseShape,
-    SegmentShape,
     Marker,
+    RectangleShape,
+    SegmentShape,
+    XRangeSelection,
 )
-from guiqwt.annotations import AnnotatedRectangle, AnnotatedEllipse, AnnotatedSegment
 from guiqwt.styles import (
-    update_style_attr,
+    COLORS,
+    MARKERS,
+    AnnotationParam,
     CurveParam,
     ErrorBarParam,
-    style_generator,
-    LabelParam,
-    LegendParam,
-    ImageParam,
-    TrImageParam,
-    HistogramParam,
+    GridParam,
     Histogram2DParam,
-    RGBImageParam,
-    MaskedImageParam,
-    XYImageParam,
+    HistogramParam,
     ImageFilterParam,
-    MARKERS,
-    COLORS,
-    GridParam,
-    LineStyleParam,
-    AnnotationParam,
-    QuadGridParam,
+    ImageParam,
+    LabelParam,
     LabelParamWithContents,
+    LegendParam,
+    LineStyleParam,
     MarkerParam,
-)
-from guiqwt.label import (
-    LabelItem,
-    LegendBoxItem,
-    RangeComputation,
-    RangeComputation2d,
-    DataInfoLabel,
-    RangeInfo,
-    SelectedLegendBoxItem,
+    MaskedImageParam,
+    QuadGridParam,
+    RGBImageParam,
+    TrImageParam,
+    XYImageParam,
+    style_generator,
+    update_style_attr,
 )
 
 # default offset positions for anchors
 ANCHOR_OFFSETS = {
     "TL": (5, 5),
     "TR": (-5, 5),
     "BL": (5, -5),
@@ -1008,16 +1015,16 @@
             param,
             title,
             alpha_mask,
             alpha,
             interpolation,
             background=background_color,
             colormap=colormap,
-            x0=x0,
-            y0=y0,
+            pos_x0=x0,
+            pos_y0=y0,
             angle=angle,
             dx=dx,
             dy=dy,
             xformat=xformat,
             yformat=yformat,
             zformat=zformat,
         )
@@ -1367,37 +1374,39 @@
         (:py:class:`guiqwt.shapes.RectangleShape` object)
 
             * x0, y0, x1, y1: rectangle coordinates
             * title: label name (optional)
         """
         return self.__shape(RectangleShape, x0, y0, x1, y1, title)
 
-    def ellipse(self, x0, y0, x1, y1, title=None):
+    def ellipse(self, x0, y0, x1, y1, x2=None, y2=None, x3=None, y3=None, title=None):
         """
         Make an ellipse shape `plot item`
         (:py:class:`guiqwt.shapes.EllipseShape` object)
 
-            * x0, y0, x1, y1: ellipse x-axis coordinates
+            * x0, y0, x1, y1, x2, y2, x3, y3: ellipse coordinates
             * title: label name (optional)
         """
-        shape = EllipseShape(x0, y0, x1, y1)
-        shape.set_style("plot", "shape/drag")
-        if title is not None:
-            shape.setTitle(title)
-        return shape
+        item = self.__shape(EllipseShape, x0, y0, x1, y1, title)
+        item.switch_to_ellipse()
+        if x2 is not None and y2 is not None and x3 is not None and y3 is not None:
+            item.set_ydiameter(x2, y2, x3, y3)
+        return item
 
     def circle(self, x0, y0, x1, y1, title=None):
         """
         Make a circle shape `plot item`
         (:py:class:`guiqwt.shapes.EllipseShape` object)
 
             * x0, y0, x1, y1: circle diameter coordinates
             * title: label name (optional)
         """
-        return self.ellipse(x0, y0, x1, y1, title=title)
+        item = self.__shape(EllipseShape, x0, y0, x1, y1, title)
+        item.switch_to_circle()
+        return item
 
     def segment(self, x0, y0, x1, y1, title=None):
         """
         Make a segment shape `plot item`
         (:py:class:`guiqwt.shapes.SegmentShape` object)
 
             * x0, y0, x1, y1: segment coordinates
@@ -1427,36 +1436,48 @@
             * x0, y0, x1, y1: rectangle coordinates
             * title, subtitle: strings
         """
         return self.__annotated_shape(
             AnnotatedRectangle, x0, y0, x1, y1, title, subtitle
         )
 
-    def annotated_ellipse(self, x0, y0, x1, y1, title=None, subtitle=None):
+    def annotated_ellipse(
+        self,
+        x0,
+        y0,
+        x1,
+        y1,
+        x2=None,
+        y2=None,
+        x3=None,
+        y3=None,
+        title=None,
+        subtitle=None,
+    ):
         """
         Make an annotated ellipse `plot item`
         (:py:class:`guiqwt.annotations.AnnotatedEllipse` object)
 
-            * x0, y0, x1, y1: ellipse rectangle coordinates
+            * x0, y0, x1, y1, x2, y2, x3, y3: ellipse coordinates
             * title, subtitle: strings
         """
-        param = self.__get_annotationparam(title, subtitle)
-        shape = AnnotatedEllipse(x0, y0, x1, y1, param)
-        shape.set_style("plot", "shape/drag")
-        return shape
+        item = self.__annotated_shape(AnnotatedEllipse, x0, y0, x1, y1, title, subtitle)
+        if x2 is not None and y2 is not None and x3 is not None and y3 is not None:
+            item.set_ydiameter(x2, y2, x3, y3)
+        return item
 
     def annotated_circle(self, x0, y0, x1, y1, title=None, subtitle=None):
         """
         Make an annotated circle `plot item`
         (:py:class:`guiqwt.annotations.AnnotatedCircle` object)
 
             * x0, y0, x1, y1: circle diameter coordinates
             * title, subtitle: strings
         """
-        return self.annotated_ellipse(x0, y0, x1, y1, title, subtitle)
+        return self.__annotated_shape(AnnotatedCircle, x0, y0, x1, y1, title, subtitle)
 
     def annotated_segment(self, x0, y0, x1, y1, title=None, subtitle=None):
         """
         Make an annotated segment `plot item`
         (:py:class:`guiqwt.annotations.AnnotatedSegment` object)
 
             * x0, y0, x1, y1: segment coordinates
```

### Comparing `guiqwt-4.3.3/guiqwt/colormap.py` & `guiqwt-4.4.0/guiqwt/colormap.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/config.py` & `guiqwt-4.4.0/guiqwt/config.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/cross_section.py` & `guiqwt-4.4.0/guiqwt/cross_section.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 import weakref
 
 from qtpy.QtWidgets import QVBoxLayout, QSizePolicy, QHBoxLayout, QToolBar, QSpacerItem
 from qtpy.QtCore import QSize, QPointF, Qt
 
 import numpy as np
 
-from guidata.utils import assert_interfaces_valid
+from guidata.utils.misc import assert_interfaces_valid
 from guidata.configtools import get_icon
 from guidata.qthelpers import create_action, add_actions
 
 # Local imports
 from guiqwt.config import CONF, _
 from guiqwt.interfaces import ICSImageItemType, IPanel, IBasePlotItem
 from guiqwt.panels import PanelWidget, ID_XCS, ID_YCS, ID_OCS
```

### Comparing `guiqwt-4.3.3/guiqwt/curve.py` & `guiqwt-4.4.0/guiqwt/curve.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,16 @@
     QVBoxLayout,
     QToolBar,
     QMessageBox,
 )
 from qtpy.QtGui import QBrush, QColor, QPen, QPolygonF
 from qtpy.QtCore import Qt, QPointF, QLineF, QRectF, Signal
 
-from guidata.utils import assert_interfaces_valid, update_dataset
+from guidata.utils.misc import assert_interfaces_valid
+from guidata.utils import update_dataset
 from guidata.configtools import get_icon, get_image_layout
 from guidata.qthelpers import create_action, add_actions
 
 # Local imports
 from guiqwt.transitional import QwtPlotCurve, QwtPlotGrid, QwtPlotItem, QwtScaleMap
 from guiqwt.config import CONF, _
 from guiqwt.interfaces import (
```

### Comparing `guiqwt-4.3.3/guiqwt/debug.py` & `guiqwt-4.4.0/guiqwt/debug.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/events.py` & `guiqwt-4.4.0/guiqwt/events.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/geometry.py` & `guiqwt-4.4.0/guiqwt/geometry.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/histogram.py` & `guiqwt-4.4.0/guiqwt/histogram.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,16 @@
 import weakref
 import numpy as np
 from qtpy.QtCore import Qt, Signal
 from qtpy.QtWidgets import QHBoxLayout, QVBoxLayout, QToolBar
 
 from guidata.dataset.datatypes import DataSet
 from guidata.dataset.dataitems import FloatItem
-from guidata.utils import assert_interfaces_valid, update_dataset
+from guidata.utils.misc import assert_interfaces_valid
+from guidata.utils import update_dataset
 from guidata.configtools import get_icon, get_image_layout
 from guidata.qthelpers import add_actions, create_action
 
 # Local imports
 from guiqwt.transitional import QwtPlotCurve
 from guiqwt.config import CONF, _
 from guiqwt.interfaces import IBasePlotItem, IHistDataSource, IVoiImageItemType, IPanel
```

### Comparing `guiqwt-4.3.3/guiqwt/image.py` & `guiqwt-4.4.0/guiqwt/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,16 @@
 from math import fabs
 
 import numpy as np
 
 from qtpy.QtGui import QColor, QImage
 from qtpy.QtCore import QRectF, QPointF, QRect
 
-from guidata.utils import assert_interfaces_valid, update_dataset
+from guidata.utils.misc import assert_interfaces_valid
+from guidata.utils import update_dataset
 
 # Local imports
 from guiqwt.transitional import QwtPlotItem, QwtInterval
 from guiqwt.config import _
 from guiqwt.interfaces import (
     IBasePlotItem,
     IBaseImageItem,
@@ -736,36 +737,31 @@
     def get_histogram(self, nbins):
         """interface de IHistDataSource"""
         if self.data is None:
             return [
                 0,
             ], [0, 1]
         if self.histogram_cache is None or nbins != self.histogram_cache[0].shape[0]:
-            # from guidata.utils import tic, toc
             if True:
-                # tic("histo1")
-                res = np.histogram(self.data, nbins)
-                # toc("histo1")
+                res = np.histogram(self.data[~np.isnan(self.data)], nbins)
             else:
                 # TODO: _histogram is faster, but caching is buggy
                 # in this version
-                # tic("histo2")
                 _min = _nanmin(self.data)
                 _max = _nanmax(self.data)
                 if self.data.dtype in (np.float64, np.float32):
                     bins = np.unique(
                         np.array(
                             np.linspace(_min, _max, nbins + 1), dtype=self.data.dtype
                         )
                     )
                 else:
                     bins = np.arange(_min, _max + 2, dtype=self.data.dtype)
                 res2 = np.zeros((bins.size + 1,), np.uint32)
                 _histogram(self.data.flatten(), bins, res2)
-                # toc("histo2")
                 res = res2[1:-1], bins
             self.histogram_cache = res
         else:
             res = self.histogram_cache
         return res
 
     def __process_cross_section(self, ydata, apply_lut):
@@ -1060,36 +1056,38 @@
         super(ImageItem, self).deserialize(reader)
         for attr in ("xmin", "xmax", "ymin", "ymax"):
             # Note: do not be tempted to write the symetric code in `serialize`
             # because calling `get_xdata` and `get_ydata` is necessary
             setattr(self, attr, reader.read(attr, func=reader.read_float))
 
     # ---- Public API ----------------------------------------------------------
-    def get_xdata(self):
+    def get_xdata(self, aligned=True):
         """Return (xmin, xmax)"""
         xmin, xmax = self.xmin, self.xmax
         if xmin is None:
             xmin = 0.0
         if xmax is None:
             xmax = self.data.shape[1]
-        dx = 0.5 * (xmax - xmin) / self.data.shape[1]
-        xmin -= dx
-        xmax -= dx
+        if aligned:
+            dx = 0.5 * (xmax - xmin) / self.data.shape[1]
+            xmin -= dx
+            xmax -= dx
         return xmin, xmax
 
-    def get_ydata(self):
+    def get_ydata(self, aligned=True):
         """Return (ymin, ymax)"""
         ymin, ymax = self.ymin, self.ymax
         if ymin is None:
             ymin = 0.0
         if ymax is None:
             ymax = self.data.shape[0]
-        dy = 0.5 * (ymax - ymin) / self.data.shape[0]
-        ymin -= dy
-        ymax -= dy
+        if aligned:
+            dy = 0.5 * (ymax - ymin) / self.data.shape[0]
+            ymin -= dy
+            ymax -= dy
         return ymin, ymax
 
     def set_xdata(self, xmin=None, xmax=None):
         self.xmin, self.xmax = xmin, xmax
 
     def set_ydata(self, ymin=None, ymax=None):
         self.ymin, self.ymax = ymin, ymax
@@ -1123,15 +1121,16 @@
     def get_y_values(self, j0, j1):
         ymin, ymax = self.get_ydata()
         yfunc = lambda index: ymin + (ymax - ymin) * index / float(self.data.shape[0])
         return np.linspace(yfunc(j0), yfunc(j1), j1 - j0)
 
     def get_closest_coordinates(self, x, y):
         """Return closest image pixel coordinates"""
-        (xmin, xmax), (ymin, ymax) = self.get_xdata(), self.get_ydata()
+        xmin, xmax = self.get_xdata(aligned=False)
+        ymin, ymax = self.get_ydata(aligned=False)
         i, j = self.get_closest_indexes(x, y)
         xpix = np.linspace(xmin, xmax, self.data.shape[1] + 1)
         ypix = np.linspace(ymin, ymax, self.data.shape[0] + 1)
         return xpix[i], ypix[j]
 
     def _rescale_src_rect(self, src_rect):
         sxl, syt, sxr, syb = src_rect
@@ -1501,14 +1500,16 @@
             angle += a1 - a0
         if self.can_resize():
             # compute pixel size
             zoom = np.linalg.norm(vec1) / np.linalg.norm(vec0)
             dx = zoom * dx
             dy = zoom * dy
         self.set_transform(x0, y0, angle, dx, dy, hflip, vflip)
+        if self.plot():
+            self.plot().SIG_ITEM_HANDLE_MOVED.emit(self)
 
     def move_local_shape(self, old_pos, new_pos):
         """Translate the shape such that old_pos becomes new_pos
         in canvas coordinates"""
         x0, y0, angle, dx, dy, hflip, vflip = self.get_transform()
         nx, ny = canvas_to_axes(self, new_pos)
         ox, oy = canvas_to_axes(self, old_pos)
@@ -2226,15 +2227,15 @@
         If inside is True (default), mask the inside of the area
         Otherwise, mask the outside
         """
         ix0, iy0, ix1, iy1 = self.get_closest_index_rect(x0, y0, x1, y1)
         if inside:
             self.data[iy0:iy1, ix0:ix1] = np.ma.masked
         else:
-            indexes = np.ones(self.data.shape, dtype=np.bool)
+            indexes = np.ones(self.data.shape, dtype=bool)
             indexes[iy0:iy1, ix0:ix1] = False
             self.data[indexes] = np.ma.masked
         if trace:
             self.add_masked_area("rectangular", x0, y0, x1, y1, inside)
         if do_signal:
             self._mask_changed()
 
@@ -2399,14 +2400,16 @@
         BaseImageItem.set_item_parameters(self, itemparams)
 
     def move_local_point_to(self, handle, pos, ctrl=None):
         """Move a handle as returned by hit_test to the new position pos
         ctrl: True if <Ctrl> button is being pressed, False otherwise"""
         npos = canvas_to_axes(self, pos)
         self.border_rect.move_point_to(handle, npos)
+        if self.plot():
+            self.plot().SIG_ITEM_HANDLE_MOVED.emit(self)
 
     def move_local_shape(self, old_pos, new_pos):
         """Translate the shape such that old_pos becomes new_pos
         in canvas coordinates"""
         old_pt = canvas_to_axes(self, old_pos)
         new_pt = canvas_to_axes(self, new_pos)
         self.border_rect.move_shape(old_pt, new_pt)
@@ -2813,14 +2816,16 @@
         ymap = self.canvasMap(self.Y_LEFT)
         xmap = self.canvasMap(self.X_BOTTOM)
         h = ymap.pDist()
         w = xmap.pDist()
         dx1, dy1 = xmap.sDist(), fabs(ymap.sDist())
         x0, y0 = xmap.s1(), ymap.s1()
         x1, y1 = xmap.s2(), ymap.s2()
+        if x0 > x1:
+            x0, x1 = x1, x0
         if y0 > y1:
             y0, y1 = y1, y0
         if full_scale:
             if w == 0:
                 return  # avoid division by zero
             dy2 = (h * dx1) / (w * self.__aspect_ratio)
             fix_yaxis = dy2 > dy1
```

### Comparing `guiqwt-4.3.3/guiqwt/images/arrow_down.png` & `guiqwt-4.4.0/guiqwt/images/arrow_down.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/arrow_up.png` & `guiqwt-4.4.0/guiqwt/images/arrow_up.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/autorefresh.png` & `guiqwt-4.4.0/guiqwt/images/autorefresh.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/axes.png` & `guiqwt-4.4.0/guiqwt/images/axes.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/center.png` & `guiqwt-4.4.0/guiqwt/images/center.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/contrast.png` & `guiqwt-4.4.0/guiqwt/images/contrast.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/copytoclipboard.png` & `guiqwt-4.4.0/guiqwt/images/copytoclipboard.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/csapplylut.png` & `guiqwt-4.4.0/guiqwt/images/csapplylut.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/csection.png` & `guiqwt-4.4.0/guiqwt/images/csection.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/csection_a.png` & `guiqwt-4.4.0/guiqwt/images/csection_a.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/csection_oblique.png` & `guiqwt-4.4.0/guiqwt/images/csection_oblique.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/curvetypes/xfy.png` & `guiqwt-4.4.0/guiqwt/images/curvetypes/xfy.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/curvetypes/yfx.png` & `guiqwt-4.4.0/guiqwt/images/curvetypes/yfx.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/eraser.png` & `guiqwt-4.4.0/guiqwt/images/eraser.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/export.png` & `guiqwt-4.4.0/guiqwt/images/export.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/funct.png` & `guiqwt-4.4.0/guiqwt/images/funct.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/guiqwt.svg` & `guiqwt-4.4.0/guiqwt/images/guiqwt.svg`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/hflip.png` & `guiqwt-4.4.0/guiqwt/images/hflip.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/imagestats.png` & `guiqwt-4.4.0/guiqwt/images/imagestats.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/item_list.png` & `guiqwt-4.4.0/guiqwt/images/item_list.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/items/annotation.png` & `guiqwt-4.4.0/guiqwt/images/items/annotation.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/items/curve.png` & `guiqwt-4.4.0/guiqwt/images/items/curve.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/items/histogram2d.png` & `guiqwt-4.4.0/guiqwt/images/items/histogram2d.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/items/image.png` & `guiqwt-4.4.0/guiqwt/images/items/image.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/items/label.png` & `guiqwt-4.4.0/guiqwt/images/items/label.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/items/legend.png` & `guiqwt-4.4.0/guiqwt/images/items/legend.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/magnifier.png` & `guiqwt-4.4.0/guiqwt/images/magnifier.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/mask/mask_circle.png` & `guiqwt-4.4.0/guiqwt/images/mask/mask_circle.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/mask/mask_circle_outside.png` & `guiqwt-4.4.0/guiqwt/images/mask/mask_circle_outside.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/on_curve.png` & `guiqwt-4.4.0/guiqwt/images/on_curve.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/print.png` & `guiqwt-4.4.0/guiqwt/images/print.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/refresh.png` & `guiqwt-4.4.0/guiqwt/images/refresh.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/shapes/circle.png` & `guiqwt-4.4.0/guiqwt/images/shapes/circle.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/shapes/ellipse_shape.png` & `guiqwt-4.4.0/guiqwt/images/shapes/ellipse_shape.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/shapes/freeform.png` & `guiqwt-4.4.0/guiqwt/images/shapes/freeform.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/shapes/gtaxes.png` & `guiqwt-4.4.0/guiqwt/images/shapes/gtaxes.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/shapes/oblique_rectangle.png` & `guiqwt-4.4.0/guiqwt/images/shapes/oblique_rectangle.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/sift.svg` & `guiqwt-4.4.0/guiqwt/images/sift.svg`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/snapshot.png` & `guiqwt-4.4.0/guiqwt/images/snapshot.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/images/vflip.png` & `guiqwt-4.4.0/guiqwt/images/vflip.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/interfaces.py` & `guiqwt-4.4.0/guiqwt/interfaces.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/io.py` & `guiqwt-4.4.0/guiqwt/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -606,15 +606,15 @@
         item = klass()
         item.deserialize(reader)
     return item
 
 
 def save_items(writer, items):
     """Save items to HDF5 file:
-    * writer: :py:class:`guidata.hdf5io.HDF5Writer` object
+    * writer: :py:class:`guidata.dataset.hdf5io.HDF5Writer` object
     * items: serializable plot items"""
     counts = {}
     names = []
 
     def _get_name(item):
         basename = item_name_from_object(item)
         count = counts[basename] = counts.setdefault(basename, 0) + 1
@@ -627,16 +627,16 @@
             item.serialize(writer)
     with writer.group("plot_items"):
         writer.write_sequence(names)
 
 
 def load_items(reader):
     """Load items from file (HDF5, JSON, ...):
-    * reader: :py:class:`guidata.hdf5io.HDF5Reader` or
-      :py:class:`guidata.jsonio.JSONReader` object"""
+    * reader: :py:class:`guidata.dataset.hdf5io.HDF5Reader` or
+      :py:class:`guidata.dataset.jsonio.JSONReader` object"""
     with reader.group("plot_items"):
         names = reader.read_sequence()
     items = []
     for name in names:
         try:
             name_str = name.decode()
         except AttributeError:
```

### Comparing `guiqwt-4.3.3/guiqwt/label.py` & `guiqwt-4.4.0/guiqwt/label.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,16 @@
    :members:
    :inherited-members:
 """
 
 from qtpy.QtGui import QPen, QColor, QTextDocument
 from qtpy.QtCore import QRectF, QPointF, QLineF
 
-from guidata.utils import assert_interfaces_valid, update_dataset
+from guidata.utils.misc import assert_interfaces_valid
+from guidata.utils import update_dataset
 
 # Local imports
 from guiqwt.transitional import QwtPlotItem
 from guiqwt.config import CONF, _
 from guiqwt.curve import CurveItem
 from guiqwt.interfaces import IBasePlotItem, IShapeItemType, ISerializableType
 from guiqwt.styles import LabelParam
```

### Comparing `guiqwt-4.3.3/guiqwt/locale/fr/LC_MESSAGES/guiqwt.mo` & `guiqwt-4.4.0/guiqwt/locale/fr/LC_MESSAGES/guiqwt.mo`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/locale/fr/LC_MESSAGES/guiqwt.po` & `guiqwt-4.4.0/guiqwt/locale/fr/LC_MESSAGES/guiqwt.po`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/locale/guiqwt.pot` & `guiqwt-4.4.0/guiqwt/locale/guiqwt.pot`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/panels.py` & `guiqwt-4.4.0/guiqwt/panels.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,44 +5,44 @@
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """
 guiqwt.panels
 -------------
 
-The `panels` module provides :py:class:`guiqwt.panels.PanelWidget` (the 
-`panel` widget class from which all panels must derived from) and identifiers 
+The `panels` module provides :py:class:`guiqwt.panels.PanelWidget` (the
+`panel` widget class from which all panels must derived from) and identifiers
 for each kind of panel:
 
     * :py:data:`guiqwt.panels.ID_ITEMLIST`: ID of the `item list` panel
-    * :py:data:`guiqwt.panels.ID_CONTRAST`: ID of the `contrast 
+    * :py:data:`guiqwt.panels.ID_CONTRAST`: ID of the `contrast
       adjustment` panel
-    * :py:data:`guiqwt.panels.ID_XCS`: ID of the `X-axis cross section` 
+    * :py:data:`guiqwt.panels.ID_XCS`: ID of the `X-axis cross section`
       panel
-    * :py:data:`guiqwt.panels.ID_YCS`: ID of the `Y-axis cross section` 
+    * :py:data:`guiqwt.panels.ID_YCS`: ID of the `Y-axis cross section`
       panel
 
 .. seealso::
-        
+
     Module :py:mod:`guiqwt.plot`
-        Module providing ready-to-use curve and image plotting widgets and 
+        Module providing ready-to-use curve and image plotting widgets and
         dialog boxes
-    
+
     Module :py:mod:`guiqwt.curve`
         Module providing curve-related plot items and plotting widgets
-        
+
     Module :py:mod:`guiqwt.image`
         Module providing image-related plot items and plotting widgets
-        
+
     Module :py:mod:`guiqwt.tools`
         Module providing the `plot tools`
 """
 
 from qtpy.QtCore import Signal
-from guidata.qtwidgets import DockableWidget
+from guidata.widgets.dockable import DockableWidget
 
 
 # ===============================================================================
 # Panel IDs
 # ===============================================================================
 
 #: Item list panel
```

### Comparing `guiqwt-4.3.3/guiqwt/plot.py` & `guiqwt-4.4.0/guiqwt/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,25 +66,25 @@
 
 Examples
 ~~~~~~~~
 
 Simple example *without* the `plot manager`:
 
 .. literalinclude:: /../guiqwt/tests/filtertest1.py
-   :start-after: SHOW
+   :start-after: guitest: show
    :end-before: Workaround for Sphinx v0.6 bug: empty 'end-before' directive
 
 Simple example *with* the `plot manager`:
 even if this simple example does not justify the use of the `plot manager`
 (this is an unnecessary complication here), it shows how to use it. In more
 complex applications, using the `plot manager` allows to design highly versatile
 graphical user interfaces.
 
 .. literalinclude:: /../guiqwt/tests/filtertest2.py
-   :start-after: SHOW
+   :start-after: guitest: show
    :end-before: Workaround for Sphinx v0.6 bug: empty 'end-before' directive
 
 Reference
 ~~~~~~~~~
 
 .. autoclass:: PlotManager
    :members:
@@ -117,15 +117,15 @@
     QWidget,
     QMainWindow,
 )
 from qtpy.QtCore import Qt
 from qtpy import PYQT5
 
 from guidata.configtools import get_icon
-from guidata.utils import assert_interfaces_valid
+from guidata.utils.misc import assert_interfaces_valid
 from guidata.qthelpers import create_action, win32_fix_title_bar_background
 
 # Local imports
 from guiqwt.config import _
 from guiqwt.baseplot import BasePlot
 from guiqwt.curve import CurvePlot, PlotItemList
 from guiqwt.image import ImagePlot
@@ -819,20 +819,17 @@
         else:
             self.manager.register_all_curve_tools()
 
     def adjust_ycsw_height(self, height=None):
         if height is None:
             height = self.xcsw.height() - self.ycsw.toolbar.height()
         self.ycsw.adjust_height(height)
-        if height:
-            QApplication.processEvents()
 
     def xcsw_is_visible(self, state):
         if state:
-            QApplication.processEvents()
             self.adjust_ycsw_height()
         else:
             self.adjust_ycsw_height(0)
 
     def add_subplot(self, plot, i=0, j=0, plot_id=None):
         """Add a plot to the grid of plots"""
         self.plotlayout.addWidget(plot, i, j)
@@ -1292,20 +1289,17 @@
         configure_plot_splitter(self)
         configure_plot_splitter(self.sub_splitter)
 
     def adjust_ycsw_height(self, height=None):
         if height is None:
             height = self.xcsw.height() - self.ycsw.toolbar.height()
         self.ycsw.adjust_height(height)
-        if height:
-            QApplication.processEvents()
 
     def xcsw_is_visible(self, state):
         if state:
-            QApplication.processEvents()
             self.adjust_ycsw_height()
         else:
             self.adjust_ycsw_height(0)
 
 
 class ImageWidget(BaseImageWidget, PlotManager):
     """
```

### Comparing `guiqwt-4.3.3/guiqwt/pyplot.py` & `guiqwt-4.4.0/guiqwt/pyplot.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/qtdesigner.py` & `guiqwt-4.4.0/guiqwt/qtdesigner.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/qthelpers.py` & `guiqwt-4.4.0/guiqwt/qthelpers.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/scaler.py` & `guiqwt-4.4.0/guiqwt/scaler.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/shapes.py` & `guiqwt-4.4.0/guiqwt/shapes.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,40 +72,41 @@
 .. autoclass:: XRangeSelection
    :members:
    :inherited-members:
 """
 
 import os
 import sys
-import numpy as np
-from math import fabs, sqrt, sin, cos, pi
-
-from qtpy.QtGui import QPen, QBrush, QPolygonF, QTransform, QPainter
-from qtpy.QtCore import Qt, QRectF, QPointF, QLineF
+from math import cos, fabs, pi, sin, sqrt
 
-from guidata.utils import assert_interfaces_valid, update_dataset
+import numpy as np
+from guidata.utils.misc import assert_interfaces_valid
+from guidata.utils import update_dataset
+from qtpy.QtCore import QLineF, QPointF, QRectF, Qt
+from qtpy.QtGui import QBrush, QPainter, QPen, QPolygonF, QTransform
 
-# Local imports
-from guiqwt.transitional import QwtPlotItem, QwtSymbol, QwtPlotMarker
+from guiqwt.baseplot import canvas_to_axes
 from guiqwt.config import CONF, _
-from guiqwt.interfaces import IBasePlotItem, IShapeItemType, ISerializableType
-from guiqwt.styles import (
-    MarkerParam,
-    ShapeParam,
-    RangeShapeParam,
-    AxesShapeParam,
-    MARKERSTYLES,
-)
 from guiqwt.geometry import (
+    compute_center,
     vector_norm,
     vector_projection,
     vector_rotation,
-    compute_center,
 )
-from guiqwt.baseplot import canvas_to_axes
+from guiqwt.interfaces import IBasePlotItem, ISerializableType, IShapeItemType
+from guiqwt.styles import (
+    MARKERSTYLES,
+    AxesShapeParam,
+    MarkerParam,
+    RangeShapeParam,
+    ShapeParam,
+)
+
+# Local imports
+from guiqwt.transitional import QwtPlotItem, QwtPlotMarker, QwtSymbol
 
 QT_API = os.environ["QT_API"]
 
 
 class AbstractShape(QwtPlotItem):
     """Interface pour les objets manipulables
     il n'est pas nécessaire de dériver de QwtShape si on
@@ -228,14 +229,16 @@
         pass
 
     def move_local_point_to(self, handle, pos, ctrl=None):
         """Move a handle as returned by hit_test to the new position pos
         ctrl: True if <Ctrl> button is being pressed, False otherwise"""
         pt = canvas_to_axes(self, pos)
         self.move_point_to(handle, pt, ctrl)
+        if self.plot():
+            self.plot().SIG_ITEM_HANDLE_MOVED.emit(self)
 
     def move_local_shape(self, old_pos, new_pos):
         """Translate the shape such that old_pos becomes new_pos
         in canvas coordinates"""
         old_pt = canvas_to_axes(self, old_pos)
         new_pt = canvas_to_axes(self, new_pos)
         self.move_shape(old_pt, new_pt)
@@ -1098,14 +1101,17 @@
         super(EllipseShape, self).__init__(shapeparam=shapeparam)
         self.is_ellipse = False
         self.set_xdiameter(x1, y1, x2, y2)
 
     def switch_to_ellipse(self):
         self.is_ellipse = True
 
+    def switch_to_circle(self):
+        self.is_ellipse = False
+
     def set_xdiameter(self, x0, y0, x1, y1):
         """Set the coordinates of the ellipse's X-axis diameter"""
         xline = QLineF(x0, y0, x1, y1)
         yline = xline.normalVector()
         yline.translate(xline.pointAt(0.5) - xline.p1())
         if self.is_ellipse:
             yline.setLength(self.get_yline().length())
@@ -1125,15 +1131,15 @@
         yline = QLineF(x2, y2, x3, y3)
         xline = yline.normalVector()
         xline.translate(yline.pointAt(0.5) - yline.p1())
         if self.is_ellipse:
             xline.setLength(self.get_xline().length())
         xline.translate(xline.pointAt(0.5) - xline.p2())
         self.set_points(
-            [(xline.x1(), xline.y1()), (xline.x2(), xline.y2()), (x2, y2), (x3, y3)]
+            [(xline.x2(), xline.y2()), (xline.x1(), xline.y1()), (x2, y2), (x3, y3)]
         )
 
     def get_ydiameter(self):
         """Return the coordinates of the ellipse's Y-axis diameter"""
         return tuple(self.points[2]) + tuple(self.points[3])
 
     def get_rect(self):
```

### Comparing `guiqwt-4.3.3/guiqwt/signals.py` & `guiqwt-4.4.0/guiqwt/signals.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,97 +5,101 @@
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """
 guiqwt.signals
 --------------
 
-In `guiqwt` version 2, the `signals` module used to contain constants defining 
-the custom Qt SIGNAL objects used by `guiqwt`: the signals definition were 
-gathered here to avoid misspelling signals at connect and emit sites (with 
-old-style signals, any misspelled signal string would have lead to a silent 
+In `guiqwt` version 2, the `signals` module used to contain constants defining
+the custom Qt SIGNAL objects used by `guiqwt`: the signals definition were
+gathered here to avoid misspelling signals at connect and emit sites (with
+old-style signals, any misspelled signal string would have lead to a silent
 failure of signal emission or connection).
 
-Since version 3, to ensure PyQt5 compatibility, `guiqwt` is using only 
+Since version 3, to ensure PyQt5 compatibility, `guiqwt` is using only
 new-style signals and slots.
 
-However, all signals are summarized below, in order to facilitate migration 
+However, all signals are summarized below, in order to facilitate migration
 from `guiqwt` v2 to `guiqwt` v3.
 
 Signals available:
     :py:data:`guiqwt.baseplot.BasePlot.SIG_ITEM_MOVED`
-        Emitted by plot when an IBasePlotItem-like object was moved from 
+        Emitted by plot when an IBasePlotItem-like object was moved from
         (x0, y0) to (x1, y1)
-        
-        Arguments: item object, x0, y0, x1, y1
+
+        Arguments: item object, old_x, old_y, new_x, new_y
+    :py:data:`guiqwt.baseplot.BasePlot.SIG_ITEM_HANDLE_MOVED`
+        Emitted by plot when an IBasePlotItem-like object handle was moved
+
+        Arguments: item object
     :py:data:`guiqwt.baseplot.BasePlot.SIG_MARKER_CHANGED`
         Emitted by plot when a `guiqwt.shapes.Marker` position changes
-        
+
         Arguments: `guiqwt.shapes.Marker` object
     :py:data:`guiqwt.baseplot.BasePlot.SIG_AXES_CHANGED`
         Emitted by plot when a `guiqwt.shapes.Axes` position (or angle) changes
-        
+
         Arguments: `guiqwt.shapes.Axes` object
     :py:data:`guiqwt.baseplot.BasePlot.SIG_ANNOTATION_CHANGED`
         Emitted by plot when an annotations.AnnotatedShape position changes
-        
+
         Arguments: annotation item
     :py:data:`guiqwt.baseplot.BasePlot.SIG_RANGE_CHANGED`
         Emitted by plot when a shapes.XRangeSelection range changes
-        
+
         Arguments: range object, lower_bound, upper_bound
     :py:data:`guiqwt.baseplot.BasePlot.SIG_ITEMS_CHANGED`
         Emitted by plot when item list has changed (item removed, added, ...)
-        
+
         Arguments: plot
     :py:data:`guiqwt.baseplot.BasePlot.SIG_ACTIVE_ITEM_CHANGED`
         Emitted by plot when selected item has changed
-        
+
         Arguments: plot
     :py:data:`guiqwt.baseplot.BasePlot.SIG_ITEM_REMOVED`
-        Emitted by plot when an item was deleted from the itemlist or using 
+        Emitted by plot when an item was deleted from the itemlist or using
         the delete item tool
-        
+
         Arguments: removed item
     :py:data:`guiqwt.baseplot.BasePlot.SIG_ITEM_SELECTION_CHANGED`
         Emitted by plot when an item is selected
 
         Arguments: plot
     :py:data:`guiqwt.baseplot.BasePlot.SIG_PLOT_LABELS_CHANGED`
         Emitted (by plot) when plot's title or any axis label has changed
-        
+
         Arguments: plot
     :py:data:`guiqwt.baseplot.BasePlot.SIG_AXIS_DIRECTION_CHANGED`
         Emitted (by plot) when any plot axis direction has changed
-        
+
         Arguments: plot
     :py:data:`guiqwt.histogram.LevelsHistogram.SIG_VOI_CHANGED`
         Emitted by "contrast" panel's histogram when the lut range of some items
-        changed (for now, this signal is for guiqwt.histogram module's internal 
-        use only - the 'public' counterpart of this signal is SIG_LUT_CHANGED, 
+        changed (for now, this signal is for guiqwt.histogram module's internal
+        use only - the 'public' counterpart of this signal is SIG_LUT_CHANGED,
         see below)
-        
+
     :py:data:`guiqwt.baseplot.BasePlot.SIG_LUT_CHANGED`
         Emitted by plot when LUT has been changed by the user
 
         Arguments: plot
     :py:data:`guiqwt.baseplot.BasePlot.SIG_MASK_CHANGED`
         Emitted by plot when image mask has changed
 
         Arguments: MaskedImageItem object
     :py:data:`guiqwt.baseplot.BasePlot.SIG_CS_CURVE_CHANGED`
         Emitted by cross section plot when cross section curve data has changed
-        
+
         Arguments: plot
     :py:data:`guiqwt.panels.PanelWidget.SIG_VISIBILITY_CHANGED`
         Emitted for example by panels when their visibility has changed
 
         Arguments: state (boolean)
     :py:data:`guiqwt.tools.InteractiveTool.SIG_VALIDATE_TOOL`
-        Emitted by an interactive tool to notify that the tool has just been 
+        Emitted by an interactive tool to notify that the tool has just been
         "validated", i.e. <ENTER>, <RETURN> or <SPACE> was pressed
 
         Arguments: filter
     :py:data:`guiqwt.tools.InteractiveTool.SIG_TOOL_JOB_FINISHED`
         Emitted by an interactive tool to notify that it is finished doing its job
     :py:data:`guiqwt.tools.OpenFileTool.SIG_OPEN_FILE`
         Emitted by an open file tool
```

### Comparing `guiqwt-4.3.3/guiqwt/styles.py` & `guiqwt-4.4.0/guiqwt/styles.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/tests/benchmarks.py` & `guiqwt-4.4.0/guiqwt/tests/benchmarks.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,14 @@
 # Copyright © 2011 CEA
 # Pierre Raybaut
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """guiqwt plot benchmarking"""
 
-
-SHOW = False  # Show test in GUI-based test launcher
-
-
 import time
 import numpy as np
 
 from qtpy.QtWidgets import QApplication
 
 from guiqwt.plot import CurveWindow, ImageWindow
 from guiqwt.builder import make
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/brain.png` & `guiqwt-4.4.0/guiqwt/tests/brain.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/tests/brain_cylinder.png` & `guiqwt-4.4.0/guiqwt/tests/brain_cylinder.png`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/tests/computations.py` & `guiqwt-4.4.0/guiqwt/tests/computations.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright © 2009-2010 CEA
 # Pierre Raybaut
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """Plot computations test"""
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 from guiqwt.plot import CurveDialog
 from guiqwt.builder import make
 
 
 def plot(*items):
     win = CurveDialog(edit=False, toolbar=True)
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/contrast.py` & `guiqwt-4.4.0/guiqwt/tests/contrast.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright © 2009-2010 CEA
 # Pierre Raybaut
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """Contrast tool test"""
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 import os.path as osp
 
 from guiqwt.plot import ImageDialog
 from guiqwt.builder import make
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/cross_section.py` & `guiqwt-4.4.0/guiqwt/tests/cross_section.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright © 2009-2010 CEA
 # Pierre Raybaut
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """Renders a cross section chosen by a cross marker"""
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 import os.path as osp, numpy as np
 
 from guiqwt.plot import ImageDialog
 from guiqwt.builder import make
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/cross_section_oblique.py` & `guiqwt-4.4.0/guiqwt/tests/cross_section_oblique.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright © 2009-2011 CEA
 # Pierre Raybaut
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """Oblique averaged cross section test"""
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 import os.path as osp
 
 import guiqwt.cross_section
 
 # debug mode shows the ROI in the top-left corner of the image plot:
 guiqwt.cross_section.DEBUG = True
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/cursors.py` & `guiqwt-4.4.0/guiqwt/tests/cursors.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright © 2009-2011 CEA
 # Pierre Raybaut
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """Horizontal/vertical cursors test"""
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 from guiqwt.plot import CurveDialog
 from guiqwt.builder import make
 
 
 def plot(*items):
     win = CurveDialog(edit=False, toolbar=True)
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/customize_shape_tool.py` & `guiqwt-4.4.0/guiqwt/tests/customize_shape_tool.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright © 2012 CEA
 # Pierre Raybaut
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """Shows how to customize a shape created with a tool like RectangleTool"""
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 import os.path as osp
 
 from guiqwt.plot import ImageDialog
 from guiqwt.tools import (
     RectangleTool,
     EllipseTool,
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/dicom_image.py` & `guiqwt-4.4.0/guiqwt/tests/dicom_image.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """DICOM image test
 
 Requires pydicom (>=0.9.3)"""
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 import os.path as osp
 import guidata
 from guiqwt.plot import ImageDialog
 from guiqwt.builder import make
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/dotarraydemo.py` & `guiqwt-4.4.0/guiqwt/tests/dotarraydemo.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """
 Dot array example
 =================
 
-Example showing how to create a custom item (drawing dots of variable size) 
-and integrate the associated `guidata` dataset (GUI-based form) to edit its 
-parameters (directly into the same window as the plot itself, *and* within 
-the custom item parameters: right-click on the selectable item to open the 
+Example showing how to create a custom item (drawing dots of variable size)
+and integrate the associated `guidata` dataset (GUI-based form) to edit its
+parameters (directly into the same window as the plot itself, *and* within
+the custom item parameters: right-click on the selectable item to open the
 associated dialog box).
 """
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 import numpy as np
 
 import qtpy.QtCore as QC
 import qtpy.QtWidgets as QW
 import qtpy.QtGui as QG
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/filtertest1.py` & `guiqwt-4.4.0/guiqwt/tests/filtertest1.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright © 2009-2010 CEA
 # Pierre Raybaut
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """Simple filter testing application based on PyQt and guiqwt"""
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 from qtpy.QtWidgets import QWidget, QVBoxLayout, QHBoxLayout, QPushButton
 
 # ---Import plot widget base class
 from guiqwt.plot import CurveWidget
 from guiqwt.builder import make
 from guidata.configtools import get_icon
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/filtertest2.py` & `guiqwt-4.4.0/guiqwt/tests/filtertest2.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Pierre Raybaut
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """Simple filter testing application based on PyQt and guiqwt
 filtertest1.py + plot manager"""
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 from qtpy.QtWidgets import QWidget, QVBoxLayout, QHBoxLayout, QPushButton, QMainWindow
 from guidata.qthelpers import win32_fix_title_bar_background
 
 # ---Import plot widget base class
 from guiqwt.curve import CurvePlot
 from guiqwt.plot import PlotManager
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/fit.py` & `guiqwt-4.4.0/guiqwt/tests/fit.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Pierre Raybaut
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """Curve fitting tools"""
 
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 import numpy as np
 
 from guiqwt.widgets.fit import FitParam, guifit
 
 
 def test():
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/fliprotate.py` & `guiqwt-4.4.0/guiqwt/tests/fliprotate.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright © 2012 CEA
 # Pierre Raybaut
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """Flip/rotate test"""
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 from guiqwt.widgets.fliprotate import FlipRotateDialog, FlipRotateWidget
 from guiqwt.tests.rotatecrop import imshow, create_test_data
 
 
 def widget_test(fname, qapp):
     """Test the rotate/crop widget"""
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/get_point.py` & `guiqwt-4.4.0/guiqwt/tests/get_point.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 SelectPointTool test
 
 This guiqwt tool provide a MATLAB-like "ginput" feature.
 """
 
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 from guiqwt.plot import CurveDialog
 from guiqwt.tools import SelectPointTool
 from guiqwt.builder import make
 from guiqwt.config import _
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/get_segment.py` & `guiqwt-4.4.0/guiqwt/tests/get_segment.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 AnnotatedSegmentTool test
 
 This guiqwt tool provide a MATLAB-like "ginput" feature.
 """
 
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 import os.path as osp
 import numpy as np
 
 from guiqwt.plot import ImageDialog
 from guiqwt.tools import SelectTool, AnnotatedSegmentTool
 from guiqwt.builder import make
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/highprecisionxy.py` & `guiqwt-4.4.0/guiqwt/tests/highprecisionxy.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 # Copyright © 2011-2012 CEA
 # Ludovic Aubry
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """Plot computations test"""
 
-SHOW = False  # Show test in GUI-based test launcher
-
 
 def xyimagebug(offset):
     from guiqwt.plot import ImageDialog
     from guiqwt.builder import make
     import numpy
     import guidata
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/hist2d.py` & `guiqwt-4.4.0/guiqwt/tests/hist2d.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright © 2009-2010 CEA
 # Pierre Raybaut
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """2-D Histogram test"""
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 from numpy import random, array, dot, concatenate
 
 from guiqwt.plot import ImageDialog
 from guiqwt.builder import make
 from guiqwt.config import _
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/hist2d_func.py` & `guiqwt-4.4.0/guiqwt/tests/hist2d_func.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/tests/histogram.py` & `guiqwt-4.4.0/guiqwt/tests/histogram.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright © 2009-2010 CEA
 # Pierre Raybaut
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """Histogram test"""
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 from guiqwt.plot import CurveDialog
 from guiqwt.builder import make
 
 
 def test():
     """Test"""
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/image.py` & `guiqwt-4.4.0/guiqwt/tests/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 """ImageDialog test"""
 
 # FIXME: unexpected behavior when changing the xmin/xmax/ymin/ymax values in
 #       the image parameters (2nd tab: "Axes")
 
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 import numpy as np
 
 from guiqwt.plot import ImageDialog
 from guiqwt.builder import make
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/image_coords.py` & `guiqwt-4.4.0/guiqwt/tests/image_coords.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 """Testing image coordinates issues: see issue #90 on GitHub"""
 
 import numpy as np
 
 from guidata import qapplication
 from guiqwt.plot import ImageDialog
 from guiqwt.builder import make
+from guiqwt.tools import DisplayCoordsTool
 
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 
 def create_2d_gaussian(size, dtype, x0=0, y0=0, mu=0.0, sigma=2.0, amp=None):
     """Creating 2D Gaussian (-10 <= x <= 10 and -10 <= y <= 10)"""
     xydata = np.linspace(-10, 10, size)
     x, y = np.meshgrid(xydata, xydata)
     if amp is None:
@@ -29,22 +30,25 @@
 
 def imshow(data, makefunc, title=None):
     """Show image in a new window"""
     win = ImageDialog(edit=False, toolbar=True, wintitle=__doc__)
     image = makefunc(data, interpolation="nearest")
     text = "First pixel should be centered on (0, 0) coordinates"
     label = make.label(text, (1, 1), (0, 0), "L")
+    rect = make.rectangle(5, 5, 10, 10, "Rectangle")
     cursors = []
     for i_cursor in range(0, 21, 10):
         cursors.append(make.vcursor(i_cursor, movable=False))
         cursors.append(make.hcursor(i_cursor, movable=False))
     plot = win.get_plot()
     plot.set_title(title)
-    for item in [image, label] + cursors:
+    for item in [image, label, rect] + cursors:
         plot.add_item(item)
+    plot.select_item(image)
+    win.get_tool(DisplayCoordsTool).activate_curve_pointer(True)
     win.show()
     win.exec()
 
 
 def test():
     """Test"""
     _app = qapplication()
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/image_masked.py` & `guiqwt-4.4.0/guiqwt/tests/image_masked.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 Masked Image test, creating the MaskedImageItem object via make.maskedimage
 
 Masked image items are constructed using a masked array item. Masked data is
 ignored in computations, like the average cross sections.
 """
 
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 import os, os.path as osp, pickle
 
 from guiqwt.plot import ImageDialog
 from guiqwt.tools import ImageMaskTool
 from guiqwt.builder import make
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 FNAME = "image_masked.pickle"
 
 if __name__ == "__main__":
     import guidata
 
     _app = guidata.qapplication()
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/image_plot_tools.py` & `guiqwt-4.4.0/guiqwt/tests/image_plot_tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright © 2009-2010 CEA
 # Pierre Raybaut
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """All image and plot tools test"""
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 import os.path as osp
 
 from guiqwt.plot import ImageDialog
 from guiqwt.tools import (
     RectangleTool,
     EllipseTool,
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/image_rgb.py` & `guiqwt-4.4.0/guiqwt/tests/plot_log.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright © 2009-2010 CEA
+# Copyright © 2009-2011 CEA
 # Pierre Raybaut
 # Licensed under the terms of the CECILL License
-# (see guidata/__init__.py for details)
+# (see guiqwt/__init__.py for details)
 
-"""RGB Image test, creating the RGBImageItem object via make.rgbimage"""
+"""Logarithmic scale test for curve plotting"""
 
-SHOW = True  # Show test in GUI-based test launcher
-
-from guiqwt.plot import ImageDialog
+from guiqwt.plot import CurveDialog
 from guiqwt.builder import make
-import os.path as osp
-
-SHOW = True  # Show test in GUI-based test launcher
-
-TESTDIR = osp.abspath(osp.dirname(__file__))
-IMGFILE = osp.join(TESTDIR, "..", "images", "items", "image.png")
-
-
-def imshow(filename):
-    win = ImageDialog(edit=False, toolbar=True, wintitle="RGB image item test")
-    item = make.rgbimage(filename=filename, xdata=[-1, 1], ydata=[-1, 1])
-    plot = win.get_plot()
-    plot.add_item(item)
-    win.show()
-    win.exec_()
 
 
 def test():
     """Test"""
     # -- Create QApplication
     import guidata
 
     _app = guidata.qapplication()
     # --
-    imshow(IMGFILE)
+    import numpy as np
+
+    x = np.linspace(1, 10, 200)
+    y = np.exp(-x)
+    y[0] = 0
+    item = make.curve(x, y, color="b")
+    item = make.error(x, y, None, y * 0.23)
+
+    win = CurveDialog()
+    plot = win.get_plot()
+    plot.set_axis_scale("left", "log")
+    plot.set_axis_scale("bottom", "log")
+    #    plot.set_axis_limits("left", 4.53999297625e-05, 22026.4657948)
+    plot.add_item(item)
+    win.show()
+    win.exec_()
 
 
 if __name__ == "__main__":
     test()
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/imagefilter.py` & `guiqwt-4.4.0/guiqwt/tests/imagefilter.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright © 2009-2010 CEA
 # Pierre Raybaut
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """Image filter demo"""
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 from scipy.ndimage import gaussian_filter
 
 from guiqwt.plot import ImageDialog
 from guiqwt.builder import make
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/imagesuperp.py` & `guiqwt-4.4.0/guiqwt/tests/imagesuperp.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright © 2009-2010 CEA
 # Pierre Raybaut
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """Image superposition test"""
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 import os.path as osp
 
 from guiqwt.plot import ImageDialog
 from guiqwt.tools import RectangleTool, EllipseTool, PlaceAxesTool, FreeFormTool
 from guiqwt.builder import make
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/imagexy.py` & `guiqwt-4.4.0/guiqwt/tests/imagexy.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Pierre Raybaut
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """Image with custom X/Y axes linear scales"""
 
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 from guiqwt.plot import ImageDialog
 from guiqwt.builder import make
 
 import numpy as np
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/loadsaveitems_hdf5.py` & `guiqwt-4.4.0/guiqwt/tests/loadsaveitems_hdf5.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 # Copyright © 2012 CEA
 # Pierre Raybaut
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """Load/save items from/to HDF5 file"""
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 # WARNING:
 # This script requires read/write permissions on current directory
 
-from guidata.hdf5io import HDF5Reader, HDF5Writer
+from guidata.dataset.hdf5io import HDF5Reader, HDF5Writer
 
 from guiqwt.tests.loadsaveitems_pickle import IOTest
 
 
 class HDF5Test(IOTest):
     FNAME = "loadsavecanvas.h5"
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/loadsaveitems_json.py` & `guiqwt-4.4.0/guiqwt/tests/loadsaveitems_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 
 """
 
 import os.path as osp
 
 from guiqwt.tests.loadsaveitems_pickle import IOTest
 
-from guidata.jsonio import JSONReader, JSONWriter
+from guidata.dataset.jsonio import JSONReader, JSONWriter
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 
 class JSONTest(IOTest):
     """Class for JSON I/O testing"""
 
     FNAME = osp.join(osp.dirname(__file__), "loadsavecanvas.json")
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/loadsaveitems_pickle.py` & `guiqwt-4.4.0/guiqwt/tests/loadsaveitems_pickle.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Pierre Raybaut
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """Load/save items using Python's pickle protocol"""
 
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 # WARNING:
 # This script requires read/write permissions on current directory
 
 from qtpy.QtGui import QFont
 
 import os
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/loadtest.py` & `guiqwt-4.4.0/guiqwt/tests/loadtest.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright © 2009-2021 CEA
 # Pierre Raybaut
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """Load test: instantiating a large number of image widgets"""
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 # import cProfile
 # from pstats import Stats
 from qtpy.QtWidgets import QApplication, QMainWindow, QWidget, QTabWidget, QGridLayout
 import numpy as np
 
 from guidata.qthelpers import win32_fix_title_bar_background
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/manager.py` & `guiqwt-4.4.0/guiqwt/tests/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright © 2009-2010 CEA
 # Pierre Raybaut
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """PlotManager test"""
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 import os.path as osp
 
 from qtpy.QtWidgets import QMainWindow, QWidget, QGridLayout
 
 from guidata.qthelpers import win32_fix_title_bar_background
 from guiqwt.image import ImagePlot
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/mandelbrot.py` & `guiqwt-4.4.0/guiqwt/tests/mandelbrot.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright © 2009-2010 CEA
 # Pierre Raybaut
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """Mandelbrot demo"""
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 import numpy as np
 
 from qtpy.QtCore import QRectF, QPointF
 
 from guiqwt.config import _
 from guiqwt.plot import ImageDialog
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/mr-brain.dcm` & `guiqwt-4.4.0/guiqwt/tests/mr-brain.dcm`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/tests/pcolor.py` & `guiqwt-4.4.0/guiqwt/tests/pcolor.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Ludovic Aubry
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """ImageDialog / Pcolor test"""
 
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 import numpy as np
 
 from guiqwt.plot import ImageDialog
 from guiqwt.builder import make
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/plot.py` & `guiqwt-4.4.0/guiqwt/tests/plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright © 2009-2010 CEA
 # Pierre Raybaut
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """CurveDialog test"""
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 from qtpy.QtGui import QFont
 
 from guiqwt.plot import CurveDialog
 from guiqwt.builder import make
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/plot_log.py` & `guiqwt-4.4.0/guiqwt/tests/image_rgb.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright © 2009-2011 CEA
+# Copyright © 2009-2010 CEA
 # Pierre Raybaut
 # Licensed under the terms of the CECILL License
-# (see guiqwt/__init__.py for details)
+# (see guidata/__init__.py for details)
 
-"""Logarithmic scale test for curve plotting"""
+"""RGB Image test, creating the RGBImageItem object via make.rgbimage"""
 
-SHOW = False  # Do not show test in GUI-based test launcher
+# guitest: show
 
-from guiqwt.plot import CurveDialog
+from guiqwt.plot import ImageDialog
 from guiqwt.builder import make
+import os.path as osp
+
+# guitest: show
+
+TESTDIR = osp.abspath(osp.dirname(__file__))
+IMGFILE = osp.join(TESTDIR, "..", "images", "items", "image.png")
+
+
+def imshow(filename):
+    win = ImageDialog(edit=False, toolbar=True, wintitle="RGB image item test")
+    item = make.rgbimage(filename=filename, xdata=[-1, 1], ydata=[-1, 1])
+    plot = win.get_plot()
+    plot.add_item(item)
+    win.show()
+    win.exec_()
 
 
 def test():
     """Test"""
     # -- Create QApplication
     import guidata
 
     _app = guidata.qapplication()
     # --
-    import numpy as np
-
-    x = np.linspace(1, 10, 200)
-    y = np.exp(-x)
-    y[0] = 0
-    item = make.curve(x, y, color="b")
-    item = make.error(x, y, None, y * 0.23)
-
-    win = CurveDialog()
-    plot = win.get_plot()
-    plot.set_axis_scale("left", "log")
-    plot.set_axis_scale("bottom", "log")
-    #    plot.set_axis_limits("left", 4.53999297625e-05, 22026.4657948)
-    plot.add_item(item)
-    win.show()
-    win.exec_()
+    imshow(IMGFILE)
 
 
 if __name__ == "__main__":
     test()
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/plot_timecurve.py` & `guiqwt-4.4.0/guiqwt/tests/plot_timecurve.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from qtpy import QtCore as QC
 from qtpy import QtWidgets as QW
 from qwt import QwtScaleDraw, QwtText
 
 from guiqwt.builder import make
 from guiqwt.plot import CurveWidget
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 
 class DummyDevice(QC.QObject):
     NEW_SAMPLE = QC.Signal(object, int, float)
 
     def __init__(self, period=500, duration_range=None, mode=None):
         super(DummyDevice, self).__init__()
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/plot_yreverse.py` & `guiqwt-4.4.0/guiqwt/tests/plot_yreverse.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 # Copyright © 2009-2010 CEA
 # Pierre Raybaut
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """Reverse y-axis test for curve plotting"""
 
-SHOW = False  # Do not show test in GUI-based test launcher
-
 from guiqwt.plot import CurveDialog
 from guiqwt.builder import make
 
 
 def test():
     """Test"""
     # -- Create QApplication
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/polygons.py` & `guiqwt-4.4.0/guiqwt/tests/polygons.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """PolygonMapItem test
 
 PolygonMapItem is intended to display maps ie items containing
 several hundreds of independent polygons.
 """
 
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 from guiqwt.plot import ImageDialog
 from guiqwt.curve import PolygonMapItem
 
 from numpy.random import rand, randint
 from numpy import concatenate, linspace, int32, uint32, zeros, empty, pi, cos, sin
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/pyplot.py` & `guiqwt-4.4.0/guiqwt/tests/pyplot.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 """
 pyplot test
 
 Interactive plotting interface with MATLAB-like syntax
 """
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 import numpy as np
 
 from guiqwt.pyplot import *
 
 
 def main():
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/qtdesigner.py` & `guiqwt-4.4.0/guiqwt/tests/qtdesigner.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 # -*- coding: utf-8 -*-
 """
 Testing guiqwt QtDesigner plugins
 
-These plugins provide CurveWidget and ImageWidget objects 
+These plugins provide CurveWidget and ImageWidget objects
 embedding in GUI layouts directly from QtDesigner.
 """
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 import sys, os.path as osp
 
 from qtpy.QtWidgets import QApplication
 from guiqwt.qtdesigner import loadui
 from guiqwt.builder import make
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/qtdesigner.ui` & `guiqwt-4.4.0/guiqwt/tests/qtdesigner.ui`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/tests/resize.py` & `guiqwt-4.4.0/guiqwt/tests/resize.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright © 2012 CEA
 # Pierre Raybaut
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """Resize test: using the scaler C++ engine to resize images"""
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 
 def test():
     """Test"""
     import os.path as osp
     from guiqwt import io, scaler, pyplot as plt
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/rotatecrop.py` & `guiqwt-4.4.0/guiqwt/tests/rotatecrop.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Pierre Raybaut
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """Rotate/crop test: using the scaler C++ engine to rotate/crop images"""
 
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 import os.path as osp
 import numpy as np
 
 from guiqwt.builder import make
 from guiqwt.plot import ImageDialog
 from guiqwt.widgets.rotatecrop import (
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/sift.py` & `guiqwt-4.4.0/guiqwt/tests/sift.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # (see guiqwt/__init__.py for details)
 
 """
 SIFT, the Signal and Image Filtering Tool
 Simple signal and image processing application based on guiqwt and guidata
 """
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 from qtpy.QtWidgets import (
     QMainWindow,
     QMessageBox,
     QSplitter,
     QListWidget,
     QVBoxLayout,
@@ -50,15 +50,15 @@
 from guidata.qthelpers import (
     create_action,
     add_actions,
     get_std_icon,
     win32_fix_title_bar_background,
 )
 from guidata.widgets.console import DockableConsole
-from guidata.qtwidgets import DockableWidget, DockableWidgetMixin
+from guidata.widgets.dockable import DockableWidget, DockableWidgetMixin
 from guidata.utils import update_dataset
 
 from guiqwt.config import _
 from guiqwt.plot import CurveWidget, ImageWidget
 from guiqwt.builder import make
 
 APP_NAME = _("Sift")
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/simple_dialog.py` & `guiqwt-4.4.0/guiqwt/tests/simple_dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright © 2009-2010 CEA
 # Pierre Raybaut
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """Simple dialog box based on guiqwt and guidata"""
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 import scipy.ndimage
 
 from guidata.dataset.datatypes import DataSet
 from guidata.dataset.dataitems import StringItem, IntItem, ChoiceItem
 from guidata.dataset.qtwidgets import DataSetShowGroupBox, DataSetEditGroupBox
 from guidata.utils import update_dataset
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/simple_window.py` & `guiqwt-4.4.0/guiqwt/tests/simple_window.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright © 2009-2010 CEA
 # Pierre Raybaut
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """Simple application based on guiqwt and guidata"""
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 
 from qtpy.QtWidgets import QMainWindow, QMessageBox, QSplitter, QListWidget
 from qtpy.QtCore import QSize, __version__, Qt
 from qtpy.compat import getopenfilename
 
 import sys, platform
 import numpy as np
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/styles.py` & `guiqwt-4.4.0/guiqwt/tests/styles.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 # Copyright © 2009-2010 CEA
 # Pierre Raybaut
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """Styles unit tests"""
 
-SHOW = False  # Do not show test in GUI-based test launcher
-
 import unittest
 
 from qtpy.QtCore import Qt, QSize
 from qtpy.QtGui import QPen, QBrush
 
 from guiqwt.transitional import QwtSymbol
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/syncplot.py` & `guiqwt-4.4.0/guiqwt/tests/syncplot.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,117 +3,144 @@
 # Copyright © 2010 Ludovic Aubry
 # Copyright © 2022 Pierre Raybaut
 # Licensed under the terms of the CECILL License
 # (see guidata/__init__.py for details)
 
 """SyncPlotDialog test"""
 
+import numpy as np
 from guidata.configtools import get_icon
 from guidata.qthelpers import win32_fix_title_bar_background
 from guiqwt.baseplot import BasePlot
 from guiqwt.builder import make
 from guiqwt.config import _
-from guiqwt.curve import CurvePlot
+from guiqwt.curve import CurvePlot, CurveItem
+from guiqwt.image import ImagePlot
 from guiqwt.plot import PlotManager, SubplotWidget
+from guiqwt.tests.image_coords import create_2d_gaussian
 from qtpy import QtGui as QG
 from qtpy import QtWidgets as QW
+from qtpy import QtCore as QC
 
-SHOW = False  # Show test in GUI-based test launcher
+# guitest: show
 
 
 class SyncPlotWindow(QW.QMainWindow):
     """Window for showing plots, optionally synchronized"""
 
     def __init__(self, parent=None, title=None):
         super().__init__(parent)
         win32_fix_title_bar_background(self)
         self.setWindowTitle(self.__doc__ if title is None else title)
         self.setWindowIcon(get_icon("guiqwt.svg"))
-
         self.manager = PlotManager(None)
         self.manager.set_main(self)
-        toolbar = QW.QToolBar(_("Tools"), self)
+        self.subplotwidget = SubplotWidget(self.manager, parent=self)
+        self.setCentralWidget(self.subplotwidget)
+        toolbar = QW.QToolBar(_("Tools"))
         self.manager.add_toolbar(toolbar, "default")
         toolbar.setMovable(True)
         toolbar.setFloatable(True)
         self.addToolBar(toolbar)
 
-        self.subplotwidget = SubplotWidget(self.manager, parent=self)
-        self.setCentralWidget(self.subplotwidget)
-
-    def showEvent(self, event):
-        """Finalize window"""
+    def add_panels(self):
+        """Add standard panels"""
         self.subplotwidget.add_standard_panels()
+
+    def rescale_plots(self):
+        """Rescale all plots"""
         QW.QApplication.instance().processEvents()
         for plot in self.subplotwidget.plots:
             plot.do_autoscale()
+
+    def showEvent(self, event):  # pylint: disable=C0103
+        """Reimplement Qt method"""
         super().showEvent(event)
+        QC.QTimer.singleShot(0, self.rescale_plots)
 
     def add_plot(self, row, col, plot, sync=False, plot_id=None):
         """Add plot to window"""
         if plot_id is None:
             plot_id = str(len(self.subplotwidget.plots) + 1)
         self.subplotwidget.add_subplot(plot, row, col, plot_id)
         if sync and len(self.subplotwidget.plots) > 1:
             syncaxis = self.manager.synchronize_axis
             for i_plot in range(len(self.subplotwidget.plots) - 1):
                 syncaxis(BasePlot.X_BOTTOM, [plot_id, f"{i_plot + 1}"])
                 syncaxis(BasePlot.Y_LEFT, [plot_id, f"{i_plot + 1}"])
 
 
-def plot(items1, items2, items3, items4):
+def plot(*itemlists):
     """Plot items in SyncPlotDialog"""
     win = SyncPlotWindow()
     row, col = 0, 0
-    for items in [items1, items2, items3, items4]:
-        plot = CurvePlot()
+    has_curves = any(isinstance(item, CurveItem) for item in itemlists[0])
+    for items in itemlists:
+        plot = CurvePlot() if has_curves else ImagePlot()
         for item in items:
             plot.add_item(item)
         plot.set_axis_font("left", QG.QFont("Courier"))
         plot.set_items_readonly(False)
         win.add_plot(row, col, plot, sync=True)
         col += 1
         if col == 2:
             row += 1
             col = 0
+    win.add_panels()
+    contrast = win.subplotwidget.contrast
+    if contrast is not None:
+        contrast.show()
+    win.resize(800, 600)
     win.show()
 
 
-def test():
+def test_curves():
     """Test"""
-    # -- Create QApplication
-    import guidata
-
-    app = guidata.qapplication()
-    # --
-    from numpy import linspace, sin
-
-    x = linspace(-10, 10, 200)
+    x = np.linspace(-10, 10, 200)
     dy = x / 100.0
-    y = sin(sin(sin(x)))
-    x2 = linspace(-10, 10, 20)
-    y2 = sin(sin(sin(x2)))
+    y = np.sin(np.sin(np.sin(x)))
+    x2 = np.linspace(-10, 10, 20)
+    y2 = np.sin(np.sin(np.sin(x2)))
     plot(
         [
             make.curve(x, y, color="b"),
             make.label(
                 "Relative position <b>outside</b>", (x[0], y[0]), (-10, -10), "BR"
             ),
         ],
         [
             make.curve(x2, y2, color="g"),
         ],
         [
-            make.curve(x, sin(2 * y), color="r"),
+            make.curve(x, np.sin(2 * y), color="r"),
             make.label("Relative position <i>inside</i>", (x[0], y[0]), (10, 10), "TL"),
         ],
         [
             make.merror(x, y / 2, dy),
             make.label("Absolute position", "R", (0, 0), "R"),
             make.legend("TR"),
         ],
     )
-    app.exec()
+    QW.QApplication.instance().exec()
+
+
+def test_images():
+    """Test"""
+    img1 = create_2d_gaussian(20, np.uint8, x0=-10, y0=-10, mu=7, sigma=10.0)
+    img2 = create_2d_gaussian(20, np.uint8, x0=-10, y0=-10, mu=5, sigma=8.0)
+    img3 = create_2d_gaussian(20, np.uint8, x0=-10, y0=-10, mu=3, sigma=6.0)
+
+    def makeim(data):
+        """Make image item"""
+        return make.image(data, interpolation="nearest")
+
+    plot([makeim(img1)], [makeim(img2)], [makeim(img3)])
+    QW.QApplication.instance().exec()
 
 
 if __name__ == "__main__":
-    test()
+    # -- Create QApplication
+    import guidata
+
+    _APP = guidata.qapplication()
+    test_curves()
+    test_images()
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/test_line.py` & `guiqwt-4.4.0/guiqwt/tests/test_line.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,17 +3,14 @@
 # Copyright © 2010 CEA
 # Ludovic Aubry
 # Licensed under the terms of the CECILL License
 # (see guidata/__init__.py for details)
 
 """Internal test related to pcolor feature"""
 
-
-SHOW = False  # Show test in GUI-based test launcher
-
 from guiqwt._scaler import _line_test as line
 from numpy import int32, zeros
 
 N = 10
 imin = zeros((N,), int32)
 imax = zeros((N,), int32)
```

### Comparing `guiqwt-4.3.3/guiqwt/tests/transform.py` & `guiqwt-4.4.0/guiqwt/tests/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Pierre Raybaut
 # Licensed under the terms of the CECILL License
 # (see guiqwt/__init__.py for details)
 
 """Tests around image transforms: rotation, translation, ..."""
 
 
-SHOW = True  # Show test in GUI-based test launcher
+# guitest: show
 import os
 
 from qtpy.QtCore import QRectF
 from qtpy.QtGui import QImage
 from qtpy import API
 
 print("Qt API: " + API)
```

### Comparing `guiqwt-4.3.3/guiqwt/tools.py` & `guiqwt-4.4.0/guiqwt/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 Example
 ~~~~~~~
 
 The following example add all the existing tools to an `ImageWidget` object
 for testing purpose:
 
 .. literalinclude:: /../guiqwt/tests/image_plot_tools.py
-   :start-after: SHOW
+   :start-after: guitest: show
    :end-before: Workaround for Sphinx v0.6 bug: empty 'end-before' directive
 
 .. image:: /images/screenshots/image_plot_tools.png
 
 
 Reference
 ~~~~~~~~~
@@ -1067,14 +1067,15 @@
         self.set_shape_style(annotation)
         return annotation, 0, 1
 
 
 class AnnotatedEllipseTool(EllipseTool):
     def create_shape(self):
         annotation = AnnotatedEllipse(0, 0, 1, 1)
+        annotation.shape.switch_to_circle()
         self.set_shape_style(annotation)
         return annotation, 0, 1
 
     def handle_final_shape(self, shape):
         shape.shape.switch_to_ellipse()
         super(EllipseTool, self).handle_final_shape(shape)
```

### Comparing `guiqwt-4.3.3/guiqwt/transitional.py` & `guiqwt-4.4.0/guiqwt/transitional.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/widgets/__init__.py` & `guiqwt-4.4.0/guiqwt/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/widgets/base.py` & `guiqwt-4.4.0/guiqwt/widgets/base.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/widgets/fit.py` & `guiqwt-4.4.0/guiqwt/widgets/fit.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     * or automatically (with standard optimization algorithms
       provided by :py:mod:`scipy`).
 
 Example
 ~~~~~~~
 
 .. literalinclude:: /../guiqwt/tests/fit.py
-   :start-after: SHOW
+   :start-after: guitest: show
    :end-before: Workaround for Sphinx v0.6 bug: empty 'end-before' directive
 
 .. image:: /images/screenshots/fit.png
 
 Reference
 ~~~~~~~~~
```

### Comparing `guiqwt-4.3.3/guiqwt/widgets/fliprotate.py` & `guiqwt-4.4.0/guiqwt/widgets/fliprotate.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/widgets/resizedialog.py` & `guiqwt-4.4.0/guiqwt/widgets/resizedialog.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt/widgets/rotatecrop.py` & `guiqwt-4.4.0/guiqwt/widgets/rotatecrop.py`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/guiqwt.egg-info/PKG-INFO` & `guiqwt-4.4.0/guiqwt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: guiqwt
-Version: 4.3.3
+Version: 4.4.0
 Summary: guiqwt is a set of tools for curve and image plotting (extension to PythonQwt)
 Home-page: https://github.com/PierreRaybaut/guiqwt
 Author: Pierre Raybaut
 Author-email: pierre.raybaut@gmail.com
 License: CeCILL V2
-Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
@@ -65,9 +64,7 @@
 .. _NumPy: https://pypi.python.org/pypi/NumPy
 .. _SciPy: https://pypi.python.org/pypi/SciPy
 .. _Pillow: https://pypi.python.org/pypi/Pillow
 
 See the `README`_ and `documentation`_ for more details.
 
 .. _README: https://github.com/PierreRaybaut/guiqwt/blob/master/README.md
-
-
```

### Comparing `guiqwt-4.3.3/guiqwt.egg-info/SOURCES.txt` & `guiqwt-4.4.0/guiqwt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/setup.py` & `guiqwt-4.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,49 @@
 import setuptools  # analysis:ignore
 import numpy
 import sys
 import os
 import os.path as osp
 import subprocess
 from numpy.distutils.core import setup, Extension
-from guidata.utils import get_subpackages, get_package_data, cythonize_all
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
 
 
 LIBNAME = "guiqwt"
 __description__ = (
     "guiqwt is a set of tools for curve and image plotting (extension to PythonQwt)"
 )
 
@@ -190,27 +224,27 @@
 # Compiling Cython modules to C source code: this is the only way I found to
 # be able to build both Fortran and Cython extensions together
 # (this could be changed now as there is no longer Fortran extensions here...)
 cythonize_all("src")
 
 setup(
     name=LIBNAME,
-    version="4.3.3",  # Update here *AND* in __init__.py!
+    version="4.4.0",  # Update here *AND* in __init__.py!
     # (Until setup.py has been fully retrofitted, this manual sync is mandatory)
     description=__description__,
     long_description=LONG_DESCRIPTION,
     packages=get_subpackages(LIBNAME),
     package_data={
         LIBNAME: get_package_data(LIBNAME, (".png", ".svg", ".mo", ".dcm", ".ui"))
     },
     data_files=[(r"Doc", [CHM_DOC])] if CHM_DOC else [],
     install_requires=[
         "NumPy>=1.3",
         "SciPy>=0.7",
-        "guidata>=2.3",
+        "guidata>=3.0",
         "PythonQwt>=0.10",
         "Pillow",
         "QtPy>=1.3",
     ],
     extras_require={
         "Doc": ["Sphinx>=1.1"],
         "DICOM": ["pydicom>=0.9.3"],
```

### Comparing `guiqwt-4.3.3/sift/create_exe.py` & `guiqwt-4.4.0/sift/create_exe.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 # SIFT is the Signal and Image Filtering Tool
 # Simple signal and image processing application based on guiqwt and guidata
 # (see guiqwt/tests/sift.py)
 
 """Create a stand-alone executable"""
 
 try:
-    from guidata.disthelpers import Distribution
+    from guidata.utils.disthelpers import Distribution
 except ImportError:
     raise ImportError("This script requires guidata 1.4+")
 
 # Importing modules to be bundled
 from guiqwt.tests import sift
 
 
 def create_executable():
-    """Build executable using ``guidata.disthelpers``"""
+    """Build executable using ``guidata.utils.disthelpers``"""
     dist = Distribution()
     dist.setup(
         name="Sift",
         version=sift.VERSION,
         description="Signal and Image Filtering Tool",
         script="sift.pyw",
         target_name="sift.exe",
```

### Comparing `guiqwt-4.3.3/sift/sift.ico` & `guiqwt-4.4.0/sift/sift.ico`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/src/arrays.hpp` & `guiqwt-4.4.0/src/arrays.hpp`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/src/debug.hpp` & `guiqwt-4.4.0/src/debug.hpp`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/src/histogram2d.c` & `guiqwt-4.4.0/src/histogram2d.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.26 */
+/* Generated by Cython 0.29.32 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_26"
-#define CYTHON_HEX_VERSION 0x001D1AF0
+#define CYTHON_ABI "0_29_32"
+#define CYTHON_HEX_VERSION 0x001D20F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -45,14 +45,15 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -81,18 +82,22 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -122,18 +127,67 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PY_NOGIL)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_PYSTON 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
+  #ifndef CYTHON_USE_TYPE_SLOTS
+    #define CYTHON_USE_TYPE_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_INTERNALS
+    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #endif
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #ifndef CYTHON_ASSUME_SAFE_MACROS
+    #define CYTHON_ASSUME_SAFE_MACROS 1
+  #endif
+  #ifndef CYTHON_UNPACK_METHODS
+    #define CYTHON_UNPACK_METHODS 1
+  #endif
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -168,32 +222,41 @@
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #ifndef CYTHON_FAST_THREAD_STATE
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_FAST_THREAD_STATE
+    #define CYTHON_FAST_THREAD_STATE 0
+  #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030B00A1)
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
     #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
   #endif
-  #ifndef CYTHON_USE_EXC_INFO_STACK
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_USE_EXC_INFO_STACK
+    #define CYTHON_USE_EXC_INFO_STACK 0
+  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
   #if PY_MAJOR_VERSION < 3
     #include "longintrepr.h"
@@ -637,16 +700,18 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(WIN32) || defined(MS_WINDOWS)
-  #define _USE_MATH_DEFINES
+#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
+  #if !defined(_USE_MATH_DEFINES)
+    #define _USE_MATH_DEFINES
+  #endif
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -955,195 +1020,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":690
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":691
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":692
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":693
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":697
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":698
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":699
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":700
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":704
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":705
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":714
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":715
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":716
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":718
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":719
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":720
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":722
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":723
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":725
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":726
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":727
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1170,42 +1235,42 @@
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":729
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":730
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":731
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":733
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -3059,15 +3124,15 @@
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_data_tmp.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":735
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3076,29 +3141,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":736
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":735
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3109,15 +3174,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":738
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3126,29 +3191,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":739
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":738
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3159,15 +3224,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":741
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3176,29 +3241,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":742
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":741
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3209,15 +3274,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":744
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3226,29 +3291,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":745
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":744
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3259,15 +3324,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":747
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3276,29 +3341,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":748
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":747
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3309,212 +3374,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":750
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":751
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":752
+    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":751
+    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":754
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":750
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":929
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":930
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":931
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":929
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":933
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":934
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":935
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":936
+    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":935
+    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":937
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":933
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":941
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3530,15 +3595,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":942
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -3546,84 +3611,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":943
+      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":942
+      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":944
+    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":945
+      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 945, __pyx_L5_except_error)
+      __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":942
+    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":941
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3638,15 +3703,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":947
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3662,15 +3727,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":948
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -3678,84 +3743,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":949
+      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":948
+      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":950
+    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":951
+      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 951, __pyx_L5_except_error)
+      __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":948
+    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":947
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3770,15 +3835,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":953
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3794,15 +3859,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":954
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -3810,84 +3875,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":955
+      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":954
+      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":956
+    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":957
+      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 957, __pyx_L5_except_error)
+      __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":954
+    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":953
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3902,176 +3967,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":967
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":979
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":967
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":982
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":994
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":982
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":997
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":1004
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":997
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":1007
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":1011
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":1007
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":1014
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":1018
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":1014
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -4160,43 +4225,43 @@
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_u, __pyx_k_u, sizeof(__pyx_k_u), 0, 0, 1, 1},
   {&__pyx_n_s_v, __pyx_k_v, sizeof(__pyx_k_v), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 32, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 945, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 944, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":945
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 945, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":951
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 951, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 950, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "histogram2d.pyx":19
  * @cython.profile(False)
  * @cython.boundscheck(False)
  * def histogram2d(np.ndarray[double, ndim=1] X, np.ndarray[double, ndim=1] Y,             # <<<<<<<<<<<<<<
@@ -4288,46 +4353,46 @@
   sizeof(PyTypeObject),
   #else
   sizeof(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 200, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 200, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
   __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 223, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
   __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 227, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
   __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 239, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
   __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 771, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
   __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 773, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
   __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 775, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
   __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 777, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
   __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 779, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
   __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 781, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
   __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 783, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
   __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 785, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
   __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 787, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
   __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 789, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
   __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 827, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -4579,15 +4644,15 @@
  * # Copyright (C) 2012 CEA
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":1014
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -5951,14 +6016,20 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
   #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
     PyCodeObject *py_code = NULL;
     PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_srcfile = NULL;
@@ -6014,22 +6085,32 @@
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
+        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) goto bad;
+        if (!py_code) {
+            /* If the code object creation fails, then we should clear the
+               fetched exception references and propagate the new exception */
+            Py_XDECREF(ptype);
+            Py_XDECREF(pvalue);
+            Py_XDECREF(ptraceback);
+            goto bad;
+        }
+        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -7154,19 +7235,41 @@
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
   static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
+    char ctversion[5];
+    int same=1, i, found_dot;
+    const char* rt_from_call = Py_GetVersion();
+    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    found_dot = 0;
+    for (i = 0; i < 4; i++) {
+        if (!ctversion[i]) {
+            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
+            break;
+        }
+        if (rt_from_call[i] != ctversion[i]) {
+            same = 0;
+            break;
+        }
+    }
+    if (!same) {
+        char rtversion[5] = {'\0'};
         char message[200];
+        for (i=0; i<4; ++i) {
+            if (rt_from_call[i] == '.') {
+                if (found_dot) break;
+                found_dot = 1;
+            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
+                break;
+            }
+            rtversion[i] = rt_from_call[i];
+        }
         PyOS_snprintf(message, sizeof(message),
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
@@ -7370,15 +7473,15 @@
   }
 #endif
   if (likely(PyLong_CheckExact(b))) {
     #if CYTHON_USE_PYLONG_INTERNALS
     const digit* digits = ((PyLongObject*)b)->ob_digit;
     const Py_ssize_t size = Py_SIZE(b);
     if (likely(__Pyx_sst_abs(size) <= 1)) {
-        ival = likely(size) ? (Py_ssize_t)(digits[0]) : 0;
+        ival = likely(size) ? digits[0] : 0;
         if (size == -1) ival = -ival;
         return ival;
     } else {
       switch (size) {
          case 2:
            if (8 * sizeof(Py_ssize_t) > 2 * PyLong_SHIFT) {
              return (Py_ssize_t) (((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
```

### Comparing `guiqwt-4.3.3/src/histogram2d.pyx` & `guiqwt-4.4.0/src/histogram2d.pyx`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/src/mandelbrot.c` & `guiqwt-4.4.0/src/mandelbrot.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.26 */
+/* Generated by Cython 0.29.32 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_26"
-#define CYTHON_HEX_VERSION 0x001D1AF0
+#define CYTHON_ABI "0_29_32"
+#define CYTHON_HEX_VERSION 0x001D20F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -45,14 +45,15 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -81,18 +82,22 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -122,18 +127,67 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PY_NOGIL)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_PYSTON 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
+  #ifndef CYTHON_USE_TYPE_SLOTS
+    #define CYTHON_USE_TYPE_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_INTERNALS
+    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #endif
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #ifndef CYTHON_ASSUME_SAFE_MACROS
+    #define CYTHON_ASSUME_SAFE_MACROS 1
+  #endif
+  #ifndef CYTHON_UNPACK_METHODS
+    #define CYTHON_UNPACK_METHODS 1
+  #endif
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -168,32 +222,41 @@
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #ifndef CYTHON_FAST_THREAD_STATE
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_FAST_THREAD_STATE
+    #define CYTHON_FAST_THREAD_STATE 0
+  #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030B00A1)
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
     #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
   #endif
-  #ifndef CYTHON_USE_EXC_INFO_STACK
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_USE_EXC_INFO_STACK
+    #define CYTHON_USE_EXC_INFO_STACK 0
+  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
   #if PY_MAJOR_VERSION < 3
     #include "longintrepr.h"
@@ -637,16 +700,18 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(WIN32) || defined(MS_WINDOWS)
-  #define _USE_MATH_DEFINES
+#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
+  #if !defined(_USE_MATH_DEFINES)
+    #define _USE_MATH_DEFINES
+  #endif
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -918,195 +983,195 @@
 
 static const char *__pyx_f[] = {
   "src\\mandelbrot.pyx",
   "__init__.pxd",
   "type.pxd",
 };
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":690
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":691
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":692
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":693
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":697
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":698
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":699
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":700
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":704
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":705
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":714
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":715
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":716
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":718
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":719
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":720
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":722
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":723
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":725
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":726
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":727
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1133,42 +1198,42 @@
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":729
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":730
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":731
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":733
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2082,15 +2147,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":735
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -2099,29 +2164,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":736
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":735
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -2132,15 +2197,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":738
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -2149,29 +2214,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":739
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":738
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -2182,15 +2247,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":741
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -2199,29 +2264,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":742
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":741
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -2232,15 +2297,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":744
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -2249,29 +2314,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":745
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":744
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -2282,15 +2347,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":747
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -2299,29 +2364,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":748
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":747
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -2332,212 +2397,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":750
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":751
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":752
+    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":751
+    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":754
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":750
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":929
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":930
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":931
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":929
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":933
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":934
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":935
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":936
+    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":935
+    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":937
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":933
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":941
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -2553,15 +2618,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":942
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -2569,84 +2634,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":943
+      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":942
+      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":944
+    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":945
+      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 945, __pyx_L5_except_error)
+      __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":942
+    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":941
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -2661,15 +2726,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":947
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -2685,15 +2750,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":948
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -2701,84 +2766,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":949
+      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":948
+      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":950
+    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":951
+      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 951, __pyx_L5_except_error)
+      __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":948
+    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":947
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -2793,15 +2858,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":953
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -2817,15 +2882,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":954
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -2833,84 +2898,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":955
+      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":954
+      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":956
+    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":957
+      /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 957, __pyx_L5_except_error)
+      __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":954
+    /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":953
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -2925,176 +2990,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":967
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":979
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":967
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":982
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":994
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":982
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":997
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":1004
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":997
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":1007
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":1011
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":1007
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":1014
+/* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":1018
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":1014
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -3174,43 +3239,43 @@
   {&__pyx_n_s_x2, __pyx_k_x2, sizeof(__pyx_k_x2), 0, 0, 1, 1},
   {&__pyx_n_s_y1, __pyx_k_y1, sizeof(__pyx_k_y1), 0, 0, 1, 1},
   {&__pyx_n_s_y2, __pyx_k_y2, sizeof(__pyx_k_y2), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 17, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 945, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 944, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":945
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 945, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":951
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 951, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 950, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "mandelbrot.pyx":25
  * 
  * @cython.boundscheck(False)
  * def mandelbrot(double x1, double y1, double x2, double y2,             # <<<<<<<<<<<<<<
@@ -3290,46 +3355,46 @@
   sizeof(PyTypeObject),
   #else
   sizeof(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 200, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 200, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
   __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 223, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
   __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 227, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
   __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 239, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
   __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 771, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
   __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 773, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
   __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 775, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
   __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 777, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
   __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 779, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
   __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 781, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
   __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 783, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
   __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 785, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
   __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 787, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
   __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 789, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
   __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 827, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -3569,15 +3634,15 @@
  * # Copyright (C) 2012 CEA
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../Apps/WPy64-31020/python-3.10.2.amd64/lib/site-packages/numpy/__init__.pxd":1014
+  /* "../../../Apps/WPy64-31110/python-3.11.1.amd64/Lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -4447,14 +4512,20 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
 #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
     PyCodeObject *py_code = NULL;
     PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_srcfile = NULL;
@@ -4510,22 +4581,32 @@
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
+        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) goto bad;
+        if (!py_code) {
+            /* If the code object creation fails, then we should clear the
+               fetched exception references and propagate the new exception */
+            Py_XDECREF(ptype);
+            Py_XDECREF(pvalue);
+            Py_XDECREF(ptraceback);
+            goto bad;
+        }
+        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -5668,19 +5749,41 @@
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
+    char ctversion[5];
+    int same=1, i, found_dot;
+    const char* rt_from_call = Py_GetVersion();
+    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    found_dot = 0;
+    for (i = 0; i < 4; i++) {
+        if (!ctversion[i]) {
+            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
+            break;
+        }
+        if (rt_from_call[i] != ctversion[i]) {
+            same = 0;
+            break;
+        }
+    }
+    if (!same) {
+        char rtversion[5] = {'\0'};
         char message[200];
+        for (i=0; i<4; ++i) {
+            if (rt_from_call[i] == '.') {
+                if (found_dot) break;
+                found_dot = 1;
+            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
+                break;
+            }
+            rtversion[i] = rt_from_call[i];
+        }
         PyOS_snprintf(message, sizeof(message),
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
@@ -5884,15 +5987,15 @@
   }
 #endif
   if (likely(PyLong_CheckExact(b))) {
     #if CYTHON_USE_PYLONG_INTERNALS
     const digit* digits = ((PyLongObject*)b)->ob_digit;
     const Py_ssize_t size = Py_SIZE(b);
     if (likely(__Pyx_sst_abs(size) <= 1)) {
-        ival = likely(size) ? (Py_ssize_t)(digits[0]) : 0;
+        ival = likely(size) ? digits[0] : 0;
         if (size == -1) ival = -ival;
         return ival;
     } else {
       switch (size) {
          case 2:
            if (8 * sizeof(Py_ssize_t) > 2 * PyLong_SHIFT) {
              return (Py_ssize_t) (((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
```

### Comparing `guiqwt-4.3.3/src/mandelbrot.pyx` & `guiqwt-4.4.0/src/mandelbrot.pyx`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/src/pcolor.cpp` & `guiqwt-4.4.0/src/pcolor.cpp`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/src/points.hpp` & `guiqwt-4.4.0/src/points.hpp`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/src/scaler.cpp` & `guiqwt-4.4.0/src/scaler.cpp`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/src/scaler.hpp` & `guiqwt-4.4.0/src/scaler.hpp`

 * *Files identical despite different names*

### Comparing `guiqwt-4.3.3/src/traits.hpp` & `guiqwt-4.4.0/src/traits.hpp`

 * *Files identical despite different names*

