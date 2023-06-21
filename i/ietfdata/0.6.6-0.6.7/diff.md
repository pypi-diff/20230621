# Comparing `tmp/ietfdata-0.6.6.tar.gz` & `tmp/ietfdata-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ietfdata-0.6.6.tar", last modified: Fri May 19 14:15:00 2023, max compression
+gzip compressed data, was "ietfdata-0.6.7.tar", last modified: Wed Jun 21 08:20:51 2023, max compression
```

## Comparing `ietfdata-0.6.6.tar` & `ietfdata-0.6.7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwx---   0 csp        (502) staff       (20)        0 2023-05-19 14:15:00.240742 ietfdata-0.6.6/
--rw-r--r--   0 csp        (502) staff       (20)     1294 2021-04-14 11:17:29.000000 ietfdata-0.6.6/LICENSE
--rw-rw----   0 csp        (502) staff       (20)     2970 2023-05-19 14:15:00.240053 ietfdata-0.6.6/PKG-INFO
--rw-rw----   0 csp        (502) staff       (20)     2529 2022-02-21 17:42:14.000000 ietfdata-0.6.6/README.md
-drwxrwx---   0 csp        (502) staff       (20)        0 2023-05-19 14:15:00.227342 ietfdata-0.6.6/examples/
--rw-rw----   0 csp        (502) staff       (20)        0 2020-08-04 12:44:47.000000 ietfdata-0.6.6/examples/__init__.py
--rw-rw----   0 csp        (502) staff       (20)     2037 2022-10-28 12:45:40.000000 ietfdata-0.6.6/examples/bluesheets.py
--rw-r--r--   0 csp        (502) staff       (20)     2223 2021-04-14 11:17:29.000000 ietfdata-0.6.6/examples/draft-authors.py
--rw-rw----   0 csp        (502) staff       (20)     2163 2022-10-28 12:50:08.000000 ietfdata-0.6.6/examples/draft-references.py
--rw-rw----   0 csp        (502) staff       (20)     2748 2021-12-02 17:45:56.000000 ietfdata-0.6.6/examples/draft-submissions-by-date.py
--rw-rw----   0 csp        (502) staff       (20)     1695 2022-11-03 14:42:34.000000 ietfdata-0.6.6/examples/draft-submissions.py
--rw-rw----   0 csp        (502) staff       (20)     1814 2022-06-27 14:31:39.000000 ietfdata-0.6.6/examples/drafts-for-person.py
--rw-r--r--   0 csp        (502) staff       (20)     1799 2022-10-28 13:00:03.000000 ietfdata-0.6.6/examples/drafts-for-rfc.py
--rw-r--r--   0 csp        (502) staff       (20)     1981 2021-04-14 11:17:29.000000 ietfdata-0.6.6/examples/drafts-for-wg.py
--rw-rw----   0 csp        (502) staff       (20)     2910 2022-10-28 13:08:25.000000 ietfdata-0.6.6/examples/emails-per-person.py
--rw-r--r--   0 csp        (502) staff       (20)     2773 2021-04-14 11:17:29.000000 ietfdata-0.6.6/examples/ietf-leadership.py
--rw-rw----   0 csp        (502) staff       (20)     1842 2022-10-28 12:36:22.000000 ietfdata-0.6.6/examples/non-wg-standards-track-rfcs.py
--rw-r--r--   0 csp        (502) staff       (20)     2084 2021-04-14 11:17:29.000000 ietfdata-0.6.6/examples/org-chart.py
--rw-rw----   0 csp        (502) staff       (20)     1995 2022-12-10 15:03:43.000000 ietfdata-0.6.6/examples/person-attendance.py
--rw-rw----   0 csp        (502) staff       (20)     1776 2022-10-28 15:37:24.000000 ietfdata-0.6.6/examples/person-emails.py
--rw-rw----   0 csp        (502) staff       (20)     7955 2022-10-28 15:48:45.000000 ietfdata-0.6.6/examples/person.py
--rw-r-----   0 csp        (502) staff       (20)     2203 2023-04-19 18:40:26.000000 ietfdata-0.6.6/examples/recent-pubreq.py
--rw-r--r--   0 csp        (502) staff       (20)     5567 2022-10-28 15:51:05.000000 ietfdata-0.6.6/examples/rfc-data.py
--rw-rw----   0 csp        (502) staff       (20)     2155 2021-08-27 12:26:02.000000 ietfdata-0.6.6/examples/rfc-streams.py
--rw-r--r--   0 csp        (502) staff       (20)     2055 2021-04-14 11:17:29.000000 ietfdata-0.6.6/examples/role-names.py
-drwxrwx---   0 csp        (502) staff       (20)        0 2023-05-19 14:15:00.235009 ietfdata-0.6.6/ietfdata/
--rw-rw----   0 csp        (502) staff       (20)        0 2020-04-11 11:24:32.000000 ietfdata-0.6.6/ietfdata/__init__.py
--rw-rw----   0 csp        (502) staff       (20)   160704 2023-05-19 14:12:42.000000 ietfdata-0.6.6/ietfdata/datatracker.py
--rw-rw----   0 csp        (502) staff       (20)    16240 2022-04-28 14:40:41.000000 ietfdata-0.6.6/ietfdata/datatracker_ext.py
--rw-rw----   0 csp        (502) staff       (20)    25946 2022-10-28 08:25:24.000000 ietfdata-0.6.6/ietfdata/mailarchive.py
--rw-rw----   0 csp        (502) staff       (20)    22261 2022-08-29 10:29:34.000000 ietfdata-0.6.6/ietfdata/mailarchive2.py
--rw-rw----   0 csp        (502) staff       (20)        0 2020-04-11 11:24:32.000000 ietfdata-0.6.6/ietfdata/py.typed
--rw-rw----   0 csp        (502) staff       (20)    24747 2022-02-13 18:30:57.000000 ietfdata-0.6.6/ietfdata/rfcindex.py
-drwxrwx---   0 csp        (502) staff       (20)        0 2023-05-19 14:15:00.239137 ietfdata-0.6.6/ietfdata.egg-info/
--rw-rw----   0 csp        (502) staff       (20)     2970 2023-05-19 14:15:00.000000 ietfdata-0.6.6/ietfdata.egg-info/PKG-INFO
--rw-rw----   0 csp        (502) staff       (20)      900 2023-05-19 14:15:00.000000 ietfdata-0.6.6/ietfdata.egg-info/SOURCES.txt
--rw-rw----   0 csp        (502) staff       (20)        1 2023-05-19 14:15:00.000000 ietfdata-0.6.6/ietfdata.egg-info/dependency_links.txt
--rw-rw----   0 csp        (502) staff       (20)      110 2023-05-19 14:15:00.000000 ietfdata-0.6.6/ietfdata.egg-info/requires.txt
--rw-rw----   0 csp        (502) staff       (20)       18 2023-05-19 14:15:00.000000 ietfdata-0.6.6/ietfdata.egg-info/top_level.txt
--rw-rw----   0 csp        (502) staff       (20)      100 2021-05-19 10:27:44.000000 ietfdata-0.6.6/pyproject.toml
--rw-rw----   0 csp        (502) staff       (20)       38 2023-05-19 14:15:00.240954 ietfdata-0.6.6/setup.cfg
--rw-rw----   0 csp        (502) staff       (20)      783 2023-05-19 14:12:49.000000 ietfdata-0.6.6/setup.py
+drwxrwx---   0 csp        (502) staff       (20)        0 2023-06-21 08:20:51.317871 ietfdata-0.6.7/
+-rw-r--r--   0 csp        (502) staff       (20)     1294 2021-04-14 11:17:29.000000 ietfdata-0.6.7/LICENSE
+-rw-rw----   0 csp        (502) staff       (20)     2970 2023-06-21 08:20:51.317015 ietfdata-0.6.7/PKG-INFO
+-rw-rw----   0 csp        (502) staff       (20)     2529 2023-06-21 08:17:16.000000 ietfdata-0.6.7/README.md
+drwxrwx---   0 csp        (502) staff       (20)        0 2023-06-21 08:20:51.299359 ietfdata-0.6.7/examples/
+-rw-rw----   0 csp        (502) staff       (20)        0 2020-08-04 12:44:47.000000 ietfdata-0.6.7/examples/__init__.py
+-rw-rw----   0 csp        (502) staff       (20)     2037 2022-10-28 12:45:40.000000 ietfdata-0.6.7/examples/bluesheets.py
+-rw-r--r--   0 csp        (502) staff       (20)     2223 2021-04-14 11:17:29.000000 ietfdata-0.6.7/examples/draft-authors.py
+-rw-rw----   0 csp        (502) staff       (20)     2163 2022-10-28 12:50:08.000000 ietfdata-0.6.7/examples/draft-references.py
+-rw-rw----   0 csp        (502) staff       (20)     2748 2021-12-02 17:45:56.000000 ietfdata-0.6.7/examples/draft-submissions-by-date.py
+-rw-rw----   0 csp        (502) staff       (20)     1695 2022-11-03 14:42:34.000000 ietfdata-0.6.7/examples/draft-submissions.py
+-rw-rw----   0 csp        (502) staff       (20)     1814 2022-06-27 14:31:39.000000 ietfdata-0.6.7/examples/drafts-for-person.py
+-rw-r--r--   0 csp        (502) staff       (20)     1799 2022-10-28 13:00:03.000000 ietfdata-0.6.7/examples/drafts-for-rfc.py
+-rw-r--r--   0 csp        (502) staff       (20)     1981 2021-04-14 11:17:29.000000 ietfdata-0.6.7/examples/drafts-for-wg.py
+-rw-rw----   0 csp        (502) staff       (20)     2910 2022-10-28 13:08:25.000000 ietfdata-0.6.7/examples/emails-per-person.py
+-rw-r--r--   0 csp        (502) staff       (20)     2773 2021-04-14 11:17:29.000000 ietfdata-0.6.7/examples/ietf-leadership.py
+-rw-rw----   0 csp        (502) staff       (20)     1842 2022-10-28 12:36:22.000000 ietfdata-0.6.7/examples/non-wg-standards-track-rfcs.py
+-rw-r--r--   0 csp        (502) staff       (20)     2084 2021-04-14 11:17:29.000000 ietfdata-0.6.7/examples/org-chart.py
+-rw-rw----   0 csp        (502) staff       (20)     1995 2022-12-10 15:03:43.000000 ietfdata-0.6.7/examples/person-attendance.py
+-rw-rw----   0 csp        (502) staff       (20)     1776 2022-10-28 15:37:24.000000 ietfdata-0.6.7/examples/person-emails.py
+-rw-rw----   0 csp        (502) staff       (20)     7955 2022-10-28 15:48:45.000000 ietfdata-0.6.7/examples/person.py
+-rw-r-----   0 csp        (502) staff       (20)     2203 2023-04-19 18:40:26.000000 ietfdata-0.6.7/examples/recent-pubreq.py
+-rw-r--r--   0 csp        (502) staff       (20)     5567 2022-10-28 15:51:05.000000 ietfdata-0.6.7/examples/rfc-data.py
+-rw-rw----   0 csp        (502) staff       (20)     2155 2021-08-27 12:26:02.000000 ietfdata-0.6.7/examples/rfc-streams.py
+-rw-r--r--   0 csp        (502) staff       (20)     2055 2021-04-14 11:17:29.000000 ietfdata-0.6.7/examples/role-names.py
+drwxrwx---   0 csp        (502) staff       (20)        0 2023-06-21 08:20:51.308664 ietfdata-0.6.7/ietfdata/
+-rw-rw----   0 csp        (502) staff       (20)        0 2020-04-11 11:24:32.000000 ietfdata-0.6.7/ietfdata/__init__.py
+-rw-rw----   0 csp        (502) staff       (20)   160734 2023-06-21 08:17:09.000000 ietfdata-0.6.7/ietfdata/datatracker.py
+-rw-rw----   0 csp        (502) staff       (20)    16240 2022-04-28 14:40:41.000000 ietfdata-0.6.7/ietfdata/datatracker_ext.py
+-rw-rw----   0 csp        (502) staff       (20)    25946 2022-10-28 08:25:24.000000 ietfdata-0.6.7/ietfdata/mailarchive.py
+-rw-rw----   0 csp        (502) staff       (20)    24502 2023-06-21 08:09:13.000000 ietfdata-0.6.7/ietfdata/mailarchive2.py
+-rw-rw----   0 csp        (502) staff       (20)        0 2020-04-11 11:24:32.000000 ietfdata-0.6.7/ietfdata/py.typed
+-rw-rw----   0 csp        (502) staff       (20)    24747 2022-02-13 18:30:57.000000 ietfdata-0.6.7/ietfdata/rfcindex.py
+drwxrwx---   0 csp        (502) staff       (20)        0 2023-06-21 08:20:51.315798 ietfdata-0.6.7/ietfdata.egg-info/
+-rw-rw----   0 csp        (502) staff       (20)     2970 2023-06-21 08:20:51.000000 ietfdata-0.6.7/ietfdata.egg-info/PKG-INFO
+-rw-rw----   0 csp        (502) staff       (20)      900 2023-06-21 08:20:51.000000 ietfdata-0.6.7/ietfdata.egg-info/SOURCES.txt
+-rw-rw----   0 csp        (502) staff       (20)        1 2023-06-21 08:20:51.000000 ietfdata-0.6.7/ietfdata.egg-info/dependency_links.txt
+-rw-rw----   0 csp        (502) staff       (20)      110 2023-06-21 08:20:51.000000 ietfdata-0.6.7/ietfdata.egg-info/requires.txt
+-rw-rw----   0 csp        (502) staff       (20)       18 2023-06-21 08:20:51.000000 ietfdata-0.6.7/ietfdata.egg-info/top_level.txt
+-rw-rw----   0 csp        (502) staff       (20)      100 2021-05-19 10:27:44.000000 ietfdata-0.6.7/pyproject.toml
+-rw-rw----   0 csp        (502) staff       (20)       38 2023-06-21 08:20:51.318108 ietfdata-0.6.7/setup.cfg
+-rw-rw----   0 csp        (502) staff       (20)      783 2023-06-21 08:17:00.000000 ietfdata-0.6.7/setup.py
```

### Comparing `ietfdata-0.6.6/LICENSE` & `ietfdata-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.6/PKG-INFO` & `ietfdata-0.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ietfdata
-Version: 0.6.6
+Version: 0.6.7
 Summary: Access the IETF Data Tracker and RFC Index
 Home-page: https://github.com/glasgow-ipl/ietfdata
 Author: Colin Perkins
 Author-email: csp@csperkins.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `ietfdata-0.6.6/README.md` & `ietfdata-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.6/examples/bluesheets.py` & `ietfdata-0.6.7/examples/bluesheets.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.6/examples/draft-authors.py` & `ietfdata-0.6.7/examples/draft-authors.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.6/examples/draft-references.py` & `ietfdata-0.6.7/examples/draft-references.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.6/examples/draft-submissions-by-date.py` & `ietfdata-0.6.7/examples/draft-submissions-by-date.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.6/examples/draft-submissions.py` & `ietfdata-0.6.7/examples/draft-submissions.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.6/examples/drafts-for-person.py` & `ietfdata-0.6.7/examples/drafts-for-person.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.6/examples/drafts-for-rfc.py` & `ietfdata-0.6.7/examples/drafts-for-rfc.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.6/examples/drafts-for-wg.py` & `ietfdata-0.6.7/examples/drafts-for-wg.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.6/examples/emails-per-person.py` & `ietfdata-0.6.7/examples/emails-per-person.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.6/examples/ietf-leadership.py` & `ietfdata-0.6.7/examples/ietf-leadership.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.6/examples/non-wg-standards-track-rfcs.py` & `ietfdata-0.6.7/examples/non-wg-standards-track-rfcs.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.6/examples/org-chart.py` & `ietfdata-0.6.7/examples/org-chart.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.6/examples/person-attendance.py` & `ietfdata-0.6.7/examples/person-attendance.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.6/examples/person-emails.py` & `ietfdata-0.6.7/examples/person-emails.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.6/examples/person.py` & `ietfdata-0.6.7/examples/person.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.6/examples/recent-pubreq.py` & `ietfdata-0.6.7/examples/recent-pubreq.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.6/examples/rfc-data.py` & `ietfdata-0.6.7/examples/rfc-data.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.6/examples/rfc-streams.py` & `ietfdata-0.6.7/examples/rfc-streams.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.6/examples/role-names.py` & `ietfdata-0.6.7/examples/role-names.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.6/ietfdata/datatracker.py` & `ietfdata-0.6.7/ietfdata/datatracker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1042,14 +1042,15 @@
     short               : str
     attendees           : Optional[int]
     modified            : datetime
     comments            : str
     on_agenda           : bool
     purpose             : SessionPurposeURI
     has_onsite_tool     : bool
+    chat_room           : str
 
 
 @dataclass(frozen=True)
 class SessionStatusNameURI(URI):
     root : str = "/api/v1/name/sessionstatusname/"
 
 
@@ -1727,15 +1728,15 @@
                 mongodb_pass = cache_pass
 
         logging.getLogger('requests_cache').setLevel('WARN')
 
         logging.basicConfig(level=os.environ.get("IETFDATA_LOGLEVEL", "INFO"))
         self.log = logging.getLogger("ietfdata")
 
-        self.ua        = "glasgow-ietfdata/0.6.6"          # Update when making a new relaase
+        self.ua        = "glasgow-ietfdata/0.6.7"          # Update when making a new relaase
         self.base_url  = os.environ.get("IETFDATA_DT_URL", "https://datatracker.ietf.org")
         self.http_req  = 0
         self.get_count = 0
 
         if use_cache:
             self.log.info(f"mongodb host = {mongodb_host}")
             self.log.info(f"mongodb port = {mongodb_port}")
```

