# Comparing `tmp/python-troveclient-8.1.0.tar.gz` & `tmp/python-troveclient-8.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-troveclient-8.1.0.tar", last modified: Fri Feb 17 15:27:29 2023, max compression
+gzip compressed data, was "python-troveclient-8.2.0.tar", last modified: Thu Jul  6 08:36:58 2023, max compression
```

## Comparing `python-troveclient-8.1.0.tar` & `python-troveclient-8.2.0.tar`

### file list

```diff
@@ -1,303 +1,304 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 15:27:29.306739 python-troveclient-8.1.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      621 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       34 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1155 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6174 2023-02-17 15:27:29.000000 python-troveclient-8.1.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      571 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29810 2023-02-17 15:27:28.000000 python-troveclient-8.1.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2885 2023-02-17 15:27:29.306739 python-troveclient-8.1.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1783 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 15:27:29.254741 python-troveclient-8.1.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      359 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 15:27:29.254741 python-troveclient-8.1.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1869 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1011 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 15:27:29.254741 python-troveclient-8.1.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 15:27:29.254741 python-troveclient-8.1.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3864 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/doc/source/user/api.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      876 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1384 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/lower-constraints.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 15:27:29.254741 python-troveclient-8.1.0/python_troveclient.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2885 2023-02-17 15:27:29.000000 python-troveclient-8.1.0/python_troveclient.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12794 2023-02-17 15:27:29.000000 python-troveclient-8.1.0/python_troveclient.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-17 15:27:29.000000 python-troveclient-8.1.0/python_troveclient.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7122 2023-02-17 15:27:29.000000 python-troveclient-8.1.0/python_troveclient.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-17 15:27:29.000000 python-troveclient-8.1.0/python_troveclient.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-02-17 15:27:29.000000 python-troveclient-8.1.0/python_troveclient.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2023-02-17 15:27:29.000000 python-troveclient-8.1.0/python_troveclient.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-02-17 15:27:29.000000 python-troveclient-8.1.0/python_troveclient.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 15:27:29.246742 python-troveclient-8.1.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 15:27:29.278740 python-troveclient-8.1.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-backup-create-to-osc-c3d257365cf65cae.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-backup-delete-to-osc-e302b87809cb814c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-backup-list-instance-to-osc-e01cf8527e499768.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-backup-list-to-osc-ea5cbfb579f3ffc7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-backup-show-to-osc-022f42ad93136ce6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-cluster-create-to-osc-47e3bb3a83dcab76.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-cluster-delete-to-osc-9601c8bc0e637c4b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-cluster-grow-shrink-to-osc-a07bc0d974b0c0a4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-cluster-instances-to-osc-429eeb91d86da663.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-cluster-list-to-osc-93532b79db906a14.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-cluster-modules-to-osc-647a0564dafcef24.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-cluster-show-to-osc-5925431f5e94a746.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-configuration-attach-detach-to-osc-c5b52784910f2b09.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-configuration-create-to-osc-fd556891b57cce05.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-configuration-default-to-osc-55867236d19d83c4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-configuration-delete-to-osc-d52e6a2cc84994e5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-configuration-groups-for-clusters-6183b0b7b4fb8c9e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-configuration-instances-to-osc-80a7d7b9d0c79f62.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-configuration-list-to-osc-4a12d508f6bb5472.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-configuration-parameter-list-to-osc-3d1a383999dd2d64.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-configuration-parameter-show-to-osc-5bcf21662683ceee.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-configuration-show-to-osc-c139bb20a2ec18ec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-database-create-to-osc-b9e85dd2cbd9b21e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-database-delete-to-osc-e6703e2d438824d1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-database-list-to-osc-b547e8954e8b6fc7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-datastore-list-to-osc-007ff4144f630c57.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-datastore-show-to-osc-79a855d2e026ae80.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-datastore-version-list-to-osc-3fe8729d493f3de2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-datastore-version-show-to-osc-8c2035dbf6104a9f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-detach-replica-to-osc-1fadef6220e96f35.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-eject-replica-source-to-osc-c985a70eaab3f16b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-execution-delete-to-osc-013b4bf00a1cb8ff.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-flavor-list-to-osc-b8b3a42f3bae3851.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-flavor-show-to-osc-16ab5640f144cab7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-force-delete-to-osc-dfff1db4da937415.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-instance-create-to-osc-77484f1c477aa864.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-instance-delete-to-osc-bf8de501c8945d58.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-instance-detailed-list-23dc77ed898cc6db.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-instance-list-to-osc-05714dfce947a57e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-instance-show-to-osc-d97cac1c697dcbdd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-log-enable-to-osc-a97bbb3a7af7b80b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-log-list-to-osc-4bc11aa6e20de286.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-promote-to-replica-source-to-osc-6eca8c5507344205.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      304 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-quota-to-osc-c50c8ec190af8f58.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      334 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-reset-status-to-osc-bd84dcdc369e2270.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-resize-flavor-to-osc-ba0e7c038df8ecfe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-resize-volume-to-osc-aa5eaabb8f25edec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-restart-instance-to-osc-760c292b5b5c95de.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-root-disable-to-osc-52d81d96ec7e4e54.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-root-enable-to-osc-e3a087cc6f10a6f9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-root-show-to-osc-17e49422c5dc71de.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-update-to-osc-05eb21c5fa18a788.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      321 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-upgrade-to-osc-837461ff1d588be2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-user-access-related-to-osc-ae7da3a8f5fbdd6a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-user-create-to-osc-03158640dcaa8a0e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-user-delete-to-osc-35cb82b041ee2b48.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-user-show-to-osc-6ef3db10a82f1f46.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add-user-update-attributes-to-osc-5adfffe826a62f3b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add_mod_inst_count-ce532a2187b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/add_module_reapply-7645e34256d4c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/allow-backup-name-in-create-1a9e85978a3ab8bc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/bulk-delete-database-instances-7938121487fb11e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/cli-configuration-name-allowed-747c5d6f2d1f8c7a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/cluster-upgrade-d58d1fc4b8da0a03.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/datastore-specific-api-extensions-973b455a9922d072.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/datastore-version-volume-types-62556ce5917195fd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/drop-py-2-7-4ca3cf6a8ab8ca34.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/drop-python-3-6-and-3-7-8e07d44dd0e12619.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/fix-config-param-list-output-27bf30fce5388d4b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/fix-output-of-cluster-create-584d85ffe1129d57.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/fix-wrong-datastore-flavors-args-in-osc-e0322cb5424f8c1b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/fix_admin_keystoneauth1-ed534462434.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/flavor-list-disk-befd656f86592af1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/flavor-list-ephemeral-de4eee3a30b09b64.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       60 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/flavor-list-vcpu-d3fd769a137e307c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/force_delete-2d6bb5f99fe821c5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/get-all-database-instance-admin-3f1b83a487dd11e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/image-upgrade-dfa20861d756532d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/incremental_backup-c18804d6277adf62.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/locality-support-for-clusters-7e89f9ddbe5f4131.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/locality-support-for-replication-5834f1a2dcaf6883.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/module-ordering-2d1e1a3c37c30c71.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/module-support-for-clusters-87b41dd7648275bf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/module_update_all_ds-f5cdbb71462e3de4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/mongo-cluster-create-use-extended-perperties-be7c075585dc709a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/multi-region-ec516da866def1ed.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/paginate-config-list-c311ce3c5394d437.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/persist-error-message-cda8dfe485fe92ba.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/quota-upgrade-aed30d50c1f58502.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/remove-rax-references-in-client-33551aa2bb25181b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/run-an-action-on-many-resources-41bbe191318b97dd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/scheduled-backups-49729ce37e586463.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/train-01-backup-filtering-43dc1912c72f11e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/train-02-public-instance-642d6490d47811e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/use-i18n-for-shell.py-924c1624e30a6617.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       40 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/use-i18n-for-v1-shell.py-08209f5721f20a1f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/ussuri-01-instance-log-actions-794fced41f9c11ea.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/ussuri-02-instance-log-tail-save-0b267a761faa11ea.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/ussuri-03-force-delete-instance-1643114c2e1b11ea.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/ussuri-04-osc-reboot-instance-760190e02eac11ea.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/ussuri-05-osc-delete-datastore-version-6e03d20430e611ea.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/ussuri-06-osc-delete-datastore-57bab744345911ea.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/victoria-01-update-config-group.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/victoria-02-remove-flavor-api.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      484 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/victoria-03-replication-cli.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/victoria-add-role-for-instances.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/victoria-backup-strategy.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/victoria-create-datastore-version.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/victoria-flavor-optional.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/victoria-get-and-update-instance-access.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/victoria-rebuild-instance.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/wallaby-bulk-backup-delete.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/wallaby-datastore-version-number.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/wallaby-instance-operating-status.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/wallaby-project-backups.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/wallaby-restore-backup-from-remote.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/wallaby-update-datastore-version.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/notes/xena-support-project-name-quota-cli.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 15:27:29.282740 python-troveclient-8.1.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 15:27:29.282740 python-troveclient-8.1.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 15:27:29.282740 python-troveclient-8.1.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8543 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/requirements.txt
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1432 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/run_local.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7935 2023-02-17 15:27:29.310738 python-troveclient-8.1.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 15:27:29.282740 python-troveclient-8.1.0/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5920 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/tools/install_venv_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1989 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 15:27:29.286740 python-troveclient-8.1.0/troveclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      986 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1205 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/_i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 15:27:29.286740 python-troveclient-8.1.0/troveclient/apiclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/apiclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6975 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/apiclient/auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16094 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/apiclient/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12662 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/apiclient/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12796 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/apiclient/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3344 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/auth_plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9249 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19150 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1618 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/common.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 15:27:29.290740 python-troveclient-8.1.0/troveclient/compat/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1548 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/compat/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13840 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/compat/auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9759 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/compat/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16231 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/compat/cli.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14117 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/compat/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14048 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/compat/common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4850 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/compat/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7714 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/compat/mcli.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 15:27:29.290740 python-troveclient-8.1.0/troveclient/compat/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/compat/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14469 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/compat/tests/test_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13536 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/compat/tests/test_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1465 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/compat/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1220 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/compat/versions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1236 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1397 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/extension.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1172 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 15:27:29.290740 python-troveclient-8.1.0/troveclient/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1801 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/osc/plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 15:27:29.294739 python-troveclient-8.1.0/troveclient/osc/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/osc/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1279 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/osc/v1/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3759 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/osc/v1/database_backup_strategy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12431 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/osc/v1/database_backups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14705 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/osc/v1/database_clusters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16737 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/osc/v1/database_configurations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3437 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/osc/v1/database_flavors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30403 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/osc/v1/database_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1280 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/osc/v1/database_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7863 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/osc/v1/database_logs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2625 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/osc/v1/database_quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4945 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/osc/v1/database_root.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11254 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/osc/v1/database_users.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4077 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/osc/v1/databases.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11581 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/osc/v1/datastores.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3455 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/service_catalog.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31222 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/shell.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 15:27:29.298739 python-troveclient-8.1.0/troveclient/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31339 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 15:27:29.298739 python-troveclient-8.1.0/troveclient/tests/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      844 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/osc/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2949 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/osc/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 15:27:29.302739 python-troveclient-8.1.0/troveclient/tests/osc/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/osc/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7056 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/osc/v1/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3220 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/osc/v1/test_database_backup_strategy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12736 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/osc/v1/test_database_backups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12520 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/osc/v1/test_database_clusters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14875 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/osc/v1/test_database_configurations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3023 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/osc/v1/test_database_flavors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26675 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/osc/v1/test_database_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1684 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/osc/v1/test_database_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3579 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/osc/v1/test_database_logs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2205 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/osc/v1/test_database_quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5187 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/osc/v1/test_database_root.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9040 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/osc/v1/test_database_users.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4191 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/osc/v1/test_databases.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7153 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/osc/v1/test_datastores.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3641 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/test_accounts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1920 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/test_apiclient_exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11134 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/test_backups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17426 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23143 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5571 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/test_clusters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3245 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/test_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9663 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/test_configurations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3551 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/test_databases.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8840 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/test_datastores.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2995 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/test_discover.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12278 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/test_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3348 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/test_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11501 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/test_management.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6341 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/test_metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6036 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/test_modules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1766 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/test_root.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4410 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/test_secgroups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12961 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/test_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5098 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/test_users.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4020 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3487 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/tests/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11305 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 15:27:29.306739 python-troveclient-8.1.0/troveclient/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2113 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/v1/accounts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2200 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/v1/backup_strategy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10852 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/v1/backups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5232 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/v1/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4807 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/v1/clusters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5408 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/v1/configurations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2511 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/v1/databases.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5337 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/v1/datastores.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1743 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/v1/diagnostics.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1996 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/v1/flavors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2242 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/v1/hosts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20206 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/v1/instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1562 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/v1/limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11337 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/v1/management.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2951 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/v1/metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7321 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/v1/modules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1971 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/v1/quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3681 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/v1/root.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2946 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/v1/security_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    98469 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/v1/shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1479 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/v1/storage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5010 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/v1/users.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2023 2023-02-17 15:27:01.000000 python-troveclient-8.1.0/troveclient/v1/volume_types.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:58.196893 python-troveclient-8.2.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      621 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       34 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1155 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6174 2023-07-06 08:36:58.000000 python-troveclient-8.2.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      571 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29898 2023-07-06 08:36:57.000000 python-troveclient-8.2.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2936 2023-07-06 08:36:58.196893 python-troveclient-8.2.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1783 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:58.148893 python-troveclient-8.2.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      359 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:58.148893 python-troveclient-8.2.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1869 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1011 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:58.148893 python-troveclient-8.2.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:58.148893 python-troveclient-8.2.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3864 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/doc/source/user/api.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      876 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1384 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/lower-constraints.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:58.148893 python-troveclient-8.2.0/python_troveclient.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2936 2023-07-06 08:36:58.000000 python-troveclient-8.2.0/python_troveclient.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12825 2023-07-06 08:36:58.000000 python-troveclient-8.2.0/python_troveclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-07-06 08:36:58.000000 python-troveclient-8.2.0/python_troveclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7122 2023-07-06 08:36:58.000000 python-troveclient-8.2.0/python_troveclient.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-07-06 08:36:58.000000 python-troveclient-8.2.0/python_troveclient.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-07-06 08:36:58.000000 python-troveclient-8.2.0/python_troveclient.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2023-07-06 08:36:58.000000 python-troveclient-8.2.0/python_troveclient.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-07-06 08:36:58.000000 python-troveclient-8.2.0/python_troveclient.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:58.144893 python-troveclient-8.2.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:58.168893 python-troveclient-8.2.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-backup-create-to-osc-c3d257365cf65cae.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-backup-delete-to-osc-e302b87809cb814c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-backup-list-instance-to-osc-e01cf8527e499768.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-backup-list-to-osc-ea5cbfb579f3ffc7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-backup-show-to-osc-022f42ad93136ce6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-cluster-create-to-osc-47e3bb3a83dcab76.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-cluster-delete-to-osc-9601c8bc0e637c4b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-cluster-grow-shrink-to-osc-a07bc0d974b0c0a4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-cluster-instances-to-osc-429eeb91d86da663.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-cluster-list-to-osc-93532b79db906a14.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-cluster-modules-to-osc-647a0564dafcef24.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-cluster-show-to-osc-5925431f5e94a746.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-configuration-attach-detach-to-osc-c5b52784910f2b09.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-configuration-create-to-osc-fd556891b57cce05.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-configuration-default-to-osc-55867236d19d83c4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-configuration-delete-to-osc-d52e6a2cc84994e5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-configuration-groups-for-clusters-6183b0b7b4fb8c9e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-configuration-instances-to-osc-80a7d7b9d0c79f62.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-configuration-list-to-osc-4a12d508f6bb5472.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-configuration-parameter-list-to-osc-3d1a383999dd2d64.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-configuration-parameter-show-to-osc-5bcf21662683ceee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-configuration-show-to-osc-c139bb20a2ec18ec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-database-create-to-osc-b9e85dd2cbd9b21e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-database-delete-to-osc-e6703e2d438824d1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-database-list-to-osc-b547e8954e8b6fc7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-datastore-list-to-osc-007ff4144f630c57.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-datastore-show-to-osc-79a855d2e026ae80.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-datastore-version-list-to-osc-3fe8729d493f3de2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-datastore-version-show-to-osc-8c2035dbf6104a9f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-detach-replica-to-osc-1fadef6220e96f35.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-eject-replica-source-to-osc-c985a70eaab3f16b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-execution-delete-to-osc-013b4bf00a1cb8ff.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-flavor-list-to-osc-b8b3a42f3bae3851.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-flavor-show-to-osc-16ab5640f144cab7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-force-delete-to-osc-dfff1db4da937415.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-instance-create-to-osc-77484f1c477aa864.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-instance-delete-to-osc-bf8de501c8945d58.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-instance-detailed-list-23dc77ed898cc6db.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-instance-list-to-osc-05714dfce947a57e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-instance-show-to-osc-d97cac1c697dcbdd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-log-enable-to-osc-a97bbb3a7af7b80b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-log-list-to-osc-4bc11aa6e20de286.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-promote-to-replica-source-to-osc-6eca8c5507344205.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      304 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-quota-to-osc-c50c8ec190af8f58.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      334 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-reset-status-to-osc-bd84dcdc369e2270.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-resize-flavor-to-osc-ba0e7c038df8ecfe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-resize-volume-to-osc-aa5eaabb8f25edec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-restart-instance-to-osc-760c292b5b5c95de.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-root-disable-to-osc-52d81d96ec7e4e54.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-root-enable-to-osc-e3a087cc6f10a6f9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-root-show-to-osc-17e49422c5dc71de.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-update-to-osc-05eb21c5fa18a788.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      321 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-upgrade-to-osc-837461ff1d588be2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-user-access-related-to-osc-ae7da3a8f5fbdd6a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-user-create-to-osc-03158640dcaa8a0e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-user-delete-to-osc-35cb82b041ee2b48.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-user-show-to-osc-6ef3db10a82f1f46.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add-user-update-attributes-to-osc-5adfffe826a62f3b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add_mod_inst_count-ce532a2187b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/add_module_reapply-7645e34256d4c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/allow-backup-name-in-create-1a9e85978a3ab8bc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/bulk-delete-database-instances-7938121487fb11e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/cli-configuration-name-allowed-747c5d6f2d1f8c7a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/cluster-upgrade-d58d1fc4b8da0a03.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/datastore-specific-api-extensions-973b455a9922d072.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/datastore-version-volume-types-62556ce5917195fd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/drop-py-2-7-4ca3cf6a8ab8ca34.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/drop-python-3-6-and-3-7-8e07d44dd0e12619.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/fix-config-param-list-output-27bf30fce5388d4b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/fix-output-of-cluster-create-584d85ffe1129d57.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/fix-wrong-datastore-flavors-args-in-osc-e0322cb5424f8c1b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/fix_admin_keystoneauth1-ed534462434.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/flavor-list-disk-befd656f86592af1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/flavor-list-ephemeral-de4eee3a30b09b64.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       60 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/flavor-list-vcpu-d3fd769a137e307c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/force_delete-2d6bb5f99fe821c5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/get-all-database-instance-admin-3f1b83a487dd11e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/image-upgrade-dfa20861d756532d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/incremental_backup-c18804d6277adf62.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/locality-support-for-clusters-7e89f9ddbe5f4131.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/locality-support-for-replication-5834f1a2dcaf6883.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/module-ordering-2d1e1a3c37c30c71.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/module-support-for-clusters-87b41dd7648275bf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/module_update_all_ds-f5cdbb71462e3de4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/mongo-cluster-create-use-extended-perperties-be7c075585dc709a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/multi-region-ec516da866def1ed.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/paginate-config-list-c311ce3c5394d437.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/persist-error-message-cda8dfe485fe92ba.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/quota-upgrade-aed30d50c1f58502.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/remove-rax-references-in-client-33551aa2bb25181b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/run-an-action-on-many-resources-41bbe191318b97dd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/scheduled-backups-49729ce37e586463.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/train-01-backup-filtering-43dc1912c72f11e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/train-02-public-instance-642d6490d47811e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/use-i18n-for-shell.py-924c1624e30a6617.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       40 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/use-i18n-for-v1-shell.py-08209f5721f20a1f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/ussuri-01-instance-log-actions-794fced41f9c11ea.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/ussuri-02-instance-log-tail-save-0b267a761faa11ea.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/ussuri-03-force-delete-instance-1643114c2e1b11ea.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/ussuri-04-osc-reboot-instance-760190e02eac11ea.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/ussuri-05-osc-delete-datastore-version-6e03d20430e611ea.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/ussuri-06-osc-delete-datastore-57bab744345911ea.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/victoria-01-update-config-group.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/victoria-02-remove-flavor-api.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      484 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/victoria-03-replication-cli.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/victoria-add-role-for-instances.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/victoria-backup-strategy.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/victoria-create-datastore-version.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/victoria-flavor-optional.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/victoria-get-and-update-instance-access.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/victoria-rebuild-instance.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/wallaby-bulk-backup-delete.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/wallaby-datastore-version-number.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/wallaby-instance-operating-status.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/wallaby-project-backups.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/wallaby-restore-backup-from-remote.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/wallaby-update-datastore-version.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/notes/xena-support-project-name-quota-cli.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:58.172893 python-troveclient-8.2.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/source/2023.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:58.172893 python-troveclient-8.2.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:58.172893 python-troveclient-8.2.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8543 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/requirements.txt
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1432 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/run_local.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7975 2023-07-06 08:36:58.196893 python-troveclient-8.2.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:58.172893 python-troveclient-8.2.0/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5920 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/tools/install_venv_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1989 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:58.176893 python-troveclient-8.2.0/troveclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      986 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1205 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/_i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:58.176893 python-troveclient-8.2.0/troveclient/apiclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/apiclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6975 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/apiclient/auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16094 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/apiclient/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12662 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/apiclient/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12796 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/apiclient/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3344 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/auth_plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9249 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19150 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1618 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/common.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:58.176893 python-troveclient-8.2.0/troveclient/compat/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1548 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/compat/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13840 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/compat/auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9759 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/compat/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16231 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/compat/cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14117 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/compat/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14048 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/compat/common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4850 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/compat/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7714 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/compat/mcli.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:58.176893 python-troveclient-8.2.0/troveclient/compat/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/compat/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14469 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/compat/tests/test_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13536 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/compat/tests/test_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1465 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/compat/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1220 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/compat/versions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1236 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1397 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/extension.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1172 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:58.180893 python-troveclient-8.2.0/troveclient/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1801 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/osc/plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:58.180893 python-troveclient-8.2.0/troveclient/osc/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/osc/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1279 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/osc/v1/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3759 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/osc/v1/database_backup_strategy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12431 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/osc/v1/database_backups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14705 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/osc/v1/database_clusters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16737 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/osc/v1/database_configurations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3437 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/osc/v1/database_flavors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30403 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/osc/v1/database_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1280 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/osc/v1/database_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7863 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/osc/v1/database_logs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2625 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/osc/v1/database_quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4945 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/osc/v1/database_root.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11254 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/osc/v1/database_users.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4077 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/osc/v1/databases.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11581 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/osc/v1/datastores.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3455 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/service_catalog.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31222 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/shell.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:58.188893 python-troveclient-8.2.0/troveclient/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31339 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:58.188893 python-troveclient-8.2.0/troveclient/tests/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      844 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/osc/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2949 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/osc/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:58.188893 python-troveclient-8.2.0/troveclient/tests/osc/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/osc/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7056 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/osc/v1/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3220 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/osc/v1/test_database_backup_strategy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12736 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/osc/v1/test_database_backups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12520 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/osc/v1/test_database_clusters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14875 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/osc/v1/test_database_configurations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3023 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/osc/v1/test_database_flavors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26675 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/osc/v1/test_database_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1684 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/osc/v1/test_database_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3579 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/osc/v1/test_database_logs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2205 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/osc/v1/test_database_quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5187 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/osc/v1/test_database_root.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9040 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/osc/v1/test_database_users.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4191 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/osc/v1/test_databases.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7153 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/osc/v1/test_datastores.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3641 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/test_accounts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1920 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/test_apiclient_exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11134 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/test_backups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17426 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23143 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5571 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/test_clusters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3245 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/test_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9663 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/test_configurations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3551 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/test_databases.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8840 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/test_datastores.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2995 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/test_discover.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12278 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/test_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3348 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/test_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11501 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/test_management.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6341 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/test_metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6036 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/test_modules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1766 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/test_root.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4410 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/test_secgroups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12961 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/test_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5098 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/test_users.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4020 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3487 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/tests/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11305 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:58.196893 python-troveclient-8.2.0/troveclient/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2113 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/v1/accounts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2200 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/v1/backup_strategy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10852 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/v1/backups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5232 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/v1/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4807 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/v1/clusters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5408 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/v1/configurations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2511 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/v1/databases.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5337 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/v1/datastores.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1743 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/v1/diagnostics.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1996 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/v1/flavors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2242 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/v1/hosts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20206 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/v1/instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1562 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/v1/limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11337 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/v1/management.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2951 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/v1/metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7321 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/v1/modules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1971 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/v1/quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3681 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/v1/root.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2946 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/v1/security_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    98469 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/v1/shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1479 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/v1/storage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5010 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/v1/users.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2023 2023-07-06 08:36:17.000000 python-troveclient-8.2.0/troveclient/v1/volume_types.py
```

### Comparing `python-troveclient-8.1.0/.coveragerc` & `python-troveclient-8.2.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/.zuul.yaml` & `python-troveclient-8.2.0/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/AUTHORS` & `python-troveclient-8.2.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/CONTRIBUTING.rst` & `python-troveclient-8.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/ChangeLog` & `python-troveclient-8.2.0/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 CHANGES
 =======
 
