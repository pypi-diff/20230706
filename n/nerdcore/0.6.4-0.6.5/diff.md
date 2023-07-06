# Comparing `tmp/nerdcore-0.6.4.tar.gz` & `tmp/nerdcore-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nerdcore-0.6.4.tar", last modified: Thu Jul  6 18:40:58 2023, max compression
+gzip compressed data, was "nerdcore-0.6.5.tar", last modified: Thu Jul  6 18:55:48 2023, max compression
```

## Comparing `nerdcore-0.6.4.tar` & `nerdcore-0.6.5.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:40:58.262749 nerdcore-0.6.4/
--rw-rw-rw-   0 root         (0) root         (0)      192 2023-07-06 18:40:39.000000 nerdcore-0.6.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      768 2023-07-06 18:40:58.262749 nerdcore-0.6.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-06 18:40:39.000000 nerdcore-0.6.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:40:58.250749 nerdcore-0.6.4/nerdcore/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:40:58.250749 nerdcore-0.6.4/nerdcore/abilities/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/abilities/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2958 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/abilities/gpt_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:40:58.250749 nerdcore-0.6.4/nerdcore/base_entities/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/base_entities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      472 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/base_entities/command_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1898 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/base_entities/deployment_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:40:58.250749 nerdcore-0.6.4/nerdcore/base_entities/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/base_entities/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3030 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/base_entities/utils/cli_runnable_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:40:58.250749 nerdcore-0.6.4/nerdcore/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1325 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/commands/list-processes.py
--rw-rw-rw-   0 root         (0) root         (0)      865 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/commands/list.py
--rw-rw-rw-   0 root         (0) root         (0)     1627 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/commands/make.py
--rw-rw-rw-   0 root         (0) root         (0)      828 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/commands/toggle-light-mode.py
--rw-rw-rw-   0 root         (0) root         (0)      243 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/commands/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:40:58.254749 nerdcore-0.6.4/nerdcore/config/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1502 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/config/env_class.py
--rw-rw-rw-   0 root         (0) root         (0)     5757 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/config/nerd_config_class.py
--rw-rw-rw-   0 root         (0) root         (0)     3002 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/config/theme.py
--rw-rw-rw-   0 root         (0) root         (0)     1448 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/config/yaml_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2362 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/defs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:40:58.254749 nerdcore-0.6.4/nerdcore/help/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/help/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:40:58.254749 nerdcore-0.6.4/nerdcore/help/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/help/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1291 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/help/commands/list-processes.py
--rw-rw-rw-   0 root         (0) root         (0)     3006 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/help/help.py
--rw-rw-rw-   0 root         (0) root         (0)     2334 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/ncdefs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:40:58.254749 nerdcore-0.6.4/nerdcore/stor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/stor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:40:58.254749 nerdcore-0.6.4/nerdcore/stor/defaults/
--rw-rw-rw-   0 root         (0) root         (0)      231 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/stor/defaults/.default-gitignore
--rw-rw-rw-   0 root         (0) root         (0)      908 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/stor/defaults/.env.default
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/stor/defaults/DEFAULT-README.md
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/stor/defaults/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1236 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/stor/defaults/apps.py
--rw-rw-rw-   0 root         (0) root         (0)        8 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/stor/defaults/default-requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      927 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/stor/defaults/nerd-config-defaults.yaml
--rw-rw-rw-   0 root         (0) root         (0)      682 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/stor/defaults/nerd-manifest.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:40:58.254749 nerdcore-0.6.4/nerdcore/stor/entity_examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/stor/entity_examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1019 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/stor/entity_examples/example-command.py
--rw-rw-rw-   0 root         (0) root         (0)      818 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/stor/entity_examples/example-deployment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:40:58.258749 nerdcore-0.6.4/nerdcore/stor/snippets/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/stor/snippets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/stor/snippets/banner.txt
--rw-rw-rw-   0 root         (0) root         (0)      496 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/stor/snippets/header-comment.py
--rw-rw-rw-   0 root         (0) root         (0)      466 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/stor/snippets/header-comment.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:40:58.258749 nerdcore-0.6.4/nerdcore/tasks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:40:58.258749 nerdcore-0.6.4/nerdcore/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:40:58.258749 nerdcore-0.6.4/nerdcore/utils/env/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/utils/env/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      339 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/utils/env/environment_checks.py
--rw-rw-rw-   0 root         (0) root         (0)      641 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/utils/env/get_env_prop_type.py
--rw-rw-rw-   0 root         (0) root         (0)     3836 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/utils/env/update_env_class.py
--rwxrwxrwx   0 root         (0) root         (0)     3103 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/utils/ncdefs_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:40:58.258749 nerdcore-0.6.4/nerdcore/utils/nerd/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/utils/nerd/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3392 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/utils/nerd/find_entity.py
--rwxrwxrwx   0 root         (0) root         (0)     2417 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/utils/nerd/generate_nerd_configs.py
--rw-rw-rw-   0 root         (0) root         (0)     2228 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/utils/nerd/get_config_name.py
--rw-rw-rw-   0 root         (0) root         (0)     2610 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/utils/nerd/parse_nerd_args.py
--rw-rw-rw-   0 root         (0) root         (0)     1328 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/utils/nerd/run_entities.py
--rw-rw-rw-   0 root         (0) root         (0)     7059 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/utils/nerd/theme_functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:40:58.258749 nerdcore-0.6.4/nerdcore/utils/nerd_config/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/utils/nerd_config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1593 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/utils/nerd_config/load_nerd_config.py
--rw-rw-rw-   0 root         (0) root         (0)     3628 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/utils/nerd_config/nerd_config_validations.py
--rw-rw-rw-   0 root         (0) root         (0)     4017 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/utils/nerd_config/update_nerd_config_class.py
--rw-rw-rw-   0 root         (0) root         (0)     1664 2023-07-06 18:40:39.000000 nerdcore-0.6.4/nerdcore/utils/ssh_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:40:58.250749 nerdcore-0.6.4/nerdcore.egg-info/
--rw-r--r--   0 root         (0) root         (0)      768 2023-07-06 18:40:58.000000 nerdcore-0.6.4/nerdcore.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2437 2023-07-06 18:40:58.000000 nerdcore-0.6.4/nerdcore.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 18:40:58.000000 nerdcore-0.6.4/nerdcore.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-07-06 18:40:58.000000 nerdcore-0.6.4/nerdcore.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-07-06 18:40:58.000000 nerdcore-0.6.4/nerdcore.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-06 18:40:58.000000 nerdcore-0.6.4/nerdcore.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:40:58.262749 nerdcore-0.6.4/scripts/
--rwxrwxrwx   0 root         (0) root         (0)     3059 2023-07-06 18:40:39.000000 nerdcore-0.6.4/scripts/nerd
--rw-rw-rw-   0 root         (0) root         (0)     3952 2023-07-06 18:40:39.000000 nerdcore-0.6.4/scripts/nerd-new
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 18:40:58.262749 nerdcore-0.6.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1350 2023-07-06 18:40:39.000000 nerdcore-0.6.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:55:48.940764 nerdcore-0.6.5/
+-rw-rw-rw-   0 root         (0) root         (0)      192 2023-07-06 18:55:31.000000 nerdcore-0.6.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      768 2023-07-06 18:55:48.940764 nerdcore-0.6.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-06 18:55:31.000000 nerdcore-0.6.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:55:48.932764 nerdcore-0.6.5/nerdcore/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:55:48.936764 nerdcore-0.6.5/nerdcore/abilities/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/abilities/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2958 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/abilities/gpt_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:55:48.936764 nerdcore-0.6.5/nerdcore/base_entities/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/base_entities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      472 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/base_entities/command_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1898 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/base_entities/deployment_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:55:48.936764 nerdcore-0.6.5/nerdcore/base_entities/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/base_entities/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3030 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/base_entities/utils/cli_runnable_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:55:48.936764 nerdcore-0.6.5/nerdcore/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1325 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/commands/list-processes.py
+-rw-rw-rw-   0 root         (0) root         (0)      865 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/commands/list.py
+-rw-rw-rw-   0 root         (0) root         (0)     1627 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/commands/make.py
+-rw-rw-rw-   0 root         (0) root         (0)      828 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/commands/toggle-light-mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      243 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/commands/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:55:48.936764 nerdcore-0.6.5/nerdcore/config/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1502 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/config/env_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     5757 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/config/nerd_config_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     3002 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/config/theme.py
+-rw-rw-rw-   0 root         (0) root         (0)     1448 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/config/yaml_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2362 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/defs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:55:48.936764 nerdcore-0.6.5/nerdcore/help/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/help/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:55:48.936764 nerdcore-0.6.5/nerdcore/help/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/help/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1291 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/help/commands/list-processes.py
+-rw-rw-rw-   0 root         (0) root         (0)     3006 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/help/help.py
+-rw-rw-rw-   0 root         (0) root         (0)     2334 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/ncdefs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:55:48.936764 nerdcore-0.6.5/nerdcore/stor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/stor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:55:48.936764 nerdcore-0.6.5/nerdcore/stor/defaults/
+-rw-rw-rw-   0 root         (0) root         (0)      231 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/stor/defaults/.default-gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      908 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/stor/defaults/.env.default
+-rw-rw-rw-   0 root         (0) root         (0)      199 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/stor/defaults/DEFAULT-README.md
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/stor/defaults/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1236 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/stor/defaults/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)        8 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/stor/defaults/default-requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      927 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/stor/defaults/nerd-config-defaults.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      682 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/stor/defaults/nerd-manifest.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:55:48.940764 nerdcore-0.6.5/nerdcore/stor/entity_examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/stor/entity_examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/stor/entity_examples/example-command.py
+-rw-rw-rw-   0 root         (0) root         (0)      818 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/stor/entity_examples/example-deployment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:55:48.940764 nerdcore-0.6.5/nerdcore/stor/snippets/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/stor/snippets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/stor/snippets/banner.txt
+-rw-rw-rw-   0 root         (0) root         (0)      496 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/stor/snippets/header-comment.py
+-rw-rw-rw-   0 root         (0) root         (0)      466 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/stor/snippets/header-comment.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:55:48.940764 nerdcore-0.6.5/nerdcore/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:55:48.940764 nerdcore-0.6.5/nerdcore/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:55:48.940764 nerdcore-0.6.5/nerdcore/utils/env/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/utils/env/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      339 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/utils/env/environment_checks.py
+-rw-rw-rw-   0 root         (0) root         (0)      641 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/utils/env/get_env_prop_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     3836 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/utils/env/update_env_class.py
+-rwxrwxrwx   0 root         (0) root         (0)     3103 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/utils/ncdefs_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:55:48.940764 nerdcore-0.6.5/nerdcore/utils/nerd/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/utils/nerd/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3392 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/utils/nerd/find_entity.py
+-rwxrwxrwx   0 root         (0) root         (0)     2417 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/utils/nerd/generate_nerd_configs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2228 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/utils/nerd/get_config_name.py
+-rw-rw-rw-   0 root         (0) root         (0)     2610 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/utils/nerd/parse_nerd_args.py
+-rw-rw-rw-   0 root         (0) root         (0)     1328 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/utils/nerd/run_entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     7056 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/utils/nerd/theme_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:55:48.940764 nerdcore-0.6.5/nerdcore/utils/nerd_config/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/utils/nerd_config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1593 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/utils/nerd_config/load_nerd_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3628 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/utils/nerd_config/nerd_config_validations.py
+-rw-rw-rw-   0 root         (0) root         (0)     4017 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/utils/nerd_config/update_nerd_config_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     1664 2023-07-06 18:55:31.000000 nerdcore-0.6.5/nerdcore/utils/ssh_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:55:48.932764 nerdcore-0.6.5/nerdcore.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-07-06 18:55:48.000000 nerdcore-0.6.5/nerdcore.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2437 2023-07-06 18:55:48.000000 nerdcore-0.6.5/nerdcore.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 18:55:48.000000 nerdcore-0.6.5/nerdcore.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-07-06 18:55:48.000000 nerdcore-0.6.5/nerdcore.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-07-06 18:55:48.000000 nerdcore-0.6.5/nerdcore.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-06 18:55:48.000000 nerdcore-0.6.5/nerdcore.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 18:55:48.940764 nerdcore-0.6.5/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)     3059 2023-07-06 18:55:31.000000 nerdcore-0.6.5/scripts/nerd
+-rw-rw-rw-   0 root         (0) root         (0)     3952 2023-07-06 18:55:31.000000 nerdcore-0.6.5/scripts/nerd-new
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 18:55:48.940764 nerdcore-0.6.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1350 2023-07-06 18:55:31.000000 nerdcore-0.6.5/setup.py
```

### Comparing `nerdcore-0.6.4/PKG-INFO` & `nerdcore-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerdcore
-Version: 0.6.4
+Version: 0.6.5
 Home-page: https://bitbucket.org/fivable/nerd-cli.git
 Author: David Wallace Cooley Jr
 Author-email: david@fivable.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `nerdcore-0.6.4/nerdcore/abilities/gpt_client.py` & `nerdcore-0.6.5/nerdcore/abilities/gpt_client.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/nerdcore/base_entities/deployment_class.py` & `nerdcore-0.6.5/nerdcore/base_entities/deployment_class.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/nerdcore/base_entities/utils/cli_runnable_class.py` & `nerdcore-0.6.5/nerdcore/base_entities/utils/cli_runnable_class.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/nerdcore/commands/list-processes.py` & `nerdcore-0.6.5/nerdcore/commands/list-processes.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/nerdcore/commands/list.py` & `nerdcore-0.6.5/nerdcore/commands/list.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/nerdcore/commands/make.py` & `nerdcore-0.6.5/nerdcore/commands/make.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/nerdcore/commands/toggle-light-mode.py` & `nerdcore-0.6.5/nerdcore/commands/toggle-light-mode.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/nerdcore/config/env_class.py` & `nerdcore-0.6.5/nerdcore/config/env_class.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/nerdcore/config/nerd_config_class.py` & `nerdcore-0.6.5/nerdcore/config/nerd_config_class.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/nerdcore/config/theme.py` & `nerdcore-0.6.5/nerdcore/config/theme.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/nerdcore/config/yaml_helpers.py` & `nerdcore-0.6.5/nerdcore/config/yaml_helpers.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/nerdcore/defs.py` & `nerdcore-0.6.5/nerdcore/defs.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/nerdcore/help/commands/list-processes.py` & `nerdcore-0.6.5/nerdcore/help/commands/list-processes.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/nerdcore/help/help.py` & `nerdcore-0.6.5/nerdcore/help/help.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/nerdcore/ncdefs.py` & `nerdcore-0.6.5/nerdcore/ncdefs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 from pkg_resources import resource_filename
 
-VERSION = '0.6.4'
+VERSION = '0.6.5'
 
 """  CORE PATHS
 
 This is a framework-level PATH definitions file.
 It is separate from defs.py for usage in nerd-new, when there is no project ROOT_PATH.
 It is also used anywhere else a framework-level path is needed.
 - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -  """
```

