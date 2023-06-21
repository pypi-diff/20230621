# Comparing `tmp/blackboardsync-0.8.5rc4.tar.gz` & `tmp/blackboardsync-0.9.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackboardsync-0.8.5rc4.tar", last modified: Fri Jun 16 21:13:01 2023, max compression
+gzip compressed data, was "blackboardsync-0.9.0a1.tar", last modified: Wed Jun 21 09:08:54 2023, max compression
```

## Comparing `blackboardsync-0.8.5rc4.tar` & `blackboardsync-0.9.0a1.tar`

### file list

```diff
@@ -1,76 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:13:01.925231 blackboardsync-0.8.5rc4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:13:01.913231 blackboardsync-0.8.5rc4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:13:01.913231 blackboardsync-0.8.5rc4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-06-16 21:13:01.925231 blackboardsync-0.8.5rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    99257 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/UNIVERSITIES.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:13:01.917231 blackboardsync-0.8.5rc4/blackboard_sync/
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/blackboard_sync/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/blackboard_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/blackboard_sync/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:13:01.917231 blackboardsync-0.8.5rc4/blackboard_sync/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/blackboard_sync/assets/alert.png
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/blackboard_sync/assets/alert.svg
--rw-r--r--   0 runner    (1001) docker     (123)   110234 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/blackboard_sync/assets/logo.ico
--rw-r--r--   0 runner    (1001) docker     (123)    31742 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/blackboard_sync/assets/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    36877 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/blackboard_sync/assets/watermark.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:13:01.917231 blackboardsync-0.8.5rc4/blackboard_sync/blackboard/
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/blackboard_sync/blackboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29665 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/blackboard_sync/blackboard/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/blackboard_sync/blackboard/blackboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/blackboard_sync/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/blackboard_sync/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/blackboard_sync/institutions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:13:01.921231 blackboardsync-0.8.5rc4/blackboard_sync/qt/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/blackboard_sync/qt/LoginWebView.ui
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/blackboard_sync/qt/PersistenceWarning.ui
--rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/blackboard_sync/qt/SettingsWindow.ui
--rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/blackboard_sync/qt/SetupWizard.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/blackboard_sync/qt/UniNotSupportedDialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/blackboard_sync/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20622 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/blackboard_sync/qt/qt_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    10725 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/blackboard_sync/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/blackboard_sync/sync_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/blackboard_sync/universities.json
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/blackboard_sync/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/blackboard_sync/webdav.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:13:01.921231 blackboardsync-0.8.5rc4/blackboardsync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-06-16 21:13:01.000000 blackboardsync-0.8.5rc4/blackboardsync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-16 21:13:01.000000 blackboardsync-0.8.5rc4/blackboardsync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 21:13:01.000000 blackboardsync-0.8.5rc4/blackboardsync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-16 21:13:01.000000 blackboardsync-0.8.5rc4/blackboardsync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 21:13:01.000000 blackboardsync-0.8.5rc4/blackboardsync.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:13:01.921231 blackboardsync-0.8.5rc4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:13:01.921231 blackboardsync-0.8.5rc4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:13:01.921231 blackboardsync-0.8.5rc4/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/docs/dev/bb_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/docs/dev/qt_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/docs/dev/sync_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:13:01.925231 blackboardsync-0.8.5rc4/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/packaging/pkg_macos.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/packaging/pkg_win.nsi
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/packaging/pyinst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-16 21:13:01.925231 blackboardsync-0.8.5rc4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:13:01.925231 blackboardsync-0.8.5rc4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/tests/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/tests/test_blackboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    12146 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/tests/test_qt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-16 21:12:19.000000 blackboardsync-0.8.5rc4/tests/test_sync_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:08:54.579336 blackboardsync-0.9.0a1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:08:54.567335 blackboardsync-0.9.0a1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:08:54.567335 blackboardsync-0.9.0a1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/.github/ISSUE_TEMPLATE/unisupport.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:08:54.567335 blackboardsync-0.9.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-06-21 09:08:54.579336 blackboardsync-0.9.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)   107308 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/UNIVERSITIES.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:08:54.571336 blackboardsync-0.9.0a1/blackboard_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:08:54.571336 blackboardsync-0.9.0a1/blackboard_sync/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/assets/alert.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/assets/alert.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   110234 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/assets/logo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    31742 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/assets/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36877 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/assets/watermark.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:08:54.571336 blackboardsync-0.9.0a1/blackboard_sync/blackboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/blackboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29665 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/blackboard/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/blackboard/blackboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10082 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/institutions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:08:54.571336 blackboardsync-0.9.0a1/blackboard_sync/qt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/qt/LoginWebView.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/qt/PersistenceWarning.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     8000 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/qt/SettingsWindow.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/qt/SetupWizard.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/qt/UniNotSupportedDialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20342 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/qt/qt_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10269 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/sync_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/universities.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/webdav.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:08:54.575336 blackboardsync-0.9.0a1/blackboardsync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-06-21 09:08:54.000000 blackboardsync-0.9.0a1/blackboardsync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-21 09:08:54.000000 blackboardsync-0.9.0a1/blackboardsync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 09:08:54.000000 blackboardsync-0.9.0a1/blackboardsync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-21 09:08:54.000000 blackboardsync-0.9.0a1/blackboardsync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-21 09:08:54.000000 blackboardsync-0.9.0a1/blackboardsync.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:08:54.575336 blackboardsync-0.9.0a1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:08:54.575336 blackboardsync-0.9.0a1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:08:54.575336 blackboardsync-0.9.0a1/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/docs/dev/bb_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/docs/dev/qt_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/docs/dev/sync_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:08:54.575336 blackboardsync-0.9.0a1/packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/packaging/pkg_macos.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/packaging/pkg_win.nsi
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/packaging/pyinst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 09:08:54.579336 blackboardsync-0.9.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:08:54.579336 blackboardsync-0.9.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/tests/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/tests/test_blackboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12146 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/tests/test_qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/tests/test_sync_config.py
```

### Comparing `blackboardsync-0.8.5rc4/.github/workflows/build.yml` & `blackboardsync-0.9.0a1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/.gitignore` & `blackboardsync-0.9.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/CONTRIBUTING.md` & `blackboardsync-0.9.0a1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/LICENSE` & `blackboardsync-0.9.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/PKG-INFO` & `blackboardsync-0.9.0a1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboardsync
-Version: 0.8.5rc4
+Version: 0.9.0a1
 Summary: Sync your blackboard content to your device
 Author-email: Jacob Sánchez <jacobszpz@protonmail.com>
 Project-URL: Homepage, https://bbsync.app
 Project-URL: Repository, https://github.com/jacobszpz/BlackboardSync
 Project-URL: Bug Tracker, https://github.com/jacobszpz/BlackboardSync/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -14,15 +14,15 @@
 Provides-Extra: test
 Provides-Extra: package
 License-File: LICENSE
 
 # BlackboardSync
 ### Automatic Syncing Of Your Blackboard Content
 
-[![License: GPL  v2][license-shield]][gnu] [![Build][build-shield]][actions]
+[![Get on PyPI][pypi-shield]][pypi] [![License: GPL  v2][license-shield]][gnu] [![Build][build-shield]][actions]
 
 **BlackboardSync** performs a periodic, incremental download of all your Blackboard content, such as lecture slides, lab sheets, and other attachments.
 
 
 <div align="center">
 	<img src="https://raw.githubusercontent.com/jacobszpz/BlackboardSync/main/blackboard_sync/assets/logo.png" height="auto" width="25%" />
 </div>
@@ -67,18 +67,23 @@
 
 
 
 ## Installation
 
 #### Binaries
 
-Currently unavailable (until a more stable version).
+You can find all releases on [GitHub][releases].
+Only MacOS (.dmg) and Windows (.exe) are supported at the moment.
 