+8.2.0
+-----
+
+* Add python 3.10 to setup.cfg metadata
+* Update master for stable/2023.1
+
 8.1.0
 -----
 
 * Switch to 2023.1 Python3 unit tests and generic template name
 * Fixing tests with tox 4.2.6
 * Update master for stable/zed
```

### Comparing `python-troveclient-8.1.0/LICENSE` & `python-troveclient-8.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/PKG-INFO` & `python-troveclient-8.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-troveclient
-Version: 8.1.0
+Version: 8.2.0
 Summary: Client library for OpenStack DBaaS API
 Home-page: https://docs.openstack.org/python-troveclient/latest
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: Python bindings to the OpenStack Trove API
         ==========================================
@@ -55,8 +55,9 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
```

### Comparing `python-troveclient-8.1.0/README.rst` & `python-troveclient-8.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/doc/source/conf.py` & `python-troveclient-8.2.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/doc/source/index.rst` & `python-troveclient-8.2.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/doc/source/user/api.rst` & `python-troveclient-8.2.0/doc/source/user/api.rst`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/doc/source/user/index.rst` & `python-troveclient-8.2.0/doc/source/user/index.rst`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/lower-constraints.txt` & `python-troveclient-8.2.0/lower-constraints.txt`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/python_troveclient.egg-info/PKG-INFO` & `python-troveclient-8.2.0/python_troveclient.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-troveclient
-Version: 8.1.0
+Version: 8.2.0
 Summary: Client library for OpenStack DBaaS API
 Home-page: https://docs.openstack.org/python-troveclient/latest
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: Python bindings to the OpenStack Trove API
         ==========================================
@@ -55,8 +55,9 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
```

