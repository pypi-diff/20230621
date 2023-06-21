# Comparing `tmp/baysalt_christmas-0.1.7.7.tar.gz` & `tmp/baysalt_christmas-0.1.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baysalt_christmas-0.1.7.7.tar", last modified: Mon Jun 12 03:13:47 2023, max compression
+gzip compressed data, was "baysalt_christmas-0.1.7.8.tar", last modified: Wed Jun 21 03:08:09 2023, max compression
```

## Comparing `baysalt_christmas-0.1.7.7.tar` & `baysalt_christmas-0.1.7.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-12 03:13:47.331713 baysalt_christmas-0.1.7.7/
--rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-05-18 11:12:41.000000 baysalt_christmas-0.1.7.7/.DS_Store
--rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.7.7/MANIFEST.in
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-06-12 03:13:47.331570 baysalt_christmas-0.1.7.7/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.7.7/README.md
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-12 03:13:47.327005 baysalt_christmas-0.1.7.7/baysalt_christmas.egg-info/
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-06-12 03:13:47.000000 baysalt_christmas-0.1.7.7/baysalt_christmas.egg-info/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)      729 2023-06-12 03:13:47.000000 baysalt_christmas-0.1.7.7/baysalt_christmas.egg-info/SOURCES.txt
--rw-r--r--   0 christmas   (501) staff       (20)        1 2023-06-12 03:13:47.000000 baysalt_christmas-0.1.7.7/baysalt_christmas.egg-info/dependency_links.txt
--rw-r--r--   0 christmas   (501) staff       (20)       30 2023-06-12 03:13:47.000000 baysalt_christmas-0.1.7.7/baysalt_christmas.egg-info/requires.txt
--rw-r--r--   0 christmas   (501) staff       (20)       10 2023-06-12 03:13:47.000000 baysalt_christmas-0.1.7.7/baysalt_christmas.egg-info/top_level.txt
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-12 03:13:47.328921 baysalt_christmas-0.1.7.7/christmas/
--rw-r--r--   0 christmas   (501) staff       (20)    21061 2023-06-08 02:22:25.000000 baysalt_christmas-0.1.7.7/christmas/Blogging.py
--rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.7.7/christmas/S_DateTime.py
--rw-r--r--   0 christmas   (501) staff       (20)      445 2023-04-23 12:43:18.000000 baysalt_christmas-0.1.7.7/christmas/__init__.py
--rw-r--r--   0 christmas   (501) staff       (20)     4676 2023-05-17 09:02:10.000000 baysalt_christmas-0.1.7.7/christmas/commonCode.py
--rw-r--r--   0 christmas   (501) staff       (20)     1638 2023-04-12 07:23:55.000000 baysalt_christmas-0.1.7.7/christmas/cprintf.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-12 03:13:47.330181 baysalt_christmas-0.1.7.7/christmas/mncPy/
--rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.7/christmas/mncPy/.gitignore
--rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.7/christmas/mncPy/LICENSE
--rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.7.7/christmas/mncPy/__init__.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-12 03:13:47.331207 baysalt_christmas-0.1.7.7/christmas/mncPy/__pycache__/
--rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.7.7/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)     8964 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.7/christmas/mncPy/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)     3411 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.7/christmas/mncPy/__pycache__/compress.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.7.7/christmas/mncPy/common.py
--rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.7.7/christmas/mncPy/compress.py
--rw-r--r--   0 christmas   (501) staff       (20)     3554 2023-03-29 02:58:20.000000 baysalt_christmas-0.1.7.7/christmas/processBar.py
--rw-r--r--   0 christmas   (501) staff       (20)     3679 2023-06-12 03:11:04.000000 baysalt_christmas-0.1.7.7/christmas/read_conf.py
--rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.7.7/christmas/server_info.py
--rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.7.7/run_twine.py
--rw-r--r--   0 christmas   (501) staff       (20)       38 2023-06-12 03:13:47.331772 baysalt_christmas-0.1.7.7/setup.cfg
--rw-r--r--   0 christmas   (501) staff       (20)      796 2023-06-12 03:13:42.000000 baysalt_christmas-0.1.7.7/setup.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-21 03:08:09.392600 baysalt_christmas-0.1.7.8/
+-rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-06-13 08:58:02.000000 baysalt_christmas-0.1.7.8/.DS_Store
+-rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.7.8/MANIFEST.in
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-06-21 03:08:09.392378 baysalt_christmas-0.1.7.8/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.7.8/README.md
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-21 03:08:09.382757 baysalt_christmas-0.1.7.8/baysalt_christmas.egg-info/
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-06-21 03:08:09.000000 baysalt_christmas-0.1.7.8/baysalt_christmas.egg-info/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)      729 2023-06-21 03:08:09.000000 baysalt_christmas-0.1.7.8/baysalt_christmas.egg-info/SOURCES.txt
+-rw-r--r--   0 christmas   (501) staff       (20)        1 2023-06-21 03:08:09.000000 baysalt_christmas-0.1.7.8/baysalt_christmas.egg-info/dependency_links.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       30 2023-06-21 03:08:09.000000 baysalt_christmas-0.1.7.8/baysalt_christmas.egg-info/requires.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       10 2023-06-21 03:08:09.000000 baysalt_christmas-0.1.7.8/baysalt_christmas.egg-info/top_level.txt
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-21 03:08:09.386828 baysalt_christmas-0.1.7.8/christmas/
+-rw-r--r--   0 christmas   (501) staff       (20)    21061 2023-06-08 02:22:25.000000 baysalt_christmas-0.1.7.8/christmas/Blogging.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.7.8/christmas/S_DateTime.py
+-rw-r--r--   0 christmas   (501) staff       (20)      445 2023-04-23 12:43:18.000000 baysalt_christmas-0.1.7.8/christmas/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4676 2023-05-17 09:02:10.000000 baysalt_christmas-0.1.7.8/christmas/commonCode.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1638 2023-04-12 07:23:55.000000 baysalt_christmas-0.1.7.8/christmas/cprintf.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-21 03:08:09.390516 baysalt_christmas-0.1.7.8/christmas/mncPy/
+-rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.8/christmas/mncPy/.gitignore
+-rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.8/christmas/mncPy/LICENSE
+-rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.7.8/christmas/mncPy/__init__.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-21 03:08:09.391579 baysalt_christmas-0.1.7.8/christmas/mncPy/__pycache__/
+-rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.7.8/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     8964 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.8/christmas/mncPy/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     3411 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.8/christmas/mncPy/__pycache__/compress.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.7.8/christmas/mncPy/common.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.7.8/christmas/mncPy/compress.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4710 2023-06-21 03:07:09.000000 baysalt_christmas-0.1.7.8/christmas/processBar.py
+-rw-r--r--   0 christmas   (501) staff       (20)     3679 2023-06-12 03:11:04.000000 baysalt_christmas-0.1.7.8/christmas/read_conf.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.7.8/christmas/server_info.py
+-rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.7.8/run_twine.py
+-rw-r--r--   0 christmas   (501) staff       (20)       38 2023-06-21 03:08:09.392690 baysalt_christmas-0.1.7.8/setup.cfg
+-rw-r--r--   0 christmas   (501) staff       (20)      796 2023-06-21 03:08:02.000000 baysalt_christmas-0.1.7.8/setup.py
```

### Comparing `baysalt_christmas-0.1.7.7/.DS_Store` & `baysalt_christmas-0.1.7.8/.DS_Store`

 * *Files 10% similar despite different names*

```diff
@@ -270,33 +270,33 @@
 000010d0: 0063 0068 0072 0069 0073 0074 006d 0061  .c.h.r.i.s.t.m.a
 000010e0: 0073 002e 0065 0067 0067 002d 0069 006e  .s...e.g.g.-.i.n
 000010f0: 0066 006f 6c67 3153 636f 6d70 0000 0000  .f.olg1Scomp....
 00001100: 0000 1301 0000 001a 0062 0061 0079 0073  .........b.a.y.s
 00001110: 0061 006c 0074 005f 0063 0068 0072 0069  .a.l.t._.c.h.r.i
 00001120: 0073 0074 006d 0061 0073 002e 0065 0067  .s.t.m.a.s...e.g
 00001130: 0067 002d 0069 006e 0066 006f 6d6f 4444  .g.-.i.n.f.omoDD
