# Comparing `tmp/sqlmap-1.7.6.tar.gz` & `tmp/sqlmap-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sqlmap-1.7.6.tar", last modified: Fri Jun  2 09:26:10 2023, max compression
+gzip compressed data, was "dist/sqlmap-1.7.7.tar", last modified: Thu Jul  6 08:43:48 2023, max compression
```

## Comparing `sqlmap-1.7.6.tar` & `sqlmap-1.7.7.tar`

### file list

```diff
@@ -1,779 +1,779 @@
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    28932 2023-06-02 09:26:09.000000 sqlmap-1.7.6/MANIFEST.in
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4952 2023-06-02 09:26:10.000000 sqlmap-1.7.6/PKG-INFO
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5213 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/README.md
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/thirdparty/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/thirdparty/wininetpton/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      319 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/wininetpton/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2775 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/wininetpton/win_inet_pton.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/thirdparty/clientform/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   126727 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/clientform/clientform.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/clientform/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/thirdparty/multipart/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4513 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/multipart/multipartpost.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/multipart/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/thirdparty/socks/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    17437 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/socks/socks.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/socks/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1401 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/socks/LICENSE
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    10510 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/escsm.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3749 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/eucjpprober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2766 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/utf8prober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    11102 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/langturkishmodel.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5110 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/charsetprober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3413 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/mbcharsetprober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    13546 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/euckrfreq.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      242 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/version.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1754 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/gb2312prober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1855 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/cp949prober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     9411 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/chardistribution.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1661 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/enums.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    11345 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/langhebrewmodel.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12688 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/langgreekmodel.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3950 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/escprober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3590 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/codingstatemachine.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    31621 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/euctwfreq.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5370 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/latin1prober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12839 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/langbulgarianmodel.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    31254 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/big5freq.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1748 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/euckrprober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    25777 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/jisfreq.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1757 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/big5prober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    25481 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/mbcssm.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12485 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/universaldetector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    20715 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/gb2312freq.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3774 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/sjisprober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1134 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/compat.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3546 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/sbcsgroupprober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1559 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3787 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/charsetgroupprober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    19643 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/jpcntx.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    17948 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/langcyrillicmodel.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12592 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/langhungarianmodel.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1747 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/euctwprober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5657 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/sbcharsetprober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2012 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/mbcsgroupprober.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    11290 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/langthaimodel.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    13838 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/chardet/hebrewprober.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/thirdparty/odict/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4283 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/odict/ordereddict.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      156 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/odict/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/thirdparty/keepalive/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      730 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/keepalive/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    22807 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/keepalive/keepalive.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/thirdparty/magic/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6723 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/magic/magic.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/magic/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/thirdparty/ansistrm/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5329 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/ansistrm/ansistrm.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/ansistrm/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/thirdparty/identywaf/
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)    25913 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/identywaf/identYwaf.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    61564 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/identywaf/data.json
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      270 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/identywaf/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1078 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/identywaf/LICENSE
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/thirdparty/prettyprint/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1357 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/prettyprint/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4215 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/prettyprint/prettyprint.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/thirdparty/bottle/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   170898 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/bottle/bottle.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        5 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/bottle/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/thirdparty/fcrypt/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1356 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/fcrypt/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    26757 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/fcrypt/fcrypt.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/thirdparty/pydes/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    27500 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/pydes/pyDes.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      720 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/pydes/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/thirdparty/beautifulsoup/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    80038 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/beautifulsoup/beautifulsoup.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1673 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/beautifulsoup/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/thirdparty/six/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    34581 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/six/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/thirdparty/termcolor/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/termcolor/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5246 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/termcolor/termcolor.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/thirdparty/colorama/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2524 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/colorama/ansi.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2065 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/colorama/initialise.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6356 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/colorama/winterm.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      240 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/colorama/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    10243 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/colorama/ansitowin32.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5365 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/thirdparty/colorama/win32.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    16703 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/.pylintrc
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/procs/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/procs/mssqlserver/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      269 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/procs/mssqlserver/create_new_xp_cmdshell.sql
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      246 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/procs/mssqlserver/configure_openrowset.sql
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       47 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/procs/mssqlserver/disable_xp_cmdshell_2000.sql
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       70 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/procs/mssqlserver/enable_xp_cmdshell_2000.sql
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      163 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/procs/mssqlserver/activate_sp_oacreate.sql
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      333 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/procs/mssqlserver/run_statement_as_user.sql
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      197 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/procs/mssqlserver/dns_request.sql
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      236 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/procs/mssqlserver/configure_xp_cmdshell.sql
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      187 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/procs/README.txt
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/procs/postgresql/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      536 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/procs/postgresql/dns_request.sql
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/procs/mysql/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       73 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/procs/mysql/write_file_limit.sql
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       85 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/procs/mysql/dns_request.sql
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/procs/oracle/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2010 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/procs/oracle/read_file_export_extension.sql
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      183 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/procs/oracle/dns_request.sql
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      282 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/README.txt
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/9.1/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2693 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/9.1/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/9.0/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2633 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/9.0/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/9.5/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2633 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/9.5/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/9.3/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2693 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/9.3/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/12/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3257 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/12/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/11/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2633 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/11/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/8.4/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2563 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/8.4/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/8.2/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2561 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/8.2/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/8.3/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2562 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/8.3/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/9.4/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2693 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/9.4/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/10/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2632 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/10/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/9.2/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2693 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/9.2/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/9.6/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2632 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/9.6/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/9.1/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2652 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/9.1/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/9.0/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2729 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/9.0/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/9.5/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2639 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/9.5/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/9.3/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2652 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/9.3/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/11/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2640 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/11/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/8.4/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2020 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/8.4/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/8.2/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2018 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/8.2/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/8.3/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2016 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/8.3/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/9.4/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2652 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/9.4/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/10/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2639 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/10/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/9.2/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2652 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/9.2/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/9.6/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2640 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/9.6/lib_postgresqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/windows/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/windows/32/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/windows/32/9.0/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4231 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/windows/32/9.0/lib_postgresqludf_sys.dll_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/windows/32/8.4/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4773 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/windows/32/8.4/lib_postgresqludf_sys.dll_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/windows/32/8.2/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4755 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/windows/32/8.2/lib_postgresqludf_sys.dll_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/windows/32/8.3/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4766 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/postgresql/windows/32/8.3/lib_postgresqludf_sys.dll_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/mysql/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/mysql/linux/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/mysql/linux/64/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3200 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/mysql/linux/64/lib_mysqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/mysql/linux/32/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2512 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/mysql/linux/32/lib_mysqludf_sys.so_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/mysql/windows/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/mysql/windows/64/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5267 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/mysql/windows/64/lib_mysqludf_sys.dll_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/udf/mysql/windows/32/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4549 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/udf/mysql/windows/32/lib_mysqludf_sys.dll_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/shell/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/shell/stagers/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      379 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/shell/stagers/stager.php_
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1201 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/shell/stagers/stager.asp_
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      529 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/shell/stagers/stager.aspx_
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1321 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/shell/stagers/stager.jsp_
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      686 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/shell/README.txt
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/shell/backdoors/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      243 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/shell/backdoors/backdoor.asp_
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      469 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/shell/backdoors/backdoor.php_
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      417 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/shell/backdoors/backdoor.aspx_
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      359 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/shell/backdoors/backdoor.jsp_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/txt/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    68896 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/txt/smalldict.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18539 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/txt/common-outputs.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    44074 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/txt/common-tables.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   399831 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/txt/user-agents.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    48329 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/txt/common-files.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    14655 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/txt/keywords.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    26013 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/txt/common-columns.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)  6076425 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/txt/wordlist.tx_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/html/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5763 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/html/index.html
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/xml/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     9507 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/xml/errors.xml
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/xml/payloads/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    19304 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/xml/payloads/union_query.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5482 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/xml/payloads/inline_query.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    68050 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/xml/payloads/error_based.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    79693 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/xml/payloads/time_blind.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    24754 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/xml/payloads/stacked_queries.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    58342 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/xml/payloads/boolean_blind.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   141238 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/xml/queries.xml
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/data/xml/banner/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      242 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/xml/banner/sharepoint.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1649 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/xml/banner/x-powered-by.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1448 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/xml/banner/set-cookie.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      233 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/xml/banner/x-aspnet-version.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   101453 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/xml/banner/mssql.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      805 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/xml/banner/servlet-engine.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3897 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/xml/banner/generic.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      327 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/xml/banner/postgresql.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    31443 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/xml/banner/server.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      158 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/xml/banner/oracle.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2956 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/xml/banner/mysql.xml
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    15092 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/data/xml/boundaries.xml
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/tamper/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1879 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/between.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      590 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/symboliclogical.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      955 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/misunion.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      753 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/schemasplit.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      906 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/dunion.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1127 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/least.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1211 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/substring2leftright.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1007 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/concat2concatws.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3046 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/luanginx.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      944 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/apostrophemask.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2589 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/space2mssqlblank.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      700 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/0eunion.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1197 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/randomcomments.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1802 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/plus2concat.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      963 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/varnish.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1314 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/multiplespaces.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1597 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/versionedkeywords.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      918 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/space2mssqlhash.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      639 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/informationschemacomment.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      559 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/ord2ascii.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1737 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/versionedmorekeywords.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      523 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/apostrophenullencode.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1413 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/percentage.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      825 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/sp_password.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      766 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/equaltorlike.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2250 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/plus2fnconcat.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1855 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/halfversionedmorekeywords.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1295 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/space2morecomment.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1201 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/modsecurityzeroversioned.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1135 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/greatest.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1290 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/bluecoat.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1065 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/uppercase.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1584 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/space2hash.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1455 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/overlongutf8more.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      680 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/decentities.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1264 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/space2dash.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1292 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/modsecurityversioned.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      715 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/hexentities.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1388 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/charencode.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      918 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/equaltolike.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1218 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/chardoubleencode.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      985 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/scientific.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1351 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/space2comment.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1306 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/unmagicquotes.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1285 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/xforwardedfor.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1282 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/space2plus.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1215 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/charunicodeescape.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      511 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/unionalltounion.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2218 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/space2morehash.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1744 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/ifnull2casewhenisnull.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      468 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/escapequotes.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1669 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/ifnull2ifisnull.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      758 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/commentbeforeparentheses.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      868 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/sleep2getlock.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1002 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/lowercase.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1225 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/commalessmid.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1646 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/charunicodeencode.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1168 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/space2mysqldash.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1377 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/hex2char.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1736 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/randomcase.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1000 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/appendnullbyte.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      519 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/base64encode.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1663 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/space2randomblank.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1295 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/binary.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1943 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/if2case.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1444 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/overlongutf8.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1977 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/space2mysqlblank.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      849 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/htmlencode.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      970 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/tamper/commalesslimit.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      258 2023-06-02 09:26:09.000000 sqlmap-1.7.6/sqlmap/__init__.py
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)    25751 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/sqlmap.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/doc/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    34109 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/doc/CHANGELOG.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    25029 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/doc/THANKS.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      190 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/doc/AUTHORS
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/doc/translations/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3281 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/doc/translations/README-it-IT.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4227 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/doc/translations/README-uk-UA.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3289 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/doc/translations/README-ko-KR.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3149 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/doc/translations/README-rs-RS.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3786 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/doc/translations/README-fa-IR.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4092 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/doc/translations/README-bg-BG.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4218 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/doc/translations/README-ru-RUS.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3055 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/doc/translations/README-id-ID.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3184 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/doc/translations/README-de-GER.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3332 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/doc/translations/README-fr-FR.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3175 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/doc/translations/README-pt-BR.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3180 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/doc/translations/README-hr-HR.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3167 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/doc/translations/README-nl-NL.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3240 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/doc/translations/README-sk-SK.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3561 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/doc/translations/README-vi-VN.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3226 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/doc/translations/README-pl-PL.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4248 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/doc/translations/README-gr-GR.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2921 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/doc/translations/README-zh-CN.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3609 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/doc/translations/README-ja-JP.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6026 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/doc/translations/README-ka-GE.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3029 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/doc/translations/README-tr-TR.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3435 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/doc/translations/README-es-MX.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    14763 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/doc/THIRD-PARTY.md
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    22119 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/sqlmap.conf
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18886 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/LICENSE
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/plugins/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/plugins/generic/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2654 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/generic/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2484 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/generic/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4909 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/generic/custom.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    30708 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/generic/entries.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    27907 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/generic/search.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1730 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/generic/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18208 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/generic/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    29216 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/generic/users.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1723 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/generic/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/generic/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6887 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/generic/misc.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    54885 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/generic/databases.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12371 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/generic/filesystem.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/presto/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1701 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/presto/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2204 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/presto/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      678 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/presto/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      971 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/presto/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5279 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/presto/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      910 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/presto/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      671 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/presto/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/hsqldb/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1445 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/hsqldb/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2784 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/hsqldb/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      687 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/hsqldb/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      971 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/hsqldb/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5276 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/hsqldb/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      909 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/hsqldb/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2537 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/hsqldb/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/mssqlserver/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18049 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/mssqlserver/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2583 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/mssqlserver/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      889 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/mssqlserver/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6499 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/mssqlserver/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6913 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/mssqlserver/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      950 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/mssqlserver/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    17213 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/mssqlserver/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/access/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2525 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/access/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2130 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/access/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      670 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/access/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1011 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/access/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5843 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/access/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      919 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/access/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      691 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/access/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/raima/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2609 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/raima/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      520 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/raima/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      687 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/raima/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1035 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/raima/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2652 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/raima/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      899 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/raima/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      703 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/raima/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/derby/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1322 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/derby/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1830 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/derby/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/derby/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      995 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/derby/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2636 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/derby/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      907 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/derby/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/derby/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/cache/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1356 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/cache/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2397 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/cache/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      735 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/cache/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      967 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/cache/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3135 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/cache/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      900 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/cache/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/cache/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/vertica/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      459 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/vertica/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1920 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/vertica/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      689 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/vertica/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      975 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/vertica/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2992 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/vertica/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      920 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/vertica/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/vertica/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/firebird/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1080 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/firebird/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2260 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/firebird/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1151 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/firebird/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      979 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/firebird/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4990 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/firebird/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      929 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/firebird/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      675 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/firebird/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/monetdb/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1103 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/monetdb/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1894 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/monetdb/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      735 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/monetdb/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      975 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/monetdb/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2549 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/monetdb/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      920 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/monetdb/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/monetdb/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/maxdb/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     9202 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/maxdb/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      507 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/maxdb/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/maxdb/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      983 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/maxdb/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3792 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/maxdb/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      903 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/maxdb/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      678 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/maxdb/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/mimersql/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      926 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/mimersql/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1858 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/mimersql/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      807 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/mimersql/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      979 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/mimersql/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2591 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/mimersql/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      930 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/mimersql/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/mimersql/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/postgresql/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      428 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/postgresql/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2097 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/postgresql/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1016 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/postgresql/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5448 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/postgresql/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     9801 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/postgresql/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1304 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/postgresql/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3005 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/postgresql/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/mysql/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      265 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/mysql/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2095 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/mysql/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1044 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/mysql/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5124 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/mysql/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12744 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/mysql/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1113 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/mysql/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7731 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/mysql/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/informix/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1022 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/informix/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1902 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/informix/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1272 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/informix/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      365 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/informix/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3284 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/informix/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      930 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/informix/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/informix/filesystem.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/altibase/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      589 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/altibase/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      506 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/altibase/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      678 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/altibase/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      979 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/altibase/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2657 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/altibase/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      930 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/altibase/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/altibase/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/extremedb/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2427 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/extremedb/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      507 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/extremedb/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/extremedb/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      983 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/extremedb/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2673 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/extremedb/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      939 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/extremedb/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      677 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/extremedb/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/mckoi/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2371 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/mckoi/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      503 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/mckoi/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/mckoi/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      967 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/mckoi/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2590 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/mckoi/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      899 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/mckoi/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      669 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/mckoi/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/db2/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      615 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/db2/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1935 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/db2/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      678 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/db2/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      365 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/db2/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5871 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/db2/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      880 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/db2/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/db2/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/cubrid/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      918 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/cubrid/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1835 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/cubrid/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      726 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/cubrid/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      971 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/cubrid/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2541 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/cubrid/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      910 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/cubrid/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/cubrid/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/h2/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1580 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/h2/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      500 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/h2/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      687 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/h2/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      955 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/h2/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3327 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/h2/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      869 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/h2/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      663 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/h2/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/oracle/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6002 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/oracle/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2817 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/oracle/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      886 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/oracle/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1101 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/oracle/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3873 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/oracle/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      909 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/oracle/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2301 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/oracle/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/cratedb/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      632 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/cratedb/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2097 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/cratedb/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/cratedb/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      975 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/cratedb/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2538 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/cratedb/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      920 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/cratedb/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/cratedb/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/sybase/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    11670 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/sybase/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2558 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/sybase/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      899 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/sybase/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      971 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/sybase/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3429 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/sybase/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      909 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/sybase/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      671 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/sybase/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/clickhouse/
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      638 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/clickhouse/enumeration.py
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      255 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/clickhouse/connector.py
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      687 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/clickhouse/syntax.py
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      987 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/clickhouse/takeover.py
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)     2627 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/clickhouse/fingerprint.py
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      950 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/clickhouse/__init__.py
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      679 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/clickhouse/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/sqlite/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2054 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/sqlite/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3083 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/sqlite/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      644 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/sqlite/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      971 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/sqlite/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3176 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/sqlite/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      909 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/sqlite/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      671 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/sqlite/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/virtuoso/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1541 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/virtuoso/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      506 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/virtuoso/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      678 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/virtuoso/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      979 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/virtuoso/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2517 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/virtuoso/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      929 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/virtuoso/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      675 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/virtuoso/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/frontbase/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      923 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/frontbase/enumeration.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      507 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/frontbase/connector.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/frontbase/syntax.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      983 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/frontbase/takeover.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2613 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/frontbase/fingerprint.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      939 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/frontbase/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      677 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/plugins/dbms/frontbase/filesystem.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/lib/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/lib/controller/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8896 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/controller/handler.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7233 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/controller/action.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    75617 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/controller/checks.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/controller/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    36761 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/controller/controller.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/lib/utils/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7907 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/utils/search.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4686 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/utils/httpd.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    48979 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/utils/hash.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2325 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/utils/getch.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5063 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/utils/sqlalchemy.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8347 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/utils/hashdb.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2935 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/utils/xrange.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      926 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/utils/versioncheck.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3337 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/utils/progress.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2674 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/utils/purge.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    10977 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/utils/crawler.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8030 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/utils/har.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    15901 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/utils/brute.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7369 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/utils/pivotdumptable.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/utils/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    34251 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/utils/api.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3190 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/utils/safe2bin.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1111 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/utils/timeout.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5564 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/utils/deps.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18275 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/utils/sgmllib.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/lib/request/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18899 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/request/basic.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6017 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/request/dns.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3229 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/request/direct.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8110 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/request/redirecthandler.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      942 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/request/rangehandler.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      590 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/request/methodrequest.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5815 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/request/httpshandler.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/request/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      633 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/request/templates.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1384 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/request/basicauthhandler.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1566 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/request/chunkedhandler.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1158 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/request/pkihandler.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    24811 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/request/inject.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    80323 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/request/connect.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7788 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/request/comparison.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/lib/techniques/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/lib/techniques/error/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    21160 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/techniques/error/use.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/techniques/error/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/lib/techniques/dns/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5061 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/techniques/dns/use.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1125 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/techniques/dns/test.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/techniques/dns/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/lib/techniques/blind/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/techniques/blind/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    34640 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/techniques/blind/inference.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/techniques/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/lib/techniques/union/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    23150 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/techniques/union/use.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18616 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/techniques/union/test.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/techniques/union/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/lib/core/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      728 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/core/data.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5865 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/core/patch.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1800 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/core/readlineng.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    28848 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/core/dump.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8414 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/core/threads.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12888 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/core/convert.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    13908 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/core/enums.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2634 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/core/decorators.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6032 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/core/bigarray.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    10052 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/core/gui.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1646 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/core/exception.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    15220 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/core/testing.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7442 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/core/optiondict.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    34129 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/core/target.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1980 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/core/session.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    59174 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/core/agent.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   106059 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/core/option.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    45491 2023-06-02 09:26:09.000000 sqlmap-1.7.6/sqlmap/lib/core/settings.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8986 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/core/compat.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/core/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5657 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/core/subprocessng.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1876 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/core/revision.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      885 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/core/profiling.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      559 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/core/defaults.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5489 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/core/log.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4956 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/core/shell.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    17637 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/core/dicts.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3201 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/core/wordlist.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      988 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/core/unescaper.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7468 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/core/update.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5046 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/core/replication.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6236 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/core/datatype.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   193586 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/core/common.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/lib/takeover/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8440 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/takeover/abstraction.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    13903 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/takeover/udf.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    28240 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/takeover/metasploit.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    11839 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/takeover/xp_cmdshell.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3838 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/takeover/registry.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18315 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/takeover/web.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/takeover/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4739 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/takeover/icmpsh.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/lib/parse/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    49596 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/parse/cmdline.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2703 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/parse/handler.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3578 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/parse/payloads.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3498 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/parse/configfile.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1460 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/parse/headers.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1805 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/parse/sitemap.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/parse/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3580 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/parse/banner.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3022 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/lib/parse/html.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6215 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/sqlmapapi.yaml
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/extra/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/extra/cloak/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2286 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/cloak/cloak.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      732 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/cloak/README.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/cloak/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/extra/shutils/
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      305 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/shutils/modernize.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      797 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/shutils/duplicates.py
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)     1140 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/shutils/precommit-hook.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      332 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/shutils/pycodestyle.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      660 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/shutils/drei.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      255 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/shutils/blanks.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      235 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/shutils/pylint.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)     5861 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/shutils/pypi.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      630 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/shutils/recloak.sh
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      903 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/shutils/newlines.py
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      869 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/shutils/strip.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      245 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/shutils/junk.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      311 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/shutils/autocompletion.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      313 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/shutils/pydiatra.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      875 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/shutils/postcommit-hook.sh
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      320 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/shutils/pyflakes.sh
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/extra/runcmd/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      193 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/runcmd/README.txt
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/extra/runcmd/src/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      883 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/runcmd/src/runcmd.sln
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      271 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/runcmd/src/README.txt
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/extra/runcmd/src/runcmd/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1348 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/runcmd/src/runcmd/runcmd.cpp
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      516 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/runcmd/src/runcmd/stdafx.h
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4508 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/runcmd/src/runcmd/runcmd.vcproj
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      293 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/runcmd/src/runcmd/stdafx.cpp
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    37206 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/runcmd/runcmd.exe_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/extra/beep/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2901 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/beep/beep.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/beep/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    46772 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/beep/beep.wav
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/extra/shellcodeexec/
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/extra/shellcodeexec/linux/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1691 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/shellcodeexec/linux/shellcodeexec.x32_
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1927 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/shellcodeexec/linux/shellcodeexec.x64_
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      282 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/shellcodeexec/README.txt
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/extra/shellcodeexec/windows/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2758 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/shellcodeexec/windows/shellcodeexec.x32.exe_
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/extra/icmpsh/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3965 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/icmpsh/icmpsh-m.c
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7009 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/icmpsh/icmpsh.exe_
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     9342 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/icmpsh/icmpsh-s.c
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1641 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/icmpsh/README.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2136 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/icmpsh/icmpsh-m.pl
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      872 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/icmpsh/__init__.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4809 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/icmpsh/icmpsh_m.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/extra/dbgtool/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2475 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/dbgtool/dbgtool.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      549 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/dbgtool/README.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/dbgtool/__init__.py
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap/extra/vulnserver/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     9127 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/vulnserver/vulnserver.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/extra/vulnserver/__init__.py
--rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)     2784 2023-06-02 09:25:07.000000 sqlmap-1.7.6/sqlmap/sqlmapapi.py
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       38 2023-06-02 09:26:10.000000 sqlmap-1.7.6/setup.cfg
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3193 2023-06-02 09:26:09.000000 sqlmap-1.7.6/README.rst
-drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap.egg-info/
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    24105 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap.egg-info/SOURCES.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4952 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap.egg-info/PKG-INFO
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        7 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap.egg-info/top_level.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        1 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap.egg-info/not-zip-safe
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       47 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap.egg-info/entry_points.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        1 2023-06-02 09:26:10.000000 sqlmap-1.7.6/sqlmap.egg-info/dependency_links.txt
--rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1549 2023-06-02 09:26:00.000000 sqlmap-1.7.6/setup.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    28932 2023-07-06 08:43:47.000000 sqlmap-1.7.7/MANIFEST.in
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4952 2023-07-06 08:43:48.000000 sqlmap-1.7.7/PKG-INFO
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5213 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/README.md
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/thirdparty/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/thirdparty/wininetpton/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      319 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/wininetpton/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2775 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/wininetpton/win_inet_pton.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/thirdparty/clientform/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   126727 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/clientform/clientform.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/clientform/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/thirdparty/multipart/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4513 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/multipart/multipartpost.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/multipart/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/thirdparty/socks/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    17437 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/socks/socks.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/socks/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1401 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/socks/LICENSE
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    10510 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/escsm.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3749 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/eucjpprober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2766 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/utf8prober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    11102 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/langturkishmodel.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5110 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/charsetprober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3413 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/mbcharsetprober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    13546 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/euckrfreq.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      242 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/version.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1754 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/gb2312prober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1855 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/cp949prober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     9411 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/chardistribution.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1661 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/enums.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    11345 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/langhebrewmodel.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12688 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/langgreekmodel.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3950 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/escprober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3590 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/codingstatemachine.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    31621 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/euctwfreq.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5370 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/latin1prober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12839 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/langbulgarianmodel.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    31254 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/big5freq.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1748 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/euckrprober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    25777 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/jisfreq.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1757 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/big5prober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    25481 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/mbcssm.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12485 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/universaldetector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    20715 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/gb2312freq.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3774 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/sjisprober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1134 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/compat.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3546 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/sbcsgroupprober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1559 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3787 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/charsetgroupprober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    19643 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/jpcntx.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    17948 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/langcyrillicmodel.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12592 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/langhungarianmodel.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1747 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/euctwprober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5657 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/sbcharsetprober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2012 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/mbcsgroupprober.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    11290 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/langthaimodel.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    13838 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/chardet/hebrewprober.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/thirdparty/odict/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4283 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/odict/ordereddict.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      156 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/odict/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/thirdparty/keepalive/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      730 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/keepalive/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    22807 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/keepalive/keepalive.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/thirdparty/magic/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6723 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/magic/magic.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/magic/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/thirdparty/ansistrm/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5329 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/ansistrm/ansistrm.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/ansistrm/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/thirdparty/identywaf/
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)    25913 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/identywaf/identYwaf.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    61564 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/identywaf/data.json
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      270 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/identywaf/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1078 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/identywaf/LICENSE
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/thirdparty/prettyprint/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1357 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/prettyprint/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4215 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/prettyprint/prettyprint.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/thirdparty/bottle/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   170898 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/bottle/bottle.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        5 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/bottle/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/thirdparty/fcrypt/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1356 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/fcrypt/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    26757 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/fcrypt/fcrypt.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/thirdparty/pydes/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    27500 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/pydes/pyDes.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      720 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/pydes/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/thirdparty/beautifulsoup/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    80038 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/beautifulsoup/beautifulsoup.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1673 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/beautifulsoup/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/thirdparty/six/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    34581 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/six/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/thirdparty/termcolor/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/termcolor/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5246 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/termcolor/termcolor.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/thirdparty/colorama/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2524 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/colorama/ansi.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2065 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/colorama/initialise.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6356 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/colorama/winterm.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      240 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/colorama/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    10243 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/colorama/ansitowin32.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5365 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/thirdparty/colorama/win32.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    16703 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/.pylintrc
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/procs/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/procs/mssqlserver/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      269 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/procs/mssqlserver/create_new_xp_cmdshell.sql
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      246 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/procs/mssqlserver/configure_openrowset.sql
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       47 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/procs/mssqlserver/disable_xp_cmdshell_2000.sql
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       70 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/procs/mssqlserver/enable_xp_cmdshell_2000.sql
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      163 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/procs/mssqlserver/activate_sp_oacreate.sql
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      333 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/procs/mssqlserver/run_statement_as_user.sql
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      197 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/procs/mssqlserver/dns_request.sql
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      236 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/procs/mssqlserver/configure_xp_cmdshell.sql
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      187 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/procs/README.txt
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/procs/postgresql/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      536 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/procs/postgresql/dns_request.sql
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/procs/mysql/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       73 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/procs/mysql/write_file_limit.sql
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       85 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/procs/mysql/dns_request.sql
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/procs/oracle/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2010 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/procs/oracle/read_file_export_extension.sql
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      397 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/procs/oracle/dns_request.sql
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      282 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/README.txt
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/9.1/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2693 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/9.1/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/9.0/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2633 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/9.0/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/9.5/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2633 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/9.5/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/9.3/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2693 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/9.3/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/12/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3257 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/12/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/11/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2633 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/11/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/8.4/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2563 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/8.4/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/8.2/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2561 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/8.2/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/8.3/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2562 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/8.3/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/9.4/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2693 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/9.4/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/10/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2632 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/10/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/9.2/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2693 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/9.2/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/9.6/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2632 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/9.6/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/9.1/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2652 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/9.1/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/9.0/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2729 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/9.0/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/9.5/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2639 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/9.5/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/9.3/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2652 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/9.3/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/11/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2640 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/11/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/8.4/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2020 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/8.4/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/8.2/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2018 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/8.2/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/8.3/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2016 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/8.3/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/9.4/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2652 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/9.4/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/10/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2639 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/10/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/9.2/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2652 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/9.2/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/9.6/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2640 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/9.6/lib_postgresqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/windows/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/windows/32/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/windows/32/9.0/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4231 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/windows/32/9.0/lib_postgresqludf_sys.dll_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/windows/32/8.4/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4773 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/windows/32/8.4/lib_postgresqludf_sys.dll_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/windows/32/8.2/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4755 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/windows/32/8.2/lib_postgresqludf_sys.dll_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/windows/32/8.3/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4766 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/postgresql/windows/32/8.3/lib_postgresqludf_sys.dll_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/mysql/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/mysql/linux/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/mysql/linux/64/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3200 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/mysql/linux/64/lib_mysqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/mysql/linux/32/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2512 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/mysql/linux/32/lib_mysqludf_sys.so_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/mysql/windows/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/mysql/windows/64/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5267 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/mysql/windows/64/lib_mysqludf_sys.dll_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/udf/mysql/windows/32/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4549 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/udf/mysql/windows/32/lib_mysqludf_sys.dll_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/shell/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/shell/stagers/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      379 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/shell/stagers/stager.php_
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1201 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/shell/stagers/stager.asp_
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      529 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/shell/stagers/stager.aspx_
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1321 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/shell/stagers/stager.jsp_
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      686 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/shell/README.txt
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/shell/backdoors/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      243 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/shell/backdoors/backdoor.asp_
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      469 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/shell/backdoors/backdoor.php_
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      417 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/shell/backdoors/backdoor.aspx_
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      359 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/shell/backdoors/backdoor.jsp_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/txt/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    68896 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/txt/smalldict.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18539 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/txt/common-outputs.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    44074 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/txt/common-tables.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   399831 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/txt/user-agents.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    48329 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/txt/common-files.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    14655 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/txt/keywords.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    26013 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/txt/common-columns.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)  6076425 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/txt/wordlist.tx_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/html/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5763 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/html/index.html
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/xml/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     9507 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/xml/errors.xml
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/xml/payloads/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    19304 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/xml/payloads/union_query.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5482 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/xml/payloads/inline_query.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    68050 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/xml/payloads/error_based.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    79693 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/xml/payloads/time_blind.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    24754 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/xml/payloads/stacked_queries.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    58342 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/xml/payloads/boolean_blind.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   141238 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/xml/queries.xml
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/data/xml/banner/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      242 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/xml/banner/sharepoint.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1649 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/xml/banner/x-powered-by.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1448 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/xml/banner/set-cookie.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      233 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/xml/banner/x-aspnet-version.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   101453 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/xml/banner/mssql.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      805 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/xml/banner/servlet-engine.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3897 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/xml/banner/generic.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      327 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/xml/banner/postgresql.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    31443 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/xml/banner/server.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      158 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/xml/banner/oracle.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2956 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/xml/banner/mysql.xml
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    15092 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/data/xml/boundaries.xml
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/tamper/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1879 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/between.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      590 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/symboliclogical.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      955 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/misunion.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      753 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/schemasplit.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      906 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/dunion.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1127 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/least.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1211 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/substring2leftright.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1007 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/concat2concatws.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3046 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/luanginx.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      944 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/apostrophemask.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2589 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/space2mssqlblank.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      700 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/0eunion.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1197 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/randomcomments.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1802 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/plus2concat.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      963 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/varnish.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1314 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/multiplespaces.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1597 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/versionedkeywords.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      918 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/space2mssqlhash.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      639 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/informationschemacomment.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      559 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/ord2ascii.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1737 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/versionedmorekeywords.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      523 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/apostrophenullencode.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1413 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/percentage.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      825 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/sp_password.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      766 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/equaltorlike.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2250 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/plus2fnconcat.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1855 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/halfversionedmorekeywords.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1295 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/space2morecomment.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1201 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/modsecurityzeroversioned.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1135 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/greatest.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1290 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/bluecoat.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1065 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/uppercase.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1584 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/space2hash.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1455 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/overlongutf8more.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      680 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/decentities.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1264 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/space2dash.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1292 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/modsecurityversioned.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      715 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/hexentities.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1388 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/charencode.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      918 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/equaltolike.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1218 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/chardoubleencode.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      985 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/scientific.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1351 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/space2comment.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1306 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/unmagicquotes.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1285 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/xforwardedfor.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1282 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/space2plus.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1215 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/charunicodeescape.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      511 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/unionalltounion.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2218 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/space2morehash.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1744 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/ifnull2casewhenisnull.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      468 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/escapequotes.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1669 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/ifnull2ifisnull.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      758 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/commentbeforeparentheses.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      868 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/sleep2getlock.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1002 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/lowercase.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1225 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/commalessmid.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1646 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/charunicodeencode.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1168 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/space2mysqldash.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1377 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/hex2char.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1736 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/randomcase.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1000 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/appendnullbyte.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      519 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/base64encode.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1663 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/space2randomblank.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1295 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/binary.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1943 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/if2case.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1444 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/overlongutf8.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1977 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/space2mysqlblank.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      849 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/htmlencode.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      970 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/tamper/commalesslimit.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      258 2023-07-06 08:43:47.000000 sqlmap-1.7.7/sqlmap/__init__.py
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)    25751 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/sqlmap.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/doc/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    34109 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/doc/CHANGELOG.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    25029 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/doc/THANKS.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      190 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/doc/AUTHORS
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/doc/translations/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3281 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/doc/translations/README-it-IT.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4227 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/doc/translations/README-uk-UA.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3289 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/doc/translations/README-ko-KR.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3149 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/doc/translations/README-rs-RS.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3786 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/doc/translations/README-fa-IR.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4092 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/doc/translations/README-bg-BG.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4218 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/doc/translations/README-ru-RUS.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3055 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/doc/translations/README-id-ID.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3184 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/doc/translations/README-de-GER.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3332 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/doc/translations/README-fr-FR.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3175 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/doc/translations/README-pt-BR.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3180 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/doc/translations/README-hr-HR.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3167 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/doc/translations/README-nl-NL.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3240 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/doc/translations/README-sk-SK.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3561 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/doc/translations/README-vi-VN.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3226 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/doc/translations/README-pl-PL.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4248 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/doc/translations/README-gr-GR.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2921 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/doc/translations/README-zh-CN.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3609 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/doc/translations/README-ja-JP.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6026 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/doc/translations/README-ka-GE.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3029 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/doc/translations/README-tr-TR.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3435 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/doc/translations/README-es-MX.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    14763 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/doc/THIRD-PARTY.md
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    22119 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/sqlmap.conf
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18886 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/LICENSE
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/plugins/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/plugins/generic/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2654 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/generic/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2484 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/generic/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4909 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/generic/custom.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    30708 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/generic/entries.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    27907 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/generic/search.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1730 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/generic/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18208 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/generic/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    29216 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/generic/users.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1723 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/generic/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/generic/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6887 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/generic/misc.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    54885 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/generic/databases.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12371 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/generic/filesystem.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/presto/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1701 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/presto/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2204 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/presto/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      678 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/presto/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      971 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/presto/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5279 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/presto/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      910 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/presto/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      671 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/presto/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/hsqldb/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1445 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/hsqldb/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2784 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/hsqldb/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      687 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/hsqldb/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      971 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/hsqldb/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5276 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/hsqldb/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      909 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/hsqldb/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2537 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/hsqldb/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/mssqlserver/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18049 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/mssqlserver/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2583 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/mssqlserver/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      889 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/mssqlserver/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6499 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/mssqlserver/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6913 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/mssqlserver/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      950 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/mssqlserver/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    17213 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/mssqlserver/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/access/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2525 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/access/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2130 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/access/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      670 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/access/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1011 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/access/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5843 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/access/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      919 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/access/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      691 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/access/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/raima/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2609 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/raima/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      520 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/raima/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      687 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/raima/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1035 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/raima/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2652 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/raima/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      899 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/raima/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      703 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/raima/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/derby/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1322 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/derby/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1830 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/derby/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/derby/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      995 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/derby/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2636 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/derby/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      907 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/derby/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/derby/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/cache/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1356 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/cache/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2397 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/cache/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      735 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/cache/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      967 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/cache/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3135 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/cache/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      900 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/cache/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/cache/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/vertica/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      459 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/vertica/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1920 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/vertica/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      689 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/vertica/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      975 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/vertica/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2992 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/vertica/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      920 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/vertica/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/vertica/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/firebird/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1080 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/firebird/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2260 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/firebird/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1151 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/firebird/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      979 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/firebird/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4990 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/firebird/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      929 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/firebird/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      675 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/firebird/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/monetdb/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1103 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/monetdb/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1894 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/monetdb/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      735 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/monetdb/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      975 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/monetdb/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2549 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/monetdb/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      920 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/monetdb/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/monetdb/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/maxdb/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     9202 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/maxdb/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      507 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/maxdb/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/maxdb/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      983 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/maxdb/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3792 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/maxdb/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      903 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/maxdb/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      678 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/maxdb/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/mimersql/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      926 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/mimersql/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1858 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/mimersql/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      807 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/mimersql/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      979 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/mimersql/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2591 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/mimersql/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      930 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/mimersql/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/mimersql/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/postgresql/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      428 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/postgresql/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2097 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/postgresql/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1016 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/postgresql/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5448 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/postgresql/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     9801 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/postgresql/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1304 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/postgresql/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3005 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/postgresql/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/mysql/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      265 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/mysql/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2095 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/mysql/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1044 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/mysql/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5124 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/mysql/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12744 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/mysql/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1113 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/mysql/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7731 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/mysql/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/informix/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1022 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/informix/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1902 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/informix/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1272 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/informix/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      365 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/informix/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3284 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/informix/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      930 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/informix/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/informix/filesystem.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/altibase/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      589 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/altibase/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      506 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/altibase/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      678 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/altibase/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      979 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/altibase/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2657 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/altibase/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      930 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/altibase/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/altibase/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/extremedb/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2427 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/extremedb/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      507 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/extremedb/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/extremedb/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      983 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/extremedb/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2673 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/extremedb/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      939 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/extremedb/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      677 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/extremedb/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/mckoi/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2371 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/mckoi/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      503 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/mckoi/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/mckoi/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      967 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/mckoi/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2590 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/mckoi/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      899 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/mckoi/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      669 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/mckoi/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/db2/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      615 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/db2/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1935 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/db2/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      678 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/db2/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      365 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/db2/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5871 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/db2/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      880 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/db2/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/db2/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/cubrid/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      918 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/cubrid/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1835 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/cubrid/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      726 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/cubrid/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      971 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/cubrid/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2541 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/cubrid/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      910 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/cubrid/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/cubrid/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/h2/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1580 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/h2/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      500 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/h2/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      687 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/h2/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      955 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/h2/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3324 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/h2/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      869 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/h2/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      663 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/h2/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/oracle/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6002 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/oracle/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2817 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/oracle/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      886 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/oracle/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1101 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/oracle/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3873 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/oracle/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      909 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/oracle/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2301 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/oracle/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/cratedb/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      632 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/cratedb/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2097 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/cratedb/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/cratedb/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      975 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/cratedb/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2538 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/cratedb/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      920 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/cratedb/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      260 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/cratedb/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/sybase/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    11670 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/sybase/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2558 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/sybase/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      899 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/sybase/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      971 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/sybase/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3429 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/sybase/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      909 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/sybase/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      671 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/sybase/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/clickhouse/
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      638 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/clickhouse/enumeration.py
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      255 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/clickhouse/connector.py
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      687 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/clickhouse/syntax.py
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      987 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/clickhouse/takeover.py
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)     2627 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/clickhouse/fingerprint.py
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      950 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/clickhouse/__init__.py
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      679 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/clickhouse/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/sqlite/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2054 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/sqlite/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3083 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/sqlite/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      644 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/sqlite/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      971 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/sqlite/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3176 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/sqlite/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      909 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/sqlite/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      671 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/sqlite/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/virtuoso/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1541 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/virtuoso/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      506 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/virtuoso/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      678 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/virtuoso/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      979 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/virtuoso/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2517 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/virtuoso/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      929 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/virtuoso/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      675 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/virtuoso/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/frontbase/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      923 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/frontbase/enumeration.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      507 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/frontbase/connector.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      447 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/frontbase/syntax.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      983 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/frontbase/takeover.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2613 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/frontbase/fingerprint.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      939 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/frontbase/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      677 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/plugins/dbms/frontbase/filesystem.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/lib/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/lib/controller/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8896 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/controller/handler.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7233 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/controller/action.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    75617 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/controller/checks.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/controller/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    36761 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/controller/controller.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/lib/utils/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7907 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/utils/search.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4686 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/utils/httpd.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    48979 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/utils/hash.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2325 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/utils/getch.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5063 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/utils/sqlalchemy.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8347 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/utils/hashdb.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2935 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/utils/xrange.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      926 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/utils/versioncheck.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3337 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/utils/progress.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2674 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/utils/purge.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    10977 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/utils/crawler.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8030 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/utils/har.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    15901 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/utils/brute.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7369 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/utils/pivotdumptable.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/utils/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    34251 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/utils/api.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3190 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/utils/safe2bin.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1111 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/utils/timeout.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5564 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/utils/deps.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18275 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/utils/sgmllib.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/lib/request/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18899 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/request/basic.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6017 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/request/dns.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3229 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/request/direct.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8110 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/request/redirecthandler.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      942 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/request/rangehandler.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      590 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/request/methodrequest.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5815 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/request/httpshandler.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/request/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      633 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/request/templates.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1384 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/request/basicauthhandler.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1566 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/request/chunkedhandler.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1158 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/request/pkihandler.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    24811 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/request/inject.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    80263 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/request/connect.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7788 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/request/comparison.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/lib/techniques/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/lib/techniques/error/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    21160 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/techniques/error/use.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/techniques/error/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/lib/techniques/dns/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5061 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/techniques/dns/use.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1125 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/techniques/dns/test.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/techniques/dns/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/lib/techniques/blind/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/techniques/blind/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    34640 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/techniques/blind/inference.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/techniques/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/lib/techniques/union/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    23150 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/techniques/union/use.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18616 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/techniques/union/test.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/techniques/union/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/lib/core/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      728 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/core/data.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5865 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/core/patch.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1800 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/core/readlineng.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    28848 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/core/dump.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8414 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/core/threads.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    12888 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/core/convert.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    13908 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/core/enums.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2634 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/core/decorators.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6032 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/core/bigarray.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    10052 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/core/gui.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1646 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/core/exception.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    15220 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/core/testing.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7442 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/core/optiondict.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    34129 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/core/target.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1980 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/core/session.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    59181 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/core/agent.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   106059 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/core/option.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    45491 2023-07-06 08:43:47.000000 sqlmap-1.7.7/sqlmap/lib/core/settings.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8986 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/core/compat.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/core/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5657 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/core/subprocessng.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1876 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/core/revision.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      885 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/core/profiling.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      559 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/core/defaults.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5489 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/core/log.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4956 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/core/shell.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    17637 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/core/dicts.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3201 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/core/wordlist.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      988 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/core/unescaper.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7468 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/core/update.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     5046 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/core/replication.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6236 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/core/datatype.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)   193586 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/core/common.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/lib/takeover/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     8440 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/takeover/abstraction.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    13903 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/takeover/udf.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    28240 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/takeover/metasploit.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    11839 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/takeover/xp_cmdshell.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3838 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/takeover/registry.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    18315 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/takeover/web.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/takeover/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4739 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/takeover/icmpsh.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/lib/parse/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    49708 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/parse/cmdline.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2703 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/parse/handler.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3578 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/parse/payloads.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3498 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/parse/configfile.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1460 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/parse/headers.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1805 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/parse/sitemap.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/parse/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3580 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/parse/banner.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3022 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/lib/parse/html.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     6215 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/sqlmapapi.yaml
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/extra/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/extra/cloak/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2286 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/cloak/cloak.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      732 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/cloak/README.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/cloak/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/extra/shutils/
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      305 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/shutils/modernize.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      797 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/shutils/duplicates.py
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)     1140 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/shutils/precommit-hook.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      332 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/shutils/pycodestyle.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      660 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/shutils/drei.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      255 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/shutils/blanks.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      235 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/shutils/pylint.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)     5861 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/shutils/pypi.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      630 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/shutils/recloak.sh
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      903 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/shutils/newlines.py
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      869 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/shutils/strip.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      245 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/shutils/junk.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      311 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/shutils/autocompletion.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      313 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/shutils/pydiatra.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      875 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/shutils/postcommit-hook.sh
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)      320 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/shutils/pyflakes.sh
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/extra/runcmd/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      193 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/runcmd/README.txt
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/extra/runcmd/src/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      883 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/runcmd/src/runcmd.sln
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      271 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/runcmd/src/README.txt
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/extra/runcmd/src/runcmd/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1348 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/runcmd/src/runcmd/runcmd.cpp
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      516 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/runcmd/src/runcmd/stdafx.h
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4508 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/runcmd/src/runcmd/runcmd.vcproj
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      293 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/runcmd/src/runcmd/stdafx.cpp
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    37206 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/runcmd/runcmd.exe_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/extra/beep/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2901 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/beep/beep.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/beep/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    46772 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/beep/beep.wav
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/extra/shellcodeexec/
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/extra/shellcodeexec/linux/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1691 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/shellcodeexec/linux/shellcodeexec.x32_
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1927 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/shellcodeexec/linux/shellcodeexec.x64_
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      282 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/shellcodeexec/README.txt
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/extra/shellcodeexec/windows/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2758 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/shellcodeexec/windows/shellcodeexec.x32.exe_
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/extra/icmpsh/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3965 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/icmpsh/icmpsh-m.c
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     7009 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/icmpsh/icmpsh.exe_
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     9342 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/icmpsh/icmpsh-s.c
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1641 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/icmpsh/README.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2136 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/icmpsh/icmpsh-m.pl
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      872 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/icmpsh/__init__.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4809 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/icmpsh/icmpsh_m.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/extra/dbgtool/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     2475 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/dbgtool/dbgtool.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      549 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/dbgtool/README.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/dbgtool/__init__.py
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap/extra/vulnserver/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     9127 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/vulnserver/vulnserver.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)      147 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/extra/vulnserver/__init__.py
+-rwxr-xr-x   0 stamparm  (1000) stamparm  (1000)     2784 2023-07-06 08:43:43.000000 sqlmap-1.7.7/sqlmap/sqlmapapi.py
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       38 2023-07-06 08:43:48.000000 sqlmap-1.7.7/setup.cfg
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     3193 2023-07-06 08:43:47.000000 sqlmap-1.7.7/README.rst
+drwxrwxr-x   0 stamparm  (1000) stamparm  (1000)        0 2023-07-06 08:43:48.000000 sqlmap-1.7.7/sqlmap.egg-info/
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)    24105 2023-07-06 08:43:47.000000 sqlmap-1.7.7/sqlmap.egg-info/SOURCES.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     4952 2023-07-06 08:43:47.000000 sqlmap-1.7.7/sqlmap.egg-info/PKG-INFO
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        7 2023-07-06 08:43:47.000000 sqlmap-1.7.7/sqlmap.egg-info/top_level.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        1 2023-07-06 08:43:47.000000 sqlmap-1.7.7/sqlmap.egg-info/not-zip-safe
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)       47 2023-07-06 08:43:47.000000 sqlmap-1.7.7/sqlmap.egg-info/entry_points.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)        1 2023-07-06 08:43:47.000000 sqlmap-1.7.7/sqlmap.egg-info/dependency_links.txt
+-rw-rw-r--   0 stamparm  (1000) stamparm  (1000)     1549 2023-07-06 08:43:45.000000 sqlmap-1.7.7/setup.py
```

### Comparing `sqlmap-1.7.6/MANIFEST.in` & `sqlmap-1.7.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/PKG-INFO` & `sqlmap-1.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sqlmap
-Version: 1.7.6
+Version: 1.7.7
 Summary: Automatic SQL injection and database takeover tool
 Home-page: https://sqlmap.org
 Author: Bernardo Damele Assumpcao Guimaraes, Miroslav Stampar
 Author-email: bernardo@sqlmap.org, miroslav@sqlmap.org
 License: GNU General Public License v2 (GPLv2)
