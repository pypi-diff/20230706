# Comparing `tmp/git-plus-v0.4.6.tar.gz` & `tmp/git-plus-v0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/git-plus-v0.4.6.tar", last modified: Mon Jul 27 15:21:55 2020, max compression
+gzip compressed data, was "git-plus-v0.4.7.tar", last modified: Sun Jul 25 12:43:57 2021, max compression
```

## Comparing `git-plus-v0.4.6.tar` & `git-plus-v0.4.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tkr        (501) staff       (20)        0 2020-07-27 15:21:55.000000 git-plus-v0.4.6/
--rw-r--r--   0 tkr        (501) staff       (20)      352 2020-07-27 15:21:55.000000 git-plus-v0.4.6/PKG-INFO
--rwxr-xr-x   0 tkr        (501) staff       (20)      624 2020-07-12 15:50:40.000000 git-plus-v0.4.6/git-multi
--rwxr-xr-x   0 tkr        (501) staff       (20)      631 2020-07-12 15:50:40.000000 git-plus-v0.4.6/git-old-branches
--rwxr-xr-x   0 tkr        (501) staff       (20)      625 2020-07-12 15:50:40.000000 git-plus-v0.4.6/git-recent
--rwxr-xr-x   0 tkr        (501) staff       (20)      627 2020-07-12 15:50:40.000000 git-plus-v0.4.6/git-relation
--rwxr-xr-x   0 tkr        (501) staff       (20)      625 2020-07-12 15:50:40.000000 git-plus-v0.4.6/git-semver
-drwxr-xr-x   0 tkr        (501) staff       (20)        0 2020-07-27 15:21:55.000000 git-plus-v0.4.6/gitplus/
--rw-r--r--   0 tkr        (501) staff       (20)       23 2020-07-12 15:50:40.000000 git-plus-v0.4.6/gitplus/__init__.py
--rwxr-xr-x   0 tkr        (501) staff       (20)     6538 2020-07-12 15:50:40.000000 git-plus-v0.4.6/gitplus/cmd_git_multi.py
--rwxr-xr-x   0 tkr        (501) staff       (20)     2906 2020-07-12 15:50:40.000000 git-plus-v0.4.6/gitplus/cmd_git_old_branches.py
--rwxr-xr-x   0 tkr        (501) staff       (20)     2553 2020-07-12 15:50:40.000000 git-plus-v0.4.6/gitplus/cmd_git_recent.py
--rwxr-xr-x   0 tkr        (501) staff       (20)     5020 2020-07-27 06:35:23.000000 git-plus-v0.4.6/gitplus/cmd_git_relation.py
--rwxr-xr-x   0 tkr        (501) staff       (20)     2606 2020-07-12 15:50:40.000000 git-plus-v0.4.6/gitplus/cmd_git_semver.py
--rw-r--r--   0 tkr        (501) staff       (20)     3976 2020-07-12 15:50:40.000000 git-plus-v0.4.6/gitplus/git.py
--rw-r--r--   0 tkr        (501) staff       (20)     2073 2020-07-12 15:50:40.000000 git-plus-v0.4.6/gitplus/semver.py
--rw-r--r--   0 tkr        (501) staff       (20)      812 2020-07-12 15:50:40.000000 git-plus-v0.4.6/gitplus/utils.py
--rwxr-xr-x   0 tkr        (501) staff       (20)     1212 2020-07-27 15:21:30.000000 git-plus-v0.4.6/setup.py
+drwxr-xr-x   0 tkr        (501) staff       (20)        0 2021-07-25 12:43:57.903272 git-plus-v0.4.7/
+-rw-r--r--   0 tkr        (501) staff       (20)      352 2021-07-25 12:43:57.903316 git-plus-v0.4.7/PKG-INFO
+-rwxr-xr-x   0 tkr        (501) staff       (20)      624 2020-07-12 15:50:40.000000 git-plus-v0.4.7/git-multi
+-rwxr-xr-x   0 tkr        (501) staff       (20)      631 2020-07-12 15:50:40.000000 git-plus-v0.4.7/git-old-branches
+-rwxr-xr-x   0 tkr        (501) staff       (20)      625 2020-07-12 15:50:40.000000 git-plus-v0.4.7/git-recent
+-rwxr-xr-x   0 tkr        (501) staff       (20)      627 2020-07-12 15:50:40.000000 git-plus-v0.4.7/git-relation
+-rwxr-xr-x   0 tkr        (501) staff       (20)      625 2020-07-12 15:50:40.000000 git-plus-v0.4.7/git-semver
+drwxr-xr-x   0 tkr        (501) staff       (20)        0 2021-07-25 12:43:57.903250 git-plus-v0.4.7/gitplus/
+-rw-r--r--   0 tkr        (501) staff       (20)       23 2020-07-12 15:50:40.000000 git-plus-v0.4.7/gitplus/__init__.py
+-rwxr-xr-x   0 tkr        (501) staff       (20)     6538 2020-11-17 13:41:18.000000 git-plus-v0.4.7/gitplus/cmd_git_multi.py
+-rwxr-xr-x   0 tkr        (501) staff       (20)     3196 2021-07-20 08:21:23.389468 git-plus-v0.4.7/gitplus/cmd_git_old_branches.py
+-rwxr-xr-x   0 tkr        (501) staff       (20)     2897 2021-04-20 18:00:54.909313 git-plus-v0.4.7/gitplus/cmd_git_recent.py
+-rwxr-xr-x   0 tkr        (501) staff       (20)     5231 2021-07-23 15:54:27.557117 git-plus-v0.4.7/gitplus/cmd_git_relation.py
+-rwxr-xr-x   0 tkr        (501) staff       (20)     2606 2020-07-12 15:50:40.000000 git-plus-v0.4.7/gitplus/cmd_git_semver.py
+-rw-r--r--   0 tkr        (501) staff       (20)     4045 2021-07-20 08:14:13.513778 git-plus-v0.4.7/gitplus/git.py
+-rw-r--r--   0 tkr        (501) staff       (20)     2073 2020-07-12 15:50:40.000000 git-plus-v0.4.7/gitplus/semver.py
+-rw-r--r--   0 tkr        (501) staff       (20)      812 2020-11-17 13:41:18.000000 git-plus-v0.4.7/gitplus/utils.py
+-rwxr-xr-x   0 tkr        (501) staff       (20)     1212 2021-07-25 12:43:32.744549 git-plus-v0.4.7/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `git-plus-v0.4.6/git-multi` & `git-plus-v0.4.7/git-multi`

 * *Files identical despite different names*

