# Comparing `tmp/neuro-extras-22.2.2.tar.gz` & `tmp/neuro-extras-23.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuro-extras-22.2.2.tar", last modified: Thu Feb 17 15:24:06 2022, max compression
+gzip compressed data, was "neuro-extras-23.7.0.tar", last modified: Thu Jul  6 20:26:38 2023, max compression
```

## Comparing `neuro-extras-22.2.2.tar` & `neuro-extras-23.7.0.tar`

### file list

```diff
@@ -1,36 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 15:24:06.323310 neuro-extras-22.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)      587 2022-02-17 15:23:31.000000 neuro-extras-22.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-02-17 15:23:31.000000 neuro-extras-22.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-02-17 15:24:06.323310 neuro-extras-22.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2732 2022-02-17 15:23:31.000000 neuro-extras-22.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 15:24:06.323310 neuro-extras-22.2.2/neuro_extras/
--rw-r--r--   0 runner    (1001) docker     (121)      633 2022-02-17 15:23:31.000000 neuro-extras-22.2.2/neuro_extras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 15:24:06.323310 neuro-extras-22.2.2/neuro_extras/assets/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1214 2022-02-17 15:23:31.000000 neuro-extras-22.2.2/neuro_extras/assets/merge_docker_auths.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 15:24:06.323310 neuro-extras-22.2.2/neuro_extras/assets/seldon.package/
--rwxr-xr-x   0 runner    (1001) docker     (121)      517 2022-02-17 15:23:31.000000 neuro-extras-22.2.2/neuro_extras/assets/seldon.package/seldon.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)     1193 2022-02-17 15:23:31.000000 neuro-extras-22.2.2/neuro_extras/assets/seldon.package/seldon_model.py
--rw-r--r--   0 runner    (1001) docker     (121)      804 2022-02-17 15:23:31.000000 neuro-extras-22.2.2/neuro_extras/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1574 2022-02-17 15:23:31.000000 neuro-extras-22.2.2/neuro_extras/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     1929 2022-02-17 15:23:31.000000 neuro-extras-22.2.2/neuro_extras/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-02-17 15:23:31.000000 neuro-extras-22.2.2/neuro_extras/const.py
--rw-r--r--   0 runner    (1001) docker     (121)    19935 2022-02-17 15:23:31.000000 neuro-extras-22.2.2/neuro_extras/data.py
--rw-r--r--   0 runner    (1001) docker     (121)    12318 2022-02-17 15:23:31.000000 neuro-extras-22.2.2/neuro_extras/image.py
--rw-r--r--   0 runner    (1001) docker     (121)    11408 2022-02-17 15:23:31.000000 neuro-extras-22.2.2/neuro_extras/image_builder.py
--rw-r--r--   0 runner    (1001) docker     (121)     1988 2022-02-17 15:23:31.000000 neuro-extras-22.2.2/neuro_extras/k8s.py
--rw-r--r--   0 runner    (1001) docker     (121)     3628 2022-02-17 15:23:31.000000 neuro-extras-22.2.2/neuro_extras/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     4172 2022-02-17 15:23:31.000000 neuro-extras-22.2.2/neuro_extras/seldon.py
--rw-r--r--   0 runner    (1001) docker     (121)     3459 2022-02-17 15:23:31.000000 neuro-extras-22.2.2/neuro_extras/upload_download.py
--rw-r--r--   0 runner    (1001) docker     (121)     8919 2022-02-17 15:23:31.000000 neuro-extras-22.2.2/neuro_extras/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-02-17 15:23:31.000000 neuro-extras-22.2.2/neuro_extras/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 15:24:06.323310 neuro-extras-22.2.2/neuro_extras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-02-17 15:24:06.000000 neuro-extras-22.2.2/neuro_extras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      790 2022-02-17 15:24:06.000000 neuro-extras-22.2.2/neuro_extras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-17 15:24:06.000000 neuro-extras-22.2.2/neuro_extras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-02-17 15:24:06.000000 neuro-extras-22.2.2/neuro_extras.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-17 15:23:45.000000 neuro-extras-22.2.2/neuro_extras.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-02-17 15:24:06.000000 neuro-extras-22.2.2/neuro_extras.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-02-17 15:24:06.000000 neuro-extras-22.2.2/neuro_extras.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      919 2022-02-17 15:23:31.000000 neuro-extras-22.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1951 2022-02-17 15:24:06.327310 neuro-extras-22.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      791 2022-02-17 15:23:31.000000 neuro-extras-22.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:26:38.827865 neuro-extras-23.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-06 20:26:38.827865 neuro-extras-23.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:26:38.827865 neuro-extras-23.7.0/neuro_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:26:38.827865 neuro-extras-23.7.0/neuro_extras/assets/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1214 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/assets/merge_docker_auths.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:26:38.827865 neuro-extras-23.7.0/neuro_extras/assets/seldon.package/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      517 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/assets/seldon.package/seldon.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/assets/seldon.package/seldon_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:26:38.827865 neuro-extras-23.7.0/neuro_extras/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/data/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/data/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12534 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/data/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/data/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/data/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13168 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/data/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/data/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9498 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/data/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/data/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/data/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12328 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11428 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/image_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/seldon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10312 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/neuro_extras/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:26:38.827865 neuro-extras-23.7.0/neuro_extras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-06 20:26:38.000000 neuro-extras-23.7.0/neuro_extras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-06 20:26:38.000000 neuro-extras-23.7.0/neuro_extras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:26:38.000000 neuro-extras-23.7.0/neuro_extras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-06 20:26:38.000000 neuro-extras-23.7.0/neuro_extras.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:26:19.000000 neuro-extras-23.7.0/neuro_extras.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-06 20:26:38.000000 neuro-extras-23.7.0/neuro_extras.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 20:26:38.000000 neuro-extras-23.7.0/neuro_extras.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-06 20:26:38.831864 neuro-extras-23.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:26:38.827865 neuro-extras-23.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:26:38.827865 neuro-extras-23.7.0/tests/e2e/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:26:38.827865 neuro-extras-23.7.0/tests/e2e/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/data/cloud_to_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/data/cloud_to_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/data/local_to_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/data/local_to_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/data/platform_to_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/data/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/data/test_data_cp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/data/test_data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18187 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/test_init_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/test_k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-07-06 20:26:09.000000 neuro-extras-23.7.0/tests/e2e/test_seldon.py
```

### Comparing `neuro-extras-22.2.2/LICENSE` & `neuro-extras-23.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neuro-extras-22.2.2/README.md` & `neuro-extras-23.7.0/README.md`

 * *Files identical despite different names*

### Comparing `neuro-extras-22.2.2/neuro_extras/__init__.py` & `neuro-extras-23.7.0/neuro_extras/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,10 +12,8 @@
 
 
 def get_neuro_extras_txt(old: str, new: str) -> str:
     return NEURO_EXTRAS_UPGRADE.format(old_ver=old, new_ver=new)
 
 
 def setup_plugin(manager: PluginManager) -> None:
