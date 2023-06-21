# Comparing `tmp/otmixmod-0.13.post7-cp39-cp39-win_amd64.whl.zip` & `tmp/otmixmod-0.14-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,22 +1,22 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                    585768 (000000000008F028h)
-  Actual end-cent-dir record offset:        585746 (000000000008F012h)
-  Expected end-cent-dir record offset:      585746 (000000000008F012h)
+  Zip archive file size:                    765632 (00000000000BAEC0h)
+  Actual end-cent-dir record offset:        765610 (00000000000BAEAAh)
+  Expected end-cent-dir record offset:      765610 (00000000000BAEAAh)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 9 entries.
-  The central directory is 864 (0000000000000360h) bytes long,
+  central directory contains 10 entries.
+  The central directory is 929 (00000000000003A1h) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 584882 (000000000008ECB2h).
+  is 764681 (00000000000BAB09h).
 
 
 Central directory entry #1:
 ---------------------------
 
   otmixmod/
 
@@ -25,17 +25,17 @@
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Nov 9 18:12:58
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:12:57 local
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:12:57 UTC
+  file last modified on (DOS date/time):          2023 Jun 21 11:40:02
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:40:02 local
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:40:02 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             9 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -43,305 +43,341 @@
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 00 00 00 00 04 00 00 00 00.
 
   There is no file comment.
 
 Central directory entry #2:
 ---------------------------
 
