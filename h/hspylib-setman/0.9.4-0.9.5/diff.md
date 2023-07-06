# Comparing `tmp/hspylib-setman-0.9.4.tar.gz` & `tmp/hspylib-setman-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-setman-0.9.4.tar", last modified: Thu Jul  6 19:17:41 2023, max compression
+gzip compressed data, was "hspylib-setman-0.9.5.tar", last modified: Thu Jul  6 19:42:03 2023, max compression
```

## Comparing `hspylib-setman-0.9.4.tar` & `hspylib-setman-0.9.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 19:17:41.893121 hspylib-setman-0.9.4/
--rw-r--r--   0 hjunior    (504) staff       (20)       51 2023-07-06 16:29:29.000000 hspylib-setman-0.9.4/MANIFEST.in
--rw-r--r--   0 hjunior    (504) staff       (20)     1675 2023-07-06 19:17:41.891800 hspylib-setman-0.9.4/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      672 2023-07-06 19:17:40.000000 hspylib-setman-0.9.4/README.md
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 19:17:41.854638 hspylib-setman-0.9.4/hspylib_setman.egg-info/
--rw-r--r--   0 hjunior    (504) staff       (20)     1675 2023-07-06 19:17:41.000000 hspylib-setman-0.9.4/hspylib_setman.egg-info/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      619 2023-07-06 19:17:41.000000 hspylib-setman-0.9.4/hspylib_setman.egg-info/SOURCES.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-07-06 19:17:41.000000 hspylib-setman-0.9.4/hspylib_setman.egg-info/dependency_links.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       41 2023-07-06 19:17:41.000000 hspylib-setman-0.9.4/hspylib_setman.egg-info/requires.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        7 2023-07-06 19:17:41.000000 hspylib-setman-0.9.4/hspylib_setman.egg-info/top_level.txt
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 19:17:41.862378 hspylib-setman-0.9.4/setman/
--rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-07-06 19:17:40.000000 hspylib-setman-0.9.4/setman/.version
--rw-r--r--   0 hjunior    (504) staff       (20)      718 2023-07-05 21:55:00.000000 hspylib-setman-0.9.4/setman/__classpath__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      166 2023-07-06 19:17:40.000000 hspylib-setman-0.9.4/setman/__init__.py
--rwxr-xr-x   0 hjunior    (504) staff       (20)     4786 2023-07-06 18:54:15.000000 hspylib-setman-0.9.4/setman/__main__.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 19:17:41.870244 hspylib-setman-0.9.4/setman/core/
--rw-r--r--   0 hjunior    (504) staff       (20)      197 2023-07-06 19:17:40.000000 hspylib-setman-0.9.4/setman/core/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     7211 2023-07-06 19:09:18.000000 hspylib-setman-0.9.4/setman/core/setman.py
--rw-r--r--   0 hjunior    (504) staff       (20)      823 2023-07-05 22:10:34.000000 hspylib-setman-0.9.4/setman/core/setman_config.py
--rw-r--r--   0 hjunior    (504) staff       (20)     1406 2023-07-05 22:27:05.000000 hspylib-setman-0.9.4/setman/core/setman_enums.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 19:17:41.888485 hspylib-setman-0.9.4/setman/settings/
--rw-r--r--   0 hjunior    (504) staff       (20)      256 2023-07-06 19:17:40.000000 hspylib-setman-0.9.4/setman/settings/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     9400 2023-07-06 19:14:49.000000 hspylib-setman-0.9.4/setman/settings/settings.py
--rw-r--r--   0 hjunior    (504) staff       (20)     1404 2023-07-05 17:37:53.000000 hspylib-setman-0.9.4/setman/settings/settings_config.py
--rw-r--r--   0 hjunior    (504) staff       (20)     3446 2023-07-05 22:08:41.000000 hspylib-setman-0.9.4/setman/settings/settings_entry.py
--rw-r--r--   0 hjunior    (504) staff       (20)     3887 2023-07-05 22:08:56.000000 hspylib-setman-0.9.4/setman/settings/settings_repository.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2054 2023-07-05 22:30:45.000000 hspylib-setman-0.9.4/setman/settings/settings_service.py
--rw-r--r--   0 hjunior    (504) staff       (20)      256 2023-07-05 22:41:51.000000 hspylib-setman-0.9.4/setman/welcome.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-07-06 19:17:41.893305 hspylib-setman-0.9.4/setup.cfg
--rw-r--r--   0 hjunior    (504) staff       (20)     2067 2023-07-05 21:51:13.000000 hspylib-setman-0.9.4/setup.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 19:42:03.352883 hspylib-setman-0.9.5/
+-rw-r--r--   0 hjunior    (504) staff       (20)       51 2023-07-06 16:29:29.000000 hspylib-setman-0.9.5/MANIFEST.in
+-rw-r--r--   0 hjunior    (504) staff       (20)     1675 2023-07-06 19:42:03.351851 hspylib-setman-0.9.5/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      672 2023-07-06 19:42:02.000000 hspylib-setman-0.9.5/README.md
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 19:42:03.308306 hspylib-setman-0.9.5/hspylib_setman.egg-info/
+-rw-r--r--   0 hjunior    (504) staff       (20)     1675 2023-07-06 19:42:03.000000 hspylib-setman-0.9.5/hspylib_setman.egg-info/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      619 2023-07-06 19:42:03.000000 hspylib-setman-0.9.5/hspylib_setman.egg-info/SOURCES.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-07-06 19:42:03.000000 hspylib-setman-0.9.5/hspylib_setman.egg-info/dependency_links.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       41 2023-07-06 19:42:03.000000 hspylib-setman-0.9.5/hspylib_setman.egg-info/requires.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        7 2023-07-06 19:42:03.000000 hspylib-setman-0.9.5/hspylib_setman.egg-info/top_level.txt
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 19:42:03.317112 hspylib-setman-0.9.5/setman/
+-rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-07-06 19:42:02.000000 hspylib-setman-0.9.5/setman/.version
+-rw-r--r--   0 hjunior    (504) staff       (20)      718 2023-07-05 21:55:00.000000 hspylib-setman-0.9.5/setman/__classpath__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      166 2023-07-06 19:42:02.000000 hspylib-setman-0.9.5/setman/__init__.py
+-rwxr-xr-x   0 hjunior    (504) staff       (20)     4903 2023-07-06 19:32:56.000000 hspylib-setman-0.9.5/setman/__main__.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 19:42:03.332239 hspylib-setman-0.9.5/setman/core/
+-rw-r--r--   0 hjunior    (504) staff       (20)      197 2023-07-06 19:42:02.000000 hspylib-setman-0.9.5/setman/core/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     7682 2023-07-06 19:39:52.000000 hspylib-setman-0.9.5/setman/core/setman.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      823 2023-07-05 22:10:34.000000 hspylib-setman-0.9.5/setman/core/setman_config.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     1406 2023-07-05 22:27:05.000000 hspylib-setman-0.9.5/setman/core/setman_enums.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 19:42:03.350606 hspylib-setman-0.9.5/setman/settings/
+-rw-r--r--   0 hjunior    (504) staff       (20)      256 2023-07-06 19:42:02.000000 hspylib-setman-0.9.5/setman/settings/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     9772 2023-07-06 19:29:15.000000 hspylib-setman-0.9.5/setman/settings/settings.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     1404 2023-07-05 17:37:53.000000 hspylib-setman-0.9.5/setman/settings/settings_config.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     3446 2023-07-05 22:08:41.000000 hspylib-setman-0.9.5/setman/settings/settings_entry.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     4135 2023-07-06 19:23:54.000000 hspylib-setman-0.9.5/setman/settings/settings_repository.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2154 2023-07-06 19:24:40.000000 hspylib-setman-0.9.5/setman/settings/settings_service.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      256 2023-07-05 22:41:51.000000 hspylib-setman-0.9.5/setman/welcome.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-07-06 19:42:03.353009 hspylib-setman-0.9.5/setup.cfg
+-rw-r--r--   0 hjunior    (504) staff       (20)     2067 2023-07-05 21:51:13.000000 hspylib-setman-0.9.5/setup.py
```

### Comparing `hspylib-setman-0.9.4/PKG-INFO` & `hspylib-setman-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-setman
-Version: 0.9.4
+Version: 0.9.5
 Summary: HsPyLib - Settings Manager
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-setman/
@@ -26,12 +26,12 @@
 Description-Content-Type: text/markdown
 
 # HsPyLib - Settings Manager
 
 ## Manage your terminal settings
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.4/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.5/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-setman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-setman-0.9.4/README.md` & `hspylib-setman-0.9.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # HsPyLib - Settings Manager
 
 ## Manage your terminal settings
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.4/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.5/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-setman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-setman-0.9.4/hspylib_setman.egg-info/PKG-INFO` & `hspylib-setman-0.9.5/hspylib_setman.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-setman
-Version: 0.9.4
+Version: 0.9.5
 Summary: HsPyLib - Settings Manager
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-setman/
@@ -26,12 +26,12 @@
 Description-Content-Type: text/markdown
 
 # HsPyLib - Settings Manager
 
 ## Manage your terminal settings
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.4/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.5/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-setman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-setman-0.9.4/hspylib_setman.egg-info/SOURCES.txt` & `hspylib-setman-0.9.5/hspylib_setman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.4/setman/__classpath__.py` & `hspylib-setman-0.9.5/setman/__classpath__.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.4/setman/__main__.py` & `hspylib-setman-0.9.5/setman/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
                 .add_option('name', 'n', 'name', 'filter settings matching name.') \
                 .add_option('type', 't', 'type', 'filter settings matching type.', choices=SettingsType.choices()) \
             .argument(SetmanOps.SEARCH.val, 'Search and display all settings matching criteria.') \
                 .add_option('name', 'n', 'name', 'filter settings matching name.') \
                 .add_option('type', 't', 'type', 'filter settings matching type.', choices=SettingsType.choices()) \
             .argument(SetmanOps.TRUNCATE.val, 'Clear all settings matching name.') \
                 .add_option('name', 'n', 'name', 'filter settings matching name.') \
