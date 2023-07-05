# Comparing `tmp/reth_db_py-0.1.3.tar.gz` & `tmp/reth_db_py-0.1.4.tar.gz`

## Comparing `reth_db_py-0.1.3.tar` & `reth_db_py-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 reth_db_py-0.1.3/Cargo.toml
--rw-r--r--   0     1001      123     2413 2023-06-30 02:03:09.000000 reth_db_py-0.1.3/.github/workflows/CI.yml
--rw-r--r--   0     1001      123     3078 2023-06-30 02:03:09.000000 reth_db_py-0.1.3/.gitignore
--rw-r--r--   0     1001      123     1061 2023-06-30 02:03:09.000000 reth_db_py-0.1.3/LICENSE
--rw-r--r--   0     1001      123     3246 2023-06-30 02:03:09.000000 reth_db_py-0.1.3/README.md
--rw-r--r--   0     1001      123     1216 2023-06-30 02:03:09.000000 reth_db_py-0.1.3/examples.py
--rw-r--r--   0     1001      123      546 2023-06-30 02:03:09.000000 reth_db_py-0.1.3/pyproject.toml
--rw-r--r--   0     1001      123      495 2023-06-30 02:03:09.000000 reth_db_py-0.1.3/src/lib.rs
--rw-r--r--   0     1001      123     2408 2023-06-30 02:03:09.000000 reth_db_py-0.1.3/src/types.rs
--rw-r--r--   0     1001      123     6238 2023-06-30 02:03:09.000000 reth_db_py-0.1.3/src/utils.rs
--rw-r--r--   0     1001      123    73089 2023-06-30 02:03:19.000000 reth_db_py-0.1.3/Cargo.lock
--rw-r--r--   0        0        0     3667 1970-01-01 00:00:00.000000 reth_db_py-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      544 1970-01-01 00:00:00.000000 reth_db_py-0.1.4/Cargo.toml
+-rw-r--r--   0     1001      123     2413 2023-07-05 22:11:32.000000 reth_db_py-0.1.4/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123     3078 2023-07-05 22:11:32.000000 reth_db_py-0.1.4/.gitignore
+-rw-r--r--   0     1001      123      726 2023-07-05 22:11:32.000000 reth_db_py-0.1.4/CHANGELOG.md
+-rw-r--r--   0     1001      123     1061 2023-07-05 22:11:32.000000 reth_db_py-0.1.4/LICENSE
+-rw-r--r--   0     1001      123     4520 2023-07-05 22:11:32.000000 reth_db_py-0.1.4/README.md
+-rw-r--r--   0     1001      123     1893 2023-07-05 22:11:32.000000 reth_db_py-0.1.4/examples.py
+-rw-r--r--   0     1001      123      546 2023-07-05 22:11:32.000000 reth_db_py-0.1.4/pyproject.toml
+-rw-r--r--   0     1001      123     3114 2023-07-05 22:11:32.000000 reth_db_py-0.1.4/reth_db_py.pyi
+-rw-r--r--   0     1001      123      374 2023-07-05 22:11:32.000000 reth_db_py-0.1.4/src/lib.rs
+-rw-r--r--   0     1001      123     3257 2023-07-05 22:11:32.000000 reth_db_py-0.1.4/src/types.rs
+-rw-r--r--   0     1001      123     3193 2023-07-05 22:11:32.000000 reth_db_py-0.1.4/src/utils.rs
+-rw-r--r--   0     1001      123    77816 2023-07-05 22:11:43.000000 reth_db_py-0.1.4/Cargo.lock
+-rw-r--r--   0        0        0     4941 1970-01-01 00:00:00.000000 reth_db_py-0.1.4/PKG-INFO
```

### Comparing `reth_db_py-0.1.3/.github/workflows/CI.yml` & `reth_db_py-0.1.4/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `reth_db_py-0.1.3/.gitignore` & `reth_db_py-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `reth_db_py-0.1.3/LICENSE` & `reth_db_py-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `reth_db_py-0.1.3/pyproject.toml` & `reth_db_py-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=1.1,<2.0"]
 build-backend = "maturin.sdist"
 
 [project]
 name = "reth-db-py"
-version = "0.1.3"
+version = "0.1.4"
 description = "Python wrapper around reth db. Written in Rust."
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/gibz104/reth-db-py"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Rust",
```

### Comparing `reth_db_py-0.1.3/Cargo.lock` & `reth_db_py-0.1.4/Cargo.lock`

 * *Files 6% similar despite different names*

