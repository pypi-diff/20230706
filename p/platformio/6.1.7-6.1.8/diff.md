# Comparing `tmp/platformio-6.1.7.tar.gz` & `tmp/platformio-6.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platformio-6.1.7.tar", last modified: Mon May  8 14:59:21 2023, max compression
+gzip compressed data, was "platformio-6.1.8.tar", last modified: Wed Jul  5 12:47:07 2023, max compression
```

## Comparing `platformio-6.1.7.tar` & `platformio-6.1.8.tar`

### file list

```diff
@@ -1,368 +1,363 @@
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.300732 platformio-6.1.7/
--rw-r--r--   0 ikravets   (501) staff       (20)     9169 2019-12-19 09:45:48.000000 platformio-6.1.7/LICENSE
--rw-r--r--   0 ikravets   (501) staff       (20)     6549 2023-05-08 14:59:21.300299 platformio-6.1.7/PKG-INFO
--rw-r--r--   0 ikravets   (501) staff       (20)     5122 2022-08-12 13:55:00.000000 platformio-6.1.7/README.rst
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.038491 platformio-6.1.7/platformio/
--rw-r--r--   0 ikravets   (501) staff       (20)     2101 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     4606 2022-10-31 20:40:30.000000 platformio-6.1.7/platformio/__main__.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.045479 platformio-6.1.7/platformio/account/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1593 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/cli.py
--rw-r--r--   0 ikravets   (501) staff       (20)    11093 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/account/client.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.051709 platformio-6.1.7/platformio/account/commands/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/commands/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1246 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/commands/destroy.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1039 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/commands/forgot.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1036 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/commands/login.py
--rw-r--r--   0 ikravets   (501) staff       (20)      879 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/commands/logout.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1086 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/commands/password.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1702 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/commands/register.py
--rw-r--r--   0 ikravets   (501) staff       (20)     4263 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/commands/show.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1255 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/commands/token.py
--rw-r--r--   0 ikravets   (501) staff       (20)     2282 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/commands/update.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.053207 platformio-6.1.7/platformio/account/org/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/org/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1267 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/org/cli.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.057801 platformio-6.1.7/platformio/account/org/commands/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/org/commands/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1089 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/org/commands/add.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1305 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/org/commands/create.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1194 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/org/commands/destroy.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1666 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/org/commands/list.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1100 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/org/commands/remove.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1804 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/account/org/commands/update.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.059307 platformio-6.1.7/platformio/account/team/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/team/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1287 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/team/cli.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.067146 platformio-6.1.7/platformio/account/team/commands/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/team/commands/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1324 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/team/commands/add.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1289 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/account/team/commands/create.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1388 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/team/commands/destroy.py
--rw-r--r--   0 ikravets   (501) staff       (20)     2181 2023-03-07 04:32:55.000000 platformio-6.1.7/platformio/account/team/commands/list.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1327 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/team/commands/remove.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1809 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/account/team/commands/update.py
--rw-r--r--   0 ikravets   (501) staff       (20)     2895 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/account/validate.py
--rw-r--r--   0 ikravets   (501) staff       (20)     8083 2022-11-01 18:28:49.000000 platformio-6.1.7/platformio/app.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.005107 platformio-6.1.7/platformio/assets/
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.068239 platformio-6.1.7/platformio/assets/system/
--rw-r--r--   0 ikravets   (501) staff       (20)     8260 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/system/99-platformio-udev.rules
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.005331 platformio-6.1.7/platformio/assets/templates/
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.009147 platformio-6.1.7/platformio/assets/templates/ide-projects/
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.074504 platformio-6.1.7/platformio/assets/templates/ide-projects/atom/
--rw-r--r--   0 ikravets   (501) staff       (20)      109 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/atom/.clang_complete.tpl
--rw-r--r--   0 ikravets   (501) staff       (20)      530 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/atom/.gcc-flags.json.tpl
--rw-r--r--   0 ikravets   (501) staff       (20)       37 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/atom/.gitignore.tpl
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.077481 platformio-6.1.7/platformio/assets/templates/ide-projects/clion/
--rw-r--r--   0 ikravets   (501) staff       (20)       43 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/clion/.gitignore.tpl
--rw-r--r--   0 ikravets   (501) staff       (20)     1068 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/clion/CMakeLists.txt.tpl
--rw-r--r--   0 ikravets   (501) staff       (20)     3885 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/clion/CMakeListsPrivate.txt.tpl
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.078575 platformio-6.1.7/platformio/assets/templates/ide-projects/codeblocks/
--rw-r--r--   0 ikravets   (501) staff       (20)     2565 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/codeblocks/platformio.cbp.tpl
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.082530 platformio-6.1.7/platformio/assets/templates/ide-projects/eclipse/
--rw-r--r--   0 ikravets   (501) staff       (20)    20663 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/eclipse/.cproject.tpl
--rw-r--r--   0 ikravets   (501) staff       (20)      817 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/eclipse/.project.tpl
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.085456 platformio-6.1.7/platformio/assets/templates/ide-projects/eclipse/.settings/
--rw-r--r--   0 ikravets   (501) staff       (20)     2838 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/eclipse/.settings/PlatformIO Debugger.launch.tpl
--rw-r--r--   0 ikravets   (501) staff       (20)     2410 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/eclipse/.settings/language.settings.xml.tpl
--rw-r--r--   0 ikravets   (501) staff       (20)      756 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/eclipse/.settings/org.eclipse.cdt.core.prefs.tpl
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.088166 platformio-6.1.7/platformio/assets/templates/ide-projects/emacs/
--rw-r--r--   0 ikravets   (501) staff       (20)      176 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/emacs/.ccls.tpl
--rw-r--r--   0 ikravets   (501) staff       (20)       27 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/emacs/.gitignore.tpl
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.007159 platformio-6.1.7/platformio/assets/templates/ide-projects/netbeans/
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.090123 platformio-6.1.7/platformio/assets/templates/ide-projects/netbeans/nbproject/
--rw-r--r--   0 ikravets   (501) staff       (20)     2520 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/netbeans/nbproject/configurations.xml.tpl
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.092719 platformio-6.1.7/platformio/assets/templates/ide-projects/netbeans/nbproject/private/
--rw-r--r--   0 ikravets   (501) staff       (20)     2330 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/netbeans/nbproject/private/configurations.xml.tpl
--rw-r--r--   0 ikravets   (501) staff       (20)     2001 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/netbeans/nbproject/private/launcher.properties.tpl
--rw-r--r--   0 ikravets   (501) staff       (20)      481 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/netbeans/nbproject/private/private.xml.tpl
--rw-r--r--   0 ikravets   (501) staff       (20)      912 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/netbeans/nbproject/project.xml.tpl
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.097969 platformio-6.1.7/platformio/assets/templates/ide-projects/qtcreator/
--rw-r--r--   0 ikravets   (501) staff       (20)       17 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/qtcreator/.gitignore.tpl
--rw-r--r--   0 ikravets   (501) staff       (20)      383 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/qtcreator/Makefile.tpl
--rw-r--r--   0 ikravets   (501) staff       (20)       52 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/qtcreator/platformio.cflags.tpl
--rw-r--r--   0 ikravets   (501) staff       (20)      171 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/qtcreator/platformio.config.tpl
--rw-r--r--   0 ikravets   (501) staff       (20)       11 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/qtcreator/platformio.creator.tpl
--rw-r--r--   0 ikravets   (501) staff       (20)       53 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/qtcreator/platformio.cxxflags.tpl
--rw-r--r--   0 ikravets   (501) staff       (20)       75 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/qtcreator/platformio.files.tpl
--rw-r--r--   0 ikravets   (501) staff       (20)       65 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/qtcreator/platformio.includes.tpl
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.099201 platformio-6.1.7/platformio/assets/templates/ide-projects/sublimetext/
--rw-r--r--   0 ikravets   (501) staff       (20)      176 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/sublimetext/.ccls.tpl
--rw-r--r--   0 ikravets   (501) staff       (20)     2069 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/sublimetext/platformio.sublime-project.tpl
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.100288 platformio-6.1.7/platformio/assets/templates/ide-projects/vim/
--rw-r--r--   0 ikravets   (501) staff       (20)      176 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/vim/.ccls.tpl
--rw-r--r--   0 ikravets   (501) staff       (20)       43 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/vim/.gitignore.tpl
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.101472 platformio-6.1.7/platformio/assets/templates/ide-projects/visualstudio/
--rw-r--r--   0 ikravets   (501) staff       (20)      975 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/visualstudio/platformio.vcxproj.filters.tpl
--rw-r--r--   0 ikravets   (501) staff       (20)     3806 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/visualstudio/platformio.vcxproj.tpl
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.102102 platformio-6.1.7/platformio/assets/templates/ide-projects/vscode/
--rw-r--r--   0 ikravets   (501) staff       (20)       94 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/vscode/.gitignore.tpl
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.104130 platformio-6.1.7/platformio/assets/templates/ide-projects/vscode/.vscode/
--rw-r--r--   0 ikravets   (501) staff       (20)     3367 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/vscode/.vscode/c_cpp_properties.json.tpl
--rw-r--r--   0 ikravets   (501) staff       (20)     1159 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/vscode/.vscode/extensions.json.tpl
--rw-r--r--   0 ikravets   (501) staff       (20)     2832 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/vscode/.vscode/launch.json.tpl
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.105355 platformio-6.1.7/platformio/builder/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2019-12-19 09:45:48.000000 platformio-6.1.7/platformio/builder/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     8228 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/builder/main.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.116201 platformio-6.1.7/platformio/builder/tools/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-04-11 08:55:48.000000 platformio-6.1.7/platformio/builder/tools/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1027 2022-08-12 13:55:00.000000 platformio-6.1.7/platformio/builder/tools/pioasm.py
--rw-r--r--   0 ikravets   (501) staff       (20)    12577 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/builder/tools/piobuild.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1676 2022-08-12 13:55:00.000000 platformio-6.1.7/platformio/builder/tools/piohooks.py
--rw-r--r--   0 ikravets   (501) staff       (20)     8210 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/builder/tools/pioino.py
--rw-r--r--   0 ikravets   (501) staff       (20)     6335 2022-11-01 18:28:49.000000 platformio-6.1.7/platformio/builder/tools/piointegration.py
--rw-r--r--   0 ikravets   (501) staff       (20)    42536 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/builder/tools/piolib.py
--rw-r--r--   0 ikravets   (501) staff       (20)     2973 2022-08-12 13:55:00.000000 platformio-6.1.7/platformio/builder/tools/piomaxlen.py
--rw-r--r--   0 ikravets   (501) staff       (20)     4431 2022-08-12 13:55:00.000000 platformio-6.1.7/platformio/builder/tools/piomisc.py
--rw-r--r--   0 ikravets   (501) staff       (20)     8217 2023-04-24 14:16:09.000000 platformio-6.1.7/platformio/builder/tools/pioplatform.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1700 2022-08-12 13:55:00.000000 platformio-6.1.7/platformio/builder/tools/pioproject.py
--rw-r--r--   0 ikravets   (501) staff       (20)     8102 2022-08-12 13:55:00.000000 platformio-6.1.7/platformio/builder/tools/piosize.py
--rw-r--r--   0 ikravets   (501) staff       (20)     3317 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/builder/tools/piotarget.py
--rw-r--r--   0 ikravets   (501) staff       (20)     2106 2022-08-12 13:55:00.000000 platformio-6.1.7/platformio/builder/tools/piotest.py
--rw-r--r--   0 ikravets   (501) staff       (20)     8472 2022-08-12 13:55:00.000000 platformio-6.1.7/platformio/builder/tools/pioupload.py
--rw-r--r--   0 ikravets   (501) staff       (20)     5269 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/cache.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.118060 platformio-6.1.7/platformio/check/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/check/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)    10813 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/check/cli.py
--rw-r--r--   0 ikravets   (501) staff       (20)     3093 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/check/defect.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.121755 platformio-6.1.7/platformio/check/tools/
--rw-r--r--   0 ikravets   (501) staff       (20)     1319 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/check/tools/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     8710 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/check/tools/base.py
--rw-r--r--   0 ikravets   (501) staff       (20)     3094 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/check/tools/clangtidy.py
--rw-r--r--   0 ikravets   (501) staff       (20)     9357 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/check/tools/cppcheck.py
--rw-r--r--   0 ikravets   (501) staff       (20)     8421 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/check/tools/pvsstudio.py
--rw-r--r--   0 ikravets   (501) staff       (20)     3192 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/cli.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.127329 platformio-6.1.7/platformio/commands/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/commands/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     2824 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/commands/boards.py
--rw-r--r--   0 ikravets   (501) staff       (20)     5638 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/commands/ci.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.128166 platformio-6.1.7/platformio/commands/device/
--rw-r--r--   0 ikravets   (501) staff       (20)      750 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/commands/device/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)    16025 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/commands/lib.py
--rw-r--r--   0 ikravets   (501) staff       (20)    12882 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/commands/platform.py
--rw-r--r--   0 ikravets   (501) staff       (20)     2477 2020-09-03 11:43:11.000000 platformio-6.1.7/platformio/commands/settings.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1244 2022-05-17 16:23:31.000000 platformio-6.1.7/platformio/commands/update.py
--rw-r--r--   0 ikravets   (501) staff       (20)     4385 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/commands/upgrade.py
--rw-r--r--   0 ikravets   (501) staff       (20)     3308 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/compat.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.130709 platformio-6.1.7/platformio/debug/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2021-10-25 08:38:45.000000 platformio-6.1.7/platformio/debug/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     6037 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/debug/cli.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.136263 platformio-6.1.7/platformio/debug/config/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2021-10-25 08:38:45.000000 platformio-6.1.7/platformio/debug/config/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     8861 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/debug/config/base.py
--rw-r--r--   0 ikravets   (501) staff       (20)     2074 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/debug/config/blackmagic.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1766 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/debug/config/factory.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1098 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/debug/config/generic.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1290 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/debug/config/jlink.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1050 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/debug/config/mspdebug.py
--rw-r--r--   0 ikravets   (501) staff       (20)      966 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/debug/config/native.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1091 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/debug/config/qemu.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1285 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/debug/config/renode.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1137 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/debug/exception.py
--rw-r--r--   0 ikravets   (501) staff       (20)     5063 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/debug/helpers.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.139206 platformio-6.1.7/platformio/debug/process/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2021-10-25 08:38:45.000000 platformio-6.1.7/platformio/debug/process/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     4893 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/debug/process/base.py
--rw-r--r--   0 ikravets   (501) staff       (20)     3461 2022-05-16 11:22:08.000000 platformio-6.1.7/platformio/debug/process/client.py
--rw-r--r--   0 ikravets   (501) staff       (20)     7370 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/debug/process/gdb.py
--rw-r--r--   0 ikravets   (501) staff       (20)     5656 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/debug/process/server.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.140918 platformio-6.1.7/platformio/device/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-05-16 11:22:08.000000 platformio-6.1.7/platformio/device/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)      933 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/device/cli.py
--rw-r--r--   0 ikravets   (501) staff       (20)     8573 2022-12-13 19:50:55.000000 platformio-6.1.7/platformio/device/finder.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.146328 platformio-6.1.7/platformio/device/list/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/device/list/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     3333 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/device/list/command.py
--rw-r--r--   0 ikravets   (501) staff       (20)     5476 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/device/list/util.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.148230 platformio-6.1.7/platformio/device/monitor/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/device/monitor/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     6127 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/device/monitor/command.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.152433 platformio-6.1.7/platformio/device/monitor/filters/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/device/monitor/filters/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     3429 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/device/monitor/filters/base.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1285 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/device/monitor/filters/hexlify.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1547 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/device/monitor/filters/log2file.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1266 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/device/monitor/filters/send_on_enter.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1386 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/device/monitor/filters/time.py
--rw-r--r--   0 ikravets   (501) staff       (20)     6224 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/device/monitor/terminal.py
--rw-r--r--   0 ikravets   (501) staff       (20)     3009 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/exception.py
--rw-r--r--   0 ikravets   (501) staff       (20)     6767 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/fs.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.154787 platformio-6.1.7/platformio/home/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/home/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     3405 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/home/cli.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.155918 platformio-6.1.7/platformio/home/rpc/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/home/rpc/__init__.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.166147 platformio-6.1.7/platformio/home/rpc/handlers/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/home/rpc/handlers/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1196 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/home/rpc/handlers/account.py
--rw-r--r--   0 ikravets   (501) staff       (20)     3122 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/home/rpc/handlers/app.py
--rw-r--r--   0 ikravets   (501) staff       (20)      653 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/home/rpc/handlers/base.py
--rw-r--r--   0 ikravets   (501) staff       (20)     2994 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/home/rpc/handlers/ide.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1966 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/home/rpc/handlers/misc.py
--rw-r--r--   0 ikravets   (501) staff       (20)     5081 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/home/rpc/handlers/os.py
--rw-r--r--   0 ikravets   (501) staff       (20)     7644 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/home/rpc/handlers/piocore.py
--rw-r--r--   0 ikravets   (501) staff       (20)     2261 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/home/rpc/handlers/platform.py
--rw-r--r--   0 ikravets   (501) staff       (20)    12206 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/home/rpc/handlers/project.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1280 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/home/rpc/handlers/registry.py
--rw-r--r--   0 ikravets   (501) staff       (20)     4604 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/home/rpc/server.py
--rw-r--r--   0 ikravets   (501) staff       (20)     4089 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/home/run.py
--rw-r--r--   0 ikravets   (501) staff       (20)     7394 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/http.py
--rw-r--r--   0 ikravets   (501) staff       (20)     8953 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/maintenance.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.176488 platformio-6.1.7/platformio/package/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2019-12-19 09:45:48.000000 platformio-6.1.7/platformio/package/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1778 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/package/cli.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.187992 platformio-6.1.7/platformio/package/commands/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-05-16 11:22:08.000000 platformio-6.1.7/platformio/package/commands/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     3888 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/package/commands/exec.py
--rw-r--r--   0 ikravets   (501) staff       (20)    12338 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/commands/install.py
--rw-r--r--   0 ikravets   (501) staff       (20)     8182 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/commands/list.py
--rw-r--r--   0 ikravets   (501) staff       (20)     7160 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/commands/outdated.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1606 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/commands/pack.py
--rw-r--r--   0 ikravets   (501) staff       (20)     6995 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/commands/publish.py
--rw-r--r--   0 ikravets   (501) staff       (20)     2367 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/package/commands/search.py
--rw-r--r--   0 ikravets   (501) staff       (20)     4841 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/package/commands/show.py
--rw-r--r--   0 ikravets   (501) staff       (20)     8362 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/commands/uninstall.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1656 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/package/commands/unpublish.py
--rw-r--r--   0 ikravets   (501) staff       (20)     8643 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/commands/update.py
--rw-r--r--   0 ikravets   (501) staff       (20)     5890 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/download.py
--rw-r--r--   0 ikravets   (501) staff       (20)     2075 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/exception.py
--rw-r--r--   0 ikravets   (501) staff       (20)     3580 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/package/lockfile.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.200785 platformio-6.1.7/platformio/package/manager/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2020-09-03 11:43:11.000000 platformio-6.1.7/platformio/package/manager/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     3875 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/manager/_download.py
--rw-r--r--   0 ikravets   (501) staff       (20)    10482 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/manager/_install.py
--rw-r--r--   0 ikravets   (501) staff       (20)     2414 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/package/manager/_legacy.py
--rw-r--r--   0 ikravets   (501) staff       (20)     7688 2022-08-12 13:55:00.000000 platformio-6.1.7/platformio/package/manager/_registry.py
--rw-r--r--   0 ikravets   (501) staff       (20)     2642 2023-04-21 08:25:48.000000 platformio-6.1.7/platformio/package/manager/_symlink.py
--rw-r--r--   0 ikravets   (501) staff       (20)     3211 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/package/manager/_uninstall.py
--rw-r--r--   0 ikravets   (501) staff       (20)     4594 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/package/manager/_update.py
--rw-r--r--   0 ikravets   (501) staff       (20)    11676 2023-04-15 15:52:33.000000 platformio-6.1.7/platformio/package/manager/base.py
--rw-r--r--   0 ikravets   (501) staff       (20)     3081 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/manager/core.py
--rw-r--r--   0 ikravets   (501) staff       (20)     4369 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/package/manager/library.py
--rw-r--r--   0 ikravets   (501) staff       (20)     6312 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/manager/platform.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1180 2022-05-16 11:22:08.000000 platformio-6.1.7/platformio/package/manager/tool.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.204077 platformio-6.1.7/platformio/package/manifest/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2019-12-19 09:45:48.000000 platformio-6.1.7/platformio/package/manifest/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)    24640 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/package/manifest/parser.py
--rw-r--r--   0 ikravets   (501) staff       (20)     9003 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/manifest/schema.py
--rw-r--r--   0 ikravets   (501) staff       (20)    15965 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/meta.py
--rw-r--r--   0 ikravets   (501) staff       (20)     8488 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/package/pack.py
--rw-r--r--   0 ikravets   (501) staff       (20)     6601 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/unpack.py
--rw-r--r--   0 ikravets   (501) staff       (20)     8602 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/vcsclient.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1686 2020-09-03 11:43:11.000000 platformio-6.1.7/platformio/package/version.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.213259 platformio-6.1.7/platformio/platform/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2020-09-03 11:43:11.000000 platformio-6.1.7/platformio/platform/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     3490 2023-04-22 10:47:04.000000 platformio-6.1.7/platformio/platform/_packages.py
--rw-r--r--   0 ikravets   (501) staff       (20)     6830 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/platform/_run.py
--rw-r--r--   0 ikravets   (501) staff       (20)     8687 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/platform/base.py
--rw-r--r--   0 ikravets   (501) staff       (20)     5114 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/platform/board.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1380 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/platform/exception.py
--rw-r--r--   0 ikravets   (501) staff       (20)     3311 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/platform/factory.py
--rw-r--r--   0 ikravets   (501) staff       (20)     6466 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/proc.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.225961 platformio-6.1.7/platformio/project/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2019-12-19 09:45:48.000000 platformio-6.1.7/platformio/project/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1016 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/project/cli.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.232507 platformio-6.1.7/platformio/project/commands/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-05-16 11:22:08.000000 platformio-6.1.7/platformio/project/commands/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1955 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/project/commands/config.py
--rw-r--r--   0 ikravets   (501) staff       (20)    12843 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/project/commands/init.py
--rw-r--r--   0 ikravets   (501) staff       (20)     2826 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/project/commands/metadata.py
--rw-r--r--   0 ikravets   (501) staff       (20)    17414 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/project/config.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1908 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/project/exception.py
--rw-r--r--   0 ikravets   (501) staff       (20)     6529 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/project/helpers.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.235803 platformio-6.1.7/platformio/project/integration/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/project/integration/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     6541 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/project/integration/generator.py
--rw-r--r--   0 ikravets   (501) staff       (20)    31475 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/project/options.py
--rw-r--r--   0 ikravets   (501) staff       (20)     3077 2022-05-16 11:22:08.000000 platformio-6.1.7/platformio/project/savedeps.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1452 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/public.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.241993 platformio-6.1.7/platformio/registry/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/registry/__init__.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.245501 platformio-6.1.7/platformio/registry/access/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/registry/access/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1234 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/registry/access/cli.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.254110 platformio-6.1.7/platformio/registry/access/commands/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/registry/access/commands/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1521 2023-04-18 19:02:58.000000 platformio-6.1.7/platformio/registry/access/commands/grant.py
--rw-r--r--   0 ikravets   (501) staff       (20)     2134 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/registry/access/commands/list.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1241 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/registry/access/commands/private.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1238 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/registry/access/commands/public.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1424 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/registry/access/commands/revoke.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1074 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/registry/access/validate.py
--rw-r--r--   0 ikravets   (501) staff       (20)     5755 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/registry/client.py
--rw-r--r--   0 ikravets   (501) staff       (20)     3748 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/registry/mirror.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.257619 platformio-6.1.7/platformio/remote/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/remote/__init__.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.263307 platformio-6.1.7/platformio/remote/ac/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/remote/ac/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     2635 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/remote/ac/base.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1421 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/remote/ac/process.py
--rw-r--r--   0 ikravets   (501) staff       (20)     2326 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/remote/ac/psync.py
--rw-r--r--   0 ikravets   (501) staff       (20)     2108 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/remote/ac/serial.py
--rw-r--r--   0 ikravets   (501) staff       (20)    11855 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/remote/cli.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.272670 platformio-6.1.7/platformio/remote/client/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/remote/client/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1337 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/remote/client/agent_list.py
--rw-r--r--   0 ikravets   (501) staff       (20)     8904 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/remote/client/agent_service.py
--rw-r--r--   0 ikravets   (501) staff       (20)     2306 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/remote/client/async_base.py
--rw-r--r--   0 ikravets   (501) staff       (20)     6967 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/remote/client/base.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1989 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/remote/client/device_list.py
--rw-r--r--   0 ikravets   (501) staff       (20)     8410 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/remote/client/device_monitor.py
--rw-r--r--   0 ikravets   (501) staff       (20)     9718 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/remote/client/run_or_test.py
--rw-r--r--   0 ikravets   (501) staff       (20)      923 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/remote/client/update_core.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.275712 platformio-6.1.7/platformio/remote/factory/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/remote/factory/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     3549 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/remote/factory/client.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1485 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/remote/factory/ssl.py
--rw-r--r--   0 ikravets   (501) staff       (20)     3879 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/remote/projectsync.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.278843 platformio-6.1.7/platformio/run/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/run/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     9788 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/run/cli.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1654 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/run/helpers.py
--rw-r--r--   0 ikravets   (501) staff       (20)     3214 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/run/processor.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.281288 platformio-6.1.7/platformio/system/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/system/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1023 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/system/cli.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.283964 platformio-6.1.7/platformio/system/commands/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/system/commands/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     2504 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/system/commands/completion.py
--rw-r--r--   0 ikravets   (501) staff       (20)     2970 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/system/commands/info.py
--rw-r--r--   0 ikravets   (501) staff       (20)     2306 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/system/commands/prune.py
--rw-r--r--   0 ikravets   (501) staff       (20)     3281 2022-11-01 18:28:49.000000 platformio-6.1.7/platformio/system/completion.py
--rw-r--r--   0 ikravets   (501) staff       (20)     3507 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/system/prune.py
--rw-r--r--   0 ikravets   (501) staff       (20)    12460 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/telemetry.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.287700 platformio-6.1.7/platformio/test/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-05-16 11:22:08.000000 platformio-6.1.7/platformio/test/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     6401 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/test/cli.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1144 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/test/exception.py
--rw-r--r--   0 ikravets   (501) staff       (20)     2848 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/test/helpers.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.291940 platformio-6.1.7/platformio/test/reports/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-05-16 11:22:08.000000 platformio-6.1.7/platformio/test/reports/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     1237 2022-05-16 11:22:08.000000 platformio-6.1.7/platformio/test/reports/base.py
--rw-r--r--   0 ikravets   (501) staff       (20)     3681 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/test/reports/json.py
--rw-r--r--   0 ikravets   (501) staff       (20)     4363 2022-05-16 11:22:08.000000 platformio-6.1.7/platformio/test/reports/junit.py
--rw-r--r--   0 ikravets   (501) staff       (20)     3703 2022-05-16 11:22:08.000000 platformio-6.1.7/platformio/test/reports/stdout.py
--rw-r--r--   0 ikravets   (501) staff       (20)     4690 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/test/result.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.296548 platformio-6.1.7/platformio/test/runners/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-05-16 11:22:08.000000 platformio-6.1.7/platformio/test/runners/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     7692 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/test/runners/base.py
--rw-r--r--   0 ikravets   (501) staff       (20)     3880 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/test/runners/doctest.py
--rw-r--r--   0 ikravets   (501) staff       (20)     2812 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/test/runners/factory.py
--rw-r--r--   0 ikravets   (501) staff       (20)     3679 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/test/runners/googletest.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.298816 platformio-6.1.7/platformio/test/runners/readers/
--rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-05-16 11:22:08.000000 platformio-6.1.7/platformio/test/runners/readers/__init__.py
--rw-r--r--   0 ikravets   (501) staff       (20)     4692 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/test/runners/readers/native.py
--rw-r--r--   0 ikravets   (501) staff       (20)     2751 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/test/runners/readers/serial.py
--rw-r--r--   0 ikravets   (501) staff       (20)     9634 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/test/runners/unity.py
--rw-r--r--   0 ikravets   (501) staff       (20)     5949 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/util.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.042236 platformio-6.1.7/platformio.egg-info/
--rw-r--r--   0 ikravets   (501) staff       (20)     6549 2023-05-08 14:59:20.000000 platformio-6.1.7/platformio.egg-info/PKG-INFO
--rw-r--r--   0 ikravets   (501) staff       (20)    11636 2023-05-08 14:59:20.000000 platformio-6.1.7/platformio.egg-info/SOURCES.txt
--rw-r--r--   0 ikravets   (501) staff       (20)        1 2023-05-08 14:59:20.000000 platformio-6.1.7/platformio.egg-info/dependency_links.txt
--rw-r--r--   0 ikravets   (501) staff       (20)      136 2023-05-08 14:59:20.000000 platformio-6.1.7/platformio.egg-info/entry_points.txt
--rw-r--r--   0 ikravets   (501) staff       (20)      252 2023-05-08 14:59:20.000000 platformio-6.1.7/platformio.egg-info/requires.txt
--rw-r--r--   0 ikravets   (501) staff       (20)       11 2023-05-08 14:59:20.000000 platformio-6.1.7/platformio.egg-info/top_level.txt
--rw-r--r--   0 ikravets   (501) staff       (20)       38 2023-05-08 14:59:21.300861 platformio-6.1.7/setup.cfg
--rw-r--r--   0 ikravets   (501) staff       (20)     3600 2023-05-08 14:58:34.000000 platformio-6.1.7/setup.py
-drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.299523 platformio-6.1.7/tests/
--rw-r--r--   0 ikravets   (501) staff       (20)     3467 2023-05-08 14:58:34.000000 platformio-6.1.7/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.234894 platformio-6.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     9169 2023-07-05 12:32:56.000000 platformio-6.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-07-05 12:47:07.234894 platformio-6.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-07-05 12:32:56.000000 platformio-6.1.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.130888 platformio-6.1.8/platformio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.134889 platformio-6.1.8/platformio/account/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11150 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.138889 platformio-6.1.8/platformio/account/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/commands/destroy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/commands/forgot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/commands/logout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/commands/password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/commands/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/commands/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/commands/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/commands/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.138889 platformio-6.1.8/platformio/account/org/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/org/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/org/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.142889 platformio-6.1.8/platformio/account/org/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/org/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/org/commands/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/org/commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/org/commands/destroy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/org/commands/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/org/commands/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/org/commands/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.142889 platformio-6.1.8/platformio/account/team/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/team/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/team/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.146889 platformio-6.1.8/platformio/account/team/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/team/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/team/commands/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/team/commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/team/commands/destroy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/team/commands/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/team/commands/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/team/commands/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/account/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.118888 platformio-6.1.8/platformio/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.146889 platformio-6.1.8/platformio/assets/system/
+-rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/assets/system/99-platformio-udev.rules
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.146889 platformio-6.1.8/platformio/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.154890 platformio-6.1.8/platformio/builder/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/tools/pioasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12663 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/tools/piobuild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/tools/piohooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/tools/pioino.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/tools/piointegration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42536 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/tools/piolib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/tools/piomaxlen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/tools/piomisc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/tools/pioplatform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/tools/pioproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/tools/piosize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/tools/piotarget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/tools/piotest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/builder/tools/pioupload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.158890 platformio-6.1.8/platformio/check/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10813 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/check/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/check/defect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.158890 platformio-6.1.8/platformio/check/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/check/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/check/tools/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/check/tools/clangtidy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/check/tools/cppcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/check/tools/pvsstudio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.162890 platformio-6.1.8/platformio/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/commands/boards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/commands/ci.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.162890 platformio-6.1.8/platformio/commands/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/commands/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16025 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/commands/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/commands/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/commands/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/commands/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/commands/upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.166890 platformio-6.1.8/platformio/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.166890 platformio-6.1.8/platformio/debug/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/config/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/config/blackmagic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/config/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/config/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/config/jlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/config/mspdebug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/config/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/config/qemu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/config/renode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.170891 platformio-6.1.8/platformio/debug/process/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/process/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/process/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/process/gdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/debug/process/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.170891 platformio-6.1.8/platformio/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/device/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/device/finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.170891 platformio-6.1.8/platformio/device/list/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/device/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/device/list/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/device/list/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.170891 platformio-6.1.8/platformio/device/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/device/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/device/monitor/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.174891 platformio-6.1.8/platformio/device/monitor/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/device/monitor/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/device/monitor/filters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/device/monitor/filters/hexlify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/device/monitor/filters/log2file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/device/monitor/filters/send_on_enter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/device/monitor/filters/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/device/monitor/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.174891 platformio-6.1.8/platformio/home/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/home/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/home/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.174891 platformio-6.1.8/platformio/home/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/home/rpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.178891 platformio-6.1.8/platformio/home/rpc/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/home/rpc/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/home/rpc/handlers/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/home/rpc/handlers/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/home/rpc/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/home/rpc/handlers/ide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/home/rpc/handlers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/home/rpc/handlers/os.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/home/rpc/handlers/piocore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/home/rpc/handlers/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13217 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/home/rpc/handlers/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/home/rpc/handlers/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/home/rpc/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/home/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9143 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/maintenance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.182891 platformio-6.1.8/platformio/package/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.186891 platformio-6.1.8/platformio/package/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/commands/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/commands/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/commands/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/commands/outdated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/commands/pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/commands/publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/commands/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/commands/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/commands/uninstall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/commands/unpublish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8643 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/commands/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/lockfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.190892 platformio-6.1.8/platformio/package/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/manager/_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/manager/_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/manager/_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/manager/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/manager/_symlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/manager/_uninstall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/manager/_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/manager/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/manager/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/manager/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/manager/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.190892 platformio-6.1.8/platformio/package/manifest/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/manifest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24640 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/manifest/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/manifest/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16117 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/unpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/vcsclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/package/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.194892 platformio-6.1.8/platformio/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/platform/_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/platform/_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/platform/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/platform/board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/platform/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/platform/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/proc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.198892 platformio-6.1.8/platformio/project/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.198892 platformio-6.1.8/platformio/project/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12843 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/commands/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/commands/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.198892 platformio-6.1.8/platformio/project/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.122888 platformio-6.1.8/platformio/project/integration/tpls/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.198892 platformio-6.1.8/platformio/project/integration/tpls/clion/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/clion/.gitignore.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/clion/CMakeLists.txt.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/clion/CMakeListsPrivate.txt.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.198892 platformio-6.1.8/platformio/project/integration/tpls/codeblocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/codeblocks/platformio.cbp.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.202892 platformio-6.1.8/platformio/project/integration/tpls/eclipse/
+-rw-r--r--   0 runner    (1001) docker     (123)    20663 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/eclipse/.cproject.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/eclipse/.project.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.202892 platformio-6.1.8/platformio/project/integration/tpls/eclipse/.settings/
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/eclipse/.settings/PlatformIO Debugger.launch.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/eclipse/.settings/language.settings.xml.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/eclipse/.settings/org.eclipse.cdt.core.prefs.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.202892 platformio-6.1.8/platformio/project/integration/tpls/emacs/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/emacs/.ccls.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/emacs/.gitignore.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.122888 platformio-6.1.8/platformio/project/integration/tpls/netbeans/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.202892 platformio-6.1.8/platformio/project/integration/tpls/netbeans/nbproject/
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/netbeans/nbproject/configurations.xml.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.202892 platformio-6.1.8/platformio/project/integration/tpls/netbeans/nbproject/private/
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/netbeans/nbproject/private/configurations.xml.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/netbeans/nbproject/private/launcher.properties.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/netbeans/nbproject/private/private.xml.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/netbeans/nbproject/project.xml.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.206893 platformio-6.1.8/platformio/project/integration/tpls/qtcreator/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/qtcreator/.gitignore.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/qtcreator/Makefile.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/qtcreator/platformio.cflags.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/qtcreator/platformio.config.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/qtcreator/platformio.creator.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/qtcreator/platformio.cxxflags.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/qtcreator/platformio.files.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/qtcreator/platformio.includes.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.210893 platformio-6.1.8/platformio/project/integration/tpls/sublimetext/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/sublimetext/.ccls.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/sublimetext/platformio.sublime-project.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.210893 platformio-6.1.8/platformio/project/integration/tpls/vim/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/vim/.ccls.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/vim/.gitignore.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.210893 platformio-6.1.8/platformio/project/integration/tpls/visualstudio/
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/visualstudio/platformio.vcxproj.filters.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/visualstudio/platformio.vcxproj.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.210893 platformio-6.1.8/platformio/project/integration/tpls/vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/vscode/.gitignore.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.210893 platformio-6.1.8/platformio/project/integration/tpls/vscode/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/vscode/.vscode/c_cpp_properties.json.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/vscode/.vscode/extensions.json.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/integration/tpls/vscode/.vscode/launch.json.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)    31475 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/project/savedeps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/public.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.210893 platformio-6.1.8/platformio/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/registry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.214893 platformio-6.1.8/platformio/registry/access/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/registry/access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/registry/access/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.214893 platformio-6.1.8/platformio/registry/access/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/registry/access/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/registry/access/commands/grant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/registry/access/commands/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/registry/access/commands/private.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/registry/access/commands/public.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/registry/access/commands/revoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/registry/access/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/registry/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/registry/mirror.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.214893 platformio-6.1.8/platformio/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.214893 platformio-6.1.8/platformio/remote/ac/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/ac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/ac/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/ac/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/ac/psync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/ac/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11855 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.218893 platformio-6.1.8/platformio/remote/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/client/agent_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/client/agent_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/client/async_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/client/device_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/client/device_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/client/run_or_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/client/update_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.218893 platformio-6.1.8/platformio/remote/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/factory/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/factory/ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/remote/projectsync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.222894 platformio-6.1.8/platformio/run/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9788 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/run/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/run/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/run/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.222894 platformio-6.1.8/platformio/system/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/system/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.222894 platformio-6.1.8/platformio/system/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/system/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/system/commands/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/system/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/system/commands/prune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/system/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/system/prune.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/telemetry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.226894 platformio-6.1.8/platformio/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:56.000000 platformio-6.1.8/platformio/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.230894 platformio-6.1.8/platformio/test/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/reports/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/reports/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/reports/junit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/reports/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.230894 platformio-6.1.8/platformio/test/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/runners/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/runners/doctest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/runners/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/runners/googletest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.234894 platformio-6.1.8/platformio/test/runners/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/runners/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/runners/readers/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/runners/readers/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9696 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/test/runners/unity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-07-05 12:32:57.000000 platformio-6.1.8/platformio/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.134889 platformio-6.1.8/platformio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-07-05 12:47:07.000000 platformio-6.1.8/platformio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-07-05 12:47:07.000000 platformio-6.1.8/platformio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 12:47:07.000000 platformio-6.1.8/platformio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-05 12:47:07.000000 platformio-6.1.8/platformio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-05 12:47:07.000000 platformio-6.1.8/platformio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 12:47:07.000000 platformio-6.1.8/platformio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 12:47:07.234894 platformio-6.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-05 12:32:57.000000 platformio-6.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:47:07.234894 platformio-6.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-07-05 12:32:57.000000 platformio-6.1.8/tests/test_examples.py
```

### Comparing `platformio-6.1.7/LICENSE` & `platformio-6.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/PKG-INFO` & `platformio-6.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: platformio
-Version: 6.1.7
+Version: 6.1.8
 Summary: A professional collaborative platform for embedded development. Cross-platform IDE and Unified Debugger. Static Code Analyzer and Remote Unit Testing. Multi-platform and Multi-architecture Build System. Firmware File Explorer and Memory Inspection. IoT, Arduino, CMSIS, ESP-IDF, FreeRTOS, libOpenCM3, mbedOS, Pulp OS, SPL, STM32Cube, Zephyr RTOS, ARM, AVR, Espressif (ESP8266/ESP32), FPGA, MCS-51 (8051), MSP430, Nordic (nRF51/nRF52), NXP i.MX RT, PIC32, RISC-V, STMicroelectronics (STM8/STM32), Teensy
 Home-page: https://platformio.org
 Author: PlatformIO Labs
 Author-email: contact@piolabs.com
 License: Apache Software License
 Keywords: iot,embedded,arduino,mbed,esp8266,esp32,fpga,firmware,continuous-integration,cloud-ide,avr,arm,ide,unit-testing,hardware,verilog,microcontroller,debug
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
@@ -118,7 +119,8 @@
 
 The PlatformIO is licensed under the permissive Apache 2.0 license,
 so you can use it in both commercial and personal projects with confidence.
 
 .. image:: https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/banner-direct.svg
     :target: https://github.com/vshymanskyy/StandWithUkraine/blob/main/docs/README.md
     :alt:  SWUbanner
