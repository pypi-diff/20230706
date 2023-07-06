# Comparing `tmp/lightdash_ops-0.1.1.tar.gz` & `tmp/lightdash_ops-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightdash_ops-0.1.1.tar", last modified: Thu Jun 29 07:49:13 2023, max compression
+gzip compressed data, was "lightdash_ops-0.2.0.tar", last modified: Wed Jul  5 04:29:51 2023, max compression
```

## Comparing `lightdash_ops-0.1.1.tar` & `lightdash_ops-0.2.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0       76 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/.env.template
--rw-r--r--   0        0        0      804 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/.github/CODEOWNERS
--rw-r--r--   0        0        0      402 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/.github/workflows/contributors-list.yml
--rw-r--r--   0        0        0     1836 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2310 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/.github/workflows/test-publish.yml
--rw-r--r--   0        0        0     1134 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/.github/workflows/test.yml
--rw-r--r--   0        0        0     1845 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/.gitignore
--rw-r--r--   0        0        0     1383 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    14060 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/.pylintrc
--rw-r--r--   0        0        0      150 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/.pypirc
--rw-r--r--   0        0        0        8 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/.python-version
--rw-r--r--   0        0        0      183 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/.yamllint
--rw-r--r--   0        0        0    11357 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/LICENSE
--rw-r--r--   0        0        0      856 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/Makefile
--rw-r--r--   0        0        0     1517 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/README.md
--rw-r--r--   0        0        0     1047 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/dev/lint.sh
--rw-r--r--   0        0        0      994 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/dev/lint_python.sh
--rwxr-xr-x   0        0        0     1391 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/dev/publish.sh
--rwxr-xr-x   0        0        0     1396 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/dev/setup.sh
--rwxr-xr-x   0        0        0     1170 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/dev/test_python.sh
--rw-r--r--   0        0        0     1175 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/dev/update_resources.sh
--rw-r--r--   0        0        0     5442 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/docs/cli.md
--rw-r--r--   0        0        0      879 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/__init__.py
--rw-r--r--   0        0        0      794 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/cli/__init__.py
--rw-r--r--   0        0        0     1206 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/cli/main.py
--rw-r--r--   0        0        0     3608 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/cli/organization_v1.py
--rw-r--r--   0        0        0     9130 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/cli/project_v1.py
--rw-r--r--   0        0        0     1165 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/cli/settings.py
--rw-r--r--   0        0        0      794 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/lightdash/__init__.py
--rw-r--r--   0        0        0     1239 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/lightdash/client.py
--rw-r--r--   0        0        0     3328 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/lightdash/organization.py
--rw-r--r--   0        0        0     3628 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/lightdash/project.py
--rw-r--r--   0        0        0     5168 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/lightdash/space.py
--rw-r--r--   0        0        0     5351 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/lightdash/user_group.py
--rw-r--r--   0        0        0      794 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/models/__init__.py
--rw-r--r--   0        0        0     1098 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/models/base_user.py
--rw-r--r--   0        0        0     2533 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/models/organization.py
--rw-r--r--   0        0        0     2625 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/models/project.py
--rw-r--r--   0        0        0     2854 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/models/project_member.py
--rw-r--r--   0        0        0     1852 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/models/settings.py
--rw-r--r--   0        0        0     3312 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/models/space.py
--rw-r--r--   0        0        0     1856 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/models/user_group.py
--rw-r--r--   0        0        0      794 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/operators/__init__.py
--rw-r--r--   0        0        0     4895 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/operators/organization_v1.py
--rw-r--r--   0        0        0     7739 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/operators/project_v1.py
--rw-r--r--   0        0        0      794 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/tests/__init__.py
--rw-r--r--   0        0        0      794 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/tests/lightdash/__init__.py
--rw-r--r--   0        0        0     1932 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/tests/lightdash/test_organization.py
--rw-r--r--   0        0        0     1604 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/tests/lightdash/test_project.py
--rw-r--r--   0        0        0      794 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/tests/models/__init__.py
--rw-r--r--   0        0        0     1385 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/tests/models/test_lightdash_user.py
--rw-r--r--   0        0        0     1350 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/tests/models/test_manager_settings.py
--rw-r--r--   0        0        0     1279 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/tests/models/test_project_member.py
--rw-r--r--   0        0        0     1389 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/tests/models/test_space.py
--rw-r--r--   0        0        0     3035 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/tests/models/test_user_group.py
--rw-r--r--   0        0        0      219 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/tests/resources/test-organization-config-v1.yml
--rw-r--r--   0        0        0      764 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/tests/resources/test-project-config-v1.yml
--rw-r--r--   0        0        0      325 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/tests/resources/test-user-group-config-v1.yml
--rw-r--r--   0        0        0     2122 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/tests/test_utils.py
--rw-r--r--   0        0        0     1932 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/tests/utils.py
--rw-r--r--   0        0        0     3615 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/lightdash_ops/utils.py
--rw-r--r--   0        0        0     2012 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      830 2023-06-29 07:49:13.000000 lightdash_ops-0.1.1/setup.py
--rw-r--r--   0        0        0     3579 1970-01-01 00:00:00.000000 lightdash_ops-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      103 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/.env.template
+-rw-r--r--   0        0        0      804 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      402 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/.github/workflows/contributors-list.yml
+-rw-r--r--   0        0        0     1836 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2310 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/.github/workflows/test-publish.yml
+-rw-r--r--   0        0        0     1134 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1845 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1383 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    14060 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/.pylintrc
+-rw-r--r--   0        0        0      150 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/.pypirc
+-rw-r--r--   0        0        0        8 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/.python-version
+-rw-r--r--   0        0        0      183 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/.yamllint
+-rw-r--r--   0        0        0    11357 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/LICENSE
+-rw-r--r--   0        0        0      856 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/Makefile
+-rw-r--r--   0        0        0     1536 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/README.md
+-rw-r--r--   0        0        0     1047 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/dev/lint.sh
+-rw-r--r--   0        0        0      994 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/dev/lint_python.sh
+-rwxr-xr-x   0        0        0     1391 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/dev/publish.sh
+-rwxr-xr-x   0        0        0     1396 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/dev/setup.sh
+-rwxr-xr-x   0        0        0     1170 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/dev/test_python.sh
+-rw-r--r--   0        0        0     1283 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/dev/update_resources.sh
+-rw-r--r--   0        0        0     4992 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/docs/cli.md
+-rw-r--r--   0        0        0      879 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/__init__.py
+-rw-r--r--   0        0        0      794 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/cli/__init__.py
+-rw-r--r--   0        0        0     1206 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/cli/main.py
+-rw-r--r--   0        0        0     3533 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/cli/organization_v1.py
+-rw-r--r--   0        0        0     8980 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/cli/project_v1.py
+-rw-r--r--   0        0        0     1165 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/cli/settings.py
+-rw-r--r--   0        0        0      794 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/lightdash/__init__.py
+-rw-r--r--   0        0        0     1239 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/lightdash/client.py
+-rw-r--r--   0        0        0     3328 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/lightdash/organization.py
+-rw-r--r--   0        0        0     3628 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/lightdash/project.py
+-rw-r--r--   0        0        0     5168 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/lightdash/space.py
+-rw-r--r--   0        0        0     5351 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/lightdash/user_group.py
+-rw-r--r--   0        0        0      794 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/models/__init__.py
+-rw-r--r--   0        0        0     1098 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/models/base_user.py
+-rw-r--r--   0        0        0     2533 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/models/organization.py
+-rw-r--r--   0        0        0     2625 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/models/project.py
+-rw-r--r--   0        0        0     2854 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/models/project_member.py
+-rw-r--r--   0        0        0     2297 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/models/settings.py
+-rw-r--r--   0        0        0     3312 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/models/space.py
+-rw-r--r--   0        0        0     1856 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/models/user_group.py
+-rw-r--r--   0        0        0      794 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/operators/__init__.py
+-rw-r--r--   0        0        0     4895 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/operators/organization_v1.py
+-rw-r--r--   0        0        0     7739 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/operators/project_v1.py
+-rw-r--r--   0        0        0      794 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/tests/__init__.py
+-rw-r--r--   0        0        0      794 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/tests/lightdash/__init__.py
+-rw-r--r--   0        0        0     1932 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/tests/lightdash/test_organization.py
+-rw-r--r--   0        0        0     1604 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/tests/lightdash/test_project.py
+-rw-r--r--   0        0        0      794 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/tests/models/__init__.py
+-rw-r--r--   0        0        0     1385 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/tests/models/test_lightdash_user.py
+-rw-r--r--   0        0        0     2072 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/tests/models/test_manager_settings.py
+-rw-r--r--   0        0        0     1279 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/tests/models/test_project_member.py
+-rw-r--r--   0        0        0     1389 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/tests/models/test_space.py
+-rw-r--r--   0        0        0     3035 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/tests/models/test_user_group.py
+-rw-r--r--   0        0        0      219 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/tests/resources/test-organization-config-v1.yml
+-rw-r--r--   0        0        0      764 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/tests/resources/test-project-config-v1.yml
+-rw-r--r--   0        0        0      325 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/tests/resources/test-user-group-config-v1.yml
+-rw-r--r--   0        0        0     2122 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/tests/test_utils.py
+-rw-r--r--   0        0        0     1932 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/tests/utils.py
+-rw-r--r--   0        0        0     3615 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/lightdash_ops/utils.py
+-rw-r--r--   0        0        0     2012 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      830 2023-07-05 04:29:51.000000 lightdash_ops-0.2.0/setup.py
+-rw-r--r--   0        0        0     3598 1970-01-01 00:00:00.000000 lightdash_ops-0.2.0/PKG-INFO
```

### Comparing `lightdash_ops-0.1.1/.github/CODEOWNERS` & `lightdash_ops-0.2.0/.github/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/.github/workflows/publish.yml` & `lightdash_ops-0.2.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/.github/workflows/test-publish.yml` & `lightdash_ops-0.2.0/.github/workflows/test-publish.yml`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/.github/workflows/test.yml` & `lightdash_ops-0.2.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/.gitignore` & `lightdash_ops-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/.pre-commit-config.yaml` & `lightdash_ops-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/.pylintrc` & `lightdash_ops-0.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/LICENSE` & `lightdash_ops-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/Makefile` & `lightdash_ops-0.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/README.md` & `lightdash_ops-0.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 The CLI provides many sub commands.
 Please refer to the detailed documentation in [docs/cli.ms](./docs/cli.md).
 
 #### Example
 The subsequent command is used to get all members in an organization.
 
 ```commandline
