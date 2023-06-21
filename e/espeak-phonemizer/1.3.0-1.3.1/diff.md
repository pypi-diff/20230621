# Comparing `tmp/espeak_phonemizer-1.3.0.tar.gz` & `tmp/espeak_phonemizer-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "espeak_phonemizer-1.3.0.tar", last modified: Tue Apr 18 03:37:37 2023, max compression
+gzip compressed data, was "espeak_phonemizer-1.3.1.tar", last modified: Wed Jun 21 20:57:06 2023, max compression
```

## Comparing `espeak_phonemizer-1.3.0.tar` & `espeak_phonemizer-1.3.1.tar`

### file list

```diff
@@ -1,20 +1,509 @@
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-18 03:37:37.979704 espeak_phonemizer-1.3.0/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    35147 2021-10-11 19:22:13.000000 espeak_phonemizer-1.3.0/LICENSE
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2275 2023-04-18 03:37:37.979704 espeak_phonemizer-1.3.0/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1712 2021-10-11 19:22:13.000000 espeak_phonemizer-1.3.0/README.md
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-18 03:37:37.979704 espeak_phonemizer-1.3.0/espeak_phonemizer/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        6 2023-04-18 03:36:43.000000 espeak_phonemizer-1.3.0/espeak_phonemizer/VERSION
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     8182 2023-04-18 03:36:43.000000 espeak_phonemizer-1.3.0/espeak_phonemizer/__init__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3981 2021-10-11 19:22:13.000000 espeak_phonemizer-1.3.0/espeak_phonemizer/__main__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        0 2021-10-11 19:22:13.000000 espeak_phonemizer-1.3.0/espeak_phonemizer/py.typed
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-18 03:37:37.979704 espeak_phonemizer-1.3.0/espeak_phonemizer.egg-info/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2275 2023-04-18 03:37:37.000000 espeak_phonemizer-1.3.0/espeak_phonemizer.egg-info/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      400 2023-04-18 03:37:37.000000 espeak_phonemizer-1.3.0/espeak_phonemizer.egg-info/SOURCES.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-04-18 03:37:37.000000 espeak_phonemizer-1.3.0/espeak_phonemizer.egg-info/dependency_links.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       71 2023-04-18 03:37:37.000000 espeak_phonemizer-1.3.0/espeak_phonemizer.egg-info/entry_points.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       24 2023-04-18 03:37:37.000000 espeak_phonemizer-1.3.0/espeak_phonemizer.egg-info/top_level.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      113 2023-04-18 03:37:37.979704 espeak_phonemizer-1.3.0/setup.cfg
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1480 2022-03-18 20:12:33.000000 espeak_phonemizer-1.3.0/setup.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-18 03:37:37.979704 espeak_phonemizer-1.3.0/tests/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        0 2021-10-11 19:22:13.000000 espeak_phonemizer-1.3.0/tests/__init__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3085 2023-04-18 03:36:43.000000 espeak_phonemizer-1.3.0/tests/test_phonemizer.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.715498 espeak_phonemizer-1.3.1/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    35147 2023-06-21 20:51:52.000000 espeak_phonemizer-1.3.1/LICENSE
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2238 2023-06-21 20:57:06.715498 espeak_phonemizer-1.3.1/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1712 2023-06-21 20:51:52.000000 espeak_phonemizer-1.3.1/README.md
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.643498 espeak_phonemizer-1.3.1/espeak_phonemizer/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        6 2023-06-21 20:56:23.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/VERSION
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     8247 2023-06-21 20:56:00.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/__init__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3981 2023-06-21 20:51:52.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/__main__.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.643498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.643498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/aarch64/
+-rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)  1768752 2023-05-30 20:25:03.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/aarch64/libespeak-ng.so
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.679498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)   121473 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/af_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    63878 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/am_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6691 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/an_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)   478165 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/ar_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5005 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/as_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    43773 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/az_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2098 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/ba_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2652 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/be_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    87051 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/bg_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    89979 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/bn_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5226 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/bpy_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    47068 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/bs_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    45566 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/ca_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2859 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/chr_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)  1566335 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/cmn_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    49645 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/cs_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1344 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/cv_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    43130 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/cy_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)   245287 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/da_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    68276 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/de_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    72841 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/el_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)   166944 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/en_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4666 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/eo_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    49252 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/es_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    44263 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/et_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    48841 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/eu_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)   293235 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/fa_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    43928 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/fi_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    63727 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/fr_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    52673 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/ga_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    49121 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/gd_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3248 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/gn_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3433 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/grc_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    82480 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/gu_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3335 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/hak_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2443 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/haw_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6963 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/he_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    92143 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/hi_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    49388 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/hr_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1803 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/ht_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)   153785 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/hu_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    62263 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/hy_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)   331275 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/ia_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    43458 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/id_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2040 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/intonations
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2165 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/io_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    44354 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/is_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)   152889 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/it_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    47652 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/ja_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2243 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/jbo_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    87775 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/ka_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1859 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/kk_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2838 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/kl_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    87828 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/kn_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    47523 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/ko_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6394 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/kok_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2265 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/ku_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    64977 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/ky_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3806 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/la_dict
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.679498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.679498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/aav/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      111 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/aav/vi
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      143 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/aav/vi-VN-x-central
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      142 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/aav/vi-VN-x-south
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.679498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/art/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       41 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/art/eo
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       29 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/art/ia
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       50 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/art/io
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       69 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/art/jbo
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      135 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/art/lfn
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       56 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/art/piqd
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      140 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/art/py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       57 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/art/qdb
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      173 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/art/qya
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      175 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/art/sjn
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.679498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/azc/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      114 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/azc/nci
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.683498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/bat/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       28 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/bat/lt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      312 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/bat/ltg
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      229 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/bat/lv
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.683498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/bnt/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       41 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/bnt/sw
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       42 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/bnt/tn
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.683498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/ccs/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      124 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/ccs/ka
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.683498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/cel/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       37 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/cel/cy
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       66 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/cel/ga
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       51 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/cel/gd
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.683498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/cus/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       39 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/cus/om
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.683498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/dra/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       55 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/dra/kn
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       57 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/dra/ml
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       51 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/dra/ta
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       70 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/dra/te
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.683498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/esx/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       30 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/esx/kl
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       54 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/eu
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.683498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/gmq/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       43 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/gmq/da
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       27 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/gmq/is
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       87 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/gmq/nb
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       25 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/gmq/sv
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.683498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/gmw/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      123 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/gmw/af
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       42 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/gmw/de
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      140 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/gmw/en
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      335 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/gmw/en-029
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      295 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/gmw/en-GB-scotland
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      238 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/gmw/en-GB-x-gbclan
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      188 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/gmw/en-GB-x-gbcwmd
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      249 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/gmw/en-GB-x-rp
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      257 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/gmw/en-US
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      271 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/gmw/en-US-nyc
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       31 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/gmw/lb
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       23 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/gmw/nl
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.687498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/grk/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       23 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/grk/el
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       99 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/grk/grc
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.687498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/inc/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       42 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/inc/as
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       25 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/inc/bn
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       39 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/inc/bpy
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       42 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/inc/gu
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       23 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/inc/hi
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       26 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/inc/kok
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       41 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/inc/mr
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       37 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/inc/ne
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       39 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/inc/or
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       25 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/inc/pa
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       66 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/inc/sd
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       55 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/inc/si
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       94 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/inc/ur
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.687498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/ine/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       61 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/ine/hy
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      365 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/ine/hyw
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      103 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/ine/sq
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.687498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/ira/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       90 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/ira/fa
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      269 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/ira/fa-Latn
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       40 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/ira/ku
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.687498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/iro/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      569 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/iro/chr
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.687498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/itc/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      297 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/itc/la
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.687498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/jpx/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       52 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/jpx/ja
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       51 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/ko
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.687498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/map/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       42 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/map/haw
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.687498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/miz/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      183 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/miz/mto
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.687498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/myn/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      210 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/myn/quc
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.687498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/poz/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      134 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/poz/id
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      367 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/poz/mi
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      430 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/poz/ms
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       88 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/qu
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.691498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/roa/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       27 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/roa/an
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       25 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/roa/ca
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       63 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/roa/es
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      167 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/roa/es-419
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       79 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/roa/fr
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       84 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/roa/fr-BE
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       86 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/roa/fr-CH
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      140 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/roa/ht
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      109 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/roa/it
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       62 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/roa/pap
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       95 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/roa/pt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      109 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/roa/pt-BR
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       26 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/roa/ro
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.691498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/sai/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       47 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/sai/gn
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.691498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/sem/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       41 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/sem/am
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       50 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/sem/ar
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       40 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/sem/he
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       41 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/sem/mt
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.691498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/sit/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      686 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/sit/cmn
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      161 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/sit/cmn-Latn-pinyin
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      128 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/sit/hak
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       56 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/sit/my
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      194 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/sit/yue
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      213 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/sit/yue-Latn-jyutping
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.691498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/tai/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       92 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/tai/shn
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       37 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/tai/th
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.695498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/trk/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       45 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/trk/az
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       25 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/trk/ba
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       40 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/trk/cv
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       40 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/trk/kk
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       43 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/trk/ky
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       39 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/trk/nog
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       25 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/trk/tk
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       25 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/trk/tr
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       23 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/trk/tt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       24 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/trk/ug
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       39 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/trk/uz
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.695498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/urj/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      237 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/urj/et
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      237 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/urj/fi
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       73 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/urj/hu
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       45 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/urj/smj
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.695498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/zle/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       52 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/zle/be
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       57 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/zle/ru
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      280 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/zle/ru-LV
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       91 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/zle/ru-cl
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       97 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/zle/uk
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.695498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/zls/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      111 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/zls/bg
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      230 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/zls/bs
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      262 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/zls/hr
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       28 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/zls/mk
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       43 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/zls/sl
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      250 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/zls/sr
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.695498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/zlw/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       23 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/zlw/cs
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/zlw/pl
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       24 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lang/zlw/sk
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)   687931 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lb_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2793 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lfn_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    49890 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lt_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    66337 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/lv_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1346 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/mi_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    63859 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/mk_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    92345 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/ml_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    87391 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/mr_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    53541 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/ms_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4384 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/mt_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3960 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/mto_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    95948 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/my_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1534 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/nci_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    95377 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/ne_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    65979 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/nl_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4178 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/no_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3294 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/nog_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2302 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/om_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    89246 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/or_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    79953 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/pa_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2128 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/pap_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)   550424 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/phondata
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    21821 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/phondata-manifest
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    39074 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/phonindex
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    55796 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/phontab
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1710 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/piqd_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    76730 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/pl_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    67817 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/pt_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2409 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/py_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3028 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/qdb_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1919 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/qu_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1450 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/quc_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1939 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/qya_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    68538 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/ro_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)  8532392 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/ru_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    59928 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/sd_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    88172 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/shn_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    85384 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/si_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1783 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/sjn_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    50002 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/sk_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    45047 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/sl_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    35095 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/smj_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    45003 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/sq_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    46832 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/sr_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    47836 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/sv_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    47804 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/sw_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)   209553 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/ta_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    94837 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/te_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2301 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/th_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    20868 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/tk_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3072 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/tn_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    46793 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/tr_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2121 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/tt_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2070 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/ug_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3492 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/uk_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)   133556 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/ur_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2540 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/uz_dict
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    52608 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/vi_dict
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.643498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.707498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      128 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/Alex
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      474 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/Alicia
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      357 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/Andrea
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      320 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/Andy
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      315 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/Annie
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      361 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/AnxiousAndy
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3858 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/Demonic
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      305 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/Denis
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      379 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/Diogo
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      281 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/Gene
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      283 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/Gene2
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      381 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/Henrique
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      378 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/Hugo
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      267 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/Jacky
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      338 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/Lee
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      467 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/Marco
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      270 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/Mario
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      270 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/Michael
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      112 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/Mike
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3193 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/Mr serious
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      280 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/Nguyen
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      202 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/Reed
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      233 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/RicishayMax
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      435 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/RicishayMax2
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      435 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/RicishayMax3
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      420 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/Storm
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3189 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/Tweaky
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      417 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/UniRobot
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       75 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/adam
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      493 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/anika
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      512 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/anikaRobot
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      300 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/announcer
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      381 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/antonio
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      358 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/aunty
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      340 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/belinda
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      201 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/benjamin
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      224 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/boris
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       57 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/caleb
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       93 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/croak
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      112 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/david
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      287 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/ed
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      151 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/edward
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      152 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/edward2
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      324 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/f1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      357 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/f2
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      375 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/f3
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      350 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/f4
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      432 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/f5
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      149 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/fast
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      263 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/grandma
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      256 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/grandpa
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      253 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/gustave
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3168 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/ian
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      261 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/iven
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      279 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/iven2
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      262 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/iven3
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      261 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/iven4
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3186 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/john
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      361 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/kaukovalta
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/klatt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/klatt2
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       39 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/klatt3
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       39 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/klatt4
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       39 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/klatt5
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       39 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/klatt6
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      350 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/linda
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      335 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/m1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      264 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/m2
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      300 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/m3
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      290 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/m4
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      262 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/m5
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      188 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/m6
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      254 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/m7
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      284 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/m8
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      251 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/marcelo
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      225 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/max
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      404 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/michel
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      382 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/miguel
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      188 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/mike2
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3189 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/norbert
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3142 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/pablo
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      284 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/paul
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      352 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/pedro
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      354 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/quincy
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      265 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/rob
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      274 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/robert
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      451 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/robosoft
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      454 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/robosoft2
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      455 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/robosoft3
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      447 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/robosoft4
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      445 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/robosoft5
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      287 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/robosoft6
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      410 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/robosoft7
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      243 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/robosoft8
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      530 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/sandro
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      280 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/shelby
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      364 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/steph
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      367 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/steph2
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      377 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/steph3
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      383 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/travis
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      253 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/victor
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      186 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/whisper
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      392 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/whisperf
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      275 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/!v/zac
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.711498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       88 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-af1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       83 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-af1-en
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       84 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-ar1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       84 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-ar2
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      132 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-br1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      136 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-br2
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      132 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-br3
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      136 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-br4
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      105 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-ca1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      105 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-ca2
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       92 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-cn1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      111 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-cr1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       70 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-cz1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       82 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-cz2
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      144 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-de1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       96 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-de1-en
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      128 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-de2
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       80 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-de2-en
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       99 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-de3
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       96 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-de3-en
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      129 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-de4
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       81 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-de4-en
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      236 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-de5
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       90 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-de5-en
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      122 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-de6
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       74 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-de6-en
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       83 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-de6-grc
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      150 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-de7
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       71 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-de8
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       97 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-ee1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      131 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-en1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      114 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-es1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      108 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-es2
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      104 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-es3
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       88 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-es4
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      166 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-fr1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      104 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-fr1-en
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      103 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-fr2
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      100 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-fr3
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      127 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-fr4
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      107 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-fr4-en
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      100 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-fr5
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      100 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-fr6
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       83 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-fr7
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       94 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-gr1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       94 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-gr2
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       88 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-gr2-en
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       68 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-hb1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       83 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-hb2
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      102 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-hu1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       97 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-hu1-en
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       88 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-ic1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      101 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-id1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       69 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-in1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       85 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-in2
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      753 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-ir1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       84 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-it1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       87 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-it2
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      142 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-it3
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      145 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-it4
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       71 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-jp1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      101 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-jp2
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       87 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-jp3
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       83 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-la1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       87 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-lt1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       87 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-lt2
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       98 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-ma1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      120 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-mx1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      120 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-mx2
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       69 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-nl1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       96 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-nl2
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       91 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-nl2-en
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       85 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-nl3
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       68 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-nz1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       99 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-pl1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       82 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-pl1-en
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      131 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-pt1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       87 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-ro1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       81 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-ro1-en
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       98 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-sw1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       93 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-sw1-en
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      102 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-sw2
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       99 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-sw2-en
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       85 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-tl1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       85 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-tr1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      114 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-tr2
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      170 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-us1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      178 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-us2
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      180 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-us3
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      144 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/voices/mb/mb-vz1
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)   563571 2023-05-30 20:29:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/espeak-ng-data/yue_dict
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.711498 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/x86_64/
+-rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)  1723856 2023-05-30 20:24:21.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/lib/x86_64/libespeak-ng.so
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        0 2021-10-11 19:22:13.000000 espeak_phonemizer-1.3.1/espeak_phonemizer/py.typed
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.643498 espeak_phonemizer-1.3.1/espeak_phonemizer.egg-info/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2238 2023-06-21 20:57:06.000000 espeak_phonemizer-1.3.1/espeak_phonemizer.egg-info/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    23015 2023-06-21 20:57:06.000000 espeak_phonemizer-1.3.1/espeak_phonemizer.egg-info/SOURCES.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-06-21 20:57:06.000000 espeak_phonemizer-1.3.1/espeak_phonemizer.egg-info/dependency_links.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       70 2023-06-21 20:57:06.000000 espeak_phonemizer-1.3.1/espeak_phonemizer.egg-info/entry_points.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       24 2023-06-21 20:57:06.000000 espeak_phonemizer-1.3.1/espeak_phonemizer.egg-info/top_level.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       25 2023-06-21 20:54:06.000000 espeak_phonemizer-1.3.1/requirements_dev.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      113 2023-06-21 20:57:06.715498 espeak_phonemizer-1.3.1/setup.cfg
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1480 2023-06-21 20:51:52.000000 espeak_phonemizer-1.3.1/setup.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-21 20:57:06.715498 espeak_phonemizer-1.3.1/tests/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        0 2023-05-24 20:45:32.000000 espeak_phonemizer-1.3.1/tests/__init__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3085 2023-06-21 20:51:52.000000 espeak_phonemizer-1.3.1/tests/test_phonemizer.py
```

### Comparing `espeak_phonemizer-1.3.0/LICENSE` & `espeak_phonemizer-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer-1.3.0/PKG-INFO` & `espeak_phonemizer-1.3.1/espeak_phonemizer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
-Name: espeak_phonemizer
-Version: 1.3.0
+Name: espeak-phonemizer
+Version: 1.3.1
 Summary: Lightweight International Phonetic Alphabet (IPA) phonemizer that uses libespeak-ng
 Home-page: https://github.com/rhasspy/espeak-phonemizer
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -86,9 +84,7 @@
 ### Parallelize with GNU Parallel
 
 ```sh
 parallel -a /path/to/input.csv --pipepart \
     espeak-phonemizer -v en-us --csv \
     > /path/to/output.csv
 ```