-Download-URL: https://github.com/sqlmapproject/sqlmap/archive/1.7.6.zip
+Download-URL: https://github.com/sqlmapproject/sqlmap/archive/1.7.7.zip
 Project-URL: Source, https://github.com/sqlmapproject/sqlmap/
 Project-URL: Documentation, https://github.com/sqlmapproject/sqlmap/wiki
 Project-URL: Tracker, https://github.com/sqlmapproject/sqlmap/issues
 Description: sqlmap
         ======
         
         |Python 2.6|2.7|3.x| |License| |Twitter|
```

### Comparing `sqlmap-1.7.6/sqlmap/README.md` & `sqlmap-1.7.7/sqlmap/README.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/wininetpton/win_inet_pton.py` & `sqlmap-1.7.7/sqlmap/thirdparty/wininetpton/win_inet_pton.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/clientform/clientform.py` & `sqlmap-1.7.7/sqlmap/thirdparty/clientform/clientform.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/multipart/multipartpost.py` & `sqlmap-1.7.7/sqlmap/thirdparty/multipart/multipartpost.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/socks/socks.py` & `sqlmap-1.7.7/sqlmap/thirdparty/socks/socks.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/socks/LICENSE` & `sqlmap-1.7.7/sqlmap/thirdparty/socks/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/escsm.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/eucjpprober.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/utf8prober.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/langturkishmodel.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/charsetprober.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/mbcharsetprober.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/euckrfreq.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/gb2312prober.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/cp949prober.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/chardistribution.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/enums.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/langhebrewmodel.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/langgreekmodel.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/escprober.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/codingstatemachine.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/euctwfreq.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/latin1prober.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/langbulgarianmodel.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/big5freq.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/euckrprober.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/jisfreq.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/big5prober.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/mbcssm.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/universaldetector.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/gb2312freq.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/sjisprober.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/compat.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/compat.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/sbcsgroupprober.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/__init__.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/charsetgroupprober.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/jpcntx.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/langcyrillicmodel.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/langcyrillicmodel.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/langhungarianmodel.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/euctwprober.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/sbcharsetprober.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/mbcsgroupprober.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/langthaimodel.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/chardet/hebrewprober.py` & `sqlmap-1.7.7/sqlmap/thirdparty/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/odict/ordereddict.py` & `sqlmap-1.7.7/sqlmap/thirdparty/odict/ordereddict.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/keepalive/__init__.py` & `sqlmap-1.7.7/sqlmap/thirdparty/keepalive/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/keepalive/keepalive.py` & `sqlmap-1.7.7/sqlmap/thirdparty/keepalive/keepalive.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/magic/magic.py` & `sqlmap-1.7.7/sqlmap/thirdparty/magic/magic.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/ansistrm/ansistrm.py` & `sqlmap-1.7.7/sqlmap/thirdparty/ansistrm/ansistrm.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/identywaf/identYwaf.py` & `sqlmap-1.7.7/sqlmap/thirdparty/identywaf/identYwaf.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/identywaf/data.json` & `sqlmap-1.7.7/sqlmap/thirdparty/identywaf/data.json`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/identywaf/LICENSE` & `sqlmap-1.7.7/sqlmap/thirdparty/identywaf/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/prettyprint/__init__.py` & `sqlmap-1.7.7/sqlmap/thirdparty/prettyprint/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/prettyprint/prettyprint.py` & `sqlmap-1.7.7/sqlmap/thirdparty/prettyprint/prettyprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/bottle/bottle.py` & `sqlmap-1.7.7/sqlmap/thirdparty/bottle/bottle.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/fcrypt/__init__.py` & `sqlmap-1.7.7/sqlmap/thirdparty/fcrypt/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/fcrypt/fcrypt.py` & `sqlmap-1.7.7/sqlmap/thirdparty/fcrypt/fcrypt.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/pydes/pyDes.py` & `sqlmap-1.7.7/sqlmap/thirdparty/pydes/pyDes.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/pydes/__init__.py` & `sqlmap-1.7.7/sqlmap/thirdparty/pydes/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/beautifulsoup/beautifulsoup.py` & `sqlmap-1.7.7/sqlmap/thirdparty/beautifulsoup/beautifulsoup.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/beautifulsoup/__init__.py` & `sqlmap-1.7.7/sqlmap/thirdparty/beautifulsoup/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/six/__init__.py` & `sqlmap-1.7.7/sqlmap/thirdparty/six/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/termcolor/termcolor.py` & `sqlmap-1.7.7/sqlmap/thirdparty/termcolor/termcolor.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/colorama/ansi.py` & `sqlmap-1.7.7/sqlmap/thirdparty/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/colorama/initialise.py` & `sqlmap-1.7.7/sqlmap/thirdparty/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/colorama/winterm.py` & `sqlmap-1.7.7/sqlmap/thirdparty/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/colorama/ansitowin32.py` & `sqlmap-1.7.7/sqlmap/thirdparty/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/thirdparty/colorama/win32.py` & `sqlmap-1.7.7/sqlmap/thirdparty/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/.pylintrc` & `sqlmap-1.7.7/sqlmap/.pylintrc`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/procs/postgresql/dns_request.sql` & `sqlmap-1.7.7/sqlmap/data/procs/postgresql/dns_request.sql`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/procs/oracle/read_file_export_extension.sql` & `sqlmap-1.7.7/sqlmap/data/procs/oracle/read_file_export_extension.sql`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/9.1/lib_postgresqludf_sys.so_` & `sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/9.1/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/9.0/lib_postgresqludf_sys.so_` & `sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/9.0/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/9.5/lib_postgresqludf_sys.so_` & `sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/9.5/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/9.3/lib_postgresqludf_sys.so_` & `sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/9.3/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/12/lib_postgresqludf_sys.so_` & `sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/12/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/11/lib_postgresqludf_sys.so_` & `sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/11/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/8.4/lib_postgresqludf_sys.so_` & `sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/8.4/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/8.2/lib_postgresqludf_sys.so_` & `sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/8.2/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/8.3/lib_postgresqludf_sys.so_` & `sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/8.3/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/9.4/lib_postgresqludf_sys.so_` & `sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/9.4/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/10/lib_postgresqludf_sys.so_` & `sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/10/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/9.2/lib_postgresqludf_sys.so_` & `sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/9.2/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/64/9.6/lib_postgresqludf_sys.so_` & `sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/64/9.6/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/9.1/lib_postgresqludf_sys.so_` & `sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/9.1/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/9.0/lib_postgresqludf_sys.so_` & `sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/9.0/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/9.5/lib_postgresqludf_sys.so_` & `sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/9.5/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/9.3/lib_postgresqludf_sys.so_` & `sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/9.3/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/11/lib_postgresqludf_sys.so_` & `sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/11/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/8.4/lib_postgresqludf_sys.so_` & `sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/8.4/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/8.2/lib_postgresqludf_sys.so_` & `sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/8.2/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/8.3/lib_postgresqludf_sys.so_` & `sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/8.3/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/9.4/lib_postgresqludf_sys.so_` & `sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/9.4/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/10/lib_postgresqludf_sys.so_` & `sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/10/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/9.2/lib_postgresqludf_sys.so_` & `sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/9.2/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/udf/postgresql/linux/32/9.6/lib_postgresqludf_sys.so_` & `sqlmap-1.7.7/sqlmap/data/udf/postgresql/linux/32/9.6/lib_postgresqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/udf/postgresql/windows/32/9.0/lib_postgresqludf_sys.dll_` & `sqlmap-1.7.7/sqlmap/data/udf/postgresql/windows/32/9.0/lib_postgresqludf_sys.dll_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/udf/postgresql/windows/32/8.4/lib_postgresqludf_sys.dll_` & `sqlmap-1.7.7/sqlmap/data/udf/postgresql/windows/32/8.4/lib_postgresqludf_sys.dll_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/udf/postgresql/windows/32/8.2/lib_postgresqludf_sys.dll_` & `sqlmap-1.7.7/sqlmap/data/udf/postgresql/windows/32/8.2/lib_postgresqludf_sys.dll_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/udf/postgresql/windows/32/8.3/lib_postgresqludf_sys.dll_` & `sqlmap-1.7.7/sqlmap/data/udf/postgresql/windows/32/8.3/lib_postgresqludf_sys.dll_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/udf/mysql/linux/64/lib_mysqludf_sys.so_` & `sqlmap-1.7.7/sqlmap/data/udf/mysql/linux/64/lib_mysqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/udf/mysql/linux/32/lib_mysqludf_sys.so_` & `sqlmap-1.7.7/sqlmap/data/udf/mysql/linux/32/lib_mysqludf_sys.so_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/udf/mysql/windows/64/lib_mysqludf_sys.dll_` & `sqlmap-1.7.7/sqlmap/data/udf/mysql/windows/64/lib_mysqludf_sys.dll_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/udf/mysql/windows/32/lib_mysqludf_sys.dll_` & `sqlmap-1.7.7/sqlmap/data/udf/mysql/windows/32/lib_mysqludf_sys.dll_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/shell/stagers/stager.asp_` & `sqlmap-1.7.7/sqlmap/data/shell/stagers/stager.asp_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/shell/stagers/stager.aspx_` & `sqlmap-1.7.7/sqlmap/data/shell/stagers/stager.aspx_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/shell/stagers/stager.jsp_` & `sqlmap-1.7.7/sqlmap/data/shell/stagers/stager.jsp_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/shell/README.txt` & `sqlmap-1.7.7/sqlmap/data/shell/README.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/txt/smalldict.txt` & `sqlmap-1.7.7/sqlmap/data/txt/smalldict.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/txt/common-outputs.txt` & `sqlmap-1.7.7/sqlmap/data/txt/common-outputs.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/txt/common-tables.txt` & `sqlmap-1.7.7/sqlmap/data/txt/common-tables.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/txt/user-agents.txt` & `sqlmap-1.7.7/sqlmap/data/txt/user-agents.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/txt/common-files.txt` & `sqlmap-1.7.7/sqlmap/data/txt/common-files.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/txt/keywords.txt` & `sqlmap-1.7.7/sqlmap/data/txt/keywords.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/txt/common-columns.txt` & `sqlmap-1.7.7/sqlmap/data/txt/common-columns.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/txt/wordlist.tx_` & `sqlmap-1.7.7/sqlmap/data/txt/wordlist.tx_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/html/index.html` & `sqlmap-1.7.7/sqlmap/data/html/index.html`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/xml/errors.xml` & `sqlmap-1.7.7/sqlmap/data/xml/errors.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/xml/payloads/union_query.xml` & `sqlmap-1.7.7/sqlmap/data/xml/payloads/union_query.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/xml/payloads/inline_query.xml` & `sqlmap-1.7.7/sqlmap/data/xml/payloads/inline_query.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/xml/payloads/error_based.xml` & `sqlmap-1.7.7/sqlmap/data/xml/payloads/error_based.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/xml/payloads/time_blind.xml` & `sqlmap-1.7.7/sqlmap/data/xml/payloads/time_blind.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/xml/payloads/stacked_queries.xml` & `sqlmap-1.7.7/sqlmap/data/xml/payloads/stacked_queries.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/xml/payloads/boolean_blind.xml` & `sqlmap-1.7.7/sqlmap/data/xml/payloads/boolean_blind.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/xml/queries.xml` & `sqlmap-1.7.7/sqlmap/data/xml/queries.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/xml/banner/x-powered-by.xml` & `sqlmap-1.7.7/sqlmap/data/xml/banner/x-powered-by.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/xml/banner/set-cookie.xml` & `sqlmap-1.7.7/sqlmap/data/xml/banner/set-cookie.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/xml/banner/mssql.xml` & `sqlmap-1.7.7/sqlmap/data/xml/banner/mssql.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/xml/banner/servlet-engine.xml` & `sqlmap-1.7.7/sqlmap/data/xml/banner/servlet-engine.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/xml/banner/generic.xml` & `sqlmap-1.7.7/sqlmap/data/xml/banner/generic.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/xml/banner/server.xml` & `sqlmap-1.7.7/sqlmap/data/xml/banner/server.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/xml/banner/mysql.xml` & `sqlmap-1.7.7/sqlmap/data/xml/banner/mysql.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/data/xml/boundaries.xml` & `sqlmap-1.7.7/sqlmap/data/xml/boundaries.xml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/between.py` & `sqlmap-1.7.7/sqlmap/tamper/between.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/symboliclogical.py` & `sqlmap-1.7.7/sqlmap/tamper/symboliclogical.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/misunion.py` & `sqlmap-1.7.7/sqlmap/tamper/misunion.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/schemasplit.py` & `sqlmap-1.7.7/sqlmap/tamper/schemasplit.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/dunion.py` & `sqlmap-1.7.7/sqlmap/tamper/dunion.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/least.py` & `sqlmap-1.7.7/sqlmap/tamper/least.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/substring2leftright.py` & `sqlmap-1.7.7/sqlmap/tamper/substring2leftright.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/concat2concatws.py` & `sqlmap-1.7.7/sqlmap/tamper/concat2concatws.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/luanginx.py` & `sqlmap-1.7.7/sqlmap/tamper/luanginx.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/apostrophemask.py` & `sqlmap-1.7.7/sqlmap/tamper/apostrophemask.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/space2mssqlblank.py` & `sqlmap-1.7.7/sqlmap/tamper/space2mssqlblank.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/0eunion.py` & `sqlmap-1.7.7/sqlmap/tamper/0eunion.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/randomcomments.py` & `sqlmap-1.7.7/sqlmap/tamper/randomcomments.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/plus2concat.py` & `sqlmap-1.7.7/sqlmap/tamper/plus2concat.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/varnish.py` & `sqlmap-1.7.7/sqlmap/tamper/varnish.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/multiplespaces.py` & `sqlmap-1.7.7/sqlmap/tamper/multiplespaces.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/versionedkeywords.py` & `sqlmap-1.7.7/sqlmap/tamper/versionedkeywords.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/space2mssqlhash.py` & `sqlmap-1.7.7/sqlmap/tamper/space2mssqlhash.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/informationschemacomment.py` & `sqlmap-1.7.7/sqlmap/tamper/informationschemacomment.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/ord2ascii.py` & `sqlmap-1.7.7/sqlmap/tamper/ord2ascii.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/versionedmorekeywords.py` & `sqlmap-1.7.7/sqlmap/tamper/versionedmorekeywords.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/apostrophenullencode.py` & `sqlmap-1.7.7/sqlmap/tamper/apostrophenullencode.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/percentage.py` & `sqlmap-1.7.7/sqlmap/tamper/percentage.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/sp_password.py` & `sqlmap-1.7.7/sqlmap/tamper/sp_password.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/equaltorlike.py` & `sqlmap-1.7.7/sqlmap/tamper/equaltorlike.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/plus2fnconcat.py` & `sqlmap-1.7.7/sqlmap/tamper/plus2fnconcat.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/halfversionedmorekeywords.py` & `sqlmap-1.7.7/sqlmap/tamper/halfversionedmorekeywords.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/space2morecomment.py` & `sqlmap-1.7.7/sqlmap/tamper/space2morecomment.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/modsecurityzeroversioned.py` & `sqlmap-1.7.7/sqlmap/tamper/modsecurityzeroversioned.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/greatest.py` & `sqlmap-1.7.7/sqlmap/tamper/greatest.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/bluecoat.py` & `sqlmap-1.7.7/sqlmap/tamper/bluecoat.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/uppercase.py` & `sqlmap-1.7.7/sqlmap/tamper/uppercase.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/space2hash.py` & `sqlmap-1.7.7/sqlmap/tamper/space2hash.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/overlongutf8more.py` & `sqlmap-1.7.7/sqlmap/tamper/overlongutf8more.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/decentities.py` & `sqlmap-1.7.7/sqlmap/tamper/decentities.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/space2dash.py` & `sqlmap-1.7.7/sqlmap/tamper/space2dash.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/modsecurityversioned.py` & `sqlmap-1.7.7/sqlmap/tamper/modsecurityversioned.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/hexentities.py` & `sqlmap-1.7.7/sqlmap/tamper/hexentities.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/charencode.py` & `sqlmap-1.7.7/sqlmap/tamper/charencode.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/equaltolike.py` & `sqlmap-1.7.7/sqlmap/tamper/equaltolike.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/chardoubleencode.py` & `sqlmap-1.7.7/sqlmap/tamper/chardoubleencode.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/scientific.py` & `sqlmap-1.7.7/sqlmap/tamper/scientific.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/space2comment.py` & `sqlmap-1.7.7/sqlmap/tamper/space2comment.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/unmagicquotes.py` & `sqlmap-1.7.7/sqlmap/tamper/unmagicquotes.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/xforwardedfor.py` & `sqlmap-1.7.7/sqlmap/tamper/xforwardedfor.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/space2plus.py` & `sqlmap-1.7.7/sqlmap/tamper/space2plus.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/charunicodeescape.py` & `sqlmap-1.7.7/sqlmap/tamper/charunicodeescape.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/space2morehash.py` & `sqlmap-1.7.7/sqlmap/tamper/space2morehash.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/ifnull2casewhenisnull.py` & `sqlmap-1.7.7/sqlmap/tamper/ifnull2casewhenisnull.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/ifnull2ifisnull.py` & `sqlmap-1.7.7/sqlmap/tamper/ifnull2ifisnull.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/commentbeforeparentheses.py` & `sqlmap-1.7.7/sqlmap/tamper/commentbeforeparentheses.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/sleep2getlock.py` & `sqlmap-1.7.7/sqlmap/tamper/sleep2getlock.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/lowercase.py` & `sqlmap-1.7.7/sqlmap/tamper/lowercase.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/commalessmid.py` & `sqlmap-1.7.7/sqlmap/tamper/commalessmid.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/charunicodeencode.py` & `sqlmap-1.7.7/sqlmap/tamper/charunicodeencode.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/space2mysqldash.py` & `sqlmap-1.7.7/sqlmap/tamper/space2mysqldash.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/hex2char.py` & `sqlmap-1.7.7/sqlmap/tamper/hex2char.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/randomcase.py` & `sqlmap-1.7.7/sqlmap/tamper/randomcase.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/appendnullbyte.py` & `sqlmap-1.7.7/sqlmap/tamper/appendnullbyte.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/base64encode.py` & `sqlmap-1.7.7/sqlmap/tamper/base64encode.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/space2randomblank.py` & `sqlmap-1.7.7/sqlmap/tamper/space2randomblank.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/binary.py` & `sqlmap-1.7.7/sqlmap/tamper/binary.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/if2case.py` & `sqlmap-1.7.7/sqlmap/tamper/if2case.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/overlongutf8.py` & `sqlmap-1.7.7/sqlmap/tamper/overlongutf8.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/space2mysqlblank.py` & `sqlmap-1.7.7/sqlmap/tamper/space2mysqlblank.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/htmlencode.py` & `sqlmap-1.7.7/sqlmap/tamper/htmlencode.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/tamper/commalesslimit.py` & `sqlmap-1.7.7/sqlmap/tamper/commalesslimit.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/sqlmap.py` & `sqlmap-1.7.7/sqlmap/sqlmap.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/doc/CHANGELOG.md` & `sqlmap-1.7.7/sqlmap/doc/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/doc/THANKS.md` & `sqlmap-1.7.7/sqlmap/doc/THANKS.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/doc/translations/README-it-IT.md` & `sqlmap-1.7.7/sqlmap/doc/translations/README-it-IT.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/doc/translations/README-uk-UA.md` & `sqlmap-1.7.7/sqlmap/doc/translations/README-uk-UA.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/doc/translations/README-ko-KR.md` & `sqlmap-1.7.7/sqlmap/doc/translations/README-ko-KR.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/doc/translations/README-rs-RS.md` & `sqlmap-1.7.7/sqlmap/doc/translations/README-rs-RS.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/doc/translations/README-fa-IR.md` & `sqlmap-1.7.7/sqlmap/doc/translations/README-fa-IR.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/doc/translations/README-bg-BG.md` & `sqlmap-1.7.7/sqlmap/doc/translations/README-bg-BG.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/doc/translations/README-ru-RUS.md` & `sqlmap-1.7.7/sqlmap/doc/translations/README-ru-RUS.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/doc/translations/README-id-ID.md` & `sqlmap-1.7.7/sqlmap/doc/translations/README-id-ID.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/doc/translations/README-de-GER.md` & `sqlmap-1.7.7/sqlmap/doc/translations/README-de-GER.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/doc/translations/README-fr-FR.md` & `sqlmap-1.7.7/sqlmap/doc/translations/README-fr-FR.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/doc/translations/README-pt-BR.md` & `sqlmap-1.7.7/sqlmap/doc/translations/README-pt-BR.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/doc/translations/README-hr-HR.md` & `sqlmap-1.7.7/sqlmap/doc/translations/README-hr-HR.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/doc/translations/README-nl-NL.md` & `sqlmap-1.7.7/sqlmap/doc/translations/README-nl-NL.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/doc/translations/README-sk-SK.md` & `sqlmap-1.7.7/sqlmap/doc/translations/README-sk-SK.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/doc/translations/README-vi-VN.md` & `sqlmap-1.7.7/sqlmap/doc/translations/README-vi-VN.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/doc/translations/README-pl-PL.md` & `sqlmap-1.7.7/sqlmap/doc/translations/README-pl-PL.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/doc/translations/README-gr-GR.md` & `sqlmap-1.7.7/sqlmap/doc/translations/README-gr-GR.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/doc/translations/README-zh-CN.md` & `sqlmap-1.7.7/sqlmap/doc/translations/README-zh-CN.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/doc/translations/README-ja-JP.md` & `sqlmap-1.7.7/sqlmap/doc/translations/README-ja-JP.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/doc/translations/README-ka-GE.md` & `sqlmap-1.7.7/sqlmap/doc/translations/README-ka-GE.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/doc/translations/README-tr-TR.md` & `sqlmap-1.7.7/sqlmap/doc/translations/README-tr-TR.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/doc/translations/README-es-MX.md` & `sqlmap-1.7.7/sqlmap/doc/translations/README-es-MX.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/doc/THIRD-PARTY.md` & `sqlmap-1.7.7/sqlmap/doc/THIRD-PARTY.md`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/sqlmap.conf` & `sqlmap-1.7.7/sqlmap/sqlmap.conf`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/LICENSE` & `sqlmap-1.7.7/sqlmap/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/generic/enumeration.py` & `sqlmap-1.7.7/sqlmap/plugins/generic/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/generic/connector.py` & `sqlmap-1.7.7/sqlmap/plugins/generic/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/generic/custom.py` & `sqlmap-1.7.7/sqlmap/plugins/generic/custom.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/generic/entries.py` & `sqlmap-1.7.7/sqlmap/plugins/generic/entries.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/generic/search.py` & `sqlmap-1.7.7/sqlmap/plugins/generic/search.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/generic/syntax.py` & `sqlmap-1.7.7/sqlmap/plugins/generic/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/generic/takeover.py` & `sqlmap-1.7.7/sqlmap/plugins/generic/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/generic/users.py` & `sqlmap-1.7.7/sqlmap/plugins/generic/users.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/generic/fingerprint.py` & `sqlmap-1.7.7/sqlmap/plugins/generic/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/generic/misc.py` & `sqlmap-1.7.7/sqlmap/plugins/generic/misc.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/generic/databases.py` & `sqlmap-1.7.7/sqlmap/plugins/generic/databases.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/generic/filesystem.py` & `sqlmap-1.7.7/sqlmap/plugins/generic/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/presto/enumeration.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/presto/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/presto/connector.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/presto/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/presto/syntax.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/presto/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/presto/takeover.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/presto/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/presto/fingerprint.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/presto/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/presto/__init__.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/presto/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/presto/filesystem.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/presto/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/hsqldb/enumeration.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/hsqldb/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/hsqldb/connector.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/hsqldb/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/hsqldb/syntax.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/hsqldb/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/hsqldb/takeover.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/hsqldb/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/hsqldb/fingerprint.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/hsqldb/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/hsqldb/__init__.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/hsqldb/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/hsqldb/filesystem.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/hsqldb/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/mssqlserver/enumeration.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/mssqlserver/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/mssqlserver/connector.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/mssqlserver/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/mssqlserver/syntax.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/mssqlserver/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/mssqlserver/takeover.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/mssqlserver/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/mssqlserver/fingerprint.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/mssqlserver/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/mssqlserver/__init__.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/mssqlserver/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/mssqlserver/filesystem.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/mssqlserver/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/access/enumeration.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/access/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/access/connector.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/access/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/access/syntax.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/access/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/access/takeover.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/access/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/access/fingerprint.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/access/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/access/__init__.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/access/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/access/filesystem.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/access/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/raima/enumeration.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/raima/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/raima/connector.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/raima/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/raima/syntax.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/raima/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/raima/takeover.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/raima/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/raima/fingerprint.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/raima/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/raima/__init__.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/raima/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/raima/filesystem.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/raima/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/derby/enumeration.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/derby/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/derby/connector.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/derby/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/derby/takeover.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/derby/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/derby/fingerprint.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/derby/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/derby/__init__.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/derby/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/cache/enumeration.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/cache/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/cache/connector.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/cache/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/cache/syntax.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/cache/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/cache/takeover.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/cache/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/cache/fingerprint.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/cache/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/cache/__init__.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/vertica/connector.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/vertica/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/vertica/syntax.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/vertica/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/vertica/takeover.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/vertica/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/vertica/fingerprint.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/vertica/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/vertica/__init__.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/vertica/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/firebird/enumeration.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/firebird/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/firebird/connector.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/firebird/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/firebird/syntax.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/firebird/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/firebird/takeover.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/firebird/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/firebird/fingerprint.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/firebird/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/firebird/__init__.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/firebird/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/firebird/filesystem.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/firebird/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/monetdb/enumeration.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/monetdb/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/monetdb/connector.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/monetdb/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/monetdb/syntax.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/monetdb/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/monetdb/takeover.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/monetdb/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/monetdb/fingerprint.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/monetdb/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/monetdb/__init__.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/monetdb/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/maxdb/enumeration.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/maxdb/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/maxdb/takeover.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/maxdb/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/maxdb/fingerprint.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/maxdb/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/maxdb/__init__.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/maxdb/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/maxdb/filesystem.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/maxdb/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/mimersql/enumeration.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/mimersql/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/mimersql/connector.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/mimersql/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/mimersql/syntax.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/mimersql/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/mimersql/takeover.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/mimersql/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/mimersql/fingerprint.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/mimersql/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/mimersql/__init__.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/mimersql/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/postgresql/connector.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/postgresql/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/postgresql/syntax.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/postgresql/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/postgresql/takeover.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/postgresql/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/postgresql/fingerprint.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/postgresql/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/postgresql/__init__.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/postgresql/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/postgresql/filesystem.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/postgresql/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/mysql/connector.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/mysql/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/mysql/syntax.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/mysql/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/mysql/takeover.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/mysql/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/mysql/fingerprint.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/mysql/fingerprint.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,17 +41,17 @@
 
             return None
 
         # Reference: https://downloads.mysql.com/archives/community/
         # Reference: https://dev.mysql.com/doc/relnotes/mysql/<major>.<minor>/en/
 
         versions = (
-            (80000, 80029),  # MySQL 8.0
+            (80000, 80033),  # MySQL 8.0
             (60000, 60014),  # MySQL 6.0
-            (50700, 50741),  # MySQL 5.7
+            (50700, 50742),  # MySQL 5.7
             (50600, 50652),  # MySQL 5.6
             (50500, 50563),  # MySQL 5.5
             (50400, 50404),  # MySQL 5.4
             (50100, 50174),  # MySQL 5.1
             (50000, 50097),  # MySQL 5.0
             (40100, 40131),  # MySQL 4.1
             (40000, 40032),  # MySQL 4.0
```

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/mysql/__init__.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/mysql/filesystem.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/mysql/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/informix/enumeration.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/informix/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/informix/connector.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/informix/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/informix/syntax.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/informix/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/informix/fingerprint.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/informix/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/informix/__init__.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/informix/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/altibase/enumeration.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/altibase/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/altibase/syntax.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/altibase/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/altibase/takeover.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/altibase/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/altibase/fingerprint.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/altibase/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/altibase/__init__.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/altibase/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/extremedb/enumeration.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/extremedb/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/extremedb/takeover.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/extremedb/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/extremedb/fingerprint.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/extremedb/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/extremedb/__init__.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/extremedb/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/extremedb/filesystem.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/extremedb/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/mckoi/enumeration.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/mckoi/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/mckoi/takeover.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/mckoi/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/mckoi/fingerprint.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/mckoi/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/mckoi/__init__.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/mckoi/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/mckoi/filesystem.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/mckoi/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/db2/enumeration.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/db2/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/db2/connector.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/db2/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/db2/syntax.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/db2/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/db2/fingerprint.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/db2/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/db2/__init__.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/db2/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/cubrid/enumeration.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/cubrid/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/cubrid/connector.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/cubrid/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/cubrid/syntax.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/cubrid/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/cubrid/takeover.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/cubrid/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/cubrid/fingerprint.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/cubrid/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/cubrid/__init__.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/cubrid/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/h2/enumeration.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/h2/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/h2/syntax.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/h2/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/h2/takeover.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/h2/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/h2/fingerprint.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/h2/fingerprint.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             self.getBanner()
 
             return True
 
         infoMsg = "testing %s" % DBMS.H2
         logger.info(infoMsg)
 
