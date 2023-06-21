# Comparing `tmp/serialtools-0.1.0.tar.gz` & `tmp/serialtools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serialtools-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "serialtools-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `serialtools-0.1.0.tar` & `serialtools-0.2.0.tar`

### file list

```diff
@@ -1,100 +1,100 @@
--rw-r--r--   0        0        0      330 2023-06-02 06:55:40.811546 serialtools-0.1.0/.gitignore
--rw-r--r--   0        0        0      119 2023-06-21 09:42:29.977581 serialtools-0.1.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      657 2023-06-21 08:53:39.687960 serialtools-0.1.0/LICENSE
--rw-r--r--   0        0        0      444 2023-06-21 09:42:29.977581 serialtools-0.1.0/README.md
--rw-r--r--   0        0        0      638 2023-06-21 09:42:29.977581 serialtools-0.1.0/docs/Makefile
--rw-r--r--   0        0        0      985 2023-06-21 09:42:29.977581 serialtools-0.1.0/docs/build/html/_sources/index.rst.txt
--rw-r--r--   0        0        0       70 2023-06-21 09:42:29.977581 serialtools-0.1.0/docs/build/html/_sources/modules.rst.txt
--rw-r--r--   0        0        0      157 2023-06-21 09:42:29.977581 serialtools-0.1.0/docs/build/html/_sources/serialtools.apps.decode.rst.txt
--rw-r--r--   0        0        0      151 2023-06-21 09:42:29.977581 serialtools-0.1.0/docs/build/html/_sources/serialtools.apps.dump.rst.txt
--rw-r--r--   0        0        0      302 2023-06-21 09:42:29.977581 serialtools-0.1.0/docs/build/html/_sources/serialtools.apps.rst.txt
--rw-r--r--   0        0        0      151 2023-06-21 09:42:29.977581 serialtools-0.1.0/docs/build/html/_sources/serialtools.apps.send.rst.txt
--rw-r--r--   0        0        0      133 2023-06-21 09:42:29.977581 serialtools-0.1.0/docs/build/html/_sources/serialtools.bus.rst.txt
--rw-r--r--   0        0        0      148 2023-06-21 09:42:29.977581 serialtools-0.1.0/docs/build/html/_sources/serialtools.database.rst.txt
--rw-r--r--   0        0        0      171 2023-06-21 09:42:29.977581 serialtools-0.1.0/docs/build/html/_sources/serialtools.database_config.rst.txt
--rw-r--r--   0        0        0      360 2023-06-21 09:42:29.977581 serialtools-0.1.0/docs/build/html/_sources/serialtools.rst.txt
--rw-r--r--   0        0        0     4289 2023-06-21 10:13:03.187415 serialtools-0.1.0/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0        0        0    14813 2023-06-21 10:13:04.494072 serialtools-0.1.0/docs/build/html/_static/basic.css
--rw-r--r--   0        0        0     3229 2023-06-21 09:42:29.977581 serialtools-0.1.0/docs/build/html/_static/css/badge_only.css
--rw-r--r--   0        0        0    87624 2023-06-21 09:42:29.977581 serialtools-0.1.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0        0        0    67312 2023-06-21 09:42:29.977581 serialtools-0.1.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0        0        0    86288 2023-06-21 09:42:29.980915 serialtools-0.1.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0        0        0    66444 2023-06-21 09:42:29.980915 serialtools-0.1.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0        0        0   165742 2023-06-21 09:42:29.980915 serialtools-0.1.0/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2023-06-21 09:42:29.984248 serialtools-0.1.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2023-06-21 09:42:29.987581 serialtools-0.1.0/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2023-06-21 09:42:29.987581 serialtools-0.1.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2023-06-21 09:42:29.987581 serialtools-0.1.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0   323344 2023-06-21 09:42:29.987581 serialtools-0.1.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0        0        0   193308 2023-06-21 09:42:29.987581 serialtools-0.1.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0        0        0   309728 2023-06-21 09:42:29.990915 serialtools-0.1.0/docs/build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0        0        0   184912 2023-06-21 09:42:29.990915 serialtools-0.1.0/docs/build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0        0        0   328412 2023-06-21 09:42:29.990915 serialtools-0.1.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0        0        0   195704 2023-06-21 09:42:29.994248 serialtools-0.1.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0        0        0   309192 2023-06-21 09:42:29.994248 serialtools-0.1.0/docs/build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0        0        0   182708 2023-06-21 09:42:29.994248 serialtools-0.1.0/docs/build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0        0        0   135314 2023-06-21 09:42:29.994248 serialtools-0.1.0/docs/build/html/_static/css/theme.css
--rw-r--r--   0        0        0     4472 2023-06-21 09:42:29.994248 serialtools-0.1.0/docs/build/html/_static/doctools.js
--rw-r--r--   0        0        0      421 2023-06-21 10:13:04.497405 serialtools-0.1.0/docs/build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2023-06-21 09:42:29.994248 serialtools-0.1.0/docs/build/html/_static/file.png
--rw-r--r--   0        0        0    89501 2023-06-21 10:13:03.187415 serialtools-0.1.0/docs/build/html/_static/jquery.js
--rw-r--r--   0        0        0      934 2023-06-21 09:42:29.997581 serialtools-0.1.0/docs/build/html/_static/js/badge_only.js
--rw-r--r--   0        0        0     4370 2023-06-21 09:42:29.997581 serialtools-0.1.0/docs/build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0        0        0     2734 2023-06-21 09:42:29.997581 serialtools-0.1.0/docs/build/html/_static/js/html5shiv.min.js
--rw-r--r--   0        0        0     5023 2023-06-21 09:42:29.997581 serialtools-0.1.0/docs/build/html/_static/js/theme.js
--rw-r--r--   0        0        0     4758 2023-06-21 10:13:04.494072 serialtools-0.1.0/docs/build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2023-06-21 09:42:29.997581 serialtools-0.1.0/docs/build/html/_static/minus.png
--rw-r--r--   0        0        0       46 2023-06-21 09:42:29.997581 serialtools-0.1.0/docs/build/html/_static/no-ligatures-in-code.css
--rw-r--r--   0        0        0       90 2023-06-21 09:42:29.997581 serialtools-0.1.0/docs/build/html/_static/plus.png
--rw-r--r--   0        0        0     4819 2023-06-21 10:13:04.487405 serialtools-0.1.0/docs/build/html/_static/pygments.css
--rw-r--r--   0        0        0    18215 2023-06-21 09:42:29.997581 serialtools-0.1.0/docs/build/html/_static/searchtools.js
--rw-r--r--   0        0        0     4712 2023-06-21 09:42:29.997581 serialtools-0.1.0/docs/build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0      204 2023-06-21 09:42:29.997581 serialtools-0.1.0/docs/build/html/_static/sphinx_paramlinks.css
--rw-r--r--   0        0        0      117 2023-06-21 09:42:29.997581 serialtools-0.1.0/docs/build/html/_static/tab-size.css
--rw-r--r--   0        0        0    26275 2023-06-21 10:13:04.464072 serialtools-0.1.0/docs/build/html/genindex.html
--rw-r--r--   0        0        0    14126 2023-06-21 10:13:04.160741 serialtools-0.1.0/docs/build/html/index.html
--rw-r--r--   0        0        0    10059 2023-06-21 10:13:04.177407 serialtools-0.1.0/docs/build/html/modules.html
--rw-r--r--   0        0        0     1242 2023-06-21 10:13:04.507405 serialtools-0.1.0/docs/build/html/objects.inv
--rw-r--r--   0        0        0     6583 2023-06-21 10:13:04.477405 serialtools-0.1.0/docs/build/html/py-modindex.html
--rw-r--r--   0        0        0     4797 2023-06-21 10:13:04.487405 serialtools-0.1.0/docs/build/html/search.html
--rw-r--r--   0        0        0    22130 2023-06-21 10:13:04.504071 serialtools-0.1.0/docs/build/html/searchindex.js
--rw-r--r--   0        0        0    14594 2023-06-21 10:13:04.280740 serialtools-0.1.0/docs/build/html/serialtools.apps.decode.html
--rw-r--r--   0        0        0    12182 2023-06-21 10:13:04.297406 serialtools-0.1.0/docs/build/html/serialtools.apps.dump.html
--rw-r--r--   0        0        0    10486 2023-06-21 10:13:04.264073 serialtools-0.1.0/docs/build/html/serialtools.apps.html
--rw-r--r--   0        0        0    10684 2023-06-21 10:13:04.307406 serialtools-0.1.0/docs/build/html/serialtools.apps.send.html
--rw-r--r--   0        0        0    41636 2023-06-21 10:13:04.347406 serialtools-0.1.0/docs/build/html/serialtools.bus.html
--rw-r--r--   0        0        0    67097 2023-06-21 10:13:04.407405 serialtools-0.1.0/docs/build/html/serialtools.database.html
--rw-r--r--   0        0        0    33114 2023-06-21 10:13:04.444072 serialtools-0.1.0/docs/build/html/serialtools.database_config.html
--rw-r--r--   0        0        0    30404 2023-06-21 10:13:04.250740 serialtools-0.1.0/docs/build/html/serialtools.html
--rw-r--r--   0        0        0      804 2023-06-21 09:42:30.000914 serialtools-0.1.0/docs/make.bat
--rw-r--r--   0        0        0       46 2023-06-21 09:42:30.000914 serialtools-0.1.0/docs/source/_static/no-ligatures-in-code.css
--rw-r--r--   0        0        0      117 2023-06-21 09:42:30.000914 serialtools-0.1.0/docs/source/_static/tab-size.css
--rw-r--r--   0        0        0     3095 2023-06-21 10:13:02.320755 serialtools-0.1.0/docs/source/conf.py
--rw-r--r--   0        0        0      985 2023-06-21 10:13:02.337421 serialtools-0.1.0/docs/source/index.rst
--rw-r--r--   0        0        0       70 2023-06-21 10:13:02.270755 serialtools-0.1.0/docs/source/modules.rst
--rw-r--r--   0        0        0      157 2023-06-21 10:13:02.270755 serialtools-0.1.0/docs/source/serialtools.apps.decode.rst
--rw-r--r--   0        0        0      151 2023-06-21 10:13:02.274088 serialtools-0.1.0/docs/source/serialtools.apps.dump.rst
--rw-r--r--   0        0        0      302 2023-06-21 10:13:02.270755 serialtools-0.1.0/docs/source/serialtools.apps.rst
--rw-r--r--   0        0        0      151 2023-06-21 10:13:02.270755 serialtools-0.1.0/docs/source/serialtools.apps.send.rst
--rw-r--r--   0        0        0      133 2023-06-21 10:13:02.274088 serialtools-0.1.0/docs/source/serialtools.bus.rst
--rw-r--r--   0        0        0      148 2023-06-21 10:13:02.274088 serialtools-0.1.0/docs/source/serialtools.database.rst
--rw-r--r--   0        0        0      171 2023-06-21 10:13:02.270755 serialtools-0.1.0/docs/source/serialtools.database_config.rst
--rw-r--r--   0        0        0      360 2023-06-21 10:13:02.270755 serialtools-0.1.0/docs/source/serialtools.rst
--rw-r--r--   0        0        0      170 2023-06-21 09:42:30.000914 serialtools-0.1.0/mypy.ini
--rw-r--r--   0        0        0     4135 2023-06-21 09:42:30.000914 serialtools-0.1.0/prepare_for_gitlab_pages.py
--rw-r--r--   0        0        0      726 2023-06-21 10:28:31.193820 serialtools-0.1.0/pyproject.toml
--rwxr-xr-x   0        0        0    12230 2023-06-21 10:10:06.092119 serialtools-0.1.0/release.sh
--rw-r--r--   0        0        0       83 2023-06-21 09:42:30.000914 serialtools-0.1.0/requirements-release.txt
--rw-r--r--   0        0        0       22 2023-06-21 09:42:30.000914 serialtools-0.1.0/requirements-test.txt
--rw-r--r--   0        0        0       87 2023-06-21 10:18:12.678404 serialtools-0.1.0/src/serialtools/__init__.py
--rw-r--r--   0        0        0     1348 2023-06-21 10:13:02.267422 serialtools-0.1.0/src/serialtools/__main__.py
--rw-r--r--   0        0        0      289 2023-06-21 10:13:02.267422 serialtools-0.1.0/src/serialtools/apps/__init__.py
--rw-r--r--   0        0        0     1143 2023-06-21 10:13:02.270755 serialtools-0.1.0/src/serialtools/apps/decode.py
--rw-r--r--   0        0        0     1346 2023-06-21 10:13:02.267422 serialtools-0.1.0/src/serialtools/apps/dump.py
--rw-r--r--   0        0        0      880 2023-06-21 10:13:02.270755 serialtools-0.1.0/src/serialtools/apps/send.py
--rw-r--r--   0        0        0     5636 2023-06-21 10:13:02.267422 serialtools-0.1.0/src/serialtools/bus.py
--rw-r--r--   0        0        0    12580 2023-06-21 10:13:02.267422 serialtools-0.1.0/src/serialtools/database.py
--rw-r--r--   0        0        0     5027 2023-06-21 10:13:02.267422 serialtools-0.1.0/src/serialtools/database_config.py
--rw-r--r--   0        0        0        0 2022-11-03 16:33:53.710006 serialtools-0.1.0/src/serialtools/py.typed
--rw-r--r--   0        0        0      336 2023-06-21 09:42:30.000914 serialtools-0.1.0/tox.ini
--rw-r--r--   0        0        0     1086 1970-01-01 00:00:00.000000 serialtools-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      330 2023-06-02 06:55:40.811546 serialtools-0.2.0/.gitignore
+-rw-r--r--   0        0        0      119 2023-06-21 10:33:17.761717 serialtools-0.2.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      657 2023-06-21 08:53:39.687960 serialtools-0.2.0/LICENSE
+-rw-r--r--   0        0        0      444 2023-06-21 10:33:17.761717 serialtools-0.2.0/README.md
+-rw-r--r--   0        0        0      638 2023-06-21 10:33:17.761717 serialtools-0.2.0/docs/Makefile
+-rw-r--r--   0        0        0      985 2023-06-21 10:33:17.761717 serialtools-0.2.0/docs/build/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0       70 2023-06-21 10:33:17.761717 serialtools-0.2.0/docs/build/html/_sources/modules.rst.txt
+-rw-r--r--   0        0        0      157 2023-06-21 10:33:17.761717 serialtools-0.2.0/docs/build/html/_sources/serialtools.apps.decode.rst.txt
+-rw-r--r--   0        0        0      151 2023-06-21 10:33:17.761717 serialtools-0.2.0/docs/build/html/_sources/serialtools.apps.dump.rst.txt
+-rw-r--r--   0        0        0      302 2023-06-21 10:33:17.761717 serialtools-0.2.0/docs/build/html/_sources/serialtools.apps.rst.txt
+-rw-r--r--   0        0        0      151 2023-06-21 10:33:17.761717 serialtools-0.2.0/docs/build/html/_sources/serialtools.apps.send.rst.txt
+-rw-r--r--   0        0        0      133 2023-06-21 10:33:17.761717 serialtools-0.2.0/docs/build/html/_sources/serialtools.bus.rst.txt
+-rw-r--r--   0        0        0      148 2023-06-21 10:33:17.761717 serialtools-0.2.0/docs/build/html/_sources/serialtools.database.rst.txt
+-rw-r--r--   0        0        0      171 2023-06-21 10:33:17.761717 serialtools-0.2.0/docs/build/html/_sources/serialtools.database_config.rst.txt
+-rw-r--r--   0        0        0      360 2023-06-21 10:33:17.765050 serialtools-0.2.0/docs/build/html/_sources/serialtools.rst.txt
+-rw-r--r--   0        0        0     4289 2023-06-21 14:16:03.162360 serialtools-0.2.0/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0        0        0    14813 2023-06-21 14:16:04.459018 serialtools-0.2.0/docs/build/html/_static/basic.css
+-rw-r--r--   0        0        0     3229 2023-06-21 10:33:17.765050 serialtools-0.2.0/docs/build/html/_static/css/badge_only.css
+-rw-r--r--   0        0        0    87624 2023-06-21 10:33:17.765050 serialtools-0.2.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0        0        0    67312 2023-06-21 10:33:17.765050 serialtools-0.2.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0        0        0    86288 2023-06-21 10:33:17.765050 serialtools-0.2.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0        0        0    66444 2023-06-21 10:33:17.765050 serialtools-0.2.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0        0        0   165742 2023-06-21 10:33:17.765050 serialtools-0.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   444379 2023-06-21 10:33:17.768383 serialtools-0.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2023-06-21 10:33:17.771717 serialtools-0.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2023-06-21 10:33:17.771717 serialtools-0.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2023-06-21 10:33:17.771717 serialtools-0.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0   323344 2023-06-21 10:33:17.771717 serialtools-0.2.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0        0        0   193308 2023-06-21 10:33:17.775050 serialtools-0.2.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0        0        0   309728 2023-06-21 10:33:17.775050 serialtools-0.2.0/docs/build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0        0        0   184912 2023-06-21 10:33:17.775050 serialtools-0.2.0/docs/build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0        0        0   328412 2023-06-21 10:33:17.778383 serialtools-0.2.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0        0        0   195704 2023-06-21 10:33:17.778383 serialtools-0.2.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0        0        0   309192 2023-06-21 10:33:17.778383 serialtools-0.2.0/docs/build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0        0        0   182708 2023-06-21 10:33:17.778383 serialtools-0.2.0/docs/build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0        0        0   135314 2023-06-21 10:33:17.781717 serialtools-0.2.0/docs/build/html/_static/css/theme.css
+-rw-r--r--   0        0        0     4472 2023-06-21 10:33:17.781717 serialtools-0.2.0/docs/build/html/_static/doctools.js
+-rw-r--r--   0        0        0      421 2023-06-21 14:17:46.944972 serialtools-0.2.0/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2023-06-21 10:33:17.781717 serialtools-0.2.0/docs/build/html/_static/file.png
+-rw-r--r--   0        0        0    89501 2023-06-21 14:16:03.162360 serialtools-0.2.0/docs/build/html/_static/jquery.js
+-rw-r--r--   0        0        0      934 2023-06-21 10:33:17.781717 serialtools-0.2.0/docs/build/html/_static/js/badge_only.js
+-rw-r--r--   0        0        0     4370 2023-06-21 10:33:17.781717 serialtools-0.2.0/docs/build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0        0        0     2734 2023-06-21 10:33:17.781717 serialtools-0.2.0/docs/build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0        0        0     5023 2023-06-21 10:33:17.781717 serialtools-0.2.0/docs/build/html/_static/js/theme.js
+-rw-r--r--   0        0        0     4758 2023-06-21 14:16:04.462351 serialtools-0.2.0/docs/build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2023-06-21 10:33:17.781717 serialtools-0.2.0/docs/build/html/_static/minus.png
+-rw-r--r--   0        0        0       46 2023-06-21 10:33:17.781717 serialtools-0.2.0/docs/build/html/_static/no-ligatures-in-code.css
+-rw-r--r--   0        0        0       90 2023-06-21 10:33:17.781717 serialtools-0.2.0/docs/build/html/_static/plus.png
+-rw-r--r--   0        0        0     4819 2023-06-21 14:16:04.455685 serialtools-0.2.0/docs/build/html/_static/pygments.css
+-rw-r--r--   0        0        0    18215 2023-06-21 10:33:17.781717 serialtools-0.2.0/docs/build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     4712 2023-06-21 10:33:17.781717 serialtools-0.2.0/docs/build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0      204 2023-06-21 10:33:17.781717 serialtools-0.2.0/docs/build/html/_static/sphinx_paramlinks.css
+-rw-r--r--   0        0        0      117 2023-06-21 10:33:17.781717 serialtools-0.2.0/docs/build/html/_static/tab-size.css
+-rw-r--r--   0        0        0    26556 2023-06-21 14:17:46.944972 serialtools-0.2.0/docs/build/html/genindex.html
+-rw-r--r--   0        0        0    14126 2023-06-21 14:17:46.944972 serialtools-0.2.0/docs/build/html/index.html
+-rw-r--r--   0        0        0    10059 2023-06-21 14:17:46.944972 serialtools-0.2.0/docs/build/html/modules.html
+-rw-r--r--   0        0        0     1253 2023-06-21 14:17:46.944972 serialtools-0.2.0/docs/build/html/objects.inv
+-rw-r--r--   0        0        0     6583 2023-06-21 14:17:46.944972 serialtools-0.2.0/docs/build/html/py-modindex.html
+-rw-r--r--   0        0        0     4797 2023-06-21 14:17:46.944972 serialtools-0.2.0/docs/build/html/search.html
+-rw-r--r--   0        0        0    22432 2023-06-21 14:17:46.944972 serialtools-0.2.0/docs/build/html/searchindex.js
+-rw-r--r--   0        0        0    14594 2023-06-21 14:17:46.944972 serialtools-0.2.0/docs/build/html/serialtools.apps.decode.html
+-rw-r--r--   0        0        0    12182 2023-06-21 14:17:46.948305 serialtools-0.2.0/docs/build/html/serialtools.apps.dump.html
+-rw-r--r--   0        0        0    10486 2023-06-21 14:17:46.948305 serialtools-0.2.0/docs/build/html/serialtools.apps.html
+-rw-r--r--   0        0        0    10684 2023-06-21 14:17:46.948305 serialtools-0.2.0/docs/build/html/serialtools.apps.send.html
+-rw-r--r--   0        0        0    44788 2023-06-21 14:17:46.948305 serialtools-0.2.0/docs/build/html/serialtools.bus.html
+-rw-r--r--   0        0        0    68246 2023-06-21 14:17:46.948305 serialtools-0.2.0/docs/build/html/serialtools.database.html
+-rw-r--r--   0        0        0    33114 2023-06-21 14:17:46.948305 serialtools-0.2.0/docs/build/html/serialtools.database_config.html
+-rw-r--r--   0        0        0    30858 2023-06-21 14:17:46.948305 serialtools-0.2.0/docs/build/html/serialtools.html
+-rw-r--r--   0        0        0      804 2023-06-21 10:33:17.785050 serialtools-0.2.0/docs/make.bat
+-rw-r--r--   0        0        0       46 2023-06-21 10:33:17.785050 serialtools-0.2.0/docs/source/_static/no-ligatures-in-code.css
+-rw-r--r--   0        0        0      117 2023-06-21 10:33:17.785050 serialtools-0.2.0/docs/source/_static/tab-size.css
+-rw-r--r--   0        0        0     3095 2023-06-21 14:17:46.948305 serialtools-0.2.0/docs/source/conf.py
+-rw-r--r--   0        0        0      985 2023-06-21 14:16:02.305699 serialtools-0.2.0/docs/source/index.rst
+-rw-r--r--   0        0        0       70 2023-06-21 14:16:02.239033 serialtools-0.2.0/docs/source/modules.rst
+-rw-r--r--   0        0        0      157 2023-06-21 14:16:02.239033 serialtools-0.2.0/docs/source/serialtools.apps.decode.rst
+-rw-r--r--   0        0        0      151 2023-06-21 14:16:02.239033 serialtools-0.2.0/docs/source/serialtools.apps.dump.rst
+-rw-r--r--   0        0        0      302 2023-06-21 14:16:02.239033 serialtools-0.2.0/docs/source/serialtools.apps.rst
+-rw-r--r--   0        0        0      151 2023-06-21 14:16:02.239033 serialtools-0.2.0/docs/source/serialtools.apps.send.rst
+-rw-r--r--   0        0        0      133 2023-06-21 14:16:02.239033 serialtools-0.2.0/docs/source/serialtools.bus.rst
+-rw-r--r--   0        0        0      148 2023-06-21 14:16:02.239033 serialtools-0.2.0/docs/source/serialtools.database.rst
+-rw-r--r--   0        0        0      171 2023-06-21 14:16:02.239033 serialtools-0.2.0/docs/source/serialtools.database_config.rst
+-rw-r--r--   0        0        0      360 2023-06-21 14:16:02.239033 serialtools-0.2.0/docs/source/serialtools.rst
+-rw-r--r--   0        0        0      170 2023-06-21 12:47:48.856235 serialtools-0.2.0/mypy.ini
+-rw-r--r--   0        0        0     4135 2023-06-21 10:33:17.785050 serialtools-0.2.0/prepare_for_gitlab_pages.py
+-rw-r--r--   0        0        0      786 2023-06-21 14:17:46.948305 serialtools-0.2.0/pyproject.toml
+-rwxr-xr-x   0        0        0    12230 2023-06-21 10:33:17.785050 serialtools-0.2.0/release.sh
+-rw-r--r--   0        0        0       83 2023-06-21 10:33:17.785050 serialtools-0.2.0/requirements-release.txt
+-rw-r--r--   0        0        0       22 2023-06-21 10:33:17.785050 serialtools-0.2.0/requirements-test.txt
+-rw-r--r--   0        0        0       87 2023-06-21 14:17:46.948305 serialtools-0.2.0/src/serialtools/__init__.py
+-rw-r--r--   0        0        0     1448 2023-06-21 14:17:46.948305 serialtools-0.2.0/src/serialtools/__main__.py
+-rw-r--r--   0        0        0      289 2023-06-21 14:16:02.235700 serialtools-0.2.0/src/serialtools/apps/__init__.py
+-rw-r--r--   0        0        0     1143 2023-06-21 14:16:02.239033 serialtools-0.2.0/src/serialtools/apps/decode.py
+-rw-r--r--   0        0        0     1346 2023-06-21 14:16:02.235700 serialtools-0.2.0/src/serialtools/apps/dump.py
+-rw-r--r--   0        0        0      880 2023-06-21 14:16:02.239033 serialtools-0.2.0/src/serialtools/apps/send.py
+-rw-r--r--   0        0        0     6066 2023-06-21 14:17:46.948305 serialtools-0.2.0/src/serialtools/bus.py
+-rw-r--r--   0        0        0    13062 2023-06-21 14:17:46.948305 serialtools-0.2.0/src/serialtools/database.py
+-rw-r--r--   0        0        0     5027 2023-06-21 14:16:02.232366 serialtools-0.2.0/src/serialtools/database_config.py
+-rw-r--r--   0        0        0        0 2022-11-03 16:33:53.710006 serialtools-0.2.0/src/serialtools/py.typed
+-rw-r--r--   0        0        0      336 2023-06-21 12:47:48.856235 serialtools-0.2.0/tox.ini
+-rw-r--r--   0        0        0     1156 1970-01-01 00:00:00.000000 serialtools-0.2.0/PKG-INFO
```

