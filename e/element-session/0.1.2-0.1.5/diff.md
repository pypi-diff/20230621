# Comparing `tmp/element-session-0.1.2.tar.gz` & `tmp/element-session-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "element-session-0.1.2.tar", last modified: Wed Jun  8 19:11:58 2022, max compression
+gzip compressed data, was "element-session-0.1.5.tar", last modified: Wed Jun 21 01:53:18 2023, max compression
```

## Comparing `element-session-0.1.2.tar` & `element-session-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 anaconda  (1001) anaconda   (101)        0 2022-06-08 19:11:58.147764 element-session-0.1.2/
--rw-r--r--   0 anaconda  (1001) anaconda   (101)     2841 2022-06-08 19:11:58.147764 element-session-0.1.2/PKG-INFO
--rw-r--r--   0 anaconda  (1001) anaconda   (101)     2144 2022-06-08 19:11:33.000000 element-session-0.1.2/README.md
-drwxr-xr-x   0 anaconda  (1001) anaconda   (101)        0 2022-06-08 19:11:58.147764 element-session-0.1.2/element_session/
--rw-r--r--   0 anaconda  (1001) anaconda   (101)       47 2022-06-08 19:11:33.000000 element-session-0.1.2/element_session/__init__.py
-drwxr-xr-x   0 anaconda  (1001) anaconda   (101)        0 2022-06-08 19:11:58.147764 element-session-0.1.2/element_session/export/
--rw-r--r--   0 anaconda  (1001) anaconda   (101)        0 2022-06-08 19:11:33.000000 element-session-0.1.2/element_session/export/__init__.py
--rw-r--r--   0 anaconda  (1001) anaconda   (101)     3661 2022-06-08 19:11:33.000000 element-session-0.1.2/element_session/export/nwb.py
--rw-r--r--   0 anaconda  (1001) anaconda   (101)     2424 2022-06-08 19:11:33.000000 element-session-0.1.2/element_session/session_with_datetime.py
--rw-r--r--   0 anaconda  (1001) anaconda   (101)     2539 2022-06-08 19:11:33.000000 element-session-0.1.2/element_session/session_with_id.py
--rw-r--r--   0 anaconda  (1001) anaconda   (101)       46 2022-06-08 19:11:33.000000 element-session-0.1.2/element_session/version.py
-drwxr-xr-x   0 anaconda  (1001) anaconda   (101)        0 2022-06-08 19:11:58.147764 element-session-0.1.2/element_session.egg-info/
--rw-r--r--   0 anaconda  (1001) anaconda   (101)     2841 2022-06-08 19:11:58.000000 element-session-0.1.2/element_session.egg-info/PKG-INFO
--rw-r--r--   0 anaconda  (1001) anaconda   (101)      408 2022-06-08 19:11:58.000000 element-session-0.1.2/element_session.egg-info/SOURCES.txt
--rw-r--r--   0 anaconda  (1001) anaconda   (101)        1 2022-06-08 19:11:58.000000 element-session-0.1.2/element_session.egg-info/dependency_links.txt
--rw-r--r--   0 anaconda  (1001) anaconda   (101)       18 2022-06-08 19:11:58.000000 element-session-0.1.2/element_session.egg-info/requires.txt
--rw-r--r--   0 anaconda  (1001) anaconda   (101)       16 2022-06-08 19:11:58.000000 element-session-0.1.2/element_session.egg-info/top_level.txt
--rw-r--r--   0 anaconda  (1001) anaconda   (101)       38 2022-06-08 19:11:58.147764 element-session-0.1.2/setup.cfg
--rw-r--r--   0 anaconda  (1001) anaconda   (101)      959 2022-06-08 19:11:33.000000 element-session-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:53:18.050517 element-session-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-21 01:53:14.000000 element-session-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-21 01:53:18.050517 element-session-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-21 01:53:14.000000 element-session-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:53:18.050517 element-session-0.1.5/element_session/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-21 01:53:14.000000 element-session-0.1.5/element_session/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:53:18.050517 element-session-0.1.5/element_session/export/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 01:53:14.000000 element-session-0.1.5/element_session/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-06-21 01:53:14.000000 element-session-0.1.5/element_session/export/nwb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-06-21 01:53:14.000000 element-session-0.1.5/element_session/session_with_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-06-21 01:53:14.000000 element-session-0.1.5/element_session/session_with_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-21 01:53:14.000000 element-session-0.1.5/element_session/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:53:18.050517 element-session-0.1.5/element_session.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-21 01:53:17.000000 element-session-0.1.5/element_session.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-21 01:53:17.000000 element-session-0.1.5/element_session.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 01:53:17.000000 element-session-0.1.5/element_session.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 01:53:17.000000 element-session-0.1.5/element_session.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-21 01:53:17.000000 element-session-0.1.5/element_session.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 01:53:18.050517 element-session-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-21 01:53:14.000000 element-session-0.1.5/setup.py
```

### Comparing `element-session-0.1.2/element_session/export/nwb.py` & `element-session-0.1.5/element_session/export/nwb.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 import datetime
 from uuid import uuid4
 import pynwb
 
 from .. import session
 