+                .add_option('type', 't', 'type', 'filter settings matching type.', choices=SettingsType.choices()) \
             .argument(SetmanOps.IMPORT.val, 'Import settings from a CSV formatted file.') \
                 .add_parameter('file', 'the path of the CSV file to be imported.') \
             .argument(SetmanOps.EXPORT.val, 'Export settings to a CSV formatted file.') \
                 .add_parameter('file', 'the path of the CSV file to be exported.') \
                 .add_option('name', 'n', 'name', 'filter settings matching name.') \
                 .add_option('type', 't', 'type', 'filter settings matching type.', choices=SettingsType.choices())
         # fmt: on
```

### Comparing `hspylib-setman-0.9.4/setman/core/setman.py` & `hspylib-setman-0.9.5/setman/core/setman.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,25 +13,24 @@
    Copyright 2023, HsPyLib team
 """
 import atexit
 import logging as log
 import os
 from typing import Any
 
+from clitt.core.tui.table.table_enums import TextAlignment
+from clitt.core.tui.table.table_renderer import TableRenderer
 from hspylib.core.enums.charset import Charset
 from hspylib.core.exception.exceptions import InvalidArgumentError
 from hspylib.core.metaclass.singleton import Singleton
 from hspylib.core.preconditions import check_state
 from hspylib.core.tools.commons import file_is_not_empty, syserr, sysout
 from hspylib.modules.application.application import Application
 from hspylib.modules.cli.keyboard import Keyboard
 
-from clitt.core.tui.table.table_enums import TextAlignment
-from clitt.core.tui.table.table_renderer import TableRenderer
-
 from setman.core.setman_config import SetmanConfig
 from setman.core.setman_enums import SetmanOps, SettingsType
 from setman.settings.settings import Settings
 
 
 class Setman(metaclass=Singleton):
     """HsPyLib application that helps managing system settings."""
@@ -89,24 +88,28 @@
                 case SetmanOps.SET:
                     self._set_setting(name, value, stype)
                 case SetmanOps.GET:
                     self._get_setting(name, simple_fmt)
                 case SetmanOps.DEL:
                     self._del_setting(name)
                 case SetmanOps.TRUNCATE:
-                    self._clear_settings(name)
+                    self._clear_settings(name, stype)
                 case SetmanOps.IMPORT:
                     self._import_settings(filepath)
                 case SetmanOps.EXPORT:
                     self._export_settings(filepath, name, stype)
                 case _:
                     raise InvalidArgumentError(f"Operation not supported: {operation}")
 
     def _set_setting(self, name: str | None, value: Any | None, stype: SettingsType | None) -> None:
-        """Upsert the specified setting."""
+        """Upsert the specified setting.
+        :param name: the settings name.
+        :param value: the settings value.
+        :param stype: the settings type.
+        """
         found, entry = self.settings.upsert(name, value, stype)
         sysout(f"%GREEN%Settings {'added' if not found else 'saved'}: %WHITE%", entry, "%EOL%")
 
     def _get_setting(self, name: str, simple_fmt: bool = False) -> None:
         """Get setting matching the specified name.
         :param name: the settings name to get.
         :param simple_fmt: whether to format the setting or not.