+
```

### Comparing `platformio-6.1.7/README.rst` & `platformio-6.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/__init__.py` & `platformio-6.1.8/platformio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-VERSION = (6, 1, 7)
+VERSION = (6, 1, 8)
 __version__ = ".".join([str(s) for s in VERSION])
 
 __title__ = "platformio"
 __description__ = (
     "A professional collaborative platform for embedded development. "
     "Cross-platform IDE and Unified Debugger. "
     "Static Code Analyzer and Remote Unit Testing. "
```

### Comparing `platformio-6.1.7/platformio/__main__.py` & `platformio-6.1.8/platformio/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import sys
-from traceback import format_exc
+import traceback
 
 import click
 
 from platformio import __version__, exception, maintenance
 from platformio.cli import PlatformioCLI
 from platformio.compat import IS_CYGWIN, ensure_python3
 
@@ -49,21 +49,21 @@
             == "true"
         ):
             # pylint: disable=protected-access
             click._compat.isatty = lambda stream: True
     except:  # pylint: disable=bare-except
         pass
 
-    maintenance.on_platformio_start(ctx, caller)
+    maintenance.on_cmd_start(ctx, caller)
 
 
 @cli.result_callback()
 @click.pass_context
-def process_result(ctx, result, *_, **__):
-    maintenance.on_platformio_end(ctx, result)
+def process_result(*_, **__):
+    maintenance.on_cmd_end()
 
 
 def configure():
     if IS_CYGWIN:
         raise exception.CygwinEnvDetected()
 
     # https://urllib3.readthedocs.org
