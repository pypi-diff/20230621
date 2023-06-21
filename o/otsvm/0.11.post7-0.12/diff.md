# Comparing `tmp/otsvm-0.11.post7-cp39-cp39-win_amd64.whl.zip` & `tmp/otsvm-0.12-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,22 +1,22 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                    439889 (000000000006B651h)
-  Actual end-cent-dir record offset:        439867 (000000000006B63Bh)
-  Expected end-cent-dir record offset:      439867 (000000000006B63Bh)
+  Zip archive file size:                    596562 (0000000000091A52h)
+  Actual end-cent-dir record offset:        596540 (0000000000091A3Ch)
+  Expected end-cent-dir record offset:      596540 (0000000000091A3Ch)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 9 entries.
-  The central directory is 828 (000000000000033Ch) bytes long,
+  central directory contains 10 entries.
+  The central directory is 890 (000000000000037Ah) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 439039 (000000000006B2FFh).
+  is 595650 (00000000000916C2h).
 
 
 Central directory entry #1:
 ---------------------------
 
   otsvm/
 
@@ -25,17 +25,17 @@
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Nov 9 18:17:12
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:17:11 local
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:17:11 UTC
+  file last modified on (DOS date/time):          2023 Jun 21 11:43:14
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:43:13 local
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:43:13 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             6 characters
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
 