### Comparing `git-plus-v0.4.6/git-old-branches` & `git-plus-v0.4.7/git-old-branches`

 * *Files identical despite different names*

### Comparing `git-plus-v0.4.6/git-recent` & `git-plus-v0.4.7/git-recent`

 * *Files identical despite different names*

### Comparing `git-plus-v0.4.6/git-relation` & `git-plus-v0.4.7/git-relation`

 * *Files identical despite different names*

### Comparing `git-plus-v0.4.6/git-semver` & `git-plus-v0.4.7/git-semver`

 * *Files identical despite different names*

### Comparing `git-plus-v0.4.6/gitplus/cmd_git_multi.py` & `git-plus-v0.4.7/gitplus/cmd_git_multi.py`

 * *Files identical despite different names*

### Comparing `git-plus-v0.4.6/gitplus/cmd_git_old_branches.py` & `git-plus-v0.4.7/gitplus/cmd_git_old_branches.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 
 remote: bool = args.remote
 all_branches: bool = args.all
 merged: bool = args.merged
 no_merged: bool = args.no_merged
 
 branches = git.get_branches(remote, all_branches, merged=merged, no_merged=no_merged)
+delete_all = False
 for branch in branches:
     if remote and not branch.startswith("remotes/"):
         branch = f"remotes/{branch}"
     command = 'log ' + branch + ' -1 --format=%at --'
     success, result = git.execute_git(command, output=False)
     if not success:
         sys.stderr.write(command)
