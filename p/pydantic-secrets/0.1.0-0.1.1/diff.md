# Comparing `tmp/pydantic_secrets-0.1.0.tar.gz` & `tmp/pydantic_secrets-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_secrets-0.1.0.tar", max compression
+gzip compressed data, was "pydantic_secrets-0.1.1.tar", max compression
```

## Comparing `pydantic_secrets-0.1.0.tar` & `pydantic_secrets-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0     1071 2023-07-05 19:12:54.349556 pydantic_secrets-0.1.0/LICENSE
--rw-r--r--   0        0        0       18 2023-07-05 19:12:54.349556 pydantic_secrets-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-05 19:21:11.952875 pydantic_secrets-0.1.0/pydantic_secrets/__init__.py
--rw-r--r--   0        0        0     2343 2023-07-05 19:44:16.051183 pydantic_secrets-0.1.0/pydantic_secrets/main.py
--rw-r--r--   0        0        0      147 2023-07-05 19:34:14.957710 pydantic_secrets-0.1.0/pydantic_secrets/protocols.py
--rw-r--r--   0        0        0       19 2023-07-05 19:21:50.641121 pydantic_secrets-0.1.0/pydantic_secrets/version.py
--rw-r--r--   0        0        0      569 2023-07-05 19:20:41.864683 pydantic_secrets-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      537 1970-01-01 00:00:00.000000 pydantic_secrets-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-05 19:12:54.349556 pydantic_secrets-0.1.1/LICENSE
+-rw-r--r--   0        0        0       18 2023-07-05 19:12:54.349556 pydantic_secrets-0.1.1/README.md
+-rw-r--r--   0        0        0      241 2023-07-05 21:27:13.228366 pydantic_secrets-0.1.1/pydantic_secrets/__init__.py
+-rw-r--r--   0        0        0      177 2023-07-05 21:36:14.151516 pydantic_secrets-0.1.1/pydantic_secrets/abstract.py
+-rw-r--r--   0        0        0     3124 2023-07-05 22:04:01.237112 pydantic_secrets-0.1.1/pydantic_secrets/main.py
+-rw-r--r--   0        0        0      159 2023-07-05 21:37:49.091713 pydantic_secrets-0.1.1/pydantic_secrets/protocols.py
+-rw-r--r--   0        0        0       18 2023-07-05 22:04:56.764868 pydantic_secrets-0.1.1/pydantic_secrets/version.py
+-rw-r--r--   0        0        0      612 2023-07-05 21:27:12.936373 pydantic_secrets-0.1.1/pydantic_secrets/warnings.py
+-rw-r--r--   0        0        0      716 2023-07-05 22:04:52.544884 pydantic_secrets-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      537 1970-01-01 00:00:00.000000 pydantic_secrets-0.1.1/PKG-INFO
```

### Comparing `pydantic_secrets-0.1.0/LICENSE` & `pydantic_secrets-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_secrets-0.1.0/pydantic_secrets/main.py` & `pydantic_secrets-0.1.1/pydantic_secrets/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,68 +1,79 @@
-import typing as t
 import os
-from pydantic import Field, BaseModel
-from pydantic.v1.env_settings import SettingsSourceCallable
-from pydantic_settings import BaseSettings
+import typing as t
+import warnings
+from typing import Any
+
+from pydantic import BaseModel
+from pydantic.fields import FieldInfo
+from pydantic_settings import BaseSettings, PydanticBaseSettingsSource
+
+from pydantic_secrets.protocols import SecretManagerClientProtocol
 
-from pydantic_secrets.protocols import SecretManagerProtocol
+from .warnings import SecretReceivingWarning, SecretVersionNotSpecifiedWarning
 
+EXTRA_SECRET_NAME_KEY = "secret_name"
+ENV_SECRET_NAME_KEY = "secret_name_env"
+EXTRA_SECRET_VERSION_KEY = "secret_version"
+ENV_SECRET_VERSION_KEY = "secret_version_env"
 
-class SecretManagerConfig:
 