-$ lightdash-ops organization get-members --api-key "${LIGHTDASH_PERSONAL_ACCESS_TOKEN}"
+$ export LIGHTDASH_API_KEY="YOUR-LIGHTDASH-PERSONAL-ACCESS-TOKEN"
+$ lightdash-ops organization get-members
 [
   {
     "member_uuid": "ade0aef5-bca8-4cbe-819b-07803390ffb0",
     "email": "lightdash-member@example.com",
     "role": "member"
   },
   {
```

### Comparing `lightdash_ops-0.1.1/dev/lint.sh` & `lightdash_ops-0.2.0/dev/lint.sh`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/dev/lint_python.sh` & `lightdash_ops-0.2.0/dev/lint_python.sh`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/dev/publish.sh` & `lightdash_ops-0.2.0/dev/publish.sh`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/dev/setup.sh` & `lightdash_ops-0.2.0/dev/setup.sh`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/dev/test_python.sh` & `lightdash_ops-0.2.0/dev/test_python.sh`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/dev/update_resources.sh` & `lightdash_ops-0.2.0/dev/update_resources.sh`

 * *Files 14% similar despite different names*

```diff
@@ -19,12 +19,16 @@
 
 set -Eeuo pipefail
 
 # Constants
 SCRIPT_DIR="$(dirname "$(readlink -f "$0")")"
 PROJECT_ROOT="$(dirname "$SCRIPT_DIR")"
 
+# Dummy values
+export LIGHTDASH_URL="https://app.lightdash.cloud"
+export LIGHTDASH_API_KEY="dummy-api-key"
+
 # Update the documentation of the CLI
 typer lightdash_ops/cli/main.py utils docs --name "lightdash-ops" --output "docs/cli.md"
 
 # Generate the JSON schemas and env template
 python lightdash_ops/cli/main.py settings get | tee "${PROJECT_ROOT}/.env.template"
```

### Comparing `lightdash_ops-0.1.1/docs/cli.md` & `lightdash_ops-0.2.0/docs/cli.md`

 * *Files 17% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 
 ```console
 $ lightdash-ops organization get-members [OPTIONS]
 ```
 
 **Options**:
 
-* `--api-key TEXT`: Lightdash API key  [required]
 * `--role [admin|developer|editor|interactive_viewer|member|viewer]`: project role
 * `--help`: Show this message and exit.
 
 ### `lightdash-ops organization get-projects`
 
 Get all projects in an organization
 
@@ -60,30 +59,28 @@
 
 ```console
 $ lightdash-ops organization get-projects [OPTIONS]
 ```
 
 **Options**:
 
-* `--api-key TEXT`: Lightdash API key  [required]
 * `--help`: Show this message and exit.
 
 ### `lightdash-ops organization grant-role`
 
 Grant a member a role in the organization
 
 **Usage**:
 
 ```console
 $ lightdash-ops organization grant-role [OPTIONS]
 ```
 
 **Options**:
 
-* `--api-key TEXT`: Lightdash API key  [required]
 * `--email TEXT`: member email  [required]
 * `--role [admin|developer|editor|interactive_viewer|member|viewer]`: project role
 * `--help`: Show this message and exit.
 
 ## `lightdash-ops project`
 
 **Usage**:
@@ -113,15 +110,14 @@
 
 ```console
 $ lightdash-ops project get-members [OPTIONS]
 ```
 
 **Options**:
 
-* `--api-key TEXT`: Lightdash API key  [required]
 * `--project-uuid TEXT`: Lightdash project UUID  [required]
 * `--help`: Show this message and exit.
 
 ### `lightdash-ops project get-spaces`
 
 Get all spaces in a project as JSON
 
@@ -129,29 +125,27 @@
 
 ```console
 $ lightdash-ops project get-spaces [OPTIONS]
 ```
 
 **Options**:
 
-* `--api-key TEXT`: Lightdash API key  [required]
 * `--project-uuid TEXT`: Lightdash project UUID  [required]
 * `--help`: Show this message and exit.
 
 ### `lightdash-ops project grant-role`
 
 **Usage**:
 
 ```console
 $ lightdash-ops project grant-role [OPTIONS]
 ```
 
 **Options**:
 
-* `--api-key TEXT`: Lightdash API key  [required]
 * `--project-uuid TEXT`: Lightdash project UUID  [required]
 * `--role [admin|developer|editor|interactive_viewer|viewer|member]`: project role  [required]
 * `--user-email TEXT`: User email
 * `--user-uuid TEXT`: User UUID
 * `--dry-run / --no-dry-run`: Dry run if true  [default: no-dry-run]
 * `--help`: Show this message and exit.
 
@@ -161,15 +155,14 @@
 
 ```console
 $ lightdash-ops project revoke-role [OPTIONS]
 ```
 
 **Options**:
 
-* `--api-key TEXT`: Lightdash API key  [required]
 * `--project-uuid TEXT`: Lightdash project UUID  [required]
 * `--role [admin|developer|editor|interactive_viewer|viewer|member]`: project role  [required]
 * `--user-email TEXT`: User email
 * `--user-uuid TEXT`: User UUID
 * `--dry-run / --no-dry-run`: Dry run if true  [default: no-dry-run]
 * `--help`: Show this message and exit.
 
@@ -181,15 +174,14 @@
 
 ```console
 $ lightdash-ops project revoke-space-access [OPTIONS]
 ```
 
 **Options**:
 
-* `--api-key TEXT`: Lightdash API key  [required]
 * `--project-uuid TEXT`: Lightdash project UUID  [required]
 * `--space-uuid TEXT`: Lightdash space UUID  [required]
 * `--user-uuid TEXT`: Lightdash user UUID  [required]
 * `--user-email TEXT`: Lightdash user email  [required]
 * `--dry-run / --no-dry-run`: Dry run if true  [default: no-dry-run]
 * `--help`: Show this message and exit.
 
@@ -201,15 +193,14 @@
 
 ```console
 $ lightdash-ops project share-space-access [OPTIONS]
 ```
 
 **Options**:
 
-* `--api-key TEXT`: Lightdash API key  [required]
 * `--project-uuid TEXT`: Lightdash project UUID  [required]
 * `--space-uuid TEXT`: Lightdash space UUID  [required]
 * `--user-uuid TEXT`: Lightdash user UUID  [required]
 * `--user-email TEXT`: Lightdash user email  [required]
 * `--dry-run / --no-dry-run`: Dry run if true  [default: no-dry-run]
 * `--help`: Show this message and exit.
```

### Comparing `lightdash_ops-0.1.1/lightdash_ops/__init__.py` & `lightdash_ops-0.2.0/lightdash_ops/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 
-__version__ = '0.1.1'
+__version__ = '0.2.0'
```

### Comparing `lightdash_ops-0.1.1/lightdash_ops/cli/__init__.py` & `lightdash_ops-0.2.0/lightdash_ops/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/lightdash_ops/cli/main.py` & `lightdash_ops-0.2.0/lightdash_ops/cli/main.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/lightdash_ops/cli/organization_v1.py` & `lightdash_ops-0.2.0/lightdash_ops/cli/organization_v1.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,62 +27,61 @@
 
 logger = loguru.logger
 
 organization_v1_app = typer.Typer()
 
 
 @organization_v1_app.command('get-projects')
-def get_projects(
-        api_key: Annotated[str, typer.Option(help='Lightdash API key')]
-):
+def get_projects():
     """Get all projects in an organization"""
     # Get the settings
     settings = get_settings()
     # Create the Lightdash client
-    client = get_lightdash_client(api_key=api_key, base_url=settings.LIGHTDASH_BASE_URL)
+    client = get_lightdash_client(api_key=settings.LIGHTDASH_API_KEY,
+                                  base_url=settings.LIGHTDASH_URL)
     # Create the operator
     operator = OrganizationOperatorV1(client=client)
     # Get all projects
     projects = operator.get_projects()
     projects_json = json.dumps([p.dict() for p in projects], indent=2)
     print(projects_json)
 
 
 @organization_v1_app.command('get-members')
 def get_members(
-        api_key: Annotated[str, typer.Option(help='Lightdash API key')],
         role: Annotated[OrganizationRole, typer.Option(help='project role')] = None  # type: ignore[assignment]
 ):
     """Get members in an organization as JSON"""
     # Get the settings
     settings = get_settings()
     # Create the Lightdash client
-    client = get_lightdash_client(api_key=api_key, base_url=settings.LIGHTDASH_BASE_URL)
+    client = get_lightdash_client(api_key=settings.LIGHTDASH_API_KEY,
+                                  base_url=settings.LIGHTDASH_URL)
     # Create the operator
     operator = OrganizationOperatorV1(client=client)
     # Get all members in the organization
     members = operator.get_organization_members()
     if role is not None:
         members = [member for member in members if member.role == role]
     # Format output
     formatted_members = [member.dict() for member in members]
     print(json.dumps(formatted_members, indent=2))
 
 
 @organization_v1_app.command('grant-role')
 def grant_member_role(
-        api_key: Annotated[str, typer.Option(help='Lightdash API key')],
         email: Annotated[str, typer.Option(help='member email')],
         role: Annotated[OrganizationRole, typer.Option(help='project role')] = None  # type: ignore[assignment]
 ):
     """Grant a member a role in the organization"""
     # Get the settings
     settings = get_settings()
     # Create the Lightdash client
-    client = get_lightdash_client(api_key=api_key, base_url=settings.LIGHTDASH_BASE_URL)
+    client = get_lightdash_client(api_key=settings.LIGHTDASH_API_KEY,
+                                  base_url=settings.LIGHTDASH_URL)
     # Create the operator
     operator = OrganizationOperatorV1(client=client)
     # Grant the role to the member
     try:
         operator.update_member_role_by_email(email=email, role=role)
         logger.info(f'Granted {email} the role {role}')
     # pylint: disable=broad-except
```

### Comparing `lightdash_ops-0.1.1/lightdash_ops/cli/project_v1.py` & `lightdash_ops-0.2.0/lightdash_ops/cli/project_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,45 +29,45 @@
 logger = loguru.logger
 
 project_v1_app = typer.Typer()
 
 
 @project_v1_app.command('get-members')
 def get_project_members(
-        api_key: Annotated[str, typer.Option(help='Lightdash API key')],
         project_uuid: Annotated[str, typer.Option(help='Lightdash project UUID')],
 ):
     """Get the members of a project as JSON"""
     # Load the settings
     settings = get_settings()
     # Create the Lightdash client
-    client = get_lightdash_client(api_key=api_key, base_url=settings.LIGHTDASH_BASE_URL)
+    client = get_lightdash_client(api_key=settings.LIGHTDASH_API_KEY,
+                                  base_url=settings.LIGHTDASH_URL)
     # Create the operator
     operator = ProjectOperatorV1(client=client)
     members = operator.get_project_members(project_uuid=project_uuid)
     print(json.dumps(members, indent=2))
 
 
 @project_v1_app.command('grant-role')
 def grant_project_role(
-        api_key: Annotated[str, typer.Option(help='Lightdash API key')],
         project_uuid: Annotated[str, typer.Option(help='Lightdash project UUID')],
         role: Annotated[ProjectRole, typer.Option(help='project role')],
         user_email: Annotated[Optional[str], typer.Option(help='User email')] = None,
         user_uuid: Annotated[Optional[str], typer.Option(help='User UUID')] = None,
         dry_run: Annotated[bool, typer.Option(help='Dry run if true')] = False,
 ):
     # Validate inputs
     if user_email is None and user_uuid is None:
         raise typer.BadParameter('One of user_email or user_uuid must be provided')
 
     # Load the settings
     settings = get_settings()
     # Create the Lightdash client
-    client = get_lightdash_client(api_key=api_key, base_url=settings.LIGHTDASH_BASE_URL)
+    client = get_lightdash_client(api_key=settings.LIGHTDASH_API_KEY,
+                                  base_url=settings.LIGHTDASH_URL)
 
     # Find user UUID by email
     if user_uuid is not None:
         organization_operator = OrganizationOperatorV1(client=client)
         user = organization_operator.get_organization_member_by_uuid(user_uuid=user_uuid)
         if user is not None:
             user_email = user.email
@@ -82,29 +82,29 @@
         email=user_email,
         role=role,
         dry_run=dry_run)
 
 
 @project_v1_app.command('revoke-role')
 def revoke_project_role(
-        api_key: Annotated[str, typer.Option(help='Lightdash API key')],
         project_uuid: Annotated[str, typer.Option(help='Lightdash project UUID')],
         role: Annotated[ProjectRole, typer.Option(help='project role')],
         user_email: Annotated[Optional[str], typer.Option(help='User email')] = None,
         user_uuid: Annotated[Optional[str], typer.Option(help='User UUID')] = None,
         dry_run: Annotated[bool, typer.Option(help='Dry run if true')] = False,
 ):
     # Validate inputs
     if user_email is None and user_uuid is None:
         raise typer.BadParameter('One of user_email or user_uuid must be provided')
 
     # Load the settings
     settings = get_settings()
     # Create the Lightdash client
-    client = get_lightdash_client(api_key=api_key, base_url=settings.LIGHTDASH_BASE_URL)
+    client = get_lightdash_client(api_key=settings.LIGHTDASH_API_KEY,
+                                  base_url=settings.LIGHTDASH_URL)
 
     # Find user UUID by email
     if user_uuid is not None:
         organization_operator = OrganizationOperatorV1(client=client)
         user = organization_operator.get_organization_member_by_uuid(user_uuid=user_uuid)
         if user is not None:
             user_email = user.email
@@ -121,22 +121,22 @@
     # pylint: disable=broad-except
     except Exception as e:
         raise RuntimeError(f'Failed to revoke role: {e}') from e
 
 
 @project_v1_app.command('get-spaces')
 def get_spaces(
-        api_key: Annotated[str, typer.Option(help='Lightdash API key')],
         project_uuid: Annotated[str, typer.Option(help='Lightdash project UUID')],
 ):
     """Get all spaces in a project as JSON"""
     # Load the settings
     settings = get_settings()
     # Create the Lightdash client
-    client = get_lightdash_client(api_key=api_key, base_url=settings.LIGHTDASH_BASE_URL)
+    client = get_lightdash_client(api_key=settings.LIGHTDASH_API_KEY,
+                                  base_url=settings.LIGHTDASH_URL)
     # Create the operator
     operator = ProjectOperatorV1(client=client)
     # Get all spaces
     spaces = operator.get_spaces(project_uuid=project_uuid)
     # Format output
     formatted_spaces = []
     for s in spaces:
@@ -147,26 +147,26 @@
             'members': [m.email for m in s.members],
         })
     print(json.dumps(formatted_spaces, indent=2))
 
 
 @project_v1_app.command('share-space-access')
 def share_space_access(
-        api_key: Annotated[str, typer.Option(help='Lightdash API key')],
         project_uuid: Annotated[str, typer.Option(help='Lightdash project UUID')],
         space_uuid: Annotated[str, typer.Option(help='Lightdash space UUID')],
         user_uuid: Annotated[str, typer.Option(help='Lightdash user UUID')],
         user_email: Annotated[str, typer.Option(help='Lightdash user email')],
         dry_run: Annotated[bool, typer.Option(help='Dry run if true')] = False,
 ):
     """Share space access with another user"""
     # Load the settings
     settings = get_settings()
     # Create the Lightdash client
