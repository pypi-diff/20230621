# Comparing `tmp/sett-4.2.0.tar.gz` & `tmp/sett-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sett-4.2.0.tar", last modified: Thu Apr  6 14:02:37 2023, max compression
+gzip compressed data, was "sett-4.3.0.tar", last modified: Wed Jun 21 12:22:40 2023, max compression
```

## Comparing `sett-4.2.0.tar` & `sett-4.3.0.tar`

### file list

```diff
@@ -1,78 +1,80 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 14:02:37.100698 sett-4.2.0/
--rw-rw-rw-   0 root         (0) root         (0)    35149 2023-04-06 14:02:23.000000 sett-4.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3072 2023-04-06 14:02:37.100698 sett-4.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1852 2023-04-06 14:02:23.000000 sett-4.2.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1992 2023-04-06 14:02:23.000000 sett-4.2.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 14:02:37.081696 sett-4.2.0/sett/
--rw-rw-rw-   0 root         (0) root         (0)     2444 2023-04-06 14:02:23.000000 sett-4.2.0/sett/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 14:02:37.084697 sett-4.2.0/sett/cli/
--rw-rw-rw-   0 root         (0) root         (0)    12781 2023-04-06 14:02:23.000000 sett-4.2.0/sett/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18796 2023-04-06 14:02:23.000000 sett-4.2.0/sett/cli/cli_builder.py
--rw-rw-rw-   0 root         (0) root         (0)     3394 2023-04-06 14:02:23.000000 sett-4.2.0/sett/cli/progress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 14:02:37.087697 sett-4.2.0/sett/core/
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-04-06 14:02:23.000000 sett-4.2.0/sett/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9765 2023-04-06 14:02:23.000000 sett-4.2.0/sett/core/archive.py
--rw-rw-rw-   0 root         (0) root         (0)     6613 2023-04-06 14:02:23.000000 sett-4.2.0/sett/core/checksum.py
--rw-rw-rw-   0 root         (0) root         (0)    15030 2023-04-06 14:02:23.000000 sett-4.2.0/sett/core/crypt.py
--rw-rw-rw-   0 root         (0) root         (0)      442 2023-04-06 14:02:23.000000 sett-4.2.0/sett/core/error.py
--rw-rw-rw-   0 root         (0) root         (0)     6635 2023-04-06 14:02:23.000000 sett-4.2.0/sett/core/filesystem.py
--rw-rw-rw-   0 root         (0) root         (0)      651 2023-04-06 14:02:23.000000 sett-4.2.0/sett/core/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     2046 2023-04-06 14:02:23.000000 sett-4.2.0/sett/core/request.py
--rw-rw-rw-   0 root         (0) root         (0)     1448 2023-04-06 14:02:23.000000 sett-4.2.0/sett/core/secret.py
--rw-rw-rw-   0 root         (0) root         (0)     2147 2023-04-06 14:02:23.000000 sett-4.2.0/sett/core/versioncheck.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 14:02:37.092697 sett-4.2.0/sett/gui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-06 14:02:23.000000 sett-4.2.0/sett/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2451 2023-04-06 14:02:23.000000 sett-4.2.0/sett/gui/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)    15705 2023-04-06 14:02:23.000000 sett-4.2.0/sett/gui/component.py
--rw-rw-rw-   0 root         (0) root         (0)     3494 2023-04-06 14:02:23.000000 sett-4.2.0/sett/gui/decrypt_tab.py
--rw-rw-rw-   0 root         (0) root         (0)    14189 2023-04-06 14:02:23.000000 sett-4.2.0/sett/gui/encrypt_tab.py
--rw-rw-rw-   0 root         (0) root         (0)     6383 2023-04-06 14:02:23.000000 sett-4.2.0/sett/gui/file_selection_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     6588 2023-04-06 14:02:23.000000 sett-4.2.0/sett/gui/key_generation_dialog.py
--rw-rw-rw-   0 root         (0) root         (0)     3272 2023-04-06 14:02:23.000000 sett-4.2.0/sett/gui/keys_download_dialog.py
--rw-rw-rw-   0 root         (0) root         (0)    18587 2023-04-06 14:02:23.000000 sett-4.2.0/sett/gui/keys_tab.py
--rw-rw-rw-   0 root         (0) root         (0)     2252 2023-04-06 14:02:23.000000 sett-4.2.0/sett/gui/listener.py
--rw-rw-rw-   0 root         (0) root         (0)     9076 2023-04-06 14:02:23.000000 sett-4.2.0/sett/gui/main_window.py
--rw-rw-rw-   0 root         (0) root         (0)    10030 2023-04-06 14:02:23.000000 sett-4.2.0/sett/gui/model.py
--rw-rw-rw-   0 root         (0) root         (0)     5864 2023-04-06 14:02:23.000000 sett-4.2.0/sett/gui/parallel.py
--rw-rw-rw-   0 root         (0) root         (0)     1555 2023-04-06 14:02:23.000000 sett-4.2.0/sett/gui/pyside.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 14:02:37.093697 sett-4.2.0/sett/gui/resources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-06 14:02:23.000000 sett-4.2.0/sett/gui/resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   401906 2023-04-06 14:02:23.000000 sett-4.2.0/sett/gui/resources/rc_icons.py
--rw-rw-rw-   0 root         (0) root         (0)    17134 2023-04-06 14:02:23.000000 sett-4.2.0/sett/gui/settings_tab.py
--rw-rw-rw-   0 root         (0) root         (0)     2422 2023-04-06 14:02:23.000000 sett-4.2.0/sett/gui/theme.py
--rw-rw-rw-   0 root         (0) root         (0)    21237 2023-04-06 14:02:23.000000 sett-4.2.0/sett/gui/transfer_tab.py
--rw-rw-rw-   0 root         (0) root         (0)     6827 2023-04-06 14:02:23.000000 sett-4.2.0/sett/gui/ui_model_bind.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 14:02:37.096697 sett-4.2.0/sett/protocols/
--rw-rw-rw-   0 root         (0) root         (0)      669 2023-04-06 14:02:23.000000 sett-4.2.0/sett/protocols/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-06 14:02:23.000000 sett-4.2.0/sett/protocols/defs.py
--rw-rw-rw-   0 root         (0) root         (0)     4261 2023-04-06 14:02:23.000000 sett-4.2.0/sett/protocols/liquid_files.py
--rw-rw-rw-   0 root         (0) root         (0)     1243 2023-04-06 14:02:23.000000 sett-4.2.0/sett/protocols/multipart.py
--rw-rw-rw-   0 root         (0) root         (0)      441 2023-04-06 14:02:23.000000 sett-4.2.0/sett/protocols/protocol.py
--rw-rw-rw-   0 root         (0) root         (0)     2149 2023-04-06 14:02:23.000000 sett-4.2.0/sett/protocols/s3.py
--rw-rw-rw-   0 root         (0) root         (0)    11403 2023-04-06 14:02:23.000000 sett-4.2.0/sett/protocols/sftp.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-06 14:02:23.000000 sett-4.2.0/sett/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 14:02:37.098698 sett-4.2.0/sett/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-06 14:02:23.000000 sett-4.2.0/sett/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18470 2023-04-06 14:02:23.000000 sett-4.2.0/sett/utils/config.py
--rw-rw-rw-   0 root         (0) root         (0)     5875 2023-04-06 14:02:23.000000 sett-4.2.0/sett/utils/error_handling.py
--rw-rw-rw-   0 root         (0) root         (0)     1430 2023-04-06 14:02:23.000000 sett-4.2.0/sett/utils/get_config_path.py
--rw-rw-rw-   0 root         (0) root         (0)     9691 2023-04-06 14:02:23.000000 sett-4.2.0/sett/utils/log.py
--rw-rw-rw-   0 root         (0) root         (0)    16450 2023-04-06 14:02:23.000000 sett-4.2.0/sett/utils/progress.py
--rw-rw-rw-   0 root         (0) root         (0)      445 2023-04-06 14:02:23.000000 sett-4.2.0/sett/utils/validation.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-06 14:02:23.000000 sett-4.2.0/sett/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 14:02:37.100698 sett-4.2.0/sett/workflows/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-06 14:02:23.000000 sett-4.2.0/sett/workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-04-06 14:02:23.000000 sett-4.2.0/sett/workflows/config.py
--rw-rw-rw-   0 root         (0) root         (0)     7625 2023-04-06 14:02:23.000000 sett-4.2.0/sett/workflows/decrypt.py
--rw-rw-rw-   0 root         (0) root         (0)    20009 2023-04-06 14:02:23.000000 sett-4.2.0/sett/workflows/encrypt.py
--rw-rw-rw-   0 root         (0) root         (0)     8137 2023-04-06 14:02:23.000000 sett-4.2.0/sett/workflows/transfer.py
--rw-rw-rw-   0 root         (0) root         (0)     2634 2023-04-06 14:02:23.000000 sett-4.2.0/sett/workflows/upload_keys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 14:02:37.083697 sett-4.2.0/sett.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3072 2023-04-06 14:02:37.000000 sett-4.2.0/sett.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1571 2023-04-06 14:02:37.000000 sett-4.2.0/sett.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 14:02:37.000000 sett-4.2.0/sett.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       86 2023-04-06 14:02:37.000000 sett-4.2.0/sett.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 14:02:35.000000 sett-4.2.0/sett.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      471 2023-04-06 14:02:37.000000 sett-4.2.0/sett.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-06 14:02:37.000000 sett-4.2.0/sett.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1908 2023-04-06 14:02:37.101698 sett-4.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:22:40.829843 sett-4.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2023-06-21 12:22:30.000000 sett-4.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3014 2023-06-21 12:22:40.830843 sett-4.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1844 2023-06-21 12:22:30.000000 sett-4.3.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1984 2023-06-21 12:22:30.000000 sett-4.3.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:22:40.819843 sett-4.3.0/sett/
+-rw-rw-rw-   0 root         (0) root         (0)     2444 2023-06-21 12:22:30.000000 sett-4.3.0/sett/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:22:40.821843 sett-4.3.0/sett/cli/
+-rw-rw-rw-   0 root         (0) root         (0)    15866 2023-06-21 12:22:30.000000 sett-4.3.0/sett/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18404 2023-06-21 12:22:30.000000 sett-4.3.0/sett/cli/cli_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)     3394 2023-06-21 12:22:30.000000 sett-4.3.0/sett/cli/progress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:22:40.823843 sett-4.3.0/sett/core/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-06-21 12:22:30.000000 sett-4.3.0/sett/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9765 2023-06-21 12:22:30.000000 sett-4.3.0/sett/core/archive.py
+-rw-rw-rw-   0 root         (0) root         (0)     6613 2023-06-21 12:22:30.000000 sett-4.3.0/sett/core/checksum.py
+-rw-rw-rw-   0 root         (0) root         (0)    17108 2023-06-21 12:22:30.000000 sett-4.3.0/sett/core/crypt.py
+-rw-rw-rw-   0 root         (0) root         (0)      442 2023-06-21 12:22:30.000000 sett-4.3.0/sett/core/error.py
+-rw-rw-rw-   0 root         (0) root         (0)     6635 2023-06-21 12:22:30.000000 sett-4.3.0/sett/core/filesystem.py
+-rw-rw-rw-   0 root         (0) root         (0)      651 2023-06-21 12:22:30.000000 sett-4.3.0/sett/core/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     2046 2023-06-21 12:22:30.000000 sett-4.3.0/sett/core/request.py
+-rw-rw-rw-   0 root         (0) root         (0)     1448 2023-06-21 12:22:30.000000 sett-4.3.0/sett/core/secret.py
+-rw-rw-rw-   0 root         (0) root         (0)     2147 2023-06-21 12:22:30.000000 sett-4.3.0/sett/core/versioncheck.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:22:40.826843 sett-4.3.0/sett/gui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 12:22:30.000000 sett-4.3.0/sett/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2451 2023-06-21 12:22:30.000000 sett-4.3.0/sett/gui/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3492 2023-06-21 12:22:30.000000 sett-4.3.0/sett/gui/cert_migration_dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     5767 2023-06-21 12:22:30.000000 sett-4.3.0/sett/gui/cert_revocation_dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)    15661 2023-06-21 12:22:30.000000 sett-4.3.0/sett/gui/component.py
+-rw-rw-rw-   0 root         (0) root         (0)     3512 2023-06-21 12:22:30.000000 sett-4.3.0/sett/gui/decrypt_tab.py
+-rw-rw-rw-   0 root         (0) root         (0)    14221 2023-06-21 12:22:30.000000 sett-4.3.0/sett/gui/encrypt_tab.py
+-rw-rw-rw-   0 root         (0) root         (0)     6341 2023-06-21 12:22:30.000000 sett-4.3.0/sett/gui/file_selection_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     7942 2023-06-21 12:22:30.000000 sett-4.3.0/sett/gui/key_generation_dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     4308 2023-06-21 12:22:30.000000 sett-4.3.0/sett/gui/keys_download_dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)    24662 2023-06-21 12:22:30.000000 sett-4.3.0/sett/gui/keys_tab.py
+-rw-rw-rw-   0 root         (0) root         (0)     2234 2023-06-21 12:22:30.000000 sett-4.3.0/sett/gui/listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     9128 2023-06-21 12:22:30.000000 sett-4.3.0/sett/gui/main_window.py
+-rw-rw-rw-   0 root         (0) root         (0)    12387 2023-06-21 12:22:30.000000 sett-4.3.0/sett/gui/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     5864 2023-06-21 12:22:30.000000 sett-4.3.0/sett/gui/parallel.py
+-rw-rw-rw-   0 root         (0) root         (0)     1555 2023-06-21 12:22:30.000000 sett-4.3.0/sett/gui/pyside.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:22:40.826843 sett-4.3.0/sett/gui/resources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 12:22:30.000000 sett-4.3.0/sett/gui/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   401906 2023-06-21 12:22:30.000000 sett-4.3.0/sett/gui/resources/rc_icons.py
+-rw-rw-rw-   0 root         (0) root         (0)    17133 2023-06-21 12:22:30.000000 sett-4.3.0/sett/gui/settings_tab.py
+-rw-rw-rw-   0 root         (0) root         (0)     3193 2023-06-21 12:22:30.000000 sett-4.3.0/sett/gui/theme.py
+-rw-rw-rw-   0 root         (0) root         (0)    21254 2023-06-21 12:22:30.000000 sett-4.3.0/sett/gui/transfer_tab.py
+-rw-rw-rw-   0 root         (0) root         (0)     6827 2023-06-21 12:22:30.000000 sett-4.3.0/sett/gui/ui_model_bind.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:22:40.827843 sett-4.3.0/sett/protocols/
+-rw-rw-rw-   0 root         (0) root         (0)      669 2023-06-21 12:22:30.000000 sett-4.3.0/sett/protocols/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-21 12:22:30.000000 sett-4.3.0/sett/protocols/defs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4261 2023-06-21 12:22:30.000000 sett-4.3.0/sett/protocols/liquid_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     1243 2023-06-21 12:22:30.000000 sett-4.3.0/sett/protocols/multipart.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2023-06-21 12:22:30.000000 sett-4.3.0/sett/protocols/protocol.py
+-rw-rw-rw-   0 root         (0) root         (0)     2149 2023-06-21 12:22:30.000000 sett-4.3.0/sett/protocols/s3.py
+-rw-rw-rw-   0 root         (0) root         (0)    11619 2023-06-21 12:22:30.000000 sett-4.3.0/sett/protocols/sftp.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 12:22:30.000000 sett-4.3.0/sett/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:22:40.828843 sett-4.3.0/sett/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 12:22:30.000000 sett-4.3.0/sett/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18440 2023-06-21 12:22:30.000000 sett-4.3.0/sett/utils/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     5875 2023-06-21 12:22:30.000000 sett-4.3.0/sett/utils/error_handling.py
+-rw-rw-rw-   0 root         (0) root         (0)     1430 2023-06-21 12:22:30.000000 sett-4.3.0/sett/utils/get_config_path.py
+-rw-rw-rw-   0 root         (0) root         (0)     9691 2023-06-21 12:22:30.000000 sett-4.3.0/sett/utils/log.py
+-rw-rw-rw-   0 root         (0) root         (0)    16450 2023-06-21 12:22:30.000000 sett-4.3.0/sett/utils/progress.py
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-06-21 12:22:30.000000 sett-4.3.0/sett/utils/validation.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-21 12:22:30.000000 sett-4.3.0/sett/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:22:40.829843 sett-4.3.0/sett/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 12:22:30.000000 sett-4.3.0/sett/workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-06-21 12:22:30.000000 sett-4.3.0/sett/workflows/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    10334 2023-06-21 12:22:30.000000 sett-4.3.0/sett/workflows/decrypt.py
+-rw-rw-rw-   0 root         (0) root         (0)    23129 2023-06-21 12:22:30.000000 sett-4.3.0/sett/workflows/encrypt.py
+-rw-rw-rw-   0 root         (0) root         (0)     8941 2023-06-21 12:22:30.000000 sett-4.3.0/sett/workflows/transfer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3382 2023-06-21 12:22:30.000000 sett-4.3.0/sett/workflows/upload_keys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:22:40.820843 sett-4.3.0/sett.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3014 2023-06-21 12:22:40.000000 sett-4.3.0/sett.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1640 2023-06-21 12:22:40.000000 sett-4.3.0/sett.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 12:22:40.000000 sett-4.3.0/sett.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2023-06-21 12:22:40.000000 sett-4.3.0/sett.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 12:22:39.000000 sett-4.3.0/sett.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      426 2023-06-21 12:22:40.000000 sett-4.3.0/sett.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-21 12:22:40.000000 sett-4.3.0/sett.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1827 2023-06-21 12:22:40.830843 sett-4.3.0/setup.cfg
```

### Comparing `sett-4.2.0/LICENSE` & `sett-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sett-4.2.0/PKG-INFO` & `sett-4.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: sett
-Version: 4.2.0
+Version: 4.3.0
 Summary: Secure Encryption and Transfer Tool
 Home-page: https://gitlab.com/biomedit/sett
 Author: Robin Engler, Jarosław Surkont, Gerhard Bräunlich, Kevin Sayers, Christian Ribeaud, François Martin, Simone Guzzi, Swen Vermeul
 Author-email: robin.engler@sib.swiss, jaroslaw.surkont@unibas.ch, gerhard.braeunlich@id.ethz.ch, sayerskt@gmail.com, christian.ribeaud@karakun.com, francois.martin@karakun.com, simone.guzzi@sib.swiss, swen@ethz.ch
 License: GPL3v3
 Project-URL: Documentation, https://sett.rtfd.io/en/stable
 Project-URL: Source, https://gitlab.com/biomedit/sett
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: socks
 Provides-Extra: legacy
 Provides-Extra: benchmark
 Provides-Extra: dev
 License-File: LICENSE
 
