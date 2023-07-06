# Comparing `tmp/pyproject_api-1.5.2.tar.gz` & `tmp/pyproject_api-1.5.3.tar.gz`

## Comparing `pyproject_api-1.5.2.tar` & `pyproject_api-1.5.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/.readthedocs.yml
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/tox.ini
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/.github/dependabot.yml
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/.github/workflows/check.yml
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/.github/workflows/release.yml
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/docs/changelog.rst
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/docs/conf.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/docs/index.rst
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/src/pyproject_api/__init__.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/src/pyproject_api/__main__.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/src/pyproject_api/_backend.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/src/pyproject_api/_backend.pyi
--rw-r--r--   0        0        0    21148 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/src/pyproject_api/_frontend.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/src/pyproject_api/_util.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/src/pyproject_api/_version.py
--rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/src/pyproject_api/_via_fresh_subprocess.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/src/pyproject_api/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/tests/_build_sdist.py
--rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/tests/test_backend.py
--rw-r--r--   0        0        0    13891 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/tests/test_frontend.py
--rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/tests/test_frontend_setuptools.py
--rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/tests/test_main.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/tests/test_util.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/tests/test_version.py
--rw-r--r--   0        0        0     4526 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/tests/demo_pkg_inline/build.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/tests/demo_pkg_inline/pyproject.toml
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/.gitignore
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/LICENSE
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/README.md
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 pyproject_api-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 pyproject_api-1.5.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 pyproject_api-1.5.3/.readthedocs.yml
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 pyproject_api-1.5.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 pyproject_api-1.5.3/tox.ini
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pyproject_api-1.5.3/.github/dependabot.yml
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 pyproject_api-1.5.3/.github/workflows/check.yml
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 pyproject_api-1.5.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 pyproject_api-1.5.3/docs/changelog.rst
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 pyproject_api-1.5.3/docs/conf.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 pyproject_api-1.5.3/docs/index.rst
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 pyproject_api-1.5.3/src/pyproject_api/__init__.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 pyproject_api-1.5.3/src/pyproject_api/__main__.py
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 pyproject_api-1.5.3/src/pyproject_api/_backend.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 pyproject_api-1.5.3/src/pyproject_api/_backend.pyi
+-rw-r--r--   0        0        0    21148 2020-02-02 00:00:00.000000 pyproject_api-1.5.3/src/pyproject_api/_frontend.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 pyproject_api-1.5.3/src/pyproject_api/_util.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pyproject_api-1.5.3/src/pyproject_api/_version.py
+-rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 pyproject_api-1.5.3/src/pyproject_api/_via_fresh_subprocess.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_api-1.5.3/src/pyproject_api/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_api-1.5.3/tests/_build_sdist.py
+-rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 pyproject_api-1.5.3/tests/test_backend.py
+-rw-r--r--   0        0        0    13891 2020-02-02 00:00:00.000000 pyproject_api-1.5.3/tests/test_frontend.py
+-rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 pyproject_api-1.5.3/tests/test_frontend_setuptools.py
+-rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 pyproject_api-1.5.3/tests/test_main.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 pyproject_api-1.5.3/tests/test_util.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 pyproject_api-1.5.3/tests/test_version.py
+-rw-r--r--   0        0        0     4526 2020-02-02 00:00:00.000000 pyproject_api-1.5.3/tests/demo_pkg_inline/build.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 pyproject_api-1.5.3/tests/demo_pkg_inline/pyproject.toml
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pyproject_api-1.5.3/.gitignore
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pyproject_api-1.5.3/LICENSE
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 pyproject_api-1.5.3/README.md
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 pyproject_api-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 pyproject_api-1.5.3/PKG-INFO
```

### Comparing `pyproject_api-1.5.2/.pre-commit-config.yaml` & `pyproject_api-1.5.3/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.0.272"
+    rev: "v0.0.275"
     hooks:
       - id: ruff
         exclude: src/pyproject_api/_backend.py
         args: [--fix, --exit-non-zero-on-fix]
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/tox-dev/tox-ini-fmt
-    rev: "1.3.0"
+    rev: "1.3.1"
     hooks:
       - id: tox-ini-fmt
         args: ["-p", "fix"]
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: "0.11.2"
+    rev: "0.12.1"
     hooks:
       - id: pyproject-fmt
         additional_dependencies: ["tox>=4.6"]
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v3.0.0-alpha.9-for-vscode"
     hooks:
       - id: prettier
