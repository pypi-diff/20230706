# Comparing `tmp/modelaapi-0.6.102.tar.gz` & `tmp/modelaapi-0.6.200.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelaapi-0.6.102.tar", last modified: Thu Jun  1 21:52:40 2023, max compression
+gzip compressed data, was "modelaapi-0.6.200.tar", last modified: Wed Jul  5 17:57:48 2023, max compression
```

## Comparing `modelaapi-0.6.102.tar` & `modelaapi-0.6.200.tar`

### file list

```diff
@@ -1,481 +1,481 @@
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.580294 modelaapi-0.6.102/
--rw-rw-r--   0 liam      (1000) liam      (1000)      139 2023-01-26 17:46:09.000000 modelaapi-0.6.102/AUTHORS.rst
--rw-rw-r--   0 liam      (1000) liam      (1000)     3579 2023-01-26 17:46:09.000000 modelaapi-0.6.102/CONTRIBUTING.rst
--rw-rw-r--   0 liam      (1000) liam      (1000)        0 2023-01-26 17:46:09.000000 modelaapi-0.6.102/DESCRIPTION.md
--rw-rw-r--   0 liam      (1000) liam      (1000)       89 2023-01-26 17:46:09.000000 modelaapi-0.6.102/HISTORY.rst
--rw-rw-r--   0 liam      (1000) liam      (1000)    11351 2023-01-26 17:46:09.000000 modelaapi-0.6.102/LICENSE.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)      437 2023-01-26 17:46:09.000000 modelaapi-0.6.102/MANIFEST.in
--rw-rw-r--   0 liam      (1000) liam      (1000)     1047 2023-01-26 17:46:09.000000 modelaapi-0.6.102/Makefile
--rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-06-01 21:52:40.580294 modelaapi-0.6.102/PKG-INFO
--rw-rw-r--   0 liam      (1000) liam      (1000)      762 2023-01-26 17:46:09.000000 modelaapi-0.6.102/README.md
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.508289 modelaapi-0.6.102/github/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.508289 modelaapi-0.6.102/github/com/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.508289 modelaapi-0.6.102/github/com/gogo/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/gogo/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.512289 modelaapi-0.6.102/github/com/gogo/protobuf/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/gogo/protobuf/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.512289 modelaapi-0.6.102/github/com/gogo/protobuf/gogoproto/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/gogo/protobuf/gogoproto/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14416 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/gogo/protobuf/gogoproto/gogo_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/gogo/protobuf/gogoproto/gogo_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.512289 modelaapi-0.6.102/github/com/metaprov/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.512289 modelaapi-0.6.102/github/com/metaprov/modelaapi/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.512289 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.512289 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.512289 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/catalog/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/catalog/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.512289 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    23584 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.512289 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/data/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/data/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.512289 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    51143 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.512289 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/inference/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/inference/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.516289 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    25376 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.516289 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/infra/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/infra/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.516289 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    25800 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.516289 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/team/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/team/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.516289 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11918 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.516289 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/training/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/training/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.516289 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    60860 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.516289 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.516289 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/account/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/account/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.520290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/account/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/account/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11310 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    24380 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.520290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/alert/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/alert/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.520290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/alert/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/alert/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7196 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11335 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.520290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/attachment/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/attachment/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.520290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/attachment/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/attachment/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7919 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.520290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/batchpredictord/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/batchpredictord/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.520290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/batchpredictord/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/batchpredictord/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7549 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7751 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.520290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/catalog/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/catalog/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.520290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/catalog/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/catalog/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    19189 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    33508 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.524290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/cloudproxyd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/cloudproxyd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.524290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/cloudproxyd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/cloudproxyd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6517 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    16493 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.524290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/commit/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/commit/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.524290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/commit/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/commit/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14479 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11490 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.524290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/common/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/common/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.524290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/common/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/common/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14189 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/common/v1/common_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.524290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/connection/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/connection/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.524290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/connection/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/connection/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8826 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14287 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.524290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/conversation/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/conversation/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.528290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/conversation/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/conversation/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    31897 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.528290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/data/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/data/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.528290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/data/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/data/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    82473 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)   111042 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.528290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataapp/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataapp/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.528290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataapp/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataapp/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9057 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    17941 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.528290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datapipeline/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datapipeline/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.528290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datapipeline/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datapipeline/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8161 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14642 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.528290 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datapipelinerun/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datapipelinerun/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.532291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datapipelinerun/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datapipelinerun/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10253 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    19897 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.532291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataproduct/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataproduct/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.532291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataproduct/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataproduct/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8425 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12265 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.532291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataproductversion/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataproductversion/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.532291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataproductversion/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataproductversion/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8095 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13350 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.532291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataset/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataset/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.532291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataset/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataset/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    19016 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    35095 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.532291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datasource/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datasource/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.532291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datasource/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datasource/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9636 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    16324 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.536291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dbproxyd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dbproxyd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.536291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dbproxyd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dbproxyd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    78210 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)   348679 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.536291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/entity/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/entity/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.536291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/entity/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/entity/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6605 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11503 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.536291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/featuregroup/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/featuregroup/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.536291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/featuregroup/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/featuregroup/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10534 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    21293 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.536291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/featurehistogram/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/featurehistogram/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.540291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/featurehistogram/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/featurehistogram/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7606 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13040 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.540291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/fileservices/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/fileservices/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.540291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/fileservices/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/fileservices/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3038 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3345 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.540291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/grpcinferenceservice/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/grpcinferenceservice/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.540291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    18564 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    24869 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.540291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/k8score/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/k8score/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.540291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/k8score/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/k8score/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    20839 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    26279 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.540291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/lab/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/lab/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.540291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/lab/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/lab/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6886 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11025 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.544291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/license/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/license/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.544291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/license/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/license/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8088 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13831 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.544291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/model/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/model/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.544291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/model/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/model/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    20626 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    44447 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.544291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelasystem/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelasystem/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.544291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelasystem/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelasystem/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4690 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7755 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.544291 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelclass/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelclass/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.548292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelclass/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelclass/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10011 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    18664 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.548292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modeldsystem/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modeldsystem/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.548292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modeldsystem/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modeldsystem/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.548292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/notifier/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/notifier/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.548292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/notifier/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/notifier/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7054 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11800 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.548292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/objectstored/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/objectstored/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.548292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/objectstored/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/objectstored/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3626 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9814 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.548292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/offlinefeaturestored/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/offlinefeaturestored/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.552292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3276 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5855 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.552292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/onlinefeaturestored/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/onlinefeaturestored/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.552292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5036 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5675 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.552292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/postmortem/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/postmortem/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.552292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/postmortem/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/postmortem/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6924 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.552292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/prediction/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/prediction/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.552292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/prediction/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/prediction/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8637 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    16389 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.552292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/predictionstore/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/predictionstore/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.552292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/predictionstore/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/predictionstore/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     2824 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3486 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.552292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/predictor/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/predictor/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.552292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/predictor/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/predictor/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9068 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    16147 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.552292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/publisherd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/publisherd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.556292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/publisherd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/publisherd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7197 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7539 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.556292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/recipe/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/recipe/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.556292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/recipe/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/recipe/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8686 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    15629 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.556292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/reciperun/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/reciperun/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.556292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/reciperun/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/reciperun/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6809 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11955 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.556292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/report/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/report/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.556292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/report/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/report/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7381 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13561 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.556292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/review/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/review/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.556292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/review/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/review/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7474 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.556292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/runbook/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/runbook/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.556292 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/runbook/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/runbook/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6596 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11645 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.560293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/servingsite/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/servingsite/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.560293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/servingsite/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/servingsite/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7910 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14432 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.560293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/sqlquery/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/sqlquery/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.560293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/sqlquery/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/sqlquery/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13739 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13906 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.560293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/sqlqueryrun/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/sqlqueryrun/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.564293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14535 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14465 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.564293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/study/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/study/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.564293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/study/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/study/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11657 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    23824 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.564293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/system/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/system/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.564293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/system/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/system/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14859 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7442 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.564293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/tenant/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/tenant/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.564293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/tenant/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/tenant/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9747 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    15755 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.564293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/todo/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/todo/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.564293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/todo/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/todo/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6407 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11180 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.564293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/trainerd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/trainerd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.568293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/trainerd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/trainerd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    22775 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    17719 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.568293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/userroleclass/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/userroleclass/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.568293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/userroleclass/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/userroleclass/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8160 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12588 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.568293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/virtualbucket/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/virtualbucket/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.568293 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/virtualbucket/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/virtualbucket/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7168 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12575 2023-06-01 21:27:56.000000 modelaapi-0.6.102/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.568293 modelaapi-0.6.102/google/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/google/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.568293 modelaapi-0.6.102/google/api/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/google/api/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1580 2023-06-01 21:27:56.000000 modelaapi-0.6.102/google/api/annotations_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-06-01 21:27:56.000000 modelaapi-0.6.102/google/api/annotations_pb2_grpc.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     2125 2023-06-01 21:27:56.000000 modelaapi-0.6.102/google/api/http_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-06-01 21:27:56.000000 modelaapi-0.6.102/google/api/http_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.568293 modelaapi-0.6.102/k8s/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.568293 modelaapi-0.6.102/k8s/io/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.568293 modelaapi-0.6.102/k8s/io/api/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/api/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.568293 modelaapi-0.6.102/k8s/io/api/apps/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/api/apps/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.568293 modelaapi-0.6.102/k8s/io/api/apps/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/api/apps/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13162 2023-06-01 21:27:56.000000 modelaapi-0.6.102/k8s/io/api/apps/v1/generated_pb2.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.568293 modelaapi-0.6.102/k8s/io/api/core/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/api/core/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.572293 modelaapi-0.6.102/k8s/io/api/core/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/api/core/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    88069 2023-06-01 21:27:56.000000 modelaapi-0.6.102/k8s/io/api/core/v1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/api/core/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.572293 modelaapi-0.6.102/k8s/io/api/rbac/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/api/rbac/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.572293 modelaapi-0.6.102/k8s/io/api/rbac/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/api/rbac/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4882 2023-06-01 21:27:56.000000 modelaapi-0.6.102/k8s/io/api/rbac/v1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/api/rbac/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.572293 modelaapi-0.6.102/k8s/io/apimachinery/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/apimachinery/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.572293 modelaapi-0.6.102/k8s/io/apimachinery/pkg/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.572293 modelaapi-0.6.102/k8s/io/apimachinery/pkg/api/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/api/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.572293 modelaapi-0.6.102/k8s/io/apimachinery/pkg/api/resource/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/api/resource/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1329 2023-06-01 21:27:56.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/api/resource/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.572293 modelaapi-0.6.102/k8s/io/apimachinery/pkg/apis/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/apis/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.572293 modelaapi-0.6.102/k8s/io/apimachinery/pkg/apis/meta/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/apis/meta/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.572293 modelaapi-0.6.102/k8s/io/apimachinery/pkg/apis/meta/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/apis/meta/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14127 2023-06-01 21:27:56.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.572293 modelaapi-0.6.102/k8s/io/apimachinery/pkg/runtime/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/runtime/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1636 2023-06-01 21:27:56.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/runtime/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/runtime/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.576294 modelaapi-0.6.102/k8s/io/apimachinery/pkg/runtime/schema/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/runtime/schema/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1085 2023-06-01 21:27:56.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.576294 modelaapi-0.6.102/k8s/io/apimachinery/pkg/util/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/util/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.576294 modelaapi-0.6.102/k8s/io/apimachinery/pkg/util/intstr/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/util/intstr/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1268 2023-06-01 21:27:56.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.102/k8s/io/apimachinery/pkg/util/intstr/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.576294 modelaapi-0.6.102/modelaapi/
--rw-rw-r--   0 liam      (1000) liam      (1000)      257 2023-01-26 17:46:09.000000 modelaapi-0.6.102/modelaapi/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    62657 2023-01-26 17:46:09.000000 modelaapi-0.6.102/modelaapi/consts.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10291 2023-01-26 17:46:09.000000 modelaapi-0.6.102/modelaapi/custom_transformers.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14165 2023-01-26 17:46:09.000000 modelaapi-0.6.102/modelaapi/graykite_model.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    25394 2023-01-26 17:46:09.000000 modelaapi-0.6.102/modelaapi/ts.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1129 2023-06-01 21:52:29.000000 modelaapi-0.6.102/modelaapi/version.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-06-01 21:52:40.580294 modelaapi-0.6.102/modelaapi.egg-info/
--rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-06-01 21:52:40.000000 modelaapi-0.6.102/modelaapi.egg-info/PKG-INFO
--rw-rw-r--   0 liam      (1000) liam      (1000)    19381 2023-06-01 21:52:40.000000 modelaapi-0.6.102/modelaapi.egg-info/SOURCES.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-06-01 21:52:40.000000 modelaapi-0.6.102/modelaapi.egg-info/dependency_links.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)       20 2023-06-01 21:52:40.000000 modelaapi-0.6.102/modelaapi.egg-info/entry_points.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-02-27 17:39:16.000000 modelaapi-0.6.102/modelaapi.egg-info/not-zip-safe
--rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-06-01 21:52:40.000000 modelaapi-0.6.102/modelaapi.egg-info/requires.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)       28 2023-06-01 21:52:40.000000 modelaapi-0.6.102/modelaapi.egg-info/top_level.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-01-26 17:46:09.000000 modelaapi-0.6.102/requirements.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)      790 2023-06-01 21:52:40.580294 modelaapi-0.6.102/setup.cfg
--rw-rw-r--   0 liam      (1000) liam      (1000)     5349 2023-02-27 17:33:55.000000 modelaapi-0.6.102/setup.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.203844 modelaapi-0.6.200/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      139 2023-01-26 17:46:09.000000 modelaapi-0.6.200/AUTHORS.rst
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3579 2023-01-26 17:46:09.000000 modelaapi-0.6.200/CONTRIBUTING.rst
+-rw-rw-r--   0 liam      (1000) liam      (1000)        0 2023-01-26 17:46:09.000000 modelaapi-0.6.200/DESCRIPTION.md
+-rw-rw-r--   0 liam      (1000) liam      (1000)       89 2023-01-26 17:46:09.000000 modelaapi-0.6.200/HISTORY.rst
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11351 2023-01-26 17:46:09.000000 modelaapi-0.6.200/LICENSE.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)      437 2023-01-26 17:46:09.000000 modelaapi-0.6.200/MANIFEST.in
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1047 2023-01-26 17:46:09.000000 modelaapi-0.6.200/Makefile
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-07-05 17:57:48.203844 modelaapi-0.6.200/PKG-INFO
+-rw-rw-r--   0 liam      (1000) liam      (1000)      762 2023-01-26 17:46:09.000000 modelaapi-0.6.200/README.md
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.175843 modelaapi-0.6.200/github/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.175843 modelaapi-0.6.200/github/com/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.175843 modelaapi-0.6.200/github/com/gogo/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/gogo/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.175843 modelaapi-0.6.200/github/com/gogo/protobuf/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/gogo/protobuf/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.175843 modelaapi-0.6.200/github/com/gogo/protobuf/gogoproto/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/gogo/protobuf/gogoproto/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14416 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/gogo/protobuf/gogoproto/gogo_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/gogo/protobuf/gogoproto/gogo_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.175843 modelaapi-0.6.200/github/com/metaprov/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.175843 modelaapi-0.6.200/github/com/metaprov/modelaapi/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.175843 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.175843 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.175843 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/catalog/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/catalog/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.175843 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    23368 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.175843 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/data/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/data/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.175843 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    51127 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.175843 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/inference/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/inference/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.175843 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    23177 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.175843 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/infra/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/infra/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.179843 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24999 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.179843 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/team/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/team/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.179843 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11918 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.179843 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/training/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/training/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.179843 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    56923 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.179843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.179843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/account/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/account/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.179843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/account/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/account/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11310 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24380 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.179843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/alert/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/alert/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.179843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/alert/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/alert/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7196 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11335 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.179843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/attachment/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/attachment/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.179843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/attachment/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/attachment/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7919 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.179843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/batchpredictord/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/batchpredictord/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.179843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/batchpredictord/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/batchpredictord/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7549 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7751 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.179843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/catalog/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/catalog/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.179843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/catalog/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/catalog/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19189 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    33508 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.179843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/cloudproxyd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/cloudproxyd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.179843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/cloudproxyd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/cloudproxyd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6226 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    18211 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.179843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/commit/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/commit/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.179843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/commit/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/commit/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14479 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11490 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.179843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/common/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/common/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.179843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/common/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/common/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14189 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/common/v1/common_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.179843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/connection/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/connection/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.179843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/connection/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/connection/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8826 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14287 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.179843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/conversation/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/conversation/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.183843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/conversation/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/conversation/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    31897 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.183843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/data/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/data/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.183843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/data/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/data/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    77258 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)   111042 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.183843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dataapp/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dataapp/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.183843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dataapp/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dataapp/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9057 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    17941 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.183843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/datapipeline/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/datapipeline/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.183843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/datapipeline/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/datapipeline/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8161 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14642 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.183843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/datapipelinerun/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/datapipelinerun/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.183843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/datapipelinerun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/datapipelinerun/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10253 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19897 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.183843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dataproduct/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dataproduct/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.183843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dataproduct/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dataproduct/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8425 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12265 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.183843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dataproductversion/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dataproductversion/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.183843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dataproductversion/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dataproductversion/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8095 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13350 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.183843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dataset/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dataset/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.183843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dataset/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dataset/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19016 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    35095 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.183843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/datasource/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/datasource/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.183843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/datasource/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/datasource/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9636 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    16324 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.183843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dbproxyd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dbproxyd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.183843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dbproxyd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dbproxyd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    78210 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)   348679 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.183843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/entity/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/entity/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.183843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/entity/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/entity/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6605 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11503 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.183843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/featuregroup/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/featuregroup/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.187843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/featuregroup/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/featuregroup/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10534 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    21293 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.187843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/featurehistogram/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/featurehistogram/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.187843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/featurehistogram/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/featurehistogram/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7606 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13040 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.187843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/fileservices/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/fileservices/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.187843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/fileservices/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/fileservices/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3038 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3345 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.187843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/grpcinferenceservice/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/grpcinferenceservice/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.187843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    18564 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24869 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.187843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/k8score/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/k8score/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.187843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/k8score/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/k8score/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    20839 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    26279 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.187843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/lab/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/lab/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.187843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/lab/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/lab/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6886 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11025 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.187843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/license/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/license/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.187843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/license/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/license/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8088 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13831 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.187843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/model/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/model/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.187843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/model/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/model/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    20626 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    44447 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.187843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/modelasystem/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/modelasystem/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.187843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/modelasystem/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/modelasystem/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4690 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7755 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.187843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/modelclass/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/modelclass/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.187843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/modelclass/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/modelclass/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10011 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    18664 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.187843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/modeldsystem/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/modeldsystem/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.187843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/modeldsystem/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/modeldsystem/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.187843 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/notifier/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/notifier/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.191844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/notifier/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/notifier/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7054 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11800 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.191844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/objectstored/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/objectstored/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.191844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/objectstored/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/objectstored/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3626 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9814 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.191844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/offlinefeaturestored/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/offlinefeaturestored/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.191844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3276 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5855 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.191844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/onlinefeaturestored/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/onlinefeaturestored/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.191844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5036 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5675 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.191844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/postmortem/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/postmortem/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.191844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/postmortem/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/postmortem/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6924 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.191844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/prediction/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/prediction/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.191844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/prediction/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/prediction/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8637 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    16389 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.191844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/predictionstore/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/predictionstore/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.191844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/predictionstore/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/predictionstore/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2824 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3486 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.191844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/predictor/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/predictor/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.191844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/predictor/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/predictor/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9068 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    16147 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.191844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/publisherd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/publisherd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.191844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/publisherd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/publisherd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7197 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7539 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.191844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/recipe/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/recipe/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.191844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/recipe/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/recipe/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8686 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    15629 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.191844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/reciperun/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/reciperun/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.191844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/reciperun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/reciperun/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6809 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11955 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.191844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/report/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/report/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.191844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/report/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/report/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7381 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13561 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.195844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/review/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/review/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.195844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/review/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/review/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7474 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.195844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/runbook/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/runbook/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.195844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/runbook/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/runbook/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6596 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11645 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.195844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/servingsite/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/servingsite/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.195844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/servingsite/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/servingsite/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7910 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14432 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.195844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/sqlquery/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/sqlquery/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.195844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/sqlquery/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/sqlquery/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13739 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13906 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.195844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/sqlqueryrun/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/sqlqueryrun/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.195844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14535 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14465 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.195844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/study/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/study/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.195844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/study/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/study/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11657 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    23824 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.195844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/system/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/system/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.195844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/system/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/system/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14859 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7442 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.195844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/tenant/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/tenant/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.195844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/tenant/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/tenant/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9747 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    15755 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.195844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/todo/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/todo/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.195844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/todo/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/todo/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6407 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11180 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.195844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/trainerd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/trainerd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.195844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/trainerd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/trainerd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13701 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13516 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.195844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/userroleclass/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/userroleclass/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.195844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/userroleclass/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/userroleclass/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8160 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12588 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.195844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/virtualbucket/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/virtualbucket/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.199844 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/virtualbucket/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/virtualbucket/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7168 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12575 2023-07-05 16:51:13.000000 modelaapi-0.6.200/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.199844 modelaapi-0.6.200/google/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.200/google/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.199844 modelaapi-0.6.200/google/api/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.200/google/api/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1580 2023-07-05 16:51:13.000000 modelaapi-0.6.200/google/api/annotations_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-05 16:51:13.000000 modelaapi-0.6.200/google/api/annotations_pb2_grpc.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2125 2023-07-05 16:51:13.000000 modelaapi-0.6.200/google/api/http_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-05 16:51:13.000000 modelaapi-0.6.200/google/api/http_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.199844 modelaapi-0.6.200/k8s/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.200/k8s/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.199844 modelaapi-0.6.200/k8s/io/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.200/k8s/io/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.199844 modelaapi-0.6.200/k8s/io/api/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.200/k8s/io/api/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.199844 modelaapi-0.6.200/k8s/io/api/apps/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.200/k8s/io/api/apps/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.199844 modelaapi-0.6.200/k8s/io/api/apps/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.200/k8s/io/api/apps/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13162 2023-07-05 16:51:13.000000 modelaapi-0.6.200/k8s/io/api/apps/v1/generated_pb2.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.199844 modelaapi-0.6.200/k8s/io/api/core/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.200/k8s/io/api/core/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.199844 modelaapi-0.6.200/k8s/io/api/core/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.200/k8s/io/api/core/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    88069 2023-07-05 16:51:13.000000 modelaapi-0.6.200/k8s/io/api/core/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.200/k8s/io/api/core/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.199844 modelaapi-0.6.200/k8s/io/api/rbac/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.200/k8s/io/api/rbac/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.199844 modelaapi-0.6.200/k8s/io/api/rbac/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.200/k8s/io/api/rbac/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4882 2023-07-05 16:51:13.000000 modelaapi-0.6.200/k8s/io/api/rbac/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.200/k8s/io/api/rbac/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.199844 modelaapi-0.6.200/k8s/io/apimachinery/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.200/k8s/io/apimachinery/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.199844 modelaapi-0.6.200/k8s/io/apimachinery/pkg/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.200/k8s/io/apimachinery/pkg/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.199844 modelaapi-0.6.200/k8s/io/apimachinery/pkg/api/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.200/k8s/io/apimachinery/pkg/api/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.199844 modelaapi-0.6.200/k8s/io/apimachinery/pkg/api/resource/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.200/k8s/io/apimachinery/pkg/api/resource/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1329 2023-07-05 16:51:13.000000 modelaapi-0.6.200/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.200/k8s/io/apimachinery/pkg/api/resource/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.199844 modelaapi-0.6.200/k8s/io/apimachinery/pkg/apis/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.200/k8s/io/apimachinery/pkg/apis/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.199844 modelaapi-0.6.200/k8s/io/apimachinery/pkg/apis/meta/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.200/k8s/io/apimachinery/pkg/apis/meta/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.199844 modelaapi-0.6.200/k8s/io/apimachinery/pkg/apis/meta/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.200/k8s/io/apimachinery/pkg/apis/meta/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14127 2023-07-05 16:51:13.000000 modelaapi-0.6.200/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.200/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.199844 modelaapi-0.6.200/k8s/io/apimachinery/pkg/runtime/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.200/k8s/io/apimachinery/pkg/runtime/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1636 2023-07-05 16:51:13.000000 modelaapi-0.6.200/k8s/io/apimachinery/pkg/runtime/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.200/k8s/io/apimachinery/pkg/runtime/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.199844 modelaapi-0.6.200/k8s/io/apimachinery/pkg/runtime/schema/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.200/k8s/io/apimachinery/pkg/runtime/schema/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1085 2023-07-05 16:51:13.000000 modelaapi-0.6.200/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.200/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.199844 modelaapi-0.6.200/k8s/io/apimachinery/pkg/util/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.200/k8s/io/apimachinery/pkg/util/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.199844 modelaapi-0.6.200/k8s/io/apimachinery/pkg/util/intstr/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.200/k8s/io/apimachinery/pkg/util/intstr/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1268 2023-07-05 16:51:13.000000 modelaapi-0.6.200/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.200/k8s/io/apimachinery/pkg/util/intstr/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.203844 modelaapi-0.6.200/modelaapi/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      257 2023-01-26 17:46:09.000000 modelaapi-0.6.200/modelaapi/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    62657 2023-01-26 17:46:09.000000 modelaapi-0.6.200/modelaapi/consts.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10291 2023-01-26 17:46:09.000000 modelaapi-0.6.200/modelaapi/custom_transformers.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14165 2023-01-26 17:46:09.000000 modelaapi-0.6.200/modelaapi/graykite_model.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    25394 2023-01-26 17:46:09.000000 modelaapi-0.6.200/modelaapi/ts.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1129 2023-07-05 17:56:37.000000 modelaapi-0.6.200/modelaapi/version.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-05 17:57:48.203844 modelaapi-0.6.200/modelaapi.egg-info/
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-07-05 17:57:48.000000 modelaapi-0.6.200/modelaapi.egg-info/PKG-INFO
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19381 2023-07-05 17:57:48.000000 modelaapi-0.6.200/modelaapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-07-05 17:57:48.000000 modelaapi-0.6.200/modelaapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)       20 2023-07-05 17:57:48.000000 modelaapi-0.6.200/modelaapi.egg-info/entry_points.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-02-27 17:39:16.000000 modelaapi-0.6.200/modelaapi.egg-info/not-zip-safe
+-rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-07-05 17:57:48.000000 modelaapi-0.6.200/modelaapi.egg-info/requires.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)       28 2023-07-05 17:57:48.000000 modelaapi-0.6.200/modelaapi.egg-info/top_level.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-01-26 17:46:09.000000 modelaapi-0.6.200/requirements.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)      790 2023-07-05 17:57:48.203844 modelaapi-0.6.200/setup.cfg
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5349 2023-02-27 17:33:55.000000 modelaapi-0.6.200/setup.py
```

### Comparing `modelaapi-0.6.102/CONTRIBUTING.rst` & `modelaapi-0.6.200/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/LICENSE.txt` & `modelaapi-0.6.200/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/Makefile` & `modelaapi-0.6.200/Makefile`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/PKG-INFO` & `modelaapi-0.6.200/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: modelaapi
-Version: 0.6.102
+Version: 0.6.200
 Summary: A suite of automatic machine learning for kubernetes
 Home-page: http://www.modela.ai
 Author: The modelaapi developers
 Author-email: info@modela.ai
 Maintainer: The modela developers
 Maintainer-email: info@modela.ai
 License: Apache 2
-Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.102
+Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.200
 Project-URL: Documentation, http://www.modela.ai
-Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.102
+Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.200
 Project-URL: Source, https://github.com/metaprov/modelaapi
 Project-URL: Tracker, https://github.com/metaprov/modelaapi/issues
 Keywords: automl,machine learning,data science
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `modelaapi-0.6.102/README.md` & `modelaapi-0.6.200/README.md`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/gogo/protobuf/gogoproto/gogo_pb2.py` & `modelaapi-0.6.200/github/com/gogo/protobuf/gogoproto/gogo_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from k8s.io.api.core.v1 import generated_pb2 as k8s_dot_io_dot_api_dot_core_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.api.resource import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_api_dot_resource_dot_generated__pb2
 from k8s.io.apimachinery.pkg.apis.meta.v1 import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_apis_dot_meta_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime.schema import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_schema_dot_generated__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x12\x37github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/api/resource/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\xae\x01\n\nAccessSpec\x12\x0c\n\x04port\x18\x01 \x01(\x05\x12\x10\n\x08nodePort\x18\x02 \x01(\x05\x12\x0c\n\x04path\x18\x03 \x01(\t\x12\x12\n\naccessType\x18\x04 \x01(\t\x12\x0c\n\x04rest\x18\x05 \x01(\x08\x12\x12\n\nauthMethod\x18\x06 \x01(\t\x12<\n\x0f\x61pikeySecretRef\x18\x07 \x01(\x0b\x32#.k8s.io.api.core.v1.SecretReference\"b\n\x12\x41\x63\x63ountPermissions\x12\x13\n\x0b\x61\x63\x63ountName\x18\x01 \x01(\t\x12\x37\n\x05roles\x18\x02 \x03(\x0b\x32(.k8s.io.api.core.v1.LocalObjectReference\"\xa5\x01\n\tAlgorithm\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12T\n\x04spec\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AlgorithmSpec\"\xa4\x01\n\rAlgorithmList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Q\n\x05items\x18\x02 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"\xc0\x01\n\rAlgorithmSpec\x12\x15\n\rframeworkName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\r\n\x05tasks\x18\x04 \x03(\t\x12\x0e\n\x06sparse\x18\x05 \x01(\x08\x12W\n\x06ranges\x18\x06 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ParameterRange\"\xf3\x01\n\x05\x43loud\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12P\n\x04spec\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CloudSpec\x12T\n\x06status\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CloudStatus\"\x9c\x01\n\tCloudList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12M\n\x05items\x18\x02 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Cloud\"\xec\x02\n\tCloudSpec\x12\x19\n\x11\x64\x65\x66\x61ultRegionName\x18\x01 \x01(\t\x12\x1f\n\x17\x64\x65\x66\x61ultMachineClassName\x18\x02 \x01(\t\x12\x1b\n\x13\x64\x65\x66\x61ultGpuClassName\x18\x03 \x01(\t\x12]\n\x0emachineClasses\x18\x04 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.MachineClass\x12U\n\ngpuClasses\x18\x05 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.GpuClass\x12P\n\x07regions\x18\x06 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Region\"\xc7\x01\n\x0b\x43loudStatus\x12_\n\x0cmachineCosts\x18\x01 \x03(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.MachineClassCost\x12W\n\x08gpuCosts\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.GpuClassCost\"A\n\x0c\x43ompilerSpec\x12\x0e\n\x06\x65nable\x18\x01 \x01(\x08\x12\x10\n\x08\x63ompiler\x18\x02 \x01(\t\x12\x0f\n\x07targets\x18\x03 \x03(\t\"l\n\x0f\x43onfusionMatrix\x12Y\n\x04rows\x18\x01 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrixRow\"F\n\x12\x43onfusionMatrixRow\x12\t\n\x01t\x18\x01 \x01(\t\x12\t\n\x01p\x18\x02 \x01(\t\x12\r\n\x05\x63ount\x18\x03 \x01(\x05\x12\x0b\n\x03pct\x18\x04 \x01(\x01\"K\n\x0c\x43ontainerLog\x12\x0b\n\x03job\x18\x01 \x01(\t\x12\x11\n\tcontainer\x18\x02 \x01(\t\x12\x0b\n\x03key\x18\x03 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x04 \x01(\t\"\"\n\nCurvePoint\x12\t\n\x01x\x18\x01 \x01(\x01\x12\t\n\x01y\x18\x02 \x01(\x01\"(\n\nDataCenter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\"\xda\x01\n\x0c\x44\x61taLocation\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x16\n\x0e\x63onnectionName\x18\x02 \x01(\t\x12\x12\n\nbucketName\x18\x03 \x01(\t\x12\x0c\n\x04path\x18\x04 \x01(\t\x12\r\n\x05table\x18\x05 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x06 \x01(\t\x12\x0b\n\x03sql\x18\x07 \x01(\t\x12\r\n\x05topic\x18\x08 \x01(\t\x12\x0b\n\x03url\x18\t \x01(\t\x12\x38\n\x0bresourceRef\x18\n \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\xc5\x04\n\x0c\x44\x61taTestCase\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x12\n\nassertThat\x18\x03 \x01(\t\x12\x36\n\tentityRef\x18\x04 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x39\n\x0c\x63ompareToRef\x18\x05 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0e\n\x06\x63olumn\x18\x06 \x01(\t\x12\x0c\n\x04type\x18\x07 \x01(\t\x12\x0e\n\x06metric\x18\x08 \x01(\t\x12\x15\n\rexpectedValue\x18\t \x01(\x01\x12\x18\n\x10\x65xpectedCategory\x18\n \x01(\t\x12\r\n\x05lower\x18\x0b \x01(\x01\x12\r\n\x05upper\x18\x0c \x01(\x01\x12\x13\n\x0b\x65xpectedSet\x18\r \x03(\t\x12\x16\n\x0elowerInclusive\x18\x0e \x01(\x08\x12\x16\n\x0eupperInclusive\x18\x0f \x01(\x08\x12\x11\n\tgenerated\x18\x10 \x01(\x08\x12\x0c\n\x04tags\x18\x11 \x03(\t\x12\x0f\n\x07\x63olumn2\x18\x12 \x01(\t\x12\x37\n\nentityRef2\x18\x13 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0f\n\x07\x63olumns\x18\x14 \x03(\t\x12\x15\n\rfeatureFilter\x18\x15 \x01(\t\x12\x12\n\ndataFilter\x18\x16 \x01(\t\x12\x15\n\rreferenceType\x18\x17 \x01(\t\x12\x0f\n\x07periods\x18\x18 \x01(\x05\"\xac\x01\n\x12\x44\x61taTestCaseResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12T\n\x06\x61\x63tual\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12\x0f\n\x07\x66\x61ilure\x18\x03 \x01(\x08\x12\r\n\x05\x65rror\x18\x04 \x01(\x08\x12\x12\n\nfailureMsg\x18\x05 \x01(\t\"0\n\x0c\x46ileLocation\x12\x12\n\nbucketName\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"t\n\x0cGithubEvents\x12\x19\n\x11gitConnectionName\x18\x01 \x01(\t\x12\x12\n\nrepository\x18\x02 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x03 \x01(\t\x12\x15\n\rblobNameRegex\x18\x04 \x01(\t\x12\x0e\n\x06\x65vents\x18\x05 \x03(\t\"z\n\x08GpuClass\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x12\n\nregionName\x18\x02 \x01(\t\x12\x0c\n\x04vcpu\x18\x03 \x01(\x05\x12>\n\x06gpumem\x18\x04 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\"\xb5\x01\n\x0cGpuClassCost\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\x45\n\rcostPerMinute\x18\x03 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\x12@\n\x08\x63ostSpot\x18\x04 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\"c\n\rHistogramData\x12\x0c\n\x04\x62ins\x18\x01 \x03(\x01\x12\x12\n\ncategories\x18\x02 \x03(\t\x12\x0e\n\x06\x63ounts\x18\x03 \x03(\x01\x12\x0f\n\x07missing\x18\x04 \x01(\x05\x12\x0f\n\x07invalid\x18\x05 \x01(\x05\"I\n\x06Images\x12\x14\n\x0ctrainerImage\x18\x01 \x01(\t\x12\x11\n\tdataImage\x18\x02 \x01(\t\x12\x16\n\x0epublisherImage\x18\x03 \x01(\t\"\xaf\x01\n\rLastRunStatus\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12?\n\x0b\x63ompletedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x10\n\x08\x64uration\x18\x04 \x01(\x05\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\"*\n\x03Lib\x12\x12\n\nframeworks\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"q\n\x04Logs\x12\x0e\n\x06\x62ucket\x18\x01 \x01(\t\x12Y\n\ncontainers\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ContainerLog\"\xa9\x01\n\x0bMLFramework\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.MLFrameworkSpec\"\xa8\x01\n\x0fMLFrameworkList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.MLFramework\"R\n\x0fMLFrameworkSpec\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x0c\n\x04lang\x18\x04 \x01(\t\"\x8c\x01\n\x0cMachineClass\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x12\n\nregionName\x18\x02 \x01(\t\x12;\n\x03mem\x18\x03 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\x12\x0c\n\x04vcpu\x18\x04 \x01(\x05\x12\x0f\n\x07storage\x18\x05 \x01(\t\"\xb9\x01\n\x10MachineClassCost\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\x45\n\rcostPerMinute\x18\x03 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\x12@\n\x08\x63ostSpot\x18\x04 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\"\xab\x01\n\x0cManagedImage\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12W\n\x04spec\x18\x02 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ManagedImageSpec\"\xaa\x01\n\x10ManagedImageList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12T\n\x05items\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ManagedImage\"\xbb\x03\n\x10ManagedImageSpec\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12\x10\n\x08registry\x18\x02 \x01(\t\x12\x12\n\nrepository\x18\x03 \x01(\t\x12\x0b\n\x03tag\x18\x04 \x01(\t\x12\'\n\x03\x65nv\x18\x05 \x03(\x0b\x32\x1a.k8s.io.api.core.v1.EnvVar\x12\x0b\n\x03gpu\x18\x06 \x01(\x08\x12\x0e\n\x06\x61\x63tive\x18\x07 \x01(\x08\x12\x0f\n\x07preload\x18\x08 \x01(\x08\x12:\n\rconnectionRef\x18\t \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0c\n\x04\x62\x61se\x18\n \x01(\t\x12\x0c\n\x04role\x18\x0b \x01(\t\x12\x13\n\x0bmantainedBy\x18\x0c \x01(\t\x12\x0b\n\x03uri\x18\r \x01(\t\x12\x12\n\nframeworks\x18\x0e \x03(\t\x12J\n\x04libs\x18\x0f \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Lib\x12\n\n\x02os\x18\x10 \x01(\t\x12\x11\n\tosVersion\x18\x11 \x01(\t\x12\x0f\n\x07private\x18\x12 \x01(\x08\"\x9a\x02\n\x0bMeasurement\x12\x33\n\x06\x65ntity\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0e\n\x06\x63olumn\x18\x02 \x01(\t\x12\x0e\n\x06metric\x18\x03 \x01(\t\x12\r\n\x05value\x18\x04 \x01(\x01\x12\x0e\n\x06stddev\x18\x05 \x01(\x01\x12\x0f\n\x07\x62oolQty\x18\x06 \x01(\x08\x12\x10\n\x08\x63\x61tegory\x18\x07 \x01(\t\x12\x10\n\x08valueSet\x18\x08 \x03(\t\x12=\n\ttimePoint\x18\t \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x10\n\x08taskType\x18\n \x01(\t\x12\x11\n\talgorithm\x18\x0b \x01(\t\"\xb3\x02\n\x13ModelDeploymentSpec\x12\x35\n\x08modelRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\x14\n\x0cmodelVersion\x18\x03 \x01(\t\x12\x0f\n\x07traffic\x18\x04 \x01(\x05\x12\x0c\n\x04role\x18\x05 \x01(\t\x12\x10\n\x08mountTar\x18\t \x01(\x08\x12\x17\n\x0ftrafficSelector\x18\n \x01(\t\x12\x37\n\napprovedBy\x18\x0c \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12>\n\napprovedAt\x18\r \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"\xea\x01\n\x10NotificationSpec\x12\x10\n\x08\x65rrorTTL\x18\x02 \x01(\x05\x12\x12\n\nsuccessTTL\x18\x04 \x01(\x05\x12\x14\n\x0cnotifierName\x18\x05 \x01(\t\x12i\n\x08selector\x18\x06 \x03(\x0b\x32W.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec.SelectorEntry\x1a/\n\rSelectorEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"-\n\rObjectiveSpec\x12\x0e\n\x06metric\x18\x01 \x01(\t\x12\x0c\n\x04goal\x18\x02 \x01(\t\"^\n\x07PRCurve\x12S\n\x06values\x18\x01 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CurvePoint\"\x93\x02\n\x0eParameterRange\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0b\n\x03low\x18\x03 \x01(\x01\x12\x0c\n\x04high\x18\x04 \x01(\x01\x12\x0c\n\x04step\x18\x05 \x01(\x05\x12\x0b\n\x03log\x18\x06 \x01(\x08\x12\x0f\n\x07\x63hoices\x18\x07 \x03(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x08 \x01(\x01\x12\x15\n\rdefaultChoice\x18\t \x01(\t\x12\x13\n\x0b\x63onditional\x18\n \x01(\x08\x12\x0e\n\x06parent\x18\x0b \x01(\t\x12\x16\n\x0eparentValueCat\x18\x0c \x01(\t\x12\x1a\n\x12parentValueInteger\x18\r \x01(\x05\x12\x18\n\x10parentValueFloat\x18\x0e \x01(\x01\"p\n\x0fPermissionsSpec\x12]\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccountPermissions\"\xb1\x01\n\x0fPretrainedModel\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Z\n\x04spec\x18\x02 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PretrainedModelSpec\"\xb0\x01\n\x13PretrainedModelList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12W\n\x05items\x18\x02 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PretrainedModel\"$\n\x13PretrainedModelSpec\x12\r\n\x05image\x18\x01 \x01(\t\"\xad\x01\n\rPublicDataset\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12X\n\x04spec\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PublicDatasetSpec\"\xac\x01\n\x11PublicDatasetList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12U\n\x05items\x18\x02 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PublicDataset\"\xb6\x02\n\x11PublicDatasetSpec\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0c\n\x04task\x18\x03 \x01(\t\x12\x10\n\x08openMLID\x18\x04 \x01(\t\x12\x0f\n\x07\x64\x61taUrl\x18\x05 \x01(\t\x12\x10\n\x08\x63itation\x18\x06 \x01(\t\x12\x0c\n\x04rows\x18\x07 \x01(\x05\x12\x0f\n\x07\x63olumns\x18\x08 \x01(\x05\x12\x10\n\x08\x66ileSize\x18\t \x01(\x05\x12\x14\n\x0ctargetColumn\x18\n \x01(\t\x12\x10\n\x08industry\x18\x0b \x01(\t\x12\x12\n\nimbalanced\x18\x0c \x01(\x08\x12\x14\n\x0c\x64\x61tasourceCR\x18\r \x01(\t\x12\x11\n\tdatasetCR\x18\x0e \x01(\t\x12\x0f\n\x07studyCR\x18\x0f \x01(\t\x12\x15\n\rdataProductCR\x18\x10 \x01(\t\"\xb6\x01\n\x06Region\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x1d\n\x15\x64\x65\x66\x61ultDatacenterName\x18\x02 \x01(\t\x12\x10\n\x08location\x18\x03 \x01(\t\x12\x13\n\x0b\x62illingCode\x18\x04 \x01(\t\x12X\n\x0b\x64\x61tacenters\x18\x05 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataCenter\"?\n\x13ResourceConsumption\x12\x0b\n\x03\x63pu\x18\x01 \x01(\x04\x12\x0e\n\x06memory\x18\x02 \x01(\x04\x12\x0b\n\x03gpu\x18\x03 \x01(\x04\"t\n\x0cResourceSpec\x12\x14\n\x0cworkloadName\x18\x01 \x01(\t\x12\x0e\n\x06\x63ustom\x18\x02 \x01(\x08\x12>\n\x0crequirements\x18\x03 \x01(\x0b\x32(.k8s.io.api.core.v1.ResourceRequirements\"b\n\x0bRocAucCurve\x12S\n\x06values\x18\x01 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CurvePoint\"\xcd\x01\n\x0bRunSchedule\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04\x63ron\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x15\n\rmaxRetryCount\x18\x04 \x01(\x05\x12\x15\n\rretryDelaySec\x18\x05 \x01(\x05\x12\x12\n\ntimeoutSec\x18\x06 \x01(\x05\x12\x10\n\x08timezone\x18\x07 \x01(\t\x12=\n\tnextRunAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"\xfe\x01\n\x11RunScheduleStatus\x12=\n\tlastRunAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x02 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x03 \x01(\t\x12\x13\n\x0blastRunName\x18\x04 \x01(\t\x12R\n\x0blastRunLogs\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12\x12\n\nretryCount\x18\x06 \x01(\x05\"r\n\tTestSuite\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12T\n\x05tests\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataTestCase\"\xc7\x02\n\x0fTestSuiteResult\x12\x36\n\tentityRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08\x66\x61ilures\x18\x02 \x01(\x05\x12\x0e\n\x06\x65rrors\x18\x03 \x01(\x05\x12=\n\tstartedAt\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12Z\n\x05tests\x18\x06 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataTestCaseResult\"G\n\x0fWorkerRunResult\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0b\n\x03uri\x18\x02 \x01(\t\x12\x0c\n\x04task\x18\x03 \x01(\t\x12\r\n\x05\x65rror\x18\x04 \x01(\t\"\xad\x01\n\rWorkloadClass\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12X\n\x04spec\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkloadClassSpec\"\xac\x01\n\x11WorkloadClassList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12U\n\x05items\x18\x02 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkloadClass\"u\n\x11WorkloadClassSpec\x12`\n\x11resourcesTemplate\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpecB9Z7github.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x12\x37github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/api/resource/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\xae\x01\n\nAccessSpec\x12\x0c\n\x04port\x18\x01 \x01(\x05\x12\x10\n\x08nodePort\x18\x02 \x01(\x05\x12\x0c\n\x04path\x18\x03 \x01(\t\x12\x12\n\naccessType\x18\x04 \x01(\t\x12\x0c\n\x04http\x18\x05 \x01(\x08\x12\x12\n\nauthMethod\x18\x06 \x01(\t\x12<\n\x0f\x61pikeySecretRef\x18\x07 \x01(\x0b\x32#.k8s.io.api.core.v1.SecretReference\"b\n\x12\x41\x63\x63ountPermissions\x12\x13\n\x0b\x61\x63\x63ountName\x18\x01 \x01(\t\x12\x37\n\x05roles\x18\x02 \x03(\x0b\x32(.k8s.io.api.core.v1.LocalObjectReference\"\xa5\x01\n\tAlgorithm\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12T\n\x04spec\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AlgorithmSpec\"\xa4\x01\n\rAlgorithmList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Q\n\x05items\x18\x02 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"\xc0\x01\n\rAlgorithmSpec\x12\x15\n\rframeworkName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\r\n\x05tasks\x18\x04 \x03(\t\x12\x0e\n\x06sparse\x18\x05 \x01(\x08\x12W\n\x06ranges\x18\x06 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ParameterRange\"\xf3\x01\n\x05\x43loud\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12P\n\x04spec\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CloudSpec\x12T\n\x06status\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CloudStatus\"\x9c\x01\n\tCloudList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12M\n\x05items\x18\x02 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Cloud\"\xec\x02\n\tCloudSpec\x12\x19\n\x11\x64\x65\x66\x61ultRegionName\x18\x01 \x01(\t\x12\x1f\n\x17\x64\x65\x66\x61ultMachineClassName\x18\x02 \x01(\t\x12\x1b\n\x13\x64\x65\x66\x61ultGpuClassName\x18\x03 \x01(\t\x12]\n\x0emachineClasses\x18\x04 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.MachineClass\x12U\n\ngpuClasses\x18\x05 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.GpuClass\x12P\n\x07regions\x18\x06 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Region\"\xc7\x01\n\x0b\x43loudStatus\x12_\n\x0cmachineCosts\x18\x01 \x03(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.MachineClassCost\x12W\n\x08gpuCosts\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.GpuClassCost\"A\n\x0c\x43ompilerSpec\x12\x0e\n\x06\x65nable\x18\x01 \x01(\x08\x12\x10\n\x08\x63ompiler\x18\x02 \x01(\t\x12\x0f\n\x07targets\x18\x03 \x03(\t\"l\n\x0f\x43onfusionMatrix\x12Y\n\x04rows\x18\x01 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrixRow\"F\n\x12\x43onfusionMatrixRow\x12\t\n\x01t\x18\x01 \x01(\t\x12\t\n\x01p\x18\x02 \x01(\t\x12\r\n\x05\x63ount\x18\x03 \x01(\x05\x12\x0b\n\x03pct\x18\x04 \x01(\x01\"K\n\x0c\x43ontainerLog\x12\x0b\n\x03job\x18\x01 \x01(\t\x12\x11\n\tcontainer\x18\x02 \x01(\t\x12\x0b\n\x03key\x18\x03 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x04 \x01(\t\"\"\n\nCurvePoint\x12\t\n\x01x\x18\x01 \x01(\x01\x12\t\n\x01y\x18\x02 \x01(\x01\"(\n\nDataCenter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\"\xda\x01\n\x0c\x44\x61taLocation\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x16\n\x0e\x63onnectionName\x18\x02 \x01(\t\x12\x12\n\nbucketName\x18\x03 \x01(\t\x12\x0c\n\x04path\x18\x04 \x01(\t\x12\r\n\x05table\x18\x05 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x06 \x01(\t\x12\x0b\n\x03sql\x18\x07 \x01(\t\x12\r\n\x05topic\x18\x08 \x01(\t\x12\x0b\n\x03url\x18\t \x01(\t\x12\x38\n\x0bresourceRef\x18\n \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\xc5\x04\n\x0c\x44\x61taTestCase\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x12\n\nassertThat\x18\x03 \x01(\t\x12\x36\n\tentityRef\x18\x04 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x39\n\x0c\x63ompareToRef\x18\x05 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0e\n\x06\x63olumn\x18\x06 \x01(\t\x12\x0c\n\x04type\x18\x07 \x01(\t\x12\x0e\n\x06metric\x18\x08 \x01(\t\x12\x15\n\rexpectedValue\x18\t \x01(\x01\x12\x18\n\x10\x65xpectedCategory\x18\n \x01(\t\x12\r\n\x05lower\x18\x0b \x01(\x01\x12\r\n\x05upper\x18\x0c \x01(\x01\x12\x13\n\x0b\x65xpectedSet\x18\r \x03(\t\x12\x16\n\x0elowerInclusive\x18\x0e \x01(\x08\x12\x16\n\x0eupperInclusive\x18\x0f \x01(\x08\x12\x11\n\tgenerated\x18\x10 \x01(\x08\x12\x0c\n\x04tags\x18\x11 \x03(\t\x12\x0f\n\x07\x63olumn2\x18\x12 \x01(\t\x12\x37\n\nentityRef2\x18\x13 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0f\n\x07\x63olumns\x18\x14 \x03(\t\x12\x15\n\rfeatureFilter\x18\x15 \x01(\t\x12\x12\n\ndataFilter\x18\x16 \x01(\t\x12\x15\n\rreferenceType\x18\x17 \x01(\t\x12\x0f\n\x07periods\x18\x18 \x01(\x05\"\xac\x01\n\x12\x44\x61taTestCaseResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12T\n\x06\x61\x63tual\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12\x0f\n\x07\x66\x61ilure\x18\x03 \x01(\x08\x12\r\n\x05\x65rror\x18\x04 \x01(\x08\x12\x12\n\nfailureMsg\x18\x05 \x01(\t\"0\n\x0c\x46ileLocation\x12\x12\n\nbucketName\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"t\n\x0cGithubEvents\x12\x19\n\x11gitConnectionName\x18\x01 \x01(\t\x12\x12\n\nrepository\x18\x02 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x03 \x01(\t\x12\x15\n\rblobNameRegex\x18\x04 \x01(\t\x12\x0e\n\x06\x65vents\x18\x05 \x03(\t\"z\n\x08GpuClass\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x12\n\nregionName\x18\x02 \x01(\t\x12\x0c\n\x04vcpu\x18\x03 \x01(\x05\x12>\n\x06gpumem\x18\x04 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\"\xb5\x01\n\x0cGpuClassCost\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\x45\n\rcostPerMinute\x18\x03 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\x12@\n\x08\x63ostSpot\x18\x04 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\"c\n\rHistogramData\x12\x0c\n\x04\x62ins\x18\x01 \x03(\x01\x12\x12\n\ncategories\x18\x02 \x03(\t\x12\x0e\n\x06\x63ounts\x18\x03 \x03(\x01\x12\x0f\n\x07missing\x18\x04 \x01(\x05\x12\x0f\n\x07invalid\x18\x05 \x01(\x05\"I\n\x06Images\x12\x14\n\x0ctrainerImage\x18\x01 \x01(\t\x12\x11\n\tdataImage\x18\x02 \x01(\t\x12\x16\n\x0epublisherImage\x18\x03 \x01(\t\"\xaf\x01\n\rLastRunStatus\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12?\n\x0b\x63ompletedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x10\n\x08\x64uration\x18\x04 \x01(\x05\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\"*\n\x03Lib\x12\x12\n\nframeworks\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"q\n\x04Logs\x12\x0e\n\x06\x62ucket\x18\x01 \x01(\t\x12Y\n\ncontainers\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ContainerLog\"\xa9\x01\n\x0bMLFramework\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.MLFrameworkSpec\"\xa8\x01\n\x0fMLFrameworkList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.MLFramework\"R\n\x0fMLFrameworkSpec\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x0c\n\x04lang\x18\x04 \x01(\t\"\x8c\x01\n\x0cMachineClass\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x12\n\nregionName\x18\x02 \x01(\t\x12;\n\x03mem\x18\x03 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\x12\x0c\n\x04vcpu\x18\x04 \x01(\x05\x12\x0f\n\x07storage\x18\x05 \x01(\t\"\xb9\x01\n\x10MachineClassCost\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\x45\n\rcostPerMinute\x18\x03 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\x12@\n\x08\x63ostSpot\x18\x04 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\"\xab\x01\n\x0cManagedImage\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12W\n\x04spec\x18\x02 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ManagedImageSpec\"\xaa\x01\n\x10ManagedImageList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12T\n\x05items\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ManagedImage\"\xbb\x03\n\x10ManagedImageSpec\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12\x10\n\x08registry\x18\x02 \x01(\t\x12\x12\n\nrepository\x18\x03 \x01(\t\x12\x0b\n\x03tag\x18\x04 \x01(\t\x12\'\n\x03\x65nv\x18\x05 \x03(\x0b\x32\x1a.k8s.io.api.core.v1.EnvVar\x12\x0b\n\x03gpu\x18\x06 \x01(\x08\x12\x0e\n\x06\x61\x63tive\x18\x07 \x01(\x08\x12\x0f\n\x07preload\x18\x08 \x01(\x08\x12:\n\rconnectionRef\x18\t \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0c\n\x04\x62\x61se\x18\n \x01(\t\x12\x0c\n\x04role\x18\x0b \x01(\t\x12\x13\n\x0bmantainedBy\x18\x0c \x01(\t\x12\x0b\n\x03uri\x18\r \x01(\t\x12\x12\n\nframeworks\x18\x0e \x03(\t\x12J\n\x04libs\x18\x0f \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Lib\x12\n\n\x02os\x18\x10 \x01(\t\x12\x11\n\tosVersion\x18\x11 \x01(\t\x12\x0f\n\x07private\x18\x12 \x01(\x08\"\x9a\x02\n\x0bMeasurement\x12\x33\n\x06\x65ntity\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0e\n\x06\x63olumn\x18\x02 \x01(\t\x12\x0e\n\x06metric\x18\x03 \x01(\t\x12\r\n\x05value\x18\x04 \x01(\x01\x12\x0e\n\x06stddev\x18\x05 \x01(\x01\x12\x0f\n\x07\x62oolQty\x18\x06 \x01(\x08\x12\x10\n\x08\x63\x61tegory\x18\x07 \x01(\t\x12\x10\n\x08valueSet\x18\x08 \x03(\t\x12=\n\ttimePoint\x18\t \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x10\n\x08taskType\x18\n \x01(\t\x12\x11\n\talgorithm\x18\x0b \x01(\t\"\xc5\x01\n\x13ModelDeploymentSpec\x12\x35\n\x08modelRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\x0f\n\x07traffic\x18\x03 \x01(\x05\x12\x0c\n\x04role\x18\x04 \x01(\t\x12\x11\n\timageName\x18\x05 \x01(\t\x12\x37\n\napprovedBy\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\xd1\x01\n\x10NotificationSpec\x12\x0b\n\x03ttl\x18\x01 \x01(\x05\x12\x14\n\x0cnotifierName\x18\x02 \x01(\t\x12i\n\x08selector\x18\x03 \x03(\x0b\x32W.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec.SelectorEntry\x1a/\n\rSelectorEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"-\n\rObjectiveSpec\x12\x0e\n\x06metric\x18\x01 \x01(\t\x12\x0c\n\x04goal\x18\x02 \x01(\t\"^\n\x07PRCurve\x12S\n\x06values\x18\x01 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CurvePoint\"\x93\x02\n\x0eParameterRange\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0b\n\x03low\x18\x03 \x01(\x01\x12\x0c\n\x04high\x18\x04 \x01(\x01\x12\x0c\n\x04step\x18\x05 \x01(\x05\x12\x0b\n\x03log\x18\x06 \x01(\x08\x12\x0f\n\x07\x63hoices\x18\x07 \x03(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x08 \x01(\x01\x12\x15\n\rdefaultChoice\x18\t \x01(\t\x12\x13\n\x0b\x63onditional\x18\n \x01(\x08\x12\x0e\n\x06parent\x18\x0b \x01(\t\x12\x16\n\x0eparentValueCat\x18\x0c \x01(\t\x12\x1a\n\x12parentValueInteger\x18\r \x01(\x05\x12\x18\n\x10parentValueFloat\x18\x0e \x01(\x01\"p\n\x0fPermissionsSpec\x12]\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccountPermissions\"\xb1\x01\n\x0fPretrainedModel\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Z\n\x04spec\x18\x02 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PretrainedModelSpec\"\xb0\x01\n\x13PretrainedModelList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12W\n\x05items\x18\x02 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PretrainedModel\"$\n\x13PretrainedModelSpec\x12\r\n\x05image\x18\x01 \x01(\t\"\xad\x01\n\rPublicDataset\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12X\n\x04spec\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PublicDatasetSpec\"\xac\x01\n\x11PublicDatasetList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12U\n\x05items\x18\x02 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PublicDataset\"\xb6\x02\n\x11PublicDatasetSpec\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0c\n\x04task\x18\x03 \x01(\t\x12\x10\n\x08openMLID\x18\x04 \x01(\t\x12\x0f\n\x07\x64\x61taUrl\x18\x05 \x01(\t\x12\x10\n\x08\x63itation\x18\x06 \x01(\t\x12\x0c\n\x04rows\x18\x07 \x01(\x05\x12\x0f\n\x07\x63olumns\x18\x08 \x01(\x05\x12\x10\n\x08\x66ileSize\x18\t \x01(\x05\x12\x14\n\x0ctargetColumn\x18\n \x01(\t\x12\x10\n\x08industry\x18\x0b \x01(\t\x12\x12\n\nimbalanced\x18\x0c \x01(\x08\x12\x14\n\x0c\x64\x61tasourceCR\x18\r \x01(\t\x12\x11\n\tdatasetCR\x18\x0e \x01(\t\x12\x0f\n\x07studyCR\x18\x0f \x01(\t\x12\x15\n\rdataProductCR\x18\x10 \x01(\t\"\xb6\x01\n\x06Region\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x1d\n\x15\x64\x65\x66\x61ultDatacenterName\x18\x02 \x01(\t\x12\x10\n\x08location\x18\x03 \x01(\t\x12\x13\n\x0b\x62illingCode\x18\x04 \x01(\t\x12X\n\x0b\x64\x61tacenters\x18\x05 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataCenter\"?\n\x13ResourceConsumption\x12\x0b\n\x03\x63pu\x18\x01 \x01(\x04\x12\x0e\n\x06memory\x18\x02 \x01(\x04\x12\x0b\n\x03gpu\x18\x03 \x01(\x04\"t\n\x0cResourceSpec\x12\x14\n\x0cworkloadName\x18\x01 \x01(\t\x12\x0e\n\x06\x63ustom\x18\x02 \x01(\x08\x12>\n\x0crequirements\x18\x03 \x01(\x0b\x32(.k8s.io.api.core.v1.ResourceRequirements\"b\n\x0bRocAucCurve\x12S\n\x06values\x18\x01 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CurvePoint\"\xcd\x01\n\x0bRunSchedule\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04\x63ron\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x15\n\rmaxRetryCount\x18\x04 \x01(\x05\x12\x15\n\rretryDelaySec\x18\x05 \x01(\x05\x12\x12\n\ntimeoutSec\x18\x06 \x01(\x05\x12\x10\n\x08timezone\x18\x07 \x01(\t\x12=\n\tnextRunAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"\xfe\x01\n\x11RunScheduleStatus\x12=\n\tlastRunAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x02 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x03 \x01(\t\x12\x13\n\x0blastRunName\x18\x04 \x01(\t\x12R\n\x0blastRunLogs\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12\x12\n\nretryCount\x18\x06 \x01(\x05\"r\n\tTestSuite\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12T\n\x05tests\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataTestCase\"\xc7\x02\n\x0fTestSuiteResult\x12\x36\n\tentityRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08\x66\x61ilures\x18\x02 \x01(\x05\x12\x0e\n\x06\x65rrors\x18\x03 \x01(\x05\x12=\n\tstartedAt\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12Z\n\x05tests\x18\x06 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataTestCaseResult\"G\n\x0fWorkerRunResult\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0b\n\x03uri\x18\x02 \x01(\t\x12\x0c\n\x04task\x18\x03 \x01(\t\x12\r\n\x05\x65rror\x18\x04 \x01(\t\"\xad\x01\n\rWorkloadClass\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12X\n\x04spec\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkloadClassSpec\"\xac\x01\n\x11WorkloadClassList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12U\n\x05items\x18\x02 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkloadClass\"u\n\x11WorkloadClassSpec\x12`\n\x11resourcesTemplate\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpecB9Z7github.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.generated_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z7github.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1'
@@ -97,57 +97,57 @@
   _MANAGEDIMAGELIST._serialized_start=5468
   _MANAGEDIMAGELIST._serialized_end=5638
   _MANAGEDIMAGESPEC._serialized_start=5641
   _MANAGEDIMAGESPEC._serialized_end=6084
   _MEASUREMENT._serialized_start=6087
   _MEASUREMENT._serialized_end=6369
   _MODELDEPLOYMENTSPEC._serialized_start=6372
-  _MODELDEPLOYMENTSPEC._serialized_end=6679
-  _NOTIFICATIONSPEC._serialized_start=6682
-  _NOTIFICATIONSPEC._serialized_end=6916
-  _NOTIFICATIONSPEC_SELECTORENTRY._serialized_start=6869
-  _NOTIFICATIONSPEC_SELECTORENTRY._serialized_end=6916
-  _OBJECTIVESPEC._serialized_start=6918
-  _OBJECTIVESPEC._serialized_end=6963
-  _PRCURVE._serialized_start=6965
-  _PRCURVE._serialized_end=7059
-  _PARAMETERRANGE._serialized_start=7062
-  _PARAMETERRANGE._serialized_end=7337
-  _PERMISSIONSSPEC._serialized_start=7339
-  _PERMISSIONSSPEC._serialized_end=7451
-  _PRETRAINEDMODEL._serialized_start=7454
-  _PRETRAINEDMODEL._serialized_end=7631
-  _PRETRAINEDMODELLIST._serialized_start=7634
-  _PRETRAINEDMODELLIST._serialized_end=7810
-  _PRETRAINEDMODELSPEC._serialized_start=7812
-  _PRETRAINEDMODELSPEC._serialized_end=7848
-  _PUBLICDATASET._serialized_start=7851
-  _PUBLICDATASET._serialized_end=8024
-  _PUBLICDATASETLIST._serialized_start=8027
-  _PUBLICDATASETLIST._serialized_end=8199
-  _PUBLICDATASETSPEC._serialized_start=8202
-  _PUBLICDATASETSPEC._serialized_end=8512
-  _REGION._serialized_start=8515
-  _REGION._serialized_end=8697
-  _RESOURCECONSUMPTION._serialized_start=8699
-  _RESOURCECONSUMPTION._serialized_end=8762
-  _RESOURCESPEC._serialized_start=8764
-  _RESOURCESPEC._serialized_end=8880
-  _ROCAUCCURVE._serialized_start=8882
-  _ROCAUCCURVE._serialized_end=8980
-  _RUNSCHEDULE._serialized_start=8983
-  _RUNSCHEDULE._serialized_end=9188
-  _RUNSCHEDULESTATUS._serialized_start=9191
-  _RUNSCHEDULESTATUS._serialized_end=9445
-  _TESTSUITE._serialized_start=9447
-  _TESTSUITE._serialized_end=9561
-  _TESTSUITERESULT._serialized_start=9564
-  _TESTSUITERESULT._serialized_end=9891
-  _WORKERRUNRESULT._serialized_start=9893
-  _WORKERRUNRESULT._serialized_end=9964
-  _WORKLOADCLASS._serialized_start=9967
-  _WORKLOADCLASS._serialized_end=10140
-  _WORKLOADCLASSLIST._serialized_start=10143
-  _WORKLOADCLASSLIST._serialized_end=10315
-  _WORKLOADCLASSSPEC._serialized_start=10317
-  _WORKLOADCLASSSPEC._serialized_end=10434
+  _MODELDEPLOYMENTSPEC._serialized_end=6569
+  _NOTIFICATIONSPEC._serialized_start=6572
+  _NOTIFICATIONSPEC._serialized_end=6781
+  _NOTIFICATIONSPEC_SELECTORENTRY._serialized_start=6734
+  _NOTIFICATIONSPEC_SELECTORENTRY._serialized_end=6781
+  _OBJECTIVESPEC._serialized_start=6783
+  _OBJECTIVESPEC._serialized_end=6828
+  _PRCURVE._serialized_start=6830
+  _PRCURVE._serialized_end=6924
+  _PARAMETERRANGE._serialized_start=6927
+  _PARAMETERRANGE._serialized_end=7202
+  _PERMISSIONSSPEC._serialized_start=7204
+  _PERMISSIONSSPEC._serialized_end=7316
+  _PRETRAINEDMODEL._serialized_start=7319
+  _PRETRAINEDMODEL._serialized_end=7496
+  _PRETRAINEDMODELLIST._serialized_start=7499
+  _PRETRAINEDMODELLIST._serialized_end=7675
+  _PRETRAINEDMODELSPEC._serialized_start=7677
+  _PRETRAINEDMODELSPEC._serialized_end=7713
+  _PUBLICDATASET._serialized_start=7716
+  _PUBLICDATASET._serialized_end=7889
+  _PUBLICDATASETLIST._serialized_start=7892
+  _PUBLICDATASETLIST._serialized_end=8064
+  _PUBLICDATASETSPEC._serialized_start=8067
+  _PUBLICDATASETSPEC._serialized_end=8377
+  _REGION._serialized_start=8380
+  _REGION._serialized_end=8562
+  _RESOURCECONSUMPTION._serialized_start=8564
+  _RESOURCECONSUMPTION._serialized_end=8627
+  _RESOURCESPEC._serialized_start=8629
+  _RESOURCESPEC._serialized_end=8745
+  _ROCAUCCURVE._serialized_start=8747
+  _ROCAUCCURVE._serialized_end=8845
+  _RUNSCHEDULE._serialized_start=8848
+  _RUNSCHEDULE._serialized_end=9053
+  _RUNSCHEDULESTATUS._serialized_start=9056
+  _RUNSCHEDULESTATUS._serialized_end=9310
+  _TESTSUITE._serialized_start=9312
+  _TESTSUITE._serialized_end=9426
+  _TESTSUITERESULT._serialized_start=9429
+  _TESTSUITERESULT._serialized_end=9756
+  _WORKERRUNRESULT._serialized_start=9758
+  _WORKERRUNRESULT._serialized_end=9829
+  _WORKLOADCLASS._serialized_start=9832
+  _WORKLOADCLASS._serialized_end=10005
+  _WORKLOADCLASSLIST._serialized_start=10008
+  _WORKLOADCLASSLIST._serialized_end=10180
+  _WORKLOADCLASSSPEC._serialized_start=10182
+  _WORKLOADCLASSSPEC._serialized_end=10299
 # @@protoc_insertion_point(module_scope)
```

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_catalog_dot_v1alpha1_dot_generated__pb2
 from k8s.io.api.core.v1 import generated_pb2 as k8s_dot_io_dot_api_dot_core_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.apis.meta.v1 import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_apis_dot_meta_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime.schema import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_schema_dot_generated__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nDgithub.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x12\x34github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\x87\x01\n\x14\x41pprovalReviewStatus\x12\x10\n\x08reviewer\x18\x01 \x01(\t\x12\x0e\n\x06result\x18\x02 \x01(\t\x12>\n\napprovedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05notes\x18\x04 \x01(\t\"F\n\x0c\x41pprovalSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x14\n\x0c\x64\x65\x63isionType\x18\x02 \x01(\t\x12\x0f\n\x07members\x18\x03 \x03(\t\"}\n\x0e\x41pprovalStatus\x12\x0e\n\x06status\x18\x01 \x01(\t\x12[\n\x07reviews\x18\x02 \x03(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ApprovalReviewStatus\"W\n\x0c\x42\x61rChartSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\t\n\x01x\x18\x02 \x01(\t\x12\t\n\x01y\x18\x03 \x01(\t\x12\x0e\n\x06legend\x18\x04 \x01(\x08\x12\x0c\n\x04sort\x18\x05 \x01(\x08\"\xa0\x07\n\x06\x43olumn\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64isplayName\x18\x02 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x03 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\x12\x0e\n\x06ignore\x18\x06 \x01(\x08\x12\x0e\n\x06target\x18\x07 \x01(\x08\x12\x10\n\x08nullable\x18\x08 \x01(\x08\x12\n\n\x02pk\x18\t \x01(\x08\x12\n\n\x02\x66k\x18\n \x01(\x08\x12\x12\n\nmultipleOf\x18\x0b \x01(\x05\x12\x0f\n\x07maximum\x18\x0c \x01(\x01\x12\x18\n\x10\x65xclusiveMaximum\x18\r \x01(\x08\x12\x0f\n\x07minimum\x18\x0e \x01(\x01\x12\x18\n\x10\x65xclusiveMinimum\x18\x0f \x01(\x08\x12\x11\n\tmaxLength\x18\x10 \x01(\x05\x12\x11\n\tminLength\x18\x11 \x01(\x05\x12\x0f\n\x07pattern\x18\x12 \x01(\t\x12\x10\n\x08required\x18\x13 \x01(\x08\x12\x0f\n\x07\x65xample\x18\x14 \x01(\t\x12\x14\n\x0c\x65xternalDocs\x18\x15 \x01(\t\x12\x0c\n\x04\x65num\x18\x16 \x03(\t\x12\x10\n\x08maxItems\x18\x18 \x01(\x05\x12\x10\n\x08minItems\x18\x19 \x01(\x05\x12\x13\n\x0buniqueItems\x18\x1a \x01(\x08\x12\x0b\n\x03pii\x18\x1c \x01(\x08\x12\x0b\n\x03phi\x18\x1d \x01(\x08\x12\x11\n\tprotected\x18\x1f \x01(\x08\x12\x17\n\x0f\x64\x65\x66\x61ultValueNum\x18  \x01(\x01\x12\x0b\n\x03log\x18! \x01(\x08\x12\n\n\x02mu\x18\" \x01(\x01\x12\r\n\x05sigma\x18# \x01(\x01\x12\x15\n\rskewThreshold\x18$ \x01(\x01\x12\x16\n\x0e\x64riftThreshold\x18% \x01(\x01\x12\x0b\n\x03key\x18& \x01(\x08\x12\x0c\n\x04\x66old\x18\' \x01(\x08\x12\x0e\n\x06weight\x18( \x01(\x08\x12\x10\n\x08reserved\x18) \x01(\x08\x12\x12\n\nimputation\x18* \x01(\t\x12\x0f\n\x07scaling\x18+ \x01(\t\x12\x11\n\tgenerated\x18, \x01(\x08\x12\x0f\n\x07\x66ormula\x18- \x01(\t\x12\n\n\x02id\x18. \x01(\x08\x12\x0c\n\x04step\x18/ \x01(\x01\x12\x0b\n\x03loc\x18\x30 \x01(\x05\x12\x16\n\x0e\x64\x61tetimeFormat\x18\x31 \x01(\t\x12\x12\n\ntimeseries\x18\x32 \x01(\x08\x12\x11\n\tregressor\x18\x33 \x01(\x08\x12\x17\n\x0flaggedRegressor\x18\x34 \x01(\x08\x12\x11\n\ttimeIndex\x18\x35 \x01(\x08\x12\x0c\n\x04\x61ggr\x18\x36 \x01(\t\x12\x0e\n\x06window\x18\x37 \x01(\x05\"\xe0\x01\n\x0f\x43olumnHistogram\x12\x0c\n\x04name\x18\x01 \x01(\t\x12Y\n\thistogram\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.HistogramData\x12U\n\x07metrics\x18\x03 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12\r\n\x05\x64rift\x18\x04 \x01(\x08\"\x81\x01\n\nColumnSpec\x12\x0e\n\x06spacer\x18\x01 \x01(\x08\x12\r\n\x05width\x18\x02 \x01(\x05\x12T\n\x07\x63ontent\x18\x03 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ComponentSpec\"\xae\x07\n\x10\x43olumnStatistics\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\r\n\x05\x63ount\x18\x03 \x01(\x01\x12\x10\n\x08\x64istinct\x18\x04 \x01(\x05\x12\x0f\n\x07missing\x18\x05 \x01(\x05\x12\x16\n\x0epercentMissing\x18\x06 \x01(\x01\x12\x0c\n\x04mean\x18\x07 \x01(\x01\x12\x0e\n\x06stddev\x18\x08 \x01(\x01\x12\x10\n\x08variance\x18\t \x01(\x01\x12\x0b\n\x03min\x18\n \x01(\x01\x12\x0b\n\x03max\x18\x0b \x01(\x01\x12\x10\n\x08kurtosis\x18\x0c \x01(\x01\x12\x10\n\x08skewness\x18\r \x01(\x01\x12\x0b\n\x03sum\x18\x0e \x01(\x01\x12\x0b\n\x03mad\x18\x0f \x01(\x01\x12\x0b\n\x03p25\x18\x10 \x01(\x01\x12\x0b\n\x03p50\x18\x11 \x01(\x01\x12\x0b\n\x03p75\x18\x12 \x01(\x01\x12\x0b\n\x03iqr\x18\x13 \x01(\x01\x12\x0c\n\x04mode\x18\x14 \x01(\t\x12\r\n\x05zeros\x18\x15 \x01(\x01\x12\x0f\n\x07invalid\x18\x16 \x01(\x05\x12\x12\n\nimportance\x18\x17 \x01(\x01\x12\x0e\n\x06target\x18\x18 \x01(\x08\x12\x0e\n\x06ignore\x18\x19 \x01(\x08\x12\x10\n\x08nullable\x18\x1a \x01(\x08\x12\x17\n\x0fhighCardinality\x18\x1b \x01(\x08\x12!\n\x19highCorrWithOtherFeatures\x18\x1c \x01(\x08\x12\x19\n\x11lowCorrWithTarget\x18\x1d \x01(\x08\x12\x16\n\x0ehighMissingPct\x18\x1e \x01(\x08\x12\x0e\n\x06skewed\x18\x1f \x01(\x08\x12\n\n\x02id\x18  \x01(\x08\x12\x10\n\x08\x63onstant\x18! \x01(\x08\x12\x11\n\tduplicate\x18\" \x01(\x08\x12\x10\n\x08reserved\x18# \x01(\x08\x12\x14\n\x0c\x63ompleteness\x18% \x01(\x01\x12\x1a\n\x12\x64istinctValueCount\x18& \x01(\x01\x12\x1b\n\x13mostFreqValuesRatio\x18\' \x01(\x01\x12\x1a\n\x12indexOfPeculiarity\x18( \x01(\x01\x12Y\n\thistogram\x18) \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.HistogramData\x12\x14\n\x0c\x63orrToTarget\x18* \x01(\x01\x12\r\n\x05index\x18+ \x01(\x05\x12S\n\x08outliers\x18, \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.OutlierStat\"\x96\x01\n\rComponentSpec\x12\r\n\x05title\x18\x01 \x01(\t\x12\x10\n\x08subtitle\x18\x02 \x01(\t\x12\x0e\n\x06\x66ooter\x18\x03 \x01(\t\x12T\n\x07\x63ontent\x18\x04 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ComponentView\"\xe3\x04\n\rComponentView\x12P\n\x06metric\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.MetricSpec\x12N\n\x05gauge\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GaugeSpec\x12V\n\thistogram\x18\x03 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.HistogramSpec\x12N\n\x05table\x18\x04 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.TableSpec\x12V\n\tlineChart\x18\x05 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LineChartSpec\x12T\n\x08\x62\x61rChart\x18\x06 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.BarChartSpec\x12Z\n\x0bscatterPlot\x18\x07 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ScatterPlotSpec\"P\n\x0b\x43orrelation\x12\x10\n\x08\x66\x65\x61ture1\x18\x01 \x01(\t\x12\x10\n\x08\x66\x65\x61ture2\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\x01\x12\x0e\n\x06method\x18\x04 \x01(\t\">\n\x0f\x43orrelationSpec\x12\x0e\n\x06\x63utoff\x18\x01 \x01(\x01\x12\x0e\n\x06method\x18\x02 \x01(\t\x12\x0b\n\x03top\x18\x03 \x01(\x05\"\xef\x01\n\x0b\x43svFileSpec\x12\x11\n\tdelimiter\x18\x01 \x01(\t\x12\r\n\x05quote\x18\x03 \x01(\t\x12\x12\n\nescapeChar\x18\x04 \x01(\t\x12\x14\n\x0c\x63ommentChars\x18\x05 \x01(\t\x12\x0e\n\x06header\x18\x06 \x01(\x08\x12\x10\n\x08skipRows\x18\x07 \x01(\x05\x12\x12\n\nnullValues\x18\x08 \x01(\t\x12\x10\n\x08\x65ncoding\x18\t \x01(\t\x12\x0f\n\x07maxRows\x18\n \x01(\x05\x12\x0e\n\x06strict\x18\x0b \x01(\x08\x12\x13\n\x0b\x63ompression\x18\x0c \x01(\t\x12\x16\n\x0ehasIndexColumn\x18\r \x01(\x08\"\xd2\x01\n\rDataInputSpec\x12\x0e\n\x06preSQL\x18\x01 \x03(\t\x12W\n\x08location\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12X\n\x06\x66ormat\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\"\x8c\x02\n\x0e\x44\x61taOutputSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12W\n\x08location\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x0e\n\x06\x66ormat\x18\x03 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\x12\x1d\n\x15\x63reateTableIfNotExist\x18\x05 \x01(\x08\x12\x17\n\x0fincludeFeatures\x18\x06 \x01(\x08\x12\x0b\n\x03xai\x18\x07 \x01(\x08\x12\x16\n\x0e\x64\x65tectOutliers\x18\x08 \x01(\x08\x12\x0f\n\x07postSQL\x18\t \x03(\t\"\x82\x02\n\x0c\x44\x61taPipeline\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12T\n\x04spec\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineSpec\x12X\n\x06status\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineStatus\"\xa7\x01\n\x10\x44\x61taPipelineList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Q\n\x05items\x18\x02 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipeline\"\x8b\x02\n\x0f\x44\x61taPipelineRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12W\n\x04spec\x18\x02 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineRunSpec\x12[\n\x06status\x18\x03 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineRunStatus\"\xa1\x01\n\x18\x44\x61taPipelineRunCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x06 \x01(\t\"\xad\x01\n\x13\x44\x61taPipelineRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12T\n\x05items\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineRun\"\xc8\x02\n\x13\x44\x61taPipelineRunSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x18\n\x10\x64\x61tapipelineName\x18\x02 \x01(\t\x12\r\n\x05owner\x18\x04 \x01(\t\x12X\n\tresources\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x10\n\x08priority\x18\x06 \x01(\t\x12\x0e\n\x06paused\x18\x07 \x01(\x08\x12\x0f\n\x07\x61\x62orted\x18\x08 \x01(\x08\x12\x33\n\x06labRef\x18\t \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x16\n\x0emodelClassName\x18\n \x01(\t\x12\x19\n\x11modelClassRunName\x18\x0b \x01(\t\"\x80\x04\n\x15\x44\x61taPipelineRunStatus\x12\x12\n\nrecipeRuns\x18\x01 \x03(\t\x12U\n\x06output\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\r\n\x05phase\x18\x03 \x01(\t\x12?\n\x0b\x63ompletedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x06 \x01(\x03\x12\x15\n\rfailureReason\x18\x07 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x08 \x01(\t\x12\x10\n\x08progress\x18\t \x01(\x05\x12K\n\x04logs\x18\n \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12=\n\tupdatedAt\x18\x0b \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\nconditions\x18\x0c \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x80\x06\n\x10\x44\x61taPipelineSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x16\n\x0emodelClassName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12t\n\x0f\x64\x61tasetSelector\x18\x04 \x03(\x0b\x32[.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineSpec.DatasetSelectorEntry\x12U\n\x07recipes\x18\x05 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipePartSpec\x12T\n\x06output\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataOutputSpec\x12V\n\x08schedule\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12_\n\x0cnotification\x18\x08 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\r\n\x05owner\x18\t \x01(\t\x12X\n\tresources\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x10\n\x08priority\x18\x0b \x01(\t\x12\x0e\n\x06paused\x18\x0c \x01(\x08\x12\x0b\n\x03ttl\x18\r \x01(\x05\x1a\x36\n\x14\x44\x61tasetSelectorEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xba\x02\n\x12\x44\x61taPipelineStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\\\n\x08schedule\x18\x03 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12\x13\n\x0blastRunName\x18\x04 \x01(\t\x12\x11\n\trunsCount\x18\x05 \x01(\x05\x12\x43\n\nconditions\x18\x06 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xff\x01\n\x0b\x44\x61taProduct\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12S\n\x04spec\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductSpec\x12W\n\x06status\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductStatus\"\xa5\x01\n\x0f\x44\x61taProductList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12P\n\x05items\x18\x02 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\"\xc5\x07\n\x0f\x44\x61taProductSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x0e\n\x06public\x18\x02 \x01(\x08\x12\x36\n\ttenantRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12V\n\x0bgitLocation\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GitLocation\x12Z\n\rimageLocation\x18\x05 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ImageLocation\x12\x16\n\x0e\x64\x65\x66\x61ultLabName\x18\x06 \x01(\t\x12\x1e\n\x16\x64\x65\x66\x61ultServingSiteName\x18\x07 \x01(\t\x12\x19\n\x11\x64\x65\x66\x61ultBucketName\x18\x08 \x01(\t\x12\x0c\n\x04task\x18\t \x01(\t\x12\x0f\n\x07subtask\x18\n \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x0b \x01(\t\x12_\n\x0cnotification\x18\x0c \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12`\n\x11trainingResources\x18\r \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12_\n\x10servingResources\x18\x0e \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x18\n\x10retriesOnFailure\x18\x0f \x01(\x05\x12\x10\n\x08priority\x18\x10 \x01(\t\x12\r\n\x05\x63olor\x18\x11 \x01(\t\x12T\n\x08\x61pproval\x18\x12 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ApprovalSpec\x12]\n\x0bpermissions\x18\x13 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PermissionsSpec\x12\x0c\n\x04tags\x18\x14 \x03(\t\"\xa9\x04\n\x11\x44\x61taProductStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x18\n\x10\x64\x61tasourcesCount\x18\x03 \x01(\x05\x12\x15\n\rdatasetsCount\x18\x04 \x01(\x05\x12\x19\n\x11\x64\x61taPipelineCount\x18\x05 \x01(\x05\x12\x1d\n\x15totalDataPipelineRuns\x18\x06 \x01(\x05\x12\x14\n\x0cstudiesCount\x18\x07 \x01(\x05\x12\x13\n\x0bmodelsCount\x18\x08 \x01(\x05\x12\x17\n\x0fpredictorsCount\x18\x0b \x01(\x05\x12\x15\n\rdataAppsCount\x18\r \x01(\x05\x12\x18\n\x10predictionsCount\x18\x0e \x01(\x05\x12\x17\n\x0finfoAlertsCount\x18\x0f \x01(\x05\x12\x18\n\x10\x65rrorAlertsCount\x18\x10 \x01(\x05\x12\x19\n\x11modelClassesCount\x18\x11 \x01(\x05\x12\x15\n\rfailureReason\x18\x12 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x13 \x01(\t\x12\x17\n\x0f\x62\x61selineVersion\x18\x14 \x01(\t\x12\x43\n\nconditions\x18\x15 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x94\x02\n\x12\x44\x61taProductVersion\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Z\n\x04spec\x18\x02 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersionSpec\x12^\n\x06status\x18\x03 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersionStatus\"\xb3\x01\n\x16\x44\x61taProductVersionList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12W\n\x05items\x18\x02 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\"\xa0\x01\n\x16\x44\x61taProductVersionSpec\x12\x37\n\nproductRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x17\n\x0fprevVersionName\x18\x03 \x01(\t\x12\x10\n\x08\x62\x61seline\x18\x04 \x01(\x08\x12\r\n\x05owner\x18\x05 \x01(\t\"\xe9\x01\n\x18\x44\x61taProductVersionStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x03 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x04 \x01(\t\x12\x43\n\nconditions\x18\x05 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xfc\x01\n\nDataSource\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12R\n\x04spec\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSourceSpec\x12V\n\x06status\x18\x03 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSourceStatus\"\xa3\x01\n\x0e\x44\x61taSourceList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12O\n\x05items\x18\x02 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\"\x91\x06\n\x0e\x44\x61taSourceSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x61tasetType\x18\x04 \x01(\t\x12L\n\x06schema\x18\x05 \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Schema\x12Z\n\x08\x66latfile\x18\x06 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\x12\x0f\n\x07labeled\x18\x07 \x01(\x08\x12P\n\x06sample\x18\t \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SampleSpec\x12\x0c\n\x04task\x18\n \x01(\t\x12\x0f\n\x07subtask\x18\x0b \x01(\t\x12]\n\rrelationships\x18\x0c \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RelationshipSpec\x12T\n\x08labeling\x18\r \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingSpec\x12[\n\x0cinferredFrom\x18\x0e \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12]\n\x11unitTestsTemplate\x18\x0f \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12\x14\n\x0cingestMethod\x18\x10 \x01(\t\"\xd2\x02\n\x10\x44\x61taSourceStatus\x12\x0c\n\x04\x63ols\x18\x01 \x01(\x05\x12\x1a\n\x12observedGeneration\x18\x02 \x01(\x03\x12H\n\x14lastDatasetCreatedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x17\n\x0flastDatasetName\x18\x04 \x01(\t\x12=\n\tupdatedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x06 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x07 \x01(\t\x12\x43\n\nconditions\x18\x08 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xf3\x01\n\x07\x44\x61taset\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12O\n\x04spec\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSpec\x12S\n\x06status\x18\x03 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetStatus\"\xe0\x01\n\x14\x44\x61tasetGroupByStatus\x12\x13\n\x0b\x64\x61tasetsURI\x18\x01 \x01(\t\x12\x13\n\x0bprofilesURI\x18\x02 \x01(\t\x12\x12\n\nreportsURI\x18\x03 \x01(\t\x12\x14\n\x0cunitTestsURI\x18\x04 \x01(\t\x12\x13\n\x0b\x66\x65\x61turesURI\x18\x05 \x01(\t\x12_\n\rworkerResults\x18\x06 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"\x9d\x01\n\x0b\x44\x61tasetList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12L\n\x05items\x18\x02 \x03(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"\xb8\x0b\n\x0b\x44\x61tasetSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x16\n\x0e\x64\x61taSourceName\x18\x03 \x01(\t\x12\x18\n\x10\x66\x65\x61tureGroupName\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12\x13\n\x0b\x64isplayName\x18\x08 \x01(\t\x12\x0c\n\x04role\x18\t \x01(\t\x12\x0c\n\x04tags\x18\n \x03(\t\x12\x0e\n\x06report\x18\x0b \x01(\x08\x12\x10\n\x08unitTest\x18\x0c \x01(\x08\x12U\n\x06origin\x18\r \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12W\n\x08location\x18\x0e \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x1a\n\x12\x61rtifactBucketName\x18\x0f \x01(\t\x12X\n\tresources\x18\x10 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0f\n\x07timeout\x18\x11 \x01(\x03\x12\x0c\n\x04type\x18\x12 \x01(\t\x12P\n\x06sample\x18\x13 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SampleSpec\x12V\n\tsynthetic\x18\x14 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SyntheticSpec\x12\x0c\n\x04task\x18\x15 \x01(\t\x12\x0f\n\x07subtask\x18\x16 \x01(\t\x12Z\n\x0b\x63orrelation\x18\x17 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.CorrelationSpec\x12\x0c\n\x04\x66\x61st\x18\x18 \x01(\x08\x12\x11\n\tfeaturize\x18\x19 \x01(\x08\x12\x33\n\x06labRef\x18\x1a \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12>\n\x11servingDatasetRef\x18\x1b \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x39\n\x0cpredictorRef\x18\x1c \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12 \n\x18generateFeatureHistogram\x18\x1d \x01(\x08\x12U\n\tunitTests\x18\x1e \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12R\n\x07groupBy\x18\x1f \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GroupBySpec\x12g\n\x0egroupLocations\x18  \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GroupDatasetLocationsSpec\x12\x0b\n\x03key\x18! \x03(\t\x12\x16\n\x0emodelClassName\x18\" \x01(\t\x12\x19\n\x11modelClassRunName\x18# \x01(\t\x12:\n\rfeatureGroups\x18$ \x03(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\xd9\x02\n\x11\x44\x61tasetStatistics\x12W\n\x07\x63olumns\x18\x01 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ColumnStatistics\x12\x0c\n\x04rows\x18\x03 \x01(\x05\x12\x0c\n\x04\x63ols\x18\x04 \x01(\x05\x12\x10\n\x08\x66ileSize\x18\x05 \x01(\x05\x12\x61\n\x16\x63orrelationsWithTarget\x18\x06 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\x12Z\n\x0ftopCorrelations\x18\x07 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\"\xed\t\n\rDatasetStatus\x12[\n\nstatistics\x18\x01 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetStatistics\x12\r\n\x05phase\x18\x02 \x01(\t\x12\x12\n\nreportName\x18\x03 \x01(\t\x12]\n\x0ereportLocation\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12^\n\x0fprofileLocation\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12`\n\x11\x61nomaliesLocation\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x12\n\nimbalanced\x18\x07 \x01(\x08\x12\x1a\n\x12observedGeneration\x18\x08 \x01(\x03\x12]\n\x0btestResults\x18\t \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12?\n\x0blastStudyAt\x18\n \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x0c \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\r \x01(\t\x12\x10\n\x08progress\x18\x0e \x01(\x05\x12\x0c\n\x04hash\x18\x0f \x01(\t\x12K\n\x04logs\x18\x10 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12\x1a\n\x12\x64\x65rivedFromDataset\x18\x11 \x01(\t\x12=\n\tupdatedAt\x18\x12 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12O\n\x06images\x18\x13 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Images\x12?\n\x0b\x63ompletedAt\x18\x15 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12@\n\x13\x66\x65\x61tureHistogramRef\x18\x16 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12[\n\x07groupby\x18\x17 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetGroupByStatus\x12\x43\n\nconditions\x18\x18 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xa6\x01\n\x0f\x44\x61tasetTemplate\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12O\n\x04spec\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSpec\"/\n\x0e\x44riftThreshold\x12\x0e\n\x06metric\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\"\xf0\x01\n\x06\x45ntity\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12N\n\x04spec\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.EntitySpec\x12R\n\x06status\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.EntityStatus\"\x9b\x01\n\nEntityList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12K\n\x05items\x18\x02 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Entity\"\x87\x01\n\nEntitySpec\x12\x36\n\ttenantRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0f\n\x07joinKey\x18\x04 \x01(\t\x12\r\n\x05owner\x18\x05 \x01(\t\x12\x0c\n\x04tags\x18\x06 \x03(\t\"\xae\x01\n\x0c\x45ntityStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\nconditions\x18\x03 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xc1\x01\n\x11\x45xcelNotebookSpec\x12\x1a\n\x12\x66irstSheetWithData\x18\x01 \x01(\x08\x12\x11\n\tsheetName\x18\x02 \x01(\t\x12\x12\n\nsheetIndex\x18\x03 \x01(\x05\x12\x15\n\rcolumnNameRow\x18\x04 \x01(\x05\x12R\n\x04\x64\x61ta\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ExcelSheetArea\"k\n\x0e\x45xcelSheetArea\x12\x13\n\x0b\x65ntireSheet\x18\x01 \x01(\x08\x12\x12\n\nfromColumn\x18\x02 \x01(\x05\x12\x10\n\x08toColumn\x18\x03 \x01(\x05\x12\x0f\n\x07\x66romRow\x18\x04 \x01(\x05\x12\r\n\x05toRow\x18\x05 \x01(\x05\"\x82\x02\n\x0c\x46\x65\x61tureGroup\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12T\n\x04spec\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroupSpec\x12X\n\x06status\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroupStatus\"\xa7\x01\n\x10\x46\x65\x61tureGroupList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Q\n\x05items\x18\x02 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\"\x84\x08\n\x10\x46\x65\x61tureGroupSpec\x12\x36\n\ttenantRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\r\n\x05owner\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x1a\n\x12\x61rtifactBucketName\x18\x04 \x01(\t\x12\x12\n\ningestType\x18\x05 \x01(\t\x12\x12\n\nentityName\x18\x06 \x01(\t\x12\x0c\n\x04tags\x18\x07 \x03(\t\x12\\\n\x0eingestSchedule\x18\x08 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12Z\n\x0csyncSchedule\x18\t \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12Z\n\x08\x66latfile\x18\n \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\x12L\n\x06schema\x18\x0b \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Schema\x12Q\n\x05tests\x18\x0c \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12W\n\x08location\x18\r \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x12\n\ntimeColumn\x18\x0e \x01(\t\x12\x18\n\x10timeColumnFormat\x18\x0f \x01(\t\x12\x11\n\tkeyColumn\x18\x10 \x01(\t\x12\x62\n\x0fmaterialization\x18\x11 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.MaterializationSpec\x12X\n\tresources\x18\x12 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x33\n\x06labRef\x18\x13 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\x85\x05\n\x12\x46\x65\x61tureGroupStatus\x12\r\n\x05phase\x18\x02 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x03 \x01(\x03\x12=\n\tupdatedAt\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0c\n\x04rows\x18\x05 \x01(\x05\x12\x62\n\x0eingestSchedule\x18\x07 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12`\n\x0csyncSchedule\x18\x08 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12Z\n\x0bonlineTable\x18\t \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x46\n\x12onlineTableCreated\x18\n \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x19\n\x11ingestDatasetName\x18\x0b \x01(\t\x12\x15\n\rfailureReason\x18\x0c \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\r \x01(\t\x12\x43\n\nconditions\x18\x0e \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x8e\x02\n\x10\x46\x65\x61tureHistogram\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12X\n\x04spec\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogramSpec\x12\\\n\x06status\x18\x03 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogramStatus\"\xaf\x01\n\x14\x46\x65\x61tureHistogramList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12U\n\x05items\x18\x02 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogram\"\xf5\x04\n\x14\x46\x65\x61tureHistogramSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x05 \x03(\t\x12\x36\n\tsourceRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08training\x18\x07 \x01(\x08\x12\x0c\n\x04live\x18\t \x01(\x08\x12\x39\n\x05start\x18\n \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x37\n\x03\x65nd\x18\x0b \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x34\n\x07\x62\x61seRef\x18\x0c \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12]\n\x0f\x64riftThresholds\x18\r \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DriftThreshold\x12\x17\n\x0fsyncIntervalSec\x18\x0e \x01(\x05\x12U\n\tunitTests\x18\x0f \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12\x14\n\x0cgenUnitTests\x18\x10 \x01(\x08\x12\x15\n\rfeatureFilter\x18\x11 \x01(\t\x12\x15\n\rreferenceType\x18\x12 \x01(\t\"\x9d\x04\n\x16\x46\x65\x61tureHistogramStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12V\n\x07\x63olumns\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ColumnHistogram\x12=\n\tupdatedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12K\n\x04logs\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12\r\n\x05phase\x18\x06 \x01(\t\x12\x15\n\rfailureReason\x18\x07 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x08 \x01(\t\x12\x61\n\x0funitTestsResult\x18\t \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\r\n\x05total\x18\n \x01(\x05\x12\x0e\n\x06\x65rrors\x18\x0b \x01(\x05\x12\x43\n\nconditions\x18\x0c \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xa6\x02\n\x12\x46latFileFormatSpec\x12\x10\n\x08\x66ileType\x18\x01 \x01(\t\x12N\n\x03\x63sv\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.CsvFileSpec\x12V\n\x05\x65xcel\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ExcelNotebookSpec\x12V\n\x07parquet\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ParquetFileSpec\"M\n\tGaugeSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\x0e\n\x06\x63olumn\x18\x02 \x01(\t\x12\x0b\n\x03row\x18\x03 \x01(\x05\x12\x0e\n\x06scalar\x18\x04 \x01(\t\"V\n\x0bGitLocation\x12\x19\n\x11gitConnectionName\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x03 \x01(\t\x12\x0f\n\x07private\x18\x04 \x01(\x08\"]\n\x0bGroupBySpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07groupby\x18\x02 \x03(\t\x12\x0c\n\x04\x66req\x18\x03 \x01(\t\x12\x10\n\x08interval\x18\x04 \x01(\x05\x12\x0c\n\x04\x61ggr\x18\x05 \x01(\t\"\xc2\x01\n\x19GroupDatasetLocationsSpec\x12\x12\n\ngroupsRoot\x18\x01 \x01(\t\x12\x11\n\tgroupRoot\x18\x02 \x01(\t\x12\x17\n\x0fgroupDataFolder\x18\x03 \x01(\t\x12\x15\n\rgroupDataFile\x18\x04 \x01(\t\x12\x1a\n\x12groupProfileFolder\x18\x05 \x01(\t\x12\x17\n\x0fgroupReportFile\x18\x06 \x01(\t\x12\x19\n\x11groupFeaturesFile\x18\x07 \x01(\t\"=\n\rHistogramSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\t\n\x01x\x18\x02 \x01(\t\x12\x0c\n\x04\x62ins\x18\x03 \x01(\x05\"=\n\rImageLocation\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1e\n\x16registryConnectionName\x18\x02 \x01(\t\"\"\n\x03KPI\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\"?\n\x0cLabelingRule\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\x10\n\x08operator\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\"\xe1\x01\n\x0cLabelingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x14\n\x0cresultColumn\x18\x02 \x01(\t\x12T\n\x08positive\x18\x03 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingRule\x12T\n\x08negative\x18\x04 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingRule\"J\n\rLineChartSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\t\n\x01x\x18\x02 \x01(\t\x12\t\n\x01y\x18\x03 \x01(\t\x12\x0e\n\x06legend\x18\x04 \x01(\x08\"\x86\x02\n\x13MaterializationSpec\x12\x0e\n\x06online\x18\x01 \x01(\x08\x12\x0f\n\x07offline\x18\x02 \x01(\x08\x12=\n\tstartDate\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x12\n\nofflineTTL\x18\x04 \x01(\x05\x12\x11\n\tonlineTTL\x18\x05 \x01(\x05\x12\x10\n\x08\x62\x61\x63kfill\x18\x06 \x01(\x05\x12V\n\x08schedule\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\"N\n\nMetricSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\x0e\n\x06\x63olumn\x18\x02 \x01(\t\x12\x0b\n\x03row\x18\x03 \x01(\x05\x12\x0e\n\x06scalar\x18\x04 \x01(\t\"<\n\x0bOutlierStat\x12\r\n\x05lower\x18\x01 \x01(\x05\x12\r\n\x05upper\x18\x02 \x01(\x05\x12\x0f\n\x07percent\x18\x03 \x01(\x02\"W\n\x08PageSpec\x12K\n\x04rows\x18\x01 \x03(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RowSpec\"!\n\x0fParquetFileSpec\x12\x0e\n\x06\x65ngine\x18\x01 \x01(\t\"\xf0\x01\n\x06Recipe\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12N\n\x04spec\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeSpec\x12R\n\x06status\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeStatus\"\x8f\x01\n\x0fRecipeInputSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12W\n\x08location\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x0e\n\x06\x66ormat\x18\x03 \x01(\t\"\x9b\x01\n\nRecipeList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12K\n\x05items\x18\x02 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Recipe\"\x97\x01\n\x10RecipeOutputSpec\x12\x15\n\rcreateDataset\x18\x01 \x01(\x08\x12\x13\n\x0b\x64\x61tasetName\x18\x02 \x01(\t\x12W\n\x08location\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"8\n\x0eRecipePartSpec\x12\x12\n\nrecipeName\x18\x01 \x01(\t\x12\x12\n\ndependents\x18\x02 \x03(\t\"\xf9\x01\n\tRecipeRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeRunSpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeRunStatus\"\xa1\x01\n\rRecipeRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeRun\"\xe0\x02\n\rRecipeRunSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x12\n\nrecipeName\x18\x02 \x01(\t\x12\x33\n\x06labRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12W\n\x08location\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12X\n\tresources\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0b\n\x03ttl\x18\x06 \x01(\x05\x12\x16\n\x0emodelClassName\x18\x07 \x01(\t\x12\x19\n\x11modelClassRunName\x18\x08 \x01(\t\"\x92\x03\n\x0fRecipeRunStatus\x12?\n\x0b\x63ompletedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x02 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x03 \x01(\x03\x12\x15\n\rfailureReason\x18\x04 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x05 \x01(\t\x12\x13\n\x0btriggeredBy\x18\x06 \x01(\t\x12K\n\x04logs\x18\x07 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12=\n\tupdatedAt\x18\t \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\nconditions\x18\x0b \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xed\x04\n\nRecipeSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12T\n\x05input\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeInputSpec\x12O\n\x05steps\x18\x05 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeStep\x12V\n\x06output\x18\x06 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeOutputSpec\x12P\n\x06sample\x18\x07 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SampleSpec\x12X\n\tresources\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0f\n\x07timeout\x18\n \x01(\x03\x12\x0b\n\x03ttl\x18\x0b \x01(\x05\x12]\n\x11unitTestsTemplate\x18\x0c \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\"\x87\x02\n\x0cRecipeStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12W\n\x07lastRun\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.LastRunStatus\x12=\n\tupdatedAt\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\nconditions\x18\x07 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"s\n\nRecipeStep\x12\n\n\x02op\x18\x01 \x01(\t\x12Y\n\nparameters\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeStepParam\".\n\x0fRecipeStepParam\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"X\n\x14RecommendationSchema\x12\x14\n\x0cuserIDColumn\x18\x01 \x01(\t\x12\x14\n\x0citemIDColumn\x18\x02 \x01(\t\x12\x14\n\x0cratingColumn\x18\x03 \x01(\t\"R\n\x10RelationshipSpec\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06\x63olumn\x18\x02 \x01(\t\x12\r\n\x05\x61rity\x18\x03 \x01(\t\x12\x11\n\trelatesTo\x18\x04 \x01(\t\"Y\n\x07RowSpec\x12N\n\x04\x63ols\x18\x01 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ColumnSpec\"j\n\nSampleSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0c\n\x04rows\x18\x03 \x01(\x05\x12\x0f\n\x07percent\x18\x04 \x01(\x05\x12\x0e\n\x06\x66ilter\x18\x05 \x01(\t\x12\x0e\n\x06\x63olumn\x18\x06 \x01(\t\"<\n\x0fScatterPlotSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\t\n\x01x\x18\x02 \x01(\t\x12\t\n\x01y\x18\x03 \x01(\t\"\xb0\x02\n\x06Schema\x12`\n\x10timeSeriesSchema\x18\x01 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.TimeSeriesSchema\x12h\n\x14recommendationSchema\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecommendationSchema\x12M\n\x07\x63olumns\x18\x03 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Column\x12\x0b\n\x03key\x18\x04 \x03(\t\".\n\rSyntheticSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04rows\x18\x02 \x01(\x05\"\x84\x01\n\tTableSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x02 \x03(\t\x12\x0f\n\x07\x66ilters\x18\x03 \x03(\t\x12\x0f\n\x07groupby\x18\x04 \x03(\t\x12\x0c\n\x04rows\x18\x05 \x01(\x05\x12\x11\n\tshowIndex\x18\x06 \x01(\x08\x12\x0e\n\x06\x62order\x18\x07 \x01(\x08\"@\n\x10TimeSeriesSchema\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0c\n\x04\x66req\x18\x02 \x01(\t\x12\x10\n\x08interval\x18\x03 \x01(\x05\x42\x36Z4github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nDgithub.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x12\x34github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\x87\x01\n\x14\x41pprovalReviewStatus\x12\x10\n\x08reviewer\x18\x01 \x01(\t\x12\x0e\n\x06result\x18\x02 \x01(\t\x12>\n\napprovedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05notes\x18\x04 \x01(\t\"F\n\x0c\x41pprovalSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x14\n\x0c\x64\x65\x63isionType\x18\x02 \x01(\t\x12\x0f\n\x07members\x18\x03 \x03(\t\"}\n\x0e\x41pprovalStatus\x12\x0e\n\x06status\x18\x01 \x01(\t\x12[\n\x07reviews\x18\x02 \x03(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ApprovalReviewStatus\"W\n\x0c\x42\x61rChartSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\t\n\x01x\x18\x02 \x01(\t\x12\t\n\x01y\x18\x03 \x01(\t\x12\x0e\n\x06legend\x18\x04 \x01(\x08\x12\x0c\n\x04sort\x18\x05 \x01(\x08\"\xa0\x07\n\x06\x43olumn\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64isplayName\x18\x02 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x03 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\x12\x0e\n\x06ignore\x18\x06 \x01(\x08\x12\x0e\n\x06target\x18\x07 \x01(\x08\x12\x10\n\x08nullable\x18\x08 \x01(\x08\x12\n\n\x02pk\x18\t \x01(\x08\x12\n\n\x02\x66k\x18\n \x01(\x08\x12\x12\n\nmultipleOf\x18\x0b \x01(\x05\x12\x0f\n\x07maximum\x18\x0c \x01(\x01\x12\x18\n\x10\x65xclusiveMaximum\x18\r \x01(\x08\x12\x0f\n\x07minimum\x18\x0e \x01(\x01\x12\x18\n\x10\x65xclusiveMinimum\x18\x0f \x01(\x08\x12\x11\n\tmaxLength\x18\x10 \x01(\x05\x12\x11\n\tminLength\x18\x11 \x01(\x05\x12\x0f\n\x07pattern\x18\x12 \x01(\t\x12\x10\n\x08required\x18\x13 \x01(\x08\x12\x0f\n\x07\x65xample\x18\x14 \x01(\t\x12\x14\n\x0c\x65xternalDocs\x18\x15 \x01(\t\x12\x0c\n\x04\x65num\x18\x16 \x03(\t\x12\x10\n\x08maxItems\x18\x18 \x01(\x05\x12\x10\n\x08minItems\x18\x19 \x01(\x05\x12\x13\n\x0buniqueItems\x18\x1a \x01(\x08\x12\x0b\n\x03pii\x18\x1c \x01(\x08\x12\x0b\n\x03phi\x18\x1d \x01(\x08\x12\x11\n\tprotected\x18\x1f \x01(\x08\x12\x17\n\x0f\x64\x65\x66\x61ultValueNum\x18  \x01(\x01\x12\x0b\n\x03log\x18! \x01(\x08\x12\n\n\x02mu\x18\" \x01(\x01\x12\r\n\x05sigma\x18# \x01(\x01\x12\x15\n\rskewThreshold\x18$ \x01(\x01\x12\x16\n\x0e\x64riftThreshold\x18% \x01(\x01\x12\x0b\n\x03key\x18& \x01(\x08\x12\x0c\n\x04\x66old\x18\' \x01(\x08\x12\x0e\n\x06weight\x18( \x01(\x08\x12\x10\n\x08reserved\x18) \x01(\x08\x12\x12\n\nimputation\x18* \x01(\t\x12\x0f\n\x07scaling\x18+ \x01(\t\x12\x11\n\tgenerated\x18, \x01(\x08\x12\x0f\n\x07\x66ormula\x18- \x01(\t\x12\n\n\x02id\x18. \x01(\x08\x12\x0c\n\x04step\x18/ \x01(\x01\x12\x0b\n\x03loc\x18\x30 \x01(\x05\x12\x16\n\x0e\x64\x61tetimeFormat\x18\x31 \x01(\t\x12\x12\n\ntimeseries\x18\x32 \x01(\x08\x12\x11\n\tregressor\x18\x33 \x01(\x08\x12\x17\n\x0flaggedRegressor\x18\x34 \x01(\x08\x12\x11\n\ttimeIndex\x18\x35 \x01(\x08\x12\x0c\n\x04\x61ggr\x18\x36 \x01(\t\x12\x0e\n\x06window\x18\x37 \x01(\x05\"\xe0\x01\n\x0f\x43olumnHistogram\x12\x0c\n\x04name\x18\x01 \x01(\t\x12Y\n\thistogram\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.HistogramData\x12U\n\x07metrics\x18\x03 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12\r\n\x05\x64rift\x18\x04 \x01(\x08\"\x81\x01\n\nColumnSpec\x12\x0e\n\x06spacer\x18\x01 \x01(\x08\x12\r\n\x05width\x18\x02 \x01(\x05\x12T\n\x07\x63ontent\x18\x03 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ComponentSpec\"\x92\x07\n\x10\x43olumnStatistics\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\r\n\x05\x63ount\x18\x03 \x01(\x01\x12\x10\n\x08\x64istinct\x18\x04 \x01(\x05\x12\x0f\n\x07missing\x18\x05 \x01(\x05\x12\x16\n\x0epercentMissing\x18\x06 \x01(\x01\x12\x0c\n\x04mean\x18\x07 \x01(\x01\x12\x0e\n\x06stddev\x18\x08 \x01(\x01\x12\x10\n\x08variance\x18\t \x01(\x01\x12\x0b\n\x03min\x18\n \x01(\x01\x12\x0b\n\x03max\x18\x0b \x01(\x01\x12\x10\n\x08kurtosis\x18\x0c \x01(\x01\x12\x10\n\x08skewness\x18\r \x01(\x01\x12\x0b\n\x03sum\x18\x0e \x01(\x01\x12\x0b\n\x03mad\x18\x0f \x01(\x01\x12\x0b\n\x03p25\x18\x10 \x01(\x01\x12\x0b\n\x03p50\x18\x11 \x01(\x01\x12\x0b\n\x03p75\x18\x12 \x01(\x01\x12\x0b\n\x03iqr\x18\x13 \x01(\x01\x12\x0c\n\x04mode\x18\x14 \x01(\t\x12\r\n\x05zeros\x18\x15 \x01(\x01\x12\x0f\n\x07invalid\x18\x16 \x01(\x05\x12\x12\n\nimportance\x18\x17 \x01(\x01\x12\x0e\n\x06target\x18\x18 \x01(\x08\x12\x0e\n\x06ignore\x18\x19 \x01(\x08\x12\x10\n\x08nullable\x18\x1a \x01(\x08\x12\x17\n\x0fhighCardinality\x18\x1b \x01(\x08\x12!\n\x19highCorrWithOtherFeatures\x18\x1c \x01(\x08\x12\x19\n\x11lowCorrWithTarget\x18\x1d \x01(\x08\x12\x16\n\x0ehighMissingPct\x18\x1e \x01(\x08\x12\x0e\n\x06skewed\x18\x1f \x01(\x08\x12\n\n\x02id\x18  \x01(\x08\x12\x10\n\x08\x63onstant\x18! \x01(\x08\x12\x11\n\tduplicate\x18\" \x01(\x08\x12\x10\n\x08reserved\x18# \x01(\x08\x12\x14\n\x0c\x63ompleteness\x18% \x01(\x01\x12\x1a\n\x12\x64istinctValueCount\x18& \x01(\x01\x12\x1b\n\x13mostFreqValuesRatio\x18\' \x01(\x01\x12Y\n\thistogram\x18) \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.HistogramData\x12\x14\n\x0c\x63orrToTarget\x18* \x01(\x01\x12\r\n\x05index\x18+ \x01(\x05\x12S\n\x08outliers\x18, \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.OutlierStat\"\x96\x01\n\rComponentSpec\x12\r\n\x05title\x18\x01 \x01(\t\x12\x10\n\x08subtitle\x18\x02 \x01(\t\x12\x0e\n\x06\x66ooter\x18\x03 \x01(\t\x12T\n\x07\x63ontent\x18\x04 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ComponentView\"\xe3\x04\n\rComponentView\x12P\n\x06metric\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.MetricSpec\x12N\n\x05gauge\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GaugeSpec\x12V\n\thistogram\x18\x03 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.HistogramSpec\x12N\n\x05table\x18\x04 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.TableSpec\x12V\n\tlineChart\x18\x05 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LineChartSpec\x12T\n\x08\x62\x61rChart\x18\x06 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.BarChartSpec\x12Z\n\x0bscatterPlot\x18\x07 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ScatterPlotSpec\"P\n\x0b\x43orrelation\x12\x10\n\x08\x66\x65\x61ture1\x18\x01 \x01(\t\x12\x10\n\x08\x66\x65\x61ture2\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\x01\x12\x0e\n\x06method\x18\x04 \x01(\t\">\n\x0f\x43orrelationSpec\x12\x0e\n\x06\x63utoff\x18\x01 \x01(\x01\x12\x0e\n\x06method\x18\x02 \x01(\t\x12\x0b\n\x03top\x18\x03 \x01(\x05\"\xef\x01\n\x0b\x43svFileSpec\x12\x11\n\tdelimiter\x18\x01 \x01(\t\x12\r\n\x05quote\x18\x03 \x01(\t\x12\x12\n\nescapeChar\x18\x04 \x01(\t\x12\x14\n\x0c\x63ommentChars\x18\x05 \x01(\t\x12\x0e\n\x06header\x18\x06 \x01(\x08\x12\x10\n\x08skipRows\x18\x07 \x01(\x05\x12\x12\n\nnullValues\x18\x08 \x01(\t\x12\x10\n\x08\x65ncoding\x18\t \x01(\t\x12\x0f\n\x07maxRows\x18\n \x01(\x05\x12\x0e\n\x06strict\x18\x0b \x01(\x08\x12\x13\n\x0b\x63ompression\x18\x0c \x01(\t\x12\x16\n\x0ehasIndexColumn\x18\r \x01(\x08\"\xd2\x01\n\rDataInputSpec\x12\x0e\n\x06preSQL\x18\x01 \x03(\t\x12W\n\x08location\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12X\n\x06\x66ormat\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\"\x8c\x02\n\x0e\x44\x61taOutputSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12W\n\x08location\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x0e\n\x06\x66ormat\x18\x03 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\t\x12\x1d\n\x15\x63reateTableIfNotExist\x18\x05 \x01(\x08\x12\x17\n\x0fincludeFeatures\x18\x06 \x01(\x08\x12\x0b\n\x03xai\x18\x07 \x01(\x08\x12\x16\n\x0e\x64\x65tectOutliers\x18\x08 \x01(\x08\x12\x0f\n\x07postSQL\x18\t \x03(\t\"\x82\x02\n\x0c\x44\x61taPipeline\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12T\n\x04spec\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineSpec\x12X\n\x06status\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineStatus\"\xa7\x01\n\x10\x44\x61taPipelineList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Q\n\x05items\x18\x02 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipeline\"\x8b\x02\n\x0f\x44\x61taPipelineRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12W\n\x04spec\x18\x02 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineRunSpec\x12[\n\x06status\x18\x03 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineRunStatus\"\xa1\x01\n\x18\x44\x61taPipelineRunCondition\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x46\n\x12lastTransitionTime\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x06 \x01(\t\"\xad\x01\n\x13\x44\x61taPipelineRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12T\n\x05items\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineRun\"\xc8\x02\n\x13\x44\x61taPipelineRunSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x18\n\x10\x64\x61tapipelineName\x18\x02 \x01(\t\x12\r\n\x05owner\x18\x04 \x01(\t\x12X\n\tresources\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x10\n\x08priority\x18\x06 \x01(\t\x12\x0e\n\x06paused\x18\x07 \x01(\x08\x12\x0f\n\x07\x61\x62orted\x18\x08 \x01(\x08\x12\x33\n\x06labRef\x18\t \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x16\n\x0emodelClassName\x18\n \x01(\t\x12\x19\n\x11modelClassRunName\x18\x0b \x01(\t\"\x80\x04\n\x15\x44\x61taPipelineRunStatus\x12\x12\n\nrecipeRuns\x18\x01 \x03(\t\x12U\n\x06output\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\r\n\x05phase\x18\x03 \x01(\t\x12?\n\x0b\x63ompletedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x06 \x01(\x03\x12\x15\n\rfailureReason\x18\x07 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x08 \x01(\t\x12\x10\n\x08progress\x18\t \x01(\x05\x12K\n\x04logs\x18\n \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12=\n\tupdatedAt\x18\x0b \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\nconditions\x18\x0c \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x80\x06\n\x10\x44\x61taPipelineSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x16\n\x0emodelClassName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12t\n\x0f\x64\x61tasetSelector\x18\x04 \x03(\x0b\x32[.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipelineSpec.DatasetSelectorEntry\x12U\n\x07recipes\x18\x05 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipePartSpec\x12T\n\x06output\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataOutputSpec\x12V\n\x08schedule\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12_\n\x0cnotification\x18\x08 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\r\n\x05owner\x18\t \x01(\t\x12X\n\tresources\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x10\n\x08priority\x18\x0b \x01(\t\x12\x0e\n\x06paused\x18\x0c \x01(\x08\x12\x0b\n\x03ttl\x18\r \x01(\x05\x1a\x36\n\x14\x44\x61tasetSelectorEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xba\x02\n\x12\x44\x61taPipelineStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\\\n\x08schedule\x18\x03 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12\x13\n\x0blastRunName\x18\x04 \x01(\t\x12\x11\n\trunsCount\x18\x05 \x01(\x05\x12\x43\n\nconditions\x18\x06 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xff\x01\n\x0b\x44\x61taProduct\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12S\n\x04spec\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductSpec\x12W\n\x06status\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductStatus\"\xa5\x01\n\x0f\x44\x61taProductList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12P\n\x05items\x18\x02 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\"\xc4\x07\n\x0f\x44\x61taProductSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x0e\n\x06public\x18\x02 \x01(\x08\x12\x36\n\ttenantRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12V\n\x0bgitLocation\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GitLocation\x12Z\n\rimageLocation\x18\x05 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ImageLocation\x12\x17\n\x0f\x63\x61\x63heBucketName\x18\x06 \x01(\t\x12\x16\n\x0e\x64\x65\x66\x61ultLabName\x18\x07 \x01(\t\x12\x1e\n\x16\x64\x65\x66\x61ultServingSiteName\x18\x08 \x01(\t\x12\x19\n\x11\x64\x65\x66\x61ultBucketName\x18\t \x01(\t\x12\x0c\n\x04task\x18\n \x01(\t\x12\x0f\n\x07subtask\x18\x0b \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x0c \x01(\t\x12_\n\x0cnotification\x18\r \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12`\n\x11trainingResources\x18\x0e \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12_\n\x10servingResources\x18\x0f \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x10\n\x08priority\x18\x10 \x01(\t\x12\r\n\x05\x63olor\x18\x11 \x01(\t\x12T\n\x08\x61pproval\x18\x12 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ApprovalSpec\x12]\n\x0bpermissions\x18\x13 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PermissionsSpec\x12\x0c\n\x04tags\x18\x14 \x03(\t\"\xa9\x04\n\x11\x44\x61taProductStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x18\n\x10\x64\x61tasourcesCount\x18\x03 \x01(\x05\x12\x15\n\rdatasetsCount\x18\x04 \x01(\x05\x12\x19\n\x11\x64\x61taPipelineCount\x18\x05 \x01(\x05\x12\x1d\n\x15totalDataPipelineRuns\x18\x06 \x01(\x05\x12\x14\n\x0cstudiesCount\x18\x07 \x01(\x05\x12\x13\n\x0bmodelsCount\x18\x08 \x01(\x05\x12\x17\n\x0fpredictorsCount\x18\x0b \x01(\x05\x12\x15\n\rdataAppsCount\x18\r \x01(\x05\x12\x18\n\x10predictionsCount\x18\x0e \x01(\x05\x12\x17\n\x0finfoAlertsCount\x18\x0f \x01(\x05\x12\x18\n\x10\x65rrorAlertsCount\x18\x10 \x01(\x05\x12\x19\n\x11modelClassesCount\x18\x11 \x01(\x05\x12\x15\n\rfailureReason\x18\x12 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x13 \x01(\t\x12\x17\n\x0f\x62\x61selineVersion\x18\x14 \x01(\t\x12\x43\n\nconditions\x18\x15 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x94\x02\n\x12\x44\x61taProductVersion\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Z\n\x04spec\x18\x02 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersionSpec\x12^\n\x06status\x18\x03 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersionStatus\"\xb3\x01\n\x16\x44\x61taProductVersionList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12W\n\x05items\x18\x02 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\"\xa0\x01\n\x16\x44\x61taProductVersionSpec\x12\x37\n\nproductRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x17\n\x0fprevVersionName\x18\x03 \x01(\t\x12\x10\n\x08\x62\x61seline\x18\x04 \x01(\x08\x12\r\n\x05owner\x18\x05 \x01(\t\"\xe9\x01\n\x18\x44\x61taProductVersionStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x03 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x04 \x01(\t\x12\x43\n\nconditions\x18\x05 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xfc\x01\n\nDataSource\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12R\n\x04spec\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSourceSpec\x12V\n\x06status\x18\x03 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSourceStatus\"\xa3\x01\n\x0e\x44\x61taSourceList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12O\n\x05items\x18\x02 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\"\x91\x06\n\x0e\x44\x61taSourceSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x61tasetType\x18\x04 \x01(\t\x12L\n\x06schema\x18\x05 \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Schema\x12Z\n\x08\x66latfile\x18\x06 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\x12\x0f\n\x07labeled\x18\x07 \x01(\x08\x12P\n\x06sample\x18\t \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SampleSpec\x12\x0c\n\x04task\x18\n \x01(\t\x12\x0f\n\x07subtask\x18\x0b \x01(\t\x12]\n\rrelationships\x18\x0c \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RelationshipSpec\x12T\n\x08labeling\x18\r \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingSpec\x12[\n\x0cinferredFrom\x18\x0e \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12]\n\x11unitTestsTemplate\x18\x0f \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12\x14\n\x0cingestMethod\x18\x10 \x01(\t\"\xd2\x02\n\x10\x44\x61taSourceStatus\x12\x0c\n\x04\x63ols\x18\x01 \x01(\x05\x12\x1a\n\x12observedGeneration\x18\x02 \x01(\x03\x12H\n\x14lastDatasetCreatedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x17\n\x0flastDatasetName\x18\x04 \x01(\t\x12=\n\tupdatedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x06 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x07 \x01(\t\x12\x43\n\nconditions\x18\x08 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xf3\x01\n\x07\x44\x61taset\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12O\n\x04spec\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSpec\x12S\n\x06status\x18\x03 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetStatus\"\xe0\x01\n\x14\x44\x61tasetGroupByStatus\x12\x13\n\x0b\x64\x61tasetsURI\x18\x01 \x01(\t\x12\x13\n\x0bprofilesURI\x18\x02 \x01(\t\x12\x12\n\nreportsURI\x18\x03 \x01(\t\x12\x14\n\x0cunitTestsURI\x18\x04 \x01(\t\x12\x13\n\x0b\x66\x65\x61turesURI\x18\x05 \x01(\t\x12_\n\rworkerResults\x18\x06 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"\x9d\x01\n\x0b\x44\x61tasetList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12L\n\x05items\x18\x02 \x03(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"\x99\x0c\n\x0b\x44\x61tasetSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x16\n\x0e\x64\x61taSourceName\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12\x13\n\x0b\x64isplayName\x18\x08 \x01(\t\x12\x0c\n\x04role\x18\t \x01(\t\x12\x0c\n\x04tags\x18\n \x03(\t\x12\x0e\n\x06report\x18\x0b \x01(\x08\x12\x10\n\x08unitTest\x18\x0c \x01(\x08\x12U\n\x06origin\x18\r \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12W\n\x08location\x18\x0e \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x1a\n\x12\x61rtifactBucketName\x18\x0f \x01(\t\x12X\n\tresources\x18\x10 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0f\n\x07timeout\x18\x11 \x01(\x03\x12\x0c\n\x04type\x18\x12 \x01(\t\x12P\n\x06sample\x18\x13 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SampleSpec\x12V\n\tsynthetic\x18\x14 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SyntheticSpec\x12\x0c\n\x04task\x18\x15 \x01(\t\x12\x0f\n\x07subtask\x18\x16 \x01(\t\x12Z\n\x0b\x63orrelation\x18\x17 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.CorrelationSpec\x12\x0c\n\x04\x66\x61st\x18\x18 \x01(\x08\x12\x11\n\tfeaturize\x18\x19 \x01(\x08\x12\x33\n\x06labRef\x18\x1a \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12>\n\x11servingDatasetRef\x18\x1b \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x39\n\x0cpredictorRef\x18\x1c \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12 \n\x18generateFeatureHistogram\x18\x1d \x01(\x08\x12U\n\tunitTests\x18\x1e \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12R\n\x07groupBy\x18\x1f \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GroupBySpec\x12g\n\x0egroupLocations\x18  \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.GroupDatasetLocationsSpec\x12\x0b\n\x03key\x18! \x03(\t\x12\x16\n\x0emodelClassName\x18\" \x01(\t\x12\x19\n\x11modelClassRunName\x18# \x01(\t\x12:\n\rfeatureGroups\x18$ \x03(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x18\n\x10\x66\x65\x61tureGroupName\x18% \x01(\t\x12_\n\x0cnotification\x18& \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\"\xd9\x02\n\x11\x44\x61tasetStatistics\x12W\n\x07\x63olumns\x18\x01 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ColumnStatistics\x12\x0c\n\x04rows\x18\x03 \x01(\x05\x12\x0c\n\x04\x63ols\x18\x04 \x01(\x05\x12\x10\n\x08\x66ileSize\x18\x05 \x01(\x05\x12\x61\n\x16\x63orrelationsWithTarget\x18\x06 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\x12Z\n\x0ftopCorrelations\x18\x07 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\"\xbe\t\n\rDatasetStatus\x12[\n\nstatistics\x18\x01 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetStatistics\x12\r\n\x05phase\x18\x02 \x01(\t\x12\x12\n\nreportName\x18\x03 \x01(\t\x12]\n\x0ereportLocation\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12^\n\x0fprofileLocation\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12`\n\x11\x61nomaliesLocation\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x12\n\nimbalanced\x18\x07 \x01(\x08\x12\x1a\n\x12observedGeneration\x18\x08 \x01(\x03\x12\x61\n\x0funitTestResults\x18\t \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12?\n\x0blastStudyAt\x18\n \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x16\n\x0e\x66\x61ilureMessage\x18\r \x01(\t\x12\x10\n\x08progress\x18\x0e \x01(\x05\x12\x0c\n\x04hash\x18\x0f \x01(\t\x12K\n\x04logs\x18\x10 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12=\n\tupdatedAt\x18\x12 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12O\n\x06images\x18\x13 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Images\x12?\n\x0b\x63ompletedAt\x18\x15 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12@\n\x13\x66\x65\x61tureHistogramRef\x18\x16 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12[\n\x07groupby\x18\x17 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetGroupByStatus\x12\x43\n\nconditions\x18\x18 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xa6\x01\n\x0f\x44\x61tasetTemplate\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12O\n\x04spec\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSpec\"/\n\x0e\x44riftThreshold\x12\x0e\n\x06metric\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\"\xf0\x01\n\x06\x45ntity\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12N\n\x04spec\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.EntitySpec\x12R\n\x06status\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.EntityStatus\"\x9b\x01\n\nEntityList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12K\n\x05items\x18\x02 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Entity\"\x87\x01\n\nEntitySpec\x12\x36\n\ttenantRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0f\n\x07joinKey\x18\x04 \x01(\t\x12\r\n\x05owner\x18\x05 \x01(\t\x12\x0c\n\x04tags\x18\x06 \x03(\t\"\xae\x01\n\x0c\x45ntityStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\nconditions\x18\x03 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xc1\x01\n\x11\x45xcelNotebookSpec\x12\x1a\n\x12\x66irstSheetWithData\x18\x01 \x01(\x08\x12\x11\n\tsheetName\x18\x02 \x01(\t\x12\x12\n\nsheetIndex\x18\x03 \x01(\x05\x12\x15\n\rcolumnNameRow\x18\x04 \x01(\x05\x12R\n\x04\x64\x61ta\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ExcelSheetArea\"k\n\x0e\x45xcelSheetArea\x12\x13\n\x0b\x65ntireSheet\x18\x01 \x01(\x08\x12\x12\n\nfromColumn\x18\x02 \x01(\x05\x12\x10\n\x08toColumn\x18\x03 \x01(\x05\x12\x0f\n\x07\x66romRow\x18\x04 \x01(\x05\x12\r\n\x05toRow\x18\x05 \x01(\x05\"\x82\x02\n\x0c\x46\x65\x61tureGroup\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12T\n\x04spec\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroupSpec\x12X\n\x06status\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroupStatus\"\xa7\x01\n\x10\x46\x65\x61tureGroupList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Q\n\x05items\x18\x02 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\"\x84\x08\n\x10\x46\x65\x61tureGroupSpec\x12\x36\n\ttenantRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\r\n\x05owner\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x1a\n\x12\x61rtifactBucketName\x18\x04 \x01(\t\x12\x12\n\ningestType\x18\x05 \x01(\t\x12\x12\n\nentityName\x18\x06 \x01(\t\x12\x0c\n\x04tags\x18\x07 \x03(\t\x12\\\n\x0eingestSchedule\x18\x08 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12Z\n\x0csyncSchedule\x18\t \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12Z\n\x08\x66latfile\x18\n \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\x12L\n\x06schema\x18\x0b \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Schema\x12Q\n\x05tests\x18\x0c \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12W\n\x08location\x18\r \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x12\n\ntimeColumn\x18\x0e \x01(\t\x12\x18\n\x10timeColumnFormat\x18\x0f \x01(\t\x12\x11\n\tkeyColumn\x18\x10 \x01(\t\x12\x62\n\x0fmaterialization\x18\x11 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.MaterializationSpec\x12X\n\tresources\x18\x12 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x33\n\x06labRef\x18\x13 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\x85\x05\n\x12\x46\x65\x61tureGroupStatus\x12\r\n\x05phase\x18\x02 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x03 \x01(\x03\x12=\n\tupdatedAt\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0c\n\x04rows\x18\x05 \x01(\x05\x12\x62\n\x0eingestSchedule\x18\x07 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12`\n\x0csyncSchedule\x18\x08 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12Z\n\x0bonlineTable\x18\t \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x46\n\x12onlineTableCreated\x18\n \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x19\n\x11ingestDatasetName\x18\x0b \x01(\t\x12\x15\n\rfailureReason\x18\x0c \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\r \x01(\t\x12\x43\n\nconditions\x18\x0e \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x8e\x02\n\x10\x46\x65\x61tureHistogram\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12X\n\x04spec\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogramSpec\x12\\\n\x06status\x18\x03 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogramStatus\"\xaf\x01\n\x14\x46\x65\x61tureHistogramList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12U\n\x05items\x18\x02 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogram\"\xf5\x04\n\x14\x46\x65\x61tureHistogramSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x05 \x03(\t\x12\x36\n\tsourceRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08training\x18\x07 \x01(\x08\x12\x0c\n\x04live\x18\t \x01(\x08\x12\x39\n\x05start\x18\n \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x37\n\x03\x65nd\x18\x0b \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x34\n\x07\x62\x61seRef\x18\x0c \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12]\n\x0f\x64riftThresholds\x18\r \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DriftThreshold\x12\x17\n\x0fsyncIntervalSec\x18\x0e \x01(\x05\x12U\n\tunitTests\x18\x0f \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12\x14\n\x0cgenUnitTests\x18\x10 \x01(\x08\x12\x15\n\rfeatureFilter\x18\x11 \x01(\t\x12\x15\n\rreferenceType\x18\x12 \x01(\t\"\x9d\x04\n\x16\x46\x65\x61tureHistogramStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12V\n\x07\x63olumns\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ColumnHistogram\x12=\n\tupdatedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12K\n\x04logs\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12\r\n\x05phase\x18\x06 \x01(\t\x12\x15\n\rfailureReason\x18\x07 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x08 \x01(\t\x12\x61\n\x0funitTestsResult\x18\t \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\r\n\x05total\x18\n \x01(\x05\x12\x0e\n\x06\x65rrors\x18\x0b \x01(\x05\x12\x43\n\nconditions\x18\x0c \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xa6\x02\n\x12\x46latFileFormatSpec\x12\x10\n\x08\x66ileType\x18\x01 \x01(\t\x12N\n\x03\x63sv\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.CsvFileSpec\x12V\n\x05\x65xcel\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ExcelNotebookSpec\x12V\n\x07parquet\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ParquetFileSpec\"M\n\tGaugeSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\x0e\n\x06\x63olumn\x18\x02 \x01(\t\x12\x0b\n\x03row\x18\x03 \x01(\x05\x12\x0e\n\x06scalar\x18\x04 \x01(\t\"V\n\x0bGitLocation\x12\x19\n\x11gitConnectionName\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x03 \x01(\t\x12\x0f\n\x07private\x18\x04 \x01(\x08\"]\n\x0bGroupBySpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07groupby\x18\x02 \x03(\t\x12\x0c\n\x04\x66req\x18\x03 \x01(\t\x12\x10\n\x08interval\x18\x04 \x01(\x05\x12\x0c\n\x04\x61ggr\x18\x05 \x01(\t\"\xc2\x01\n\x19GroupDatasetLocationsSpec\x12\x12\n\ngroupsRoot\x18\x01 \x01(\t\x12\x11\n\tgroupRoot\x18\x02 \x01(\t\x12\x17\n\x0fgroupDataFolder\x18\x03 \x01(\t\x12\x15\n\rgroupDataFile\x18\x04 \x01(\t\x12\x1a\n\x12groupProfileFolder\x18\x05 \x01(\t\x12\x17\n\x0fgroupReportFile\x18\x06 \x01(\t\x12\x19\n\x11groupFeaturesFile\x18\x07 \x01(\t\"=\n\rHistogramSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\t\n\x01x\x18\x02 \x01(\t\x12\x0c\n\x04\x62ins\x18\x03 \x01(\x05\"=\n\rImageLocation\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1e\n\x16registryConnectionName\x18\x02 \x01(\t\"\"\n\x03KPI\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\"?\n\x0cLabelingRule\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\x10\n\x08operator\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\"\xe1\x01\n\x0cLabelingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x14\n\x0cresultColumn\x18\x02 \x01(\t\x12T\n\x08positive\x18\x03 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingRule\x12T\n\x08negative\x18\x04 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.LabelingRule\"J\n\rLineChartSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\t\n\x01x\x18\x02 \x01(\t\x12\t\n\x01y\x18\x03 \x01(\t\x12\x0e\n\x06legend\x18\x04 \x01(\x08\"\x86\x02\n\x13MaterializationSpec\x12\x0e\n\x06online\x18\x01 \x01(\x08\x12\x0f\n\x07offline\x18\x02 \x01(\x08\x12=\n\tstartDate\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x12\n\nofflineTTL\x18\x04 \x01(\x05\x12\x11\n\tonlineTTL\x18\x05 \x01(\x05\x12\x10\n\x08\x62\x61\x63kfill\x18\x06 \x01(\x05\x12V\n\x08schedule\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\"N\n\nMetricSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\x0e\n\x06\x63olumn\x18\x02 \x01(\t\x12\x0b\n\x03row\x18\x03 \x01(\x05\x12\x0e\n\x06scalar\x18\x04 \x01(\t\"<\n\x0bOutlierStat\x12\r\n\x05lower\x18\x01 \x01(\x05\x12\r\n\x05upper\x18\x02 \x01(\x05\x12\x0f\n\x07percent\x18\x03 \x01(\x02\"W\n\x08PageSpec\x12K\n\x04rows\x18\x01 \x03(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RowSpec\"!\n\x0fParquetFileSpec\x12\x0e\n\x06\x65ngine\x18\x01 \x01(\t\"\xf0\x01\n\x06Recipe\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12N\n\x04spec\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeSpec\x12R\n\x06status\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeStatus\"\x8f\x01\n\x0fRecipeInputSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12W\n\x08location\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x0e\n\x06\x66ormat\x18\x03 \x01(\t\"\x9b\x01\n\nRecipeList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12K\n\x05items\x18\x02 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Recipe\"\x97\x01\n\x10RecipeOutputSpec\x12\x15\n\rcreateDataset\x18\x01 \x01(\x08\x12\x13\n\x0b\x64\x61tasetName\x18\x02 \x01(\t\x12W\n\x08location\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"8\n\x0eRecipePartSpec\x12\x12\n\nrecipeName\x18\x01 \x01(\t\x12\x12\n\ndependents\x18\x02 \x03(\t\"\xf9\x01\n\tRecipeRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeRunSpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeRunStatus\"\xa1\x01\n\rRecipeRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeRun\"\xe0\x02\n\rRecipeRunSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x12\n\nrecipeName\x18\x02 \x01(\t\x12\x33\n\x06labRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12W\n\x08location\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12X\n\tresources\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0b\n\x03ttl\x18\x06 \x01(\x05\x12\x16\n\x0emodelClassName\x18\x07 \x01(\t\x12\x19\n\x11modelClassRunName\x18\x08 \x01(\t\"\x92\x03\n\x0fRecipeRunStatus\x12?\n\x0b\x63ompletedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x02 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x03 \x01(\x03\x12\x15\n\rfailureReason\x18\x04 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x05 \x01(\t\x12\x13\n\x0btriggeredBy\x18\x06 \x01(\t\x12K\n\x04logs\x18\x07 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12=\n\tupdatedAt\x18\t \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\nconditions\x18\x0b \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xed\x04\n\nRecipeSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12T\n\x05input\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeInputSpec\x12O\n\x05steps\x18\x05 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeStep\x12V\n\x06output\x18\x06 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeOutputSpec\x12P\n\x06sample\x18\x07 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.SampleSpec\x12X\n\tresources\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0f\n\x07timeout\x18\n \x01(\x03\x12\x0b\n\x03ttl\x18\x0b \x01(\x05\x12]\n\x11unitTestsTemplate\x18\x0c \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\"\x87\x02\n\x0cRecipeStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12W\n\x07lastRun\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.LastRunStatus\x12=\n\tupdatedAt\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\nconditions\x18\x07 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"s\n\nRecipeStep\x12\n\n\x02op\x18\x01 \x01(\t\x12Y\n\nparameters\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeStepParam\".\n\x0fRecipeStepParam\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"X\n\x14RecommendationSchema\x12\x14\n\x0cuserIDColumn\x18\x01 \x01(\t\x12\x14\n\x0citemIDColumn\x18\x02 \x01(\t\x12\x14\n\x0cratingColumn\x18\x03 \x01(\t\"R\n\x10RelationshipSpec\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06\x63olumn\x18\x02 \x01(\t\x12\r\n\x05\x61rity\x18\x03 \x01(\t\x12\x11\n\trelatesTo\x18\x04 \x01(\t\"Y\n\x07RowSpec\x12N\n\x04\x63ols\x18\x01 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ColumnSpec\"j\n\nSampleSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0c\n\x04rows\x18\x03 \x01(\x05\x12\x0f\n\x07percent\x18\x04 \x01(\x05\x12\x0e\n\x06\x66ilter\x18\x05 \x01(\t\x12\x0e\n\x06\x63olumn\x18\x06 \x01(\t\"<\n\x0fScatterPlotSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\t\n\x01x\x18\x02 \x01(\t\x12\t\n\x01y\x18\x03 \x01(\t\"\xb0\x02\n\x06Schema\x12`\n\x10timeSeriesSchema\x18\x01 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.TimeSeriesSchema\x12h\n\x14recommendationSchema\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecommendationSchema\x12M\n\x07\x63olumns\x18\x03 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Column\x12\x0b\n\x03key\x18\x04 \x03(\t\".\n\rSyntheticSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04rows\x18\x02 \x01(\x05\"\x84\x01\n\tTableSpec\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x02 \x03(\t\x12\x0f\n\x07\x66ilters\x18\x03 \x03(\t\x12\x0f\n\x07groupby\x18\x04 \x03(\t\x12\x0c\n\x04rows\x18\x05 \x01(\x05\x12\x11\n\tshowIndex\x18\x06 \x01(\x08\x12\x0e\n\x06\x62order\x18\x07 \x01(\x08\"@\n\x10TimeSeriesSchema\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0c\n\x04\x66req\x18\x02 \x01(\t\x12\x10\n\x08interval\x18\x03 \x01(\x05\x42\x36Z4github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.generated_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z4github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1'
@@ -39,187 +39,187 @@
   _COLUMN._serialized_start=821
   _COLUMN._serialized_end=1749
   _COLUMNHISTOGRAM._serialized_start=1752
   _COLUMNHISTOGRAM._serialized_end=1976
   _COLUMNSPEC._serialized_start=1979
   _COLUMNSPEC._serialized_end=2108
   _COLUMNSTATISTICS._serialized_start=2111
-  _COLUMNSTATISTICS._serialized_end=3053
-  _COMPONENTSPEC._serialized_start=3056
-  _COMPONENTSPEC._serialized_end=3206
-  _COMPONENTVIEW._serialized_start=3209
-  _COMPONENTVIEW._serialized_end=3820
-  _CORRELATION._serialized_start=3822
-  _CORRELATION._serialized_end=3902
-  _CORRELATIONSPEC._serialized_start=3904
-  _CORRELATIONSPEC._serialized_end=3966
-  _CSVFILESPEC._serialized_start=3969
-  _CSVFILESPEC._serialized_end=4208
-  _DATAINPUTSPEC._serialized_start=4211
-  _DATAINPUTSPEC._serialized_end=4421
-  _DATAOUTPUTSPEC._serialized_start=4424
-  _DATAOUTPUTSPEC._serialized_end=4692
-  _DATAPIPELINE._serialized_start=4695
-  _DATAPIPELINE._serialized_end=4953
-  _DATAPIPELINELIST._serialized_start=4956
-  _DATAPIPELINELIST._serialized_end=5123
-  _DATAPIPELINERUN._serialized_start=5126
-  _DATAPIPELINERUN._serialized_end=5393
-  _DATAPIPELINERUNCONDITION._serialized_start=5396
-  _DATAPIPELINERUNCONDITION._serialized_end=5557
-  _DATAPIPELINERUNLIST._serialized_start=5560
-  _DATAPIPELINERUNLIST._serialized_end=5733
-  _DATAPIPELINERUNSPEC._serialized_start=5736
-  _DATAPIPELINERUNSPEC._serialized_end=6064
-  _DATAPIPELINERUNSTATUS._serialized_start=6067
-  _DATAPIPELINERUNSTATUS._serialized_end=6579
-  _DATAPIPELINESPEC._serialized_start=6582
-  _DATAPIPELINESPEC._serialized_end=7350
-  _DATAPIPELINESPEC_DATASETSELECTORENTRY._serialized_start=7296
-  _DATAPIPELINESPEC_DATASETSELECTORENTRY._serialized_end=7350
-  _DATAPIPELINESTATUS._serialized_start=7353
-  _DATAPIPELINESTATUS._serialized_end=7667
-  _DATAPRODUCT._serialized_start=7670
-  _DATAPRODUCT._serialized_end=7925
-  _DATAPRODUCTLIST._serialized_start=7928
-  _DATAPRODUCTLIST._serialized_end=8093
-  _DATAPRODUCTSPEC._serialized_start=8096
-  _DATAPRODUCTSPEC._serialized_end=9061
-  _DATAPRODUCTSTATUS._serialized_start=9064
-  _DATAPRODUCTSTATUS._serialized_end=9617
-  _DATAPRODUCTVERSION._serialized_start=9620
-  _DATAPRODUCTVERSION._serialized_end=9896
-  _DATAPRODUCTVERSIONLIST._serialized_start=9899
-  _DATAPRODUCTVERSIONLIST._serialized_end=10078
-  _DATAPRODUCTVERSIONSPEC._serialized_start=10081
-  _DATAPRODUCTVERSIONSPEC._serialized_end=10241
-  _DATAPRODUCTVERSIONSTATUS._serialized_start=10244
-  _DATAPRODUCTVERSIONSTATUS._serialized_end=10477
-  _DATASOURCE._serialized_start=10480
-  _DATASOURCE._serialized_end=10732
-  _DATASOURCELIST._serialized_start=10735
-  _DATASOURCELIST._serialized_end=10898
-  _DATASOURCESPEC._serialized_start=10901
-  _DATASOURCESPEC._serialized_end=11686
-  _DATASOURCESTATUS._serialized_start=11689
-  _DATASOURCESTATUS._serialized_end=12027
-  _DATASET._serialized_start=12030
-  _DATASET._serialized_end=12273
-  _DATASETGROUPBYSTATUS._serialized_start=12276
-  _DATASETGROUPBYSTATUS._serialized_end=12500
-  _DATASETLIST._serialized_start=12503
-  _DATASETLIST._serialized_end=12660
-  _DATASETSPEC._serialized_start=12663
-  _DATASETSPEC._serialized_end=14127
-  _DATASETSTATISTICS._serialized_start=14130
-  _DATASETSTATISTICS._serialized_end=14475
-  _DATASETSTATUS._serialized_start=14478
-  _DATASETSTATUS._serialized_end=15739
-  _DATASETTEMPLATE._serialized_start=15742
-  _DATASETTEMPLATE._serialized_end=15908
-  _DRIFTTHRESHOLD._serialized_start=15910
-  _DRIFTTHRESHOLD._serialized_end=15957
-  _ENTITY._serialized_start=15960
-  _ENTITY._serialized_end=16200
-  _ENTITYLIST._serialized_start=16203
-  _ENTITYLIST._serialized_end=16358
-  _ENTITYSPEC._serialized_start=16361
-  _ENTITYSPEC._serialized_end=16496
-  _ENTITYSTATUS._serialized_start=16499
-  _ENTITYSTATUS._serialized_end=16673
-  _EXCELNOTEBOOKSPEC._serialized_start=16676
-  _EXCELNOTEBOOKSPEC._serialized_end=16869
-  _EXCELSHEETAREA._serialized_start=16871
-  _EXCELSHEETAREA._serialized_end=16978
-  _FEATUREGROUP._serialized_start=16981
-  _FEATUREGROUP._serialized_end=17239
-  _FEATUREGROUPLIST._serialized_start=17242
-  _FEATUREGROUPLIST._serialized_end=17409
-  _FEATUREGROUPSPEC._serialized_start=17412
-  _FEATUREGROUPSPEC._serialized_end=18440
-  _FEATUREGROUPSTATUS._serialized_start=18443
-  _FEATUREGROUPSTATUS._serialized_end=19088
-  _FEATUREHISTOGRAM._serialized_start=19091
-  _FEATUREHISTOGRAM._serialized_end=19361
-  _FEATUREHISTOGRAMLIST._serialized_start=19364
-  _FEATUREHISTOGRAMLIST._serialized_end=19539
-  _FEATUREHISTOGRAMSPEC._serialized_start=19542
-  _FEATUREHISTOGRAMSPEC._serialized_end=20171
-  _FEATUREHISTOGRAMSTATUS._serialized_start=20174
-  _FEATUREHISTOGRAMSTATUS._serialized_end=20715
-  _FLATFILEFORMATSPEC._serialized_start=20718
-  _FLATFILEFORMATSPEC._serialized_end=21012
-  _GAUGESPEC._serialized_start=21014
-  _GAUGESPEC._serialized_end=21091
-  _GITLOCATION._serialized_start=21093
-  _GITLOCATION._serialized_end=21179
-  _GROUPBYSPEC._serialized_start=21181
-  _GROUPBYSPEC._serialized_end=21274
-  _GROUPDATASETLOCATIONSSPEC._serialized_start=21277
-  _GROUPDATASETLOCATIONSSPEC._serialized_end=21471
-  _HISTOGRAMSPEC._serialized_start=21473
-  _HISTOGRAMSPEC._serialized_end=21534
-  _IMAGELOCATION._serialized_start=21536
-  _IMAGELOCATION._serialized_end=21597
-  _KPI._serialized_start=21599
-  _KPI._serialized_end=21633
-  _LABELINGRULE._serialized_start=21635
-  _LABELINGRULE._serialized_end=21698
-  _LABELINGSPEC._serialized_start=21701
-  _LABELINGSPEC._serialized_end=21926
-  _LINECHARTSPEC._serialized_start=21928
-  _LINECHARTSPEC._serialized_end=22002
-  _MATERIALIZATIONSPEC._serialized_start=22005
-  _MATERIALIZATIONSPEC._serialized_end=22267
-  _METRICSPEC._serialized_start=22269
-  _METRICSPEC._serialized_end=22347
-  _OUTLIERSTAT._serialized_start=22349
-  _OUTLIERSTAT._serialized_end=22409
-  _PAGESPEC._serialized_start=22411
-  _PAGESPEC._serialized_end=22498
-  _PARQUETFILESPEC._serialized_start=22500
-  _PARQUETFILESPEC._serialized_end=22533
-  _RECIPE._serialized_start=22536
-  _RECIPE._serialized_end=22776
-  _RECIPEINPUTSPEC._serialized_start=22779
-  _RECIPEINPUTSPEC._serialized_end=22922
-  _RECIPELIST._serialized_start=22925
-  _RECIPELIST._serialized_end=23080
-  _RECIPEOUTPUTSPEC._serialized_start=23083
-  _RECIPEOUTPUTSPEC._serialized_end=23234
-  _RECIPEPARTSPEC._serialized_start=23236
-  _RECIPEPARTSPEC._serialized_end=23292
-  _RECIPERUN._serialized_start=23295
-  _RECIPERUN._serialized_end=23544
-  _RECIPERUNLIST._serialized_start=23547
-  _RECIPERUNLIST._serialized_end=23708
-  _RECIPERUNSPEC._serialized_start=23711
-  _RECIPERUNSPEC._serialized_end=24063
-  _RECIPERUNSTATUS._serialized_start=24066
-  _RECIPERUNSTATUS._serialized_end=24468
-  _RECIPESPEC._serialized_start=24471
-  _RECIPESPEC._serialized_end=25092
-  _RECIPESTATUS._serialized_start=25095
-  _RECIPESTATUS._serialized_end=25358
-  _RECIPESTEP._serialized_start=25360
-  _RECIPESTEP._serialized_end=25475
-  _RECIPESTEPPARAM._serialized_start=25477
-  _RECIPESTEPPARAM._serialized_end=25523
-  _RECOMMENDATIONSCHEMA._serialized_start=25525
-  _RECOMMENDATIONSCHEMA._serialized_end=25613
-  _RELATIONSHIPSPEC._serialized_start=25615
-  _RELATIONSHIPSPEC._serialized_end=25697
-  _ROWSPEC._serialized_start=25699
-  _ROWSPEC._serialized_end=25788
-  _SAMPLESPEC._serialized_start=25790
-  _SAMPLESPEC._serialized_end=25896
-  _SCATTERPLOTSPEC._serialized_start=25898
-  _SCATTERPLOTSPEC._serialized_end=25958
-  _SCHEMA._serialized_start=25961
-  _SCHEMA._serialized_end=26265
-  _SYNTHETICSPEC._serialized_start=26267
-  _SYNTHETICSPEC._serialized_end=26313
-  _TABLESPEC._serialized_start=26316
-  _TABLESPEC._serialized_end=26448
-  _TIMESERIESSCHEMA._serialized_start=26450
-  _TIMESERIESSCHEMA._serialized_end=26514
+  _COLUMNSTATISTICS._serialized_end=3025
+  _COMPONENTSPEC._serialized_start=3028
+  _COMPONENTSPEC._serialized_end=3178
+  _COMPONENTVIEW._serialized_start=3181
+  _COMPONENTVIEW._serialized_end=3792
+  _CORRELATION._serialized_start=3794
+  _CORRELATION._serialized_end=3874
+  _CORRELATIONSPEC._serialized_start=3876
+  _CORRELATIONSPEC._serialized_end=3938
+  _CSVFILESPEC._serialized_start=3941
+  _CSVFILESPEC._serialized_end=4180
+  _DATAINPUTSPEC._serialized_start=4183
+  _DATAINPUTSPEC._serialized_end=4393
+  _DATAOUTPUTSPEC._serialized_start=4396
+  _DATAOUTPUTSPEC._serialized_end=4664
+  _DATAPIPELINE._serialized_start=4667
+  _DATAPIPELINE._serialized_end=4925
+  _DATAPIPELINELIST._serialized_start=4928
+  _DATAPIPELINELIST._serialized_end=5095
+  _DATAPIPELINERUN._serialized_start=5098
+  _DATAPIPELINERUN._serialized_end=5365
+  _DATAPIPELINERUNCONDITION._serialized_start=5368
+  _DATAPIPELINERUNCONDITION._serialized_end=5529
+  _DATAPIPELINERUNLIST._serialized_start=5532
+  _DATAPIPELINERUNLIST._serialized_end=5705
+  _DATAPIPELINERUNSPEC._serialized_start=5708
+  _DATAPIPELINERUNSPEC._serialized_end=6036
+  _DATAPIPELINERUNSTATUS._serialized_start=6039
+  _DATAPIPELINERUNSTATUS._serialized_end=6551
+  _DATAPIPELINESPEC._serialized_start=6554
+  _DATAPIPELINESPEC._serialized_end=7322
+  _DATAPIPELINESPEC_DATASETSELECTORENTRY._serialized_start=7268
+  _DATAPIPELINESPEC_DATASETSELECTORENTRY._serialized_end=7322
+  _DATAPIPELINESTATUS._serialized_start=7325
+  _DATAPIPELINESTATUS._serialized_end=7639
+  _DATAPRODUCT._serialized_start=7642
+  _DATAPRODUCT._serialized_end=7897
+  _DATAPRODUCTLIST._serialized_start=7900
+  _DATAPRODUCTLIST._serialized_end=8065
+  _DATAPRODUCTSPEC._serialized_start=8068
+  _DATAPRODUCTSPEC._serialized_end=9032
+  _DATAPRODUCTSTATUS._serialized_start=9035
+  _DATAPRODUCTSTATUS._serialized_end=9588
+  _DATAPRODUCTVERSION._serialized_start=9591
+  _DATAPRODUCTVERSION._serialized_end=9867
+  _DATAPRODUCTVERSIONLIST._serialized_start=9870
+  _DATAPRODUCTVERSIONLIST._serialized_end=10049
+  _DATAPRODUCTVERSIONSPEC._serialized_start=10052
+  _DATAPRODUCTVERSIONSPEC._serialized_end=10212
+  _DATAPRODUCTVERSIONSTATUS._serialized_start=10215
+  _DATAPRODUCTVERSIONSTATUS._serialized_end=10448
+  _DATASOURCE._serialized_start=10451
+  _DATASOURCE._serialized_end=10703
+  _DATASOURCELIST._serialized_start=10706
+  _DATASOURCELIST._serialized_end=10869
+  _DATASOURCESPEC._serialized_start=10872
+  _DATASOURCESPEC._serialized_end=11657
+  _DATASOURCESTATUS._serialized_start=11660
+  _DATASOURCESTATUS._serialized_end=11998
+  _DATASET._serialized_start=12001
+  _DATASET._serialized_end=12244
+  _DATASETGROUPBYSTATUS._serialized_start=12247
+  _DATASETGROUPBYSTATUS._serialized_end=12471
+  _DATASETLIST._serialized_start=12474
+  _DATASETLIST._serialized_end=12631
+  _DATASETSPEC._serialized_start=12634
+  _DATASETSPEC._serialized_end=14195
+  _DATASETSTATISTICS._serialized_start=14198
+  _DATASETSTATISTICS._serialized_end=14543
+  _DATASETSTATUS._serialized_start=14546
+  _DATASETSTATUS._serialized_end=15760
+  _DATASETTEMPLATE._serialized_start=15763
+  _DATASETTEMPLATE._serialized_end=15929
+  _DRIFTTHRESHOLD._serialized_start=15931
+  _DRIFTTHRESHOLD._serialized_end=15978
+  _ENTITY._serialized_start=15981
+  _ENTITY._serialized_end=16221
+  _ENTITYLIST._serialized_start=16224
+  _ENTITYLIST._serialized_end=16379
+  _ENTITYSPEC._serialized_start=16382
+  _ENTITYSPEC._serialized_end=16517
+  _ENTITYSTATUS._serialized_start=16520
+  _ENTITYSTATUS._serialized_end=16694
+  _EXCELNOTEBOOKSPEC._serialized_start=16697
+  _EXCELNOTEBOOKSPEC._serialized_end=16890
+  _EXCELSHEETAREA._serialized_start=16892
+  _EXCELSHEETAREA._serialized_end=16999
+  _FEATUREGROUP._serialized_start=17002
+  _FEATUREGROUP._serialized_end=17260
+  _FEATUREGROUPLIST._serialized_start=17263
+  _FEATUREGROUPLIST._serialized_end=17430
+  _FEATUREGROUPSPEC._serialized_start=17433
+  _FEATUREGROUPSPEC._serialized_end=18461
+  _FEATUREGROUPSTATUS._serialized_start=18464
+  _FEATUREGROUPSTATUS._serialized_end=19109
+  _FEATUREHISTOGRAM._serialized_start=19112
+  _FEATUREHISTOGRAM._serialized_end=19382
+  _FEATUREHISTOGRAMLIST._serialized_start=19385
+  _FEATUREHISTOGRAMLIST._serialized_end=19560
+  _FEATUREHISTOGRAMSPEC._serialized_start=19563
+  _FEATUREHISTOGRAMSPEC._serialized_end=20192
+  _FEATUREHISTOGRAMSTATUS._serialized_start=20195
+  _FEATUREHISTOGRAMSTATUS._serialized_end=20736
+  _FLATFILEFORMATSPEC._serialized_start=20739
+  _FLATFILEFORMATSPEC._serialized_end=21033
+  _GAUGESPEC._serialized_start=21035
+  _GAUGESPEC._serialized_end=21112
+  _GITLOCATION._serialized_start=21114
+  _GITLOCATION._serialized_end=21200
+  _GROUPBYSPEC._serialized_start=21202
+  _GROUPBYSPEC._serialized_end=21295
+  _GROUPDATASETLOCATIONSSPEC._serialized_start=21298
+  _GROUPDATASETLOCATIONSSPEC._serialized_end=21492
+  _HISTOGRAMSPEC._serialized_start=21494
+  _HISTOGRAMSPEC._serialized_end=21555
+  _IMAGELOCATION._serialized_start=21557
+  _IMAGELOCATION._serialized_end=21618
+  _KPI._serialized_start=21620
+  _KPI._serialized_end=21654
+  _LABELINGRULE._serialized_start=21656
+  _LABELINGRULE._serialized_end=21719
+  _LABELINGSPEC._serialized_start=21722
+  _LABELINGSPEC._serialized_end=21947
+  _LINECHARTSPEC._serialized_start=21949
+  _LINECHARTSPEC._serialized_end=22023
+  _MATERIALIZATIONSPEC._serialized_start=22026
+  _MATERIALIZATIONSPEC._serialized_end=22288
+  _METRICSPEC._serialized_start=22290
+  _METRICSPEC._serialized_end=22368
+  _OUTLIERSTAT._serialized_start=22370
+  _OUTLIERSTAT._serialized_end=22430
+  _PAGESPEC._serialized_start=22432
+  _PAGESPEC._serialized_end=22519
+  _PARQUETFILESPEC._serialized_start=22521
+  _PARQUETFILESPEC._serialized_end=22554
+  _RECIPE._serialized_start=22557
+  _RECIPE._serialized_end=22797
+  _RECIPEINPUTSPEC._serialized_start=22800
+  _RECIPEINPUTSPEC._serialized_end=22943
+  _RECIPELIST._serialized_start=22946
+  _RECIPELIST._serialized_end=23101
+  _RECIPEOUTPUTSPEC._serialized_start=23104
+  _RECIPEOUTPUTSPEC._serialized_end=23255
+  _RECIPEPARTSPEC._serialized_start=23257
+  _RECIPEPARTSPEC._serialized_end=23313
+  _RECIPERUN._serialized_start=23316
+  _RECIPERUN._serialized_end=23565
+  _RECIPERUNLIST._serialized_start=23568
+  _RECIPERUNLIST._serialized_end=23729
+  _RECIPERUNSPEC._serialized_start=23732
+  _RECIPERUNSPEC._serialized_end=24084
+  _RECIPERUNSTATUS._serialized_start=24087
+  _RECIPERUNSTATUS._serialized_end=24489
+  _RECIPESPEC._serialized_start=24492
+  _RECIPESPEC._serialized_end=25113
+  _RECIPESTATUS._serialized_start=25116
+  _RECIPESTATUS._serialized_end=25379
+  _RECIPESTEP._serialized_start=25381
+  _RECIPESTEP._serialized_end=25496
+  _RECIPESTEPPARAM._serialized_start=25498
+  _RECIPESTEPPARAM._serialized_end=25544
+  _RECOMMENDATIONSCHEMA._serialized_start=25546
+  _RECOMMENDATIONSCHEMA._serialized_end=25634
+  _RELATIONSHIPSPEC._serialized_start=25636
+  _RELATIONSHIPSPEC._serialized_end=25718
+  _ROWSPEC._serialized_start=25720
+  _ROWSPEC._serialized_end=25809
+  _SAMPLESPEC._serialized_start=25811
+  _SAMPLESPEC._serialized_end=25917
+  _SCATTERPLOTSPEC._serialized_start=25919
+  _SCATTERPLOTSPEC._serialized_end=25979
+  _SCHEMA._serialized_start=25982
+  _SCHEMA._serialized_end=26286
+  _SYNTHETICSPEC._serialized_start=26288
+  _SYNTHETICSPEC._serialized_end=26334
+  _TABLESPEC._serialized_start=26337
+  _TABLESPEC._serialized_end=26469
+  _TIMESERIESSCHEMA._serialized_start=26471
+  _TIMESERIESSCHEMA._serialized_end=26535
 # @@protoc_insertion_point(module_scope)
```

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_training_dot_v1alpha1_dot_generated__pb2
 from k8s.io.api.core.v1 import generated_pb2 as k8s_dot_io_dot_api_dot_core_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.apis.meta.v1 import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_apis_dot_meta_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime.schema import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_schema_dot_generated__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nIgithub.com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated.proto\x12\x39github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1aHgithub.com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated.proto\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\x82\x01\n\x0f\x41utoScalingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x13\n\x0bminReplicas\x18\x02 \x01(\x05\x12\x13\n\x0bmaxReplicas\x18\x03 \x01(\x05\x12\x19\n\x11\x63puAvgUtilization\x18\x04 \x01(\x05\x12\x19\n\x11memAvgUtilization\x18\x05 \x01(\x05\"\x8e\x01\n\x13\x42\x61\x63kwardCurtainSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x37\n\naccountRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x15\n\rconfidenceLow\x18\x04 \x01(\x01\x12\x16\n\x0e\x63onfidenceHigh\x18\x05 \x01(\x01\"\xca\x01\n\x13\x42\x61tchPredictionSpec\x12V\n\x08schedule\x18\x01 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12[\n\x08template\x18\x02 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionSpec\"|\n\rCustomAppSpec\x12\r\n\x05owner\x18\x01 \x01(\x08\x12\r\n\x05title\x18\x02 \x01(\t\x12M\n\x05pages\x18\x03 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.PageSpec\"\xfd\x01\n\x07\x44\x61taApp\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12T\n\x04spec\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.DataAppSpec\x12X\n\x06status\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.DataAppStatus\"\xa2\x01\n\x0b\x44\x61taAppList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Q\n\x05items\x18\x02 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.DataApp\"\x82\x04\n\x0b\x44\x61taAppSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x16\n\x0emodelClassName\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x11\n\tmodelName\x18\x05 \x01(\t\x12S\n\x06\x61\x63\x63\x65ss\x18\x06 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\x07 \x01(\x05\x12X\n\tresources\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x37\n\nproductRef\x18\x0c \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12;\n\x0eservingsiteRef\x18\r \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12X\n\x06\x63ustom\x18\x0e \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.CustomAppSpec\"\xd8\x02\n\rDataAppStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12=\n\x10\x64\x65ploymentStatus\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x39\n\x0eservicetStatus\x18\x04 \x01(\x0b\x32!.k8s.io.api.core.v1.ServiceStatus\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\x12\x43\n\nconditions\x18\x07 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xf0\x03\n\x12\x44riftDetectionSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x15\n\rgenDriftTests\x18\x02 \x01(\x08\x12\x16\n\x0eminPredictions\x18\x03 \x01(\x05\x12\x0f\n\x07\x63olumns\x18\x04 \x03(\t\x12]\n\x0f\x64riftThresholds\x18\x05 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DriftThreshold\x12]\n\x11unitTestsTemplate\x18\x06 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12V\n\x08schedule\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\x45\n\x18outlierDetectionModelRef\x18\x08 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x15\n\rmaxHistograms\x18\t \x01(\x05\x12\x15\n\rperiodSeconds\x18\n \x01(\x05\"\x16\n\x14\x44riftDetectionStatus\"\xc5\x01\n\x11\x46\x61stSlowModelSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x39\n\x0c\x66\x61stModelRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x39\n\x0cslowModelRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0bprobaLowPct\x18\x04 \x01(\x05\x12\x14\n\x0cprobaHighPct\x18\x05 \x01(\x05\"\xce\x01\n\x10\x46\x65\x65\x64\x62\x61\x63kTestSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12Q\n\x05tests\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12V\n\x08schedule\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\"\xa8\x02\n\x16\x46orecastPredictionSpec\x12\x7f\n\x0fhierarchyValues\x18\x01 \x03(\x0b\x32\x66.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastPredictionSpec.HierarchyValuesEntry\x12U\n\x07horizon\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\x1a\x36\n\x14HierarchyValuesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x83\x01\n\x0b\x46orecastRun\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x10\n\x08modelURI\x18\x02 \x01(\t\x12U\n\x07horizon\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\"\xe4\x01\n\x0c\x46orecastSpec\x12_\n\x04runs\x18\t \x03(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastSpec.RunsEntry\x1as\n\tRunsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12U\n\x05value\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastRun:\x02\x38\x01\"\xd1\x01\n\x0e\x46orecastStatus\x12\x12\n\nprofileURI\x18\x01 \x01(\t\x12\x11\n\treportURI\x18\x02 \x01(\t\x12\x13\n\x0b\x66orecastURI\x18\x03 \x01(\t\x12\x0e\n\x06\x66\x61iled\x18\x04 \x01(\x08\x12\x12\n\nfailureMsg\x18\x05 \x01(\t\x12_\n\rworkerResults\x18\x06 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"o\n\x12\x46orwardCurtainSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x37\n\naccountRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0f\n\x07percent\x18\x03 \x01(\x05\"Z\n\x16KubernetesObjectStatus\x12\x30\n\x03ref\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0e\n\x06status\x18\x02 \x01(\t\"0\n\rMetricHistory\x12\x0e\n\x06metric\x18\x01 \x01(\t\x12\x0f\n\x07history\x18\x02 \x03(\x01\"\xab\n\n\x15ModelDeploymentStatus\x12\x11\n\tmodelName\x18\x01 \x01(\t\x12\x14\n\x0cmodelVersion\x18\x02 \x01(\t\x12\x11\n\timageName\x18\x03 \x01(\t\x12:\n\rdeploymentRef\x18\x04 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x37\n\nserviceRef\x18\x05 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x33\n\x06hpaRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0b\n\x03p50\x18\x07 \x01(\x01\x12\x0b\n\x03p95\x18\x08 \x01(\x01\x12\x0b\n\x03p99\x18\t \x01(\x01\x12\x46\n\x12lastPredictionTime\x18\n \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12\x64\x61ilyPredictionAvg\x18\x0b \x01(\x05\x12\x13\n\x0blastFailure\x18\x0c \x01(\t\x12\r\n\x05phase\x18\r \x01(\t\x12>\n\ndeployedAt\x18\x0e \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12>\n\nreleasedAt\x18\x0f \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x11\n\tdataDrift\x18\x10 \x01(\x08\x12\x14\n\x0c\x63onceptDrift\x18\x11 \x01(\x08\x12\x1c\n\x14lastDailyPredictions\x18\x12 \x03(\x05\x12i\n\x0eobjectStatuses\x18\x13 \x03(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.KubernetesObjectStatus\x12Z\n\x06\x65rrors\x18\x14 \x03(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ValidationError\x12\x43\n\x16lastFeedbackDatasetRef\x18\x15 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x44\n\x10lastFeedbackTest\x18\x16 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x65\n\x17lastFeedbackTestResults\x18\x17 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12|\n\x0emetricsHistory\x18\x18 \x03(\x0b\x32\x64.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ModelDeploymentStatus.MetricsHistoryEntry\x1a\x7f\n\x13MetricsHistoryEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12W\n\x05value\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.MetricHistory:\x02\x38\x01\"\xe1\x01\n\x0bModelRecord\x12\x11\n\tmodelName\x18\x01 \x01(\t\x12\x14\n\x0cmodelVersion\x18\x02 \x01(\t\x12:\n\x06liveAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12=\n\tretiredAt\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12\x61vgDailyPrediction\x18\x05 \x01(\x05\x12\x12\n\navgLatency\x18\x06 \x01(\x01\"\x80\x01\n\x10ModelServingSpec\x12\x12\n\nserverless\x18\x02 \x01(\x08\x12X\n\x0cservingTests\x18\x04 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\";\n\x16OnlineFeatureStoreSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08hostname\x18\x02 \x01(\t\"U\n\x11OnlineStoreStatus\x12@\n\x0clastAccessed\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"=\n PartitionPredictionLocationsSpec\x12\x19\n\x11groupForecastFile\x18\x02 \x01(\t\"\x86\x02\n\nPrediction\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12W\n\x04spec\x18\x02 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionSpec\x12[\n\x06status\x18\x03 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionStatus\"\x83\x01\n\x13PredictionCacheSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08inMemory\x18\x02 \x01(\x08\x12\r\n\x05redis\x18\x03 \x01(\x08\x12:\n\rconnectionRef\x18\x04 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"Y\n\x15PredictionCacheStatus\x12@\n\x0clastAccessed\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"\xa8\x01\n\x0ePredictionList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12T\n\x05items\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\"\x83\x02\n\x15PredictionLoggingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x15\n\rsamplePercent\x18\x02 \x01(\x05\x12\x0c\n\x04rows\x18\x03 \x01(\x05\x12\x19\n\x11\x62\x61\x63kupFreqSeconds\x18\x04 \x01(\x05\x12@\n\x13\x62\x61\x63kupConnectionRef\x18\x05 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12W\n\x08location\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\xdc\x07\n\x0ePredictionSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x16\n\x0emodelClassName\x18\x02 \x01(\t\x12\x39\n\x0cpredictorRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0f\n\x07labeled\x18\x04 \x01(\x08\x12\x10\n\x08\x66orecast\x18\x05 \x01(\x08\x12:\n\rdataSourceRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12R\n\x05input\x18\x07 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataInputSpec\x12T\n\x06output\x18\x08 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataOutputSpec\x12\x15\n\rcreateDataset\x18\t \x01(\x08\x12[\n\tunitTests\x18\n \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelTestSuite\x12\r\n\x05owner\x18\x0b \x01(\t\x12X\n\tresources\x18\x0c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18\r \x01(\x03\x12\x10\n\x08priority\x18\x0e \x01(\t\x12\x0f\n\x07\x61\x62orted\x18\x0f \x01(\x08\x12\x0b\n\x03ttl\x18\x10 \x01(\x05\x12g\n\x0c\x66orecastSpec\x18\x11 \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastPredictionSpec\x12;\n\x0eservingsiteRef\x18\x13 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12v\n\x11partitionLocation\x18\x14 \x01(\x0b\x32[.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PartitionPredictionLocationsSpec\x12\x0f\n\x07workers\x18\x15 \x01(\x05\"\xe0\x06\n\x10PredictionStatus\x12?\n\x0b\x63ompletedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x02 \x01(\t\x12\x61\n\x0funitTestsResult\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x0c\n\x04rows\x18\x05 \x01(\x05\x12\x13\n\x0btriggeredBy\x18\x06 \x01(\t\x12K\n\x04logs\x18\x07 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12=\n\tupdatedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\t \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\n \x01(\t\x12\x37\n\ndatasetRef\x18\x0b \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12V\n\x07\x63olumns\x18\x0c \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ColumnHistogram\x12\x0f\n\x07\x64rifted\x18\r \x01(\x08\x12[\n\x08\x66orecast\x18\x0e \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastStatus\x12[\n\x05usage\x18\x0f \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x43\n\nconditions\x18\x10 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x83\x02\n\tPredictor\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictorSpec\x12Z\n\x06status\x18\x03 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictorStatus\"\xa6\x01\n\rPredictorList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Predictor\"\xf6\x0e\n\rPredictorSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x16\n\x0emodelClassName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x37\n\nproductRef\x18\x04 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08template\x18\x05 \x01(\x08\x12\x0e\n\x06online\x18\x06 \x01(\x08\x12;\n\x0eservingsiteRef\x18\x07 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\\\n\x06models\x18\x08 \x03(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ModelDeploymentSpec\x12_\n\x0bprogressive\x18\t \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ProgressiveSpec\x12^\n\x0f\x61rtifactsFolder\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12S\n\x06\x61\x63\x63\x65ss\x18\x0b \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\x0c \x01(\x05\x12_\n\x0b\x61utoScaling\x18\r \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.AutoScalingSpec\x12\r\n\x05owner\x18\x0e \x01(\t\x12X\n\tresources\x18\x0f \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12]\n\x05\x63\x61\x63he\x18\x10 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionCacheSpec\x12`\n\x05store\x18\x11 \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.OnlineFeatureStoreSpec\x12\\\n\x07serving\x18\x12 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ModelServingSpec\x12\x0c\n\x04task\x18\x13 \x01(\t\x12\x1b\n\x13predictionThreshold\x18\x14 \x01(\x01\x12\\\n\x05\x64rift\x18\x15 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.DriftDetectionSpec\x12]\n\x08\x66\x65\x65\x64\x62\x61\x63k\x18\x16 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.FeedbackTestSpec\x12\x38\n\x0bnotifierRef\x18\x17 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12k\n\x11predictionLogging\x18\x18 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionLoggingSpec\x12\x65\n\x0e\x66orwardCurtain\x18\x19 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForwardCurtainSpec\x12g\n\x0f\x62\x61\x63kwardCurtain\x18\x1a \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.BackwardCurtainSpec\x12^\n\x08\x66\x61stSlow\x18\x1b \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.FastSlowModelSpec\x12]\n\x05\x62\x61tch\x18\x1c \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.BatchPredictionSpec\"\xc5\x08\n\x0fPredictorStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12W\n\x07history\x18\x02 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ModelRecord\x12\x66\n\x0cmodelsStatus\x18\x04 \x03(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ModelDeploymentStatus\x12i\n\x12predictorletStatus\x18\x05 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictorletStatus\x12\x65\n\x0b\x63\x61\x63heStatus\x18\x06 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionCacheStatus\x12g\n\x11onlineStoreStatus\x18\x07 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.OnlineStoreStatus\x12=\n\tupdatedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x10\n\x08\x65ndPoint\x18\t \x01(\t\x12\x15\n\rfailureReason\x18\n \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x0b \x01(\t\x12\x42\n\x12loadBalancerStatus\x18\x0c \x01(\x0b\x32&.k8s.io.api.core.v1.LoadBalancerStatus\x12\x42\n\x15lastPredictionDataset\x18\r \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x65\n\x13servingTestsResults\x18\x0e \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\x66\n\x12predictionSchedule\x18\x0f \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12\x43\n\nconditions\x18\x11 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xdf\x03\n\x12PredictorletStatus\x12\x11\n\timageName\x18\x01 \x01(\t\x12:\n\rdeploymentRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x37\n\nserviceRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0b\n\x03p50\x18\x04 \x01(\x01\x12\x0b\n\x03p95\x18\x05 \x01(\x01\x12\x0b\n\x03p99\x18\x06 \x01(\x01\x12\x1a\n\x12\x64\x61ilyPredictionAvg\x18\x07 \x01(\x05\x12\x18\n\x10totalPredictions\x18\x08 \x01(\x05\x12\x1c\n\x14lastDailyPredictions\x18\t \x03(\x05\x12\x46\n\x12lastPredictionTime\x18\n \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x13\n\x0blastFailure\x18\x0b \x01(\t\x12i\n\x0eobjectStatuses\x18\x0c \x03(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.KubernetesObjectStatus\"R\n\x0fProgressiveSpec\x12\x0e\n\x06warmup\x18\x01 \x01(\x05\x12\x18\n\x10trafficIncrement\x18\x02 \x01(\x05\x12\x15\n\rcanaryMetrics\x18\x03 \x03(\t\"[\n\x0fValidationError\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\x0e\n\x06metric\x18\x02 \x01(\t\x12\x0b\n\x03min\x18\x03 \x01(\x01\x12\x0b\n\x03max\x18\x04 \x01(\x01\x12\x0e\n\x06\x61\x63tual\x18\x05 \x01(\x01\x42;Z9github.com/metaprov/modelaapi/pkg/apis/inference/v1alpha1')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nIgithub.com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated.proto\x12\x39github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1aHgithub.com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated.proto\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\x82\x01\n\x0f\x41utoScalingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x13\n\x0bminReplicas\x18\x02 \x01(\x05\x12\x13\n\x0bmaxReplicas\x18\x03 \x01(\x05\x12\x19\n\x11\x63puAvgUtilization\x18\x04 \x01(\x05\x12\x19\n\x11memAvgUtilization\x18\x05 \x01(\x05\"\x8e\x01\n\x13\x42\x61\x63kwardCurtainSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x37\n\naccountRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x15\n\rconfidenceLow\x18\x04 \x01(\x01\x12\x16\n\x0e\x63onfidenceHigh\x18\x05 \x01(\x01\"|\n\rCustomAppSpec\x12\r\n\x05owner\x18\x01 \x01(\x08\x12\r\n\x05title\x18\x02 \x01(\t\x12M\n\x05pages\x18\x03 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.PageSpec\"\xfd\x01\n\x07\x44\x61taApp\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12T\n\x04spec\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.DataAppSpec\x12X\n\x06status\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.DataAppStatus\"\xa2\x01\n\x0b\x44\x61taAppList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Q\n\x05items\x18\x02 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.DataApp\"\xc9\x03\n\x0b\x44\x61taAppSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x16\n\x0emodelClassName\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x11\n\tmodelName\x18\x05 \x01(\t\x12S\n\x06\x61\x63\x63\x65ss\x18\x06 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\x07 \x01(\x05\x12X\n\tresources\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12;\n\x0eservingsiteRef\x18\r \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12X\n\x06\x63ustom\x18\x0e \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.CustomAppSpec\"\xd8\x02\n\rDataAppStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12=\n\x10\x64\x65ploymentStatus\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x39\n\x0eservicetStatus\x18\x04 \x01(\x0b\x32!.k8s.io.api.core.v1.ServiceStatus\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\x12\x43\n\nconditions\x18\x07 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xf0\x03\n\x12\x44riftDetectionSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x15\n\rgenDriftTests\x18\x02 \x01(\x08\x12\x16\n\x0eminPredictions\x18\x03 \x01(\x05\x12\x0f\n\x07\x63olumns\x18\x04 \x03(\t\x12]\n\x0f\x64riftThresholds\x18\x05 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DriftThreshold\x12]\n\x11unitTestsTemplate\x18\x06 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12V\n\x08schedule\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\x45\n\x18outlierDetectionModelRef\x18\x08 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x15\n\rmaxHistograms\x18\t \x01(\x05\x12\x15\n\rperiodSeconds\x18\n \x01(\x05\"\xc5\x01\n\x11\x46\x61stSlowModelSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x39\n\x0c\x66\x61stModelRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x39\n\x0cslowModelRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0bprobaLowPct\x18\x04 \x01(\x05\x12\x14\n\x0cprobaHighPct\x18\x05 \x01(\x05\"\xce\x01\n\x10\x46\x65\x65\x64\x62\x61\x63kTestSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12Q\n\x05tests\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12V\n\x08schedule\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\"\xa8\x02\n\x16\x46orecastPredictionSpec\x12\x7f\n\x0fhierarchyValues\x18\x01 \x03(\x0b\x32\x66.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastPredictionSpec.HierarchyValuesEntry\x12U\n\x07horizon\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\x1a\x36\n\x14HierarchyValuesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x88\x01\n\x0b\x46orecastRun\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x15\n\rmodelLocation\x18\x02 \x01(\t\x12U\n\x07horizon\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\"\xe4\x01\n\x0c\x46orecastSpec\x12_\n\x04runs\x18\t \x03(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastSpec.RunsEntry\x1as\n\tRunsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12U\n\x05value\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastRun:\x02\x38\x01\"\xd1\x01\n\x0e\x46orecastStatus\x12\x12\n\nprofileURI\x18\x01 \x01(\t\x12\x11\n\treportURI\x18\x02 \x01(\t\x12\x13\n\x0b\x66orecastURI\x18\x03 \x01(\t\x12\x0e\n\x06\x66\x61iled\x18\x04 \x01(\x08\x12\x12\n\nfailureMsg\x18\x05 \x01(\t\x12_\n\rworkerResults\x18\x06 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"o\n\x12\x46orwardCurtainSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x37\n\naccountRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0f\n\x07percent\x18\x03 \x01(\x05\"0\n\rMetricHistory\x12\x0e\n\x06metric\x18\x01 \x01(\t\x12\x0f\n\x07history\x18\x02 \x03(\x01\"\xad\x02\n\x15ModelDeploymentRecord\x12\x11\n\tmodelName\x18\x01 \x01(\t\x12\x14\n\x0cmodelVersion\x18\x02 \x01(\t\x12\x11\n\tmodelRole\x18\x03 \x01(\t\x12\x11\n\timageName\x18\x04 \x01(\t\x12>\n\ndeployedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12=\n\tretiredAt\x18\x06 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x16\n\x0e\x66\x61ilureMessage\x18\x07 \x01(\t\x12\x1a\n\x12\x61vgDailyPrediction\x18\x08 \x01(\x05\x12\x12\n\navgLatency\x18\t \x01(\x01\"\x9d\x07\n\x15ModelDeploymentStatus\x12\x11\n\tmodelName\x18\x01 \x01(\t\x12\x14\n\x0cmodelVersion\x18\x02 \x01(\t\x12\x11\n\tmodelRole\x18\x03 \x01(\t\x12\x11\n\timageName\x18\x04 \x01(\t\x12:\n\rdeploymentRef\x18\x05 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x37\n\nserviceRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x33\n\x06hpaRef\x18\x07 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x16\n\x0e\x66\x61ilureMessage\x18\x08 \x01(\t\x12>\n\ndeployedAt\x18\t \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\x16lastFeedbackDatasetRef\x18\n \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x46\n\x12lastFeedbackTestAt\x18\x0b \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x65\n\x17lastFeedbackTestResults\x18\x0c \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12|\n\x0emetricsHistory\x18\r \x03(\x0b\x32\x64.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ModelDeploymentStatus.MetricsHistoryEntry\x12\x1a\n\x12\x61vgDailyPrediction\x18\x0e \x01(\x05\x12\x12\n\navgLatency\x18\x0f \x01(\x01\x12\x10\n\x08\x65ndpoint\x18\x10 \x01(\t\x1a\x7f\n\x13MetricsHistoryEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12W\n\x05value\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.MetricHistory:\x02\x38\x01\"\x80\x01\n\x10ModelServingSpec\x12\x12\n\nserverless\x18\x02 \x01(\x08\x12X\n\x0cservingTests\x18\x04 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\";\n\x16OnlineFeatureStoreSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08hostname\x18\x02 \x01(\t\"U\n\x11OnlineStoreStatus\x12@\n\x0clastAccessed\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"=\n PartitionPredictionLocationsSpec\x12\x19\n\x11groupForecastFile\x18\x02 \x01(\t\"\x86\x02\n\nPrediction\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12W\n\x04spec\x18\x02 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionSpec\x12[\n\x06status\x18\x03 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionStatus\"\x83\x01\n\x13PredictionCacheSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08inMemory\x18\x02 \x01(\x08\x12\r\n\x05redis\x18\x03 \x01(\x08\x12:\n\rconnectionRef\x18\x04 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\xa8\x01\n\x0ePredictionList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12T\n\x05items\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\"\x83\x02\n\x15PredictionLoggingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x15\n\rsamplePercent\x18\x02 \x01(\x05\x12\x0c\n\x04rows\x18\x03 \x01(\x05\x12\x19\n\x11\x62\x61\x63kupFreqSeconds\x18\x04 \x01(\x05\x12@\n\x13\x62\x61\x63kupConnectionRef\x18\x05 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12W\n\x08location\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\xdc\x07\n\x0ePredictionSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x16\n\x0emodelClassName\x18\x02 \x01(\t\x12\x39\n\x0cpredictorRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0f\n\x07labeled\x18\x04 \x01(\x08\x12\x10\n\x08\x66orecast\x18\x05 \x01(\x08\x12:\n\rdataSourceRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12R\n\x05input\x18\x07 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataInputSpec\x12T\n\x06output\x18\x08 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataOutputSpec\x12\x15\n\rcreateDataset\x18\t \x01(\x08\x12[\n\tunitTests\x18\n \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelTestSuite\x12\r\n\x05owner\x18\x0b \x01(\t\x12X\n\tresources\x18\x0c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18\r \x01(\x03\x12\x10\n\x08priority\x18\x0e \x01(\t\x12\x0f\n\x07\x61\x62orted\x18\x0f \x01(\x08\x12\x0b\n\x03ttl\x18\x10 \x01(\x05\x12g\n\x0c\x66orecastSpec\x18\x11 \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastPredictionSpec\x12;\n\x0eservingsiteRef\x18\x13 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12v\n\x11partitionLocation\x18\x14 \x01(\x0b\x32[.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PartitionPredictionLocationsSpec\x12\x0f\n\x07workers\x18\x15 \x01(\x05\"\xe0\x06\n\x10PredictionStatus\x12?\n\x0b\x63ompletedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x02 \x01(\t\x12\x61\n\x0funitTestsResult\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x0c\n\x04rows\x18\x05 \x01(\x05\x12\x13\n\x0btriggeredBy\x18\x06 \x01(\t\x12K\n\x04logs\x18\x07 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12=\n\tupdatedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\t \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\n \x01(\t\x12\x37\n\ndatasetRef\x18\x0b \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12V\n\x07\x63olumns\x18\x0c \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ColumnHistogram\x12\x0f\n\x07\x64rifted\x18\r \x01(\x08\x12[\n\x08\x66orecast\x18\x0e \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastStatus\x12[\n\x05usage\x18\x0f \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x43\n\nconditions\x18\x10 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x83\x02\n\tPredictor\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictorSpec\x12Z\n\x06status\x18\x03 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictorStatus\"\xa6\x01\n\rPredictorList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Predictor\"\xb1\r\n\rPredictorSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x16\n\x0emodelClassName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x37\n\nproductRef\x18\x04 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08template\x18\x05 \x01(\x08\x12;\n\x0eservingSiteRef\x18\x07 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\\\n\x06models\x18\x08 \x03(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ModelDeploymentSpec\x12_\n\x0bprogressive\x18\t \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ProgressiveSpec\x12S\n\x06\x61\x63\x63\x65ss\x18\x0b \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\x0c \x01(\x05\x12_\n\x0b\x61utoScaling\x18\r \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.AutoScalingSpec\x12\r\n\x05owner\x18\x0e \x01(\t\x12X\n\tresources\x18\x0f \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12]\n\x05\x63\x61\x63he\x18\x10 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionCacheSpec\x12`\n\x05store\x18\x11 \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.OnlineFeatureStoreSpec\x12\\\n\x07serving\x18\x12 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ModelServingSpec\x12\x0c\n\x04task\x18\x13 \x01(\t\x12\\\n\x05\x64rift\x18\x15 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.DriftDetectionSpec\x12]\n\x08\x66\x65\x65\x64\x62\x61\x63k\x18\x16 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.FeedbackTestSpec\x12_\n\x0cnotification\x18\x17 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12k\n\x11predictionLogging\x18\x18 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionLoggingSpec\x12\x65\n\x0e\x66orwardCurtain\x18\x19 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForwardCurtainSpec\x12g\n\x0f\x62\x61\x63kwardCurtain\x18\x1a \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.BackwardCurtainSpec\x12^\n\x08\x66\x61stSlow\x18\x1b \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.FastSlowModelSpec\"\xd6\x06\n\x0fPredictorStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12\x61\n\x07history\x18\x02 \x03(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ModelDeploymentRecord\x12\x65\n\x0bmodelStatus\x18\x04 \x03(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ModelDeploymentStatus\x12i\n\x12predictorletStatus\x18\x05 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictorletStatus\x12g\n\x11onlineStoreStatus\x18\x07 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.OnlineStoreStatus\x12=\n\tupdatedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x16\n\x0e\x66\x61ilureMessage\x18\x0b \x01(\t\x12\x42\n\x12loadBalancerStatus\x18\x0c \x01(\x0b\x32&.k8s.io.api.core.v1.LoadBalancerStatus\x12\x42\n\x15lastPredictionDataset\x18\r \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x65\n\x13servingTestsResults\x18\x0e \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\x43\n\nconditions\x18\x11 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x86\x03\n\x12PredictorletStatus\x12:\n\rdeploymentRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x37\n\nserviceRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12>\n\ndeployedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0b\n\x03p50\x18\x04 \x01(\x01\x12\x0b\n\x03p95\x18\x05 \x01(\x01\x12\x0b\n\x03p99\x18\x06 \x01(\x01\x12\x1a\n\x12\x61vgDailyPrediction\x18\x07 \x01(\x05\x12\x18\n\x10totalPredictions\x18\x08 \x01(\x05\x12\x46\n\x12lastPredictionTime\x18\t \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x16\n\x0e\x66\x61ilureMessage\x18\n \x01(\t\"R\n\x0fProgressiveSpec\x12\x0e\n\x06warmup\x18\x01 \x01(\x05\x12\x18\n\x10trafficIncrement\x18\x02 \x01(\x05\x12\x15\n\rcanaryMetrics\x18\x03 \x03(\t\"[\n\x0fValidationError\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\x0e\n\x06metric\x18\x02 \x01(\t\x12\x0b\n\x03min\x18\x03 \x01(\x01\x12\x0b\n\x03max\x18\x04 \x01(\x01\x12\x0e\n\x06\x61\x63tual\x18\x05 \x01(\x01\x42;Z9github.com/metaprov/modelaapi/pkg/apis/inference/v1alpha1')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.generated_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z9github.com/metaprov/modelaapi/pkg/apis/inference/v1alpha1'
@@ -34,88 +34,80 @@
   _FORECASTSPEC_RUNSENTRY._serialized_options = b'8\001'
   _MODELDEPLOYMENTSTATUS_METRICSHISTORYENTRY._options = None
   _MODELDEPLOYMENTSTATUS_METRICSHISTORYENTRY._serialized_options = b'8\001'
   _AUTOSCALINGSPEC._serialized_start=549
   _AUTOSCALINGSPEC._serialized_end=679
   _BACKWARDCURTAINSPEC._serialized_start=682
   _BACKWARDCURTAINSPEC._serialized_end=824
-  _BATCHPREDICTIONSPEC._serialized_start=827
-  _BATCHPREDICTIONSPEC._serialized_end=1029
-  _CUSTOMAPPSPEC._serialized_start=1031
-  _CUSTOMAPPSPEC._serialized_end=1155
-  _DATAAPP._serialized_start=1158
-  _DATAAPP._serialized_end=1411
-  _DATAAPPLIST._serialized_start=1414
-  _DATAAPPLIST._serialized_end=1576
-  _DATAAPPSPEC._serialized_start=1579
-  _DATAAPPSPEC._serialized_end=2093
-  _DATAAPPSTATUS._serialized_start=2096
-  _DATAAPPSTATUS._serialized_end=2440
-  _DRIFTDETECTIONSPEC._serialized_start=2443
-  _DRIFTDETECTIONSPEC._serialized_end=2939
-  _DRIFTDETECTIONSTATUS._serialized_start=2941
-  _DRIFTDETECTIONSTATUS._serialized_end=2963
-  _FASTSLOWMODELSPEC._serialized_start=2966
-  _FASTSLOWMODELSPEC._serialized_end=3163
-  _FEEDBACKTESTSPEC._serialized_start=3166
-  _FEEDBACKTESTSPEC._serialized_end=3372
-  _FORECASTPREDICTIONSPEC._serialized_start=3375
-  _FORECASTPREDICTIONSPEC._serialized_end=3671
-  _FORECASTPREDICTIONSPEC_HIERARCHYVALUESENTRY._serialized_start=3617
-  _FORECASTPREDICTIONSPEC_HIERARCHYVALUESENTRY._serialized_end=3671
-  _FORECASTRUN._serialized_start=3674
-  _FORECASTRUN._serialized_end=3805
-  _FORECASTSPEC._serialized_start=3808
-  _FORECASTSPEC._serialized_end=4036
-  _FORECASTSPEC_RUNSENTRY._serialized_start=3921
-  _FORECASTSPEC_RUNSENTRY._serialized_end=4036
-  _FORECASTSTATUS._serialized_start=4039
-  _FORECASTSTATUS._serialized_end=4248
-  _FORWARDCURTAINSPEC._serialized_start=4250
-  _FORWARDCURTAINSPEC._serialized_end=4361
-  _KUBERNETESOBJECTSTATUS._serialized_start=4363
-  _KUBERNETESOBJECTSTATUS._serialized_end=4453
-  _METRICHISTORY._serialized_start=4455
-  _METRICHISTORY._serialized_end=4503
-  _MODELDEPLOYMENTSTATUS._serialized_start=4506
-  _MODELDEPLOYMENTSTATUS._serialized_end=5829
-  _MODELDEPLOYMENTSTATUS_METRICSHISTORYENTRY._serialized_start=5702
-  _MODELDEPLOYMENTSTATUS_METRICSHISTORYENTRY._serialized_end=5829
-  _MODELRECORD._serialized_start=5832
-  _MODELRECORD._serialized_end=6057
-  _MODELSERVINGSPEC._serialized_start=6060
-  _MODELSERVINGSPEC._serialized_end=6188
-  _ONLINEFEATURESTORESPEC._serialized_start=6190
-  _ONLINEFEATURESTORESPEC._serialized_end=6249
-  _ONLINESTORESTATUS._serialized_start=6251
-  _ONLINESTORESTATUS._serialized_end=6336
-  _PARTITIONPREDICTIONLOCATIONSSPEC._serialized_start=6338
-  _PARTITIONPREDICTIONLOCATIONSSPEC._serialized_end=6399
-  _PREDICTION._serialized_start=6402
-  _PREDICTION._serialized_end=6664
-  _PREDICTIONCACHESPEC._serialized_start=6667
-  _PREDICTIONCACHESPEC._serialized_end=6798
-  _PREDICTIONCACHESTATUS._serialized_start=6800
-  _PREDICTIONCACHESTATUS._serialized_end=6889
-  _PREDICTIONLIST._serialized_start=6892
-  _PREDICTIONLIST._serialized_end=7060
-  _PREDICTIONLOGGINGSPEC._serialized_start=7063
-  _PREDICTIONLOGGINGSPEC._serialized_end=7322
-  _PREDICTIONSPEC._serialized_start=7325
-  _PREDICTIONSPEC._serialized_end=8313
-  _PREDICTIONSTATUS._serialized_start=8316
-  _PREDICTIONSTATUS._serialized_end=9180
-  _PREDICTOR._serialized_start=9183
-  _PREDICTOR._serialized_end=9442
-  _PREDICTORLIST._serialized_start=9445
-  _PREDICTORLIST._serialized_end=9611
-  _PREDICTORSPEC._serialized_start=9614
-  _PREDICTORSPEC._serialized_end=11524
-  _PREDICTORSTATUS._serialized_start=11527
-  _PREDICTORSTATUS._serialized_end=12620
-  _PREDICTORLETSTATUS._serialized_start=12623
-  _PREDICTORLETSTATUS._serialized_end=13102
-  _PROGRESSIVESPEC._serialized_start=13104
-  _PROGRESSIVESPEC._serialized_end=13186
-  _VALIDATIONERROR._serialized_start=13188
-  _VALIDATIONERROR._serialized_end=13279
+  _CUSTOMAPPSPEC._serialized_start=826
+  _CUSTOMAPPSPEC._serialized_end=950
+  _DATAAPP._serialized_start=953
+  _DATAAPP._serialized_end=1206
+  _DATAAPPLIST._serialized_start=1209
+  _DATAAPPLIST._serialized_end=1371
+  _DATAAPPSPEC._serialized_start=1374
+  _DATAAPPSPEC._serialized_end=1831
+  _DATAAPPSTATUS._serialized_start=1834
+  _DATAAPPSTATUS._serialized_end=2178
+  _DRIFTDETECTIONSPEC._serialized_start=2181
+  _DRIFTDETECTIONSPEC._serialized_end=2677
+  _FASTSLOWMODELSPEC._serialized_start=2680
+  _FASTSLOWMODELSPEC._serialized_end=2877
+  _FEEDBACKTESTSPEC._serialized_start=2880
+  _FEEDBACKTESTSPEC._serialized_end=3086
+  _FORECASTPREDICTIONSPEC._serialized_start=3089
+  _FORECASTPREDICTIONSPEC._serialized_end=3385
+  _FORECASTPREDICTIONSPEC_HIERARCHYVALUESENTRY._serialized_start=3331
+  _FORECASTPREDICTIONSPEC_HIERARCHYVALUESENTRY._serialized_end=3385
+  _FORECASTRUN._serialized_start=3388
+  _FORECASTRUN._serialized_end=3524
+  _FORECASTSPEC._serialized_start=3527
+  _FORECASTSPEC._serialized_end=3755
+  _FORECASTSPEC_RUNSENTRY._serialized_start=3640
+  _FORECASTSPEC_RUNSENTRY._serialized_end=3755
+  _FORECASTSTATUS._serialized_start=3758
+  _FORECASTSTATUS._serialized_end=3967
+  _FORWARDCURTAINSPEC._serialized_start=3969
+  _FORWARDCURTAINSPEC._serialized_end=4080
+  _METRICHISTORY._serialized_start=4082
+  _METRICHISTORY._serialized_end=4130
+  _MODELDEPLOYMENTRECORD._serialized_start=4133
+  _MODELDEPLOYMENTRECORD._serialized_end=4434
+  _MODELDEPLOYMENTSTATUS._serialized_start=4437
+  _MODELDEPLOYMENTSTATUS._serialized_end=5362
+  _MODELDEPLOYMENTSTATUS_METRICSHISTORYENTRY._serialized_start=5235
+  _MODELDEPLOYMENTSTATUS_METRICSHISTORYENTRY._serialized_end=5362
+  _MODELSERVINGSPEC._serialized_start=5365
+  _MODELSERVINGSPEC._serialized_end=5493
+  _ONLINEFEATURESTORESPEC._serialized_start=5495
+  _ONLINEFEATURESTORESPEC._serialized_end=5554
+  _ONLINESTORESTATUS._serialized_start=5556
+  _ONLINESTORESTATUS._serialized_end=5641
+  _PARTITIONPREDICTIONLOCATIONSSPEC._serialized_start=5643
+  _PARTITIONPREDICTIONLOCATIONSSPEC._serialized_end=5704
+  _PREDICTION._serialized_start=5707
+  _PREDICTION._serialized_end=5969
+  _PREDICTIONCACHESPEC._serialized_start=5972
+  _PREDICTIONCACHESPEC._serialized_end=6103
+  _PREDICTIONLIST._serialized_start=6106
+  _PREDICTIONLIST._serialized_end=6274
+  _PREDICTIONLOGGINGSPEC._serialized_start=6277
+  _PREDICTIONLOGGINGSPEC._serialized_end=6536
+  _PREDICTIONSPEC._serialized_start=6539
+  _PREDICTIONSPEC._serialized_end=7527
+  _PREDICTIONSTATUS._serialized_start=7530
+  _PREDICTIONSTATUS._serialized_end=8394
+  _PREDICTOR._serialized_start=8397
+  _PREDICTOR._serialized_end=8656
+  _PREDICTORLIST._serialized_start=8659
+  _PREDICTORLIST._serialized_end=8825
+  _PREDICTORSPEC._serialized_start=8828
+  _PREDICTORSPEC._serialized_end=10541
+  _PREDICTORSTATUS._serialized_start=10544
+  _PREDICTORSTATUS._serialized_end=11398
+  _PREDICTORLETSTATUS._serialized_start=11401
+  _PREDICTORLETSTATUS._serialized_end=11791
+  _PROGRESSIVESPEC._serialized_start=11793
+  _PROGRESSIVESPEC._serialized_end=11875
+  _VALIDATIONERROR._serialized_start=11877
+  _VALIDATIONERROR._serialized_end=11968
 # @@protoc_insertion_point(module_scope)
```

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from k8s.io.api.core.v1 import generated_pb2 as k8s_dot_io_dot_api_dot_core_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.api.resource import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_api_dot_resource_dot_generated__pb2
 from k8s.io.apimachinery.pkg.apis.meta.v1 import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_apis_dot_meta_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime.schema import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_schema_dot_generated__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nEgithub.com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated.proto\x12\x35github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/api/resource/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\xf5\x01\n\x07\x41\x63\x63ount\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12P\n\x04spec\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.AccountSpec\x12T\n\x06status\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.AccountStatus\"\x9e\x01\n\x0b\x41\x63\x63ountList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12M\n\x05items\x18\x02 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Account\"\xd1\x02\n\x0b\x41\x63\x63ountSpec\x12\x36\n\ttenantRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x10\n\x08username\x18\x04 \x01(\t\x12\x11\n\tfirstName\x18\x05 \x01(\t\x12\x10\n\x08lastName\x18\x06 \x01(\t\x12\r\n\x05\x65mail\x18\x07 \x01(\t\x12\r\n\x05phone\x18\x08 \x01(\t\x12\r\n\x05\x61\x64min\x18\t \x01(\x08\x12\x10\n\x08memberOf\x18\x0b \x01(\t\x12\x15\n\rresetPassword\x18\r \x01(\x08\x12U\n\x06\x61vatar\x18\x12 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x18\n\x10\x66\x61voriteProducts\x18\x13 \x03(\t\"\xf0\x02\n\rAccountStatus\x12=\n\tupdatedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x02 \x01(\x03\x12\x15\n\rfailureReason\x18\x03 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x04 \x01(\t\x12\x13\n\x0bmodelsCount\x18\x05 \x01(\x05\x12\x19\n\x11modelClassesCount\x18\x06 \x01(\x05\x12\x17\n\x0fpredictorsCount\x18\x07 \x01(\x05\x12\x1a\n\x12\x66\x65\x61tureGroupsCount\x18\x08 \x01(\x05\x12\x15\n\rdatasetsCount\x18\t \x01(\x05\x12\x14\n\x0cmembersCount\x18\n \x01(\x05\x12\x43\n\nconditions\x18\x0b \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xef\x01\n\x05\x41lert\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12N\n\x04spec\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.AlertSpec\x12R\n\x06status\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.AlertStatus\"\x9a\x01\n\tAlertList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12K\n\x05items\x18\x02 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Alert\"\x87\x03\n\tAlertSpec\x12\x0f\n\x07subject\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\r\n\x05level\x18\x03 \x01(\t\x12\x36\n\tentityRef\x18\x04 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x14\n\x0cnotifierName\x18\x05 \x01(\t\x12\r\n\x05owner\x18\x06 \x01(\t\x12\x0b\n\x03ttl\x18\x07 \x01(\x05\x12\\\n\x06\x66ields\x18\x08 \x03(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.AlertSpec.FieldsEntry\x12\x0b\n\x03url\x18\t \x01(\t\x12\r\n\x05image\x18\n \x01(\t\x12\x36\n\ttenantRef\x18\x0b \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x1a-\n\x0b\x46ieldsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x99\x02\n\x0b\x41lertStatus\x12;\n\x07\x66iredAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x03 \x01(\x03\x12=\n\tupdatedAt\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\x12\x43\n\nconditions\x18\x07 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xfe\x01\n\nAttachment\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12S\n\x04spec\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.AttachmentSpec\x12W\n\x06status\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.AttachmentStatus\"\xa4\x01\n\x0e\x41ttachmentList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12P\n\x05items\x18\x02 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Attachment\"\xc6\x01\n\x0e\x41ttachmentSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x36\n\tentityRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x12\n\nbucketName\x18\x04 \x01(\t\x12\x0c\n\x04path\x18\x05 \x01(\t\x12\x36\n\ttenantRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\xe1\x01\n\x10\x41ttachmentStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x03 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x04 \x01(\t\x12\x43\n\nconditions\x18\x05 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"j\n\x14\x42ucketResourceQuotas\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x41\n\thardLimit\x18\x02 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\"\xfe\x01\n\nConnection\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12S\n\x04spec\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ConnectionSpec\x12W\n\x06status\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ConnectionStatus\"\xa4\x01\n\x0e\x43onnectionList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12P\n\x05items\x18\x02 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\xe6\x03\n\x0e\x43onnectionSpec\x12\x36\n\ttenantRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08\x63\x61tegory\x18\x02 \x01(\t\x12\x10\n\x08provider\x18\x03 \x01(\t\x12i\n\nsecretData\x18\x04 \x03(\x0b\x32U.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ConnectionSpec.SecretDataEntry\x12\x63\n\x07options\x18\x05 \x03(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ConnectionSpec.OptionsEntry\x12\r\n\x05owner\x18\x06 \x01(\t\x12\x36\n\tsecretRef\x18\x07 \x01(\x0b\x32#.k8s.io.api.core.v1.SecretReference\x1a\x31\n\x0fSecretDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a.\n\x0cOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xe1\x01\n\x10\x43onnectionStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x03 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x04 \x01(\t\x12\x43\n\nconditions\x18\x05 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x97\x01\n\x0bIngressSpec\x12\x0c\n\x04\x66qdn\x18\x01 \x01(\t\x12\x0c\n\x04grpc\x18\x02 \x01(\x08\x12\x0c\n\x04rest\x18\x03 \x01(\x08\x12\x18\n\x10ingressClassName\x18\x04 \x01(\t\x12\x12\n\nissuerName\x18\x05 \x01(\t\x12\x19\n\x11\x63lusterIssuerName\x18\x06 \x01(\t\x12\x15\n\rtlsSecretName\x18\x07 \x01(\t\"\xe9\x01\n\x03Lab\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12L\n\x04spec\x18\x02 \x01(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.LabSpec\x12P\n\x06status\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.LabStatus\"\x96\x01\n\x07LabList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12I\n\x05items\x18\x02 \x03(\x0b\x32:.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Lab\"\xa3\x02\n\x07LabSpec\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12\x36\n\ttenantRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12X\n\x06limits\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ResourceLimitSpec\x12\x62\n\x0f\x65xternalCluster\x18\x04 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualClusterSpec\x12\r\n\x05owner\x18\x05 \x01(\t\"\xab\x01\n\tLabStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\nconditions\x18\x03 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xf5\x01\n\x07License\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12P\n\x04spec\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.LicenseSpec\x12T\n\x06status\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.LicenseStatus\"\x9e\x01\n\x0bLicenseList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12M\n\x05items\x18\x02 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.License\"\xf9\x03\n\x0bLicenseSpec\x12\x36\n\tsecretRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.SecretReference\x12\r\n\x05\x65mail\x18\x04 \x01(\t\x12@\n\x0ctrialStartAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12>\n\ntrialEndAt\x18\x06 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x13\n\x0bmaxProducts\x18\x07 \x01(\x05\x12\x13\n\x0bmaxTrainers\x18\x08 \x01(\x05\x12\x12\n\nmaxServers\x18\t \x01(\x05\x12\x10\n\x08maxUsers\x18\n \x01(\x05\x12\x15\n\rmaxDataPlanes\x18\x0b \x01(\x05\x12\x10\n\x08\x66orecast\x18\x0c \x01(\x08\x12\x0b\n\x03nlp\x18\r \x01(\x08\x12\x0e\n\x06vision\x18\x0e \x01(\x08\x12\x0f\n\x07\x63hatbot\x18\x0f \x01(\x08\x12\x13\n\x0bproductName\x18\x10 \x01(\t\x12\x11\n\tpriceName\x18\x11 \x01(\t\x12<\n\x08\x65xpireAt\x18\x12 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x14\n\x0cnotifierName\x18\x13 \x01(\t\"\xde\x01\n\rLicenseStatus\x12=\n\tupdatedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x02 \x01(\x03\x12\x15\n\rfailureReason\x18\x03 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x04 \x01(\t\x12\x43\n\nconditions\x18\x05 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xe6\x01\n\x17NotificationChannelSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x16\n\x0e\x63onnectionName\x18\x02 \x01(\t\x12\x0c\n\x04info\x18\x03 \x01(\x08\x12\r\n\x05\x65rror\x18\x04 \x01(\x08\x12\x38\n\x04\x66rom\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x36\n\x02to\x18\x06 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x13\n\x0b\x64\x65stination\x18\x07 \x01(\t\"\x8d\x01\n\x19NotificationChannelStatus\x12\x41\n\rlastMessageAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x02 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x03 \x01(\t\"\xf8\x01\n\x08Notifier\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.NotifierSpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.NotifierStatus\"\xa0\x01\n\x0cNotifierList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Notifier\"\xdd\x01\n\x0cNotifierSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x36\n\ttenantRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\r\n\x05owner\x18\x04 \x01(\t\x12`\n\x08\x63hannels\x18\x05 \x03(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.NotificationChannelSpec\"\x9a\x02\n\x0eNotifierStatus\x12\x1a\n\x12observedGeneration\x18\x02 \x01(\x03\x12=\n\tupdatedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12h\n\x0e\x63hannelsStatus\x18\x04 \x03(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.NotificationChannelStatus\x12\x43\n\nconditions\x18\x05 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xb3\x02\n\x11ResourceLimitSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12>\n\x06maxMem\x18\x02 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\x12>\n\x06maxCpu\x18\x03 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\x12\x0f\n\x07maxPods\x18\x04 \x01(\x05\x12\x0e\n\x06maxPvc\x18\x05 \x01(\x05\x12\x34\n\x05quota\x18\x06 \x01(\x0b\x32%.k8s.io.api.core.v1.ResourceQuotaSpec\x12\x36\n\nlimitRange\x18\x07 \x01(\x0b\x32\".k8s.io.api.core.v1.LimitRangeSpec\"+\n\x08RuleSpec\x12\x10\n\x08resource\x18\x01 \x01(\t\x12\r\n\x05verbs\x18\x02 \x03(\t\"\x81\x02\n\x0bServingSite\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12T\n\x04spec\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ServingSiteSpec\x12X\n\x06status\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ServingSiteStatus\"\xa6\x01\n\x0fServingSiteList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Q\n\x05items\x18\x02 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ServingSite\"\x8f\x03\n\x0fServingSiteSpec\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12\x36\n\ttenantRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12X\n\x06limits\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ResourceLimitSpec\x12S\n\x07ingress\x18\x04 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.IngressSpec\x12\x62\n\x0f\x65xternalCluster\x18\x05 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualClusterSpec\x12\r\n\x05owner\x18\x07 \x01(\t\x12\r\n\x05stage\x18\x08 \x01(\t\"\x90\x04\n\x11ServingSiteStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x18\n\x10\x61\x63tivePredictors\x18\x03 \x01(\x05\x12\x1a\n\x12inactivePredictors\x18\x04 \x01(\x05\x12#\n\x1btotalPredictorServiceFailed\x18\x05 \x01(\x05\x12%\n\x1dtotalPredictorDataDriftFailed\x18\x06 \x01(\x05\x12$\n\x1ctotalPredictorAccuracyFailed\x18\x07 \x01(\x05\x12\x1e\n\x16\x64\x61ilyPredictionsCounts\x18\x08 \x03(\x05\x12\x15\n\rfailureReason\x18\t \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\n \x01(\t\x12\x17\n\x0fgrpcIngressName\x18\x0b \x01(\t\x12\x17\n\x0frestIngressName\x18\x0c \x01(\t\x12\x18\n\x10grpcIngressReady\x18\r \x01(\x08\x12\x18\n\x10restIngressReady\x18\x0e \x01(\x08\x12\x43\n\nconditions\x18\x0f \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xf2\x01\n\x06Tenant\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12O\n\x04spec\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.TenantSpec\x12S\n\x06status\x18\x03 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.TenantStatus\"\x9c\x01\n\nTenantList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12L\n\x05items\x18\x02 \x03(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Tenant\"\xa7\x03\n\nTenantSpec\x12\x16\n\x0e\x64\x65\x66\x61ultLabName\x18\x01 \x01(\t\x12\x1e\n\x16\x64\x65\x66\x61ultServingSiteName\x18\x02 \x01(\t\x12\x19\n\x11\x64\x65\x66\x61ultBucketName\x18\x03 \x01(\t\x12]\n\x0bpermissions\x18\x04 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PermissionsSpec\x12_\n\x0cnotification\x18\x05 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\x42\n\x15onlineStoreConnection\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x42\n\x15metricStoreConnection\x18\x07 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\xdd\x01\n\x0cTenantStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x03 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x04 \x01(\t\x12\x43\n\nconditions\x18\x05 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xab\x01\n\rUserRoleClass\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.UserRoleClassSpec\"\xaa\x01\n\x11UserRoleClassList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.UserRoleClass\"\xbf\x01\n\x11UserRoleClassSpec\x12\x36\n\ttenantRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\r\n\x05owner\x18\x03 \x01(\t\x12N\n\x05rules\x18\x04 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.RuleSpec\"\x87\x02\n\rVirtualBucket\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucketSpec\x12Z\n\x06status\x18\x03 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucketStatus\"\xaa\x01\n\x11VirtualBucketList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\"\x88\x02\n\x11VirtualBucketSpec\x12\x36\n\ttenantRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x16\n\x0e\x63onnectionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\r\n\x05owner\x18\x04 \x01(\t\x12\x0e\n\x06region\x18\x05 \x01(\t\x12\x12\n\nversioning\x18\x06 \x01(\x08\x12[\n\x06quotas\x18\x07 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.BucketResourceQuotas\"\xe4\x01\n\x13VirtualBucketStatus\x12=\n\tupdatedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x03 \x01(\x03\x12\x15\n\rfailureReason\x18\x04 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x05 \x01(\t\x12\x43\n\nconditions\x18\x06 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xdb\x03\n\x12VirtualClusterSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\r\n\x05nodes\x18\x03 \x01(\x05\x12\x14\n\x0cinstanceType\x18\x04 \x01(\t\x12\x0c\n\x04gpus\x18\x05 \x01(\x05\x12\x14\n\x0cgpuClassName\x18\x06 \x01(\t\x12\x12\n\nvolumeSize\x18\x07 \x01(\x05\x12\x0c\n\x04spot\x18\x08 \x01(\x08\x12\x16\n\x0e\x63onnectionName\x18\t \x01(\t\x12\r\n\x05owner\x18\n \x01(\t\x12X\n\x06limits\x18\x0b \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ResourceLimitSpec\x12\x0e\n\x06region\x18\x0c \x01(\t\x12\n\n\x02\x61z\x18\r \x01(\t\x12\x19\n\x11kubernetesVersion\x18\x0e \x01(\t\x12\x11\n\tautoscale\x18\x0f \x01(\x08\x12\x10\n\x08minNodes\x18\x10 \x01(\x05\x12\x10\n\x08maxNodes\x18\x11 \x01(\x05\x12\x35\n\x08\x63loudRef\x18\x12 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0e\n\x06sshKey\x18\x13 \x01(\tB7Z5github.com/metaprov/modelaapi/pkg/apis/infra/v1alpha1')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nEgithub.com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated.proto\x12\x35github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/api/resource/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\xf5\x01\n\x07\x41\x63\x63ount\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12P\n\x04spec\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.AccountSpec\x12T\n\x06status\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.AccountStatus\"\x9e\x01\n\x0b\x41\x63\x63ountList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12M\n\x05items\x18\x02 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Account\"\xd1\x02\n\x0b\x41\x63\x63ountSpec\x12\x36\n\ttenantRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x10\n\x08username\x18\x04 \x01(\t\x12\x11\n\tfirstName\x18\x05 \x01(\t\x12\x10\n\x08lastName\x18\x06 \x01(\t\x12\r\n\x05\x65mail\x18\x07 \x01(\t\x12\r\n\x05phone\x18\x08 \x01(\t\x12\r\n\x05\x61\x64min\x18\t \x01(\x08\x12\x10\n\x08memberOf\x18\x0b \x01(\t\x12\x15\n\rresetPassword\x18\r \x01(\x08\x12U\n\x06\x61vatar\x18\x12 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x18\n\x10\x66\x61voriteProducts\x18\x13 \x03(\t\"\xf0\x02\n\rAccountStatus\x12=\n\tupdatedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x02 \x01(\x03\x12\x15\n\rfailureReason\x18\x03 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x04 \x01(\t\x12\x13\n\x0bmodelsCount\x18\x05 \x01(\x05\x12\x19\n\x11modelClassesCount\x18\x06 \x01(\x05\x12\x17\n\x0fpredictorsCount\x18\x07 \x01(\x05\x12\x1a\n\x12\x66\x65\x61tureGroupsCount\x18\x08 \x01(\x05\x12\x15\n\rdatasetsCount\x18\t \x01(\x05\x12\x14\n\x0cmembersCount\x18\n \x01(\x05\x12\x43\n\nconditions\x18\x0b \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xef\x01\n\x05\x41lert\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12N\n\x04spec\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.AlertSpec\x12R\n\x06status\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.AlertStatus\"\x9a\x01\n\tAlertList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12K\n\x05items\x18\x02 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Alert\"\xfc\x02\n\tAlertSpec\x12\x0f\n\x07subject\x18\x01 \x01(\t\x12\r\n\x05level\x18\x02 \x01(\t\x12\x36\n\tentityRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\r\n\x05owner\x18\x04 \x01(\t\x12\\\n\x06\x66ields\x18\x05 \x03(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.AlertSpec.FieldsEntry\x12\x0b\n\x03url\x18\x06 \x01(\t\x12\r\n\x05image\x18\x07 \x01(\t\x12_\n\x0cnotification\x18\x08 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x1a-\n\x0b\x46ieldsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x82\x02\n\x0b\x41lertStatus\x12;\n\x07\x66iredAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x03 \x01(\x03\x12=\n\tupdatedAt\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x16\n\x0e\x66\x61ilureMessage\x18\x05 \x01(\t\x12\x43\n\nconditions\x18\x06 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xfe\x01\n\nAttachment\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12S\n\x04spec\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.AttachmentSpec\x12W\n\x06status\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.AttachmentStatus\"\xa4\x01\n\x0e\x41ttachmentList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12P\n\x05items\x18\x02 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Attachment\"\xc6\x01\n\x0e\x41ttachmentSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x36\n\tentityRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x12\n\nbucketName\x18\x04 \x01(\t\x12\x0c\n\x04path\x18\x05 \x01(\t\x12\x36\n\ttenantRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\xe1\x01\n\x10\x41ttachmentStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x03 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x04 \x01(\t\x12\x43\n\nconditions\x18\x05 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xfe\x01\n\nConnection\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12S\n\x04spec\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ConnectionSpec\x12W\n\x06status\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ConnectionStatus\"\xa4\x01\n\x0e\x43onnectionList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12P\n\x05items\x18\x02 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\xe6\x03\n\x0e\x43onnectionSpec\x12\x36\n\ttenantRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08\x63\x61tegory\x18\x02 \x01(\t\x12\x10\n\x08provider\x18\x03 \x01(\t\x12i\n\nsecretData\x18\x04 \x03(\x0b\x32U.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ConnectionSpec.SecretDataEntry\x12\x63\n\x07options\x18\x05 \x03(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ConnectionSpec.OptionsEntry\x12\r\n\x05owner\x18\x06 \x01(\t\x12\x36\n\tsecretRef\x18\x07 \x01(\x0b\x32#.k8s.io.api.core.v1.SecretReference\x1a\x31\n\x0fSecretDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a.\n\x0cOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xe1\x01\n\x10\x43onnectionStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x03 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x04 \x01(\t\x12\x43\n\nconditions\x18\x05 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x97\x01\n\x0bIngressSpec\x12\x0c\n\x04\x66qdn\x18\x01 \x01(\t\x12\x0c\n\x04grpc\x18\x02 \x01(\x08\x12\x0c\n\x04http\x18\x03 \x01(\x08\x12\x18\n\x10ingressClassName\x18\x04 \x01(\t\x12\x12\n\nissuerName\x18\x05 \x01(\t\x12\x19\n\x11\x63lusterIssuerName\x18\x06 \x01(\t\x12\x15\n\rtlsSecretName\x18\x07 \x01(\t\"\xe9\x01\n\x03Lab\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12L\n\x04spec\x18\x02 \x01(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.LabSpec\x12P\n\x06status\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.LabStatus\"\x96\x01\n\x07LabList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12I\n\x05items\x18\x02 \x03(\x0b\x32:.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Lab\"\xa3\x02\n\x07LabSpec\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12\x36\n\ttenantRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12X\n\x06limits\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ResourceLimitSpec\x12\x62\n\x0f\x65xternalCluster\x18\x04 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualClusterSpec\x12\r\n\x05owner\x18\x05 \x01(\t\"\xab\x01\n\tLabStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\nconditions\x18\x03 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xf5\x01\n\x07License\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12P\n\x04spec\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.LicenseSpec\x12T\n\x06status\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.LicenseStatus\"\x9e\x01\n\x0bLicenseList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12M\n\x05items\x18\x02 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.License\"\xf9\x03\n\x0bLicenseSpec\x12\x36\n\tsecretRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.SecretReference\x12\r\n\x05\x65mail\x18\x04 \x01(\t\x12@\n\x0ctrialStartAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12>\n\ntrialEndAt\x18\x06 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x13\n\x0bmaxProducts\x18\x07 \x01(\x05\x12\x13\n\x0bmaxTrainers\x18\x08 \x01(\x05\x12\x12\n\nmaxServers\x18\t \x01(\x05\x12\x10\n\x08maxUsers\x18\n \x01(\x05\x12\x15\n\rmaxDataPlanes\x18\x0b \x01(\x05\x12\x10\n\x08\x66orecast\x18\x0c \x01(\x08\x12\x0b\n\x03nlp\x18\r \x01(\x08\x12\x0e\n\x06vision\x18\x0e \x01(\x08\x12\x0f\n\x07\x63hatbot\x18\x0f \x01(\x08\x12\x13\n\x0bproductName\x18\x10 \x01(\t\x12\x11\n\tpriceName\x18\x11 \x01(\t\x12<\n\x08\x65xpireAt\x18\x12 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x14\n\x0cnotifierName\x18\x13 \x01(\t\"\xde\x01\n\rLicenseStatus\x12=\n\tupdatedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x02 \x01(\x03\x12\x15\n\rfailureReason\x18\x03 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x04 \x01(\t\x12\x43\n\nconditions\x18\x05 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"t\n\x17NotificationChannelSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x16\n\x0e\x63onnectionName\x18\x02 \x01(\t\x12\x0c\n\x04info\x18\x03 \x01(\x08\x12\r\n\x05\x65rror\x18\x04 \x01(\x08\x12\x13\n\x0b\x64\x65stination\x18\x07 \x01(\t\"\x8e\x01\n\x19NotificationChannelStatus\x12\x16\n\x0e\x63onnectionName\x18\x02 \x01(\t\x12\x41\n\rlastMessageAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x16\n\x0e\x66\x61ilureMessage\x18\x03 \x01(\t\"\xf8\x01\n\x08Notifier\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.NotifierSpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.NotifierStatus\"\xa0\x01\n\x0cNotifierList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Notifier\"\xdd\x01\n\x0cNotifierSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x36\n\ttenantRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\r\n\x05owner\x18\x04 \x01(\t\x12`\n\x08\x63hannels\x18\x05 \x03(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.NotificationChannelSpec\"\x9a\x02\n\x0eNotifierStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12h\n\x0e\x63hannelsStatus\x18\x03 \x03(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.NotificationChannelStatus\x12\x43\n\nconditions\x18\x04 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xb3\x02\n\x11ResourceLimitSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12>\n\x06maxMem\x18\x02 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\x12>\n\x06maxCpu\x18\x03 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\x12\x0f\n\x07maxPods\x18\x04 \x01(\x05\x12\x0e\n\x06maxPvc\x18\x05 \x01(\x05\x12\x34\n\x05quota\x18\x06 \x01(\x0b\x32%.k8s.io.api.core.v1.ResourceQuotaSpec\x12\x36\n\nlimitRange\x18\x07 \x01(\x0b\x32\".k8s.io.api.core.v1.LimitRangeSpec\"+\n\x08RuleSpec\x12\x10\n\x08resource\x18\x01 \x01(\t\x12\r\n\x05verbs\x18\x02 \x03(\t\"\x81\x02\n\x0bServingSite\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12T\n\x04spec\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ServingSiteSpec\x12X\n\x06status\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ServingSiteStatus\"\xa6\x01\n\x0fServingSiteList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Q\n\x05items\x18\x02 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ServingSite\"\x8f\x03\n\x0fServingSiteSpec\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12\x36\n\ttenantRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12X\n\x06limits\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ResourceLimitSpec\x12S\n\x07ingress\x18\x04 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.IngressSpec\x12\x62\n\x0f\x65xternalCluster\x18\x05 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualClusterSpec\x12\r\n\x05owner\x18\x07 \x01(\t\x12\r\n\x05stage\x18\x08 \x01(\t\"\x90\x04\n\x11ServingSiteStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x18\n\x10\x61\x63tivePredictors\x18\x03 \x01(\x05\x12\x1a\n\x12inactivePredictors\x18\x04 \x01(\x05\x12#\n\x1btotalPredictorServiceFailed\x18\x05 \x01(\x05\x12%\n\x1dtotalPredictorDataDriftFailed\x18\x06 \x01(\x05\x12$\n\x1ctotalPredictorAccuracyFailed\x18\x07 \x01(\x05\x12\x1e\n\x16\x64\x61ilyPredictionsCounts\x18\x08 \x03(\x05\x12\x15\n\rfailureReason\x18\t \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\n \x01(\t\x12\x17\n\x0fgrpcIngressName\x18\x0b \x01(\t\x12\x17\n\x0frestIngressName\x18\x0c \x01(\t\x12\x18\n\x10grpcIngressReady\x18\r \x01(\x08\x12\x18\n\x10restIngressReady\x18\x0e \x01(\x08\x12\x43\n\nconditions\x18\x0f \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xf2\x01\n\x06Tenant\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12O\n\x04spec\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.TenantSpec\x12S\n\x06status\x18\x03 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.TenantStatus\"\x9c\x01\n\nTenantList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12L\n\x05items\x18\x02 \x03(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Tenant\"\xc0\x03\n\nTenantSpec\x12\x16\n\x0e\x64\x65\x66\x61ultLabName\x18\x01 \x01(\t\x12\x1e\n\x16\x64\x65\x66\x61ultServingSiteName\x18\x02 \x01(\t\x12\x19\n\x11\x64\x65\x66\x61ultBucketName\x18\x03 \x01(\t\x12\x17\n\x0f\x63\x61\x63heBucketName\x18\x04 \x01(\t\x12]\n\x0bpermissions\x18\x05 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PermissionsSpec\x12_\n\x0cnotification\x18\x06 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\x42\n\x15onlineStoreConnection\x18\x07 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x42\n\x15metricStoreConnection\x18\x08 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\xdd\x01\n\x0cTenantStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x03 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x04 \x01(\t\x12\x43\n\nconditions\x18\x05 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xab\x01\n\rUserRoleClass\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.UserRoleClassSpec\"\xaa\x01\n\x11UserRoleClassList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.UserRoleClass\"\xbf\x01\n\x11UserRoleClassSpec\x12\x36\n\ttenantRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\r\n\x05owner\x18\x03 \x01(\t\x12N\n\x05rules\x18\x04 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.RuleSpec\"\x87\x02\n\rVirtualBucket\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucketSpec\x12Z\n\x06status\x18\x03 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucketStatus\"\xaa\x01\n\x11VirtualBucketList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\"O\n\x11VirtualBucketSpec\x12\x16\n\x0e\x63onnectionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\r\n\x05owner\x18\x04 \x01(\t\"\xcd\x01\n\x13VirtualBucketStatus\x12=\n\tupdatedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12observedGeneration\x18\x03 \x01(\x03\x12\x16\n\x0e\x66\x61ilureMessage\x18\x05 \x01(\t\x12\x43\n\nconditions\x18\x06 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xdb\x03\n\x12VirtualClusterSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\r\n\x05nodes\x18\x03 \x01(\x05\x12\x14\n\x0cinstanceType\x18\x04 \x01(\t\x12\x0c\n\x04gpus\x18\x05 \x01(\x05\x12\x14\n\x0cgpuClassName\x18\x06 \x01(\t\x12\x12\n\nvolumeSize\x18\x07 \x01(\x05\x12\x0c\n\x04spot\x18\x08 \x01(\x08\x12\x16\n\x0e\x63onnectionName\x18\t \x01(\t\x12\r\n\x05owner\x18\n \x01(\t\x12X\n\x06limits\x18\x0b \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.ResourceLimitSpec\x12\x0e\n\x06region\x18\x0c \x01(\t\x12\n\n\x02\x61z\x18\r \x01(\t\x12\x19\n\x11kubernetesVersion\x18\x0e \x01(\t\x12\x11\n\tautoscale\x18\x0f \x01(\x08\x12\x10\n\x08minNodes\x18\x10 \x01(\x05\x12\x10\n\x08maxNodes\x18\x11 \x01(\x05\x12\x35\n\x08\x63loudRef\x18\x12 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0e\n\x06sshKey\x18\x13 \x01(\tB7Z5github.com/metaprov/modelaapi/pkg/apis/infra/v1alpha1')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.generated_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z5github.com/metaprov/modelaapi/pkg/apis/infra/v1alpha1'
@@ -42,101 +42,99 @@
   _ACCOUNTSTATUS._serialized_start=1200
   _ACCOUNTSTATUS._serialized_end=1568
   _ALERT._serialized_start=1571
   _ALERT._serialized_end=1810
   _ALERTLIST._serialized_start=1813
   _ALERTLIST._serialized_end=1967
   _ALERTSPEC._serialized_start=1970
-  _ALERTSPEC._serialized_end=2361
-  _ALERTSPEC_FIELDSENTRY._serialized_start=2316
-  _ALERTSPEC_FIELDSENTRY._serialized_end=2361
-  _ALERTSTATUS._serialized_start=2364
-  _ALERTSTATUS._serialized_end=2645
-  _ATTACHMENT._serialized_start=2648
-  _ATTACHMENT._serialized_end=2902
-  _ATTACHMENTLIST._serialized_start=2905
-  _ATTACHMENTLIST._serialized_end=3069
-  _ATTACHMENTSPEC._serialized_start=3072
-  _ATTACHMENTSPEC._serialized_end=3270
-  _ATTACHMENTSTATUS._serialized_start=3273
-  _ATTACHMENTSTATUS._serialized_end=3498
-  _BUCKETRESOURCEQUOTAS._serialized_start=3500
-  _BUCKETRESOURCEQUOTAS._serialized_end=3606
-  _CONNECTION._serialized_start=3609
-  _CONNECTION._serialized_end=3863
-  _CONNECTIONLIST._serialized_start=3866
-  _CONNECTIONLIST._serialized_end=4030
-  _CONNECTIONSPEC._serialized_start=4033
-  _CONNECTIONSPEC._serialized_end=4519
-  _CONNECTIONSPEC_SECRETDATAENTRY._serialized_start=4422
-  _CONNECTIONSPEC_SECRETDATAENTRY._serialized_end=4471
-  _CONNECTIONSPEC_OPTIONSENTRY._serialized_start=4473
-  _CONNECTIONSPEC_OPTIONSENTRY._serialized_end=4519
-  _CONNECTIONSTATUS._serialized_start=4522
-  _CONNECTIONSTATUS._serialized_end=4747
-  _INGRESSSPEC._serialized_start=4750
-  _INGRESSSPEC._serialized_end=4901
-  _LAB._serialized_start=4904
-  _LAB._serialized_end=5137
-  _LABLIST._serialized_start=5140
-  _LABLIST._serialized_end=5290
-  _LABSPEC._serialized_start=5293
-  _LABSPEC._serialized_end=5584
-  _LABSTATUS._serialized_start=5587
-  _LABSTATUS._serialized_end=5758
-  _LICENSE._serialized_start=5761
-  _LICENSE._serialized_end=6006
-  _LICENSELIST._serialized_start=6009
-  _LICENSELIST._serialized_end=6167
-  _LICENSESPEC._serialized_start=6170
-  _LICENSESPEC._serialized_end=6675
-  _LICENSESTATUS._serialized_start=6678
-  _LICENSESTATUS._serialized_end=6900
-  _NOTIFICATIONCHANNELSPEC._serialized_start=6903
-  _NOTIFICATIONCHANNELSPEC._serialized_end=7133
-  _NOTIFICATIONCHANNELSTATUS._serialized_start=7136
-  _NOTIFICATIONCHANNELSTATUS._serialized_end=7277
-  _NOTIFIER._serialized_start=7280
-  _NOTIFIER._serialized_end=7528
-  _NOTIFIERLIST._serialized_start=7531
-  _NOTIFIERLIST._serialized_end=7691
-  _NOTIFIERSPEC._serialized_start=7694
-  _NOTIFIERSPEC._serialized_end=7915
-  _NOTIFIERSTATUS._serialized_start=7918
-  _NOTIFIERSTATUS._serialized_end=8200
-  _RESOURCELIMITSPEC._serialized_start=8203
-  _RESOURCELIMITSPEC._serialized_end=8510
-  _RULESPEC._serialized_start=8512
-  _RULESPEC._serialized_end=8555
-  _SERVINGSITE._serialized_start=8558
-  _SERVINGSITE._serialized_end=8815
-  _SERVINGSITELIST._serialized_start=8818
-  _SERVINGSITELIST._serialized_end=8984
-  _SERVINGSITESPEC._serialized_start=8987
-  _SERVINGSITESPEC._serialized_end=9386
-  _SERVINGSITESTATUS._serialized_start=9389
-  _SERVINGSITESTATUS._serialized_end=9917
-  _TENANT._serialized_start=9920
-  _TENANT._serialized_end=10162
-  _TENANTLIST._serialized_start=10165
-  _TENANTLIST._serialized_end=10321
-  _TENANTSPEC._serialized_start=10324
-  _TENANTSPEC._serialized_end=10747
-  _TENANTSTATUS._serialized_start=10750
-  _TENANTSTATUS._serialized_end=10971
-  _USERROLECLASS._serialized_start=10974
-  _USERROLECLASS._serialized_end=11145
-  _USERROLECLASSLIST._serialized_start=11148
-  _USERROLECLASSLIST._serialized_end=11318
-  _USERROLECLASSSPEC._serialized_start=11321
-  _USERROLECLASSSPEC._serialized_end=11512
-  _VIRTUALBUCKET._serialized_start=11515
-  _VIRTUALBUCKET._serialized_end=11778
-  _VIRTUALBUCKETLIST._serialized_start=11781
-  _VIRTUALBUCKETLIST._serialized_end=11951
-  _VIRTUALBUCKETSPEC._serialized_start=11954
-  _VIRTUALBUCKETSPEC._serialized_end=12218
-  _VIRTUALBUCKETSTATUS._serialized_start=12221
-  _VIRTUALBUCKETSTATUS._serialized_end=12449
-  _VIRTUALCLUSTERSPEC._serialized_start=12452
-  _VIRTUALCLUSTERSPEC._serialized_end=12927
+  _ALERTSPEC._serialized_end=2350
+  _ALERTSPEC_FIELDSENTRY._serialized_start=2305
+  _ALERTSPEC_FIELDSENTRY._serialized_end=2350
+  _ALERTSTATUS._serialized_start=2353
+  _ALERTSTATUS._serialized_end=2611
+  _ATTACHMENT._serialized_start=2614
+  _ATTACHMENT._serialized_end=2868
+  _ATTACHMENTLIST._serialized_start=2871
+  _ATTACHMENTLIST._serialized_end=3035
+  _ATTACHMENTSPEC._serialized_start=3038
+  _ATTACHMENTSPEC._serialized_end=3236
+  _ATTACHMENTSTATUS._serialized_start=3239
+  _ATTACHMENTSTATUS._serialized_end=3464
+  _CONNECTION._serialized_start=3467
+  _CONNECTION._serialized_end=3721
+  _CONNECTIONLIST._serialized_start=3724
+  _CONNECTIONLIST._serialized_end=3888
+  _CONNECTIONSPEC._serialized_start=3891
+  _CONNECTIONSPEC._serialized_end=4377
+  _CONNECTIONSPEC_SECRETDATAENTRY._serialized_start=4280
+  _CONNECTIONSPEC_SECRETDATAENTRY._serialized_end=4329
+  _CONNECTIONSPEC_OPTIONSENTRY._serialized_start=4331
+  _CONNECTIONSPEC_OPTIONSENTRY._serialized_end=4377
+  _CONNECTIONSTATUS._serialized_start=4380
+  _CONNECTIONSTATUS._serialized_end=4605
+  _INGRESSSPEC._serialized_start=4608
+  _INGRESSSPEC._serialized_end=4759
+  _LAB._serialized_start=4762
+  _LAB._serialized_end=4995
+  _LABLIST._serialized_start=4998
+  _LABLIST._serialized_end=5148
+  _LABSPEC._serialized_start=5151
+  _LABSPEC._serialized_end=5442
+  _LABSTATUS._serialized_start=5445
+  _LABSTATUS._serialized_end=5616
+  _LICENSE._serialized_start=5619
+  _LICENSE._serialized_end=5864
+  _LICENSELIST._serialized_start=5867
+  _LICENSELIST._serialized_end=6025
+  _LICENSESPEC._serialized_start=6028
+  _LICENSESPEC._serialized_end=6533
+  _LICENSESTATUS._serialized_start=6536
+  _LICENSESTATUS._serialized_end=6758
+  _NOTIFICATIONCHANNELSPEC._serialized_start=6760
+  _NOTIFICATIONCHANNELSPEC._serialized_end=6876
+  _NOTIFICATIONCHANNELSTATUS._serialized_start=6879
+  _NOTIFICATIONCHANNELSTATUS._serialized_end=7021
+  _NOTIFIER._serialized_start=7024
+  _NOTIFIER._serialized_end=7272
+  _NOTIFIERLIST._serialized_start=7275
+  _NOTIFIERLIST._serialized_end=7435
+  _NOTIFIERSPEC._serialized_start=7438
+  _NOTIFIERSPEC._serialized_end=7659
+  _NOTIFIERSTATUS._serialized_start=7662
+  _NOTIFIERSTATUS._serialized_end=7944
+  _RESOURCELIMITSPEC._serialized_start=7947
+  _RESOURCELIMITSPEC._serialized_end=8254
+  _RULESPEC._serialized_start=8256
+  _RULESPEC._serialized_end=8299
+  _SERVINGSITE._serialized_start=8302
+  _SERVINGSITE._serialized_end=8559
+  _SERVINGSITELIST._serialized_start=8562
+  _SERVINGSITELIST._serialized_end=8728
+  _SERVINGSITESPEC._serialized_start=8731
+  _SERVINGSITESPEC._serialized_end=9130
+  _SERVINGSITESTATUS._serialized_start=9133
+  _SERVINGSITESTATUS._serialized_end=9661
+  _TENANT._serialized_start=9664
+  _TENANT._serialized_end=9906
+  _TENANTLIST._serialized_start=9909
+  _TENANTLIST._serialized_end=10065
+  _TENANTSPEC._serialized_start=10068
+  _TENANTSPEC._serialized_end=10516
+  _TENANTSTATUS._serialized_start=10519
+  _TENANTSTATUS._serialized_end=10740
+  _USERROLECLASS._serialized_start=10743
+  _USERROLECLASS._serialized_end=10914
+  _USERROLECLASSLIST._serialized_start=10917
+  _USERROLECLASSLIST._serialized_end=11087
+  _USERROLECLASSSPEC._serialized_start=11090
+  _USERROLECLASSSPEC._serialized_end=11281
+  _VIRTUALBUCKET._serialized_start=11284
+  _VIRTUALBUCKET._serialized_end=11547
+  _VIRTUALBUCKETLIST._serialized_start=11550
+  _VIRTUALBUCKETLIST._serialized_end=11720
+  _VIRTUALBUCKETSPEC._serialized_start=11722
+  _VIRTUALBUCKETSPEC._serialized_end=11801
+  _VIRTUALBUCKETSTATUS._serialized_start=11804
+  _VIRTUALBUCKETSTATUS._serialized_end=12009
+  _VIRTUALCLUSTERSPEC._serialized_start=12012
+  _VIRTUALCLUSTERSPEC._serialized_end=12487
 # @@protoc_insertion_point(module_scope)
```

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_data_dot_v1alpha1_dot_generated__pb2
 from k8s.io.api.core.v1 import generated_pb2 as k8s_dot_io_dot_api_dot_core_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.apis.meta.v1 import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_apis_dot_meta_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime.schema import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_schema_dot_generated__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nHgithub.com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated.proto\x12\x38github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\x80\x01\n\x17\x41lgorithmParameterRange\x12\x0c\n\x04name\x18\x01 \x01(\t\x12W\n\x06ranges\x18\x02 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ParameterRange\"\x9f\x01\n\x18\x41lgorithmSearchSpaceSpec\x12\x0f\n\x07include\x18\x01 \x03(\t\x12\x0f\n\x07\x65xclude\x18\x02 \x03(\t\x12\x61\n\x06\x63ustom\x18\x03 \x03(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AlgorithmParameterRange\"`\n\x07\x41nomaly\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0bvalueColumn\x18\x02 \x01(\t\x12\x16\n\x0e\x61\x64jDeltaColumn\x18\x03 \x01(\t\x12\r\n\x05start\x18\x04 \x01(\t\x12\x0b\n\x03\x65nd\x18\x05 \x01(\t\"\'\n\x11\x41udioPipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\"M\n\x0c\x42\x61\x63ktestSpec\x12\x0f\n\x07sliding\x18\x01 \x01(\x08\x12\x0e\n\x06splits\x18\x02 \x01(\x05\x12\x0f\n\x07Initial\x18\x03 \x01(\x05\x12\x0b\n\x03gap\x18\x05 \x01(\x05\"?\n\x0c\x42\x61selineSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tbaselines\x18\x02 \x03(\t\x12\x0b\n\x03\x61ll\x18\x03 \x01(\x08\"\r\n\x0b\x43hangePoint\"$\n\x14\x43hatbotEstimatorSpec\x12\x0c\n\x04\x62\x61se\x18\x01 \x01(\t\"\x96\x01\n\x0e\x43heckpointSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1a\n\x12\x63heckpointInterval\x18\x02 \x01(\x05\x12W\n\x08location\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\x92\x01\n\x16\x43lassicalEstimatorSpec\x12\x15\n\ralgorithmName\x18\x01 \x01(\t\x12\x61\n\nparameters\x18\x02 \x03(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.HyperParameterValue\"a\n\x10\x43ustomReportSpec\x12M\n\x05pages\x18\x08 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.PageSpec\"L\n\nDataHashes\x12\x11\n\ttrainHash\x18\x01 \x01(\t\x12\x13\n\x0btestingHash\x18\x02 \x01(\t\x12\x16\n\x0evalidationHash\x18\x03 \x01(\t\"\x84\x02\n\rDataSplitSpec\x12\x0e\n\x06method\x18\x01 \x01(\t\x12\r\n\x05train\x18\x02 \x01(\x05\x12\x12\n\nvalidation\x18\x03 \x01(\x05\x12\x0c\n\x04test\x18\x04 \x01(\x05\x12\x13\n\x0bsplitColumn\x18\x05 \x01(\t\x12W\n\x08segments\x18\x06 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SegmentSpec\x12\x14\n\x0ctrainDataset\x18\x07 \x01(\t\x12\x13\n\x0btestDataset\x18\x08 \x01(\t\x12\x19\n\x11validationDataset\x18\t \x01(\t\"\xa5\x01\n\x12\x44\x65\x65pEstimatorLayer\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12^\n\nparameters\x18\x03 \x03(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.NNLayerParameter\x12\x13\n\x0binputLayers\x18\x04 \x03(\t\"\xe6\x01\n\x11\x44\x65\x65pEstimatorSpec\x12\\\n\x06layers\x18\x01 \x03(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DeepEstimatorLayer\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x11\n\tbatchSize\x18\x03 \x01(\x05\x12\x0e\n\x06\x65pochs\x18\x04 \x01(\x05\x12\x17\n\x0fvalidationSplit\x18\x05 \x01(\x05\x12\r\n\x05isSeq\x18\x06 \x01(\x08\x12\x0c\n\x04gpus\x18\x07 \x01(\x05\x12\x0c\n\x04loss\x18\x08 \x01(\t\".\n\x13\x44riftDetectorStatus\x12\x17\n\x0foutlierModelURI\x18\x01 \x01(\t\";\n\x0e\x44riftModelSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x18\n\x10outlierAlgorithm\x18\x02 \x01(\t\"R\n\rEarlyStopSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07initial\x18\x02 \x01(\x05\x12\x1f\n\x17minModelsWithNoProgress\x18\x03 \x01(\x05\"\x0f\n\rEnsembleRules\"\xf3\x01\n\x0c\x45nsembleSpec\x12\x0e\n\x06models\x18\x01 \x03(\t\x12\x64\n\nestimators\x18\x02 \x03(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12_\n\x05\x66inal\x18\x03 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12\x0c\n\x04type\x18\x04 \x01(\t\"_\n\rEnsemblesSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x16\n\x0evotingEnsemble\x18\x02 \x01(\x08\x12\x18\n\x10stackingEnsemble\x18\x03 \x01(\x08\x12\x0b\n\x03top\x18\x04 \x01(\x05\"*\n\tEntityRef\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07\x65xclude\x18\x02 \x03(\t\"\x89\x01\n\x0b\x45valMetrics\x12\x11\n\tselection\x18\x01 \x01(\t\x12\x11\n\treporting\x18\x02 \x03(\t\x12\x0f\n\x07\x61ggFunc\x18\x03 \x01(\t\x12\x11\n\taggPeriod\x18\x04 \x01(\x05\x12\x17\n\x0fnullModelParams\x18\x05 \x01(\t\x12\x17\n\x0frelErrTolerance\x18\x06 \x01(\x01\"\xe0\x01\n\nEvalPeriod\x12\x13\n\x0btestHorizon\x18\x01 \x01(\x05\x12\x1f\n\x17periodsBetweenTrainTest\x18\x02 \x01(\x05\x12\x1e\n\x16\x63vPeriodsBetweenSplits\x18\x03 \x01(\x05\x12\x1a\n\x12\x63vExpandingWindows\x18\x04 \x01(\x08\x12\x11\n\tcvHorizon\x18\x05 \x01(\x05\x12\x19\n\x11\x63vMinTrainPeriods\x18\x06 \x01(\x05\x12\x13\n\x0b\x63vMaxSplits\x18\x07 \x01(\x05\x12\x1d\n\x15\x63vUseMostRecentSplits\x18\x08 \x01(\x08\"\xc7\x06\n\x1a\x46\x65\x61tureEngineeringPipeline\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x03 \x03(\t\x12\x12\n\nimputation\x18\x04 \x01(\t\x12\x10\n\x08\x65ncoding\x18\x05 \x01(\t\x12\x0f\n\x07scaling\x18\x06 \x01(\t\x12\x16\n\x0e\x64iscretisation\x18\x07 \x01(\t\x12\x1e\n\x16variableTransformation\x18\x08 \x01(\t\x12\x17\n\x0foutlierHandling\x18\t \x01(\t\x12\x1e\n\x16\x64\x61tetimeTransformation\x18\n \x01(\t\x12X\n\x04text\x18\x0b \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TextPipelineSpec\x12Z\n\x05image\x18\x0c \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ImagePipelineSpec\x12Z\n\x05\x61udio\x18\r \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AudioPipelineSpec\x12Z\n\x05video\x18\x0e \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.VideoPipelineSpec\x12`\n\tgenerated\x18\x10 \x03(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GeneratedColumnSpec\x12]\n\x06\x63ustom\x18\x11 \x03(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GeneratedColumnSpec\x12\x0c\n\x04\x64rop\x18\x12 \x01(\x08\x12\x13\n\x0bpassthrough\x18\x13 \x01(\x08\"\x8d\x03\n\x1c\x46\x65\x61tureEngineeringSearchSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x19\n\x11imbalancedHandler\x18\x02 \x01(\t\x12\x11\n\testimator\x18\x03 \x01(\t\x12\x11\n\tmaxModels\x18\x04 \x01(\x05\x12\x0f\n\x07maxTime\x18\x05 \x01(\x05\x12\x13\n\x0bmaxTrainers\x18\x06 \x01(\x05\x12\x11\n\tsamplePct\x18\x07 \x01(\x05\x12\x12\n\nautoRemove\x18\x08 \x01(\x08\x12\r\n\x05reuse\x18\t \x01(\x08\x12\x63\n\x0b\x66\x65Selection\x18\n \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureSelectionSpec\x12Z\n\tearlyStop\x18\x0c \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EarlyStopSpec\"\x80\x01\n\x1e\x46\x65\x61tureEngineeringSearchStatus\x12^\n\x04\x62\x65st\x18\x01 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\"\xf7\x01\n\x16\x46\x65\x61tureEngineeringSpec\x12g\n\tpipelines\x18\x01 \x03(\x0b\x32T.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringPipeline\x12\x11\n\timbalance\x18\x02 \x01(\t\x12\x61\n\tselection\x18\x03 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureSelectionSpec\"8\n\x11\x46\x65\x61tureImportance\x12\x0f\n\x07\x66\x65\x61ture\x18\x01 \x01(\t\x12\x12\n\nimportance\x18\x02 \x01(\x01\":\n\x0b\x46\x65\x61tureInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\x01\"#\n\x0b\x46\x65\x61turePair\x12\t\n\x01x\x18\x01 \x01(\t\x12\t\n\x01y\x18\x02 \x01(\t\"\xd5\x01\n\x14\x46\x65\x61tureSelectionSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tembedding\x18\x03 \x01(\x08\x12\x0e\n\x06\x66ilter\x18\x04 \x01(\x08\x12\x0f\n\x07wrapper\x18\x05 \x01(\x08\x12\x10\n\x08pipeline\x18\x06 \x03(\t\x12\x14\n\x0cvarThreshold\x18\x07 \x01(\x05\x12\x15\n\rcorrThreshold\x18\x08 \x01(\x05\x12\x13\n\x0bmaxFeatures\x18\t \x01(\x05\x12\x12\n\npercentile\x18\n \x01(\x05\x12\x10\n\x08reserved\x18\x0c \x03(\t\"\xf8\x07\n\x0e\x46orecasterSpec\x12Y\n\x06\x65vents\x18\x02 \x03(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TimeSeriesEvent\x12R\n\x04past\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\x12T\n\x06\x66uture\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\x12\x10\n\x08\x66orecast\x18\x05 \x01(\x08\x12\x10\n\x08\x63overage\x18\x06 \x01(\x01\x12]\n\x0eoutputLocation\x18\x07 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x10\n\x08\x66\x65\x61tures\x18\x08 \x03(\t\x12\x0e\n\x06groups\x18\t \x03(\t\x12\x1a\n\x12predefinedTemplate\x18\n \x01(\t\x12T\n\tanomalies\x18\x0b \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Anomaly\x12\x14\n\x0ctrainEndData\x18\x0c \x01(\t\x12\x13\n\x0bvalueColumn\x18\r \x01(\t\x12\x11\n\thpoBudget\x18\x0e \x01(\x05\x12`\n\x11\x65valuationMetrics\x18\x0f \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EvalMetrics\x12^\n\x10\x65valuationPeriod\x18\x10 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EvalPeriod\x12^\n\x0bseasonality\x18\x11 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalitySpec\x12\x12\n\nregressors\x18\x12 \x03(\t\x12\x18\n\x10laggedRegressors\x18\x13 \x03(\t\x12\x0e\n\x06growth\x18\x14 \x01(\t\x12\x0b\n\x03key\x18\x15 \x03(\t\x12\x12\n\nestimators\x18\x16 \x03(\t\x12\x0b\n\x03hts\x18\x17 \x01(\t\"x\n\x15GarbageCollectionSpec\x12\x1e\n\x16\x63ollectAtModelClassEnd\x18\x01 \x01(\x08\x12%\n\x1dkeepOnlyBestModelPerAlgorithm\x18\x02 \x01(\x08\x12\x18\n\x10keepPrunedModels\x18\x03 \x01(\x08\"\x8e\x01\n\x17GarbageCollectionStatus\x12\x1c\n\x14\x63ollectedModelsCount\x18\x01 \x01(\x05\x12U\n\x06models\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelResult\"f\n\x13GeneratedColumnSpec\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\r\n\x05\x66irst\x18\x03 \x01(\t\x12\x0e\n\x06second\x18\x04 \x01(\t\x12\x10\n\x08original\x18\x05 \x01(\t\"V\n\x17GroupSplitLocationsSpec\x12\x1d\n\x15groupTrainingDataFile\x18\x01 \x01(\t\x12\x1c\n\x14groupTestingDataFile\x18\x02 \x01(\t\"2\n\x13HyperParameterValue\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"o\n\x10HyperbandOptions\x12\x14\n\x0cminResources\x18\x01 \x01(\x05\x12\x14\n\x0cmaxResources\x18\x02 \x01(\x05\x12\x17\n\x0freductionFactor\x18\x03 \x01(\x05\x12\x16\n\x0e\x62ootstrapCount\x18\x04 \x01(\x05\"\'\n\x11ImagePipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\";\n\x15ImbalanceHandlingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\timbalance\x18\x02 \x01(\t\"\x9a\x02\n\x14InterpretabilitySpec\x12\x0b\n\x03ice\x18\x01 \x01(\x08\x12W\n\x08icepairs\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeaturePair\x12\x0c\n\x04lime\x18\x03 \x01(\x08\x12\x0c\n\x04shap\x18\x04 \x01(\t\x12X\n\tshappairs\x18\x05 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeaturePair\x12\x16\n\x0e\x63ounterfactual\x18\x06 \x01(\x08\x12\x0e\n\x06\x61nchor\x18\x07 \x01(\x08\"\xc6\x02\n\x16InterpretabilityStatus\x12=\n\tstartedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x14\n\x0c\x65xplainerURI\x18\x03 \x01(\t\x12\x1a\n\x12trainShapValuesURI\x18\x04 \x01(\t\x12\x19\n\x11testShapValuesURI\x18\x05 \x01(\t\x12_\n\nimportance\x18\x06 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\"V\n\x05Level\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05index\x18\x02 \x03(\t\x12\x0f\n\x07horizon\x18\x03 \x01(\x05\x12\x0c\n\x04\x66req\x18\x04 \x01(\t\x12\x11\n\taggregate\x18\x05 \x01(\t\"k\n\x13MedianPrunerOptions\x12\x15\n\rstartupTrials\x18\x01 \x01(\x05\x12\x13\n\x0bwarmupSteps\x18\x02 \x01(\x05\x12\x15\n\rintervalSteps\x18\x03 \x01(\x05\x12\x11\n\tminTrials\x18\x04 \x01(\x05\"\xf5\x01\n\x05Model\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelSpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelStatus\"\x84\x02\n\nModelClass\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassSpec\x12Z\n\x06status\x18\x03 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassStatus\"\xcd\x04\n\x12ModelClassDataSpec\x12[\n\x0cobservations\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12Z\n\x0bpredictions\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12L\n\x06schema\x18\x03 \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Schema\x12Z\n\x08\x66latFile\x18\x04 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\x12\x12\n\nprimaryKey\x18\x05 \x03(\t\x12\x1c\n\x14predictionTimeColumn\x18\x06 \x01(\t\x12\x0e\n\x06target\x18\x07 \x01(\t\x12Q\n\x05tests\x18\x08 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12\x1e\n\x16onlineFeatureStoreName\x18\t \x01(\t\x12\x1f\n\x17offlineFeatureStoreName\x18\n \x01(\t\"\xa7\x01\n\x0eModelClassList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\"\x8d\x02\n\rModelClassRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Y\n\x04spec\x18\x02 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRunSpec\x12]\n\x06status\x18\x03 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRunStatus\"\xad\x01\n\x11ModelClassRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12V\n\x05items\x18\x02 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\"\xce\x01\n\x11ModelClassRunSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x61tasetName\x18\x03 \x01(\t\x12\x16\n\x0emodelClassName\x18\x04 \x01(\t\x12\r\n\x05owner\x18\x05 \x01(\t\x12\x10\n\x08priority\x18\x06 \x01(\t\x12\x0e\n\x06paused\x18\x07 \x01(\x08\x12\x0f\n\x07\x61\x62orted\x18\x08 \x01(\x08\x12\x0b\n\x03ttl\x18\t \x01(\x05\x12\x13\n\x0btriggeredBy\x18\n \x01(\t\"\xed\x04\n\x13ModelClassRunStatus\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\x11\n\tstudyName\x18\x02 \x01(\t\x12\x11\n\tmodelName\x18\x03 \x01(\t\x12?\n\x0b\x63ompletedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x06 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x07 \x01(\x03\x12\x13\n\x0b\x65valMetrics\x18\x08 \x01(\t\x12\x15\n\rfailureReason\x18\t \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\n \x01(\t\x12=\n\tupdatedAt\x18\x0c \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12K\n\x04logs\x18\r \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12>\n\npromotedAt\x18\x0e \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0c\n\x04\x61uto\x18\x0f \x01(\x08\x12\x37\n\napprovedBy\x18\x10 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0bmodelsCount\x18\x11 \x01(\x05\x12\x43\n\nconditions\x18\x12 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xd5\x02\n\x15ModelClassServingSpec\x12W\n\x08template\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingSpec\x12`\n\x12monitoringSchedule\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12`\n\x12predictionSchedule\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\x0e\n\x06preSQL\x18\x04 \x03(\t\x12\x0f\n\x07postSQL\x18\x05 \x03(\t\"\xc9\x06\n\x0eModelClassSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0c\n\x04task\x18\x04 \x01(\t\x12\x0f\n\x07subtask\x18\x05 \x01(\t\x12Y\n\tobjective\x18\x06 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12U\n\x08\x65ntities\x18\x07 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EntityRef\x12Z\n\x04\x64\x61ta\x18\x08 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassDataSpec\x12\x62\n\x08training\x18\t \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassTrainingSpec\x12`\n\x07serving\x18\n \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassServingSpec\x12_\n\x0cnotification\x18\x0b \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\\\n\x0ereportSchedule\x18\x0c \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\x0c\n\x04\x66\x61st\x18\r \x01(\x08\x12\x0e\n\x06paused\x18\x0e \x01(\x08\x12\x12\n\nregistered\x18\x0f \x01(\x08\x12\x1a\n\x12\x61rtifactBucketName\x18\x10 \x01(\t\"\xfb\x08\n\x10ModelClassStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12`\n\x06\x62\x65stFE\x18\x03 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12j\n\x16trainingScheduleStatus\x18\x04 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12k\n\x17predictionSceduleStatus\x18\x05 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12k\n\x17monitoringSceduleStatus\x18\x06 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12g\n\x13reportSceduleStatus\x18\x07 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12\x16\n\x0e\x62\x65stModelScore\x18\x08 \x01(\x01\x12\x0f\n\x07retired\x18\t \x03(\t\x12\x15\n\rpredictorName\x18\n \x01(\t\x12\x13\n\x0b\x64\x61taAppName\x18\x0b \x01(\t\x12\x13\n\x0btriggeredBy\x18\x0c \x01(\t\x12\x15\n\rfailureReason\x18\r \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x0e \x01(\t\x12=\n\tlastRunAt\x18\x0f \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x13\n\x0blastRunName\x18\x10 \x01(\t\x12\x44\n\x10lastPredictionAt\x18\x11 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12lastPredictionName\x18\x12 \x01(\t\x12\x18\n\x10predictionsCount\x18\x13 \x01(\x05\x12\x11\n\trunsCount\x18\x14 \x01(\x05\x12\x13\n\x0bmodelsCount\x18\x15 \x01(\x05\x12\x0c\n\x04live\x18\x16 \x01(\x08\x12\x17\n\x0fpredictorsCount\x18\x17 \x01(\x05\x12\x43\n\nconditions\x18\x18 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xe5\x05\n\x16ModelClassTrainingSpec\x12\x33\n\x06labRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x19\n\x11studyTemplateName\x18\x02 \x01(\t\x12Z\n\x0emodelUnitTests\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12^\n\x10trainingSchedule\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\\\n\nmodelImage\x18\x05 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelImageSpec\x12g\n\x0bsearchSpace\x18\x08 \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AlgorithmSearchSpaceSpec\x12X\n\tresources\x18\t \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x13\n\x0btriggeredBy\x18\n \x01(\t\x12\x0e\n\x06paused\x18\x0b \x01(\x08\x12\x0f\n\x07maxTime\x18\x0c \x01(\x05\x12\x11\n\tmaxModels\x18\r \x01(\x05\x12\x10\n\x08trainers\x18\x0e \x01(\x05\x12\x0f\n\x07\x61\x62orted\x18\x0f \x01(\x08\x12\x11\n\texplained\x18\x10 \x01(\x08\x12\x0e\n\x06preSQL\x18\x11 \x03(\t\x12\x0f\n\x07postSQL\x18\x12 \x03(\t\"\xb3\x01\n\x12ModelGroupByStatus\x12\x11\n\tmodelsURI\x18\x01 \x01(\t\x12\x13\n\x0bprofilesURI\x18\x02 \x01(\t\x12\x14\n\x0c\x66orecastsURI\x18\x03 \x01(\t\x12_\n\rworkerResults\x18\x04 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"R\n\x0eModelImageSpec\x12\r\n\x05\x65xist\x18\x01 \x01(\x08\x12\x11\n\timageName\x18\x02 \x01(\t\x12\x1e\n\x16registryConnectionName\x18\x03 \x01(\t\"\x9d\x01\n\tModelList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"W\n\x0bModelResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03\x61lg\x18\x02 \x01(\t\x12\r\n\x05score\x18\x03 \x01(\x01\x12\r\n\x05\x65rror\x18\x04 \x01(\x08\x12\x0f\n\x07trialID\x18\x05 \x01(\x05\"\xd9\x11\n\tModelSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x14\n\x0cmodelVersion\x18\x04 \x01(\t\x12\x11\n\tstudyName\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x61tasetName\x18\x06 \x01(\t\x12\x0c\n\x04task\x18\x07 \x01(\t\x12\x0f\n\x07subtask\x18\x08 \x01(\t\x12Y\n\tobjective\x18\t \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12l\n\x12\x66\x65\x61tureEngineering\x18\n \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12\x63\n\testimator\x18\x0b \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12X\n\x03\x64nn\x18\x0c \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DeepEstimatorSpec\x12_\n\x07\x63hatbot\x18\r \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ChatbotEstimatorSpec\x12`\n\x0cnlpEstimator\x18\x0e \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.NLPEstimatorSpec\x12X\n\x08\x65nsemble\x18\x0f \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EnsembleSpec\x12X\n\x08training\x18\x10 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TrainingSpec\x12\x0e\n\x06tested\x18\x12 \x01(\x08\x12\x0f\n\x07\x61\x62orted\x18\x13 \x01(\x08\x12\x10\n\x08packaged\x18\x14 \x01(\x08\x12\x11\n\tpublished\x18\x15 \x01(\x08\x12\x0e\n\x06pushed\x18\x16 \x01(\x08\x12\x10\n\x08reported\x18\x17 \x01(\x08\x12\x0e\n\x06paused\x18\x18 \x01(\x08\x12\x10\n\x08profiled\x18\x19 \x01(\x08\x12\x10\n\x08\x61rchived\x18\x1a \x01(\x08\x12\x12\n\nforecasted\x18\x1b \x01(\x08\x12\x0f\n\x07predict\x18\x1e \x01(\x08\x12\r\n\x05tuned\x18\x1f \x01(\x08\x12\x11\n\texplained\x18  \x01(\x08\x12\x15\n\rcodeGenerated\x18! \x01(\x08\x12\x10\n\x08\x62\x61seline\x18\" \x01(\x08\x12\x18\n\x10genDriftDetector\x18# \x01(\x08\x12\x0c\n\x04\x66\x61st\x18$ \x01(\x08\x12\x12\n\nunitTested\x18% \x01(\x08\x12?\n\x12\x66\x65\x65\x64\x62\x61\x63kDatasetRef\x18& \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0f\n\x07\x66lagged\x18\' \x01(\x08\x12W\n\x08location\x18( \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12]\n\x0b\x66orecasting\x18) \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ForecasterSpec\x12Z\n\x0b\x63ompilation\x18* \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CompilerSpec\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18+ \x01(\x03\x12\x15\n\restimatorType\x18, \x01(\t\x12\x0b\n\x03ttl\x18- \x01(\x05\x12\x12\n\nmodelClass\x18. \x01(\t\x12\x0f\n\x07trialID\x18/ \x01(\x05\x12T\n\x08\x61pproval\x18\x30 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ApprovalSpec\x12h\n\x10interpretability\x18\x31 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilitySpec\x12U\n\tunitTests\x18\x32 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12Y\n\rfeedbackTests\x18\x33 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12q\n\x12partitionLocations\x18\x34 \x01(\x0b\x32U.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PartitionModelLocationsSpec\x12\x16\n\x0emodelClassName\x18\x35 \x01(\t\x12\x19\n\x11modelClassRunName\x18\x36 \x01(\t\x12\x0c\n\x04role\x18\x37 \x01(\t\x12\x10\n\x08released\x18\x38 \x01(\x08\"\x93\x02\n\x10ModelStageStatus\x12\r\n\x05phase\x18\x01 \x01(\t\x12=\n\tstartedAt\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x61\n\x0funitTestsResult\x18\t \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\r\n\x05\x65rror\x18\n \x01(\t\"\xd7\"\n\x0bModelStatus\x12\x45\n\x11trainingStartedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12G\n\x13trainingCompletedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x44\n\x10testingStartedAt\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x46\n\x12testingCompletedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\x0ftuningStartedAt\x18\x06 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x45\n\x11tuningCompletedAt\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0f\n\x07\x63vScore\x18\t \x01(\x01\x12\x15\n\rtrainingScore\x18\n \x01(\x01\x12\x11\n\ttestScore\x18\x0b \x01(\x01\x12\x0c\n\x04\x63ost\x18\x0c \x01(\x01\x12\x0c\n\x04\x62\x65st\x18\r \x01(\x08\x12P\n\x02\x63v\x18\x0e \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12S\n\x05train\x18\x0f \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12R\n\x04test\x18\x10 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12R\n\x04tune\x18\x11 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12V\n\x08\x66\x65\x65\x64\x62\x61\x63k\x18\x12 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12\x43\n\x16lastFeedbackDatasetRef\x18\x13 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\r\n\x05phase\x18\x14 \x01(\t\x12\x12\n\nreportName\x18\x15 \x01(\t\x12\x11\n\treportURI\x18\x16 \x01(\t\x12\x13\n\x0bmanifestURI\x18\x17 \x01(\t\x12\x17\n\x0ftrainWeightsURI\x18\x18 \x01(\t\x12\x16\n\x0etestWeightsURI\x18\x19 \x01(\t\x12\x16\n\x0e\x66ullWeightsURI\x18\x1a \x01(\t\x12\x18\n\x10\x64riftDetectorURI\x18\x1b \x01(\t\x12\x1c\n\x14trainLabelEncoderURI\x18\x1c \x01(\t\x12\x1b\n\x13testLabelEncoderURI\x18\x1d \x01(\t\x12\x1b\n\x13\x66ullLabelEncoderURI\x18\x1e \x01(\t\x12\x0f\n\x07logsURI\x18\x1f \x01(\t\x12\x12\n\nprofileURI\x18  \x01(\t\x12\x1c\n\x14misclassificationURI\x18! \x01(\t\x12\x0e\n\x06tarURI\x18\" \x01(\t\x12\x0e\n\x06\x61ppURI\x18# \x01(\t\x12\x11\n\timageName\x18$ \x01(\t\x12g\n\x12impurityImportance\x18% \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\x12j\n\x15permutationImportance\x18& \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\x12\x13\n\x0b\x66orecastURI\x18\' \x01(\t\x12X\n\x07runtime\x18( \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.RuntimeStatus\x12\x63\n\x14trainDatasetLocation\x18) \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13testDatasetLocation\x18* \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19validationDatasetLocation\x18+ \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x1a\n\x12observedGeneration\x18, \x01(\x03\x12\x14\n\x0ctrainingRows\x18- \x01(\x05\x12\x13\n\x0btestingRows\x18. \x01(\x05\x12\x16\n\x0evalidationRows\x18/ \x01(\x05\x12\x15\n\rfailureReason\x18\x30 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x31 \x01(\t\x12\x10\n\x08progress\x18\x32 \x01(\x05\x12\x13\n\x0bsizeInBytes\x18\x33 \x01(\x05\x12\x0f\n\x07latency\x18\x34 \x01(\x01\x12\x0b\n\x03url\x18\x35 \x01(\t\x12X\n\x07serving\x18\x36 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingStatus\x12>\n\nreleasedAt\x18\x37 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0bpredictedAt\x18\x38 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x13\n\x0btarFileHash\x18\x39 \x01(\t\x12\x11\n\timageHash\x18: \x01(\t\x12^\n\x10trainingDataHash\x18; \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataHashes\x12g\n\x11trainingResources\x18< \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x66\n\x10testingResources\x18= \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x11\n\ttrainedBy\x18> \x01(\t\x12\x0c\n\x04team\x18? \x01(\t\x12K\n\x04logs\x18\x41 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12V\n\x08rocCurve\x18\x42 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RocAucCurve\x12Q\n\x07prCurve\x18\x43 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PRCurve\x12\x66\n\x14trainConfusionMatrix\x18\x44 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrix\x12\x65\n\x13testConfusionMatrix\x18\x45 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrix\x12\x61\n\x16\x63orrelationsWithTarget\x18\x46 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\x12Z\n\x0ftopCorrelations\x18G \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\x12=\n\tupdatedAt\x18H \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12V\n\x08\x61pproval\x18I \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ApprovalStatus\x12j\n\x10interpretability\x18J \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilityStatus\x12O\n\x06images\x18K \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Images\x12\x61\n\x0funitTestsResult\x18L \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\x65\n\x13\x66\x65\x65\x64\x62\x61\x63kTestsResult\x18M \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12]\n\x07groupby\x18N \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelGroupByStatus\x12Z\n\x06stages\x18O \x03(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelStageStatus\x12[\n\x05usage\x18P \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x43\n\nconditions\x18Q \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xdf\x01\n\x0eModelTestSuite\x12=\n\x10\x62\x61selineModelRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x37\n\ndatasetRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12U\n\tunitTests\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\" \n\x10NLPEstimatorSpec\x12\x0c\n\x04\x62\x61se\x18\x01 \x01(\t\"/\n\x10NNLayerParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\xcc\x01\n\x1bPartitionModelLocationsSpec\x12\x17\n\x0fpartitionFolder\x18\x01 \x01(\t\x12\x1e\n\x16partitionProfileFolder\x18\x02 \x01(\t\x12\x1b\n\x13partitionReportFile\x18\x03 \x01(\t\x12\x1c\n\x14partitionModelFolder\x18\x04 \x01(\t\x12\x1a\n\x12partitionModelFile\x18\x05 \x01(\t\x12\x1d\n\x15partitionForecastFile\x18\x06 \x01(\t\"\x84\x01\n\x17PercentilePrunerOptions\x12\x12\n\npercentile\x18\x01 \x01(\x05\x12\x15\n\rstartupTrials\x18\x02 \x01(\x05\x12\x13\n\x0bwarmupSteps\x18\x03 \x01(\x05\x12\x16\n\x0eintervalTrials\x18\x04 \x01(\x05\x12\x11\n\tminTrials\x18\x05 \x01(\x05\"\x93\x04\n\nPrunerSpec\x12\x0c\n\x04type\x18\x01 \x01(\t\x12]\n\x06median\x18\x02 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.MedianPrunerOptions\x12\x65\n\npercentile\x18\x03 \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PercentilePrunerOptions\x12m\n\x11successiveHalving\x18\x04 \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SuccessiveHalvingOptions\x12]\n\thyperband\x18\x05 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.HyperbandOptions\x12\x63\n\tthreshold\x18\x06 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ThresholdPrunerOptions\"\xd0\x01\n\x18RegressionForecasterSpec\x12\x10\n\x08\x65nsemble\x18\x01 \x01(\x08\x12\x12\n\nimputation\x18\x02 \x01(\t\x12\x10\n\x08\x65ncoding\x18\x03 \x01(\t\x12\x0f\n\x07scaling\x18\x04 \x01(\t\x12\x0c\n\x04\x64\x61te\x18\x05 \x01(\x08\x12\x0f\n\x07windows\x18\x06 \x03(\x05\x12\x0c\n\x04lags\x18\x07 \x03(\x05\x12\x11\n\tfunctions\x18\x08 \x03(\t\x12\x0b\n\x03\x65ma\x18\t \x01(\x08\x12\x0b\n\x03log\x18\n \x01(\x08\x12\x11\n\treduction\x18\x0b \x01(\t\"\xf8\x01\n\x06Report\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12R\n\x04spec\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportSpec\x12V\n\x06status\x18\x03 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportStatus\"\x8a\x01\n\x13ReportGroupByStatus\x12\x12\n\nreportsURI\x18\x01 \x01(\t\x12_\n\rworkerResults\x18\x04 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"\x9f\x01\n\nReportList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12O\n\x05items\x18\x02 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\x9e\x03\n\nReportSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x36\n\tentityRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x12\n\nreportType\x18\x03 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x04 \x01(\t\x12\x14\n\x0cnotifierName\x18\x05 \x01(\t\x12\r\n\x05owner\x18\x06 \x01(\t\x12X\n\tresources\x18\x07 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0f\n\x07timeout\x18\x08 \x01(\x03\x12\x33\n\x06labRef\x18\t \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0b\n\x03key\x18\n \x03(\t\x12\x1a\n\x12\x61rtifactBucketName\x18\x0b \x01(\t\x12\x16\n\x0emodelClassName\x18\x0c \x01(\t\x12\x19\n\x11modelClassRunName\x18\r \x01(\t\"\xb3\x04\n\x0cReportStatus\x12?\n\x0b\x63ompletedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x02 \x01(\t\x12W\n\x08location\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\x12K\n\x04logs\x18\x07 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12=\n\tupdatedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12^\n\x07groupby\x18\t \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportGroupByStatus\x12\x43\n\nconditions\x18\n \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xf1\x01\n\rRuntimeStatus\x12\x15\n\rpythonVersion\x18\x01 \x01(\t\x12\x11\n\tpythonCmd\x18\x02 \x01(\t\x12\n\n\x02os\x18\x03 \x01(\t\x12s\n\x0epythonPackages\x18\x04 \x03(\x0b\x32[.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.RuntimeStatus.PythonPackagesEntry\x1a\x35\n\x13PythonPackagesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x9e\x05\n\nSearchSpec\x12\x0f\n\x07sampler\x18\x01 \x01(\t\x12T\n\x06pruner\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PrunerSpec\x12\x0f\n\x07maxCost\x18\x03 \x01(\x05\x12\x0f\n\x07maxTime\x18\x04 \x01(\x05\x12\x11\n\tmaxModels\x18\x05 \x01(\x05\x12\x14\n\x0cminBestScore\x18\x06 \x01(\x01\x12\x10\n\x08trainers\x18\x07 \x01(\x05\x12\x0c\n\x04test\x18\x08 \x01(\x05\x12\x11\n\tretainTop\x18\t \x01(\x05\x12\x13\n\x0bretainedFor\x18\n \x01(\x05\x12g\n\x0bsearchSpace\x18\x0b \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AlgorithmSearchSpaceSpec\x12Z\n\tearlyStop\x18\x0c \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EarlyStopSpec\x12Y\n\tobjective\x18\x0e \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12Z\n\nobjective2\x18\x0f \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12\x0c\n\x04tune\x18\x10 \x01(\x08\x12\x0c\n\x04goal\x18\x11 \x01(\t\"L\n\x15SeasonalityPeriodSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04\x61uto\x18\x02 \x01(\x08\x12\x14\n\x0c\x66ourierOrder\x18\x03 \x01(\x05\"\x87\x04\n\x0fSeasonalitySpec\x12\x0c\n\x04\x61uto\x18\x01 \x01(\x08\x12_\n\x06yearly\x18\x02 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12\x62\n\tquarterly\x18\x03 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12`\n\x07monthly\x18\x04 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12_\n\x06weekly\x18\x05 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12^\n\x05\x64\x61ily\x18\x06 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\"<\n\x0bSegmentSpec\x12\x12\n\ncolumnName\x18\x01 \x01(\t\x12\n\n\x02op\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\"\xb7\x03\n\x12ServingEnvironment\x12\x0c\n\x04name\x18\x01 \x01(\t\x12Q\n\x05tests\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12;\n\x0eservingSiteRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12S\n\x06\x61\x63\x63\x65ss\x18\x04 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\x05 \x01(\x05\x12\x0e\n\x06online\x18\x06 \x01(\x08\x12\x11\n\tdashboard\x18\x07 \x01(\x08\x12X\n\tresources\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0e\n\x06preSQL\x18\t \x03(\t\x12\x0f\n\x07postSQL\x18\n \x03(\t\"\xe2\x03\n\x0bServingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x15\n\rpredictorName\x18\x02 \x01(\t\x12X\n\tresources\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12;\n\x0eservingSiteRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0e\n\x06online\x18\x07 \x01(\x08\x12\x11\n\tdashboard\x18\x08 \x01(\x08\x12S\n\x06\x61\x63\x63\x65ss\x18\t \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\n \x01(\x05\x12\x11\n\tpromotion\x18\x0c \x01(\t\x12\x37\n\napprovedBy\x18\r \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12>\n\napprovedAt\x18\x0e \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"g\n\rServingStatus\x12\x15\n\rpredictorName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x61taAppName\x18\x03 \x01(\t\x12\x14\n\x0cpredictorURI\x18\x04 \x01(\t\x12\x14\n\x0c\x64\x61shboardURI\x18\x05 \x01(\t\"\xf5\x01\n\x05Study\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudySpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyStatus\"\x89\x01\n\x12StudyGroupByStatus\x12\x12\n\nstudiesURI\x18\x01 \x01(\t\x12_\n\rworkerResults\x18\x02 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"\x9d\x01\n\tStudyList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\"\xb4\x02\n\x10StudyPhaseStatus\x12=\n\tstartedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12waitingModelsCount\x18\x03 \x01(\x05\x12\x1a\n\x12runningModelsCount\x18\x04 \x01(\x05\x12\x19\n\x11\x66\x61iledModelsCount\x18\x05 \x01(\x05\x12\x1c\n\x14\x63ompletedModelsCount\x18\x06 \x01(\x05\x12\x11\n\tbestScore\x18\x07 \x01(\x01\x12\x1c\n\x14modelsWithNoProgress\x18\x08 \x01(\x05\"a\n\x11StudyScheduleSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12;\n\x07startAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"\xee\x10\n\tStudySpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x33\n\x06labRef\x18\x05 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0b\x64\x61tasetName\x18\x06 \x01(\t\x12\x0c\n\x04task\x18\x07 \x01(\t\x12\x0f\n\x07subtask\x18\x08 \x01(\t\x12h\n\x08\x66\x65Search\x18\t \x01(\x0b\x32V.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSearchSpec\x12i\n\x10imbalanceHandler\x18\n \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ImbalanceHandlingSpec\x12X\n\x08\x62\x61seline\x18\x0b \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.BaselineSpec\x12T\n\x06search\x18\x0c \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SearchSpec\x12Z\n\tensembles\x18\r \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EnsemblesSpec\x12`\n\x10trainingTemplate\x18\x0e \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TrainingSpec\x12]\n\x0b\x66\x63tTemplate\x18\x10 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ForecasterSpec\x12]\n\x08schedule\x18\x11 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyScheduleSpec\x12h\n\x10interpretability\x18\x12 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilitySpec\x12`\n\x0e\x64riftDetection\x18\x13 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DriftModelSpec\x12\x0f\n\x07\x61\x62orted\x18\x14 \x01(\x08\x12\x10\n\x08reported\x18\x15 \x01(\x08\x12\x0e\n\x06paused\x18\x16 \x01(\x08\x12\x10\n\x08profiled\x18\x17 \x01(\x08\x12\x16\n\x0emodelPublished\x18\x18 \x01(\x08\x12\x18\n\x10modelImagePushed\x18\x19 \x01(\x08\x12\x16\n\x0emodelExplained\x18\x1a \x01(\x08\x12\x0c\n\x04\x66\x61st\x18\x1b \x01(\x08\x12\x1a\n\x12\x61rtifactBucketName\x18\x1c \x01(\t\x12\r\n\x05owner\x18\x1d \x01(\t\x12Z\n\x0b\x63ompilation\x18\x1e \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CompilerSpec\x12\x10\n\x08template\x18\x1f \x01(\x08\x12\x0f\n\x07\x66lagged\x18  \x01(\x08\x12_\n\x0cnotification\x18! \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\\\n\nmodelImage\x18\" \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelImageSpec\x12[\n\x02gc\x18# \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GarbageCollectionSpec\x12\x0b\n\x03ttl\x18$ \x01(\x05\x12\x14\n\x0cmodelVersion\x18% \x01(\t\x12\x0f\n\x07timeout\x18& \x01(\x05\x12\x15\n\rcodeGenerated\x18\' \x01(\x08\x12]\n\x11unitTestsTemplate\x18( \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12i\n\x0egroupLocations\x18) \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GroupSplitLocationsSpec\x12\x16\n\x0emodelClassName\x18* \x01(\t\x12\x19\n\x11modelClassRunName\x18+ \x01(\t\x12V\n\x07serving\x18, \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingSpec\"\xb0\x10\n\x0bStudyStatus\x12\x13\n\x0bmodelsCount\x18\x01 \x01(\x05\x12?\n\x0b\x63ompletedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x11\n\tbestModel\x18\x04 \x01(\t\x12\x16\n\x0e\x62\x65stModelScore\x18\x05 \x01(\x01\x12\x12\n\nprofileURI\x18\x06 \x01(\t\x12\x11\n\treportURI\x18\x07 \x01(\t\x12\x12\n\nreportName\x18\x08 \x01(\t\x12\r\n\x05phase\x18\t \x01(\t\x12\x1a\n\x12observedGeneration\x18\n \x01(\x03\x12\x63\n\x14trainDatasetLocation\x18\x0b \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13testDatasetLocation\x18\x0c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19validationDatasetLocation\x18\r \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x13\n\x0blastModelID\x18\x0e \x01(\x03\x12\x15\n\rfailureReason\x18\x0f \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x10 \x01(\t\x12\x19\n\x11trainingRowsCount\x18\x11 \x01(\x05\x12\x18\n\x10testingRowsCount\x18\x12 \x01(\x05\x12\x1b\n\x13validationRowsCount\x18\x13 \x01(\x05\x12\x10\n\x08progress\x18\x14 \x01(\x05\x12^\n\x10trainingDataHash\x18\x16 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataHashes\x12\x13\n\x0btriggeredBy\x18\x17 \x01(\t\x12K\n\x04logs\x18\x18 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12\x66\n\x12\x66\x65\x61tureEngineering\x18\x19 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\\\n\x08\x62\x61seline\x18\x1a \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12Z\n\x06search\x18\x1b \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\\\n\x08\x65nsemble\x18\x1c \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12X\n\x04test\x18\x1d \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12[\n\x07\x65xplain\x18\x1e \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\x65\n\x0e\x64riftDetection\x18\x1f \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DriftDetectorStatus\x12=\n\tupdatedAt\x18  \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12`\n\x06\x62\x65stFE\x18! \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12]\n\x02gc\x18\" \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GarbageCollectionStatus\x12]\n\x07groupby\x18# \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyGroupByStatus\x12[\n\x05usage\x18$ \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x43\n\nconditions\x18% \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x7f\n\x18SuccessiveHalvingOptions\x12\x14\n\x0cminResources\x18\x01 \x01(\x05\x12\x17\n\x0freductionFactor\x18\x02 \x01(\x05\x12\x1c\n\x14minEarlyStoppingRate\x18\x03 \x01(\x05\x12\x16\n\x0e\x62ootstrapCount\x18\x04 \x01(\x05\"h\n\x15SuccessiveHalvingSpec\x12\x0e\n\x06\x62udget\x18\x01 \x01(\x05\x12\x0f\n\x07\x62racket\x18\x02 \x01(\x05\x12\x0c\n\x04rung\x18\x03 \x01(\x05\x12\x0e\n\x06\x63onfID\x18\x04 \x01(\x05\x12\x10\n\x08modality\x18\x1a \x01(\t\"\xad\x01\n\x10TextPipelineSpec\x12\x0f\n\x07\x65ncoder\x18\x01 \x01(\t\x12\x11\n\ttokenizer\x18\x02 \x01(\t\x12\x11\n\tstopwords\x18\x03 \x01(\x08\x12\x0b\n\x03pos\x18\x04 \x01(\x08\x12\r\n\x05lemma\x18\x05 \x01(\x08\x12\x0c\n\x04stem\x18\x06 \x01(\x08\x12\x11\n\tembedding\x18\x07 \x01(\t\x12\x0b\n\x03svd\x18\x08 \x01(\x08\x12\x18\n\x10maxSvdComponents\x18\t \x01(\x05\"b\n\x16ThresholdPrunerOptions\x12\r\n\x05lower\x18\x01 \x01(\x01\x12\r\n\x05upper\x18\x02 \x01(\x01\x12\x13\n\x0bwarmupSteps\x18\x03 \x01(\x05\x12\x15\n\rintervalSteps\x18\x04 \x01(\x05\"\x8a\x01\n\x0fTimeSeriesEvent\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06method\x18\x02 \x01(\t\x12\x0f\n\x07holiday\x18\x03 \x01(\x08\x12\x0f\n\x07\x63ountry\x18\x04 \x01(\t\x12\x10\n\x08preEvent\x18\x05 \x01(\x05\x12\x11\n\tpostEvent\x18\x06 \x01(\x05\x12\x12\n\ntimePoints\x18\x07 \x03(\t\"\x9c\x05\n\x0cTrainingSpec\x12\x33\n\x06labRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08priority\x18\x02 \x01(\t\x12\x0e\n\x06\x63vtype\x18\x03 \x01(\t\x12\n\n\x02\x63V\x18\x04 \x01(\x08\x12\r\n\x05\x66olds\x18\x05 \x01(\x05\x12V\n\x05split\x18\x06 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataSplitSpec\x12\x13\n\x0b\x65valMetrics\x18\x07 \x03(\t\x12[\n\x02sh\x18\n \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SuccessiveHalvingSpec\x12\x0c\n\x04seed\x18\x0b \x01(\x01\x12X\n\tresources\x18\x0c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0b\n\x03gpu\x18\r \x01(\x08\x12\x13\n\x0b\x64istributed\x18\x0e \x01(\x08\x12\x19\n\x11\x66\x65\x61tureImportance\x18\x0f \x01(\x08\x12\x11\n\tnodeCount\x18\x10 \x01(\x05\x12\x11\n\tsamplePct\x18\x11 \x01(\x05\x12\\\n\ncheckpoint\x18\x12 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.CheckpointSpec\x12\x10\n\x08logLevel\x18\x13 \x01(\t\x12\x15\n\rtimeoutInSecs\x18\x14 \x01(\x05\"\xdc\x01\n\x18UnivariateForecastStatus\x12\x1b\n\x13gridSearchResultURI\x18\x01 \x01(\t\x12g\n\rbaseEstimator\x18\x02 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12\x10\n\x08modelURI\x18\x03 \x01(\t\x12\x13\n\x0b\x63vResultURI\x18\x04 \x01(\t\x12\x13\n\x0b\x66orecastURI\x18\x05 \x01(\t\"\'\n\x11VideoPipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\"=\n\nWindowSpec\x12\x10\n\x08interval\x18\x01 \x01(\t\x12\r\n\x05start\x18\x02 \x01(\x05\x12\x0e\n\x06length\x18\x03 \x01(\x05\x42:Z8github.com/metaprov/modelaapi/pkg/apis/training/v1alpha1')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nHgithub.com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated.proto\x12\x38github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\x80\x01\n\x17\x41lgorithmParameterRange\x12\x0c\n\x04name\x18\x01 \x01(\t\x12W\n\x06ranges\x18\x02 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ParameterRange\"\x9f\x01\n\x18\x41lgorithmSearchSpaceSpec\x12\x0f\n\x07include\x18\x01 \x03(\t\x12\x0f\n\x07\x65xclude\x18\x02 \x03(\t\x12\x61\n\x06\x63ustom\x18\x03 \x03(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AlgorithmParameterRange\"`\n\x07\x41nomaly\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0bvalueColumn\x18\x02 \x01(\t\x12\x16\n\x0e\x61\x64jDeltaColumn\x18\x03 \x01(\t\x12\r\n\x05start\x18\x04 \x01(\t\x12\x0b\n\x03\x65nd\x18\x05 \x01(\t\"\'\n\x11\x41udioPipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\"M\n\x0c\x42\x61\x63ktestSpec\x12\x0f\n\x07sliding\x18\x01 \x01(\x08\x12\x0e\n\x06splits\x18\x02 \x01(\x05\x12\x0f\n\x07Initial\x18\x03 \x01(\x05\x12\x0b\n\x03gap\x18\x05 \x01(\x05\"?\n\x0c\x42\x61selineSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tbaselines\x18\x02 \x03(\t\x12\x0b\n\x03\x61ll\x18\x03 \x01(\x08\"\r\n\x0b\x43hangePoint\"\x96\x01\n\x0e\x43heckpointSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1a\n\x12\x63heckpointInterval\x18\x02 \x01(\x05\x12W\n\x08location\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\x92\x01\n\x16\x43lassicalEstimatorSpec\x12\x15\n\ralgorithmName\x18\x01 \x01(\t\x12\x61\n\nparameters\x18\x02 \x03(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.HyperParameterValue\"a\n\x10\x43ustomReportSpec\x12M\n\x05pages\x18\x08 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.PageSpec\"L\n\nDataHashes\x12\x11\n\ttrainHash\x18\x01 \x01(\t\x12\x13\n\x0btestingHash\x18\x02 \x01(\t\x12\x16\n\x0evalidationHash\x18\x03 \x01(\t\"\xab\x01\n\rDataSplitSpec\x12\x0e\n\x06method\x18\x01 \x01(\t\x12\r\n\x05train\x18\x02 \x01(\x05\x12\x12\n\nvalidation\x18\x03 \x01(\x05\x12\x0c\n\x04test\x18\x04 \x01(\x05\x12\x13\n\x0bsplitColumn\x18\x05 \x01(\t\x12\x14\n\x0ctrainDataset\x18\x07 \x01(\t\x12\x13\n\x0btestDataset\x18\x08 \x01(\t\x12\x19\n\x11validationDataset\x18\t \x01(\t\"\xa5\x01\n\x12\x44\x65\x65pEstimatorLayer\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12^\n\nparameters\x18\x03 \x03(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.NNLayerParameter\x12\x13\n\x0binputLayers\x18\x04 \x03(\t\"\xe6\x01\n\x11\x44\x65\x65pEstimatorSpec\x12\\\n\x06layers\x18\x01 \x03(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DeepEstimatorLayer\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x11\n\tbatchSize\x18\x03 \x01(\x05\x12\x0e\n\x06\x65pochs\x18\x04 \x01(\x05\x12\x17\n\x0fvalidationSplit\x18\x05 \x01(\x05\x12\r\n\x05isSeq\x18\x06 \x01(\x08\x12\x0c\n\x04gpus\x18\x07 \x01(\x05\x12\x0c\n\x04loss\x18\x08 \x01(\t\".\n\x13\x44riftDetectorStatus\x12\x17\n\x0foutlierModelURI\x18\x01 \x01(\t\"O\n\rEarlyStopSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07initial\x18\x02 \x01(\x05\x12\x1c\n\x14modelsWithNoProgress\x18\x03 \x01(\x05\"\xfb\x01\n\x0c\x45nsembleSpec\x12\x0e\n\x06models\x18\x01 \x03(\t\x12\x64\n\nestimators\x18\x02 \x03(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12g\n\rbaseEstimator\x18\x03 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12\x0c\n\x04type\x18\x04 \x01(\t\"_\n\rEnsemblesSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x16\n\x0evotingEnsemble\x18\x02 \x01(\x08\x12\x18\n\x10stackingEnsemble\x18\x03 \x01(\x08\x12\x0b\n\x03top\x18\x04 \x01(\x05\"*\n\tEntityRef\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07\x65xclude\x18\x02 \x03(\t\"\x89\x01\n\x0b\x45valMetrics\x12\x11\n\tselection\x18\x01 \x01(\t\x12\x11\n\treporting\x18\x02 \x03(\t\x12\x0f\n\x07\x61ggFunc\x18\x03 \x01(\t\x12\x11\n\taggPeriod\x18\x04 \x01(\x05\x12\x17\n\x0fnullModelParams\x18\x05 \x01(\t\x12\x17\n\x0frelErrTolerance\x18\x06 \x01(\x01\"\xe0\x01\n\nEvalPeriod\x12\x13\n\x0btestHorizon\x18\x01 \x01(\x05\x12\x1f\n\x17periodsBetweenTrainTest\x18\x02 \x01(\x05\x12\x1e\n\x16\x63vPeriodsBetweenSplits\x18\x03 \x01(\x05\x12\x1a\n\x12\x63vExpandingWindows\x18\x04 \x01(\x08\x12\x11\n\tcvHorizon\x18\x05 \x01(\x05\x12\x19\n\x11\x63vMinTrainPeriods\x18\x06 \x01(\x05\x12\x13\n\x0b\x63vMaxSplits\x18\x07 \x01(\x05\x12\x1d\n\x15\x63vUseMostRecentSplits\x18\x08 \x01(\x08\"\xf2\x02\n\x1a\x46\x65\x61tureEngineeringPipeline\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x03 \x03(\t\x12\x12\n\nimputation\x18\x04 \x01(\t\x12\x10\n\x08\x65ncoding\x18\x05 \x01(\t\x12\x0f\n\x07scaling\x18\x06 \x01(\t\x12\x16\n\x0e\x64iscretisation\x18\x07 \x01(\t\x12\x1e\n\x16variableTransformation\x18\x08 \x01(\t\x12\x17\n\x0foutlierHandling\x18\t \x01(\t\x12\x1e\n\x16\x64\x61tetimeTransformation\x18\n \x01(\t\x12X\n\x04text\x18\x0b \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TextPipelineSpec\x12\x0c\n\x04\x64rop\x18\x0c \x01(\x08\x12\x13\n\x0bpassthrough\x18\r \x01(\x08\"\xcd\x02\n\x1c\x46\x65\x61tureEngineeringSearchSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\testimator\x18\x03 \x01(\t\x12\x11\n\tmaxModels\x18\x04 \x01(\x05\x12\x0f\n\x07maxTime\x18\x05 \x01(\x05\x12\x10\n\x08trainers\x18\x06 \x01(\x05\x12\r\n\x05reuse\x18\t \x01(\x08\x12h\n\x10\x66\x65\x61tureSelection\x18\n \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureSelectionSpec\x12Z\n\tearlyStop\x18\x0c \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EarlyStopSpec\"\x80\x01\n\x1e\x46\x65\x61tureEngineeringSearchStatus\x12^\n\x04\x62\x65st\x18\x01 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\"\xf7\x01\n\x16\x46\x65\x61tureEngineeringSpec\x12g\n\tpipelines\x18\x01 \x03(\x0b\x32T.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringPipeline\x12\x11\n\timbalance\x18\x02 \x01(\t\x12\x61\n\tselection\x18\x03 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureSelectionSpec\"8\n\x11\x46\x65\x61tureImportance\x12\x0f\n\x07\x66\x65\x61ture\x18\x01 \x01(\t\x12\x12\n\nimportance\x18\x02 \x01(\x01\":\n\x0b\x46\x65\x61tureInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\x01\"#\n\x0b\x46\x65\x61turePair\x12\t\n\x01x\x18\x01 \x01(\t\x12\t\n\x01y\x18\x02 \x01(\t\"\xd5\x01\n\x14\x46\x65\x61tureSelectionSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tembedding\x18\x03 \x01(\x08\x12\x0e\n\x06\x66ilter\x18\x04 \x01(\x08\x12\x0f\n\x07wrapper\x18\x05 \x01(\x08\x12\x10\n\x08pipeline\x18\x06 \x03(\t\x12\x14\n\x0cvarThreshold\x18\x07 \x01(\x05\x12\x15\n\rcorrThreshold\x18\x08 \x01(\x05\x12\x13\n\x0bmaxFeatures\x18\t \x01(\x05\x12\x12\n\npercentile\x18\n \x01(\x05\x12\x10\n\x08reserved\x18\x0c \x03(\t\"\xf8\x07\n\x0e\x46orecasterSpec\x12Y\n\x06\x65vents\x18\x02 \x03(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TimeSeriesEvent\x12R\n\x04past\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\x12T\n\x06\x66uture\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\x12\x10\n\x08\x66orecast\x18\x05 \x01(\x08\x12\x10\n\x08\x63overage\x18\x06 \x01(\x01\x12]\n\x0eoutputLocation\x18\x07 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x10\n\x08\x66\x65\x61tures\x18\x08 \x03(\t\x12\x0e\n\x06groups\x18\t \x03(\t\x12\x1a\n\x12predefinedTemplate\x18\n \x01(\t\x12T\n\tanomalies\x18\x0b \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Anomaly\x12\x14\n\x0ctrainEndData\x18\x0c \x01(\t\x12\x13\n\x0bvalueColumn\x18\r \x01(\t\x12\x11\n\thpoBudget\x18\x0e \x01(\x05\x12`\n\x11\x65valuationMetrics\x18\x0f \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EvalMetrics\x12^\n\x10\x65valuationPeriod\x18\x10 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EvalPeriod\x12^\n\x0bseasonality\x18\x11 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalitySpec\x12\x12\n\nregressors\x18\x12 \x03(\t\x12\x18\n\x10laggedRegressors\x18\x13 \x03(\t\x12\x0e\n\x06growth\x18\x14 \x01(\t\x12\x0b\n\x03key\x18\x15 \x03(\t\x12\x12\n\nestimators\x18\x16 \x03(\t\x12\x0b\n\x03hts\x18\x17 \x01(\t\"e\n\x15GarbageCollectionSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12!\n\x19keepBestModelPerAlgorithm\x18\x02 \x01(\x08\x12\x18\n\x10keepPrunedModels\x18\x03 \x01(\x08\"\x8e\x01\n\x17GarbageCollectionStatus\x12\x1c\n\x14\x63ollectedModelsCount\x18\x01 \x01(\x05\x12U\n\x06models\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelResult\"f\n\x13GeneratedColumnSpec\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\r\n\x05\x66irst\x18\x03 \x01(\t\x12\x0e\n\x06second\x18\x04 \x01(\t\x12\x10\n\x08original\x18\x05 \x01(\t\"V\n\x17GroupSplitLocationsSpec\x12\x1d\n\x15groupTrainingDataFile\x18\x01 \x01(\t\x12\x1c\n\x14groupTestingDataFile\x18\x02 \x01(\t\"2\n\x13HyperParameterValue\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"o\n\x10HyperbandOptions\x12\x14\n\x0cminResources\x18\x01 \x01(\x05\x12\x14\n\x0cmaxResources\x18\x02 \x01(\x05\x12\x17\n\x0freductionFactor\x18\x03 \x01(\x05\x12\x16\n\x0e\x62ootstrapCount\x18\x04 \x01(\x05\"\'\n\x11ImagePipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\";\n\x15ImbalanceHandlingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\timbalance\x18\x02 \x01(\t\"\x9a\x02\n\x14InterpretabilitySpec\x12\x0b\n\x03ice\x18\x01 \x01(\x08\x12W\n\x08icepairs\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeaturePair\x12\x0c\n\x04lime\x18\x03 \x01(\x08\x12\x0c\n\x04shap\x18\x04 \x01(\t\x12X\n\tshappairs\x18\x05 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeaturePair\x12\x16\n\x0e\x63ounterfactual\x18\x06 \x01(\x08\x12\x0e\n\x06\x61nchor\x18\x07 \x01(\x08\"\xaa\x04\n\x16InterpretabilityStatus\x12=\n\tstartedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12`\n\x11\x65xplainerLocation\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x66\n\x17trainShapValuesLocation\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x65\n\x16testShapValuesLocation\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12_\n\nimportance\x18\x06 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\"k\n\x13MedianPrunerOptions\x12\x15\n\rstartupTrials\x18\x01 \x01(\x05\x12\x13\n\x0bwarmupSteps\x18\x02 \x01(\x05\x12\x15\n\rintervalSteps\x18\x03 \x01(\x05\x12\x11\n\tminTrials\x18\x04 \x01(\x05\"\xf5\x01\n\x05Model\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelSpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelStatus\"\x84\x02\n\nModelClass\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassSpec\x12Z\n\x06status\x18\x03 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassStatus\"\xcd\x04\n\x12ModelClassDataSpec\x12[\n\x0cobservations\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12Z\n\x0bpredictions\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12L\n\x06schema\x18\x03 \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Schema\x12Z\n\x08\x66latFile\x18\x04 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\x12\x12\n\nprimaryKey\x18\x05 \x03(\t\x12\x1c\n\x14predictionTimeColumn\x18\x06 \x01(\t\x12\x0e\n\x06target\x18\x07 \x01(\t\x12Q\n\x05tests\x18\x08 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12\x1e\n\x16onlineFeatureStoreName\x18\t \x01(\t\x12\x1f\n\x17offlineFeatureStoreName\x18\n \x01(\t\"\xa7\x01\n\x0eModelClassList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\"\x8d\x02\n\rModelClassRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Y\n\x04spec\x18\x02 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRunSpec\x12]\n\x06status\x18\x03 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRunStatus\"\xad\x01\n\x11ModelClassRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12V\n\x05items\x18\x02 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\"\xce\x01\n\x11ModelClassRunSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x61tasetName\x18\x03 \x01(\t\x12\x16\n\x0emodelClassName\x18\x04 \x01(\t\x12\r\n\x05owner\x18\x05 \x01(\t\x12\x10\n\x08priority\x18\x06 \x01(\t\x12\x0e\n\x06paused\x18\x07 \x01(\x08\x12\x0f\n\x07\x61\x62orted\x18\x08 \x01(\x08\x12\x0b\n\x03ttl\x18\t \x01(\x05\x12\x13\n\x0btriggeredBy\x18\n \x01(\t\"\xed\x04\n\x13ModelClassRunStatus\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\x11\n\tstudyName\x18\x02 \x01(\t\x12\x11\n\tmodelName\x18\x03 \x01(\t\x12?\n\x0b\x63ompletedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x06 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x07 \x01(\x03\x12\x13\n\x0b\x65valMetrics\x18\x08 \x01(\t\x12\x15\n\rfailureReason\x18\t \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\n \x01(\t\x12=\n\tupdatedAt\x18\x0c \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12K\n\x04logs\x18\r \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12>\n\npromotedAt\x18\x0e \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0c\n\x04\x61uto\x18\x0f \x01(\x08\x12\x37\n\napprovedBy\x18\x10 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0bmodelsCount\x18\x11 \x01(\x05\x12\x43\n\nconditions\x18\x12 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xd5\x02\n\x15ModelClassServingSpec\x12W\n\x08template\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingSpec\x12`\n\x12monitoringSchedule\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12`\n\x12predictionSchedule\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\x0e\n\x06preSQL\x18\x04 \x03(\t\x12\x0f\n\x07postSQL\x18\x05 \x03(\t\"\xc9\x06\n\x0eModelClassSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0c\n\x04task\x18\x04 \x01(\t\x12\x0f\n\x07subtask\x18\x05 \x01(\t\x12Y\n\tobjective\x18\x06 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12U\n\x08\x65ntities\x18\x07 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EntityRef\x12Z\n\x04\x64\x61ta\x18\x08 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassDataSpec\x12\x62\n\x08training\x18\t \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassTrainingSpec\x12`\n\x07serving\x18\n \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassServingSpec\x12_\n\x0cnotification\x18\x0b \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\\\n\x0ereportSchedule\x18\x0c \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\x0c\n\x04\x66\x61st\x18\r \x01(\x08\x12\x0e\n\x06paused\x18\x0e \x01(\x08\x12\x12\n\nregistered\x18\x0f \x01(\x08\x12\x1a\n\x12\x61rtifactBucketName\x18\x10 \x01(\t\"\xe7\x08\n\x10ModelClassStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12`\n\x06\x62\x65stFE\x18\x03 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12j\n\x16trainingScheduleStatus\x18\x04 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12l\n\x18predictionScheduleStatus\x18\x05 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12l\n\x18monitoringScheduleStatus\x18\x06 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12h\n\x14reportScheduleStatus\x18\x07 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12\x16\n\x0e\x62\x65stModelScore\x18\x08 \x01(\x01\x12\x0f\n\x07retired\x18\t \x03(\t\x12\x15\n\rpredictorName\x18\n \x01(\t\x12\x13\n\x0b\x64\x61taAppName\x18\x0b \x01(\t\x12\x13\n\x0btriggeredBy\x18\x0c \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x0e \x01(\t\x12=\n\tlastRunAt\x18\x0f \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x13\n\x0blastRunName\x18\x10 \x01(\t\x12\x44\n\x10lastPredictionAt\x18\x11 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12lastPredictionName\x18\x12 \x01(\t\x12\x18\n\x10predictionsCount\x18\x13 \x01(\x05\x12\x11\n\trunsCount\x18\x14 \x01(\x05\x12\x13\n\x0bmodelsCount\x18\x15 \x01(\x05\x12\x0c\n\x04live\x18\x16 \x01(\x08\x12\x17\n\x0fpredictorsCount\x18\x17 \x01(\x05\x12\x43\n\nconditions\x18\x18 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x87\x05\n\x16ModelClassTrainingSpec\x12\x33\n\x06labRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x19\n\x11studyTemplateName\x18\x02 \x01(\t\x12Z\n\x0emodelUnitTests\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12^\n\x10trainingSchedule\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12g\n\x0bsearchSpace\x18\x08 \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AlgorithmSearchSpaceSpec\x12X\n\tresources\x18\t \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x13\n\x0btriggeredBy\x18\n \x01(\t\x12\x0e\n\x06paused\x18\x0b \x01(\x08\x12\x0f\n\x07maxTime\x18\x0c \x01(\x05\x12\x11\n\tmaxModels\x18\r \x01(\x05\x12\x10\n\x08trainers\x18\x0e \x01(\x05\x12\x0f\n\x07\x61\x62orted\x18\x0f \x01(\x08\x12\x11\n\texplained\x18\x10 \x01(\x08\x12\x0e\n\x06preSQL\x18\x11 \x03(\t\x12\x0f\n\x07postSQL\x18\x12 \x03(\t\"\xb3\x01\n\x12ModelGroupByStatus\x12\x11\n\tmodelsURI\x18\x01 \x01(\t\x12\x13\n\x0bprofilesURI\x18\x02 \x01(\t\x12\x14\n\x0c\x66orecastsURI\x18\x03 \x01(\t\x12_\n\rworkerResults\x18\x04 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"\x9d\x01\n\tModelList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"]\n\x0bModelResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\talgorithm\x18\x02 \x01(\t\x12\r\n\x05score\x18\x03 \x01(\x01\x12\r\n\x05\x65rror\x18\x04 \x01(\x08\x12\x0f\n\x07trialID\x18\x05 \x01(\x05\"\x95\x0c\n\tModelSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x14\n\x0cmodelVersion\x18\x03 \x01(\t\x12\x11\n\tstudyName\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x61tasetName\x18\x05 \x01(\t\x12\x0c\n\x04task\x18\x06 \x01(\t\x12\x0f\n\x07subtask\x18\x07 \x01(\t\x12Y\n\tobjective\x18\x08 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12l\n\x12\x66\x65\x61tureEngineering\x18\t \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12\x63\n\testimator\x18\n \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12X\n\x08\x65nsemble\x18\x0b \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EnsembleSpec\x12X\n\x08training\x18\x0c \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TrainingSpec\x12\x0c\n\x04test\x18\r \x01(\x08\x12\r\n\x05\x61\x62ort\x18\x0e \x01(\x08\x12\x0f\n\x07package\x18\x0f \x01(\x08\x12\x0e\n\x06report\x18\x10 \x01(\x08\x12\r\n\x05pause\x18\x11 \x01(\x08\x12\x0f\n\x07profile\x18\x12 \x01(\x08\x12\x10\n\x08\x66orecast\x18\x13 \x01(\x08\x12\x0f\n\x07\x65xplain\x18\x14 \x01(\x08\x12\x10\n\x08unitTest\x18\x15 \x01(\x08\x12\x10\n\x08\x62\x61seline\x18\x16 \x01(\x08\x12\x0c\n\x04\x66\x61st\x18\x17 \x01(\x08\x12\x1a\n\x12\x61rtifactBucketName\x18\x18 \x01(\t\x12]\n\x0b\x66orecasting\x18\x19 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ForecasterSpec\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18\x1a \x01(\x03\x12\x15\n\restimatorType\x18\x1b \x01(\t\x12\x12\n\nmodelClass\x18\x1c \x01(\t\x12\x0f\n\x07trialID\x18\x1d \x01(\x05\x12T\n\x08\x61pproval\x18\x1e \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ApprovalSpec\x12h\n\x10interpretability\x18\x1f \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilitySpec\x12U\n\tunitTests\x18  \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12q\n\x12partitionLocations\x18! \x01(\x0b\x32U.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PartitionModelLocationsSpec\x12\x16\n\x0emodelClassName\x18\" \x01(\t\x12\x19\n\x11modelClassRunName\x18# \x01(\t\x12_\n\x0cnotification\x18$ \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\"\x93\x02\n\x10ModelStageStatus\x12\r\n\x05phase\x18\x01 \x01(\t\x12=\n\tstartedAt\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x61\n\x0funitTestsResult\x18\t \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\r\n\x05\x65rror\x18\n \x01(\t\"\xeb\"\n\x0bModelStatus\x12\x45\n\x11trainingStartedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12G\n\x13trainingCompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x44\n\x10testingStartedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x46\n\x12testingCompletedAt\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x17\n\x0fvalidationScore\x18\x08 \x01(\x01\x12\x15\n\rtrainingScore\x18\t \x01(\x01\x12\x11\n\ttestScore\x18\n \x01(\x01\x12X\n\nvalidation\x18\r \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12S\n\x05train\x18\x0e \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12R\n\x04test\x18\x0f \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12R\n\x04tune\x18\x10 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12V\n\x08\x66\x65\x65\x64\x62\x61\x63k\x18\x11 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12\r\n\x05phase\x18\x12 \x01(\t\x12\x12\n\nreportName\x18\x13 \x01(\t\x12]\n\x0ereportLocation\x18\x14 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x63\n\x14trainWeightsLocation\x18\x15 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13testWeightsLocation\x18\x16 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13\x66ullWeightsLocation\x18\x17 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19trainLabelEncoderLocation\x18\x18 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12^\n\x0fprofileLocation\x18\x1b \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19misclassificationLocation\x18\x1c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12_\n\x10\x66orecastLocation\x18\x1d \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12^\n\x0fpackageLocation\x18\x1e \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12g\n\x12impurityImportance\x18\x1f \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\x12j\n\x15permutationImportance\x18  \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\x12X\n\x07runtime\x18! \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.RuntimeStatus\x12\x63\n\x14trainDatasetLocation\x18\" \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13testDatasetLocation\x18# \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19validationDatasetLocation\x18$ \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x1a\n\x12observedGeneration\x18% \x01(\x03\x12\x14\n\x0ctrainingRows\x18& \x01(\x05\x12\x13\n\x0btestingRows\x18\' \x01(\x05\x12\x16\n\x0evalidationRows\x18( \x01(\x05\x12\x16\n\x0e\x66\x61ilureMessage\x18* \x01(\t\x12\x10\n\x08progress\x18+ \x01(\x05\x12\x13\n\x0bsizeInBytes\x18, \x01(\x05\x12\x0f\n\x07latency\x18- \x01(\x01\x12X\n\x07serving\x18/ \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingStatus\x12\x13\n\x0btarFileHash\x18\x30 \x01(\t\x12^\n\x10trainingDataHash\x18\x31 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataHashes\x12g\n\x11trainingResources\x18\x32 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x66\n\x10testingResources\x18\x33 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x11\n\ttrainedBy\x18\x34 \x01(\t\x12K\n\x04logs\x18\x35 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12V\n\x08rocCurve\x18\x36 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RocAucCurve\x12Q\n\x07prCurve\x18\x37 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PRCurve\x12\x66\n\x14trainConfusionMatrix\x18\x38 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrix\x12\x65\n\x13testConfusionMatrix\x18\x39 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrix\x12\x61\n\x16\x63orrelationsWithTarget\x18: \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\x12Z\n\x0ftopCorrelations\x18; \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\x12=\n\tupdatedAt\x18< \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12V\n\x08\x61pproval\x18= \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ApprovalStatus\x12j\n\x10interpretability\x18> \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilityStatus\x12O\n\x06images\x18? \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Images\x12\x61\n\x0funitTestResults\x18@ \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\x65\n\x13\x66\x65\x65\x64\x62\x61\x63kTestResults\x18\x41 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12]\n\x07groupby\x18\x42 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelGroupByStatus\x12[\n\x05usage\x18\x44 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x43\n\nconditions\x18\x45 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xdf\x01\n\x0eModelTestSuite\x12=\n\x10\x62\x61selineModelRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x37\n\ndatasetRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12U\n\tunitTests\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\"/\n\x10NNLayerParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"=\n\x10OutlierModelSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x18\n\x10outlierAlgorithm\x18\x02 \x01(\t\"\xcc\x01\n\x1bPartitionModelLocationsSpec\x12\x17\n\x0fpartitionFolder\x18\x01 \x01(\t\x12\x1e\n\x16partitionProfileFolder\x18\x02 \x01(\t\x12\x1b\n\x13partitionReportFile\x18\x03 \x01(\t\x12\x1c\n\x14partitionModelFolder\x18\x04 \x01(\t\x12\x1a\n\x12partitionModelFile\x18\x05 \x01(\t\x12\x1d\n\x15partitionForecastFile\x18\x06 \x01(\t\"\x84\x01\n\x17PercentilePrunerOptions\x12\x12\n\npercentile\x18\x01 \x01(\x05\x12\x15\n\rstartupTrials\x18\x02 \x01(\x05\x12\x13\n\x0bwarmupSteps\x18\x03 \x01(\x05\x12\x16\n\x0eintervalTrials\x18\x04 \x01(\x05\x12\x11\n\tminTrials\x18\x05 \x01(\x05\"\x93\x04\n\nPrunerSpec\x12\x0c\n\x04type\x18\x01 \x01(\t\x12]\n\x06median\x18\x02 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.MedianPrunerOptions\x12\x65\n\npercentile\x18\x03 \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PercentilePrunerOptions\x12m\n\x11successiveHalving\x18\x04 \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SuccessiveHalvingOptions\x12]\n\thyperband\x18\x05 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.HyperbandOptions\x12\x63\n\tthreshold\x18\x06 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ThresholdPrunerOptions\"\xd0\x01\n\x18RegressionForecasterSpec\x12\x10\n\x08\x65nsemble\x18\x01 \x01(\x08\x12\x12\n\nimputation\x18\x02 \x01(\t\x12\x10\n\x08\x65ncoding\x18\x03 \x01(\t\x12\x0f\n\x07scaling\x18\x04 \x01(\t\x12\x0c\n\x04\x64\x61te\x18\x05 \x01(\x08\x12\x0f\n\x07windows\x18\x06 \x03(\x05\x12\x0c\n\x04lags\x18\x07 \x03(\x05\x12\x11\n\tfunctions\x18\x08 \x03(\t\x12\x0b\n\x03\x65ma\x18\t \x01(\x08\x12\x0b\n\x03log\x18\n \x01(\x08\x12\x11\n\treduction\x18\x0b \x01(\t\"\xf8\x01\n\x06Report\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12R\n\x04spec\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportSpec\x12V\n\x06status\x18\x03 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportStatus\"\x8a\x01\n\x13ReportGroupByStatus\x12\x12\n\nreportsURI\x18\x01 \x01(\t\x12_\n\rworkerResults\x18\x04 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"\x9f\x01\n\nReportList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12O\n\x05items\x18\x02 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xe9\x03\n\nReportSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x36\n\tentityRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x12\n\nreportType\x18\x03 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x04 \x01(\t\x12_\n\x0cnotification\x18\x05 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\r\n\x05owner\x18\x06 \x01(\t\x12X\n\tresources\x18\x07 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0f\n\x07timeout\x18\x08 \x01(\x03\x12\x33\n\x06labRef\x18\t \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0b\n\x03key\x18\n \x03(\t\x12\x1a\n\x12\x61rtifactBucketName\x18\x0b \x01(\t\x12\x16\n\x0emodelClassName\x18\x0c \x01(\t\x12\x19\n\x11modelClassRunName\x18\r \x01(\t\"\xb3\x04\n\x0cReportStatus\x12?\n\x0b\x63ompletedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x02 \x01(\t\x12W\n\x08location\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\x12K\n\x04logs\x18\x07 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12=\n\tupdatedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12^\n\x07groupby\x18\t \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportGroupByStatus\x12\x43\n\nconditions\x18\n \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xde\x01\n\rRuntimeStatus\x12\x15\n\rpythonVersion\x18\x01 \x01(\t\x12\n\n\x02os\x18\x03 \x01(\t\x12s\n\x0epythonPackages\x18\x04 \x03(\x0b\x32[.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.RuntimeStatus.PythonPackagesEntry\x1a\x35\n\x13PythonPackagesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x83\x05\n\nSearchSpec\x12\x0f\n\x07sampler\x18\x01 \x01(\t\x12T\n\x06pruner\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PrunerSpec\x12\x0f\n\x07maxTime\x18\x04 \x01(\x05\x12\x11\n\tmaxModels\x18\x05 \x01(\x05\x12\x10\n\x08maxScore\x18\x06 \x01(\x01\x12\x10\n\x08trainers\x18\x07 \x01(\x05\x12\x0c\n\x04test\x18\x08 \x01(\x05\x12\x11\n\tretainTop\x18\t \x01(\x05\x12\x13\n\x0bretainedFor\x18\n \x01(\x05\x12g\n\x0bsearchSpace\x18\x0b \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AlgorithmSearchSpaceSpec\x12Z\n\tearlyStop\x18\x0c \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EarlyStopSpec\x12Y\n\tobjective\x18\r \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12\x62\n\x12secondaryObjective\x18\x0e \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12\x0c\n\x04goal\x18\x0f \x01(\t\"L\n\x15SeasonalityPeriodSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04\x61uto\x18\x02 \x01(\x08\x12\x14\n\x0c\x66ourierOrder\x18\x03 \x01(\x05\"\x87\x04\n\x0fSeasonalitySpec\x12\x0c\n\x04\x61uto\x18\x01 \x01(\x08\x12_\n\x06yearly\x18\x02 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12\x62\n\tquarterly\x18\x03 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12`\n\x07monthly\x18\x04 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12_\n\x06weekly\x18\x05 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12^\n\x05\x64\x61ily\x18\x06 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\"\xb7\x03\n\x12ServingEnvironment\x12\x0c\n\x04name\x18\x01 \x01(\t\x12Q\n\x05tests\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12;\n\x0eservingSiteRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12S\n\x06\x61\x63\x63\x65ss\x18\x04 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\x05 \x01(\x05\x12\x0e\n\x06online\x18\x06 \x01(\x08\x12\x11\n\tdashboard\x18\x07 \x01(\x08\x12X\n\tresources\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0e\n\x06preSQL\x18\t \x03(\t\x12\x0f\n\x07postSQL\x18\n \x03(\t\"\xe2\x03\n\x0bServingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x15\n\rpredictorName\x18\x02 \x01(\t\x12X\n\tresources\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12;\n\x0eservingSiteRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0e\n\x06online\x18\x07 \x01(\x08\x12\x11\n\tdashboard\x18\x08 \x01(\x08\x12S\n\x06\x61\x63\x63\x65ss\x18\t \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\n \x01(\x05\x12\x11\n\tpromotion\x18\x0c \x01(\t\x12\x37\n\napprovedBy\x18\r \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12>\n\napprovedAt\x18\x0e \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"\x7f\n\rServingStatus\x12\x15\n\rpredictorName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x61taAppName\x18\x03 \x01(\t\x12\x19\n\x11predictorEndpoint\x18\x04 \x01(\t\x12\x19\n\x11\x64\x61shboardEndpoint\x18\x05 \x01(\t\x12\x0c\n\x04role\x18\x06 \x01(\t\"\xf5\x01\n\x05Study\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudySpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyStatus\"\x9d\x01\n\tStudyList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\"\xb4\x02\n\x10StudyPhaseStatus\x12=\n\tstartedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12waitingModelsCount\x18\x03 \x01(\x05\x12\x1a\n\x12runningModelsCount\x18\x04 \x01(\x05\x12\x19\n\x11\x66\x61iledModelsCount\x18\x05 \x01(\x05\x12\x1c\n\x14\x63ompletedModelsCount\x18\x06 \x01(\x05\x12\x11\n\tbestScore\x18\x07 \x01(\x01\x12\x1c\n\x14modelsWithNoProgress\x18\x08 \x01(\x05\"a\n\x11StudyScheduleSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12;\n\x07startAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"\xc5\x0e\n\tStudySpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x33\n\x06labRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0b\x64\x61tasetName\x18\x04 \x01(\t\x12\x0c\n\x04task\x18\x05 \x01(\t\x12\x0f\n\x07subtask\x18\x06 \x01(\t\x12h\n\x08\x66\x65Search\x18\x07 \x01(\x0b\x32V.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSearchSpec\x12i\n\x10imbalanceHandler\x18\x08 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ImbalanceHandlingSpec\x12X\n\x08\x62\x61seline\x18\t \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.BaselineSpec\x12T\n\x06search\x18\n \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SearchSpec\x12Z\n\tensembles\x18\x0b \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EnsemblesSpec\x12`\n\x10trainingTemplate\x18\x0c \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TrainingSpec\x12\x62\n\x10\x66orecastTemplate\x18\r \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ForecasterSpec\x12]\n\x08schedule\x18\x0e \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyScheduleSpec\x12h\n\x10interpretability\x18\x0f \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilitySpec\x12`\n\x0coutlierModel\x18\x10 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.OutlierModelSpec\x12\r\n\x05\x61\x62ort\x18\x11 \x01(\x08\x12\x0e\n\x06report\x18\x12 \x01(\x08\x12\r\n\x05pause\x18\x13 \x01(\x08\x12\x0f\n\x07profile\x18\x14 \x01(\x08\x12\x0f\n\x07\x65xplain\x18\x15 \x01(\x08\x12\x0c\n\x04\x66\x61st\x18\x16 \x01(\x08\x12\x1a\n\x12\x61rtifactBucketName\x18\x17 \x01(\t\x12\r\n\x05owner\x18\x18 \x01(\t\x12\x10\n\x08template\x18\x19 \x01(\x08\x12_\n\x0cnotification\x18\x1a \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12[\n\x02gc\x18\x1b \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GarbageCollectionSpec\x12\x14\n\x0cmodelVersion\x18\x1c \x01(\t\x12\x0f\n\x07timeout\x18\x1d \x01(\x05\x12]\n\x11unitTestsTemplate\x18\x1e \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12i\n\x0egroupLocations\x18\x1f \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GroupSplitLocationsSpec\x12\x16\n\x0emodelClassName\x18  \x01(\t\x12\x19\n\x11modelClassRunName\x18! \x01(\t\x12V\n\x07serving\x18\" \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingSpec\"\xfe\x10\n\x0bStudyStatus\x12\x13\n\x0bmodelsCount\x18\x01 \x01(\x05\x12?\n\x0b\x63ompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x11\n\tbestModel\x18\x03 \x01(\t\x12\x16\n\x0e\x62\x65stModelScore\x18\x04 \x01(\x01\x12^\n\x0fprofileLocation\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12]\n\x0ereportLocation\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x12\n\nreportName\x18\x07 \x01(\t\x12\r\n\x05phase\x18\x08 \x01(\t\x12\x1a\n\x12observedGeneration\x18\t \x01(\x03\x12\x63\n\x14trainDatasetLocation\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13testDatasetLocation\x18\x0b \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19validationDatasetLocation\x18\x0c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12`\n\x11optimizerLocation\x18\r \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x13\n\x0blastModelID\x18\x0e \x01(\x03\x12\x15\n\rfailureReason\x18\x0f \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x10 \x01(\t\x12\x19\n\x11trainingRowsCount\x18\x11 \x01(\x05\x12\x18\n\x10testingRowsCount\x18\x12 \x01(\x05\x12\x1b\n\x13validationRowsCount\x18\x13 \x01(\x05\x12\x10\n\x08progress\x18\x14 \x01(\x05\x12^\n\x10trainingDataHash\x18\x15 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataHashes\x12\x13\n\x0btriggeredBy\x18\x16 \x01(\t\x12K\n\x04logs\x18\x17 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12\x66\n\x12\x66\x65\x61tureEngineering\x18\x18 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\\\n\x08\x62\x61seline\x18\x19 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12Z\n\x06search\x18\x1a \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\\\n\x08\x65nsemble\x18\x1b \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12X\n\x04test\x18\x1c \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12[\n\x07\x65xplain\x18\x1d \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\x65\n\x0e\x64riftDetection\x18\x1e \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DriftDetectorStatus\x12=\n\tupdatedAt\x18\x1f \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12p\n\x16\x62\x65stFeatureEngineering\x18  \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12]\n\x02gc\x18! \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GarbageCollectionStatus\x12\x43\n\nconditions\x18% \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x7f\n\x18SuccessiveHalvingOptions\x12\x14\n\x0cminResources\x18\x01 \x01(\x05\x12\x17\n\x0freductionFactor\x18\x02 \x01(\x05\x12\x1c\n\x14minEarlyStoppingRate\x18\x03 \x01(\x05\x12\x16\n\x0e\x62ootstrapCount\x18\x04 \x01(\x05\"h\n\x15SuccessiveHalvingSpec\x12\x0e\n\x06\x62udget\x18\x01 \x01(\x05\x12\x0f\n\x07\x62racket\x18\x02 \x01(\x05\x12\x0c\n\x04rung\x18\x03 \x01(\x05\x12\x0e\n\x06\x63onfID\x18\x04 \x01(\x05\x12\x10\n\x08modality\x18\x1a \x01(\t\"\xad\x01\n\x10TextPipelineSpec\x12\x0f\n\x07\x65ncoder\x18\x01 \x01(\t\x12\x11\n\ttokenizer\x18\x02 \x01(\t\x12\x11\n\tstopwords\x18\x03 \x01(\x08\x12\x0b\n\x03pos\x18\x04 \x01(\x08\x12\r\n\x05lemma\x18\x05 \x01(\x08\x12\x0c\n\x04stem\x18\x06 \x01(\x08\x12\x11\n\tembedding\x18\x07 \x01(\t\x12\x0b\n\x03svd\x18\x08 \x01(\x08\x12\x18\n\x10maxSvdComponents\x18\t \x01(\x05\"b\n\x16ThresholdPrunerOptions\x12\r\n\x05lower\x18\x01 \x01(\x01\x12\r\n\x05upper\x18\x02 \x01(\x01\x12\x13\n\x0bwarmupSteps\x18\x03 \x01(\x05\x12\x15\n\rintervalSteps\x18\x04 \x01(\x05\"\x8a\x01\n\x0fTimeSeriesEvent\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06method\x18\x02 \x01(\t\x12\x0f\n\x07holiday\x18\x03 \x01(\x08\x12\x0f\n\x07\x63ountry\x18\x04 \x01(\t\x12\x10\n\x08preEvent\x18\x05 \x01(\x05\x12\x11\n\tpostEvent\x18\x06 \x01(\x05\x12\x12\n\ntimePoints\x18\x07 \x03(\t\"\xe2\x04\n\x0cTrainingSpec\x12\x33\n\x06labRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08priority\x18\x02 \x01(\t\x12\x0e\n\x06\x63vtype\x18\x03 \x01(\t\x12\r\n\x05\x66olds\x18\x05 \x01(\x05\x12V\n\x05split\x18\x06 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataSplitSpec\x12\x13\n\x0b\x65valMetrics\x18\x07 \x03(\t\x12[\n\x02sh\x18\n \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SuccessiveHalvingSpec\x12\x0c\n\x04seed\x18\x0b \x01(\x01\x12X\n\tresources\x18\x0c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0b\n\x03gpu\x18\r \x01(\x08\x12\x19\n\x11\x66\x65\x61tureImportance\x18\x0f \x01(\x08\x12\x11\n\tsamplePct\x18\x11 \x01(\x05\x12\\\n\ncheckpoint\x18\x12 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.CheckpointSpec\x12\x10\n\x08logLevel\x18\x13 \x01(\t\x12\x0f\n\x07timeout\x18\x14 \x01(\x05\"\xdc\x01\n\x18UnivariateForecastStatus\x12\x1b\n\x13gridSearchResultURI\x18\x01 \x01(\t\x12g\n\rbaseEstimator\x18\x02 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12\x10\n\x08modelURI\x18\x03 \x01(\t\x12\x13\n\x0b\x63vResultURI\x18\x04 \x01(\t\x12\x13\n\x0b\x66orecastURI\x18\x05 \x01(\t\"\'\n\x11VideoPipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\"=\n\nWindowSpec\x12\x10\n\x08interval\x18\x01 \x01(\t\x12\r\n\x05start\x18\x02 \x01(\x05\x12\x0e\n\x06length\x18\x03 \x01(\x05\x42:Z8github.com/metaprov/modelaapi/pkg/apis/training/v1alpha1')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.generated_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z8github.com/metaprov/modelaapi/pkg/apis/training/v1alpha1'
@@ -39,196 +39,182 @@
   _AUDIOPIPELINESPEC._serialized_end=902
   _BACKTESTSPEC._serialized_start=904
   _BACKTESTSPEC._serialized_end=981
   _BASELINESPEC._serialized_start=983
   _BASELINESPEC._serialized_end=1046
   _CHANGEPOINT._serialized_start=1048
   _CHANGEPOINT._serialized_end=1061
-  _CHATBOTESTIMATORSPEC._serialized_start=1063
-  _CHATBOTESTIMATORSPEC._serialized_end=1099
-  _CHECKPOINTSPEC._serialized_start=1102
-  _CHECKPOINTSPEC._serialized_end=1252
-  _CLASSICALESTIMATORSPEC._serialized_start=1255
-  _CLASSICALESTIMATORSPEC._serialized_end=1401
-  _CUSTOMREPORTSPEC._serialized_start=1403
-  _CUSTOMREPORTSPEC._serialized_end=1500
-  _DATAHASHES._serialized_start=1502
-  _DATAHASHES._serialized_end=1578
-  _DATASPLITSPEC._serialized_start=1581
-  _DATASPLITSPEC._serialized_end=1841
-  _DEEPESTIMATORLAYER._serialized_start=1844
-  _DEEPESTIMATORLAYER._serialized_end=2009
-  _DEEPESTIMATORSPEC._serialized_start=2012
-  _DEEPESTIMATORSPEC._serialized_end=2242
-  _DRIFTDETECTORSTATUS._serialized_start=2244
-  _DRIFTDETECTORSTATUS._serialized_end=2290
-  _DRIFTMODELSPEC._serialized_start=2292
-  _DRIFTMODELSPEC._serialized_end=2351
-  _EARLYSTOPSPEC._serialized_start=2353
-  _EARLYSTOPSPEC._serialized_end=2435
-  _ENSEMBLERULES._serialized_start=2437
-  _ENSEMBLERULES._serialized_end=2452
-  _ENSEMBLESPEC._serialized_start=2455
-  _ENSEMBLESPEC._serialized_end=2698
-  _ENSEMBLESSPEC._serialized_start=2700
-  _ENSEMBLESSPEC._serialized_end=2795
-  _ENTITYREF._serialized_start=2797
-  _ENTITYREF._serialized_end=2839
-  _EVALMETRICS._serialized_start=2842
-  _EVALMETRICS._serialized_end=2979
-  _EVALPERIOD._serialized_start=2982
-  _EVALPERIOD._serialized_end=3206
-  _FEATUREENGINEERINGPIPELINE._serialized_start=3209
-  _FEATUREENGINEERINGPIPELINE._serialized_end=4048
-  _FEATUREENGINEERINGSEARCHSPEC._serialized_start=4051
-  _FEATUREENGINEERINGSEARCHSPEC._serialized_end=4448
-  _FEATUREENGINEERINGSEARCHSTATUS._serialized_start=4451
-  _FEATUREENGINEERINGSEARCHSTATUS._serialized_end=4579
-  _FEATUREENGINEERINGSPEC._serialized_start=4582
-  _FEATUREENGINEERINGSPEC._serialized_end=4829
-  _FEATUREIMPORTANCE._serialized_start=4831
-  _FEATUREIMPORTANCE._serialized_end=4887
-  _FEATUREINFO._serialized_start=4889
-  _FEATUREINFO._serialized_end=4947
-  _FEATUREPAIR._serialized_start=4949
-  _FEATUREPAIR._serialized_end=4984
-  _FEATURESELECTIONSPEC._serialized_start=4987
-  _FEATURESELECTIONSPEC._serialized_end=5200
-  _FORECASTERSPEC._serialized_start=5203
-  _FORECASTERSPEC._serialized_end=6219
-  _GARBAGECOLLECTIONSPEC._serialized_start=6221
-  _GARBAGECOLLECTIONSPEC._serialized_end=6341
-  _GARBAGECOLLECTIONSTATUS._serialized_start=6344
-  _GARBAGECOLLECTIONSTATUS._serialized_end=6486
-  _GENERATEDCOLUMNSPEC._serialized_start=6488
-  _GENERATEDCOLUMNSPEC._serialized_end=6590
-  _GROUPSPLITLOCATIONSSPEC._serialized_start=6592
-  _GROUPSPLITLOCATIONSSPEC._serialized_end=6678
-  _HYPERPARAMETERVALUE._serialized_start=6680
-  _HYPERPARAMETERVALUE._serialized_end=6730
-  _HYPERBANDOPTIONS._serialized_start=6732
-  _HYPERBANDOPTIONS._serialized_end=6843
-  _IMAGEPIPELINESPEC._serialized_start=6845
-  _IMAGEPIPELINESPEC._serialized_end=6884
-  _IMBALANCEHANDLINGSPEC._serialized_start=6886
-  _IMBALANCEHANDLINGSPEC._serialized_end=6945
-  _INTERPRETABILITYSPEC._serialized_start=6948
-  _INTERPRETABILITYSPEC._serialized_end=7230
-  _INTERPRETABILITYSTATUS._serialized_start=7233
-  _INTERPRETABILITYSTATUS._serialized_end=7559
-  _LEVEL._serialized_start=7561
-  _LEVEL._serialized_end=7647
-  _MEDIANPRUNEROPTIONS._serialized_start=7649
-  _MEDIANPRUNEROPTIONS._serialized_end=7756
-  _MODEL._serialized_start=7759
-  _MODEL._serialized_end=8004
-  _MODELCLASS._serialized_start=8007
-  _MODELCLASS._serialized_end=8267
-  _MODELCLASSDATASPEC._serialized_start=8270
-  _MODELCLASSDATASPEC._serialized_end=8859
-  _MODELCLASSLIST._serialized_start=8862
-  _MODELCLASSLIST._serialized_end=9029
-  _MODELCLASSRUN._serialized_start=9032
-  _MODELCLASSRUN._serialized_end=9301
-  _MODELCLASSRUNLIST._serialized_start=9304
-  _MODELCLASSRUNLIST._serialized_end=9477
-  _MODELCLASSRUNSPEC._serialized_start=9480
-  _MODELCLASSRUNSPEC._serialized_end=9686
-  _MODELCLASSRUNSTATUS._serialized_start=9689
-  _MODELCLASSRUNSTATUS._serialized_end=10310
-  _MODELCLASSSERVINGSPEC._serialized_start=10313
-  _MODELCLASSSERVINGSPEC._serialized_end=10654
-  _MODELCLASSSPEC._serialized_start=10657
-  _MODELCLASSSPEC._serialized_end=11498
-  _MODELCLASSSTATUS._serialized_start=11501
-  _MODELCLASSSTATUS._serialized_end=12648
-  _MODELCLASSTRAININGSPEC._serialized_start=12651
-  _MODELCLASSTRAININGSPEC._serialized_end=13392
-  _MODELGROUPBYSTATUS._serialized_start=13395
-  _MODELGROUPBYSTATUS._serialized_end=13574
-  _MODELIMAGESPEC._serialized_start=13576
-  _MODELIMAGESPEC._serialized_end=13658
-  _MODELLIST._serialized_start=13661
-  _MODELLIST._serialized_end=13818
-  _MODELRESULT._serialized_start=13820
-  _MODELRESULT._serialized_end=13907
-  _MODELSPEC._serialized_start=13910
-  _MODELSPEC._serialized_end=16175
-  _MODELSTAGESTATUS._serialized_start=16178
-  _MODELSTAGESTATUS._serialized_end=16453
-  _MODELSTATUS._serialized_start=16456
-  _MODELSTATUS._serialized_end=20895
-  _MODELTESTSUITE._serialized_start=20898
-  _MODELTESTSUITE._serialized_end=21121
-  _NLPESTIMATORSPEC._serialized_start=21123
-  _NLPESTIMATORSPEC._serialized_end=21155
-  _NNLAYERPARAMETER._serialized_start=21157
-  _NNLAYERPARAMETER._serialized_end=21204
-  _PARTITIONMODELLOCATIONSSPEC._serialized_start=21207
-  _PARTITIONMODELLOCATIONSSPEC._serialized_end=21411
-  _PERCENTILEPRUNEROPTIONS._serialized_start=21414
-  _PERCENTILEPRUNEROPTIONS._serialized_end=21546
-  _PRUNERSPEC._serialized_start=21549
-  _PRUNERSPEC._serialized_end=22080
-  _REGRESSIONFORECASTERSPEC._serialized_start=22083
-  _REGRESSIONFORECASTERSPEC._serialized_end=22291
-  _REPORT._serialized_start=22294
-  _REPORT._serialized_end=22542
-  _REPORTGROUPBYSTATUS._serialized_start=22545
-  _REPORTGROUPBYSTATUS._serialized_end=22683
-  _REPORTLIST._serialized_start=22686
-  _REPORTLIST._serialized_end=22845
-  _REPORTSPEC._serialized_start=22848
-  _REPORTSPEC._serialized_end=23262
-  _REPORTSTATUS._serialized_start=23265
-  _REPORTSTATUS._serialized_end=23828
-  _RUNTIMESTATUS._serialized_start=23831
-  _RUNTIMESTATUS._serialized_end=24072
-  _RUNTIMESTATUS_PYTHONPACKAGESENTRY._serialized_start=24019
-  _RUNTIMESTATUS_PYTHONPACKAGESENTRY._serialized_end=24072
-  _SEARCHSPEC._serialized_start=24075
-  _SEARCHSPEC._serialized_end=24745
-  _SEASONALITYPERIODSPEC._serialized_start=24747
-  _SEASONALITYPERIODSPEC._serialized_end=24823
-  _SEASONALITYSPEC._serialized_start=24826
-  _SEASONALITYSPEC._serialized_end=25345
-  _SEGMENTSPEC._serialized_start=25347
-  _SEGMENTSPEC._serialized_end=25407
-  _SERVINGENVIRONMENT._serialized_start=25410
-  _SERVINGENVIRONMENT._serialized_end=25849
-  _SERVINGSPEC._serialized_start=25852
-  _SERVINGSPEC._serialized_end=26334
-  _SERVINGSTATUS._serialized_start=26336
-  _SERVINGSTATUS._serialized_end=26439
-  _STUDY._serialized_start=26442
-  _STUDY._serialized_end=26687
-  _STUDYGROUPBYSTATUS._serialized_start=26690
-  _STUDYGROUPBYSTATUS._serialized_end=26827
-  _STUDYLIST._serialized_start=26830
-  _STUDYLIST._serialized_end=26987
-  _STUDYPHASESTATUS._serialized_start=26990
-  _STUDYPHASESTATUS._serialized_end=27298
-  _STUDYSCHEDULESPEC._serialized_start=27300
-  _STUDYSCHEDULESPEC._serialized_end=27397
-  _STUDYSPEC._serialized_start=27400
-  _STUDYSPEC._serialized_end=29558
-  _STUDYSTATUS._serialized_start=29561
-  _STUDYSTATUS._serialized_end=31657
-  _SUCCESSIVEHALVINGOPTIONS._serialized_start=31659
-  _SUCCESSIVEHALVINGOPTIONS._serialized_end=31786
-  _SUCCESSIVEHALVINGSPEC._serialized_start=31788
-  _SUCCESSIVEHALVINGSPEC._serialized_end=31892
-  _TEXTPIPELINESPEC._serialized_start=31895
-  _TEXTPIPELINESPEC._serialized_end=32068
-  _THRESHOLDPRUNEROPTIONS._serialized_start=32070
-  _THRESHOLDPRUNEROPTIONS._serialized_end=32168
-  _TIMESERIESEVENT._serialized_start=32171
-  _TIMESERIESEVENT._serialized_end=32309
-  _TRAININGSPEC._serialized_start=32312
-  _TRAININGSPEC._serialized_end=32980
-  _UNIVARIATEFORECASTSTATUS._serialized_start=32983
-  _UNIVARIATEFORECASTSTATUS._serialized_end=33203
-  _VIDEOPIPELINESPEC._serialized_start=33205
-  _VIDEOPIPELINESPEC._serialized_end=33244
-  _WINDOWSPEC._serialized_start=33246
-  _WINDOWSPEC._serialized_end=33307
+  _CHECKPOINTSPEC._serialized_start=1064
+  _CHECKPOINTSPEC._serialized_end=1214
+  _CLASSICALESTIMATORSPEC._serialized_start=1217
+  _CLASSICALESTIMATORSPEC._serialized_end=1363
+  _CUSTOMREPORTSPEC._serialized_start=1365
+  _CUSTOMREPORTSPEC._serialized_end=1462
+  _DATAHASHES._serialized_start=1464
+  _DATAHASHES._serialized_end=1540
+  _DATASPLITSPEC._serialized_start=1543
+  _DATASPLITSPEC._serialized_end=1714
+  _DEEPESTIMATORLAYER._serialized_start=1717
+  _DEEPESTIMATORLAYER._serialized_end=1882
+  _DEEPESTIMATORSPEC._serialized_start=1885
+  _DEEPESTIMATORSPEC._serialized_end=2115
+  _DRIFTDETECTORSTATUS._serialized_start=2117
+  _DRIFTDETECTORSTATUS._serialized_end=2163
+  _EARLYSTOPSPEC._serialized_start=2165
+  _EARLYSTOPSPEC._serialized_end=2244
+  _ENSEMBLESPEC._serialized_start=2247
+  _ENSEMBLESPEC._serialized_end=2498
+  _ENSEMBLESSPEC._serialized_start=2500
+  _ENSEMBLESSPEC._serialized_end=2595
+  _ENTITYREF._serialized_start=2597
+  _ENTITYREF._serialized_end=2639
+  _EVALMETRICS._serialized_start=2642
+  _EVALMETRICS._serialized_end=2779
+  _EVALPERIOD._serialized_start=2782
+  _EVALPERIOD._serialized_end=3006
+  _FEATUREENGINEERINGPIPELINE._serialized_start=3009
+  _FEATUREENGINEERINGPIPELINE._serialized_end=3379
+  _FEATUREENGINEERINGSEARCHSPEC._serialized_start=3382
+  _FEATUREENGINEERINGSEARCHSPEC._serialized_end=3715
+  _FEATUREENGINEERINGSEARCHSTATUS._serialized_start=3718
+  _FEATUREENGINEERINGSEARCHSTATUS._serialized_end=3846
+  _FEATUREENGINEERINGSPEC._serialized_start=3849
+  _FEATUREENGINEERINGSPEC._serialized_end=4096
+  _FEATUREIMPORTANCE._serialized_start=4098
+  _FEATUREIMPORTANCE._serialized_end=4154
+  _FEATUREINFO._serialized_start=4156
+  _FEATUREINFO._serialized_end=4214
+  _FEATUREPAIR._serialized_start=4216
+  _FEATUREPAIR._serialized_end=4251
+  _FEATURESELECTIONSPEC._serialized_start=4254
+  _FEATURESELECTIONSPEC._serialized_end=4467
+  _FORECASTERSPEC._serialized_start=4470
+  _FORECASTERSPEC._serialized_end=5486
+  _GARBAGECOLLECTIONSPEC._serialized_start=5488
+  _GARBAGECOLLECTIONSPEC._serialized_end=5589
+  _GARBAGECOLLECTIONSTATUS._serialized_start=5592
+  _GARBAGECOLLECTIONSTATUS._serialized_end=5734
+  _GENERATEDCOLUMNSPEC._serialized_start=5736
+  _GENERATEDCOLUMNSPEC._serialized_end=5838
+  _GROUPSPLITLOCATIONSSPEC._serialized_start=5840
+  _GROUPSPLITLOCATIONSSPEC._serialized_end=5926
+  _HYPERPARAMETERVALUE._serialized_start=5928
+  _HYPERPARAMETERVALUE._serialized_end=5978
+  _HYPERBANDOPTIONS._serialized_start=5980
+  _HYPERBANDOPTIONS._serialized_end=6091
+  _IMAGEPIPELINESPEC._serialized_start=6093
+  _IMAGEPIPELINESPEC._serialized_end=6132
+  _IMBALANCEHANDLINGSPEC._serialized_start=6134
+  _IMBALANCEHANDLINGSPEC._serialized_end=6193
+  _INTERPRETABILITYSPEC._serialized_start=6196
+  _INTERPRETABILITYSPEC._serialized_end=6478
+  _INTERPRETABILITYSTATUS._serialized_start=6481
+  _INTERPRETABILITYSTATUS._serialized_end=7035
+  _MEDIANPRUNEROPTIONS._serialized_start=7037
+  _MEDIANPRUNEROPTIONS._serialized_end=7144
+  _MODEL._serialized_start=7147
+  _MODEL._serialized_end=7392
+  _MODELCLASS._serialized_start=7395
+  _MODELCLASS._serialized_end=7655
+  _MODELCLASSDATASPEC._serialized_start=7658
+  _MODELCLASSDATASPEC._serialized_end=8247
+  _MODELCLASSLIST._serialized_start=8250
+  _MODELCLASSLIST._serialized_end=8417
+  _MODELCLASSRUN._serialized_start=8420
+  _MODELCLASSRUN._serialized_end=8689
+  _MODELCLASSRUNLIST._serialized_start=8692
+  _MODELCLASSRUNLIST._serialized_end=8865
+  _MODELCLASSRUNSPEC._serialized_start=8868
+  _MODELCLASSRUNSPEC._serialized_end=9074
+  _MODELCLASSRUNSTATUS._serialized_start=9077
+  _MODELCLASSRUNSTATUS._serialized_end=9698
+  _MODELCLASSSERVINGSPEC._serialized_start=9701
+  _MODELCLASSSERVINGSPEC._serialized_end=10042
+  _MODELCLASSSPEC._serialized_start=10045
+  _MODELCLASSSPEC._serialized_end=10886
+  _MODELCLASSSTATUS._serialized_start=10889
+  _MODELCLASSSTATUS._serialized_end=12016
+  _MODELCLASSTRAININGSPEC._serialized_start=12019
+  _MODELCLASSTRAININGSPEC._serialized_end=12666
+  _MODELGROUPBYSTATUS._serialized_start=12669
+  _MODELGROUPBYSTATUS._serialized_end=12848
+  _MODELLIST._serialized_start=12851
+  _MODELLIST._serialized_end=13008
+  _MODELRESULT._serialized_start=13010
+  _MODELRESULT._serialized_end=13103
+  _MODELSPEC._serialized_start=13106
+  _MODELSPEC._serialized_end=14663
+  _MODELSTAGESTATUS._serialized_start=14666
+  _MODELSTAGESTATUS._serialized_end=14941
+  _MODELSTATUS._serialized_start=14944
+  _MODELSTATUS._serialized_end=19403
+  _MODELTESTSUITE._serialized_start=19406
+  _MODELTESTSUITE._serialized_end=19629
+  _NNLAYERPARAMETER._serialized_start=19631
+  _NNLAYERPARAMETER._serialized_end=19678
+  _OUTLIERMODELSPEC._serialized_start=19680
+  _OUTLIERMODELSPEC._serialized_end=19741
+  _PARTITIONMODELLOCATIONSSPEC._serialized_start=19744
+  _PARTITIONMODELLOCATIONSSPEC._serialized_end=19948
+  _PERCENTILEPRUNEROPTIONS._serialized_start=19951
+  _PERCENTILEPRUNEROPTIONS._serialized_end=20083
+  _PRUNERSPEC._serialized_start=20086
+  _PRUNERSPEC._serialized_end=20617
+  _REGRESSIONFORECASTERSPEC._serialized_start=20620
+  _REGRESSIONFORECASTERSPEC._serialized_end=20828
+  _REPORT._serialized_start=20831
+  _REPORT._serialized_end=21079
+  _REPORTGROUPBYSTATUS._serialized_start=21082
+  _REPORTGROUPBYSTATUS._serialized_end=21220
+  _REPORTLIST._serialized_start=21223
+  _REPORTLIST._serialized_end=21382
+  _REPORTSPEC._serialized_start=21385
+  _REPORTSPEC._serialized_end=21874
+  _REPORTSTATUS._serialized_start=21877
+  _REPORTSTATUS._serialized_end=22440
+  _RUNTIMESTATUS._serialized_start=22443
+  _RUNTIMESTATUS._serialized_end=22665
+  _RUNTIMESTATUS_PYTHONPACKAGESENTRY._serialized_start=22612
+  _RUNTIMESTATUS_PYTHONPACKAGESENTRY._serialized_end=22665
+  _SEARCHSPEC._serialized_start=22668
+  _SEARCHSPEC._serialized_end=23311
+  _SEASONALITYPERIODSPEC._serialized_start=23313
+  _SEASONALITYPERIODSPEC._serialized_end=23389
+  _SEASONALITYSPEC._serialized_start=23392
+  _SEASONALITYSPEC._serialized_end=23911
+  _SERVINGENVIRONMENT._serialized_start=23914
+  _SERVINGENVIRONMENT._serialized_end=24353
+  _SERVINGSPEC._serialized_start=24356
+  _SERVINGSPEC._serialized_end=24838
+  _SERVINGSTATUS._serialized_start=24840
+  _SERVINGSTATUS._serialized_end=24967
+  _STUDY._serialized_start=24970
+  _STUDY._serialized_end=25215
+  _STUDYLIST._serialized_start=25218
+  _STUDYLIST._serialized_end=25375
+  _STUDYPHASESTATUS._serialized_start=25378
+  _STUDYPHASESTATUS._serialized_end=25686
+  _STUDYSCHEDULESPEC._serialized_start=25688
+  _STUDYSCHEDULESPEC._serialized_end=25785
+  _STUDYSPEC._serialized_start=25788
+  _STUDYSPEC._serialized_end=27649
+  _STUDYSTATUS._serialized_start=27652
+  _STUDYSTATUS._serialized_end=29826
+  _SUCCESSIVEHALVINGOPTIONS._serialized_start=29828
+  _SUCCESSIVEHALVINGOPTIONS._serialized_end=29955
+  _SUCCESSIVEHALVINGSPEC._serialized_start=29957
+  _SUCCESSIVEHALVINGSPEC._serialized_end=30061
+  _TEXTPIPELINESPEC._serialized_start=30064
+  _TEXTPIPELINESPEC._serialized_end=30237
+  _THRESHOLDPRUNEROPTIONS._serialized_start=30239
+  _THRESHOLDPRUNEROPTIONS._serialized_end=30337
+  _TIMESERIESEVENT._serialized_start=30340
+  _TIMESERIESEVENT._serialized_end=30478
+  _TRAININGSPEC._serialized_start=30481
+  _TRAININGSPEC._serialized_end=31091
+  _UNIVARIATEFORECASTSTATUS._serialized_start=31094
+  _UNIVARIATEFORECASTSTATUS._serialized_end=31314
+  _VIDEOPIPELINESPEC._serialized_start=31316
+  _VIDEOPIPELINESPEC._serialized_end=31355
+  _WINDOWSPEC._serialized_start=31357
+  _WINDOWSPEC._serialized_end=31418
 # @@protoc_insertion_point(module_scope)
```

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,52 +10,50 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_infra_dot_v1alpha1_dot_generated__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nGgithub.com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd.proto\x12\x35github.com.metaprov.modelaapi.services.cloudproxyd.v1\x1a\x45github.com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated.proto\"\x11\n\x0fShutdownRequest\"\x12\n\x10ShutdownResponse\"q\n\x19VirtualBucketExistRequest\x12T\n\x06\x62ucket\x18\x01 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\"+\n\x1aVirtualBucketExistResponse\x12\r\n\x05\x65xist\x18\x01 \x01(\x08\"\x93\x01\n\x1eKeyExistInVirtualBucketRequest\x12\x0e\n\x06region\x18\x01 \x01(\t\x12T\n\x06\x62ucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x0b\n\x03key\x18\x03 \x01(\t\"0\n\x1fKeyExistInVirtualBucketResponse\x12\r\n\x05\x65xist\x18\x01 \x01(\x08\"\x1c\n\x1a\x43loudVirtualBucketResponse\"\x96\x01\n\x13\x46ileDownloadRequest\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x0e\n\x06tenant\x18\x04 \x01(\t\"\x16\n\x14\x46ileDownloadResponse\"\x8a\x01\n\x12ListObjectsRequest\x12\x0e\n\x06prefix\x18\x01 \x01(\t\x12T\n\x06\x62ucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x0e\n\x06tenant\x18\x03 \x01(\t\"#\n\x13ListObjectsResponse\x12\x0c\n\x04keys\x18\x01 \x03(\t\"\x99\x02\n\x11\x46ileUploadRequest\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x64\n\x06secret\x18\x04 \x03(\x0b\x32T.github.com.metaprov.modelaapi.services.cloudproxyd.v1.FileUploadRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x14\n\x12\x46ileUploadResponse\"r\n\x1a\x43reateVirtualBucketRequest\x12T\n\x06\x62ucket\x18\x01 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\"\x1d\n\x1b\x43reateVirtualBucketResponse2\xf5\t\n\x11\x43loudProxyService\x12\xa5\x01\n\x08\x44ownload\x12J.github.com.metaprov.modelaapi.services.cloudproxyd.v1.FileDownloadRequest\x1aK.github.com.metaprov.modelaapi.services.cloudproxyd.v1.FileDownloadResponse\"\x00\x12\x9f\x01\n\x04List\x12I.github.com.metaprov.modelaapi.services.cloudproxyd.v1.ListObjectsRequest\x1aJ.github.com.metaprov.modelaapi.services.cloudproxyd.v1.ListObjectsResponse\"\x00\x12\x9f\x01\n\x06Upload\x12H.github.com.metaprov.modelaapi.services.cloudproxyd.v1.FileUploadRequest\x1aI.github.com.metaprov.modelaapi.services.cloudproxyd.v1.FileUploadResponse\"\x00\x12\xca\x01\n\x17KeyExistInVirtualBucket\x12U.github.com.metaprov.modelaapi.services.cloudproxyd.v1.KeyExistInVirtualBucketRequest\x1aV.github.com.metaprov.modelaapi.services.cloudproxyd.v1.KeyExistInVirtualBucketResponse\"\x00\x12\xbb\x01\n\x12VirtualBucketExist\x12P.github.com.metaprov.modelaapi.services.cloudproxyd.v1.VirtualBucketExistRequest\x1aQ.github.com.metaprov.modelaapi.services.cloudproxyd.v1.VirtualBucketExistResponse\"\x00\x12\xc8\x01\n\x1d\x43reateVirtualBucketIfNotExist\x12Q.github.com.metaprov.modelaapi.services.cloudproxyd.v1.CreateVirtualBucketRequest\x1aR.github.com.metaprov.modelaapi.services.cloudproxyd.v1.CreateVirtualBucketResponse\"\x00\x12\x9d\x01\n\x08Shutdown\x12\x46.github.com.metaprov.modelaapi.services.cloudproxyd.v1.ShutdownRequest\x1aG.github.com.metaprov.modelaapi.services.cloudproxyd.v1.ShutdownResponse\"\x00\x42\x37Z5github.com/metaprov/modelaapi/services/cloudproxyd/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nGgithub.com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd.proto\x12\x35github.com.metaprov.modelaapi.services.cloudproxyd.v1\x1a\x45github.com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated.proto\"\x11\n\x0fShutdownRequest\"\x12\n\x10ShutdownResponse\"j\n\x12\x42ucketExistRequest\x12T\n\x06\x62ucket\x18\x01 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\"$\n\x13\x42ucketExistResponse\x12\r\n\x05\x65xist\x18\x01 \x01(\x08\"z\n\x15\x45xistsInBucketRequest\x12T\n\x06\x62ucket\x18\x01 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x0b\n\x03key\x18\x02 \x01(\t\"\'\n\x16\x45xistsInBucketResponse\x12\r\n\x05\x65xist\x18\x01 \x01(\x08\"r\n\rDeleteRequest\x12T\n\x06\x62ucket\x18\x01 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x0b\n\x03key\x18\x02 \x01(\t\"\x10\n\x0e\x44\x65leteResponse\"\x96\x01\n\x13\x46ileDownloadRequest\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x0e\n\x06tenant\x18\x04 \x01(\t\"\x16\n\x14\x46ileDownloadResponse\"\x8a\x01\n\x12ListObjectsRequest\x12\x0e\n\x06prefix\x18\x01 \x01(\t\x12T\n\x06\x62ucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x0e\n\x06tenant\x18\x03 \x01(\t\"#\n\x13ListObjectsResponse\x12\x0c\n\x04keys\x18\x01 \x03(\t\"\x84\x01\n\x11\x46ileUploadRequest\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\"\x14\n\x12\x46ileUploadResponse\"k\n\x13\x43reateBucketRequest\x12T\n\x06\x62ucket\x18\x01 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\"\x16\n\x14\x43reateBucketResponse2\xc0\n\n\x11\x43loudProxyService\x12\xa5\x01\n\x08\x44ownload\x12J.github.com.metaprov.modelaapi.services.cloudproxyd.v1.FileDownloadRequest\x1aK.github.com.metaprov.modelaapi.services.cloudproxyd.v1.FileDownloadResponse\"\x00\x12\x9f\x01\n\x04List\x12I.github.com.metaprov.modelaapi.services.cloudproxyd.v1.ListObjectsRequest\x1aJ.github.com.metaprov.modelaapi.services.cloudproxyd.v1.ListObjectsResponse\"\x00\x12\x9f\x01\n\x06Upload\x12H.github.com.metaprov.modelaapi.services.cloudproxyd.v1.FileUploadRequest\x1aI.github.com.metaprov.modelaapi.services.cloudproxyd.v1.FileUploadResponse\"\x00\x12\x97\x01\n\x06\x44\x65lete\x12\x44.github.com.metaprov.modelaapi.services.cloudproxyd.v1.DeleteRequest\x1a\x45.github.com.metaprov.modelaapi.services.cloudproxyd.v1.DeleteResponse\"\x00\x12\xaf\x01\n\x0e\x45xistsInBucket\x12L.github.com.metaprov.modelaapi.services.cloudproxyd.v1.ExistsInBucketRequest\x1aM.github.com.metaprov.modelaapi.services.cloudproxyd.v1.ExistsInBucketResponse\"\x00\x12\xa6\x01\n\x0b\x42ucketExist\x12I.github.com.metaprov.modelaapi.services.cloudproxyd.v1.BucketExistRequest\x1aJ.github.com.metaprov.modelaapi.services.cloudproxyd.v1.BucketExistResponse\"\x00\x12\xa9\x01\n\x0c\x43reateBucket\x12J.github.com.metaprov.modelaapi.services.cloudproxyd.v1.CreateBucketRequest\x1aK.github.com.metaprov.modelaapi.services.cloudproxyd.v1.CreateBucketResponse\"\x00\x12\x9d\x01\n\x08Shutdown\x12\x46.github.com.metaprov.modelaapi.services.cloudproxyd.v1.ShutdownRequest\x1aG.github.com.metaprov.modelaapi.services.cloudproxyd.v1.ShutdownResponse\"\x00\x42\x37Z5github.com/metaprov/modelaapi/services/cloudproxyd/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'github.com.metaprov.modelaapi.services.cloudproxyd.v1.cloudproxyd_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z5github.com/metaprov/modelaapi/services/cloudproxyd/v1'
-  _FILEUPLOADREQUEST_SECRETENTRY._options = None
-  _FILEUPLOADREQUEST_SECRETENTRY._serialized_options = b'8\001'
   _SHUTDOWNREQUEST._serialized_start=201
   _SHUTDOWNREQUEST._serialized_end=218
   _SHUTDOWNRESPONSE._serialized_start=220
   _SHUTDOWNRESPONSE._serialized_end=238
-  _VIRTUALBUCKETEXISTREQUEST._serialized_start=240
-  _VIRTUALBUCKETEXISTREQUEST._serialized_end=353
-  _VIRTUALBUCKETEXISTRESPONSE._serialized_start=355
-  _VIRTUALBUCKETEXISTRESPONSE._serialized_end=398
-  _KEYEXISTINVIRTUALBUCKETREQUEST._serialized_start=401
-  _KEYEXISTINVIRTUALBUCKETREQUEST._serialized_end=548
-  _KEYEXISTINVIRTUALBUCKETRESPONSE._serialized_start=550
-  _KEYEXISTINVIRTUALBUCKETRESPONSE._serialized_end=598
-  _CLOUDVIRTUALBUCKETRESPONSE._serialized_start=600
-  _CLOUDVIRTUALBUCKETRESPONSE._serialized_end=628
-  _FILEDOWNLOADREQUEST._serialized_start=631
-  _FILEDOWNLOADREQUEST._serialized_end=781
-  _FILEDOWNLOADRESPONSE._serialized_start=783
-  _FILEDOWNLOADRESPONSE._serialized_end=805
-  _LISTOBJECTSREQUEST._serialized_start=808
-  _LISTOBJECTSREQUEST._serialized_end=946
-  _LISTOBJECTSRESPONSE._serialized_start=948
-  _LISTOBJECTSRESPONSE._serialized_end=983
-  _FILEUPLOADREQUEST._serialized_start=986
-  _FILEUPLOADREQUEST._serialized_end=1267
-  _FILEUPLOADREQUEST_SECRETENTRY._serialized_start=1222
-  _FILEUPLOADREQUEST_SECRETENTRY._serialized_end=1267
-  _FILEUPLOADRESPONSE._serialized_start=1269
-  _FILEUPLOADRESPONSE._serialized_end=1289
-  _CREATEVIRTUALBUCKETREQUEST._serialized_start=1291
-  _CREATEVIRTUALBUCKETREQUEST._serialized_end=1405
-  _CREATEVIRTUALBUCKETRESPONSE._serialized_start=1407
-  _CREATEVIRTUALBUCKETRESPONSE._serialized_end=1436
-  _CLOUDPROXYSERVICE._serialized_start=1439
-  _CLOUDPROXYSERVICE._serialized_end=2708
+  _BUCKETEXISTREQUEST._serialized_start=240
+  _BUCKETEXISTREQUEST._serialized_end=346
+  _BUCKETEXISTRESPONSE._serialized_start=348
+  _BUCKETEXISTRESPONSE._serialized_end=384
+  _EXISTSINBUCKETREQUEST._serialized_start=386
+  _EXISTSINBUCKETREQUEST._serialized_end=508
+  _EXISTSINBUCKETRESPONSE._serialized_start=510
+  _EXISTSINBUCKETRESPONSE._serialized_end=549
+  _DELETEREQUEST._serialized_start=551
+  _DELETEREQUEST._serialized_end=665
+  _DELETERESPONSE._serialized_start=667
+  _DELETERESPONSE._serialized_end=683
+  _FILEDOWNLOADREQUEST._serialized_start=686
+  _FILEDOWNLOADREQUEST._serialized_end=836
+  _FILEDOWNLOADRESPONSE._serialized_start=838
+  _FILEDOWNLOADRESPONSE._serialized_end=860
+  _LISTOBJECTSREQUEST._serialized_start=863
+  _LISTOBJECTSREQUEST._serialized_end=1001
+  _LISTOBJECTSRESPONSE._serialized_start=1003
+  _LISTOBJECTSRESPONSE._serialized_end=1038
+  _FILEUPLOADREQUEST._serialized_start=1041
+  _FILEUPLOADREQUEST._serialized_end=1173
+  _FILEUPLOADRESPONSE._serialized_start=1175
+  _FILEUPLOADRESPONSE._serialized_end=1195
+  _CREATEBUCKETREQUEST._serialized_start=1197
+  _CREATEBUCKETREQUEST._serialized_end=1304
+  _CREATEBUCKETRESPONSE._serialized_start=1306
+  _CREATEBUCKETRESPONSE._serialized_end=1328
+  _CLOUDPROXYSERVICE._serialized_start=1331
+  _CLOUDPROXYSERVICE._serialized_end=2675
 # @@protoc_insertion_point(module_scope)
```

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,28 +25,33 @@
                 response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.ListObjectsResponse.FromString,
                 )
         self.Upload = channel.unary_unary(
                 '/github.com.metaprov.modelaapi.services.cloudproxyd.v1.CloudProxyService/Upload',
                 request_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.FileUploadRequest.SerializeToString,
                 response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.FileUploadResponse.FromString,
                 )
-        self.KeyExistInVirtualBucket = channel.unary_unary(
-                '/github.com.metaprov.modelaapi.services.cloudproxyd.v1.CloudProxyService/KeyExistInVirtualBucket',
-                request_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.KeyExistInVirtualBucketRequest.SerializeToString,
-                response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.KeyExistInVirtualBucketResponse.FromString,
-                )
-        self.VirtualBucketExist = channel.unary_unary(
-                '/github.com.metaprov.modelaapi.services.cloudproxyd.v1.CloudProxyService/VirtualBucketExist',
-                request_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.VirtualBucketExistRequest.SerializeToString,
-                response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.VirtualBucketExistResponse.FromString,
-                )
-        self.CreateVirtualBucketIfNotExist = channel.unary_unary(
-                '/github.com.metaprov.modelaapi.services.cloudproxyd.v1.CloudProxyService/CreateVirtualBucketIfNotExist',
-                request_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.CreateVirtualBucketRequest.SerializeToString,
-                response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.CreateVirtualBucketResponse.FromString,
+        self.Delete = channel.unary_unary(
+                '/github.com.metaprov.modelaapi.services.cloudproxyd.v1.CloudProxyService/Delete',
+                request_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.DeleteRequest.SerializeToString,
+                response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.DeleteResponse.FromString,
+                )
+        self.ExistsInBucket = channel.unary_unary(
+                '/github.com.metaprov.modelaapi.services.cloudproxyd.v1.CloudProxyService/ExistsInBucket',
+                request_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.ExistsInBucketRequest.SerializeToString,
+                response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.ExistsInBucketResponse.FromString,
+                )
+        self.BucketExist = channel.unary_unary(
+                '/github.com.metaprov.modelaapi.services.cloudproxyd.v1.CloudProxyService/BucketExist',
+                request_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.BucketExistRequest.SerializeToString,
+                response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.BucketExistResponse.FromString,
+                )
+        self.CreateBucket = channel.unary_unary(
+                '/github.com.metaprov.modelaapi.services.cloudproxyd.v1.CloudProxyService/CreateBucket',
+                request_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.CreateBucketRequest.SerializeToString,
+                response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.CreateBucketResponse.FromString,
                 )
         self.Shutdown = channel.unary_unary(
                 '/github.com.metaprov.modelaapi.services.cloudproxyd.v1.CloudProxyService/Shutdown',
                 request_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.ShutdownRequest.SerializeToString,
                 response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.ShutdownResponse.FromString,
                 )
 
@@ -68,27 +73,33 @@
 
     def Upload(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def KeyExistInVirtualBucket(self, request, context):
+    def Delete(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def ExistsInBucket(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def VirtualBucketExist(self, request, context):
+    def BucketExist(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def CreateVirtualBucketIfNotExist(self, request, context):
+    def CreateBucket(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def Shutdown(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -110,28 +121,33 @@
                     response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.ListObjectsResponse.SerializeToString,
             ),
             'Upload': grpc.unary_unary_rpc_method_handler(
                     servicer.Upload,
                     request_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.FileUploadRequest.FromString,
                     response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.FileUploadResponse.SerializeToString,
             ),
-            'KeyExistInVirtualBucket': grpc.unary_unary_rpc_method_handler(
-                    servicer.KeyExistInVirtualBucket,
-                    request_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.KeyExistInVirtualBucketRequest.FromString,
-                    response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.KeyExistInVirtualBucketResponse.SerializeToString,
-            ),
-            'VirtualBucketExist': grpc.unary_unary_rpc_method_handler(
-                    servicer.VirtualBucketExist,
-                    request_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.VirtualBucketExistRequest.FromString,
-                    response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.VirtualBucketExistResponse.SerializeToString,
-            ),
-            'CreateVirtualBucketIfNotExist': grpc.unary_unary_rpc_method_handler(
-                    servicer.CreateVirtualBucketIfNotExist,
-                    request_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.CreateVirtualBucketRequest.FromString,
-                    response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.CreateVirtualBucketResponse.SerializeToString,
+            'Delete': grpc.unary_unary_rpc_method_handler(
+                    servicer.Delete,
+                    request_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.DeleteRequest.FromString,
+                    response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.DeleteResponse.SerializeToString,
+            ),
+            'ExistsInBucket': grpc.unary_unary_rpc_method_handler(
+                    servicer.ExistsInBucket,
+                    request_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.ExistsInBucketRequest.FromString,
+                    response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.ExistsInBucketResponse.SerializeToString,
+            ),
+            'BucketExist': grpc.unary_unary_rpc_method_handler(
+                    servicer.BucketExist,
+                    request_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.BucketExistRequest.FromString,
+                    response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.BucketExistResponse.SerializeToString,
+            ),
+            'CreateBucket': grpc.unary_unary_rpc_method_handler(
+                    servicer.CreateBucket,
+                    request_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.CreateBucketRequest.FromString,
+                    response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.CreateBucketResponse.SerializeToString,
             ),
             'Shutdown': grpc.unary_unary_rpc_method_handler(
                     servicer.Shutdown,
                     request_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.ShutdownRequest.FromString,
                     response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.ShutdownResponse.SerializeToString,
             ),
     }
@@ -192,61 +208,78 @@
         return grpc.experimental.unary_unary(request, target, '/github.com.metaprov.modelaapi.services.cloudproxyd.v1.CloudProxyService/Upload',
             github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.FileUploadRequest.SerializeToString,
             github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.FileUploadResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def KeyExistInVirtualBucket(request,
+    def Delete(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/github.com.metaprov.modelaapi.services.cloudproxyd.v1.CloudProxyService/Delete',
+            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.DeleteRequest.SerializeToString,
+            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.DeleteResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ExistsInBucket(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/github.com.metaprov.modelaapi.services.cloudproxyd.v1.CloudProxyService/KeyExistInVirtualBucket',
-            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.KeyExistInVirtualBucketRequest.SerializeToString,
-            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.KeyExistInVirtualBucketResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/github.com.metaprov.modelaapi.services.cloudproxyd.v1.CloudProxyService/ExistsInBucket',
+            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.ExistsInBucketRequest.SerializeToString,
+            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.ExistsInBucketResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def VirtualBucketExist(request,
+    def BucketExist(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/github.com.metaprov.modelaapi.services.cloudproxyd.v1.CloudProxyService/VirtualBucketExist',
-            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.VirtualBucketExistRequest.SerializeToString,
-            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.VirtualBucketExistResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/github.com.metaprov.modelaapi.services.cloudproxyd.v1.CloudProxyService/BucketExist',
+            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.BucketExistRequest.SerializeToString,
+            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.BucketExistResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def CreateVirtualBucketIfNotExist(request,
+    def CreateBucket(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/github.com.metaprov.modelaapi.services.cloudproxyd.v1.CloudProxyService/CreateVirtualBucketIfNotExist',
-            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.CreateVirtualBucketRequest.SerializeToString,
-            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.CreateVirtualBucketResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/github.com.metaprov.modelaapi.services.cloudproxyd.v1.CloudProxyService/CreateBucket',
+            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.CreateBucketRequest.SerializeToString,
+            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_cloudproxyd_dot_v1_dot_cloudproxyd__pb2.CreateBucketResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def Shutdown(request,
             target,
             options=(),
```

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_inference_dot_v1alpha1_dot_generated__pb2
 from github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_infra_dot_v1alpha1_dot_generated__pb2
 from github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_catalog_dot_v1alpha1_dot_generated__pb2
 from github.com.metaprov.modelaapi.services.common.v1 import common_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_common_dot_v1_dot_common__pb2
 from k8s.io.api.core.v1 import generated_pb2 as k8s_dot_io_dot_api_dot_core_dot_v1_dot_generated__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n9github.com/metaprov/modelaapi/services/data/v1/data.proto\x12.github.com.metaprov.modelaapi.services.data.v1\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1aHgithub.com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated.proto\x1aIgithub.com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated.proto\x1a\x45github.com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated.proto\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a=github.com/metaprov/modelaapi/services/common/v1/common.proto\x1a\"k8s.io/api/core/v1/generated.proto\"\xfd\x03\n\x11\x44sReadFileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12U\n\nconnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12]\n\x06secret\x18\x06 \x03(\x0b\x32M.github.com.metaprov.modelaapi.services.data.v1.DsReadFileRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x83\x04\n\x14\x44sReadFeatureRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\x06\x62ucket\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x05 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12`\n\x06secret\x18\x06 \x03(\x0b\x32P.github.com.metaprov.modelaapi.services.data.v1.DsReadFeatureRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xcf\x04\n\x12\x44sWriteFileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x07\x63ontent\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12^\n\x06secret\x18\x07 \x03(\x0b\x32N.github.com.metaprov.modelaapi.services.data.v1.DsWriteFileRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xd0\x02\n\x12\x44sReadAudioRequest\x12T\n\x06\x62ucket\x18\x01 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12^\n\x06secret\x18\x03 \x03(\x0b\x32N.github.com.metaprov.modelaapi.services.data.v1.DsReadAudioRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x89\x04\n\x17\x44sReadTextCorpusRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x63\n\x06secret\x18\x05 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.DsReadTextCorpusRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xd8\x04\n\x17\x44sReadFromStoreResponse\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12M\n\x06result\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x05 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x63\n\x06secret\x18\x06 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"p\n\x18\x44sRunDataPipelineRequest\x12T\n\x08pipeline\x18\x01 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipeline\"j\n\x19\x44sRunDataPipelineResponse\x12M\n\x06result\x18\x01 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"\xd1\x08\n\x12\x44sRunRecipeRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\\\n\x11storageConnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12l\n\rstorageSecret\x18\x07 \x03(\x0b\x32U.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x08 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x62\n\x08\x64\x62Secret\x18\t \x03(\x0b\x32P.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeRequest.DbSecretEntry\x12L\n\x06recipe\x18\n \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Recipe\x12R\n\treciperun\x18\x0b \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeRun\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"c\n\x13\x44sRunRecipeResponse\x12L\n\x06result\x18\x01 \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Recipe\"\x9b\x08\n\x1c\x44sCreateRecipeProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\\\n\x11storageConnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12v\n\rstorageSecret\x18\x07 \x03(\x0b\x32_.github.com.metaprov.modelaapi.services.data.v1.DsCreateRecipeProfileRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x08 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12l\n\x08\x64\x62Secret\x18\t \x03(\x0b\x32Z.github.com.metaprov.modelaapi.services.data.v1.DsCreateRecipeProfileRequest.DbSecretEntry\x12L\n\x06recipe\x18\n \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Recipe\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"l\n\x1d\x44sCreateRecipeProfileResponse\x12K\n\x06result\x18\x01 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\"\x14\n\x12\x44\x61taSourceResponse\"\x11\n\x0f\x44\x61tasetResponse\"\xf4\x02\n\x1d\x44sCreateDatasetProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"\xb3\x02\n\x1e\x44sCreateDatasetProfileResponse\x12Q\n\x07profile\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.services.common.v1.DatasetProfile\x12^\n\x0fprofileLocation\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12^\n\x0f\x61nomalyLocation\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\xce\x08\n\x1b\x44sCreateModelProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12U\n\nconnection\x18\x08 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\t \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12g\n\x06secret\x18\n \x03(\x0b\x32W.github.com.metaprov.modelaapi.services.data.v1.DsCreateModelProfileRequest.SecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x0b \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12k\n\x08\x64\x62Secret\x18\x0c \x03(\x0b\x32Y.github.com.metaprov.modelaapi.services.data.v1.DsCreateModelProfileRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"+\n\x1c\x44sCreateModelProfileResponse\x12\x0b\n\x03uri\x18\x01 \x01(\t\"\xde\x08\n\x1a\x44sMergeForecastFileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12U\n\nconnection\x18\x08 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\t \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x66\n\x06secret\x18\n \x03(\x0b\x32V.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileRequest.SecretEntry\x12\x11\n\tforecasts\x18\x0b \x03(\t\x12W\n\x0c\x64\x62\x43onnection\x18\x0c \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12j\n\x08\x64\x62Secret\x18\r \x03(\x0b\x32X.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"*\n\x1b\x44sMergeForecastFileResponse\x12\x0b\n\x03uri\x18\x01 \x01(\t\"\xcf\x08\n\x1b\x44sCreateStudyProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x05study\x18\x04 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12U\n\nconnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12O\n\x06models\x18\x08 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12g\n\x06secret\x18\t \x03(\x0b\x32W.github.com.metaprov.modelaapi.services.data.v1.DsCreateStudyProfileRequest.SecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\n \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12k\n\x08\x64\x62Secret\x18\x0b \x03(\x0b\x32Y.github.com.metaprov.modelaapi.services.data.v1.DsCreateStudyProfileRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"+\n\x1c\x44sCreateStudyProfileResponse\x12\x0b\n\x03uri\x18\x01 \x01(\t\"\xc3\x07\n\x13RunTestSuiteRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12U\n\nconnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x08 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12Y\n\thistogram\x18\t \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogram\x12\\\n\x0crefHistogram\x18\n \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogram\x12Q\n\x05suite\x18\x0b \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\"p\n\x14RunTestSuiteResponse\x12X\n\x06result\x18\x01 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\"\xba\x07\n\x18\x44sGenerateDatasetRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12U\n\nconnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x64\n\x06secret\x18\x06 \x03(\x0b\x32T.github.com.metaprov.modelaapi.services.data.v1.DsGenerateDatasetRequest.SecretEntry\x12\x0c\n\x04rows\x18\x07 \x01(\x05\x12W\n\x0c\x64\x62\x43onnection\x18\x08 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12h\n\x08\x64\x62Secret\x18\t \x03(\x0b\x32V.github.com.metaprov.modelaapi.services.data.v1.DsGenerateDatasetRequest.DbSecretEntry\x12U\n\x06target\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"r\n\x19\x44sGenerateDatasetResponse\x12U\n\x06target\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\xaa\t\n\x15\x44sSplitDatasetRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12U\n\nconnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x61\n\x06secret\x18\x08 \x03(\x0b\x32Q.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetRequest.SecretEntry\x12V\n\x0ftrainingDataset\x18\t \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12U\n\x0etestingDataset\x18\n \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12\r\n\x05group\x18\x0b \x01(\x08\x12W\n\x0c\x64\x62\x43onnection\x18\x0c \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x65\n\x08\x64\x62Secret\x18\r \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xa8\x01\n\x16\x44sSplitDatasetResponse\x12\x10\n\x08training\x18\x01 \x01(\x05\x12\x0f\n\x07testing\x18\x02 \x01(\x05\x12\x12\n\nvalidation\x18\x03 \x01(\x05\x12\x15\n\rtraining_hash\x18\x04 \x01(\t\x12\x14\n\x0ctesting_hash\x18\x05 \x01(\t\x12\x17\n\x0fvalidation_hash\x18\x06 \x01(\t\x12\x11\n\tindexFile\x18\x07 \x01(\t\"\xc8\x05\n\x1c\x44sSplitDatasetToRungsRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12U\n\nconnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12h\n\x06secret\x18\x07 \x03(\x0b\x32X.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetToRungsRequest.SecretEntry\x12\r\n\x05rungs\x18\x08 \x01(\x05\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x1f\n\x1d\x44sSplitDatasetToRungsResponse\"\xa4\x07\n\x12\x44sTransformRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12U\n\nconnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12^\n\x06secret\x18\x08 \x03(\x0b\x32N.github.com.metaprov.modelaapi.services.data.v1.DsTransformRequest.SecretEntry\x12V\n\x0ftrainingDataset\x18\t \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12U\n\x0etestingDataset\x18\n \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"[\n\x13\x44sTransformResponse\x12\x15\n\rtraining_hash\x18\x04 \x01(\t\x12\x14\n\x0ctesting_hash\x18\x05 \x01(\t\x12\x17\n\x0fvalidation_hash\x18\x06 \x01(\t\"\xd9\x07\n\x1c\x44sCreateColumnProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12h\n\x06secret\x18\x07 \x03(\x0b\x32X.github.com.metaprov.modelaapi.services.data.v1.DsCreateColumnProfileRequest.SecretEntry\x12\x12\n\ncolumnType\x18\x08 \x01(\t\x12\x12\n\ncolumnName\x18\t \x01(\t\x12W\n\x0c\x64\x62\x43onnection\x18\n \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12l\n\x08\x64\x62Secret\x18\x0b \x03(\x0b\x32Z.github.com.metaprov.modelaapi.services.data.v1.DsCreateColumnProfileRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"s\n\x1d\x44sCreateColumnProfileResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x44\n\x04plot\x18\x02 \x01(\x0b\x32\x36.github.com.metaprov.modelaapi.services.common.v1.Plot\"\x9c\x07\n\x15GroupByDatasetRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12U\n\nconnection\x18\x05 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x61\n\x06secret\x18\x07 \x03(\x0b\x32Q.github.com.metaprov.modelaapi.services.data.v1.GroupByDatasetRequest.SecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x08 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x65\n\x08\x64\x62Secret\x18\t \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.GroupByDatasetRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"%\n\x16GroupByDatasetResponse\x12\x0b\n\x03uri\x18\x01 \x01(\t\"\xd5\x01\n\x14\x44sInferSchemaRequest\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12\x0e\n\x06tenant\x18\x03 \x01(\t\"j\n\x15\x44sInferSchemaResponse\x12Q\n\x07profile\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.services.common.v1.DatasetProfile\"\xdc\x01\n\x15\x44sGetTableViewRequest\x12Z\n\x08\x66latfile\x18\x01 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\x12W\n\x08location\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x0e\n\x06tenant\x18\x03 \x01(\t\"h\n\x16\x44sGetTableViewResponse\x12N\n\ttableview\x18\x01 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\"\xe1\x04\n\x18\x43reateModelReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\ndatasource\x18\x05 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12P\n\x06report\x18\x07 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xb2\t\n\x1b\x43reateForecastReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\ndatasource\x18\x05 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12Q\n\x08\x66orecast\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12U\n\nconnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12g\n\x06secret\x18\x08 \x03(\x0b\x32W.github.com.metaprov.modelaapi.services.data.v1.CreateForecastReportRequest.SecretEntry\x12T\n\x06\x62ucket\x18\t \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12P\n\x06report\x18\n \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\x12\r\n\x05group\x18\x0b \x01(\x08\x12W\n\x0c\x64\x62\x43onnection\x18\x0c \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12k\n\x08\x64\x62Secret\x18\r \x03(\x0b\x32Y.github.com.metaprov.modelaapi.services.data.v1.CreateForecastReportRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xd7\x06\n\x1a\x43reateSummaryReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12U\n\nconnection\x18\x03 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x66\n\x06secret\x18\x04 \x03(\x0b\x32V.github.com.metaprov.modelaapi.services.data.v1.CreateSummaryReportRequest.SecretEntry\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12P\n\x06report\x18\x06 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\x12W\n\x0c\x64\x62\x43onnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12j\n\x08\x64\x62Secret\x18\x08 \x03(\x0b\x32X.github.com.metaprov.modelaapi.services.data.v1.CreateSummaryReportRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"#\n\x14\x43reateReportResponse\x12\x0b\n\x03pdf\x18\x01 \x01(\x0c\"\xc3\x03\n\x1a\x43reateDatasetReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12P\n\x06report\x18\x05 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xe6\x04\n\x18\x43reateStudyReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\ndatasource\x18\x05 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12S\n\x06models\x18\x06 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelList\x12P\n\x06report\x18\x07 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xc4\x04\n\x0f\x41skModelRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12\x0e\n\x06\x62udget\x18\x06 \x01(\x05\x12\x11\n\tdefaultHP\x18\x07 \x01(\x08\x12\x11\n\talgorithm\x18\x08 \x01(\t\x12V\n\nalgorithms\x18\t \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"\xc6\x03\n\x1fGetTimeSeriesDatasetKeysRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"0\n GetTimeSeriesDatasetKeysResponse\x12\x0c\n\x04keys\x18\x01 \x03(\t\"\xa4\x04\n\x17\x41skForecastModelRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12\x0c\n\x04keys\x18\x06 \x03(\t\x12V\n\nalgorithms\x18\x07 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"j\n\x18\x41skForecastModelResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xe2\x04\n\x12\x41skEnsembleRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12O\n\x06models\x18\x06 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12V\n\nalgorithms\x18\x07 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"e\n\x13\x41skEnsembleResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xb0\x04\n\x12\x41skBaselineRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12\x10\n\x08\x61lgnames\x18\x06 \x03(\t\x12\x0b\n\x03\x61ll\x18\x07 \x01(\x08\x12V\n\nalgorithms\x18\x08 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"e\n\x13\x41skBaselineResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xb7\x04\n\x1a\x41skAllModelsForTaskRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12\x0e\n\x06\x62udget\x18\x06 \x01(\x05\x12\x0c\n\x04task\x18\x07 \x01(\t\x12V\n\nalgorithms\x18\x08 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"m\n\x1b\x41skAllModelsForTaskResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\x97\x04\n\x10TellModelRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12\x0e\n\x06\x66\x61iled\x18\x07 \x01(\x08\"#\n\x11TellModelResponse\x12\x0e\n\x06pruned\x18\x01 \x01(\x08\"\x13\n\x11\x44sShutdownRequest\"\x14\n\x12\x44sShutdownResponse\"\xda\x02\n\x17\x44sTestConnectionRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x63\n\x06secret\x18\x03 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.DsTestConnectionRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"7\n\x18\x44sTestConnectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x08\x12\x0b\n\x03msg\x18\x02 \x01(\t\"\xf7\x05\n\x13\x44sStudyEndedRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12U\n\nconnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12_\n\x06secret\x18\x08 \x03(\x0b\x32O.github.com.metaprov.modelaapi.services.data.v1.DsStudyEndedRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x16\n\x14\x44sStudyEndedResponse\"\xfd\x05\n\x16SaveOptimizerDBRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12U\n\nconnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x62\n\x06secret\x18\x08 \x03(\x0b\x32R.github.com.metaprov.modelaapi.services.data.v1.SaveOptimizerDBRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x19\n\x17SaveOptimizerDBResponse\"n\n\x15\x44sGetDatabasesRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"+\n\x16\x44sGetDatabasesResponse\x12\x11\n\tdatabases\x18\x01 \x03(\t\"k\n\x12\x44sGetTablesRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"%\n\x13\x44sGetTablesResponse\x12\x0e\n\x06tables\x18\x01 \x03(\t\"y\n\x13\x44sExecuteSqlRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x0b\n\x03sql\x18\x04 \x01(\t\"f\n\x14\x44sExecuteSqlResponse\x12N\n\ttableview\x18\x01 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\"\xe8\x02\n\x11\x44sSnapshotRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"\x14\n\x12\x44sSnapshotResponse\"b\n\x10\x41skModelResponse\x12N\n\x05model\x18\x01 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\x95\x08\n\x16GenTrainingDataRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12\\\n\x11storageConnection\x18\x03 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12p\n\rstorageSecret\x18\x05 \x03(\x0b\x32Y.github.com.metaprov.modelaapi.services.data.v1.GenTrainingDataRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x66\n\x08\x64\x62Secret\x18\x07 \x03(\x0b\x32T.github.com.metaprov.modelaapi.services.data.v1.GenTrainingDataRequest.DbSecretEntry\x12S\n\x05model\x18\x08 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x08\x65ntities\x18\t \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Entity\x12R\n\x06groups\x18\n \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\'\n\x17GenTrainingDataResponse\x12\x0c\n\x04path\x18\x01 \x01(\t\"\xeb\x06\n\x16SyncOnlineStoreRequest\x12\\\n\x11storageConnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12p\n\rstorageSecret\x18\x03 \x03(\x0b\x32Y.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x66\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32T.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreRequest.DbSecretEntry\x12S\n\x05model\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x02\x66g\x18\x07 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12W\n\x08location\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x19\n\x17SyncOnlineStoreResponse\"\xfd\x06\n\x1cGenOnlineStoreDatasetRequest\x12\\\n\x11storageConnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12v\n\rstorageSecret\x18\x03 \x03(\x0b\x32_.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12l\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32Z.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetRequest.DbSecretEntry\x12S\n\x05model\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x02\x66g\x18\x07 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12W\n\x08location\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"x\n\x1dGenOnlineStoreDatasetResponse\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\x8d\x08\n\x13\x42\x61tchPredictRequest\x12\\\n\x11storageConnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12m\n\rstorageSecret\x18\x03 \x03(\x0b\x32V.github.com.metaprov.modelaapi.services.data.v1.BatchPredictRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x63\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32Q.github.com.metaprov.modelaapi.services.data.v1.BatchPredictRequest.DbSecretEntry\x12X\n\nmodelclass\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x05model\x18\x07 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12N\n\x08\x65ntities\x18\x08 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Entity\x12R\n\x06groups\x18\t \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12Y\n\nprediction\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"$\n\x14\x42\x61tchPredictResponse\x12\x0c\n\x04rows\x18\x01 \x01(\x05\"\xba\x05\n\x12SaveDatasetRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12X\n\nmodelclass\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelclassrun\x18\x05 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12W\n\x0c\x64\x62\x43onnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x62\n\x08\x64\x62Secret\x18\x07 \x03(\x0b\x32P.github.com.metaprov.modelaapi.services.data.v1.SaveDatasetRequest.DbSecretEntry\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x84\x06\n\x10SaveModelRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12X\n\nmodelclass\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelclassrun\x18\x04 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12N\n\x05model\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12R\n\x06groups\x18\x06 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12W\n\x0c\x64\x62\x43onnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12`\n\x08\x64\x62Secret\x18\x08 \x03(\x0b\x32N.github.com.metaprov.modelaapi.services.data.v1.SaveModelRequest.DbSecretEntry\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xce\x05\n\x15SavePredictionRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12X\n\nmodelclass\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelclassrun\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12W\n\tpredictor\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Predictor\x12Y\n\nprediction\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\x12W\n\x0c\x64\x62\x43onnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x65\n\x08\x64\x62Secret\x18\x07 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.SavePredictionRequest.DbSecretEntry\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x92\x04\n\x14SavePredictorRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12X\n\nmodelclass\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12X\n\tpredictor\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x64\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32R.github.com.metaprov.modelaapi.services.data.v1.SavePredictorRequest.DbSecretEntry\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x84\x01\n\x19\x43reateMetricsStoreRequest\x12\x0e\n\x06tenant\x18\x01 \x01(\t\x12W\n\x0c\x64\x62\x43onnection\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\x1c\n\x1a\x43reateMetricsStoreResponse\"\x1c\n\x0cSaveResponse\x12\x0c\n\x04\x64\x62id\x18\x01 \x01(\x05\x32\xf7\x43\n\x0b\x44\x61taService\x12\x98\x01\n\x08ReadFile\x12\x41.github.com.metaprov.modelaapi.services.data.v1.DsReadFileRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\x9e\x01\n\x0bReadFeature\x12\x44.github.com.metaprov.modelaapi.services.data.v1.DsReadFeatureRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\x9a\x01\n\tReadAudio\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsReadAudioRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\xa8\x01\n\x0fRunDataPipeline\x12H.github.com.metaprov.modelaapi.services.data.v1.DsRunDataPipelineRequest\x1aI.github.com.metaprov.modelaapi.services.data.v1.DsRunDataPipelineResponse\"\x00\x12\x96\x01\n\tRunRecipe\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeResponse\"\x00\x12\x9a\x01\n\tWriteFile\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsWriteFileRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\xa8\x01\n\x0fGenerateDataset\x12H.github.com.metaprov.modelaapi.services.data.v1.DsGenerateDatasetRequest\x1aI.github.com.metaprov.modelaapi.services.data.v1.DsGenerateDatasetResponse\"\x00\x12\x9f\x01\n\x0cSplitDataset\x12\x45.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetResponse\"\x00\x12\x96\x01\n\tTransform\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsTransformRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.DsTransformResponse\"\x00\x12\xb4\x01\n\x13\x43reateColumnProfile\x12L.github.com.metaprov.modelaapi.services.data.v1.DsCreateColumnProfileRequest\x1aM.github.com.metaprov.modelaapi.services.data.v1.DsCreateColumnProfileResponse\"\x00\x12\x9c\x01\n\x0bInferSchema\x12\x44.github.com.metaprov.modelaapi.services.data.v1.DsInferSchemaRequest\x1a\x45.github.com.metaprov.modelaapi.services.data.v1.DsInferSchemaResponse\"\x00\x12\x9f\x01\n\x0cGetTableView\x12\x45.github.com.metaprov.modelaapi.services.data.v1.DsGetTableViewRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.DsGetTableViewResponse\"\x00\x12\xb4\x01\n\x13SplitDatasetToRungs\x12L.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetToRungsRequest\x1aM.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetToRungsResponse\"\x00\x12\xb7\x01\n\x14\x43reateDatasetProfile\x12M.github.com.metaprov.modelaapi.services.data.v1.DsCreateDatasetProfileRequest\x1aN.github.com.metaprov.modelaapi.services.data.v1.DsCreateDatasetProfileResponse\"\x00\x12\xb1\x01\n\x12\x43reateModelProfile\x12K.github.com.metaprov.modelaapi.services.data.v1.DsCreateModelProfileRequest\x1aL.github.com.metaprov.modelaapi.services.data.v1.DsCreateModelProfileResponse\"\x00\x12\xb1\x01\n\x12\x43reateStudyProfile\x12K.github.com.metaprov.modelaapi.services.data.v1.DsCreateStudyProfileRequest\x1aL.github.com.metaprov.modelaapi.services.data.v1.DsCreateStudyProfileResponse\"\x00\x12\xb4\x01\n\x13\x43reateRecipeProfile\x12L.github.com.metaprov.modelaapi.services.data.v1.DsCreateRecipeProfileRequest\x1aM.github.com.metaprov.modelaapi.services.data.v1.DsCreateRecipeProfileResponse\"\x00\x12\xa5\x01\n\x11\x43reateModelReport\x12H.github.com.metaprov.modelaapi.services.data.v1.CreateModelReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xa5\x01\n\x11\x43reateStudyReport\x12H.github.com.metaprov.modelaapi.services.data.v1.CreateStudyReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xa9\x01\n\x13\x43reateDatasetReport\x12J.github.com.metaprov.modelaapi.services.data.v1.CreateDatasetReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xab\x01\n\x14\x43reateForecastReport\x12K.github.com.metaprov.modelaapi.services.data.v1.CreateForecastReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xa9\x01\n\x13\x43reateSummaryReport\x12J.github.com.metaprov.modelaapi.services.data.v1.CreateSummaryReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\x8c\x01\n\x05\x41skFE\x12?.github.com.metaprov.modelaapi.services.data.v1.AskModelRequest\x1a@.github.com.metaprov.modelaapi.services.data.v1.AskModelResponse\"\x00\x12\x98\x01\n\x0b\x41skBaseline\x12\x42.github.com.metaprov.modelaapi.services.data.v1.AskBaselineRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.AskBaselineResponse\"\x00\x12\x98\x01\n\x0b\x41skEnsemble\x12\x42.github.com.metaprov.modelaapi.services.data.v1.AskEnsembleRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.AskEnsembleResponse\"\x00\x12\xa7\x01\n\x10\x41skForecastModel\x12G.github.com.metaprov.modelaapi.services.data.v1.AskForecastModelRequest\x1aH.github.com.metaprov.modelaapi.services.data.v1.AskForecastModelResponse\"\x00\x12\x8f\x01\n\x08\x41skModel\x12?.github.com.metaprov.modelaapi.services.data.v1.AskModelRequest\x1a@.github.com.metaprov.modelaapi.services.data.v1.AskModelResponse\"\x00\x12\xb0\x01\n\x13\x41skAllModelsForTask\x12J.github.com.metaprov.modelaapi.services.data.v1.AskAllModelsForTaskRequest\x1aK.github.com.metaprov.modelaapi.services.data.v1.AskAllModelsForTaskResponse\"\x00\x12\x99\x01\n\x10TellPartialModel\x12@.github.com.metaprov.modelaapi.services.data.v1.TellModelRequest\x1a\x41.github.com.metaprov.modelaapi.services.data.v1.TellModelResponse\"\x00\x12\x92\x01\n\tTellModel\x12@.github.com.metaprov.modelaapi.services.data.v1.TellModelRequest\x1a\x41.github.com.metaprov.modelaapi.services.data.v1.TellModelResponse\"\x00\x12\xae\x01\n\x11MergeForecastFile\x12J.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileRequest\x1aK.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileResponse\"\x00\x12\xa7\x01\n\x10\x44sTestConnection\x12G.github.com.metaprov.modelaapi.services.data.v1.DsTestConnectionRequest\x1aH.github.com.metaprov.modelaapi.services.data.v1.DsTestConnectionResponse\"\x00\x12\x93\x01\n\x08ShutDown\x12\x41.github.com.metaprov.modelaapi.services.data.v1.DsShutdownRequest\x1a\x42.github.com.metaprov.modelaapi.services.data.v1.DsShutdownResponse\"\x00\x12\x99\x01\n\nStudyEnded\x12\x43.github.com.metaprov.modelaapi.services.data.v1.DsStudyEndedRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.DsStudyEndedResponse\"\x00\x12\xa4\x01\n\x0fSaveOptimizerDB\x12\x46.github.com.metaprov.modelaapi.services.data.v1.SaveOptimizerDBRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.SaveOptimizerDBResponse\"\x00\x12\x9f\x01\n\x0cGetDatabases\x12\x45.github.com.metaprov.modelaapi.services.data.v1.DsGetDatabasesRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.DsGetDatabasesResponse\"\x00\x12\x96\x01\n\tGetTables\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsGetTablesRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.DsGetTablesResponse\"\x00\x12\x99\x01\n\nExecuteSql\x12\x43.github.com.metaprov.modelaapi.services.data.v1.DsExecuteSqlRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.DsExecuteSqlResponse\"\x00\x12\x93\x01\n\x08Snapshot\x12\x41.github.com.metaprov.modelaapi.services.data.v1.DsSnapshotRequest\x1a\x42.github.com.metaprov.modelaapi.services.data.v1.DsSnapshotResponse\"\x00\x12\x9e\x01\n\x0fUnitTestDataset\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\x9c\x01\n\rUnitTestModel\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\x9f\x01\n\x10UnitTestFeedback\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\xa7\x01\n\x18UnitTestFeatureHistogram\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\xa0\x01\n\x11UnitTestPredictor\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\xa1\x01\n\x0eGroupByDataset\x12\x45.github.com.metaprov.modelaapi.services.data.v1.GroupByDatasetRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.GroupByDatasetResponse\"\x00\x12\xa4\x01\n\x0fSyncOnlineStore\x12\x46.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreResponse\"\x00\x12\xa4\x01\n\x0fGenTrainingData\x12\x46.github.com.metaprov.modelaapi.services.data.v1.GenTrainingDataRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.GenTrainingDataResponse\"\x00\x12\xb6\x01\n\x15GenOnlineStoreDataset\x12L.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetRequest\x1aM.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetResponse\"\x00\x12\x9b\x01\n\x0c\x42\x61tchPredict\x12\x43.github.com.metaprov.modelaapi.services.data.v1.BatchPredictRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.BatchPredictResponse\"\x00\x12\x91\x01\n\x0bSaveDataSet\x12\x42.github.com.metaprov.modelaapi.services.data.v1.SaveDatasetRequest\x1a<.github.com.metaprov.modelaapi.services.data.v1.SaveResponse\"\x00\x12\x8d\x01\n\tSaveModel\x12@.github.com.metaprov.modelaapi.services.data.v1.SaveModelRequest\x1a<.github.com.metaprov.modelaapi.services.data.v1.SaveResponse\"\x00\x12\x97\x01\n\x0eSavePrediction\x12\x45.github.com.metaprov.modelaapi.services.data.v1.SavePredictionRequest\x1a<.github.com.metaprov.modelaapi.services.data.v1.SaveResponse\"\x00\x12\xad\x01\n\x12\x43reateMetricsStore\x12I.github.com.metaprov.modelaapi.services.data.v1.CreateMetricsStoreRequest\x1aJ.github.com.metaprov.modelaapi.services.data.v1.CreateMetricsStoreResponse\"\x00\x42\x30Z.github.com/metaprov/modelaapi/services/data/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n9github.com/metaprov/modelaapi/services/data/v1/data.proto\x12.github.com.metaprov.modelaapi.services.data.v1\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1aHgithub.com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated.proto\x1aIgithub.com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated.proto\x1a\x45github.com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated.proto\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a=github.com/metaprov/modelaapi/services/common/v1/common.proto\x1a\"k8s.io/api/core/v1/generated.proto\"\xfd\x03\n\x11\x44sReadFileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12U\n\nconnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12]\n\x06secret\x18\x06 \x03(\x0b\x32M.github.com.metaprov.modelaapi.services.data.v1.DsReadFileRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x83\x04\n\x14\x44sReadFeatureRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\x06\x62ucket\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x05 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12`\n\x06secret\x18\x06 \x03(\x0b\x32P.github.com.metaprov.modelaapi.services.data.v1.DsReadFeatureRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xcf\x04\n\x12\x44sWriteFileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x07\x63ontent\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12^\n\x06secret\x18\x07 \x03(\x0b\x32N.github.com.metaprov.modelaapi.services.data.v1.DsWriteFileRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xd0\x02\n\x12\x44sReadAudioRequest\x12T\n\x06\x62ucket\x18\x01 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12^\n\x06secret\x18\x03 \x03(\x0b\x32N.github.com.metaprov.modelaapi.services.data.v1.DsReadAudioRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x89\x04\n\x17\x44sReadTextCorpusRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x63\n\x06secret\x18\x05 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.DsReadTextCorpusRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xd8\x04\n\x17\x44sReadFromStoreResponse\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12M\n\x06result\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x05 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x63\n\x06secret\x18\x06 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"p\n\x18\x44sRunDataPipelineRequest\x12T\n\x08pipeline\x18\x01 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipeline\"j\n\x19\x44sRunDataPipelineResponse\x12M\n\x06result\x18\x01 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"\xd1\x08\n\x12\x44sRunRecipeRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\\\n\x11storageConnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12l\n\rstorageSecret\x18\x07 \x03(\x0b\x32U.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x08 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x62\n\x08\x64\x62Secret\x18\t \x03(\x0b\x32P.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeRequest.DbSecretEntry\x12L\n\x06recipe\x18\n \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Recipe\x12R\n\treciperun\x18\x0b \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeRun\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"c\n\x13\x44sRunRecipeResponse\x12L\n\x06result\x18\x01 \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Recipe\"\x9b\x08\n\x1c\x44sCreateRecipeProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\\\n\x11storageConnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12v\n\rstorageSecret\x18\x07 \x03(\x0b\x32_.github.com.metaprov.modelaapi.services.data.v1.DsCreateRecipeProfileRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x08 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12l\n\x08\x64\x62Secret\x18\t \x03(\x0b\x32Z.github.com.metaprov.modelaapi.services.data.v1.DsCreateRecipeProfileRequest.DbSecretEntry\x12L\n\x06recipe\x18\n \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Recipe\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"l\n\x1d\x44sCreateRecipeProfileResponse\x12K\n\x06result\x18\x01 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\"\x14\n\x12\x44\x61taSourceResponse\"\x11\n\x0f\x44\x61tasetResponse\"\xca\x03\n\x1d\x44sCreateDatasetProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\"\xb3\x02\n\x1e\x44sCreateDatasetProfileResponse\x12Q\n\x07profile\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.services.common.v1.DatasetProfile\x12^\n\x0fprofileLocation\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12^\n\x0f\x61nomalyLocation\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\xe8\x04\n\x1b\x44sCreateModelProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12T\n\x06\x62ucket\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\"~\n\x1c\x44sCreateModelProfileResponse\x12^\n\x0fprofileLocation\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\xde\x08\n\x1a\x44sMergeForecastFileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12U\n\nconnection\x18\x08 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\t \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x66\n\x06secret\x18\n \x03(\x0b\x32V.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileRequest.SecretEntry\x12\x11\n\tforecasts\x18\x0b \x03(\t\x12W\n\x0c\x64\x62\x43onnection\x18\x0c \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12j\n\x08\x64\x62Secret\x18\r \x03(\x0b\x32X.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"*\n\x1b\x44sMergeForecastFileResponse\x12\x0b\n\x03uri\x18\x01 \x01(\t\"\xe9\x04\n\x1b\x44sCreateStudyProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\x06\x62ucket\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12O\n\x06models\x18\x07 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"~\n\x1c\x44sCreateStudyProfileResponse\x12^\n\x0fprofileLocation\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\xc3\x07\n\x13RunTestSuiteRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12U\n\nconnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x08 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12Y\n\thistogram\x18\t \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogram\x12\\\n\x0crefHistogram\x18\n \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogram\x12Q\n\x05suite\x18\x0b \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\"p\n\x14RunTestSuiteResponse\x12X\n\x06result\x18\x01 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\"\xba\x07\n\x18\x44sGenerateDatasetRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12U\n\nconnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x64\n\x06secret\x18\x06 \x03(\x0b\x32T.github.com.metaprov.modelaapi.services.data.v1.DsGenerateDatasetRequest.SecretEntry\x12\x0c\n\x04rows\x18\x07 \x01(\x05\x12W\n\x0c\x64\x62\x43onnection\x18\x08 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12h\n\x08\x64\x62Secret\x18\t \x03(\x0b\x32V.github.com.metaprov.modelaapi.services.data.v1.DsGenerateDatasetRequest.DbSecretEntry\x12U\n\x06target\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"r\n\x19\x44sGenerateDatasetResponse\x12U\n\x06target\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\xc1\x05\n\x15\x44sSplitDatasetRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\x06\x62ucket\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12V\n\x0ftrainingDataset\x18\x07 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12U\n\x0etestingDataset\x18\x08 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"\xc3\x03\n\x16\x44sSplitDatasetResponse\x12\x10\n\x08training\x18\x01 \x01(\x05\x12\x0f\n\x07testing\x18\x02 \x01(\x05\x12\x12\n\nvalidation\x18\x03 \x01(\x05\x12\x14\n\x0ctrainingHash\x18\x04 \x01(\t\x12\x13\n\x0btestingHash\x18\x05 \x01(\t\x12\x16\n\x0evalidationHash\x18\x06 \x01(\t\x12\x11\n\tindexFile\x18\x07 \x01(\t\x12\\\n\rtrainLocation\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12[\n\x0ctestLocation\x18\t \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x61\n\x12validationLocation\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\xd8\x03\n\x1c\x44sSplitDatasetToRungsRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\r\n\x05rungs\x18\x06 \x01(\x05\"\x1f\n\x1d\x44sSplitDatasetToRungsResponse\"\xa4\x07\n\x12\x44sTransformRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12U\n\nconnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12^\n\x06secret\x18\x08 \x03(\x0b\x32N.github.com.metaprov.modelaapi.services.data.v1.DsTransformRequest.SecretEntry\x12V\n\x0ftrainingDataset\x18\t \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12U\n\x0etestingDataset\x18\n \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"[\n\x13\x44sTransformResponse\x12\x15\n\rtraining_hash\x18\x04 \x01(\t\x12\x14\n\x0ctesting_hash\x18\x05 \x01(\t\x12\x17\n\x0fvalidation_hash\x18\x06 \x01(\t\"\xd9\x07\n\x1c\x44sCreateColumnProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12h\n\x06secret\x18\x07 \x03(\x0b\x32X.github.com.metaprov.modelaapi.services.data.v1.DsCreateColumnProfileRequest.SecretEntry\x12\x12\n\ncolumnType\x18\x08 \x01(\t\x12\x12\n\ncolumnName\x18\t \x01(\t\x12W\n\x0c\x64\x62\x43onnection\x18\n \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12l\n\x08\x64\x62Secret\x18\x0b \x03(\x0b\x32Z.github.com.metaprov.modelaapi.services.data.v1.DsCreateColumnProfileRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"s\n\x1d\x44sCreateColumnProfileResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x44\n\x04plot\x18\x02 \x01(\x0b\x32\x36.github.com.metaprov.modelaapi.services.common.v1.Plot\"\x9c\x07\n\x15GroupByDatasetRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12U\n\nconnection\x18\x05 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x61\n\x06secret\x18\x07 \x03(\x0b\x32Q.github.com.metaprov.modelaapi.services.data.v1.GroupByDatasetRequest.SecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x08 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x65\n\x08\x64\x62Secret\x18\t \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.GroupByDatasetRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"%\n\x16GroupByDatasetResponse\x12\x0b\n\x03uri\x18\x01 \x01(\t\"\xd5\x01\n\x14\x44sInferSchemaRequest\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12\x0e\n\x06tenant\x18\x03 \x01(\t\"j\n\x15\x44sInferSchemaResponse\x12Q\n\x07profile\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.services.common.v1.DatasetProfile\"\xdc\x01\n\x15\x44sGetTableViewRequest\x12Z\n\x08\x66latfile\x18\x01 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\x12W\n\x08location\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x0e\n\x06tenant\x18\x03 \x01(\t\"h\n\x16\x44sGetTableViewResponse\x12N\n\ttableview\x18\x01 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\"\xe1\x04\n\x18\x43reateModelReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\ndatasource\x18\x05 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12P\n\x06report\x18\x07 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xb2\t\n\x1b\x43reateForecastReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\ndatasource\x18\x05 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12Q\n\x08\x66orecast\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12U\n\nconnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12g\n\x06secret\x18\x08 \x03(\x0b\x32W.github.com.metaprov.modelaapi.services.data.v1.CreateForecastReportRequest.SecretEntry\x12T\n\x06\x62ucket\x18\t \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12P\n\x06report\x18\n \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\x12\r\n\x05group\x18\x0b \x01(\x08\x12W\n\x0c\x64\x62\x43onnection\x18\x0c \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12k\n\x08\x64\x62Secret\x18\r \x03(\x0b\x32Y.github.com.metaprov.modelaapi.services.data.v1.CreateForecastReportRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xd7\x06\n\x1a\x43reateSummaryReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12U\n\nconnection\x18\x03 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x66\n\x06secret\x18\x04 \x03(\x0b\x32V.github.com.metaprov.modelaapi.services.data.v1.CreateSummaryReportRequest.SecretEntry\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12P\n\x06report\x18\x06 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\x12W\n\x0c\x64\x62\x43onnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12j\n\x08\x64\x62Secret\x18\x08 \x03(\x0b\x32X.github.com.metaprov.modelaapi.services.data.v1.CreateSummaryReportRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"#\n\x14\x43reateReportResponse\x12\x0b\n\x03pdf\x18\x01 \x01(\x0c\"\xc3\x03\n\x1a\x43reateDatasetReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12P\n\x06report\x18\x05 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xe6\x04\n\x18\x43reateStudyReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\ndatasource\x18\x05 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12S\n\x06models\x18\x06 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelList\x12P\n\x06report\x18\x07 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xc4\x04\n\x0f\x41skModelRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12\x0e\n\x06\x62udget\x18\x06 \x01(\x05\x12\x11\n\tdefaultHP\x18\x07 \x01(\x08\x12\x11\n\talgorithm\x18\x08 \x01(\t\x12V\n\nalgorithms\x18\t \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"\xc6\x03\n\x1fGetTimeSeriesDatasetKeysRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"0\n GetTimeSeriesDatasetKeysResponse\x12\x0c\n\x04keys\x18\x01 \x03(\t\"\xa4\x04\n\x17\x41skForecastModelRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12\x0c\n\x04keys\x18\x06 \x03(\t\x12V\n\nalgorithms\x18\x07 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"j\n\x18\x41skForecastModelResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xe2\x04\n\x12\x41skEnsembleRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12O\n\x06models\x18\x06 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12V\n\nalgorithms\x18\x07 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"e\n\x13\x41skEnsembleResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xb0\x04\n\x12\x41skBaselineRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12\x10\n\x08\x61lgnames\x18\x06 \x03(\t\x12\x0b\n\x03\x61ll\x18\x07 \x01(\x08\x12V\n\nalgorithms\x18\x08 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"e\n\x13\x41skBaselineResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xb7\x04\n\x1a\x41skAllModelsForTaskRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12\x0e\n\x06\x62udget\x18\x06 \x01(\x05\x12\x0c\n\x04task\x18\x07 \x01(\t\x12V\n\nalgorithms\x18\x08 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"m\n\x1b\x41skAllModelsForTaskResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\x97\x04\n\x10TellModelRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12\x0e\n\x06\x66\x61iled\x18\x07 \x01(\x08\"#\n\x11TellModelResponse\x12\x0e\n\x06pruned\x18\x01 \x01(\x08\"\x13\n\x11\x44sShutdownRequest\"\x14\n\x12\x44sShutdownResponse\"\xda\x02\n\x17\x44sTestConnectionRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x63\n\x06secret\x18\x03 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.DsTestConnectionRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"7\n\x18\x44sTestConnectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x08\x12\x0b\n\x03msg\x18\x02 \x01(\t\"\x94\x02\n\x13\x44sStudyEndedRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\"\x16\n\x14\x44sStudyEndedResponse\"\xed\x02\n\x16SaveOptimizerDBRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\x06\x62ucket\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\"r\n\x17SaveOptimizerDBResponse\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"n\n\x15\x44sGetDatabasesRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"+\n\x16\x44sGetDatabasesResponse\x12\x11\n\tdatabases\x18\x01 \x03(\t\"k\n\x12\x44sGetTablesRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"%\n\x13\x44sGetTablesResponse\x12\x0e\n\x06tables\x18\x01 \x03(\t\"y\n\x13\x44sExecuteSqlRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x0b\n\x03sql\x18\x04 \x01(\t\"f\n\x14\x44sExecuteSqlResponse\x12N\n\ttableview\x18\x01 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\"\xe8\x02\n\x11\x44sSnapshotRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"\x14\n\x12\x44sSnapshotResponse\"b\n\x10\x41skModelResponse\x12N\n\x05model\x18\x01 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\x95\x08\n\x16GenTrainingDataRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12\\\n\x11storageConnection\x18\x03 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12p\n\rstorageSecret\x18\x05 \x03(\x0b\x32Y.github.com.metaprov.modelaapi.services.data.v1.GenTrainingDataRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x66\n\x08\x64\x62Secret\x18\x07 \x03(\x0b\x32T.github.com.metaprov.modelaapi.services.data.v1.GenTrainingDataRequest.DbSecretEntry\x12S\n\x05model\x18\x08 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x08\x65ntities\x18\t \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Entity\x12R\n\x06groups\x18\n \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\'\n\x17GenTrainingDataResponse\x12\x0c\n\x04path\x18\x01 \x01(\t\"\xeb\x06\n\x16SyncOnlineStoreRequest\x12\\\n\x11storageConnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12p\n\rstorageSecret\x18\x03 \x03(\x0b\x32Y.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x66\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32T.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreRequest.DbSecretEntry\x12S\n\x05model\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x02\x66g\x18\x07 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12W\n\x08location\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x19\n\x17SyncOnlineStoreResponse\"\xfd\x06\n\x1cGenOnlineStoreDatasetRequest\x12\\\n\x11storageConnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12v\n\rstorageSecret\x18\x03 \x03(\x0b\x32_.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12l\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32Z.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetRequest.DbSecretEntry\x12S\n\x05model\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x02\x66g\x18\x07 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12W\n\x08location\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"x\n\x1dGenOnlineStoreDatasetResponse\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\x8d\x08\n\x13\x42\x61tchPredictRequest\x12\\\n\x11storageConnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12m\n\rstorageSecret\x18\x03 \x03(\x0b\x32V.github.com.metaprov.modelaapi.services.data.v1.BatchPredictRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x63\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32Q.github.com.metaprov.modelaapi.services.data.v1.BatchPredictRequest.DbSecretEntry\x12X\n\nmodelclass\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x05model\x18\x07 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12N\n\x08\x65ntities\x18\x08 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Entity\x12R\n\x06groups\x18\t \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12Y\n\nprediction\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"$\n\x14\x42\x61tchPredictResponse\x12\x0c\n\x04rows\x18\x01 \x01(\x05\"\xba\x05\n\x12SaveDatasetRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12X\n\nmodelclass\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelclassrun\x18\x05 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12W\n\x0c\x64\x62\x43onnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x62\n\x08\x64\x62Secret\x18\x07 \x03(\x0b\x32P.github.com.metaprov.modelaapi.services.data.v1.SaveDatasetRequest.DbSecretEntry\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x84\x06\n\x10SaveModelRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12X\n\nmodelclass\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelclassrun\x18\x04 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12N\n\x05model\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12R\n\x06groups\x18\x06 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12W\n\x0c\x64\x62\x43onnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12`\n\x08\x64\x62Secret\x18\x08 \x03(\x0b\x32N.github.com.metaprov.modelaapi.services.data.v1.SaveModelRequest.DbSecretEntry\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xce\x05\n\x15SavePredictionRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12X\n\nmodelclass\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelclassrun\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12W\n\tpredictor\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Predictor\x12Y\n\nprediction\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\x12W\n\x0c\x64\x62\x43onnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x65\n\x08\x64\x62Secret\x18\x07 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.SavePredictionRequest.DbSecretEntry\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x92\x04\n\x14SavePredictorRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12X\n\nmodelclass\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12X\n\tpredictor\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x64\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32R.github.com.metaprov.modelaapi.services.data.v1.SavePredictorRequest.DbSecretEntry\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x84\x01\n\x19\x43reateMetricsStoreRequest\x12\x0e\n\x06tenant\x18\x01 \x01(\t\x12W\n\x0c\x64\x62\x43onnection\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\x1c\n\x1a\x43reateMetricsStoreResponse\"\x1c\n\x0cSaveResponse\x12\x0c\n\x04\x64\x62id\x18\x01 \x01(\x05\x32\xf7\x43\n\x0b\x44\x61taService\x12\x98\x01\n\x08ReadFile\x12\x41.github.com.metaprov.modelaapi.services.data.v1.DsReadFileRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\x9e\x01\n\x0bReadFeature\x12\x44.github.com.metaprov.modelaapi.services.data.v1.DsReadFeatureRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\x9a\x01\n\tReadAudio\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsReadAudioRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\xa8\x01\n\x0fRunDataPipeline\x12H.github.com.metaprov.modelaapi.services.data.v1.DsRunDataPipelineRequest\x1aI.github.com.metaprov.modelaapi.services.data.v1.DsRunDataPipelineResponse\"\x00\x12\x96\x01\n\tRunRecipe\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeResponse\"\x00\x12\x9a\x01\n\tWriteFile\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsWriteFileRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\xa8\x01\n\x0fGenerateDataset\x12H.github.com.metaprov.modelaapi.services.data.v1.DsGenerateDatasetRequest\x1aI.github.com.metaprov.modelaapi.services.data.v1.DsGenerateDatasetResponse\"\x00\x12\x9f\x01\n\x0cSplitDataset\x12\x45.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetResponse\"\x00\x12\x96\x01\n\tTransform\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsTransformRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.DsTransformResponse\"\x00\x12\xb4\x01\n\x13\x43reateColumnProfile\x12L.github.com.metaprov.modelaapi.services.data.v1.DsCreateColumnProfileRequest\x1aM.github.com.metaprov.modelaapi.services.data.v1.DsCreateColumnProfileResponse\"\x00\x12\x9c\x01\n\x0bInferSchema\x12\x44.github.com.metaprov.modelaapi.services.data.v1.DsInferSchemaRequest\x1a\x45.github.com.metaprov.modelaapi.services.data.v1.DsInferSchemaResponse\"\x00\x12\x9f\x01\n\x0cGetTableView\x12\x45.github.com.metaprov.modelaapi.services.data.v1.DsGetTableViewRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.DsGetTableViewResponse\"\x00\x12\xb4\x01\n\x13SplitDatasetToRungs\x12L.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetToRungsRequest\x1aM.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetToRungsResponse\"\x00\x12\xb7\x01\n\x14\x43reateDatasetProfile\x12M.github.com.metaprov.modelaapi.services.data.v1.DsCreateDatasetProfileRequest\x1aN.github.com.metaprov.modelaapi.services.data.v1.DsCreateDatasetProfileResponse\"\x00\x12\xb1\x01\n\x12\x43reateModelProfile\x12K.github.com.metaprov.modelaapi.services.data.v1.DsCreateModelProfileRequest\x1aL.github.com.metaprov.modelaapi.services.data.v1.DsCreateModelProfileResponse\"\x00\x12\xb1\x01\n\x12\x43reateStudyProfile\x12K.github.com.metaprov.modelaapi.services.data.v1.DsCreateStudyProfileRequest\x1aL.github.com.metaprov.modelaapi.services.data.v1.DsCreateStudyProfileResponse\"\x00\x12\xb4\x01\n\x13\x43reateRecipeProfile\x12L.github.com.metaprov.modelaapi.services.data.v1.DsCreateRecipeProfileRequest\x1aM.github.com.metaprov.modelaapi.services.data.v1.DsCreateRecipeProfileResponse\"\x00\x12\xa5\x01\n\x11\x43reateModelReport\x12H.github.com.metaprov.modelaapi.services.data.v1.CreateModelReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xa5\x01\n\x11\x43reateStudyReport\x12H.github.com.metaprov.modelaapi.services.data.v1.CreateStudyReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xa9\x01\n\x13\x43reateDatasetReport\x12J.github.com.metaprov.modelaapi.services.data.v1.CreateDatasetReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xab\x01\n\x14\x43reateForecastReport\x12K.github.com.metaprov.modelaapi.services.data.v1.CreateForecastReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xa9\x01\n\x13\x43reateSummaryReport\x12J.github.com.metaprov.modelaapi.services.data.v1.CreateSummaryReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\x8c\x01\n\x05\x41skFE\x12?.github.com.metaprov.modelaapi.services.data.v1.AskModelRequest\x1a@.github.com.metaprov.modelaapi.services.data.v1.AskModelResponse\"\x00\x12\x98\x01\n\x0b\x41skBaseline\x12\x42.github.com.metaprov.modelaapi.services.data.v1.AskBaselineRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.AskBaselineResponse\"\x00\x12\x98\x01\n\x0b\x41skEnsemble\x12\x42.github.com.metaprov.modelaapi.services.data.v1.AskEnsembleRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.AskEnsembleResponse\"\x00\x12\xa7\x01\n\x10\x41skForecastModel\x12G.github.com.metaprov.modelaapi.services.data.v1.AskForecastModelRequest\x1aH.github.com.metaprov.modelaapi.services.data.v1.AskForecastModelResponse\"\x00\x12\x8f\x01\n\x08\x41skModel\x12?.github.com.metaprov.modelaapi.services.data.v1.AskModelRequest\x1a@.github.com.metaprov.modelaapi.services.data.v1.AskModelResponse\"\x00\x12\xb0\x01\n\x13\x41skAllModelsForTask\x12J.github.com.metaprov.modelaapi.services.data.v1.AskAllModelsForTaskRequest\x1aK.github.com.metaprov.modelaapi.services.data.v1.AskAllModelsForTaskResponse\"\x00\x12\x99\x01\n\x10TellPartialModel\x12@.github.com.metaprov.modelaapi.services.data.v1.TellModelRequest\x1a\x41.github.com.metaprov.modelaapi.services.data.v1.TellModelResponse\"\x00\x12\x92\x01\n\tTellModel\x12@.github.com.metaprov.modelaapi.services.data.v1.TellModelRequest\x1a\x41.github.com.metaprov.modelaapi.services.data.v1.TellModelResponse\"\x00\x12\xae\x01\n\x11MergeForecastFile\x12J.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileRequest\x1aK.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileResponse\"\x00\x12\xa7\x01\n\x10\x44sTestConnection\x12G.github.com.metaprov.modelaapi.services.data.v1.DsTestConnectionRequest\x1aH.github.com.metaprov.modelaapi.services.data.v1.DsTestConnectionResponse\"\x00\x12\x93\x01\n\x08ShutDown\x12\x41.github.com.metaprov.modelaapi.services.data.v1.DsShutdownRequest\x1a\x42.github.com.metaprov.modelaapi.services.data.v1.DsShutdownResponse\"\x00\x12\x99\x01\n\nStudyEnded\x12\x43.github.com.metaprov.modelaapi.services.data.v1.DsStudyEndedRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.DsStudyEndedResponse\"\x00\x12\xa4\x01\n\x0fSaveOptimizerDB\x12\x46.github.com.metaprov.modelaapi.services.data.v1.SaveOptimizerDBRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.SaveOptimizerDBResponse\"\x00\x12\x9f\x01\n\x0cGetDatabases\x12\x45.github.com.metaprov.modelaapi.services.data.v1.DsGetDatabasesRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.DsGetDatabasesResponse\"\x00\x12\x96\x01\n\tGetTables\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsGetTablesRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.DsGetTablesResponse\"\x00\x12\x99\x01\n\nExecuteSql\x12\x43.github.com.metaprov.modelaapi.services.data.v1.DsExecuteSqlRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.DsExecuteSqlResponse\"\x00\x12\x93\x01\n\x08Snapshot\x12\x41.github.com.metaprov.modelaapi.services.data.v1.DsSnapshotRequest\x1a\x42.github.com.metaprov.modelaapi.services.data.v1.DsSnapshotResponse\"\x00\x12\x9e\x01\n\x0fUnitTestDataset\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\x9c\x01\n\rUnitTestModel\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\x9f\x01\n\x10UnitTestFeedback\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\xa7\x01\n\x18UnitTestFeatureHistogram\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\xa0\x01\n\x11UnitTestPredictor\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\xa1\x01\n\x0eGroupByDataset\x12\x45.github.com.metaprov.modelaapi.services.data.v1.GroupByDatasetRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.GroupByDatasetResponse\"\x00\x12\xa4\x01\n\x0fSyncOnlineStore\x12\x46.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreResponse\"\x00\x12\xa4\x01\n\x0fGenTrainingData\x12\x46.github.com.metaprov.modelaapi.services.data.v1.GenTrainingDataRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.GenTrainingDataResponse\"\x00\x12\xb6\x01\n\x15GenOnlineStoreDataset\x12L.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetRequest\x1aM.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetResponse\"\x00\x12\x9b\x01\n\x0c\x42\x61tchPredict\x12\x43.github.com.metaprov.modelaapi.services.data.v1.BatchPredictRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.BatchPredictResponse\"\x00\x12\x91\x01\n\x0bSaveDataSet\x12\x42.github.com.metaprov.modelaapi.services.data.v1.SaveDatasetRequest\x1a<.github.com.metaprov.modelaapi.services.data.v1.SaveResponse\"\x00\x12\x8d\x01\n\tSaveModel\x12@.github.com.metaprov.modelaapi.services.data.v1.SaveModelRequest\x1a<.github.com.metaprov.modelaapi.services.data.v1.SaveResponse\"\x00\x12\x97\x01\n\x0eSavePrediction\x12\x45.github.com.metaprov.modelaapi.services.data.v1.SavePredictionRequest\x1a<.github.com.metaprov.modelaapi.services.data.v1.SaveResponse\"\x00\x12\xad\x01\n\x12\x43reateMetricsStore\x12I.github.com.metaprov.modelaapi.services.data.v1.CreateMetricsStoreRequest\x1aJ.github.com.metaprov.modelaapi.services.data.v1.CreateMetricsStoreResponse\"\x00\x42\x30Z.github.com/metaprov/modelaapi/services/data/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'github.com.metaprov.modelaapi.services.data.v1.data_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z.github.com/metaprov/modelaapi/services/data/v1'
@@ -44,36 +44,22 @@
   _DSRUNRECIPEREQUEST_STORAGESECRETENTRY._serialized_options = b'8\001'
   _DSRUNRECIPEREQUEST_DBSECRETENTRY._options = None
   _DSRUNRECIPEREQUEST_DBSECRETENTRY._serialized_options = b'8\001'
   _DSCREATERECIPEPROFILEREQUEST_STORAGESECRETENTRY._options = None
   _DSCREATERECIPEPROFILEREQUEST_STORAGESECRETENTRY._serialized_options = b'8\001'
   _DSCREATERECIPEPROFILEREQUEST_DBSECRETENTRY._options = None
   _DSCREATERECIPEPROFILEREQUEST_DBSECRETENTRY._serialized_options = b'8\001'
-  _DSCREATEMODELPROFILEREQUEST_SECRETENTRY._options = None
-  _DSCREATEMODELPROFILEREQUEST_SECRETENTRY._serialized_options = b'8\001'
-  _DSCREATEMODELPROFILEREQUEST_DBSECRETENTRY._options = None
-  _DSCREATEMODELPROFILEREQUEST_DBSECRETENTRY._serialized_options = b'8\001'
   _DSMERGEFORECASTFILEREQUEST_SECRETENTRY._options = None
   _DSMERGEFORECASTFILEREQUEST_SECRETENTRY._serialized_options = b'8\001'
   _DSMERGEFORECASTFILEREQUEST_DBSECRETENTRY._options = None
   _DSMERGEFORECASTFILEREQUEST_DBSECRETENTRY._serialized_options = b'8\001'
-  _DSCREATESTUDYPROFILEREQUEST_SECRETENTRY._options = None
-  _DSCREATESTUDYPROFILEREQUEST_SECRETENTRY._serialized_options = b'8\001'
-  _DSCREATESTUDYPROFILEREQUEST_DBSECRETENTRY._options = None
-  _DSCREATESTUDYPROFILEREQUEST_DBSECRETENTRY._serialized_options = b'8\001'
   _DSGENERATEDATASETREQUEST_SECRETENTRY._options = None
   _DSGENERATEDATASETREQUEST_SECRETENTRY._serialized_options = b'8\001'
   _DSGENERATEDATASETREQUEST_DBSECRETENTRY._options = None
   _DSGENERATEDATASETREQUEST_DBSECRETENTRY._serialized_options = b'8\001'
-  _DSSPLITDATASETREQUEST_SECRETENTRY._options = None
-  _DSSPLITDATASETREQUEST_SECRETENTRY._serialized_options = b'8\001'
-  _DSSPLITDATASETREQUEST_DBSECRETENTRY._options = None
-  _DSSPLITDATASETREQUEST_DBSECRETENTRY._serialized_options = b'8\001'
-  _DSSPLITDATASETTORUNGSREQUEST_SECRETENTRY._options = None
-  _DSSPLITDATASETTORUNGSREQUEST_SECRETENTRY._serialized_options = b'8\001'
   _DSTRANSFORMREQUEST_SECRETENTRY._options = None
   _DSTRANSFORMREQUEST_SECRETENTRY._serialized_options = b'8\001'
   _DSCREATECOLUMNPROFILEREQUEST_SECRETENTRY._options = None
   _DSCREATECOLUMNPROFILEREQUEST_SECRETENTRY._serialized_options = b'8\001'
   _DSCREATECOLUMNPROFILEREQUEST_DBSECRETENTRY._options = None
   _DSCREATECOLUMNPROFILEREQUEST_DBSECRETENTRY._serialized_options = b'8\001'
   _GROUPBYDATASETREQUEST_SECRETENTRY._options = None
@@ -86,18 +72,14 @@
   _CREATEFORECASTREPORTREQUEST_DBSECRETENTRY._serialized_options = b'8\001'
   _CREATESUMMARYREPORTREQUEST_SECRETENTRY._options = None
   _CREATESUMMARYREPORTREQUEST_SECRETENTRY._serialized_options = b'8\001'
   _CREATESUMMARYREPORTREQUEST_DBSECRETENTRY._options = None
   _CREATESUMMARYREPORTREQUEST_DBSECRETENTRY._serialized_options = b'8\001'
   _DSTESTCONNECTIONREQUEST_SECRETENTRY._options = None
   _DSTESTCONNECTIONREQUEST_SECRETENTRY._serialized_options = b'8\001'
-  _DSSTUDYENDEDREQUEST_SECRETENTRY._options = None
-  _DSSTUDYENDEDREQUEST_SECRETENTRY._serialized_options = b'8\001'
-  _SAVEOPTIMIZERDBREQUEST_SECRETENTRY._options = None
-  _SAVEOPTIMIZERDBREQUEST_SECRETENTRY._serialized_options = b'8\001'
   _GENTRAININGDATAREQUEST_STORAGESECRETENTRY._options = None
   _GENTRAININGDATAREQUEST_STORAGESECRETENTRY._serialized_options = b'8\001'
   _GENTRAININGDATAREQUEST_DBSECRETENTRY._options = None
   _GENTRAININGDATAREQUEST_DBSECRETENTRY._serialized_options = b'8\001'
   _SYNCONLINESTOREREQUEST_STORAGESECRETENTRY._options = None
   _SYNCONLINESTOREREQUEST_STORAGESECRETENTRY._serialized_options = b'8\001'
   _SYNCONLINESTOREREQUEST_DBSECRETENTRY._options = None
@@ -163,233 +145,215 @@
   _DSCREATERECIPEPROFILERESPONSE._serialized_start=6146
   _DSCREATERECIPEPROFILERESPONSE._serialized_end=6254
   _DATASOURCERESPONSE._serialized_start=6256
   _DATASOURCERESPONSE._serialized_end=6276
   _DATASETRESPONSE._serialized_start=6278
   _DATASETRESPONSE._serialized_end=6295
   _DSCREATEDATASETPROFILEREQUEST._serialized_start=6298
-  _DSCREATEDATASETPROFILEREQUEST._serialized_end=6670
-  _DSCREATEDATASETPROFILERESPONSE._serialized_start=6673
-  _DSCREATEDATASETPROFILERESPONSE._serialized_end=6980
-  _DSCREATEMODELPROFILEREQUEST._serialized_start=6983
-  _DSCREATEMODELPROFILEREQUEST._serialized_end=8085
-  _DSCREATEMODELPROFILEREQUEST_SECRETENTRY._serialized_start=1036
-  _DSCREATEMODELPROFILEREQUEST_SECRETENTRY._serialized_end=1081
-  _DSCREATEMODELPROFILEREQUEST_DBSECRETENTRY._serialized_start=4942
-  _DSCREATEMODELPROFILEREQUEST_DBSECRETENTRY._serialized_end=4989
-  _DSCREATEMODELPROFILERESPONSE._serialized_start=8087
-  _DSCREATEMODELPROFILERESPONSE._serialized_end=8130
-  _DSMERGEFORECASTFILEREQUEST._serialized_start=8133
-  _DSMERGEFORECASTFILEREQUEST._serialized_end=9251
+  _DSCREATEDATASETPROFILEREQUEST._serialized_end=6756
+  _DSCREATEDATASETPROFILERESPONSE._serialized_start=6759
+  _DSCREATEDATASETPROFILERESPONSE._serialized_end=7066
+  _DSCREATEMODELPROFILEREQUEST._serialized_start=7069
+  _DSCREATEMODELPROFILEREQUEST._serialized_end=7685
+  _DSCREATEMODELPROFILERESPONSE._serialized_start=7687
+  _DSCREATEMODELPROFILERESPONSE._serialized_end=7813
+  _DSMERGEFORECASTFILEREQUEST._serialized_start=7816
+  _DSMERGEFORECASTFILEREQUEST._serialized_end=8934
   _DSMERGEFORECASTFILEREQUEST_SECRETENTRY._serialized_start=1036
   _DSMERGEFORECASTFILEREQUEST_SECRETENTRY._serialized_end=1081
   _DSMERGEFORECASTFILEREQUEST_DBSECRETENTRY._serialized_start=4942
   _DSMERGEFORECASTFILEREQUEST_DBSECRETENTRY._serialized_end=4989
-  _DSMERGEFORECASTFILERESPONSE._serialized_start=9253
-  _DSMERGEFORECASTFILERESPONSE._serialized_end=9295
-  _DSCREATESTUDYPROFILEREQUEST._serialized_start=9298
-  _DSCREATESTUDYPROFILEREQUEST._serialized_end=10401
-  _DSCREATESTUDYPROFILEREQUEST_SECRETENTRY._serialized_start=1036
-  _DSCREATESTUDYPROFILEREQUEST_SECRETENTRY._serialized_end=1081
-  _DSCREATESTUDYPROFILEREQUEST_DBSECRETENTRY._serialized_start=4942
-  _DSCREATESTUDYPROFILEREQUEST_DBSECRETENTRY._serialized_end=4989
-  _DSCREATESTUDYPROFILERESPONSE._serialized_start=10403
-  _DSCREATESTUDYPROFILERESPONSE._serialized_end=10446
-  _RUNTESTSUITEREQUEST._serialized_start=10449
-  _RUNTESTSUITEREQUEST._serialized_end=11412
-  _RUNTESTSUITERESPONSE._serialized_start=11414
-  _RUNTESTSUITERESPONSE._serialized_end=11526
-  _DSGENERATEDATASETREQUEST._serialized_start=11529
-  _DSGENERATEDATASETREQUEST._serialized_end=12483
+  _DSMERGEFORECASTFILERESPONSE._serialized_start=8936
+  _DSMERGEFORECASTFILERESPONSE._serialized_end=8978
+  _DSCREATESTUDYPROFILEREQUEST._serialized_start=8981
+  _DSCREATESTUDYPROFILEREQUEST._serialized_end=9598
+  _DSCREATESTUDYPROFILERESPONSE._serialized_start=9600
+  _DSCREATESTUDYPROFILERESPONSE._serialized_end=9726
+  _RUNTESTSUITEREQUEST._serialized_start=9729
+  _RUNTESTSUITEREQUEST._serialized_end=10692
+  _RUNTESTSUITERESPONSE._serialized_start=10694
+  _RUNTESTSUITERESPONSE._serialized_end=10806
+  _DSGENERATEDATASETREQUEST._serialized_start=10809
+  _DSGENERATEDATASETREQUEST._serialized_end=11763
   _DSGENERATEDATASETREQUEST_SECRETENTRY._serialized_start=1036
   _DSGENERATEDATASETREQUEST_SECRETENTRY._serialized_end=1081
   _DSGENERATEDATASETREQUEST_DBSECRETENTRY._serialized_start=4942
   _DSGENERATEDATASETREQUEST_DBSECRETENTRY._serialized_end=4989
-  _DSGENERATEDATASETRESPONSE._serialized_start=12485
-  _DSGENERATEDATASETRESPONSE._serialized_end=12599
-  _DSSPLITDATASETREQUEST._serialized_start=12602
-  _DSSPLITDATASETREQUEST._serialized_end=13796
-  _DSSPLITDATASETREQUEST_SECRETENTRY._serialized_start=1036
-  _DSSPLITDATASETREQUEST_SECRETENTRY._serialized_end=1081
-  _DSSPLITDATASETREQUEST_DBSECRETENTRY._serialized_start=4942
-  _DSSPLITDATASETREQUEST_DBSECRETENTRY._serialized_end=4989
-  _DSSPLITDATASETRESPONSE._serialized_start=13799
-  _DSSPLITDATASETRESPONSE._serialized_end=13967
-  _DSSPLITDATASETTORUNGSREQUEST._serialized_start=13970
-  _DSSPLITDATASETTORUNGSREQUEST._serialized_end=14682
-  _DSSPLITDATASETTORUNGSREQUEST_SECRETENTRY._serialized_start=1036
-  _DSSPLITDATASETTORUNGSREQUEST_SECRETENTRY._serialized_end=1081
-  _DSSPLITDATASETTORUNGSRESPONSE._serialized_start=14684
-  _DSSPLITDATASETTORUNGSRESPONSE._serialized_end=14715
-  _DSTRANSFORMREQUEST._serialized_start=14718
-  _DSTRANSFORMREQUEST._serialized_end=15650
+  _DSGENERATEDATASETRESPONSE._serialized_start=11765
+  _DSGENERATEDATASETRESPONSE._serialized_end=11879
+  _DSSPLITDATASETREQUEST._serialized_start=11882
+  _DSSPLITDATASETREQUEST._serialized_end=12587
+  _DSSPLITDATASETRESPONSE._serialized_start=12590
+  _DSSPLITDATASETRESPONSE._serialized_end=13041
+  _DSSPLITDATASETTORUNGSREQUEST._serialized_start=13044
+  _DSSPLITDATASETTORUNGSREQUEST._serialized_end=13516
+  _DSSPLITDATASETTORUNGSRESPONSE._serialized_start=13518
+  _DSSPLITDATASETTORUNGSRESPONSE._serialized_end=13549
+  _DSTRANSFORMREQUEST._serialized_start=13552
+  _DSTRANSFORMREQUEST._serialized_end=14484
   _DSTRANSFORMREQUEST_SECRETENTRY._serialized_start=1036
   _DSTRANSFORMREQUEST_SECRETENTRY._serialized_end=1081
-  _DSTRANSFORMRESPONSE._serialized_start=15652
-  _DSTRANSFORMRESPONSE._serialized_end=15743
-  _DSCREATECOLUMNPROFILEREQUEST._serialized_start=15746
-  _DSCREATECOLUMNPROFILEREQUEST._serialized_end=16731
+  _DSTRANSFORMRESPONSE._serialized_start=14486
+  _DSTRANSFORMRESPONSE._serialized_end=14577
+  _DSCREATECOLUMNPROFILEREQUEST._serialized_start=14580
+  _DSCREATECOLUMNPROFILEREQUEST._serialized_end=15565
   _DSCREATECOLUMNPROFILEREQUEST_SECRETENTRY._serialized_start=1036
   _DSCREATECOLUMNPROFILEREQUEST_SECRETENTRY._serialized_end=1081
   _DSCREATECOLUMNPROFILEREQUEST_DBSECRETENTRY._serialized_start=4942
   _DSCREATECOLUMNPROFILEREQUEST_DBSECRETENTRY._serialized_end=4989
-  _DSCREATECOLUMNPROFILERESPONSE._serialized_start=16733
-  _DSCREATECOLUMNPROFILERESPONSE._serialized_end=16848
-  _GROUPBYDATASETREQUEST._serialized_start=16851
-  _GROUPBYDATASETREQUEST._serialized_end=17775
+  _DSCREATECOLUMNPROFILERESPONSE._serialized_start=15567
+  _DSCREATECOLUMNPROFILERESPONSE._serialized_end=15682
+  _GROUPBYDATASETREQUEST._serialized_start=15685
+  _GROUPBYDATASETREQUEST._serialized_end=16609
   _GROUPBYDATASETREQUEST_SECRETENTRY._serialized_start=1036
   _GROUPBYDATASETREQUEST_SECRETENTRY._serialized_end=1081
   _GROUPBYDATASETREQUEST_DBSECRETENTRY._serialized_start=4942
   _GROUPBYDATASETREQUEST_DBSECRETENTRY._serialized_end=4989
-  _GROUPBYDATASETRESPONSE._serialized_start=17777
-  _GROUPBYDATASETRESPONSE._serialized_end=17814
-  _DSINFERSCHEMAREQUEST._serialized_start=17817
-  _DSINFERSCHEMAREQUEST._serialized_end=18030
-  _DSINFERSCHEMARESPONSE._serialized_start=18032
-  _DSINFERSCHEMARESPONSE._serialized_end=18138
-  _DSGETTABLEVIEWREQUEST._serialized_start=18141
-  _DSGETTABLEVIEWREQUEST._serialized_end=18361
-  _DSGETTABLEVIEWRESPONSE._serialized_start=18363
-  _DSGETTABLEVIEWRESPONSE._serialized_end=18467
-  _CREATEMODELREPORTREQUEST._serialized_start=18470
-  _CREATEMODELREPORTREQUEST._serialized_end=19079
-  _CREATEFORECASTREPORTREQUEST._serialized_start=19082
-  _CREATEFORECASTREPORTREQUEST._serialized_end=20284
+  _GROUPBYDATASETRESPONSE._serialized_start=16611
+  _GROUPBYDATASETRESPONSE._serialized_end=16648
+  _DSINFERSCHEMAREQUEST._serialized_start=16651
+  _DSINFERSCHEMAREQUEST._serialized_end=16864
+  _DSINFERSCHEMARESPONSE._serialized_start=16866
+  _DSINFERSCHEMARESPONSE._serialized_end=16972
+  _DSGETTABLEVIEWREQUEST._serialized_start=16975
+  _DSGETTABLEVIEWREQUEST._serialized_end=17195
+  _DSGETTABLEVIEWRESPONSE._serialized_start=17197
+  _DSGETTABLEVIEWRESPONSE._serialized_end=17301
+  _CREATEMODELREPORTREQUEST._serialized_start=17304
+  _CREATEMODELREPORTREQUEST._serialized_end=17913
+  _CREATEFORECASTREPORTREQUEST._serialized_start=17916
+  _CREATEFORECASTREPORTREQUEST._serialized_end=19118
   _CREATEFORECASTREPORTREQUEST_SECRETENTRY._serialized_start=1036
   _CREATEFORECASTREPORTREQUEST_SECRETENTRY._serialized_end=1081
   _CREATEFORECASTREPORTREQUEST_DBSECRETENTRY._serialized_start=4942
   _CREATEFORECASTREPORTREQUEST_DBSECRETENTRY._serialized_end=4989
-  _CREATESUMMARYREPORTREQUEST._serialized_start=20287
-  _CREATESUMMARYREPORTREQUEST._serialized_end=21142
+  _CREATESUMMARYREPORTREQUEST._serialized_start=19121
+  _CREATESUMMARYREPORTREQUEST._serialized_end=19976
   _CREATESUMMARYREPORTREQUEST_SECRETENTRY._serialized_start=1036
   _CREATESUMMARYREPORTREQUEST_SECRETENTRY._serialized_end=1081
   _CREATESUMMARYREPORTREQUEST_DBSECRETENTRY._serialized_start=4942
   _CREATESUMMARYREPORTREQUEST_DBSECRETENTRY._serialized_end=4989
-  _CREATEREPORTRESPONSE._serialized_start=21144
-  _CREATEREPORTRESPONSE._serialized_end=21179
-  _CREATEDATASETREPORTREQUEST._serialized_start=21182
-  _CREATEDATASETREPORTREQUEST._serialized_end=21633
-  _CREATESTUDYREPORTREQUEST._serialized_start=21636
-  _CREATESTUDYREPORTREQUEST._serialized_end=22250
-  _ASKMODELREQUEST._serialized_start=22253
-  _ASKMODELREQUEST._serialized_end=22833
-  _GETTIMESERIESDATASETKEYSREQUEST._serialized_start=22836
-  _GETTIMESERIESDATASETKEYSREQUEST._serialized_end=23290
-  _GETTIMESERIESDATASETKEYSRESPONSE._serialized_start=23292
-  _GETTIMESERIESDATASETKEYSRESPONSE._serialized_end=23340
-  _ASKFORECASTMODELREQUEST._serialized_start=23343
-  _ASKFORECASTMODELREQUEST._serialized_end=23891
-  _ASKFORECASTMODELRESPONSE._serialized_start=23893
-  _ASKFORECASTMODELRESPONSE._serialized_end=23999
-  _ASKENSEMBLEREQUEST._serialized_start=24002
-  _ASKENSEMBLEREQUEST._serialized_end=24612
-  _ASKENSEMBLERESPONSE._serialized_start=24614
-  _ASKENSEMBLERESPONSE._serialized_end=24715
-  _ASKBASELINEREQUEST._serialized_start=24718
-  _ASKBASELINEREQUEST._serialized_end=25278
-  _ASKBASELINERESPONSE._serialized_start=25280
-  _ASKBASELINERESPONSE._serialized_end=25381
-  _ASKALLMODELSFORTASKREQUEST._serialized_start=25384
-  _ASKALLMODELSFORTASKREQUEST._serialized_end=25951
-  _ASKALLMODELSFORTASKRESPONSE._serialized_start=25953
-  _ASKALLMODELSFORTASKRESPONSE._serialized_end=26062
-  _TELLMODELREQUEST._serialized_start=26065
-  _TELLMODELREQUEST._serialized_end=26600
-  _TELLMODELRESPONSE._serialized_start=26602
-  _TELLMODELRESPONSE._serialized_end=26637
-  _DSSHUTDOWNREQUEST._serialized_start=26639
-  _DSSHUTDOWNREQUEST._serialized_end=26658
-  _DSSHUTDOWNRESPONSE._serialized_start=26660
-  _DSSHUTDOWNRESPONSE._serialized_end=26680
-  _DSTESTCONNECTIONREQUEST._serialized_start=26683
-  _DSTESTCONNECTIONREQUEST._serialized_end=27029
+  _CREATEREPORTRESPONSE._serialized_start=19978
+  _CREATEREPORTRESPONSE._serialized_end=20013
+  _CREATEDATASETREPORTREQUEST._serialized_start=20016
+  _CREATEDATASETREPORTREQUEST._serialized_end=20467
+  _CREATESTUDYREPORTREQUEST._serialized_start=20470
+  _CREATESTUDYREPORTREQUEST._serialized_end=21084
+  _ASKMODELREQUEST._serialized_start=21087
+  _ASKMODELREQUEST._serialized_end=21667
+  _GETTIMESERIESDATASETKEYSREQUEST._serialized_start=21670
+  _GETTIMESERIESDATASETKEYSREQUEST._serialized_end=22124
+  _GETTIMESERIESDATASETKEYSRESPONSE._serialized_start=22126
+  _GETTIMESERIESDATASETKEYSRESPONSE._serialized_end=22174
+  _ASKFORECASTMODELREQUEST._serialized_start=22177
+  _ASKFORECASTMODELREQUEST._serialized_end=22725
+  _ASKFORECASTMODELRESPONSE._serialized_start=22727
+  _ASKFORECASTMODELRESPONSE._serialized_end=22833
+  _ASKENSEMBLEREQUEST._serialized_start=22836
+  _ASKENSEMBLEREQUEST._serialized_end=23446
+  _ASKENSEMBLERESPONSE._serialized_start=23448
+  _ASKENSEMBLERESPONSE._serialized_end=23549
+  _ASKBASELINEREQUEST._serialized_start=23552
+  _ASKBASELINEREQUEST._serialized_end=24112
+  _ASKBASELINERESPONSE._serialized_start=24114
+  _ASKBASELINERESPONSE._serialized_end=24215
+  _ASKALLMODELSFORTASKREQUEST._serialized_start=24218
+  _ASKALLMODELSFORTASKREQUEST._serialized_end=24785
+  _ASKALLMODELSFORTASKRESPONSE._serialized_start=24787
+  _ASKALLMODELSFORTASKRESPONSE._serialized_end=24896
+  _TELLMODELREQUEST._serialized_start=24899
+  _TELLMODELREQUEST._serialized_end=25434
+  _TELLMODELRESPONSE._serialized_start=25436
+  _TELLMODELRESPONSE._serialized_end=25471
+  _DSSHUTDOWNREQUEST._serialized_start=25473
+  _DSSHUTDOWNREQUEST._serialized_end=25492
+  _DSSHUTDOWNRESPONSE._serialized_start=25494
+  _DSSHUTDOWNRESPONSE._serialized_end=25514
+  _DSTESTCONNECTIONREQUEST._serialized_start=25517
+  _DSTESTCONNECTIONREQUEST._serialized_end=25863
   _DSTESTCONNECTIONREQUEST_SECRETENTRY._serialized_start=1036
   _DSTESTCONNECTIONREQUEST_SECRETENTRY._serialized_end=1081
-  _DSTESTCONNECTIONRESPONSE._serialized_start=27031
-  _DSTESTCONNECTIONRESPONSE._serialized_end=27086
-  _DSSTUDYENDEDREQUEST._serialized_start=27089
-  _DSSTUDYENDEDREQUEST._serialized_end=27848
-  _DSSTUDYENDEDREQUEST_SECRETENTRY._serialized_start=1036
-  _DSSTUDYENDEDREQUEST_SECRETENTRY._serialized_end=1081
-  _DSSTUDYENDEDRESPONSE._serialized_start=27850
-  _DSSTUDYENDEDRESPONSE._serialized_end=27872
-  _SAVEOPTIMIZERDBREQUEST._serialized_start=27875
-  _SAVEOPTIMIZERDBREQUEST._serialized_end=28640
-  _SAVEOPTIMIZERDBREQUEST_SECRETENTRY._serialized_start=1036
-  _SAVEOPTIMIZERDBREQUEST_SECRETENTRY._serialized_end=1081
-  _SAVEOPTIMIZERDBRESPONSE._serialized_start=28642
-  _SAVEOPTIMIZERDBRESPONSE._serialized_end=28667
-  _DSGETDATABASESREQUEST._serialized_start=28669
-  _DSGETDATABASESREQUEST._serialized_end=28779
-  _DSGETDATABASESRESPONSE._serialized_start=28781
-  _DSGETDATABASESRESPONSE._serialized_end=28824
-  _DSGETTABLESREQUEST._serialized_start=28826
-  _DSGETTABLESREQUEST._serialized_end=28933
-  _DSGETTABLESRESPONSE._serialized_start=28935
-  _DSGETTABLESRESPONSE._serialized_end=28972
-  _DSEXECUTESQLREQUEST._serialized_start=28974
-  _DSEXECUTESQLREQUEST._serialized_end=29095
-  _DSEXECUTESQLRESPONSE._serialized_start=29097
-  _DSEXECUTESQLRESPONSE._serialized_end=29199
-  _DSSNAPSHOTREQUEST._serialized_start=29202
-  _DSSNAPSHOTREQUEST._serialized_end=29562
-  _DSSNAPSHOTRESPONSE._serialized_start=29564
-  _DSSNAPSHOTRESPONSE._serialized_end=29584
-  _ASKMODELRESPONSE._serialized_start=29586
-  _ASKMODELRESPONSE._serialized_end=29684
-  _GENTRAININGDATAREQUEST._serialized_start=29687
-  _GENTRAININGDATAREQUEST._serialized_end=30732
+  _DSTESTCONNECTIONRESPONSE._serialized_start=25865
+  _DSTESTCONNECTIONRESPONSE._serialized_end=25920
+  _DSSTUDYENDEDREQUEST._serialized_start=25923
+  _DSSTUDYENDEDREQUEST._serialized_end=26199
+  _DSSTUDYENDEDRESPONSE._serialized_start=26201
+  _DSSTUDYENDEDRESPONSE._serialized_end=26223
+  _SAVEOPTIMIZERDBREQUEST._serialized_start=26226
+  _SAVEOPTIMIZERDBREQUEST._serialized_end=26591
+  _SAVEOPTIMIZERDBRESPONSE._serialized_start=26593
+  _SAVEOPTIMIZERDBRESPONSE._serialized_end=26707
+  _DSGETDATABASESREQUEST._serialized_start=26709
+  _DSGETDATABASESREQUEST._serialized_end=26819
+  _DSGETDATABASESRESPONSE._serialized_start=26821
+  _DSGETDATABASESRESPONSE._serialized_end=26864
+  _DSGETTABLESREQUEST._serialized_start=26866
+  _DSGETTABLESREQUEST._serialized_end=26973
+  _DSGETTABLESRESPONSE._serialized_start=26975
+  _DSGETTABLESRESPONSE._serialized_end=27012
+  _DSEXECUTESQLREQUEST._serialized_start=27014
+  _DSEXECUTESQLREQUEST._serialized_end=27135
+  _DSEXECUTESQLRESPONSE._serialized_start=27137
+  _DSEXECUTESQLRESPONSE._serialized_end=27239
+  _DSSNAPSHOTREQUEST._serialized_start=27242
+  _DSSNAPSHOTREQUEST._serialized_end=27602
+  _DSSNAPSHOTRESPONSE._serialized_start=27604
+  _DSSNAPSHOTRESPONSE._serialized_end=27624
+  _ASKMODELRESPONSE._serialized_start=27626
+  _ASKMODELRESPONSE._serialized_end=27724
+  _GENTRAININGDATAREQUEST._serialized_start=27727
+  _GENTRAININGDATAREQUEST._serialized_end=28772
   _GENTRAININGDATAREQUEST_STORAGESECRETENTRY._serialized_start=4888
   _GENTRAININGDATAREQUEST_STORAGESECRETENTRY._serialized_end=4940
   _GENTRAININGDATAREQUEST_DBSECRETENTRY._serialized_start=4942
   _GENTRAININGDATAREQUEST_DBSECRETENTRY._serialized_end=4989
-  _GENTRAININGDATARESPONSE._serialized_start=30734
-  _GENTRAININGDATARESPONSE._serialized_end=30773
-  _SYNCONLINESTOREREQUEST._serialized_start=30776
-  _SYNCONLINESTOREREQUEST._serialized_end=31651
+  _GENTRAININGDATARESPONSE._serialized_start=28774
+  _GENTRAININGDATARESPONSE._serialized_end=28813
+  _SYNCONLINESTOREREQUEST._serialized_start=28816
+  _SYNCONLINESTOREREQUEST._serialized_end=29691
   _SYNCONLINESTOREREQUEST_STORAGESECRETENTRY._serialized_start=4888
   _SYNCONLINESTOREREQUEST_STORAGESECRETENTRY._serialized_end=4940
   _SYNCONLINESTOREREQUEST_DBSECRETENTRY._serialized_start=4942
   _SYNCONLINESTOREREQUEST_DBSECRETENTRY._serialized_end=4989
-  _SYNCONLINESTORERESPONSE._serialized_start=31653
-  _SYNCONLINESTORERESPONSE._serialized_end=31678
-  _GENONLINESTOREDATASETREQUEST._serialized_start=31681
-  _GENONLINESTOREDATASETREQUEST._serialized_end=32574
+  _SYNCONLINESTORERESPONSE._serialized_start=29693
+  _SYNCONLINESTORERESPONSE._serialized_end=29718
+  _GENONLINESTOREDATASETREQUEST._serialized_start=29721
+  _GENONLINESTOREDATASETREQUEST._serialized_end=30614
   _GENONLINESTOREDATASETREQUEST_STORAGESECRETENTRY._serialized_start=4888
   _GENONLINESTOREDATASETREQUEST_STORAGESECRETENTRY._serialized_end=4940
   _GENONLINESTOREDATASETREQUEST_DBSECRETENTRY._serialized_start=4942
   _GENONLINESTOREDATASETREQUEST_DBSECRETENTRY._serialized_end=4989
-  _GENONLINESTOREDATASETRESPONSE._serialized_start=32576
-  _GENONLINESTOREDATASETRESPONSE._serialized_end=32696
-  _BATCHPREDICTREQUEST._serialized_start=32699
-  _BATCHPREDICTREQUEST._serialized_end=33736
+  _GENONLINESTOREDATASETRESPONSE._serialized_start=30616
+  _GENONLINESTOREDATASETRESPONSE._serialized_end=30736
+  _BATCHPREDICTREQUEST._serialized_start=30739
+  _BATCHPREDICTREQUEST._serialized_end=31776
   _BATCHPREDICTREQUEST_STORAGESECRETENTRY._serialized_start=4888
   _BATCHPREDICTREQUEST_STORAGESECRETENTRY._serialized_end=4940
   _BATCHPREDICTREQUEST_DBSECRETENTRY._serialized_start=4942
   _BATCHPREDICTREQUEST_DBSECRETENTRY._serialized_end=4989
-  _BATCHPREDICTRESPONSE._serialized_start=33738
-  _BATCHPREDICTRESPONSE._serialized_end=33774
-  _SAVEDATASETREQUEST._serialized_start=33777
-  _SAVEDATASETREQUEST._serialized_end=34475
+  _BATCHPREDICTRESPONSE._serialized_start=31778
+  _BATCHPREDICTRESPONSE._serialized_end=31814
+  _SAVEDATASETREQUEST._serialized_start=31817
+  _SAVEDATASETREQUEST._serialized_end=32515
   _SAVEDATASETREQUEST_DBSECRETENTRY._serialized_start=4942
   _SAVEDATASETREQUEST_DBSECRETENTRY._serialized_end=4989
-  _SAVEMODELREQUEST._serialized_start=34478
-  _SAVEMODELREQUEST._serialized_end=35250
+  _SAVEMODELREQUEST._serialized_start=32518
+  _SAVEMODELREQUEST._serialized_end=33290
   _SAVEMODELREQUEST_DBSECRETENTRY._serialized_start=4942
   _SAVEMODELREQUEST_DBSECRETENTRY._serialized_end=4989
-  _SAVEPREDICTIONREQUEST._serialized_start=35253
-  _SAVEPREDICTIONREQUEST._serialized_end=35971
+  _SAVEPREDICTIONREQUEST._serialized_start=33293
+  _SAVEPREDICTIONREQUEST._serialized_end=34011
   _SAVEPREDICTIONREQUEST_DBSECRETENTRY._serialized_start=4942
   _SAVEPREDICTIONREQUEST_DBSECRETENTRY._serialized_end=4989
-  _SAVEPREDICTORREQUEST._serialized_start=35974
-  _SAVEPREDICTORREQUEST._serialized_end=36504
+  _SAVEPREDICTORREQUEST._serialized_start=34014
+  _SAVEPREDICTORREQUEST._serialized_end=34544
   _SAVEPREDICTORREQUEST_DBSECRETENTRY._serialized_start=4942
   _SAVEPREDICTORREQUEST_DBSECRETENTRY._serialized_end=4989
-  _CREATEMETRICSSTOREREQUEST._serialized_start=36507
-  _CREATEMETRICSSTOREREQUEST._serialized_end=36639
-  _CREATEMETRICSSTORERESPONSE._serialized_start=36641
-  _CREATEMETRICSSTORERESPONSE._serialized_end=36669
-  _SAVERESPONSE._serialized_start=36671
-  _SAVERESPONSE._serialized_end=36699
-  _DATASERVICE._serialized_start=36702
-  _DATASERVICE._serialized_end=45397
+  _CREATEMETRICSSTOREREQUEST._serialized_start=34547
+  _CREATEMETRICSSTOREREQUEST._serialized_end=34679
+  _CREATEMETRICSSTORERESPONSE._serialized_start=34681
+  _CREATEMETRICSSTORERESPONSE._serialized_end=34709
+  _SAVERESPONSE._serialized_start=34711
+  _SAVERESPONSE._serialized_end=34739
+  _DATASERVICE._serialized_start=34742
+  _DATASERVICE._serialized_end=43437
 # @@protoc_insertion_point(module_scope)
```

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,108 +14,56 @@
 from github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_training_dot_v1alpha1_dot_generated__pb2
 from github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_data_dot_v1alpha1_dot_generated__pb2
 from github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_infra_dot_v1alpha1_dot_generated__pb2
 from github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_catalog_dot_v1alpha1_dot_generated__pb2
 from k8s.io.api.core.v1 import generated_pb2 as k8s_dot_io_dot_api_dot_core_dot_v1_dot_generated__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nAgithub.com/metaprov/modelaapi/services/trainerd/v1/trainerd.proto\x12\x32github.com.metaprov.modelaapi.services.trainerd.v1\x1aHgithub.com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated.proto\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1a\x45github.com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated.proto\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a\"k8s.io/api/core/v1/generated.proto\"\xf5\x07\n\x0cTrainRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12N\n\x05model\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12N\n\x05study\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x07 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x08 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12U\n\nconnection\x18\t \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\\\n\x06secret\x18\n \x03(\x0b\x32L.github.com.metaprov.modelaapi.services.trainerd.v1.TrainRequest.SecretEntry\x12R\n\x0btestDataset\x18\x0b \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12S\n\x0ctrainDataset\x18\x0c \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12\r\n\x05group\x18\r \x01(\x08\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x9c\x08\n\rTrainResponse\x12T\n\x06result\x18\x01 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12\x17\n\x0fweightsCloudUri\x18\x02 \x01(\t\x12\x18\n\x10manifestCloudUri\x18\x03 \x01(\t\x12\x14\n\x0clogsCloudUri\x18\x04 \x01(\t\x12\x14\n\x0clabelEncoder\x18\x05 \x01(\t\x12\x19\n\x11pythonVersionInfo\x18\x06 \x01(\t\x12\x11\n\tpythonCMD\x18\x07 \x01(\t\x12\n\n\x02OS\x18\x08 \x01(\t\x12\x63\n\tpipFreeze\x18\t \x03(\x0b\x32P.github.com.metaprov.modelaapi.services.trainerd.v1.TrainResponse.PipFreezeEntry\x12\x83\x01\n\x19impurityFeatureImportance\x18\n \x03(\x0b\x32`.github.com.metaprov.modelaapi.services.trainerd.v1.TrainResponse.ImpurityFeatureImportanceEntry\x12\x89\x01\n\x1cpermutationFeatureImportance\x18\x0b \x03(\x0b\x32\x63.github.com.metaprov.modelaapi.services.trainerd.v1.TrainResponse.PermutationFeatureImportanceEntry\x12T\n\x02\x63m\x18\x0c \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrix\x12\x15\n\rmodelIndexURI\x18\r \x01(\t\x12\x13\n\x0b\x66orecastURI\x18\x0e \x01(\t\x12V\n\x08\x66\x65\x61tures\x18\x0f \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12\x12\n\nprofileURI\x18\x10 \x01(\t\x1a\x30\n\x0ePipFreezeEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a@\n\x1eImpurityFeatureImportanceEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\x1a\x43\n!PermutationFeatureImportanceEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\"\xc1\x06\n\x0e\x43ompileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12N\n\x05model\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12N\n\x05study\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x07 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x08 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12U\n\nconnection\x18\t \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12^\n\x06secret\x18\n \x03(\x0b\x32N.github.com.metaprov.modelaapi.services.trainerd.v1.CompileRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"+\n\x0f\x43ompileResponse\x12\x18\n\x10\x63ompiledModelUri\x18\x01 \x01(\t\"\xca\x06\n\x0bTestRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12N\n\x05model\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12N\n\x05study\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x07 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x08 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12U\n\nconnection\x18\t \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\x06secret\x18\n \x03(\x0b\x32K.github.com.metaprov.modelaapi.services.trainerd.v1.TestRequest.SecretEntry\x12\r\n\x05group\x18\x0b \x01(\x08\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xe0\n\n\x0cTestResponse\x12Z\n\x0ctrain_result\x18\x01 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12Y\n\x0btest_result\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12^\n\x10\x62\x65nchmark_result\x18\x03 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12#\n\x1btestingModelWeightsCloudUri\x18\x04 \x01(\t\x12\x1b\n\x13testingLabelEncoder\x18\x05 \x01(\t\x12 \n\x18\x66ullModelWeightsCloudUri\x18\x06 \x01(\t\x12\x18\n\x10\x66ullLabelEncoder\x18\x07 \x01(\t\x12\x1d\n\x15modelManifestCloudUri\x18\x08 \x01(\t\x12\x19\n\x11modelLogsCloudUri\x18\t \x01(\t\x12\x1a\n\x12preWeightsCloudUri\x18\n \x01(\t\x12\x1b\n\x13preManifestCloudUri\x18\x0b \x01(\t\x12\x17\n\x0fpreLogsCloudUri\x18\x0c \x01(\t\x12\x11\n\tpythonCMD\x18\r \x01(\t\x12\n\n\x02OS\x18\x0e \x01(\t\x12\x19\n\x11pythonVersionInfo\x18\x0f \x01(\t\x12\x62\n\tpipFreeze\x18\x10 \x03(\x0b\x32O.github.com.metaprov.modelaapi.services.trainerd.v1.TestResponse.PipFreezeEntry\x12\x13\n\x0bmisclassUri\x18\x11 \x01(\t\x12\x82\x01\n\x19impurityFeatureImportance\x18\x12 \x03(\x0b\x32_.github.com.metaprov.modelaapi.services.trainerd.v1.TestResponse.ImpurityFeatureImportanceEntry\x12\x88\x01\n\x1cpermutationFeatureImportance\x18\x13 \x03(\x0b\x32\x62.github.com.metaprov.modelaapi.services.trainerd.v1.TestResponse.PermutationFeatureImportanceEntry\x12Y\n\x07trainCM\x18\x14 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrix\x12X\n\x06testCM\x18\x15 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrix\x1a\x30\n\x0ePipFreezeEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a@\n\x1eImpurityFeatureImportanceEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\x1a\x43\n!PermutationFeatureImportanceEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\"\xab\x07\n\x14TrainEnsembleRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12M\n\x04\x62\x61se\x18\x05 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12N\n\x05study\x18\x07 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x08 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\t \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12U\n\nconnection\x18\n \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x64\n\x06secret\x18\x0b \x03(\x0b\x32T.github.com.metaprov.modelaapi.services.trainerd.v1.TrainEnsembleRequest.SecretEntry\x12\r\n\x05group\x18\x0c \x01(\x08\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xa9\x07\n\x13TestEnsembleRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12M\n\x04\x62\x61se\x18\x05 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12N\n\x05study\x18\x07 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x08 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\t \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12U\n\nconnection\x18\n \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x63\n\x06secret\x18\x0b \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.trainerd.v1.TestEnsembleRequest.SecretEntry\x12\r\n\x05group\x18\x0c \x01(\x08\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xb5\x07\n\x19TrainDriftDetectorRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12M\n\x04\x62\x61se\x18\x05 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12N\n\x05study\x18\x07 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x08 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\t \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12U\n\nconnection\x18\n \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12i\n\x06secret\x18\x0b \x03(\x0b\x32Y.github.com.metaprov.modelaapi.services.trainerd.v1.TrainDriftDetectorRequest.SecretEntry\x12\r\n\x05group\x18\x0c \x01(\x08\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xd2\x06\n\x0f\x46orecastRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12N\n\x05model\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12N\n\x05study\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x07 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x08 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12U\n\nconnection\x18\t \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12_\n\x06secret\x18\n \x03(\x0b\x32O.github.com.metaprov.modelaapi.services.trainerd.v1.ForecastRequest.SecretEntry\x12\r\n\x05group\x18\x0b \x01(\x08\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\",\n\x10\x46orecastResponse\x12\x18\n\x10\x66orecastCloudUri\x18\x02 \x01(\t\"\x11\n\x0fShutdownRequest\"\x12\n\x10ShutdownResponse\"\xd0\x06\n\x0e\x45xplainRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12N\n\x05model\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12N\n\x05study\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x07 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x08 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12U\n\nconnection\x18\t \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12^\n\x06secret\x18\n \x03(\x0b\x32N.github.com.metaprov.modelaapi.services.trainerd.v1.ExplainRequest.SecretEntry\x12\r\n\x05group\x18\x0b \x01(\x08\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x9e\x02\n\x0f\x45xplainResponse\x12\x14\n\x0c\x65xplainerUri\x18\x01 \x01(\t\x12\x1a\n\x12trainShapValuesUri\x18\x02 \x01(\t\x12\x19\n\x11testShapValuesUri\x18\x03 \x01(\t\x12\x7f\n\x16shapFeaturesImportance\x18\x04 \x03(\x0b\x32_.github.com.metaprov.modelaapi.services.trainerd.v1.ExplainResponse.ShapFeaturesImportanceEntry\x1a=\n\x1bShapFeaturesImportanceEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\x32\xe5\t\n\x0fTrainerdService\x12\x8e\x01\n\x05Train\x12@.github.com.metaprov.modelaapi.services.trainerd.v1.TrainRequest\x1a\x41.github.com.metaprov.modelaapi.services.trainerd.v1.TrainResponse\"\x00\x12\x94\x01\n\x07\x45xplain\x12\x42.github.com.metaprov.modelaapi.services.trainerd.v1.ExplainRequest\x1a\x43.github.com.metaprov.modelaapi.services.trainerd.v1.ExplainResponse\"\x00\x12\x97\x01\n\x08\x46orecast\x12\x43.github.com.metaprov.modelaapi.services.trainerd.v1.ForecastRequest\x1a\x44.github.com.metaprov.modelaapi.services.trainerd.v1.ForecastResponse\"\x00\x12\x8b\x01\n\x04Test\x12?.github.com.metaprov.modelaapi.services.trainerd.v1.TestRequest\x1a@.github.com.metaprov.modelaapi.services.trainerd.v1.TestResponse\"\x00\x12\x9e\x01\n\rTrainEnsemble\x12H.github.com.metaprov.modelaapi.services.trainerd.v1.TrainEnsembleRequest\x1a\x41.github.com.metaprov.modelaapi.services.trainerd.v1.TrainResponse\"\x00\x12\xa8\x01\n\x12TrainDriftDetector\x12M.github.com.metaprov.modelaapi.services.trainerd.v1.TrainDriftDetectorRequest\x1a\x41.github.com.metaprov.modelaapi.services.trainerd.v1.TrainResponse\"\x00\x12\x9b\x01\n\x0cTestEnsemble\x12G.github.com.metaprov.modelaapi.services.trainerd.v1.TestEnsembleRequest\x1a@.github.com.metaprov.modelaapi.services.trainerd.v1.TestResponse\"\x00\x12\x97\x01\n\x08Shutdown\x12\x43.github.com.metaprov.modelaapi.services.trainerd.v1.ShutdownRequest\x1a\x44.github.com.metaprov.modelaapi.services.trainerd.v1.ShutdownResponse\"\x00\x42\x34Z2github.com/metaprov/modelaapi/services/trainerd/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nAgithub.com/metaprov/modelaapi/services/trainerd/v1/trainerd.proto\x12\x32github.com.metaprov.modelaapi.services.trainerd.v1\x1aHgithub.com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated.proto\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1a\x45github.com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated.proto\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a\"k8s.io/api/core/v1/generated.proto\"\xae\x05\n\x0cTrainRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12N\n\x05model\x18\x04 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x06 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x07 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12S\n\nbaseModels\x18\x08 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xd5\x07\n\rTrainResponse\x12U\n\x07results\x18\x01 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12^\n\x0fweightsLocation\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x63\n\x14labelEncoderLocation\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12_\n\x10\x66orecastLocation\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12^\n\x0fprofileLocation\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x61\n\x0f\x63onfusionMatrix\x18\x06 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrix\x12\x19\n\x11pythonVersionInfo\x18\x07 \x01(\t\x12\n\n\x02OS\x18\t \x01(\t\x12\x63\n\tpipFreeze\x18\n \x03(\x0b\x32P.github.com.metaprov.modelaapi.services.trainerd.v1.TrainResponse.PipFreezeEntry\x12\x83\x01\n\x19impurityFeatureImportance\x18\x0b \x03(\x0b\x32`.github.com.metaprov.modelaapi.services.trainerd.v1.TrainResponse.ImpurityFeatureImportanceEntry\x1a\x30\n\x0ePipFreezeEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a@\n\x1eImpurityFeatureImportanceEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\"\xdb\x04\n\x0e\x43ompileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12N\n\x05model\x18\x04 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x06 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x07 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"+\n\x0f\x43ompileResponse\x12\x18\n\x10\x63ompiledModelUri\x18\x01 \x01(\t\"\xad\x05\n\x0bTestRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12N\n\x05model\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12N\n\x05study\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x07 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x08 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12S\n\nbaseModels\x18\t \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\x8d\x07\n\x0cTestResponse\x12Z\n\x0ctrainResults\x18\x01 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12Y\n\x0btestResults\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12\x62\n\x13testWeightsLocation\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13\x66ullWeightsLocation\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12_\n\x10misclassLocation\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x88\x01\n\x1cpermutationFeatureImportance\x18\x06 \x03(\x0b\x32\x62.github.com.metaprov.modelaapi.services.trainerd.v1.TestResponse.PermutationFeatureImportanceEntry\x12\x66\n\x14trainConfusionMatrix\x18\x07 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrix\x12\x65\n\x13testConfusionMatrix\x18\x08 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrix\x1a\x43\n!PermutationFeatureImportanceEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\"\xb5\x05\n\x19TrainDriftDetectorRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12M\n\x04\x62\x61se\x18\x05 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12N\n\x05study\x18\x07 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x08 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\t \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"\xdc\x04\n\x0f\x46orecastRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12N\n\x05model\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12N\n\x05study\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x07 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x08 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"s\n\x10\x46orecastResponse\x12_\n\x10\x66orecastLocation\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\x11\n\x0fShutdownRequest\"\x12\n\x10ShutdownResponse\"\xdb\x04\n\x0e\x45xplainRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Y\n\x07version\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProductVersion\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12N\n\x05model\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12N\n\x05study\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x07 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x08 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"\xc2\x02\n\x0f\x45xplainResponse\x12`\n\x11\x65xplainerLocation\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x66\n\x17trainShapValuesLocation\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x65\n\x16testShapValuesLocation\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation2\xa6\x07\n\x0fTrainerdService\x12\x8e\x01\n\x05Train\x12@.github.com.metaprov.modelaapi.services.trainerd.v1.TrainRequest\x1a\x41.github.com.metaprov.modelaapi.services.trainerd.v1.TrainResponse\"\x00\x12\x94\x01\n\x07\x45xplain\x12\x42.github.com.metaprov.modelaapi.services.trainerd.v1.ExplainRequest\x1a\x43.github.com.metaprov.modelaapi.services.trainerd.v1.ExplainResponse\"\x00\x12\x97\x01\n\x08\x46orecast\x12\x43.github.com.metaprov.modelaapi.services.trainerd.v1.ForecastRequest\x1a\x44.github.com.metaprov.modelaapi.services.trainerd.v1.ForecastResponse\"\x00\x12\x8b\x01\n\x04Test\x12?.github.com.metaprov.modelaapi.services.trainerd.v1.TestRequest\x1a@.github.com.metaprov.modelaapi.services.trainerd.v1.TestResponse\"\x00\x12\xa8\x01\n\x12TrainDriftDetector\x12M.github.com.metaprov.modelaapi.services.trainerd.v1.TrainDriftDetectorRequest\x1a\x41.github.com.metaprov.modelaapi.services.trainerd.v1.TrainResponse\"\x00\x12\x97\x01\n\x08Shutdown\x12\x43.github.com.metaprov.modelaapi.services.trainerd.v1.ShutdownRequest\x1a\x44.github.com.metaprov.modelaapi.services.trainerd.v1.ShutdownResponse\"\x00\x42\x34Z2github.com/metaprov/modelaapi/services/trainerd/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'github.com.metaprov.modelaapi.services.trainerd.v1.trainerd_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z2github.com/metaprov/modelaapi/services/trainerd/v1'
-  _TRAINREQUEST_SECRETENTRY._options = None
-  _TRAINREQUEST_SECRETENTRY._serialized_options = b'8\001'
   _TRAINRESPONSE_PIPFREEZEENTRY._options = None
   _TRAINRESPONSE_PIPFREEZEENTRY._serialized_options = b'8\001'
   _TRAINRESPONSE_IMPURITYFEATUREIMPORTANCEENTRY._options = None
   _TRAINRESPONSE_IMPURITYFEATUREIMPORTANCEENTRY._serialized_options = b'8\001'
-  _TRAINRESPONSE_PERMUTATIONFEATUREIMPORTANCEENTRY._options = None
-  _TRAINRESPONSE_PERMUTATIONFEATUREIMPORTANCEENTRY._serialized_options = b'8\001'
-  _COMPILEREQUEST_SECRETENTRY._options = None
-  _COMPILEREQUEST_SECRETENTRY._serialized_options = b'8\001'
-  _TESTREQUEST_SECRETENTRY._options = None
-  _TESTREQUEST_SECRETENTRY._serialized_options = b'8\001'
-  _TESTRESPONSE_PIPFREEZEENTRY._options = None
-  _TESTRESPONSE_PIPFREEZEENTRY._serialized_options = b'8\001'
-  _TESTRESPONSE_IMPURITYFEATUREIMPORTANCEENTRY._options = None
-  _TESTRESPONSE_IMPURITYFEATUREIMPORTANCEENTRY._serialized_options = b'8\001'
   _TESTRESPONSE_PERMUTATIONFEATUREIMPORTANCEENTRY._options = None
   _TESTRESPONSE_PERMUTATIONFEATUREIMPORTANCEENTRY._serialized_options = b'8\001'
-  _TRAINENSEMBLEREQUEST_SECRETENTRY._options = None
-  _TRAINENSEMBLEREQUEST_SECRETENTRY._serialized_options = b'8\001'
-  _TESTENSEMBLEREQUEST_SECRETENTRY._options = None
-  _TESTENSEMBLEREQUEST_SECRETENTRY._serialized_options = b'8\001'
-  _TRAINDRIFTDETECTORREQUEST_SECRETENTRY._options = None
-  _TRAINDRIFTDETECTORREQUEST_SECRETENTRY._serialized_options = b'8\001'
-  _FORECASTREQUEST_SECRETENTRY._options = None
-  _FORECASTREQUEST_SECRETENTRY._serialized_options = b'8\001'
-  _EXPLAINREQUEST_SECRETENTRY._options = None
-  _EXPLAINREQUEST_SECRETENTRY._serialized_options = b'8\001'
-  _EXPLAINRESPONSE_SHAPFEATURESIMPORTANCEENTRY._options = None
-  _EXPLAINRESPONSE_SHAPFEATURESIMPORTANCEENTRY._serialized_options = b'8\001'
   _TRAINREQUEST._serialized_start=446
-  _TRAINREQUEST._serialized_end=1459
-  _TRAINREQUEST_SECRETENTRY._serialized_start=1414
-  _TRAINREQUEST_SECRETENTRY._serialized_end=1459
-  _TRAINRESPONSE._serialized_start=1462
-  _TRAINRESPONSE._serialized_end=2514
-  _TRAINRESPONSE_PIPFREEZEENTRY._serialized_start=2331
-  _TRAINRESPONSE_PIPFREEZEENTRY._serialized_end=2379
-  _TRAINRESPONSE_IMPURITYFEATUREIMPORTANCEENTRY._serialized_start=2381
-  _TRAINRESPONSE_IMPURITYFEATUREIMPORTANCEENTRY._serialized_end=2445
-  _TRAINRESPONSE_PERMUTATIONFEATUREIMPORTANCEENTRY._serialized_start=2447
-  _TRAINRESPONSE_PERMUTATIONFEATUREIMPORTANCEENTRY._serialized_end=2514
-  _COMPILEREQUEST._serialized_start=2517
-  _COMPILEREQUEST._serialized_end=3350
-  _COMPILEREQUEST_SECRETENTRY._serialized_start=1414
-  _COMPILEREQUEST_SECRETENTRY._serialized_end=1459
-  _COMPILERESPONSE._serialized_start=3352
-  _COMPILERESPONSE._serialized_end=3395
-  _TESTREQUEST._serialized_start=3398
-  _TESTREQUEST._serialized_end=4240
-  _TESTREQUEST_SECRETENTRY._serialized_start=1414
-  _TESTREQUEST_SECRETENTRY._serialized_end=1459
-  _TESTRESPONSE._serialized_start=4243
-  _TESTRESPONSE._serialized_end=5619
-  _TESTRESPONSE_PIPFREEZEENTRY._serialized_start=2331
-  _TESTRESPONSE_PIPFREEZEENTRY._serialized_end=2379
-  _TESTRESPONSE_IMPURITYFEATUREIMPORTANCEENTRY._serialized_start=2381
-  _TESTRESPONSE_IMPURITYFEATUREIMPORTANCEENTRY._serialized_end=2445
-  _TESTRESPONSE_PERMUTATIONFEATUREIMPORTANCEENTRY._serialized_start=2447
-  _TESTRESPONSE_PERMUTATIONFEATUREIMPORTANCEENTRY._serialized_end=2514
-  _TRAINENSEMBLEREQUEST._serialized_start=5622
-  _TRAINENSEMBLEREQUEST._serialized_end=6561
-  _TRAINENSEMBLEREQUEST_SECRETENTRY._serialized_start=1414
-  _TRAINENSEMBLEREQUEST_SECRETENTRY._serialized_end=1459
-  _TESTENSEMBLEREQUEST._serialized_start=6564
-  _TESTENSEMBLEREQUEST._serialized_end=7501
-  _TESTENSEMBLEREQUEST_SECRETENTRY._serialized_start=1414
-  _TESTENSEMBLEREQUEST_SECRETENTRY._serialized_end=1459
-  _TRAINDRIFTDETECTORREQUEST._serialized_start=7504
-  _TRAINDRIFTDETECTORREQUEST._serialized_end=8453
-  _TRAINDRIFTDETECTORREQUEST_SECRETENTRY._serialized_start=1414
-  _TRAINDRIFTDETECTORREQUEST_SECRETENTRY._serialized_end=1459
-  _FORECASTREQUEST._serialized_start=8456
-  _FORECASTREQUEST._serialized_end=9306
-  _FORECASTREQUEST_SECRETENTRY._serialized_start=1414
-  _FORECASTREQUEST_SECRETENTRY._serialized_end=1459
-  _FORECASTRESPONSE._serialized_start=9308
-  _FORECASTRESPONSE._serialized_end=9352
-  _SHUTDOWNREQUEST._serialized_start=9354
-  _SHUTDOWNREQUEST._serialized_end=9371
-  _SHUTDOWNRESPONSE._serialized_start=9373
-  _SHUTDOWNRESPONSE._serialized_end=9391
-  _EXPLAINREQUEST._serialized_start=9394
-  _EXPLAINREQUEST._serialized_end=10242
-  _EXPLAINREQUEST_SECRETENTRY._serialized_start=1414
-  _EXPLAINREQUEST_SECRETENTRY._serialized_end=1459
-  _EXPLAINRESPONSE._serialized_start=10245
-  _EXPLAINRESPONSE._serialized_end=10531
-  _EXPLAINRESPONSE_SHAPFEATURESIMPORTANCEENTRY._serialized_start=10470
-  _EXPLAINRESPONSE_SHAPFEATURESIMPORTANCEENTRY._serialized_end=10531
-  _TRAINERDSERVICE._serialized_start=10534
-  _TRAINERDSERVICE._serialized_end=11787
+  _TRAINREQUEST._serialized_end=1132
+  _TRAINRESPONSE._serialized_start=1135
+  _TRAINRESPONSE._serialized_end=2116
+  _TRAINRESPONSE_PIPFREEZEENTRY._serialized_start=2002
+  _TRAINRESPONSE_PIPFREEZEENTRY._serialized_end=2050
+  _TRAINRESPONSE_IMPURITYFEATUREIMPORTANCEENTRY._serialized_start=2052
+  _TRAINRESPONSE_IMPURITYFEATUREIMPORTANCEENTRY._serialized_end=2116
+  _COMPILEREQUEST._serialized_start=2119
+  _COMPILEREQUEST._serialized_end=2722
+  _COMPILERESPONSE._serialized_start=2724
+  _COMPILERESPONSE._serialized_end=2767
+  _TESTREQUEST._serialized_start=2770
+  _TESTREQUEST._serialized_end=3455
+  _TESTRESPONSE._serialized_start=3458
+  _TESTRESPONSE._serialized_end=4367
+  _TESTRESPONSE_PERMUTATIONFEATUREIMPORTANCEENTRY._serialized_start=4300
+  _TESTRESPONSE_PERMUTATIONFEATUREIMPORTANCEENTRY._serialized_end=4367
+  _TRAINDRIFTDETECTORREQUEST._serialized_start=4370
+  _TRAINDRIFTDETECTORREQUEST._serialized_end=5063
+  _FORECASTREQUEST._serialized_start=5066
+  _FORECASTREQUEST._serialized_end=5670
+  _FORECASTRESPONSE._serialized_start=5672
+  _FORECASTRESPONSE._serialized_end=5787
+  _SHUTDOWNREQUEST._serialized_start=5789
+  _SHUTDOWNREQUEST._serialized_end=5806
+  _SHUTDOWNRESPONSE._serialized_start=5808
+  _SHUTDOWNRESPONSE._serialized_end=5826
+  _EXPLAINREQUEST._serialized_start=5829
+  _EXPLAINREQUEST._serialized_end=6432
+  _EXPLAINRESPONSE._serialized_start=6435
+  _EXPLAINRESPONSE._serialized_end=6757
+  _TRAINERDSERVICE._serialized_start=6760
+  _TRAINERDSERVICE._serialized_end=7694
 # @@protoc_insertion_point(module_scope)
```

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,29 +30,19 @@
                 response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_trainerd_dot_v1_dot_trainerd__pb2.ForecastResponse.FromString,
                 )
         self.Test = channel.unary_unary(
                 '/github.com.metaprov.modelaapi.services.trainerd.v1.TrainerdService/Test',
                 request_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_trainerd_dot_v1_dot_trainerd__pb2.TestRequest.SerializeToString,
                 response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_trainerd_dot_v1_dot_trainerd__pb2.TestResponse.FromString,
                 )
-        self.TrainEnsemble = channel.unary_unary(
-                '/github.com.metaprov.modelaapi.services.trainerd.v1.TrainerdService/TrainEnsemble',
-                request_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_trainerd_dot_v1_dot_trainerd__pb2.TrainEnsembleRequest.SerializeToString,
-                response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_trainerd_dot_v1_dot_trainerd__pb2.TrainResponse.FromString,
-                )
         self.TrainDriftDetector = channel.unary_unary(
                 '/github.com.metaprov.modelaapi.services.trainerd.v1.TrainerdService/TrainDriftDetector',
                 request_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_trainerd_dot_v1_dot_trainerd__pb2.TrainDriftDetectorRequest.SerializeToString,
                 response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_trainerd_dot_v1_dot_trainerd__pb2.TrainResponse.FromString,
                 )
-        self.TestEnsemble = channel.unary_unary(
-                '/github.com.metaprov.modelaapi.services.trainerd.v1.TrainerdService/TestEnsemble',
-                request_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_trainerd_dot_v1_dot_trainerd__pb2.TestEnsembleRequest.SerializeToString,
-                response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_trainerd_dot_v1_dot_trainerd__pb2.TestResponse.FromString,
-                )
         self.Shutdown = channel.unary_unary(
                 '/github.com.metaprov.modelaapi.services.trainerd.v1.TrainerdService/Shutdown',
                 request_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_trainerd_dot_v1_dot_trainerd__pb2.ShutdownRequest.SerializeToString,
                 response_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_trainerd_dot_v1_dot_trainerd__pb2.ShutdownResponse.FromString,
                 )
 
 
@@ -79,32 +69,20 @@
 
     def Test(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def TrainEnsemble(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
     def TrainDriftDetector(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def TestEnsemble(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
     def Shutdown(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
@@ -126,29 +104,19 @@
                     response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_trainerd_dot_v1_dot_trainerd__pb2.ForecastResponse.SerializeToString,
             ),
             'Test': grpc.unary_unary_rpc_method_handler(
                     servicer.Test,
                     request_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_trainerd_dot_v1_dot_trainerd__pb2.TestRequest.FromString,
                     response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_trainerd_dot_v1_dot_trainerd__pb2.TestResponse.SerializeToString,
             ),
-            'TrainEnsemble': grpc.unary_unary_rpc_method_handler(
-                    servicer.TrainEnsemble,
-                    request_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_trainerd_dot_v1_dot_trainerd__pb2.TrainEnsembleRequest.FromString,
-                    response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_trainerd_dot_v1_dot_trainerd__pb2.TrainResponse.SerializeToString,
-            ),
             'TrainDriftDetector': grpc.unary_unary_rpc_method_handler(
                     servicer.TrainDriftDetector,
                     request_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_trainerd_dot_v1_dot_trainerd__pb2.TrainDriftDetectorRequest.FromString,
                     response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_trainerd_dot_v1_dot_trainerd__pb2.TrainResponse.SerializeToString,
             ),
-            'TestEnsemble': grpc.unary_unary_rpc_method_handler(
-                    servicer.TestEnsemble,
-                    request_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_trainerd_dot_v1_dot_trainerd__pb2.TestEnsembleRequest.FromString,
-                    response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_trainerd_dot_v1_dot_trainerd__pb2.TestResponse.SerializeToString,
-            ),
             'Shutdown': grpc.unary_unary_rpc_method_handler(
                     servicer.Shutdown,
                     request_deserializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_trainerd_dot_v1_dot_trainerd__pb2.ShutdownRequest.FromString,
                     response_serializer=github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_trainerd_dot_v1_dot_trainerd__pb2.ShutdownResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
@@ -225,31 +193,14 @@
         return grpc.experimental.unary_unary(request, target, '/github.com.metaprov.modelaapi.services.trainerd.v1.TrainerdService/Test',
             github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_trainerd_dot_v1_dot_trainerd__pb2.TestRequest.SerializeToString,
             github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_trainerd_dot_v1_dot_trainerd__pb2.TestResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def TrainEnsemble(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/github.com.metaprov.modelaapi.services.trainerd.v1.TrainerdService/TrainEnsemble',
-            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_trainerd_dot_v1_dot_trainerd__pb2.TrainEnsembleRequest.SerializeToString,
-            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_trainerd_dot_v1_dot_trainerd__pb2.TrainResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
     def TrainDriftDetector(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -259,31 +210,14 @@
         return grpc.experimental.unary_unary(request, target, '/github.com.metaprov.modelaapi.services.trainerd.v1.TrainerdService/TrainDriftDetector',
             github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_trainerd_dot_v1_dot_trainerd__pb2.TrainDriftDetectorRequest.SerializeToString,
             github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_trainerd_dot_v1_dot_trainerd__pb2.TrainResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def TestEnsemble(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/github.com.metaprov.modelaapi.services.trainerd.v1.TrainerdService/TestEnsemble',
-            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_trainerd_dot_v1_dot_trainerd__pb2.TestEnsembleRequest.SerializeToString,
-            github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_trainerd_dot_v1_dot_trainerd__pb2.TestResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
     def Shutdown(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py` & `modelaapi-0.6.200/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/google/api/annotations_pb2.py` & `modelaapi-0.6.200/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/google/api/http_pb2.py` & `modelaapi-0.6.200/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/k8s/io/api/apps/v1/generated_pb2.py` & `modelaapi-0.6.200/k8s/io/api/apps/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/k8s/io/api/core/v1/generated_pb2.py` & `modelaapi-0.6.200/k8s/io/api/core/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/k8s/io/api/rbac/v1/generated_pb2.py` & `modelaapi-0.6.200/k8s/io/api/rbac/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py` & `modelaapi-0.6.200/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py` & `modelaapi-0.6.200/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/k8s/io/apimachinery/pkg/runtime/generated_pb2.py` & `modelaapi-0.6.200/k8s/io/apimachinery/pkg/runtime/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py` & `modelaapi-0.6.200/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py` & `modelaapi-0.6.200/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/modelaapi/consts.py` & `modelaapi-0.6.200/modelaapi/consts.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/modelaapi/custom_transformers.py` & `modelaapi-0.6.200/modelaapi/custom_transformers.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/modelaapi/graykite_model.py` & `modelaapi-0.6.200/modelaapi/graykite_model.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/modelaapi/ts.py` & `modelaapi-0.6.200/modelaapi/ts.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/modelaapi/version.py` & `modelaapi-0.6.200/modelaapi/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ##########################################################################
 ## Module Info
 ##########################################################################
 
 __version_info__ = {
     "major": 0,
     "minor": 6,
-    "micro": 102,
+    "micro": 200,
     "releaselevel": "alpha",
     "post": 0,
     "serial": 1,
 }
 
 ##########################################################################
 ## Helper Functions
```

### Comparing `modelaapi-0.6.102/modelaapi.egg-info/PKG-INFO` & `modelaapi-0.6.200/modelaapi.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: modelaapi
-Version: 0.6.102
+Version: 0.6.200
 Summary: A suite of automatic machine learning for kubernetes
 Home-page: http://www.modela.ai
 Author: The modelaapi developers
 Author-email: info@modela.ai
 Maintainer: The modela developers
 Maintainer-email: info@modela.ai
 License: Apache 2
-Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.102
+Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.200
 Project-URL: Documentation, http://www.modela.ai
-Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.102
+Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.200
 Project-URL: Source, https://github.com/metaprov/modelaapi
 Project-URL: Tracker, https://github.com/metaprov/modelaapi/issues
 Keywords: automl,machine learning,data science
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `modelaapi-0.6.102/modelaapi.egg-info/SOURCES.txt` & `modelaapi-0.6.200/modelaapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/setup.cfg` & `modelaapi-0.6.200/setup.cfg`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.102/setup.py` & `modelaapi-0.6.200/setup.py`

 * *Files identical despite different names*

