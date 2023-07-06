# Comparing `tmp/snowpark_session-0.1.0.tar.gz` & `tmp/snowpark_session-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowpark_session-0.1.0.tar", max compression
+gzip compressed data, was "snowpark_session-0.1.1.tar", max compression
```

## Comparing `snowpark_session-0.1.0.tar` & `snowpark_session-0.1.1.tar`

### file list

```diff
@@ -1,79 +1,81 @@
--rw-r--r--   0        0        0      132 2023-06-29 04:22:34.900454 snowpark_session-0.1.0/.git/FETCH_HEAD
--rw-r--r--   0        0        0       21 2023-06-29 04:22:34.912455 snowpark_session-0.1.0/.git/HEAD
--rw-r--r--   0        0        0      421 2023-06-29 04:22:34.912455 snowpark_session-0.1.0/.git/config
--rwxr-xr-x   0        0        0       73 2023-06-29 04:22:34.388441 snowpark_session-0.1.0/.git/description
--rwxr-xr-x   0        0        0      478 2023-06-29 04:22:34.384441 snowpark_session-0.1.0/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0        0        0      896 2023-06-29 04:22:34.388441 snowpark_session-0.1.0/.git/hooks/commit-msg.sample
--rwxr-xr-x   0        0        0     4726 2023-06-29 04:22:34.388441 snowpark_session-0.1.0/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0        0        0      189 2023-06-29 04:22:34.388441 snowpark_session-0.1.0/.git/hooks/post-update.sample
--rwxr-xr-x   0        0        0      424 2023-06-29 04:22:34.388441 snowpark_session-0.1.0/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0        0        0     1643 2023-06-29 04:22:34.388441 snowpark_session-0.1.0/.git/hooks/pre-commit.sample
--rwxr-xr-x   0        0        0      416 2023-06-29 04:22:34.388441 snowpark_session-0.1.0/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0        0        0     1374 2023-06-29 04:22:34.388441 snowpark_session-0.1.0/.git/hooks/pre-push.sample
--rwxr-xr-x   0        0        0     4898 2023-06-29 04:22:34.384441 snowpark_session-0.1.0/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0        0        0      544 2023-06-29 04:22:34.388441 snowpark_session-0.1.0/.git/hooks/pre-receive.sample
--rwxr-xr-x   0        0        0     1492 2023-06-29 04:22:34.388441 snowpark_session-0.1.0/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0        0        0     2783 2023-06-29 04:22:34.388441 snowpark_session-0.1.0/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0        0        0     2308 2023-06-29 04:22:34.388441 snowpark_session-0.1.0/.git/hooks/sendemail-validate.sample
--rwxr-xr-x   0        0        0     3650 2023-06-29 04:22:34.388441 snowpark_session-0.1.0/.git/hooks/update.sample
--rw-r--r--   0        0        0     2036 2023-06-29 04:22:34.912455 snowpark_session-0.1.0/.git/index
--rwxr-xr-x   0        0        0      240 2023-06-29 04:22:34.384441 snowpark_session-0.1.0/.git/info/exclude
--rw-r--r--   0        0        0      217 2023-06-29 04:22:34.912455 snowpark_session-0.1.0/.git/logs/HEAD
--rw-r--r--   0        0        0      226 2023-06-29 04:22:34.912455 snowpark_session-0.1.0/.git/logs/refs/heads/main
--rw-r--r--   0        0        0      336 2023-06-29 04:22:34.900454 snowpark_session-0.1.0/.git/logs/refs/remotes/origin/main
--rw-r--r--   0        0        0      322 2023-06-29 04:22:34.880454 snowpark_session-0.1.0/.git/objects/03/4e848032092eaf8ef96eac731b6ed5961987f3
--rw-r--r--   0        0        0     1393 2023-06-29 04:22:34.876454 snowpark_session-0.1.0/.git/objects/14/446eee817b1c0bab80e209dcfb0e5d08707eb2
--rw-r--r--   0        0        0      388 2023-06-29 04:22:34.876454 snowpark_session-0.1.0/.git/objects/14/584c967384924df013583d2d15fd5b16262832
--rw-r--r--   0        0        0      578 2023-06-29 04:22:34.880454 snowpark_session-0.1.0/.git/objects/23/5f8dd1de8e46360557cc68b63dce1ad592f89f
--rw-r--r--   0        0        0       82 2023-06-29 04:22:34.896454 snowpark_session-0.1.0/.git/objects/24/eab5e15c1b0ca711315422777797afa4386411
--rw-r--r--   0        0        0     1294 2023-06-29 04:22:34.896454 snowpark_session-0.1.0/.git/objects/2b/666086c9de37553886a4b26d75310b117305d6
--rw-r--r--   0        0        0       38 2023-06-29 04:22:34.896454 snowpark_session-0.1.0/.git/objects/3d/c1f76bc69e3f559bee6253b24fc93acee9e1f9
--rw-r--r--   0        0        0     2149 2023-06-29 04:22:34.876454 snowpark_session-0.1.0/.git/objects/58/299f512aa9e532cc8695ca7ad5e2e48d976d43
--rw-r--r--   0        0        0      675 2023-06-29 04:22:34.876454 snowpark_session-0.1.0/.git/objects/6c/a8426bc395952c8514daf4a1f69db45be11700
--rw-r--r--   0        0        0      264 2023-06-29 04:22:34.880454 snowpark_session-0.1.0/.git/objects/6f/b0748c2f1fba135d1763e049cac49f6c8b734f
--rw-r--r--   0        0        0       41 2023-06-29 04:22:34.880454 snowpark_session-0.1.0/.git/objects/71/7ab457193f390f8fe9648f29ede3e4d3cc42d9
--rw-r--r--   0        0        0      329 2023-06-29 04:22:34.896454 snowpark_session-0.1.0/.git/objects/8d/8b8292475860cfc2137fe0ac357a5012de0cb0
--rw-r--r--   0        0        0      665 2023-06-29 04:22:34.880454 snowpark_session-0.1.0/.git/objects/94/eacce9677d11bbd9dfba2f044adb38bb447845
--rw-r--r--   0        0        0      789 2023-06-29 04:22:34.876454 snowpark_session-0.1.0/.git/objects/99/86bf80f28944c4ca25ac70806d69e0e6b07692
--rw-r--r--   0        0        0    34428 2023-06-29 04:22:34.896454 snowpark_session-0.1.0/.git/objects/a4/5d60a15129fdfb2ba654740529c92edfcf6419
--rw-r--r--   0        0        0      136 2023-06-29 04:22:34.880454 snowpark_session-0.1.0/.git/objects/a5/4b33eb107873280680b274e0f0c48e60e70bc0
--rw-r--r--   0        0        0      129 2023-06-29 04:22:34.896454 snowpark_session-0.1.0/.git/objects/a9/b17f44eee3e56f8eeaf799d7a0d1ba9da1df26
--rw-r--r--   0        0        0       83 2023-06-29 04:22:34.876454 snowpark_session-0.1.0/.git/objects/ac/260f43d40317792366ba48f7bedf1132cf8bdc
--rw-r--r--   0        0        0       26 2023-06-29 04:22:34.880454 snowpark_session-0.1.0/.git/objects/bb/87656e2e4cb6e1c10750b8bc02aef5600bf899
--rw-r--r--   0        0        0     1572 2023-06-29 04:22:34.876454 snowpark_session-0.1.0/.git/objects/d1/9e2c2c707e5abd11a270fa04a60c14414750d7
--rw-r--r--   0        0        0     3944 2023-06-29 04:22:34.880454 snowpark_session-0.1.0/.git/objects/d3/a3410b3d1e6422a6e17a121d28c14913264c44
--rw-r--r--   0        0        0     1285 2023-06-29 04:22:34.896454 snowpark_session-0.1.0/.git/objects/d3/effead825f365d31539fb24c9c8e0dbb39949c
--rw-r--r--   0        0        0      239 2023-06-29 04:22:34.880454 snowpark_session-0.1.0/.git/objects/e3/9680a4340a55826e5adbe20e7215b60f3a0399
--rw-r--r--   0        0        0       82 2023-06-29 04:22:34.880454 snowpark_session-0.1.0/.git/objects/e5/ebc7b54f2c9b974961ad088cc5ef70799acff1
--rw-r--r--   0        0        0       15 2023-06-29 04:22:34.880454 snowpark_session-0.1.0/.git/objects/e6/9de29bb2d1d6434b8b29ae775ad8c2e48c5391
--rw-r--r--   0        0        0      869 2023-06-29 04:22:34.876454 snowpark_session-0.1.0/.git/objects/f3/b6cff04f053b938b2380803d8e81744fb01f8d
--rw-r--r--   0        0        0       56 2023-06-29 04:22:34.876454 snowpark_session-0.1.0/.git/objects/fc/e262124261545357747b4e5682f26a123a81bb
--rw-r--r--   0        0        0       51 2023-06-29 04:22:34.876454 snowpark_session-0.1.0/.git/objects/fe/2f413f569299278261009c9048d591eda8cd48
--rw-r--r--   0        0        0       41 2023-06-29 04:22:34.912455 snowpark_session-0.1.0/.git/refs/heads/main
--rw-r--r--   0        0        0       41 2023-06-29 04:22:34.900454 snowpark_session-0.1.0/.git/refs/remotes/origin/main
--rw-r--r--   0        0        0       41 2023-06-29 04:22:34.852453 snowpark_session-0.1.0/.git/shallow
--rw-r--r--   0        0        0       44 2023-06-29 04:22:34.908455 snowpark_session-0.1.0/.gitcommit
--rw-r--r--   0        0        0     1665 2023-06-29 04:22:34.908455 snowpark_session-0.1.0/.github/workflows/python-cd.yml
--rw-r--r--   0        0        0     3282 2023-06-29 04:22:34.908455 snowpark_session-0.1.0/.github/workflows/python-ci.yml
--rw-r--r--   0        0        0     3127 2023-06-29 04:22:34.908455 snowpark_session-0.1.0/.gitignore
--rw-r--r--   0        0        0      796 2023-06-29 04:22:34.908455 snowpark_session-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     4404 2023-06-29 04:22:34.908455 snowpark_session-0.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     9084 2023-06-29 04:22:34.908455 snowpark_session-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1083 2023-06-29 04:22:34.908455 snowpark_session-0.1.0/LICENSE
--rw-r--r--   0        0        0       10 2023-06-29 04:22:34.912455 snowpark_session-0.1.0/MANIFEST.in
--rw-r--r--   0        0        0      497 2023-06-29 04:22:34.912455 snowpark_session-0.1.0/Makefile
--rw-r--r--   0        0        0     1218 2023-06-29 04:22:34.912455 snowpark_session-0.1.0/README.md
--rw-r--r--   0        0        0      619 2023-06-29 04:22:34.912455 snowpark_session-0.1.0/SECURITY.md
--rw-r--r--   0        0        0      201 2023-06-29 04:22:34.912455 snowpark_session-0.1.0/environment.yml
--rw-r--r--   0        0        0      545 2023-06-29 04:22:34.912455 snowpark_session-0.1.0/it.py
--rw-r--r--   0        0        0       73 2023-06-29 04:22:34.912455 snowpark_session-0.1.0/main.py
--rw-r--r--   0        0        0       25 2023-06-29 04:22:34.912455 snowpark_session-0.1.0/package.json
--rw-r--r--   0        0        0        0 2023-06-29 04:22:34.912455 snowpark_session-0.1.0/pip.conf
--rw-r--r--   0        0        0    99739 2023-06-29 04:22:34.912455 snowpark_session-0.1.0/poetry.lock
--rw-r--r--   0        0        0      504 2023-06-29 04:22:34.912455 snowpark_session-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      145 2023-06-29 04:22:34.912455 snowpark_session-0.1.0/requirements.txt
--rw-r--r--   0        0        0       66 2023-06-29 04:22:34.912455 snowpark_session-0.1.0/setup.cfg
--rw-r--r--   0        0        0     3130 2023-06-29 04:22:34.912455 snowpark_session-0.1.0/setup.py
--rw-r--r--   0        0        0     4441 2023-06-29 04:22:34.912455 snowpark_session-0.1.0/snowpark_session.py
--rw-r--r--   0        0        0       22 2023-06-29 04:22:34.912455 snowpark_session-0.1.0/version.py
--rw-r--r--   0        0        0     1835 1970-01-01 00:00:00.000000 snowpark_session-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      132 2023-07-06 20:14:09.834721 snowpark_session-0.1.1/.git/FETCH_HEAD
+-rw-r--r--   0        0        0       21 2023-07-06 20:14:09.846721 snowpark_session-0.1.1/.git/HEAD
+-rw-r--r--   0        0        0      421 2023-07-06 20:14:09.846721 snowpark_session-0.1.1/.git/config
+-rwxr-xr-x   0        0        0       73 2023-07-06 20:14:09.358715 snowpark_session-0.1.1/.git/description
+-rwxr-xr-x   0        0        0      478 2023-07-06 20:14:09.358715 snowpark_session-0.1.1/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0        0        0      896 2023-07-06 20:14:09.358715 snowpark_session-0.1.1/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0        0        0     4726 2023-07-06 20:14:09.358715 snowpark_session-0.1.1/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0        0        0      189 2023-07-06 20:14:09.358715 snowpark_session-0.1.1/.git/hooks/post-update.sample
+-rwxr-xr-x   0        0        0      424 2023-07-06 20:14:09.358715 snowpark_session-0.1.1/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0        0        0     1643 2023-07-06 20:14:09.362715 snowpark_session-0.1.1/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0        0        0      416 2023-07-06 20:14:09.358715 snowpark_session-0.1.1/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0        0        0     1374 2023-07-06 20:14:09.358715 snowpark_session-0.1.1/.git/hooks/pre-push.sample
+-rwxr-xr-x   0        0        0     4898 2023-07-06 20:14:09.362715 snowpark_session-0.1.1/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0        0        0      544 2023-07-06 20:14:09.358715 snowpark_session-0.1.1/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0        0        0     1492 2023-07-06 20:14:09.358715 snowpark_session-0.1.1/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0        0        0     2783 2023-07-06 20:14:09.358715 snowpark_session-0.1.1/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0        0        0     2308 2023-07-06 20:14:09.358715 snowpark_session-0.1.1/.git/hooks/sendemail-validate.sample
+-rwxr-xr-x   0        0        0     3650 2023-07-06 20:14:09.358715 snowpark_session-0.1.1/.git/hooks/update.sample
+-rw-r--r--   0        0        0     2173 2023-07-06 20:14:09.846721 snowpark_session-0.1.1/.git/index
+-rwxr-xr-x   0        0        0      240 2023-07-06 20:14:09.358715 snowpark_session-0.1.1/.git/info/exclude
+-rw-r--r--   0        0        0      217 2023-07-06 20:14:09.846721 snowpark_session-0.1.1/.git/logs/HEAD
+-rw-r--r--   0        0        0      226 2023-07-06 20:14:09.846721 snowpark_session-0.1.1/.git/logs/refs/heads/main
+-rw-r--r--   0        0        0      336 2023-07-06 20:14:09.834721 snowpark_session-0.1.1/.git/logs/refs/remotes/origin/main
+-rw-r--r--   0        0        0      322 2023-07-06 20:14:09.806720 snowpark_session-0.1.1/.git/objects/03/4e848032092eaf8ef96eac731b6ed5961987f3
+-rw-r--r--   0        0        0      676 2023-07-06 20:14:09.794720 snowpark_session-0.1.1/.git/objects/0f/1b0a7f829f051435b5ae3057ab5c4462e20df4
+-rw-r--r--   0        0        0     1393 2023-07-06 20:14:09.794720 snowpark_session-0.1.1/.git/objects/14/446eee817b1c0bab80e209dcfb0e5d08707eb2
+-rw-r--r--   0        0        0      578 2023-07-06 20:14:09.806720 snowpark_session-0.1.1/.git/objects/23/5f8dd1de8e46360557cc68b63dce1ad592f89f
+-rw-r--r--   0        0        0       82 2023-07-06 20:14:09.830721 snowpark_session-0.1.1/.git/objects/24/eab5e15c1b0ca711315422777797afa4386411
+-rw-r--r--   0        0        0     1294 2023-07-06 20:14:09.830721 snowpark_session-0.1.1/.git/objects/2b/666086c9de37553886a4b26d75310b117305d6
+-rw-r--r--   0        0        0       38 2023-07-06 20:14:09.830721 snowpark_session-0.1.1/.git/objects/48/5f44ac21b2ee78a2ee1ed0ea584114a1c957c3
+-rw-r--r--   0        0        0      817 2023-07-06 20:14:09.794720 snowpark_session-0.1.1/.git/objects/4a/65c9934f763497f4fe7a8dcc04257bec34584b
+-rw-r--r--   0        0        0     2149 2023-07-06 20:14:09.798720 snowpark_session-0.1.1/.git/objects/58/299f512aa9e532cc8695ca7ad5e2e48d976d43
+-rw-r--r--   0        0        0     1296 2023-07-06 20:14:09.830721 snowpark_session-0.1.1/.git/objects/67/80bc4d83bf0662401e0e2c42871b2c45b6fe74
+-rw-r--r--   0        0        0      264 2023-07-06 20:14:09.806720 snowpark_session-0.1.1/.git/objects/6f/b0748c2f1fba135d1763e049cac49f6c8b734f
+-rw-r--r--   0        0        0       41 2023-07-06 20:14:09.806720 snowpark_session-0.1.1/.git/objects/71/7ab457193f390f8fe9648f29ede3e4d3cc42d9
+-rw-r--r--   0        0        0      476 2023-07-06 20:14:09.798720 snowpark_session-0.1.1/.git/objects/7e/61656297b5b1a6bb4d7deafd3e123078bb8e3c
+-rw-r--r--   0        0        0      665 2023-07-06 20:14:09.806720 snowpark_session-0.1.1/.git/objects/94/eacce9677d11bbd9dfba2f044adb38bb447845
+-rw-r--r--   0        0        0       55 2023-07-06 20:14:09.794720 snowpark_session-0.1.1/.git/objects/9d/0569021c8442ef52179a5900c4cbbbb375000a
+-rw-r--r--   0        0        0      136 2023-07-06 20:14:09.806720 snowpark_session-0.1.1/.git/objects/a5/4b33eb107873280680b274e0f0c48e60e70bc0
+-rw-r--r--   0        0        0      129 2023-07-06 20:14:09.830721 snowpark_session-0.1.1/.git/objects/a9/b17f44eee3e56f8eeaf799d7a0d1ba9da1df26
+-rw-r--r--   0        0        0       83 2023-07-06 20:14:09.794720 snowpark_session-0.1.1/.git/objects/ac/260f43d40317792366ba48f7bedf1132cf8bdc
+-rw-r--r--   0        0        0       26 2023-07-06 20:14:09.806720 snowpark_session-0.1.1/.git/objects/bb/87656e2e4cb6e1c10750b8bc02aef5600bf899
+-rw-r--r--   0        0        0     1572 2023-07-06 20:14:09.798720 snowpark_session-0.1.1/.git/objects/d1/9e2c2c707e5abd11a270fa04a60c14414750d7
+-rw-r--r--   0        0        0     3944 2023-07-06 20:14:09.806720 snowpark_session-0.1.1/.git/objects/d3/a3410b3d1e6422a6e17a121d28c14913264c44
+-rw-r--r--   0        0        0      341 2023-07-06 20:14:09.830721 snowpark_session-0.1.1/.git/objects/e0/9ba6a715eb48c48853c199b04cc81ac6935f41
+-rw-r--r--   0        0        0      239 2023-07-06 20:14:09.806720 snowpark_session-0.1.1/.git/objects/e3/9680a4340a55826e5adbe20e7215b60f3a0399
+-rw-r--r--   0        0        0       82 2023-07-06 20:14:09.806720 snowpark_session-0.1.1/.git/objects/e5/ebc7b54f2c9b974961ad088cc5ef70799acff1
+-rw-r--r--   0        0        0       15 2023-07-06 20:14:09.806720 snowpark_session-0.1.1/.git/objects/e6/9de29bb2d1d6434b8b29ae775ad8c2e48c5391
+-rw-r--r--   0        0        0    37000 2023-07-06 20:14:09.826721 snowpark_session-0.1.1/.git/objects/f0/b5172123cc520afd0a8feb4b6c09c2a6ba6c34
+-rw-r--r--   0        0        0      869 2023-07-06 20:14:09.794720 snowpark_session-0.1.1/.git/objects/f3/b6cff04f053b938b2380803d8e81744fb01f8d
+-rw-r--r--   0        0        0       56 2023-07-06 20:14:09.794720 snowpark_session-0.1.1/.git/objects/fc/e262124261545357747b4e5682f26a123a81bb
+-rw-r--r--   0        0        0       51 2023-07-06 20:14:09.794720 snowpark_session-0.1.1/.git/objects/fe/2f413f569299278261009c9048d591eda8cd48
+-rw-r--r--   0        0        0       41 2023-07-06 20:14:09.846721 snowpark_session-0.1.1/.git/refs/heads/main
+-rw-r--r--   0        0        0       41 2023-07-06 20:14:09.834721 snowpark_session-0.1.1/.git/refs/remotes/origin/main
+-rw-r--r--   0        0        0       41 2023-07-06 20:14:09.762720 snowpark_session-0.1.1/.git/shallow
+-rw-r--r--   0        0        0       44 2023-07-06 20:14:09.842721 snowpark_session-0.1.1/.gitcommit
+-rw-r--r--   0        0        0     1665 2023-07-06 20:14:09.842721 snowpark_session-0.1.1/.github/workflows/python-cd.yml
+-rw-r--r--   0        0        0     3282 2023-07-06 20:14:09.842721 snowpark_session-0.1.1/.github/workflows/python-ci.yml
+-rw-r--r--   0        0        0     3127 2023-07-06 20:14:09.842721 snowpark_session-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1059 2023-07-06 20:14:09.842721 snowpark_session-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     4404 2023-07-06 20:14:09.842721 snowpark_session-0.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     9084 2023-07-06 20:14:09.842721 snowpark_session-0.1.1/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1083 2023-07-06 20:14:09.842721 snowpark_session-0.1.1/LICENSE
+-rw-r--r--   0        0        0       10 2023-07-06 20:14:09.842721 snowpark_session-0.1.1/MANIFEST.in
+-rw-r--r--   0        0        0      497 2023-07-06 20:14:09.842721 snowpark_session-0.1.1/Makefile
+-rw-r--r--   0        0        0     1218 2023-07-06 20:14:09.842721 snowpark_session-0.1.1/README.md
+-rw-r--r--   0        0        0      619 2023-07-06 20:14:09.842721 snowpark_session-0.1.1/SECURITY.md
+-rw-r--r--   0        0        0      201 2023-07-06 20:14:09.842721 snowpark_session-0.1.1/environment.yml
+-rw-r--r--   0        0        0      545 2023-07-06 20:14:09.842721 snowpark_session-0.1.1/it.py
+-rw-r--r--   0        0        0       73 2023-07-06 20:14:09.842721 snowpark_session-0.1.1/main.py
+-rw-r--r--   0        0        0       25 2023-07-06 20:14:09.842721 snowpark_session-0.1.1/package.json
+-rw-r--r--   0        0        0        0 2023-07-06 20:14:09.842721 snowpark_session-0.1.1/pip.conf
+-rw-r--r--   0        0        0   106697 2023-07-06 20:14:09.842721 snowpark_session-0.1.1/poetry.lock
+-rw-r--r--   0        0        0      531 2023-07-06 20:14:09.842721 snowpark_session-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      145 2023-07-06 20:14:09.842721 snowpark_session-0.1.1/requirements.txt
+-rw-r--r--   0        0        0       66 2023-07-06 20:14:09.842721 snowpark_session-0.1.1/setup.cfg
+-rw-r--r--   0        0        0     3130 2023-07-06 20:14:09.842721 snowpark_session-0.1.1/setup.py
+-rw-r--r--   0        0        0     4423 2023-07-06 20:14:09.842721 snowpark_session-0.1.1/snowpark_session/__init__.py
+-rw-r--r--   0        0        0     4423 2023-07-06 20:14:09.842721 snowpark_session-0.1.1/snowpark_session.py
+-rw-r--r--   0        0        0       22 2023-07-06 20:14:09.846721 snowpark_session-0.1.1/version.py
+-rw-r--r--   0        0        0     1883 1970-01-01 00:00:00.000000 snowpark_session-0.1.1/PKG-INFO
```

### Comparing `snowpark_session-0.1.0/.git/hooks/commit-msg.sample` & `snowpark_session-0.1.1/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `snowpark_session-0.1.0/.git/hooks/fsmonitor-watchman.sample` & `snowpark_session-0.1.1/.git/hooks/fsmonitor-watchman.sample`

 * *Files identical despite different names*