-        result = inject.checkBooleanExpression("ZERO() IS 0")
+        result = inject.checkBooleanExpression("ZERO()=0")
 
         if result:
             infoMsg = "confirming %s" % DBMS.H2
             logger.info(infoMsg)
 
             result = inject.checkBooleanExpression("ROUNDMAGIC(PI())>=3")
```

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/h2/__init__.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/h2/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/h2/filesystem.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/h2/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/oracle/enumeration.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/oracle/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/oracle/connector.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/oracle/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/oracle/syntax.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/oracle/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/oracle/takeover.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/oracle/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/oracle/fingerprint.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/oracle/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/oracle/__init__.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/oracle/filesystem.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/oracle/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/cratedb/enumeration.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/cratedb/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/cratedb/connector.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/cratedb/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/cratedb/takeover.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/cratedb/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/cratedb/fingerprint.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/cratedb/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/cratedb/__init__.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/cratedb/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/sybase/enumeration.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/sybase/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/sybase/connector.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/sybase/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/sybase/syntax.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/sybase/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/sybase/takeover.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/sybase/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/sybase/fingerprint.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/sybase/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/sybase/__init__.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/sybase/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/sybase/filesystem.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/sybase/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/clickhouse/enumeration.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/clickhouse/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/clickhouse/syntax.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/clickhouse/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/clickhouse/takeover.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/clickhouse/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/clickhouse/fingerprint.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/clickhouse/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/clickhouse/__init__.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/clickhouse/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/clickhouse/filesystem.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/clickhouse/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/sqlite/enumeration.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/sqlite/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/sqlite/connector.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/sqlite/connector.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/sqlite/syntax.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/sqlite/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/sqlite/takeover.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/sqlite/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/sqlite/fingerprint.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/sqlite/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/sqlite/__init__.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/sqlite/filesystem.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/sqlite/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/virtuoso/enumeration.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/virtuoso/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/virtuoso/syntax.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/virtuoso/syntax.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/virtuoso/takeover.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/virtuoso/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/virtuoso/fingerprint.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/virtuoso/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/virtuoso/__init__.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/virtuoso/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/virtuoso/filesystem.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/virtuoso/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/frontbase/enumeration.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/frontbase/enumeration.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/frontbase/takeover.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/frontbase/takeover.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/frontbase/fingerprint.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/frontbase/fingerprint.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/frontbase/__init__.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/frontbase/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/plugins/dbms/frontbase/filesystem.py` & `sqlmap-1.7.7/sqlmap/plugins/dbms/frontbase/filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/controller/handler.py` & `sqlmap-1.7.7/sqlmap/lib/controller/handler.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/controller/action.py` & `sqlmap-1.7.7/sqlmap/lib/controller/action.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/controller/checks.py` & `sqlmap-1.7.7/sqlmap/lib/controller/checks.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/controller/controller.py` & `sqlmap-1.7.7/sqlmap/lib/controller/controller.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/utils/search.py` & `sqlmap-1.7.7/sqlmap/lib/utils/search.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/utils/httpd.py` & `sqlmap-1.7.7/sqlmap/lib/utils/httpd.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/utils/hash.py` & `sqlmap-1.7.7/sqlmap/lib/utils/hash.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/utils/getch.py` & `sqlmap-1.7.7/sqlmap/lib/utils/getch.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/utils/sqlalchemy.py` & `sqlmap-1.7.7/sqlmap/lib/utils/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/utils/hashdb.py` & `sqlmap-1.7.7/sqlmap/lib/utils/hashdb.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/utils/xrange.py` & `sqlmap-1.7.7/sqlmap/lib/utils/xrange.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/utils/versioncheck.py` & `sqlmap-1.7.7/sqlmap/lib/utils/versioncheck.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/utils/progress.py` & `sqlmap-1.7.7/sqlmap/lib/utils/progress.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/utils/purge.py` & `sqlmap-1.7.7/sqlmap/lib/utils/purge.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/utils/crawler.py` & `sqlmap-1.7.7/sqlmap/lib/utils/crawler.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/utils/har.py` & `sqlmap-1.7.7/sqlmap/lib/utils/har.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/utils/brute.py` & `sqlmap-1.7.7/sqlmap/lib/utils/brute.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/utils/pivotdumptable.py` & `sqlmap-1.7.7/sqlmap/lib/utils/pivotdumptable.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/utils/api.py` & `sqlmap-1.7.7/sqlmap/lib/utils/api.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/utils/safe2bin.py` & `sqlmap-1.7.7/sqlmap/lib/utils/safe2bin.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/utils/timeout.py` & `sqlmap-1.7.7/sqlmap/lib/utils/timeout.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/utils/deps.py` & `sqlmap-1.7.7/sqlmap/lib/utils/deps.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/utils/sgmllib.py` & `sqlmap-1.7.7/sqlmap/lib/utils/sgmllib.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/request/basic.py` & `sqlmap-1.7.7/sqlmap/lib/request/basic.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/request/dns.py` & `sqlmap-1.7.7/sqlmap/lib/request/dns.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/request/direct.py` & `sqlmap-1.7.7/sqlmap/lib/request/direct.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/request/redirecthandler.py` & `sqlmap-1.7.7/sqlmap/lib/request/redirecthandler.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/request/rangehandler.py` & `sqlmap-1.7.7/sqlmap/lib/request/rangehandler.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/request/methodrequest.py` & `sqlmap-1.7.7/sqlmap/lib/request/methodrequest.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/request/httpshandler.py` & `sqlmap-1.7.7/sqlmap/lib/request/httpshandler.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/request/templates.py` & `sqlmap-1.7.7/sqlmap/lib/request/templates.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/request/basicauthhandler.py` & `sqlmap-1.7.7/sqlmap/lib/request/basicauthhandler.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/request/chunkedhandler.py` & `sqlmap-1.7.7/sqlmap/lib/request/chunkedhandler.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/request/pkihandler.py` & `sqlmap-1.7.7/sqlmap/lib/request/pkihandler.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/request/inject.py` & `sqlmap-1.7.7/sqlmap/lib/request/inject.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/request/connect.py` & `sqlmap-1.7.7/sqlmap/lib/request/connect.py`

 * *Files 0% similar despite different names*