### Comparing `serialtools-0.1.0/LICENSE` & `serialtools-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/Makefile` & `serialtools-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/build/html/_sources/index.rst.txt` & `serialtools-0.2.0/docs/build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js` & `serialtools-0.2.0/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/build/html/_static/basic.css` & `serialtools-0.2.0/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/build/html/_static/css/badge_only.css` & `serialtools-0.2.0/docs/build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `serialtools-0.2.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `serialtools-0.2.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `serialtools-0.2.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `serialtools-0.2.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/build/html/_static/css/fonts/fontawesome-webfont.eot` & `serialtools-0.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg` & `serialtools-0.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf` & `serialtools-0.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff` & `serialtools-0.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2` & `serialtools-0.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff` & `serialtools-0.2.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff2` & `serialtools-0.2.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/build/html/_static/css/fonts/lato-bold.woff` & `serialtools-0.2.0/docs/build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/build/html/_static/css/fonts/lato-bold.woff2` & `serialtools-0.2.0/docs/build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff` & `serialtools-0.2.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff2` & `serialtools-0.2.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/build/html/_static/css/fonts/lato-normal.woff` & `serialtools-0.2.0/docs/build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/build/html/_static/css/fonts/lato-normal.woff2` & `serialtools-0.2.0/docs/build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/build/html/_static/css/theme.css` & `serialtools-0.2.0/docs/build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/build/html/_static/doctools.js` & `serialtools-0.2.0/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/build/html/_static/jquery.js` & `serialtools-0.2.0/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/build/html/_static/js/badge_only.js` & `serialtools-0.2.0/docs/build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/build/html/_static/js/html5shiv-printshiv.min.js` & `serialtools-0.2.0/docs/build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/build/html/_static/js/html5shiv.min.js` & `serialtools-0.2.0/docs/build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/build/html/_static/js/theme.js` & `serialtools-0.2.0/docs/build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/build/html/_static/language_data.js` & `serialtools-0.2.0/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/build/html/_static/pygments.css` & `serialtools-0.2.0/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/build/html/_static/searchtools.js` & `serialtools-0.2.0/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/build/html/_static/sphinx_highlight.js` & `serialtools-0.2.0/docs/build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/build/html/genindex.html` & `serialtools-0.2.0/docs/build/html/genindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Index &mdash; serialtools v0.1.0 documentation</title>
+  <title>Index &mdash; serialtools v0.2.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -31,15 +31,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.1.0
+                v0.2.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -165,14 +165,16 @@
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="serialtools.bus.html#serialtools.bus.ReadFromFileBus.close">close() (serialtools.bus.ReadFromFileBus method)</a>
 
       <ul>
         <li><a href="serialtools.bus.html#serialtools.bus.WriteToFileBus.close">(serialtools.bus.WriteToFileBus method)</a>
 </li>
       </ul></li>