### Comparing `python-troveclient-8.1.0/python_troveclient.egg-info/SOURCES.txt` & `python-troveclient-8.2.0/python_troveclient.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -142,14 +142,15 @@
 releasenotes/notes/wallaby-bulk-backup-delete.yaml
 releasenotes/notes/wallaby-datastore-version-number.yaml
 releasenotes/notes/wallaby-instance-operating-status.yaml
 releasenotes/notes/wallaby-project-backups.yaml
 releasenotes/notes/wallaby-restore-backup-from-remote.yaml
 releasenotes/notes/wallaby-update-datastore-version.yaml
 releasenotes/notes/xena-support-project-name-quota-cli.yaml
+releasenotes/source/2023.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/mitaka.rst
 releasenotes/source/newton.rst
 releasenotes/source/ocata.rst
 releasenotes/source/pike.rst
 releasenotes/source/queens.rst
```

### Comparing `python-troveclient-8.1.0/python_troveclient.egg-info/entry_points.txt` & `python-troveclient-8.2.0/python_troveclient.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/releasenotes/source/conf.py` & `python-troveclient-8.2.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/requirements.txt` & `python-troveclient-8.2.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/run_local.sh` & `python-troveclient-8.2.0/run_local.sh`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/setup.cfg` & `python-troveclient-8.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: Apache Software License
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 
 [files]
 packages = 
 	troveclient
 
 [entry_points]
 console_scripts =
```

