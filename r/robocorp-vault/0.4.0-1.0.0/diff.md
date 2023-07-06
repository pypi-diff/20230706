# Comparing `tmp/robocorp_vault-0.4.0.tar.gz` & `tmp/robocorp_vault-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_vault-0.4.0.tar", max compression
+gzip compressed data, was "robocorp_vault-1.0.0.tar", max compression
```

## Comparing `robocorp_vault-0.4.0.tar` & `robocorp_vault-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      523 2023-06-14 16:04:59.522158 robocorp_vault-0.4.0/README.md
--rw-r--r--   0        0        0      710 2023-06-14 16:04:59.526157 robocorp_vault-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4076 2023-06-14 16:04:59.526157 robocorp_vault-0.4.0/src/robocorp/vault/__init__.py
--rw-r--r--   0        0        0      112 2023-06-14 16:04:59.526157 robocorp_vault-0.4.0/src/robocorp/vault/_errors.py
--rw-r--r--   0        0        0     1587 2023-06-14 16:04:59.526157 robocorp_vault-0.4.0/src/robocorp/vault/_secrets.py
--rw-r--r--   0        0        0     1858 2023-06-14 16:04:59.526157 robocorp_vault-0.4.0/src/robocorp/vault/_utils.py
--rw-r--r--   0        0        0    18337 2023-06-14 16:04:59.526157 robocorp_vault-0.4.0/src/robocorp/vault/_vault.py
--rw-r--r--   0        0        0        0 2023-06-14 16:04:59.526157 robocorp_vault-0.4.0/src/robocorp/vault/py.typed
--rw-r--r--   0        0        0     1082 1970-01-01 00:00:00.000000 robocorp_vault-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1194 2023-07-06 17:44:26.187811 robocorp_vault-1.0.0/README.md
+-rw-r--r--   0        0        0      782 2023-07-06 17:44:26.187811 robocorp_vault-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5351 2023-07-06 17:44:26.187811 robocorp_vault-1.0.0/src/robocorp/vault/__init__.py
+-rw-r--r--   0        0        0      112 2023-07-06 17:44:26.187811 robocorp_vault-1.0.0/src/robocorp/vault/_errors.py
+-rw-r--r--   0        0        0     1587 2023-07-06 17:44:26.187811 robocorp_vault-1.0.0/src/robocorp/vault/_secrets.py
+-rw-r--r--   0        0        0     1858 2023-07-06 17:44:26.187811 robocorp_vault-1.0.0/src/robocorp/vault/_utils.py
+-rw-r--r--   0        0        0    18022 2023-07-06 17:44:26.187811 robocorp_vault-1.0.0/src/robocorp/vault/_vault.py
+-rw-r--r--   0        0        0        0 2023-07-06 17:44:26.187811 robocorp_vault-1.0.0/src/robocorp/vault/py.typed
+-rw-r--r--   0        0        0     1940 1970-01-01 00:00:00.000000 robocorp_vault-1.0.0/PKG-INFO
```

### Comparing `robocorp_vault-0.4.0/pyproject.toml` & `robocorp_vault-1.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 [tool.poetry]
 name = "robocorp-vault"
-version = "0.4.0"
+version = "1.0.0"
 description = "Robocorp Control Room Vault API integration library"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 	"Ossi R. <ossi@robocorp.com>",
 ]
 readme = "README.md"