+      <li><a href="serialtools.bus.html#serialtools.bus.BusCreator.create_args">create_args() (serialtools.bus.BusCreator method)</a>
+</li>
       <li><a href="serialtools.bus.html#serialtools.bus.BusCreator.create_bus">create_bus() (serialtools.bus.BusCreator method)</a>
 </li>
   </ul></td>
 </tr></table>
 
 <h2 id="D">D</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
@@ -410,14 +412,16 @@
 </tr></table>
 
 <h2 id="S">S</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="serialtools.apps.send.html#serialtools.apps.send.send">send() (in module serialtools.apps.send)</a>
 </li>
+      <li><a href="serialtools.database.html#serialtools.database.Reader.send_msg">send_msg() (serialtools.database.Reader method)</a>
+</li>
       <li>
     serialtools
 
       <ul>
         <li><a href="serialtools.html#module-serialtools">module</a>
 </li>
       </ul></li>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 
 serialtools
-v0.1.0
+v0.2.0
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
     * serialtools.apps.send_module
     * serialtools.bus_module
     * serialtools.database_module
@@ -34,23 +34,23 @@
       attribute)                           * bytesize_
     * BIG_                                   (serialtools.bus.BusCreator
       (serialtools.database.Endianness       attribute)
       attribute)                           * ByteSpec_(class_in
     * BOOL_(serialtools.database.Type        serialtools.database)
       attribute)
 ***** C *****