-[![pipeline status](https://gitlab.com/biomedit/sett/badges/master/pipeline.svg)](https://gitlab.com/biomedit/sett/-/commits/master)
-[![coverage report](https://gitlab.com/biomedit/sett/badges/master/coverage.svg)](https://gitlab.com/biomedit/sett/-/commits/master)
+[![pipeline status](https://gitlab.com/biomedit/sett/badges/main/pipeline.svg)](https://gitlab.com/biomedit/sett/-/commits/main)
+[![coverage report](https://gitlab.com/biomedit/sett/badges/main/coverage.svg)](https://gitlab.com/biomedit/sett/-/commits/main)
 [![documentation status](https://readthedocs.org/projects/sett/badge/)](https://sett.readthedocs.io/)
 [![license](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![python version](https://img.shields.io/pypi/pyversions/sett.svg?logo=python&logoColor=white)](https://pypi.org/project/sett)
 [![latest version](https://img.shields.io/pypi/v/sett.svg)](https://pypi.org/project/sett)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # SETT - Secure Encryption and Transfer Tool
@@ -43,17 +42,17 @@
 [sett documentation](https://sett.readthedocs.io/en/stable).
 
 For the latest, non-stable, version of the docs, see
 [here](https://sett.readthedocs.io/en/latest).
 
 ### Documentation quick-links
 
-* [Requirements and installation](https://sett.readthedocs.io/en/stable/installation.html).
-* [Quick-start guide](https://sett.readthedocs.io/en/stable/quick_start.html).
-* [Creating and managing GnuPG keys with sett](https://sett.readthedocs.io/en/stable/key_management.html).
-* [Using sett to encrypt, transfer and decrypt data](https://sett.readthedocs.io/en/stable/usage.html)
+- [Requirements and installation](https://sett.readthedocs.io/en/stable/installation.html).
+- [Quick-start guide](https://sett.readthedocs.io/en/stable/quick_start.html).
+- [Creating and managing GnuPG keys with sett](https://sett.readthedocs.io/en/stable/key_management.html).
+- [Using sett to encrypt, transfer and decrypt data](https://sett.readthedocs.io/en/stable/usage.html)
 
 ## Unit tests coverage
 
 Please note that a number of gui-specific files are excluded from the unit
 tests coverage. The detailed list of excluded files can be found in
 [`pyproject.toml`](pyproject.toml), under the `[tool.coverage.run]` section.
```

### Comparing `sett-4.2.0/README.md` & `sett-4.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-[![pipeline status](https://gitlab.com/biomedit/sett/badges/master/pipeline.svg)](https://gitlab.com/biomedit/sett/-/commits/master)
-[![coverage report](https://gitlab.com/biomedit/sett/badges/master/coverage.svg)](https://gitlab.com/biomedit/sett/-/commits/master)
+[![pipeline status](https://gitlab.com/biomedit/sett/badges/main/pipeline.svg)](https://gitlab.com/biomedit/sett/-/commits/main)
+[![coverage report](https://gitlab.com/biomedit/sett/badges/main/coverage.svg)](https://gitlab.com/biomedit/sett/-/commits/main)
 [![documentation status](https://readthedocs.org/projects/sett/badge/)](https://sett.readthedocs.io/)
 [![license](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![python version](https://img.shields.io/pypi/pyversions/sett.svg?logo=python&logoColor=white)](https://pypi.org/project/sett)
 [![latest version](https://img.shields.io/pypi/v/sett.svg)](https://pypi.org/project/sett)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # SETT - Secure Encryption and Transfer Tool
@@ -17,17 +17,17 @@
 [sett documentation](https://sett.readthedocs.io/en/stable).
 
 For the latest, non-stable, version of the docs, see
 [here](https://sett.readthedocs.io/en/latest).
 
 ### Documentation quick-links
 
-* [Requirements and installation](https://sett.readthedocs.io/en/stable/installation.html).
-* [Quick-start guide](https://sett.readthedocs.io/en/stable/quick_start.html).
-* [Creating and managing GnuPG keys with sett](https://sett.readthedocs.io/en/stable/key_management.html).
-* [Using sett to encrypt, transfer and decrypt data](https://sett.readthedocs.io/en/stable/usage.html)
+- [Requirements and installation](https://sett.readthedocs.io/en/stable/installation.html).
+- [Quick-start guide](https://sett.readthedocs.io/en/stable/quick_start.html).
+- [Creating and managing GnuPG keys with sett](https://sett.readthedocs.io/en/stable/key_management.html).
+- [Using sett to encrypt, transfer and decrypt data](https://sett.readthedocs.io/en/stable/usage.html)
 
 ## Unit tests coverage
 
 Please note that a number of gui-specific files are excluded from the unit
 tests coverage. The detailed list of excluded files can be found in
 [`pyproject.toml`](pyproject.toml), under the `[tool.coverage.run]` section.
```

### Comparing `sett-4.2.0/pyproject.toml` & `sett-4.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,23 +15,23 @@
     "sett/gui/transfer_tab.py",
     "sett/gui/file_selection_widget.py",
 ]
 
 [tool.tox]
 legacy_tox_ini = '''
 [tox]
-envlist = py{37,38,39,310,311},report
+envlist = py{38,39,310,311},report
 isolated_build = true
 
 [testenv]
 setenv =
     SETT_LEGACY=true
-    py{37,38,39,310,311}: COVERAGE_FILE = .coverage.{envname}
+    py{38,39,310,311}: COVERAGE_FILE = .coverage.{envname}
 depends =
-    report: py{37,38,39,310,311}
+    report: py{38,39,310,311}
 deps =
     PySide2
     pytest
     pytest-cov
     pytest-randomly
     pytest-factoryboy
 commands =
@@ -57,15 +57,15 @@
     "PySide2",
     "matplotlib",
     "matplotlib.pyplot",
     "seaborn",
     "minio",
     "minio.error",
     "factory",
-    "darkdetect"
+    "darkdetect",
 ]
 ignore_missing_imports = true
 
 [tool.pylint.MAIN]
 jobs = 2
 load-plugins = ["pylint.extensions.docparams", "biomedit_lints"]
```

### Comparing `sett-4.2.0/sett/__init__.py` & `sett-4.3.0/sett/__init__.py`

 * *Files identical despite different names*

### Comparing `sett-4.2.0/sett/cli/__init__.py` & `sett-4.3.0/sett/cli/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 import json
 import shlex
 import subprocess  # nosec B404:blacklist import_subprocess
 from functools import wraps
 from getpass import getpass
 from typing import List, Dict, Any, Optional, Callable, Type, Union, TypeVar, cast
 
+from sett_rs.cert import CertStore, CertType
+
 from .progress import CliProgress
 from .cli_builder import (
     rename,
     return_to_stdout,
     partial,
     lazy_partial,
     CliWithSubcommands,
@@ -49,14 +51,15 @@
     liquid_files,
     parse_protocol,
     __all__ as available_protocols,
 )
 from ..core.versioncheck import check_version
 from ..core.error import UserError
 from ..core.filesystem import OutOfSpaceError
+from ..core.metadata import Purpose
 from .. import URL_READTHEDOCS, URL_GITLAB_ISSUES
 
 logger = create_logger(__name__)
 
 
 def parse_dict(s: str) -> Dict[str, Any]:
     """Convert/deserialize a JSON formatted string to a dict object."""
@@ -69,20 +72,24 @@
     dictionary object.
 
     Example of input string:
     {"host": "sftp.example.com", "username": "sftp",
     "destination_dir": "upload", "pkey": "~/.ssh/id_rsa", "pkey_password": ""}
     """
     args = parse_dict(s)
-    not_provided = object()
-    pw = args.get("pkey_password", not_provided)
-    if pw is None:  # pw is provided and is None
-        args["pkey_password"] = Secret(
-            getpass("Please enter your ssh private key password:")
-        )
+
+    # Convert the provided password (if any) to a `Secret` object (i.e. an
+    # object that will not print its encapsulated content). If the value
+    # {"pkey_password": null} was passed, the "null" is converted to an
+    # empty string `""` rather than to None.
+    args["pkey_password"] = Secret(
+        str(args["pkey_password"] if args["pkey_password"] else "")
+        if "pkey_password" in args
+        else getpass("Please enter your SSH private key password:")
+    )
     return args
 
 
 def two_factor_cli_prompt() -> str:
     return input("Please enter 2FA verification code: ")
 
 
@@ -109,42 +116,107 @@
     msg: str, passphrase_cmd: Optional[str]
 ) -> Secret[str]:
     if passphrase_cmd:
         return get_passphrase_from_cmd(passphrase_cmd)
     return Secret(getpass(msg))
 
 
-@wraps(workflows_encrypt)
+def get_certificate_fingerprint(
+    search_term: str, store: CertStore, cert_type: CertType
+) -> str:
+    """Check that the specified search term matches exactly one certificate
+    in the local CertStore, and return the fingerprint of the matching
+    certificate.
+
+    The search term can be one of the following: email, fingerprint or
+    keyID (the last 16 chars of the fingerprint)
+    """
+
+    certs = [
+        cert
+        for cert in store.list_certs(cert_type)
+        if search_term in (cert.email, cert.fingerprint, cert.key_id)
+    ]
+    try:
+        (cert,) = certs
+        return cert.fingerprint
+    except ValueError:
+        raise UserError(
+            f"{'No' if len(certs) == 0 else 'More than one'} certificate "
+            f"matching '{search_term}' was found in the local CertStore."
+        ) from None
+
+
 def encrypt(
-    *files: str,
+    files: List[str],
     config: Config,
-    dry_run: bool,
-    passphrase_cmd: Optional[str],
+    recipient: List[str],
+    sender: Optional[str] = None,
+    compression_level: Optional[int] = None,
+    dry_run: bool = False,
+    passphrase_cmd: Optional[str] = None,
     dtr_id: Optional[int] = None,
-    **kwargs: Any,
+    output: Optional[str] = None,
+    output_suffix: Optional[str] = None,
+    force: bool = False,
+    purpose: Optional[Purpose] = None,
+    progress: Optional[ProgressInterface] = None,
 ) -> Optional[str]:
     """Wrapper for the main function of the encrypt workflow."""
 
-    # Retrieve the user's PGP key password (needed to sign the data).
-    kwargs["passphrase"] = (
-        None
-        if dry_run
-        else get_passphrase_from_cmd_or_prompt(
-            "Please enter your PGP private key password:", passphrase_cmd
+    def get_value_from_config(arg_name: str, arg_name_in_config: str) -> Any:
+        value_from_config = getattr(config, arg_name_in_config)
+        if value_from_config is None:
+            raise UserError(f"{arg_name} not specified with no default in config.")
+        return value_from_config
+
+    # If no sender or compression level is specified, attempt to retrieve their
+    # default values from config.
+    if sender is None:
+        sender = get_value_from_config("sender", "default_sender")
+    if compression_level is None:
+        compression_level = get_value_from_config(
+            "compression_level", "compression_level"
         )
-    )
+
+    # Make sure that sender and recipient certificates are present in the local
+    # CertStore. If needed, this also converts the certificate identifier from
+    # an email to a fingerprint.
+    # Note: only applies when using Sequoia as crypto backend (experimental).
+    if config.experimental:
+        store = CertStore()
+        sender = get_certificate_fingerprint(sender, store, CertType.Secret)
+        recipients = [
+            get_certificate_fingerprint(r, store, CertType.Public) for r in recipient
+        ]
+    else:
+        # Note: we use "recipient" instead of "recipients" in the signature of
+        # this function because it's used to build the CLI options.
+        recipients = recipient
 
     # Run the encrypt workflow.
     try:
         return workflows_encrypt(
-            *files,
+            files=files,
             dtr_id=dtr_id,
             config=config,
+            sender=sender,
+            recipients=recipients,
+            output=output,
+            output_suffix=output_suffix,
+            force=force,
+            purpose=purpose,
             dry_run=dry_run,
-            **kwargs,
+            compression_level=compression_level,
+            passphrase=None
+            if dry_run
+            else get_passphrase_from_cmd_or_prompt(
+                "Please enter your PGP private key password:", passphrase_cmd
+            ),
+            progress=progress,
         )
     except OutOfSpaceError as e:
         raise OutOfSpaceError(f"{e} Use --force or -f to ignore this error.") from e
 
 
 @wraps(workflows_decrypt)
 def decrypt(
@@ -241,20 +313,21 @@
                 partial(config=config),
                 lazy_partial(progress=CliProgress),
             ),
             overrides={
                 "files": {"help": "Input file(s) or directories."},
                 "sender": {
                     "help": "Fingerprint, key ID or email associated "
-                    "with GPG key of data sender.",
+                    "with OpenPGP key of data sender.",
                     "alias": "-s",
                 },
                 "recipient": {
                     "help": "Fingerprint, key ID or email associated with "
-                    "GPG key of data recipient(s).",
+                    "OpenPGP key of data recipient. Multiple recipients can "
+                    "be specified by passing this option multiple times.",
                     "alias": "-r",
                 },
                 "dtr_id": {
                     "help": "Data Transfer Request (DTR) ID (optional if "
                     "`verify_dtr` is disabled in settings).",
                     "alias": "-t",
                 },
@@ -280,15 +353,15 @@
                 "dry_run": dry_run_override,
                 "compression_level": {
                     "help": "Compression level for inner tarball in the range "
                     "0 (no compression) to 9 (highest compression). "
                     "Higher compression levels require more computing "
                     "time."
                 },
-                "passphrase": passphrase_override,
+                "passphrase_cmd": passphrase_override,
             },
         ),
         Subcommand(
             decorate(
                 transfer,
                 partial(config=config, two_factor_callback=two_factor_cli_prompt),
                 lazy_partial(progress=CliProgress),
@@ -320,16 +393,17 @@
         Subcommand(
             decorate(
                 decrypt, partial(config=config), lazy_partial(progress=CliProgress)
             ),
             overrides={
                 "files": {"help": "Path(s) to encrypted package(s)"},
                 "output_dir": {
-                    "help": "Path to the directory where package content is saved after decryption. "
-                    "If no path is specified, current working directory is taken.",
+                    "help": "Path to the directory where package content is "
+                    "saved after decryption. If no path is specified, current "
+                    "working directory is taken.",
                     "default": os.getcwd(),
                     "alias": "-o",
                 },
                 "decrypt_only": {"help": "Skip extraction."},
                 "dry_run": dry_run_override,
                 "passphrase": passphrase_override,
             },
```

### Comparing `sett-4.2.0/sett/cli/cli_builder.py` & `sett-4.3.0/sett/cli/cli_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,31 @@
 import collections
 import argparse
 import inspect
-import sys
 from functools import wraps, partial as ft_partial
 from typing import (
     Callable,
     Generator,
     Iterable,
     Optional,
+    Protocol,
     Union,
     Sequence,
     Tuple,
     Dict,
     cast,
     Any,
     TypeVar,
     FrozenSet,
 )
 import pprint
 
 from libbiomedit.lib.classify import is_optional, IsTypingType
 from libbiomedit.lib.deserialize import optional_type as _libbiomedit_optional_type
 
-# Python 3.7: Protocol is not present in the base typing module for
-# python versions <= 3.7, and must be imported from typing_extensions.
-# NOTE: mypy does not accept the "try: ... except ImportError:" syntax for
-# importing Protocol.
-if sys.version_info >= (3, 8):
-    from typing import Protocol
-else:
-    from typing_extensions import Protocol
-
 
 class ParserLike(Protocol):
     """Protocol interface to define a generic parser that has both the
     add_argument and add_mutually_exclusive_group methods.
     This allows the ParserLike class to impersonate objects from both the
     argparse.ArgumentParser and argparse._MutuallyExclusiveGroup classes.
     """
@@ -298,15 +289,15 @@
 
         # Run the function corresponding to the subcommand passed by the user.
         action = actions[cmd_args.pop("action")]
         action(**cmd_args)
 
 
 # Starting with python 3.7, the typing module has a new API.
-_origin_attr = "__extra__" if sys.version_info < (3, 7) else "__origin__"
+_origin_attr = "__origin__"
 
 
 # T is used as generic variable type.
 T = TypeVar("T")
 
 
 def default_args(default: T) -> Dict[str, Union[bool, T]]:
```

### Comparing `sett-4.2.0/sett/cli/progress.py` & `sett-4.3.0/sett/cli/progress.py`

 * *Files identical despite different names*

### Comparing `sett-4.2.0/sett/core/archive.py` & `sett-4.3.0/sett/core/archive.py`

 * *Files identical despite different names*

### Comparing `sett-4.2.0/sett/core/checksum.py` & `sett-4.3.0/sett/core/checksum.py`

 * *Files identical despite different names*

### Comparing `sett-4.2.0/sett/core/crypt.py` & `sett-4.3.0/sett/core/crypt.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,21 @@
     Type,
     TypeVar,
     Union,
     cast,
 )
 
 from libbiomedit import crypt
+from sett_rs.cert import (
+    CertInfo,
+    CertStore,
+    CertType,
+    generate_cert,
+    create_revocation_signature as _create_revocation_signature,
+)
 
 from . import gpg
 from .error import UserError
 from .request import urlopen
 from .secret import Secret, reveal
 from ..utils.config import Config
 
@@ -49,14 +56,15 @@
 
     return _to_user_error
 
 
 verify_metadata_signature = to_user_error(RuntimeError)(
     partial(crypt.verify_metadata_signature, url_opener=urlopen)
 )
+create_revocation_signature = to_user_error(RuntimeError)(_create_revocation_signature)
 
 
 @to_user_error((RuntimeError, gpg.GPGError))
 def retrieve_refresh_and_validate_keys(
     key_identifiers: Iterable[str], config: Config
 ) -> Tuple[gpg.Key, ...]:
     """Performs the following tasks on the keys matching the specified
@@ -113,45 +121,52 @@
     """
 
     RSA = 1
     DSA = 2
     ECC = 22
 
 
-def verify_key_length(key: gpg.Key, min_key_length: int = 4096) -> None:
+def verify_key_length(
+    key: Union[gpg.Key, CertInfo], min_key_length: int = 4096
+) -> None:
     """Verify that the type (algorithm) of a PGP keys is strong enough."""
 
     allowed_key_description = (
         f"Only RSA (min. key length: {min_key_length}) and ECC keys are allowed"
     )
 
     try:
-        algorithm = KeyAlgorithm(key.pub_key_algorithm)
+        algorithm = (
+            KeyAlgorithm(key.pub_key_algorithm)
+            if isinstance(key, gpg.Key)
+            else KeyAlgorithm(key.primary_key.pub_key_algorithm)
+        )
     except ValueError as e:
-        if key.key_length < min_key_length:
-            raise UserError(
-                f"Non-allowed PGP key algorithm: key {key.key_id} is using a "
-                f"non-allowed algorithm. {allowed_key_description}."
-            ) from e
+        raise UserError(
+            f"OpenPGP key {key.key_id} is using a forbidden algorithm. "
+            f"{allowed_key_description}."
+        ) from e
 
-    if algorithm == KeyAlgorithm.ECC:
-        warnings.warn(
-            f"Please note: key {key.key_id} is of type ECC, which is not "
-            "supported by older versions of GnuPG."
-        )
-        return
     if algorithm == KeyAlgorithm.DSA:
         raise UserError(
             f"Non-allowed PGP key algorithm: key {key.key_id} is of type DSA. "
             f"{allowed_key_description}."
         )
-    if key.key_length < min_key_length:
+    key_length = (
+        key.key_length if isinstance(key, gpg.Key) else key.primary_key.length or 0
+    )
+    if algorithm == KeyAlgorithm.RSA and key_length < min_key_length:
         raise UserError(
-            f"Non-allowed PGP key algorithm: key {key.key_id} is shorter than "
-            f"the minimal required length. {allowed_key_description}."
+            f"OpenPGP key {key.key_id} is shorter than the required minimal "
+            f"length. {allowed_key_description}."
+        )
+    if algorithm == KeyAlgorithm.ECC:
+        warnings.warn(
+            f"Please note: key {key.key_id} is of type ECC, which is not "
+            "supported by older versions of GnuPG."
         )
 
 
 @to_user_error((gpg.KeyserverError, gpg.KeyserverOtherError))
 def request_key_verification(
     token: str, address: str, keyserver: str
 ) -> gpg.keyserver.VksUploadResponse:
@@ -166,25 +181,44 @@
     """Upload public keys to keyserver."""
     return tuple(
         gpg_store.vks_send_key(fingerprint, keyserver=keyserver)
         for fingerprint in fingerprints
     )
 
 
+@to_user_error((gpg.KeyserverError, gpg.KeyserverOtherError))
+def upload_cert(
+    ascii_armored_cert: str, keyserver: str
+) -> gpg.keyserver.VksUploadResponse:
+    """Upload an OpenPGP certificate to a verifying keyserver (VKS)."""
+    return gpg.keyserver.vks_upload_key(ascii_armored_cert, keyserver=keyserver)
+
+
 @to_user_error(
     (gpg.KeyserverError, gpg.KeyserverOtherError, gpg.KeyserverKeyNotFoundError)
 )
 def download_keys(
     key_identifiers: List[str], keyserver: str, gpg_store: GPGStore
 ) -> None:
     """Download public keys from a verifying keyserver (VKS)."""
     for key_identifier in key_identifiers:
         gpg_store.vks_recv_key(key_identifier, keyserver=keyserver)
 
 
+@to_user_error(
+    (gpg.KeyserverError, gpg.KeyserverOtherError, gpg.KeyserverKeyNotFoundError)
+)
+def download_cert(keyserver: str, identifier: str) -> bytes:
+    """Download a public certificate from a verifying keyserver (VKS)."""
+    with gpg.keyserver.vks_get_key_by_any_identifier(
+        keyserver=keyserver, identifier=identifier
+    ) as response:
+        return response.read()
+
+
 def detach_sign_file(
     src: Union[bytes, IO[bytes]],
     signature_fingerprint: str,
     passphrase: Secret[str],
     gpg_store: GPGStore,
 ) -> bytes:
     """Sign a file with a detached signature."""
@@ -358,15 +392,15 @@
                 "sign it with an external tool (e.g. GnuPG) or enable "
                 "'Always trust recipient key' in the settings."
             )
         msg.append(f"Original error: {e}")
         raise UserError(" ".join(msg)) from e
 
 
-def get_recipient_email(key: gpg.Key) -> str:
+def get_recipient_email(key: Union[gpg.Key, CertInfo]) -> str:
     """Retrieve the email address associated with a PGP key, and generate a
     an error if the email address is missing or could not be retrieved.
     """
     try:
         email = key.uids[0].email
     except (IndexError, UnpackError):
         raise UserError(
@@ -417,36 +451,64 @@
             "Encrypted package has multiple signatures. "
             "This is not compliant with the BiomedIT Protocol"
         )
     return sender_fingerprints
 
 
 def create_key(
-    full_name: str,
+    name: str,
     email: str,
     pwd: Secret[str],
     gpg_store: GPGStore,
+    comment: Optional[str] = None,
     key_type: str = "RSA",
     key_length: int = 4096,
 ) -> gpg.Key:
     """Create a new PGP public/private key."""
 
     min_pwd_len = 10
-    if len(full_name) < 5:
+    if len(name) < 5:
         raise UserError("Full name must be at least 5 characters long.")
     if not re.search(r"[^@]+@[^@]+\.[^@]+", email):
         raise UserError("Invalid email address.")
     if len(pwd.reveal()) < min_pwd_len:
         raise UserError("Password is too short (min length: " f"{min_pwd_len})")
     fingerprint = gpg_store.gen_key(
         key_type=key_type,
         key_length=key_length,
-        full_name=full_name,
+        full_name=name + (f" ({comment})" if comment else ""),
         email=email,
         passphrase=pwd.reveal(),
     )
     pkey = gpg_store.list_sec_keys(search_terms=(fingerprint,))
     if not pkey:
         raise UserError(f"No private keys found for: {fingerprint}")
     if len(pkey) > 1:
         raise UserError(f"Multiple private keys found for: {fingerprint}")
     return pkey[0]
+
+
+@to_user_error(RuntimeError)
+def generate_and_import_certificate(
+    name: str,
+    email: str,
+    password: Secret[str],
+    comment: Optional[str] = None,
+) -> Tuple[bytes, bytes]:
+    min_pwd_len = 10
+    if len(name) < 5:
+        raise UserError("Full name must be at least 5 characters long.")
+    if not re.search(r"[^@]+@[^@]+\.[^@]+", email):
+        raise UserError("Invalid email address.")
+    if len(password.reveal()) < min_pwd_len:
+        raise UserError("Password is too short (min length: " f"{min_pwd_len})")
+    (cert, rev_sig) = generate_cert(
+        uid=f"{name} {f'({comment}) ' if comment else ''}<{email}>",
+        password=password.reveal().encode("utf8"),
+    )
+    CertStore().import_cert(cert, CertType.Secret)
+    return (cert, rev_sig)
+
+
+@to_user_error(RuntimeError)
+def revoke_certificate(rev_sig: bytes) -> None:
+    CertStore().revoke(rev_sig)
```

### Comparing `sett-4.2.0/sett/core/filesystem.py` & `sett-4.3.0/sett/core/filesystem.py`

 * *Files identical despite different names*

### Comparing `sett-4.2.0/sett/core/metadata.py` & `sett-4.3.0/sett/core/metadata.py`

 * *Files identical despite different names*

### Comparing `sett-4.2.0/sett/core/request.py` & `sett-4.3.0/sett/core/request.py`

 * *Files identical despite different names*

### Comparing `sett-4.2.0/sett/core/secret.py` & `sett-4.3.0/sett/core/secret.py`

 * *Files identical despite different names*

### Comparing `sett-4.2.0/sett/core/versioncheck.py` & `sett-4.3.0/sett/core/versioncheck.py`

 * *Files identical despite different names*

### Comparing `sett-4.2.0/sett/gui/__main__.py` & `sett-4.3.0/sett/gui/__main__.py`

 * *Files identical despite different names*

### Comparing `sett-4.2.0/sett/gui/component.py` & `sett-4.3.0/sett/gui/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     TypeVar,
     Type,
     Iterable,
 )
 
 from .parallel import run_thread
 from .pyside import QtCore, QtWidgets, open_window
-from .theme import Action, IconRepainterWidget, PushButton
+from .theme import Action, PushButton
 from .. import APP_NAME_SHORT
 from ..core.secret import Secret
 from ..utils.progress import ProgressInterface
 
 EXTRA_HEIGHT = 1
 MACOS_TOOLTIP_BG_COLOR = "#ffffca"
 
@@ -71,15 +71,15 @@
     """
 
     def __init__(self, label: str):
         super().__init__(label + " <sup><font color='red'>*</font></sup>")
 
 
 class SelectionButton(QtWidgets.QPushButton):
-    """A push button extension which connects this button to given selection
+    """A push button extension which connects this button to a given selection
     model.
 
     The button is disabled by default. And gets enabled when the selection has,
     at least, one selected row.
     """
 
     def __init__(self, label: str, selection_model: QtCore.QItemSelectionModel):
@@ -136,15 +136,15 @@
         self.n = completed_fraction
         self.updated.emit(round(completed_fraction * 100, 0))
 
     def get_completed_fraction(self) -> float:
         return self.n
 
 
-class ConsoleWidget(QtWidgets.QGroupBox, IconRepainterWidget):
+class ConsoleWidget(QtWidgets.QGroupBox):
     def __init__(self, title: str, parent: QtWidgets.QWidget):
         super().__init__(title, parent)
         self.textbox = QtWidgets.QTextEdit()
         self.textbox.setReadOnly(True)
         btn_clear_console = PushButton(":icon/feather/slash.png", "", self)
         btn_clear_console.setToolTip("Clear console")
         btn_clear_console.clicked.connect(self.clear)
@@ -163,15 +163,15 @@
 
 
 class PathInput:
     """Path selection container with a select button and a 'show path' field."""
 
     def __init__(
         self,
-        parent: IconRepainterWidget,
+        parent: QtWidgets.QWidget,
         directory: bool = True,
         path: Optional[Path] = Path.home(),
         btn_clear: bool = True,
     ):
         self.parent = parent
         self.text = LineEdit(parent)
         self.text.setReadOnly(True)
@@ -217,15 +217,15 @@
         self.text.setStatusTip(msg)
 
     def on_path_change(self, fn: Callable[[Optional[Path]], None]) -> None:
         """Run callback when path changes."""
         self.text.editingFinished.connect(lambda: fn(self.path))
 
 
-class BaseTab(IconRepainterWidget):
+class BaseTab(QtWidgets.QWidget):
     """Adds two boxes to the layout of a QWidget (a Tab from the application):
     - Box with buttons to run and test run a workflow.
     - Box with a console.
     """
 
     def create_console(self) -> None:
         # pylint:disable=attribute-defined-outside-init
```

### Comparing `sett-4.2.0/sett/gui/decrypt_tab.py` & `sett-4.3.0/sett/gui/decrypt_tab.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,11 +88,11 @@
                 "output_dir": str(self.app_data.decrypt_output_location),
                 "config": self.app_data.config,
                 "decrypt_only": self.app_data.decrypt_decrypt_only,
                 "passphrase": pw,
                 "dry_run": dry_run,
                 "progress": GuiProgress(self.progress_bar.setValue),
             },
-            capture_loggers=(decrypt.logger,),
+            capture_loggers=(decrypt.logger, decrypt.logger_rs),
             ignore_exceptions=True,
             report_config=self.app_data.config,
         )
```

### Comparing `sett-4.2.0/sett/gui/encrypt_tab.py` & `sett-4.3.0/sett/gui/encrypt_tab.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,23 @@
 
 from .component import (
     BaseTab,
     PathInput,
     GuiProgress,
     create_slider,
     get_pass_input,
-    SelectionButton,
     MandatoryLabel,
     LineEdit,
     grid_layout,
     GridLayoutCell,
     vbox_layout,
     hbox_layout,
 )
 from .file_selection_widget import DirectoryAndFileSelectionWidget
-from .theme import Icon, PushButton
+from .theme import PushButton, EnabledOnSelectionButton
 from .model import TableModel, AppData, KeyValueListModel
 from .pyside import QtCore, QtGui, QtWidgets
 from ..core.filesystem import OutOfSpaceError
 from ..core.metadata import Purpose
 from ..utils.config import LABEL_COMPRESSION_LEVEL, DESCRIPTION_COMPRESSION_LEVEL
 from ..utils.validation import PACKAGE_SUFFIX
 from ..workflows import encrypt
@@ -100,37 +99,35 @@
         if self.app_data.default_key_index:
             sender_widget.setCurrentIndex(self.app_data.default_key_index)
 
         recipients_input_view = QtWidgets.QComboBox()
         recipients_input_view.setModel(self.app_data.pub_keys_model)
 
         recipients_output_view = QtWidgets.QTableView()
-        recipients_output_model = TableModel(columns=("Name", "Email", "Fingerprint"))
-        recipients_output_view.setModel(recipients_output_model)
+        recipients_output_view.setModel(self.app_data.encrypt_recipients_model)
         recipients_output_view.verticalHeader().hide()
         recipients_output_view.horizontalHeader().setSectionResizeMode(
             QtWidgets.QHeaderView.ResizeMode.ResizeToContents
         )
         recipients_output_view.horizontalHeader().setStretchLastSection(True)
         recipients_output_view.setSelectionBehavior(
             QtWidgets.QTableView.SelectionBehavior.SelectRows
         )
         recipients_output_view.setSelectionMode(
             QtWidgets.QTableView.SelectionMode.SingleSelection
         )
 
         recipients_btn_add = PushButton(":icon/feather/user-plus.png", "", self)
         recipients_btn_add.setToolTip("Add recipient to the list")
-        recipients_btn_remove = SelectionButton(
-            "", recipients_output_view.selectionModel()
-        )
-        icon_file_name = ":icon/feather/user-minus.png"
-        recipients_btn_remove.setIcon(Icon(icon_file_name))
-        self.icon_repainter().register(
-            lambda: recipients_btn_remove.setIcon(Icon(icon_file_name))
+
+        recipients_btn_remove = EnabledOnSelectionButton(
+            ":icon/feather/user-minus.png",
+            "",
+            self,
+            recipients_output_view.selectionModel(),
         )
         recipients_btn_remove.setToolTip("Remove recipient from the list")
 
         def update_sender(index: int) -> None:
             self.app_data.encrypt_sender = (
                 ""
                 if index == -1
@@ -145,31 +142,40 @@
             )
 
         def add_recipient() -> None:
             # Note: it's probably possible to get rid of the cast() here.
             key = cast(KeyValueListModel, recipients_input_view.model()).get_value(
                 recipients_input_view.currentIndex()
             )
-            row = (key.uids[0].full_name, key.uids[0].email, key.fingerprint)
-            recipients_output_model.set_data(
-                tuple(set(recipients_output_model.get_data()) | set([row]))
+            row = (
+                key.uids[0].full_name
+                if hasattr(key.uids[0], "full_name")
+                else key.uids[0].name,
+                key.uids[0].email,
+                key.fingerprint,
+            )
+            self.app_data.encrypt_recipients_model.set_data(
+                tuple(
+                    set(self.app_data.encrypt_recipients_model.get_data()) | set([row])
+                )
             )
 
         def remove_recipient() -> None:
             recipients_output_view.model().removeRows(
                 recipients_output_view.currentIndex().row(), 1
             )
             recipients_output_view.clearSelection()
 
         # Connect actions.
         recipients_btn_add.clicked.connect(add_recipient)
         recipients_btn_remove.clicked.connect(remove_recipient)
-        recipients_output_model.dataChanged.connect(update_recipients)
+        self.app_data.encrypt_recipients_model.dataChanged.connect(update_recipients)
         sender_widget.currentIndexChanged.connect(update_sender)
-        # Set the default value for the sender
+
+        # Set the default value for the sender.
         update_sender(sender_widget.currentIndex())
         grid_layout(
             (
                 GridLayoutCell(
                     QtWidgets.QLabel(
                         "Select data sender and add at least one recipient:"
                     ),
@@ -335,17 +341,17 @@
             passphrase = None
 
         # Run the encrypt workflow in a separate thread.
         self.run_workflow_thread(
             encrypt_workflow,
             f_kwargs={
                 "files": self.app_data.encrypt_files,
-                "capture_loggers": (encrypt.logger,),
+                "capture_loggers": (encrypt.logger, encrypt.logger_rs),
                 "sender": self.app_data.encrypt_sender,
-                "recipient": self.app_data.encrypt_recipients,
+                "recipients": self.app_data.encrypt_recipients,
                 "dtr_id": self.app_data.encrypt_transfer_id,
                 "config": self.app_data.config,
                 "passphrase": passphrase,
                 "output": self.app_data.encrypt_output_location,
                 "output_suffix": self.app_data.encrypt_package_name_suffix,
                 "dry_run": dry_run,
                 "compression_level": self.app_data.encrypt_compression_level,
```

### Comparing `sett-4.2.0/sett/gui/file_selection_widget.py` & `sett-4.3.0/sett/gui/file_selection_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 from .component import (
     SelectionAction,
     MandatoryLabel,
     show_warning,
     ToolBar,
     vbox_layout,
 )
-from .theme import Action, IconRepainterWidget
+from .theme import Action
 from .pyside import QtWidgets, QtCore, QtGui, QAction, open_window
 
 
-class FileSelectionWidget(QtWidgets.QGroupBox, IconRepainterWidget):
+class FileSelectionWidget(QtWidgets.QGroupBox):
     """File selection widget."""
 
     def __init__(
         self,
         title: str,
         parent: QtWidgets.QWidget,
         name_filter: Optional[str] = None,
```

### Comparing `sett-4.2.0/sett/gui/key_generation_dialog.py` & `sett-4.3.0/sett/gui/key_generation_dialog.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Tuple
+
 from libbiomedit.lib.secret import Secret
 
 from sett import URL_READTHEDOCS
 from .model import AppData, ConfigProxy
 from ..core import gpg, crypt
 from ..core.error import UserError
 from .component import (
@@ -82,15 +84,15 @@
         self.text_name_full.clear()
         self.text_name_extra.clear()
         self.text_email.clear()
         self.text_pass.clear()
         self.text_pass_repeat.clear()
 
     def post_key_creation(self, key: gpg.Key) -> None:
-        msg = NormalMessageBox(self.parentWidget(), "GPG Key Generation")
+        msg = NormalMessageBox(self.parentWidget(), "OpenPGP Key Generation")
         try:
             revocation_cert = crypt.create_revocation_certificate(
                 key.fingerprint,
                 self.text_pass.text(),
                 self.config.gpg_store,
             )
             msg.setIcon(QtWidgets.QMessageBox.Icon.Information)
@@ -114,50 +116,83 @@
         finally:
             open_window(msg)
             self.clear_form()
             self.app_data.update_private_keys()
             self.app_data.update_public_keys()
             self.close()
 
+    def post_cert_creation(self, cert_rev_sig: Tuple[bytes, bytes]) -> None:
+        (_, rev_sig) = cert_rev_sig
+        msg = NormalMessageBox(self.parentWidget(), "OpenPGP Key Generation")
+        msg.setIcon(QtWidgets.QMessageBox.Icon.Information)
+        msg.setText(
+            revocation_cert_creation_successful_text.format(self.config.dcc_portal_url)
+        )
+        msg.setDetailedText(rev_sig.decode())
+        # Programmatically click the "Show Details..." button so that the
+        # certificate is shown by default.
+        click_show_details(msgbox=msg)
+        open_window(msg)
+        self.clear_form()
+        self.app_data.update_private_keys()
+        self.app_data.update_public_keys()
+        self.close()
+
     @property
     def config(self) -> ConfigProxy:
         return self.app_data.config
 
     def create_private_key(self) -> None:
         self.btn_run.setEnabled(False)
-        name_full = self.text_name_full.text().strip()
-        name_extra = self.text_name_extra.text().strip()
-        if name_extra:
-            if not name_extra.startswith("(") and not name_extra.endswith(")"):
-                name_extra = f"({name_extra})"
-            name_full = name_full + " " + name_extra
-        if self.text_pass.text() != self.text_pass_repeat.text():
+        name = self.text_name_full.text().strip()
+        comment = self.text_name_extra.text().strip(" \t()")
+        email = self.text_email.text().strip(" \t<>")
+        password = Secret(self.text_pass.text())
+        if password.reveal() != self.text_pass_repeat.text():
             show_warning(
-                "GPG Key Generation Error",
+                "OpenPGP Key Generation Error",
                 "Password and repeated password do not match.",
                 self,
             )
             self.btn_run.setEnabled(True)
             return
 
-        run_thread(
-            crypt.create_key,
-            f_kwargs={
-                "full_name": name_full,
-                "email": self.text_email.text(),
-                "pwd": Secret(self.text_pass.text()),
-                "gpg_store": self.config.gpg_store,
-            },
-            forward_errors=warning_callback("GPG Key Generation Error"),
-            report_config=self.config,
-            signals={
-                "result": self.post_key_creation,
-                "finished": lambda: self.btn_run.setEnabled(True),
-            },
-        )
+        if self.config.experimental:
+            run_thread(
+                crypt.generate_and_import_certificate,
+                f_kwargs={
+                    "name": name,
+                    "email": email,
+                    "password": password,
+                    "comment": comment,
+                },
+                forward_errors=warning_callback("OpenPGP Key Generation Error"),
+                report_config=self.config,
+                signals={
+                    "result": self.post_cert_creation,
+                    "finished": lambda: self.btn_run.setEnabled(True),
+                },
+            )
+        else:
+            run_thread(
+                crypt.create_key,
+                f_kwargs={
+                    "name": name,
+                    "email": email,
+                    "pwd": password,
+                    "gpg_store": self.config.gpg_store,
+                    "comment": comment,
+                },
+                forward_errors=warning_callback("OpenPGP Key Generation Error"),
+                report_config=self.config,
+                signals={
+                    "result": self.post_key_creation,
+                    "finished": lambda: self.btn_run.setEnabled(True),
+                },
+            )
 
 
 def click_show_details(msgbox: QtWidgets.QMessageBox) -> None:
     for button in msgbox.buttons():
         if msgbox.buttonRole(button) is QtWidgets.QMessageBox.ButtonRole.ActionRole:
             button.click()
```

### Comparing `sett-4.2.0/sett/gui/keys_download_dialog.py` & `sett-4.3.0/sett/gui/keys_download_dialog.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import cast
+from typing import cast, Optional
+
+from sett_rs.cert import CertStore, CertType
 
 from . import keys_tab
 from .component import LineEdit, grid_layout, warning_callback
 from .model import AppData, ConfigProxy
 from .parallel import run_thread
 from .pyside import QtWidgets, QtCore
 from ..core import crypt
@@ -48,46 +50,71 @@
         return self.app_data.config
 
     def download(self) -> None:
         """Download key identified by given input to user's local keyring."""
 
         key_identifier = self.key_identifier.text()
 
-        def on_result() -> None:
-            self.app_data.update_public_keys()
-            cast(
-                keys_tab.KeysTab, self.parentWidget()
-            ).update_display_selected_pub_key()
-            try:
-                key = crypt.search_pub_key(
-                    key_identifier, self.config.gpg_store, sigs=False
-                )
+        def refresh_and_show_msg(info: Optional[str]) -> None:
+            if info is not None:
+                self.app_data.update_public_keys()
+                cast(
+                    keys_tab.KeysTab, self.parentWidget()
+                ).update_display_selected_pub_key()
                 keys_tab.open_info_msgbox(
                     "The following public key has been downloaded from the "
                     "keyserver:",
-                    f"{key.uids[0].email} ({key.fingerprint})",
+                    info,
                     "Please verify that the fingerprint is correct, "
                     "otherwise delete the key.",
                     title="PGP key download",
                     parent=self.parentWidget(),
                 )
+            self.btn_download.setEnabled(True)
+            self.close()
+
+        def on_result() -> None:
+            summary = None
+            try:
+                key = crypt.search_pub_key(
+                    key_identifier, self.config.gpg_store, sigs=False
+                )
+                summary = f"{key.uids[0].email} ({key.fingerprint})"
             except crypt.UnpackError:
                 # No (new) key has been downloaded resp. no single key could be found for given
                 # key identifier.
                 pass
-            self.btn_download.setEnabled(True)
-            self.close()
+            refresh_and_show_msg(summary)
 
         self.btn_download.setEnabled(False)
-        run_thread(
-            crypt.download_keys,
-            f_kwargs={
-                "key_identifiers": [self.key_identifier.text()],
-                "keyserver": self.config.keyserver_url,
-                "gpg_store": self.config.gpg_store,
-            },
-            report_config=self.config,
-            forward_errors=warning_callback("GPG key search error"),
-            signals={
-                "result": on_result,
-            },
-        )
+        if self.config.experimental:
+            run_thread(
+                lambda: CertStore().import_cert(
+                    crypt.download_cert(
+                        keyserver=self.app_data.config.keyserver_url,
+                        identifier=key_identifier,
+                    ),
+                    CertType.Public,
+                ),
+                f_kwargs={},
+                report_config=self.config,
+                forward_errors=warning_callback("OpenPGP key search error"),
+                signals={
+                    "result": lambda cert: refresh_and_show_msg(
+                        cert.uid and str(cert.uid)
+                    )
+                },
+            )
+        else:
+            run_thread(
+                crypt.download_keys,
+                f_kwargs={
+                    "key_identifiers": [self.key_identifier.text()],
+                    "keyserver": self.config.keyserver_url,
+                    "gpg_store": self.config.gpg_store,
+                },
+                report_config=self.config,
+                forward_errors=warning_callback("OpenPGP key search error"),
+                signals={
+                    "result": on_result,
+                },
+            )
```

### Comparing `sett-4.2.0/sett/gui/keys_tab.py` & `sett-4.3.0/sett/gui/keys_tab.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,36 +3,40 @@
 import warnings
 import functools
 from pathlib import Path
 from typing import (
     Any,
     Callable,
     Iterator,
-    Sequence,
+    List,
     Tuple,
+    Union,
     cast,
 )
 
+from sett_rs.cert import CertInfo, CertStore, CertType, KeyType
 from libbiomedit.portal import KeyStatus
 
 from sett.core.error import UserError
 from .component import (
     GridLayoutCell,
     SelectionAction,
     ToolBar,
     grid_layout,
     warning_callback,
     NormalMessageBox,
 )
 from .key_generation_dialog import KeyGenDialog
 from .keys_download_dialog import KeyDownloadDialog
+from .cert_revocation_dialog import CertCreateRevocationDialog, CertRevokeDialog
+from .cert_migration_dialog import CertMigrationDialog
 from .model import AppData, KeyValueListModel
 from .parallel import run_thread
 from .pyside import QAction, QtCore, QtWidgets, open_window
-from .theme import Action, IconRepainterWidget
+from .theme import Action
 from ..core import crypt, gpg
 from ..workflows import upload_keys as upload_keys_workflow
 
 
 def open_message_box(
     *text: str,
     title: str,
@@ -62,15 +66,15 @@
     open_message_box, icon_type=QtWidgets.QMessageBox.Icon.Warning
 )
 open_info_msgbox = functools.partial(
     open_message_box, icon_type=QtWidgets.QMessageBox.Icon.Information
 )
 
 
-class KeysTab(IconRepainterWidget):
+class KeysTab(QtWidgets.QWidget):
     def __init__(self, parent: QtWidgets.QMainWindow, app_data: AppData):
         super().__init__(parent=parent)
         self.app_data = app_data
 
         self.text_panel = QtWidgets.QTextEdit()
         self.text_panel.setReadOnly(True)
 
@@ -102,15 +106,15 @@
             self,
         )
         action_generate_key.triggered.connect(
             lambda: KeyGenDialog(parent=self, app_data=app_data).show()
         )
         action_refresh_keys = Action(
             ":icon/feather/refresh-cw.png",
-            "Refresh keys from the local keyring",
+            "Refresh keys from the local keyring and refresh key status from portal",
             self,
         )
 
         def refresh_keys() -> None:
             """Fetch PGP key approval status from portal."""
             self.app_data.update_private_keys()
             self.app_data.update_public_keys()
@@ -145,14 +149,63 @@
                 (GridLayoutCell(self.text_panel, span=2),),
             )
         )
 
         # Fetch PGP key approval status from portal.
         refresh_keys()
 
+    def cert_to_html(self, cert: CertInfo) -> str:
+        """Represent a PGP key as an HTML string"""
+
+        # Add key info (user ID, key ID, fingerprint, signatures).
+        content = ["<table>"]
+        rows = [
+            ("User ID", html.escape(str(cert.uid))),
+            ("Key ID", cert.key_id),
+            ("Key fingerprint", cert.fingerprint),
+            (
+                "Key algorithm",
+                crypt.KeyAlgorithm(cert.primary_key.pub_key_algorithm).name,
+            ),
+            ("Key length", cert.primary_key.length),
+        ]
+        if cert.primary_key.key_type == KeyType.Public:
+            rows.append(("Validity", str(cert.validity)))
+        for k, v in rows:
+            content.append(f"<tr><th>{k}</th><td>{v}</td></tr>")
+        content.append("</td></tr></table>")
+        if cert.primary_key.revocation_reason:
+            for reason in cert.primary_key.revocation_reason:
+                content.append(f'<p class="danger">&#215; {reason}</p>')
+        # Add key validation info: display whether a key is approved or not.
+        if cert.primary_key.key_type == KeyType.Public:
+            if not self.app_data.config.verify_key_approval:
+                content.append(
+                    '<p class="info">Key approval cannot be verified because '
+                    "approval verification is disabled in your config file.</p>"
+                )
+            else:
+                cert_status = self.app_data.pub_key_status.get(
+                    cert.fingerprint, KeyStatus.UNKNOWN_KEY
+                )
+                if cert_status == KeyStatus.APPROVED:
+                    content.append('<p class="safe">&#x2714; This key is approved.</p>')
+                else:
+                    content.append(
+                        '<p class="danger">&#215; This key is not approved. '
+                        f"Status: {cert_status.value}"
+                    )
+        else:
+            content.append(
+                "<p>This is a private key. Private keys are not subject to "
+                "approval.</p>"
+            )
+
+        return "".join(content)
+
     def key_to_html(self, key: gpg.Key) -> str:
         """Represent a PGP key as an HTML string"""
 
         # Add key info (user ID, key ID, fingerprint, signatures).
         content = ["<table>"]
         rows = [
             ("User ID", html.escape(str(key.uids[0]))),
@@ -198,27 +251,27 @@
             content.append(
                 "<p>This is a private key. Private keys are not subject to "
                 "approval.</p>"
             )
         return "".join(content)
 
     @staticmethod
-    def key_to_text(key: gpg.Key) -> str:
-        uid = key.uids[0]
-        return f"{uid.email} ({key.key_id})"
+    def key_to_text(key: Union[gpg.Key, CertInfo]) -> str:
+        email = key.uids[0].email if isinstance(key, gpg.Key) else key.email
+        return f"{email} ({key.key_id})"
 
     def create_public_keys_actions(self) -> Iterator[QAction]:
         selection_model = self.pub_keys_view.selectionModel()
 
         # Create a dict of actions (functions) to associate to each
         # action button of the GUI.
         # The reason to create a dict object before looping over it is so
         # that mypy gets the correct typing information (for some reason
         # SelectionAction is not recognized as a subtype of QAction).
-        functions_by_action: Sequence[Tuple[QAction, Callable[..., Any]]] = (
+        functions_by_action: List[Tuple[QAction, Callable[..., Any]]] = [
             (
                 Action(
                     ":icon/feather/download-cloud.png",
                     "Download keys from the keyserver",
                     self,
                 ),
                 lambda: KeyDownloadDialog(parent=self, app_data=self.app_data).show(),
@@ -238,36 +291,93 @@
                     "Update selected keys from the keyserver",
                     self,
                     selection_model=selection_model,
                 ),
                 self.update_keys,
             ),
             (
-                SelectionAction(
-                    ":icon/feather/trash-2.png",
-                    "Delete selected keys from your computer",
-                    self,
-                    selection_model=selection_model,
-                ),
-                self.delete_keys,
-            ),
-            (
                 Action(
                     ":icon/feather/file-plus.png",
                     "Import key from file",
                     self,
                 ),
                 self.import_key,
             ),
-        )
+        ]
+        if self.app_data.config.experimental:
+            functions_by_action.extend(
+                [
+                    (
+                        SelectionAction(
+                            ":icon/feather/share.png",
+                            "Export key to file",
+                            self,
+                            selection_model=selection_model,
+                        ),
+                        self.export_certificate,
+                    ),
+                    (
+                        Action(
+                            ":icon/feather/edit-3.png",
+                            "Create revocation signature",
+                            self,
+                        ),
+                        lambda: CertCreateRevocationDialog(
+                            parent=self, app_data=self.app_data
+                        ).show(),
+                    ),
+                    (
+                        Action(
+                            ":icon/feather/flag.png",
+                            "Revoke certificate",
+                            self,
+                        ),
+                        lambda: CertRevokeDialog(
+                            parent=self, app_data=self.app_data
+                        ).show(),
+                    ),
+                    (
+                        Action(
+                            ":icon/feather/copy.png",
+                            "Migrate secret key from GnuPG",
+                            self,
+                        ),
+                        lambda: CertMigrationDialog(
+                            parent=self, app_data=self.app_data
+                        ).show(),
+                    ),
+                ]
+            )
+        else:
+            functions_by_action.append(
+                (
+                    SelectionAction(
+                        ":icon/feather/trash-2.png",
+                        "Delete selected keys from your computer",
+                        self,
+                        selection_model=selection_model,
+                    ),
+                    self.delete_keys,
+                )
+            )
+
         for action, fn in functions_by_action:
             action.triggered.connect(fn)
             yield action
 
-    def get_selected_keys(self) -> Tuple[gpg.Key, ...]:
+    def export_certificate(self) -> None:
+        for cert in self.get_selected_keys():
+            cert_ascii_armored = CertStore().export_cert(
+                cert.fingerprint, CertType.Public
+            )
+            QtWidgets.QFileDialog.saveFileContent(
+                cert_ascii_armored, f"{cert.fingerprint}.pub.asc"
+            )
+
+    def get_selected_keys(self) -> Tuple[Union[gpg.Key, CertInfo], ...]:
         """Returns the gpg.Key objects corresponding to the keys currently
         selected in the GUI.
         """
         # Note: it's probably possible to get rid of the cast() here.
         selected_keys = (
             cast(KeyValueListModel, index.model()).get_value(index)
             for index in self.pub_keys_view.selectedIndexes()
@@ -280,60 +390,86 @@
         if keys_to_update:
 
             def on_result() -> None:
                 self.app_data.update_public_keys()
                 self.update_display_selected_pub_key()
                 open_info_msgbox(
                     "Keys have been successfully updated.",
-                    title="Updated PGP keys",
+                    title="Updated OpenPGP keys",
                     parent=self.parentWidget(),
                 )
 
-            run_thread(
-                crypt.download_keys,
-                f_kwargs={
-                    "key_identifiers": [key.fingerprint for key in keys_to_update],
-                    "keyserver": self.app_data.config.keyserver_url,
-                    "gpg_store": self.app_data.config.gpg_store,
-                },
-                report_config=self.app_data.config,
-                forward_errors=warning_callback("GPG key update error"),
-                signals={"result": on_result},
-            )
+            if self.app_data.config.experimental:
+
+                def update_selected_certificates() -> None:
+                    for cert in keys_to_update:
+                        CertStore().import_cert(
+                            crypt.download_cert(
+                                keyserver=self.app_data.config.keyserver_url,
+                                identifier=cert.fingerprint,
+                            ),
+                            CertType.Public,
+                        )
+
+                run_thread(
+                    update_selected_certificates,
+                    f_kwargs={},
+                    report_config=self.app_data.config,
+                    forward_errors=warning_callback("OpenPGP key update error"),
+                    signals={"result": on_result},
+                )
+            else:
+                run_thread(
+                    crypt.download_keys,
+                    f_kwargs={
+                        "key_identifiers": [key.fingerprint for key in keys_to_update],
+                        "keyserver": self.app_data.config.keyserver_url,
+                        "gpg_store": self.app_data.config.gpg_store,
+                    },
+                    report_config=self.app_data.config,
+                    forward_errors=warning_callback("OpenPGP key update error"),
+                    signals={"result": on_result},
+                )
 
     def import_key(self) -> None:
         """Import a PGP key from a local file."""
         path = QtWidgets.QFileDialog.getOpenFileName(
-            self, "Select PGP key file", str(Path.home())
+            self, "Select OpenPGP key file", str(Path.home())
         )[0]
-        msgbox_title = "PGP public key import"
+        msgbox_title = "OpenPGP public key import"
         try:
             if path:
-                with open(path, encoding="utf-8") as fin:
-                    key_data = fin.read()
-                crypt.import_keys(key_data, self.app_data.config.gpg_store)
+                if self.app_data.config.experimental:
+                    with open(path, "rb") as fin:
+                        try:
+                            CertStore().import_cert(fin.read(), CertType.Public)
+                        except RuntimeError as e:
+                            raise UserError(str(e)) from e
+                else:
+                    with open(path, encoding="utf-8") as fin:
+                        crypt.import_keys(fin.read(), self.app_data.config.gpg_store)
                 self.app_data.update_private_keys()
                 self.app_data.update_public_keys()
                 self.update_display_selected_pub_key()
                 open_info_msgbox(
-                    "PGP key has been imported successfully.",
+                    "OpenPGP key has been imported successfully.",
                     title=msgbox_title,
                     parent=self,
                 )
         except (UnicodeDecodeError, UserError) as e:
             open_warning_msgbox(
                 "Error while importing PGP key.",
                 f"Detailed reason: {format(e)}",
                 title=msgbox_title,
                 parent=self,
             )
 
     def delete_keys(self) -> None:
         """Delete the selected public keys from the user's local keyring. Only
-        public keys with no associated private key can be deleted.
+        public keys with no associated secret key can be deleted.
         """
         keys_to_delete = self.get_selected_keys()
         user_answer = open_message_box(
             "Do you really want to delete the following public key(s)?",
             "<br />".join([self.key_to_text(key) for key in keys_to_delete]),
             title="Delete public key",
             parent=self.parentWidget(),
@@ -408,19 +544,21 @@
                         f_kwargs={
                             "fingerprints": [key.fingerprint],
                             "verify_key": cb.isChecked(),
                             "config": self.app_data.config,
                         },
                         capture_loggers=(upload_keys_workflow.logger,),
                         report_config=self.app_data.config,
-                        forward_errors=warning_callback("GPG key upload error"),
+                        forward_errors=warning_callback(
+                            "OpenPGP certificate upload error"
+                        ),
                         signals={
                             "result": lambda _: open_info_msgbox(
-                                "Key has been successfully uploaded to keyserver.",
-                                title="Sent PGP keys",
+                                "OpenPGP certificate successfully uploaded to keyserver.",
+                                title="Sent OpenPGP certificate",
                                 parent=self.parentWidget(),
                             )
                         },
                     )
 
     def _update_display(self, index: QtCore.QModelIndex) -> None:
         """Display key info summary in GUI text panel."""
@@ -432,29 +570,33 @@
             "</style>"
         )
         if index.isValid():
             try:
                 # Note: it's probably possible to get rid of the cast() here.
                 self.text_panel.setHtml(
                     style
-                    + self.key_to_html(
+                    + self.cert_to_html(
+                        cast(KeyValueListModel, index.model()).get_value(index)
+                    )
+                    if self.app_data.config.experimental
+                    else self.key_to_html(
                         cast(KeyValueListModel, index.model()).get_value(index)
                     )
                 )
             except IndexError:
                 self.text_panel.setHtml("")
 
     def update_display_selected_pub_key(self) -> None:
         """Refresh the displayed key info of the currently selected public keys."""
         self._update_display(self.pub_keys_view.selectionModel().currentIndex())
 
 
 def verify_key_length(
     parent: QtWidgets.QWidget,
-    key: gpg.Key,
+    key: Union[gpg.Key, CertInfo],
 ) -> int:
     """Verifies length and type of the given key.
 
     If some warning or error is caught, an additional popup (asking for user
     interaction) is displayed. If this is NOT the case, it simply return
     `QtWidgets.QMessageBox.Ok` (meaning everything is fine).
     """
```

### Comparing `sett-4.2.0/sett/gui/listener.py` & `sett-4.3.0/sett/gui/listener.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,15 @@
         """Each time an attribute is set, check whether it is being watched,
         and if so, run the associated functions."""
         self.set_value(attr, val)
         self._trigger(attr)
 
     def add_listener(self, attr: str, callback: Callable[[], Any]) -> None:
         """Add a listener to the specified attribute. Each time the value of
-        the attributed will change, the specified callback function(s) will
-        be called.
+        the attribute changes, the specified callback function(s) is called.
         """
         self._listeners[attr].append(callback)
 
 
 class ClassWithListener(Listener):
     def set_value(self, attr: str, val: Any) -> None:
         super().__setattr__(attr, val)
```

### Comparing `sett-4.2.0/sett/gui/main_window.py` & `sett-4.3.0/sett/gui/main_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,37 +14,37 @@
 from .decrypt_tab import DecryptTab
 from .encrypt_tab import EncryptTab
 from .keys_tab import KeysTab
 from .model import AppData, ConfigProxy
 from .parallel import run_thread
 from .pyside import QtCore, QtGui, QtWidgets, open_window
 from .settings_tab import SettingsTab
-from .theme import Icon, IconRepainter, Action, IconRepainterWidget
+from .theme import Icon, IconRepainter, Action, get_icon_repainter
 from .transfer_tab import TransferTab
 from ..core.versioncheck import check_version
 from ..utils.config import Config, load_config, save_config, config_to_dict
 
 QtCore.QThreadPool.globalInstance().setExpiryTimeout(-1)
 
 
 @dataclass(frozen=True)
 class Tab:
     icon_file_name: str
     label: str
     component: Type[QtWidgets.QWidget]
 
 
-class MainWindow(QtWidgets.QMainWindow, IconRepainterWidget):
+class MainWindow(QtWidgets.QMainWindow):
     """Class that initializes the main QtWidget (window) of the application,
     onto which all other components will be added.
     """
 
     def __init__(self, icon_repainter: IconRepainter) -> None:
         super().__init__()
-        self._icon_repainter = icon_repainter
+        self.icon_repainter = icon_repainter
         self.app_data = AppData(config=ConfigProxy(self.load_config_from_disk()))
         self.tabs = (
             Tab(":icon/feather/lock.png", "&Encrypt", EncryptTab),
             Tab(":icon/feather/send.png", "&Transfer", TransferTab),
             Tab(":icon/feather/unlock.png", "&Decrypt", DecryptTab),
             Tab(":icon/feather/key.png", "&Keys", KeysTab),
             Tab(":icon/feather/settings.png", "&Settings", SettingsTab),
@@ -71,27 +71,28 @@
         tab_widget = QtWidgets.QTabWidget()
         for tab in self.tabs:
             tab_widget.addTab(
                 tab.component(parent=self, app_data=self.app_data),  # type: ignore
                 Icon(tab.icon_file_name),
                 tab.label,
             )
-        self.icon_repainter().register(self.repaint_tab_icons)
+        get_icon_repainter(self).register(self.repaint_tab_icons)
         scrollArea = QtWidgets.QScrollArea(self)
         scrollArea.setWidget(tab_widget)
         scrollArea.setWidgetResizable(True)
         self.setCentralWidget(scrollArea)
 
     def repaint_tab_icons(self) -> None:
         for i, tab in enumerate(self.tabs):
             self.tab_widget.setTabIcon(i, Icon(tab.icon_file_name))
 
     @property
     def tab_widget(self) -> QtWidgets.QTabWidget:
-        return cast(QtWidgets.QTabWidget, self.centralWidget())
+        scroll_area = cast(QtWidgets.QScrollArea, self.centralWidget())
+        return cast(QtWidgets.QTabWidget, scroll_area.widget())
 
     def add_status_bar(self) -> None:
         self.status = QtWidgets.QStatusBar()
         self.setStatusBar(self.status)
 
     def add_menu(self) -> None:
         action_exit = Action(":icon/feather/log-out.png", "&Exit", self)
```

### Comparing `sett-4.2.0/sett/gui/model.py` & `sett-4.3.0/sett/gui/model.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     Union,
     Sequence,
     Type,
     cast,
     TYPE_CHECKING,
 )
 
+from sett_rs.cert import CertInfo, CertStore, CertType
 from libbiomedit.portal import KeyStatus
 
 from .listener import ClassWithListener
 from .listener import ListenerWrap
 from .pyside import QtCore
 from ..core import gpg
 from ..core.metadata import Purpose
@@ -116,14 +117,17 @@
         self.set_data(data or [])
 
     def set_data(self, data: Iterable[Tuple[Hashable, Any]]) -> None:
         self._keyvalues = dict(data)
         self._keys = list(self._keyvalues.keys())
         self.layoutChanged.emit()
 
+    def get_data(self) -> Dict[Hashable, Any]:
+        return self._keyvalues
+
     # Default value Qt.DisplayRole for index is not an int (upstream issue):
     def data(self, index, role) -> Optional[Hashable]:  # type: ignore
         if role == QtCore.Qt.ItemDataRole.DisplayRole:
             key: Hashable = self._keys[index.row()]
             return key
         return None
 
@@ -225,53 +229,99 @@
     transfer_files: QtCore.QStringListModel = field(
         default_factory=QtCore.QStringListModel
     )
 
     priv_keys_model: KeyValueListModel = field(default_factory=KeyValueListModel)
     pub_keys_model: KeyValueListModel = field(default_factory=KeyValueListModel)
     pub_key_status: Dict[str, KeyStatus] = field(default_factory=dict)
+    encrypt_recipients_model: TableModel = field(
+        default_factory=lambda: TableModel(columns=("Name", "Email", "Fingerprint"))
+    )
     default_key_index: Optional[int] = None
 
     def update_private_keys(self) -> None:
         """Retrieve/reload all private keys from the user's local keyring and
-        store them in the application's memory."""
-        keys_private = self.config.gpg_store.list_sec_keys()
-        try:
-            default_key = (
-                self.config.default_sender or self.config.gpg_store.default_key()
-            )
-            self.default_key_index = next(
-                index
-                for index, entry in enumerate(keys_private)
-                if entry.fingerprint == default_key
-            )
-            self.encrypt_sender = default_key
-        except StopIteration:
-            pass
-        self.priv_keys_model.set_data(data=keys_as_tuple(keys=keys_private))
+        store them in the application's memory.
+        """
+        if self.config.experimental:
+            certs = CertStore().list_certs(CertType.Secret)
+            try:
+                self.default_key_index = next(
+                    index
+                    for index, entry in enumerate(certs)
+                    if entry.fingerprint == self.config.default_sender
+                )
+                self.encrypt_sender = self.config.default_sender
+            except StopIteration:
+                pass
+            self.priv_keys_model.set_data(data=certs_as_tuple(certs))
+        else:
+            keys_private = self.config.gpg_store.list_sec_keys()
+            try:
+                default_key = (
+                    self.config.default_sender or self.config.gpg_store.default_key()
+                )
+                self.default_key_index = next(
+                    index
+                    for index, entry in enumerate(keys_private)
+                    if entry.fingerprint == default_key
+                )
+                self.encrypt_sender = default_key
+            except StopIteration:
+                pass
+            self.priv_keys_model.set_data(data=keys_as_tuple(keys=keys_private))
+        self.priv_keys_model.endResetModel()
 
     def update_public_keys(self) -> None:
         """Retrieve/reload all public keys from the user's local keyring and
-        store them in the application's memory."""
-        keys_public = self.config.gpg_store.list_pub_keys(sigs=True)
-        self.pub_keys_model.set_data(data=keys_as_tuple(keys=keys_public))
+        store them in the application's memory.
+        """
+
+        if self.config.experimental:
+            certs = CertStore().list_certs(CertType.Public)
+            self.pub_keys_model.set_data(data=certs_as_tuple(certs))
+        else:
+            keys_public = self.config.gpg_store.list_pub_keys(sigs=True)
+            self.pub_keys_model.set_data(data=keys_as_tuple(keys=keys_public))
+        self.pub_keys_model.endResetModel()
+
+        # Go through the list of currently selected data recipients (displayed
+        # in the encrypt tab) to make sure all keys are still present. If a
+        # selected key is no longer available, it gets removed.
+        available_pub_keys = [
+            k.fingerprint for k in self.pub_keys_model.get_data().values()
+        ]
+        for index, row in list(enumerate(self.encrypt_recipients_model.get_data()))[
+            ::-1
+        ]:
+            fingerprint = row[2]
+            if fingerprint not in available_pub_keys:
+                self.encrypt_recipients_model.removeRow(index)
 
     def update_key_approval_status(self) -> None:
         """Check whether public keys from the user's local keyring are approved
         in the portal and store/update this information in the application's
         memory.
         If no keys are present in the user's local PGP keyring, the request to
         the Portal's API is skipped.
         """
-        fingerprints = tuple(
-            k.fingerprint for k in self.config.gpg_store.list_pub_keys()
-        )
-        self.pub_key_status = (
-            self.config.portal_api.get_key_status(fingerprints) if fingerprints else {}
-        )
+        if self.config.verify_key_approval:
+            if self.config.experimental:
+                fingerprints = [
+                    cert.fingerprint for cert in CertStore().list_certs(CertType.Public)
+                ]
+            else:
+                fingerprints = [
+                    k.fingerprint for k in self.config.gpg_store.list_pub_keys()
+                ]
+            self.pub_key_status = (
+                self.config.portal_api.get_key_status(fingerprints)
+                if fingerprints
+                else {}
+            )
 
     def __post_init__(self) -> None:
         super().__init__()
         if self.config.output_dir:
             self.encrypt_output_location = Path(self.config.output_dir)
             self.decrypt_output_location = Path(self.config.output_dir)
         if self.config.compression_level is not None:
@@ -282,7 +332,17 @@
         self.update_private_keys()
         self.update_public_keys()
 
 
 def keys_as_tuple(keys: Sequence[gpg.Key]) -> Iterable[Tuple[str, gpg.Key]]:
     """Returns a generator of tuples of the form ("userID keyID", key)."""
     return ((f"{key.uids[0]} {key.key_id}", key) for key in keys)
+
+
+def certs_as_tuple(
+    certs: Sequence[CertInfo],
+) -> Iterable[Tuple[str, CertInfo]]:
+    """Returns a generator of tuples of the form ("userID keyID", cert)."""
+    return (
+        (f"{'' if cert.uid is None else str(cert.uid)} {cert.key_id}", cert)
+        for cert in certs
+    )
```

### Comparing `sett-4.2.0/sett/gui/parallel.py` & `sett-4.3.0/sett/gui/parallel.py`

 * *Files identical despite different names*

### Comparing `sett-4.2.0/sett/gui/pyside.py` & `sett-4.3.0/sett/gui/pyside.py`

 * *Files identical despite different names*

### Comparing `sett-4.2.0/sett/gui/resources/rc_icons.py` & `sett-4.3.0/sett/gui/resources/rc_icons.py`

 * *Files identical despite different names*

### Comparing `sett-4.2.0/sett/gui/settings_tab.py` & `sett-4.3.0/sett/gui/settings_tab.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     LineEdit,
     SpinBox,
     grid_layout,
     GridLayoutCell,
 )
 from .model import AppData, ConfigProxy
 from .pyside import QtCore, QtGui, QtWidgets, open_window
-from .theme import Icon, IconRepainterWidget, PushButton
+from .theme import Icon, PushButton, get_icon_repainter
 from .ui_model_bind import (
     bind,
     TextControl,
     PathControl,
     BoolControl,
     NumericControl,
 )
@@ -52,15 +52,15 @@
     for row in items:
         aligned: List[Any] = []
         for col in row:
             aligned.extend(chain(col, repeat(None, longest - len(col))))
         yield tuple(aligned)
 
 
-class SettingsTab(IconRepainterWidget):
+class SettingsTab(QtWidgets.QWidget):
     """Class that builds the tab where users can modify the settings of their
     application.
     """
 
     persist_btn_text = "Save to config file"
     persist_btn_icon_file_name = ":icon/feather/save.png"
 
@@ -119,14 +119,15 @@
                         ((label_field("Miscellaneous"),), ()),
                         (cfg_field("repo_url"), cfg_field("log_dir")),
                         (cfg_field("check_version"), cfg_field("log_max_file_number")),
                         (
                             cfg_field("gui_quit_confirmation"),
                             cfg_field("error_reports"),
                         ),
+                        (cfg_field("experimental"),),
                     )
                 )
             )
         )
         layout.addStretch()
         layout.addWidget(self._footer())
         self.setLayout(layout)
@@ -140,15 +141,15 @@
             QtWidgets.QLineEdit, widget_register["keyserver_url"]
         )
         self._enable_checkbox_key_autodownload()
         self.field_keyserver_url.textChanged.connect(
             self._enable_checkbox_key_autodownload
         )
         self.config_proxy.refresh()
-        self.icon_repainter().register(self.refresh_icon)
+        get_icon_repainter(self).register(self.refresh_icon)
 
     def _save_config_to_disk(self) -> None:
         """Write the current in-app config values to a config file on disk."""
         config.save_config(config.config_to_dict(self.config_proxy.get_config()))
         msg = NormalMessageBox(parent=self, window_title="Settings")
         msg.setIcon(QtWidgets.QMessageBox.Icon.Information)
         msg.setText(f'Successfully saved settings to "{get_config_file()}"')
@@ -329,15 +330,15 @@
 
 
 def widget_path(
     config_proxy: ConfigProxy,
     config_key: str,
     status_tip: str,
     file_type: FileType,
-    parent: IconRepainterWidget,
+    parent: QtWidgets.QWidget,
 ) -> Tuple[QtWidgets.QWidget, ...]:
     """Return a path widget associated with the specified setting `config_key`."""
     widget = PathInput(
         directory=file_type is FileType.directory, path=None, parent=parent
     )
     widget.setStatusTip(status_tip)
     bind(config_proxy, config_key, widget, PathControl)
@@ -407,16 +408,15 @@
 widget_by_type: Dict[type, Callable[..., Tuple[QtWidgets.QWidget, ...]]] = {
     int: widget_int,
     bool: widget_bool,
     str: widget_str,
 }
 
 
-# TODO: when dropping support for python 3.7, remove quotes around "Field"
-#       and Field will no longer need to be imported.
+# TODO: when dropping support for python 3.8, remove quotes around "Field".
 def widget_row_from_field(
     config_proxy: ConfigProxy,
     field: "Field[Any]",
     widget_register: Optional[Dict[str, QtWidgets.QWidget]] = None,
     parent: Optional[QtWidgets.QWidget] = None,
 ) -> Tuple[QtWidgets.QWidget, ...]:
     """Create a widget row consisting of a label, a main widget and possible
```

### Comparing `sett-4.2.0/sett/gui/transfer_tab.py` & `sett-4.3.0/sett/gui/transfer_tab.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     hbox_layout,
     GridLayoutCell,
     NormalMessageBox,
 )
 from .file_selection_widget import ArchiveOnlyFileSelectionWidget
 from .model import new_sftp_connection, AppData
 from .pyside import QtCore, QtGui, QtWidgets, QAction, open_window
-from .theme import Action, IconRepainterWidget
+from .theme import Action
 from .ui_model_bind import (
     bind,
     TextControl,
     OptionalTextControl,
     OptionalPasswordControl,
     OptionalPathControl,
     BoolControl,
@@ -54,26 +54,26 @@
 
     def create_button(self) -> QtWidgets.QRadioButton:
         btn = QtWidgets.QRadioButton(self.value)
         btn.setStatusTip(self.status_tip)
         return btn
 
     def create_options_panel(
-        self, data: AppData, parent: IconRepainterWidget
+        self, data: AppData, parent: QtWidgets.QWidget
     ) -> QtWidgets.QGroupBox:
         if self is TransferProtocol.sftp:
             return self._create_sftp_options_panel(data, parent)
         if self is TransferProtocol.s3:
             return self._create_s3_options_panel(data)
         if self is TransferProtocol.liquid_files:
             return self._create_lf_options_panel(data)
         raise RuntimeError("Unreachable")
 
     def _create_sftp_options_panel(
-        self, data: AppData, parent: IconRepainterWidget
+        self, data: AppData, parent: QtWidgets.QWidget
     ) -> QtWidgets.QGroupBox:
         args = data.transfer_protocol_args[Sftp]
         text_username = LineEdit()
         text_username.setStatusTip("Username on the SFTP server")
         bind(args, "username", text_username, TextControl)
 
         text_destination_dir = LineEdit()
@@ -494,14 +494,15 @@
                 "pkg_name_suffix": self.app_data.encrypt_package_name_suffix,
                 "progress": GuiProgress(self.progress_bar.setValue),
                 "two_factor_callback": second_factor_callback,
             },
             capture_loggers=(
                 transfer.logger,
                 protocols.sftp.logger,
+                protocols.sftp.logger_rs,
                 protocols.s3.logger,
             ),
             ignore_exceptions=True,
             report_config=self.app_data.config,
         )
```

### Comparing `sett-4.2.0/sett/gui/ui_model_bind.py` & `sett-4.3.0/sett/gui/ui_model_bind.py`

 * *Files identical despite different names*

### Comparing `sett-4.2.0/sett/protocols/__init__.py` & `sett-4.3.0/sett/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `sett-4.2.0/sett/protocols/liquid_files.py` & `sett-4.3.0/sett/protocols/liquid_files.py`

 * *Files identical despite different names*

### Comparing `sett-4.2.0/sett/protocols/multipart.py` & `sett-4.3.0/sett/protocols/multipart.py`

 * *Files identical despite different names*

### Comparing `sett-4.2.0/sett/protocols/s3.py` & `sett-4.3.0/sett/protocols/s3.py`

 * *Files identical despite different names*

### Comparing `sett-4.2.0/sett/protocols/sftp.py` & `sett-4.3.0/sett/protocols/sftp.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 from . import protocol
 
 # Re-exports
 SSHException = _SSHException
 
 
 logger = create_logger(__name__)
+logger_rs = create_logger("sett.sftp")
 
 
 def opt_reverse_expanduser(path: Optional[str]) -> Optional[str]:
     return reverse_expanduser(path) if path else None
 
 
 @dataclass
@@ -77,17 +78,16 @@
     pkey_password_encoding: str = (
         "utf_8"  # nosec (False Positive: pkey_password_encoding)
     )
     jumphost: Optional[str] = None
     buffer_size: int = 1048576
 
     def __post_init__(self) -> None:
-        # Turn empty strings into None and check that the ssh key file exists
+        # Check that the ssh key file exists.
         self.pkey = os.path.expanduser(self.pkey) if self.pkey else None
-        self.pkey_password = self.pkey_password or None
 
     def required_password_args(self) -> Sequence[str]:
         if self.pkey is not None and self.pkey_password is None:
             return ("pkey_password",)
         return ()
 
     def upload(
@@ -102,40 +102,48 @@
         if self.jumphost:
             self.upload_paramiko(
                 files, progress=progress, two_factor_callback=two_factor_callback
             )
         else:
             host, port = parse_host(self.host)
             try:
-                sett_rs.sftp_upload(
+                sftp_opts = sett_rs.workflow.SftpOpts(
+                    host=host,
+                    port=port,
+                    username=self.username,
+                    base_path=self.destination_dir,
+                    envelope_dir=self.envelope_dir,
+                    pkey=self.pkey,
+                    pkey_password=reveal(self.pkey_password),
+                    buf_size=self.buffer_size,
+                )
+                sett_rs.workflow.transfer(
                     files,
-                    f"{host}:{port}",
-                    self.username,
-                    self.destination_dir,
-                    self.envelope_dir,
-                    self.pkey,
-                    reveal(self.pkey_password),
-                    progress.update if progress is not None else None,
+                    destination=sftp_opts,
+                    progress=progress.update if progress is not None else None,
                     two_factor_callback=two_factor_callback,
-                    buf_size=self.buffer_size,
                 )
             except RuntimeError as e:
                 logger.warning(format(e))
                 self.upload_paramiko(
                     files, progress=progress, two_factor_callback=two_factor_callback
                 )
 
     def upload_paramiko(
         self,
         files: Sequence[str],
         two_factor_callback: Callable[[], str],
         progress: Optional[ProgressInterface] = None,
     ) -> None:
-        if self.envelope_dir is None:
-            envelope_dir = datetime.now().strftime(ENVELOPE_DIR_FMT)
+        envelope_dir = (
+            datetime.now().strftime(ENVELOPE_DIR_FMT)
+            if self.envelope_dir is None
+            else self.envelope_dir
+        )
+
         progress_callback = (
             (lambda x, y: progress.update(x / y)) if progress is not None else None
         )
         remote_dir = PurePosixPath(self.destination_dir) / envelope_dir
         try:
             with sftp_connection(
                 host=self.host,
```

### Comparing `sett-4.2.0/sett/utils/config.py` & `sett-4.3.0/sett/utils/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,15 @@
 import platform
 import warnings
 import dataclasses
 from dataclasses import dataclass, field as _field, fields
 from pathlib import Path
 from typing import Dict, Optional, Callable, Union, Any
 
-# TODO: this can be removed when support for python 3.7 is dropped, as
-#       typing.get_args is natively present in python >= 3.8.
-try:
-    from typing import get_args
-except ImportError:
-    from typing_extensions import get_args
+from typing import get_args
 
 from libbiomedit.lib import deserialize as serialization
 from libbiomedit.portal import PortalApi
 
 from .log import get_default_log_dir, create_logger
 from .validation import REGEX_FQDN, PACKAGE_SUFFIX
 from .get_config_path import get_config_file, CONFIG_FILE_NAME
@@ -260,14 +255,20 @@
     )
     verify_dtr: bool = field_ext(
         default=True,
         label="Verify DTR",
         description="Verify that the given Data Transfer ID is valid and the "
         "associated metadata is correct.",
     )
+    experimental: bool = field_ext(
+        default=False,
+        label="Enable experimental features",
+        description="REQUIRES APPLICATION RESTART. Warning: enabling experimental "
+        "features may cause unexpected errors.",
+    )
 
     def __post_init__(self) -> None:
         for url in ("dcc_portal_url", "repo_url"):
             setattr(
                 self, url, getattr(self, url).rstrip("/")  # pylint: disable=no-member
             )
 
@@ -288,16 +289,15 @@
          * There is no key approval verification. If keys do not need to be
            approved by a central key authority, auto-downloading them presents
            a security risk (keys should be manually downloaded and checked) and
            is therefore not allowed.
         """
         return self.gpg_key_autodownload and self.verify_key_approval
 
-    # TODO: when dropping support for python 3.7, remove quotes around "Field"
-    #       and dataclasses.Field will no longer need to be imported.
+    # TODO: when dropping support for python 3.8, remove quotes around "Field".
     @classmethod
     def get_field(cls, arg: str) -> "dataclasses.Field[Any]":
         """Return the class field corresponding to the argument `arg`.
 
         :raise ValueError: if the specified `arg` is not an argument of the
             class.
         """
```

### Comparing `sett-4.2.0/sett/utils/error_handling.py` & `sett-4.3.0/sett/utils/error_handling.py`

 * *Files identical despite different names*

### Comparing `sett-4.2.0/sett/utils/get_config_path.py` & `sett-4.3.0/sett/utils/get_config_path.py`

 * *Files identical despite different names*

### Comparing `sett-4.2.0/sett/utils/log.py` & `sett-4.3.0/sett/utils/log.py`

 * *Files identical despite different names*

### Comparing `sett-4.2.0/sett/utils/progress.py` & `sett-4.3.0/sett/utils/progress.py`

 * *Files identical despite different names*

### Comparing `sett-4.2.0/sett/workflows/config.py` & `sett-4.3.0/sett/workflows/config.py`

 * *Files identical despite different names*

### Comparing `sett-4.2.0/sett/workflows/decrypt.py` & `sett-4.3.0/sett/workflows/decrypt.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import os
+import json
 from functools import partial
 from typing import List, Optional
 
+import sett_rs
+from sett_rs.cert import CertInfo, CertStore, CertType
+
 from ..core import gpg
 from ..core.archive import (
     check_package,
     extract,
     unpack_from_stream,
     DATA_ARCHIVE,
     DATA_FILE_ENCRYPTED,
@@ -24,21 +28,23 @@
     get_compression_stats,
     get_total_size,
     to_human_readable_size,
     unique_filename,
     check_space,
 )
 from ..core.checksum import verify_checksums, read_checksum_file
+from ..core.metadata import METADATA_FILE, load_metadata
 from ..core.secret import Secret
 from ..core.error import UserError
 from ..utils.log import create_logger, log_runtime_info, log_timing
 from ..utils.progress import ProgressInterface, subprogress
 from ..utils.config import Config
 
 logger = create_logger(__name__)
+logger_rs = create_logger("sett.decrypt")
 
 
 @log_timing(logger)
 @log_runtime_info(logger)
 def decrypt(
     files: List[str],
     *,
@@ -72,22 +78,90 @@
 
     for archive_file in files:
         with logger.log_task(f"Processing file: {archive_file}..."):
             # Reset progress bar for each archive file.
             if progress is not None:
                 progress.update(0.0)
 
-            decrypt_archive(
-                archive_file,
-                passphrase=passphrase,
-                output_dir=output_dir,
-                config=config,
-                decrypt_only=decrypt_only,
-                progress=progress,
+            if config.experimental:
+                _decrypt_archive_experimental(
+                    archive_file,
+                    passphrase=passphrase,
+                    output_dir=output_dir,
+                    config=config,
+                    decrypt_only=decrypt_only,
+                    progress=progress,
+                )
+            else:
+                decrypt_archive(
+                    archive_file,
+                    passphrase=passphrase,
+                    output_dir=output_dir,
+                    config=config,
+                    decrypt_only=decrypt_only,
+                    progress=progress,
+                )
+
+
+def _decrypt_archive_experimental(
+    archive_file: str,
+    passphrase: Optional[Secret[str]],
+    output_dir: str,
+    config: Config,
+    decrypt_only: bool = False,
+    progress: Optional[ProgressInterface] = None,
+) -> None:
+    """Decrypts and decompresses a data package using sett-rs."""
+
+    with extract(archive_file, METADATA_FILE) as f_data:
+        passphrase = enforce_passphrase(passphrase)
+        metadata = load_metadata(json.load(f_data))
+        logger.debug("Recipients: %s", ", ".join(metadata.recipients))
+        store = CertStore()
+        recipients_certs = []
+        for recipient_fp in metadata.recipients:
+            try:
+                recipients_certs.append(
+                    store.export_cert(recipient_fp, CertType.Secret)
+                )
+            except RuntimeError as e:
+                logger.debug("Unable to retrieve recipient's certificate: %s", e)
+        if not recipients_certs:
+            raise UserError(
+                "No secret key was found that is able to decrypt the data. "
+                "Please make sure your secret key is present on the local "
+                "machine and that the data was encrypted for you."
             )
+        logger.info(
+            "Data encrypted for: %s",
+            ", ".join(
+                f"{cert_info.uid} ({cert_info.fingerprint})"
+                for cert_info in (
+                    CertInfo.from_bytes(cert) for cert in recipients_certs
+                )
+            ),
+        )
+        try:
+            sender_cert = store.export_cert(metadata.sender, CertType.Public)
+        except RuntimeError as e:
+            raise UserError(f"Unable to retrieve sender's key: {e}") from e
+
+    sett_rs.workflow.decrypt(
+        opts=sett_rs.workflow.DecryptOpts(
+            file=archive_file,
+            recipients=recipients_certs,
+            signer=sender_cert,
+            password=passphrase.reveal(),
+            dry_run=False,
+            decrypt_only=decrypt_only,
+            output=output_dir,
+            max_cpu=config.max_cpu,
+        ),
+        progress=progress.update if progress is not None else None,
+    )
 
 
 def decrypt_archive(
     archive_file: str,
     passphrase: Optional[Secret[str]],
     output_dir: str,
     config: Config,
```

### Comparing `sett-4.2.0/sett/workflows/encrypt.py` & `sett-4.3.0/sett/workflows/encrypt.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 import os
 from pathlib import Path
 from datetime import datetime
 from functools import partial
 from typing import List, Optional, Callable, Tuple, Iterable, Any, TypeVar
 from zipfile import ZipFile, ZipInfo, ZIP_STORED
 
+import sett_rs
+from sett_rs.cert import CertStore, CertType
+
 from ..core import gpg
 from ..core.metadata import METADATA_FILE, METADATA_FILE_SIG
 from ..core.archive import (
     write_tar,
     ArchiveInMemoryFile,
     ArchiveFile,
     ArchiveFileBase,
@@ -41,14 +44,15 @@
 from ..core.secret import Secret
 from ..utils.progress import ProgressInterface, subprogress, progress_file_iter
 from ..utils.config import Config
 from ..utils.log import create_logger, log_runtime_info, log_timing
 
 DATE_FMT_FILENAME = "%Y%m%dT%H%M%S"
 logger = create_logger(__name__)
+logger_rs = create_logger("sett.encrypt")
 
 
 def check_path(
     directory: bool = False, writable: bool = False
 ) -> Callable[[str], None]:
     """Generate a 'type definition' function that will check that a string is
     a valid path (file or directory).
@@ -105,138 +109,169 @@
 
 
 check_compression_level = check_integer_in_range(min_value=0, max_value=9)
 
 
 @log_timing(logger)
 @log_runtime_info(logger)
-def encrypt(  # pylint: disable=too-many-statements
+def encrypt(
     files: List[str],
-    *,
     config: Config,
-    recipient: List[str],
+    sender: str,
+    recipients: List[str],
     dtr_id: Optional[int] = None,
-    sender: Optional[str] = None,
     passphrase: Optional[Secret[str]] = None,
     output: Optional[str] = None,
     output_suffix: Optional[str] = None,
     dry_run: bool = False,
     force: bool = False,
-    compression_level: Optional[int] = None,
+    compression_level: int = 5,
     purpose: Optional[Purpose] = None,
     progress: Optional[ProgressInterface] = None,
 ) -> Optional[str]:
     """Compress and encrypt files and/or directories.
 
     Main function of the encryption workflow. It compresses the input files
     into a single archive file, which is then encrypted for the specified
     recipients and signed by the specified sender.
-
     Finally, the encrypted data is bundled with a metadata file in a single
     .zip archive.
-
     The function returns the file name of the created data package.
     """
 
     with logger.log_task(
         f"Input data verification{' (dry_run)' if dry_run else ''}..."
     ):
-        # Verify user has specified at least 1 file to encrypt and that the
-        # file(s) have read permission for the user.
-        logger.info("Verify files to encrypt")
-        if not files:
-            raise UserError("Empty file list.")
-        files_to_encrypt = list(search_files_recursively(files))
-        if not files_to_encrypt:
-            raise UserError(
-                "No input files found. Did you try encrypting an empty directory?"
-            )
-        check_file_read_permission(files_to_encrypt)
-
-        # If no sender is specified, retrieve default sender from config.
-        if sender is None:
-            sender = config.default_sender or config.gpg_store.default_key()
-            if sender is None:
-                raise UserError("Sender not specified with no default sender.")
-
-        # If no compression level is specified, retrieve it from config.
-        if compression_level is None:
-            compression_level = config.compression_level
         check_arg_value(
             arg_value=compression_level,
             arg_name="compression level",
             arg_type_checker=check_compression_level,
         )
 
-        # Retrieve the sender's and recipients' public keys:
-        #  - sender public key : the matching private key will be used to
-        #                        encrypt data.
-        #  - recipient public key: needed to encrypt the data.
-        #
-        # The sender/recipient information can be either an email, a keyID or
-        # a full fingerprint.
-        logger.info("Retrieve sender and recipient GnuPG keys")
-        sender_pub_key, *recipients_pub_key = retrieve_refresh_and_validate_keys(
-            key_identifiers=(sender, *recipient),
+    if config.experimental:
+        return _encrypt_experimental(
+            files=files,
             config=config,
+            sender_fingerprint=sender,
+            recipients_fingerprints=recipients,
+            passphrase=passphrase,
+            output=output,
+            output_suffix=output_suffix,
+            dtr_id=dtr_id,
+            dry_run=dry_run,
+            force=force,
+            compression_level=compression_level,
+            purpose=purpose,
+            progress=progress,
         )
 
-        # Verify a private key matching the user's public key exists. The key
-        # itself is not needed because it shares the fingerprint with the
-        # public key.
-        search_priv_key(sender_pub_key.fingerprint, config.gpg_store)
-        logger.info(
-            "Sender: %s",
-            f"{sender_pub_key.uids[0]} ({sender_pub_key.fingerprint})",
-        )
-        logger.info(
-            "Recipients: %s",
-            ", ".join(
-                f"{key.uids[0]} ({key.fingerprint})" for key in recipients_pub_key
-            ),
-        )
+    return _encrypt_stable(
+        files=files,
+        config=config,
+        sender=sender,
+        recipients=recipients,
+        passphrase=passphrase,
+        output=output,
+        output_suffix=output_suffix,
+        compression_level=compression_level,
+        dtr_id=dtr_id,
+        dry_run=dry_run,
+        force=force,
+        purpose=purpose,
+        progress=progress,
+    )
 
-        # If requested, verify data transfer related information.
-        if config.verify_dtr:
-            logger.info("Verify Data Transfer ID")
-            # Connect to the portal API to retrieve the code (abbreviation)
-            # associated with the DTR ID.
-            project_code = verify_dtr_info_and_get_project_code(
-                dtr_id, purpose, config, sender_pub_key, recipients_pub_key
-            )
-            logger.info("DTR ID '%s' is valid for project '%s'", dtr_id, project_code)
-        else:
-            project_code = None
-
-        logger.info("Verify available disk space")
-
-        # The default value for the output name is based on date and time
-        # when the script is being run.
-        # Example output name: "20191011T145012.zip".
-        timestamp = datetime.now().astimezone()
-        output_name = generate_output_archive_name(
-            prefix=project_code,
-            timestamp=timestamp,
-            suffix=output_suffix or config.package_name_suffix,
-            dir_or_name_override=output,
+
+def _encrypt_stable(  # pylint: disable=too-many-statements
+    files: List[str],
+    config: Config,
+    sender: str,
+    recipients: List[str],
+    passphrase: Optional[Secret[str]],
+    output: Optional[str],
+    output_suffix: Optional[str],
+    compression_level: int,
+    dtr_id: Optional[int],
+    dry_run: bool,
+    force: bool,
+    purpose: Optional[Purpose],
+    progress: Optional[ProgressInterface],
+) -> Optional[str]:
+    # Retrieve the sender's and recipients' public keys:
+    #  - sender public key: matching private key will be used to encrypt data.
+    #  - recipient public key: needed to encrypt the data.
+    #
+    # The sender/recipient information can be either an email, a keyID or
+    # a full fingerprint.
+    logger.info("Retrieve sender and recipient GnuPG keys")
+    sender_pub_key, *recipients_pub_key = retrieve_refresh_and_validate_keys(
+        key_identifiers=(sender, *recipients),
+        config=config,
+    )
+    # Verify a private key matching the user's public key exists. The key
+    # itself is not needed because it shares the fingerprint with the
+    # public key.
+    search_priv_key(sender_pub_key.fingerprint, config.gpg_store)
+    logger.info(
+        "Sender: %s",
+        f"{sender_pub_key.uids[0]} ({sender_pub_key.fingerprint})",
+    )
+    logger.info(
+        "Recipients: %s",
+        ", ".join(f"{key.uids[0]} ({key.fingerprint})" for key in recipients_pub_key),
+    )
+    # If requested, verify data transfer related information.
+    if config.verify_dtr:
+        logger.info("Verify Data Transfer ID")
+        # Connect to the portal API to retrieve the code (abbreviation)
+        # associated with the DTR ID.
+        project_code = verify_dtr_info_and_get_project_code(
+            dtr_id,
+            purpose,
+            config,
+            sender_pub_key.fingerprint,
+            [k.fingerprint for k in recipients_pub_key],
         )
-        total_input_file_size = get_total_size(files_to_encrypt)
-        check_space(total_input_file_size, os.path.dirname(output_name), force=force)
+        logger.info("DTR ID '%s' is valid for project '%s'", dtr_id, project_code)
+    else:
+        project_code = None
+
+    # The default value for the output name is based on date and time
+    # when the script is being run.
+    # Example output name: "20191011T145012.zip".
+    timestamp = datetime.now().astimezone()
+    output = generate_output_archive_name(
+        prefix=project_code,
+        timestamp=timestamp,
+        suffix=output_suffix or config.package_name_suffix,
+        dir_or_name_override=output,
+    )
 
-        # Create a list of file paths (i.e. the files to package) as they will
-        # appear in the output archive file. For this we start by retrieving
-        # the lowest common directory of all input files/directories.
-        root_dir = os.path.commonpath(
-            [Path(x).absolute().parent.as_posix() for x in files]
+    files_to_encrypt = list(search_files_recursively(files))
+    if not files_to_encrypt:
+        raise UserError(
+            "No input files found. Did you try encrypting an empty directory?"
         )
-        archive_paths = [
-            os.path.join(CONTENT_FOLDER, os.path.relpath(f, start=root_dir))
-            for f in files_to_encrypt
-        ]
-        check_paths_on_posix(archive_paths)
+    check_file_read_permission(files_to_encrypt)
+
+    logger.info("Verify available disk space")
+    total_input_file_size = get_total_size(files_to_encrypt)
+    check_space(total_input_file_size, os.path.dirname(output), force=force)
+
+    # Create a list of file paths (i.e. the files to package) as they will
+    # appear in the output archive file. For this we start by retrieving
+    # the lowest common directory of all input files/directories.
+    root_dir = os.path.commonpath(
+        [Path(x).absolute().parent.as_posix() for x in files_to_encrypt]
+    )
+    archive_paths = [
+        os.path.join(CONTENT_FOLDER, os.path.relpath(f, start=root_dir))
+        for f in files_to_encrypt
+    ]
+    check_paths_on_posix(archive_paths)
 
     if dry_run:
         logger.info("Dry run completed successfully")
         return None
 
     # Verify the user's PGP key passphrase. The passphrase is needed to unlock
     # the private PGP key used to sign the data.
@@ -265,16 +300,16 @@
             progress.update(0.1)
 
     with logger.log_task("Compress and encrypt input data [this can take a while]..."):
         # Encryption is done with the recipient's public key and the optional
         # signing with the user's (i.e sender) private key. The user's private
         # PGP key passphrase is needed to sign the encrypted file.
         encrypted_checksum_buf = io.StringIO()
-        with delete_file_on_error(output_name), ZipFile(
-            output_name, mode="w", compression=ZIP_STORED
+        with delete_file_on_error(output), ZipFile(
+            output, mode="w", compression=ZIP_STORED
         ) as zip_obj:
             with subprogress(progress, step_completion_increase=0.9) as scaled_progress:
                 # Create a tar archive containing all input files
                 archive_content: Tuple[ArchiveFileBase, ...] = (
                     ArchiveInMemoryFile(CHECKSUM_FILE, checksums),
                 ) + tuple(
                     ArchiveFile(a_path, f)
@@ -339,18 +374,93 @@
                 zip_obj.writestr(
                     ZipInfo(name, date_time=datetime.utcnow().timetuple()[:6]),
                     contents,
                 )
 
     logger.info(
         "Completed data encryption: %s [%s]",
-        output_name,
-        get_compression_stats(total_input_file_size, os.path.getsize(output_name)),
+        output,
+        get_compression_stats(total_input_file_size, os.path.getsize(output)),
+    )
+    return output
+
+
+def _encrypt_experimental(
+    files: List[str],
+    config: Config,
+    sender_fingerprint: str,
+    recipients_fingerprints: List[str],
+    passphrase: Optional[Secret[str]],
+    output: Optional[str],
+    output_suffix: Optional[str],
+    dtr_id: Optional[int],
+    dry_run: bool,
+    force: bool,
+    compression_level: Optional[int],
+    purpose: Optional[Purpose],
+    progress: Optional[ProgressInterface],
+) -> Optional[str]:
+    # If requested, verify data transfer related information.
+    if config.verify_dtr:
+        logger.info("Verify Data Transfer ID")
+        # Connect to the portal API to retrieve the code (abbreviation)
+        # associated with the DTR ID.
+        project_code = verify_dtr_info_and_get_project_code(
+            dtr_id,
+            purpose,
+            config,
+            sender_fingerprint,
+            recipients_fingerprints,
+        )
+        logger.info("DTR ID '%s' is valid for project '%s'", dtr_id, project_code)
+    else:
+        project_code = None
+    output = generate_output_archive_name(
+        prefix=project_code,
+        timestamp=None,
+        suffix=output_suffix or config.package_name_suffix,
+        dir_or_name_override=output,
     )
-    return output_name
+
+    store = CertStore()
+    output_path = sett_rs.workflow.encrypt(
+        opts=sett_rs.workflow.EncryptOpts(
+            files=[str(Path(f).absolute()) for f in files],
+            recipients=[
+                get_certificate_from_store(fingerprint, store, CertType.Public)
+                for fingerprint in recipients_fingerprints
+            ],
+            signer=None
+            if dry_run
+            else get_certificate_from_store(sender_fingerprint, store, CertType.Secret),
+            password=passphrase.reveal() if passphrase is not None else None,
+            dry_run=dry_run,
+            force=force,
+            purpose=None if purpose is None else purpose.value,
+            transfer_id=dtr_id,
+            compression_algorithm=sett_rs.workflow.CompressionAlgorithm.Gzip
+            if compression_level is not None and compression_level > 0
+            else sett_rs.workflow.CompressionAlgorithm.Stored,
+            compression_level=compression_level,
+        ),
+        destination=sett_rs.workflow.LocalOpts(output=output),
+        progress=progress.update if progress is not None else None,
+        two_factor_callback=None,
+    )
+    return output_path
+
+
+def get_certificate_from_store(
+    fingerprint: str, store: CertStore, cert_type: CertType
+) -> bytes:
+    """Returns an OpenPGP certificate as bytes based on its fingerprint."""
+    try:
+        return store.export_cert(fingerprint, cert_type)
+    except RuntimeError as e:
+        raise UserError(f"Unable to retrieve certificate '{fingerprint}': {e}") from e
 
 
 T = TypeVar("T")
 
 
 def check_arg_value(
     arg_value: T,
@@ -395,16 +505,16 @@
 
 
 @to_user_error(RuntimeError)
 def verify_dtr_info_and_get_project_code(
     dtr_id: Optional[int],
     purpose: Optional[Purpose],
     config: Config,
-    sender_pub_key: gpg.Key,
-    recipients_pub_key: Iterable[gpg.Key],
+    sender_fingerprint: str,
+    recipients_fingerprint: Iterable[str],
 ) -> str:
     """Determine the "code" (i.e. short name) of a project based on its DTR ID
     (Data Transfer ID) and perform some sanity checks on data associated with
     the transfer by querying the portal API:
      * Verify the data sender's key (sender_pub_key) is authorized.
      * Verify the data recipients' keys (recipients_pub_key) is authorized and
        that the recipient is a DM (data manager) for the project.
@@ -425,16 +535,16 @@
 
     # Query the portal API for the specified DTR ID and return project code.
     # Raises a RuntimeError if the DTR is not-approved or some of the metadata
     # does not match with the project the DTR ID belongs to.
     return config.portal_api.verify_dpkg_metadata(
         metadata=MetaData(
             transfer_id=dtr_id,
-            sender=HexStr1024(sender_pub_key.fingerprint),
-            recipients=[HexStr1024(key.fingerprint) for key in recipients_pub_key],
+            sender=HexStr1024(sender_fingerprint),
+            recipients=[HexStr1024(fp) for fp in recipients_fingerprint],
             checksum=HexStr256("0" * 64),
             purpose=purpose,
         ),
         file_name="missing",
     )
```

### Comparing `sett-4.2.0/sett/workflows/transfer.py` & `sett-4.3.0/sett/workflows/transfer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 import re
 import json
 import time
 from typing import List, Tuple, Dict, Optional, Callable
 
+from sett_rs.cert import CertInfo, CertStore, CertType
+
 from ..core import gpg
 from ..core.crypt import get_recipient_email, retrieve_refresh_and_validate_keys
 from ..core.archive import (
     check_package,
     extract_multiple,
     DATA_FILE_ENCRYPTED,
 )
@@ -54,15 +56,15 @@
     :raises UserError:
     """
 
     with logger.log_task(
         f"Input data verification{' (dry_run)' if dry_run else ''}..."
     ):
         logger.info("Files to transfer: %s", ", ".join(files))
-        files_by_recipient: Dict[Tuple[gpg.Key, ...], List[str]] = {}
+        files_by_recipient: Dict[Tuple[str, ...], List[str]] = {}
 
         # Loop through all files to transfer and verify their content.
         for archive_path in files:
             logger.info("Verifying: %s", archive_path)
 
             # Verify input data package extension and content.
             check_package(archive_path)
@@ -71,19 +73,37 @@
             with extract_multiple(
                 archive_path, (METADATA_FILE, DATA_FILE_ENCRYPTED)
             ) as (
                 metadata_io,
                 encrypted_file,
             ):
                 raw_metadata = json.load(metadata_io)
-                keys = retrieve_refresh_and_validate_keys(
-                    key_identifiers=gpg.extract_key_id(encrypted_file),
-                    config=config,
-                )
-            metadata = load_metadata(raw_metadata)
+                metadata = load_metadata(raw_metadata)
+                if config.experimental:
+                    try:
+                        store = CertStore()
+                        certs = tuple(
+                            CertInfo.from_bytes(store.export_cert(r, CertType.Public))
+                            for r in metadata.recipients
+                        )
+                        files_by_recipient.setdefault(
+                            tuple(get_recipient_email(k) for k in certs), []
+                        ).append(archive_path)
+                    except RuntimeError as e:
+                        raise UserError(
+                            f"Unable to retrieve recipient's certificate: {e}"
+                        ) from e
+                else:
+                    keys = retrieve_refresh_and_validate_keys(
+                        key_identifiers=gpg.extract_key_id(encrypted_file),
+                        config=config,
+                    )
+                    files_by_recipient.setdefault(
+                        tuple(get_recipient_email(k) for k in keys), []
+                    ).append(archive_path)
 
             if config.verify_dtr:
                 if metadata.transfer_id is None:
                     raise UserError(
                         "DTR (Data Transfer Request) ID verification was "
                         "requested but DTR ID is missing in file metadata."
                     )
@@ -107,27 +127,24 @@
 
             if config.verify_package_name:
                 check_archive_name_follows_convention(
                     archive_path=archive_path,
                     project_code=project_code if config.verify_dtr else None,
                     package_name_suffix=pkg_name_suffix,
                 )
-            files_by_recipient.setdefault(keys, []).append(archive_path)
 
     if dry_run:
         logger.info("Dry run completed successfully")
         return
 
     # Transfer files to their destination.
     with logger.log_task("Transferring files..."):
         # For efficiency, files for a same recipient/destination are
         # transferred together.
-        for recipient_keys, r_files in files_by_recipient.items():
-            emails = [get_recipient_email(k) for k in recipient_keys]
-
+        for emails, r_files in files_by_recipient.items():
             for label, value in (
                 # LiquidFiles: email addresses of recipient must be specified.
                 ("recipients", emails),
                 # SFTP: encoding of public SSH key and buffer size must be specified.
                 ("pkey_password_encoding", config.ssh_password_encoding),
                 ("buffer_size", config.sftp_buffer_size),
             ):
```

### Comparing `sett-4.2.0/sett/workflows/upload_keys.py` & `sett-4.3.0/sett/workflows/upload_keys.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from typing import Sequence, Iterable
 
-from gpg_lite.keyserver import VksEmailStatus
+from gpg_lite.keyserver import VksEmailStatus, VksUploadResponse
+from sett_rs.cert import CertInfo, CertStore, CertType
 
 from ..core.crypt import (
-    upload_keys as crypt_upload_keys,
     request_key_verification as crypt_request_key_verification,
     search_pub_key,
+    upload_cert,
+    upload_keys as crypt_upload_keys,
     verify_key_length,
 )
 from ..core.error import UserError
 from ..utils.config import Config
 from ..utils.log import create_logger, log_runtime_info
 
 logger = create_logger(__name__)
@@ -38,38 +40,54 @@
     """Uploads one or more public PGP keys to the keyserver specified in the
     config. Triggers a verification if the status returned by the keyserver is appropriate.
 
     Note that we basically assume that each key contains one single UID (email address).
     """
     if config.keyserver_url is None:
         raise UserError("Keyserver URL is undefined.")
-    keys = frozenset(
-        search_pub_key(k, config.gpg_store, sigs=False) for k in fingerprints
-    )
-    if keys:
-        logger.info("Uploading keys '%s'", ", ".join(k.key_id for k in keys))
-        for key in keys:
+
+    def handle_response(response: VksUploadResponse, email: str, key_id: str) -> None:
+        if email in response.status:
+            if (
+                response.status[email]
+                in (
+                    VksEmailStatus.UNPUBLISHED,
+                    VksEmailStatus.PENDING,
+                )
+                and verify_key
+            ):
+                logger.info("Requesting verification for '%s'", email)
+                crypt_request_key_verification(
+                    response.token, email, config.keyserver_url
+                )
+            if response.status[email] == VksEmailStatus.REVOKED:
+                raise UserError(f"'{key_id}' is revoked and can NOT be used.")
+
+    if config.experimental:
+        for cert_armored in [
+            CertStore().export_cert(f, CertType.Public) for f in fingerprints
+        ]:
+            cert = CertInfo.from_bytes(cert_armored)
+            if not cert.uids or not cert.email:
+                raise UserError(
+                    f"The selected certificate '{cert}' does NOT contain UID or email."
+                )
+            logger.info("Uploading certificate '%s'", cert.key_id)
+            response = upload_cert(
+                cert_armored.decode("utf-8"), keyserver=config.keyserver_url
+            )
+            handle_response(response, cert.email, cert.key_id)
+    else:
+        for key in frozenset(
+            search_pub_key(k, config.gpg_store, sigs=False) for k in fingerprints
+        ):
+            logger.info("Uploading key '%s'", key.key_id)
             if not key.uids or not key.uids[0].email:
                 raise UserError(
                     f"The selected key '{key}' does NOT contain UID or email."
                 )
-            email = key.uids[0].email
             (response,) = crypt_upload_keys(
                 [key.fingerprint],
                 keyserver=config.keyserver_url,
                 gpg_store=config.gpg_store,
             )
-            if email in response.status:
-                if (
-                    response.status[email]
-                    in (
-                        VksEmailStatus.UNPUBLISHED,
-                        VksEmailStatus.PENDING,
-                    )
-                    and verify_key
-                ):
-                    logger.info("Requesting verification for '%s'", email)
-                    crypt_request_key_verification(
-                        response.token, key.uids[0].email, config.keyserver_url
-                    )
-                if response.status[email] == VksEmailStatus.REVOKED:
-                    raise UserError(f"'{key.key_id}' is revoked and can NOT be used.")
+            handle_response(response, key.uids[0].email, key.key_id)
```

### Comparing `sett-4.2.0/sett.egg-info/PKG-INFO` & `sett-4.3.0/sett.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: sett
-Version: 4.2.0
+Version: 4.3.0
 Summary: Secure Encryption and Transfer Tool
 Home-page: https://gitlab.com/biomedit/sett
 Author: Robin Engler, Jarosław Surkont, Gerhard Bräunlich, Kevin Sayers, Christian Ribeaud, François Martin, Simone Guzzi, Swen Vermeul
 Author-email: robin.engler@sib.swiss, jaroslaw.surkont@unibas.ch, gerhard.braeunlich@id.ethz.ch, sayerskt@gmail.com, christian.ribeaud@karakun.com, francois.martin@karakun.com, simone.guzzi@sib.swiss, swen@ethz.ch
 License: GPL3v3
 Project-URL: Documentation, https://sett.rtfd.io/en/stable
 Project-URL: Source, https://gitlab.com/biomedit/sett
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: socks
 Provides-Extra: legacy
 Provides-Extra: benchmark
 Provides-Extra: dev
 License-File: LICENSE
 
-[![pipeline status](https://gitlab.com/biomedit/sett/badges/master/pipeline.svg)](https://gitlab.com/biomedit/sett/-/commits/master)
-[![coverage report](https://gitlab.com/biomedit/sett/badges/master/coverage.svg)](https://gitlab.com/biomedit/sett/-/commits/master)
+[![pipeline status](https://gitlab.com/biomedit/sett/badges/main/pipeline.svg)](https://gitlab.com/biomedit/sett/-/commits/main)
+[![coverage report](https://gitlab.com/biomedit/sett/badges/main/coverage.svg)](https://gitlab.com/biomedit/sett/-/commits/main)
 [![documentation status](https://readthedocs.org/projects/sett/badge/)](https://sett.readthedocs.io/)
 [![license](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![python version](https://img.shields.io/pypi/pyversions/sett.svg?logo=python&logoColor=white)](https://pypi.org/project/sett)
 [![latest version](https://img.shields.io/pypi/v/sett.svg)](https://pypi.org/project/sett)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # SETT - Secure Encryption and Transfer Tool
@@ -43,17 +42,17 @@
 [sett documentation](https://sett.readthedocs.io/en/stable).
 
 For the latest, non-stable, version of the docs, see
 [here](https://sett.readthedocs.io/en/latest).
 
 ### Documentation quick-links
 
-* [Requirements and installation](https://sett.readthedocs.io/en/stable/installation.html).
-* [Quick-start guide](https://sett.readthedocs.io/en/stable/quick_start.html).
-* [Creating and managing GnuPG keys with sett](https://sett.readthedocs.io/en/stable/key_management.html).
-* [Using sett to encrypt, transfer and decrypt data](https://sett.readthedocs.io/en/stable/usage.html)
+- [Requirements and installation](https://sett.readthedocs.io/en/stable/installation.html).
+- [Quick-start guide](https://sett.readthedocs.io/en/stable/quick_start.html).
+- [Creating and managing GnuPG keys with sett](https://sett.readthedocs.io/en/stable/key_management.html).
+- [Using sett to encrypt, transfer and decrypt data](https://sett.readthedocs.io/en/stable/usage.html)
 
 ## Unit tests coverage
 
 Please note that a number of gui-specific files are excluded from the unit
 tests coverage. The detailed list of excluded files can be found in
 [`pyproject.toml`](pyproject.toml), under the `[tool.coverage.run]` section.
```

### Comparing `sett-4.2.0/sett.egg-info/SOURCES.txt` & `sett-4.3.0/sett.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 sett/core/filesystem.py
 sett/core/metadata.py
 sett/core/request.py
 sett/core/secret.py
 sett/core/versioncheck.py
 sett/gui/__init__.py
 sett/gui/__main__.py
+sett/gui/cert_migration_dialog.py
+sett/gui/cert_revocation_dialog.py
 sett/gui/component.py
 sett/gui/decrypt_tab.py
 sett/gui/encrypt_tab.py
 sett/gui/file_selection_widget.py
 sett/gui/key_generation_dialog.py
 sett/gui/keys_download_dialog.py
 sett/gui/keys_tab.py
```

### Comparing `sett-4.2.0/setup.cfg` & `sett-4.3.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Robin Engler, Jarosław Surkont, Gerhard Bräunlich, Kevin Sayers, Christian Ribeaud, François Martin, Simone Guzzi, Swen Vermeul
 author_email = robin.engler@sib.swiss, jaroslaw.surkont@unibas.ch, gerhard.braeunlich@id.ethz.ch, sayerskt@gmail.com, christian.ribeaud@karakun.com, francois.martin@karakun.com, simone.guzzi@sib.swiss, swen@ethz.ch
 url = https://gitlab.com/biomedit/sett
 classifiers = 
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Operating System :: OS Independent
 project_urls = 
@@ -24,21 +23,20 @@
 [options]
 install_requires = 
 	PySide6>=6.4.0, <6.5.0
 	colorama>=0.4.5 ; platform_system=='Windows'
 	gpg-lite>=0.12.3, <0.13.0
 	libbiomedit>=0.6.2, <0.7.0
 	paramiko>=2.12.0
-	sett-rs>=0.2.2, <0.3.0
-	typing_extensions ; python_version<'3.8'
+	sett-rs>=0.4.0, <0.5.0
 	minio>=7.1.12
 	darkdetect>=0.7.1
 packages = find:
 zip_safe = False
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.entry_points]
 console_scripts = 
 	sett = sett.cli:run
 gui_scripts = 
 	sett-gui = sett.gui.__main__:run
```

