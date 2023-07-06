# Comparing `tmp/cookiecutter-2.1.1.tar.gz` & `tmp/cookiecutter-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cookiecutter-2.1.1.tar", last modified: Wed Jun  1 17:01:02 2022, max compression
+gzip compressed data, was "cookiecutter-2.2.0.tar", last modified: Thu Jul  6 16:27:19 2023, max compression
```

## Comparing `cookiecutter-2.1.1.tar` & `cookiecutter-2.2.0.tar`

### file list

```diff
@@ -1,288 +1,341 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.279470 cookiecutter-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11784 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (121)      326 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)    12892 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)    67831 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (121)     1493 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    12339 2022-06-01 17:01:02.279470 cookiecutter-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11013 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.251470 cookiecutter-2.1.1/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/cookiecutter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/cookiecutter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6926 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/cookiecutter/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     4250 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/cookiecutter/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2259 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/cookiecutter/environment.py
--rw-r--r--   0 runner    (1001) docker     (121)     3886 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/cookiecutter/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1861 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/cookiecutter/extensions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1008 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/cookiecutter/find.py
--rw-r--r--   0 runner    (1001) docker     (121)    14827 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/cookiecutter/generate.py
--rw-r--r--   0 runner    (1001) docker     (121)     4227 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/cookiecutter/hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1568 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/cookiecutter/log.py
--rw-r--r--   0 runner    (1001) docker     (121)     4657 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/cookiecutter/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     8197 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/cookiecutter/prompt.py
--rw-r--r--   0 runner    (1001) docker     (121)     1512 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/cookiecutter/replay.py
--rw-r--r--   0 runner    (1001) docker     (121)     4206 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/cookiecutter/repository.py
--rw-r--r--   0 runner    (1001) docker     (121)     3136 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/cookiecutter/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4184 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/cookiecutter/vcs.py
--rw-r--r--   0 runner    (1001) docker     (121)     4264 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/cookiecutter/zipfile.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.251470 cookiecutter-2.1.1/cookiecutter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12339 2022-06-01 17:01:01.000000 cookiecutter-2.1.1/cookiecutter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9377 2022-06-01 17:01:02.000000 cookiecutter-2.1.1/cookiecutter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-01 17:01:01.000000 cookiecutter-2.1.1/cookiecutter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-06-01 17:01:01.000000 cookiecutter-2.1.1/cookiecutter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-01 17:00:59.000000 cookiecutter-2.1.1/cookiecutter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-06-01 17:01:02.000000 cookiecutter-2.1.1/cookiecutter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-06-01 17:01:02.000000 cookiecutter-2.1.1/cookiecutter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-06-01 17:01:02.279470 cookiecutter-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2175 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.259470 cookiecutter-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7672 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.259470 cookiecutter-2.1.1/tests/fake-repo/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/fake-repo/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.259470 cookiecutter-2.1.1/tests/fake-repo/fake-project/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/fake-repo/fake-project/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.259470 cookiecutter-2.1.1/tests/fake-repo-bad/
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/fake-repo-bad/no-project-in-here.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.259470 cookiecutter-2.1.1/tests/fake-repo-bad-json/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/fake-repo-bad-json/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.259470 cookiecutter-2.1.1/tests/fake-repo-bad-json/{{cookiecutter.repo_name}}/
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/fake-repo-bad-json/{{cookiecutter.repo_name}}/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.259470 cookiecutter-2.1.1/tests/fake-repo-dict/
--rw-r--r--   0 runner    (1001) docker     (121)      413 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/fake-repo-dict/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.259470 cookiecutter-2.1.1/tests/fake-repo-dict/{{cookiecutter.project_slug}}/
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/fake-repo-dict/{{cookiecutter.project_slug}}/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.239470 cookiecutter-2.1.1/tests/fake-repo-dir/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.259470 cookiecutter-2.1.1/tests/fake-repo-dir/my-dir/
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/fake-repo-dir/my-dir/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.259470 cookiecutter-2.1.1/tests/fake-repo-dir/my-dir/{{cookiecutter.repo_name}}/
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/fake-repo-dir/my-dir/{{cookiecutter.repo_name}}/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.259470 cookiecutter-2.1.1/tests/fake-repo-pre/
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/fake-repo-pre/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.259470 cookiecutter-2.1.1/tests/fake-repo-pre/{{cookiecutter.repo_name}}/
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/fake-repo-pre/{{cookiecutter.repo_name}}/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.259470 cookiecutter-2.1.1/tests/fake-repo-pre2/
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/fake-repo-pre2/cookiecutter.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/fake-repo-pre2/whatever.some.thing
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.259470 cookiecutter-2.1.1/tests/fake-repo-pre2/{{cookiecutter.repo_name}}/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/fake-repo-pre2/{{cookiecutter.repo_name}}/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.259470 cookiecutter-2.1.1/tests/fake-repo-tmpl/
--rw-r--r--   0 runner    (1001) docker     (121)      333 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/fake-repo-tmpl/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.259470 cookiecutter-2.1.1/tests/fake-repo-tmpl/{{cookiecutter.repo_name}}/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/fake-repo-tmpl/{{cookiecutter.repo_name}}/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.263470 cookiecutter-2.1.1/tests/files/
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/files/bad-zip-file.zip
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/files/empty.zip
--rw-r--r--   0 runner    (1001) docker     (121)      994 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/files/fake-repo-tmpl.zip
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/files/not-a-repo.zip
--rw-r--r--   0 runner    (1001) docker     (121)     1114 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/files/protected-fake-repo-tmpl.zip
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/files/syntax_error.txt
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/files/unicode.txt
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/files/{% if cookiecutter.generate_file == 'y' %}cheese.txt{% endif %}
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/files/{{cookiecutter.generate_file}}.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/files/{{cookiecutter.generate_file}}_crlf_newlines.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/files/{{cookiecutter.generate_file}}_lf_newlines.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/files/{{cookiecutter.jsonify_file}}.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/files/{{cookiecutter.random_string_file}}.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.239470 cookiecutter-2.1.1/tests/hooks-abort-render/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.263470 cookiecutter-2.1.1/tests/hooks-abort-render/hooks/
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/hooks-abort-render/hooks/post_gen_project.py
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/hooks-abort-render/hooks/pre_gen_project.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.263470 cookiecutter-2.1.1/tests/hooks-abort-render/{{cookiecutter.repo_dir}}/
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/hooks-abort-render/{{cookiecutter.repo_dir}}/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.263470 cookiecutter-2.1.1/tests/replay/
--rw-r--r--   0 runner    (1001) docker     (121)      670 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/replay/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     3342 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/replay/test_dump.py
--rw-r--r--   0 runner    (1001) docker     (121)     1881 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/replay/test_load.py
--rw-r--r--   0 runner    (1001) docker     (121)     2304 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/replay/test_replay.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.263470 cookiecutter-2.1.1/tests/repository/
--rw-r--r--   0 runner    (1001) docker     (121)     1837 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/repository/test_abbreviation_expansion.py
--rw-r--r--   0 runner    (1001) docker     (121)     3221 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/repository/test_determine_repo_dir_clones_repo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1264 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/repository/test_determine_repo_dir_finds_existing_cookiecutter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2359 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/repository/test_determine_repo_dir_finds_subdirectories.py
--rw-r--r--   0 runner    (1001) docker     (121)     2032 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/repository/test_determine_repository_should_use_local_repo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2212 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/repository/test_is_repo_url.py
--rw-r--r--   0 runner    (1001) docker     (121)      606 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/repository/test_repository_has_cookiecutter_json.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.267470 cookiecutter-2.1.1/tests/test-config/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-config/config-expand-user.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-config/config-expand-vars.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-config/invalid-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      440 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-config/valid-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-config/valid-partial-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.243470 cookiecutter-2.1.1/tests/test-extensions/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.267470 cookiecutter-2.1.1/tests/test-extensions/custom-extension-post/
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-extensions/custom-extension-post/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.267470 cookiecutter-2.1.1/tests/test-extensions/custom-extension-post/hooks/
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-extensions/custom-extension-post/hooks/post_gen_project.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.267470 cookiecutter-2.1.1/tests/test-extensions/custom-extension-post/{{cookiecutter.project_slug}}/
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-extensions/custom-extension-post/{{cookiecutter.project_slug}}/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.267470 cookiecutter-2.1.1/tests/test-extensions/custom-extension-pre/
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-extensions/custom-extension-pre/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.267470 cookiecutter-2.1.1/tests/test-extensions/custom-extension-pre/hooks/
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-extensions/custom-extension-pre/hooks/pre_gen_project.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.267470 cookiecutter-2.1.1/tests/test-extensions/custom-extension-pre/{{cookiecutter.project_slug}}/
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-extensions/custom-extension-pre/{{cookiecutter.project_slug}}/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.267470 cookiecutter-2.1.1/tests/test-extensions/default/
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-extensions/default/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.267470 cookiecutter-2.1.1/tests/test-extensions/default/{{cookiecutter.project_slug}}/
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-extensions/default/{{cookiecutter.project_slug}}/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-extensions/default/{{cookiecutter.project_slug}}/id
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.267470 cookiecutter-2.1.1/tests/test-extensions/hello_extension/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-extensions/hello_extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      786 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-extensions/hello_extension/hello_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.267470 cookiecutter-2.1.1/tests/test-extensions/local_extension/
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-extensions/local_extension/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.267470 cookiecutter-2.1.1/tests/test-extensions/local_extension/local_extensions/
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-extensions/local_extension/local_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      548 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-extensions/local_extension/local_extensions/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.267470 cookiecutter-2.1.1/tests/test-extensions/local_extension/{{cookiecutter.project_slug}}/
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-extensions/local_extension/{{cookiecutter.project_slug}}/HISTORY.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.267470 cookiecutter-2.1.1/tests/test-extensions/unknown/
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-extensions/unknown/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.267470 cookiecutter-2.1.1/tests/test-extensions/unknown/{{cookiecutter.project_slug}}/
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-extensions/unknown/{{cookiecutter.project_slug}}/HISTORY.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.243470 cookiecutter-2.1.1/tests/test-generate-binaries/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.271470 cookiecutter-2.1.1/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/
--rw-r--r--   0 runner    (1001) docker     (121)    15364 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (121)     4381 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/logo.png
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/readme.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)    18116 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/some_font.otf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.271470 cookiecutter-2.1.1/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/
--rw-r--r--   0 runner    (1001) docker     (121)    12292 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (121)     4381 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/logo.png
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/readme.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)    18116 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/some_font.otf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.271470 cookiecutter-2.1.1/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/
--rw-r--r--   0 runner    (1001) docker     (121)     4381 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.271470 cookiecutter-2.1.1/tests/test-generate-context/
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-generate-context/choices_template.json
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-generate-context/invalid-syntax.json
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-generate-context/non_ascii.json
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-generate-context/test.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.243470 cookiecutter-2.1.1/tests/test-generate-copy-without-render/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.271470 cookiecutter-2.1.1/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.271470 cookiecutter-2.1.1/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/rendered/
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/rendered/not_rendered.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.271470 cookiecutter-2.1.1/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-not-rendered/
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-not-rendered/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.271470 cookiecutter-2.1.1/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.243470 cookiecutter-2.1.1/tests/test-generate-files/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.275470 cookiecutter-2.1.1/tests/test-generate-files/input{{cookiecutter.food}}/
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-generate-files/input{{cookiecutter.food}}/simple-with-conditions.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-generate-files/input{{cookiecutter.food}}/simple-with-newline-crlf.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-generate-files/input{{cookiecutter.food}}/simple-with-newline.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-generate-files/input{{cookiecutter.food}}/simple.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.271470 cookiecutter-2.1.1/tests/test-generate-files-line-end/
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-generate-files-line-end/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.271470 cookiecutter-2.1.1/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.271470 cookiecutter-2.1.1/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/folder/
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/folder/in_folder.txt
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/something.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.271470 cookiecutter-2.1.1/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/{{cookiecutter.folder_name}}/
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/{{cookiecutter.folder_name}}/{{cookiecutter.filename}}.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.243470 cookiecutter-2.1.1/tests/test-generate-files-nontemplated/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.271470 cookiecutter-2.1.1/tests/test-generate-files-nontemplated/input/
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-generate-files-nontemplated/input/simple.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.243470 cookiecutter-2.1.1/tests/test-generate-files-permissions/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.275470 cookiecutter-2.1.1/tests/test-generate-files-permissions/input{{cookiecutter.permissions}}/
--rwxr-xr-x   0 runner    (1001) docker     (121)       32 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-generate-files-permissions/input{{cookiecutter.permissions}}/script.sh
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-generate-files-permissions/input{{cookiecutter.permissions}}/simple.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.275470 cookiecutter-2.1.1/tests/test-output-folder/
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-output-folder/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.275470 cookiecutter-2.1.1/tests/test-output-folder/{{cookiecutter.test_name}}/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.275470 cookiecutter-2.1.1/tests/test-output-folder/{{cookiecutter.test_name}}/folder/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-output-folder/{{cookiecutter.test_name}}/folder/in_folder.txt
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-output-folder/{{cookiecutter.test_name}}/something.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.275470 cookiecutter-2.1.1/tests/test-output-folder/{{cookiecutter.test_name}}/{{cookiecutter.folder_name}}/
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-output-folder/{{cookiecutter.test_name}}/{{cookiecutter.folder_name}}/{{cookiecutter.filename}}.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.243470 cookiecutter-2.1.1/tests/test-pyhooks/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.275470 cookiecutter-2.1.1/tests/test-pyhooks/hooks/
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-pyhooks/hooks/post_gen_project.py
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-pyhooks/hooks/pre_gen_project.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.275470 cookiecutter-2.1.1/tests/test-pyhooks/input{{cookiecutter.pyhooks}}/
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-pyhooks/input{{cookiecutter.pyhooks}}/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.243470 cookiecutter-2.1.1/tests/test-pyshellhooks/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.275470 cookiecutter-2.1.1/tests/test-pyshellhooks/hooks/
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-pyshellhooks/hooks/post_gen_project.py
--rwxr-xr-x   0 runner    (1001) docker     (121)       65 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-pyshellhooks/hooks/post_gen_project.sh
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-pyshellhooks/hooks/pre_gen_project.py
--rwxr-xr-x   0 runner    (1001) docker     (121)       64 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-pyshellhooks/hooks/pre_gen_project.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.275470 cookiecutter-2.1.1/tests/test-pyshellhooks/input{{pyshellhooks}}/
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-pyshellhooks/input{{pyshellhooks}}/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.275470 cookiecutter-2.1.1/tests/test-replay/
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-replay/cookiedozer_load.json
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-replay/invalid_replay.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.247470 cookiecutter-2.1.1/tests/test-shellhooks/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.279470 cookiecutter-2.1.1/tests/test-shellhooks/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (121)       65 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-shellhooks/hooks/post_gen_project.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)       63 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-shellhooks/hooks/pre_gen_project.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.279470 cookiecutter-2.1.1/tests/test-shellhooks/input{{cookiecutter.shellhooks}}/
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-shellhooks/input{{cookiecutter.shellhooks}}/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.247470 cookiecutter-2.1.1/tests/test-shellhooks-empty/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.275470 cookiecutter-2.1.1/tests/test-shellhooks-empty/hooks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-shellhooks-empty/hooks/pre_gen_project.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.275470 cookiecutter-2.1.1/tests/test-shellhooks-empty/input{{cookiecutter.shellhooks}}/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-shellhooks-empty/input{{cookiecutter.shellhooks}}/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.247470 cookiecutter-2.1.1/tests/test-shellhooks-win/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.275470 cookiecutter-2.1.1/tests/test-shellhooks-win/hooks/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-shellhooks-win/hooks/post_gen_project.bat
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-shellhooks-win/hooks/pre_gen_project.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.279470 cookiecutter-2.1.1/tests/test-shellhooks-win/input{{cookiecutter.shellhooks}}/
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test-shellhooks-win/input{{cookiecutter.shellhooks}}/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1203 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test_abort_generate_on_hook_error.py
--rw-r--r--   0 runner    (1001) docker     (121)    20100 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      897 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test_cookiecutter_invocation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4602 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test_cookiecutter_local_no_input.py
--rw-r--r--   0 runner    (1001) docker     (121)     1645 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test_cookiecutter_local_with_input.py
--rw-r--r--   0 runner    (1001) docker     (121)     1325 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test_custom_extensions_in_hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1830 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test_default_extensions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (121)      712 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test_find.py
--rw-r--r--   0 runner    (1001) docker     (121)     7014 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test_generate_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     2446 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test_generate_copy_without_render.py
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test_generate_file.py
--rw-r--r--   0 runner    (1001) docker     (121)    15571 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test_generate_files.py
--rw-r--r--   0 runner    (1001) docker     (121)     8106 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test_generate_hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)     4396 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test_get_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     5403 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test_get_user_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    10528 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test_hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)     3957 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (121)     2366 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (121)     1880 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test_output_folder.py
--rw-r--r--   0 runner    (1001) docker     (121)      847 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test_preferred_encoding.py
--rw-r--r--   0 runner    (1001) docker     (121)    15368 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test_read_repo_password.py
--rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test_read_user_choice.py
--rw-r--r--   0 runner    (1001) docker     (121)     3628 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test_read_user_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test_read_user_variable.py
--rw-r--r--   0 runner    (1001) docker     (121)      524 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test_read_user_yes_no.py
--rw-r--r--   0 runner    (1001) docker     (121)      367 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test_repo_not_found.py
--rw-r--r--   0 runner    (1001) docker     (121)     2245 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test_specify_output_dir.py
--rw-r--r--   0 runner    (1001) docker     (121)     6883 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.247470 cookiecutter-2.1.1/tests/undefined-variable/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.247470 cookiecutter-2.1.1/tests/undefined-variable/dir-name/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.279470 cookiecutter-2.1.1/tests/undefined-variable/dir-name/{{cookiecutter.project_slug}}/
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/undefined-variable/dir-name/{{cookiecutter.project_slug}}/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.279470 cookiecutter-2.1.1/tests/undefined-variable/dir-name/{{cookiecutter.project_slug}}/{{cookiecutter.foobar}}/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/undefined-variable/dir-name/{{cookiecutter.project_slug}}/{{cookiecutter.foobar}}/helloworld.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.247470 cookiecutter-2.1.1/tests/undefined-variable/file-content/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.279470 cookiecutter-2.1.1/tests/undefined-variable/file-content/{{cookiecutter.project_slug}}/
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/undefined-variable/file-content/{{cookiecutter.project_slug}}/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.279470 cookiecutter-2.1.1/tests/undefined-variable/file-name/
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/undefined-variable/file-name/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.279470 cookiecutter-2.1.1/tests/undefined-variable/file-name/{{cookiecutter.project_slug}}/
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/undefined-variable/file-name/{{cookiecutter.project_slug}}/{{cookiecutter.foobar}}
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.279470 cookiecutter-2.1.1/tests/vcs/
--rw-r--r--   0 runner    (1001) docker     (121)     7164 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/vcs/test_clone.py
--rw-r--r--   0 runner    (1001) docker     (121)     2549 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/vcs/test_identify_repo.py
--rw-r--r--   0 runner    (1001) docker     (121)      500 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/vcs/test_is_vcs_installed.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 17:01:02.279470 cookiecutter-2.1.1/tests/zipfile/
--rw-r--r--   0 runner    (1001) docker     (121)     9576 2022-06-01 17:00:44.000000 cookiecutter-2.1.1/tests/zipfile/test_unzip.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.105624 cookiecutter-2.2.0/
+-rw-r--r--   0 ericof     (501) staff       (20)    11796 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/AUTHORS.md
+-rw-r--r--   0 ericof     (501) staff       (20)      326 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 ericof     (501) staff       (20)    12666 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/CONTRIBUTING.md
+-rw-r--r--   0 ericof     (501) staff       (20)    72699 2023-07-06 16:16:26.000000 cookiecutter-2.2.0/HISTORY.md
+-rw-r--r--   0 ericof     (501) staff       (20)     1493 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/LICENSE
+-rw-r--r--   0 ericof     (501) staff       (20)      376 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/MANIFEST.in
+-rw-r--r--   0 ericof     (501) staff       (20)    12922 2023-07-06 16:27:19.105738 cookiecutter-2.2.0/PKG-INFO
+-rw-r--r--   0 ericof     (501) staff       (20)    11356 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/README.md
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.019796 cookiecutter-2.2.0/cookiecutter/
+-rw-r--r--   0 ericof     (501) staff       (20)       64 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/cookiecutter/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      194 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/cookiecutter/__main__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     7319 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/cookiecutter/cli.py
+-rw-r--r--   0 ericof     (501) staff       (20)     4250 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/cookiecutter/config.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2280 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/cookiecutter/environment.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3886 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/cookiecutter/exceptions.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3957 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/cookiecutter/extensions.py
+-rw-r--r--   0 ericof     (501) staff       (20)      909 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/cookiecutter/find.py
+-rw-r--r--   0 ericof     (501) staff       (20)    15885 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/cookiecutter/generate.py
+-rw-r--r--   0 ericof     (501) staff       (20)     4230 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/cookiecutter/hooks.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1568 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/cookiecutter/log.py
+-rw-r--r--   0 ericof     (501) staff       (20)     6092 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/cookiecutter/main.py
+-rw-r--r--   0 ericof     (501) staff       (20)     9324 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/cookiecutter/prompt.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1465 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/cookiecutter/replay.py
+-rw-r--r--   0 ericof     (501) staff       (20)     4237 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/cookiecutter/repository.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3173 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/cookiecutter/utils.py
+-rw-r--r--   0 ericof     (501) staff       (20)     4382 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/cookiecutter/vcs.py
+-rw-r--r--   0 ericof     (501) staff       (20)     4451 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/cookiecutter/zipfile.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.024893 cookiecutter-2.2.0/cookiecutter.egg-info/
+-rw-r--r--   0 ericof     (501) staff       (20)    12922 2023-07-06 16:27:18.000000 cookiecutter-2.2.0/cookiecutter.egg-info/PKG-INFO
+-rw-r--r--   0 ericof     (501) staff       (20)    11578 2023-07-06 16:27:18.000000 cookiecutter-2.2.0/cookiecutter.egg-info/SOURCES.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        1 2023-07-06 16:27:18.000000 cookiecutter-2.2.0/cookiecutter.egg-info/dependency_links.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       60 2023-07-06 16:27:18.000000 cookiecutter-2.2.0/cookiecutter.egg-info/entry_points.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        1 2023-06-13 08:11:02.000000 cookiecutter-2.2.0/cookiecutter.egg-info/not-zip-safe
+-rw-r--r--   0 ericof     (501) staff       (20)      115 2023-07-06 16:27:18.000000 cookiecutter-2.2.0/cookiecutter.egg-info/requires.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       13 2023-07-06 16:27:18.000000 cookiecutter-2.2.0/cookiecutter.egg-info/top_level.txt
+-rw-r--r--   0 ericof     (501) staff       (20)      161 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/pyproject.toml
+-rw-r--r--   0 ericof     (501) staff       (20)      225 2023-07-06 16:27:19.106110 cookiecutter-2.2.0/setup.cfg
+-rw-r--r--   0 ericof     (501) staff       (20)     2405 2023-07-06 16:27:10.000000 cookiecutter-2.2.0/setup.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.053549 cookiecutter-2.2.0/tests/
+-rw-r--r--   0 ericof     (501) staff       (20)       38 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     7329 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/conftest.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.053959 cookiecutter-2.2.0/tests/fake-nested-templates/
+-rw-r--r--   0 ericof     (501) staff       (20)       58 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/fake-nested-templates/cookiecutter.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.054426 cookiecutter-2.2.0/tests/fake-nested-templates/fake-project/
+-rw-r--r--   0 ericof     (501) staff       (20)        3 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/fake-nested-templates/fake-project/cookiecutter.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.054884 cookiecutter-2.2.0/tests/fake-repo/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/fake-repo/cookiecutter.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.065236 cookiecutter-2.2.0/tests/fake-repo/fake-project/
+-rw-r--r--   0 ericof     (501) staff       (20)       49 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/fake-repo/fake-project/README.rst
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.055105 cookiecutter-2.2.0/tests/fake-repo-bad/
+-rw-r--r--   0 ericof     (501) staff       (20)       10 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/fake-repo-bad/no-project-in-here.txt
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.055691 cookiecutter-2.2.0/tests/fake-repo-bad-json/
+-rw-r--r--   0 ericof     (501) staff       (20)       33 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/fake-repo-bad-json/cookiecutter.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.056021 cookiecutter-2.2.0/tests/fake-repo-bad-json/{{cookiecutter.repo_name}}/
+-rw-r--r--   0 ericof     (501) staff       (20)      100 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/fake-repo-bad-json/{{cookiecutter.repo_name}}/README.rst
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.056570 cookiecutter-2.2.0/tests/fake-repo-dict/
+-rw-r--r--   0 ericof     (501) staff       (20)      319 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/fake-repo-dict/cookiecutter.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.056849 cookiecutter-2.2.0/tests/fake-repo-dict/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 ericof     (501) staff       (20)      353 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/fake-repo-dict/{{cookiecutter.project_slug}}/README.md
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.002222 cookiecutter-2.2.0/tests/fake-repo-dir/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.057776 cookiecutter-2.2.0/tests/fake-repo-dir/my-dir/
+-rw-r--r--   0 ericof     (501) staff       (20)      289 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/fake-repo-dir/my-dir/cookiecutter.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.058219 cookiecutter-2.2.0/tests/fake-repo-dir/my-dir/{{cookiecutter.repo_name}}/
+-rw-r--r--   0 ericof     (501) staff       (20)      100 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/fake-repo-dir/my-dir/{{cookiecutter.repo_name}}/README.rst
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.058389 cookiecutter-2.2.0/tests/fake-repo-pre/
+-rw-r--r--   0 ericof     (501) staff       (20)      289 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/fake-repo-pre/cookiecutter.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.062090 cookiecutter-2.2.0/tests/fake-repo-pre/{{cookiecutter.repo_name}}/
+-rw-r--r--   0 ericof     (501) staff       (20)      100 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/fake-repo-pre/{{cookiecutter.repo_name}}/README.rst
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.062531 cookiecutter-2.2.0/tests/fake-repo-pre2/
+-rw-r--r--   0 ericof     (501) staff       (20)      289 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/fake-repo-pre2/cookiecutter.json
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/fake-repo-pre2/whatever.some.thing
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.062644 cookiecutter-2.2.0/tests/fake-repo-pre2/{{cookiecutter.repo_name}}/
+-rw-r--r--   0 ericof     (501) staff       (20)       49 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/fake-repo-pre2/{{cookiecutter.repo_name}}/README.rst
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.062806 cookiecutter-2.2.0/tests/fake-repo-tmpl/
+-rw-r--r--   0 ericof     (501) staff       (20)      342 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/fake-repo-tmpl/cookiecutter.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.065049 cookiecutter-2.2.0/tests/fake-repo-tmpl/{{cookiecutter.repo_name}}/
+-rw-r--r--   0 ericof     (501) staff       (20)       49 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/fake-repo-tmpl/{{cookiecutter.repo_name}}/README.rst
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.064579 cookiecutter-2.2.0/tests/fake-repo-tmpl-_cookiecutter/
+-rw-r--r--   0 ericof     (501) staff       (20)      430 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/fake-repo-tmpl-_cookiecutter/cookiecutter.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.064858 cookiecutter-2.2.0/tests/fake-repo-tmpl-_cookiecutter/{{cookiecutter.repo_name}}/
+-rw-r--r--   0 ericof     (501) staff       (20)       49 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/fake-repo-tmpl-_cookiecutter/{{cookiecutter.repo_name}}/README.rst
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.071357 cookiecutter-2.2.0/tests/files/
+-rw-r--r--   0 ericof     (501) staff       (20)       28 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/files/bad-zip-file.zip
+-rw-r--r--   0 ericof     (501) staff       (20)       22 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/files/empty.zip
+-rw-r--r--   0 ericof     (501) staff       (20)      994 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/files/fake-repo-tmpl.zip
+-rw-r--r--   0 ericof     (501) staff       (20)      206 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/files/not-a-repo.zip
+-rw-r--r--   0 ericof     (501) staff       (20)     1114 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/files/protected-fake-repo-tmpl.zip
+-rw-r--r--   0 ericof     (501) staff       (20)       56 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/files/syntax_error.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       89 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/files/unicode.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       64 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/files/{% if cookiecutter.generate_file == 'y' %}cheese.txt{% endif %}
+-rw-r--r--   0 ericof     (501) staff       (20)       41 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/files/{{cookiecutter.generate_file}}.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       51 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/files/{{cookiecutter.generate_file}}_crlf_newlines.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       28 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/files/{{cookiecutter.generate_file}}_lf_newlines.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       29 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/files/{{cookiecutter.jsonify_file}}.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       47 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/files/{{cookiecutter.random_string_file}}.txt
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.003216 cookiecutter-2.2.0/tests/hooks-abort-render/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.072659 cookiecutter-2.2.0/tests/hooks-abort-render/hooks/
+-rw-r--r--   0 ericof     (501) staff       (20)      199 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/hooks-abort-render/hooks/post_gen_project.py
+-rw-r--r--   0 ericof     (501) staff       (20)      197 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/hooks-abort-render/hooks/pre_gen_project.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.072948 cookiecutter-2.2.0/tests/hooks-abort-render/{{cookiecutter.repo_dir}}/
+-rw-r--r--   0 ericof     (501) staff       (20)       52 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/hooks-abort-render/{{cookiecutter.repo_dir}}/README.rst
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.074524 cookiecutter-2.2.0/tests/replay/
+-rw-r--r--   0 ericof     (501) staff       (20)      670 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/replay/conftest.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3357 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/replay/test_dump.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1881 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/replay/test_load.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2304 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/replay/test_replay.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.076827 cookiecutter-2.2.0/tests/repository/
+-rw-r--r--   0 ericof     (501) staff       (20)     1837 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/repository/test_abbreviation_expansion.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3221 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/repository/test_determine_repo_dir_clones_repo.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1294 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/repository/test_determine_repo_dir_finds_existing_cookiecutter.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2389 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/repository/test_determine_repo_dir_finds_subdirectories.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2032 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/repository/test_determine_repository_should_use_local_repo.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2229 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/repository/test_is_repo_url.py
+-rw-r--r--   0 ericof     (501) staff       (20)      606 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/repository/test_repository_has_cookiecutter_json.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.078379 cookiecutter-2.2.0/tests/test-config/
+-rw-r--r--   0 ericof     (501) staff       (20)       62 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-config/config-expand-user.yaml
+-rw-r--r--   0 ericof     (501) staff       (20)       76 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-config/config-expand-vars.yaml
+-rw-r--r--   0 ericof     (501) staff       (20)      162 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-config/invalid-config.yaml
+-rw-r--r--   0 ericof     (501) staff       (20)      440 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-config/valid-config.yaml
+-rw-r--r--   0 ericof     (501) staff       (20)      126 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-config/valid-partial-config.yaml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.004467 cookiecutter-2.2.0/tests/test-extensions/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.078554 cookiecutter-2.2.0/tests/test-extensions/custom-extension-post/
+-rw-r--r--   0 ericof     (501) staff       (20)      111 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-extensions/custom-extension-post/cookiecutter.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.078958 cookiecutter-2.2.0/tests/test-extensions/custom-extension-post/hooks/
+-rw-r--r--   0 ericof     (501) staff       (20)      199 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-extensions/custom-extension-post/hooks/post_gen_project.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.079689 cookiecutter-2.2.0/tests/test-extensions/custom-extension-post/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 ericof     (501) staff       (20)       30 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-extensions/custom-extension-post/{{cookiecutter.project_slug}}/README.rst
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.080129 cookiecutter-2.2.0/tests/test-extensions/custom-extension-pre/
+-rw-r--r--   0 ericof     (501) staff       (20)      111 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-extensions/custom-extension-pre/cookiecutter.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.080442 cookiecutter-2.2.0/tests/test-extensions/custom-extension-pre/hooks/
+-rw-r--r--   0 ericof     (501) staff       (20)      198 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-extensions/custom-extension-pre/hooks/pre_gen_project.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.080729 cookiecutter-2.2.0/tests/test-extensions/custom-extension-pre/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 ericof     (501) staff       (20)       30 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-extensions/custom-extension-pre/{{cookiecutter.project_slug}}/README.rst
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.080974 cookiecutter-2.2.0/tests/test-extensions/default/
+-rw-r--r--   0 ericof     (501) staff       (20)      103 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-extensions/default/cookiecutter.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.081597 cookiecutter-2.2.0/tests/test-extensions/default/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 ericof     (501) staff       (20)       92 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-extensions/default/{{cookiecutter.project_slug}}/HISTORY.rst
+-rw-r--r--   0 ericof     (501) staff       (20)       14 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-extensions/default/{{cookiecutter.project_slug}}/id
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.082259 cookiecutter-2.2.0/tests/test-extensions/hello_extension/
+-rw-r--r--   0 ericof     (501) staff       (20)       23 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-extensions/hello_extension/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      786 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-extensions/hello_extension/hello_extension.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.082536 cookiecutter-2.2.0/tests/test-extensions/local_extension/
+-rw-r--r--   0 ericof     (501) staff       (20)      298 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-extensions/local_extension/cookiecutter.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.083011 cookiecutter-2.2.0/tests/test-extensions/local_extension/local_extensions/
+-rw-r--r--   0 ericof     (501) staff       (20)       65 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-extensions/local_extension/local_extensions/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      548 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-extensions/local_extension/local_extensions/main.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.083214 cookiecutter-2.2.0/tests/test-extensions/local_extension/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 ericof     (501) staff       (20)      139 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-extensions/local_extension/{{cookiecutter.project_slug}}/HISTORY.rst
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.083429 cookiecutter-2.2.0/tests/test-extensions/unknown/
+-rw-r--r--   0 ericof     (501) staff       (20)      121 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-extensions/unknown/cookiecutter.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.083826 cookiecutter-2.2.0/tests/test-extensions/unknown/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 ericof     (501) staff       (20)      119 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-extensions/unknown/{{cookiecutter.project_slug}}/HISTORY.rst
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.004748 cookiecutter-2.2.0/tests/test-generate-binaries/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.084702 cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/
+-rw-r--r--   0 ericof     (501) staff       (20)    15364 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/.DS_Store
+-rw-r--r--   0 ericof     (501) staff       (20)     4381 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/logo.png
+-rw-r--r--   0 ericof     (501) staff       (20)       37 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/readme.txt
+-rwxr-xr-x   0 ericof     (501) staff       (20)    18116 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/some_font.otf
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.085815 cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/
+-rw-r--r--   0 ericof     (501) staff       (20)    12292 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/.DS_Store
+-rw-r--r--   0 ericof     (501) staff       (20)     4381 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/logo.png
+-rw-r--r--   0 ericof     (501) staff       (20)       37 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/readme.txt
+-rwxr-xr-x   0 ericof     (501) staff       (20)    18116 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/some_font.otf
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.086068 cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/
+-rw-r--r--   0 ericof     (501) staff       (20)     4381 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/logo.png
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.087093 cookiecutter-2.2.0/tests/test-generate-context/
+-rw-r--r--   0 ericof     (501) staff       (20)      227 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-generate-context/choices_template.json
+-rw-r--r--   0 ericof     (501) staff       (20)       33 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-context/invalid-syntax.json
+-rw-r--r--   0 ericof     (501) staff       (20)      287 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-generate-context/nested_dict.json
+-rw-r--r--   0 ericof     (501) staff       (20)       28 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-generate-context/non_ascii.json
+-rw-r--r--   0 ericof     (501) staff       (20)       39 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-generate-context/test.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.005914 cookiecutter-2.2.0/tests/test-generate-copy-without-render/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.089847 cookiecutter-2.2.0/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/
+-rw-r--r--   0 ericof     (501) staff       (20)       69 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/README.rst
+-rw-r--r--   0 ericof     (501) staff       (20)       69 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/README.txt
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.090030 cookiecutter-2.2.0/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/rendered/
+-rw-r--r--   0 ericof     (501) staff       (20)       41 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/rendered/not_rendered.yml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.090637 cookiecutter-2.2.0/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-not-rendered/
+-rw-r--r--   0 ericof     (501) staff       (20)       69 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-not-rendered/README.rst
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.091634 cookiecutter-2.2.0/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/
+-rw-r--r--   0 ericof     (501) staff       (20)       45 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.md
+-rw-r--r--   0 ericof     (501) staff       (20)       69 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.rst
+-rw-r--r--   0 ericof     (501) staff       (20)       69 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.txt
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.005406 cookiecutter-2.2.0/tests/test-generate-copy-without-render-override/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.087567 cookiecutter-2.2.0/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/
+-rw-r--r--   0 ericof     (501) staff       (20)       69 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/README.rst
+-rw-r--r--   0 ericof     (501) staff       (20)       69 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/README.txt
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.088279 cookiecutter-2.2.0/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/rendered/
+-rw-r--r--   0 ericof     (501) staff       (20)       41 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/rendered/not_rendered.yml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.088587 cookiecutter-2.2.0/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-not-rendered/
+-rw-r--r--   0 ericof     (501) staff       (20)       69 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-not-rendered/README.rst
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.089271 cookiecutter-2.2.0/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/
+-rw-r--r--   0 ericof     (501) staff       (20)       45 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.md
+-rw-r--r--   0 ericof     (501) staff       (20)       69 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.rst
+-rw-r--r--   0 ericof     (501) staff       (20)       69 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.txt
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.007456 cookiecutter-2.2.0/tests/test-generate-files/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.094006 cookiecutter-2.2.0/tests/test-generate-files/input{{cookiecutter.food}}/
+-rw-r--r--   0 ericof     (501) staff       (20)      111 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-files/input{{cookiecutter.food}}/simple-with-conditions.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       51 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-files/input{{cookiecutter.food}}/simple-with-newline-crlf.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       28 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-files/input{{cookiecutter.food}}/simple-with-newline.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       30 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-generate-files/input{{cookiecutter.food}}/simple.txt
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.091992 cookiecutter-2.2.0/tests/test-generate-files-line-end/
+-rw-r--r--   0 ericof     (501) staff       (20)      183 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-generate-files-line-end/cookiecutter.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.092290 cookiecutter-2.2.0/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.092484 cookiecutter-2.2.0/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/folder/
+-rw-r--r--   0 ericof     (501) staff       (20)       83 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/folder/in_folder.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       76 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/something.txt
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.092693 cookiecutter-2.2.0/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/{{cookiecutter.folder_name}}/
+-rw-r--r--   0 ericof     (501) staff       (20)      125 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/{{cookiecutter.folder_name}}/{{cookiecutter.filename}}.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.007148 cookiecutter-2.2.0/tests/test-generate-files-nontemplated/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.092891 cookiecutter-2.2.0/tests/test-generate-files-nontemplated/input/
+-rw-r--r--   0 ericof     (501) staff       (20)       17 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-generate-files-nontemplated/input/simple.txt
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.007291 cookiecutter-2.2.0/tests/test-generate-files-permissions/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.093284 cookiecutter-2.2.0/tests/test-generate-files-permissions/input{{cookiecutter.permissions}}/
+-rwxr-xr-x   0 ericof     (501) staff       (20)       32 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-generate-files-permissions/input{{cookiecutter.permissions}}/script.sh
+-rw-r--r--   0 ericof     (501) staff       (20)       17 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-generate-files-permissions/input{{cookiecutter.permissions}}/simple.txt
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.094164 cookiecutter-2.2.0/tests/test-output-folder/
+-rw-r--r--   0 ericof     (501) staff       (20)      181 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-output-folder/cookiecutter.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.094381 cookiecutter-2.2.0/tests/test-output-folder/{{cookiecutter.test_name}}/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.094644 cookiecutter-2.2.0/tests/test-output-folder/{{cookiecutter.test_name}}/folder/
+-rw-r--r--   0 ericof     (501) staff       (20)       83 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-output-folder/{{cookiecutter.test_name}}/folder/in_folder.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       76 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-output-folder/{{cookiecutter.test_name}}/something.txt
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.094859 cookiecutter-2.2.0/tests/test-output-folder/{{cookiecutter.test_name}}/{{cookiecutter.folder_name}}/
+-rw-r--r--   0 ericof     (501) staff       (20)      128 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-output-folder/{{cookiecutter.test_name}}/{{cookiecutter.folder_name}}/{{cookiecutter.filename}}.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.008051 cookiecutter-2.2.0/tests/test-pyhooks/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.095196 cookiecutter-2.2.0/tests/test-pyhooks/hooks/
+-rw-r--r--   0 ericof     (501) staff       (20)      153 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-pyhooks/hooks/post_gen_project.py
+-rw-r--r--   0 ericof     (501) staff       (20)      151 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-pyhooks/hooks/pre_gen_project.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.095344 cookiecutter-2.2.0/tests/test-pyhooks/input{{cookiecutter.pyhooks}}/
+-rw-r--r--   0 ericof     (501) staff       (20)       13 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-pyhooks/input{{cookiecutter.pyhooks}}/README.rst
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.008295 cookiecutter-2.2.0/tests/test-pyshellhooks/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.095908 cookiecutter-2.2.0/tests/test-pyshellhooks/hooks/
+-rw-r--r--   0 ericof     (501) staff       (20)      153 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-pyshellhooks/hooks/post_gen_project.py
+-rwxr-xr-x   0 ericof     (501) staff       (20)       65 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-pyshellhooks/hooks/post_gen_project.sh
+-rw-r--r--   0 ericof     (501) staff       (20)      152 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-pyshellhooks/hooks/pre_gen_project.py
+-rwxr-xr-x   0 ericof     (501) staff       (20)       64 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-pyshellhooks/hooks/pre_gen_project.sh
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.096086 cookiecutter-2.2.0/tests/test-pyshellhooks/input{{pyshellhooks}}/
+-rw-r--r--   0 ericof     (501) staff       (20)       13 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-pyshellhooks/input{{pyshellhooks}}/README.rst
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.096453 cookiecutter-2.2.0/tests/test-replay/
+-rw-r--r--   0 ericof     (501) staff       (20)      161 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-replay/cookiedozer_load.json
+-rw-r--r--   0 ericof     (501) staff       (20)      165 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-replay/invalid_replay.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.009154 cookiecutter-2.2.0/tests/test-shellhooks/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.098322 cookiecutter-2.2.0/tests/test-shellhooks/hooks/
+-rwxr-xr-x   0 ericof     (501) staff       (20)       65 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-shellhooks/hooks/post_gen_project.sh
+-rwxr-xr-x   0 ericof     (501) staff       (20)       63 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-shellhooks/hooks/pre_gen_project.sh
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.098529 cookiecutter-2.2.0/tests/test-shellhooks/input{{cookiecutter.shellhooks}}/
+-rw-r--r--   0 ericof     (501) staff       (20)       13 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-shellhooks/input{{cookiecutter.shellhooks}}/README.rst
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.008595 cookiecutter-2.2.0/tests/test-shellhooks-empty/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.096652 cookiecutter-2.2.0/tests/test-shellhooks-empty/hooks/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-shellhooks-empty/hooks/pre_gen_project.sh
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.096784 cookiecutter-2.2.0/tests/test-shellhooks-empty/input{{cookiecutter.shellhooks}}/
+-rw-r--r--   0 ericof     (501) staff       (20)       43 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-shellhooks-empty/input{{cookiecutter.shellhooks}}/README.rst
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.008984 cookiecutter-2.2.0/tests/test-shellhooks-win/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.097392 cookiecutter-2.2.0/tests/test-shellhooks-win/hooks/
+-rw-r--r--   0 ericof     (501) staff       (20)       59 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-shellhooks-win/hooks/post_gen_project.bat
+-rw-r--r--   0 ericof     (501) staff       (20)       57 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-shellhooks-win/hooks/pre_gen_project.bat
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.097637 cookiecutter-2.2.0/tests/test-shellhooks-win/input{{cookiecutter.shellhooks}}/
+-rw-r--r--   0 ericof     (501) staff       (20)       13 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test-shellhooks-win/input{{cookiecutter.shellhooks}}/README.rst
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.009776 cookiecutter-2.2.0/tests/test-templates/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.098741 cookiecutter-2.2.0/tests/test-templates/extends/
+-rw-r--r--   0 ericof     (501) staff       (20)       89 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-templates/extends/cookiecutter.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.099398 cookiecutter-2.2.0/tests/test-templates/extends/templates/
+-rw-r--r--   0 ericof     (501) staff       (20)      252 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-templates/extends/templates/base-requirements.jinja
+-rw-r--r--   0 ericof     (501) staff       (20)        6 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-templates/extends/templates/click-requirements.jinja
+-rw-r--r--   0 ericof     (501) staff       (20)        7 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-templates/extends/templates/pytest-requirements.jinja
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.099598 cookiecutter-2.2.0/tests/test-templates/extends/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 ericof     (501) staff       (20)       40 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-templates/extends/{{cookiecutter.project_slug}}/requirements.txt
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.099920 cookiecutter-2.2.0/tests/test-templates/include/
+-rw-r--r--   0 ericof     (501) staff       (20)       89 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-templates/include/cookiecutter.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.100736 cookiecutter-2.2.0/tests/test-templates/include/templates/
+-rw-r--r--   0 ericof     (501) staff       (20)        6 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-templates/include/templates/click-requirements.jinja
+-rw-r--r--   0 ericof     (501) staff       (20)        7 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-templates/include/templates/pytest-requirements.jinja
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.101060 cookiecutter-2.2.0/tests/test-templates/include/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 ericof     (501) staff       (20)      213 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-templates/include/{{cookiecutter.project_slug}}/requirements.txt
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.101459 cookiecutter-2.2.0/tests/test-templates/no-templates/
+-rw-r--r--   0 ericof     (501) staff       (20)       89 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-templates/no-templates/cookiecutter.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.101687 cookiecutter-2.2.0/tests/test-templates/no-templates/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 ericof     (501) staff       (20)      143 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-templates/no-templates/{{cookiecutter.project_slug}}/requirements.txt
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.101919 cookiecutter-2.2.0/tests/test-templates/super/
+-rw-r--r--   0 ericof     (501) staff       (20)       89 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test-templates/super/cookiecutter.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.102726 cookiecutter-2.2.0/tests/test-templates/super/templates/
+-rw-r--r--   0 ericof     (501) staff       (20)      297 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-templates/super/templates/base-requirements.jinja
+-rw-r--r--   0 ericof     (501) staff       (20)        6 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-templates/super/templates/click-requirements.jinja
+-rw-r--r--   0 ericof     (501) staff       (20)        7 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-templates/super/templates/pytest-requirements.jinja
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.102971 cookiecutter-2.2.0/tests/test-templates/super/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 ericof     (501) staff       (20)       96 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test-templates/super/{{cookiecutter.project_slug}}/requirements.txt
+-rw-r--r--   0 ericof     (501) staff       (20)     1203 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_abort_generate_on_hook_error.py
+-rw-r--r--   0 ericof     (501) staff       (20)    20303 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test_cli.py
+-rw-r--r--   0 ericof     (501) staff       (20)      897 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_cookiecutter_invocation.py
+-rw-r--r--   0 ericof     (501) staff       (20)     4558 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_cookiecutter_local_no_input.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1681 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test_cookiecutter_local_with_input.py
+-rw-r--r--   0 ericof     (501) staff       (20)      527 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_cookiecutter_nested_templates.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1256 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_custom_extensions_in_hooks.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1849 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test_default_extensions.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1071 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test_environment.py
+-rw-r--r--   0 ericof     (501) staff       (20)      712 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_exceptions.py
+-rw-r--r--   0 ericof     (501) staff       (20)      555 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_find.py
+-rw-r--r--   0 ericof     (501) staff       (20)     8477 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test_generate_context.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2499 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_generate_copy_without_render.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3129 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_generate_copy_without_render_override.py
+-rw-r--r--   0 ericof     (501) staff       (20)     6102 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_generate_file.py
+-rw-r--r--   0 ericof     (501) staff       (20)    15950 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test_generate_files.py
+-rw-r--r--   0 ericof     (501) staff       (20)     8141 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_generate_hooks.py
+-rw-r--r--   0 ericof     (501) staff       (20)     4396 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_get_config.py
+-rw-r--r--   0 ericof     (501) staff       (20)     5403 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_get_user_config.py
+-rw-r--r--   0 ericof     (501) staff       (20)    10502 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_hooks.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3957 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_log.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3117 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test_main.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1918 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test_output_folder.py
+-rw-r--r--   0 ericof     (501) staff       (20)      847 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_preferred_encoding.py
+-rw-r--r--   0 ericof     (501) staff       (20)    19445 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test_prompt.py
+-rw-r--r--   0 ericof     (501) staff       (20)      480 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_read_repo_password.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1233 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_read_user_choice.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3628 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_read_user_dict.py
+-rw-r--r--   0 ericof     (501) staff       (20)      498 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_read_user_variable.py
+-rw-r--r--   0 ericof     (501) staff       (20)      524 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_read_user_yes_no.py
+-rw-r--r--   0 ericof     (501) staff       (20)      367 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_repo_not_found.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2323 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_specify_output_dir.py
+-rw-r--r--   0 ericof     (501) staff       (20)      933 2023-07-05 21:37:08.000000 cookiecutter-2.2.0/tests/test_templates.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2439 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/test_time_extension.py
+-rw-r--r--   0 ericof     (501) staff       (20)     6791 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/test_utils.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.010313 cookiecutter-2.2.0/tests/undefined-variable/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.010071 cookiecutter-2.2.0/tests/undefined-variable/dir-name/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.103236 cookiecutter-2.2.0/tests/undefined-variable/dir-name/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 ericof     (501) staff       (20)       84 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/undefined-variable/dir-name/{{cookiecutter.project_slug}}/README.rst
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.103587 cookiecutter-2.2.0/tests/undefined-variable/dir-name/{{cookiecutter.project_slug}}/{{cookiecutter.foobar}}/
+-rw-r--r--   0 ericof     (501) staff       (20)      121 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/undefined-variable/dir-name/{{cookiecutter.project_slug}}/{{cookiecutter.foobar}}/helloworld.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.010251 cookiecutter-2.2.0/tests/undefined-variable/file-content/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.103906 cookiecutter-2.2.0/tests/undefined-variable/file-content/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 ericof     (501) staff       (20)      192 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/undefined-variable/file-content/{{cookiecutter.project_slug}}/README.rst
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.104180 cookiecutter-2.2.0/tests/undefined-variable/file-name/
+-rw-r--r--   0 ericof     (501) staff       (20)       70 2023-06-18 20:18:21.000000 cookiecutter-2.2.0/tests/undefined-variable/file-name/cookiecutter.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.104396 cookiecutter-2.2.0/tests/undefined-variable/file-name/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 ericof     (501) staff       (20)       84 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/undefined-variable/file-name/{{cookiecutter.project_slug}}/{{cookiecutter.foobar}}
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.105185 cookiecutter-2.2.0/tests/vcs/
+-rw-r--r--   0 ericof     (501) staff       (20)     7144 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/vcs/test_clone.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2573 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/vcs/test_identify_repo.py
+-rw-r--r--   0 ericof     (501) staff       (20)      500 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/vcs/test_is_vcs_installed.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-07-06 16:27:19.105373 cookiecutter-2.2.0/tests/zipfile/
+-rw-r--r--   0 ericof     (501) staff       (20)     9611 2023-06-13 08:07:06.000000 cookiecutter-2.2.0/tests/zipfile/test_unzip.py
```

### Comparing `cookiecutter-2.1.1/AUTHORS.md` & `cookiecutter-2.2.0/AUTHORS.md`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
 ### PyCon 2016 Sprint
 
 The following people made contributions to the cookiecutter project at the PyCon sprints in Portland, OR from June 2-5 2016.
 Contributions include user testing, debugging, improving documentation, reviewing issues, writing tutorials, creating and updating project templates, and teaching each other.
 
 - Adam Chainz ([@adamchainz](https://github.com/adamchainz))
 - Andrew Ittner ([@tephyr](https://github.com/tephyr))
-- Audrey Roy Greenfeld ([@audreyr](https://github.com/audreyr))
+- Audrey Roy Greenfeld ([@audreyfeldroy](https://github.com/audreyfeldroy))
 - Carol Willing ([@willingc](https://github.com/willingc))
 - Christopher Clarke ([@chrisdev](https://github.com/chrisdev))
 - Citlalli Murillo ([@citmusa](https://github.com/citmusa))
 - Daniel Roy Greenfeld ([@pydanny](https://github.com/pydanny))
 - Diane DeMers Chen ([@purplediane](https://github.com/purplediane))
 - Elaine Wong ([@elainewong](https://github.com/elainewong))
 - Elias Dorneles ([@eliasdorneles](https://github.com/eliasdorneles))
```