-    * cancel_read()_
-      (serialtools.bus.ReadFromFileBus          * close()_
-      method)                                     (serialtools.bus.ReadFromFileBus
-          o (serialtools.bus.WriteToFileBus       method)
-            method)                                   o (serialtools.bus.WriteToFileBus
-    * cancel_write()_                                   method)
-      (serialtools.bus.ReadFromFileBus          * create_bus()_
-      method)                                     (serialtools.bus.BusCreator_method)
-          o (serialtools.bus.WriteToFileBus
+    * cancel_read()_                            * close()_
+      (serialtools.bus.ReadFromFileBus            (serialtools.bus.ReadFromFileBus
+      method)                                     method)
+          o (serialtools.bus.WriteToFileBus           o (serialtools.bus.WriteToFileBus
+            method)                                     method)
+    * cancel_write()_                           * create_args()_
+      (serialtools.bus.ReadFromFileBus            (serialtools.bus.BusCreator_method)
+      method)                                   * create_bus()_
+          o (serialtools.bus.WriteToFileBus       (serialtools.bus.BusCreator_method)
             method)
 ***** D *****
     * Database_(class_in                       * defined_parameters_
       serialtools.database)                      (serialtools.database_config.Param
     * DatabaseCreator_(class_in                  attribute)
       serialtools.database_config)             * dsrdtr_(serialtools.bus.BusCreator
     * decode()_(in_module                        attribute)
@@ -141,31 +141,31 @@
     * read_in_other_thread()_                     method)
       (serialtools.database.Reader_method)            o (serialtools.database_config.Param
     * read_msg()_                                       method)
       (serialtools.database.Reader_method)            o (serialtools.database_config.Signal
     * read_n_bytes()_                                   method)
       (serialtools.database.Reader_method)
 ***** S *****
-                                  * serialtools.bus
-                                        o module
-    * send()_(in_module           * serialtools.database
-      serialtools.apps.send)            o module
-    * serialtools                 * serialtools.database_config
-          o module                      o module
-    * serialtools.apps            * Signal_(class_in_serialtools.database)
-          o module                      o (class_in
-    * serialtools.apps.decode             serialtools.database_config)
-          o module                * signals_(serialtools.database.Database
-    * serialtools.apps.dump         attribute)
-          o module                      o (serialtools.database_config.Signal
-    * serialtools.apps.send               attribute)
-          o module                * stop()_(serialtools.database.Reader
-                                    method)
-                                  * stopbits_(serialtools.bus.BusCreator
-                                    attribute)
+                                       * serialtools.bus
+    * send()_(in_module                      o module
+      serialtools.apps.send)           * serialtools.database
+    * send_msg()_                            o module
+      (serialtools.database.Reader     * serialtools.database_config
+      method)                                o module
+    * serialtools                      * Signal_(class_in_serialtools.database)
+          o module                           o (class_in
+    * serialtools.apps                         serialtools.database_config)
+          o module                     * signals_(serialtools.database.Database
+    * serialtools.apps.decode            attribute)
+          o module                           o (serialtools.database_config.Signal
+    * serialtools.apps.dump                    attribute)
+          o module                     * stop()_(serialtools.database.Reader
+    * serialtools.apps.send              method)
+          o module                     * stopbits_(serialtools.bus.BusCreator
+                                         attribute)
 ***** T *****
     * TEXT_(serialtools.database.Type
       attribute)
     * timestamp_                                * Type_(class_in
       (serialtools.bus.ReadFromFileBus            serialtools.database)
       attribute)
           o (serialtools.bus.WriteToFileBus
```

### Comparing `serialtools-0.1.0/docs/build/html/index.html` & `serialtools-0.2.0/docs/build/html/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Welcome to serialtools’ documentation! &mdash; serialtools v0.1.0 documentation</title>
+  <title>Welcome to serialtools’ documentation! &mdash; serialtools v0.2.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -33,15 +33,15 @@
 
           
           
           <a href="#" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.1.0
+                v0.2.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 
 
 
 
 
 
 serialtools
-v0.1.0
+v0.2.0
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
     * serialtools.apps.send_module
     * serialtools.bus_module
     * serialtools.database_module
```

### Comparing `serialtools-0.1.0/docs/build/html/modules.html` & `serialtools-0.2.0/docs/build/html/modules.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools &mdash; serialtools v0.1.0 documentation</title>
+  <title>serialtools &mdash; serialtools v0.2.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -32,15 +32,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.1.0
+                v0.2.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 
 serialtools
-v0.1.0
+v0.2.0
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
     * serialtools.apps.send_module
     * serialtools.bus_module
     * serialtools.database_module
```

### Comparing `serialtools-0.1.0/docs/build/html/py-modindex.html` & `serialtools-0.2.0/docs/build/html/py-modindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Python Module Index &mdash; serialtools v0.1.0 documentation</title>
+  <title>Python Module Index &mdash; serialtools v0.2.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.1.0
+                v0.2.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 
 serialtools
-v0.1.0
+v0.2.0
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
     * serialtools.apps.send_module
     * serialtools.bus_module
     * serialtools.database_module
```

### Comparing `serialtools-0.1.0/docs/build/html/search.html` & `serialtools-0.2.0/docs/build/html/search.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Search &mdash; serialtools v0.1.0 documentation</title>
+  <title>Search &mdash; serialtools v0.2.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
     
   <!--[if lt IE 9]>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.1.0
+                v0.2.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="#" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 
 serialtools
-v0.1.0
+v0.2.0
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
     * serialtools.apps.send_module
     * serialtools.bus_module
     * serialtools.database_module
```

### Comparing `serialtools-0.1.0/docs/build/html/searchindex.js` & `serialtools-0.2.0/docs/build/html/searchindex.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -99,15 +99,15 @@
         "subpars": [4, 5, 6],
         "argpars": [4, 5, 6],
         "_subparsersact": [4, 5, 6],
         "ani": [4, 5, 6],
         "db": [4, 8, 9],
         "file": [4, 5, 7, 8, 9],
         "textio": [4, 5, 7],
-        "msg": [4, 6],
+        "msg": [4, 6, 8],
         "str": [4, 6, 7, 8, 9],
         "noreturn": 4,
         "arg": [4, 5, 6, 7, 9],
         "namespac": [4, 5, 6, 7, 9],
         "break_time_m": [5, 7],
         "100": 5,
         "class": [7, 8, 9],
@@ -243,15 +243,17 @@
         "bug": 0,
         "tracker": 0,
         "log": 0,
         "pypi": 0,
         "part": 8,
         "consist": 8,
         "itself": 8,
-        "possibl": 8
+        "possibl": 8,
+        "create_arg": [2, 7],
+        "send_msg": [2, 8]
     },
     "objects": {
         "": [
             [2, 0, 0, "-", "serialtools"]
         ],
         "serialtools": [
             [3, 0, 0, "-", "apps"],
@@ -289,14 +291,15 @@
             [7, 2, 1, "", "WriteToFileBus"],
             [7, 1, 1, "", "get_timestamp"]
         ],
         "serialtools.bus.BusCreator": [
             [7, 3, 1, "", "add_arguments"],
             [7, 4, 1, "", "baudrate"],
             [7, 4, 1, "", "bytesize"],
+            [7, 3, 1, "", "create_args"],
             [7, 3, 1, "", "create_bus"],
             [7, 4, 1, "", "dsrdtr"],
             [7, 4, 1, "", "parity"],
             [7, 4, 1, "", "port"],
             [7, 4, 1, "", "rtscts"],
             [7, 4, 1, "", "stopbits"],
             [7, 4, 1, "", "virtual"],
@@ -363,14 +366,15 @@
         "serialtools.database.Reader": [
             [8, 4, 1, "", "ignore_bytes_between_messages"],
             [8, 3, 1, "", "read"],
             [8, 3, 1, "", "read_byte"],
             [8, 3, 1, "", "read_in_other_thread"],
             [8, 3, 1, "", "read_msg"],
             [8, 3, 1, "", "read_n_bytes"],
+            [8, 3, 1, "", "send_msg"],
             [8, 3, 1, "", "stop"]
         ],
         "serialtools.database.Signal": [
             [8, 3, 1, "", "get_bitstruct_fmt"]
         ],
         "serialtools.database.Type": [
             [8, 4, 1, "", "BOOL"],
@@ -619,14 +623,17 @@
         ],
         "close() (serialtools.bus.readfromfilebus method)": [
             [7, "serialtools.bus.ReadFromFileBus.close"]
         ],
         "close() (serialtools.bus.writetofilebus method)": [
             [7, "serialtools.bus.WriteToFileBus.close"]
         ],
+        "create_args() (serialtools.bus.buscreator method)": [
+            [7, "serialtools.bus.BusCreator.create_args"]
+        ],
         "create_bus() (serialtools.bus.buscreator method)": [
             [7, "serialtools.bus.BusCreator.create_bus"]
         ],
         "dsrdtr (serialtools.bus.buscreator attribute)": [
             [7, "serialtools.bus.BusCreator.dsrdtr"]
         ],
         "get_timestamp() (in module serialtools.bus)": [
@@ -775,14 +782,17 @@
         ],
         "read_msg() (serialtools.database.reader method)": [
             [8, "serialtools.database.Reader.read_msg"]
         ],
         "read_n_bytes() (serialtools.database.reader method)": [
             [8, "serialtools.database.Reader.read_n_bytes"]
         ],
+        "send_msg() (serialtools.database.reader method)": [
+            [8, "serialtools.database.Reader.send_msg"]
+        ],
         "serialtools.database": [
             [8, "module-serialtools.database"]
         ],
         "signals (serialtools.database.database attribute)": [
             [8, "serialtools.database.Database.signals"]
         ],
         "stop() (serialtools.database.reader method)": [
```

### Comparing `serialtools-0.1.0/docs/build/html/serialtools.apps.decode.html` & `serialtools-0.2.0/docs/build/html/serialtools.apps.decode.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.apps.decode module &mdash; serialtools v0.1.0 documentation</title>
+  <title>serialtools.apps.decode module &mdash; serialtools v0.2.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.1.0
+                v0.2.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 
 
 serialtools
-v0.1.0
+v0.2.0
 [q                   ]
     * serialtools_package
           o Subpackages
                 # serialtools.apps_package
                       # Submodules
                       # Module_contents
           o Submodules
```

### Comparing `serialtools-0.1.0/docs/build/html/serialtools.apps.dump.html` & `serialtools-0.2.0/docs/build/html/serialtools.apps.dump.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.apps.dump module &mdash; serialtools v0.1.0 documentation</title>
+  <title>serialtools.apps.dump module &mdash; serialtools v0.2.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.1.0
+                v0.2.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 
 
 serialtools
-v0.1.0
+v0.2.0
 [q                   ]
     * serialtools_package
           o Subpackages
                 # serialtools.apps_package
                       # Submodules
                       # Module_contents
           o Submodules
```

### Comparing `serialtools-0.1.0/docs/build/html/serialtools.apps.html` & `serialtools-0.2.0/docs/build/html/serialtools.apps.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.apps package &mdash; serialtools v0.1.0 documentation</title>
+  <title>serialtools.apps package &mdash; serialtools v0.2.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.1.0
+                v0.2.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 
 
 serialtools
-v0.1.0
+v0.2.0
 [q                   ]
     * serialtools_package
           o Subpackages
                 # serialtools.apps_package
                       # Submodules
                       # Module_contents
           o Submodules
```

### Comparing `serialtools-0.1.0/docs/build/html/serialtools.apps.send.html` & `serialtools-0.2.0/docs/build/html/serialtools.apps.send.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.apps.send module &mdash; serialtools v0.1.0 documentation</title>
+  <title>serialtools.apps.send module &mdash; serialtools v0.2.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.1.0
+                v0.2.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 
 
 serialtools
-v0.1.0
+v0.2.0
 [q                   ]
     * serialtools_package
           o Subpackages
                 # serialtools.apps_package
                       # Submodules
                       # Module_contents
           o Submodules
```

### Comparing `serialtools-0.1.0/docs/build/html/serialtools.bus.html` & `serialtools-0.2.0/docs/build/html/serialtools.bus.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.bus module &mdash; serialtools v0.1.0 documentation</title>
+  <title>serialtools.bus module &mdash; serialtools v0.2.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.1.0
+                v0.2.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -71,14 +71,15 @@
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.dump.html">serialtools.apps.dump module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.send.html">serialtools.apps.send module</a></li>
 <li class="toctree-l1 current"><a class="current reference internal" href="#">serialtools.bus module</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.bus.BusCreator"><code class="docutils literal notranslate"><span class="pre">BusCreator</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.BusCreator.add_arguments"><code class="docutils literal notranslate"><span class="pre">BusCreator.add_arguments()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.BusCreator.baudrate"><code class="docutils literal notranslate"><span class="pre">BusCreator.baudrate</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.BusCreator.bytesize"><code class="docutils literal notranslate"><span class="pre">BusCreator.bytesize</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.BusCreator.create_args"><code class="docutils literal notranslate"><span class="pre">BusCreator.create_args()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.BusCreator.create_bus"><code class="docutils literal notranslate"><span class="pre">BusCreator.create_bus()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.BusCreator.dsrdtr"><code class="docutils literal notranslate"><span class="pre">BusCreator.dsrdtr</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.BusCreator.parity"><code class="docutils literal notranslate"><span class="pre">BusCreator.parity</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.BusCreator.port"><code class="docutils literal notranslate"><span class="pre">BusCreator.port</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.BusCreator.rtscts"><code class="docutils literal notranslate"><span class="pre">BusCreator.rtscts</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.BusCreator.stopbits"><code class="docutils literal notranslate"><span class="pre">BusCreator.stopbits</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.BusCreator.virtual"><code class="docutils literal notranslate"><span class="pre">BusCreator.virtual</span></code></a></li>
@@ -161,14 +162,19 @@
 <span class="sig-name descname"><span class="pre">bytesize</span></span><a class="headerlink" href="#serialtools.bus.BusCreator.bytesize" title="Permalink to this definition"></a></dt>
 <dd><p>Each instance of this class represents a setting which can be changed in a config file.</p>
 <p>This class implements the <a class="reference external" href="https://docs.python.org/3/reference/datamodel.html#implementing-descriptors">descriptor protocol</a> to return <code class="xref py py-attr docutils literal notranslate"><span class="pre">value</span></code> if an instance of this class is accessed as an instance attribute.
 If you want to get this object you need to access it as a class attribute.</p>
 </dd></dl>
 
 <dl class="py method">
+<dt class="sig sig-object py" id="serialtools.bus.BusCreator.create_args">
+<span class="sig-name descname"><span class="pre">create_args</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="o"><span class="pre">*</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">port</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">baudrate</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">virtual</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><span class="pre">bool</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/argparse.html#argparse.Namespace" title="(in Python v3.11)"><span class="pre">Namespace</span></a></span></span><a class="headerlink" href="#serialtools.bus.BusCreator.create_args" title="Permalink to this definition"></a></dt>
+<dd></dd></dl>
+
+<dl class="py method">
 <dt class="sig sig-object py" id="serialtools.bus.BusCreator.create_bus">
 <span class="sig-name descname"><span class="pre">create_bus</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">args</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/argparse.html#argparse.Namespace" title="(in Python v3.11)"><span class="pre">Namespace</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Serial</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference internal" href="#serialtools.bus.ReadFromFileBus" title="serialtools.bus.ReadFromFileBus"><span class="pre">ReadFromFileBus</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference internal" href="#serialtools.bus.WriteToFileBus" title="serialtools.bus.WriteToFileBus"><span class="pre">WriteToFileBus</span></a></span></span><a class="headerlink" href="#serialtools.bus.BusCreator.create_bus" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="serialtools.bus.BusCreator.dsrdtr">
 <span class="sig-name descname"><span class="pre">dsrdtr</span></span><a class="headerlink" href="#serialtools.bus.BusCreator.dsrdtr" title="Permalink to this definition"></a></dt>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 
 
 serialtools
-v0.1.0
+v0.2.0
 [q                   ]
     * serialtools_package
           o Subpackages
           o Submodules
                 # serialtools.bus_module
                       # BusCreator
                       # ReadFromFileBus
@@ -27,14 +27,15 @@
     * serialtools.apps.dump_module
     * serialtools.apps.send_module
     * serialtools.bus_module
           o BusCreator
                 # BusCreator.add_arguments()
                 # BusCreator.baudrate
                 # BusCreator.bytesize
+                # BusCreator.create_args()
                 # BusCreator.create_bus()
                 # BusCreator.dsrdtr
                 # BusCreator.parity
                 # BusCreator.port
                 # BusCreator.rtscts
                 # BusCreator.stopbits
                 # BusCreator.virtual
@@ -76,14 +77,16 @@
             want to get this object you need to access it as a class attribute.
         bytesizeï
             Each instance of this class represents a setting which can be
             changed in a config file.
             This class implements the descriptor_protocol to return value if an
             instance of this class is accessed as an instance attribute. If you
             want to get this object you need to access it as a class attribute.
+        create_args(*, port: str | None = None, baudrate: int | None = None,
+        virtual: bool | None = None) &#x2192; Namespaceï
         create_bus(args: Namespace) &#x2192; Serial | ReadFromFileBus |
         WriteToFileBusï
         dsrdtrï
             Each instance of this class represents a setting which can be
             changed in a config file.
             This class implements the descriptor_protocol to return value if an
             instance of this class is accessed as an instance attribute. If you
```

### Comparing `serialtools-0.1.0/docs/build/html/serialtools.database.html` & `serialtools-0.2.0/docs/build/html/serialtools.database.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.database module &mdash; serialtools v0.1.0 documentation</title>
+  <title>serialtools.database module &mdash; serialtools v0.2.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.1.0
+                v0.2.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -107,14 +107,15 @@
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.database.Reader"><code class="docutils literal notranslate"><span class="pre">Reader</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Reader.ignore_bytes_between_messages"><code class="docutils literal notranslate"><span class="pre">Reader.ignore_bytes_between_messages</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Reader.read"><code class="docutils literal notranslate"><span class="pre">Reader.read()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Reader.read_byte"><code class="docutils literal notranslate"><span class="pre">Reader.read_byte()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Reader.read_in_other_thread"><code class="docutils literal notranslate"><span class="pre">Reader.read_in_other_thread()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Reader.read_msg"><code class="docutils literal notranslate"><span class="pre">Reader.read_msg()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Reader.read_n_bytes"><code class="docutils literal notranslate"><span class="pre">Reader.read_n_bytes()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Reader.send_msg"><code class="docutils literal notranslate"><span class="pre">Reader.send_msg()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Reader.stop"><code class="docutils literal notranslate"><span class="pre">Reader.stop()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.database.Signal"><code class="docutils literal notranslate"><span class="pre">Signal</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Signal.get_bitstruct_fmt"><code class="docutils literal notranslate"><span class="pre">Signal.get_bitstruct_fmt()</span></code></a></li>
 </ul>
 </li>
@@ -312,14 +313,19 @@
 
 <dl class="py method">
 <dt class="sig sig-object py" id="serialtools.database.Reader.read_n_bytes">
 <span class="sig-name descname"><span class="pre">read_n_bytes</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">n</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.11)"><span class="pre">bytes</span></a></span></span><a class="headerlink" href="#serialtools.database.Reader.read_n_bytes" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 <dl class="py method">
+<dt class="sig sig-object py" id="serialtools.database.Reader.send_msg">
+<span class="sig-name descname"><span class="pre">send_msg</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">msg</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#serialtools.database.Message" title="serialtools.database.Message"><span class="pre">Message</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#serialtools.database.Reader.send_msg" title="Permalink to this definition"></a></dt>
+<dd></dd></dl>
+
+<dl class="py method">
 <dt class="sig sig-object py" id="serialtools.database.Reader.stop">
 <span class="sig-name descname"><span class="pre">stop</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#serialtools.database.Reader.stop" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 
 
 serialtools
-v0.1.0
+v0.2.0
 [q                   ]
     * serialtools_package
           o Subpackages
           o Submodules
                 # serialtools.bus_module
                 # serialtools.database_module
                       # ByteSpec
@@ -55,14 +55,15 @@
           o Reader
                 # Reader.ignore_bytes_between_messages
                 # Reader.read()
                 # Reader.read_byte()
                 # Reader.read_in_other_thread()
                 # Reader.read_msg()
                 # Reader.read_n_bytes()
+                # Reader.send_msg()
                 # Reader.stop()
           o Signal
                 # Signal.get_bitstruct_fmt()
           o Type
                 # Type.BOOL
                 # Type.FLOAT
                 # Type.INT
@@ -128,14 +129,15 @@
             want to get this object you need to access it as a class attribute.
         read() &#x2192; Iterator[Message]ï
         read_byte() &#x2192; intï
         read_in_other_thread(callback: Callable[[Message], None]) &#x2192;
         Noneï
         read_msg() &#x2192; Message | Noneï
         read_n_bytes(n: int) &#x2192; bytesï
+        send_msg(msg: Message) &#x2192; Noneï
         stop() &#x2192; Noneï
   classserialtools.database.Signal(name: str, type: Type, address: int, *,
   bits: int | None = None, startbit: int = 0, scale: float = 1, offset: float =
   0, unit: str = '')ï
       Bases: object
         Paramref name:
             The name of the signal
```

### Comparing `serialtools-0.1.0/docs/build/html/serialtools.database_config.html` & `serialtools-0.2.0/docs/build/html/serialtools.database_config.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.database_config module &mdash; serialtools v0.1.0 documentation</title>
+  <title>serialtools.database_config module &mdash; serialtools v0.2.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -33,15 +33,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.1.0
+                v0.2.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 
 
 
 
 
 
 serialtools
-v0.1.0
+v0.2.0
 [q                   ]
     * serialtools_package
           o Subpackages
           o Submodules
                 # serialtools.bus_module
                 # serialtools.database_module
                 # serialtools.database_config_module
```

### Comparing `serialtools-0.1.0/docs/build/html/serialtools.html` & `serialtools-0.2.0/docs/build/html/serialtools.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools package &mdash; serialtools v0.1.0 documentation</title>
+  <title>serialtools package &mdash; serialtools v0.2.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.1.0
+                v0.2.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -139,14 +139,15 @@
 <div class="toctree-wrapper compound">
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.bus.html">serialtools.bus module</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.BusCreator"><code class="docutils literal notranslate"><span class="pre">BusCreator</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.BusCreator.add_arguments"><code class="docutils literal notranslate"><span class="pre">BusCreator.add_arguments()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.BusCreator.baudrate"><code class="docutils literal notranslate"><span class="pre">BusCreator.baudrate</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.BusCreator.bytesize"><code class="docutils literal notranslate"><span class="pre">BusCreator.bytesize</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.BusCreator.create_args"><code class="docutils literal notranslate"><span class="pre">BusCreator.create_args()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.BusCreator.create_bus"><code class="docutils literal notranslate"><span class="pre">BusCreator.create_bus()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.BusCreator.dsrdtr"><code class="docutils literal notranslate"><span class="pre">BusCreator.dsrdtr</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.BusCreator.parity"><code class="docutils literal notranslate"><span class="pre">BusCreator.parity</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.BusCreator.port"><code class="docutils literal notranslate"><span class="pre">BusCreator.port</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.BusCreator.rtscts"><code class="docutils literal notranslate"><span class="pre">BusCreator.rtscts</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.BusCreator.stopbits"><code class="docutils literal notranslate"><span class="pre">BusCreator.stopbits</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.BusCreator.virtual"><code class="docutils literal notranslate"><span class="pre">BusCreator.virtual</span></code></a></li>
@@ -209,14 +210,15 @@
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database.html#serialtools.database.Reader"><code class="docutils literal notranslate"><span class="pre">Reader</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Reader.ignore_bytes_between_messages"><code class="docutils literal notranslate"><span class="pre">Reader.ignore_bytes_between_messages</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Reader.read"><code class="docutils literal notranslate"><span class="pre">Reader.read()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Reader.read_byte"><code class="docutils literal notranslate"><span class="pre">Reader.read_byte()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Reader.read_in_other_thread"><code class="docutils literal notranslate"><span class="pre">Reader.read_in_other_thread()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Reader.read_msg"><code class="docutils literal notranslate"><span class="pre">Reader.read_msg()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Reader.read_n_bytes"><code class="docutils literal notranslate"><span class="pre">Reader.read_n_bytes()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Reader.send_msg"><code class="docutils literal notranslate"><span class="pre">Reader.send_msg()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Reader.stop"><code class="docutils literal notranslate"><span class="pre">Reader.stop()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database.html#serialtools.database.Signal"><code class="docutils literal notranslate"><span class="pre">Signal</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Signal.get_bitstruct_fmt"><code class="docutils literal notranslate"><span class="pre">Signal.get_bitstruct_fmt()</span></code></a></li>
 </ul>
 </li>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 
 
 serialtools
-v0.1.0
+v0.2.0
 [q                   ]
     * serialtools_package
           o Subpackages
                 # serialtools.apps_package
           o Submodules
                 # serialtools.bus_module
                 # serialtools.database_module
@@ -52,14 +52,15 @@
 
 ***** Submodulesï *****
     * serialtools.bus_module
           o BusCreator
                 # BusCreator.add_arguments()
                 # BusCreator.baudrate
                 # BusCreator.bytesize
+                # BusCreator.create_args()
                 # BusCreator.create_bus()
                 # BusCreator.dsrdtr
                 # BusCreator.parity
                 # BusCreator.port
                 # BusCreator.rtscts
                 # BusCreator.stopbits
                 # BusCreator.virtual
@@ -106,14 +107,15 @@
           o Reader
                 # Reader.ignore_bytes_between_messages
                 # Reader.read()
                 # Reader.read_byte()
                 # Reader.read_in_other_thread()
                 # Reader.read_msg()
                 # Reader.read_n_bytes()
+                # Reader.send_msg()
                 # Reader.stop()
           o Signal
                 # Signal.get_bitstruct_fmt()
           o Type
                 # Type.BOOL
                 # Type.FLOAT
                 # Type.INT
```

### Comparing `serialtools-0.1.0/docs/make.bat` & `serialtools-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/docs/source/conf.py` & `serialtools-0.2.0/docs/source/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'serialtools'
 copyright = '2023, erzo'
 author = 'erzo'
-release = 'v0.1.0'
+release = 'v0.2.0'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['sphinx.ext.autodoc', 'sphinx.ext.intersphinx', 'sphinx_paramlinks']
 
 templates_path = ['_templates']
```

### Comparing `serialtools-0.1.0/docs/source/index.rst` & `serialtools-0.2.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/prepare_for_gitlab_pages.py` & `serialtools-0.2.0/prepare_for_gitlab_pages.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/pyproject.toml` & `serialtools-0.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -17,13 +17,14 @@
 	"Operating System :: POSIX",
 	"Operating System :: Unix",
 	"Environment :: Console",
 	"License :: OSI Approved :: BSD License",
 ]
 
 [project.urls]
+Documentation = "https://erzo.gitlab.io/serialtools/latest"
 "Source code" = "https://gitlab.com/erzo/serialtools"
 "Bug tracker" = "https://gitlab.com/erzo/serialtools/-/issues"
 "Change log" = "https://gitlab.com/erzo/serialtools/-/tags"
 
 [project.scripts]
 serialtools = "serialtools.__main__:main"
```

### Comparing `serialtools-0.1.0/release.sh` & `serialtools-0.2.0/release.sh`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/src/serialtools/__main__.py` & `serialtools-0.2.0/src/serialtools/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,19 @@
 
 	cf = ConfigFile(appname=APPNAME)
 	cf.set_ui_callback(lambda msg: print(msg, file=sys.stderr))
 	cf.load()
 	if args.config:
 		cf.load_file(os.path.abspath(os.path.expanduser(args.config)))
 
+	if not hasattr(args, 'func'):
+		print("missing command")
+		print()
+		parser.print_help()
+		exit(1)
 	args.func(args)
 
 
 def print_version_and_exit() -> None:
 	print(f"{APPNAME} {__version__}")
 	sys.exit(0)
```

### Comparing `serialtools-0.1.0/src/serialtools/apps/decode.py` & `serialtools-0.2.0/src/serialtools/apps/decode.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/src/serialtools/apps/dump.py` & `serialtools-0.2.0/src/serialtools/apps/dump.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/src/serialtools/apps/send.py` & `serialtools-0.2.0/src/serialtools/apps/send.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/src/serialtools/bus.py` & `serialtools-0.2.0/src/serialtools/bus.py`

 * *Files 6% similar despite different names*

```diff
@@ -177,14 +177,28 @@
 			g = parser
 		g.add_argument('-p', '-c', '--port', '--channel')
 		if rx_only:
 			g.add_argument('-m', '--message')
 		parser.add_argument('-b', '--baudrate', default=self.baudrate, type=int)
 		parser.set_defaults(rx_only=rx_only)
 
+	def create_args(self, *, port: 'str|None' = None, baudrate: 'int|None' = None, virtual: 'bool|None' = None) -> argparse.Namespace:
+		parser = argparse.ArgumentParser()
+		self.add_arguments(parser)
+		args: 'list[str]' = []
+		if port:
+			args.append('--port')
+			args.append(port)
+		if baudrate:
+			args.append('--baudrate')
+			args.append(str(baudrate))
+		if virtual:
+			args.append('--virtual')
+		return parser.parse_args(args)
+
 	def create_bus(self, args: 'argparse.Namespace') -> Bus:
 		if args.rx_only:
 			if args.message:
 				return ReadFromParameterBus(args.message)
 			if args.port and os.path.isfile(args.port):
 				return ReadFromFileBus(args.port)
```

### Comparing `serialtools-0.1.0/src/serialtools/database.py` & `serialtools-0.2.0/src/serialtools/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,28 @@
 					break
 				val.append(b)
 				first_byte = False
 			values[spec.name] = bytes(val)
 
 		return Message(self.db, values=values, timestamp=get_timestamp(self.bus))
 
+	def send_msg(self, msg: Message) -> None:
+		values = dict(msg.values)
+		out: 'list[int]' = []
+		for spec in self.db.message_spec:
+			if spec.name in values:
+				out.extend(values.pop(spec.name))
+			elif spec.allowed_values and len(spec.allowed_values) == 1:
+				out.extend(spec.allowed_values[0])
+			else:
+				raise TypeError(f"Missing value for {spec.name!r}")
+		if values:
+			raise TypeError(f"Invalid value(s) passed: " + ", ".join(values.keys()))
+
+		self.bus.write(bytes(out))
 
 	def read_byte(self) -> int:
 		out = self.read_n_bytes(1)
 		assert len(out) == 1
 		b = out[0]
 		return b
```

### Comparing `serialtools-0.1.0/src/serialtools/database_config.py` & `serialtools-0.2.0/src/serialtools/database_config.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.1.0/PKG-INFO` & `serialtools-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: serialtools
-Version: 0.1.0
+Version: 0.2.0
 Summary: Tools to work with a serial bus
 Author-email: erzo <erzo@posteo.de>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: BSD License
 Requires-Dist: pyserial
 Requires-Dist: confattr >= 0.13.0
 Requires-Dist: bitstruct
 Project-URL: Bug tracker, https://gitlab.com/erzo/serialtools/-/issues
 Project-URL: Change log, https://gitlab.com/erzo/serialtools/-/tags
+Project-URL: Documentation, https://erzo.gitlab.io/serialtools/latest
 Project-URL: Source code, https://gitlab.com/erzo/serialtools
 
 Tools to work with a serial bus.
 
 This project aims to become for the serial bus what [cantools](https://cantools.readthedocs.io/en/latest/) is for the CAN bus.
 
 In contrast to other tools for a serial bus like
```

