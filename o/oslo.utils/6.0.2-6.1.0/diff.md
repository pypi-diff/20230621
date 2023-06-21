# Comparing `tmp/oslo.utils-6.0.2.tar.gz` & `tmp/oslo.utils-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oslo.utils-6.0.2.tar", last modified: Thu Jun  1 15:28:22 2023, max compression
+gzip compressed data, was "oslo.utils-6.1.0.tar", last modified: Thu Nov 17 10:05:08 2022, max compression
```

## Comparing `oslo.utils-6.0.2.tar` & `oslo.utils-6.1.0.tar`

### file list

```diff
@@ -1,159 +1,160 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:28:22.444294 oslo.utils-6.0.2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/.pre-commit-config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7047 2023-06-01 15:28:22.000000 oslo.utils-6.0.2/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26819 2023-06-01 15:28:22.000000 oslo.utils-6.0.2/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2068 2023-06-01 15:28:22.444294 oslo.utils-6.0.2/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      967 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:28:22.424293 oslo.utils-6.0.2/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      378 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:28:22.424293 oslo.utils-6.0.2/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2507 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:28:22.424293 oslo.utils-6.0.2/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      663 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:28:22.424293 oslo.utils-6.0.2/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:28:22.424293 oslo.utils-6.0.2/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/doc/source/reference/dictutils.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/doc/source/reference/encodeutils.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/doc/source/reference/eventletutils.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/doc/source/reference/excutils.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/doc/source/reference/fileutils.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/doc/source/reference/fixture.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/doc/source/reference/importutils.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/doc/source/reference/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/doc/source/reference/netutils.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/doc/source/reference/reflection.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/doc/source/reference/secretutils.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/doc/source/reference/specs_matcher.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/doc/source/reference/strutils.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/doc/source/reference/timeutils.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/doc/source/reference/units.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/doc/source/reference/uuidutils.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/doc/source/reference/versionutils.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:28:22.428293 oslo.utils-6.0.2/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/doc/source/user/history.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2488 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/doc/source/user/timeutils.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/doc/source/user/usage.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:28:22.428293 oslo.utils-6.0.2/oslo.utils.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2068 2023-06-01 15:28:22.000000 oslo.utils-6.0.2/oslo.utils.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4448 2023-06-01 15:28:22.000000 oslo.utils-6.0.2/oslo.utils.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-06-01 15:28:22.000000 oslo.utils-6.0.2/oslo.utils.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-06-01 15:28:22.000000 oslo.utils-6.0.2/oslo.utils.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-06-01 15:28:22.000000 oslo.utils-6.0.2/oslo.utils.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2023-06-01 15:28:22.000000 oslo.utils-6.0.2/oslo.utils.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2023-06-01 15:28:22.000000 oslo.utils-6.0.2/oslo.utils.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:28:22.432294 oslo.utils-6.0.2/oslo_utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/_i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1194 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/dictutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6233 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/encodeutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7090 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/eventletutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14561 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/excutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6098 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/fileutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3420 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/fixture.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8716 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/imageutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3743 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/importutils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:28:22.416292 oslo.utils-6.0.2/oslo_utils/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:28:22.416292 oslo.utils-6.0.2/oslo_utils/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:28:22.432294 oslo.utils-6.0.2/oslo_utils/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2183 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/locale/de/LC_MESSAGES/oslo_utils.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:28:22.416292 oslo.utils-6.0.2/oslo_utils/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:28:22.432294 oslo.utils-6.0.2/oslo_utils/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3025 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/locale/en_GB/LC_MESSAGES/oslo_utils.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:28:22.416292 oslo.utils-6.0.2/oslo_utils/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:28:22.432294 oslo.utils-6.0.2/oslo_utils/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2277 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/locale/fr/LC_MESSAGES/oslo_utils.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16492 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/netutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8707 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/reflection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2198 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/secretutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5979 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/specs_matcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21500 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/strutils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:28:22.436294 oslo.utils-6.0.2/oslo_utils/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      570 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1976 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:28:22.436294 oslo.utils-6.0.2/oslo_utils/tests/fake/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      898 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/tests/fake/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:28:22.436294 oslo.utils-6.0.2/oslo_utils/tests/fake/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/tests/fake/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      929 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/tests/fake/v2/dummpy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1486 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/tests/test_dictutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8513 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/tests/test_eventletutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23309 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/tests/test_excutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10716 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/tests/test_fileutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3645 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/tests/test_fixture.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11728 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/tests/test_imageutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6728 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/tests/test_importutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20171 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/tests/test_netutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10996 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/tests/test_reflection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4447 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/tests/test_secretutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12430 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/tests/test_specs_matcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    42855 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/tests/test_strutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21421 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/tests/test_timeutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2367 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/tests/test_uuidutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3735 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/tests/test_versionutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7016 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/tests/tests_encodeutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15755 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/timeutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1236 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/units.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1572 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/uuidutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2870 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/oslo_utils/versionutils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:28:22.416292 oslo.utils-6.0.2/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:28:22.440294 oslo.utils-6.0.2/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      773 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/notes/add-md5-wrapper-7bf81c2464a7a224.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/notes/add-methods-for-json-yaml-file-check-746dca0a11c2f9c9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/notes/add-reno-350f5f34f794fb5e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/notes/allow-to-convert-ipv4-address-from-text-to-binary-8c46ad2d9989e8c5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/notes/bug-1942682-ea95d54b2587b32f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/notes/bump-up-port-range-f774a16336158339.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/notes/deprecate-fnmatch-057a092d434a0c53.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/notes/drop-imageutils-human-format-support-a89101a36c4dd3cb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/notes/drop-python27-support-f97f680651693b47.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/notes/fix_mask_password_regex-c0661f95a23369a4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/notes/image-utils-handle-scientific-notation-6f65d46e9c8c8f8c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/notes/introduce-keystoneidsentinel-16bf3e7f2ae7e9f3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/notes/mask-dict-passwords-99357ffb7972fb0b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/notes/mask-password-pattern-c8c880098743de3e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/notes/mask-password-patterns-f41524069b8ae488.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/notes/netutils-get_mac_addr_by_ipv6-c3ce6a35a69f7c2b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/notes/remove-fnmatch-f227b54f237a02c2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/notes/remove-timeutils-deprecated-helpers-5de68c21dd281529.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:28:22.444294 oslo.utils-6.0.2/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:28:22.444294 oslo.utils-6.0.2/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:28:22.444294 oslo.utils-6.0.2/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8611 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:28:22.420292 oslo.utils-6.0.2/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:28:22.420292 oslo.utils-6.0.2/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:28:22.444294 oslo.utils-6.0.2/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10185 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      477 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      788 2023-06-01 15:28:22.448295 oslo.utils-6.0.2/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      784 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:28:22.444294 oslo.utils-6.0.2/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1494 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/tools/perf_test_mask_password.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1356 2023-06-01 15:27:51.000000 oslo.utils-6.0.2/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.786223 oslo.utils-6.1.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/.pre-commit-config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7047 2022-11-17 10:05:08.000000 oslo.utils-6.1.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26838 2022-11-17 10:05:08.000000 oslo.utils-6.1.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2068 2022-11-17 10:05:08.786223 oslo.utils-6.1.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      967 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.774222 oslo.utils-6.1.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      378 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.774222 oslo.utils-6.1.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2507 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.774222 oslo.utils-6.1.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      663 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.774222 oslo.utils-6.1.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.774222 oslo.utils-6.1.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/dictutils.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/encodeutils.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/eventletutils.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/excutils.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/fileutils.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/fixture.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/importutils.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/netutils.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/reflection.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/secretutils.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/specs_matcher.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/strutils.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/timeutils.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/units.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/uuidutils.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/reference/versionutils.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.774222 oslo.utils-6.1.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/user/history.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2488 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/user/timeutils.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/doc/source/user/usage.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.778222 oslo.utils-6.1.0/oslo.utils.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2068 2022-11-17 10:05:08.000000 oslo.utils-6.1.0/oslo.utils.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4476 2022-11-17 10:05:08.000000 oslo.utils-6.1.0/oslo.utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-11-17 10:05:08.000000 oslo.utils-6.1.0/oslo.utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-11-17 10:05:08.000000 oslo.utils-6.1.0/oslo.utils.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2022-11-17 10:05:08.000000 oslo.utils-6.1.0/oslo.utils.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2022-11-17 10:05:08.000000 oslo.utils-6.1.0/oslo.utils.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2022-11-17 10:05:08.000000 oslo.utils-6.1.0/oslo.utils.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.778222 oslo.utils-6.1.0/oslo_utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/_i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1194 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/dictutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6233 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/encodeutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7090 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/eventletutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14561 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/excutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6098 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/fileutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3420 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/fixture.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8716 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/imageutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3743 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/importutils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.770222 oslo.utils-6.1.0/oslo_utils/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.770222 oslo.utils-6.1.0/oslo_utils/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.778222 oslo.utils-6.1.0/oslo_utils/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2183 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/locale/de/LC_MESSAGES/oslo_utils.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.770222 oslo.utils-6.1.0/oslo_utils/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.778222 oslo.utils-6.1.0/oslo_utils/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3025 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/locale/en_GB/LC_MESSAGES/oslo_utils.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.770222 oslo.utils-6.1.0/oslo_utils/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.778222 oslo.utils-6.1.0/oslo_utils/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2277 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/locale/fr/LC_MESSAGES/oslo_utils.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16492 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/netutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8707 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/reflection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2198 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/secretutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5979 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/specs_matcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21500 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/strutils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.782222 oslo.utils-6.1.0/oslo_utils/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      570 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1976 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.782222 oslo.utils-6.1.0/oslo_utils/tests/fake/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      898 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/fake/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.782222 oslo.utils-6.1.0/oslo_utils/tests/fake/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/fake/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      929 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/fake/v2/dummpy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1486 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/test_dictutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8513 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/test_eventletutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23309 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/test_excutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10716 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/test_fileutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3645 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/test_fixture.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11728 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/test_imageutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6728 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/test_importutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20171 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/test_netutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10996 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/test_reflection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4447 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/test_secretutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12430 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/test_specs_matcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    42855 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/test_strutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21421 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/test_timeutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2367 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/test_uuidutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3735 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/test_versionutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7016 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/tests/tests_encodeutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15755 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/timeutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1236 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/units.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1572 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/uuidutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2870 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/oslo_utils/versionutils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.770222 oslo.utils-6.1.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.786223 oslo.utils-6.1.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      773 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/add-md5-wrapper-7bf81c2464a7a224.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/add-methods-for-json-yaml-file-check-746dca0a11c2f9c9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/add-reno-350f5f34f794fb5e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/allow-to-convert-ipv4-address-from-text-to-binary-8c46ad2d9989e8c5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/bug-1942682-ea95d54b2587b32f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/bump-up-port-range-f774a16336158339.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/deprecate-fnmatch-057a092d434a0c53.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/drop-imageutils-human-format-support-a89101a36c4dd3cb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/drop-python27-support-f97f680651693b47.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/fix_mask_password_regex-c0661f95a23369a4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/image-utils-handle-scientific-notation-6f65d46e9c8c8f8c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/introduce-keystoneidsentinel-16bf3e7f2ae7e9f3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/mask-dict-passwords-99357ffb7972fb0b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/mask-password-pattern-c8c880098743de3e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/mask-password-patterns-f41524069b8ae488.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/netutils-get_mac_addr_by_ipv6-c3ce6a35a69f7c2b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/remove-fnmatch-f227b54f237a02c2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/notes/remove-timeutils-deprecated-helpers-5de68c21dd281529.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.786223 oslo.utils-6.1.0/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.786223 oslo.utils-6.1.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.786223 oslo.utils-6.1.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8611 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.770222 oslo.utils-6.1.0/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.770222 oslo.utils-6.1.0/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.786223 oslo.utils-6.1.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10181 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      477 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      788 2022-11-17 10:05:08.790223 oslo.utils-6.1.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      784 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-11-17 10:05:08.786223 oslo.utils-6.1.0/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1494 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/tools/perf_test_mask_password.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1362 2022-11-17 10:04:40.000000 oslo.utils-6.1.0/tox.ini
```

### Comparing `oslo.utils-6.0.2/.pre-commit-config.yaml` & `oslo.utils-6.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/AUTHORS` & `oslo.utils-6.1.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/CONTRIBUTING.rst` & `oslo.utils-6.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/ChangeLog` & `oslo.utils-6.1.0/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 CHANGES
 =======
 