-00001140: 626c 6f62 0000 0008 a182 0dd7 670a c541  blob........g..A
+00001140: 626c 6f62 0000 0008 2097 9c75 621b c541  blob.... ..ub..A
 00001150: 0000 001a 0062 0061 0079 0073 0061 006c  .....b.a.y.s.a.l
 00001160: 0074 005f 0063 0068 0072 0069 0073 0074  .t._.c.h.r.i.s.t
 00001170: 006d 0061 0073 002e 0065 0067 0067 002d  .m.a.s...e.g.g.-
 00001180: 0069 006e 0066 006f 6d6f 6444 626c 6f62  .i.n.f.omodDblob
-00001190: 0000 0008 a182 0dd7 670a c541 0000 001a  ........g..A....
+00001190: 0000 0008 2097 9c75 621b c541 0000 001a  .... ..ub..A....
 000011a0: 0062 0061 0079 0073 0061 006c 0074 005f  .b.a.y.s.a.l.t._
 000011b0: 0063 0068 0072 0069 0073 0074 006d 0061  .c.h.r.i.s.t.m.a
 000011c0: 0073 002e 0065 0067 0067 002d 0069 006e  .s...e.g.g.-.i.n
 000011d0: 0066 006f 7068 3153 636f 6d70 0000 0000  .f.oph1Scomp....
 000011e0: 0000 5000 0000 0005 0062 0075 0069 006c  ..P......b.u.i.l
 000011f0: 0064 6c67 3153 636f 6d70 0000 0000 0001  .dlg1Scomp......