### Comparing `cookiecutter-2.1.1/CONTRIBUTING.md` & `cookiecutter-2.2.0/CONTRIBUTING.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Contributing
 
 Contributions are welcome, and they are greatly appreciated!
 Every little bit helps, and credit will always be given.
 
-- [Types of Contributions](#Types-of-Contributions)
-- [Contributor Setup](#Setting-Up-the-Code-for-Local-Development)
-- [Contributor Guidelines](#Contributor-Guidelines)
-- [Contributor Testing](#Testing-with-tox)
-- [Core Committer Guide](#Core-Committer-Guide)
+- [Types of Contributions](#types-of-contributions)
+- [Contributor Setup](#setting-up-the-code-for-local-development)
+- [Contributor Guidelines](#contributor-guidelines)
+- [Contributor Testing](#testing-with-tox)
+- [Core Committer Guide](#core-committer-guide)
 
 ## Types of Contributions
 
 You can contribute in many ways:
 
 ### Report Bugs
 
@@ -94,23 +94,15 @@
 5. When you're done making changes, check that your changes pass the tests and lint check:
 
    ```bash
    pip install tox
    tox
    ```
 
-   Please note that tox runs lint check automatically, since we have a test environment for it.
-
-   If you feel like running only the lint environment, please use the following command:
-
-   ```bash
-   make lint
-   ```
-
-6. Ensure that your feature or commit is fully covered by tests. Check report after regular tox run.
+6. Ensure that your feature or commit is fully covered by tests. Check report after regular `tox` run.
    You can also run coverage only report and get html report with statement by statement highlighting:
 
    ```bash
    make coverage
    ```
 
    You report will be placed to `htmlcov` directory. Please do not include this directory to your commits.
@@ -162,39 +154,39 @@
     def is_pirate(message):
         """Return True if the given message sounds piratical."""
         return re.search(r"(?i)(arr|avast|yohoho)!", message) is not None
     ```
 
 ## Testing with tox
 
-Tox uses py.test under the hood, hence it supports the same syntax for selecting tests.
+`tox` uses `pytest` under the hood, hence it supports the same syntax for selecting tests.
 
 For further information please consult the [pytest usage docs](http://pytest.org/en/latest/example/index.html).
 
-To run a particular test class with tox:
+To run a particular test class with `tox`:
 
 ```bash
-tox -e py '-k TestFindHooks'
+tox -e py310 -- '-k TestFindHooks'
 ```
 
 To run some tests with names matching a string expression:
 
 ```bash
-tox -e py '-k generate'
+tox -e py310 -- '-k generate'
 ```
 
 Will run all tests matching "generate", test_generate_files for example.
 
 To run just one method:
 
 ```bash
-tox -e py '-k "TestFindHooks and test_find_hook"'
+tox -e py310 -- '-k "TestFindHooks and test_find_hook"'
 ```
 
-To run all tests using various versions of python in virtualenvs defined in tox.ini, just run tox:
+To run all tests using various versions of Python, just run `tox`:
 
 ```bash
 tox
 ```
 
 This configuration file setup the pytest-cov plugin and it is an additional dependency.
 It generate a coverage report after the tests.
```

### Comparing `cookiecutter-2.1.1/HISTORY.md` & `cookiecutter-2.2.0/HISTORY.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,94 @@
 # History
 
 History is important, but our current roadmap can be found [here](https://github.com/cookiecutter/cookiecutter/projects)
 
+
+## 2.2.0 (2023-07-06)
+
+### Changes
+
+* Added timeout on request.get() for ensuring that if a recipient serve… (#1772) @openrefactory
+* Fixing Carriage Return Line Feed (CRLF) order in docs #1792 (#1793) @Lahiry
+* Reduce I/O (#1877) @kurtmckee
+* Remove a pre-commit hook special case (#1875) @kurtmckee
+* Remove universal bdist_wheel option; use "python -m build" (#1739) @mwtoews
+* Remove unused import from post-generate hook script example (#1795) @KAZYPinkSaurus
+* Standardize newlines for all platforms (#1870) @kurtmckee
+* feat: Add resolved template repository path as _repo_dir to the context (#1771) @tmeckel
+
+### Minor Changes
+
+* Added support for providing human-readable prompts to the different variables (#1881) @vemonet
+* Added: Boolean variable support in JSON (#1626) @liortct
+* Added: CLI option to keep project files on failure. (#1669) @MaciejPatro
+* Added: Support partially overwrite keys in nested dict (#1692) @cksac
+* Added: Templates inheritance (#1485) @simobasso
+* Code quality: Tests upgrade: Use pathlib for files read/write (#1718) @insspb
+* Inline jinja2-time extension code (#1779) @tranzystorek-io
+* Support Python 3.11 (#1850) @kurtmckee
+* Support nested config files (#1770) @dariocurr
+* preserves original options in `_cookiecutter` (#1874) @kjaymiller
+
+### CI/CD and QA changes
+
+* Add a Dependabot config to autoupdate GitHub workflow actions (#1851) @kurtmckee
+* Added: Readthedocs build config (#1707) @insspb
+* Bump actions/setup-python from 3 to 4 (#1854) @dependabot
+* Bump paambaati/codeclimate-action from 3.0.0 to 4.0.0 (#1853) @dependabot
+* CI/CD: Tox -> Nox: Added nox configuration (#1706) @insspb
+* CI/CD: Tox -> Nox: Github actions definition minimized + Sync nox and github actions (#1714) @insspb
+* CI/CD: Tox -> Nox: Makefile update: Removed watchmedo and sed dependency, tox replaced with nox (#1713) @insspb
+* CI/CD: Updated .pre-commit-config.yaml to use latest hooks versions (#1712) @insspb
+* Code quality: Core files: Added exception reason reraise when exception class changed (PEP 3134) (#1719) @insspb
+* Code quality: Tests upgrade: Use pathlib for files read/write (#1718) @insspb
+* Code quality: core files: Format replaced with f-strings (#1716) @insspb
+* Code quality: find.py refactored and type annotated (#1721) @insspb
+* Code quality: tests files: Simplify statements fixes (#1717) @insspb
+* Code quality: utils.make_sure_path_exists refactored and type annotated (#1722) @insspb
+* Fixed: recommonmark replaced with myst, as recommonmark is deprecated (#1709) @insspb
+* Pretty-format JSON files (#1864) @kurtmckee
+* Rename `master` to `main` so CI runs correctly on merge (#1852) @kurtmckee
+* Standardize EOF newlines (#1876) @kurtmckee
+* Update `.gitignore` and cite where it was copied from (#1879) @kurtmckee
+* Update base docs, remove tox (#1858) @ericof
+* Update pre-commit hook versions (#1849) @kurtmckee
+* Updated: Release drafter configuration (#1704) @insspb
+* Use tox (#1866) @kurtmckee
+* Verify an expected warning is raised (#1869) @kurtmckee
+* fixed failing lint ci action by updating repo of flake8 (#1838) @Tamronimus
+
+### Documentation updates
+
+* Add jinja env docs (#1872) @pamelafox
+* Documentation extension: Create a Cookiecutter From Scratch tutorial (#1592) @miro-jelaska
+* Easy PR! Fix typos and add minor doc updates (#1741) @Alex0Blackwell
+* Expand cli documentation relating to the no-input flag (#1543) (#1587) @jeremyswerdlow
+* Fix @audreyr to @audreyfeldroy github account rename (#1604) @ri0t
+* Fixed broken links to jinja docs (#1691) @insspb
+* Fixed minor typos in docs (#1753) @segunb
+* Fixed: Python code block in the replay documentation (#1715) @juhannc
+* Fixed: recommonmark replaced with myst, as recommonmark is deprecated (#1709) @insspb
+* Improve Docs Readability (#1690) @ryanrussell
+* Update base docs, remove tox (#1858) @ericof
+* Updated: Boolean Variables documentation and docstrings (#1705) @italomaia
+* docs: fix simple typo, shat -> that (#1749) @timgates42
+* fixing badge display problem (#1798) @Paulokim1
+
+### Bugfixes
+
+* Fixed the override not working with copy only dir #1650 (#1651) @zhongdai
+* Fixed: Removed mention of packages versions, to exclude dependabot warnings alerts (#1711) @insspb
+* cleanup files if panics during hooks - bugfix (#1760) @liortct
+
+### This release is made by wonderful contributors:
+
+@Alex0Blackwell, @KAZYPinkSaurus, @Lahiry, @MaciejPatro, @Paulokim1, @Tamronimus, @cksac, @cookies-xor-cream, @dariocurr, @dependabot, @dependabot[bot], @ericof, @insspb, @italomaia, @jeremyswerdlow, @juhannc, @kjaymiller, @kurtmckee, @liortct, @miro-jelaska, @mwtoews, @openrefactory, @pamelafox, @ri0t, @ryanrussell, @segunb, @simobasso, @timgates42, @tmeckel, @tranzystorek-io, @vemonet and @zhongdai
+
+
 ## 2.1.1 (2022-06-01)
 
 ### Documentation updates
 
 * Fix local extensions documentation (#1686) @alkatar21
 
 ### Bugfixes
@@ -219,15 +302,15 @@
 * Fixed tests sequence for appveyor, to exclude file not found bug. Thanks to [@insspb](https://github.com/insspb) (#1257)
 * Updates REAMDE.md with svg badge for appveyor. Thanks to [@sobolevn](https://github.com/sobolevn) (#1254)
 * Add missing {% endif %} to Choice Variables example. Thanks to [@mattstibbs](https://github.com/mattstibbs) (#1249)
 * Core documentation converted to Markdown format thanks to [@wagnernegrao](https://github.com/wagnernegrao), [@insspb](https://github.com/insspb) (#1216)
 * Tests update: use sys.executable when invoking python in python 3 only environment thanks to [@vincentbernat](https://github.com/vincentbernat) (#1221)
 * Prevent `click` API v7.0 from showing choices when already shown, thanks to [@rly](https://github.com/rly) and [@luzfcb](https://github.com/luzfcb) (#1168)
 * Test the codebase with python3.8 beta on tox and travis-ci (#1206), thanks to [@mihrab34](https://github.com/mihrab34)
-* Add a [CODE\_OF\_CONDUCT.md](https://github.com/audreyr/cookiecutter/blob/master/CODE_OF_CONDUCT.md) file to the project, thanks to [@andreagrandi](https://github.com/andreagrandi) (#1009)
+* Add a [CODE\_OF\_CONDUCT.md](https://github.com/audreyfeldroy/cookiecutter/blob/master/CODE_OF_CONDUCT.md) file to the project, thanks to [@andreagrandi](https://github.com/andreagrandi) (#1009)
 * Update docstrings in `cookiecutter/main.py`, `cookiecutter/__init__.py`, and `cookiecutter/log.py` to follow the PEP 257 style guide, thanks to [@meahow](https://github.com/meahow) (#998, #999, #1000)
 * Update docstrings in `cookiecutter/utils.py` to follow the PEP 257 style guide, thanks to [@dornheimer](https://github.com/dornheimer)(#1026)
 * Fix grammar in *Choice Variables* documentation, thanks to [@jubrilissa](https://github.com/jubrilissa) (#1011)
 * Update installation docs with links to the Windows Subsystem and GNU utilities, thanks to [@Nythiennzo](https://github.com/Nythiennzo) for the PR and [@BruceEckel](https://github.com/BruceEckel) for the review (#1016)
 * Upgrade flake8 to version 3.5.0, thanks to [@cclauss](https://github.com/cclauss) (#1038)
 * Update tutorial with explanation for how cookiecutter finds the template file, thanks to [@accraze](https://github.com/accraze)(#1025)
 * Update CI config files to use `TOXENV` environment variable, thanks to [@asottile](https://github.com/asottile) (#1019)
@@ -396,15 +479,15 @@
 * Add a make rule to update git submodules, thanks to [@hackebrot](https://github.com/hackebrot) (#746)
 * Split up advanced usage docs, thanks to [@zzzirk](https://github.com/zzzirk) (#749)
 * Documentation for the `no_input` option, thanks to [@pokoli](https://github.com/pokoli/) (#701)
 * Remove unnecessary shebangs from python files, thanks to [@michaeljoseph](https://github.com/michaeljoseph) (#763)
 * Refactor cookiecutter template identification, thanks to [@michaeljoseph](https://github.com/michaeljoseph) (#777)
 * Add a `cli_runner` test fixture to simplify CLI tests, thanks to [@hackebrot](https://github.com/hackebrot) (#790)
 * Add a check to ensure cookiecutter repositories have JSON context, thanks to [@michaeljoseph](https://github.com/michaeljoseph)(#782)
-* Rename the internal function that determines whether a file should be rendered, thanks to [@audreyr](https://github.com/audreyr) for raising the issue and [@hackebrot](https://github.com/hackebrot)for the PR (#741, #802)
+* Rename the internal function that determines whether a file should be rendered, thanks to [@audreyfeldroy](https://github.com/audreyfeldroy) for raising the issue and [@hackebrot](https://github.com/hackebrot)for the PR (#741, #802)
 * Fix typo in docs, thanks to [@mwarkentin](https://github.com/mwarkentin) (#828)
 * Fix broken link to *Invoke* docs, thanks to [@B3QL](https://github.com/B3QL) (#820)
 * Add documentation to `render_variable` function in `prompt.py`, thanks to [@pydanny](https://github.com/pydanny) (#678)
 * Fix python3.6 travis-ci and tox configuration, thanks to [@luzfcb](https://github.com/luzfcb) (#844)
 * Add missing encoding declarations to python files, thanks to [@andytom](https://github.com/andytom) (#852)
 * Disable poyo logging for tests, thanks to [@hackebrot](https://github.com/hackebrot) (#855)
 * Remove pycache directories in make clean-pyc, thanks to [@hackebrot](https://github.com/hackebrot) (#849)
@@ -474,19 +557,19 @@
 
 Other Changes:
 
 * Set path before running tox, thanks to [@maiksensi](https://github.com/maiksensi) (#615, #620)
 * Removed xfail in test\_cookiecutters, thanks to [@hackebrot](https://github.com/hackebrot) (#618)
 * Removed django-cms-plugin on account of 404 error, thanks to [@mativs](https://github.com/mativs) and [@pydanny](https://github.com/pydanny) (#593)
 * Fixed docs/usage.rst, thanks to [@macrotim](https://github.com/macrotim) (#604)
-* Update .gitignore to latest Python.gitignore and ignore PyCharm files, thanks to [@audreyr](https://github.com/audreyr)
+* Update .gitignore to latest Python.gitignore and ignore PyCharm files, thanks to [@audreyfeldroy](https://github.com/audreyfeldroy)
 * Use open context manager to read context\_file in generate() function, thanks to [@hackebrot](https://github.com/hackebrot)
 (#607, #608)
 * Added documentation for choice variables, thanks to [@maiksensi](https://github.com/maiksensi) (#611)
-* Set up Scrutinizer to check code quality, thanks to [@audreyr](https://github.com/audreyr)
+* Set up Scrutinizer to check code quality, thanks to [@audreyfeldroy](https://github.com/audreyfeldroy)
 * Drop distutils support in setup.py, thanks to [@hackebrot](https://github.com/hackebrot) (#606, #609)
 * Change cookiecutter-pypackage-minimal link, thanks to [@kragniz](https://github.com/kragniz) (#614)
 * Fix typo in one of the template\'s description, thanks to [@ryanfreckleton](https://github.com/ryanfreckleton) (#643)
 * Fix broken link to [\_copy\_without\_render](http://cookiecutter.readthedocs.io/en/latest/advanced_usage.html#copy-without-render)
     in *troubleshooting.rst*, thanks to [@ptim](https://github.com/ptim) (#647)
 
 * Added more cookiecutter templates to the mix:
@@ -541,15 +624,15 @@
 
 * Factor in *choice* variables (as introduced in 1.1.0) when using a user config or extra context, thanks to [@ionelmc](https://github.com/ionelmc) and [@hackebrot](https://github.com/hackebrot) (#536, #542).
 
 Other Changes:
 
 * Enable py35 support on Travis by using Python 3.5 as base Python ([@maiksensi](https://github.com/maiksensi) / #540)
 * If a filename is empty, do not generate. Log instead ([@iljabauer](https://github.com/iljabauer) / #444)
-* Fix tests as per last changes in [cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage), thanks to [@eliasdorneles](https://github.com/eliasdorneles)(#555).
+* Fix tests as per last changes in [cookiecutter-pypackage](https://github.com/audreyfeldroy/cookiecutter-pypackage), thanks to [@eliasdorneles](https://github.com/eliasdorneles)(#555).
 * Removed deprecated cookiecutter-pylibrary-minimal from the list, thanks to [@ionelmc](https://github.com/ionelmc) (#556)
 * Moved to using rualmel.yaml instead of PyYAML, except for Windows users on Python 2.7, thanks
     to [@pydanny](https://github.com/pydanny) (#557)
 
 *Why 1.2.1 instead of 1.2.0? There was a problem in the distribution that we pushed to PyPI. Since you can\'t replace previous files uploaded to PyPI, we deleted the files on PyPI and released 1.2.1.*
 
 ## 1.1.0 (2015-09-26) Snickerdoodle
@@ -664,15 +747,15 @@
 
 ## 0.8.0 (2014-10-30)
 
 The goal of this release was to allow for injection of extra context via the Cookiecutter API, and to fix minor bugs.
 
 Features:
 
-* cookiecutter() now takes an optional extra\_context parameter, thanks to [@michaeljoseph](https://github.com/michaeljoseph), [@fcurella](https://github.com/fcurella), [@aventurella](https://github.com/aventurella),  [@emonty](https://github.com/emonty), [@schacki](https://github.com/schacki), [@ryanolson](https://github.com/ryanolson), [@pfmoore](https://github.com/pfmoore), [@pydanny](https://github.com/pydanny), [@audreyr](https://github.com/audreyr) (#260).
+* cookiecutter() now takes an optional extra\_context parameter, thanks to [@michaeljoseph](https://github.com/michaeljoseph), [@fcurella](https://github.com/fcurella), [@aventurella](https://github.com/aventurella),  [@emonty](https://github.com/emonty), [@schacki](https://github.com/schacki), [@ryanolson](https://github.com/ryanolson), [@pfmoore](https://github.com/pfmoore), [@pydanny](https://github.com/pydanny), [@audreyfeldroy](https://github.com/audreyfeldroy) (#260).
 * Context is now injected into hooks, thanks to [@michaeljoseph](https://github.com/michaeljoseph) and [@dinopetrone](https://github.com/dinopetrone).
 * Moved all Python 2/3 compatibility code into cookiecutter.compat, making the eventual move to six easier, thanks to [@michaeljoseph](https://github.com/michaeljoseph) (#60, #102).
 * Added cookiecutterrc defined aliases for cookiecutters, thanks to [@pfmoore](https://github.com/pfmoore) (#246)
 * Added flake8 to tox to check for pep8 violations, thanks to [@natim](https://github.com/Natim).
 
 Bug Fixes:
 
@@ -704,20 +787,20 @@
 * Made rmtree remove readonly files, thanks to [@pfmoore](https://github.com/pfmoore).
 * Now using tox to run tests on Appveyor, thanks to [@pfmoore](https://github.com/pfmoore) (#241).
 * Fixed tests that assumed the system encoding was utf-8, thanks to [@pfmoore](https://github.com/pfmoore) (#242, #244).
 * Added a tox ini file that uses py.test, thanks to [@pfmoore](https://github.com/pfmoore) (#245).
 
 Other Changes:
 
-* [@audreyr](https://github.com/audreyr) formally accepted position as **BDFL of cookiecutter**.
+* [@audreyfeldroy](https://github.com/audreyfeldroy) formally accepted position as **BDFL of cookiecutter**.
 * Elevated [@pydanny](https://github.com/pydanny), [@michaeljoseph](https://github.com/michaeljoseph), and [@pfmoore](https://github.com/pfmoore) to core committer status.
-* Added Core Committer guide, by [@audreyr](https://github.com/audreyr).
-* Generated apidocs from make docs, by [@audreyr](https://github.com/audreyr).
+* Added Core Committer guide, by [@audreyfeldroy](https://github.com/audreyfeldroy).
+* Generated apidocs from make docs, by [@audreyfeldroy](https://github.com/audreyfeldroy).
 * Added contributing command to the makedocs function, by [@pydanny](https://github.com/pydanny).
-* Refactored contributing documentation, included adding core committer instructions, by [@pydanny](https://github.com/pydanny) and [@audreyr](https://github.com/audreyr).
+* Refactored contributing documentation, included adding core committer instructions, by [@pydanny](https://github.com/pydanny) and [@audreyfeldroy](https://github.com/audreyfeldroy).
 * Do not convert input prompt to bytes, thanks to [@uranusjr](https://github.com/uranusjr) (#192).
 * Added troubleshooting info about Python 3.3 tests and tox.
 * Added documentation about command line arguments, thanks to [@saxix](https://github.com/saxix).
 * Style cleanups.
 * Added environment variable to disable network tests for environments without networking, thanks to [@vincentbernat](https://github.com/vincentbernat).
 * Added Appveyor support to aid Windows integrations, thanks to [@pydanny](https://github.com/pydanny) (#215).
 * CONTRIBUTING.rst is now generated via make contributing, thanks to [@pydanny](https://github.com/pydanny) (#220).
@@ -816,27 +899,27 @@
 
 * Friendlier, more simplified command line usage:
 
 ```bash
     # Create project from the cookiecutter-pypackage/ template
     $ cookiecutter cookiecutter-pypackage/
     # Create project from the cookiecutter-pypackage.git repo template
-    $ cookiecutter https://github.com/audreyr/cookiecutter-pypackage.git
+    $ cookiecutter https://github.com/audreyfeldroy/cookiecutter-pypackage.git
 ```
 
 * Can now use Cookiecutter from Python as a package:
 
 ```python
     from cookiecutter.main import cookiecutter
 
     # Create project from the cookiecutter-pypackage/ template
     cookiecutter('cookiecutter-pypackage/')
 
     # Create project from the cookiecutter-pypackage.git repo template
-    cookiecutter('https://github.com/audreyr/cookiecutter-pypackage.git')
+    cookiecutter('https://github.com/audreyfeldroy/cookiecutter-pypackage.git')
 ```
 
 * Internal refactor to remove any code that changes the working
     directory.
 
 ## 0.4 (2013-07-22)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cookiecutter-2.1.1/LICENSE` & `cookiecutter-2.2.0/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2013-2021, Audrey Roy Greenfeld
+Copyright (c) 2013-2022, Audrey Roy Greenfeld
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following
 conditions are met:
 
 * Redistributions of source code must retain the above copyright
```

### Comparing `cookiecutter-2.1.1/PKG-INFO` & `cookiecutter-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,60 +1,71 @@
 Metadata-Version: 2.1
 Name: cookiecutter
-Version: 2.1.1
+Version: 2.2.0
 Summary: A command-line utility that creates projects from project templates, e.g. creating a Python package project from a Python package project template.
 Home-page: https://github.com/cookiecutter/cookiecutter
 Author: Audrey Feldroy
 Author-email: audreyr@gmail.com
 License: BSD
+Project-URL: Documentation, https://cookiecutter.readthedocs.io
+Project-URL: Issues, https://github.com/cookiecutter/cookiecutter/issues
+Project-URL: Discord, https://discord.gg/9BrxzPKuEW
 Keywords: cookiecutter,Python,projects,project templates,Jinja2,skeleton,scaffolding,project directory,package,packaging
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
-# Cookiecutter
+<h1 align="center">
+    <img alt="cookiecutter Logo" width="200px" src="https://raw.githubusercontent.com/cookiecutter/cookiecutter/3ac078356adf5a1a72042dfe72ebfa4a9cd5ef38/logo/cookiecutter_medium.png">
+</h1>
+
+<div align="center">
 
 [![pypi](https://img.shields.io/pypi/v/cookiecutter.svg)](https://pypi.org/project/cookiecutter/)
 [![python](https://img.shields.io/pypi/pyversions/cookiecutter.svg)](https://pypi.org/project/cookiecutter/)
-[![Build Status](https://github.com/cookiecutter/cookiecutter/actions/workflows/main.yml/badge.svg?branch=master)](https://github.com/cookiecutter/cookiecutter/actions)
+[![Build Status](https://github.com/cookiecutter/cookiecutter/actions/workflows/tests.yml/badge.svg?branch=master)](https://github.com/cookiecutter/cookiecutter/actions)
 [![codecov](https://codecov.io/gh/cookiecutter/cookiecutter/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/cookiecutter/cookiecutter?branch=master)
 [![discord](https://img.shields.io/badge/Discord-cookiecutter-5865F2?style=flat&logo=discord&logoColor=white)](https://discord.gg/9BrxzPKuEW)
 [![docs](https://readthedocs.org/projects/cookiecutter/badge/?version=latest)](https://readthedocs.org/projects/cookiecutter/?badge=latest)
 [![Code Quality](https://img.shields.io/scrutinizer/g/cookiecutter/cookiecutter.svg)](https://scrutinizer-ci.com/g/cookiecutter/cookiecutter/?branch=master)
 
+</div>
+
+# cookiecutter
+
 A command-line utility that creates projects from **cookiecutters** (project templates), e.g. creating a Python package project from a Python package project template.
 
 - Documentation: [https://cookiecutter.readthedocs.io](https://cookiecutter.readthedocs.io)
 - GitHub: [https://github.com/cookiecutter/cookiecutter](https://github.com/cookiecutter/cookiecutter)
 - PyPI: [https://pypi.org/project/cookiecutter/](https://pypi.org/project/cookiecutter/)
-- Free and open source software: [BSD license](https://github.com/cookiecutter/cookiecutter/blob/master/LICENSE)
+- Free and open source software: [BSD license](https://github.com/cookiecutter/cookiecutter/blob/main/LICENSE)
 
-![Cookiecutter](https://raw.githubusercontent.com/cookiecutter/cookiecutter/3ac078356adf5a1a72042dfe72ebfa4a9cd5ef38/logo/cookiecutter_medium.png)
 
 ## Features
 
 - Cross-platform: Windows, Mac, and Linux are officially supported.
 - You don't have to know/write Python code to use Cookiecutter.
-- Works with Python 3.7, 3.8, 3.9., 3.10
+- Works with Python 3.7, 3.8, 3.9, 3.10, 3.11
 - Project templates can be in any programming language or markup format:
   Python, JavaScript, Ruby, CoffeeScript, RST, Markdown, CSS, HTML, you name it.
   You can use multiple languages in the same project template.
 
 ### For users of existing templates
 
 - Simple command line usage:
@@ -109,88 +120,92 @@
   ```bash
   # Clone cookiecutter-pypackage
   $ cookiecutter gh:audreyfeldroy/cookiecutter-pypackage
   # Now you can use the already cloned cookiecutter by name
   $ cookiecutter cookiecutter-pypackage
   ```
 
-- You can use local cookiecutters, or remote cookiecutters directly from Git repos or from Mercurial repos on Bitbucket.
-- Default context: specify key/value pairs that you want used as defaults  whenever you generate a project.
+- You can use local cookiecutters, or remote cookiecutters directly from Git repos or Mercurial repos on Bitbucket.
+- Default context: specify key/value pairs that you want to be used as defaults whenever you generate a project.
 - Inject extra context with command-line arguments:
 
   ```bash
   cookiecutter --no-input gh:msabramo/cookiecutter-supervisor program_name=foobar startsecs=10
   ```
 
-- Direct access to the Cookiecutter API allows for injection of extra context.
+- Direct access to the Cookiecutter API allows for the injection of extra context.
 - Paths to local projects can be specified as absolute or relative.
-- Projects generated to your current directory or to target directory if specified with `-o` option.
+Projects are generated to your current directory or to the target directory if specified with `-o` option.
 
 ### For template creators
 
 - Supports unlimited levels of directory nesting.
 - 100% of templating is done with Jinja2.
 - Both, directory names and filenames can be templated.
   For example:
 
   ```py
   {{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}.py
   ```
-- Simply define your template variables in a `cookiecutter.json` file.
+- Simply define your template variables in a `cookiecutter.json` file. You can also add human-readable questions that will be prompted to the user for each variable using the `__prompts__` key.
   For example:
 
   ```json
   {
     "full_name": "Audrey Roy Greenfeld",
     "email": "audreyr@gmail.com",
     "project_name": "Complexity",
     "repo_name": "complexity",
     "project_short_description": "Refreshingly simple static site generator.",
     "release_date": "2013-07-10",
     "year": "2013",
-    "version": "0.1.1"
+    "version": "0.1.1",
+    "__prompts__": {
+      "full_name": "Provide your full name",
+      "email": "Provide your email"
+    }
   }
   ```
 - Pre- and post-generate hooks: Python or shell scripts to run before or after generating a project.
 
 ## Available Cookiecutters
 
 Making great cookies takes a lot of cookiecutters and contributors.
 We're so pleased that there are many Cookiecutter project templates to choose from.
 We hope you find a cookiecutter that is just right for your needs.
 
 ### A Pantry Full of Cookiecutters
 
-The best place to start searching for specific and ready to use cookiecutter template is [Github search](https://github.com/search?q=cookiecutter&type=Repositories).
+The best place to start searching for specific and ready-to-use cookiecutter templates is [Github search](https://github.com/search?q=cookiecutter&type=Repositories).
 Just type `cookiecutter` and you will discover over 4000 related repositories.
 
-We also recommend you to check related GitHub topics.
+We also recommend you check related GitHub topics.
 For general search use [cookiecutter-template](https://github.com/topics/cookiecutter-template).
 For specific topics try to use `cookiecutter-yourtopic`, like `cookiecutter-python` or `cookiecutter-datascience`.
 This is a new GitHub feature, so not all active repositories use it at the moment.
 
-If you are template developer please add related [topics](https://help.github.com/en/github/administering-a-repository/classifying-your-repository-with-topics) with `cookiecutter` prefix to you repository.
+If you are a template developer please add related [topics](https://help.github.com/en/github/administering-a-repository/classifying-your-repository-with-topics) with `cookiecutter` prefix to your repository.
 We believe it will make it more discoverable.
-You are almost not limited in topics amount, use it!
+You are almost not limited in topic amount, use it!
 
 ### Cookiecutter Specials
 
 These Cookiecutters are maintained by the cookiecutter team:
 
 - [cookiecutter-pypackage](https://github.com/audreyfeldroy/cookiecutter-pypackage):
   ultimate Python package project template by [@audreyfeldroy's](https://github.com/audreyfeldroy).
 - [cookiecutter-django](https://github.com/pydanny/cookiecutter-django):
   a framework for jumpstarting production-ready Django projects quickly.
-  It is bleeding edge with Bootstrap 5, customizable users app, starter templates, working user registration, celery setup, and much more.
+  It is bleeding edge with Bootstrap 5, a customizable users app, starter templates, working user registration, celery setup, and much more.
 - [cookiecutter-pytest-plugin](https://github.com/pytest-dev/cookiecutter-pytest-plugin):
   Minimal Cookiecutter template for authoring [pytest](https://docs.pytest.org/) plugins that help you to write better programs.
 
 ## Community
 
-The core committer team can be found in [authors section](AUTHORS.md).
+The core committer team can be found in the [authors' section](AUTHORS.md).
 We are always welcome and invite you to participate.
 
 Stuck? Try one of the following:
 
 - See the [Troubleshooting](https://cookiecutter.readthedocs.io/en/latest/troubleshooting.html) page.
 - Ask for help on [Stack Overflow](https://stackoverflow.com/questions/tagged/cookiecutter).
 - You are strongly encouraged to [file an issue](https://github.com/cookiecutter/cookiecutter/issues?q=is%3Aopen) about the problem.
@@ -236,14 +251,14 @@
 
 This project is run by volunteers.
 Shortly we will be providing means for organizations and individuals to support the project.
 
 ## Code of Conduct
 
 Everyone interacting in the Cookiecutter project's codebases and documentation is expected to follow the [PyPA Code of Conduct](https://www.pypa.io/en/latest/code-of-conduct/).
-This includes, but is not limited to, issue trackers, chat rooms, mailing lists, and other virtual or in real life communication.
+This includes but is not limited to, issue trackers, chat rooms, mailing lists, and other virtual or in real-life communication.
 
 ## Creator / Leader
 
-This project was created and is led by [Audrey Roy Greenfeld](https://github.com/audreyfeldroy).
+This project was created and led by [Audrey Roy Greenfeld](https://github.com/audreyfeldroy).
 
 She is supported by a team of maintainers.
```

### Comparing `cookiecutter-2.1.1/README.md` & `cookiecutter-2.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,38 @@
-# Cookiecutter
+<h1 align="center">
+    <img alt="cookiecutter Logo" width="200px" src="https://raw.githubusercontent.com/cookiecutter/cookiecutter/3ac078356adf5a1a72042dfe72ebfa4a9cd5ef38/logo/cookiecutter_medium.png">
+</h1>
+
+<div align="center">
 
 [![pypi](https://img.shields.io/pypi/v/cookiecutter.svg)](https://pypi.org/project/cookiecutter/)
 [![python](https://img.shields.io/pypi/pyversions/cookiecutter.svg)](https://pypi.org/project/cookiecutter/)
-[![Build Status](https://github.com/cookiecutter/cookiecutter/actions/workflows/main.yml/badge.svg?branch=master)](https://github.com/cookiecutter/cookiecutter/actions)
+[![Build Status](https://github.com/cookiecutter/cookiecutter/actions/workflows/tests.yml/badge.svg?branch=master)](https://github.com/cookiecutter/cookiecutter/actions)
 [![codecov](https://codecov.io/gh/cookiecutter/cookiecutter/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/cookiecutter/cookiecutter?branch=master)
 [![discord](https://img.shields.io/badge/Discord-cookiecutter-5865F2?style=flat&logo=discord&logoColor=white)](https://discord.gg/9BrxzPKuEW)
 [![docs](https://readthedocs.org/projects/cookiecutter/badge/?version=latest)](https://readthedocs.org/projects/cookiecutter/?badge=latest)
 [![Code Quality](https://img.shields.io/scrutinizer/g/cookiecutter/cookiecutter.svg)](https://scrutinizer-ci.com/g/cookiecutter/cookiecutter/?branch=master)
 
+</div>
+
+# cookiecutter
+
 A command-line utility that creates projects from **cookiecutters** (project templates), e.g. creating a Python package project from a Python package project template.
 
 - Documentation: [https://cookiecutter.readthedocs.io](https://cookiecutter.readthedocs.io)
 - GitHub: [https://github.com/cookiecutter/cookiecutter](https://github.com/cookiecutter/cookiecutter)
 - PyPI: [https://pypi.org/project/cookiecutter/](https://pypi.org/project/cookiecutter/)
-- Free and open source software: [BSD license](https://github.com/cookiecutter/cookiecutter/blob/master/LICENSE)
+- Free and open source software: [BSD license](https://github.com/cookiecutter/cookiecutter/blob/main/LICENSE)
 
-![Cookiecutter](https://raw.githubusercontent.com/cookiecutter/cookiecutter/3ac078356adf5a1a72042dfe72ebfa4a9cd5ef38/logo/cookiecutter_medium.png)
 
 ## Features
 
 - Cross-platform: Windows, Mac, and Linux are officially supported.
 - You don't have to know/write Python code to use Cookiecutter.
-- Works with Python 3.7, 3.8, 3.9., 3.10
+- Works with Python 3.7, 3.8, 3.9, 3.10, 3.11
 - Project templates can be in any programming language or markup format:
   Python, JavaScript, Ruby, CoffeeScript, RST, Markdown, CSS, HTML, you name it.
   You can use multiple languages in the same project template.
 
 ### For users of existing templates
 
 - Simple command line usage:
@@ -80,88 +87,92 @@
   ```bash
   # Clone cookiecutter-pypackage
   $ cookiecutter gh:audreyfeldroy/cookiecutter-pypackage
   # Now you can use the already cloned cookiecutter by name
   $ cookiecutter cookiecutter-pypackage
   ```
 
-- You can use local cookiecutters, or remote cookiecutters directly from Git repos or from Mercurial repos on Bitbucket.
-- Default context: specify key/value pairs that you want used as defaults  whenever you generate a project.
+- You can use local cookiecutters, or remote cookiecutters directly from Git repos or Mercurial repos on Bitbucket.
+- Default context: specify key/value pairs that you want to be used as defaults whenever you generate a project.
 - Inject extra context with command-line arguments:
 
   ```bash
   cookiecutter --no-input gh:msabramo/cookiecutter-supervisor program_name=foobar startsecs=10
   ```
 
-- Direct access to the Cookiecutter API allows for injection of extra context.
+- Direct access to the Cookiecutter API allows for the injection of extra context.
 - Paths to local projects can be specified as absolute or relative.
-- Projects generated to your current directory or to target directory if specified with `-o` option.
+Projects are generated to your current directory or to the target directory if specified with `-o` option.
 
 ### For template creators
 
 - Supports unlimited levels of directory nesting.
 - 100% of templating is done with Jinja2.
 - Both, directory names and filenames can be templated.
   For example:
 
   ```py
   {{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}.py
   ```
-- Simply define your template variables in a `cookiecutter.json` file.
+- Simply define your template variables in a `cookiecutter.json` file. You can also add human-readable questions that will be prompted to the user for each variable using the `__prompts__` key.
   For example:
 
   ```json
   {
     "full_name": "Audrey Roy Greenfeld",
     "email": "audreyr@gmail.com",
     "project_name": "Complexity",
     "repo_name": "complexity",
     "project_short_description": "Refreshingly simple static site generator.",
     "release_date": "2013-07-10",
     "year": "2013",
-    "version": "0.1.1"
+    "version": "0.1.1",
+    "__prompts__": {
+      "full_name": "Provide your full name",
+      "email": "Provide your email"
+    }
   }
   ```
 - Pre- and post-generate hooks: Python or shell scripts to run before or after generating a project.
 
 ## Available Cookiecutters
 
 Making great cookies takes a lot of cookiecutters and contributors.
 We're so pleased that there are many Cookiecutter project templates to choose from.
 We hope you find a cookiecutter that is just right for your needs.
 
 ### A Pantry Full of Cookiecutters
 
-The best place to start searching for specific and ready to use cookiecutter template is [Github search](https://github.com/search?q=cookiecutter&type=Repositories).
+The best place to start searching for specific and ready-to-use cookiecutter templates is [Github search](https://github.com/search?q=cookiecutter&type=Repositories).
 Just type `cookiecutter` and you will discover over 4000 related repositories.
 
-We also recommend you to check related GitHub topics.
+We also recommend you check related GitHub topics.
 For general search use [cookiecutter-template](https://github.com/topics/cookiecutter-template).
 For specific topics try to use `cookiecutter-yourtopic`, like `cookiecutter-python` or `cookiecutter-datascience`.
 This is a new GitHub feature, so not all active repositories use it at the moment.
 
-If you are template developer please add related [topics](https://help.github.com/en/github/administering-a-repository/classifying-your-repository-with-topics) with `cookiecutter` prefix to you repository.
+If you are a template developer please add related [topics](https://help.github.com/en/github/administering-a-repository/classifying-your-repository-with-topics) with `cookiecutter` prefix to your repository.
 We believe it will make it more discoverable.
-You are almost not limited in topics amount, use it!
+You are almost not limited in topic amount, use it!
 
 ### Cookiecutter Specials
 
 These Cookiecutters are maintained by the cookiecutter team:
 
 - [cookiecutter-pypackage](https://github.com/audreyfeldroy/cookiecutter-pypackage):
   ultimate Python package project template by [@audreyfeldroy's](https://github.com/audreyfeldroy).
 - [cookiecutter-django](https://github.com/pydanny/cookiecutter-django):
   a framework for jumpstarting production-ready Django projects quickly.
-  It is bleeding edge with Bootstrap 5, customizable users app, starter templates, working user registration, celery setup, and much more.
+  It is bleeding edge with Bootstrap 5, a customizable users app, starter templates, working user registration, celery setup, and much more.
 - [cookiecutter-pytest-plugin](https://github.com/pytest-dev/cookiecutter-pytest-plugin):
   Minimal Cookiecutter template for authoring [pytest](https://docs.pytest.org/) plugins that help you to write better programs.
 
 ## Community
 
-The core committer team can be found in [authors section](AUTHORS.md).
+The core committer team can be found in the [authors' section](AUTHORS.md).
 We are always welcome and invite you to participate.
 
 Stuck? Try one of the following:
 
 - See the [Troubleshooting](https://cookiecutter.readthedocs.io/en/latest/troubleshooting.html) page.
 - Ask for help on [Stack Overflow](https://stackoverflow.com/questions/tagged/cookiecutter).
 - You are strongly encouraged to [file an issue](https://github.com/cookiecutter/cookiecutter/issues?q=is%3Aopen) about the problem.
@@ -207,14 +218,14 @@
 
 This project is run by volunteers.
 Shortly we will be providing means for organizations and individuals to support the project.
 
 ## Code of Conduct
 
 Everyone interacting in the Cookiecutter project's codebases and documentation is expected to follow the [PyPA Code of Conduct](https://www.pypa.io/en/latest/code-of-conduct/).
-This includes, but is not limited to, issue trackers, chat rooms, mailing lists, and other virtual or in real life communication.
+This includes but is not limited to, issue trackers, chat rooms, mailing lists, and other virtual or in real-life communication.
 
 ## Creator / Leader
 
-This project was created and is led by [Audrey Roy Greenfeld](https://github.com/audreyfeldroy).
+This project was created and led by [Audrey Roy Greenfeld](https://github.com/audreyfeldroy).
 
 She is supported by a team of maintainers.
```

### Comparing `cookiecutter-2.1.1/cookiecutter/cli.py` & `cookiecutter-2.2.0/cookiecutter/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,40 +23,39 @@
 from cookiecutter.config import get_user_config
 
 
 def version_msg():
     """Return the Cookiecutter version, location and Python powering it."""
     python_version = sys.version
     location = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
-    message = 'Cookiecutter %(version)s from {} (Python {})'
-    return message.format(location, python_version)
+    return f"Cookiecutter {__version__} from {location} (Python {python_version})"
 
 
 def validate_extra_context(ctx, param, value):
     """Validate extra context."""
-    for s in value:
-        if '=' not in s:
+    for string in value:
+        if '=' not in string:
             raise click.BadParameter(
-                'EXTRA_CONTEXT should contain items of the form key=value; '
-                "'{}' doesn't match that form".format(s)
+                f"EXTRA_CONTEXT should contain items of the form key=value; "
+                f"'{string}' doesn't match that form"
             )
 
     # Convert tuple -- e.g.: ('program_name=foobar', 'startsecs=66')
     # to dict -- e.g.: {'program_name': 'foobar', 'startsecs': '66'}
     return collections.OrderedDict(s.split('=', 1) for s in value) or None
 
 
 def list_installed_templates(default_config, passed_config_file):
     """List installed (locally cloned) templates. Use cookiecutter --list-installed."""
     config = get_user_config(passed_config_file, default_config)
     cookiecutter_folder = config.get('cookiecutters_dir')
     if not os.path.exists(cookiecutter_folder):
         click.echo(
-            'Error: Cannot list installed templates. Folder does not exist: '
-            '{}'.format(cookiecutter_folder)
+            f"Error: Cannot list installed templates. "
+            f"Folder does not exist: {cookiecutter_folder}"
         )
         sys.exit(-1)
 
     template_names = [
         folder
         for folder in os.listdir(cookiecutter_folder)
         if os.path.exists(
@@ -71,15 +70,17 @@
 @click.command(context_settings=dict(help_option_names=['-h', '--help']))
 @click.version_option(__version__, '-V', '--version', message=version_msg())
 @click.argument('template', required=False)
 @click.argument('extra_context', nargs=-1, callback=validate_extra_context)
 @click.option(
     '--no-input',
     is_flag=True,
-    help='Do not prompt for parameters and only use cookiecutter.json file content',
+    help='Do not prompt for parameters and only use cookiecutter.json file content. '
+    'Defaults to deleting any cached resources and redownloading them. '
+    'Cannot be combined with the --replay flag.',
 )
 @click.option(
     '-c',
     '--checkout',
     help='branch, tag or commit to checkout after git clone',
 )
 @click.option(
@@ -89,15 +90,16 @@
 )
 @click.option(
     '-v', '--verbose', is_flag=True, help='Print debug information', default=False
 )
 @click.option(
     '--replay',
     is_flag=True,
-    help='Do not prompt for parameters and only use information entered previously',
+    help='Do not prompt for parameters and only use information entered previously. '
+    'Cannot be combined with the --no-input flag or with extra configuration passed.',
 )
 @click.option(
     '--replay-file',
     type=click.Path(),
     default=None,
     help='Use this file for replay instead of the default.',
 )
@@ -140,14 +142,19 @@
     type=click.Choice(['yes', 'ask', 'no']),
     default='yes',
     help='Accept pre/post hooks',
 )
 @click.option(
     '-l', '--list-installed', is_flag=True, help='List currently installed templates.'
 )
+@click.option(
+    '--keep-project-on-failure',
+    is_flag=True,
+    help='Do not delete project folder on failure',
+)
 def main(
     template,
     extra_context,
     no_input,
     checkout,
     verbose,
     replay,
@@ -157,14 +164,15 @@
     default_config,
     debug_file,
     directory,
     skip_if_file_exists,
     accept_hooks,
     replay_file,
     list_installed,
+    keep_project_on_failure,
 ):
     """Create a project from a Cookiecutter project template (TEMPLATE).
 
     Cookiecutter is free and open source software, developed and managed by
     volunteers. If you would like to help out or fund the project, please get
     in touch at https://github.com/cookiecutter/cookiecutter.
     """
@@ -201,14 +209,15 @@
             output_dir=output_dir,
             config_file=config_file,
             default_config=default_config,
             password=os.environ.get('COOKIECUTTER_REPO_PASSWORD'),
             directory=directory,
             skip_if_file_exists=skip_if_file_exists,
             accept_hooks=_accept_hooks,
+            keep_project_on_failure=keep_project_on_failure,
         )
     except (
         ContextDecodingException,
         OutputDirExistsException,
         InvalidModeException,
         FailedHookException,
         UnknownExtension,
```

### Comparing `cookiecutter-2.1.1/cookiecutter/config.py` & `cookiecutter-2.2.0/cookiecutter/config.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.1.1/cookiecutter/environment.py` & `cookiecutter-2.2.0/cookiecutter/environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,23 +22,23 @@
         """
         context = kwargs.pop('context', {})
 
         default_extensions = [
             'cookiecutter.extensions.JsonifyExtension',
             'cookiecutter.extensions.RandomStringExtension',
             'cookiecutter.extensions.SlugifyExtension',
+            'cookiecutter.extensions.TimeExtension',
             'cookiecutter.extensions.UUIDExtension',
-            'jinja2_time.TimeExtension',
         ]
         extensions = default_extensions + self._read_extensions(context)
 
         try:
             super().__init__(extensions=extensions, **kwargs)
         except ImportError as err:
-            raise UnknownExtension(f'Unable to load extension: {err}')
+            raise UnknownExtension(f'Unable to load extension: {err}') from err
 
     def _read_extensions(self, context):
         """Return list of extensions as str to be passed on to the Jinja2 env.
 
         If context does not contain the relevant info, return an empty
         list instead.
         """
```

### Comparing `cookiecutter-2.1.1/cookiecutter/exceptions.py` & `cookiecutter-2.2.0/cookiecutter/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
             f"Error message: {self.error.message}. "
             f"Context: {self.context}"
         )
 
 
 class UnknownExtension(CookiecutterException):
     """
-    Exception for un-importable extention.
+    Exception for un-importable extension.
 
     Raised when an environment is unable to import a required extension.
     """
 
 
 class RepositoryNotFound(CookiecutterException):
     """
```

### Comparing `cookiecutter-2.1.1/cookiecutter/generate.py` & `cookiecutter-2.2.0/cookiecutter/generate.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import fnmatch
 import json
 import logging
 import os
 import shutil
 import warnings
 from collections import OrderedDict
-
+from pathlib import Path
 from binaryornot.check import is_binary
-from jinja2 import FileSystemLoader
+from jinja2 import FileSystemLoader, Environment
 from jinja2.exceptions import TemplateSyntaxError, UndefinedError
 
 from cookiecutter.environment import StrictEnvironment
 from cookiecutter.exceptions import (
     ContextDecodingException,
     FailedHookException,
     NonTemplatedInputDirException,
@@ -61,17 +61,21 @@
                 # This overwrite is actually valid for the given context
                 # Let's set it as default (by definition first item in list)
                 # see ``cookiecutter.prompt.prompt_choice_for_config``
                 context_value.remove(overwrite)
                 context_value.insert(0, overwrite)
             else:
                 raise ValueError(
-                    "{} provided for choice variable {}, but the "
-                    "choices are {}.".format(overwrite, variable, context_value)
+                    f"{overwrite} provided for choice variable {variable}, "
+                    f"but the choices are {context_value}."
                 )
+        elif isinstance(context_value, dict) and isinstance(overwrite, dict):
+            # Partially overwrite some keys in original dict
+            apply_overwrites_to_context(context_value, overwrite)
+            context[variable] = context_value
         else:
             # Simply overwrite the value for this variable
             context[variable] = overwrite
 
 
 def generate_context(
     context_file='cookiecutter.json', default_context=None, extra_context=None
@@ -92,31 +96,31 @@
             obj = json.load(file_handle, object_pairs_hook=OrderedDict)
     except ValueError as e:
         # JSON decoding error.  Let's throw a new exception that is more
         # friendly for the developer or user.
         full_fpath = os.path.abspath(context_file)
         json_exc_message = str(e)
         our_exc_message = (
-            'JSON decoding error while loading "{}".  Decoding'
-            ' error details: "{}"'.format(full_fpath, json_exc_message)
+            f"JSON decoding error while loading '{full_fpath}'. "
+            f"Decoding error details: '{json_exc_message}'"
         )
-        raise ContextDecodingException(our_exc_message)
+        raise ContextDecodingException(our_exc_message) from e
 
     # Add the Python object to the context dictionary
     file_name = os.path.split(context_file)[1]
     file_stem = file_name.split('.')[0]
     context[file_stem] = obj
 
     # Overwrite context variable defaults with the default context from the
     # user's global config, if available
     if default_context:
         try:
             apply_overwrites_to_context(obj, default_context)
-        except ValueError as ex:
-            warnings.warn("Invalid default received: " + str(ex))
+        except ValueError as error:
+            warnings.warn(f"Invalid default received: {error}")
     if extra_context:
         apply_overwrites_to_context(obj, extra_context)
 
     logger.debug('Context generated is %s', context)
     return context
 
 
@@ -159,63 +163,69 @@
     logger.debug('Created file at %s', outfile)
 
     # Just copy over binary files. Don't render.
     logger.debug("Check %s to see if it's a binary", infile)
     if is_binary(infile):
         logger.debug('Copying binary %s to %s without rendering', infile, outfile)
         shutil.copyfile(infile, outfile)
-    else:
-        # Force fwd slashes on Windows for get_template
-        # This is a by-design Jinja issue
-        infile_fwd_slashes = infile.replace(os.path.sep, '/')
+        shutil.copymode(infile, outfile)
+        return
 
-        # Render the file
-        try:
-            tmpl = env.get_template(infile_fwd_slashes)
-        except TemplateSyntaxError as exception:
-            # Disable translated so that printed exception contains verbose
-            # information about syntax error location
-            exception.translated = False
-            raise
-        rendered_file = tmpl.render(**context)
+    # Force fwd slashes on Windows for get_template
+    # This is a by-design Jinja issue
+    infile_fwd_slashes = infile.replace(os.path.sep, '/')
 
-        # Detect original file newline to output the rendered file
-        # note: newline='' ensures newlines are not converted
-        with open(infile, encoding='utf-8', newline='') as rd:
-            rd.readline()  # Read the first line to load 'newlines' value
-
-            # Use `_new_lines` overwrite from context, if configured.
-            newline = rd.newlines
-            if context['cookiecutter'].get('_new_lines', False):
-                newline = context['cookiecutter']['_new_lines']
-                logger.debug('Overwriting end line character with %s', newline)
+    # Render the file
+    try:
+        tmpl = env.get_template(infile_fwd_slashes)
+    except TemplateSyntaxError as exception:
+        # Disable translated so that printed exception contains verbose
+        # information about syntax error location
+        exception.translated = False
+        raise
+    rendered_file = tmpl.render(**context)
+
+    if context['cookiecutter'].get('_new_lines', False):
+        # Use `_new_lines` from context, if configured.
+        newline = context['cookiecutter']['_new_lines']
+        logger.debug('Using configured newline character %s', repr(newline))
+    else:
+        # Detect original file newline to output the rendered file.
+        with open(infile, encoding='utf-8') as rd:
+            rd.readline()  # Read only the first line to load a 'newlines' value.
+        newline = rd.newlines
+        logger.debug('Using detected newline character %s', repr(newline))
 
-        logger.debug('Writing contents to file %s', outfile)
+    logger.debug('Writing contents to file %s', outfile)
 
-        with open(outfile, 'w', encoding='utf-8', newline=newline) as fh:
-            fh.write(rendered_file)
+    with open(outfile, 'w', encoding='utf-8', newline=newline) as fh:
+        fh.write(rendered_file)
 
     # Apply file permissions to output file
     shutil.copymode(infile, outfile)
 
 
 def render_and_create_dir(
-    dirname, context, output_dir, environment, overwrite_if_exists=False
+    dirname: str,
+    context: dict,
+    output_dir: "os.PathLike[str]",
+    environment: Environment,
+    overwrite_if_exists: bool = False,
 ):
     """Render name of a directory, create the directory, return its path."""
     name_tmpl = environment.from_string(dirname)
     rendered_dirname = name_tmpl.render(**context)
 
-    dir_to_create = os.path.normpath(os.path.join(output_dir, rendered_dirname))
+    dir_to_create = Path(output_dir, rendered_dirname)
 
     logger.debug(
         'Rendered dir %s must exist in output_dir %s', dir_to_create, output_dir
     )
 
-    output_dir_exists = os.path.exists(dir_to_create)
+    output_dir_exists = dir_to_create.exists()
 
     if output_dir_exists:
         if overwrite_if_exists:
             logger.debug(
                 'Output directory %s already exists, overwriting it', dir_to_create
             )
         else:
@@ -246,15 +256,18 @@
     :param context: Cookiecutter project context.
     :param delete_project_on_failure: Delete the project directory on hook
         failure?
     """
     with work_in(repo_dir):
         try:
             run_hook(hook_name, project_dir, context)
-        except FailedHookException:
+        except (
+            FailedHookException,
+            UndefinedError,
+        ):
             if delete_project_on_failure:
                 rmtree(project_dir)
             logger.error(
                 "Stopping generation because %s hook "
                 "script didn't exit successfully",
                 hook_name,
             )
@@ -264,23 +277,28 @@
 def generate_files(
     repo_dir,
     context=None,
     output_dir='.',
     overwrite_if_exists=False,
     skip_if_file_exists=False,
     accept_hooks=True,
+    keep_project_on_failure=False,
 ):
     """Render the templates and saves them to files.
 
     :param repo_dir: Project template input directory.
     :param context: Dict for populating the template's variables.
     :param output_dir: Where to output the generated project dir into.
     :param overwrite_if_exists: Overwrite the contents of the output directory
         if it exists.
+    :param skip_if_file_exists: Skip the files in the corresponding directories
+        if they already exist
     :param accept_hooks: Accept pre and post hooks if set to `True`.
+    :param keep_project_on_failure: If `True` keep generated project directory even when
+        generation fails
     """
     template_dir = find_template(repo_dir)
     logger.debug('Generating project from %s...', template_dir)
     context = context or OrderedDict([])
 
     envvars = context.get('cookiecutter', {}).get('_jinja2_env_vars', {})
 
@@ -289,60 +307,67 @@
     env = StrictEnvironment(context=context, keep_trailing_newline=True, **envvars)
     try:
         project_dir, output_directory_created = render_and_create_dir(
             unrendered_dir, context, output_dir, env, overwrite_if_exists
         )
     except UndefinedError as err:
         msg = f"Unable to create project directory '{unrendered_dir}'"
-        raise UndefinedVariableInTemplate(msg, err, context)
+        raise UndefinedVariableInTemplate(msg, err, context) from err
 
     # We want the Jinja path and the OS paths to match. Consequently, we'll:
     #   + CD to the template folder
     #   + Set Jinja's path to '.'
     #
     #  In order to build our files to the correct folder(s), we'll use an
     # absolute path for the target folder (project_dir)
 
     project_dir = os.path.abspath(project_dir)
     logger.debug('Project directory is %s', project_dir)
 
     # if we created the output directory, then it's ok to remove it
     # if rendering fails
-    delete_project_on_failure = output_directory_created
+    delete_project_on_failure = output_directory_created and not keep_project_on_failure
 
     if accept_hooks:
         _run_hook_from_repo_dir(
             repo_dir, 'pre_gen_project', project_dir, context, delete_project_on_failure
         )
 
     with work_in(template_dir):
-        env.loader = FileSystemLoader('.')
+        env.loader = FileSystemLoader(['.', '../templates'])
 
         for root, dirs, files in os.walk('.'):
             # We must separate the two types of dirs into different lists.
             # The reason is that we don't want ``os.walk`` to go through the
             # unrendered directories, since they will just be copied.
             copy_dirs = []
             render_dirs = []
 
             for d in dirs:
                 d_ = os.path.normpath(os.path.join(root, d))
                 # We check the full path, because that's how it can be
                 # specified in the ``_copy_without_render`` setting, but
                 # we store just the dir name
                 if is_copy_only_path(d_, context):
+                    logger.debug('Found copy only path %s', d)
                     copy_dirs.append(d)
                 else:
                     render_dirs.append(d)
 
             for copy_dir in copy_dirs:
                 indir = os.path.normpath(os.path.join(root, copy_dir))
                 outdir = os.path.normpath(os.path.join(project_dir, indir))
                 outdir = env.from_string(outdir).render(**context)
                 logger.debug('Copying dir %s to %s without rendering', indir, outdir)
+
+                # The outdir is not the root dir, it is the dir which marked as copy
+                # only in the config file. If the program hits this line, which means
+                # the overwrite_if_exists = True, and root dir exists
+                if os.path.isdir(outdir):
+                    shutil.rmtree(outdir)
                 shutil.copytree(indir, outdir)
 
             # We mutate ``dirs``, because we only want to go through these dirs
             # recursively
             dirs[:] = render_dirs
             for d in dirs:
                 unrendered_dir = os.path.join(project_dir, root, d)
@@ -351,15 +376,15 @@
                         unrendered_dir, context, output_dir, env, overwrite_if_exists
                     )
                 except UndefinedError as err:
                     if delete_project_on_failure:
                         rmtree(project_dir)
                     _dir = os.path.relpath(unrendered_dir, output_dir)
                     msg = f"Unable to create directory '{_dir}'"
-                    raise UndefinedVariableInTemplate(msg, err, context)
+                    raise UndefinedVariableInTemplate(msg, err, context) from err
 
             for f in files:
                 infile = os.path.normpath(os.path.join(root, f))
                 if is_copy_only_path(infile, context):
                     outfile_tmpl = env.from_string(infile)
                     outfile_rendered = outfile_tmpl.render(**context)
                     outfile = os.path.join(project_dir, outfile_rendered)
@@ -373,15 +398,15 @@
                     generate_file(
                         project_dir, infile, context, env, skip_if_file_exists
                     )
                 except UndefinedError as err:
                     if delete_project_on_failure:
                         rmtree(project_dir)
                     msg = f"Unable to create file '{infile}'"
-                    raise UndefinedVariableInTemplate(msg, err, context)
+                    raise UndefinedVariableInTemplate(msg, err, context) from err
 
     if accept_hooks:
         _run_hook_from_repo_dir(
             repo_dir,
             'post_gen_project',
             project_dir,
             context,
```

### Comparing `cookiecutter-2.1.1/cookiecutter/hooks.py` & `cookiecutter-2.2.0/cookiecutter/hooks.py`

 * *Files 12% similar despite different names*

```diff
@@ -81,20 +81,20 @@
     try:
         proc = subprocess.Popen(script_command, shell=run_thru_shell, cwd=cwd)  # nosec
         exit_status = proc.wait()
         if exit_status != EXIT_SUCCESS:
             raise FailedHookException(
                 f'Hook script failed (exit status: {exit_status})'
             )
-    except OSError as os_error:
-        if os_error.errno == errno.ENOEXEC:
+    except OSError as err:
+        if err.errno == errno.ENOEXEC:
             raise FailedHookException(
                 'Hook script failed, might be an empty file or missing a shebang'
-            )
-        raise FailedHookException(f'Hook script failed (error: {os_error})')
+            ) from err
+        raise FailedHookException(f'Hook script failed (error: {err})') from err
 
 
 def run_script_with_context(script_path, cwd, context):
     """Execute a script after rendering it with Jinja.
 
     :param script_path: Absolute path to the script to run.
     :param cwd: The directory to run the script from.
```

### Comparing `cookiecutter-2.1.1/cookiecutter/log.py` & `cookiecutter-2.2.0/cookiecutter/log.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.1.1/cookiecutter/main.py` & `cookiecutter-2.2.0/cookiecutter/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 Main entry point for the `cookiecutter` command.
 
 The code in this module is also a good example of how to use Cookiecutter as a
 library rather than a script.
 """
-from copy import copy
 import logging
 import os
+import re
 import sys
+from copy import copy
 
 from cookiecutter.config import get_user_config
 from cookiecutter.exceptions import InvalidModeException
 from cookiecutter.generate import generate_context, generate_files
 from cookiecutter.prompt import prompt_for_config
 from cookiecutter.replay import dump, load
 from cookiecutter.repository import determine_repo_dir
@@ -30,33 +31,38 @@
     output_dir='.',
     config_file=None,
     default_config=False,
     password=None,
     directory=None,
     skip_if_file_exists=False,
     accept_hooks=True,
+    keep_project_on_failure=False,
 ):
     """
     Run Cookiecutter just as if using it from the command line.
 
     :param template: A directory containing a project template directory,
         or a URL to a git repository.
     :param checkout: The branch, tag or commit ID to checkout after clone.
-    :param no_input: Prompt the user at command line for manual configuration?
+    :param no_input: Do not prompt for user input.
+        Use default values for template parameters taken from `cookiecutter.json`, user
+        config and `extra_dict`. Force a refresh of cached resources.
     :param extra_context: A dictionary of context that overrides default
         and user configuration.
     :param replay: Do not prompt for input, instead read from saved json. If
         ``True`` read from the ``replay_dir``.
         if it exists
     :param output_dir: Where to output the generated project dir into.
     :param config_file: User configuration file path.
     :param default_config: Use default values rather than a config file.
     :param password: The password to use when extracting the repository.
     :param directory: Relative path to a cookiecutter template in a repository.
     :param accept_hooks: Accept pre and post hooks if set to `True`.
+    :param keep_project_on_failure: If `True` keep generated project directory even when
+        generation fails
     """
     if replay and ((no_input is not False) or (extra_context is not None)):
         err_msg = (
             "You can not use both replay and no_input or extra_context "
             "at the same time."
         )
         raise InvalidModeException(err_msg)
@@ -92,36 +98,64 @@
 
         context = generate_context(
             context_file=context_file,
             default_context=config_dict['default_context'],
             extra_context=extra_context,
         )
 
+        # preserve the original cookiecutter options
+        context['_cookiecutter'] = context['cookiecutter']
+
         # prompt the user to manually configure at the command line.
         # except when 'no-input' flag is set
         with import_patch:
             context['cookiecutter'] = prompt_for_config(context, no_input)
 
+        if "template" in context["cookiecutter"]:
+            nested_template = re.search(
+                r'\((.*?)\)', context["cookiecutter"]["template"]
+            ).group(1)
+            return cookiecutter(
+                template=os.path.join(template, nested_template),
+                checkout=checkout,
+                no_input=no_input,
+                extra_context=extra_context,
+                replay=replay,
+                overwrite_if_exists=overwrite_if_exists,
+                output_dir=output_dir,
+                config_file=config_file,
+                default_config=default_config,
+                password=password,
+                directory=directory,
+                skip_if_file_exists=skip_if_file_exists,
+                accept_hooks=accept_hooks,
+                keep_project_on_failure=keep_project_on_failure,
+            )
+
         # include template dir or url in the context dict
         context['cookiecutter']['_template'] = template
 
+        # include repo dir or url in the context dict
+        context['cookiecutter']['_repo_dir'] = repo_dir
+
         # include output+dir in the context dict
         context['cookiecutter']['_output_dir'] = os.path.abspath(output_dir)
 
         dump(config_dict['replay_dir'], template_name, context)
 
     # Create project from local context and project template.
     with import_patch:
         result = generate_files(
             repo_dir=repo_dir,
             context=context,
             overwrite_if_exists=overwrite_if_exists,
             skip_if_file_exists=skip_if_file_exists,
             output_dir=output_dir,
             accept_hooks=accept_hooks,
+            keep_project_on_failure=keep_project_on_failure,
         )
 
     # Cleanup (if required)
     if cleanup:
         rmtree(repo_dir)
 
     return result
```

### Comparing `cookiecutter-2.1.1/cookiecutter/prompt.py` & `cookiecutter-2.2.0/cookiecutter/prompt.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,72 +6,89 @@
 import click
 from jinja2.exceptions import UndefinedError
 
 from cookiecutter.environment import StrictEnvironment
 from cookiecutter.exceptions import UndefinedVariableInTemplate
 
 
-def read_user_variable(var_name, default_value):
+def read_user_variable(var_name, default_value, prompts=None):
     """Prompt user for variable and return the entered value or given default.
 
     :param str var_name: Variable of the context to query the user
     :param default_value: Value that will be returned if no input happens
     """
-    # Please see https://click.palletsprojects.com/en/7.x/api/#click.prompt
-    return click.prompt(var_name, default=default_value)
+    question = (
+        prompts[var_name]
+        if prompts and var_name in prompts.keys() and prompts[var_name]
+        else var_name
+    )
+    return click.prompt(question, default=default_value)
 
 
-def read_user_yes_no(question, default_value):
+def read_user_yes_no(var_name, default_value, prompts=None):
     """Prompt the user to reply with 'yes' or 'no' (or equivalent values).
 
-    Note:
-      Possible choices are 'true', '1', 'yes', 'y' or 'false', '0', 'no', 'n'
+    - These input values will be converted to ``True``:
+      "1", "true", "t", "yes", "y", "on"
+    - These input values will be converted to ``False``:
+      "0", "false", "f", "no", "n", "off"
+
+    Actual parsing done by :func:`click.prompt`; Check this function codebase change in
+    case of unexpected behaviour.
 
     :param str question: Question to the user
     :param default_value: Value that will be returned if no input happens
     """
-    # Please see https://click.palletsprojects.com/en/7.x/api/#click.prompt
+    question = (
+        prompts[var_name]
+        if prompts and var_name in prompts.keys() and prompts[var_name]
+        else var_name
+    )
     return click.prompt(question, default=default_value, type=click.BOOL)
 
 
 def read_repo_password(question):
     """Prompt the user to enter a password.
 
     :param str question: Question to the user
     """
-    # Please see https://click.palletsprojects.com/en/7.x/api/#click.prompt
     return click.prompt(question, hide_input=True)
 
 
-def read_user_choice(var_name, options):
+def read_user_choice(var_name, options, prompts=None):
     """Prompt the user to choose from several options for the given variable.
 
     The first item will be returned if no input happens.
 
     :param str var_name: Variable as specified in the context
     :param list options: Sequence of options that are available to select from
     :return: Exactly one item of ``options`` that has been chosen by the user
     """
-    # Please see https://click.palletsprojects.com/en/7.x/api/#click.prompt
     if not isinstance(options, list):
         raise TypeError
 
     if not options:
         raise ValueError
 
     choice_map = OrderedDict((f'{i}', value) for i, value in enumerate(options, 1))
     choices = choice_map.keys()
     default = '1'
 
+    question = (
+        prompts[var_name]
+        if prompts and var_name in prompts.keys() and prompts[var_name]
+        else f"Select {var_name}"
+    )
+
     choice_lines = ['{} - {}'.format(*c) for c in choice_map.items()]
     prompt = '\n'.join(
         (
-            f'Select {var_name}:',
-            '\n'.join(choice_lines),
-            'Choose from {}'.format(', '.join(choices)),
+            f"{question}:",
+            "\n".join(choice_lines),
+            f"Choose from {', '.join(choices)}",
         )
     )
 
     user_choice = click.prompt(
         prompt, type=click.Choice(choices), default=default, show_choices=False
     )
     return choice_map[user_choice]
@@ -87,38 +104,42 @@
     """
     if user_value == DEFAULT_DISPLAY:
         # Return the given default w/o any processing
         return default_value
 
     try:
         user_dict = json.loads(user_value, object_pairs_hook=OrderedDict)
-    except Exception:
+    except Exception as error:
         # Leave it up to click to ask the user again
-        raise click.UsageError('Unable to decode to JSON.')
+        raise click.UsageError('Unable to decode to JSON.') from error
 
     if not isinstance(user_dict, dict):
         # Leave it up to click to ask the user again
         raise click.UsageError('Requires JSON dict.')
 
     return user_dict
 
 
-def read_user_dict(var_name, default_value):
+def read_user_dict(var_name, default_value, prompts=None):
     """Prompt the user to provide a dictionary of data.
 
     :param str var_name: Variable as specified in the context
     :param default_value: Value that will be returned if no input is provided
     :return: A Python dictionary to use in the context.
     """
-    # Please see https://click.palletsprojects.com/en/7.x/api/#click.prompt
     if not isinstance(default_value, dict):
         raise TypeError
 
+    question = (
+        prompts[var_name]
+        if prompts and var_name in prompts.keys() and prompts[var_name]
+        else var_name
+    )
     user_value = click.prompt(
-        var_name,
+        question,
         default=DEFAULT_DISPLAY,
         type=click.STRING,
         value_proc=functools.partial(process_json, default_value=default_value),
     )
 
     if click.__version__.startswith("7.") and user_value == DEFAULT_DISPLAY:
         # click 7.x does not invoke value_proc on the default value.
@@ -139,55 +160,60 @@
 
     :param Environment env: A Jinja2 Environment object.
     :param raw: The next value to be prompted for by the user.
     :param dict cookiecutter_dict: The current context as it's gradually
         being populated with variables.
     :return: The rendered value for the default variable.
     """
-    if raw is None:
-        return None
+    if raw is None or isinstance(raw, bool):
+        return raw
     elif isinstance(raw, dict):
         return {
             render_variable(env, k, cookiecutter_dict): render_variable(
                 env, v, cookiecutter_dict
             )
             for k, v in raw.items()
         }
     elif isinstance(raw, list):
         return [render_variable(env, v, cookiecutter_dict) for v in raw]
     elif not isinstance(raw, str):
         raw = str(raw)
 
     template = env.from_string(raw)
 
-    rendered_template = template.render(cookiecutter=cookiecutter_dict)
-    return rendered_template
+    return template.render(cookiecutter=cookiecutter_dict)
 
 
-def prompt_choice_for_config(cookiecutter_dict, env, key, options, no_input):
+def prompt_choice_for_config(
+    cookiecutter_dict, env, key, options, no_input, prompts=None
+):
     """Prompt user with a set of options to choose from.
 
-    Each of the possible choices is rendered beforehand.
+    :param no_input: Do not prompt for user input and return the first available option.
     """
     rendered_options = [render_variable(env, raw, cookiecutter_dict) for raw in options]
-
     if no_input:
         return rendered_options[0]
-    return read_user_choice(key, rendered_options)
+    return read_user_choice(key, rendered_options, prompts)
 
 
 def prompt_for_config(context, no_input=False):
     """Prompt user to enter a new config.
 
     :param dict context: Source for field names and sample values.
-    :param no_input: Prompt the user at command line for manual configuration?
+    :param no_input: Do not prompt for user input and use only values from context.
     """
     cookiecutter_dict = OrderedDict([])
     env = StrictEnvironment(context=context)
 
+    prompts = {}
+    if '__prompts__' in context['cookiecutter'].keys():
+        prompts = context['cookiecutter']['__prompts__']
+        del context['cookiecutter']['__prompts__']
+
     # First pass: Handle simple and raw variables, plus choices.
     # These must be done first because the dictionaries keys and
     # values might refer to them.
     for key, raw in context['cookiecutter'].items():
         if key.startswith('_') and not key.startswith('__'):
             cookiecutter_dict[key] = raw
             continue
@@ -195,42 +221,50 @@
             cookiecutter_dict[key] = render_variable(env, raw, cookiecutter_dict)
             continue
 
         try:
             if isinstance(raw, list):
                 # We are dealing with a choice variable
                 val = prompt_choice_for_config(
-                    cookiecutter_dict, env, key, raw, no_input
+                    cookiecutter_dict, env, key, raw, no_input, prompts
                 )
                 cookiecutter_dict[key] = val
+            elif isinstance(raw, bool):
+                # We are dealing with a boolean variable
+                if no_input:
+                    cookiecutter_dict[key] = render_variable(
+                        env, raw, cookiecutter_dict
+                    )
+                else:
+                    cookiecutter_dict[key] = read_user_yes_no(key, raw)
             elif not isinstance(raw, dict):
                 # We are dealing with a regular variable
                 val = render_variable(env, raw, cookiecutter_dict)
 
                 if not no_input:
-                    val = read_user_variable(key, val)
+                    val = read_user_variable(key, val, prompts)
 
                 cookiecutter_dict[key] = val
         except UndefinedError as err:
             msg = f"Unable to render variable '{key}'"
-            raise UndefinedVariableInTemplate(msg, err, context)
+            raise UndefinedVariableInTemplate(msg, err, context) from err
 
     # Second pass; handle the dictionaries.
     for key, raw in context['cookiecutter'].items():
-        # Skip private type dicts not ot be rendered.
+        # Skip private type dicts not to be rendered.
         if key.startswith('_') and not key.startswith('__'):
             continue
 
         try:
             if isinstance(raw, dict):
                 # We are dealing with a dict variable
                 val = render_variable(env, raw, cookiecutter_dict)
 
                 if not no_input and not key.startswith('__'):
-                    val = read_user_dict(key, val)
+                    val = read_user_dict(key, val, prompts)
 
                 cookiecutter_dict[key] = val
         except UndefinedError as err:
             msg = f"Unable to render variable '{key}'"
-            raise UndefinedVariableInTemplate(msg, err, context)
+            raise UndefinedVariableInTemplate(msg, err, context) from err
 
     return cookiecutter_dict
```

### Comparing `cookiecutter-2.1.1/cookiecutter/replay.py` & `cookiecutter-2.2.0/cookiecutter/replay.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,18 +12,17 @@
 def get_file_name(replay_dir, template_name):
     """Get the name of file."""
     suffix = '.json' if not template_name.endswith('.json') else ''
     file_name = f'{template_name}{suffix}'
     return os.path.join(replay_dir, file_name)
 
 
-def dump(replay_dir, template_name, context):
+def dump(replay_dir: "os.PathLike[str]", template_name: str, context: dict):
     """Write json data to file."""
-    if not make_sure_path_exists(replay_dir):
-        raise OSError(f'Unable to create replay dir at {replay_dir}')
+    make_sure_path_exists(replay_dir)
 
     if not isinstance(template_name, str):
         raise TypeError('Template name is required to be of type str')
 
     if not isinstance(context, dict):
         raise TypeError('Context is required to be of type dict')
```

### Comparing `cookiecutter-2.1.1/cookiecutter/repository.py` & `cookiecutter-2.2.0/cookiecutter/repository.py`

 * *Files 7% similar despite different names*

```diff
@@ -78,19 +78,20 @@
 
     :param template: A directory containing a project template directory,
         or a URL to a git repository.
     :param abbreviations: A dictionary of repository abbreviation
         definitions.
     :param clone_to_dir: The directory to clone the repository into.
     :param checkout: The branch, tag or commit ID to checkout after clone.
-    :param no_input: Prompt the user at command line for manual configuration?
+    :param no_input: Do not prompt for user input and eventually force a refresh of
+        cached resources.
     :param password: The password to use when extracting the repository.
     :param directory: Directory within repo where cookiecutter.json lives.
     :return: A tuple containing the cookiecutter template directory, and
-        a boolean descriving whether that directory should be cleaned up
+        a boolean describing whether that directory should be cleaned up
         after the template has been instantiated.
     :raises: `RepositoryNotFound` if a repository directory could not be found.
     """
     template = expand_abbreviations(template, abbreviations)
 
     if is_zip_file(template):
         unzipped_dir = unzip(
```

### Comparing `cookiecutter-2.1.1/cookiecutter/utils.py` & `cookiecutter-2.2.0/cookiecutter/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Helper functions used throughout Cookiecutter."""
 import contextlib
-import errno
 import logging
 import os
 import shutil
 import stat
 import sys
+from pathlib import Path
 
-from cookiecutter.prompt import read_user_yes_no
 from jinja2.ext import Extension
 
+from cookiecutter.prompt import read_user_yes_no
+
 logger = logging.getLogger(__name__)
 
 
 def force_delete(func, path, exc_info):
     """Error handler for `shutil.rmtree()` equivalent to `rm -rf`.
 
     Usage: `shutil.rmtree(path, onerror=force_delete)`
@@ -27,27 +28,24 @@
     """Remove a directory and all its contents. Like rm -rf on Unix.
 
     :param path: A directory path.
     """
     shutil.rmtree(path, onerror=force_delete)
 
 
-def make_sure_path_exists(path):
+def make_sure_path_exists(path: "os.PathLike[str]") -> None:
     """Ensure that a directory exists.
 
-    :param path: A directory path.
+    :param path: A directory tree path for creation.
     """
-    logger.debug('Making sure path exists: %s', path)
+    logger.debug('Making sure path exists (creates tree if not exist): %s', path)
     try:
-        os.makedirs(path)
-        logger.debug('Created directory at: %s', path)
-    except OSError as exception:
-        if exception.errno != errno.EEXIST:
-            return False
-    return True
+        Path(path).mkdir(parents=True, exist_ok=True)
+    except OSError as error:
+        raise OSError(f'Unable to create directory at {path}') from error
 
 
 @contextlib.contextmanager
 def work_in(dirname=None):
     """Context manager version of os.chdir.
 
     When exited, returns to the working directory prior to entering.
@@ -82,16 +80,16 @@
     :return: True if the content was deleted
     """
     # Suppress prompt if called via API
     if no_input:
         ok_to_delete = True
     else:
         question = (
-            "You've downloaded {} before. Is it okay to delete and re-download it?"
-        ).format(path)
+            f"You've downloaded {path} before. Is it okay to delete and re-download it?"
+        )
 
         ok_to_delete = read_user_yes_no(question, 'yes')
 
     if ok_to_delete:
         if os.path.isdir(path):
             rmtree(path)
         else:
```

### Comparing `cookiecutter-2.1.1/cookiecutter/vcs.py` & `cookiecutter-2.2.0/cookiecutter/vcs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Helper functions for working with version control systems."""
 import logging
 import os
 import subprocess  # nosec
+from pathlib import Path
 from shutil import which
+from typing import Optional
 
 from cookiecutter.exceptions import (
     RepositoryCloneFailed,
     RepositoryNotFound,
     UnknownRepoType,
     VCSNotInstalled,
 )
@@ -50,26 +52,32 @@
     Check if the version control system for a repo type is installed.
 
     :param repo_type:
     """
     return bool(which(repo_type))
 
 
-def clone(repo_url, checkout=None, clone_to_dir='.', no_input=False):
+def clone(
+    repo_url: str,
+    checkout: Optional[str] = None,
+    clone_to_dir: "os.PathLike[str]" = ".",
+    no_input: bool = False,
+):
     """Clone a repo to the current directory.
 
     :param repo_url: Repo URL of unknown type.
     :param checkout: The branch, tag or commit ID to checkout after clone.
     :param clone_to_dir: The directory to clone to.
                          Defaults to the current directory.
-    :param no_input: Suppress all user prompts when calling via API.
+    :param no_input: Do not prompt for user input and eventually force a refresh of
+        cached resources.
     :returns: str with path to the new directory of the repository.
     """
     # Ensure that clone_to_dir exists
-    clone_to_dir = os.path.expanduser(clone_to_dir)
+    clone_to_dir = Path(clone_to_dir).expanduser()
     make_sure_path_exists(clone_to_dir)
 
     # identify the repo_type
     repo_type, repo_url = identify_repo(repo_url)
 
     # check that the appropriate VCS for the repo_type is installed
     if not is_vcs_installed(repo_type):
@@ -109,17 +117,17 @@
                 )
         except subprocess.CalledProcessError as clone_error:
             output = clone_error.output.decode('utf-8')
             if 'not found' in output.lower():
                 raise RepositoryNotFound(
                     f'The repository {repo_url} could not be found, '
                     'have you made a typo?'
-                )
+                ) from clone_error
             if any(error in output for error in BRANCH_ERRORS):
                 raise RepositoryCloneFailed(
                     f'The {checkout} branch of repository '
                     f'{repo_url} could not found, have you made a typo?'
-                )
+                ) from clone_error
             logger.error('git clone failed with error: %s', output)
             raise
 
     return repo_dir
```

### Comparing `cookiecutter-2.1.1/cookiecutter/zipfile.py` & `cookiecutter-2.2.0/cookiecutter/zipfile.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 """Utility functions for handling and fetching repo archives in zip format."""
 import os
 import tempfile
+from pathlib import Path
+from typing import Optional
 from zipfile import BadZipFile, ZipFile
 
 import requests
 
 from cookiecutter.exceptions import InvalidZipRepository
 from cookiecutter.prompt import read_repo_password
 from cookiecutter.utils import make_sure_path_exists, prompt_and_delete
 
 
-def unzip(zip_uri, is_url, clone_to_dir='.', no_input=False, password=None):
+def unzip(
+    zip_uri: str,
+    is_url: bool,
+    clone_to_dir: "os.PathLike[str]" = ".",
+    no_input: bool = False,
+    password: Optional[str] = None,
+):
     """Download and unpack a zipfile at a given URI.
 
     This will download the zipfile to the cookiecutter repository,
     and unpack into a temporary directory.
 
     :param zip_uri: The URI for the zipfile.
     :param is_url: Is the zip URI a URL or a file?
     :param clone_to_dir: The cookiecutter repository directory
         to put the archive into.
-    :param no_input: Suppress any prompts
+    :param no_input: Do not prompt for user input and eventually force a refresh of
+        cached resources.
     :param password: The password to use when unpacking the repository.
     """
     # Ensure that clone_to_dir exists
-    clone_to_dir = os.path.expanduser(clone_to_dir)
+    clone_to_dir = Path(clone_to_dir).expanduser()
     make_sure_path_exists(clone_to_dir)
 
     if is_url:
         # Build the name of the cached zipfile,
         # and prompt to delete if it already exists.
         identifier = zip_uri.rsplit('/', 1)[1]
         zip_path = os.path.join(clone_to_dir, identifier)
@@ -36,15 +45,15 @@
         if os.path.exists(zip_path):
             download = prompt_and_delete(zip_path, no_input=no_input)
         else:
             download = True
 
         if download:
             # (Re) download the zipfile
-            r = requests.get(zip_uri, stream=True)
+            r = requests.get(zip_uri, stream=True, timeout=100)
             with open(zip_path, 'wb') as f:
                 for chunk in r.iter_content(chunk_size=1024):
                     if chunk:  # filter out keep-alive new chunks
                         f.write(chunk)
     else:
         # Just use the local zipfile as-is.
         zip_path = os.path.abspath(zip_uri)
@@ -58,16 +67,15 @@
             raise InvalidZipRepository(f'Zip repository {zip_uri} is empty')
 
         # The first record in the zipfile should be the directory entry for
         # the archive. If it isn't a directory, there's a problem.
         first_filename = zip_file.namelist()[0]
         if not first_filename.endswith('/'):
             raise InvalidZipRepository(
-                'Zip repository {} does not include '
-                'a top-level directory'.format(zip_uri)
+                f"Zip repository {zip_uri} does not include a top-level directory"
             )
 
         # Construct the final target directory
         project_name = first_filename[:-1]
         unzip_base = tempfile.mkdtemp()
         unzip_path = os.path.join(unzip_base, project_name)
```

### Comparing `cookiecutter-2.1.1/cookiecutter.egg-info/PKG-INFO` & `cookiecutter-2.2.0/cookiecutter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,60 +1,71 @@
 Metadata-Version: 2.1
 Name: cookiecutter
-Version: 2.1.1
+Version: 2.2.0
 Summary: A command-line utility that creates projects from project templates, e.g. creating a Python package project from a Python package project template.
 Home-page: https://github.com/cookiecutter/cookiecutter
 Author: Audrey Feldroy
 Author-email: audreyr@gmail.com
 License: BSD
+Project-URL: Documentation, https://cookiecutter.readthedocs.io
+Project-URL: Issues, https://github.com/cookiecutter/cookiecutter/issues
+Project-URL: Discord, https://discord.gg/9BrxzPKuEW
 Keywords: cookiecutter,Python,projects,project templates,Jinja2,skeleton,scaffolding,project directory,package,packaging
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
-# Cookiecutter
+<h1 align="center">
+    <img alt="cookiecutter Logo" width="200px" src="https://raw.githubusercontent.com/cookiecutter/cookiecutter/3ac078356adf5a1a72042dfe72ebfa4a9cd5ef38/logo/cookiecutter_medium.png">
+</h1>
+
+<div align="center">
 
 [![pypi](https://img.shields.io/pypi/v/cookiecutter.svg)](https://pypi.org/project/cookiecutter/)
 [![python](https://img.shields.io/pypi/pyversions/cookiecutter.svg)](https://pypi.org/project/cookiecutter/)
-[![Build Status](https://github.com/cookiecutter/cookiecutter/actions/workflows/main.yml/badge.svg?branch=master)](https://github.com/cookiecutter/cookiecutter/actions)
+[![Build Status](https://github.com/cookiecutter/cookiecutter/actions/workflows/tests.yml/badge.svg?branch=master)](https://github.com/cookiecutter/cookiecutter/actions)
 [![codecov](https://codecov.io/gh/cookiecutter/cookiecutter/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/cookiecutter/cookiecutter?branch=master)
 [![discord](https://img.shields.io/badge/Discord-cookiecutter-5865F2?style=flat&logo=discord&logoColor=white)](https://discord.gg/9BrxzPKuEW)
 [![docs](https://readthedocs.org/projects/cookiecutter/badge/?version=latest)](https://readthedocs.org/projects/cookiecutter/?badge=latest)
 [![Code Quality](https://img.shields.io/scrutinizer/g/cookiecutter/cookiecutter.svg)](https://scrutinizer-ci.com/g/cookiecutter/cookiecutter/?branch=master)
 
+</div>
+
+# cookiecutter
+
 A command-line utility that creates projects from **cookiecutters** (project templates), e.g. creating a Python package project from a Python package project template.
 
 - Documentation: [https://cookiecutter.readthedocs.io](https://cookiecutter.readthedocs.io)
 - GitHub: [https://github.com/cookiecutter/cookiecutter](https://github.com/cookiecutter/cookiecutter)
 - PyPI: [https://pypi.org/project/cookiecutter/](https://pypi.org/project/cookiecutter/)
-- Free and open source software: [BSD license](https://github.com/cookiecutter/cookiecutter/blob/master/LICENSE)
+- Free and open source software: [BSD license](https://github.com/cookiecutter/cookiecutter/blob/main/LICENSE)
 
-![Cookiecutter](https://raw.githubusercontent.com/cookiecutter/cookiecutter/3ac078356adf5a1a72042dfe72ebfa4a9cd5ef38/logo/cookiecutter_medium.png)
 
 ## Features
 
 - Cross-platform: Windows, Mac, and Linux are officially supported.
 - You don't have to know/write Python code to use Cookiecutter.
-- Works with Python 3.7, 3.8, 3.9., 3.10
+- Works with Python 3.7, 3.8, 3.9, 3.10, 3.11
 - Project templates can be in any programming language or markup format:
   Python, JavaScript, Ruby, CoffeeScript, RST, Markdown, CSS, HTML, you name it.
   You can use multiple languages in the same project template.
 
 ### For users of existing templates
 
 - Simple command line usage:
@@ -109,88 +120,92 @@
   ```bash
   # Clone cookiecutter-pypackage
   $ cookiecutter gh:audreyfeldroy/cookiecutter-pypackage
   # Now you can use the already cloned cookiecutter by name
   $ cookiecutter cookiecutter-pypackage
   ```
 
-- You can use local cookiecutters, or remote cookiecutters directly from Git repos or from Mercurial repos on Bitbucket.
-- Default context: specify key/value pairs that you want used as defaults  whenever you generate a project.
+- You can use local cookiecutters, or remote cookiecutters directly from Git repos or Mercurial repos on Bitbucket.
+- Default context: specify key/value pairs that you want to be used as defaults whenever you generate a project.
 - Inject extra context with command-line arguments:
 
   ```bash
   cookiecutter --no-input gh:msabramo/cookiecutter-supervisor program_name=foobar startsecs=10
   ```
 
-- Direct access to the Cookiecutter API allows for injection of extra context.
+- Direct access to the Cookiecutter API allows for the injection of extra context.
 - Paths to local projects can be specified as absolute or relative.
-- Projects generated to your current directory or to target directory if specified with `-o` option.
+Projects are generated to your current directory or to the target directory if specified with `-o` option.
 
 ### For template creators
 
 - Supports unlimited levels of directory nesting.
 - 100% of templating is done with Jinja2.
 - Both, directory names and filenames can be templated.
   For example:
 
   ```py
   {{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}.py
   ```
-- Simply define your template variables in a `cookiecutter.json` file.
+- Simply define your template variables in a `cookiecutter.json` file. You can also add human-readable questions that will be prompted to the user for each variable using the `__prompts__` key.
   For example:
 
   ```json
   {
     "full_name": "Audrey Roy Greenfeld",
     "email": "audreyr@gmail.com",
     "project_name": "Complexity",
     "repo_name": "complexity",
     "project_short_description": "Refreshingly simple static site generator.",
     "release_date": "2013-07-10",
     "year": "2013",
-    "version": "0.1.1"
+    "version": "0.1.1",
+    "__prompts__": {
+      "full_name": "Provide your full name",
+      "email": "Provide your email"
+    }
   }
   ```
 - Pre- and post-generate hooks: Python or shell scripts to run before or after generating a project.
 
 ## Available Cookiecutters
 
 Making great cookies takes a lot of cookiecutters and contributors.
 We're so pleased that there are many Cookiecutter project templates to choose from.
 We hope you find a cookiecutter that is just right for your needs.
 
 ### A Pantry Full of Cookiecutters
 
-The best place to start searching for specific and ready to use cookiecutter template is [Github search](https://github.com/search?q=cookiecutter&type=Repositories).
+The best place to start searching for specific and ready-to-use cookiecutter templates is [Github search](https://github.com/search?q=cookiecutter&type=Repositories).
 Just type `cookiecutter` and you will discover over 4000 related repositories.
 
-We also recommend you to check related GitHub topics.
+We also recommend you check related GitHub topics.
 For general search use [cookiecutter-template](https://github.com/topics/cookiecutter-template).
 For specific topics try to use `cookiecutter-yourtopic`, like `cookiecutter-python` or `cookiecutter-datascience`.
 This is a new GitHub feature, so not all active repositories use it at the moment.
 
-If you are template developer please add related [topics](https://help.github.com/en/github/administering-a-repository/classifying-your-repository-with-topics) with `cookiecutter` prefix to you repository.
+If you are a template developer please add related [topics](https://help.github.com/en/github/administering-a-repository/classifying-your-repository-with-topics) with `cookiecutter` prefix to your repository.
 We believe it will make it more discoverable.
-You are almost not limited in topics amount, use it!
+You are almost not limited in topic amount, use it!
 
 ### Cookiecutter Specials
 
 These Cookiecutters are maintained by the cookiecutter team:
 
 - [cookiecutter-pypackage](https://github.com/audreyfeldroy/cookiecutter-pypackage):
   ultimate Python package project template by [@audreyfeldroy's](https://github.com/audreyfeldroy).
 - [cookiecutter-django](https://github.com/pydanny/cookiecutter-django):
   a framework for jumpstarting production-ready Django projects quickly.
-  It is bleeding edge with Bootstrap 5, customizable users app, starter templates, working user registration, celery setup, and much more.
+  It is bleeding edge with Bootstrap 5, a customizable users app, starter templates, working user registration, celery setup, and much more.
 - [cookiecutter-pytest-plugin](https://github.com/pytest-dev/cookiecutter-pytest-plugin):
   Minimal Cookiecutter template for authoring [pytest](https://docs.pytest.org/) plugins that help you to write better programs.
 
 ## Community
 
-The core committer team can be found in [authors section](AUTHORS.md).
+The core committer team can be found in the [authors' section](AUTHORS.md).
 We are always welcome and invite you to participate.
 
 Stuck? Try one of the following:
 
 - See the [Troubleshooting](https://cookiecutter.readthedocs.io/en/latest/troubleshooting.html) page.
 - Ask for help on [Stack Overflow](https://stackoverflow.com/questions/tagged/cookiecutter).
 - You are strongly encouraged to [file an issue](https://github.com/cookiecutter/cookiecutter/issues?q=is%3Aopen) about the problem.
@@ -236,14 +251,14 @@
 
 This project is run by volunteers.
 Shortly we will be providing means for organizations and individuals to support the project.
 
 ## Code of Conduct
 
 Everyone interacting in the Cookiecutter project's codebases and documentation is expected to follow the [PyPA Code of Conduct](https://www.pypa.io/en/latest/code-of-conduct/).
-This includes, but is not limited to, issue trackers, chat rooms, mailing lists, and other virtual or in real life communication.
+This includes but is not limited to, issue trackers, chat rooms, mailing lists, and other virtual or in real-life communication.
 
 ## Creator / Leader
 
-This project was created and is led by [Audrey Roy Greenfeld](https://github.com/audreyfeldroy).
+This project was created and led by [Audrey Roy Greenfeld](https://github.com/audreyfeldroy).
 
 She is supported by a team of maintainers.
```

### Comparing `cookiecutter-2.1.1/cookiecutter.egg-info/SOURCES.txt` & `cookiecutter-2.2.0/cookiecutter.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -36,21 +36,23 @@
 tests/__init__.py
 tests/conftest.py
 tests/test_abort_generate_on_hook_error.py
 tests/test_cli.py
 tests/test_cookiecutter_invocation.py
 tests/test_cookiecutter_local_no_input.py
 tests/test_cookiecutter_local_with_input.py
+tests/test_cookiecutter_nested_templates.py
 tests/test_custom_extensions_in_hooks.py
 tests/test_default_extensions.py
 tests/test_environment.py
 tests/test_exceptions.py
 tests/test_find.py
 tests/test_generate_context.py
 tests/test_generate_copy_without_render.py
+tests/test_generate_copy_without_render_override.py
 tests/test_generate_file.py
 tests/test_generate_files.py
 tests/test_generate_hooks.py
 tests/test_get_config.py
 tests/test_get_user_config.py
 tests/test_hooks.py
 tests/test_log.py
@@ -61,29 +63,35 @@
 tests/test_read_repo_password.py
 tests/test_read_user_choice.py
 tests/test_read_user_dict.py
 tests/test_read_user_variable.py
 tests/test_read_user_yes_no.py
 tests/test_repo_not_found.py
 tests/test_specify_output_dir.py
+tests/test_templates.py
+tests/test_time_extension.py
 tests/test_utils.py
+tests/fake-nested-templates/cookiecutter.json
+tests/fake-nested-templates/fake-project/cookiecutter.json
 tests/fake-repo/cookiecutter.json
 tests/fake-repo-bad/no-project-in-here.txt
 tests/fake-repo-bad-json/cookiecutter.json
 tests/fake-repo-bad-json/{{cookiecutter.repo_name}}/README.rst
 tests/fake-repo-dict/cookiecutter.json
 tests/fake-repo-dict/{{cookiecutter.project_slug}}/README.md
 tests/fake-repo-dir/my-dir/cookiecutter.json
 tests/fake-repo-dir/my-dir/{{cookiecutter.repo_name}}/README.rst
 tests/fake-repo-pre/cookiecutter.json
 tests/fake-repo-pre/{{cookiecutter.repo_name}}/README.rst
 tests/fake-repo-pre2/cookiecutter.json
 tests/fake-repo-pre2/whatever.some.thing
 tests/fake-repo-pre2/{{cookiecutter.repo_name}}/README.rst
 tests/fake-repo-tmpl/cookiecutter.json
+tests/fake-repo-tmpl-_cookiecutter/cookiecutter.json
+tests/fake-repo-tmpl-_cookiecutter/{{cookiecutter.repo_name}}/README.rst
 tests/fake-repo-tmpl/{{cookiecutter.repo_name}}/README.rst
 tests/fake-repo/fake-project/README.rst
 tests/files/bad-zip-file.zip
 tests/files/empty.zip
 tests/files/fake-repo-tmpl.zip
 tests/files/not-a-repo.zip
 tests/files/protected-fake-repo-tmpl.zip
@@ -138,16 +146,24 @@
 tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/.DS_Store
 tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/logo.png
 tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/readme.txt
 tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/some_font.otf
 tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/logo.png
 tests/test-generate-context/choices_template.json
 tests/test-generate-context/invalid-syntax.json
+tests/test-generate-context/nested_dict.json
 tests/test-generate-context/non_ascii.json
 tests/test-generate-context/test.json
+tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/README.rst
+tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/README.txt
+tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/rendered/not_rendered.yml
+tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-not-rendered/README.rst
+tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.md
+tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.rst
+tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.txt
 tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/README.rst
 tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/README.txt
 tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/rendered/not_rendered.yml
 tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-not-rendered/README.rst
 tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.md
 tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.rst
 tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.txt
@@ -180,14 +196,30 @@
 tests/test-shellhooks-empty/input{{cookiecutter.shellhooks}}/README.rst
 tests/test-shellhooks-win/hooks/post_gen_project.bat
 tests/test-shellhooks-win/hooks/pre_gen_project.bat
 tests/test-shellhooks-win/input{{cookiecutter.shellhooks}}/README.rst
 tests/test-shellhooks/hooks/post_gen_project.sh
 tests/test-shellhooks/hooks/pre_gen_project.sh
 tests/test-shellhooks/input{{cookiecutter.shellhooks}}/README.rst
+tests/test-templates/extends/cookiecutter.json
+tests/test-templates/extends/templates/base-requirements.jinja
+tests/test-templates/extends/templates/click-requirements.jinja
+tests/test-templates/extends/templates/pytest-requirements.jinja
+tests/test-templates/extends/{{cookiecutter.project_slug}}/requirements.txt
+tests/test-templates/include/cookiecutter.json
+tests/test-templates/include/templates/click-requirements.jinja
+tests/test-templates/include/templates/pytest-requirements.jinja
+tests/test-templates/include/{{cookiecutter.project_slug}}/requirements.txt
+tests/test-templates/no-templates/cookiecutter.json
+tests/test-templates/no-templates/{{cookiecutter.project_slug}}/requirements.txt
+tests/test-templates/super/cookiecutter.json
+tests/test-templates/super/templates/base-requirements.jinja
+tests/test-templates/super/templates/click-requirements.jinja
+tests/test-templates/super/templates/pytest-requirements.jinja
+tests/test-templates/super/{{cookiecutter.project_slug}}/requirements.txt
 tests/undefined-variable/dir-name/{{cookiecutter.project_slug}}/README.rst
 tests/undefined-variable/dir-name/{{cookiecutter.project_slug}}/{{cookiecutter.foobar}}/helloworld.py
 tests/undefined-variable/file-content/{{cookiecutter.project_slug}}/README.rst
 tests/undefined-variable/file-name/cookiecutter.json
 tests/undefined-variable/file-name/{{cookiecutter.project_slug}}/{{cookiecutter.foobar}}
 tests/vcs/test_clone.py
 tests/vcs/test_identify_repo.py
```

### Comparing `cookiecutter-2.1.1/setup.py` & `cookiecutter-2.2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-#!/usr/bin/env python
 """cookiecutter distutils configuration."""
 from setuptools import setup
 
-version = "2.1.1"
+version = "2.2.0"
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 requirements = [
     'binaryornot>=0.4.4',
     'Jinja2>=2.7,<4.0.0',
     'click>=7.0,<9.0.0',
     'pyyaml>=5.3.1',
-    'jinja2-time>=0.2.0',
     'python-slugify>=4.0.0',
     'requests>=2.23.0',
+    'arrow',
 ]
 
 setup(
     name='cookiecutter',
     version=version,
     description=(
         'A command-line utility that creates projects from project '
@@ -26,14 +25,19 @@
         'Python package project template.'
     ),
     long_description=readme,
     long_description_content_type='text/markdown',
     author='Audrey Feldroy',
     author_email='audreyr@gmail.com',
     url='https://github.com/cookiecutter/cookiecutter',
+    project_urls={
+        "Documentation": "https://cookiecutter.readthedocs.io",
+        "Issues": "https://github.com/cookiecutter/cookiecutter/issues",
+        "Discord": "https://discord.gg/9BrxzPKuEW",
+    },
     packages=['cookiecutter'],
     package_dir={'cookiecutter': 'cookiecutter'},
     entry_points={'console_scripts': ['cookiecutter = cookiecutter.__main__:main']},
     include_package_data=True,
     python_requires='>=3.7',
     install_requires=requirements,
     license='BSD',
@@ -46,14 +50,15 @@
         "License :: OSI Approved :: BSD License",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Programming Language :: Python",
         "Topic :: Software Development",
     ],
     keywords=[
         "cookiecutter",
```

### Comparing `cookiecutter-2.1.1/tests/conftest.py` & `cookiecutter-2.2.0/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,14 @@
 from cookiecutter.config import DEFAULT_CONFIG
 
 
 USER_CONFIG = """
 cookiecutters_dir: '{cookiecutters_dir}'
 replay_dir: '{replay_dir}'
 """
-# In YAML, double quotes mean to use escape sequences.
-# Single quotes mean we will have unescaped backslahes.
-# http://blogs.perl.org/users/tinita/2018/03/
-# strings-in-yaml---to-quote-or-not-to-quote.html
 
 
 @pytest.fixture(autouse=True)
 def isolated_filesystem(monkeypatch, tmp_path):
     """Ensure filesystem isolation, set the user home to a tmp_path."""
     root_path = tmp_path.joinpath("home")
     root_path.mkdir()
@@ -34,30 +30,27 @@
 
 def backup_dir(original_dir, backup_dir):
     """Generate backup directory based on original directory."""
     # If the default original_dir is pre-existing, move it to a temp location
     if not os.path.isdir(original_dir):
         return False
 
-    # Remove existing backups before backing up. If they exist, they're stale.
+    # Remove existing stale backups before backing up.
     if os.path.isdir(backup_dir):
         utils.rmtree(backup_dir)
 
     shutil.copytree(original_dir, backup_dir)
     return True
 
 
 def restore_backup_dir(original_dir, backup_dir, original_dir_found):
     """Restore default contents."""
-    # Carefully delete the created original_dir only in certain
-    # conditions.
     original_dir_is_dir = os.path.isdir(original_dir)
     if original_dir_found:
-        # Delete the created original_dir as long as a backup
-        # exists
+        # Delete original_dir if a backup exists
         if original_dir_is_dir and os.path.isdir(backup_dir):
             utils.rmtree(original_dir)
     else:
         # Delete the created original_dir.
         # There's no backup because it never existed
         if original_dir_is_dir:
             utils.rmtree(original_dir)
```

### Comparing `cookiecutter-2.1.1/tests/files/fake-repo-tmpl.zip` & `cookiecutter-2.2.0/tests/files/fake-repo-tmpl.zip`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.1.1/tests/files/protected-fake-repo-tmpl.zip` & `cookiecutter-2.2.0/tests/files/protected-fake-repo-tmpl.zip`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.1.1/tests/replay/conftest.py` & `cookiecutter-2.2.0/tests/replay/conftest.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.1.1/tests/replay/test_dump.py` & `cookiecutter-2.2.0/tests/replay/test_dump.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,30 +53,32 @@
 @pytest.fixture
 def mock_ensure_failure(mocker):
     """Replace cookiecutter.replay.make_sure_path_exists function.
 
     Used to mock internal function and limit test scope.
     Always return expected value: False
     """
-    return mocker.patch('cookiecutter.replay.make_sure_path_exists', return_value=False)
+    return mocker.patch(
+        'cookiecutter.replay.make_sure_path_exists', side_effect=OSError
+    )
 
 
 @pytest.fixture
 def mock_ensure_success(mocker):
     """Replace cookiecutter.replay.make_sure_path_exists function.
 
     Used to mock internal function and limit test scope.
     Always return expected value: True
     """
     return mocker.patch('cookiecutter.replay.make_sure_path_exists', return_value=True)
 
 
 def test_ioerror_if_replay_dir_creation_fails(mock_ensure_failure, replay_test_dir):
     """Test that replay.dump raises when the replay_dir cannot be created."""
-    with pytest.raises(IOError):
+    with pytest.raises(OSError):
         replay.dump(replay_test_dir, 'foo', {'cookiecutter': {'hello': 'world'}})
 
     mock_ensure_failure.assert_called_once_with(replay_test_dir)
 
 
 def test_run_json_dump(
     mocker,
```

### Comparing `cookiecutter-2.1.1/tests/replay/test_load.py` & `cookiecutter-2.2.0/tests/replay/test_load.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.1.1/tests/replay/test_replay.py` & `cookiecutter-2.2.0/tests/replay/test_replay.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.1.1/tests/repository/test_abbreviation_expansion.py` & `cookiecutter-2.2.0/tests/repository/test_abbreviation_expansion.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.1.1/tests/repository/test_determine_repo_dir_clones_repo.py` & `cookiecutter-2.2.0/tests/repository/test_determine_repo_dir_clones_repo.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.1.1/tests/repository/test_determine_repo_dir_finds_existing_cookiecutter.py` & `cookiecutter-2.2.0/tests/repository/test_determine_repo_dir_finds_existing_cookiecutter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Tests around detection whether cookiecutter templates are cached locally."""
 import os
+from pathlib import Path
 
 import pytest
 
 from cookiecutter import repository
 
 
 @pytest.fixture
@@ -16,15 +17,15 @@
 def cloned_cookiecutter_path(user_config_data, template):
     """Fixture. Create fake project directory in special user folder."""
     cookiecutters_dir = user_config_data['cookiecutters_dir']
 
     cloned_template_path = os.path.join(cookiecutters_dir, template)
     os.mkdir(cloned_template_path)
 
-    open(os.path.join(cloned_template_path, 'cookiecutter.json'), 'w')
+    Path(cloned_template_path, "cookiecutter.json").touch()  # creates file
 
     return cloned_template_path
 
 
 def test_should_find_existing_cookiecutter(
     template, user_config_data, cloned_cookiecutter_path
 ):
```

### Comparing `cookiecutter-2.1.1/tests/repository/test_determine_repo_dir_finds_subdirectories.py` & `cookiecutter-2.2.0/tests/repository/test_determine_repo_dir_finds_subdirectories.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Tests around locally cached cookiecutter template repositories."""
 import os
+from pathlib import Path
 
 import pytest
 
 from cookiecutter import exceptions, repository
 
 
 @pytest.fixture
@@ -20,15 +21,15 @@
     cloned_template_path = os.path.join(cookiecutters_dir, template)
     if not os.path.exists(cloned_template_path):
         os.mkdir(cloned_template_path)  # might exist from other tests.
 
     subdir_template_path = os.path.join(cloned_template_path, 'my-dir')
     if not os.path.exists(subdir_template_path):
         os.mkdir(subdir_template_path)
-    open(os.path.join(subdir_template_path, 'cookiecutter.json'), 'w')
+    Path(subdir_template_path, 'cookiecutter.json').touch()  # creates file
 
     return subdir_template_path
 
 
 def test_should_find_existing_cookiecutter(
     template, user_config_data, cloned_cookiecutter_path
 ):
```

### Comparing `cookiecutter-2.1.1/tests/repository/test_determine_repository_should_use_local_repo.py` & `cookiecutter-2.2.0/tests/repository/test_determine_repository_should_use_local_repo.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.1.1/tests/repository/test_is_repo_url.py` & `cookiecutter-2.2.0/tests/repository/test_is_repo_url.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     """Verify is_repo_url works."""
     assert is_zip_file(zipfile) is True
 
 
 @pytest.fixture(
     params=[
         'gitolite@server:team/repo',
-        'git@github.com:audreyr/cookiecutter.git',
-        'https://github.com/audreyr/cookiecutter.git',
+        'git@github.com:audreyfeldroy/cookiecutter.git',
+        'https://github.com/cookiecutter/cookiecutter.git',
         'git+https://private.com/gitrepo',
         'hg+https://private.com/mercurialrepo',
         'https://bitbucket.org/pokoli/cookiecutter.hg',
         'file://server/path/to/repo.git',
     ]
 )
 def remote_repo_url(request):
@@ -61,15 +61,15 @@
 def test_is_repo_url_for_local_urls(local_repo_url):
     """Verify is_repo_url works."""
     assert is_repo_url(local_repo_url) is False
 
 
 def test_expand_abbreviations():
     """Validate `repository.expand_abbreviations` correctly translate url."""
-    template = 'gh:audreyr/cookiecutter-pypackage'
+    template = 'gh:audreyfeldroy/cookiecutter-pypackage'
 
     # This is not a valid repo url just yet!
     # First `repository.expand_abbreviations` needs to translate it
     assert is_repo_url(template) is False
 
     expanded_template = expand_abbreviations(template, BUILTIN_ABBREVIATIONS)
     assert is_repo_url(expanded_template) is True
```

### Comparing `cookiecutter-2.1.1/tests/repository/test_repository_has_cookiecutter_json.py` & `cookiecutter-2.2.0/tests/repository/test_repository_has_cookiecutter_json.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.1.1/tests/test-extensions/hello_extension/hello_extension.py` & `cookiecutter-2.2.0/tests/test-extensions/hello_extension/hello_extension.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.1.1/tests/test-extensions/local_extension/local_extensions/main.py` & `cookiecutter-2.2.0/tests/test-extensions/local_extension/local_extensions/main.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.1.1/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/.DS_Store` & `cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/.DS_Store`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.1.1/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/logo.png` & `cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/logo.png`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.1.1/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/some_font.otf` & `cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/some_font.otf`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.1.1/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/.DS_Store` & `cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/.DS_Store`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.1.1/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/logo.png` & `cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/logo.png`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.1.1/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/some_font.otf` & `cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/some_font.otf`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.1.1/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/logo.png` & `cookiecutter-2.2.0/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/logo.png`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.1.1/tests/test_abort_generate_on_hook_error.py` & `cookiecutter-2.2.0/tests/test_abort_generate_on_hook_error.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.1.1/tests/test_cli.py` & `cookiecutter-2.2.0/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Collection of tests around cookiecutter's command-line interface."""
-
 import json
 import os
 import re
-
+from pathlib import Path
 
 import pytest
 from click.testing import CliRunner
 
 from cookiecutter import utils
 from cookiecutter.__main__ import main
 from cookiecutter.environment import StrictEnvironment
@@ -68,26 +67,26 @@
 
 @pytest.mark.usefixtures('remove_fake_project_dir')
 def test_cli(cli_runner):
     """Test cli invocation work without flags if directory not exist."""
     result = cli_runner('tests/fake-repo-pre/', '--no-input')
     assert result.exit_code == 0
     assert os.path.isdir('fake-project')
-    with open(os.path.join('fake-project', 'README.rst')) as f:
-        assert 'Project name: **Fake Project**' in f.read()
+    content = Path("fake-project", "README.rst").read_text()
+    assert 'Project name: **Fake Project**' in content
 
 
 @pytest.mark.usefixtures('remove_fake_project_dir')
 def test_cli_verbose(cli_runner):
     """Test cli invocation display log if called with `verbose` flag."""
     result = cli_runner('tests/fake-repo-pre/', '--no-input', '-v')
     assert result.exit_code == 0
     assert os.path.isdir('fake-project')
-    with open(os.path.join('fake-project', 'README.rst')) as f:
-        assert 'Project name: **Fake Project**' in f.read()
+    content = Path("fake-project", "README.rst").read_text()
+    assert 'Project name: **Fake Project**' in content
 
 
 @pytest.mark.usefixtures('remove_fake_project_dir')
 def test_cli_replay(mocker, cli_runner):
     """Test cli invocation display log with `verbose` and `replay` flags."""
     mock_cookiecutter = mocker.patch('cookiecutter.cli.cookiecutter')
 
@@ -105,14 +104,15 @@
         output_dir='.',
         config_file=None,
         default_config=False,
         extra_context=None,
         password=None,
         directory=None,
         accept_hooks=True,
+        keep_project_on_failure=False,
     )
 
 
 @pytest.mark.usefixtures('remove_fake_project_dir')
 def test_cli_replay_file(mocker, cli_runner):
     """Test cli invocation correctly pass --replay-file option."""
     mock_cookiecutter = mocker.patch('cookiecutter.cli.cookiecutter')
@@ -131,14 +131,15 @@
         output_dir='.',
         config_file=None,
         default_config=False,
         extra_context=None,
         password=None,
         directory=None,
         accept_hooks=True,
+        keep_project_on_failure=False,
     )
 
 
 @pytest.mark.usefixtures('remove_fake_project_dir')
 def test_cli_exit_on_noinput_and_replay(mocker, cli_runner):
     """Test cli invocation fail if both `no-input` and `replay` flags passed."""
     mock_cookiecutter = mocker.patch(
@@ -166,14 +167,15 @@
         output_dir='.',
         config_file=None,
         default_config=False,
         extra_context=None,
         password=None,
         directory=None,
         accept_hooks=True,
+        keep_project_on_failure=False,
     )
 
 
 @pytest.fixture(params=['-f', '--overwrite-if-exists'])
 def overwrite_cli_flag(request):
     """Pytest fixture return all `overwrite-if-exists` invocation options."""
     return request.param
@@ -201,14 +203,15 @@
         output_dir='.',
         config_file=None,
         default_config=False,
         extra_context=None,
         password=None,
         directory=None,
         accept_hooks=True,
+        keep_project_on_failure=False,
     )
 
 
 @pytest.mark.usefixtures('remove_fake_project_dir')
 def test_cli_overwrite_if_exists_when_output_dir_does_not_exist(
     cli_runner, overwrite_cli_flag
 ):
@@ -257,14 +260,15 @@
         output_dir=output_dir,
         config_file=None,
         default_config=False,
         extra_context=None,
         password=None,
         directory=None,
         accept_hooks=True,
+        keep_project_on_failure=False,
     )
 
 
 @pytest.fixture(params=['-h', '--help', 'help'])
 def help_cli_flag(request):
     """Pytest fixture return all help invocation options."""
     return request.param
@@ -301,14 +305,15 @@
         output_dir='.',
         config_file=user_config_path,
         default_config=False,
         extra_context=None,
         password=None,
         directory=None,
         accept_hooks=True,
+        keep_project_on_failure=False,
     )
 
 
 def test_default_user_config_overwrite(mocker, cli_runner, user_config_path):
     """Test cli invocation ignores `config-file` if `default-config` passed."""
     mock_cookiecutter = mocker.patch('cookiecutter.cli.cookiecutter')
 
@@ -331,14 +336,15 @@
         output_dir='.',
         config_file=user_config_path,
         default_config=True,
         extra_context=None,
         password=None,
         directory=None,
         accept_hooks=True,
+        keep_project_on_failure=False,
     )
 
 
 def test_default_user_config(mocker, cli_runner):
     """Test cli invocation accepts `default-config` flag correctly."""
     mock_cookiecutter = mocker.patch('cookiecutter.cli.cookiecutter')
 
@@ -356,14 +362,15 @@
         output_dir='.',
         config_file=None,
         default_config=True,
         extra_context=None,
         password=None,
         directory=None,
         accept_hooks=True,
+        keep_project_on_failure=False,
     )
 
 
 def test_echo_undefined_variable_error(output_dir, cli_runner):
     """Cli invocation return error if variable undefined in template."""
     template_path = 'tests/undefined-variable/file-name/'
 
@@ -382,20 +389,25 @@
 
     message = (
         "Error message: 'collections.OrderedDict object' has no attribute 'foobar'"
     )
     assert message in result.output
 
     context = {
+        '_cookiecutter': {
+            'github_username': 'hackebrot',
+            'project_slug': 'testproject',
+        },
         'cookiecutter': {
             'github_username': 'hackebrot',
             'project_slug': 'testproject',
             '_template': template_path,
+            '_repo_dir': template_path,
             '_output_dir': output_dir,
-        }
+        },
     }
     context_str = json.dumps(context, indent=4, sort_keys=True)
     assert context_str in result.output
 
 
 def test_echo_unknown_extension_error(output_dir, cli_runner):
     """Cli return error if extension incorrectly defined in template."""
@@ -423,18 +435,17 @@
         '--no-input',
         '--default-config',
         '--output-dir',
         output_dir,
         template_path,
     )
     assert result.exit_code == 0
-    with open(os.path.join(output_dir, 'Foobar', 'HISTORY.rst')) as f:
-        data = f.read()
-        assert 'FoobarFoobar' in data
-        assert 'FOOBAR' in data
+    content = Path(output_dir, 'Foobar', 'HISTORY.rst').read_text()
+    assert 'FoobarFoobar' in content
+    assert 'FOOBAR' in content
 
 
 def test_local_extension_not_available(tmpdir, cli_runner):
     """Test handling of included but unavailable local extension."""
     context = {'cookiecutter': {'_extensions': ['foobar']}}
 
     with pytest.raises(UnknownExtension) as err:
@@ -450,16 +461,16 @@
         'tests/fake-repo-pre/',
         '--no-input',
         '-v',
         'project_name=Awesomez',
     )
     assert result.exit_code == 0
     assert os.path.isdir('fake-project')
-    with open(os.path.join('fake-project', 'README.rst')) as f:
-        assert 'Project name: **Awesomez**' in f.read()
+    content = Path('fake-project', 'README.rst').read_text()
+    assert 'Project name: **Awesomez**' in content
 
 
 @pytest.mark.usefixtures('remove_fake_project_dir')
 def test_cli_extra_context_invalid_format(cli_runner):
     """Cli invocation raise error if called with unknown argument."""
     result = cli_runner(
         'tests/fake-repo-pre/',
@@ -532,21 +543,17 @@
 
 
 @pytest.mark.usefixtures('make_fake_project_dir', 'remove_fake_project_dir')
 def test_debug_list_installed_templates(cli_runner, debug_file, user_config_path):
     """Verify --list-installed command correct invocation."""
     fake_template_dir = os.path.dirname(os.path.abspath('fake-project'))
     os.makedirs(os.path.dirname(user_config_path))
-    with open(user_config_path, 'w') as config_file:
-        # In YAML, double quotes mean to use escape sequences.
-        # Single quotes mean we will have unescaped backslahes.
-        # http://blogs.perl.org/users/tinita/2018/03/
-        # strings-in-yaml---to-quote-or-not-to-quote.html
-        config_file.write("cookiecutters_dir: '%s'" % fake_template_dir)
-    open(os.path.join('fake-project', 'cookiecutter.json'), 'w').write('{}')
+    # Single quotes in YAML will not parse escape codes (\).
+    Path(user_config_path).write_text(f"cookiecutters_dir: '{fake_template_dir}'")
+    Path("fake-project", "cookiecutter.json").write_text('{}')
 
     result = cli_runner(
         '--list-installed',
         '--config-file',
         user_config_path,
         str(debug_file),
     )
@@ -556,16 +563,15 @@
 
 
 def test_debug_list_installed_templates_failure(
     cli_runner, debug_file, user_config_path
 ):
     """Verify --list-installed command error on invocation."""
     os.makedirs(os.path.dirname(user_config_path))
-    with open(user_config_path, 'w') as config_file:
-        config_file.write('cookiecutters_dir: "/notarealplace/"')
+    Path(user_config_path).write_text('cookiecutters_dir: "/notarealplace/"')
 
     result = cli_runner(
         '--list-installed', '--config-file', user_config_path, str(debug_file)
     )
 
     assert "Error: Cannot list installed templates." in result.output
     assert result.exit_code == -1
@@ -578,16 +584,16 @@
         'tests/fake-repo-dir/',
         '--no-input',
         '-v',
         '--directory=my-dir',
     )
     assert result.exit_code == 0
     assert os.path.isdir("fake-project")
-    with open(os.path.join("fake-project", "README.rst")) as f:
-        assert "Project name: **Fake Project**" in f.read()
+    content = Path("fake-project", "README.rst").read_text()
+    assert "Project name: **Fake Project**" in content
 
 
 cli_accept_hook_arg_testdata = [
     ("--accept-hooks=yes", None, True),
     ("--accept-hooks=no", None, False),
     ("--accept-hooks=ask", "yes", True),
     ("--accept-hooks=ask", "no", False),
@@ -625,14 +631,15 @@
         config_file=None,
         default_config=False,
         extra_context=None,
         password=None,
         directory=None,
         skip_if_file_exists=False,
         accept_hooks=expected,
+        keep_project_on_failure=False,
     )
 
 
 @pytest.mark.usefixtures('remove_fake_project_dir')
 def test_cli_with_json_decoding_error(cli_runner):
     """Test cli invocation with a malformed JSON file."""
     template_path = 'tests/fake-repo-bad-json/'
```

### Comparing `cookiecutter-2.1.1/tests/test_cookiecutter_invocation.py` & `cookiecutter-2.2.0/tests/test_cookiecutter_invocation.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.1.1/tests/test_cookiecutter_local_no_input.py` & `cookiecutter-2.2.0/tests/test_cookiecutter_local_no_input.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Test cookiecutter for work without any input.
 
 Tests in this file execute `cookiecutter()` with `no_input=True` flag and
 verify result with different settings in `cookiecutter.json`.
 """
 import os
 import textwrap
+from pathlib import Path
 
 import pytest
 
 from cookiecutter import main, utils
 
 
 @pytest.fixture(scope='function')
@@ -61,30 +62,27 @@
 
 
 @pytest.mark.usefixtures('clean_system', 'remove_additional_dirs')
 def test_cookiecutter_no_input_return_rendered_file():
     """Verify Jinja2 templating correctly works in `cookiecutter.json` file."""
     project_dir = main.cookiecutter('tests/fake-repo-pre', no_input=True)
     assert project_dir == os.path.abspath('fake-project')
-    with open(os.path.join(project_dir, 'README.rst')) as fh:
-        contents = fh.read()
-    assert "Project name: **Fake Project**" in contents
+    content = Path(project_dir, 'README.rst').read_text()
+    assert "Project name: **Fake Project**" in content
 
 
 @pytest.mark.usefixtures('clean_system', 'remove_additional_dirs')
 def test_cookiecutter_dict_values_in_context():
     """Verify configured dictionary from `cookiecutter.json` correctly unpacked."""
     project_dir = main.cookiecutter('tests/fake-repo-dict', no_input=True)
     assert project_dir == os.path.abspath('fake-project-dict')
 
-    with open(os.path.join(project_dir, 'README.md')) as fh:
-        contents = fh.read()
-
+    content = Path(project_dir, 'README.md').read_text()
     assert (
-        contents
+        content
         == textwrap.dedent(
             """
         # README
 
 
         <dl>
           <dt>Format name:</dt>
```

### Comparing `cookiecutter-2.1.1/tests/test_cookiecutter_local_with_input.py` & `cookiecutter-2.2.0/tests/test_cookiecutter_local_with_input.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,29 +16,31 @@
         utils.rmtree('fake-project-input-extra')
 
 
 @pytest.mark.usefixtures('clean_system', 'remove_additional_dirs')
 def test_cookiecutter_local_with_input(monkeypatch):
     """Verify simple cookiecutter run results, without extra_context provided."""
     monkeypatch.setattr(
-        'cookiecutter.prompt.read_user_variable', lambda var, default: default
+        'cookiecutter.prompt.read_user_variable',
+        lambda var, default, prompts: default,
     )
     main.cookiecutter('tests/fake-repo-pre/', no_input=False)
     assert os.path.isdir('tests/fake-repo-pre/{{cookiecutter.repo_name}}')
     assert not os.path.isdir('tests/fake-repo-pre/fake-project')
     assert os.path.isdir('fake-project')
     assert os.path.isfile('fake-project/README.rst')
     assert not os.path.exists('fake-project/json/')
 
 
 @pytest.mark.usefixtures('clean_system', 'remove_additional_dirs')
 def test_cookiecutter_input_extra_context(monkeypatch):
     """Verify simple cookiecutter run results, with extra_context provided."""
     monkeypatch.setattr(
-        'cookiecutter.prompt.read_user_variable', lambda var, default: default
+        'cookiecutter.prompt.read_user_variable',
+        lambda var, default, prompts: default,
     )
     main.cookiecutter(
         'tests/fake-repo-pre',
         no_input=False,
         extra_context={'repo_name': 'fake-project-input-extra'},
     )
     assert os.path.isdir('fake-project-input-extra')
```

### Comparing `cookiecutter-2.1.1/tests/test_custom_extensions_in_hooks.py` & `cookiecutter-2.2.0/tests/test_custom_extensions_in_hooks.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """
 test_custom_extension_in_hooks.
 
 Tests to ensure custom cookiecutter extensions are properly made available to
 pre- and post-gen hooks.
 """
-import codecs
-import os
+from pathlib import Path
 
 import pytest
 
 from cookiecutter import main
 
 
 @pytest.fixture(
     params=['custom-extension-pre', 'custom-extension-post'],
     ids=['pre_gen_hook', 'post_gen_hook'],
 )
 def template(request):
     """Fixture. Allows to split pre and post hooks test directories."""
-    return 'tests/test-extensions/' + request.param
+    return f"tests/test-extensions/{request.param}"
 
 
 @pytest.fixture(autouse=True)
 def modify_syspath(monkeypatch):
     """Fixture. Make sure that the custom extension can be loaded."""
     monkeypatch.syspath_prepend('tests/test-extensions/hello_extension')
 
@@ -36,13 +35,9 @@
     project_dir = main.cookiecutter(
         template,
         no_input=True,
         output_dir=output_dir,
         extra_context={'project_slug': 'foobar', 'name': 'Cookiemonster'},
     )
 
-    readme_file = os.path.join(project_dir, 'README.rst')
-
-    with codecs.open(readme_file, encoding='utf8') as f:
-        readme = f.read().strip()
-
-    assert readme == 'Hello Cookiemonster!'
+    readme = Path(project_dir, 'README.rst').read_text(encoding="utf-8")
+    assert readme.strip() == 'Hello Cookiemonster!'
```

### Comparing `cookiecutter-2.1.1/tests/test_default_extensions.py` & `cookiecutter-2.2.0/tests/test_default_extensions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Verify Jinja2 filters/extensions are available from pre-gen/post-gen hooks."""
 import os
+import uuid
+from pathlib import Path
 
 import freezegun
 import pytest
-import uuid
 
 from cookiecutter.main import cookiecutter
 
 
 @pytest.fixture(autouse=True)
 def freeze():
     """Fixture. Make time stating during all tests in this file."""
@@ -21,15 +22,15 @@
     """Verify Jinja2 time extension work correctly."""
     project_dir = cookiecutter(
         'tests/test-extensions/default/', no_input=True, output_dir=str(tmp_path)
     )
     changelog_file = os.path.join(project_dir, 'HISTORY.rst')
     assert os.path.isfile(changelog_file)
 
-    with open(changelog_file, encoding='utf-8') as f:
+    with Path(changelog_file).open(encoding='utf-8') as f:
         changelog_lines = f.readlines()
 
     expected_lines = [
         'History\n',
         '-------\n',
         '\n',
         '0.1.0 (2015-12-09)\n',
@@ -53,12 +54,11 @@
     """Verify Jinja2 uuid extension work correctly."""
     project_dir = cookiecutter(
         'tests/test-extensions/default/', no_input=True, output_dir=str(tmp_path)
     )
     changelog_file = os.path.join(project_dir, 'id')
     assert os.path.isfile(changelog_file)
 
-    with open(changelog_file, encoding='utf-8') as f:
-        changelog_lines = f.readlines()
+    with Path(changelog_file).open(encoding='utf-8') as f:
+        changelog_lines = f.read().strip()
 
-    uuid.UUID(changelog_lines[0], version=4)
-    assert True
+    uuid.UUID(changelog_lines, version=4)
```

### Comparing `cookiecutter-2.1.1/tests/test_environment.py` & `cookiecutter-2.2.0/tests/test_environment.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,12 +14,12 @@
 
     assert 'Unable to load extension: ' in str(err.value)
 
 
 def test_env_should_come_with_default_extensions():
     """Verify default extensions loaded with StrictEnvironment."""
     env = StrictEnvironment(keep_trailing_newline=True)
-    assert 'jinja2_time.jinja2_time.TimeExtension' in env.extensions
     assert 'cookiecutter.extensions.JsonifyExtension' in env.extensions
     assert 'cookiecutter.extensions.RandomStringExtension' in env.extensions
     assert 'cookiecutter.extensions.SlugifyExtension' in env.extensions
+    assert 'cookiecutter.extensions.TimeExtension' in env.extensions
     assert 'cookiecutter.extensions.UUIDExtension' in env.extensions
```

### Comparing `cookiecutter-2.1.1/tests/test_exceptions.py` & `cookiecutter-2.2.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.1.1/tests/test_find.py` & `cookiecutter-2.2.0/tests/test_find.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Tests for `cookiecutter.find` module."""
-import os
+from pathlib import Path
 
 import pytest
 
 from cookiecutter import find
 
 
 @pytest.fixture(params=['fake-repo-pre', 'fake-repo-pre2'])
 def repo_dir(request):
     """Fixture returning path for `test_find_template` test."""
-    return os.path.join('tests', request.param)
+    return Path('tests', request.param)
 
 
 def test_find_template(repo_dir):
     """Verify correctness of `find.find_template` path detection."""
     template = find.find_template(repo_dir=repo_dir)
 
-    test_dir = os.path.join(repo_dir, '{{cookiecutter.repo_name}}')
+    test_dir = Path(repo_dir, '{{cookiecutter.repo_name}}')
     assert template == test_dir
```

### Comparing `cookiecutter-2.1.1/tests/test_generate_context.py` & `cookiecutter-2.2.0/tests/test_generate_context.py`

 * *Files 9% similar despite different names*

```diff
@@ -167,26 +167,27 @@
                 ('project_name', 'Kivy Project'),
                 ('repo_name', '{{cookiecutter.project_name|lower}}'),
                 ('orientation', ['all', 'landscape', 'portrait']),
             ]
         )
     }
 
-    generated_context = generate.generate_context(
-        context_file='tests/test-generate-context/choices_template.json',
-        default_context={
-            'not_in_template': 'foobar',
-            'project_name': 'Kivy Project',
-            'orientation': 'foobar',
-        },
-        extra_context={
-            'also_not_in_template': 'foobar2',
-            'github_username': 'hackebrot',
-        },
-    )
+    with pytest.warns(UserWarning, match="Invalid default received"):
+        generated_context = generate.generate_context(
+            context_file='tests/test-generate-context/choices_template.json',
+            default_context={
+                'not_in_template': 'foobar',
+                'project_name': 'Kivy Project',
+                'orientation': 'foobar',
+            },
+            extra_context={
+                'also_not_in_template': 'foobar2',
+                'github_username': 'hackebrot',
+            },
+        )
 
     assert generated_context == expected_context
 
 
 def test_apply_overwrites_invalid_overwrite(template_context):
     """Verify variables overwrite for list if variable not in list not ignored."""
     with pytest.raises(ValueError):
@@ -198,7 +199,49 @@
 def test_apply_overwrites_sets_default_for_choice_variable(template_context):
     """Verify overwritten list member became a default value."""
     generate.apply_overwrites_to_context(
         context=template_context, overwrite_context={'orientation': 'landscape'}
     )
 
     assert template_context['orientation'] == ['landscape', 'all', 'portrait']
+
+
+def test_apply_overwrites_in_nested_dict():
+    """Verify nested dict in default content settings are correctly replaced."""
+    expected_context = {
+        'nested_dict': OrderedDict(
+            [
+                ('full_name', 'Raphael Pierzina'),
+                ('github_username', 'hackebrot'),
+                (
+                    'project',
+                    OrderedDict(
+                        [
+                            ('name', 'My Kivy Project'),
+                            ('description', 'My Kivy Project'),
+                            ('repo_name', '{{cookiecutter.project_name|lower}}'),
+                            ('orientation', ["all", "landscape", "portrait"]),
+                        ]
+                    ),
+                ),
+            ]
+        )
+    }
+
+    generated_context = generate.generate_context(
+        context_file='tests/test-generate-context/nested_dict.json',
+        default_context={
+            'not_in_template': 'foobar',
+            'project': {
+                'description': 'My Kivy Project',
+            },
+        },
+        extra_context={
+            'also_not_in_template': 'foobar2',
+            'github_username': 'hackebrot',
+            'project': {
+                'name': 'My Kivy Project',
+            },
+        },
+    )
+
+    assert generated_context == expected_context
```

### Comparing `cookiecutter-2.1.1/tests/test_generate_file.py` & `cookiecutter-2.2.0/tests/test_generate_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Tests for `generate_file` function, part of `generate_files` function workflow."""
 import json
 import os
 import re
+from pathlib import Path
 
 import pytest
 from jinja2 import FileSystemLoader
 from jinja2.exceptions import TemplateSyntaxError
 
 from cookiecutter import generate
 from cookiecutter.environment import StrictEnvironment
@@ -41,44 +42,41 @@
     generate.generate_file(
         project_dir=".",
         infile=infile,
         context={'cookiecutter': {'generate_file': 'cheese'}},
         env=env,
     )
     assert os.path.isfile('tests/files/cheese.txt')
-    with open('tests/files/cheese.txt') as f:
-        generated_text = f.read()
-        assert generated_text == 'Testing cheese'
+    generated_text = Path('tests/files/cheese.txt').read_text()
+    assert generated_text == 'Testing cheese'
 
 
 def test_generate_file_jsonify_filter(env):
     """Verify jsonify filter works during files generation process."""
     infile = 'tests/files/{{cookiecutter.jsonify_file}}.txt'
     data = {'jsonify_file': 'cheese', 'type': 'roquefort'}
     generate.generate_file(
         project_dir=".", infile=infile, context={'cookiecutter': data}, env=env
     )
     assert os.path.isfile('tests/files/cheese.txt')
-    with open('tests/files/cheese.txt') as f:
-        generated_text = f.read()
-        assert json.loads(generated_text) == data
+    generated_text = Path('tests/files/cheese.txt').read_text()
+    assert json.loads(generated_text) == data
 
 
 @pytest.mark.parametrize("length", (10, 40))
 @pytest.mark.parametrize("punctuation", (True, False))
 def test_generate_file_random_ascii_string(env, length, punctuation):
     """Verify correct work of random_ascii_string extension on file generation."""
     infile = 'tests/files/{{cookiecutter.random_string_file}}.txt'
     data = {'random_string_file': 'cheese'}
     context = {"cookiecutter": data, "length": length, "punctuation": punctuation}
     generate.generate_file(project_dir=".", infile=infile, context=context, env=env)
     assert os.path.isfile('tests/files/cheese.txt')
-    with open('tests/files/cheese.txt') as f:
-        generated_text = f.read()
-        assert len(generated_text) == length
+    generated_text = Path('tests/files/cheese.txt').read_text()
+    assert len(generated_text) == length
 
 
 def test_generate_file_with_true_condition(env):
     """Verify correct work of boolean condition in file name on file generation.
 
     This test has positive answer, so file should be rendered.
     """
@@ -88,17 +86,16 @@
     generate.generate_file(
         project_dir=".",
         infile=infile,
         context={'cookiecutter': {'generate_file': 'y'}},
         env=env,
     )
     assert os.path.isfile('tests/files/cheese.txt')
-    with open('tests/files/cheese.txt') as f:
-        generated_text = f.read()
-        assert generated_text == 'Testing that generate_file was y'
+    generated_text = Path('tests/files/cheese.txt').read_text()
+    assert generated_text == 'Testing that generate_file was y'
 
 
 def test_generate_file_with_false_condition(env):
     """Verify correct work of boolean condition in file name on file generation.
 
     This test has negative answer, so file should not be rendered.
     """
@@ -144,15 +141,15 @@
         infile=infile,
         context={'cookiecutter': {'generate_file': 'cheese'}},
         env=env,
     )
 
     # this generated file should have a LF line ending
     gf = 'tests/files/cheese_lf_newlines.txt'
-    with open(gf, encoding='utf-8', newline='') as f:
+    with Path(gf).open(encoding='utf-8', newline='') as f:
         simple_text = f.readline()
     assert simple_text == 'newline is LF\n'
     assert f.newlines == '\n'
 
 
 def test_generate_file_does_not_translate_crlf_newlines_to_lf(env):
     """Verify that file generation use same line ending, as in source file."""
@@ -162,11 +159,11 @@
         infile=infile,
         context={'cookiecutter': {'generate_file': 'cheese'}},
         env=env,
     )
 
     # this generated file should have a CRLF line ending
     gf = 'tests/files/cheese_crlf_newlines.txt'
-    with open(gf, encoding='utf-8', newline='') as f:
+    with Path(gf).open(encoding='utf-8', newline='') as f:
         simple_text = f.readline()
     assert simple_text == 'newline is CRLF\r\n'
     assert f.newlines == '\r\n'
```

### Comparing `cookiecutter-2.1.1/tests/test_generate_files.py` & `cookiecutter-2.2.0/tests/test_generate_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,31 +40,31 @@
         output_dir=tmp_path,
     )
 
     simple_file = Path(tmp_path, 'inputpizzä/simple.txt')
     assert simple_file.exists()
     assert simple_file.is_file()
 
-    simple_text = open(simple_file, encoding='utf-8').read()
-    assert simple_text == 'I eat pizzä'
+    simple_text = Path(simple_file).read_text(encoding='utf-8')
+    assert simple_text == 'I eat pizzä\n'
 
 
 def test_generate_files_with_linux_newline(tmp_path):
     """Verify new line not removed by templating engine after folder generation."""
     generate.generate_files(
         context={'cookiecutter': {'food': 'pizzä'}},
         repo_dir='tests/test-generate-files',
         output_dir=tmp_path,
     )
 
     newline_file = Path(tmp_path, 'inputpizzä/simple-with-newline.txt')
     assert newline_file.is_file()
     assert newline_file.exists()
 
-    with open(newline_file, encoding='utf-8', newline='') as f:
+    with Path(newline_file).open(encoding='utf-8', newline='') as f:
         simple_text = f.readline()
     assert simple_text == 'newline is LF\n'
     assert f.newlines == '\n'
 
 
 def test_generate_files_with_jinja2_environment(tmp_path):
     """Extend StrictEnvironment with _jinja2_env_vars cookiecutter template option."""
@@ -79,15 +79,15 @@
         output_dir=tmp_path,
     )
 
     conditions_file = tmp_path.joinpath('inputpizzä/simple-with-conditions.txt')
     assert conditions_file.is_file()
     assert conditions_file.exists()
 
-    simple_text = conditions_file.open('rt', encoding='utf-8').read()
+    simple_text = conditions_file.read_text(encoding='utf-8')
     assert simple_text == 'I eat pizzä\n'
 
 
 def test_generate_files_with_trailing_newline_forced_to_linux_by_context(tmp_path):
     """Verify new line not removed by templating engine after folder generation."""
     generate.generate_files(
         context={'cookiecutter': {'food': 'pizzä', '_new_lines': '\r\n'}},
@@ -96,15 +96,15 @@
     )
 
     # assert 'Overwritting endline character with %s' in caplog.messages
     newline_file = Path(tmp_path, 'inputpizzä/simple-with-newline.txt')
     assert newline_file.is_file()
     assert newline_file.exists()
 
-    with open(newline_file, encoding='utf-8', newline='') as f:
+    with Path(newline_file).open(encoding='utf-8', newline='') as f:
         simple_text = f.readline()
     assert simple_text == 'newline is LF\r\n'
     assert f.newlines == '\r\n'
 
 
 def test_generate_files_with_windows_newline(tmp_path):
     """Verify windows source line end not changed during files generation."""
@@ -114,15 +114,15 @@
         output_dir=tmp_path,
     )
 
     newline_file = Path(tmp_path, 'inputpizzä/simple-with-newline-crlf.txt')
     assert newline_file.is_file()
     assert newline_file.exists()
 
-    with open(newline_file, encoding='utf-8', newline='') as f:
+    with Path(newline_file).open(encoding='utf-8', newline='') as f:
         simple_text = f.readline()
     assert simple_text == 'newline is CRLF\r\n'
     assert f.newlines == '\r\n'
 
 
 def test_generate_files_with_windows_newline_forced_to_linux_by_context(tmp_path):
     """Verify windows line end changed to linux during files generation."""
@@ -132,15 +132,15 @@
         output_dir=tmp_path,
     )
 
     newline_file = Path(tmp_path, 'inputpizzä/simple-with-newline-crlf.txt')
     assert newline_file.is_file()
     assert newline_file.exists()
 
-    with open(newline_file, encoding='utf-8', newline='') as f:
+    with Path(newline_file).open(encoding='utf-8', newline='') as f:
         simple_text = f.readline()
 
     assert simple_text == 'newline is CRLF\n'
     assert f.newlines == '\n'
 
 
 def test_generate_files_binaries(tmp_path):
@@ -198,15 +198,14 @@
     """
     generate.generate_files(
         context={'cookiecutter': {'permissions': 'permissions'}},
         repo_dir='tests/test-generate-files-permissions',
         output_dir=tmp_path,
     )
 
-    assert Path(tmp_path, 'inputpermissions/simple.txt').exists()
     assert Path(tmp_path, 'inputpermissions/simple.txt').is_file()
 
     # Verify source simple.txt should still be 0o644
     tests_simple_file = Path(
         'tests',
         'test-generate-files-permissions',
         'input{{cookiecutter.permissions}}',
@@ -237,15 +236,15 @@
 
 def test_generate_files_with_overwrite_if_exists_with_skip_if_file_exists(tmp_path):
     """Verify `skip_if_file_exist` has priority over `overwrite_if_exists`."""
     simple_file = Path(tmp_path, 'inputpizzä/simple.txt')
     simple_with_new_line_file = Path(tmp_path, 'inputpizzä/simple-with-newline.txt')
 
     Path(tmp_path, 'inputpizzä').mkdir(parents=True)
-    with open(simple_file, 'w') as f:
+    with Path(simple_file).open('w') as f:
         f.write('temp')
 
     generate.generate_files(
         context={'cookiecutter': {'food': 'pizzä'}},
         repo_dir='tests/test-generate-files',
         overwrite_if_exists=True,
         skip_if_file_exists=True,
@@ -253,67 +252,64 @@
     )
 
     assert Path(simple_file).is_file()
     assert Path(simple_file).exists()
     assert Path(simple_with_new_line_file).is_file()
     assert Path(simple_with_new_line_file).exists()
 
-    simple_text = open(simple_file, encoding='utf-8').read()
+    simple_text = Path(simple_file).read_text(encoding='utf-8')
     assert simple_text == 'temp'
 
 
 def test_generate_files_with_skip_if_file_exists(tmp_path):
     """Verify existed files not removed if error raised with `skip_if_file_exists`."""
     simple_file = Path(tmp_path, 'inputpizzä/simple.txt')
     simple_with_new_line_file = Path(tmp_path, 'inputpizzä/simple-with-newline.txt')
 
     Path(tmp_path, 'inputpizzä').mkdir(parents=True)
-    with open(simple_file, 'w') as f:
-        f.write('temp')
+    Path(simple_file).write_text('temp')
 
     with pytest.raises(exceptions.OutputDirExistsException):
         generate.generate_files(
             context={'cookiecutter': {'food': 'pizzä'}},
             repo_dir='tests/test-generate-files',
             skip_if_file_exists=True,
             output_dir=tmp_path,
         )
 
     assert Path(simple_file).is_file()
-    assert Path(simple_file).exists()
     assert not Path(simple_with_new_line_file).is_file()
     assert not Path(simple_with_new_line_file).exists()
 
-    simple_text = open(simple_file, encoding='utf-8').read()
+    simple_text = Path(simple_file).read_text(encoding='utf-8')
     assert simple_text == 'temp'
 
 
 def test_generate_files_with_overwrite_if_exists(tmp_path):
     """Verify overwrite_if_exists overwrites old files."""
     simple_file = Path(tmp_path, 'inputpizzä/simple.txt')
     simple_with_new_line_file = Path(tmp_path, 'inputpizzä/simple-with-newline.txt')
 
     Path(tmp_path, 'inputpizzä').mkdir(parents=True)
-    with open(simple_file, 'w') as f:
-        f.write('temp')
+    Path(simple_file).write_text('temp')
 
     generate.generate_files(
         context={'cookiecutter': {'food': 'pizzä'}},
         repo_dir='tests/test-generate-files',
         overwrite_if_exists=True,
         output_dir=tmp_path,
     )
 
     assert Path(simple_file).is_file()
     assert Path(simple_file).exists()
     assert Path(simple_with_new_line_file).is_file()
     assert Path(simple_with_new_line_file).exists()
 
-    simple_text = open(simple_file, encoding='utf-8').read()
-    assert simple_text == 'I eat pizzä'
+    simple_text = Path(simple_file).read_text(encoding='utf-8')
+    assert simple_text == 'I eat pizzä\n'
 
 
 @pytest.fixture
 def undefined_context():
     """Fixture. Populate context variable for future tests."""
     return {
         'cookiecutter': {'project_slug': 'testproject', 'github_username': 'hackebrot'}
@@ -386,14 +382,26 @@
     assert msg == error.message
 
     assert error.context == undefined_context
 
     assert not Path(output_dir).joinpath('testproject').exists()
 
 
+def test_keep_project_dir_on_failure(output_dir, undefined_context):
+    """Verify correct error raised when directory name cannot be rendered."""
+    with pytest.raises(exceptions.UndefinedVariableInTemplate):
+        generate.generate_files(
+            repo_dir='tests/undefined-variable/dir-name/',
+            output_dir=output_dir,
+            context=undefined_context,
+            keep_project_on_failure=True,
+        )
+    assert Path(output_dir).joinpath('testproject').exists()
+
+
 def test_raise_undefined_variable_dir_name_existing_project(
     output_dir, undefined_context
 ):
     """Verify correct error raised when directory name cannot be rendered."""
     testproj_path = Path(output_dir, 'testproject')
     testproj_path.mkdir()
```

### Comparing `cookiecutter-2.1.1/tests/test_generate_hooks.py` & `cookiecutter-2.2.0/tests/test_generate_hooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Test work of python and shell hooks for generated projects."""
 import errno
 import os
 import sys
+from pathlib import Path
 
 import pytest
 
 from cookiecutter import generate, utils
 from cookiecutter.exceptions import FailedHookException
 
 WINDOWS = sys.platform.startswith('win')
@@ -119,15 +120,15 @@
     template = os.path.join(repo_path, 'input{{cookiecutter.hooks}}')
     os.mkdir(repo_path)
     os.mkdir(hook_dir)
     os.mkdir(template)
 
     hook_path = os.path.join(hooks_path, 'pre_gen_project.py')
 
-    with open(hook_path, 'w') as f:
+    with Path(hook_path).open('w') as f:
         f.write("#!/usr/bin/env python\n")
         f.write("import sys; sys.exit(1)\n")
 
     with pytest.raises(FailedHookException) as excinfo:
         generate.generate_files(
             context={'cookiecutter': {'hooks': 'hooks'}},
             repo_dir='tests/test-hooks/',
@@ -148,15 +149,15 @@
     template = os.path.join(repo_path, 'input{{cookiecutter.hooks}}')
     os.mkdir(repo_path)
     os.mkdir(hook_dir)
     os.mkdir(template)
 
     hook_path = os.path.join(hooks_path, 'pre_gen_project.py')
 
-    with open(hook_path, 'w') as f:
+    with Path(hook_path).open('w') as f:
         f.write("#!/usr/bin/env python\n")
         f.write("import sys; sys.exit(1)\n")
 
     os.mkdir('inputhooks')
     with pytest.raises(FailedHookException) as excinfo:
         generate.generate_files(
             context={'cookiecutter': {'hooks': 'hooks'}},
```

### Comparing `cookiecutter-2.1.1/tests/test_get_config.py` & `cookiecutter-2.2.0/tests/test_get_config.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.1.1/tests/test_get_user_config.py` & `cookiecutter-2.2.0/tests/test_get_user_config.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.1.1/tests/test_hooks.py` & `cookiecutter-2.2.0/tests/test_hooks.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,70 +1,70 @@
 """Tests for `cookiecutter.hooks` module."""
-import os
 import errno
+import os
 import stat
 import sys
 import textwrap
+from pathlib import Path
 
 import pytest
 
 from cookiecutter import hooks, utils, exceptions
 
 
 def make_test_repo(name, multiple_hooks=False):
     """Create test repository for test setup methods."""
     hook_dir = os.path.join(name, 'hooks')
     template = os.path.join(name, 'input{{hooks}}')
     os.mkdir(name)
     os.mkdir(hook_dir)
     os.mkdir(template)
 
-    with open(os.path.join(template, 'README.rst'), 'w') as f:
-        f.write("foo\n===\n\nbar\n")
+    Path(template, 'README.rst').write_text("foo\n===\n\nbar\n")
 
-    with open(os.path.join(hook_dir, 'pre_gen_project.py'), 'w') as f:
+    with Path(hook_dir, 'pre_gen_project.py').open('w') as f:
         f.write("#!/usr/bin/env python\n")
         f.write("# -*- coding: utf-8 -*-\n")
         f.write("from __future__ import print_function\n")
         f.write("\n")
         f.write("print('pre generation hook')\n")
         f.write("f = open('python_pre.txt', 'w')\n")
         f.write("f.close()\n")
 
     if sys.platform.startswith('win'):
         post = 'post_gen_project.bat'
-        with open(os.path.join(hook_dir, post), 'w') as f:
+        with Path(hook_dir, post).open('w') as f:
             f.write("@echo off\n")
             f.write("\n")
             f.write("echo post generation hook\n")
             f.write("echo. >shell_post.txt\n")
     else:
         post = 'post_gen_project.sh'
         filename = os.path.join(hook_dir, post)
-        with open(filename, 'w') as f:
+        with Path(filename).open('w') as f:
             f.write("#!/bin/bash\n")
             f.write("\n")
             f.write("echo 'post generation hook';\n")
             f.write("touch 'shell_post.txt'\n")
         # Set the execute bit
         os.chmod(filename, os.stat(filename).st_mode | stat.S_IXUSR)
 
     # Adding an additional pre script
     if multiple_hooks:
         if sys.platform.startswith('win'):
             pre = 'pre_gen_project.bat'
-            with open(os.path.join(hook_dir, pre), 'w') as f:
+            with Path(hook_dir, pre).open('w') as f:
                 f.write("@echo off\n")
                 f.write("\n")
                 f.write("echo post generation hook\n")
                 f.write("echo. >shell_pre.txt\n")
         else:
             pre = 'pre_gen_project.sh'
             filename = os.path.join(hook_dir, pre)
-            with open(filename, 'w') as f:
+            with Path(filename).open('w') as f:
                 f.write("#!/bin/bash\n")
                 f.write("\n")
                 f.write("echo 'post generation hook';\n")
                 f.write("touch 'shell_pre.txt'\n")
             # Set the execute bit
             os.chmod(filename, os.stat(filename).st_mode | stat.S_IXUSR)
 
@@ -178,21 +178,21 @@
 
     def test_run_script_with_context(self):
         """Execute a hook script, passing a context."""
         hook_path = os.path.join(self.hooks_path, 'post_gen_project.sh')
 
         if sys.platform.startswith('win'):
             post = 'post_gen_project.bat'
-            with open(os.path.join(self.hooks_path, post), 'w') as f:
+            with Path(self.hooks_path, post).open('w') as f:
                 f.write("@echo off\n")
                 f.write("\n")
                 f.write("echo post generation hook\n")
                 f.write("echo. >{{cookiecutter.file}}\n")
         else:
-            with open(hook_path, 'w') as fh:
+            with Path(hook_path).open('w') as fh:
                 fh.write("#!/bin/bash\n")
                 fh.write("\n")
                 fh.write("echo 'post generation hook';\n")
                 fh.write("touch 'shell_post.txt'\n")
                 fh.write("touch '{{cookiecutter.file}}'\n")
                 os.chmod(hook_path, os.stat(hook_path).st_mode | stat.S_IXUSR)
 
@@ -217,15 +217,15 @@
             assert os.path.isfile(os.path.join(tests_dir, 'shell_post.txt'))
 
     def test_run_failing_hook(self):
         """Test correct exception raise if hook exit code is not zero."""
         hook_path = os.path.join(self.hooks_path, 'pre_gen_project.py')
         tests_dir = os.path.join(self.repo_path, 'input{{hooks}}')
 
-        with open(hook_path, 'w') as f:
+        with Path(hook_path).open('w') as f:
             f.write("#!/usr/bin/env python\n")
             f.write("import sys; sys.exit(1)\n")
 
         with utils.work_in(self.repo_path):
             with pytest.raises(exceptions.FailedHookException) as excinfo:
                 hooks.run_hook('pre_gen_project', tests_dir, {})
             assert 'Hook script failed' in str(excinfo.value)
```

### Comparing `cookiecutter-2.1.1/tests/test_log.py` & `cookiecutter-2.2.0/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.1.1/tests/test_main.py` & `cookiecutter-2.2.0/tests/test_main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,37 @@
 """Collection of tests around cookiecutter's replay feature."""
 from cookiecutter.main import cookiecutter
 
 
+def test_original_cookiecutter_options_preserved_in__cookiecutter(
+    monkeypatch,
+    mocker,
+    user_config_file,
+):
+    """Preserve original context options.
+
+    Tests you can access the original context options via
+    `context['_cookiecutter']`.
+    """
+    monkeypatch.chdir('tests/fake-repo-tmpl-_cookiecutter')
+    mock_generate_files = mocker.patch('cookiecutter.main.generate_files')
+    cookiecutter(
+        '.',
+        no_input=True,
+        replay=False,
+        config_file=user_config_file,
+    )
+    assert mock_generate_files.call_args[1]['context']['_cookiecutter'][
+        'test_list'
+    ] == [1, 2, 3, 4]
+    assert mock_generate_files.call_args[1]['context']['_cookiecutter'][
+        'test_dict'
+    ] == {"foo": "bar"}
+
+
 def test_replay_dump_template_name(
     monkeypatch, mocker, user_config_data, user_config_file
 ):
     """Check that replay_dump is called with a valid template_name.
 
     Template name must not be a relative path.
```

### Comparing `cookiecutter-2.1.1/tests/test_output_folder.py` & `cookiecutter-2.2.0/tests/test_output_folder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 tests_output_folder.
 
 Test formerly known from a unittest residing in test_generate.py named
 TestOutputFolder.test_output_folder
 """
 import os
+from pathlib import Path
 
 import pytest
 
 from cookiecutter import exceptions
 from cookiecutter import generate
 from cookiecutter import utils
 
@@ -27,20 +28,21 @@
     context = generate.generate_context(
         context_file='tests/test-output-folder/cookiecutter.json'
     )
     generate.generate_files(context=context, repo_dir='tests/test-output-folder')
 
     something = """Hi!
 My name is Audrey Greenfeld.
-It is 2014."""
-    something2 = open('output_folder/something.txt').read()
+It is 2014.
+"""
+    something2 = Path('output_folder/something.txt').read_text()
     assert something == something2
 
-    in_folder = "The color is green and the letter is D."
-    in_folder2 = open('output_folder/folder/in_folder.txt').read()
+    in_folder = "The color is green and the letter is D.\n"
+    in_folder2 = Path('output_folder/folder/in_folder.txt').read_text()
     assert in_folder == in_folder2
 
     assert os.path.isdir('output_folder/im_a.dir')
     assert os.path.isfile('output_folder/im_a.dir/im_a.file.py')
 
 
 @pytest.mark.usefixtures('clean_system', 'remove_output_folder')
```

### Comparing `cookiecutter-2.1.1/tests/test_preferred_encoding.py` & `cookiecutter-2.2.0/tests/test_preferred_encoding.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.1.1/tests/test_prompt.py` & `cookiecutter-2.2.0/tests/test_prompt.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 class TestRenderVariable:
     """Class to unite simple and complex tests for render_variable function."""
 
     @pytest.mark.parametrize(
         'raw_var, rendered_var',
         [
             (1, '1'),
-            (True, 'True'),
+            (True, True),
             ('foo', 'foo'),
             ('{{cookiecutter.project}}', 'foobar'),
             (None, None),
         ],
     )
     def test_convert_to_str(self, mocker, raw_var, rendered_var):
         """Verify simple items correctly rendered to strings."""
@@ -35,28 +35,28 @@
         )
         context = {'project': 'foobar'}
 
         result = prompt.render_variable(env, raw_var, context)
         assert result == rendered_var
 
         # Make sure that non None non str variables are converted beforehand
-        if raw_var is not None:
+        if raw_var is not None and not isinstance(raw_var, bool):
             if not isinstance(raw_var, str):
                 raw_var = str(raw_var)
             from_string.assert_called_once_with(raw_var)
         else:
             assert not from_string.called
 
     @pytest.mark.parametrize(
         'raw_var, rendered_var',
         [
-            ({1: True, 'foo': False}, {'1': 'True', 'foo': 'False'}),
+            ({1: True, 'foo': False}, {'1': True, 'foo': False}),
             (
                 {'{{cookiecutter.project}}': ['foo', 1], 'bar': False},
-                {'foobar': ['foo', '1'], 'bar': 'False'},
+                {'foobar': ['foo', '1'], 'bar': False},
             ),
             (['foo', '{{cookiecutter.project}}', None], ['foo', 'foobar', None]),
         ],
     )
     def test_convert_to_str_complex_variables(self, raw_var, rendered_var):
         """Verify tree items correctly rendered."""
         env = environment.StrictEnvironment()
@@ -77,25 +77,60 @@
         ],
         ids=['ASCII default prompt/input', 'Unicode default prompt/input'],
     )
     def test_prompt_for_config(self, monkeypatch, context):
         """Verify `prompt_for_config` call `read_user_variable` on text request."""
         monkeypatch.setattr(
             'cookiecutter.prompt.read_user_variable',
-            lambda var, default: default,
+            lambda var, default, prompts: default,
+        )
+
+        cookiecutter_dict = prompt.prompt_for_config(context)
+        assert cookiecutter_dict == context['cookiecutter']
+
+    @pytest.mark.parametrize(
+        'context',
+        [
+            {
+                'cookiecutter': {
+                    'full_name': 'Your Name',
+                    'check': ['yes', 'no'],
+                    'nothing': 'ok',
+                    '__prompts__': {
+                        'full_name': 'Name please',
+                        'check': 'Checking',
+                    },
+                }
+            },
+        ],
+        ids=['ASCII default prompt/input'],
+    )
+    def test_prompt_for_config_with_human_prompts(self, monkeypatch, context):
+        """Verify call `read_user_variable` on request when human-readable prompts."""
+        monkeypatch.setattr(
+            'cookiecutter.prompt.read_user_variable',
+            lambda var, default, prompts: default,
+        )
+        monkeypatch.setattr(
+            'cookiecutter.prompt.read_user_yes_no',
+            lambda var, default, prompts: default,
+        )
+        monkeypatch.setattr(
+            'cookiecutter.prompt.read_user_choice',
+            lambda var, default, prompts: default,
         )
 
         cookiecutter_dict = prompt.prompt_for_config(context)
         assert cookiecutter_dict == context['cookiecutter']
 
     def test_prompt_for_config_dict(self, monkeypatch):
         """Verify `prompt_for_config` call `read_user_variable` on dict request."""
         monkeypatch.setattr(
             'cookiecutter.prompt.read_user_dict',
-            lambda var, default: {"key": "value", "integer": 37},
+            lambda var, default, prompts: {"key": "value", "integer": 37},
         )
         context = {'cookiecutter': {'details': {}}}
 
         cookiecutter_dict = prompt.prompt_for_config(context)
         assert cookiecutter_dict == {'details': {'key': 'value', 'integer': 37}}
 
     def test_should_render_dict(self):
@@ -156,18 +191,61 @@
                     "deep_other_name": "Slartibartfast",
                     "deep_list": ["deep value 1", "Slartibartfast", "deep value 3"],
                 },
                 "list_key": ["value 1", "Slartibartfast", "value 3"],
             },
         }
 
+    def test_should_render_deep_dict_with_human_prompts(self):
+        """Verify dict rendered correctly when human-readable prompts."""
+        context = {
+            'cookiecutter': {
+                'project_name': "Slartibartfast",
+                'details': {
+                    "key": "value",
+                    "integer_key": 37,
+                    "other_name": '{{cookiecutter.project_name}}',
+                    "dict_key": {
+                        "deep_key": "deep_value",
+                    },
+                },
+                '__prompts__': {'project_name': 'Project name'},
+            }
+        }
+        cookiecutter_dict = prompt.prompt_for_config(context, no_input=True)
+        assert cookiecutter_dict == {
+            'project_name': "Slartibartfast",
+            'details': {
+                "key": "value",
+                "integer_key": "37",
+                "other_name": "Slartibartfast",
+                "dict_key": {
+                    "deep_key": "deep_value",
+                },
+            },
+        }
+
+    def test_internal_use_no_human_prompts(self):
+        """Verify dict rendered correctly when human-readable prompts empty."""
+        context = {
+            'cookiecutter': {
+                'project_name': "Slartibartfast",
+                '__prompts__': {},
+            }
+        }
+        cookiecutter_dict = prompt.prompt_for_config(context, no_input=True)
+        assert cookiecutter_dict == {
+            'project_name': "Slartibartfast",
+        }
+
     def test_prompt_for_templated_config(self, monkeypatch):
         """Verify Jinja2 templating works in unicode prompts."""
         monkeypatch.setattr(
-            'cookiecutter.prompt.read_user_variable', lambda var, default: default
+            'cookiecutter.prompt.read_user_variable',
+            lambda var, default, prompts: default,
         )
         context = {
             'cookiecutter': OrderedDict(
                 [
                     ('project_name', 'A New Project'),
                     (
                         'pkg_name',
@@ -270,15 +348,15 @@
         choices = ['landscape', 'portrait', 'all']
         context = {'cookiecutter': {'orientation': choices}}
 
         cookiecutter_dict = prompt.prompt_for_config(context)
 
         assert not read_user_variable.called
         assert prompt_choice.called
-        read_user_choice.assert_called_once_with('orientation', choices)
+        read_user_choice.assert_called_once_with('orientation', choices, {})
         assert cookiecutter_dict == {'orientation': 'all'}
 
     def test_should_invoke_read_user_variable(self, mocker):
         """Verify correct function called for string input variables."""
         read_user_variable = mocker.patch('cookiecutter.prompt.read_user_variable')
         read_user_variable.return_value = 'Audrey Roy'
 
@@ -288,15 +366,15 @@
 
         context = {'cookiecutter': {'full_name': 'Your Name'}}
 
         cookiecutter_dict = prompt.prompt_for_config(context)
 
         assert not prompt_choice.called
         assert not read_user_choice.called
-        read_user_variable.assert_called_once_with('full_name', 'Your Name')
+        read_user_variable.assert_called_once_with('full_name', 'Your Name', {})
         assert cookiecutter_dict == {'full_name': 'Audrey Roy'}
 
     def test_should_render_choices(self, mocker):
         """Verify Jinja2 templating engine works inside choices variables."""
         read_user_choice = mocker.patch('cookiecutter.prompt.read_user_choice')
         read_user_choice.return_value = 'anewproject'
 
@@ -323,16 +401,16 @@
 
         expected = {
             'project_name': 'A New Project',
             'pkg_name': 'anewproject',
         }
         cookiecutter_dict = prompt.prompt_for_config(context)
 
-        read_user_variable.assert_called_once_with('project_name', 'A New Project')
-        read_user_choice.assert_called_once_with('pkg_name', rendered_choices)
+        read_user_variable.assert_called_once_with('project_name', 'A New Project', {})
+        read_user_choice.assert_called_once_with('pkg_name', rendered_choices, {})
         assert cookiecutter_dict == expected
 
 
 class TestPromptChoiceForConfig:
     """Class to unite choices prompt related tests with config test."""
 
     @pytest.fixture
@@ -372,18 +450,54 @@
         actual_choice = prompt.prompt_choice_for_config(
             cookiecutter_dict=context,
             env=environment.StrictEnvironment(),
             key='orientation',
             options=choices,
             no_input=False,  # Ask the user for input
         )
-        read_user_choice.assert_called_once_with('orientation', choices)
+        read_user_choice.assert_called_once_with('orientation', choices, None)
         assert expected_choice == actual_choice
 
 
+class TestReadUserYesNo(object):
+    """Class to unite boolean prompt related tests."""
+
+    @pytest.mark.parametrize(
+        'run_as_docker',
+        (
+            True,
+            False,
+        ),
+    )
+    def test_should_invoke_read_user_yes_no(self, mocker, run_as_docker):
+        """Verify correct function called for boolean variables."""
+        read_user_yes_no = mocker.patch('cookiecutter.prompt.read_user_yes_no')
+        read_user_yes_no.return_value = run_as_docker
+
+        read_user_variable = mocker.patch('cookiecutter.prompt.read_user_variable')
+
+        context = {'cookiecutter': {'run_as_docker': run_as_docker}}
+
+        cookiecutter_dict = prompt.prompt_for_config(context)
+
+        assert not read_user_variable.called
+        read_user_yes_no.assert_called_once_with('run_as_docker', run_as_docker)
+        assert cookiecutter_dict == {'run_as_docker': run_as_docker}
+
+    def test_boolean_parameter_no_input(self):
+        """Verify boolean parameter sent to prompt for config with no input."""
+        context = {
+            'cookiecutter': {
+                'run_as_docker': True,
+            }
+        }
+        cookiecutter_dict = prompt.prompt_for_config(context, no_input=True)
+        assert cookiecutter_dict == context['cookiecutter']
+
+
 @pytest.mark.parametrize(
     'context',
     (
         {'cookiecutter': {'foo': '{{cookiecutter.nope}}'}},
         {'cookiecutter': {'foo': ['123', '{{cookiecutter.nope}}', '456']}},
         {'cookiecutter': {'foo': {'{{cookiecutter.nope}}': 'value'}}},
         {'cookiecutter': {'foo': {'key': '{{cookiecutter.nope}}'}}},
```

### Comparing `cookiecutter-2.1.1/tests/test_read_user_choice.py` & `cookiecutter-2.2.0/tests/test_read_user_choice.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.1.1/tests/test_read_user_dict.py` & `cookiecutter-2.2.0/tests/test_read_user_dict.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.1.1/tests/test_read_user_yes_no.py` & `cookiecutter-2.2.0/tests/test_read_user_yes_no.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.1.1/tests/test_specify_output_dir.py` & `cookiecutter-2.2.0/tests/test_specify_output_dir.py`

 * *Files 9% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     mock_gen_files.assert_called_once_with(
         repo_dir=template,
         context=context,
         overwrite_if_exists=False,
         skip_if_file_exists=False,
         output_dir=output_dir,
         accept_hooks=True,
+        keep_project_on_failure=False,
     )
 
 
 def test_default_output_dir(mocker, template, context):
     """Verify default output dir is current working folder."""
     mock_gen_files = mocker.patch('cookiecutter.main.generate_files')
 
@@ -69,8 +70,9 @@
     mock_gen_files.assert_called_once_with(
         repo_dir=template,
         context=context,
         overwrite_if_exists=False,
         skip_if_file_exists=False,
         output_dir='.',
         accept_hooks=True,
+        keep_project_on_failure=False,
     )
```

### Comparing `cookiecutter-2.1.1/tests/test_utils.py` & `cookiecutter-2.2.0/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,33 +13,31 @@
     mode = Path.stat(path).st_mode
     Path.chmod(path, mode & ~stat.S_IWRITE)
 
 
 def test_force_delete(mocker, tmp_path):
     """Verify `utils.force_delete` makes files writable."""
     ro_file = Path(tmp_path, 'bar')
-
-    with open(ro_file, "w") as f:
-        f.write("Test data")
+    ro_file.write_text("Test data")
     make_readonly(ro_file)
 
     rmtree = mocker.Mock()
     utils.force_delete(rmtree, ro_file, sys.exc_info())
 
     assert (ro_file.stat().st_mode & stat.S_IWRITE) == stat.S_IWRITE
     rmtree.assert_called_once_with(ro_file)
 
     utils.rmtree(tmp_path)
 
 
 def test_rmtree(tmp_path):
     """Verify `utils.rmtree` remove files marked as read-only."""
-    with open(Path(tmp_path, 'bar'), "w") as f:
-        f.write("Test data")
-    make_readonly(Path(tmp_path, 'bar'))
+    file_path = Path(tmp_path, "bar")
+    file_path.write_text("Test data")
+    make_readonly(file_path)
 
     utils.rmtree(tmp_path)
 
     assert not Path(tmp_path).exists()
 
 
 def test_make_sure_path_exists(tmp_path):
@@ -47,38 +45,34 @@
 
     Should return True if directory exist or created.
     Should return False if impossible to create directory (for example protected)
     """
     existing_directory = tmp_path
     directory_to_create = Path(tmp_path, "not_yet_created")
 
-    assert utils.make_sure_path_exists(existing_directory)
-    assert utils.make_sure_path_exists(directory_to_create)
+    utils.make_sure_path_exists(existing_directory)
+    utils.make_sure_path_exists(directory_to_create)
 
     # Ensure by base system methods.
     assert existing_directory.is_dir()
     assert existing_directory.exists()
     assert directory_to_create.is_dir()
     assert directory_to_create.exists()
 
 
 def test_make_sure_path_exists_correctly_handle_os_error(mocker):
     """Verify correct True/False response from `utils.make_sure_path_exists`.
 
     Should return True if directory exist or created.
     Should return False if impossible to create directory (for example protected)
     """
-
-    def raiser(*args, **kwargs):
-        raise OSError()
-
-    mocker.patch("os.makedirs", raiser)
-    uncreatable_directory = Path('protected_path')
-
-    assert not utils.make_sure_path_exists(uncreatable_directory)
+    mocker.patch("pathlib.Path.mkdir", side_effect=OSError)
+    with pytest.raises(OSError) as err:
+        utils.make_sure_path_exists(Path('protected_path'))
+    assert str(err.value) == "Unable to create directory at protected_path"
 
 
 def test_work_in(tmp_path):
     """Verify returning to original folder after `utils.work_in` use."""
     cwd = Path.cwd()
     ch_to = tmp_path
 
@@ -171,18 +165,15 @@
 
 
 def test_prompt_should_ask_and_keep_repo_on_reuse(mocker, tmp_path):
     """In `prompt_and_delete()`, if the user wants to keep their old \
     cloned template repo, it should not be deleted."""
 
     def answer(question, default):
-        if 'okay to delete' in question:
-            return False
-        else:
-            return True
+        return 'okay to delete' not in question
 
     mock_read_user = mocker.patch(
         'cookiecutter.utils.read_user_yes_no', side_effect=answer, autospec=True
     )
     repo_dir = Path(tmp_path, 'repo')
     repo_dir.mkdir()
```

### Comparing `cookiecutter-2.1.1/tests/vcs/test_clone.py` & `cookiecutter-2.2.0/tests/vcs/test_clone.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,19 +24,19 @@
     mocker.patch('cookiecutter.vcs.is_vcs_installed', autospec=True, return_value=True)
 
     mock_subprocess = mocker.patch(
         'cookiecutter.vcs.subprocess.check_output',
         autospec=True,
     )
 
-    vcs.clone('https://github.com/foo/bar/', clone_to_dir=str(clone_dir), no_input=True)
+    vcs.clone('https://github.com/foo/bar/', clone_to_dir=clone_dir, no_input=True)
 
     mock_subprocess.assert_called_once_with(
         ['git', 'clone', 'https://github.com/foo/bar'],
-        cwd=str(clone_dir),
+        cwd=clone_dir,
         stderr=subprocess.STDOUT,
     )
 
 
 def test_clone_should_abort_if_user_does_not_want_to_reclone(mocker, clone_dir):
     """In `clone()`, if user doesn't want to reclone, Cookiecutter should exit \
     without cloning anything."""
@@ -110,21 +110,21 @@
         autospec=True,
     )
     expected_repo_dir = os.path.normpath(os.path.join(clone_dir, repo_name))
 
     branch = 'foobar'
 
     repo_dir = vcs.clone(
-        repo_url, checkout=branch, clone_to_dir=str(clone_dir), no_input=True
+        repo_url, checkout=branch, clone_to_dir=clone_dir, no_input=True
     )
 
     assert repo_dir == expected_repo_dir
 
     mock_subprocess.assert_any_call(
-        [repo_type, 'clone', repo_url], cwd=str(clone_dir), stderr=subprocess.STDOUT
+        [repo_type, 'clone', repo_url], cwd=clone_dir, stderr=subprocess.STDOUT
     )
 
     branch_info = [branch]
     # We sanitize branch information for Mercurial
     if repo_type == "hg":
         branch_info.insert(0, "--")
```

### Comparing `cookiecutter-2.1.1/tests/vcs/test_identify_repo.py` & `cookiecutter-2.2.0/tests/vcs/test_identify_repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,22 +20,22 @@
         (
             'https://github.com/pytest-dev/cookiecutter-pytest-plugin.git',
             'git',
             'https://github.com/pytest-dev/cookiecutter-pytest-plugin.git',
         ),
         ('https://bitbucket.org/foo/bar.hg', 'hg', 'https://bitbucket.org/foo/bar.hg'),
         (
-            'https://github.com/audreyr/cookiecutter-pypackage.git',
+            'https://github.com/audreyfeldroy/cookiecutter-pypackage.git',
             'git',
-            'https://github.com/audreyr/cookiecutter-pypackage.git',
+            'https://github.com/audreyfeldroy/cookiecutter-pypackage.git',
         ),
         (
-            'https://github.com/audreyr/cookiecutter-pypackage',
+            'https://github.com/audreyfeldroy/cookiecutter-pypackage',
             'git',
-            'https://github.com/audreyr/cookiecutter-pypackage',
+            'https://github.com/audreyfeldroy/cookiecutter-pypackage',
         ),
         (
             'git@gitorious.org:cookiecutter-gitorious/cookiecutter-gitorious.git',
             'git',
             'git@gitorious.org:cookiecutter-gitorious/cookiecutter-gitorious.git',
         ),
         (
```

### Comparing `cookiecutter-2.1.1/tests/zipfile/test_unzip.py` & `cookiecutter-2.2.0/tests/zipfile/test_unzip.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 """Tests for function unzip() from zipfile module."""
+import shutil
 import tempfile
+from pathlib import Path
 
 import pytest
-import shutil
 
 from cookiecutter import zipfile
 from cookiecutter.exceptions import InvalidZipRepository
 
 
 def mock_download():
     """Fake download function."""
-    with open('tests/files/fake-repo-tmpl.zip', 'rb') as zf:
+    with Path('tests/files/fake-repo-tmpl.zip').open('rb') as zf:
         chunk = zf.read(1024)
         while chunk:
             yield chunk
             chunk = zf.read(1024)
 
 
 def mock_download_with_empty_chunks():
     """Fake download function."""
     yield
-    with open('tests/files/fake-repo-tmpl.zip', 'rb') as zf:
+    with Path('tests/files/fake-repo-tmpl.zip').open('rb') as zf:
         chunk = zf.read(1024)
         while chunk:
             yield chunk
             chunk = zf.read(1024)
 
 
 def test_unzip_local_file(mocker, clone_dir):
```