-    manager.config.define_str("extra", "remote-project-dir")
-
     manager.version_checker.register("neuro-extras", get_neuro_extras_txt)
```

### Comparing `neuro-extras-22.2.2/neuro_extras/assets/merge_docker_auths.sh` & `neuro-extras-23.7.0/neuro_extras/assets/merge_docker_auths.sh`

 * *Files identical despite different names*

### Comparing `neuro-extras-22.2.2/neuro_extras/assets/seldon.package/seldon.Dockerfile` & `neuro-extras-23.7.0/neuro_extras/assets/seldon.package/seldon.Dockerfile`

 * *Files identical despite different names*

### Comparing `neuro-extras-22.2.2/neuro_extras/assets/seldon.package/seldon_model.py` & `neuro-extras-23.7.0/neuro_extras/assets/seldon.package/seldon_model.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-22.2.2/neuro_extras/common.py` & `neuro-extras-23.7.0/neuro_extras/common.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-22.2.2/neuro_extras/config.py` & `neuro-extras-23.7.0/neuro_extras/config.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-22.2.2/neuro_extras/image.py` & `neuro-extras-23.7.0/neuro_extras/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from .image_builder import (
     MIN_BUILD_PRESET_CPU,
     MIN_BUILD_PRESET_MEM,
     DockerConfigAuth,
     ImageBuilder,
     create_docker_config_auth,
 )
-from .utils import get_neuro_client, select_build_preset
+from .utils import get_neuro_client, select_job_preset
 
 
 logger = logging.getLogger(__name__)
 
 
 @main.group()
 def image() -> None:
@@ -336,15 +336,15 @@
                 )
             else:
                 raise click.ClickException(
                     f"Target image '{image_uri_str}' exists. "
                     f"Use -F/--force-overwrite flag to enforce overwriting."
                 )
 
-        preset = select_build_preset(
+        preset = select_job_preset(
             preset=preset,
             client=client,
             min_cpu=MIN_BUILD_PRESET_CPU,
             min_mem=MIN_BUILD_PRESET_MEM,
         )
 
         builder_cls = ImageBuilder.get(local=local)
@@ -402,15 +402,15 @@
             "If it does exist - it will be overwritten!"
         )
         return False
     try:
         existing_images = await client.images.tags(
             neuro_sdk.RemoteImage(
                 name=image.name,
-                owner=image.owner,
+                project_name=image.project_name,
                 cluster_name=image.cluster_name,
                 registry=image.registry,
                 tag=None,
             )
         )
         return image in existing_images
     except neuro_sdk.ResourceNotFound:
```

### Comparing `neuro-extras-22.2.2/neuro_extras/image_builder.py` & `neuro-extras-23.7.0/neuro_extras/image_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,15 +214,15 @@
         docker_config = await self.create_docker_config()
         docker_config_uri = build_uri / ".docker.config.json"
         logger.debug(f"Uploading {docker_config_uri}")
         await self.save_docker_config(docker_config, docker_config_uri)
 
         cache_image = neuro_sdk.RemoteImage(
             name="layer-cache/cache",
-            owner=self._client.config.username,
+            project_name=self._client.config.project_name_or_raise,
             registry=str(self._client.config.registry_url),
             cluster_name=self._client.cluster_name,
         )
         cache_repo = self.parse_image_ref(str(cache_image))
         cache_repo = re.sub(r":.*$", "", cache_repo)  # drop tag
 
         if any(KANIKO_AUTH_PREFIX in env for env in envs):
```

### Comparing `neuro-extras-22.2.2/neuro_extras/k8s.py` & `neuro-extras-23.7.0/neuro_extras/k8s.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-22.2.2/neuro_extras/main.py` & `neuro-extras-23.7.0/neuro_extras/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 from .cli import main
 from .config import save_registry_auth  # noqa
 from .data import data_cp, data_transfer  # noqa
 from .image import image_build, image_transfer  # noqa
 from .k8s import generate_k8s_registry_secret, generate_k8s_secret  # noqa
 from .seldon import generate_seldon_deployment, seldon_init_package  # noqa
-from .upload_download import download, upload  # noqa
 
 
 logger = logging.getLogger(__name__)
 
 
 @main.command("init-aliases")
 def init_aliases() -> None:
```

### Comparing `neuro-extras-22.2.2/neuro_extras/seldon.py` & `neuro-extras-23.7.0/neuro_extras/seldon.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-22.2.2/neuro_extras/utils.py` & `neuro-extras-23.7.0/neuro_extras/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,24 +2,45 @@
 import itertools
 import logging
 import os
 import sys
 import threading
 import warnings
 from contextlib import asynccontextmanager
+from pathlib import Path
+from tempfile import TemporaryDirectory
 from types import TracebackType
 from typing import Any, AsyncIterator, Callable, Dict, List, Optional, Type
 
 import neuro_sdk
 from neuro_sdk import Client
 
 
 logger = logging.getLogger(__name__)
 
 
+class CLIRunner:
+    """Utility class for running shell commands"""
+
+    async def run_command(self, command: str, args: List[str]) -> None:
+        """Execute command with args
+
+        If resulting statuscode is non-zero, RuntimeError is thrown
+        with stderr as a message.
+        """
+        logger.info(f"Executing: {[command] + args}")
+        # logger.warn(f"Calling echo instead of actual command!")
+        # process = await asyncio.create_subprocess_exec("echo", *([command] + args))
+
+        process = await asyncio.create_subprocess_exec(command, *args)
+        status_code = await process.wait()
+        if status_code != 0:
+            raise RuntimeError(process.stderr)
+
+
 @asynccontextmanager
 async def get_neuro_client(
     cluster: Optional[str] = None,
 ) -> AsyncIterator[neuro_sdk.Client]:
     client: neuro_sdk.Client = await neuro_sdk.get()
     cluster_orig: Optional[str] = None
     try:
