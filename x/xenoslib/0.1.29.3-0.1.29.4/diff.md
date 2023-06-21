# Comparing `tmp/xenoslib-0.1.29.3.tar.gz` & `tmp/xenoslib-0.1.29.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xenoslib-0.1.29.3.tar", last modified: Tue Jun 20 07:10:58 2023, max compression
+gzip compressed data, was "xenoslib-0.1.29.4.tar", last modified: Wed Jun 21 02:34:54 2023, max compression
```

## Comparing `xenoslib-0.1.29.3.tar` & `xenoslib-0.1.29.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:10:58.821624 xenoslib-0.1.29.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-20 07:10:45.000000 xenoslib-0.1.29.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-20 07:10:58.821624 xenoslib-0.1.29.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-20 07:10:45.000000 xenoslib-0.1.29.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 07:10:58.821624 xenoslib-0.1.29.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-20 07:10:45.000000 xenoslib-0.1.29.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:10:58.821624 xenoslib-0.1.29.3/xenoslib/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-20 07:10:45.000000 xenoslib-0.1.29.3/xenoslib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-20 07:10:45.000000 xenoslib-0.1.29.3/xenoslib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-20 07:10:45.000000 xenoslib-0.1.29.3/xenoslib/about.py
--rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-06-20 07:10:45.000000 xenoslib-0.1.29.3/xenoslib/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-20 07:10:45.000000 xenoslib-0.1.29.3/xenoslib/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-06-20 07:10:45.000000 xenoslib-0.1.29.3/xenoslib/extend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-20 07:10:45.000000 xenoslib-0.1.29.3/xenoslib/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-06-20 07:10:45.000000 xenoslib-0.1.29.3/xenoslib/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-20 07:10:45.000000 xenoslib-0.1.29.3/xenoslib/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-06-20 07:10:45.000000 xenoslib-0.1.29.3/xenoslib/onedrive.py
--rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-06-20 07:10:45.000000 xenoslib-0.1.29.3/xenoslib/win_trayicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-20 07:10:45.000000 xenoslib-0.1.29.3/xenoslib/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:10:58.821624 xenoslib-0.1.29.3/xenoslib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-20 07:10:58.000000 xenoslib-0.1.29.3/xenoslib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-20 07:10:58.000000 xenoslib-0.1.29.3/xenoslib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 07:10:58.000000 xenoslib-0.1.29.3/xenoslib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-20 07:10:58.000000 xenoslib-0.1.29.3/xenoslib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 07:10:58.000000 xenoslib-0.1.29.3/xenoslib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:34:54.284539 xenoslib-0.1.29.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-21 02:34:42.000000 xenoslib-0.1.29.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-21 02:34:54.284539 xenoslib-0.1.29.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-21 02:34:42.000000 xenoslib-0.1.29.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 02:34:54.284539 xenoslib-0.1.29.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-21 02:34:42.000000 xenoslib-0.1.29.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:34:54.284539 xenoslib-0.1.29.4/xenoslib/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-21 02:34:42.000000 xenoslib-0.1.29.4/xenoslib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-21 02:34:42.000000 xenoslib-0.1.29.4/xenoslib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-21 02:34:42.000000 xenoslib-0.1.29.4/xenoslib/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-06-21 02:34:42.000000 xenoslib-0.1.29.4/xenoslib/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-21 02:34:42.000000 xenoslib-0.1.29.4/xenoslib/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-06-21 02:34:42.000000 xenoslib-0.1.29.4/xenoslib/extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-21 02:34:42.000000 xenoslib-0.1.29.4/xenoslib/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-06-21 02:34:42.000000 xenoslib-0.1.29.4/xenoslib/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-21 02:34:42.000000 xenoslib-0.1.29.4/xenoslib/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-06-21 02:34:42.000000 xenoslib-0.1.29.4/xenoslib/onedrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-06-21 02:34:42.000000 xenoslib-0.1.29.4/xenoslib/win_trayicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-21 02:34:42.000000 xenoslib-0.1.29.4/xenoslib/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 02:34:54.284539 xenoslib-0.1.29.4/xenoslib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-21 02:34:54.000000 xenoslib-0.1.29.4/xenoslib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-21 02:34:54.000000 xenoslib-0.1.29.4/xenoslib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 02:34:54.000000 xenoslib-0.1.29.4/xenoslib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-21 02:34:54.000000 xenoslib-0.1.29.4/xenoslib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 02:34:54.000000 xenoslib-0.1.29.4/xenoslib.egg-info/top_level.txt
```

### Comparing `xenoslib-0.1.29.3/LICENSE` & `xenoslib-0.1.29.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.3/README.md` & `xenoslib-0.1.29.4/README.md`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.3/setup.py` & `xenoslib-0.1.29.4/setup.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.3/xenoslib/base.py` & `xenoslib-0.1.29.4/xenoslib/base.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.3/xenoslib/dev.py` & `xenoslib-0.1.29.4/xenoslib/dev.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.3/xenoslib/extend.py` & `xenoslib-0.1.29.4/xenoslib/extend.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.3/xenoslib/linux.py` & `xenoslib-0.1.29.4/xenoslib/linux.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.3/xenoslib/mail.py` & `xenoslib-0.1.29.4/xenoslib/mail.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
                 continue
             body = email.message_from_bytes(msg[b"BODY[]"])
             subject = str(email.header.make_header(email.header.decode_header(body["Subject"])))
 
             payload = body.get_payload(decode=True)
             if payload:
                 payload = payload.decode()
+            body["raw"] = msg[b"BODY[]"]
             body["subjectx"] = subject
             body["payload"] = payload
             body["internal_date"] = msg[b"INTERNALDATE"]
             yield body
             self.msg_ids.append(msg_id)
 
     def fetch_emails(self):
```

### Comparing `xenoslib-0.1.29.3/xenoslib/mock.py` & `xenoslib-0.1.29.4/xenoslib/mock.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.3/xenoslib/onedrive.py` & `xenoslib-0.1.29.4/xenoslib/onedrive.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.3/xenoslib/win_trayicon.py` & `xenoslib-0.1.29.4/xenoslib/win_trayicon.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.3/xenoslib/windows.py` & `xenoslib-0.1.29.4/xenoslib/windows.py`

 * *Files identical despite different names*