-00001200: 97f8 0000 0005 0062 0075 0069 006c 0064  .......b.u.i.l.d
-00001210: 6d6f 4444 626c 6f62 0000 0008 b036 39d7  moDDblob.....69.
-00001220: 670a c541 0000 0005 0062 0075 0069 006c  g..A.....b.u.i.l
-00001230: 0064 6d6f 6444 626c 6f62 0000 0008 b036  .dmodDblob.....6
-00001240: 39d7 670a c541 0000 0005 0062 0075 0069  9.g..A.....b.u.i
+00001200: b1d7 0000 0005 0062 0075 0069 006c 0064  .......b.u.i.l.d
+00001210: 6d6f 4444 626c 6f62 0000 0008 9aef 0785  moDDblob........
+00001220: 331c c541 0000 0005 0062 0075 0069 006c  3..A.....b.u.i.l
+00001230: 0064 6d6f 6444 626c 6f62 0000 0008 9aef  .dmodDblob......
+00001240: 0785 331c c541 0000 0005 0062 0075 0069  ..3..A.....b.u.i
 00001250: 006c 0064 7068 3153 636f 6d70 0000 0000  .l.dph1Scomp....
-00001260: 0002 4000 0000 0009 0063 0068 0072 0069  ..@......c.h.r.i
+00001260: 0002 6000 0000 0009 0063 0068 0072 0069  ..`......c.h.r.i
 00001270: 0073 0074 006d 0061 0073 6277 7370 626c  .s.t.m.a.sbwspbl
 00001280: 6f62 0000 00ba 6270 6c69 7374 3030 d601  ob....bplist00..
 00001290: 0203 0405 0607 0807 080b 085d 5368 6f77  ...........]Show
 000012a0: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
 000012b0: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
 000012c0: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
 000012d0: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
@@ -306,15 +306,15 @@
 00001310: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8c  }}...#/;R_klmno.
 00001320: 0000 0000 0000 0101 0000 0000 0000 000d  ................
 00001330: 0000 0000 0000 0000 0000 0000 0000 008d  ................
 00001340: 0000 0009 0063 0068 0072 0069 0073 0074  .....c.h.r.i.s.t
 00001350: 006d 0061 0073 6473 636c 626f 6f6c 0100  .m.a.sdsclbool..
 00001360: 0000 0900 6300 6800 7200 6900 7300 7400  ....c.h.r.i.s.t.
 00001370: 6d00 6100 736c 6731 5363 6f6d 7000 0000  m.a.slg1Scomp...
-00001380: 0000 0216 8f00 0000 0900 6300 6800 7200  ..........c.h.r.
+00001380: 0000 021a 7b00 0000 0900 6300 6800 7200  ....{.....c.h.r.
 00001390: 6900 7300 7400 6d00 6100 736c 7376 4362  i.s.t.m.a.slsvCb
 000013a0: 6c6f 6200 0003 0062 706c 6973 7430 30d8  lob....bplist00.
 000013b0: 0102 0304 0506 0708 090a 0b16 5354 550a  ............STU.
 000013c0: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
 000013d0: 7273 696f 6e5f 100f 7368 6f77 4963 6f6e  rsion_..showIcon
 000013e0: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
 000013f0: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
@@ -400,17 +400,17 @@
 000018f0: 0169 0172 0174 0175 0176 017f 0181 0182  .i.r.t.u.v......
 00001900: 0184 0185 018e 0190 0191 0194 0195 019e  ................
 00001910: 01a0 01a1 01a2 01a3 01ac 01b9 01c2 0000  ................
 00001920: 0000 0000 0201 0000 0000 0000 0049 0000  .............I..
 00001930: 0000 0000 0000 0000 0000 0000 01c3 0000  ................
 00001940: 0009 0063 0068 0072 0069 0073 0074 006d  ...c.h.r.i.s.t.m
 00001950: 0061 0073 6d6f 4444 626c 6f62 0000 0008  .a.smoDDblob....
-00001960: 8fa1 18c9 670a c541 0000 0009 0063 0068  ....g..A.....c.h
+00001960: 5b8c 5224 621b c541 0000 0009 0063 0068  [.R$b..A.....c.h
 00001970: 0072 0069 0073 0074 006d 0061 0073 6d6f  .r.i.s.t.m.a.smo
-00001980: 6444 626c 6f62 0000 0008 8fa1 18c9 670a  dDblob........g.
+00001980: 6444 626c 6f62 0000 0008 5b8c 5224 621b  dDblob....[.R$b.
 00001990: c541 0000 0009 0063 0068 0072 0069 0073  .A.....c.h.r.i.s
 000019a0: 0074 006d 0061 0073 7068 3153 636f 6d70  .t.m.a.sph1Scomp
 000019b0: 0000 0000 0003 1000 0000 0009 0063 0068  .............c.h
 000019c0: 0072 0069 0073 0074 006d 0061 0073 7653  .r.i.s.t.m.a.svS
 000019d0: 726e 6c6f 6e67 0000 0001 0000 0004 0064  rnlong.........d
 000019e0: 0069 0073 0074 6277 7370 626c 6f62 0000  .i.s.tbwspblob..
 000019f0: 00b9 6270 6c69 7374 3030 d601 0203 0405  ..bplist00......
@@ -422,19 +422,19 @@
 00001a50: 735b 5368 6f77 5369 6465 6261 7208 0908  s[ShowSidebar...
 00001a60: 095f 1019 7b7b 3430 342c 2034 3738 7d2c  ._..{{404, 478},
 00001a70: 207b 3132 3338 2c20 3436 377d 7d09 0815   {1238, 467}}...
 00001a80: 232f 3b52 5f6b 6c6d 6e6f 8b00 0000 0000  #/;R_klmno......
 00001a90: 0001 0100 0000 0000 0000 0d00 0000 0000  ................
 00001aa0: 0000 0000 0000 0000 0000 8c00 0000 0400  ................
 00001ab0: 6400 6900 7300 746c 6731 5363 6f6d 7000  d.i.s.tlg1Scomp.
-00001ac0: 0000 0000 013a 3400 0000 0400 6400 6900  .....:4.....d.i.
-00001ad0: 7300 746d 6f44 4462 6c6f 6200 0000 08c3  s.tmoDDblob.....
-00001ae0: 703d d767 0ac5 4100 0000 0400 6400 6900  p=.g..A.....d.i.
-00001af0: 7300 746d 6f64 4462 6c6f 6200 0000 08c3  s.tmodDblob.....
-00001b00: 703d d767 0ac5 4100 0000 0400 6400 6900  p=.g..A.....d.i.
+00001ac0: 0000 0000 013b 3300 0000 0400 6400 6900  .....;3.....d.i.
+00001ad0: 7300 746d 6f44 4462 6c6f 6200 0000 0856  s.tmoDDblob....V
+00001ae0: b20e 8433 1cc5 4100 0000 0400 6400 6900  ...3..A.....d.i.
+00001af0: 7300 746d 6f64 4462 6c6f 6200 0000 0897  s.tmodDblob.....
+00001b00: 05d1 7562 1bc5 4100 0000 0400 6400 6900  ..ub..A.....d.i.
 00001b10: 7300 7470 6831 5363 6f6d 7000 0000 0000  s.tph1Scomp.....
 00001b20: 0150 0000 0000 0400 6400 6900 7300 7476  .P......d.i.s.tv
 00001b30: 5372 6e6c 6f6e 6700 0000 0100 0000 0000  Srnlong.........
 00001b40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001b50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001b60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001b70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `baysalt_christmas-0.1.7.7/PKG-INFO` & `baysalt_christmas-0.1.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt_christmas