@@ -122,44 +125,51 @@
         """
         if found := self.settings.remove(name):
             sysout("%GREEN%Setting deleted: %WHITE%", found, "%EOL%")
         else:
             syserr("%EOL%%YELLOW%No settings found matching: %WHITE%", name, "%EOL%")
 
     def _list_settings(self, name: str | None, stype: SettingsType | None) -> None:
-        """List in a table all settings matching criteria."""
+        """List in a table all settings matching criteria.
+        :param name: the settings name to filter.
+        :param stype: the settings type to filter.
+        """
         data = list(map(lambda s: s.values, self.settings.search(name, stype)))
         tr = TableRenderer(self.settings.HEADERS, data, "Systems Settings")
         tr.adjust_auto_fit()
         tr.set_header_alignment(TextAlignment.CENTER)
         tr.set_cell_alignment(TextAlignment.LEFT)
         tr.render()
 
     def _search_settings(self, name: str | None, stype: SettingsType | None, simple_fmt: bool) -> None:
-        """Search and display all settings matching criteria."""
+        """Search and display all settings matching criteria.
+        :param name: the settings name to filter.
+        :param stype: the settings type to filter.
+        :param simple_fmt: whether to display simple or formatted.
+        """
         data = list(map(lambda e: e.to_string(simple_fmt), self.settings.search(name, stype)))
         sysout(os.linesep.join(data)) \
             if data \
             else sysout(
-            f"%EOL%%YELLOW%No settings found matching: %WHITE%[name={name.replace('%', '*')}, stype={stype}] %EOL%"
-        )
+            f"%EOL%%YELLOW%No settings found matching: "
+            f"%WHITE%[name={name}, stype={stype}] %EOL%")
 
-    def _clear_settings(self, name: str | None) -> None:
+    def _clear_settings(self, name: str | None, stype: SettingsType | None) -> None:
         """Clear all settings.
         :param name: clear settings matching name.
         """
-        if not name:
+        if not name and not stype:
             sysout("%EOL%%ORANGE%All settings will be removed. Are you sure (y/[n])? ")
-            keystroke = Keyboard.wait_keystroke()
-            if keystroke and keystroke in [Keyboard.VK_y, Keyboard.VK_Y]:
-                self.settings.clear("*")
-                sysout("%EOL%%ORANGE%!!! All system settings have been removed !!!%EOL%")
+            if (keystroke := Keyboard.wait_keystroke()) and keystroke in [Keyboard.VK_y, Keyboard.VK_Y]:
+                self.settings.clear("*", stype)
+                sysout("%EOL%%ORANGE%!!! All settings have been removed !!!%EOL%")
         else:
-            self.settings.clear(name)
-            sysout(f"%EOL%%ORANGE%!!! System settings matching [{name}] have been removed !!!%EOL%")
+            self.settings.clear(name, stype)
+            sysout(f"%EOL%%ORANGE%Removed settings matching: "
+                   f"%WHITE%[name={name}, stype={stype}] %EOL%")
 
     def _import_settings(self, filepath: str) -> None:
         """Import settings from CSV file."""
         count = self.settings.import_csv(filepath)
         sysout(f"%EOL%%GREEN%Imported {count} settings from {filepath}! %EOL%")
 
     def _export_settings(self, filepath: str, name: str | None = None, stype: SettingsType | None = None) -> None:
```

### Comparing `hspylib-setman-0.9.4/setman/core/setman_config.py` & `hspylib-setman-0.9.5/setman/core/setman_config.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.4/setman/core/setman_enums.py` & `hspylib-setman-0.9.5/setman/core/setman_enums.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.4/setman/settings/settings.py` & `hspylib-setman-0.9.5/setman/settings/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -136,26 +136,26 @@
         check_state(self.is_open, "Settings database is not open")
         if name:
             return self._service.get(name)
         return None
 
     def upsert(
         self,
-        name: str,
-        value: Any,
-        stype: SettingsType) -> Tuple[Optional[SettingsEntry], Optional[SettingsEntry]]:
+        name: str | None = None,
+        value: Any | None = None,
+        stype: SettingsType | None = None) -> Tuple[Optional[SettingsEntry], Optional[SettingsEntry]]:
         """Upsert the specified setting.
         :param name: the settings name.
         :param value: the settings value.
         :param stype: the settings type.
         """
         check_state(self.is_open, "Settings database is not open")
         found = self._service.get(name)
         entry = found or SettingsEntry(Identity(SettingsEntry.SetmanId(uuid.uuid4().hex)), name, value, stype)
-        if not name or value is None or not stype:
+        if not name or not value or not stype:
             entry = SettingsEntry.prompt(entry)
         if entry:
             entry.modified = now()
             self._service.save(entry)
             self._clear_caches()
         return found, entry
 
@@ -169,26 +169,29 @@
             if found:
                 self._service.remove(found)
                 self._clear_caches()
                 return found
         return None
 
     @lru_cache(maxsize=500)
-    def search(self, name: str = None, stype: SettingsType = None) -> List[SettingsEntry]:
-        """Display all settings matching the name and settings type.
-        :param name: the setting name to get.
+    def search(self, name: str | None = None, stype: SettingsType | None = None) -> List[SettingsEntry]:
+        """Search all settings matching criteria.
+        :param name: the settings name to filter.
         :param stype: the settings type to filter.
         """
         check_state(self.is_open, "Settings database is not open")
         return self._service.search(name, stype, self.limit, self.offset)
 
