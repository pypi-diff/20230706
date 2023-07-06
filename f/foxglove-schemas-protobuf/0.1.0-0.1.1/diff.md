# Comparing `tmp/foxglove-schemas-protobuf-0.1.0.tar.gz` & `tmp/foxglove-schemas-protobuf-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxglove-schemas-protobuf-0.1.0.tar", last modified: Tue Apr 18 22:45:48 2023, max compression
+gzip compressed data, was "foxglove-schemas-protobuf-0.1.1.tar", last modified: Thu Jul  6 16:59:41 2023, max compression
```

## Comparing `foxglove-schemas-protobuf-0.1.0.tar` & `foxglove-schemas-protobuf-0.1.1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:45:48.239673 foxglove-schemas-protobuf-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-18 22:45:48.239673 foxglove-schemas-protobuf-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-18 22:44:58.000000 foxglove-schemas-protobuf-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:45:48.239673 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/ArrowPrimitive_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/ArrowPrimitive_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CameraCalibration_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CameraCalibration_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CircleAnnotation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CircleAnnotation_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Color_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Color_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CompressedImage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CompressedImage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CubePrimitive_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CubePrimitive_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CylinderPrimitive_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CylinderPrimitive_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/FrameTransform_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/FrameTransform_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/FrameTransforms_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/FrameTransforms_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/GeoJSON_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/GeoJSON_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Grid_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Grid_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/ImageAnnotations_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/ImageAnnotations_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/KeyValuePair_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/KeyValuePair_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/LaserScan_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/LaserScan_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/LinePrimitive_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/LinePrimitive_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/LocationFix_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/LocationFix_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Log_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Log_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/ModelPrimitive_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/ModelPrimitive_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PackedElementField_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PackedElementField_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Point2_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Point2_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Point3_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Point3_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PointCloud_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PointCloud_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PointsAnnotation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PointsAnnotation_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PoseInFrame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PoseInFrame_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Pose_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Pose_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PosesInFrame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PosesInFrame_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Quaternion_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Quaternion_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/RawImage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/RawImage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/SceneEntityDeletion_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/SceneEntityDeletion_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/SceneEntity_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/SceneEntity_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/SceneUpdate_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/SceneUpdate_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/SpherePrimitive_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/SpherePrimitive_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/TextAnnotation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/TextAnnotation_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/TextPrimitive_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/TextPrimitive_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/TriangleListPrimitive_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/TriangleListPrimitive_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Vector2_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Vector2_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Vector3_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-18 22:45:35.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Vector3_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:44:58.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:44:58.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:45:48.239673 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-18 22:45:48.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-04-18 22:45:48.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 22:45:48.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 22:45:48.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-18 22:45:48.000000 foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-18 22:44:58.000000 foxglove-schemas-protobuf-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-18 22:45:48.243672 foxglove-schemas-protobuf-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:45:48.239673 foxglove-schemas-protobuf-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-18 22:44:58.000000 foxglove-schemas-protobuf-0.1.0/tests/test_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:59:41.011784 foxglove-schemas-protobuf-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-06 16:59:41.011784 foxglove-schemas-protobuf-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-06 16:59:00.000000 foxglove-schemas-protobuf-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:59:41.007784 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/ArrowPrimitive_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/ArrowPrimitive_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/CameraCalibration_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/CameraCalibration_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/CircleAnnotation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/CircleAnnotation_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Color_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Color_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/CompressedImage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/CompressedImage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/CubePrimitive_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/CubePrimitive_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/CylinderPrimitive_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/CylinderPrimitive_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/FrameTransform_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/FrameTransform_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/FrameTransforms_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/FrameTransforms_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/GeoJSON_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/GeoJSON_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Grid_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Grid_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/ImageAnnotations_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/ImageAnnotations_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/KeyValuePair_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/KeyValuePair_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/LaserScan_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/LaserScan_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/LinePrimitive_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/LinePrimitive_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/LocationFix_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/LocationFix_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Log_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Log_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/ModelPrimitive_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/ModelPrimitive_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/PackedElementField_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/PackedElementField_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Point2_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Point2_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Point3_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Point3_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/PointCloud_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/PointCloud_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/PointsAnnotation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/PointsAnnotation_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/PoseInFrame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/PoseInFrame_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Pose_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Pose_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/PosesInFrame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/PosesInFrame_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Quaternion_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Quaternion_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/RawImage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/RawImage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/SceneEntityDeletion_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/SceneEntityDeletion_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/SceneEntity_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/SceneEntity_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/SceneUpdate_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/SceneUpdate_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/SpherePrimitive_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/SpherePrimitive_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/TextAnnotation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/TextAnnotation_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/TextPrimitive_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/TextPrimitive_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/TriangleListPrimitive_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/TriangleListPrimitive_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Vector2_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Vector2_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Vector3_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-06 16:59:31.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Vector3_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:59:00.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:59:00.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:59:41.011784 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-06 16:59:40.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-07-06 16:59:40.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 16:59:40.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 16:59:40.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 16:59:40.000000 foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-06 16:59:00.000000 foxglove-schemas-protobuf-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-06 16:59:41.011784 foxglove-schemas-protobuf-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:59:41.011784 foxglove-schemas-protobuf-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-06 16:59:00.000000 foxglove-schemas-protobuf-0.1.1/tests/test_schemas.py
```

### Comparing `foxglove-schemas-protobuf-0.1.0/PKG-INFO` & `foxglove-schemas-protobuf-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxglove-schemas-protobuf
-Version: 0.1.0
+Version: 0.1.1
 Summary: Protobuf classes for Foxglove Schemas
 Home-page: https://github.com/foxglove/schemas
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `foxglove-schemas-protobuf-0.1.0/README.md` & `foxglove-schemas-protobuf-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/ArrowPrimitive_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/ArrowPrimitive_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/ArrowPrimitive_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/ArrowPrimitive_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CameraCalibration_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/CameraCalibration_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CameraCalibration_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/CameraCalibration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CircleAnnotation_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/CircleAnnotation_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CircleAnnotation_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/CircleAnnotation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Color_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Color_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Color_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Color_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CompressedImage_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/CompressedImage_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CompressedImage_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/CompressedImage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CubePrimitive_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/CubePrimitive_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CubePrimitive_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/CubePrimitive_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CylinderPrimitive_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/CylinderPrimitive_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/CylinderPrimitive_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/CylinderPrimitive_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/FrameTransform_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/FrameTransform_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/FrameTransform_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/FrameTransform_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/FrameTransforms_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/FrameTransforms_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/FrameTransforms_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/FrameTransforms_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/GeoJSON_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/GeoJSON_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/GeoJSON_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/GeoJSON_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Grid_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Grid_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Grid_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Grid_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/ImageAnnotations_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/ImageAnnotations_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/ImageAnnotations_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/ImageAnnotations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/KeyValuePair_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/KeyValuePair_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/KeyValuePair_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/KeyValuePair_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/LaserScan_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/LaserScan_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/LaserScan_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/LaserScan_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/LinePrimitive_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/LinePrimitive_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/LinePrimitive_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/LinePrimitive_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/LocationFix_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/LocationFix_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x66oxglove/LocationFix.proto\x12\x08\x66oxglove\"\x89\x02\n\x0bLocationFix\x12\x10\n\x08latitude\x18\x01 \x01(\x01\x12\x11\n\tlongitude\x18\x02 \x01(\x01\x12\x10\n\x08\x61ltitude\x18\x03 \x01(\x01\x12\x1b\n\x13position_covariance\x18\x04 \x03(\x01\x12N\n\x18position_covariance_type\x18\x05 \x01(\x0e\x32,.foxglove.LocationFix.PositionCovarianceType\"V\n\x16PositionCovarianceType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x10\n\x0c\x41PPROXIMATED\x10\x01\x12\x12\n\x0e\x44IAGONAL_KNOWN\x10\x02\x12\t\n\x05KNOWN\x10\x03\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x66oxglove/LocationFix.proto\x12\x08\x66oxglove\x1a\x1fgoogle/protobuf/timestamp.proto\"\xca\x02\n\x0bLocationFix\x12-\n\ttimestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08\x66rame_id\x18\x07 \x01(\t\x12\x10\n\x08latitude\x18\x01 \x01(\x01\x12\x11\n\tlongitude\x18\x02 \x01(\x01\x12\x10\n\x08\x61ltitude\x18\x03 \x01(\x01\x12\x1b\n\x13position_covariance\x18\x04 \x03(\x01\x12N\n\x18position_covariance_type\x18\x05 \x01(\x0e\x32,.foxglove.LocationFix.PositionCovarianceType\"V\n\x16PositionCovarianceType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x10\n\x0c\x41PPROXIMATED\x10\x01\x12\x12\n\x0e\x44IAGONAL_KNOWN\x10\x02\x12\t\n\x05KNOWN\x10\x03\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'foxglove.LocationFix_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _LOCATIONFIX._serialized_start=41
-  _LOCATIONFIX._serialized_end=306
-  _LOCATIONFIX_POSITIONCOVARIANCETYPE._serialized_start=220
-  _LOCATIONFIX_POSITIONCOVARIANCETYPE._serialized_end=306
+  _LOCATIONFIX._serialized_start=74
+  _LOCATIONFIX._serialized_end=404
+  _LOCATIONFIX_POSITIONCOVARIANCETYPE._serialized_start=318
+  _LOCATIONFIX_POSITIONCOVARIANCETYPE._serialized_end=404
 # @@protoc_insertion_point(module_scope)
```

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/LocationFix_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/LocationFix_pb2.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Generated by https://github.com/foxglove/schemas"""
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
+import google.protobuf.timestamp_pb2
 import sys
 import typing
 
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
@@ -39,19 +40,26 @@
         """Type of position covariance"""
 
     UNKNOWN: LocationFix.PositionCovarianceType.ValueType  # 0
     APPROXIMATED: LocationFix.PositionCovarianceType.ValueType  # 1
     DIAGONAL_KNOWN: LocationFix.PositionCovarianceType.ValueType  # 2
     KNOWN: LocationFix.PositionCovarianceType.ValueType  # 3
 