### Comparing `snowpark_session-0.1.0/.git/hooks/pre-commit.sample` & `snowpark_session-0.1.1/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `snowpark_session-0.1.0/.git/hooks/pre-push.sample` & `snowpark_session-0.1.1/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `snowpark_session-0.1.0/.git/hooks/pre-rebase.sample` & `snowpark_session-0.1.1/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `snowpark_session-0.1.0/.git/hooks/pre-receive.sample` & `snowpark_session-0.1.1/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `snowpark_session-0.1.0/.git/hooks/prepare-commit-msg.sample` & `snowpark_session-0.1.1/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `snowpark_session-0.1.0/.git/hooks/push-to-checkout.sample` & `snowpark_session-0.1.1/.git/hooks/push-to-checkout.sample`

 * *Files identical despite different names*

### Comparing `snowpark_session-0.1.0/.git/hooks/sendemail-validate.sample` & `snowpark_session-0.1.1/.git/hooks/sendemail-validate.sample`

 * *Files identical despite different names*

### Comparing `snowpark_session-0.1.0/.git/hooks/update.sample` & `snowpark_session-0.1.1/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `snowpark_session-0.1.0/.git/objects/14/446eee817b1c0bab80e209dcfb0e5d08707eb2` & `snowpark_session-0.1.1/.git/objects/14/446eee817b1c0bab80e209dcfb0e5d08707eb2`

 * *Files identical despite different names*