@@ -92,47 +92,50 @@
 
 def main(argv=None):
     exit_code = 0
     prev_sys_argv = sys.argv[:]
     if argv:
         assert isinstance(argv, list)
         sys.argv = argv
+
     try:
         ensure_python3(raise_exception=True)
         configure()
         cli()  # pylint: disable=no-value-for-parameter
     except SystemExit as exc:
         if exc.code and str(exc.code).isdigit():
             exit_code = int(exc.code)
     except Exception as exc:  # pylint: disable=broad-except
         if not isinstance(exc, exception.ReturnErrorCode):
             maintenance.on_platformio_exception(exc)
-            error_str = "Error: "
+            error_str = f"{exc.__class__.__name__}: "
             if isinstance(exc, exception.PlatformioException):
                 error_str += str(exc)
             else:
-                error_str += format_exc()
+                error_str += traceback.format_exc()
                 error_str += """
 ============================================================
 
 An unexpected error occurred. Further steps:
 
 * Verify that you have the latest version of PlatformIO using
-  `pip install -U platformio` command
+  `python -m pip install -U platformio` command
 
 * Try to find answer in FAQ Troubleshooting section
   https://docs.platformio.org/page/faq/index.html
 
 * Report this problem to the developers
   https://github.com/platformio/platformio-core/issues
 
 ============================================================
 """
             click.secho(error_str, fg="red", err=True)
         exit_code = int(str(exc)) if str(exc).isdigit() else 1
+
+    maintenance.on_platformio_exit()
     sys.argv = prev_sys_argv
     return exit_code
 
 
 def debug_gdb_main():
     return main([sys.argv[0], "debug", "--interface", "gdb"] + sys.argv[1:])
```

### Comparing `platformio-6.1.7/platformio/account/__init__.py` & `platformio-6.1.8/platformio/account/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/account/cli.py` & `platformio-6.1.8/platformio/account/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/account/client.py` & `platformio-6.1.8/platformio/account/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import time
 
 from platformio import __accounts_api__, app
-from platformio.exception import PlatformioException
+from platformio.exception import PlatformioException, UserSideException
 from platformio.http import HTTPClient, HTTPClientError
 
 
 class AccountError(PlatformioException):
     MESSAGE = "{0}"
 
 
-class AccountNotAuthorized(AccountError):
+class AccountNotAuthorized(AccountError, UserSideException):
     MESSAGE = "You are not authorized! Please log in to PlatformIO Account."
 
 
-class AccountAlreadyAuthorized(AccountError):
+class AccountAlreadyAuthorized(AccountError, UserSideException):
     MESSAGE = "You are already authorized with {0} account."
 
 
 class AccountClient(HTTPClient):  # pylint:disable=too-many-public-methods
     SUMMARY_CACHE_TTL = 60 * 60 * 24 * 7
 
     def __init__(self):
```

### Comparing `platformio-6.1.7/platformio/account/commands/__init__.py` & `platformio-6.1.8/platformio/account/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/account/commands/destroy.py` & `platformio-6.1.8/platformio/account/commands/destroy.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/account/commands/forgot.py` & `platformio-6.1.8/platformio/account/commands/forgot.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/account/commands/login.py` & `platformio-6.1.8/platformio/account/commands/login.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/account/commands/logout.py` & `platformio-6.1.8/platformio/account/commands/logout.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/account/commands/password.py` & `platformio-6.1.8/platformio/account/commands/password.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/account/commands/register.py` & `platformio-6.1.8/platformio/account/commands/register.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/account/commands/show.py` & `platformio-6.1.8/platformio/account/commands/show.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/account/commands/token.py` & `platformio-6.1.8/platformio/account/commands/token.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/account/commands/update.py` & `platformio-6.1.8/platformio/account/commands/update.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/account/org/__init__.py` & `platformio-6.1.8/platformio/account/org/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/account/org/cli.py` & `platformio-6.1.8/platformio/account/org/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/account/org/commands/__init__.py` & `platformio-6.1.8/platformio/account/org/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/account/org/commands/add.py` & `platformio-6.1.8/platformio/account/org/commands/add.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/account/org/commands/create.py` & `platformio-6.1.8/platformio/account/org/commands/create.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/account/org/commands/destroy.py` & `platformio-6.1.8/platformio/account/org/commands/destroy.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/account/org/commands/list.py` & `platformio-6.1.8/platformio/account/org/commands/list.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/account/org/commands/remove.py` & `platformio-6.1.8/platformio/account/org/commands/remove.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/account/org/commands/update.py` & `platformio-6.1.8/platformio/account/org/commands/update.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/account/team/__init__.py` & `platformio-6.1.8/platformio/account/team/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/account/team/cli.py` & `platformio-6.1.8/platformio/account/team/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/account/team/commands/__init__.py` & `platformio-6.1.8/platformio/account/team/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/account/team/commands/add.py` & `platformio-6.1.8/platformio/account/team/commands/add.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/account/team/commands/create.py` & `platformio-6.1.8/platformio/account/team/commands/create.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/account/team/commands/destroy.py` & `platformio-6.1.8/platformio/account/team/commands/destroy.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/account/team/commands/list.py` & `platformio-6.1.8/platformio/account/team/commands/list.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/account/team/commands/remove.py` & `platformio-6.1.8/platformio/account/team/commands/remove.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/account/team/commands/update.py` & `platformio-6.1.8/platformio/account/team/commands/update.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/account/validate.py` & `platformio-6.1.8/platformio/account/validate.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/app.py` & `platformio-6.1.8/platformio/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 import getpass
 import hashlib
 import json
 import os
 import platform
 import socket
+import time
 import uuid
 
 from platformio import __version__, exception, fs, proc
 from platformio.compat import IS_WINDOWS, hashlib_encode_data
 from platformio.package.lockfile import LockFile
 from platformio.project.config import ProjectConfig
 from platformio.project.helpers import get_default_projects_dir
@@ -64,26 +65,31 @@
     },
 }
 
 SESSION_VARS = {
     "command_ctx": None,
     "caller_id": None,
     "custom_project_conf": None,
+    "pause_telemetry": False,
 }
 
 
+def resolve_state_path(conf_option_dir, file_name, ensure_dir_exists=True):
+    state_dir = ProjectConfig.get_instance().get("platformio", conf_option_dir)
+    if ensure_dir_exists and not os.path.isdir(state_dir):
+        os.makedirs(state_dir)
+    return os.path.join(state_dir, file_name)
+
+
 class State:
     def __init__(self, path=None, lock=False):
         self.path = path
         self.lock = lock
         if not self.path:
-            core_dir = ProjectConfig.get_instance().get("platformio", "core_dir")
-            if not os.path.isdir(core_dir):
-                os.makedirs(core_dir)
-            self.path = os.path.join(core_dir, "appstate.json")
+            self.path = resolve_state_path("core_dir", "appstate.json")
         self._storage = {}
         self._lockfile = None
         self.modified = False
 
     def __enter__(self):
         try:
             self._lock_state_file()
@@ -244,14 +250,15 @@
         uid = os.getenv("GITPOD_GIT_USER_NAME")
     if not uid:
         uid = uuid.getnode()
     cid = uuid.UUID(bytes=hashlib.md5(hashlib_encode_data(uid)).digest())
     cid = str(cid)
     if IS_WINDOWS or os.getuid() > 0:  # pylint: disable=no-member
         set_state_item("cid", cid)
+        set_state_item("created_at", int(time.time()))
     return cid
 
 
 def get_user_agent():
     data = [
         "PlatformIO/%s" % __version__,
         "CI/%d" % int(proc.is_ci()),
```

### Comparing `platformio-6.1.7/platformio/assets/system/99-platformio-udev.rules` & `platformio-6.1.8/platformio/assets/system/99-platformio-udev.rules`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/assets/templates/ide-projects/clion/CMakeLists.txt.tpl` & `platformio-6.1.8/platformio/project/integration/tpls/clion/CMakeLists.txt.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/assets/templates/ide-projects/clion/CMakeListsPrivate.txt.tpl` & `platformio-6.1.8/platformio/project/integration/tpls/clion/CMakeListsPrivate.txt.tpl`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # If you need to override existing CMake configuration or add extra,
 # please create `CMakeListsUser.txt` in the root of project.
 # The `CMakeListsUser.txt` will not be overwritten by PlatformIO.
 
 % import os
 % import re
 %
+% from platformio.compat import shlex_join
 % from platformio.project.helpers import load_build_metadata
 %
 % def _normalize_path(path):
 %   if project_dir in path:
 %     path = path.replace(project_dir, "${CMAKE_CURRENT_LIST_DIR}")
 %   elif user_home_dir in path:
 %     if "windows" in systype:
@@ -60,25 +61,24 @@
 
 % if svd_path:
 set(CLION_SVD_FILE_PATH "{{ _normalize_path(svd_path) }}" CACHE FILEPATH "Peripheral Registers Definitions File" FORCE)
 % end
 
 SET(CMAKE_C_COMPILER "{{ _normalize_path(cc_path) }}")
 SET(CMAKE_CXX_COMPILER "{{ _normalize_path(cxx_path) }}")
-SET(CMAKE_CXX_FLAGS "{{ _normalize_path(to_unix_path(cxx_flags)) }}")
-SET(CMAKE_C_FLAGS "{{ _normalize_path(to_unix_path(cc_flags)) }}")
+SET(CMAKE_CXX_FLAGS {{ _normalize_path(to_unix_path(shlex_join(cxx_flags))) }})
+SET(CMAKE_C_FLAGS {{ _normalize_path(to_unix_path(shlex_join(cc_flags))) }})
 
-% STD_RE = re.compile(r"\-std=[a-z\+]+(\w+)")
-% cc_stds = STD_RE.findall(cc_flags)
-% cxx_stds = STD_RE.findall(cxx_flags)
+% cc_stds = [arg for arg in cc_flags if arg.startswith("-std=")]
+% cxx_stds = [arg for arg in cxx_flags if arg.startswith("-std=")]
 % if cc_stds:
-SET(CMAKE_C_STANDARD {{ cc_stds[-1] }})
+SET(CMAKE_C_STANDARD {{ cc_stds[-1][-2:] }})
 % end
 % if cxx_stds:
-set(CMAKE_CXX_STANDARD {{ cxx_stds[-1] }})
+set(CMAKE_CXX_STANDARD {{ cxx_stds[-1][-2:] }})
 % end
 
 if (CMAKE_BUILD_TYPE MATCHES "{{ env_name }}")
 % for define in defines:
     add_definitions(-D{{!re.sub(r"([\"\(\)\ #])", r"\\\1", define)}})
 % end
```

### Comparing `platformio-6.1.7/platformio/assets/templates/ide-projects/codeblocks/platformio.cbp.tpl` & `platformio-6.1.8/platformio/project/integration/tpls/codeblocks/platformio.cbp.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/assets/templates/ide-projects/eclipse/.cproject.tpl` & `platformio-6.1.8/platformio/project/integration/tpls/eclipse/.cproject.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/assets/templates/ide-projects/eclipse/.project.tpl` & `platformio-6.1.8/platformio/project/integration/tpls/eclipse/.project.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/assets/templates/ide-projects/eclipse/.settings/PlatformIO Debugger.launch.tpl` & `platformio-6.1.8/platformio/project/integration/tpls/eclipse/.settings/PlatformIO Debugger.launch.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/assets/templates/ide-projects/eclipse/.settings/language.settings.xml.tpl` & `platformio-6.1.8/platformio/project/integration/tpls/eclipse/.settings/language.settings.xml.tpl`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-% import re
-% STD_RE = re.compile(r"(\-std=[a-z\+]+\w+)")
-% cxx_stds = STD_RE.findall(cxx_flags)
+% cxx_stds = [arg for arg in cxx_flags if arg.startswith("-std=")]
 % cxx_std = cxx_stds[-1] if cxx_stds else ""
 %
 % if cxx_path.startswith(user_home_dir):
 % if "windows" in systype:
 %    cxx_path = "${USERPROFILE}" + cxx_path.replace(user_home_dir, "")
 % else:
 %    cxx_path = "${HOME}" + cxx_path.replace(user_home_dir, "")
```

### Comparing `platformio-6.1.7/platformio/assets/templates/ide-projects/eclipse/.settings/org.eclipse.cdt.core.prefs.tpl` & `platformio-6.1.8/platformio/project/integration/tpls/eclipse/.settings/org.eclipse.cdt.core.prefs.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/assets/templates/ide-projects/netbeans/nbproject/configurations.xml.tpl` & `platformio-6.1.8/platformio/project/integration/tpls/netbeans/nbproject/configurations.xml.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/assets/templates/ide-projects/netbeans/nbproject/private/configurations.xml.tpl` & `platformio-6.1.8/platformio/project/integration/tpls/netbeans/nbproject/private/configurations.xml.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/assets/templates/ide-projects/netbeans/nbproject/private/launcher.properties.tpl` & `platformio-6.1.8/platformio/project/integration/tpls/netbeans/nbproject/private/launcher.properties.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/assets/templates/ide-projects/netbeans/nbproject/project.xml.tpl` & `platformio-6.1.8/platformio/project/integration/tpls/netbeans/nbproject/project.xml.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/assets/templates/ide-projects/sublimetext/platformio.sublime-project.tpl` & `platformio-6.1.8/platformio/project/integration/tpls/sublimetext/platformio.sublime-project.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/assets/templates/ide-projects/visualstudio/platformio.vcxproj.filters.tpl` & `platformio-6.1.8/platformio/project/integration/tpls/visualstudio/platformio.vcxproj.filters.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/assets/templates/ide-projects/visualstudio/platformio.vcxproj.tpl` & `platformio-6.1.8/platformio/project/integration/tpls/visualstudio/platformio.vcxproj.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/assets/templates/ide-projects/vscode/.vscode/c_cpp_properties.json.tpl` & `platformio-6.1.8/platformio/project/integration/tpls/vscode/.vscode/c_cpp_properties.json.tpl`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,50 @@
 % import os
 % import platform
-% import re
-%
-% import click
 %
 % systype = platform.system().lower()
 %
 % cpp_standards_remap = {
-%   "0x": "11",
-%   "1y": "14",
-%   "1z": "17",
-%   "2a": "20",
-%   "2b": "23"
+%   "c++0x": "c++11",
+%   "c++1y": "c++14",
+%   "c++1z": "c++17",
+%   "c++2a": "c++20",
+%   "c++2b": "c++23",
+%   "gnu++0x": "gnu++11",
+%   "gnu++1y": "gnu++14",
+%   "gnu++1z": "gnu++17",
+%   "gnu++2a": "gnu++20",
+%   "gnu++2b": "gnu++23"
 % }
 %
 % def _escape(text):
 %   return to_unix_path(text).replace('"', '\\"')
 % end
 %
-% def split_args(args_string):
-%   return click.parser.split_arg_string(to_unix_path(args_string))
-% end
-%
 % def filter_args(args, allowed, ignore=None):
 %   if not allowed:
 %     return []
 %   end
 %
 %   ignore = ignore or []
 %   result = []
 %   i = 0
 %   length = len(args)
-%     while(i < length):
-%      if any(args[i].startswith(f) for f in allowed) and not any(
-%        args[i].startswith(f) for f in ignore):
-%        result.append(args[i])
-%        if i + 1 < length and not args[i + 1].startswith("-"):
-%          i += 1
-%          result.append(args[i])
-%        end
+%   while(i < length):
+%     if any(args[i].startswith(f) for f in allowed) and not any(
+%           args[i].startswith(f) for f in ignore):
+%       result.append(args[i])
+%       if i + 1 < length and not args[i + 1].startswith("-"):
+%         i += 1
+%         result.append(args[i])
 %       end
-%      i += 1
-%    end
-%    return result
+%     end
+%     i += 1
+%   end
+%   return result
 % end
 %
 % def _find_abs_path(inc, inc_paths):
 %   for path in inc_paths:
 %     if os.path.isfile(os.path.join(path, inc)):
 %       return os.path.join(path, inc)
 %     end
@@ -72,20 +70,18 @@
 %     end
 %   end
 %   return result
 % end
 %
 % cleaned_includes = filter_includes(includes, ["toolchain"])
 %
-% STD_RE = re.compile(r"\-std=[a-z\+]+(\w+)")
-% cc_stds = STD_RE.findall(cc_flags)
-% cxx_stds = STD_RE.findall(cxx_flags)
-% cc_m_flags = split_args(cc_flags)
+% cc_stds = [arg[5:] for arg in cc_flags if arg.startswith("-std=")]
+% cxx_stds = [arg[5:] for arg in cxx_flags if arg.startswith("-std=")]
 % forced_includes = _find_forced_includes(
-%   filter_args(cc_m_flags, ["-include", "-imacros"]), cleaned_includes)
+%   filter_args(cc_flags, ["-include", "-imacros"]), cleaned_includes)
 %
 //
 // !!! WARNING !!! AUTO-GENERATED FILE!
 // PLEASE DO NOT MODIFY IT AND USE "platformio.ini":
 // https://docs.platformio.org/page/projectconf/section_env_build.html#build-flags
 //
 {
@@ -110,31 +106,31 @@
             "defines": [
 % for define in defines:
                 "{{! _escape(define) }}",
 % end
                 ""
             ],
 % if cc_stds:
-            "cStandard": "c{{ cc_stds[-1] }}",
+            "cStandard": "{{ cc_stds[-1] }}",
 % end
 % if cxx_stds:
-            "cppStandard": "c++{{ cpp_standards_remap.get(cxx_stds[-1], cxx_stds[-1]) }}",
+            "cppStandard": "{{ cpp_standards_remap.get(cxx_stds[-1], cxx_stds[-1]) }}",
 % end
 % if forced_includes:
             "forcedInclude": [
 % for include in forced_includes:
                 "{{ include }}",
 % end
                 ""
             ],
 % end
             "compilerPath": "{{ cc_path }}",
             "compilerArgs": [
 % for flag in [
-%     f for f in filter_args(cc_m_flags, ["-m", "-i", "@"], ["-include", "-imacros"])
+%     f for f in filter_args(cc_flags, ["-m", "-i", "@"], ["-include", "-imacros"])
 % ]:
                 "{{ flag }}",
 % end
                 ""
             ]
         }
     ],
```

### Comparing `platformio-6.1.7/platformio/assets/templates/ide-projects/vscode/.vscode/extensions.json.tpl` & `platformio-6.1.8/platformio/project/integration/tpls/vscode/.vscode/extensions.json.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/assets/templates/ide-projects/vscode/.vscode/launch.json.tpl` & `platformio-6.1.8/platformio/project/integration/tpls/vscode/.vscode/launch.json.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/builder/__init__.py` & `platformio-6.1.8/platformio/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/builder/main.py` & `platformio-6.1.8/platformio/builder/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,16 @@
         "piointegration",
         "piomaxlen",
     ],
     toolpath=[os.path.join(fs.get_source_dir(), "builder", "tools")],
     variables=clivars,
     # Propagating External Environment
     ENV=os.environ,
-    UNIX_TIME=int(time()),
+    TIMESTAMP=int(time()),
+    UNIX_TIME="$TIMESTAMP",  # deprecated
     BUILD_DIR=os.path.join("$PROJECT_BUILD_DIR", "$PIOENV"),
     BUILD_SRC_DIR=os.path.join("$BUILD_DIR", "src"),
     BUILD_TEST_DIR=os.path.join("$BUILD_DIR", "test"),
     COMPILATIONDB_PATH=os.path.join("$PROJECT_DIR", "compile_commands.json"),
     LIBPATH=["$BUILD_DIR"],
     PROGNAME="program",
     PROGPATH=os.path.join("$BUILD_DIR", "$PROGNAME$PROGSUFFIX"),
```

### Comparing `platformio-6.1.7/platformio/builder/tools/__init__.py` & `platformio-6.1.8/platformio/builder/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/builder/tools/pioasm.py` & `platformio-6.1.8/platformio/builder/tools/pioasm.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/builder/tools/piobuild.py` & `platformio-6.1.8/platformio/builder/tools/piobuild.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,21 +196,24 @@
             value = float(value)
         cppdefines.append((name, value))
     result["CPPDEFINES"] = cppdefines
 
     # fix relative CPPPATH & LIBPATH
     for k in ("CPPPATH", "LIBPATH"):
         for i, p in enumerate(result.get(k, [])):
+            p = env.subst(p)
             if os.path.isdir(p):
                 result[k][i] = os.path.abspath(p)
 
     # fix relative path for "-include"
     for i, f in enumerate(result.get("CCFLAGS", [])):
         if isinstance(f, tuple) and f[0] == "-include":
-            result["CCFLAGS"][i] = (f[0], env.File(os.path.abspath(f[1].get_path())))
+            p = env.subst(f[1].get_path())
+            if os.path.exists(p):
+                result["CCFLAGS"][i] = (f[0], os.path.abspath(p))
 
     return result
 
 
 def ProcessFlags(env, flags):  # pylint: disable=too-many-branches
     if not flags:
         return
```

### Comparing `platformio-6.1.7/platformio/builder/tools/piohooks.py` & `platformio-6.1.8/platformio/builder/tools/piohooks.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/builder/tools/pioino.py` & `platformio-6.1.8/platformio/builder/tools/pioino.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/builder/tools/piointegration.py` & `platformio-6.1.8/platformio/builder/tools/piointegration.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import glob
 import os
 
+import click
 import SCons.Defaults  # pylint: disable=import-error
 import SCons.Subst  # pylint: disable=import-error
 from SCons.Script import COMMAND_LINE_TARGETS  # pylint: disable=import-error
 
 from platformio.proc import exec_command, where_is_program
 
 
