# Comparing `tmp/ftmq-0.1.2.tar.gz` & `tmp/ftmq-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftmq-0.1.2.tar", max compression
+gzip compressed data, was "ftmq-0.1.3.tar", max compression
```

## Comparing `ftmq-0.1.2.tar` & `ftmq-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1077 2023-04-04 14:31:45.930293 ftmq-0.1.2/LICENSE
--rw-r--r--   0        0        0     4039 2023-06-14 16:58:41.577739 ftmq-0.1.2/README.md
--rw-r--r--   0        0        0       22 2023-06-14 18:57:52.786294 ftmq-0.1.2/ftmq/__init__.py
--rw-r--r--   0        0        0     1221 2023-06-14 18:32:14.390982 ftmq-0.1.2/ftmq/cli.py
--rw-r--r--   0        0        0       43 2023-02-17 15:30:40.666516 ftmq-0.1.2/ftmq/exceptions.py
--rw-r--r--   0        0        0     5115 2023-06-14 18:50:42.961409 ftmq-0.1.2/ftmq/filters.py
--rw-r--r--   0        0        0     1593 2023-06-14 18:17:13.454654 ftmq-0.1.2/ftmq/io.py
--rw-r--r--   0        0        0     1784 2023-06-14 17:04:10.502390 ftmq-0.1.2/ftmq/query.py
--rw-r--r--   0        0        0      383 2023-06-14 15:32:48.293679 ftmq-0.1.2/ftmq/types.py
--rw-r--r--   0        0        0      523 2023-06-14 17:55:59.782847 ftmq-0.1.2/ftmq/util.py
--rw-r--r--   0        0        0     1285 2023-06-14 18:57:52.786294 ftmq-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5161 1970-01-01 00:00:00.000000 ftmq-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-04 14:31:45.930293 ftmq-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4376 2023-06-20 10:59:09.516461 ftmq-0.1.3/README.md
+-rw-r--r--   0        0        0       22 2023-06-21 05:48:36.344091 ftmq-0.1.3/ftmq/__init__.py
+-rw-r--r--   0        0        0     2714 2023-06-20 10:59:09.516461 ftmq-0.1.3/ftmq/cli.py
+-rw-r--r--   0        0        0       43 2023-02-17 15:30:40.666516 ftmq-0.1.3/ftmq/exceptions.py
+-rw-r--r--   0        0        0     5115 2023-06-14 18:50:42.961409 ftmq-0.1.3/ftmq/filters.py
+-rw-r--r--   0        0        0     1964 2023-06-20 10:59:09.516461 ftmq-0.1.3/ftmq/io.py
+-rw-r--r--   0        0        0     1784 2023-06-14 17:04:10.502390 ftmq-0.1.3/ftmq/query.py
+-rw-r--r--   0        0        0      383 2023-06-14 15:32:48.293679 ftmq-0.1.3/ftmq/types.py
+-rw-r--r--   0        0        0      973 2023-06-14 20:07:15.762203 ftmq-0.1.3/ftmq/util.py
+-rw-r--r--   0        0        0     1316 2023-06-21 05:48:36.344091 ftmq-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5549 1970-01-01 00:00:00.000000 ftmq-0.1.3/PKG-INFO
```

### Comparing `ftmq-0.1.2/LICENSE` & `ftmq-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ftmq-0.1.2/README.md` & `ftmq-0.1.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -179,75 +179,96 @@
 00000b20: 494c 494b 4560 2c20 6361 7365 2d69 6e73  ILIKE`, case-ins
 00000b30: 656e 7369 7469 7665 2028 7573 6520 6025  ensitive (use `%
 00000b40: 6020 706c 6163 6568 6f6c 6465 7273 290a  ` placeholders).
 00000b50: 2d20 605b 5d60 202d 2075 7361 6765 3a20  - `[]` - usage: 
 00000b60: 6070 726f 705b 5d3d 666f 6f60 2065 7661  `prop[]=foo` eva
 00000b70: 6c75 6174 6573 2069 6620 6066 6f6f 6020  luates if `foo` 
 00000b80: 6973 206d 656d 6265 7220 6f66 2061 7272  is member of arr
-00000b90: 6179 2060 7072 6f70 600a 0a23 2323 2066  ay `prop`..### f
-00000ba0: 746d 7374 6f72 6520 2864 6174 6162 6173  tmstore (databas
-00000bb0: 6520 7265 6164 290a 0a54 6865 2073 616d  e read)..The sam
-00000bc0: 6520 636c 6920 6c6f 6769 6320 6170 706c  e cli logic appl
-00000bd0: 6965 733a 0a0a 2020 2020 6674 6d71 2073  ies:..    ftmq s
-00000be0: 746f 7265 2069 7465 7261 7465 202d 6420  tore iterate -d 
-00000bf0: 6563 5f6d 6565 7469 6e67 7320 2d73 2045  ec_meetings -s E
-00000c00: 7665 6e74 202d 2d64 6174 655f 5f67 7465  vent --date__gte
-00000c10: 3d32 3031 3920 2d2d 6461 7465 5f5f 6c74  =2019 --date__lt
-00000c20: 653d 3230 3230 0a0a 2323 2050 7974 686f  e=2020..## Pytho
-00000c30: 6e20 4c69 6272 6172 790a 0a60 6060 7079  n Library..```py
-00000c40: 7468 6f6e 0a66 726f 6d20 6674 6d71 2069  thon.from ftmq i
-00000c50: 6d70 6f72 7420 5175 6572 790a 0a71 203d  mport Query..q =
-00000c60: 2051 7565 7279 2865 6e67 696e 653d 2273   Query(engine="s
-00000c70: 716c 6974 6522 2920 5c0a 2020 2020 2e77  qlite") \.    .w
-00000c80: 6865 7265 2864 6174 6173 6574 3d22 6563  here(dataset="ec
-00000c90: 5f6d 6565 7469 6e67 7322 2c20 6461 7465  _meetings", date
-00000ca0: 5f5f 6c74 653d 3230 3230 2920 5c0a 2020  __lte=2020) \.  
-00000cb0: 2020 2e77 6865 7265 2873 6368 656d 613d    .where(schema=
-00000cc0: 2245 7665 6e74 2229 205c 0a20 2020 202e  "Event") \.    .
-00000cd0: 6f72 6465 725f 6279 2822 6461 7465 222c  order_by("date",
-00000ce0: 2061 7363 656e 6469 6e67 3d46 616c 7365   ascending=False
-00000cf0: 290a 0a23 2072 6573 756c 7469 6e67 2073  )..# resulting s
-00000d00: 716c 6974 6520 7175 6572 793a 0a73 7472  qlite query:.str
-00000d10: 2871 290a 2222 220a 5345 4c45 4354 2074  (q).""".SELECT t
-00000d20: 2e69 642c 0a20 2020 2074 2e73 6368 656d  .id,.    t.schem
-00000d30: 612c 0a20 2020 2074 2e65 6e74 6974 792c  a,.    t.entity,
-00000d40: 0a20 2020 206a 736f 6e5f 6578 7472 6163  .    json_extrac
-00000d50: 7428 742e 656e 7469 7479 2c20 2724 2e70  t(t.entity, '$.p
-00000d60: 726f 7065 7274 6965 732e 6461 7465 2729  roperties.date')
-00000d70: 2041 5320 6461 7465 0a46 524f 4d20 6563   AS date.FROM ec
-00000d80: 5f6d 6565 7469 6e67 7320 740a 5748 4552  _meetings t.WHER
-00000d90: 450a 2020 2020 2845 5849 5354 5320 2853  E.    (EXISTS (S
-00000da0: 454c 4543 5420 3120 4652 4f4d 206a 736f  ELECT 1 FROM jso
-00000db0: 6e5f 6561 6368 2864 6174 6529 2057 4845  n_each(date) WHE
-00000dc0: 5245 2076 616c 7565 203c 3d20 3f29 2920  RE value <= ?)) 
-00000dd0: 414e 4420 2874 2e73 6368 656d 6120 3d20  AND (t.schema = 
-00000de0: 3f29 0a4f 5244 4552 2042 5920 6461 7465  ?).ORDER BY date
-00000df0: 2044 4553 430a 2222 220a 0a23 2070 6172   DESC."""..# par
-00000e00: 616d 6574 6572 697a 6564 0a5b 7020 666f  ameterized.[p fo
-00000e10: 7220 7020 696e 2071 2e70 6172 616d 6574  r p in q.paramet
-00000e20: 6572 735d 0a5b 3230 3230 2c20 2745 7665  ers].[2020, 'Eve
-00000e30: 6e74 275d 0a60 6060 0a0a 2323 2073 7570  nt'].```..## sup
-00000e40: 706f 7274 0a0a 2a54 6869 7320 7072 6f6a  port..*This proj
-00000e50: 6563 7420 6973 2070 6172 7420 6f66 205b  ect is part of [
-00000e60: 696e 7665 7374 6967 7261 7068 5d28 6874  investigraph](ht
-00000e70: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000e80: 2f69 6e76 6573 7469 6761 7469 7665 6461  /investigativeda
-00000e90: 7461 2f69 6e76 6573 7469 6772 6170 6829  ta/investigraph)
-00000ea0: 2a0a 0a5b 4d65 6469 6120 5465 6368 204c  *..[Media Tech L
-00000eb0: 6162 2042 6179 6572 6e20 6261 7463 6820  ab Bayern batch 
-00000ec0: 2333 5d28 6874 7470 733a 2f2f 6769 7468  #3](https://gith
-00000ed0: 7562 2e63 6f6d 2f6d 6564 6961 2d74 6563  ub.com/media-tec
-00000ee0: 682d 6c61 6229 0a0a 3c61 2068 7265 663d  h-lab)..<a href=
-00000ef0: 2268 7474 7073 3a2f 2f77 7777 2e6d 6564  "https://www.med
-00000f00: 6961 2d6c 6162 2e64 652f 656e 2f70 726f  ia-lab.de/en/pro
-00000f10: 6772 616d 732f 6d65 6469 612d 7465 6368  grams/media-tech
-00000f20: 2d6c 6162 223e 0a20 2020 203c 696d 6720  -lab">.    <img 
-00000f30: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
-00000f40: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-00000f50: 6e74 2e63 6f6d 2f6d 6564 6961 2d74 6563  nt.com/media-tec
-00000f60: 682d 6c61 622f 2e67 6974 6875 622f 6d61  h-lab/.github/ma
-00000f70: 696e 2f61 7373 6574 732f 6d74 6c2d 706f  in/assets/mtl-po
-00000f80: 7765 7265 642d 6279 2e70 6e67 2220 7769  wered-by.png" wi
-00000f90: 6474 683d 2232 3430 2220 7469 746c 653d  dth="240" title=
-00000fa0: 224d 6564 6961 2054 6563 6820 4c61 6220  "Media Tech Lab 
-00000fb0: 706f 7765 7265 6420 6279 206c 6f67 6f22  powered by logo"
-00000fc0: 3e0a 3c2f 613e 0a                        >.</a>.
+00000b90: 6179 2060 7072 6f70 600a 0a0a 2323 2320  ay `prop`...### 
+00000ba0: 6674 6d71 2061 7070 6c79 0a0a 2255 706c  ftmq apply.."Upl
+00000bb0: 6576 656c 2220 616e 2065 6e74 6974 7920  evel" an entity 
+00000bc0: 696e 7075 7420 7374 7265 616d 2074 6f20  input stream to 
+00000bd0: 606e 6f6d 656e 6b6c 6174 7572 612e 656e  `nomenklatura.en
+00000be0: 7469 7479 2e43 6f6d 706f 7369 7465 456e  tity.CompositeEn
+00000bf0: 7469 7479 6020 616e 640a 6f70 7469 6f6e  tity` and.option
+00000c00: 616c 6c79 2061 7070 6c79 2061 2064 6174  ally apply a dat
+00000c10: 6173 6574 2e0a 0a20 2020 2066 746d 7120  aset...    ftmq 
+00000c20: 6170 706c 7920 2d69 202e 2f65 6e74 6974  apply -i ./entit
+00000c30: 6965 732e 6674 6d2e 6a73 6f6e 202d 6420  ies.ftm.json -d 
+00000c40: 3c61 6469 7469 6f6e 616c 5f64 6174 6173  <aditional_datas
+00000c50: 6574 3e0a 0a4f 7665 7277 7269 7465 2064  et>..Overwrite d
+00000c60: 6174 6173 6574 733a 0a0a 2020 2020 6674  atasets:..    ft
+00000c70: 6d71 2061 7070 6c79 202d 6920 2e2f 656e  mq apply -i ./en
+00000c80: 7469 7469 6573 2e66 746d 2e6a 736f 6e20  tities.ftm.json 
+00000c90: 2d64 203c 6164 6974 696f 6e61 6c5f 6461  -d <aditional_da
+00000ca0: 7461 7365 743e 202d 2d72 6570 6c61 6365  taset> --replace
+00000cb0: 2d64 6174 6173 6574 0a0a 2323 2320 6674  -dataset..### ft
+00000cc0: 6d73 746f 7265 2028 6461 7461 6261 7365  mstore (database
+00000cd0: 2072 6561 6429 0a0a 2a2a 4e4f 5420 494d   read)..**NOT IM
+00000ce0: 504c 454d 454e 5445 4420 5945 542a 2a0a  PLEMENTED YET**.
+00000cf0: 0a54 6865 2073 616d 6520 636c 6920 6c6f  .The same cli lo
+00000d00: 6769 6320 6170 706c 6965 733a 0a0a 2020  gic applies:..  
+00000d10: 2020 6674 6d71 2073 746f 7265 2069 7465    ftmq store ite
+00000d20: 7261 7465 202d 6420 6563 5f6d 6565 7469  rate -d ec_meeti
+00000d30: 6e67 7320 2d73 2045 7665 6e74 202d 2d64  ngs -s Event --d
+00000d40: 6174 655f 5f67 7465 3d32 3031 3920 2d2d  ate__gte=2019 --
+00000d50: 6461 7465 5f5f 6c74 653d 3230 3230 0a0a  date__lte=2020..
+00000d60: 2323 2050 7974 686f 6e20 4c69 6272 6172  ## Python Librar
+00000d70: 790a 0a2a 2a4e 4f54 2049 4d50 4c45 4d45  y..**NOT IMPLEME
+00000d80: 4e54 4544 2059 4554 2a2a 0a0a 6060 6070  NTED YET**..```p
+00000d90: 7974 686f 6e0a 6672 6f6d 2066 746d 7120  ython.from ftmq 
+00000da0: 696d 706f 7274 2051 7565 7279 0a0a 7120  import Query..q 
+00000db0: 3d20 5175 6572 7928 656e 6769 6e65 3d22  = Query(engine="
+00000dc0: 7371 6c69 7465 2229 205c 0a20 2020 202e  sqlite") \.    .
+00000dd0: 7768 6572 6528 6461 7461 7365 743d 2265  where(dataset="e
+00000de0: 635f 6d65 6574 696e 6773 222c 2064 6174  c_meetings", dat
+00000df0: 655f 5f6c 7465 3d32 3032 3029 205c 0a20  e__lte=2020) \. 
+00000e00: 2020 202e 7768 6572 6528 7363 6865 6d61     .where(schema
+00000e10: 3d22 4576 656e 7422 2920 5c0a 2020 2020  ="Event") \.    
+00000e20: 2e6f 7264 6572 5f62 7928 2264 6174 6522  .order_by("date"
+00000e30: 2c20 6173 6365 6e64 696e 673d 4661 6c73  , ascending=Fals
+00000e40: 6529 0a0a 2320 7265 7375 6c74 696e 6720  e)..# resulting 
+00000e50: 7371 6c69 7465 2071 7565 7279 3a0a 7374  sqlite query:.st
+00000e60: 7228 7129 0a22 2222 0a53 454c 4543 5420  r(q).""".SELECT 
+00000e70: 742e 6964 2c0a 2020 2020 742e 7363 6865  t.id,.    t.sche
+00000e80: 6d61 2c0a 2020 2020 742e 656e 7469 7479  ma,.    t.entity
+00000e90: 2c0a 2020 2020 6a73 6f6e 5f65 7874 7261  ,.    json_extra
+00000ea0: 6374 2874 2e65 6e74 6974 792c 2027 242e  ct(t.entity, '$.
+00000eb0: 7072 6f70 6572 7469 6573 2e64 6174 6527  properties.date'
+00000ec0: 2920 4153 2064 6174 650a 4652 4f4d 2065  ) AS date.FROM e
+00000ed0: 635f 6d65 6574 696e 6773 2074 0a57 4845  c_meetings t.WHE
+00000ee0: 5245 0a20 2020 2028 4558 4953 5453 2028  RE.    (EXISTS (
+00000ef0: 5345 4c45 4354 2031 2046 524f 4d20 6a73  SELECT 1 FROM js
+00000f00: 6f6e 5f65 6163 6828 6461 7465 2920 5748  on_each(date) WH
+00000f10: 4552 4520 7661 6c75 6520 3c3d 203f 2929  ERE value <= ?))
+00000f20: 2041 4e44 2028 742e 7363 6865 6d61 203d   AND (t.schema =
+00000f30: 203f 290a 4f52 4445 5220 4259 2064 6174   ?).ORDER BY dat
+00000f40: 6520 4445 5343 0a22 2222 0a0a 2320 7061  e DESC."""..# pa
+00000f50: 7261 6d65 7465 7269 7a65 640a 5b70 2066  rameterized.[p f
+00000f60: 6f72 2070 2069 6e20 712e 7061 7261 6d65  or p in q.parame
+00000f70: 7465 7273 5d0a 5b32 3032 302c 2027 4576  ters].[2020, 'Ev
+00000f80: 656e 7427 5d0a 6060 600a 0a23 2320 7375  ent'].```..## su
+00000f90: 7070 6f72 740a 0a2a 5468 6973 2070 726f  pport..*This pro
+00000fa0: 6a65 6374 2069 7320 7061 7274 206f 6620  ject is part of 
+00000fb0: 5b69 6e76 6573 7469 6772 6170 685d 2868  [investigraph](h
+00000fc0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000fd0: 6d2f 696e 7665 7374 6967 6174 6976 6564  m/investigatived
+00000fe0: 6174 612f 696e 7665 7374 6967 7261 7068  ata/investigraph
+00000ff0: 292a 0a0a 5b4d 6564 6961 2054 6563 6820  )*..[Media Tech 
+00001000: 4c61 6220 4261 7965 726e 2062 6174 6368  Lab Bayern batch
+00001010: 2023 335d 2868 7474 7073 3a2f 2f67 6974   #3](https://git
+00001020: 6875 622e 636f 6d2f 6d65 6469 612d 7465  hub.com/media-te
+00001030: 6368 2d6c 6162 290a 0a3c 6120 6872 6566  ch-lab)..<a href
+00001040: 3d22 6874 7470 733a 2f2f 7777 772e 6d65  ="https://www.me
+00001050: 6469 612d 6c61 622e 6465 2f65 6e2f 7072  dia-lab.de/en/pr
+00001060: 6f67 7261 6d73 2f6d 6564 6961 2d74 6563  ograms/media-tec
+00001070: 682d 6c61 6222 3e0a 2020 2020 3c69 6d67  h-lab">.    <img
+00001080: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
+00001090: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
+000010a0: 656e 742e 636f 6d2f 6d65 6469 612d 7465  ent.com/media-te
+000010b0: 6368 2d6c 6162 2f2e 6769 7468 7562 2f6d  ch-lab/.github/m
+000010c0: 6169 6e2f 6173 7365 7473 2f6d 746c 2d70  ain/assets/mtl-p
+000010d0: 6f77 6572 6564 2d62 792e 706e 6722 2077  owered-by.png" w
+000010e0: 6964 7468 3d22 3234 3022 2074 6974 6c65  idth="240" title
+000010f0: 3d22 4d65 6469 6120 5465 6368 204c 6162  ="Media Tech Lab
+00001100: 2070 6f77 6572 6564 2062 7920 6c6f 676f   powered by logo
+00001110: 223e 0a3c 2f61 3e0a                      ">.</a>.
```

### Comparing `ftmq-0.1.2/ftmq/filters.py` & `ftmq-0.1.3/ftmq/filters.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.1.2/ftmq/io.py` & `ftmq-0.1.3/ftmq/io.py`

 * *Files 19% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         while True:
             line = fh.readline()
             if not line:
                 break
             data = orjson.loads(line)
             if serialize:
                 data = load_proxy(data)
+            data.datasets.discard("default")
             yield data
 
 
 def smart_write_proxies(
     uri: PathLike,
     proxies: Iterable[CE | SDict],
     mode: str | None = "wb",
@@ -57,7 +58,19 @@
     with smart_open(uri, sys.stdout.buffer, mode=mode) as fh:
         for proxy in proxies:
             ix += 1
             if serialize:
                 proxy = proxy.to_dict()
             fh.write(orjson.dumps(proxy, option=orjson.OPT_APPEND_NEWLINE))
     return ix
+
+
+def apply_datasets(
+    proxies: Iterable[CE], *datasets: Iterable[str], replace: bool | None = False
+) -> CEGenerator:
+    for proxy in proxies:
+        if datasets:
+            if replace:
+                proxy.datasets = set(datasets)
+            else:
+                proxy.datasets.update(datasets)
+        yield proxy
```

### Comparing `ftmq-0.1.2/ftmq/query.py` & `ftmq-0.1.3/ftmq/query.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.1.2/pyproject.toml` & `ftmq-0.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ftmq"
-version = "0.1.2"
+version = "0.1.3"
 description = "followthemoney query dsl and io helpers"
 authors = ["Simon Wörpel <simon.woerpel@pm.me>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/investigativedata/ftmq"
 repository = "https://github.com/investigativedata/ftmq"
 documentation = "https://github.com/investigativedata/ftmq"
@@ -27,16 +27,17 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 banal = "^1.0.6"
 followthemoney = "^3.4.0"
 nomenklatura = "^2.14.0"
 orjson = "^3.9.1"
 PyICU = "^2.11"
-typer = "^0.9.0"
 smart-open = {version = "6.3.0", extras = ["all"]}
+click = "^8.1.3"
+click-default-group = "^1.2.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.2"
 pytest-cov = "^4.1.0"
 black = "^23.3.0"
 isort = "^5.12.0"
 mypy = "^1.3.0"
```

### Comparing `ftmq-0.1.2/PKG-INFO` & `ftmq-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftmq
-Version: 0.1.2
+Version: 0.1.3
 Summary: followthemoney query dsl and io helpers
 Home-page: https://github.com/investigativedata/ftmq
 License: MIT
 Author: Simon Wörpel
 Author-email: simon.woerpel@pm.me
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
@@ -12,19 +12,20 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyICU (>=2.11,<3.0)
 Requires-Dist: banal (>=1.0.6,<2.0.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: click-default-group (>=1.2.2,<2.0.0)
 Requires-Dist: followthemoney (>=3.4.0,<4.0.0)
 Requires-Dist: nomenklatura (>=2.14.0,<3.0.0)
 Requires-Dist: orjson (>=3.9.1,<4.0.0)
 Requires-Dist: smart-open[all] (==6.3.0)
-Requires-Dist: typer (>=0.9.0,<0.10.0)
 Project-URL: Bug Tracker, https://github.com/investigativedata/ftmq/issues
 Project-URL: Documentation, https://github.com/investigativedata/ftmq
 Project-URL: Repository, https://github.com/investigativedata/ftmq
 Description-Content-Type: text/markdown
 
 [![ftmq on pypi](https://img.shields.io/pypi/v/ftmq)](https://pypi.org/project/ftmq/) [![Python test and package](https://github.com/investigativedata/ftmq/actions/workflows/python.yml/badge.svg)](https://github.com/investigativedata/ftmq/actions/workflows/python.yml) [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit) [![Coverage Status](https://coveralls.io/repos/github/investigativedata/ftmq/badge.svg?branch=main)](https://coveralls.io/github/investigativedata/ftmq?branch=main) [![MIT License](https://img.shields.io/pypi/l/ftmq)](./LICENSE)
 
@@ -100,22 +101,38 @@
 - `lt` - lower than
 - `gte` - greater or equal
 - `lte` - lower or equal
 - `like` - SQLish `LIKE` (use `%` placeholders)
 - `ilike` - SQLish `ILIKE`, case-insensitive (use `%` placeholders)
 - `[]` - usage: `prop[]=foo` evaluates if `foo` is member of array `prop`
 
+
+### ftmq apply
+
+"Uplevel" an entity input stream to `nomenklatura.entity.CompositeEntity` and
+optionally apply a dataset.
+
+    ftmq apply -i ./entities.ftm.json -d <aditional_dataset>
+
+Overwrite datasets:
+
+    ftmq apply -i ./entities.ftm.json -d <aditional_dataset> --replace-dataset
+
 ### ftmstore (database read)
 
+**NOT IMPLEMENTED YET**
+
 The same cli logic applies:
 
     ftmq store iterate -d ec_meetings -s Event --date__gte=2019 --date__lte=2020
 
 ## Python Library
 
+**NOT IMPLEMENTED YET**
+
 ```python
 from ftmq import Query
 
 q = Query(engine="sqlite") \
     .where(dataset="ec_meetings", date__lte=2020) \
     .where(schema="Event") \
     .order_by("date", ascending=False)
```