-    client = get_lightdash_client(api_key=api_key, base_url=settings.LIGHTDASH_BASE_URL)
+    client = get_lightdash_client(api_key=settings.LIGHTDASH_API_KEY,
+                                  base_url=settings.LIGHTDASH_URL)
 
     # Find user UUID by email
     if user_uuid is not None:
         organization_operator = OrganizationOperatorV1(client=client)
         user = organization_operator.get_organization_member_by_uuid(user_uuid=user_uuid)
         if user is not None:
             user_email = user.email
@@ -187,26 +187,26 @@
     # pylint: disable=broad-except
     except Exception as e:
         raise RuntimeError(f'Failed to share space access: {e}') from e
 
 
 @project_v1_app.command('revoke-space-access')
 def revoke_space_access(
-        api_key: Annotated[str, typer.Option(help='Lightdash API key')],
         project_uuid: Annotated[str, typer.Option(help='Lightdash project UUID')],
         space_uuid: Annotated[str, typer.Option(help='Lightdash space UUID')],
         user_uuid: Annotated[str, typer.Option(help='Lightdash user UUID')],
         user_email: Annotated[str, typer.Option(help='Lightdash user email')],
         dry_run: Annotated[bool, typer.Option(help='Dry run if true')] = False,
 ):
     """Share space access with another user"""
     # Load the settings
     settings = get_settings()
     # Create the Lightdash client
