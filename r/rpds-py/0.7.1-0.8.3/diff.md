# Comparing `tmp/rpds_py-0.7.1.tar.gz` & `tmp/rpds_py-0.8.3.tar.gz`

## Comparing `rpds_py-0.7.1.tar` & `rpds_py-0.8.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0      238 1970-01-01 00:00:00.000000 rpds_py-0.7.1/Cargo.toml
--rw-r--r--   0        0        0      219 2023-03-20 19:29:29.000000 rpds_py-0.7.1/.github/dependabot.yml
--rw-r--r--   0        0        0     4321 2023-03-20 19:29:29.000000 rpds_py-0.7.1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      758 2023-03-20 19:29:29.000000 rpds_py-0.7.1/.gitignore
--rw-r--r--   0        0        0     1039 2023-03-20 19:29:29.000000 rpds_py-0.7.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1076 2023-03-20 19:29:29.000000 rpds_py-0.7.1/LICENSE
--rw-r--r--   0        0        0     1741 2023-03-20 19:29:29.000000 rpds_py-0.7.1/README.rst
--rw-r--r--   0        0        0     1043 2023-03-20 19:29:29.000000 rpds_py-0.7.1/noxfile.py
--rw-r--r--   0        0        0     1129 2023-03-20 19:29:29.000000 rpds_py-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     1697 2023-03-20 19:29:29.000000 rpds_py-0.7.1/rpds.pyi
--rw-r--r--   0        0        0    17579 2023-03-20 19:29:29.000000 rpds_py-0.7.1/src/lib.rs
--rw-r--r--   0        0        0       20 2023-03-20 19:29:29.000000 rpds_py-0.7.1/tests/requirements.in
--rw-r--r--   0        0        0      484 2023-03-20 19:29:29.000000 rpds_py-0.7.1/tests/requirements.txt
--rw-r--r--   0        0        0     8651 2023-03-20 19:29:29.000000 rpds_py-0.7.1/tests/test_hash_trie_map.py
--rw-r--r--   0        0        0     5096 2023-03-20 19:29:29.000000 rpds_py-0.7.1/tests/test_hash_trie_set.py
--rw-r--r--   0        0        0     3531 2023-03-20 19:29:29.000000 rpds_py-0.7.1/tests/test_list.py
--rw-r--r--   0        0        0     8633 2023-03-20 19:29:29.000000 rpds_py-0.7.1/Cargo.lock
--rw-r--r--   0        0        0     2651 1970-01-01 00:00:00.000000 rpds_py-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      245 1970-01-01 00:00:00.000000 rpds_py-0.8.3/Cargo.toml
+-rw-r--r--   0        0        0      219 2023-07-06 11:45:33.000000 rpds_py-0.8.3/.github/dependabot.yml
+-rw-r--r--   0        0        0       81 2023-07-06 11:45:33.000000 rpds_py-0.8.3/.github/release.yml
+-rw-r--r--   0        0        0     4321 2023-07-06 11:45:33.000000 rpds_py-0.8.3/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      758 2023-07-06 11:45:33.000000 rpds_py-0.8.3/.gitignore
+-rw-r--r--   0        0        0     1050 2023-07-06 11:45:33.000000 rpds_py-0.8.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1076 2023-07-06 11:45:33.000000 rpds_py-0.8.3/LICENSE
+-rw-r--r--   0        0        0     1741 2023-07-06 11:45:33.000000 rpds_py-0.8.3/README.rst
+-rw-r--r--   0        0        0     1043 2023-07-06 11:45:33.000000 rpds_py-0.8.3/noxfile.py
+-rw-r--r--   0        0        0     1406 2023-07-06 11:45:33.000000 rpds_py-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0     1697 2023-07-06 11:45:33.000000 rpds_py-0.8.3/rpds.pyi
+-rw-r--r--   0        0        0    17578 2023-07-06 11:45:33.000000 rpds_py-0.8.3/src/lib.rs
+-rw-r--r--   0        0        0       20 2023-07-06 11:45:33.000000 rpds_py-0.8.3/tests/requirements.in
+-rw-r--r--   0        0        0      484 2023-07-06 11:45:33.000000 rpds_py-0.8.3/tests/requirements.txt
+-rw-r--r--   0        0        0     8653 2023-07-06 11:45:33.000000 rpds_py-0.8.3/tests/test_hash_trie_map.py
+-rw-r--r--   0        0        0     5098 2023-07-06 11:45:33.000000 rpds_py-0.8.3/tests/test_hash_trie_set.py
+-rw-r--r--   0        0        0     3533 2023-07-06 11:45:33.000000 rpds_py-0.8.3/tests/test_list.py
+-rw-r--r--   0        0        0     8325 2023-07-06 11:46:07.000000 rpds_py-0.8.3/Cargo.lock
+-rw-r--r--   0        0        0     2924 1970-01-01 00:00:00.000000 rpds_py-0.8.3/PKG-INFO
```

### Comparing `rpds_py-0.7.1/.github/workflows/CI.yml` & `rpds_py-0.8.3/.github/workflows/CI.yml`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
   list:
     runs-on: ubuntu-latest
     outputs:
       noxenvs: ${{ steps.noxenvs-matrix.outputs.noxenvs }}
     steps:
       - uses: actions/checkout@v3
       - name: Set up nox
-        uses: wntrblm/nox@2022.11.21
+        uses: wntrblm/nox@2023.04.22
       - id: noxenvs-matrix
         run: |
           echo >>$GITHUB_OUTPUT noxenvs=$(
             nox --list-sessions |
             grep '^* ' |
             cut -d ' ' -f 2- |
             jq --raw-input --slurp 'split("\n") | map(select(. != ""))'
@@ -61,15 +61,15 @@
         run: brew install enchant
         if: runner.os == 'macOS' && startsWith(matrix.noxenv, 'docs')
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: "3.x"
       - name: Set up nox
-        uses: wntrblm/nox@2022.11.21
+        uses: wntrblm/nox@2023.04.22
       - name: Run nox
         run: nox -s "${{ matrix.noxenv }}"
 
   linux:
     needs: test
     runs-on: ubuntu-latest
     strategy:
```

