# Comparing `tmp/cvat_sdk-2.4.7.tar.gz` & `tmp/cvat_sdk-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvat_sdk-2.4.7.tar", last modified: Wed Jun 21 13:43:49 2023, max compression
+gzip compressed data, was "cvat_sdk-2.5.0.tar", last modified: Thu Jul  6 08:16:05 2023, max compression
```

## Comparing `cvat_sdk-2.4.7.tar` & `cvat_sdk-2.5.0.tar`

### file list

```diff
@@ -1,239 +1,248 @@
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:43:49.880040 cvat_sdk-2.4.7/
--rw-r--r--   0 andrey    (1000) andrey    (1000)       83 2023-04-05 10:02:25.000000 cvat_sdk-2.4.7/MANIFEST.in
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1463 2023-06-21 13:43:49.880040 cvat_sdk-2.4.7/PKG-INFO
--rw-r--r--   0 andrey    (1000) andrey    (1000)      989 2023-04-05 10:02:25.000000 cvat_sdk-2.4.7/README.md
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:43:49.850040 cvat_sdk-2.4.7/cvat_sdk/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      188 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/__init__.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:43:49.850040 cvat_sdk-2.4.7/cvat_sdk/api_client/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      767 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/__init__.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:43:49.860040 cvat_sdk-2.4.7/cvat_sdk/api_client/api/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      503 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    45482 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/auth_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    60873 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/cloudstorages_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    31388 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/comments_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15033 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/events_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    30703 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/invitations_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    31878 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/issues_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    92134 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/jobs_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    26740 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/labels_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    33105 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/lambda_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    24997 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/memberships_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    29848 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/organizations_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    75123 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/projects_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    53046 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/quality_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    10673 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/schema_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    21217 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/server_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)   131655 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/tasks_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    30201 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/users_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    65408 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/webhooks_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    45325 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api_client.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:43:49.860040 cvat_sdk-2.4.7/cvat_sdk/api_client/apis/
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1770 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/apis/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    19679 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/configuration.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     5132 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/exceptions.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:43:49.880040 cvat_sdk-2.4.7/cvat_sdk/api_client/model/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      353 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13042 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/about.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15100 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/annotation_conflict.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15328 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/annotation_conflict_type_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12460 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/annotation_file_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13969 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/annotation_id.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14124 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/annotation_id_shape_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13018 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/annotation_id_type_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15640 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/annotations_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14199 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/attribute.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13995 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/attribute_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12612 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/attribute_val.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12647 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/attribute_val_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14272 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/backup_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14112 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/basic_user.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13574 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/basic_user_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13023 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/chunk_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12999 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/client_events.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13105 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/client_events_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13139 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/cloud_storage_content.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17365 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/cloud_storage_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18328 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/cloud_storage_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14263 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/comment_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15468 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/comment_read_owner.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12658 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/comment_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12743 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/comments_summary.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14282 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/credentials_type_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16405 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/data_meta_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    33482 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/data_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12406 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/dataset_file_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13648 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/dataset_format.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12999 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/dataset_formats.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14276 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/dataset_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18298 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/event.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18849 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/event_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12988 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/events.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18731 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/events_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13186 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/file_info.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12821 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/file_info_type_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13644 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/frame_meta.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13071 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/frame_selection_method_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13367 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/input_type_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14184 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/invitation_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12807 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/invitation_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15954 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/issue_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14034 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/issue_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12590 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/issues_summary.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16288 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/job_annotations_update_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    22827 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/job_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15464 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/job_read_assignee.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13213 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/job_stage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13203 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/job_status.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13016 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/job_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17144 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/job_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13215 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/jobs_summary.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17310 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/label.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14504 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/labeled_data.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14752 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/labeled_data_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14732 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/labeled_image.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14901 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/labeled_image_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18094 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/labeled_shape.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18334 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/labeled_shape_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15751 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/labeled_track.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16062 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/labeled_track_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12590 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/labels_summary.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12981 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/location_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13020 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/login_serializer_ex_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14975 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/membership_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17616 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/meta_user.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12611 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/null_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12583 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/online_function_call_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13335 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/operation_status.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15424 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/organization_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13862 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/organization_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13703 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_annotation_conflict_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13674 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_cloud_storage_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13598 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_comment_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13643 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_invitation_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13568 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_issue_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13538 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_job_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13507 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_label_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13643 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_membership_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13553 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_meta_user_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13673 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_organization_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13598 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_project_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13628 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_quality_report_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13658 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_quality_settings_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13553 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_task_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13719 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_webhook_delivery_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13598 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_webhook_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13433 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/password_change_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13634 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/password_reset_confirm_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12417 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/password_reset_serializer_ex_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18255 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_cloud_storage_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12397 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_comment_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12418 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_data_meta_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12866 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_invitation_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13069 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_issue_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13342 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_job_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16560 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_label_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14787 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_labeled_data_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12514 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_membership_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13897 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_organization_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16059 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_project_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14845 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_project_write_request_target_storage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    21880 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_quality_settings_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16209 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_task_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14832 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_task_write_request_target_storage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16216 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_user_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14962 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_webhook_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13269 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/plugins.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12406 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/project_file_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    19106 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/project_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15469 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/project_read_owner.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14944 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/project_read_target_storage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16024 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/project_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13747 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/provider_type_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15893 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/quality_report.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12351 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/quality_report_create_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15291 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/quality_report_summary.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12851 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/quality_report_target.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    22444 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/quality_settings.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13363 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/register_serializer_ex.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14361 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/register_serializer_ex_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12298 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/rest_auth_detail.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13300 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/role_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12264 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/rq_id.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13564 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/rq_status.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13285 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/rq_status_state_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12891 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/severity_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13953 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/shape_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12299 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/signing_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13430 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/sorting_method.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13336 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/storage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12956 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/storage_method.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13074 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/storage_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13123 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/storage_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17568 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/sub_labeled_shape.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17737 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/sub_labeled_shape_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15225 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/sub_labeled_track.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15465 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/sub_labeled_track_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15279 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/sublabel.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15414 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/sublabel_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16291 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/task_annotations_update_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14338 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/task_annotations_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12352 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/task_file_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    23631 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/task_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14932 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/task_read_target_storage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17123 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/task_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12728 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/tasks_summary.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12255 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/token.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16249 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/tracked_shape.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16355 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/tracked_shape_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17571 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/user.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12666 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/webhook_content_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16432 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/webhook_delivery_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18535 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/webhook_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12991 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/webhook_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15742 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/webhook_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    84566 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model_utils.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:43:49.880040 cvat_sdk-2.4.7/cvat_sdk/api_client/models/
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15606 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/models/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14475 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/rest.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:43:49.880040 cvat_sdk-2.4.7/cvat_sdk/core/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      188 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12038 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/client.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     3115 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/downloading.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      353 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/exceptions.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1832 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/git.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     3061 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/helpers.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     3147 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/progress.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:43:49.880040 cvat_sdk-2.4.7/cvat_sdk/core/proxies/
--rw-r--r--   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/proxies/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     2116 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/proxies/annotations.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1737 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/proxies/issues.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     5550 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/proxies/jobs.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     5824 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/proxies/model_proxy.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      967 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/proxies/organizations.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     6652 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/proxies/projects.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14269 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/proxies/tasks.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      832 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/proxies/users.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14651 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/uploading.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     2103 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/utils.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      325 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/exceptions.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      167 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/models.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:43:49.880040 cvat_sdk-2.4.7/cvat_sdk/pytorch/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      362 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/pytorch/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    11405 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/pytorch/caching.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      969 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/pytorch/common.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     4303 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/pytorch/project_dataset.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     6982 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/pytorch/task_dataset.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     2885 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/pytorch/transforms.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)       18 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/version.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:43:49.880040 cvat_sdk-2.4.7/cvat_sdk.egg-info/
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1463 2023-06-21 13:43:49.000000 cvat_sdk-2.4.7/cvat_sdk.egg-info/PKG-INFO
--rw-r--r--   0 andrey    (1000) andrey    (1000)    10328 2023-06-21 13:43:49.000000 cvat_sdk-2.4.7/cvat_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)        1 2023-06-21 13:43:49.000000 cvat_sdk-2.4.7/cvat_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)      202 2023-06-21 13:43:49.000000 cvat_sdk-2.4.7/cvat_sdk.egg-info/requires.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)        9 2023-06-21 13:43:49.000000 cvat_sdk-2.4.7/cvat_sdk.egg-info/top_level.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)      383 2022-12-22 11:37:46.000000 cvat_sdk-2.4.7/pyproject.toml
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:43:49.880040 cvat_sdk-2.4.7/requirements/
--rw-r--r--   0 andrey    (1000) andrey    (1000)       64 2023-06-21 13:43:05.000000 cvat_sdk-2.4.7/requirements/api_client.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)      206 2023-04-05 10:02:25.000000 cvat_sdk-2.4.7/requirements/base.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)       38 2023-06-21 13:43:49.880040 cvat_sdk-2.4.7/setup.cfg
--rw-r--r--   0 andrey    (1000) andrey    (1000)     2753 2023-06-21 13:43:05.000000 cvat_sdk-2.4.7/setup.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:16:05.707215 cvat_sdk-2.5.0/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       83 2023-04-05 10:02:25.000000 cvat_sdk-2.5.0/MANIFEST.in
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1463 2023-07-06 08:16:05.707215 cvat_sdk-2.5.0/PKG-INFO
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      989 2023-04-05 10:02:25.000000 cvat_sdk-2.5.0/README.md
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:16:05.667215 cvat_sdk-2.5.0/cvat_sdk/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      188 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/__init__.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:16:05.667215 cvat_sdk-2.5.0/cvat_sdk/api_client/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      765 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/__init__.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:16:05.677215 cvat_sdk-2.5.0/cvat_sdk/api_client/api/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      503 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16495 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/assets_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    45480 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/auth_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    60871 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/cloudstorages_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    31386 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/comments_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15031 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/events_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    22684 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/guides_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    30701 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/invitations_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    31876 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/issues_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    92132 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/jobs_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    26738 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/labels_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    34059 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/lambda_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    24995 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/memberships_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    29846 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/organizations_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    75121 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/projects_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    53044 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/quality_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    10671 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/schema_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    21215 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/server_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)   131653 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/tasks_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    30199 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/users_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    65406 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/webhooks_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    45517 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api_client.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:16:05.677215 cvat_sdk-2.5.0/cvat_sdk/api_client/apis/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1886 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/apis/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    19675 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/configuration.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     5130 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/exceptions.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:16:05.697215 cvat_sdk-2.5.0/cvat_sdk/api_client/model/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      353 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13040 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/about.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15098 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotation_conflict.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15326 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotation_conflict_type_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12458 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotation_file_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14274 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotation_guide_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13110 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotation_guide_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13967 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotation_id.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14122 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotation_id_shape_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13016 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotation_id_type_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15638 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotations_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13891 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/asset_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14197 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/attribute.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13993 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/attribute_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12610 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/attribute_val.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12645 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/attribute_val_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14270 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/backup_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14110 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/basic_user.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13572 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/basic_user_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13021 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/chunk_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12997 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/client_events.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13103 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/client_events_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13137 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/cloud_storage_content.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17473 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/cloud_storage_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15486 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/cloud_storage_read_owner.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18326 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/cloud_storage_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14307 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/comment_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12656 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/comment_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12741 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/comments_summary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14280 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/credentials_type_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16403 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/data_meta_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    33480 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/data_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12404 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/dataset_file_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13646 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/dataset_format.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12997 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/dataset_formats.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14274 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/dataset_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18296 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/event.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18847 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/event_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12986 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/events.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18729 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/events_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13184 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/file_info.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12819 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/file_info_type_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13642 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/frame_meta.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13069 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/frame_selection_method_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15273 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/function_call.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13574 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/function_call_params.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17192 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/function_call_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13365 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/input_type_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14394 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/invitation_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12805 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/invitation_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16023 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/issue_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14032 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/issue_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12588 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/issues_summary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16286 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/job_annotations_update_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    23239 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/job_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15462 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/job_read_assignee.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13211 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/job_stage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13201 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/job_status.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13014 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/job_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17142 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/job_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13538 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/jobs_summary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17308 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/label.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14502 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/labeled_data.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14750 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/labeled_data_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14730 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/labeled_image.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14899 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/labeled_image_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18092 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/labeled_shape.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18332 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/labeled_shape_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15749 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/labeled_track.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16060 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/labeled_track_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12588 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/labels_summary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12979 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/location_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13018 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/login_serializer_ex_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14973 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/membership_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17614 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/meta_user.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12609 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/null_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12581 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/online_function_call_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13333 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/operation_status.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15532 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/organization_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13860 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/organization_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13701 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_annotation_conflict_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13672 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_cloud_storage_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13596 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_comment_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13641 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_invitation_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13566 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_issue_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13536 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_job_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13505 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_label_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13641 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_membership_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13551 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_meta_user_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13671 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_organization_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13596 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_project_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13626 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_quality_report_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13656 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_quality_settings_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13551 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_task_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13717 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_webhook_delivery_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13596 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_webhook_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13431 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/password_change_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13632 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/password_reset_confirm_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12415 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/password_reset_serializer_ex_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13145 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_annotation_guide_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18253 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_cloud_storage_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12395 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_comment_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12416 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_data_meta_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12864 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_invitation_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13067 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_issue_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13340 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_job_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16558 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_label_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14785 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_labeled_data_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12512 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_membership_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13895 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_organization_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16057 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_project_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14843 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_project_write_request_target_storage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    21878 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_quality_settings_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16207 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_task_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14830 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_task_write_request_target_storage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16214 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_user_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14960 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_webhook_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13267 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/plugins.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12404 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/project_file_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    19348 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/project_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14942 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/project_read_target_storage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16022 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/project_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13745 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/provider_type_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12974 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/quality_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15891 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/quality_report.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12349 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/quality_report_create_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15289 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/quality_report_summary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12849 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/quality_report_target.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    22442 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/quality_settings.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13361 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/register_serializer_ex.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14359 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/register_serializer_ex_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12296 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/rest_auth_detail.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13298 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/role_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12262 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/rq_id.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13562 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/rq_status.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13283 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/rq_status_state_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12889 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/severity_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13951 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/shape_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12297 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/signing_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13428 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/sorting_method.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13334 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/storage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12954 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/storage_method.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13072 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/storage_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13121 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/storage_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17566 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/sub_labeled_shape.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17735 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/sub_labeled_shape_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15223 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/sub_labeled_track.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15463 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/sub_labeled_track_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15277 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/sublabel.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15412 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/sublabel_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16289 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/task_annotations_update_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14336 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/task_annotations_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12350 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/task_file_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    24013 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/task_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14930 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/task_read_target_storage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17121 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/task_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12726 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/tasks_summary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12253 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/token.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16247 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/tracked_shape.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16353 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/tracked_shape_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17569 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/user.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12664 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/webhook_content_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16430 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/webhook_delivery_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18524 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/webhook_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12989 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/webhook_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15740 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/webhook_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    84564 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model_utils.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:16:05.697215 cvat_sdk-2.5.0/cvat_sdk/api_client/models/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16348 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/models/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14473 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/rest.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:16:05.697215 cvat_sdk-2.5.0/cvat_sdk/core/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      188 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12038 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/client.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     3115 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/downloading.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      353 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/exceptions.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1832 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/git.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     3061 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/helpers.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     3147 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/progress.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:16:05.707215 cvat_sdk-2.5.0/cvat_sdk/core/proxies/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/proxies/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2116 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/proxies/annotations.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1737 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/proxies/issues.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     5550 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/proxies/jobs.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     5824 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/proxies/model_proxy.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      967 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/proxies/organizations.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     6652 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/proxies/projects.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14269 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/proxies/tasks.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      832 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/proxies/users.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14651 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/uploading.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2103 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/utils.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      325 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/exceptions.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      167 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/models.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:16:05.707215 cvat_sdk-2.5.0/cvat_sdk/pytorch/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      362 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/pytorch/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    11415 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/pytorch/caching.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      969 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/pytorch/common.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     4303 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/pytorch/project_dataset.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     6982 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/pytorch/task_dataset.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2885 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/pytorch/transforms.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       18 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/version.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:16:05.707215 cvat_sdk-2.5.0/cvat_sdk.egg-info/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1463 2023-07-06 08:16:05.000000 cvat_sdk-2.5.0/cvat_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    10785 2023-07-06 08:16:05.000000 cvat_sdk-2.5.0/cvat_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        1 2023-07-06 08:16:05.000000 cvat_sdk-2.5.0/cvat_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      202 2023-07-06 08:16:05.000000 cvat_sdk-2.5.0/cvat_sdk.egg-info/requires.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        9 2023-07-06 08:16:05.000000 cvat_sdk-2.5.0/cvat_sdk.egg-info/top_level.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      383 2022-12-22 11:37:46.000000 cvat_sdk-2.5.0/pyproject.toml
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:16:05.707215 cvat_sdk-2.5.0/requirements/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       64 2023-07-06 08:15:35.000000 cvat_sdk-2.5.0/requirements/api_client.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      206 2023-04-05 10:02:25.000000 cvat_sdk-2.5.0/requirements/base.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       38 2023-07-06 08:16:05.707215 cvat_sdk-2.5.0/setup.cfg
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2751 2023-07-06 08:15:35.000000 cvat_sdk-2.5.0/setup.py
```

### Comparing `cvat_sdk-2.4.7/PKG-INFO` & `cvat_sdk-2.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvat_sdk
-Version: 2.4.7
+Version: 2.5.0
 Summary: CVAT REST API
 Home-page: https://github.com/cvat-ai/cvat
 Author: CVAT.ai team
 Author-email: support@cvat.ai
 License: MIT License
 Keywords: OpenAPI,OpenAPI-Generator,CVAT REST API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cvat_sdk-2.4.7/README.md` & `cvat_sdk-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/__init__.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
