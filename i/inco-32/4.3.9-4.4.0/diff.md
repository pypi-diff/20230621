# Comparing `tmp/inco_32-4.3.9.tar.gz` & `tmp/inco_32-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inco_32-4.3.9.tar", last modified: Wed Mar 15 14:04:42 2023, max compression
+gzip compressed data, was "inco_32-4.4.0.tar", last modified: Wed Jun 21 12:55:41 2023, max compression
```

## Comparing `inco_32-4.3.9.tar` & `inco_32-4.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-15 14:04:42.599439 inco_32-4.3.9/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1053 2020-11-30 10:14:07.000000 inco_32-4.3.9/LICENSE.txt
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      601 2021-06-15 13:14:13.000000 inco_32-4.3.9/MANIFEST.in
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2795 2023-03-15 14:04:42.599439 inco_32-4.3.9/PKG-INFO
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1593 2020-11-30 10:14:07.000000 inco_32-4.3.9/README.md
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      146 2020-11-30 10:14:07.000000 inco_32-4.3.9/pyproject.toml
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1173 2023-03-15 14:04:42.599439 inco_32-4.3.9/setup.cfg
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-15 14:04:42.595439 inco_32-4.3.9/src/
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-15 14:04:42.599439 inco_32-4.3.9/src/inco_32/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       46 2020-11-30 10:14:07.000000 inco_32-4.3.9/src/inco_32/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    31377 2023-03-15 14:04:42.000000 inco_32-4.3.9/src/inco_32/errinco.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    30768 2023-03-15 13:34:59.000000 inco_32-4.3.9/src/inco_32/inco_32.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-03-15 14:04:42.599439 inco_32-4.3.9/src/inco_32.egg-info/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2795 2023-03-15 14:04:42.000000 inco_32-4.3.9/src/inco_32.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      268 2023-03-15 14:04:42.000000 inco_32-4.3.9/src/inco_32.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        1 2023-03-15 14:04:42.000000 inco_32-4.3.9/src/inco_32.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        8 2023-03-15 14:04:42.000000 inco_32-4.3.9/src/inco_32.egg-info/top_level.txt
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-06-21 12:55:41.449985 inco_32-4.4.0/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1053 2020-11-30 10:14:07.000000 inco_32-4.4.0/LICENSE.txt
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      601 2021-06-15 13:14:13.000000 inco_32-4.4.0/MANIFEST.in
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2795 2023-06-21 12:55:41.449985 inco_32-4.4.0/PKG-INFO
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1593 2020-11-30 10:14:07.000000 inco_32-4.4.0/README.md
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      146 2020-11-30 10:14:07.000000 inco_32-4.4.0/pyproject.toml
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     1173 2023-06-21 12:55:41.449985 inco_32-4.4.0/setup.cfg
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-06-21 12:55:41.449985 inco_32-4.4.0/src/
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-06-21 12:55:41.449985 inco_32-4.4.0/src/inco_32/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       46 2020-11-30 10:14:07.000000 inco_32-4.4.0/src/inco_32/__init__.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    31489 2023-06-21 12:55:41.000000 inco_32-4.4.0/src/inco_32/errinco.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    31658 2023-06-21 12:49:37.000000 inco_32-4.4.0/src/inco_32/inco_32.py
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-06-21 12:55:41.449985 inco_32-4.4.0/src/inco_32.egg-info/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2795 2023-06-21 12:55:41.000000 inco_32-4.4.0/src/inco_32.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      268 2023-06-21 12:55:41.000000 inco_32-4.4.0/src/inco_32.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        1 2023-06-21 12:55:41.000000 inco_32-4.4.0/src/inco_32.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        8 2023-06-21 12:55:41.000000 inco_32-4.4.0/src/inco_32.egg-info/top_level.txt
```

### Comparing `inco_32-4.3.9/LICENSE.txt` & `inco_32-4.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `inco_32-4.3.9/MANIFEST.in` & `inco_32-4.4.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `inco_32-4.3.9/PKG-INFO` & `inco_32-4.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inco_32
-Version: 4.3.9
+Version: 4.4.0
 Summary: Python binding for libinco_32
 Home-page: https://gitlab.indel.ch/indel-public/python-inco_32
 Maintainer: C. Walther, Indel AG
 Maintainer-email: walther@indel.ch
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `inco_32-4.3.9/README.md` & `inco_32-4.4.0/README.md`

 * *Files identical despite different names*

### Comparing `inco_32-4.3.9/setup.cfg` & `inco_32-4.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `inco_32-4.3.9/src/inco_32/errinco.py` & `inco_32-4.4.0/src/inco_32/errinco.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,14 +289,15 @@
 ER_INCO_DT_DEVICE_UNSUPPORTED			= 0x00080005	# Data transfer error: This device type is not support
 ER_INCO_DT_METHOD_UNKONWN				= 0x00080006	# Data transfer error: This transfer method is unkown. Updating libinco_32 may fix the issue
 ER_INCO_DT_CONNECTING_REFUSED			= 0x00080007	# Data transfer error: Remote refused to connect
 ER_INCO_DT_TOO_MUCH_DATA					= 0x00080008	# Data transfer error: The remote cannot handle that much data
 ER_INCO_DT_BUFFER_TO_SMALL				= 0x00080009	# Data transfer error: The provided buffer size is to small. It must at least provide as much memory as defined by the datachannel
 ER_INCO_DT_LOCK_FAILED					= 0x0008000A	# Data transfer error: Failed to initialize lock
 ER_INCO_DT_LOCK_TIMEOUT					= 0x0008000B	# Data transfer error: Timeout while waiting for lock