-  otsvm/_otsvm.pyd
+  otsvm/__init__.py
 
   offset of local header from start of archive:   64
                                                   (0000000000000040h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Nov 9 18:17:12
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:17:11 local
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:17:11 UTC
-  32-bit CRC value (hex):                         260430f7
-  compressed size:                                242866 bytes
-  uncompressed size:                              947545 bytes
-  length of filename:                             16 characters
+  file last modified on (DOS date/time):          2023 Jun 21 11:42:14
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:42:13 local
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:42:13 UTC
+  32-bit CRC value (hex):                         09eda088
+  compressed size:                                324 bytes
+  uncompressed size:                              613 bytes
+  length of filename:                             17 characters
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
 
 Central directory entry #3:
 ---------------------------
 
   otsvm/otsvm.py
 
-  offset of local header from start of archive:   243004
-                                                  (000000000003B53Ch) bytes
+  offset of local header from start of archive:   463
+                                                  (00000000000001CFh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Nov 9 18:16:22
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:16:22 local
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:16:22 UTC
-  32-bit CRC value (hex):                         9bf4c79a
-  compressed size:                                4790 bytes
-  uncompressed size:                              35765 bytes
+  file last modified on (DOS date/time):          2023 Jun 21 11:42:42
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:42:41 local
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:42:41 UTC
+  32-bit CRC value (hex):                         ab261b52
+  compressed size:                                4899 bytes
+  uncompressed size:                              36320 bytes
   length of filename:                             14 characters
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
 
 Central directory entry #4:
 ---------------------------
 
-  otsvm/libotsvm.dll
+  otsvm/_otsvm.so
 
-  offset of local header from start of archive:   247866
-                                                  (000000000003C83Ah) bytes
+  offset of local header from start of archive:   5434
+                                                  (000000000000153Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Nov 9 18:17:12
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:17:11 local
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:17:11 UTC
-  32-bit CRC value (hex):                         20cec5a9
-  compressed size:                                189338 bytes
-  uncompressed size:                              543468 bytes
-  length of filename:                             18 characters
+  file last modified on (DOS date/time):          2023 Jun 21 11:43:14
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:43:13 local
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:43:13 UTC
+  32-bit CRC value (hex):                         6f906be2
+  compressed size:                                337493 bytes
+  uncompressed size:                              1552729 bytes
+  length of filename:                             15 characters
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
 
 Central directory entry #5:
 ---------------------------
 
-  otsvm/__init__.py
+  otsvm.libs/
 
-  offset of local header from start of archive:   437280
-                                                  (000000000006AC20h) bytes
+  offset of local header from start of archive:   343000
+                                                  (0000000000053BD8h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 Jun 21 11:43:14
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:43:13 local
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:43:13 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             11 characters
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
+  otsvm.libs/libotsvm.so.0
+
+  offset of local header from start of archive:   343069
+                                                  (0000000000053C1Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Nov 9 18:16:02
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:16:02 local
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:16:02 UTC
-  32-bit CRC value (hex):                         d1d40478
-  compressed size:                                337 bytes
-  uncompressed size:                              638 bytes
-  length of filename:                             17 characters
+  file last modified on (DOS date/time):          2023 Jun 21 11:43:14
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:43:13 local
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:43:13 UTC
+  32-bit CRC value (hex):                         68de49b4
+  compressed size:                                251232 bytes
+  uncompressed size:                              998001 bytes
+  length of filename:                             24 characters
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
 
-  otsvm-0.11.post7.dist-info/
+  otsvm-0.12.dist-info/
 
-  offset of local header from start of archive:   437692
-                                                  (000000000006ADBCh) bytes
+  offset of local header from start of archive:   594383
+                                                  (00000000000911CFh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Nov 9 18:17:12
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:17:11 local
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:17:11 UTC
+  file last modified on (DOS date/time):          2023 Jun 21 11:43:14
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:43:13 local
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:43:13 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             27 characters
+  length of filename:                             21 characters
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
 
-  otsvm-0.11.post7.dist-info/WHEEL
+  otsvm-0.12.dist-info/METADATA
 
-  offset of local header from start of archive:   437777
-                                                  (000000000006AE11h) bytes
+  offset of local header from start of archive:   594462
+                                                  (000000000009121Eh) bytes
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
-  file last modified on (DOS date/time):          2022 Nov 9 18:16:08
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:16:08 local
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:16:08 UTC
-  32-bit CRC value (hex):                         3917d65e
-  compressed size:                                66 bytes
-  uncompressed size:                              66 bytes
-  length of filename:                             32 characters
+  file last modified on (DOS date/time):          2023 Jun 21 11:42:14
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:42:14 local
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:42:14 UTC
+  32-bit CRC value (hex):                         dcf7d9aa
+  compressed size:                                568 bytes
+  uncompressed size:                              1651 bytes
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
 
-Central directory entry #8:
+Central directory entry #9:
 ---------------------------
 
-  otsvm-0.11.post7.dist-info/RECORD
+  otsvm-0.12.dist-info/WHEEL
 
-  offset of local header from start of archive:   437933
-                                                  (000000000006AEADh) bytes
+  offset of local header from start of archive:   595117
+                                                  (00000000000914ADh) bytes
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
-  file last modified on (DOS date/time):          2022 Nov 9 18:17:12
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:17:11 local
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:17:11 UTC
-  32-bit CRC value (hex):                         97e3c942
-  compressed size:                                350 bytes
-  uncompressed size:                              518 bytes
-  length of filename:                             33 characters
+  file last modified on (DOS date/time):          2023 Jun 21 11:42:14
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:42:14 local
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:42:14 UTC
+  32-bit CRC value (hex):                         3917d65e
+  compressed size:                                66 bytes
+  uncompressed size:                              66 bytes
+  length of filename:                             26 characters
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
 
-  otsvm-0.11.post7.dist-info/METADATA
+  otsvm-0.12.dist-info/RECORD
 
-  offset of local header from start of archive:   438374
-                                                  (000000000006B066h) bytes
+  offset of local header from start of archive:   595267
+                                                  (0000000000091543h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Nov 9 18:16:08
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:16:08 local
-  file last modified on (UT extra field modtime): 2022 Nov 9 18:16:08 UTC
-  32-bit CRC value (hex):                         d0438d9f
-  compressed size:                                572 bytes
-  uncompressed size:                              1657 bytes
-  length of filename:                             35 characters
+  file last modified on (DOS date/time):          2023 Jun 21 11:43:14
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:43:13 local
+  file last modified on (UT extra field modtime): 2023 Jun 21 11:43:13 UTC
+  32-bit CRC value (hex):                         657146d5
+  compressed size:                                298 bytes
+  uncompressed size:                              422 bytes
+  length of filename:                             27 characters
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
 Filename: otsvm/
 Comment: 
 
-Filename: otsvm/_otsvm.pyd
+Filename: otsvm/__init__.py
 Comment: 
 
 Filename: otsvm/otsvm.py
 Comment: 
 
-Filename: otsvm/libotsvm.dll
+Filename: otsvm/_otsvm.so
 Comment: 
 
-Filename: otsvm/__init__.py
+Filename: otsvm.libs/
+Comment: 
+
+Filename: otsvm.libs/libotsvm.so.0
 Comment: 
 
-Filename: otsvm-0.11.post7.dist-info/
+Filename: otsvm-0.12.dist-info/
 Comment: 
 
-Filename: otsvm-0.11.post7.dist-info/WHEEL
+Filename: otsvm-0.12.dist-info/METADATA
 Comment: 
 
-Filename: otsvm-0.11.post7.dist-info/RECORD
+Filename: otsvm-0.12.dist-info/WHEEL
 Comment: 
 
-Filename: otsvm-0.11.post7.dist-info/METADATA
+Filename: otsvm-0.12.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## otsvm/otsvm.py

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
 
 """otsvm module"""
 
 from sys import version_info as _swig_python_version_info
-if _swig_python_version_info < (2, 7, 0):
-    raise RuntimeError("Python 2.7 or later required")
-
 # Import the low-level C/C++ module
 if __package__ or "." in __name__:
     from . import _otsvm
 else:
     import _otsvm
 
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
 
 
@@ -131,15 +128,14 @@
 
     def __init__(self, *args):
         _otsvm.SVMKernelImplementation_swiginit(self, _otsvm.new_SVMKernelImplementation(*args))
     __swig_destroy__ = _otsvm.delete_SVMKernelImplementation
 
 # Register SVMKernelImplementation in _otsvm:
 _otsvm.SVMKernelImplementation_swigregister(SVMKernelImplementation)
-
 class SVMKernelImplementationTypedInterfaceObject(openturns.common.InterfaceObject):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
 
     def __init__(self, *args):
         _otsvm.SVMKernelImplementationTypedInterfaceObject_swiginit(self, _otsvm.new_SVMKernelImplementationTypedInterfaceObject(*args))
 
@@ -181,15 +177,14 @@
 
     def __ne__(self, other):
         return _otsvm.SVMKernelImplementationTypedInterfaceObject___ne__(self, other)
     __swig_destroy__ = _otsvm.delete_SVMKernelImplementationTypedInterfaceObject
 
 # Register SVMKernelImplementationTypedInterfaceObject in _otsvm:
 _otsvm.SVMKernelImplementationTypedInterfaceObject_swigregister(SVMKernelImplementationTypedInterfaceObject)
-
 class SVMKernel(SVMKernelImplementationTypedInterfaceObject):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
 
     @staticmethod
     def GetClassName():
         return _otsvm.SVMKernel_GetClassName()
 
@@ -225,18 +220,14 @@
 
     def __init__(self, *args):
         _otsvm.SVMKernel_swiginit(self, _otsvm.new_SVMKernel(*args))
     __swig_destroy__ = _otsvm.delete_SVMKernel
 
 # Register SVMKernel in _otsvm:
 _otsvm.SVMKernel_swigregister(SVMKernel)
-
-def SVMKernel_GetClassName():
-    return _otsvm.SVMKernel_GetClassName()
-
 class NormalRBF(SVMKernelImplementation):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
 
     def getClassName(self):
         r"""
         Accessor to the object's name.
 
@@ -279,15 +270,14 @@
 
     def __init__(self, *args):
         _otsvm.NormalRBF_swiginit(self, _otsvm.new_NormalRBF(*args))
     __swig_destroy__ = _otsvm.delete_NormalRBF
 
 # Register NormalRBF in _otsvm:
 _otsvm.NormalRBF_swigregister(NormalRBF)
-
 class ExponentialRBF(SVMKernelImplementation):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
 
     def getClassName(self):
         r"""
         Accessor to the object's name.
 
@@ -330,15 +320,14 @@
 
     def __init__(self, *args):
         _otsvm.ExponentialRBF_swiginit(self, _otsvm.new_ExponentialRBF(*args))
     __swig_destroy__ = _otsvm.delete_ExponentialRBF
 
 # Register ExponentialRBF in _otsvm:
 _otsvm.ExponentialRBF_swigregister(ExponentialRBF)
-
 class RationalKernel(SVMKernelImplementation):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
 
     def getClassName(self):
         r"""
         Accessor to the object's name.
 
@@ -381,15 +370,14 @@
 
     def __init__(self, *args):
         _otsvm.RationalKernel_swiginit(self, _otsvm.new_RationalKernel(*args))
     __swig_destroy__ = _otsvm.delete_RationalKernel
 
 # Register RationalKernel in _otsvm:
 _otsvm.RationalKernel_swigregister(RationalKernel)
-
 class PolynomialKernel(SVMKernelImplementation):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
 
     def getClassName(self):
         r"""
         Accessor to the object's name.
 
@@ -444,15 +432,14 @@
 
     def __init__(self, *args):
         _otsvm.PolynomialKernel_swiginit(self, _otsvm.new_PolynomialKernel(*args))
     __swig_destroy__ = _otsvm.delete_PolynomialKernel
 
 # Register PolynomialKernel in _otsvm:
 _otsvm.PolynomialKernel_swigregister(PolynomialKernel)
-
 class SigmoidKernel(SVMKernelImplementation):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
 
     def getClassName(self):
         r"""
         Accessor to the object's name.
 
@@ -495,15 +482,14 @@
 
     def __init__(self, *args):
         _otsvm.SigmoidKernel_swiginit(self, _otsvm.new_SigmoidKernel(*args))
     __swig_destroy__ = _otsvm.delete_SigmoidKernel
 
 # Register SigmoidKernel in _otsvm:
 _otsvm.SigmoidKernel_swigregister(SigmoidKernel)
-
 class LinearKernel(SVMKernelImplementation):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
 
     def getClassName(self):
         r"""
         Accessor to the object's name.
 
@@ -528,15 +514,14 @@
 
     def __init__(self, *args):
         _otsvm.LinearKernel_swiginit(self, _otsvm.new_LinearKernel(*args))
     __swig_destroy__ = _otsvm.delete_LinearKernel
 
 # Register LinearKernel in _otsvm:
 _otsvm.LinearKernel_swigregister(LinearKernel)
-
 class LibSVM(openturns.common.PersistentObject):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
 
     def getClassName(self):
         r"""
         Accessor to the object's name.
@@ -659,18 +644,14 @@
 
     def __init__(self, *args):
         _otsvm.LibSVM_swiginit(self, _otsvm.new_LibSVM(*args))
     __swig_destroy__ = _otsvm.delete_LibSVM
 
 # Register LibSVM in _otsvm:
 _otsvm.LibSVM_swigregister(LibSVM)
-
-def LibSVM_SVMLog(arg1):
-    return _otsvm.LibSVM_SVMLog(arg1)
-
 class SVMRegressionImplementationdInterfaceObject(openturns.common.InterfaceObject):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
 
     def __init__(self, *args):
         _otsvm.SVMRegressionImplementationdInterfaceObject_swiginit(self, _otsvm.new_SVMRegressionImplementationdInterfaceObject(*args))
 
@@ -712,15 +693,14 @@
 
     def __ne__(self, other):
         return _otsvm.SVMRegressionImplementationdInterfaceObject___ne__(self, other)
     __swig_destroy__ = _otsvm.delete_SVMRegressionImplementationdInterfaceObject
 
 # Register SVMRegressionImplementationdInterfaceObject in _otsvm:
 _otsvm.SVMRegressionImplementationdInterfaceObject_swigregister(SVMRegressionImplementationdInterfaceObject)
-
 class SVMRegressionImplementation(openturns.common.PersistentObject):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
 
     def getClassName(self):
         r"""
         Accessor to the object's name.
@@ -752,15 +732,14 @@
 
     def __init__(self, *args):
         _otsvm.SVMRegressionImplementation_swiginit(self, _otsvm.new_SVMRegressionImplementation(*args))
     __swig_destroy__ = _otsvm.delete_SVMRegressionImplementation
 
 # Register SVMRegressionImplementation in _otsvm:
 _otsvm.SVMRegressionImplementation_swigregister(SVMRegressionImplementation)
-
 class SVMRegression(SVMRegressionImplementationdInterfaceObject):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
 
     @staticmethod
     def GetClassName():
         return _otsvm.SVMRegression_GetClassName()
@@ -788,18 +767,14 @@
 
     def __init__(self, *args):
         _otsvm.SVMRegression_swiginit(self, _otsvm.new_SVMRegression(*args))
     __swig_destroy__ = _otsvm.delete_SVMRegression
 
 # Register SVMRegression in _otsvm:
 _otsvm.SVMRegression_swigregister(SVMRegression)
-
-def SVMRegression_GetClassName():
-    return _otsvm.SVMRegression_GetClassName()
-
 class LibSVMRegression(SVMRegressionImplementation):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
 
     def getClassName(self):
         r"""
         Accessor to the object's name.
@@ -822,16 +797,15 @@
 
     def __init__(self, *args):
         _otsvm.LibSVMRegression_swiginit(self, _otsvm.new_LibSVMRegression(*args))
     __swig_destroy__ = _otsvm.delete_LibSVMRegression
 
 # Register LibSVMRegression in _otsvm:
 _otsvm.LibSVMRegression_swigregister(LibSVMRegression)
-
-class LibSVMClassification(openturns.common.PersistentObject):
+class LibSVMClassification(openturns.algo.ClassifierImplementation):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
 
     def getClassName(self):
         r"""
         Accessor to the object's name.
 
         Returns
@@ -841,20 +815,48 @@
         """
         return _otsvm.LibSVMClassification_getClassName(self)
 
     def getAccuracy(self):
         return _otsvm.LibSVMClassification_getAccuracy(self)
 
     def classify(self, vector):
+        r"""
+        Classify points according to the classifier.
+
+        Parameters
+        ----------
+        input : sequence of float or 2-d a sequence of float
+            A point or set of points to classify.
+
+        Returns
+        -------
+        cls : int or :class:`~openturns.Indices`
+            The class index of the input points, or indices of the classes of each points.
+        """
         return _otsvm.LibSVMClassification_classify(self, vector)
 
     def __repr__(self):
         return _otsvm.LibSVMClassification___repr__(self)
 
     def grade(self, inP, outC):
+        r"""
+        Grade points according to the classifier.
+
+        Parameters
+        ----------
+        inputPoint : sequence of float or 2-d a sequence of float
+            A point or set of points to grade.
+        k : int or sequence of int
+            The class index, or class indices.
+
+        Returns
+        -------
+        grade : float or :class:`~openturns.Point`
+            Grade or list of grades of each input point with respect to each class index
+        """
         return _otsvm.LibSVMClassification_grade(self, inP, outC)
 
     def predict(self, inP):
         return _otsvm.LibSVMClassification_predict(self, inP)
 
     def runKMeans(self, k):
         return _otsvm.LibSVMClassification_runKMeans(self, k)
@@ -876,15 +878,14 @@
 
     def __init__(self, *args):
         _otsvm.LibSVMClassification_swiginit(self, _otsvm.new_LibSVMClassification(*args))
     __swig_destroy__ = _otsvm.delete_LibSVMClassification
 
 # Register LibSVMClassification in _otsvm:
 _otsvm.LibSVMClassification_swigregister(LibSVMClassification)
-
 class KMeansClustering(openturns.common.PersistentObject):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
 
     def getClassName(self):
         r"""
         Accessor to the object's name.
@@ -907,15 +908,14 @@
 
     def __init__(self, *args):
         _otsvm.KMeansClustering_swiginit(self, _otsvm.new_KMeansClustering(*args))
     __swig_destroy__ = _otsvm.delete_KMeansClustering
 
 # Register KMeansClustering in _otsvm:
 _otsvm.KMeansClustering_swigregister(KMeansClustering)
-
 class SVMKernelCollection(object):
     r"""
     Collection.
 
     Examples
     --------
     >>> import openturns as ot
@@ -1158,9 +1158,7 @@
 
     def __init__(self, *args):
         _otsvm.SVMKernelCollection_swiginit(self, _otsvm.new_SVMKernelCollection(*args))
 
 # Register SVMKernelCollection in _otsvm:
 _otsvm.SVMKernelCollection_swigregister(SVMKernelCollection)
 
-
-
```

## otsvm/__init__.py

```diff
@@ -10,15 +10,15 @@
 
     Classes
     --------
     LibSVMRegression                                The class that supports the regression.
 
 """
 
-import sys
-if sys.platform.startswith('win'):
-    # this ensures OT dll is loaded
-    import openturns
+# flake8: noqa
+
+# ensures swig type tables order & dll load
+import openturns as _ot
 
 from .otsvm import *
 
-__version__ = '0.11.post7'
+__version__ = "0.11"
```

## Comparing `otsvm-0.11.post7.dist-info/METADATA` & `otsvm-0.12.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: otsvm
-Version: 0.11.post7
+Version: 0.12
 Summary: SVM module
 Home-page:  http://www.openturns.org
 Author: OpenTURNS Developers
 Author-email: users@openturns.org
 License: LGPL
 Keywords: probability reliability sensitivity metamodel
 Platform: any
```