### Comparing `rpds_py-0.7.1/.gitignore` & `rpds_py-0.8.3/.gitignore`

 * *Files identical despite different names*

### Comparing `rpds_py-0.7.1/.pre-commit-config.yaml` & `rpds_py-0.8.3/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -21,20 +21,20 @@
     hooks:
       - id: isort
   - repo: https://github.com/pycqa/flake8
     rev: "6.0.0"
     hooks:
       - id: flake8
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.8.0
     hooks:
       - id: pyupgrade
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - name: black
         id: black
         args: ["--line-length", "79"]
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v3.0.0-alpha.4"
+    rev: "v3.0.0-alpha.9-for-vscode"
     hooks:
       - id: prettier
```

### Comparing `rpds_py-0.7.1/LICENSE` & `rpds_py-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rpds_py-0.7.1/README.rst` & `rpds_py-0.8.3/README.rst`

 * *Files identical despite different names*

### Comparing `rpds_py-0.7.1/noxfile.py` & `rpds_py-0.8.3/noxfile.py`

 * *Files identical despite different names*

### Comparing `rpds_py-0.7.1/rpds.pyi` & `rpds_py-0.8.3/rpds.pyi`

 * *Files identical despite different names*

### Comparing `rpds_py-0.7.1/src/lib.rs` & `rpds_py-0.8.3/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
             .into_py(py)),
             _ => Ok(py.NotImplemented()),
         }
     }
 
     #[classmethod]
     fn convert(_cls: &PyType, value: &PyAny, py: Python) -> PyResult<PyObject> {
-        if value.is_instance_of::<HashTrieMapPy>()? {
+        if value.is_instance_of::<HashTrieMapPy>() {
             Ok(value.into())
         } else {
             Ok(HashTrieMapPy::extract(value)?.into_py(py))
         }
     }
 
     fn get(&self, key: Key) -> Option<&PyObject> {
```

### Comparing `rpds_py-0.7.1/tests/test_hash_trie_map.py` & `rpds_py-0.8.3/tests/test_hash_trie_map.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,17 +24,18 @@
     HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
     WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
     FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
     OTHER DEALINGS IN THE SOFTWARE.
 """
 from collections.abc import Hashable, Mapping
 
-from rpds import HashTrieMap
 import pytest
 
+from rpds import HashTrieMap
+
 HASH_MSG = "Not sure HashTrieMap implements Hash, it has mutable methods"
 
 
 @pytest.mark.xfail(reason=HASH_MSG)
 def test_instance_of_hashable():
     assert isinstance(HashTrieMap(), Hashable)
```

### Comparing `rpds_py-0.7.1/tests/test_hash_trie_set.py` & `rpds_py-0.8.3/tests/test_hash_trie_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,17 +22,18 @@
     OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
     NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
     HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
     WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
     FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
     OTHER DEALINGS IN THE SOFTWARE.
 """
-from rpds import HashTrieSet
 import pytest
 
+from rpds import HashTrieSet
+
 HASH_MSG = "Not sure HashTrieSet implements Hash, it has mutable methods"
 
 
 def test_key_is_tuple():
     with pytest.raises(KeyError):
         HashTrieSet().remove((1, 1))
```

### Comparing `rpds_py-0.7.1/tests/test_list.py` & `rpds_py-0.8.3/tests/test_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,17 +22,18 @@
     OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
     NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
     HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
     WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
     FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
     OTHER DEALINGS IN THE SOFTWARE.
 """
-from rpds import List
 import pytest
 
+from rpds import List
+
 HASH_MSG = "Not sure List implements Hash, it has mutable methods"
 
 
 def test_literalish_works():
     assert List(1, 2, 3) == List([1, 2, 3])
```

### Comparing `rpds_py-0.7.1/Cargo.lock` & `rpds_py-0.8.3/Cargo.lock`

 * *Files 24% similar despite different names*

```diff
@@ -1,308 +1,308 @@
-# This file is automatically @generated by Cargo.
-# It is not intended for manual editing.
-version = 3
-
-[[package]]
-name = "archery"
-version = "0.5.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b6cd774058b1b415c4855d8b86436c04bf050c003156fe24bc326fb3fe75c343"
-dependencies = [
- "static_assertions",
-]
-
-[[package]]
-name = "autocfg"
-version = "1.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
-
-[[package]]
-name = "bitflags"
-version = "1.3.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
-
-[[package]]
-name = "cfg-if"
-version = "1.0.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
-
-[[package]]
-name = "indoc"
-version = "1.0.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
-
-[[package]]
-name = "libc"
-version = "0.2.139"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "201de327520df007757c1f0adce6e827fe8562fbc28bfd9c15571c66ca1f5f79"
-
-[[package]]
-name = "lock_api"
-version = "0.4.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
-dependencies = [
- "autocfg",
- "scopeguard",
-]
-
-[[package]]
-name = "memoffset"
-version = "0.8.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
-dependencies = [
- "autocfg",
-]
-
-[[package]]
-name = "once_cell"
-version = "1.17.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
-
-[[package]]
-name = "parking_lot"
-version = "0.12.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
-dependencies = [
- "lock_api",
- "parking_lot_core",
-]
-
-[[package]]
-name = "parking_lot_core"
-version = "0.9.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
-dependencies = [
- "cfg-if",
- "libc",
- "redox_syscall",
- "smallvec",
- "windows-sys",
-]
-
-[[package]]
-name = "proc-macro2"
-version = "1.0.51"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d727cae5b39d21da60fa540906919ad737832fe0b1c165da3a34d6548c849d6"
-dependencies = [
- "unicode-ident",
-]
-
-[[package]]
-name = "pyo3"
-version = "0.18.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "06a3d8e8a46ab2738109347433cb7b96dffda2e4a218b03ef27090238886b147"
-dependencies = [
- "cfg-if",
- "indoc",
- "libc",
- "memoffset",
- "parking_lot",
- "pyo3-build-config",
- "pyo3-ffi",
- "pyo3-macros",
- "unindent",
-]
-
-[[package]]
-name = "pyo3-build-config"
-version = "0.18.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75439f995d07ddfad42b192dfcf3bc66a7ecfd8b4a1f5f6f046aa5c2c5d7677d"
-dependencies = [
- "once_cell",
- "target-lexicon",
-]
-
-[[package]]
-name = "pyo3-ffi"
-version = "0.18.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "839526a5c07a17ff44823679b68add4a58004de00512a95b6c1c98a6dcac0ee5"
-dependencies = [
- "libc",
- "pyo3-build-config",
-]
-
-[[package]]
-name = "pyo3-macros"
-version = "0.18.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd44cf207476c6a9760c4653559be4f206efafb924d3e4cbf2721475fc0d6cc5"
-dependencies = [
- "proc-macro2",
- "pyo3-macros-backend",
- "quote",
- "syn",
-]
-
-[[package]]
-name = "pyo3-macros-backend"
-version = "0.18.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc1f43d8e30460f36350d18631ccf85ded64c059829208fe680904c65bcd0a4c"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn",
-]
-
-[[package]]
-name = "quote"
-version = "1.0.23"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
-dependencies = [
- "proc-macro2",
-]
-
-[[package]]
-name = "redox_syscall"
-version = "0.2.16"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
-dependencies = [
- "bitflags",
-]
-
-[[package]]
-name = "rpds"
-version = "0.13.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9bd6ce569b15c331b1e5fd8cf6adb0bf240678b5f0cdc4d0f41e11683f6feba9"
-dependencies = [
- "archery",
-]
-
-[[package]]
-name = "rpds-py"
-version = "0.7.1"
-dependencies = [
- "archery",
- "pyo3",
- "rpds",
-]
-
-[[package]]
-name = "scopeguard"
-version = "1.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
-
-[[package]]
-name = "smallvec"
-version = "1.10.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
-
-[[package]]
-name = "static_assertions"
-version = "1.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
-
-[[package]]
-name = "syn"
-version = "1.0.109"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
-dependencies = [
- "proc-macro2",
- "quote",
- "unicode-ident",
-]
-
-[[package]]
-name = "target-lexicon"
-version = "0.12.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
-
-[[package]]
-name = "unicode-ident"
-version = "1.0.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84a22b9f218b40614adcb3f4ff08b703773ad44fa9423e4e0d346d5db86e4ebc"
-
-[[package]]
-name = "unindent"
-version = "0.1.11"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
-
-[[package]]
-name = "windows-sys"
-version = "0.45.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
-dependencies = [
- "windows-targets",
-]
-
-[[package]]
-name = "windows-targets"
-version = "0.42.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e2522491fbfcd58cc84d47aeb2958948c4b8982e9a2d8a2a35bbaed431390e7"
-dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
-]
-
-[[package]]
-name = "windows_aarch64_gnullvm"
-version = "0.42.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c9864e83243fdec7fc9c5444389dcbbfd258f745e7853198f365e3c4968a608"
-
-[[package]]
-name = "windows_aarch64_msvc"
-version = "0.42.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8b1b673ffc16c47a9ff48570a9d85e25d265735c503681332589af6253c6c7"
-
-[[package]]
-name = "windows_i686_gnu"
-version = "0.42.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3887528ad530ba7bdbb1faa8275ec7a1155a45ffa57c37993960277145d640"
-
-[[package]]
-name = "windows_i686_msvc"
-version = "0.42.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf4d1122317eddd6ff351aa852118a2418ad4214e6613a50e0191f7004372605"
-
-[[package]]
-name = "windows_x86_64_gnu"
-version = "0.42.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1040f221285e17ebccbc2591ffdc2d44ee1f9186324dd3e84e99ac68d699c45"
-
-[[package]]
-name = "windows_x86_64_gnullvm"
-version = "0.42.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "628bfdf232daa22b0d64fdb62b09fcc36bb01f05a3939e20ab73aaf9470d0463"
-
-[[package]]
-name = "windows_x86_64_msvc"
-version = "0.42.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "447660ad36a13288b1db4d4248e857b510e8c3a225c822ba4fb748c0aafecffd"
+# This file is automatically @generated by Cargo.
+# It is not intended for manual editing.
+version = 3
+
+[[package]]
+name = "archery"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6cd774058b1b415c4855d8b86436c04bf050c003156fe24bc326fb3fe75c343"
+dependencies = [
+ "static_assertions",
+]
+
+[[package]]
+name = "autocfg"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+
+[[package]]
+name = "bitflags"
+version = "1.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
+
+[[package]]
+name = "cfg-if"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
+
+[[package]]
+name = "indoc"
+version = "1.0.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
+
+[[package]]
+name = "libc"
+version = "0.2.139"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "201de327520df007757c1f0adce6e827fe8562fbc28bfd9c15571c66ca1f5f79"
+
+[[package]]
+name = "lock_api"
+version = "0.4.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+dependencies = [
+ "autocfg",
+ "scopeguard",
+]
+
+[[package]]
+name = "memoffset"
+version = "0.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+dependencies = [
+ "autocfg",
+]
+
+[[package]]
+name = "once_cell"
+version = "1.17.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+
+[[package]]
+name = "parking_lot"
+version = "0.12.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+dependencies = [
+ "lock_api",
+ "parking_lot_core",
+]
+
+[[package]]
+name = "parking_lot_core"
+version = "0.9.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+dependencies = [
+ "cfg-if",
+ "libc",
+ "redox_syscall",
+ "smallvec",
+ "windows-sys",
+]
+
+[[package]]
+name = "proc-macro2"
+version = "1.0.51"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5d727cae5b39d21da60fa540906919ad737832fe0b1c165da3a34d6548c849d6"
+dependencies = [
+ "unicode-ident",
+]
+
+[[package]]
+name = "pyo3"
+version = "0.19.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ffb88ae05f306b4bfcde40ac4a51dc0b05936a9207a4b75b798c7729c4258a59"
+dependencies = [
+ "cfg-if",
+ "indoc",
+ "libc",
+ "memoffset",
+ "parking_lot",
+ "pyo3-build-config",
+ "pyo3-ffi",
+ "pyo3-macros",
+ "unindent",
+]
+
+[[package]]
+name = "pyo3-build-config"
+version = "0.19.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "554db24f0b3c180a9c0b1268f91287ab3f17c162e15b54caaae5a6b3773396b0"
+dependencies = [
+ "once_cell",
+ "target-lexicon",
+]
+
+[[package]]
+name = "pyo3-ffi"
+version = "0.19.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "922ede8759e8600ad4da3195ae41259654b9c55da4f7eec84a0ccc7d067a70a4"
+dependencies = [
+ "libc",
+ "pyo3-build-config",
+]
+
+[[package]]
+name = "pyo3-macros"
+version = "0.19.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8a5caec6a1dd355964a841fcbeeb1b89fe4146c87295573f94228911af3cc5a2"
+dependencies = [
+ "proc-macro2",
+ "pyo3-macros-backend",
+ "quote",
+ "syn",
+]
+
+[[package]]
+name = "pyo3-macros-backend"
+version = "0.19.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e0b78ccbb160db1556cdb6fd96c50334c5d4ec44dc5e0a968d0a1208fa0efa8b"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn",
+]
+
+[[package]]
+name = "quote"
+version = "1.0.23"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+dependencies = [
+ "proc-macro2",
+]
+
+[[package]]
+name = "redox_syscall"
+version = "0.2.16"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+dependencies = [
+ "bitflags",
+]
+
+[[package]]
+name = "rpds"
+version = "0.13.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9bd6ce569b15c331b1e5fd8cf6adb0bf240678b5f0cdc4d0f41e11683f6feba9"
+dependencies = [
+ "archery",
+]
+
+[[package]]
+name = "rpds-py"
+version = "0.8.3"
+dependencies = [
+ "archery",
+ "pyo3",
+ "rpds",
+]
+
+[[package]]
+name = "scopeguard"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+
+[[package]]
+name = "smallvec"
+version = "1.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+
+[[package]]
+name = "static_assertions"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
+
+[[package]]
+name = "syn"
+version = "1.0.109"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
+
+[[package]]
+name = "target-lexicon"
+version = "0.12.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+
+[[package]]
+name = "unicode-ident"
+version = "1.0.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "84a22b9f218b40614adcb3f4ff08b703773ad44fa9423e4e0d346d5db86e4ebc"
+
+[[package]]
+name = "unindent"
+version = "0.1.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
+
+[[package]]
+name = "windows-sys"
+version = "0.45.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
+dependencies = [
+ "windows-targets",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.42.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8e2522491fbfcd58cc84d47aeb2958948c4b8982e9a2d8a2a35bbaed431390e7"
+dependencies = [
+ "windows_aarch64_gnullvm",
+ "windows_aarch64_msvc",
+ "windows_i686_gnu",
+ "windows_i686_msvc",
+ "windows_x86_64_gnu",
+ "windows_x86_64_gnullvm",
+ "windows_x86_64_msvc",
+]
+
+[[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.42.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8c9864e83243fdec7fc9c5444389dcbbfd258f745e7853198f365e3c4968a608"
+
+[[package]]
+name = "windows_aarch64_msvc"
+version = "0.42.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4c8b1b673ffc16c47a9ff48570a9d85e25d265735c503681332589af6253c6c7"
+
+[[package]]
+name = "windows_i686_gnu"
+version = "0.42.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "de3887528ad530ba7bdbb1faa8275ec7a1155a45ffa57c37993960277145d640"
+
+[[package]]
+name = "windows_i686_msvc"
+version = "0.42.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bf4d1122317eddd6ff351aa852118a2418ad4214e6613a50e0191f7004372605"
+
+[[package]]
+name = "windows_x86_64_gnu"
+version = "0.42.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c1040f221285e17ebccbc2591ffdc2d44ee1f9186324dd3e84e99ac68d699c45"
+
+[[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.42.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "628bfdf232daa22b0d64fdb62b09fcc36bb01f05a3939e20ab73aaf9470d0463"
+
+[[package]]
+name = "windows_x86_64_msvc"
+version = "0.42.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "447660ad36a13288b1db4d4248e857b510e8c3a225c822ba4fb748c0aafecffd"
```

### Comparing `rpds_py-0.7.1/PKG-INFO` & `rpds_py-0.8.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: rpds-py
-Version: 0.7.1
+Version: 0.8.3
 Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Rust
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
@@ -16,14 +17,18 @@
 Summary: Python bindings to Rust's persistent data structures (rpds)
 Keywords: data structures,rust,persistent
 Author: Julian Berman
 Author-email: Julian+rpds@GrayVines.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst; charset=UTF-8
+Project-URL: Homepage, https://github.com/crate-py/rpds
+Project-URL: Issues, https://github.com/crate-py/rpds/issues/
+Project-URL: Funding, https://github.com/sponsors/Julian
+Project-URL: Source, https://github.com/crate-py/rpds
 
 ===========
 ``rpds.py``
 ===========
 
 |PyPI| |Pythons| |CI|
```

