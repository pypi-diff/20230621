# Comparing `tmp/httpbinx-1.3.2.tar.gz` & `tmp/httpbinx-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpbinx-1.3.2.tar", last modified: Thu Jun  1 08:51:07 2023, max compression
+gzip compressed data, was "httpbinx-1.4.0.tar", last modified: Wed Jun 21 10:36:12 2023, max compression
```

## Comparing `httpbinx-1.3.2.tar` & `httpbinx-1.4.0.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:51:07.578337 httpbinx-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-01 08:50:52.000000 httpbinx-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-01 08:50:52.000000 httpbinx-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-01 08:51:07.574337 httpbinx-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-01 08:50:52.000000 httpbinx-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:51:07.566337 httpbinx-1.3.2/httpbinx/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-01 08:50:52.000000 httpbinx-1.3.2/httpbinx/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-01 08:50:52.000000 httpbinx-1.3.2/httpbinx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-01 08:50:52.000000 httpbinx-1.3.2/httpbinx/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:51:07.570337 httpbinx-1.3.2/httpbinx/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:50:52.000000 httpbinx-1.3.2/httpbinx/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-01 08:50:52.000000 httpbinx-1.3.2/httpbinx/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-01 08:50:52.000000 httpbinx-1.3.2/httpbinx/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:51:07.570337 httpbinx-1.3.2/httpbinx/routers/
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-01 08:50:52.000000 httpbinx-1.3.2/httpbinx/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-01 08:50:52.000000 httpbinx-1.3.2/httpbinx/routers/anything.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-01 08:50:52.000000 httpbinx-1.3.2/httpbinx/routers/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-01 08:50:52.000000 httpbinx-1.3.2/httpbinx/routers/cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-06-01 08:50:52.000000 httpbinx-1.3.2/httpbinx/routers/dynamicdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-01 08:50:52.000000 httpbinx-1.3.2/httpbinx/routers/httpmethods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-01 08:50:52.000000 httpbinx-1.3.2/httpbinx/routers/images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:51:07.570337 httpbinx-1.3.2/httpbinx/routers/inspection/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-01 08:50:52.000000 httpbinx-1.3.2/httpbinx/routers/inspection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-01 08:50:52.000000 httpbinx-1.3.2/httpbinx/routers/inspection/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-06-01 08:50:52.000000 httpbinx-1.3.2/httpbinx/routers/inspection/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-01 08:50:52.000000 httpbinx-1.3.2/httpbinx/routers/redirects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-06-01 08:50:52.000000 httpbinx-1.3.2/httpbinx/routers/responseformats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-01 08:50:52.000000 httpbinx-1.3.2/httpbinx/routers/statuscodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-01 08:50:52.000000 httpbinx-1.3.2/httpbinx/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:51:07.574337 httpbinx-1.3.2/httpbinx/static/
--rw-r--r--   0 runner    (1001) docker     (123)    14058 2023-06-01 08:50:52.000000 httpbinx-1.3.2/httpbinx/static/UTF-8-demo.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-01 08:50:52.000000 httpbinx-1.3.2/httpbinx/static/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:51:07.574337 httpbinx-1.3.2/httpbinx/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-06-01 08:50:52.000000 httpbinx-1.3.2/httpbinx/static/images/httbinx_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-01 08:50:52.000000 httpbinx-1.3.2/httpbinx/static/images/httpbinx_cover.png
--rw-r--r--   0 runner    (1001) docker     (123)    35588 2023-06-01 08:50:52.000000 httpbinx-1.3.2/httpbinx/static/images/jackal.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-06-01 08:50:52.000000 httpbinx-1.3.2/httpbinx/static/images/pig_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-06-01 08:50:52.000000 httpbinx-1.3.2/httpbinx/static/images/svg_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-06-01 08:50:52.000000 httpbinx-1.3.2/httpbinx/static/images/wolf_1.webp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:51:07.574337 httpbinx-1.3.2/httpbinx/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-01 08:50:52.000000 httpbinx-1.3.2/httpbinx/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-06-01 08:50:52.000000 httpbinx-1.3.2/httpbinx/templates/moby.html
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-01 08:50:52.000000 httpbinx-1.3.2/httpbinx/templates/sample.xml
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-01 08:50:52.000000 httpbinx-1.3.2/httpbinx/templates/trackingscripts.html
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-01 08:50:52.000000 httpbinx-1.3.2/httpbinx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:51:07.570337 httpbinx-1.3.2/httpbinx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-01 08:51:07.000000 httpbinx-1.3.2/httpbinx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-01 08:51:07.000000 httpbinx-1.3.2/httpbinx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 08:51:07.000000 httpbinx-1.3.2/httpbinx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-01 08:51:07.000000 httpbinx-1.3.2/httpbinx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 08:51:07.000000 httpbinx-1.3.2/httpbinx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 08:51:07.578337 httpbinx-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-01 08:50:52.000000 httpbinx-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:51:07.574337 httpbinx-1.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-01 08:50:52.000000 httpbinx-1.3.2/tests/test_anything.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-01 08:50:52.000000 httpbinx-1.3.2/tests/test_dynamic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-01 08:50:52.000000 httpbinx-1.3.2/tests/test_http_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-01 08:50:52.000000 httpbinx-1.3.2/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-01 08:50:52.000000 httpbinx-1.3.2/tests/test_redirects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-01 08:50:52.000000 httpbinx-1.3.2/tests/test_request_inspection.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-01 08:50:52.000000 httpbinx-1.3.2/tests/test_response_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-01 08:50:52.000000 httpbinx-1.3.2/tests/test_status_codes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:36:12.901183 httpbinx-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-21 10:35:55.000000 httpbinx-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-21 10:35:55.000000 httpbinx-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-21 10:36:12.901183 httpbinx-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-21 10:35:55.000000 httpbinx-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:36:12.881183 httpbinx-1.4.0/httpbinx/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:36:12.885183 httpbinx-1.4.0/httpbinx/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:36:12.889183 httpbinx-1.4.0/httpbinx/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/routers/anything.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/routers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/routers/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/routers/dynamicdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/routers/httpmethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/routers/images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:36:12.889183 httpbinx-1.4.0/httpbinx/routers/inspection/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/routers/inspection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/routers/inspection/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/routers/inspection/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/routers/redirects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/routers/responseformats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/routers/statuscodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:36:12.893183 httpbinx-1.4.0/httpbinx/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    14058 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/static/UTF-8-demo.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/static/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:36:12.893183 httpbinx-1.4.0/httpbinx/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/static/images/httbinx_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/static/images/httpbinx_cover.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35588 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/static/images/jackal.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/static/images/pig_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/static/images/svg_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/static/images/wolf_1.webp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:36:12.897183 httpbinx-1.4.0/httpbinx/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/templates/moby.html
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/templates/sample.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/templates/trackingscripts.html
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-21 10:35:55.000000 httpbinx-1.4.0/httpbinx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:36:12.885183 httpbinx-1.4.0/httpbinx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-21 10:36:12.000000 httpbinx-1.4.0/httpbinx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-21 10:36:12.000000 httpbinx-1.4.0/httpbinx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 10:36:12.000000 httpbinx-1.4.0/httpbinx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-21 10:36:12.000000 httpbinx-1.4.0/httpbinx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 10:36:12.000000 httpbinx-1.4.0/httpbinx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 10:36:12.901183 httpbinx-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-21 10:35:55.000000 httpbinx-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:36:12.897183 httpbinx-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-21 10:35:55.000000 httpbinx-1.4.0/tests/test_anything.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-21 10:35:55.000000 httpbinx-1.4.0/tests/test_dynamic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-21 10:35:55.000000 httpbinx-1.4.0/tests/test_http_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-21 10:35:55.000000 httpbinx-1.4.0/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-21 10:35:55.000000 httpbinx-1.4.0/tests/test_redirects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-21 10:35:55.000000 httpbinx-1.4.0/tests/test_request_inspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-21 10:35:55.000000 httpbinx-1.4.0/tests/test_response_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-21 10:35:55.000000 httpbinx-1.4.0/tests/test_status_codes.py
```

### Comparing `httpbinx-1.3.2/LICENSE` & `httpbinx-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/PKG-INFO` & `httpbinx-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpbinx
-Version: 1.3.2
+Version: 1.4.0
 Summary: HTTP Request & Response Service, written in Python + FastAPI.
 Home-page: https://github.com/imleowoo/httpbinx
 Author: Leo
 Author-email: imleowoo@outlook.com
 Maintainer: Leo
 Maintainer-email: imleowoo@outlook.com
 License: MIT
