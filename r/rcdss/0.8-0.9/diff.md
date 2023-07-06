# Comparing `tmp/rcdss-0.8.tar.gz` & `tmp/rcdss-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcdss-0.8.tar", last modified: Fri Jun 18 16:23:30 2021, max compression
+gzip compressed data, was "rcdss-0.9.tar", last modified: Thu Jul  6 14:17:43 2023, max compression
```

## Comparing `rcdss-0.8.tar` & `rcdss-0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ocaletka   (502) staff       (20)        0 2021-06-18 16:23:30.189489 rcdss-0.8/
--rw-r--r--   0 ocaletka   (502) staff       (20)     1516 2021-06-07 09:39:28.000000 rcdss-0.8/LICENSE
--rw-r--r--   0 ocaletka   (502) staff       (20)     2475 2021-06-18 16:23:30.189733 rcdss-0.8/PKG-INFO
--rw-r--r--   0 ocaletka   (502) staff       (20)     1828 2021-06-18 14:58:17.000000 rcdss-0.8/README.md
-drwxr-xr-x   0 ocaletka   (502) staff       (20)        0 2021-06-18 16:23:30.177690 rcdss-0.8/rcdss/
--rw-r--r--   0 ocaletka   (502) staff       (20)       48 2021-06-18 16:19:26.000000 rcdss-0.8/rcdss/__init__.py
--rw-r--r--   0 ocaletka   (502) staff       (20)     3535 2021-06-18 14:59:55.000000 rcdss-0.8/rcdss/__main__.py
--rw-r--r--   0 ocaletka   (502) staff       (20)     7602 2021-06-18 15:00:51.000000 rcdss-0.8/rcdss/dsscanner.py
--rw-r--r--   0 ocaletka   (502) staff       (20)      619 2021-04-28 20:45:10.000000 rcdss-0.8/rcdss/log.py
--rw-r--r--   0 ocaletka   (502) staff       (20)     1879 2021-01-13 14:14:01.000000 rcdss-0.8/rcdss/rpsl.py
--rw-r--r--   0 ocaletka   (502) staff       (20)     1226 2021-04-07 11:41:51.000000 rcdss-0.8/rcdss/stats.py
-drwxr-xr-x   0 ocaletka   (502) staff       (20)        0 2021-06-18 16:23:30.186804 rcdss-0.8/rcdss.egg-info/
--rw-r--r--   0 ocaletka   (502) staff       (20)     2475 2021-06-18 16:23:30.000000 rcdss-0.8/rcdss.egg-info/PKG-INFO
--rw-r--r--   0 ocaletka   (502) staff       (20)      309 2021-06-18 16:23:30.000000 rcdss-0.8/rcdss.egg-info/SOURCES.txt
--rw-r--r--   0 ocaletka   (502) staff       (20)        1 2021-06-18 16:23:30.000000 rcdss-0.8/rcdss.egg-info/dependency_links.txt
--rw-r--r--   0 ocaletka   (502) staff       (20)       47 2021-06-18 16:23:30.000000 rcdss-0.8/rcdss.egg-info/entry_points.txt
--rw-r--r--   0 ocaletka   (502) staff       (20)       29 2021-06-18 16:23:30.000000 rcdss-0.8/rcdss.egg-info/requires.txt
--rw-r--r--   0 ocaletka   (502) staff       (20)        6 2021-06-18 16:23:30.000000 rcdss-0.8/rcdss.egg-info/top_level.txt
--rw-r--r--   0 ocaletka   (502) staff       (20)       63 2021-06-18 16:23:30.190629 rcdss-0.8/setup.cfg
--rw-r--r--   0 ocaletka   (502) staff       (20)     1084 2021-06-08 14:01:32.000000 rcdss-0.8/setup.py
+drwxr-xr-x   0 ocaletka   (502) staff       (20)        0 2023-07-06 14:17:43.020586 rcdss-0.9/
+-rw-r--r--   0 ocaletka   (502) staff       (20)     1516 2021-06-07 09:39:28.000000 rcdss-0.9/LICENSE
+-rw-r--r--   0 ocaletka   (502) staff       (20)     2438 2023-07-06 14:17:43.020866 rcdss-0.9/PKG-INFO
+-rw-r--r--   0 ocaletka   (502) staff       (20)     1828 2021-06-18 14:58:17.000000 rcdss-0.9/README.md
+drwxr-xr-x   0 ocaletka   (502) staff       (20)        0 2023-07-06 14:17:43.014713 rcdss-0.9/rcdss/
+-rw-r--r--   0 ocaletka   (502) staff       (20)       48 2023-06-30 13:43:21.000000 rcdss-0.9/rcdss/__init__.py
+-rw-r--r--   0 ocaletka   (502) staff       (20)     3535 2021-06-18 14:59:55.000000 rcdss-0.9/rcdss/__main__.py
+-rw-r--r--   0 ocaletka   (502) staff       (20)     8144 2023-06-30 13:43:21.000000 rcdss-0.9/rcdss/dsscanner.py
+-rw-r--r--   0 ocaletka   (502) staff       (20)      619 2021-04-28 20:45:10.000000 rcdss-0.9/rcdss/log.py
+-rw-r--r--   0 ocaletka   (502) staff       (20)     1879 2021-01-13 14:14:01.000000 rcdss-0.9/rcdss/rpsl.py
+-rw-r--r--   0 ocaletka   (502) staff       (20)     1226 2021-04-07 11:41:51.000000 rcdss-0.9/rcdss/stats.py
+drwxr-xr-x   0 ocaletka   (502) staff       (20)        0 2023-07-06 14:17:43.020049 rcdss-0.9/rcdss.egg-info/
+-rw-r--r--   0 ocaletka   (502) staff       (20)     2438 2023-07-06 14:17:42.000000 rcdss-0.9/rcdss.egg-info/PKG-INFO
+-rw-r--r--   0 ocaletka   (502) staff       (20)      309 2023-07-06 14:17:42.000000 rcdss-0.9/rcdss.egg-info/SOURCES.txt
+-rw-r--r--   0 ocaletka   (502) staff       (20)        1 2023-07-06 14:17:42.000000 rcdss-0.9/rcdss.egg-info/dependency_links.txt
+-rw-r--r--   0 ocaletka   (502) staff       (20)       46 2023-07-06 14:17:42.000000 rcdss-0.9/rcdss.egg-info/entry_points.txt
+-rw-r--r--   0 ocaletka   (502) staff       (20)       36 2023-07-06 14:17:42.000000 rcdss-0.9/rcdss.egg-info/requires.txt
+-rw-r--r--   0 ocaletka   (502) staff       (20)        6 2023-07-06 14:17:42.000000 rcdss-0.9/rcdss.egg-info/top_level.txt
+-rw-r--r--   0 ocaletka   (502) staff       (20)       63 2023-07-06 14:17:43.022744 rcdss-0.9/setup.cfg
+-rw-r--r--   0 ocaletka   (502) staff       (20)     1091 2023-06-30 13:43:21.000000 rcdss-0.9/setup.py
```

### Comparing `rcdss-0.8/LICENSE` & `rcdss-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rcdss-0.8/PKG-INFO` & `rcdss-0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: rcdss
-Version: 0.8
+Version: 0.9
 Summary: RIPE NCC CDS Scanner
 Home-page: https://github.com/ripe-ncc/rcdss
 Author: Ondřej Caletka
 Author-email: ondrej.caletka@ripe.net
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: System :: Systems Administration
@@ -58,9 +56,7 @@
 preferably into its own
 [`virtualenv`](https://docs.python.org/3/tutorial/venv.html).
 
     $ python3 -m venv rcdss-venv
     $ source rcdss-venv/bin/activate
     (rcdss-venv)$ pip install rcdss
     (rcdss-venv)$ rcdss --help
-
-
```

### Comparing `rcdss-0.8/README.md` & `rcdss-0.9/README.md`

 * *Files identical despite different names*

### Comparing `rcdss-0.8/rcdss/__main__.py` & `rcdss-0.9/rcdss/__main__.py`

 * *Files identical despite different names*

### Comparing `rcdss-0.8/rcdss/dsscanner.py` & `rcdss-0.9/rcdss/dsscanner.py`

 * *Files 8% similar despite different names*

```diff
@@ -152,63 +152,75 @@
     return inception > lm
 
 
 def filter_dnskey_set(dnskeyset, dsset):
     """
     Return a set of DNSKEYs with only keys
     matching fingerprints in the dsset.
+    We allow any supported DS record type,
+    even those deprecated by RFC 8624
     """
     s = set()
     for dnskey in dnskeyset:
         key_id = dns.dnssec.key_id(dnskey)
         for ds in dsset:
             if ds.key_tag != key_id:
                 continue
             try:
                 if ds == dns.dnssec.make_ds(
                     dnskeyset.name,
                     dnskey,
                     ds.digest_type,
+                    policy=dns.dnssec.allow_all_policy,
                 ):
                     s.add(dnskey)
             except dns.dnssec.UnsupportedAlgorithm:
                 pass
+            except dns.dnssec.DeniedByPolicy:
+                pass
     return s
 
 
 def check_signed_by_KSK(cds, ds_rdataset, dnskeyset):
     """
     Check if the CDS is actually signed by a key contained in the
     current DS RRSET as per RFC 7344 section 4.1
+
+    We use RFC 8624 policy to ignore deprecated algorithms.
     """
     dsset = {
         dns.rdata.from_text(
             dns.rdataclass.IN, dns.rdatatype.DS,
             rdata,
         ) for rdata in ds_rdataset
     }
     keyset = filter_dnskey_set(dnskeyset, dsset)
     try:
         dns.dnssec.validate(
             cds.rrset,
             get_rrsigset(cds.response),
             {cds.name: keyset},
+            policy=dns.dnssec.rfc_8624_policy,
         )
         return True
     except dns.dnssec.ValidationFailure:
         return False
+    except dns.dnssec.DeniedByPolicy:
+        return False
 
 
 def check_CDS_continuity(cds, dnskeyset):
     """
     Check if the CDS, when applied, will not break the current delegation
     as per RFC 7344 section 4.1
 
     In a nutshell this means that at least one of the CDS rdata must be
     used to sign zone's DNSKEY record for each signature algorithm present.
+
+    We use RFC 8624 policy to ignore deprecated algorithms.
     """
     dssets = defaultdict(set)
     for ds in (
         dns.rdata.from_text(
             dns.rdataclass.IN,
             dns.rdatatype.DS,
             rdata.to_text(),
@@ -222,11 +234,14 @@
                 dns.dnssec.algorithm_to_text(alg),
             )
             keyset = filter_dnskey_set(dnskeyset, dsset)
             dns.dnssec.validate(
                 dnskeyset.rrset,
                 get_rrsigset(dnskeyset.response),
                 {cds.name: keyset},
+                policy=dns.dnssec.rfc_8624_policy,
             )
         return True
     except dns.dnssec.ValidationFailure:
         return False
+    except dns.dnssec.DeniedByPolicy:
+        return False
```

### Comparing `rcdss-0.8/rcdss/log.py` & `rcdss-0.9/rcdss/log.py`

 * *Files identical despite different names*

### Comparing `rcdss-0.8/rcdss/rpsl.py` & `rcdss-0.9/rcdss/rpsl.py`

 * *Files identical despite different names*

### Comparing `rcdss-0.8/rcdss/stats.py` & `rcdss-0.9/rcdss/stats.py`

 * *Files identical despite different names*

### Comparing `rcdss-0.8/rcdss.egg-info/PKG-INFO` & `rcdss-0.9/rcdss.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: rcdss
-Version: 0.8
+Version: 0.9
 Summary: RIPE NCC CDS Scanner
 Home-page: https://github.com/ripe-ncc/rcdss
 Author: Ondřej Caletka
 Author-email: ondrej.caletka@ripe.net
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: System :: Systems Administration
@@ -58,9 +56,7 @@
 preferably into its own
 [`virtualenv`](https://docs.python.org/3/tutorial/venv.html).
 
     $ python3 -m venv rcdss-venv
     $ source rcdss-venv/bin/activate
     (rcdss-venv)$ pip install rcdss
     (rcdss-venv)$ rcdss --help
-
-
```

### Comparing `rcdss-0.8/setup.py` & `rcdss-0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     long_description_content_type="text/markdown",
     url="https://github.com/ripe-ncc/rcdss",
     author="Ondřej Caletka",
     author_email="ondrej.caletka@ripe.net",
     packages=["rcdss"],
     setup_requires=["pytest-runner"],
     python_requires=">=3.6",
-    install_requires=["dnspython", "cryptography", "click"],
+    install_requires=["dnspython>=2.3.0", "cryptography", "click"],
     tests_require=["pytest"],
     entry_points={
         "console_scripts": [
             "rcdss = rcdss.__main__:main",
         ],
     },
     classifiers=[
```