@@ -150,16 +151,20 @@
         "build_type": globalenv.GetBuildType(),
         "env_name": globalenv["PIOENV"],
         "libsource_dirs": [
             globalenv.subst(item) for item in globalenv.GetLibSourceDirs()
         ],
         "defines": dump_defines(projenv),
         "includes": projenv.DumpIntegrationIncludes(),
-        "cc_flags": _subst_cmd(projenv, "$CFLAGS $CCFLAGS $CPPFLAGS"),
-        "cxx_flags": _subst_cmd(projenv, "$CXXFLAGS $CCFLAGS $CPPFLAGS"),
+        "cc_flags": click.parser.split_arg_string(
+            _subst_cmd(projenv, "$CFLAGS $CCFLAGS $CPPFLAGS")
+        ),
+        "cxx_flags": click.parser.split_arg_string(
+            _subst_cmd(projenv, "$CXXFLAGS $CCFLAGS $CPPFLAGS")
+        ),
         "cc_path": where_is_program(
             globalenv.subst("$CC"), globalenv.subst("${ENV['PATH']}")
         ),
         "cxx_path": where_is_program(
             globalenv.subst("$CXX"), globalenv.subst("${ENV['PATH']}")
         ),
         "gdb_path": where_is_program(
```

### Comparing `platformio-6.1.7/platformio/builder/tools/piolib.py` & `platformio-6.1.8/platformio/builder/tools/piolib.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/builder/tools/piomaxlen.py` & `platformio-6.1.8/platformio/builder/tools/piomaxlen.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/builder/tools/piomisc.py` & `platformio-6.1.8/platformio/builder/tools/piomisc.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/builder/tools/pioplatform.py` & `platformio-6.1.8/platformio/builder/tools/pioplatform.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/builder/tools/pioproject.py` & `platformio-6.1.8/platformio/builder/tools/pioproject.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/builder/tools/piosize.py` & `platformio-6.1.8/platformio/builder/tools/piosize.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/builder/tools/piotarget.py` & `platformio-6.1.8/platformio/builder/tools/piotarget.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/builder/tools/piotest.py` & `platformio-6.1.8/platformio/builder/tools/piotest.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/builder/tools/pioupload.py` & `platformio-6.1.8/platformio/builder/tools/pioupload.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/cache.py` & `platformio-6.1.8/platformio/cache.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/check/__init__.py` & `platformio-6.1.8/platformio/check/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/check/cli.py` & `platformio-6.1.8/platformio/check/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/check/defect.py` & `platformio-6.1.8/platformio/check/defect.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/check/tools/__init__.py` & `platformio-6.1.8/platformio/check/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/check/tools/base.py` & `platformio-6.1.8/platformio/check/tools/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,16 +56,16 @@
             for s in self.options["severity"]
         ]
 
     def _load_cpp_data(self):
         data = load_build_metadata(self.project_dir, self.envname)
         if not data:
             return
-        self.cc_flags = click.parser.split_arg_string(data.get("cc_flags", ""))
-        self.cxx_flags = click.parser.split_arg_string(data.get("cxx_flags", ""))
+        self.cc_flags = data.get("cc_flags", [])
+        self.cxx_flags = data.get("cxx_flags", [])
         self.cpp_includes = self._dump_includes(data.get("includes", {}))
         self.cpp_defines = data.get("defines", [])
         self.cc_path = data.get("cc_path")
         self.cxx_path = data.get("cxx_path")
         self.toolchain_defines = self._get_toolchain_defines()
 
     def get_tool_dir(self, pkg_name):
```

### Comparing `platformio-6.1.7/platformio/check/tools/clangtidy.py` & `platformio-6.1.8/platformio/check/tools/clangtidy.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/check/tools/cppcheck.py` & `platformio-6.1.8/platformio/check/tools/cppcheck.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/check/tools/pvsstudio.py` & `platformio-6.1.8/platformio/check/tools/pvsstudio.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/cli.py` & `platformio-6.1.8/platformio/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -59,14 +59,29 @@
                 args[0] == "debug" and "--interpreter" in " ".join(args),
                 args[0] == "upgrade",
                 "--json-output" in args,
                 "--version" in args,
             ]
         )
 
+    @classmethod
+    def reveal_cmd_path_args(cls, ctx):
+        result = []
+        group = ctx.command
+        args = cls.leftover_args[::]
+        while args:
+            cmd_name = args.pop(0)
+            next_group = group.get_command(ctx, cmd_name)
+            if next_group:
+                group = next_group
+                result.append(cmd_name)
+            if not hasattr(group, "get_command"):
+                break
+        return result
+
     def invoke(self, ctx):
         PlatformioCLI.leftover_args = ctx.args
         if hasattr(ctx, "protected_args"):
             PlatformioCLI.leftover_args = ctx.protected_args + ctx.args
         return super().invoke(ctx)
 
     def list_commands(self, ctx):
```

### Comparing `platformio-6.1.7/platformio/commands/__init__.py` & `platformio-6.1.8/platformio/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/commands/boards.py` & `platformio-6.1.8/platformio/commands/boards.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/commands/ci.py` & `platformio-6.1.8/platformio/commands/ci.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/commands/device/__init__.py` & `platformio-6.1.8/platformio/commands/device/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/commands/lib.py` & `platformio-6.1.8/platformio/commands/lib.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/commands/platform.py` & `platformio-6.1.8/platformio/commands/platform.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/commands/settings.py` & `platformio-6.1.8/platformio/commands/settings.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/commands/update.py` & `platformio-6.1.8/platformio/commands/update.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/commands/upgrade.py` & `platformio-6.1.8/platformio/commands/upgrade.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,24 +49,23 @@
     to_develop = dev or not all(c.isdigit() for c in __version__ if c != ".")
     pkg_spec = DEVELOP_ZIP_URL if to_develop else "platformio"
 
     try:
         subprocess.run(
             [python_exe, "-m", "pip", "install", "--upgrade", pkg_spec],
             check=True,
-            capture_output=not verbose,
+            stdout=subprocess.PIPE if not verbose else None,
         )
-        r = subprocess.run(
+        output = subprocess.run(
             [python_exe, "-m", "platformio", "--version"],
             check=True,
-            capture_output=True,
-            text=True,
-        )
-        assert "version" in r.stdout
-        actual_version = r.stdout.split("version", 1)[1].strip()
+            stdout=subprocess.PIPE,
+        ).stdout.decode()
+        assert "version" in output
+        actual_version = output.split("version", 1)[1].strip()
         click.secho(
             "PlatformIO has been successfully upgraded to %s" % actual_version,
             fg="green",
         )
         click.echo("Release notes: ", nl=False)
         click.secho("https://docs.platformio.org/en/latest/history.html", fg="cyan")
         if app.get_session_var("caller_id"):
```

### Comparing `platformio-6.1.7/platformio/compat.py` & `platformio-6.1.8/platformio/compat.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,26 +13,41 @@
 # limitations under the License.
 
 # pylint: disable=unused-import,no-name-in-module
 
 import importlib.util
 import inspect
 import locale
+import shlex
 import sys
 
 from platformio.exception import UserSideException
 
 if sys.version_info >= (3, 7):
     from asyncio import create_task as aio_create_task
     from asyncio import get_running_loop as aio_get_running_loop
 else:
     from asyncio import ensure_future as aio_create_task
     from asyncio import get_event_loop as aio_get_running_loop
 
 
+if sys.version_info >= (3, 8):
+    from shlex import join as shlex_join
+else:
+
+    def shlex_join(split_command):
+        return " ".join(shlex.quote(arg) for arg in split_command)
+
+
+if sys.version_info >= (3, 9):
+    from asyncio import to_thread as aio_to_thread
+else:
+    from starlette.concurrency import run_in_threadpool as aio_to_thread
+
+
 PY2 = sys.version_info[0] == 2  # DO NOT REMOVE IT. ESP8266/ESP32 depend on it
 IS_CYGWIN = sys.platform.startswith("cygwin")
 IS_WINDOWS = WINDOWS = sys.platform.startswith("win")
 IS_MACOS = sys.platform.startswith("darwin")
 MISSING = object()
 string_types = (str,)
```

### Comparing `platformio-6.1.7/platformio/debug/__init__.py` & `platformio-6.1.8/platformio/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/debug/cli.py` & `platformio-6.1.8/platformio/debug/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/debug/config/__init__.py` & `platformio-6.1.8/platformio/debug/config/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/debug/config/base.py` & `platformio-6.1.8/platformio/debug/config/base.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/debug/config/blackmagic.py` & `platformio-6.1.8/platformio/debug/config/blackmagic.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/debug/config/factory.py` & `platformio-6.1.8/platformio/debug/config/factory.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/debug/config/generic.py` & `platformio-6.1.8/platformio/debug/config/generic.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/debug/config/jlink.py` & `platformio-6.1.8/platformio/debug/config/jlink.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/debug/config/mspdebug.py` & `platformio-6.1.8/platformio/debug/config/mspdebug.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/debug/config/native.py` & `platformio-6.1.8/platformio/debug/config/native.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/debug/config/qemu.py` & `platformio-6.1.8/platformio/debug/config/qemu.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/debug/config/renode.py` & `platformio-6.1.8/platformio/debug/config/renode.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/debug/exception.py` & `platformio-6.1.8/platformio/debug/exception.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,7 +26,11 @@
         "platformio-core/issues \nor visit -> https://docs.platformio.org"
         "/page/plus/debugging.html"
     )
 
 
 class DebugInvalidOptionsError(DebugError, UserSideException):
     pass
+
+
+class DebugInitError(DebugError, UserSideException):
+    pass
```

### Comparing `platformio-6.1.7/platformio/debug/helpers.py` & `platformio-6.1.8/platformio/debug/helpers.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/debug/process/__init__.py` & `platformio-6.1.8/platformio/debug/process/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/debug/process/base.py` & `platformio-6.1.8/platformio/debug/process/base.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/debug/process/client.py` & `platformio-6.1.8/platformio/debug/process/client.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/debug/process/gdb.py` & `platformio-6.1.8/platformio/debug/process/gdb.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
-import re
 import signal
 import time
 
 from platformio import telemetry
 from platformio.compat import aio_get_running_loop, is_bytes
 from platformio.debug import helpers
+from platformio.debug.exception import DebugInitError
 from platformio.debug.process.client import DebugClientProcess
 
 
 class GDBClientProcess(DebugClientProcess):
     PIO_SRC_NAME = ".pioinit"
     INIT_COMPLETED_BANNER = "PlatformIO: Initialization completed"
 
@@ -126,19 +126,15 @@
         self.transport.get_pipe_transport(0).write(data)
 
     def stdout_data_received(self, data):
         super().stdout_data_received(data)
         self._handle_error(data)
         # go to init break automatically
         if self.INIT_COMPLETED_BANNER.encode() in data:
-            telemetry.send_event(
-                "Debug",
-                "Started",
-                telemetry.dump_run_environment(self.debug_config.env_options),
-            )
+            telemetry.log_debug_started(self.debug_config)
             self._auto_exec_continue()
 
     def console_log(self, msg):
         if helpers.is_gdbmi_mode():
             msg = helpers.escape_gdbmi_stream("~", msg)
         self.stdout_data_received(msg if is_bytes(msg) else msg.encode())
 
@@ -175,18 +171,11 @@
     def _handle_error(self, data):
         self._errors_buffer = (self._errors_buffer + data)[-8192:]  # keep last 8 KBytes
         if not (
             self.PIO_SRC_NAME.encode() in self._errors_buffer
             and b"Error in sourced" in self._errors_buffer
         ):
             return