-    client = get_lightdash_client(api_key=api_key, base_url=settings.LIGHTDASH_BASE_URL)
+    client = get_lightdash_client(api_key=settings.LIGHTDASH_API_KEY,
+                                  base_url=settings.LIGHTDASH_URL)
 
     # Find user UUID by email
     if user_uuid is not None:
         organization_operator = OrganizationOperatorV1(client=client)
         user = organization_operator.get_organization_member_by_uuid(user_uuid=user_uuid)
         if user is not None:
             user_email = user.email
```

### Comparing `lightdash_ops-0.1.1/lightdash_ops/cli/settings.py` & `lightdash_ops-0.2.0/lightdash_ops/cli/settings.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/lightdash_ops/lightdash/__init__.py` & `lightdash_ops-0.2.0/lightdash_ops/lightdash/__init__.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/lightdash_ops/lightdash/client.py` & `lightdash_ops-0.2.0/lightdash_ops/lightdash/client.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/lightdash_ops/lightdash/organization.py` & `lightdash_ops-0.2.0/lightdash_ops/lightdash/organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/lightdash_ops/lightdash/project.py` & `lightdash_ops-0.2.0/lightdash_ops/lightdash/project.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/lightdash_ops/lightdash/space.py` & `lightdash_ops-0.2.0/lightdash_ops/lightdash/space.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/lightdash_ops/lightdash/user_group.py` & `lightdash_ops-0.2.0/lightdash_ops/lightdash/user_group.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/lightdash_ops/models/__init__.py` & `lightdash_ops-0.2.0/lightdash_ops/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/lightdash_ops/models/base_user.py` & `lightdash_ops-0.2.0/lightdash_ops/models/base_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/lightdash_ops/models/organization.py` & `lightdash_ops-0.2.0/lightdash_ops/models/organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/lightdash_ops/models/project.py` & `lightdash_ops-0.2.0/lightdash_ops/models/project.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/lightdash_ops/models/project_member.py` & `lightdash_ops-0.2.0/lightdash_ops/models/project_member.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/lightdash_ops/models/settings.py` & `lightdash_ops-0.2.0/lightdash_ops/models/settings.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,21 +22,32 @@
 class LightdashOpsSettings(BaseSettings):
     """Global settings
 
     NOTE Pydantic enables us to parse environment variables.
 
     SEE https://docs.pydantic.dev/latest/usage/settings/
     """