### Comparing `ietfdata-0.6.6/ietfdata/datatracker_ext.py` & `ietfdata-0.6.7/ietfdata/datatracker_ext.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.6/ietfdata/mailarchive.py` & `ietfdata-0.6.7/ietfdata/mailarchive.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.6/ietfdata/mailarchive2.py` & `ietfdata-0.6.7/ietfdata/mailarchive2.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 from gridfs             import GridFS
 from pymongo            import MongoClient, ASCENDING, ReplaceOne, UpdateOne
 from pymongo.database   import Database
 from email              import policy, utils
 from email.message      import Message as EmailMessage
 from email_reply_parser import EmailReplyParser
 from imapclient         import IMAPClient
+from dataclasses        import field
 
 # =================================================================================================
 # Database design for the mail archive:
 #
 # The data is stored in a MongoDB database `ietfdata_mailarchive_v2`. The database
 # contains two collections plus a GridFS instance.
 #
@@ -96,14 +97,16 @@
     _mailing_list : MailingList
     _uidvalidity  : int
     _uid          : int
     _gridfs_id    : int
     _timestamp    : datetime
     _size         : int
     _headers      : Dict[str, List[str]]
+    _parent       : Optional[Message] = None
+    _children     : List[Message] = field(default_factory=list)
 
     def __init__(self,
                  ml: MailingList,
                  uidvalidity: int,
                  uid: int,
                  gridfs_id: int,
                  timestamp: datetime,
@@ -112,14 +115,15 @@
         self._mailing_list = ml
         self._uidvalidity  = uidvalidity
         self._uid          = uid
         self._gridfs_id    = gridfs_id
         self._timestamp    = timestamp
         self._size         = size
         self._headers      = headers
+        self._children     = []
 
 
     # Accessors for messages properties. Messages in IMAP are assigned
     # a unique identifier `uid()` within a folder representing a mailing
     # list. That identifier is not supposed to change, but the IMAP
     # standard recognises that mailboxes occasionally get rebuilt. If
     # this happens, the `uidvalidity()` will change. The combination of
@@ -159,16 +163,25 @@
         return self._headers["cc"][0] if "cc" in self._headers else None
 
 
     def header_subject(self) -> Optional[str]:
         return self._headers["subject"][0] if "subject" in self._headers else None
 
 
-    def header_date(self) -> Optional[str]:
-        return self._headers["date"][0] if "date" in self._headers else None
+    def header_date(self) -> Optional[datetime]:
+        msg_date = None # type: Optional[datetime]
+        try:
+            parsed_date = email.utils.parsedate(self._headers["date"][0]) 
+            if parsed_date is not None:
+                msg_date = datetime.fromtimestamp(time.mktime(parsed_date))
+            else:
+                msg_date = None
+        except:
+            msg_date = None
+        return msg_date
 
 
     def header_message_id(self) -> Optional[str]:
         return self._headers["message-id"][0] if "message-id" in self._headers else None
 
 
     def header_in_reply_to(self) -> Optional[str]:
@@ -227,31 +240,58 @@
             timestamp    = message["timestamp"]
             size         = message["size"]
             headers      = message["headers"]
             replies.append(Message(mailing_list, uidvalidity, uid, gridfs_id, timestamp, size, headers))
         return replies
 
 
+    def add_child_message(self, child: Message):
+        self._children.append(child)
+
+
+    def get_child_count(self) -> int:
+        return len(self._children) + sum([child.get_child_count() for child in self._children])
+
+
+    def get_child_from_addrs(self, child_from_addrs: List[str]) -> List[str]:
+        header_from = self.header_from()
+        if header_from is not None:
+            child_from_addrs.append(header_from)
+        for child in self._children:
+            child.get_child_from_addrs(child_from_addrs)
+        return child_from_addrs
+
+
+    def get_child_dates(self, child_dates: List[datetime]):
+        child_dates.append(self.timestamp())
+        for child in self._children:
+            child.get_child_dates(child_dates)
+        return child_dates
+
+
 # =================================================================================================
 
 class MessageThread:
     def __init__(self, root: Message):
         self.root = root
 
 
     def get_message_count(self):
-        pass # FIXME
+        return 1 + self.root.get_child_count()
 
 
     def get_unique_from_count(self):
-        pass # FIXME
+        from_addrs = self.root.get_child_from_addrs([])
+        return len(list(set(from_addrs)))
 
 
     def get_duration(self):
-        pass # FIXME
+        earliest_date = self.root.timestamp()
+        latest_date = sorted(self.root.get_child_dates([]), reverse=True)[0]
+        return latest_date - earliest_date
 
 
 # =================================================================================================
 
 class MailingList:
     _log          : logging.Logger
     _mail_archive : MailArchive
@@ -422,14 +462,28 @@
                 self._log.info(f"saved message {self._list_name}/{uid}")
 
         imap.unselect_folder()
         imap.logout()
         return msgs_to_fetch
 
 
+    def threads(self) -> Iterator[MessageThread]:
+        threads = []
+        message_by_message_id = {message.header_message_id() : message for message in self.messages()}
+
+        for message_id in message_by_message_id:
+            message = message_by_message_id[message_id]
+            if message.header_in_reply_to() is None:
+                threads.append(message)
+            if message.header_in_reply_to() is not None and message.header_in_reply_to() in message_by_message_id:
+                message._parent = message_by_message_id[message.header_in_reply_to()]
+                message_by_message_id[message.header_in_reply_to()].add_child_message(message)
+
+        return iter([MessageThread(message) for message in threads])
+
     #def threads(self) -> Iterator[MessageThread]:
     #    ts = TopologicalSorter()
     #    for msg in self.messages():
     #        if msg.header_references() is not None:
     #            ts.add(msg.header_message_id(), msg.header_references().split(" ").reverse())
     #        elif msg.header_in_reply_to() is not None:
     #            ts.add(msg.header_message_id(), msg.header_in_reply_to())
```

### Comparing `ietfdata-0.6.6/ietfdata/rfcindex.py` & `ietfdata-0.6.7/ietfdata/rfcindex.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.6/ietfdata.egg-info/PKG-INFO` & `ietfdata-0.6.7/ietfdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ietfdata
-Version: 0.6.6
+Version: 0.6.7
 Summary: Access the IETF Data Tracker and RFC Index
 Home-page: https://github.com/glasgow-ipl/ietfdata
 Author: Colin Perkins
 Author-email: csp@csperkins.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `ietfdata-0.6.6/ietfdata.egg-info/SOURCES.txt` & `ietfdata-0.6.7/ietfdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.6/setup.py` & `ietfdata-0.6.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ietfdata",
-    version="0.6.6",
+    version="0.6.7",
     author="Colin Perkins",
     author_email="csp@csperkins.org",
     description="Access the IETF Data Tracker and RFC Index",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/glasgow-ipl/ietfdata",
     packages=setuptools.find_packages(),
```