-Alternatively, you can run the python package [directly](#running-without-building), or build an executable yourself by following [these steps](#building-from-source).
+Note: These releases are automatically built on GitHub Actions from source.
 
+**⚠️ ATTENTION MACOS USERS **
+
+On MacOS, you will face an issue when trying to open the application, since it has not
+been notarised by Apple. A workaround can be found [here][apple-dev].
 
 
 #### From PyPI
 
 ```bash
 python3 -m pip install blackboardsync
 ```
@@ -174,14 +179,15 @@
 
 
 
 <!-- LINK REFERENCES -->
 
 [universal-login]: https://github.com/jacobszpz/BlackboardSync/issues/3	"BBSync login"
 [pyqt]: https://pypi.org/project/PyQt5/5.15.1/	"Python Bindings for Qt 5"
+[pypi]: https://pypi.org/project/blackboardsync
 [typora]: https://typora.io/ "Typora"
 [releases]: https://github.com/jacobszpz/BlackboardSync/releases "BlackboardSync Releases"
 [issues]: https://github.com/jacobszpz/BlackboardSync/issues/new "BlackboardSync Issues"
 [git]: https://git-scm.com/	"Git"
 [python]: https://www.python.org/ "Python.org"
 [pipenv]: https://pipenv.pypa.io/en/latest/ "Pipenv"
 [license]: LICENSE "General Public License"
@@ -190,27 +196,28 @@
 [pyinstaller]: https://www.pyinstaller.org/	"PyInstaller"
 
 
 
 <!-- RELEASES -->
 
 [releases]: https://github.com/jacobszpz/BlackboardSync/releases/
+[apple-dev]: https://support.apple.com/en-gb/guide/mac-help/mh40616/mac
 
 
 <!-- README TEMPLATES -->
 
 [tonycrosby]: https://gist.github.com/tonycrosby-tech/c18c2b6c74900c6080fc097ca0718839	"tonycrosby-tech README template"
 [neildrew]: https://github.com/othneildrew/Best-README-Template	"othneildrew README template"
 [bulldogjob]: https://bulldogjob.com/news/449-how-to-write-a-good-readme-for-your-github-project	"bulldogjob README guide"
 
 
 
 <!-- SHIELDS -->
 
-[version-shield]: https://img.shields.io/pypi/v/BlackboardSync
+[pypi-shield]: https://img.shields.io/pypi/v/BlackboardSync
 [license-shield]: https://img.shields.io/github/license/jacobszpz/BlackboardSync
 [build-shield]: https://img.shields.io/github/actions/workflow/status/jacobszpz/BlackboardSync/build.yml?branch=main
 [kofi-shield]: https://ko-fi.com/img/githubbutton_sm.svg
 [lp-shield]: https://img.shields.io/liberapay/receives/BlackboardSync.svg?logo=liberapay
```

### Comparing `blackboardsync-0.8.5rc4/Pipfile` & `blackboardsync-0.9.0a1/Pipfile`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/Pipfile.lock` & `blackboardsync-0.9.0a1/Pipfile.lock`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9800347222222223%*

 * *Differences: {"'default'": '{\'charset-normalizer\': {\'markers\': "python_version >= \'3.7\'"}, \'pydantic\': '*

 * *              "{'hashes': "*

 * *              "['sha256:07293ab08e7b4d3c9d7de4949a0ea571f11e4557d19ea24dd3ae0c524c0c334d', "*

 * *              "'sha256:0a2aabdc73c2a5960e87c3ffebca6ccde88665616d1fd6d3db3178ef427b267a', "*

 * *              "'sha256:0da48717dc9495d3a8f215e0d012599db6b8092db02acac5e0d58a65248ec5bc', "*

 * *              "'sha256:128d9453d92e6e81e881dd7e2484e08d8b164da5507f62d06ceecf84bf2e21d3', "*

 * *              " […]*

```diff
@@ -114,15 +114,15 @@
                 "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
                 "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
                 "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
                 "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
                 "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
                 "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
             ],
-            "markers": "python_full_version >= '3.7.0'",
+            "markers": "python_version >= '3.7'",
             "version": "==3.1.0"
         },
         "idna": {
             "hashes": [
                 "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
@@ -226,53 +226,53 @@
                 "sha256:dcdb89f0bde6fd5eba6f2202a7863f657afbc810ef32f60e9258d58ede8155ac"
             ],
             "index": "pypi",
             "version": "==3.0.0"
         },
         "pydantic": {
             "hashes": [
-                "sha256:052d8654cb65174d6f9490cc9b9a200083a82cf5c3c5d3985db765757eb3b375",
-                "sha256:0c6fafa0965b539d7aab0a673a046466d23b86e4b0e8019d25fd53f4df62c277",
-                "sha256:1243d28e9b05003a89d72e7915fdb26ffd1d39bdd39b00b7dbe4afae4b557f9d",
-                "sha256:12f7b0bf8553e310e530e9f3a2f5734c68699f42218bf3568ef49cd9b0e44df4",
-                "sha256:1410275520dfa70effadf4c21811d755e7ef9bb1f1d077a21958153a92c8d9ca",
-                "sha256:16f8c3e33af1e9bb16c7a91fc7d5fa9fe27298e9f299cff6cb744d89d573d62c",
-                "sha256:17aef11cc1b997f9d574b91909fed40761e13fac438d72b81f902226a69dac01",
-                "sha256:191ba419b605f897ede9892f6c56fb182f40a15d309ef0142212200a10af4c18",
-                "sha256:1952526ba40b220b912cdc43c1c32bcf4a58e3f192fa313ee665916b26befb68",
-                "sha256:1ced8375969673929809d7f36ad322934c35de4af3b5e5b09ec967c21f9f7887",
-                "sha256:2e4148e635994d57d834be1182a44bdb07dd867fa3c2d1b37002000646cc5459",
-                "sha256:34d327c81e68a1ecb52fe9c8d50c8a9b3e90d3c8ad991bfc8f953fb477d42fb4",
-                "sha256:35db5301b82e8661fa9c505c800d0990bc14e9f36f98932bb1d248c0ac5cada5",
-                "sha256:3e59417ba8a17265e632af99cc5f35ec309de5980c440c255ab1ca3ae96a3e0e",
-                "sha256:42aa0c4b5c3025483240a25b09f3c09a189481ddda2ea3a831a9d25f444e03c1",
-                "sha256:666bdf6066bf6dbc107b30d034615d2627e2121506c555f73f90b54a463d1f33",
-                "sha256:66a703d1983c675a6e0fed8953b0971c44dba48a929a2000a493c3772eb61a5a",
-                "sha256:6a82d6cda82258efca32b40040228ecf43a548671cb174a1e81477195ed3ed56",
-                "sha256:6f2e754d5566f050954727c77f094e01793bcb5725b663bf628fa6743a5a9108",
-                "sha256:7456eb22ed9aaa24ff3e7b4757da20d9e5ce2a81018c1b3ebd81a0b88a18f3b2",
-                "sha256:7b1f6cb446470b7ddf86c2e57cd119a24959af2b01e552f60705910663af09a4",
-                "sha256:7d5b8641c24886d764a74ec541d2fc2c7fb19f6da2a4001e6d580ba4a38f7878",
-                "sha256:84d80219c3f8d4cad44575e18404099c76851bc924ce5ab1c4c8bb5e2a2227d0",
-                "sha256:88f195f582851e8db960b4a94c3e3ad25692c1c1539e2552f3df7a9e972ef60e",
-                "sha256:93e6bcfccbd831894a6a434b0aeb1947f9e70b7468f274154d03d71fabb1d7c6",
-                "sha256:93e766b4a8226e0708ef243e843105bf124e21331694367f95f4e3b4a92bbb3f",
-                "sha256:ab523c31e22943713d80d8d342d23b6f6ac4b792a1e54064a8d0cf78fd64e800",
-                "sha256:bb14388ec45a7a0dc429e87def6396f9e73c8c77818c927b6a60706603d5f2ea",
-                "sha256:c0ab53b609c11dfc0c060d94335993cc2b95b2150e25583bec37a49b2d6c6c3f",
-                "sha256:c33b60054b2136aef8cf190cd4c52a3daa20b2263917c49adad20eaf381e823b",
-                "sha256:ceb6a23bf1ba4b837d0cfe378329ad3f351b5897c8d4914ce95b85fba96da5a1",
-                "sha256:d532bf00f381bd6bc62cabc7d1372096b75a33bc197a312b03f5838b4fb84edd",
-                "sha256:df7800cb1984d8f6e249351139667a8c50a379009271ee6236138a22a0c0f319",
-                "sha256:e82d4566fcd527eae8b244fa952d99f2ca3172b7e97add0b43e2d97ee77f81ab",
-                "sha256:f90c1e29f447557e9e26afb1c4dbf8768a10cc676e3781b6a577841ade126b85",
-                "sha256:f9613fadad06b4f3bc5db2653ce2f22e0de84a7c6c293909b48f6ed37b83c61f"
+                "sha256:07293ab08e7b4d3c9d7de4949a0ea571f11e4557d19ea24dd3ae0c524c0c334d",
+                "sha256:0a2aabdc73c2a5960e87c3ffebca6ccde88665616d1fd6d3db3178ef427b267a",
+                "sha256:0da48717dc9495d3a8f215e0d012599db6b8092db02acac5e0d58a65248ec5bc",
+                "sha256:128d9453d92e6e81e881dd7e2484e08d8b164da5507f62d06ceecf84bf2e21d3",
+                "sha256:2196c06484da2b3fded1ab6dbe182bdabeb09f6318b7fdc412609ee2b564c49a",
+                "sha256:2e9aec8627a1a6823fc62fb96480abe3eb10168fd0d859ee3d3b395105ae19a7",
+                "sha256:3283b574b01e8dbc982080d8287c968489d25329a463b29a90d4157de4f2baaf",
+                "sha256:3c52eb595db83e189419bf337b59154bdcca642ee4b2a09e5d7797e41ace783f",
+                "sha256:4b466a23009ff5cdd7076eb56aca537c745ca491293cc38e72bf1e0e00de5b91",
+                "sha256:517a681919bf880ce1dac7e5bc0c3af1e58ba118fd774da2ffcd93c5f96eaece",
+                "sha256:5f8bbaf4013b9a50e8100333cc4e3fa2f81214033e05ac5aa44fa24a98670a29",
+                "sha256:6257bb45ad78abacda13f15bde5886efd6bf549dd71085e64b8dcf9919c38b60",
+                "sha256:67195274fd27780f15c4c372f4ba9a5c02dad6d50647b917b6a92bf00b3d301a",
+                "sha256:6cafde02f6699ce4ff643417d1a9223716ec25e228ddc3b436fe7e2d25a1f305",
+                "sha256:73ef93e5e1d3c8e83f1ff2e7fdd026d9e063c7e089394869a6e2985696693766",
+                "sha256:7845b31959468bc5b78d7b95ec52fe5be32b55d0d09983a877cca6aedc51068f",
+                "sha256:7847ca62e581e6088d9000f3c497267868ca2fa89432714e21a4fb33a04d52e8",
+                "sha256:7e1d5290044f620f80cf1c969c542a5468f3656de47b41aa78100c5baa2b8276",
+                "sha256:7ee829b86ce984261d99ff2fd6e88f2230068d96c2a582f29583ed602ef3fc2c",
+                "sha256:83fcff3c7df7adff880622a98022626f4f6dbce6639a88a15a3ce0f96466cb60",
+                "sha256:939328fd539b8d0edf244327398a667b6b140afd3bf7e347cf9813c736211896",
+                "sha256:95c70da2cd3b6ddf3b9645ecaa8d98f3d80c606624b6d245558d202cd23ea3be",
+                "sha256:963671eda0b6ba6926d8fc759e3e10335e1dc1b71ff2a43ed2efd6996634dafb",
+                "sha256:970b1bdc6243ef663ba5c7e36ac9ab1f2bfecb8ad297c9824b542d41a750b298",
+                "sha256:9863b9420d99dfa9c064042304868e8ba08e89081428a1c471858aa2af6f57c4",
+                "sha256:ad428e92ab68798d9326bb3e5515bc927444a3d71a93b4a2ca02a8a5d795c572",
+                "sha256:b48d3d634bca23b172f47f2335c617d3fcb4b3ba18481c96b7943a4c634f5c8d",
+                "sha256:b9cd67fb763248cbe38f0593cd8611bfe4b8ad82acb3bdf2b0898c23415a1f82",
+                "sha256:d111a21bbbfd85c17248130deac02bbd9b5e20b303338e0dbe0faa78330e37e0",
+                "sha256:e1aa5c2410769ca28aa9a7841b80d9d9a1c5f223928ca8bec7e7c9a34d26b1d4",
+                "sha256:e692dec4a40bfb40ca530e07805b1208c1de071a18d26af4a2a0d79015b352ca",
+                "sha256:e7c9900b43ac14110efa977be3da28931ffc74c27e96ee89fbcaaf0b0fe338e1",
+                "sha256:eec39224b2b2e861259d6f3c8b6290d4e0fbdce147adb797484a42278a1a486f",
+                "sha256:f0b7628fb8efe60fe66fd4adadd7ad2304014770cdc1f4934db41fe46cc8825f",
+                "sha256:f50e1764ce9353be67267e7fd0da08349397c7db17a562ad036aa7c8f4adfdb6",
+                "sha256:fab81a92f42d6d525dd47ced310b0c3e10c416bbfae5d59523e63ea22f82b31e"
             ],
             "index": "pypi",
-            "version": "==1.10.8"
+            "version": "==1.10.9"
         },
         "pyqt5": {
             "hashes": [
                 "sha256:883ba5c8a348be78c8be6a3d3ba014c798e679503bce00d76c666c2dc6afe828",
                 "sha256:dc41e8401a90dc3e2b692b411bd5492ab559ae27a27424eed4bd3915564ec4c0",
                 "sha256:dd5ce10e79fbf1df29507d2daf99270f2057cdd25e4de6fbf2052b46c652e3a5",
                 "sha256:e030d795df4cbbfcf4f38b18e2e119bcc9e177ef658a5094b87bb16cac0ce4c5",
@@ -351,19 +351,19 @@
                 "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
             "index": "pypi",
             "version": "==2.31.0"
         },
         "setuptools": {
             "hashes": [
-                "sha256:5df61bf30bb10c6f756eb19e7c9f3b473051f48db77fddbe06ff2ca307df9a6f",
-                "sha256:62642358adc77ffa87233bc4d2354c4b2682d214048f500964dbe760ccedf102"
+                "sha256:11e52c67415a381d10d6b462ced9cfb97066179f0e871399e006c4ab101fc85f",
+                "sha256:baf1fdb41c6da4cd2eae722e135500da913332ab3f2f5c7d33af9b492acb5235"
             ],
             "index": "pypi",
-            "version": "==67.8.0"
+            "version": "==68.0.0"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -383,19 +383,19 @@
                 "sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==4.6.3"
         },
         "urllib3": {
             "hashes": [
-                "sha256:61717a1095d7e155cdb737ac7bb2f4324a858a1e2e6466f6d03ff630ca68d3cc",
-                "sha256:d055c2f9d38dc53c808f6fdc8eab7360b6fdbbde02340ed25cfbcd817c62469e"
+                "sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1",
+                "sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.0.2"
+            "version": "==2.0.3"
         }
     },
     "develop": {
         "alabaster": {
             "hashes": [
                 "sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3",
                 "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"
@@ -492,14 +492,83 @@
             "hashes": [
                 "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
                 "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==2023.5.7"
         },
+        "cffi": {
+            "hashes": [
+                "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
+                "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
+                "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
+                "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
+                "sha256:173379135477dc8cac4bc58f45db08ab45d228b3363adb7af79436135d028405",
+                "sha256:198caafb44239b60e252492445da556afafc7d1e3ab7a1fb3f0584ef6d742375",
+                "sha256:1e74c6b51a9ed6589199c787bf5f9875612ca4a8a0785fb2d4a84429badaf22a",
+                "sha256:2012c72d854c2d03e45d06ae57f40d78e5770d252f195b93f581acf3ba44496e",
+                "sha256:21157295583fe8943475029ed5abdcf71eb3911894724e360acff1d61c1d54bc",
+                "sha256:2470043b93ff09bf8fb1d46d1cb756ce6132c54826661a32d4e4d132e1977adf",
+                "sha256:285d29981935eb726a4399badae8f0ffdff4f5050eaa6d0cfc3f64b857b77185",
+                "sha256:30d78fbc8ebf9c92c9b7823ee18eb92f2e6ef79b45ac84db507f52fbe3ec4497",
+                "sha256:320dab6e7cb2eacdf0e658569d2575c4dad258c0fcc794f46215e1e39f90f2c3",
+                "sha256:33ab79603146aace82c2427da5ca6e58f2b3f2fb5da893ceac0c42218a40be35",
+                "sha256:3548db281cd7d2561c9ad9984681c95f7b0e38881201e157833a2342c30d5e8c",
+                "sha256:3799aecf2e17cf585d977b780ce79ff0dc9b78d799fc694221ce814c2c19db83",
+                "sha256:39d39875251ca8f612b6f33e6b1195af86d1b3e60086068be9cc053aa4376e21",
+                "sha256:3b926aa83d1edb5aa5b427b4053dc420ec295a08e40911296b9eb1b6170f6cca",
+                "sha256:3bcde07039e586f91b45c88f8583ea7cf7a0770df3a1649627bf598332cb6984",
+                "sha256:3d08afd128ddaa624a48cf2b859afef385b720bb4b43df214f85616922e6a5ac",
+                "sha256:3eb6971dcff08619f8d91607cfc726518b6fa2a9eba42856be181c6d0d9515fd",
+                "sha256:40f4774f5a9d4f5e344f31a32b5096977b5d48560c5592e2f3d2c4374bd543ee",
+                "sha256:4289fc34b2f5316fbb762d75362931e351941fa95fa18789191b33fc4cf9504a",
+                "sha256:470c103ae716238bbe698d67ad020e1db9d9dba34fa5a899b5e21577e6d52ed2",
+                "sha256:4f2c9f67e9821cad2e5f480bc8d83b8742896f1242dba247911072d4fa94c192",
+                "sha256:50a74364d85fd319352182ef59c5c790484a336f6db772c1a9231f1c3ed0cbd7",
+                "sha256:54a2db7b78338edd780e7ef7f9f6c442500fb0d41a5a4ea24fff1c929d5af585",
+                "sha256:5635bd9cb9731e6d4a1132a498dd34f764034a8ce60cef4f5319c0541159392f",
+                "sha256:59c0b02d0a6c384d453fece7566d1c7e6b7bae4fc5874ef2ef46d56776d61c9e",
+                "sha256:5d598b938678ebf3c67377cdd45e09d431369c3b1a5b331058c338e201f12b27",
+                "sha256:5df2768244d19ab7f60546d0c7c63ce1581f7af8b5de3eb3004b9b6fc8a9f84b",
+                "sha256:5ef34d190326c3b1f822a5b7a45f6c4535e2f47ed06fec77d3d799c450b2651e",
+                "sha256:6975a3fac6bc83c4a65c9f9fcab9e47019a11d3d2cf7f3c0d03431bf145a941e",
+                "sha256:6c9a799e985904922a4d207a94eae35c78ebae90e128f0c4e521ce339396be9d",
+                "sha256:70df4e3b545a17496c9b3f41f5115e69a4f2e77e94e1d2a8e1070bc0c38c8a3c",
+                "sha256:7473e861101c9e72452f9bf8acb984947aa1661a7704553a9f6e4baa5ba64415",
+                "sha256:8102eaf27e1e448db915d08afa8b41d6c7ca7a04b7d73af6514df10a3e74bd82",
+                "sha256:87c450779d0914f2861b8526e035c5e6da0a3199d8f1add1a665e1cbc6fc6d02",
+                "sha256:8b7ee99e510d7b66cdb6c593f21c043c248537a32e0bedf02e01e9553a172314",
+                "sha256:91fc98adde3d7881af9b59ed0294046f3806221863722ba7d8d120c575314325",
+                "sha256:94411f22c3985acaec6f83c6df553f2dbe17b698cc7f8ae751ff2237d96b9e3c",
+                "sha256:98d85c6a2bef81588d9227dde12db8a7f47f639f4a17c9ae08e773aa9c697bf3",
+                "sha256:9ad5db27f9cabae298d151c85cf2bad1d359a1b9c686a275df03385758e2f914",
+                "sha256:a0b71b1b8fbf2b96e41c4d990244165e2c9be83d54962a9a1d118fd8657d2045",
+                "sha256:a0f100c8912c114ff53e1202d0078b425bee3649ae34d7b070e9697f93c5d52d",
+                "sha256:a591fe9e525846e4d154205572a029f653ada1a78b93697f3b5a8f1f2bc055b9",
+                "sha256:a5c84c68147988265e60416b57fc83425a78058853509c1b0629c180094904a5",
+                "sha256:a66d3508133af6e8548451b25058d5812812ec3798c886bf38ed24a98216fab2",
+                "sha256:a8c4917bd7ad33e8eb21e9a5bbba979b49d9a97acb3a803092cbc1133e20343c",
+                "sha256:b3bbeb01c2b273cca1e1e0c5df57f12dce9a4dd331b4fa1635b8bec26350bde3",
+                "sha256:cba9d6b9a7d64d4bd46167096fc9d2f835e25d7e4c121fb2ddfc6528fb0413b2",
+                "sha256:cc4d65aeeaa04136a12677d3dd0b1c0c94dc43abac5860ab33cceb42b801c1e8",
+                "sha256:ce4bcc037df4fc5e3d184794f27bdaab018943698f4ca31630bc7f84a7b69c6d",
+                "sha256:cec7d9412a9102bdc577382c3929b337320c4c4c4849f2c5cdd14d7368c5562d",
+                "sha256:d400bfb9a37b1351253cb402671cea7e89bdecc294e8016a707f6d1d8ac934f9",
+                "sha256:d61f4695e6c866a23a21acab0509af1cdfd2c013cf256bbf5b6b5e2695827162",
+                "sha256:db0fbb9c62743ce59a9ff687eb5f4afbe77e5e8403d6697f7446e5f609976f76",
+                "sha256:dd86c085fae2efd48ac91dd7ccffcfc0571387fe1193d33b6394db7ef31fe2a4",
+                "sha256:e00b098126fd45523dd056d2efba6c5a63b71ffe9f2bbe1a4fe1716e1d0c331e",
+                "sha256:e229a521186c75c8ad9490854fd8bbdd9a0c9aa3a524326b55be83b54d4e0ad9",
+                "sha256:e263d77ee3dd201c3a142934a086a4450861778baaeeb45db4591ef65550b0a6",
+                "sha256:ed9cb427ba5504c1dc15ede7d516b84757c3e3d7868ccc85121d9310d27eed0b",
+                "sha256:fa6693661a4c91757f4412306191b6dc88c1703f780c8234035eac011922bc01",
+                "sha256:fcd131dd944808b5bdb38e6f5b53013c5aa4f334c5cad0c72742f6eba4b73db0"
+            ],
+            "version": "==1.15.1"
+        },
         "charset-normalizer": {
             "hashes": [
                 "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6",
                 "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1",
                 "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e",
                 "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373",
                 "sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62",
@@ -570,15 +639,15 @@
                 "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
                 "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
                 "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
                 "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
                 "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
                 "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
             ],
-            "markers": "python_full_version >= '3.7.0'",
+            "markers": "python_version >= '3.7'",
             "version": "==3.1.0"
         },
         "click": {
             "hashes": [
                 "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e",
                 "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
             ],
@@ -654,14 +723,39 @@
                 "sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e",
                 "sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850",
                 "sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3"
             ],
             "index": "pypi",
             "version": "==7.2.7"
         },
+        "cryptography": {
+            "hashes": [
+                "sha256:059e348f9a3c1950937e1b5d7ba1f8e968508ab181e75fc32b879452f08356db",
+                "sha256:1a5472d40c8f8e91ff7a3d8ac6dfa363d8e3138b961529c996f3e2df0c7a411a",
+                "sha256:1a8e6c2de6fbbcc5e14fd27fb24414507cb3333198ea9ab1258d916f00bc3039",
+                "sha256:1fee5aacc7367487b4e22484d3c7e547992ed726d14864ee33c0176ae43b0d7c",
+                "sha256:5d092fdfedaec4cbbffbf98cddc915ba145313a6fdaab83c6e67f4e6c218e6f3",
+                "sha256:5f0ff6e18d13a3de56f609dd1fd11470918f770c6bd5d00d632076c727d35485",
+                "sha256:7bfc55a5eae8b86a287747053140ba221afc65eb06207bedf6e019b8934b477c",
+                "sha256:7fa01527046ca5facdf973eef2535a27fec4cb651e4daec4d043ef63f6ecd4ca",
+                "sha256:8dde71c4169ec5ccc1087bb7521d54251c016f126f922ab2dfe6649170a3b8c5",
+                "sha256:8f4ab7021127a9b4323537300a2acfb450124b2def3756f64dc3a3d2160ee4b5",
+                "sha256:948224d76c4b6457349d47c0c98657557f429b4e93057cf5a2f71d603e2fc3a3",
+                "sha256:9a6c7a3c87d595608a39980ebaa04d5a37f94024c9f24eb7d10262b92f739ddb",
+                "sha256:b46e37db3cc267b4dea1f56da7346c9727e1209aa98487179ee8ebed09d21e43",
+                "sha256:b4ceb5324b998ce2003bc17d519080b4ec8d5b7b70794cbd2836101406a9be31",
+                "sha256:cb33ccf15e89f7ed89b235cff9d49e2e62c6c981a6061c9c8bb47ed7951190bc",
+                "sha256:d198820aba55660b4d74f7b5fd1f17db3aa5eb3e6893b0a41b75e84e4f9e0e4b",
+                "sha256:d34579085401d3f49762d2f7d6634d6b6c2ae1242202e860f4d26b046e3a1006",
+                "sha256:eb8163f5e549a22888c18b0d53d6bb62a20510060a22fd5a995ec8a05268df8a",
+                "sha256:f73bff05db2a3e5974a6fd248af2566134d8981fd7ab012e5dd4ddb1d9a70699"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==41.0.1"
+        },
         "dill": {
             "hashes": [
                 "sha256:a07ffd2351b8c678dfc4a856a3005f8067aea51d6ba6c700796a4d9e280f39f0",
                 "sha256:e5db55f3687856d8fbdab002ed78544e1c4559a130302693d839dfe8f93f2373"
             ],
             "markers": "python_version < '3.11'",
             "version": "==0.3.6"
@@ -695,19 +789,19 @@
                 "sha256:3833794e27ff64ea4e9cf5d410082a8b97ff1a06c16aa3d2027339cd0f1195c7",
                 "sha256:c61007e76655af75e6785a931f452915b371dc48f56efd765247c8fe68f2b181"
             ],
             "version": "==6.0.0"
         },
         "hypothesis": {
             "hashes": [
-                "sha256:034f73dd485933b0f4c319d7c3c58230492fdd7b16e821d67d150a78138adb93",
-                "sha256:526657eb3e4f2076b0383f722b2e6a92fd15d1d42db532decae8c41b14cab801"
+                "sha256:7a0b8ca178f16720e96f11e96b71b6139db0e30727e9cf8bd8e3059710393fc7",
+                "sha256:de8fb599fc855d3006236ab58cd0edafd099d63837225aad848dac22e239475b"
             ],
             "index": "pypi",
-            "version": "==6.76.0"
+            "version": "==6.79.1"
         },
         "idna": {
             "hashes": [
                 "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3.5'",
@@ -719,19 +813,19 @@
                 "sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.4.1"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:43dd286a2cd8995d5eaef7fee2066340423b818ed3fd70adf0bad5f1fac53fed",
-                "sha256:92501cdf9cc66ebd3e612f1b4f0c0765dfa42f0fa38ffb319b6bd84dd675d705"
+                "sha256:1aaf550d4f73e5d6783e7acb77aec43d49da8017410afae93822cc9cca98c4d4",
+                "sha256:cb52082e659e97afc5dac71e79de97d8681de3aa07ff18578330904a9d18e5b5"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==6.6.0"
+            "version": "==6.7.0"
         },
         "iniconfig": {
             "hashes": [
                 "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
                 "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
             ],
             "markers": "python_version >= '3.7'",
@@ -760,29 +854,37 @@
             "hashes": [
                 "sha256:203c1fd9d969ab8f2119ec0a3342e0b49910045abe6af0a3ae83a5764d54639e",
                 "sha256:bae794c30d07f6d910d32a7048af09b5a39ed740918da923c6b780790ebac612"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.18.2"
         },
+        "jeepney": {
+            "hashes": [
+                "sha256:5efe48d255973902f6badc3ce55e2aa6c5c3b3bc642059ef3a91247bcfcc5806",
+                "sha256:c0a454ad016ca575060802ee4d590dd912e35c122fa04e70306de3d076cce755"
+            ],
+            "markers": "sys_platform == 'linux'",
+            "version": "==0.8.0"
+        },
         "jinja2": {
             "hashes": [
                 "sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852",
                 "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.1.2"
         },
         "keyring": {
             "hashes": [
-                "sha256:771ed2a91909389ed6148631de678f82ddc73737d85a927f382a8a1b157898cd",
-                "sha256:ba2e15a9b35e21908d0aaf4e0a47acc52d6ae33444df0da2b49d41a46ef6d678"
+                "sha256:4e87665a19c514c7edada8b15015cf89bd99b8d7edabc5c43cca77166fa8dfad",
+                "sha256:770f609eed2a16c65a6349f3ba1545d00c73f9fed4254c13766c674fe6d0d22b"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==23.13.1"
+            "version": "==24.0.0"
         },
         "lazy-object-proxy": {
             "hashes": [
                 "sha256:09763491ce220c0299688940f8dc2c5d05fd1f45af1e42e636b2e8b2303e4382",
                 "sha256:0a891e4e41b54fd5b8313b96399f8b0e173bbbfc03c7631f01efbe29bb0bcf82",
                 "sha256:189bbd5d41ae7a498397287c408617fe5c48633e7755287b21d741f7db2706a9",
                 "sha256:18b78ec83edbbeb69efdc0e9c1cb41a3b1b1ed11ddd8ded602464c3fc6020494",
@@ -818,29 +920,21 @@
                 "sha256:f12ad7126ae0c98d601a7ee504c1122bcef553d1d5e0c3bfa77b16b3968d2734",
                 "sha256:f2457189d8257dd41ae9b434ba33298aec198e30adf2dcdaaa3a28b9994f6adb",
                 "sha256:f699ac1c768270c9e384e4cbd268d6e67aebcfae6cd623b4d7c3bfde5a35db59"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.9.0"
         },
-        "macholib": {
-            "hashes": [
-                "sha256:44c40f2cd7d6726af8fa6fe22549178d3a4dfecc35a9cd15ea916d9c83a688e0",
-                "sha256:557bbfa1bb255c20e9abafe7ed6cd8046b48d9525db2f9b77d3122a63a2a8bf8"
-            ],
-            "markers": "sys_platform == 'darwin'",
-            "version": "==1.16.2"
-        },
         "markdown-it-py": {
             "hashes": [
-                "sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30",
-                "sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1"
+                "sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1",
+                "sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==2.2.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==3.0.0"
         },
         "markupsafe": {
             "hashes": [
                 "sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e",
                 "sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e",
                 "sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431",
                 "sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686",
@@ -1067,19 +1161,19 @@
                 "sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.9.6"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:412dae91f52a6f84830f39a8078cecd0e866cb72294a5c66808e74d5e88d251f",
-                "sha256:e2378146f1964972c03c085bb5662ae80b2b8c06226c54b2ff4aa9483e8a13a5"
+                "sha256:57e28820ca8094678b807ff529196506d7a21e17156cb1cddb3e74cebce54640",
+                "sha256:ffa199e3fbab8365778c4a10e1fbf1b9cd50707de826eb304b50e57ec0cc8d38"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.5.1"
+            "version": "==3.6.0"
         },
         "pluggy": {
             "hashes": [
                 "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
@@ -1088,14 +1182,21 @@
         "pycodestyle": {
             "hashes": [
                 "sha256:347187bdb476329d98f695c213d7295a846d1152ff4fe9bacb8a9590b8ee7053",
                 "sha256:8a4eaf0d0495c7395bdab3589ac2db602797d76207242c17d470186815706610"
             ],
             "version": "==2.10.0"
         },
+        "pycparser": {
+            "hashes": [
+                "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9",
+                "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"
+            ],
+            "version": "==2.21"
+        },
         "pydocstyle": {
             "hashes": [
                 "sha256:118762d452a49d6b05e194ef344a55822987a462831ade91ec5c06fd2169d019",
                 "sha256:7ce43f0c0ac87b07494eb9c0b462c0b73e6ff276807f204d6b53edc72b7e44e1"
             ],
             "version": "==6.3.0"
         },
@@ -1153,27 +1254,27 @@
                 "sha256:f271b298b97f5955d53fb12b72c1fb1948c22c1a6b70b315c54cedaca0264ef5"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.0.0"
         },
         "pytest": {
             "hashes": [
-                "sha256:3799fa815351fea3a5e96ac7e503a96fa51cc9942c3753cda7651b93c1cfa362",
-                "sha256:434afafd78b1d78ed0addf160ad2b77a30d35d4bdf8af234fe621919d9ed15e3"
+                "sha256:cdcbd012c9312258922f8cd3f1b62a6580fdced17db6014896053d47cddf9295",
+                "sha256:ee990a3cc55ba808b80795a79944756f315c67c12b56abd3ac993a7b8c17030b"
             ],
             "index": "pypi",
-            "version": "==7.3.1"
+            "version": "==7.3.2"
         },
         "pytest-mock": {
             "hashes": [
-                "sha256:f4c973eeae0282963eb293eb173ce91b091a79c1334455acfac9ddee8a1c784b",
-                "sha256:fbbdb085ef7c252a326fd8cdcac0aa3b1333d8811f131bdcc701002e1be7ed4f"
+                "sha256:21c279fff83d70763b05f8874cc9cfb3fcacd6d354247a976f9529d19f9acf39",
+                "sha256:7f6b125602ac6d743e523ae0bfa71e1a697a2f5534064528c6ff84c2f7c2fc7f"
             ],
             "index": "pypi",
-            "version": "==3.10.0"
+            "version": "==3.11.1"
         },
         "pytest-qt": {
             "hashes": [
                 "sha256:00a17b586dd530b6d7a9399923a40489ca4a9a309719011175f55dc6b5dc8f41",
                 "sha256:a7659960a1ab2af8fc944655a157ff45d714b80ed7a6af96a4b5bb99ecf40a22"
             ],
             "index": "pypi",
@@ -1206,27 +1307,27 @@
                 "sha256:a50f9dfe23b03a9d40414c1fdf902fefbeae12f2ac75a3c8f915944d6ffac279"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.2.5"
         },
         "pywin32-ctypes": {
             "hashes": [
-                "sha256:24ffc3b341d457d48e8922352130cf2644024a4ff09762a2261fd34c36ee5942",
-                "sha256:9dc2d991b3479cc2df15930958b674a48a227d5361d413827a4cfd0b5876fc98"
+                "sha256:934a2def1e5cbc472b2b6bf80680c0f03cd87df65dfd58bfd1846969de095b03",
+                "sha256:b9a53ef754c894a525469933ab2a447c74ec1ea6b9d2ef446f40ec50d3dcec9f"
             ],
             "index": "pypi",
-            "version": "==0.2.0"
+            "version": "==0.2.1"
         },
         "readme-renderer": {
             "hashes": [
-                "sha256:cd653186dfc73055656f090f227f5cb22a046d7f71a841dfa305f55c9a513273",
-                "sha256:f67a16caedfa71eef48a31b39708637a6f4664c4394801a7b0d6432d13907343"
+                "sha256:9f77b519d96d03d7d7dce44977ba543090a14397c4f60de5b6eb5b8048110aa4",
+                "sha256:e18feb2a1e7706f2865b81ebb460056d93fb29d69daa10b223c00faa7bd9a00a"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==37.3"
+            "markers": "python_version >= '3.8'",
+            "version": "==40.0"
         },
         "recommonmark": {
             "hashes": [
                 "sha256:1b1db69af0231efce3fa21b94ff627ea33dee7079a01dd0a7f8482c3da148b3f",
                 "sha256:bdb4db649f2222dcd8d2d844f0006b958d627f732415d399791ee436a3686d67"
             ],
             "index": "pypi",
@@ -1254,34 +1355,42 @@
                 "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
         "rich": {
             "hashes": [
-                "sha256:76f6b65ea7e5c5d924ba80e322231d7cb5b5981aa60bfc1e694f1bc097fe6fe1",
-                "sha256:d204aadb50b936bf6b1a695385429d192bc1fdaf3e8b907e8e26f4c4e4b5bf75"
+                "sha256:8f87bc7ee54675732fa66a05ebfe489e27264caeeff3728c945d25971b6485ec",
+                "sha256:d653d6bccede5844304c605d5aac802c7cf9621efd700b46c7ec2b51ea914898"
             ],
-            "markers": "python_full_version >= '3.7.0'",
-            "version": "==13.4.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==13.4.2"
         },
         "rope": {
             "hashes": [
                 "sha256:0767424ed40ce237dcf1c1f5088054fef960e5b19f4a0850783a259a3600d7bd",
                 "sha256:3de1d1f1cf2412540c6a150067fe25298175e7c2b72455b6ca8395f61678da82"
             ],
             "version": "==1.8.0"
         },
+        "secretstorage": {
+            "hashes": [
+                "sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77",
+                "sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99"
+            ],
+            "markers": "sys_platform == 'linux'",
+            "version": "==3.3.3"
+        },
         "setuptools": {
             "hashes": [
-                "sha256:5df61bf30bb10c6f756eb19e7c9f3b473051f48db77fddbe06ff2ca307df9a6f",
-                "sha256:62642358adc77ffa87233bc4d2354c4b2682d214048f500964dbe760ccedf102"
+                "sha256:11e52c67415a381d10d6b462ced9cfb97066179f0e871399e006c4ab101fc85f",
+                "sha256:baf1fdb41c6da4cd2eae722e135500da913332ab3f2f5c7d33af9b492acb5235"
             ],
             "index": "pypi",
-            "version": "==67.8.0"
+            "version": "==68.0.0"
         },
         "setuptools-scm": {
             "extras": [
                 "toml"
             ],
             "hashes": [
                 "sha256:6c508345a771aad7d56ebff0e70628bf2b0ec7573762be9960214730de278f27",
@@ -1398,90 +1507,86 @@
                 "sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==4.6.3"
         },
         "ujson": {
             "hashes": [
-                "sha256:00343501dbaa5172e78ef0e37f9ebd08040110e11c12420ff7c1f9f0332d939e",
-                "sha256:0e4e8981c6e7e9e637e637ad8ffe948a09e5434bc5f52ecbb82b4b4cfc092bfb",
-                "sha256:0ee295761e1c6c30400641f0a20d381633d7622633cdf83a194f3c876a0e4b7e",
-                "sha256:137831d8a0db302fb6828ee21c67ad63ac537bddc4376e1aab1c8573756ee21c",
-                "sha256:14f9082669f90e18e64792b3fd0bf19f2b15e7fe467534a35ea4b53f3bf4b755",
-                "sha256:16b2254a77b310f118717715259a196662baa6b1f63b1a642d12ab1ff998c3d7",
-                "sha256:18679484e3bf9926342b1c43a3bd640f93a9eeeba19ef3d21993af7b0c44785d",
-                "sha256:24ad1aa7fc4e4caa41d3d343512ce68e41411fb92adf7f434a4d4b3749dc8f58",
-                "sha256:26c2b32b489c393106e9cb68d0a02e1a7b9d05a07429d875c46b94ee8405bdb7",
-                "sha256:2f242eec917bafdc3f73a1021617db85f9958df80f267db69c76d766058f7b19",
-                "sha256:341f891d45dd3814d31764626c55d7ab3fd21af61fbc99d070e9c10c1190680b",
-                "sha256:35209cb2c13fcb9d76d249286105b4897b75a5e7f0efb0c0f4b90f222ce48910",
-                "sha256:3d3b3499c55911f70d4e074c626acdb79a56f54262c3c83325ffb210fb03e44d",
-                "sha256:4a3d794afbf134df3056a813e5c8a935208cddeae975bd4bc0ef7e89c52f0ce0",
-                "sha256:4c592eb91a5968058a561d358d0fef59099ed152cfb3e1cd14eee51a7a93879e",
-                "sha256:4ee997799a23227e2319a3f8817ce0b058923dbd31904761b788dc8f53bd3e30",
-                "sha256:523ee146cdb2122bbd827f4dcc2a8e66607b3f665186bce9e4f78c9710b6d8ab",
-                "sha256:54384ce4920a6d35fa9ea8e580bc6d359e3eb961fa7e43f46c78e3ed162d56ff",
-                "sha256:5593263a7fcfb934107444bcfba9dde8145b282de0ee9f61e285e59a916dda0f",
-                "sha256:581c945b811a3d67c27566539bfcb9705ea09cb27c4be0002f7a553c8886b817",
-                "sha256:5eba5e69e4361ac3a311cf44fa71bc619361b6e0626768a494771aacd1c2f09b",
-                "sha256:6411aea4c94a8e93c2baac096fbf697af35ba2b2ed410b8b360b3c0957a952d3",
-                "sha256:64772a53f3c4b6122ed930ae145184ebaed38534c60f3d859d8c3f00911eb122",
-                "sha256:67a19fd8e7d8cc58a169bea99fed5666023adf707a536d8f7b0a3c51dd498abf",
-                "sha256:6abb8e6d8f1ae72f0ed18287245f5b6d40094e2656d1eab6d99d666361514074",
-                "sha256:6e80f0d03e7e8646fc3d79ed2d875cebd4c83846e129737fdc4c2532dbd43d9e",
-                "sha256:6faf46fa100b2b89e4db47206cf8a1ffb41542cdd34dde615b2fc2288954f194",
-                "sha256:7312731c7826e6c99cdd3ac503cd9acd300598e7a80bcf41f604fee5f49f566c",
-                "sha256:75204a1dd7ec6158c8db85a2f14a68d2143503f4bafb9a00b63fe09d35762a5e",
-                "sha256:7592f40175c723c032cdbe9fe5165b3b5903604f774ab0849363386e99e1f253",
-                "sha256:7b9dc5a90e2149643df7f23634fe202fed5ebc787a2a1be95cf23632b4d90651",
-                "sha256:7df3fd35ebc14dafeea031038a99232b32f53fa4c3ecddb8bed132a43eefb8ad",
-                "sha256:800bf998e78dae655008dd10b22ca8dc93bdcfcc82f620d754a411592da4bbf2",
-                "sha256:8b4257307e3662aa65e2644a277ca68783c5d51190ed9c49efebdd3cbfd5fa44",
-                "sha256:90712dfc775b2c7a07d4d8e059dd58636bd6ff1776d79857776152e693bddea6",
-                "sha256:9b0f2680ce8a70f77f5d70aaf3f013d53e6af6d7058727a35d8ceb4a71cdd4e9",
-                "sha256:a5d2f44331cf04689eafac7a6596c71d6657967c07ac700b0ae1c921178645da",
-                "sha256:aae4d9e1b4c7b61780f0a006c897a4a1904f862fdab1abb3ea8f45bd11aa58f3",
-                "sha256:adf445a49d9a97a5a4c9bb1d652a1528de09dd1c48b29f79f3d66cea9f826bf6",
-                "sha256:af4639f684f425177d09ae409c07602c4096a6287027469157bfb6f83e01448b",
-                "sha256:afff311e9f065a8f03c3753db7011bae7beb73a66189c7ea5fcb0456b7041ea4",
-                "sha256:b01a9af52a0d5c46b2c68e3f258fdef2eacaa0ce6ae3e9eb97983f5b1166edb6",
-                "sha256:b522be14a28e6ac1cf818599aeff1004a28b42df4ed4d7bc819887b9dac915fc",
-                "sha256:b5ac3d5c5825e30b438ea92845380e812a476d6c2a1872b76026f2e9d8060fc2",
-                "sha256:b6a6961fc48821d84b1198a09516e396d56551e910d489692126e90bf4887d29",
-                "sha256:b7316d3edeba8a403686cdcad4af737b8415493101e7462a70ff73dd0609eafc",
-                "sha256:b738282e12a05f400b291966630a98d622da0938caa4bc93cf65adb5f4281c60",
-                "sha256:bab10165db6a7994e67001733f7f2caf3400b3e11538409d8756bc9b1c64f7e8",
-                "sha256:bea8d30e362180aafecabbdcbe0e1f0b32c9fa9e39c38e4af037b9d3ca36f50c",
-                "sha256:c0d1f7c3908357ee100aa64c4d1cf91edf99c40ac0069422a4fd5fd23b263263",
-                "sha256:c3af9f9f22a67a8c9466a32115d9073c72a33ae627b11de6f592df0ee09b98b6",
-                "sha256:c96e3b872bf883090ddf32cc41957edf819c5336ab0007d0cf3854e61841726d",
-                "sha256:cd90027e6d93e8982f7d0d23acf88c896d18deff1903dd96140613389b25c0dd",
-                "sha256:d2e43ccdba1cb5c6d3448eadf6fc0dae7be6c77e357a3abc968d1b44e265866d",
-                "sha256:d36a807a24c7d44f71686685ae6fbc8793d784bca1adf4c89f5f780b835b6243",
-                "sha256:d7ff6ebb43bc81b057724e89550b13c9a30eda0f29c2f506f8b009895438f5a6",
-                "sha256:d8cd622c069368d5074bd93817b31bdb02f8d818e57c29e206f10a1f9c6337dd",
-                "sha256:dda9aa4c33435147262cd2ea87c6b7a1ca83ba9b3933ff7df34e69fee9fced0c",
-                "sha256:e788e5d5dcae8f6118ac9b45d0b891a0d55f7ac480eddcb7f07263f2bcf37b23",
-                "sha256:e87cec407ec004cf1b04c0ed7219a68c12860123dfb8902ef880d3d87a71c172",
-                "sha256:ea7423d8a2f9e160c5e011119741682414c5b8dce4ae56590a966316a07a4618",
-                "sha256:ed22f9665327a981f288a4f758a432824dc0314e4195a0eaeb0da56a477da94d",
-                "sha256:ed24406454bb5a31df18f0a423ae14beb27b28cdfa34f6268e7ebddf23da807e",
-                "sha256:f7f241488879d91a136b299e0c4ce091996c684a53775e63bb442d1a8e9ae22a",
-                "sha256:ff0004c3f5a9a6574689a553d1b7819d1a496b4f005a7451f339dc2d9f4cf98c"
+                "sha256:07d459aca895eb17eb463b00441986b021b9312c6c8cc1d06880925c7f51009c",
+                "sha256:0be81bae295f65a6896b0c9030b55a106fb2dec69ef877253a87bc7c9c5308f7",
+                "sha256:0fe1b7edaf560ca6ab023f81cbeaf9946a240876a993b8c5a21a1c539171d903",
+                "sha256:102bf31c56f59538cccdfec45649780ae00657e86247c07edac434cb14d5388c",
+                "sha256:11da6bed916f9bfacf13f4fc6a9594abd62b2bb115acfb17a77b0f03bee4cfd5",
+                "sha256:16fde596d5e45bdf0d7de615346a102510ac8c405098e5595625015b0d4b5296",
+                "sha256:193349a998cd821483a25f5df30b44e8f495423840ee11b3b28df092ddfd0f7f",
+                "sha256:20768961a6a706170497129960762ded9c89fb1c10db2989c56956b162e2a8a3",
+                "sha256:27a2a3c7620ebe43641e926a1062bc04e92dbe90d3501687957d71b4bdddaec4",
+                "sha256:2873d196725a8193f56dde527b322c4bc79ed97cd60f1d087826ac3290cf9207",
+                "sha256:299a312c3e85edee1178cb6453645217ba23b4e3186412677fa48e9a7f986de6",
+                "sha256:2a64cc32bb4a436e5813b83f5aab0889927e5ea1788bf99b930fad853c5625cb",
+                "sha256:2b852bdf920fe9f84e2a2c210cc45f1b64f763b4f7d01468b33f7791698e455e",
+                "sha256:2e72ba76313d48a1a3a42e7dc9d1db32ea93fac782ad8dde6f8b13e35c229130",
+                "sha256:3659deec9ab9eb19e8646932bfe6fe22730757c4addbe9d7d5544e879dc1b721",
+                "sha256:3b27a8da7a080add559a3b73ec9ebd52e82cc4419f7c6fb7266e62439a055ed0",
+                "sha256:3f9b63530a5392eb687baff3989d0fb5f45194ae5b1ca8276282fb647f8dcdb3",
+                "sha256:407d60eb942c318482bbfb1e66be093308bb11617d41c613e33b4ce5be789adc",
+                "sha256:40931d7c08c4ce99adc4b409ddb1bbb01635a950e81239c2382cfe24251b127a",
+                "sha256:48c7d373ff22366eecfa36a52b9b55b0ee5bd44c2b50e16084aa88b9de038916",
+                "sha256:4ddeabbc78b2aed531f167d1e70387b151900bc856d61e9325fcdfefb2a51ad8",
+                "sha256:5ac97b1e182d81cf395ded620528c59f4177eee024b4b39a50cdd7b720fdeec6",
+                "sha256:5ce24909a9c25062e60653073dd6d5e6ec9d6ad7ed6e0069450d5b673c854405",
+                "sha256:69b3104a2603bab510497ceabc186ba40fef38ec731c0ccaa662e01ff94a985c",
+                "sha256:6a4dafa9010c366589f55afb0fd67084acd8added1a51251008f9ff2c3e44042",
+                "sha256:6d230d870d1ce03df915e694dcfa3f4e8714369cce2346686dbe0bc8e3f135e7",
+                "sha256:78e318def4ade898a461b3d92a79f9441e7e0e4d2ad5419abed4336d702c7425",
+                "sha256:7a42baa647a50fa8bed53d4e242be61023bd37b93577f27f90ffe521ac9dc7a3",
+                "sha256:7cba16b26efe774c096a5e822e4f27097b7c81ed6fb5264a2b3f5fd8784bab30",
+                "sha256:7d8283ac5d03e65f488530c43d6610134309085b71db4f675e9cf5dff96a8282",
+                "sha256:7ecc33b107ae88405aebdb8d82c13d6944be2331ebb04399134c03171509371a",
+                "sha256:9249fdefeb021e00b46025e77feed89cd91ffe9b3a49415239103fc1d5d9c29a",
+                "sha256:9399eaa5d1931a0ead49dce3ffacbea63f3177978588b956036bfe53cdf6af75",
+                "sha256:94c7bd9880fa33fcf7f6d7f4cc032e2371adee3c5dba2922b918987141d1bf07",
+                "sha256:9571de0c53db5cbc265945e08f093f093af2c5a11e14772c72d8e37fceeedd08",
+                "sha256:9721cd112b5e4687cb4ade12a7b8af8b048d4991227ae8066d9c4b3a6642a582",
+                "sha256:9ab282d67ef3097105552bf151438b551cc4bedb3f24d80fada830f2e132aeb9",
+                "sha256:9d9707e5aacf63fb919f6237d6490c4e0244c7f8d3dc2a0f84d7dec5db7cb54c",
+                "sha256:a70f776bda2e5072a086c02792c7863ba5833d565189e09fabbd04c8b4c3abba",
+                "sha256:a89cf3cd8bf33a37600431b7024a7ccf499db25f9f0b332947fbc79043aad879",
+                "sha256:a8c91b6f4bf23f274af9002b128d133b735141e867109487d17e344d38b87d94",
+                "sha256:ad24ec130855d4430a682c7a60ca0bc158f8253ec81feed4073801f6b6cb681b",
+                "sha256:ae7f4725c344bf437e9b881019c558416fe84ad9c6b67426416c131ad577df67",
+                "sha256:b748797131ac7b29826d1524db1cc366d2722ab7afacc2ce1287cdafccddbf1f",
+                "sha256:bdf04c6af3852161be9613e458a1fb67327910391de8ffedb8332e60800147a2",
+                "sha256:bf5737dbcfe0fa0ac8fa599eceafae86b376492c8f1e4b84e3adf765f03fb564",
+                "sha256:c4e7bb7eba0e1963f8b768f9c458ecb193e5bf6977090182e2b4f4408f35ac76",
+                "sha256:d524a8c15cfc863705991d70bbec998456a42c405c291d0f84a74ad7f35c5109",
+                "sha256:d53039d39de65360e924b511c7ca1a67b0975c34c015dd468fca492b11caa8f7",
+                "sha256:d6f84a7a175c75beecde53a624881ff618e9433045a69fcfb5e154b73cdaa377",
+                "sha256:e0147d41e9fb5cd174207c4a2895c5e24813204499fd0839951d4c8784a23bf5",
+                "sha256:e3673053b036fd161ae7a5a33358ccae6793ee89fd499000204676baafd7b3aa",
+                "sha256:e54578fa8838ddc722539a752adfce9372474114f8c127bb316db5392d942f8b",
+                "sha256:eb0142f6f10f57598655340a3b2c70ed4646cbe674191da195eb0985a9813b83",
+                "sha256:efeddf950fb15a832376c0c01d8d7713479fbeceaed1eaecb2665aa62c305aec",
+                "sha256:f26629ac531d712f93192c233a74888bc8b8212558bd7d04c349125f10199fcf",
+                "sha256:f2e385a7679b9088d7bc43a64811a7713cc7c33d032d020f757c54e7d41931ae",
+                "sha256:f3554eaadffe416c6f543af442066afa6549edbc34fe6a7719818c3e72ebfe95",
+                "sha256:f4511560d75b15ecb367eef561554959b9d49b6ec3b8d5634212f9fed74a6df1",
+                "sha256:f504117a39cb98abba4153bf0b46b4954cc5d62f6351a14660201500ba31fe7f",
+                "sha256:fb87decf38cc82bcdea1d7511e73629e651bdec3a43ab40985167ab8449b769c"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==5.7.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==5.8.0"
         },
         "urllib3": {
             "hashes": [
-                "sha256:61717a1095d7e155cdb737ac7bb2f4324a858a1e2e6466f6d03ff630ca68d3cc",
-                "sha256:d055c2f9d38dc53c808f6fdc8eab7360b6fdbbde02340ed25cfbcd817c62469e"
+                "sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1",
+                "sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.0.2"
+            "version": "==2.0.3"
         },
         "webencodings": {
             "hashes": [
                 "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78",
                 "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"
             ],
             "version": "==0.5.1"
@@ -1572,18 +1677,18 @@
                 "sha256:fd69666217b62fa5d7c6aa88e507493a34dec4fa20c5bd925e4bc12fce586639"
             ],
             "markers": "python_version < '3.11'",
             "version": "==1.15.0"
         },
         "yapf": {
             "hashes": [
-                "sha256:4c2b59bd5ffe46f3a7da48df87596877189148226ce267c16e8b44240e51578d",
-                "sha256:da62bdfea3df3673553351e6246abed26d9fe6780e548a5af9e70f6d2b4f5b9a"
+                "sha256:958587eb5c8ec6c860119a9c25d02addf30a44f75aa152a4220d30e56a98037c",
+                "sha256:b8bfc1f280949153e795181768ca14ef43d7312629a06c43e7abd279323af313"
             ],
-            "version": "==0.33.0"
+            "version": "==0.40.1"
         },
         "zipp": {
             "hashes": [
                 "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
                 "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
             ],
             "markers": "python_version >= '3.7'",
```

### Comparing `blackboardsync-0.8.5rc4/README.md` & `blackboardsync-0.9.0a1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # BlackboardSync
 ### Automatic Syncing Of Your Blackboard Content
 
-[![License: GPL  v2][license-shield]][gnu] [![Build][build-shield]][actions]
+[![Get on PyPI][pypi-shield]][pypi] [![License: GPL  v2][license-shield]][gnu] [![Build][build-shield]][actions]
 
 **BlackboardSync** performs a periodic, incremental download of all your Blackboard content, such as lecture slides, lab sheets, and other attachments.
 
 
 <div align="center">
 	<img src="https://raw.githubusercontent.com/jacobszpz/BlackboardSync/main/blackboard_sync/assets/logo.png" height="auto" width="25%" />
 </div>
@@ -50,18 +50,23 @@
 
 
 
 ## Installation
 
 #### Binaries
 
-Currently unavailable (until a more stable version).
+You can find all releases on [GitHub][releases].
+Only MacOS (.dmg) and Windows (.exe) are supported at the moment.
 
-Alternatively, you can run the python package [directly](#running-without-building), or build an executable yourself by following [these steps](#building-from-source).
+Note: These releases are automatically built on GitHub Actions from source.
 
+**⚠️ ATTENTION MACOS USERS **
+
+On MacOS, you will face an issue when trying to open the application, since it has not
+been notarised by Apple. A workaround can be found [here][apple-dev].
 
 
 #### From PyPI
 
 ```bash
 python3 -m pip install blackboardsync
 ```
@@ -157,14 +162,15 @@
 
 
 
 <!-- LINK REFERENCES -->
 
 [universal-login]: https://github.com/jacobszpz/BlackboardSync/issues/3	"BBSync login"
 [pyqt]: https://pypi.org/project/PyQt5/5.15.1/	"Python Bindings for Qt 5"
+[pypi]: https://pypi.org/project/blackboardsync
 [typora]: https://typora.io/ "Typora"
 [releases]: https://github.com/jacobszpz/BlackboardSync/releases "BlackboardSync Releases"
 [issues]: https://github.com/jacobszpz/BlackboardSync/issues/new "BlackboardSync Issues"
 [git]: https://git-scm.com/	"Git"
 [python]: https://www.python.org/ "Python.org"
 [pipenv]: https://pipenv.pypa.io/en/latest/ "Pipenv"
 [license]: LICENSE "General Public License"
@@ -173,27 +179,28 @@
 [pyinstaller]: https://www.pyinstaller.org/	"PyInstaller"
 
 
 
 <!-- RELEASES -->
 
 [releases]: https://github.com/jacobszpz/BlackboardSync/releases/
+[apple-dev]: https://support.apple.com/en-gb/guide/mac-help/mh40616/mac
 
 
 <!-- README TEMPLATES -->
 
 [tonycrosby]: https://gist.github.com/tonycrosby-tech/c18c2b6c74900c6080fc097ca0718839	"tonycrosby-tech README template"
 [neildrew]: https://github.com/othneildrew/Best-README-Template	"othneildrew README template"
 [bulldogjob]: https://bulldogjob.com/news/449-how-to-write-a-good-readme-for-your-github-project	"bulldogjob README guide"
 
 
 
 <!-- SHIELDS -->
 
-[version-shield]: https://img.shields.io/pypi/v/BlackboardSync
+[pypi-shield]: https://img.shields.io/pypi/v/BlackboardSync
 [license-shield]: https://img.shields.io/github/license/jacobszpz/BlackboardSync
 [build-shield]: https://img.shields.io/github/actions/workflow/status/jacobszpz/BlackboardSync/build.yml?branch=main
 [kofi-shield]: https://ko-fi.com/img/githubbutton_sm.svg
 [lp-shield]: https://img.shields.io/liberapay/receives/BlackboardSync.svg?logo=liberapay
```

### Comparing `blackboardsync-0.8.5rc4/blackboard_sync/__about__.py` & `blackboardsync-0.9.0a1/blackboard_sync/__about__.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,14 +29,14 @@
     "__copyright__",
 ]
 
 __title__ = "BlackboardSync"
 __summary__ = "Automatic Syncing Of Your Blackboard Content"
 __uri__ = "https://github.com/jacobszpz/BlackboardSync"
 
-__version__ = "0.8.5-rc.4"
+__version__ = "0.9.0-alpha.1"
 
 __author__ = "Jacob Sánchez"
 __email__ = "jacobszpz@protonmail.com"
 
 __license__ = "GNU General Public License v2"
 __copyright__ = f"2023, {__author__}"
```

### Comparing `blackboardsync-0.8.5rc4/blackboard_sync/__init__.py` & `blackboardsync-0.9.0a1/blackboard_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/blackboard_sync/__main__.py` & `blackboardsync-0.9.0a1/blackboard_sync/__main__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/blackboard_sync/assets/alert.png` & `blackboardsync-0.9.0a1/blackboard_sync/assets/alert.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/blackboard_sync/assets/alert.svg` & `blackboardsync-0.9.0a1/blackboard_sync/assets/alert.svg`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/blackboard_sync/assets/logo.ico` & `blackboardsync-0.9.0a1/blackboard_sync/assets/logo.ico`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/blackboard_sync/assets/logo.png` & `blackboardsync-0.9.0a1/blackboard_sync/assets/logo.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/blackboard_sync/assets/watermark.png` & `blackboardsync-0.9.0a1/blackboard_sync/assets/watermark.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/blackboard_sync/blackboard/__init__.py` & `blackboardsync-0.9.0a1/blackboard_sync/blackboard/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/blackboard_sync/blackboard/api.py` & `blackboardsync-0.9.0a1/blackboard_sync/blackboard/api.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/blackboard_sync/blackboard/blackboard.py` & `blackboardsync-0.9.0a1/blackboard_sync/blackboard/blackboard.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/blackboard_sync/config.py` & `blackboardsync-0.9.0a1/blackboard_sync/config.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/blackboard_sync/download.py` & `blackboardsync-0.9.0a1/blackboard_sync/download.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,22 +36,21 @@
 from .webdav import ContentParser, Link, validate_webdav_response
 
 
 class BlackboardDownload:
     """Blackboard download job."""
 
     _last_downloaded = datetime.fromtimestamp(0, tz=timezone.utc)
-    _data_source = "_21_1"
 
     _logger = logging.getLogger(__name__)
     _logger.setLevel(logging.DEBUG)
     _logger.addHandler(logging.StreamHandler())
 
     def __init__(self, sess: BlackboardSession, download_location: Path,
-                 last_downloaded: datetime = None):
+                 last_downloaded: datetime = None, data_sources: list[str] = []):
         """BlackboardDownload constructor
 
         Download all files in blackboard recursively to download_location,
         only if they have been altered since specified datetime
 
         Keyword arguments:
 
@@ -59,14 +58,15 @@
         :param (str / Path) download_location: Where files will be stored
         :param str last_downloaded: Files modified before this will not be downloaded
         """
 
         self._sess = sess
         self._user_id = sess.username
         self._download_location = download_location
+        self._data_sources = data_sources
         self._files_processed = 0
         self.executor = ThreadPoolExecutor(max_workers=8)
         self.cancelled = False
 
         if last_downloaded is not None:
             self._last_downloaded = last_downloaded
 
@@ -188,18 +188,21 @@
         """
         if self.cancelled:
             return None
 
         start_time = datetime.now(timezone.utc)
 
         self.logger.info("Fetching user memberships")
-        memberships = self._sess.fetch_user_memberships(user_id=self.user_id,
-                                                        dataSourceId=self._data_source)
-        for ms in memberships:
 
+        memberships = self._sess.fetch_user_memberships(user_id=self.user_id)
+
+        if self._data_sources:
+            memberships = [m for m in memberships if m.dataSourceId in self._data_sources]
+
+        for ms in memberships:
             if self.cancelled:
                 break
 
             private = False
             self.logger.debug("Fetching course")
             try:
                 course = self._sess.fetch_courses(course_id=ms.courseId)
@@ -233,21 +236,21 @@
 
     @property
     def download_location(self) -> str:
         """The location where files will be downloaded to."""
         return self._download_location
 
     @property
-    def data_source(self) -> str:
+    def data_sources(self) -> list[str]:
         """Filter for courses."""
-        return self._data_source
+        return self._data_sources
 
-    @data_source.setter
-    def data_source(self, source: str) -> None:
-        self._data_source = source
+    @data_sources.setter
+    def data_sources(self, sources: list[str]) -> None:
+        self._data_sources = sources
 
     @property
     def user_id(self) -> str:
         """User ID used for API calls."""
         return self._user_id
 
     @property
```

### Comparing `blackboardsync-0.8.5rc4/blackboard_sync/institutions.py` & `blackboardsync-0.9.0a1/blackboard_sync/institutions.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/blackboard_sync/qt/LoginWebView.ui` & `blackboardsync-0.9.0a1/blackboard_sync/qt/LoginWebView.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/blackboard_sync/qt/PersistenceWarning.ui` & `blackboardsync-0.9.0a1/blackboard_sync/qt/PersistenceWarning.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/blackboard_sync/qt/SettingsWindow.ui` & `blackboardsync-0.9.0a1/blackboard_sync/qt/SettingsWindow.ui`

 * *Files 7% similar despite different names*

#### Comparing `blackboardsync-0.8.5rc4/blackboard_sync/qt/SettingsWindow.ui` & `blackboardsync-0.9.0a1/blackboard_sync/qt/SettingsWindow.ui`

```diff
@@ -185,56 +185,14 @@
                   <width>0</width>
                   <height>18</height>
                 </size>
               </property>
             </spacer>
           </item>
           <item>
-            <widget class="QLabel" name="data_source_label">
-              <property name="font">
-                <font>
-                  <family>Open Sans</family>
-                  <pointsize>11</pointsize>
-                </font>
-              </property>
-              <property name="text">
-                <string>Data Source</string>
-              </property>
-            </widget>
-          </item>
-          <item>
-            <widget class="QLineEdit" name="data_source_edit">
-              <property name="enabled">
-                <bool>false</bool>
-              </property>
-              <property name="font">
-                <font>
-                  <family>Open Sans</family>
-                  <pointsize>11</pointsize>
-                </font>
-              </property>
-            </widget>
-          </item>
-          <item>
-            <spacer name="verticalSpacer_5">
-              <property name="orientation">
-                <enum>Qt::Vertical</enum>
-              </property>
-              <property name="sizeType">
-                <enum>QSizePolicy::Fixed</enum>
-              </property>
-              <property name="sizeHint" stdset="0">
-                <size>
-                  <width>0</width>
-                  <height>18</height>
-                </size>
-              </property>
-            </spacer>
-          </item>
-          <item>
             <widget class="QLabel" name="session_label">
               <property name="font">
                 <font>
                   <family>Open Sans</family>
                   <pointsize>11</pointsize>
                 </font>
               </property>
```

### Comparing `blackboardsync-0.8.5rc4/blackboard_sync/qt/SetupWizard.ui` & `blackboardsync-0.9.0a1/blackboard_sync/qt/SetupWizard.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/blackboard_sync/qt/UniNotSupportedDialog.ui` & `blackboardsync-0.9.0a1/blackboard_sync/qt/UniNotSupportedDialog.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/blackboard_sync/qt/__init__.py` & `blackboardsync-0.9.0a1/blackboard_sync/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/blackboard_sync/qt/qt_elements.py` & `blackboardsync-0.9.0a1/blackboard_sync/qt/qt_elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -401,23 +401,14 @@
 
     @download_location.setter
     def download_location(self, location: Path) -> None:
         self._download_location = location.resolve()
         self.download_location_hint.setText(str(self._download_location))
 
     @property
-    def data_source(self) -> str:
-        """Filter which Blackboard source to download."""
-        return self.data_source_edit.text()
-
-    @data_source.setter
-    def data_source(self, data_source: str) -> None:
-        self.data_source_edit.setText(data_source)
-
-    @property
     def sync_frequency(self) -> int:
         """Seconds to wait between each sync job."""
         return int([*SyncPeriod][self.frequency_combo.currentIndex()])
 
     @sync_frequency.setter
     def sync_frequency(self, f: int) -> None:
         self.frequency_combo.setCurrentIndex([*SyncPeriod].index(SyncPeriod(f)))
```

### Comparing `blackboardsync-0.8.5rc4/blackboard_sync/sync.py` & `blackboardsync-0.9.0a1/blackboard_sync/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,14 @@
 
 class BlackboardSync:
     """Represents an instance of the BlackboardSync application."""
 
     _log_directory = "log"
     _app_name = 'blackboard_sync'
 
-    # Filters out non-subjects from blackboard (may need more testing)
-    _data_source = "_21_1"
-
     # Seconds between each check of time elapsed since last sync
     _check_sleep_time = 10
     # Sync thread max retries
     _max_retries = 3
 
     _logger = logging.getLogger(__name__)
 
@@ -143,15 +140,15 @@
 
         while self._is_active:
             if self.outdated or self._force_sync:
                 self.logger.debug("Syncing now")
                 self._is_syncing = True
 
                 # Download from last datetime
-                self._download = BlackboardDownload(self.sess, self.download_location / '', self.last_sync_time)
+                self._download = BlackboardDownload(self.sess, self.download_location / '', self.last_sync_time, self.university.data_sources)
 
                 try:
                     if not self._is_active:
                         self._download.cancel()
                     job_start_time = self._download.download()
                     if job_start_time is not None:
                         self.last_sync_time = job_start_time
@@ -245,25 +242,14 @@
     def outdated(self) -> bool:
         """Return true if last download job is outdated."""
         if self._config.last_sync_time is None:
             return True
         return datetime.now(timezone.utc) >= self.next_sync
 
     @property
-    def data_source(self) -> str:
-        """Filter the modules to download."""
-        # The default works in my testing. However, this might need tweaking for other users,
-        # specially if used for different institutions than UCLan.
-        return self._data_source
-
-    @data_source.setter
-    def data_source(self, d: str) -> None:
-        self._data_source = d
-
-    @property
     def university_index(self):
         return self._config.university_index
 
     @university_index.setter
     def university_index(self, uni_index: int) -> None:
         self._config.university_index = uni_index
         self.university = get_by_index(uni_index)
```

### Comparing `blackboardsync-0.8.5rc4/blackboard_sync/sync_controller.py` & `blackboardsync-0.9.0a1/blackboard_sync/sync_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -113,15 +113,14 @@
 
     def _show_setup_window(self) -> None:
         self._show_window(self.setup_window)
 
     def _show_config_window(self) -> None:
         # Update displayed settings
         self.config_window.download_location = self.model.download_location
-        self.config_window.data_source = self.model.data_source
         self.config_window.username = self.model.username.split(':')[1]
         self.config_window.sync_frequency = self.model.sync_interval
         self._show_window(self.config_window)
 
     def _show_window(self, window: QWindow) -> None:
         window.setWindowState(Qt.WindowNoState)
         window.show()
@@ -149,15 +148,14 @@
     def _save_setting_changes(self) -> None:
         self.config_window.setVisible(False)
 
         if self.model.download_location != self.config_window.download_location:
             redownload = RedownloadDialog().redownload
             self.model.change_download_location(self.config_window.download_location, redownload)
 
-        self.model.data_source = self.config_window.data_source
         self.model.sync_interval = self.config_window.sync_frequency
 
     def _force_sync(self) -> None:
         self.model.force_sync()
 
     def _update_tray_menu(self) -> None:
         # Update last sync time
```

### Comparing `blackboardsync-0.8.5rc4/blackboard_sync/updates.py` & `blackboardsync-0.9.0a1/blackboard_sync/updates.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/blackboard_sync/webdav.py` & `blackboardsync-0.9.0a1/blackboard_sync/webdav.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/blackboardsync.egg-info/PKG-INFO` & `blackboardsync-0.9.0a1/blackboardsync.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboardsync
-Version: 0.8.5rc4
+Version: 0.9.0a1
 Summary: Sync your blackboard content to your device
 Author-email: Jacob Sánchez <jacobszpz@protonmail.com>
 Project-URL: Homepage, https://bbsync.app
 Project-URL: Repository, https://github.com/jacobszpz/BlackboardSync
 Project-URL: Bug Tracker, https://github.com/jacobszpz/BlackboardSync/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -14,15 +14,15 @@
 Provides-Extra: test
 Provides-Extra: package
 License-File: LICENSE
 
 # BlackboardSync
 ### Automatic Syncing Of Your Blackboard Content
 
-[![License: GPL  v2][license-shield]][gnu] [![Build][build-shield]][actions]
+[![Get on PyPI][pypi-shield]][pypi] [![License: GPL  v2][license-shield]][gnu] [![Build][build-shield]][actions]
 
 **BlackboardSync** performs a periodic, incremental download of all your Blackboard content, such as lecture slides, lab sheets, and other attachments.
 
 
 <div align="center">
 	<img src="https://raw.githubusercontent.com/jacobszpz/BlackboardSync/main/blackboard_sync/assets/logo.png" height="auto" width="25%" />
 </div>
@@ -67,18 +67,23 @@
 
 
 
 ## Installation
 
 #### Binaries
 
-Currently unavailable (until a more stable version).
+You can find all releases on [GitHub][releases].
+Only MacOS (.dmg) and Windows (.exe) are supported at the moment.
 
-Alternatively, you can run the python package [directly](#running-without-building), or build an executable yourself by following [these steps](#building-from-source).
+Note: These releases are automatically built on GitHub Actions from source.
 
+**⚠️ ATTENTION MACOS USERS **
+
+On MacOS, you will face an issue when trying to open the application, since it has not
+been notarised by Apple. A workaround can be found [here][apple-dev].
 
 
 #### From PyPI
 
 ```bash
 python3 -m pip install blackboardsync
 ```
@@ -174,14 +179,15 @@
 
 
 
 <!-- LINK REFERENCES -->
 
 [universal-login]: https://github.com/jacobszpz/BlackboardSync/issues/3	"BBSync login"
 [pyqt]: https://pypi.org/project/PyQt5/5.15.1/	"Python Bindings for Qt 5"
+[pypi]: https://pypi.org/project/blackboardsync
 [typora]: https://typora.io/ "Typora"
 [releases]: https://github.com/jacobszpz/BlackboardSync/releases "BlackboardSync Releases"
 [issues]: https://github.com/jacobszpz/BlackboardSync/issues/new "BlackboardSync Issues"
 [git]: https://git-scm.com/	"Git"
 [python]: https://www.python.org/ "Python.org"
 [pipenv]: https://pipenv.pypa.io/en/latest/ "Pipenv"
 [license]: LICENSE "General Public License"
@@ -190,27 +196,28 @@
 [pyinstaller]: https://www.pyinstaller.org/	"PyInstaller"
 
 
 
 <!-- RELEASES -->
 
 [releases]: https://github.com/jacobszpz/BlackboardSync/releases/
+[apple-dev]: https://support.apple.com/en-gb/guide/mac-help/mh40616/mac
 
 
 <!-- README TEMPLATES -->
 
 [tonycrosby]: https://gist.github.com/tonycrosby-tech/c18c2b6c74900c6080fc097ca0718839	"tonycrosby-tech README template"
 [neildrew]: https://github.com/othneildrew/Best-README-Template	"othneildrew README template"
 [bulldogjob]: https://bulldogjob.com/news/449-how-to-write-a-good-readme-for-your-github-project	"bulldogjob README guide"
 
 
 
 <!-- SHIELDS -->
 
-[version-shield]: https://img.shields.io/pypi/v/BlackboardSync
+[pypi-shield]: https://img.shields.io/pypi/v/BlackboardSync
 [license-shield]: https://img.shields.io/github/license/jacobszpz/BlackboardSync
 [build-shield]: https://img.shields.io/github/actions/workflow/status/jacobszpz/BlackboardSync/build.yml?branch=main
 [kofi-shield]: https://ko-fi.com/img/githubbutton_sm.svg
 [lp-shield]: https://img.shields.io/liberapay/receives/BlackboardSync.svg?logo=liberapay
```

### Comparing `blackboardsync-0.8.5rc4/blackboardsync.egg-info/SOURCES.txt` & `blackboardsync-0.9.0a1/blackboardsync.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 LICENSE
 Pipfile
 Pipfile.lock
 README.md
 UNIVERSITIES.md
 main.py
 pyproject.toml
-setup.cfg
+.github/FUNDING.yml
 .github/dependabot.yml
+.github/ISSUE_TEMPLATE/unisupport.yml
 .github/workflows/build.yml
 blackboard_sync/__about__.py
 blackboard_sync/__init__.py
 blackboard_sync/__main__.py
 blackboard_sync/config.py
 blackboard_sync/download.py
 blackboard_sync/institutions.py
```

### Comparing `blackboardsync-0.8.5rc4/docs/Makefile` & `blackboardsync-0.9.0a1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/docs/conf.py` & `blackboardsync-0.9.0a1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/docs/index.rst` & `blackboardsync-0.9.0a1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/docs/make.bat` & `blackboardsync-0.9.0a1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/main.py` & `blackboardsync-0.9.0a1/main.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/packaging/pkg_macos.sh` & `blackboardsync-0.9.0a1/packaging/pkg_macos.sh`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/packaging/pkg_win.nsi` & `blackboardsync-0.9.0a1/packaging/pkg_win.nsi`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/packaging/pyinst.py` & `blackboardsync-0.9.0a1/packaging/pyinst.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/pyproject.toml` & `blackboardsync-0.9.0a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/tests/strategies.py` & `blackboardsync-0.9.0a1/tests/strategies.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/tests/test_api.py` & `blackboardsync-0.9.0a1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/tests/test_blackboard.py` & `blackboardsync-0.9.0a1/tests/test_blackboard.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/tests/test_download.py` & `blackboardsync-0.9.0a1/tests/test_download.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,29 +101,25 @@
             assert link_file.read() == contents
 
 def test_download_location(mock_session, tmp_path):
     download = BlackboardDownload(mock_session, tmp_path)
     assert download.download_location == tmp_path
     assert tmp_path.exists()
 
-def test_default_data_source(mock_session, tmp_path):
-    download = BlackboardDownload(mock_session, tmp_path)
-    assert download.data_source == '_21_1'
-
 def test_logger(mock_session, tmp_path):
     download = BlackboardDownload(mock_session, tmp_path)
     assert isinstance(download.logger, logging.Logger)
 
 def test_download_method_call_fetch_user_memberships_with_username(mock_session, tmp_path):
     expected_user = "test_username"
     mock_session.fetch_user_memberships.return_value = []
     mock_session.username = expected_user
     download = BlackboardDownload(mock_session, tmp_path)
     download.download()
-    mock_session.fetch_user_memberships.assert_called_once_with(user_id=expected_user, dataSourceId=ANY)
+    mock_session.fetch_user_memberships.assert_called_once_with(user_id=expected_user)
 
 def test_download_method_call_fetch_courses_skip_private(mock_session, tmp_path):
     expected_course_id = 'TEST_BBC_ID'
     mock_session.fetch_courses.side_effect = ValueError('Private course')
     download = BlackboardDownload(mock_session, tmp_path)
     download.download()
     mock_session.fetch_courses.assert_called_once_with(course_id=expected_course_id)
```

### Comparing `blackboardsync-0.8.5rc4/tests/test_qt.py` & `blackboardsync-0.9.0a1/tests/test_qt.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc4/tests/test_sync_config.py` & `blackboardsync-0.9.0a1/tests/test_sync_config.py`

 * *Files identical despite different names*