```

### Comparing `pyproject_api-1.5.2/CODE_OF_CONDUCT.md` & `pyproject_api-1.5.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyproject_api-1.5.2/tox.ini` & `pyproject_api-1.5.3/tox.ini`

 * *Files identical despite different names*

### Comparing `pyproject_api-1.5.2/.github/workflows/check.yml` & `pyproject_api-1.5.3/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `pyproject_api-1.5.2/.github/workflows/release.yml` & `pyproject_api-1.5.3/.github/workflows/release.yml`

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,8 @@
         run: python -m pip install build
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: Build package
         run: pyproject-build -s -w . -o dist
       - name: Publish to PyPI
-        uses: pypa/gh-action-pypi-publish@v1.8.6
+        uses: pypa/gh-action-pypi-publish@v1.8.7
```

### Comparing `pyproject_api-1.5.2/docs/changelog.rst` & `pyproject_api-1.5.3/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `pyproject_api-1.5.2/docs/conf.py` & `pyproject_api-1.5.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyproject_api-1.5.2/docs/index.rst` & `pyproject_api-1.5.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyproject_api-1.5.2/src/pyproject_api/__init__.py` & `pyproject_api-1.5.3/src/pyproject_api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_api-1.5.2/src/pyproject_api/__main__.py` & `pyproject_api-1.5.3/src/pyproject_api/__main__.py`

 * *Files identical despite different names*

### Comparing `pyproject_api-1.5.2/src/pyproject_api/_backend.py` & `pyproject_api-1.5.3/src/pyproject_api/_backend.py`

 * *Files 13% similar despite different names*

```diff
@@ -108,24 +108,25 @@
                     print("Backend: Wrote response {} to {}".format(result, result_file))
                     flush()  # pragma: no branch
         if reuse_process is False:  # pragma: no branch # no test for reuse process in root test env
             break
     return 0
 
 
-def read_line():
+def read_line(fd=0):
     # for some reason input() seems to break (hangs forever) so instead we read byte by byte the unbuffered stream
     content = bytearray()
     while True:
-        try:
-            char = os.read(0, 1)
-        except EOFError:  # pragma: no cover # when the stdout is closed without exit
-            break  # pragma: no cover
-        if char == b"\n":  # pragma: no cover
+        char = os.read(fd, 1)
+        if not char:
+            if not content:
+                raise EOFError("EOF without reading anything")  # we didn't get a line at all, let the caller know
             break
-        if char != b"\r":  # pragma: win32 cover
+        if char == b"\n":
+            break
+        if char != b"\r":
             content += char
     return content
 
 
 if __name__ == "__main__":
     sys.exit(run(sys.argv[1:]))
```

### Comparing `pyproject_api-1.5.2/src/pyproject_api/_backend.pyi` & `pyproject_api-1.5.3/src/pyproject_api/_backend.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -8,9 +8,9 @@
     backend: Any
     def __init__(self, backend_module: str, backend_obj: str | None) -> None: ...
     def __call__(self, name: str, *args: Any, **kwargs: Any) -> Any: ...
     def _exit(self) -> None: ...
     def _optional_commands(self) -> dict[str, bool]: ...
 
 def run(argv: Sequence[str]) -> int: ...
-def read_line() -> bytearray: ...
+def read_line(fd: int = 0) -> bytearray: ...
 def flush() -> None: ...
```

### Comparing `pyproject_api-1.5.2/src/pyproject_api/_frontend.py` & `pyproject_api-1.5.3/src/pyproject_api/_frontend.py`

 * *Files identical despite different names*

### Comparing `pyproject_api-1.5.2/src/pyproject_api/_util.py` & `pyproject_api-1.5.3/src/pyproject_api/_util.py`

 * *Files identical despite different names*

### Comparing `pyproject_api-1.5.2/src/pyproject_api/_via_fresh_subprocess.py` & `pyproject_api-1.5.3/src/pyproject_api/_via_fresh_subprocess.py`

 * *Files identical despite different names*

### Comparing `pyproject_api-1.5.2/tests/test_backend.py` & `pyproject_api-1.5.3/tests/test_backend.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 import json
+import os
 from typing import TYPE_CHECKING, Any
 
 import pytest
 
-from pyproject_api._backend import BackendProxy, run
+from pyproject_api._backend import BackendProxy, read_line, run
 
 if TYPE_CHECKING:
     from pathlib import Path
 
     import pytest_mock
 
 
@@ -123,7 +124,41 @@
     assert ret == 0
     captured = capsys.readouterr()
     assert "started backend FakeBackendProxy" in captured.out
     assert "Backend: run command dummy_command_a with args {'foo': 'bar'}" in captured.out
     assert "Backend: run command dummy_command_b with args {'baz': 'qux'}" in captured.out
     assert "Backend: run command dummy_command_c with args {'win': 'wow'}" in captured.out
     assert "SystemExit: 2" in captured.err