```diff
@@ -437,29 +437,26 @@
             elif get:
                 url = "%s?%s" % (url, get)
                 requestMsg += "?%s" % get
 
             requestMsg += " %s" % _http_client.HTTPConnection._http_vsn_str
 
             # Prepare HTTP headers
-            headers = forgeHeaders({HTTP_HEADER.COOKIE: cookie, HTTP_HEADER.USER_AGENT: ua, HTTP_HEADER.REFERER: referer, HTTP_HEADER.HOST: host}, base=None if target else {})
+            headers = forgeHeaders({HTTP_HEADER.COOKIE: cookie, HTTP_HEADER.USER_AGENT: ua, HTTP_HEADER.REFERER: referer, HTTP_HEADER.HOST: getHeader(dict(conf.httpHeaders), HTTP_HEADER.HOST) or getHostHeader(url)}, base=None if target else {})
 
             if HTTP_HEADER.COOKIE in headers:
                 cookie = headers[HTTP_HEADER.COOKIE]
 
             if kb.authHeader:
                 headers[HTTP_HEADER.AUTHORIZATION] = kb.authHeader
 
             if kb.proxyAuthHeader:
                 headers[HTTP_HEADER.PROXY_AUTHORIZATION] = kb.proxyAuthHeader
 
             if not conf.requestFile or not target:
-                if not getHeader(headers, HTTP_HEADER.HOST):
-                    headers[HTTP_HEADER.HOST] = getHostHeader(url)
-
                 if not getHeader(headers, HTTP_HEADER.ACCEPT):
                     headers[HTTP_HEADER.ACCEPT] = HTTP_ACCEPT_HEADER_VALUE
 
                 if not getHeader(headers, HTTP_HEADER.ACCEPT_ENCODING):
                     headers[HTTP_HEADER.ACCEPT_ENCODING] = HTTP_ACCEPT_ENCODING_HEADER_VALUE if kb.pageCompress else "identity"
 
             elif conf.requestFile and getHeader(headers, HTTP_HEADER.USER_AGENT) == DEFAULT_USER_AGENT:
```

