# Comparing `tmp/django_twined-0.4.3.tar.gz` & `tmp/django_twined-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_twined-0.4.3.tar", max compression
+gzip compressed data, was "django_twined-0.4.4.tar", max compression
```

## Comparing `django_twined-0.4.3.tar` & `django_twined-0.4.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     1088 2023-06-13 08:00:29.727306 django_twined-0.4.3/LICENSE
--rw-r--r--   0        0        0     1463 2023-06-13 08:00:29.727306 django_twined-0.4.3/README.md
--rw-r--r--   0        0        0       64 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/__init__.py
--rw-r--r--   0        0        0      257 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/admin/__init__.py
--rw-r--r--   0        0        0     6781 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/admin/admin.py
--rw-r--r--   0        0        0      402 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/admin/fieldsets.py
--rw-r--r--   0        0        0      881 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/admin/mixins.py
--rw-r--r--   0        0        0      682 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/admin/proxy.py
--rw-r--r--   0        0        0      496 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/apps.py
--rw-r--r--   0        0        0      104 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/consumers/__init__.py
--rw-r--r--   0        0        0     3765 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/consumers/analysis.py
--rw-r--r--   0        0        0     1001 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/consumers/analysis_log.py
--rw-r--r--   0        0        0     5822 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/consumers/service.py
--rw-r--r--   0        0        0      130 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/exceptions.py
--rw-r--r--   0        0        0     2357 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/fields.py
--rw-r--r--   0        0        0        0 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/management/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/management/commands/__init__.py
--rw-r--r--   0        0        0     2299 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/management/commands/sync_data_stores.py
--rw-r--r--   0        0        0     2990 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/messages.py
--rw-r--r--   0        0        0     2345 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/migrations/0001_initial.py
--rw-r--r--   0        0        0      595 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/migrations/0002_slug_unique_and_not_editable.py
--rw-r--r--   0        0        0      408 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/migrations/0003_rename_slug_to_name.py
--rw-r--r--   0        0        0      670 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/migrations/0004_add_timestamps.py
--rw-r--r--   0        0        0      731 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/migrations/0005_question_date_help_text.py
--rw-r--r--   0        0        0     4710 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/migrations/0006_service_revisions_and_events.py
--rw-r--r--   0        0        0     1476 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/migrations/0007_registered_to_revision.py
--rw-r--r--   0        0        0      669 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/migrations/0008_registered_relations_to_nullable.py
--rw-r--r--   0        0        0      683 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/migrations/0009_remove_registered_services.py
--rw-r--r--   0        0        0      681 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/migrations/0010_alter_servicerevision_project_name.py
--rw-r--r--   0        0        0      362 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/migrations/0011_remove_servicerevision_topic_id.py
--rw-r--r--   0        0        0      568 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/migrations/0012_servicerevision_is_default.py
--rw-r--r--   0        0        0      639 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/migrations/0013_alter_serviceusageevent_question.py
--rw-r--r--   0        0        0        0 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/migrations/__init__.py
--rw-r--r--   0        0        0      698 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/models/__init__.py
--rw-r--r--   0        0        0    11448 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/models/datastores.py
--rw-r--r--   0        0        0       85 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/models/querysets/__init__.py
--rw-r--r--   0        0        0     9794 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/models/querysets/datastore_queryset.py
--rw-r--r--   0        0        0     6623 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/models/questions.py
--rw-r--r--   0        0        0     7824 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/models/service_revisions.py
--rw-r--r--   0        0        0     2514 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/models/service_usage_events.py
--rw-r--r--   0        0        0      290 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/routing.py
--rw-r--r--   0        0        0      479 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/signals/__init__.py
--rw-r--r--   0        0        0     3079 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/signals/receivers.py
--rw-r--r--   0        0        0      262 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/signals/senders.py
--rw-r--r--   0        0        0        0 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/static/.gitignore
--rw-r--r--   0        0        0     2666 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/tasks.py
--rw-r--r--   0        0        0     1149 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/templates/admin/question_ask_row.html
--rw-r--r--   0        0        0        0 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/templates/django_twined/.gitignore
--rw-r--r--   0        0        0      343 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/templates/django_twined/question_changeform.html
--rw-r--r--   0        0        0        0 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/templatetags/__init__.py
--rw-r--r--   0        0        0      480 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/templatetags/question_ask_row.py
--rw-r--r--   0        0        0     1532 2023-06-13 08:00:29.731306 django_twined-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     2599 1970-01-01 00:00:00.000000 django_twined-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-06-21 17:04:03.628860 django_twined-0.4.4/LICENSE
+-rw-r--r--   0        0        0     1463 2023-06-21 17:04:03.628860 django_twined-0.4.4/README.md
+-rw-r--r--   0        0        0       64 2023-06-21 17:04:03.628860 django_twined-0.4.4/django_twined/__init__.py
+-rw-r--r--   0        0        0      257 2023-06-21 17:04:03.628860 django_twined-0.4.4/django_twined/admin/__init__.py
+-rw-r--r--   0        0        0     6781 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/admin/admin.py
+-rw-r--r--   0        0        0      402 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/admin/fieldsets.py
+-rw-r--r--   0        0        0      881 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/admin/mixins.py
+-rw-r--r--   0        0        0      682 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/admin/proxy.py
+-rw-r--r--   0        0        0      496 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/apps.py
+-rw-r--r--   0        0        0      104 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/consumers/__init__.py
+-rw-r--r--   0        0        0     3765 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/consumers/analysis.py
+-rw-r--r--   0        0        0     1001 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/consumers/analysis_log.py
+-rw-r--r--   0        0        0     5822 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/consumers/service.py
+-rw-r--r--   0        0        0      130 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/exceptions.py
+-rw-r--r--   0        0        0     2357 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/fields.py
+-rw-r--r--   0        0        0        0 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/management/commands/__init__.py
+-rw-r--r--   0        0        0     2299 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/management/commands/sync_data_stores.py
+-rw-r--r--   0        0        0     2990 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/messages.py
+-rw-r--r--   0        0        0     2345 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/migrations/0001_initial.py
+-rw-r--r--   0        0        0      595 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/migrations/0002_slug_unique_and_not_editable.py
+-rw-r--r--   0        0        0      408 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/migrations/0003_rename_slug_to_name.py
+-rw-r--r--   0        0        0      670 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/migrations/0004_add_timestamps.py
+-rw-r--r--   0        0        0      731 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/migrations/0005_question_date_help_text.py
+-rw-r--r--   0        0        0     4710 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/migrations/0006_service_revisions_and_events.py
+-rw-r--r--   0        0        0     1476 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/migrations/0007_registered_to_revision.py
+-rw-r--r--   0        0        0      669 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/migrations/0008_registered_relations_to_nullable.py
+-rw-r--r--   0        0        0      683 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/migrations/0009_remove_registered_services.py
+-rw-r--r--   0        0        0      681 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/migrations/0010_alter_servicerevision_project_name.py
+-rw-r--r--   0        0        0      362 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/migrations/0011_remove_servicerevision_topic_id.py
+-rw-r--r--   0        0        0      568 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/migrations/0012_servicerevision_is_default.py
+-rw-r--r--   0        0        0      639 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/migrations/0013_alter_serviceusageevent_question.py
+-rw-r--r--   0        0        0        0 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/migrations/__init__.py
+-rw-r--r--   0        0        0      698 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/models/__init__.py
+-rw-r--r--   0        0        0    11440 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/models/datastores.py
+-rw-r--r--   0        0        0       85 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/models/querysets/__init__.py
+-rw-r--r--   0        0        0     9794 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/models/querysets/datastore_queryset.py
+-rw-r--r--   0        0        0     6623 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/models/questions.py
+-rw-r--r--   0        0        0     7824 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/models/service_revisions.py
+-rw-r--r--   0        0        0     2514 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/models/service_usage_events.py
+-rw-r--r--   0        0        0      290 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/routing.py
+-rw-r--r--   0        0        0      479 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/signals/__init__.py
+-rw-r--r--   0        0        0     3079 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/signals/receivers.py
+-rw-r--r--   0        0        0      262 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/signals/senders.py
+-rw-r--r--   0        0        0        0 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/static/.gitignore
+-rw-r--r--   0        0        0     2666 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/tasks.py
+-rw-r--r--   0        0        0     1149 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/templates/admin/question_ask_row.html
+-rw-r--r--   0        0        0        0 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/templates/django_twined/.gitignore
+-rw-r--r--   0        0        0      343 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/templates/django_twined/question_changeform.html
+-rw-r--r--   0        0        0        0 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/templatetags/__init__.py
+-rw-r--r--   0        0        0      480 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/templatetags/question_ask_row.py
+-rw-r--r--   0        0        0     1532 2023-06-21 17:04:03.632860 django_twined-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     2599 1970-01-01 00:00:00.000000 django_twined-0.4.4/PKG-INFO
```

### Comparing `django_twined-0.4.3/LICENSE` & `django_twined-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.3/README.md` & `django_twined-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.3/django_twined/admin/admin.py` & `django_twined-0.4.4/django_twined/admin/admin.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.3/django_twined/admin/mixins.py` & `django_twined-0.4.4/django_twined/admin/mixins.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.3/django_twined/admin/proxy.py` & `django_twined-0.4.4/django_twined/admin/proxy.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.3/django_twined/consumers/analysis.py` & `django_twined-0.4.4/django_twined/consumers/analysis.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.3/django_twined/consumers/analysis_log.py` & `django_twined-0.4.4/django_twined/consumers/analysis_log.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.3/django_twined/consumers/service.py` & `django_twined-0.4.4/django_twined/consumers/service.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.3/django_twined/fields.py` & `django_twined-0.4.4/django_twined/fields.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.3/django_twined/management/commands/sync_data_stores.py` & `django_twined-0.4.4/django_twined/management/commands/sync_data_stores.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.3/django_twined/messages.py` & `django_twined-0.4.4/django_twined/messages.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.3/django_twined/migrations/0001_initial.py` & `django_twined-0.4.4/django_twined/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.3/django_twined/migrations/0002_slug_unique_and_not_editable.py` & `django_twined-0.4.4/django_twined/migrations/0002_slug_unique_and_not_editable.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.3/django_twined/migrations/0004_add_timestamps.py` & `django_twined-0.4.4/django_twined/migrations/0004_add_timestamps.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.3/django_twined/migrations/0005_question_date_help_text.py` & `django_twined-0.4.4/django_twined/migrations/0005_question_date_help_text.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.3/django_twined/migrations/0006_service_revisions_and_events.py` & `django_twined-0.4.4/django_twined/migrations/0006_service_revisions_and_events.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.3/django_twined/migrations/0007_registered_to_revision.py` & `django_twined-0.4.4/django_twined/migrations/0007_registered_to_revision.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.3/django_twined/migrations/0008_registered_relations_to_nullable.py` & `django_twined-0.4.4/django_twined/migrations/0008_registered_relations_to_nullable.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.3/django_twined/migrations/0009_remove_registered_services.py` & `django_twined-0.4.4/django_twined/migrations/0009_remove_registered_services.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.3/django_twined/migrations/0010_alter_servicerevision_project_name.py` & `django_twined-0.4.4/django_twined/migrations/0010_alter_servicerevision_project_name.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.3/django_twined/migrations/0012_servicerevision_is_default.py` & `django_twined-0.4.4/django_twined/migrations/0012_servicerevision_is_default.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.3/django_twined/migrations/0013_alter_serviceusageevent_question.py` & `django_twined-0.4.4/django_twined/migrations/0013_alter_serviceusageevent_question.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.3/django_twined/models/__init__.py` & `django_twined-0.4.4/django_twined/models/__init__.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.3/django_twined/models/datastores.py` & `django_twined-0.4.4/django_twined/models/datastores.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
 import logging
 import uuid
 import warnings
 from django.db import models