-6.0.2
+6.1.0
 -----
 
 * [imageutils] Fix \_\_str\_\_ for QemuImgInfo
-* Update TOX\_CONSTRAINTS\_FILE for stable/zed
-* Update .gitreview for stable/zed
+* Imported Translations from Zanata
+* Add Python3 antelope unit tests
+* Update master for stable/zed
 
 6.0.1
 -----
 
 * Imported Translations from Zanata
 * Imported Translations from Zanata
```

### Comparing `oslo.utils-6.0.2/LICENSE` & `oslo.utils-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/PKG-INFO` & `oslo.utils-6.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: oslo.utils
-Version: 6.0.2
+Version: 6.1.0
 Summary: Oslo Utility library
 Home-page: https://docs.openstack.org/oslo.utils/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `oslo.utils-6.0.2/README.rst` & `oslo.utils-6.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/doc/source/conf.py` & `oslo.utils-6.1.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/doc/source/index.rst` & `oslo.utils-6.1.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/doc/source/user/timeutils.rst` & `oslo.utils-6.1.0/doc/source/user/timeutils.rst`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo.utils.egg-info/PKG-INFO` & `oslo.utils-6.1.0/oslo.utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: oslo.utils
-Version: 6.0.2
+Version: 6.1.0
 Summary: Oslo Utility library
 Home-page: https://docs.openstack.org/oslo.utils/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `oslo.utils-6.0.2/oslo.utils.egg-info/SOURCES.txt` & `oslo.utils-6.1.0/oslo.utils.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -120,11 +120,12 @@
 releasenotes/source/train.rst
 releasenotes/source/unreleased.rst
 releasenotes/source/ussuri.rst
 releasenotes/source/victoria.rst
 releasenotes/source/wallaby.rst
 releasenotes/source/xena.rst
 releasenotes/source/yoga.rst