### Comparing `sqlmap-1.7.6/sqlmap/lib/request/comparison.py` & `sqlmap-1.7.7/sqlmap/lib/request/comparison.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/techniques/error/use.py` & `sqlmap-1.7.7/sqlmap/lib/techniques/error/use.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/techniques/dns/use.py` & `sqlmap-1.7.7/sqlmap/lib/techniques/dns/use.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/techniques/dns/test.py` & `sqlmap-1.7.7/sqlmap/lib/techniques/dns/test.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/techniques/blind/inference.py` & `sqlmap-1.7.7/sqlmap/lib/techniques/blind/inference.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/techniques/union/use.py` & `sqlmap-1.7.7/sqlmap/lib/techniques/union/use.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/techniques/union/test.py` & `sqlmap-1.7.7/sqlmap/lib/techniques/union/test.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/core/data.py` & `sqlmap-1.7.7/sqlmap/lib/core/data.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/core/patch.py` & `sqlmap-1.7.7/sqlmap/lib/core/patch.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/core/readlineng.py` & `sqlmap-1.7.7/sqlmap/lib/core/readlineng.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/core/dump.py` & `sqlmap-1.7.7/sqlmap/lib/core/dump.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/core/threads.py` & `sqlmap-1.7.7/sqlmap/lib/core/threads.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/core/convert.py` & `sqlmap-1.7.7/sqlmap/lib/core/convert.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/core/enums.py` & `sqlmap-1.7.7/sqlmap/lib/core/enums.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/core/decorators.py` & `sqlmap-1.7.7/sqlmap/lib/core/decorators.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/core/bigarray.py` & `sqlmap-1.7.7/sqlmap/lib/core/bigarray.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/core/gui.py` & `sqlmap-1.7.7/sqlmap/lib/core/gui.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/core/exception.py` & `sqlmap-1.7.7/sqlmap/lib/core/exception.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/core/testing.py` & `sqlmap-1.7.7/sqlmap/lib/core/testing.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/core/optiondict.py` & `sqlmap-1.7.7/sqlmap/lib/core/optiondict.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/core/target.py` & `sqlmap-1.7.7/sqlmap/lib/core/target.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/core/session.py` & `sqlmap-1.7.7/sqlmap/lib/core/session.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/core/agent.py` & `sqlmap-1.7.7/sqlmap/lib/core/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,15 +218,16 @@
                 retVal = paramString.replace("%s%s" % (origValue, BOUNDED_INJECTION_MARKER), self.addPayloadDelimiters(newValue))
         elif place in (PLACE.USER_AGENT, PLACE.REFERER, PLACE.HOST):
             retVal = paramString.replace(origValue, self.addPayloadDelimiters(newValue))
         else:
             def _(pattern, repl, string):
                 retVal = string
                 match = None