-  otmixmod/otmixmod.py
+  otmixmod/__init__.py
 
   offset of local header from start of archive:   67
                                                   (0000000000000043h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Nov 9 18:12:04
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:12:03 local
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:12:03 UTC
-  32-bit CRC value (hex):                         2c1ee859
-  compressed size:                                2013 bytes
-  uncompressed size:                              8475 bytes
+  file last modified on (DOS date/time):          2023 Jun 21 11:39:14
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:39:13 local
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:39:13 UTC
+  32-bit CRC value (hex):                         f08309c2
+  compressed size:                                229 bytes
+  uncompressed size:                              402 bytes
   length of filename:                             20 characters
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
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 00 00 00 00 04 00 00 00 00.
 
   There is no file comment.
 
 Central directory entry #3:
 ---------------------------
 
-  otmixmod/_otmixmod.pyd
+  otmixmod/_otmixmod.so
 
-  offset of local header from start of archive:   2158
-                                                  (000000000000086Eh) bytes
+  offset of local header from start of archive:   374
+                                                  (0000000000000176h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Nov 9 18:12:58
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:12:57 local
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:12:57 UTC
-  32-bit CRC value (hex):                         f1d79586
-  compressed size:                                138188 bytes
-  uncompressed size:                              535441 bytes
-  length of filename:                             22 characters
+  file last modified on (DOS date/time):          2023 Jun 21 11:40:02
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:40:02 local
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:40:02 UTC
+  32-bit CRC value (hex):                         d5aaced6
+  compressed size:                                208258 bytes
+  uncompressed size:                              1058849 bytes
+  length of filename:                             21 characters
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
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 00 00 00 00 04 00 00 00 00.
 
   There is no file comment.
 
 Central directory entry #4:
 ---------------------------
 
-  otmixmod/libotmixmod.dll
+  otmixmod/otmixmod.py
 
-  offset of local header from start of archive:   140426
-                                                  (000000000002248Ah) bytes
+  offset of local header from start of archive:   208711
+                                                  (0000000000032F47h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Nov 9 18:12:58
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:12:57 local
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:12:57 UTC
-  32-bit CRC value (hex):                         3a82ced8
-  compressed size:                                442692 bytes
-  uncompressed size:                              1153632 bytes
-  length of filename:                             24 characters
+  file last modified on (DOS date/time):          2023 Jun 21 11:39:26
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:39:26 local
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:39:26 UTC
+  32-bit CRC value (hex):                         6789ab64
+  compressed size:                                1948 bytes
+  uncompressed size:                              8112 bytes
+  length of filename:                             20 characters
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
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 00 00 00 00 04 00 00 00 00.
 
   There is no file comment.
 
 Central directory entry #5:
 ---------------------------
 
-  otmixmod/__init__.py
+  otmixmod.libs/
+
+  offset of local header from start of archive:   210737
+                                                  (0000000000033731h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 Jun 21 11:40:02
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:40:02 local
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:40:02 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             14 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 00 00 00 00 04 00 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #6:
+---------------------------
+
+  otmixmod.libs/libotmixmod.so.0
 
-  offset of local header from start of archive:   583200
-                                                  (000000000008E620h) bytes
+  offset of local header from start of archive:   210809
+                                                  (0000000000033779h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Nov 9 18:11:44
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:11:44 local
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:11:44 UTC
-  32-bit CRC value (hex):                         3d9897ec
-  compressed size:                                240 bytes
-  uncompressed size:                              427 bytes
-  length of filename:                             20 characters
+  file last modified on (DOS date/time):          2023 Jun 21 11:40:02
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:40:02 local
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:40:02 UTC
+  32-bit CRC value (hex):                         634154f0
+  compressed size:                                552511 bytes
+  uncompressed size:                              1921217 bytes
+  length of filename:                             30 characters
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
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 00 00 00 00 04 00 00 00 00.
 
   There is no file comment.
 
-Central directory entry #6:
+Central directory entry #7:
 ---------------------------
 
-  otmixmod-0.13.post7.dist-info/
+  otmixmod-0.14.dist-info/
 
-  offset of local header from start of archive:   583518
-                                                  (000000000008E75Eh) bytes
+  offset of local header from start of archive:   763408
+                                                  (00000000000BA610h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Nov 9 18:12:58
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:12:57 local
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:12:57 UTC
+  file last modified on (DOS date/time):          2023 Jun 21 11:40:02
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:40:02 local
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:40:02 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             30 characters
+  length of filename:                             24 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 00 00 00 00 04 00 00 00 00.
 
   There is no file comment.
 
-Central directory entry #7:
+Central directory entry #8:
 ---------------------------
 
-  otmixmod-0.13.post7.dist-info/WHEEL
+  otmixmod-0.14.dist-info/METADATA
 
-  offset of local header from start of archive:   583606
-                                                  (000000000008E7B6h) bytes
+  offset of local header from start of archive:   763490
+                                                  (00000000000BA662h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Nov 9 18:11:50
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:11:50 local
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:11:50 UTC
-  32-bit CRC value (hex):                         3917d65e
-  compressed size:                                66 bytes
-  uncompressed size:                              66 bytes
-  length of filename:                             35 characters
+  file last modified on (DOS date/time):          2023 Jun 21 11:39:14
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:39:14 local
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:39:14 UTC
+  32-bit CRC value (hex):                         3330f9ac
+  compressed size:                                564 bytes
+  uncompressed size:                              1641 bytes
+  length of filename:                             32 characters
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
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 00 00 00 00 04 00 00 00 00.
 
   There is no file comment.
 
-Central directory entry #8:
+Central directory entry #9:
 ---------------------------
 
-  otmixmod-0.13.post7.dist-info/RECORD
+  otmixmod-0.14.dist-info/WHEEL
 
-  offset of local header from start of archive:   583765
-                                                  (000000000008E855h) bytes
+  offset of local header from start of archive:   764144
+                                                  (00000000000BA8F0h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Nov 9 18:12:58
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:12:57 local
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:12:57 UTC
-  32-bit CRC value (hex):                         c468314e
-  compressed size:                                358 bytes
-  uncompressed size:                              548 bytes
-  length of filename:                             36 characters
+  file last modified on (DOS date/time):          2023 Jun 21 11:39:14
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:39:14 local
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:39:14 UTC
+  32-bit CRC value (hex):                         3917d65e
+  compressed size:                                66 bytes
+  uncompressed size:                              66 bytes
+  length of filename:                             29 characters
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
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 00 00 00 00 04 00 00 00 00.
 
   There is no file comment.
 
-Central directory entry #9:
+Central directory entry #10:
 ---------------------------
 
-  otmixmod-0.13.post7.dist-info/METADATA
+  otmixmod-0.14.dist-info/RECORD
 
-  offset of local header from start of archive:   584217
-                                                  (000000000008EA19h) bytes
+  offset of local header from start of archive:   764297
+                                                  (00000000000BA989h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Nov 9 18:11:50
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:11:50 local
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:11:50 UTC
-  32-bit CRC value (hex):                         833c1833
-  compressed size:                                569 bytes
-  uncompressed size:                              1647 bytes
-  length of filename:                             38 characters
+  file last modified on (DOS date/time):          2023 Jun 21 11:40:02
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:40:02 local
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:40:02 UTC
+  32-bit CRC value (hex):                         0d8e2501
+  compressed size:                                296 bytes
+  uncompressed size:                              444 bytes
+  length of filename:                             30 characters
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
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 00 00 00 00 04 00 00 00 00.
 
   There is no file comment.
```

## zipnote {}

```diff
@@ -1,28 +1,31 @@
 Filename: otmixmod/
 Comment: 
 
-Filename: otmixmod/otmixmod.py
+Filename: otmixmod/__init__.py
+Comment: 
+
+Filename: otmixmod/_otmixmod.so
 Comment: 
 
-Filename: otmixmod/_otmixmod.pyd
+Filename: otmixmod/otmixmod.py
 Comment: 
 
-Filename: otmixmod/libotmixmod.dll
+Filename: otmixmod.libs/
 Comment: 
 
-Filename: otmixmod/__init__.py
+Filename: otmixmod.libs/libotmixmod.so.0
 Comment: 
 
-Filename: otmixmod-0.13.post7.dist-info/
+Filename: otmixmod-0.14.dist-info/
 Comment: 
 
-Filename: otmixmod-0.13.post7.dist-info/WHEEL
+Filename: otmixmod-0.14.dist-info/METADATA
 Comment: 
 
-Filename: otmixmod-0.13.post7.dist-info/RECORD
+Filename: otmixmod-0.14.dist-info/WHEEL
 Comment: 
 
-Filename: otmixmod-0.13.post7.dist-info/METADATA
+Filename: otmixmod-0.14.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## otmixmod/otmixmod.py

```diff
@@ -1,19 +1,16 @@
-# This file was automatically generated by SWIG (http://www.swig.org).
-# Version 4.0.2
+# This file was automatically generated by SWIG (https://www.swig.org).
+# Version 4.1.1
 #
-# Do not make changes to this file unless you know what you are doing--modify
+# Do not make changes to this file unless you know what you are doing - modify
 # the SWIG interface file instead.
 
 """otmixmod module"""
 
 from sys import version_info as _swig_python_version_info
-if _swig_python_version_info < (2, 7, 0):
-    raise RuntimeError("Python 2.7 or later required")
-
 # Import the low-level C/C++ module
 if __package__ or "." in __name__:
     from . import _otmixmod
 else:
     import _otmixmod
 
 try:
@@ -27,18 +24,18 @@
     except __builtin__.Exception:
         strthis = ""
     return "<%s.%s; %s >" % (self.__class__.__module__, self.__class__.__name__, strthis,)
 
 
 def _swig_setattr_nondynamic_instance_variable(set):
     def set_instance_attr(self, name, value):
-        if name == "thisown":
-            self.this.own(value)
-        elif name == "this":
+        if name == "this":
             set(self, name, value)
+        elif name == "thisown":
+            self.this.own(value)
         elif hasattr(self, name) and isinstance(getattr(type(self), name), property):
             set(self, name, value)
         else:
             raise AttributeError("You cannot add instance attributes to %s" % self)
     return set_instance_attr
 
 
@@ -173,19 +170,14 @@
         __init__(MixtureFactory self, MixtureFactory other) -> MixtureFactory
         """
         _otmixmod.MixtureFactory_swiginit(self, _otmixmod.new_MixtureFactory(*args))
     __swig_destroy__ = _otmixmod.delete_MixtureFactory
 
 # Register MixtureFactory in _otmixmod:
 _otmixmod.MixtureFactory_swigregister(MixtureFactory)
-
-def MixtureFactory_BuildClusters(data, labels, nbClusters):
-    r"""MixtureFactory_BuildClusters(Sample data, Indices labels, OT::UnsignedInteger const nbClusters) -> SampleCollection"""
-    return _otmixmod.MixtureFactory_BuildClusters(data, labels, nbClusters)
-
 class MixtureClassifierFactory(openturns.common.Object):
     r"""Proxy of C++ OTMIXMOD::MixtureClassifierFactory class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
 
     def getClassName(self):
@@ -220,9 +212,7 @@
         """
         _otmixmod.MixtureClassifierFactory_swiginit(self, _otmixmod.new_MixtureClassifierFactory(*args))
     __swig_destroy__ = _otmixmod.delete_MixtureClassifierFactory
 
 # Register MixtureClassifierFactory in _otmixmod:
 _otmixmod.MixtureClassifierFactory_swigregister(MixtureClassifierFactory)
 
-
-
```

## otmixmod/__init__.py

```diff
@@ -5,15 +5,15 @@
     Contents
     --------
       'otmixmod' is a python module for Open TURNS that allows to use
       the Mixmod software to build Open TURNS objects.
 
 """
 
-import sys
-if sys.platform.startswith('win'):
-    # this ensures OT dll is loaded
-    import openturns
+# flake8: noqa
+
+# ensures swig type tables order & dll load
+import openturns as _ot
 
 from .otmixmod import *
 
-__version__ = '0.13.post7'
+__version__ = '0.14'
```

## Comparing `otmixmod-0.13.post7.dist-info/METADATA` & `otmixmod-0.14.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: otmixmod
-Version: 0.13.post7
+Version: 0.14
 Summary: Mixmod module
 Home-page:  http://www.openturns.org
 Author: OpenTURNS Developers
 Author-email: users@openturns.org
 License: LGPL
 Keywords: probability reliability sensitivity metamodel
 Platform: any
```