+releasenotes/source/zed.rst
 releasenotes/source/_static/.placeholder
 releasenotes/source/_templates/.placeholder
 releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
 tools/perf_test_mask_password.py
```

### Comparing `oslo.utils-6.0.2/oslo_utils/_i18n.py` & `oslo.utils-6.1.0/oslo_utils/_i18n.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/dictutils.py` & `oslo.utils-6.1.0/oslo_utils/dictutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/encodeutils.py` & `oslo.utils-6.1.0/oslo_utils/encodeutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/eventletutils.py` & `oslo.utils-6.1.0/oslo_utils/eventletutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/excutils.py` & `oslo.utils-6.1.0/oslo_utils/excutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/fileutils.py` & `oslo.utils-6.1.0/oslo_utils/fileutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/fixture.py` & `oslo.utils-6.1.0/oslo_utils/fixture.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/imageutils.py` & `oslo.utils-6.1.0/oslo_utils/imageutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/importutils.py` & `oslo.utils-6.1.0/oslo_utils/importutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/locale/de/LC_MESSAGES/oslo_utils.po` & `oslo.utils-6.1.0/oslo_utils/locale/de/LC_MESSAGES/oslo_utils.po`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/locale/en_GB/LC_MESSAGES/oslo_utils.po` & `oslo.utils-6.1.0/oslo_utils/locale/en_GB/LC_MESSAGES/oslo_utils.po`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/locale/fr/LC_MESSAGES/oslo_utils.po` & `oslo.utils-6.1.0/oslo_utils/locale/fr/LC_MESSAGES/oslo_utils.po`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/netutils.py` & `oslo.utils-6.1.0/oslo_utils/netutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/reflection.py` & `oslo.utils-6.1.0/oslo_utils/reflection.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/secretutils.py` & `oslo.utils-6.1.0/oslo_utils/secretutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/specs_matcher.py` & `oslo.utils-6.1.0/oslo_utils/specs_matcher.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/strutils.py` & `oslo.utils-6.1.0/oslo_utils/strutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/tests/__init__.py` & `oslo.utils-6.1.0/oslo_utils/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/tests/base.py` & `oslo.utils-6.1.0/oslo_utils/tests/base.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/tests/fake/__init__.py` & `oslo.utils-6.1.0/oslo_utils/tests/fake/__init__.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/tests/fake/v2/dummpy.py` & `oslo.utils-6.1.0/oslo_utils/tests/fake/v2/dummpy.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/tests/test_dictutils.py` & `oslo.utils-6.1.0/oslo_utils/tests/test_dictutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/tests/test_eventletutils.py` & `oslo.utils-6.1.0/oslo_utils/tests/test_eventletutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/tests/test_excutils.py` & `oslo.utils-6.1.0/oslo_utils/tests/test_excutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/tests/test_fileutils.py` & `oslo.utils-6.1.0/oslo_utils/tests/test_fileutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/tests/test_fixture.py` & `oslo.utils-6.1.0/oslo_utils/tests/test_fixture.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/tests/test_imageutils.py` & `oslo.utils-6.1.0/oslo_utils/tests/test_imageutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/tests/test_importutils.py` & `oslo.utils-6.1.0/oslo_utils/tests/test_importutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/tests/test_netutils.py` & `oslo.utils-6.1.0/oslo_utils/tests/test_netutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/tests/test_reflection.py` & `oslo.utils-6.1.0/oslo_utils/tests/test_reflection.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/tests/test_secretutils.py` & `oslo.utils-6.1.0/oslo_utils/tests/test_secretutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/tests/test_specs_matcher.py` & `oslo.utils-6.1.0/oslo_utils/tests/test_specs_matcher.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/tests/test_strutils.py` & `oslo.utils-6.1.0/oslo_utils/tests/test_strutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/tests/test_timeutils.py` & `oslo.utils-6.1.0/oslo_utils/tests/test_timeutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/tests/test_uuidutils.py` & `oslo.utils-6.1.0/oslo_utils/tests/test_uuidutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/tests/test_versionutils.py` & `oslo.utils-6.1.0/oslo_utils/tests/test_versionutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/tests/tests_encodeutils.py` & `oslo.utils-6.1.0/oslo_utils/tests/tests_encodeutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/timeutils.py` & `oslo.utils-6.1.0/oslo_utils/timeutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/units.py` & `oslo.utils-6.1.0/oslo_utils/units.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/uuidutils.py` & `oslo.utils-6.1.0/oslo_utils/uuidutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/oslo_utils/versionutils.py` & `oslo.utils-6.1.0/oslo_utils/versionutils.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/releasenotes/notes/add-md5-wrapper-7bf81c2464a7a224.yaml` & `oslo.utils-6.1.0/releasenotes/notes/add-md5-wrapper-7bf81c2464a7a224.yaml`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/releasenotes/source/conf.py` & `oslo.utils-6.1.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `oslo.utils-6.1.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 # Andi Chandler <andi@gowling.com>, 2018. #zanata
 # Andi Chandler <andi@gowling.com>, 2020. #zanata
 # Andi Chandler <andi@gowling.com>, 2022. #zanata
 msgid ""
 msgstr ""
 "Project-Id-Version: oslo.utils\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-06-21 16:33+0000\n"
+"POT-Creation-Date: 2022-09-09 15:52+0000\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"PO-Revision-Date: 2022-06-26 09:18+0000\n"
+"PO-Revision-Date: 2022-08-14 12:25+0000\n"
 "Last-Translator: Andi Chandler <andi@gowling.com>\n"
 "Language-Team: English (United Kingdom)\n"
 "Language: en_GB\n"
 "X-Generator: Zanata 4.3.3\n"
 "Plural-Forms: nplurals=2; plural=(n != 1)\n"
 
 msgid "3.13.0"
@@ -103,16 +103,16 @@
 
 msgid "4.8.2"
 msgstr "4.8.2"
 
 msgid "4.9.1"
 msgstr "4.9.1"
 
-msgid "5.0.0-4"
-msgstr "5.0.0-4"
+msgid "6.0.0"
+msgstr "6.0.0"
 
 msgid ""
 "A wrapper for hashlib.md5() has been added to allow OpenStack to run on "
 "systems where FIPS is enabled.  Under FIPS, md5 is disabled and calls to "
 "hashlib.md5() will fail.  In most cases in OpenStack, though, md5 is not "
 "used within a security context."
 msgstr ""
```

