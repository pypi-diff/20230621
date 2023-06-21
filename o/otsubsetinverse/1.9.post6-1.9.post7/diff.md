# Comparing `tmp/otsubsetinverse-1.9.post6-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/otsubsetinverse-1.9.post7-cp39-cp39-win_amd64.whl.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,22 +1,22 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                    313330 (000000000004C7F2h)
-  Actual end-cent-dir record offset:        313308 (000000000004C7DCh)
-  Expected end-cent-dir record offset:      313308 (000000000004C7DCh)
+  Zip archive file size:                    190410 (000000000002E7CAh)
+  Actual end-cent-dir record offset:        190388 (000000000002E7B4h)
+  Expected end-cent-dir record offset:      190388 (000000000002E7B4h)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 10 entries.
-  The central directory is 1040 (0000000000000410h) bytes long,
+  central directory contains 9 entries.
+  The central directory is 944 (00000000000003B0h) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 312268 (000000000004C3CCh).
+  is 189444 (000000000002E404h).
 
 
 Central directory entry #1:
 ---------------------------
 
   otsubsetinverse/
 
@@ -25,17 +25,17 @@
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Nov 8 17:00:04
-  file last modified on (UT extra field modtime): 2022 Nov 8 17:00:03 local
-  file last modified on (UT extra field modtime): 2022 Nov 8 17:00:03 UTC
+  file last modified on (DOS date/time):          2022 Nov 9 18:16:02
+  file last modified on (UT extra field modtime): 2022 Nov 9 18:16:02 local
+  file last modified on (UT extra field modtime): 2022 Nov 9 18:16:02 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             16 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -43,219 +43,183 @@
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
+    01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
 Central directory entry #2:
 ---------------------------
 