```diff
@@ -84,21 +84,21 @@
 name = "arrayvec"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "96d30a06541fbafbc7f82ed10c06164cfbd2c401138f6addd8404629c4b16711"
 
 [[package]]
 name = "async-trait"
-version = "0.1.68"
+version = "0.1.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
+checksum = "a564d521dd56509c4c47480d00b80ee55f7e385ae48db5744c67ad50c92d2ebf"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "atomic-polyfill"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3ff7eb3f316534d83a8a2c3d1674ace8a5a71198eba31e2e2b597833f699b28"
@@ -168,36 +168,42 @@
 
 [[package]]
 name = "bindgen"
 version = "0.65.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cfdf7b466f9a4903edc73f95d6d2bcd5baf8ae620638762244d3f60143643cc5"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "cexpr",
  "clang-sys",
  "lazy_static",
  "lazycell",
  "peeking_take_while",
  "prettyplease",
  "proc-macro2",
  "quote",
  "regex",
  "rustc-hash",
  "shlex",
- "syn 2.0.22",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "bitflags"
+version = "2.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "630be753d4e58660abd17930c71b647fe46c27ea6b63cc59e1e3851406972e42"
+
+[[package]]
 name = "bitvec"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1bc2832c24239b0141d5674bb9174f9d68a8b5b3f2753311927c172ca46f7e9c"
 dependencies = [
  "funty",
  "radium",
@@ -314,22 +320,22 @@
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "67ba02a97a2bd10f4b59b25c7973101c79642302776489e030cd13cdab09ed15"
 
 [[package]]
 name = "codecs-derive"
 version = "0.1.0-alpha.1"
-source = "git+https://github.com/paradigmxyz/reth#3dcc76e2b0aba962dd130934f698231250ef5ae6"
+source = "git+https://github.com/paradigmxyz/reth#428a6dc2f63ac7f2798c0cb56cf099108d7cbd00"
 dependencies = [
  "convert_case 0.6.0",
  "parity-scale-codec",
  "proc-macro2",
  "quote",
  "serde",
- "syn 2.0.22",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "const-oid"
 version = "0.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6340df57935414636969091153f35f68d9f00bbc8fb4a9c6054706c213e6c6bc"
@@ -353,17 +359,17 @@
 name = "core-foundation-sys"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03e69e28e9f7f77debdedbaafa2866e1de9ba56df55a8bd7cfc724c25a09987c"
+checksum = "a17b76ff3a4162b0b27f354a0c87015ddad39d35f9c0c36607a3bdd175dde1f1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc"
 version = "3.0.1"
@@ -439,26 +445,26 @@
 checksum = "ab8bfa2e259f8ee1ce5e97824a3c55ec4404a0d772ca7fa96bf19f0752a046eb"
 dependencies = [
  "fnv",
  "ident_case",
  "proc-macro2",
  "quote",
  "strsim",
- "syn 2.0.22",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "darling_macro"
 version = "0.20.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "29a358ff9f12ec09c3e61fef9b5a9902623a695a46a917b07f269bff1445611a"
 dependencies = [
  "darling_core",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "der"
 version = "0.7.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c7ed52955ce76b1554f509074bb357d3fb8ac9b51288a65a3fd480d1dfba946"
@@ -515,14 +521,20 @@
  "enum-ordinalize",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "either"
+version = "1.8.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
+
+[[package]]
 name = "elliptic-curve"
 version = "0.13.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "968405c8fdc9b3bf4df0a6638858cc0b52462836ab6b1c87377785dd09cf1c0b"
 dependencies = [
  "base16ct",
  "crypto-bigint",
@@ -543,26 +555,26 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e4f76552f53cefc9a7f64987c3701b99d982f7690606fd67de1d09712fbf52f1"
 dependencies = [
  "num-bigint",
  "num-traits",
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "enumn"
-version = "0.1.8"
+version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "48016319042fb7c87b78d2993084a831793a897a5cd1a2a67cab9d1eeb4b7d76"
+checksum = "c9838a970f5de399d3070ae1739e131986b2f5dcc223c7423ca0927e3a878522"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "equivalent"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "88bffebc5d80432c9b140ee17875ff173a8ab62faad5b257da912bd2f6c1c0a1"
@@ -777,15 +789,15 @@
 name = "futures-macro"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
@@ -902,29 +914,29 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "db04bc24a18b9ea980628ecf00e6c0264f3c1426dac36c00cb49b6fbad8b0743"
 dependencies = [
  "atomic-polyfill",
  "hash32",
  "rustc_version",
  "serde",
- "spin",
+ "spin 0.9.8",
  "stable_deref_trait",
 ]
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hermit-abi"
-version = "0.3.1"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
+checksum = "443144c8cdadd93ebf52ddb4056d257f5b52c04d3c804e657d19eb73fc33668b"
 
 [[package]]
 name = "hex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 dependencies = [
@@ -1089,18 +1101,27 @@
 dependencies = [
  "hermit-abi",
  "libc",
  "windows-sys",
 ]
 
 [[package]]
+name = "itertools"
+version = "0.10.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
+dependencies = [
+ "either",
+]
+
+[[package]]
 name = "itoa"
-version = "1.0.6"
+version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
+checksum = "62b02a5381cc465bd3041d84623d0fa3b66738b52b8e2fc3bab8ad63ab032f4a"
 
 [[package]]
 name = "jobserver"
 version = "0.1.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "936cfd212a0155903bcbc060e316fb6cc7cbf2e1907329391ebadc1fe0ce77c2"
 dependencies = [
@@ -1153,14 +1174,17 @@
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
+dependencies = [
+ "spin 0.5.2",
+]
 
 [[package]]
 name = "lazycell"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830d08ce1d1d941e6b30645f1a0eb5643013d835ce3779a5fc208261dbe10f55"
 
@@ -1293,35 +1317,81 @@
 checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
 dependencies = [
  "memchr",
  "minimal-lexical",
 ]
 
 [[package]]
+name = "num"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "43db66d1170d347f9a065114077f7dccb00c1b9478c89384490a3425279a4606"
+dependencies = [
+ "num-bigint",
+ "num-complex",
+ "num-integer",
+ "num-iter",
+ "num-rational",
+ "num-traits",
+]
+
+[[package]]
 name = "num-bigint"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f93ab6289c7b344a8a9f60f88d80aa20032336fe78da341afc91c8a2341fc75f"
 dependencies = [
  "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
+name = "num-complex"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "02e0d21255c828d6f128a1e41534206671e8c3ea0c62f32291e808dc82cff17d"
+dependencies = [
+ "num-traits",
+]
+
+[[package]]
 name = "num-integer"
 version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
 dependencies = [
  "autocfg",
  "num-traits",
 ]
 
 [[package]]
+name = "num-iter"
+version = "0.1.43"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7d03e6c028c5dc5cac6e2dec0efda81fc887605bb3d884578bb6d6bf7514e252"
+dependencies = [
+ "autocfg",
+ "num-integer",
+ "num-traits",
+]
+
+[[package]]
+name = "num-rational"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0638a1c9d0a3c0914158145bc76cff373a75a627e6ecbfb71cbe6f453a5a19b0"
+dependencies = [
+ "autocfg",
+ "num-bigint",
+ "num-integer",
+ "num-traits",
+]
+
+[[package]]
 name = "num-traits"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
 ]
@@ -1350,15 +1420,24 @@
 version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "96667db765a921f7b295ffee8b60472b686a51d4f21c2ee4ffdb94c7013b65a6"
 dependencies = [
  "proc-macro-crate",
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.23",
+]
+
+[[package]]
+name = "num_threads"
+version = "0.1.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2819ce041d2ee131036f4fc9d6ae7ae125a3a40e97ba64d04fe799ad9dabbb44"
+dependencies = [
+ "libc",
 ]
 
 [[package]]
 name = "object"
 version = "0.31.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8bda667d9f2b5051b8833f59f3bf748b28ef54f850f4fcb389a252aa383866d1"
@@ -1405,32 +1484,32 @@
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "parity-scale-codec"
-version = "3.6.1"
+version = "3.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2287753623c76f953acd29d15d8100bcab84d29db78fb6f352adb3c53e83b967"
+checksum = "756d439303e94fae44f288ba881ad29670c65b0c4b0e05674ca81061bb65f2c5"
 dependencies = [
  "arrayvec",
  "bitvec",
  "byte-slice-cast",
  "bytes",
  "impl-trait-for-tuples",
  "parity-scale-codec-derive",
  "serde",
 ]
 
 [[package]]
 name = "parity-scale-codec-derive"
-version = "3.6.1"
+version = "3.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b6937b5e67bfba3351b87b040d48352a2fcb6ad72f81855412ce97b45c8f110"
+checksum = "9d884d78fcf214d70b1e239fcd1c6e5e95aa3be1881918da2e488cc946c7a476"
 dependencies = [
  "proc-macro-crate",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
@@ -1467,37 +1546,37 @@
 name = "percent-encoding"
 version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
 
 [[package]]
 name = "pin-project"
-version = "1.1.1"
+version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6e138fdd8263907a2b0e1b4e80b7e58c721126479b6e6eedfb1b402acea7b9bd"
+checksum = "030ad2bc4db10a8944cb0d837f158bdfec4d4a4873ab701a95046770d11f8842"
 dependencies = [
  "pin-project-internal",
 ]
 
 [[package]]
 name = "pin-project-internal"
-version = "1.1.1"
+version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d1fef411b303e3e12d534fb6e7852de82da56edd937d895125821fb7c09436c7"
+checksum = "ec2e072ecce94ec471b13398d5402c188e76ac03cf74dd1a975161b23a3f6d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.9"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
+checksum = "4c40d25201921e5ff0c862a505c6557ea88568a4e3ace775ab55e93f2f4f9d57"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
@@ -1556,20 +1635,20 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "prettyplease"
-version = "0.2.9"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9825a04601d60621feed79c4e6b56d65db77cdca55cef43b46b0de1096d1c282"
+checksum = "92139198957b410250d43fad93e630d956499a625c527eda65175c8680f83387"
 dependencies = [
  "proc-macro2",
- "syn 2.0.22",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "primitive-types"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9f3486ccba82358b11a77516035647c34ba167dfa53312630de83b12bd4f3d66"
@@ -1623,66 +1702,66 @@
 checksum = "7b368fba921b0dce7e60f5e04ec15e565b3303972b42bcfde1d0713b881959eb"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cffef52f74ec3b1a1baf295d9b8fcc3070327aefc39a6d00656b13c1d0b8885c"
+checksum = "ffb88ae05f306b4bfcde40ac4a51dc0b05936a9207a4b75b798c7729c4258a59"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "713eccf888fb05f1a96eb78c0dbc51907fee42b3377272dc902eb38985f418d5"
+checksum = "554db24f0b3c180a9c0b1268f91287ab3f17c162e15b54caaae5a6b3773396b0"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b2ecbdcfb01cbbf56e179ce969a048fd7305a66d4cdf3303e0da09d69afe4c3"
+checksum = "922ede8759e8600ad4da3195ae41259654b9c55da4f7eec84a0ccc7d067a70a4"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b78fdc0899f2ea781c463679b20cb08af9247febc8d052de941951024cd8aea0"
+checksum = "8a5caec6a1dd355964a841fcbeeb1b89fe4146c87295573f94228911af3cc5a2"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "60da7b84f1227c3e2fe7593505de274dcf4c8928b4e0a1c23d551a14e4e80a0f"
+checksum = "e0b78ccbb160db1556cdb6fd96c50334c5d4ec44dc5e0a968d0a1208fa0efa8b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
@@ -1732,48 +1811,60 @@
 
 [[package]]
 name = "redox_syscall"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
-version = "1.8.4"
+version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
+checksum = "89089e897c013b3deb627116ae56a6955a72b8bed395c9526af31c9fe528b484"
+dependencies = [
+ "aho-corasick",
+ "memchr",
+ "regex-automata",
+ "regex-syntax",
+]
+
+[[package]]
+name = "regex-automata"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fa250384981ea14565685dea16a9ccc4d1c541a13f82b9c168572264d1df8c56"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.7.2"
+version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
+checksum = "2ab07dc67230e4a4718e70fd5c20055a4334b121f1f9db8fe63ef39ce9b8c846"
 
 [[package]]
 name = "reth-codecs"
 version = "0.1.0-alpha.1"
-source = "git+https://github.com/paradigmxyz/reth#3dcc76e2b0aba962dd130934f698231250ef5ae6"
+source = "git+https://github.com/paradigmxyz/reth#428a6dc2f63ac7f2798c0cb56cf099108d7cbd00"
 dependencies = [
  "bytes",
  "codecs-derive",
  "revm-primitives",
 ]
 
 [[package]]
 name = "reth-db"
 version = "0.1.0-alpha.1"
-source = "git+https://github.com/paradigmxyz/reth#3dcc76e2b0aba962dd130934f698231250ef5ae6"
+source = "git+https://github.com/paradigmxyz/reth#428a6dc2f63ac7f2798c0cb56cf099108d7cbd00"
 dependencies = [
  "bytes",
  "derive_more",
  "eyre",
  "futures",
  "heapless",
  "modular-bitfield",
@@ -1791,27 +1882,28 @@
  "thiserror",
  "tokio-stream",
  "vergen",
 ]
 
 [[package]]
 name = "reth-db-py"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
  "eyre",
  "pyo3",
  "reth-db",
  "reth-primitives",
+ "reth-provider",
  "serde_json",
 ]
 
 [[package]]
 name = "reth-ecies"
 version = "0.1.0-alpha.1"
-source = "git+https://github.com/paradigmxyz/reth#3dcc76e2b0aba962dd130934f698231250ef5ae6"
+source = "git+https://github.com/paradigmxyz/reth#428a6dc2f63ac7f2798c0cb56cf099108d7cbd00"
 dependencies = [
  "aes",
  "block-padding",
  "byteorder",
  "cipher",
  "ctr",
  "digest",
@@ -1834,15 +1926,15 @@
  "tracing",
  "typenum",
 ]
 
 [[package]]
 name = "reth-eth-wire"
 version = "0.1.0-alpha.1"
-source = "git+https://github.com/paradigmxyz/reth#3dcc76e2b0aba962dd130934f698231250ef5ae6"
+source = "git+https://github.com/paradigmxyz/reth#428a6dc2f63ac7f2798c0cb56cf099108d7cbd00"
 dependencies = [
  "async-trait",
  "bytes",
  "ethers-core",
  "futures",
  "pin-project",
  "reth-codecs",
@@ -1859,15 +1951,15 @@
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
 name = "reth-interfaces"
 version = "0.1.0-alpha.1"
-source = "git+https://github.com/paradigmxyz/reth#3dcc76e2b0aba962dd130934f698231250ef5ae6"
+source = "git+https://github.com/paradigmxyz/reth#428a6dc2f63ac7f2798c0cb56cf099108d7cbd00"
 dependencies = [
  "async-trait",
  "auto_impl",
  "futures",
  "modular-bitfield",
  "parity-scale-codec",
  "parking_lot",
@@ -1883,85 +1975,85 @@
  "tokio-stream",
  "tracing",
 ]
 
 [[package]]
 name = "reth-libmdbx"
 version = "0.1.0-alpha.1"
-source = "git+https://github.com/paradigmxyz/reth#3dcc76e2b0aba962dd130934f698231250ef5ae6"
+source = "git+https://github.com/paradigmxyz/reth#428a6dc2f63ac7f2798c0cb56cf099108d7cbd00"
 dependencies = [
- "bitflags",
+ "bitflags 2.3.3",
  "byteorder",
  "derive_more",
  "indexmap 1.9.3",
  "libc",
  "parking_lot",
  "reth-mdbx-sys",
  "thiserror",
 ]
 
 [[package]]
 name = "reth-mdbx-sys"
 version = "0.1.0-alpha.1"
-source = "git+https://github.com/paradigmxyz/reth#3dcc76e2b0aba962dd130934f698231250ef5ae6"
+source = "git+https://github.com/paradigmxyz/reth#428a6dc2f63ac7f2798c0cb56cf099108d7cbd00"
 dependencies = [
  "bindgen",
  "cc",
  "libc",
 ]
 
 [[package]]
 name = "reth-metrics"
 version = "0.1.0-alpha.1"
-source = "git+https://github.com/paradigmxyz/reth#3dcc76e2b0aba962dd130934f698231250ef5ae6"
+source = "git+https://github.com/paradigmxyz/reth#428a6dc2f63ac7f2798c0cb56cf099108d7cbd00"
 dependencies = [
  "metrics",
  "reth-metrics-derive",
 ]
 
 [[package]]
 name = "reth-metrics-derive"
 version = "0.1.0-alpha.1"
-source = "git+https://github.com/paradigmxyz/reth#3dcc76e2b0aba962dd130934f698231250ef5ae6"
+source = "git+https://github.com/paradigmxyz/reth#428a6dc2f63ac7f2798c0cb56cf099108d7cbd00"
 dependencies = [
  "once_cell",
  "proc-macro2",
  "quote",
  "regex",
- "syn 2.0.22",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "reth-net-common"
 version = "0.1.0-alpha.1"
-source = "git+https://github.com/paradigmxyz/reth#3dcc76e2b0aba962dd130934f698231250ef5ae6"
+source = "git+https://github.com/paradigmxyz/reth#428a6dc2f63ac7f2798c0cb56cf099108d7cbd00"
 dependencies = [
  "pin-project",
  "reth-primitives",
  "tokio",
 ]
 
 [[package]]
 name = "reth-network-api"
 version = "0.1.0-alpha.1"
-source = "git+https://github.com/paradigmxyz/reth#3dcc76e2b0aba962dd130934f698231250ef5ae6"
+source = "git+https://github.com/paradigmxyz/reth#428a6dc2f63ac7f2798c0cb56cf099108d7cbd00"
 dependencies = [
  "async-trait",
  "reth-eth-wire",
  "reth-primitives",
  "reth-rpc-types",
  "serde",
  "thiserror",
  "tokio",
 ]
 
 [[package]]
 name = "reth-primitives"
 version = "0.1.0-alpha.1"
-source = "git+https://github.com/paradigmxyz/reth#3dcc76e2b0aba962dd130934f698231250ef5ae6"
+source = "git+https://github.com/paradigmxyz/reth#428a6dc2f63ac7f2798c0cb56cf099108d7cbd00"
 dependencies = [
  "bytes",
  "crc",
  "crunchy",
  "derive_more",
  "ethers-core",
  "fixed-hash",
@@ -1990,51 +2082,136 @@
  "tracing",
  "triehash",
  "url",
  "zstd",
 ]
 
 [[package]]
+name = "reth-provider"
+version = "0.1.0-alpha.1"
+source = "git+https://github.com/paradigmxyz/reth#428a6dc2f63ac7f2798c0cb56cf099108d7cbd00"
+dependencies = [
+ "auto_impl",
+ "derive_more",
+ "itertools",
+ "parking_lot",
+ "pin-project",
+ "reth-db",
+ "reth-interfaces",
+ "reth-primitives",
+ "reth-revm-primitives",
+ "reth-trie",
+ "tokio",
+ "tokio-stream",
+ "tracing",
+]
+
+[[package]]
+name = "reth-revm-primitives"
+version = "0.1.0-alpha.1"
+source = "git+https://github.com/paradigmxyz/reth#428a6dc2f63ac7f2798c0cb56cf099108d7cbd00"
+dependencies = [
+ "reth-primitives",
+ "revm",
+]
+
+[[package]]
 name = "reth-rlp"
 version = "0.1.0-alpha.1"
-source = "git+https://github.com/paradigmxyz/reth#3dcc76e2b0aba962dd130934f698231250ef5ae6"
+source = "git+https://github.com/paradigmxyz/reth#428a6dc2f63ac7f2798c0cb56cf099108d7cbd00"
 dependencies = [
  "arrayvec",
  "auto_impl",
  "bytes",
  "ethereum-types",
  "reth-rlp-derive",
  "revm-primitives",
  "smol_str",
 ]
 
 [[package]]
 name = "reth-rlp-derive"
 version = "0.1.0-alpha.1"
-source = "git+https://github.com/paradigmxyz/reth#3dcc76e2b0aba962dd130934f698231250ef5ae6"
+source = "git+https://github.com/paradigmxyz/reth#428a6dc2f63ac7f2798c0cb56cf099108d7cbd00"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "reth-rpc-types"
 version = "0.1.0-alpha.1"
-source = "git+https://github.com/paradigmxyz/reth#3dcc76e2b0aba962dd130934f698231250ef5ae6"
+source = "git+https://github.com/paradigmxyz/reth#428a6dc2f63ac7f2798c0cb56cf099108d7cbd00"
 dependencies = [
  "jsonrpsee-types",
  "reth-primitives",
  "reth-rlp",
  "serde",
  "serde_json",
  "thiserror",
 ]
 
 [[package]]
+name = "reth-trie"
+version = "0.1.0-alpha.1"
+source = "git+https://github.com/paradigmxyz/reth#428a6dc2f63ac7f2798c0cb56cf099108d7cbd00"
+dependencies = [
+ "derive_more",
+ "hex",
+ "reth-db",
+ "reth-interfaces",
+ "reth-primitives",
+ "reth-rlp",
+ "thiserror",
+ "tokio",
+ "tracing",
+]
+
+[[package]]
+name = "revm"
+version = "3.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f293f351c4c203d321744e54ed7eed3d2b6eef4c140228910dde3ac9a5ea8031"
+dependencies = [
+ "auto_impl",
+ "revm-interpreter",
+ "revm-precompile",
+]
+
+[[package]]
+name = "revm-interpreter"
+version = "1.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a53980a26f9b5a66d13511c35074d4b53631e157850a1d7cf1af4efc2c2b72c9"
+dependencies = [
+ "derive_more",
+ "enumn",
+ "revm-primitives",
+ "sha3",
+]
+
+[[package]]
+name = "revm-precompile"
+version = "2.0.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "41320af3bd6a65153d38eb1d3638ba89104cc9513c7feedb2d8510e8307dab29"
+dependencies = [
+ "k256",
+ "num",
+ "once_cell",
+ "revm-primitives",
+ "ripemd",
+ "secp256k1",
+ "sha2",
+ "sha3",
+ "substrate-bn",
+]
+
+[[package]]
 name = "revm-primitives"
 version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "304d998f466ffef72d76c7f20b05bf08a96801736a6fb1fdef47d49a292618df"
 dependencies = [
  "auto_impl",
  "bitvec",
@@ -2059,14 +2236,23 @@
 checksum = "f8dd2a808d456c4a54e300a23e9f5a67e122c3024119acbfd73e3bf664491cb2"
 dependencies = [
  "hmac",
  "subtle",
 ]
 
 [[package]]
+name = "ripemd"
+version = "0.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bd124222d17ad93a644ed9d011a40f4fb64aa54275c08cc216524a9ea82fb09f"
+dependencies = [
+ "digest",
+]
+
+[[package]]
 name = "rlp"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bb919243f34364b6bd2fc10ef797edbfa75f33c252e7998527479c6d6b47e1ec"
 dependencies = [
  "bytes",
  "rlp-derive",
@@ -2130,55 +2316,55 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.37.21"
+version = "0.37.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62f25693a73057a1b4cb56179dd3c7ea21a7c6c5ee7d85781f5749b46f34b79c"
+checksum = "4d69718bf81c6127a49dc64e44a742e8bb9213c0ff8869a22c308f84c1d4ab06"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
  "windows-sys",
 ]
 
 [[package]]
 name = "rustversion"
-version = "1.0.12"
+version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f3208ce4d8448b3f3e7d168a73f5e0c43a61e32930de3bceeccedb388b6bf06"
+checksum = "dc31bd9b61a32c31f9650d18add92aa83a49ba979c143eefd27fe7177b05bd5f"
 
 [[package]]
 name = "ryu"
-version = "1.0.13"
+version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
+checksum = "fe232bdf6be8c8de797b22184ee71118d63780ea42ac85b61d1baa6d3b782ae9"
 
 [[package]]
 name = "scale-info"
-version = "2.8.0"
+version = "2.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ad560913365790f17cbf12479491169f01b9d46d29cfc7422bf8c64bdc61b731"
+checksum = "35c0a159d0c45c12b20c5a844feb1fe4bea86e28f17b92a5f0c42193634d3782"
 dependencies = [
  "cfg-if",
  "derive_more",
  "parity-scale-codec",
  "scale-info-derive",
 ]
 
 [[package]]
 name = "scale-info-derive"
-version = "2.8.0"
+version = "2.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "19df9bd9ace6cc2fe19387c96ce677e823e07d017ceed253e7bb3d1d1bd9c73b"
+checksum = "912e55f6d20e0e80d63733872b40e1227c0bce1e1ab81ba67d696339bfd7fd29"
 dependencies = [
  "proc-macro-crate",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
@@ -2225,37 +2411,37 @@
 name = "semver"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
 
 [[package]]
 name = "serde"
-version = "1.0.164"
+version = "1.0.166"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
+checksum = "d01b7404f9d441d3ad40e6a636a7782c377d2abdbe4fa2440e2edcc2f4f10db8"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.164"
+version = "1.0.166"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
+checksum = "5dd83d6dde2b6b2d466e14d9d1acce8816dedee94f735eac6395808b3483c6d6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.99"
+version = "1.0.100"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46266871c240a00b8f503b877622fe33430b3c7d963bdc0f2adc511e54a1eae3"
+checksum = "0f1e14e89be7aa4c4b78bdbdc9eb5bf8517829a600ae8eaa39a6e1d960b5185c"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -2279,15 +2465,15 @@
 version = "2.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "881b6f881b17d13214e5d494c939ebab463d01264ce1811e9d4ac3a882e7695f"
 dependencies = [
  "darling",
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "sha2"
 version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "479fb9d862239e610720565ca91403019f2f00410f1864c5aa7479b950a76ed8"
@@ -2339,17 +2525,17 @@
 checksum = "6528351c9bc8ab22353f9d776db39a20288e8d6c37ef8cfe3317cf875eecfc2d"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "smol_str"
 version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fad6c857cbab2627dcf01ec85a623ca4e7dcb5691cbaa3d7fb7653671f0d09c9"
 dependencies = [
@@ -2370,14 +2556,20 @@
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "spin"
+version = "0.5.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6e63cff320ae2c57904679ba7cb63280a3dc4613885beafb148ee7bf9aa9042d"
+
+[[package]]
+name = "spin"
 version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
 dependencies = [
  "lock_api",
 ]
 
@@ -2428,14 +2620,27 @@
  "proc-macro2",
  "quote",
  "rustversion",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "substrate-bn"
+version = "0.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "72b5bbfa79abbae15dd642ea8176a21a635ff3c00059961d1ea27ad04e5b441c"
+dependencies = [
+ "byteorder",
+ "crunchy",
+ "lazy_static",
+ "rand",
+ "rustc-hex",
+]
+
+[[package]]
 name = "subtle"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
 
 [[package]]
 name = "sucds"
@@ -2455,17 +2660,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.22"
+version = "2.0.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2efbeae7acf4eabd6bcdcbd11c92f45231ddda7539edc7806bd1a04a03b24616"
+checksum = "59fb7d6d8281a51045d62b8eb3a7d1ce347b76f312af50cd3dc0af39c87c1737"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -2492,39 +2697,41 @@
  "redox_syscall",
  "rustix",
  "windows-sys",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.40"
+version = "1.0.41"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
+checksum = "c16a64ba9387ef3fdae4f9c1a7f07a0997fce91985c0336f1ddc1822b3b37802"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.40"
+version = "1.0.41"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
+checksum = "d14928354b01c4d6a4f0e549069adef399a284e7995c7ccca94e8a07a5346c59"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "time"
 version = "0.3.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ea9e1b3cf1243ae005d9e74085d4d542f3125458f3a81af210d901dcd7411efd"
 dependencies = [
  "itoa",
+ "libc",
+ "num_threads",
  "serde",
  "time-core",
  "time-macros",
 ]
 
 [[package]]
 name = "time-core"
@@ -2589,26 +2796,27 @@
 name = "tokio-macros"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "tokio-stream"
 version = "0.1.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "397c988d37662c7dda6d2208364a706264bf3d6138b11d436cbac0ad38832842"
 dependencies = [
  "futures-core",
  "pin-project-lite",
  "tokio",
+ "tokio-util",
 ]
 
 [[package]]
 name = "tokio-util"
 version = "0.7.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "806fe8c2c87eccc8b3267cbae29ed3ab2d0bd37fca70ab622e46aaa9375ddb7d"
@@ -2625,17 +2833,17 @@
 name = "toml_datetime"
 version = "0.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7cda73e2f1397b1262d6dfdcef8aafae14d1de7748d66822d3bfeeb6d03e5e4b"
 
 [[package]]
 name = "toml_edit"
-version = "0.19.11"
+version = "0.19.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "266f016b7f039eec8a1a80dfe6156b633d208b9fccca5e4db1d6775b0c4e34a7"
+checksum = "c500344a19072298cd05a7224b3c0c629348b78692bf48466c5238656e315a78"
 dependencies = [
  "indexmap 2.0.0",
  "toml_datetime",
  "winnow",
 ]
 
 [[package]]
@@ -2654,15 +2862,15 @@
 name = "tracing-attributes"
 version = "0.1.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5f4f31f56159e98206da9efd823404b79b6ef3143b4a7ab76e67b1751b25a4ab"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
@@ -2702,17 +2910,17 @@
 name = "unicode-bidi"
 version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.9"
+version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
+checksum = "22049a19f4a68748a168c0fc439f9516686aa045927ff767eca0a85101fb6e73"
 
 [[package]]
 name = "unicode-normalization"
 version = "0.1.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
 dependencies = [
@@ -2746,17 +2954,17 @@
  "form_urlencoded",
  "idna",
  "percent-encoding",
 ]
 
 [[package]]
 name = "vergen"
-version = "8.2.1"
+version = "8.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8b3c89c2c7e50f33e4d35527e5bf9c11d6d132226dbbd1753f0fbe9f19ef88c6"
+checksum = "bbc5ad0d9d26b2c49a5ab7da76c3e79d3ee37e7821799f8223fcb8f2f391a2e7"
 dependencies = [
  "anyhow",
  "rustversion",
  "time",
 ]
 
 [[package]]
@@ -2788,15 +2996,15 @@
 checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.23",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2810,15 +3018,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.23",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.87"
```

