# Comparing `tmp/tiled-0.1.0a95.tar.gz` & `tmp/tiled-0.1.0a96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiled-0.1.0a95.tar", last modified: Wed Jun 21 14:57:30 2023, max compression
+gzip compressed data, was "tiled-0.1.0a96.tar", last modified: Wed Jun 21 15:13:23 2023, max compression
```

## Comparing `tiled-0.1.0a95.tar` & `tiled-0.1.0a96.tar`

### file list

```diff
@@ -1,321 +1,321 @@
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 14:57:30.849061 tiled-0.1.0a95/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1538 2023-05-20 21:53:34.000000 tiled-0.1.0a95/LICENSE
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      783 2023-05-20 21:53:34.000000 tiled-0.1.0a95/MANIFEST.in
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7221 2023-06-21 14:57:30.849061 tiled-0.1.0a95/PKG-INFO
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     6555 2023-05-20 21:53:34.000000 tiled-0.1.0a95/README.md
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 14:57:30.829061 tiled-0.1.0a95/benchmarks/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-05-20 21:53:34.000000 tiled-0.1.0a95/benchmarks/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1065 2023-05-20 21:53:34.000000 tiled-0.1.0a95/benchmarks/benchmarks.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 14:57:30.829061 tiled-0.1.0a95/docs/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      673 2023-05-20 21:53:34.000000 tiled-0.1.0a95/docs/Makefile
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      797 2023-05-20 21:53:34.000000 tiled-0.1.0a95/docs/make.bat
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 14:57:30.829061 tiled-0.1.0a95/docs/source/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     9186 2023-05-20 21:53:34.000000 tiled-0.1.0a95/docs/source/conf.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 14:57:30.829061 tiled-0.1.0a95/docs/source/reference/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1083 2023-05-20 21:53:34.000000 tiled-0.1.0a95/docs/source/reference/min-versions.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      123 2023-05-20 21:53:34.000000 tiled-0.1.0a95/docs/source/reference/release-history.rst
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 14:57:30.829061 tiled-0.1.0a95/docs/source/tutorials/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2347 2023-05-20 21:53:34.000000 tiled-0.1.0a95/docs/source/tutorials/installation.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      280 2023-05-20 21:53:34.000000 tiled-0.1.0a95/pyproject.toml
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       90 2023-05-20 21:53:34.000000 tiled-0.1.0a95/requirements-array.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      175 2023-05-20 21:53:34.000000 tiled-0.1.0a95/requirements-client.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      159 2023-05-20 21:53:34.000000 tiled-0.1.0a95/requirements-compression.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      107 2023-05-20 21:53:34.000000 tiled-0.1.0a95/requirements-dataframe.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      478 2023-06-02 23:35:51.000000 tiled-0.1.0a95/requirements-dev.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      111 2023-05-20 21:53:34.000000 tiled-0.1.0a95/requirements-formats.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      423 2023-06-20 23:27:32.000000 tiled-0.1.0a95/requirements-server.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       23 2023-05-20 21:53:34.000000 tiled-0.1.0a95/requirements-sparse.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      107 2023-05-20 21:53:34.000000 tiled-0.1.0a95/requirements-xarray.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      174 2023-06-21 14:57:30.849061 tiled-0.1.0a95/setup.cfg
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4316 2023-05-20 21:53:34.000000 tiled-0.1.0a95/setup.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 14:57:30.825061 tiled-0.1.0a95/share/
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 14:57:30.829061 tiled-0.1.0a95/share/tiled/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      128 2023-05-20 21:53:34.000000 tiled-0.1.0a95/share/tiled/.identifying_file_72628d5f953b4229b58c9f1f8f6a9a09
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 14:57:30.829061 tiled-0.1.0a95/share/tiled/static/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    16958 2023-05-20 21:53:34.000000 tiled-0.1.0a95/share/tiled/static/favicon.ico
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 14:57:30.829061 tiled-0.1.0a95/share/tiled/templates/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      189 2023-05-20 21:53:34.000000 tiled-0.1.0a95/share/tiled/templates/device_code_failure.html
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      733 2023-05-20 21:53:34.000000 tiled-0.1.0a95/share/tiled/templates/device_code_form.html
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      276 2023-05-20 21:53:34.000000 tiled-0.1.0a95/share/tiled/templates/device_code_success.html
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2320 2023-05-20 21:53:34.000000 tiled-0.1.0a95/share/tiled/templates/index.html
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      491 2023-05-20 21:53:34.000000 tiled-0.1.0a95/share/tiled/templates/page.html
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 14:57:30.829061 tiled-0.1.0a95/share/tiled/ui/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7954 2023-06-21 14:55:14.000000 tiled-0.1.0a95/share/tiled/ui/asset-manifest.json
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 14:57:30.829061 tiled-0.1.0a95/share/tiled/ui/config/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1588 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/config/default.yml
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      203 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/configuration_manifest.yml
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    16958 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/favicon.ico
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      674 2023-06-21 14:55:14.000000 tiled-0.1.0a95/share/tiled/ui/index.html
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      292 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/manifest.json
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       67 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/robots.txt
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 14:57:30.829061 tiled-0.1.0a95/share/tiled/ui/static/
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 14:57:30.829061 tiled-0.1.0a95/share/tiled/ui/static/css/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     9577 2023-06-21 14:55:14.000000 tiled-0.1.0a95/share/tiled/ui/static/css/main.da25efef.css
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    12761 2023-06-21 14:55:14.000000 tiled-0.1.0a95/share/tiled/ui/static/css/main.da25efef.css.map
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 14:57:30.837061 tiled-0.1.0a95/share/tiled/ui/static/js/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     8354 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/113.a6dabf86.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    25023 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/113.a6dabf86.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      492 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/128.74bef542.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      869 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/128.74bef542.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    95776 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/197.6f7f332e.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)   490879 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/197.6f7f332e.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    10212 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/214.2a10743e.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    46572 2023-06-21 14:55:14.000000 tiled-0.1.0a95/share/tiled/ui/static/js/214.2a10743e.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    13141 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/276.0058e750.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       88 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/276.0058e750.chunk.js.LICENSE.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    37684 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/276.0058e750.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3633 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/321.c6b9dcec.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    14931 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/321.c6b9dcec.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3549 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/356.6a2946e1.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    10402 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/356.6a2946e1.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)   436519 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/393.73e08fb5.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      808 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/393.73e08fb5.chunk.js.LICENSE.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)   943354 2023-06-21 14:55:14.000000 tiled-0.1.0a95/share/tiled/ui/static/js/393.73e08fb5.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5877 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/446.ae1590fd.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    25688 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/446.ae1590fd.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)   407639 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/470.a78b4c62.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3921 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/470.a78b4c62.chunk.js.LICENSE.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)  1832576 2023-06-21 14:55:14.000000 tiled-0.1.0a95/share/tiled/ui/static/js/470.a78b4c62.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7736 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/485.0ed51a45.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    18509 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/485.0ed51a45.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    13996 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/494.3371b974.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    64957 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/494.3371b974.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    50521 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/689.0cde4405.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      245 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/689.0cde4405.chunk.js.LICENSE.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)   221121 2023-06-21 14:55:14.000000 tiled-0.1.0a95/share/tiled/ui/static/js/689.0cde4405.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      534 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/69.c379776e.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1255 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/69.c379776e.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    39133 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/705.eeca3f97.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       68 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/705.eeca3f97.chunk.js.LICENSE.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)   168665 2023-06-21 14:55:14.000000 tiled-0.1.0a95/share/tiled/ui/static/js/705.eeca3f97.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1175 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/741.fbe96b6d.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2715 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/741.fbe96b6d.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)  1032300 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/773.590aa2f4.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)  1877220 2023-06-21 14:55:14.000000 tiled-0.1.0a95/share/tiled/ui/static/js/773.590aa2f4.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4591 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/787.54a97274.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    10281 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/787.54a97274.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5344 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/837.22b95b21.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    14836 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/837.22b95b21.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    27323 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/858.2658cad8.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)   124490 2023-06-21 14:55:14.000000 tiled-0.1.0a95/share/tiled/ui/static/js/858.2658cad8.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4386 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/883.31ddd2ac.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    14318 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/883.31ddd2ac.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      527 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/921.22e363f6.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1293 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/921.22e363f6.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    22754 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/986.f5c9d7cf.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       88 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/986.f5c9d7cf.chunk.js.LICENSE.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    84726 2023-06-21 14:55:14.000000 tiled-0.1.0a95/share/tiled/ui/static/js/986.f5c9d7cf.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)   257278 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/main.5cc3eaa8.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1898 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/main.5cc3eaa8.js.LICENSE.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)   898204 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/js/main.5cc3eaa8.js.map
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 14:57:30.841061 tiled-0.1.0a95/share/tiled/ui/static/media/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    64952 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/media/roboto-all-300-normal.8fc5f5f22c9951113696.woff
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    65244 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/media/roboto-all-400-normal.376ea5d93f71583052f6.woff
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    65492 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/media/roboto-all-500-normal.52cb737b682eb9661ee1.woff
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    65292 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/media/roboto-all-700-normal.ef6d1d09b20b877fee4e.woff
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     9500 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/media/roboto-cyrillic-300-normal.48e4b37ecbc5e155460e.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     9688 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/media/roboto-cyrillic-400-normal.5e493812deabd1d01e60.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     9776 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/media/roboto-cyrillic-500-normal.d1615fb9cd7f67f5018c.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     9544 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/media/roboto-cyrillic-700-normal.0334efc0de1012200889.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    14988 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/media/roboto-cyrillic-ext-300-normal.12d37040a0160a948ff1.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    15344 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/media/roboto-cyrillic-ext-400-normal.493afe7ae8ecfe268800.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    15080 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/media/roboto-cyrillic-ext-500-normal.3e748c93fe6a87bdedaa.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    14720 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/media/roboto-cyrillic-ext-700-normal.b816cda3107bb21c87e1.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7120 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/media/roboto-greek-300-normal.7c6b44c55d4d9661e3ed.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7100 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/media/roboto-greek-400-normal.1cbfc636c911faa4d0ca.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7000 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/media/roboto-greek-500-normal.007ca18d2cbae7381b39.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     6888 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/media/roboto-greek-700-normal.3292e831b18d0c23d609.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1476 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/media/roboto-greek-ext-300-normal.04e05839d6a35e046c13.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1492 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/media/roboto-greek-ext-400-normal.bb723e8458c9c653e505.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1508 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/media/roboto-greek-ext-500-normal.9c0d384f31e2c914edf3.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1436 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/media/roboto-greek-ext-700-normal.9674bc0ae12c2551d9d1.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    15732 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/media/roboto-latin-300-normal.0109a2ace896a506a0aa.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    15688 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/media/roboto-latin-400-normal.4673b4537a84c7f7a130.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    15920 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/media/roboto-latin-500-normal.869888415d0b1a99ae5c.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    15828 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/media/roboto-latin-700-normal.0682ca7f74351d42bf73.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    11812 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/media/roboto-latin-ext-300-normal.a29236e0fc30e8482530.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    11860 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/media/roboto-latin-ext-400-normal.c3dcdbd5bb4d4af80817.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    11768 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/media/roboto-latin-ext-500-normal.feaff916fd609e310efe.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    11836 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/media/roboto-latin-ext-700-normal.bcf37d666ce10b3556cd.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5460 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/media/roboto-vietnamese-300-normal.af9afdc10c93e4118e90.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5540 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/media/roboto-vietnamese-400-normal.c0bec65d01f776c00c91.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5580 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/media/roboto-vietnamese-500-normal.b8e494da1ec1f1824769.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5524 2023-06-21 14:55:13.000000 tiled-0.1.0a95/share/tiled/ui/static/media/roboto-vietnamese-700-normal.3096f18acebc3f07020d.woff2
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 14:57:30.849061 tiled-0.1.0a95/tiled/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       73 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       43 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/__main__.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 14:57:30.841061 tiled-0.1.0a95/tiled/_tests/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2826 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/_tests/conftest.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7775 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/_tests/test_access_control.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1072 2023-06-08 18:09:49.000000 tiled-0.1.0a95/tiled/_tests/test_allow_origins.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5569 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_array.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    16121 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_authentication.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1453 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_authenticators.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2224 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_caches.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    10951 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/_tests/test_catalog.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     6306 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/_tests/test_client.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    13661 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_client_cache.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3285 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_config.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 14:57:30.841061 tiled-0.1.0a95/tiled/_tests/test_configs/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      166 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_configs/config_missing_api_key.yml
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      332 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_configs/config_missing_secret_keys.yml
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      448 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_configs/config_missing_secret_keys_public.yml
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      195 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_configs/config_public_no_authenticator.yml
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      196 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_configs/config_with_api_key.yml
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      434 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_configs/config_with_secret_keys.yml
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1475 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_custom_format.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2297 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_dataframe.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    11651 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_directory_walker.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4037 2023-06-02 23:35:51.000000 tiled-0.1.0a95/tiled/_tests/test_distinct.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4628 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_export.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4090 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_hdf5.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      555 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_history.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1189 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_import_object.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2782 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_indexers.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3958 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_inlined_contents.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      780 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_json.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1565 2023-06-08 18:41:15.000000 tiled-0.1.0a95/tiled/_tests/test_metrics.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      411 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_no_heavy_imports.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5087 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_object_cache.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1385 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_openapi.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1369 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_pickle.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     8564 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/_tests/test_queries.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      362 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_routes.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1125 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_scaled_config_option.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1999 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_search.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      290 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_sentinel.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2408 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_size_limit.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3364 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_sort.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2320 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_sparse.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2357 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_specs_and_references.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1211 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_structured_array.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4237 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_tiff.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      342 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_tokenize.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4241 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/_tests/test_validation.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    13151 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/_tests/test_writing.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4967 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/_tests/test_xarray.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2160 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/_tests/utils.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      500 2023-06-21 14:57:30.849061 tiled-0.1.0a95/tiled/_version.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3198 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/access_policies.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 14:57:30.845061 tiled-0.1.0a95/tiled/adapters/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/adapters/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4176 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/adapters/array.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5386 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/adapters/dataframe.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1942 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/adapters/excel.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    30376 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/adapters/files.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4635 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/adapters/hdf5.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    14630 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/adapters/mapping.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2115 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/adapters/parquet.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3639 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/adapters/sparse.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3316 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/adapters/sparse_blocks_parquet.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7659 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/adapters/tiff.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1195 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/adapters/utils.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1890 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/adapters/xarray.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2376 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/adapters/zarr.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    32406 2023-06-02 23:35:51.000000 tiled-0.1.0a95/tiled/authenticators.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 14:57:30.845061 tiled-0.1.0a95/tiled/catalog/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       55 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/catalog/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    29042 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/catalog/adapter.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      157 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/catalog/base.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2230 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/catalog/explain.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     6511 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/catalog/orm.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 14:57:30.845061 tiled-0.1.0a95/tiled/client/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      244 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/client/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    29314 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/client/_testclient.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     8896 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/client/array.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     6561 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/client/auth.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    10209 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/client/base.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    27705 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/client/cache.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    10173 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/client/constructors.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    37527 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/client/context.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     9129 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/client/dataframe.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    35731 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/client/node.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4934 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/client/sparse.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    13106 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/client/utils.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     8070 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/client/xarray.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 14:57:30.845061 tiled-0.1.0a95/tiled/commandline/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/commandline/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4919 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/commandline/_admin.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3230 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/commandline/_api_key.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1247 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/commandline/_catalog.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1411 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/commandline/_profile.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    13088 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/commandline/_serve.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2487 2023-05-25 18:31:19.000000 tiled-0.1.0a95/tiled/commandline/_utils.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     8073 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/commandline/main.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    16568 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/config.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 14:57:30.845061 tiled-0.1.0a95/tiled/config_schemas/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5275 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/config_schemas/client_profiles.yml
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    16272 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/config_schemas/service_configuration.yml
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 14:57:30.845061 tiled-0.1.0a95/tiled/database/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/database/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2658 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/database/alembic.ini.template
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2690 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/database/alembic_utils.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      157 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/database/base.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1704 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/database/connection_pool.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    11164 2023-06-02 23:35:51.000000 tiled-0.1.0a95/tiled/database/core.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 14:57:30.845061 tiled-0.1.0a95/tiled/database/migrations/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2261 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/database/migrations/env.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      494 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/database/migrations/script.py.mako
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 14:57:30.845061 tiled-0.1.0a95/tiled/database/migrations/versions/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4023 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/database/migrations/versions/481830dd6c11_initialize.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      889 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/database/migrations/versions/4a9dfaba4a98_add_pendingsession.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1270 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/database/migrations/versions/56809bcbfcb0_add_create_scope_to_default_roles.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1292 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/database/migrations/versions/722ff4e4fcc7_add_write_scopes_to_default_roles.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7253 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/database/orm.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 14:57:30.845061 tiled-0.1.0a95/tiled/examples/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/examples/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1234 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/examples/generate_files.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4902 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/examples/generated.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      941 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/examples/generated_minimal.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      963 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/examples/nexus.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      454 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/examples/numpy_structured_dtypes.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      582 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/examples/toy_authentication.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4762 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/examples/xdi.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     6544 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/iterviews.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    10560 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/media_type_registration.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     8917 2023-05-25 18:31:19.000000 tiled-0.1.0a95/tiled/profiles.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    11716 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/queries.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4616 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/query_registration.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      690 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/scopes.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 14:57:30.845061 tiled-0.1.0a95/tiled/serialization/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      960 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/serialization/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5187 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/serialization/array.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3880 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/serialization/dataframe.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    12933 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/serialization/image_serializer_helpers.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3558 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/serialization/node.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3179 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/serialization/sparse.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5155 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/serialization/xarray.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 14:57:30.845061 tiled-0.1.0a95/tiled/server/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/server/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    34605 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/server/app.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    37847 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/server/authentication.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     6204 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/server/compression.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    29335 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/server/core.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     6010 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/server/dependencies.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1082 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/server/etag.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5637 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/server/metrics.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5845 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/server/object_cache.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     8486 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/server/pydantic_array.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2739 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/server/pydantic_dataframe.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      570 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/server/pydantic_sparse.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    34955 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/server/router.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    16920 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/server/schemas.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3071 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/server/settings.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4248 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/server/utils.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 14:57:30.849061 tiled-0.1.0a95/tiled/structures/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/structures/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7821 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/structures/array.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1060 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/structures/core.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2529 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/structures/dataframe.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1035 2023-06-09 00:02:28.000000 tiled-0.1.0a95/tiled/structures/sparse.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    18126 2023-06-20 23:27:32.000000 tiled-0.1.0a95/tiled/utils.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      645 2023-05-20 21:53:34.000000 tiled-0.1.0a95/tiled/validation_registration.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 14:57:30.841061 tiled-0.1.0a95/tiled.egg-info/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7221 2023-06-21 14:57:30.000000 tiled-0.1.0a95/tiled.egg-info/PKG-INFO
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    11367 2023-06-21 14:57:30.000000 tiled-0.1.0a95/tiled.egg-info/SOURCES.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        1 2023-06-21 14:57:30.000000 tiled-0.1.0a95/tiled.egg-info/dependency_links.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       54 2023-06-21 14:57:30.000000 tiled-0.1.0a95/tiled.egg-info/entry_points.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2217 2023-06-21 14:57:30.000000 tiled-0.1.0a95/tiled.egg-info/requires.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       17 2023-06-21 14:57:30.000000 tiled-0.1.0a95/tiled.egg-info/top_level.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    80049 2023-05-20 21:53:34.000000 tiled-0.1.0a95/versioneer.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 15:13:23.189435 tiled-0.1.0a96/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1538 2023-05-20 21:53:34.000000 tiled-0.1.0a96/LICENSE
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      783 2023-05-20 21:53:34.000000 tiled-0.1.0a96/MANIFEST.in
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7221 2023-06-21 15:13:23.189435 tiled-0.1.0a96/PKG-INFO
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     6555 2023-05-20 21:53:34.000000 tiled-0.1.0a96/README.md
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 15:13:23.173435 tiled-0.1.0a96/benchmarks/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-05-20 21:53:34.000000 tiled-0.1.0a96/benchmarks/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1065 2023-05-20 21:53:34.000000 tiled-0.1.0a96/benchmarks/benchmarks.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 15:13:23.173435 tiled-0.1.0a96/docs/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      673 2023-05-20 21:53:34.000000 tiled-0.1.0a96/docs/Makefile
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      797 2023-05-20 21:53:34.000000 tiled-0.1.0a96/docs/make.bat
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 15:13:23.173435 tiled-0.1.0a96/docs/source/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     9186 2023-05-20 21:53:34.000000 tiled-0.1.0a96/docs/source/conf.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 15:13:23.173435 tiled-0.1.0a96/docs/source/reference/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1083 2023-05-20 21:53:34.000000 tiled-0.1.0a96/docs/source/reference/min-versions.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      123 2023-05-20 21:53:34.000000 tiled-0.1.0a96/docs/source/reference/release-history.rst
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 15:13:23.173435 tiled-0.1.0a96/docs/source/tutorials/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2347 2023-05-20 21:53:34.000000 tiled-0.1.0a96/docs/source/tutorials/installation.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      280 2023-05-20 21:53:34.000000 tiled-0.1.0a96/pyproject.toml
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       90 2023-05-20 21:53:34.000000 tiled-0.1.0a96/requirements-array.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      175 2023-05-20 21:53:34.000000 tiled-0.1.0a96/requirements-client.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      159 2023-05-20 21:53:34.000000 tiled-0.1.0a96/requirements-compression.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      107 2023-05-20 21:53:34.000000 tiled-0.1.0a96/requirements-dataframe.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      478 2023-06-02 23:35:51.000000 tiled-0.1.0a96/requirements-dev.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      111 2023-05-20 21:53:34.000000 tiled-0.1.0a96/requirements-formats.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      423 2023-06-20 23:27:32.000000 tiled-0.1.0a96/requirements-server.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       23 2023-05-20 21:53:34.000000 tiled-0.1.0a96/requirements-sparse.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      107 2023-05-20 21:53:34.000000 tiled-0.1.0a96/requirements-xarray.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      174 2023-06-21 15:13:23.189435 tiled-0.1.0a96/setup.cfg
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4316 2023-05-20 21:53:34.000000 tiled-0.1.0a96/setup.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 15:13:23.169435 tiled-0.1.0a96/share/
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 15:13:23.173435 tiled-0.1.0a96/share/tiled/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      128 2023-05-20 21:53:34.000000 tiled-0.1.0a96/share/tiled/.identifying_file_72628d5f953b4229b58c9f1f8f6a9a09
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 15:13:23.173435 tiled-0.1.0a96/share/tiled/static/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    16958 2023-05-20 21:53:34.000000 tiled-0.1.0a96/share/tiled/static/favicon.ico
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 15:13:23.173435 tiled-0.1.0a96/share/tiled/templates/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      189 2023-05-20 21:53:34.000000 tiled-0.1.0a96/share/tiled/templates/device_code_failure.html
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      733 2023-05-20 21:53:34.000000 tiled-0.1.0a96/share/tiled/templates/device_code_form.html
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      276 2023-05-20 21:53:34.000000 tiled-0.1.0a96/share/tiled/templates/device_code_success.html
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2320 2023-05-20 21:53:34.000000 tiled-0.1.0a96/share/tiled/templates/index.html
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      491 2023-05-20 21:53:34.000000 tiled-0.1.0a96/share/tiled/templates/page.html
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 15:13:23.173435 tiled-0.1.0a96/share/tiled/ui/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7954 2023-06-21 14:55:14.000000 tiled-0.1.0a96/share/tiled/ui/asset-manifest.json
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 15:13:23.173435 tiled-0.1.0a96/share/tiled/ui/config/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1588 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/config/default.yml
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      203 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/configuration_manifest.yml
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    16958 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/favicon.ico
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      674 2023-06-21 14:55:14.000000 tiled-0.1.0a96/share/tiled/ui/index.html
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      292 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/manifest.json
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       67 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/robots.txt
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 15:13:23.169435 tiled-0.1.0a96/share/tiled/ui/static/
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 15:13:23.173435 tiled-0.1.0a96/share/tiled/ui/static/css/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     9577 2023-06-21 14:55:14.000000 tiled-0.1.0a96/share/tiled/ui/static/css/main.da25efef.css
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    12761 2023-06-21 14:55:14.000000 tiled-0.1.0a96/share/tiled/ui/static/css/main.da25efef.css.map
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 15:13:23.181435 tiled-0.1.0a96/share/tiled/ui/static/js/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     8354 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/113.a6dabf86.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    25023 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/113.a6dabf86.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      492 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/128.74bef542.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      869 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/128.74bef542.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    95776 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/197.6f7f332e.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)   490879 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/197.6f7f332e.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    10212 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/214.2a10743e.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    46572 2023-06-21 14:55:14.000000 tiled-0.1.0a96/share/tiled/ui/static/js/214.2a10743e.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    13141 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/276.0058e750.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       88 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/276.0058e750.chunk.js.LICENSE.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    37684 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/276.0058e750.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3633 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/321.c6b9dcec.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    14931 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/321.c6b9dcec.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3549 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/356.6a2946e1.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    10402 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/356.6a2946e1.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)   436519 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/393.73e08fb5.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      808 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/393.73e08fb5.chunk.js.LICENSE.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)   943354 2023-06-21 14:55:14.000000 tiled-0.1.0a96/share/tiled/ui/static/js/393.73e08fb5.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5877 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/446.ae1590fd.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    25688 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/446.ae1590fd.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)   407639 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/470.a78b4c62.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3921 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/470.a78b4c62.chunk.js.LICENSE.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)  1832576 2023-06-21 14:55:14.000000 tiled-0.1.0a96/share/tiled/ui/static/js/470.a78b4c62.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7736 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/485.0ed51a45.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    18509 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/485.0ed51a45.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    13996 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/494.3371b974.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    64957 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/494.3371b974.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    50521 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/689.0cde4405.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      245 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/689.0cde4405.chunk.js.LICENSE.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)   221121 2023-06-21 14:55:14.000000 tiled-0.1.0a96/share/tiled/ui/static/js/689.0cde4405.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      534 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/69.c379776e.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1255 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/69.c379776e.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    39133 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/705.eeca3f97.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       68 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/705.eeca3f97.chunk.js.LICENSE.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)   168665 2023-06-21 14:55:14.000000 tiled-0.1.0a96/share/tiled/ui/static/js/705.eeca3f97.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1175 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/741.fbe96b6d.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2715 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/741.fbe96b6d.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)  1032300 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/773.590aa2f4.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)  1877220 2023-06-21 14:55:14.000000 tiled-0.1.0a96/share/tiled/ui/static/js/773.590aa2f4.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4591 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/787.54a97274.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    10281 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/787.54a97274.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5344 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/837.22b95b21.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    14836 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/837.22b95b21.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    27323 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/858.2658cad8.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)   124490 2023-06-21 14:55:14.000000 tiled-0.1.0a96/share/tiled/ui/static/js/858.2658cad8.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4386 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/883.31ddd2ac.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    14318 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/883.31ddd2ac.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      527 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/921.22e363f6.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1293 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/921.22e363f6.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    22754 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/986.f5c9d7cf.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       88 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/986.f5c9d7cf.chunk.js.LICENSE.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    84726 2023-06-21 14:55:14.000000 tiled-0.1.0a96/share/tiled/ui/static/js/986.f5c9d7cf.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)   257278 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/main.5cc3eaa8.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1898 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/main.5cc3eaa8.js.LICENSE.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)   898204 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/js/main.5cc3eaa8.js.map
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 15:13:23.181435 tiled-0.1.0a96/share/tiled/ui/static/media/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    64952 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/media/roboto-all-300-normal.8fc5f5f22c9951113696.woff
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    65244 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/media/roboto-all-400-normal.376ea5d93f71583052f6.woff
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    65492 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/media/roboto-all-500-normal.52cb737b682eb9661ee1.woff
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    65292 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/media/roboto-all-700-normal.ef6d1d09b20b877fee4e.woff
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     9500 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/media/roboto-cyrillic-300-normal.48e4b37ecbc5e155460e.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     9688 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/media/roboto-cyrillic-400-normal.5e493812deabd1d01e60.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     9776 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/media/roboto-cyrillic-500-normal.d1615fb9cd7f67f5018c.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     9544 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/media/roboto-cyrillic-700-normal.0334efc0de1012200889.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    14988 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/media/roboto-cyrillic-ext-300-normal.12d37040a0160a948ff1.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    15344 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/media/roboto-cyrillic-ext-400-normal.493afe7ae8ecfe268800.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    15080 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/media/roboto-cyrillic-ext-500-normal.3e748c93fe6a87bdedaa.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    14720 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/media/roboto-cyrillic-ext-700-normal.b816cda3107bb21c87e1.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7120 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/media/roboto-greek-300-normal.7c6b44c55d4d9661e3ed.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7100 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/media/roboto-greek-400-normal.1cbfc636c911faa4d0ca.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7000 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/media/roboto-greek-500-normal.007ca18d2cbae7381b39.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     6888 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/media/roboto-greek-700-normal.3292e831b18d0c23d609.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1476 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/media/roboto-greek-ext-300-normal.04e05839d6a35e046c13.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1492 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/media/roboto-greek-ext-400-normal.bb723e8458c9c653e505.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1508 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/media/roboto-greek-ext-500-normal.9c0d384f31e2c914edf3.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1436 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/media/roboto-greek-ext-700-normal.9674bc0ae12c2551d9d1.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    15732 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/media/roboto-latin-300-normal.0109a2ace896a506a0aa.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    15688 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/media/roboto-latin-400-normal.4673b4537a84c7f7a130.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    15920 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/media/roboto-latin-500-normal.869888415d0b1a99ae5c.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    15828 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/media/roboto-latin-700-normal.0682ca7f74351d42bf73.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    11812 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/media/roboto-latin-ext-300-normal.a29236e0fc30e8482530.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    11860 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/media/roboto-latin-ext-400-normal.c3dcdbd5bb4d4af80817.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    11768 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/media/roboto-latin-ext-500-normal.feaff916fd609e310efe.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    11836 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/media/roboto-latin-ext-700-normal.bcf37d666ce10b3556cd.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5460 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/media/roboto-vietnamese-300-normal.af9afdc10c93e4118e90.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5540 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/media/roboto-vietnamese-400-normal.c0bec65d01f776c00c91.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5580 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/media/roboto-vietnamese-500-normal.b8e494da1ec1f1824769.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5524 2023-06-21 14:55:13.000000 tiled-0.1.0a96/share/tiled/ui/static/media/roboto-vietnamese-700-normal.3096f18acebc3f07020d.woff2
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 15:13:23.189435 tiled-0.1.0a96/tiled/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       73 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       43 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/__main__.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 15:13:23.185435 tiled-0.1.0a96/tiled/_tests/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2826 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/_tests/conftest.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7775 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/_tests/test_access_control.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1072 2023-06-08 18:09:49.000000 tiled-0.1.0a96/tiled/_tests/test_allow_origins.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5569 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_array.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    16121 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_authentication.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1453 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_authenticators.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2224 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_caches.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    10951 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/_tests/test_catalog.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     6306 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/_tests/test_client.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    13661 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_client_cache.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3285 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_config.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 15:13:23.185435 tiled-0.1.0a96/tiled/_tests/test_configs/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      166 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_configs/config_missing_api_key.yml
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      332 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_configs/config_missing_secret_keys.yml
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      448 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_configs/config_missing_secret_keys_public.yml
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      195 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_configs/config_public_no_authenticator.yml
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      196 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_configs/config_with_api_key.yml
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      434 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_configs/config_with_secret_keys.yml
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1475 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_custom_format.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2297 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_dataframe.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    11651 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_directory_walker.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4037 2023-06-02 23:35:51.000000 tiled-0.1.0a96/tiled/_tests/test_distinct.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4628 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_export.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4090 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_hdf5.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      555 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_history.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1189 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_import_object.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2782 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_indexers.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3958 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_inlined_contents.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      780 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_json.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1565 2023-06-08 18:41:15.000000 tiled-0.1.0a96/tiled/_tests/test_metrics.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      411 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_no_heavy_imports.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5087 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_object_cache.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1385 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_openapi.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1369 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_pickle.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     8564 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/_tests/test_queries.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      362 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_routes.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1125 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_scaled_config_option.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1999 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_search.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      290 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_sentinel.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2408 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_size_limit.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3364 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_sort.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2320 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_sparse.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2357 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_specs_and_references.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1211 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_structured_array.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4237 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_tiff.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      342 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_tokenize.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4241 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/_tests/test_validation.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    13151 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/_tests/test_writing.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4967 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/_tests/test_xarray.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2160 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/_tests/utils.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      500 2023-06-21 15:13:23.189435 tiled-0.1.0a96/tiled/_version.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3198 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/access_policies.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 15:13:23.185435 tiled-0.1.0a96/tiled/adapters/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/adapters/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4176 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/adapters/array.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5386 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/adapters/dataframe.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1942 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/adapters/excel.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    30376 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/adapters/files.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4635 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/adapters/hdf5.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    14630 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/adapters/mapping.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2115 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/adapters/parquet.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3639 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/adapters/sparse.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3316 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/adapters/sparse_blocks_parquet.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7659 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/adapters/tiff.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1195 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/adapters/utils.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1890 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/adapters/xarray.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2376 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/adapters/zarr.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    32406 2023-06-02 23:35:51.000000 tiled-0.1.0a96/tiled/authenticators.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 15:13:23.185435 tiled-0.1.0a96/tiled/catalog/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       55 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/catalog/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    29042 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/catalog/adapter.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      157 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/catalog/base.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2230 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/catalog/explain.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     6511 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/catalog/orm.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 15:13:23.185435 tiled-0.1.0a96/tiled/client/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      244 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/client/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    29314 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/client/_testclient.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     8896 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/client/array.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     6561 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/client/auth.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    10209 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/client/base.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    27705 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/client/cache.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    10173 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/client/constructors.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    37527 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/client/context.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     9129 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/client/dataframe.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    35731 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/client/node.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4934 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/client/sparse.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    13106 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/client/utils.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     8070 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/client/xarray.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 15:13:23.185435 tiled-0.1.0a96/tiled/commandline/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/commandline/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4919 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/commandline/_admin.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3230 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/commandline/_api_key.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1247 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/commandline/_catalog.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1411 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/commandline/_profile.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    13088 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/commandline/_serve.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2487 2023-05-25 18:31:19.000000 tiled-0.1.0a96/tiled/commandline/_utils.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     8073 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/commandline/main.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    16568 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/config.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 15:13:23.185435 tiled-0.1.0a96/tiled/config_schemas/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5275 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/config_schemas/client_profiles.yml
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    16272 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/config_schemas/service_configuration.yml
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 15:13:23.185435 tiled-0.1.0a96/tiled/database/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/database/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2658 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/database/alembic.ini.template
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2690 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/database/alembic_utils.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      157 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/database/base.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1704 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/database/connection_pool.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    11164 2023-06-02 23:35:51.000000 tiled-0.1.0a96/tiled/database/core.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 15:13:23.185435 tiled-0.1.0a96/tiled/database/migrations/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2261 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/database/migrations/env.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      494 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/database/migrations/script.py.mako
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 15:13:23.185435 tiled-0.1.0a96/tiled/database/migrations/versions/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4023 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/database/migrations/versions/481830dd6c11_initialize.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      889 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/database/migrations/versions/4a9dfaba4a98_add_pendingsession.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1270 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/database/migrations/versions/56809bcbfcb0_add_create_scope_to_default_roles.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1292 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/database/migrations/versions/722ff4e4fcc7_add_write_scopes_to_default_roles.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7253 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/database/orm.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 15:13:23.185435 tiled-0.1.0a96/tiled/examples/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/examples/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1234 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/examples/generate_files.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4902 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/examples/generated.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      941 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/examples/generated_minimal.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      963 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/examples/nexus.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      454 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/examples/numpy_structured_dtypes.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      582 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/examples/toy_authentication.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4762 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/examples/xdi.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     6544 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/iterviews.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    10560 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/media_type_registration.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     8917 2023-05-25 18:31:19.000000 tiled-0.1.0a96/tiled/profiles.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    11716 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/queries.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4616 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/query_registration.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      690 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/scopes.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 15:13:23.189435 tiled-0.1.0a96/tiled/serialization/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      960 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/serialization/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5187 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/serialization/array.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3880 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/serialization/dataframe.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    12933 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/serialization/image_serializer_helpers.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3558 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/serialization/node.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3179 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/serialization/sparse.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5155 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/serialization/xarray.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 15:13:23.189435 tiled-0.1.0a96/tiled/server/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/server/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    34605 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/server/app.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    37847 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/server/authentication.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     6204 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/server/compression.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    29335 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/server/core.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     6010 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/server/dependencies.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1082 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/server/etag.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5637 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/server/metrics.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5845 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/server/object_cache.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     8486 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/server/pydantic_array.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2739 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/server/pydantic_dataframe.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      570 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/server/pydantic_sparse.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    34955 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/server/router.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    16920 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/server/schemas.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3071 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/server/settings.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4248 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/server/utils.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 15:13:23.189435 tiled-0.1.0a96/tiled/structures/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/structures/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7821 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/structures/array.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1060 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/structures/core.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2529 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/structures/dataframe.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1035 2023-06-09 00:02:28.000000 tiled-0.1.0a96/tiled/structures/sparse.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    18126 2023-06-20 23:27:32.000000 tiled-0.1.0a96/tiled/utils.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      645 2023-05-20 21:53:34.000000 tiled-0.1.0a96/tiled/validation_registration.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-21 15:13:23.181435 tiled-0.1.0a96/tiled.egg-info/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7221 2023-06-21 15:13:23.000000 tiled-0.1.0a96/tiled.egg-info/PKG-INFO
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    11367 2023-06-21 15:13:23.000000 tiled-0.1.0a96/tiled.egg-info/SOURCES.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)        1 2023-06-21 15:13:23.000000 tiled-0.1.0a96/tiled.egg-info/dependency_links.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       54 2023-06-21 15:13:23.000000 tiled-0.1.0a96/tiled.egg-info/entry_points.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2217 2023-06-21 15:13:23.000000 tiled-0.1.0a96/tiled.egg-info/requires.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       17 2023-06-21 15:13:23.000000 tiled-0.1.0a96/tiled.egg-info/top_level.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    80049 2023-05-20 21:53:34.000000 tiled-0.1.0a96/versioneer.py
```

### Comparing `tiled-0.1.0a95/LICENSE` & `tiled-0.1.0a96/LICENSE`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/MANIFEST.in` & `tiled-0.1.0a96/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/PKG-INFO` & `tiled-0.1.0a96/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiled
-Version: 0.1.0a95
+Version: 0.1.0a96
 Summary: Tile-based access to SciPy/PyData data structures over the web in many formats
 Home-page: https://github.com/bluesky/tiled
 Author: Bluesky Collaboration
 Author-email: dallan@bnl.gov
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `tiled-0.1.0a95/README.md` & `tiled-0.1.0a96/README.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/benchmarks/benchmarks.py` & `tiled-0.1.0a96/benchmarks/benchmarks.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/docs/Makefile` & `tiled-0.1.0a96/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/docs/make.bat` & `tiled-0.1.0a96/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/docs/source/conf.py` & `tiled-0.1.0a96/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/docs/source/reference/min-versions.rst` & `tiled-0.1.0a96/docs/source/reference/min-versions.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/docs/source/tutorials/installation.rst` & `tiled-0.1.0a96/docs/source/tutorials/installation.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/setup.py` & `tiled-0.1.0a96/setup.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/static/favicon.ico` & `tiled-0.1.0a96/share/tiled/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/templates/device_code_form.html` & `tiled-0.1.0a96/share/tiled/templates/device_code_form.html`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/templates/index.html` & `tiled-0.1.0a96/share/tiled/templates/index.html`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/asset-manifest.json` & `tiled-0.1.0a96/share/tiled/ui/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/config/default.yml` & `tiled-0.1.0a96/share/tiled/ui/config/default.yml`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/favicon.ico` & `tiled-0.1.0a96/share/tiled/ui/favicon.ico`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/index.html` & `tiled-0.1.0a96/share/tiled/ui/index.html`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/css/main.da25efef.css` & `tiled-0.1.0a96/share/tiled/ui/static/css/main.da25efef.css`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/css/main.da25efef.css.map` & `tiled-0.1.0a96/share/tiled/ui/static/css/main.da25efef.css.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/113.a6dabf86.chunk.js` & `tiled-0.1.0a96/share/tiled/ui/static/js/113.a6dabf86.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/113.a6dabf86.chunk.js.map` & `tiled-0.1.0a96/share/tiled/ui/static/js/113.a6dabf86.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/128.74bef542.chunk.js.map` & `tiled-0.1.0a96/share/tiled/ui/static/js/128.74bef542.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/197.6f7f332e.chunk.js` & `tiled-0.1.0a96/share/tiled/ui/static/js/197.6f7f332e.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/197.6f7f332e.chunk.js.map` & `tiled-0.1.0a96/share/tiled/ui/static/js/197.6f7f332e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/214.2a10743e.chunk.js` & `tiled-0.1.0a96/share/tiled/ui/static/js/214.2a10743e.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/214.2a10743e.chunk.js.map` & `tiled-0.1.0a96/share/tiled/ui/static/js/214.2a10743e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/276.0058e750.chunk.js` & `tiled-0.1.0a96/share/tiled/ui/static/js/276.0058e750.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/276.0058e750.chunk.js.map` & `tiled-0.1.0a96/share/tiled/ui/static/js/276.0058e750.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/321.c6b9dcec.chunk.js` & `tiled-0.1.0a96/share/tiled/ui/static/js/321.c6b9dcec.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/321.c6b9dcec.chunk.js.map` & `tiled-0.1.0a96/share/tiled/ui/static/js/321.c6b9dcec.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/356.6a2946e1.chunk.js` & `tiled-0.1.0a96/share/tiled/ui/static/js/356.6a2946e1.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/356.6a2946e1.chunk.js.map` & `tiled-0.1.0a96/share/tiled/ui/static/js/356.6a2946e1.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/393.73e08fb5.chunk.js` & `tiled-0.1.0a96/share/tiled/ui/static/js/393.73e08fb5.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/393.73e08fb5.chunk.js.LICENSE.txt` & `tiled-0.1.0a96/share/tiled/ui/static/js/393.73e08fb5.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/393.73e08fb5.chunk.js.map` & `tiled-0.1.0a96/share/tiled/ui/static/js/393.73e08fb5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/446.ae1590fd.chunk.js` & `tiled-0.1.0a96/share/tiled/ui/static/js/446.ae1590fd.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/446.ae1590fd.chunk.js.map` & `tiled-0.1.0a96/share/tiled/ui/static/js/446.ae1590fd.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/470.a78b4c62.chunk.js` & `tiled-0.1.0a96/share/tiled/ui/static/js/470.a78b4c62.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/470.a78b4c62.chunk.js.LICENSE.txt` & `tiled-0.1.0a96/share/tiled/ui/static/js/470.a78b4c62.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/470.a78b4c62.chunk.js.map` & `tiled-0.1.0a96/share/tiled/ui/static/js/470.a78b4c62.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/485.0ed51a45.chunk.js` & `tiled-0.1.0a96/share/tiled/ui/static/js/485.0ed51a45.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/485.0ed51a45.chunk.js.map` & `tiled-0.1.0a96/share/tiled/ui/static/js/485.0ed51a45.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/494.3371b974.chunk.js` & `tiled-0.1.0a96/share/tiled/ui/static/js/494.3371b974.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/494.3371b974.chunk.js.map` & `tiled-0.1.0a96/share/tiled/ui/static/js/494.3371b974.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/689.0cde4405.chunk.js` & `tiled-0.1.0a96/share/tiled/ui/static/js/689.0cde4405.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/689.0cde4405.chunk.js.map` & `tiled-0.1.0a96/share/tiled/ui/static/js/689.0cde4405.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/69.c379776e.chunk.js` & `tiled-0.1.0a96/share/tiled/ui/static/js/69.c379776e.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/69.c379776e.chunk.js.map` & `tiled-0.1.0a96/share/tiled/ui/static/js/69.c379776e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/705.eeca3f97.chunk.js` & `tiled-0.1.0a96/share/tiled/ui/static/js/705.eeca3f97.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/705.eeca3f97.chunk.js.map` & `tiled-0.1.0a96/share/tiled/ui/static/js/705.eeca3f97.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/741.fbe96b6d.chunk.js` & `tiled-0.1.0a96/share/tiled/ui/static/js/741.fbe96b6d.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/741.fbe96b6d.chunk.js.map` & `tiled-0.1.0a96/share/tiled/ui/static/js/741.fbe96b6d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/773.590aa2f4.chunk.js` & `tiled-0.1.0a96/share/tiled/ui/static/js/773.590aa2f4.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/773.590aa2f4.chunk.js.map` & `tiled-0.1.0a96/share/tiled/ui/static/js/773.590aa2f4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/787.54a97274.chunk.js` & `tiled-0.1.0a96/share/tiled/ui/static/js/787.54a97274.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/787.54a97274.chunk.js.map` & `tiled-0.1.0a96/share/tiled/ui/static/js/787.54a97274.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/837.22b95b21.chunk.js` & `tiled-0.1.0a96/share/tiled/ui/static/js/837.22b95b21.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/837.22b95b21.chunk.js.map` & `tiled-0.1.0a96/share/tiled/ui/static/js/837.22b95b21.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/858.2658cad8.chunk.js` & `tiled-0.1.0a96/share/tiled/ui/static/js/858.2658cad8.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/858.2658cad8.chunk.js.map` & `tiled-0.1.0a96/share/tiled/ui/static/js/858.2658cad8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/883.31ddd2ac.chunk.js` & `tiled-0.1.0a96/share/tiled/ui/static/js/883.31ddd2ac.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/883.31ddd2ac.chunk.js.map` & `tiled-0.1.0a96/share/tiled/ui/static/js/883.31ddd2ac.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/921.22e363f6.chunk.js` & `tiled-0.1.0a96/share/tiled/ui/static/js/921.22e363f6.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/921.22e363f6.chunk.js.map` & `tiled-0.1.0a96/share/tiled/ui/static/js/921.22e363f6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/986.f5c9d7cf.chunk.js` & `tiled-0.1.0a96/share/tiled/ui/static/js/986.f5c9d7cf.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/986.f5c9d7cf.chunk.js.map` & `tiled-0.1.0a96/share/tiled/ui/static/js/986.f5c9d7cf.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/main.5cc3eaa8.js` & `tiled-0.1.0a96/share/tiled/ui/static/js/main.5cc3eaa8.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/main.5cc3eaa8.js.LICENSE.txt` & `tiled-0.1.0a96/share/tiled/ui/static/js/main.5cc3eaa8.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/js/main.5cc3eaa8.js.map` & `tiled-0.1.0a96/share/tiled/ui/static/js/main.5cc3eaa8.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/media/roboto-all-300-normal.8fc5f5f22c9951113696.woff` & `tiled-0.1.0a96/share/tiled/ui/static/media/roboto-all-300-normal.8fc5f5f22c9951113696.woff`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/media/roboto-all-400-normal.376ea5d93f71583052f6.woff` & `tiled-0.1.0a96/share/tiled/ui/static/media/roboto-all-400-normal.376ea5d93f71583052f6.woff`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/media/roboto-all-500-normal.52cb737b682eb9661ee1.woff` & `tiled-0.1.0a96/share/tiled/ui/static/media/roboto-all-500-normal.52cb737b682eb9661ee1.woff`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/media/roboto-all-700-normal.ef6d1d09b20b877fee4e.woff` & `tiled-0.1.0a96/share/tiled/ui/static/media/roboto-all-700-normal.ef6d1d09b20b877fee4e.woff`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/media/roboto-cyrillic-300-normal.48e4b37ecbc5e155460e.woff2` & `tiled-0.1.0a96/share/tiled/ui/static/media/roboto-cyrillic-300-normal.48e4b37ecbc5e155460e.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/media/roboto-cyrillic-400-normal.5e493812deabd1d01e60.woff2` & `tiled-0.1.0a96/share/tiled/ui/static/media/roboto-cyrillic-400-normal.5e493812deabd1d01e60.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/media/roboto-cyrillic-500-normal.d1615fb9cd7f67f5018c.woff2` & `tiled-0.1.0a96/share/tiled/ui/static/media/roboto-cyrillic-500-normal.d1615fb9cd7f67f5018c.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/media/roboto-cyrillic-700-normal.0334efc0de1012200889.woff2` & `tiled-0.1.0a96/share/tiled/ui/static/media/roboto-cyrillic-700-normal.0334efc0de1012200889.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/media/roboto-cyrillic-ext-300-normal.12d37040a0160a948ff1.woff2` & `tiled-0.1.0a96/share/tiled/ui/static/media/roboto-cyrillic-ext-300-normal.12d37040a0160a948ff1.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/media/roboto-cyrillic-ext-400-normal.493afe7ae8ecfe268800.woff2` & `tiled-0.1.0a96/share/tiled/ui/static/media/roboto-cyrillic-ext-400-normal.493afe7ae8ecfe268800.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/media/roboto-cyrillic-ext-500-normal.3e748c93fe6a87bdedaa.woff2` & `tiled-0.1.0a96/share/tiled/ui/static/media/roboto-cyrillic-ext-500-normal.3e748c93fe6a87bdedaa.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/media/roboto-cyrillic-ext-700-normal.b816cda3107bb21c87e1.woff2` & `tiled-0.1.0a96/share/tiled/ui/static/media/roboto-cyrillic-ext-700-normal.b816cda3107bb21c87e1.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/media/roboto-greek-300-normal.7c6b44c55d4d9661e3ed.woff2` & `tiled-0.1.0a96/share/tiled/ui/static/media/roboto-greek-300-normal.7c6b44c55d4d9661e3ed.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/media/roboto-greek-400-normal.1cbfc636c911faa4d0ca.woff2` & `tiled-0.1.0a96/share/tiled/ui/static/media/roboto-greek-400-normal.1cbfc636c911faa4d0ca.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/media/roboto-greek-500-normal.007ca18d2cbae7381b39.woff2` & `tiled-0.1.0a96/share/tiled/ui/static/media/roboto-greek-500-normal.007ca18d2cbae7381b39.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/media/roboto-greek-700-normal.3292e831b18d0c23d609.woff2` & `tiled-0.1.0a96/share/tiled/ui/static/media/roboto-greek-700-normal.3292e831b18d0c23d609.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/media/roboto-greek-ext-300-normal.04e05839d6a35e046c13.woff2` & `tiled-0.1.0a96/share/tiled/ui/static/media/roboto-greek-ext-300-normal.04e05839d6a35e046c13.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/media/roboto-greek-ext-400-normal.bb723e8458c9c653e505.woff2` & `tiled-0.1.0a96/share/tiled/ui/static/media/roboto-greek-ext-400-normal.bb723e8458c9c653e505.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/media/roboto-greek-ext-500-normal.9c0d384f31e2c914edf3.woff2` & `tiled-0.1.0a96/share/tiled/ui/static/media/roboto-greek-ext-500-normal.9c0d384f31e2c914edf3.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/media/roboto-greek-ext-700-normal.9674bc0ae12c2551d9d1.woff2` & `tiled-0.1.0a96/share/tiled/ui/static/media/roboto-greek-ext-700-normal.9674bc0ae12c2551d9d1.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/media/roboto-latin-300-normal.0109a2ace896a506a0aa.woff2` & `tiled-0.1.0a96/share/tiled/ui/static/media/roboto-latin-300-normal.0109a2ace896a506a0aa.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/media/roboto-latin-400-normal.4673b4537a84c7f7a130.woff2` & `tiled-0.1.0a96/share/tiled/ui/static/media/roboto-latin-400-normal.4673b4537a84c7f7a130.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/media/roboto-latin-500-normal.869888415d0b1a99ae5c.woff2` & `tiled-0.1.0a96/share/tiled/ui/static/media/roboto-latin-500-normal.869888415d0b1a99ae5c.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/media/roboto-latin-700-normal.0682ca7f74351d42bf73.woff2` & `tiled-0.1.0a96/share/tiled/ui/static/media/roboto-latin-700-normal.0682ca7f74351d42bf73.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/media/roboto-latin-ext-300-normal.a29236e0fc30e8482530.woff2` & `tiled-0.1.0a96/share/tiled/ui/static/media/roboto-latin-ext-300-normal.a29236e0fc30e8482530.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/media/roboto-latin-ext-400-normal.c3dcdbd5bb4d4af80817.woff2` & `tiled-0.1.0a96/share/tiled/ui/static/media/roboto-latin-ext-400-normal.c3dcdbd5bb4d4af80817.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/media/roboto-latin-ext-500-normal.feaff916fd609e310efe.woff2` & `tiled-0.1.0a96/share/tiled/ui/static/media/roboto-latin-ext-500-normal.feaff916fd609e310efe.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/media/roboto-latin-ext-700-normal.bcf37d666ce10b3556cd.woff2` & `tiled-0.1.0a96/share/tiled/ui/static/media/roboto-latin-ext-700-normal.bcf37d666ce10b3556cd.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/media/roboto-vietnamese-300-normal.af9afdc10c93e4118e90.woff2` & `tiled-0.1.0a96/share/tiled/ui/static/media/roboto-vietnamese-300-normal.af9afdc10c93e4118e90.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/media/roboto-vietnamese-400-normal.c0bec65d01f776c00c91.woff2` & `tiled-0.1.0a96/share/tiled/ui/static/media/roboto-vietnamese-400-normal.c0bec65d01f776c00c91.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/media/roboto-vietnamese-500-normal.b8e494da1ec1f1824769.woff2` & `tiled-0.1.0a96/share/tiled/ui/static/media/roboto-vietnamese-500-normal.b8e494da1ec1f1824769.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/share/tiled/ui/static/media/roboto-vietnamese-700-normal.3096f18acebc3f07020d.woff2` & `tiled-0.1.0a96/share/tiled/ui/static/media/roboto-vietnamese-700-normal.3096f18acebc3f07020d.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/conftest.py` & `tiled-0.1.0a96/tiled/_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_access_control.py` & `tiled-0.1.0a96/tiled/_tests/test_access_control.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_allow_origins.py` & `tiled-0.1.0a96/tiled/_tests/test_allow_origins.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_array.py` & `tiled-0.1.0a96/tiled/_tests/test_array.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_authentication.py` & `tiled-0.1.0a96/tiled/_tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_authenticators.py` & `tiled-0.1.0a96/tiled/_tests/test_authenticators.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_caches.py` & `tiled-0.1.0a96/tiled/_tests/test_caches.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_catalog.py` & `tiled-0.1.0a96/tiled/_tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_client.py` & `tiled-0.1.0a96/tiled/_tests/test_client.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_client_cache.py` & `tiled-0.1.0a96/tiled/_tests/test_client_cache.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_config.py` & `tiled-0.1.0a96/tiled/_tests/test_config.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_custom_format.py` & `tiled-0.1.0a96/tiled/_tests/test_custom_format.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_dataframe.py` & `tiled-0.1.0a96/tiled/_tests/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_directory_walker.py` & `tiled-0.1.0a96/tiled/_tests/test_directory_walker.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_distinct.py` & `tiled-0.1.0a96/tiled/_tests/test_distinct.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_export.py` & `tiled-0.1.0a96/tiled/_tests/test_export.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_hdf5.py` & `tiled-0.1.0a96/tiled/_tests/test_hdf5.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_history.py` & `tiled-0.1.0a96/tiled/_tests/test_history.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_import_object.py` & `tiled-0.1.0a96/tiled/_tests/test_import_object.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_indexers.py` & `tiled-0.1.0a96/tiled/_tests/test_indexers.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_inlined_contents.py` & `tiled-0.1.0a96/tiled/_tests/test_inlined_contents.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_json.py` & `tiled-0.1.0a96/tiled/_tests/test_json.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_metrics.py` & `tiled-0.1.0a96/tiled/_tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_object_cache.py` & `tiled-0.1.0a96/tiled/_tests/test_object_cache.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_openapi.py` & `tiled-0.1.0a96/tiled/_tests/test_openapi.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_pickle.py` & `tiled-0.1.0a96/tiled/_tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_queries.py` & `tiled-0.1.0a96/tiled/_tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_scaled_config_option.py` & `tiled-0.1.0a96/tiled/_tests/test_scaled_config_option.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_search.py` & `tiled-0.1.0a96/tiled/_tests/test_search.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_size_limit.py` & `tiled-0.1.0a96/tiled/_tests/test_size_limit.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_sort.py` & `tiled-0.1.0a96/tiled/_tests/test_sort.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_sparse.py` & `tiled-0.1.0a96/tiled/_tests/test_sparse.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_specs_and_references.py` & `tiled-0.1.0a96/tiled/_tests/test_specs_and_references.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_structured_array.py` & `tiled-0.1.0a96/tiled/_tests/test_structured_array.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_tiff.py` & `tiled-0.1.0a96/tiled/_tests/test_tiff.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_validation.py` & `tiled-0.1.0a96/tiled/_tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_writing.py` & `tiled-0.1.0a96/tiled/_tests/test_writing.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/test_xarray.py` & `tiled-0.1.0a96/tiled/_tests/test_xarray.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/_tests/utils.py` & `tiled-0.1.0a96/tiled/_tests/utils.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/access_policies.py` & `tiled-0.1.0a96/tiled/access_policies.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/adapters/array.py` & `tiled-0.1.0a96/tiled/adapters/array.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/adapters/dataframe.py` & `tiled-0.1.0a96/tiled/adapters/dataframe.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/adapters/excel.py` & `tiled-0.1.0a96/tiled/adapters/excel.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/adapters/files.py` & `tiled-0.1.0a96/tiled/adapters/files.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/adapters/hdf5.py` & `tiled-0.1.0a96/tiled/adapters/hdf5.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/adapters/mapping.py` & `tiled-0.1.0a96/tiled/adapters/mapping.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/adapters/parquet.py` & `tiled-0.1.0a96/tiled/adapters/parquet.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/adapters/sparse.py` & `tiled-0.1.0a96/tiled/adapters/sparse.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/adapters/sparse_blocks_parquet.py` & `tiled-0.1.0a96/tiled/adapters/sparse_blocks_parquet.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/adapters/tiff.py` & `tiled-0.1.0a96/tiled/adapters/tiff.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/adapters/utils.py` & `tiled-0.1.0a96/tiled/adapters/utils.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/adapters/xarray.py` & `tiled-0.1.0a96/tiled/adapters/xarray.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/adapters/zarr.py` & `tiled-0.1.0a96/tiled/adapters/zarr.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/authenticators.py` & `tiled-0.1.0a96/tiled/authenticators.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/catalog/adapter.py` & `tiled-0.1.0a96/tiled/catalog/adapter.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/catalog/explain.py` & `tiled-0.1.0a96/tiled/catalog/explain.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/catalog/orm.py` & `tiled-0.1.0a96/tiled/catalog/orm.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/client/_testclient.py` & `tiled-0.1.0a96/tiled/client/_testclient.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/client/array.py` & `tiled-0.1.0a96/tiled/client/array.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/client/auth.py` & `tiled-0.1.0a96/tiled/client/auth.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/client/base.py` & `tiled-0.1.0a96/tiled/client/base.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/client/cache.py` & `tiled-0.1.0a96/tiled/client/cache.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/client/constructors.py` & `tiled-0.1.0a96/tiled/client/constructors.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/client/context.py` & `tiled-0.1.0a96/tiled/client/context.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/client/dataframe.py` & `tiled-0.1.0a96/tiled/client/dataframe.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/client/node.py` & `tiled-0.1.0a96/tiled/client/node.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/client/sparse.py` & `tiled-0.1.0a96/tiled/client/sparse.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/client/utils.py` & `tiled-0.1.0a96/tiled/client/utils.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/client/xarray.py` & `tiled-0.1.0a96/tiled/client/xarray.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/commandline/_admin.py` & `tiled-0.1.0a96/tiled/commandline/_admin.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/commandline/_api_key.py` & `tiled-0.1.0a96/tiled/commandline/_api_key.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/commandline/_catalog.py` & `tiled-0.1.0a96/tiled/commandline/_catalog.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/commandline/_profile.py` & `tiled-0.1.0a96/tiled/commandline/_profile.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/commandline/_serve.py` & `tiled-0.1.0a96/tiled/commandline/_serve.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/commandline/_utils.py` & `tiled-0.1.0a96/tiled/commandline/_utils.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/commandline/main.py` & `tiled-0.1.0a96/tiled/commandline/main.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/config.py` & `tiled-0.1.0a96/tiled/config.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/config_schemas/client_profiles.yml` & `tiled-0.1.0a96/tiled/config_schemas/client_profiles.yml`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/config_schemas/service_configuration.yml` & `tiled-0.1.0a96/tiled/config_schemas/service_configuration.yml`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/database/alembic.ini.template` & `tiled-0.1.0a96/tiled/database/alembic.ini.template`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/database/alembic_utils.py` & `tiled-0.1.0a96/tiled/database/alembic_utils.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/database/connection_pool.py` & `tiled-0.1.0a96/tiled/database/connection_pool.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/database/core.py` & `tiled-0.1.0a96/tiled/database/core.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/database/migrations/env.py` & `tiled-0.1.0a96/tiled/database/migrations/env.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/database/migrations/versions/481830dd6c11_initialize.py` & `tiled-0.1.0a96/tiled/database/migrations/versions/481830dd6c11_initialize.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/database/migrations/versions/4a9dfaba4a98_add_pendingsession.py` & `tiled-0.1.0a96/tiled/database/migrations/versions/4a9dfaba4a98_add_pendingsession.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/database/migrations/versions/56809bcbfcb0_add_create_scope_to_default_roles.py` & `tiled-0.1.0a96/tiled/database/migrations/versions/56809bcbfcb0_add_create_scope_to_default_roles.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/database/migrations/versions/722ff4e4fcc7_add_write_scopes_to_default_roles.py` & `tiled-0.1.0a96/tiled/database/migrations/versions/722ff4e4fcc7_add_write_scopes_to_default_roles.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/database/orm.py` & `tiled-0.1.0a96/tiled/database/orm.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/examples/generate_files.py` & `tiled-0.1.0a96/tiled/examples/generate_files.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/examples/generated.py` & `tiled-0.1.0a96/tiled/examples/generated.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/examples/generated_minimal.py` & `tiled-0.1.0a96/tiled/examples/generated_minimal.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/examples/nexus.py` & `tiled-0.1.0a96/tiled/examples/nexus.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/examples/toy_authentication.py` & `tiled-0.1.0a96/tiled/examples/toy_authentication.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/examples/xdi.py` & `tiled-0.1.0a96/tiled/examples/xdi.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/iterviews.py` & `tiled-0.1.0a96/tiled/iterviews.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/media_type_registration.py` & `tiled-0.1.0a96/tiled/media_type_registration.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/profiles.py` & `tiled-0.1.0a96/tiled/profiles.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/queries.py` & `tiled-0.1.0a96/tiled/queries.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/query_registration.py` & `tiled-0.1.0a96/tiled/query_registration.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/scopes.py` & `tiled-0.1.0a96/tiled/scopes.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/serialization/__init__.py` & `tiled-0.1.0a96/tiled/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/serialization/array.py` & `tiled-0.1.0a96/tiled/serialization/array.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/serialization/dataframe.py` & `tiled-0.1.0a96/tiled/serialization/dataframe.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/serialization/image_serializer_helpers.py` & `tiled-0.1.0a96/tiled/serialization/image_serializer_helpers.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/serialization/node.py` & `tiled-0.1.0a96/tiled/serialization/node.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/serialization/sparse.py` & `tiled-0.1.0a96/tiled/serialization/sparse.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/serialization/xarray.py` & `tiled-0.1.0a96/tiled/serialization/xarray.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/server/app.py` & `tiled-0.1.0a96/tiled/server/app.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/server/authentication.py` & `tiled-0.1.0a96/tiled/server/authentication.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/server/compression.py` & `tiled-0.1.0a96/tiled/server/compression.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/server/core.py` & `tiled-0.1.0a96/tiled/server/core.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/server/dependencies.py` & `tiled-0.1.0a96/tiled/server/dependencies.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/server/etag.py` & `tiled-0.1.0a96/tiled/server/etag.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/server/metrics.py` & `tiled-0.1.0a96/tiled/server/metrics.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/server/object_cache.py` & `tiled-0.1.0a96/tiled/server/object_cache.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/server/pydantic_array.py` & `tiled-0.1.0a96/tiled/server/pydantic_array.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/server/pydantic_dataframe.py` & `tiled-0.1.0a96/tiled/server/pydantic_dataframe.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/server/pydantic_sparse.py` & `tiled-0.1.0a96/tiled/server/pydantic_sparse.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/server/router.py` & `tiled-0.1.0a96/tiled/server/router.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/server/schemas.py` & `tiled-0.1.0a96/tiled/server/schemas.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/server/settings.py` & `tiled-0.1.0a96/tiled/server/settings.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/server/utils.py` & `tiled-0.1.0a96/tiled/server/utils.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/structures/array.py` & `tiled-0.1.0a96/tiled/structures/array.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/structures/core.py` & `tiled-0.1.0a96/tiled/structures/core.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/structures/dataframe.py` & `tiled-0.1.0a96/tiled/structures/dataframe.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/structures/sparse.py` & `tiled-0.1.0a96/tiled/structures/sparse.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/utils.py` & `tiled-0.1.0a96/tiled/utils.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled/validation_registration.py` & `tiled-0.1.0a96/tiled/validation_registration.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled.egg-info/PKG-INFO` & `tiled-0.1.0a96/tiled.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiled
-Version: 0.1.0a95
+Version: 0.1.0a96
 Summary: Tile-based access to SciPy/PyData data structures over the web in many formats
 Home-page: https://github.com/bluesky/tiled
 Author: Bluesky Collaboration
 Author-email: dallan@bnl.gov
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `tiled-0.1.0a95/tiled.egg-info/SOURCES.txt` & `tiled-0.1.0a96/tiled.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/tiled.egg-info/requires.txt` & `tiled-0.1.0a96/tiled.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a95/versioneer.py` & `tiled-0.1.0a96/versioneer.py`

 * *Files identical despite different names*