### Comparing `nerdcore-0.6.4/nerdcore/stor/defaults/.env.default` & `nerdcore-0.6.5/nerdcore/stor/defaults/.env.default`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/nerdcore/stor/defaults/apps.py` & `nerdcore-0.6.5/nerdcore/stor/defaults/apps.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/nerdcore/stor/defaults/nerd-config-defaults.yaml` & `nerdcore-0.6.5/nerdcore/stor/defaults/nerd-config-defaults.yaml`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/nerdcore/stor/defaults/nerd-manifest.yaml` & `nerdcore-0.6.5/nerdcore/stor/defaults/nerd-manifest.yaml`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/nerdcore/stor/entity_examples/example-command.py` & `nerdcore-0.6.5/nerdcore/stor/entity_examples/example-command.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/nerdcore/stor/entity_examples/example-deployment.py` & `nerdcore-0.6.5/nerdcore/stor/entity_examples/example-deployment.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/nerdcore/utils/env/get_env_prop_type.py` & `nerdcore-0.6.5/nerdcore/utils/env/get_env_prop_type.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/nerdcore/utils/env/update_env_class.py` & `nerdcore-0.6.5/nerdcore/utils/env/update_env_class.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/nerdcore/utils/ncdefs_utils.py` & `nerdcore-0.6.5/nerdcore/utils/ncdefs_utils.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/nerdcore/utils/nerd/find_entity.py` & `nerdcore-0.6.5/nerdcore/utils/nerd/find_entity.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/nerdcore/utils/nerd/generate_nerd_configs.py` & `nerdcore-0.6.5/nerdcore/utils/nerd/generate_nerd_configs.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/nerdcore/utils/nerd/get_config_name.py` & `nerdcore-0.6.5/nerdcore/utils/nerd/get_config_name.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/nerdcore/utils/nerd/parse_nerd_args.py` & `nerdcore-0.6.5/nerdcore/utils/nerd/parse_nerd_args.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/nerdcore/utils/nerd/run_entities.py` & `nerdcore-0.6.5/nerdcore/utils/nerd/run_entities.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/nerdcore/utils/nerd/theme_functions.py` & `nerdcore-0.6.5/nerdcore/utils/nerd/theme_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 ENV = import_env_class()
 env = ENV.get()
 text_themes = env.text_themes
 light_mode_enabled = env.light_mode_enabled
 max_terminal_width = env.max_terminal_width
 keywords = env.keywords
 