-from django_twined.exceptions import ConsistencyError
 from octue.resources import Datafile
 from octue.utils.encoders import OctueJSONEncoder
 
 from .querysets import DatastoreQueryset
 
 
 logger = logging.getLogger(__name__)
@@ -108,16 +107,19 @@
                 path,
                 ignore_stored_metadata=False,
                 tags=self.get_tags_from_instance(),
                 labels=self.get_labels_from_instance(),
             )
 
         if df.id != str(self.id):
-            raise ConsistencyError(
-                f"Datafile at {self.gs_path} has bound id {df.id} but that does not match this instance id {str(self.id)}. Re-sync your database to the store."
+            logger.warning(
+                "Datafile at %s has bound id %s but that does not match this instance id %s. Re-sync your database to the store.",
+                self.gs_path,
+                df.id,
+                str(self.id),
             )
 
         return df
 
     @classmethod
     def from_datafile(cls, datafile, create_if_missing=True, update_db_metadata=True):
         """Gets database record corresponding to an octue datafile object.
```

### Comparing `django_twined-0.4.3/django_twined/models/querysets/datastore_queryset.py` & `django_twined-0.4.4/django_twined/models/querysets/datastore_queryset.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.3/django_twined/models/questions.py` & `django_twined-0.4.4/django_twined/models/questions.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.3/django_twined/models/service_revisions.py` & `django_twined-0.4.4/django_twined/models/service_revisions.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.3/django_twined/models/service_usage_events.py` & `django_twined-0.4.4/django_twined/models/service_usage_events.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.3/django_twined/signals/receivers.py` & `django_twined-0.4.4/django_twined/signals/receivers.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.3/django_twined/tasks.py` & `django_twined-0.4.4/django_twined/tasks.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.3/django_twined/templates/admin/question_ask_row.html` & `django_twined-0.4.4/django_twined/templates/admin/question_ask_row.html`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.3/pyproject.toml` & `django_twined-0.4.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-twined"
-version = "0.4.3"
+version = "0.4.4"
 description = "A django app to manage octue services"
 authors = ["Tom Clark <tom@octue.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

### Comparing `django_twined-0.4.3/PKG-INFO` & `django_twined-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-twined
-Version: 0.4.3
+Version: 0.4.4
 Summary: A django app to manage octue services
 Home-page: https://github.com/octue/django-twined
 License: MIT
 Keywords: django,services,octue,twined
 Author: Tom Clark
 Author-email: tom@octue.com
 Requires-Python: >=3.9,<3.11
```