### Comparing `python-troveclient-8.1.0/setup.py` & `python-troveclient-8.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/test-requirements.txt` & `python-troveclient-8.2.0/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/tools/install_venv_common.py` & `python-troveclient-8.2.0/tools/install_venv_common.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/tox.ini` & `python-troveclient-8.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/__init__.py` & `python-troveclient-8.2.0/troveclient/__init__.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/_i18n.py` & `python-troveclient-8.2.0/troveclient/_i18n.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/apiclient/auth.py` & `python-troveclient-8.2.0/troveclient/apiclient/auth.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/apiclient/base.py` & `python-troveclient-8.2.0/troveclient/apiclient/base.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/apiclient/client.py` & `python-troveclient-8.2.0/troveclient/apiclient/client.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/apiclient/exceptions.py` & `python-troveclient-8.2.0/troveclient/apiclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/auth_plugin.py` & `python-troveclient-8.2.0/troveclient/auth_plugin.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/base.py` & `python-troveclient-8.2.0/troveclient/base.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/client.py` & `python-troveclient-8.2.0/troveclient/client.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/common.py` & `python-troveclient-8.2.0/troveclient/common.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/compat/__init__.py` & `python-troveclient-8.2.0/troveclient/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/compat/auth.py` & `python-troveclient-8.2.0/troveclient/compat/auth.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/compat/base.py` & `python-troveclient-8.2.0/troveclient/compat/base.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/compat/cli.py` & `python-troveclient-8.2.0/troveclient/compat/cli.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/compat/client.py` & `python-troveclient-8.2.0/troveclient/compat/client.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/compat/common.py` & `python-troveclient-8.2.0/troveclient/compat/common.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/compat/exceptions.py` & `python-troveclient-8.2.0/troveclient/compat/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/compat/mcli.py` & `python-troveclient-8.2.0/troveclient/compat/mcli.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/compat/tests/test_auth.py` & `python-troveclient-8.2.0/troveclient/compat/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/compat/tests/test_common.py` & `python-troveclient-8.2.0/troveclient/compat/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/compat/utils.py` & `python-troveclient-8.2.0/troveclient/compat/utils.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/compat/versions.py` & `python-troveclient-8.2.0/troveclient/compat/versions.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/exceptions.py` & `python-troveclient-8.2.0/troveclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/extension.py` & `python-troveclient-8.2.0/troveclient/extension.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/i18n.py` & `python-troveclient-8.2.0/troveclient/i18n.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/osc/plugin.py` & `python-troveclient-8.2.0/troveclient/osc/plugin.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/osc/v1/base.py` & `python-troveclient-8.2.0/troveclient/osc/v1/base.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/osc/v1/database_backup_strategy.py` & `python-troveclient-8.2.0/troveclient/osc/v1/database_backup_strategy.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/osc/v1/database_backups.py` & `python-troveclient-8.2.0/troveclient/osc/v1/database_backups.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/osc/v1/database_clusters.py` & `python-troveclient-8.2.0/troveclient/osc/v1/database_clusters.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/osc/v1/database_configurations.py` & `python-troveclient-8.2.0/troveclient/osc/v1/database_configurations.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/osc/v1/database_flavors.py` & `python-troveclient-8.2.0/troveclient/osc/v1/database_flavors.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/osc/v1/database_instances.py` & `python-troveclient-8.2.0/troveclient/osc/v1/database_instances.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/osc/v1/database_limits.py` & `python-troveclient-8.2.0/troveclient/osc/v1/database_limits.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/osc/v1/database_logs.py` & `python-troveclient-8.2.0/troveclient/osc/v1/database_logs.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/osc/v1/database_quota.py` & `python-troveclient-8.2.0/troveclient/osc/v1/database_quota.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/osc/v1/database_root.py` & `python-troveclient-8.2.0/troveclient/osc/v1/database_root.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/osc/v1/database_users.py` & `python-troveclient-8.2.0/troveclient/osc/v1/database_users.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/osc/v1/databases.py` & `python-troveclient-8.2.0/troveclient/osc/v1/databases.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/osc/v1/datastores.py` & `python-troveclient-8.2.0/troveclient/osc/v1/datastores.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/service_catalog.py` & `python-troveclient-8.2.0/troveclient/service_catalog.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/shell.py` & `python-troveclient-8.2.0/troveclient/shell.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/fakes.py` & `python-troveclient-8.2.0/troveclient/tests/fakes.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/osc/fakes.py` & `python-troveclient-8.2.0/troveclient/tests/osc/fakes.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/osc/utils.py` & `python-troveclient-8.2.0/troveclient/tests/osc/utils.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/osc/v1/fakes.py` & `python-troveclient-8.2.0/troveclient/tests/osc/v1/fakes.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/osc/v1/test_database_backup_strategy.py` & `python-troveclient-8.2.0/troveclient/tests/osc/v1/test_database_backup_strategy.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/osc/v1/test_database_backups.py` & `python-troveclient-8.2.0/troveclient/tests/osc/v1/test_database_backups.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/osc/v1/test_database_clusters.py` & `python-troveclient-8.2.0/troveclient/tests/osc/v1/test_database_clusters.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/osc/v1/test_database_configurations.py` & `python-troveclient-8.2.0/troveclient/tests/osc/v1/test_database_configurations.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/osc/v1/test_database_flavors.py` & `python-troveclient-8.2.0/troveclient/tests/osc/v1/test_database_flavors.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/osc/v1/test_database_instances.py` & `python-troveclient-8.2.0/troveclient/tests/osc/v1/test_database_instances.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/osc/v1/test_database_limits.py` & `python-troveclient-8.2.0/troveclient/tests/osc/v1/test_database_limits.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/osc/v1/test_database_logs.py` & `python-troveclient-8.2.0/troveclient/tests/osc/v1/test_database_logs.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/osc/v1/test_database_quota.py` & `python-troveclient-8.2.0/troveclient/tests/osc/v1/test_database_quota.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/osc/v1/test_database_root.py` & `python-troveclient-8.2.0/troveclient/tests/osc/v1/test_database_root.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/osc/v1/test_database_users.py` & `python-troveclient-8.2.0/troveclient/tests/osc/v1/test_database_users.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/osc/v1/test_databases.py` & `python-troveclient-8.2.0/troveclient/tests/osc/v1/test_databases.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/osc/v1/test_datastores.py` & `python-troveclient-8.2.0/troveclient/tests/osc/v1/test_datastores.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/test_accounts.py` & `python-troveclient-8.2.0/troveclient/tests/test_accounts.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/test_apiclient_exceptions.py` & `python-troveclient-8.2.0/troveclient/tests/test_apiclient_exceptions.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/test_backups.py` & `python-troveclient-8.2.0/troveclient/tests/test_backups.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/test_base.py` & `python-troveclient-8.2.0/troveclient/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/test_client.py` & `python-troveclient-8.2.0/troveclient/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/test_clusters.py` & `python-troveclient-8.2.0/troveclient/tests/test_clusters.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/test_common.py` & `python-troveclient-8.2.0/troveclient/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/test_configurations.py` & `python-troveclient-8.2.0/troveclient/tests/test_configurations.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/test_databases.py` & `python-troveclient-8.2.0/troveclient/tests/test_databases.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/test_datastores.py` & `python-troveclient-8.2.0/troveclient/tests/test_datastores.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/test_discover.py` & `python-troveclient-8.2.0/troveclient/tests/test_discover.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/test_instances.py` & `python-troveclient-8.2.0/troveclient/tests/test_instances.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/test_limits.py` & `python-troveclient-8.2.0/troveclient/tests/test_limits.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/test_management.py` & `python-troveclient-8.2.0/troveclient/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/test_metadata.py` & `python-troveclient-8.2.0/troveclient/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/test_modules.py` & `python-troveclient-8.2.0/troveclient/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/test_root.py` & `python-troveclient-8.2.0/troveclient/tests/test_root.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/test_secgroups.py` & `python-troveclient-8.2.0/troveclient/tests/test_secgroups.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/test_shell.py` & `python-troveclient-8.2.0/troveclient/tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/test_users.py` & `python-troveclient-8.2.0/troveclient/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/test_utils.py` & `python-troveclient-8.2.0/troveclient/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/tests/utils.py` & `python-troveclient-8.2.0/troveclient/tests/utils.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/utils.py` & `python-troveclient-8.2.0/troveclient/utils.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/v1/accounts.py` & `python-troveclient-8.2.0/troveclient/v1/accounts.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/v1/backup_strategy.py` & `python-troveclient-8.2.0/troveclient/v1/backup_strategy.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/v1/backups.py` & `python-troveclient-8.2.0/troveclient/v1/backups.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/v1/client.py` & `python-troveclient-8.2.0/troveclient/v1/client.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/v1/clusters.py` & `python-troveclient-8.2.0/troveclient/v1/clusters.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/v1/configurations.py` & `python-troveclient-8.2.0/troveclient/v1/configurations.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/v1/databases.py` & `python-troveclient-8.2.0/troveclient/v1/databases.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/v1/datastores.py` & `python-troveclient-8.2.0/troveclient/v1/datastores.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/v1/diagnostics.py` & `python-troveclient-8.2.0/troveclient/v1/diagnostics.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/v1/flavors.py` & `python-troveclient-8.2.0/troveclient/v1/flavors.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/v1/hosts.py` & `python-troveclient-8.2.0/troveclient/v1/hosts.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/v1/instances.py` & `python-troveclient-8.2.0/troveclient/v1/instances.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/v1/limits.py` & `python-troveclient-8.2.0/troveclient/v1/limits.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/v1/management.py` & `python-troveclient-8.2.0/troveclient/v1/management.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/v1/metadata.py` & `python-troveclient-8.2.0/troveclient/v1/metadata.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/v1/modules.py` & `python-troveclient-8.2.0/troveclient/v1/modules.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/v1/quota.py` & `python-troveclient-8.2.0/troveclient/v1/quota.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/v1/root.py` & `python-troveclient-8.2.0/troveclient/v1/root.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/v1/security_groups.py` & `python-troveclient-8.2.0/troveclient/v1/security_groups.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/v1/shell.py` & `python-troveclient-8.2.0/troveclient/v1/shell.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/v1/storage.py` & `python-troveclient-8.2.0/troveclient/v1/storage.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/v1/users.py` & `python-troveclient-8.2.0/troveclient/v1/users.py`

 * *Files identical despite different names*

### Comparing `python-troveclient-8.1.0/troveclient/v1/volume_types.py` & `python-troveclient-8.2.0/troveclient/v1/volume_types.py`

 * *Files identical despite different names*