```

### Comparing `httpbinx-1.3.2/README.md` & `httpbinx-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/httpbinx/constants.py` & `httpbinx-1.4.0/httpbinx/constants.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/httpbinx/helpers.py` & `httpbinx-1.4.0/httpbinx/helpers.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/httpbinx/main.py` & `httpbinx-1.4.0/httpbinx/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # -*- coding: utf-8 -*-
 from os import path
 
 from fastapi import FastAPI
 from starlette.middleware.cors import CORSMiddleware
 from starlette.staticfiles import StaticFiles
 
+from httpbinx.meta import tags_metadata
 from httpbinx.routers import router
 
 app = FastAPI(
     title='httpbinx',
     description='HTTP Request & Response Service, '
                 'written in Python + FastAPI.',
     docs_url='/',  # swagger docs page url
     swagger_ui_parameters={'docExpansion': 'none'},
+    openapi_tags=tags_metadata
 )
 
 app.mount(
     '/static',
     StaticFiles(directory=path.join(path.dirname(__file__), 'static')),
     name='static'
 )
```

### Comparing `httpbinx-1.3.2/httpbinx/routers/__init__.py` & `httpbinx-1.4.0/httpbinx/routers/__init__.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/httpbinx/routers/anything.py` & `httpbinx-1.4.0/httpbinx/routers/anything.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/httpbinx/routers/auth.py` & `httpbinx-1.4.0/httpbinx/routers/auth.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/httpbinx/routers/cookies.py` & `httpbinx-1.4.0/httpbinx/routers/cookies.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/httpbinx/routers/dynamicdata.py` & `httpbinx-1.4.0/httpbinx/routers/dynamicdata.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/httpbinx/routers/httpmethods.py` & `httpbinx-1.4.0/httpbinx/routers/httpmethods.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/httpbinx/routers/images.py` & `httpbinx-1.4.0/httpbinx/routers/images.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/httpbinx/routers/inspection/request.py` & `httpbinx-1.4.0/httpbinx/routers/inspection/request.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/httpbinx/routers/inspection/response.py` & `httpbinx-1.4.0/httpbinx/routers/inspection/response.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/httpbinx/routers/redirects.py` & `httpbinx-1.4.0/httpbinx/routers/redirects.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/httpbinx/routers/responseformats.py` & `httpbinx-1.4.0/httpbinx/routers/responseformats.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/httpbinx/routers/statuscodes.py` & `httpbinx-1.4.0/httpbinx/routers/statuscodes.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/httpbinx/schemas.py` & `httpbinx-1.4.0/httpbinx/schemas.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/httpbinx/static/UTF-8-demo.txt` & `httpbinx-1.4.0/httpbinx/static/UTF-8-demo.txt`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/httpbinx/static/favicon.png` & `httpbinx-1.4.0/httpbinx/static/favicon.png`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/httpbinx/static/images/httbinx_logo.png` & `httpbinx-1.4.0/httpbinx/static/images/httbinx_logo.png`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/httpbinx/static/images/httpbinx_cover.png` & `httpbinx-1.4.0/httpbinx/static/images/httpbinx_cover.png`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/httpbinx/static/images/jackal.jpg` & `httpbinx-1.4.0/httpbinx/static/images/jackal.jpg`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/httpbinx/static/images/pig_icon.png` & `httpbinx-1.4.0/httpbinx/static/images/pig_icon.png`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/httpbinx/static/images/svg_logo.svg` & `httpbinx-1.4.0/httpbinx/static/images/svg_logo.svg`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/httpbinx/static/images/wolf_1.webp` & `httpbinx-1.4.0/httpbinx/static/images/wolf_1.webp`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/httpbinx/templates/index.html` & `httpbinx-1.4.0/httpbinx/templates/index.html`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/httpbinx/templates/moby.html` & `httpbinx-1.4.0/httpbinx/templates/moby.html`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/httpbinx/templates/sample.xml` & `httpbinx-1.4.0/httpbinx/templates/sample.xml`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/httpbinx/templates/trackingscripts.html` & `httpbinx-1.4.0/httpbinx/templates/trackingscripts.html`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/httpbinx.egg-info/PKG-INFO` & `httpbinx-1.4.0/httpbinx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpbinx
-Version: 1.3.2
+Version: 1.4.0
 Summary: HTTP Request & Response Service, written in Python + FastAPI.
 Home-page: https://github.com/imleowoo/httpbinx
 Author: Leo
 Author-email: imleowoo@outlook.com
 Maintainer: Leo
 Maintainer-email: imleowoo@outlook.com
 License: MIT
```

### Comparing `httpbinx-1.3.2/httpbinx.egg-info/SOURCES.txt` & `httpbinx-1.4.0/httpbinx.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 setup.py
 httpbinx/VERSION
 httpbinx/__init__.py
 httpbinx/constants.py
 httpbinx/helpers.py
 httpbinx/main.py
+httpbinx/meta.py
 httpbinx/schemas.py
 httpbinx/utils.py
 httpbinx.egg-info/PKG-INFO
 httpbinx.egg-info/SOURCES.txt
 httpbinx.egg-info/dependency_links.txt
 httpbinx.egg-info/requires.txt
 httpbinx.egg-info/top_level.txt
```

### Comparing `httpbinx-1.3.2/setup.py` & `httpbinx-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/tests/test_dynamic_data.py` & `httpbinx-1.4.0/tests/test_dynamic_data.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/tests/test_http_methods.py` & `httpbinx-1.4.0/tests/test_http_methods.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/tests/test_request_inspection.py` & `httpbinx-1.4.0/tests/test_request_inspection.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/tests/test_response_formats.py` & `httpbinx-1.4.0/tests/test_response_formats.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.2/tests/test_status_codes.py` & `httpbinx-1.4.0/tests/test_status_codes.py`

 * *Files identical despite different names*