-    LIGHTDASH_BASE_URL: str = Field(default='https://app.lightdash.cloud',
-                                    qdescription='Lightdash base URL',
-                                    env='LIGHTDASH_BASE_URL')
+    LIGHTDASH_URL: str = Field(default=None,
+                               qdescription='Lightdash base URL',
+                               env='LIGHTDASH_URL')
+    LIGHTDASH_API_KEY: str = Field(default=None,
+                                   qdescription='Lightdash API key',
+                                   env='LIGHTDASH_API_KEY')
     LIGHTDASH_CLIENT_TIMEOUT: float = Field(default=5.0,
                                             qdescription='Lightdash base URL',
                                             env='LIGHTDASH_CLIENT_TIMEOUT')
 
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        # Validate settings
+        if self.LIGHTDASH_URL is None:
+            raise ValueError('LIGHTDASH_URL is not set')
+        if self.LIGHTDASH_API_KEY is None:
+            raise ValueError('LIGHTDASH_API_KEY is not set')
+
     class Config:
         env_file = '.env'
         env_file_encoding = 'utf-8'
 
 
 # Singleton
 @lru_cache(maxsize=None)
```

### Comparing `lightdash_ops-0.1.1/lightdash_ops/models/space.py` & `lightdash_ops-0.2.0/lightdash_ops/models/space.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/lightdash_ops/models/user_group.py` & `lightdash_ops-0.2.0/lightdash_ops/models/user_group.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/lightdash_ops/operators/__init__.py` & `lightdash_ops-0.2.0/lightdash_ops/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/lightdash_ops/operators/organization_v1.py` & `lightdash_ops-0.2.0/lightdash_ops/operators/organization_v1.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/lightdash_ops/operators/project_v1.py` & `lightdash_ops-0.2.0/lightdash_ops/operators/project_v1.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/lightdash_ops/tests/__init__.py` & `lightdash_ops-0.2.0/lightdash_ops/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/lightdash_ops/tests/lightdash/__init__.py` & `lightdash_ops-0.2.0/lightdash_ops/tests/lightdash/__init__.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/lightdash_ops/tests/lightdash/test_organization.py` & `lightdash_ops-0.2.0/lightdash_ops/tests/lightdash/test_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/lightdash_ops/tests/lightdash/test_project.py` & `lightdash_ops-0.2.0/lightdash_ops/tests/lightdash/test_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/lightdash_ops/tests/models/__init__.py` & `lightdash_ops-0.2.0/lightdash_ops/tests/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/lightdash_ops/tests/models/test_lightdash_user.py` & `lightdash_ops-0.2.0/lightdash_ops/tests/models/test_lightdash_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/lightdash_ops/tests/models/test_manager_settings.py` & `lightdash_ops-0.2.0/lightdash_ops/tests/models/test_manager_settings.py`

 * *Files 27% similar despite different names*

```diff
@@ -20,14 +20,32 @@
 from lightdash_ops.models.settings import LightdashOpsSettings
 
 
 class TestManagerSettings(unittest.TestCase):
 
     def test_set_by_env_vars(self):
         # Configure the settings by env vars