-    __secret_manager__: SecretManagerProtocol
+class SecretManagerSource(PydanticBaseSettingsSource):
+    def __init__(
+        self,
+        settings_cls: type[BaseSettings],
+        secret_manager_client: SecretManagerClientProtocol,
+        default_secret_version: str | None = None,
+    ):
+        super().__init__(settings_cls)
+        self.__secret_manager__ = secret_manager_client
+        self.__default_secret_version__ = default_secret_version
+
+    def get_field_value(
+        self, field: FieldInfo, field_name: str
+    ) -> tuple[Any, str, bool]:
+        return field_name, field.default, self.field_is_complex(field)
+
+    def __call__(self) -> dict[str, Any]:
+        return self._process_fields(self.settings_cls.model_fields)
 
-    @classmethod
     def _get_secret_info_from_extra(
-        cls, extra: dict[str, t.Any]
+        self,
+        extra: dict[str, t.Any],
     ) -> tuple[str | None, str | None]:
-        secret_name = extra.get("secret_name")
-        secret_name_env = extra.get("secret_name_env")
+        secret_name = extra.get(EXTRA_SECRET_NAME_KEY)
+        secret_name_env = extra.get(ENV_SECRET_NAME_KEY)
         if secret_name_env:
             secret_name = os.getenv(secret_name_env) or secret_name
-        secret_version = extra.get("secret_version")
-        secret_version_env = extra.get("secret_version_env")
+        secret_version = extra.get(EXTRA_SECRET_VERSION_KEY)
+        secret_version_env = extra.get(ENV_SECRET_VERSION_KEY)
         if secret_version_env:
             secret_version = os.getenv(secret_version_env) or secret_version
-        secret_version = secret_version or "latest"
+        secret_version = secret_version or self.__default_secret_version__
         return secret_name, secret_version
 
-    @classmethod
-    def _process_fields(cls, fields: dict[str, Field]):
+    def _process_fields(self, fields: dict[str, FieldInfo]):
         d: dict[str, t.Any] = {}
         for field_name, field in fields.items():
-            if field.is_complex():
-                if issubclass(field.type_, BaseModel):
-                    d[field_name] = cls._process_fields(field.type_.model_fields)
+            if self.field_is_complex(field):
+                if field.annotation and issubclass(field.annotation, BaseModel):
+                    d[field_name] = self._process_fields(field.annotation.model_fields)
                     continue
                 d[field_name] = field
                 continue
-            secret_name, secret_version = cls._get_secret_info_from_extra(
-                field.field_info.extra
+            secret_name, secret_version = (
+                self._get_secret_info_from_extra(field.json_schema_extra)
+                if field.json_schema_extra
+                else (None, None)
             )
             if secret_name and secret_version:
                 try:
-                    d[field_name] = cls.__secret_manager__.get_secret(
+                    d[field_name] = self.__secret_manager__.get_secret(
                         secret_name=secret_name,
                         secret_version=secret_version,
                     )
                 except Exception:
+                    warnings.warn(field_name, category=SecretReceivingWarning)
                     pass
+            elif secret_name and not secret_version:
+                warnings.warn(field_name, category=SecretVersionNotSpecifiedWarning)
         return d
-
-    @classmethod
-    def get_secrets(cls, settings: BaseSettings) -> dict[str, str]:
-        return cls._process_fields(settings.model_fields)
-
-    @classmethod
-    def customise_sources(
-        cls,
-        init_settings: SettingsSourceCallable,
-        env_settings: SettingsSourceCallable,
-        file_secret_settings: SettingsSourceCallable,
-    ):
-        return (
-            init_settings,
-            env_settings,
-            file_secret_settings,
-            cls.get_secrets,
-        )
```

### Comparing `pydantic_secrets-0.1.0/PKG-INFO` & `pydantic_secrets-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-secrets
-Version: 0.1.0
+Version: 0.1.1
 Summary: The library is designed for extending your BaseSettings config class to load secrets from a secret manager
 License: MIT
 Author: Dmitry Marchuk
 Author-email: marchuk.d13@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

