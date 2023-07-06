# Comparing `tmp/mob-tool-1.0.8.tar.gz` & `tmp/mob-tool-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mob-tool-1.0.8.tar", last modified: Fri Feb 17 11:33:30 2023, max compression
+gzip compressed data, was "mob-tool-1.0.9.tar", last modified: Fri Feb 17 11:38:15 2023, max compression
```

## Comparing `mob-tool-1.0.8.tar` & `mob-tool-1.0.9.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:30.624870 mob-tool-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-02-17 11:33:16.000000 mob-tool-1.0.8/.env
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:30.608869 mob-tool-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:30.612870 mob-tool-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-02-17 11:33:16.000000 mob-tool-1.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-02-17 11:33:16.000000 mob-tool-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-02-17 11:33:16.000000 mob-tool-1.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-02-17 11:33:30.624870 mob-tool-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-02-17 11:33:16.000000 mob-tool-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:30.612870 mob-tool-1.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    31687 2023-02-17 11:33:16.000000 mob-tool-1.0.8/docs/done-output.png
--rw-r--r--   0 runner    (1001) docker     (123)    20021 2023-02-17 11:33:16.000000 mob-tool-1.0.8/docs/next-output.png
--rw-r--r--   0 runner    (1001) docker     (123)    73451 2023-02-17 11:33:16.000000 mob-tool-1.0.8/docs/rollback-example.png
--rw-r--r--   0 runner    (1001) docker     (123)    32422 2023-02-17 11:33:16.000000 mob-tool-1.0.8/docs/start-output.png
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-02-17 11:33:16.000000 mob-tool-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 11:33:30.624870 mob-tool-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 11:33:16.000000 mob-tool-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:30.608869 mob-tool-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:30.612870 mob-tool-1.0.8/src/mob_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-02-17 11:33:30.000000 mob-tool-1.0.8/src/mob_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-02-17 11:33:30.000000 mob-tool-1.0.8/src/mob_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 11:33:30.000000 mob-tool-1.0.8/src/mob_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-17 11:33:30.000000 mob-tool-1.0.8/src/mob_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-02-17 11:33:30.000000 mob-tool-1.0.8/src/mob_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-17 11:33:30.000000 mob-tool-1.0.8/src/mob_tool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:30.616870 mob-tool-1.0.8/src/mobt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:30.616870 mob-tool-1.0.8/src/mobt/AutoUpdate/
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/AutoUpdate/AutoUpdateRepository.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/AutoUpdate/AutoUpdateService.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/AutoUpdate/CachedVersion.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/AutoUpdate/PyPi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/AutoUpdate/VersionCheckerThread.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/AutoUpdate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:30.616870 mob-tool-1.0.8/src/mobt/Controllers/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/Controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/Controllers/boostrap_cli_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/Controllers/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/Controllers/done.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/Controllers/next.py
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/Controllers/start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:30.616870 mob-tool-1.0.8/src/mobt/DotEnv/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/DotEnv/DotEnv.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/DotEnv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:30.616870 mob-tool-1.0.8/src/mobt/FileAccess/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/FileAccess/FileAccess.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/FileAccess/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:30.616870 mob-tool-1.0.8/src/mobt/GitCli/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/GitCli/BranchName.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/GitCli/Exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/GitCli/GitCliInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/GitCli/GitCliWithAutoRollback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:30.620870 mob-tool-1.0.8/src/mobt/GitCli/GitPython/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:30.620870 mob-tool-1.0.8/src/mobt/GitCli/GitPython/GitActions/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/GitCli/GitPython/GitActions/AddAll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/GitCli/GitPython/GitActions/AddEntryToInfoExclude.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/GitCli/GitPython/GitActions/Checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/GitCli/GitPython/GitActions/Commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/GitCli/GitPython/GitActions/ComposedGitActions.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/GitCli/GitPython/GitActions/CreateHead.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/GitCli/GitPython/GitActions/Exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/GitCli/GitPython/GitActions/GitAction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/GitCli/GitPython/GitActions/Push.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/GitCli/GitPython/GitActions/Reset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/GitCli/GitPython/GitActions/SquashAll.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/GitCli/GitPython/GitActions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/GitCli/GitPython/GitCliWithGitPython.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/GitCli/GitPython/GitLogHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/GitCli/GitPython/Module.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/GitCli/GitPython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/GitCli/Module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:30.620870 mob-tool-1.0.8/src/mobt/GitCli/UndoCommands/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/GitCli/UndoCommands/ComposedUndoCommand.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/GitCli/UndoCommands/UndoCallable.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/GitCli/UndoCommands/UndoCommand.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/GitCli/UndoCommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/GitCli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:30.620870 mob-tool-1.0.8/src/mobt/Gui/
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/Gui/GuiService.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/Gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:30.620870 mob-tool-1.0.8/src/mobt/JsonSerializer/
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/JsonSerializer/DataClassesSerializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/JsonSerializer/Exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/JsonSerializer/JsonSerializerInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/JsonSerializer/Module.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/JsonSerializer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:30.624870 mob-tool-1.0.8/src/mobt/LastTeamMembers/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/LastTeamMembers/Exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/LastTeamMembers/LastTeamMembersRepository.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/LastTeamMembers/LastTeamMembersService.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/LastTeamMembers/TeamMemberName.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/LastTeamMembers/TeamMembers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/LastTeamMembers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:30.624870 mob-tool-1.0.8/src/mobt/Logging/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/Logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/Logging/color_by_log_level.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:30.624870 mob-tool-1.0.8/src/mobt/MobApp/
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/MobApp/EndMob.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/MobApp/Exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/MobApp/MobNext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/MobApp/StartMobbing.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/MobApp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/MobException.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/MobSecrets.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/Module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:30.624870 mob-tool-1.0.8/src/mobt/SessionSettings/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/SessionSettings/Exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/SessionSettings/RotationSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/SessionSettings/SessionSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/SessionSettings/SessionSettingsRepository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/SessionSettings/SessionSettingsService.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/SessionSettings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:30.624870 mob-tool-1.0.8/src/mobt/Timer/
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/Timer/TimerService.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/Timer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/WorkDir.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-02-17 11:33:16.000000 mob-tool-1.0.8/src/mobt/di.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:38:15.347262 mob-tool-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-02-17 11:37:59.000000 mob-tool-1.0.9/.env
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:38:15.335261 mob-tool-1.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:38:15.335261 mob-tool-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-02-17 11:37:59.000000 mob-tool-1.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-02-17 11:37:59.000000 mob-tool-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-02-17 11:37:59.000000 mob-tool-1.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-02-17 11:38:15.347262 mob-tool-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-02-17 11:37:59.000000 mob-tool-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:38:15.335261 mob-tool-1.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    31687 2023-02-17 11:37:59.000000 mob-tool-1.0.9/docs/done-output.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20021 2023-02-17 11:37:59.000000 mob-tool-1.0.9/docs/next-output.png
+-rw-r--r--   0 runner    (1001) docker     (123)    73451 2023-02-17 11:37:59.000000 mob-tool-1.0.9/docs/rollback-example.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32422 2023-02-17 11:37:59.000000 mob-tool-1.0.9/docs/start-output.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-02-17 11:37:59.000000 mob-tool-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 11:38:15.347262 mob-tool-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 11:37:59.000000 mob-tool-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:38:15.335261 mob-tool-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:38:15.339262 mob-tool-1.0.9/src/mob_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-02-17 11:38:15.000000 mob-tool-1.0.9/src/mob_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-02-17 11:38:15.000000 mob-tool-1.0.9/src/mob_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 11:38:15.000000 mob-tool-1.0.9/src/mob_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-17 11:38:15.000000 mob-tool-1.0.9/src/mob_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-02-17 11:38:15.000000 mob-tool-1.0.9/src/mob_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-17 11:38:15.000000 mob-tool-1.0.9/src/mob_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:38:15.339262 mob-tool-1.0.9/src/mobt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:38:15.339262 mob-tool-1.0.9/src/mobt/AutoUpdate/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/AutoUpdate/AutoUpdateRepository.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/AutoUpdate/AutoUpdateService.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/AutoUpdate/CachedVersion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/AutoUpdate/PyPi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/AutoUpdate/VersionCheckerThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/AutoUpdate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:38:15.339262 mob-tool-1.0.9/src/mobt/Controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/Controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/Controllers/boostrap_cli_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/Controllers/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/Controllers/done.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/Controllers/next.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/Controllers/start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:38:15.339262 mob-tool-1.0.9/src/mobt/DotEnv/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/DotEnv/DotEnv.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/DotEnv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:38:15.339262 mob-tool-1.0.9/src/mobt/FileAccess/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/FileAccess/FileAccess.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/FileAccess/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:38:15.339262 mob-tool-1.0.9/src/mobt/GitCli/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/GitCli/BranchName.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/GitCli/Exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/GitCli/GitCliInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/GitCli/GitCliWithAutoRollback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:38:15.339262 mob-tool-1.0.9/src/mobt/GitCli/GitPython/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:38:15.343262 mob-tool-1.0.9/src/mobt/GitCli/GitPython/GitActions/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/GitCli/GitPython/GitActions/AddAll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/GitCli/GitPython/GitActions/AddEntryToInfoExclude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/GitCli/GitPython/GitActions/Checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/GitCli/GitPython/GitActions/Commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/GitCli/GitPython/GitActions/ComposedGitActions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/GitCli/GitPython/GitActions/CreateHead.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/GitCli/GitPython/GitActions/Exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/GitCli/GitPython/GitActions/GitAction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/GitCli/GitPython/GitActions/Push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/GitCli/GitPython/GitActions/Reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/GitCli/GitPython/GitActions/SquashAll.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/GitCli/GitPython/GitActions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/GitCli/GitPython/GitCliWithGitPython.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/GitCli/GitPython/GitLogHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/GitCli/GitPython/Module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/GitCli/GitPython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/GitCli/Module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:38:15.343262 mob-tool-1.0.9/src/mobt/GitCli/UndoCommands/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/GitCli/UndoCommands/ComposedUndoCommand.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/GitCli/UndoCommands/UndoCallable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/GitCli/UndoCommands/UndoCommand.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/GitCli/UndoCommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/GitCli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:38:15.343262 mob-tool-1.0.9/src/mobt/Gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/Gui/GuiService.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/Gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:38:15.343262 mob-tool-1.0.9/src/mobt/JsonSerializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/JsonSerializer/DataClassesSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/JsonSerializer/Exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/JsonSerializer/JsonSerializerInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/JsonSerializer/Module.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/JsonSerializer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:38:15.343262 mob-tool-1.0.9/src/mobt/LastTeamMembers/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/LastTeamMembers/Exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/LastTeamMembers/LastTeamMembersRepository.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/LastTeamMembers/LastTeamMembersService.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/LastTeamMembers/TeamMemberName.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/LastTeamMembers/TeamMembers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/LastTeamMembers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:38:15.343262 mob-tool-1.0.9/src/mobt/Logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/Logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/Logging/color_by_log_level.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:38:15.347262 mob-tool-1.0.9/src/mobt/MobApp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/MobApp/EndMob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/MobApp/Exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/MobApp/MobNext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/MobApp/StartMobbing.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/MobApp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/MobException.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/MobSecrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/Module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:38:15.347262 mob-tool-1.0.9/src/mobt/SessionSettings/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/SessionSettings/Exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/SessionSettings/RotationSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/SessionSettings/SessionSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/SessionSettings/SessionSettingsRepository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/SessionSettings/SessionSettingsService.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/SessionSettings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:38:15.347262 mob-tool-1.0.9/src/mobt/Timer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/Timer/TimerService.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/Timer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/WorkDir.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-02-17 11:37:59.000000 mob-tool-1.0.9/src/mobt/di.py
```

### Comparing `mob-tool-1.0.8/.github/workflows/python-publish.yml` & `mob-tool-1.0.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/.gitignore` & `mob-tool-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/LICENSE.txt` & `mob-tool-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/PKG-INFO` & `mob-tool-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mob-tool
-Version: 1.0.8
+Version: 1.0.9
 Summary: Mob session management tool
 Author: rfst
 License: MIT License
         
         Copyright (c) 2023
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mob-tool-1.0.8/README.md` & `mob-tool-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/docs/done-output.png` & `mob-tool-1.0.9/docs/done-output.png`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/docs/next-output.png` & `mob-tool-1.0.9/docs/next-output.png`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/docs/rollback-example.png` & `mob-tool-1.0.9/docs/rollback-example.png`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/docs/start-output.png` & `mob-tool-1.0.9/docs/start-output.png`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/pyproject.toml` & `mob-tool-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 67.3.2", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mob-tool"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
     { name = "rfst" },
 ]
 description = "Mob session management tool"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = [
```

### Comparing `mob-tool-1.0.8/src/mob_tool.egg-info/PKG-INFO` & `mob-tool-1.0.9/src/mob_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mob-tool
-Version: 1.0.8
+Version: 1.0.9
 Summary: Mob session management tool
 Author: rfst
 License: MIT License
         
         Copyright (c) 2023
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mob-tool-1.0.8/src/mob_tool.egg-info/SOURCES.txt` & `mob-tool-1.0.9/src/mob_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/AutoUpdate/AutoUpdateRepository.py` & `mob-tool-1.0.9/src/mobt/AutoUpdate/AutoUpdateRepository.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/AutoUpdate/AutoUpdateService.py` & `mob-tool-1.0.9/src/mobt/AutoUpdate/AutoUpdateService.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/AutoUpdate/CachedVersion.py` & `mob-tool-1.0.9/src/mobt/AutoUpdate/CachedVersion.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/AutoUpdate/PyPi.py` & `mob-tool-1.0.9/src/mobt/AutoUpdate/PyPi.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/AutoUpdate/VersionCheckerThread.py` & `mob-tool-1.0.9/src/mobt/AutoUpdate/VersionCheckerThread.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/Controllers/boostrap_cli_app.py` & `mob-tool-1.0.9/src/mobt/Controllers/boostrap_cli_app.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/Controllers/cli.py` & `mob-tool-1.0.9/src/mobt/Controllers/cli.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/Controllers/next.py` & `mob-tool-1.0.9/src/mobt/Controllers/next.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/Controllers/start.py` & `mob-tool-1.0.9/src/mobt/Controllers/start.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/DotEnv/DotEnv.py` & `mob-tool-1.0.9/src/mobt/DotEnv/DotEnv.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/FileAccess/FileAccess.py` & `mob-tool-1.0.9/src/mobt/FileAccess/FileAccess.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/GitCli/Exceptions.py` & `mob-tool-1.0.9/src/mobt/GitCli/Exceptions.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/GitCli/GitCliInterface.py` & `mob-tool-1.0.9/src/mobt/GitCli/GitCliInterface.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/GitCli/GitCliWithAutoRollback.py` & `mob-tool-1.0.9/src/mobt/GitCli/GitCliWithAutoRollback.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/GitCli/GitPython/GitActions/AddEntryToInfoExclude.py` & `mob-tool-1.0.9/src/mobt/GitCli/GitPython/GitActions/AddEntryToInfoExclude.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/GitCli/GitPython/GitActions/Checkout.py` & `mob-tool-1.0.9/src/mobt/GitCli/GitPython/GitActions/Checkout.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/GitCli/GitPython/GitActions/ComposedGitActions.py` & `mob-tool-1.0.9/src/mobt/GitCli/GitPython/GitActions/ComposedGitActions.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/GitCli/GitPython/GitActions/CreateHead.py` & `mob-tool-1.0.9/src/mobt/GitCli/GitPython/GitActions/CreateHead.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/GitCli/GitPython/GitActions/Exceptions.py` & `mob-tool-1.0.9/src/mobt/GitCli/GitPython/GitActions/Exceptions.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/GitCli/GitPython/GitActions/GitAction.py` & `mob-tool-1.0.9/src/mobt/GitCli/GitPython/GitActions/GitAction.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/GitCli/GitPython/GitActions/Push.py` & `mob-tool-1.0.9/src/mobt/GitCli/GitPython/GitActions/Push.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/GitCli/GitPython/GitActions/Reset.py` & `mob-tool-1.0.9/src/mobt/GitCli/GitPython/GitActions/Reset.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/GitCli/GitPython/GitActions/SquashAll.py` & `mob-tool-1.0.9/src/mobt/GitCli/GitPython/GitActions/SquashAll.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/GitCli/GitPython/GitCliWithGitPython.py` & `mob-tool-1.0.9/src/mobt/GitCli/GitPython/GitCliWithGitPython.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/GitCli/GitPython/GitLogHandler.py` & `mob-tool-1.0.9/src/mobt/GitCli/GitPython/GitLogHandler.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/GitCli/UndoCommands/ComposedUndoCommand.py` & `mob-tool-1.0.9/src/mobt/GitCli/UndoCommands/ComposedUndoCommand.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/Gui/GuiService.py` & `mob-tool-1.0.9/src/mobt/Gui/GuiService.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/JsonSerializer/DataClassesSerializer.py` & `mob-tool-1.0.9/src/mobt/JsonSerializer/DataClassesSerializer.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/LastTeamMembers/Exceptions.py` & `mob-tool-1.0.9/src/mobt/LastTeamMembers/Exceptions.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/LastTeamMembers/LastTeamMembersRepository.py` & `mob-tool-1.0.9/src/mobt/LastTeamMembers/LastTeamMembersRepository.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/LastTeamMembers/LastTeamMembersService.py` & `mob-tool-1.0.9/src/mobt/LastTeamMembers/LastTeamMembersService.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/LastTeamMembers/TeamMembers.py` & `mob-tool-1.0.9/src/mobt/LastTeamMembers/TeamMembers.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/MobApp/EndMob.py` & `mob-tool-1.0.9/src/mobt/MobApp/EndMob.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/MobApp/Exceptions.py` & `mob-tool-1.0.9/src/mobt/MobApp/Exceptions.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/MobApp/MobNext.py` & `mob-tool-1.0.9/src/mobt/MobApp/MobNext.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/MobApp/StartMobbing.py` & `mob-tool-1.0.9/src/mobt/MobApp/StartMobbing.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/SessionSettings/SessionSettingsRepository.py` & `mob-tool-1.0.9/src/mobt/SessionSettings/SessionSettingsRepository.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/SessionSettings/SessionSettingsService.py` & `mob-tool-1.0.9/src/mobt/SessionSettings/SessionSettingsService.py`

 * *Files identical despite different names*

### Comparing `mob-tool-1.0.8/src/mobt/Timer/TimerService.py` & `mob-tool-1.0.9/src/mobt/Timer/TimerService.py`

 * *Files identical despite different names*