-        os.environ['LIGHTDASH_BASE_URL'] = 'http://localhost:8000'
+        os.environ['LIGHTDASH_URL'] = 'http://localhost:8000'
+        os.environ['LIGHTDASH_API_KEY'] = 'dummy-api-key'
         os.environ['LIGHTDASH_CLIENT_TIMEOUT'] = '1'
 
         # Create the settings
         settings = LightdashOpsSettings()
-        self.assertEqual(settings.LIGHTDASH_BASE_URL, 'http://localhost:8000')
+        self.assertEqual(settings.LIGHTDASH_URL, 'http://localhost:8000')
         self.assertEqual(settings.LIGHTDASH_CLIENT_TIMEOUT, 1)
+
+        # Tear down
+        del os.environ['LIGHTDASH_URL']
+        del os.environ['LIGHTDASH_CLIENT_TIMEOUT']
+        del os.environ['LIGHTDASH_API_KEY']
+
+    def test_violations(self):
+        # Test if ValueError is raised when no api key is set
+        keep_lightdash_api_key = None
+        if os.getenv('LIGHTDASH_API_KEY') is not None:
+            keep_lightdash_api_key = os.getenv('LIGHTDASH_API_KEY')
+            del os.environ['LIGHTDASH_API_KEY']
+        with self.assertRaises(ValueError):
+            LightdashOpsSettings()
+        # Tear down
+        if keep_lightdash_api_key is not None:
+            os.environ['LIGHTDASH_API_KEY'] = keep_lightdash_api_key
```

### Comparing `lightdash_ops-0.1.1/lightdash_ops/tests/models/test_project_member.py` & `lightdash_ops-0.2.0/lightdash_ops/tests/models/test_project_member.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/lightdash_ops/tests/models/test_space.py` & `lightdash_ops-0.2.0/lightdash_ops/tests/models/test_space.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/lightdash_ops/tests/models/test_user_group.py` & `lightdash_ops-0.2.0/lightdash_ops/tests/models/test_user_group.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/lightdash_ops/tests/resources/test-project-config-v1.yml` & `lightdash_ops-0.2.0/lightdash_ops/tests/resources/test-project-config-v1.yml`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/lightdash_ops/tests/test_utils.py` & `lightdash_ops-0.2.0/lightdash_ops/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/lightdash_ops/tests/utils.py` & `lightdash_ops-0.2.0/lightdash_ops/tests/utils.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/lightdash_ops/utils.py` & `lightdash_ops-0.2.0/lightdash_ops/utils.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/pyproject.toml` & `lightdash_ops-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/setup.py` & `lightdash_ops-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `lightdash_ops-0.1.1/PKG-INFO` & `lightdash_ops-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightdash-ops
-Version: 0.1.1
+Version: 0.2.0
 Summary: The CLI enables us to operate resources on Lightdash.
 Author: yu-iskw
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
@@ -77,15 +77,16 @@
 The CLI provides many sub commands.
 Please refer to the detailed documentation in [docs/cli.ms](./docs/cli.md).
 
 #### Example
 The subsequent command is used to get all members in an organization.
 
 ```commandline
-$ lightdash-ops organization get-members --api-key "${LIGHTDASH_PERSONAL_ACCESS_TOKEN}"
+$ export LIGHTDASH_API_KEY="YOUR-LIGHTDASH-PERSONAL-ACCESS-TOKEN"
+$ lightdash-ops organization get-members
 [
   {
     "member_uuid": "ade0aef5-bca8-4cbe-819b-07803390ffb0",
     "email": "lightdash-member@example.com",
     "role": "member"
   },
   {
```

