# Comparing `tmp/srsgui-0.4.0.1.tar.gz` & `tmp/srsgui-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-8d6hs4yl\srsgui-0.4.0.1.tar", last modified: Mon Jun 26 20:07:06 2023, max compression
+gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-24fcqa60\srsgui-0.4.1.tar", last modified: Thu Jul  6 00:39:16 2023, max compression
```

## Comparing `srsgui-0.4.0.1.tar` & `srsgui-0.4.1.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.421602 srsgui-0.4.0.1/
-drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.313116 srsgui-0.4.0.1/.github/
-drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.321620 srsgui-0.4.0.1/.github/workflows/
--rw-rw-rw-   0        0        0      388 2023-06-19 18:04:40.000000 srsgui-0.4.0.1/.github/workflows/pages.yml
--rw-rw-rw-   0        0        0     1356 2023-05-16 23:33:10.000000 srsgui-0.4.0.1/.gitignore
--rw-rw-rw-   0        0        0     1113 2023-05-16 18:54:46.000000 srsgui-0.4.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     3967 2023-06-26 20:07:06.421602 srsgui-0.4.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2985 2023-06-19 17:56:19.000000 srsgui-0.4.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.351636 srsgui-0.4.0.1/docs/
--rw-rw-rw-   0        0        0      654 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.371628 srsgui-0.4.0.1/docs/_static/
--rw-rw-rw-   0        0        0    31067 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/docs/_static/cg-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    27242 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/docs/_static/cg-terminal-screen-capture.png
--rw-rw-rw-   0        0        0     5762 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/docs/_static/connect-dialog-box-capture.png
--rw-rw-rw-   0        0        0    88057 2023-06-08 18:01:11.000000 srsgui-0.4.0.1/docs/_static/dock_widget_floating.png
--rw-rw-rw-   0        0        0    97266 2023-06-08 18:01:11.000000 srsgui-0.4.0.1/docs/_static/dock_widgets_expanded.png
--rw-rw-rw-   0        0        0    71070 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/docs/_static/example-screen-capture-1.png
--rw-rw-rw-   0        0        0    71011 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/docs/_static/example-screen-capture-2.png
--rw-rw-rw-   0        0        0    56013 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/docs/_static/initial-screen-capture.png
--rw-rw-rw-   0        0        0    52123 2023-06-08 23:01:31.000000 srsgui-0.4.0.1/docs/_static/lockin-capture.png
--rw-rw-rw-   0        0        0    29667 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/docs/_static/osc-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    50740 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/docs/_static/second-task-screen-capture.png
--rw-rw-rw-   0        0        0    38581 2023-06-08 18:01:11.000000 srsgui-0.4.0.1/docs/_static/task_selection.png
--rw-rw-rw-   0        0        0    39412 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/docs/_static/terminal-with-example-2.png
--rw-rw-rw-   0        0        0    37573 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/docs/_static/terminal-with-example.png
--rw-rw-rw-   0        0        0     8513 2023-06-15 00:44:23.000000 srsgui-0.4.0.1/docs/application.rst
--rw-rw-rw-   0        0        0      840 2023-06-26 20:05:20.000000 srsgui-0.4.0.1/docs/changelog.rst
--rw-rw-rw-   0        0        0     1924 2023-06-08 18:01:11.000000 srsgui-0.4.0.1/docs/conf.py
--rw-rw-rw-   0        0        0     6097 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/docs/create-project.rst
--rw-rw-rw-   0        0        0     6656 2023-06-08 23:01:31.000000 srsgui-0.4.0.1/docs/create-task.rst
--rw-rw-rw-   0        0        0     6112 2023-06-08 23:01:31.000000 srsgui-0.4.0.1/docs/define-instrument.rst
--rw-rw-rw-   0        0        0    15640 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/docs/example.rst
--rw-rw-rw-   0        0        0     3803 2023-06-15 00:44:23.000000 srsgui-0.4.0.1/docs/index.rst
--rw-rw-rw-   0        0        0     4405 2023-06-15 00:44:23.000000 srsgui-0.4.0.1/docs/installation.rst
--rwxrwxrwx   0        0        0      802 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/docs/make.bat
--rw-rw-rw-   0        0        0       34 2023-05-16 19:47:28.000000 srsgui-0.4.0.1/docs/requirements..txt
--rw-rw-rw-   0        0        0      936 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/docs/srsgui.inst.communications.rst
--rw-rw-rw-   0        0        0      930 2023-06-08 18:01:11.000000 srsgui-0.4.0.1/docs/srsgui.inst.rst
--rw-rw-rw-   0        0        0      113 2023-05-24 20:30:53.000000 srsgui-0.4.0.1/docs/srsgui.rst
--rw-rw-rw-   0        0        0     1077 2023-05-24 20:30:53.000000 srsgui-0.4.0.1/docs/srsgui.task.rst
--rw-rw-rw-   0        0        0     2065 2023-05-24 20:30:53.000000 srsgui-0.4.0.1/docs/srsgui.ui.commandtree.rst
--rw-rw-rw-   0        0        0      603 2023-05-24 20:30:53.000000 srsgui-0.4.0.1/docs/srsgui.ui.qt.rst
--rw-rw-rw-   0        0        0     1646 2023-05-24 20:30:53.000000 srsgui-0.4.0.1/docs/srsgui.ui.rst
--rw-rw-rw-   0        0        0     1101 2023-06-23 17:22:50.000000 srsgui-0.4.0.1/docs/troubleshooting.rst
--rw-rw-rw-   0        0        0     1489 2023-06-15 00:44:23.000000 srsgui-0.4.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.4.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 20:07:06.421602 srsgui-0.4.0.1/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsgui-0.4.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.371628 srsgui-0.4.0.1/srsgui/
--rw-rw-rw-   0        0        0     1539 2023-06-26 20:05:20.000000 srsgui-0.4.0.1/srsgui/__init__.py
--rw-rw-rw-   0        0        0      314 2023-05-15 21:54:54.000000 srsgui-0.4.0.1/srsgui/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.313116 srsgui-0.4.0.1/srsgui/examples/
-drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.371628 srsgui-0.4.0.1/srsgui/examples/oscilloscope example/
-drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.381591 srsgui-0.4.0.1/srsgui/examples/oscilloscope example/instruments/
--rw-rw-rw-   0        0        0     1828 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/examples/oscilloscope example/instruments/cg635.py
--rw-rw-rw-   0        0        0     3146 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/examples/oscilloscope example/instruments/sds1202.py
--rw-rw-rw-   0        0        0     1977 2023-06-19 17:56:19.000000 srsgui-0.4.0.1/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
-drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.381591 srsgui-0.4.0.1/srsgui/examples/oscilloscope example/tasks/
--rw-rw-rw-   0        0        0     2522 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/examples/oscilloscope example/tasks/fifth.py
--rw-rw-rw-   0        0        0     1662 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/examples/oscilloscope example/tasks/first.py
--rw-rw-rw-   0        0        0     4099 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/examples/oscilloscope example/tasks/fourth.py
--rw-rw-rw-   0        0        0     2250 2023-06-19 17:56:19.000000 srsgui-0.4.0.1/srsgui/examples/oscilloscope example/tasks/second.py
--rw-rw-rw-   0        0        0     2014 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/examples/oscilloscope example/tasks/third.py
-drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.391610 srsgui-0.4.0.1/srsgui/inst/
--rw-rw-rw-   0        0        0     1074 2023-05-15 21:54:54.000000 srsgui-0.4.0.1/srsgui/inst/__init__.py
--rw-rw-rw-   0        0        0     9907 2023-05-24 20:30:53.000000 srsgui-0.4.0.1/srsgui/inst/commands.py
-drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.391610 srsgui-0.4.0.1/srsgui/inst/communications/
--rw-rw-rw-   0        0        0      126 2023-05-15 21:54:54.000000 srsgui-0.4.0.1/srsgui/inst/communications/__init__.py
--rw-rw-rw-   0        0        0     8308 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/inst/communications/interface.py
--rw-rw-rw-   0        0        0     1276 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/inst/communications/serial_ports.py
--rw-rw-rw-   0        0        0     8774 2023-06-23 17:22:50.000000 srsgui-0.4.0.1/srsgui/inst/communications/serialinterface.py
--rw-rw-rw-   0        0        0    11333 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/inst/communications/tcpipinterface.py
--rw-rw-rw-   0        0        0    19291 2023-06-23 17:22:50.000000 srsgui-0.4.0.1/srsgui/inst/component.py
--rw-rw-rw-   0        0        0      844 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/inst/exceptions.py
--rw-rw-rw-   0        0        0    10410 2023-05-24 20:30:53.000000 srsgui-0.4.0.1/srsgui/inst/indexcommands.py
--rw-rw-rw-   0        0        0     9990 2023-06-19 18:04:40.000000 srsgui-0.4.0.1/srsgui/inst/instrument.py
-drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.401611 srsgui-0.4.0.1/srsgui/task/
--rw-rw-rw-   0        0        0        2 2023-05-15 21:54:54.000000 srsgui-0.4.0.1/srsgui/task/__init__.py
--rw-rw-rw-   0        0        0      811 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/task/callbacks.py
--rw-rw-rw-   0        0        0     6989 2023-06-21 20:11:21.000000 srsgui-0.4.0.1/srsgui/task/config.py
--rw-rw-rw-   0        0        0     5856 2023-06-21 20:11:21.000000 srsgui-0.4.0.1/srsgui/task/inputs.py
--rw-rw-rw-   0        0        0     6938 2023-05-24 20:30:53.000000 srsgui-0.4.0.1/srsgui/task/sessionhandler.py
--rw-rw-rw-   0        0        0    23469 2023-06-08 18:01:11.000000 srsgui-0.4.0.1/srsgui/task/task.py
--rw-rw-rw-   0        0        0     4225 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/task/taskresult.py
-drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.411601 srsgui-0.4.0.1/srsgui/ui/
--rw-rw-rw-   0        0        0        0 2023-05-15 21:54:55.000000 srsgui-0.4.0.1/srsgui/ui/__init__.py
--rw-rw-rw-   0        0        0     3894 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/ui/commandhandler.py
--rw-rw-rw-   0        0        0     6880 2023-05-24 20:30:53.000000 srsgui-0.4.0.1/srsgui/ui/commandterminal.py
-drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.421602 srsgui-0.4.0.1/srsgui/ui/commandtree/
--rw-rw-rw-   0        0        0        0 2023-05-19 00:30:39.000000 srsgui-0.4.0.1/srsgui/ui/commandtree/__init__.py
--rw-rw-rw-   0        0        0     3941 2023-05-23 19:11:06.000000 srsgui-0.4.0.1/srsgui/ui/commandtree/commanddelegate.py
--rw-rw-rw-   0        0        0     1603 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/ui/commandtree/commandhandler.py
--rw-rw-rw-   0        0        0    12605 2023-06-23 17:22:50.000000 srsgui-0.4.0.1/srsgui/ui/commandtree/commanditem.py
--rw-rw-rw-   0        0        0     8669 2023-05-24 20:30:53.000000 srsgui-0.4.0.1/srsgui/ui/commandtree/commandmodel.py
--rw-rw-rw-   0        0        0     5109 2023-05-24 20:30:53.000000 srsgui-0.4.0.1/srsgui/ui/commandtree/commandspinbox.py
--rw-rw-rw-   0        0        0     3452 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/ui/commandtree/commandtreeview.py
--rw-rw-rw-   0        0        0     4852 2023-06-19 18:04:40.000000 srsgui-0.4.0.1/srsgui/ui/commandtree/commandtreewidget.py
--rw-rw-rw-   0        0        0     4806 2023-05-15 21:54:55.000000 srsgui-0.4.0.1/srsgui/ui/commandtree/ui_commandtreewidget.py
--rw-rw-rw-   0        0        0     9798 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/ui/connectdlg.py
--rw-rw-rw-   0        0        0     3975 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/ui/deviceinfohandler.py
--rw-rw-rw-   0        0        0    15880 2023-06-08 18:01:11.000000 srsgui-0.4.0.1/srsgui/ui/dockhandler.py
--rw-rw-rw-   0        0        0    14950 2023-06-21 20:11:21.000000 srsgui-0.4.0.1/srsgui/ui/inputpanel.py
-drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.421602 srsgui-0.4.0.1/srsgui/ui/qt/
--rw-rw-rw-   0        0        0      799 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/ui/qt/QtCore.py
--rw-rw-rw-   0        0        0      677 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/ui/qt/QtGui.py
--rw-rw-rw-   0        0        0      777 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/ui/qt/QtWidgets.py
--rw-rw-rw-   0        0        0     1449 2023-05-24 20:30:53.000000 srsgui-0.4.0.1/srsgui/ui/qt/__init__.py
--rw-rw-rw-   0        0        0     1285 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/ui/qtloghandler.py
--rw-rw-rw-   0        0        0      268 2023-05-15 21:54:55.000000 srsgui-0.4.0.1/srsgui/ui/resource.qrc
--rw-rw-rw-   0        0        0    15479 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/ui/resource_rc.py
--rw-rw-rw-   0        0        0     2717 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/ui/signalhandler.py
--rw-rw-rw-   0        0        0    47891 2023-05-15 21:54:55.000000 srsgui-0.4.0.1/srsgui/ui/srslogo.jpg
--rw-rw-rw-   0        0        0     1005 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/ui/stdout.py
--rw-rw-rw-   0        0        0    26550 2023-06-26 20:05:20.000000 srsgui-0.4.0.1/srsgui/ui/taskmain.py
--rw-rw-rw-   0        0        0    10403 2023-05-15 21:54:55.000000 srsgui-0.4.0.1/srsgui/ui/taskmain.ui
--rw-rw-rw-   0        0        0    11293 2023-05-15 21:54:55.000000 srsgui-0.4.0.1/srsgui/ui/ui_taskmain.py
-drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.371628 srsgui-0.4.0.1/srsgui.egg-info/
--rw-rw-rw-   0        0        0     3967 2023-06-26 20:07:06.000000 srsgui-0.4.0.1/srsgui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3170 2023-06-26 20:07:06.000000 srsgui-0.4.0.1/srsgui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 20:07:06.000000 srsgui-0.4.0.1/srsgui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-06-26 20:07:06.000000 srsgui-0.4.0.1/srsgui.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      103 2023-06-26 20:07:06.000000 srsgui-0.4.0.1/srsgui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-26 20:07:06.000000 srsgui-0.4.0.1/srsgui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.473875 srsgui-0.4.1/
+drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.317450 srsgui-0.4.1/.github/
+drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.327688 srsgui-0.4.1/.github/workflows/
+-rw-rw-rw-   0        0        0      388 2023-06-19 18:04:40.000000 srsgui-0.4.1/.github/workflows/pages.yml
+-rw-rw-rw-   0        0        0     1356 2023-05-16 23:33:10.000000 srsgui-0.4.1/.gitignore
+-rw-rw-rw-   0        0        0     1113 2023-05-16 18:54:46.000000 srsgui-0.4.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     4047 2023-07-06 00:39:16.467606 srsgui-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3068 2023-06-27 19:21:08.000000 srsgui-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.352532 srsgui-0.4.1/docs/
+-rw-rw-rw-   0        0        0      654 2023-05-16 18:43:29.000000 srsgui-0.4.1/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.372521 srsgui-0.4.1/docs/_static/
+-rw-rw-rw-   0        0        0    31067 2023-05-16 18:43:29.000000 srsgui-0.4.1/docs/_static/cg-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    27242 2023-05-16 18:43:29.000000 srsgui-0.4.1/docs/_static/cg-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0     5762 2023-05-16 18:43:29.000000 srsgui-0.4.1/docs/_static/connect-dialog-box-capture.png
+-rw-rw-rw-   0        0        0    88057 2023-06-08 18:01:11.000000 srsgui-0.4.1/docs/_static/dock_widget_floating.png
+-rw-rw-rw-   0        0        0    97266 2023-06-08 18:01:11.000000 srsgui-0.4.1/docs/_static/dock_widgets_expanded.png
+-rw-rw-rw-   0        0        0    71070 2023-05-16 18:43:29.000000 srsgui-0.4.1/docs/_static/example-screen-capture-1.png
+-rw-rw-rw-   0        0        0    71011 2023-05-16 18:43:29.000000 srsgui-0.4.1/docs/_static/example-screen-capture-2.png
+-rw-rw-rw-   0        0        0    56013 2023-05-16 18:43:29.000000 srsgui-0.4.1/docs/_static/initial-screen-capture.png
+-rw-rw-rw-   0        0        0    52123 2023-06-08 23:01:31.000000 srsgui-0.4.1/docs/_static/lockin-capture.png
+-rw-rw-rw-   0        0        0    29667 2023-05-16 18:43:29.000000 srsgui-0.4.1/docs/_static/osc-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    50740 2023-05-16 18:43:29.000000 srsgui-0.4.1/docs/_static/second-task-screen-capture.png
+-rw-rw-rw-   0        0        0    38581 2023-06-08 18:01:11.000000 srsgui-0.4.1/docs/_static/task_selection.png
+-rw-rw-rw-   0        0        0    39412 2023-05-16 18:43:29.000000 srsgui-0.4.1/docs/_static/terminal-with-example-2.png
+-rw-rw-rw-   0        0        0    37573 2023-05-16 18:43:29.000000 srsgui-0.4.1/docs/_static/terminal-with-example.png
+-rw-rw-rw-   0        0        0     8703 2023-06-27 19:21:08.000000 srsgui-0.4.1/docs/application.rst
+-rw-rw-rw-   0        0        0      840 2023-06-26 20:05:20.000000 srsgui-0.4.1/docs/changelog.rst
+-rw-rw-rw-   0        0        0     1921 2023-06-29 20:28:19.000000 srsgui-0.4.1/docs/conf.py
+-rw-rw-rw-   0        0        0     6261 2023-07-06 00:33:39.000000 srsgui-0.4.1/docs/create-project.rst
+-rw-rw-rw-   0        0        0     7546 2023-06-29 20:28:19.000000 srsgui-0.4.1/docs/create-task.rst
+-rw-rw-rw-   0        0        0     6547 2023-06-29 20:28:19.000000 srsgui-0.4.1/docs/define-instrument.rst
+-rw-rw-rw-   0        0        0    16624 2023-06-27 19:21:08.000000 srsgui-0.4.1/docs/example.rst
+-rw-rw-rw-   0        0        0     3803 2023-06-15 00:44:23.000000 srsgui-0.4.1/docs/index.rst
+-rw-rw-rw-   0        0        0     4539 2023-06-27 19:21:08.000000 srsgui-0.4.1/docs/installation.rst
+-rwxrwxrwx   0        0        0      802 2023-05-16 18:43:29.000000 srsgui-0.4.1/docs/make.bat
+-rw-rw-rw-   0        0        0       34 2023-05-16 19:47:28.000000 srsgui-0.4.1/docs/requirements..txt
+-rw-rw-rw-   0        0        0      936 2023-05-16 18:43:29.000000 srsgui-0.4.1/docs/srsgui.inst.communications.rst
+-rw-rw-rw-   0        0        0      930 2023-06-08 18:01:11.000000 srsgui-0.4.1/docs/srsgui.inst.rst
+-rw-rw-rw-   0        0        0      113 2023-05-24 20:30:53.000000 srsgui-0.4.1/docs/srsgui.rst
+-rw-rw-rw-   0        0        0     1077 2023-05-24 20:30:53.000000 srsgui-0.4.1/docs/srsgui.task.rst
+-rw-rw-rw-   0        0        0     2065 2023-05-24 20:30:53.000000 srsgui-0.4.1/docs/srsgui.ui.commandtree.rst
+-rw-rw-rw-   0        0        0      603 2023-05-24 20:30:53.000000 srsgui-0.4.1/docs/srsgui.ui.qt.rst
+-rw-rw-rw-   0        0        0     1646 2023-05-24 20:30:53.000000 srsgui-0.4.1/docs/srsgui.ui.rst
+-rw-rw-rw-   0        0        0     1101 2023-06-23 17:22:50.000000 srsgui-0.4.1/docs/troubleshooting.rst
+-rw-rw-rw-   0        0        0     1488 2023-07-06 00:33:39.000000 srsgui-0.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.4.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 00:39:16.473875 srsgui-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsgui-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.382514 srsgui-0.4.1/srsgui/
+-rw-rw-rw-   0        0        0     1537 2023-07-06 00:38:03.000000 srsgui-0.4.1/srsgui/__init__.py
+-rw-rw-rw-   0        0        0      314 2023-05-15 21:54:54.000000 srsgui-0.4.1/srsgui/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.325684 srsgui-0.4.1/srsgui/examples/
+drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.382514 srsgui-0.4.1/srsgui/examples/oscilloscope example/
+drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.392509 srsgui-0.4.1/srsgui/examples/oscilloscope example/instruments/
+-rw-rw-rw-   0        0        0     1828 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/examples/oscilloscope example/instruments/cg635.py
+-rw-rw-rw-   0        0        0     3146 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/examples/oscilloscope example/instruments/sds1202.py
+-rw-rw-rw-   0        0        0     1960 2023-06-27 19:21:08.000000 srsgui-0.4.1/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
+drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.392509 srsgui-0.4.1/srsgui/examples/oscilloscope example/tasks/
+-rw-rw-rw-   0        0        0     2522 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/examples/oscilloscope example/tasks/fifth.py
+-rw-rw-rw-   0        0        0     1662 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/examples/oscilloscope example/tasks/first.py
+-rw-rw-rw-   0        0        0     4099 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/examples/oscilloscope example/tasks/fourth.py
+-rw-rw-rw-   0        0        0     2583 2023-06-27 19:21:08.000000 srsgui-0.4.1/srsgui/examples/oscilloscope example/tasks/second.py
+-rw-rw-rw-   0        0        0     2014 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/examples/oscilloscope example/tasks/third.py
+drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.402504 srsgui-0.4.1/srsgui/inst/
+-rw-rw-rw-   0        0        0     1074 2023-05-15 21:54:54.000000 srsgui-0.4.1/srsgui/inst/__init__.py
+-rw-rw-rw-   0        0        0     9907 2023-05-24 20:30:53.000000 srsgui-0.4.1/srsgui/inst/commands.py
+drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.412499 srsgui-0.4.1/srsgui/inst/communications/
+-rw-rw-rw-   0        0        0      126 2023-05-15 21:54:54.000000 srsgui-0.4.1/srsgui/inst/communications/__init__.py
+-rw-rw-rw-   0        0        0     8308 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/inst/communications/interface.py
+-rw-rw-rw-   0        0        0     1276 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/inst/communications/serial_ports.py
+-rw-rw-rw-   0        0        0     8774 2023-06-23 17:22:50.000000 srsgui-0.4.1/srsgui/inst/communications/serialinterface.py
+-rw-rw-rw-   0        0        0    11333 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/inst/communications/tcpipinterface.py
+-rw-rw-rw-   0        0        0    19291 2023-06-23 17:22:50.000000 srsgui-0.4.1/srsgui/inst/component.py
+-rw-rw-rw-   0        0        0      844 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/inst/exceptions.py
+-rw-rw-rw-   0        0        0    10410 2023-05-24 20:30:53.000000 srsgui-0.4.1/srsgui/inst/indexcommands.py
+-rw-rw-rw-   0        0        0     9990 2023-06-19 18:04:40.000000 srsgui-0.4.1/srsgui/inst/instrument.py
+drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.427623 srsgui-0.4.1/srsgui/task/
+-rw-rw-rw-   0        0        0        2 2023-05-15 21:54:54.000000 srsgui-0.4.1/srsgui/task/__init__.py
+-rw-rw-rw-   0        0        0     1192 2023-06-27 19:21:08.000000 srsgui-0.4.1/srsgui/task/callbacks.py
+-rw-rw-rw-   0        0        0     6989 2023-06-21 20:11:21.000000 srsgui-0.4.1/srsgui/task/config.py
+-rw-rw-rw-   0        0        0     5856 2023-06-21 20:11:21.000000 srsgui-0.4.1/srsgui/task/inputs.py
+-rw-rw-rw-   0        0        0     6938 2023-05-24 20:30:53.000000 srsgui-0.4.1/srsgui/task/sessionhandler.py
+-rw-rw-rw-   0        0        0    25859 2023-06-29 20:28:19.000000 srsgui-0.4.1/srsgui/task/task.py
+-rw-rw-rw-   0        0        0     4225 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/task/taskresult.py
+drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.447616 srsgui-0.4.1/srsgui/ui/
+-rw-rw-rw-   0        0        0        0 2023-05-15 21:54:55.000000 srsgui-0.4.1/srsgui/ui/__init__.py
+-rw-rw-rw-   0        0        0     3894 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/ui/commandhandler.py
+-rw-rw-rw-   0        0        0     6880 2023-05-24 20:30:53.000000 srsgui-0.4.1/srsgui/ui/commandterminal.py
+drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.457636 srsgui-0.4.1/srsgui/ui/commandtree/
+-rw-rw-rw-   0        0        0        0 2023-05-19 00:30:39.000000 srsgui-0.4.1/srsgui/ui/commandtree/__init__.py
+-rw-rw-rw-   0        0        0     3941 2023-05-23 19:11:06.000000 srsgui-0.4.1/srsgui/ui/commandtree/commanddelegate.py
+-rw-rw-rw-   0        0        0     1603 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/ui/commandtree/commandhandler.py
+-rw-rw-rw-   0        0        0    12605 2023-06-23 17:22:50.000000 srsgui-0.4.1/srsgui/ui/commandtree/commanditem.py
+-rw-rw-rw-   0        0        0     8669 2023-05-24 20:30:53.000000 srsgui-0.4.1/srsgui/ui/commandtree/commandmodel.py
+-rw-rw-rw-   0        0        0     5109 2023-05-24 20:30:53.000000 srsgui-0.4.1/srsgui/ui/commandtree/commandspinbox.py
+-rw-rw-rw-   0        0        0     3452 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/ui/commandtree/commandtreeview.py
+-rw-rw-rw-   0        0        0     4852 2023-06-19 18:04:40.000000 srsgui-0.4.1/srsgui/ui/commandtree/commandtreewidget.py
+-rw-rw-rw-   0        0        0     4806 2023-05-15 21:54:55.000000 srsgui-0.4.1/srsgui/ui/commandtree/ui_commandtreewidget.py
+-rw-rw-rw-   0        0        0     9796 2023-06-27 19:21:08.000000 srsgui-0.4.1/srsgui/ui/connectdlg.py
+-rw-rw-rw-   0        0        0     3975 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/ui/deviceinfohandler.py
+-rw-rw-rw-   0        0        0    15880 2023-06-08 18:01:11.000000 srsgui-0.4.1/srsgui/ui/dockhandler.py
+-rw-rw-rw-   0        0        0    14950 2023-06-27 19:15:07.000000 srsgui-0.4.1/srsgui/ui/inputpanel.py
+drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.467606 srsgui-0.4.1/srsgui/ui/qt/
+-rw-rw-rw-   0        0        0      799 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/ui/qt/QtCore.py
+-rw-rw-rw-   0        0        0      677 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/ui/qt/QtGui.py
+-rw-rw-rw-   0        0        0      777 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/ui/qt/QtWidgets.py
+-rw-rw-rw-   0        0        0     1449 2023-05-24 20:30:53.000000 srsgui-0.4.1/srsgui/ui/qt/__init__.py
+-rw-rw-rw-   0        0        0     1285 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/ui/qtloghandler.py
+-rw-rw-rw-   0        0        0      268 2023-05-15 21:54:55.000000 srsgui-0.4.1/srsgui/ui/resource.qrc
+-rw-rw-rw-   0        0        0    15479 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/ui/resource_rc.py
+-rw-rw-rw-   0        0        0     2717 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/ui/signalhandler.py
+-rw-rw-rw-   0        0        0    47891 2023-05-15 21:54:55.000000 srsgui-0.4.1/srsgui/ui/srslogo.jpg
+-rw-rw-rw-   0        0        0     1005 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/ui/stdout.py
+-rw-rw-rw-   0        0        0    26550 2023-06-26 20:05:20.000000 srsgui-0.4.1/srsgui/ui/taskmain.py
+-rw-rw-rw-   0        0        0    10403 2023-05-15 21:54:55.000000 srsgui-0.4.1/srsgui/ui/taskmain.ui
+-rw-rw-rw-   0        0        0    11293 2023-05-15 21:54:55.000000 srsgui-0.4.1/srsgui/ui/ui_taskmain.py
+drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.382514 srsgui-0.4.1/srsgui.egg-info/
+-rw-rw-rw-   0        0        0     4047 2023-07-06 00:39:16.000000 srsgui-0.4.1/srsgui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3170 2023-07-06 00:39:16.000000 srsgui-0.4.1/srsgui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 00:39:16.000000 srsgui-0.4.1/srsgui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-06 00:39:16.000000 srsgui-0.4.1/srsgui.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      103 2023-07-06 00:39:16.000000 srsgui-0.4.1/srsgui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-06 00:39:16.000000 srsgui-0.4.1/srsgui.egg-info/top_level.txt
```

### Comparing `srsgui-0.4.0.1/.gitignore` & `srsgui-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/LICENSE.txt` & `srsgui-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/PKG-INFO` & `srsgui-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.4.0.1
+Version: 0.4.1
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Project-URL: homepage, https://github.com/thinkSRS/srsgui
 Project-URL: repository, https://github.com/thinkSRS/srsgui.git
 Project-URL: documentation, https://thinksrs.github.io/srsgui
 Project-URL: changelog, https://thinksrs.github.io/srsgui/changelog.html
 Keywords: instrument control,data acquisition,data visualization
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
@@ -23,74 +23,69 @@
 License-File: LICENSE.txt
 
 # ``Srsgui`` - Organize instrument-controlling Python scripts as a GUI application
 
 `Srsgui` is a simple framework:
 
    - To define instrument classes for instruments that use remote communication,
-     based on `Instrument` class and the communication `Interface` class 
-     (By default, serial and TCPIP is available. VXI11, GPIB and USB-TMC are optional.).
+     based on the `Instrument` class and the communication `Interface` class. 
+     (By default, serial and TCPIP is available. VXI11, GPIB and USB-TMC are optional).
 
    - To write Python scripts (tasks) that run in GUI environment with simple APIs
      provided in ``Task`` class.
 
    - To organize instrument classes and task scripts presented in a GUI application
-     using a configuration (.taskconfig) file for a project
+     using a configuration (.taskconfig) file for a project.
 
 ![screenshot](https://thinksrs.github.io/srsgui/_images/example-screen-capture-2.png " ")
 
 ## Installation
 
 To run ``srsgui`` as an application, create a virtual environment, if necessary, 
-and install using ``pip`` with [full] option:  
+and install using ``pip`` with the `[full]` option:  
 
     python -m pip install srsgui[full]
 
 ``Srsgui`` package has the following 3 main dependencies: 
 [pyserial](https://pypi.org/project/pyserial/), 
 [matplotlib](https://pypi.org/project/matplotlib/) and
 [PySide6](https://pypi.org/project/PySide6/). If the installation above fails, 
 you have to install the failed pacakge manually. Using a virtual environment will
 eliminate possible conflicts between packages in the main Python installation and 
-the packagesSome used in `srsgui`. Some Linux distributions offer 
-some of the Python packages from their repositories only, not from ``pip``. 
-Run web search for more information on system-specific installation.   
-
-Once pyserial, matplotlib and PySide6 are installed properly, or you plan to use
-`srsgui` for instrument drivers only without GUI support, 
-you can install ``srsgui`` without [full] option:
+the packages. Some Linux distributions offer certain Python packages from their repositories only (i.e. not from ``pip``). 
+Run a web search for more information on system-specific installation.   
+
+Once pyserial, matplotlib and PySide6 are installed properly, or if you plan to use `srsgui` for instrument drivers only without GUI support, 
+you can install ``srsgui`` without the `[full]` option:
 
     python -m pip install srsgui
 
 ## Start ``srsgui`` application
     
-if the Python Script directory is in PATH environment variable,
-Start the application by typing from the command line:
+If the Python Script directory is in the PATH environment variable,
+launch the application by typing the module name into the command line:
 
     srsgui
 
 If the script directory is not in PATH, run the srsgui module with Python. 
 
     python -m srsgui
-    
-It will start `srsgui` application.
+
 
 ## Run the example project
 
-By default, `srsgui` application starts with the last project it ran,
-when it is closed.
+By default, the `srsgui` application starts with the project that was running when it was last closed.
  
-To open the example project included in the `srsgui` package 
-(if `srsgui` does not start with the example project), select the menu/File/Open config, 
-go to the `srsgui` package directory, find the examples directory, and find a .taskconfig file
+To open the **oscilloscope example project** included in the `srsgui` package 
+(if `srsgui` does not start with the example project), select File/Open config, 
+go to the `srsgui` package directory, find the examples directory, and select the `oscilloscope example project.taskconfig` file
 in the example project folder. 
 
-You can run the second and fifth task in the Task menu 
-even without any instruments connected.
+You can run the **Plot example** and **FFT of simulated waveform** tasks from the Task menu without any instruments connected.
 
 ## Create a project
 
-`Srsgui` is a framework to helps you to write your own instrument-controlling 
-Python scripts running as a GUI application. Using its APIs, you can write 
-scripts running in GUI with the same amount of code with writing console-based 
-scripts. For programming API, refer to
+`Srsgui` is a framework to help you to write your own instrument-controlling 
+Python scripts and run them from a GUI application. Using its APIs, you can write 
+scripts running in GUI with the same amount of code as writing console-based 
+scripts. For programming using the API, refer to the
 [`srsgui` documentation](https://thinksrs.github.io/srsgui).
```

### Comparing `srsgui-0.4.0.1/README.md` & `srsgui-0.4.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,72 +1,67 @@
 # ``Srsgui`` - Organize instrument-controlling Python scripts as a GUI application
 
 `Srsgui` is a simple framework:
 
    - To define instrument classes for instruments that use remote communication,
-     based on `Instrument` class and the communication `Interface` class 
-     (By default, serial and TCPIP is available. VXI11, GPIB and USB-TMC are optional.).
+     based on the `Instrument` class and the communication `Interface` class. 
+     (By default, serial and TCPIP is available. VXI11, GPIB and USB-TMC are optional).
 
    - To write Python scripts (tasks) that run in GUI environment with simple APIs
      provided in ``Task`` class.
 
    - To organize instrument classes and task scripts presented in a GUI application
-     using a configuration (.taskconfig) file for a project
+     using a configuration (.taskconfig) file for a project.
 
 ![screenshot](https://thinksrs.github.io/srsgui/_images/example-screen-capture-2.png " ")
 
 ## Installation
 
 To run ``srsgui`` as an application, create a virtual environment, if necessary, 
-and install using ``pip`` with [full] option:  
+and install using ``pip`` with the `[full]` option:  
 
     python -m pip install srsgui[full]
 
 ``Srsgui`` package has the following 3 main dependencies: 
 [pyserial](https://pypi.org/project/pyserial/), 
 [matplotlib](https://pypi.org/project/matplotlib/) and
 [PySide6](https://pypi.org/project/PySide6/). If the installation above fails, 
 you have to install the failed pacakge manually. Using a virtual environment will
 eliminate possible conflicts between packages in the main Python installation and 
-the packagesSome used in `srsgui`. Some Linux distributions offer 
-some of the Python packages from their repositories only, not from ``pip``. 
-Run web search for more information on system-specific installation.   
-
-Once pyserial, matplotlib and PySide6 are installed properly, or you plan to use
-`srsgui` for instrument drivers only without GUI support, 
-you can install ``srsgui`` without [full] option:
+the packages. Some Linux distributions offer certain Python packages from their repositories only (i.e. not from ``pip``). 
+Run a web search for more information on system-specific installation.   
+
+Once pyserial, matplotlib and PySide6 are installed properly, or if you plan to use `srsgui` for instrument drivers only without GUI support, 
+you can install ``srsgui`` without the `[full]` option:
 
     python -m pip install srsgui
 
 ## Start ``srsgui`` application
     
-if the Python Script directory is in PATH environment variable,
-Start the application by typing from the command line:
+If the Python Script directory is in the PATH environment variable,
+launch the application by typing the module name into the command line:
 
     srsgui
 
 If the script directory is not in PATH, run the srsgui module with Python. 
 
     python -m srsgui
-    
-It will start `srsgui` application.
+
 
 ## Run the example project
 
-By default, `srsgui` application starts with the last project it ran,
-when it is closed.
+By default, the `srsgui` application starts with the project that was running when it was last closed.
  
-To open the example project included in the `srsgui` package 
-(if `srsgui` does not start with the example project), select the menu/File/Open config, 
-go to the `srsgui` package directory, find the examples directory, and find a .taskconfig file
+To open the **oscilloscope example project** included in the `srsgui` package 
+(if `srsgui` does not start with the example project), select File/Open config, 
+go to the `srsgui` package directory, find the examples directory, and select the `oscilloscope example project.taskconfig` file
 in the example project folder. 
 
-You can run the second and fifth task in the Task menu 
-even without any instruments connected.
+You can run the **Plot example** and **FFT of simulated waveform** tasks from the Task menu without any instruments connected.
 
 ## Create a project
 
-`Srsgui` is a framework to helps you to write your own instrument-controlling 
-Python scripts running as a GUI application. Using its APIs, you can write 
-scripts running in GUI with the same amount of code with writing console-based 
-scripts. For programming API, refer to
+`Srsgui` is a framework to help you to write your own instrument-controlling 
+Python scripts and run them from a GUI application. Using its APIs, you can write 
+scripts running in GUI with the same amount of code as writing console-based 
+scripts. For programming using the API, refer to the
 [`srsgui` documentation](https://thinksrs.github.io/srsgui).
```

### Comparing `srsgui-0.4.0.1/docs/Makefile` & `srsgui-0.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/docs/_static/cg-dir-terminal-screen-capture.png` & `srsgui-0.4.1/docs/_static/cg-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/docs/_static/cg-terminal-screen-capture.png` & `srsgui-0.4.1/docs/_static/cg-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/docs/_static/connect-dialog-box-capture.png` & `srsgui-0.4.1/docs/_static/connect-dialog-box-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/docs/_static/dock_widget_floating.png` & `srsgui-0.4.1/docs/_static/dock_widget_floating.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/docs/_static/dock_widgets_expanded.png` & `srsgui-0.4.1/docs/_static/dock_widgets_expanded.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/docs/_static/example-screen-capture-1.png` & `srsgui-0.4.1/docs/_static/example-screen-capture-1.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/docs/_static/example-screen-capture-2.png` & `srsgui-0.4.1/docs/_static/example-screen-capture-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/docs/_static/initial-screen-capture.png` & `srsgui-0.4.1/docs/_static/initial-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/docs/_static/lockin-capture.png` & `srsgui-0.4.1/docs/_static/lockin-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/docs/_static/osc-dir-terminal-screen-capture.png` & `srsgui-0.4.1/docs/_static/osc-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/docs/_static/second-task-screen-capture.png` & `srsgui-0.4.1/docs/_static/second-task-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/docs/_static/task_selection.png` & `srsgui-0.4.1/docs/_static/task_selection.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/docs/_static/terminal-with-example-2.png` & `srsgui-0.4.1/docs/_static/terminal-with-example-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/docs/_static/terminal-with-example.png` & `srsgui-0.4.1/docs/_static/terminal-with-example.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/docs/application.rst` & `srsgui-0.4.1/docs/application.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,64 @@
 Running ``srsgui`` application
 ================================
 
 Starting ``srsgui`` application
 ---------------------------------
 
-With proper installation, you can start ``srsgui`` application by typing
-one of the following commands from the command prompt.
+Following proper installation, you can launch the ``srsgui`` application by typing
+one of the following commands into a command prompt.
 If you installed it with a virtual environment, activate the virtual environment
-before stating ``srsgui``.
+before starting ``srsgui``.
 
 .. code-block::
 
     # If python/script directory is in PATH setting,
     srsgui
     
     # If not, 
     python -m srsgui
 
-The initial window looks like the :ref:`image <top-of-initial-screen-capture>`
-in the previous page, if ``Srsgui`` is started with the default example project. 
+On initial launch, the GUI window will load the default example project,
+and look like this: :ref:`image <top-of-initial-screen-capture>`.
 
 Selecting a configuration file 
 -------------------------------
 
-``Srsgui`` application starts, loading the last configuration file it used.
+When the ``srsgui`` application starts it loads the last configuration file it used.
 If you want to use a different project from the loaded one, you can choose another one
-by selecting a configuration file with the .taskconfig extension from the **menu/File/Open**.
+by selecting a configuration file with the .taskconfig extension from the **File/Open** menu.
 
 Connecting instruments to use
 ------------------------------
 
-If you need to control instruments in your tasks, select the instrument from the **menu/Instrument**.
-It will bring up the dialog box with connection options. Once an instrument is connected,
-the Instrument Info panel displays information on the instrument.
+To connect to a remote instrument, select the instrument from the **Instruments** menu.
+This will bring up a dialog box with connection options. Once an instrument is connected,
+the Instrument Info panel displays information about the instrument.
 
 Instruments that will be used in a task must be connected before running the task.
-Connection and disconnection of an instrument should be handled in ``srsgui`` application, not from a task.
+Connection and disconnection to/from an instrument should be handled in the ``srsgui`` application
+(or in the .taskconfig file, see :ref:`here <fixed_connection_parameters>`), and not from the task itself.
 
 If you select a instrument that is already connected, it will ask if you want to disconnect the instrument. 
 
 Running a task
 ---------------
-You can choose a task to run from the **menu/Tasks**. Once you select a task,
-the Parameters panel will display the parameters for the task, and the description
-on the task from the class doc string will be displayed in the Task Result panel.
+You can choose a task to run from the **Tasks** menu. Once you select a task,
+the Parameters panel will display the parameters for the task, 
+and the Task Result panel will display the description
+of the task (defined by the the class doc string).
 
 .. figure:: ./_static/task_selection.png
     :align: center
     :scale: 75 % 
 
     Srsgui application with a floating (undocked) dock widget
 
 After selecting the task you want to run, adjust the Parameters if necessary,
-and press the green arrow under the menu, or select the **menu/Control/Run**.
+and press the green arrow under the menu toolbar, or select **Control/Run**.
 
 Stopping a running task
 ------------------------
 
 ``Srsgui`` application does not kill a running task. Instead, it sets a flag to indicate 
 the stop is requested. The running task should check the flag frequently, and stop at its earliest convenience. 
 
@@ -64,31 +66,31 @@
 --------------------
 
 Every run of a task automatically generates a data file as
 *%USERPROFILE%\\task-results\\the_name_in_taskconfig_file\\RNxxx\\task_name-timestamp.sgdata*.
 Typically, the *%USERPROFILE%* directory is *C:\\users\\your_user_name* in Windows.
 It is the home directory, *$HOME*, in Linux.
 
-A default instance of :class:`TaskResult <srsgui.task.taskresult.TaskResult>` class is generated
+A default instance of the class :class:`TaskResult <srsgui.task.taskresult.TaskResult>` is generated
 after an instance of  :class:`Task<srsgui.task.task.Task>` subclass and saved
 as a Python dictionary in the data file.
 
-A task can save additional Python dictionaries and create tables for large data in the default data file
-using APIs in :class:`Task<srsgui.task.task.Task>` class .
+A task can save additional Python dictionaries and create tables for large data sets in the default data file
+using APIs in :class:`Task<srsgui.task.task.Task>` class.
 
 Dock widgets in ``srsgui`` application
 ------------------------------------------ 
  
-``Srsgui`` application is a Qt application_ built on QMainWindow_ for GUI.
+The ``Srsgui`` application is a Qt application_ built on QMainWindow_ for GUI.
 Thanks to Python Qt binder, such as, Pyside6_, we can write Python scripts using the Qt C++ library.
 
 ``Srsgui`` extensively uses QDockWidget_ as a container for its widgets,
-such as the console, the terminal and the command capture.
+such as the console, the terminal, and the instrument capture.
 By putting the widgets in QDockWidget_, they can be
-laid out as many different ways as you want. Qt dock widgets can be docked anywhere
+arranged however you want. Qt dock widgets can be docked anywhere
 around the main window, stacked together with one another, closed, or floated (undocked)
 outside the main window. 
 
 
 .. figure:: ./_static/dock_widgets_expanded.png
     :align: center
     :scale: 50 % 
@@ -100,82 +102,84 @@
     :align: center
     :scale: 50 % 
 
     Srsgui application with a floating (undocked) dock widget
     
 The other major GUI component is Matplotlib_, the most popular Python data visualiation
 library. By putting a Matplotlib_ Figure_ in a QDockWidget_, ``srsgui`` provides
-flexible layouts of multiple Matplotlib_ plots. And encapsulating Matplotlib Figure_
-handling into :class:`Task <srsgui.task.task.Task>` class makes it simple to use a
+flexible layouts of multiple Matplotlib_ plots. Encapsulating Matplotlib Figure_-handling 
+into the :class:`Task <srsgui.task.task.Task>` class makes it simple to use a
 Matplotlib_ figure_ in :class:`Task <srsgui.task.task.Task>` subclasses.
 
-When you choose a dock widget from the **menu/Docks**, it will be brought up the dock wdget
-to the top level, even if it is closed.
+When you choose a dock widget from the **Docks** menu, it will bring the dock widget
+to the top level, even if it was previously closed.
 
 Capture dock widget
 -----------------------------
 
-Capture dock widget is the latest addition to ``srsgui`` application. Each instrument
-in the configuration file will have its capture dock widget. You can open it by select the menu item
-named as "*instrument_name-caputre*" from the menu/Docks.
-
-It is used to visualize a :class:`Instrument <srsgui.inst.instrument.Instrument>` class
-containing multiple :class:`components <srsgui.inst.component.Component>`,
+The capture dock widget is the latest addition to the ``srsgui`` application. 
+Each instrument in the configuration file will have its own capture dock widget. 
+You can open it by selecting the menu item named "*instrument_name-capture*" from the **Docks** menu.
+
+The capture dock is used to provide an interactive snapshot of the instrument state
+via a tree view of the :class:`Instrument <srsgui.inst.instrument.Instrument>` class
+and its multiple :class:`components <srsgui.inst.component.Component>`,
 :mod:`commands <srsgui.inst.commands>` and
-:mod:`index commands <srsgui.inst.indexcommands>`
-using `Qt Model/View programming. <model_view_programming_>`_
+:mod:`index commands <srsgui.inst.indexcommands>`.
+(This utilizes `Qt Model/View programming. <model_view_programming_>`_)
 
-It captures the values of :mod:`commands <srsgui.inst.commands>` and
+The capture dock captures the values of :mod:`commands <srsgui.inst.commands>` and
 :mod:`index commands <srsgui.inst.indexcommands>`
 defined in an instrument class,
 and allows you to change the values interactively.
 
 .. note::
 
     An active capture dock widget generates a lot of communication traffic to the physical
     instrument whenever it needs to update the item values.
     If the running task needs the full communication capacity,
-    close the dock widget not to interfere with generating any additional communication load.
+    you can avoid the extra communication load and prevent interference with the task
+    by closing the dock widget.
 
 It can display optional insformation:
 
     - With *Show query-only cmds* option checked, commands that can be queried,
-      but cannot not be set will be displayed with [QO] tag after the command name,
-      along with its query value.
+      but not set will be displayed with the [QO] tag after their command name,
+      along with the query value.
     - With *Show set-only cmds* option checked, the name of commands that cannot be queried
-      will be displayed with [SO] tag after the command name.
-    - With *Show excluded cmds* checked, the name of commands that intentionally excluded
-      will be displayed with [EX] tag after the command name, however, without its query return value.
+      will be displayed with the [SO] tag after the command name.
+    - With *Show excluded cmds* checked, the name of commands that are intentionally excluded
+      will be displayed with the [EX] tag after the command name. The query return value will not be shown.
     - With *Show methods* checked, methods of the components of the instrument class will be displayed
-      with [M] tag after the command name.
-      some simple methods that can run without parameters defined and does not return value
-      can have the run button that allows to run the method directly.
+      with the [M] tag after the command name.
+      Simple methods that can run without parameters defined and do not return a value
+      can be executed directly.
     - With *Show raw cmds* option checked, the raw remote command name associated with the
-      item will be shown inside the angled brackets, < >   .
+      item will be shown inside angle brackets, `< >`.
 
 Capture dock widgets help you to understand the hierarchical structure of an instrument class
-and to use command more easily in the command terminal and writing the Python scripts.
+and to use commands more easily in the command terminal or when writing task scripts in Python.
 
 .. figure:: ./_static/lockin-capture.png
     :align: center
     :scale: 75 %
 
     Screenshot of Capture dock widget of `SR860 lock-in amplifier instrument class <sr860_>`_
 
 Plot menu
 --------------
 
 When you resize a plot window, sometimes the plot does not fit well in the resized windows.
-Pressing the **menu/Plot/Adjust Layout**, will adjust the layouts of all the plots in the application.
+Pressing **Plot/Adjust Layout** will adjust the layouts of all the plots in the application.
 The layout will change with the next update.
 
 All the figures_ used in ``srsgui`` application are accompanied by
 `Matplotlib interactive navigation tool bars <toolbar_>`_.
-You can show or hide the toolbars in all the plot windows
-by selecting the **menu/Plot/Show or Hide toolbar**.
+You can show or hide the toolbars in all plot windows
+by selecting **Plot/Show or Hide toolbar**.
 
 
 .. _application: https://doc.qt.io/qt-6/qapplication.html#details
 .. _QMainWindow: https://doc.qt.io/qt-6/qmainwindow.html#details
 .. _QDockWidget: https://doc.qt.io/qt-5/qdockwidget.html#details
 .. _model_view_programming: https://doc.qt.io/qt-6/model-view-programming.html
 .. _pyside6: https://doc.qt.io/qtforpython-6/
```

### Comparing `srsgui-0.4.0.1/docs/changelog.rst` & `srsgui-0.4.1/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/docs/conf.py` & `srsgui-0.4.1/docs/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # -- Path setup --------------------------------------------------------------
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import sys
-sys.path.insert(0, os.path.abspath('/PyPI/srsgui'))
+sys.path.insert(0, os.path.abspath('../srsgui'))
 
 from srsgui import __version__
 
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
```

### Comparing `srsgui-0.4.0.1/docs/create-project.rst` & `srsgui-0.4.1/docs/create-project.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 
 .. _top-of-creating-project:
 
 Creating a project
 ===================
 
-Here is how to create a ``srsgui`` project as shown in the example
+Here is how to create an ``srsgui`` project as shown in the examples
 directory.
 
     - Create file structure for a project.
     - Make a list of instrument classes and Python scripts in a .taskconfig file.
-    - Define instrument drivers based on the :class:`Instrument<srsgui.inst.instrument.Instrument>` class
-    - Write Python scripts based on the :class:`Task<srsgui.task.task.Task>` class.
+    - Define instrument drivers based on the :class:`Instrument<srsgui.inst.instrument.Instrument>` class,
+      if you don't find ones that you want to use.
+    - Write Python scripts based on the :class:`Task<srsgui.task.task.Task>` class, or modify existing ones.
     - Open the configuration file in the ``srsgui`` application
-    - Connect instruments from the Instruments menu, if connections not defined
-      in the configuration file.
+    - Connect instruments from the Instruments menu (if connections are not defined
+      in the .taskconfig file).
     - Select a task from the Task menu and run it.
 
 
 Creating file structure for a project
 ------------------------------------------
 
 Each ``srsgui`` project makes a use of the predefined directory structure.
@@ -26,118 +27,120 @@
 
     /Project root directory
         /instruments
         /tasks
         project.taskconfig
 
 A project directory has a .taskconfig configuration file and multiple Python
-modules in two special subdirectory: instruments and tasks.
-Whenever open a .taskconfig file from the SRSGUI application,
+modules in two special subdirectories: ``instruments`` and ``tasks``.
+Whenever .taskconfig file is loaded in the SRSGUI application,
 Python modules in those directories will be forced to reload.
 
 Typically, a Python interpreter loads a module when it is imported for the first time,
-and never check again if the module is modified. When you make changes to a module, save it,
+and does not check again if the module has been modified. When you make changes to a module, save it,
 and run a script using it, you would not see the changes because the Python interpreter
 would not use the modified module, as long as the previous copy of the module is in memory.
-The Python interpreter needs to restart to take an effect of the changed modules.
+The Python interpreter needs to restart for the changed modules to take effect.
 
-When you open a .taskconfig file again from the ``srsgui`` application,
+When you open (or re-open) a .taskconfig file from the ``srsgui`` application,
 it reloads all the Python modules in the 2 subdirectories.
-It helps when you modify and debug a module in the subdirectories.
-Instead of restart the application every time a module is changed,
+Instead of restarting the ``srsgui`` application every time a module is changed,
 you can reopen the .taskconfig file to see the changes from modified modules.
-If you modify a Python module other than the ones in the 2 directories
+If you modify a Python module other than those in the 2 directories
 with respect to the current .taskconfig file, you have to restart the ``srsgui`` application
 to use the modified module.
 
-Python does not allow to use spaces in its package and module names.
-Use underscore if you need spaces between words.
+Python does not allow use of spaces in its package and module names.
+Use underscores if you need spaces between words.
 
 
 Populating the .taskconfig file
 -----------------------------------
 
 Each ``srsgui`` project has a \.taskconfig file. The configuration file
 contains:
 
-    - name of the project,
+    - name of the project
     - a list of instruments to use
     - a list tasks to run
 
 
-The following is the configuration file in the example directory
-of ``srsgui`` package without comment lines.
+The following is the configuration file in the examples directory
+of ``srsgui`` package (comment lines have been removed).
 
 .. code-block::
 
-    name: srsgui example project using an oscilloscope and a clock generator
+    name: Srsgui Example - Oscilloscope and Clock Generator
 
     inst: cg,  instruments.cg635,   CG635
     inst: osc, instruments.sds1202, SDS1202
 
     task: *IDN test,    tasks.first,  FirstTask
     task: Plot example, tasks.second, SecondTask
     ...
 
 
-The keyword 'name:' is use as
+The keyword `name:` is used as
 
-    - Title of the SRSGUI application main window (Look at the top of
-      this :ref:`screen capture <top-of-screen-capture-1>`.
-    - Directory name for the project data saving under ~/home/task-results
+    - The title of the SRSGUI application main window (see the top of
+      this :ref:`screen capture <top-of-screen-capture-1>`).
+    - The ddirectory name for the project data, which is saved under ~/home/task-results
 
-You can specify a list of instrument classes to be included in the project using 'inst:' keyword.
+You can specify a list of instrument classes to be included in the project using the `inst:` keyword.
 The first column after the keyword is the name of the instrument used across the project:
 
-    - Menu items under **Instruments** menu. It is used to connect and disconnect
-      the selected instrument.
-    - Tab labels in Instrument Info panel (in the top left corner under the red STOP button
-      in this :ref:`screen capture <top-of-screen-capture-1>`.
-    - Name used in terminal to specify a instrument. Make it short if you use a lot
-      in the terminal at the bottom right corner in this
-      :ref:`screen capture <top-of-screen-capture-1>`.
-
+    - Menu items under **Instruments** menu. Selecting an instrument from this menu is
+      allows you to connect and disconnect the selected instrument.
+    - Tab labels in the Instrument Info panel (in the top left corner under the red STOP button
+      in this :ref:`screen capture <top-of-screen-capture-1>`).
+    - Name used in the Terminal to specify an instrument (at the bottom right corner in this
+      :ref:`screen capture <top-of-screen-capture-1>`). 
+      Keep names short if you plan to interact with instruments frequently via the Terminal.
     - Argument in :meth:`get_instrument() <srsgui.task.task.Task.get_instrument>` method in
       :class:`Task<srsgui.task.task.Task>` class.
 
 The second column is the path to the module that contains the instrument class.
 The path can be relative to the .taskconfig file if it is a local module,
 
 .. code-block::
 
     inst: cg,  instruments.cg635,   CG635
 
-or a path from one of the Python site_package directory.
+or a path from the Python site_package directory.
 
 .. code-block::
 
     inst: lia, srsinst.sr860,  SR860
 
 The third column is the name of the class defined in the module.
 
+.. _fixed_connection_parameters:
 
 You can add the optional fourth column if an instrument is used with a fixed connection parameters.
+This automatically establishes the connection to the instrument when the .taskconfig is loaded.
 
 .. code-block::
 
     inst: cg2,  instruments.cg635,   CG635,   serial:COM4:9600
     inst: osc2, instruments.sds1202, SDS1202, tcpip:192.168.1.100:5035
 
-It gets the instruments connected, while a configuration file is loading.
+
 
 
 The first instrument that appears in the configuration file is the default instrument.
 When a command is entered from the terminal of the srsgui application, without instrument prefix,
 it will be sent to the default instrument.
 
 
 The keyword 'task:' is used to specify a task class to be used in the configuration file.
-the first column after the 'task:' keyword is the name of the task,
-the second is path to the module, the third one is the name of the task class.
-It specifies a task class in the same way with instrument classes.
+The columns that follow the `task` keyword are (in order)
+
+  1. The name of the task,
+  2. The path to the module, the third one is 
+  3. The name of the task class.
 
 When you open a .taskconfig file, in ``srsgui`` application, the names of the tasks
 appear as menu items under the Task menu, as shown at the top of
 this :ref:`screen capture <top-of-screen-capture-1>`.
 
 You can select one of the task items and run the task.
```

### Comparing `srsgui-0.4.0.1/docs/create-task.rst` & `srsgui-0.4.1/docs/create-task.rst`

 * *Files 27% similar despite different names*

```diff
@@ -25,54 +25,56 @@
             print('Test finished.')
 
         def cleanup(self):
             print('Cleanup done.')
 
 When a task runs, the setup() method runs first. if the setup finished with an exception,
 the task is aborted without running test() or cleanup(). If the setup() method completes
-without exception, the test() method runs next. Regardless of exception happened while
-the test() is finished, running the cleanup() method completes the task.
+without exception, the test() method runs next. Regardless of any exceptions,
+the cleanup() method runs last.
 
-You write a task based on the template any way you want, utilizing the resources and APIs
-provided in Task class for Graphic User Interface (GUI) inputs and outputs. As long as
-your tasks use the limited GUI resources available from Task class,
-your task will run along with ``srsgui`` application.
+Your task may be much more involved of course, utilizing the resources and APIs
+provided in the Task class for Graphical User Interface (GUI) inputs and outputs. 
+As long as your tasks make proper use of the GUI resources available from the :class:`Task <srsgui.task.task.Task>` class,
+your task will run successfully in the ``srsgui`` application.
 
-A task is a Python thread_ (if it is run by an application with a Qt backend,
-it will be QThread_.), running as concurrently with the main application.
+A task is executed as a Python thread_ (if it is run by an application with a Qt backend,
+it will be QThread_.), running concurrently with the main application.
 
 The :class:`Task <srsgui.task.task.Task>` is designed with much consideration
-on protection of the main application from crashing caused by unhandled Exception,
-while a buggy task running. ``srsgui`` provides information as much as Python
-interpreter does. After modifying a task, reopen the .taskconfig file will reload
-the modified task before you run it again.
+on protection of the main application from crashing caused by unhandled Exceptions. 
+``srsgui`` provides debug information and error handling just as Python interpreter does. 
+
+If you have modified a task, reopen the .taskconfig file from within ``srsgui`` in order to reload
+the modified task before you run it again (otherwise your modified code will not be run).
 
 
 The main application provides resources that a task can use,
 and responds to the callbacks from the task. The resources are set using
 the APIs provided by the task.
 
-    - :meth:`set_inst_dict <srsgui.task.task.Task.set_inst_dict>` is to set the
-      instrument dictionary that contains the instrument instances.
-    - :meth:`set_data_dict <srsgui.task.task.Task.set_data_dict>` is to set the
-      data dictionary that contains the data instances.
-    - :meth:`set_figure_dict <srsgui.task.task.Task.set_figure_dict>` is to set the
-      figure dictionary that contains the figure instances.
-    - :meth:`set_session_handler <srsgui.task.task.Task.set_session_handler>` is
-       to set the session handler that saves the data to a file.
-    - :meth:`set_callback_handler <srsgui.task.task.Task.set_session_handler>` is
-      to set the callback handler that handles the callbacks from the task.
+    - :meth:`set_inst_dict <srsgui.task.task.Task.set_inst_dict>` -- 
+      set the instrument dictionary that contains the instrument instances.
+    - :meth:`set_data_dict <srsgui.task.task.Task.set_data_dict>` -- 
+      set the data dictionary that contains the data instances.
+    - :meth:`set_figure_dict <srsgui.task.task.Task.set_figure_dict>` -- 
+      set the figure dictionary that contains the figure instances.
+    - :meth:`set_session_handler <srsgui.task.task.Task.set_session_handler>` -- 
+      set the session handler that saves the data to a file.
+    - :meth:`set_callback_handler <srsgui.task.task.Task.set_session_handler>` -- 
+      set the callback handler that handles the callbacks from the task.
 
 
 The main application and the running task are separate threads, and the main application responds only to
-the callbacks from the task.
+the callbacks from the task. Following are convenience methods for callbacks and related ones
+in the :class:`Task <srsgui.task.task.Task>` class.
 
 For text output,
     - :meth:`write_text <srsgui.task.task.Task.write_text>` is the base method for Task to use
-      :meth:`callbacks.text_available <srsgui.task.callbacks.text_available>` callback.
+      :meth:`callbacks.text_available <srsgui.task.callbacks.Callbacks.text_available>` callback.
     - :meth:`display_device_info <srsgui.task.task.Task.display_device_info>`
     - :meth:`display_result <srsgui.task.task.Task.display_result>`
     - :meth:`update_status <srsgui.task.task.Task.update_status>`
     - :meth:`print <srsgui.ui.taskmain.TaskMain.print_redirect>`
 
 For python logging_,
     - :meth:`get_logger <srsgui.task.task.Task.get_logger>` is to get the logger instance for the task.
@@ -80,59 +82,61 @@
     - ``logger.info`` is to use the logger instance to log info messages.
     - ``logger.error`` is to use the logger instance to log error messages.
     - ``logger.warning`` is to use the logger instance to log warning messages.
     - ``logger.critical`` is to use the logger instance to log critical messages.
 
 
 For the input panel in the ``srsgui`` main window,
-    :attr:`input_parameters <srsgui.task.task.Task.input_paramteres>` is a dictionary that contains
+    :attr:`input_parameters <srsgui.task.task.Task.input_parameters>` is a dictionary that contains
     the input parameters that will be displayed in the input panel.
 
     - :meth:`get_all_input_parameters <srsgui.task.task.Task.get_all_input_parameters>` is to get all the input
       parameters that are displayed in the input panel.
     - :meth:`set_input_parameter <srsgui.task.task.Task.set_input_parameter>` is to set the value of an input
       parameter.
     - :meth:`get_input_parameter <srsgui.task.task.Task.get_input_parameter>` is to get the value of an input
       parameter.
-    - :meth:`notify_parameter_changed <srsgui.task.task.Task.notify_parameter_changed>` is a wrapper method for
-      :meth:`callbacks.parameter_changed <srsgui.task.callbacks.parameter_changed`, which is to notify the
+    - :meth:`notify_parameter_changed <srsgui.task.task.Task.notify_parameter_changed>` is to notify the
       main application that the value of an input parameter has changed. The main application will
       update the value of the input parameter in the input panel.
 
-For Matplotlib Figures,
-
-    callbacks.request_figure_update - draw
-    callbacks.notify_data_available - update
-    clear_figure
-    get_figure
+For Matplotlib `figures <figure_>`_,
+    You can use most of Axes_-based Matplotlib APIs with the figure instance you get with
+    :meth:`get_figure <srsgui.task.task.Task.get_figure>`. After adding data and formats
+    into the figure, call :meth:`request_figure_update <srsgui.task.task.Task.request_figure_update>`.
+
+    - :meth:`get_figure <srsgui.task.task.Task.get_figure>`
+    - :meth:`request_figure_update <srsgui.task.task.Task.request_figure_update>`
+    - :meth:`notify_data_available <srsgui.task.task.Task.notify_data_available>`
+    - :meth:`clear_figures <srsgui.task.task.Task.clear_figures>`
 
 For a question dialog box during running a task,
-    - :meth:`ask_question <srsgui.task.task.Task.ask_question>` is a wrapper method
-      for the Task :meth:`callbacks.new_question <srsgui.task.callbacks.new_question>`.
+    - :meth:`ask_question <srsgui.task.task.Task.ask_question>`
     - :meth:`question_background_update <srsgui.task.task.Task.question_background_update>`
 
-
-For the session_handler that save information from a task to a file,
-    add_details
-    create_table
-    add_data_to_table
-    create_table_in_file
-    add_to_table_in_file
+For the session_handler (which saves information from a task to a file),
+    - :meth:`add_details <srsgui.task.task.Task.add_details>`
+    - :meth:`create_table <srsgui.task.task.Task.create_table>`
+    - :meth:`add_data_to_table <srsgui.task.task.Task.add_data_to_table>`
+    - :meth:`create_table_in_file <srsgui.task.task.Task.create_table_in_file>`
+    - :meth:`add_to_table_in_file <srsgui.task.task.Task.add_to_table_in_file>`
 
 For inst_dict
     - :meth:`get_instrument <srsgui.task.task.Task.get_instrument>` is to retrieve
       the Instrument subclass instance named in the \.taskconfig file. Once getting
       the instrument instance, you can use it in the task in the same way with
       the instance created from a Python interpreter.
 
-Once you get used to the APIs of Task class, you can write scripts that runs
-as a part of ``srsgui``.
+Once you get used to the API for the :class:`Task <srsgui.task.task.Task>` class,
+you can write scripts that run as a part of ``srsgui``.
 
 
 .. _PyVisa: https://pyvisa.readthedocs.io/en/latest/
 .. _srsinst.sr860: https://pypi.org/project/srsinst.sr860/
 .. _VXI11: https://www.lxistandard.org/About/VXI-11-and-LXI.aspx
 .. _GPIB: https://en.wikipedia.org/wiki/IEEE-488
 .. _USB-TMC: https://www.testandmeasurementtips.com/remote-communication-with-usbtmc-faq/
-.. _thread: https://realpython.com/intro-to-python-threading/
+.. _thread: https://docs.python.org/3/library/threading.html
 .. _QThread: https://doc.qt.io/qt-6/qthread.html
-.. _logging: https://docs.python.org/3/howto/logging.html
+.. _logging: https://docs.python.org/3/howto/logging.html
+.. _figure: https://matplotlib.org/stable/api/figure_api.html#matplotlib.figure.Figure
+.. _axes: https://matplotlib.org/stable/api/axes_api.html
```

### Comparing `srsgui-0.4.0.1/docs/define-instrument.rst` & `srsgui-0.4.1/docs/define-instrument.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,382 +1,410 @@
-00000000: 0d44 6566 696e 696e 6720 616e 2069 6e73  .Defining an ins
-00000010: 7472 756d 656e 7420 636c 6173 730d 2d2d  trument class.--
+00000000: 0d0a 4465 6669 6e69 6e67 2061 6e20 696e  ..Defining an in
+00000010: 7374 7275 6d65 6e74 2063 6c61 7373 0d0a  strument class..
 00000020: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000030: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0d 616e  ------------..an
-00000040: 2069 6e73 7472 756d 656e 7420 636c 6173   instrument clas
-00000050: 7320 6973 2061 2073 7562 636c 6173 7320  s is a subclass 
-00000060: 6465 7269 7665 6420 6672 6f6d 2074 6865  derived from the
-00000070: 0d3a 636c 6173 733a 6049 6e73 7472 756d  .:class:`Instrum
-00000080: 656e 743c 7372 7367 7569 2e69 6e73 742e  ent<srsgui.inst.
-00000090: 696e 7374 7275 6d65 6e74 2e49 6e73 7472  instrument.Instr
-000000a0: 756d 656e 743e 6020 636c 6173 732e 0d4d  ument>` class..M
-000000b0: 696e 696d 756d 2072 6571 7569 7265 6d65  inimum requireme
-000000c0: 6e74 2069 7320 746f 2068 6176 6520 2a2a  nt is to have **
-000000d0: 5f49 6453 7472 696e 672a 2a20 746f 2063  _IdString** to c
-000000e0: 6865 636b 2069 6620 6120 636f 6e6e 6563  heck if a connec
-000000f0: 7465 640d 696e 7374 7275 6d65 6e74 2069  ted.instrument i
-00000100: 7320 6120 636f 7272 6563 7420 696e 7374  s a correct inst
-00000110: 7275 6d65 6e74 2020 7468 6174 2063 616e  rument  that can
-00000120: 2062 6520 7573 6564 2077 6974 6820 7468   be used with th
-00000130: 6520 636c 6173 732e 0d0d 2e2e 2063 6f64  e class..... cod
-00000140: 652d 626c 6f63 6b3a 3a0d 0d20 2020 2066  e-block::..    f
-00000150: 726f 6d20 7372 7367 7569 2069 6d70 6f72  rom srsgui impor
-00000160: 7420 496e 7374 7275 6d65 6e74 0d20 2020  t Instrument.   
-00000170: 2063 6c61 7373 2043 4736 3335 2849 6e73   class CG635(Ins
-00000180: 7472 756d 656e 7429 3a0d 2020 2020 2020  trument):.      
-00000190: 2020 5f49 6453 7472 696e 6720 3d20 2743    _IdString = 'C
-000001a0: 4736 3335 270d 2020 2020 2020 2020 5f74  G635'.        _t
-000001b0: 6572 6d5f 6368 6172 203d 2062 275c 7227  erm_char = b'\r'
-000001c0: 2020 2320 4164 6420 7468 6973 206c 696e    # Add this lin
-000001d0: 6520 6966 2074 6865 2063 6172 7269 6167  e if the carriag
-000001e0: 6520 7265 7475 726e 2069 7320 7468 6520  e return is the 
-000001f0: 7465 726d 696e 6174 696f 6e20 6368 6172  termination char
-00000200: 6163 7465 720d 2020 2020 2020 2020 2020  acter.          
-00000210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000220: 2020 2320 6f66 2074 6865 2069 6e73 7472    # of the instr
-00000230: 756d 656e 742c 2069 6e73 7465 6164 206f  ument, instead o
-00000240: 6620 7468 6520 6c69 6e65 2066 6565 6420  f the line feed 
-00000250: 2841 5343 4949 3a20 3078 3130 2c20 6227  (ASCII: 0x10, b'
-00000260: 5c6e 2729 2e0d 0d0d 4966 2074 6865 2069  \n')....If the i
-00000270: 6e73 7472 756d 656e 7420 6861 733a 0d20  nstrument has:. 
-00000280: 2020 2031 2e20 7468 6520 2a2a 5c2a 4944     1. the **\*ID
-00000290: 4e3f 2a2a 2072 656d 6f74 6520 636f 6d6d  N?** remote comm
-000002a0: 616e 640d 2020 2020 322e 2065 6974 6865  and.    2. eithe
-000002b0: 7220 5253 3233 3220 7365 7269 616c 2063  r RS232 serial c
-000002c0: 6f6d 6d75 6e69 6361 7469 6f6e 206f 7220  ommunication or 
-000002d0: 4574 6865 726e 6574 2054 4350 4950 2063  Ethernet TCPIP c
-000002e0: 6f6d 6d75 6e69 6361 7469 6f6e 2070 6f72  ommunication por
-000002f0: 7420 6176 6169 6c61 626c 652c 0d0d 7468  t available,..th
-00000300: 6520 696e 7374 7275 6d65 6e74 2063 616e  e instrument can
-00000310: 2062 6520 636f 6e6e 6563 7465 6420 616e   be connected an
-00000320: 6420 7573 6564 2069 6e20 7461 736b 2073  d used in task s
-00000330: 6372 6970 7473 2061 6e64 2069 6e20 7468  cripts and in th
-00000340: 6520 7465 726d 696e 616c 2c0d 7769 7468  e terminal,.with
-00000350: 2034 206c 696e 6573 206f 6620 6465 6669   4 lines of defi
-00000360: 6e69 7469 6f6e 206c 696b 6520 6162 6f76  nition like abov
-00000370: 652e 2049 6620 6974 2064 6f65 7320 6e6f  e. If it does no
-00000380: 7420 6861 7665 2074 6865 205c 2a49 444e  t have the \*IDN
-00000390: 3f20 7265 6d6f 7465 2063 6f6d 6d61 6e64  ? remote command
-000003a0: 2c0d 3a6d 6574 683a 6063 6865 636b 5f69  ,.:meth:`check_i
-000003b0: 6428 293c 7372 7367 7569 2e69 6e73 742e  d()<srsgui.inst.
-000003c0: 696e 7374 7275 6d65 6e74 2e49 6e73 7472  instrument.Instr
-000003d0: 756d 656e 742e 6368 6563 6b5f 6964 3e60  ument.check_id>`
-000003e0: 206d 6574 686f 6420 696e 2049 6e73 7472   method in Instr
-000003f0: 756d 656e 740d 636c 6173 7320 6e65 6564  ument.class need
-00000400: 7320 746f 2062 6520 7265 696d 706c 656d  s to be reimplem
-00000410: 656e 7465 642e 0d0d 4176 6169 6c61 626c  ented...Availabl
-00000420: 655f 696e 7465 7266 6163 6573 0d5e 5e5e  e_interfaces.^^^
-00000430: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ^^^^^^^^^^^^^^^^
-00000440: 5e5e 0d0d 6041 7661 696c 6162 6c65 5f69  ^^..`Available_i
-00000450: 6e74 6572 6661 6365 6020 6465 6669 6e65  nterface` define
-00000460: 7320 7768 6174 206b 696e 6420 6f66 2063  s what kind of c
-00000470: 6f6d 6d75 6e69 6361 7469 6f6e 2069 7320  ommunication is 
-00000480: 6176 6169 6c61 626c 6520 666f 7220 7468  available for th
-00000490: 6520 696e 7374 7275 6d65 6e74 2c0d 7468  e instrument,.th
-000004a0: 6520 6261 7365 203a 636c 6173 733a 6049  e base :class:`I
-000004b0: 6e73 7472 756d 656e 743c 7372 7367 7569  nstrument<srsgui
-000004c0: 2e69 6e73 742e 696e 7374 7275 6d65 6e74  .inst.instrument
-000004d0: 2e49 6e73 7472 756d 656e 743e 6020 636c  .Instrument>` cl
-000004e0: 6173 7320 6861 7320 7468 6520 666f 6c6c  ass has the foll
-000004f0: 6f77 696e 670d 6465 6669 6e69 7469 6f6e  owing.definition
-00000500: 2066 6f72 2073 6572 6961 6c20 616e 6420   for serial and 
-00000510: 5443 5049 5020 636f 6d6d 756e 6963 6174  TCPIP communicat
-00000520: 696f 6e20 696e 7465 7266 6163 6573 3a0d  ion interfaces:.
-00000530: 0d2e 2e20 636f 6465 2d62 6c6f 636b 3a3a  ... code-block::
-00000540: 0d0d 2020 2020 6176 6169 6c61 626c 655f  ..    available_
-00000550: 696e 7465 7266 6163 6573 203d 205b 0d20  interfaces = [. 
-00000560: 2020 2020 2020 205b 2020 2053 6572 6961         [   Seria
-00000570: 6c49 6e74 6572 6661 6365 2c0d 2020 2020  lInterface,.    
-00000580: 2020 2020 2020 2020 7b0d 2020 2020 2020          {.      
-00000590: 2020 2020 2020 2020 2020 2770 6f72 7427            'port'
-000005a0: 3a20 4669 6e64 4c69 7374 496e 7075 7428  : FindListInput(
-000005b0: 292c 0d20 2020 2020 2020 2020 2020 2020  ),.             
-000005c0: 2020 2027 6261 7564 5f72 6174 6527 3a20     'baud_rate': 
-000005d0: 496e 7465 6765 724c 6973 7449 6e70 7574  IntegerListInput
-000005e0: 285b 3936 3030 2c20 3131 3532 3030 5d29  ([9600, 115200])
-000005f0: 2c0d 2020 2020 2020 2020 2020 2020 2020  ,.              
-00000600: 2020 2768 6172 6477 6172 655f 666c 6f77    'hardware_flow
-00000610: 5f63 6f6e 7472 6f6c 273a 2042 6f6f 6c49  _control': BoolI
-00000620: 6e70 7574 285b 274f 6666 272c 2027 4f6e  nput(['Off', 'On
-00000630: 275d 290d 2020 2020 2020 2020 2020 2020  ']).            
-00000640: 7d0d 2020 2020 2020 2020 5d2c 0d20 2020  }.        ],.   
-00000650: 2020 2020 205b 2020 2054 6370 6970 496e       [   TcpipIn
-00000660: 7465 7266 6163 652c 0d20 2020 2020 2020  terface,.       
-00000670: 2020 2020 207b 0d20 2020 2020 2020 2020       {.         
-00000680: 2020 2020 2020 2027 6970 5f61 6464 7265         'ip_addre
-00000690: 7373 273a 2049 7034 496e 7075 7428 2731  ss': Ip4Input('1
-000006a0: 3932 2e31 3638 2e31 2e31 3027 292c 0d20  92.168.1.10'),. 
-000006b0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000006c0: 706f 7274 273a 2049 6e74 6567 6572 496e  port': IntegerIn
-000006d0: 7075 7428 3233 290d 2020 2020 2020 2020  put(23).        
-000006e0: 2020 2020 7d0d 2020 2020 2020 2020 5d0d      }.        ].
-000006f0: 2020 2020 5d0d 0d49 6620 796f 7572 2069      ]..If your i
-00000700: 6e73 7472 756d 656e 7420 6e65 6564 7320  nstrument needs 
-00000710: 6f74 6865 7220 7468 616e 2073 6572 6961  other than seria
-00000720: 6c20 616e 6420 5443 5049 5020 696e 7465  l and TCPIP inte
-00000730: 7266 6163 6573 2c20 6060 7372 7367 7569  rfaces, ``srsgui
-00000740: 6060 2061 6c6c 6f77 7320 746f 2061 6464  `` allows to add
-00000750: 0d6f 7468 6572 2063 6f6d 6d75 6e69 6361  .other communica
-00000760: 7469 6f6e 2063 6c61 7373 6573 2064 6572  tion classes der
-00000770: 6976 6564 2066 726f 6d0d 3a63 6c61 7373  ived from.:class
-00000780: 3a60 496e 7465 7266 6163 6520 3c73 7273  :`Interface <srs
-00000790: 6775 692e 696e 7374 2e63 6f6d 6d75 6e69  gui.inst.communi
-000007a0: 6361 7469 6f6e 2e69 6e74 6572 6661 6365  cation.interface
-000007b0: 2e49 6e74 6572 6661 6365 3e60 2063 6c61  .Interface>` cla
-000007c0: 7373 2e0d 4375 7272 656e 746c 7920 7468  ss..Currently th
-000007d0: 6572 6520 6172 6520 7477 6f20 6578 7465  ere are two exte
-000007e0: 726e 616c 2063 6f6d 6d75 6e69 6361 7469  rnal communicati
-000007f0: 6f6e 2069 6e74 6572 6661 6365 7320 6172  on interfaces ar
-00000800: 6520 6176 6169 6c61 626c 6520 6672 6f6d  e available from
-00000810: 0d60 7372 7369 6e73 742e 7372 3836 3060  .`srsinst.sr860`
-00000820: 5f20 7061 636b 6167 653a 2060 6056 7869  _ package: ``Vxi
-00000830: 3131 496e 7465 7266 6163 6560 6020 616e  11Interface`` an
-00000840: 6420 6060 5669 7361 496e 7465 7266 6163  d ``VisaInterfac
-00000850: 6560 602c 0d77 6869 6368 2063 6f76 6572  e``,.which cover
-00000860: 7320 666f 7220 5658 4931 315f 2c20 4750  s for VXI11_, GP
-00000870: 4942 5f20 616e 6420 5553 422d 544d 435f  IB_ and USB-TMC_
-00000880: 2e20 596f 7520 6361 6e20 696d 706f 7274  . You can import
-00000890: 2074 6865 2069 6e74 6572 6661 6365 206d   the interface m
-000008a0: 6f64 756c 6573 0d66 726f 6d20 6073 7273  odules.from `srs
-000008b0: 696e 7374 2e73 7238 3630 605f 202e 0d0d  inst.sr860`_ ...
-000008c0: 4176 6169 6c61 626c 655f 696e 7465 7266  Available_interf
-000008d0: 6163 6573 2069 6e20 5353 5238 3635 2063  aces in SSR865 c
-000008e0: 6c61 7373 2069 7320 6465 6669 6e65 2061  lass is define a
-000008f0: 7320 666f 6c6c 6f77 696e 673a 0d0d 2e2e  s following:....
-00000900: 2063 6f64 652d 626c 6f63 6b3a 3a0d 0d20   code-block::.. 
-00000910: 2020 2061 7661 696c 6162 6c65 5f69 6e74     available_int
-00000920: 6572 6661 6365 7320 3d20 5b0d 2020 2020  erfaces = [.    
-00000930: 2020 2020 5b20 2020 5678 6931 3149 6e74      [   Vxi11Int
-00000940: 6572 6661 6365 2c0d 2020 2020 2020 2020  erface,.        
-00000950: 2020 2020 7b0d 2020 2020 2020 2020 2020      {.          
-00000960: 2020 2020 2020 2769 705f 6164 6472 6573        'ip_addres
-00000970: 7327 3a20 4970 3449 6e70 7574 2827 3139  s': Ip4Input('19
-00000980: 322e 3136 382e 312e 3130 2729 2c0d 2020  2.168.1.10'),.  
-00000990: 2020 2020 2020 2020 2020 7d0d 2020 2020            }.    
-000009a0: 2020 2020 5d2c 0d20 2020 2020 2020 205b      ],.        [
-000009b0: 2020 2056 6973 6149 6e74 6572 6661 6365     VisaInterface
-000009c0: 2c0d 2020 2020 2020 2020 2020 2020 7b0d  ,.            {.
-000009d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009e0: 2772 6573 6f75 7263 6527 3a20 4669 6e64  'resource': Find
-000009f0: 4c69 7374 496e 7075 7428 292c 0d20 2020  ListInput(),.   
-00000a00: 2020 2020 2020 2020 207d 0d20 2020 2020           }.     
-00000a10: 2020 205d 2c0d 2020 2020 2020 2020 5b20     ],.        [ 
-00000a20: 2020 5463 7069 7049 6e74 6572 6661 6365    TcpipInterface
-00000a30: 2c0d 2020 2020 2020 2020 2020 2020 7b0d  ,.            {.
-00000a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a50: 2769 705f 6164 6472 6573 7327 3a20 4970  'ip_address': Ip
-00000a60: 3449 6e70 7574 2827 3139 322e 3136 382e  4Input('192.168.
-00000a70: 312e 3130 2729 2c0d 2020 2020 2020 2020  1.10'),.        
-00000a80: 2020 2020 2020 2020 2770 6f72 7427 3a20          'port': 
-00000a90: 3233 0d20 2020 2020 2020 2020 2020 207d  23.            }
-00000aa0: 0d20 2020 2020 2020 205d 2c0d 2020 2020  .        ],.    
-00000ab0: 2020 2020 5b20 2020 5365 7269 616c 496e      [   SerialIn
-00000ac0: 7465 7266 6163 652c 0d20 2020 2020 2020  terface,.       
-00000ad0: 2020 2020 207b 0d20 2020 2020 2020 2020       {.         
-00000ae0: 2020 2020 2020 2027 706f 7274 273a 2046         'port': F
-00000af0: 696e 644c 6973 7449 6e70 7574 2829 2c0d  indListInput(),.
-00000b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b10: 2762 6175 645f 7261 7465 273a 2049 6e74  'baud_rate': Int
-00000b20: 6567 6572 4c69 7374 496e 7075 7428 5b39  egerListInput([9
-00000b30: 3630 302c 2031 3932 3030 2c20 3338 3430  600, 19200, 3840
-00000b40: 302c 2031 3135 3230 302c 0d20 2020 2020  0, 115200,.     
-00000b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b70: 2020 2020 2020 2020 2020 3233 3034 3030            230400
-00000b80: 2c20 3436 3038 3030 5d2c 2033 290d 2020  , 460800], 3).  
-00000b90: 2020 2020 2020 2020 2020 7d0d 2020 2020            }.    
-00000ba0: 2020 2020 5d2c 0d20 2020 205d 0d0d 5468      ],.    ]..Th
-00000bb0: 6520 6465 6669 6e69 7469 6f6e 206f 6620  e definition of 
-00000bc0: 6176 6169 6c61 626c 655f 696e 7465 7266  available_interf
-00000bd0: 6163 6573 2069 7320 616c 6c20 796f 7520  aces is all you 
-00000be0: 6e65 6564 2074 6f20 646f 2074 6f20 6765  need to do to ge
-00000bf0: 7420 6120 6375 7374 6f6d 697a 6564 0d64  t a customized.d
-00000c00: 6961 6c6f 6720 626f 7820 6f70 656e 6564  ialog box opened
-00000c10: 2066 6f72 2074 6865 2069 6e73 7472 756d   for the instrum
-00000c20: 656e 7420 696e 2060 6073 7273 6775 6960  ent in ``srsgui`
-00000c30: 6020 6170 706c 6963 6174 696f 6e2e 0d0d  ` application...
-00000c40: 2e2e 2066 6967 7572 653a 3a20 2e2f 5f73  .. figure:: ./_s
-00000c50: 7461 7469 632f 636f 6e6e 6563 742d 6469  tatic/connect-di
-00000c60: 616c 6f67 2d62 6f78 2d63 6170 7475 7265  alog-box-capture
-00000c70: 2e70 6e67 0d20 2020 203a 616c 6967 6e3a  .png.    :align:
-00000c80: 2063 656e 7465 720d 2020 2020 3a66 6967   center.    :fig
-00000c90: 636c 6173 733a 2061 6c69 676e 2d63 656e  class: align-cen
-00000ca0: 7465 720d 0d46 6f72 2060 6056 6973 6149  ter..For ``VisaI
-00000cb0: 6e74 6572 6661 6365 6060 2c20 796f 7520  nterface``, you 
-00000cc0: 6861 7665 2074 6f20 6765 7420 5079 5649  have to get PyVI
-00000cd0: 5341 5f20 776f 726b 696e 6720 6265 666f  SA_ working befo
-00000ce0: 7265 2072 756e 6e69 6e67 2060 6073 7273  re running ``srs
-00000cf0: 6775 6960 6020 6170 706c 6963 6174 696f  gui`` applicatio
-00000d00: 6e2e 0d49 7420 696e 766f 6c76 6573 2069  n..It involves i
-00000d10: 6e73 7461 6c6c 6174 696f 6e20 6f66 2074  nstallation of t
-00000d20: 6865 2050 7956 4953 4120 7061 636b 6167  he PyVISA packag
-00000d30: 6520 616e 6420 6974 7320 6261 636b 656e  e and its backen
-00000d40: 6420 6c69 6272 6172 792e 0d52 6566 6572  d library..Refer
-00000d50: 2074 6f20 5079 5649 5341 5f20 646f 6375   to PyVISA_ docu
-00000d60: 6d65 6e74 6174 696f 6e20 666f 7220 696e  mentation for in
-00000d70: 7374 616c 6c61 7469 6f6e 2064 6574 6169  stallation detai
-00000d80: 6c2e 0d0d 4672 6f6d 2050 7974 686f 6e20  l...From Python 
-00000d90: 696e 7465 7270 7265 7465 722c 2079 6f75  interpreter, you
-00000da0: 2063 616e 2063 6f6e 6e65 6374 2061 6e64   can connect and
-00000db0: 2075 7365 2061 2069 6e73 7472 756d 656e   use a instrumen
-00000dc0: 742c 206f 6e63 6520 6974 7320 6060 496e  t, once its ``In
-00000dd0: 7374 7275 6d65 6e74 6060 2063 6c61 7373  strument`` class
-00000de0: 2069 7320 6465 6669 6e65 642e 0d0d 2e2e   is defined.....
-00000df0: 2063 6f64 652d 626c 6f63 6b3a 3a0d 0d20   code-block::.. 
-00000e00: 2020 2043 3a5c 7372 7367 7569 3e70 7974     C:\srsgui>pyt
-00000e10: 686f 6e0d 2020 2020 5079 7468 6f6e 2033  hon.    Python 3
-00000e20: 2e38 2e33 2028 7461 6773 2f76 332e 382e  .8.3 (tags/v3.8.
-00000e30: 333a 3666 3863 3833 322c 204d 6179 2031  3:6f8c832, May 1
-00000e40: 3320 3230 3230 2c20 3232 3a33 373a 3032  3 2020, 22:37:02
-00000e50: 2920 5b4d 5343 2076 2e31 3932 3420 3634  ) [MSC v.1924 64
-00000e60: 2062 6974 2028 414d 4436 3429 5d20 6f6e   bit (AMD64)] on
-00000e70: 2077 696e 3332 0d20 2020 2054 7970 6520   win32.    Type 
-00000e80: 2268 656c 7022 2c20 2263 6f70 7972 6967  "help", "copyrig
-00000e90: 6874 222c 2022 6372 6564 6974 7322 206f  ht", "credits" o
-00000ea0: 7220 226c 6963 656e 7365 2220 666f 7220  r "license" for 
-00000eb0: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
-00000ec0: 2e0d 2020 2020 3e3e 3e0d 2020 2020 3e3e  ..    >>>.    >>
-00000ed0: 3e20 6672 6f6d 2073 7273 696e 7374 2e73  > from srsinst.s
-00000ee0: 7238 3630 2069 6d70 6f72 7420 5352 3836  r860 import SR86
-00000ef0: 300d 2020 2020 3e3e 3e20 6672 6f6d 2073  0.    >>> from s
-00000f00: 7273 6775 6920 696d 706f 7274 2053 6572  rsgui import Ser
-00000f10: 6961 6c49 6e74 650d 2020 2020 3e3e 3e20  ialInte.    >>> 
-00000f20: 5365 7269 616c 496e 7465 7266 6163 652e  SerialInterface.
-00000f30: 6669 6e64 2829 0d20 2020 205b 2743 4f4d  find().    ['COM
-00000f40: 3327 2c20 2743 4f4d 3427 2c20 2743 4f4d  3', 'COM4', 'COM
-00000f50: 3235 3627 5d0d 2020 2020 3e3e 3e20 6c69  256'].    >>> li
-00000f60: 6120 3d20 5352 3836 3028 2773 6572 6961  a = SR860('seria
-00000f70: 6c27 2c27 434f 4d34 272c 3131 3532 3030  l','COM4',115200
-00000f80: 2c20 4661 6c73 6529 0d20 2020 203e 3e3e  , False).    >>>
-00000f90: 206c 6961 2e71 7565 7279 5f74 6578 7428   lia.query_text(
-00000fa0: 272a 6964 6e3f 2729 0d20 2020 2027 5374  '*idn?').    'St
-00000fb0: 616e 666f 7264 5f52 6573 6561 7263 685f  anford_Research_
-00000fc0: 5379 7374 656d 732c 5352 3836 3541 2c30  Systems,SR865A,0
-00000fd0: 3032 3732 352c 7631 2e33 3427 0d20 2020  02725,v1.34'.   
-00000fe0: 203e 3e3e 206c 6961 2e64 6973 636f 6e6e   >>> lia.disconn
-00000ff0: 6563 7428 290d 2020 2020 3e3e 3e0d 2020  ect().    >>>.  
-00001000: 2020 3e3e 3e20 6672 6f6d 2073 7273 696e    >>> from srsin
-00001010: 7374 2e73 7238 3630 2069 6d70 6f72 7420  st.sr860 import 
-00001020: 5669 7361 496e 7465 7266 6163 650d 2020  VisaInterface.  
-00001030: 2020 3e3e 3e20 5669 7361 496e 7465 7266    >>> VisaInterf
-00001040: 6163 652e 6669 6e64 2829 0d20 2020 205b  ace.find().    [
-00001050: 2755 5342 303a 3a30 7842 3530 363a 3a30  'USB0::0xB506::0
-00001060: 7832 3030 303a 3a30 3032 3732 353a 3a49  x2000::002725::I
-00001070: 4e53 5452 272c 2027 4750 4942 303a 3a34  NSTR', 'GPIB0::4
-00001080: 3a3a 494e 5354 5227 5d0d 2020 2020 3e3e  ::INSTR'].    >>
-00001090: 3e20 6c69 612e 636f 6e6e 6563 7428 2776  > lia.connect('v
-000010a0: 6973 6127 2c20 2755 5342 303a 3a30 7842  isa', 'USB0::0xB
-000010b0: 3530 363a 3a30 7832 3030 303a 3a30 3032  506::0x2000::002
-000010c0: 3732 353a 3a49 4e53 5452 2729 0d20 2020  725::INSTR').   
-000010d0: 203e 3e3e 206c 6961 2e71 7565 7279 5f74   >>> lia.query_t
-000010e0: 6578 7428 272a 6964 6e3f 2729 0d20 2020  ext('*idn?').   
-000010f0: 2027 5374 616e 666f 7264 5f52 6573 6561   'Stanford_Resea
-00001100: 7263 685f 5379 7374 656d 732c 5352 3836  rch_Systems,SR86
-00001110: 3541 2c30 3032 3732 352c 7631 2e33 345c  5A,002725,v1.34\
-00001120: 6e27 0d20 2020 203e 3e3e 0d0d 5765 6c6c  n'.    >>>..Well
-00001130: 2c20 7468 6573 6520 6f70 6572 6174 696f  , these operatio
-00001140: 6e73 2061 7265 2077 6861 7420 796f 7520  ns are what you 
-00001150: 6361 6e20 646f 2077 6974 6820 5079 5649  can do with PyVI
-00001160: 5341 5f20 6974 7365 6c66 2e20 4465 6669  SA_ itself. Defi
-00001170: 6e69 6e67 2061 6e20 696e 7374 7275 6d65  ning an instrume
-00001180: 6e74 2063 6c61 7373 2c0d 6164 6469 6e67  nt class,.adding
-00001190: 2069 7420 696e 2061 202e 7461 736b 636f   it in a .taskco
-000011a0: 6e66 6967 2066 696c 652c 2061 6e64 206f  nfig file, and o
-000011b0: 7065 6e69 6e67 2069 7420 696e 2060 6073  pening it in ``s
-000011c0: 7273 6775 6960 6020 6170 706c 6963 6174  rsgui`` applicat
-000011d0: 696f 6e20 6c65 7420 796f 750d 7573 6520  ion let you.use 
-000011e0: 7468 6520 7465 726d 696e 616c 2074 6f20  the terminal to 
-000011f0: 696e 7465 7261 6374 2077 6974 6820 6d75  interact with mu
-00001200: 6c74 6970 6c65 2069 6e73 7472 756d 656e  ltiple instrumen
-00001210: 7420 6174 206f 6e63 652c 2061 6e64 2075  t at once, and u
-00001220: 7365 2068 6967 6820 6c65 7665 6c20 6060  se high level ``
-00001230: 496e 7374 7275 6d65 6e74 6060 0d63 6c61  Instrument``.cla
-00001240: 7373 2061 7474 7269 6275 7465 7320 616e  ss attributes an
-00001250: 6420 6d65 7468 6f64 732e 0d0d 4265 6c6f  d methods...Belo
-00001260: 7720 6973 2061 6e20 696d 6167 6520 6f66  w is an image of
-00001270: 2074 6572 6d69 6e61 6c20 6361 7074 7572   terminal captur
-00001280: 6564 2077 6974 6820 7468 6520 6578 616d  ed with the exam
-00001290: 706c 6520 7072 6f6a 6563 7420 6f70 656e  ple project open
-000012a0: 6564 2e0d 4173 2079 6f75 2063 616e 2073  ed..As you can s
-000012b0: 6565 2c20 796f 7520 6361 6e20 696e 7465  ee, you can inte
-000012c0: 7261 6374 2077 6974 6820 7468 6520 636c  ract with the cl
-000012d0: 6f63 6b20 6765 6e65 7261 746f 7220 616e  ock generator an
-000012e0: 6420 6f73 6369 6c6c 6f73 636f 7065 2069  d oscilloscope i
-000012f0: 6e20 6d61 6e79 2077 6179 732e 0d54 6865  n many ways..The
-00001300: 7265 2061 7265 2074 776f 2063 6f6d 6d61  re are two comma
-00001310: 6e64 7320 666f 7220 6f73 633a 205c 2a69  nds for osc: \*i
-00001320: 646e 3f2c 2073 6172 613f 2075 7365 642c  dn?, sara? used,
-00001330: 2061 6e64 2074 776f 2063 6f6d 6d61 6e64   and two command
-00001340: 7320 666f 7220 6367 3a0d 5c2a 6964 6e3f  s for cg:.\*idn?
-00001350: 2c20 6672 6571 283f 2920 7573 6564 2069  , freq(?) used i
-00001360: 6e20 7468 6520 7465 726d 696e 616c 2e0d  n the terminal..
-00001370: 0d2e 2e20 6669 6775 7265 3a3a 202e 2f5f  ... figure:: ./_
-00001380: 7374 6174 6963 2f74 6572 6d69 6e61 6c2d  static/terminal-
-00001390: 7769 7468 2d65 7861 6d70 6c65 2e70 6e67  with-example.png
-000013a0: 0d20 2020 203a 616c 6967 6e3a 2063 656e  .    :align: cen
-000013b0: 7465 720d 2020 2020 3a66 6967 636c 6173  ter.    :figclas
-000013c0: 733a 2061 6c69 676e 2d63 656e 7465 720d  s: align-center.
-000013d0: 0d7c 0d0d 0d43 6f6d 706f 6e65 6e74 2c20  .|...Component, 
-000013e0: 436f 6d6d 616e 6473 2061 6e64 2049 6e64  Commands and Ind
-000013f0: 6578 436f 6d6d 616e 6473 0d5e 5e5e 5e5e  exCommands.^^^^^
-00001400: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ^^^^^^^^^^^^^^^^
-00001410: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ^^^^^^^^^^^^^^^^
-00001420: 5e0d 0d3a 636c 6173 733a 6049 6e73 7472  ^..:class:`Instr
-00001430: 756d 656e 7420 3c73 7273 6775 692e 696e  ument <srsgui.in
-00001440: 7374 2e69 6e73 7472 756d 656e 742e 496e  st.instrument.In
-00001450: 7374 7275 6d65 6e74 3e60 2063 6c61 7373  strument>` class
-00001460: 2075 7365 730d 3a63 6c61 7373 3a60 436f   uses.:class:`Co
-00001470: 6d70 6f6e 656e 7420 3c73 7273 6775 692e  mponent <srsgui.
-00001480: 696e 7374 2e63 6f6d 706f 6e65 6e74 2e43  inst.component.C
-00001490: 6f6d 706f 6e65 6e74 3e60 2063 6c61 7373  omponent>` class
-000014a0: 2c0d 3a6d 6f64 3a60 436f 6d6d 616e 6420  ,.:mod:`Command 
-000014b0: 3c73 7273 6775 692e 696e 7374 2e63 6f6d  <srsgui.inst.com
-000014c0: 6d61 6e64 733e 6020 636c 6173 7365 7320  mands>` classes 
-000014d0: 616e 640d 3a6d 6f64 3a60 496e 6465 7843  and.:mod:`IndexC
-000014e0: 6f6d 6d61 6e64 203c 7372 7367 7569 2e69  ommand <srsgui.i
-000014f0: 6e73 742e 696e 6465 7863 6f6d 6d61 6e64  nst.indexcommand
-00001500: 733e 6020 636c 6173 7365 730d 746f 206f  s>` classes.to o
-00001510: 7267 616e 697a 6520 7468 6520 6675 6e63  rganize the func
-00001520: 7469 6f6e 616c 6974 7920 6f66 2061 6e20  tionality of an 
-00001530: 696e 7374 7275 6d65 6e74 2e0d 0d49 6620  instrument...If 
-00001540: 796f 7520 6861 7665 2074 6f20 6465 616c  you have to deal
-00001550: 2077 6974 6820 6875 6e64 7265 6473 206f   with hundreds o
-00001560: 6620 7265 6d6f 7465 2063 6f6d 6d61 6e64  f remote command
-00001570: 7320 746f 2075 7365 2061 6e20 696e 7374  s to use an inst
-00001580: 7275 6d65 6e74 2072 656d 6f74 656c 792c  rument remotely,
-00001590: 0d6f 7267 616e 697a 696e 6720 7468 656d  .organizing them
-000015a0: 2069 6e20 6120 6d61 6e61 6765 6162 6c65   in a manageable
-000015b0: 2077 6179 2069 7320 6372 7563 6961 6c2e   way is crucial.
-000015c0: 2060 5372 7369 6e73 742e 7372 3836 3060   `Srsinst.sr860`
-000015d0: 5f20 7061 636b 6167 6520 7368 6f77 7320  _ package shows 
-000015e0: 686f 7720 7468 6573 650d 636f 6e76 656e  how these.conven
-000015f0: 6965 6e63 6520 636c 6173 7365 7320 6172  ience classes ar
-00001600: 6520 7573 6564 2074 6f20 6f72 6761 6e69  e used to organi
-00001610: 7a65 2061 206c 6172 6765 2073 6574 206f  ze a large set o
-00001620: 6620 7265 6d6f 7465 2063 6f6d 6d61 6e64  f remote command
-00001630: 732e 0d0d 0d2e 2e20 5f50 7956 6973 613a  s...... _PyVisa:
-00001640: 2068 7474 7073 3a2f 2f70 7976 6973 612e   https://pyvisa.
-00001650: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-00001660: 6e2f 6c61 7465 7374 2f0d 2e2e 205f 7372  n/latest/... _sr
-00001670: 7369 6e73 742e 7372 3836 303a 2068 7474  sinst.sr860: htt
-00001680: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
-00001690: 6f6a 6563 742f 7372 7369 6e73 742e 7372  oject/srsinst.sr
-000016a0: 3836 302f 0d2e 2e20 5f56 5849 3131 3a20  860/... _VXI11: 
-000016b0: 6874 7470 733a 2f2f 7777 772e 6c78 6973  https://www.lxis
-000016c0: 7461 6e64 6172 642e 6f72 672f 4162 6f75  tandard.org/Abou
-000016d0: 742f 5658 492d 3131 2d61 6e64 2d4c 5849  t/VXI-11-and-LXI
-000016e0: 2e61 7370 780d 2e2e 205f 4750 4942 3a20  .aspx... _GPIB: 
-000016f0: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
-00001700: 6564 6961 2e6f 7267 2f77 696b 692f 4945  edia.org/wiki/IE
-00001710: 4545 2d34 3838 0d2e 2e20 5f55 5342 2d54  EE-488... _USB-T
-00001720: 4d43 3a20 6874 7470 733a 2f2f 7777 772e  MC: https://www.
-00001730: 7465 7374 616e 646d 6561 7375 7265 6d65  testandmeasureme
-00001740: 6e74 7469 7073 2e63 6f6d 2f72 656d 6f74  nttips.com/remot
-00001750: 652d 636f 6d6d 756e 6963 6174 696f 6e2d  e-communication-
-00001760: 7769 7468 2d75 7362 746d 632d 6661 712f  with-usbtmc-faq/
-00001770: 0d2e 2e20 5f74 6872 6561 643a 2068 7474  ... _thread: htt
-00001780: 7073 3a2f 2f72 6561 6c70 7974 686f 6e2e  ps://realpython.
-00001790: 636f 6d2f 696e 7472 6f2d 746f 2d70 7974  com/intro-to-pyt
-000017a0: 686f 6e2d 7468 7265 6164 696e 672f 0d2e  hon-threading/..
-000017b0: 2e20 5f51 5468 7265 6164 3a20 6874 7470  . _QThread: http
-000017c0: 733a 2f2f 646f 632e 7174 2e69 6f2f 7174  s://doc.qt.io/qt
-000017d0: 2d36 2f71 7468 7265 6164 2e68 746d 6c0d  -6/qthread.html.
+00000030: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a  --------------..
+00000040: 0d0a 416e 2069 6e73 7472 756d 656e 7420  ..An instrument 
+00000050: 636c 6173 7320 6973 2061 2073 7562 636c  class is a subcl
+00000060: 6173 7320 6465 7269 7665 6420 6672 6f6d  ass derived from
+00000070: 2074 6865 0d0a 3a63 6c61 7373 3a60 496e   the..:class:`In
+00000080: 7374 7275 6d65 6e74 3c73 7273 6775 692e  strument<srsgui.
+00000090: 696e 7374 2e69 6e73 7472 756d 656e 742e  inst.instrument.
+000000a0: 496e 7374 7275 6d65 6e74 3e60 2063 6c61  Instrument>` cla
+000000b0: 7373 2e0d 0a54 6865 202a 2a5f 4964 5374  ss...The **_IdSt
+000000c0: 7269 6e67 2a2a 206d 7573 7420 6265 2064  ring** must be d
+000000d0: 6566 696e 6564 2e20 0d0a 2854 6869 7320  efined. ..(This 
+000000e0: 6973 2075 7365 6420 746f 2063 6865 636b  is used to check
+000000f0: 2069 6620 6120 636f 6e6e 6563 7465 640d   if a connected.
+00000100: 0a69 6e73 7472 756d 656e 7420 6973 206f  .instrument is o
+00000110: 6620 7468 6520 7072 6f70 6572 2074 7970  f the proper typ
+00000120: 6520 746f 2062 6520 7573 6564 2077 6974  e to be used wit
+00000130: 6820 7468 6520 7375 6263 6c61 7373 292e  h the subclass).
+00000140: 0d0a 0d0a 2e2e 2063 6f64 652d 626c 6f63  ...... code-bloc
+00000150: 6b3a 3a0d 0a0d 0a20 2020 2066 726f 6d20  k::....    from 
+00000160: 7372 7367 7569 2069 6d70 6f72 7420 496e  srsgui import In
+00000170: 7374 7275 6d65 6e74 0d0a 2020 2020 636c  strument..    cl
+00000180: 6173 7320 4347 3633 3528 496e 7374 7275  ass CG635(Instru
+00000190: 6d65 6e74 293a 0d0a 2020 2020 2020 2020  ment):..        
+000001a0: 5f49 6453 7472 696e 6720 3d20 2743 4736  _IdString = 'CG6
+000001b0: 3335 270d 0a20 2020 2020 2020 205f 7465  35'..        _te
+000001c0: 726d 5f63 6861 7220 3d20 6227 5c72 2720  rm_char = b'\r' 
+000001d0: 2023 2041 6464 2074 6869 7320 6c69 6e65   # Add this line
+000001e0: 2069 6620 7468 6520 6361 7272 6961 6765   if the carriage
+000001f0: 2072 6574 7572 6e20 6973 2074 6865 2074   return is the t
+00000200: 6572 6d69 6e61 7469 6f6e 2063 6861 7261  ermination chara
+00000210: 6374 6572 0d0a 2020 2020 2020 2020 2020  cter..          
+00000220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000230: 2020 2320 6f66 2074 6865 2069 6e73 7472    # of the instr
+00000240: 756d 656e 742c 2069 6e73 7465 6164 206f  ument, instead o
+00000250: 6620 7468 6520 6c69 6e65 2066 6565 6420  f the line feed 
+00000260: 2841 5343 4949 3a20 3078 3130 2c20 6227  (ASCII: 0x10, b'
+00000270: 5c6e 2729 2e0d 0a0d 0a0d 0a49 6620 7468  \n').......If th
+00000280: 6520 696e 7374 7275 6d65 6e74 2068 6173  e instrument has
+00000290: 3a0d 0a20 2020 2031 2e20 7468 6520 2a2a  :..    1. the **
+000002a0: 5c2a 4944 4e3f 2a2a 2072 656d 6f74 6520  \*IDN?** remote 
+000002b0: 636f 6d6d 616e 642c 2061 6e64 0d0a 2020  command, and..  
+000002c0: 2020 322e 2065 6974 6865 7220 5253 3233    2. either RS23
+000002d0: 3220 7365 7269 616c 2063 6f6d 6d75 6e69  2 serial communi
+000002e0: 6361 7469 6f6e 206f 7220 4574 6865 726e  cation or Ethern
+000002f0: 6574 2054 4350 4950 2063 6f6d 6d75 6e69  et TCPIP communi
+00000300: 6361 7469 6f6e 2070 6f72 7420 6176 6169  cation port avai
+00000310: 6c61 626c 652c 0d0a 0d0a 7468 6520 696e  lable,....the in
+00000320: 7374 7275 6d65 6e74 2063 616e 2062 6520  strument can be 
+00000330: 636f 6e6e 6563 7465 6420 616e 6420 7573  connected and us
+00000340: 6564 2069 6e20 7461 736b 2073 6372 6970  ed in task scrip
+00000350: 7473 2061 6e64 2069 6e20 7468 6520 7465  ts and in the te
+00000360: 726d 696e 616c 2c0d 0a77 6974 6820 3420  rminal,..with 4 
+00000370: 6c69 6e65 7320 6f66 2064 6566 696e 6974  lines of definit
+00000380: 696f 6e2c 2061 7320 7368 6f77 6e20 6162  ion, as shown ab
+00000390: 6f76 652e 2049 6620 6974 2064 6f65 7320  ove. If it does 
+000003a0: 6e6f 7420 6861 7665 2061 205c 2a49 444e  not have a \*IDN
+000003b0: 3f20 7265 6d6f 7465 2063 6f6d 6d61 6e64  ? remote command
+000003c0: 2c0d 0a74 6865 203a 6d65 7468 3a60 6368  ,..the :meth:`ch
+000003d0: 6563 6b5f 6964 2829 3c73 7273 6775 692e  eck_id()<srsgui.
+000003e0: 696e 7374 2e69 6e73 7472 756d 656e 742e  inst.instrument.
+000003f0: 496e 7374 7275 6d65 6e74 2e63 6865 636b  Instrument.check
+00000400: 5f69 643e 6020 6d65 7468 6f64 2069 6e20  _id>` method in 
+00000410: 3a63 6c61 7373 3a60 496e 7374 7275 6d65  :class:`Instrume
+00000420: 6e74 3c73 7273 6775 692e 696e 7374 2e69  nt<srsgui.inst.i
+00000430: 6e73 7472 756d 656e 742e 496e 7374 7275  nstrument.Instru
+00000440: 6d65 6e74 3e60 0d0a 636c 6173 7320 6e65  ment>`..class ne
+00000450: 6564 7320 746f 2062 6520 7265 696d 706c  eds to be reimpl
+00000460: 656d 656e 7465 642e 0d0a 0d0a 4176 6169  emented.....Avai
+00000470: 6c61 626c 655f 696e 7465 7266 6163 6573  lable_interfaces
+00000480: 0d0a 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ..^^^^^^^^^^^^^^
+00000490: 5e5e 5e5e 5e5e 5e0d 0a0d 0a60 6176 6169  ^^^^^^^....`avai
+000004a0: 6c61 626c 655f 696e 7465 7266 6163 6573  lable_interfaces
+000004b0: 6020 6465 6669 6e65 7320 7768 6174 2063  ` defines what c
+000004c0: 6f6d 6d75 6e69 6361 7469 6f6e 2069 6e74  ommunication int
+000004d0: 6572 6661 6365 7320 6172 6520 6176 6169  erfaces are avai
+000004e0: 6c61 626c 6520 666f 7220 7468 6520 696e  lable for the in
+000004f0: 7374 7275 6d65 6e74 2e0d 0a54 6865 2062  strument...The b
+00000500: 6173 6520 3a63 6c61 7373 3a60 496e 7374  ase :class:`Inst
+00000510: 7275 6d65 6e74 3c73 7273 6775 692e 696e  rument<srsgui.in
+00000520: 7374 2e69 6e73 7472 756d 656e 742e 496e  st.instrument.In
+00000530: 7374 7275 6d65 6e74 3e60 2063 6c61 7373  strument>` class
+00000540: 2068 6173 2074 6865 2066 6f6c 6c6f 7769   has the followi
+00000550: 6e67 0d0a 6465 6669 6e69 7469 6f6e 2066  ng..definition f
+00000560: 6f72 2073 6572 6961 6c20 616e 6420 5443  or serial and TC
+00000570: 502f 4950 2063 6f6d 6d75 6e69 6361 7469  P/IP communicati
+00000580: 6f6e 2069 6e74 6572 6661 6365 733a 0d0a  on interfaces:..
+00000590: 0d0a 2e2e 2063 6f64 652d 626c 6f63 6b3a  .... code-block:
+000005a0: 3a0d 0a0d 0a20 2020 2061 7661 696c 6162  :....    availab
+000005b0: 6c65 5f69 6e74 6572 6661 6365 7320 3d20  le_interfaces = 
+000005c0: 5b0d 0a20 2020 2020 2020 205b 2020 2053  [..        [   S
+000005d0: 6572 6961 6c49 6e74 6572 6661 6365 2c0d  erialInterface,.
+000005e0: 0a20 2020 2020 2020 2020 2020 207b 0d0a  .            {..
+000005f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000600: 2770 6f72 7427 3a20 4669 6e64 4c69 7374  'port': FindList
+00000610: 496e 7075 7428 292c 0d0a 2020 2020 2020  Input(),..      
+00000620: 2020 2020 2020 2020 2020 2762 6175 645f            'baud_
+00000630: 7261 7465 273a 2049 6e74 6567 6572 4c69  rate': IntegerLi
+00000640: 7374 496e 7075 7428 5b39 3630 302c 2031  stInput([9600, 1
+00000650: 3135 3230 305d 292c 0d0a 2020 2020 2020  15200]),..      
+00000660: 2020 2020 2020 2020 2020 2768 6172 6477            'hardw
+00000670: 6172 655f 666c 6f77 5f63 6f6e 7472 6f6c  are_flow_control
+00000680: 273a 2042 6f6f 6c49 6e70 7574 285b 274f  ': BoolInput(['O
+00000690: 6666 272c 2027 4f6e 275d 290d 0a20 2020  ff', 'On'])..   
+000006a0: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
+000006b0: 2020 2020 5d2c 0d0a 2020 2020 2020 2020      ],..        
+000006c0: 5b20 2020 5463 7069 7049 6e74 6572 6661  [   TcpipInterfa
+000006d0: 6365 2c0d 0a20 2020 2020 2020 2020 2020  ce,..           
+000006e0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+000006f0: 2020 2020 2769 705f 6164 6472 6573 7327      'ip_address'
+00000700: 3a20 4970 3449 6e70 7574 2827 3139 322e  : Ip4Input('192.
+00000710: 3136 382e 312e 3130 2729 2c0d 0a20 2020  168.1.10'),..   
+00000720: 2020 2020 2020 2020 2020 2020 2027 706f               'po
+00000730: 7274 273a 2049 6e74 6567 6572 496e 7075  rt': IntegerInpu
+00000740: 7428 3233 290d 0a20 2020 2020 2020 2020  t(23)..         
+00000750: 2020 207d 0d0a 2020 2020 2020 2020 5d0d     }..        ].
+00000760: 0a20 2020 205d 0d0a 0d0a 4966 2079 6f75  .    ]....If you
+00000770: 7220 696e 7374 7275 6d65 6e74 206e 6565  r instrument nee
+00000780: 6473 2069 6e74 6572 6661 6365 7320 6f74  ds interfaces ot
+00000790: 6865 7220 7468 616e 2073 6572 6961 6c20  her than serial 
+000007a0: 616e 6420 5443 502f 4950 2c20 0d0a 6060  and TCP/IP, ..``
+000007b0: 7372 7367 7569 6060 2061 6c6c 6f77 7320  srsgui`` allows 
+000007c0: 6164 6469 7469 6f6e 616c 2063 6f6d 6d75  additional commu
+000007d0: 6e69 6361 7469 6f6e 2063 6c61 7373 6573  nication classes
+000007e0: 2064 6572 6976 6564 2066 726f 6d20 7468   derived from th
+000007f0: 650d 0a3a 636c 6173 733a 6049 6e74 6572  e..:class:`Inter
+00000800: 6661 6365 203c 7372 7367 7569 2e69 6e73  face <srsgui.ins
+00000810: 742e 636f 6d6d 756e 6963 6174 696f 6e2e  t.communication.
+00000820: 696e 7465 7266 6163 652e 496e 7465 7266  interface.Interf
+00000830: 6163 653e 6020 636c 6173 732e 0d0a 4375  ace>` class...Cu
+00000840: 7272 656e 746c 7920 7468 6572 6520 6172  rrently there ar
+00000850: 6520 7477 6f20 6578 7465 726e 616c 2063  e two external c
+00000860: 6f6d 6d75 6e69 6361 7469 6f6e 2069 6e74  ommunication int
+00000870: 6572 6661 6365 7320 6176 6169 6c61 626c  erfaces availabl
+00000880: 6520 6672 6f6d 2074 6865 0d0a 6073 7273  e from the..`srs
+00000890: 696e 7374 2e73 7238 3630 605f 2070 6163  inst.sr860`_ pac
+000008a0: 6b61 6765 3a20 6060 5678 6931 3149 6e74  kage: ``Vxi11Int
+000008b0: 6572 6661 6365 6060 2061 6e64 2060 6056  erface`` and ``V
+000008c0: 6973 6149 6e74 6572 6661 6365 6060 2c0d  isaInterface``,.
+000008d0: 0a77 6869 6368 2063 6f76 6572 7320 666f  .which covers fo
+000008e0: 7220 5658 4931 315f 2c20 4750 4942 5f20  r VXI11_, GPIB_ 
+000008f0: 616e 6420 5553 422d 544d 435f 2e20 596f  and USB-TMC_. Yo
+00000900: 7520 6361 6e20 696d 706f 7274 2074 6865  u can import the
+00000910: 2069 6e74 6572 6661 6365 206d 6f64 756c   interface modul
+00000920: 6573 0d0a 6672 6f6d 2060 7372 7369 6e73  es..from `srsins
+00000930: 742e 7372 3836 3060 5f20 2e0d 0a0d 0a60  t.sr860`_ .....`
+00000940: 6176 6169 6c61 626c 655f 696e 7465 7266  available_interf
+00000950: 6163 6573 6020 696e 2074 6865 2053 5238  aces` in the SR8
+00000960: 3630 2063 6c61 7373 2069 7320 6465 6669  60 class is defi
+00000970: 6e65 6420 6173 2066 6f6c 6c6f 7769 6e67  ned as following
+00000980: 3a0d 0a0d 0a2e 2e20 636f 6465 2d62 6c6f  :...... code-blo
+00000990: 636b 3a3a 0d0a 0d0a 2020 2020 6176 6169  ck::....    avai
+000009a0: 6c61 626c 655f 696e 7465 7266 6163 6573  lable_interfaces
+000009b0: 203d 205b 0d0a 2020 2020 2020 2020 5b20   = [..        [ 
+000009c0: 2020 5678 6931 3149 6e74 6572 6661 6365    Vxi11Interface
+000009d0: 2c0d 0a20 2020 2020 2020 2020 2020 207b  ,..            {
+000009e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000009f0: 2020 2769 705f 6164 6472 6573 7327 3a20    'ip_address': 
+00000a00: 4970 3449 6e70 7574 2827 3139 322e 3136  Ip4Input('192.16
+00000a10: 382e 312e 3130 2729 2c0d 0a20 2020 2020  8.1.10'),..     
+00000a20: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
+00000a30: 2020 5d2c 0d0a 2020 2020 2020 2020 5b20    ],..        [ 
+00000a40: 2020 5669 7361 496e 7465 7266 6163 652c    VisaInterface,
+00000a50: 0d0a 2020 2020 2020 2020 2020 2020 7b0d  ..            {.
+00000a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000a70: 2027 7265 736f 7572 6365 273a 2046 696e   'resource': Fin
+00000a80: 644c 6973 7449 6e70 7574 2829 2c0d 0a20  dListInput(),.. 
+00000a90: 2020 2020 2020 2020 2020 207d 0d0a 2020             }..  
+00000aa0: 2020 2020 2020 5d2c 0d0a 2020 2020 2020        ],..      
+00000ab0: 2020 5b20 2020 5463 7069 7049 6e74 6572    [   TcpipInter
+00000ac0: 6661 6365 2c0d 0a20 2020 2020 2020 2020  face,..         
+00000ad0: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
+00000ae0: 2020 2020 2020 2769 705f 6164 6472 6573        'ip_addres
+00000af0: 7327 3a20 4970 3449 6e70 7574 2827 3139  s': Ip4Input('19
+00000b00: 322e 3136 382e 312e 3130 2729 2c0d 0a20  2.168.1.10'),.. 
+00000b10: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00000b20: 706f 7274 273a 2032 330d 0a20 2020 2020  port': 23..     
+00000b30: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
+00000b40: 2020 5d2c 0d0a 2020 2020 2020 2020 5b20    ],..        [ 
+00000b50: 2020 5365 7269 616c 496e 7465 7266 6163    SerialInterfac
+00000b60: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00000b70: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
+00000b80: 2020 2027 706f 7274 273a 2046 696e 644c     'port': FindL
+00000b90: 6973 7449 6e70 7574 2829 2c0d 0a20 2020  istInput(),..   
+00000ba0: 2020 2020 2020 2020 2020 2020 2027 6261               'ba
+00000bb0: 7564 5f72 6174 6527 3a20 496e 7465 6765  ud_rate': Intege
+00000bc0: 724c 6973 7449 6e70 7574 285b 3936 3030  rListInput([9600
+00000bd0: 2c20 3139 3230 302c 2033 3834 3030 2c20  , 19200, 38400, 
+00000be0: 3131 3532 3030 2c0d 0a20 2020 2020 2020  115200,..       
+00000bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c10: 2020 2020 2020 2020 3233 3034 3030 2c20          230400, 
+00000c20: 3436 3038 3030 5d2c 2033 290d 0a20 2020  460800], 3)..   
+00000c30: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
+00000c40: 2020 2020 5d2c 0d0a 2020 2020 5d0d 0a0d      ],..    ]...
+00000c50: 0a44 6566 696e 696e 6720 6061 7661 696c  .Defining `avail
+00000c60: 6162 6c65 5f69 6e74 6572 6661 6365 7360  able_interfaces`
+00000c70: 2069 7320 616c 6c20 796f 7520 6e65 6564   is all you need
+00000c80: 2074 6f20 646f 2074 6f20 6765 7420 6120   to do to get a 
+00000c90: 6375 7374 6f6d 697a 6564 0d0a 6469 616c  customized..dial
+00000ca0: 6f67 2062 6f78 206f 7065 6e65 6420 666f  og box opened fo
+00000cb0: 7220 7468 6520 696e 7374 7275 6d65 6e74  r the instrument
+00000cc0: 2069 6e20 6060 7372 7367 7569 6060 2061   in ``srsgui`` a
+00000cd0: 7070 6c69 6361 7469 6f6e 2e0d 0a0d 0a2e  pplication......
+00000ce0: 2e20 6669 6775 7265 3a3a 202e 2f5f 7374  . figure:: ./_st
+00000cf0: 6174 6963 2f63 6f6e 6e65 6374 2d64 6961  atic/connect-dia
+00000d00: 6c6f 672d 626f 782d 6361 7074 7572 652e  log-box-capture.
+00000d10: 706e 670d 0a20 2020 203a 616c 6967 6e3a  png..    :align:
+00000d20: 2063 656e 7465 720d 0a20 2020 203a 6669   center..    :fi
+00000d30: 6763 6c61 7373 3a20 616c 6967 6e2d 6365  gclass: align-ce
+00000d40: 6e74 6572 0d0a 0d0a 466f 7220 6060 5669  nter....For ``Vi
+00000d50: 7361 496e 7465 7266 6163 6560 602c 2079  saInterface``, y
+00000d60: 6f75 2068 6176 6520 746f 2067 6574 2050  ou have to get P
+00000d70: 7956 4953 415f 2077 6f72 6b69 6e67 2062  yVISA_ working b
+00000d80: 6566 6f72 6520 7275 6e6e 696e 6720 6060  efore running ``
+00000d90: 7372 7367 7569 6060 2061 7070 6c69 6361  srsgui`` applica
+00000da0: 7469 6f6e 2e0d 0a54 6869 7320 696e 766f  tion...This invo
+00000db0: 6c76 6573 2069 6e73 7461 6c6c 6174 696f  lves installatio
+00000dc0: 6e20 6f66 2074 6865 2050 7956 4953 4120  n of the PyVISA 
+00000dd0: 7061 636b 6167 6520 616e 6420 6974 7320  package and its 
+00000de0: 6261 636b 656e 6420 6c69 6272 6172 792e  backend library.
+00000df0: 0d0a 5265 6665 7220 746f 2050 7956 4953  ..Refer to PyVIS
+00000e00: 415f 2064 6f63 756d 656e 7461 7469 6f6e  A_ documentation
+00000e10: 2066 6f72 2069 6e73 7461 6c6c 6174 696f   for installatio
+00000e20: 6e20 6465 7461 696c 732e 0d0a 0d0a 496e  n details.....In
+00000e30: 7465 7261 6374 696e 6720 7769 7468 2061  teracting with a
+00000e40: 6e20 696e 7374 7275 6d65 6e74 0d0a 5e5e  n instrument..^^
+00000e50: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ^^^^^^^^^^^^^^^^
+00000e60: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 0d0a 0d0a  ^^^^^^^^^^^^....
+00000e70: 4f6e 6365 2061 6e20 6060 496e 7374 7275  Once an ``Instru
+00000e80: 6d65 6e74 6060 2063 6c61 7373 2069 7320  ment`` class is 
+00000e90: 6465 6669 6e65 642c 2079 6f75 2063 616e  defined, you can
+00000ea0: 2063 6f6e 6e65 6374 2074 6f20 616e 6420   connect to and 
+00000eb0: 636f 6d6d 756e 6963 6174 6520 7769 7468  communicate with
+00000ec0: 2074 6865 2069 6e73 7472 756d 656e 7420   the instrument 
+00000ed0: 0d0a 7669 6120 6b65 7962 6f61 7264 2062  ..via keyboard b
+00000ee0: 7920 6c61 756e 6368 696e 6720 6120 5079  y launching a Py
+00000ef0: 7468 6f6e 2069 6e74 6572 7072 6574 6572  thon interpreter
+00000f00: 2066 726f 6d20 796f 7572 2063 6f6d 6d61   from your comma
+00000f10: 6e64 2070 726f 6d70 743a 0d0a 0d0a 2e2e  nd prompt:......
+00000f20: 2063 6f64 652d 626c 6f63 6b3a 3a0d 0a0d   code-block::...
+00000f30: 0a20 2020 2043 3a5c 7372 7367 7569 3e70  .    C:\srsgui>p
+00000f40: 7974 686f 6e0d 0a20 2020 2050 7974 686f  ython..    Pytho
+00000f50: 6e20 332e 382e 3320 2874 6167 732f 7633  n 3.8.3 (tags/v3
+00000f60: 2e38 2e33 3a36 6638 6338 3332 2c20 4d61  .8.3:6f8c832, Ma
+00000f70: 7920 3133 2032 3032 302c 2032 323a 3337  y 13 2020, 22:37
+00000f80: 3a30 3229 205b 4d53 4320 762e 3139 3234  :02) [MSC v.1924
+00000f90: 2036 3420 6269 7420 2841 4d44 3634 295d   64 bit (AMD64)]
+00000fa0: 206f 6e20 7769 6e33 320d 0a20 2020 2054   on win32..    T
+00000fb0: 7970 6520 2268 656c 7022 2c20 2263 6f70  ype "help", "cop
+00000fc0: 7972 6967 6874 222c 2022 6372 6564 6974  yright", "credit
+00000fd0: 7322 206f 7220 226c 6963 656e 7365 2220  s" or "license" 
+00000fe0: 666f 7220 6d6f 7265 2069 6e66 6f72 6d61  for more informa
+00000ff0: 7469 6f6e 2e0d 0a20 2020 203e 3e3e 0d0a  tion...    >>>..
+00001000: 2020 2020 3e3e 3e20 6672 6f6d 2073 7273      >>> from srs
+00001010: 696e 7374 2e73 7238 3630 2069 6d70 6f72  inst.sr860 impor
+00001020: 7420 5352 3836 300d 0a20 2020 203e 3e3e  t SR860..    >>>
+00001030: 2066 726f 6d20 7372 7367 7569 2069 6d70   from srsgui imp
+00001040: 6f72 7420 5365 7269 616c 496e 7465 7266  ort SerialInterf
+00001050: 6163 650d 0a20 2020 203e 3e3e 2053 6572  ace..    >>> Ser
+00001060: 6961 6c49 6e74 6572 6661 6365 2e66 696e  ialInterface.fin
+00001070: 6428 290d 0a20 2020 205b 2743 4f4d 3327  d()..    ['COM3'
+00001080: 2c20 2743 4f4d 3427 2c20 2743 4f4d 3235  , 'COM4', 'COM25
+00001090: 3627 5d0d 0a20 2020 203e 3e3e 206c 6961  6']..    >>> lia
+000010a0: 203d 2053 5238 3630 2827 7365 7269 616c   = SR860('serial
+000010b0: 272c 2743 4f4d 3427 2c31 3135 3230 302c  ','COM4',115200,
+000010c0: 2046 616c 7365 290d 0a20 2020 203e 3e3e   False)..    >>>
+000010d0: 206c 6961 2e71 7565 7279 5f74 6578 7428   lia.query_text(
+000010e0: 272a 6964 6e3f 2729 0d0a 2020 2020 2753  '*idn?')..    'S
+000010f0: 7461 6e66 6f72 645f 5265 7365 6172 6368  tanford_Research
+00001100: 5f53 7973 7465 6d73 2c53 5238 3635 412c  _Systems,SR865A,
+00001110: 3030 3237 3235 2c76 312e 3334 270d 0a20  002725,v1.34'.. 
+00001120: 2020 203e 3e3e 206c 6961 2e64 6973 636f     >>> lia.disco
+00001130: 6e6e 6563 7428 290d 0a20 2020 203e 3e3e  nnect()..    >>>
+00001140: 0d0a 2020 2020 3e3e 3e20 6672 6f6d 2073  ..    >>> from s
+00001150: 7273 696e 7374 2e73 7238 3630 2069 6d70  rsinst.sr860 imp
+00001160: 6f72 7420 5669 7361 496e 7465 7266 6163  ort VisaInterfac
+00001170: 650d 0a20 2020 203e 3e3e 2056 6973 6149  e..    >>> VisaI
+00001180: 6e74 6572 6661 6365 2e66 696e 6428 290d  nterface.find().
+00001190: 0a20 2020 205b 2755 5342 303a 3a30 7842  .    ['USB0::0xB
+000011a0: 3530 363a 3a30 7832 3030 303a 3a30 3032  506::0x2000::002
+000011b0: 3732 353a 3a49 4e53 5452 272c 2027 4750  725::INSTR', 'GP
+000011c0: 4942 303a 3a34 3a3a 494e 5354 5227 5d0d  IB0::4::INSTR'].
+000011d0: 0a20 2020 203e 3e3e 206c 6961 2e63 6f6e  .    >>> lia.con
+000011e0: 6e65 6374 2827 7669 7361 272c 2027 5553  nect('visa', 'US
+000011f0: 4230 3a3a 3078 4235 3036 3a3a 3078 3230  B0::0xB506::0x20
+00001200: 3030 3a3a 3030 3237 3235 3a3a 494e 5354  00::002725::INST
+00001210: 5227 290d 0a20 2020 203e 3e3e 206c 6961  R')..    >>> lia
+00001220: 2e71 7565 7279 5f74 6578 7428 272a 6964  .query_text('*id
+00001230: 6e3f 2729 0d0a 2020 2020 2753 7461 6e66  n?')..    'Stanf
+00001240: 6f72 645f 5265 7365 6172 6368 5f53 7973  ord_Research_Sys
+00001250: 7465 6d73 2c53 5238 3635 412c 3030 3237  tems,SR865A,0027
+00001260: 3235 2c76 312e 3334 5c6e 270d 0a20 2020  25,v1.34\n'..   
+00001270: 203e 3e3e 0d0a 0d0a 4675 7274 6865 726d   >>>....Furtherm
+00001280: 6f72 652c 2062 7920 6164 6469 6e67 2074  ore, by adding t
+00001290: 6865 2069 6e73 7472 756d 656e 7420 746f  he instrument to
+000012a0: 2061 202e 7461 736b 636f 6e66 6967 2066   a .taskconfig f
+000012b0: 696c 6520 0d0a 616e 6420 6f70 656e 696e  ile ..and openin
+000012c0: 6720 7468 6520 2e74 6173 6b63 6f6e 6669  g the .taskconfi
+000012d0: 6720 6669 6c65 2069 6e20 7468 6520 6060  g file in the ``
+000012e0: 7372 7367 7569 6060 2061 7070 6c69 6361  srsgui`` applica
+000012f0: 7469 6f6e 2c20 0d0a 796f 7520 6361 6e20  tion, ..you can 
+00001300: 7573 6520 7468 6520 6275 696c 742d 696e  use the built-in
+00001310: 2074 6572 6d69 6e61 6c20 746f 2069 6e74   terminal to int
+00001320: 6572 6163 7420 7769 7468 206d 756c 7469  eract with multi
+00001330: 706c 6520 696e 7374 7275 6d65 6e74 7320  ple instruments 
+00001340: 6174 206f 6e63 652c 200d 0a61 6e64 2075  at once, ..and u
+00001350: 7365 2068 6967 6820 6c65 7665 6c20 6060  se high level ``
+00001360: 496e 7374 7275 6d65 6e74 6060 2063 6c61  Instrument`` cla
+00001370: 7373 2061 7474 7269 6275 7465 7320 616e  ss attributes an
+00001380: 6420 6d65 7468 6f64 732e 0d0a 0d0a 4265  d methods.....Be
+00001390: 6c6f 7720 6973 2061 6e20 696d 6167 6520  low is an image 
+000013a0: 6f66 2074 6865 2060 6073 7273 6775 6960  of the ``srsgui`
+000013b0: 6020 6170 706c 6963 6174 696f 6e20 6361  ` application ca
+000013c0: 7074 7572 6564 2077 6974 6820 7468 6520  ptured with the 
+000013d0: 6578 616d 706c 6520 7072 6f6a 6563 7420  example project 
+000013e0: 6f70 656e 6564 2e0d 0a41 7320 796f 7520  opened...As you 
+000013f0: 6361 6e20 7365 652c 2079 6f75 2063 616e  can see, you can
+00001400: 2069 6e74 6572 6163 7420 7769 7468 2074   interact with t
+00001410: 6865 2063 6c6f 636b 2067 656e 6572 6174  he clock generat
+00001420: 6f72 2061 6e64 206f 7363 696c 6c6f 7363  or and oscillosc
+00001430: 6f70 6520 696e 206d 616e 7920 7761 7973  ope in many ways
+00001440: 2e0d 0a59 6f75 2063 616e 2073 6565 2074  ...You can see t
+00001450: 776f 2065 7861 6d70 6c65 7320 6f66 2020  wo examples of  
+00001460: 636f 6d6d 616e 6473 2073 656e 7420 746f  commands sent to
+00001470: 2074 6865 206f 7363 696c 6c6f 7363 6f70   the oscilloscop
+00001480: 6520 6060 6f73 6360 603a 200d 0a60 605c  e ``osc``: ..``\
+00001490: 2a69 646e 3f60 602c 2061 6e64 2060 6073  *idn?``, and ``s
+000014a0: 6172 613f 6060 0d0a 6173 2077 656c 6c20  ara?``..as well 
+000014b0: 6173 2074 776f 2063 6f6d 6d61 6e64 7320  as two commands 
+000014c0: 7365 6e74 2074 6f20 7468 6520 7468 6520  sent to the the 
+000014d0: 636c 6f63 6b20 6765 6e65 7261 746f 7220  clock generator 
+000014e0: 6060 6367 6060 0d0a 6060 5c2a 6964 6e3f  ``cg``..``\*idn?
+000014f0: 6060 2c20 616e 6420 6060 6672 6571 283f  ``, and ``freq(?
+00001500: 2960 602e 0d0a 0d0a 2e2e 2066 6967 7572  )``....... figur
+00001510: 653a 3a20 2e2f 5f73 7461 7469 632f 7465  e:: ./_static/te
+00001520: 726d 696e 616c 2d77 6974 682d 6578 616d  rminal-with-exam
+00001530: 706c 652e 706e 670d 0a20 2020 203a 616c  ple.png..    :al
+00001540: 6967 6e3a 2063 656e 7465 720d 0a20 2020  ign: center..   
+00001550: 203a 6669 6763 6c61 7373 3a20 616c 6967   :figclass: alig
+00001560: 6e2d 6365 6e74 6572 0d0a 0d0a 7c0d 0a0d  n-center....|...
+00001570: 0a0d 0a43 6f6d 706f 6e65 6e74 2c20 436f  ...Component, Co
+00001580: 6d6d 616e 6473 2061 6e64 2049 6e64 6578  mmands and Index
+00001590: 436f 6d6d 616e 6473 0d0a 5e5e 5e5e 5e5e  Commands..^^^^^^
+000015a0: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ^^^^^^^^^^^^^^^^
+000015b0: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  ^^^^^^^^^^^^^^^^
+000015c0: 0d0a 0d0a 3a63 6c61 7373 3a60 496e 7374  ....:class:`Inst
+000015d0: 7275 6d65 6e74 203c 7372 7367 7569 2e69  rument <srsgui.i
+000015e0: 6e73 742e 696e 7374 7275 6d65 6e74 2e49  nst.instrument.I
+000015f0: 6e73 7472 756d 656e 743e 6020 636c 6173  nstrument>` clas
+00001600: 7320 7573 6573 0d0a 3a63 6c61 7373 3a60  s uses..:class:`
+00001610: 436f 6d70 6f6e 656e 7420 3c73 7273 6775  Component <srsgu
+00001620: 692e 696e 7374 2e63 6f6d 706f 6e65 6e74  i.inst.component
+00001630: 2e43 6f6d 706f 6e65 6e74 3e60 2063 6c61  .Component>` cla
+00001640: 7373 2c0d 0a3a 6d6f 643a 6043 6f6d 6d61  ss,..:mod:`Comma
+00001650: 6e64 203c 7372 7367 7569 2e69 6e73 742e  nd <srsgui.inst.
+00001660: 636f 6d6d 616e 6473 3e60 2063 6c61 7373  commands>` class
+00001670: 6573 2061 6e64 0d0a 3a6d 6f64 3a60 496e  es and..:mod:`In
+00001680: 6465 7843 6f6d 6d61 6e64 203c 7372 7367  dexCommand <srsg
+00001690: 7569 2e69 6e73 742e 696e 6465 7863 6f6d  ui.inst.indexcom
+000016a0: 6d61 6e64 733e 6020 636c 6173 7365 730d  mands>` classes.
+000016b0: 0a74 6f20 6f72 6761 6e69 7a65 2074 6865  .to organize the
+000016c0: 2066 756e 6374 696f 6e61 6c69 7479 206f   functionality o
+000016d0: 6620 616e 2069 6e73 7472 756d 656e 742e  f an instrument.
+000016e0: 0d0a 0d0a 4966 2079 6f75 2068 6176 6520  ....If you have 
+000016f0: 746f 2064 6561 6c20 7769 7468 2068 756e  to deal with hun
+00001700: 6472 6564 7320 6f66 2072 656d 6f74 6520  dreds of remote 
+00001710: 636f 6d6d 616e 6473 2074 6f20 7573 6520  commands to use 
+00001720: 616e 2069 6e73 7472 756d 656e 7420 7265  an instrument re
+00001730: 6d6f 7465 6c79 2c0d 0a6f 7267 616e 697a  motely,..organiz
+00001740: 696e 6720 7468 656d 2069 6e20 6120 6d61  ing them in a ma
+00001750: 6e61 6765 6162 6c65 2077 6179 2069 7320  nageable way is 
+00001760: 6372 7563 6961 6c2e 2060 5372 7369 6e73  crucial. `Srsins
+00001770: 742e 7372 3836 3060 5f20 7061 636b 6167  t.sr860`_ packag
+00001780: 6520 7368 6f77 7320 686f 7720 7468 6573  e shows how thes
+00001790: 650d 0a63 6f6e 7665 6e69 656e 6365 2063  e..convenience c
+000017a0: 6c61 7373 6573 2061 7265 2075 7365 6420  lasses are used 
+000017b0: 746f 206f 7267 616e 697a 6520 6120 6c61  to organize a la
+000017c0: 7267 6520 7365 7420 6f66 2072 656d 6f74  rge set of remot
+000017d0: 6520 636f 6d6d 616e 6473 2e0d 0a0d 0a0d  e commands......
+000017e0: 0a2e 2e20 5f50 7956 6973 613a 2068 7474  ... _PyVisa: htt
+000017f0: 7073 3a2f 2f70 7976 6973 612e 7265 6164  ps://pyvisa.read
+00001800: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+00001810: 7465 7374 2f0d 0a2e 2e20 5f73 7273 696e  test/.... _srsin
+00001820: 7374 2e73 7238 3630 3a20 6874 7470 733a  st.sr860: https:
+00001830: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
+00001840: 6374 2f73 7273 696e 7374 2e73 7238 3630  ct/srsinst.sr860
+00001850: 2f0d 0a2e 2e20 5f56 5849 3131 3a20 6874  /.... _VXI11: ht
+00001860: 7470 733a 2f2f 7777 772e 6c78 6973 7461  tps://www.lxista
+00001870: 6e64 6172 642e 6f72 672f 4162 6f75 742f  ndard.org/About/
+00001880: 5658 492d 3131 2d61 6e64 2d4c 5849 2e61  VXI-11-and-LXI.a
+00001890: 7370 780d 0a2e 2e20 5f47 5049 423a 2068  spx.... _GPIB: h
+000018a0: 7474 7073 3a2f 2f65 6e2e 7769 6b69 7065  ttps://en.wikipe
+000018b0: 6469 612e 6f72 672f 7769 6b69 2f49 4545  dia.org/wiki/IEE
+000018c0: 452d 3438 380d 0a2e 2e20 5f55 5342 2d54  E-488.... _USB-T
+000018d0: 4d43 3a20 6874 7470 733a 2f2f 7777 772e  MC: https://www.
+000018e0: 7465 7374 616e 646d 6561 7375 7265 6d65  testandmeasureme
+000018f0: 6e74 7469 7073 2e63 6f6d 2f72 656d 6f74  nttips.com/remot
+00001900: 652d 636f 6d6d 756e 6963 6174 696f 6e2d  e-communication-
+00001910: 7769 7468 2d75 7362 746d 632d 6661 712f  with-usbtmc-faq/
+00001920: 0d0a 2e2e 205f 7468 7265 6164 3a20 6874  .... _thread: ht
+00001930: 7470 733a 2f2f 7265 616c 7079 7468 6f6e  tps://realpython
+00001940: 2e63 6f6d 2f69 6e74 726f 2d74 6f2d 7079  .com/intro-to-py
+00001950: 7468 6f6e 2d74 6872 6561 6469 6e67 2f0d  thon-threading/.
+00001960: 0a2e 2e20 5f51 5468 7265 6164 3a20 6874  ... _QThread: ht
+00001970: 7470 733a 2f2f 646f 632e 7174 2e69 6f2f  tps://doc.qt.io/
+00001980: 7174 2d36 2f71 7468 7265 6164 2e68 746d  qt-6/qthread.htm
+00001990: 6c0d 0a                                  l..
```

### Comparing `srsgui-0.4.0.1/docs/example.rst` & `srsgui-0.4.1/docs/example.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,978 +1,1039 @@
 00000000: 0d0a 2e2e 205f 746f 702d 6f66 2d65 7861  .... _top-of-exa
 00000010: 6d70 6c65 2d70 726f 6a65 6374 3a0d 0a0d  mple-project:...
 00000020: 0a45 7861 6d70 6c65 2070 726f 6a65 6374  .Example project
 00000030: 0d0a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ..==============
 00000040: 3d3d 3d0d 0a0d 0a57 6865 6e20 796f 7520  ===....When you 
 00000050: 7275 6e20 7468 6520 6060 7372 7367 7569  run the ``srsgui
 00000060: 6060 2061 7070 6c69 6361 7469 6f6e 2c20  `` application, 
-00000070: 6974 2073 686f 7773 2069 6e20 7468 6520  it shows in the 
-00000080: 636f 6e73 6f6c 6520 7769 6e64 6f77 0d0a  console window..
-00000090: 7768 6572 6520 7468 6520 5079 7468 6f6e  where the Python
-000000a0: 2069 7320 7275 6e6e 696e 6720 6672 6f6d   is running from
-000000b0: 2c20 616e 6420 7768 6572 6520 6060 7372  , and where ``sr
-000000c0: 7367 7569 6060 2069 7320 6c6f 6361 7465  sgui`` is locate
-000000d0: 642e 0d0a 4966 2079 6f75 2067 6f20 696e  d...If you go in
-000000e0: 746f 2074 6865 2064 6972 6563 746f 7279  to the directory
-000000f0: 2077 6865 7265 2060 6073 7273 6775 6960   where ``srsgui`
-00000100: 6020 7265 7369 6465 732c 2079 6f75 2063  ` resides, you c
-00000110: 616e 2066 696e 640d 0a74 6865 2027 6578  an find..the 'ex
-00000120: 616d 706c 6573 2720 6469 7265 6374 6f72  amples' director
-00000130: 792e 2057 6865 6e20 796f 7520 6669 6e64  y. When you find
-00000140: 2061 2020 2e74 6173 6b63 6f6e 6669 6720   a  .taskconfig 
-00000150: 6669 6c65 2069 6e20 226f 7363 696c 6c6f  file in "oscillo
-00000160: 7363 6f70 6520 6578 616d 706c 6522 0d0a  scope example"..
-00000170: 6469 7265 6374 6f72 792c 204f 7065 6e20  directory, Open 
-00000180: 7468 6520 6669 6c65 2066 726f 6d20 7468  the file from th
-00000190: 6520 6d65 6e75 202a 2f46 696c 652f 4f70  e menu */File/Op
-000001a0: 656e 2043 6f6e 6669 672a 206f 6620 6060  en Config* of ``
-000001b0: 7372 7367 7569 6060 2061 7070 6c69 6361  srsgui`` applica
-000001c0: 7469 6f6e 2e0d 0a49 6620 796f 7520 706c  tion...If you pl
-000001d0: 616e 2074 6f20 6d6f 6469 6679 2066 696c  an to modify fil
-000001e0: 6573 2069 6e20 7468 6520 7072 6f6a 6563  es in the projec
-000001f0: 742c 2079 6f75 2062 6574 7465 7220 636f  t, you better co
-00000200: 7079 2074 6865 2077 686f 6c65 2065 7861  py the whole exa
-00000210: 6d70 6c65 2064 6972 6563 746f 7279 0d0a  mple directory..
-00000220: 746f 2077 6865 7265 2079 6f75 2075 7375  to where you usu
-00000230: 616c 6c79 206b 6565 7020 796f 7572 2064  ally keep your d
-00000240: 6f63 756d 656e 7473 2066 6f72 2070 726f  ocuments for pro
-00000250: 6772 616d 696e 672e 2041 6e64 206f 7065  graming. And ope
-00000260: 6e20 7468 6520 2e74 6173 6b63 6f6e 6669  n the .taskconfi
-00000270: 6720 6669 6c65 0d0a 666f 726d 2074 6865  g file..form the
-00000280: 2063 6f70 6965 6420 6469 7265 6374 6f72   copied director
-00000290: 792c 2074 6865 6e20 6e6f 2077 6f72 7269  y, then no worri
-000002a0: 6573 2061 626f 7574 206c 6f73 696e 6720  es about losing 
-000002b0: 7468 6520 6f72 6967 696e 616c 2066 696c  the original fil
-000002c0: 6573 2e0d 0a0d 0a41 7320 616e 2065 7861  es.....As an exa
-000002d0: 6d70 6c65 2070 726f 6a65 6374 206f 6620  mple project of 
-000002e0: 6060 7372 7367 7569 6060 2c20 4920 7761  ``srsgui``, I wa
-000002f0: 6e74 6564 2074 6f20 7573 6520 7562 6971  nted to use ubiq
-00000300: 7569 746f 7573 206d 6561 7375 7265 6d65  uitous measureme
-00000310: 6e74 0d0a 696e 7374 7275 6d65 6e74 7320  nt..instruments 
-00000320: 7769 7468 2072 656d 6f74 6520 636f 6d6d  with remote comm
-00000330: 756e 6963 6174 696f 6e20 6176 6169 6c61  unication availa
-00000340: 626c 652e 2049 2068 6170 7065 6e65 6420  ble. I happened 
-00000350: 746f 2068 6176 6520 616e 0d0a 6f73 6369  to have an..osci
-00000360: 6c6c 6f73 636f 7065 2061 6e64 2061 2066  lloscope and a f
-00000370: 756e 6374 696f 6e20 6765 6e65 7261 746f  unction generato
-00000380: 7220 286d 6f72 6520 7370 6563 6966 6963  r (more specific
-00000390: 616c 6c79 2c20 6120 636c 6f63 6b20 6765  ally, a clock ge
-000003a0: 6e65 7261 746f 7229 0d0a 6f6e 206d 7920  nerator)..on my 
-000003b0: 6465 736b 3a0d 0a0d 0a20 2020 202d 2053  desk:....    - S
-000003c0: 6967 6c65 6e74 2053 4453 3132 3032 5845  iglent SDS1202XE
-000003d0: 5f20 6469 6769 7461 6c20 6f73 6369 6c6c  _ digital oscill
-000003e0: 6f73 636f 7065 2028 3120 4753 612f 732c  oscope (1 GSa/s,
-000003f0: 2032 3030 204d 487a 2062 616e 6477 6964   200 MHz bandwid
-00000400: 7468 292c 0d0a 2020 2020 2020 4920 626f  th),..      I bo
-00000410: 7567 6874 2069 7420 6265 6361 7573 6520  ught it because 
-00000420: 6f66 2069 7473 2061 6666 6f72 6461 626c  of its affordabl
-00000430: 6520 7072 6963 6520 616e 6420 6974 2077  e price and it w
-00000440: 6f72 6b73 206e 6963 656c 7921 0d0a 0d0a  orks nicely!....
-00000450: 2020 2020 2d20 5374 616e 666f 7264 2052      - Stanford R
-00000460: 6573 6561 7263 6820 5379 7374 656d 7320  esearch Systems 
-00000470: 4347 3633 355f 2c20 3220 4748 7a20 436c  CG635_, 2 GHz Cl
-00000480: 6f63 6b20 4765 6e65 7261 746f 720d 0a20  ock Generator.. 
-00000490: 2020 2020 2028 4469 7363 6c61 696d 6572       (Disclaimer
-000004a0: 3a20 4920 776f 726b 2066 6f72 2074 6865  : I work for the
-000004b0: 2063 6f6d 7061 6e79 292e 0d0a 0d0a 4920   company).....I 
-000004c0: 6275 696c 7420 6120 7072 6f6a 6563 7420  built a project 
-000004d0: 7468 6174 2063 6f6e 7472 6f6c 7320 626f  that controls bo
-000004e0: 7468 2069 6e73 7472 756d 656e 7473 2061  th instruments a
-000004f0: 6e64 0d0a 6361 7074 7572 6520 6f75 7470  nd..capture outp
-00000500: 7574 2077 6176 6566 6f72 6d20 6672 6f6d  ut waveform from
-00000510: 2074 6865 2063 6c6f 636b 2067 656e 6572   the clock gener
-00000520: 6174 6f72 2077 6974 6820 7468 6520 6f73  ator with the os
-00000530: 6369 6c6c 6f73 636f 7065 2c0d 0a72 756e  cilloscope,..run
-00000540: 2046 4654 2061 6e64 2064 6973 706c 6179   FFT and display
-00000550: 2074 6865 2077 6176 6566 6f72 6d73 2069   the waveforms i
-00000560: 6e20 6060 7372 7367 7569 6060 2061 7070  n ``srsgui`` app
-00000570: 6c69 6361 7469 6f6e 2e0d 0a0d 0a41 6e79  lication.....Any
-00000580: 206f 7363 696c 6c6f 7363 6f70 6520 616e   oscilloscope an
-00000590: 6420 6675 6e63 7469 6f6e 2067 656e 6572  d function gener
-000005a0: 6174 6f72 2077 696c 6c20 776f 726b 2066  ator will work f
-000005b0: 6f72 2074 6869 7320 6578 616d 706c 652e  or this example.
-000005c0: 0d0a 4966 2079 6f75 2067 6f74 2069 6e74  ..If you got int
-000005d0: 6572 6573 7465 6420 696e 2060 6073 7273  erested in ``srs
-000005e0: 6775 6960 602c 2049 2062 6574 2079 6f75  gui``, I bet you
-000005f0: 2063 616e 2066 696e 6420 616e 206f 7363   can find an osc
-00000600: 696c 6c6f 7363 6f70 650d 0a61 6e64 2061  illoscope..and a
-00000610: 2066 756e 6374 696f 6e20 6765 6e65 7261   function genera
-00000620: 746f 7220 736f 6d65 7768 6572 6520 696e  tor somewhere in
-00000630: 2079 6f75 7220 6275 696c 6469 6e67 2e0d   your building..
-00000640: 0a0d 0a49 6620 796f 7520 636f 756c 6420  ...If you could 
-00000650: 6e6f 742c 2064 6f6e 2774 2077 6f72 7279  not, don't worry
-00000660: 2e20 4576 656e 2077 6974 686f 7574 2061  . Even without a
-00000670: 6e20 616e 7920 696e 7374 7275 6d65 6e74  n any instrument
-00000680: 732c 2077 6520 6361 6e20 6765 6e65 7261  s, we can genera
-00000690: 7465 0d0a 7369 6d75 6c61 7465 6420 7761  te..simulated wa
-000006a0: 7665 666f 726d 2074 6f20 6465 6d6f 6e73  veform to demons
-000006b0: 7472 6174 6520 7468 6520 7573 6162 696c  trate the usabil
-000006c0: 6974 7920 6f66 2060 6073 7273 6775 6960  ity of ``srsgui`
-000006d0: 6020 6173 2061 6e20 6f72 6761 6e69 7a65  ` as an organize
-000006e0: 7220 666f 720d 0a50 7974 686f 6e20 7363  r for..Python sc
-000006f0: 7269 7074 7320 616e 6420 4755 4920 656e  ripts and GUI en
-00000700: 7669 726f 6e6d 656e 7420 666f 7220 636f  vironment for co
-00000710: 6e76 656e 6965 6e74 2064 6174 6120 6163  nvenient data ac
-00000720: 7175 6973 6974 696f 6e20 616e 6420 6461  quisition and da
-00000730: 7461 2076 6973 7561 6c69 7a61 7469 6f6e  ta visualization
-00000740: 2e0d 0a0d 0a0d 0a44 6972 6563 746f 7279  .......Directory
-00000750: 2073 7472 7563 7475 7265 0d0a 2d2d 2d2d   structure..----
-00000760: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000770: 2d0d 0a0d 0a4c 6574 2773 206c 6f6f 6b20  -....Let's look 
-00000780: 6174 2074 6865 2064 6972 6563 746f 7279  at the directory
-00000790: 2073 7472 7563 7475 7265 206f 6620 7468   structure of th
-000007a0: 6520 7072 6f6a 6563 742e 0d0a 0d0a 2e2e  e project.......
-000007b0: 2063 6f64 652d 626c 6f63 6b3a 3a0d 0a0d   code-block::...
-000007c0: 0a20 2020 202f 4f73 6369 6c6c 6f73 636f  .    /Oscillosco
-000007d0: 7065 2065 7861 6d70 6c65 2070 726f 6a65  pe example proje
-000007e0: 6374 2064 6972 6563 746f 7279 0d0a 2020  ct directory..  
-000007f0: 2020 2020 2020 2f69 6e73 7472 756d 656e        /instrumen
-00000800: 7473 0d0a 2020 2020 2020 2020 2020 2020  ts..            
-00000810: 6367 3633 352e 7079 0d0a 2020 2020 2020  cg635.py..      
-00000820: 2020 2020 2020 7364 7331 3230 322e 7079        sds1202.py
-00000830: 0d0a 2020 2020 2020 2020 2f74 6173 6b73  ..        /tasks
-00000840: 0d0a 2020 2020 2020 2020 2020 2020 6669  ..            fi
-00000850: 7273 742e 7079 0d0a 2020 2020 2020 2020  rst.py..        
-00000860: 2020 2020 7365 636f 6e64 2e70 790d 0a20      second.py.. 
-00000870: 2020 2020 2020 2020 2020 202e 2e2e 0d0a             .....
-00000880: 0d0a 2020 2020 2020 2020 6f73 6369 6c6c  ..        oscill
-00000890: 6f73 636f 7065 2065 7861 6d70 6c65 2070  oscope example p
-000008a0: 726f 6a65 6374 2e74 6173 6b63 6f6e 6669  roject.taskconfi
-000008b0: 670d 0a0d 0a54 6869 7320 6669 6c65 2073  g....This file s
-000008c0: 7472 7563 7475 7265 2066 6f6c 6c6f 7773  tructure follows
-000008d0: 2074 6865 2067 7569 6465 6c69 6e65 2064   the guideline d
-000008e0: 6573 6372 6962 6564 2069 6e0d 0a3a 7265  escribed in..:re
-000008f0: 663a 6043 7265 6174 696e 6720 6669 6c65  f:`Creating file
-00000900: 2073 7472 7563 7475 7265 2066 6f72 2061   structure for a
-00000910: 2070 726f 6a65 6374 602e 0d0a 5765 2068   project`...We h
-00000920: 6176 6520 7477 6f20 696e 7374 7275 6d65  ave two instrume
-00000930: 6e74 2064 7269 7665 7220 7363 7269 7074  nt driver script
-00000940: 7320 666f 7220 5344 5331 3230 3258 455f  s for SDS1202XE_
-00000950: 2061 6e64 2043 4736 3335 5f0d 0a69 6e20   and CG635_..in 
-00000960: 7468 6520 7375 6264 6972 6563 746f 7279  the subdirectory
-00000970: 2063 616c 6c65 6420 2a2a 696e 7374 7275   called **instru
-00000980: 6d65 6e74 732a 2a2c 2066 6976 6520 7461  ments**, five ta
-00000990: 736b 2073 6372 6970 7473 0d0a 696e 2074  sk scripts..in t
-000009a0: 6865 2073 7562 6469 7265 6374 6f72 7920  he subdirectory 
-000009b0: 6361 6c6c 6564 202a 2a74 6173 6b73 2a2a  called **tasks**
-000009c0: 2061 6c6f 6e67 2077 6974 6820 6120 636f   along with a co
-000009d0: 6e66 6967 7572 6174 696f 6e20 6669 6c65  nfiguration file
-000009e0: 0d0a 696e 2074 6865 2070 726f 6a65 6374  ..in the project
-000009f0: 2072 6f6f 7420 6469 7265 6374 6f72 792e   root directory.
-00000a00: 0d0a 0d0a 5072 6f6a 6563 7420 636f 6e66  ....Project conf
-00000a10: 6967 7572 6174 696f 6e20 6669 6c65 0d0a  iguration file..
-00000a20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000a30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a0d  -------------...
-00000a40: 0a54 6865 2073 7472 7563 7475 7265 206f  .The structure o
-00000a50: 6620 6120 2e74 6173 6b63 6f6e 6669 6720  f a .taskconfig 
-00000a60: 6669 6c65 2069 7320 7369 6d70 6c65 2061  file is simple a
-00000a70: 6e64 0d0a 6578 706c 6169 6e65 6420 696e  nd..explained in
-00000a80: 203a 7265 663a 6050 6f70 756c 6174 696e   :ref:`Populatin
-00000a90: 6720 7468 6520 2e74 6173 6b63 6f6e 6669  g the .taskconfi
-00000aa0: 6720 6669 6c65 600d 0a0d 0a2e 2e20 636f  g file`...... co
-00000ab0: 6465 2d62 6c6f 636b 3a3a 0d0a 2020 2020  de-block::..    
-00000ac0: 3a6c 696e 656e 6f73 3a0d 0a0d 0a20 2020  :linenos:....   
-00000ad0: 206e 616d 653a 2053 7273 6775 6920 6578   name: Srsgui ex
-00000ae0: 616d 706c 6520 7072 6f6a 6563 7420 7573  ample project us
-00000af0: 696e 6720 616e 206f 7363 696c 6c6f 7363  ing an oscillosc
-00000b00: 6f70 6520 616e 6420 6120 636c 6f63 6b20  ope and a clock 
-00000b10: 6765 6e65 7261 746f 720d 0a0d 0a20 2020  generator....   
-00000b20: 2069 6e73 743a 2063 672c 2020 696e 7374   inst: cg,  inst
-00000b30: 7275 6d65 6e74 732e 6367 3633 352c 2020  ruments.cg635,  
-00000b40: 2043 4736 3335 0d0a 2020 2020 696e 7374   CG635..    inst
-00000b50: 3a20 6f73 632c 2069 6e73 7472 756d 656e  : osc, instrumen
-00000b60: 7473 2e73 6473 3132 3032 2c20 5344 5331  ts.sds1202, SDS1
-00000b70: 3230 320d 0a0d 0a20 2020 2074 6173 6b3a  202....    task:
-00000b80: 202a 4944 4e20 7465 7374 2c20 2020 2020   *IDN test,     
-00000b90: 2020 2020 2020 2020 2020 2020 7461 736b              task
-00000ba0: 732e 6669 7273 742c 2020 4669 7273 7454  s.first,  FirstT
-00000bb0: 6173 6b0d 0a20 2020 2074 6173 6b3a 2050  ask..    task: P
-00000bc0: 6c6f 7420 6578 616d 706c 652c 2020 2020  lot example,    
-00000bd0: 2020 2020 2020 2020 2020 7461 736b 732e            tasks.
-00000be0: 7365 636f 6e64 2c20 5365 636f 6e64 5461  second, SecondTa
-00000bf0: 736b 0d0a 2020 2020 2e2e 2e0d 0a0d 0a49  sk..    .......I
-00000c00: 6e73 7472 756d 656e 7420 6472 6976 6572  nstrument driver
-00000c10: 730d 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  s..-------------
-00000c20: 2d2d 2d2d 2d2d 2d0d 0a0d 0a43 4736 3335  -------....CG635
-00000c30: 0d0a 2d2d 2d2d 2d2d 2d0d 0a0d 0a4c 6574  ..-------....Let
-00000c40: 2773 2074 616b 6520 6120 6c6f 6f6b 2069  's take a look i
-00000c50: 6e74 6f20 7468 6520 696e 7374 7275 6d65  nto the instrume
-00000c60: 6e74 2f63 6736 3335 2e70 7920 6d6f 6475  nt/cg635.py modu
-00000c70: 6c65 2e20 4576 656e 2074 686f 7567 6820  le. Even though 
-00000c80: 6974 2073 6565 6d73 206c 6f6e 672c 0d0a  it seems long,..
-00000c90: 6974 2068 6173 206f 6e6c 7920 3520 6c69  it has only 5 li
-00000ca0: 6e65 2069 6620 7468 6520 636f 6d6d 656e  ne if the commen
-00000cb0: 7420 6c69 6e65 7320 7265 6d6f 7665 642e  t lines removed.
-00000cc0: 2049 6620 796f 7520 6861 7665 2061 2043   If you have a C
-00000cd0: 4736 3335 2c0d 0a63 6f6e 6772 6174 756c  G635,..congratul
-00000ce0: 6174 696f 6e73 2120 596f 7520 6361 6e20  ations! You can 
-00000cf0: 7573 6520 7468 6520 6669 6c65 2061 7320  use the file as 
-00000d00: 6973 2e20 4966 2079 6f75 2068 6176 6520  is. If you have 
-00000d10: 616e 7920 6675 6e63 7469 6f6e 0d0a 6765  any function..ge
-00000d20: 6e65 7261 746f 7220 7468 6174 2063 616e  nerator that can
-00000d30: 2063 6861 6e67 6520 7468 6520 6f75 7470   change the outp
-00000d40: 7574 2066 7265 7175 656e 6379 2c20 796f  ut frequency, yo
-00000d50: 7520 6361 6e20 7573 6520 6974 2069 6e73  u can use it ins
-00000d60: 7465 6164 206f 6620 4347 3633 350d 0a69  tead of CG635..i
-00000d70: 6e20 7468 6520 6578 616d 706c 652e 2059  n the example. Y
-00000d80: 6f75 2063 6861 6e67 6520 7468 6520 636c  ou change the cl
-00000d90: 6173 7320 6e61 6d65 2061 6e64 205f 4964  ass name and _Id
-00000da0: 5374 7269 6e67 2074 6f20 6d61 7463 6820  String to match 
-00000db0: 7468 6520 696e 7374 7275 6d65 6e74 206e  the instrument n
-00000dc0: 616d 652c 0d0a 616c 6f6e 6720 7769 7468  ame,..along with
-00000dd0: 205f 7465 726d 5f63 6861 722c 2061 6e64   _term_char, and
-00000de0: 2066 696e 6420 6f75 7420 7468 6520 636f   find out the co
-00000df0: 6d6d 616e 6420 746f 2063 6861 6e67 6520  mmand to change 
-00000e00: 6672 6571 7565 6e63 792c 2072 6566 6572  frequency, refer
-00000e10: 7269 6e67 2074 6f20 7468 6520 6d61 6e75  ring to the manu
-00000e20: 616c 2e0d 0a41 6e64 2073 6176 6520 6974  al...And save it
-00000e30: 2074 6f20 6120 6469 6666 6572 656e 7420   to a different 
-00000e40: 6e61 6d65 2e20 4368 616e 6765 2074 6865  name. Change the
-00000e50: 2069 6e73 743a 206c 696e 6520 666f 7220   inst: line for 
-00000e60: 2763 6727 0d0a 696e 2074 6865 202e 7461  'cg'..in the .ta
-00000e70: 736b 636f 6e66 6967 2066 696c 6520 746f  skconfig file to
-00000e80: 206d 6174 6368 2074 6865 206d 6f64 756c   match the modul
-00000e90: 6520 7061 7468 2061 6e64 2074 6865 2063  e path and the c
-00000ea0: 6c61 7373 206e 616d 652e 0d0a 0d0a 2e2e  lass name.......
-00000eb0: 2063 6f64 652d 626c 6f63 6b3a 3a0d 0a20   code-block::.. 
-00000ec0: 2020 203a 6c69 6e65 6e6f 733a 0d0a 0d0a     :linenos:....
-00000ed0: 2020 2020 6672 6f6d 2073 7273 6775 6920      from srsgui 
-00000ee0: 696d 706f 7274 2049 6e73 7472 756d 656e  import Instrumen
-00000ef0: 740d 0a20 2020 2066 726f 6d20 7372 7367  t..    from srsg
-00000f00: 7569 2e69 6e73 7420 696d 706f 7274 2046  ui.inst import F
-00000f10: 6c6f 6174 436f 6d6d 616e 640d 0a0d 0a20  loatCommand.... 
-00000f20: 2020 2063 6c61 7373 2043 4736 3335 2849     class CG635(I
-00000f30: 6e73 7472 756d 656e 7429 3a0d 0a20 2020  nstrument):..   
-00000f40: 2020 2020 205f 4964 5374 7269 6e67 203d       _IdString =
-00000f50: 2027 4347 3633 3527 0d0a 2020 2020 2020   'CG635'..      
-00000f60: 2020 6672 6571 7565 6e63 7920 3d20 466c    frequency = Fl
-00000f70: 6f61 7443 6f6d 6d61 6e64 2827 4652 4551  oatCommand('FREQ
-00000f80: 2729 0d0a 0d0a 5769 7468 6f75 7420 7265  ')....Without re
-00000f90: 6465 6669 6e69 6e67 202a 2a61 7661 696c  defining **avail
-00000fa0: 6162 5f69 6e74 6572 6661 6365 732a 2a20  ab_interfaces** 
-00000fb0: 636c 6173 7320 6174 7472 6962 7574 652c  class attribute,
-00000fc0: 2079 6f75 2063 616e 2075 7365 2074 6865   you can use the
-00000fd0: 2073 6572 6961 6c0d 0a63 6f6d 6d75 6e69   serial..communi
-00000fe0: 6361 7469 6f6e 206f 6e6c 792e 2049 6620  cation only. If 
-00000ff0: 796f 7520 7761 6e74 2074 6f20 7573 6520  you want to use 
-00001000: 4750 4942 2063 6f6d 6d75 6e69 6361 7469  GPIB communicati
-00001010: 6f6e 2c20 796f 7520 6861 7665 2074 6f20  on, you have to 
-00001020: 756e 636f 6d6d 656e 7420 7468 650d 0a2a  uncomment the..*
-00001030: 2a61 7661 696c 6162 6c65 5f69 6e74 6572  *available_inter
-00001040: 6661 6365 732a 2a20 696e 2043 4736 3335  faces** in CG635
-00001050: 2063 6c61 7373 2e0d 0a0d 0a2e 2e20 636f   class....... co
-00001060: 6465 2d62 6c6f 636b 3a3a 0d0a 0d0a 2020  de-block::....  
-00001070: 2020 6672 6f6d 2073 7273 6775 6920 696d    from srsgui im
-00001080: 706f 7274 2053 6572 6961 6c49 6e74 6572  port SerialInter
-00001090: 6661 6365 2c20 4669 6e64 4c69 7374 496e  face, FindListIn
-000010a0: 7075 740d 0a20 2020 2066 726f 6d20 7372  put..    from sr
-000010b0: 7369 6e73 742e 7372 3836 3020 696d 706f  sinst.sr860 impo
-000010c0: 7274 2056 6973 6149 6e74 6572 6661 6365  rt VisaInterface
-000010d0: 0d0a 0d0a 2020 2020 6176 6169 6c61 626c  ....    availabl
-000010e0: 655f 696e 7465 7266 6163 6573 203d 205b  e_interfaces = [
-000010f0: 0d0a 2020 2020 2020 2020 5b20 2020 5365  ..        [   Se
-00001100: 7269 616c 496e 7465 7266 6163 652c 0d0a  rialInterface,..
-00001110: 2020 2020 2020 2020 2020 2020 7b0d 0a20              {.. 
-00001120: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00001130: 434f 4d20 706f 7274 273a 2046 696e 644c  COM port': FindL
-00001140: 6973 7449 6e70 7574 2829 2c0d 0a20 2020  istInput(),..   
-00001150: 2020 2020 2020 2020 2020 2020 2027 6261               'ba
-00001160: 7564 2072 6174 6527 3a20 3936 3030 0d0a  ud rate': 9600..
-00001170: 2020 2020 2020 2020 2020 2020 7d0d 0a20              }.. 
-00001180: 2020 2020 2020 205d 2c0d 0a20 2020 2020         ],..     
-00001190: 2020 205b 2020 2056 6973 6149 6e74 6572     [   VisaInter
-000011a0: 6661 6365 2c0d 0a20 2020 2020 2020 2020  face,..         
-000011b0: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
-000011c0: 2020 2020 2020 2772 6573 6f75 7263 6527        'resource'
-000011d0: 3a20 4669 6e64 4c69 7374 496e 7075 7428  : FindListInput(
-000011e0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-000011f0: 7d0d 0a20 2020 2020 2020 205d 2c0d 0a20  }..        ],.. 
-00001200: 2020 205d 0d0a 0d0a 796f 7520 6861 7665     ]....you have
-00001210: 2074 6f20 696e 7374 616c 6c20 6073 7273   to install `srs
-00001220: 696e 7374 2e73 7238 3630 605f 2066 6f72  inst.sr860`_ for
-00001230: 2056 6973 6149 6e74 6572 6661 6365 2063   VisaInterface c
-00001240: 6c61 7373 2c20 616e 6420 5079 5649 5341  lass, and PyVISA
-00001250: 5f20 616e 640d 0a69 7473 2062 6163 6b65  _ and..its backe
-00001260: 6e64 206c 6962 7261 7279 2c20 666f 6c6c  nd library, foll
-00001270: 6f77 696e 6720 5079 5669 7361 2069 6e73  owing PyVisa ins
-00001280: 7461 6c6c 6174 696f 6e20 696e 7374 7275  tallation instru
-00001290: 6374 696f 6e2e 0d0a 0d0a 4f6e 6365 2043  ction.....Once C
-000012a0: 4736 3335 2069 7320 636f 6e6e 6563 7465  G635 is connecte
-000012b0: 642c 2079 6f75 2077 696c 6c20 7365 6520  d, you will see 
-000012c0: 7468 6520 636f 6e6e 6563 7469 6f6e 2069  the connection i
-000012d0: 6e66 6f72 6d61 7469 6f6e 2069 6e20 7468  nformation in th
-000012e0: 6520 696e 7374 7275 6d65 6e74 2069 6e66  e instrument inf
-000012f0: 6f20 7061 6e65 6c2c 0d0a 616e 6420 796f  o panel,..and yo
-00001300: 7520 6361 6e20 7573 6520 6974 2069 6e20  u can use it in 
-00001310: 7468 6520 7465 726d 696e 616c 2c20 6173  the terminal, as
-00001320: 2073 686f 776e 2062 656c 6f77 2e0d 0a0d   shown below....
-00001330: 0a2e 2e20 6669 6775 7265 3a3a 202e 2f5f  ... figure:: ./_
-00001340: 7374 6174 6963 2f63 672d 7465 726d 696e  static/cg-termin
-00001350: 616c 2d73 6372 6565 6e2d 6361 7074 7572  al-screen-captur
-00001360: 652e 706e 670d 0a20 2020 203a 616c 6967  e.png..    :alig
-00001370: 6e3a 2063 656e 7465 720d 0a20 2020 203a  n: center..    :
-00001380: 6669 6763 6c61 7373 3a20 616c 6967 6e2d  figclass: align-
-00001390: 6365 6e74 6572 0d0a 0d0a 7c0d 0a0d 0a54  center....|....T
-000013a0: 6f20 6669 7820 7468 6520 274e 6f74 2069  o fix the 'Not i
-000013b0: 6d70 6c65 6d65 6e74 6564 2720 7761 726e  mplemented' warn
-000013c0: 696e 672c 0d0a 3a6d 6574 683a 6049 6e73  ing,..:meth:`Ins
-000013d0: 7472 756d 656e 742e 6765 745f 7374 6174  trument.get_stat
-000013e0: 7573 2829 203c 7372 7367 7569 2e69 6e73  us() <srsgui.ins
-000013f0: 742e 696e 7374 7275 6d65 6e74 2e49 6e73  t.instrument.Ins
-00001400: 7472 756d 656e 742e 6765 745f 7374 6174  trument.get_stat
-00001410: 7573 3e60 0d0a 6e65 6564 2074 6f20 6265  us>`..need to be
-00001420: 2072 6564 6566 696e 6564 2e20 546f 2066   redefined. To f
-00001430: 6565 6c20 6265 7474 6572 2c20 7765 2063  eel better, we c
-00001440: 616e 206f 7665 7272 6964 6520 6974 2020  an override it  
-00001450: 6173 2061 2043 4736 3335 206d 6574 686f  as a CG635 metho
-00001460: 6420 6173 2066 6f6c 6c6f 7769 6e67 3a0d  d as following:.
-00001470: 0a0d 0a2e 2e20 636f 6465 2d62 6c6f 636b  ..... code-block
-00001480: 3a3a 0d0a 0d0a 2020 2020 6465 6620 6765  ::....    def ge
-00001490: 745f 7374 6174 7573 2873 656c 6629 3a0d  t_status(self):.
-000014a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000014b0: 2753 7461 7475 733a 204f 4b27 0d0a 0d0a  'Status: OK'....
-000014c0: 5765 2077 696c 6c20 7573 6520 6f6e 6c79  We will use only
-000014d0: 206f 6e65 2063 6f6d 6d61 6e64 205c 2e66   one command \.f
-000014e0: 7265 7175 656e 6379 2c20 6f72 2069 7473  requency, or its
-000014f0: 2072 6177 2072 656d 6f74 6520 636f 6d6d   raw remote comm
-00001500: 616e 642c 2027 6672 6571 2720 696e 2074  and, 'freq' in t
-00001510: 6869 7320 6578 616d 706c 652e 0d0a 4265  his example...Be
-00001520: 6361 7573 6520 2763 6727 2069 7320 7468  cause 'cg' is th
-00001530: 6520 6465 6661 756c 7420 696e 7374 7275  e default instru
-00001540: 6d65 6e74 2c20 7468 6520 6669 7273 7420  ment, the first 
-00001550: 696e 7374 7275 6d65 6e74 206d 656e 7469  instrument menti
-00001560: 6f6e 6564 2069 6e20 7468 6520 2e74 6173  oned in the .tas
-00001570: 6b63 6f6e 6669 6720 6669 6c65 2c0d 0a79  kconfig file,..y
-00001580: 6f75 2063 616e 2073 656e 6420 616e 7920  ou can send any 
-00001590: 7261 7720 7265 6d6f 7465 2063 6f6d 6d61  raw remote comma
-000015a0: 6e64 2077 6974 686f 7574 2027 6367 3a27  nd without 'cg:'
-000015b0: 2070 7265 6669 7820 6966 2079 6f75 2077   prefix if you w
-000015c0: 616e 7420 746f 2e0d 0a42 6f74 6820 275c  ant to...Both '\
-000015d0: 2a69 646e 3f27 2061 6e64 2027 6367 3a5c  *idn?' and 'cg:\
-000015e0: 2a69 646e 3f27 2077 696c 6c20 7265 7475  *idn?' will retu
-000015f0: 726e 2074 6865 2063 6f72 7265 6374 2072  rn the correct r
-00001600: 6570 6c79 2e0d 0a0d 0a57 6520 7573 6520  eply.....We use 
-00001610: 7468 6520 7072 6566 6978 2027 6367 3a27  the prefix 'cg:'
-00001620: 2066 6f72 2072 6177 2072 656d 6f74 6520   for raw remote 
-00001630: 636f 6d6d 616e 6420 616e 6420 7468 6520  command and the 
-00001640: 7072 6566 6978 2027 6367 2e27 2066 6f72  prefix 'cg.' for
-00001650: 2050 7974 686f 6e20 636f 6d6d 616e 6473   Python commands
-00001660: 2e0d 0a49 6e20 7468 6520 7465 726d 696e  ...In the termin
-00001670: 616c 2061 6c6c 2061 7474 7269 6275 7465  al all attribute
-00001680: 2061 6e64 206d 6574 686f 6420 6f66 2043   and method of C
-00001690: 4738 3335 2063 616c 7373 2063 616e 2062  G835 calss can b
-000016a0: 6520 7573 6564 2077 6974 6820 7072 6566  e used with pref
-000016b0: 6978 2027 6367 2e27 2e0d 0a42 6563 6175  ix 'cg.'...Becau
-000016c0: 7365 2077 6520 6465 6669 6e65 6420 6672  se we defined fr
-000016d0: 6571 7565 6e63 7920 6173 2061 2046 6c6f  equency as a Flo
-000016e0: 6174 436f 6d6d 616e 642c 2077 6520 6361  atCommand, we ca
-000016f0: 6e20 7573 6520 2763 672e 6672 6571 7565  n use 'cg.freque
-00001700: 6e63 7927 2070 726f 7065 7274 7920 696e  ncy' property in
-00001710: 2074 6865 0d0a 7465 726d 696e 616c 2061   the..terminal a
-00001720: 6e64 2061 6e79 2070 7974 686f 6e20 7363  nd any python sc
-00001730: 7269 7074 732c 206f 6e63 6520 6765 745f  ripts, once get_
-00001740: 696e 7374 7275 6d65 6e74 2827 6367 2729  instrument('cg')
-00001750: 2069 6e20 6120 7461 736b 2063 6c61 7373   in a task class
-00001760: 2e0d 0a42 6563 6175 7365 2071 7572 6579  ...Because qurey
-00001770: 5f66 6c6f 6174 2829 2069 7320 7468 6520  _float() is the 
-00001780: 666c 6f61 7420 7175 6572 7920 636f 6d6d  float query comm
-00001790: 616e 6420 6465 6669 6e65 6420 696e 2074  and defined in t
-000017a0: 6865 2049 6e73 7472 756d 656e 7420 636c  he Instrument cl
-000017b0: 6173 732c 0d0a 796f 7520 6361 6e20 7573  ass,..you can us
-000017c0: 6520 6974 2069 6e20 7468 6520 7465 726d  e it in the term
-000017d0: 696e 616c 2e0d 0a0d 0a41 6374 7561 6c6c  inal.....Actuall
-000017e0: 7920 796f 7520 6361 6e20 7573 6520 616c  y you can use al
-000017f0: 6c20 7468 6520 6174 7472 6962 7574 6520  l the attribute 
-00001800: 616e 6420 6d65 7468 6f64 2064 6566 696e  and method defin
-00001810: 6564 2069 6e20 4347 3633 3520 636c 6173  ed in CG635 clas
-00001820: 7320 616e 6420 6974 7320 7375 7065 7220  s and its super 
-00001830: 636c 6173 7365 732e 0d0a 5468 6572 6520  classes...There 
-00001840: 6973 2063 672e 6469 7228 2920 6d65 7468  is cg.dir() meth
-00001850: 6f64 2064 6566 696e 6564 2069 6e20 436f  od defined in Co
-00001860: 6d70 6f6e 656e 7420 636c 6173 732e 2049  mponent class. I
-00001870: 7420 7368 6f77 7320 616c 6c20 7468 6520  t shows all the 
-00001880: 6176 6169 6c61 626c 650d 0a63 6f6d 706f  available..compo
-00001890: 6e65 6e74 732c 2063 6f6d 6d61 6e64 732c  nents, commands,
-000018a0: 2061 6e64 206d 6574 686f 642e 2049 7420   and method. It 
-000018b0: 6865 6c70 7320 7573 2074 6f20 6e61 7669  helps us to navi
-000018c0: 6761 7465 2074 6872 6f75 6768 2072 6573  gate through res
-000018d0: 6f75 7263 6573 0d0a 6176 6169 6c61 626c  ources..availabl
-000018e0: 6520 7769 7468 2074 6865 2063 6c61 7373  e with the class
-000018f0: 2e0d 0a0d 0a2e 2e20 6669 6775 7265 3a3a  ....... figure::
-00001900: 202e 2f5f 7374 6174 6963 2f63 672d 6469   ./_static/cg-di
-00001910: 722d 7465 726d 696e 616c 2d73 6372 6565  r-terminal-scree
-00001920: 6e2d 6361 7074 7572 652e 706e 670d 0a20  n-capture.png.. 
-00001930: 2020 203a 616c 6967 6e3a 2063 656e 7465     :align: cente
-00001940: 720d 0a20 2020 203a 6669 6763 6c61 7373  r..    :figclass
-00001950: 3a20 616c 6967 6e2d 6365 6e74 6572 0d0a  : align-center..
-00001960: 0d0a 7c0d 0a0d 0a46 726f 6d20 7468 6520  ..|....From the 
-00001970: 7465 726d 696e 616c 2c20 796f 7520 6361  terminal, you ca
-00001980: 6e20 636f 6e74 726f 6c20 616c 6c20 7468  n control all th
-00001990: 6520 696e 7374 7275 6d65 6e74 732c 2061  e instruments, a
-000019a0: 7320 6d75 6368 2061 7320 796f 7520 6361  s much as you ca
-000019b0: 6e20 646f 2077 6974 6820 7461 736b 2073  n do with task s
-000019c0: 6372 6970 7473 2e0d 0a44 6566 696e 696e  cripts...Definin
-000019d0: 6720 6d61 6e79 2075 7365 6675 6c20 6d65  g many useful me
-000019e0: 7468 6f64 7320 696e 2061 6e20 696e 7374  thods in an inst
-000019f0: 7275 6d65 6e74 2063 6c61 7373 2070 726f  rument class pro
-00001a00: 7669 6465 7320 6d6f 7265 2063 6f6e 7472  vides more contr
-00001a10: 6f6c 7320 6672 6f6d 2074 6865 2074 6572  ols from the ter
-00001a20: 6d69 6e61 6c2c 0d0a 7768 696c 6520 796f  minal,..while yo
-00001a30: 7520 6172 6520 7477 6561 6b69 6e67 2074  u are tweaking t
-00001a40: 6f20 6669 6e64 206f 7074 696d 616c 206f  o find optimal o
-00001a50: 7065 7261 7469 6f6e 2070 6172 616d 6574  peration paramet
-00001a60: 6572 7320 6f66 2069 6e73 7472 756d 656e  ers of instrumen
-00001a70: 7473 2e0d 0a0d 0a53 4453 3132 3032 0d0a  ts.....SDS1202..
-00001a80: 2d2d 2d2d 2d2d 2d2d 0d0a 0d0a 4576 656e  --------....Even
-00001a90: 2074 686f 7567 6820 796f 7520 6d61 7920   though you may 
-00001aa0: 6e6f 7420 6861 7665 2061 6e20 5344 5331  not have an SDS1
-00001ab0: 3230 3220 6f73 6369 6c6c 6f73 636f 7065  202 oscilloscope
-00001ac0: 2074 6861 7420 4920 6861 7070 656e 6564   that I happened
-00001ad0: 0d0a 746f 2075 7365 2066 6f72 2074 6869  ..to use for thi
-00001ae0: 7320 6578 616d 706c 652c 2049 2062 6574  s example, I bet
-00001af0: 2079 6f75 2063 616e 2066 696e 6420 616e   you can find an
-00001b00: 206f 7363 696c 6c6f 7363 6f70 6520 736f   oscilloscope so
-00001b10: 6d65 7768 6572 650d 0a69 6e20 796f 7572  mewhere..in your
-00001b20: 2062 7569 6c64 696e 672e 2057 6865 6e20   building. When 
-00001b30: 796f 7520 6765 7420 6120 686f 6c64 206f  you get a hold o
-00001b40: 6620 6f6e 652c 2069 7420 6d61 7920 6861  f one, it may ha
-00001b50: 7665 2061 2055 5342 2063 6f6e 6e65 6374  ve a USB connect
-00001b60: 6f72 206f 6e6c 792c 0d0a 6c69 6b65 2061  or only,..like a
-00001b70: 206c 6f74 206f 6620 6261 7365 206d 6f64   lot of base mod
-00001b80: 656c 206f 7363 696c 6c6f 7363 6f70 6573  el oscilloscopes
-00001b90: 2064 6f2e 0d0a 4974 206d 6561 6e73 2079   do...It means y
-00001ba0: 6f75 2068 6176 6520 746f 2075 7365 2055  ou have to use U
-00001bb0: 5342 2d54 4d43 2069 6e74 6572 6661 6365  SB-TMC interface
-00001bc0: 2e20 496e 206f 7264 6572 2074 6f20 646f  . In order to do
-00001bd0: 2074 6861 742c 2079 6f75 206e 6565 6420   that, you need 
-00001be0: 746f 0d0a 696e 7374 616c 6c20 5079 5649  to..install PyVI
-00001bf0: 5341 2061 6d64 206d 616b 6520 6974 2077  SA amd make it w
-00001c00: 6f72 6b2e 2059 6f75 206e 6565 6420 746f  ork. You need to
-00001c10: 2075 6e63 6f6d 6d65 6e74 2074 6865 2061   uncomment the a
-00001c20: 7661 696c 6162 6c65 5f69 6e74 6572 6661  vailable_interfa
-00001c30: 6365 7320 6f66 0d0a 5344 5331 3230 3220  ces of..SDS1202 
-00001c40: 636c 6173 732c 206d 6f64 6966 7920 6974  class, modify it
-00001c50: 2074 6f20 6669 7420 7468 6520 7370 6563   to fit the spec
-00001c60: 6966 6963 6174 696f 6e20 6f66 2079 6f75  ification of you
-00001c70: 7220 6f73 6369 6c6c 6f73 636f 7065 2c20  r oscilloscope, 
-00001c80: 616c 6f6e 6720 7769 7468 0d0a 6368 616e  along with..chan
-00001c90: 6769 6e67 2074 6f20 7468 6520 636f 7272  ging to the corr
-00001ca0: 6563 7420 5f49 6453 7472 696e 672e 2041  ect _IdString. A
-00001cb0: 6e64 2079 6f75 2068 6176 6520 746f 2067  nd you have to g
-00001cc0: 6574 2077 6176 6566 6f72 6d20 646f 776e  et waveform down
-00001cd0: 6c6f 6164 2077 6f72 6b69 6e67 2e0d 0a49  load working...I
-00001ce0: 6620 796f 7520 6172 6520 6c75 636b 792c  f you are lucky,
-00001cf0: 2079 6f75 2063 616e 2066 696e 6420 6120   you can find a 
-00001d00: 776f 726b 696e 6720 5079 7468 6f6e 2073  working Python s
-00001d10: 6e69 7070 6574 2066 726f 6d20 6a75 6469  nippet from judi
-00001d20: 6369 6f75 7320 7765 6220 7365 6172 6368  cious web search
-00001d30: 2e0d 0a49 6620 6e6f 7420 796f 7520 6861  ...If not you ha
-00001d40: 7665 2074 6f20 6465 6369 7068 6572 2074  ve to decipher t
-00001d50: 6865 2070 726f 6772 616d 6d69 6e67 206d  he programming m
-00001d60: 616e 7561 6c20 6f66 2074 6865 206f 7363  anual of the osc
-00001d70: 696c 6c6f 7363 6f70 6520 746f 206d 616b  illoscope to mak
-00001d80: 6520 7468 6520 7761 7665 666f 726d 0d0a  e the waveform..
-00001d90: 646f 776e 6c6f 6164 2077 6f72 6b69 6e67  download working
-00001da0: 2e20 4974 206d 6179 2074 616b 6520 7469  . It may take ti
-00001db0: 6d65 2c20 4974 2077 696c 6c20 6265 2076  me, It will be v
-00001dc0: 6572 7920 7265 7761 7264 696e 6720 666f  ery rewarding fo
-00001dd0: 7220 796f 7572 2064 6174 6120 6163 7175  r your data acqu
-00001de0: 6973 6974 696f 6e0d 0a73 6b69 6c6c 2073  isition..skill s
-00001df0: 6574 2069 6d70 726f 7665 6d65 6e74 2e0d  et improvement..
-00001e00: 0a0d 0a4f 7468 6572 2074 6861 6e20 7468  ...Other than th
-00001e10: 6520 6269 6e61 7279 2077 6176 6566 6f72  e binary wavefor
-00001e20: 6d20 646f 776e 6c6f 6164 2c20 436f 6d6d  m download, Comm
-00001e30: 756e 6963 6174 696f 6e20 7769 7468 2061  unication with a
-00001e40: 6e20 6f73 6369 6c6c 6f73 636f 7065 2077  n oscilloscope w
-00001e50: 696c 6c20 776f 726b 204f 4b0d 0a75 7369  ill work OK..usi
-00001e60: 6e67 2074 6578 7420 6261 7365 6420 636f  ng text based co
-00001e70: 6d6d 756e 6963 6174 696f 6e20 666f 7220  mmunication for 
-00001e80: 6d6f 7374 206f 6620 7265 6d6f 7465 2063  most of remote c
-00001e90: 6f6d 6d61 6e64 732e 0d0a 0d0a 5769 7468  ommands.....With
-00001ea0: 2064 6566 6175 6c74 2061 7661 696c 6162   default availab
-00001eb0: 6c65 5f69 6e74 6572 6661 6365 7320 6f66  le_interfaces of
-00001ec0: 2049 6e73 7472 756d 656e 7420 636c 6173   Instrument clas
-00001ed0: 732c 2054 6370 6970 496e 7465 7266 6163  s, TcpipInterfac
-00001ee0: 6520 7368 6f75 6c64 2062 6520 7573 6564  e should be used
-00001ef0: 2077 6974 6820 706f 7274 2035 3032 352e   with port 5025.
-00001f00: 0d0a 0d0a 5468 6520 696e 7374 7275 6d65  ....The instrume
-00001f10: 6e74 2064 7269 7665 7220 666f 7220 5344  nt driver for SD
-00001f20: 5331 3230 3220 7769 6c6c 2077 6f72 6b20  S1202 will work 
-00001f30: 7769 7468 2034 206c 696e 6573 206f 6620  with 4 lines of 
-00001f40: 636f 6465 2c20 6a75 7374 206c 696b 6520  code, just like 
-00001f50: 4347 3633 352c 0d0a 6265 666f 7265 2061  CG635,..before a
-00001f60: 6464 696e 6720 7468 6520 6d65 7468 6f64  dding the method
-00001f70: 2074 6f20 646f 776e 6c6f 6164 2077 6176   to download wav
-00001f80: 6566 6f72 6d73 2066 726f 6d20 7468 6520  eforms from the 
-00001f90: 6f73 6369 6c6c 6f73 636f 7065 2e20 4164  oscilloscope. Ad
-00001fa0: 6420 6174 7472 6962 7574 6573 2061 6e64  d attributes and
-00001fb0: 206d 6574 686f 6473 0d0a 696e 6372 656d   methods..increm
-00001fc0: 656e 7461 6c6c 7920 6173 2079 6f75 206e  entally as you n
-00001fd0: 6565 6420 746f 2075 7365 206d 6f72 6520  eed to use more 
-00001fe0: 6675 6e63 7469 6f6e 7320 6f66 2074 6865  functions of the
-00001ff0: 2069 6e73 7472 756d 656e 742e 0d0a 0d0a   instrument.....
-00002000: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a0d  .. code-block::.
-00002010: 0a20 2020 203a 6c69 6e65 6e6f 733a 0d0a  .    :linenos:..
-00002020: 0d0a 2020 2020 696d 706f 7274 206e 756d  ..    import num
-00002030: 7079 2061 7320 6e70 0d0a 2020 2020 6672  py as np..    fr
-00002040: 6f6d 2073 7273 6775 6920 696d 706f 7274  om srsgui import
-00002050: 2049 6e73 7472 756d 656e 740d 0a0d 0a20   Instrument.... 
-00002060: 2020 2063 6c61 7373 2053 4453 3132 3032     class SDS1202
-00002070: 2849 6e73 7472 756d 656e 7429 3a0d 0a20  (Instrument):.. 
-00002080: 2020 2020 2020 205f 4964 5374 7269 6e67         _IdString
-00002090: 203d 2027 5344 5331 3230 3227 0d0a 0d0a   = 'SDS1202'....
-000020a0: 2020 2020 2020 2020 6465 6620 6765 745f          def get_
-000020b0: 7761 7665 666f 726d 2873 656c 662c 2063  waveform(self, c
-000020c0: 6861 6e6e 656c 293a 0d0a 2020 2020 2020  hannel):..      
-000020d0: 2020 2020 2020 2e2e 2e0d 0a0d 0a20 2020        .......   
-000020e0: 2020 2020 2064 6566 2067 6574 5f73 616d       def get_sam
-000020f0: 706c 696e 675f 7261 7465 2873 656c 6629  pling_rate(self)
-00002100: 3a0d 0a20 2020 2020 2020 2020 2020 202e  :..            .
-00002110: 2e2e 0d0a 0d0a 4f6e 6365 2074 6865 206f  ......Once the o
-00002120: 7363 696c 6c6f 7363 6f70 6520 6973 2063  scilloscope is c
-00002130: 6f6e 6e65 6374 6564 2074 6f20 7468 6520  onnected to the 
-00002140: 6170 706c 6963 6174 696f 6e2c 2079 6f75  application, you
-00002150: 2063 616e 2075 7365 2074 6865 2074 6572   can use the ter
-00002160: 6d69 6e61 6c20 746f 2065 7870 6c6f 7265  minal to explore
-00002170: 2074 6865 206f 7363 696c 6c6f 7363 6f70   the oscilloscop
-00002180: 652e 0d0a 0d0a 2e2e 2066 6967 7572 653a  e....... figure:
-00002190: 3a20 2e2f 5f73 7461 7469 632f 6f73 632d  : ./_static/osc-
-000021a0: 6469 722d 7465 726d 696e 616c 2d73 6372  dir-terminal-scr
-000021b0: 6565 6e2d 6361 7074 7572 652e 706e 670d  een-capture.png.
-000021c0: 0a20 2020 203a 616c 6967 6e3a 2063 656e  .    :align: cen
-000021d0: 7465 720d 0a20 2020 203a 6669 6763 6c61  ter..    :figcla
-000021e0: 7373 3a20 616c 6967 6e2d 6365 6e74 6572  ss: align-center
-000021f0: 0d0a 0d0a 7c0d 0a0d 0a42 6563 6173 7565  ....|....Becasue
-00002200: 2027 6f73 6327 2069 7320 6e6f 7420 7468   'osc' is not th
-00002210: 6520 6465 6661 756c 7420 696e 7374 7275  e default instru
-00002220: 6d65 6e74 2c20 796f 7520 6861 7665 2074  ment, you have t
-00002230: 6f20 7573 6520 7468 6520 7072 6566 6978  o use the prefix
-00002240: 2027 6f73 633a 2720 7769 7468 2061 6c6c   'osc:' with all
-00002250: 2074 6865 0d0a 7261 7720 7265 6d6f 7465   the..raw remote
-00002260: 2063 6f6d 6d61 6e64 7320 796f 7520 7365   commands you se
-00002270: 6e64 2074 6f20 7468 6520 696e 7374 7275  nd to the instru
-00002280: 6d65 6e74 2e20 4173 2073 686f 776e 2077  ment. As shown w
-00002290: 6974 6820 276f 7363 2e64 6972 272c 2074  ith 'osc.dir', t
-000022a0: 6865 7265 2061 7265 206d 616e 7920 6d65  here are many me
-000022b0: 7468 6f64 730d 0a61 7661 6961 626c 6520  thods..avaiable 
-000022c0: 7769 7468 2027 6f73 632e 2720 4576 656e  with 'osc.' Even
-000022d0: 206f 7363 2e67 6574 5f77 6176 6566 6f72   osc.get_wavefor
-000022e0: 6d28 2920 6973 2061 7661 696c 6162 6c65  m() is available
-000022f0: 2066 726f 6d20 7468 6520 7465 726d 696e   from the termin
-00002300: 616c 2e20 5468 6520 7465 726d 696e 616c  al. The terminal
-00002310: 206b 696e 646c 790d 0a74 656c 6c73 206d   kindly..tells m
-00002320: 6520 7468 6174 2074 6865 7265 2069 7320  e that there is 
-00002330: 6120 6d69 7373 696e 6720 6172 6775 6d65  a missing argume
-00002340: 6e74 2069 6e20 6120 6675 6e63 7469 6f6e  nt in a function
-00002350: 2063 616c 6c2c 2077 6865 6e20 796f 7520   call, when you 
-00002360: 7573 6520 6120 6d65 7468 6f64 2069 6e63  use a method inc
-00002370: 6f72 7265 6374 6c79 2e0d 0a59 6f75 2063  orrectly...You c
-00002380: 616e 2073 6565 206f 7363 2e67 6574 5f77  an see osc.get_w
-00002390: 6176 6566 6f72 6d28 6368 616e 6e65 6c29  aveform(channel)
-000023a0: 206d 6574 686f 6420 7265 7475 726e 7320   method returns 
-000023b0: 7477 6f20 6e75 6d70 7920 6172 7261 792c  two numpy array,
-000023c0: 2069 6620 796f 7520 7275 6e20 6974 2e0d   if you run it..
-000023d0: 0a53 696e 6365 2074 6865 2074 6572 6d69  .Since the termi
-000023e0: 6e61 6c20 6f6e 6c79 2061 6c6c 6f77 2074  nal only allow t
-000023f0: 6f20 7573 6520 6174 7472 6962 7574 6573  o use attributes
-00002400: 2061 6e64 206d 6574 686f 6473 206f 6620   and methods of 
-00002410: 696e 7374 7275 6d65 6e74 7320 6465 6669  instruments defi
-00002420: 6e65 6420 696e 2074 6865 0d0a 636f 6e66  ned in the..conf
-00002430: 6967 7572 6174 696f 6e20 6669 6c65 2c20  iguration file, 
-00002440: 6966 2079 6f75 2068 6176 6520 6d6f 7265  if you have more
-00002450: 2075 7365 6675 6c20 6d65 7468 6f64 7320   useful methods 
-00002460: 6465 6669 6e65 6420 666f 7220 7468 6520  defined for the 
-00002470: 696e 7374 7275 6d65 6e74 2c0d 0a79 6f75  instrument,..you
-00002480: 2063 616e 2064 6f20 6d6f 7265 2069 6e20   can do more in 
-00002490: 7468 6520 7465 726d 696e 616c 2e20 486f  the terminal. Ho
-000024a0: 7765 7665 722c 2079 6f75 2061 7265 2073  wever, you are s
-000024b0: 7570 706f 7365 6420 746f 2072 756e 206d  upposed to run m
-000024c0: 6f72 6520 736f 7068 6973 7469 6361 7465  ore sophisticate
-000024d0: 6420 6461 7461 0d0a 6861 6e64 6c69 6e67  d data..handling
-000024e0: 2069 6e20 7461 736b 7320 6e6f 7420 6672   in tasks not fr
-000024f0: 6f6d 2074 6865 2074 6572 6d69 6e61 6c2e  om the terminal.
-00002500: 0d0a 0d0a 5461 736b 730d 0a2d 2d2d 2d2d  ....Tasks..-----
-00002510: 2d2d 0d0a 0d0a 486f 7720 746f 2072 756e  --....How to run
-00002520: 2061 2074 6173 6b0d 0a5e 5e5e 5e5e 5e5e   a task..^^^^^^^
-00002530: 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e 0d0a 0d0a  ^^^^^^^^^^^^....
-00002540: 5374 6172 7420 6060 7372 7367 7569 6060  Start ``srsgui``
-00002550: 2061 7070 6c69 6361 7469 6f6e 2e20 596f   application. Yo
-00002560: 7520 6361 6e20 7365 6520 7768 6572 6520  u can see where 
-00002570: 7468 6520 2e63 6f6e 6669 6720 6669 6c65  the .config file
-00002580: 2069 7320 6f70 656e 6564 0d0a 6672 6f6d   is opened..from
-00002590: 2074 6865 2063 6f6e 736f 6c65 2077 696e   the console win
-000025a0: 646f 7720 283a 7265 663a 6068 6572 6520  dow (:ref:`here 
-000025b0: 3c74 6f70 2d6f 662d 696e 6974 6961 6c2d  <top-of-initial-
-000025c0: 7363 7265 656e 2d63 6170 7475 7265 3e60  screen-capture>`
-000025d0: 292e 0d0a 4966 2079 6f75 206d 6164 6520  )...If you made 
-000025e0: 6120 636f 7079 206f 6620 7468 6520 6f72  a copy of the or
-000025f0: 6967 696e 616c 2065 7861 6d70 6c65 2066  iginal example f
-00002600: 726f 6d20 7468 6520 6060 7372 7367 7569  rom the ``srsgui
-00002610: 6060 0d0a 7061 636b 6167 6520 6469 7265  ``..package dire
-00002620: 6374 6f72 792c 206f 7065 6e20 6974 2061  ctory, open it a
-00002630: 6761 696e 2066 726f 6d20 7468 6520 636f  gain from the co
-00002640: 7272 6563 7420 6469 7265 6374 6f72 792e  rrect directory.
-00002650: 0d0a 0d0a 4966 2074 6865 7265 2069 7320  ....If there is 
-00002660: 6e6f 2065 7272 6f72 206d 6573 7361 6765  no error message
-00002670: 2069 6e20 7468 6520 436f 6e73 6f6c 6520   in the Console 
-00002680: 7769 6e64 6f77 2c20 636f 6e6e 6563 7420  window, connect 
-00002690: 7468 6520 6675 6e63 7469 6f6e 2067 656e  the function gen
-000026a0: 6572 6174 6f72 0d0a 616e 6420 7468 6520  erator..and the 
-000026b0: 6f73 6369 6c6c 6f73 636f 7065 2066 726f  oscilloscope fro
-000026c0: 6d20 7468 6520 496e 7374 7275 6d65 6e74  m the Instrument
-000026d0: 7320 6d65 6e75 2c20 636c 6963 6b69 6e67  s menu, clicking
-000026e0: 2074 6865 2069 6e73 7472 756d 656e 7420   the instrument 
-000026f0: 6e61 6d65 0d0a 7468 6174 2079 6f75 2077  name..that you w
-00002700: 616e 7420 746f 2063 6f6e 6e65 6374 2e0d  ant to connect..
-00002710: 0a0d 0a53 656c 6563 7420 7468 6520 6669  ...Select the fi
-00002720: 7273 7420 7461 736b 2028 5c2a 4944 4e20  rst task (\*IDN 
-00002730: 7465 7374 2920 6672 6f6d 2074 6865 2054  test) from the T
-00002740: 6173 6b73 206d 656e 7520 6f72 206f 7468  asks menu or oth
-00002750: 6572 6573 2069 6e20 7468 6520 5461 736b  eres in the Task
-00002760: 7320 6d65 6e75 0d0a 616e 6420 636c 6963  s menu..and clic
-00002770: 6b20 7468 6520 6772 6565 6e20 6172 726f  k the green arro
-00002780: 7720 696e 2074 6865 2074 6f6f 6c20 6261  w in the tool ba
-00002790: 7220 746f 2072 756e 2074 6865 2074 6173  r to run the tas
-000027a0: 6b2e 0d0a 0d0a 0d0a 5468 6520 6f76 6572  k.......The over
-000027b0: 616c 6c20 7374 7275 6374 7572 6520 6f66  all structure of
-000027c0: 2061 2074 6173 6b20 6973 2064 6573 6372   a task is descr
-000027d0: 6962 6564 2069 6e20 3a72 6566 3a60 5772  ibed in :ref:`Wr
-000027e0: 6974 696e 6720 6120 7461 736b 2073 6372  iting a task scr
-000027f0: 6970 7460 2073 6563 7469 6f6e 2e0d 0a54  ipt` section...T
-00002800: 6865 7265 2061 7265 2035 2074 6173 6b73  here are 5 tasks
-00002810: 2061 7265 2069 6e63 6c75 6465 6420 696e   are included in
-00002820: 2074 6865 2065 7861 6d70 6c65 2070 726f   the example pro
-00002830: 6a65 6374 2e20 5468 6579 2067 7261 6475  ject. They gradu
-00002840: 616c 6c79 2061 6464 7320 6d6f 7265 2066  ally adds more f
-00002850: 6561 7475 7265 730d 0a6f 6e20 7468 6520  eatures..on the 
-00002860: 746f 7020 6f66 2074 6865 2070 7265 7669  top of the previ
-00002870: 6f75 7320 7461 736b 732e 2048 6f70 6566  ous tasks. Hopef
-00002880: 756c 6c79 2c20 7468 6579 2073 686f 7720  ully, they show 
-00002890: 6d6f 7374 206f 6620 5461 736b 2063 6c61  most of Task cla
-000028a0: 7373 2075 7361 6765 2e0d 0a0d 0a0d 0a46  ss usage.......F
-000028b0: 6972 7374 5461 736b 0d0a 2d2d 2d2d 2d2d  irstTask..------
-000028c0: 2d2d 2d2d 2d0d 0a0d 0a54 6865 2066 6972  -----....The fir
-000028d0: 7374 2074 6173 6b20 7368 6f77 733a 0d0a  st task shows:..
-000028e0: 0d0a 2020 2020 2d20 486f 7720 746f 2075  ..    - How to u
-000028f0: 7365 206d 6f64 756c 652d 6c65 7665 6c20  se module-level 
-00002900: 6c6f 6767 6572 2066 6f72 2050 7974 686f  logger for Pytho
-00002910: 6e20 6c6f 6767 696e 675f 2069 6e20 6120  n logging_ in a 
-00002920: 7461 736b 0d0a 2020 2020 2d20 486f 7720  task..    - How 
-00002930: 746f 2075 7365 2069 6e73 7472 756d 656e  to use instrumen
-00002940: 7473 2064 6566 696e 6564 2069 6e20 7468  ts defined in th
-00002950: 6520 636f 6e66 6967 7572 6174 696f 6e20  e configuration 
-00002960: 6669 6c65 0d0a 2020 2020 2d20 486f 7720  file..    - How 
-00002970: 746f 2075 7365 2074 6578 7420 6f75 7470  to use text outp
-00002980: 7574 2074 6f20 7468 6520 636f 6e73 6f6c  ut to the consol
-00002990: 6520 7769 6e64 6f77 0d0a 0d0a 4974 2069  e window....It i
-000029a0: 7320 6e6f 7420 6d75 6368 2064 6966 6665  s not much diffe
-000029b0: 7265 6e74 2066 726f 6d20 7468 6520 3a72  rent from the :r
-000029c0: 6566 3a60 6261 7265 2062 6f6e 6520 7374  ef:`bare bone st
-000029d0: 7275 6374 7572 6520 3c74 6f70 2d6f 662d  ructure <top-of-
-000029e0: 6261 7265 2d62 6f6e 652d 7461 736b 3e60  bare-bone-task>`
-000029f0: 0d0a 7368 6f77 6e20 696e 2074 6865 203a  ..shown in the :
-00002a00: 7265 663a 6057 7269 7469 6e67 2061 2074  ref:`Writing a t
-00002a10: 6173 6b20 7363 7269 7074 6020 7365 6374  ask script` sect
-00002a20: 696f 6e2e 0d0a 0d0a 2e2e 206c 6974 6572  ion....... liter
-00002a30: 616c 696e 636c 7564 653a 3a20 2e2e 2f73  alinclude:: ../s
-00002a40: 7273 6775 692f 6578 616d 706c 6573 2f6f  rsgui/examples/o
-00002a50: 7363 696c 6c6f 7363 6f70 6520 6578 616d  scilloscope exam
-00002a60: 706c 652f 7461 736b 732f 6669 7273 742e  ple/tasks/first.
-00002a70: 7079 0d0a 2020 2020 3a6c 616e 6775 6167  py..    :languag
-00002a80: 653a 2050 7974 686f 6e0d 0a20 2020 203a  e: Python..    :
-00002a90: 6c69 6e65 6e6f 733a 0d0a 0d0a 5573 696e  linenos:....Usin
-00002aa0: 6720 2a2a 7365 6c66 2e6c 6f67 6765 722a  g **self.logger*
-00002ab0: 2a20 7365 6e64 7320 7468 6520 6c6f 6767  * sends the logg
-00002ac0: 696e 6720 6f75 7470 7574 2074 6f20 7468  ing output to th
-00002ad0: 6520 636f 6e73 6f6c 6520 7769 6e64 6f77  e console window
-00002ae0: 2c20 7468 6520 6d61 7374 6572 206c 6f67  , the master log
-00002af0: 6769 6e67 2066 696c 6520 696e 0d0a 7e2f  ging file in..~/
-00002b00: 7461 736b 2d72 6573 756c 7473 2064 6972  task-results dir
-00002b10: 6563 746f 7279 2f6d 6169 6e6c 6f67 2d78  ectory/mainlog-x
-00002b20: 782e 7478 742e 782c 2061 6e64 2074 6f20  x.txt.x, and to 
-00002b30: 7468 6520 7461 736b 2072 6573 756c 7420  the task result 
-00002b40: 6461 7461 2066 696c 6520 6c6f 6361 7465  data file locate
-00002b50: 6420 696e 0d0a 7e2f 7461 736b 2d72 6573  d in..~/task-res
-00002b60: 756c 7473 2f70 726f 6a65 6374 2d6e 616d  ults/project-nam
-00002b70: 652d 696e 2d63 6f6e 6669 672d 6669 6c65  e-in-config-file
-00002b80: 2f52 4e78 7878 2064 6972 6563 746f 7279  /RNxxx directory
-00002b90: 2e0d 0a0d 0a57 6974 6820 3a6d 6574 683a  .....With :meth:
-00002ba0: 6067 6574 5f69 6e73 7472 756d 656e 7420  `get_instrument 
-00002bb0: 3c73 7273 6775 692e 7461 736b 2e74 6173  <srsgui.task.tas
-00002bc0: 6b2e 5461 736b 2e67 6574 5f69 6e73 7472  k.Task.get_instr
-00002bd0: 756d 656e 743e 6020 796f 7520 6361 6e20  ument>` you can 
-00002be0: 6765 7420 7468 6520 696e 7374 7275 6d65  get the instrume
-00002bf0: 6e74 0d0a 6465 6669 6e65 6420 696e 2074  nt..defined in t
-00002c00: 6865 2063 6f6e 6669 6775 7261 7469 6f6e  he configuration
-00002c10: 2066 696c 6520 696e 2061 2074 6173 6b2e   file in a task.
-00002c20: 202a 2a44 6f20 6e6f 7420 6469 7363 6f6e   **Do not discon
-00002c30: 6e65 6374 2074 6865 2069 6e73 7472 756d  nect the instrum
-00002c40: 656e 7420 696e 2074 6865 2074 6173 6b21  ent in the task!
-00002c50: 2a2a 0d0a 496e 7374 7275 6d65 6e74 2043  **..Instrument C
-00002c60: 6f6e 6e65 6374 6976 6974 7920 6973 206d  onnectivity is m
-00002c70: 616e 6167 6564 2069 6e20 7468 6520 6170  anaged in the ap
-00002c80: 706c 6963 6174 696f 6e20 6c65 7665 6c2e  plication level.
-00002c90: 0d0a 0d0a 4974 2073 686f 7720 686f 7720  ....It show how 
-00002ca0: 6d75 6368 2069 7420 7369 6d70 6c69 6669  much it simplifi
-00002cb0: 6573 2072 656d 6f74 6520 636f 6d6d 616e  es remote comman
-00002cc0: 6420 7365 7420 616e 6420 7175 6572 7920  d set and query 
-00002cd0: 7472 616e 7361 6374 696f 6e73 2062 7920  transactions by 
-00002ce0: 6465 6669 6e69 6e67 2066 7265 7175 656e  defining frequen
-00002cf0: 6379 0d0a 6174 7472 6962 7574 6520 7573  cy..attribute us
-00002d00: 696e 6720 3a6d 6f64 3a60 7372 7367 7569  ing :mod:`srsgui
-00002d10: 2e69 6e73 742e 636f 6d6d 616e 6473 6020  .inst.commands` 
-00002d20: 6d6f 6475 6c65 2e0d 0a0d 0a53 6563 6f6e  module.....Secon
-00002d30: 6454 6173 6b0d 0a2d 2d2d 2d2d 2d2d 2d2d  dTask..---------
-00002d40: 2d2d 0d0a 0d0a 5468 6520 7365 636f 6e64  --....The second
-00002d50: 2074 6173 6b20 7368 6f77 733a 0d0a 0d0a   task shows:....
-00002d60: 2020 2020 2d20 486f 7720 746f 2064 6566      - How to def
-00002d70: 696e 6520 3a61 7474 723a 6069 6e70 7574  ine :attr:`input
-00002d80: 5f70 6172 616d 6574 6572 7320 3c73 7273  _parameters <srs
-00002d90: 6775 692e 7461 736b 2e74 6173 6b2e 5461  gui.task.task.Ta
-00002da0: 736b 2e69 6e70 7574 5f70 6172 616d 6574  sk.input_paramet
-00002db0: 6572 733e 600d 0a20 2020 2020 2066 6f72  ers>`..      for
-00002dc0: 2069 6e74 6572 6163 7469 7665 2075 7365   interactive use
-00002dd0: 7220 696e 7075 7420 6672 6f6d 2074 6865  r input from the
-00002de0: 2061 7070 6c69 6361 7469 6f6e 2069 6e70   application inp
-00002df0: 7574 2070 616e 656c 0d0a 2020 2020 2d20  ut panel..    - 
-00002e00: 486f 7720 746f 2067 6574 206d 6174 706c  How to get matpl
-00002e10: 6f67 6c69 6220 6669 6775 7265 2061 6e64  oglib figure and
-00002e20: 2075 7365 2069 7420 746f 2070 6c6f 740d   use it to plot.
-00002e30: 0a20 2020 202d 2048 6f77 2074 6f20 7365  .    - How to se
-00002e40: 6e64 2074 6578 7420 6f75 7470 7574 2074  nd text output t
-00002e50: 6f20 7265 7375 6c74 2077 696e 646f 7720  o result window 
-00002e60: 7573 696e 670d 0a20 2020 2020 203a 6d65  using..      :me
-00002e70: 7468 3a60 6469 7370 6c61 795f 7265 7375  th:`display_resu
-00002e80: 6c74 2829 203c 7372 7367 7569 2e74 6173  lt() <srsgui.tas
-00002e90: 6b2e 7461 736b 2e54 6173 6b2e 6469 7370  k.task.Task.disp
-00002ea0: 6c61 795f 7265 7375 6c74 3e60 0d0a 2020  lay_result>`..  
-00002eb0: 2020 2d20 486f 7720 746f 2073 746f 7020    - How to stop 
-00002ec0: 7468 6520 6d61 696e 206c 6f6f 7020 6279  the main loop by
-00002ed0: 2063 6865 636b 696e 670d 0a20 2020 2020   checking..     
-00002ee0: 203a 6d65 7468 3a60 6973 5f72 756e 6e69   :meth:`is_runni
-00002ef0: 6e67 2829 203c 7372 7367 7569 2e74 6173  ng() <srsgui.tas
-00002f00: 6b2e 7461 736b 2e54 6173 6b2e 6973 5f72  k.task.Task.is_r
-00002f10: 756e 6e69 6e67 3e60 2e0d 0a0d 0a2e 2e20  unning>`....... 
-00002f20: 6c69 7465 7261 6c69 6e63 6c75 6465 3a3a  literalinclude::
-00002f30: 202e 2e2f 7372 7367 7569 2f65 7861 6d70   ../srsgui/examp
-00002f40: 6c65 732f 6f73 6369 6c6c 6f73 636f 7065  les/oscilloscope
-00002f50: 2065 7861 6d70 6c65 2f74 6173 6b73 2f73   example/tasks/s
-00002f60: 6563 6f6e 642e 7079 0d0a 2020 2020 3a6c  econd.py..    :l
-00002f70: 616e 6775 6167 653a 2050 7974 686f 6e0d  anguage: Python.
-00002f80: 0a20 2020 203a 6c69 6e65 6e6f 733a 0d0a  .    :linenos:..
-00002f90: 0d0a 5573 696e 6720 6d61 7470 6c6f 746c  ..Using matplotl
-00002fa0: 6962 5f20 6973 2073 7472 6169 6768 7466  ib_ is straightf
-00002fb0: 6f72 7761 7264 2e20 4e6f 2068 6172 6465  orward. No harde
-00002fc0: 7220 7468 616e 2073 7461 6e64 6172 6420  r than standard 
-00002fd0: 706c 6f74 7320 7573 696e 6720 6669 6775  plots using figu
-00002fe0: 7265 7320 616e 6420 6178 6573 2e0d 0a52  res and axes...R
-00002ff0: 6566 6572 2074 6f20 6d61 7470 6c6f 746c  efer to matplotl
-00003000: 6962 5f20 646f 6375 6d65 6e74 6174 696f  ib_ documentatio
-00003010: 6e20 6f6e 2068 6f77 2074 6f20 7573 6520  n on how to use 
-00003020: 6974 2e0d 0a0d 0a54 6865 2069 6d70 6f72  it.....The impor
-00003030: 7461 6e74 2064 6966 6665 7265 6e63 6573  tant differences
-00003040: 2075 7369 6e67 206d 6174 706c 6f74 6c69   using matplotli
-00003050: 6220 696e 2060 6073 7273 6775 6960 6020  b in ``srsgui`` 
-00003060: 6172 653a 0d0a 2020 2020 2d20 596f 7520  are:..    - You 
-00003070: 6861 7665 2074 6f20 6765 7420 7468 6520  have to get the 
-00003080: 6669 6775 7265 2075 7369 6e67 2067 6574  figure using get
-00003090: 5f66 6967 7572 6528 292c 206e 6f74 2063  _figure(), not c
-000030a0: 7265 6174 696e 6720 6f6e 6520 206f 6e20  reating one  on 
-000030b0: 796f 7572 206f 776e 2e0d 0a20 2020 202d  your own...    -
-000030c0: 2059 6f75 2063 7265 6174 6520 706c 6f74   You create plot
-000030d0: 7320 6475 7269 6e67 2073 6574 7570 2829  s during setup()
-000030e0: 2c20 6265 6361 7573 6520 6974 2069 7320  , because it is 
-000030f0: 736c 6f77 2070 726f 6365 7373 2e20 4475  slow process. Du
-00003100: 7269 6e67 2074 6573 7428 292c 0d0a 2020  ring test(),..  
-00003110: 2020 2020 796f 7520 6a75 7374 2075 7064      you just upd
-00003120: 6174 6520 6461 7461 2075 7369 6e67 2073  ate data using s
-00003130: 6574 5f64 6174 6128 2920 6f72 2073 696d  et_data() or sim
-00003140: 696c 6961 7220 6d65 7468 6f64 7320 666f  iliar methods fo
-00003150: 7220 6461 7461 2075 7064 6174 652e 0d0a  r data update...
-00003160: 2020 2020 2d20 596f 7520 6861 7665 2075      - You have u
-00003170: 7365 2072 6571 7565 7374 5f66 6967 7572  se request_figur
-00003180: 655f 7570 6461 7465 2829 2074 6f20 7265  e_update() to re
-00003190: 6472 6177 2074 6865 2070 6c6f 742c 2061  draw the plot, a
-000031a0: 6674 6572 2073 6574 5f64 6174 6128 292e  fter set_data().
-000031b0: 0d0a 2020 2020 2020 5468 6520 6576 656e  ..      The even
-000031c0: 7420 6c6f 6f70 2068 616e 646c 6572 2069  t loop handler i
-000031d0: 6e20 7468 6520 6d61 696e 2061 7070 6c69  n the main appli
-000031e0: 6361 7469 6f6e 2077 696c 6c20 7570 6461  cation will upda
-000031f0: 7465 2074 6865 2070 6c6f 7420 6174 2069  te the plot at i
-00003200: 7473 2065 6172 6c69 6573 740d 0a20 2020  ts earliest..   
-00003210: 2020 2063 6f6e 7665 6e69 656e 6365 2e0d     convenience..
-00003220: 0a0d 0a0d 0a2e 2e20 6669 6775 7265 3a3a  ....... figure::
-00003230: 202e 2f5f 7374 6174 6963 2f73 6563 6f6e   ./_static/secon
-00003240: 642d 7461 736b 2d73 6372 6565 6e2d 6361  d-task-screen-ca
-00003250: 7074 7572 652e 706e 670d 0a20 2020 203a  pture.png..    :
-00003260: 616c 6967 6e3a 2063 656e 7465 720d 0a20  align: center.. 
-00003270: 2020 203a 6669 6763 6c61 7373 3a20 616c     :figclass: al
-00003280: 6967 6e2d 6365 6e74 6572 0d0a 0d0a 7c0d  ign-center....|.
-00003290: 0a0d 0a54 6869 7264 5461 736b 0d0a 2d2d  ...ThirdTask..--
-000032a0: 2d2d 2d2d 2d2d 2d2d 2d0d 0a0d 0a54 6865  ---------....The
-000032b0: 2074 6869 7264 2074 6173 6b20 7573 6573   third task uses
-000032c0: 2074 6865 206f 7363 696c 6c6f 7363 6f70   the oscilloscop
-000032d0: 6520 6f6e 6c79 2e20 4974 2067 6574 7320  e only. It gets 
-000032e0: 7468 6520 6e75 6d62 6572 206f 6620 6361  the number of ca
-000032f0: 7074 7572 6573 2066 726f 6d20 7573 6572  ptures from user
-00003300: 2069 6e70 7574 2c0d 0a72 6570 6561 7420   input,..repeat 
-00003310: 6f73 6369 6c6c 6f73 636f 7065 2077 6176  oscilloscope wav
-00003320: 6566 6f72 6d20 6361 7074 7572 6520 616e  eform capture an
-00003330: 6420 7570 6461 7465 2074 6865 2077 6176  d update the wav
-00003340: 6566 6f72 6d20 706c 6f74 2e20 4974 2073  eform plot. It s
-00003350: 746f 7073 2061 6674 6572 2072 6570 6561  tops after repea
-00003360: 7473 0d0a 7468 6520 6e75 6d62 6572 206f  ts..the number o
-00003370: 6620 7469 6d65 7320 7365 6c65 6374 6564  f times selected
-00003380: 2062 6572 666f 7265 2072 756e 2c20 6f72   berfore run, or
-00003390: 2077 6865 6e20 7468 6520 5374 6f70 2062   when the Stop b
-000033a0: 7574 746f 6e20 6973 2070 7265 7373 7565  utton is pressue
-000033b0: 642e 0d0a 5768 656e 2069 7420 7275 6e73  d...When it runs
-000033c0: 2069 7420 6361 7074 7572 6573 2061 6e64   it captures and
-000033d0: 2064 6973 706c 6179 2061 2077 6176 6566   display a wavef
-000033e0: 6f72 6d20 7769 7468 2037 3030 3030 3020  orm with 700000 
-000033f0: 706f 696e 7473 2065 7665 7279 2030 2e32  points every 0.2
-00003400: 2073 6563 6f6e 640d 0a6f 7665 7220 5443   second..over TC
-00003410: 5049 5020 636f 6d6d 756e 6361 7469 6f6e  PIP communcation
-00003420: 2e0d 0a0d 0a0d 0a2e 2e20 6c69 7465 7261  ......... litera
-00003430: 6c69 6e63 6c75 6465 3a3a 202e 2e2f 7372  linclude:: ../sr
-00003440: 7367 7569 2f65 7861 6d70 6c65 732f 6f73  sgui/examples/os
-00003450: 6369 6c6c 6f73 636f 7065 2065 7861 6d70  cilloscope examp
-00003460: 6c65 2f74 6173 6b73 2f74 6869 7264 2e70  le/tasks/third.p
-00003470: 790d 0a20 2020 203a 6c61 6e67 7561 6765  y..    :language
-00003480: 3a20 5079 7468 6f6e 0d0a 2020 2020 3a6c  : Python..    :l
-00003490: 696e 656e 6f73 3a0d 0a0d 0a46 6f75 7274  inenos:....Fourt
-000034a0: 6854 6173 6b0d 0a2d 2d2d 2d2d 2d2d 2d2d  hTask..---------
-000034b0: 2d2d 0d0a 0d0a 5468 6520 666f 7572 7468  --....The fourth
-000034c0: 2065 7861 6d70 6c65 2069 7320 7468 6520   example is the 
-000034d0: 636c 696d 6178 206f 6620 7468 6520 6578  climax of the ex
-000034e0: 616d 706c 6573 2073 6572 6965 732e 2049  amples series. I
-000034f0: 7420 7573 6573 2069 6e70 7574 5f70 6172  t uses input_par
-00003500: 616d 6574 6572 730d 0a74 6f20 6368 616e  ameters..to chan
-00003510: 6765 206f 7574 7075 7420 6672 6571 7565  ge output freque
-00003520: 6e63 7920 6f66 2074 6865 2063 6c6f 636b  ncy of the clock
-00003530: 2067 656e 6572 6174 6f72 2069 6e74 6572   generator inter
-00003540: 6163 7469 7665 6c79 2c20 6361 7074 7572  actively, captur
-00003550: 6573 2077 6176 6566 6f72 6d73 0d0a 6672  es waveforms..fr
-00003560: 6f6d 2074 6865 206f 7363 696c 6c6f 7363  om the oscillosc
-00003570: 6f70 652c 2072 756e 2046 4654 206f 6620  ope, run FFT of 
-00003580: 7468 6520 7761 7665 666f 726d 7320 7769  the waveforms wi
-00003590: 7468 204e 756d 7079 2c20 616e 6420 706c  th Numpy, and pl
-000035a0: 6f74 0d0a 7573 696e 6720 3220 6d61 7470  ot..using 2 matp
-000035b0: 6c6f 746c 6962 2066 6967 7572 6573 2e0d  lotlib figures..
-000035c0: 0a0d 0a62 7920 6164 6469 6e67 2074 6865  ...by adding the
-000035d0: 206e 616d 6573 206f 6620 6669 6775 7265   names of figure
-000035e0: 7320 7468 6174 2079 6f75 2077 616e 7420  s that you want 
-000035f0: 746f 2075 7365 2069 6e20 6164 6469 7469  to use in additi
-00003600: 6f6e 616c 5f66 6967 7572 655f 6e61 6d65  onal_figure_name
-00003610: 732c 0d0a 6060 7372 7367 7569 6060 2070  s,..``srsgui`` p
-00003620: 726f 7669 6465 7320 6d6f 7265 2066 6967  rovides more fig
-00003630: 7572 6573 2074 6f20 7468 6520 7461 736b  ures to the task
-00003640: 2062 6566 6f72 6520 6974 2073 7461 7274   before it start
-00003650: 732e 0d0a 0d0a 2e2e 206c 6974 6572 616c  s....... literal
-00003660: 696e 636c 7564 653a 3a20 2e2e 2f73 7273  include:: ../srs
-00003670: 6775 692f 6578 616d 706c 6573 2f6f 7363  gui/examples/osc
-00003680: 696c 6c6f 7363 6f70 6520 6578 616d 706c  illoscope exampl
-00003690: 652f 7461 736b 732f 666f 7572 7468 2e70  e/tasks/fourth.p
-000036a0: 790d 0a20 2020 203a 6c61 6e67 7561 6765  y..    :language
-000036b0: 3a20 5079 7468 6f6e 0d0a 2020 2020 3a6c  : Python..    :l
-000036c0: 696e 656e 6f73 3a0d 0a0d 0a46 6966 7468  inenos:....Fifth
-000036d0: 5461 736b 0d0a 2d2d 2d2d 2d2d 2d2d 2d2d  Task..----------
-000036e0: 0d0a 0d0a 7468 6520 6669 6674 6820 6578  ....the fifth ex
-000036f0: 616d 706c 6573 2069 7320 746f 2073 686f  amples is to sho
-00003700: 7720 686f 7720 746f 2073 7562 636c 6173  w how to subclas
-00003710: 7320 616e 2065 7869 7374 696e 6720 7461  s an existing ta
-00003720: 736b 2063 6c61 7373 2074 6f20 7265 7573  sk class to reus
-00003730: 652e 0d0a 7468 6520 6d65 7468 6f64 2067  e...the method g
-00003740: 6574 5f77 6176 6566 6f72 6d28 2920 696e  et_waveform() in
-00003750: 2074 6865 2066 6f75 7274 6820 6578 616d   the fourth exam
-00003760: 706c 6520 6973 2072 6569 6d70 6c65 6d65  ple is reimpleme
-00003770: 6e74 6564 2074 6f20 6765 6e65 7261 7465  nted to generate
-00003780: 0d0a 7369 6d75 6c61 7465 6420 7761 7665  ..simulated wave
-00003790: 666f 726d 2074 6861 7420 7275 6e73 2077  form that runs w
-000037a0: 6974 686f 7574 2061 6e79 2072 6561 6c20  ithout any real 
-000037b0: 6f73 6369 6c6c 6f73 636f 7065 2e0d 0a0d  oscilloscope....
-000037c0: 0a4e 6f74 6520 7468 6174 2074 6865 2073  .Note that the s
-000037d0: 7175 6172 6520 7761 7665 2065 6467 6520  quare wave edge 
-000037e0: 6361 6c63 756c 6174 696f 6e20 6973 2063  calculation is c
-000037f0: 7275 6465 2c20 616e 6420 6361 7573 696e  rude, and causin
-00003800: 6720 6d6f 6475 6c61 7469 6f6e 2069 6e20  g modulation in 
-00003810: 7075 6c73 6520 7769 6474 680d 0a74 6861  pulse width..tha
-00003820: 7420 7368 6f77 7320 7369 6465 2062 616e  t shows side ban
-00003830: 6473 2069 6e20 4646 5420 7370 6563 7472  ds in FFT spectr
-00003840: 756d 2c20 6966 2074 6865 2073 6574 2066  um, if the set f
-00003850: 7265 7175 656e 6379 2069 7320 6e6f 7420  requency is not 
-00003860: 636f 6d6d 656e 7375 7261 7465 6420 7769  commensurated wi
-00003870: 7468 0d0a 7468 6520 7361 6d70 6c69 6e67  th..the sampling
-00003880: 2072 6174 652e 2054 6f20 6765 6e65 7261   rate. To genera
-00003890: 7465 2063 6c65 616e 2073 7175 6172 6520  te clean square 
-000038a0: 7761 7665 2c20 7468 6520 7269 7369 6e67  wave, the rising
-000038b0: 2061 6e64 2066 616c 6c69 6e67 2065 6467   and falling edg
-000038c0: 6573 2073 686f 756c 640d 0a68 6176 6520  es should..have 
-000038d0: 6174 206c 6561 7374 2074 776f 2070 6f69  at least two poi
-000038e0: 6e74 7320 746f 2072 6570 7265 7365 6e74  nts to represent
-000038f0: 2065 7861 6374 2070 6861 7365 2e20 4469   exact phase. Di
-00003900: 7265 6374 2074 7261 6e73 6974 696f 6e20  rect transition 
-00003910: 6672 6f6d 206c 6f77 2074 6f20 6869 6768  from low to high
-00003920: 0d0a 7769 7468 6f75 7420 616e 7920 696e  ..without any in
-00003930: 7465 726d 6564 6961 7465 2070 6f69 6e74  termediate point
-00003940: 7320 7375 6666 6572 7320 6672 6f6d 2073  s suffers from s
-00003950: 7562 746c 6520 6d6f 6475 6c61 7469 6f6e  ubtle modulation
-00003960: 2069 6e20 7469 6d65 2064 6f6d 6169 6e2c   in time domain,
-00003970: 0d0a 7768 6963 6820 6d61 6e69 6665 7374  ..which manifest
-00003980: 7320 6173 2073 6964 6520 6261 6e64 7320  s as side bands 
-00003990: 696e 2046 4654 2e20 5468 6973 2069 7320  in FFT. This is 
-000039a0: 6120 636f 6d6d 6f6e 2070 726f 626c 656d  a common problem
-000039b0: 2069 6e20 6469 6769 7461 6c20 7369 676e   in digital sign
-000039c0: 616c 0d0a 7072 6f63 6573 7369 6e67 2e20  al..processing. 
-000039d0: 4974 2069 7320 6e6f 7420 6120 7072 6f62  It is not a prob
-000039e0: 6c65 6d20 696e 2074 6865 2072 6561 6c20  lem in the real 
-000039f0: 776f 726c 642c 2062 6563 6175 7365 2074  world, because t
-00003a00: 6865 2073 6967 6e61 6c20 6973 2061 6e61  he signal is ana
-00003a10: 6c6f 672c 0d0a 616e 6420 7468 6520 7361  log,..and the sa
-00003a20: 6d70 6c69 6e67 2072 6174 6520 6973 206c  mpling rate is l
-00003a30: 696d 6974 6564 2062 7920 7468 6520 6261  imited by the ba
-00003a40: 6e64 7769 6474 6820 6f66 2074 6865 2073  ndwidth of the s
-00003a50: 6967 6e61 6c2e 0d0a 0d0a 0d0a 2e2e 206c  ignal......... l
-00003a60: 6974 6572 616c 696e 636c 7564 653a 3a20  iteralinclude:: 
-00003a70: 2e2e 2f73 7273 6775 692f 6578 616d 706c  ../srsgui/exampl
-00003a80: 6573 2f6f 7363 696c 6c6f 7363 6f70 6520  es/oscilloscope 
-00003a90: 6578 616d 706c 652f 7461 736b 732f 666f  example/tasks/fo
-00003aa0: 7572 7468 2e70 790d 0a20 2020 203a 6c61  urth.py..    :la
-00003ab0: 6e67 7561 6765 3a20 5079 7468 6f6e 0d0a  nguage: Python..
-00003ac0: 2020 2020 3a6c 696e 656e 6f73 3a0d 0a0d      :linenos:...
-00003ad0: 0a0d 0a0d 0a2e 2e20 5f50 7956 6973 613a  ....... _PyVisa:
-00003ae0: 2068 7474 7073 3a2f 2f70 7976 6973 612e   https://pyvisa.
-00003af0: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-00003b00: 6e2f 6c61 7465 7374 2f0d 0a2e 2e20 5f73  n/latest/.... _s
-00003b10: 7273 696e 7374 2e73 7238 3630 3a20 6874  rsinst.sr860: ht
-00003b20: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
-00003b30: 726f 6a65 6374 2f73 7273 696e 7374 2e73  roject/srsinst.s
-00003b40: 7238 3630 2f0d 0a2e 2e20 5f56 5849 3131  r860/.... _VXI11
-00003b50: 3a20 6874 7470 733a 2f2f 7777 772e 6c78  : https://www.lx
-00003b60: 6973 7461 6e64 6172 642e 6f72 672f 4162  istandard.org/Ab
-00003b70: 6f75 742f 5658 492d 3131 2d61 6e64 2d4c  out/VXI-11-and-L
-00003b80: 5849 2e61 7370 780d 0a2e 2e20 5f47 5049  XI.aspx.... _GPI
-00003b90: 423a 2068 7474 7073 3a2f 2f65 6e2e 7769  B: https://en.wi
-00003ba0: 6b69 7065 6469 612e 6f72 672f 7769 6b69  kipedia.org/wiki
-00003bb0: 2f49 4545 452d 3438 380d 0a2e 2e20 5f55  /IEEE-488.... _U
-00003bc0: 5342 2d54 4d43 3a20 6874 7470 733a 2f2f  SB-TMC: https://
-00003bd0: 7777 772e 7465 7374 616e 646d 6561 7375  www.testandmeasu
-00003be0: 7265 6d65 6e74 7469 7073 2e63 6f6d 2f72  rementtips.com/r
-00003bf0: 656d 6f74 652d 636f 6d6d 756e 6963 6174  emote-communicat
-00003c00: 696f 6e2d 7769 7468 2d75 7362 746d 632d  ion-with-usbtmc-
-00003c10: 6661 712f 0d0a 2e2e 205f 5344 5331 3230  faq/.... _SDS120
-00003c20: 3258 453a 2068 7474 7073 3a2f 2f73 6967  2XE: https://sig
-00003c30: 6c65 6e74 6e61 2e63 6f6d 2f70 726f 6475  lentna.com/produ
-00003c40: 6374 2f73 6473 3132 3032 782d 652f 0d0a  ct/sds1202x-e/..
-00003c50: 2e2e 205f 5352 533a 2068 7474 7073 3a2f  .. _SRS: https:/
-00003c60: 2f74 6869 6e6b 7372 732e 636f 6d2f 0d0a  /thinksrs.com/..
-00003c70: 2e2e 205f 4347 3633 353a 2068 7474 7073  .. _CG635: https
-00003c80: 3a2f 2f74 6869 6e6b 7372 732e 636f 6d2f  ://thinksrs.com/
-00003c90: 7072 6f64 7563 7473 2f63 6736 3335 2e68  products/cg635.h
-00003ca0: 746d 6c0d 0a2e 2e20 5f6c 6f67 6769 6e67  tml.... _logging
-00003cb0: 3a20 6874 7470 733a 2f2f 646f 6373 2e70  : https://docs.p
-00003cc0: 7974 686f 6e2e 6f72 672f 332f 686f 7774  ython.org/3/howt
-00003cd0: 6f2f 6c6f 6767 696e 672e 6874 6d6c 0d0a  o/logging.html..
-00003ce0: 2e2e 205f 6d61 7470 6c6f 746c 6962 3a20  .. _matplotlib: 
-00003cf0: 6874 7470 733a 2f2f 6d61 7470 6c6f 746c  https://matplotl
-00003d00: 6962 2e6f 7267 2f73 7461 626c 652f 696e  ib.org/stable/in
-00003d10: 6465 782e 6874 6d6c                      dex.html
+00000070: 7468 6520 636f 6e73 6f6c 6520 7769 6e64  the console wind
+00000080: 6f77 2073 686f 7773 0d0a 7768 6572 6520  ow shows..where 
+00000090: 5079 7468 6f6e 2069 7320 7275 6e6e 696e  Python is runnin
+000000a0: 6720 6672 6f6d 2c20 616e 6420 7768 6572  g from, and wher
+000000b0: 6520 6060 7372 7367 7569 6060 2069 7320  e ``srsgui`` is 
+000000c0: 6c6f 6361 7465 642e 0d0a 4966 2079 6f75  located...If you
+000000d0: 2067 6f20 696e 746f 2074 6865 2064 6972   go into the dir
+000000e0: 6563 746f 7279 2077 6865 7265 2060 6073  ectory where ``s
+000000f0: 7273 6775 6960 6020 7265 7369 6465 732c  rsgui`` resides,
+00000100: 2079 6f75 2063 616e 2066 696e 640d 0a74   you can find..t
+00000110: 6865 2027 6578 616d 706c 6573 2720 6469  he 'examples' di
+00000120: 7265 6374 6f72 792e 2057 6865 6e20 796f  rectory. When yo
+00000130: 7520 6669 6e64 2061 2020 2e74 6173 6b63  u find a  .taskc
+00000140: 6f6e 6669 6720 6669 6c65 2069 6e20 226f  onfig file in "o
+00000150: 7363 696c 6c6f 7363 6f70 6520 6578 616d  scilloscope exam
+00000160: 706c 6522 0d0a 6469 7265 6374 6f72 792c  ple"..directory,
+00000170: 204f 7065 6e20 7468 6520 6669 6c65 2066   Open the file f
+00000180: 726f 6d20 7468 6520 2a2a 4669 6c65 2f4f  rom the **File/O
+00000190: 7065 6e20 436f 6e66 6967 2a2a 206d 656e  pen Config** men
+000001a0: 7520 6f66 2060 6073 7273 6775 6960 6020  u of ``srsgui`` 
+000001b0: 6170 706c 6963 6174 696f 6e2e 0d0a 4966  application...If
+000001c0: 2079 6f75 2070 6c61 6e20 746f 206d 6f64   you plan to mod
+000001d0: 6966 7920 6669 6c65 7320 696e 2074 6865  ify files in the
+000001e0: 2070 726f 6a65 6374 2c20 796f 7520 7368   project, you sh
+000001f0: 6f75 6c64 2063 6f70 7920 7468 6520 7768  ould copy the wh
+00000200: 6f6c 6520 2a2a 6578 616d 706c 6573 2a2a  ole **examples**
+00000210: 2064 6972 6563 746f 7279 0d0a 746f 2061   directory..to a
+00000220: 2073 6570 6172 6174 6520 6c6f 6361 7469   separate locati
+00000230: 6f6e 2028 6f75 7473 6964 6520 6f66 2074  on (outside of t
+00000240: 6865 2076 6972 7475 616c 2065 6e76 6972  he virtual envir
+00000250: 6f6e 6d65 6e74 206f 7220 5079 7468 6f6e  onment or Python
+00000260: 2064 6972 6563 746f 7279 3b20 0d0a 652e   directory; ..e.
+00000270: 672e 2077 6865 7265 2079 6f75 2075 7375  g. where you usu
+00000280: 616c 6c79 206b 6565 7020 796f 7572 2064  ally keep your d
+00000290: 6f63 756d 656e 7473 2066 6f72 2070 726f  ocuments for pro
+000002a0: 6772 616d 696e 6729 2e20 0d0a 5468 656e  graming). ..Then
+000002b0: 2079 6f75 2063 616e 206f 7065 6e20 616e   you can open an
+000002c0: 6420 6d6f 6469 6679 2074 6865 202e 7461  d modify the .ta
+000002d0: 736b 636f 6e66 6967 2066 696c 6520 696e  skconfig file in
+000002e0: 2074 6865 2063 6f70 6965 6420 6469 7265   the copied dire
+000002f0: 6374 6f72 790d 0a77 6974 686f 7574 2061  ctory..without a
+00000300: 6e79 2077 6f72 7279 206f 6620 636f 7272  ny worry of corr
+00000310: 7570 7469 6e67 206f 7220 6c6f 7369 6e67  upting or losing
+00000320: 2074 6865 206f 7269 6769 6e61 6c20 6669   the original fi
+00000330: 6c65 732e 0d0a 0d0a 4173 2061 6e20 6578  les.....As an ex
+00000340: 616d 706c 6520 7072 6f6a 6563 7420 666f  ample project fo
+00000350: 7220 6060 7372 7367 7569 6060 2c20 4920  r ``srsgui``, I 
+00000360: 7761 6e74 6564 2074 6f20 7573 6520 7562  wanted to use ub
+00000370: 6971 7569 746f 7573 206d 6561 7375 7265  iquitous measure
+00000380: 6d65 6e74 0d0a 696e 7374 7275 6d65 6e74  ment..instrument
+00000390: 7320 7769 7468 2072 656d 6f74 6520 636f  s with remote co
+000003a0: 6d6d 756e 6963 6174 696f 6e20 6176 6169  mmunication avai
+000003b0: 6c61 626c 652e 2049 2068 6170 7065 6e65  lable. I happene
+000003c0: 6420 746f 2068 6176 6520 616e 0d0a 6f73  d to have an..os
+000003d0: 6369 6c6c 6f73 636f 7065 2061 6e64 2061  cilloscope and a
+000003e0: 2066 756e 6374 696f 6e20 6765 6e65 7261   function genera
+000003f0: 746f 7220 286d 6f72 6520 7370 6563 6966  tor (more specif
+00000400: 6963 616c 6c79 2c20 6120 636c 6f63 6b20  ically, a clock 
+00000410: 6765 6e65 7261 746f 7229 0d0a 6f6e 206d  generator)..on m
+00000420: 7920 6465 736b 3a0d 0a0d 0a20 2020 202d  y desk:....    -
+00000430: 2053 6967 6c65 6e74 2053 4453 3132 3032   Siglent SDS1202
+00000440: 5845 5f20 6469 6769 7461 6c20 6f73 6369  XE_ digital osci
+00000450: 6c6c 6f73 636f 7065 2028 3120 4753 612f  lloscope (1 GSa/
+00000460: 732c 2032 3030 204d 487a 2062 616e 6477  s, 200 MHz bandw
+00000470: 6964 7468 292e 0d0a 2020 2020 2020 4920  idth)...      I 
+00000480: 626f 7567 6874 2069 7420 6265 6361 7573  bought it becaus
+00000490: 6520 6f66 2069 7473 2061 6666 6f72 6461  e of its afforda
+000004a0: 626c 6520 7072 6963 6520 616e 6420 6974  ble price and it
+000004b0: 2077 6f72 6b73 206e 6963 656c 7921 0d0a   works nicely!..
+000004c0: 0d0a 2020 2020 2d20 5374 616e 666f 7264  ..    - Stanford
+000004d0: 2052 6573 6561 7263 6820 5379 7374 656d   Research System
+000004e0: 7320 4347 3633 355f 2c20 3220 4748 7a20  s CG635_, 2 GHz 
+000004f0: 436c 6f63 6b20 4765 6e65 7261 746f 720d  Clock Generator.
+00000500: 0a20 2020 2020 2028 4469 7363 6c61 696d  .      (Disclaim
+00000510: 6572 3a20 4920 776f 726b 2066 6f72 2074  er: I work for t
+00000520: 6865 2063 6f6d 7061 6e79 292e 0d0a 0d0a  he company).....
+00000530: 4920 6275 696c 7420 6120 7072 6f6a 6563  I built a projec
+00000540: 7420 7468 6174 2063 6f6e 7472 6f6c 7320  t that controls 
+00000550: 626f 7468 2069 6e73 7472 756d 656e 7473  both instruments
+00000560: 2061 6e64 0d0a 6361 7074 7572 6573 206f   and..captures o
+00000570: 7574 7075 7420 7761 7665 666f 726d 2066  utput waveform f
+00000580: 726f 6d20 7468 6520 636c 6f63 6b20 6765  rom the clock ge
+00000590: 6e65 7261 746f 7220 7769 7468 2074 6865  nerator with the
+000005a0: 206f 7363 696c 6c6f 7363 6f70 652c 0d0a   oscilloscope,..
+000005b0: 6361 6c63 756c 6174 6573 2061 6e20 4646  calculates an FF
+000005c0: 542c 2061 6e64 2064 6973 706c 6179 7320  T, and displays 
+000005d0: 7468 6520 7761 7665 666f 726d 7320 696e  the waveforms in
+000005e0: 2074 6865 2060 6073 7273 6775 6960 6020   the ``srsgui`` 
+000005f0: 6170 706c 6963 6174 696f 6e2e 0d0a 0d0a  application.....
+00000600: 416e 7920 6f73 6369 6c6c 6f73 636f 7065  Any oscilloscope
+00000610: 2061 6e64 2066 756e 6374 696f 6e20 6765   and function ge
+00000620: 6e65 7261 746f 7220 7769 6c6c 2077 6f72  nerator will wor
+00000630: 6b20 666f 7220 7468 6973 2065 7861 6d70  k for this examp
+00000640: 6c65 2e0d 0a49 6620 796f 7520 6172 6520  le...If you are 
+00000650: 696e 7465 7265 7374 6564 2069 6e20 6060  interested in ``
+00000660: 7372 7367 7569 6060 2c20 6368 616e 6365  srsgui``, chance
+00000670: 7320 6172 6520 796f 7520 6361 6e20 6669  s are you can fi
+00000680: 6e64 2061 6e20 6f73 6369 6c6c 6f73 636f  nd an oscillosco
+00000690: 7065 0d0a 616e 6420 6120 6675 6e63 7469  pe..and a functi
+000006a0: 6f6e 2067 656e 6572 6174 6f72 2073 6f6d  on generator som
+000006b0: 6577 6865 7265 2069 6e20 796f 7572 2062  ewhere in your b
+000006c0: 7569 6c64 696e 672e 0d0a 0d0a 4966 2079  uilding.....If y
+000006d0: 6f75 2063 6f75 6c64 206e 6f74 2c20 646f  ou could not, do
+000006e0: 6e27 7420 776f 7272 792e 2045 7665 6e20  n't worry. Even 
+000006f0: 7769 7468 6f75 7420 616e 2061 6e79 2069  without an any i
+00000700: 6e73 7472 756d 656e 7473 2c20 7765 2063  nstruments, we c
+00000710: 616e 2067 656e 6572 6174 6520 610d 0a73  an generate a..s
+00000720: 696d 756c 6174 6564 2077 6176 6566 6f72  imulated wavefor
+00000730: 6d20 746f 2064 656d 6f6e 7374 7261 7465  m to demonstrate
+00000740: 2074 6865 2075 7361 6269 6c69 7479 206f   the usability o
+00000750: 6620 6060 7372 7367 7569 6060 2061 7320  f ``srsgui`` as 
+00000760: 616e 206f 7267 616e 697a 6572 2066 6f72  an organizer for
+00000770: 0d0a 5079 7468 6f6e 2073 6372 6970 7473  ..Python scripts
+00000780: 2061 6e64 2047 5549 2065 6e76 6972 6f6e   and GUI environ
+00000790: 6d65 6e74 2066 6f72 2063 6f6e 7665 6e69  ment for conveni
+000007a0: 656e 7420 6461 7461 2061 6371 7569 7369  ent data acquisi
+000007b0: 7469 6f6e 2061 6e64 2064 6174 6120 7669  tion and data vi
+000007c0: 7375 616c 697a 6174 696f 6e2e 0d0a 0d0a  sualization.....
+000007d0: 0d0a 4469 7265 6374 6f72 7920 7374 7275  ..Directory stru
+000007e0: 6374 7572 650d 0a2d 2d2d 2d2d 2d2d 2d2d  cture..---------
+000007f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 0d0a  ------------....
+00000800: 4c65 7427 7320 6c6f 6f6b 2061 7420 7468  Let's look at th
+00000810: 6520 6469 7265 6374 6f72 7920 7374 7275  e directory stru
+00000820: 6374 7572 6520 6f66 2074 6865 2070 726f  cture of the pro
+00000830: 6a65 6374 2e0d 0a0d 0a2e 2e20 636f 6465  ject....... code
+00000840: 2d62 6c6f 636b 3a3a 0d0a 0d0a 2020 2020  -block::....    
+00000850: 2f4f 7363 696c 6c6f 7363 6f70 6520 6578  /Oscilloscope ex
+00000860: 616d 706c 6520 7072 6f6a 6563 7420 6469  ample project di
+00000870: 7265 6374 6f72 790d 0a20 2020 2020 2020  rectory..       
+00000880: 202f 696e 7374 7275 6d65 6e74 730d 0a20   /instruments.. 
+00000890: 2020 2020 2020 2020 2020 2063 6736 3335             cg635
+000008a0: 2e70 790d 0a20 2020 2020 2020 2020 2020  .py..           
+000008b0: 2073 6473 3132 3032 2e70 790d 0a20 2020   sds1202.py..   
+000008c0: 2020 2020 202f 7461 736b 730d 0a20 2020       /tasks..   
+000008d0: 2020 2020 2020 2020 2066 6972 7374 2e70           first.p
+000008e0: 790d 0a20 2020 2020 2020 2020 2020 2073  y..            s
+000008f0: 6563 6f6e 642e 7079 0d0a 2020 2020 2020  econd.py..      
+00000900: 2020 2020 2020 2e2e 2e0d 0a0d 0a20 2020        .......   
+00000910: 2020 2020 206f 7363 696c 6c6f 7363 6f70       oscilloscop
+00000920: 6520 6578 616d 706c 6520 7072 6f6a 6563  e example projec
+00000930: 742e 7461 736b 636f 6e66 6967 0d0a 0d0a  t.taskconfig....
+00000940: 5468 6973 2066 696c 6520 7374 7275 6374  This file struct
+00000950: 7572 6520 666f 6c6c 6f77 7320 7468 6520  ure follows the 
+00000960: 6775 6964 656c 696e 6520 6465 7363 7269  guideline descri
+00000970: 6265 6420 696e 0d0a 3a72 6566 3a60 4372  bed in..:ref:`Cr
+00000980: 6561 7469 6e67 2066 696c 6520 7374 7275  eating file stru
+00000990: 6374 7572 6520 666f 7220 6120 7072 6f6a  cture for a proj
+000009a0: 6563 7460 2e0d 0a57 6520 6861 7665 2074  ect`...We have t
+000009b0: 776f 2069 6e73 7472 756d 656e 7420 6472  wo instrument dr
+000009c0: 6976 6572 2073 6372 6970 7473 2066 6f72  iver scripts for
+000009d0: 2053 4453 3132 3032 5845 5f20 616e 6420   SDS1202XE_ and 
+000009e0: 4347 3633 355f 0d0a 696e 2074 6865 2073  CG635_..in the s
+000009f0: 7562 6469 7265 6374 6f72 7920 6361 6c6c  ubdirectory call
+00000a00: 6564 202a 2a69 6e73 7472 756d 656e 7473  ed **instruments
+00000a10: 2a2a 2c20 6669 7665 2074 6173 6b20 7363  **, five task sc
+00000a20: 7269 7074 730d 0a69 6e20 7468 6520 7375  ripts..in the su
+00000a30: 6264 6972 6563 746f 7279 2063 616c 6c65  bdirectory calle
+00000a40: 6420 2a2a 7461 736b 732a 2a2c 2070 6c75  d **tasks**, plu
+00000a50: 7320 6120 636f 6e66 6967 7572 6174 696f  s a configuratio
+00000a60: 6e20 6669 6c65 0d0a 696e 2074 6865 2070  n file..in the p
+00000a70: 726f 6a65 6374 2072 6f6f 7420 6469 7265  roject root dire
+00000a80: 6374 6f72 792e 0d0a 0d0a 5072 6f6a 6563  ctory.....Projec
+00000a90: 7420 636f 6e66 6967 7572 6174 696f 6e20  t configuration 
+00000aa0: 6669 6c65 0d0a 2d2d 2d2d 2d2d 2d2d 2d2d  file..----------
+00000ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000ac0: 2d2d 2d0d 0a0d 0a54 6865 2073 7472 7563  ---....The struc
+00000ad0: 7475 7265 206f 6620 6120 2e74 6173 6b63  ture of a .taskc
+00000ae0: 6f6e 6669 6720 6669 6c65 2069 7320 7369  onfig file is si
+00000af0: 6d70 6c65 2061 6e64 0d0a 6578 706c 6169  mple and..explai
+00000b00: 6e65 6420 696e 203a 7265 663a 6050 6f70  ned in :ref:`Pop
+00000b10: 756c 6174 696e 6720 7468 6520 2e74 6173  ulating the .tas
+00000b20: 6b63 6f6e 6669 6720 6669 6c65 600d 0a0d  kconfig file`...
+00000b30: 0a2e 2e20 636f 6465 2d62 6c6f 636b 3a3a  ... code-block::
+00000b40: 0d0a 2020 2020 3a6c 696e 656e 6f73 3a0d  ..    :linenos:.
+00000b50: 0a0d 0a20 2020 206e 616d 653a 2053 7273  ...    name: Srs
+00000b60: 6775 6920 4578 616d 706c 6520 2d20 4f73  gui Example - Os
+00000b70: 6369 6c6c 6f73 636f 7065 2061 6e64 2043  cilloscope and C
+00000b80: 6c6f 636b 2047 656e 6572 6174 6f72 0d0a  lock Generator..
+00000b90: 0d0a 2020 2020 696e 7374 3a20 6367 2c20  ..    inst: cg, 
+00000ba0: 2069 6e73 7472 756d 656e 7473 2e63 6736   instruments.cg6
+00000bb0: 3335 2c20 2020 4347 3633 350d 0a20 2020  35,   CG635..   
+00000bc0: 2069 6e73 743a 206f 7363 2c20 696e 7374   inst: osc, inst
+00000bd0: 7275 6d65 6e74 732e 7364 7331 3230 322c  ruments.sds1202,
+00000be0: 2053 4453 3132 3032 0d0a 0d0a 2020 2020   SDS1202....    
+00000bf0: 7461 736b 3a20 2a49 444e 2074 6573 742c  task: *IDN test,
+00000c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c10: 2074 6173 6b73 2e66 6972 7374 2c20 2046   tasks.first,  F
+00000c20: 6972 7374 5461 736b 0d0a 2020 2020 7461  irstTask..    ta
+00000c30: 736b 3a20 506c 6f74 2065 7861 6d70 6c65  sk: Plot example
+00000c40: 2c20 2020 2020 2020 2020 2020 2020 2074  ,              t
+00000c50: 6173 6b73 2e73 6563 6f6e 642c 2053 6563  asks.second, Sec
+00000c60: 6f6e 6454 6173 6b0d 0a20 2020 202e 2e2e  ondTask..    ...
+00000c70: 0d0a 0d0a 496e 7374 7275 6d65 6e74 2064  ....Instrument d
+00000c80: 7269 7665 7273 0d0a 2d2d 2d2d 2d2d 2d2d  rivers..--------
+00000c90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 0d0a  ------------....
+00000ca0: 4347 3633 350d 0a5e 5e5e 5e5e 0d0a 0d0a  CG635..^^^^^....
+00000cb0: 4c65 7427 7320 7461 6b65 2061 206c 6f6f  Let's take a loo
+00000cc0: 6b20 696e 746f 2074 6865 2060 696e 7374  k into the `inst
+00000cd0: 7275 6d65 6e74 732f 6367 3633 352e 7079  ruments/cg635.py
+00000ce0: 6020 6d6f 6475 6c65 2e20 4576 656e 2074  ` module. Even t
+00000cf0: 686f 7567 6820 6974 2073 6565 6d73 206c  hough it seems l
+00000d00: 6f6e 672c 0d0a 6974 2068 6173 206f 6e6c  ong,..it has onl
+00000d10: 7920 3520 6c69 6e65 7320 6f66 206e 6f6e  y 5 lines of non
+00000d20: 2d63 6f6d 6d65 6e74 2063 6f64 652e 2049  -comment code. I
+00000d30: 6620 796f 7520 6861 7665 2061 2043 4736  f you have a CG6
+00000d40: 3335 2c0d 0a63 6f6e 6772 6174 756c 6174  35,..congratulat
+00000d50: 696f 6e73 2120 596f 7520 6361 6e20 7573  ions! You can us
+00000d60: 6520 7468 6520 6669 6c65 2061 7320 6973  e the file as is
+00000d70: 2e20 4966 2079 6f75 2068 6176 6520 616e  . If you have an
+00000d80: 7920 6675 6e63 7469 6f6e 0d0a 6765 6e65  y function..gene
+00000d90: 7261 746f 7220 7468 6174 2063 616e 2063  rator that can c
+00000da0: 6861 6e67 6520 7468 6520 6f75 7470 7574  hange the output
+00000db0: 2066 7265 7175 656e 6379 2c20 796f 7520   frequency, you 
+00000dc0: 6361 6e20 7573 6520 6974 2069 6e73 7465  can use it inste
+00000dd0: 6164 206f 6620 7468 6520 4347 3633 350d  ad of the CG635.
+00000de0: 0a69 6e20 7468 6520 6578 616d 706c 652e  .in the example.
+00000df0: 2059 6f75 2063 6861 6e67 6520 7468 6520   You change the 
+00000e00: 636c 6173 7320 6e61 6d65 2061 6e64 205f  class name and _
+00000e10: 4964 5374 7269 6e67 2074 6f20 6d61 7463  IdString to matc
+00000e20: 6820 7468 6520 696e 7374 7275 6d65 6e74  h the instrument
+00000e30: 206e 616d 652c 0d0a 616c 6f6e 6720 7769   name,..along wi
+00000e40: 7468 205f 7465 726d 5f63 6861 722e 204c  th _term_char. L
+00000e50: 6f6f 6b20 7570 2074 6865 2063 6f6d 6d61  ook up the comma
+00000e60: 6e64 2074 6f20 6368 616e 6765 2066 7265  nd to change fre
+00000e70: 7175 656e 6379 2c20 7265 6665 7272 696e  quency, referrin
+00000e80: 6720 746f 2074 6865 206d 616e 7561 6c2e  g to the manual.
+00000e90: 0d0a 5361 7665 2074 6865 202e 7079 2066  ..Save the .py f
+00000ea0: 696c 6520 7769 7468 2061 2028 6469 6666  ile with a (diff
+00000eb0: 6572 656e 7429 2061 7070 726f 7072 6961  erent) appropria
+00000ec0: 7465 2066 696c 656e 616d 652e 2043 6861  te filename. Cha
+00000ed0: 6e67 6520 7468 6520 6069 6e73 743a 6020  nge the `inst:` 
+00000ee0: 6c69 6e65 2066 6f72 2060 6367 600d 0a69  line for `cg`..i
+00000ef0: 6e20 7468 6520 2e74 6173 6b63 6f6e 6669  n the .taskconfi
+00000f00: 6720 6669 6c65 2074 6f20 6d61 7463 6820  g file to match 
+00000f10: 7468 6520 6d6f 6475 6c65 2070 6174 6820  the module path 
+00000f20: 616e 6420 7468 6520 636c 6173 7320 6e61  and the class na
+00000f30: 6d65 2074 6861 7420 796f 7520 6372 6561  me that you crea
+00000f40: 7465 642e 0d0a 0d0a 2e2e 2063 6f64 652d  ted....... code-
+00000f50: 626c 6f63 6b3a 3a0d 0a20 2020 203a 6c69  block::..    :li
+00000f60: 6e65 6e6f 733a 0d0a 0d0a 2020 2020 6672  nenos:....    fr
+00000f70: 6f6d 2073 7273 6775 6920 696d 706f 7274  om srsgui import
+00000f80: 2049 6e73 7472 756d 656e 740d 0a20 2020   Instrument..   
+00000f90: 2066 726f 6d20 7372 7367 7569 2e69 6e73   from srsgui.ins
+00000fa0: 7420 696d 706f 7274 2046 6c6f 6174 436f  t import FloatCo
+00000fb0: 6d6d 616e 640d 0a0d 0a20 2020 2063 6c61  mmand....    cla
+00000fc0: 7373 2043 4736 3335 2849 6e73 7472 756d  ss CG635(Instrum
+00000fd0: 656e 7429 3a0d 0a20 2020 2020 2020 205f  ent):..        _
+00000fe0: 4964 5374 7269 6e67 203d 2027 4347 3633  IdString = 'CG63
+00000ff0: 3527 0d0a 2020 2020 2020 2020 6672 6571  5'..        freq
+00001000: 7565 6e63 7920 3d20 466c 6f61 7443 6f6d  uency = FloatCom
+00001010: 6d61 6e64 2827 4652 4551 2729 0d0a 0d0a  mand('FREQ')....
+00001020: 5769 7468 6f75 7420 7265 6465 6669 6e69  Without redefini
+00001030: 6e67 202a 2a61 7661 696c 6162 6c65 5f69  ng **available_i
+00001040: 6e74 6572 6661 6365 732a 2a20 636c 6173  nterfaces** clas
+00001050: 7320 6174 7472 6962 7574 652c 2079 6f75  s attribute, you
+00001060: 2063 616e 2075 7365 2073 6572 6961 6c0d   can use serial.
+00001070: 0a63 6f6d 6d75 6e69 6361 7469 6f6e 206f  .communication o
+00001080: 6e6c 792e 2049 6620 796f 7520 7761 6e74  nly. If you want
+00001090: 2074 6f20 7573 6520 4750 4942 2063 6f6d   to use GPIB com
+000010a0: 6d75 6e69 6361 7469 6f6e 2c20 796f 7520  munication, you 
+000010b0: 6861 7665 2074 6f20 756e 2d63 6f6d 6d65  have to un-comme
+000010c0: 6e74 2074 6865 0d0a 2a2a 6176 6169 6c61  nt the..**availa
+000010d0: 626c 655f 696e 7465 7266 6163 6573 2a2a  ble_interfaces**
+000010e0: 2069 6e20 4347 3633 3520 636c 6173 732e   in CG635 class.
+000010f0: 0d0a 0d0a 2e2e 2063 6f64 652d 626c 6f63  ...... code-bloc
+00001100: 6b3a 3a0d 0a0d 0a20 2020 2066 726f 6d20  k::....    from 
+00001110: 7372 7367 7569 2069 6d70 6f72 7420 5365  srsgui import Se
+00001120: 7269 616c 496e 7465 7266 6163 652c 2046  rialInterface, F
+00001130: 696e 644c 6973 7449 6e70 7574 0d0a 2020  indListInput..  
+00001140: 2020 6672 6f6d 2073 7273 696e 7374 2e73    from srsinst.s
+00001150: 7238 3630 2069 6d70 6f72 7420 5669 7361  r860 import Visa
+00001160: 496e 7465 7266 6163 650d 0a0d 0a20 2020  Interface....   
+00001170: 2061 7661 696c 6162 6c65 5f69 6e74 6572   available_inter
+00001180: 6661 6365 7320 3d20 5b0d 0a20 2020 2020  faces = [..     
+00001190: 2020 205b 2020 2053 6572 6961 6c49 6e74     [   SerialInt
+000011a0: 6572 6661 6365 2c0d 0a20 2020 2020 2020  erface,..       
+000011b0: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
+000011c0: 2020 2020 2020 2020 2743 4f4d 2070 6f72          'COM por
+000011d0: 7427 3a20 4669 6e64 4c69 7374 496e 7075  t': FindListInpu
+000011e0: 7428 292c 0d0a 2020 2020 2020 2020 2020  t(),..          
+000011f0: 2020 2020 2020 2762 6175 6420 7261 7465        'baud rate
+00001200: 273a 2039 3630 300d 0a20 2020 2020 2020  ': 9600..       
+00001210: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
+00001220: 5d2c 0d0a 2020 2020 2020 2020 5b20 2020  ],..        [   
+00001230: 5669 7361 496e 7465 7266 6163 652c 0d0a  VisaInterface,..
+00001240: 2020 2020 2020 2020 2020 2020 7b0d 0a20              {.. 
+00001250: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00001260: 7265 736f 7572 6365 273a 2046 696e 644c  resource': FindL
+00001270: 6973 7449 6e70 7574 2829 2c0d 0a20 2020  istInput(),..   
+00001280: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
+00001290: 2020 2020 5d2c 0d0a 2020 2020 5d0d 0a0d      ],..    ]...
+000012a0: 0a59 6f75 206d 7573 7420 696e 7374 616c  .You must instal
+000012b0: 6c20 6073 7273 696e 7374 2e73 7238 3630  l `srsinst.sr860
+000012c0: 605f 2066 6f72 2056 6973 6149 6e74 6572  `_ for VisaInter
+000012d0: 6661 6365 2063 6c61 7373 2c20 616e 6420  face class, and 
+000012e0: 5079 5649 5341 5f20 616e 640d 0a69 7473  PyVISA_ and..its
+000012f0: 2062 6163 6b65 6e64 206c 6962 7261 7279   backend library
+00001300: 2c20 666f 6c6c 6f77 696e 6720 5079 5669  , following PyVi
+00001310: 7361 2069 6e73 7461 6c6c 6174 696f 6e20  sa installation 
+00001320: 696e 7374 7275 6374 696f 6e2e 0d0a 0d0a  instruction.....
+00001330: 4f6e 6365 2074 6865 2043 4736 3335 2028  Once the CG635 (
+00001340: 6f72 2079 6f75 7220 6675 6e63 7469 6f6e  or your function
+00001350: 2067 656e 6572 6174 6f72 2920 6973 2063   generator) is c
+00001360: 6f6e 6e65 6374 6564 2c20 0d0a 796f 7520  onnected, ..you 
+00001370: 7769 6c6c 2073 6565 2074 6865 2063 6f6e  will see the con
+00001380: 6e65 6374 696f 6e20 696e 666f 726d 6174  nection informat
+00001390: 696f 6e20 696e 2074 6865 2069 6e73 7472  ion in the instr
+000013a0: 756d 656e 7420 696e 666f 2070 616e 656c  ument info panel
+000013b0: 2c0d 0a61 6e64 2079 6f75 2063 616e 2075  ,..and you can u
+000013c0: 7365 2069 7420 696e 2074 6865 2074 6572  se it in the ter
+000013d0: 6d69 6e61 6c2c 2061 7320 7368 6f77 6e20  minal, as shown 
+000013e0: 6265 6c6f 772e 0d0a 0d0a 2e2e 2066 6967  below....... fig
+000013f0: 7572 653a 3a20 2e2f 5f73 7461 7469 632f  ure:: ./_static/
+00001400: 6367 2d74 6572 6d69 6e61 6c2d 7363 7265  cg-terminal-scre
+00001410: 656e 2d63 6170 7475 7265 2e70 6e67 0d0a  en-capture.png..
+00001420: 2020 2020 3a61 6c69 676e 3a20 6365 6e74      :align: cent
+00001430: 6572 0d0a 2020 2020 3a66 6967 636c 6173  er..    :figclas
+00001440: 733a 2061 6c69 676e 2d63 656e 7465 720d  s: align-center.
+00001450: 0a0d 0a7c 0d0a 0d0a 546f 2066 6978 2074  ...|....To fix t
+00001460: 6865 2027 4e6f 7420 696d 706c 656d 656e  he 'Not implemen
+00001470: 7465 6427 2077 6172 6e69 6e67 2c0d 0a3a  ted' warning,..:
+00001480: 6d65 7468 3a60 496e 7374 7275 6d65 6e74  meth:`Instrument
+00001490: 2e67 6574 5f73 7461 7475 7328 2920 3c73  .get_status() <s
+000014a0: 7273 6775 692e 696e 7374 2e69 6e73 7472  rsgui.inst.instr
+000014b0: 756d 656e 742e 496e 7374 7275 6d65 6e74  ument.Instrument
+000014c0: 2e67 6574 5f73 7461 7475 733e 600d 0a6e  .get_status>`..n
+000014d0: 6565 6473 2074 6f20 6265 2072 6564 6566  eeds to be redef
+000014e0: 696e 6564 2e20 0d0a 466f 7220 6578 616d  ined. ..For exam
+000014f0: 706c 652c 2077 6520 6361 6e20 6f76 6572  ple, we can over
+00001500: 7269 6465 2069 7420 6173 2066 6f6c 6c6f  ride it as follo
+00001510: 7769 6e67 3a0d 0a0d 0a2e 2e20 636f 6465  wing:...... code
+00001520: 2d62 6c6f 636b 3a3a 0d0a 0d0a 2020 2020  -block::....    
+00001530: 6465 6620 6765 745f 7374 6174 7573 2873  def get_status(s
+00001540: 656c 6629 3a0d 0a20 2020 2020 2020 2072  elf):..        r
+00001550: 6574 7572 6e20 2753 7461 7475 733a 204f  eturn 'Status: O
+00001560: 4b27 0d0a 0d0a 2849 6620 796f 7520 6172  K'....(If you ar
+00001570: 6520 6661 6d69 6c69 6172 2077 6974 6820  e familiar with 
+00001580: 7374 6174 7573 2062 7974 6573 2c20 796f  status bytes, yo
+00001590: 7520 6361 6e20 6f76 6572 7269 6465 2074  u can override t
+000015a0: 6865 2060 6765 745f 7374 6174 7573 6020  he `get_status` 
+000015b0: 6d65 7468 6f64 0d0a 746f 2071 7565 7279  method..to query
+000015c0: 2074 6865 2073 7461 7475 7320 6279 7465   the status byte
+000015d0: 2873 2920 616e 6420 7265 7475 726e 2074  (s) and return t
+000015e0: 6865 2072 656c 6576 616e 7420 7374 6174  he relevant stat
+000015f0: 7573 2069 6e66 6f72 6d61 7469 6f6e 2061  us information a
+00001600: 7320 796f 7520 6465 7369 7265 2e29 0d0a  s you desire.)..
+00001610: 0d0a 5765 2077 696c 6c20 7573 6520 6f6e  ..We will use on
+00001620: 6c79 206f 6e65 2063 6f6d 6d61 6e64 205c  ly one command \
+00001630: 2e66 7265 7175 656e 6379 2c20 6f72 2069  .frequency, or i
+00001640: 7473 2072 6177 2072 656d 6f74 6520 636f  ts raw remote co
+00001650: 6d6d 616e 642c 2027 6672 6571 2720 696e  mmand, 'freq' in
+00001660: 2074 6869 7320 6578 616d 706c 652e 0d0a   this example...
+00001670: 4265 6361 7573 6520 2763 6727 2069 7320  Because 'cg' is 
+00001680: 7468 6520 6465 6661 756c 7420 696e 7374  the default inst
+00001690: 7275 6d65 6e74 2028 7468 6520 6669 7273  rument (the firs
+000016a0: 7420 696e 7374 7275 6d65 6e74 206d 656e  t instrument men
+000016b0: 7469 6f6e 6564 2069 6e20 7468 6520 2e74  tioned in the .t
+000016c0: 6173 6b63 6f6e 6669 6720 6669 6c65 292c  askconfig file),
+000016d0: 0d0a 616e 7920 7261 7720 7265 6d6f 7465  ..any raw remote
+000016e0: 2063 6f6d 6d61 6e64 2077 6974 686f 7574   command without
+000016f0: 2074 6865 2027 6367 3a27 2070 7265 6669   the 'cg:' prefi
+00001700: 7820 7769 6c6c 2062 6520 7365 6e74 2074  x will be sent t
+00001710: 6f20 6974 2e0d 0a42 6f74 6820 275c 2a69  o it...Both '\*i
+00001720: 646e 3f27 2061 6e64 2027 6367 3a5c 2a69  dn?' and 'cg:\*i
+00001730: 646e 3f27 2077 696c 6c20 7265 7475 726e  dn?' will return
+00001740: 2074 6865 2073 616d 6520 7265 706c 792e   the same reply.
+00001750: 0d0a 0d0a 5765 2075 7365 2074 6865 2070  ....We use the p
+00001760: 7265 6669 7820 2763 673a 2720 666f 7220  refix 'cg:' for 
+00001770: 7261 7720 7265 6d6f 7465 2063 6f6d 6d61  raw remote comma
+00001780: 6e64 2061 6e64 2074 6865 2070 7265 6669  nd and the prefi
+00001790: 7820 2763 672e 2720 666f 7220 5079 7468  x 'cg.' for Pyth
+000017a0: 6f6e 2063 6f6d 6d61 6e64 732e 0d0a 496e  on commands...In
+000017b0: 2074 6865 2074 6572 6d69 6e61 6c20 616c   the terminal al
+000017c0: 6c20 6174 7472 6962 7574 6573 2061 6e64  l attributes and
+000017d0: 206d 6574 686f 6473 206f 6620 4347 3833   methods of CG83
+000017e0: 3520 636c 6173 7320 6361 6e20 6265 2075  5 class can be u
+000017f0: 7365 6420 7769 7468 2070 7265 6669 7820  sed with prefix 
+00001800: 2763 672e 272e 0d0a 4265 6361 7573 6520  'cg.'...Because 
+00001810: 7765 2064 6566 696e 6564 2066 7265 7175  we defined frequ
+00001820: 656e 6379 2061 7320 6120 466c 6f61 7443  ency as a FloatC
+00001830: 6f6d 6d61 6e64 2c20 7765 2063 616e 2061  ommand, we can a
+00001840: 6c73 6f20 7573 6520 7468 6520 2763 672e  lso use the 'cg.
+00001850: 6672 6571 7565 6e63 7927 2070 726f 7065  frequency' prope
+00001860: 7274 7920 696e 2074 6865 0d0a 7465 726d  rty in the..term
+00001870: 696e 616c 2e20 5468 6973 206d 6561 6e73  inal. This means
+00001880: 2074 6861 7420 7468 6520 666f 6c6c 6f77   that the follow
+00001890: 696e 6720 6172 6520 6571 7569 7661 6c65  ing are equivale
+000018a0: 6e74 3a0d 0a2d 2060 6367 3a66 7265 7120  nt:..- `cg:freq 
+000018b0: 3130 302e 3060 0d0a 2d20 6063 672e 6672  100.0`..- `cg.fr
+000018c0: 6571 7565 6e63 7920 3130 3060 0d0a 2020  equency 100`..  
+000018d0: 0d0a 4675 7274 6865 726d 6f72 652c 2066  ..Furthermore, f
+000018e0: 726f 6d20 6120 5079 7468 6f6e 2073 6372  rom a Python scr
+000018f0: 6970 742c 206f 6e63 6520 6067 6574 5f69  ipt, once `get_i
+00001900: 6e73 7472 756d 656e 7428 2763 6727 2960  nstrument('cg')`
+00001910: 2068 6173 2062 6565 6e20 6361 6c6c 6564   has been called
+00001920: 2069 6e20 6120 7461 736b 2063 6c61 7373   in a task class
+00001930: 2c0d 0a79 6f75 2063 616e 2075 7365 2060  ,..you can use `
+00001940: 6367 2e66 7265 7175 656e 6379 203d 2031  cg.frequency = 1
+00001950: 3030 6020 696e 2074 6865 2050 7974 686f  00` in the Pytho
+00001960: 6e20 7461 736b 2063 6f64 6520 286f 7220  n task code (or 
+00001970: 6063 672e 6672 6571 7565 6e63 7960 2061  `cg.frequency` a
+00001980: 7320 7468 6520 7175 6572 7920 666f 726d  s the query form
+00001990: 292e 0d0a 0d0a 4163 7475 616c 6c79 2079  ).....Actually y
+000019a0: 6f75 2063 616e 2075 7365 2061 6c6c 2074  ou can use all t
+000019b0: 6865 2061 7474 7269 6275 7465 7320 616e  he attributes an
+000019c0: 6420 6d65 7468 6f64 7320 6465 6669 6e65  d methods define
+000019d0: 6420 696e 2074 6865 2043 4736 3335 2063  d in the CG635 c
+000019e0: 6c61 7373 2061 6e64 2069 7473 2073 7570  lass and its sup
+000019f0: 6572 2063 6c61 7373 6573 2e0d 0a54 6865  er classes...The
+00001a00: 2060 6367 2e64 6972 2829 6020 6d65 7468   `cg.dir()` meth
+00001a10: 6f64 2028 7768 6572 6520 6064 6972 2829  od (where `dir()
+00001a20: 6020 6973 2064 6566 696e 6564 2069 6e20  ` is defined in 
+00001a30: 3a63 6c61 7373 3a60 436f 6d70 6f6e 656e  :class:`Componen
+00001a40: 7420 3c73 7273 6775 692e 696e 7374 2e63  t <srsgui.inst.c
+00001a50: 6f6d 706f 6e65 6e74 2e43 6f6d 706f 6e65  omponent.Compone
+00001a60: 6e74 3e60 2063 6c61 7373 290d 0a73 686f  nt>` class)..sho
+00001a70: 7773 2061 6c6c 2074 6865 2061 7661 696c  ws all the avail
+00001a80: 6162 6c65 2063 6f6d 706f 6e65 6e74 732c  able components,
+00001a90: 2063 6f6d 6d61 6e64 732c 2061 6e64 206d   commands, and m
+00001aa0: 6574 686f 6473 2061 7661 696c 6162 6c65  ethods available
+00001ab0: 2074 6f20 616e 2069 6e73 7461 6e63 6520   to an instance 
+00001ac0: 6f66 2074 6865 2043 4736 3335 2063 6c61  of the CG635 cla
+00001ad0: 7373 2e20 0d0a 5468 6973 2068 656c 7073  ss. ..This helps
+00001ae0: 2075 7320 746f 206e 6176 6967 6174 6520   us to navigate 
+00001af0: 7468 726f 7567 6820 7265 736f 7572 6365  through resource
+00001b00: 7320 6176 6169 6c61 626c 6520 7769 7468  s available with
+00001b10: 2074 6865 2063 6c61 7373 2e0d 0a0d 0a2e   the class......
+00001b20: 2e20 6669 6775 7265 3a3a 202e 2f5f 7374  . figure:: ./_st
+00001b30: 6174 6963 2f63 672d 6469 722d 7465 726d  atic/cg-dir-term
+00001b40: 696e 616c 2d73 6372 6565 6e2d 6361 7074  inal-screen-capt
+00001b50: 7572 652e 706e 670d 0a20 2020 203a 616c  ure.png..    :al
+00001b60: 6967 6e3a 2063 656e 7465 720d 0a20 2020  ign: center..   
+00001b70: 203a 6669 6763 6c61 7373 3a20 616c 6967   :figclass: alig
+00001b80: 6e2d 6365 6e74 6572 0d0a 0d0a 0d0a 4372  n-center......Cr
+00001b90: 6163 6b69 6e67 206f 7065 6e20 7468 6520  acking open the 
+00001ba0: 696e 7374 7275 6d65 6e74 206d 616e 7561  instrument manua
+00001bb0: 6c20 616e 6420 6465 6669 6e69 6e67 2075  l and defining u
+00001bc0: 7365 6675 6c20 6d65 7468 6f64 7320 696e  seful methods in
+00001bd0: 2061 6e20 696e 7374 7275 6d65 6e74 2063   an instrument c
+00001be0: 6c61 7373 200d 0a70 726f 7669 6465 7320  lass ..provides 
+00001bf0: 6561 7365 206f 6620 696e 7374 7275 6d65  ease of instrume
+00001c00: 6e74 2063 6f6e 7472 6f6c 2066 726f 6d20  nt control from 
+00001c10: 6569 7468 6572 2074 6865 2054 6572 6d69  either the Termi
+00001c20: 6e61 6c20 6f72 2066 726f 6d20 796f 7572  nal or from your
+00001c30: 2074 6173 6b20 636f 6465 2c20 0d0a 7769   task code, ..wi
+00001c40: 7468 6f75 7420 6861 7669 6e67 2074 6f20  thout having to 
+00001c50: 7265 6d65 6d62 6572 2074 6865 2072 656d  remember the rem
+00001c60: 6f74 6520 636f 6d6d 616e 6420 6d6e 656d  ote command mnem
+00001c70: 6f6e 6963 7320 7468 656d 7365 6c76 6573  onics themselves
+00001c80: 2e20 0d0a 0d0a 5344 5331 3230 320d 0a5e  . ....SDS1202..^
+00001c90: 5e5e 5e5e 5e5e 0d0a 0d0a 4576 656e 2074  ^^^^^^....Even t
+00001ca0: 686f 7567 6820 796f 7520 6d61 7920 6e6f  hough you may no
+00001cb0: 7420 6861 7665 2061 6e20 5344 5331 3230  t have an SDS120
+00001cc0: 3220 6f73 6369 6c6c 6f73 636f 7065 2074  2 oscilloscope t
+00001cd0: 6861 7420 4920 6861 7070 656e 6564 0d0a  hat I happened..
+00001ce0: 746f 2075 7365 2066 6f72 2074 6869 7320  to use for this 
+00001cf0: 6578 616d 706c 652c 2049 2062 6574 2079  example, I bet y
+00001d00: 6f75 2063 616e 2066 696e 6420 616e 206f  ou can find an o
+00001d10: 7363 696c 6c6f 7363 6f70 6520 736f 6d65  scilloscope some
+00001d20: 7768 6572 650d 0a69 6e20 796f 7572 2062  where..in your b
+00001d30: 7569 6c64 696e 672e 2057 6865 6e20 796f  uilding. When yo
+00001d40: 7520 6765 7420 6120 686f 6c64 206f 6620  u get a hold of 
+00001d50: 6f6e 652c 2069 7420 6d61 7920 6861 7665  one, it may have
+00001d60: 2061 2055 5342 2063 6f6e 6e65 6374 6f72   a USB connector
+00001d70: 206f 6e6c 792c 0d0a 6c69 6b65 2061 206c   only,..like a l
+00001d80: 6f74 206f 6620 6261 7365 206d 6f64 656c  ot of base model
+00001d90: 206f 7363 696c 6c6f 7363 6f70 6573 2064   oscilloscopes d
+00001da0: 6f2e 0d0a 5468 6973 206d 6561 6e73 2079  o...This means y
+00001db0: 6f75 206d 6179 2068 6176 6520 746f 2075  ou may have to u
+00001dc0: 7365 2055 5342 2d54 4d43 2069 6e74 6572  se USB-TMC inter
+00001dd0: 6661 6365 2e20 0d0a 496e 206f 7264 6572  face. ..In order
+00001de0: 2074 6f20 646f 2074 6861 742c 2079 6f75   to do that, you
+00001df0: 206e 6565 6420 746f 2069 6e73 7461 6c6c   need to install
+00001e00: 2050 7956 4953 412e 200d 0a59 6f75 206e   PyVISA. ..You n
+00001e10: 6565 6420 746f 2075 6e63 6f6d 6d65 6e74  eed to uncomment
+00001e20: 2074 6865 2061 7661 696c 6162 6c65 5f69   the available_i
+00001e30: 6e74 6572 6661 6365 7320 6f66 2053 4453  nterfaces of SDS
+00001e40: 3132 3032 2063 6c61 7373 2c20 0d0a 6d6f  1202 class, ..mo
+00001e50: 6469 6679 2069 7420 746f 2066 6974 2074  dify it to fit t
+00001e60: 6865 2073 7065 6369 6669 6361 7469 6f6e  he specification
+00001e70: 206f 6620 796f 7572 206f 7363 696c 6c6f   of your oscillo
+00001e80: 7363 6f70 652c 2061 6c6f 6e67 2077 6974  scope, along wit
+00001e90: 680d 0a63 6861 6e67 696e 6720 746f 2074  h..changing to t
+00001ea0: 6865 2063 6f72 7265 6374 2060 5f49 6453  he correct `_IdS
+00001eb0: 7472 696e 6760 2e20 0d0a 5468 656e 2079  tring`. ..Then y
+00001ec0: 6f75 2068 6176 6520 746f 2067 6574 2077  ou have to get w
+00001ed0: 6176 6566 6f72 6d20 646f 776e 6c6f 6164  aveform download
+00001ee0: 2077 6f72 6b69 6e67 2c20 7768 6963 6820   working, which 
+00001ef0: 6f66 7465 6e20 696e 766f 6c76 6573 2072  often involves r
+00001f00: 6563 6965 7669 6e67 2061 6e64 2070 726f  ecieving and pro
+00001f10: 7065 726c 7920 7061 7273 696e 6720 6269  perly parsing bi
+00001f20: 6e61 7279 2064 6174 610d 0a28 6269 6e61  nary data..(bina
+00001f30: 7279 2064 6174 6120 6973 2075 7365 6420  ry data is used 
+00001f40: 746f 206d 696e 696d 697a 6520 7468 6520  to minimize the 
+00001f50: 6e75 6d62 6572 206f 6620 6368 6172 6163  number of charac
+00001f60: 7465 7273 2073 656e 7420 6f76 6572 2074  ters sent over t
+00001f70: 6865 2072 656d 6f74 6520 636f 6d6d 756e  he remote commun
+00001f80: 6963 6174 696f 6e20 696e 7465 7266 6163  ication interfac
+00001f90: 652c 0d0a 7468 6572 6562 7920 6d61 6b69  e,..thereby maki
+00001fa0: 6e67 2064 6174 6120 7472 616e 7366 6572  ng data transfer
+00001fb0: 7320 6f66 2070 6572 6861 7073 2076 6572  s of perhaps ver
+00001fc0: 7920 6c65 6e67 7468 7920 7761 7665 666f  y lengthy wavefo
+00001fd0: 726d 7320 7265 6c61 7469 7665 6c79 2066  rms relatively f
+00001fe0: 6173 7429 2e0d 0a49 6620 796f 7520 6172  ast)...If you ar
+00001ff0: 6520 6c75 636b 792c 2079 6f75 2063 616e  e lucky, you can
+00002000: 2066 696e 6420 6120 776f 726b 696e 6720   find a working 
+00002010: 5079 7468 6f6e 2073 6e69 7070 6574 2066  Python snippet f
+00002020: 726f 6d20 6a75 6469 6369 6f75 7320 7765  rom judicious we
+00002030: 6220 7365 6172 6368 2e0d 0a49 6620 6e6f  b search...If no
+00002040: 742c 2079 6f75 2068 6176 6520 746f 2064  t, you have to d
+00002050: 6563 6970 6865 7220 7468 6520 7072 6f67  ecipher the prog
+00002060: 7261 6d6d 696e 6720 6d61 6e75 616c 206f  ramming manual o
+00002070: 6620 7468 6520 6f73 6369 6c6c 6f73 636f  f the oscillosco
+00002080: 7065 2e20 0d0a 4974 206d 6179 2074 616b  pe. ..It may tak
+00002090: 6520 7469 6d65 2c20 6275 7420 6974 2077  e time, but it w
+000020a0: 696c 6c20 6265 2076 6572 7920 7265 7761  ill be very rewa
+000020b0: 7264 696e 6720 666f 7220 796f 7572 2064  rding for your d
+000020c0: 6174 6120 6163 7175 6973 6974 696f 6e0d  ata acquisition.
+000020d0: 0a73 6b69 6c6c 2d73 6574 2069 6d70 726f  .skill-set impro
+000020e0: 7665 6d65 6e74 2e0d 0a0d 0a4f 7468 6572  vement.....Other
+000020f0: 2074 6861 6e20 7468 6520 6269 6e61 7279   than the binary
+00002100: 2077 6176 6566 6f72 6d20 646f 776e 6c6f   waveform downlo
+00002110: 6164 2c20 0d0a 6d6f 7374 206f 7468 6572  ad, ..most other
+00002120: 2063 6f6d 6d61 6e64 7320 666f 7220 696e   commands for in
+00002130: 7465 7261 6374 696e 6720 7769 7468 2074  teracting with t
+00002140: 6865 206f 7363 696c 6c6f 7363 6f70 6520  he oscilloscope 
+00002150: 0d0a 7769 6c6c 2062 6520 7374 616e 6461  ..will be standa
+00002160: 7264 2041 5343 4949 2d62 6173 6564 2074  rd ASCII-based t
+00002170: 6578 7420 636f 6d6d 616e 6473 2e0d 0a0d  ext commands....
+00002180: 0a2e 2e20 6e6f 7465 3a3a 0d0a 2020 5769  ... note::..  Wi
+00002190: 7468 2064 6566 6175 6c74 2061 7661 696c  th default avail
+000021a0: 6162 6c65 5f69 6e74 6572 6661 6365 7320  able_interfaces 
+000021b0: 6f66 2049 6e73 7472 756d 656e 7420 636c  of Instrument cl
+000021c0: 6173 732c 2054 6370 6970 496e 7465 7266  ass, TcpipInterf
+000021d0: 6163 6520 7368 6f75 6c64 2062 6520 7573  ace should be us
+000021e0: 6564 2077 6974 6820 706f 7274 2035 3032  ed with port 502
+000021f0: 352e 0d0a 0d0a 5468 6520 696e 7374 7275  5.....The instru
+00002200: 6d65 6e74 2064 7269 7665 7220 666f 7220  ment driver for 
+00002210: 5344 5331 3230 3220 7769 6c6c 2077 6f72  SDS1202 will wor
+00002220: 6b20 7769 7468 2034 206c 696e 6573 206f  k with 4 lines o
+00002230: 6620 636f 6465 2c20 6a75 7374 206c 696b  f code, just lik
+00002240: 6520 7468 6520 4347 3633 352c 0d0a 6265  e the CG635,..be
+00002250: 666f 7265 2061 6464 696e 6720 7468 6520  fore adding the 
+00002260: 6d65 7468 6f64 2074 6f20 646f 776e 6c6f  method to downlo
+00002270: 6164 2077 6176 6566 6f72 6d73 2066 726f  ad waveforms fro
+00002280: 6d20 7468 6520 6f73 6369 6c6c 6f73 636f  m the oscillosco
+00002290: 7065 2e20 0d0a 4164 6420 6174 7472 6962  pe. ..Add attrib
+000022a0: 7574 6573 2061 6e64 206d 6574 686f 6473  utes and methods
+000022b0: 2069 6e63 7265 6d65 6e74 616c 6c79 2061   incrementally a
+000022c0: 7320 796f 7520 6e65 6564 2074 6f20 7573  s you need to us
+000022d0: 6520 6d6f 7265 2066 756e 6374 696f 6e73  e more functions
+000022e0: 206f 6620 7468 6520 696e 7374 7275 6d65   of the instrume
+000022f0: 6e74 2e0d 0a0d 0a2e 2e20 636f 6465 2d62  nt....... code-b
+00002300: 6c6f 636b 3a3a 0d0a 2020 2020 3a6c 696e  lock::..    :lin
+00002310: 656e 6f73 3a0d 0a0d 0a20 2020 2069 6d70  enos:....    imp
+00002320: 6f72 7420 6e75 6d70 7920 6173 206e 700d  ort numpy as np.
+00002330: 0a20 2020 2066 726f 6d20 7372 7367 7569  .    from srsgui
+00002340: 2069 6d70 6f72 7420 496e 7374 7275 6d65   import Instrume
+00002350: 6e74 0d0a 0d0a 2020 2020 636c 6173 7320  nt....    class 
+00002360: 5344 5331 3230 3228 496e 7374 7275 6d65  SDS1202(Instrume
+00002370: 6e74 293a 0d0a 2020 2020 2020 2020 5f49  nt):..        _I
+00002380: 6453 7472 696e 6720 3d20 2753 4453 3132  dString = 'SDS12
+00002390: 3032 270d 0a0d 0a20 2020 2020 2020 2064  02'....        d
+000023a0: 6566 2067 6574 5f77 6176 6566 6f72 6d28  ef get_waveform(
+000023b0: 7365 6c66 2c20 6368 616e 6e65 6c29 3a0d  self, channel):.
+000023c0: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
+000023d0: 0d0a 0d0a 2020 2020 2020 2020 6465 6620  ....        def 
+000023e0: 6765 745f 7361 6d70 6c69 6e67 5f72 6174  get_sampling_rat
+000023f0: 6528 7365 6c66 293a 0d0a 2020 2020 2020  e(self):..      
+00002400: 2020 2020 2020 2e2e 2e0d 0a0d 0a4f 6e63        .......Onc
+00002410: 6520 7468 6520 6f73 6369 6c6c 6f73 636f  e the oscillosco
+00002420: 7065 2069 7320 636f 6e6e 6563 7465 6420  pe is connected 
+00002430: 746f 2074 6865 2061 7070 6c69 6361 7469  to the applicati
+00002440: 6f6e 2c20 796f 7520 6361 6e20 7573 6520  on, you can use 
+00002450: 7468 6520 7465 726d 696e 616c 2074 6f20  the terminal to 
+00002460: 6578 706c 6f72 6520 7468 6520 6f73 6369  explore the osci
+00002470: 6c6c 6f73 636f 7065 2e0d 0a0d 0a2e 2e20  lloscope....... 
+00002480: 6669 6775 7265 3a3a 202e 2f5f 7374 6174  figure:: ./_stat
+00002490: 6963 2f6f 7363 2d64 6972 2d74 6572 6d69  ic/osc-dir-termi
+000024a0: 6e61 6c2d 7363 7265 656e 2d63 6170 7475  nal-screen-captu
+000024b0: 7265 2e70 6e67 0d0a 2020 2020 3a61 6c69  re.png..    :ali
+000024c0: 676e 3a20 6365 6e74 6572 0d0a 2020 2020  gn: center..    
+000024d0: 3a66 6967 636c 6173 733a 2061 6c69 676e  :figclass: align
+000024e0: 2d63 656e 7465 720d 0a0d 0a7c 0d0a 0d0a  -center....|....
+000024f0: 4265 6361 7573 6520 276f 7363 2720 6973  Because 'osc' is
+00002500: 206e 6f74 2074 6865 2064 6566 6175 6c74   not the default
+00002510: 2069 6e73 7472 756d 656e 742c 2079 6f75   instrument, you
+00002520: 2068 6176 6520 746f 2075 7365 2074 6865   have to use the
+00002530: 2070 7265 6669 7820 276f 7363 3a27 2077   prefix 'osc:' w
+00002540: 6974 6820 616c 6c20 7468 650d 0a72 6177  ith all the..raw
+00002550: 2072 656d 6f74 6520 636f 6d6d 616e 6473   remote commands
+00002560: 2079 6f75 2073 656e 6420 746f 2074 6865   you send to the
+00002570: 2069 6e73 7472 756d 656e 742e 2041 7320   instrument. As 
+00002580: 7368 6f77 6e20 7769 7468 2027 6f73 632e  shown with 'osc.
+00002590: 6469 7227 2c20 7468 6572 6520 6172 6520  dir', there are 
+000025a0: 6d61 6e79 206d 6574 686f 6473 0d0a 6176  many methods..av
+000025b0: 6169 6c61 626c 6520 7769 7468 2027 6f73  ailable with 'os
+000025c0: 632e 2720 4576 656e 206f 7363 2e67 6574  c.' Even osc.get
+000025d0: 5f77 6176 6566 6f72 6d28 2920 6973 2061  _waveform() is a
+000025e0: 7661 696c 6162 6c65 2066 726f 6d20 7468  vailable from th
+000025f0: 6520 7465 726d 696e 616c 2e20 0d0a 5768  e terminal. ..Wh
+00002600: 656e 2079 6f75 2075 7365 2061 206d 6574  en you use a met
+00002610: 686f 6420 696e 636f 7272 6563 746c 792c  hod incorrectly,
+00002620: 2074 6865 2074 6572 6d69 6e61 6c20 6b69   the terminal ki
+00002630: 6e64 6c79 2074 656c 6c73 206d 6520 7468  ndly tells me th
+00002640: 6174 2074 6865 7265 2069 7320 6120 6d69  at there is a mi
+00002650: 7373 696e 6720 6172 6775 6d65 6e74 200d  ssing argument .
+00002660: 0a69 6e20 6120 6675 6e63 7469 6f6e 2063  .in a function c
+00002670: 616c 6c2e 0d0a 596f 7520 6361 6e20 7365  all...You can se
+00002680: 6520 606f 7363 2e67 6574 5f77 6176 6566  e `osc.get_wavef
+00002690: 6f72 6d28 6368 616e 6e65 6c29 6020 7265  orm(channel)` re
+000026a0: 7475 726e 7320 7477 6f20 6e75 6d70 7920  turns two numpy 
+000026b0: 6172 7261 7973 2e0d 0a57 6861 7420 6966  arrays...What if
+000026c0: 2079 6f75 2077 616e 7420 746f 2070 6c6f   you want to plo
+000026d0: 7420 7468 6520 6461 7461 3f0d 0a41 7320  t the data?..As 
+000026e0: 7468 6520 6d65 7468 6f64 7320 796f 7520  the methods you 
+000026f0: 696d 706c 656d 656e 7420 666f 7220 696e  implement for in
+00002700: 7465 7261 6374 696e 6720 7769 7468 2079  teracting with y
+00002710: 6f75 7220 696e 7374 7275 6d65 6e74 7320  our instruments 
+00002720: 616e 6420 6461 7461 2067 726f 7720 696e  and data grow in
+00002730: 2063 6f6d 706c 6578 6974 792c 0d0a 796f   complexity,..yo
+00002740: 7520 6d61 7920 6e65 6564 2074 6f20 6772  u may need to gr
+00002750: 6164 7561 7465 2066 726f 6d20 7465 726d  aduate from term
+00002760: 696e 616c 2d62 6173 6564 2069 6e74 6572  inal-based inter
+00002770: 6163 7469 6f6e 2074 6f20 7461 736b 2d62  action to task-b
+00002780: 6173 6564 2069 6e74 6572 6163 7469 6f6e  ased interaction
+00002790: 2e20 5265 6164 206f 6e2e 0d0a 0d0a 5461  . Read on.....Ta
+000027a0: 736b 730d 0a2d 2d2d 2d2d 2d2d 0d0a 0d0a  sks..-------....
+000027b0: 486f 7720 746f 2072 756e 2061 2074 6173  How to run a tas
+000027c0: 6b0d 0a5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  k..^^^^^^^^^^^^^
+000027d0: 5e5e 5e5e 5e5e 0d0a 0d0a 5374 6172 7420  ^^^^^^....Start 
+000027e0: 7468 6520 6060 7372 7367 7569 6060 2061  the ``srsgui`` a
+000027f0: 7070 6c69 6361 7469 6f6e 2e20 596f 7520  pplication. You 
+00002800: 6361 6e20 7365 6520 7768 6572 6520 7468  can see where th
+00002810: 6520 2e74 6173 6b63 6f6e 6669 6720 6669  e .taskconfig fi
+00002820: 6c65 2069 7320 6f70 656e 6564 0d0a 6672  le is opened..fr
+00002830: 6f6d 2074 6865 2063 6f6e 736f 6c65 2077  om the console w
+00002840: 696e 646f 7720 283a 7265 663a 6068 6572  indow (:ref:`her
+00002850: 6520 3c74 6f70 2d6f 662d 696e 6974 6961  e <top-of-initia
+00002860: 6c2d 7363 7265 656e 2d63 6170 7475 7265  l-screen-capture
+00002870: 3e60 292e 0d0a 4966 2079 6f75 206d 6164  >`)...If you mad
+00002880: 6520 6120 636f 7079 206f 6620 7468 6520  e a copy of the 
+00002890: 6f72 6967 696e 616c 2065 7861 6d70 6c65  original example
+000028a0: 2066 726f 6d20 7468 6520 6060 7372 7367   from the ``srsg
+000028b0: 7569 6060 0d0a 7061 636b 6167 6520 6469  ui``..package di
+000028c0: 7265 6374 6f72 792c 206f 7065 6e20 6974  rectory, open it
+000028d0: 2061 6761 696e 2066 726f 6d20 7468 6520   again from the 
+000028e0: 636f 7272 6563 7420 6469 7265 6374 6f72  correct director
+000028f0: 792e 0d0a 0d0a 4966 2074 6865 7265 2061  y.....If there a
+00002900: 7265 206e 6f20 6572 726f 7220 6d65 7373  re no error mess
+00002910: 6167 6573 2069 6e20 7468 6520 436f 6e73  ages in the Cons
+00002920: 6f6c 6520 7769 6e64 6f77 2c20 636f 6e6e  ole window, conn
+00002930: 6563 7420 7468 6520 6675 6e63 7469 6f6e  ect the function
+00002940: 2067 656e 6572 6174 6f72 0d0a 616e 6420   generator..and 
+00002950: 7468 6520 6f73 6369 6c6c 6f73 636f 7065  the oscilloscope
+00002960: 2066 726f 6d20 7468 6520 496e 7374 7275   from the Instru
+00002970: 6d65 6e74 7320 6d65 6e75 2e0d 0a0d 0a54  ments menu.....T
+00002980: 6865 206f 7665 7261 6c6c 2073 7472 7563  he overall struc
+00002990: 7475 7265 206f 6620 6120 7461 736b 2069  ture of a task i
+000029a0: 7320 6465 7363 7269 6265 6420 696e 203a  s described in :
+000029b0: 7265 663a 6057 7269 7469 6e67 2061 2074  ref:`Writing a t
+000029c0: 6173 6b20 7363 7269 7074 6020 7365 6374  ask script` sect
+000029d0: 696f 6e2e 0d0a 5468 6572 6520 6172 6520  ion...There are 
+000029e0: 3520 7461 736b 7320 6172 6520 696e 636c  5 tasks are incl
+000029f0: 7564 6564 2069 6e20 7468 6520 6578 616d  uded in the exam
+00002a00: 706c 6520 7072 6f6a 6563 742e 2054 6865  ple project. The
+00002a10: 7920 6772 6164 7561 6c6c 7920 6164 6420  y gradually add 
+00002a20: 6d6f 7265 2066 6561 7475 7265 730d 0a6f  more features..o
+00002a30: 6e20 7468 6520 746f 7020 6f66 2074 6865  n the top of the
+00002a40: 2070 7265 7669 6f75 7320 7461 736b 732e   previous tasks.
+00002a50: 200d 0a54 6865 7920 6172 6520 6465 7369   ..They are desi
+00002a60: 676e 6564 2074 6f20 7368 6f77 6361 7365  gned to showcase
+00002a70: 2068 6f77 2074 6f20 7573 6520 7468 6520   how to use the 
+00002a80: 5461 736b 2063 6c61 7373 2e0d 0a0d 0a53  Task class.....S
+00002a90: 656c 6563 7420 7468 6520 6669 7273 7420  elect the first 
+00002aa0: 7461 736b 2028 5c2a 4944 4e20 7465 7374  task (\*IDN test
+00002ab0: 2920 6672 6f6d 2074 6865 2054 6173 6b73  ) from the Tasks
+00002ac0: 206d 656e 750d 0a61 6e64 2063 6c69 636b   menu..and click
+00002ad0: 2074 6865 2067 7265 656e 2061 7272 6f77   the green arrow
+00002ae0: 2069 6e20 7468 6520 746f 6f6c 2062 6172   in the tool bar
+00002af0: 2074 6f20 7275 6e20 7468 6520 7461 736b   to run the task
+00002b00: 2e0d 0a0d 0a46 6972 7374 5461 736b 0d0a  .....FirstTask..
+00002b10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a0d 0a54  -----------....T
+00002b20: 6865 2066 6972 7374 2074 6173 6b20 7368  he first task sh
+00002b30: 6f77 733a 0d0a 0d0a 2020 2020 2d20 486f  ows:....    - Ho
+00002b40: 7720 746f 2075 7365 206d 6f64 756c 652d  w to use module-
+00002b50: 6c65 7665 6c20 6c6f 6767 6572 2066 6f72  level logger for
+00002b60: 2050 7974 686f 6e20 6c6f 6767 696e 675f   Python logging_
+00002b70: 2069 6e20 6120 7461 736b 0d0a 2020 2020   in a task..    
+00002b80: 2d20 486f 7720 746f 2075 7365 2069 6e73  - How to use ins
+00002b90: 7472 756d 656e 7473 2064 6566 696e 6564  truments defined
+00002ba0: 2069 6e20 7468 6520 636f 6e66 6967 7572   in the configur
+00002bb0: 6174 696f 6e20 6669 6c65 0d0a 2020 2020  ation file..    
+00002bc0: 2d20 486f 7720 746f 2075 7365 2074 6578  - How to use tex
+00002bd0: 7420 6f75 7470 7574 2074 6f20 7468 6520  t output to the 
+00002be0: 636f 6e73 6f6c 6520 7769 6e64 6f77 0d0a  console window..
+00002bf0: 0d0a 4974 2069 7320 6e6f 7420 6d75 6368  ..It is not much
+00002c00: 2064 6966 6665 7265 6e74 2066 726f 6d20   different from 
+00002c10: 7468 6520 3a72 6566 3a60 6261 7265 2062  the :ref:`bare b
+00002c20: 6f6e 6520 7374 7275 6374 7572 6520 3c74  one structure <t
+00002c30: 6f70 2d6f 662d 6261 7265 2d62 6f6e 652d  op-of-bare-bone-
+00002c40: 7461 736b 3e60 0d0a 7368 6f77 6e20 696e  task>`..shown in
+00002c50: 2074 6865 203a 7265 663a 6057 7269 7469   the :ref:`Writi
+00002c60: 6e67 2061 2074 6173 6b20 7363 7269 7074  ng a task script
+00002c70: 6020 7365 6374 696f 6e2e 0d0a 0d0a 2e2e  ` section.......
+00002c80: 206c 6974 6572 616c 696e 636c 7564 653a   literalinclude:
+00002c90: 3a20 2e2e 2f73 7273 6775 692f 6578 616d  : ../srsgui/exam
+00002ca0: 706c 6573 2f6f 7363 696c 6c6f 7363 6f70  ples/oscilloscop
+00002cb0: 6520 6578 616d 706c 652f 7461 736b 732f  e example/tasks/
+00002cc0: 6669 7273 742e 7079 0d0a 2020 2020 3a6c  first.py..    :l
+00002cd0: 616e 6775 6167 653a 2050 7974 686f 6e0d  anguage: Python.
+00002ce0: 0a20 2020 203a 6c69 6e65 6e6f 733a 0d0a  .    :linenos:..
+00002cf0: 0d0a 5573 696e 6720 2a2a 7365 6c66 2e6c  ..Using **self.l
+00002d00: 6f67 6765 722a 2a20 7365 6e64 7320 7468  ogger** sends th
+00002d10: 6520 6c6f 6767 696e 6720 6f75 7470 7574  e logging output
+00002d20: 2074 6f20 7468 6520 636f 6e73 6f6c 6520   to the console 
+00002d30: 7769 6e64 6f77 2c20 7468 6520 6d61 7374  window, the mast
+00002d40: 6572 206c 6f67 6769 6e67 2066 696c 6520  er logging file 
+00002d50: 696e 0d0a 607e 2f74 6173 6b2d 7265 7375  in..`~/task-resu
+00002d60: 6c74 7320 6469 7265 6374 6f72 792f 6d61  lts directory/ma
+00002d70: 696e 6c6f 672d 7878 2e74 7874 2e78 602c  inlog-xx.txt.x`,
+00002d80: 2061 6e64 2074 6f20 7468 6520 7461 736b   and to the task
+00002d90: 2072 6573 756c 7420 6461 7461 2066 696c   result data fil
+00002da0: 6520 6c6f 6361 7465 6420 696e 0d0a 607e  e located in..`~
+00002db0: 2f74 6173 6b2d 7265 7375 6c74 732f 7072  /task-results/pr
+00002dc0: 6f6a 6563 742d 6e61 6d65 2d69 6e2d 636f  oject-name-in-co
+00002dd0: 6e66 6967 2d66 696c 652f 524e 7878 7860  nfig-file/RNxxx`
+00002de0: 2064 6972 6563 746f 7279 2e0d 0a0d 0a57   directory.....W
+00002df0: 6974 6820 3a6d 6574 683a 6067 6574 5f69  ith :meth:`get_i
+00002e00: 6e73 7472 756d 656e 7420 3c73 7273 6775  nstrument <srsgu
+00002e10: 692e 7461 736b 2e74 6173 6b2e 5461 736b  i.task.task.Task
+00002e20: 2e67 6574 5f69 6e73 7472 756d 656e 743e  .get_instrument>
+00002e30: 6020 796f 7520 6361 6e20 6765 7420 7468  ` you can get th
+00002e40: 6520 696e 7374 7275 6d65 6e74 0d0a 6465  e instrument..de
+00002e50: 6669 6e65 6420 696e 2074 6865 2063 6f6e  fined in the con
+00002e60: 6669 6775 7261 7469 6f6e 2066 696c 6520  figuration file 
+00002e70: 696e 2061 2074 6173 6b2e 202a 2a44 6f20  in a task. **Do 
+00002e80: 6e6f 7420 6469 7363 6f6e 6e65 6374 2074  not disconnect t
+00002e90: 6865 2069 6e73 7472 756d 656e 7420 696e  he instrument in
+00002ea0: 2074 6865 2074 6173 6b21 2a2a 0d0a 496e   the task!**..In
+00002eb0: 7374 7275 6d65 6e74 2043 6f6e 6e65 6374  strument Connect
+00002ec0: 6976 6974 7920 6973 206d 616e 6167 6564  ivity is managed
+00002ed0: 2061 7420 7468 6520 6060 7372 7367 7569   at the ``srsgui
+00002ee0: 6060 2061 7070 6c69 6361 7469 6f6e 206c  `` application l
+00002ef0: 6576 656c 2e0d 0a0d 0a54 6869 7320 7461  evel.....This ta
+00002f00: 736b 2068 6967 686c 6967 6874 7320 686f  sk highlights ho
+00002f10: 7720 7265 6d6f 7465 2063 6f6d 6d61 6e64  w remote command
+00002f20: 2073 6574 2061 6e64 2071 7565 7279 2074   set and query t
+00002f30: 7261 6e73 6163 7469 6f6e 7320 6172 6520  ransactions are 
+00002f40: 7369 6d70 6c69 6669 6564 2062 7920 6465  simplified by de
+00002f50: 6669 6e69 6e67 200d 0a61 6e20 6174 7472  fining ..an attr
+00002f60: 6962 7574 6520 7573 696e 6720 3a6d 6f64  ibute using :mod
+00002f70: 3a60 7372 7367 7569 2e69 6e73 742e 636f  :`srsgui.inst.co
+00002f80: 6d6d 616e 6473 6020 6d6f 6475 6c65 2c20  mmands` module, 
+00002f90: 0d0a 7768 6963 6820 6973 2075 7469 6c69  ..which is utili
+00002fa0: 7a65 6420 696e 2074 6865 2043 4736 3335  zed in the CG635
+00002fb0: 2063 6c61 7373 2064 6566 696e 6974 696f   class definitio
+00002fc0: 6e20 7669 6120 7468 6520 666f 6c6c 6f77  n via the follow
+00002fd0: 696e 6720 6c69 6e65 3a20 200d 0a0d 0a60  ing line:  ....`
+00002fe0: 6066 7265 7175 656e 6379 203d 2046 6c6f  `frequency = Flo
+00002ff0: 6174 436f 6d6d 616e 6428 2746 5245 5127  atCommand('FREQ'
+00003000: 2960 600d 0a0d 0a54 6869 7320 7369 6d70  )``....This simp
+00003010: 6c65 206c 696e 6520 6d61 6b65 7320 6974  le line makes it
+00003020: 2070 6f73 7369 626c 6520 746f 2073 6574   possible to set
+00003030: 2061 6e64 2071 7565 7279 2074 6865 2060   and query the `
+00003040: 6367 2e66 7265 7175 656e 6379 6020 0d0a  cg.frequency` ..
+00003050: 7769 7468 6f75 7420 6861 7669 6e67 2074  without having t
+00003060: 6f20 6469 7265 6374 6c79 206d 616e 6970  o directly manip
+00003070: 756c 6174 6520 636f 6d6d 616e 6420 6f72  ulate command or
+00003080: 2072 6573 706f 6e73 6520 7374 7269 6e67   response string
+00003090: 732e 200d 0a0d 0a53 6563 6f6e 6454 6173  s. ....SecondTas
+000030a0: 6b0d 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a  k..-----------..
+000030b0: 0d0a 5468 6520 7365 636f 6e64 2074 6173  ..The second tas
+000030c0: 6b20 7265 7175 6972 6573 206e 6f20 696e  k requires no in
+000030d0: 7374 7275 6d65 6e74 2063 6f6e 6e65 6374  strument connect
+000030e0: 696f 6e73 2c20 616e 6420 7368 6f77 733a  ions, and shows:
+000030f0: 0d0a 0d0a 2020 2020 2d20 486f 7720 746f  ....    - How to
+00003100: 2064 6566 696e 6520 3a61 7474 723a 6069   define :attr:`i
+00003110: 6e70 7574 5f70 6172 616d 6574 6572 7320  nput_parameters 
+00003120: 3c73 7273 6775 692e 7461 736b 2e74 6173  <srsgui.task.tas
+00003130: 6b2e 5461 736b 2e69 6e70 7574 5f70 6172  k.Task.input_par
+00003140: 616d 6574 6572 733e 600d 0a20 2020 2020  ameters>`..     
+00003150: 2066 6f72 2069 6e74 6572 6163 7469 7665   for interactive
+00003160: 2075 7365 7220 696e 7075 7420 6672 6f6d   user input from
+00003170: 2074 6865 2061 7070 6c69 6361 7469 6f6e   the application
+00003180: 2069 6e70 7574 2070 616e 656c 0d0a 2020   input panel..  
+00003190: 2020 2d20 486f 7720 746f 2075 7365 206d    - How to use m
+000031a0: 6174 706c 6f74 6c69 6220 6669 6775 7265  atplotlib figure
+000031b0: 7320 666f 7220 706c 6f74 7469 6e67 2064  s for plotting d
+000031c0: 6174 610d 0a20 2020 202d 2048 6f77 2074  ata..    - How t
+000031d0: 6f20 7365 6e64 2074 6578 7420 6f75 7470  o send text outp
+000031e0: 7574 2074 6f20 7468 6520 7265 7375 6c74  ut to the result
+000031f0: 2077 696e 646f 7720 7573 696e 670d 0a20   window using.. 
+00003200: 2020 2020 203a 6d65 7468 3a60 6469 7370       :meth:`disp
+00003210: 6c61 795f 7265 7375 6c74 2829 203c 7372  lay_result() <sr
+00003220: 7367 7569 2e74 6173 6b2e 7461 736b 2e54  sgui.task.task.T
+00003230: 6173 6b2e 6469 7370 6c61 795f 7265 7375  ask.display_resu
+00003240: 6c74 3e60 0d0a 2020 2020 2d20 486f 7720  lt>`..    - How 
+00003250: 746f 2073 746f 7020 7468 6520 7461 736b  to stop the task
+00003260: 2062 7920 6368 6563 6b69 6e67 0d0a 2020   by checking..  
+00003270: 2020 2020 3a6d 6574 683a 6069 735f 7275      :meth:`is_ru
+00003280: 6e6e 696e 6728 2920 3c73 7273 6775 692e  nning() <srsgui.
+00003290: 7461 736b 2e74 6173 6b2e 5461 736b 2e69  task.task.Task.i
+000032a0: 735f 7275 6e6e 696e 673e 602e 0d0a 0d0a  s_running>`.....
+000032b0: 2e2e 206c 6974 6572 616c 696e 636c 7564  .. literalinclud
+000032c0: 653a 3a20 2e2e 2f73 7273 6775 692f 6578  e:: ../srsgui/ex
+000032d0: 616d 706c 6573 2f6f 7363 696c 6c6f 7363  amples/oscillosc
+000032e0: 6f70 6520 6578 616d 706c 652f 7461 736b  ope example/task
+000032f0: 732f 7365 636f 6e64 2e70 790d 0a20 2020  s/second.py..   
+00003300: 203a 6c61 6e67 7561 6765 3a20 5079 7468   :language: Pyth
+00003310: 6f6e 0d0a 2020 2020 3a6c 696e 656e 6f73  on..    :linenos
+00003320: 3a0d 0a0d 0a55 7369 6e67 206d 6174 706c  :....Using matpl
+00003330: 6f74 6c69 625f 2077 6974 6820 6060 7372  otlib_ with ``sr
+00003340: 7367 7569 6060 2069 7320 7374 7261 6967  sgui`` is straig
+00003350: 6874 666f 7277 6172 6420 6966 2079 6f75  htforward if you
+00003360: 2061 7265 2061 6c72 6561 6479 2066 616d   are already fam
+00003370: 696c 6961 7220 7769 7468 2069 7473 2075  iliar with its u
+00003380: 7361 6765 2e0d 0a28 5265 6665 7220 746f  sage...(Refer to
+00003390: 206d 6174 706c 6f74 6c69 625f 2064 6f63   matplotlib_ doc
+000033a0: 756d 656e 7461 7469 6f6e 292e 0d0a 0d0a  umentation).....
+000033b0: 5468 6520 696d 706f 7274 616e 7420 6469  The important di
+000033c0: 6666 6572 656e 6365 7320 7768 656e 2075  fferences when u
+000033d0: 7369 6e67 206d 6174 706c 6f74 6c69 6220  sing matplotlib 
+000033e0: 696e 2060 6073 7273 6775 6960 6020 6172  in ``srsgui`` ar
+000033f0: 653a 0d0a 2020 2020 2d20 596f 7520 6861  e:..    - You ha
+00003400: 7665 2074 6f20 6765 7420 7468 6520 6669  ve to get the fi
+00003410: 6775 7265 2075 7369 6e67 2067 6574 5f66  gure using get_f
+00003420: 6967 7572 6528 292c 2072 6174 6865 7220  igure(), rather 
+00003430: 7468 616e 2063 7265 6174 696e 6720 6f6e  than creating on
+00003440: 6520 6f6e 2079 6f75 7220 6f77 6e2e 0d0a  e on your own...
+00003450: 2020 2020 2d20 506c 6f74 7320 6172 6520      - Plots are 
+00003460: 6372 6561 7465 6420 6475 7269 6e67 2060  created during `
+00003470: 7365 7475 7028 2960 2c20 6265 6361 7573  setup()`, becaus
+00003480: 6520 6974 2069 7320 6120 736c 6f77 2070  e it is a slow p
+00003490: 726f 6365 7373 2e20 4475 7269 6e67 2060  rocess. During `
+000034a0: 7465 7374 2829 602c 0d0a 2020 2020 2020  test()`,..      
+000034b0: 796f 7520 7369 6d70 6c79 2075 7064 6174  you simply updat
+000034c0: 6520 6461 7461 2075 7369 6e67 2060 7365  e data using `se
+000034d0: 745f 6461 7461 2829 6020 6f72 2073 696d  t_data()` or sim
+000034e0: 696c 6961 7220 6d65 7468 6f64 7320 666f  iliar methods fo
+000034f0: 7220 6461 7461 2075 7064 6174 652e 0d0a  r data update...
+00003500: 2020 2020 2d20 596f 7520 6d75 7374 2075      - You must u
+00003510: 7365 2060 7265 7175 6573 745f 6669 6775  se `request_figu
+00003520: 7265 5f75 7064 6174 6528 2960 2074 6f20  re_update()` to 
+00003530: 7265 6472 6177 2074 6865 2070 6c6f 742c  redraw the plot,
+00003540: 2061 6674 6572 2060 7365 745f 6461 7461   after `set_data
+00003550: 2829 602e 0d0a 2020 2020 2020 5468 6520  ()`...      The 
+00003560: 6576 656e 7420 6c6f 6f70 2068 616e 646c  event loop handl
+00003570: 6572 2069 6e20 7468 6520 6d61 696e 2061  er in the main a
+00003580: 7070 6c69 6361 7469 6f6e 2077 696c 6c20  pplication will 
+00003590: 7570 6461 7465 2074 6865 2070 6c6f 7420  update the plot 
+000035a0: 6174 2069 7473 2065 6172 6c69 6573 740d  at its earliest.
+000035b0: 0a20 2020 2020 2063 6f6e 7665 6e69 656e  .      convenien
+000035c0: 6365 2e0d 0a0d 0a0d 0a2e 2e20 6669 6775  ce......... figu
+000035d0: 7265 3a3a 202e 2f5f 7374 6174 6963 2f73  re:: ./_static/s
+000035e0: 6563 6f6e 642d 7461 736b 2d73 6372 6565  econd-task-scree
+000035f0: 6e2d 6361 7074 7572 652e 706e 670d 0a20  n-capture.png.. 
+00003600: 2020 203a 616c 6967 6e3a 2063 656e 7465     :align: cente
+00003610: 720d 0a20 2020 203a 6669 6763 6c61 7373  r..    :figclass
+00003620: 3a20 616c 6967 6e2d 6365 6e74 6572 0d0a  : align-center..
+00003630: 0d0a 7c0d 0a0d 0a54 6869 7264 5461 736b  ..|....ThirdTask
+00003640: 0d0a 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a0d  ..-----------...
+00003650: 0a54 6865 2074 6869 7264 2074 6173 6b20  .The third task 
+00003660: 7573 6573 2074 6865 206f 7363 696c 6c6f  uses the oscillo
+00003670: 7363 6f70 6520 6f6e 6c79 2e20 4974 2067  scope only. It g
+00003680: 6574 7320 7468 6520 7265 7175 6573 7465  ets the requeste
+00003690: 6420 6e75 6d62 6572 206f 6620 6361 7074  d number of capt
+000036a0: 7572 6573 2066 726f 6d20 7573 6572 2069  ures from user i
+000036b0: 6e70 7574 2c0d 0a74 6865 6e20 7265 7065  nput,..then repe
+000036c0: 6174 7320 6f73 6369 6c6c 6f73 636f 7065  ats oscilloscope
+000036d0: 2077 6176 6566 6f72 6d20 6361 7074 7572   waveform captur
+000036e0: 6520 616e 6420 7570 6461 7465 7320 7468  e and updates th
+000036f0: 6520 7761 7665 666f 726d 2070 6c6f 742e  e waveform plot.
+00003700: 200d 0a49 7420 7374 6f70 7320 6f6e 6365   ..It stops once
+00003710: 2074 6865 2064 6573 6972 6564 206e 756d   the desired num
+00003720: 6265 7220 6f66 2063 6170 7475 7265 7320  ber of captures 
+00003730: 6861 7665 2062 6565 6e20 6f62 7461 696e  have been obtain
+00003740: 6564 2c20 6f72 2077 6865 6e20 7468 6520  ed, or when the 
+00003750: 5374 6f70 2062 7574 746f 6e20 6973 2070  Stop button is p
+00003760: 7265 7373 6564 2e0d 0a57 6176 6566 6f72  ressed...Wavefor
+00003770: 6d73 2061 7265 2063 6170 7475 7265 6420  ms are captured 
+00003780: 7769 7468 2037 3030 3030 3020 706f 696e  with 700000 poin
+00003790: 7473 2061 626f 7574 2065 7665 7279 2030  ts about every 0
+000037a0: 2e32 2073 6563 6f6e 6473 206f 7665 7220  .2 seconds over 
+000037b0: 5443 502f 4950 2063 6f6d 6d75 6e63 6174  TCP/IP communcat
+000037c0: 696f 6e2e 0d0a 0d0a 0d0a 2e2e 206c 6974  ion......... lit
+000037d0: 6572 616c 696e 636c 7564 653a 3a20 2e2e  eralinclude:: ..
+000037e0: 2f73 7273 6775 692f 6578 616d 706c 6573  /srsgui/examples
+000037f0: 2f6f 7363 696c 6c6f 7363 6f70 6520 6578  /oscilloscope ex
+00003800: 616d 706c 652f 7461 736b 732f 7468 6972  ample/tasks/thir
+00003810: 642e 7079 0d0a 2020 2020 3a6c 616e 6775  d.py..    :langu
+00003820: 6167 653a 2050 7974 686f 6e0d 0a20 2020  age: Python..   
+00003830: 203a 6c69 6e65 6e6f 733a 0d0a 0d0a 466f   :linenos:....Fo
+00003840: 7572 7468 5461 736b 0d0a 2d2d 2d2d 2d2d  urthTask..------
+00003850: 2d2d 2d2d 2d0d 0a0d 0a54 6865 2066 6f75  -----....The fou
+00003860: 7274 6820 6578 616d 706c 6520 6973 2074  rth example is t
+00003870: 6865 2063 6c69 6d61 7820 6f66 2074 6865  he climax of the
+00003880: 2065 7861 6d70 6c65 7320 7365 7269 6573   examples series
+00003890: 2028 3a72 6566 3a60 7363 7265 656e 7368   (:ref:`screensh
+000038a0: 6f74 203c 746f 702d 6f66 2d73 6372 6565  ot <top-of-scree
+000038b0: 6e2d 6361 7074 7572 652d 313e 6029 2e0d  n-capture-1>`)..
+000038c0: 0a49 7420 7573 6573 2060 696e 7075 745f  .It uses `input_
+000038d0: 7061 7261 6d65 7465 7273 6020 746f 2063  parameters` to c
+000038e0: 6861 6e67 6520 6f75 7470 7574 2066 7265  hange output fre
+000038f0: 7175 656e 6379 206f 6620 7468 6520 636c  quency of the cl
+00003900: 6f63 6b20 6765 6e65 7261 746f 7220 696e  ock generator in
+00003910: 7465 7261 6374 6976 656c 792c 0d0a 6361  teractively,..ca
+00003920: 7074 7572 6573 2077 6176 6566 6f72 6d73  ptures waveforms
+00003930: 2066 726f 6d20 7468 6520 6f73 6369 6c6c   from the oscill
+00003940: 6f73 636f 7065 2c20 6361 6c63 756c 6174  oscope, calculat
+00003950: 6573 2061 6e20 4646 5420 6f66 2074 6865  es an FFT of the
+00003960: 2077 6176 6566 6f72 6d73 2077 6974 6820   waveforms with 
+00003970: 6e75 6d70 792c 0d0a 616e 6420 6765 6e65  numpy,..and gene
+00003980: 7261 7465 7320 706c 6f74 7320 7573 696e  rates plots usin
+00003990: 6720 3220 6d61 7470 6c6f 746c 6962 2066  g 2 matplotlib f
+000039a0: 6967 7572 6573 2e0d 0a0d 0a42 7920 6164  igures.....By ad
+000039b0: 6469 6e67 2074 6865 206e 616d 6573 206f  ding the names o
+000039c0: 6620 6669 6775 7265 7320 7468 6174 2079  f figures that y
+000039d0: 6f75 2077 616e 7420 746f 2075 7365 2069  ou want to use i
+000039e0: 6e20 6164 6469 7469 6f6e 616c 5f66 6967  n additional_fig
+000039f0: 7572 655f 6e61 6d65 732c 0d0a 6060 7372  ure_names,..``sr
+00003a00: 7367 7569 6060 2070 726f 7669 6465 7320  sgui`` provides 
+00003a10: 6d6f 7265 2066 6967 7572 6573 2074 6f20  more figures to 
+00003a20: 7468 6520 7461 736b 2062 6566 6f72 6520  the task before 
+00003a30: 6974 2073 7461 7274 732e 0d0a 0d0a 2e2e  it starts.......
+00003a40: 206c 6974 6572 616c 696e 636c 7564 653a   literalinclude:
+00003a50: 3a20 2e2e 2f73 7273 6775 692f 6578 616d  : ../srsgui/exam
+00003a60: 706c 6573 2f6f 7363 696c 6c6f 7363 6f70  ples/oscilloscop
+00003a70: 6520 6578 616d 706c 652f 7461 736b 732f  e example/tasks/
+00003a80: 666f 7572 7468 2e70 790d 0a20 2020 203a  fourth.py..    :
+00003a90: 6c61 6e67 7561 6765 3a20 5079 7468 6f6e  language: Python
+00003aa0: 0d0a 2020 2020 3a6c 696e 656e 6f73 3a0d  ..    :linenos:.
+00003ab0: 0a0d 0a46 6966 7468 5461 736b 0d0a 2d2d  ...FifthTask..--
+00003ac0: 2d2d 2d2d 2d2d 2d2d 0d0a 0d0a 5468 6520  --------....The 
+00003ad0: 6669 6674 6820 7461 736b 2073 686f 7773  fifth task shows
+00003ae0: 2068 6f77 2074 6f20 7375 6263 6c61 7373   how to subclass
+00003af0: 2061 6e20 6578 6973 7469 6e67 2074 6173   an existing tas
+00003b00: 6b20 636c 6173 7320 666f 7220 7265 7573  k class for reus
+00003b10: 652e 0d0a 5468 6520 6d65 7468 6f64 2067  e...The method g
+00003b20: 6574 5f77 6176 6566 6f72 6d28 2920 696e  et_waveform() in
+00003b30: 2074 6865 2066 6f75 7274 6820 6578 616d   the fourth exam
+00003b40: 706c 6520 6973 2072 6569 6d70 6c65 6d65  ple is reimpleme
+00003b50: 6e74 6564 2074 6f20 6765 6e65 7261 7465  nted to generate
+00003b60: 0d0a 7369 6d75 6c61 7465 6420 7761 7665  ..simulated wave
+00003b70: 666f 726d 2074 6861 7420 7275 6e73 2077  form that runs w
+00003b80: 6974 686f 7574 2061 6e79 2072 6561 6c20  ithout any real 
+00003b90: 6f73 6369 6c6c 6f73 636f 7065 2e0d 0a0d  oscilloscope....
+00003ba0: 0a4e 6f74 6520 7468 6174 2074 6865 2073  .Note that the s
+00003bb0: 7175 6172 6520 7761 7665 2065 6467 6520  quare wave edge 
+00003bc0: 6361 6c63 756c 6174 696f 6e20 6973 2063  calculation is c
+00003bd0: 7275 6465 2c20 6361 7573 696e 6720 6d6f  rude, causing mo
+00003be0: 6475 6c61 7469 6f6e 2069 6e20 7075 6c73  dulation in puls
+00003bf0: 6520 7769 6474 680d 0a61 6e64 2073 6964  e width..and sid
+00003c00: 6520 6261 6e64 7320 696e 2074 6865 2046  e bands in the F
+00003c10: 4654 2073 7065 6374 7275 6d20 6966 2074  FT spectrum if t
+00003c20: 6865 2073 6574 2066 7265 7175 656e 6379  he set frequency
+00003c30: 2069 7320 6e6f 7420 636f 6d6d 656e 7375   is not commensu
+00003c40: 7261 7465 2077 6974 680d 0a74 6865 2073  rate with..the s
+00003c50: 616d 706c 696e 6720 7261 7465 2e20 546f  ampling rate. To
+00003c60: 2067 656e 6572 6174 6520 6120 636c 6561   generate a clea
+00003c70: 6e20 7371 7561 7265 2077 6176 652c 2074  n square wave, t
+00003c80: 6865 2072 6973 696e 6720 616e 6420 6661  he rising and fa
+00003c90: 6c6c 696e 6720 6564 6765 7320 7368 6f75  lling edges shou
+00003ca0: 6c64 0d0a 6861 7665 2061 7420 6c65 6173  ld..have at leas
+00003cb0: 7420 7477 6f20 706f 696e 7473 2074 6f20  t two points to 
+00003cc0: 7265 7072 6573 656e 7420 6578 6163 7420  represent exact 
+00003cd0: 7068 6173 652e 2044 6972 6563 7420 7472  phase. Direct tr
+00003ce0: 616e 7369 7469 6f6e 2066 726f 6d20 6c6f  ansition from lo
+00003cf0: 7720 746f 2068 6967 680d 0a77 6974 686f  w to high..witho
+00003d00: 7574 2061 6e79 2069 6e74 6572 6d65 6469  ut any intermedi
+00003d10: 6174 6520 706f 696e 7473 2073 7566 6665  ate points suffe
+00003d20: 7273 2066 726f 6d20 7375 6274 6c65 206d  rs from subtle m
+00003d30: 6f64 756c 6174 696f 6e20 696e 2074 696d  odulation in tim
+00003d40: 6520 646f 6d61 696e 2c0d 0a77 6869 6368  e domain,..which
+00003d50: 206d 616e 6966 6573 7473 2061 7320 7369   manifests as si
+00003d60: 6465 2062 616e 6473 2069 6e20 4646 542e  de bands in FFT.
+00003d70: 2054 6869 7320 6973 2061 2063 6f6d 6d6f   This is a commo
+00003d80: 6e20 7072 6f62 6c65 6d20 696e 2064 6967  n problem in dig
+00003d90: 6974 616c 2073 6967 6e61 6c0d 0a70 726f  ital signal..pro
+00003da0: 6365 7373 696e 672e 2049 7420 6973 206e  cessing. It is n
+00003db0: 6f74 2061 2070 726f 626c 656d 2069 6e20  ot a problem in 
+00003dc0: 7468 6520 7265 616c 2077 6f72 6c64 2c20  the real world, 
+00003dd0: 6265 6361 7573 6520 7468 6520 7369 676e  because the sign
+00003de0: 616c 2069 7320 616e 616c 6f67 2c0d 0a61  al is analog,..a
+00003df0: 6e64 2074 6865 2073 616d 706c 696e 6720  nd the sampling 
+00003e00: 7261 7465 2069 7320 6c69 6d69 7465 6420  rate is limited 
+00003e10: 6279 2074 6865 2062 616e 6477 6964 7468  by the bandwidth
+00003e20: 206f 6620 7468 6520 7369 676e 616c 2e0d   of the signal..
+00003e30: 0a0d 0a0d 0a2e 2e20 6c69 7465 7261 6c69  ....... literali
+00003e40: 6e63 6c75 6465 3a3a 202e 2e2f 7372 7367  nclude:: ../srsg
+00003e50: 7569 2f65 7861 6d70 6c65 732f 6f73 6369  ui/examples/osci
+00003e60: 6c6c 6f73 636f 7065 2065 7861 6d70 6c65  lloscope example
+00003e70: 2f74 6173 6b73 2f66 6966 7468 2e70 790d  /tasks/fifth.py.
+00003e80: 0a20 2020 203a 6c61 6e67 7561 6765 3a20  .    :language: 
+00003e90: 5079 7468 6f6e 0d0a 2020 2020 3a6c 696e  Python..    :lin
+00003ea0: 656e 6f73 3a0d 0a0d 0a0d 0a0d 0a2e 2e20  enos:.......... 
+00003eb0: 5f50 7956 6973 613a 2068 7474 7073 3a2f  _PyVisa: https:/
+00003ec0: 2f70 7976 6973 612e 7265 6164 7468 6564  /pyvisa.readthed
+00003ed0: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00003ee0: 2f0d 0a2e 2e20 5f73 7273 696e 7374 2e73  /.... _srsinst.s
+00003ef0: 7238 3630 3a20 6874 7470 733a 2f2f 7079  r860: https://py
+00003f00: 7069 2e6f 7267 2f70 726f 6a65 6374 2f73  pi.org/project/s
+00003f10: 7273 696e 7374 2e73 7238 3630 2f0d 0a2e  rsinst.sr860/...
+00003f20: 2e20 5f56 5849 3131 3a20 6874 7470 733a  . _VXI11: https:
+00003f30: 2f2f 7777 772e 6c78 6973 7461 6e64 6172  //www.lxistandar
+00003f40: 642e 6f72 672f 4162 6f75 742f 5658 492d  d.org/About/VXI-
+00003f50: 3131 2d61 6e64 2d4c 5849 2e61 7370 780d  11-and-LXI.aspx.
+00003f60: 0a2e 2e20 5f47 5049 423a 2068 7474 7073  ... _GPIB: https
+00003f70: 3a2f 2f65 6e2e 7769 6b69 7065 6469 612e  ://en.wikipedia.
+00003f80: 6f72 672f 7769 6b69 2f49 4545 452d 3438  org/wiki/IEEE-48
+00003f90: 380d 0a2e 2e20 5f55 5342 2d54 4d43 3a20  8.... _USB-TMC: 
+00003fa0: 6874 7470 733a 2f2f 7777 772e 7465 7374  https://www.test
+00003fb0: 616e 646d 6561 7375 7265 6d65 6e74 7469  andmeasurementti
+00003fc0: 7073 2e63 6f6d 2f72 656d 6f74 652d 636f  ps.com/remote-co
+00003fd0: 6d6d 756e 6963 6174 696f 6e2d 7769 7468  mmunication-with
+00003fe0: 2d75 7362 746d 632d 6661 712f 0d0a 2e2e  -usbtmc-faq/....
+00003ff0: 205f 5344 5331 3230 3258 453a 2068 7474   _SDS1202XE: htt
+00004000: 7073 3a2f 2f73 6967 6c65 6e74 6e61 2e63  ps://siglentna.c
+00004010: 6f6d 2f70 726f 6475 6374 2f73 6473 3132  om/product/sds12
+00004020: 3032 782d 652f 0d0a 2e2e 205f 5352 533a  02x-e/.... _SRS:
+00004030: 2068 7474 7073 3a2f 2f74 6869 6e6b 7372   https://thinksr
+00004040: 732e 636f 6d2f 0d0a 2e2e 205f 4347 3633  s.com/.... _CG63
+00004050: 353a 2068 7474 7073 3a2f 2f74 6869 6e6b  5: https://think
+00004060: 7372 732e 636f 6d2f 7072 6f64 7563 7473  srs.com/products
+00004070: 2f63 6736 3335 2e68 746d 6c0d 0a2e 2e20  /cg635.html.... 
+00004080: 5f6c 6f67 6769 6e67 3a20 6874 7470 733a  _logging: https:
+00004090: 2f2f 646f 6373 2e70 7974 686f 6e2e 6f72  //docs.python.or
+000040a0: 672f 332f 686f 7774 6f2f 6c6f 6767 696e  g/3/howto/loggin
+000040b0: 672e 6874 6d6c 0d0a 2e2e 205f 6d61 7470  g.html.... _matp
+000040c0: 6c6f 746c 6962 3a20 6874 7470 733a 2f2f  lotlib: https://
+000040d0: 6d61 7470 6c6f 746c 6962 2e6f 7267 2f73  matplotlib.org/s
+000040e0: 7461 626c 652f 696e 6465 782e 6874 6d6c  table/index.html
```

### Comparing `srsgui-0.4.0.1/docs/index.rst` & `srsgui-0.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/docs/installation.rst` & `srsgui-0.4.1/docs/installation.rst`

 * *Files 6% similar despite different names*

```diff
@@ -13,103 +13,104 @@
 
 .. note::
 
     Commands running from the command prompt shown here are assumed using
     a Windows computer system. If you use other systems, commands may be
     different. Refer to `this page. <install-packages_>`_
 
-If you have a Python older than the required version,
-`install a newer Python. <install-python_>`_
+If your version of Python is older than the required version,
+`install a newer version of Python. <install-python_>`_
 
-Using `virtual environment <virtual-environment_>`_ helps to avoid possible dependency
+Using a `virtual environment <virtual-environment_>`_ helps to avoid possible dependency
 conflicts among Python packages. If you want to use a virtual environment, create one with
 your favorite virtual environment package. If you do not have a preference,
 use Python default ``venv``.
 
 .. code-block::
 
     python -m venv env
-    .\env\Scripts\activate
+    .\venv\Scripts\activate
 
 .. note::
-    Commands to use ``venv`` are different among computer systems. Other than Windows, refer to
-    `this page <venv_>`_.
+    Commands to use ``venv`` are different among computer systems. 
+    For operating systems other than Windows, refer to `this page <venv_>`_.
 
 Srsgui installation
 --------------------
 
 To run ``srsgui`` as a GUI application, install it with [full] option using pip_:
 
 .. code-block::
 
     python -m pip install srsgui[full]
 
-It will install ``srsgui`` package along with
+This will install the ``srsgui`` package along with
 the 3 main packages (pyserial_, matplotlib_ and pyside6_) and their dependencies.
 
 If
 
-    - you plan only to use the instrument driver part of ``srsgui`` package without GUI support,
-    - your system requires to install matplotlib_ or pyside6_ from sources other than pip
-      (Some linux systems do so),
-    - you want to use pyqt5_ or pyside2_ instead of pyside6_ as GUI backend,
-    - you have trouble with the full installation and you want to install dependency manually,
+    - you plan to use the instrument driver part of ``srsgui`` only, without GUI support,
+    - your system requires installation of matplotlib_ or pyside6_ from sources other than pip
+      (Some Linux systems do so),
+    - you want to use pyqt5_ or pyside2_ instead of pyside6_ as GUI backend, or
+    - you have trouble with the full installation and you want to install the dependencies manually,
 
 you can install without the extra [full] option:
 
 .. code-block::
 
     python -m pip install srsgui
 
-It will install ``srsgui`` with pyserial_ only.
+This will install ``srsgui`` with pyserial_ only.
 
 .. note::
-    ``srsgui`` runs with either pyside6_, pyside2_ or pyqt5_ installed as GUI backend.
-    If your system already have pyside2_ or pyqt5_ installed, you do not have to install pyside6_.
+    ``srsgui`` runs with either pyside6_, pyside2_, or pyqt5_ installed as the GUI backend.
+    If your system already has pyside2_ or pyqt5_ installed, you do not have to install pyside6_.
+    To determine if these are installed, you can check the following from a terminal:
 
         python -m pip show pyside2
 
         python -m pip show pyqt5
 
-    will show if pyside2_ or pyqt5_ is installed.
+    
 
 .. note::
     In order to maintain the MIT_ license for your projects or modified ``srsgui``, you have to use
-    pyside6_ or pyside2_. Note that pyqt5_ imposes GPLv3_ license to packages using pyqt5_.
+    pyside6_ or pyside2_. pyqt5_ imposes the GPLv3_ license to any packages using pyqt5_.
 
 Starting srsgui application
 ----------------------------
 
 After ``srsgui`` is installed, you can start ``srsgui`` application from the command prompt.
 
 .. code-block::
 
     srsgui
 
     or
 
     python -m srsgui
 
-``srsgui`` installs a executable script named "srsgui" in Python/Scripts directory.
+``srsgui`` installs an executable script named "srsgui" in the Python/Scripts directory.
 If the directory is included in PATH environment variable, **srsgui** command will work.
 Otherwise, **python -m srsgui** will work regardless of PATH setting.
 
 .. _top-of-initial-screen-capture:
 
 .. figure:: ./_static/initial-screen-capture.png
     :align: center
     :figclass: align-center
 
-If you see the application is open and running, the installation is successful!
+If you see the application is open and running, the installation was successful!
 
 .. note::
-    Instead of seeing the application running, you may get errors, probably ImportError.
-    Carefully look through the exception traceback to find out which package causes the error.
-    When the latest python is installed, some packages may not be installed properly. If the problem
-    is not from ``srsgui`` directly, web search of the problem usually leads to a fix.
+    Instead of seeing the application running, you may get errors (most likely, an `ImportError`).
+    Carefully look through the exception traceback to find out which package caused the error.
+    When the latest version of python is installed, some packages may not be installed properly. 
+    If the problem is not from ``srsgui`` directly, a web search of the problem usually leads to a fix.
 
 
 
 
 .. _install-packages: https://packaging.python.org/en/latest/tutorials/installing-packages/
 .. _install-python: https://www.python.org/
 .. _virtual-environment: https://realpython.com/python-virtual-environments-a-primer/
```

### Comparing `srsgui-0.4.0.1/docs/make.bat` & `srsgui-0.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/docs/srsgui.inst.communications.rst` & `srsgui-0.4.1/docs/srsgui.inst.communications.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/docs/srsgui.inst.rst` & `srsgui-0.4.1/docs/srsgui.inst.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/docs/srsgui.task.rst` & `srsgui-0.4.1/docs/srsgui.task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/docs/srsgui.ui.commandtree.rst` & `srsgui-0.4.1/docs/srsgui.ui.commandtree.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/docs/srsgui.ui.qt.rst` & `srsgui-0.4.1/docs/srsgui.ui.qt.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/docs/srsgui.ui.rst` & `srsgui-0.4.1/docs/srsgui.ui.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/docs/troubleshooting.rst` & `srsgui-0.4.1/docs/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/pyproject.toml` & `srsgui-0.4.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ]
 description = "Framework to run instrument-controlling Python scripts in GUI"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["instrument control", "data acquisition", "data visualization"]
 license = {text = "MIT license"}
 classifiers = [
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Topic :: Scientific/Engineering"
 ]
@@ -28,15 +28,15 @@
 dynamic = ["version"]
 
 [tool.setuptools.dynamic]
 version = {attr = "srsgui.__version__"}
 
 [project.optional-dependencies]
 full = ['matplotlib >= 3.6.2', 'pyside6']
-docs = ['matplotlib', 'pyside6', 'sphinx>=5', 'sphinx-rtd-theme>=1']
+docs = ['matplotlib', 'pyside2', 'sphinx>=5', 'sphinx-rtd-theme>=1']
 
 [project.urls]
 homepage = "https://github.com/thinkSRS/srsgui"
 repository = "https://github.com/thinkSRS/srsgui.git"
 documentation = "https://thinksrs.github.io/srsgui"
 changelog = "https://thinksrs.github.io/srsgui/changelog.html"
```

### Comparing `srsgui-0.4.0.1/srsgui/__init__.py` & `srsgui-0.4.1/srsgui/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,8 +22,8 @@
                         InstLoginFailureError, InstIdError, \
                         InstSetError, InstQueryError, InstIndexError
 
 from srsgui.inst import Interface, SerialInterface, TcpipInterface
 from srsgui.inst.instrument import Instrument
 from srsgui.inst.component import Component
 
-__version__ = "0.4.0.1"  # Global version number
+__version__ = "0.4.1"  # Global version number
```

### Comparing `srsgui-0.4.0.1/srsgui/examples/oscilloscope example/instruments/cg635.py` & `srsgui-0.4.1/srsgui/examples/oscilloscope example/instruments/cg635.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/examples/oscilloscope example/instruments/sds1202.py` & `srsgui-0.4.1/srsgui/examples/oscilloscope example/instruments/sds1202.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig` & `srsgui-0.4.1/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Lines that start with '#' is comment lines
 # Example project for SRSGUI package using an oscilloscope and a function generator
 
 
 # The name is used for the main window title and for the directory name for result data saving
 
-name: Srsgui example project using an oscilloscope and a clock generator
+name: Srsgui Example - Oscilloscope and Clock Generator
 
 
 # Specify Instruments used in the project
 # A line that starts with 'inst' adds an instrument to be used in the project.
 # An instrument is a subclass derived from Instrument class in SRSGUI package
 # The first volumn after 'inst:' is the instrument name used in tasks and main terminal.
 # The second column is the Python module or package that contains the instrument class.
```

### Comparing `srsgui-0.4.0.1/srsgui/examples/oscilloscope example/tasks/fifth.py` & `srsgui-0.4.1/srsgui/examples/oscilloscope example/tasks/fifth.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/examples/oscilloscope example/tasks/first.py` & `srsgui-0.4.1/srsgui/examples/oscilloscope example/tasks/first.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/examples/oscilloscope example/tasks/fourth.py` & `srsgui-0.4.1/srsgui/examples/oscilloscope example/tasks/fourth.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/examples/oscilloscope example/tasks/third.py` & `srsgui-0.4.1/srsgui/examples/oscilloscope example/tasks/third.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/inst/__init__.py` & `srsgui-0.4.1/srsgui/inst/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/inst/commands.py` & `srsgui-0.4.1/srsgui/inst/commands.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/inst/communications/interface.py` & `srsgui-0.4.1/srsgui/inst/communications/interface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/inst/communications/serial_ports.py` & `srsgui-0.4.1/srsgui/inst/communications/serial_ports.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/inst/communications/serialinterface.py` & `srsgui-0.4.1/srsgui/inst/communications/serialinterface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/inst/communications/tcpipinterface.py` & `srsgui-0.4.1/srsgui/inst/communications/tcpipinterface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/inst/component.py` & `srsgui-0.4.1/srsgui/inst/component.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/inst/exceptions.py` & `srsgui-0.4.1/srsgui/inst/exceptions.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/inst/indexcommands.py` & `srsgui-0.4.1/srsgui/inst/indexcommands.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/inst/instrument.py` & `srsgui-0.4.1/srsgui/inst/instrument.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/task/callbacks.py` & `srsgui-0.4.1/srsgui/task/callbacks.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,25 +6,34 @@
 import logging
 from matplotlib.figure import Figure
 
 logger = logging.getLogger(__file__)
 
 
 class Callbacks:
-
+    """
+    Base callbacks used by :class:`Task <srsgui.task.task.Task>` class.
+    The parent of Task should subclass Callbacks class, override callback methods that it will use
+    and call set_callback_handler() to make it available to the Task subclass.
+    """
     def started(self):
+
         logger.info('Task started')
 
     def finished(self):
         logger.info('Task finished')
 
     def text_available(self, text: str):
+
         print(text)
 
     def parameter_changed(self):
+        """
+        Override to do something when a parameter in input_parameters is changed
+        """
         logger.info('Task.InputParameters changed')
 
     def figure_update_requested(self, fig: Figure):
         fig.canvas.draw_idle()
 
     def data_available(self, data: dict):
         logger.info('data available')
```

### Comparing `srsgui-0.4.0.1/srsgui/task/config.py` & `srsgui-0.4.1/srsgui/task/config.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/task/inputs.py` & `srsgui-0.4.1/srsgui/task/inputs.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/task/sessionhandler.py` & `srsgui-0.4.1/srsgui/task/sessionhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/task/task.py` & `srsgui-0.4.1/srsgui/task/task.py`

 * *Files 5% similar despite different names*

```diff
@@ -336,15 +336,15 @@
         else:
             self.figure = None
             raise ValueError('No figure in figure_dict to set as default')
 
     def get_figure(self, name=None) -> Figure:
         """
         Get a Matplotlib figure from figure_dict.
-        if name is None, it will reutrn the first figure in figure_dict as the defualt
+        if name is None, it will return the first figure in figure_dict as the default.
         """
 
         if name is None:
             name = list(self.figure_dict.keys())[0]
         if name in self.figure_dict:
             return self.figure_dict[name]
         raise KeyError('Invalid figure name: {}'.format(name))
@@ -384,63 +384,123 @@
         """
         Mark Task is stopped with an error
         """
         self._error_raised = True
 
     # Wrapper for TaskResult.add_details
     def add_details(self, msg: str, key='summary'):
+        """
+        Add msg to :class:`TaskResult <srsgui.task.task.taskresult.TaskResult>` with key.
+        Also display it on the Result panel.
+        """
         self.result.add_details(msg, key)
         self.display_result('{}: {}'.format(key, msg))
 
     # Wrapper for TaskResult.create_table
     def create_table(self, name: str, *args):
+        """
+        Create a table with name in :class:`TaskResult <srsgui.task.task.taskresult.TaskResult>`
+
+        Parameters
+        -----------
+            name: str
+                name of the table
+            args
+                horizontal header for the table.
+                The length of args defines the number of table columns
+        """
         self.result.create_table(name, *args)
 
     # Wrapper for TaskResult.add_data_to_table
     def add_data_to_table(self, name: str, *args, ):
+        """
+        Add args into the table with name
+
+        Parameters
+        -----------
+            name: str
+                the name of the table into which data are added
+            args
+                A row of data
+                The length of args should match with the number of columns in the table
+        """
         self.result.add_data_to_table(name, *args)
 
     # The file for raw data is created by SessionHandler automatically.
     # You can sequentially add data to the table until you create another new table.
-    # TaskResult is attached to the file in the last before closed.
+    # TaskResult is attached to the enf og the file when closed.
 
     def create_table_in_file(self, name, *args):
+        """
+        Create a table only saved outside :class:`TaskResult <srsgui.task.task.taskresult.TaskResult>` class.
+
+        When a table will get big, use this instead of :meth:`create_table <srsgui.task.task.Task.create_table>`.
+
+        Parameters
+        -----------
+            name: str
+                name of the table
+            args
+                horizontal header for the table.
+                The length of args defines the number of table columns
+        """
         if self.session_handler is None:
             raise AttributeError("No session handler available")
         self.session_handler.create_table_in_file(name, *args)
 
-    def add_to_table_in_file(self, *args, format_list=None):
+    def add_to_table_in_file(self, name, *args, format_list=None):
+        """
+        Add args into the table with name
+
+        Parameters
+        -----------
+            name: str
+                the name of the table into which data are added
+            args
+                A row of data
+                The length of args should match with the number of columns in the table
+            format_list: tuple
+                optional format for args
+        """
+
         if self.session_handler is None:
             raise AttributeError("No session handler available")
-        self.session_handler.add_to_table_in_file(*args, format_list=format_list)
+        self.session_handler.add_to_table_in_file(name, *args, format_list=format_list)
 
     def add_dict_to_file(self, name, data_dict):
         """
         Add a dictionary to the file.
         """
         if self.session_handler is None:
             raise AttributeError("No session handler available")
         self.session_handler.add_dict_to_file(name, data_dict)
 
     def save_result(self, msg):
-        self.logger.error('Do not use save_result. Use add_to_table_in_file, or result.add_details, instead.')
+        """
+        Deprecated. Use add_details instead
+        """
+        self.logger.error('Do not use save_result. Use add_details or add_to_table_in_file instead.')
         # raise NotImplementedError()
 
     def round_float(self, number):
-        # set the resolution of the number with self.round_float_resolution
+        """
+        Round a float number with a resolution
+
+        Set the resolution of the number with self.round_float_resolution
+        """
         fmt = '{{:.{}e}}'.format(self.round_float_resolution)
         return float(fmt.format(number))
 
     # Following methods will be used with stdout redirection
     def update_status(self, message):
         """ Output to the status bar at the bottom of srsgui application"""
         self.write_text(self.EscapeForStatus + message)
 
     def display_device_info(self, message='', device_name=None, update=False,  clear=False):
-        """output to device info windows
+        """output to the Device Info panel
         """
         if update:
             if device_name:
                 self.write_text('{}{}:update'.format(self.EscapeForDevice, device_name))
             else:
                 name = list(self.inst_dict.keys())[0]
                 self.write_text('{}{}:update'.format(self.EscapeForDevice, name))
@@ -454,30 +514,32 @@
 
         if device_name:
             self.write_text('{}{}:{}'.format(self.EscapeForDevice, device_name, message))
         else:
             self.write_text('{}{}'.format(self.EscapeForDevice, message))
 
     def display_result(self, message, clear=False):
-        """ output to the result window
+        """ output to the Result panel
         """
         if clear:
             self.write_text('{}cls'.format(self.EscapeForResult))
         self.write_text('{}{}'.format(self.EscapeForResult, message))
 
     def _notify_start(self):
         self.write_text(self.EscapeForStart + self.name)
         self.update_status(self.name + ' running')
 
     def _notify_finish(self):
         self.write_text(self.EscapeForStop + self.name)
         self.update_status(self.name + ' stopped')
 
-    # output text to UI
     def write_text(self, text):
+        """
+        Base method to send output text to UI
+        """
         self.callbacks.text_available(str(text))
 
     def get_input_parameter(self, name):
         """
         Get the parameter value in input_parameters
 
         Parameters
@@ -537,25 +599,36 @@
     def notify_parameter_changed(self):
         """
         Notify UI that there are changes in input_parameters for display update
         """
         self.callbacks.parameter_changed()
 
     def request_figure_update(self, figure=None):
+        """
+        It requests the parent of the task to update the figure,
+        if the callback is set up properly.
+        """
         if type(figure) is not Figure:
             figure = self.figure
         self.callbacks.figure_update_requested(figure)
 
     def update_figure(self, figure: Figure):
+        """
+        Deprecated. Use request_figure_update instead.
+        """
         if type(figure) is not Figure:
             raise TypeError('{} is not  a Figure'.format(type(figure)))
         self.callbacks.figure_update_requested(figure)
 
-    # It needs a matching update() as a slot to run from UI
     def notify_data_available(self, data={}):
+        """
+        It needs a matching update() defined in the task class that will be run by the parent.
+        It is used to run both data processing and figure_update from the parent thread
+        to prevent a race condition between them.
+        """
         self.callbacks.data_available(data)
 
     def update(self, data: dict):
         """
         when notify_data_available is called, this method handles data processing
         and display update. By default, it does no data handling, but figure update request.
         GUI related data processing needs to be done here to be handled
```

### Comparing `srsgui-0.4.0.1/srsgui/task/taskresult.py` & `srsgui-0.4.1/srsgui/task/taskresult.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/ui/commandhandler.py` & `srsgui-0.4.1/srsgui/ui/commandhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/ui/commandterminal.py` & `srsgui-0.4.1/srsgui/ui/commandterminal.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/ui/commandtree/commanddelegate.py` & `srsgui-0.4.1/srsgui/ui/commandtree/commanddelegate.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/ui/commandtree/commandhandler.py` & `srsgui-0.4.1/srsgui/ui/commandtree/commandhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/ui/commandtree/commanditem.py` & `srsgui-0.4.1/srsgui/ui/commandtree/commanditem.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/ui/commandtree/commandmodel.py` & `srsgui-0.4.1/srsgui/ui/commandtree/commandmodel.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/ui/commandtree/commandspinbox.py` & `srsgui-0.4.1/srsgui/ui/commandtree/commandspinbox.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/ui/commandtree/commandtreeview.py` & `srsgui-0.4.1/srsgui/ui/commandtree/commandtreeview.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/ui/commandtree/commandtreewidget.py` & `srsgui-0.4.1/srsgui/ui/commandtree/commandtreewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/ui/commandtree/ui_commandtreewidget.py` & `srsgui-0.4.1/srsgui/ui/commandtree/ui_commandtreewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/ui/connectdlg.py` & `srsgui-0.4.1/srsgui/ui/connectdlg.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 class ConnectDlg(QDialog):
     """
     * To build the connection dialog box based on *available_interface* of subclasses of
       :class:`srsgui.inst.instrument.Instrument` class listed in the current .taskconfig file.
 
     * To connect to the selected interface of the instrument.
-
     """
 
     def __init__(self, inst, parent=None):
         super().__init__(parent)
 
         self.inst = inst
         self.parent = parent
```

### Comparing `srsgui-0.4.0.1/srsgui/ui/deviceinfohandler.py` & `srsgui-0.4.1/srsgui/ui/deviceinfohandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/ui/dockhandler.py` & `srsgui-0.4.1/srsgui/ui/dockhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/ui/inputpanel.py` & `srsgui-0.4.1/srsgui/ui/inputpanel.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/ui/qt/QtCore.py` & `srsgui-0.4.1/srsgui/ui/qt/QtCore.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/ui/qt/QtGui.py` & `srsgui-0.4.1/srsgui/ui/qt/QtGui.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/ui/qt/QtWidgets.py` & `srsgui-0.4.1/srsgui/ui/qt/QtWidgets.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/ui/qt/__init__.py` & `srsgui-0.4.1/srsgui/ui/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/ui/qtloghandler.py` & `srsgui-0.4.1/srsgui/ui/qtloghandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/ui/resource_rc.py` & `srsgui-0.4.1/srsgui/ui/resource_rc.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/ui/signalhandler.py` & `srsgui-0.4.1/srsgui/ui/signalhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/ui/srslogo.jpg` & `srsgui-0.4.1/srsgui/ui/srslogo.jpg`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/ui/stdout.py` & `srsgui-0.4.1/srsgui/ui/stdout.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/ui/taskmain.py` & `srsgui-0.4.1/srsgui/ui/taskmain.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/ui/taskmain.ui` & `srsgui-0.4.1/srsgui/ui/taskmain.ui`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui/ui/ui_taskmain.py` & `srsgui-0.4.1/srsgui/ui/ui_taskmain.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0.1/srsgui.egg-info/PKG-INFO` & `srsgui-0.4.1/srsgui.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.4.0.1
+Version: 0.4.1
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Project-URL: homepage, https://github.com/thinkSRS/srsgui
 Project-URL: repository, https://github.com/thinkSRS/srsgui.git
 Project-URL: documentation, https://thinksrs.github.io/srsgui
 Project-URL: changelog, https://thinksrs.github.io/srsgui/changelog.html
 Keywords: instrument control,data acquisition,data visualization
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
@@ -23,74 +23,69 @@
 License-File: LICENSE.txt
 
 # ``Srsgui`` - Organize instrument-controlling Python scripts as a GUI application
 
 `Srsgui` is a simple framework:
 
    - To define instrument classes for instruments that use remote communication,
-     based on `Instrument` class and the communication `Interface` class 
-     (By default, serial and TCPIP is available. VXI11, GPIB and USB-TMC are optional.).
+     based on the `Instrument` class and the communication `Interface` class. 
+     (By default, serial and TCPIP is available. VXI11, GPIB and USB-TMC are optional).
 
    - To write Python scripts (tasks) that run in GUI environment with simple APIs
      provided in ``Task`` class.
 
    - To organize instrument classes and task scripts presented in a GUI application
-     using a configuration (.taskconfig) file for a project
+     using a configuration (.taskconfig) file for a project.
 
 ![screenshot](https://thinksrs.github.io/srsgui/_images/example-screen-capture-2.png " ")
 
 ## Installation
 
 To run ``srsgui`` as an application, create a virtual environment, if necessary, 
-and install using ``pip`` with [full] option:  
+and install using ``pip`` with the `[full]` option:  
 
     python -m pip install srsgui[full]
 
 ``Srsgui`` package has the following 3 main dependencies: 
 [pyserial](https://pypi.org/project/pyserial/), 
 [matplotlib](https://pypi.org/project/matplotlib/) and
 [PySide6](https://pypi.org/project/PySide6/). If the installation above fails, 
 you have to install the failed pacakge manually. Using a virtual environment will
 eliminate possible conflicts between packages in the main Python installation and 
-the packagesSome used in `srsgui`. Some Linux distributions offer 
-some of the Python packages from their repositories only, not from ``pip``. 
-Run web search for more information on system-specific installation.   
-
-Once pyserial, matplotlib and PySide6 are installed properly, or you plan to use
-`srsgui` for instrument drivers only without GUI support, 
-you can install ``srsgui`` without [full] option:
+the packages. Some Linux distributions offer certain Python packages from their repositories only (i.e. not from ``pip``). 
+Run a web search for more information on system-specific installation.   
+
+Once pyserial, matplotlib and PySide6 are installed properly, or if you plan to use `srsgui` for instrument drivers only without GUI support, 
+you can install ``srsgui`` without the `[full]` option:
 
     python -m pip install srsgui
 
 ## Start ``srsgui`` application
     
-if the Python Script directory is in PATH environment variable,
-Start the application by typing from the command line:
+If the Python Script directory is in the PATH environment variable,
+launch the application by typing the module name into the command line:
 
     srsgui
 
 If the script directory is not in PATH, run the srsgui module with Python. 
 
     python -m srsgui
-    
-It will start `srsgui` application.
+
 
 ## Run the example project
 
-By default, `srsgui` application starts with the last project it ran,
-when it is closed.
+By default, the `srsgui` application starts with the project that was running when it was last closed.
  
-To open the example project included in the `srsgui` package 
-(if `srsgui` does not start with the example project), select the menu/File/Open config, 
-go to the `srsgui` package directory, find the examples directory, and find a .taskconfig file
+To open the **oscilloscope example project** included in the `srsgui` package 
+(if `srsgui` does not start with the example project), select File/Open config, 
+go to the `srsgui` package directory, find the examples directory, and select the `oscilloscope example project.taskconfig` file
 in the example project folder. 
 
-You can run the second and fifth task in the Task menu 
-even without any instruments connected.
+You can run the **Plot example** and **FFT of simulated waveform** tasks from the Task menu without any instruments connected.
 
 ## Create a project
 
-`Srsgui` is a framework to helps you to write your own instrument-controlling 
-Python scripts running as a GUI application. Using its APIs, you can write 
-scripts running in GUI with the same amount of code with writing console-based 
-scripts. For programming API, refer to
+`Srsgui` is a framework to help you to write your own instrument-controlling 
+Python scripts and run them from a GUI application. Using its APIs, you can write 
+scripts running in GUI with the same amount of code as writing console-based 
+scripts. For programming using the API, refer to the
 [`srsgui` documentation](https://thinksrs.github.io/srsgui).
```

### Comparing `srsgui-0.4.0.1/srsgui.egg-info/SOURCES.txt` & `srsgui-0.4.1/srsgui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