+
 def session_to_nwb(
     session_key: dict,
-    lab_key=None,
-    project_key=None,
-    protocol_key=None,
+    lab_key: dict = None,
+    project_key: dict = None,
+    protocol_key: dict = None,
     additional_nwbfile_kwargs=None,
-):
-    """Gather session- and subject-level metadata and use it to create an NWBFile. If
-    there is no subject_to_nwb export function in the current namespace, subject_id will
-    be inferred from the set of primary attributes in the Subject table upstream of Session.
+) -> pynwb.NWBFile:
+    """Return subject and session metadata ass NWBFile object
 
-    Parameters
-    ----------
-    session_key: dict,
-        e.g.,
-        {
-            'subject': 'subject5',
-            'session_datetime': datetime.datetime(2020, 5, 12, 4, 13, 7),
-        }
-        Assumes session_datetime is in UTC time zone.
-    lab_key, project_key, protocol_key: dict, optional
-        Used to gather additional optional metadata.
-    additional_nwbfile_kwargs: dict, optional
-        Optionally overwrite or add fields to NWBFile.
-
-    Returns
-    -------
-    pynwb.NWBFile
-
-    mappings:
-        session.Session::KEY -> NWBFile.session_id
-        session.Session::session_datetime -> NWBFile.session_start_time
-        session.SessionNote::session_note -> NWBFile.session_description
-        session.SessionExperimenter::user -> NWBFile.experimenter
-
-        subject.Subject::subject -> NWBFile.subject.subject_id
-        subject.Subject::sex -> NWBFile.subject.sex
-
-        lab.Lab::institution -> NWBFile.institution
-        lab.Lab::lab_name -> NWBFile.lab
-
-        lab.Protocol::protocol -> NWBFile.protocol
-        lab.Protocol::protocol_description -> NWBFile.notes
-
-        lab.Project::project_description -> NWBFile.experiment_description
-        lab.ProjectKeywords.keyword -> NWBFile.keywords
-        lab.ProjectPublication.publication -> NWBFile.related_publications
+    Gather session- and subject-level metadata and use it to create an NWBFile. If there
+    is no subject_to_nwb export function in the current namespace, subject_id will be
+    inferred from the set of primary attributes in the Subject table upstream of
+    Session.
+
+    Example:
+        session_to_nwb(
+            session_key={'subject': 'subject5',
+                'session_datetime': datetime.datetime(2020, 5, 12, 4, 13, 7)},
+            lab_key={"lab": "LabA"}
+            )
+
+    Element to NWB Mappings:
+        session.Session::KEY -> NWBFile.session_id  \n
+        session.Session::session_datetime -> NWBFile.session_start_time \n
+        session.SessionNote::session_note -> NWBFile.session_description \n
+        session.SessionExperimenter::user -> NWBFile.experimenter \n
+        subject.Subject::subject -> NWBFile.subject.subject_id \n
+        subject.Subject::sex -> NWBFile.subject.sex \n
+        lab.Lab::institution -> NWBFile.institution \n
+        lab.Lab::lab_name -> NWBFile.lab \n
+        lab.Protocol::protocol -> NWBFile.protocol \n
+        lab.Protocol::protocol_description -> NWBFile.notes \n
+        lab.Project::project_description -> NWBFile.experiment_description \n
+        lab.ProjectKeywords.keyword -> NWBFile.keywords \n
+        lab.ProjectPublication.publication -> NWBFile.related_publications \n
+
+    Args:
+        session_key (dict): Key for session.Session.
+            Assumes session_datetime is in UTC time zone.
+        lab_key (dict, optional): Key for lab.Lab. Defaults to None.
+        project_key (dict, optional): Key for lab.Project. Defaults to None.
+        protocol_key (dict, optional): Key for Lab.Protocol. Defaults to None.
+        additional_nwbfile_kwargs (dict, optional): Optionally overwrite or add fields
+            to NWBFile. Defaults to None.
 
+    Returns:
+        pynwb.NWBFile: NWB file object
     """
 
     # ensure only one session key is entered
     session_key = (session.Session & session_key).fetch1("KEY")
 
     session_identifier = {
         k: v.isoformat() if isinstance(v, datetime.datetime) else v
```

### Comparing `element-session-0.1.2/setup.py` & `element-session-0.1.5/setup.py`

 * *Files identical despite different names*