-    def clear(self, name: str = None) -> None:
-        """Clear all settings from the settings table."""
+    def clear(self, name: str | None = None, stype: SettingsType | None = None) -> None:
+        """Clear all settings from the settings table.
+        :param name: the settings name to filter.
+        :param stype: the settings type to filter.
+        """
         check_state(self.is_open, "Settings database is not open")
-        self._service.clear(name)
+        self._service.clear(name, stype)
         self._clear_caches()
 
     def import_csv(self, filepath: str) -> int:
         """Upsert settings from CSV file into the database.
         :param filepath: the path of the CSV file to be imported.
         """
         count, csv_file = 0, ensure_endswith(filepath, ".csv")
@@ -202,15 +205,19 @@
                 entry = SettingsEntry(Identity(SettingsEntry.SetmanId(uid)), name, value, stype)
                 self._service.save(entry)
                 count += 1
             self._clear_caches()
             return count
 
     def export_csv(self, filepath: str, name: str = None, stype: SettingsType = None) -> int:
-        """Export settings from CSV file into the database."""
+        """Export settings from CSV file into the database.
+        :param filepath: the path of the CSV file to be exported.
+        :param name: the settings name to filter.
+        :param stype: the settings type to filter.
+        """
         dest_dir, csv_file = dirname(filepath), ensure_endswith(filepath, ".csv")
         check_argument(os.path.exists(dest_dir), "Destination dir does not exist: " + dest_dir)
         settings = self.search(name, stype)
         with open(csv_file, "w", encoding="UTF8") as f_csv:
             writer = csv.writer(f_csv, delimiter=',')
             writer.writerow(self.HEADERS)
             writer.writerows(list(map(lambda s: s.values, settings)))