+print_lock = threading.Lock()
+
 
 def get_theme(theme):
     theme_values = text_themes.get(theme)
     if theme_values:
         prefix = theme_values['pre']
         color = theme_values['light_mode'] if light_mode_enabled else theme_values['color']
         return True, color, prefix
@@ -86,15 +88,14 @@
             for i, line in enumerate(text.split(nl))
         )
 
     color_pattern = re.compile(r'(\x1b\[[0-9;]*m)(.*?)(\x1b\[0m)', re.DOTALL)
 
     text = color_pattern.sub(lambda m: m.group(1) + apply_bold_to_keywords(m.group(2)) + m.group(3), text)
 
-    print_lock = threading.Lock()
     with print_lock:
         print(text, end=end, file=file, flush=flush)
 
 
 def apply_bold_to_keywords(text):
     return re.sub(fr"(?i)\b{'|'.join(keywords)}\b", r'\033[1m\g<0>\033[22m', text)
```

### Comparing `nerdcore-0.6.4/nerdcore/utils/nerd_config/load_nerd_config.py` & `nerdcore-0.6.5/nerdcore/utils/nerd_config/load_nerd_config.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/nerdcore/utils/nerd_config/nerd_config_validations.py` & `nerdcore-0.6.5/nerdcore/utils/nerd_config/nerd_config_validations.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/nerdcore/utils/nerd_config/update_nerd_config_class.py` & `nerdcore-0.6.5/nerdcore/utils/nerd_config/update_nerd_config_class.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/nerdcore/utils/ssh_utils.py` & `nerdcore-0.6.5/nerdcore/utils/ssh_utils.py`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/nerdcore.egg-info/PKG-INFO` & `nerdcore-0.6.5/nerdcore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerdcore
-Version: 0.6.4
+Version: 0.6.5
 Home-page: https://bitbucket.org/fivable/nerd-cli.git
 Author: David Wallace Cooley Jr
 Author-email: david@fivable.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `nerdcore-0.6.4/nerdcore.egg-info/SOURCES.txt` & `nerdcore-0.6.5/nerdcore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/scripts/nerd` & `nerdcore-0.6.5/scripts/nerd`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/scripts/nerd-new` & `nerdcore-0.6.5/scripts/nerd-new`

 * *Files identical despite different names*

### Comparing `nerdcore-0.6.4/setup.py` & `nerdcore-0.6.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nerdcore',
-    version='0.6.4',
+    version='0.6.5',
     __description__="Nerd CLI is a Fivable-specific and highly configurable CLI tool for creating/running deployments, " \
                     "commands, and more.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://bitbucket.org/fivable/nerd-cli.git',
     author='David Wallace Cooley Jr',
     author_email='david@fivable.com',
```

