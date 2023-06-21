# Comparing `tmp/cvat_sdk-2.4.6.tar.gz` & `tmp/cvat_sdk-2.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvat_sdk-2.4.6.tar", last modified: Wed Jun 14 19:55:23 2023, max compression
+gzip compressed data, was "cvat_sdk-2.4.7.tar", last modified: Wed Jun 21 13:43:49 2023, max compression
```

## Comparing `cvat_sdk-2.4.6.tar` & `cvat_sdk-2.4.7.tar`

### file list

```diff
@@ -1,219 +1,239 @@
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:55:23.065931 cvat_sdk-2.4.6/
--rw-r--r--   0 andrey    (1000) andrey    (1000)       83 2023-04-05 10:02:25.000000 cvat_sdk-2.4.6/MANIFEST.in
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1463 2023-06-14 19:55:23.065931 cvat_sdk-2.4.6/PKG-INFO
--rw-r--r--   0 andrey    (1000) andrey    (1000)      989 2023-04-05 10:02:25.000000 cvat_sdk-2.4.6/README.md
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:55:23.015929 cvat_sdk-2.4.6/cvat_sdk/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      188 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/__init__.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:55:23.015929 cvat_sdk-2.4.6/cvat_sdk/api_client/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      767 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/__init__.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:55:23.015929 cvat_sdk-2.4.6/cvat_sdk/api_client/api/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      503 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    45482 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/auth_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    60873 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/cloudstorages_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    31388 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/comments_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15033 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/events_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    30703 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/invitations_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    31878 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/issues_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    79891 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/jobs_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    26740 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/labels_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    33105 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/lambda_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    24997 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/memberships_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    29848 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/organizations_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    75123 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/projects_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    10673 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/schema_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    21217 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/server_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)   131955 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/tasks_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    30201 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/users_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    66191 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api/webhooks_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    45222 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/api_client.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:55:23.015929 cvat_sdk-2.4.6/cvat_sdk/api_client/apis/
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1711 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/apis/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    19679 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/configuration.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     5132 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/exceptions.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:55:23.055930 cvat_sdk-2.4.6/cvat_sdk/api_client/model/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      353 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13042 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/about.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12460 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/annotation_file_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15640 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/annotations_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14199 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/attribute.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13995 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/attribute_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12612 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/attribute_val.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12647 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/attribute_val_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14272 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/backup_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14112 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/basic_user.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13574 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/basic_user_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13023 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/chunk_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12999 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/client_events.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13105 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/client_events_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13139 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/cloud_storage_content.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17365 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/cloud_storage_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18328 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/cloud_storage_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14263 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/comment_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15468 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/comment_read_owner.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12658 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/comment_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12743 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/comments_summary.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14282 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/credentials_type_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15330 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/data_meta_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    33482 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/data_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12406 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/dataset_file_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13648 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/dataset_format.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12999 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/dataset_formats.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14276 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/dataset_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18298 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/event.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18849 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/event_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12988 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/events.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18731 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/events_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13186 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/file_info.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12821 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/file_info_type_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13644 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/frame_meta.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13367 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/input_type_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14184 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/invitation_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12807 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/invitation_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15954 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/issue_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14034 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/issue_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12590 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/issues_summary.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16288 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/job_annotations_update_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    21389 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/job_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15464 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/job_read_assignee.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13213 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/job_stage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13203 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/job_status.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13215 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/jobs_summary.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17310 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/label.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14504 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/labeled_data.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14752 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/labeled_data_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14732 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/labeled_image.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14901 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/labeled_image_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18094 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/labeled_shape.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18334 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/labeled_shape_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15751 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/labeled_track.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16062 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/labeled_track_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12590 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/labels_summary.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12981 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/location_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13020 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/login_serializer_ex_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14975 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/membership_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17616 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/meta_user.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12583 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/online_function_call_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13335 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/operation_status.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15424 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/organization_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13862 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/organization_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13674 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_cloud_storage_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13598 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_comment_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13643 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_invitation_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13568 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_issue_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13538 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_job_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13507 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_label_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13643 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_membership_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13553 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_meta_user_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13673 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_organization_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13598 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_project_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13553 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_task_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13719 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_webhook_delivery_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13598 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_webhook_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13433 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/password_change_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13634 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/password_reset_confirm_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12417 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/password_reset_serializer_ex_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18255 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_cloud_storage_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12397 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_comment_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12418 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_data_meta_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12866 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_invitation_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13069 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_issue_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13342 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_job_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16560 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_label_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14787 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_labeled_data_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12514 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_membership_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13897 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_organization_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16059 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_project_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14845 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_project_write_request_target_storage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16209 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_task_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14832 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_task_write_request_target_storage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16216 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_user_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14962 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_webhook_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13269 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/plugins.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12406 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/project_file_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    19106 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/project_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15469 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/project_read_owner.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14944 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/project_read_target_storage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16024 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/project_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13747 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/provider_type_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13363 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/register_serializer_ex.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14361 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/register_serializer_ex_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12298 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/rest_auth_detail.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13300 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/role_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12215 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/rq_id.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13564 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/rq_status.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13285 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/rq_status_state_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13953 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/shape_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12299 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/signing_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13430 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/sorting_method.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13336 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/storage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12956 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/storage_method.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13074 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/storage_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13123 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/storage_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17568 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/sub_labeled_shape.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17737 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/sub_labeled_shape_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15225 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/sub_labeled_track.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15465 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/sub_labeled_track_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15279 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/sublabel.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15414 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/sublabel_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16291 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/task_annotations_update_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14338 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/task_annotations_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12352 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/task_file_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    23631 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/task_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14932 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/task_read_target_storage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17123 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/task_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12728 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/tasks_summary.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12255 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/token.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16249 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/tracked_shape.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16355 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/tracked_shape_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17571 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/user.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12666 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/webhook_content_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16432 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/webhook_delivery_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18535 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/webhook_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12991 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/webhook_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15742 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model/webhook_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    84566 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/model_utils.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:55:23.055930 cvat_sdk-2.4.6/cvat_sdk/api_client/models/
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13663 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/models/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14475 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/api_client/rest.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:55:23.055930 cvat_sdk-2.4.6/cvat_sdk/core/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      188 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12038 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/client.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     3115 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/downloading.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      353 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/exceptions.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1832 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/git.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     3061 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/helpers.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     3147 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/progress.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:55:23.055930 cvat_sdk-2.4.6/cvat_sdk/core/proxies/
--rw-r--r--   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/proxies/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     2116 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/proxies/annotations.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1737 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/proxies/issues.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     5550 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/proxies/jobs.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     5824 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/proxies/model_proxy.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      967 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/proxies/organizations.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     6652 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/proxies/projects.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14269 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/proxies/tasks.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      832 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/proxies/users.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14651 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/uploading.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     2103 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/core/utils.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      325 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/exceptions.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      167 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/models.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:55:23.065931 cvat_sdk-2.4.6/cvat_sdk/pytorch/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      362 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/pytorch/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    11405 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/pytorch/caching.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      969 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/pytorch/common.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     4303 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/pytorch/project_dataset.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     6982 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/pytorch/task_dataset.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     2885 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/pytorch/transforms.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)       18 2023-06-14 19:54:48.000000 cvat_sdk-2.4.6/cvat_sdk/version.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:55:23.065931 cvat_sdk-2.4.6/cvat_sdk.egg-info/
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1463 2023-06-14 19:55:22.000000 cvat_sdk-2.4.6/cvat_sdk.egg-info/PKG-INFO
--rw-r--r--   0 andrey    (1000) andrey    (1000)     9269 2023-06-14 19:55:23.000000 cvat_sdk-2.4.6/cvat_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)        1 2023-06-14 19:55:22.000000 cvat_sdk-2.4.6/cvat_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)      202 2023-06-14 19:55:22.000000 cvat_sdk-2.4.6/cvat_sdk.egg-info/requires.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)        9 2023-06-14 19:55:22.000000 cvat_sdk-2.4.6/cvat_sdk.egg-info/top_level.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)      383 2022-12-22 11:37:46.000000 cvat_sdk-2.4.6/pyproject.toml
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-14 19:55:23.065931 cvat_sdk-2.4.6/requirements/
--rw-r--r--   0 andrey    (1000) andrey    (1000)       64 2023-06-14 19:54:47.000000 cvat_sdk-2.4.6/requirements/api_client.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)      206 2023-04-05 10:02:25.000000 cvat_sdk-2.4.6/requirements/base.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)       38 2023-06-14 19:55:23.065931 cvat_sdk-2.4.6/setup.cfg
--rw-r--r--   0 andrey    (1000) andrey    (1000)     2753 2023-06-14 19:54:47.000000 cvat_sdk-2.4.6/setup.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:43:49.880040 cvat_sdk-2.4.7/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       83 2023-04-05 10:02:25.000000 cvat_sdk-2.4.7/MANIFEST.in
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1463 2023-06-21 13:43:49.880040 cvat_sdk-2.4.7/PKG-INFO
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      989 2023-04-05 10:02:25.000000 cvat_sdk-2.4.7/README.md
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:43:49.850040 cvat_sdk-2.4.7/cvat_sdk/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      188 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/__init__.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:43:49.850040 cvat_sdk-2.4.7/cvat_sdk/api_client/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      767 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/__init__.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:43:49.860040 cvat_sdk-2.4.7/cvat_sdk/api_client/api/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      503 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    45482 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/auth_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    60873 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/cloudstorages_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    31388 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/comments_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15033 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/events_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    30703 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/invitations_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    31878 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/issues_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    92134 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/jobs_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    26740 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/labels_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    33105 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/lambda_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    24997 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/memberships_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    29848 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/organizations_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    75123 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/projects_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    53046 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/quality_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    10673 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/schema_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    21217 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/server_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)   131655 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/tasks_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    30201 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/users_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    65408 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api/webhooks_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    45325 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/api_client.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:43:49.860040 cvat_sdk-2.4.7/cvat_sdk/api_client/apis/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1770 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/apis/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    19679 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/configuration.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     5132 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/exceptions.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:43:49.880040 cvat_sdk-2.4.7/cvat_sdk/api_client/model/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      353 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13042 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/about.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15100 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/annotation_conflict.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15328 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/annotation_conflict_type_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12460 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/annotation_file_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13969 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/annotation_id.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14124 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/annotation_id_shape_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13018 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/annotation_id_type_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15640 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/annotations_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14199 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/attribute.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13995 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/attribute_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12612 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/attribute_val.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12647 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/attribute_val_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14272 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/backup_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14112 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/basic_user.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13574 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/basic_user_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13023 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/chunk_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12999 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/client_events.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13105 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/client_events_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13139 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/cloud_storage_content.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17365 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/cloud_storage_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18328 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/cloud_storage_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14263 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/comment_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15468 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/comment_read_owner.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12658 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/comment_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12743 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/comments_summary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14282 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/credentials_type_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16405 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/data_meta_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    33482 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/data_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12406 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/dataset_file_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13648 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/dataset_format.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12999 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/dataset_formats.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14276 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/dataset_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18298 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/event.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18849 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/event_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12988 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/events.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18731 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/events_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13186 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/file_info.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12821 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/file_info_type_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13644 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/frame_meta.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13071 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/frame_selection_method_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13367 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/input_type_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14184 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/invitation_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12807 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/invitation_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15954 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/issue_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14034 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/issue_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12590 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/issues_summary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16288 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/job_annotations_update_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    22827 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/job_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15464 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/job_read_assignee.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13213 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/job_stage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13203 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/job_status.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13016 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/job_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17144 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/job_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13215 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/jobs_summary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17310 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/label.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14504 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/labeled_data.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14752 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/labeled_data_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14732 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/labeled_image.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14901 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/labeled_image_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18094 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/labeled_shape.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18334 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/labeled_shape_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15751 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/labeled_track.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16062 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/labeled_track_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12590 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/labels_summary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12981 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/location_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13020 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/login_serializer_ex_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14975 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/membership_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17616 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/meta_user.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12611 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/null_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12583 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/online_function_call_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13335 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/operation_status.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15424 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/organization_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13862 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/organization_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13703 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_annotation_conflict_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13674 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_cloud_storage_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13598 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_comment_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13643 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_invitation_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13568 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_issue_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13538 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_job_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13507 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_label_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13643 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_membership_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13553 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_meta_user_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13673 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_organization_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13598 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_project_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13628 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_quality_report_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13658 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_quality_settings_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13553 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_task_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13719 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_webhook_delivery_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13598 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_webhook_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13433 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/password_change_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13634 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/password_reset_confirm_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12417 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/password_reset_serializer_ex_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18255 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_cloud_storage_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12397 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_comment_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12418 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_data_meta_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12866 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_invitation_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13069 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_issue_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13342 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_job_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16560 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_label_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14787 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_labeled_data_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12514 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_membership_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13897 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_organization_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16059 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_project_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14845 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_project_write_request_target_storage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    21880 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_quality_settings_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16209 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_task_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14832 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_task_write_request_target_storage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16216 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_user_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14962 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_webhook_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13269 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/plugins.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12406 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/project_file_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    19106 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/project_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15469 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/project_read_owner.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14944 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/project_read_target_storage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16024 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/project_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13747 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/provider_type_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15893 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/quality_report.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12351 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/quality_report_create_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15291 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/quality_report_summary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12851 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/quality_report_target.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    22444 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/quality_settings.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13363 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/register_serializer_ex.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14361 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/register_serializer_ex_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12298 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/rest_auth_detail.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13300 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/role_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12264 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/rq_id.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13564 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/rq_status.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13285 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/rq_status_state_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12891 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/severity_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13953 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/shape_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12299 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/signing_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13430 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/sorting_method.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13336 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/storage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12956 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/storage_method.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13074 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/storage_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13123 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/storage_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17568 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/sub_labeled_shape.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17737 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/sub_labeled_shape_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15225 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/sub_labeled_track.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15465 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/sub_labeled_track_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15279 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/sublabel.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15414 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/sublabel_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16291 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/task_annotations_update_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14338 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/task_annotations_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12352 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/task_file_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    23631 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/task_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14932 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/task_read_target_storage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17123 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/task_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12728 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/tasks_summary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12255 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/token.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16249 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/tracked_shape.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16355 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/tracked_shape_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17571 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/user.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12666 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/webhook_content_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16432 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/webhook_delivery_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18535 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/webhook_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12991 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/webhook_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15742 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model/webhook_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    84566 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/model_utils.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:43:49.880040 cvat_sdk-2.4.7/cvat_sdk/api_client/models/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15606 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/models/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14475 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/api_client/rest.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:43:49.880040 cvat_sdk-2.4.7/cvat_sdk/core/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      188 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12038 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/client.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     3115 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/downloading.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      353 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/exceptions.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1832 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/git.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     3061 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/helpers.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     3147 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/progress.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:43:49.880040 cvat_sdk-2.4.7/cvat_sdk/core/proxies/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/proxies/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2116 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/proxies/annotations.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1737 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/proxies/issues.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     5550 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/proxies/jobs.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     5824 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/proxies/model_proxy.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      967 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/proxies/organizations.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     6652 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/proxies/projects.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14269 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/proxies/tasks.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      832 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/proxies/users.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14651 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/uploading.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2103 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/core/utils.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      325 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/exceptions.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      167 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/models.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:43:49.880040 cvat_sdk-2.4.7/cvat_sdk/pytorch/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      362 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/pytorch/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    11405 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/pytorch/caching.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      969 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/pytorch/common.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     4303 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/pytorch/project_dataset.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     6982 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/pytorch/task_dataset.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2885 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/pytorch/transforms.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       18 2023-06-21 13:43:06.000000 cvat_sdk-2.4.7/cvat_sdk/version.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:43:49.880040 cvat_sdk-2.4.7/cvat_sdk.egg-info/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1463 2023-06-21 13:43:49.000000 cvat_sdk-2.4.7/cvat_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    10328 2023-06-21 13:43:49.000000 cvat_sdk-2.4.7/cvat_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        1 2023-06-21 13:43:49.000000 cvat_sdk-2.4.7/cvat_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      202 2023-06-21 13:43:49.000000 cvat_sdk-2.4.7/cvat_sdk.egg-info/requires.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        9 2023-06-21 13:43:49.000000 cvat_sdk-2.4.7/cvat_sdk.egg-info/top_level.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      383 2022-12-22 11:37:46.000000 cvat_sdk-2.4.7/pyproject.toml
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-06-21 13:43:49.880040 cvat_sdk-2.4.7/requirements/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       64 2023-06-21 13:43:05.000000 cvat_sdk-2.4.7/requirements/api_client.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      206 2023-04-05 10:02:25.000000 cvat_sdk-2.4.7/requirements/base.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       38 2023-06-21 13:43:49.880040 cvat_sdk-2.4.7/setup.cfg
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2753 2023-06-21 13:43:05.000000 cvat_sdk-2.4.7/setup.py
```

### Comparing `cvat_sdk-2.4.6/PKG-INFO` & `cvat_sdk-2.4.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvat_sdk
-Version: 2.4.6
+Version: 2.4.7
 Summary: CVAT REST API
 Home-page: https://github.com/cvat-ai/cvat
 Author: CVAT.ai team
 Author-email: support@cvat.ai
 License: MIT License
 Keywords: OpenAPI,OpenAPI-Generator,CVAT REST API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cvat_sdk-2.4.6/README.md` & `cvat_sdk-2.4.7/README.md`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/__init__.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
-__version__ = "2.4.6"
+__version__ = "2.4.7"
 
 from cvat_sdk.api_client.api_client import ApiClient
 
 from cvat_sdk.api_client.configuration import Configuration
 
 from cvat_sdk.api_client.exceptions import OpenApiException
 from cvat_sdk.api_client.exceptions import ApiAttributeError
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/api/auth_api.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/api/auth_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/api/cloudstorages_api.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/api/cloudstorages_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/api/comments_api.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/api/comments_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/api/events_api.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/api/events_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/api/invitations_api.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/api/invitations_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/api/issues_api.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/api/issues_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/api/jobs_api.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/api/jobs_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -26,14 +26,15 @@
     none_type,
 )
 from cvat_sdk.api_client.model.annotation_file_request import AnnotationFileRequest
 from cvat_sdk.api_client.model.annotations_read import AnnotationsRead
 from cvat_sdk.api_client.model.data_meta_read import DataMetaRead
 from cvat_sdk.api_client.model.job_annotations_update_request import JobAnnotationsUpdateRequest
 from cvat_sdk.api_client.model.job_read import JobRead
+from cvat_sdk.api_client.model.job_write_request import JobWriteRequest
 from cvat_sdk.api_client.model.paginated_job_read_list import PaginatedJobReadList
 from cvat_sdk.api_client.model.patched_job_write_request import PatchedJobWriteRequest
 from cvat_sdk.api_client.model.patched_labeled_data_request import PatchedLabeledDataRequest
 from cvat_sdk.api_client.model.rq_id import RqId
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
@@ -49,14 +50,70 @@
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
+        self.create_endpoint = _Endpoint(
+            settings={
+                'response_schema': (JobRead,),
+                'auth': [
+                    'basicAuth',
+                    'csrfAuth',
+                    'sessionAuth',
+                    'signatureAuth',
+                    'tokenAuth'
+                ],
+                'endpoint_path': '/api/jobs',
+                'operation_id': 'create',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'job_write_request',
+                ],
+                'required': [
+                    'job_write_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'job_write_request':
+                        (JobWriteRequest,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'job_write_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/vnd.cvat+json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.create_annotations_endpoint = _Endpoint(
             settings={
                 'response_schema': None,
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
@@ -67,24 +124,23 @@
                 'operation_id': 'create_annotations',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'annotation_file_request',
                     'cloud_storage_id',
                     'filename',
                     'format',
                     'location',
                     'use_default_location',
+                    'annotation_file_request',
                 ],
                 'required': [
                     'id',
-                    'annotation_file_request',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                     'location',
                 ],
                 'validation': [
@@ -99,43 +155,43 @@
                         "CLOUD_STORAGE": "cloud_storage",
                         "LOCAL": "local"
                     },
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'annotation_file_request':
-                        (AnnotationFileRequest,),
                     'cloud_storage_id':
                         (float,),
                     'filename':
                         (str,),
                     'format':
                         (str,),
                     'location':
                         (str,),
                     'use_default_location':
                         (bool,),
+                    'annotation_file_request':
+                        (AnnotationFileRequest,),
                 },
                 'attribute_map': {
                     'id': 'id',
                     'cloud_storage_id': 'cloud_storage_id',
                     'filename': 'filename',
                     'format': 'format',
                     'location': 'location',
                     'use_default_location': 'use_default_location',
                 },
                 'location_map': {
                     'id': 'path',
-                    'annotation_file_request': 'body',
                     'cloud_storage_id': 'query',
                     'filename': 'query',
                     'format': 'query',
                     'location': 'query',
                     'use_default_location': 'query',
+                    'annotation_file_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
@@ -143,14 +199,67 @@
                 'content_type': [
                     'application/json',
                     'multipart/form-data'
                 ]
             },
             api_client=api_client
         )
+        self.destroy_endpoint = _Endpoint(
+            settings={
+                'response_schema': None,
+                'auth': [
+                    'basicAuth',
+                    'csrfAuth',
+                    'sessionAuth',
+                    'signatureAuth',
+                    'tokenAuth'
+                ],
+                'endpoint_path': '/api/jobs/{id}',
+                'operation_id': 'destroy',
+                'http_method': 'DELETE',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'id',
+                ],
+                'required': [
+                    'id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'id':
+                        (int,),
+                },
+                'attribute_map': {
+                    'id': 'id',
+                },
+                'location_map': {
+                    'id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
         self.destroy_annotations_endpoint = _Endpoint(
             settings={
                 'response_schema': None,
                 'auth': [
                     'basicAuth',
                     'csrfAuth',
                     'sessionAuth',
@@ -229,22 +338,24 @@
                     'project_name',
                     'search',
                     'sort',
                     'stage',
                     'state',
                     'task_id',
                     'task_name',
+                    'type',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
                     'dimension',
                     'stage',
                     'state',
+                    'type',
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
@@ -263,14 +374,19 @@
                     ('state',): {
 
                         "NEW": "new",
                         "IN_PROGRESS": "in progress",
                         "COMPLETED": "completed",
                         "REJECTED": "rejected"
                     },
+                    ('type',): {
+
+                        "ANNOTATION": "annotation",
+                        "GROUND_TRUTH": "ground_truth"
+                    },
                 },
                 'openapi_types': {
                     'x_organization':
                         (str,),
                     'assignee':
                         (str,),
                     'dimension':
@@ -297,14 +413,16 @@
                         (str,),
                     'state':
                         (str,),
                     'task_id':
                         (int,),
                     'task_name':
                         (str,),
+                    'type':
+                        (str,),
                 },
                 'attribute_map': {
                     'x_organization': 'X-Organization',
                     'assignee': 'assignee',
                     'dimension': 'dimension',
                     'filter': 'filter',
                     'org': 'org',
@@ -315,14 +433,15 @@
                     'project_name': 'project_name',
                     'search': 'search',
                     'sort': 'sort',
                     'stage': 'stage',
                     'state': 'state',
                     'task_id': 'task_id',
                     'task_name': 'task_name',
+                    'type': 'type',
                 },
                 'location_map': {
                     'x_organization': 'header',
                     'assignee': 'query',
                     'dimension': 'query',
                     'filter': 'query',
                     'org': 'query',
@@ -333,14 +452,15 @@
                     'project_name': 'query',
                     'search': 'query',
                     'sort': 'query',
                     'stage': 'query',
                     'state': 'query',
                     'task_id': 'query',
                     'task_name': 'query',
+                    'type': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
@@ -936,52 +1056,78 @@
                 'operation_id': 'update_annotations',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
+                    'cloud_storage_id',
+                    'filename',
                     'format',
+                    'location',
                     'rq_id',
+                    'use_default_location',
                     'job_annotations_update_request',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
+                    'location',
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
+                    ('location',): {
+
+                        "CLOUD_STORAGE": "cloud_storage",
+                        "LOCAL": "local"
+                    },
                 },
                 'openapi_types': {
                     'id':
                         (int,),
+                    'cloud_storage_id':
+                        (float,),
+                    'filename':
+                        (str,),
                     'format':
                         (str,),
+                    'location':
+                        (str,),
                     'rq_id':
                         (str,),
+                    'use_default_location':
+                        (bool,),
                     'job_annotations_update_request':
                         (JobAnnotationsUpdateRequest,),
                 },
                 'attribute_map': {
                     'id': 'id',
+                    'cloud_storage_id': 'cloud_storage_id',
+                    'filename': 'filename',
                     'format': 'format',
+                    'location': 'location',
                     'rq_id': 'rq_id',
+                    'use_default_location': 'use_default_location',
                 },
                 'location_map': {
                     'id': 'path',
+                    'cloud_storage_id': 'query',
+                    'filename': 'query',
                     'format': 'query',
+                    'location': 'query',
                     'rq_id': 'query',
+                    'use_default_location': 'query',
                     'job_annotations_update_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
@@ -989,18 +1135,95 @@
                     'application/json',
                     'multipart/form-data'
                 ]
             },
             api_client=api_client
         )
 
+    def create(
+        self,
+        job_write_request: JobWriteRequest,
+        *,
+        _parse_response: bool = True,
+        _request_timeout: typing.Union[int, float, tuple] = None,
+        _validate_inputs: bool = True,
+        _validate_outputs: bool = True,
+        _check_status: bool = True,
+        _spec_property_naming: bool = False,
+        _content_type: typing.Optional[str] = None,
+        _host_index: typing.Optional[int] = None,
+        _request_auths: typing.Optional[typing.List] = None,
+        _async_call: bool = False,
+        **kwargs,
+    ) -> typing.Tuple[typing.Optional[JobRead], urllib3.HTTPResponse]:
+        """Method creates a new job in the task  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass _async_call=True
+
+        >>> thread = api.create(job_write_request, _async_call=True)
+        >>> result = thread.get()
+
+        Args:
+            job_write_request (JobWriteRequest):
+
+        Keyword Args:
+            _parse_response (bool): if False, the response data will not be parsed,
+                None is returned for data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _validate_inputs (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _validate_outputs (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _check_status (bool): whether to check response status
+                for being positive or not.
+                Default is True
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            _async_call (bool): execute request asynchronously
+
+        Returns:
+            (JobRead, HTTPResponse)
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['_async_call'] = _async_call
+        kwargs['_parse_response'] = _parse_response
+        kwargs['_request_timeout'] = _request_timeout
+        kwargs['_validate_inputs'] = _validate_inputs
+        kwargs['_validate_outputs'] = _validate_outputs
+        kwargs['_check_status'] = _check_status
+        kwargs['_spec_property_naming'] = _spec_property_naming
+        kwargs['_content_type'] = _content_type
+        kwargs['_host_index'] = _host_index
+        kwargs['_request_auths'] = _request_auths
+        kwargs['job_write_request'] = job_write_request
+        return self.create_endpoint.call_with_http_info(**kwargs)
+
     def create_annotations(
         self,
         id: int,
-        annotation_file_request: AnnotationFileRequest,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
         _validate_outputs: bool = True,
         _check_status: bool = True,
         _spec_property_naming: bool = False,
@@ -1012,27 +1235,27 @@
     ) -> typing.Tuple[typing.Optional[None], urllib3.HTTPResponse]:
         """Method allows to initialize the process of the job annotation upload from a local file or a cloud storage  # noqa: E501
 
          The request POST /api/jobs/id/annotations will initiate file upload and will create the rq job on the server in which the process of annotations uploading from file will be carried out. Please, use the PUT /api/jobs/id/annotations endpoint for checking status of the process.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
-        >>> thread = api.create_annotations(id, annotation_file_request, _async_call=True)
+        >>> thread = api.create_annotations(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this job.
-            annotation_file_request (AnnotationFileRequest):
 
         Keyword Args:
             cloud_storage_id (float): Storage id. [optional]
             filename (str): Annotation file name. [optional]
             format (str): Input format name You can get the list of supported formats at: /server/annotation/formats. [optional]
             location (str): where to import the annotation from. [optional]
             use_default_location (bool): Use the location that was configured in the task to import annotation. [optional] if omitted the server will use the default value of True
+            annotation_file_request (AnnotationFileRequest): [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -1073,17 +1296,95 @@
         kwargs['_validate_outputs'] = _validate_outputs
         kwargs['_check_status'] = _check_status
         kwargs['_spec_property_naming'] = _spec_property_naming
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
         kwargs['id'] = id
-        kwargs['annotation_file_request'] = annotation_file_request
         return self.create_annotations_endpoint.call_with_http_info(**kwargs)
 
+    def destroy(
+        self,
+        id: int,
+        *,
+        _parse_response: bool = True,
+        _request_timeout: typing.Union[int, float, tuple] = None,
+        _validate_inputs: bool = True,
+        _validate_outputs: bool = True,
+        _check_status: bool = True,
+        _spec_property_naming: bool = False,
+        _content_type: typing.Optional[str] = None,
+        _host_index: typing.Optional[int] = None,
+        _request_auths: typing.Optional[typing.List] = None,
+        _async_call: bool = False,
+        **kwargs,
+    ) -> typing.Tuple[typing.Optional[None], urllib3.HTTPResponse]:
+        """Method deletes a job and its related annotations  # noqa: E501
+
+        Please note, that not every job can be removed. Currently, it is only available for Ground Truth jobs.   # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass _async_call=True
+
+        >>> thread = api.destroy(id, _async_call=True)
+        >>> result = thread.get()
+
+        Args:
+            id (int): A unique integer value identifying this job.
+
+        Keyword Args:
+            _parse_response (bool): if False, the response data will not be parsed,
+                None is returned for data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _validate_inputs (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _validate_outputs (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _check_status (bool): whether to check response status
+                for being positive or not.
+                Default is True
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            _async_call (bool): execute request asynchronously
+
+        Returns:
+            (None, HTTPResponse)
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['_async_call'] = _async_call
+        kwargs['_parse_response'] = _parse_response
+        kwargs['_request_timeout'] = _request_timeout
+        kwargs['_validate_inputs'] = _validate_inputs
+        kwargs['_validate_outputs'] = _validate_outputs
+        kwargs['_check_status'] = _check_status
+        kwargs['_spec_property_naming'] = _spec_property_naming
+        kwargs['_content_type'] = _content_type
+        kwargs['_host_index'] = _host_index
+        kwargs['_request_auths'] = _request_auths
+        kwargs['id'] = id
+        return self.destroy_endpoint.call_with_http_info(**kwargs)
+
     def destroy_annotations(
         self,
         id: int,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
@@ -1182,27 +1483,28 @@
         >>> result = thread.get()
 
 
         Keyword Args:
             x_organization (str): Organization unique slug. [optional]
             assignee (str): A simple equality filter for the assignee field. [optional]
             dimension (str): A simple equality filter for the dimension field. [optional]
-            filter (str): A filter term. Available filter_fields: ['task_name', 'project_name', 'assignee', 'state', 'stage', 'id', 'task_id', 'project_id', 'updated_date', 'dimension']. [optional]
+            filter (str): A filter term. Available filter_fields: ['task_name', 'project_name', 'assignee', 'state', 'stage', 'id', 'task_id', 'project_id', 'updated_date', 'dimension', 'type']. [optional]
             org (str): Organization unique slug. [optional]
             org_id (int): Organization identifier. [optional]
             page (int): A page number within the paginated result set.. [optional]
             page_size (int): Number of results to return per page.. [optional]
             project_id (int): A simple equality filter for the project_id field. [optional]
             project_name (str): A simple equality filter for the project_name field. [optional]
             search (str): A search term. Available search_fields: ('task_name', 'project_name', 'assignee', 'state', 'stage'). [optional]
-            sort (str): Which field to use when ordering the results. Available ordering_fields: ['task_name', 'project_name', 'assignee', 'state', 'stage', 'id', 'task_id', 'project_id', 'updated_date', 'dimension']. [optional]
+            sort (str): Which field to use when ordering the results. Available ordering_fields: ['task_name', 'project_name', 'assignee', 'state', 'stage', 'id', 'task_id', 'project_id', 'updated_date', 'dimension', 'type']. [optional]
             stage (str): A simple equality filter for the stage field. [optional]
             state (str): A simple equality filter for the state field. [optional]
             task_id (int): A simple equality filter for the task_id field. [optional]
             task_name (str): A simple equality filter for the task_name field. [optional]
+            type (str): A simple equality filter for the type field. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -1919,16 +2221,20 @@
         >>> thread = api.update_annotations(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this job.
 
         Keyword Args:
+            cloud_storage_id (float): Storage id. [optional]
+            filename (str): Annotation file name. [optional]
             format (str): Input format name You can get the list of supported formats at: /server/annotation/formats. [optional]
+            location (str): where to import the annotation from. [optional]
             rq_id (str): rq id. [optional]
+            use_default_location (bool): Use the location that was configured in the task to import annotation. [optional] if omitted the server will use the default value of True
             job_annotations_update_request (JobAnnotationsUpdateRequest): [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/api/labels_api.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/api/labels_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/api/lambda_api.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/api/lambda_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/api/memberships_api.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/api/memberships_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/api/organizations_api.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/api/organizations_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/api/projects_api.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/api/projects_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/api/schema_api.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/api/schema_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/api/server_api.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/api/server_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/api/tasks_api.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/api/tasks_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -298,26 +298,24 @@
                 'endpoint_path': '/api/tasks/backup/',
                 'operation_id': 'create_backup',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'task_file_request',
                     'x_organization',
                     'cloud_storage_id',
                     'filename',
                     'location',
                     'org',
                     'org_id',
                     'rq_id',
-                ],
-                'required': [
                     'task_file_request',
                 ],
+                'required': [],
                 'nullable': [
                 ],
                 'enum': [
                     'location',
                 ],
                 'validation': [
                 ]
@@ -329,49 +327,49 @@
                     ('location',): {
 
                         "CLOUD_STORAGE": "cloud_storage",
                         "LOCAL": "local"
                     },
                 },
                 'openapi_types': {
-                    'task_file_request':
-                        (TaskFileRequest,),
                     'x_organization':
                         (str,),
                     'cloud_storage_id':
                         (float,),
                     'filename':
                         (str,),
                     'location':
                         (str,),
                     'org':
                         (str,),
                     'org_id':
                         (int,),
                     'rq_id':
                         (str,),
+                    'task_file_request':
+                        (TaskFileRequest,),
                 },
                 'attribute_map': {
                     'x_organization': 'X-Organization',
                     'cloud_storage_id': 'cloud_storage_id',
                     'filename': 'filename',
                     'location': 'location',
                     'org': 'org',
                     'org_id': 'org_id',
                     'rq_id': 'rq_id',
                 },
                 'location_map': {
-                    'task_file_request': 'body',
                     'x_organization': 'header',
                     'cloud_storage_id': 'query',
                     'filename': 'query',
                     'location': 'query',
                     'org': 'query',
                     'org_id': 'query',
                     'rq_id': 'query',
+                    'task_file_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
@@ -397,22 +395,21 @@
                 'operation_id': 'create_data',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'data_request',
                     'upload_finish',
                     'upload_multiple',
                     'upload_start',
+                    'data_request',
                 ],
                 'required': [
                     'id',
-                    'data_request',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
@@ -421,35 +418,35 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'data_request':
-                        (DataRequest,),
                     'upload_finish':
                         (bool,),
                     'upload_multiple':
                         (bool,),
                     'upload_start':
                         (bool,),
+                    'data_request':
+                        (DataRequest,),
                 },
                 'attribute_map': {
                     'id': 'id',
                     'upload_finish': 'Upload-Finish',
                     'upload_multiple': 'Upload-Multiple',
                     'upload_start': 'Upload-Start',
                 },
                 'location_map': {
                     'id': 'path',
-                    'data_request': 'body',
                     'upload_finish': 'header',
                     'upload_multiple': 'header',
                     'upload_start': 'header',
+                    'data_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [
@@ -1809,15 +1806,14 @@
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
         kwargs['id'] = id
         return self.create_annotations_endpoint.call_with_http_info(**kwargs)
 
     def create_backup(
         self,
-        task_file_request: TaskFileRequest,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
         _validate_outputs: bool = True,
         _check_status: bool = True,
         _spec_property_naming: bool = False,
@@ -1829,28 +1825,27 @@
     ) -> typing.Tuple[typing.Optional[None], urllib3.HTTPResponse]:
         """Method recreates a task from an attached task backup file  # noqa: E501
 
          The backup import process is as follows:  The first request POST /api/tasks/backup will initiate file upload and will create the rq job on the server in which the process of a task creating from an uploaded backup will be carried out.  After initiating the backup upload, you will receive an rq_id parameter. Make sure to include this parameter as a query parameter in your subsequent requests to track the status of the task creation. Once the task has been successfully created, the server will return the id of the newly created task.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
-        >>> thread = api.create_backup(task_file_request, _async_call=True)
+        >>> thread = api.create_backup(_async_call=True)
         >>> result = thread.get()
 
-        Args:
-            task_file_request (TaskFileRequest):
 
         Keyword Args:
             x_organization (str): Organization unique slug. [optional]
             cloud_storage_id (float): Storage id. [optional]
             filename (str): Backup file name. [optional]
             location (str): Where to import the backup file from. [optional] if omitted the server will use the default value of "local"
             org (str): Organization unique slug. [optional]
             org_id (int): Organization identifier. [optional]
             rq_id (str): rq id. [optional]
+            task_file_request (TaskFileRequest): [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -1890,21 +1885,19 @@
         kwargs['_validate_inputs'] = _validate_inputs
         kwargs['_validate_outputs'] = _validate_outputs
         kwargs['_check_status'] = _check_status
         kwargs['_spec_property_naming'] = _spec_property_naming
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
-        kwargs['task_file_request'] = task_file_request
         return self.create_backup_endpoint.call_with_http_info(**kwargs)
 
     def create_data(
         self,
         id: int,
-        data_request: DataRequest,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
         _validate_outputs: bool = True,
         _check_status: bool = True,
         _spec_property_naming: bool = False,
@@ -1916,25 +1909,25 @@
     ) -> typing.Tuple[typing.Optional[None], urllib3.HTTPResponse]:
         """Method permanently attaches data (images, video, etc.) to a task  # noqa: E501
 
         Allows to upload data to a task. Supports the TUS open file uploading protocol (https://tus.io/).  Supports the following protocols:  1. A single Data request  and  2.1. An Upload-Start request 2.2.a. Regular TUS protocol requests (Upload-Length + Chunks) 2.2.b. Upload-Multiple requests 2.3. An Upload-Finish request  Requests: - Data - POST, no extra headers or 'Upload-Start' + 'Upload-Finish' headers.   Contains data in the body. - Upload-Start - POST, has an 'Upload-Start' header. No body is expected. - Upload-Length - POST, has an 'Upload-Length' header (see the TUS specification) - Chunk - HEAD/PATCH (see the TUS specification). Sent to /data/<file id> endpoints. - Upload-Finish - POST, has an 'Upload-Finish' header. Can contain data in the body. - Upload-Multiple - POST, has an 'Upload-Multiple' header. Contains data in the body.  The 'Upload-Finish' request allows to specify the uploaded files should be ordered. This may be needed if the files can be sent unordered. To state that the input files are sent ordered, pass an empty list of files in the 'upload_file_order' field. If the files are sent unordered, the ordered file list is expected in the 'upload_file_order' field. It must be a list of string file paths, relative to the dataset root.  Example: files = [     \"cats/cat_1.jpg\",     \"dogs/dog2.jpg\",     \"image_3.png\",     ... ]  Independently of the file declaration field used ('client_files', 'server_files', etc.), when the 'predefined' sorting method is selected, the uploaded files will be ordered according to the '.jsonl' manifest file, if it is found in the list of files. For archives (e.g. '.zip'), a manifest file ('*.jsonl') is required when using the 'predefined' file ordering. Such file must be provided next to the archive in the list of files. Read more about manifest files here: https://opencv.github.io/cvat/docs/manual/advanced/dataset_manifest/  After all data is sent, the operation status can be retrieved via the /status endpoint.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass _async_call=True
 
-        >>> thread = api.create_data(id, data_request, _async_call=True)
+        >>> thread = api.create_data(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this task.
-            data_request (DataRequest):
 
         Keyword Args:
             upload_finish (bool): Finishes data upload. Can be combined with Upload-Start header to create task data with one request. [optional]
             upload_multiple (bool): Indicates that data with this request are single or multiple files that should be attached to a task. [optional]
             upload_start (bool): Initializes data upload. Optionally, can include upload metadata in the request body.. [optional]
+            data_request (DataRequest): [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
@@ -1975,15 +1968,14 @@
         kwargs['_validate_outputs'] = _validate_outputs
         kwargs['_check_status'] = _check_status
         kwargs['_spec_property_naming'] = _spec_property_naming
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
         kwargs['id'] = id
-        kwargs['data_request'] = data_request
         return self.create_data_endpoint.call_with_http_info(**kwargs)
 
     def destroy(
         self,
         id: int,
         *,
         _parse_response: bool = True,
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/api/users_api.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/api/users_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/api/webhooks_api.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/api/webhooks_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -424,19 +424,16 @@
                 'operation_id': 'list_deliveries',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
-                    'filter',
                     'page',
                     'page_size',
-                    'search',
-                    'sort',
                 ],
                 'required': [
                     'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -448,40 +445,28 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'id':
                         (int,),
-                    'filter':
-                        (str,),
                     'page':
                         (int,),
                     'page_size':
                         (int,),
-                    'search':
-                        (str,),
-                    'sort':
-                        (str,),
                 },
                 'attribute_map': {
                     'id': 'id',
-                    'filter': 'filter',
                     'page': 'page',
                     'page_size': 'page_size',
-                    'search': 'search',
-                    'sort': 'sort',
                 },
                 'location_map': {
                     'id': 'path',
-                    'filter': 'query',
                     'page': 'query',
                     'page_size': 'query',
-                    'search': 'query',
-                    'sort': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
@@ -1218,19 +1203,16 @@
         >>> thread = api.list_deliveries(id, _async_call=True)
         >>> result = thread.get()
 
         Args:
             id (int): A unique integer value identifying this webhook.
 
         Keyword Args:
-            filter (str): A filter term. Available filter_fields: None. [optional]
             page (int): A page number within the paginated result set.. [optional]
             page_size (int): Number of results to return per page.. [optional]
-            search (str): A search term. Available search_fields: None. [optional]
-            sort (str): Which field to use when ordering the results. Available ordering_fields: None. [optional]
             _parse_response (bool): if False, the response data will not be parsed,
                 None is returned for data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
                 be a pair (tuple) of (connection, read) timeouts.
                 Default is None.
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/api_client.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import json
@@ -77,14 +77,15 @@
     issues_api: IssuesApi
     jobs_api: JobsApi
     labels_api: LabelsApi
     lambda_api: LambdaApi
     memberships_api: MembershipsApi
     organizations_api: OrganizationsApi
     projects_api: ProjectsApi
+    quality_api: QualityApi
     schema_api: SchemaApi
     server_api: ServerApi
     tasks_api: TasksApi
     users_api: UsersApi
     webhooks_api: WebhooksApi
     """
 
@@ -110,15 +111,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers: typing.Dict[str, str] = headers or {}
         self.cookies = SimpleCookie()
         if cookies:
             self.cookies.update(cookies)
         # Set default User-Agent.
-        self.user_agent = 'cvat_sdk/2.4.6'
+        self.user_agent = 'cvat_sdk/2.4.7'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
@@ -727,14 +728,15 @@
     issues_api: 'IssuesApi'
     jobs_api: 'JobsApi'
     labels_api: 'LabelsApi'
     lambda_api: 'LambdaApi'
     memberships_api: 'MembershipsApi'
     organizations_api: 'OrganizationsApi'
     projects_api: 'ProjectsApi'
+    quality_api: 'QualityApi'
     schema_api: 'SchemaApi'
     server_api: 'ServerApi'
     tasks_api: 'TasksApi'
     users_api: 'UsersApi'
     webhooks_api: 'WebhooksApi'
 
     _apis: typing.Dict[str, object] = { 
@@ -746,14 +748,15 @@
         'issues_api': [None, 'IssuesApi'],
         'jobs_api': [None, 'JobsApi'],
         'labels_api': [None, 'LabelsApi'],
         'lambda_api': [None, 'LambdaApi'],
         'memberships_api': [None, 'MembershipsApi'],
         'organizations_api': [None, 'OrganizationsApi'],
         'projects_api': [None, 'ProjectsApi'],
+        'quality_api': [None, 'QualityApi'],
         'schema_api': [None, 'SchemaApi'],
         'server_api': [None, 'ServerApi'],
         'tasks_api': [None, 'TasksApi'],
         'users_api': [None, 'UsersApi'],
         'webhooks_api': [None, 'WebhooksApi'],
     }
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/apis/__init__.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/apis/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 # Import all APIs into this package.
 # If you have many APIs here with many many models used in each API this may
 # raise a `RecursionError`.
@@ -33,12 +33,13 @@
 from cvat_sdk.api_client.api.issues_api import IssuesApi
 from cvat_sdk.api_client.api.jobs_api import JobsApi
 from cvat_sdk.api_client.api.labels_api import LabelsApi
 from cvat_sdk.api_client.api.lambda_api import LambdaApi
 from cvat_sdk.api_client.api.memberships_api import MembershipsApi
 from cvat_sdk.api_client.api.organizations_api import OrganizationsApi
 from cvat_sdk.api_client.api.projects_api import ProjectsApi
+from cvat_sdk.api_client.api.quality_api import QualityApi
 from cvat_sdk.api_client.api.schema_api import SchemaApi
 from cvat_sdk.api_client.api.server_api import ServerApi
 from cvat_sdk.api_client.api.tasks_api import TasksApi
 from cvat_sdk.api_client.api.users_api import UsersApi
 from cvat_sdk.api_client.api.webhooks_api import WebhooksApi
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/configuration.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
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
-               "Version of the API: 2.4.6\n"\
-               "SDK Package Version: 2.4.6".\
+               "Version of the API: 2.4.7\n"\
+               "SDK Package Version: 2.4.7".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/exceptions.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/about.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/about.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/annotation_file_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/annotation_file_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/annotations_read.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/annotations_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/attribute.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/attribute.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/attribute_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/attribute_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/attribute_val.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/attribute_val.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/attribute_val_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/attribute_val_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/backup_write_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/backup_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/basic_user.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/basic_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/basic_user_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/basic_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/chunk_type.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/chunk_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/client_events.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/client_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/client_events_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/client_events_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/cloud_storage_content.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/cloud_storage_content.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/cloud_storage_read.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/cloud_storage_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/cloud_storage_write_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/cloud_storage_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/comment_read.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/comment_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/comment_read_owner.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/comment_read_owner.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/comment_write_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/comment_write_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/comments_summary.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/comments_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/credentials_type_enum.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/credentials_type_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/data_meta_read.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/data_meta_read.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -62,14 +62,15 @@
     """
     [optional]
     """
 
     size: int # noqa: E501
     """
     [optional]
+    The number of frames included. Deleted frames do not affect this value. .
     """
 
     image_quality: int # noqa: E501
     """
     """
 
     start_frame: int # noqa: E501
@@ -93,14 +94,21 @@
     """
 
     deleted_frames: typing.List[int] # noqa: E501
     """
     [int]
     """
 
+    included_frames: typing.Union[typing.List[int], none_type] # noqa: E501
+    """
+    [optional]
+    [int], none_type
+    A list of valid frame ids. The None value means all frames are included. .
+    """
+
 
 class DataMetaRead(ModelNormal, IDataMetaRead):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -110,22 +118,24 @@
 
       frames ([FrameMeta], none_type):
 
       deleted_frames ([int]):
 
       chunk_size (int, none_type): [optional]  # noqa: E501
 
-      size (int): [optional]  # noqa: E501
+      size (int): The number of frames included. Deleted frames do not affect this value. . [optional]  # noqa: E501
 
       start_frame (int): [optional]  # noqa: E501
 
       stop_frame (int): [optional]  # noqa: E501
 
       frame_filter (str): [optional]  # noqa: E501
 
+      included_frames ([int], none_type): A list of valid frame ids. The None value means all frames are included. . [optional]  # noqa: E501
+
 
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
       attribute_map (dict): The key is attribute name
           and the value is json key in definition.
@@ -178,14 +188,15 @@
             'frames': ([FrameMeta], none_type,),  # noqa: E501
             'deleted_frames': ([int],),  # noqa: E501
             'chunk_size': (int, none_type,),  # noqa: E501
             'size': (int,),  # noqa: E501
             'start_frame': (int,),  # noqa: E501
             'stop_frame': (int,),  # noqa: E501
             'frame_filter': (str,),  # noqa: E501
+            'included_frames': ([int], none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -195,14 +206,15 @@
         'frames': 'frames',  # noqa: E501
         'deleted_frames': 'deleted_frames',  # noqa: E501
         'chunk_size': 'chunk_size',  # noqa: E501
         'size': 'size',  # noqa: E501
         'start_frame': 'start_frame',  # noqa: E501
         'stop_frame': 'stop_frame',  # noqa: E501
         'frame_filter': 'frame_filter',  # noqa: E501
+        'included_frames': 'included_frames',  # noqa: E501
     }
 
     read_only_vars = {
         'chunk_size',  # noqa: E501
         'size',  # noqa: E501
         'start_frame',  # noqa: E501
         'stop_frame',  # noqa: E501
@@ -220,22 +232,24 @@
             image_quality (int):
             frames ([FrameMeta], none_type):
             deleted_frames ([int]):
 
         Keyword Args:
             chunk_size (int, none_type): [optional]  # noqa: E501
 
-            size (int): [optional]  # noqa: E501
+            size (int): The number of frames included. Deleted frames do not affect this value. . [optional]  # noqa: E501
 
             start_frame (int): [optional]  # noqa: E501
 
             stop_frame (int): [optional]  # noqa: E501
 
             frame_filter (str): [optional]  # noqa: E501
 
+            included_frames ([int], none_type): A list of valid frame ids. The None value means all frames are included. . [optional]  # noqa: E501
+
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -324,22 +338,24 @@
             image_quality (int):
             frames ([FrameMeta], none_type):
             deleted_frames ([int]):
 
         Keyword Args:
             chunk_size (int, none_type): [optional]  # noqa: E501
 
-            size (int): [optional]  # noqa: E501
+            size (int): The number of frames included. Deleted frames do not affect this value. . [optional]  # noqa: E501
 
             start_frame (int): [optional]  # noqa: E501
 
             stop_frame (int): [optional]  # noqa: E501
 
             frame_filter (str): [optional]  # noqa: E501
 
+            included_frames ([int], none_type): A list of valid frame ids. The None value means all frames are included. . [optional]  # noqa: E501
+
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/data_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/data_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/dataset_file_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/dataset_file_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/dataset_format.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/dataset_format.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/dataset_formats.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/dataset_formats.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/dataset_write_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/dataset_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/event.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/event_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/event_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/events.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/events_enum.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/events_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/file_info.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/file_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/file_info_type_enum.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/file_info_type_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/frame_meta.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/frame_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/input_type_enum.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/input_type_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/invitation_read.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/invitation_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/invitation_write_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/invitation_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/issue_read.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/issue_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/issue_write_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/issue_write_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/issues_summary.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/issues_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/job_annotations_update_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/job_annotations_update_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/job_read.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/job_read.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -45,21 +45,23 @@
 
 def lazy_import():
     from cvat_sdk.api_client.model.chunk_type import ChunkType
     from cvat_sdk.api_client.model.issues_summary import IssuesSummary
     from cvat_sdk.api_client.model.job_read_assignee import JobReadAssignee
     from cvat_sdk.api_client.model.job_stage import JobStage
     from cvat_sdk.api_client.model.job_status import JobStatus
+    from cvat_sdk.api_client.model.job_type import JobType
     from cvat_sdk.api_client.model.labels_summary import LabelsSummary
     from cvat_sdk.api_client.model.operation_status import OperationStatus
     globals()['ChunkType'] = ChunkType
     globals()['IssuesSummary'] = IssuesSummary
     globals()['JobReadAssignee'] = JobReadAssignee
     globals()['JobStage'] = JobStage
     globals()['JobStatus'] = JobStatus
+    globals()['JobType'] = JobType
     globals()['LabelsSummary'] = LabelsSummary
     globals()['OperationStatus'] = OperationStatus
 
 
 
 class IJobRead(IModelData):
     """
@@ -121,14 +123,19 @@
     """
 
     mode: str # noqa: E501
     """
     [optional]
     """
 
+    frame_count: int # noqa: E501
+    """
+    [optional]
+    """
+
     start_frame: int # noqa: E501
     """
     [optional]
     """
 
     stop_frame: int # noqa: E501
     """
@@ -136,20 +143,20 @@
     """
 
     data_chunk_size: typing.Union[int, none_type] # noqa: E501
     """
     [optional]
     """
 
-    organization: typing.Union[int, none_type] # noqa: E501
+    data_compressed_chunk_type: typing.Union[typing.Any, none_type] # noqa: E501
     """
     [optional]
     """
 
-    data_compressed_chunk_type: typing.Union[typing.Any, none_type] # noqa: E501
+    created_date: datetime # noqa: E501
     """
     [optional]
     """
 
     updated_date: datetime # noqa: E501
     """
     [optional]
@@ -159,14 +166,24 @@
     """
     """
 
     labels: LabelsSummary # noqa: E501
     """
     """
 
+    type: typing.Union[typing.Any, none_type] # noqa: E501
+    """
+    [optional]
+    """
+
+    organization: typing.Union[int, none_type] # noqa: E501
+    """
+    [optional]
+    """
+
 
 class JobRead(ModelNormal, IJobRead):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -194,26 +211,32 @@
 
       stage (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
       state (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
       mode (str): [optional]  # noqa: E501
 
+      frame_count (int): [optional]  # noqa: E501
+
       start_frame (int): [optional]  # noqa: E501
 
       stop_frame (int): [optional]  # noqa: E501
 
       data_chunk_size (int, none_type): [optional]  # noqa: E501
 
-      organization (int, none_type): [optional]  # noqa: E501
-
       data_compressed_chunk_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
+      created_date (datetime): [optional]  # noqa: E501
+
       updated_date (datetime): [optional]  # noqa: E501
 
+      type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+
+      organization (int, none_type): [optional]  # noqa: E501
+
 
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
       attribute_map (dict): The key is attribute name
           and the value is json key in definition.
@@ -285,20 +308,23 @@
             'assignee': (JobReadAssignee,),  # noqa: E501
             'dimension': (str,),  # noqa: E501
             'bug_tracker': (str, none_type,),  # noqa: E501
             'status': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'stage': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'state': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'mode': (str,),  # noqa: E501
+            'frame_count': (int,),  # noqa: E501
             'start_frame': (int,),  # noqa: E501
             'stop_frame': (int,),  # noqa: E501
             'data_chunk_size': (int, none_type,),  # noqa: E501
-            'organization': (int, none_type,),  # noqa: E501
             'data_compressed_chunk_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'created_date': (datetime,),  # noqa: E501
             'updated_date': (datetime,),  # noqa: E501
+            'type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'organization': (int, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -313,39 +339,45 @@
         'assignee': 'assignee',  # noqa: E501
         'dimension': 'dimension',  # noqa: E501
         'bug_tracker': 'bug_tracker',  # noqa: E501
         'status': 'status',  # noqa: E501
         'stage': 'stage',  # noqa: E501
         'state': 'state',  # noqa: E501
         'mode': 'mode',  # noqa: E501
+        'frame_count': 'frame_count',  # noqa: E501
         'start_frame': 'start_frame',  # noqa: E501
         'stop_frame': 'stop_frame',  # noqa: E501
         'data_chunk_size': 'data_chunk_size',  # noqa: E501
-        'organization': 'organization',  # noqa: E501
         'data_compressed_chunk_type': 'data_compressed_chunk_type',  # noqa: E501
+        'created_date': 'created_date',  # noqa: E501
         'updated_date': 'updated_date',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'organization': 'organization',  # noqa: E501
     }
 
     read_only_vars = {
         'url',  # noqa: E501
         'id',  # noqa: E501
         'task_id',  # noqa: E501
         'project_id',  # noqa: E501
         'dimension',  # noqa: E501
         'bug_tracker',  # noqa: E501
         'status',  # noqa: E501
         'stage',  # noqa: E501
         'state',  # noqa: E501
         'mode',  # noqa: E501
+        'frame_count',  # noqa: E501
         'start_frame',  # noqa: E501
         'stop_frame',  # noqa: E501
         'data_chunk_size',  # noqa: E501
-        'organization',  # noqa: E501
         'data_compressed_chunk_type',  # noqa: E501
+        'created_date',  # noqa: E501
         'updated_date',  # noqa: E501
+        'type',  # noqa: E501
+        'organization',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, issues, labels, *args, **kwargs):  # noqa: E501
@@ -374,26 +406,32 @@
 
             stage (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
             state (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
             mode (str): [optional]  # noqa: E501
 
+            frame_count (int): [optional]  # noqa: E501
+
             start_frame (int): [optional]  # noqa: E501
 
             stop_frame (int): [optional]  # noqa: E501
 
             data_chunk_size (int, none_type): [optional]  # noqa: E501
 
-            organization (int, none_type): [optional]  # noqa: E501
-
             data_compressed_chunk_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
+            created_date (datetime): [optional]  # noqa: E501
+
             updated_date (datetime): [optional]  # noqa: E501
 
+            type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+
+            organization (int, none_type): [optional]  # noqa: E501
+
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -500,26 +538,32 @@
 
             stage (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
             state (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
             mode (str): [optional]  # noqa: E501
 
+            frame_count (int): [optional]  # noqa: E501
+
             start_frame (int): [optional]  # noqa: E501
 
             stop_frame (int): [optional]  # noqa: E501
 
             data_chunk_size (int, none_type): [optional]  # noqa: E501
 
-            organization (int, none_type): [optional]  # noqa: E501
-
             data_compressed_chunk_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
+            created_date (datetime): [optional]  # noqa: E501
+
             updated_date (datetime): [optional]  # noqa: E501
 
+            type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+
+            organization (int, none_type): [optional]  # noqa: E501
+
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/job_read_assignee.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/job_read_assignee.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/job_stage.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/job_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/job_status.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/job_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/jobs_summary.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/jobs_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/label.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/label.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/labeled_data.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/labeled_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/labeled_data_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/labeled_data_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/labeled_image.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/labeled_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/labeled_image_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/labeled_image_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/labeled_shape.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/labeled_shape.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/labeled_shape_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/labeled_shape_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/labeled_track.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/labeled_track.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/labeled_track_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/labeled_track_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/labels_summary.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/labels_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/location_enum.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/location_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/login_serializer_ex_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/login_serializer_ex_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/membership_read.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/membership_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/meta_user.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/meta_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/online_function_call_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/online_function_call_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/operation_status.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/operation_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/organization_read.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/organization_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/organization_write_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/organization_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_cloud_storage_read_list.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_cloud_storage_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_comment_read_list.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_comment_read_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_invitation_read_list.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_invitation_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_issue_read_list.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_issue_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_job_read_list.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_job_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_label_list.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_label_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_membership_read_list.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_membership_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_meta_user_list.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_meta_user_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_organization_read_list.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_organization_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_project_read_list.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_project_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_task_read_list.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_task_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_webhook_delivery_read_list.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_webhook_delivery_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/paginated_webhook_read_list.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/paginated_webhook_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/password_change_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/password_change_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/password_reset_confirm_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/password_reset_confirm_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/password_reset_serializer_ex_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/password_reset_serializer_ex_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_cloud_storage_write_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_cloud_storage_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_comment_write_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_comment_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_data_meta_write_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_data_meta_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_invitation_write_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_invitation_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_issue_write_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_issue_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_job_write_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_job_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_label_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_label_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_labeled_data_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_labeled_data_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_membership_write_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_membership_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_organization_write_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_organization_write_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_project_write_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_project_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_project_write_request_target_storage.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_project_write_request_target_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_task_write_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_task_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_task_write_request_target_storage.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_task_write_request_target_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_user_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/patched_webhook_write_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/patched_webhook_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/plugins.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/plugins.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/project_file_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/project_file_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/project_read.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/project_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/project_read_owner.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/project_read_owner.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/project_read_target_storage.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/project_read_target_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/project_write_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/project_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/provider_type_enum.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/provider_type_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/register_serializer_ex.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/register_serializer_ex.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/register_serializer_ex_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/register_serializer_ex_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/rest_auth_detail.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/rest_auth_detail.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/role_enum.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/role_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/rq_id.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/rq_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -52,26 +52,27 @@
 
     Do not edit the class manually.
     """
 
     # member type declarations
     rq_id: str # noqa: E501
     """
+    Request id.
     """
 
 
 class RqId(ModelNormal, IRqId):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
-      rq_id (str):
+      rq_id (str): Request id
 
 
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
       attribute_map (dict): The key is attribute name
@@ -135,15 +136,15 @@
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, rq_id, *args, **kwargs):  # noqa: E501
         """RqId - a model defined in OpenAPI
 
         Args:
-            rq_id (str):
+            rq_id (str): Request id
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -225,15 +226,15 @@
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, rq_id, *args, **kwargs):  # noqa: E501
         """RqId - a model defined in OpenAPI
 
         Args:
-            rq_id (str):
+            rq_id (str): Request id
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/rq_status.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/rq_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/rq_status_state_enum.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/rq_status_state_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/shape_type.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/shape_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/signing_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/signing_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/sorting_method.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/sorting_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/storage.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/storage_method.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/storage_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/storage_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/storage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/storage_type.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/storage_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/sub_labeled_shape.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/sub_labeled_shape.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/sub_labeled_shape_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/sub_labeled_shape_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/sub_labeled_track.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/sub_labeled_track.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/sub_labeled_track_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/sub_labeled_track_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/sublabel.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/sublabel.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/sublabel_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/sublabel_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/task_annotations_update_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/task_annotations_update_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/task_annotations_write_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/task_annotations_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/task_file_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/task_file_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/task_read.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/task_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/task_read_target_storage.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/task_read_target_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/task_write_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/task_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/tasks_summary.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/tasks_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/token.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/token.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/tracked_shape.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/tracked_shape.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/tracked_shape_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/tracked_shape_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/user.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/webhook_content_type.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/webhook_content_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/webhook_delivery_read.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/webhook_delivery_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/webhook_read.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/webhook_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/webhook_type.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/webhook_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model/webhook_write_request.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model/webhook_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/model_utils.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
 import inspect
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/models/__init__.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,30 +2,35 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 # import all models into this package
 # if you have many models here with many references from one model to another this may
 # raise a RecursionError
 # to avoid this, import only the models that you directly need like:
 # from from cvat_sdk.api_client.model.pet import Pet
 # or import this package, but before doing it, use:
 # import sys
 # sys.setrecursionlimit(n)
 
 from cvat_sdk.api_client.model.about import About, IAbout
+from cvat_sdk.api_client.model.annotation_conflict import AnnotationConflict, IAnnotationConflict
+from cvat_sdk.api_client.model.annotation_conflict_type_enum import AnnotationConflictTypeEnum, IAnnotationConflictTypeEnum
 from cvat_sdk.api_client.model.annotation_file_request import AnnotationFileRequest, IAnnotationFileRequest
+from cvat_sdk.api_client.model.annotation_id import AnnotationId, IAnnotationId
+from cvat_sdk.api_client.model.annotation_id_shape_type import AnnotationIdShapeType
+from cvat_sdk.api_client.model.annotation_id_type_enum import AnnotationIdTypeEnum, IAnnotationIdTypeEnum
 from cvat_sdk.api_client.model.annotations_read import AnnotationsRead
 from cvat_sdk.api_client.model.attribute import Attribute, IAttribute
 from cvat_sdk.api_client.model.attribute_request import AttributeRequest, IAttributeRequest
 from cvat_sdk.api_client.model.attribute_val import AttributeVal, IAttributeVal
 from cvat_sdk.api_client.model.attribute_val_request import AttributeValRequest, IAttributeValRequest
 from cvat_sdk.api_client.model.backup_write_request import BackupWriteRequest
 from cvat_sdk.api_client.model.basic_user import BasicUser, IBasicUser
@@ -50,25 +55,28 @@
 from cvat_sdk.api_client.model.event import Event, IEvent
 from cvat_sdk.api_client.model.event_request import EventRequest, IEventRequest
 from cvat_sdk.api_client.model.events import Events, IEvents
 from cvat_sdk.api_client.model.events_enum import EventsEnum, IEventsEnum
 from cvat_sdk.api_client.model.file_info import FileInfo, IFileInfo
 from cvat_sdk.api_client.model.file_info_type_enum import FileInfoTypeEnum, IFileInfoTypeEnum
 from cvat_sdk.api_client.model.frame_meta import FrameMeta, IFrameMeta
+from cvat_sdk.api_client.model.frame_selection_method_enum import FrameSelectionMethodEnum, IFrameSelectionMethodEnum
 from cvat_sdk.api_client.model.input_type_enum import InputTypeEnum, IInputTypeEnum
 from cvat_sdk.api_client.model.invitation_read import InvitationRead, IInvitationRead
 from cvat_sdk.api_client.model.invitation_write_request import InvitationWriteRequest, IInvitationWriteRequest
 from cvat_sdk.api_client.model.issue_read import IssueRead, IIssueRead
 from cvat_sdk.api_client.model.issue_write_request import IssueWriteRequest, IIssueWriteRequest
 from cvat_sdk.api_client.model.issues_summary import IssuesSummary, IIssuesSummary
 from cvat_sdk.api_client.model.job_annotations_update_request import JobAnnotationsUpdateRequest
 from cvat_sdk.api_client.model.job_read import JobRead, IJobRead
 from cvat_sdk.api_client.model.job_read_assignee import JobReadAssignee
 from cvat_sdk.api_client.model.job_stage import JobStage, IJobStage
 from cvat_sdk.api_client.model.job_status import JobStatus, IJobStatus
+from cvat_sdk.api_client.model.job_type import JobType, IJobType
+from cvat_sdk.api_client.model.job_write_request import JobWriteRequest, IJobWriteRequest
 from cvat_sdk.api_client.model.jobs_summary import JobsSummary, IJobsSummary
 from cvat_sdk.api_client.model.label import Label, ILabel
 from cvat_sdk.api_client.model.labeled_data import LabeledData, ILabeledData
 from cvat_sdk.api_client.model.labeled_data_request import LabeledDataRequest, ILabeledDataRequest
 from cvat_sdk.api_client.model.labeled_image import LabeledImage, ILabeledImage
 from cvat_sdk.api_client.model.labeled_image_request import LabeledImageRequest, ILabeledImageRequest
 from cvat_sdk.api_client.model.labeled_shape import LabeledShape, ILabeledShape
@@ -76,28 +84,32 @@
 from cvat_sdk.api_client.model.labeled_track import LabeledTrack, ILabeledTrack
 from cvat_sdk.api_client.model.labeled_track_request import LabeledTrackRequest, ILabeledTrackRequest
 from cvat_sdk.api_client.model.labels_summary import LabelsSummary, ILabelsSummary
 from cvat_sdk.api_client.model.location_enum import LocationEnum, ILocationEnum
 from cvat_sdk.api_client.model.login_serializer_ex_request import LoginSerializerExRequest, ILoginSerializerExRequest
 from cvat_sdk.api_client.model.membership_read import MembershipRead, IMembershipRead
 from cvat_sdk.api_client.model.meta_user import MetaUser
+from cvat_sdk.api_client.model.null_enum import NullEnum, INullEnum
 from cvat_sdk.api_client.model.online_function_call_request import OnlineFunctionCallRequest, IOnlineFunctionCallRequest
 from cvat_sdk.api_client.model.operation_status import OperationStatus, IOperationStatus
 from cvat_sdk.api_client.model.organization_read import OrganizationRead, IOrganizationRead
 from cvat_sdk.api_client.model.organization_write_request import OrganizationWriteRequest, IOrganizationWriteRequest
+from cvat_sdk.api_client.model.paginated_annotation_conflict_list import PaginatedAnnotationConflictList, IPaginatedAnnotationConflictList
 from cvat_sdk.api_client.model.paginated_cloud_storage_read_list import PaginatedCloudStorageReadList, IPaginatedCloudStorageReadList
 from cvat_sdk.api_client.model.paginated_comment_read_list import PaginatedCommentReadList, IPaginatedCommentReadList
 from cvat_sdk.api_client.model.paginated_invitation_read_list import PaginatedInvitationReadList, IPaginatedInvitationReadList
 from cvat_sdk.api_client.model.paginated_issue_read_list import PaginatedIssueReadList, IPaginatedIssueReadList
 from cvat_sdk.api_client.model.paginated_job_read_list import PaginatedJobReadList, IPaginatedJobReadList
 from cvat_sdk.api_client.model.paginated_label_list import PaginatedLabelList, IPaginatedLabelList
 from cvat_sdk.api_client.model.paginated_membership_read_list import PaginatedMembershipReadList, IPaginatedMembershipReadList
 from cvat_sdk.api_client.model.paginated_meta_user_list import PaginatedMetaUserList, IPaginatedMetaUserList
 from cvat_sdk.api_client.model.paginated_organization_read_list import PaginatedOrganizationReadList, IPaginatedOrganizationReadList
 from cvat_sdk.api_client.model.paginated_project_read_list import PaginatedProjectReadList, IPaginatedProjectReadList
+from cvat_sdk.api_client.model.paginated_quality_report_list import PaginatedQualityReportList, IPaginatedQualityReportList
+from cvat_sdk.api_client.model.paginated_quality_settings_list import PaginatedQualitySettingsList, IPaginatedQualitySettingsList
 from cvat_sdk.api_client.model.paginated_task_read_list import PaginatedTaskReadList, IPaginatedTaskReadList
 from cvat_sdk.api_client.model.paginated_webhook_delivery_read_list import PaginatedWebhookDeliveryReadList, IPaginatedWebhookDeliveryReadList
 from cvat_sdk.api_client.model.paginated_webhook_read_list import PaginatedWebhookReadList, IPaginatedWebhookReadList
 from cvat_sdk.api_client.model.password_change_request import PasswordChangeRequest, IPasswordChangeRequest
 from cvat_sdk.api_client.model.password_reset_confirm_request import PasswordResetConfirmRequest, IPasswordResetConfirmRequest
 from cvat_sdk.api_client.model.password_reset_serializer_ex_request import PasswordResetSerializerExRequest, IPasswordResetSerializerExRequest
 from cvat_sdk.api_client.model.patched_cloud_storage_write_request import PatchedCloudStorageWriteRequest, IPatchedCloudStorageWriteRequest
@@ -108,32 +120,39 @@
 from cvat_sdk.api_client.model.patched_job_write_request import PatchedJobWriteRequest, IPatchedJobWriteRequest
 from cvat_sdk.api_client.model.patched_label_request import PatchedLabelRequest, IPatchedLabelRequest
 from cvat_sdk.api_client.model.patched_labeled_data_request import PatchedLabeledDataRequest, IPatchedLabeledDataRequest
 from cvat_sdk.api_client.model.patched_membership_write_request import PatchedMembershipWriteRequest, IPatchedMembershipWriteRequest
 from cvat_sdk.api_client.model.patched_organization_write_request import PatchedOrganizationWriteRequest, IPatchedOrganizationWriteRequest
 from cvat_sdk.api_client.model.patched_project_write_request import PatchedProjectWriteRequest, IPatchedProjectWriteRequest
 from cvat_sdk.api_client.model.patched_project_write_request_target_storage import PatchedProjectWriteRequestTargetStorage
+from cvat_sdk.api_client.model.patched_quality_settings_request import PatchedQualitySettingsRequest, IPatchedQualitySettingsRequest
 from cvat_sdk.api_client.model.patched_task_write_request import PatchedTaskWriteRequest, IPatchedTaskWriteRequest
 from cvat_sdk.api_client.model.patched_task_write_request_target_storage import PatchedTaskWriteRequestTargetStorage
 from cvat_sdk.api_client.model.patched_user_request import PatchedUserRequest, IPatchedUserRequest
 from cvat_sdk.api_client.model.patched_webhook_write_request import PatchedWebhookWriteRequest, IPatchedWebhookWriteRequest
 from cvat_sdk.api_client.model.plugins import Plugins, IPlugins
 from cvat_sdk.api_client.model.project_file_request import ProjectFileRequest, IProjectFileRequest
 from cvat_sdk.api_client.model.project_read import ProjectRead, IProjectRead
 from cvat_sdk.api_client.model.project_read_owner import ProjectReadOwner
 from cvat_sdk.api_client.model.project_read_target_storage import ProjectReadTargetStorage
 from cvat_sdk.api_client.model.project_write_request import ProjectWriteRequest, IProjectWriteRequest
 from cvat_sdk.api_client.model.provider_type_enum import ProviderTypeEnum, IProviderTypeEnum
+from cvat_sdk.api_client.model.quality_report import QualityReport, IQualityReport
+from cvat_sdk.api_client.model.quality_report_create_request import QualityReportCreateRequest, IQualityReportCreateRequest
+from cvat_sdk.api_client.model.quality_report_summary import QualityReportSummary, IQualityReportSummary
+from cvat_sdk.api_client.model.quality_report_target import QualityReportTarget, IQualityReportTarget
+from cvat_sdk.api_client.model.quality_settings import QualitySettings, IQualitySettings
 from cvat_sdk.api_client.model.register_serializer_ex import RegisterSerializerEx, IRegisterSerializerEx
 from cvat_sdk.api_client.model.register_serializer_ex_request import RegisterSerializerExRequest, IRegisterSerializerExRequest
 from cvat_sdk.api_client.model.rest_auth_detail import RestAuthDetail, IRestAuthDetail
 from cvat_sdk.api_client.model.role_enum import RoleEnum, IRoleEnum
 from cvat_sdk.api_client.model.rq_id import RqId, IRqId
 from cvat_sdk.api_client.model.rq_status import RqStatus, IRqStatus
 from cvat_sdk.api_client.model.rq_status_state_enum import RqStatusStateEnum, IRqStatusStateEnum
+from cvat_sdk.api_client.model.severity_enum import SeverityEnum, ISeverityEnum
 from cvat_sdk.api_client.model.shape_type import ShapeType, IShapeType
 from cvat_sdk.api_client.model.signing_request import SigningRequest, ISigningRequest
 from cvat_sdk.api_client.model.sorting_method import SortingMethod, ISortingMethod
 from cvat_sdk.api_client.model.storage import Storage, IStorage
 from cvat_sdk.api_client.model.storage_method import StorageMethod, IStorageMethod
 from cvat_sdk.api_client.model.storage_request import StorageRequest, IStorageRequest
 from cvat_sdk.api_client.model.storage_type import StorageType, IStorageType
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/api_client/rest.py` & `cvat_sdk-2.4.7/cvat_sdk/api_client/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 import io
 import json
 import logging
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk/core/client.py` & `cvat_sdk-2.4.7/cvat_sdk/core/client.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.6/cvat_sdk/core/downloading.py` & `cvat_sdk-2.4.7/cvat_sdk/core/downloading.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.6/cvat_sdk/core/git.py` & `cvat_sdk-2.4.7/cvat_sdk/core/git.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.6/cvat_sdk/core/helpers.py` & `cvat_sdk-2.4.7/cvat_sdk/core/helpers.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.6/cvat_sdk/core/progress.py` & `cvat_sdk-2.4.7/cvat_sdk/core/progress.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.6/cvat_sdk/core/proxies/annotations.py` & `cvat_sdk-2.4.7/cvat_sdk/core/proxies/annotations.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.6/cvat_sdk/core/proxies/issues.py` & `cvat_sdk-2.4.7/cvat_sdk/core/proxies/issues.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.6/cvat_sdk/core/proxies/jobs.py` & `cvat_sdk-2.4.7/cvat_sdk/core/proxies/jobs.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.6/cvat_sdk/core/proxies/model_proxy.py` & `cvat_sdk-2.4.7/cvat_sdk/core/proxies/model_proxy.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.6/cvat_sdk/core/proxies/organizations.py` & `cvat_sdk-2.4.7/cvat_sdk/core/proxies/organizations.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.6/cvat_sdk/core/proxies/projects.py` & `cvat_sdk-2.4.7/cvat_sdk/core/proxies/projects.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.6/cvat_sdk/core/proxies/tasks.py` & `cvat_sdk-2.4.7/cvat_sdk/core/proxies/tasks.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.6/cvat_sdk/core/proxies/users.py` & `cvat_sdk-2.4.7/cvat_sdk/core/proxies/users.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.6/cvat_sdk/core/uploading.py` & `cvat_sdk-2.4.7/cvat_sdk/core/uploading.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.6/cvat_sdk/core/utils.py` & `cvat_sdk-2.4.7/cvat_sdk/core/utils.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.6/cvat_sdk/pytorch/caching.py` & `cvat_sdk-2.4.7/cvat_sdk/pytorch/caching.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.6/cvat_sdk/pytorch/common.py` & `cvat_sdk-2.4.7/cvat_sdk/pytorch/common.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.6/cvat_sdk/pytorch/project_dataset.py` & `cvat_sdk-2.4.7/cvat_sdk/pytorch/project_dataset.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.6/cvat_sdk/pytorch/task_dataset.py` & `cvat_sdk-2.4.7/cvat_sdk/pytorch/task_dataset.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.6/cvat_sdk/pytorch/transforms.py` & `cvat_sdk-2.4.7/cvat_sdk/pytorch/transforms.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.6/cvat_sdk.egg-info/PKG-INFO` & `cvat_sdk-2.4.7/cvat_sdk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvat-sdk
-Version: 2.4.6
+Version: 2.4.7
 Summary: CVAT REST API
 Home-page: https://github.com/cvat-ai/cvat
 Author: CVAT.ai team
 Author-email: support@cvat.ai
 License: MIT License
 Keywords: OpenAPI,OpenAPI-Generator,CVAT REST API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cvat_sdk-2.4.6/cvat_sdk.egg-info/SOURCES.txt` & `cvat_sdk-2.4.7/cvat_sdk.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -21,23 +21,29 @@
 ./cvat_sdk/api_client/api/issues_api.py
 ./cvat_sdk/api_client/api/jobs_api.py
 ./cvat_sdk/api_client/api/labels_api.py
 ./cvat_sdk/api_client/api/lambda_api.py
 ./cvat_sdk/api_client/api/memberships_api.py
 ./cvat_sdk/api_client/api/organizations_api.py
 ./cvat_sdk/api_client/api/projects_api.py
+./cvat_sdk/api_client/api/quality_api.py
 ./cvat_sdk/api_client/api/schema_api.py
 ./cvat_sdk/api_client/api/server_api.py
 ./cvat_sdk/api_client/api/tasks_api.py
 ./cvat_sdk/api_client/api/users_api.py
 ./cvat_sdk/api_client/api/webhooks_api.py
 ./cvat_sdk/api_client/apis/__init__.py
 ./cvat_sdk/api_client/model/__init__.py
 ./cvat_sdk/api_client/model/about.py
+./cvat_sdk/api_client/model/annotation_conflict.py
+./cvat_sdk/api_client/model/annotation_conflict_type_enum.py
 ./cvat_sdk/api_client/model/annotation_file_request.py
+./cvat_sdk/api_client/model/annotation_id.py
+./cvat_sdk/api_client/model/annotation_id_shape_type.py
+./cvat_sdk/api_client/model/annotation_id_type_enum.py
 ./cvat_sdk/api_client/model/annotations_read.py
 ./cvat_sdk/api_client/model/attribute.py
 ./cvat_sdk/api_client/model/attribute_request.py
 ./cvat_sdk/api_client/model/attribute_val.py
 ./cvat_sdk/api_client/model/attribute_val_request.py
 ./cvat_sdk/api_client/model/backup_write_request.py
 ./cvat_sdk/api_client/model/basic_user.py
@@ -62,25 +68,28 @@
 ./cvat_sdk/api_client/model/event.py
 ./cvat_sdk/api_client/model/event_request.py
 ./cvat_sdk/api_client/model/events.py
 ./cvat_sdk/api_client/model/events_enum.py
 ./cvat_sdk/api_client/model/file_info.py
 ./cvat_sdk/api_client/model/file_info_type_enum.py
 ./cvat_sdk/api_client/model/frame_meta.py
+./cvat_sdk/api_client/model/frame_selection_method_enum.py
 ./cvat_sdk/api_client/model/input_type_enum.py
 ./cvat_sdk/api_client/model/invitation_read.py
 ./cvat_sdk/api_client/model/invitation_write_request.py
 ./cvat_sdk/api_client/model/issue_read.py
 ./cvat_sdk/api_client/model/issue_write_request.py
 ./cvat_sdk/api_client/model/issues_summary.py
 ./cvat_sdk/api_client/model/job_annotations_update_request.py
 ./cvat_sdk/api_client/model/job_read.py
 ./cvat_sdk/api_client/model/job_read_assignee.py
 ./cvat_sdk/api_client/model/job_stage.py
 ./cvat_sdk/api_client/model/job_status.py
+./cvat_sdk/api_client/model/job_type.py
+./cvat_sdk/api_client/model/job_write_request.py
 ./cvat_sdk/api_client/model/jobs_summary.py
 ./cvat_sdk/api_client/model/label.py
 ./cvat_sdk/api_client/model/labeled_data.py
 ./cvat_sdk/api_client/model/labeled_data_request.py
 ./cvat_sdk/api_client/model/labeled_image.py
 ./cvat_sdk/api_client/model/labeled_image_request.py
 ./cvat_sdk/api_client/model/labeled_shape.py
@@ -88,28 +97,32 @@
 ./cvat_sdk/api_client/model/labeled_track.py
 ./cvat_sdk/api_client/model/labeled_track_request.py
 ./cvat_sdk/api_client/model/labels_summary.py
 ./cvat_sdk/api_client/model/location_enum.py
 ./cvat_sdk/api_client/model/login_serializer_ex_request.py
 ./cvat_sdk/api_client/model/membership_read.py
 ./cvat_sdk/api_client/model/meta_user.py
+./cvat_sdk/api_client/model/null_enum.py
 ./cvat_sdk/api_client/model/online_function_call_request.py
 ./cvat_sdk/api_client/model/operation_status.py
 ./cvat_sdk/api_client/model/organization_read.py
 ./cvat_sdk/api_client/model/organization_write_request.py
+./cvat_sdk/api_client/model/paginated_annotation_conflict_list.py
 ./cvat_sdk/api_client/model/paginated_cloud_storage_read_list.py
 ./cvat_sdk/api_client/model/paginated_comment_read_list.py
 ./cvat_sdk/api_client/model/paginated_invitation_read_list.py
 ./cvat_sdk/api_client/model/paginated_issue_read_list.py
 ./cvat_sdk/api_client/model/paginated_job_read_list.py
 ./cvat_sdk/api_client/model/paginated_label_list.py
 ./cvat_sdk/api_client/model/paginated_membership_read_list.py
 ./cvat_sdk/api_client/model/paginated_meta_user_list.py
 ./cvat_sdk/api_client/model/paginated_organization_read_list.py
 ./cvat_sdk/api_client/model/paginated_project_read_list.py
+./cvat_sdk/api_client/model/paginated_quality_report_list.py
+./cvat_sdk/api_client/model/paginated_quality_settings_list.py
 ./cvat_sdk/api_client/model/paginated_task_read_list.py
 ./cvat_sdk/api_client/model/paginated_webhook_delivery_read_list.py
 ./cvat_sdk/api_client/model/paginated_webhook_read_list.py
 ./cvat_sdk/api_client/model/password_change_request.py
 ./cvat_sdk/api_client/model/password_reset_confirm_request.py
 ./cvat_sdk/api_client/model/password_reset_serializer_ex_request.py
 ./cvat_sdk/api_client/model/patched_cloud_storage_write_request.py
@@ -120,32 +133,39 @@
 ./cvat_sdk/api_client/model/patched_job_write_request.py
 ./cvat_sdk/api_client/model/patched_label_request.py
 ./cvat_sdk/api_client/model/patched_labeled_data_request.py
 ./cvat_sdk/api_client/model/patched_membership_write_request.py
 ./cvat_sdk/api_client/model/patched_organization_write_request.py
 ./cvat_sdk/api_client/model/patched_project_write_request.py
 ./cvat_sdk/api_client/model/patched_project_write_request_target_storage.py
+./cvat_sdk/api_client/model/patched_quality_settings_request.py
 ./cvat_sdk/api_client/model/patched_task_write_request.py
 ./cvat_sdk/api_client/model/patched_task_write_request_target_storage.py
 ./cvat_sdk/api_client/model/patched_user_request.py
 ./cvat_sdk/api_client/model/patched_webhook_write_request.py
 ./cvat_sdk/api_client/model/plugins.py
 ./cvat_sdk/api_client/model/project_file_request.py
 ./cvat_sdk/api_client/model/project_read.py
 ./cvat_sdk/api_client/model/project_read_owner.py
 ./cvat_sdk/api_client/model/project_read_target_storage.py
 ./cvat_sdk/api_client/model/project_write_request.py
 ./cvat_sdk/api_client/model/provider_type_enum.py
+./cvat_sdk/api_client/model/quality_report.py
+./cvat_sdk/api_client/model/quality_report_create_request.py
+./cvat_sdk/api_client/model/quality_report_summary.py
+./cvat_sdk/api_client/model/quality_report_target.py
+./cvat_sdk/api_client/model/quality_settings.py
 ./cvat_sdk/api_client/model/register_serializer_ex.py
 ./cvat_sdk/api_client/model/register_serializer_ex_request.py
 ./cvat_sdk/api_client/model/rest_auth_detail.py
 ./cvat_sdk/api_client/model/role_enum.py
 ./cvat_sdk/api_client/model/rq_id.py
 ./cvat_sdk/api_client/model/rq_status.py
 ./cvat_sdk/api_client/model/rq_status_state_enum.py
+./cvat_sdk/api_client/model/severity_enum.py
 ./cvat_sdk/api_client/model/shape_type.py
 ./cvat_sdk/api_client/model/signing_request.py
 ./cvat_sdk/api_client/model/sorting_method.py
 ./cvat_sdk/api_client/model/storage.py
 ./cvat_sdk/api_client/model/storage_method.py
 ./cvat_sdk/api_client/model/storage_request.py
 ./cvat_sdk/api_client/model/storage_type.py
```

### Comparing `cvat_sdk-2.4.6/setup.py` & `cvat_sdk-2.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.4.6
+# The version of the OpenAPI document: 2.4.7
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 import os.path as osp
 import re
 from setuptools import find_packages, setup
```