-__version__ = "2.4.7"
+__version__ = "2.5.0"
 
 from cvat_sdk.api_client.api_client import ApiClient
 
 from cvat_sdk.api_client.configuration import Configuration
 
 from cvat_sdk.api_client.exceptions import OpenApiException
 from cvat_sdk.api_client.exceptions import ApiAttributeError
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/api/auth_api.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/api/auth_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/api/cloudstorages_api.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/api/cloudstorages_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/api/comments_api.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/api/comments_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/api/events_api.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/api/events_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -314,15 +314,15 @@
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
     ) -> typing.Tuple[typing.Optional[None], urllib3.HTTPResponse]:
         """Method returns csv log file   # noqa: E501
 
-        Recieve logs from the server  # noqa: E501
+        Receive logs from the server  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.list(_async_call=True)
         >>> result = thread.get()
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/api/invitations_api.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/api/invitations_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/api/issues_api.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/api/issues_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/api/jobs_api.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/api/jobs_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/api/labels_api.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/api/labels_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/api/lambda_api.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/api/lambda_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -21,14 +21,16 @@
 from cvat_sdk.api_client.api_client import ApiClient, Endpoint as _Endpoint
 from cvat_sdk.api_client.model_utils import (  # noqa: F401
     date,
     datetime,
     file_type,
     none_type,
 )
+from cvat_sdk.api_client.model.function_call import FunctionCall
+from cvat_sdk.api_client.model.function_call_request import FunctionCallRequest
 from cvat_sdk.api_client.model.online_function_call_request import OnlineFunctionCallRequest
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
@@ -109,70 +111,80 @@
                     'application/json'
                 ]
             },
             api_client=api_client
         )
         self.create_requests_endpoint = _Endpoint(
             settings={
-                'response_schema': None,
+                'response_schema': (FunctionCall,),
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
                     'signatureAuth',
                     'tokenAuth'
                 ],
                 'endpoint_path': '/api/lambda/requests',
                 'operation_id': 'create_requests',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
+                    'function_call_request',
                     'x_organization',
                     'org',
                     'org_id',
                 ],
-                'required': [],
+                'required': [
+                    'function_call_request',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
+                    'function_call_request':
+                        (FunctionCallRequest,),
                     'x_organization':
                         (str,),
                     'org':
                         (str,),
                     'org_id':
                         (int,),
                 },
                 'attribute_map': {
                     'x_organization': 'X-Organization',
                     'org': 'org',
                     'org_id': 'org_id',
                 },
                 'location_map': {
+                    'function_call_request': 'body',
                     'x_organization': 'header',
                     'org': 'query',
                     'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
-                'accept': [],
-                'content_type': [],
+                'accept': [
+                    'application/vnd.cvat+json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
             },
             api_client=api_client
         )
         self.list_functions_endpoint = _Endpoint(
             settings={
                 'response_schema': None,
                 'auth': [
@@ -216,15 +228,15 @@
                 'accept': [],
                 'content_type': [],
             },
             api_client=api_client
         )
         self.list_requests_endpoint = _Endpoint(
             settings={
-                'response_schema': None,
+                'response_schema': ([FunctionCall],),
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
                     'signatureAuth',
                     'tokenAuth'
                 ],
@@ -255,15 +267,17 @@
                 },
                 'location_map': {
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
-                'accept': [],
+                'accept': [
+                    'application/vnd.cvat+json'
+                ],
                 'content_type': [],
             },
             api_client=api_client
         )
         self.retrieve_functions_endpoint = _Endpoint(
             settings={
                 'response_schema': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
@@ -324,15 +338,15 @@
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
         self.retrieve_requests_endpoint = _Endpoint(
             settings={
-                'response_schema': None,
+                'response_schema': (FunctionCall,),
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
                     'signatureAuth',
                     'tokenAuth'
                 ],
@@ -358,27 +372,29 @@
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
-                        (int,),
+                        (str,),
                 },
                 'attribute_map': {
                     'id': 'id',
                 },
                 'location_map': {
                     'id': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
-                'accept': [],
+                'accept': [
+                    'application/vnd.cvat+json'
+                ],
                 'content_type': [],
             },
             api_client=api_client
         )
 
     def create_functions(
         self,
@@ -458,35 +474,38 @@
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
         kwargs['func_id'] = func_id
         return self.create_functions_endpoint.call_with_http_info(**kwargs)
 
     def create_requests(
         self,
+        function_call_request: FunctionCallRequest,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
         _validate_outputs: bool = True,
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
-    ) -> typing.Tuple[typing.Optional[None], urllib3.HTTPResponse]:
+    ) -> typing.Tuple[typing.Optional[FunctionCall], urllib3.HTTPResponse]:
         """Method calls the function  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
-        >>> thread = api.create_requests(_async_call=True)
+        >>> thread = api.create_requests(function_call_request, _async_call=True)
         >>> result = thread.get()
 
+        Args:
+            function_call_request (FunctionCallRequest):
 
         Keyword Args:
             x_organization (str): Organization unique slug. [optional]
             org (str): Organization unique slug. [optional]
             org_id (int): Organization identifier. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
@@ -517,28 +536,29 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             _async_call (bool): execute request asynchronously
 
         Returns:
-            (None, HTTPResponse)
+            (FunctionCall, HTTPResponse)
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['_async_call'] = _async_call
         kwargs['_parse_response'] = _parse_response
         kwargs['_request_timeout'] = _request_timeout
         kwargs['_validate_inputs'] = _validate_inputs
         kwargs['_validate_outputs'] = _validate_outputs
         kwargs['_check_status'] = _check_status
         kwargs['_spec_property_naming'] = _spec_property_naming
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
+        kwargs['function_call_request'] = function_call_request
         return self.create_requests_endpoint.call_with_http_info(**kwargs)
 
     def list_functions(
         self,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
@@ -621,15 +641,15 @@
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
-    ) -> typing.Tuple[typing.Optional[None], urllib3.HTTPResponse]:
+    ) -> typing.Tuple[typing.Optional[typing.List[FunctionCall]], urllib3.HTTPResponse]:
         """Method returns a list of requests  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.list_requests(_async_call=True)
         >>> result = thread.get()
@@ -665,15 +685,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             _async_call (bool): execute request asynchronously
 
         Returns:
-            (None, HTTPResponse)
+            ([FunctionCall], HTTPResponse)
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['_async_call'] = _async_call
         kwargs['_parse_response'] = _parse_response
         kwargs['_request_timeout'] = _request_timeout
         kwargs['_validate_inputs'] = _validate_inputs
@@ -761,38 +781,38 @@
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
         kwargs['func_id'] = func_id
         return self.retrieve_functions_endpoint.call_with_http_info(**kwargs)
 
     def retrieve_requests(
         self,
-        id: int,
+        id: str,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
         _validate_outputs: bool = True,
         _check_status: bool = True,
         _spec_property_naming: bool = False,
         _content_type: typing.Optional[str] = None,
         _host_index: typing.Optional[int] = None,
         _request_auths: typing.Optional[typing.List] = None,
         _async_call: bool = False,
         **kwargs,
-    ) -> typing.Tuple[typing.Optional[None], urllib3.HTTPResponse]:
+    ) -> typing.Tuple[typing.Optional[FunctionCall], urllib3.HTTPResponse]:
         """Method returns the status of the request  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
         >>> thread = api.retrieve_requests(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
-            id (int): Request id
+            id (str): Request id
 
         Keyword Args:
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -820,15 +840,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             _async_call (bool): execute request asynchronously
 
         Returns:
-            (None, HTTPResponse)
+            (FunctionCall, HTTPResponse)
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['_async_call'] = _async_call
         kwargs['_parse_response'] = _parse_response
         kwargs['_request_timeout'] = _request_timeout
         kwargs['_validate_inputs'] = _validate_inputs
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/api/memberships_api.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/api/memberships_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/api/organizations_api.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/api/organizations_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/api/projects_api.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/api/projects_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/api/quality_api.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/api/quality_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/api/schema_api.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/api/schema_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/api/server_api.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/api/server_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/api/tasks_api.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/api/tasks_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/api/users_api.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/api/users_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/api/webhooks_api.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/api/webhooks_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/api_client.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import json
@@ -65,18 +65,20 @@
 
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
     Do not edit the class manually.
 
     Class members:
 
+    assets_api: AssetsApi
     auth_api: AuthApi
     cloudstorages_api: CloudstoragesApi
     comments_api: CommentsApi
     events_api: EventsApi
+    guides_api: GuidesApi
     invitations_api: InvitationsApi
     issues_api: IssuesApi
     jobs_api: JobsApi
     labels_api: LabelsApi
     lambda_api: LambdaApi
     memberships_api: MembershipsApi
     organizations_api: OrganizationsApi
@@ -111,15 +113,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers: typing.Dict[str, str] = headers or {}
         self.cookies = SimpleCookie()
         if cookies:
             self.cookies.update(cookies)
         # Set default User-Agent.
-        self.user_agent = 'cvat_sdk/2.4.7'
+        self.user_agent = 'cvat_sdk/2.5.0'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
@@ -716,18 +718,20 @@
             queries.append((auth_setting['key'], auth_setting['value']))
         else:
             raise ApiValueError(
                 'Authentication token must be in `query` or `header`'
             )
 
 
+    assets_api: 'AssetsApi'
     auth_api: 'AuthApi'
     cloudstorages_api: 'CloudstoragesApi'
     comments_api: 'CommentsApi'
     events_api: 'EventsApi'
+    guides_api: 'GuidesApi'
     invitations_api: 'InvitationsApi'
     issues_api: 'IssuesApi'
     jobs_api: 'JobsApi'
     labels_api: 'LabelsApi'
     lambda_api: 'LambdaApi'
     memberships_api: 'MembershipsApi'
     organizations_api: 'OrganizationsApi'
@@ -736,18 +740,20 @@
     schema_api: 'SchemaApi'
     server_api: 'ServerApi'
     tasks_api: 'TasksApi'
     users_api: 'UsersApi'
     webhooks_api: 'WebhooksApi'
 
     _apis: typing.Dict[str, object] = { 
+        'assets_api': [None, 'AssetsApi'],
         'auth_api': [None, 'AuthApi'],
         'cloudstorages_api': [None, 'CloudstoragesApi'],
         'comments_api': [None, 'CommentsApi'],
         'events_api': [None, 'EventsApi'],
+        'guides_api': [None, 'GuidesApi'],
         'invitations_api': [None, 'InvitationsApi'],
         'issues_api': [None, 'IssuesApi'],
         'jobs_api': [None, 'JobsApi'],
         'labels_api': [None, 'LabelsApi'],
         'lambda_api': [None, 'LambdaApi'],
         'memberships_api': [None, 'MembershipsApi'],
         'organizations_api': [None, 'OrganizationsApi'],
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/apis/__init__.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/apis/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,36 +3,38 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 # Import all APIs into this package.
 # If you have many APIs here with many many models used in each API this may
 # raise a `RecursionError`.
 # In order to avoid this, import only the API that you directly need like:
 #
-#   from cvat_sdk.api_client.api.auth_api import AuthApi
+#   from cvat_sdk.api_client.api.assets_api import AssetsApi
 #
 # or import this package, but before doing it, use:
 #
 #   import sys
 #   sys.setrecursionlimit(n)
 
 # Import APIs into API package:
+from cvat_sdk.api_client.api.assets_api import AssetsApi
 from cvat_sdk.api_client.api.auth_api import AuthApi
 from cvat_sdk.api_client.api.cloudstorages_api import CloudstoragesApi
 from cvat_sdk.api_client.api.comments_api import CommentsApi
 from cvat_sdk.api_client.api.events_api import EventsApi
+from cvat_sdk.api_client.api.guides_api import GuidesApi
 from cvat_sdk.api_client.api.invitations_api import InvitationsApi
 from cvat_sdk.api_client.api.issues_api import IssuesApi
 from cvat_sdk.api_client.api.jobs_api import JobsApi
 from cvat_sdk.api_client.api.labels_api import LabelsApi
 from cvat_sdk.api_client.api.lambda_api import LambdaApi
 from cvat_sdk.api_client.api.memberships_api import MembershipsApi
 from cvat_sdk.api_client.api.organizations_api import OrganizationsApi
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/configuration.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 import copy
 import logging
 import multiprocessing
@@ -484,16 +484,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 2.4.7\n"\
-               "SDK Package Version: 2.4.7".\
+               "Version of the API: 2.6\n"\
+               "SDK Package Version: 2.5.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/exceptions.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/about.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/about.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/annotation_conflict.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotation_conflict.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/annotation_conflict_type_enum.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotation_conflict_type_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/annotation_file_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotation_file_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/annotation_id.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotation_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/annotation_id_shape_type.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotation_id_shape_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/annotation_id_type_enum.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotation_id_type_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/annotations_read.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotations_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/attribute.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/attribute.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/attribute_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/attribute_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/attribute_val.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/attribute_val.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/attribute_val_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/attribute_val_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/backup_write_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/backup_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/basic_user.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/basic_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/basic_user_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/basic_user_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/chunk_type.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/chunk_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/client_events.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/client_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/client_events_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/client_events_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/cloud_storage_content.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/cloud_storage_content.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/cloud_storage_read.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/cloud_storage_read.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -40,18 +40,18 @@
 if TYPE_CHECKING:
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 def lazy_import():
-    from cvat_sdk.api_client.model.basic_user import BasicUser
+    from cvat_sdk.api_client.model.cloud_storage_read_owner import CloudStorageReadOwner
     from cvat_sdk.api_client.model.credentials_type_enum import CredentialsTypeEnum
     from cvat_sdk.api_client.model.provider_type_enum import ProviderTypeEnum
-    globals()['BasicUser'] = BasicUser
+    globals()['CloudStorageReadOwner'] = CloudStorageReadOwner
     globals()['CredentialsTypeEnum'] = CredentialsTypeEnum
     globals()['ProviderTypeEnum'] = ProviderTypeEnum
 
 
 
 class ICloudStorageRead(IModelData):
     """
@@ -63,15 +63,15 @@
 
     # member type declarations
     id: int # noqa: E501
     """
     [optional]
     """
 
-    owner: BasicUser # noqa: E501
+    owner: CloudStorageReadOwner # noqa: E501
     """
     [optional]
     """
 
     manifests: typing.List[str] # noqa: E501
     """
     [optional, default: []]
@@ -134,15 +134,15 @@
 
       display_name (str):
 
       credentials_type (CredentialsTypeEnum):
 
       id (int): [optional]  # noqa: E501
 
-      owner (BasicUser): [optional]  # noqa: E501
+      owner (CloudStorageReadOwner): [optional]  # noqa: E501
 
       manifests ([str]): [optional] if omitted the server will use the default value of []  # noqa: E501
 
       created_date (datetime): [optional]  # noqa: E501
 
       updated_date (datetime): [optional]  # noqa: E501
 
@@ -210,15 +210,15 @@
         lazy_import()
         return {
             'provider_type': (ProviderTypeEnum,),  # noqa: E501
             'resource': (str,),  # noqa: E501
             'display_name': (str,),  # noqa: E501
             'credentials_type': (CredentialsTypeEnum,),  # noqa: E501
             'id': (int,),  # noqa: E501
-            'owner': (BasicUser,),  # noqa: E501
+            'owner': (CloudStorageReadOwner,),  # noqa: E501
             'manifests': ([str],),  # noqa: E501
             'created_date': (datetime,),  # noqa: E501
             'updated_date': (datetime,),  # noqa: E501
             'specific_attributes': (str,),  # noqa: E501
             'description': (str,),  # noqa: E501
             'organization': (int, none_type,),  # noqa: E501
         }
@@ -263,15 +263,15 @@
             resource (str):
             display_name (str):
             credentials_type (CredentialsTypeEnum):
 
         Keyword Args:
             id (int): [optional]  # noqa: E501
 
-            owner (BasicUser): [optional]  # noqa: E501
+            owner (CloudStorageReadOwner): [optional]  # noqa: E501
 
             manifests ([str]): [optional] if omitted the server will use the default value of []  # noqa: E501
 
             created_date (datetime): [optional]  # noqa: E501
 
             updated_date (datetime): [optional]  # noqa: E501
 
@@ -375,15 +375,15 @@
             resource (str):
             display_name (str):
             credentials_type (CredentialsTypeEnum):
 
         Keyword Args:
             id (int): [optional]  # noqa: E501
 
-            owner (BasicUser): [optional]  # noqa: E501
+            owner (CloudStorageReadOwner): [optional]  # noqa: E501
 
             manifests ([str]): [optional] if omitted the server will use the default value of []  # noqa: E501
 
             created_date (datetime): [optional]  # noqa: E501
 
             updated_date (datetime): [optional]  # noqa: E501
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/cloud_storage_write_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/cloud_storage_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/comment_read.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/comment_read.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -40,16 +40,16 @@
 if TYPE_CHECKING:
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 def lazy_import():
-    from cvat_sdk.api_client.model.comment_read_owner import CommentReadOwner
-    globals()['CommentReadOwner'] = CommentReadOwner
+    from cvat_sdk.api_client.model.cloud_storage_read_owner import CloudStorageReadOwner
+    globals()['CloudStorageReadOwner'] = CloudStorageReadOwner
 
 
 
 class ICommentRead(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
@@ -64,15 +64,15 @@
     """
 
     issue: int # noqa: E501
     """
     [optional]
     """
 
-    owner: CommentReadOwner # noqa: E501
+    owner: CloudStorageReadOwner # noqa: E501
     """
     [optional]
     """
 
     message: str # noqa: E501
     """
     [optional]
@@ -97,15 +97,15 @@
     Do not edit the class manually.
 
     Attributes:
       id (int): [optional]  # noqa: E501
 
       issue (int): [optional]  # noqa: E501
 
-      owner (CommentReadOwner): [optional]  # noqa: E501
+      owner (CloudStorageReadOwner): [optional]  # noqa: E501
 
       message (str): [optional]  # noqa: E501
 
       created_date (datetime): [optional]  # noqa: E501
 
       updated_date (datetime): [optional]  # noqa: E501
 
@@ -155,15 +155,15 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'id': (int,),  # noqa: E501
             'issue': (int,),  # noqa: E501
-            'owner': (CommentReadOwner,),  # noqa: E501
+            'owner': (CloudStorageReadOwner,),  # noqa: E501
             'message': (str,),  # noqa: E501
             'created_date': (datetime,),  # noqa: E501
             'updated_date': (datetime,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
@@ -196,15 +196,15 @@
         """CommentRead - a model defined in OpenAPI
 
         Keyword Args:
             id (int): [optional]  # noqa: E501
 
             issue (int): [optional]  # noqa: E501
 
-            owner (CommentReadOwner): [optional]  # noqa: E501
+            owner (CloudStorageReadOwner): [optional]  # noqa: E501
 
             message (str): [optional]  # noqa: E501
 
             created_date (datetime): [optional]  # noqa: E501
 
             updated_date (datetime): [optional]  # noqa: E501
 
@@ -294,15 +294,15 @@
         """CommentRead - a model defined in OpenAPI
 
         Keyword Args:
             id (int): [optional]  # noqa: E501
 
             issue (int): [optional]  # noqa: E501
 
-            owner (CommentReadOwner): [optional]  # noqa: E501
+            owner (CloudStorageReadOwner): [optional]  # noqa: E501
 
             message (str): [optional]  # noqa: E501
 
             created_date (datetime): [optional]  # noqa: E501
 
             updated_date (datetime): [optional]  # noqa: E501
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/comment_read_owner.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/job_read_assignee.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -44,15 +44,15 @@
 
 
 def lazy_import():
     from cvat_sdk.api_client.model.basic_user import BasicUser
     globals()['BasicUser'] = BasicUser
 
 
-class CommentReadOwner(ModelComposed):
+class JobReadAssignee(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -137,16 +137,16 @@
     read_only_vars = {
         'url',  # noqa: E501
         'id',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, username, *args, **kwargs) -> CommentReadOwner:  # noqa: E501
-        """CommentReadOwner - a model defined in OpenAPI
+    def _from_openapi_data(cls, username, *args, **kwargs) -> JobReadAssignee:  # noqa: E501
+        """JobReadAssignee - a model defined in OpenAPI
 
         Keyword Args:
             username (str): Required. 150 characters or fewer. Letters, digits and @/./+/-/_ only.
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -251,15 +251,15 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, username, *args, **kwargs):  # noqa: E501
-        """CommentReadOwner - a model defined in OpenAPI
+        """JobReadAssignee - a model defined in OpenAPI
 
         Keyword Args:
             username (str): Required. 150 characters or fewer. Letters, digits and @/./+/-/_ only.
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/comment_write_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/comment_write_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/comments_summary.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/comments_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/credentials_type_enum.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/credentials_type_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/data_meta_read.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/data_meta_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/data_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/data_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/dataset_file_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/dataset_file_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/dataset_format.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/dataset_format.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/dataset_formats.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/dataset_formats.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/dataset_write_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/dataset_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/event.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/event_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/event_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/events.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/events_enum.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/events_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/file_info.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/file_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/file_info_type_enum.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/file_info_type_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/frame_meta.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/frame_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/frame_selection_method_enum.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/frame_selection_method_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/input_type_enum.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/input_type_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/invitation_read.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/asset_read.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -41,75 +41,69 @@
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 def lazy_import():
     from cvat_sdk.api_client.model.basic_user import BasicUser
-    from cvat_sdk.api_client.model.role_enum import RoleEnum
     globals()['BasicUser'] = BasicUser
-    globals()['RoleEnum'] = RoleEnum
 
 
 
-class IInvitationRead(IModelData):
+class IAssetRead(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     # member type declarations
-    key: str # noqa: E501
+    uuid: str # noqa: E501
     """
     [optional]
     """
 
-    created_date: datetime # noqa: E501
-    """
-    [optional]
-    """
-
-    owner: BasicUser # noqa: E501
+    filename: str # noqa: E501
     """
     """
 
-    role: RoleEnum # noqa: E501
+    created_date: datetime # noqa: E501
     """
+    [optional]
     """
 
-    user: BasicUser # noqa: E501
+    owner: BasicUser # noqa: E501
     """
+    [optional]
     """
 
-    organization: int # noqa: E501
+    guide_id: int # noqa: E501
     """
+    [optional]
     """
 
 
-class InvitationRead(ModelNormal, IInvitationRead):
+class AssetRead(ModelNormal, IAssetRead):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
-      owner (BasicUser):
+      filename (str):
 
-      role (RoleEnum):
+      uuid (str): [optional]  # noqa: E501
 
-      user (BasicUser):
-
-      organization (int):
+      created_date (datetime): [optional]  # noqa: E501
 
-      key (str): [optional]  # noqa: E501
+      owner (BasicUser): [optional]  # noqa: E501
 
-      created_date (datetime): [optional]  # noqa: E501
+      guide_id (int): [optional]  # noqa: E501
 
 
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
       attribute_map (dict): The key is attribute name
@@ -126,14 +120,17 @@
 
     """
 
     allowed_values = {
     }
 
     validations = {
+        ('filename',): {
+            'max_length': 1024,
+        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -151,60 +148,60 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'owner': (BasicUser,),  # noqa: E501
-            'role': (RoleEnum,),  # noqa: E501
-            'user': (BasicUser,),  # noqa: E501
-            'organization': (int,),  # noqa: E501
-            'key': (str,),  # noqa: E501
+            'filename': (str,),  # noqa: E501
+            'uuid': (str,),  # noqa: E501
             'created_date': (datetime,),  # noqa: E501
+            'owner': (BasicUser,),  # noqa: E501
+            'guide_id': (int,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
 
     attribute_map = {
-        'owner': 'owner',  # noqa: E501
-        'role': 'role',  # noqa: E501
-        'user': 'user',  # noqa: E501
-        'organization': 'organization',  # noqa: E501
-        'key': 'key',  # noqa: E501
+        'filename': 'filename',  # noqa: E501
+        'uuid': 'uuid',  # noqa: E501
         'created_date': 'created_date',  # noqa: E501
+        'owner': 'owner',  # noqa: E501
+        'guide_id': 'guide_id',  # noqa: E501
     }
 
     read_only_vars = {
-        'key',  # noqa: E501
+        'uuid',  # noqa: E501
         'created_date',  # noqa: E501
+        'guide_id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, owner, role, user, organization, *args, **kwargs):  # noqa: E501
-        """InvitationRead - a model defined in OpenAPI
+    def _from_openapi_data(cls, filename, *args, **kwargs):  # noqa: E501
+        """AssetRead - a model defined in OpenAPI
 
         Args:
-            owner (BasicUser):
-            role (RoleEnum):
-            user (BasicUser):
-            organization (int):
+            filename (str):
 
         Keyword Args:
-            key (str): [optional]  # noqa: E501
+            uuid (str): [optional]  # noqa: E501
 
             created_date (datetime): [optional]  # noqa: E501
 
+            owner (BasicUser): [optional]  # noqa: E501
+
+            guide_id (int): [optional]  # noqa: E501
+
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -259,18 +256,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.owner = owner
-        self.role = role
-        self.user = user
-        self.organization = organization
+        self.filename = filename
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -283,28 +277,29 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, owner, role, user, organization, *args, **kwargs):  # noqa: E501
-        """InvitationRead - a model defined in OpenAPI
+    def __init__(self, filename, *args, **kwargs):  # noqa: E501
+        """AssetRead - a model defined in OpenAPI
 
         Args:
-            owner (BasicUser):
-            role (RoleEnum):
-            user (BasicUser):
-            organization (int):
+            filename (str):
 
         Keyword Args:
-            key (str): [optional]  # noqa: E501
+            uuid (str): [optional]  # noqa: E501
 
             created_date (datetime): [optional]  # noqa: E501
 
+            owner (BasicUser): [optional]  # noqa: E501
+
+            guide_id (int): [optional]  # noqa: E501
+
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -357,18 +352,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.owner = owner
-        self.role = role
-        self.user = user
-        self.organization = organization
+        self.filename = filename
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/invitation_write_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/invitation_write_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/issue_read.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/issue_read.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -40,17 +40,17 @@
 if TYPE_CHECKING:
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 def lazy_import():
-    from cvat_sdk.api_client.model.comment_read_owner import CommentReadOwner
+    from cvat_sdk.api_client.model.cloud_storage_read_owner import CloudStorageReadOwner
     from cvat_sdk.api_client.model.comments_summary import CommentsSummary
-    globals()['CommentReadOwner'] = CommentReadOwner
+    globals()['CloudStorageReadOwner'] = CloudStorageReadOwner
     globals()['CommentsSummary'] = CommentsSummary
 
 
 
 class IIssueRead(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
@@ -76,20 +76,20 @@
     """
 
     job: int # noqa: E501
     """
     [optional]
     """
 
-    owner: CommentReadOwner # noqa: E501
+    owner: CloudStorageReadOwner # noqa: E501
     """
     [optional]
     """
 
-    assignee: CommentReadOwner # noqa: E501
+    assignee: CloudStorageReadOwner # noqa: E501
     """
     [optional]
     """
 
     created_date: typing.Union[datetime, none_type] # noqa: E501
     """
     [optional]
@@ -124,17 +124,17 @@
 
       id (int): [optional]  # noqa: E501
 
       frame (int): [optional]  # noqa: E501
 
       job (int): [optional]  # noqa: E501
 
-      owner (CommentReadOwner): [optional]  # noqa: E501
+      owner (CloudStorageReadOwner): [optional]  # noqa: E501
 
-      assignee (CommentReadOwner): [optional]  # noqa: E501
+      assignee (CloudStorageReadOwner): [optional]  # noqa: E501
 
       created_date (datetime, none_type): [optional]  # noqa: E501
 
       updated_date (datetime, none_type): [optional]  # noqa: E501
 
       resolved (bool): [optional]  # noqa: E501
 
@@ -187,16 +187,16 @@
         lazy_import()
         return {
             'position': ([float],),  # noqa: E501
             'comments': (CommentsSummary,),  # noqa: E501
             'id': (int,),  # noqa: E501
             'frame': (int,),  # noqa: E501
             'job': (int,),  # noqa: E501
-            'owner': (CommentReadOwner,),  # noqa: E501
-            'assignee': (CommentReadOwner,),  # noqa: E501
+            'owner': (CloudStorageReadOwner,),  # noqa: E501
+            'assignee': (CloudStorageReadOwner,),  # noqa: E501
             'created_date': (datetime, none_type,),  # noqa: E501
             'updated_date': (datetime, none_type,),  # noqa: E501
             'resolved': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
@@ -240,17 +240,17 @@
         Keyword Args:
             id (int): [optional]  # noqa: E501
 
             frame (int): [optional]  # noqa: E501
 
             job (int): [optional]  # noqa: E501
 
-            owner (CommentReadOwner): [optional]  # noqa: E501
+            owner (CloudStorageReadOwner): [optional]  # noqa: E501
 
-            assignee (CommentReadOwner): [optional]  # noqa: E501
+            assignee (CloudStorageReadOwner): [optional]  # noqa: E501
 
             created_date (datetime, none_type): [optional]  # noqa: E501
 
             updated_date (datetime, none_type): [optional]  # noqa: E501
 
             resolved (bool): [optional]  # noqa: E501
 
@@ -348,17 +348,17 @@
         Keyword Args:
             id (int): [optional]  # noqa: E501
 
             frame (int): [optional]  # noqa: E501
 
             job (int): [optional]  # noqa: E501
 
-            owner (CommentReadOwner): [optional]  # noqa: E501
+            owner (CloudStorageReadOwner): [optional]  # noqa: E501
 
-            assignee (CommentReadOwner): [optional]  # noqa: E501
+            assignee (CloudStorageReadOwner): [optional]  # noqa: E501
 
             created_date (datetime, none_type): [optional]  # noqa: E501
 
             updated_date (datetime, none_type): [optional]  # noqa: E501
 
             resolved (bool): [optional]  # noqa: E501
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/issue_write_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/issue_write_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/issues_summary.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/issues_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/job_annotations_update_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/job_annotations_update_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/job_read.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/job_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -93,14 +93,19 @@
     """
 
     assignee: JobReadAssignee # noqa: E501
     """
     [optional]
     """
 
+    guide_id: typing.Union[int, none_type] # noqa: E501
+    """
+    [optional]
+    """
+
     dimension: str # noqa: E501
     """
     [optional]
     """
 
     bug_tracker: typing.Union[str, none_type] # noqa: E501
     """
@@ -199,14 +204,16 @@
 
       task_id (int): [optional]  # noqa: E501
 
       project_id (int, none_type): [optional]  # noqa: E501
 
       assignee (JobReadAssignee): [optional]  # noqa: E501
 
+      guide_id (int, none_type): [optional]  # noqa: E501
+
       dimension (str): [optional]  # noqa: E501
 
       bug_tracker (str, none_type): [optional]  # noqa: E501
 
       status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
       stage (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
@@ -302,14 +309,15 @@
             'issues': (IssuesSummary,),  # noqa: E501
             'labels': (LabelsSummary,),  # noqa: E501
             'url': (str,),  # noqa: E501
             'id': (int,),  # noqa: E501
             'task_id': (int,),  # noqa: E501
             'project_id': (int, none_type,),  # noqa: E501
             'assignee': (JobReadAssignee,),  # noqa: E501
+            'guide_id': (int, none_type,),  # noqa: E501
             'dimension': (str,),  # noqa: E501
             'bug_tracker': (str, none_type,),  # noqa: E501
             'status': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'stage': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'state': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'mode': (str,),  # noqa: E501
             'frame_count': (int,),  # noqa: E501
@@ -333,14 +341,15 @@
         'issues': 'issues',  # noqa: E501
         'labels': 'labels',  # noqa: E501
         'url': 'url',  # noqa: E501
         'id': 'id',  # noqa: E501
         'task_id': 'task_id',  # noqa: E501
         'project_id': 'project_id',  # noqa: E501
         'assignee': 'assignee',  # noqa: E501
+        'guide_id': 'guide_id',  # noqa: E501
         'dimension': 'dimension',  # noqa: E501
         'bug_tracker': 'bug_tracker',  # noqa: E501
         'status': 'status',  # noqa: E501
         'stage': 'stage',  # noqa: E501
         'state': 'state',  # noqa: E501
         'mode': 'mode',  # noqa: E501
         'frame_count': 'frame_count',  # noqa: E501
@@ -355,14 +364,15 @@
     }
 
     read_only_vars = {
         'url',  # noqa: E501
         'id',  # noqa: E501
         'task_id',  # noqa: E501
         'project_id',  # noqa: E501
+        'guide_id',  # noqa: E501
         'dimension',  # noqa: E501
         'bug_tracker',  # noqa: E501
         'status',  # noqa: E501
         'stage',  # noqa: E501
         'state',  # noqa: E501
         'mode',  # noqa: E501
         'frame_count',  # noqa: E501
@@ -394,14 +404,16 @@
 
             task_id (int): [optional]  # noqa: E501
 
             project_id (int, none_type): [optional]  # noqa: E501
 
             assignee (JobReadAssignee): [optional]  # noqa: E501
 
+            guide_id (int, none_type): [optional]  # noqa: E501
+
             dimension (str): [optional]  # noqa: E501
 
             bug_tracker (str, none_type): [optional]  # noqa: E501
 
             status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
             stage (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
@@ -526,14 +538,16 @@
 
             task_id (int): [optional]  # noqa: E501
 
             project_id (int, none_type): [optional]  # noqa: E501
 
             assignee (JobReadAssignee): [optional]  # noqa: E501
 
+            guide_id (int, none_type): [optional]  # noqa: E501
+
             dimension (str): [optional]  # noqa: E501
 
             bug_tracker (str, none_type): [optional]  # noqa: E501
 
             status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
             stage (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/job_read_assignee.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/cloud_storage_read_owner.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -44,15 +44,15 @@
 
 
 def lazy_import():
     from cvat_sdk.api_client.model.basic_user import BasicUser
     globals()['BasicUser'] = BasicUser
 
 
-class JobReadAssignee(ModelComposed):
+class CloudStorageReadOwner(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -137,16 +137,16 @@
     read_only_vars = {
         'url',  # noqa: E501
         'id',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, username, *args, **kwargs) -> JobReadAssignee:  # noqa: E501
-        """JobReadAssignee - a model defined in OpenAPI
+    def _from_openapi_data(cls, username, *args, **kwargs) -> CloudStorageReadOwner:  # noqa: E501
+        """CloudStorageReadOwner - a model defined in OpenAPI
 
         Keyword Args:
             username (str): Required. 150 characters or fewer. Letters, digits and @/./+/-/_ only.
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -251,15 +251,15 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, username, *args, **kwargs):  # noqa: E501
-        """JobReadAssignee - a model defined in OpenAPI
+        """CloudStorageReadOwner - a model defined in OpenAPI
 
         Keyword Args:
             username (str): Required. 150 characters or fewer. Letters, digits and @/./+/-/_ only.
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/job_stage.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/job_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/job_status.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/job_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/job_type.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/job_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/job_write_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/job_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/jobs_summary.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/jobs_summary.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -55,17 +55,20 @@
 
     # member type declarations
     count: int # noqa: E501
     """
     [optional, default: 0]
     """
 
-    completed: int # noqa: E501
+    completed: typing.Union[int, none_type] # noqa: E501
+    """
+    """
+
+    validation: typing.Union[int, none_type] # noqa: E501
     """
-    [optional, default: 0]
     """
 
     url: str # noqa: E501
     """
     [optional]
     """
 
@@ -74,17 +77,19 @@
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
-      count (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
+      completed (int, none_type):
+
+      validation (int, none_type):
 
-      completed (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
+      count (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
 
       url (str): [optional]  # noqa: E501
 
 
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
@@ -126,47 +131,51 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
+            'completed': (int, none_type,),  # noqa: E501
+            'validation': (int, none_type,),  # noqa: E501
             'count': (int,),  # noqa: E501
-            'completed': (int,),  # noqa: E501
             'url': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
 
     attribute_map = {
-        'count': 'count',  # noqa: E501
         'completed': 'completed',  # noqa: E501
+        'validation': 'validation',  # noqa: E501
+        'count': 'count',  # noqa: E501
         'url': 'url',  # noqa: E501
     }
 
     read_only_vars = {
         'url',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, completed, validation, *args, **kwargs):  # noqa: E501
         """JobsSummary - a model defined in OpenAPI
 
+        Args:
+            completed (int, none_type):
+            validation (int, none_type):
+
         Keyword Args:
             count (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
 
-            completed (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
-
             url (str): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -223,14 +232,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.completed = completed
+        self.validation = validation
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -243,22 +254,24 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
+    def __init__(self, completed, validation, *args, **kwargs):  # noqa: E501
         """JobsSummary - a model defined in OpenAPI
 
+        Args:
+            completed (int, none_type):
+            validation (int, none_type):
+
         Keyword Args:
             count (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
 
-            completed (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
-
             url (str): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -313,14 +326,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.completed = completed
+        self.validation = validation
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/label.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/label.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/labeled_data.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/labeled_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/labeled_data_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/labeled_data_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/labeled_image.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/labeled_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/labeled_image_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/labeled_image_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/labeled_shape.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/labeled_shape.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/labeled_shape_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/labeled_shape_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/labeled_track.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/labeled_track.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/labeled_track_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/labeled_track_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/labels_summary.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/labels_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/location_enum.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/location_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/login_serializer_ex_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/login_serializer_ex_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/membership_read.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/membership_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/meta_user.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/meta_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/null_enum.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/null_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/online_function_call_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/online_function_call_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/operation_status.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/operation_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/organization_read.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/organization_read.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -40,16 +40,16 @@
 if TYPE_CHECKING:
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 def lazy_import():
-    from cvat_sdk.api_client.model.basic_user import BasicUser
-    globals()['BasicUser'] = BasicUser
+    from cvat_sdk.api_client.model.cloud_storage_read_owner import CloudStorageReadOwner
+    globals()['CloudStorageReadOwner'] = CloudStorageReadOwner
 
 
 
 class IOrganizationRead(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
@@ -90,28 +90,28 @@
 
     contact: typing.Dict[str, typing.Union[typing.Any, none_type]] # noqa: E501
     """
     [optional]
     {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
     """
 
-    owner: BasicUser # noqa: E501
+    owner: CloudStorageReadOwner # noqa: E501
     """
     """
 
 
 class OrganizationRead(ModelNormal, IOrganizationRead):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
-      owner (BasicUser):
+      owner (CloudStorageReadOwner):
 
       id (int): [optional]  # noqa: E501
 
       slug (str): [optional]  # noqa: E501
 
       name (str): [optional]  # noqa: E501
 
@@ -172,15 +172,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'owner': (BasicUser,),  # noqa: E501
+            'owner': (CloudStorageReadOwner,),  # noqa: E501
             'id': (int,),  # noqa: E501
             'slug': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'description': (str,),  # noqa: E501
             'created_date': (datetime,),  # noqa: E501
             'updated_date': (datetime,),  # noqa: E501
             'contact': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
@@ -217,15 +217,15 @@
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, owner, *args, **kwargs):  # noqa: E501
         """OrganizationRead - a model defined in OpenAPI
 
         Args:
-            owner (BasicUser):
+            owner (CloudStorageReadOwner):
 
         Keyword Args:
             id (int): [optional]  # noqa: E501
 
             slug (str): [optional]  # noqa: E501
 
             name (str): [optional]  # noqa: E501
@@ -321,15 +321,15 @@
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, owner, *args, **kwargs):  # noqa: E501
         """OrganizationRead - a model defined in OpenAPI
 
         Args:
-            owner (BasicUser):
+            owner (CloudStorageReadOwner):
 
         Keyword Args:
             id (int): [optional]  # noqa: E501
 
             slug (str): [optional]  # noqa: E501
 
             name (str): [optional]  # noqa: E501
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/organization_write_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/organization_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_annotation_conflict_list.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_annotation_conflict_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_cloud_storage_read_list.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_cloud_storage_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_comment_read_list.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_comment_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_invitation_read_list.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_invitation_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_issue_read_list.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_issue_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_job_read_list.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_job_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_label_list.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_label_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_membership_read_list.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_membership_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_meta_user_list.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_meta_user_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_organization_read_list.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_organization_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_project_read_list.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_project_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_quality_report_list.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_quality_report_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_quality_settings_list.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_quality_settings_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_task_read_list.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_task_read_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_webhook_delivery_read_list.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_webhook_delivery_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_webhook_read_list.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_webhook_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/password_change_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/password_change_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/password_reset_confirm_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/password_reset_confirm_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/password_reset_serializer_ex_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/password_reset_serializer_ex_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_cloud_storage_write_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_cloud_storage_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_comment_write_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_comment_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_data_meta_write_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_data_meta_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_invitation_write_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_invitation_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_issue_write_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_issue_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_job_write_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_job_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_label_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_label_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_labeled_data_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_labeled_data_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_membership_write_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_membership_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_organization_write_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_organization_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_project_write_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_project_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_project_write_request_target_storage.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_project_write_request_target_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_quality_settings_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_quality_settings_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_task_write_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_task_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_task_write_request_target_storage.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_task_write_request_target_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_user_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_user_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_webhook_write_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_webhook_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/plugins.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/plugins.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/project_file_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/project_file_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/project_read.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/project_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -43,21 +43,19 @@
     from cvat_sdk.api_client.models import *
 
 
 def lazy_import():
     from cvat_sdk.api_client.model.job_read_assignee import JobReadAssignee
     from cvat_sdk.api_client.model.job_status import JobStatus
     from cvat_sdk.api_client.model.labels_summary import LabelsSummary
-    from cvat_sdk.api_client.model.project_read_owner import ProjectReadOwner
     from cvat_sdk.api_client.model.project_read_target_storage import ProjectReadTargetStorage
     from cvat_sdk.api_client.model.tasks_summary import TasksSummary
     globals()['JobReadAssignee'] = JobReadAssignee
     globals()['JobStatus'] = JobStatus
     globals()['LabelsSummary'] = LabelsSummary
-    globals()['ProjectReadOwner'] = ProjectReadOwner
     globals()['ProjectReadTargetStorage'] = ProjectReadTargetStorage
     globals()['TasksSummary'] = TasksSummary
 
 
 
 class IProjectRead(IModelData):
     """
@@ -79,24 +77,29 @@
     """
 
     name: str # noqa: E501
     """
     [optional]
     """
 
-    owner: ProjectReadOwner # noqa: E501
+    owner: JobReadAssignee # noqa: E501
     """
     [optional]
     """
 
     assignee: JobReadAssignee # noqa: E501
     """
     [optional]
     """
 
+    guide_id: typing.Union[int, none_type] # noqa: E501
+    """
+    [optional]
+    """
+
     bug_tracker: str # noqa: E501
     """
     [optional]
     """
 
     task_subsets: typing.List[str] # noqa: E501
     """
@@ -162,18 +165,20 @@
 
       url (str): [optional]  # noqa: E501
 
       id (int): [optional]  # noqa: E501
 
       name (str): [optional]  # noqa: E501
 
-      owner (ProjectReadOwner): [optional]  # noqa: E501
+      owner (JobReadAssignee): [optional]  # noqa: E501
 
       assignee (JobReadAssignee): [optional]  # noqa: E501
 
+      guide_id (int, none_type): [optional]  # noqa: E501
+
       bug_tracker (str): [optional]  # noqa: E501
 
       task_subsets ([str]): [optional]  # noqa: E501
 
       created_date (datetime): [optional]  # noqa: E501
 
       updated_date (datetime): [optional]  # noqa: E501
@@ -240,16 +245,17 @@
         lazy_import()
         return {
             'tasks': (TasksSummary,),  # noqa: E501
             'labels': (LabelsSummary,),  # noqa: E501
             'url': (str,),  # noqa: E501
             'id': (int,),  # noqa: E501
             'name': (str,),  # noqa: E501
-            'owner': (ProjectReadOwner,),  # noqa: E501
+            'owner': (JobReadAssignee,),  # noqa: E501
             'assignee': (JobReadAssignee,),  # noqa: E501
+            'guide_id': (int, none_type,),  # noqa: E501
             'bug_tracker': (str,),  # noqa: E501
             'task_subsets': ([str],),  # noqa: E501
             'created_date': (datetime,),  # noqa: E501
             'updated_date': (datetime,),  # noqa: E501
             'status': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'dimension': (str, none_type,),  # noqa: E501
             'organization': (int, none_type,),  # noqa: E501
@@ -267,14 +273,15 @@
         'tasks': 'tasks',  # noqa: E501
         'labels': 'labels',  # noqa: E501
         'url': 'url',  # noqa: E501
         'id': 'id',  # noqa: E501
         'name': 'name',  # noqa: E501
         'owner': 'owner',  # noqa: E501
         'assignee': 'assignee',  # noqa: E501
+        'guide_id': 'guide_id',  # noqa: E501
         'bug_tracker': 'bug_tracker',  # noqa: E501
         'task_subsets': 'task_subsets',  # noqa: E501
         'created_date': 'created_date',  # noqa: E501
         'updated_date': 'updated_date',  # noqa: E501
         'status': 'status',  # noqa: E501
         'dimension': 'dimension',  # noqa: E501
         'organization': 'organization',  # noqa: E501
@@ -309,18 +316,20 @@
         Keyword Args:
             url (str): [optional]  # noqa: E501
 
             id (int): [optional]  # noqa: E501
 
             name (str): [optional]  # noqa: E501
 
-            owner (ProjectReadOwner): [optional]  # noqa: E501
+            owner (JobReadAssignee): [optional]  # noqa: E501
 
             assignee (JobReadAssignee): [optional]  # noqa: E501
 
+            guide_id (int, none_type): [optional]  # noqa: E501
+
             bug_tracker (str): [optional]  # noqa: E501
 
             task_subsets ([str]): [optional]  # noqa: E501
 
             created_date (datetime): [optional]  # noqa: E501
 
             updated_date (datetime): [optional]  # noqa: E501
@@ -429,18 +438,20 @@
         Keyword Args:
             url (str): [optional]  # noqa: E501
 
             id (int): [optional]  # noqa: E501
 
             name (str): [optional]  # noqa: E501
 
-            owner (ProjectReadOwner): [optional]  # noqa: E501
+            owner (JobReadAssignee): [optional]  # noqa: E501
 
             assignee (JobReadAssignee): [optional]  # noqa: E501
 
+            guide_id (int, none_type): [optional]  # noqa: E501
+
             bug_tracker (str): [optional]  # noqa: E501
 
             task_subsets ([str]): [optional]  # noqa: E501
 
             created_date (datetime): [optional]  # noqa: E501
 
             updated_date (datetime): [optional]  # noqa: E501
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/project_read_owner.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/register_serializer_ex.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -39,26 +39,62 @@
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
-def lazy_import():
-    from cvat_sdk.api_client.model.basic_user import BasicUser
-    globals()['BasicUser'] = BasicUser
 
 
-class ProjectReadOwner(ModelComposed):
-    """NOTE: This class is auto generated by OpenAPI Generator.
+class IRegisterSerializerEx(IModelData):
+    """
+    NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+    """
+
+    # member type declarations
+    username: str # noqa: E501
+    """
+    """
+
+    email: str # noqa: E501
+    """
+    [optional]
+    """
+
+    first_name: str # noqa: E501
+    """
+    [optional]
+    """
+
+    last_name: str # noqa: E501
+    """
+    [optional]
+    """
+
+
+class RegisterSerializerEx(ModelNormal, IRegisterSerializerEx):
+    """
+    NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
+      username (str):
+
+      email (str): [optional]  # noqa: E501
+
+      first_name (str): [optional]  # noqa: E501
+
+      last_name (str): [optional]  # noqa: E501
+
+
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
       attribute_map (dict): The key is attribute name
           and the value is json key in definition.
       discriminator_value_class_map (dict): A dict to go from the discriminator
@@ -66,90 +102,87 @@
       validations (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           that stores validations for max_length, min_length, max_items,
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
+
     """
 
     allowed_values = {
     }
 
     validations = {
         ('username',): {
             'max_length': 150,
-            'regex': {
-                'pattern': r'^[\w.@+-]+$',  # noqa: E501
-            },
-        },
-        ('first_name',): {
-            'max_length': 150,
-        },
-        ('last_name',): {
-            'max_length': 150,
+            'min_length': 5,
         },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
             'username': (str,),  # noqa: E501
-            'url': (str,),  # noqa: E501
-            'id': (int,),  # noqa: E501
+            'email': (str,),  # noqa: E501
             'first_name': (str,),  # noqa: E501
             'last_name': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
 
     attribute_map = {
         'username': 'username',  # noqa: E501
-        'url': 'url',  # noqa: E501
-        'id': 'id',  # noqa: E501
+        'email': 'email',  # noqa: E501
         'first_name': 'first_name',  # noqa: E501
         'last_name': 'last_name',  # noqa: E501
     }
 
     read_only_vars = {
-        'url',  # noqa: E501
-        'id',  # noqa: E501
     }
 
+    _composed_schemas = {}
+
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, username, *args, **kwargs) -> ProjectReadOwner:  # noqa: E501
-        """ProjectReadOwner - a model defined in OpenAPI
+    def _from_openapi_data(cls, username, *args, **kwargs):  # noqa: E501
+        """RegisterSerializerEx - a model defined in OpenAPI
+
+        Args:
+            username (str):
 
         Keyword Args:
-            username (str): Required. 150 characters or fewer. Letters, digits and @/./+/-/_ only.
+            email (str): [optional]  # noqa: E501
+
+            first_name (str): [optional]  # noqa: E501
+
+            last_name (str): [optional]  # noqa: E501
+
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -172,23 +205,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            url (str): [optional]  # noqa: E501
-            id (int): [optional]  # noqa: E501
-            first_name (str): [optional]  # noqa: E501
-            last_name (str): [optional]  # noqa: E501
-        """
+"""
         from cvat_sdk.api_client.configuration import Configuration
 
         _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', Configuration())
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         self = super(OpenApiModel, cls).__new__(cls)
 
         if args:
@@ -208,61 +237,48 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        constant_args = {
-            '_check_type': _check_type,
-            '_path_to_item': _path_to_item,
-            '_spec_property_naming': _spec_property_naming,
-            '_configuration': _configuration,
-            '_visited_composed_classes': self._visited_composed_classes,
-        }
-        required_args = {
-            'username': username,
-        }
-        kwargs.update(required_args)
-        composed_info = validate_get_composed_info(
-            constant_args, kwargs, self)
-        self._composed_instances = composed_info[0]
-        self._var_name_to_model_instances = composed_info[1]
-        self._additional_properties_model_instances = composed_info[2]
-        discarded_args = composed_info[3]
-
+        self.username = username
         for var_name, var_value in kwargs.items():
-            if var_name in discarded_args and \
+            if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
-                        self._additional_properties_model_instances:
+                        self.additional_properties_type is None:
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
-
         return self
 
     required_properties = set([
         '_data_store',
         '_check_type',
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
-        '_composed_instances',
-        '_var_name_to_model_instances',
-        '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, username, *args, **kwargs):  # noqa: E501
-        """ProjectReadOwner - a model defined in OpenAPI
+        """RegisterSerializerEx - a model defined in OpenAPI
+
+        Args:
+            username (str):
 
         Keyword Args:
-            username (str): Required. 150 characters or fewer. Letters, digits and @/./+/-/_ only.
+            email (str): [optional]  # noqa: E501
+
+            first_name (str): [optional]  # noqa: E501
+
+            last_name (str): [optional]  # noqa: E501
+
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -285,24 +301,21 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            url (str): [optional]  # noqa: E501
-            id (int): [optional]  # noqa: E501
-            first_name (str): [optional]  # noqa: E501
-            last_name (str): [optional]  # noqa: E501
-        """
+"""
+        from cvat_sdk.api_client.configuration import Configuration
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
+        _configuration = kwargs.pop('_configuration', Configuration())
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
             for arg in args:
                 if isinstance(arg, dict):
                     kwargs.update(arg)
                 else:
@@ -318,56 +331,20 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        constant_args = {
-            '_check_type': _check_type,
-            '_path_to_item': _path_to_item,
-            '_spec_property_naming': _spec_property_naming,
-            '_configuration': _configuration,
-            '_visited_composed_classes': self._visited_composed_classes,
-        }
-        required_args = {
-            'username': username,
-        }
-        kwargs.update(required_args)
-        composed_info = validate_get_composed_info(
-            constant_args, kwargs, self)
-        self._composed_instances = composed_info[0]
-        self._var_name_to_model_instances = composed_info[1]
-        self._additional_properties_model_instances = composed_info[2]
-        discarded_args = composed_info[3]
-
+        self.username = username
         for var_name, var_value in kwargs.items():
-            if var_name in discarded_args and \
+            if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
-                        self._additional_properties_model_instances:
+                        self.additional_properties_type is None:
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
             if var_name in self.read_only_vars:
                 raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
                                      f"class with read only attributes.")
 
-    @cached_property
-    def _composed_schemas():
-        # we need this here to make our import statements work
-        # we must store _composed_schemas in here so the code is only run
-        # when we invoke this method. If we kept this at the class
-        # level we would get an error because the class level
-        # code would be run when this module is imported, and these composed
-        # classes don't exist yet because their module has not finished
-        # loading
-        lazy_import()
-        return {
-          'anyOf': [
-          ],
-          'allOf': [
-              BasicUser,
-          ],
-          'oneOf': [
-          ],
-        }
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/project_read_target_storage.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/project_read_target_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/project_write_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/project_write_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/provider_type_enum.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/provider_type_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/quality_report.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/quality_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/quality_report_create_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/quality_report_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/quality_report_summary.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/quality_report_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/quality_report_target.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/quality_report_target.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/quality_settings.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/quality_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/register_serializer_ex.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/register_serializer_ex_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -41,15 +41,15 @@
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 
 
-class IRegisterSerializerEx(IModelData):
+class IRegisterSerializerExRequest(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
@@ -59,35 +59,47 @@
     """
 
     email: str # noqa: E501
     """
     [optional]
     """
 
+    password1: str # noqa: E501
+    """
+    """
+
+    password2: str # noqa: E501
+    """
+    """
+
     first_name: str # noqa: E501
     """
     [optional]
     """
 
     last_name: str # noqa: E501
     """
     [optional]
     """
 
 
-class RegisterSerializerEx(ModelNormal, IRegisterSerializerEx):
+class RegisterSerializerExRequest(ModelNormal, IRegisterSerializerExRequest):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       username (str):
 
+      password1 (str):
+
+      password2 (str):
+
       email (str): [optional]  # noqa: E501
 
       first_name (str): [optional]  # noqa: E501
 
       last_name (str): [optional]  # noqa: E501
 
 
@@ -113,14 +125,29 @@
     }
 
     validations = {
         ('username',): {
             'max_length': 150,
             'min_length': 5,
         },
+        ('password1',): {
+            'min_length': 1,
+        },
+        ('password2',): {
+            'min_length': 1,
+        },
+        ('email',): {
+            'min_length': 1,
+        },
+        ('first_name',): {
+            'min_length': 1,
+        },
+        ('last_name',): {
+            'min_length': 1,
+        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -137,44 +164,50 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'username': (str,),  # noqa: E501
+            'password1': (str,),  # noqa: E501
+            'password2': (str,),  # noqa: E501
             'email': (str,),  # noqa: E501
             'first_name': (str,),  # noqa: E501
             'last_name': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
 
     attribute_map = {
         'username': 'username',  # noqa: E501
+        'password1': 'password1',  # noqa: E501
+        'password2': 'password2',  # noqa: E501
         'email': 'email',  # noqa: E501
         'first_name': 'first_name',  # noqa: E501
         'last_name': 'last_name',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, username, *args, **kwargs):  # noqa: E501
-        """RegisterSerializerEx - a model defined in OpenAPI
+    def _from_openapi_data(cls, username, password1, password2, *args, **kwargs):  # noqa: E501
+        """RegisterSerializerExRequest - a model defined in OpenAPI
 
         Args:
             username (str):
+            password1 (str):
+            password2 (str):
 
         Keyword Args:
             email (str): [optional]  # noqa: E501
 
             first_name (str): [optional]  # noqa: E501
 
             last_name (str): [optional]  # noqa: E501
@@ -238,14 +271,16 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.username = username
+        self.password1 = password1
+        self.password2 = password2
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -258,19 +293,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, username, *args, **kwargs):  # noqa: E501
-        """RegisterSerializerEx - a model defined in OpenAPI
+    def __init__(self, username, password1, password2, *args, **kwargs):  # noqa: E501
+        """RegisterSerializerExRequest - a model defined in OpenAPI
 
         Args:
             username (str):
+            password1 (str):
+            password2 (str):
 
         Keyword Args:
             email (str): [optional]  # noqa: E501
 
             first_name (str): [optional]  # noqa: E501
 
             last_name (str): [optional]  # noqa: E501
@@ -332,14 +369,16 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.username = username
+        self.password1 = password1
+        self.password2 = password2
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/register_serializer_ex_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/storage.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -39,72 +39,58 @@
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
+def lazy_import():
+    from cvat_sdk.api_client.model.location_enum import LocationEnum
+    globals()['LocationEnum'] = LocationEnum
 
 
-class IRegisterSerializerExRequest(IModelData):
+
+class IStorage(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     # member type declarations
-    username: str # noqa: E501
-    """
-    """
-
-    email: str # noqa: E501
+    id: int # noqa: E501
     """
     [optional]
     """
 
-    password1: str # noqa: E501
-    """
-    """
-
-    password2: str # noqa: E501
-    """
-    """
-
-    first_name: str # noqa: E501
+    location: LocationEnum # noqa: E501
     """
     [optional]
     """
 
-    last_name: str # noqa: E501
+    cloud_storage_id: typing.Union[int, none_type] # noqa: E501
     """
     [optional]
     """
 
 
-class RegisterSerializerExRequest(ModelNormal, IRegisterSerializerExRequest):
+class Storage(ModelNormal, IStorage):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
-      username (str):
+      id (int): [optional]  # noqa: E501
 
-      password1 (str):
+      location (LocationEnum): [optional]  # noqa: E501
 
-      password2 (str):
-
-      email (str): [optional]  # noqa: E501
-
-      first_name (str): [optional]  # noqa: E501
-
-      last_name (str): [optional]  # noqa: E501
+      cloud_storage_id (int, none_type): [optional]  # noqa: E501
 
 
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
       attribute_map (dict): The key is attribute name
@@ -121,100 +107,77 @@
 
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('username',): {
-            'max_length': 150,
-            'min_length': 5,
-        },
-        ('password1',): {
-            'min_length': 1,
-        },
-        ('password2',): {
-            'min_length': 1,
-        },
-        ('email',): {
-            'min_length': 1,
-        },
-        ('first_name',): {
-            'min_length': 1,
-        },
-        ('last_name',): {
-            'min_length': 1,
+        ('cloud_storage_id',): {
+            'inclusive_maximum': 2147483647,
+            'inclusive_minimum': -2147483648,
         },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'username': (str,),  # noqa: E501
-            'password1': (str,),  # noqa: E501
-            'password2': (str,),  # noqa: E501
-            'email': (str,),  # noqa: E501
-            'first_name': (str,),  # noqa: E501
-            'last_name': (str,),  # noqa: E501
+            'id': (int,),  # noqa: E501
+            'location': (LocationEnum,),  # noqa: E501
+            'cloud_storage_id': (int, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
 
     attribute_map = {
-        'username': 'username',  # noqa: E501
-        'password1': 'password1',  # noqa: E501
-        'password2': 'password2',  # noqa: E501
-        'email': 'email',  # noqa: E501
-        'first_name': 'first_name',  # noqa: E501
-        'last_name': 'last_name',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'location': 'location',  # noqa: E501
+        'cloud_storage_id': 'cloud_storage_id',  # noqa: E501
     }
 
     read_only_vars = {
+        'id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, username, password1, password2, *args, **kwargs):  # noqa: E501
-        """RegisterSerializerExRequest - a model defined in OpenAPI
-
-        Args:
-            username (str):
-            password1 (str):
-            password2 (str):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """Storage - a model defined in OpenAPI
 
         Keyword Args:
-            email (str): [optional]  # noqa: E501
+            id (int): [optional]  # noqa: E501
 
-            first_name (str): [optional]  # noqa: E501
+            location (LocationEnum): [optional]  # noqa: E501
 
-            last_name (str): [optional]  # noqa: E501
+            cloud_storage_id (int, none_type): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -270,17 +233,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.username = username
-        self.password1 = password1
-        self.password2 = password2
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -293,28 +253,23 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, username, password1, password2, *args, **kwargs):  # noqa: E501
-        """RegisterSerializerExRequest - a model defined in OpenAPI
-
-        Args:
-            username (str):
-            password1 (str):
-            password2 (str):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """Storage - a model defined in OpenAPI
 
         Keyword Args:
-            email (str): [optional]  # noqa: E501
+            id (int): [optional]  # noqa: E501
 
-            first_name (str): [optional]  # noqa: E501
+            location (LocationEnum): [optional]  # noqa: E501
 
-            last_name (str): [optional]  # noqa: E501
+            cloud_storage_id (int, none_type): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -368,17 +323,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.username = username
-        self.password1 = password1
-        self.password2 = password2
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/rest_auth_detail.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/rest_auth_detail.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/role_enum.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/role_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/rq_id.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/rq_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/rq_status.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/rq_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/rq_status_state_enum.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/rq_status_state_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/severity_enum.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/severity_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/shape_type.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/shape_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/signing_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/signing_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/sorting_method.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/sorting_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/storage.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/storage_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -45,49 +45,42 @@
 
 def lazy_import():
     from cvat_sdk.api_client.model.location_enum import LocationEnum
     globals()['LocationEnum'] = LocationEnum
 
 
 
-class IStorage(IModelData):
+class IStorageRequest(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     # member type declarations
-    id: int # noqa: E501
-    """
-    [optional]
-    """
-
     location: LocationEnum # noqa: E501
     """
     [optional]
     """
 
     cloud_storage_id: typing.Union[int, none_type] # noqa: E501
     """
     [optional]
     """
 
 
-class Storage(ModelNormal, IStorage):
+class StorageRequest(ModelNormal, IStorageRequest):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
-      id (int): [optional]  # noqa: E501
-
       location (LocationEnum): [optional]  # noqa: E501
 
       cloud_storage_id (int, none_type): [optional]  # noqa: E501
 
 
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
@@ -136,45 +129,40 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'id': (int,),  # noqa: E501
             'location': (LocationEnum,),  # noqa: E501
             'cloud_storage_id': (int, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
         'location': 'location',  # noqa: E501
         'cloud_storage_id': 'cloud_storage_id',  # noqa: E501
     }
 
     read_only_vars = {
-        'id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Storage - a model defined in OpenAPI
+        """StorageRequest - a model defined in OpenAPI
 
         Keyword Args:
-            id (int): [optional]  # noqa: E501
-
             location (LocationEnum): [optional]  # noqa: E501
 
             cloud_storage_id (int, none_type): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
@@ -254,19 +242,17 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """Storage - a model defined in OpenAPI
+        """StorageRequest - a model defined in OpenAPI
 
         Keyword Args:
-            id (int): [optional]  # noqa: E501
-
             location (LocationEnum): [optional]  # noqa: E501
 
             cloud_storage_id (int, none_type): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/storage_method.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/storage_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/storage_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/tasks_summary.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -39,51 +39,47 @@
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
-def lazy_import():
-    from cvat_sdk.api_client.model.location_enum import LocationEnum
-    globals()['LocationEnum'] = LocationEnum
 
 
-
-class IStorageRequest(IModelData):
+class ITasksSummary(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     # member type declarations
-    location: LocationEnum # noqa: E501
+    count: int # noqa: E501
     """
-    [optional]
+    [optional, default: 0]
     """
 
-    cloud_storage_id: typing.Union[int, none_type] # noqa: E501
+    url: str # noqa: E501
     """
     [optional]
     """
 
 
-class StorageRequest(ModelNormal, IStorageRequest):
+class TasksSummary(ModelNormal, ITasksSummary):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
-      location (LocationEnum): [optional]  # noqa: E501
+      count (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
 
-      cloud_storage_id (int, none_type): [optional]  # noqa: E501
+      url (str): [optional]  # noqa: E501
 
 
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
       attribute_map (dict): The key is attribute name
@@ -100,72 +96,67 @@
 
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('cloud_storage_id',): {
-            'inclusive_maximum': 2147483647,
-            'inclusive_minimum': -2147483648,
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'location': (LocationEnum,),  # noqa: E501
-            'cloud_storage_id': (int, none_type,),  # noqa: E501
+            'count': (int,),  # noqa: E501
+            'url': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
 
     attribute_map = {
-        'location': 'location',  # noqa: E501
-        'cloud_storage_id': 'cloud_storage_id',  # noqa: E501
+        'count': 'count',  # noqa: E501
+        'url': 'url',  # noqa: E501
     }
 
     read_only_vars = {
+        'url',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """StorageRequest - a model defined in OpenAPI
+        """TasksSummary - a model defined in OpenAPI
 
         Keyword Args:
-            location (LocationEnum): [optional]  # noqa: E501
+            count (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
 
-            cloud_storage_id (int, none_type): [optional]  # noqa: E501
+            url (str): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -242,20 +233,20 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """StorageRequest - a model defined in OpenAPI
+        """TasksSummary - a model defined in OpenAPI
 
         Keyword Args:
-            location (LocationEnum): [optional]  # noqa: E501
+            count (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
 
-            cloud_storage_id (int, none_type): [optional]  # noqa: E501
+            url (str): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/storage_type.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/storage_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/sub_labeled_shape.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/sub_labeled_shape.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/sub_labeled_shape_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/sub_labeled_shape_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/sub_labeled_track.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/sub_labeled_track.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/sub_labeled_track_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/sub_labeled_track_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/sublabel.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/sublabel.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/sublabel_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/sublabel_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/task_annotations_update_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/task_annotations_update_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/task_annotations_write_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/task_annotations_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/task_file_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/task_file_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/task_read.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/task_read.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -40,24 +40,22 @@
 if TYPE_CHECKING:
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 def lazy_import():
-    from cvat_sdk.api_client.model.basic_user import BasicUser
     from cvat_sdk.api_client.model.chunk_type import ChunkType
-    from cvat_sdk.api_client.model.comment_read_owner import CommentReadOwner
+    from cvat_sdk.api_client.model.cloud_storage_read_owner import CloudStorageReadOwner
     from cvat_sdk.api_client.model.job_status import JobStatus
     from cvat_sdk.api_client.model.jobs_summary import JobsSummary
     from cvat_sdk.api_client.model.labels_summary import LabelsSummary
     from cvat_sdk.api_client.model.task_read_target_storage import TaskReadTargetStorage
-    globals()['BasicUser'] = BasicUser
     globals()['ChunkType'] = ChunkType
-    globals()['CommentReadOwner'] = CommentReadOwner
+    globals()['CloudStorageReadOwner'] = CloudStorageReadOwner
     globals()['JobStatus'] = JobStatus
     globals()['JobsSummary'] = JobsSummary
     globals()['LabelsSummary'] = LabelsSummary
     globals()['TaskReadTargetStorage'] = TaskReadTargetStorage
 
 
 
@@ -91,20 +89,20 @@
     """
 
     mode: str # noqa: E501
     """
     [optional]
     """
 
-    owner: BasicUser # noqa: E501
+    owner: CloudStorageReadOwner # noqa: E501
     """
     [optional]
     """
 
-    assignee: CommentReadOwner # noqa: E501
+    assignee: CloudStorageReadOwner # noqa: E501
     """
     [optional]
     """
 
     bug_tracker: str # noqa: E501
     """
     [optional]
@@ -141,14 +139,19 @@
     """
 
     data_compressed_chunk_type: typing.Union[typing.Any, none_type] # noqa: E501
     """
     [optional]
     """
 
+    guide_id: typing.Union[int, none_type] # noqa: E501
+    """
+    [optional]
+    """
+
     data_original_chunk_type: typing.Union[typing.Any, none_type] # noqa: E501
     """
     [optional]
     """
 
     size: int # noqa: E501
     """
@@ -217,17 +220,17 @@
 
       name (str): [optional]  # noqa: E501
 
       project_id (int, none_type): [optional]  # noqa: E501
 
       mode (str): [optional]  # noqa: E501
 
-      owner (BasicUser): [optional]  # noqa: E501
+      owner (CloudStorageReadOwner): [optional]  # noqa: E501
 
-      assignee (CommentReadOwner): [optional]  # noqa: E501
+      assignee (CloudStorageReadOwner): [optional]  # noqa: E501
 
       bug_tracker (str): [optional]  # noqa: E501
 
       created_date (datetime): [optional]  # noqa: E501
 
       updated_date (datetime): [optional]  # noqa: E501
 
@@ -237,14 +240,16 @@
 
       status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
       data_chunk_size (int, none_type): [optional]  # noqa: E501
 
       data_compressed_chunk_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
+      guide_id (int, none_type): [optional]  # noqa: E501
+
       data_original_chunk_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
       size (int): [optional]  # noqa: E501
 
       image_quality (int): [optional]  # noqa: E501
 
       data (int): [optional]  # noqa: E501
@@ -322,24 +327,25 @@
             'jobs': (JobsSummary,),  # noqa: E501
             'labels': (LabelsSummary,),  # noqa: E501
             'url': (str,),  # noqa: E501
             'id': (int,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'project_id': (int, none_type,),  # noqa: E501
             'mode': (str,),  # noqa: E501
-            'owner': (BasicUser,),  # noqa: E501
-            'assignee': (CommentReadOwner,),  # noqa: E501
+            'owner': (CloudStorageReadOwner,),  # noqa: E501
+            'assignee': (CloudStorageReadOwner,),  # noqa: E501
             'bug_tracker': (str,),  # noqa: E501
             'created_date': (datetime,),  # noqa: E501
             'updated_date': (datetime,),  # noqa: E501
             'overlap': (int, none_type,),  # noqa: E501
             'segment_size': (int,),  # noqa: E501
             'status': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'data_chunk_size': (int, none_type,),  # noqa: E501
             'data_compressed_chunk_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'guide_id': (int, none_type,),  # noqa: E501
             'data_original_chunk_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'size': (int,),  # noqa: E501
             'image_quality': (int,),  # noqa: E501
             'data': (int,),  # noqa: E501
             'dimension': (str,),  # noqa: E501
             'subset': (str,),  # noqa: E501
             'organization': (int, none_type,),  # noqa: E501
@@ -367,14 +373,15 @@
         'created_date': 'created_date',  # noqa: E501
         'updated_date': 'updated_date',  # noqa: E501
         'overlap': 'overlap',  # noqa: E501
         'segment_size': 'segment_size',  # noqa: E501
         'status': 'status',  # noqa: E501
         'data_chunk_size': 'data_chunk_size',  # noqa: E501
         'data_compressed_chunk_type': 'data_compressed_chunk_type',  # noqa: E501
+        'guide_id': 'guide_id',  # noqa: E501
         'data_original_chunk_type': 'data_original_chunk_type',  # noqa: E501
         'size': 'size',  # noqa: E501
         'image_quality': 'image_quality',  # noqa: E501
         'data': 'data',  # noqa: E501
         'dimension': 'dimension',  # noqa: E501
         'subset': 'subset',  # noqa: E501
         'organization': 'organization',  # noqa: E501
@@ -421,17 +428,17 @@
 
             name (str): [optional]  # noqa: E501
 
             project_id (int, none_type): [optional]  # noqa: E501
 
             mode (str): [optional]  # noqa: E501
 
-            owner (BasicUser): [optional]  # noqa: E501
+            owner (CloudStorageReadOwner): [optional]  # noqa: E501
 
-            assignee (CommentReadOwner): [optional]  # noqa: E501
+            assignee (CloudStorageReadOwner): [optional]  # noqa: E501
 
             bug_tracker (str): [optional]  # noqa: E501
 
             created_date (datetime): [optional]  # noqa: E501
 
             updated_date (datetime): [optional]  # noqa: E501
 
@@ -441,14 +448,16 @@
 
             status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
             data_chunk_size (int, none_type): [optional]  # noqa: E501
 
             data_compressed_chunk_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
+            guide_id (int, none_type): [optional]  # noqa: E501
+
             data_original_chunk_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
             size (int): [optional]  # noqa: E501
 
             image_quality (int): [optional]  # noqa: E501
 
             data (int): [optional]  # noqa: E501
@@ -561,17 +570,17 @@
 
             name (str): [optional]  # noqa: E501
 
             project_id (int, none_type): [optional]  # noqa: E501
 
             mode (str): [optional]  # noqa: E501
 
-            owner (BasicUser): [optional]  # noqa: E501
+            owner (CloudStorageReadOwner): [optional]  # noqa: E501
 
-            assignee (CommentReadOwner): [optional]  # noqa: E501
+            assignee (CloudStorageReadOwner): [optional]  # noqa: E501
 
             bug_tracker (str): [optional]  # noqa: E501
 
             created_date (datetime): [optional]  # noqa: E501
 
             updated_date (datetime): [optional]  # noqa: E501
 
@@ -581,14 +590,16 @@
 
             status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
             data_chunk_size (int, none_type): [optional]  # noqa: E501
 
             data_compressed_chunk_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
+            guide_id (int, none_type): [optional]  # noqa: E501
+
             data_original_chunk_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
             size (int): [optional]  # noqa: E501
 
             image_quality (int): [optional]  # noqa: E501
 
             data (int): [optional]  # noqa: E501
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/task_read_target_storage.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/task_read_target_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/task_write_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/task_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/tasks_summary.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_annotation_guide_write_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -41,45 +41,52 @@
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 
 
-class ITasksSummary(IModelData):
+class IPatchedAnnotationGuideWriteRequest(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     # member type declarations
-    count: int # noqa: E501
+    task_id: typing.Union[int, none_type] # noqa: E501
     """
-    [optional, default: 0]
+    [optional]
+    """
+
+    project_id: typing.Union[int, none_type] # noqa: E501
+    """
+    [optional]
     """
 
-    url: str # noqa: E501
+    markdown: str # noqa: E501
     """
     [optional]
     """
 
 
-class TasksSummary(ModelNormal, ITasksSummary):
+class PatchedAnnotationGuideWriteRequest(ModelNormal, IPatchedAnnotationGuideWriteRequest):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
-      count (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
+      task_id (int, none_type): [optional]  # noqa: E501
+
+      project_id (int, none_type): [optional]  # noqa: E501
 
-      url (str): [optional]  # noqa: E501
+      markdown (str): [optional]  # noqa: E501
 
 
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
       attribute_map (dict): The key is attribute name
@@ -119,44 +126,47 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'count': (int,),  # noqa: E501
-            'url': (str,),  # noqa: E501
+            'task_id': (int, none_type,),  # noqa: E501
+            'project_id': (int, none_type,),  # noqa: E501
+            'markdown': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
 
     attribute_map = {
-        'count': 'count',  # noqa: E501
-        'url': 'url',  # noqa: E501
+        'task_id': 'task_id',  # noqa: E501
+        'project_id': 'project_id',  # noqa: E501
+        'markdown': 'markdown',  # noqa: E501
     }
 
     read_only_vars = {
-        'url',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TasksSummary - a model defined in OpenAPI
+        """PatchedAnnotationGuideWriteRequest - a model defined in OpenAPI
 
         Keyword Args:
-            count (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
+            task_id (int, none_type): [optional]  # noqa: E501
 
-            url (str): [optional]  # noqa: E501
+            project_id (int, none_type): [optional]  # noqa: E501
+
+            markdown (str): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -233,20 +243,22 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TasksSummary - a model defined in OpenAPI
+        """PatchedAnnotationGuideWriteRequest - a model defined in OpenAPI
 
         Keyword Args:
-            count (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
+            task_id (int, none_type): [optional]  # noqa: E501
+
+            project_id (int, none_type): [optional]  # noqa: E501
 
-            url (str): [optional]  # noqa: E501
+            markdown (str): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/token.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/token.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/tracked_shape.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/tracked_shape.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/tracked_shape_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/tracked_shape_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/user.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/webhook_content_type.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/webhook_content_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/webhook_delivery_read.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/webhook_delivery_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/webhook_read.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/webhook_read.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -41,19 +41,19 @@
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 def lazy_import():
     from cvat_sdk.api_client.model.events_enum import EventsEnum
-    from cvat_sdk.api_client.model.project_read_owner import ProjectReadOwner
+    from cvat_sdk.api_client.model.job_read_assignee import JobReadAssignee
     from cvat_sdk.api_client.model.webhook_content_type import WebhookContentType
     from cvat_sdk.api_client.model.webhook_type import WebhookType
     globals()['EventsEnum'] = EventsEnum
-    globals()['ProjectReadOwner'] = ProjectReadOwner
+    globals()['JobReadAssignee'] = JobReadAssignee
     globals()['WebhookContentType'] = WebhookContentType
     globals()['WebhookType'] = WebhookType
 
 
 
 class IWebhookRead(IModelData):
     """
@@ -108,15 +108,15 @@
     """
 
     updated_date: datetime # noqa: E501
     """
     [optional]
     """
 
-    owner: ProjectReadOwner # noqa: E501
+    owner: JobReadAssignee # noqa: E501
     """
     [optional]
     """
 
     project_id: typing.Union[int, none_type] # noqa: E501
     """
     [optional]
@@ -168,15 +168,15 @@
 
       enable_ssl (bool): [optional]  # noqa: E501
 
       created_date (datetime): [optional]  # noqa: E501
 
       updated_date (datetime): [optional]  # noqa: E501
 
-      owner (ProjectReadOwner): [optional]  # noqa: E501
+      owner (JobReadAssignee): [optional]  # noqa: E501
 
       project_id (int, none_type): [optional]  # noqa: E501
 
       organization (int, none_type): [optional]  # noqa: E501
 
       events ([EventsEnum]): [optional]  # noqa: E501
 
@@ -238,15 +238,15 @@
             'url': (str,),  # noqa: E501
             'target_url': (str,),  # noqa: E501
             'description': (str,),  # noqa: E501
             'is_active': (bool,),  # noqa: E501
             'enable_ssl': (bool,),  # noqa: E501
             'created_date': (datetime,),  # noqa: E501
             'updated_date': (datetime,),  # noqa: E501
-            'owner': (ProjectReadOwner,),  # noqa: E501
+            'owner': (JobReadAssignee,),  # noqa: E501
             'project_id': (int, none_type,),  # noqa: E501
             'organization': (int, none_type,),  # noqa: E501
             'events': ([EventsEnum],),  # noqa: E501
             'last_status': (int,),  # noqa: E501
             'last_delivery_date': (datetime,),  # noqa: E501
         }
 
@@ -314,15 +314,15 @@
 
             enable_ssl (bool): [optional]  # noqa: E501
 
             created_date (datetime): [optional]  # noqa: E501
 
             updated_date (datetime): [optional]  # noqa: E501
 
-            owner (ProjectReadOwner): [optional]  # noqa: E501
+            owner (JobReadAssignee): [optional]  # noqa: E501
 
             project_id (int, none_type): [optional]  # noqa: E501
 
             organization (int, none_type): [optional]  # noqa: E501
 
             events ([EventsEnum]): [optional]  # noqa: E501
 
@@ -434,15 +434,15 @@
 
             enable_ssl (bool): [optional]  # noqa: E501
 
             created_date (datetime): [optional]  # noqa: E501
 
             updated_date (datetime): [optional]  # noqa: E501
 
-            owner (ProjectReadOwner): [optional]  # noqa: E501
+            owner (JobReadAssignee): [optional]  # noqa: E501
 
             project_id (int, none_type): [optional]  # noqa: E501
 
             organization (int, none_type): [optional]  # noqa: E501
 
             events ([EventsEnum]): [optional]  # noqa: E501
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/webhook_type.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/webhook_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model/webhook_write_request.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model/webhook_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/model_utils.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
 import inspect
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/models/__init__.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 # import all models into this package
 # if you have many models here with many references from one model to another this may
 # raise a RecursionError
@@ -20,33 +20,36 @@
 # import sys
 # sys.setrecursionlimit(n)
 
 from cvat_sdk.api_client.model.about import About, IAbout
 from cvat_sdk.api_client.model.annotation_conflict import AnnotationConflict, IAnnotationConflict
 from cvat_sdk.api_client.model.annotation_conflict_type_enum import AnnotationConflictTypeEnum, IAnnotationConflictTypeEnum
 from cvat_sdk.api_client.model.annotation_file_request import AnnotationFileRequest, IAnnotationFileRequest
+from cvat_sdk.api_client.model.annotation_guide_read import AnnotationGuideRead, IAnnotationGuideRead
+from cvat_sdk.api_client.model.annotation_guide_write_request import AnnotationGuideWriteRequest, IAnnotationGuideWriteRequest
 from cvat_sdk.api_client.model.annotation_id import AnnotationId, IAnnotationId
 from cvat_sdk.api_client.model.annotation_id_shape_type import AnnotationIdShapeType
 from cvat_sdk.api_client.model.annotation_id_type_enum import AnnotationIdTypeEnum, IAnnotationIdTypeEnum
 from cvat_sdk.api_client.model.annotations_read import AnnotationsRead
+from cvat_sdk.api_client.model.asset_read import AssetRead, IAssetRead
 from cvat_sdk.api_client.model.attribute import Attribute, IAttribute
 from cvat_sdk.api_client.model.attribute_request import AttributeRequest, IAttributeRequest
 from cvat_sdk.api_client.model.attribute_val import AttributeVal, IAttributeVal
 from cvat_sdk.api_client.model.attribute_val_request import AttributeValRequest, IAttributeValRequest
 from cvat_sdk.api_client.model.backup_write_request import BackupWriteRequest
 from cvat_sdk.api_client.model.basic_user import BasicUser, IBasicUser
 from cvat_sdk.api_client.model.basic_user_request import BasicUserRequest, IBasicUserRequest
 from cvat_sdk.api_client.model.chunk_type import ChunkType, IChunkType
 from cvat_sdk.api_client.model.client_events import ClientEvents, IClientEvents
 from cvat_sdk.api_client.model.client_events_request import ClientEventsRequest, IClientEventsRequest
 from cvat_sdk.api_client.model.cloud_storage_content import CloudStorageContent, ICloudStorageContent
 from cvat_sdk.api_client.model.cloud_storage_read import CloudStorageRead, ICloudStorageRead
+from cvat_sdk.api_client.model.cloud_storage_read_owner import CloudStorageReadOwner
 from cvat_sdk.api_client.model.cloud_storage_write_request import CloudStorageWriteRequest, ICloudStorageWriteRequest
 from cvat_sdk.api_client.model.comment_read import CommentRead, ICommentRead
-from cvat_sdk.api_client.model.comment_read_owner import CommentReadOwner
 from cvat_sdk.api_client.model.comment_write_request import CommentWriteRequest, ICommentWriteRequest
 from cvat_sdk.api_client.model.comments_summary import CommentsSummary, ICommentsSummary
 from cvat_sdk.api_client.model.credentials_type_enum import CredentialsTypeEnum, ICredentialsTypeEnum
 from cvat_sdk.api_client.model.data_meta_read import DataMetaRead, IDataMetaRead
 from cvat_sdk.api_client.model.data_request import DataRequest, IDataRequest
 from cvat_sdk.api_client.model.dataset_file_request import DatasetFileRequest, IDatasetFileRequest
 from cvat_sdk.api_client.model.dataset_format import DatasetFormat, IDatasetFormat
@@ -56,14 +59,17 @@
 from cvat_sdk.api_client.model.event_request import EventRequest, IEventRequest
 from cvat_sdk.api_client.model.events import Events, IEvents
 from cvat_sdk.api_client.model.events_enum import EventsEnum, IEventsEnum
 from cvat_sdk.api_client.model.file_info import FileInfo, IFileInfo
 from cvat_sdk.api_client.model.file_info_type_enum import FileInfoTypeEnum, IFileInfoTypeEnum
 from cvat_sdk.api_client.model.frame_meta import FrameMeta, IFrameMeta
 from cvat_sdk.api_client.model.frame_selection_method_enum import FrameSelectionMethodEnum, IFrameSelectionMethodEnum
+from cvat_sdk.api_client.model.function_call import FunctionCall, IFunctionCall
+from cvat_sdk.api_client.model.function_call_params import FunctionCallParams, IFunctionCallParams
+from cvat_sdk.api_client.model.function_call_request import FunctionCallRequest, IFunctionCallRequest
 from cvat_sdk.api_client.model.input_type_enum import InputTypeEnum, IInputTypeEnum
 from cvat_sdk.api_client.model.invitation_read import InvitationRead, IInvitationRead
 from cvat_sdk.api_client.model.invitation_write_request import InvitationWriteRequest, IInvitationWriteRequest
 from cvat_sdk.api_client.model.issue_read import IssueRead, IIssueRead
 from cvat_sdk.api_client.model.issue_write_request import IssueWriteRequest, IIssueWriteRequest
 from cvat_sdk.api_client.model.issues_summary import IssuesSummary, IIssuesSummary
 from cvat_sdk.api_client.model.job_annotations_update_request import JobAnnotationsUpdateRequest
@@ -108,14 +114,15 @@
 from cvat_sdk.api_client.model.paginated_quality_settings_list import PaginatedQualitySettingsList, IPaginatedQualitySettingsList
 from cvat_sdk.api_client.model.paginated_task_read_list import PaginatedTaskReadList, IPaginatedTaskReadList
 from cvat_sdk.api_client.model.paginated_webhook_delivery_read_list import PaginatedWebhookDeliveryReadList, IPaginatedWebhookDeliveryReadList
 from cvat_sdk.api_client.model.paginated_webhook_read_list import PaginatedWebhookReadList, IPaginatedWebhookReadList
 from cvat_sdk.api_client.model.password_change_request import PasswordChangeRequest, IPasswordChangeRequest
 from cvat_sdk.api_client.model.password_reset_confirm_request import PasswordResetConfirmRequest, IPasswordResetConfirmRequest
 from cvat_sdk.api_client.model.password_reset_serializer_ex_request import PasswordResetSerializerExRequest, IPasswordResetSerializerExRequest
+from cvat_sdk.api_client.model.patched_annotation_guide_write_request import PatchedAnnotationGuideWriteRequest, IPatchedAnnotationGuideWriteRequest
 from cvat_sdk.api_client.model.patched_cloud_storage_write_request import PatchedCloudStorageWriteRequest, IPatchedCloudStorageWriteRequest
 from cvat_sdk.api_client.model.patched_comment_write_request import PatchedCommentWriteRequest, IPatchedCommentWriteRequest
 from cvat_sdk.api_client.model.patched_data_meta_write_request import PatchedDataMetaWriteRequest, IPatchedDataMetaWriteRequest
 from cvat_sdk.api_client.model.patched_invitation_write_request import PatchedInvitationWriteRequest, IPatchedInvitationWriteRequest
 from cvat_sdk.api_client.model.patched_issue_write_request import PatchedIssueWriteRequest, IPatchedIssueWriteRequest
 from cvat_sdk.api_client.model.patched_job_write_request import PatchedJobWriteRequest, IPatchedJobWriteRequest
 from cvat_sdk.api_client.model.patched_label_request import PatchedLabelRequest, IPatchedLabelRequest
@@ -128,18 +135,18 @@
 from cvat_sdk.api_client.model.patched_task_write_request import PatchedTaskWriteRequest, IPatchedTaskWriteRequest
 from cvat_sdk.api_client.model.patched_task_write_request_target_storage import PatchedTaskWriteRequestTargetStorage
 from cvat_sdk.api_client.model.patched_user_request import PatchedUserRequest, IPatchedUserRequest
 from cvat_sdk.api_client.model.patched_webhook_write_request import PatchedWebhookWriteRequest, IPatchedWebhookWriteRequest
 from cvat_sdk.api_client.model.plugins import Plugins, IPlugins
 from cvat_sdk.api_client.model.project_file_request import ProjectFileRequest, IProjectFileRequest
 from cvat_sdk.api_client.model.project_read import ProjectRead, IProjectRead
-from cvat_sdk.api_client.model.project_read_owner import ProjectReadOwner
 from cvat_sdk.api_client.model.project_read_target_storage import ProjectReadTargetStorage
 from cvat_sdk.api_client.model.project_write_request import ProjectWriteRequest, IProjectWriteRequest
 from cvat_sdk.api_client.model.provider_type_enum import ProviderTypeEnum, IProviderTypeEnum
+from cvat_sdk.api_client.model.quality_enum import QualityEnum, IQualityEnum
 from cvat_sdk.api_client.model.quality_report import QualityReport, IQualityReport
 from cvat_sdk.api_client.model.quality_report_create_request import QualityReportCreateRequest, IQualityReportCreateRequest
 from cvat_sdk.api_client.model.quality_report_summary import QualityReportSummary, IQualityReportSummary
 from cvat_sdk.api_client.model.quality_report_target import QualityReportTarget, IQualityReportTarget
 from cvat_sdk.api_client.model.quality_settings import QualitySettings, IQualitySettings
 from cvat_sdk.api_client.model.register_serializer_ex import RegisterSerializerEx, IRegisterSerializerEx
 from cvat_sdk.api_client.model.register_serializer_ex_request import RegisterSerializerExRequest, IRegisterSerializerExRequest
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/api_client/rest.py` & `cvat_sdk-2.5.0/cvat_sdk/api_client/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 import io
 import json
 import logging
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/core/client.py` & `cvat_sdk-2.5.0/cvat_sdk/core/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,16 +58,16 @@
 class Client:
     """
     Provides session management, implements authentication operations
     and simplifies access to server APIs.
     """
 
     SUPPORTED_SERVER_VERSIONS = (
-        pv.Version("2.4"),
         pv.Version("2.5"),
+        pv.Version("2.6"),
     )
 
     def __init__(
         self,
         url: str,
         *,
         logger: Optional[logging.Logger] = None,
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/core/downloading.py` & `cvat_sdk-2.5.0/cvat_sdk/core/downloading.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.7/cvat_sdk/core/git.py` & `cvat_sdk-2.5.0/cvat_sdk/core/git.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.7/cvat_sdk/core/helpers.py` & `cvat_sdk-2.5.0/cvat_sdk/core/helpers.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.7/cvat_sdk/core/progress.py` & `cvat_sdk-2.5.0/cvat_sdk/core/progress.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.7/cvat_sdk/core/proxies/annotations.py` & `cvat_sdk-2.5.0/cvat_sdk/core/proxies/annotations.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.7/cvat_sdk/core/proxies/issues.py` & `cvat_sdk-2.5.0/cvat_sdk/core/proxies/issues.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.7/cvat_sdk/core/proxies/jobs.py` & `cvat_sdk-2.5.0/cvat_sdk/core/proxies/jobs.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.7/cvat_sdk/core/proxies/model_proxy.py` & `cvat_sdk-2.5.0/cvat_sdk/core/proxies/model_proxy.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.7/cvat_sdk/core/proxies/organizations.py` & `cvat_sdk-2.5.0/cvat_sdk/core/proxies/organizations.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.7/cvat_sdk/core/proxies/projects.py` & `cvat_sdk-2.5.0/cvat_sdk/core/proxies/projects.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.7/cvat_sdk/core/proxies/tasks.py` & `cvat_sdk-2.5.0/cvat_sdk/core/proxies/tasks.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.7/cvat_sdk/core/proxies/users.py` & `cvat_sdk-2.5.0/cvat_sdk/core/proxies/users.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.7/cvat_sdk/core/uploading.py` & `cvat_sdk-2.5.0/cvat_sdk/core/uploading.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.7/cvat_sdk/core/utils.py` & `cvat_sdk-2.5.0/cvat_sdk/core/utils.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.7/cvat_sdk/pytorch/caching.py` & `cvat_sdk-2.5.0/cvat_sdk/pytorch/caching.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         except Exception:
             self._logger.info(f"Task {task.id} is not yet cached or the cache is corrupted")
 
             # If the cache was corrupted, the directory might already be there; clear it.
             if task_dir.exists():
                 shutil.rmtree(task_dir)
         else:
-            if saved_task.updated_date < task.updated_date:
+            if saved_task.api_model.updated_date < task.updated_date:
                 self._logger.info(
                     f"Task {task.id} has been updated on the server since it was cached; purging the cache"
                 )
                 shutil.rmtree(task_dir)
 
         task_dir.mkdir(exist_ok=True, parents=True)
         self.save_model(task_json_path, _OfflineTaskModel.from_entity(task))
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk/pytorch/common.py` & `cvat_sdk-2.5.0/cvat_sdk/pytorch/common.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.7/cvat_sdk/pytorch/project_dataset.py` & `cvat_sdk-2.5.0/cvat_sdk/pytorch/project_dataset.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.7/cvat_sdk/pytorch/task_dataset.py` & `cvat_sdk-2.5.0/cvat_sdk/pytorch/task_dataset.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.7/cvat_sdk/pytorch/transforms.py` & `cvat_sdk-2.5.0/cvat_sdk/pytorch/transforms.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.7/cvat_sdk.egg-info/PKG-INFO` & `cvat_sdk-2.5.0/cvat_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvat-sdk
-Version: 2.4.7
+Version: 2.5.0
 Summary: CVAT REST API
 Home-page: https://github.com/cvat-ai/cvat
 Author: CVAT.ai team
 Author-email: support@cvat.ai
 License: MIT License
 Keywords: OpenAPI,OpenAPI-Generator,CVAT REST API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cvat_sdk-2.4.7/cvat_sdk.egg-info/SOURCES.txt` & `cvat_sdk-2.5.0/cvat_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,20 @@
 ./cvat_sdk/api_client/__init__.py
 ./cvat_sdk/api_client/api_client.py
 ./cvat_sdk/api_client/configuration.py
 ./cvat_sdk/api_client/exceptions.py
 ./cvat_sdk/api_client/model_utils.py
 ./cvat_sdk/api_client/rest.py
 ./cvat_sdk/api_client/api/__init__.py
+./cvat_sdk/api_client/api/assets_api.py
 ./cvat_sdk/api_client/api/auth_api.py
 ./cvat_sdk/api_client/api/cloudstorages_api.py
 ./cvat_sdk/api_client/api/comments_api.py
 ./cvat_sdk/api_client/api/events_api.py
+./cvat_sdk/api_client/api/guides_api.py
 ./cvat_sdk/api_client/api/invitations_api.py
 ./cvat_sdk/api_client/api/issues_api.py
 ./cvat_sdk/api_client/api/jobs_api.py
 ./cvat_sdk/api_client/api/labels_api.py
 ./cvat_sdk/api_client/api/lambda_api.py
 ./cvat_sdk/api_client/api/memberships_api.py
 ./cvat_sdk/api_client/api/organizations_api.py
@@ -33,33 +35,36 @@
 ./cvat_sdk/api_client/api/webhooks_api.py
 ./cvat_sdk/api_client/apis/__init__.py
 ./cvat_sdk/api_client/model/__init__.py
 ./cvat_sdk/api_client/model/about.py
 ./cvat_sdk/api_client/model/annotation_conflict.py
 ./cvat_sdk/api_client/model/annotation_conflict_type_enum.py
 ./cvat_sdk/api_client/model/annotation_file_request.py
+./cvat_sdk/api_client/model/annotation_guide_read.py
+./cvat_sdk/api_client/model/annotation_guide_write_request.py
 ./cvat_sdk/api_client/model/annotation_id.py
 ./cvat_sdk/api_client/model/annotation_id_shape_type.py
 ./cvat_sdk/api_client/model/annotation_id_type_enum.py
 ./cvat_sdk/api_client/model/annotations_read.py
+./cvat_sdk/api_client/model/asset_read.py
 ./cvat_sdk/api_client/model/attribute.py
 ./cvat_sdk/api_client/model/attribute_request.py
 ./cvat_sdk/api_client/model/attribute_val.py
 ./cvat_sdk/api_client/model/attribute_val_request.py
 ./cvat_sdk/api_client/model/backup_write_request.py
 ./cvat_sdk/api_client/model/basic_user.py
 ./cvat_sdk/api_client/model/basic_user_request.py
 ./cvat_sdk/api_client/model/chunk_type.py
 ./cvat_sdk/api_client/model/client_events.py
 ./cvat_sdk/api_client/model/client_events_request.py
 ./cvat_sdk/api_client/model/cloud_storage_content.py
 ./cvat_sdk/api_client/model/cloud_storage_read.py
+./cvat_sdk/api_client/model/cloud_storage_read_owner.py
 ./cvat_sdk/api_client/model/cloud_storage_write_request.py
 ./cvat_sdk/api_client/model/comment_read.py
-./cvat_sdk/api_client/model/comment_read_owner.py
 ./cvat_sdk/api_client/model/comment_write_request.py
 ./cvat_sdk/api_client/model/comments_summary.py
 ./cvat_sdk/api_client/model/credentials_type_enum.py
 ./cvat_sdk/api_client/model/data_meta_read.py
 ./cvat_sdk/api_client/model/data_request.py
 ./cvat_sdk/api_client/model/dataset_file_request.py
 ./cvat_sdk/api_client/model/dataset_format.py
@@ -69,14 +74,17 @@
 ./cvat_sdk/api_client/model/event_request.py
 ./cvat_sdk/api_client/model/events.py
 ./cvat_sdk/api_client/model/events_enum.py
 ./cvat_sdk/api_client/model/file_info.py
 ./cvat_sdk/api_client/model/file_info_type_enum.py
 ./cvat_sdk/api_client/model/frame_meta.py
 ./cvat_sdk/api_client/model/frame_selection_method_enum.py
+./cvat_sdk/api_client/model/function_call.py
+./cvat_sdk/api_client/model/function_call_params.py
+./cvat_sdk/api_client/model/function_call_request.py
 ./cvat_sdk/api_client/model/input_type_enum.py
 ./cvat_sdk/api_client/model/invitation_read.py
 ./cvat_sdk/api_client/model/invitation_write_request.py
 ./cvat_sdk/api_client/model/issue_read.py
 ./cvat_sdk/api_client/model/issue_write_request.py
 ./cvat_sdk/api_client/model/issues_summary.py
 ./cvat_sdk/api_client/model/job_annotations_update_request.py
@@ -121,14 +129,15 @@
 ./cvat_sdk/api_client/model/paginated_quality_settings_list.py
 ./cvat_sdk/api_client/model/paginated_task_read_list.py
 ./cvat_sdk/api_client/model/paginated_webhook_delivery_read_list.py
 ./cvat_sdk/api_client/model/paginated_webhook_read_list.py
 ./cvat_sdk/api_client/model/password_change_request.py
 ./cvat_sdk/api_client/model/password_reset_confirm_request.py
 ./cvat_sdk/api_client/model/password_reset_serializer_ex_request.py
+./cvat_sdk/api_client/model/patched_annotation_guide_write_request.py
 ./cvat_sdk/api_client/model/patched_cloud_storage_write_request.py
 ./cvat_sdk/api_client/model/patched_comment_write_request.py
 ./cvat_sdk/api_client/model/patched_data_meta_write_request.py
 ./cvat_sdk/api_client/model/patched_invitation_write_request.py
 ./cvat_sdk/api_client/model/patched_issue_write_request.py
 ./cvat_sdk/api_client/model/patched_job_write_request.py
 ./cvat_sdk/api_client/model/patched_label_request.py
@@ -141,18 +150,18 @@
 ./cvat_sdk/api_client/model/patched_task_write_request.py
 ./cvat_sdk/api_client/model/patched_task_write_request_target_storage.py
 ./cvat_sdk/api_client/model/patched_user_request.py
 ./cvat_sdk/api_client/model/patched_webhook_write_request.py
 ./cvat_sdk/api_client/model/plugins.py
 ./cvat_sdk/api_client/model/project_file_request.py
 ./cvat_sdk/api_client/model/project_read.py
-./cvat_sdk/api_client/model/project_read_owner.py
 ./cvat_sdk/api_client/model/project_read_target_storage.py
 ./cvat_sdk/api_client/model/project_write_request.py
 ./cvat_sdk/api_client/model/provider_type_enum.py
+./cvat_sdk/api_client/model/quality_enum.py
 ./cvat_sdk/api_client/model/quality_report.py
 ./cvat_sdk/api_client/model/quality_report_create_request.py
 ./cvat_sdk/api_client/model/quality_report_summary.py
 ./cvat_sdk/api_client/model/quality_report_target.py
 ./cvat_sdk/api_client/model/quality_settings.py
 ./cvat_sdk/api_client/model/register_serializer_ex.py
 ./cvat_sdk/api_client/model/register_serializer_ex_request.py
```

### Comparing `cvat_sdk-2.4.7/setup.py` & `cvat_sdk-2.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.7
+# The version of the OpenAPI document: 2.6
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 import os.path as osp
 import re
 from setuptools import find_packages, setup
```