-Version: 0.1.7.7
+Version: 0.1.7.8
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.7.7/README.md` & `baysalt_christmas-0.1.7.8/README.md`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.7/baysalt_christmas.egg-info/PKG-INFO` & `baysalt_christmas-0.1.7.8/baysalt_christmas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt-christmas
-Version: 0.1.7.7
+Version: 0.1.7.8
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.7.7/baysalt_christmas.egg-info/SOURCES.txt` & `baysalt_christmas-0.1.7.8/baysalt_christmas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.7/christmas/Blogging.py` & `baysalt_christmas-0.1.7.8/christmas/Blogging.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.7/christmas/S_DateTime.py` & `baysalt_christmas-0.1.7.8/christmas/S_DateTime.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.7/christmas/commonCode.py` & `baysalt_christmas-0.1.7.8/christmas/commonCode.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.7/christmas/cprintf.py` & `baysalt_christmas-0.1.7.8/christmas/cprintf.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.7/christmas/mncPy/.gitignore` & `baysalt_christmas-0.1.7.8/christmas/mncPy/.gitignore`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.7/christmas/mncPy/LICENSE` & `baysalt_christmas-0.1.7.8/christmas/mncPy/LICENSE`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.7/christmas/mncPy/__pycache__/common.cpython-39.pyc` & `baysalt_christmas-0.1.7.8/christmas/mncPy/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.7/christmas/mncPy/__pycache__/compress.cpython-39.pyc` & `baysalt_christmas-0.1.7.8/christmas/mncPy/__pycache__/compress.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.7/christmas/mncPy/common.py` & `baysalt_christmas-0.1.7.8/christmas/mncPy/common.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.7/christmas/mncPy/compress.py` & `baysalt_christmas-0.1.7.8/christmas/mncPy/compress.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.7/christmas/processBar.py` & `baysalt_christmas-0.1.7.8/christmas/processBar.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 #  邮箱 : 273519355@qq.com
 #  项目 : Project
 #  版本 : python 3
 #  摘要 :
 """
 processBar such as: ftp sftp
 """
+import time
 import datetime
 
 
 class SftpProcessbar(object):
 	"""
 	sftp_obj =SftpProcessbar()
 	Sprocess_bar = sftp_obj.process_bar
@@ -63,43 +64,71 @@
 		return '{:.2f} GB'.format(B / GB)
 	else:
 		return '{:.2f} TB'.format(B / TB)
 
 
 class FtpProcessbar(object):
 	"""
+	upload ------------------->:
 	Ftp_obj = FtpProcessbar(os.path.getsize(local_path))
 	Fprocess_bar = Ftp_obj.process_bar()
 
 	# ftp = ftplib.FTP()
 	# ftp.encoding = 'utf-8'
 	# ftp.set_debuglevel(0)
 	# ftp.connect(host=_host, port=_port)
 	# ftp.login(_username, _password)
-	# Ftp_obj = FtpProcessbar(os.path.getsize(local_path))
-	# Fprocess_bar = Ftp_obj.process_bar()
 	# with open(local_path, 'rb') as fp:
+	#   Ftp_obj = FtpProcessbar(os.path.getsize(local_path))
+	#   Fprocess_bar = Ftp_obj.process_bar()
 	#   ftp.storbinary(f'STOR {file}', fp, buf_size, Fprocess_bar)
+	#   ==============================================
+	download ------------------->:
+	Ftp_obj = FtpProcessbar(ftp.size(local_path), fp=fp)
+	Fprocess_bar = Ftp_obj.process_bar()
+
+	# ftp = ftplib.FTP()
+	# ftp.encoding = 'utf-8'
+	# ftp.set_debuglevel(0)
+	# ftp.connect(host=_host, port=_port)
+	# ftp.login(_username, _password)
+	# Ftp_obj = FtpProcessbar(ftp.size(local_path), fp=fp)
+	# Fprocess_bar = Ftp_obj.process_bar()
+	# with open(local_path, 'rb') as fp:
+	#   Ftp_obj = FtpProcessbar(ftp.size(local_path), fp=fp)
+	#   Fprocess_bar = Ftp_obj.process_bar()
+	#   ftp.retrbinary(f'RETR {file}', Fprocess_bar,  buf_size)
 	"""
 
-	def __init__(self, totalSize, bar_length=30, change_percent=1):
-		self.totalSize = totalSize
-		self.sizeWritten = 0
-		self.lastShownPercent = 0
+	def __init__(self, totalSize, fp=None, bar_length=30, change_percent=1):
+		self.totalSize = totalSize  # 已上传或下载大小
+		self.time_start = time.time()  # 开始上传或下载时间(注意是实例化时开始计时)
+		self.sizeWritten = 0   # 文件总大小
+		self.lastShownPercent = 0  # 上次显示的百分比
 		self.bar_length = bar_length  # 进度条长度
 		self.change_percent = change_percent  # 进度条变化百分比 0为1%输出 1为0.1%输出 2为0.01%输出
+		if fp:
+			self.fp = fp                   # 文件对象
 
 	def call_back(self, block):
+		"""
+		:param block: 上传或下载的数据块
+		"""
+		if self.fp:
+			self.fp.write(block)
 		self.sizeWritten += len(block)
-		bar_length = self.bar_length
 		percents = '\033[32;1m%s\033[0m' % round(float(self.sizeWritten) * 100 / float(self.totalSize), self.change_percent)
-		filled = int(bar_length * self.sizeWritten / float(self.totalSize))
-		bar = '\033[32;1m%s\033[0m' % '=' * filled + '-' * (bar_length - filled)
+		filled = int(self.bar_length * self.sizeWritten / float(self.totalSize))
+		bar = '\033[32;1m%s\033[0m' % '=' * filled + '-' * (self.bar_length - filled)
+		speed = self.sizeWritten / (time.time() - self.time_start)
 
-		percentComplete = round((self.sizeWritten / self.totalSize) * 100, self.change_percent)
+		percentComplete = round((self.sizeWritten / self.totalSize) * 100, self.change_percent)  # 粗分辨率,防止刷新过快
 		if self.lastShownPercent != percentComplete:
 			self.lastShownPercent = percentComplete
 			ddt = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
-			print(f'{ddt} ---> [{bar}] {percents}% already complete: {translate_byte(self.sizeWritten)}, total: {translate_byte(self.totalSize)}\r', end='')
+			print(f'{ddt} ---> [{bar}] {percents}% speed:{translate_byte(speed)}/s, already complete: {translate_byte(self.sizeWritten)}, total: {translate_byte(self.totalSize)}\r', end='')
 
 	def process_bar(self):
+		"""
+		:return: 返回一个函数对象
+		"""
 		return self.call_back
```

### Comparing `baysalt_christmas-0.1.7.7/christmas/read_conf.py` & `baysalt_christmas-0.1.7.8/christmas/read_conf.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.7/christmas/server_info.py` & `baysalt_christmas-0.1.7.8/christmas/server_info.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.7/setup.py` & `baysalt_christmas-0.1.7.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="baysalt_christmas",
-    version="0.1.7.7",
+    version="0.1.7.8",
     author="Christmas",
     author_email="273519355@qq.com",
     description="Some simple tools for Christmas",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     include_package_data=True,
```