### Comparing `snowpark_session-0.1.0/.git/objects/23/5f8dd1de8e46360557cc68b63dce1ad592f89f` & `snowpark_session-0.1.1/.git/objects/23/5f8dd1de8e46360557cc68b63dce1ad592f89f`

 * *Files identical despite different names*

### Comparing `snowpark_session-0.1.0/.git/objects/2b/666086c9de37553886a4b26d75310b117305d6` & `snowpark_session-0.1.1/.git/objects/2b/666086c9de37553886a4b26d75310b117305d6`

 * *Files identical despite different names*

### Comparing `snowpark_session-0.1.0/.git/objects/58/299f512aa9e532cc8695ca7ad5e2e48d976d43` & `snowpark_session-0.1.1/.git/objects/58/299f512aa9e532cc8695ca7ad5e2e48d976d43`

 * *Files identical despite different names*

### Comparing `snowpark_session-0.1.0/.git/objects/94/eacce9677d11bbd9dfba2f044adb38bb447845` & `snowpark_session-0.1.1/.git/objects/94/eacce9677d11bbd9dfba2f044adb38bb447845`

 * *Files identical despite different names*

### Comparing `snowpark_session-0.1.0/.git/objects/d1/9e2c2c707e5abd11a270fa04a60c14414750d7` & `snowpark_session-0.1.1/.git/objects/d1/9e2c2c707e5abd11a270fa04a60c14414750d7`

 * *Files identical despite different names*