@@ -66,12 +67,20 @@
         time_diff_days = int((float(time_diff_seconds) / (60*60*24)) * 100) / 100.
 
         #print 'Last commit in %s was %s days ago' % (branch, time_diff_days)
 
         if time_diff_days > args.days:
             print('Branch %s is older than %s days (%s)!' % (branch, args.days, time_diff_days))
             if args.delete:
-                answer = input('Remove [yes/N] ?')
-                if answer.lower() == 'yes':
+                if delete_all:
+                    answer = 'y'
+                else:
+                    answer = input('Remove [y/N/all] ?')
+
+                if answer.lower() == 'all' and input(f"Really delete all filtered branches [y/N]?") == 'y':
+                    delete_all = True
+                    answer = 'y'
+
+                if answer.lower() == 'y':
                     git.delete_branch(branch, force=True)
                 else:
                     print('Not deleted')
```

### Comparing `git-plus-v0.4.6/gitplus/cmd_git_recent.py` & `git-plus-v0.4.7/gitplus/cmd_git_recent.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,50 +15,61 @@
 
 import sys as mod_sys
 import argparse as mod_argparse
 import time as mod_time
 
 from . import git
 
+from typing import *
+
 git.assert_in_git_repository()
 
 parser = mod_argparse.ArgumentParser(
     description='Show list of branches sorted by last commit time')
 
 parser.add_argument('-r', '--remote', action='store_true',
                     default=False, help='Get remote branches')
+parser.add_argument('-b', '--brief', action='store_true',
+                    default=False, help='brief output')
 parser.add_argument('-a', '--all', action='store_true',
                     default=False, help='Get all (local and remote) branches')