```

### Comparing `hspylib-setman-0.9.4/setman/settings/settings_config.py` & `hspylib-setman-0.9.5/setman/settings/settings_config.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.4/setman/settings/settings_entry.py` & `hspylib-setman-0.9.5/setman/settings/settings_entry.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.4/setman/settings/settings_repository.py` & `hspylib-setman-0.9.5/setman/settings/settings_repository.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,34 +33,38 @@
         sql = f"SELECT * FROM SETTINGS WHERE name = ? ORDER BY name"
         result = next((e for e in self.execute(sql, name=name)[1]), None)
 
         return self.to_entity_type(result) if result else None
 
     def search(
         self,
-        name: str = None,
-        stype: SettingsType = None,
+        name: str | None = None,
+        stype: SettingsType | None = None,
         limit: int = 500,
         offset: int = 0) -> List[SettingsEntry]:
         """Search settings by settings type."""
         search_name = name.replace("*", "%") if name else "%"
         if stype:
             sql = f"SELECT * FROM SETTINGS WHERE name LIKE ? AND stype = ? ORDER BY name LIMIT {limit} OFFSET {offset}"
             result = self.execute(sql, name=search_name, stype=stype.val)[1] or []
         else:
             sql = f"SELECT * FROM SETTINGS WHERE name LIKE ? ORDER BY name LIMIT {limit} OFFSET {offset}"
             result = self.execute(sql, name=search_name)[1] or []
 
         return list(map(self.to_entity_type, result))
 