### Comparing `oslo.utils-6.0.2/setup.cfg` & `oslo.utils-6.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/setup.py` & `oslo.utils-6.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/test-requirements.txt` & `oslo.utils-6.1.0/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/tools/perf_test_mask_password.py` & `oslo.utils-6.1.0/tools/perf_test_mask_password.py`

 * *Files identical despite different names*

### Comparing `oslo.utils-6.0.2/tox.ini` & `oslo.utils-6.1.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 minversion = 3.18.0
 envlist = py3,pep8
 ignore_basepython_conflict = true
 
 [testenv]
 basepython = python3
 deps =
-  -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/zed}
+  -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
   -r{toxinidir}/test-requirements.txt
   -r{toxinidir}/requirements.txt
 commands = stestr run --slowest {posargs}
 
 [testenv:pep8]
 commands =
   pre-commit run -a
@@ -19,15 +19,15 @@
 
 [testenv:venv]
 commands = {posargs}
 
 [testenv:docs]
 allowlist_externals = rm
 deps =
-  -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/zed}
+  -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
   -r{toxinidir}/doc/requirements.txt
 commands =
   rm -fr doc/build
   sphinx-build -W --keep-going -b html doc/source doc/build/html
 
 [testenv:cover]
 commands = python setup.py test --coverage --coverage-package-name=oslo_utils --testr-args='{posargs}'
```

