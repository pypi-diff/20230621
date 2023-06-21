# Comparing `tmp/lusid-notification-sdk-preview-0.1.748.post2.tar.gz` & `tmp/lusid-notification-sdk-preview-0.1.748.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lusid-notification-sdk-preview-0.1.748.post2.tar", last modified: Mon Jun 19 18:54:53 2023, max compression
+gzip compressed data, was "dist/lusid-notification-sdk-preview-0.1.748.post3.tar", last modified: Wed Jun 21 10:40:04 2023, max compression
```

## Comparing `lusid-notification-sdk-preview-0.1.748.post2.tar` & `lusid-notification-sdk-preview-0.1.748.post3.tar`

### file list

```diff
@@ -1,65 +1,64 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:54:53.000000 lusid-notification-sdk-preview-0.1.748.post2/
--rw-r--r--   0 root         (0) root         (0)       53 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      385 2023-06-19 18:54:53.000000 lusid-notification-sdk-preview-0.1.748.post2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8006 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:54:53.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/
--rw-r--r--   0 root         (0) root         (0)     4352 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/__init__.py
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:54:53.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/api/
--rw-r--r--   0 root         (0) root         (0)      442 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6851 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/api/application_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)    13990 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/api/event_types_api.py
--rw-r--r--   0 root         (0) root         (0)     7824 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/api/manual_event_api.py
--rw-r--r--   0 root         (0) root         (0)    52809 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/api/notifications_api.py
--rw-r--r--   0 root         (0) root         (0)    47815 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/api/subscriptions_api.py
--rw-r--r--   0 root         (0) root         (0)    27787 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/api_client.py
--rw-r--r--   0 root         (0) root         (0)    16637 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5101 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:54:53.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/
--rw-r--r--   0 root         (0) root         (0)     3062 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7256 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/access_controlled_action.py
--rw-r--r--   0 root         (0) root         (0)     9019 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7233 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/action_id.py
--rw-r--r--   0 root         (0) root         (0)    10959 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/amazon_sqs_notification_type.py
--rw-r--r--   0 root         (0) root         (0)     9236 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/api_request_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    10720 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/create_notification_request.py
--rw-r--r--   0 root         (0) root         (0)    38059 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/create_notification_request_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    12415 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/create_subscription.py
--rw-r--r--   0 root         (0) root         (0)    14937 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/email_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    11112 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     8023 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/id_selector_definition.py
--rw-r--r--   0 root         (0) root         (0)     9512 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/identifier_part_schema.py
--rw-r--r--   0 root         (0) root         (0)     6427 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/link.py
--rw-r--r--   0 root         (0) root         (0)     9541 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/lusid_problem_details.py
--rw-r--r--   0 root         (0) root         (0)    10706 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/lusid_validation_problem_details.py
--rw-r--r--   0 root         (0) root         (0)     5088 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/manual_event.py
--rw-r--r--   0 root         (0) root         (0)     7865 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/manual_event_body.py
--rw-r--r--   0 root         (0) root         (0)     6829 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/manual_event_header.py
--rw-r--r--   0 root         (0) root         (0)     4164 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/manual_event_request.py
--rw-r--r--   0 root         (0) root         (0)     7438 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/matching_pattern.py
--rw-r--r--   0 root         (0) root         (0)    15841 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/notification.py
--rw-r--r--   0 root         (0) root         (0)    37019 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/notification_notification_type.py
--rw-r--r--   0 root         (0) root         (0)     5156 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/notification_status.py
--rw-r--r--   0 root         (0) root         (0)     6100 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/resource_id.py
--rw-r--r--   0 root         (0) root         (0)     7770 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7518 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/resource_list_of_event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     7434 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/resource_list_of_notification.py
--rw-r--r--   0 root         (0) root         (0)     7434 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/resource_list_of_subscription.py
--rw-r--r--   0 root         (0) root         (0)     8014 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/sms_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    16642 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/subscription.py
--rw-r--r--   0 root         (0) root         (0)     8549 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/update_notification_request.py
--rw-r--r--   0 root         (0) root         (0)    11553 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/update_subscription.py
--rw-r--r--   0 root         (0) root         (0)    15805 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/webhook_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    13562 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:54:53.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/utilities/
--rw-r--r--   0 root         (0) root         (0)       64 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/utilities/config_keys.json
--rw-r--r--   0 root         (0) root         (0)      295 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/utilities/config_keys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 18:54:53.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification_sdk_preview.egg-info/
--rw-r--r--   0 root         (0) root         (0)      385 2023-06-19 18:54:53.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification_sdk_preview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2654 2023-06-19 18:54:53.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification_sdk_preview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 18:54:53.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification_sdk_preview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2023-06-19 18:54:53.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification_sdk_preview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-06-19 18:54:53.000000 lusid-notification-sdk-preview-0.1.748.post2/lusid_notification_sdk_preview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-19 18:54:53.000000 lusid-notification-sdk-preview-0.1.748.post2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2327 2023-06-19 18:54:23.000000 lusid-notification-sdk-preview-0.1.748.post2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 10:40:04.000000 lusid-notification-sdk-preview-0.1.748.post3/
+-rw-r--r--   0 root         (0) root         (0)       53 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      385 2023-06-21 10:40:04.000000 lusid-notification-sdk-preview-0.1.748.post3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7789 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 10:40:04.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/
+-rw-r--r--   0 root         (0) root         (0)     4201 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 10:40:04.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/api/
+-rw-r--r--   0 root         (0) root         (0)      442 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6851 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/api/application_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)    13990 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/api/event_types_api.py
+-rw-r--r--   0 root         (0) root         (0)     7824 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/api/manual_event_api.py
+-rw-r--r--   0 root         (0) root         (0)    52809 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/api/notifications_api.py
+-rw-r--r--   0 root         (0) root         (0)    47815 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/api/subscriptions_api.py
+-rw-r--r--   0 root         (0) root         (0)    27787 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    16601 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5101 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 10:40:04.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/
+-rw-r--r--   0 root         (0) root         (0)     2911 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7256 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/access_controlled_action.py
+-rw-r--r--   0 root         (0) root         (0)     9019 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7233 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/action_id.py
+-rw-r--r--   0 root         (0) root         (0)     9645 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/amazon_sqs_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)     7918 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/api_request_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    10781 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/create_notification_request.py
+-rw-r--r--   0 root         (0) root         (0)    12415 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/create_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    13639 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/email_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    11112 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     8023 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/id_selector_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9512 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/identifier_part_schema.py
+-rw-r--r--   0 root         (0) root         (0)     6427 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     9541 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/lusid_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)    10706 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/lusid_validation_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)     5088 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/manual_event.py
+-rw-r--r--   0 root         (0) root         (0)     7865 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/manual_event_body.py
+-rw-r--r--   0 root         (0) root         (0)     6829 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/manual_event_header.py
+-rw-r--r--   0 root         (0) root         (0)     4164 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/manual_event_request.py
+-rw-r--r--   0 root         (0) root         (0)     7438 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/matching_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    15923 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/notification.py
+-rw-r--r--   0 root         (0) root         (0)     5156 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/notification_status.py
+-rw-r--r--   0 root         (0) root         (0)    36418 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/notification_type.py
+-rw-r--r--   0 root         (0) root         (0)     6100 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/resource_id.py
+-rw-r--r--   0 root         (0) root         (0)     7770 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7518 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/resource_list_of_event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     7434 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/resource_list_of_notification.py
+-rw-r--r--   0 root         (0) root         (0)     7434 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/resource_list_of_subscription.py
+-rw-r--r--   0 root         (0) root         (0)     6724 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/sms_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    16642 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     8610 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/update_notification_request.py
+-rw-r--r--   0 root         (0) root         (0)    11553 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/update_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    14499 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/webhook_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    13562 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 10:40:04.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/utilities/
+-rw-r--r--   0 root         (0) root         (0)       64 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/utilities/config_keys.json
+-rw-r--r--   0 root         (0) root         (0)      295 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/utilities/config_keys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 10:40:04.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification_sdk_preview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      385 2023-06-21 10:40:04.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification_sdk_preview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2566 2023-06-21 10:40:04.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification_sdk_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 10:40:04.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification_sdk_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      116 2023-06-21 10:40:04.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification_sdk_preview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-21 10:40:04.000000 lusid-notification-sdk-preview-0.1.748.post3/lusid_notification_sdk_preview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 10:40:04.000000 lusid-notification-sdk-preview-0.1.748.post3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-06-21 10:39:37.000000 lusid-notification-sdk-preview-0.1.748.post3/setup.py
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/README.md` & `lusid-notification-sdk-preview-0.1.748.post3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-notification-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.748-2
-- Package version: 0.1.748-2
+- API version: 0.1.748-3
+- Package version: 0.1.748-3
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
@@ -49,28 +49,28 @@
 from __future__ import print_function
 
 import time
 import lusid_notification
 from lusid_notification.rest import ApiException
 from pprint import pprint
 