-    def clear(self, name: str = None) -> None:
+    def clear(self, name: str | None = None, stype: SettingsType | None = None) -> None:
         """Remove all settings matching prefix."""
-        name = name.replace("*", "%") if name else "%"
-        sql = "DELETE FROM SETTINGS WHERE name LIKE ?"
-        self.execute(sql, name=name)
+        search_name = name.replace("*", "%") if name else "%"
+        if stype:
+            sql = "DELETE FROM SETTINGS WHERE name LIKE ? AND stype = ?"
+            self.execute(sql, name=search_name, stype=stype.val)
+        else:
+            sql = "DELETE FROM SETTINGS WHERE name LIKE ?"
+            self.execute(sql, name=search_name)
 
     def create_db(self) -> None:
         """TODO"""
         self.execute(
             dedent(
                 """
                 CREATE TABLE IF NOT EXISTS SETTINGS
```

### Comparing `hspylib-setman-0.9.4/setman/settings/settings_service.py` & `hspylib-setman-0.9.5/setman/settings/settings_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,23 +37,24 @@
     def search(
         self,
         name: str,
         stype: SettingsType = None,
         limit: int = 500,
         offset: int = 0) -> List[SettingsEntry]:
         """Search settings matching the specified name.
-        :param name: the settings name to search.
+        :param name: the settings name to filter.
         :param stype: the settings type to filter.
         :param limit: the max amount of records to search.
         :param offset: the records offset from which to search.
         """
         return self.repository.search(name, stype, limit, offset)
 
-    def clear(self, name: str = None) -> None:
+    def clear(self, name: str | None = None, stype: SettingsType | None = None) -> None:
         """Clear all settings from the settings table matching the specified name.
-        :param name: the settings name to search.
+        :param name: the settings name to filter.
+        :param stype: the settings type to filter.
         """
-        self.repository.clear(name)
+        self.repository.clear(name, stype)
 
     def create_db(self) -> None:
         """Create a brand new setman database file."""
         self.repository.create_db()
```

### Comparing `hspylib-setman-0.9.4/setup.py` & `hspylib-setman-0.9.5/setup.py`

 * *Files identical despite different names*

