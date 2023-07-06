# Comparing `tmp/mnnllzz-1.4.2.tar.gz` & `tmp/mnnllzz-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnnllzz-1.4.2.tar", last modified: Thu Apr 13 07:41:42 2023, max compression
+gzip compressed data, was "mnnllzz-1.4.3.tar", last modified: Thu Jul  6 10:04:07 2023, max compression
```

## Comparing `mnnllzz-1.4.2.tar` & `mnnllzz-1.4.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
-drwxr-xr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 07:41:42.013728 mnnllzz-1.4.2/
--rw-r--r--   0 andrea    (1000) andrea    (1000)      391 2023-04-13 07:41:42.013728 mnnllzz-1.4.2/PKG-INFO
-drwxr-xr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 07:41:42.012730 mnnllzz-1.4.2/mnnllzz/
--rw-r--r--   0 andrea    (1000) andrea    (1000)        0 2022-02-07 08:57:12.000000 mnnllzz-1.4.2/mnnllzz/__init__.py
--rw-r--r--   0 andrea    (1000) andrea    (1000)      537 2023-02-20 17:34:38.000000 mnnllzz-1.4.2/mnnllzz/__main__.py
--rw-r--r--   0 andrea    (1000) andrea    (1000)    24950 2023-04-13 07:22:25.556788 mnnllzz-1.4.2/mnnllzz/mnnllzz.py
--rw-r--r--   0 andrea    (1000) andrea    (1000)       42 2022-02-14 09:41:48.000000 mnnllzz-1.4.2/setup.cfg
--rw-r--r--   0 andrea    (1000) andrea    (1000)      450 2023-04-13 07:39:49.219107 mnnllzz-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 10:04:07.138214 mnnllzz-1.4.3/
+-rw-rw-rw-   0        0        0      405 2023-07-06 10:04:07.138214 mnnllzz-1.4.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-06 10:04:07.138214 mnnllzz-1.4.3/mnnllzz/
+-rw-rw-rw-   0        0        0        0 2022-02-07 08:57:12.000000 mnnllzz-1.4.3/mnnllzz/__init__.py
+-rw-rw-rw-   0        0        0      537 2023-02-20 17:34:38.000000 mnnllzz-1.4.3/mnnllzz/__main__.py
+-rw-rw-rw-   0        0        0    25012 2023-06-19 06:36:33.000000 mnnllzz-1.4.3/mnnllzz/mnnllzz.py
+-rw-rw-rw-   0        0        0       42 2022-02-14 09:41:48.000000 mnnllzz-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      450 2023-07-06 10:03:19.288242 mnnllzz-1.4.3/setup.py
```

### Comparing `mnnllzz-1.4.2/mnnllzz/__main__.py` & `mnnllzz-1.4.3/mnnllzz/__main__.py`

 * *Files identical despite different names*

### Comparing `mnnllzz-1.4.2/mnnllzz/mnnllzz.py` & `mnnllzz-1.4.3/mnnllzz/mnnllzz.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
                  solutions,
                  test_name, year, month, day,
                  salt_1, salt_2,
                  mark_sol=False):
         # A string containing the whole TeX template.
         self.source_text = template_text
         # The number of this test.
-        self.testnr = testnr
+        self.testnr = int(testnr)
         # List of lists of dictionaries with the solutions.
         self.solutions = solutions
         # Name of the test.  Some checks on the format.
         ww = test_name.replace("_", " ").split()  # from underscore to spaces
         for iw,w in enumerate(ww):
             if (len(w) > 3):    # capitalize first letter of long words
                 ww[iw] = w[0].upper() + w[1:]
@@ -53,16 +53,18 @@
         # The date.
         self.test_year = year
         self.test_month = month
         self.test_day = day
         # Whether to mark correct solutions.
         self.mark_sol = mark_sol
         # Set seeds for the random numbers based on the test number.
-        random.seed(salt_1 * (testnr + 1))  # for the letters
-        np.random.seed(salt_2 * (testnr + 1))   # for the values
+        seed_1 = int(salt_1 * (testnr + 1))
+        seed_2 = int(salt_2 * (testnr + 1))
+        random.seed(seed_1)  # for the letters
+        np.random.seed(seed_2)  # for the values
         # Constant: uppercase alphabet.
         self._letters = string.ascii_uppercase
         # Mathematical functions for the evaluation of formulas.
         self.mfe = {
             "sqrt": np.sqrt, "exp": np.exp, "sin": np.sin, "cos": np.cos,
             "tan": np.tan, "log": np.log, "log10": np.log10, "pi": np.pi,
             "floor": np.floor, "ceil": np.ceil, "round": np.round, "abs": np.abs,
```