@@ -179,29 +200,33 @@
 
         asyncio.set_event_loop_policy(WindowsProactorEventLoopPolicy())
     else:
         if sys.version_info < (3, 8):
             asyncio.set_child_watcher(ThreadedChildWatcher())
 
 
-def select_build_preset(
+def select_job_preset(
     preset: Optional[str], client: Client, min_cpu: float = 2, min_mem: int = 4096
 ) -> Optional[str]:
     """
-    Try to automatically select the best available preset for tasak
+    Try to automatically select the best available preset for a task.
+    Memory is specified in mebibytes.
     """
     good_presets = []
     good_presets_names = []
-    # Build a shortlist of presets that
+    # Build a shortlist of presets that could fit
     for cluster_preset_name, cluster_preset_info in client.presets.items():
         # Don't even try to use GPU machines for image builds
+        # Also ignore scheduled presets (they don't work with schedule-timeout)
+        # see https://github.com/neuro-inc/neuro-extras/issues/488
         if (
             cluster_preset_info.cpu >= min_cpu
             and cluster_preset_info.memory_mb >= min_mem
             and cluster_preset_info.gpu is None
+            and not cluster_preset_info.scheduler_enabled
         ):
             good_presets.append((cluster_preset_name, cluster_preset_info))
             good_presets_names.append(cluster_preset_name)
     # Sort presets by cost - memory - cpu
     good_presets.sort(key=lambda p: (p[1].credits_per_hour, p[1].memory_mb, p[1].cpu))
 
     if preset is None:
@@ -218,15 +243,15 @@
                 "The job might take long time to accomplish. "
                 "Consider contacting your cluster manager or admin "
                 "to adjust the cluster configuration"
             )
             return None
     else:
         if preset in good_presets_names:
-            # If user asked for a preset and it's a good one - let them use it
+            # If user asked for a preset, and it's a good one - let them use it
             return preset
         else:
             if len(good_presets) > 0:
                 # We have a better preset
                 logger.warning(
                     f"The selected resource preset {preset} does not "
                     f"satisfy recommended minimum hardware requirements. "
@@ -238,7 +263,20 @@
                     f"Selected resource preset {preset} does not satisfy "
                     f"minimal hardware requirements. "
                     "The job might take long time to accomplish. "
                     "Consider contacting your cluster manager or admin "
                     "to adjust the cluster configuration"
                 )
             return preset
+
+
+def get_default_preset(neuro_client: Client) -> str:
+    """Get default preset name via Neu.ro client"""
+    return next(iter(neuro_client.presets.keys()))
+
+
+def provide_temp_dir(
+    dir: Path = Path.home() / ".neuro-tmp",
+) -> TemporaryDirectory:  # type: ignore
+    """Provide temp directory"""
+    dir.mkdir(exist_ok=True, parents=True)
+    return TemporaryDirectory(dir=dir)
```

### Comparing `neuro-extras-22.2.2/pyproject.toml` & `neuro-extras-23.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `neuro-extras-22.2.2/setup.cfg` & `neuro-extras-23.7.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 	ignore::ResourceWarning:asyncio
 	ignore::UserWarning:_pytest
 	ignore:'autocompletion' is renamed to 'shell_complete'.+:DeprecationWarning:click
 	ignore:.*Inheritance class AuthorizedSession from ClientSession is discouraged:DeprecationWarning:google
 	ignore:.*The loop argument is deprecated since Python 3.8, and scheduled for removal in Python 3.10.+:DeprecationWarning:asyncio
 markers = 
 	serial: run these tests non-parallel
+	smoke: run these tests during smoke testing
+	smoke_only: run these tests only during smoke testing
 
 [mypy]
 check_untyped_defs = True
 disallow_any_generics = True
 disallow_untyped_defs = True
 follow_imports = silent
 strict_optional = True
```

### Comparing `neuro-extras-22.2.2/setup.py` & `neuro-extras-23.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     except IndexError:
         raise RuntimeError("Unable to determine version.")
 
 
 setup(
     name="neuro-extras",
     version=version,
-    python_requires=">=3.7.0",
+    python_requires=">=3.8.0",
     url="https://github.com/neuro-inc/neuro-extras",
     packages=find_packages(),
     install_requires=[
         "neuro-cli>=21.11.4",
         "click>=8.0",
         "toml>=0.10.0",
         "pyyaml>=3.0",
```