### Comparing `snowpark_session-0.1.0/.git/objects/d3/a3410b3d1e6422a6e17a121d28c14913264c44` & `snowpark_session-0.1.1/.git/objects/d3/a3410b3d1e6422a6e17a121d28c14913264c44`

 * *Files identical despite different names*

### Comparing `snowpark_session-0.1.0/.git/objects/f3/b6cff04f053b938b2380803d8e81744fb01f8d` & `snowpark_session-0.1.1/.git/objects/f3/b6cff04f053b938b2380803d8e81744fb01f8d`

 * *Files identical despite different names*

### Comparing `snowpark_session-0.1.0/.github/workflows/python-cd.yml` & `snowpark_session-0.1.1/.github/workflows/python-cd.yml`

 * *Files identical despite different names*

### Comparing `snowpark_session-0.1.0/.github/workflows/python-ci.yml` & `snowpark_session-0.1.1/.github/workflows/python-ci.yml`

 * *Files identical despite different names*

### Comparing `snowpark_session-0.1.0/.gitignore` & `snowpark_session-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `snowpark_session-0.1.0/CHANGELOG.md` & `snowpark_session-0.1.1/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+## [0.1.1](https://github.com/Broomva/snowpark_session/compare/v0.1.0...v0.1.1) (2023-07-06)
+
+
+### Bug Fixes
+
+* corrected imports and spark session creation ([4a61673](https://github.com/Broomva/snowpark_session/commit/4a6167340c5ff751c08400b08bc67e3e8701112b))
+
 ## 0.1.0 (2023-06-29)
 
 
 ### Features
 
 * **init:** Initial snowpark_session commit ([81619bf](https://github.com/Broomva/snowpark_session/commit/81619bf8c45282e3fd031ef4f65728c9a853c827))
```

### Comparing `snowpark_session-0.1.0/CODE_OF_CONDUCT.md` & `snowpark_session-0.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `snowpark_session-0.1.0/CONTRIBUTING.rst` & `snowpark_session-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `snowpark_session-0.1.0/LICENSE` & `snowpark_session-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `snowpark_session-0.1.0/README.md` & `snowpark_session-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `snowpark_session-0.1.0/SECURITY.md` & `snowpark_session-0.1.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `snowpark_session-0.1.0/it.py` & `snowpark_session-0.1.1/it.py`

 * *Files identical despite different names*

### Comparing `snowpark_session-0.1.0/poetry.lock` & `snowpark_session-0.1.1/poetry.lock`

 * *Files 2% similar despite different names*

```diff
@@ -130,53 +130,45 @@
 ]
 
 [package.dependencies]
 azure-core = ">=1.26.2,<2.0.0"
 
 [[package]]
 name = "azure-storage-blob"
-version = "12.16.0"
+version = "12.13.0"
 description = "Microsoft Azure Blob Storage Client Library for Python"
 category = "main"
 optional = false
-python-versions = ">=3.7"
+python-versions = ">=3.6"
 files = [
-    {file = "azure-storage-blob-12.16.0.zip", hash = "sha256:43b45f19a518a5c6895632f263b3825ebc23574f25cc84b66e1630a6160e466f"},
-    {file = "azure_storage_blob-12.16.0-py3-none-any.whl", hash = "sha256:91bb192b2a97939c4259c72373bac0f41e30810bbc853d5184f0f45904eacafd"},
+    {file = "azure-storage-blob-12.13.0.zip", hash = "sha256:53f0d4cd32970ac9ff9b9753f83dd2fb3f9ac30e1d01e71638c436c509bfd884"},
+    {file = "azure_storage_blob-12.13.0-py3-none-any.whl", hash = "sha256:280a6ab032845bab9627582bee78a50497ca2f14772929b5c5ee8b4605af0cb3"},
 ]
 
 [package.dependencies]
-azure-core = ">=1.26.0,<2.0.0"
+azure-core = ">=1.23.1,<2.0.0"
 cryptography = ">=2.1.4"
-isodate = ">=0.6.1"
-typing-extensions = ">=4.0.1"
-
-[package.extras]
-aio = ["azure-core[aio] (>=1.26.0,<2.0.0)"]
+msrest = ">=0.6.21"
 
 [[package]]
 name = "azure-storage-file-datalake"
-version = "12.11.0"
+version = "12.8.0"
 description = "Microsoft Azure File DataLake Storage Client Library for Python"
 category = "main"
 optional = false
-python-versions = ">=3.7"
+python-versions = ">=3.6"
 files = [
-    {file = "azure-storage-file-datalake-12.11.0.zip", hash = "sha256:89b7556403c29ca5b6531c112f0e2d2ef3f340a9add553e8c3484a25bce6216c"},
-    {file = "azure_storage_file_datalake-12.11.0-py3-none-any.whl", hash = "sha256:0ebf00c7a54adc623e38673732dd07cf969f017024a597fc03631c0d1b9ed70f"},
+    {file = "azure-storage-file-datalake-12.8.0.zip", hash = "sha256:12e6306e5efb5ca28e0ccd9fa79a2c61acd589866d6109fe5601b18509da92f4"},
+    {file = "azure_storage_file_datalake-12.8.0-py3-none-any.whl", hash = "sha256:b6cf5733fe794bf3c866efbe3ce1941409e35b6b125028ac558b436bf90f2de7"},
 ]
 
 [package.dependencies]
-azure-core = ">=1.26.0,<2.0.0"
-azure-storage-blob = ">=12.16.0b1,<13.0.0"
-isodate = ">=0.6.1"
-typing-extensions = ">=4.0.1"
-
-[package.extras]
-aio = ["azure-core[aio] (>=1.26.0,<2.0.0)"]
+azure-core = ">=1.23.1,<2.0.0"
+azure-storage-blob = ">=12.13.0,<13.0.0"
+msrest = ">=0.6.21"
 
 [[package]]
 name = "azure-storage-file-share"
 version = "12.12.0"
 description = "Microsoft Azure Azure File Share Storage Client Library for Python"
 category = "main"
 optional = false
@@ -192,14 +184,40 @@
 isodate = ">=0.6.1"
 typing-extensions = ">=4.0.1"
 
 [package.extras]
 aio = ["azure-core[aio] (>=1.26.0,<2.0.0)"]
 
 [[package]]
+name = "azureml-mlflow"
+version = "1.52.0"
+description = "Contains the integration code of AzureML with Mlflow."
+category = "main"
+optional = false
+python-versions = ">=3.7,<4.0"
+files = [
+    {file = "azureml_mlflow-1.52.0-py3-none-any.whl", hash = "sha256:ca8b2f197108e2d8ad9661c25dc8220cfb092681824fbd9587d57152d7c238ee"},
+]
+
+[package.dependencies]
+azure-common = ">=1.1,<2.0.0"
+azure-core = ">=1.8.0,<1.22.0 || >1.22.0,<2.0.0"
+azure-identity = "*"
+azure-mgmt-core = ">=1.2.0,<2.0.0"
+azure-storage-blob = ">=12.5.0,<=12.13.0"
+cryptography = "*"
+jsonpickle = "*"
+mlflow-skinny = "*"
+msrest = ">=0.6.18"
+python-dateutil = ">=2.7.3,<3.0.0"
+
+[package.extras]
+deployments = ["flask", "numpy", "pandas"]
+
+[[package]]
 name = "black"
 version = "23.3.0"
 description = "The uncompromising code formatter."
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
@@ -431,15 +449,15 @@
     {file = "charset_normalizer-3.1.0-py3-none-any.whl", hash = "sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d"},
 ]
 
 [[package]]
 name = "click"
 version = "8.1.3"
 description = "Composable command line interface toolkit"
-category = "dev"
+category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "click-8.1.3-py3-none-any.whl", hash = "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"},
     {file = "click-8.1.3.tar.gz", hash = "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e"},
 ]
 
@@ -509,14 +527,47 @@
 sdist = ["setuptools-rust (>=0.11.4)"]
 ssh = ["bcrypt (>=3.1.5)"]
 test = ["iso8601", "pretend", "pytest (>=6.2.0)", "pytest-benchmark", "pytest-cov", "pytest-shard (>=0.1.2)", "pytest-subtests", "pytest-xdist"]
 test-randomorder = ["pytest-randomly"]
 tox = ["tox"]
 
 [[package]]
+name = "databricks-cli"
+version = "0.17.7"
+description = "A command line interface for Databricks"
+category = "main"
+optional = false
+python-versions = "*"
+files = [
+    {file = "databricks-cli-0.17.7.tar.gz", hash = "sha256:5a545063449f3b9ad904644c0f251058485e29e564dedf8d4e4a7b45caf9549b"},
+    {file = "databricks_cli-0.17.7-py2-none-any.whl", hash = "sha256:5b025943c70bbd374415264d38bfaddfb34ce070fadb083d851aec311e0f8901"},
+]
+
+[package.dependencies]
+click = ">=7.0"
+oauthlib = ">=3.1.0"
+pyjwt = ">=1.7.0"
+requests = ">=2.17.3"
+six = ">=1.10.0"
+tabulate = ">=0.7.7"
+urllib3 = ">=1.26.7,<2.0.0"
+
+[[package]]
+name = "entrypoints"
+version = "0.4"
+description = "Discover and load entry points from installed packages."
+category = "main"
+optional = false
+python-versions = ">=3.6"
+files = [
+    {file = "entrypoints-0.4-py3-none-any.whl", hash = "sha256:f174b5ff827504fd3cd97cc3f8649f3693f51538c7e4bdf3ef002c8429d42f9f"},
+    {file = "entrypoints-0.4.tar.gz", hash = "sha256:b706eddaa9218a19ebcd67b56818f05bb27589b1ca9e8d797b74affad4ccacd4"},
+]
+
+[[package]]
 name = "exceptiongroup"
 version = "1.1.1"
 description = "Backport of PEP 654 (exception groups)"
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
@@ -540,14 +591,44 @@
 ]
 
 [package.extras]
 docs = ["furo (>=2023.5.20)", "sphinx (>=7.0.1)", "sphinx-autodoc-typehints (>=1.23,!=1.23.4)"]
 testing = ["covdefaults (>=2.3)", "coverage (>=7.2.7)", "diff-cover (>=7.5)", "pytest (>=7.3.1)", "pytest-cov (>=4.1)", "pytest-mock (>=3.10)", "pytest-timeout (>=2.1)"]
 
 [[package]]
+name = "gitdb"
+version = "4.0.10"
+description = "Git Object Database"
+category = "main"
+optional = false
+python-versions = ">=3.7"
+files = [
+    {file = "gitdb-4.0.10-py3-none-any.whl", hash = "sha256:c286cf298426064079ed96a9e4a9d39e7f3e9bf15ba60701e95f5492f28415c7"},
+    {file = "gitdb-4.0.10.tar.gz", hash = "sha256:6eb990b69df4e15bad899ea868dc46572c3f75339735663b81de79b06f17eb9a"},
+]
+
+[package.dependencies]
+smmap = ">=3.0.1,<6"
+
+[[package]]
+name = "gitpython"
+version = "3.1.31"
+description = "GitPython is a Python library used to interact with Git repositories"
+category = "main"
+optional = false
+python-versions = ">=3.7"
+files = [
+    {file = "GitPython-3.1.31-py3-none-any.whl", hash = "sha256:f04893614f6aa713a60cbbe1e6a97403ef633103cdd0ef5eb6efe0deb98dbe8d"},
+    {file = "GitPython-3.1.31.tar.gz", hash = "sha256:8ce3bcf69adfdf7c7d503e78fd3b1c492af782d58893b650adb2ac8912ddd573"},
+]
+
+[package.dependencies]
+gitdb = ">=4.0.1,<5"
+
+[[package]]
 name = "google-api-core"
 version = "2.11.1"
 description = "Google API client core library"
 category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
@@ -619,14 +700,34 @@
 python-versions = ">=3.5"
 files = [
     {file = "idna-3.4-py3-none-any.whl", hash = "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"},
     {file = "idna-3.4.tar.gz", hash = "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4"},
 ]
 
 [[package]]
+name = "importlib-metadata"
+version = "6.7.0"
+description = "Read metadata from Python packages"
+category = "main"
+optional = false
+python-versions = ">=3.7"
+files = [
+    {file = "importlib_metadata-6.7.0-py3-none-any.whl", hash = "sha256:cb52082e659e97afc5dac71e79de97d8681de3aa07ff18578330904a9d18e5b5"},
+    {file = "importlib_metadata-6.7.0.tar.gz", hash = "sha256:1aaf550d4f73e5d6783e7acb77aec43d49da8017410afae93822cc9cca98c4d4"},
+]
+
+[package.dependencies]
+zipp = ">=0.5"
+
+[package.extras]
+docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
+perf = ["ipython"]
+testing = ["flufl.flake8", "importlib-resources (>=1.3)", "packaging", "pyfakefs", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-mypy (>=0.9.1)", "pytest-perf (>=0.9.2)", "pytest-ruff"]
+
+[[package]]
 name = "importlib-resources"
 version = "5.12.0"
 description = "Read resources from Python packages"
 category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
@@ -665,14 +766,31 @@
     {file = "isodate-0.6.1.tar.gz", hash = "sha256:48c5881de7e8b0a0d648cb024c8062dc84e7b840ed81e864c7614fd3c127bde9"},
 ]
 
 [package.dependencies]
 six = "*"
 
 [[package]]
+name = "jsonpickle"
+version = "3.0.1"
+description = "Python library for serializing any arbitrary object graph into JSON"
+category = "main"
+optional = false
+python-versions = ">=3.7"
+files = [
+    {file = "jsonpickle-3.0.1-py2.py3-none-any.whl", hash = "sha256:130d8b293ea0add3845de311aaba55e6d706d0bb17bc123bd2c8baf8a39ac77c"},
+    {file = "jsonpickle-3.0.1.tar.gz", hash = "sha256:032538804795e73b94ead410800ac387fdb6de98f8882ac957fcd247e3a85200"},
+]
+
+[package.extras]
+docs = ["jaraco.packaging (>=3.2)", "rst.linker (>=1.9)", "sphinx"]
+testing = ["ecdsa", "feedparser", "gmpy2", "numpy", "pandas", "pymongo", "pytest (>=3.5,!=3.7.3)", "pytest-black-multipy", "pytest-checkdocs (>=1.2.3)", "pytest-cov", "pytest-flake8 (>=1.1.1)", "scikit-learn", "sqlalchemy"]
+testing-libs = ["simplejson", "ujson"]
+
+[[package]]
 name = "jsonschema"
 version = "4.17.3"
 description = "An implementation of JSON Schema validation for Python"
 category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
@@ -708,14 +826,47 @@
 [package.extras]
 dev = ["flake8 (==5.0.4)", "flake8-bugbear (==22.10.25)", "mypy (==0.990)", "pre-commit (>=2.4,<3.0)", "pytest", "pytz", "simplejson", "tox"]
 docs = ["alabaster (==0.7.12)", "autodocsumm (==0.2.9)", "sphinx (==5.3.0)", "sphinx-issues (==3.0.1)", "sphinx-version-warning (==1.1.2)"]
 lint = ["flake8 (==5.0.4)", "flake8-bugbear (==22.10.25)", "mypy (==0.990)", "pre-commit (>=2.4,<3.0)"]
 tests = ["pytest", "pytz", "simplejson"]
 
 [[package]]
+name = "mlflow-skinny"
+version = "2.4.1"
+description = "MLflow: A Platform for ML Development and Productionization"
+category = "main"
+optional = false
+python-versions = ">=3.8"
+files = [
+    {file = "mlflow-skinny-2.4.1.tar.gz", hash = "sha256:ec5c8459a4bb1d0c619490dff0a3dce4949590a4bf76c77e0cb218143c33c29a"},
+    {file = "mlflow_skinny-2.4.1-py3-none-any.whl", hash = "sha256:b3226bbfdc5adcb7dcc2835c6956269641a07c9c2085d9f8f026bd577bd9660c"},
+]
+
+[package.dependencies]
+click = ">=7.0,<9"
+cloudpickle = "<3"
+databricks-cli = ">=0.8.7,<1"
+entrypoints = "<1"
+gitpython = ">=2.1.0,<4"
+importlib-metadata = ">=3.7.0,<4.7.0 || >4.7.0,<7"
+packaging = "<24"
+protobuf = ">=3.12.0,<5"
+pytz = "<2024"
+pyyaml = ">=5.1,<7"
+requests = ">=2.17.3,<3"
+sqlparse = ">=0.4.0,<1"
+
+[package.extras]
+aliyun-oss = ["aliyunstoreplugin"]
+databricks = ["azure-storage-file-datalake (>12)", "boto3 (>1)", "google-cloud-storage (>=1.30.0)"]
+extras = ["azureml-core (>=1.2.0)", "boto3", "google-cloud-storage (>=1.30.0)", "kubernetes", "mlserver (>=1.2.0,!=1.3.1)", "mlserver-mlflow (>=1.2.0,!=1.3.1)", "prometheus-flask-exporter", "pyarrow", "pysftp", "requests-auth-aws-sigv4", "virtualenv"]
+gateway = ["fastapi (<1)", "pydantic (>=1.0,<3)", "uvicorn (<1)"]
+sqlserver = ["mlflow-dbstore"]
+
+[[package]]
 name = "msal"
 version = "1.22.0"
 description = "The Microsoft Authentication Library (MSAL) for Python library enables your app to access the Microsoft Cloud by supporting authentication of users with Microsoft Azure Active Directory accounts (AAD) and Microsoft Accounts (MSA) using industry standard OAuth2 and OpenID Connect."
 category = "main"
 optional = false
 python-versions = "*"
 files = [
@@ -1380,14 +1531,26 @@
 python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*"
 files = [
     {file = "six-1.16.0-py2.py3-none-any.whl", hash = "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"},
     {file = "six-1.16.0.tar.gz", hash = "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926"},
 ]
 
 [[package]]
+name = "smmap"
+version = "5.0.0"
+description = "A pure Python implementation of a sliding window memory map manager"
+category = "main"
+optional = false
+python-versions = ">=3.6"
+files = [
+    {file = "smmap-5.0.0-py3-none-any.whl", hash = "sha256:2aba19d6a040e78d8b09de5c57e96207b09ed71d8e55ce0959eeee6c8e190d94"},
+    {file = "smmap-5.0.0.tar.gz", hash = "sha256:c840e62059cd3be204b0c9c9f74be2c09d5648eddd4580d9314c3ecde0b30936"},
+]
+
+[[package]]
 name = "snowflake-connector-python"
 version = "3.0.4"
 description = "Snowflake Connector for Python"
 category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
@@ -1475,14 +1638,31 @@
 python-versions = "*"
 files = [
     {file = "sortedcontainers-2.4.0-py2.py3-none-any.whl", hash = "sha256:a163dcaede0f1c021485e957a39245190e74249897e2ae4b2aa38595db237ee0"},
     {file = "sortedcontainers-2.4.0.tar.gz", hash = "sha256:25caa5a06cc30b6b83d11423433f65d1f9d76c4c6a0c90e3379eaa43b9bfdb88"},
 ]
 
 [[package]]
+name = "sqlparse"
+version = "0.4.4"
+description = "A non-validating SQL parser."
+category = "main"
+optional = false
+python-versions = ">=3.5"
+files = [
+    {file = "sqlparse-0.4.4-py3-none-any.whl", hash = "sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3"},
+    {file = "sqlparse-0.4.4.tar.gz", hash = "sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c"},
+]
+
+[package.extras]
+dev = ["build", "flake8"]
+doc = ["sphinx"]
+test = ["pytest", "pytest-cov"]
+
+[[package]]
 name = "strictyaml"
 version = "1.7.3"
 description = "Strict, typed YAML parser"
 category = "main"
 optional = false
 python-versions = ">=3.7.0"
 files = [
@@ -1490,14 +1670,29 @@
     {file = "strictyaml-1.7.3.tar.gz", hash = "sha256:22f854a5fcab42b5ddba8030a0e4be51ca89af0267961c8d6cfa86395586c407"},
 ]
 
 [package.dependencies]
 python-dateutil = ">=2.6.0"
 
 [[package]]
+name = "tabulate"
+version = "0.9.0"
+description = "Pretty-print tabular data"
+category = "main"
+optional = false
+python-versions = ">=3.7"
+files = [
+    {file = "tabulate-0.9.0-py3-none-any.whl", hash = "sha256:024ca478df22e9340661486f85298cff5f6dcdba14f3813e8830015b9ed1948f"},
+    {file = "tabulate-0.9.0.tar.gz", hash = "sha256:0095b12bf5966de529c0feb1fa08671671b3368eec77d7ef7ab114be2c068b3c"},
+]
+
+[package.extras]
+widechars = ["wcwidth"]
+
+[[package]]
 name = "tomli"
 version = "2.0.1"
 description = "A lil' TOML parser"
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
@@ -1585,8 +1780,8 @@
 [package.extras]
 docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
 testing = ["big-O", "flake8 (<5)", "jaraco.functools", "jaraco.itertools", "more-itertools", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)"]
 
 [metadata]
 lock-version = "2.0"
 python-versions = "^3.8"
-content-hash = "6a26cfc674bd3a5e64bb624e5b63097c94b8f43dc4df4ce4d69f6c03788532d7"
+content-hash = "817279519d637e59cf901692c7978d5d80e2046655c0c93b054a5e8f139d1895"
```

### Comparing `snowpark_session-0.1.0/setup.py` & `snowpark_session-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `snowpark_session-0.1.0/snowpark_session.py` & `snowpark_session-0.1.1/snowpark_session/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,41 +21,36 @@
     ...
 
     class Config:
         env_file = ".env"
 
 
 class SnowparkSession(SparkSession):
-    ...
-
-
-class SnowparkSession(SparkSession):
     snowflake_account: str
     snowflake_user: str
     snowflake_password: str
     snowflake_user_role: str
     snowflake_warehouse: str
     snowflake_database: str
     snowflake_schema: str
     spark: Optional[object] = None
 
-    def get_session(self):
-        from mlflow import create_session
-
-        self.spark = create_session(
+    def get_session(self, ):
+        from snowflake.snowpark import Session
+        self.spark = Session.builder.configs(
             {
-                "account": self.snowflake_account,
-                "user": self.snowflake_user,
-                "password": self.snowflake_password,
-                "role": self.snowflake_user_role,
-                "warehouse": self.snowflake_warehouse,
-                "database": self.snowflake_database,
-                "schema": self.snowflake_schema,
+                'account': self.snowflake_account, 
+                'user': self.snowflake_user, 
+                'password': self.snowflake_password, 
+                'role': self.snowflake_user_role, 
+                'warehouse': self.snowflake_warehouse, 
+                'database': self.snowflake_database, 
+                'schema': self.snowflake_schema
             }
-        )
+        ).create()
         self.spark.use_warehouse(self.snowflake_warehouse)
         return self.spark
 
 
 class MLFlowSession(BaseSettings):
     deployment_client: Optional[object] = None
```

### Comparing `snowpark_session-0.1.0/PKG-INFO` & `snowpark_session-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: snowpark-session
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Carlos D. Escobar-Valbuena
 Author-email: carlosdavidescobar@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: azure-ai-ml (>=1.8.0,<2.0.0)
+Requires-Dist: azureml-mlflow (>=1.52.0,<2.0.0)
 Requires-Dist: snowflake-snowpark-python (==1.5.1) ; python_version >= "3.6" and python_version < "3.10"
 Description-Content-Type: text/markdown
 
 # Snowpark Session Util
 **A simple utility for spark and mlflow session objects**
```