+
+
+def test_read_line_success() -> None:
+    r, w = os.pipe()
+    try:
+        line_in = b"this is a line\r\n"
+        os.write(w, line_in)
+        line_out = read_line(fd=r)
+        assert line_out == bytearray(b"this is a line")
+    finally:
+        os.close(r)
+        os.close(w)
+
+
+def test_read_line_eof_before_newline() -> None:
+    r, w = os.pipe()
+    try:
+        line_in = b"this is a line"
+        os.write(w, line_in)
+        os.close(w)
+        line_out = read_line(fd=r)
+        assert line_out == bytearray(b"this is a line")
+    finally:
+        os.close(r)
+
+
+def test_read_line_eof_at_the_beginning() -> None:
+    r, w = os.pipe()
+    try:
+        os.close(w)
+        with pytest.raises(EOFError):
+            read_line(fd=r)
+    finally:
+        os.close(r)
```

### Comparing `pyproject_api-1.5.2/tests/test_frontend.py` & `pyproject_api-1.5.3/tests/test_frontend.py`

 * *Files identical despite different names*

### Comparing `pyproject_api-1.5.2/tests/test_frontend_setuptools.py` & `pyproject_api-1.5.3/tests/test_frontend_setuptools.py`

 * *Files identical despite different names*

### Comparing `pyproject_api-1.5.2/tests/test_main.py` & `pyproject_api-1.5.3/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pyproject_api-1.5.2/tests/test_util.py` & `pyproject_api-1.5.3/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `pyproject_api-1.5.2/tests/demo_pkg_inline/build.py` & `pyproject_api-1.5.3/tests/demo_pkg_inline/build.py`

 * *Files identical despite different names*

### Comparing `pyproject_api-1.5.2/LICENSE` & `pyproject_api-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject_api-1.5.2/README.md` & `pyproject_api-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `pyproject_api-1.5.2/pyproject.toml` & `pyproject_api-1.5.3/pyproject.toml`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -67,36 +67,14 @@
 [tool.hatch]
 build.hooks.vcs.version-file = "src/pyproject_api/_version.py"
 version.source = "vcs"
 
 [tool.black]
 line-length = 120
 
-[tool.coverage]
-html.show_contexts = true
-html.skip_covered = false
-paths.source = [
-  "src",
-  ".tox*/*/lib/python*/site-packages",
-  ".tox*/pypy*/site-packages",
-  ".tox*\\*\\Lib\\site-packages",
-  "*/src",
-  "*\\src",
-]
-report.fail_under = 98
-report.omit = []
-run.parallel = true
-run.plugins = ["covdefaults"]
-
-[tool.mypy]
-python_version = "3.11"
-show_error_codes = true
-strict = true
-overrides = [{ module = ["virtualenv.*"], ignore_missing_imports = true }]
-
 [tool.ruff]
 select = ["ALL"]
 line-length = 120
 target-version = "py37"
 isort = {known-first-party = ["pyproject_api"], required-imports = ["from __future__ import annotations"]}
 ignore = [
   "INP001",  # no implicit namespaces here
@@ -112,7 +90,29 @@
   "S101",  # asserts allowed in tests...
   "FBT",  # don"t care about booleans as positional arguments in tests
   "INP001", # no implicit namespace
   "D",  # don"t care about documentation in tests
   "S603",  # `subprocess` call: check for execution of untrusted input
   "PLR2004",  # Magic value used in comparison, consider replacing with a constant variable
 ]
+
+[tool.coverage]
+html.show_contexts = true
+html.skip_covered = false
+paths.source = [
+  "src",
+  ".tox*/*/lib/python*/site-packages",
+  ".tox*/pypy*/site-packages",
+  ".tox*\\*\\Lib\\site-packages",
+  "*/src",
+  "*\\src",
+]
+report.fail_under = 98
+report.omit = []
+run.parallel = true
+run.plugins = ["covdefaults"]
+
+[tool.mypy]
+python_version = "3.11"
+show_error_codes = true
+strict = true
+overrides = [{ module = ["virtualenv.*"], ignore_missing_imports = true }]
```

### Comparing `pyproject_api-1.5.2/PKG-INFO` & `pyproject_api-1.5.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-api
-Version: 1.5.2
+Version: 1.5.3
 Summary: API to interact with the python pyproject.toml based projects
 Project-URL: Homepage, http://pyproject_api.readthedocs.org
 Project-URL: Source, https://github.com/tox-dev/pyproject-api
 Project-URL: Tracker, https://github.com/tox-dev/pyproject-api/issues
 Author-email: Bernát Gábor <gaborjbernat@gmail.com>
 Maintainer-email: Bernát Gábor <gaborjbernat@gmail.com>
 License-Expression: MIT
```