-  otsubsetinverse/_otsubsetinverse.so
+  otsubsetinverse/_otsubsetinverse.pyd
 
   offset of local header from start of archive:   74
                                                   (000000000000004Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Nov 8 17:00:04
-  file last modified on (UT extra field modtime): 2022 Nov 8 17:00:03 local
-  file last modified on (UT extra field modtime): 2022 Nov 8 17:00:03 UTC
-  32-bit CRC value (hex):                         8f68f44a
-  compressed size:                                186686 bytes
-  uncompressed size:                              986888 bytes
-  length of filename:                             35 characters
+  file last modified on (DOS date/time):          2022 Nov 9 18:16:02
+  file last modified on (UT extra field modtime): 2022 Nov 9 18:16:02 local
+  file last modified on (UT extra field modtime): 2022 Nov 9 18:16:02 UTC
+  32-bit CRC value (hex):                         c65e35af
+  compressed size:                                121080 bytes
+  uncompressed size:                              501710 bytes
+  length of filename:                             36 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (100755 octal):            -rwxr-xr-x
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
+    01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
 Central directory entry #3:
 ---------------------------
 
   otsubsetinverse/otsubsetinverse.py
 
-  offset of local header from start of archive:   186853
-                                                  (000000000002D9E5h) bytes
+  offset of local header from start of archive:   121248
+                                                  (000000000001D9A0h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Nov 8 16:59:52
-  file last modified on (UT extra field modtime): 2022 Nov 8 16:59:52 local
-  file last modified on (UT extra field modtime): 2022 Nov 8 16:59:52 UTC
-  32-bit CRC value (hex):                         c7bb6e5a
-  compressed size:                                3915 bytes
-  uncompressed size:                              16912 bytes
+  file last modified on (DOS date/time):          2022 Nov 9 18:15:50
+  file last modified on (UT extra field modtime): 2022 Nov 9 18:15:50 local
+  file last modified on (UT extra field modtime): 2022 Nov 9 18:15:50 UTC
+  32-bit CRC value (hex):                         45e8b2c2
+  compressed size:                                3960 bytes
+  uncompressed size:                              17010 bytes
   length of filename:                             34 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
+    01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
 Central directory entry #4:
 ---------------------------
 
-  otsubsetinverse/__init__.py
+  otsubsetinverse/libotsubsetinverse.dll
 
-  offset of local header from start of archive:   190860
-                                                  (000000000002E98Ch) bytes
+  offset of local header from start of archive:   125300
+                                                  (000000000001E974h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Nov 8 16:59:40
-  file last modified on (UT extra field modtime): 2022 Nov 8 16:59:39 local
-  file last modified on (UT extra field modtime): 2022 Nov 8 16:59:39 UTC
-  32-bit CRC value (hex):                         36c4fc32
-  compressed size:                                194 bytes
-  uncompressed size:                              333 bytes
-  length of filename:                             27 characters
+  file last modified on (DOS date/time):          2022 Nov 9 18:16:02
+  file last modified on (UT extra field modtime): 2022 Nov 9 18:16:02 local
+  file last modified on (UT extra field modtime): 2022 Nov 9 18:16:02 UTC
+  32-bit CRC value (hex):                         fb6f1c90
+  compressed size:                                62371 bytes
+  uncompressed size:                              181637 bytes
+  length of filename:                             38 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             binary
+  Unix file attributes (100755 octal):            -rwxr-xr-x
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
+    01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
 Central directory entry #5:
 ---------------------------
 
-  otsubsetinverse.libs/
-
-  offset of local header from start of archive:   191139
-                                                  (000000000002EAA3h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2022 Nov 8 17:00:04
-  file last modified on (UT extra field modtime): 2022 Nov 8 17:00:03 local
-  file last modified on (UT extra field modtime): 2022 Nov 8 17:00:03 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             21 characters
-  length of extra field:                          24 bytes
-  length of file comment:                         0 characters
-  disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
-  There is no file comment.
-
-Central directory entry #6:
----------------------------
-
-  otsubsetinverse.libs/libotsubsetinverse.so.0
+  otsubsetinverse/__init__.py
 
-  offset of local header from start of archive:   191218
-                                                  (000000000002EAF2h) bytes
+  offset of local header from start of archive:   187767
+                                                  (000000000002DD77h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Nov 8 17:00:04
-  file last modified on (UT extra field modtime): 2022 Nov 8 17:00:03 local
-  file last modified on (UT extra field modtime): 2022 Nov 8 17:00:03 UTC
-  32-bit CRC value (hex):                         39e62dea
-  compressed size:                                119601 bytes
-  uncompressed size:                              557960 bytes
-  length of filename:                             44 characters
+  file last modified on (DOS date/time):          2022 Nov 9 18:15:32
+  file last modified on (UT extra field modtime): 2022 Nov 9 18:15:31 local
+  file last modified on (UT extra field modtime): 2022 Nov 9 18:15:31 UTC
+  32-bit CRC value (hex):                         8e789b57
+  compressed size:                                194 bytes
+  uncompressed size:                              333 bytes
+  length of filename:                             27 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100755 octal):            -rwxr-xr-x
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
+    01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #7:
+Central directory entry #6:
 ---------------------------
 
-  otsubsetinverse-1.9.post6.dist-info/
+  otsubsetinverse-1.9.post7.dist-info/
 
-  offset of local header from start of archive:   310921
-                                                  (000000000004BE89h) bytes
+  offset of local header from start of archive:   188046
+                                                  (000000000002DE8Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Nov 8 17:00:04
-  file last modified on (UT extra field modtime): 2022 Nov 8 17:00:03 local
-  file last modified on (UT extra field modtime): 2022 Nov 8 17:00:03 UTC
+  file last modified on (DOS date/time):          2022 Nov 9 18:16:02
+  file last modified on (UT extra field modtime): 2022 Nov 9 18:16:02 local
+  file last modified on (UT extra field modtime): 2022 Nov 9 18:16:02 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             36 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -263,35 +227,35 @@
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
+    01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #8:
+Central directory entry #7:
 ---------------------------
 
-  otsubsetinverse-1.9.post6.dist-info/WHEEL
+  otsubsetinverse-1.9.post7.dist-info/WHEEL
 
-  offset of local header from start of archive:   311015
-                                                  (000000000004BEE7h) bytes
+  offset of local header from start of archive:   188140
+                                                  (000000000002DEECh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Nov 8 16:59:40
-  file last modified on (UT extra field modtime): 2022 Nov 8 16:59:39 local
-  file last modified on (UT extra field modtime): 2022 Nov 8 16:59:39 UTC
+  file last modified on (DOS date/time):          2022 Nov 9 18:15:38
+  file last modified on (UT extra field modtime): 2022 Nov 9 18:15:37 local
+  file last modified on (UT extra field modtime): 2022 Nov 9 18:15:37 UTC
   32-bit CRC value (hex):                         3917d65e
   compressed size:                                66 bytes
   uncompressed size:                              66 bytes
   length of filename:                             41 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -299,85 +263,85 @@
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
+    01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #9:
+Central directory entry #8:
 ---------------------------
 
-  otsubsetinverse-1.9.post6.dist-info/RECORD
+  otsubsetinverse-1.9.post7.dist-info/RECORD
 
-  offset of local header from start of archive:   311180
-                                                  (000000000004BF8Ch) bytes
+  offset of local header from start of archive:   188305
+                                                  (000000000002DF91h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Nov 8 17:00:04
-  file last modified on (UT extra field modtime): 2022 Nov 8 17:00:03 local
-  file last modified on (UT extra field modtime): 2022 Nov 8 17:00:03 UTC
-  32-bit CRC value (hex):                         6b6e7149
-  compressed size:                                314 bytes
-  uncompressed size:                              516 bytes
+  file last modified on (DOS date/time):          2022 Nov 9 18:16:02
+  file last modified on (UT extra field modtime): 2022 Nov 9 18:16:02 local
+  file last modified on (UT extra field modtime): 2022 Nov 9 18:16:02 UTC
+  32-bit CRC value (hex):                         f5f5396e
+  compressed size:                                365 bytes
+  uncompressed size:                              615 bytes
   length of filename:                             42 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
+    01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #10:
+Central directory entry #9:
 ---------------------------
 
-  otsubsetinverse-1.9.post6.dist-info/METADATA
+  otsubsetinverse-1.9.post7.dist-info/METADATA
 
-  offset of local header from start of archive:   311594
-                                                  (000000000004C12Ah) bytes
+  offset of local header from start of archive:   188770
+                                                  (000000000002E162h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Nov 8 16:59:40
-  file last modified on (UT extra field modtime): 2022 Nov 8 16:59:39 local
-  file last modified on (UT extra field modtime): 2022 Nov 8 16:59:39 UTC
-  32-bit CRC value (hex):                         15a92825
+  file last modified on (DOS date/time):          2022 Nov 9 18:15:38
+  file last modified on (UT extra field modtime): 2022 Nov 9 18:15:37 local
+  file last modified on (UT extra field modtime): 2022 Nov 9 18:15:37 UTC
+  32-bit CRC value (hex):                         569feb43
   compressed size:                                572 bytes
   uncompressed size:                              1679 bytes
   length of filename:                             44 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
+    01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
```

## zipnote {}

```diff
@@ -1,31 +1,28 @@
 Filename: otsubsetinverse/
 Comment: 
 
-Filename: otsubsetinverse/_otsubsetinverse.so
+Filename: otsubsetinverse/_otsubsetinverse.pyd
 Comment: 
 
 Filename: otsubsetinverse/otsubsetinverse.py
 Comment: 
 
-Filename: otsubsetinverse/__init__.py
-Comment: 
-
-Filename: otsubsetinverse.libs/
+Filename: otsubsetinverse/libotsubsetinverse.dll
 Comment: 
 
-Filename: otsubsetinverse.libs/libotsubsetinverse.so.0
+Filename: otsubsetinverse/__init__.py
 Comment: 
 
-Filename: otsubsetinverse-1.9.post6.dist-info/
+Filename: otsubsetinverse-1.9.post7.dist-info/
 Comment: 
 
-Filename: otsubsetinverse-1.9.post6.dist-info/WHEEL
+Filename: otsubsetinverse-1.9.post7.dist-info/WHEEL
 Comment: 
 
-Filename: otsubsetinverse-1.9.post6.dist-info/RECORD
+Filename: otsubsetinverse-1.9.post7.dist-info/RECORD
 Comment: 
 
-Filename: otsubsetinverse-1.9.post6.dist-info/METADATA
+Filename: otsubsetinverse-1.9.post7.dist-info/METADATA
 Comment: 
 
 Zip file comment:
```

## otsubsetinverse/otsubsetinverse.py

```diff
@@ -1,16 +1,19 @@
-# This file was automatically generated by SWIG (https://www.swig.org).
-# Version 4.1.0
+# This file was automatically generated by SWIG (http://www.swig.org).
+# Version 4.0.2
 #
-# Do not make changes to this file unless you know what you are doing - modify
+# Do not make changes to this file unless you know what you are doing--modify
 # the SWIG interface file instead.
 
 """otsubsetinverse module"""
 
 from sys import version_info as _swig_python_version_info
+if _swig_python_version_info < (2, 7, 0):
+    raise RuntimeError("Python 2.7 or later required")
+
 # Import the low-level C/C++ module
 if __package__ or "." in __name__:
     from . import _otsubsetinverse
 else:
     import _otsubsetinverse
 
 try:
@@ -24,18 +27,18 @@
     except __builtin__.Exception:
         strthis = ""
     return "<%s.%s; %s >" % (self.__class__.__module__, self.__class__.__name__, strthis,)
 
 
 def _swig_setattr_nondynamic_instance_variable(set):
     def set_instance_attr(self, name, value):
-        if name == "this":
-            set(self, name, value)
-        elif name == "thisown":
+        if name == "thisown":
             self.this.own(value)
+        elif name == "this":
+            set(self, name, value)
         elif hasattr(self, name) and isinstance(getattr(type(self), name), property):
             set(self, name, value)
         else:
             raise AttributeError("You cannot add instance attributes to %s" % self)
     return set_instance_attr
 
 
@@ -120,14 +123,15 @@
 
     def __init__(self, *args):
         _otsubsetinverse.SubsetInverseSamplingResult_swiginit(self, _otsubsetinverse.new_SubsetInverseSamplingResult(*args))
     __swig_destroy__ = _otsubsetinverse.delete_SubsetInverseSamplingResult
 
 # Register SubsetInverseSamplingResult in _otsubsetinverse:
 _otsubsetinverse.SubsetInverseSamplingResult_swigregister(SubsetInverseSamplingResult)
+
 class SubsetInverseSampling(openturns.simulation.EventSimulation):
     r"""
     Subset inverse simulation.
 
     Parameters
     ----------
     event : :class:`~openturns.Event`
@@ -528,7 +532,8 @@
 cvar = _otsubsetinverse.cvar
 SubsetInverseSampling.DefaultMaximumOuterSampling = _otsubsetinverse.cvar.SubsetInverseSampling_DefaultMaximumOuterSampling
 SubsetInverseSampling.DefaultProposalRange = _otsubsetinverse.cvar.SubsetInverseSampling_DefaultProposalRange
 SubsetInverseSampling.DefaultConditionalProbability = _otsubsetinverse.cvar.SubsetInverseSampling_DefaultConditionalProbability
 SubsetInverseSampling.DefaultBetaMin = _otsubsetinverse.cvar.SubsetInverseSampling_DefaultBetaMin
 
 
+
```

## otsubsetinverse/__init__.py

```diff
@@ -11,9 +11,9 @@
 import sys
 if sys.platform.startswith('win'):
     # this ensures OT dll is loaded
     import openturns
 
 from .otsubsetinverse import *
 
-__version__ = '1.9.post6'
+__version__ = '1.9.post7'
```

## Comparing `otsubsetinverse-1.9.post6.dist-info/METADATA` & `otsubsetinverse-1.9.post7.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: otsubsetinverse
-Version: 1.9.post6
+Version: 1.9.post7
 Summary: Inverse subset module
 Home-page:  http://www.openturns.org
 Author: OpenTURNS Developers
 Author-email: users@openturns.org
 License: LGPL
 Keywords: probability reliability sensitivity metamodel
 Platform: any
```