+repository = "https://github.com/robocorp/robo/"
+license = "Apache-2.0"
 packages = [{include = "robocorp", from="src"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 cryptography = "^41.0.1"
 requests = "^2.31"
 pyyaml = "^6.0"
```

### Comparing `robocorp_vault-0.4.0/src/robocorp/vault/__init__.py` & `robocorp_vault-1.0.0/src/robocorp/vault/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -60,19 +60,20 @@
     secret = vault.get_secret("swaglabs")
     secret["username"] = "nobody"
     vault.set_secret(secret)
 ```
 """  # noqa: E501
 
 
+from contextlib import nullcontext
 from functools import lru_cache
 
 from ._secrets import SecretContainer
 
-__version__ = "0.4.0"
+__version__ = "1.0.0"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 @lru_cache
 def _get_vault():
     from ._vault import Vault
 
@@ -85,59 +86,99 @@
     Args:
         secret_name: Name of secret to fetch.
 
     Note:
         The returned secret is not cached, so, calling this function again
         may do a new network roundtrip.
 
+    Note:
+        When used, if `robocorp.log` is in the environment, all the values
+        gotten will be automatically hidden from the logs.
+        i.e.: For each value, `log.hide_from_output(value)` will be called.
+
     Returns:
         The container for the secret (which has key-value pairs).
 
     Raises:
         RobocorpVaultError: Error with API request or response payload.
     """
-    vault = _get_vault()
-
-    # Note: secrets are always gotten from the backend when requested
-    # (so any updates will be gotten in a new `get_secret` call).
-    secret = vault.get_secret(secret_name)
-
     try:
         from robocorp import log  # type: ignore [attr-defined]
+
+        ctx = log.suppress_variables()
+        has_log = True
     except ImportError:
         pass  # If robocorp.log is not being used that's OK.
-    else:
-        # There's no caching in place, so, on any new call it's possible
-        # that values changed, so, call this every time.
-        for value in secret.values():
-            log.hide_from_output(str(value))
+        ctx = nullcontext()
+        has_log = False
+
+    with ctx:
+        vault = _get_vault()
+
+        # Note: secrets are always gotten from the backend when requested
+        # (so any updates will be gotten in a new `get_secret` call).
+        secret = vault.get_secret(secret_name)
+
+        if has_log:
+            # There's no caching in place, so, on any new call it's possible
+            # that values changed, so, call this every time.
+            _ignore_secret_values(secret)
 
     return secret
 
 
 def set_secret(secret: SecretContainer) -> None:
     """Overwrite an existing secret with new values.
 
     Note:
         Only allows modifying existing secrets, and replaces
           all values contained within it.
 
+    Note:
+        When used, if `robocorp.log` is in the environment, all the values
+        set will be automatically hidden from the logs.
+        i.e.: For each value, `log.hide_from_output(value)` will be called.
+
     Args:
         secret: the secret object which was mutated.
     """
-    vault = _get_vault()
-    vault.set_secret(secret)
-
     try:
         from robocorp import log  # type: ignore [attr-defined]
+
+        ctx = log.suppress_variables()
+        has_log = True
     except ImportError:
         pass  # If robocorp.log is not being used that's OK.
-    else:
-        # When it's set it's expected that some value was changed, so,
-        # start hiding it from the logs.
-        # Note: users should've actually done that already, but doing
-        # it again is harmless.
-        for value in secret.values():
-            log.hide_from_output(str(value))
+        ctx = nullcontext()
+        has_log = False
+
+    with ctx:
+        vault = _get_vault()
+        vault.set_secret(secret)
+
+        if has_log:
+            # When it's set it's expected that some value was changed, so,
+            # start hiding it from the logs.
+            # Note: users should've actually done that already, but doing
+            # it again is harmless.
+            _ignore_secret_values(secret)
+
+
+def _ignore_secret_values(secret):
+    from robocorp import log
+
+    for value in secret.values():
+        s = str(value)
+        log.hide_from_output(s)
+
+        # Now, also take care of the case where the user does a repr(value)
+        # and not just str(value) as in some places it's the repr(value)
+        # that'll appear in the logs.
+        r = repr(value)
+        if r.startswith("'") and r.endswith("'"):
+            r = r[1:-1]
+        if r != s:
+            log.hide_from_output(r)
+            log.hide_from_output(r.replace("\\", "\\\\"))
 
 
 __all__ = ["get_secret", "set_secret"]
```

### Comparing `robocorp_vault-0.4.0/src/robocorp/vault/_secrets.py` & `robocorp_vault-1.0.0/src/robocorp/vault/_secrets.py`

 * *Files identical despite different names*

### Comparing `robocorp_vault-0.4.0/src/robocorp/vault/_utils.py` & `robocorp_vault-1.0.0/src/robocorp/vault/_utils.py`

 * *Files identical despite different names*

### Comparing `robocorp_vault-0.4.0/src/robocorp/vault/_vault.py` & `robocorp_vault-1.0.0/src/robocorp/vault/_vault.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,35 +98,28 @@
         #  because it is wrong starting from the "env.json" configuration level.
         raise ValueError(
             f"Local vault secrets file extension {extension!r} not supported."
         )
 
     def _load(self):
         """Load secrets file."""
-        try:
-            with open(self.path, encoding="utf-8") as fd:
-                data = self._loader(fd)
+        with open(self.path, encoding="utf-8") as fd:
+            data = self._loader(fd)
 
-            if not isinstance(data, dict):
-                raise ValueError("Invalid content format")
+        if not isinstance(data, dict):
+            raise ValueError("Invalid content format")
 
-            return data
-        except (IOError, ValueError) as err:
-            self.logger.error("Failed to load secrets file: %s", err)
-            return {}
+        return data
 
     def _save(self, data):
         """Save the secrets content to disk."""
-        try:
-            with open(self.path, "w", encoding="utf-8") as f:
-                if not isinstance(data, dict):
-                    raise ValueError("Invalid content format")
-                self._dumper(data, f, indent=4)
-        except (IOError, ValueError) as err:
-            self.logger.error("Failed to _save secrets file: %s", err)
+        with open(self.path, "w", encoding="utf-8") as f:
+            if not isinstance(data, dict):
+                raise ValueError("Invalid content format")
+            self._dumper(data, f, indent=4)
 
     def get_secret(self, secret_name: str) -> SecretContainer:
         """Get secret defined with given name from file.
 
         Args:
             secret_name: Name of secret to fetch
         Returns:
```