+    TIMESTAMP_FIELD_NUMBER: builtins.int
+    FRAME_ID_FIELD_NUMBER: builtins.int
     LATITUDE_FIELD_NUMBER: builtins.int
     LONGITUDE_FIELD_NUMBER: builtins.int
     ALTITUDE_FIELD_NUMBER: builtins.int
     POSITION_COVARIANCE_FIELD_NUMBER: builtins.int
     POSITION_COVARIANCE_TYPE_FIELD_NUMBER: builtins.int
+    @property
+    def timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp:
+        """Timestamp of the message"""
+    frame_id: builtins.str
+    """Frame for the sensor. Latitude and longitude readings are at the origin of the frame."""
     latitude: builtins.float
     """Latitude in degrees"""
     longitude: builtins.float
     """Longitude in degrees"""
     altitude: builtins.float
     """Altitude in meters"""
     @property
@@ -60,16 +68,19 @@
         length 9
         """
     position_covariance_type: global___LocationFix.PositionCovarianceType.ValueType
     """If `position_covariance` is available, `position_covariance_type` must be set to indicate the type of covariance."""
     def __init__(
         self,
         *,
+        timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
+        frame_id: builtins.str = ...,
         latitude: builtins.float = ...,
         longitude: builtins.float = ...,
         altitude: builtins.float = ...,
         position_covariance: collections.abc.Iterable[builtins.float] | None = ...,
         position_covariance_type: global___LocationFix.PositionCovarianceType.ValueType = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["altitude", b"altitude", "latitude", b"latitude", "longitude", b"longitude", "position_covariance", b"position_covariance", "position_covariance_type", b"position_covariance_type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["timestamp", b"timestamp"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["altitude", b"altitude", "frame_id", b"frame_id", "latitude", b"latitude", "longitude", b"longitude", "position_covariance", b"position_covariance", "position_covariance_type", b"position_covariance_type", "timestamp", b"timestamp"]) -> None: ...
 
 global___LocationFix = LocationFix
```

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Log_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Log_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Log_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Log_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/ModelPrimitive_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/ModelPrimitive_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/ModelPrimitive_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/ModelPrimitive_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PackedElementField_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/PackedElementField_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PackedElementField_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/PackedElementField_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Point2_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Point2_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Point2_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Point2_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Point3_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Point3_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Point3_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Point3_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PointCloud_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/PointCloud_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PointCloud_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/PointCloud_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PointsAnnotation_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/PointsAnnotation_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PointsAnnotation_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/PointsAnnotation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PoseInFrame_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/PoseInFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PoseInFrame_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/PoseInFrame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Pose_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Pose_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Pose_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Pose_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PosesInFrame_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/PosesInFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/PosesInFrame_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/PosesInFrame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Quaternion_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Quaternion_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Quaternion_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Quaternion_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/RawImage_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/RawImage_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/RawImage_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/RawImage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/SceneEntityDeletion_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/SceneEntityDeletion_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/SceneEntityDeletion_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/SceneEntityDeletion_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/SceneEntity_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/SceneEntity_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/SceneEntity_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/SceneEntity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/SceneUpdate_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/SceneUpdate_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/SceneUpdate_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/SceneUpdate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/SpherePrimitive_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/SpherePrimitive_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/SpherePrimitive_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/SpherePrimitive_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/TextAnnotation_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/TextAnnotation_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/TextAnnotation_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/TextAnnotation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/TextPrimitive_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/TextPrimitive_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/TextPrimitive_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/TextPrimitive_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/TriangleListPrimitive_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/TriangleListPrimitive_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/TriangleListPrimitive_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/TriangleListPrimitive_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Vector2_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Vector2_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Vector2_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Vector2_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Vector3_pb2.py` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Vector3_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf/Vector3_pb2.pyi` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf/Vector3_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf.egg-info/PKG-INFO` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxglove-schemas-protobuf
-Version: 0.1.0
+Version: 0.1.1
 Summary: Protobuf classes for Foxglove Schemas
 Home-page: https://github.com/foxglove/schemas
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `foxglove-schemas-protobuf-0.1.0/foxglove_schemas_protobuf.egg-info/SOURCES.txt` & `foxglove-schemas-protobuf-0.1.1/foxglove_schemas_protobuf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.1.0/setup.cfg` & `foxglove-schemas-protobuf-0.1.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [metadata]
 name = foxglove-schemas-protobuf
-version = 0.1.0
+version = 0.1.1
 description = Protobuf classes for Foxglove Schemas
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/foxglove/schemas
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 install_requires = 
-	protobuf
+	protobuf>=3.20.0
 install_package_data = True
 packages = find:
 python_requires = >=3.7
 
 [options.package_data]
 foxglove_schemas_protobuf = py.typed, *.pyi
```