-
-        last_erros = self._errors_buffer.decode()
-        last_erros = " ".join(reversed(last_erros.split("\n")))
-        last_erros = re.sub(r'((~|&)"|\\n\"|\\t)', " ", last_erros, flags=re.M)
-
-        err = "%s -> %s" % (
-            telemetry.dump_run_environment(self.debug_config.env_options),
-            last_erros,
+        telemetry.log_debug_exception(
+            DebugInitError(self._errors_buffer.decode()), self.debug_config
         )
-        telemetry.send_exception("DebugInitError: %s" % err)
         self.transport.close()
```

### Comparing `platformio-6.1.7/platformio/debug/process/server.py` & `platformio-6.1.8/platformio/debug/process/server.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/device/__init__.py` & `platformio-6.1.8/platformio/device/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/device/cli.py` & `platformio-6.1.8/platformio/device/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/device/finder.py` & `platformio-6.1.8/platformio/device/finder.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,15 @@
         return best_port or port
 
     def _reveal_device_port(self, device):
         candidates = []
         for item in list_serial_ports(as_objects=True):
             if item.vid == device.vid and item.pid == device.pid:
                 candidates.append(item)
-        if len(candidates) == 1:
+        if len(candidates) <= 1:
             return device.device
         for item in candidates:
             if ("GDB" if self.prefer_gdb_port else "UART") in item.description:
                 return item.device
         candidates = sorted(candidates, key=lambda item: item.device)
         # first port is GDB? BlackMagic, ESP-Prog
         return candidates[0 if self.prefer_gdb_port else -1].device
```

### Comparing `platformio-6.1.7/platformio/device/list/__init__.py` & `platformio-6.1.8/platformio/device/list/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/device/list/command.py` & `platformio-6.1.8/platformio/device/list/command.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/device/list/util.py` & `platformio-6.1.8/platformio/device/list/util.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/device/monitor/__init__.py` & `platformio-6.1.8/platformio/device/monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/device/monitor/command.py` & `platformio-6.1.8/platformio/device/monitor/command.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/device/monitor/filters/__init__.py` & `platformio-6.1.8/platformio/device/monitor/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/device/monitor/filters/base.py` & `platformio-6.1.8/platformio/device/monitor/filters/base.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/device/monitor/filters/hexlify.py` & `platformio-6.1.8/platformio/device/monitor/filters/hexlify.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/device/monitor/filters/log2file.py` & `platformio-6.1.8/platformio/device/monitor/filters/log2file.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/device/monitor/filters/send_on_enter.py` & `platformio-6.1.8/platformio/device/monitor/filters/send_on_enter.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/device/monitor/filters/time.py` & `platformio-6.1.8/platformio/device/monitor/filters/time.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/device/monitor/terminal.py` & `platformio-6.1.8/platformio/device/monitor/terminal.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/exception.py` & `platformio-6.1.8/platformio/exception.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     MESSAGE = "Invalid setting with the name '{0}'"
 
 
 class InvalidSettingValue(UserSideException):
     MESSAGE = "Invalid value '{0}' for the setting '{1}'"
 
 
-class InvalidJSONFile(PlatformioException):
+class InvalidJSONFile(ValueError, UserSideException):
     MESSAGE = "Could not load broken JSON: {0}"
 
 
 class CIBuildEnvsEmpty(UserSideException):
     MESSAGE = (
         "Can't find PlatformIO build environments.\n"
         "Please specify `--board` or path to `platformio.ini` with "
```

### Comparing `platformio-6.1.7/platformio/fs.py` & `platformio-6.1.8/platformio/fs.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/home/__init__.py` & `platformio-6.1.8/platformio/home/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/home/cli.py` & `platformio-6.1.8/platformio/home/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/home/rpc/__init__.py` & `platformio-6.1.8/platformio/home/rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/home/rpc/handlers/__init__.py` & `platformio-6.1.8/platformio/home/rpc/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/home/rpc/handlers/account.py` & `platformio-6.1.8/platformio/home/rpc/handlers/account.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/home/rpc/handlers/app.py` & `platformio-6.1.8/platformio/home/rpc/handlers/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,20 +8,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import os
 from pathlib import Path
 
 from platformio import __version__, app, fs, util
 from platformio.home.rpc.handlers.base import BaseRPCHandler
-from platformio.project.config import ProjectConfig
 from platformio.project.helpers import is_platformio_project
 
 
 class AppRPC(BaseRPCHandler):
     IGNORE_STORAGE_KEYS = [
         "cid",
         "coreVersion",
@@ -29,23 +27,18 @@
         "coreCaller",
         "coreSettings",
         "homeDir",
         "projectsDir",
     ]
 
     @staticmethod
-    def get_state_path():
-        core_dir = ProjectConfig.get_instance().get("platformio", "core_dir")
-        if not os.path.isdir(core_dir):
-            os.makedirs(core_dir)
-        return os.path.join(core_dir, "homestate.json")
-
-    @staticmethod
     def load_state():
-        with app.State(AppRPC.get_state_path(), lock=True) as state:
+        with app.State(
+            app.resolve_state_path("core_dir", "homestate.json"), lock=True
+        ) as state:
             storage = state.get("storage", {})
 
             # base data
             caller_id = app.get_session_var("caller_id")
             storage["cid"] = app.get_cid()
             storage["coreVersion"] = __version__
             storage["coreSystype"] = util.get_systype()
@@ -77,15 +70,17 @@
 
     @staticmethod
     def get_state():
         return AppRPC.load_state()
 
     @staticmethod
     def save_state(state):
-        with app.State(AppRPC.get_state_path(), lock=True) as s:
+        with app.State(
+            app.resolve_state_path("core_dir", "homestate.json"), lock=True
+        ) as s:
             s.clear()
             s.update(state)
             storage = s.get("storage", {})
             for k in AppRPC.IGNORE_STORAGE_KEYS:
                 if k in storage:
                     del storage[k]
         return True
```

### Comparing `platformio-6.1.7/platformio/home/rpc/handlers/base.py` & `platformio-6.1.8/platformio/home/rpc/handlers/base.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/home/rpc/handlers/ide.py` & `platformio-6.1.8/platformio/home/rpc/handlers/ide.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/home/rpc/handlers/misc.py` & `platformio-6.1.8/platformio/home/rpc/handlers/misc.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/home/rpc/handlers/os.py` & `platformio-6.1.8/platformio/home/rpc/handlers/os.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,34 +15,36 @@
 import glob
 import io
 import os
 import shutil
 from functools import cmp_to_key
 
 import click
-from starlette.concurrency import run_in_threadpool
 
 from platformio import fs
 from platformio.cache import ContentCache
+from platformio.compat import aio_to_thread
 from platformio.device.list.util import list_logical_devices
 from platformio.home.rpc.handlers.base import BaseRPCHandler
 from platformio.http import HTTPSession, ensure_internet_on
 
 
 class HTTPAsyncSession(HTTPSession):
     async def request(  # pylint: disable=signature-differs,invalid-overridden-method
         self, *args, **kwargs
     ):
         func = super().request
-        return await run_in_threadpool(func, *args, **kwargs)
+        return await aio_to_thread(func, *args, **kwargs)
 
 
 class OSRPC(BaseRPCHandler):
-    @staticmethod
-    async def fetch_content(url, data=None, headers=None, cache_valid=None):
+    _http_session = None
+
+    @classmethod
+    async def fetch_content(cls, url, data=None, headers=None, cache_valid=None):
         if not headers:
             headers = {
                 "User-Agent": (
                     "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_12_6) "
                     "AppleWebKit/603.3.8 (KHTML, like Gecko) Version/10.1.2 "
                     "Safari/603.3.8"
                 )
@@ -53,33 +55,35 @@
                 result = cc.get(cache_key)
                 if result is not None:
                     return result
 
         # check internet before and resolve issue with 60 seconds timeout
         ensure_internet_on(raise_exception=True)
 
-        session = HTTPAsyncSession()
+        if not cls._http_session:
+            cls._http_session = HTTPAsyncSession()
+
         if data:
-            r = await session.post(url, data=data, headers=headers)
+            r = await cls._http_session.post(url, data=data, headers=headers)
         else:
-            r = await session.get(url, headers=headers)
+            r = await cls._http_session.get(url, headers=headers)
 
         r.raise_for_status()
         result = r.text
         if cache_valid:
             with ContentCache() as cc:
                 cc.set(cache_key, result, cache_valid)
         return result
 
     async def request_content(self, uri, data=None, headers=None, cache_valid=None):
         if uri.startswith("http"):
             return await self.fetch_content(uri, data, headers, cache_valid)
-        if os.path.isfile(uri):
-            with io.open(uri, encoding="utf-8") as fp:
-                return fp.read()
+        local_path = uri[7:] if uri.startswith("file://") else uri
+        with io.open(local_path, encoding="utf-8") as fp:
+            return fp.read()
         return None
 
     @staticmethod
     def open_url(url):
         return click.launch(url)
 
     @staticmethod
```

### Comparing `platformio-6.1.7/platformio/home/rpc/handlers/piocore.py` & `platformio-6.1.8/platformio/home/rpc/handlers/piocore.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 import json
 import os
 import sys
 import threading
 
 import click
 from ajsonrpc.core import JSONRPC20DispatchException
-from starlette.concurrency import run_in_threadpool
 
 from platformio import __main__, __version__, app, fs, proc, util
 from platformio.compat import (
     IS_WINDOWS,
     aio_create_task,
     aio_get_running_loop,
+    aio_to_thread,
     get_locale_encoding,
     is_bytes,
 )
 from platformio.exception import PlatformioException
 from platformio.home.rpc.handlers.base import BaseRPCHandler
 
 
@@ -173,15 +173,15 @@
         except Exception as exc:  # pylint: disable=bare-except
             raise JSONRPC20DispatchException(
                 code=5000, message="PIO Core Call Error", data=str(exc)
             ) from exc
 
     @staticmethod
     async def _call_subprocess(args, options):
-        result = await run_in_threadpool(
+        result = await aio_to_thread(
             proc.exec_command,
             [get_core_fullpath()] + args,
             cwd=options.get("cwd") or os.getcwd(),
         )
         return (result["out"], result["err"], result["returncode"])
 
     @staticmethod
@@ -193,15 +193,15 @@
                 exit_code = __main__.main(["-c"] + args)
             return (
                 PIOCoreRPC.thread_stdout.get_value_and_reset(),
                 PIOCoreRPC.thread_stderr.get_value_and_reset(),
                 exit_code,
             )
 
-        return await run_in_threadpool(
+        return await aio_to_thread(
             _thread_safe_call, args=args, cwd=options.get("cwd") or os.getcwd()
         )
 
     @staticmethod
     def _process_result(result, to_json=False):
         out, err, code = result
         if out and is_bytes(out):
```

### Comparing `platformio-6.1.7/platformio/home/rpc/handlers/project.py` & `platformio-6.1.8/platformio/home/rpc/handlers/project.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import shutil
 import time
+from pathlib import Path
 
 import semantic_version
 from ajsonrpc.core import JSONRPC20DispatchException
 
 from platformio import app, exception, fs
 from platformio.home.rpc.handlers.app import AppRPC
 from platformio.home.rpc.handlers.base import BaseRPCHandler
@@ -263,45 +264,74 @@
         if ide in ProjectGenerator.get_supported_ides():
             args.extend(["--ide", ide])
         await PIOCoreRPC.call(
             args, options={"cwd": new_project_dir, "force_subprocess": True}
         )
         return new_project_dir
 
-    async def create_empty(self, configuration, options=None):
+    async def init_v2(self, configuration, options=None):
         project_dir = os.path.join(configuration["location"], configuration["name"])
         if not os.path.isdir(project_dir):
             os.makedirs(project_dir)
 
+        envclone = os.environ.copy()
+        envclone["PLATFORMIO_FORCE_ANSI"] = "true"
+        options = options or {}
+        options["spawn"] = {"env": envclone, "cwd": project_dir}
+
+        args = ["project", "init"]
+        ide = app.get_session_var("caller_id")
+        if ide in ProjectGenerator.get_supported_ides():
+            args.extend(["--ide", ide])
+
+        if configuration.get("example"):
+            await self.factory.notify_clients(
+                method=options.get("stdoutNotificationMethod"),
+                params=["Copying example files...\n"],
+                actor="frontend",
+            )
+            await self._pre_init_example(configuration, project_dir)
+        else:
+            args.extend(self._pre_init_empty(configuration))
+
+        return await self.factory.manager.dispatcher["core.exec"](args, options=options)
+
+    @staticmethod
+    def _pre_init_empty(configuration):
         project_options = []
         platform = configuration["platform"]
-        board = configuration.get("board", {}).get("id")
-        env_name = board or platform["name"]
+        board_id = configuration.get("board", {}).get("id")
+        env_name = board_id or platform["name"]
         if configuration.get("description"):
             project_options.append(("description", configuration.get("description")))
         try:
             v = semantic_version.Version(platform.get("version"))
             assert not v.prerelease
             project_options.append(
                 ("platform", "{name} @ ^{version}".format(**platform))
             )
         except (AssertionError, ValueError):
             project_options.append(
                 ("platform", "{name} @ {version}".format(**platform))
             )
-        if board:
-            project_options.append(("board", board))
+        if board_id:
+            project_options.append(("board", board_id))
         if configuration.get("framework"):
             project_options.append(("framework", configuration["framework"]["name"]))
 
-        args = ["project", "init", "-e", env_name, "--sample-code"]
-        ide = app.get_session_var("caller_id")
-        if ide in ProjectGenerator.get_supported_ides():
-            args.extend(["--ide", ide])
+        args = ["-e", env_name, "--sample-code"]
         for name, value in project_options:
             args.extend(["-O", f"{name}={value}"])
+        return args
 
-        envclone = os.environ.copy()
-        envclone["PLATFORMIO_FORCE_ANSI"] = "true"
-        options = options or {}
-        options["spawn"] = {"env": envclone, "cwd": project_dir}
-        return await self.factory.manager.dispatcher["core.exec"](args, options=options)
+    async def _pre_init_example(self, configuration, project_dir):
+        for item in configuration["example"]["files"]:
+            p = Path(project_dir).joinpath(item["path"])
+            if not p.parent.is_dir():
+                p.parent.mkdir(parents=True)
+            p.write_text(
+                await self.factory.manager.dispatcher["os.request_content"](
+                    item["url"]
+                ),
+                encoding="utf-8",
+            )
+        return []
```

### Comparing `platformio-6.1.7/platformio/home/rpc/handlers/registry.py` & `platformio-6.1.8/platformio/home/rpc/handlers/registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from ajsonrpc.core import JSONRPC20DispatchException
-from starlette.concurrency import run_in_threadpool
 
+from platformio.compat import aio_to_thread
 from platformio.home.rpc.handlers.base import BaseRPCHandler
 from platformio.registry.client import RegistryClient
 
 
 class RegistryRPC(BaseRPCHandler):
     @staticmethod
     async def call_client(method, *args, **kwargs):
         try:
             client = RegistryClient()
-            return await run_in_threadpool(getattr(client, method), *args, **kwargs)
+            return await aio_to_thread(getattr(client, method), *args, **kwargs)
         except Exception as exc:  # pylint: disable=bare-except
             raise JSONRPC20DispatchException(
                 code=5000, message="Registry Call Error", data=str(exc)
             ) from exc
```

### Comparing `platformio-6.1.7/platformio/home/rpc/server.py` & `platformio-6.1.8/platformio/home/rpc/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,24 +10,29 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from urllib.parse import parse_qs
 
+import ajsonrpc.utils
 import click
 from ajsonrpc.core import JSONRPC20Error, JSONRPC20Request
 from ajsonrpc.dispatcher import Dispatcher
 from ajsonrpc.manager import AsyncJSONRPCResponseManager, JSONRPC20Response
 from starlette.endpoints import WebSocketEndpoint
 
 from platformio.compat import aio_create_task, aio_get_running_loop
 from platformio.http import InternetConnectionError
 from platformio.proc import force_exit
 
+# Remove this line when PR is merged
+# https://github.com/pavlov99/ajsonrpc/pull/22
+ajsonrpc.utils.is_invalid_params = lambda: False
+
 
 class JSONRPCServerFactoryBase:
     connection_nums = 0
     shutdown_timer = None
 
     def __init__(self, shutdown_timeout=0):
         self.shutdown_timeout = shutdown_timeout
```

### Comparing `platformio-6.1.7/platformio/home/run.py` & `platformio-6.1.8/platformio/home/run.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/http.py` & `platformio-6.1.8/platformio/http.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 
 import json
 import os
 import socket
 from urllib.parse import urljoin
 
 import requests.adapters
-from requests.packages.urllib3.util.retry import Retry  # pylint:disable=import-error
+from urllib3.util.retry import Retry
 
 from platformio import __check_internet_hosts__, app, util
 from platformio.cache import ContentCache, cleanup_content_cache
 from platformio.exception import PlatformioException, UserSideException
 
 __default_requests_timeout__ = (10, None)  # (connect, read)
 
 
-class HTTPClientError(PlatformioException):
+class HTTPClientError(UserSideException):
     def __init__(self, message, response=None):
         super().__init__()
         self.message = message
         self.response = response
 
     def __str__(self):  # pragma: no cover
         return self.message
@@ -46,15 +46,18 @@
 
 
 class HTTPSession(requests.Session):
     def __init__(self, *args, **kwargs):
         self._x_base_url = kwargs.pop("x_base_url") if "x_base_url" in kwargs else None
         super().__init__(*args, **kwargs)
         self.headers.update({"User-Agent": app.get_user_agent()})
-        self.verify = app.get_setting("enable_proxy_strict_ssl")
+        try:
+            self.verify = app.get_setting("enable_proxy_strict_ssl")
+        except PlatformioException:
+            self.verify = True
 
     def request(  # pylint: disable=signature-differs,arguments-differ
         self, method, url, *args, **kwargs
     ):
         # print("HTTPSession::request", self._x_base_url, method, url, args, kwargs)
         if "timeout" not in kwargs:
             kwargs["timeout"] = __default_requests_timeout__
@@ -150,15 +153,18 @@
             return self._parse_json_response(self.send_request(method, path, **kwargs))
         cache_key = ContentCache.key_from_args(
             method, path, kwargs.get("params"), kwargs.get("data")
         )
         with ContentCache("http") as cc:
             result = cc.get(cache_key)
             if result is not None:
-                return json.loads(result)
+                try:
+                    return json.loads(result)
+                except json.JSONDecodeError:
+                    pass
             response = self.send_request(method, path, **kwargs)
             data = self._parse_json_response(response)
             cc.set(cache_key, response.text, cache_valid)
             return data
 
     @staticmethod
     def _parse_json_response(response, expected_codes=(200, 201, 202)):
```

### Comparing `platformio-6.1.7/platformio/maintenance.py` & `platformio-6.1.8/platformio/maintenance.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,31 +21,28 @@
 
 from platformio import __version__, app, exception, fs, telemetry
 from platformio.cache import cleanup_content_cache
 from platformio.cli import PlatformioCLI
 from platformio.commands.upgrade import get_latest_version
 from platformio.http import HTTPClientError, InternetConnectionError, ensure_internet_on
 from platformio.package.manager.core import update_core_packages
-from platformio.package.manager.tool import ToolPackageManager
-from platformio.package.meta import PackageSpec
 from platformio.package.version import pepver_to_semver
 from platformio.system.prune import calculate_unnecessary_system_data
 
 
-def on_platformio_start(ctx, caller):
+def on_cmd_start(ctx, caller):
     app.set_session_var("command_ctx", ctx)
     set_caller(caller)
-    telemetry.on_command()
-
+    telemetry.on_cmd_start(ctx)
     if PlatformioCLI.in_silence():
         return
     after_upgrade(ctx)
 
 
-def on_platformio_end(ctx, result):  # pylint: disable=unused-argument
+def on_cmd_end():
     if PlatformioCLI.in_silence():
         return
 
     try:
         check_platformio_upgrade()
         check_prune_system()
     except (
@@ -56,16 +53,20 @@
         click.secho(
             "Failed to check for PlatformIO upgrades. "
             "Please check your Internet connection.",
             fg="red",
         )
 
 
-def on_platformio_exception(e):
-    telemetry.on_exception(e)
+def on_platformio_exception(exc):
+    telemetry.log_exception(exc)
+
+
+def on_platformio_exit():
+    telemetry.on_exit()
 
 
 def set_caller(caller=None):
     caller = caller or os.getenv("PLATFORMIO_CALLER")
     if not caller:
         if os.getenv("CODESPACES"):
             caller = "codespaces"
@@ -75,19 +76,18 @@
             caller = "gitpod"
     if caller:
         app.set_session_var("caller_id", caller)
 
 
 class Upgrader:
     def __init__(self, from_version, to_version):
-        self.from_version = pepver_to_semver(from_version)
-        self.to_version = pepver_to_semver(to_version)
-
+        self.from_version = from_version
+        self.to_version = to_version
         self._upgraders = [
-            (semantic_version.Version("4.4.0-a.8"), self._update_pkg_metadata),
+            (semantic_version.Version("6.1.8-a.1"), self._appstate_migration),
         ]
 
     def run(self, ctx):
         if self.from_version > self.to_version:
             return True
 
         result = [True]
@@ -95,91 +95,104 @@
             if self.from_version >= version or self.to_version < version:
                 continue
             result.append(callback(ctx))
 
         return all(result)
 
     @staticmethod
-    def _update_pkg_metadata(_):
-        pm = ToolPackageManager()
-        for pkg in pm.get_installed():
-            if not pkg.metadata or pkg.metadata.spec.external or pkg.metadata.spec.id:
-                continue
-            result = pm.search_registry_packages(PackageSpec(name=pkg.metadata.name))
-            if len(result) != 1:
-                continue
-            result = result[0]
-            pkg.metadata.spec = PackageSpec(
-                id=result["id"],
-                owner=result["owner"]["username"],
-                name=result["name"],
+    def _appstate_migration(_):
+        state_path = app.resolve_state_path("core_dir", "appstate.json")
+        if not os.path.isfile(state_path):
+            return True
+        app.delete_state_item("telemetry")
+        created_at = app.get_state_item("created_at", None)
+        if not created_at:
+            state_stat = os.stat(state_path)
+            app.set_state_item(
+                "created_at",
+                int(
+                    state_stat.st_birthtime
+                    if hasattr(state_stat, "st_birthtime")
+                    else state_stat.st_ctime
+                ),
             )
-            pkg.dump_meta()
         return True
 
 
 def after_upgrade(ctx):
     terminal_width = shutil.get_terminal_size().columns
-    last_version = app.get_state_item("last_version", "0.0.0")
-    if last_version == __version__:
-        return
+    last_version_str = app.get_state_item("last_version", "0.0.0")
+    if last_version_str == __version__:
+        return None
 
-    if last_version == "0.0.0":
+    if last_version_str == "0.0.0":
         app.set_state_item("last_version", __version__)
-    elif pepver_to_semver(last_version) > pepver_to_semver(__version__):
+        return print_welcome_banner()
+
+    last_version = pepver_to_semver(last_version_str)
+    current_version = pepver_to_semver(__version__)
+
+    if last_version > current_version and not last_version.prerelease:
         click.secho("*" * terminal_width, fg="yellow")
         click.secho(
             "Obsolete PIO Core v%s is used (previous was %s)"
-            % (__version__, last_version),
+            % (__version__, last_version_str),
             fg="yellow",
         )
         click.secho("Please remove multiple PIO Cores from a system:", fg="yellow")
         click.secho(
             "https://docs.platformio.org/en/latest/core"
             "/installation/troubleshooting.html",
             fg="cyan",
         )
         click.secho("*" * terminal_width, fg="yellow")
-        return
-    else:
-        click.secho("Please wait while upgrading PlatformIO...", fg="yellow")
+        return None
 
-        # Update PlatformIO's Core packages
-        cleanup_content_cache("http")
-        update_core_packages()
-
-        u = Upgrader(last_version, __version__)
-        if u.run(ctx):
-            app.set_state_item("last_version", __version__)
-            click.secho(
-                "PlatformIO has been successfully upgraded to %s!\n" % __version__,
-                fg="green",
-            )
-            telemetry.send_event(
-                category="Auto",
-                action="Upgrade",
-                label="%s > %s" % (last_version, __version__),
-            )
+    click.secho("Please wait while upgrading PlatformIO...", fg="yellow")
+
+    # Update PlatformIO's Core packages
+    cleanup_content_cache("http")
+    update_core_packages()
 
-    # PlatformIO banner
+    u = Upgrader(last_version, current_version)
+    if u.run(ctx):
+        app.set_state_item("last_version", __version__)
+        click.secho(
+            "PlatformIO has been successfully upgraded to %s!\n" % __version__,
+            fg="green",
+        )
+        telemetry.log_event(
+            "pio_upgrade_core",
+            {
+                "label": "%s > %s" % (last_version_str, __version__),
+                "from_version": last_version_str,
+                "to_version": __version__,
+            },
+        )
+
+    return print_welcome_banner()
+
+
+def print_welcome_banner():
+    terminal_width = shutil.get_terminal_size().columns
     click.echo("*" * terminal_width)
     click.echo("If you like %s, please:" % (click.style("PlatformIO", fg="cyan")))
     click.echo(
-        "- %s us on Twitter to stay up-to-date "
-        "on the latest project news > %s"
+        "- %s it on GitHub > %s"
         % (
-            click.style("follow", fg="cyan"),
-            click.style("https://twitter.com/PlatformIO_Org", fg="cyan"),
+            click.style("star", fg="cyan"),
+            click.style("https://github.com/platformio/platformio-core", fg="cyan"),
         )
     )
     click.echo(
-        "- %s it on GitHub > %s"
+        "- %s us on LinkedIn to stay up-to-date "
+        "on the latest project news > %s"
         % (
-            click.style("star", fg="cyan"),
-            click.style("https://github.com/platformio/platformio", fg="cyan"),
+            click.style("follow", fg="cyan"),
+            click.style("https://www.linkedin.com/company/platformio/", fg="cyan"),
         )
     )
     if not os.getenv("PLATFORMIO_IDE"):
         click.echo(
             "- %s PlatformIO IDE for embedded development > %s"
             % (
                 click.style("try", fg="cyan"),
@@ -224,15 +237,15 @@
     )
     if os.path.join("Cellar", "platformio") in fs.get_source_dir():
         click.secho("brew update && brew upgrade", fg="cyan", nl=False)
         click.secho("` command.", fg="yellow")
     else:
         click.secho("platformio upgrade", fg="cyan", nl=False)
         click.secho("` or `", fg="yellow", nl=False)
-        click.secho("pip install -U platformio", fg="cyan", nl=False)
+        click.secho("python -m pip install -U platformio", fg="cyan", nl=False)
         click.secho("` command.", fg="yellow")
     click.secho("Changes: ", fg="yellow", nl=False)
     click.secho("https://docs.platformio.org/en/latest/history.html", fg="cyan")
     click.echo("*" * terminal_width)
     click.echo("")
```

### Comparing `platformio-6.1.7/platformio/package/__init__.py` & `platformio-6.1.8/platformio/package/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/package/cli.py` & `platformio-6.1.8/platformio/package/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/package/commands/__init__.py` & `platformio-6.1.8/platformio/package/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/package/commands/exec.py` & `platformio-6.1.8/platformio/package/commands/exec.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/package/commands/install.py` & `platformio-6.1.8/platformio/package/commands/install.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/package/commands/list.py` & `platformio-6.1.8/platformio/package/commands/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,16 @@
         list_project_packages(options)
 
 
 def humanize_package(pkg, spec=None, verbose=False):
     if spec and not isinstance(spec, PackageSpec):
         spec = PackageSpec(spec)
     data = [
-        click.style("{name} @ {version}".format(**pkg.metadata.as_dict()), fg="cyan")
+        click.style(pkg.metadata.name, fg="cyan"),
+        click.style(f"@ {str(pkg.metadata.version)}", bold=True),
     ]
     extra_data = ["required: %s" % (spec.humanize() if spec else "Any")]
     if verbose:
         extra_data.append(pkg.path)
     data.append("(%s)" % ", ".join(extra_data))
     return " ".join(data)
 
@@ -131,41 +132,41 @@
 def list_global_packages(options):
     data = [
         ("platforms", PlatformPackageManager(options.get("storage_dir"))),
         ("tools", ToolPackageManager(options.get("storage_dir"))),
         ("libraries", LibraryPackageManager(options.get("storage_dir"))),
     ]
     only_packages = any(
-        options.get(type_) or options.get(f"only_{type_}") for (type_, _) in data
+        options.get(typex) or options.get(f"only_{typex}") for (typex, _) in data
     )
-    for type_, pm in data:
+    for typex, pm in data:
         skip_conds = [
             only_packages
-            and not options.get(type_)
-            and not options.get(f"only_{type_}"),
+            and not options.get(typex)
+            and not options.get(f"only_{typex}"),
             not pm.get_installed(),
         ]
         if any(skip_conds):
             continue
-        click.secho(type_.capitalize(), bold=True)
+        click.secho(typex.capitalize(), bold=True)
         print_dependency_tree(
-            pm, filter_specs=options.get(type_), verbose=options.get("verbose")
+            pm, filter_specs=options.get(typex), verbose=options.get("verbose")
         )
         click.echo()
 
 
 def list_project_packages(options):
     environments = options["environments"]
     only_packages = any(
-        options.get(type_) or options.get(f"only_{type_}")
-        for type_ in ("platforms", "tools", "libraries")
+        options.get(typex) or options.get(f"only_{typex}")
+        for typex in ("platforms", "tools", "libraries")
     )
     only_platform_packages = any(
-        options.get(type_) or options.get(f"only_{type_}")
-        for type_ in ("platforms", "tools")
+        options.get(typex) or options.get(f"only_{typex}")
+        for typex in ("platforms", "tools")
     )
     only_library_packages = options.get("libraries") or options.get("only_libraries")
 
     with fs.cd(options["project_dir"]):
         config = ProjectConfig.get_instance()
         config.validate(environments)
         for env in config.envs():
```

### Comparing `platformio-6.1.7/platformio/package/commands/outdated.py` & `platformio-6.1.8/platformio/package/commands/outdated.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/package/commands/pack.py` & `platformio-6.1.8/platformio/package/commands/pack.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/package/commands/publish.py` & `platformio-6.1.8/platformio/package/commands/publish.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 @click.option(
     "--owner",
     help="PIO Account username (can be organization username). "
     "Default is set to a username of the authorized PIO Account",
 )
 @click.option(
     "--type",
-    "type_",
+    "typex",
     type=click.Choice(list(PackageType.items().values())),
     help="Custom package type",
 )
 @click.option(
     "--released-at",
     callback=validate_datetime,
     help="Custom release date and time in the next format (UTC): 2014-06-13 17:08:52",
@@ -79,15 +79,15 @@
 @click.option(
     "--non-interactive",
     is_flag=True,
     help="Do not show interactive prompt",
     hidden=True,
 )
 def package_publish_cmd(  # pylint: disable=too-many-arguments, too-many-locals
-    package, owner, type_, released_at, private, notify, no_interactive, non_interactive
+    package, owner, typex, released_at, private, notify, no_interactive, non_interactive
 ):
     click.secho("Preparing a package...", fg="cyan")
     no_interactive = no_interactive or non_interactive
     owner = owner or AccountClient().get_logged_username()
     do_not_pack = (
         not os.path.isdir(package)
         and isinstance(FileUnpacker.new_archiver(package), TARArchiver)
@@ -99,42 +99,42 @@
         if do_not_pack:
             archive_path = package
         else:
             with fs.cd(tmp_dir):
                 p = PackagePacker(package)
                 archive_path = p.pack()
 
-        type_ = type_ or PackageType.from_archive(archive_path)
+        typex = typex or PackageType.from_archive(archive_path)
         manifest = ManifestSchema().load_manifest(
             ManifestParserFactory.new_from_archive(archive_path).as_dict()
         )
         name = manifest.get("name")
         version = manifest.get("version")
         data = [
-            ("Type:", type_),
+            ("Type:", typex),
             ("Owner:", owner),
             ("Name:", name),
             ("Version:", version),
             ("Size:", fs.humanize_file_size(os.path.getsize(archive_path))),
         ]
         if manifest.get("system"):
             data.insert(len(data) - 1, ("System:", ", ".join(manifest.get("system"))))
         click.echo(tabulate(data, tablefmt="plain"))
 
         # check files containing non-ascii chars
         check_archive_file_names(archive_path)
 
         # look for duplicates
-        check_package_duplicates(owner, type_, name, version, manifest.get("system"))
+        check_package_duplicates(owner, typex, name, version, manifest.get("system"))
 
         if not no_interactive:
             click.confirm(
                 "Are you sure you want to publish the %s %s to the registry?\n"
                 % (
-                    type_,
+                    typex,
                     click.style(
                         "%s/%s@%s" % (owner, name, version),
                         fg="cyan",
                     ),
                 ),
                 abort=True,
             )
@@ -142,15 +142,15 @@
         click.secho(
             "The package publishing may take some time depending "
             "on your Internet connection and the package size.",
             fg="yellow",
         )
         click.echo("Publishing...")
         response = RegistryClient().publish_package(
-            owner, type_, archive_path, released_at, private, notify
+            owner, typex, archive_path, released_at, private, notify
         )
         if not do_not_pack:
             os.remove(archive_path)
         click.secho(response.get("message"), fg="green")
 
 
 def check_archive_file_names(archive_path):
```

### Comparing `platformio-6.1.7/platformio/package/commands/search.py` & `platformio-6.1.8/platformio/package/commands/search.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/package/commands/show.py` & `platformio-6.1.8/platformio/package/commands/show.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/package/commands/uninstall.py` & `platformio-6.1.8/platformio/package/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/package/commands/unpublish.py` & `platformio-6.1.8/platformio/package/commands/unpublish.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/package/commands/update.py` & `platformio-6.1.8/platformio/package/commands/update.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/package/download.py` & `platformio-6.1.8/platformio/package/download.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/package/exception.py` & `platformio-6.1.8/platformio/package/exception.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from platformio import util
-from platformio.exception import PlatformioException, UserSideException
+from platformio.exception import UserSideException
 
 
-class PackageException(PlatformioException):
+class PackageException(UserSideException):
     pass
 
 
 class ManifestException(PackageException):
     pass
 
 
@@ -47,22 +47,22 @@
         )
 
 
 class MissingPackageManifestError(ManifestException):
     MESSAGE = "Could not find one of '{0}' manifest files in the package"
 
 
-class UnknownPackageError(UserSideException):
+class UnknownPackageError(PackageException):
     MESSAGE = (
         "Could not find the package with '{0}' requirements for your system '%s'"
         % util.get_systype()
     )
 
 
-class NotGlobalLibDir(UserSideException):
+class NotGlobalLibDir(PackageException):
     MESSAGE = (
         "The `{0}` is not a PlatformIO project.\n\n"
         "To manage libraries in global storage `{1}`,\n"
         "please use `platformio lib --global {2}` or specify custom storage "
         "`platformio lib --storage-dir /path/to/storage/ {2}`.\n"
         "Check `platformio lib --help` for details."
     )
```

### Comparing `platformio-6.1.7/platformio/package/lockfile.py` & `platformio-6.1.8/platformio/package/lockfile.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 from time import sleep, time
 
-from platformio.exception import PlatformioException
+from platformio.exception import UserSideException
 
 LOCKFILE_TIMEOUT = 3600  # in seconds, 1 hour
 LOCKFILE_DELAY = 0.2
 
 LOCKFILE_INTERFACE_FCNTL = 1
 LOCKFILE_INTERFACE_MSVCRT = 2
 
@@ -32,19 +32,19 @@
         import msvcrt
 
         LOCKFILE_CURRENT_INTERFACE = LOCKFILE_INTERFACE_MSVCRT
     except ImportError:
         LOCKFILE_CURRENT_INTERFACE = None
 
 
-class LockFileExists(PlatformioException):
+class LockFileExists(UserSideException):
     pass
 
 
-class LockFileTimeoutError(PlatformioException):
+class LockFileTimeoutError(UserSideException):
     pass
 
 
 class LockFile:
     def __init__(self, path, timeout=LOCKFILE_TIMEOUT, delay=LOCKFILE_DELAY):
         self.timeout = timeout
         self.delay = delay
```

### Comparing `platformio-6.1.7/platformio/package/manager/__init__.py` & `platformio-6.1.8/platformio/package/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/package/manager/_download.py` & `platformio-6.1.8/platformio/package/manager/_download.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/package/manager/_install.py` & `platformio-6.1.8/platformio/package/manager/_install.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/package/manager/_legacy.py` & `platformio-6.1.8/platformio/package/manager/_legacy.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/package/manager/_registry.py` & `platformio-6.1.8/platformio/package/manager/_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,20 +21,21 @@
 from platformio.package.version import cast_version_to_semver
 from platformio.registry.client import RegistryClient
 from platformio.registry.mirror import RegistryFileMirrorIterator
 
 
 class PackageManagerRegistryMixin:
     def install_from_registry(self, spec, search_qualifiers=None):
+        package = version = None
         if spec.owner and spec.name and not search_qualifiers:
             package = self.fetch_registry_package(spec)
             if not package:
                 raise UnknownPackageError(spec.humanize())
             version = self.pick_best_registry_version(package["versions"], spec)
-        else:
+        elif spec.id or spec.name:
             packages = self.search_registry_packages(spec, search_qualifiers)
             if not packages:
                 raise UnknownPackageError(spec.humanize())
             if len(packages) > 1:
                 self.print_multi_package_issue(self.log.warning, packages, spec)
             package, version = self.find_best_registry_version(packages, spec)
```

### Comparing `platformio-6.1.7/platformio/package/manager/_symlink.py` & `platformio-6.1.8/platformio/package/manager/_symlink.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/package/manager/_uninstall.py` & `platformio-6.1.8/platformio/package/manager/_uninstall.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/package/manager/_update.py` & `platformio-6.1.8/platformio/package/manager/_update.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/package/manager/base.py` & `platformio-6.1.8/platformio/package/manager/base.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/package/manager/core.py` & `platformio-6.1.8/platformio/package/manager/core.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/package/manager/library.py` & `platformio-6.1.8/platformio/package/manager/library.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/package/manager/platform.py` & `platformio-6.1.8/platformio/package/manager/platform.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/package/manager/tool.py` & `platformio-6.1.8/platformio/package/manager/tool.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/package/manifest/__init__.py` & `platformio-6.1.8/platformio/package/manifest/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/package/manifest/parser.py` & `platformio-6.1.8/platformio/package/manifest/parser.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/package/manifest/schema.py` & `platformio-6.1.8/platformio/package/manifest/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,15 +179,15 @@
     downloadUrl = fields.Url(validate=validate.Length(min=1, max=255))
 
     keywords = StrictListField(
         fields.Str(
             validate=[
                 validate.Length(min=1, max=50),
                 validate.Regexp(
-                    r"^[a-z\d\-\+\. ]+$", error="Only [a-z0-9-+. ] chars are allowed"
+                    r"^[a-z\d\-_\+\. ]+$", error="Only [a-z0-9+_-. ] chars are allowed"
                 ),
             ]
         )
     )
     platforms = StrictListField(
         fields.Str(
             validate=[
@@ -272,13 +272,13 @@
             "Invalid SPDX license identifier. See valid identifiers at "
             "https://spdx.org/licenses/"
         )
 
     @staticmethod
     @memoized(expire="1h")
     def load_spdx_licenses():
-        version = "3.20"
+        version = "3.21"
         spdx_data_url = (
             "https://raw.githubusercontent.com/spdx/license-list-data/"
-            "v%s/json/licenses.json" % version
+            f"v{version}/json/licenses.json"
         )
         return json.loads(fetch_remote_content(spdx_data_url))
```

### Comparing `platformio-6.1.7/platformio/package/meta.py` & `platformio-6.1.8/platformio/package/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from urllib.parse import urlparse
 
 import semantic_version
 
 from platformio import fs
 from platformio.compat import get_object_members, hashlib_encode_data, string_types
 from platformio.package.manifest.parser import ManifestFileType
-from platformio.package.version import cast_version_to_semver
+from platformio.package.version import SemanticVersionError, cast_version_to_semver
 from platformio.util import items_in_list
 
 
 class PackageType:
     LIBRARY = "library"
     PLATFORM = "platform"
     TOOL = "tool"
@@ -171,15 +171,15 @@
         self.id = id
         self.name = name
         self.uri = uri
         self.raw = raw
         if requirements:
             try:
                 self.requirements = requirements
-            except ValueError as exc:
+            except SemanticVersionError as exc:
                 if not self.name or self.uri or self.raw:
                     raise exc
                 self.raw = "%s=%s" % (self.name, requirements)
         self._name_is_custom = False
         self._parse(self.raw)
 
     def __eq__(self, other):
@@ -220,19 +220,22 @@
         return self._requirements
 
     @requirements.setter
     def requirements(self, value):
         if not value:
             self._requirements = None
             return
-        self._requirements = (
-            value
-            if isinstance(value, semantic_version.SimpleSpec)
-            else semantic_version.SimpleSpec(str(value))
-        )
+        try:
+            self._requirements = (
+                value
+                if isinstance(value, semantic_version.SimpleSpec)
+                else semantic_version.SimpleSpec(str(value))
+            )
+        except ValueError as exc:
+            raise SemanticVersionError(exc) from exc
 
     def humanize(self):
         result = ""
         if self.uri:
             result = self.uri
         elif self.name:
             if self.owner:
```

### Comparing `platformio-6.1.7/platformio/package/pack.py` & `platformio-6.1.8/platformio/package/pack.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/package/unpack.py` & `platformio-6.1.8/platformio/package/unpack.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/package/vcsclient.py` & `platformio-6.1.8/platformio/package/vcsclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,22 +14,18 @@
 
 import os
 import re
 import subprocess
 from urllib.parse import urlparse
 
 from platformio import proc
-from platformio.package.exception import (
-    PackageException,
-    PlatformioException,
-    UserSideException,
-)
+from platformio.exception import UserSideException
 
 
-class VCSBaseException(PackageException):
+class VCSBaseException(UserSideException):
     pass
 
 
 class VCSClientFactory:
     @staticmethod
     def new(src_dir, remote_url, silent=False):
         result = urlparse(remote_url)
@@ -70,16 +66,16 @@
     def check_client(self):
         try:
             assert self.command
             if self.silent:
                 self.get_cmd_output(["--version"])
             else:
                 assert self.run_cmd(["--version"])
-        except (AssertionError, OSError, PlatformioException) as exc:
-            raise UserSideException(
+        except (AssertionError, OSError) as exc:
+            raise VCSBaseException(
                 "VCS: `%s` client is not installed in your system" % self.command
             ) from exc
         return True
 
     @property
     def storage_dir(self):
         return os.path.join(self.src_dir, "." + self.command)
```

### Comparing `platformio-6.1.7/platformio/package/version.py` & `platformio-6.1.8/platformio/package/version.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,28 +12,34 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import re
 
 import semantic_version
 
+from platformio.exception import UserSideException
+
+
+class SemanticVersionError(UserSideException):
+    pass
+
 
 def cast_version_to_semver(value, force=True, raise_exception=False):
     assert value
     try:
         return semantic_version.Version(value)
     except ValueError:
         pass
     if force:
         try:
             return semantic_version.Version.coerce(value)
         except ValueError:
             pass
     if raise_exception:
-        raise ValueError("Invalid SemVer version %s" % value)
+        raise SemanticVersionError("Invalid SemVer version %s" % value)
     # parse commit hash
     if re.match(r"^[\da-f]+$", value, flags=re.I):
         return semantic_version.Version("0.0.0+sha." + value)
     return semantic_version.Version("0.0.0+" + value)
 
 
 def pepver_to_semver(pepver):
```

### Comparing `platformio-6.1.7/platformio/platform/__init__.py` & `platformio-6.1.8/platformio/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/platform/_packages.py` & `platformio-6.1.8/platformio/platform/_packages.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/platform/_run.py` & `platformio-6.1.8/platformio/platform/_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,40 +48,32 @@
         self, variables, targets, silent, verbose, jobs
     ):
         assert isinstance(variables, dict)
         assert isinstance(targets, list)
 
         self.ensure_engine_compatible()
         self.configure_project_packages(variables["pioenv"], targets)
-        self._report_non_sensitive_data(variables["pioenv"], targets)
 
         self.silent = silent
         self.verbose = verbose or app.get_setting("force_verbose")
 
         variables["platform_manifest"] = self.manifest_path
 
         if "build_script" not in variables:
             variables["build_script"] = self.get_build_script()
         if not os.path.isfile(variables["build_script"]):
             raise BuildScriptNotFound(variables["build_script"])
 
+        telemetry.log_platform_run(self, self.config, variables["pioenv"], targets)
         result = self._run_scons(variables, targets, jobs)
+
         assert "returncode" in result
 
         return result
 
-    def _report_non_sensitive_data(self, env, targets):
-        options = self.config.items(env=env, as_dict=True)
-        options["platform_packages"] = [
-            dict(name=item["name"], version=item["version"])
-            for item in self.dump_used_packages()
-        ]
-        options["platform"] = {"name": self.name, "version": self.version}
-        telemetry.send_run_environment(options, targets)
-
     def _run_scons(self, variables, targets, jobs):
         scons_dir = get_core_package_dir("tool-scons")
         args = [
             proc.get_pythonexe_path(),
             os.path.join(scons_dir, "scons.py"),
             "-Q",
             "--warn=no-no-parallel-support",
```

### Comparing `platformio-6.1.7/platformio/platform/base.py` & `platformio-6.1.8/platformio/platform/base.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/platform/board.py` & `platformio-6.1.8/platformio/platform/board.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,29 +10,29 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 
-from platformio import fs, telemetry, util
+from platformio import fs, util
 from platformio.compat import MISSING
 from platformio.debug.exception import DebugInvalidOptionsError, DebugSupportError
-from platformio.exception import UserSideException
+from platformio.exception import InvalidJSONFile, UserSideException
 from platformio.platform.exception import InvalidBoardManifest
 
 
 class PlatformBoardConfig:
     def __init__(self, manifest_path):
         self._id = os.path.basename(manifest_path)[:-5]
         assert os.path.isfile(manifest_path)
         self.manifest_path = manifest_path
         try:
             self._manifest = fs.load_json(manifest_path)
-        except ValueError as exc:
+        except InvalidJSONFile as exc:
             raise InvalidBoardManifest(manifest_path) from exc
         if not set(["name", "url", "vendor"]) <= set(self._manifest):
             raise UserSideException(
                 "Please specify name, url and vendor fields for " + manifest_path
             )
 
     def get(self, path, default=MISSING):
@@ -115,15 +115,14 @@
 
     def get_debug_tool_name(self, custom=None):
         debug_tools = self._manifest.get("debug", {}).get("tools")
         tool_name = custom
         if tool_name == "custom":
             return tool_name
         if not debug_tools:
-            telemetry.send_event("Debug", "Request", self.id)
             raise DebugSupportError(self._manifest["name"])
         if tool_name:
             if tool_name in debug_tools:
                 return tool_name
             raise DebugInvalidOptionsError(
                 "Unknown debug tool `%s`. Please use one of `%s` or `custom`"
                 % (tool_name, ", ".join(sorted(list(debug_tools))))
```

### Comparing `platformio-6.1.7/platformio/platform/exception.py` & `platformio-6.1.8/platformio/platform/exception.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from platformio.exception import PlatformioException
+from platformio.exception import UserSideException
 
 
-class PlatformException(PlatformioException):
+class PlatformException(UserSideException):
     pass
 
 
 class UnknownPlatform(PlatformException):
     MESSAGE = "Unknown development platform '{0}'"
```

### Comparing `platformio-6.1.7/platformio/platform/factory.py` & `platformio-6.1.8/platformio/platform/factory.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/proc.py` & `platformio-6.1.8/platformio/proc.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/project/__init__.py` & `platformio-6.1.8/platformio/project/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/project/cli.py` & `platformio-6.1.8/platformio/project/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/project/commands/__init__.py` & `platformio-6.1.8/platformio/project/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/project/commands/config.py` & `platformio-6.1.8/platformio/project/commands/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,24 +26,31 @@
 @click.command("config", short_help="Show computed configuration")
 @click.option(
     "-d",
     "--project-dir",
     default=os.getcwd,
     type=click.Path(exists=True, file_okay=False, dir_okay=True),
 )
+@click.option("--lint", is_flag=True)
 @click.option("--json-output", is_flag=True)
-def project_config_cmd(project_dir, json_output):
+def project_config_cmd(project_dir, lint, json_output):
     if not is_platformio_project(project_dir):
         raise NotPlatformIOProjectError(project_dir)
     with fs.cd(project_dir):
-        config = ProjectConfig.get_instance()
+        if lint:
+            return lint_configuration(json_output)
+        return print_configuration(json_output)
+
+
+def print_configuration(json_output=False):
+    config = ProjectConfig.get_instance()
     if json_output:
         return click.echo(config.to_json())
     click.echo(
-        "Computed project configuration for %s" % click.style(project_dir, fg="cyan")
+        "Computed project configuration for %s" % click.style(os.getcwd(), fg="cyan")
     )
     for section, options in config.as_tuple():
         click.secho(section, fg="cyan")
         click.echo("-" * len(section))
         click.echo(
             tabulate(
                 [
@@ -51,7 +58,47 @@
                     for name, value in options
                 ],
                 tablefmt="plain",
             )
         )
         click.echo()
     return None
+
+
+def lint_configuration(json_output=False):
+    result = ProjectConfig.lint()
+    errors = result["errors"]
+    warnings = result["warnings"]
+    if json_output:
+        return click.echo(result)
+    if not errors and not warnings:
+        return click.secho(
+            'The "platformio.ini" configuration file is free from linting errors.',
+            fg="green",
+        )
+    if errors:
+        click.echo(
+            tabulate(
+                [
+                    (
+                        click.style(error["type"], fg="red"),
+                        error["message"],
+                        error.get("source", "") + (f":{error.get('lineno')}")
+                        if "lineno" in error
+                        else "",
+                    )
+                    for error in errors
+                ],
+                tablefmt="plain",
+            )
+        )
+    if warnings:
+        click.echo(
+            tabulate(
+                [
+                    (click.style("Warning", fg="yellow"), warning)
+                    for warning in warnings
+                ],
+                tablefmt="plain",
+            )
+        )
+    return None
```

### Comparing `platformio-6.1.7/platformio/project/commands/init.py` & `platformio-6.1.8/platformio/project/commands/init.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/project/commands/metadata.py` & `platformio-6.1.8/platformio/project/commands/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     default=os.getcwd,
     type=click.Path(exists=True, file_okay=False, dir_okay=True),
 )
 @click.option("-e", "--environment", "environments", multiple=True)
 @click.option("--json-output", is_flag=True)
 @click.option("--json-output-path", type=click.Path())
 def project_metadata_cmd(project_dir, environments, json_output, json_output_path):
+    project_dir = os.path.abspath(project_dir)
     with fs.cd(project_dir):
         config = ProjectConfig.get_instance()
         config.validate(environments)
         environments = list(environments or config.envs())
         build_metadata = load_build_metadata(project_dir, environments)
 
     if not json_output:
```

### Comparing `platformio-6.1.7/platformio/project/config.py` & `platformio-6.1.8/platformio/project/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,39 +82,39 @@
         self.expand_interpolations = expand_interpolations
         self.warnings = []
         self._parsed = []
         self._parser = configparser.ConfigParser(inline_comment_prefixes=("#", ";"))
         if path and os.path.isfile(path):
             self.read(path, parse_extra)
 
-        self._maintain_renaimed_options()
+        self._maintain_renamed_options()
 
     def __getattr__(self, name):
         return getattr(self._parser, name)
 
     def read(self, path, parse_extra=True):
         if path in self._parsed:
             return
         self._parsed.append(path)
         try:
             self._parser.read(path, "utf-8")
         except configparser.Error as exc:
-            raise exception.InvalidProjectConfError(path, str(exc))
+            raise exception.InvalidProjectConfError(path, str(exc)) from exc
 
         if not parse_extra:
             return
 
         # load extra configs
         for pattern in self.get("platformio", "extra_configs", []):
             if pattern.startswith("~"):
                 pattern = fs.expanduser(pattern)
             for item in glob.glob(pattern, recursive=True):
                 self.read(item)
 
-    def _maintain_renaimed_options(self):
+    def _maintain_renamed_options(self):
         renamed_options = {}
         for option in ProjectOptions.values():
             if option.oldnames:
                 renamed_options.update({name: option.name for name in option.oldnames})
 
         for section in self._parser.sections():
             scope = self.get_section_scope(section)
@@ -320,23 +320,27 @@
             section = parent_section
             if option == "__env__":
                 if not parent_section.startswith("env:"):
                     raise exception.ProjectOptionValueError(
                         f"`${{this.__env__}}` is called from the `{parent_section}` "
                         "section that is not valid PlatformIO environment, see",
                         option,
+                        " ",
                         section,
                     )
                 return parent_section[4:]
         # handle nested calls
         try:
             value = self.get(section, option)
         except RecursionError as exc:
             raise exception.ProjectOptionValueError(
-                "Infinite recursion has been detected", option, section
+                "Infinite recursion has been detected",
+                option,
+                " ",
+                section,
             ) from exc
         if isinstance(value, list):
             return "\n".join(value)
         return str(value)
 
     def get(self, section, option, default=MISSING):
         value = None
@@ -355,15 +359,18 @@
             value = self.parse_multi_values(value or [])
         try:
             return self.cast_to(value, option_meta.type)
         except click.BadParameter as exc:
             if not self.expand_interpolations:
                 return value
             raise exception.ProjectOptionValueError(
-                exc.format_message(), option, section
+                exc.format_message(),
+                option,
+                " (%s) " % option_meta.description,
+                section,
             )
 
     @staticmethod
     def cast_to(value, to_type):
         items = value
         if not isinstance(value, (list, tuple)):
             items = [value]
@@ -420,24 +427,59 @@
         if not silent:
             for warning in self.warnings:
                 click.secho("Warning! %s" % warning, fg="yellow")
 
         return True
 
 
+class ProjectConfigLintMixin:
+    @classmethod
+    def lint(cls, path=None):
+        errors = []
+        warnings = []
+        try:
+            config = cls.get_instance(path)
+            config.validate(silent=True)
+            warnings = config.warnings
+            config.as_tuple()
+        except Exception as exc:  # pylint: disable=broad-exception-caught
+            if exc.__cause__ is not None:
+                exc = exc.__cause__
+
+            item = {"type": exc.__class__.__name__, "message": str(exc)}
+            for attr in ("lineno", "source"):
+                if hasattr(exc, attr):
+                    item[attr] = getattr(exc, attr)
+
+            if item["type"] == "ParsingError" and hasattr(exc, "errors"):
+                for lineno, line in getattr(exc, "errors"):
+                    errors.append(
+                        {
+                            "type": item["type"],
+                            "message": f"Parsing error: {line}",
+                            "lineno": lineno,
+                            "source": item["source"],
+                        }
+                    )
+            else:
+                errors.append(item)
+        return {"errors": errors, "warnings": warnings}
+
+
 class ProjectConfigDirsMixin:
     def get_optional_dir(self, name):
         """
         Deprecated, used by platformio-node-helpers.project.observer.fetchLibDirs
         PlatformIO IDE for Atom depends on platformio-node-helpers@~7.2.0
+        PIO Home 3.0 Project Inspection depends on it
         """
         return self.get("platformio", f"{name}_dir")
 
 
-class ProjectConfig(ProjectConfigBase, ProjectConfigDirsMixin):
+class ProjectConfig(ProjectConfigBase, ProjectConfigLintMixin, ProjectConfigDirsMixin):
     _instances = {}
 
     @staticmethod
     def get_instance(path=None):
         path = ProjectConfig.get_default_path() if path is None else path
         mtime = os.path.getmtime(path) if os.path.isfile(path) else 0
         instance = ProjectConfig._instances.get(path)
```

### Comparing `platformio-6.1.7/platformio/project/exception.py` & `platformio-6.1.8/platformio/project/exception.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,8 +47,8 @@
     MESSAGE = (
         "Invalid environment name '{0}'. The name can contain "
         "alphanumeric, underscore, and hyphen characters (a-z, 0-9, -, _)"
     )
 
 
 class ProjectOptionValueError(ProjectError, UserSideException):
-    MESSAGE = "{0} for option `{1}` in section [{2}]"
+    MESSAGE = "{0} for option `{1}`{2}in section [{3}]"
```

### Comparing `platformio-6.1.7/platformio/project/helpers.py` & `platformio-6.1.8/platformio/project/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -160,28 +160,31 @@
 
 # Backward compatibiility with dev-platforms
 load_project_ide_data = load_build_metadata
 
 
 def _load_build_metadata(project_dir, env_names, debug=False):
     # pylint: disable=import-outside-toplevel
+    from platformio import app
     from platformio.run.cli import cli as cmd_run
 
     args = ["--project-dir", project_dir, "--target", "__idedata"]
     if debug:
         args.extend(["--target", "__debug"])
     for name in env_names:
         args.extend(["-e", name])
+    app.set_session_var("pause_telemetry", True)
     result = CliRunner().invoke(cmd_run, args)
+    app.set_session_var("pause_telemetry", False)
     if result.exit_code != 0 and not isinstance(
         result.exception, exception.ReturnErrorCode
     ):
         raise result.exception
     if '"includes":' not in result.output:
-        raise exception.PlatformioException(result.output)
+        raise exception.UserSideException(result.output)
     return _get_cached_build_metadata(project_dir, env_names)
 
 
 def _get_cached_build_metadata(project_dir, env_names):
     build_dir = ProjectConfig.get_instance(
         os.path.join(project_dir, "platformio.ini")
     ).get("platformio", "build_dir")
```

### Comparing `platformio-6.1.7/platformio/project/integration/__init__.py` & `platformio-6.1.8/platformio/project/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/project/integration/generator.py` & `platformio-6.1.8/platformio/project/integration/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             items = self.config.items(env=env, as_dict=True)
             if "board" in items and items.get("board") in boards:
                 return env
         return envname
 
     @staticmethod
     def get_ide_tpls_dir():
-        return os.path.join(fs.get_assets_dir(), "templates", "ide-projects")
+        return os.path.join(os.path.dirname(__file__), "tpls")
 
     @classmethod
     def get_supported_ides(cls):
         tpls_dir = cls.get_ide_tpls_dir()
         return sorted(
             [
                 name
```

### Comparing `platformio-6.1.7/platformio/project/options.py` & `platformio-6.1.8/platformio/project/options.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/project/savedeps.py` & `platformio-6.1.8/platformio/project/savedeps.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/public.py` & `platformio-6.1.8/platformio/public.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/registry/__init__.py` & `platformio-6.1.8/platformio/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/registry/access/__init__.py` & `platformio-6.1.8/platformio/registry/access/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/registry/access/cli.py` & `platformio-6.1.8/platformio/registry/access/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/registry/access/commands/__init__.py` & `platformio-6.1.8/platformio/registry/access/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/registry/access/commands/grant.py` & `platformio-6.1.8/platformio/registry/access/commands/grant.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/registry/access/commands/list.py` & `platformio-6.1.8/platformio/registry/access/commands/list.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/registry/access/commands/private.py` & `platformio-6.1.8/platformio/registry/access/commands/private.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/registry/access/commands/public.py` & `platformio-6.1.8/platformio/registry/access/commands/public.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/registry/access/commands/revoke.py` & `platformio-6.1.8/platformio/registry/access/commands/revoke.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/registry/access/validate.py` & `platformio-6.1.8/platformio/registry/access/validate.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/registry/client.py` & `platformio-6.1.8/platformio/registry/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,20 +138,20 @@
             "get",
             "/v3/search",
             params=params,
             x_cache_valid="1h",
             x_with_authorization=self.allowed_private_packages(),
         )
 
-    def get_package(self, type_, owner, name, version=None, extra_path=None):
+    def get_package(self, typex, owner, name, version=None, extra_path=None):
         try:
             return self.fetch_json_data(
                 "get",
                 "/v3/packages/{owner}/{type}/{name}{extra_path}".format(
-                    type=type_,
+                    type=typex,
                     owner=owner.lower(),
                     name=name.lower(),
                     extra_path=extra_path or "",
                 ),
                 params=dict(version=version) if version else None,
                 x_cache_valid="1h",
                 x_with_authorization=self.allowed_private_packages(),
```

### Comparing `platformio-6.1.7/platformio/registry/mirror.py` & `platformio-6.1.8/platformio/registry/mirror.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/remote/__init__.py` & `platformio-6.1.8/platformio/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/remote/ac/__init__.py` & `platformio-6.1.8/platformio/remote/ac/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/remote/ac/base.py` & `platformio-6.1.8/platformio/remote/ac/base.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/remote/ac/process.py` & `platformio-6.1.8/platformio/remote/ac/process.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/remote/ac/psync.py` & `platformio-6.1.8/platformio/remote/ac/psync.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/remote/ac/serial.py` & `platformio-6.1.8/platformio/remote/ac/serial.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/remote/cli.py` & `platformio-6.1.8/platformio/remote/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/remote/client/__init__.py` & `platformio-6.1.8/platformio/remote/client/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/remote/client/agent_list.py` & `platformio-6.1.8/platformio/remote/client/agent_list.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/remote/client/agent_service.py` & `platformio-6.1.8/platformio/remote/client/agent_service.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/remote/client/async_base.py` & `platformio-6.1.8/platformio/remote/client/async_base.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/remote/client/base.py` & `platformio-6.1.8/platformio/remote/client/base.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/remote/client/device_list.py` & `platformio-6.1.8/platformio/remote/client/device_list.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/remote/client/device_monitor.py` & `platformio-6.1.8/platformio/remote/client/device_monitor.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/remote/client/run_or_test.py` & `platformio-6.1.8/platformio/remote/client/run_or_test.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/remote/client/update_core.py` & `platformio-6.1.8/platformio/remote/client/update_core.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/remote/factory/__init__.py` & `platformio-6.1.8/platformio/remote/factory/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/remote/factory/client.py` & `platformio-6.1.8/platformio/remote/factory/client.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/remote/factory/ssl.py` & `platformio-6.1.8/platformio/remote/factory/ssl.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/remote/projectsync.py` & `platformio-6.1.8/platformio/remote/projectsync.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/run/__init__.py` & `platformio-6.1.8/platformio/run/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/run/cli.py` & `platformio-6.1.8/platformio/run/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/run/helpers.py` & `platformio-6.1.8/platformio/run/helpers.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/run/processor.py` & `platformio-6.1.8/platformio/run/processor.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/system/__init__.py` & `platformio-6.1.8/platformio/system/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/system/cli.py` & `platformio-6.1.8/platformio/system/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/system/commands/__init__.py` & `platformio-6.1.8/platformio/system/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/system/commands/completion.py` & `platformio-6.1.8/platformio/system/commands/completion.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/system/commands/info.py` & `platformio-6.1.8/platformio/system/commands/info.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,13 +73,12 @@
         "title": "Tools & Toolchains",
         "value": len(
             ToolPackageManager(
                 project_config.get("platformio", "packages_dir")
             ).get_installed()
         ),
     }
-
     click.echo(
         json.dumps(data)
         if json_output
         else tabulate([(item["title"], item["value"]) for item in data.values()])
     )
```

### Comparing `platformio-6.1.7/platformio/system/commands/prune.py` & `platformio-6.1.8/platformio/system/commands/prune.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/system/completion.py` & `platformio-6.1.8/platformio/system/completion.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,18 @@
 class ShellType(Enum):
     FISH = "fish"
     ZSH = "zsh"
     BASH = "bash"
 
 
 def get_bash_version():
-    result = subprocess.run(["bash", "--version"], capture_output=True, check=True)
-    match = re.search(r"version\s+(\d+)\.(\d+)", result.stdout.decode(), re.IGNORECASE)
+    output = subprocess.run(
+        ["bash", "--version"], check=True, stdout=subprocess.PIPE
+    ).stdout.decode()
+    match = re.search(r"version\s+(\d+)\.(\d+)", output, re.IGNORECASE)
     if match:
         return (int(match.group(1)), int(match.group(2)))
     return (0, 0)
 
 
 def get_completion_install_path(shell):
     home_dir = os.path.expanduser("~")
```

### Comparing `platformio-6.1.7/platformio/system/prune.py` & `platformio-6.1.8/platformio/system/prune.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/telemetry.py` & `platformio-6.1.8/platformio/telemetry.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,431 +10,374 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import atexit
 import hashlib
-import json
 import os
 import queue
 import re
-import shutil
 import sys
 import threading
+import time
+import traceback
 from collections import deque
-from time import sleep, time
-from traceback import format_exc
 
 import requests
 
-from platformio import __version__, app, exception, util
+from platformio import __title__, __version__, app, exception, fs, util
 from platformio.cli import PlatformioCLI
-from platformio.compat import hashlib_encode_data, string_types
-from platformio.http import HTTPSession
-from platformio.proc import is_ci, is_container
-from platformio.project.helpers import is_platformio_project
+from platformio.compat import hashlib_encode_data
+from platformio.debug.config.base import DebugConfigBase
+from platformio.http import HTTPSession, ensure_internet_on
+from platformio.proc import is_ci
+
+KEEP_MAX_REPORTS = 100
+SEND_MAX_EVENTS = 25
+
+
+class MeasurementProtocol:
+    def __init__(self, events=None):
+        self.client_id = app.get_cid()
+        self._events = events or []
+        self._user_properties = {}
+
+        self.set_user_property("systype", util.get_systype())
+        created_at = app.get_state_item("created_at", None)
+        if created_at:
+            self.set_user_property("created_at", int(created_at))
+
+    @staticmethod
+    def event_to_dict(name, params, timestamp=None):
+        event = {"name": name, "params": params}
+        if timestamp is not None:
+            event["timestamp"] = timestamp
+        return event
+
+    def set_user_property(self, name, value):
+        self._user_properties[name] = value
+
+    def add_event(self, name, params):
+        self._events.append(self.event_to_dict(name, params))
+
+    def to_payload(self):
+        return {
+            "client_id": self.client_id,
+            "user_properties": self._user_properties,
+            "events": self._events,
+        }
 
 
-class TelemetryBase:
-    def __init__(self):
-        self._params = {}
-
-    def __getitem__(self, name):
-        return self._params.get(name, None)
-
-    def __setitem__(self, name, value):
-        self._params[name] = value
-
-    def __delitem__(self, name):
-        if name in self._params:
-            del self._params[name]
-
-    def send(self, hittype):
-        raise NotImplementedError()
-
-
-class MeasurementProtocol(TelemetryBase):
-    TID = "UA-1768265-9"
-    PARAMS_MAP = {
-        "screen_name": "cd",
-        "event_category": "ec",
-        "event_action": "ea",
-        "event_label": "el",
-        "event_value": "ev",
-    }
-
+@util.singleton
+class TelemetryLogger:
     def __init__(self):
-        super().__init__()
-        self["v"] = 1
-        self["tid"] = self.TID
-        self["cid"] = app.get_cid()
+        self._events = deque()
 
-        try:
-            self["sr"] = "%dx%d" % shutil.get_terminal_size()
-        except ValueError:
-            pass
-
-        self._prefill_screen_name()
-        self._prefill_appinfo()
-        self._prefill_sysargs()
-        self._prefill_custom_data()
-
-    def __getitem__(self, name):
-        if name in self.PARAMS_MAP:
-            name = self.PARAMS_MAP[name]
-        return super().__getitem__(name)
-
-    def __setitem__(self, name, value):
-        if name in self.PARAMS_MAP:
-            name = self.PARAMS_MAP[name]
-        super().__setitem__(name, value)
-
-    def _prefill_appinfo(self):
-        self["av"] = __version__
-        self["an"] = app.get_user_agent()
-
-    def _prefill_sysargs(self):
-        args = []
-        for arg in sys.argv[1:]:
-            arg = str(arg)
-            if arg == "account":  # ignore account cmd which can contain username
-                return
-            if any(("@" in arg, "/" in arg, "\\" in arg)):
-                arg = "***"
-            args.append(arg.lower())
-        self["cd3"] = " ".join(args)
-
-    def _prefill_custom_data(self):
-        caller_id = str(app.get_session_var("caller_id"))
-        self["cd1"] = util.get_systype()
-        self["cd4"] = 1 if (not is_ci() and (caller_id or not is_container())) else 0
-        if caller_id:
-            self["cd5"] = caller_id.lower()
-
-    def _prefill_screen_name(self):
-        def _first_arg_from_list(args_, list_):
-            for _arg in args_:
-                if _arg in list_:
-                    return _arg
-            return None
-
-        args = []
-        for arg in PlatformioCLI.leftover_args:
-            if not isinstance(arg, string_types):
-                arg = str(arg)
-            if not arg.startswith("-"):
-                args.append(arg.lower())
-        if not args:
-            return
+        self._sender_thread = None
+        self._sender_queue = queue.Queue()
+        self._sender_terminated = False
 
-        cmd_path = args[:1]
-        if args[0] in (
-            "access",
-            "account",
-            "device",
-            "org",
-            "package",
-            "pkg",
-            "platform",
-            "project",
-            "settings",
-            "system",
-            "team",
-        ):
-            cmd_path = args[:2]
-        if args[0] == "lib" and len(args) > 1:
-            lib_subcmds = (
-                "builtin",
-                "install",
-                "list",
-                "register",
-                "search",
-                "show",
-                "stats",
-                "uninstall",
-                "update",
-            )
-            sub_cmd = _first_arg_from_list(args[1:], lib_subcmds)
-            if sub_cmd:
-                cmd_path.append(sub_cmd)
-        elif args[0] == "remote" and len(args) > 1:
-            remote_subcmds = ("agent", "device", "run", "test")
-            sub_cmd = _first_arg_from_list(args[1:], remote_subcmds)
-            if sub_cmd:
-                cmd_path.append(sub_cmd)
-                if len(args) > 2 and sub_cmd in ("agent", "device"):
-                    remote2_subcmds = ("list", "start", "monitor")
-                    sub_cmd = _first_arg_from_list(args[2:], remote2_subcmds)
-                    if sub_cmd:
-                        cmd_path.append(sub_cmd)
-        self["screen_name"] = " ".join([p.title() for p in cmd_path])
-
-    def _ignore_hit(self):
-        if not app.get_setting("enable_telemetry"):
-            return True
-        if self["ea"] in ("Idedata", "__Idedata"):
-            return True
-        return False
-
-    def send(self, hittype):
-        if self._ignore_hit():
-            return
-        self["t"] = hittype
-        # correct queue time
-        if "qt" in self._params and isinstance(self["qt"], float):
-            self["qt"] = int((time() - self["qt"]) * 1000)
-        MPDataPusher().push(self._params)
-
-
-@util.singleton
-class MPDataPusher:
-    MAX_WORKERS = 5
-
-    def __init__(self):
-        self._queue = queue.LifoQueue()
-        self._failedque = deque()
         self._http_session = HTTPSession()
         self._http_offline = False
-        self._workers = []
 
-    def push(self, item):
-        # if network is off-line
-        if self._http_offline:
-            if "qt" not in item:
-                item["qt"] = time()
-            self._failedque.append(item)
-            return
-
-        self._queue.put(item)
-        self._tune_workers()
-
-    def in_wait(self):
-        return self._queue.unfinished_tasks
+    def close(self):
+        self._http_session.close()
 
-    def get_items(self):
-        items = list(self._failedque)
-        try:
-            while True:
-                items.append(self._queue.get_nowait())
-        except queue.Empty:
-            pass
-        return items
+    def log_event(self, name, params, timestamp=None, instant_sending=False):
+        if not app.get_setting("enable_telemetry") or app.get_session_var(
+            "pause_telemetry"
+        ):
+            return None
+        timestamp = timestamp or int(time.time())
+        self._events.append(
+            MeasurementProtocol.event_to_dict(name, params, timestamp=timestamp)
+        )
+        if self._http_offline:  # if network is off-line
+            return False
+        if instant_sending:
+            self.send()
+        return True
 
-    def _tune_workers(self):
-        for i, w in enumerate(self._workers):
-            if not w.is_alive():
-                del self._workers[i]
-
-        need_nums = min(self._queue.qsize(), self.MAX_WORKERS)
-        active_nums = len(self._workers)
-        if need_nums <= active_nums:
+    def send(self):
+        if not self._events or self._sender_terminated:
             return
+        if not self._sender_thread:
+            self._sender_thread = threading.Thread(
+                target=self._sender_worker, daemon=True
+            )
+            self._sender_thread.start()
+        while self._events:
+            events = []
+            try:
+                while len(events) < SEND_MAX_EVENTS:
+                    events.append(self._events.popleft())
+            except IndexError:
+                pass
+            self._sender_queue.put(events)
 
-        for i in range(need_nums - active_nums):
-            t = threading.Thread(target=self._worker)
-            t.daemon = True
-            t.start()
-            self._workers.append(t)
-
-    def _worker(self):
+    def _sender_worker(self):
         while True:
+            if self._sender_terminated:
+                return
             try:
-                item = self._queue.get()
-                _item = item.copy()
-                if "qt" not in _item:
-                    _item["qt"] = time()
-                self._failedque.append(_item)
-                if self._send_data(item):
-                    self._failedque.remove(_item)
-                self._queue.task_done()
-            except:  # pylint: disable=W0702
+                events = self._sender_queue.get()
+                if not self._commit_events(events):
+                    self._events.extend(events)
+                self._sender_queue.task_done()
+            except (queue.Empty, ValueError):
                 pass
 
-    def _send_data(self, data):
+    def _commit_events(self, events):
         if self._http_offline:
             return False
+        mp = MeasurementProtocol(events)
+        payload = mp.to_payload()
+        # print("_commit_payload", payload)
         try:
             r = self._http_session.post(
-                "https://ssl.google-analytics.com/collect",
-                data=data,
-                timeout=1,
+                "https://telemetry.platformio.org/collect",
+                json=payload,
+                timeout=(2, 5),  # connect, read
             )
             r.raise_for_status()
             return True
         except requests.exceptions.HTTPError as exc:
             # skip Bad Request
-            if 400 >= exc.response.status_code < 500:
+            if exc.response.status_code >= 400 and exc.response.status_code < 500:
                 return True
         except:  # pylint: disable=bare-except
             pass
         self._http_offline = True
         return False
 
+    def terminate_sender(self):
+        self._sender_terminated = True
 
-def on_command():
-    resend_backuped_reports()
+    def is_sending(self):
+        return self._sender_queue.unfinished_tasks
 
-    mp = MeasurementProtocol()
-    mp.send("screenview")
+    def get_unsent_events(self):
+        result = list(self._events)
+        try:
+            while True:
+                result.extend(self._sender_queue.get_nowait())
+        except queue.Empty:
+            pass
+        return result
 
-    if is_ci():
-        measure_ci()
 
+def log_event(name, params, instant_sending=False):
+    TelemetryLogger().log_event(name, params, instant_sending=instant_sending)
+
+
+def on_cmd_start(cmd_ctx):
+    process_postponed_logs()
+    log_command(cmd_ctx)
 
-def on_exception(e):
-    skip_conditions = [
-        isinstance(e, cls)
-        for cls in (
-            IOError,
-            exception.ReturnErrorCode,
-            exception.UserSideException,
-        )
-    ]
-    if any(skip_conditions):
-        return
-    is_fatal = any(
-        [
-            not isinstance(e, exception.PlatformioException),
-            "Error" in e.__class__.__name__,
-        ]
-    )
-    description = "%s: %s" % (
-        type(e).__name__,
-        " ".join(reversed(format_exc().split("\n"))) if is_fatal else str(e),
-    )
-    send_exception(description, is_fatal)
 
+def on_exit():
+    TelemetryLogger().send()
 
-def measure_ci():
-    event = {"category": "CI", "action": "NoName", "label": None}
+
+def log_command(ctx):
+    params = {
+        "path_args": PlatformioCLI.reveal_cmd_path_args(ctx),
+    }
+    if is_ci():
+        params["ci_actor"] = resolve_ci_actor() or "Unknown"
+    log_event("cmd_run", params)
+
+
+def resolve_ci_actor():
     known_cis = (
         "GITHUB_ACTIONS",
         "TRAVIS",
         "APPVEYOR",
         "GITLAB_CI",
         "CIRCLECI",
         "SHIPPABLE",
         "DRONE",
     )
     for name in known_cis:
         if os.getenv(name, "false").lower() == "true":
-            event["action"] = name
-            break
-    send_event(**event)
+            return name
+    return None
 
 
-def dump_run_environment(options):
+def dump_project_env_params(config, env, platform):
     non_sensitive_data = [
         "platform",
-        "platform_packages",
         "framework",
         "board",
         "upload_protocol",
         "check_tool",
         "debug_tool",
-        "monitor_filters",
         "test_framework",
     ]
-    safe_options = {k: v for k, v in options.items() if k in non_sensitive_data}
-    if is_platformio_project(os.getcwd()):
-        phash = hashlib.sha1(hashlib_encode_data(app.get_cid()))
-        safe_options["pid"] = phash.hexdigest()
-    return json.dumps(safe_options, sort_keys=True, ensure_ascii=False)
+    section = f"env:{env}"
+    params = {
+        option: config.get(section, option)
+        for option in non_sensitive_data
+        if config.has_option(section, option)
+    }
+    params["pid"] = hashlib.sha1(hashlib_encode_data(config.path)).hexdigest()
+    params["platform_name"] = platform.name
+    params["platform_version"] = platform.version
+    return params
+
 
+def log_platform_run(platform, project_config, project_env, targets=None):
+    params = dump_project_env_params(project_config, project_env, platform)
+    if targets:
+        params["targets"] = targets
+    log_event("platform_run", params, instant_sending=True)
 
-def send_run_environment(options, targets):
-    send_event(
-        "Env",
-        " ".join([t.title() for t in targets or ["run"]]),
-        dump_run_environment(options),
+
+def log_exception(exc):
+    skip_conditions = [
+        isinstance(exc, cls)
+        for cls in (
+            IOError,
+            exception.ReturnErrorCode,
+            exception.UserSideException,
+        )
+    ]
+    skip_conditions.append(not isinstance(exc, Exception))
+    if any(skip_conditions):
+        return
+    is_fatal = any(
+        [
+            not isinstance(exc, exception.PlatformioException),
+            "Error" in exc.__class__.__name__,
+        ]
     )
 
+    def _strip_module_path(match):
+        module_path = match.group(1).replace(fs.get_source_dir() + os.sep, "")
+        sp_folder_name = "site-packages"
+        sp_pos = module_path.find(sp_folder_name)
+        if sp_pos != -1:
+            module_path = module_path[sp_pos + len(sp_folder_name) + 1 :]
+        module_path = fs.to_unix_path(module_path)
+        return f'File "{module_path}",'
+
+    trace = re.sub(
+        r'File "([^"]+)",',
+        _strip_module_path,
+        traceback.format_exc(),
+        flags=re.MULTILINE,
+    )
 
-def send_event(category, action, label=None, value=None, screen_name=None):
-    mp = MeasurementProtocol()
-    mp["event_category"] = category[:150]
-    mp["event_action"] = action[:500]
-    if label:
-        mp["event_label"] = label[:500]
-    if value:
-        mp["event_value"] = int(value)
-    if screen_name:
-        mp["screen_name"] = screen_name[:2048]
-    mp.send("event")
+    params = {
+        "name": exc.__class__.__name__,
+        "description": str(exc),
+        "traceback": trace,
+        "cmd_args": sys.argv[1:],
+        "is_fatal": is_fatal,
+    }
+    log_event("exception", params)
 
 
-def send_exception(description, is_fatal=False):
+def log_debug_started(debug_config: DebugConfigBase):
+    log_event(
+        "debug_started",
+        dump_project_env_params(
+            debug_config.project_config, debug_config.env_name, debug_config.platform
+        ),
+    )
+
+
+def log_debug_exception(exc, debug_config: DebugConfigBase):
     # cleanup sensitive information, such as paths
-    description = description.replace("Traceback (most recent call last):", "")
-    description = description.replace("\\", "/")
+    description = fs.to_unix_path(str(exc))
     description = re.sub(
         r'(^|\s+|")(?:[a-z]\:)?((/[^"/]+)+)(\s+|"|$)',
         lambda m: " %s " % os.path.join(*m.group(2).split("/")[-2:]),
         description,
         re.I | re.M,
     )
-    description = re.sub(r"\s+", " ", description, flags=re.M)
-
-    mp = MeasurementProtocol()
-    mp["exd"] = description[:8192].strip()
-    mp["exf"] = 1 if is_fatal else 0
-    mp.send("exception")
+    params = {
+        "name": exc.__class__.__name__,
+        "description": description.strip(),
+    }
+    params.update(
+        dump_project_env_params(
+            debug_config.project_config, debug_config.env_name, debug_config.platform
+        )
+    )
+    log_event("debug_exception", params)
 
 
 @atexit.register
 def _finalize():
     timeout = 1000  # msec
     elapsed = 0
+    telemetry = TelemetryLogger()
+    telemetry.terminate_sender()
     try:
         while elapsed < timeout:
-            if not MPDataPusher().in_wait():
+            if not telemetry.is_sending():
                 break
-            sleep(0.2)
+            time.sleep(0.2)
             elapsed += 200
-        backup_reports(MPDataPusher().get_items())
     except KeyboardInterrupt:
         pass
+    postpone_events(telemetry.get_unsent_events())
+    telemetry.close()
 
 
-def backup_reports(items):
-    if not items:
-        return
+def load_postponed_events():
+    state_path = app.resolve_state_path(
+        "cache_dir", "telemetry.json", ensure_dir_exists=False
+    )
+    if not os.path.isfile(state_path):
+        return []
+    with app.State(state_path) as state:
+        return state.get("events", [])
 
-    KEEP_MAX_REPORTS = 100
-    tm = app.get_state_item("telemetry", {})
-    if "backup" not in tm:
-        tm["backup"] = []
-
-    for params in items:
-        # skip static options
-        for key in list(params.keys()):
-            if key in ("v", "tid", "cid", "cd1", "cd2", "sr", "an"):
-                del params[key]
-
-        # store time in UNIX format
-        if "qt" not in params:
-            params["qt"] = time()
-        elif not isinstance(params["qt"], float):
-            params["qt"] = time() - (params["qt"] / 1000)
-
-        tm["backup"].append(params)
-
-    tm["backup"] = tm["backup"][KEEP_MAX_REPORTS * -1 :]
-    app.set_state_item("telemetry", tm)
-
-
-def resend_backuped_reports():
-    tm = app.get_state_item("telemetry", {})
-    if "backup" not in tm or not tm["backup"]:
-        return False
 
-    for report in tm["backup"]:
-        mp = MeasurementProtocol()
-        for key, value in report.items():
-            mp[key] = value
-        mp.send(report["t"])
-
-    # clean
-    tm["backup"] = []
-    app.set_state_item("telemetry", tm)
+def save_postponed_events(events):
+    state_path = app.resolve_state_path("cache_dir", "telemetry.json")
+    if not events:
+        try:
+            if os.path.isfile(state_path):
+                os.remove(state_path)
+        except:  # pylint: disable=bare-except
+            pass
+        return None
+    with app.State(state_path, lock=True) as state:
+        state["events"] = events
+        state.modified = True
+    return True
+
+
+def postpone_events(events):
+    if not events:
+        return None
+    postponed_events = load_postponed_events() or []
+    timestamp = int(time.time())
+    for event in events:
+        if "timestamp" not in event:
+            event["timestamp"] = timestamp
+        postponed_events.append(event)
+    save_postponed_events(postponed_events[KEEP_MAX_REPORTS * -1 :])
+    return True
+
+
+def process_postponed_logs():
+    if not ensure_internet_on():
+        return None
+    events = load_postponed_events()
+    if not events:
+        return None
+    save_postponed_events([])  # clean
+    telemetry = TelemetryLogger()
+    for event in events:
+        if set(["name", "params", "timestamp"]) <= set(event.keys()):
+            telemetry.log_event(
+                event["name"],
+                event["params"],
+                timestamp=event["timestamp"],
+                instant_sending=False,
+            )
     return True
```

### Comparing `platformio-6.1.7/platformio/test/__init__.py` & `platformio-6.1.8/platformio/test/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/test/cli.py` & `platformio-6.1.8/platformio/test/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/test/exception.py` & `platformio-6.1.8/platformio/test/exception.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/test/helpers.py` & `platformio-6.1.8/platformio/test/helpers.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/test/reports/__init__.py` & `platformio-6.1.8/platformio/test/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/test/reports/base.py` & `platformio-6.1.8/platformio/test/reports/base.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/test/reports/json.py` & `platformio-6.1.8/platformio/test/reports/json.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/test/reports/junit.py` & `platformio-6.1.8/platformio/test/reports/junit.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/test/reports/stdout.py` & `platformio-6.1.8/platformio/test/reports/stdout.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/test/result.py` & `platformio-6.1.8/platformio/test/result.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/test/runners/__init__.py` & `platformio-6.1.8/platformio/test/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/test/runners/base.py` & `platformio-6.1.8/platformio/test/runners/base.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/test/runners/doctest.py` & `platformio-6.1.8/platformio/test/runners/doctest.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/test/runners/factory.py` & `platformio-6.1.8/platformio/test/runners/factory.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/test/runners/googletest.py` & `platformio-6.1.8/platformio/test/runners/googletest.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/test/runners/readers/__init__.py` & `platformio-6.1.8/platformio/test/runners/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/test/runners/readers/native.py` & `platformio-6.1.8/platformio/test/runners/readers/native.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/test/runners/readers/serial.py` & `platformio-6.1.8/platformio/test/runners/readers/serial.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.7/platformio/test/runners/unity.py` & `platformio-6.1.8/platformio/test/runners/unity.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,16 +51,16 @@
 #ifdef __cplusplus
 extern "C"
 {
 #endif
 
 void unityOutputStart(unsigned long);
 void unityOutputChar(unsigned int);
-void unityOutputFlush();
-void unityOutputComplete();
+void unityOutputFlush(void);
+void unityOutputComplete(void);
 
 #define UNITY_OUTPUT_START()    unityOutputStart((unsigned long) $baudrate)
 #define UNITY_OUTPUT_CHAR(c)    unityOutputChar(c)
 #define UNITY_OUTPUT_FLUSH()    unityOutputFlush()
 #define UNITY_OUTPUT_COMPLETE() unityOutputComplete()
 
 #ifdef __cplusplus
@@ -242,26 +242,28 @@
     def generate_unity_extras(self, dst_dir):
         dst_dir = Path(dst_dir)
         if not dst_dir.is_dir():
             dst_dir.mkdir(parents=True)
         unity_h = dst_dir / "unity_config.h"
         if not unity_h.is_file():
             unity_h.write_text(
-                string.Template(self.UNITY_CONFIG_H).substitute(
-                    baudrate=self.get_test_speed()
-                ),
+                string.Template(self.UNITY_CONFIG_H)
+                .substitute(baudrate=self.get_test_speed())
+                .strip()
+                + "\n",
                 encoding="utf8",
             )
         framework_config = self.get_unity_framework_config()
         unity_c = dst_dir / ("unity_config.%s" % framework_config.get("language", "c"))
         if not unity_c.is_file():
             unity_c.write_text(
-                string.Template(self.UNITY_CONFIG_C).substitute(
-                    framework_config_code=framework_config["code"]
-                ),
+                string.Template(self.UNITY_CONFIG_C)
+                .substitute(framework_config_code=framework_config["code"])
+                .strip()
+                + "\n",
                 encoding="utf8",
             )
 
     def on_testing_line_output(self, line):
         if self.options.verbose:
             click.echo(line, nl=False)
         line = strip_ansi_codes(line or "").strip()
```

### Comparing `platformio-6.1.7/platformio/util.py` & `platformio-6.1.8/platformio/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import datetime
 import functools
 import math
 import platform
 import re
 import shutil
 import time
-from datetime import datetime
 
 import click
 
 from platformio import __version__
 
 # pylint: disable=unused-import
 from platformio.device.list.util import list_serial_ports as get_serial_ports
@@ -165,16 +165,16 @@
     if "*" in needle or "*" in haystack:
         return True
     return set(needle) & set(haystack)
 
 
 def parse_datetime(datestr):
     if "T" in datestr and "Z" in datestr:
-        return datetime.strptime(datestr, "%Y-%m-%dT%H:%M:%SZ")
-    return datetime.strptime(datestr)
+        return datetime.datetime.strptime(datestr, "%Y-%m-%dT%H:%M:%SZ")
+    return datetime.datetime.strptime(datestr)
 
 
 def merge_dicts(d1, d2, path=None):
     if path is None:
         path = []
     for key in d2:
         if key in d1 and isinstance(d1[key], dict) and isinstance(d2[key], dict):
```

### Comparing `platformio-6.1.7/platformio.egg-info/PKG-INFO` & `platformio-6.1.8/platformio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: platformio
-Version: 6.1.7
+Version: 6.1.8
 Summary: A professional collaborative platform for embedded development. Cross-platform IDE and Unified Debugger. Static Code Analyzer and Remote Unit Testing. Multi-platform and Multi-architecture Build System. Firmware File Explorer and Memory Inspection. IoT, Arduino, CMSIS, ESP-IDF, FreeRTOS, libOpenCM3, mbedOS, Pulp OS, SPL, STM32Cube, Zephyr RTOS, ARM, AVR, Espressif (ESP8266/ESP32), FPGA, MCS-51 (8051), MSP430, Nordic (nRF51/nRF52), NXP i.MX RT, PIC32, RISC-V, STMicroelectronics (STM8/STM32), Teensy
 Home-page: https://platformio.org
 Author: PlatformIO Labs
 Author-email: contact@piolabs.com
 License: Apache Software License
 Keywords: iot,embedded,arduino,mbed,esp8266,esp32,fpga,firmware,continuous-integration,cloud-ide,avr,arm,ide,unit-testing,hardware,verilog,microcontroller,debug
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
@@ -118,7 +119,8 @@
 
 The PlatformIO is licensed under the permissive Apache 2.0 license,
 so you can use it in both commercial and personal projects with confidence.
 
 .. image:: https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/banner-direct.svg
     :target: https://github.com/vshymanskyy/StandWithUkraine/blob/main/docs/README.md
     :alt:  SWUbanner
+
```

### Comparing `platformio-6.1.7/setup.py` & `platformio-6.1.8/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,52 +8,68 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import sys
 from setuptools import find_packages, setup
 
 from platformio import (
     __author__,
     __description__,
     __email__,
     __license__,
     __title__,
     __url__,
     __version__,
 )
 
-PY36 = sys.version_info < (3, 7)
-
+env_marker_below_37 = "python_version < '3.7'"
+env_marker_gte_37 = "python_version >= '3.7'"
 
 minimal_requirements = [
     "bottle==0.12.*",
-    "click%s" % ("==8.0.4" if PY36 else ">=8.0.4,<9"),
+    "click==8.0.4; " + env_marker_below_37,
+    "click==8.1.*; " + env_marker_gte_37,
     "colorama",
-    "marshmallow==%s" % ("3.14.1" if PY36 else "3.*"),
-    "pyelftools>=0.27,<1",
+    "marshmallow==3.14.1; " + env_marker_below_37,
+    "marshmallow==3.19.*; " + env_marker_gte_37,
+    "pyelftools==0.29",
     "pyserial==3.5.*",  # keep in sync "device/monitor/terminal.py"
     "requests==2.*",
-    "urllib3<2", # issue 4614: urllib3 v2.0 only supports OpenSSL 1.1.1+
-    "requests==%s" % ("2.27.1" if PY36 else "2.*"),
     "semantic_version==2.10.*",
-    "tabulate==%s" % ("0.8.10" if PY36 else "0.9.*"),
+    "tabulate==0.*",
 ]
 
 home_requirements = [
-    "aiofiles==%s" % ("0.8.0" if PY36 else "23.1.*"),
-    "ajsonrpc==1.*",
-    "starlette==%s" % ("0.19.1" if PY36 else "0.26.*"),
-    "uvicorn==%s" % ("0.16.0" if PY36 else "0.22.*"),
-    "wsproto==%s" % ("1.0.0" if PY36 else "1.2.*"),
+    "aiofiles>=0.8.0",
+    "ajsonrpc==1.2.*",
+    "starlette==0.19.1; " + env_marker_below_37,
+    "starlette==0.28.*; " + env_marker_gte_37,
+    "uvicorn==0.16.0; " + env_marker_below_37,
+    "uvicorn==0.22.*; " + env_marker_gte_37,
+    "wsproto==1.0.0; " + env_marker_below_37,
+    "wsproto==1.2.*; " + env_marker_gte_37,
 ]
 
+# issue 4614: urllib3 v2.0 only supports OpenSSL 1.1.1+
+try:
+    import ssl
+
+    if ssl.OPENSSL_VERSION.startswith("OpenSSL ") and ssl.OPENSSL_VERSION_INFO < (
+        1,
+        1,
+        1,
+    ):
+        minimal_requirements.append("urllib3<2")
+except ImportError:
+    pass
+
+
 setup(
     name=__title__,
     version=__version__,
     description=__description__,
     long_description=open("README.rst").read(),
     author=__author__,
     author_email=__email__,
@@ -61,19 +77,19 @@
     license=__license__,
     install_requires=minimal_requirements + home_requirements,
     python_requires=">=3.6",
     packages=find_packages(include=["platformio", "platformio.*"]),
     package_data={
         "platformio": [
             "assets/system/99-platformio-udev.rules",
-            "assets/templates/ide-projects/*/*.tpl",
-            "assets/templates/ide-projects/*/.*.tpl",  # include hidden files
-            "assets/templates/ide-projects/*/.*/*.tpl",  # include hidden folders
-            "assets/templates/ide-projects/*/*/*.tpl",  # NetBeans
-            "assets/templates/ide-projects/*/*/*/*.tpl", # NetBeans
+            "project/integration/tpls/*/*.tpl",
+            "project/integration/tpls/*/.*.tpl",  # include hidden files
+            "project/integration/tpls/*/.*/*.tpl",  # include hidden folders
+            "project/integration/tpls/*/*/*.tpl",  # NetBeans
+            "project/integration/tpls/*/*/*/*.tpl",  # NetBeans
         ]
     },
     entry_points={
         "console_scripts": [
             "platformio = platformio.__main__:main",
             "pio = platformio.__main__:main",
             "piodebuggdb = platformio.__main__:debug_gdb_main",
```

### Comparing `platformio-6.1.7/tests/test_examples.py` & `platformio-6.1.8/tests/test_examples.py`

 * *Files identical despite different names*