-                for match in re.finditer(pattern, string):
+
+                for match in re.finditer(pattern, string or ""):
                     pass
 
                 if match:
                     while True:
                         _ = re.search(r"\\g<([^>]+)>", repl)
                         if _:
                             try:
```

### Comparing `sqlmap-1.7.6/sqlmap/lib/core/option.py` & `sqlmap-1.7.7/sqlmap/lib/core/option.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/core/settings.py` & `sqlmap-1.7.7/sqlmap/lib/core/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from lib.core.enums import DBMS
 from lib.core.enums import DBMS_DIRECTORY_NAME
 from lib.core.enums import OS
 from thirdparty import six
 from thirdparty.six import unichr as _unichr
 
 # sqlmap version (<major>.<minor>.<month>.<monthly commit>)
-VERSION = "1.7.6"
+VERSION = "1.7.7"
 TYPE = "pip"
 TYPE_COLORS = {"dev": 33, "stable": 90, "pip": 34}
 VERSION_STRING = "sqlmap/%s#%s" % ('.'.join(VERSION.split('.')[:-1]) if VERSION.count('.') > 2 and VERSION.split('.')[-1] == '0' else VERSION, TYPE)
 DESCRIPTION = "automatic SQL injection and database takeover tool"
 SITE = "https://sqlmap.org"
 DEFAULT_USER_AGENT = "%s (%s)" % (VERSION_STRING, SITE)
 DEV_EMAIL_ADDRESS = "dev@sqlmap.org"
