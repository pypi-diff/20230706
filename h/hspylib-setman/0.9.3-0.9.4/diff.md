# Comparing `tmp/hspylib-setman-0.9.3.tar.gz` & `tmp/hspylib-setman-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-setman-0.9.3.tar", last modified: Thu Jul  6 16:29:37 2023, max compression
+gzip compressed data, was "hspylib-setman-0.9.4.tar", last modified: Thu Jul  6 19:17:41 2023, max compression
```

## Comparing `hspylib-setman-0.9.3.tar` & `hspylib-setman-0.9.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 16:29:37.436548 hspylib-setman-0.9.3/
--rw-r--r--   0 hjunior    (504) staff       (20)       51 2023-07-06 16:29:29.000000 hspylib-setman-0.9.3/MANIFEST.in
--rw-r--r--   0 hjunior    (504) staff       (20)     1675 2023-07-06 16:29:37.435739 hspylib-setman-0.9.3/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      672 2023-07-06 16:29:36.000000 hspylib-setman-0.9.3/README.md
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 16:29:37.404110 hspylib-setman-0.9.3/hspylib_setman.egg-info/
--rw-r--r--   0 hjunior    (504) staff       (20)     1675 2023-07-06 16:29:37.000000 hspylib-setman-0.9.3/hspylib_setman.egg-info/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      619 2023-07-06 16:29:37.000000 hspylib-setman-0.9.3/hspylib_setman.egg-info/SOURCES.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-07-06 16:29:37.000000 hspylib-setman-0.9.3/hspylib_setman.egg-info/dependency_links.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       41 2023-07-06 16:29:37.000000 hspylib-setman-0.9.3/hspylib_setman.egg-info/requires.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        7 2023-07-06 16:29:37.000000 hspylib-setman-0.9.3/hspylib_setman.egg-info/top_level.txt
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 16:29:37.413527 hspylib-setman-0.9.3/setman/
--rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-07-06 16:29:36.000000 hspylib-setman-0.9.3/setman/.version
--rw-r--r--   0 hjunior    (504) staff       (20)      718 2023-07-05 21:55:00.000000 hspylib-setman-0.9.3/setman/__classpath__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      166 2023-07-06 16:29:36.000000 hspylib-setman-0.9.3/setman/__init__.py
--rwxr-xr-x   0 hjunior    (504) staff       (20)     4752 2023-07-05 23:38:47.000000 hspylib-setman-0.9.3/setman/__main__.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 16:29:37.421895 hspylib-setman-0.9.3/setman/core/
--rw-r--r--   0 hjunior    (504) staff       (20)      197 2023-07-06 16:29:36.000000 hspylib-setman-0.9.3/setman/core/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     6164 2023-07-05 23:02:34.000000 hspylib-setman-0.9.3/setman/core/setman.py
--rw-r--r--   0 hjunior    (504) staff       (20)      823 2023-07-05 22:10:34.000000 hspylib-setman-0.9.3/setman/core/setman_config.py
--rw-r--r--   0 hjunior    (504) staff       (20)     1406 2023-07-05 22:27:05.000000 hspylib-setman-0.9.3/setman/core/setman_enums.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 16:29:37.434053 hspylib-setman-0.9.3/setman/settings/
--rw-r--r--   0 hjunior    (504) staff       (20)      256 2023-07-06 16:29:36.000000 hspylib-setman-0.9.3/setman/settings/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     9241 2023-07-05 23:11:54.000000 hspylib-setman-0.9.3/setman/settings/settings.py
--rw-r--r--   0 hjunior    (504) staff       (20)     1404 2023-07-05 17:37:53.000000 hspylib-setman-0.9.3/setman/settings/settings_config.py
--rw-r--r--   0 hjunior    (504) staff       (20)     3446 2023-07-05 22:08:41.000000 hspylib-setman-0.9.3/setman/settings/settings_entry.py
--rw-r--r--   0 hjunior    (504) staff       (20)     3887 2023-07-05 22:08:56.000000 hspylib-setman-0.9.3/setman/settings/settings_repository.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2054 2023-07-05 22:30:45.000000 hspylib-setman-0.9.3/setman/settings/settings_service.py
--rw-r--r--   0 hjunior    (504) staff       (20)      256 2023-07-05 22:41:51.000000 hspylib-setman-0.9.3/setman/welcome.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-07-06 16:29:37.436706 hspylib-setman-0.9.3/setup.cfg
--rw-r--r--   0 hjunior    (504) staff       (20)     2067 2023-07-05 21:51:13.000000 hspylib-setman-0.9.3/setup.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 19:17:41.893121 hspylib-setman-0.9.4/
+-rw-r--r--   0 hjunior    (504) staff       (20)       51 2023-07-06 16:29:29.000000 hspylib-setman-0.9.4/MANIFEST.in
+-rw-r--r--   0 hjunior    (504) staff       (20)     1675 2023-07-06 19:17:41.891800 hspylib-setman-0.9.4/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      672 2023-07-06 19:17:40.000000 hspylib-setman-0.9.4/README.md
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 19:17:41.854638 hspylib-setman-0.9.4/hspylib_setman.egg-info/
+-rw-r--r--   0 hjunior    (504) staff       (20)     1675 2023-07-06 19:17:41.000000 hspylib-setman-0.9.4/hspylib_setman.egg-info/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      619 2023-07-06 19:17:41.000000 hspylib-setman-0.9.4/hspylib_setman.egg-info/SOURCES.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-07-06 19:17:41.000000 hspylib-setman-0.9.4/hspylib_setman.egg-info/dependency_links.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       41 2023-07-06 19:17:41.000000 hspylib-setman-0.9.4/hspylib_setman.egg-info/requires.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        7 2023-07-06 19:17:41.000000 hspylib-setman-0.9.4/hspylib_setman.egg-info/top_level.txt
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 19:17:41.862378 hspylib-setman-0.9.4/setman/
+-rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-07-06 19:17:40.000000 hspylib-setman-0.9.4/setman/.version
+-rw-r--r--   0 hjunior    (504) staff       (20)      718 2023-07-05 21:55:00.000000 hspylib-setman-0.9.4/setman/__classpath__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      166 2023-07-06 19:17:40.000000 hspylib-setman-0.9.4/setman/__init__.py
+-rwxr-xr-x   0 hjunior    (504) staff       (20)     4786 2023-07-06 18:54:15.000000 hspylib-setman-0.9.4/setman/__main__.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 19:17:41.870244 hspylib-setman-0.9.4/setman/core/
+-rw-r--r--   0 hjunior    (504) staff       (20)      197 2023-07-06 19:17:40.000000 hspylib-setman-0.9.4/setman/core/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     7211 2023-07-06 19:09:18.000000 hspylib-setman-0.9.4/setman/core/setman.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      823 2023-07-05 22:10:34.000000 hspylib-setman-0.9.4/setman/core/setman_config.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     1406 2023-07-05 22:27:05.000000 hspylib-setman-0.9.4/setman/core/setman_enums.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 19:17:41.888485 hspylib-setman-0.9.4/setman/settings/
+-rw-r--r--   0 hjunior    (504) staff       (20)      256 2023-07-06 19:17:40.000000 hspylib-setman-0.9.4/setman/settings/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     9400 2023-07-06 19:14:49.000000 hspylib-setman-0.9.4/setman/settings/settings.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     1404 2023-07-05 17:37:53.000000 hspylib-setman-0.9.4/setman/settings/settings_config.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     3446 2023-07-05 22:08:41.000000 hspylib-setman-0.9.4/setman/settings/settings_entry.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     3887 2023-07-05 22:08:56.000000 hspylib-setman-0.9.4/setman/settings/settings_repository.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2054 2023-07-05 22:30:45.000000 hspylib-setman-0.9.4/setman/settings/settings_service.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      256 2023-07-05 22:41:51.000000 hspylib-setman-0.9.4/setman/welcome.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-07-06 19:17:41.893305 hspylib-setman-0.9.4/setup.cfg
+-rw-r--r--   0 hjunior    (504) staff       (20)     2067 2023-07-05 21:51:13.000000 hspylib-setman-0.9.4/setup.py
```

### Comparing `hspylib-setman-0.9.3/PKG-INFO` & `hspylib-setman-0.9.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-setman
-Version: 0.9.3
+Version: 0.9.4
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
-[![Release](https://badgen.net/badge/release/v0.9.3/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.4/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-setman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-setman-0.9.3/README.md` & `hspylib-setman-0.9.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # HsPyLib - Settings Manager
 
 ## Manage your terminal settings
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.3/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.4/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-setman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-setman-0.9.3/hspylib_setman.egg-info/PKG-INFO` & `hspylib-setman-0.9.4/hspylib_setman.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-setman
-Version: 0.9.3
+Version: 0.9.4
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
-[![Release](https://badgen.net/badge/release/v0.9.3/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.4/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-setman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-setman-0.9.3/hspylib_setman.egg-info/SOURCES.txt` & `hspylib-setman-0.9.4/hspylib_setman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.3/setman/__classpath__.py` & `hspylib-setman-0.9.4/setman/__classpath__.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.3/setman/__main__.py` & `hspylib-setman-0.9.4/setman/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,16 @@
         op = self.get_arg("operation")
         st = self.get_arg("type")
         self._setman.execute(
             SetmanOps.of_value(op) if op else None,
             self.get_arg("name"),
             self.get_arg("value"),
             SettingsType.of_value(st) if st else None,
-            self.get_arg("simple")
+            self.get_arg("simple"),
+            self.get_arg("file")
         )
 
         return ExitStatus.SUCCESS
 
 
 # Application entry point
 if __name__ == "__main__":
```

### Comparing `hspylib-setman-0.9.3/setman/core/setman.py` & `hspylib-setman-0.9.4/setman/core/setman.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 """
 import atexit
 import logging as log
 import os
 from typing import Any
 
 from hspylib.core.enums.charset import Charset
+from hspylib.core.exception.exceptions import InvalidArgumentError
 from hspylib.core.metaclass.singleton import Singleton
 from hspylib.core.preconditions import check_state
 from hspylib.core.tools.commons import file_is_not_empty, syserr, sysout
 from hspylib.modules.application.application import Application
 from hspylib.modules.cli.keyboard import Keyboard
 
 from clitt.core.tui.table.table_enums import TextAlignment
@@ -70,14 +71,15 @@
     def execute(
         self,
         operation: SetmanOps,
         name: str | None,
         value: Any | None,
         stype: SettingsType = None,
         simple_fmt: bool = False,
+        filepath: str = None
     ) -> None:
         """Execute the specified operation."""
         log.debug(f"{operation} Name: {name or '*'} Value: {value or '-'} SettingsType: {stype or '*'}")
         atexit.register(self.settings.close)
         with self.settings.open():
             match operation:
                 case SetmanOps.LIST:
@@ -88,38 +90,44 @@
                     self._set_setting(name, value, stype)
                 case SetmanOps.GET:
                     self._get_setting(name, simple_fmt)
                 case SetmanOps.DEL:
                     self._del_setting(name)
                 case SetmanOps.TRUNCATE:
                     self._clear_settings(name)
+                case SetmanOps.IMPORT:
+                    self._import_settings(filepath)
+                case SetmanOps.EXPORT:
+                    self._export_settings(filepath, name, stype)
+                case _:
+                    raise InvalidArgumentError(f"Operation not supported: {operation}")
 
     def _set_setting(self, name: str | None, value: Any | None, stype: SettingsType | None) -> None:
         """Upsert the specified setting."""
         found, entry = self.settings.upsert(name, value, stype)
-        sysout(f"%GREEN%Settings {'added' if not found else 'saved'}: %WHITE%", entry)
+        sysout(f"%GREEN%Settings {'added' if not found else 'saved'}: %WHITE%", entry, "%EOL%")
 
     def _get_setting(self, name: str, simple_fmt: bool = False) -> None:
         """Get setting matching the specified name.
         :param name: the settings name to get.
         :param simple_fmt: whether to format the setting or not.
         """
         if found := self.settings.get(name):
             sysout(found.to_string(simple_fmt))
         else:
-            syserr("%EOL%%YELLOW%No settings found matching: %WHITE%", name)
+            syserr("%EOL%%YELLOW%No settings found matching: %WHITE%", name, "%EOL%")
 
     def _del_setting(self, name: str) -> None:
         """Delete specified setting.
         :param name: the settings name to delete.
         """
         if found := self.settings.remove(name):
-            sysout("%GREEN%Setting deleted: %WHITE%", found)
+            sysout("%GREEN%Setting deleted: %WHITE%", found, "%EOL%")
         else:
-            syserr("%EOL%%YELLOW%No settings found matching: %WHITE%", name)
+            syserr("%EOL%%YELLOW%No settings found matching: %WHITE%", name, "%EOL%")
 
     def _list_settings(self, name: str | None, stype: SettingsType | None) -> None:
         """List in a table all settings matching criteria."""
         data = list(map(lambda s: s.values, self.settings.search(name, stype)))
         tr = TableRenderer(self.settings.HEADERS, data, "Systems Settings")
         tr.adjust_auto_fit()
         tr.set_header_alignment(TextAlignment.CENTER)
@@ -128,28 +136,40 @@
 
     def _search_settings(self, name: str | None, stype: SettingsType | None, simple_fmt: bool) -> None:
         """Search and display all settings matching criteria."""
         data = list(map(lambda e: e.to_string(simple_fmt), self.settings.search(name, stype)))
         sysout(os.linesep.join(data)) \
             if data \
             else sysout(
-            f"%EOL%%YELLOW%No settings found matching: %WHITE%[name={name.replace('%', '*')}, stype={stype}]"
+            f"%EOL%%YELLOW%No settings found matching: %WHITE%[name={name.replace('%', '*')}, stype={stype}] %EOL%"
         )
 
-    def _clear_settings(self, name: str) -> None:
-        """Clear all settings."""
+    def _clear_settings(self, name: str | None) -> None:
+        """Clear all settings.
+        :param name: clear settings matching name.
+        """
         if not name:
             sysout("%EOL%%ORANGE%All settings will be removed. Are you sure (y/[n])? ")
             keystroke = Keyboard.wait_keystroke()
             if keystroke and keystroke in [Keyboard.VK_y, Keyboard.VK_Y]:
                 self.settings.clear("*")
                 sysout("%EOL%%ORANGE%!!! All system settings have been removed !!!%EOL%")
         else:
             self.settings.clear(name)
             sysout(f"%EOL%%ORANGE%!!! System settings matching [{name}] have been removed !!!%EOL%")
 
+    def _import_settings(self, filepath: str) -> None:
+        """Import settings from CSV file."""
+        count = self.settings.import_csv(filepath)
+        sysout(f"%EOL%%GREEN%Imported {count} settings from {filepath}! %EOL%")
+
+    def _export_settings(self, filepath: str, name: str | None = None, stype: SettingsType | None = None) -> None:
+        """Import settings from CSV file."""
+        count = self.settings.export_csv(filepath, name, stype)
+        sysout(f"%EOL%%GREEN%Exported {count} settings to {filepath}! %EOL%")
+
     def _setup(self, filepath: str) -> None:
         """Setup SetMan on the system."""
         with open(filepath, "w+", encoding=Charset.UTF_8.val) as f_configs:
             f_configs.write(f"hhs.setman.database = {self.SETMAN_DB_FILE} {os.linesep}")
             f_configs.write(f"hhs.setman.encode.database = True")
             check_state(os.path.exists(filepath), "Unable to create Setman configuration file: " + filepath)
```

### Comparing `hspylib-setman-0.9.3/setman/core/setman_config.py` & `hspylib-setman-0.9.4/setman/core/setman_config.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.3/setman/core/setman_enums.py` & `hspylib-setman-0.9.4/setman/core/setman_enums.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.3/setman/settings/settings.py` & `hspylib-setman-0.9.4/setman/settings/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import uuid
 from functools import lru_cache
 from typing import Any, List, Optional, Tuple
 
 from datasource.identity import Identity
 from hspylib.core.exception.exceptions import ApplicationError
 from hspylib.core.preconditions import check_argument, check_state
-from hspylib.core.tools.commons import file_is_not_empty, safe_delete_file, touch_file
+from hspylib.core.tools.commons import dirname, file_is_not_empty, safe_delete_file, touch_file
 from hspylib.core.tools.text_tools import ensure_endswith
 from hspylib.core.zoned_datetime import now
 from hspylib.modules.security.security import decode_file, encode_file
 
 from setman.core.setman_enums import SettingsType
 from setman.settings.settings_config import SettingsConfig
 from setman.settings.settings_entry import SettingsEntry
@@ -187,32 +187,33 @@
         self._service.clear(name)
         self._clear_caches()
 
     def import_csv(self, filepath: str) -> int:
         """Upsert settings from CSV file into the database.
         :param filepath: the path of the CSV file to be imported.
         """
-        check_argument(file_is_not_empty(filepath), f"File not found: {filepath}")
-        count = 0
-        csv_file = ensure_endswith(filepath, ".csv")
+        count, csv_file = 0, ensure_endswith(filepath, ".csv")
+        check_argument(os.path.exists(filepath), "CSV file does not exist: " + csv_file)
         with open(csv_file, encoding="UTF8") as f_csv:
             csv_reader = csv.reader(f_csv, delimiter=',')
             for row in csv_reader:
                 if row == self.HEADERS:
                     continue
                 uid, name, value, stype = str(row[0]), str(row[1]), str(row[2]), SettingsType.of_value(row[3])
                 entry = SettingsEntry(Identity(SettingsEntry.SetmanId(uid)), name, value, stype)
                 self._service.save(entry)
+                count += 1
             self._clear_caches()
             return count
 
     def export_csv(self, filepath: str, name: str = None, stype: SettingsType = None) -> int:
         """Export settings from CSV file into the database."""
+        dest_dir, csv_file = dirname(filepath), ensure_endswith(filepath, ".csv")
+        check_argument(os.path.exists(dest_dir), "Destination dir does not exist: " + dest_dir)
         settings = self.search(name, stype)
-        csv_file = ensure_endswith(filepath, ".csv")
         with open(csv_file, "w", encoding="UTF8") as f_csv:
             writer = csv.writer(f_csv, delimiter=',')
             writer.writerow(self.HEADERS)
             writer.writerows(list(map(lambda s: s.values, settings)))
             return len(settings)
 
     def _create_db(self) -> bool:
```

### Comparing `hspylib-setman-0.9.3/setman/settings/settings_config.py` & `hspylib-setman-0.9.4/setman/settings/settings_config.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.3/setman/settings/settings_entry.py` & `hspylib-setman-0.9.4/setman/settings/settings_entry.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.3/setman/settings/settings_repository.py` & `hspylib-setman-0.9.4/setman/settings/settings_repository.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.3/setman/settings/settings_service.py` & `hspylib-setman-0.9.4/setman/settings/settings_service.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.3/setup.py` & `hspylib-setman-0.9.4/setup.py`

 * *Files identical despite different names*