-parser.add_argument('--no-merged', action='store_true',
+parser.add_argument('-n', '--no-merged', action='store_true',
                     default=False, help='Only *not* merged branches')
-parser.add_argument('--merged', action='store_true',
+parser.add_argument('-m', '--merged', action='store_true',
                     default=False, help='Only merged branches')
 parser.add_argument('entries', metavar='entries', type=int, default=1000, nargs='?',
                     help='Number of entries (negative number if you want the last N entries)')
 
 args = parser.parse_args()
 
 now = mod_time.time()
 
 times_and_branches = []
 
-branches = git.get_branches(args.remote, merged=args.merged, no_merged=args.no_merged, all=args.all)
+brief: bool = args.brief
+merged: bool = args.merged
+remote: bool = args.remote
+get_all: bool = args.all
+no_merged: bool = args.no_merged
+
+branches = git.get_branches(remote, merged=merged, no_merged=no_merged, all=get_all)
 for branch in branches:
     cmd = 'log ' + branch + ' -1 --format=%at --'
     success, result = git.execute_git(cmd, output=False)
     if not success:
         mod_sys.stderr.write(cmd)
         mod_sys.stderr.write(result)
 
+    time_diff_seconds = int(now) - int(result)
     if (not success) or (len(result.strip()) == 0):
         print('Cannot find the age of %s' % branch)
+    elif brief:
+        times_and_branches.append((time_diff_seconds, branch))
     else:
-        time_diff_seconds = int(now) - int(result)
         time_diff_days = int((float(time_diff_seconds) / (60*60*24)) * 100) / 100.
-
         times_and_branches.append((time_diff_seconds, '%10s days: %s' % (time_diff_days, branch), ))
 
 times_and_branches.sort()
 
 try:
     entries = int(args.entries)
 except:
```

### Comparing `git-plus-v0.4.6/gitplus/cmd_git_relation.py` & `git-plus-v0.4.7/gitplus/cmd_git_relation.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 
 parser.add_argument('branch_1', metavar='branch_1', type=str, default='HEAD', nargs='?',
                    help='the one commit/tag/branch')
 parser.add_argument('branch_2', metavar='branch_2', type=str, nargs='?', default='HEAD',
                    help='the other commit/tag/branch (default HEAD)')
 parser.add_argument('-b', '--brief', action='store_true',
                     default=False, help='brief output')
+parser.add_argument('-m', '--msg', action='store_true',
+                    default=False, help='only commit messages')
 parser.add_argument('-u', '--upstream', action='store_true',
                     default=False, help='relation with upstream branch')
 parser.add_argument('-a', '--all', action='store_true',
                     default=False, help='show all commits')
 parser.add_argument('-sv', '--semver', action='store_true',
                     default=False, help='relation with latest semver tag')
 parser.add_argument('-svn', '--semvern', type=int,
@@ -41,14 +43,15 @@
 
 args = parser.parse_args()
 
 branch_1: str = args.branch_1
 branch_2: str = args.branch_2
 branch_2_latest_semver: bool = args.semver
 branch_2_n_old_semver: int = args.semvern
+only_messages: str = args.msg
 
 if branch_2_latest_semver:
     branch_2_n_old_semver = 1
 if branch_2_n_old_semver:
     versions = semver.get_all_versions_ordered()
     if not versions:
         print('no semver tags found')
@@ -68,17 +71,20 @@
         print('error getting upstream branch')
         sys.exit(1)
     first_line = optput.split("\n")[0]
     branch_2 = first_line
 
 
 def print_log(commit_1: str, commit_2: str, all_commits: bool=False) -> None:
-    success, log = git.execute_git(
-        'log %s..%s --format=%%x20%%x20%%x20%%h%%x20%%Cgreen%%an%%Creset%%x20\"%%Cred%%s%%Creset\",%%x20%%ar' % (commit_1, commit_2),
-        output=False)
+    cmd = 'log %s..%s' % (commit_1, commit_2)
+    if only_messages:
+        cmd += ' --oneline'
+    else:
+        cmd += ' --format=%x20%x20%x20%h%x20%Cgreen%an%Creset%x20\"%Cred%s%Creset\",%x20%ar'
+    success, log = git.execute_git(cmd, output=False)
     if not success:
         print('Error retrieving log %s..%s' % (commit_1, commit_2))
         sys.exit(1)
     result = log.rstrip()
 
     lines = result.split('\n')
```

### Comparing `git-plus-v0.4.6/gitplus/cmd_git_semver.py` & `git-plus-v0.4.7/gitplus/cmd_git_semver.py`

 * *Files identical despite different names*

### Comparing `git-plus-v0.4.6/gitplus/git.py` & `git-plus-v0.4.7/gitplus/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,16 @@
     def _filter_branch(branch: str) -> str:
         if '*' in branch:
             # Current branch:
             return branch.replace('*', '').strip()
         elif '->' in branch:
             # Branch is an alias
             return branch.split('->')[0].strip()
+        elif 'HEAD detached at' in branch:
+            return 'HEAD'
         return branch.strip()
 
     lines = result.strip().split('\n')
     lines = list(map(_filter_branch, lines))
     lines = [line for line in lines if line]
     return lines
```

### Comparing `git-plus-v0.4.6/gitplus/semver.py` & `git-plus-v0.4.7/gitplus/semver.py`

 * *Files identical despite different names*

### Comparing `git-plus-v0.4.6/gitplus/utils.py` & `git-plus-v0.4.7/gitplus/utils.py`

 * *Files identical despite different names*

### Comparing `git-plus-v0.4.6/setup.py` & `git-plus-v0.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import distutils.core as mod_distutilscore
 
 mod_distutilscore.setup(
     name='git-plus',
-    version='v0.4.6',
+    version='v0.4.7',
     description='Set of git utilities',
     license='Apache License, Version 2.0',
     author='Tomo Krajina',
     author_email='tkrajina@gmail.com',
     url='https://github.com/tkrajina/git-plus',
     packages=['gitplus', ],
     classifiers=[
```