```

### Comparing `sqlmap-1.7.6/sqlmap/lib/core/compat.py` & `sqlmap-1.7.7/sqlmap/lib/core/compat.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/core/subprocessng.py` & `sqlmap-1.7.7/sqlmap/lib/core/subprocessng.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/core/revision.py` & `sqlmap-1.7.7/sqlmap/lib/core/revision.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/core/profiling.py` & `sqlmap-1.7.7/sqlmap/lib/core/profiling.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/core/defaults.py` & `sqlmap-1.7.7/sqlmap/lib/core/defaults.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/core/log.py` & `sqlmap-1.7.7/sqlmap/lib/core/log.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/core/shell.py` & `sqlmap-1.7.7/sqlmap/lib/core/shell.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/core/dicts.py` & `sqlmap-1.7.7/sqlmap/lib/core/dicts.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/core/wordlist.py` & `sqlmap-1.7.7/sqlmap/lib/core/wordlist.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/core/unescaper.py` & `sqlmap-1.7.7/sqlmap/lib/core/unescaper.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/core/update.py` & `sqlmap-1.7.7/sqlmap/lib/core/update.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/core/replication.py` & `sqlmap-1.7.7/sqlmap/lib/core/replication.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/core/datatype.py` & `sqlmap-1.7.7/sqlmap/lib/core/datatype.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/core/common.py` & `sqlmap-1.7.7/sqlmap/lib/core/common.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/takeover/abstraction.py` & `sqlmap-1.7.7/sqlmap/lib/takeover/abstraction.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/takeover/udf.py` & `sqlmap-1.7.7/sqlmap/lib/takeover/udf.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/takeover/metasploit.py` & `sqlmap-1.7.7/sqlmap/lib/takeover/metasploit.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/takeover/xp_cmdshell.py` & `sqlmap-1.7.7/sqlmap/lib/takeover/xp_cmdshell.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/takeover/registry.py` & `sqlmap-1.7.7/sqlmap/lib/takeover/registry.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/takeover/web.py` & `sqlmap-1.7.7/sqlmap/lib/takeover/web.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/takeover/icmpsh.py` & `sqlmap-1.7.7/sqlmap/lib/takeover/icmpsh.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/parse/cmdline.py` & `sqlmap-1.7.7/sqlmap/lib/parse/cmdline.py`

 * *Files 0% similar despite different names*

```diff
@@ -997,14 +997,17 @@
                 argv[i] = ""
             elif argv[i].startswith("--data-raw"):
                 argv[i] = argv[i].replace("--data-raw", "--data", 1)
             elif argv[i].startswith("--auth-creds"):
                 argv[i] = argv[i].replace("--auth-creds", "--auth-cred", 1)
             elif argv[i].startswith("--drop-cookie"):
                 argv[i] = argv[i].replace("--drop-cookie", "--drop-set-cookie", 1)
