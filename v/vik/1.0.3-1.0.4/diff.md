# Comparing `tmp/vik-1.0.3.tar.gz` & `tmp/vik-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vik-1.0.3.tar", last modified: Mon Jun  5 07:17:13 2023, max compression
+gzip compressed data, was "vik-1.0.4.tar", last modified: Thu Jul  6 08:48:05 2023, max compression
```

## Comparing `vik-1.0.3.tar` & `vik-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 07:17:13.832357 vik-1.0.3/
--rw-rw-rw-   0        0        0    35149 2023-03-25 15:10:13.000000 vik-1.0.3/LICENSE
--rw-rw-rw-   0        0        0       20 2023-06-05 07:14:54.000000 vik-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      953 2023-06-05 07:17:13.832357 vik-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      606 2023-03-25 15:10:13.000000 vik-1.0.3/README.md
--rw-rw-rw-   0        0        0       81 2023-03-25 15:10:13.000000 vik-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      573 2023-06-05 07:17:13.832357 vik-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-05 07:17:13.800358 vik-1.0.3/vik/
--rw-rw-rw-   0        0        0      807 2023-06-05 07:11:34.000000 vik-1.0.3/vik/.vimrc
--rw-rw-rw-   0        0        0        0 2023-03-25 15:10:13.000000 vik-1.0.3/vik/__init__.py
--rw-rw-rw-   0        0        0      814 2023-03-25 15:10:13.000000 vik-1.0.3/vik/vik.py
-drwxrwxrwx   0        0        0        0 2023-06-05 07:17:13.832357 vik-1.0.3/vik.egg-info/
--rw-rw-rw-   0        0        0      953 2023-06-05 07:17:13.000000 vik-1.0.3/vik.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-06-05 07:17:13.000000 vik-1.0.3/vik.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 07:17:13.000000 vik-1.0.3/vik.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-06-05 07:17:13.000000 vik-1.0.3/vik.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2023-06-05 07:17:13.000000 vik-1.0.3/vik.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-05 07:17:13.000000 vik-1.0.3/vik.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:48:05.593134 vik-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-06 08:47:55.000000 vik-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 08:47:55.000000 vik-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-06 08:48:05.593134 vik-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-06 08:47:55.000000 vik-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-06 08:47:55.000000 vik-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-06 08:48:05.593134 vik-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:48:05.593134 vik-1.0.4/vik/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-06 08:47:55.000000 vik-1.0.4/vik/.vimrc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:47:55.000000 vik-1.0.4/vik/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      814 2023-07-06 08:47:55.000000 vik-1.0.4/vik/vik.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:48:05.593134 vik-1.0.4/vik.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-06 08:48:05.000000 vik-1.0.4/vik.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-06 08:48:05.000000 vik-1.0.4/vik.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 08:48:05.000000 vik-1.0.4/vik.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 08:48:05.000000 vik-1.0.4/vik.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 08:48:05.000000 vik-1.0.4/vik.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-06 08:48:05.000000 vik-1.0.4/vik.egg-info/top_level.txt
```

### Comparing `vik-1.0.3/LICENSE` & `vik-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vik-1.0.3/README.md` & `vik-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `vik-1.0.3/vik/.vimrc` & `vik-1.0.4/vik/.vimrc`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 
 let &t_EI = "\e[2 q"
 let &t_SI = "\e[6 q"
 
 syntax on
 set filetype=markdown
 
+set binary
+set autoread
+
 set ignorecase
 set smartcase
 
 set tabstop=2
 set shiftwidth=2
 set softtabstop=2
 set expandtab
@@ -21,17 +24,14 @@
 set smartindent
 
 set linebreak
 
 set mouse=a
 set backspace=2
 
-set binary
-set autoread
-
 nnoremap <F2> :set invpaste paste?<CR>
 set pastetoggle=<F2>
 set showmode
 
 nnoremap <F3> :set invhlsearch<CR>
 
 nnoremap <F4> :set number!<CR>
```

### Comparing `vik-1.0.3/vik/vik.py` & `vik-1.0.4/vik/vik.py`

 * *Files identical despite different names*