+ER_INCO_DT_RETRY_OCCURRED				= 0x0008000C	# Data transfer error: Retransmission occurred (degraded performance)
 ER_SOCKET_OS_BASE                       = 0x00090000	# socket OS error base
 ER_SOCKET_APP_BASE                      = 0x00098000	# socket application error base
 ER_SOCKET_UNMAPPABLE_OS_ERROR           = 0x00098001	# unmappable OS error
 ER_SOCKET_CLOSED                        = 0x00098002	# socket is closed
 ER_SOCKET_TIMEOUT                       = 0x00098003	# socket timeout
 ER_SOCKET_TIMEOUT_RECV                  = 0x00098004	# socket receive timeout
 ER_SOCKET_TIMEOUT_SEND                  = 0x00098005	# socket send timeout
```

### Comparing `inco_32-4.3.9/src/inco_32/inco_32.py` & `inco_32-4.4.0/src/inco_32/inco_32.py`

 * *Files 3% similar despite different names*

```diff
@@ -139,14 +139,33 @@
 	return _stringFromInco(cBuffer.value)
 
 def GetMcMessage(aTargetName, aMessageHandlerPath='Target.message', auError=0):
 	buffer = create_string_buffer(1024)
 	error = _GetMcMessage(_stringToInco(aTargetName), _stringToInco(aMessageHandlerPath), auError, buffer, len(buffer))
 	return HandleError(error, _stringFromInco(buffer.value), '%s 0x%X' % (aMessageHandlerPath, auError), aTargetName)
 
+def GetRevisions(aTargetName):
+
+	# init revisions to magic number. this is necessary to get the "full" revision
+	# instead of a right-shifted-by-8 compatibility mode for "old" applications
+	uServerRevision = c_uint32(0xdeadbeef)
+	uDllRevision = c_uint32(0xdeadbeef)
+	
+	error = _GetRevisions(_stringToInco(aTargetName), byref(uServerRevision), byref(uDllRevision))
+	if error != 0:
+		raise INCOError(error, aPathInformation="GetRevisions", aTarget=aTargetName)	
+	
+	# convert to string
+	x = uServerRevision.value
+	sServerRevision = "%d.%d.%d" % ((x >> 16) & 0xFFFF, (x >> 8) & 0xFF, x & 0xFF)
+	x = uDllRevision.value
+	sDllRevision = "%d.%d.%d" % ((x >> 16) & 0xFFFF, (x >> 8) & 0xFF, x & 0xFF)
+	
+	return sServerRevision, sDllRevision
+
 
 #-------------------------------------------------------------------------------
 # API functions
 #-------------------------------------------------------------------------------
 #
 #  V a r i a b l e
 #
@@ -661,14 +680,18 @@
 #
 # Error Messages
 _GetErrorDescription = UseClass.__getattr__(LibraryLocation).GetErrorDescription;
 _GetErrorDescription.argtypes = [ c_char_p, c_uint32, c_char_p, c_uint32 ]
 _GetMcMessage = UseClass.__getattr__(LibraryLocation).GetMcMessage;
 _GetMcMessage.argtypes = [ c_char_p, c_char_p, c_uint32, c_char_p, c_uint32 ]
 #
+# Revisions
+_GetRevisions = UseClass.__getattr__(LibraryLocation).GetRevisions;
+_GetRevisions.argtypes = [ c_char_p, POINTER(c_uint32), POINTER(c_uint32) ]
+#
 # GetBlock
 _GetBlock8 = UseClass.__getattr__(LibraryLocation).GetBlock8
 _GetBlock8.argtypes = [ c_char_p, c_uint32, c_char_p, c_uint32 ]
 _GetBlock16 = UseClass.__getattr__(LibraryLocation).GetBlock16
 _GetBlock16.argtypes = [ c_char_p, c_uint32, c_char_p, c_uint32 ]
 _GetBlock32 = UseClass.__getattr__(LibraryLocation).GetBlock32
 _GetBlock32.argtypes = [ c_char_p, c_uint32, c_char_p, c_uint32 ]
```

### Comparing `inco_32-4.3.9/src/inco_32.egg-info/PKG-INFO` & `inco_32-4.4.0/src/inco_32.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inco-32
-Version: 4.3.9
+Version: 4.4.0
 Summary: Python binding for libinco_32
 Home-page: https://gitlab.indel.ch/indel-public/python-inco_32
 Maintainer: C. Walther, Indel AG
 Maintainer-email: walther@indel.ch
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