+            elif re.search(r"\A--tamper[^=\s]", argv[i]):
+                argv[i] = ""
+                continue
             elif re.search(r"\A(--(tamper|ignore-code|skip))(?!-)", argv[i]):
                 key = re.search(r"\-?\-(\w+)\b", argv[i]).group(1)
                 index = auxIndexes.get(key, None)
                 if index is None:
                     index = i if '=' in argv[i] else (i + 1 if i + 1 < len(argv) and not argv[i + 1].startswith('-') else None)
                     auxIndexes[key] = index
                 else:
```

### Comparing `sqlmap-1.7.6/sqlmap/lib/parse/handler.py` & `sqlmap-1.7.7/sqlmap/lib/parse/handler.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/parse/payloads.py` & `sqlmap-1.7.7/sqlmap/lib/parse/payloads.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/parse/configfile.py` & `sqlmap-1.7.7/sqlmap/lib/parse/configfile.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/parse/headers.py` & `sqlmap-1.7.7/sqlmap/lib/parse/headers.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/parse/sitemap.py` & `sqlmap-1.7.7/sqlmap/lib/parse/sitemap.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/parse/banner.py` & `sqlmap-1.7.7/sqlmap/lib/parse/banner.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/lib/parse/html.py` & `sqlmap-1.7.7/sqlmap/lib/parse/html.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/sqlmapapi.yaml` & `sqlmap-1.7.7/sqlmap/sqlmapapi.yaml`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/extra/cloak/cloak.py` & `sqlmap-1.7.7/sqlmap/extra/cloak/cloak.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/extra/cloak/README.txt` & `sqlmap-1.7.7/sqlmap/extra/cloak/README.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/extra/shutils/duplicates.py` & `sqlmap-1.7.7/sqlmap/extra/shutils/duplicates.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/extra/shutils/precommit-hook.sh` & `sqlmap-1.7.7/sqlmap/extra/shutils/precommit-hook.sh`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/extra/shutils/drei.sh` & `sqlmap-1.7.7/sqlmap/extra/shutils/drei.sh`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/extra/shutils/pypi.sh` & `sqlmap-1.7.7/sqlmap/extra/shutils/pypi.sh`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/extra/shutils/recloak.sh` & `sqlmap-1.7.7/sqlmap/extra/shutils/recloak.sh`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/extra/shutils/newlines.py` & `sqlmap-1.7.7/sqlmap/extra/shutils/newlines.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/extra/shutils/strip.sh` & `sqlmap-1.7.7/sqlmap/extra/shutils/strip.sh`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/extra/shutils/postcommit-hook.sh` & `sqlmap-1.7.7/sqlmap/extra/shutils/postcommit-hook.sh`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/extra/runcmd/src/runcmd.sln` & `sqlmap-1.7.7/sqlmap/extra/runcmd/src/runcmd.sln`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/extra/runcmd/src/runcmd/runcmd.cpp` & `sqlmap-1.7.7/sqlmap/extra/runcmd/src/runcmd/runcmd.cpp`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/extra/runcmd/src/runcmd/stdafx.h` & `sqlmap-1.7.7/sqlmap/extra/runcmd/src/runcmd/stdafx.h`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/extra/runcmd/src/runcmd/runcmd.vcproj` & `sqlmap-1.7.7/sqlmap/extra/runcmd/src/runcmd/runcmd.vcproj`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/extra/runcmd/runcmd.exe_` & `sqlmap-1.7.7/sqlmap/extra/runcmd/runcmd.exe_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/extra/beep/beep.py` & `sqlmap-1.7.7/sqlmap/extra/beep/beep.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/extra/beep/beep.wav` & `sqlmap-1.7.7/sqlmap/extra/beep/beep.wav`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/extra/shellcodeexec/linux/shellcodeexec.x32_` & `sqlmap-1.7.7/sqlmap/extra/shellcodeexec/linux/shellcodeexec.x32_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/extra/shellcodeexec/linux/shellcodeexec.x64_` & `sqlmap-1.7.7/sqlmap/extra/shellcodeexec/linux/shellcodeexec.x64_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/extra/shellcodeexec/windows/shellcodeexec.x32.exe_` & `sqlmap-1.7.7/sqlmap/extra/shellcodeexec/windows/shellcodeexec.x32.exe_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/extra/icmpsh/icmpsh-m.c` & `sqlmap-1.7.7/sqlmap/extra/icmpsh/icmpsh-m.c`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/extra/icmpsh/icmpsh.exe_` & `sqlmap-1.7.7/sqlmap/extra/icmpsh/icmpsh.exe_`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/extra/icmpsh/icmpsh-s.c` & `sqlmap-1.7.7/sqlmap/extra/icmpsh/icmpsh-s.c`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/extra/icmpsh/README.txt` & `sqlmap-1.7.7/sqlmap/extra/icmpsh/README.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/extra/icmpsh/icmpsh-m.pl` & `sqlmap-1.7.7/sqlmap/extra/icmpsh/icmpsh-m.pl`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/extra/icmpsh/__init__.py` & `sqlmap-1.7.7/sqlmap/extra/icmpsh/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/extra/icmpsh/icmpsh_m.py` & `sqlmap-1.7.7/sqlmap/extra/icmpsh/icmpsh_m.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/extra/dbgtool/dbgtool.py` & `sqlmap-1.7.7/sqlmap/extra/dbgtool/dbgtool.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/extra/dbgtool/README.txt` & `sqlmap-1.7.7/sqlmap/extra/dbgtool/README.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/extra/vulnserver/vulnserver.py` & `sqlmap-1.7.7/sqlmap/extra/vulnserver/vulnserver.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap/sqlmapapi.py` & `sqlmap-1.7.7/sqlmap/sqlmapapi.py`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/README.rst` & `sqlmap-1.7.7/README.rst`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap.egg-info/SOURCES.txt` & `sqlmap-1.7.7/sqlmap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlmap-1.7.6/sqlmap.egg-info/PKG-INFO` & `sqlmap-1.7.7/sqlmap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sqlmap
-Version: 1.7.6
+Version: 1.7.7
 Summary: Automatic SQL injection and database takeover tool
 Home-page: https://sqlmap.org
 Author: Bernardo Damele Assumpcao Guimaraes, Miroslav Stampar
 Author-email: bernardo@sqlmap.org, miroslav@sqlmap.org
 License: GNU General Public License v2 (GPLv2)
-Download-URL: https://github.com/sqlmapproject/sqlmap/archive/1.7.6.zip
+Download-URL: https://github.com/sqlmapproject/sqlmap/archive/1.7.7.zip
 Project-URL: Source, https://github.com/sqlmapproject/sqlmap/
 Project-URL: Documentation, https://github.com/sqlmapproject/sqlmap/wiki
 Project-URL: Tracker, https://github.com/sqlmapproject/sqlmap/issues
 Description: sqlmap
         ======
         
         |Python 2.6|2.7|3.x| |License| |Twitter|
```

### Comparing `sqlmap-1.7.6/setup.py` & `sqlmap-1.7.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 See the file 'LICENSE' for copying permission
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name='sqlmap',
-    version='1.7.6',
+    version='1.7.7',
     description='Automatic SQL injection and database takeover tool',
     long_description=open('README.rst').read(),
     long_description_content_type='text/x-rst',
     author='Bernardo Damele Assumpcao Guimaraes, Miroslav Stampar',
     author_email='bernardo@sqlmap.org, miroslav@sqlmap.org',
     url='https://sqlmap.org',
     project_urls={
         'Documentation': 'https://github.com/sqlmapproject/sqlmap/wiki',
         'Source': 'https://github.com/sqlmapproject/sqlmap/',
         'Tracker': 'https://github.com/sqlmapproject/sqlmap/issues',
     },
-    download_url='https://github.com/sqlmapproject/sqlmap/archive/1.7.6.zip',
+    download_url='https://github.com/sqlmapproject/sqlmap/archive/1.7.7.zip',
     license='GNU General Public License v2 (GPLv2)',
     packages=find_packages(),
     include_package_data=True,
     zip_safe=False,
     # https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         'Development Status :: 5 - Production/Stable',
```

