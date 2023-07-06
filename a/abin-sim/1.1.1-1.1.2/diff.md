# Comparing `tmp/abin_sim-1.1.1.tar.gz` & `tmp/abin_sim-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abin_sim-1.1.1.tar", max compression
+gzip compressed data, was "abin_sim-1.1.2.tar", max compression
```

## Comparing `abin_sim-1.1.1.tar` & `abin_sim-1.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      260 2023-07-03 20:07:56.409411 abin_sim-1.1.1/LICENSE
--rw-r--r--   0        0        0     8594 2023-07-03 20:07:56.409411 abin_sim-1.1.1/README.md
--rw-r--r--   0        0        0       21 2023-07-03 20:07:56.409411 abin_sim-1.1.1/abin_sim/__init__.py
--rw-r--r--   0        0        0     8435 2023-07-03 20:07:56.409411 abin_sim-1.1.1/abin_sim/cli.py
--rw-r--r--   0        0        0      194 2023-07-03 20:07:56.409411 abin_sim-1.1.1/abin_sim/config.py
--rw-r--r--   0        0        0     1174 2023-07-03 20:07:56.409411 abin_sim-1.1.1/abin_sim/core/file_manager.py
--rw-r--r--   0        0        0     5320 2023-07-03 20:07:56.409411 abin_sim-1.1.1/abin_sim/core/functions.py
--rw-r--r--   0        0        0     1190 2023-07-03 20:07:56.409411 abin_sim-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     9483 1970-01-01 00:00:00.000000 abin_sim-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      260 2023-07-05 14:09:06.428831 abin_sim-1.1.2/LICENSE
+-rw-r--r--   0        0        0     8594 2023-07-05 14:09:06.428831 abin_sim-1.1.2/README.md
+-rw-r--r--   0        0        0       21 2023-07-05 14:09:06.428831 abin_sim-1.1.2/abin_sim/__init__.py
+-rw-r--r--   0        0        0     8435 2023-07-05 14:09:06.428831 abin_sim-1.1.2/abin_sim/cli.py
+-rw-r--r--   0        0        0      194 2023-07-05 14:09:06.428831 abin_sim-1.1.2/abin_sim/config.py
+-rw-r--r--   0        0        0     1174 2023-07-05 14:09:06.428831 abin_sim-1.1.2/abin_sim/core/file_manager.py
+-rw-r--r--   0        0        0     5745 2023-07-05 14:09:06.428831 abin_sim-1.1.2/abin_sim/core/functions.py
+-rw-r--r--   0        0        0     1190 2023-07-05 14:09:06.432831 abin_sim-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     9483 1970-01-01 00:00:00.000000 abin_sim-1.1.2/PKG-INFO
```

### Comparing `abin_sim-1.1.1/README.md` & `abin_sim-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `abin_sim-1.1.1/abin_sim/cli.py` & `abin_sim-1.1.2/abin_sim/cli.py`

 * *Files identical despite different names*

### Comparing `abin_sim-1.1.1/abin_sim/core/file_manager.py` & `abin_sim-1.1.2/abin_sim/core/file_manager.py`

 * *Files identical despite different names*

### Comparing `abin_sim-1.1.1/abin_sim/core/functions.py` & `abin_sim-1.1.2/abin_sim/core/functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,14 +71,22 @@
         for i, x in enumerate(v.split('$')[1:]):
             key = re.findall(r'\w+', x)[0]
             v = v.replace('$' + key, contentDict[key])
         contentDict[k] = v.strip()
 
     return json.dumps(contentDict)
 
+def replace_string(secret, search, replace):
+    with open(secret, 'rt') as file_in:
+        novo_arquivo = file_in.read()
+
+    with open(secret, 'wt') as file_out:
+        novo_arquivo = novo_arquivo.replace(search, replace)
+        file_out.write(novo_arquivo)
+
 def update_secret(
     app: str,
     env: str,
     proj: str,
     secret: str,
     token: str,
     vault_url: str,
@@ -94,15 +102,17 @@
             try:
                 ret = requests.request(
                     'POST', url=vault_url + f'/v1/{env}-{proj}/data/{app}/{secret}', headers=headers, data=payload
                 )
             except Exception as e:
                 return {'Status': e}
             json_file.unlink()
-        case _:            
+        case _:
+            if secret == 'env.js':
+                replace_string(file, '\"', '\\\"')
             with open(file, 'r') as f:
                 content = f.readlines()
             converted = ''
             # contentList = [x.strip().split('#')[0].split('=', 1) for x in content if '=' in x.split('#')[0]]
             for line in content:
                 if converted == '':
                     converted = f'{line}'.strip()+'\\n'
@@ -118,14 +128,17 @@
                 ret = requests.request(
                     'POST', url=vault_url + f'/v1/{env}-{proj}/data/{app}/{secret}', headers=headers, data=payload
                 )
             except Exception as e:
                 return {'Status': e}
             json_file.unlink()
 
+            if secret == 'env.js':
+                replace_string(file, '\\\"', '\"')
+
     if ret.status_code == 200:
         return {'Status': 'Success'}
     else:
         return {'Status': (ret.text)}
 
 def make_conf() -> dict:
     home_dir = environ['HOME']
```

### Comparing `abin_sim-1.1.1/pyproject.toml` & `abin_sim-1.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "abin-sim"
-version = "1.1.1"
+version = "1.1.2"
 description = "ABIN é um CLI para interagir com a API do Vault e auxiliar os Desenvolvedores nos projetos da SIMTech"
 license = "BeerWare"
 authors = ["Bonatto <andrebonatto@gmail.com>"]
 readme = "README.md"
 packages = [{include = "abin_sim"}]
 classifiers = [
     "Topic :: Utilities",
```

### Comparing `abin_sim-1.1.1/PKG-INFO` & `abin_sim-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abin-sim
-Version: 1.1.1
+Version: 1.1.2
 Summary: ABIN é um CLI para interagir com a API do Vault e auxiliar os Desenvolvedores nos projetos da SIMTech
 License: Beerware
 Author: Bonatto
 Author-email: andrebonatto@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