-# Defining the host is optional and defaults to https://www.lusid.com/notification
+# Defining the host is optional and defaults to http://localhost
 # See configuration.py for a list of all supported configuration parameters.
 configuration = lusid_notification.Configuration(
-    host = "https://www.lusid.com/notification"
+    host = "http://localhost"
 )
 
 # The client must configure the authentication and authorization parameters
 # in accordance with the API server security policy.
 # Examples for each auth method are provided below, use the example that
 # satisfies your auth use case.
 
 # Configure OAuth2 access token for authorization: oauth2
 configuration = lusid_notification.Configuration(
-    host = "https://www.lusid.com/notification"
+    host = "http://localhost"
 )
 configuration.access_token = 'YOUR_ACCESS_TOKEN'
 
 
 # Enter a context with an instance of the API client
 with lusid_notification.ApiClient(configuration) as api_client:
     # Create an instance of the API class
@@ -83,15 +83,15 @@
     except ApiException as e:
         print("Exception when calling ApplicationMetadataApi->list_access_controlled_resources: %s\n" % e)
     
 ```
 
 ## Documentation for API Endpoints
 
-All URIs are relative to *https://www.lusid.com/notification*
+All URIs are relative to *http://localhost*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *ApplicationMetadataApi* | [**list_access_controlled_resources**](docs/ApplicationMetadataApi.md#list_access_controlled_resources) | **GET** /api/metadata/access/resources | [EARLY ACCESS] ListAccessControlledResources: Get resources available for access control
 *EventTypesApi* | [**get_event_type**](docs/EventTypesApi.md#get_event_type) | **GET** /api/eventtypes/{eventType} | [EXPERIMENTAL] GetEventType: Gets the specified event type schema.
 *EventTypesApi* | [**list_event_types**](docs/EventTypesApi.md#list_event_types) | **GET** /api/eventtypes | [EXPERIMENTAL] ListEventTypes: Lists all of the available event types.
 *ManualEventApi* | [**trigger_manual_event**](docs/ManualEventApi.md#trigger_manual_event) | **POST** /api/manualevent | [EXPERIMENTAL] TriggerManualEvent: Trigger a manual event.
@@ -111,31 +111,30 @@
 
  - [AccessControlledAction](docs/AccessControlledAction.md)
  - [AccessControlledResource](docs/AccessControlledResource.md)
  - [ActionId](docs/ActionId.md)
  - [AmazonSqsNotificationType](docs/AmazonSqsNotificationType.md)
  - [ApiRequestNotificationType](docs/ApiRequestNotificationType.md)
  - [CreateNotificationRequest](docs/CreateNotificationRequest.md)
- - [CreateNotificationRequestNotificationType](docs/CreateNotificationRequestNotificationType.md)
  - [CreateSubscription](docs/CreateSubscription.md)
  - [EmailNotificationType](docs/EmailNotificationType.md)
  - [EventTypeSchema](docs/EventTypeSchema.md)
  - [IdSelectorDefinition](docs/IdSelectorDefinition.md)
  - [IdentifierPartSchema](docs/IdentifierPartSchema.md)
  - [Link](docs/Link.md)
  - [LusidProblemDetails](docs/LusidProblemDetails.md)
  - [LusidValidationProblemDetails](docs/LusidValidationProblemDetails.md)
  - [ManualEvent](docs/ManualEvent.md)
  - [ManualEventBody](docs/ManualEventBody.md)
  - [ManualEventHeader](docs/ManualEventHeader.md)
  - [ManualEventRequest](docs/ManualEventRequest.md)
  - [MatchingPattern](docs/MatchingPattern.md)
  - [Notification](docs/Notification.md)
- - [NotificationNotificationType](docs/NotificationNotificationType.md)
  - [NotificationStatus](docs/NotificationStatus.md)
+ - [NotificationType](docs/NotificationType.md)
  - [ResourceId](docs/ResourceId.md)
  - [ResourceListOfAccessControlledResource](docs/ResourceListOfAccessControlledResource.md)
  - [ResourceListOfEventTypeSchema](docs/ResourceListOfEventTypeSchema.md)
  - [ResourceListOfNotification](docs/ResourceListOfNotification.md)
  - [ResourceListOfSubscription](docs/ResourceListOfSubscription.md)
  - [SmsNotificationType](docs/SmsNotificationType.md)
  - [Subscription](docs/Subscription.md)
@@ -150,15 +149,15 @@
 
 Authentication schemes defined for the API:
 <a id="oauth2"></a>
 ### oauth2
 
 - **Type**: OAuth
 - **Flow**: implicit
-- **Authorization URL**: https://lusid.okta.com/oauth2/default/v1/authorize
+- **Authorization URL**: https://dummyurl.lusid.com/
 - **Scopes**: N/A
 
 
 ## Author
 
 info@finbourne.com
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/__init__.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.1.748-2"
+__version__ = "0.1.748-3"
 
 # import apis into sdk package
 from lusid_notification.api.application_metadata_api import ApplicationMetadataApi
 from lusid_notification.api.event_types_api import EventTypesApi
 from lusid_notification.api.manual_event_api import ManualEventApi
 from lusid_notification.api.notifications_api import NotificationsApi
 from lusid_notification.api.subscriptions_api import SubscriptionsApi
@@ -35,31 +35,30 @@
 # import models into sdk package
 from lusid_notification.models.access_controlled_action import AccessControlledAction
 from lusid_notification.models.access_controlled_resource import AccessControlledResource
 from lusid_notification.models.action_id import ActionId
 from lusid_notification.models.amazon_sqs_notification_type import AmazonSqsNotificationType
 from lusid_notification.models.api_request_notification_type import ApiRequestNotificationType
 from lusid_notification.models.create_notification_request import CreateNotificationRequest
-from lusid_notification.models.create_notification_request_notification_type import CreateNotificationRequestNotificationType
 from lusid_notification.models.create_subscription import CreateSubscription
 from lusid_notification.models.email_notification_type import EmailNotificationType
 from lusid_notification.models.event_type_schema import EventTypeSchema
 from lusid_notification.models.id_selector_definition import IdSelectorDefinition
 from lusid_notification.models.identifier_part_schema import IdentifierPartSchema
 from lusid_notification.models.link import Link
 from lusid_notification.models.lusid_problem_details import LusidProblemDetails
 from lusid_notification.models.lusid_validation_problem_details import LusidValidationProblemDetails
 from lusid_notification.models.manual_event import ManualEvent
 from lusid_notification.models.manual_event_body import ManualEventBody
 from lusid_notification.models.manual_event_header import ManualEventHeader
 from lusid_notification.models.manual_event_request import ManualEventRequest
 from lusid_notification.models.matching_pattern import MatchingPattern
 from lusid_notification.models.notification import Notification
-from lusid_notification.models.notification_notification_type import NotificationNotificationType
 from lusid_notification.models.notification_status import NotificationStatus
+from lusid_notification.models.notification_type import NotificationType
 from lusid_notification.models.resource_id import ResourceId
 from lusid_notification.models.resource_list_of_access_controlled_resource import ResourceListOfAccessControlledResource
 from lusid_notification.models.resource_list_of_event_type_schema import ResourceListOfEventTypeSchema
 from lusid_notification.models.resource_list_of_notification import ResourceListOfNotification
 from lusid_notification.models.resource_list_of_subscription import ResourceListOfSubscription
 from lusid_notification.models.sms_notification_type import SmsNotificationType
 from lusid_notification.models.subscription import Subscription
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/api/application_metadata_api.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/api/application_metadata_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -141,15 +141,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748-2'
+        header_params['X-LUSID-SDK-Version'] = '0.1.748-3'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfAccessControlledResource",
         }
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/api/event_types_api.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/api/event_types_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -160,15 +160,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748-2'
+        header_params['X-LUSID-SDK-Version'] = '0.1.748-3'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "EventTypeSchema",
             400: "LusidValidationProblemDetails",
@@ -292,15 +292,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748-2'
+        header_params['X-LUSID-SDK-Version'] = '0.1.748-3'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfEventTypeSchema",
             404: "str",
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/api/manual_event_api.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/api/manual_event_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -155,15 +155,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748-2'
+        header_params['X-LUSID-SDK-Version'] = '0.1.748-3'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "ManualEvent",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/api/notifications_api.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/api/notifications_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -195,15 +195,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748-2'
+        header_params['X-LUSID-SDK-Version'] = '0.1.748-3'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Notification",
             400: "LusidValidationProblemDetails",
@@ -375,15 +375,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748-2'
+        header_params['X-LUSID-SDK-Version'] = '0.1.748-3'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -552,15 +552,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748-2'
+        header_params['X-LUSID-SDK-Version'] = '0.1.748-3'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
@@ -722,15 +722,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748-2'
+        header_params['X-LUSID-SDK-Version'] = '0.1.748-3'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfNotification",
             400: "LusidValidationProblemDetails",
@@ -925,15 +925,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748-2'
+        header_params['X-LUSID-SDK-Version'] = '0.1.748-3'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/api/subscriptions_api.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/api/subscriptions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -157,15 +157,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748-2'
+        header_params['X-LUSID-SDK-Version'] = '0.1.748-3'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Subscription",
             400: "LusidValidationProblemDetails",
@@ -326,15 +326,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748-2'
+        header_params['X-LUSID-SDK-Version'] = '0.1.748-3'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -492,15 +492,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748-2'
+        header_params['X-LUSID-SDK-Version'] = '0.1.748-3'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Subscription",
             400: "LusidValidationProblemDetails",
@@ -680,15 +680,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748-2'
+        header_params['X-LUSID-SDK-Version'] = '0.1.748-3'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfSubscription",
             400: "LusidValidationProblemDetails",
@@ -863,15 +863,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748-2'
+        header_params['X-LUSID-SDK-Version'] = '0.1.748-3'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Subscription",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/api_client.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.1.748-2/python'
+        self.user_agent = 'OpenAPI-Generator/0.1.748-3/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/configuration.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -95,15 +95,15 @@
                  server_index=None, server_variables=None,
                  server_operation_index=None, server_operation_variables=None,
                  ssl_ca_cert=None,
                  tcp_keep_alive=False,
                  ):
         """Constructor
         """
-        self._base_path = "https://www.lusid.com/notification" if host is None else host
+        self._base_path = "http://localhost" if host is None else host
         """Default Base url
         """
         self.server_index = 0 if server_index is None and host is None else server_index
         self.server_operation_index = server_operation_index or {}
         """Default server index
         """
         self.server_variables = server_variables or {}
@@ -392,26 +392,26 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.748-2\n"\
-               "SDK Package Version: 0.1.748-2".\
+               "Version of the API: 0.1.748-3\n"\
+               "SDK Package Version: 0.1.748-3".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
         return [
             {
-                'url': "https://www.lusid.com/notification",
+                'url': "http://localhost",
                 'description': "No description provided",
             }
         ]
 
     def get_host_from_settings(self, index, variables=None, servers=None):
         """Gets host URL based on the index and variables
         :param index: array index of the host settings
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/exceptions.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/__init__.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,46 +2,45 @@
 
 # flake8: noqa
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 # import models into model package
 from lusid_notification.models.access_controlled_action import AccessControlledAction
 from lusid_notification.models.access_controlled_resource import AccessControlledResource
 from lusid_notification.models.action_id import ActionId
 from lusid_notification.models.amazon_sqs_notification_type import AmazonSqsNotificationType
 from lusid_notification.models.api_request_notification_type import ApiRequestNotificationType
 from lusid_notification.models.create_notification_request import CreateNotificationRequest
-from lusid_notification.models.create_notification_request_notification_type import CreateNotificationRequestNotificationType
 from lusid_notification.models.create_subscription import CreateSubscription
 from lusid_notification.models.email_notification_type import EmailNotificationType
 from lusid_notification.models.event_type_schema import EventTypeSchema
 from lusid_notification.models.id_selector_definition import IdSelectorDefinition
 from lusid_notification.models.identifier_part_schema import IdentifierPartSchema
 from lusid_notification.models.link import Link
 from lusid_notification.models.lusid_problem_details import LusidProblemDetails
 from lusid_notification.models.lusid_validation_problem_details import LusidValidationProblemDetails
 from lusid_notification.models.manual_event import ManualEvent
 from lusid_notification.models.manual_event_body import ManualEventBody
 from lusid_notification.models.manual_event_header import ManualEventHeader
 from lusid_notification.models.manual_event_request import ManualEventRequest
 from lusid_notification.models.matching_pattern import MatchingPattern
 from lusid_notification.models.notification import Notification
-from lusid_notification.models.notification_notification_type import NotificationNotificationType
 from lusid_notification.models.notification_status import NotificationStatus
+from lusid_notification.models.notification_type import NotificationType
 from lusid_notification.models.resource_id import ResourceId
 from lusid_notification.models.resource_list_of_access_controlled_resource import ResourceListOfAccessControlledResource
 from lusid_notification.models.resource_list_of_event_type_schema import ResourceListOfEventTypeSchema
 from lusid_notification.models.resource_list_of_notification import ResourceListOfNotification
 from lusid_notification.models.resource_list_of_subscription import ResourceListOfSubscription
 from lusid_notification.models.sms_notification_type import SmsNotificationType
 from lusid_notification.models.subscription import Subscription
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/access_controlled_action.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/access_controlled_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/access_controlled_resource.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/action_id.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/action_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/amazon_sqs_notification_type.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/amazon_sqs_notification_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -35,98 +35,63 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'type': 'str',
         'api_key_ref': 'str',
         'api_secret_ref': 'str',
         'body': 'str',
         'queue_url_ref': 'str'
     }
 
     attribute_map = {
-        'type': 'type',
         'api_key_ref': 'apiKeyRef',
         'api_secret_ref': 'apiSecretRef',
         'body': 'body',
         'queue_url_ref': 'queueUrlRef'
     }
 
     required_map = {
-        'type': 'required',
         'api_key_ref': 'required',
         'api_secret_ref': 'required',
         'body': 'required',
         'queue_url_ref': 'required'
     }
 
-    def __init__(self, type=None, api_key_ref=None, api_secret_ref=None, body=None, queue_url_ref=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, api_key_ref=None, api_secret_ref=None, body=None, queue_url_ref=None, local_vars_configuration=None):  # noqa: E501
         """AmazonSqsNotificationType - a model defined in OpenAPI"
         
-        :param type:  The type of delivery mechanism for this notification (required)
-        :type type: str
         :param api_key_ref:  Reference to API key from Configuration Store (required)
         :type api_key_ref: str
         :param api_secret_ref:  Reference to API secret from Configuration Store (required)
         :type api_secret_ref: str
         :param body:  The body of the Amazon Queue Message (required)
         :type body: str
         :param queue_url_ref:  Reference to queue url from Configuration Store (required)
         :type queue_url_ref: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._type = None
         self._api_key_ref = None
         self._api_secret_ref = None
         self._body = None
         self._queue_url_ref = None
         self.discriminator = None
 
-        self.type = type
         self.api_key_ref = api_key_ref
         self.api_secret_ref = api_secret_ref
         self.body = body
         self.queue_url_ref = queue_url_ref
 
     @property
-    def type(self):
-        """Gets the type of this AmazonSqsNotificationType.  # noqa: E501
-
-        The type of delivery mechanism for this notification  # noqa: E501
-
-        :return: The type of this AmazonSqsNotificationType.  # noqa: E501
-        :rtype: str
-        """
-        return self._type
-
-    @type.setter
-    def type(self, type):
-        """Sets the type of this AmazonSqsNotificationType.
-
-        The type of delivery mechanism for this notification  # noqa: E501
-
-        :param type: The type of this AmazonSqsNotificationType.  # noqa: E501
-        :type type: str
-        """
-        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
-            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                type is not None and len(type) < 1):
-            raise ValueError("Invalid value for `type`, length must be greater than or equal to `1`")  # noqa: E501
-
-        self._type = type
-
-    @property
     def api_key_ref(self):
         """Gets the api_key_ref of this AmazonSqsNotificationType.  # noqa: E501
 
         Reference to API key from Configuration Store  # noqa: E501
 
         :return: The api_key_ref of this AmazonSqsNotificationType.  # noqa: E501
         :rtype: str
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/api_request_notification_type.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/api_request_notification_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -35,91 +35,56 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'type': 'str',
         'http_method': 'str',
         'path_and_query': 'str',
         'content': 'object'
     }
 
     attribute_map = {
-        'type': 'type',
         'http_method': 'httpMethod',
         'path_and_query': 'pathAndQuery',
         'content': 'content'
     }
 
     required_map = {
-        'type': 'required',
         'http_method': 'required',
         'path_and_query': 'required',
         'content': 'optional'
     }
 
-    def __init__(self, type=None, http_method=None, path_and_query=None, content=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, http_method=None, path_and_query=None, content=None, local_vars_configuration=None):  # noqa: E501
         """ApiRequestNotificationType - a model defined in OpenAPI"
         
-        :param type:  The type of delivery mechanism for this notification (required)
-        :type type: str
         :param http_method:  The HTTP method such as GET, POST, etc. to use on the Api Request (required)
         :type http_method: str
         :param path_and_query:  The url to send the request to. (required)
         :type path_and_query: str
         :param content:  The content of the request
         :type content: object
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._type = None
         self._http_method = None
         self._path_and_query = None
         self._content = None
         self.discriminator = None
 
-        self.type = type
         self.http_method = http_method
         self.path_and_query = path_and_query
         self.content = content
 
     @property
-    def type(self):
-        """Gets the type of this ApiRequestNotificationType.  # noqa: E501
-
-        The type of delivery mechanism for this notification  # noqa: E501
-
-        :return: The type of this ApiRequestNotificationType.  # noqa: E501
-        :rtype: str
-        """
-        return self._type
-
-    @type.setter
-    def type(self, type):
-        """Sets the type of this ApiRequestNotificationType.
-
-        The type of delivery mechanism for this notification  # noqa: E501
-
-        :param type: The type of this ApiRequestNotificationType.  # noqa: E501
-        :type type: str
-        """
-        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
-            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                type is not None and len(type) < 1):
-            raise ValueError("Invalid value for `type`, length must be greater than or equal to `1`")  # noqa: E501
-
-        self._type = type
-
-    @property
     def http_method(self):
         """Gets the http_method of this ApiRequestNotificationType.  # noqa: E501
 
         The HTTP method such as GET, POST, etc. to use on the Api Request  # noqa: E501
 
         :return: The http_method of this ApiRequestNotificationType.  # noqa: E501
         :rtype: str
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/create_notification_request.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/create_notification_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -38,15 +38,15 @@
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
         'notification_id': 'str',
         'display_name': 'str',
         'description': 'str',
-        'notification_type': 'CreateNotificationRequestNotificationType'
+        'notification_type': 'NotificationType'
     }
 
     attribute_map = {
         'notification_id': 'notificationId',
         'display_name': 'displayName',
         'description': 'description',
         'notification_type': 'notificationType'
@@ -64,16 +64,16 @@
         
         :param notification_id:  The identifier of the notification. (required)
         :type notification_id: str
         :param display_name:  The name of the notification (required)
         :type display_name: str
         :param description:  The summary of the services provided by the notification
         :type description: str
-        :param notification_type:  (required)
-        :type notification_type: lusid_notification.CreateNotificationRequestNotificationType
+        :param notification_type:  The contents of the notification type. (required)
+        :type notification_type: lusid_notification.NotificationType
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._notification_id = None
@@ -187,27 +187,29 @@
 
         self._description = description
 
     @property
     def notification_type(self):
         """Gets the notification_type of this CreateNotificationRequest.  # noqa: E501
 
+        The contents of the notification type.  # noqa: E501
 
         :return: The notification_type of this CreateNotificationRequest.  # noqa: E501
-        :rtype: lusid_notification.CreateNotificationRequestNotificationType
+        :rtype: lusid_notification.NotificationType
         """
         return self._notification_type
 
     @notification_type.setter
     def notification_type(self, notification_type):
         """Sets the notification_type of this CreateNotificationRequest.
 
+        The contents of the notification type.  # noqa: E501
 
         :param notification_type: The notification_type of this CreateNotificationRequest.  # noqa: E501
-        :type notification_type: lusid_notification.CreateNotificationRequestNotificationType
+        :type notification_type: lusid_notification.NotificationType
         """
         if self.local_vars_configuration.client_side_validation and notification_type is None:  # noqa: E501
             raise ValueError("Invalid value for `notification_type`, must not be `None`")  # noqa: E501
 
         self._notification_type = notification_type
 
     def to_dict(self, serialize=False):
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/create_notification_request_notification_type.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/notification_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_notification.configuration import Configuration
 
 
-class CreateNotificationRequestNotificationType(object):
+class NotificationType(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -100,16 +100,19 @@
         'recipients': 'required',
         'url': 'required',
         'authentication_type': 'required',
         'authentication_configuration_item_paths': 'optional',
         'content_type': 'required'
     }
 
+    discriminator_value_class_map = {
+    }
+
     def __init__(self, type=None, api_key_ref=None, api_secret_ref=None, body=None, queue_url_ref=None, http_method=None, path_and_query=None, content=None, subject=None, plain_text_body=None, html_body=None, email_address_to=None, email_address_cc=None, email_address_bcc=None, recipients=None, url=None, authentication_type=None, authentication_configuration_item_paths=None, content_type=None, local_vars_configuration=None):  # noqa: E501
-        """CreateNotificationRequestNotificationType - a model defined in OpenAPI"
+        """NotificationType - a model defined in OpenAPI"
         
         :param type:  The type of delivery mechanism for this notification (required)
         :type type: str
         :param api_key_ref:  Reference to API key from Configuration Store (required)
         :type api_key_ref: str
         :param api_secret_ref:  Reference to API secret from Configuration Store (required)
         :type api_secret_ref: str
@@ -166,15 +169,15 @@
         self._email_address_cc = None
         self._email_address_bcc = None
         self._recipients = None
         self._url = None
         self._authentication_type = None
         self._authentication_configuration_item_paths = None
         self._content_type = None
-        self.discriminator = None
+        self.discriminator = 'type'
 
         self.type = type
         self.api_key_ref = api_key_ref
         self.api_secret_ref = api_secret_ref
         self.body = body
         self.queue_url_ref = queue_url_ref
         self.http_method = http_method
@@ -190,114 +193,114 @@
         self.url = url
         self.authentication_type = authentication_type
         self.authentication_configuration_item_paths = authentication_configuration_item_paths
         self.content_type = content_type
 
     @property
     def type(self):
-        """Gets the type of this CreateNotificationRequestNotificationType.  # noqa: E501
+        """Gets the type of this NotificationType.  # noqa: E501
 
         The type of delivery mechanism for this notification  # noqa: E501
 
-        :return: The type of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :return: The type of this NotificationType.  # noqa: E501
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
-        """Sets the type of this CreateNotificationRequestNotificationType.
+        """Sets the type of this NotificationType.
 
         The type of delivery mechanism for this notification  # noqa: E501
 
-        :param type: The type of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :param type: The type of this NotificationType.  # noqa: E501
         :type type: str
         """
         if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
             raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 type is not None and len(type) < 1):
             raise ValueError("Invalid value for `type`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._type = type
 
     @property
     def api_key_ref(self):
-        """Gets the api_key_ref of this CreateNotificationRequestNotificationType.  # noqa: E501
+        """Gets the api_key_ref of this NotificationType.  # noqa: E501
 
         Reference to API key from Configuration Store  # noqa: E501
 
-        :return: The api_key_ref of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :return: The api_key_ref of this NotificationType.  # noqa: E501
         :rtype: str
         """
         return self._api_key_ref
 
     @api_key_ref.setter
     def api_key_ref(self, api_key_ref):
-        """Sets the api_key_ref of this CreateNotificationRequestNotificationType.
+        """Sets the api_key_ref of this NotificationType.
 
         Reference to API key from Configuration Store  # noqa: E501
 
-        :param api_key_ref: The api_key_ref of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :param api_key_ref: The api_key_ref of this NotificationType.  # noqa: E501
         :type api_key_ref: str
         """
         if self.local_vars_configuration.client_side_validation and api_key_ref is None:  # noqa: E501
             raise ValueError("Invalid value for `api_key_ref`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 api_key_ref is not None and len(api_key_ref) < 1):
             raise ValueError("Invalid value for `api_key_ref`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._api_key_ref = api_key_ref
 
     @property
     def api_secret_ref(self):
-        """Gets the api_secret_ref of this CreateNotificationRequestNotificationType.  # noqa: E501
+        """Gets the api_secret_ref of this NotificationType.  # noqa: E501
 
         Reference to API secret from Configuration Store  # noqa: E501
 
-        :return: The api_secret_ref of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :return: The api_secret_ref of this NotificationType.  # noqa: E501
         :rtype: str
         """
         return self._api_secret_ref
 
     @api_secret_ref.setter
     def api_secret_ref(self, api_secret_ref):
-        """Sets the api_secret_ref of this CreateNotificationRequestNotificationType.
+        """Sets the api_secret_ref of this NotificationType.
 
         Reference to API secret from Configuration Store  # noqa: E501
 
-        :param api_secret_ref: The api_secret_ref of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :param api_secret_ref: The api_secret_ref of this NotificationType.  # noqa: E501
         :type api_secret_ref: str
         """
         if self.local_vars_configuration.client_side_validation and api_secret_ref is None:  # noqa: E501
             raise ValueError("Invalid value for `api_secret_ref`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 api_secret_ref is not None and len(api_secret_ref) < 1):
             raise ValueError("Invalid value for `api_secret_ref`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._api_secret_ref = api_secret_ref
 
     @property
     def body(self):
-        """Gets the body of this CreateNotificationRequestNotificationType.  # noqa: E501
+        """Gets the body of this NotificationType.  # noqa: E501
 
         The body of the SMS  # noqa: E501
 
-        :return: The body of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :return: The body of this NotificationType.  # noqa: E501
         :rtype: str
         """
         return self._body
 
     @body.setter
     def body(self, body):
-        """Sets the body of this CreateNotificationRequestNotificationType.
+        """Sets the body of this NotificationType.
 
         The body of the SMS  # noqa: E501
 
-        :param body: The body of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :param body: The body of this NotificationType.  # noqa: E501
         :type body: str
         """
         if self.local_vars_configuration.client_side_validation and body is None:  # noqa: E501
             raise ValueError("Invalid value for `body`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 body is not None and len(body) > 1024):
             raise ValueError("Invalid value for `body`, length must be less than or equal to `1024`")  # noqa: E501
@@ -308,86 +311,86 @@
                 body is not None and not re.search(r'^[\s\S]*$', body)):  # noqa: E501
             raise ValueError(r"Invalid value for `body`, must be a follow pattern or equal to `/^[\s\S]*$/`")  # noqa: E501
 
         self._body = body
 
     @property
     def queue_url_ref(self):
-        """Gets the queue_url_ref of this CreateNotificationRequestNotificationType.  # noqa: E501
+        """Gets the queue_url_ref of this NotificationType.  # noqa: E501
 
         Reference to queue url from Configuration Store  # noqa: E501
 
-        :return: The queue_url_ref of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :return: The queue_url_ref of this NotificationType.  # noqa: E501
         :rtype: str
         """
         return self._queue_url_ref
 
     @queue_url_ref.setter
     def queue_url_ref(self, queue_url_ref):
-        """Sets the queue_url_ref of this CreateNotificationRequestNotificationType.
+        """Sets the queue_url_ref of this NotificationType.
 
         Reference to queue url from Configuration Store  # noqa: E501
 
-        :param queue_url_ref: The queue_url_ref of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :param queue_url_ref: The queue_url_ref of this NotificationType.  # noqa: E501
         :type queue_url_ref: str
         """
         if self.local_vars_configuration.client_side_validation and queue_url_ref is None:  # noqa: E501
             raise ValueError("Invalid value for `queue_url_ref`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 queue_url_ref is not None and len(queue_url_ref) < 1):
             raise ValueError("Invalid value for `queue_url_ref`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._queue_url_ref = queue_url_ref
 
     @property
     def http_method(self):
-        """Gets the http_method of this CreateNotificationRequestNotificationType.  # noqa: E501
+        """Gets the http_method of this NotificationType.  # noqa: E501
 
         The HTTP method such as GET, POST, etc. to use on the request  # noqa: E501
 
-        :return: The http_method of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :return: The http_method of this NotificationType.  # noqa: E501
         :rtype: str
         """
         return self._http_method
 
     @http_method.setter
     def http_method(self, http_method):
-        """Sets the http_method of this CreateNotificationRequestNotificationType.
+        """Sets the http_method of this NotificationType.
 
         The HTTP method such as GET, POST, etc. to use on the request  # noqa: E501
 
-        :param http_method: The http_method of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :param http_method: The http_method of this NotificationType.  # noqa: E501
         :type http_method: str
         """
         if self.local_vars_configuration.client_side_validation and http_method is None:  # noqa: E501
             raise ValueError("Invalid value for `http_method`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 http_method is not None and len(http_method) < 1):
             raise ValueError("Invalid value for `http_method`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._http_method = http_method
 
     @property
     def path_and_query(self):
-        """Gets the path_and_query of this CreateNotificationRequestNotificationType.  # noqa: E501
+        """Gets the path_and_query of this NotificationType.  # noqa: E501
 
         The url to send the request to.  # noqa: E501
 
-        :return: The path_and_query of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :return: The path_and_query of this NotificationType.  # noqa: E501
         :rtype: str
         """
         return self._path_and_query
 
     @path_and_query.setter
     def path_and_query(self, path_and_query):
-        """Sets the path_and_query of this CreateNotificationRequestNotificationType.
+        """Sets the path_and_query of this NotificationType.
 
         The url to send the request to.  # noqa: E501
 
-        :param path_and_query: The path_and_query of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :param path_and_query: The path_and_query of this NotificationType.  # noqa: E501
         :type path_and_query: str
         """
         if self.local_vars_configuration.client_side_validation and path_and_query is None:  # noqa: E501
             raise ValueError("Invalid value for `path_and_query`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 path_and_query is not None and len(path_and_query) > 16384):
             raise ValueError("Invalid value for `path_and_query`, length must be less than or equal to `16384`")  # noqa: E501
@@ -398,53 +401,53 @@
                 path_and_query is not None and not re.search(r'^([A-Za-z0-9-._~:\/?#[\]@!$&\'()*+,;%=]|(\{\{([a-zA-Z0-9\s])*\}\}))*$', path_and_query)):  # noqa: E501
             raise ValueError(r"Invalid value for `path_and_query`, must be a follow pattern or equal to `/^([A-Za-z0-9-._~:\/?#[\]@!$&'()*+,;%=]|(\{\{([a-zA-Z0-9\s])*\}\}))*$/`")  # noqa: E501
 
         self._path_and_query = path_and_query
 
     @property
     def content(self):
-        """Gets the content of this CreateNotificationRequestNotificationType.  # noqa: E501
+        """Gets the content of this NotificationType.  # noqa: E501
 
         The content of the request  # noqa: E501
 
-        :return: The content of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :return: The content of this NotificationType.  # noqa: E501
         :rtype: object
         """
         return self._content
 
     @content.setter
     def content(self, content):
-        """Sets the content of this CreateNotificationRequestNotificationType.
+        """Sets the content of this NotificationType.
 
         The content of the request  # noqa: E501
 
-        :param content: The content of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :param content: The content of this NotificationType.  # noqa: E501
         :type content: object
         """
 
         self._content = content
 
     @property
     def subject(self):
-        """Gets the subject of this CreateNotificationRequestNotificationType.  # noqa: E501
+        """Gets the subject of this NotificationType.  # noqa: E501
 
         The subject of the email  # noqa: E501
 
-        :return: The subject of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :return: The subject of this NotificationType.  # noqa: E501
         :rtype: str
         """
         return self._subject
 
     @subject.setter
     def subject(self, subject):
-        """Sets the subject of this CreateNotificationRequestNotificationType.
+        """Sets the subject of this NotificationType.
 
         The subject of the email  # noqa: E501
 
-        :param subject: The subject of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :param subject: The subject of this NotificationType.  # noqa: E501
         :type subject: str
         """
         if self.local_vars_configuration.client_side_validation and subject is None:  # noqa: E501
             raise ValueError("Invalid value for `subject`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 subject is not None and len(subject) > 1024):
             raise ValueError("Invalid value for `subject`, length must be less than or equal to `1024`")  # noqa: E501
@@ -455,30 +458,30 @@
                 subject is not None and not re.search(r'^[\s\S]*$', subject)):  # noqa: E501
             raise ValueError(r"Invalid value for `subject`, must be a follow pattern or equal to `/^[\s\S]*$/`")  # noqa: E501
 
         self._subject = subject
 
     @property
     def plain_text_body(self):
-        """Gets the plain_text_body of this CreateNotificationRequestNotificationType.  # noqa: E501
+        """Gets the plain_text_body of this NotificationType.  # noqa: E501
 
         The plain text body of the email  # noqa: E501
 
-        :return: The plain_text_body of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :return: The plain_text_body of this NotificationType.  # noqa: E501
         :rtype: str
         """
         return self._plain_text_body
 
     @plain_text_body.setter
     def plain_text_body(self, plain_text_body):
-        """Sets the plain_text_body of this CreateNotificationRequestNotificationType.
+        """Sets the plain_text_body of this NotificationType.
 
         The plain text body of the email  # noqa: E501
 
-        :param plain_text_body: The plain_text_body of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :param plain_text_body: The plain_text_body of this NotificationType.  # noqa: E501
         :type plain_text_body: str
         """
         if self.local_vars_configuration.client_side_validation and plain_text_body is None:  # noqa: E501
             raise ValueError("Invalid value for `plain_text_body`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 plain_text_body is not None and len(plain_text_body) > 2147483647):
             raise ValueError("Invalid value for `plain_text_body`, length must be less than or equal to `2147483647`")  # noqa: E501
@@ -489,56 +492,56 @@
                 plain_text_body is not None and not re.search(r'^[\s\S]*$', plain_text_body)):  # noqa: E501
             raise ValueError(r"Invalid value for `plain_text_body`, must be a follow pattern or equal to `/^[\s\S]*$/`")  # noqa: E501
 
         self._plain_text_body = plain_text_body
 
     @property
     def html_body(self):
-        """Gets the html_body of this CreateNotificationRequestNotificationType.  # noqa: E501
+        """Gets the html_body of this NotificationType.  # noqa: E501
 
         The HTML body of the email (if any)  # noqa: E501
 
-        :return: The html_body of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :return: The html_body of this NotificationType.  # noqa: E501
         :rtype: str
         """
         return self._html_body
 
     @html_body.setter
     def html_body(self, html_body):
-        """Sets the html_body of this CreateNotificationRequestNotificationType.
+        """Sets the html_body of this NotificationType.
 
         The HTML body of the email (if any)  # noqa: E501
 
-        :param html_body: The html_body of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :param html_body: The html_body of this NotificationType.  # noqa: E501
         :type html_body: str
         """
         if (self.local_vars_configuration.client_side_validation and
                 html_body is not None and not re.search(r'^[\s\S]*$', html_body)):  # noqa: E501
             raise ValueError(r"Invalid value for `html_body`, must be a follow pattern or equal to `/^[\s\S]*$/`")  # noqa: E501
 
         self._html_body = html_body
 
     @property
     def email_address_to(self):
-        """Gets the email_address_to of this CreateNotificationRequestNotificationType.  # noqa: E501
+        """Gets the email_address_to of this NotificationType.  # noqa: E501
 
         'To' recipients of the email  # noqa: E501
 
-        :return: The email_address_to of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :return: The email_address_to of this NotificationType.  # noqa: E501
         :rtype: list[str]
         """
         return self._email_address_to
 
     @email_address_to.setter
     def email_address_to(self, email_address_to):
-        """Sets the email_address_to of this CreateNotificationRequestNotificationType.
+        """Sets the email_address_to of this NotificationType.
 
         'To' recipients of the email  # noqa: E501
 
-        :param email_address_to: The email_address_to of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :param email_address_to: The email_address_to of this NotificationType.  # noqa: E501
         :type email_address_to: list[str]
         """
         if self.local_vars_configuration.client_side_validation and email_address_to is None:  # noqa: E501
             raise ValueError("Invalid value for `email_address_to`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 email_address_to is not None and len(email_address_to) > 10):
             raise ValueError("Invalid value for `email_address_to`, number of items must be less than or equal to `10`")  # noqa: E501
@@ -546,88 +549,88 @@
                 email_address_to is not None and len(email_address_to) < 1):
             raise ValueError("Invalid value for `email_address_to`, number of items must be greater than or equal to `1`")  # noqa: E501
 
         self._email_address_to = email_address_to
 
     @property
     def email_address_cc(self):
-        """Gets the email_address_cc of this CreateNotificationRequestNotificationType.  # noqa: E501
+        """Gets the email_address_cc of this NotificationType.  # noqa: E501
 
         'Cc' recipients of the email  # noqa: E501
 
-        :return: The email_address_cc of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :return: The email_address_cc of this NotificationType.  # noqa: E501
         :rtype: list[str]
         """
         return self._email_address_cc
 
     @email_address_cc.setter
     def email_address_cc(self, email_address_cc):
-        """Sets the email_address_cc of this CreateNotificationRequestNotificationType.
+        """Sets the email_address_cc of this NotificationType.
 
         'Cc' recipients of the email  # noqa: E501
 
-        :param email_address_cc: The email_address_cc of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :param email_address_cc: The email_address_cc of this NotificationType.  # noqa: E501
         :type email_address_cc: list[str]
         """
         if (self.local_vars_configuration.client_side_validation and
                 email_address_cc is not None and len(email_address_cc) > 10):
             raise ValueError("Invalid value for `email_address_cc`, number of items must be less than or equal to `10`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 email_address_cc is not None and len(email_address_cc) < 0):
             raise ValueError("Invalid value for `email_address_cc`, number of items must be greater than or equal to `0`")  # noqa: E501
 
         self._email_address_cc = email_address_cc
 
     @property
     def email_address_bcc(self):
-        """Gets the email_address_bcc of this CreateNotificationRequestNotificationType.  # noqa: E501
+        """Gets the email_address_bcc of this NotificationType.  # noqa: E501
 
         'Bcc' recipients of the email  # noqa: E501
 
-        :return: The email_address_bcc of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :return: The email_address_bcc of this NotificationType.  # noqa: E501
         :rtype: list[str]
         """
         return self._email_address_bcc
 
     @email_address_bcc.setter
     def email_address_bcc(self, email_address_bcc):
-        """Sets the email_address_bcc of this CreateNotificationRequestNotificationType.
+        """Sets the email_address_bcc of this NotificationType.
 
         'Bcc' recipients of the email  # noqa: E501
 
-        :param email_address_bcc: The email_address_bcc of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :param email_address_bcc: The email_address_bcc of this NotificationType.  # noqa: E501
         :type email_address_bcc: list[str]
         """
         if (self.local_vars_configuration.client_side_validation and
                 email_address_bcc is not None and len(email_address_bcc) > 10):
             raise ValueError("Invalid value for `email_address_bcc`, number of items must be less than or equal to `10`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 email_address_bcc is not None and len(email_address_bcc) < 0):
             raise ValueError("Invalid value for `email_address_bcc`, number of items must be greater than or equal to `0`")  # noqa: E501
 
         self._email_address_bcc = email_address_bcc
 
     @property
     def recipients(self):
-        """Gets the recipients of this CreateNotificationRequestNotificationType.  # noqa: E501
+        """Gets the recipients of this NotificationType.  # noqa: E501
 
         The phone numbers to which the SMS will be sent to (E.164 format)  # noqa: E501
 
-        :return: The recipients of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :return: The recipients of this NotificationType.  # noqa: E501
         :rtype: list[str]
         """
         return self._recipients
 
     @recipients.setter
     def recipients(self, recipients):
-        """Sets the recipients of this CreateNotificationRequestNotificationType.
+        """Sets the recipients of this NotificationType.
 
         The phone numbers to which the SMS will be sent to (E.164 format)  # noqa: E501
 
-        :param recipients: The recipients of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :param recipients: The recipients of this NotificationType.  # noqa: E501
         :type recipients: list[str]
         """
         if self.local_vars_configuration.client_side_validation and recipients is None:  # noqa: E501
             raise ValueError("Invalid value for `recipients`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 recipients is not None and len(recipients) > 10):
             raise ValueError("Invalid value for `recipients`, number of items must be less than or equal to `10`")  # noqa: E501
@@ -635,30 +638,30 @@
                 recipients is not None and len(recipients) < 1):
             raise ValueError("Invalid value for `recipients`, number of items must be greater than or equal to `1`")  # noqa: E501
 
         self._recipients = recipients
 
     @property
     def url(self):
-        """Gets the url of this CreateNotificationRequestNotificationType.  # noqa: E501
+        """Gets the url of this NotificationType.  # noqa: E501
 
         The URL to send the request to  # noqa: E501
 
-        :return: The url of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :return: The url of this NotificationType.  # noqa: E501
         :rtype: str
         """
         return self._url
 
     @url.setter
     def url(self, url):
-        """Sets the url of this CreateNotificationRequestNotificationType.
+        """Sets the url of this NotificationType.
 
         The URL to send the request to  # noqa: E501
 
-        :param url: The url of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :param url: The url of this NotificationType.  # noqa: E501
         :type url: str
         """
         if self.local_vars_configuration.client_side_validation and url is None:  # noqa: E501
             raise ValueError("Invalid value for `url`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 url is not None and len(url) > 16384):
             raise ValueError("Invalid value for `url`, length must be less than or equal to `16384`")  # noqa: E501
@@ -669,91 +672,97 @@
                 url is not None and not re.search(r'^([A-Za-z0-9-._~:\/?#[\]@!$&\'()*+,;%=]|(\{\{([a-zA-Z0-9\s])*\}\}))*$', url)):  # noqa: E501
             raise ValueError(r"Invalid value for `url`, must be a follow pattern or equal to `/^([A-Za-z0-9-._~:\/?#[\]@!$&'()*+,;%=]|(\{\{([a-zA-Z0-9\s])*\}\}))*$/`")  # noqa: E501
 
         self._url = url
 
     @property
     def authentication_type(self):
-        """Gets the authentication_type of this CreateNotificationRequestNotificationType.  # noqa: E501
+        """Gets the authentication_type of this NotificationType.  # noqa: E501
 
         The type of authentication to use on the request  # noqa: E501
 
-        :return: The authentication_type of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :return: The authentication_type of this NotificationType.  # noqa: E501
         :rtype: str
         """
         return self._authentication_type
 
     @authentication_type.setter
     def authentication_type(self, authentication_type):
-        """Sets the authentication_type of this CreateNotificationRequestNotificationType.
+        """Sets the authentication_type of this NotificationType.
 
         The type of authentication to use on the request  # noqa: E501
 
-        :param authentication_type: The authentication_type of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :param authentication_type: The authentication_type of this NotificationType.  # noqa: E501
         :type authentication_type: str
         """
         if self.local_vars_configuration.client_side_validation and authentication_type is None:  # noqa: E501
             raise ValueError("Invalid value for `authentication_type`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 authentication_type is not None and len(authentication_type) < 1):
             raise ValueError("Invalid value for `authentication_type`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._authentication_type = authentication_type
 
     @property
     def authentication_configuration_item_paths(self):
-        """Gets the authentication_configuration_item_paths of this CreateNotificationRequestNotificationType.  # noqa: E501
+        """Gets the authentication_configuration_item_paths of this NotificationType.  # noqa: E501
 
         The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }  # noqa: E501
 
-        :return: The authentication_configuration_item_paths of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :return: The authentication_configuration_item_paths of this NotificationType.  # noqa: E501
         :rtype: dict[str, str]
         """
         return self._authentication_configuration_item_paths
 
     @authentication_configuration_item_paths.setter
     def authentication_configuration_item_paths(self, authentication_configuration_item_paths):
-        """Sets the authentication_configuration_item_paths of this CreateNotificationRequestNotificationType.
+        """Sets the authentication_configuration_item_paths of this NotificationType.
 
         The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }  # noqa: E501
 
-        :param authentication_configuration_item_paths: The authentication_configuration_item_paths of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :param authentication_configuration_item_paths: The authentication_configuration_item_paths of this NotificationType.  # noqa: E501
         :type authentication_configuration_item_paths: dict[str, str]
         """
 
         self._authentication_configuration_item_paths = authentication_configuration_item_paths
 
     @property
     def content_type(self):
-        """Gets the content_type of this CreateNotificationRequestNotificationType.  # noqa: E501
+        """Gets the content_type of this NotificationType.  # noqa: E501
 
         The type of the content e.g. Json  # noqa: E501
 
-        :return: The content_type of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :return: The content_type of this NotificationType.  # noqa: E501
         :rtype: str
         """
         return self._content_type
 
     @content_type.setter
     def content_type(self, content_type):
-        """Sets the content_type of this CreateNotificationRequestNotificationType.
+        """Sets the content_type of this NotificationType.
 
         The type of the content e.g. Json  # noqa: E501
 
-        :param content_type: The content_type of this CreateNotificationRequestNotificationType.  # noqa: E501
+        :param content_type: The content_type of this NotificationType.  # noqa: E501
         :type content_type: str
         """
         if self.local_vars_configuration.client_side_validation and content_type is None:  # noqa: E501
             raise ValueError("Invalid value for `content_type`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 content_type is not None and len(content_type) < 1):
             raise ValueError("Invalid value for `content_type`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._content_type = content_type
 
+    def get_real_child_model(self, data):
+        """Returns the real base class specified by the discriminator"""
+        discriminator_key = self.attribute_map[self.discriminator]
+        discriminator_value = data[discriminator_key]
+        return self.discriminator_value_class_map.get(discriminator_value)
+
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = getfullargspec(x.to_dict).args
@@ -788,18 +797,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, CreateNotificationRequestNotificationType):
+        if not isinstance(other, NotificationType):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, CreateNotificationRequestNotificationType):
+        if not isinstance(other, NotificationType):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/create_subscription.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/create_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/email_notification_type.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/email_notification_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -35,48 +35,43 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'type': 'str',
         'subject': 'str',
         'plain_text_body': 'str',
         'html_body': 'str',
         'email_address_to': 'list[str]',
         'email_address_cc': 'list[str]',
         'email_address_bcc': 'list[str]'
     }
 
     attribute_map = {
-        'type': 'type',
         'subject': 'subject',
         'plain_text_body': 'plainTextBody',
         'html_body': 'htmlBody',
         'email_address_to': 'emailAddressTo',
         'email_address_cc': 'emailAddressCc',
         'email_address_bcc': 'emailAddressBcc'
     }
 
     required_map = {
-        'type': 'required',
         'subject': 'required',
         'plain_text_body': 'required',
         'html_body': 'optional',
         'email_address_to': 'required',
         'email_address_cc': 'optional',
         'email_address_bcc': 'optional'
     }
 
-    def __init__(self, type=None, subject=None, plain_text_body=None, html_body=None, email_address_to=None, email_address_cc=None, email_address_bcc=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, subject=None, plain_text_body=None, html_body=None, email_address_to=None, email_address_cc=None, email_address_bcc=None, local_vars_configuration=None):  # noqa: E501
         """EmailNotificationType - a model defined in OpenAPI"
         
-        :param type:  The type of delivery mechanism for this notification (required)
-        :type type: str
         :param subject:  The subject of the email (required)
         :type subject: str
         :param plain_text_body:  The plain text body of the email (required)
         :type plain_text_body: str
         :param html_body:  The HTML body of the email (if any)
         :type html_body: str
         :param email_address_to:  'To' recipients of the email (required)
@@ -87,60 +82,30 @@
         :type email_address_bcc: list[str]
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._type = None
         self._subject = None
         self._plain_text_body = None
         self._html_body = None
         self._email_address_to = None
         self._email_address_cc = None
         self._email_address_bcc = None
         self.discriminator = None
 
-        self.type = type
         self.subject = subject
         self.plain_text_body = plain_text_body
         self.html_body = html_body
         self.email_address_to = email_address_to
         self.email_address_cc = email_address_cc
         self.email_address_bcc = email_address_bcc
 
     @property
-    def type(self):
-        """Gets the type of this EmailNotificationType.  # noqa: E501
-
-        The type of delivery mechanism for this notification  # noqa: E501
-
-        :return: The type of this EmailNotificationType.  # noqa: E501
-        :rtype: str
-        """
-        return self._type
-
-    @type.setter
-    def type(self, type):
-        """Sets the type of this EmailNotificationType.
-
-        The type of delivery mechanism for this notification  # noqa: E501
-
-        :param type: The type of this EmailNotificationType.  # noqa: E501
-        :type type: str
-        """
-        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
-            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                type is not None and len(type) < 1):
-            raise ValueError("Invalid value for `type`, length must be greater than or equal to `1`")  # noqa: E501
-
-        self._type = type
-
-    @property
     def subject(self):
         """Gets the subject of this EmailNotificationType.  # noqa: E501
 
         The subject of the email  # noqa: E501
 
         :return: The subject of this EmailNotificationType.  # noqa: E501
         :rtype: str
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/event_type_schema.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/event_type_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/id_selector_definition.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/id_selector_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/identifier_part_schema.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/identifier_part_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/link.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/lusid_problem_details.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/lusid_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/lusid_validation_problem_details.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/lusid_validation_problem_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/manual_event.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/manual_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/manual_event_body.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/manual_event_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/manual_event_header.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/manual_event_header.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/manual_event_request.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/manual_event_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/matching_pattern.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/matching_pattern.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/notification.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/notification.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -38,15 +38,15 @@
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
         'notification_id': 'str',
         'display_name': 'str',
         'description': 'str',
-        'notification_type': 'NotificationNotificationType',
+        'notification_type': 'Object',
         'created_at': 'datetime',
         'user_id_created': 'str',
         'modified_at': 'datetime',
         'user_id_modified': 'str',
         'href': 'str'
     }
 
@@ -79,16 +79,16 @@
         
         :param notification_id:  The identifier of the notification (required)
         :type notification_id: str
         :param display_name:  The name of the notification
         :type display_name: str
         :param description:  The summary of the services provided by the notification
         :type description: str
-        :param notification_type:  (required)
-        :type notification_type: lusid_notification.NotificationNotificationType
+        :param notification_type:  The type and contents of the notification (required)
+        :type notification_type: lusid_notification.Object
         :param created_at:  The time at which the subscription was made (required)
         :type created_at: datetime
         :param user_id_created:  The user who made the subscription (required)
         :type user_id_created: str
         :param modified_at:  The time at which the subscription was last modified (required)
         :type modified_at: datetime
         :param user_id_modified:  The user who last modified the subscription (required)
@@ -214,27 +214,29 @@
 
         self._description = description
 
     @property
     def notification_type(self):
         """Gets the notification_type of this Notification.  # noqa: E501
 
+        The type and contents of the notification  # noqa: E501
 
         :return: The notification_type of this Notification.  # noqa: E501
-        :rtype: lusid_notification.NotificationNotificationType
+        :rtype: lusid_notification.Object
         """
         return self._notification_type
 
     @notification_type.setter
     def notification_type(self, notification_type):
         """Sets the notification_type of this Notification.
 
+        The type and contents of the notification  # noqa: E501
 
         :param notification_type: The notification_type of this Notification.  # noqa: E501
-        :type notification_type: lusid_notification.NotificationNotificationType
+        :type notification_type: lusid_notification.Object
         """
         if self.local_vars_configuration.client_side_validation and notification_type is None:  # noqa: E501
             raise ValueError("Invalid value for `notification_type`, must not be `None`")  # noqa: E501
 
         self._notification_type = notification_type
 
     @property
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/notification_status.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/notification_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/resource_id.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/resource_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/resource_list_of_access_controlled_resource.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/resource_list_of_access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/resource_list_of_event_type_schema.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/resource_list_of_event_type_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/resource_list_of_notification.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/resource_list_of_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/resource_list_of_subscription.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/resource_list_of_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/sms_notification_type.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/sms_notification_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -35,84 +35,49 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'type': 'str',
         'body': 'str',
         'recipients': 'list[str]'
     }
 
     attribute_map = {
-        'type': 'type',
         'body': 'body',
         'recipients': 'recipients'
     }
 
     required_map = {
-        'type': 'required',
         'body': 'required',
         'recipients': 'required'
     }
 
-    def __init__(self, type=None, body=None, recipients=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, body=None, recipients=None, local_vars_configuration=None):  # noqa: E501
         """SmsNotificationType - a model defined in OpenAPI"
         
-        :param type:  The type of delivery mechanism for this notification (required)
-        :type type: str
         :param body:  The body of the SMS (required)
         :type body: str
         :param recipients:  The phone numbers to which the SMS will be sent to (E.164 format) (required)
         :type recipients: list[str]
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._type = None
         self._body = None
         self._recipients = None
         self.discriminator = None
 
-        self.type = type
         self.body = body
         self.recipients = recipients
 
     @property
-    def type(self):
-        """Gets the type of this SmsNotificationType.  # noqa: E501
-
-        The type of delivery mechanism for this notification  # noqa: E501
-
-        :return: The type of this SmsNotificationType.  # noqa: E501
-        :rtype: str
-        """
-        return self._type
-
-    @type.setter
-    def type(self, type):
-        """Sets the type of this SmsNotificationType.
-
-        The type of delivery mechanism for this notification  # noqa: E501
-
-        :param type: The type of this SmsNotificationType.  # noqa: E501
-        :type type: str
-        """
-        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
-            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                type is not None and len(type) < 1):
-            raise ValueError("Invalid value for `type`, length must be greater than or equal to `1`")  # noqa: E501
-
-        self._type = type
-
-    @property
     def body(self):
         """Gets the body of this SmsNotificationType.  # noqa: E501
 
         The body of the SMS  # noqa: E501
 
         :return: The body of this SmsNotificationType.  # noqa: E501
         :rtype: str
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/subscription.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/update_notification_request.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/update_notification_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -37,15 +37,15 @@
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
         'display_name': 'str',
         'description': 'str',
-        'notification_type': 'CreateNotificationRequestNotificationType'
+        'notification_type': 'NotificationType'
     }
 
     attribute_map = {
         'display_name': 'displayName',
         'description': 'description',
         'notification_type': 'notificationType'
     }
@@ -59,16 +59,16 @@
     def __init__(self, display_name=None, description=None, notification_type=None, local_vars_configuration=None):  # noqa: E501
         """UpdateNotificationRequest - a model defined in OpenAPI"
         
         :param display_name:  The name of the notification (required)
         :type display_name: str
         :param description:  The summary of the services provided by the notification
         :type description: str
-        :param notification_type:  (required)
-        :type notification_type: lusid_notification.CreateNotificationRequestNotificationType
+        :param notification_type:  The contents of the notification type. (required)
+        :type notification_type: lusid_notification.NotificationType
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._display_name = None
@@ -146,27 +146,29 @@
 
         self._description = description
 
     @property
     def notification_type(self):
         """Gets the notification_type of this UpdateNotificationRequest.  # noqa: E501
 
+        The contents of the notification type.  # noqa: E501
 
         :return: The notification_type of this UpdateNotificationRequest.  # noqa: E501
-        :rtype: lusid_notification.CreateNotificationRequestNotificationType
+        :rtype: lusid_notification.NotificationType
         """
         return self._notification_type
 
     @notification_type.setter
     def notification_type(self, notification_type):
         """Sets the notification_type of this UpdateNotificationRequest.
 
+        The contents of the notification type.  # noqa: E501
 
         :param notification_type: The notification_type of this UpdateNotificationRequest.  # noqa: E501
-        :type notification_type: lusid_notification.CreateNotificationRequestNotificationType
+        :type notification_type: lusid_notification.NotificationType
         """
         if self.local_vars_configuration.client_side_validation and notification_type is None:  # noqa: E501
             raise ValueError("Invalid value for `notification_type`, must not be `None`")  # noqa: E501
 
         self._notification_type = notification_type
 
     def to_dict(self, serialize=False):
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/update_subscription.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/update_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/models/webhook_notification_type.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/models/webhook_notification_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -35,48 +35,43 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'type': 'str',
         'http_method': 'str',
         'url': 'str',
         'authentication_type': 'str',
         'authentication_configuration_item_paths': 'dict[str, str]',
         'content_type': 'str',
         'content': 'object'
     }
 
     attribute_map = {
-        'type': 'type',
         'http_method': 'httpMethod',
         'url': 'url',
         'authentication_type': 'authenticationType',
         'authentication_configuration_item_paths': 'authenticationConfigurationItemPaths',
         'content_type': 'contentType',
         'content': 'content'
     }
 
     required_map = {
-        'type': 'required',
         'http_method': 'required',
         'url': 'required',
         'authentication_type': 'required',
         'authentication_configuration_item_paths': 'optional',
         'content_type': 'required',
         'content': 'optional'
     }
 
-    def __init__(self, type=None, http_method=None, url=None, authentication_type=None, authentication_configuration_item_paths=None, content_type=None, content=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, http_method=None, url=None, authentication_type=None, authentication_configuration_item_paths=None, content_type=None, content=None, local_vars_configuration=None):  # noqa: E501
         """WebhookNotificationType - a model defined in OpenAPI"
         
-        :param type:  The type of delivery mechanism for this notification (required)
-        :type type: str
         :param http_method:  The HTTP method such as GET, POST, etc. to use on the request (required)
         :type http_method: str
         :param url:  The URL to send the request to (required)
         :type url: str
         :param authentication_type:  The type of authentication to use on the request (required)
         :type authentication_type: str
         :param authentication_configuration_item_paths:  The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }
@@ -87,60 +82,30 @@
         :type content: object
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._type = None
         self._http_method = None
         self._url = None
         self._authentication_type = None
         self._authentication_configuration_item_paths = None
         self._content_type = None
         self._content = None
         self.discriminator = None
 
-        self.type = type
         self.http_method = http_method
         self.url = url
         self.authentication_type = authentication_type
         self.authentication_configuration_item_paths = authentication_configuration_item_paths
         self.content_type = content_type
         self.content = content
 
     @property
-    def type(self):
-        """Gets the type of this WebhookNotificationType.  # noqa: E501
-
-        The type of delivery mechanism for this notification  # noqa: E501
-
-        :return: The type of this WebhookNotificationType.  # noqa: E501
-        :rtype: str
-        """
-        return self._type
-
-    @type.setter
-    def type(self, type):
-        """Sets the type of this WebhookNotificationType.
-
-        The type of delivery mechanism for this notification  # noqa: E501
-
-        :param type: The type of this WebhookNotificationType.  # noqa: E501
-        :type type: str
-        """
-        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
-            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                type is not None and len(type) < 1):
-            raise ValueError("Invalid value for `type`, length must be greater than or equal to `1`")  # noqa: E501
-
-        self._type = type
-
-    @property
     def http_method(self):
         """Gets the http_method of this WebhookNotificationType.  # noqa: E501
 
         The HTTP method such as GET, POST, etc. to use on the request  # noqa: E501
 
         :return: The http_method of this WebhookNotificationType.  # noqa: E501
         :rtype: str
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/rest.py` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-2
+    The version of the OpenAPI document: 0.1.748-3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification/utilities/config_keys.json` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification/utilities/config_keys.json`

 * *Files identical despite different names*

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/lusid_notification_sdk_preview.egg-info/SOURCES.txt` & `lusid-notification-sdk-preview-0.1.748.post3/lusid_notification_sdk_preview.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,31 +16,30 @@
 lusid_notification/models/__init__.py
 lusid_notification/models/access_controlled_action.py
 lusid_notification/models/access_controlled_resource.py
 lusid_notification/models/action_id.py
 lusid_notification/models/amazon_sqs_notification_type.py
 lusid_notification/models/api_request_notification_type.py
 lusid_notification/models/create_notification_request.py
-lusid_notification/models/create_notification_request_notification_type.py
 lusid_notification/models/create_subscription.py
 lusid_notification/models/email_notification_type.py
 lusid_notification/models/event_type_schema.py
 lusid_notification/models/id_selector_definition.py
 lusid_notification/models/identifier_part_schema.py
 lusid_notification/models/link.py
 lusid_notification/models/lusid_problem_details.py
 lusid_notification/models/lusid_validation_problem_details.py
 lusid_notification/models/manual_event.py
 lusid_notification/models/manual_event_body.py
 lusid_notification/models/manual_event_header.py
 lusid_notification/models/manual_event_request.py
 lusid_notification/models/matching_pattern.py
 lusid_notification/models/notification.py
-lusid_notification/models/notification_notification_type.py
 lusid_notification/models/notification_status.py
+lusid_notification/models/notification_type.py
 lusid_notification/models/resource_id.py
 lusid_notification/models/resource_list_of_access_controlled_resource.py
 lusid_notification/models/resource_list_of_event_type_schema.py
 lusid_notification/models/resource_list_of_notification.py
 lusid_notification/models/resource_list_of_subscription.py
 lusid_notification/models/sms_notification_type.py
 lusid_notification/models/subscription.py
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post2/setup.py` & `lusid-notification-sdk-preview-0.1.748.post3/setup.py`

 * *Files identical despite different names*

