# Comparing `tmp/nonebot_plugin_heweather-0.6.6.tar.gz` & `tmp/nonebot_plugin_heweather-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_heweather-0.6.6.tar", max compression
+gzip compressed data, was "nonebot_plugin_heweather-0.6.7.tar", last modified: Wed Jun 21 07:52:51 2023, max compression
```

## Comparing `nonebot_plugin_heweather-0.6.6.tar` & `nonebot_plugin_heweather-0.6.7.tar`

### file list

```diff
@@ -1,16 +1,20 @@
--rw-r--r--   0        0        0     1062 2023-05-18 13:53:48.324067 nonebot_plugin_heweather-0.6.6/LICENSE
--rw-r--r--   0        0        0     1455 2023-05-18 13:53:48.324067 nonebot_plugin_heweather-0.6.6/README.md
--rw-r--r--   0        0        0     1812 2023-05-18 13:53:48.324067 nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/__init__.py
--rw-r--r--   0        0        0      223 2023-05-18 13:53:48.324067 nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/config.py
--rw-r--r--   0        0        0     1104 2023-05-18 13:53:48.324067 nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/model.py
--rw-r--r--   0        0        0     1785 2023-05-18 13:53:48.324067 nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/render_pic.py
--rwxr-xr-x   0        0        0    69948 2023-05-18 13:53:48.328068 nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.ttf
--rwxr-xr-x   0        0        0    27920 2023-05-18 13:53:48.328068 nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.woff
--rwxr-xr-x   0        0        0    19688 2023-05-18 13:53:48.328068 nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.woff2
--rwxr-xr-x   0        0        0    20240 2023-05-18 13:53:48.328068 nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/templates/css/qweather-icons.css
--rwxr-xr-x   0        0        0     9784 2023-05-18 13:53:48.328068 nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/templates/css/qweather-icons.json
--rw-r--r--   0        0        0     2850 2023-05-18 13:53:48.328068 nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/templates/css/weather.css
--rw-r--r--   0        0        0     5219 2023-05-18 13:53:48.328068 nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/templates/weather.html
--rw-r--r--   0        0        0     4960 2023-05-18 13:53:48.328068 nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/weather_data.py
--rw-r--r--   0        0        0      839 2023-05-18 13:53:48.328068 nonebot_plugin_heweather-0.6.6/pyproject.toml
--rw-r--r--   0        0        0     2234 1970-01-01 00:00:00.000000 nonebot_plugin_heweather-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-21 07:52:36.993460 nonebot_plugin_heweather-0.6.7/LICENSE
+-rw-r--r--   0        0        0     2272 2023-06-21 07:52:36.993460 nonebot_plugin_heweather-0.6.7/README.md
+-rw-r--r--   0        0        0     1867 2023-06-21 07:52:36.997460 nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/__init__.py
+-rw-r--r--   0        0        0      435 2023-06-21 07:52:36.997460 nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/config.py
+-rw-r--r--   0        0        0     1104 2023-06-21 07:52:36.997460 nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/model.py
+-rw-r--r--   0        0        0     1785 2023-06-21 07:52:36.997460 nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/render_pic.py
+-rwxr-xr-x   0        0        0    69948 2023-06-21 07:52:37.001460 nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.ttf
+-rwxr-xr-x   0        0        0    27920 2023-06-21 07:52:37.001460 nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.woff
+-rwxr-xr-x   0        0        0    19688 2023-06-21 07:52:37.001460 nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.woff2
+-rwxr-xr-x   0        0        0    20240 2023-06-21 07:52:37.001460 nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/templates/css/qweather-icons.css
+-rwxr-xr-x   0        0        0     9784 2023-06-21 07:52:37.001460 nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/templates/css/qweather-icons.json
+-rw-r--r--   0        0        0     2850 2023-06-21 07:52:37.001460 nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/templates/css/weather.css
+-rw-r--r--   0        0        0     5219 2023-06-21 07:52:37.001460 nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/templates/weather.html
+-rw-r--r--   0        0        0     4978 2023-06-21 07:52:37.001460 nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/weather_data.py
+-rw-r--r--   0        0        0      831 2023-06-21 07:52:51.905481 nonebot_plugin_heweather-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0        6 2023-06-21 07:52:37.001460 nonebot_plugin_heweather-0.6.7/tests/.gitignore
+-rw-r--r--   0        0        0        0 2023-06-21 07:52:37.001460 nonebot_plugin_heweather-0.6.7/tests/__init__.py
+-rw-r--r--   0        0        0      487 2023-06-21 07:52:37.001460 nonebot_plugin_heweather-0.6.7/tests/conftest.py
+-rw-r--r--   0        0        0      784 2023-06-21 07:52:37.001460 nonebot_plugin_heweather-0.6.7/tests/test_heweather.py
+-rw-r--r--   0        0        0     2725 1970-01-01 00:00:00.000000 nonebot_plugin_heweather-0.6.7/PKG-INFO
```

### Comparing `nonebot_plugin_heweather-0.6.6/LICENSE` & `nonebot_plugin_heweather-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.6/README.md` & `nonebot_plugin_heweather-0.6.7/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,91 +1,142 @@
-00000000: 2320 6e6f 6e65 626f 742d 706c 7567 696e  # nonebot-plugin
-00000010: 2d68 6577 6561 7468 6572 0a0a e88e b7e5  -heweather......
-00000020: 8f96 e592 8ce9 a38e e5a4 a9e6 b094 e4bf  ................
-00000030: a1e6 81af e5b9 b6e8 bdac e68d a2e4 b8ba  ................
-00000040: e59b bee7 8987 0a0a 2320 e4bd bfe7 94a8  ........# ......
-00000050: 6874 6d6c 2b70 6c61 7977 7269 6768 74e6  html+playwright.
-00000060: 9da5 e6b8 b2e6 9f93 e5a5 bde7 9c8b e79a  ................
-00000070: 84ef bc81 0a0a 2d20 e4bd bfe7 94a8 e4ba  ......- ........
-00000080: 867e 7ee8 87aa e4ba a7e8 87aa e994 80e7  .~~.............
-00000090: 9a84 7e7e 5b6e 6f6e 6562 6f74 2d70 6c75  ..~~[nonebot-plu
-000000a0: 6769 6e2d 6874 6d6c 7265 6e64 6572 5d28  gin-htmlrender](
-000000b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000000c0: 6f6d 2f6b 6578 7565 2d7a 2f6e 6f6e 6562  om/kexue-z/noneb
-000000d0: 6f74 2d70 6c75 6769 6e2d 6874 6d6c 7265  ot-plugin-htmlre
-000000e0: 6e64 6572 290a 2d20 2a2a e99c 80e8 a681  nder).- **......
-000000f0: e585 88e4 bf9d e8af 8170 6c61 7977 7269  .........playwri
-00000100: 6768 74e5 8faf e4bb a5e6 ada3 e5b8 b8e8  ght.............
-00000110: bf90 e8a1 8ce5 b9b6 e59c a8e7 b3bb e7bb  ................
-00000120: 9fef bc88 e688 96e5 aeb9 e599 a8e4 b8ad  ................
-00000130: efbc 89e5 ad98 e59c a8e4 b8ad e696 87e5  ................
-00000140: ad97 e4bd 932a 2a0a 0a0a 2320 e5ae 89e8  .....**...# ....
-00000150: a385 0a0a e79b b4e6 8ea5 e4bd bfe7 94a8  ................
-00000160: 2060 7069 7020 696e 7374 616c 6c20 6e6f   `pip install no
-00000170: 6e65 626f 742d 706c 7567 696e 2d68 6577  nebot-plugin-hew
-00000180: 6561 7468 6572 6020 e8bf 9be8 a18c e5ae  eather` ........
-00000190: 89e8 a385 0a0a e59c a820 6062 6f74 2e70  ......... `bot.p
-000001a0: 7960 20e4 b8ad 20e5 8699 e585 a520 606e  y` ... ...... `n
-000001b0: 6f6e 6562 6f74 2e6c 6f61 645f 706c 7567  onebot.load_plug
-000001c0: 696e 2822 6e6f 6e65 626f 745f 706c 7567  in("nonebot_plug
-000001d0: 696e 5f68 6577 6561 7468 6572 2229 600a  in_heweather")`.
-000001e0: 0a23 20e6 8c87 e4bb a40a 0a60 e5a4 a9e6  .# ........`....
-000001f0: b094 2be5 9cb0 e58c ba60 20e6 8896 2060  ..+......` ... `
-00000200: e59c b0e5 8cba 2be5 a4a9 e6b0 9460 2020  ......+......`  
-00000210: 0ae4 be8b e5a6 82ef bc9a 60e4 b88a e6b5  ..........`.....
-00000220: b7e5 a4a9 e6b0 9460 20e6 8896 2060 e5a4  .......` ... `..
-00000230: a9e6 b094 e5b9 bfe5 b79e 600a 0a23 20e9  ..........`..# .
-00000240: 858d e7bd ae0a 0a23 2320 6170 696b 6579  .......## apikey
-00000250: 20e5 bf85 e9a1 bbe9 858d e7bd ae20 e78e   ............ ..
-00000260: afe5 a283 e985 8de7 bdae 0a0a 6060 600a  ............```.
-00000270: 5157 4541 5448 4552 5f41 5049 4b45 5920  QWEATHER_APIKEY 
-00000280: 3d20 7878 780a 6060 600a 0a23 2320 6170  = xxx.```..## ap
-00000290: 69e7 b1bb e59e 8b20 e5bf 85e9 a1bb e985  i...... ........
-000002a0: 8de7 bdae 20e7 8eaf e5a2 83e9 858d e7bd  .... ...........
-000002b0: ae0a 0a30 203d 20e6 99ae e980 9ae7 8988  ...0 = .........
-000002c0: 2833 e5a4 a9e5 a4a9 e6b0 94e9 a284 e68a  (3..............
-000002d0: a529 0a31 203d 20e4 b8aa e4ba bae5 bc80  .).1 = .........
-000002e0: e58f 91e7 8988 2837 e5a4 a9e5 a4a9 e6b0  ......(7........
-000002f0: 94e9 a284 e68a a529 0a32 203d 20e5 9586  .......).2 = ...
-00000300: e4b8 9ae7 8988 2028 37e5 a4a9 e5a4 a9e6  ...... (7.......
-00000310: b094 e9a2 84e6 8aa5 290a 0a0a 6060 600a  ........)...```.
-00000320: 5157 4541 5448 4552 5f41 5049 5459 5045  QWEATHER_APITYPE
-00000330: 203d 2030 0a60 6060 0a0a 2323 2041 5049   = 0.```..## API
-00000340: 4b45 59e8 8eb7 e58f 96e6 96b9 e5bc 8f0a  KEY.............
-00000350: 0a2a 2a31 e380 81e6 b3a8 e586 8ce5 928c  .**1............
-00000360: e9a3 8ee5 a4a9 e6b0 94e8 b4a6 e58f b72a  ...............*
-00000370: 2a20 200a e8bf 9be5 85a5 e5ae 98e7 bd91  *  .............
-00000380: e6b3 a8e5 868c 5b68 7474 7073 3a2f 2f69  ......[https://i
-00000390: 642e 7177 6561 7468 6572 2e63 6f6d 2f23  d.qweather.com/#
-000003a0: 2f6c 6f67 696e 5d28 6874 7470 733a 2f2f  /login](https://
-000003b0: 6964 2e71 7765 6174 6865 722e 636f 6d2f  id.qweather.com/
-000003c0: 232f 6c6f 6769 6e29 2020 0a2a 2a32 e380  #/login)  .**2..
-000003d0: 81e8 bf9b e585 a5e6 8ea7 e588 b6e5 8fb0  ................
-000003e0: 2a2a 2020 0ae7 99bb e5bd 95e5 908e efbc  **  ............
-000003f0: 8ce7 82b9 e587 bb20 e280 9ce5 928c e9a3  ....... ........
-00000400: 8ee5 a4a9 e6b0 94e5 bc80 e58f 91e8 8085  ................
-00000410: e68e a7e5 88b6 e58f b0e2 809d 2020 0a2a  ............  .*
-00000420: 2a33 e380 81e5 889b e5bb bae9 a1b9 e79b  *3..............
-00000430: ae2a 2a20 200a e782 b9e5 87bb e68e a7e5  .**  ...........
-00000440: 88b6 e58f b0e5 b7a6 e4be a720 e280 9ce9  ........... ....
-00000450: a1b9 e79b aee7 aea1 e790 86e2 809d efbc  ................
-00000460: 8ce7 84b6 e590 8ee7 82b9 e587 bb20 e280  ............. ..
-00000470: 9ce5 889b e5bb bae9 a1b9 e79b aee2 809d  ................
-00000480: efbc 8ce6 a0b9 e68d aee6 8f90 e7a4 bae8  ................
-00000490: 87aa e8a1 8ce5 a1ab e586 9920 200a e280  ...........  ...
-000004a0: 9ce9 8089 e68b a9e8 aea2 e998 85e2 809d  ................
-000004b0: 202d 3e20 e280 9ce5 858d e8b4 b9e8 aea2   -> ............
-000004c0: e998 85e2 809d efbc 8ce2 809c e8ae bee7  ................
-000004d0: bdae 4b45 59e2 809d 202d 3e20 e280 9c57  ..KEY... -> ...W
-000004e0: 6562 2041 5049 e280 9def bc8c e983 bde5  eb API..........
-000004f0: a1ab e5a5 bde5 908e e280 9ce5 889b e5bb  ................
-00000500: bae2 809d 2020 0a2a 2a34 e380 81e8 8eb7  ....  .**4......
-00000510: e58f 966b 6579 e5b9 b6e9 858d e7bd ae2e  ...key..........
-00000520: 656e 762e 7878 2a2a 2020 0ae8 bf94 e59b  env.xx**  ......
-00000530: 9e20 e280 9ce9 a1b9 e79b aee7 aea1 e790  . ..............
-00000540: 86e2 809d efbc 8ce5 8faf e4bb a5e7 9c8b  ................
-00000550: e588 b0e5 889b e5bb bae7 9a84 e9a1 b9e7  ................
-00000560: 9bae efbc 8ce7 82b9 e587 bb4b 4559 e4b8  ...........KEY..
-00000570: 8be9 9da2 e79a 8420 e280 9ce6 9fa5 e79c  ....... ........
-00000580: 8be2 809d efbc 8ce5 a48d e588 b64b 4559  .............KEY
-00000590: e588 b0e4 bda0 e79a 842e 656e 762e 7878  ..........env.xx
-000005a0: e58d b3e5 8faf e380 8220 200a 200a 0a    .........  . ..
+00000000: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+00000010: 223e 0a20 203c 6120 6872 6566 3d22 6874  ">.  <a href="ht
+00000020: 7470 733a 2f2f 7632 2e6e 6f6e 6562 6f74  tps://v2.nonebot
+00000030: 2e64 6576 2f73 746f 7265 223e 3c69 6d67  .dev/store"><img
+00000040: 2073 7263 3d22 6874 7470 733a 2f2f 7573   src="https://us
+00000050: 6572 2d69 6d61 6765 732e 6769 7468 7562  er-images.github
+00000060: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00000070: 3434 3534 3536 3235 2f32 3039 3836 3235  44545625/2098625
+00000080: 3735 2d61 6364 6339 6665 622d 3363 3736  75-acdc9feb-3c76
+00000090: 2d34 3731 642d 6164 3839 2d63 6337 3839  -471d-ad89-cc789
+000000a0: 3237 6535 3837 352e 706e 6722 2077 6964  27e5875.png" wid
+000000b0: 7468 3d22 3138 3022 2068 6569 6768 743d  th="180" height=
+000000c0: 2231 3830 2220 616c 743d 224e 6f6e 6542  "180" alt="NoneB
+000000d0: 6f74 506c 7567 696e 4c6f 676f 223e 3c2f  otPluginLogo"></
+000000e0: 613e 0a3c 2f70 3e0a 0a3c 6469 7620 616c  a>.</p>..<div al
+000000f0: 6967 6e3d 2263 656e 7465 7222 3e0a 0a23  ign="center">..#
+00000100: 206e 6f6e 6562 6f74 2d70 6c75 6769 6e2d   nonebot-plugin-
+00000110: 6865 7765 6174 6865 720a 0a5f e29c a820  heweather.._... 
+00000120: e88e b7e5 8f96 e592 8ce9 a38e e5a4 a9e6  ................
+00000130: b094 e4bf a1e6 81af e5b9 b6e8 bdac e68d  ................
+00000140: a2e4 b8ba e59b bee7 8987 20e2 9ca8 5f0a  .......... ..._.
+00000150: 0a3c 2f64 6976 3e0a 0a3c 7020 616c 6967  .</div>..<p alig
+00000160: 6e3d 2263 656e 7465 7222 3e0a 2020 3c61  n="center">.  <a
+00000170: 2068 7265 663d 2268 7474 7073 3a2f 2f72   href="https://r
+00000180: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
+00000190: 7465 6e74 2e63 6f6d 2f6b 6578 7565 2d7a  tent.com/kexue-z
+000001a0: 2f6e 6f6e 6562 6f74 2d70 6c75 6769 6e2d  /nonebot-plugin-
+000001b0: 6865 7765 6174 6865 722f 6d61 7374 6572  heweather/master
+000001c0: 2f4c 4943 454e 5345 223e 0a20 2020 203c  /LICENSE">.    <
+000001d0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+000001e0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+000001f0: 6769 7468 7562 2f6c 6963 656e 7365 2f6b  github/license/k
+00000200: 6578 7565 2d7a 2f6e 6f6e 6562 6f74 2d70  exue-z/nonebot-p
+00000210: 6c75 6769 6e2d 6865 7765 6174 6865 722e  lugin-heweather.
+00000220: 7376 6722 2061 6c74 3d22 6c69 6365 6e73  svg" alt="licens
+00000230: 6522 3e0a 2020 3c2f 613e 0a20 203c 6120  e">.  </a>.  <a 
+00000240: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
+00000250: 7069 2e6f 7267 2f70 726f 6a65 6374 2f6e  pi.org/project/n
+00000260: 6f6e 6562 6f74 2d70 6c75 6769 6e2d 6865  onebot-plugin-he
+00000270: 7765 6174 6865 722f 223e 0a20 2020 203c  weather/">.    <
+00000280: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00000290: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+000002a0: 7079 7069 2f76 2f6e 6f6e 6562 6f74 2d70  pypi/v/nonebot-p
+000002b0: 6c75 6769 6e2d 6865 7765 6174 6865 7222  lugin-heweather"
+000002c0: 2061 6c74 3d22 7079 7069 223e 0a20 203c   alt="pypi">.  <
+000002d0: 2f61 3e0a 2020 3c69 6d67 2073 7263 3d22  /a>.  <img src="
+000002e0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000002f0: 6c64 732e 696f 2f62 6164 6765 2f70 7974  lds.io/badge/pyt
+00000300: 686f 6e2d 332e 382b 2d62 6c75 652e 7376  hon-3.8+-blue.sv
+00000310: 6722 2061 6c74 3d22 7079 7468 6f6e 223e  g" alt="python">
+00000320: 0a3c 2f70 3e0a 0a3c 6469 7620 616c 6967  .</p>..<div alig
+00000330: 6e3d 2263 656e 7465 7222 3e0a 0a23 20e4  n="center">..# .
+00000340: bdbf e794 a820 6874 6d6c 2b70 6c61 7977  ..... html+playw
+00000350: 7269 6768 7420 e69d a5e6 b8b2 e69f 93e5  right ..........
+00000360: a5bd e79c 8be7 9a84 efbc 810a 0a3c 696d  .............<im
+00000370: 6720 7372 633d 2264 6f63 732f 7765 6174  g src="docs/weat
+00000380: 6865 722e 706e 6722 2020 7769 6474 683d  her.png"  width=
+00000390: 2235 3025 223e 0a3c 2f64 6976 3e0a 0a2d  "50%">.</div>..-
+000003a0: 20e4 bdbf e794 a8e4 ba86 7e7e e887 aae4   .........~~....
+000003b0: baa7 e887 aae9 9480 e79a 847e 7e5b 6e6f  ...........~~[no
+000003c0: 6e65 626f 742d 706c 7567 696e 2d68 746d  nebot-plugin-htm
+000003d0: 6c72 656e 6465 725d 2868 7474 7073 3a2f  lrender](https:/
+000003e0: 2f67 6974 6875 622e 636f 6d2f 6b65 7875  /github.com/kexu
+000003f0: 652d 7a2f 6e6f 6e65 626f 742d 706c 7567  e-z/nonebot-plug
+00000400: 696e 2d68 746d 6c72 656e 6465 7229 0a2d  in-htmlrender).-
+00000410: 202a 2ae9 9c80 e8a6 81e5 8588 e4bf 9de8   **.............
+00000420: af81 2070 6c61 7977 7269 6768 7420 e58f  .. playwright ..
+00000430: afe4 bba5 e6ad a3e5 b8b8 e8bf 90e8 a18c  ................
+00000440: e5b9 b6e5 9ca8 e7b3 bbe7 bb9f efbc 88e6  ................
+00000450: 8896 e5ae b9e5 99a8 e4b8 adef bc89 e5ad  ................
+00000460: 98e5 9ca8 e4b8 ade6 9687 e5ad 97e4 bd93  ................
+00000470: 2a2a 0a0a 2320 e5ae 89e8 a385 0a0a e79b  **..# ..........
+00000480: b4e6 8ea5 e4bd bfe7 94a8 2060 7069 7020  .......... `pip 
+00000490: 696e 7374 616c 6c20 6e6f 6e65 626f 742d  install nonebot-
+000004a0: 706c 7567 696e 2d68 6577 6561 7468 6572  plugin-heweather
+000004b0: 6020 e8bf 9be8 a18c e5ae 89e8 a385 0a0a  ` ..............
+000004c0: e59c a820 6062 6f74 2e70 7960 20e4 b8ad  ... `bot.py` ...
+000004d0: 20e5 8699 e585 a520 606e 6f6e 6562 6f74   ...... `nonebot
+000004e0: 2e6c 6f61 645f 706c 7567 696e 2822 6e6f  .load_plugin("no
+000004f0: 6e65 626f 745f 706c 7567 696e 5f68 6577  nebot_plugin_hew
+00000500: 6561 7468 6572 2229 600a 0a23 20e6 8c87  eather")`..# ...
+00000510: e4bb a40a 0a60 e5a4 a9e6 b094 2be5 9cb0  .....`......+...
+00000520: e58c ba60 20e6 8896 2060 e59c b0e5 8cba  ...` ... `......
+00000530: 2be5 a4a9 e6b0 9460 2020 0ae4 be8b e5a6  +......`  ......
+00000540: 82ef bc9a 60e4 b88a e6b5 b7e5 a4a9 e6b0  ....`...........
+00000550: 9460 20e6 8896 2060 e5a4 a9e6 b094 e5b9  .` ... `........
+00000560: bfe5 b79e 600a 0a23 20e9 858d e7bd ae0a  ....`..# .......
+00000570: 0a23 2320 6170 696b 6579 20e5 bf85 e9a1  .## apikey .....
+00000580: bbe9 858d e7bd ae20 e78e afe5 a283 e985  ....... ........
+00000590: 8de7 bdae 0a0a 6060 600a 5157 4541 5448  ......```.QWEATH
+000005a0: 4552 5f41 5049 4b45 5920 3d20 7878 780a  ER_APIKEY = xxx.
+000005b0: 6060 600a 0a23 2320 6170 6920 e7b1 bbe5  ```..## api ....
+000005c0: 9e8b 20e5 bf85 e9a1 bbe9 858d e7bd ae20  .. ............ 
+000005d0: e78e afe5 a283 e985 8de7 bdae 0a0a 3020  ..............0 
+000005e0: 3d20 e699 aee9 809a e789 8828 3320 e5a4  = .........(3 ..
+000005f0: a9e5 a4a9 e6b0 94e9 a284 e68a a529 0a31  .............).1
+00000600: 203d 20e4 b8aa e4ba bae5 bc80 e58f 91e7   = .............
+00000610: 8988 2837 20e5 a4a9 e5a4 a9e6 b094 e9a2  ..(7 ...........
+00000620: 84e6 8aa5 290a 3220 3d20 e595 86e4 b89a  ....).2 = ......
+00000630: e789 8820 2837 20e5 a4a9 e5a4 a9e6 b094  ... (7 .........
+00000640: e9a2 84e6 8aa5 290a 0a60 6060 0a51 5745  ......)..```.QWE
+00000650: 4154 4845 525f 4150 4954 5950 4520 3d20  ATHER_APITYPE = 
+00000660: 300a 6060 600a 0a23 2320 4150 494b 4559  0.```..## APIKEY
+00000670: 20e8 8eb7 e58f 96e6 96b9 e5bc 8f0a 0a2a   ..............*
+00000680: 2a31 e380 81e6 b3a8 e586 8ce5 928c e9a3  *1..............
+00000690: 8ee5 a4a9 e6b0 94e8 b4a6 e58f b72a 2a20  .............** 
+000006a0: 200a e8bf 9be5 85a5 e5ae 98e7 bd91 e6b3   ...............
+000006b0: a8e5 868c 5b68 7474 7073 3a2f 2f69 642e  ....[https://id.
+000006c0: 7177 6561 7468 6572 2e63 6f6d 2f23 2f6c  qweather.com/#/l
+000006d0: 6f67 696e 5d28 6874 7470 733a 2f2f 6964  ogin](https://id
+000006e0: 2e71 7765 6174 6865 722e 636f 6d2f 232f  .qweather.com/#/
+000006f0: 6c6f 6769 6e29 2020 0a2a 2a32 e380 81e8  login)  .**2....
+00000700: bf9b e585 a5e6 8ea7 e588 b6e5 8fb0 2a2a  ..............**
+00000710: 2020 0ae7 99bb e5bd 95e5 908e efbc 8ce7    ..............
+00000720: 82b9 e587 bb20 e280 9ce5 928c e9a3 8ee5  ..... ..........
+00000730: a4a9 e6b0 94e5 bc80 e58f 91e8 8085 e68e  ................
+00000740: a7e5 88b6 e58f b0e2 809d 2020 0a2a 2a33  ..........  .**3
+00000750: e380 81e5 889b e5bb bae9 a1b9 e79b ae2a  ...............*
+00000760: 2a20 200a e782 b9e5 87bb e68e a7e5 88b6  *  .............
+00000770: e58f b0e5 b7a6 e4be a720 e280 9ce9 a1b9  ......... ......
+00000780: e79b aee7 aea1 e790 86e2 809d efbc 8ce7  ................
+00000790: 84b6 e590 8ee7 82b9 e587 bb20 e280 9ce5  ........... ....
+000007a0: 889b e5bb bae9 a1b9 e79b aee2 809d efbc  ................
+000007b0: 8ce6 a0b9 e68d aee6 8f90 e7a4 bae8 87aa  ................
+000007c0: e8a1 8ce5 a1ab e586 9920 200a e280 9ce9  .........  .....
+000007d0: 8089 e68b a9e8 aea2 e998 85e2 809d 202d  .............. -
+000007e0: 3e20 e280 9ce5 858d e8b4 b9e8 aea2 e998  > ..............
+000007f0: 85e2 809d efbc 8ce2 809c e8ae bee7 bdae  ................
+00000800: 204b 4559 e280 9d20 2d3e 20e2 809c 5765   KEY... -> ...We
+00000810: 6220 4150 49e2 809d efbc 8ce9 83bd e5a1  b API...........
+00000820: abe5 a5bd e590 8ee2 809c e588 9be5 bbba  ................
+00000830: e280 9d20 200a 2a2a 34e3 8081 e88e b7e5  ...  .**4.......
+00000840: 8f96 206b 6579 20e5 b9b6 e985 8de7 bdae  .. key .........
+00000850: 2e65 6e76 2e78 782a 2a20 200a e8bf 94e5  .env.xx**  .....
+00000860: 9b9e 20e2 809c e9a1 b9e7 9bae e7ae a1e7  .. .............
+00000870: 9086 e280 9def bc8c e58f afe4 bba5 e79c  ................
+00000880: 8be5 88b0 e588 9be5 bbba e79a 84e9 a1b9  ................
+00000890: e79b aeef bc8c e782 b9e5 87bb 204b 4559  ............ KEY
+000008a0: 20e4 b88b e99d a2e7 9a84 20e2 809c e69f   ......... .....
+000008b0: a5e7 9c8b e280 9def bc8c e5a4 8de5 88b6  ................
+000008c0: 204b 4559 20e5 88b0 e4bd a0e7 9a84 2e65   KEY ..........e
+000008d0: 6e76 2e78 7820 e58d b3e5 8faf e380 820a  nv.xx ..........
```

### Comparing `nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/model.py` & `nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/render_pic.py` & `nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/render_pic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.ttf` & `nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.woff` & `nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.woff`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.woff2` & `nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/templates/css/fonts/qweather-icons.woff2`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/templates/css/qweather-icons.css` & `nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/templates/css/qweather-icons.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/templates/css/qweather-icons.json` & `nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/templates/css/qweather-icons.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/templates/css/weather.css` & `nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/templates/css/weather.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/templates/weather.html` & `nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/templates/weather.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_heweather-0.6.6/nonebot_plugin_heweather/weather_data.py` & `nonebot_plugin_heweather-0.6.7/nonebot_plugin_heweather/weather_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,18 +40,18 @@
                 logger.info("使用个人开发版API")
         else:
             raise ConfigError(
                 "api_type 必须是为 (int)0 -> 普通版, (int)1 -> 个人开发版, (int)2 -> 商业版"
                 f"\n当前为: ({type(self.api_type)}){self.api_type}"
             )
 
-    def __init__(self, city_name: str, api_key: str, api_type: int = 0):
+    def __init__(self, city_name: str, api_key: str, api_type: int | str = 0):
         self.city_name = city_name
         self.apikey = api_key
-        self.api_type = api_type
+        self.api_type = int(api_type)
         self.__url__()
 
         # self.now: Optional[Dict[str, str]] = None
         # self.daily = None
         # self.air = None
         # self.warning = None
         self.__reference = "\n请参考: https://dev.qweather.com/docs/start/status-code/"
@@ -128,14 +128,14 @@
             url=self.url_air,
             params={"location": self.city_id, "key": self.apikey},
         )
         self._check_response(res)
         return AirApi(**res.json())
 
     @property
-    async def _warning(self) -> WarningApi:
+    async def _warning(self) -> WarningApi | None:
         res = await self._get_data(
             url=self.url_weather_warning,
             params={"location": self.city_id, "key": self.apikey},
         )
         self._check_response(res)
         return None if res.json().get("code") == "204" else WarningApi(**res.json())
```