-
-
```

### Comparing `espeak_phonemizer-1.3.0/README.md` & `espeak_phonemizer-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer-1.3.0/espeak_phonemizer/__init__.py` & `espeak_phonemizer-1.3.1/espeak_phonemizer/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -195,28 +195,27 @@
     ) -> List[str]:
         phoneme_flags = Phonemizer.espeakPHONEMES_IPA
         if phoneme_separator:
             phoneme_flags = phoneme_flags | (ord(phoneme_separator) << 8)
 
         text_bytes = text.encode("utf-8")
         text_pointer = ctypes.c_char_p(text_bytes)
-
         text_flags = Phonemizer.espeakCHARS_AUTO
-
         phoneme_lines = []
+        fcn_ttp = self.lib_espeak.espeak_TextToPhonemes
+        fcn_ttp.restype = ctypes.c_char_p
         while text_pointer:
-            clause_phonemes = ctypes.c_char_p(
-                self.lib_espeak.espeak_TextToPhonemes(
-                    ctypes.pointer(text_pointer), text_flags, phoneme_flags,
-                )
+            clause_phonemes = fcn_ttp(
+                ctypes.pointer(text_pointer), text_flags, phoneme_flags
             )
-            if clause_phonemes.value is not None:
-                phoneme_lines.append(
-                    clause_phonemes.value.decode()  # pylint: disable=no-member
-                )
+            if isinstance(clause_phonemes, bytes):
+                clause_phonemes_str = (
+                    clause_phonemes.decode()
+                )  # pylint: disable=no-member
+                phoneme_lines.append(clause_phonemes_str)
 
         return phoneme_lines
 
     def _maybe_init(self):
         if self.lib_espeak:
             # Already initialized
             return
```

### Comparing `espeak_phonemizer-1.3.0/espeak_phonemizer/__main__.py` & `espeak_phonemizer-1.3.1/espeak_phonemizer/__main__.py`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer-1.3.0/espeak_phonemizer.egg-info/PKG-INFO` & `espeak_phonemizer-1.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
-Name: espeak-phonemizer
-Version: 1.3.0
+Name: espeak_phonemizer
+Version: 1.3.1
 Summary: Lightweight International Phonetic Alphabet (IPA) phonemizer that uses libespeak-ng
 Home-page: https://github.com/rhasspy/espeak-phonemizer
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -86,9 +84,7 @@
 ### Parallelize with GNU Parallel
 
 ```sh
 parallel -a /path/to/input.csv --pipepart \
     espeak-phonemizer -v en-us --csv \
     > /path/to/output.csv
 ```
-
-
```

### Comparing `espeak_phonemizer-1.3.0/setup.py` & `espeak_phonemizer-1.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer-1.3.0/tests/test_phonemizer.py` & `espeak_phonemizer-1.3.1/tests/test_phonemizer.py`

 * *Files identical despite different names*

