# Comparing `tmp/reuse-1.1.2.tar.gz` & `tmp/reuse-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reuse-1.1.2.tar", max compression
+gzip compressed data, was "reuse-2.0.0.tar", max compression
```

## Comparing `reuse-1.1.2.tar` & `reuse-2.0.0.tar`

### file list

```diff
@@ -1,86 +1,89 @@
--rw-r--r--   0        0        0     1040 2022-11-23 09:51:25.298341 reuse-1.1.2/.reuse/dep5
--rw-r--r--   0        0        0     1776 2023-02-08 21:45:38.862290 reuse-1.1.2/AUTHORS.rst
--rw-r--r--   0        0        0    26429 2023-02-09 16:58:17.731010 reuse-1.1.2/CHANGELOG.md
-drwxr-xr-x   0        0        0        0 2023-02-09 16:31:00.947458 reuse-1.1.2/LICENSES/
--rw-r--r--   0        0        0    11358 2022-01-22 22:24:28.393509 reuse-1.1.2/LICENSES/Apache-2.0.txt
--rw-r--r--   0        0        0    20131 2022-01-22 22:24:28.394509 reuse-1.1.2/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0        0        0     7048 2022-01-22 22:24:28.394509 reuse-1.1.2/LICENSES/CC0-1.0.txt
--rw-r--r--   0        0        0    35149 2022-01-22 22:24:28.394509 reuse-1.1.2/LICENSES/GPL-3.0-or-later.txt
--rw-r--r--   0        0        0    10102 2023-02-09 16:58:17.781010 reuse-1.1.2/README.md
--rw-r--r--   0        0        0     3049 2023-02-09 16:54:28.824053 reuse-1.1.2/_build.py
--rw-r--r--   0        0        0      712 2023-02-08 21:45:38.863290 reuse-1.1.2/docs/Makefile
--rw-r--r--   0        0        0        0 2022-01-22 22:24:28.395509 reuse-1.1.2/docs/_static/.gitkeep
--rw-r--r--   0        0        0      164 2022-01-22 22:24:28.395509 reuse-1.1.2/docs/authors.rst
--rw-r--r--   0        0        0     6266 2023-02-09 16:58:17.781010 reuse-1.1.2/docs/conf.py
--rw-r--r--   0        0        0      617 2023-02-09 16:54:22.960081 reuse-1.1.2/docs/index.rst
--rw-r--r--   0        0        0     5776 2023-02-08 21:45:38.863290 reuse-1.1.2/docs/scripts.rst
--rw-r--r--   0        0        0    12291 2023-02-09 16:54:22.960081 reuse-1.1.2/docs/usage.rst
--rw-r--r--   0        0        0      192 2022-01-22 22:24:28.396509 reuse-1.1.2/docs/usage.rst.license
--rw-r--r--   0        0        0      331 2022-01-22 22:24:28.396509 reuse-1.1.2/po/POTFILES.in
--rw-r--r--   0        0        0    28233 2022-01-22 22:24:28.396509 reuse-1.1.2/po/de.po
--rw-r--r--   0        0        0    31745 2022-01-22 22:24:28.397509 reuse-1.1.2/po/eo.po
--rw-r--r--   0        0        0    33286 2022-01-22 22:29:39.513915 reuse-1.1.2/po/es.po
--rw-r--r--   0        0        0    24847 2022-01-22 22:24:28.397509 reuse-1.1.2/po/fr.po
--rw-r--r--   0        0        0    27946 2022-01-22 22:24:28.398509 reuse-1.1.2/po/gl.po
--rw-r--r--   0        0        0    28116 2022-01-22 22:24:28.398509 reuse-1.1.2/po/it.po
--rw-r--r--   0        0        0    32609 2022-01-22 22:24:28.398509 reuse-1.1.2/po/nl.po
--rw-r--r--   0        0        0    28271 2022-01-22 22:24:28.399509 reuse-1.1.2/po/pt.po
--rw-r--r--   0        0        0    27508 2022-01-22 22:24:28.399509 reuse-1.1.2/po/tr.po
--rw-r--r--   0        0        0     2261 2023-02-09 16:58:17.781010 reuse-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     2467 2023-02-09 16:58:17.781010 reuse-1.1.2/src/reuse/__init__.py
--rw-r--r--   0        0        0      254 2022-10-06 20:16:20.552069 reuse-1.1.2/src/reuse/__main__.py
--rw-r--r--   0        0        0    23030 2023-02-09 16:54:22.961081 reuse-1.1.2/src/reuse/_comment.py
--rw-r--r--   0        0        0     1256 2022-01-22 22:24:28.400509 reuse-1.1.2/src/reuse/_format.py
--rw-r--r--   0        0        0     2040 2022-04-28 21:34:46.325501 reuse-1.1.2/src/reuse/_licenses.py
--rw-r--r--   0        0        0     9191 2023-02-08 21:45:38.864290 reuse-1.1.2/src/reuse/_main.py
--rw-r--r--   0        0        0    16868 2023-02-09 16:54:22.961081 reuse-1.1.2/src/reuse/_util.py
--rw-r--r--   0        0        0     5034 2023-02-08 21:45:38.864290 reuse-1.1.2/src/reuse/download.py
--rw-r--r--   0        0        0    24624 2023-02-09 16:54:22.961081 reuse-1.1.2/src/reuse/header.py
--rw-r--r--   0        0        0     4015 2023-02-08 21:45:38.865290 reuse-1.1.2/src/reuse/init.py
--rw-r--r--   0        0        0    10077 2022-04-28 21:34:46.327501 reuse-1.1.2/src/reuse/lint.py
--rw-r--r--   0        0        0    19083 2023-02-09 17:03:06.763009 reuse-1.1.2/src/reuse/locale/de/LC_MESSAGES/reuse.mo
--rw-r--r--   0        0        0    18051 2023-02-09 17:03:06.764009 reuse-1.1.2/src/reuse/locale/eo/LC_MESSAGES/reuse.mo
--rw-r--r--   0        0        0    18394 2023-02-09 17:03:06.766009 reuse-1.1.2/src/reuse/locale/es/LC_MESSAGES/reuse.mo
--rw-r--r--   0        0        0    19367 2023-02-09 17:03:06.764009 reuse-1.1.2/src/reuse/locale/fr/LC_MESSAGES/reuse.mo
--rw-r--r--   0        0        0    18816 2023-02-09 17:03:06.764009 reuse-1.1.2/src/reuse/locale/gl/LC_MESSAGES/reuse.mo
--rw-r--r--   0        0        0    19029 2023-02-09 17:03:06.765009 reuse-1.1.2/src/reuse/locale/it/LC_MESSAGES/reuse.mo
--rw-r--r--   0        0        0    18702 2023-02-09 17:03:06.765009 reuse-1.1.2/src/reuse/locale/nl/LC_MESSAGES/reuse.mo
--rw-r--r--   0        0        0    19155 2023-02-09 17:03:06.765009 reuse-1.1.2/src/reuse/locale/pt/LC_MESSAGES/reuse.mo
--rw-r--r--   0        0        0    18447 2023-02-09 17:03:06.765009 reuse-1.1.2/src/reuse/locale/tr/LC_MESSAGES/reuse.mo
--rw-r--r--   0        0        0    12135 2022-10-06 20:16:20.553069 reuse-1.1.2/src/reuse/project.py
--rw-r--r--   0        0        0    13902 2022-04-28 21:34:46.329501 reuse-1.1.2/src/reuse/report.py
--rw-r--r--   0        0        0    17950 2023-02-08 21:45:38.865290 reuse-1.1.2/src/reuse/resources/exceptions.json
--rw-r--r--   0        0        0      100 2022-01-22 22:24:28.402509 reuse-1.1.2/src/reuse/resources/exceptions.json.license
--rw-r--r--   0        0        0   223999 2023-02-08 21:45:38.865290 reuse-1.1.2/src/reuse/resources/licenses.json
--rw-r--r--   0        0        0      100 2022-01-22 22:24:28.404509 reuse-1.1.2/src/reuse/resources/licenses.json.license
--rw-r--r--   0        0        0     1589 2022-10-06 20:16:20.554069 reuse-1.1.2/src/reuse/spdx.py
--rw-r--r--   0        0        0      926 2022-04-28 21:34:46.329501 reuse-1.1.2/src/reuse/supported_licenses.py
--rw-r--r--   0        0        0      175 2022-01-23 10:56:25.986207 reuse-1.1.2/src/reuse/templates/default_template.jinja2
--rw-r--r--   0        0        0      119 2022-01-22 22:24:28.404509 reuse-1.1.2/src/reuse/templates/default_template.jinja2.license
--rw-r--r--   0        0        0     6626 2022-01-22 22:24:28.404509 reuse-1.1.2/src/reuse/vcs.py
--rw-r--r--   0        0        0    10078 2023-02-09 16:54:22.961081 reuse-1.1.2/tests/conftest.py
--rw-r--r--   0        0        0      215 2022-01-29 14:32:52.242396 reuse-1.1.2/tests/resources/fake_repository/.reuse/dep5
--rw-r--r--   0        0        0       14 2022-01-22 22:24:28.405509 reuse-1.1.2/tests/resources/fake_repository/LICENSES/Autoconf-exception-3.0.txt
--rw-r--r--   0        0        0       13 2022-01-22 22:24:28.405509 reuse-1.1.2/tests/resources/fake_repository/LICENSES/CC0-1.0.txt
--rw-r--r--   0        0        0       13 2022-01-22 22:24:28.405509 reuse-1.1.2/tests/resources/fake_repository/LICENSES/GPL-3.0-or-later.txt
--rw-r--r--   0        0        0        0 2022-01-22 22:24:28.405509 reuse-1.1.2/tests/resources/fake_repository/LICENSES/LicenseRef-custom.txt
--rw-r--r--   0        0        0       14 2022-01-22 22:24:28.405509 reuse-1.1.2/tests/resources/fake_repository/doc/index.rst
--rw-r--r--   0        0        0       58 2022-03-27 09:48:13.872508 reuse-1.1.2/tests/resources/fake_repository/src/custom.py
--rw-r--r--   0        0        0       58 2022-03-27 09:48:13.872508 reuse-1.1.2/tests/resources/fake_repository/src/exception.py
--rw-r--r--   0        0        0      156 2022-01-29 14:32:52.242396 reuse-1.1.2/tests/resources/fake_repository/src/source_code.c
--rw-r--r--   0        0        0      111 2022-10-06 20:16:20.555069 reuse-1.1.2/tests/resources/fake_repository/src/source_code.html
--rw-r--r--   0        0        0      109 2022-10-06 20:16:20.555069 reuse-1.1.2/tests/resources/fake_repository/src/source_code.jinja2
--rw-r--r--   0        0        0      166 2022-01-29 14:32:52.242396 reuse-1.1.2/tests/resources/fake_repository/src/source_code.py
--rw-r--r--   0        0        0     5450 2022-01-22 22:24:28.406509 reuse-1.1.2/tests/resources/fsfe.png
--rw-r--r--   0        0        0    14499 2023-02-09 16:54:22.961081 reuse-1.1.2/tests/test_comment.py
--rw-r--r--   0        0        0     3201 2023-02-08 21:45:38.866290 reuse-1.1.2/tests/test_download.py
--rw-r--r--   0        0        0    10651 2023-02-09 16:54:22.961081 reuse-1.1.2/tests/test_header.py
--rw-r--r--   0        0        0     4827 2022-10-06 20:16:20.555069 reuse-1.1.2/tests/test_lint.py
--rw-r--r--   0        0        0    11623 2023-02-08 21:45:38.866290 reuse-1.1.2/tests/test_main.py
--rw-r--r--   0        0        0    32292 2023-02-09 16:54:22.961081 reuse-1.1.2/tests/test_main_annotate.py
--rw-r--r--   0        0        0     3712 2023-02-08 21:45:38.866290 reuse-1.1.2/tests/test_main_annotate_merge.py
--rw-r--r--   0        0        0    13250 2022-10-06 20:16:20.557069 reuse-1.1.2/tests/test_project.py
--rw-r--r--   0        0        0     9436 2022-10-06 20:16:20.557069 reuse-1.1.2/tests/test_report.py
--rw-r--r--   0        0        0    19494 2023-02-08 21:45:38.866290 reuse-1.1.2/tests/test_util.py
--rw-r--r--   0        0        0      900 2022-04-28 21:34:46.334501 reuse-1.1.2/tests/test_vcs.py
--rw-r--r--   0        0        0    11305 2023-02-09 17:11:40.950566 reuse-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1154 2023-06-21 09:24:49.565014 reuse-2.0.0/.reuse/dep5
+-rw-r--r--   0        0        0     1814 2023-06-21 09:24:49.565014 reuse-2.0.0/AUTHORS.rst
+-rw-r--r--   0        0        0    29293 2023-06-21 11:00:49.131810 reuse-2.0.0/CHANGELOG.md
+drwxr-xr-x   0        0        0        0 2023-06-21 09:24:49.569014 reuse-2.0.0/LICENSES/
+-rw-r--r--   0        0        0    11358 2023-06-21 09:24:49.569014 reuse-2.0.0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0        0        0    20131 2023-06-21 09:24:49.569014 reuse-2.0.0/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0        0        0     7048 2023-06-21 09:24:49.569014 reuse-2.0.0/LICENSES/CC0-1.0.txt
+-rw-r--r--   0        0        0    35149 2023-06-21 09:24:49.569014 reuse-2.0.0/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0        0        0     9941 2023-06-21 10:51:41.407169 reuse-2.0.0/README.md
+-rw-r--r--   0        0        0     2173 2023-06-21 09:24:49.569014 reuse-2.0.0/_build.py
+-rw-r--r--   0        0        0      712 2023-06-21 09:24:49.569014 reuse-2.0.0/docs/Makefile
+-rw-r--r--   0        0        0        0 2023-06-21 09:24:49.569014 reuse-2.0.0/docs/_static/.gitkeep
+-rw-r--r--   0        0        0      164 2023-06-21 09:24:49.569014 reuse-2.0.0/docs/authors.rst
+-rw-r--r--   0        0        0     5955 2023-06-21 10:51:41.407169 reuse-2.0.0/docs/conf.py
+-rw-r--r--   0        0        0      643 2023-06-21 09:24:49.569014 reuse-2.0.0/docs/index.rst
+-rw-r--r--   0        0        0     4232 2023-06-21 09:24:49.569014 reuse-2.0.0/docs/requirements.txt
+-rw-r--r--   0        0        0      124 2023-06-21 09:24:49.569014 reuse-2.0.0/docs/requirements.txt.license
+-rw-r--r--   0        0        0     5608 2023-06-21 09:24:49.569014 reuse-2.0.0/docs/reuse-r-only.svg
+-rw-r--r--   0        0        0      105 2023-06-21 09:24:49.569014 reuse-2.0.0/docs/reuse-r-only.svg.license
+-rw-r--r--   0        0        0     5776 2023-06-21 09:24:49.569014 reuse-2.0.0/docs/scripts.rst
+-rw-r--r--   0        0        0    12618 2023-06-21 09:24:49.569014 reuse-2.0.0/docs/usage.rst
+-rw-r--r--   0        0        0      192 2023-06-21 09:24:49.569014 reuse-2.0.0/docs/usage.rst.license
+-rw-r--r--   0        0        0      331 2023-06-21 09:24:49.569014 reuse-2.0.0/po/POTFILES.in
+-rw-r--r--   0        0        0    29042 2023-06-21 10:46:01.722193 reuse-2.0.0/po/cs.po
+-rw-r--r--   0        0        0    28286 2023-06-21 10:46:01.722193 reuse-2.0.0/po/de.po
+-rw-r--r--   0        0        0    31871 2023-06-21 10:46:01.722193 reuse-2.0.0/po/eo.po
+-rw-r--r--   0        0        0    33269 2023-06-21 10:46:01.722193 reuse-2.0.0/po/es.po
+-rw-r--r--   0        0        0    24933 2023-06-21 10:46:01.722193 reuse-2.0.0/po/fr.po
+-rw-r--r--   0        0        0    27746 2023-06-21 10:46:01.722193 reuse-2.0.0/po/gl.po
+-rw-r--r--   0        0        0    28199 2023-06-21 10:46:01.722193 reuse-2.0.0/po/it.po
+-rw-r--r--   0        0        0    32658 2023-06-21 10:46:01.722193 reuse-2.0.0/po/nl.po
+-rw-r--r--   0        0        0    28325 2023-06-21 10:46:01.722193 reuse-2.0.0/po/pt.po
+-rw-r--r--   0        0        0    20298 2023-06-21 09:24:49.569014 reuse-2.0.0/po/reuse.pot
+-rw-r--r--   0        0        0      108 2023-06-21 09:24:49.569014 reuse-2.0.0/po/reuse.pot.license
+-rw-r--r--   0        0        0    27570 2023-06-21 10:46:01.722193 reuse-2.0.0/po/tr.po
+-rw-r--r--   0        0        0    42021 2023-06-21 10:46:01.726193 reuse-2.0.0/po/uk.po
+-rw-r--r--   0        0        0     3086 2023-06-21 10:51:41.407169 reuse-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5708 2023-06-21 10:51:41.407169 reuse-2.0.0/src/reuse/__init__.py
+-rw-r--r--   0        0        0      254 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/__main__.py
+-rw-r--r--   0        0        0     1358 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/_format.py
+-rw-r--r--   0        0        0     2161 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/_licenses.py
+-rw-r--r--   0        0        0     9668 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/_main.py
+-rw-r--r--   0        0        0    18609 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/_util.py
+-rw-r--r--   0        0        0    24169 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/comment.py
+-rw-r--r--   0        0        0     5272 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/download.py
+-rw-r--r--   0        0        0    25834 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/header.py
+-rw-r--r--   0        0        0     4156 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/init.py
+-rw-r--r--   0        0        0     8425 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/lint.py
+-rw-r--r--   0        0        0    14788 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/project.py
+-rw-r--r--   0        0        0      122 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/py.typed
+-rw-r--r--   0        0        0    18953 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/report.py
+-rw-r--r--   0        0        0    23174 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/resources/exceptions.json
+-rw-r--r--   0        0        0      100 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/resources/exceptions.json.license
+-rw-r--r--   0        0        0   251607 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/resources/licenses.json
+-rw-r--r--   0        0        0      100 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/resources/licenses.json.license
+-rw-r--r--   0        0        0     3132 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/spdx.py
+-rw-r--r--   0        0        0     1040 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/supported_licenses.py
+-rw-r--r--   0        0        0      281 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/templates/default_template.jinja2
+-rw-r--r--   0        0        0      119 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/templates/default_template.jinja2.license
+-rw-r--r--   0        0        0     6784 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/vcs.py
+-rw-r--r--   0        0        0    11145 2023-06-21 09:24:49.569014 reuse-2.0.0/tests/conftest.py
+-rw-r--r--   0        0        0      215 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/resources/fake_repository/.reuse/dep5
+-rw-r--r--   0        0        0       14 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/resources/fake_repository/LICENSES/Apache-2.0.txt
+-rw-r--r--   0        0        0       14 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/resources/fake_repository/LICENSES/Autoconf-exception-3.0.txt
+-rw-r--r--   0        0        0       13 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/resources/fake_repository/LICENSES/CC0-1.0.txt
+-rw-r--r--   0        0        0       13 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/resources/fake_repository/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0        0        0        0 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/resources/fake_repository/LICENSES/LicenseRef-custom.txt
+-rw-r--r--   0        0        0       14 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/resources/fake_repository/doc/index.rst
+-rw-r--r--   0        0        0       58 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/resources/fake_repository/src/custom.py
+-rw-r--r--   0        0        0       58 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/resources/fake_repository/src/exception.py
+-rw-r--r--   0        0        0       59 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/resources/fake_repository/src/multiple_licenses.rs
+-rw-r--r--   0        0        0      156 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/resources/fake_repository/src/source_code.c
+-rw-r--r--   0        0        0      111 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/resources/fake_repository/src/source_code.html
+-rw-r--r--   0        0        0      109 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/resources/fake_repository/src/source_code.jinja2
+-rw-r--r--   0        0        0      166 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/resources/fake_repository/src/source_code.py
+-rw-r--r--   0        0        0     5450 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/resources/fsfe.png
+-rw-r--r--   0        0        0    14497 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/test_comment.py
+-rw-r--r--   0        0        0     2480 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/test_core.py
+-rw-r--r--   0        0        0     3201 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/test_download.py
+-rw-r--r--   0        0        0    10656 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/test_header.py
+-rw-r--r--   0        0        0     7156 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/test_lint.py
+-rw-r--r--   0        0        0    14494 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/test_main.py
+-rw-r--r--   0        0        0    34232 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/test_main_annotate.py
+-rw-r--r--   0        0        0     3712 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/test_main_annotate_merge.py
+-rw-r--r--   0        0        0    13333 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/test_project.py
+-rw-r--r--   0        0        0    13056 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/test_report.py
+-rw-r--r--   0        0        0    20096 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/test_util.py
+-rw-r--r--   0        0        0      900 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/test_vcs.py
+-rw-r--r--   0        0        0    11431 1970-01-01 00:00:00.000000 reuse-2.0.0/PKG-INFO
```

### Comparing `reuse-1.1.2/.reuse/dep5` & `reuse-2.0.0/.reuse/dep5`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 Copyright: 2017 Free Software Foundation Europe e.V. <https://fsfe.org>
 License: CC-BY-SA-4.0
 
 Files: docs/modules.rst
 Copyright: 2017 Free Software Foundation Europe e.V. <https://fsfe.org>
 License: CC-BY-SA-4.0
 
+Files: po/*.po
+Copyright: 2023 Free Software Foundation Europe e.V. <https://fsfe.org>
+License: GPL-3.0-or-later
+
 Files: tests/resources/*
 Copyright: 2017 Free Software Foundation Europe e.V. <https://fsfe.org>
 License: GPL-3.0-or-later
 
 Files: src/reuse.egg-info/*
 Copyright: 2017 Free Software Foundation Europe e.V. <https://fsfe.org>
 License: GPL-3.0-or-later
```

### Comparing `reuse-1.1.2/AUTHORS.rst` & `reuse-2.0.0/AUTHORS.rst`

 * *Files 10% similar despite different names*

```diff
@@ -56,14 +56,16 @@
 
 - Yaman Qalieh
 
 - Pietro Albini <pietro.albini@ferrous-systems.com>
 
 - Stefan Hynek <stefan.hynek@uni-goettingen.de>
 
+- roberto-red <roberto@redradix.com>
+
 Translators
 -----------
 
 - Dutch:
 
   + André Ockers <ao@fsfe.org>
```

### Comparing `reuse-1.1.2/CHANGELOG.md` & `reuse-2.0.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 <!--
 SPDX-FileCopyrightText: 2017 Free Software Foundation Europe e.V. <https://fsfe.org>
 SPDX-FileCopyrightText: © 2020 Liferay, Inc. <https://liferay.com>
+SPDX-FileCopyrightText: 2023 DB Systel GmbH
 
 SPDX-License-Identifier: CC-BY-SA-4.0
 -->
 
 # Change log
 
 This change log follows the [Keep a Changelog](http://keepachangelog.com/) spec.
@@ -13,15 +14,17 @@
 - `Added` for new features.
 - `Changed` for changes in existing functionality.
 - `Deprecated` for soon-to-be removed features.
 - `Removed` for now removed features.
 - `Fixed` for any bug fixes.
 - `Security` in case of vulnerabilities.
 
-The versions follow [semantic versioning](https://semver.org).
+The versions follow [semantic versioning](https://semver.org) for the `reuse`
+CLI command and its behaviour. There are no guarantees of stability for the
+`reuse` Python library.
 
 <!--
 ## Unreleased - YYYY-MM-DD
 
 ### Added
 
 ### Changed
@@ -31,14 +34,83 @@
 ### Removed
 
 ### Fixed
 
 ### Security
 -->
 
+## 2.0.0 - 2023-06-21
+
+### Added
+
+- Detect SPDX snippet tags in files. (#699)
+- More file types are recognised:
+  - Fennel (`.fnl`) (#638)
+  - CommonJS (`.cjs`) (#632)
+  - Qt .pro (`.pro`) (#632)
+  - Qt .pri (`.pri`) (#755)
+  - Qt .qrc (`.qrc`) (#755)
+  - Qt .qss(`.qss`) (#755)
+  - Qt .ui (`.ui`) (#755)
+  - Textile (`.textile`) (#712)
+  - Visual Studio Code workspace (`.code-workspace`) (#747)
+  - Application Resource Bundle (`.arb`) (#749)
+  - Svelte components (`.svelte`)
+  - AES encrypted files (`.aes`) (#758)
+  - Jakarte Server Page (`.jsp`) (#757)
+- More files are recognised:
+  - Clang format (`.clang-format`) (#632)
+  - Browserslist config (`.browserslist`)
+  - Prettier config (`.prettierrc`) and ignored files (`.prettierignore`)
+  - Flutter pubspec.lock (`pubspec.lock`) (#751)
+  - Flutter .metadata (`.metadata`) (#751)
+  - Terraform (`.tf`, `tfvars`) and HCL (`.hcl`). (#756)
+- Added loglevel argument to pytest and skip one test if loglevel is too high
+  (#645).
+- `--add-license-concluded`, `--creator-person`, and `--creator-organization`
+  added to `reuse spdx`. (#623)
+- Additional license metadata for the Python package has been added. The actual
+  SPDX license expression remains the same:
+  `Apache-2.0 AND CC0-1.0 AND CC-BY-SA-4.0 AND GPL-3.0-or-later`. (#733)
+- Added `--contributor` option to `annotate`. (#669)
+- Added `--json` flag to `lint` command (#654).
+- `reuse.ReuseInfo` now has `copy` and `union` methods. (#759)
+- Added Ukrainian and Czech translations (#767)
+
+### Changed
+
+- Bumped SPDX license list to v3.20. (#692)
+- `reuse.SpdxInfo` was renamed to `reuse.ReuseInfo`. It is now a (frozen)
+  dataclass instead of a namedtuple. This is only relevant if you're using reuse
+  as a library in Python. (#669)
+- Sphinx documentation: Switched from RTD theme to Furo. (#673, #716)
+- Removed dependency on setuptools' `pkg_resources` to determine the installed
+  version of reuse. (#724)
+- Bumped SPDX license list to v3.21. (#763)
+- Bumped REUSE Spec version to 3.1. (#768)
+- Introduce an order of precedence. The copyright and licensing information from
+  different sources (e.g. `.license` or `.reuse/dep5` file) is no longer merged.
+  (#654)
+
+### Removed
+
+- Python 3.6 and 3.7 support has been dropped. (#673, #759)
+- Removed runtime and build time dependency on `setuptools`. (#724)
+
+### Fixed
+
+- Fixed automatic generation of Sphinx documentation via readthedocs.io by
+  adding a `.readthedocs.yaml` configuration file (#648)
+- Fixed a compatibility issue where reuse could not be installed (built) if
+  gettext is not installed. (#691)
+- Translations are available in Docker images. (#701)
+- Marked the `/data` directory in Docker containers as safe in Git, preventing
+  errors related to linting Git repositories. (#720)
+- Repaired error when using Galician translations. (#719)
+
 ## 1.1.2 - 2023-02-09
 
 ### Fixed
 
 - Note to maintainers: It is now possible/easier to use the `build` module to
   build this module. Previously, there was a namespace conflict. (#640)
 
@@ -51,29 +123,23 @@
 - Include documentation directory in sdist. (#657)
 
 ## 1.1.0 - 2022-12-01
 
 ### Added
 
 - Added support for Python 3.11. (#603)
-
 - More file types are recognised:
-
   - Kotlin script (`.kts`)
   - Android Interface Definition Language (`.aidl`)
   - Certificate files (`.pem`)
-
 - Added comment styles:
-
   - Apache Velocity Template (Extensions: `.vm`, `.vtl`) (#554)
   - XQuery comment style (Extensions: `.xq(l|m|y|uery|)`) (#610)
-
 - Some special endings are always stripped from copyright and licensing
   statements (#602):
-
   - `">` (and variations such as `'>`, `" >`, and `"/>`)
   - `] ::`
 
 ### Changed
 
 - Removed `setup.py` and replaced it with a Poetry configuration. Maintainers
   beware. (#600)
@@ -129,58 +195,42 @@
 @ventosus.
 
 ### Added
 
 - Extend [tool documentation](https://reuse.readthedocs.io) with scripts to help
   using this tool and automating some steps that are not built into the tool
   itself. (#500)
-
 - Recommendations for installation/run methods: package managers and pipx (#457)
-
 - Docker images for AArch64 (#478)
-
 - Added the ability to ignore parts of a file when running `reuse lint`. Simply
   add `REUSE-IgnoreStart` and `REUSE-IgnoreEnd` as comments and all lines
   between the two will be ignored by the next run of `reuse lint`. (#463)
-
 - [Meson subprojects](https://mesonbuild.com/Subprojects.html) are now ignored
   by default. (#496)
-
 - More file types are recognised:
-
   - sbt build files (`.sbt`)
   - Vimscript files (`.vim`)
-
 - Added `--skip-existing` flag to `addheader` in order to skip files that
   already contain SPDX information. This may be useful for only adding SPDX
   information to newly created files. (#480)
-
 - Added `--recursive` flag to `addheader`. (#469)
-
 - Preserve shebang for more script files:
-
   - V-Lang (#432)
-
 - Ignore all SPDX files with their typical formats and extensions. (#494)
-
 - Add support for merging copyright lines based on copyright statement,
   transforming multiple lines with a single year into a single line with a
   range. (#328)
 
 ### Changed
 
 - Use `setuptools` instead of the deprecated `distutils` which will be removed
   with Python 3.12. (#451)
-
 - `addheader --explicit-license` renamed to `--force-dot-license`. (#476)
-
 - Dockerfiles for reuse-tool are now in a separate subdirectory `docker`. (#499)
-
 - Updated SPDX license list to 3.17. (#513)
-
 - The copyright detection mechanism now silently accepts the following strings:
   `Copyright(c)` and `Copyright(C)`. (#440)
 
 ### Deprecated
 
 - Deprecated `--explicit-license` in favour of `--force-dot-license`.
   `--explicit-license` will remain useable (although undocumented) for the
@@ -193,20 +243,17 @@
 
 ### Fixed
 
 - Better support for unary "+" operator in license identifiers. For example, if
   `Apache-1.0+` appears as a declared license, it should not be identified as
   missing, bad, or unused if `LICENSES/Apache-1.0.txt` exists. It is, however,
   identified separately as a used license. (#123)
-
 - When `addheader` creates a `.license` file, that file now has a newline at the
   end. (#477)
-
 - Cleaned up internal string manipulation. (#477)
-
 - JSX (`.jxs` and `.tsx`) actually uses C comment syntax as JSX blocks never
   stand at the beginning of the file where the licensing info needs to go.
   (#406)
 
 ## 0.14.0 - 2021-12-27
 
 Happy holidays! This is mainly a maintenance release fixing some subcommands and
@@ -214,24 +261,19 @@
 the `supported-licenses` subcommand and the `--quiet` flag for linting as well
 as better suggestions for license identifiers. Thanks to everyone who
 contributed!
 
 ### Added
 
 - `supported-licenses` command that lists all licenses supported by REUSE (#401)
-
 - `--quiet` switch to the `lint` command (#402)
-
 - Better suggestions for faulty SPDX license identifiers in `download` and
   `init` (#416)
-
 - Python 3.10 support declared
-
 - More file types are recognised:
-
   - Apache FreeMarker Template Language (`.ftl`)
   - AsciiDoc (`.adoc`, `.asc`, `.asciidoc`)
   - Bibliography (`.csl`)
   - C++ (`.cc` and `.hh`)
   - GraphQL (`.graphql`)
   - Handlebars (`.hbs`)
   - Markdown-linter config (`.mdlrc`)
@@ -242,17 +284,15 @@
   - Portable document format (`.pdf`)
   - Protobuf files (`.proto`)
   - Soy templates (`.soy`)
   - SuperCollider (`.sc`, `.scsyndef`)
   - Turtle/RDF (`.ttl`)
   - V-Lang (`.v`, `.vsh`)
   - Vue.js (`.vue`)
-
 - More file names are recognised:
-
   - Doxygen (`Doxyfile`)
   - ESLint (`.eslintignore` and `.eslintrc`)
   - Meson options file (`meson_options.txt`)
   - NPM ignore (`.npmignore`)
   - Podman container files (`Containerfile`)
   - SuperCollider (`archive.sctxar`)
   - Yarn package manager (`.yarn.lock` and `.yarnrc`)
@@ -260,84 +300,67 @@
 ### Changed
 
 - Updated SPDX license list to 3.15
 
 ### Fixed
 
 - Fix Extensible Stylesheet Language (`.xsl`) to use HTML comment syntax
-
 - Allow creating .license file for write-protected files (#347) (#418)
-
 - Do not break XML files special first line (#378)
-
 - Make `download` subcommand work correctly outside of project root and with
   `--root` (#430)
 
 ## 0.13.0 - 2021-06-11
 
 ### Added
 
 - `addheader` recognises file types that specifically require .license files
   instead of headers using `UncommentableCommentStyle`. (#189)
-
 - `.hgtags` is ignored. (#227)
-
 - `spdx-symbol` added to possible copyright styles. (#350)
-
 - `addheader` ignores case when matching file extensions and names. (#359)
-
 - Provide `latest-debian` as Docker Hub tag, created by `Dockerfile-debian`.
   (#321)
-
 - More file types are recognised:
-
   - Javascript modules (`.mjs`)
   - Jupyter Notebook (`.ipynb`)
   - Scalable Vector Graphics (`.svg`)
   - JSON (`.json`)
   - Comma-separated values (`.csv`)
   - Racket (`.rkt`)
   - Org-mode (`.org`)
   - LaTeX package files (`.sty`)
   - devicetree (`.dts`, `.dtsi`)
   - Bitbake (.bb, .bbappend, .bbclass)
   - XML schemas (`.xsd`)
   - OpenSCAD (`.scad`)
-
 - More file names are recognised:
   - Bash configuration (`.bashrc`)
   - Coverage.py (`.coveragerc`)
   - Jenkins (`Jenkinsfile`)
   - SonarScanner (`sonar-project.properties`)
   - Gradle (`gradle-wrapper.properties`, `gradlew`)
 
 ### Changed
 
 - Bump `alpine` Docker base image to 3.13. (#369)
 
 ### Fixed
 
 - Fixed a regression where unused licenses were not at all detected. (#285)
-
 - Declared dependency on `python-debian != 0.1.39` on Windows. This version does
   not import on Windows. (#310)
-
 - `MANIFEST.in` is now recognised instead of the incorrect `Manifest.in` by
   `addheader`. (#306)
-
 - `addheader` now checks whether a file is both readable and writeable instead
   of only writeable. (#241)
-
 - `addheader` now preserves line endings. (#308)
-
 - `download` does no longer fail when both `--output` and `--all` are used.
   (#326)
-
 - Catch erroneous SPDX expressions. (#331)
-
 - Updated SPDX license list to 3.13.
 
 ## 0.12.1 - 2020-12-17
 
 ### Fixed
 
 - Bumped versions of requirements. (#288)
@@ -351,35 +374,30 @@
 Piuola, Wolfgang Traylor, Paul Spooren, Robert Cohn, ethulhu, pukkamustard, and
 Diego Elio Pettenò.
 
 ### Added
 
 - Separate Docker image with additional executables installed
   (`fsfe/reuse:latest-extra`) (#238)
-
 - Allow different styles of copyright lines: SPDX (default), String, String (C),
   String ©, and © (#248)
-
 - Convenience function to update resources (SPDX license list and exceptions)
   (#268)
-
 - More file types are recognised:
-
   - ClojureScript (`.cljc`, `.cljs`)
   - Fortran (`.F`, `.F90`, `.f90`, `.f95`, `.f03`, `.f`, `.for`)
   - Makefile (`.mk`)
   - PlantUML (`.iuml`, `.plantuml`, `.pu`, `.puml`)
   - R (`.R`, `.Renviron`, `.Rprofile`)
   - ReStructured Text (`.rst`)
   - RMarkdown (`.Rmd`)
   - Scheme (`.scm`)
   - TypeScript (`.ts`)
   - TypeScript JSX (`.tsx`)
   - Windows Batch (`.bat`)
-
 - More file names are recognised:
   - .dockerignore
   - Gemfile
   - go.mod
   - meson.build
   - Rakefile
 
@@ -405,22 +423,20 @@
 - Added `--skip-unrecognised` flag to `addheader` in order to skip files with
   unrecognised comment styles instead of aborting without processing any file.
 
 ### Changed
 
 - Always write the output files encoded in UTF-8, explicitly. This is already
   the default on most Unix systems, but it was not on Windows.
-
 - All symlinks and 0-sized files in projects are now ignored.
 
 ### Fixed
 
 - The licenses CAL-1.0 and CAL-1.0-Combined-Work-Exception contain an SPDX tag
   within themselves. Files that are named after these licenses are now ignored.
-
 - Fixed a bug where `addheader` wouldn't properly apply the template on
   `.license` files if the `.license` file was non-empty, but did not contain
   valid SPDX tags.
 
 ## 0.10.1 - 2020-05-14
 
 ### Fixed
@@ -428,200 +444,161 @@
 - Updated license list to 3.8-106-g4cfec76.
 
 ## 0.10.0 - 2020-04-24
 
 ### Added
 
 - Add support for autoconf comment style (listed as m4).
-
 - More file types are recognised:
-
   - Cython (`.pyx`, `.pxd`)
   - Sass and SCSS (`.sass`, `.scss`)
   - XSL (`.xsl`)
   - Mailmap (`.mailmap`)
-
 - Added `--single-line` and `--multi-line` flags to `addheader`. These flags
   force a certain comment style.
 
 ### Changed
 
 - The Docker image has an entrypoint now. In effect, this means running:
-
-  `docker run -v $(pwd):/data fsfe/reuse lint`
-
-  instead of
-
+  `docker run -v $(pwd):/data fsfe/reuse lint` instead of
   `docker run -v $(pwd):/data fsfe/reuse reuse lint`.
 
 ## 0.9.0 - 2020-04-21
 
 ### Added
 
 - Added support for Mercurial 4.3+.
-
 - A pre-commit hook has been added.
-
 - When an incorrect SPDX identifier is forwarded to `download` or `init`, the
   tool now suggests what you might have meant.
 
 ### Changed
 
 - Under the hood, a lot of code that has to do with Git and Mercurial was moved
   into its own module.
-
 - The Docker image has been changed such that it now automagically runs
   `reuse lint` on the `/data` directory unless something else is specified by
   the user.
 
 ### Fixed
 
 - Fixed a bug with `addheader --explicit-license` that would result in
   `file.license.license` if `file.license` already existed.
-
 - Fixed a Windows-only bug to do with calling subprocesses.
-
 - Fixed a rare bug that would trigger when a directory is both ignored and
   contains a `.git` file.
 
 ## 0.8.1 - 2020-02-22
 
 ### Added
 
 - Support Jinja (Jinja2) comment style.
-
 - Support all multi-line comment endings when parsing for SPDX information.
 
 ### Fixed
 
 - Improvements to German translation by Thomas Doczkal.
-
 - No longer remove newlines at the end of files when using `addheader`.
-
 - There can now be a tab as whitespace after `SPDX-License-Identifier` and
   `SPDX-FileCopyrightText`.
 
 ## 0.8.0 - 2020-01-20
 
 ### Added
 
 - Implemented `--root` argument to specify the root of the project without
   heuristics.
-
 - The linter will complain about licenses without file extensions.
-
 - Deprecated licenses are now recognised. `lint` will complain about deprecated
   licenses.
-
 - ProjectReport generation (`lint`, `spdx`) now uses Python multiprocessing,
   more commonly called multi-threading outside of Python. This has a significant
   speedup of approximately 300% in testing. Because of overhead, performance
   increase is not exactly linear.
-
 - For setups where multiprocessing is unsupported or unwanted,
   `--no-multiprocessing` is added as flag.
-
 - `addheader` now recognises many more extensions. Too many to list here.
-
 - `addheader` now also recognises full filenames such as `Makefile` and
   `.gitignore`.
-
 - Added BibTex comment style.
-
 - Updated translations:
-
   - Dutch (André Ockers, Carmen Bianca Bakker)
   - French (OliBug, Vincent Lequertier)
   - Galician (pd)
   - German (Max Mehl)
   - Esperanto (Carmen Bianca Bakker)
   - Portuguese (José Vieira)
   - Spanish (Roberto Bauglir)
   - Turkish (T. E. Kalayci)
 
 ### Changed
 
 - The linter output has been very slightly re-ordered to be more internally
   consistent.
-
 - `reuse --version` now prints a version with a Git hash on development
   versions. Towards that end, the tool now depends on `setuptools-scm` during
   setup. It is not a runtime dependency.
 
 ### Removed
 
 - `lint` no longer accepts path arguments. Where previously one could do
   `reuse lint SUBDIRECTORY`, this is no longer possible. When linting, you must
   always lint the entire project. To change the project's root, use `--root`.
-
 - `FileReportInfo` has been removed. `FileReport` is used instead.
 
 ### Fixed
 
 - A license that does not have a file extension, but whose full name is a valid
   SPDX License Identifier, is now correctly identified as such. The linter will
   complain about them, however.
-
 - If the linter detects a license as being a bad license, that license can now
   also be detected as being missing.
-
 - Performance of `project.all_files()` has been improved by quite a lot.
-
 - Files with CRLF line endings are now better supported.
 
 ## 0.7.0 - 2019-11-28
 
 ### Changed
 
 - The program's package name on PyPI has been changed from `fsfe-reuse` to
   `reuse`. `fsfe-reuse==1.0.0` has been created as an alias that depends on
   `reuse`. `fsfe-reuse` will not receive any more updates, but will still host
   the old versions.
-
 - For users of `fsfe-reuse`, this means:
-
   - If you depend on `fsfe-reuse` or `fsfe-reuse>=0.X.Y` in your
     requirements.txt, you will get the latest version of `reuse` when you
     install `fsfe-reuse`. You may like to change the name to `reuse` explicitly,
     but this is not strictly necessary.
-
   - If you depend on `fsfe-reuse==0.X.Y`, then you will keep getting that
     version. When you bump the version you depend on, you will need to change
     the name to `reuse`.
-
   - If you depend on `fsfe-reuse>=0.X.Y<1.0.0`, then 0.6.0 will be the latest
     version you receive. In order to get a later version, you will need to
     change the name to `reuse`.
 
 ## 0.6.0 - 2019-11-19
 
 ### Added
 
 - `--include-submodules` is added to also include submodules when linting et
   cetera.
-
 - `addheader` now also recognises the following extensions:
-
   - .kt
   - .xml
   - .yaml
   - .yml
 
 ### Changed
 
 - Made the workaround for `MachineReadableFormatError` introduced in 0.5.2 more
   generic.
-
 - Improved shebang detection in `addheader`.
-
 - For `addheader`, the SPDX comment block now need not be the first thing in the
   file. It will find the SPDX comment block and deal with it in-place.
-
 - Git submodules are now ignored by default.
-
 - `addheader --explicit-license` now no longer breaks on unsupported filetypes.
 
 ## 0.5.2 - 2019-10-27
 
 ### Added
 
 - `python3 -m reuse` now works.
@@ -630,120 +607,97 @@
 
 - Updated license list to 3.6-2-g2a14810.
 
 ### Fixed
 
 - Performance of `reuse lint` improved by at least a factor of 2. It no longer
   does any checksums on files behind the scenes.
-
 - Also handle `MachineReadableFormatError` when parsing DEP5 files. Tries to
   import that error. If the import is unsuccessful, it is handled.
 
 ## 0.5.1 - 2019-10-24 [YANKED]
 
 This release was replaced by 0.5.2 due to importing
 `MachineReadableFormatError`, which is not a backwards-compatible change.
 
 ## 0.5.0 - 2019-08-29
 
 ### Added
 
 - TeX and ML comment styles added.
-
 - Added `--year` and `--exclude-year` to `reuse addheader`.
-
 - Added `--template` to `reuse addheader`.
-
 - Added `--explicit-license` to `reuse addheader`.
-
 - `binaryornot` added as new dependency.
-
 - Greatly improved the usage documentation.
 
 ### Changed
 
 - `reuse addheader` now automatically adds the current year to the copyright
   notice.
-
 - `reuse addheader` preserves the original header below the new header if it did
   not contain any SPDX information.
-
 - `reuse addheader` now correctly handles `.license` files.
-
 - Bad licenses are no longer resolved to LicenseRef-Unknown<n>. They are instead
   resolved to the stem of the path. This reduces the magic in the code base.
-
 - `.gitkeep` files are now ignored by the tool.
-
 - Changed Lisp's comment character from ';;' to ';'.
 
 ## 0.4.1 - 2019-08-07
 
 ### Added
 
 - `--all` argument help to `reuse download`, which downloads all detected
   missing licenses.
 
 ### Fixed
 
 - When using `reuse addheader` on a file that contains a shebang, the shebang is
   preserved.
-
 - Copyright lines in `reuse spdx` are now sorted.
-
 - Some publicly visible TODOs were patched away.
 
 ## 0.4.0 - 2019-08-07
 
 This release is a major overhaul and refactoring of the tool. Its primary focus
 is improved usability and speed, as well as adhering to version 3.0 of the REUSE
 Specification.
 
 ### Added
 
 - `reuse addheader` has been added as a way to automatically add copyright
   statements and license identifiers to the headers of files. It is currently
   not complete.
-
 - `reuse init` has been added as a way to initialise a REUSE project. Its
   functionality is currently scarce, but should improve in the future.
 
 ### Changed
 
 - `reuse lint` now provides a helpful summary instead of merely spitting out
   non-compliant files.
-
 - `reuse compile` is now `reuse spdx`.
-
 - In addition to `Copyright` and `©`, copyright lines can be marked with the tag
   `SPDX-FileCopyrightText:`. This is the new recommended default.
-
 - Project no longer depends on pygit2.
-
 - The list of SPDX licenses has been updated.
-
 - `Valid-License-Identifier` is no longer used, and licenses and exceptions can
   now only live inside of the LICENSES/ directory.
 
 ### Removed
 
 - Removed `--ignore-debian`.
-
 - Removed `--spdx-mandatory`, `--copyright-mandatory`, `--ignore-missing`
   arguments from `reuse lint`.
-
 - Remove `reuse license`.
-
 - GPL-3.0 and GPL-3.0+ (and all other similar GPL licenses) are no longer
   detected as SPDX identifiers. Use GPL-3.0-only and GPL-3.0-or-later instead.
 
 ### Fixed
 
 - Scanning a Git directory is a lot faster now.
-
 - Scanning binary files is a lot faster now.
 
 ## 0.3.4 - 2019-04-15
 
 This release should be a short-lived one. A new (slightly
 backwards-incompatible) version is in the works.
```

### Comparing `reuse-1.1.2/LICENSES/Apache-2.0.txt` & `reuse-2.0.0/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `reuse-1.1.2/LICENSES/CC-BY-SA-4.0.txt` & `reuse-2.0.0/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `reuse-1.1.2/LICENSES/CC0-1.0.txt` & `reuse-2.0.0/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `reuse-1.1.2/LICENSES/GPL-3.0-or-later.txt` & `reuse-2.0.0/LICENSES/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `reuse-1.1.2/README.md` & `reuse-2.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -5,37 +5,51 @@
 -->
 
 # reuse
 
 [![The latest version of reuse can be found on PyPI.](https://img.shields.io/pypi/v/reuse.svg)](https://pypi.python.org/pypi/reuse)
 [![Information on what versions of Python reuse supports can be found on PyPI.](https://img.shields.io/pypi/pyversions/reuse.svg)](https://pypi.python.org/pypi/reuse)
 [![REUSE status](https://api.reuse.software/badge/github.com/fsfe/reuse-tool)](https://api.reuse.software/info/github.com/fsfe/reuse-tool)
-[![readme style standard](https://img.shields.io/badge/readme_style-standard-brightgreen.svg)](https://github.com/RichardLitt/standard-readme)
+[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg)](https://github.com/RichardLitt/standard-readme)
 [![Packaging status](https://repology.org/badge/tiny-repos/reuse.svg?header=in%20distro%20repos)](https://repology.org/project/reuse/versions)
+[![Translation status](https://hosted.weblate.org/widgets/fsfe/-/reuse-tool/svg-badge.svg)](https://hosted.weblate.org/projects/fsfe/reuse-tool/)
 
-> reuse is a tool for compliance with the [REUSE](https://reuse.software/)
-> recommendations.
+reuse is a tool for compliance with the [REUSE](https://reuse.software/)
+recommendations.
 
 - Documentation: <https://reuse.readthedocs.io> and <https://reuse.software>
 - Source code: <https://github.com/fsfe/reuse-tool>
 - PyPI: <https://pypi.python.org/pypi/reuse>
 - REUSE: 3.0
-- Python: 3.6+
+- Python: 3.8+
+
+## Table of contents
+
+- [Background](#background)
+- [Install](#install)
+- [Usage](#usage)
+- [Maintainers](#maintainers)
+- [Contributing](#contributing)
+- [License](#license)
 
 ## Background
 
+<!-- REUSE-IgnoreStart -->
+
 Copyright and licensing is difficult, especially when reusing software from
 different projects that are released under various different licenses.
 [REUSE](https://reuse.software) was started by the
 [Free Software Foundation Europe](https://fsfe.org) (FSFE) to provide a set of
 recommendations to make licensing your Free Software projects easier. Not only
 do these recommendations make it easier for you to declare the licenses under
 which your works are released, but they also make it easier for a computer to
 understand how your project is licensed.
 
+<!-- REUSE-IgnoreEnd -->
+
 As a short summary, the recommendations are threefold:
 
 1. Choose and provide licenses
 2. Add copyright and licensing information to each file
 3. Confirm REUSE compliance
 
 You are recommended to read [our tutorial](https://reuse.software/tutorial) for
@@ -49,39 +63,21 @@
 
 There are [other tools](https://reuse.software/comparison) that have a lot more
 features and functionality surrounding the analysis and inspection of copyright
 and licenses in software projects. The REUSE helper tool, on the other hand, is
 solely designed to be a simple tool to assist in compliance with the REUSE
 recommendations.
 
-## Example demo
-
-In this screencast, we are going to follow the
-[tutorial](https://reuse.software/tutorial), making the
-[REUSE example repository](https://github.com/fsfe/reuse-example/) compliant.
-
-![Demo of some basic REUSE tool commands](https://download.fsfe.org/videos/reuse/screencasts/reuse-tool.gif)
-
 ## Install
 
-### Installation via package managers (Recommended)
+### Installation via package manager (Recommended)
 
-There are packages available for easy install on some operating systems. You are
+There are packages available for easy install on many operating systems. You are
 welcome to help us package this tool for more distributions!
 
-- Alpine Linux: [reuse](https://pkgs.alpinelinux.org/packages?name=reuse)
-- Arch Linux: [reuse](https://archlinux.org/packages/community/any/reuse/)
-- Debian: [reuse](https://packages.debian.org/search?keywords=reuse&exact=1)
-- GNU Guix: [reuse](https://guix.gnu.org/en/packages/reuse-1.0.0/)
-- Fedora: [reuse](https://packages.fedoraproject.org/pkgs/reuse/reuse/)
-- MacPorts: [reuse](https://ports.macports.org/port/reuse/)
-- NixOS: [reuse](https://search.nixos.org/packages?show=reuse)
-- openSUSE: [reuse](https://software.opensuse.org/package/reuse)
-- VoidLinux: [reuse](https://voidlinux.org/packages/?arch=x86_64&q=reuse)
-
 An automatically generated list can be found at
 [repology.org](https://repology.org/project/reuse/versions), without any
 guarantee for completeness.
 
 ### Install and run via pipx (Recommended)
 
 The following one-liner both installs and runs this tool from
@@ -102,44 +98,47 @@
 ```bash
 pipx install reuse
 ```
 
 reuse will then be available in `~/.local/bin`, which must be added to your
 `$PATH`.
 
-### Installation via pip
-
-To install reuse, you need to have the following pieces of software on your
-computer:
-
-- Python 3.6+
-- pip
-
-You then only need to run the following command:
-
-```bash
-pip3 install --user reuse
-```
-
 After this, make sure that `~/.local/bin` is in your `$PATH`. On Windows, the
 required path for your environment may look like
 `%USERPROFILE%\AppData\Roaming\Python\Python39\Scripts`, depending on the Python
 version you have installed.
 
-To update reuse, run this command:
+To upgrade reuse, run this command:
 
 ```bash
-pip3 install --user --upgrade reuse
+pipx upgrade reuse
 ```
 
 For full functionality, the following pieces of software are recommended:
 
 - Git
 - Mercurial 4.3+
 
+### Installation via pip
+
+To install reuse into `~/.local/bin`, run:
+
+```bash
+pip3 install --user reuse
+```
+
+Subsequently, make sure that `~/.local/bin` is in your `$PATH` like described in
+the previous section.
+
+To upgrade reuse, run this command:
+
+```bash
+pip3 install --user --upgrade reuse
+```
+
 ### Installation from source
 
 You can also install this tool from the source code, but we recommend the
 methods above for easier and more stable updates. Please make sure the
 requirements for the installation via pip are present on your machine.
 
 ```bash
@@ -147,14 +146,16 @@
 ```
 
 ## Usage
 
 First, read the [REUSE tutorial](https://reuse.software/tutorial/). In a
 nutshell:
 
+<!-- REUSE-IgnoreStart -->
+
 1. Put your licenses in the `LICENSES/` directory.
 2. Add a comment header to each file that says
    `SPDX-License-Identifier: GPL-3.0-or-later`, and
    `SPDX-FileCopyrightText: $YEAR $NAME`. You can be flexible with the format,
    just make sure that the line starts with `SPDX-FileCopyrightText:`.
 3. Verify your work using this tool.
 
@@ -162,39 +163,46 @@
 
 ```
 # SPDX-FileCopyrightText: 2017 Free Software Foundation Europe e.V. <https://fsfe.org>
 #
 # SPDX-License-Identifier: CC-BY-SA-4.0
 ```
 
+<!-- REUSE-IgnoreEnd -->
+
+### CLI
+
 To check against the recommendations, use `reuse lint`:
 
 ```
 ~/Projects/reuse-tool $ reuse lint
 [...]
 
 Congratulations! Your project is compliant with version 3.0 of the REUSE Specification :-)
 ```
 
 This tool can do various more things, detailed in the documentation. Here a
 short summary:
 
 - `annotate` --- Add copyright and/or licensing information to the header of a
   file.
-
 - `download` --- Download the specified license into the `LICENSES/` directory.
-
 - `init` --- Set up the project for REUSE compliance.
-
 - `lint` --- Verify the project for REUSE compliance.
-
 - `spdx` --- Generate an SPDX Document of all files in the project.
-
 - `supported-licenses` --- Prints all licenses supported by REUSE.
 
+### Example demo
+
+In this screencast, we are going to follow the
+[tutorial](https://reuse.software/tutorial), making the
+[REUSE example repository](https://github.com/fsfe/reuse-example/) compliant.
+
+![Demo of some basic REUSE tool commands](https://download.fsfe.org/videos/reuse/screencasts/reuse-tool.gif)
+
 ### Run in Docker
 
 The `fsfe/reuse` Docker image is available on
 [Docker Hub](https://hub.docker.com/r/fsfe/reuse). With it, you can easily
 include REUSE in CI/CD processes. This way, you can check for REUSE compliance
 for each build. In our [resources for developers](https://reuse.software/dev/)
 you can learn how to integrate the REUSE tool in Drone, Travis, GitHub, or
@@ -231,59 +239,50 @@
 Git. This uses [pre-commit](https://pre-commit.com/). Once you
 [have it installed](https://pre-commit.com/#install), add this to the
 `.pre-commit-config.yaml` in your repository:
 
 ```yaml
 repos:
   - repo: https://github.com/fsfe/reuse-tool
-    rev: v1.1.2
+    rev: v2.0.0
     hooks:
       - id: reuse
 ```
 
 Then run `pre-commit install`. Now, every time you commit, `reuse lint` is run
 in the background, and will prevent your commit from going through if there was
 an error.
 
 ## Maintainers
 
-- Carmen Bianca Bakker - <carmenbianca@fsfe.org>
-- Max Mehl - <max.mehl@fsfe.org>
-
-## Contribute
-
-Any pull requests or suggestions are welcome at
-<https://github.com/fsfe/reuse-tool> or via e-mail to one of the maintainers.
-General inquiries can be sent to <reuse@lists.fsfe.org>.
-
-Interaction within this project is covered by the
-[FSFE's Code of Conduct](https://fsfe.org/about/codeofconduct).
+- Carmen Bianca Bakker <carmenbianca@fsfe.org>
+- Max Mehl <max.mehl@fsfe.org>
+- Linus Sehn <linus@fsfe.org>
+
+## Contributing
+
+If you're interested in contributing to the reuse project, there are several
+ways to get involved. Development of the project takes place on GitHub at
+<https://github.com/fsfe/reuse-tool>. There, you can submit bug reports, feature
+requests, and pull requests. Even and especially when in doubt, feel free to
+open an issue with a question. Contributions of all types are welcome, and the
+development team is happy to provide guidance and support for new contributors.
 
-Starting local development is very simple, just execute the following commands:
-
-```bash
-git clone git@github.com:fsfe/reuse-tool.git
-cd reuse-tool/
-poetry install  # You may need to install poetry using your package manager.
-poetry run pre-commit install  # Using poetry is optional here if you already have pre-commit.
-```
+Additionally, the <reuse@lists.fsfe.org> mailing list is available for
+discussion and support related to the project.
 
-Next, you'll find the following commands handy:
-
-- `poetry run reuse`
-- `poetry run pytest`
-- `poetry run pylint src`
-- `make docs`
+You can find the full contribution guidelines at
+<https://reuse.readthedocs.io/en/latest/contributing.html>.
 
 ## License
 
 This work is licensed under multiple licences. Because keeping this section
-up-to-date is challenging, here is a brief summary as of April 2020:
+up-to-date is challenging, here is a brief summary as of February 2023:
 
 - All original source code is licensed under GPL-3.0-or-later.
 - All documentation is licensed under CC-BY-SA-4.0.
 - Some configuration and data files are licensed under CC0-1.0.
 - Some code borrowed from
-  [spdx/tool-python](https://github.com/spdx/tools-python) is licensed under
+  [spdx/tools-python](https://github.com/spdx/tools-python) is licensed under
   Apache-2.0.
 
 For more accurate information, check the individual files.
```

### Comparing `reuse-1.1.2/docs/Makefile` & `reuse-2.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reuse-1.1.2/docs/conf.py` & `reuse-2.0.0/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,17 @@
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import sys
+from importlib.metadata import PackageNotFoundError, version
 from shutil import copyfile
 
-from pkg_resources import DistributionNotFound, get_distribution
-
 sys.path.insert(0, os.path.abspath("../src/"))
 
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
@@ -61,35 +60,36 @@
 source_suffix = [".rst", ".txt", ".md"]
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "reuse"
-copyright = "2017-2019, Free Software Foundation Europe. CC-BY-SA-4.0"
+copyright = "2017-2023, Free Software Foundation Europe. CC-BY-SA-4.0"
 author = "Free Software Foundation Europe"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 
 try:
     # The full version, including alpha/beta/rc tags.
-    release = get_distribution("reuse").version
-except DistributionNotFound:
-    release = "1.1.2"
+    release = version("reuse")
+except PackageNotFoundError:
+    release = "2.0.0"
+
 # The short X.Y.Z version.
 version = ".".join(release.split(".")[:3])
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The name of the Pygments (syntax highlighting) style to use.
@@ -100,40 +100,28 @@
 
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = "sphinx_rtd_theme"
+html_theme = "furo"
+html_logo = "reuse-r-only.svg"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 
-# Custom sidebar templates, must be a dictionary that maps document names
-# to template names.
-#
-# This is required for the alabaster theme
-# refs: http://alabaster.readthedocs.io/en/latest/installation.html#sidebars
-html_sidebars = {
-    "**": [
-        "relations.html",  # needs 'show_related': True theme option to display
-        "searchbox.html",
-    ]
-}
-
-
 # -- Options for HTMLHelp output ------------------------------------------
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = "reusedoc"
 
 
 # -- Options for LaTeX output ---------------------------------------------
@@ -198,11 +186,12 @@
 
 def copy_markdown(_):
     """Copy the markdown files from the root of the project into the docs/
     directory.
     """
     copyfile("../README.md", "readme.md")
     copyfile("../CHANGELOG.md", "history.md")
+    copyfile("../CONTRIBUTING.md", "contributing.md")
 
 
 def setup(app):
     app.connect("builder-inited", copy_markdown)
```

### Comparing `reuse-1.1.2/docs/index.rst` & `reuse-2.0.0/docs/index.rst`

 * *Files 26% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 
 Welcome to reuse's documentation!
 =================================
 
 .. toctree::
    :maxdepth: 2
 
-   readme
+   Overview<readme>
    usage
    scripts
+   contributing
    authors
    history
    API<api/modules>
 
 
 
 Indices and tables
```

### Comparing `reuse-1.1.2/docs/scripts.rst` & `reuse-2.0.0/docs/scripts.rst`

 * *Files identical despite different names*

### Comparing `reuse-1.1.2/docs/usage.rst` & `reuse-2.0.0/docs/usage.rst`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,18 @@
 working directory is inside a VCS repository. Otherwise, it treats the working
 directory as the root of the project. You can override the root of the project
 with the ``--root`` optional argument.
 
 Git submodules are automatically ignored unless ``--include-submodules`` is
 passed as optional argument.
 
-Symbolically links and files that are zero-sized are automatically ignored.
+Meson subprojects are automatically ignored if ``meson.build`` exists in the
+project root. ``--include-meson-subprojects`` overrides this behaviour.
+
+Symbolic links and files that are zero-sized are automatically ignored.
 
 annotate
 ========
 
 ``annotate`` makes it possible to semi-automatically add copyright and
 licensing information into the header of a file. This is useful especially in
 scenarios where you want to add a copyright holder or license to a lot of files
@@ -71,14 +74,15 @@
 
 With the argument ``--copyright-style`` it is possible to change the default
 ``SPDX-FileCopyrightText`` to one of the following style:
 
 .. code-block::
 
   spdx:           SPDX-FileCopyrightText: <year> <statement>
+  spdx-c:         SPDX-FileCopyrightText: (C) <year> <statement>
   spdx-symbol:    SPDX-FileCopyrightText: © <year> <statement>
   string:         Copyright <year> <statement>
   string-c:       Copyright (C) <year> <statement>
   string-symbol:  Copyright © <year> <statement>
   symbol:         © <year> <statement>
 
 Shebangs are always preserved at the top of the file. If you also want to
@@ -127,28 +131,15 @@
 
 Comment styles
 --------------
 
 The tool normally tries to auto-detect the comment style to use from the file
 extension of a file, and use that comment style. If the tool is unable to detect
 the comment style, or if it detects the wrong style, you can override the style
-using ``--style``. The supported styles are:
-
-- AppleScript
-- ASPX
-- BibTex
-- C
-- CSS
-- Haskell
-- HTML
-- Jinja
-- JSX
-- ML
-- Python
-- TeX
+using ``--style``. The list of styles can be found in :doc:`api/reuse.comment`.
 
 If your comment style is not supported or a file extension is not correctly
 detected, please `open an issue <https://github.com/fsfe/reuse-tool/issues>`_.
 
 Normally, the tool uses a single-line comment style when it is available (e.g.,
 `//` is used instead of `/* */` for C comment styles). If no single-line comment
 style is available, a multi-line style is used. You can force a certain comment
@@ -166,14 +157,17 @@
 The default template is:
 
 .. code-block:: jinja
 
   {% for copyright_line in copyright_lines %}
   {{ copyright_line }}
   {% endfor %}
+  {% for contributor_line in contributor_lines %}
+  SPDX-FileContributor: {{ contributor_line }}
+  {% endfor %}
 
   {% for expression in spdx_expressions %}
   SPDX-License-Identifier: {{ expression }}
   {% endfor %}
 
 Templates are automatically commented by the tool, depending on the detected or
 specified comment style.
@@ -182,14 +176,15 @@
 ``.reuse/templates/``. If you create the template ``mytemplate.jinja2``, you can
 use it with ``reuse annotate --copyright="Jane Doe" --template=mytemplate
 foo.py``.
 
 Inside of the template, you have access to the following variables:
 
 - ``copyright_lines`` --- a list of copyright notices (string).
+- ``contributor_lines`` --- a list of contributors (string).
 - ``spdx_expressions`` --- a list of SPDX License Expressions (string).
 
 In the future, more variables will be added.
 
 In some cases, you might want to do custom comment formatting. In those cases,
 you can pre-format your header as a comment. When doing so, suffix your template
 with ``.commented.jinja2``.
```

### Comparing `reuse-1.1.2/po/de.po` & `reuse-2.0.0/po/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2020-01-09 13:51+0100\n"
-"PO-Revision-Date: 2020-02-10 16:07+0100\n"
-"Language-Team: \n"
+"PO-Revision-Date: 2023-06-21 09:53+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: German <https://hosted.weblate.org/projects/fsfe/reuse-tool/"
+"de/>\n"
+"Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"X-Generator: Poedit 2.2.4\n"
-"Last-Translator: Carmen Bianca BAKKER <carmen@carmenbianca.eu>\n"
-"Language: de\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 4.18.1\n"
 
 #: src/reuse/_main.py:30
 msgid ""
 "reuse is a tool for compliance with the REUSE recommendations. See <https://"
 "reuse.software/> for more information, and <https://reuse.readthedocs.io/> "
 "for the online documentation."
 msgstr ""
@@ -99,24 +100,24 @@
 "\n"
 "IMPORTANT: This is currently EXPERIMENTAL!"
 msgstr ""
 "Schreibe Urheberrechts- und Lizenzinformationen in die Kopfzeilen von einer "
 "oder mehr Dateien.\n"
 "\n"
 "Mit der Benutzung von --copyright und --license können Sie bestimmen, welche "
-"Urheber und Lizenzen Sie in die Kopfzeilen der jeweiligen Dateien "
-"hinzufügen.\n"
+"Urheber und Lizenzen Sie in die Kopfzeilen der jeweiligen Dateien hinzufügen."
+"\n"
 "\n"
 "Der Kommentarstil wird normalerweise automatisch erkannt. Wenn das nicht der "
 "Fall ist, endet der Vorgang. Benutzen Sie --style um einen Kommentarstil zu "
 "bestimmen oder zu forcieren.\n"
 "\n"
 "Sie können die Vorlage für die Kopfzeilen-Kommentare mit --template ändern. "
-"Erstellen Sie dazu eine Jinja2-Vorlage in .reuse/templates/mytemplate."
-"jinja2. Sie können die Vorlage verwenden mithilfe von '--template "
+"Erstellen Sie dazu eine Jinja2-Vorlage in .reuse/templates/"
+"mytemplate.jinja2. Sie können die Vorlage verwenden mithilfe von '--template "
 "mytemplate'. Mehr Informationen zu dieser Funktion in der Online-"
 "Dokumentation.\n"
 "\n"
 "Wenn eine Binärdatei erkannt wurde, oder wenn --explicit-license verwendet "
 "wurde, werden die Kopfzeilen in einer .license-Datei gespeichert.\n"
 "\n"
 "WICHTIG: Diese Funktion ist momentan EXPERIMENTELL!"
@@ -288,16 +289,16 @@
 
 #: src/reuse/header.py:293
 #, python-brace-format
 msgid ""
 "'{path}' does not have a recognised file extension, please use --style or --"
 "explicit-license"
 msgstr ""
-"'{path}' hat keine erkannte Dateiendung, bitte verwenden Sie --style oder --"
-"explicit-license"
+"'{path}' hat keine erkannte Dateiendung, bitte verwenden Sie --style oder "
+"--explicit-license"
 
 #: src/reuse/header.py:352
 #, python-brace-format
 msgid "Error: Could not create comment for '{path}'"
 msgstr "Fehler: Kann kein Kommentar für '{path}' erstellen"
 
 #: src/reuse/header.py:359
@@ -440,16 +441,16 @@
 "Spezifikation :-)"
 
 #: src/reuse/lint.py:62
 msgid ""
 "Unfortunately, your project is not compliant with version {} of the REUSE "
 "Specification :-("
 msgstr ""
-"Leider ist Ihr Projekt nicht konform mit Version {} der REUSE-"
-"Spezifikation :-("
+"Leider ist Ihr Projekt nicht konform mit Version {} der REUSE-Spezifikation "
+":-("
 
 #: src/reuse/lint.py:79
 msgid "BAD LICENSES"
 msgstr "FALSCHE LIZENZEN"
 
 #: src/reuse/lint.py:83 src/reuse/lint.py:148
 msgid "'{}' found in:"
```

### Comparing `reuse-1.1.2/po/eo.po` & `reuse-2.0.0/po/eo.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,33 +3,34 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 msgid ""
 msgstr ""
 "Project-Id-Version: unnamed project\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2019-12-20 12:18+0100\n"
-"PO-Revision-Date: 2019-12-20 12:21+0100\n"
-"Last-Translator: Carmen Bianca BAKKER <carmen@carmenbianca.eu>\n"
-"Language-Team: Esperanto <gnome-eo-list@gnome.org>\n"
+"PO-Revision-Date: 2023-02-16 16:01+0000\n"
+"Last-Translator: Carmen Bianca Bakker <account@carmenbianca.eu>\n"
+"Language-Team: Esperanto <https://hosted.weblate.org/projects/fsfe/"
+"reuse-tool/eo/>\n"
 "Language: eo\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"X-Generator: Poedit 2.2.4\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 4.16-dev\n"
 
 #: src/reuse/_main.py:30
 msgid ""
 "reuse is a tool for compliance with the REUSE recommendations. See <https://"
 "reuse.software/> for more information, and <https://reuse.readthedocs.io/> "
 "for the online documentation."
 msgstr ""
-"reuse estas ilo por konformiĝo al la rekomendoj de REUSE. Vidu <https://"
-"reuse.software/> por pli da informo, kaj <https://reuse.readthedocs.io/> por "
-"la reta dokumentado."
+"reuse estas ilo por konformiĝo al la rekomendoj de REUSE. Vidu <https://reuse"
+".software/> por pli da informo, kaj <https://reuse.readthedocs.io/> por la "
+"reta dokumentado."
 
 #: src/reuse/_main.py:36
 msgid ""
 "This version of reuse is compatible with version {} of the REUSE "
 "Specification."
 msgstr "Ĉi tiu versio de reuse kongruas al versio {} de la REUSE Specifo."
 
@@ -95,22 +96,21 @@
 "header is placed in a .license file.\n"
 "\n"
 "IMPORTANT: This is currently EXPERIMENTAL!"
 msgstr ""
 "Aldoni kopirajtahn kaj permesilajn informojn en la kapojn de dosieroj.\n"
 "\n"
 "Tra uzi --copyright kaj --license, vi povas specifi kiujn kopirajtajn "
-"proprulojn kaj permesilojn oni aldonu al la kapojn de la specifitaj "
-"dosieroj.\n"
+"proprulojn kaj permesilojn oni aldonu al la kapojn de la specifitaj dosieroj."
+"\n"
 "\n"
 "Oni aŭtomate eltrovos la komentstilon de viaj dosieroj. Se oni ne povas "
 "eltrovi tion, la procezo haltas. Uzu --style por specifi aŭ superskribi la "
 "uzendan komentstilon.\n"
 "\n"
-"\n"
 "Vi povas ŝanĝi la ŝablonon de la kapo tra uzi --template. Metu Jinja2-"
 "ŝablonon en .reuse/templates/miaŝablono.jinja2. Vi povas uzi la ŝablonon tra "
 "specifi '--template miaŝablono'. Legu la reta dokumentado por pli da "
 "informoj pri ĉi tiu funkcio.\n"
 "\n"
 "Se oni detektas duuman dosieron, aŭ se vi specifas --explicit-license, la "
 "kapon oni metas en .license-dosieron.\n"
@@ -172,21 +172,24 @@
 "\n"
 "- Are any licenses included in the LICENSES/ directory that are not used "
 "inside of the project?\n"
 "\n"
 "- Do all files have valid copyright and licensing information?"
 msgstr ""
 "Kontroli la projektdosierujon por konformiĝo je versio {reuse_version} de la "
-"REUSE Specifo. Vi povas trovi la lastan version de la specifo ĉe <https://"
-"reuse.software/spec/>.\n"
+"REUSE Specifo. Vi povas trovi la lastan version de la specifo ĉe "
+"<https://reuse.software/spec/>.\n"
 "\n"
 "Specife, oni kontrolas la sekvajn kriteriojn:\n"
 "\n"
 "- Ĉu estas malbonaj (nekonitaj, nekonformaj) permesiloj en la projekto?\n"
 "\n"
+"- Ĉu uziĝas permesiloj en la projekto, kiuj ne estas en la LICENSES/"
+"-dosierujo?\n"
+"\n"
 "- Ĉu estas permesiloj en la LICENSES/-dosierujo, kiuj estas neuzataj?\n"
 "\n"
 "- Ĉu ĉiuj dosieroj havas validajn kopirajtajn kaj permesilajn informojn?"
 
 #: src/reuse/_main.py:199
 msgid "print the project's bill of materials in SPDX format"
 msgstr "presi la pecoliston de la projekto en SPDX-formo"
@@ -246,15 +249,15 @@
 msgstr "'{}' ne estas valida SPDX Permesila Identigilo."
 
 #: src/reuse/download.py:115 src/reuse/init.py:55
 msgid ""
 "See <https://spdx.org/licenses/> for a list of valid SPDX License "
 "Identifiers."
 msgstr ""
-"Vidu  <https://spdx.org/licenses/> por listo de validaj SPDX Permesilaj "
+"Vidu <https://spdx.org/licenses/> por listo de validaj SPDX Permesilaj "
 "Identigiloj."
 
 #: src/reuse/download.py:120
 msgid "Is your internet connection working?"
 msgstr "Ĉu via retkonekto funkcias?"
 
 #: src/reuse/download.py:125
```

### Comparing `reuse-1.1.2/po/es.po` & `reuse-2.0.0/po/es.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 msgid ""
 msgstr ""
 "Project-Id-Version: FSFE reuse\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2021-09-09 15:07+0100\n"
-"PO-Revision-Date: \n"
-"Last-Translator: Alejandro Criado-Pérez <alejandro@criadoperez.com>\n"
-"Language-Team: \n"
+"PO-Revision-Date: 2023-02-20 19:38+0000\n"
+"Last-Translator: gallegonovato <fran-carro@hotmail.es>\n"
+"Language-Team: Spanish <https://hosted.weblate.org/projects/fsfe/reuse-tool/"
+"es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"X-Generator: Poedit 2.2.1\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 4.18.1\n"
 
 #: src/reuse/_main.py:30
 msgid ""
 "reuse is a tool for compliance with the REUSE recommendations. See <https://"
 "reuse.software/> for more information, and <https://reuse.readthedocs.io/> "
 "for the online documentation."
 msgstr ""
@@ -97,34 +98,33 @@
 "documentation on how to use this feature.\n"
 "\n"
 "If a binary file is detected, or if --explicit-license is specified, the "
 "header is placed in a .license file.\n"
 "\n"
 "IMPORTANT: This is currently EXPERIMENTAL!"
 msgstr ""
-"Incluye el copyright y la licencia en la cabecera de uno o más archivos.\n"
+"Añade copyright y licencias en la cabecera de uno o más archivos.\n"
 "\n"
-"Utilizando --copyright y --license, puedes especificar qué propietarios del "
-"copyright y qué licencias añadir a las cabeceras de tales ficheros.\n"
+"Usando --copyright y --license, puede especificar qué titulares de derechos "
+"de autor y licencias añadir a las cabeceras de los archivos dados.\n"
 "\n"
-"El estilo del comentario debería ser autodetectado en tus ficheros. Si el "
-"estilo de un comentario no pudiera ser determinado, el proceso sería "
-"abortado. Usa --style para especificar, o sobreescribir, el estilo de "
-"comentario a utilizar.\n"
+"El estilo de comentario debería detectarse automáticamente para sus "
+"archivos. Si no se puede detectar un estilo de comentario, el proceso se "
+"aborta. Utilice --style para especificar o anular el estilo de comentario a "
+"utilizar.\n"
 "\n"
-"Puedes cambiar la plantilla de la cabecera utilizando --template. Coloca una "
-"plantilla Jinja2 en .reuse/templates/mytemplate.jinja2. Puedes utilizar la "
-"plantilla especificando '--template mytemplate'. Lee la documentación en "
-"línea que explica cómo utilizar esta función.\n"
+"Puede cambiar la plantilla del comentario de cabecera usando --template. "
+"Coloque una plantilla Jinja2 en .reuse/templates/mytemplate.jinja2. Puedes "
+"usar la plantilla especificando '--template mytemplate'. Lea la información "
+"en internet sobre cómo utilizar esta función.\n"
 "\n"
+"Si se detecta un archivo binario, o si se especifica --explicit-license, la "
+"cabecera se coloca en un archivo .license.\n"
 "\n"
-"Si se detecta un fichero de binarios, o si se especifica --explicit-license, "
-"la cabecera es incluida en un archivo .license.\n"
-"\n"
-"IMPORTANTE: ¡Esto es EXPERIMENTAL!"
+"IMPORTANTE: ¡Esto está actualmente disponible de forma EXPERIMENTAL!"
 
 #: src/reuse/_main.py:135
 msgid "download a license and place it in the LICENSES/ directory"
 msgstr "descarga una licencia y guárdala en el directorio \"LICENSES/\""
 
 #: src/reuse/_main.py:138
 msgid ""
@@ -191,16 +191,15 @@
 "\n"
 "- ¿Se hace referencia a alguna licencia dentro del proyecto, pero esta no se "
 "encuentra incluida en el directorio LICENSES/?\n"
 "\n"
 "- ¿Existe alguna licencia, de las incluidas en el directorio LICENSES/, que "
 "no esté en uso en el proyecto?\n"
 "\n"
-"- ¿Tienen todos los ficheros información válida sobre copyright y "
-"licencia?"
+"- ¿Tienen todos los ficheros información válida sobre copyright y licencia?"
 
 #: src/reuse/_main.py:199
 msgid "print the project's bill of materials in SPDX format"
 msgstr "imprime la lista de materiales del proyecto en formato SPDX"
 
 #: src/reuse/_util.py:216
 #, python-brace-format
@@ -315,22 +314,20 @@
 #. TODO: This may need to be rephrased more elegantly.
 #: src/reuse/header.py:370
 #, python-brace-format
 msgid "Successfully changed header of {path}"
 msgstr "Cabecera de {path} correctamente cambiada"
 
 #: src/reuse/header.py:383
-#, fuzzy
 msgid "copyright statement, repeatable"
-msgstr "declaración de copyright; repetible"
+msgstr "declaración de los derechos de autor, repetible"
 
 #: src/reuse/header.py:390
-#, fuzzy
 msgid "SPDX Identifier, repeatable"
-msgstr "Identificador SPDX; repetible"
+msgstr "Identificador SPDX, repetible"
 
 #: src/reuse/header.py:397
 msgid "year of copyright statement, optional"
 msgstr "año de la declaración de copyright; opcional"
 
 #: src/reuse/header.py:405
 msgid "comment style to use, optional"
@@ -384,22 +381,20 @@
 "Identificador SPDX de Licencia."
 
 #: src/reuse/init.py:40
 msgid "To stop adding licenses, hit RETURN."
 msgstr "Para terminar de añadir licencias pulsa RETORNO."
 
 #: src/reuse/init.py:85
-#, fuzzy
 msgid "Project already initialized"
-msgstr "Proyecto ya iniciado"
+msgstr "Proyecto ya inicializado"
 
 #: src/reuse/init.py:89
-#, fuzzy
 msgid "Initializing project for REUSE."
-msgstr "Iniciando proyecto para REUSE."
+msgstr "Inicializando el proyecto para REUSE."
 
 #: src/reuse/init.py:94
 msgid "What is the name of the project?"
 msgstr "¿Cuál es el nombre del proyecto?"
 
 #: src/reuse/init.py:100
 msgid "What is the internet address of the project?"
@@ -430,17 +425,16 @@
 msgstr "No se pudo descargar {}"
 
 #: src/reuse/init.py:139
 msgid "Creating .reuse/dep5"
 msgstr "Creando .reuse/dep5"
 
 #: src/reuse/init.py:162
-#, fuzzy
 msgid "Initialization complete."
-msgstr "Inicio completado."
+msgstr "Inicialización completa."
 
 #: src/reuse/lint.py:55
 msgid ""
 "Congratulations! Your project is compliant with version {} of the REUSE "
 "Specification :-)"
 msgstr ""
 "¡Enhorabuena! Tu proyecto es compatible con la versión {} de la "
@@ -455,15 +449,14 @@
 "Especificación REUSE :-("
 
 #: src/reuse/lint.py:79
 msgid "BAD LICENSES"
 msgstr "LICENCIAS MALAS"
 
 #: src/reuse/lint.py:83 src/reuse/lint.py:148
-#, fuzzy
 msgid "'{}' found in:"
 msgstr "'{}' encontrado en:"
 
 #: src/reuse/lint.py:101
 msgid "DEPRECATED LICENSES"
 msgstr "LICENCIAS OBSOLETAS"
 
@@ -501,17 +494,15 @@
 
 #: src/reuse/lint.py:209
 msgid "MISSING COPYRIGHT AND LICENSING INFORMATION"
 msgstr "FALTA INFORMACIÓN SOBRE COPYRIGHT Y LICENCIA"
 
 #: src/reuse/lint.py:214
 msgid "The following files have no copyright and licensing information:"
-msgstr ""
-"Los siguientes archivos carecen de información de copyright y "
-"licencia:"
+msgstr "Los siguientes archivos carecen de información de copyright y licencia:"
 
 #: src/reuse/lint.py:223
 msgid "The following files have no copyright information:"
 msgstr "Los siguientes ficheros carecen de información de copyright:"
 
 #: src/reuse/lint.py:229
 msgid "The following files have no licensing information:"
@@ -630,17 +621,16 @@
 #: /usr/lib64/python3.5/argparse.py:291 /usr/lib64/python3.6/argparse.py:295
 #: /usr/lib64/python3.7/argparse.py:297 /usr/lib64/python3.8/argparse.py:295
 msgid "usage: "
 msgstr "uso: "
 
 #: /usr/lib64/python3.5/argparse.py:822 /usr/lib64/python3.6/argparse.py:830
 #: /usr/lib64/python3.7/argparse.py:845 /usr/lib64/python3.8/argparse.py:846
-#, fuzzy
 msgid ".__call__() not defined"
-msgstr ".__call__() no está definido"
+msgstr ".__call__() no definido"
 
 #: /usr/lib64/python3.5/argparse.py:1119 /usr/lib64/python3.6/argparse.py:1127
 #: /usr/lib64/python3.7/argparse.py:1148 /usr/lib64/python3.8/argparse.py:1149
 #, python-format
 msgid "unknown parser %(parser_name)r (choices: %(choices)s)"
 msgstr ""
 "analizador sintáctico desconocido: %(parser_name)r (alternativas: "
@@ -662,27 +652,25 @@
 #: /usr/lib64/python3.7/argparse.py:1414 /usr/lib64/python3.8/argparse.py:1427
 #, python-format
 msgid "cannot merge actions - two groups are named %r"
 msgstr "no se pueden fusionar las acciones: dos grupos se llaman %r"
 
 #: /usr/lib64/python3.5/argparse.py:1423 /usr/lib64/python3.6/argparse.py:1431
 #: /usr/lib64/python3.7/argparse.py:1452 /usr/lib64/python3.8/argparse.py:1465
-#, fuzzy
 msgid "'required' is an invalid argument for positionals"
-msgstr "'required' es un argumento no válido para posicionales"
+msgstr "'required' es un argumento posicional inválido"
 
 #: /usr/lib64/python3.5/argparse.py:1445 /usr/lib64/python3.6/argparse.py:1453
 #: /usr/lib64/python3.7/argparse.py:1474 /usr/lib64/python3.8/argparse.py:1487
-#, fuzzy, python-format
+#, python-format
 msgid ""
 "invalid option string %(option)r: must start with a character "
 "%(prefix_chars)r"
 msgstr ""
-"la cadena de la opción %(option)r es inválida: debe comenzar con un carácter "
-"%(prefix_chars)r"
+"Opción no válida %(option)r: Debe comenzar con una letra %(prefix_chars)r"
 
 #: /usr/lib64/python3.5/argparse.py:1465 /usr/lib64/python3.6/argparse.py:1473
 #: /usr/lib64/python3.7/argparse.py:1494 /usr/lib64/python3.8/argparse.py:1507
 #, python-format
 msgid "dest= is required for options like %r"
 msgstr "se requiere dest= para opciones como %r"
 
@@ -949,8 +937,7 @@
 #~ msgstr "las notas de copyright son de obligatorio cumplimiento"
 
 #~ msgid "print the SPDX expressions of each provided file"
 #~ msgstr "imprime las expresiones SPDX de cada fichero proporcionado"
 
 #~ msgid "reuse, version {}\n"
 #~ msgstr "reuse, versión {}\n"
-
```

### Comparing `reuse-1.1.2/po/fr.po` & `reuse-2.0.0/po/fr.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,33 +3,34 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2020-01-15 20:23+0100\n"
-"PO-Revision-Date: 2020-01-20 14:33+0100\n"
-"Last-Translator: Carmen Bianca BAKKER <carmen@carmenbianca.eu>\n"
-"Language-Team: French\n"
+"PO-Revision-Date: 2023-02-18 10:24+0000\n"
+"Last-Translator: \"J. Lavoie\" <j.lavoie@net-c.ca>\n"
+"Language-Team: French <https://hosted.weblate.org/projects/fsfe/reuse-tool/"
+"fr/>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
-"X-Generator: Poedit 2.2.4\n"
+"Plural-Forms: nplurals=2; plural=n > 1;\n"
+"X-Generator: Weblate 4.16-dev\n"
 
 #: src/reuse/_main.py:30
 msgid ""
 "reuse is a tool for compliance with the REUSE recommendations. See <https://reuse."
 "software/> for more information, and <https://reuse.readthedocs.io/> for the "
 "online documentation."
 msgstr ""
-"reuse est un outil pour la conformité aux recommandations de l'initiative REUSE. "
-"Voir <https://reuse.software/> pour plus d'informations, et <https://reuse."
-"readthedocs.io/> pour la documentation en ligne."
+"reuse est un outil pour la conformité aux recommandations de l'initiative "
+"REUSE. Voir <https://reuse.software/> pour plus d'informations, et "
+"<https://reuse.readthedocs.io/> pour la documentation en ligne."
 
 #: src/reuse/_main.py:36
 msgid ""
 "This version of reuse is compatible with version {} of the REUSE Specification."
 msgstr ""
 "Cette version de reuse est compatible avec la version {} de la spécification "
 "REUSE."
@@ -40,17 +41,17 @@
 
 #: src/reuse/_main.py:43
 msgid ""
 "Donations are critical to our strength and autonomy. They enable us to continue "
 "working for Free Software wherever necessary. Please consider making a donation "
 "at <https://fsfe.org/donate/>."
 msgstr ""
-"Les dons sont cruciaux pour notre force et notre autonomie. Ils nous permettent "
-"de continuer à travailler pour le Logiciel Libre partout où c'est nécessaire. "
-"Merci d'envisager de faire un don <https://fsfe.org/donate/>."
+"Les dons sont cruciaux pour notre force et notre autonomie. Ils nous "
+"permettent de continuer à travailler pour le Logiciel Libre partout où c'est "
+"nécessaire. Merci d'envisager de faire un don <https://fsfe.org/donate/>."
 
 #: src/reuse/_main.py:66
 msgid "enable debug statements"
 msgstr "activer les instructions de débogage"
 
 #: src/reuse/_main.py:71
 msgid "do not skip over Git submodules"
@@ -95,30 +96,31 @@
 "use this feature.\n"
 "\n"
 "If a binary file is detected, or if --explicit-license is specified, the header "
 "is placed in a .license file.\n"
 "\n"
 "IMPORTANT: This is currently EXPERIMENTAL!"
 msgstr ""
-"Ajout des informations de droits d'auteur et de licence dans les en-têtes d'un ou "
-"plusieurs fichiers.\n"
+"Ajout des informations de droits d'auteur et de licence dans les en-têtes "
+"d'un ou plusieurs fichiers.\n"
 "\n"
-"En sélectionnant --copyright et --license, vous pouvez spécifier quels titulaires "
-"de droits et licences sont ajoutés aux en-têtes des fichiers listés.\n"
+"En sélectionnant --copyright et --license, vous pouvez spécifier quels "
+"titulaires de droits et licences sont ajoutés aux en-têtes des fichiers "
+"listés.\n"
 "\n"
 "Les styles de commentaire doivent être détectés automatiquement pour vos "
-"fichiers. Si un style de commentaire ne peut pas être détecté, le processus est "
-"interrompu. Utilisez --style pour spécifier ou passer outre le style de "
+"fichiers. Si un style de commentaire ne peut pas être détecté, le processus "
+"est interrompu. Utilisez --style pour spécifier ou passer outre le style de "
 "commentaire utilisé.\n"
 "\n"
-"Vous pouvez modifier le modèle des commentaires d'en-tête en utilisant l'option --"
-"template. Placez un modèle Jinja2 dans le répertoire .reuse/templates/mytemplate."
-"jinja2. Vous pouvez utiliser le modèle en précisant '--template mytemplate'. "
-"Consultez la documentation en ligne pour plus d'informations sur l'utilisation de "
-"cette fonctionnalité.\n"
+"Vous pouvez modifier le modèle des commentaires d'en-tête en utilisant "
+"l'option --template. Placez un modèle Jinja2 dans le répertoire .reuse/"
+"templates/mytemplate.jinja2. Vous pouvez utiliser le modèle en précisant '--"
+"template mytemplate'. Consultez la documentation en ligne pour plus "
+"d'informations sur l'utilisation de cette fonctionnalité.\n"
 "\n"
 "IMPORTANT: cette fonctionnalité est EXPÉRIMENTALE pour le moment !"
 
 #: src/reuse/_main.py:135
 msgid "download a license and place it in the LICENSES/ directory"
 msgstr "télécharger une licence et la placer dans le répertoire LICENSES/"
 
@@ -134,15 +136,16 @@
 "\n"
 "- The LICENSES/ directory in the current directory.\n"
 "\n"
 "If the LICENSES/ directory cannot be found, one is simply created."
 msgstr ""
 "Téléchargez une licence et placez-la dans le répertoire LICENSES/.\n"
 "\n"
-"Les répertoires LICENSES/ se trouvent automatiquement dans l'ordre suivant :\n"
+"Les répertoires LICENSES/ se trouvent automatiquement dans l'ordre suivant :"
+"\n"
 "\n"
 "- Le répertoire LICENSES/ à la racine du répertoire VCS.\n"
 "\n"
 "- Le répertoire actuel, si son nom est LICENSES.\n"
 "\n"
 "- Le répertoire LICENSES/ dans le répertoire courant.\n"
 "\n"
@@ -176,24 +179,24 @@
 "\n"
 "- Do all files have valid copyright and licensing information?"
 msgstr ""
 "Vérifiez le répertoire projet pour assurer la conformité à la version "
 "{reuse_version} de la spécification REUSE. Vous pouvez trouver la dernière "
 "version de la spécification à l'adresse <https://reuse.software/spec/>.\n"
 "\n"
-"En particulier, les critères suivants sont vérifiés :\n"
+"En particulier, les critères suivants sont vérifiés :\n"
 "\n"
-"- Une mauvaise licence (non reconnue, non-conforme à SPDX) se trouve-t-elle dans "
-"le projet?\n"
+"- Une mauvaise licence (non reconnue, non-conforme à SPDX) se trouve-t-elle "
+"dans le projet ?\n"
 "\n"
-"- Y a-t-il des licences dans le répertoire LICENSES/ qui sont inutilisées dans le "
-"projet?\n"
+"- Y a-t-il des licences dans le répertoire LICENSES/ qui sont inutilisées "
+"dans le projet ?\n"
 "\n"
-"- Tous les fichiers disposent-ils d'informations de droits d'auteur et de licence "
-"valides ?"
+"- Tous les fichiers disposent-ils d'informations de droits d'auteur et de "
+"licence valides ?"
 
 #: src/reuse/_main.py:199
 msgid "print the project's bill of materials in SPDX format"
 msgstr "imprimer la nomenclature du projet au format SPDX"
 
 #: src/reuse/_util.py:216
 #, python-brace-format
@@ -249,16 +252,16 @@
 msgid "'{}' is not a valid SPDX License Identifier."
 msgstr "'{}' n'est pas un identifiant de licence SPDX valide."
 
 #: src/reuse/download.py:115 src/reuse/init.py:55
 msgid ""
 "See <https://spdx.org/licenses/> for a list of valid SPDX License Identifiers."
 msgstr ""
-"Consultez <https://spdx.org/licenses/> pour une liste des identifiants de licence "
-"SPDX valides."
+"Consultez <https://spdx.org/licenses/> pour une liste des identifiants de "
+"licence SPDX valides."
 
 #: src/reuse/download.py:120
 msgid "Is your internet connection working?"
 msgstr "Votre connexion internet fonctionne-t-elle ?"
 
 #: src/reuse/download.py:125
 #, python-brace-format
@@ -272,40 +275,40 @@
 #: src/reuse/download.py:138
 msgid "cannot use --output with more than one license"
 msgstr "--output ne peut pas être utilisé avec plus d'une licence"
 
 #: src/reuse/header.py:103
 msgid "generated comment is missing copyright lines or license expressions"
 msgstr ""
-"les commentaires générés ne contiennent pas de ligne ou d'expression de droits "
-"d'auteur ou de licence"
+"les commentaires générés ne contiennent pas de ligne ou d'expression de "
+"droits d'auteur ou de licence"
 
 #: src/reuse/header.py:293
 #, python-brace-format
 msgid ""
 "'{path}' does not have a recognised file extension, please use --style or --"
 "explicit-license"
 msgstr ""
-"'{path}' n'est pas une extension de fichier reconnue, merci d'utiliser --style ou "
-"--explicit-license"
+"'{path}' n'est pas une extension de fichier reconnue, merci d'utiliser --"
+"style ou --explicit-license"
 
 #: src/reuse/header.py:352
 #, python-brace-format
 msgid "Error: Could not create comment for '{path}'"
 msgstr "Erreur : les commentaires ne peuvent être créés dans '{path}'"
 
 #: src/reuse/header.py:359
 #, python-brace-format
 msgid ""
 "Error: Generated comment header for '{path}' is missing copyright lines or "
 "license expressions. The template is probably incorrect. Did not write new header."
 msgstr ""
-"Erreur: l'en-tête de commentaire généré dans '{path}' ne contient pas de ligne ou "
-"d'expression de droits d'auteur ou de licence. Le modèle est probablement "
-"incorrect. Nouvel en-tête non écrit."
+"Erreur : l'en-tête de commentaire généré dans '{path}' ne contient pas de "
+"ligne ou d'expression de droits d'auteur ou de licence. Le modèle est "
+"probablement incorrect. Nouvel en-tête non écrit."
 
 #. TODO: This may need to be rephrased more elegantly.
 #: src/reuse/header.py:370
 #, python-brace-format
 msgid "Successfully changed header of {path}"
 msgstr "En-tête de {path} modifié avec succès"
 
@@ -356,16 +359,16 @@
 msgstr ""
 "'{path}' est un fichier binaire, par conséquent le fichier '{new_path}' est "
 "utilisé pour l'en-tête"
 
 #: src/reuse/init.py:25
 msgid "What license is your project under? Provide the SPDX License Identifier."
 msgstr ""
-"Sous quelle licence est enregistrè votre projet ? Merci de fournir un identifiant "
-"de licence SPDX."
+"Sous quelle licence est enregistrè votre projet ? Merci de fournir un "
+"identifiant de licence SPDX."
 
 #: src/reuse/init.py:29
 msgid ""
 "What other license is your project under? Provide the SPDX License Identifier."
 msgstr ""
 "Sous quelle autre licence est enregistré votre projet ? Merci de fournir un "
 "identifiant de licence SPDX."
@@ -392,19 +395,20 @@
 
 #: src/reuse/init.py:106
 msgid "What is the name of the maintainer?"
 msgstr "Quel est le nom de la personne chargée de la maintenance ?"
 
 #: src/reuse/init.py:112
 msgid "What is the e-mail address of the maintainer?"
-msgstr "Quelle est l'adresse mail de la personne chargée de la maintenance ?"
+msgstr ""
+"Quelle est l'adresse électronique de la personne chargée de la maintenance ?"
 
 #: src/reuse/init.py:118
 msgid "All done! Initializing now."
-msgstr "Tout est prêt ! Maintenant, on initialise."
+msgstr "Tout est prêt ! Maintenant, on initialise."
 
 #: src/reuse/init.py:126
 msgid "Downloading {}"
 msgstr "Télécharge {}"
 
 #: src/reuse/init.py:131
 msgid "{} already exists"
@@ -423,16 +427,16 @@
 msgstr "Initialisation terminée."
 
 #: src/reuse/lint.py:55
 msgid ""
 "Congratulations! Your project is compliant with version {} of the REUSE "
 "Specification :-)"
 msgstr ""
-"Félicitations ! Votre projet est conforme à la version {} de la spécification "
-"REUSE :-)"
+"Félicitations ! Votre projet est conforme à la version {} de la "
+"spécification REUSE :-)"
 
 #: src/reuse/lint.py:62
 msgid ""
 "Unfortunately, your project is not compliant with version {} of the REUSE "
 "Specification :-("
 msgstr ""
 "Malheureusement, votre projet n'est pas conforme à la version {} de la "
@@ -485,16 +489,16 @@
 #: src/reuse/lint.py:209
 msgid "MISSING COPYRIGHT AND LICENSING INFORMATION"
 msgstr "INFORMATION DE DROITS D'AUTEUR ET DE LICENCE MANQUANTE"
 
 #: src/reuse/lint.py:214
 msgid "The following files have no copyright and licensing information:"
 msgstr ""
-"Les fichiers suivants ne contiennent pas d'information de droits d'auteurs et de "
-"licence :"
+"Les fichiers suivants ne contiennent pas d'information de droits d'auteurs "
+"et de licence :"
 
 #: src/reuse/lint.py:223
 msgid "The following files have no copyright information:"
 msgstr ""
 "Les fichiers suivants ne contiennent pas d'information de droits d'auteurs :"
 
 #: src/reuse/lint.py:229
@@ -533,15 +537,16 @@
 #, python-brace-format
 msgid "Read errors: {count}"
 msgstr "Erreurs de lecture : {count}"
 
 #: src/reuse/lint.py:308
 #, python-brace-format
 msgid "Files with copyright information: {count} / {total}"
-msgstr "Fichiers contenant des informations de droits d'auteur : {count} / {total}"
+msgstr ""
+"Fichiers contenant des informations de droits d'auteur : {count} / {total}"
 
 #: src/reuse/lint.py:317
 #, python-brace-format
 msgid "Files with license information: {count} / {total}"
 msgstr "Fichiers contenant des informations de licence : {count} / {total}"
 
 #: src/reuse/project.py:59
@@ -553,16 +558,16 @@
 msgid "'{path}' covered by .reuse/dep5"
 msgstr "'{path}' est couvert par .reuse/dep5"
 
 #: src/reuse/project.py:145
 #, python-brace-format
 msgid "'{path}' holds an SPDX expression that cannot be parsed, skipping the file"
 msgstr ""
-"'{path}' contient une expression SPDX qui ne peut pas être analysée, le fichier "
-"est ignoré"
+"'{path}' contient une expression SPDX qui ne peut pas être analysée, le "
+"fichier est ignoré"
 
 #: src/reuse/project.py:231
 msgid ".reuse/dep5 has syntax errors"
 msgstr ".reuse/dep5 contient des erreurs de syntaxe"
 
 #: src/reuse/project.py:257
 #, python-brace-format
@@ -577,18 +582,18 @@
 #: src/reuse/project.py:275
 #, python-brace-format
 msgid ""
 "Could not resolve SPDX License Identifier of {path}, resolving to {identifier}. "
 "Make sure the license is in the license list found at <https://spdx.org/licenses/"
 "> or that it starts with 'LicenseRef-', and that it has a file extension."
 msgstr ""
-"Impossible de résoudre l'identifiant de licence SPDX de {path}, utilisation de "
-"{identifier}. Merci de vérifier que la licence est dans la liste trouvable "
-"à<https://spdx.org/licenses/> ou qu'elle débute par 'LicenseRef-', et qu'elle "
-"contient une extension de fichier."
+"Impossible de résoudre l'identifiant de licence SPDX de {path}, utilisation "
+"de {identifier}. Merci de vérifier que la licence est dans la liste "
+"trouvable à<https://spdx.org/licenses/> ou qu'elle débute par 'LicenseRef-', "
+"et qu'elle contient une extension de fichier."
 
 #: src/reuse/project.py:287
 #, python-brace-format
 msgid "{identifier} is the SPDX License Identifier of both {path} and {other_path}"
 msgstr "{identifier} est l'identifiant de {path} comme de {other_path}"
 
 #: src/reuse/report.py:206
```

### Comparing `reuse-1.1.2/po/gl.po` & `reuse-2.0.0/po/gl.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,31 +2,24 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2020-01-09 13:51+0100\n"
-"PO-Revision-Date: 2020-01-17 22:07+0100\n"
-"Language-Team: \n"
+"PO-Revision-Date: 2023-06-21 09:53+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Galician <https://hosted.weblate.org/projects/fsfe/reuse-tool/"
+"gl/>\n"
+"Language: gl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Project-Id-Version: PACKAGE VERSION\n"
-"Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-01-09 13:51+0100\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=CHARSET\n"
-"Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"X-Generator: Poedit 2.2.4\n"
-"Last-Translator: \n"
-"Language: gl\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 4.18.1\n"
 
 #: src/reuse/_main.py:30
 msgid ""
 "reuse is a tool for compliance with the REUSE recommendations. See <https://"
 "reuse.software/> for more information, and <https://reuse.readthedocs.io/> "
 "for the online documentation."
 msgstr ""
@@ -111,17 +104,18 @@
 "copyright a engadir nas cabeceiras dos arquivos indicados.\n"
 "\n"
 "O estilo dos comentarios dos arquivos debería detectarse automáticamente, de "
 "non se detectar o proceso abórtase. Pódese usar --style para definir ou "
 "forzar o estilo de comentario a usar.\n"
 "\n"
 "É posible cambiar o modelo do comentario de cabeceira usando --template. Por "
-"exemplo, gardando o modelo Jinja2 na carpeta .reuse/templates/mytemplate."
-"jinja2 pode usar este modelo indicando  '--template mytemplate'. Consulte a "
-"documentación en liña para máis información sobre esta característica.\n"
+"exemplo, gardando o modelo Jinja2 na carpeta .reuse/templates/"
+"mytemplate.jinja2 pode usar este modelo indicando  '--template mytemplate'. "
+"Consulte a documentación en liña para máis información sobre esta "
+"característica.\n"
 "\n"
 "Se o arquivo é binario ou se especifica --explicit-license, a cabeceira "
 "gárdase nun arquivo .license.\n"
 "\n"
 "IMPORTANTE: Actualmente isto é EXPERIMENTAL!"
 
 #: src/reuse/_main.py:135
@@ -257,16 +251,16 @@
 msgstr "'{}' non é un Identificador de Licenza SPDX válido."
 
 #: src/reuse/download.py:115 src/reuse/init.py:55
 msgid ""
 "See <https://spdx.org/licenses/> for a list of valid SPDX License "
 "Identifiers."
 msgstr ""
-"Consulte unha lista de Identificadores de Licenza SPDX válidos en <https://"
-"spdx.org/licenses/>."
+"Consulte unha lista de Identificadores de Licenza SPDX válidos en "
+"<https://spdx.org/licenses/>."
 
 #: src/reuse/download.py:120
 msgid "Is your internet connection working?"
 msgstr "Está a funcionar a súa conexión a internet?"
 
 #: src/reuse/download.py:125
 #, python-brace-format
@@ -279,16 +273,15 @@
 
 #: src/reuse/download.py:138
 msgid "cannot use --output with more than one license"
 msgstr "non se pode usar --output con máis dunha licenza"
 
 #: src/reuse/header.py:103
 msgid "generated comment is missing copyright lines or license expressions"
-msgstr ""
-"o comentario xerado non ten liñas de copyright ou expresións de licenza"
+msgstr "o comentario xerado non ten liñas de copyright ou expresións de licenza"
 
 #: src/reuse/header.py:293
 #, python-brace-format
 msgid ""
 "'{path}' does not have a recognised file extension, please use --style or --"
 "explicit-license"
 msgstr ""
```

### Comparing `reuse-1.1.2/po/it.po` & `reuse-2.0.0/po/it.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 msgid ""
 msgstr ""
 "Project-Id-Version: FSFE reuse\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2020-01-09 13:51+0100\n"
-"PO-Revision-Date: \n"
-"Last-Translator: Carmen Bianca BAKKER <carmen@carmenbianca.eu>\n"
-"Language-Team: \n"
+"PO-Revision-Date: 2023-02-18 10:24+0000\n"
+"Last-Translator: \"J. Lavoie\" <j.lavoie@net-c.ca>\n"
+"Language-Team: Italian <https://hosted.weblate.org/projects/fsfe/reuse-tool/"
+"it/>\n"
 "Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"X-Generator: Poedit 2.3\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 4.16-dev\n"
 
 #: src/reuse/_main.py:30
 msgid ""
 "reuse is a tool for compliance with the REUSE recommendations. See <https://"
 "reuse.software/> for more information, and <https://reuse.readthedocs.io/> "
 "for the online documentation."
 msgstr ""
@@ -111,16 +112,16 @@
 "style per specificare o forzare lo stile dei commenti da usare.\n"
 "\n"
 "Puoi cambiare il modello dell'intestazione utilizzando --template. Metti un "
 "modello Jinja2 in .reuse/templates/miomodello.jinja2. Puoi usare il modello "
 "specificando '--template miomodello'. Leggi la documentazione in linea su "
 "come usare questa funzione.\n"
 "\n"
-"Se viene rilevato un file binario, o se --explicit-licence viene specificato, "
-"l'intestazione verrà inserita nel file .license.\n"
+"Se viene rilevato un file binario, o se --explicit-licence viene "
+"specificato, l'intestazione verrà inserita nel file .license.\n"
 "\n"
 "IMPORTANTE: Questo è ancora SPERIMENTALE!"
 
 #: src/reuse/_main.py:135
 msgid "download a license and place it in the LICENSES/ directory"
 msgstr "scarica una licenza e salvala nella directory LICENSES/"
 
@@ -180,22 +181,22 @@
 msgstr ""
 "Controlla che la directory del progetto sia conforme con la versione "
 "{reuse_version} della Specifica REUSE. Puoi trovare l'ultima versione della "
 "specifica su <https://reuse.software/spec/>\n"
 "\n"
 "In particolare, vengono eseguiti i seguenti controlli:\n"
 "\n"
-"- Nel progetto c'è qualche licenza non valida (non riconosciuta, non conforme "
-"con SPDX)?\n"
+"- Nel progetto c'è qualche licenza non valida (non riconosciuta, non "
+"conforme con SPDX)?\n"
 "\n"
 "- C'è qualche licenza utilizzata all'interno del progetto, ma non inclusa "
 "nella directory LICENSES/?\n"
 "\n"
-"- C'è qualche licenza inclusa della directory LICENSES/ ma non utilizzata nel "
-"progetto?\n"
+"- C'è qualche licenza inclusa della directory LICENSES/ ma non utilizzata "
+"nel progetto?\n"
 "\n"
 "- Tutti i file hanno informazioni valide sul copyright e sulla licenza?"
 
 #: src/reuse/_main.py:199
 msgid "print the project's bill of materials in SPDX format"
 msgstr "stampa l'elenco dei componenti del progetto in formato SPDX"
 
@@ -354,21 +355,22 @@
 msgid "template {template} could not be found"
 msgstr "il modello {template} non è stato trovato"
 
 #: src/reuse/header.py:482
 #, python-brace-format
 msgid "'{path}' is a binary, therefore using '{new_path}' for the header"
 msgstr ""
-"'{path}' è un file binario, occorre utilizzare '{new_path}' per l'intestazione"
+"'{path}' è un file binario, occorre utilizzare '{new_path}' per "
+"l'intestazione"
 
 #: src/reuse/init.py:25
 msgid "What license is your project under? Provide the SPDX License Identifier."
 msgstr ""
-"Sotto quale licenza viene rilasciato il tuo progetto? Indica l'Identificativo "
-"di Licenza SPDX."
+"Sotto quale licenza viene rilasciato il tuo progetto? Indica "
+"l'Identificativo di Licenza SPDX."
 
 #: src/reuse/init.py:29
 msgid ""
 "What other license is your project under? Provide the SPDX License Identifier."
 msgstr ""
 "Quali altre licenze utilizza il tuo progetto? Indica l'Identificativo di "
 "Licenza SPDX."
@@ -554,16 +556,16 @@
 msgstr "'{path}' verificato da .reuse/dep5"
 
 #: src/reuse/project.py:145
 #, python-brace-format
 msgid ""
 "'{path}' holds an SPDX expression that cannot be parsed, skipping the file"
 msgstr ""
-"'{path}' contiene un'espressione SPDX che non può essere parsificata, il file "
-"viene saltato."
+"'{path}' contiene un'espressione SPDX che non può essere parsificata, il "
+"file viene saltato"
 
 #: src/reuse/project.py:231
 msgid ".reuse/dep5 has syntax errors"
 msgstr ".reuse/dep5 presenta errori di sintassi"
 
 #: src/reuse/project.py:257
 #, python-brace-format
@@ -581,16 +583,16 @@
 "Could not resolve SPDX License Identifier of {path}, resolving to "
 "{identifier}. Make sure the license is in the license list found at <https://"
 "spdx.org/licenses/> or that it starts with 'LicenseRef-', and that it has a "
 "file extension."
 msgstr ""
 "Non è possibile rilevare l'Identificativo di Licenza SPDX per {path}, viene "
 "impostato a {identifier}. Assicurati che la licenza sia nella lista delle "
-"licenze elencate su <https://spdx.org/licenses/> o che inizi con "
-"'LicenseRef-', e che abbia un'estensione del file."
+"licenze elencate su <https://spdx.org/licenses/> o che inizi con 'LicenseRef-"
+"', e che abbia un'estensione del file."
 
 #: src/reuse/project.py:287
 #, python-brace-format
 msgid ""
 "{identifier} is the SPDX License Identifier of both {path} and {other_path}"
 msgstr ""
 "{identifier} è l'Identificativo di Licenza SPDX sia di {path} che di "
```

### Comparing `reuse-1.1.2/po/nl.po` & `reuse-2.0.0/po/nl.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2019-12-20 12:18+0100\n"
-"PO-Revision-Date: 2020-01-11 20:35+0100\n"
-"Last-Translator: Carmen Bianca BAKKER <carmen@carmenbianca.eu>\n"
-"Language-Team: Esperanto <>\n"
+"PO-Revision-Date: 2023-02-18 10:24+0000\n"
+"Last-Translator: \"J. Lavoie\" <j.lavoie@net-c.ca>\n"
+"Language-Team: Dutch <https://hosted.weblate.org/projects/fsfe/reuse-tool/nl/"
+">\n"
 "Language: nl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"X-Generator: Poedit 2.2.4\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 4.18.1\n"
 
 #: src/reuse/_main.py:30
 msgid ""
 "reuse is a tool for compliance with the REUSE recommendations. See <https://"
 "reuse.software/> for more information, and <https://reuse.readthedocs.io/> "
 "for the online documentation."
 msgstr ""
@@ -397,15 +398,15 @@
 
 #: src/reuse/init.py:106
 msgid "What is the name of the maintainer?"
 msgstr "Wat is de naam van de beheerder?"
 
 #: src/reuse/init.py:112
 msgid "What is the e-mail address of the maintainer?"
-msgstr "Wat is het emailadres van de beheerder?"
+msgstr "Wat is het e-mailadres van de beheerder?"
 
 #: src/reuse/init.py:118
 msgid "All done! Initializing now."
 msgstr "Klaar! Nu aan het initialiseren."
 
 #: src/reuse/init.py:126
 msgid "Downloading {}"
@@ -434,16 +435,15 @@
 msgstr ""
 "Gefeliciteerd! Uw project leeft nu versie {} van de REUSE-specificatie na :-)"
 
 #: src/reuse/lint.py:62
 msgid ""
 "Unfortunately, your project is not compliant with version {} of the REUSE "
 "Specification :-("
-msgstr ""
-"Helaas leeft uw project versie {} van de REUSE-specificatie niet na :-("
+msgstr "Helaas leeft uw project versie {} van de REUSE-specificatie niet na :-("
 
 #: src/reuse/lint.py:79
 msgid "BAD LICENSES"
 msgstr "SLECHTE LICENTIES"
 
 #: src/reuse/lint.py:83 src/reuse/lint.py:148
 msgid "'{}' found in:"
@@ -581,15 +581,15 @@
 #, python-brace-format
 msgid ""
 "Could not resolve SPDX License Identifier of {path}, resolving to "
 "{identifier}. Make sure the license is in the license list found at <https://"
 "spdx.org/licenses/> or that it starts with 'LicenseRef-', and that it has a "
 "file extension."
 msgstr ""
-"Kon de SPDX Licentie Identificatie van {path} niet bepalen, bepalen "
+"Kon de SPDX Licentie Identificatie van {path} niet bepalen, dus gebruiken we "
 "{identifier}. Zorg ervoor dat de licentie zich in de licentielijst bevind "
 "die gevonden kan worden op <https://spdx.org/licenses/> of dat deze begint "
 "met 'LicenseRef-' en dat deze een bestandsextensie heeft."
 
 #: src/reuse/project.py:287
 #, python-brace-format
 msgid ""
```

### Comparing `reuse-1.1.2/po/pt.po` & `reuse-2.0.0/po/pt.po`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2020-01-09 13:51+0100\n"
-"PO-Revision-Date: 2020-01-20 14:55+0100\n"
+"PO-Revision-Date: 2023-06-21 09:53+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Portuguese <https://hosted.weblate.org/projects/fsfe/"
+"reuse-tool/pt/>\n"
 "Language: pt\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
-"Last-Translator: Carmen Bianca BAKKER <carmen@carmenbianca.eu>\n"
-"Language-Team: \n"
-"X-Generator: Poedit 2.2.4\n"
+"Plural-Forms: nplurals=2; plural=n > 1;\n"
+"X-Generator: Weblate 4.18.1\n"
 
 #: src/reuse/_main.py:30
 msgid ""
 "reuse is a tool for compliance with the REUSE recommendations. See <https://"
 "reuse.software/> for more information, and <https://reuse.readthedocs.io/> "
 "for the online documentation."
 msgstr ""
@@ -253,16 +254,16 @@
 msgstr "'{}' não é um Identificador de Licença SPDX válido."
 
 #: src/reuse/download.py:115 src/reuse/init.py:55
 msgid ""
 "See <https://spdx.org/licenses/> for a list of valid SPDX License "
 "Identifiers."
 msgstr ""
-"Consultar uma lista de Identificadores de Licença SPDX válidos em <https://"
-"spdx.org/licenses/>."
+"Consultar uma lista de Identificadores de Licença SPDX válidos em "
+"<https://spdx.org/licenses/>."
 
 #: src/reuse/download.py:120
 msgid "Is your internet connection working?"
 msgstr "A ligação à Internet está a funcionar?"
 
 #: src/reuse/download.py:125
 #, python-brace-format
@@ -285,16 +286,16 @@
 
 #: src/reuse/header.py:293
 #, python-brace-format
 msgid ""
 "'{path}' does not have a recognised file extension, please use --style or --"
 "explicit-license"
 msgstr ""
-"'{path}' não têm uma extensão de ficheiro reconhecida; usar --style ou --"
-"explicit-license"
+"'{path}' não têm uma extensão de ficheiro reconhecida; usar --style ou "
+"--explicit-license"
 
 #: src/reuse/header.py:352
 #, python-brace-format
 msgid "Error: Could not create comment for '{path}'"
 msgstr "Erro: Não foi possível criar um comentário para '{path}'"
 
 #: src/reuse/header.py:359
@@ -590,16 +591,15 @@
 "publicada em <https://spdx.org/licenses/> ou que começa por 'LicenseRef-' e "
 "tem uma extensão de ficheiro."
 
 #: src/reuse/project.py:287
 #, python-brace-format
 msgid ""
 "{identifier} is the SPDX License Identifier of both {path} and {other_path}"
-msgstr ""
-"{identifier} é o Identificador de Licença SPDX de {path} e {other_path}"
+msgstr "{identifier} é o Identificador de Licença SPDX de {path} e {other_path}"
 
 #: src/reuse/report.py:206
 #, python-brace-format
 msgid "Could not read '{path}'"
 msgstr "Não foi possível ler '{path}'"
 
 #: src/reuse/report.py:213
```

### Comparing `reuse-1.1.2/po/tr.po` & `reuse-2.0.0/po/tr.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,33 +2,34 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 msgid ""
 msgstr ""
 "Project-Id-Version: FSFE reuse\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2020-01-09 13:51+0100\n"
-"PO-Revision-Date: 2020-01-12 18:28+0100\n"
-"Last-Translator: T. E. Kalayci <tekrei@member.fsf.org>\n"
-"Language-Team: \n"
+"PO-Revision-Date: 2023-06-21 09:53+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Turkish <https://hosted.weblate.org/projects/fsfe/reuse-tool/"
+"tr/>\n"
 "Language: tr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"X-Generator: Poedit 2.2.4\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 4.18.1\n"
 
 #: src/reuse/_main.py:30
 msgid ""
 "reuse is a tool for compliance with the REUSE recommendations. See <https://"
 "reuse.software/> for more information, and <https://reuse.readthedocs.io/> "
 "for the online documentation."
 msgstr ""
 "reuse, REUSE önerileriyle uyum için bir araçtır. Daha fazla bilgi için "
-"<https://reuse.software/> sitesini, çevrimiçi belgelendirme için <https://"
-"reuse.readthedocs.io/> sitesini ziyaret edebilirsiniz."
+"<https://reuse.software/> sitesini, çevrimiçi belgelendirme için "
+"<https://reuse.readthedocs.io/> sitesini ziyaret edebilirsiniz."
 
 #: src/reuse/_main.py:36
 msgid ""
 "This version of reuse is compatible with version {} of the REUSE "
 "Specification."
 msgstr "Bu reuse sürümü, REUSE Belirtiminin {} sürümüyle uyumludur."
 
@@ -104,16 +105,16 @@
 "Yorum biçimi dosyalarınız için otomatik olarak belirlenecektir. Eğer bir "
 "yorum biçimi belirlenemezse, süreç iptal edilecektir. Kullanılacak yorum "
 "biçimini belirtmek için --style değişkenini kullanın.\n"
 "\n"
 "Başlık yorumu şablonunu --template değişkenini kullanarak "
 "değiştirebilirsiniz. Bir Jinja2 şablonunu .reuse/templates/mytemplate.jinja2 "
 "içerisine koyun. Şablonu '--template mytemplate' şeklinde kullanabilirsiniz. "
-"Bu özelliği nasıl kullanabileceğinizi çevrimiçi belgelerden "
-"öğrenebilirsiniz.\n"
+"Bu özelliği nasıl kullanabileceğinizi çevrimiçi belgelerden öğrenebilirsiniz."
+"\n"
 "\n"
 "Eğer ikili bir dosya tespit edilirse veya eğer --explicit-license "
 "tanımlıysa, başlık .license dosyasına koyulacaktır.\n"
 "\n"
 "ÖNEMLİ: Bu şu anda DENEYSELDİR!"
 
 #: src/reuse/_main.py:135
@@ -176,16 +177,16 @@
 msgstr ""
 "Proje dizinini REUSE Belirtimi {reuse_version} sürümüyle uyumu için inceler. "
 "Belirtimin son sürümüne <https://reuse.software/spec/> adresinden "
 "erişebilirsiniz.\n"
 "\n"
 "Özellikle aşağıdaki ölçütler denetleniyor:\n"
 "\n"
-"- Projede herhangi bir kötü (tanımlanamayan, SPDX ile uyumsuz) lisans var "
-"mı?\n"
+"- Projede herhangi bir kötü (tanımlanamayan, SPDX ile uyumsuz) lisans var mı?"
+"\n"
 "\n"
 "- Projede belirtilen ama LICENSES/ dizininde yer almayan lisans var mı?\n"
 "\n"
 "- LICENSES/ dizininde yer alan ama projede kullanılmayan lisanslar var mı?\n"
 "\n"
 "- Bütün dosyalar telif hakkı ve lisans bilgisi içeriyor mu?"
 
@@ -278,16 +279,16 @@
 
 #: src/reuse/header.py:293
 #, python-brace-format
 msgid ""
 "'{path}' does not have a recognised file extension, please use --style or --"
 "explicit-license"
 msgstr ""
-"'{path}' tanınan bir dosya uzantısına sahip değil, lütfen --style veya --"
-"explicit-license değişkenlerini kullanın"
+"'{path}' tanınan bir dosya uzantısına sahip değil, lütfen --style veya "
+"--explicit-license değişkenlerini kullanın"
 
 #: src/reuse/header.py:352
 #, python-brace-format
 msgid "Error: Could not create comment for '{path}'"
 msgstr "Hata: '{path}' için yorum oluşturulamıyor"
 
 #: src/reuse/header.py:359
```

### Comparing `reuse-1.1.2/pyproject.toml` & `reuse-2.0.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # SPDX-FileCopyrightText: 2018 Free Software Foundation Europe e.V. <https://fsfe.org>
 # SPDX-FileCopyrightText: 2022 Alliander N.V. <https://www.alliander.com>
 # SPDX-FileCopyrightText: 2022 Carmen Bianca Bakker <carmenbianca@fsfe.org>
+# SPDX-FileCopyrightText: 2023 DB Systel GmbH
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 [tool.poetry]
 name = "reuse"
-version = "1.1.2"
+version = "2.0.0"
 description = "reuse is a tool for compliance with the REUSE recommendations."
 authors = [
     "Free Software Foundation Europe <contact@fsfe.org>",
 ]
 maintainers = [
     "Carmen Bianca Bakker <carmenbianca@fsfe.org>",
+    "Max Mehl <max.mehl@fsfe.org>",
+    "Linus Sehn <linus@fsfe.org>",
 ]
-license = "Apache-2.0 AND CC0-1.0 AND GPL-3.0-or-later"
+license = "Apache-2.0 AND CC0-1.0 AND CC-BY-SA-4.0 AND GPL-3.0-or-later"
 readme = "README.md"
 
 packages = [
     { include = "reuse", from = "src" }
 ]
 include = [
     { path = "src/reuse/locale/**/*.mo", format="wheel" },
@@ -35,52 +38,84 @@
 homepage = "https://reuse.software/"
 repository = "https://github.com/fsfe/reuse-tool"
 documentation = "https://reuse.readthedocs.org/"
 
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
+    "License :: OSI Approved",
+    "License :: DFSG approved",
+    "License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication",
+    "License :: OSI Approved :: Apache Software License",
+    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6.2"
+python = "^3.8"
 Jinja2 = "^3.0.0"
 binaryornot = "^0.4.4"
 "boolean.py" = ">=3.8"
 license-expression = ">=1.0"
 python-debian = "^0.1.38,!=0.1.45,!=0.1.46,!=0.1.47"
-setuptools = "*"
 
 [tool.poetry.dev-dependencies]
 Sphinx = ">=4.0.0"
 recommonmark = "^0.7.1"
 sphinx-autodoc-typehints = "^1.12.0"
-sphinx-rtd-theme = "^1.0.0"
 sphinxcontrib-apidoc = "^0.3.0"
+furo = "^2023.3.27"
 black = ">=20"
 isort = "^5.6.0"
 bump2version = "^1.0.0"
 pre-commit = "^2.9.0"
 pylint = "^2.12.2"
 pytest = ">=6.0.0"
 pytest-cov = ">=2.10.0"
+mypy = "^1.0"
 
 [tool.poetry.scripts]
 reuse = 'reuse._main:main'
 
 [tool.poetry.build]
 generate-setup-file = false
 script = "_build.py"
 
 [build-system]
-requires = ["poetry-core>=1.1.0", "setuptools"]
+requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 80
 
 [tool.isort]
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 line_length = 80
+
+[tool.pytest.ini_options]
+addopts = "--doctest-modules"
+
+[tool.mypy]
+files = [
+    "src/reuse/**.py",
+    "tests/**.py",
+]
+exclude = [
+    '^_build\.py$',
+    '^conf\.py$',
+]
+
+[[tool.mypy.overrides]]
+module = "reuse.*"
+disallow_untyped_defs = true
+disallow_incomplete_defs = true
+
+[[tool.mypy.overrides]]
+module = [
+    "binaryornot.check",
+    "boolean.boolean",
+    "license_expression",
+    "pkg_resources",
+]
+ignore_missing_imports = true
```

### Comparing `reuse-1.1.2/src/reuse/_comment.py` & `reuse-2.0.0/src/reuse/comment.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,25 +5,29 @@
 # SPDX-FileCopyrightText: 2021 Alvar Penning
 # SPDX-FileCopyrightText: 2021 Robin Vobruba <hoijui.quaero@gmail.com>
 # SPDX-FileCopyrightText: 2021 Matija Šuklje <matija@suklje.name>
 # SPDX-FileCopyrightText: 2022 Florian Snow <florian@familysnow.net>
 # SPDX-FileCopyrightText: 2022 Nico Rikken <nico.rikken@fsfe.org>
 # SPDX-FileCopyrightText: 2022 Stefan Hynek <stefan.hynek@uni-goettingen.de>
 # SPDX-FileCopyrightText: 2022 Carmen Bianca Bakker <carmenbianca@fsfe.org>
+# SPDX-FileCopyrightText: 2022 Sebastian Crane <seabass@fsfe.org>
+# SPDX-FileCopyrightText: 2023 Redradix S.L. <info@redradix.com>
+# SPDX-FileCopyrightText: 2023 Kevin Meagher
+# SPDX-FileCopyrightText: 2023 Mathias Dannesbo <md@magenta.dk>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Module for parsing and creating comments. Just enough to deal with comment
 headers, in any case.
 """
 
 import logging
 import operator
 from textwrap import dedent
-from typing import List, NamedTuple
+from typing import List, NamedTuple, Type
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class CommentParseError(Exception):
     """An error occurred during the parsing of a comment."""
 
@@ -41,23 +45,24 @@
     middle: str
     end: str
 
 
 class CommentStyle:
     """Base class for comment style."""
 
+    SHORTHAND = ""
     SINGLE_LINE = ""
     INDENT_AFTER_SINGLE = ""
     # (start, middle, end)
     # e.g., ("/*", "*", "*/")
     MULTI_LINE = MultiLineSegments("", "", "")
     INDENT_BEFORE_MIDDLE = ""
     INDENT_AFTER_MIDDLE = ""
     INDENT_BEFORE_END = ""
-    SHEBANGS = []
+    SHEBANGS: List[str] = []
 
     @classmethod
     def can_handle_single(cls) -> bool:
         """Whether the :class:`CommentStyle` can handle single-line comments."""
         return bool(cls.SINGLE_LINE)
 
     @classmethod
@@ -134,24 +139,24 @@
         """Uncomment all lines in *text*, assuming they are commented by
         single-line comments.
 
         :raises CommentParseError: if *text* could not be parsed.
         """
         if not cls.can_handle_single():
             raise CommentParseError(f"{cls} cannot parse single-line comments")
-        result = []
+        result_lines = []
 
         for line in text.splitlines():
             if not line.startswith(cls.SINGLE_LINE):
                 raise CommentParseError(
                     f"'{line}' does not start with a comment marker"
                 )
             line = line.lstrip(cls.SINGLE_LINE)
-            result.append(line)
-        result = "\n".join(result)
+            result_lines.append(line)
+        result = "\n".join(result_lines)
         return dedent(result)
 
     @classmethod
     def _remove_middle_marker(cls, line: str) -> str:
         if cls.MULTI_LINE.middle:
             possible_line = line.lstrip()
             prefix = cls.MULTI_LINE.middle
@@ -173,60 +178,60 @@
         multi-line comments.
 
         :raises CommentParseError: if *text* could not be parsed.
         """
         if not cls.can_handle_multi():
             raise CommentParseError(f"{cls} cannot parse multi-line comments")
 
-        result = []
+        result_lines = []
         try:
             first, *lines, last = text.splitlines()
             last_is_first = False
         except ValueError:
             first = text
             lines = []
-            last = None  # Set this later.
+            last = ""  # Set this later.
             last_is_first = True
 
         if not first.startswith(cls.MULTI_LINE.start):
             raise CommentParseError(
                 f"'{first}' does not start with a comment marker"
             )
         first = first.lstrip(cls.MULTI_LINE.start)
         first = first.lstrip()
 
         for line in lines:
             line = cls._remove_middle_marker(line)
-            result.append(line)
+            result_lines.append(line)
 
         if last_is_first:
             last = first
             first = ""
         if not last.endswith(cls.MULTI_LINE.end):
             raise CommentParseError(
                 f"'{last}' does not end with a comment delimiter"
             )
         last = last.rstrip(cls.MULTI_LINE.end)
         last = last.rstrip()
         last = cls._remove_middle_marker(last)
 
-        result = "\n".join(result)
+        result = "\n".join(result_lines)
         result = dedent(result)
 
         return "\n".join(item for item in (first, result, last) if item)
 
     @classmethod
     def comment_at_first_character(cls, text: str) -> str:
         """Return the comment block that starts at the first character of
         *text*. This is chiefly handy to get the header comment of a file,
         assuming that the header comment starts at the first character in the
         file.
 
         :raises CommentParseError: if *text* does not start with a parseable
-        comment block.
+            comment block.
         """
         if not any((cls.can_handle_single(), cls.can_handle_multi())):
             raise CommentParseError(f"{cls} cannot parse comments")
 
         lines = text.splitlines()
 
         if cls.can_handle_single() and text.startswith(cls.SINGLE_LINE):
@@ -250,50 +255,50 @@
             "Could not find a parseable comment block at the first character"
         )
 
 
 class AppleScriptCommentStyle(CommentStyle):
     """AppleScript comment style."""
 
-    _shorthand = "applescript"
+    SHORTHAND = "applescript"
 
     SINGLE_LINE = "--"
     INDENT_AFTER_SINGLE = " "
     MULTI_LINE = MultiLineSegments("(*", "", "*)")
 
 
 class AspxCommentStyle(CommentStyle):
     """ASPX comment style."""
 
-    _shorthand = "aspx"
+    SHORTHAND = "aspx"
 
     MULTI_LINE = MultiLineSegments("<%--", "", "--%>")
 
 
 class BatchFileCommentStyle(CommentStyle):
     """Windows batch file comment style."""
 
-    _shorthand = "bat"
+    SHORTHAND = "bat"
 
     SINGLE_LINE = "REM"
     INDENT_AFTER_SINGLE = " "
 
 
 class BibTexCommentStyle(CommentStyle):
     """BibTex comment style."""
 
-    _shorthand = "bibtex"
+    SHORTHAND = "bibtex"
 
     MULTI_LINE = MultiLineSegments("@Comment{", "", "}")
 
 
 class CCommentStyle(CommentStyle):
     """C comment style."""
 
-    _shorthand = "c"
+    SHORTHAND = "c"
 
     SINGLE_LINE = "//"
     INDENT_AFTER_SINGLE = " "
     MULTI_LINE = MultiLineSegments("/*", "*", "*/")
     INDENT_BEFORE_MIDDLE = " "
     INDENT_AFTER_MIDDLE = " "
     INDENT_BEFORE_END = " "
@@ -302,15 +307,15 @@
         "<?php",  # PHP
     ]
 
 
 class CssCommentStyle(CommentStyle):
     """CSS comment style."""
 
-    _shorthand = "css"
+    SHORTHAND = "css"
 
     MULTI_LINE = MultiLineSegments("/*", "*", "*/")
     INDENT_BEFORE_MIDDLE = " "
     INDENT_AFTER_MIDDLE = " "
     INDENT_BEFORE_END = " "
 
 
@@ -329,176 +334,178 @@
     def comment_at_first_character(cls, text: str) -> str:
         return text
 
 
 class FortranCommentStyle(CommentStyle):
     """Fortran comment style."""
 
-    _shorthand = "f"
+    SHORTHAND = "f"
 
     SINGLE_LINE = "c"
     INDENT_AFTER_SINGLE = " "
 
 
 class FtlCommentStyle(CommentStyle):
     """FreeMarker Template Language comment style."""
 
-    _shorthand = "ftl"
+    SHORTHAND = "ftl"
 
     MULTI_LINE = MultiLineSegments("<#--", "", "-->")
 
 
 class HandlebarsCommentStyle(CommentStyle):
     """Handlebars comment style."""
 
-    _shorthand = "handlebars"
+    SHORTHAND = "handlebars"
 
     MULTI_LINE = MultiLineSegments("{{!--", "", "--}}")
 
 
 class HaskellCommentStyle(CommentStyle):
     """Haskell comment style."""
 
-    _shorthand = "haskell"
+    SHORTHAND = "haskell"
 
     SINGLE_LINE = "--"
     INDENT_AFTER_SINGLE = " "
 
 
 class HtmlCommentStyle(CommentStyle):
     """HTML comment style."""
 
-    _shorthand = "html"
+    SHORTHAND = "html"
 
     MULTI_LINE = MultiLineSegments("<!--", "", "-->")
     SHEBANGS = ["<?xml"]
 
 
 class JinjaCommentStyle(CommentStyle):
     """Jinja2 comment style."""
 
-    _shorthand = "jinja"
+    SHORTHAND = "jinja"
 
     MULTI_LINE = MultiLineSegments("{#", "", "#}")
 
 
 class LispCommentStyle(CommentStyle):
     """Lisp comment style."""
 
-    _shorthand = "lisp"
+    SHORTHAND = "lisp"
 
     SINGLE_LINE = ";"
     INDENT_AFTER_SINGLE = " "
 
 
 class M4CommentStyle(CommentStyle):
     """M4 (autoconf) comment style."""
 
-    _shorthand = "m4"
+    SHORTHAND = "m4"
 
     SINGLE_LINE = "dnl"
     INDENT_AFTER_SINGLE = " "
 
 
 class MlCommentStyle(CommentStyle):
     """ML comment style."""
 
-    _shorthand = "ml"
+    SHORTHAND = "ml"
 
     MULTI_LINE = MultiLineSegments("(*", "*", "*)")
     INDENT_BEFORE_MIDDLE = " "
     INDENT_AFTER_MIDDLE = " "
     INDENT_BEFORE_END = " "
 
 
 class PlantUmlCommentStyle(CommentStyle):
     """PlantUML comment style."""
 
-    _shorthand = "plantuml"
+    SHORTHAND = "plantuml"
 
     SINGLE_LINE = "'"
     INDENT_AFTER_SINGLE = " "
     MULTI_LINE = MultiLineSegments("/'", "'", "'/")
     INDENT_BEFORE_MIDDLE = " "
     INDENT_AFTER_MIDDLE = " "
     INDENT_BEFORE_END = " "
 
 
 class PythonCommentStyle(CommentStyle):
     """Python comment style."""
 
-    _shorthand = "python"
+    SHORTHAND = "python"
 
     SINGLE_LINE = "#"
     INDENT_AFTER_SINGLE = " "
     SHEBANGS = ["#!"]
 
 
 class ReStructedTextCommentStyle(CommentStyle):
     """reStructuredText comment style."""
 
-    _shorthand = "rst"
+    SHORTHAND = "rst"
 
     SINGLE_LINE = ".."
     INDENT_AFTER_SINGLE = " "
 
 
 class TexCommentStyle(CommentStyle):
     """TeX comment style."""
 
-    _shorthand = "tex"
+    SHORTHAND = "tex"
 
     SINGLE_LINE = "%"
     INDENT_AFTER_SINGLE = " "
 
 
 class UncommentableCommentStyle(EmptyCommentStyle):
     """A pseudo comment style to indicate that this file is uncommentable. This
     results in an external .license file as for binaries or --explicit-license.
     """
 
 
 class VelocityCommentStyle(CommentStyle):
     """Apache Velocity Template Language comment style."""
 
-    _shorthand = "vst"
+    SHORTHAND = "vst"
 
     # TODO: SINGLE_LINE requires refactor to support trailing `**`.
     MULTI_LINE = MultiLineSegments("#*", "  ", "*#")
 
 
 class VimCommentStyle(CommentStyle):
     """Vim(Script|Config) style."""
 
-    _shorthand = "vim"
+    SHORTHAND = "vim"
 
     SINGLE_LINE = '"'
     INDENT_AFTER_SINGLE = " "
 
 
 class XQueryCommentStyle(CommentStyle):
     """XQuery comment style."""
 
-    _shorthand = "xquery"
+    SHORTHAND = "xquery"
 
     MULTI_LINE = MultiLineSegments("(:", ":", ":)")
     INDENT_BEFORE_MIDDLE = " "
     INDENT_AFTER_MIDDLE = " "
     INDENT_BEFORE_END = " "
 
 
 #: A map of (common) file extensions against comment types.
 EXTENSION_COMMENT_STYLE_MAP = {
     ".adb": HaskellCommentStyle,
     ".adoc": CCommentStyle,
     ".ads": HaskellCommentStyle,
+    ".aes": UncommentableCommentStyle,
     ".ahk": LispCommentStyle,
     ".ahkl": LispCommentStyle,
     ".aidl": CCommentStyle,
     ".applescript": AppleScriptCommentStyle,
+    ".arb": UncommentableCommentStyle,
     ".asax": AspxCommentStyle,
     ".asc": CCommentStyle,
     ".asciidoc": CCommentStyle,
     ".ashx": AspxCommentStyle,
     ".asmx": AspxCommentStyle,
     ".aspx": AspxCommentStyle,
     ".aux": TexCommentStyle,
@@ -508,25 +515,28 @@
     ".bat": BatchFileCommentStyle,
     ".bb": PythonCommentStyle,
     ".bbappend": PythonCommentStyle,
     ".bbclass": PythonCommentStyle,
     ".bib": BibTexCommentStyle,
     ".c": CCommentStyle,
     ".cc": CCommentStyle,
+    ".cjs": CCommentStyle,
     ".cl": LispCommentStyle,
     ".clj": LispCommentStyle,
     ".cljc": LispCommentStyle,
     ".cljs": LispCommentStyle,
     ".cmake": PythonCommentStyle,  # TODO: Bracket comments not supported.
+    ".code-workspace": CCommentStyle,
     ".coffee": PythonCommentStyle,
     ".cpp": CCommentStyle,
     ".cs": CCommentStyle,
     ".csl": HtmlCommentStyle,  # Bibliography (XML based)
     ".css": CssCommentStyle,
     ".csv": UncommentableCommentStyle,
+    ".cxx": CCommentStyle,
     ".d": CCommentStyle,
     ".dart": CCommentStyle,
     ".di": CCommentStyle,
     ".doc": UncommentableCommentStyle,
     ".docx": UncommentableCommentStyle,
     ".dotx": UncommentableCommentStyle,
     ".dts": CCommentStyle,
@@ -536,28 +546,30 @@
     ".ex": PythonCommentStyle,
     ".exs": PythonCommentStyle,
     ".f": FortranCommentStyle,
     ".f03": FortranCommentStyle,
     ".f90": FortranCommentStyle,
     ".f95": FortranCommentStyle,
     ".fish": PythonCommentStyle,
+    ".fnl": LispCommentStyle,
     ".fodp": UncommentableCommentStyle,
     ".fods": UncommentableCommentStyle,
     ".fodt": UncommentableCommentStyle,
     ".for": FortranCommentStyle,
     ".fs": CCommentStyle,
     ".ftl": FtlCommentStyle,
     ".gemspec": PythonCommentStyle,
     ".go": CCommentStyle,
     ".gradle": CCommentStyle,
     ".graphql": PythonCommentStyle,
     ".groovy": CCommentStyle,
     ".h": CCommentStyle,
     ".ha": CCommentStyle,
     ".hbs": HandlebarsCommentStyle,
+    ".hcl": PythonCommentStyle,
     ".hh": CCommentStyle,
     ".hpp": CCommentStyle,
     ".hrl": TexCommentStyle,
     ".hs": HaskellCommentStyle,
     ".html": HtmlCommentStyle,
     ".hx": CCommentStyle,
     ".hxsl": CCommentStyle,
@@ -566,14 +578,15 @@
     ".ipynb": UncommentableCommentStyle,
     ".iuml": PlantUmlCommentStyle,
     ".java": CCommentStyle,
     ".jinja": JinjaCommentStyle,
     ".jinja2": JinjaCommentStyle,
     ".js": CCommentStyle,
     ".json": UncommentableCommentStyle,
+    ".jsp": AspxCommentStyle,
     ".jsx": CCommentStyle,
     ".jy": PythonCommentStyle,
     ".ksh": PythonCommentStyle,
     ".kt": CCommentStyle,
     ".kts": CCommentStyle,
     ".l": LispCommentStyle,
     ".latex": TexCommentStyle,
@@ -614,61 +627,70 @@
     ".pl": PythonCommentStyle,
     ".plantuml": PlantUmlCommentStyle,
     ".po": PythonCommentStyle,
     ".pod": PythonCommentStyle,
     ".pot": PythonCommentStyle,
     ".ppt": UncommentableCommentStyle,
     ".pptx": UncommentableCommentStyle,
+    ".pri": PythonCommentStyle,
+    ".pro": PythonCommentStyle,
     ".proto": CCommentStyle,
     ".ps1": PythonCommentStyle,  # TODO: Multiline comments
     ".psm1": PythonCommentStyle,  # TODO: Multiline comments
     ".pu": PlantUmlCommentStyle,
     ".puml": PlantUmlCommentStyle,
     ".pxd": PythonCommentStyle,
     ".py": PythonCommentStyle,
     ".pyi": PythonCommentStyle,
     ".pyw": PythonCommentStyle,
     ".pyx": PythonCommentStyle,
     ".qbs": CCommentStyle,
     ".qml": CCommentStyle,
+    ".qrc": UncommentableCommentStyle,
+    ".qss": CssCommentStyle,
     ".R": PythonCommentStyle,
     ".rake": PythonCommentStyle,
     ".rb": PythonCommentStyle,
     ".rbw": PythonCommentStyle,
     ".rbx": PythonCommentStyle,
     ".rkt": LispCommentStyle,
     ".Rmd": HtmlCommentStyle,
     ".rs": CCommentStyle,
     ".rss": HtmlCommentStyle,
     ".rst": ReStructedTextCommentStyle,
     ".sass": CssCommentStyle,
     ".sbt": CCommentStyle,
     ".sc": CCommentStyle,  # SuperCollider source file
     ".scad": CCommentStyle,
-    ".scala": PythonCommentStyle,
+    ".scala": CCommentStyle,
     ".scm": LispCommentStyle,
     ".scpt": AppleScriptCommentStyle,
     ".scptd": AppleScriptCommentStyle,
     ".scss": CssCommentStyle,
     # SuperCollider synth definition (binary)
     ".scsyndef": UncommentableCommentStyle,
     ".sh": PythonCommentStyle,
     ".sml": MlCommentStyle,
     ".soy": CCommentStyle,
     ".sql": HaskellCommentStyle,
     ".sty": TexCommentStyle,
     ".svg": UncommentableCommentStyle,
+    ".svelte": HtmlCommentStyle,
     ".swift": CCommentStyle,
     ".tex": TexCommentStyle,
+    ".textile": HtmlCommentStyle,
+    ".tf": PythonCommentStyle,
+    ".tfvars": PythonCommentStyle,
     ".thy": MlCommentStyle,
     ".toc": TexCommentStyle,
     ".toml": PythonCommentStyle,
     ".ts": CCommentStyle,
     ".tsx": CCommentStyle,
     ".ttl": PythonCommentStyle,  # Turtle/RDF
+    ".ui": UncommentableCommentStyle,
     ".v": CCommentStyle,  # V-Lang source code
     ".vala": CCommentStyle,
     ".vim": VimCommentStyle,
     ".vm": VelocityCommentStyle,
     ".vsh": CCommentStyle,  # V-Lang script
     ".vtl": VelocityCommentStyle,
     ".vue": HtmlCommentStyle,
@@ -685,30 +707,35 @@
     ".xsl": HtmlCommentStyle,
     ".yaml": PythonCommentStyle,
     ".yml": PythonCommentStyle,
     ".zsh": PythonCommentStyle,
 }
 
 EXTENSION_COMMENT_STYLE_MAP_LOWERCASE = {
-    k.lower(): v for k, v in EXTENSION_COMMENT_STYLE_MAP.items()
+    key.lower(): value for key, value in EXTENSION_COMMENT_STYLE_MAP.items()
 }
 
 FILENAME_COMMENT_STYLE_MAP = {
     ".bashrc": PythonCommentStyle,
+    ".browserslist": PythonCommentStyle,
+    ".clang-format": PythonCommentStyle,
     ".coveragerc": PythonCommentStyle,
     ".dockerignore": PythonCommentStyle,
     ".editorconfig": PythonCommentStyle,
     ".eslintignore": PythonCommentStyle,
     ".eslintrc": UncommentableCommentStyle,
     ".gitattributes": PythonCommentStyle,
     ".gitignore": PythonCommentStyle,
     ".gitmodules": PythonCommentStyle,
     ".mailmap": PythonCommentStyle,
+    ".metadata": UncommentableCommentStyle,
     ".mdlrc": PythonCommentStyle,  # Markdown-linter config
     ".npmignore": PythonCommentStyle,
+    ".prettierrc": UncommentableCommentStyle,  # could either be JSON or YAML
+    ".prettierignore": PythonCommentStyle,
     ".pylintrc": PythonCommentStyle,
     ".Renviron": PythonCommentStyle,
     ".Rprofile": PythonCommentStyle,
     ".vimrc": VimCommentStyle,
     ".yarnrc": PythonCommentStyle,
     "ansible.cfg": PythonCommentStyle,
     "archive.sctxar": UncommentableCommentStyle,  # SuperCollider global archive
@@ -726,37 +753,36 @@
     "Jenkinsfile": CCommentStyle,
     "Makefile.am": PythonCommentStyle,
     "Makefile": PythonCommentStyle,
     "MANIFEST.in": PythonCommentStyle,
     "manifest": PythonCommentStyle,  # used by cdist
     "meson.build": PythonCommentStyle,
     "meson_options.txt": PythonCommentStyle,
+    "pubspec.lock": UncommentableCommentStyle,
     "Rakefile": PythonCommentStyle,
     "requirements.txt": PythonCommentStyle,
     "ROOT": MlCommentStyle,
     "setup.cfg": PythonCommentStyle,
     "sonar-project.properties": PythonCommentStyle,
     "yarn.lock": UncommentableCommentStyle,
 }
 
 FILENAME_COMMENT_STYLE_MAP_LOWERCASE = {
-    k.lower(): v for k, v in FILENAME_COMMENT_STYLE_MAP.items()
+    key.lower(): value for key, value in FILENAME_COMMENT_STYLE_MAP.items()
 }
 
 
-def _all_style_classes() -> List[CommentStyle]:
+def _all_style_classes() -> List[Type[CommentStyle]]:
     """Return a list of all defined style classes, excluding the base class."""
     result = []
     for key, value in globals().items():
         if key.endswith("CommentStyle") and key != "CommentStyle":
             result.append(value)
     return sorted(result, key=operator.attrgetter("__name__"))
 
 
-# pylint: disable=protected-access
-
 _result = _all_style_classes()
 _result.remove(EmptyCommentStyle)
 _result.remove(UncommentableCommentStyle)
 
 #: A map of human-friendly names against style classes.
-NAME_STYLE_MAP = {style._shorthand: style for style in _result}
+NAME_STYLE_MAP = {style.SHORTHAND: style for style in _result}
```

### Comparing `reuse-1.1.2/src/reuse/_licenses.py` & `reuse-2.0.0/src/reuse/_licenses.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,37 +7,38 @@
 # load_license_list was copied and altered from its original location
 # at <https://github.com/spdx/tools-python/blob/master/spdx/config.py>.
 
 """A list with all SPDX licenses."""
 
 import json
 import os
+from typing import Dict, List, Tuple
 
 _BASE_DIR = os.path.dirname(__file__)
 _RESOURCES_DIR = os.path.join(_BASE_DIR, "resources")
 _LICENSES = os.path.join(_RESOURCES_DIR, "licenses.json")
 _EXCEPTIONS = os.path.join(_RESOURCES_DIR, "exceptions.json")
 
 
-def _load_license_list(file_name):
+def _load_license_list(file_name: str) -> Tuple[List[int], Dict[str, Dict]]:
     """Return the licenses list version tuple and a mapping of licenses
     id->name loaded from a JSON file
     from https://github.com/spdx/license-list-data
     """
     licenses_map = {}
     with open(file_name, "r", encoding="utf-8") as lics:
         licenses = json.load(lics)
         version = licenses["licenseListVersion"].split(".")
         for lic in licenses["licenses"]:
             identifier = lic["licenseId"]
             licenses_map[identifier] = lic
     return version, licenses_map
 
 
-def _load_exception_list(file_name):
+def _load_exception_list(file_name: str) -> Tuple[List[int], Dict[str, Dict]]:
     """Return the exceptions list version tuple and a mapping of
     exceptions id->name loaded from a JSON file
     from https://github.com/spdx/license-list-data
     """
     exceptions_map = {}
     with open(file_name, "r", encoding="utf-8") as excs:
         exceptions = json.load(excs)
```

### Comparing `reuse-1.1.2/src/reuse/_main.py` & `reuse-2.0.0/src/reuse/_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 """Entry functions for reuse."""
 
 import argparse
 import logging
 import sys
 from gettext import gettext as _
-from typing import List
+from typing import IO, Callable, List, Optional, Type, cast
 
 from . import (
     __REUSE_version__,
     __version__,
     download,
     header,
     init,
@@ -110,14 +110,17 @@
                 "Add copyright and licensing into the header of one or more"
                 " files.\n"
                 "\n"
                 "By using --copyright and --license, you can specify which"
                 " copyright holders and licenses to add to the headers of the"
                 " given files.\n"
                 "\n"
+                "By using --contributor, you can specify people or entity that"
+                " contributed but are not copyright holder of the given files."
+                "\n"
                 "The first comment is replaced with a new header containing"
                 " the new copyright and licensing information and its former"
                 " copyright and licensing. If you want to keep the first"
                 " comment intact, use --no-replace.\n"
                 "\n"
                 "The comment style should be auto-detected for your files. If"
                 " a comment style could not be detected and --skip-unrecognised"
@@ -143,15 +146,15 @@
     )
 
     add_command(
         subparsers,
         "addheader",
         header.add_arguments,
         header.run,
-        help=argparse.SUPPRESS,
+        help=_("deprecated in favor of annotate"),
     )
 
     add_command(
         subparsers,
         "download",
         download.add_arguments,
         download.run,
@@ -231,22 +234,22 @@
         aliases=["supported-licences"],
     )
 
     return parser
 
 
 def add_command(  # pylint: disable=too-many-arguments,redefined-builtin
-    subparsers,
+    subparsers: argparse._SubParsersAction,
     name: str,
-    add_arguments_func,
-    run_func,
-    formatter_class=None,
-    description: str = None,
-    help: str = None,
-    aliases: list = None,
+    add_arguments_func: Callable[[argparse.ArgumentParser], None],
+    run_func: Callable[[argparse.Namespace, Project, IO[str]], int],
+    formatter_class: Optional[Type[argparse.HelpFormatter]] = None,
+    description: Optional[str] = None,
+    help: Optional[str] = None,
+    aliases: Optional[List[str]] = None,
 ) -> None:
     """Add a subparser for a command."""
     if formatter_class is None:
         formatter_class = argparse.RawTextHelpFormatter
     subparser = subparsers.add_parser(
         name,
         formatter_class=formatter_class,
@@ -255,18 +258,18 @@
         aliases=aliases or [],
     )
     add_arguments_func(subparser)
     subparser.set_defaults(func=run_func)
     subparser.set_defaults(parser=subparser)
 
 
-def main(args: List[str] = None, out=sys.stdout) -> int:
+def main(args: Optional[List[str]] = None, out: IO[str] = sys.stdout) -> int:
     """Main entry function."""
     if args is None:
-        args = sys.argv[1:]
+        args = cast(List[str], sys.argv[1:])
 
     main_parser = parser()
     parsed_args = main_parser.parse_args(args)
 
     setup_logging(level=logging.DEBUG if parsed_args.debug else logging.WARNING)
 
     if parsed_args.version:
```

### Comparing `reuse-1.1.2/src/reuse/_util.py` & `reuse-2.0.0/src/reuse/_util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,57 @@
 # SPDX-FileCopyrightText: 2017 Free Software Foundation Europe e.V. <https://fsfe.org>
 # SPDX-FileCopyrightText: © 2020 Liferay, Inc. <https://liferay.com>
 # SPDX-FileCopyrightText: 2020 Tuomas Siipola <tuomas@zpl.fi>
 # SPDX-FileCopyrightText: 2022 Nico Rikken <nico.rikken@fsfe.org>
 # SPDX-FileCopyrightText: 2022 Florian Snow <florian@familysnow.net>
 # SPDX-FileCopyrightText: 2022 Carmen Bianca Bakker <carmenbianca@fsfe.org>
 # SPDX-FileCopyrightText: 2022 Pietro Albini <pietro.albini@ferrous-systems.com>
+# SPDX-FileCopyrightText: 2023 DB Systel GmbH
+# SPDX-FileCopyrightText: 2023 Johannes Zarl-Zierl <johannes@zarl-zierl.at>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Misc. utilities for reuse."""
 
 
 import logging
 import os
 import re
 import shutil
 import subprocess
 import sys
 from argparse import ArgumentTypeError
+from collections import Counter
 from difflib import SequenceMatcher
 from gettext import gettext as _
 from hashlib import sha1
 from itertools import chain
 from os import PathLike
 from pathlib import Path
-from typing import BinaryIO, Iterator, List, Optional, Set
+from typing import IO, Any, BinaryIO, Dict, Iterator, List, Optional, Set, Union
 
 from boolean.boolean import Expression, ParseError
 from debian.copyright import Copyright
 from license_expression import ExpressionError, Licensing
 
-from . import SpdxInfo
-from ._comment import _all_style_classes
+from . import ReuseInfo, SourceType
 from ._licenses import ALL_NON_DEPRECATED_MAP
+from .comment import _all_style_classes
+
+# TODO: When removing Python 3.8 support, use PathLike[str]
+StrPath = Union[str, PathLike]
 
 GIT_EXE = shutil.which("git")
 HG_EXE = shutil.which("hg")
 
 REUSE_IGNORE_START = "REUSE-IgnoreStart"
 REUSE_IGNORE_END = "REUSE-IgnoreEnd"
 
+SPDX_SNIPPET_INDICATOR = b"SPDX-SnippetBegin"
+
 _LOGGER = logging.getLogger(__name__)
 _LICENSING = Licensing()
 
 # REUSE-IgnoreStart
 
 _END_PATTERN = r"{}$".format(
     "".join(
@@ -68,37 +76,46 @@
                         r"\]\s*::",
                     ]
                 ),
             )
         }
     )
 )
-_IDENTIFIER_PATTERN = re.compile(
+_LICENSE_IDENTIFIER_PATTERN = re.compile(
     r"^(.*?)SPDX-License-Identifier:[ \t]+(.*?)" + _END_PATTERN, re.MULTILINE
 )
+_CONTRIBUTOR_PATTERN = re.compile(
+    r"^(.*?)SPDX-FileContributor:[ \t]+(.*?)" + _END_PATTERN, re.MULTILINE
+)
+# The keys match the relevant attributes of ReuseInfo.
+_SPDX_TAGS: Dict[str, re.Pattern] = {
+    "spdx_expressions": _LICENSE_IDENTIFIER_PATTERN,
+    "contributor_lines": _CONTRIBUTOR_PATTERN,
+}
+
 _COPYRIGHT_PATTERNS = [
     re.compile(
-        r"(?P<copyright>(?P<prefix>SPDX-FileCopyrightText:)\s+"
-        r"((?P<year>\d{4} - \d{4}|\d{4}),?\s+)?"
+        r"(?P<copyright>(?P<prefix>SPDX-(File|Snippet)CopyrightText:)\s+"
+        r"((?P<year>\d{4} ?- ?\d{4}|\d{4}),?\s+)?"
         r"(?P<statement>.*?))" + _END_PATTERN
     ),
     re.compile(
         r"(?P<copyright>(?P<prefix>Copyright(\s?\([cC]\))?)\s+"
-        r"((?P<year>\d{4} - \d{4}|\d{4}),?\s+)?"
+        r"((?P<year>\d{4} ?- ?\d{4}|\d{4}),?\s+)?"
         r"(?P<statement>.*?))" + _END_PATTERN
     ),
     re.compile(
         r"(?P<copyright>(?P<prefix>©)\s+"
-        r"((?P<year>\d{4} - \d{4}|\d{4}),?\s+)?"
+        r"((?P<year>\d{4} ?- ?\d{4}|\d{4}),?\s+)?"
         r"(?P<statement>.*?))" + _END_PATTERN
     ),
 ]
-
 _COPYRIGHT_STYLES = {
     "spdx": "SPDX-FileCopyrightText:",
+    "spdx-c": "SPDX-FileCopyrightText: (C)",
     "spdx-symbol": "SPDX-FileCopyrightText: ©",
     "string": "Copyright",
     "string-c": "Copyright (C)",
     "string-symbol": "Copyright ©",
     "symbol": "©",
 }
 
@@ -122,35 +139,38 @@
         handler = logging.StreamHandler()
         formatter = logging.Formatter("%(name)s - %(levelname)s - %(message)s")
         handler.setFormatter(formatter)
         library_logger.addHandler(handler)
 
 
 def execute_command(
-    command: List[str], logger: logging.Logger, cwd: PathLike = None, **kwargs
+    command: List[str],
+    logger: logging.Logger,
+    cwd: Optional[StrPath] = None,
+    **kwargs: Any,
 ) -> subprocess.CompletedProcess:
     """Run the given command with subprocess.run. Forward kwargs. Silence
     output into a pipe unless kwargs override it.
     """
     logger.debug("running '%s'", " ".join(command))
 
-    stdout = kwargs.get("stdout", subprocess.PIPE)
-    stderr = kwargs.get("stderr", subprocess.PIPE)
+    stdout: Union[None, int, IO[Any]] = kwargs.get("stdout", subprocess.PIPE)
+    stderr: Union[None, int, IO[Any]] = kwargs.get("stderr", subprocess.PIPE)
 
     return subprocess.run(
-        map(str, command),
+        list(map(str, command)),
         stdout=stdout,
         stderr=stderr,
         check=False,
         cwd=str(cwd),
         **kwargs,
     )
 
 
-def find_licenses_directory(root: PathLike) -> Optional[Path]:
+def find_licenses_directory(root: StrPath) -> Path:
     """Find the licenses directory from CWD or *root*. In the following order:
 
     - LICENSES/ in *root*.
 
     - Current directory if its name is "LICENSES"
 
     - LICENSES/ in CWD.
@@ -158,80 +178,101 @@
     The returned LICENSES/ directory NEED NOT EXIST. It may still need to be
     created.
     """
     cwd = Path.cwd()
     licenses_path = cwd / "LICENSES"
 
     if root:
-        licenses_path = root / "LICENSES"
+        licenses_path = Path(root) / "LICENSES"
     elif cwd.name == "LICENSES":
         licenses_path = cwd
 
     return licenses_path
 
 
-def decoded_text_from_binary(binary_file: BinaryIO, size: int = None) -> str:
+def decoded_text_from_binary(
+    binary_file: BinaryIO, size: Optional[int] = None
+) -> str:
     """Given a binary file object, detect its encoding and return its contents
     as a decoded string. Do not throw any errors if the encoding contains
     errors:  Just replace the false characters.
 
     If *size* is specified, only read so many bytes.
     """
+    if size is None:
+        size = -1
     rawdata = binary_file.read(size)
     result = rawdata.decode("utf-8", errors="replace")
     return result.replace("\r\n", "\n")
 
 
-def _determine_license_path(path: PathLike) -> Path:
+def _determine_license_path(path: StrPath) -> Path:
     """Given a path FILE, return FILE.license if it exists, otherwise return
     FILE.
     """
     license_path = Path(f"{path}.license")
     if not license_path.exists():
         license_path = Path(path)
     return license_path
 
 
-def _determine_license_suffix_path(path: PathLike) -> Path:
+def _determine_license_suffix_path(path: StrPath) -> Path:
     """Given a path FILE or FILE.license, return FILE.license."""
     path = Path(path)
     if path.suffix == ".license":
         return path
     return Path(f"{path}.license")
 
 
-def _copyright_from_dep5(path: PathLike, dep5_copyright: Copyright) -> SpdxInfo:
+def _copyright_from_dep5(path: StrPath, dep5_copyright: Copyright) -> ReuseInfo:
     """Find the reuse information of *path* in the dep5 Copyright object."""
     result = dep5_copyright.find_files_paragraph(Path(path).as_posix())
 
     if result is None:
-        return SpdxInfo(set(), set())
+        return ReuseInfo()
 
-    return SpdxInfo(
-        set(map(_LICENSING.parse, [result.license.synopsis])),
-        set(map(str.strip, result.copyright.splitlines())),
+    return ReuseInfo(
+        spdx_expressions=set(
+            map(_LICENSING.parse, [result.license.synopsis])  # type: ignore
+        ),
+        copyright_lines=set(
+            map(str.strip, result.copyright.splitlines())  # type: ignore
+        ),
+        source_type=SourceType.DEP5_FILE,
     )
 
 
 def _parse_copyright_year(year: str) -> list:
     """Parse copyright years and return list."""
     if not year:
         ret = []
     if re.match(r"\d{4}$", year):
         ret = [int(year)]
-    if re.match(r"\d{4} - \d{4}$", year):
+    if re.match(r"\d{4} ?- ?\d{4}$", year):
         ret = [int(year[:4]), int(year[-4:])]
     return ret
 
 
+def _contains_snippet(binary_file: BinaryIO) -> bool:
+    """Check if a file seems to contain a SPDX snippet"""
+    # Assumes that if SPDX_SNIPPET_INDICATOR (SPDX-SnippetBegin) is found in a
+    # file, the file contains a snippet
+    content = binary_file.read()
+    if SPDX_SNIPPET_INDICATOR in content:
+        return True
+    return False
+
+
 def merge_copyright_lines(copyright_lines: Set[str]) -> Set[str]:
     """Parse all copyright lines and merge identical statements making years
     into a range.
     If a same statement uses multiple prefixes, use only the most frequent one.
     """
+    # pylint: disable=too-many-locals
+    # TODO: Rewrite this function. It's a bit of a mess.
     copyright_in = []
     for line in copyright_lines:
         for pattern in _COPYRIGHT_PATTERNS:
             match = pattern.search(line)
             if match is not None:
                 copyright_in.append(
                     {
@@ -239,57 +280,62 @@
                         "year": _parse_copyright_year(
                             match.groupdict()["year"]
                         ),
                         "prefix": match.groupdict()["prefix"],
                     }
                 )
 
-    copyright_out = []
-    for statement in {item["statement"] for item in copyright_in}:
+    copyright_out = set()
+    for line_info in copyright_in:
+        statement = str(line_info["statement"])
         copyright_list = [
             item for item in copyright_in if item["statement"] == statement
         ]
-        prefixes = [item["prefix"] for item in copyright_list]
 
         # Get the style of the most common prefix
-        prefix = max(set(prefixes), key=prefixes.count)
+        prefix = str(
+            Counter([item["prefix"] for item in copyright_list]).most_common(1)[
+                0
+            ][0]
+        )
         style = "spdx"
-        # pylint: disable=consider-using-dict-items
-        for sty in _COPYRIGHT_STYLES:
-            if prefix == _COPYRIGHT_STYLES[sty]:
-                style = sty
+        for key, value in _COPYRIGHT_STYLES.items():
+            if prefix == value:
+                style = key
                 break
 
         # get year range if any
-        years = []
+        years: List[str] = []
         for copy in copyright_list:
             years += copy["year"]
 
-        if len(years) == 0:
-            year = None
-        elif min(years) == max(years):
+        year: Optional[str] = None
+        if min(years) == max(years):
             year = min(years)
         else:
             year = f"{min(years)} - {max(years)}"
 
-        copyright_out.append(make_copyright_line(statement, year, style))
+        copyright_out.add(make_copyright_line(statement, year, style))
     return copyright_out
 
 
-def extract_spdx_info(text: str) -> SpdxInfo:
-    """Extract SPDX information from comments in a string.
+def extract_reuse_info(text: str) -> ReuseInfo:
+    """Extract REUSE information from comments in a string.
 
     :raises ExpressionError: if an SPDX expression could not be parsed
     :raises ParseError: if an SPDX expression could not be parsed
     """
     text = filter_ignore_block(text)
-    expression_matches = set(find_license_identifiers(text))
+    spdx_tags: Dict[str, Set[str]] = {}
+    for tag, pattern in _SPDX_TAGS.items():
+        spdx_tags[tag] = set(find_spdx_tag(text, pattern))
+    # License expressions and copyright matches are special cases.
     expressions = set()
     copyright_matches = set()
-    for expression in expression_matches:
+    for expression in spdx_tags.pop("spdx_expressions"):
         try:
             expressions.add(_LICENSING.parse(expression))
         except (ExpressionError, ParseError):
             _LOGGER.error(
                 _("Could not parse '{expression}'").format(
                     expression=expression
                 )
@@ -298,37 +344,42 @@
     for line in text.splitlines():
         for pattern in _COPYRIGHT_PATTERNS:
             match = pattern.search(line)
             if match is not None:
                 copyright_matches.add(match.groupdict()["copyright"].strip())
                 break
 
-    return SpdxInfo(expressions, copyright_matches)
+    return ReuseInfo(
+        spdx_expressions=expressions,
+        copyright_lines=copyright_matches,
+        **spdx_tags,  # type: ignore
+    )
 
 
-def find_license_identifiers(text: str) -> Iterator[str]:
-    """Extract all the license identifiers matching the IDENTIFIER_PATTERN
-    regex, taking care of stripping extraneous whitespace of formatting."""
-    for prefix, identifier in _IDENTIFIER_PATTERN.findall(text):
-        prefix, identifier = prefix.strip(), identifier.strip()
+def find_spdx_tag(text: str, pattern: re.Pattern) -> Iterator[str]:
+    """Extract all the values in *text* matching *pattern*'s regex, taking care
+    of stripping extraneous whitespace of formatting.
+    """
+    for prefix, value in pattern.findall(text):
+        prefix, value = prefix.strip(), value.strip()
 
         # Some comment headers have ASCII art to "frame" the comment, like this:
         #
         # /***********************\
         # |*  This is a comment  *|
         # \***********************/
         #
         # To ensure we parse them correctly, if the line ends with the inverse
         # of the comment prefix, we strip that suffix. See #343 for a real
         # world example of a project doing this (LLVM).
         suffix = prefix[::-1]
-        if suffix and identifier.endswith(suffix):
-            identifier = identifier[: -len(suffix)]
+        if suffix and value.endswith(suffix):
+            value = value[: -len(suffix)]
 
-        yield identifier.strip()
+        yield value.strip()
 
 
 def filter_ignore_block(text: str) -> str:
     """Filter out blocks beginning with REUSE_IGNORE_START and ending with
     REUSE_IGNORE_END to remove lines that should not be treated as copyright and
     licensing information.
     """
@@ -347,18 +398,18 @@
     rest = text[ignore_start + len(REUSE_IGNORE_START) :]
     if REUSE_IGNORE_END in rest:
         ignore_end = rest.index(REUSE_IGNORE_END) + len(REUSE_IGNORE_END)
         return text[:ignore_start] + filter_ignore_block(rest[ignore_end:])
     return text[:ignore_start]
 
 
-def contains_spdx_info(text: str) -> bool:
-    """The text contains SPDX info."""
+def contains_reuse_info(text: str) -> bool:
+    """The text contains REUSE info."""
     try:
-        return any(extract_spdx_info(text))
+        return bool(extract_reuse_info(text))
     except (ExpressionError, ParseError):
         return False
 
 
 def make_copyright_line(
     statement: str, year: Optional[str] = None, copyright_style: str = "spdx"
 ) -> str:
@@ -367,77 +418,82 @@
     """
     if "\n" in statement:
         raise RuntimeError(f"Unexpected newline in '{statement}'")
 
     copyright_prefix = _COPYRIGHT_STYLES.get(copyright_style)
     if copyright_prefix is None:
         raise RuntimeError(
-            "Unexpected copyright style: Need 'spdx', 'spdx-symbol', 'string', "
-            "'string-c', 'string-symbol' or 'symbol'"
+            "Unexpected copyright style: Need 'spdx', 'spdx-c', "
+            "'spdx-symbol', 'string', 'string-c', "
+            "'string-symbol', or 'symbol'"
         )
 
     for pattern in _COPYRIGHT_PATTERNS:
         match = pattern.search(statement)
         if match is not None:
             return statement
     if year is not None:
         return f"{copyright_prefix} {year} {statement}"
     return f"{copyright_prefix} {statement}"
 
 
-def _checksum(path: PathLike) -> str:
+def _checksum(path: StrPath) -> str:
     path = Path(path)
 
     file_sha1 = sha1()
     with path.open("rb") as fp:
         for chunk in iter(lambda: fp.read(128 * file_sha1.block_size), b""):
             file_sha1.update(chunk)
 
     return file_sha1.hexdigest()
 
 
 class PathType:
     """Factory for creating Paths"""
 
-    def __init__(self, mode="r", force_file=False, force_directory=False):
+    def __init__(
+        self,
+        mode: str = "r",
+        force_file: bool = False,
+        force_directory: bool = False,
+    ):
         if mode in ("r", "r+", "w"):
             self._mode = mode
         else:
             raise ValueError(f"mode='{mode}' is not valid")
         self._force_file = force_file
         self._force_directory = force_directory
         if self._force_file and self._force_directory:
             raise ValueError(
                 "'force_file' and 'force_directory' cannot both be True"
             )
 
-    def _check_read(self, path):
+    def _check_read(self, path: Path) -> None:
         if path.exists() and os.access(path, os.R_OK):
             if self._force_file and not path.is_file():
                 raise ArgumentTypeError(_("'{}' is not a file").format(path))
             if self._force_directory and not path.is_dir():
                 raise ArgumentTypeError(
                     _("'{}' is not a directory").format(path)
                 )
             return
         raise ArgumentTypeError(_("can't open '{}'").format(path))
 
-    def _check_write(self, path):
-        # pylint: disable=no-self-use
+    def _check_write(self, path: Path) -> None:
         if path.is_dir():
             raise ArgumentTypeError(
                 _("can't write to directory '{}'").format(path)
             )
         if path.exists() and os.access(path, os.W_OK):
             return
         if not path.exists() and os.access(path.parent, os.W_OK):
             return
         raise ArgumentTypeError(_("can't write to '{}'").format(path))
 
-    def __call__(self, string):
+    def __call__(self, string: str) -> Path:
         path = Path(string)
 
         try:
             if self._mode in ("r", "r+"):
                 self._check_read(path)
             if self._mode in ("w", "r+"):
                 self._check_write(path)
@@ -456,30 +512,32 @@
         raise ArgumentTypeError(
             _("'{}' is not a valid SPDX expression, aborting").format(text)
         ) from error
 
 
 def similar_spdx_identifiers(identifier: str) -> List[str]:
     """Given an incorrect SPDX identifier, return a list of similar ones."""
-    suggestions = []
+    suggestions: List[str] = []
     if identifier in ALL_NON_DEPRECATED_MAP:
         return suggestions
 
     for valid_identifier in ALL_NON_DEPRECATED_MAP:
         distance = SequenceMatcher(
             a=identifier.lower(), b=valid_identifier[: len(identifier)].lower()
         ).ratio()
         if distance > 0.75:
             suggestions.append(valid_identifier)
     suggestions = sorted(suggestions)
 
     return suggestions
 
 
-def print_incorrect_spdx_identifier(identifier: str, out=sys.stdout) -> None:
+def print_incorrect_spdx_identifier(
+    identifier: str, out: IO[str] = sys.stdout
+) -> None:
     """Print out that *identifier* is not valid, and follow up with some
     suggestions.
     """
     out.write(
         _("'{}' is not a valid SPDX License Identifier.").format(identifier)
     )
     out.write("\n")
```

### Comparing `reuse-1.1.2/src/reuse/download.py` & `reuse-2.0.0/src/reuse/download.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # SPDX-FileCopyrightText: 2019 Free Software Foundation Europe e.V. <https://fsfe.org>
+# SPDX-FileCopyrightText: 2023 Nico Rikken <nico.rikken@fsfe.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Functions for downloading license files from spdx/license-data-list."""
 
 import errno
 import logging
 import sys
 import urllib.request
+from argparse import ArgumentParser, Namespace
 from gettext import gettext as _
-from os import PathLike
 from pathlib import Path
+from typing import IO
 from urllib.error import URLError
 from urllib.parse import urljoin
 
 from ._licenses import ALL_NON_DEPRECATED_MAP
 from ._util import (
     PathType,
+    StrPath,
     find_licenses_directory,
     print_incorrect_spdx_identifier,
 )
 from .project import Project
 from .report import ProjectReport
 
 _LOGGER = logging.getLogger(__name__)
@@ -36,27 +39,28 @@
 
     :param spdx_identifier: SPDX identifier of the license.
     :raises URLError: if the license could not be downloaded.
     :return: The license text.
     """
     # This is fairly naive, but I can't see anything wrong with it.
     url = urljoin(_SPDX_REPOSITORY_BASE_URL, "".join((spdx_identifier, ".txt")))
+    _LOGGER.debug("downloading license from '%s'", url)
     # TODO: Cache result?
     with urllib.request.urlopen(url) as response:
         if response.getcode() == 200:
             return response.read().decode("utf-8")
     raise URLError("Status code was not 200")
 
 
-def _path_to_license_file(spdx_identifier: str, root: PathLike) -> Path:
+def _path_to_license_file(spdx_identifier: str, root: StrPath) -> Path:
     licenses_path = find_licenses_directory(root=root)
     return licenses_path / "".join((spdx_identifier, ".txt"))
 
 
-def put_license_in_file(spdx_identifier: str, destination: PathLike) -> None:
+def put_license_in_file(spdx_identifier: str, destination: StrPath) -> None:
     """Download a license and put it in the destination file.
 
     This function exists solely for convenience.
 
     :param spdx_identifier: SPDX License Identifier of the license.
     :param destination: Where to put the license.
     :raises URLError: if the license could not be downloaded.
@@ -71,15 +75,15 @@
 
     text = download_license(spdx_identifier)
     with destination.open("w", encoding="utf-8") as fp:
         fp.write(header)
         fp.write(text)
 
 
-def add_arguments(parser) -> None:
+def add_arguments(parser: ArgumentParser) -> None:
     """Add arguments to parser."""
     parser.add_argument(
         "license",
         action="store",
         nargs="*",
         help=_("SPDX License Identifier of license"),
     )
@@ -89,35 +93,35 @@
         help=_("download all missing licenses detected in the project"),
     )
     parser.add_argument(
         "--output", "-o", dest="file", action="store", type=PathType("w")
     )
 
 
-def run(args, project: Project, out=sys.stdout) -> int:
+def run(args: Namespace, project: Project, out: IO[str] = sys.stdout) -> int:
     """Download license and place it in the LICENSES/ directory."""
 
-    def _already_exists(path: PathLike):
+    def _already_exists(path: StrPath) -> None:
         out.write(
             _("Error: {spdx_identifier} already exists.").format(
                 spdx_identifier=path
             )
         )
         out.write("\n")
 
-    def _could_not_download(identifier: str):
+    def _could_not_download(identifier: str) -> None:
         out.write(_("Error: Failed to download license."))
         out.write(" ")
         if identifier not in ALL_NON_DEPRECATED_MAP:
             print_incorrect_spdx_identifier(identifier, out=out)
         else:
             out.write(_("Is your internet connection working?"))
         out.write("\n")
 
-    def _successfully_downloaded(destination: PathLike):
+    def _successfully_downloaded(destination: StrPath) -> None:
         out.write(
             _("Successfully downloaded {spdx_identifier}.").format(
                 spdx_identifier=destination
             )
         )
         out.write("\n")
```

### Comparing `reuse-1.1.2/src/reuse/header.py` & `reuse-2.0.0/src/reuse/header.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,50 +17,60 @@
 
 import argparse
 import datetime
 import logging
 import os
 import re
 import sys
-from argparse import ArgumentParser
+from argparse import ArgumentParser, Namespace
 from gettext import gettext as _
-from os import PathLike
 from pathlib import Path
-from typing import Iterable, List, NamedTuple, Optional, Sequence, Tuple
+from typing import (
+    IO,
+    Iterable,
+    NamedTuple,
+    Optional,
+    Sequence,
+    Set,
+    Tuple,
+    Type,
+    cast,
+)
 
 from binaryornot.check import is_binary
 from boolean.boolean import ParseError
 from jinja2 import Environment, FileSystemLoader, PackageLoader, Template
 from jinja2.exceptions import TemplateNotFound
 from license_expression import ExpressionError
 
-from . import SpdxInfo
-from ._comment import (
-    EXTENSION_COMMENT_STYLE_MAP_LOWERCASE,
-    FILENAME_COMMENT_STYLE_MAP_LOWERCASE,
-    NAME_STYLE_MAP,
-    CommentCreateError,
-    CommentParseError,
-    CommentStyle,
-    EmptyCommentStyle,
-    PythonCommentStyle,
-    UncommentableCommentStyle,
-)
+from . import ReuseInfo
 from ._util import (
     _COPYRIGHT_STYLES,
     PathType,
+    StrPath,
     _determine_license_path,
     _determine_license_suffix_path,
-    contains_spdx_info,
+    contains_reuse_info,
     detect_line_endings,
-    extract_spdx_info,
+    extract_reuse_info,
     make_copyright_line,
     merge_copyright_lines,
     spdx_identifier,
 )
+from .comment import (
+    EXTENSION_COMMENT_STYLE_MAP_LOWERCASE,
+    FILENAME_COMMENT_STYLE_MAP_LOWERCASE,
+    NAME_STYLE_MAP,
+    CommentCreateError,
+    CommentParseError,
+    CommentStyle,
+    EmptyCommentStyle,
+    PythonCommentStyle,
+    UncommentableCommentStyle,
+)
 from .project import Project
 
 _LOGGER = logging.getLogger(__name__)
 
 _ENV = Environment(loader=PackageLoader("reuse", "templates"), trim_blocks=True)
 DEFAULT_TEMPLATE = _ENV.get_template("default_template.jinja2")
 
@@ -71,119 +81,118 @@
     """Used to split up text in three parts."""
 
     before: str
     middle: str
     after: str
 
 
-class MissingSpdxInfo(Exception):
-    """Some SPDX information is missing from the result."""
+class MissingReuseInfo(Exception):
+    """Some REUSE information is missing from the result."""
 
 
 # TODO: Add a template here maybe.
 def _create_new_header(
-    spdx_info: SpdxInfo,
-    template: Template = None,
+    reuse_info: ReuseInfo,
+    template: Optional[Template] = None,
     template_is_commented: bool = False,
-    style: CommentStyle = None,
+    style: Optional[Type[CommentStyle]] = None,
     force_multi: bool = False,
 ) -> str:
     """Format a new header from scratch.
 
     :raises CommentCreateError: if a comment could not be created.
-    :raises MissingSpdxInfo: if the generated comment is missing SPDX
+    :raises MissingReuseInfo: if the generated comment is missing SPDX
         information.
     """
     if template is None:
         template = DEFAULT_TEMPLATE
     if style is None:
-        style = PythonCommentStyle
+        style = cast(Type[CommentStyle], PythonCommentStyle)
 
     rendered = template.render(
-        copyright_lines=sorted(spdx_info.copyright_lines),
-        spdx_expressions=sorted(map(str, spdx_info.spdx_expressions)),
+        copyright_lines=sorted(reuse_info.copyright_lines),
+        contributor_lines=sorted(reuse_info.contributor_lines),
+        spdx_expressions=sorted(map(str, reuse_info.spdx_expressions)),
     ).strip("\n")
 
     if template_is_commented:
         result = rendered
     else:
         result = style.create_comment(rendered, force_multi=force_multi).strip(
             "\n"
         )
 
-    # Verify that the result contains all SpdxInfo.
-    new_spdx_info = extract_spdx_info(result)
+    # Verify that the result contains all ReuseInfo.
+    new_reuse_info = extract_reuse_info(result)
     if (
-        spdx_info.copyright_lines != new_spdx_info.copyright_lines
-        and spdx_info.spdx_expressions != new_spdx_info.spdx_expressions
+        reuse_info.copyright_lines != new_reuse_info.copyright_lines
+        and reuse_info.spdx_expressions != new_reuse_info.spdx_expressions
     ):
         _LOGGER.debug(
             _(
                 "generated comment is missing copyright lines or license"
                 " expressions"
             )
         )
         _LOGGER.debug(result)
-        raise MissingSpdxInfo()
+        raise MissingReuseInfo()
 
     return result
 
 
 # pylint: disable=too-many-arguments
 def create_header(
-    spdx_info: SpdxInfo,
-    header: str = None,
-    template: Template = None,
+    reuse_info: ReuseInfo,
+    header: Optional[str] = None,
+    template: Optional[Template] = None,
     template_is_commented: bool = False,
-    style: CommentStyle = None,
+    style: Optional[Type[CommentStyle]] = None,
     force_multi: bool = False,
     merge_copyrights: bool = False,
 ) -> str:
-    """Create a header containing *spdx_info*. *header* is an optional argument
-    containing a header which should be modified to include *spdx_info*. If
+    """Create a header containing *reuse_info*. *header* is an optional argument
+    containing a header which should be modified to include *reuse_info*. If
     *header* is not given, a brand new header is created.
 
     *template*, *template_is_commented*, and *style* determine what the header
     will look like, and whether it will be commented or not.
 
     :raises CommentCreateError: if a comment could not be created.
-    :raises MissingSpdxInfo: if the generated comment is missing SPDX
+    :raises MissingReuseInfo: if the generated comment is missing SPDX
         information.
     """
     if template is None:
         template = DEFAULT_TEMPLATE
     if style is None:
         style = PythonCommentStyle
 
     new_header = ""
     if header:
         try:
-            existing_spdx = extract_spdx_info(header)
+            existing_spdx = extract_reuse_info(header)
         except (ExpressionError, ParseError) as err:
             raise CommentCreateError(
                 "existing header contains an erroneous SPDX expression"
             ) from err
 
         if merge_copyrights:
             spdx_copyrights = merge_copyright_lines(
-                spdx_info.copyright_lines.union(existing_spdx.copyright_lines),
+                reuse_info.copyright_lines.union(existing_spdx.copyright_lines),
             )
         else:
-            spdx_copyrights = spdx_info.copyright_lines.union(
+            spdx_copyrights = reuse_info.copyright_lines.union(
                 existing_spdx.copyright_lines
             )
 
         # TODO: This behaviour does not match the docstring.
-        spdx_info = SpdxInfo(
-            spdx_info.spdx_expressions.union(existing_spdx.spdx_expressions),
-            spdx_copyrights,
-        )
+        reuse_info = existing_spdx | reuse_info
+        reuse_info = reuse_info.copy(copyright_lines=spdx_copyrights)
 
     new_header += _create_new_header(
-        spdx_info,
+        reuse_info,
         template=template,
         template_is_commented=template_is_commented,
         style=style,
         force_multi=force_multi,
     )
     return new_header
 
@@ -200,37 +209,37 @@
         else:
             break
 
     return indices
 
 
 def _find_first_spdx_comment(
-    text: str, style: CommentStyle = None
+    text: str, style: Optional[Type[CommentStyle]] = None
 ) -> _TextSections:
     """Find the first SPDX comment in the file. Return a tuple with everything
     preceding the comment, the comment itself, and everything following it.
 
-    :raises MissingSpdxInfo: if no SPDX info can be found in any comment
+    :raises MissingReuseInfo: if no REUSE info can be found in any comment
     """
     if style is None:
         style = PythonCommentStyle
 
     indices = _indices_of_newlines(text)
 
     for index in indices:
         try:
             comment = style.comment_at_first_character(text[index:])
         except CommentParseError:
             continue
-        if contains_spdx_info(comment):
+        if contains_reuse_info(comment):
             return _TextSections(
                 text[:index], comment + "\n", text[index + len(comment) + 1 :]
             )
 
-    raise MissingSpdxInfo()
+    raise MissingReuseInfo()
 
 
 def _extract_shebang(prefix: str, text: str) -> Tuple[str, str]:
     """Remove all lines that start with the shebang prefix from *text*. Return a
     tuple of (shebang, reduced_text).
     """
     shebang_lines = []
@@ -243,46 +252,46 @@
             break
     return (shebang, text)
 
 
 # pylint: disable=too-many-arguments
 def find_and_replace_header(
     text: str,
-    spdx_info: SpdxInfo,
-    template: Template = None,
+    reuse_info: ReuseInfo,
+    template: Optional[Template] = None,
     template_is_commented: bool = False,
-    style: CommentStyle = None,
+    style: Optional[Type[CommentStyle]] = None,
     force_multi: bool = False,
     merge_copyrights: bool = False,
 ) -> str:
     """Find the first SPDX comment block in *text*. That comment block is
-    replaced by a new comment block containing *spdx_info*. It is formatted as
+    replaced by a new comment block containing *reuse_info*. It is formatted as
     according to *template*. The template is normally uncommented, but if it is
     already commented, *template_is_commented* should be :const:`True`.
 
     If both *style* and *template_is_commented* are provided, *style* is only
     used to find the header comment.
 
-    If the comment block already contained some SPDX information, that
-    information is merged into *spdx_info*.
+    If the comment block already contained some REUSE information, that
+    information is merged into *reuse_info*.
 
     If no header exists, one is simply created.
 
     *text* is returned with a new header.
 
     :raises CommentCreateError: if a comment could not be created.
-    :raises MissingSpdxInfo: if the generated comment is missing SPDX
+    :raises MissingReuseInfo: if the generated comment is missing SPDX
         information.
     """
     if style is None:
         style = PythonCommentStyle
 
     try:
         before, header, after = _find_first_spdx_comment(text, style=style)
-    except MissingSpdxInfo:
+    except MissingReuseInfo:
         before, header, after = "", "", text
 
     # Workaround. EmptyCommentStyle should always be completely replaced.
     if style is EmptyCommentStyle:
         after = ""
 
     _LOGGER.debug(f"before = {repr(before)}")
@@ -300,15 +309,15 @@
             elif after.startswith(shebang) and not any((before, header)):
                 before, after = _extract_shebang(shebang, after)
             else:
                 continue
             break
 
     header = create_header(
-        spdx_info,
+        reuse_info,
         header,
         template=template,
         template_is_commented=template_is_commented,
         style=style,
         force_multi=force_multi,
         merge_copyrights=merge_copyrights,
     )
@@ -320,24 +329,24 @@
         new_text = f"{new_text}\n{after.lstrip()}"
     return new_text
 
 
 # pylint: disable=too-many-arguments
 def add_new_header(
     text: str,
-    spdx_info: SpdxInfo,
-    template: Template = None,
+    reuse_info: ReuseInfo,
+    template: Optional[Template] = None,
     template_is_commented: bool = False,
-    style: CommentStyle = None,
+    style: Optional[Type[CommentStyle]] = None,
     force_multi: bool = False,
     merge_copyrights: bool = False,
 ) -> str:
     """Add a new header at the very top of *text*, similar to
     find_and_replace_header. But in this function, do not replace any headers or
-    search for any existing SPDX information.
+    search for any existing REUSE information.
 
     :raises CommentCreateError: if a comment could not be created.
     """
     if style is None:
         style = PythonCommentStyle
 
     shebang = ""
@@ -345,15 +354,15 @@
     if style.SHEBANGS:
         for shebang_prefix in style.SHEBANGS:
             if text.startswith(shebang_prefix):
                 shebang, text = _extract_shebang(shebang_prefix, text)
                 break
 
     header = create_header(
-        spdx_info,
+        reuse_info,
         None,
         template=template,
         template_is_commented=template_is_commented,
         style=style,
         force_multi=force_multi,
         merge_copyrights=merge_copyrights,
     )
@@ -362,36 +371,40 @@
     if shebang.strip():
         new_text = f"{shebang.rstrip()}\n\n{new_text}"
     if text.strip():
         new_text = f"{new_text}\n{text.lstrip()}"
     return new_text
 
 
-def _get_comment_style(path: Path) -> Optional[CommentStyle]:
+def _get_comment_style(path: StrPath) -> Optional[Type[CommentStyle]]:
     """Return value of CommentStyle detected for *path* or None."""
+    path = Path(path)
     style = FILENAME_COMMENT_STYLE_MAP_LOWERCASE.get(path.name.lower())
     if style is None:
-        style = EXTENSION_COMMENT_STYLE_MAP_LOWERCASE.get(path.suffix.lower())
+        style = cast(
+            Optional[Type[CommentStyle]],
+            EXTENSION_COMMENT_STYLE_MAP_LOWERCASE.get(path.suffix.lower()),
+        )
     return style
 
 
 def _is_uncommentable(path: Path) -> bool:
     """Determines if *path* is uncommentable, e.g., the file is a binary or
     registered as an UncommentableCommentStyle.
     """
     is_uncommentable = _get_comment_style(path) == UncommentableCommentStyle
     return is_uncommentable or is_binary(str(path))
 
 
 def _verify_paths_line_handling(
-    paths: List[Path],
+    paths: Iterable[Path],
     parser: ArgumentParser,
     force_single: bool,
     force_multi: bool,
-):
+) -> None:
     """This function aborts the parser when *force_single* or *force_multi* is
     used, but the file type does not support that type of comment style.
     """
     for path in paths:
         style = _get_comment_style(path)
         if style is None:
             continue
@@ -407,15 +420,17 @@
                 _(
                     "'{path}' does not support multi-line comments, please"
                     " do not use --multi-line"
                 ).format(path=path)
             )
 
 
-def _verify_paths_comment_style(paths: List[Path], parser: ArgumentParser):
+def _verify_paths_comment_style(
+    paths: Iterable[Path], parser: ArgumentParser
+) -> None:
     unrecognised_files = []
 
     for path in paths:
         style = _get_comment_style(path)
         not_uncommentable = not _is_uncommentable(path)
 
         # TODO: This check is duplicated.
@@ -456,114 +471,116 @@
             return env.get_template(item)
         except TemplateNotFound:
             pass
     raise TemplateNotFound(name)
 
 
 def _add_header_to_file(
-    path: PathLike,
-    spdx_info: SpdxInfo,
-    template: Template,
+    path: StrPath,
+    reuse_info: ReuseInfo,
+    template: Optional[Template],
     template_is_commented: bool,
     style: Optional[str],
     force_multi: bool = False,
     skip_existing: bool = False,
     merge_copyrights: bool = False,
     replace: bool = True,
-    out=sys.stdout,
+    out: IO[str] = sys.stdout,
 ) -> int:
     """Helper function."""
-    # pylint: disable=too-many-arguments
+    # pylint: disable=too-many-arguments,too-many-locals
     result = 0
     if style is not None:
-        style = NAME_STYLE_MAP[style]
+        comment_style: Optional[Type[CommentStyle]] = NAME_STYLE_MAP.get(style)
     else:
-        style = _get_comment_style(path)
-        if style is None:
-            out.write(_("Skipped unrecognised file {path}").format(path=path))
-            out.write("\n")
-            return result
+        comment_style = _get_comment_style(path)
+    if comment_style is None:
+        out.write(_("Skipped unrecognised file {path}").format(path=path))
+        out.write("\n")
+        return result
 
-    with path.open("r", encoding="utf-8", newline="") as fp:
+    with open(path, "r", encoding="utf-8", newline="") as fp:
         text = fp.read()
 
     # Ideally, this check is done elsewhere. But that would necessitate reading
     # the file contents before this function is called.
-    if skip_existing and contains_spdx_info(text):
+    if skip_existing and contains_reuse_info(text):
         out.write(
             _(
-                "Skipped file '{path}' already containing SPDX information"
+                "Skipped file '{path}' already containing REUSE information"
             ).format(path=path)
         )
         out.write("\n")
         return result
 
     # Detect and remember line endings for later conversion.
     line_ending = detect_line_endings(text)
     # Normalise line endings.
     text = text.replace(line_ending, "\n")
 
     try:
         if replace:
             output = find_and_replace_header(
                 text,
-                spdx_info,
+                reuse_info,
                 template=template,
                 template_is_commented=template_is_commented,
-                style=style,
+                style=comment_style,
                 force_multi=force_multi,
                 merge_copyrights=merge_copyrights,
             )
         else:
             output = add_new_header(
                 text,
-                spdx_info,
+                reuse_info,
                 template=template,
                 template_is_commented=template_is_commented,
-                style=style,
+                style=comment_style,
                 force_multi=force_multi,
                 merge_copyrights=merge_copyrights,
             )
     except CommentCreateError:
         out.write(
             _("Error: Could not create comment for '{path}'").format(path=path)
         )
         out.write("\n")
         result = 1
-    except MissingSpdxInfo:
+    except MissingReuseInfo:
         out.write(
             _(
                 "Error: Generated comment header for '{path}' is missing"
                 " copyright lines or license expressions. The template is"
                 " probably incorrect. Did not write new header."
             ).format(path=path)
         )
         out.write("\n")
         result = 1
     else:
-        with path.open("w", encoding="utf-8", newline=line_ending) as fp:
+        with open(path, "w", encoding="utf-8", newline=line_ending) as fp:
             fp.write(output)
         # TODO: This may need to be rephrased more elegantly.
         out.write(_("Successfully changed header of {path}").format(path=path))
         out.write("\n")
 
     return result
 
 
-def _verify_write_access(paths: Iterable[PathLike], parser: ArgumentParser):
+def _verify_write_access(
+    paths: Iterable[StrPath], parser: ArgumentParser
+) -> None:
     not_writeable = [
         str(path) for path in paths if not os.access(path, os.W_OK)
     ]
     if not_writeable:
         parser.error(
             _("can't write to '{}'").format("', '".join(not_writeable))
         )
 
 
-def add_arguments(parser) -> None:
+def add_arguments(parser: ArgumentParser) -> None:
     """Add arguments to parser."""
     parser.add_argument(
         "--copyright",
         "-c",
         action="append",
         type=str,
         help=_("copyright statement, repeatable"),
@@ -572,14 +589,20 @@
         "--license",
         "-l",
         action="append",
         type=spdx_identifier,
         help=_("SPDX Identifier, repeatable"),
     )
     parser.add_argument(
+        "--contributor",
+        action="append",
+        type=str,
+        help=_("file contributor, repeatable"),
+    )
+    parser.add_argument(
         "--year",
         "-y",
         action="append",
         type=str,
         help=_("year of copyright statement, optional"),
     )
     parser.add_argument(
@@ -652,32 +675,34 @@
         "--skip-unrecognised",
         action="store_true",
         help=_("skip files with unrecognised comment styles"),
     )
     parser.add_argument(
         "--skip-existing",
         action="store_true",
-        help=_("skip files that already contain SPDX information"),
+        help=_("skip files that already contain REUSE information"),
     )
     parser.add_argument("path", action="store", nargs="+", type=PathType("r"))
 
 
-def run(args, project: Project, out=sys.stdout) -> int:
+def run(args: Namespace, project: Project, out: IO[str] = sys.stdout) -> int:
     """Add headers to files."""
     # pylint: disable=too-many-branches,too-many-locals,too-many-statements
     if "addheader" in args.parser.prog.split():
         _LOGGER.warning(
             _(
                 "'reuse addheader' has been deprecated in favour of"
                 " 'reuse annotate'"
             )
         )
 
-    if not any((args.copyright, args.license)):
-        args.parser.error(_("option --copyright or --license is required"))
+    if not any((args.contributor, args.copyright, args.license)):
+        args.parser.error(
+            _("option --contributor, --copyright or --license is required")
+        )
 
     if args.exclude_year and args.year:
         args.parser.error(
             _("option --exclude-year and --year are mutually exclusive")
         )
 
     if args.single_line and args.multi_line:
@@ -698,15 +723,15 @@
                 "--explicit-license has been deprecated in favour of"
                 " --force-dot-license"
             )
         )
         args.force_dot_license = True
 
     if args.recursive:
-        paths = set()
+        paths: Set[Path] = set()
         all_files = [path.resolve() for path in project.all_files()]
         for path in args.path:
             if path.is_file():
                 paths.add(path)
             else:
                 paths |= {
                     child
@@ -728,52 +753,64 @@
             args.parser,
             force_single=args.single_line,
             force_multi=args.multi_line,
         )
         if not args.skip_unrecognised:
             _verify_paths_comment_style(paths, args.parser)
 
-    template = None
+    template: Optional[Template] = None
     commented = False
     if args.template:
         try:
-            template = _find_template(project, args.template)
+            template = cast(Template, _find_template(project, args.template))
         except TemplateNotFound:
             args.parser.error(
                 _("template {template} could not be found").format(
                     template=args.template
                 )
             )
+            # This code is never reached, but mypy is not aware that
+            # parser.error quits the program.
+            raise
 
-        if ".commented" in Path(template.name).suffixes:
+        if ".commented" in Path(cast(str, template.name)).suffixes:
             commented = True
 
     year = None
     if not args.exclude_year:
         if args.year and len(args.year) > 1:
             year = f"{min(args.year)} - {max(args.year)}"
         elif args.year:
             year = args.year.pop()
         else:
-            year = datetime.date.today().year
+            year = str(datetime.date.today().year)
 
     expressions = set(args.license) if args.license is not None else set()
     copyright_style = (
         args.copyright_style if args.copyright_style is not None else "spdx"
     )
     copyright_lines = (
         {
-            make_copyright_line(x, year=year, copyright_style=copyright_style)
-            for x in args.copyright
+            make_copyright_line(
+                item, year=year, copyright_style=copyright_style
+            )
+            for item in args.copyright
         }
         if args.copyright is not None
         else set()
     )
+    contributors = (
+        set(args.contributor) if args.contributor is not None else set()
+    )
 
-    spdx_info = SpdxInfo(expressions, copyright_lines)
+    reuse_info = ReuseInfo(
+        spdx_expressions=expressions,
+        copyright_lines=copyright_lines,
+        contributor_lines=contributors,
+    )
 
     result = 0
     for path in paths:
         uncommentable = _is_uncommentable(path)
         if uncommentable or args.force_dot_license:
             new_path = _determine_license_suffix_path(path)
             if uncommentable:
@@ -783,15 +820,15 @@
                         " for the header"
                     ).format(path=path, new_path=new_path)
                 )
             path = Path(new_path)
             path.touch()
         result += _add_header_to_file(
             path=path,
-            spdx_info=spdx_info,
+            reuse_info=reuse_info,
             template=template,
             template_is_commented=commented,
             style=args.style,
             force_multi=args.multi_line,
             skip_existing=args.skip_existing,
             merge_copyrights=args.merge_copyrights,
             replace=not args.no_replace,
```

### Comparing `reuse-1.1.2/src/reuse/init.py` & `reuse-2.0.0/src/reuse/init.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 # SPDX-FileCopyrightText: 2019 Free Software Foundation Europe e.V. <https://fsfe.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Functions for REUSE-ifying a project."""
 
 import sys
+from argparse import ArgumentParser, Namespace
 from gettext import gettext as _
 from inspect import cleandoc
 from pathlib import Path
-from typing import List
+from typing import IO, List
 from urllib.error import URLError
 
 from ._licenses import ALL_NON_DEPRECATED_MAP
 from ._util import PathType, print_incorrect_spdx_identifier
 from .download import _path_to_license_file, put_license_in_file
 from .project import Project
 from .vcs import find_root
 
 
-def prompt_licenses(out=sys.stdout) -> List[str]:
+def prompt_licenses(out: IO[str] = sys.stdout) -> List[str]:
     """Prompt the user for a list of licenses."""
     first = _(
         "What license is your project under? "
         "Provide the SPDX License Identifier."
     )
     multi = _(
         "What other license is your project under? "
         "Provide the SPDX License Identifier."
     )
-    licenses = []
+    licenses: List[str] = []
 
     while True:
         if not licenses:
             out.write(first)
         else:
             out.write(multi)
         out.write("\n")
@@ -45,25 +46,29 @@
         if result not in ALL_NON_DEPRECATED_MAP:
             print_incorrect_spdx_identifier(result, out=out)
             out.write("\n\n")
         else:
             licenses.append(result)
 
 
-def add_arguments(parser):
+def add_arguments(parser: ArgumentParser) -> None:
     """Add arguments to parser."""
     parser.add_argument(
         "path",
         action="store",
         nargs="?",
         type=PathType("r", force_directory=True),
     )
 
 
-def run(args, project: Project, out=sys.stdout):
+def run(
+    args: Namespace,
+    project: Project,
+    out: IO[str] = sys.stdout,
+) -> int:
     """List all non-compliant files."""
     # pylint: disable=too-many-statements,unused-argument
     if args.path:
         root = args.path
     else:
         root = find_root()
     if root is None:
```

### Comparing `reuse-1.1.2/src/reuse/project.py` & `reuse-2.0.0/src/reuse/project.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,104 +1,118 @@
 # SPDX-FileCopyrightText: 2017 Free Software Foundation Europe e.V. <https://fsfe.org>
 # SPDX-FileCopyrightText: 2022 Florian Snow <florian@familysnow.net>
+# SPDX-FileCopyrightText: 2023 DB Systel GmbH
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Module that contains the central Project class."""
 
 import contextlib
 import glob
 import logging
 import os
 from gettext import gettext as _
 from pathlib import Path
-from typing import Dict, Iterator, Optional
+from typing import Dict, Iterator, Optional, Union, cast
 
 from boolean.boolean import ParseError
 from debian.copyright import Copyright
 from debian.copyright import Error as DebianError
 from license_expression import ExpressionError
 
 from . import (
     _IGNORE_DIR_PATTERNS,
     _IGNORE_FILE_PATTERNS,
     _IGNORE_MESON_PARENT_DIR_PATTERNS,
     IdentifierNotFound,
-    SpdxInfo,
+    ReuseInfo,
+    SourceType,
 )
 from ._licenses import EXCEPTION_MAP, LICENSE_MAP
 from ._util import (
     _HEADER_BYTES,
     GIT_EXE,
     HG_EXE,
-    PathLike,
+    StrPath,
+    _contains_snippet,
     _copyright_from_dep5,
     _determine_license_path,
     decoded_text_from_binary,
-    extract_spdx_info,
+    extract_reuse_info,
+)
+from .vcs import (
+    VCSStrategy,
+    VCSStrategyGit,
+    VCSStrategyHg,
+    VCSStrategyNone,
+    find_root,
 )
-from .vcs import VCSStrategyGit, VCSStrategyHg, VCSStrategyNone, find_root
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class Project:
     """Simple object that holds the project's root, which is necessary for many
     interactions.
     """
 
     def __init__(
         self,
-        root: PathLike,
+        root: StrPath,
         include_submodules: bool = False,
         include_meson_subprojects: bool = False,
     ):
         self._root = Path(root)
         if not self._root.is_dir():
             raise NotADirectoryError(f"{self._root} is no valid path")
 
         if GIT_EXE and VCSStrategyGit.in_repo(self._root):
-            self.vcs_strategy = VCSStrategyGit(self)
+            self.vcs_strategy: VCSStrategy = VCSStrategyGit(self)
         elif HG_EXE and VCSStrategyHg.in_repo(self._root):
             self.vcs_strategy = VCSStrategyHg(self)
         else:
-            _LOGGER.warning(_("could not find supported VCS"))
+            _LOGGER.info(
+                _(
+                    "project is not a VCS repository or required VCS software"
+                    " is not installed"
+                )
+            )
             self.vcs_strategy = VCSStrategyNone(self)
 
-        self.licenses_without_extension = {}
+        self.licenses_without_extension: Dict[str, Path] = {}
 
         self.license_map = LICENSE_MAP.copy()
         # TODO: Is this correct?
         self.license_map.update(EXCEPTION_MAP)
         self.licenses = self._licenses()
         # Use '0' as None, because None is a valid value...
-        self._copyright_val = 0
+        self._copyright_val: Optional[Union[int, Copyright]] = 0
         self.include_submodules = include_submodules
 
         meson_build_path = self._root / "meson.build"
         uses_meson = meson_build_path.is_file()
         self.include_meson_subprojects = (
             include_meson_subprojects and uses_meson
         )
 
-    def all_files(self, directory: PathLike = None) -> Iterator[Path]:
+    def all_files(self, directory: Optional[StrPath] = None) -> Iterator[Path]:
         """Yield all files in *directory* and its subdirectories.
 
         The files that are not yielded are:
 
         - Files ignored by VCS (e.g., see .gitignore)
 
         - Files/directories matching IGNORE_*_PATTERNS.
         """
         if directory is None:
             directory = self.root
         directory = Path(directory)
 
-        for root, dirs, files in os.walk(directory):
-            root = Path(root)
+        for root_str, dirs, files in os.walk(directory):
+            root = Path(root_str)
             _LOGGER.debug("currently walking in '%s'", root)
 
             # Don't walk ignored directories
             for dir_ in list(dirs):
                 the_dir = root / dir_
                 if self._is_path_ignored(the_dir):
                     _LOGGER.debug("ignoring '%s'", the_dir)
@@ -129,59 +143,110 @@
                     if the_file.stat().st_size == 0:
                         _LOGGER.debug("skipping 0-sized file '%s'", the_file)
                         continue
 
                 _LOGGER.debug("yielding '%s'", the_file)
                 yield the_file
 
-    def spdx_info_of(self, path: PathLike) -> SpdxInfo:
-        """Return SPDX info of *path*.
+    def reuse_info_of(self, path: StrPath) -> ReuseInfo:
+        """Return REUSE info of *path*.
+
+        This function will return any REUSE information that it can find, both
+        from within the file, the .license file and from the .reuse/dep5 file.
 
-        This function will return any SPDX information that it can find, both
-        from within the file and from the .reuse/dep5 file.
+        It also returns a single primary source path of the license/copyright
+        information, where 'primary' means '.license file' > 'header' > 'dep5'
         """
+        original_path = path
         path = _determine_license_path(path)
-        _LOGGER.debug(f"searching '{path}' for SPDX information")
+        dep5_path: Optional[str] = None
+        source_path = ""
+        source_type = None
+
+        _LOGGER.debug(f"searching '{path}' for REUSE information")
+
+        # This means that only one 'source' of licensing/copyright information
+        # is captured in ReuseInfo
+        dep5_result = ReuseInfo()
+        file_result = ReuseInfo()
 
-        dep5_result = SpdxInfo(set(), set())
-        file_result = SpdxInfo(set(), set())
-
-        # Search the .reuse/dep5 file for SPDX information.
+        # Search the .reuse/dep5 file for REUSE information.
         if self._copyright:
             dep5_result = _copyright_from_dep5(
                 self.relative_from_root(path), self._copyright
             )
-            if any(dep5_result):
+            if dep5_result.contains_copyright_or_licensing():
                 _LOGGER.info(
                     _("'{path}' covered by .reuse/dep5").format(path=path)
                 )
+                source_path = str(self.root / ".reuse/dep5")
+                dep5_path = source_path
 
-        # Search the file for SPDX information.
+        # Search the file for REUSE information.
         with path.open("rb") as fp:
             try:
-                file_result = extract_spdx_info(
-                    decoded_text_from_binary(fp, size=_HEADER_BYTES)
+                # Completely read the file once to search for possible snippets
+                if _contains_snippet(fp):
+                    _LOGGER.debug(f"'{path}' seems to contain a SPDX Snippet")
+                    read_limit = None
+                else:
+                    read_limit = _HEADER_BYTES
+                # Reset read position
+                fp.seek(0)
+                # Scan the file for REUSE info, possible limiting the read
+                # length
+                file_result = extract_reuse_info(
+                    decoded_text_from_binary(fp, size=read_limit)
                 )
+                if file_result:
+                    source_path = str(path)
+                    if path.suffix == ".license":
+                        source_type = SourceType.DOT_LICENSE_FILE
+                    else:
+                        source_type = SourceType.FILE_HEADER
+
             except (ExpressionError, ParseError):
                 _LOGGER.error(
                     _(
                         "'{path}' holds an SPDX expression that cannot be"
                         " parsed, skipping the file"
                     ).format(path=path)
                 )
 
-        return SpdxInfo(
-            dep5_result.spdx_expressions.union(file_result.spdx_expressions),
-            dep5_result.copyright_lines.union(file_result.copyright_lines),
+        # There is both information in a .dep5 file and in the file header
+        if (
+            dep5_result.contains_copyright_or_licensing()
+            and file_result.contains_copyright_or_licensing()
+        ):
+            _LOGGER.warning(
+                _(
+                    "Copyright and licensing information for '{original_path}'"
+                    " have been found in '{path}' and the DEP5 file located at"
+                    " '{dep5_path}'. The information in the DEP5 file has been"
+                    " overridden. Please ensure that this is correct."
+                ).format(
+                    original_path=original_path, path=path, dep5_path=dep5_path
+                )
+            )
+        # Information is only found in a DEP5 file
+        elif (
+            dep5_result.contains_copyright_or_licensing()
+            and not file_result.contains_copyright_or_licensing()
+        ):
+            return dep5_result.copy(source_path=source_path)
+        # There is a file header or a .license file
+        return file_result.copy(
+            source_path=source_path, source_type=source_type
         )
 
-    def relative_from_root(self, path: Path) -> Path:
+    def relative_from_root(self, path: StrPath) -> Path:
         """If the project root is /tmp/project, and *path* is
         /tmp/project/src/file, then return src/file.
         """
+        path = Path(path)
         try:
             return path.relative_to(self.root)
         except ValueError:
             return Path(os.path.relpath(path, start=self.root))
 
     def _is_path_ignored(self, path: Path) -> bool:
         """Is *path* ignored by some mechanism?"""
@@ -241,25 +306,25 @@
             except UnicodeError:
                 _LOGGER.exception(_(".reuse/dep5 could not be parsed as utf-8"))
 
             # This check is a bit redundant, but otherwise I'd have to repeat
             # this line under each exception.
             if not self._copyright_val:
                 self._copyright_val = None
-        return self._copyright_val
+        return cast(Optional[Copyright], self._copyright_val)
 
     def _licenses(self) -> Dict[str, Path]:
         """Return a dictionary of all licenses in the project, with their SPDX
         identifiers as names and paths as values.
         """
-        license_files = {}
+        license_files: Dict[str, Path] = {}
 
         directory = str(self.root / "LICENSES/**")
-        for path in glob.iglob(directory, recursive=True):
-            path = Path(path)
+        for path_str in glob.iglob(directory, recursive=True):
+            path = Path(path_str)
             # For some reason, LICENSES/** is resolved even though it
             # doesn't exist. I have no idea why. Deal with that here.
             if not Path(path).exists() or Path(path).is_dir():
                 continue
             if Path(path).suffix == ".license":
                 continue
```

### Comparing `reuse-1.1.2/src/reuse/report.py` & `reuse-2.0.0/src/reuse/report.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,130 +1,188 @@
 # SPDX-FileCopyrightText: 2017 Free Software Foundation Europe e.V. <https://fsfe.org>
 # SPDX-FileCopyrightText: 2022 Florian Snow <florian@familysnow.net>
+# SPDX-FileCopyrightText: 2022 Pietro Albini <pietro.albini@ferrous-systems.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Module that contains reports about files and projects for linting."""
 
 import datetime
 import logging
 import multiprocessing as mp
 import random
 from gettext import gettext as _
 from hashlib import md5
 from io import StringIO
-from os import PathLike, cpu_count
+from os import cpu_count
 from pathlib import Path
-from typing import Iterable, List, NamedTuple, Optional, Set
+from typing import Any, Dict, Iterable, List, NamedTuple, Optional, Set, cast
 from uuid import uuid4
 
-from . import __version__
-from ._util import _LICENSING, _checksum
-from .project import Project
+from . import __REUSE_version__, __version__
+from ._util import _LICENSING, StrPath, _checksum
+from .project import Project, ReuseInfo
 
 _LOGGER = logging.getLogger(__name__)
 
+LINT_VERSION = "1.0"
+
 
 class _MultiprocessingContainer:
     """Container that remembers some data in order to generate a FileReport."""
 
-    def __init__(self, project, do_checksum):
+    def __init__(
+        self, project: Project, do_checksum: bool, add_license_concluded: bool
+    ):
         self.project = project
         self.do_checksum = do_checksum
+        self.add_license_concluded = add_license_concluded
 
-    def __call__(self, file_):
+    def __call__(self, file_: StrPath) -> "_MultiprocessingResult":
         # pylint: disable=broad-except
         try:
             return _MultiprocessingResult(
                 file_,
                 FileReport.generate(
-                    self.project, file_, do_checksum=self.do_checksum
+                    self.project,
+                    file_,
+                    do_checksum=self.do_checksum,
+                    add_license_concluded=self.add_license_concluded,
                 ),
                 None,
             )
         except Exception as exc:
             return _MultiprocessingResult(file_, None, exc)
 
 
 class _MultiprocessingResult(NamedTuple):
     """Result of :class:`MultiprocessingContainer`."""
 
-    path: PathLike
+    path: StrPath
     report: Optional["FileReport"]
     error: Optional[Exception]
 
 
 class ProjectReport:  # pylint: disable=too-many-instance-attributes
     """Object that holds linting report about the project."""
 
     def __init__(self, do_checksum: bool = True):
-        self.path = None
-        self.licenses = {}
-        self.missing_licenses = {}
-        self.bad_licenses = {}
-        self.deprecated_licenses = set()
-        self.read_errors = set()
-        self.file_reports = set()
-        self.licenses_without_extension = {}
+        self.path: StrPath = ""
+        self.licenses: Dict[str, Path] = {}
+        self.missing_licenses: Dict[str, Set[Path]] = {}
+        self.bad_licenses: Dict[str, Set[Path]] = {}
+        self.deprecated_licenses: Set[str] = set()
+        self.read_errors: Set[Path] = set()
+        self.file_reports: Set[FileReport] = set()
+        self.licenses_without_extension: Dict[str, Path] = {}
 
         self.do_checksum = do_checksum
 
-        self._unused_licenses = None
-        self._used_licenses = None
-        self._files_without_licenses = None
-        self._files_without_copyright = None
+        self._unused_licenses: Optional[Set[str]] = None
+        self._used_licenses: Optional[Set[str]] = None
+        self._files_without_licenses: Optional[Set[Path]] = None
+        self._files_without_copyright: Optional[Set[Path]] = None
+        self._is_compliant: Optional[bool] = None
+
+    def to_dict_lint(self) -> Dict[str, Any]:
+        """Collects and formats data relevant to linting from report and returns
+        it as a dictionary.
 
-    def to_dict(self):
-        """Turn the report into a json-like dictionary."""
-        return {
-            "path": str(Path(self.path).resolve()),
-            "licenses": {
-                identifier: str(path)
-                for identifier, path in self.licenses.items()
-            },
-            "bad_licenses": {
-                lic: [str(file_) for file_ in files]
-                for lic, files in self.bad_licenses.items()
-            },
-            "deprecated_licenses": sorted(self.deprecated_licenses),
-            "licenses_without_extension": {
-                identifier: str(path)
-                for identifier, path in self.licenses_without_extension.items()
+        :return: Dictionary containing data from the ProjectReport object
+        """
+        # Setup report data container
+        data: Dict[str, Any] = {
+            "non_compliant": {
+                "missing_licenses": self.missing_licenses,
+                "unused_licenses": [str(file) for file in self.unused_licenses],
+                "deprecated_licenses": [
+                    str(file) for file in self.deprecated_licenses
+                ],
+                "bad_licenses": self.bad_licenses,
+                "licenses_without_extension": self.licenses_without_extension,
+                "missing_copyright_info": [
+                    str(file) for file in self.files_without_copyright
+                ],
+                "missing_licensing_info": [
+                    str(file) for file in self.files_without_licenses
+                ],
+                "read_errors": [str(file) for file in self.read_errors],
             },
-            "missing_licenses": {
-                lic: [str(file_) for file_ in files]
-                for lic, files in self.missing_licenses.items()
+            "files": [],
+            "summary": {
+                "used_licenses": [],
             },
-            "read_errors": list(map(str, self.read_errors)),
-            "file_reports": [report.to_dict() for report in self.file_reports],
         }
 
-    def bill_of_materials(self) -> str:
+        # Populate 'files'
+        for file_report in self.file_reports:
+            data["files"].append(file_report.to_dict_lint())
+
+        # Populate 'summary'
+        number_of_files = len(self.file_reports)
+        data["summary"] = {
+            "used_licenses": list(self.used_licenses),
+            "files_total": number_of_files,
+            "files_with_copyright_info": number_of_files
+            - len(self.files_without_copyright),
+            "files_with_licensing_info": number_of_files
+            - len(self.files_without_licenses),
+            "compliant": self.is_compliant,
+        }
+
+        # Add the top three keys
+        unsorted_data = {
+            "lint_version": LINT_VERSION,
+            "reuse_spec_version": __REUSE_version__,
+            "reuse_tool_version": __version__,
+            **data,
+        }
+
+        # Sort dictionary keys while keeping the top three keys at the beginning
+        sorted_keys = sorted(list(unsorted_data.keys()))
+        sorted_keys.remove("lint_version")
+        sorted_keys.remove("reuse_spec_version")
+        sorted_keys.remove("reuse_tool_version")
+        sorted_keys = [
+            "lint_version",
+            "reuse_spec_version",
+            "reuse_tool_version",
+        ] + sorted_keys
+
+        sorted_data = {key: unsorted_data[key] for key in sorted_keys}
+
+        return sorted_data
+
+    def bill_of_materials(
+        self,
+        creator_person: Optional[str] = None,
+        creator_organization: Optional[str] = None,
+    ) -> str:
         """Generate a bill of materials from the project.
 
         See https://spdx.org/specifications.
         """
         out = StringIO()
         # Write mandatory tags
         out.write("SPDXVersion: SPDX-2.1\n")
         out.write("DataLicense: CC0-1.0\n")
         out.write("SPDXID: SPDXRef-DOCUMENT\n")
 
         out.write(f"DocumentName: {Path(self.path).resolve().name}\n")
         # TODO: Generate UUID from git revision maybe
         # TODO: Fix the URL
         out.write(
-            f"DocumentNamespace:"
-            f" http://spdx.org/spdxdocs/spdx-v2.1-{uuid4()}\n"
+            f"DocumentNamespace: http://spdx.org/spdxdocs/spdx-v2.1-{uuid4()}\n"
         )
 
         # Author
-        # TODO: Fix Person and Organization
-        out.write("Creator: Person: Anonymous ()\n")
-        out.write("Creator: Organization: Anonymous ()\n")
+        out.write(f"Creator: Person: {format_creator(creator_person)}\n")
+        out.write(
+            f"Creator: Organization: {format_creator(creator_organization)}\n"
+        )
         out.write(f"Creator: Tool: reuse-{__version__}\n")
 
         now = datetime.datetime.utcnow()
         now = now.replace(microsecond=0)
         out.write(f"Created: {now.isoformat()}Z\n")
         out.write(
             "CreatorComment: <text>This document was created automatically"
@@ -132,32 +190,32 @@
             " REUSE.</text>\n"
         )
 
         reports = sorted(self.file_reports, key=lambda x: x.spdxfile.name)
 
         for report in reports:
             out.write(
-                f"Relationship: SPDXRef-DOCUMENT describes"
+                "Relationship: SPDXRef-DOCUMENT describes"
                 f" {report.spdxfile.spdx_id}\n"
             )
 
         for report in reports:
             out.write("\n")
             out.write(f"FileName: {report.spdxfile.name}\n")
             out.write(f"SPDXID: {report.spdxfile.spdx_id}\n")
             out.write(f"FileChecksum: SHA1: {report.spdxfile.chk_sum}\n")
-            # IMPORTANT: Make no assertion about concluded license. This tool
-            # cannot, with full certainty, determine the license of a file.
-            out.write("LicenseConcluded: NOASSERTION\n")
+            out.write(
+                f"LicenseConcluded: {report.spdxfile.license_concluded}\n"
+            )
 
             for lic in sorted(report.spdxfile.licenses_in_file):
                 out.write(f"LicenseInfoInFile: {lic}\n")
             if report.spdxfile.copyright:
                 out.write(
-                    f"FileCopyrightText:"
+                    "FileCopyrightText:"
                     f" <text>{report.spdxfile.copyright}</text>\n"
                 )
             else:
                 out.write("FileCopyrightText: NONE\n")
 
         # Licenses
         for lic, path in sorted(self.licenses.items()):
@@ -172,60 +230,67 @@
         return out.getvalue()
 
     @classmethod
     def generate(
         cls,
         project: Project,
         do_checksum: bool = True,
-        multiprocessing: bool = cpu_count() > 1,
+        multiprocessing: bool = cpu_count() > 1,  # type: ignore
+        add_license_concluded: bool = False,
     ) -> "ProjectReport":
         """Generate a ProjectReport from a Project."""
         project_report = cls(do_checksum=do_checksum)
         project_report.path = project.root
         project_report.licenses = project.licenses
         project_report.licenses_without_extension = (
             project.licenses_without_extension
         )
 
-        container = _MultiprocessingContainer(project, do_checksum)
+        container = _MultiprocessingContainer(
+            project, do_checksum, add_license_concluded
+        )
 
         if multiprocessing:
             with mp.Pool() as pool:
-                results = pool.map(container, project.all_files())
+                results: Iterable[_MultiprocessingResult] = pool.map(
+                    container, project.all_files()
+                )
             pool.join()
         else:
             results = map(container, project.all_files())
 
         for result in results:
             if result.error:
                 if isinstance(result.error, (OSError, UnicodeError)):
                     _LOGGER.error(
                         _("Could not read '{path}'").format(path=result.path),
                         exc_info=result.error,
                     )
-                    project_report.read_errors.add(result.path)
+                    project_report.read_errors.add(Path(result.path))
                     continue
                 _LOGGER.error(
                     _(
                         "Unexpected error occurred while parsing '{path}'"
                     ).format(path=result.path),
                     exc_info=result.error,
                 )
-                project_report.read_errors.add(result.path)
+                project_report.read_errors.add(Path(result.path))
                 continue
-            file_report = result.report
+            file_report = cast(FileReport, result.report)
 
             # File report.
             project_report.file_reports.add(file_report)
 
-            # Bad and missing licenses.
+            # Missing licenses.
             for missing_license in file_report.missing_licenses:
                 project_report.missing_licenses.setdefault(
                     missing_license, set()
                 ).add(file_report.path)
+
+            # Bad licenses
             for bad_license in file_report.bad_licenses:
                 project_report.bad_licenses.setdefault(bad_license, set()).add(
                     file_report.path
                 )
 
         # More bad licenses, and also deprecated licenses
         for name, path in project.licenses.items():
@@ -264,84 +329,123 @@
             lic
             for lic in suspected_unused_licenses
             if f"{lic}+" not in self.used_licenses
         }
         return self._unused_licenses
 
     @property
-    def files_without_licenses(self) -> Iterable[PathLike]:
-        """Iterable of paths that have no license information."""
+    def files_without_licenses(self) -> Set[Path]:
+        """Set of paths that have no license information."""
         if self._files_without_licenses is not None:
             return self._files_without_licenses
 
         self._files_without_licenses = {
             file_report.path
             for file_report in self.file_reports
             if not file_report.spdxfile.licenses_in_file
         }
 
         return self._files_without_licenses
 
     @property
-    def files_without_copyright(self) -> Iterable[PathLike]:
-        """Iterable of paths that have no copyright information."""
+    def files_without_copyright(self) -> Set[Path]:
+        """Set of paths that have no copyright information."""
         if self._files_without_copyright is not None:
             return self._files_without_copyright
 
         self._files_without_copyright = {
             file_report.path
             for file_report in self.file_reports
             if not file_report.spdxfile.copyright
         }
 
         return self._files_without_copyright
 
+    @property
+    def is_compliant(self) -> bool:
+        """Whether the report is compliant with the REUSE Spec."""
+        if self._is_compliant is not None:
+            return self._is_compliant
+
+        self._is_compliant = not any(
+            (
+                self.missing_licenses,
+                self.unused_licenses,
+                self.bad_licenses,
+                self.deprecated_licenses,
+                self.licenses_without_extension,
+                self.files_without_copyright,
+                self.files_without_licenses,
+                self.read_errors,
+            )
+        )
+
+        return self._is_compliant
+
 
 class _File:  # pylint: disable=too-few-public-methods
     """Represent an SPDX file. Sufficiently enough for our purposes, in any
     case.
     """
 
-    def __init__(self, name, spdx_id=None, chk_sum=None):
+    def __init__(
+        self,
+        name: str,
+        spdx_id: Optional[str] = None,
+        chk_sum: Optional[str] = None,
+    ):
         self.name: str = name
-        self.spdx_id: str = spdx_id
-        self.chk_sum: str = chk_sum
+        self.spdx_id: Optional[str] = spdx_id
+        self.chk_sum: Optional[str] = chk_sum
         self.licenses_in_file: List[str] = []
-        self.copyright: str = None
+        self.license_concluded: str = ""
+        self.copyright: str = ""
+        self.info: ReuseInfo = ReuseInfo()
 
 
 class FileReport:
     """Object that holds a linting report about a single file. Importantly,
     it also contains SPDX File information in :attr:`spdxfile`.
     """
 
-    def __init__(
-        self, name: PathLike, path: PathLike, do_checksum: bool = True
-    ):
-        self.spdxfile = _File(name)
+    def __init__(self, name: StrPath, path: StrPath, do_checksum: bool = True):
+        self.spdxfile = _File(str(name))
         self.path = Path(path)
         self.do_checksum = do_checksum
 
-        self.bad_licenses = set()
-        self.missing_licenses = set()
+        self.bad_licenses: Set[str] = set()
+        self.missing_licenses: Set[str] = set()
 
-    def to_dict(self):
-        """Turn the report into a json-like dictionary."""
+    def to_dict_lint(self) -> Dict[str, Any]:
+        """Turn the report into a json-like dictionary with exclusively
+        information relevant for linting.
+        """
         return {
             "path": str(Path(self.path).resolve()),
-            "name": self.spdxfile.name,
-            "spdx_id": self.spdxfile.spdx_id,
-            "chk_sum": self.spdxfile.chk_sum,
-            "licenses_in_file": sorted(self.spdxfile.licenses_in_file),
-            "copyright": self.spdxfile.copyright,
+            # TODO: Why does every copyright line have the same source?
+            "copyrights": [
+                {"value": copyright_, "source": self.spdxfile.info.source_path}
+                for copyright_ in self.spdxfile.copyright.split("\n")
+                if copyright_
+            ],
+            # TODO: Why does every license expression have the same source?
+            "licenses": [
+                {"value": license_, "source": self.spdxfile.info.source_path}
+                for license_ in self.spdxfile.licenses_in_file
+                if license_
+            ],
         }
 
     @classmethod
     def generate(
-        cls, project: Project, path: PathLike, do_checksum: bool = True
+        cls,
+        project: Project,
+        path: StrPath,
+        do_checksum: bool = True,
+        add_license_concluded: bool = False,
     ) -> "FileReport":
         """Generate a FileReport from a path in a Project."""
         path = Path(path)
         if not path.is_file():
             raise OSError(f"{path} is not a file")
 
         relative = project.relative_from_root(path)
@@ -356,16 +460,16 @@
             # hash.
             report.spdxfile.chk_sum = f"{random.getrandbits(160):040x}"
         spdx_id = md5()
         spdx_id.update(str(relative).encode("utf-8"))
         spdx_id.update(report.spdxfile.chk_sum.encode("utf-8"))
         report.spdxfile.spdx_id = f"SPDXRef-{spdx_id.hexdigest()}"
 
-        spdx_info = project.spdx_info_of(path)
-        for expression in spdx_info.spdx_expressions:
+        reuse_info = project.reuse_info_of(path)
+        for expression in reuse_info.spdx_expressions:
             for identifier in _LICENSING.license_keys(expression):
                 # A license expression akin to Apache-1.0+ should register
                 # correctly if LICENSES/Apache-1.0.txt exists.
                 identifiers = {identifier}
                 if identifier.endswith("+"):
                     identifiers.add(identifier[:-1])
                 # Bad license
@@ -374,16 +478,49 @@
                 # Missing license
                 if not identifiers.intersection(project.licenses):
                     report.missing_licenses.add(identifier)
 
                 # Add license to report.
                 report.spdxfile.licenses_in_file.append(identifier)
 
-        # Copyright text
-        report.spdxfile.copyright = "\n".join(sorted(spdx_info.copyright_lines))
+        if not add_license_concluded:
+            report.spdxfile.license_concluded = "NOASSERTION"
+        elif not reuse_info.spdx_expressions:
+            report.spdxfile.license_concluded = "NONE"
+        else:
+            # Merge all the license expressions together, wrapping them in
+            # parentheses to make sure an expression doesn't spill into another
+            # one. The extra parentheses will be removed by the roundtrip
+            # through parse() -> simplify() -> render().
+            report.spdxfile.license_concluded = (
+                _LICENSING.parse(
+                    " AND ".join(
+                        f"({expression})"
+                        for expression in reuse_info.spdx_expressions
+                    ),
+                )
+                .simplify()
+                .render()
+            )
 
+        # Copyright text
+        report.spdxfile.copyright = "\n".join(
+            sorted(reuse_info.copyright_lines)
+        )
+        # Source of licensing and copyright info
+        report.spdxfile.info = reuse_info
         return report
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         if self.spdxfile.chk_sum is not None:
             return hash(self.spdxfile.name + self.spdxfile.chk_sum)
-        return super().__hash__(self)
+        return super().__hash__()
+
+
+def format_creator(creator: Optional[str]) -> str:
+    """Render the creator field based on the provided flag"""
+    if creator is None:
+        return "Anonymous ()"
+    if "(" in creator and creator.endswith(")"):
+        # The creator field already contains an email address
+        return creator
+    return creator + " ()"
```

### Comparing `reuse-1.1.2/src/reuse/resources/exceptions.json` & `reuse-2.0.0/src/reuse/resources/exceptions.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6243622448979592%*

 * *Differences: {"'exceptions'": "{0: {'referenceNumber': 48}, 2: {'referenceNumber': 42}, 3: {'referenceNumber': "*

 * *                 "41}, 6: {'referenceNumber': 11}, 7: {'referenceNumber': 50}, 8: "*

 * *                 "{'referenceNumber': 36}, 9: {'referenceNumber': 9}, 11: {'referenceNumber': 20}, "*

 * *                 "12: {'referenceNumber': 38}, 13: {'referenceNumber': 8}, 14: {'referenceNumber': "*

 * *                 "18}, 15: {'referenceNumber': 7}, 16: {'referenceNumber': 47}, 17: "*

 * *                 "{'referenceNumber': 54 […]*

```diff
@@ -2,510 +2,642 @@
     "exceptions": [
         {
             "detailsUrl": "./389-exception.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "389-exception",
             "name": "389 Directory Server Exception",
             "reference": "./389-exception.json",
-            "referenceNumber": 37,
+            "referenceNumber": 48,
             "seeAlso": [
                 "http://directory.fedoraproject.org/wiki/GPL_Exception_License_Text",
                 "https://web.archive.org/web/20080828121337/http://directory.fedoraproject.org/wiki/GPL_Exception_License_Text"
             ]
         },
         {
+            "detailsUrl": "./Asterisk-exception.html",
+            "isDeprecatedLicenseId": false,
+            "licenseExceptionId": "Asterisk-exception",
+            "name": "Asterisk exception",
+            "reference": "./Asterisk-exception.json",
+            "referenceNumber": 33,
+            "seeAlso": [
+                "https://github.com/asterisk/libpri/blob/7f91151e6bd10957c746c031c1f4a030e8146e9a/pri.c#L22",
+                "https://github.com/asterisk/libss7/blob/03e81bcd0d28ff25d4c77c78351ddadc82ff5c3f/ss7.c#L24"
+            ]
+        },
+        {
             "detailsUrl": "./Autoconf-exception-2.0.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "Autoconf-exception-2.0",
             "name": "Autoconf exception 2.0",
             "reference": "./Autoconf-exception-2.0.json",
-            "referenceNumber": 13,
+            "referenceNumber": 42,
             "seeAlso": [
                 "http://ac-archive.sourceforge.net/doc/copyright.html",
                 "http://ftp.gnu.org/gnu/autoconf/autoconf-2.59.tar.gz"
             ]
         },
         {
             "detailsUrl": "./Autoconf-exception-3.0.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "Autoconf-exception-3.0",
             "name": "Autoconf exception 3.0",
             "reference": "./Autoconf-exception-3.0.json",
-            "referenceNumber": 32,
+            "referenceNumber": 41,
             "seeAlso": [
                 "http://www.gnu.org/licenses/autoconf-exception-3.0.html"
             ]
         },
         {
+            "detailsUrl": "./Autoconf-exception-generic.html",
+            "isDeprecatedLicenseId": false,
+            "licenseExceptionId": "Autoconf-exception-generic",
+            "name": "Autoconf generic exception",
+            "reference": "./Autoconf-exception-generic.json",
+            "referenceNumber": 4,
+            "seeAlso": [
+                "https://launchpad.net/ubuntu/precise/+source/xmltooling/+copyright",
+                "https://tracker.debian.org/media/packages/s/sipwitch/copyright-1.9.15-3",
+                "https://opensource.apple.com/source/launchd/launchd-258.1/launchd/compile.auto.html"
+            ]
+        },
+        {
+            "detailsUrl": "./Autoconf-exception-macro.html",
+            "isDeprecatedLicenseId": false,
+            "licenseExceptionId": "Autoconf-exception-macro",
+            "name": "Autoconf macro exception",
+            "reference": "./Autoconf-exception-macro.json",
+            "referenceNumber": 19,
+            "seeAlso": [
+                "https://github.com/freedesktop/xorg-macros/blob/39f07f7db58ebbf3dcb64a2bf9098ed5cf3d1223/xorg-macros.m4.in",
+                "https://www.gnu.org/software/autoconf-archive/ax_pthread.html",
+                "https://launchpad.net/ubuntu/precise/+source/xmltooling/+copyright"
+            ]
+        },
+        {
             "detailsUrl": "./Bison-exception-2.2.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "Bison-exception-2.2",
             "name": "Bison exception 2.2",
             "reference": "./Bison-exception-2.2.json",
-            "referenceNumber": 17,
+            "referenceNumber": 11,
             "seeAlso": [
                 "http://git.savannah.gnu.org/cgit/bison.git/tree/data/yacc.c?id=193d7c7054ba7197b0789e14965b739162319b5e#n141"
             ]
         },
         {
             "detailsUrl": "./Bootloader-exception.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "Bootloader-exception",
             "name": "Bootloader Distribution Exception",
             "reference": "./Bootloader-exception.json",
-            "referenceNumber": 21,
+            "referenceNumber": 50,
             "seeAlso": [
                 "https://github.com/pyinstaller/pyinstaller/blob/develop/COPYING.txt"
             ]
         },
         {
             "detailsUrl": "./Classpath-exception-2.0.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "Classpath-exception-2.0",
             "name": "Classpath exception 2.0",
             "reference": "./Classpath-exception-2.0.json",
-            "referenceNumber": 29,
+            "referenceNumber": 36,
             "seeAlso": [
                 "http://www.gnu.org/software/classpath/license.html",
                 "https://fedoraproject.org/wiki/Licensing/GPL_Classpath_Exception"
             ]
         },
         {
             "detailsUrl": "./CLISP-exception-2.0.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "CLISP-exception-2.0",
             "name": "CLISP exception 2.0",
             "reference": "./CLISP-exception-2.0.json",
-            "referenceNumber": 6,
+            "referenceNumber": 9,
             "seeAlso": [
                 "http://sourceforge.net/p/clisp/clisp/ci/default/tree/COPYRIGHT"
             ]
         },
         {
+            "detailsUrl": "./cryptsetup-OpenSSL-exception.html",
+            "isDeprecatedLicenseId": false,
+            "licenseExceptionId": "cryptsetup-OpenSSL-exception",
+            "name": "cryptsetup OpenSSL exception",
+            "reference": "./cryptsetup-OpenSSL-exception.json",
+            "referenceNumber": 39,
+            "seeAlso": [
+                "https://gitlab.com/cryptsetup/cryptsetup/-/blob/main/COPYING",
+                "https://gitlab.nic.cz/datovka/datovka/-/blob/develop/COPYING",
+                "https://github.com/nbs-system/naxsi/blob/951123ad456bdf5ac94e8d8819342fe3d49bc002/naxsi_src/naxsi_raw.c",
+                "http://web.mit.edu/jgross/arch/amd64_deb60/bin/mosh"
+            ]
+        },
+        {
             "detailsUrl": "./DigiRule-FOSS-exception.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "DigiRule-FOSS-exception",
             "name": "DigiRule FOSS License Exception",
             "reference": "./DigiRule-FOSS-exception.json",
-            "referenceNumber": 26,
+            "referenceNumber": 20,
             "seeAlso": [
                 "http://www.digirulesolutions.com/drupal/foss"
             ]
         },
         {
             "detailsUrl": "./eCos-exception-2.0.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "eCos-exception-2.0",
             "name": "eCos exception 2.0",
             "reference": "./eCos-exception-2.0.json",
-            "referenceNumber": 11,
+            "referenceNumber": 38,
             "seeAlso": [
                 "http://ecos.sourceware.org/license-overview.html"
             ]
         },
         {
             "detailsUrl": "./Fawkes-Runtime-exception.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "Fawkes-Runtime-exception",
             "name": "Fawkes Runtime Exception",
             "reference": "./Fawkes-Runtime-exception.json",
-            "referenceNumber": 2,
+            "referenceNumber": 8,
             "seeAlso": [
                 "http://www.fawkesrobotics.org/about/license/"
             ]
         },
         {
             "detailsUrl": "./FLTK-exception.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "FLTK-exception",
             "name": "FLTK exception",
             "reference": "./FLTK-exception.json",
-            "referenceNumber": 34,
+            "referenceNumber": 18,
             "seeAlso": [
                 "http://www.fltk.org/COPYING.php"
             ]
         },
         {
             "detailsUrl": "./Font-exception-2.0.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "Font-exception-2.0",
             "name": "Font exception 2.0",
             "reference": "./Font-exception-2.0.json",
-            "referenceNumber": 14,
+            "referenceNumber": 7,
             "seeAlso": [
                 "http://www.gnu.org/licenses/gpl-faq.html#FontException"
             ]
         },
         {
             "detailsUrl": "./freertos-exception-2.0.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "freertos-exception-2.0",
             "name": "FreeRTOS Exception 2.0",
             "reference": "./freertos-exception-2.0.json",
-            "referenceNumber": 45,
+            "referenceNumber": 47,
             "seeAlso": [
                 "https://web.archive.org/web/20060809182744/http://www.freertos.org/a00114.html"
             ]
         },
         {
             "detailsUrl": "./GCC-exception-2.0.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "GCC-exception-2.0",
             "name": "GCC Runtime Library exception 2.0",
             "reference": "./GCC-exception-2.0.json",
-            "referenceNumber": 28,
+            "referenceNumber": 54,
             "seeAlso": [
                 "https://gcc.gnu.org/git/?p=gcc.git;a=blob;f=gcc/libgcc1.c;h=762f5143fc6eed57b6797c82710f3538aa52b40b;hb=cb143a3ce4fb417c68f5fa2691a1b1b1053dfba9#l10"
             ]
         },
         {
             "detailsUrl": "./GCC-exception-3.1.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "GCC-exception-3.1",
             "name": "GCC Runtime Library exception 3.1",
             "reference": "./GCC-exception-3.1.json",
-            "referenceNumber": 3,
+            "referenceNumber": 27,
             "seeAlso": [
                 "http://www.gnu.org/licenses/gcc-exception-3.1.html"
             ]
         },
         {
+            "detailsUrl": "./GNAT-exception.html",
+            "isDeprecatedLicenseId": false,
+            "licenseExceptionId": "GNAT-exception",
+            "name": "GNAT exception",
+            "reference": "./GNAT-exception.json",
+            "referenceNumber": 13,
+            "seeAlso": [
+                "https://github.com/AdaCore/florist/blob/master/libsrc/posix-configurable_file_limits.adb"
+            ]
+        },
+        {
             "detailsUrl": "./gnu-javamail-exception.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "gnu-javamail-exception",
             "name": "GNU JavaMail exception",
             "reference": "./gnu-javamail-exception.json",
-            "referenceNumber": 19,
+            "referenceNumber": 34,
             "seeAlso": [
                 "http://www.gnu.org/software/classpathx/javamail/javamail.html"
             ]
         },
         {
+            "detailsUrl": "./GPL-3.0-interface-exception.html",
+            "isDeprecatedLicenseId": false,
+            "licenseExceptionId": "GPL-3.0-interface-exception",
+            "name": "GPL-3.0 Interface Exception",
+            "reference": "./GPL-3.0-interface-exception.json",
+            "referenceNumber": 21,
+            "seeAlso": [
+                "https://www.gnu.org/licenses/gpl-faq.en.html#LinkingOverControlledInterface"
+            ]
+        },
+        {
             "detailsUrl": "./GPL-3.0-linking-exception.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "GPL-3.0-linking-exception",
             "name": "GPL-3.0 Linking Exception",
             "reference": "./GPL-3.0-linking-exception.json",
-            "referenceNumber": 36,
+            "referenceNumber": 1,
             "seeAlso": [
                 "https://www.gnu.org/licenses/gpl-faq.en.html#GPLIncompatibleLibs"
             ]
         },
         {
             "detailsUrl": "./GPL-3.0-linking-source-exception.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "GPL-3.0-linking-source-exception",
             "name": "GPL-3.0 Linking Exception (with Corresponding Source)",
             "reference": "./GPL-3.0-linking-source-exception.json",
-            "referenceNumber": 25,
+            "referenceNumber": 37,
             "seeAlso": [
                 "https://www.gnu.org/licenses/gpl-faq.en.html#GPLIncompatibleLibs",
                 "https://github.com/mirror/wget/blob/master/src/http.c#L20"
             ]
         },
         {
             "detailsUrl": "./GPL-CC-1.0.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "GPL-CC-1.0",
             "name": "GPL Cooperation Commitment 1.0",
             "reference": "./GPL-CC-1.0.json",
-            "referenceNumber": 38,
+            "referenceNumber": 52,
             "seeAlso": [
                 "https://github.com/gplcc/gplcc/blob/master/Project/COMMITMENT",
                 "https://gplcc.github.io/gplcc/Project/README-PROJECT.html"
             ]
         },
         {
             "detailsUrl": "./GStreamer-exception-2005.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "GStreamer-exception-2005",
             "name": "GStreamer Exception (2005)",
             "reference": "./GStreamer-exception-2005.json",
-            "referenceNumber": 27,
+            "referenceNumber": 35,
             "seeAlso": [
                 "https://gstreamer.freedesktop.org/documentation/frequently-asked-questions/licensing.html?gi-language=c#licensing-of-applications-using-gstreamer"
             ]
         },
         {
             "detailsUrl": "./GStreamer-exception-2008.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "GStreamer-exception-2008",
             "name": "GStreamer Exception (2008)",
             "reference": "./GStreamer-exception-2008.json",
-            "referenceNumber": 16,
+            "referenceNumber": 30,
             "seeAlso": [
                 "https://gstreamer.freedesktop.org/documentation/frequently-asked-questions/licensing.html?gi-language=c#licensing-of-applications-using-gstreamer"
             ]
         },
         {
             "detailsUrl": "./i2p-gpl-java-exception.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "i2p-gpl-java-exception",
             "name": "i2p GPL+Java Exception",
             "reference": "./i2p-gpl-java-exception.json",
-            "referenceNumber": 18,
+            "referenceNumber": 40,
             "seeAlso": [
                 "http://geti2p.net/en/get-involved/develop/licenses#java_exception"
             ]
         },
         {
             "detailsUrl": "./KiCad-libraries-exception.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "KiCad-libraries-exception",
             "name": "KiCad Libraries Exception",
             "reference": "./KiCad-libraries-exception.json",
-            "referenceNumber": 39,
+            "referenceNumber": 28,
             "seeAlso": [
                 "https://www.kicad.org/libraries/license/"
             ]
         },
         {
             "detailsUrl": "./LGPL-3.0-linking-exception.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "LGPL-3.0-linking-exception",
             "name": "LGPL-3.0 Linking Exception",
             "reference": "./LGPL-3.0-linking-exception.json",
-            "referenceNumber": 4,
+            "referenceNumber": 2,
             "seeAlso": [
                 "https://raw.githubusercontent.com/go-xmlpath/xmlpath/v2/LICENSE",
                 "https://github.com/goamz/goamz/blob/master/LICENSE",
                 "https://github.com/juju/errors/blob/master/LICENSE"
             ]
         },
         {
+            "detailsUrl": "./libpri-OpenH323-exception.html",
+            "isDeprecatedLicenseId": false,
+            "licenseExceptionId": "libpri-OpenH323-exception",
+            "name": "libpri OpenH323 exception",
+            "reference": "./libpri-OpenH323-exception.json",
+            "referenceNumber": 32,
+            "seeAlso": [
+                "https://github.com/asterisk/libpri/blob/1.6.0/README#L19-L22"
+            ]
+        },
+        {
             "detailsUrl": "./Libtool-exception.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "Libtool-exception",
             "name": "Libtool Exception",
             "reference": "./Libtool-exception.json",
-            "referenceNumber": 7,
+            "referenceNumber": 17,
             "seeAlso": [
                 "http://git.savannah.gnu.org/cgit/libtool.git/tree/m4/libtool.m4"
             ]
         },
         {
             "detailsUrl": "./Linux-syscall-note.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "Linux-syscall-note",
             "name": "Linux Syscall Note",
             "reference": "./Linux-syscall-note.json",
-            "referenceNumber": 42,
+            "referenceNumber": 49,
             "seeAlso": [
                 "https://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux.git/tree/COPYING"
             ]
         },
         {
+            "detailsUrl": "./LLGPL.html",
+            "isDeprecatedLicenseId": false,
+            "licenseExceptionId": "LLGPL",
+            "name": "LLGPL Preamble",
+            "reference": "./LLGPL.json",
+            "referenceNumber": 3,
+            "seeAlso": [
+                "http://opensource.franz.com/preamble.html"
+            ]
+        },
+        {
             "detailsUrl": "./LLVM-exception.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "LLVM-exception",
             "name": "LLVM Exception",
             "reference": "./LLVM-exception.json",
-            "referenceNumber": 41,
+            "referenceNumber": 14,
             "seeAlso": [
                 "http://llvm.org/foundation/relicensing/LICENSE.txt"
             ]
         },
         {
             "detailsUrl": "./LZMA-exception.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "LZMA-exception",
             "name": "LZMA exception",
             "reference": "./LZMA-exception.json",
-            "referenceNumber": 31,
+            "referenceNumber": 55,
             "seeAlso": [
                 "http://nsis.sourceforge.net/Docs/AppendixI.html#I.6"
             ]
         },
         {
             "detailsUrl": "./mif-exception.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "mif-exception",
             "name": "Macros and Inline Functions Exception",
             "reference": "./mif-exception.json",
-            "referenceNumber": 1,
+            "referenceNumber": 53,
             "seeAlso": [
                 "http://www.scs.stanford.edu/histar/src/lib/cppsup/exception",
                 "http://dev.bertos.org/doxygen/",
                 "https://www.threadingbuildingblocks.org/licensing"
             ]
         },
         {
             "detailsUrl": "./Nokia-Qt-exception-1.1.html",
             "isDeprecatedLicenseId": true,
             "licenseExceptionId": "Nokia-Qt-exception-1.1",
             "name": "Nokia Qt LGPL exception 1.1",
             "reference": "./Nokia-Qt-exception-1.1.json",
-            "referenceNumber": 8,
+            "referenceNumber": 31,
             "seeAlso": [
                 "https://www.keepassx.org/dev/projects/keepassx/repository/revisions/b8dfb9cc4d5133e0f09cd7533d15a4f1c19a40f2/entry/LICENSE.NOKIA-LGPL-EXCEPTION"
             ]
         },
         {
             "detailsUrl": "./OCaml-LGPL-linking-exception.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "OCaml-LGPL-linking-exception",
             "name": "OCaml LGPL Linking Exception",
             "reference": "./OCaml-LGPL-linking-exception.json",
-            "referenceNumber": 10,
+            "referenceNumber": 29,
             "seeAlso": [
                 "https://caml.inria.fr/ocaml/license.en.html"
             ]
         },
         {
             "detailsUrl": "./OCCT-exception-1.0.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "OCCT-exception-1.0",
             "name": "Open CASCADE Exception 1.0",
             "reference": "./OCCT-exception-1.0.json",
-            "referenceNumber": 20,
+            "referenceNumber": 15,
             "seeAlso": [
                 "http://www.opencascade.com/content/licensing"
             ]
         },
         {
             "detailsUrl": "./OpenJDK-assembly-exception-1.0.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "OpenJDK-assembly-exception-1.0",
             "name": "OpenJDK Assembly exception 1.0",
             "reference": "./OpenJDK-assembly-exception-1.0.json",
-            "referenceNumber": 30,
+            "referenceNumber": 24,
             "seeAlso": [
                 "http://openjdk.java.net/legal/assembly-exception.html"
             ]
         },
         {
             "detailsUrl": "./openvpn-openssl-exception.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "openvpn-openssl-exception",
             "name": "OpenVPN OpenSSL Exception",
             "reference": "./openvpn-openssl-exception.json",
-            "referenceNumber": 44,
+            "referenceNumber": 43,
             "seeAlso": [
                 "http://openvpn.net/index.php/license.html"
             ]
         },
         {
             "detailsUrl": "./PS-or-PDF-font-exception-20170817.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "PS-or-PDF-font-exception-20170817",
             "name": "PS/PDF font exception (2017-08-17)",
             "reference": "./PS-or-PDF-font-exception-20170817.json",
-            "referenceNumber": 35,
+            "referenceNumber": 45,
             "seeAlso": [
                 "https://github.com/ArtifexSoftware/urw-base35-fonts/blob/65962e27febc3883a17e651cdb23e783668c996f/LICENSE"
             ]
         },
         {
+            "detailsUrl": "./QPL-1.0-INRIA-2004-exception.html",
+            "isDeprecatedLicenseId": false,
+            "licenseExceptionId": "QPL-1.0-INRIA-2004-exception",
+            "name": "INRIA QPL 1.0 2004 variant exception",
+            "reference": "./QPL-1.0-INRIA-2004-exception.json",
+            "referenceNumber": 44,
+            "seeAlso": [
+                "https://git.frama-c.com/pub/frama-c/-/blob/master/licenses/Q_MODIFIED_LICENSE",
+                "https://github.com/maranget/hevea/blob/master/LICENSE"
+            ]
+        },
+        {
             "detailsUrl": "./Qt-GPL-exception-1.0.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "Qt-GPL-exception-1.0",
             "name": "Qt GPL exception 1.0",
             "reference": "./Qt-GPL-exception-1.0.json",
-            "referenceNumber": 24,
+            "referenceNumber": 10,
             "seeAlso": [
                 "http://code.qt.io/cgit/qt/qtbase.git/tree/LICENSE.GPL3-EXCEPT"
             ]
         },
         {
             "detailsUrl": "./Qt-LGPL-exception-1.1.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "Qt-LGPL-exception-1.1",
             "name": "Qt LGPL exception 1.1",
             "reference": "./Qt-LGPL-exception-1.1.json",
-            "referenceNumber": 5,
+            "referenceNumber": 16,
             "seeAlso": [
                 "http://code.qt.io/cgit/qt/qtbase.git/tree/LGPL_EXCEPTION.txt"
             ]
         },
         {
             "detailsUrl": "./Qwt-exception-1.0.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "Qwt-exception-1.0",
             "name": "Qwt exception 1.0",
             "reference": "./Qwt-exception-1.0.json",
-            "referenceNumber": 9,
+            "referenceNumber": 51,
             "seeAlso": [
                 "http://qwt.sourceforge.net/qwtlicense.html"
             ]
         },
         {
             "detailsUrl": "./SHL-2.0.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "SHL-2.0",
             "name": "Solderpad Hardware License v2.0",
             "reference": "./SHL-2.0.json",
-            "referenceNumber": 33,
+            "referenceNumber": 26,
             "seeAlso": [
                 "https://solderpad.org/licenses/SHL-2.0/"
             ]
         },
         {
             "detailsUrl": "./SHL-2.1.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "SHL-2.1",
             "name": "Solderpad Hardware License v2.1",
             "reference": "./SHL-2.1.json",
-            "referenceNumber": 43,
+            "referenceNumber": 23,
             "seeAlso": [
                 "https://solderpad.org/licenses/SHL-2.1/"
             ]
         },
         {
+            "detailsUrl": "./SWI-exception.html",
+            "isDeprecatedLicenseId": false,
+            "licenseExceptionId": "SWI-exception",
+            "name": "SWI exception",
+            "reference": "./SWI-exception.json",
+            "referenceNumber": 22,
+            "seeAlso": [
+                "https://github.com/SWI-Prolog/packages-clpqr/blob/bfa80b9270274f0800120d5b8e6fef42ac2dc6a5/clpqr/class.pl"
+            ]
+        },
+        {
             "detailsUrl": "./Swift-exception.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "Swift-exception",
             "name": "Swift Exception",
             "reference": "./Swift-exception.json",
-            "referenceNumber": 12,
+            "referenceNumber": 46,
             "seeAlso": [
                 "https://swift.org/LICENSE.txt",
                 "https://github.com/apple/swift-package-manager/blob/7ab2275f447a5eb37497ed63a9340f8a6d1e488b/LICENSE.txt#L205"
             ]
         },
         {
             "detailsUrl": "./u-boot-exception-2.0.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "u-boot-exception-2.0",
             "name": "U-Boot exception 2.0",
             "reference": "./u-boot-exception-2.0.json",
-            "referenceNumber": 15,
+            "referenceNumber": 5,
             "seeAlso": [
                 "http://git.denx.de/?p=u-boot.git;a=blob;f=Licenses/Exceptions"
             ]
         },
         {
             "detailsUrl": "./Universal-FOSS-exception-1.0.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "Universal-FOSS-exception-1.0",
             "name": "Universal FOSS Exception, Version 1.0",
             "reference": "./Universal-FOSS-exception-1.0.json",
-            "referenceNumber": 22,
+            "referenceNumber": 12,
             "seeAlso": [
                 "https://oss.oracle.com/licenses/universal-foss-exception/"
             ]
         },
         {
+            "detailsUrl": "./vsftpd-openssl-exception.html",
+            "isDeprecatedLicenseId": false,
+            "licenseExceptionId": "vsftpd-openssl-exception",
+            "name": "vsftpd OpenSSL exception",
+            "reference": "./vsftpd-openssl-exception.json",
+            "referenceNumber": 56,
+            "seeAlso": [
+                "https://git.stg.centos.org/source-git/vsftpd/blob/f727873674d9c9cd7afcae6677aa782eb54c8362/f/LICENSE",
+                "https://launchpad.net/debian/squeeze/+source/vsftpd/+copyright",
+                "https://github.com/richardcochran/vsftpd/blob/master/COPYING"
+            ]
+        },
+        {
             "detailsUrl": "./WxWindows-exception-3.1.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "WxWindows-exception-3.1",
             "name": "WxWindows Library Exception 3.1",
             "reference": "./WxWindows-exception-3.1.json",
-            "referenceNumber": 40,
+            "referenceNumber": 25,
             "seeAlso": [
                 "http://www.opensource.org/licenses/WXwindows"
             ]
         },
         {
             "detailsUrl": "./x11vnc-openssl-exception.html",
             "isDeprecatedLicenseId": false,
             "licenseExceptionId": "x11vnc-openssl-exception",
             "name": "x11vnc OpenSSL Exception",
             "reference": "./x11vnc-openssl-exception.json",
-            "referenceNumber": 23,
+            "referenceNumber": 6,
             "seeAlso": [
                 "https://github.com/LibVNC/x11vnc/blob/master/src/8to24.c#L22"
             ]
         }
     ],
-    "licenseListVersion": "3.19",
-    "releaseDate": "2022-11-30"
+    "licenseListVersion": "3.21",
+    "releaseDate": "2023-06-18"
 }
```

### Comparing `reuse-1.1.2/src/reuse/resources/licenses.json` & `reuse-2.0.0/src/reuse/resources/licenses.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6405159086375428%*

 * *Differences: {"'licenseListVersion'": "'3.21'",*

 * * "'licenses'": "{0: {'referenceNumber': 534}, 1: {'referenceNumber': 152}, 2: {'referenceNumber': "*

 * *               "225}, 4: {'referenceNumber': 106}, 5: {'referenceNumber': 92}, 6: "*

 * *               "{'referenceNumber': 73}, 7: {'referenceNumber': 463}, 8: {'referenceNumber': 306}, "*

 * *               "9: {'referenceNumber': 154}, 10: {'referenceNumber': 305}, 11: {'referenceNumber': "*

 * *               "502}, 12: {'referenceNumber': 111}, 13: {'referenceNumber': 256}, 14: "*

 * *    […]*

```diff
@@ -1,2063 +1,2263 @@
 {
-    "licenseListVersion": "3.19",
+    "licenseListVersion": "3.21",
     "licenses": [
         {
             "detailsUrl": "https://spdx.org/licenses/0BSD.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "0BSD",
             "name": "BSD Zero Clause License",
             "reference": "https://spdx.org/licenses/0BSD.html",
-            "referenceNumber": 280,
+            "referenceNumber": 534,
             "seeAlso": [
                 "http://landley.net/toybox/license.html",
                 "https://opensource.org/licenses/0BSD"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/AAL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "AAL",
             "name": "Attribution Assurance License",
             "reference": "https://spdx.org/licenses/AAL.html",
-            "referenceNumber": 340,
+            "referenceNumber": 152,
             "seeAlso": [
                 "https://opensource.org/licenses/attribution"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Abstyles.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Abstyles",
             "name": "Abstyles License",
             "reference": "https://spdx.org/licenses/Abstyles.html",
-            "referenceNumber": 418,
+            "referenceNumber": 225,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Abstyles"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/AdaCore-doc.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "AdaCore-doc",
+            "name": "AdaCore Doc License",
+            "reference": "https://spdx.org/licenses/AdaCore-doc.html",
+            "referenceNumber": 396,
+            "seeAlso": [
+                "https://github.com/AdaCore/xmlada/blob/master/docs/index.rst",
+                "https://github.com/AdaCore/gnatcoll-core/blob/master/docs/index.rst",
+                "https://github.com/AdaCore/gnatcoll-db/blob/master/docs/index.rst"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Adobe-2006.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Adobe-2006",
             "name": "Adobe Systems Incorporated Source Code License Agreement",
             "reference": "https://spdx.org/licenses/Adobe-2006.html",
-            "referenceNumber": 243,
+            "referenceNumber": 106,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/AdobeLicense"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Adobe-Glyph.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Adobe-Glyph",
             "name": "Adobe Glyph List License",
             "reference": "https://spdx.org/licenses/Adobe-Glyph.html",
-            "referenceNumber": 246,
+            "referenceNumber": 92,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/MIT#AdobeGlyph"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/ADSL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "ADSL",
             "name": "Amazon Digital Services License",
             "reference": "https://spdx.org/licenses/ADSL.html",
-            "referenceNumber": 173,
+            "referenceNumber": 73,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/AmazonDigitalServicesLicense"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/AFL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "AFL-1.1",
             "name": "Academic Free License v1.1",
             "reference": "https://spdx.org/licenses/AFL-1.1.html",
-            "referenceNumber": 245,
+            "referenceNumber": 463,
             "seeAlso": [
                 "http://opensource.linux-mirror.org/licenses/afl-1.1.txt",
                 "http://wayback.archive.org/web/20021004124254/http://www.opensource.org/licenses/academic.php"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/AFL-1.2.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "AFL-1.2",
             "name": "Academic Free License v1.2",
             "reference": "https://spdx.org/licenses/AFL-1.2.html",
-            "referenceNumber": 447,
+            "referenceNumber": 306,
             "seeAlso": [
                 "http://opensource.linux-mirror.org/licenses/afl-1.2.txt",
                 "http://wayback.archive.org/web/20021204204652/http://www.opensource.org/licenses/academic.php"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/AFL-2.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "AFL-2.0",
             "name": "Academic Free License v2.0",
             "reference": "https://spdx.org/licenses/AFL-2.0.html",
-            "referenceNumber": 476,
+            "referenceNumber": 154,
             "seeAlso": [
                 "http://wayback.archive.org/web/20060924134533/http://www.opensource.org/licenses/afl-2.0.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/AFL-2.1.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "AFL-2.1",
             "name": "Academic Free License v2.1",
             "reference": "https://spdx.org/licenses/AFL-2.1.html",
-            "referenceNumber": 358,
+            "referenceNumber": 305,
             "seeAlso": [
                 "http://opensource.linux-mirror.org/licenses/afl-2.1.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/AFL-3.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "AFL-3.0",
             "name": "Academic Free License v3.0",
             "reference": "https://spdx.org/licenses/AFL-3.0.html",
-            "referenceNumber": 444,
+            "referenceNumber": 502,
             "seeAlso": [
                 "http://www.rosenlaw.com/AFL3.0.htm",
                 "https://opensource.org/licenses/afl-3.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Afmparse.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Afmparse",
             "name": "Afmparse License",
             "reference": "https://spdx.org/licenses/Afmparse.html",
-            "referenceNumber": 310,
+            "referenceNumber": 111,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Afmparse"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/AGPL-1.0.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "AGPL-1.0",
             "name": "Affero General Public License v1.0",
             "reference": "https://spdx.org/licenses/AGPL-1.0.html",
-            "referenceNumber": 78,
+            "referenceNumber": 256,
             "seeAlso": [
                 "http://www.affero.org/oagpl.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/AGPL-1.0-only.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "AGPL-1.0-only",
             "name": "Affero General Public License v1.0 only",
             "reference": "https://spdx.org/licenses/AGPL-1.0-only.html",
-            "referenceNumber": 350,
+            "referenceNumber": 389,
             "seeAlso": [
                 "http://www.affero.org/oagpl.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/AGPL-1.0-or-later.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "AGPL-1.0-or-later",
             "name": "Affero General Public License v1.0 or later",
             "reference": "https://spdx.org/licenses/AGPL-1.0-or-later.html",
-            "referenceNumber": 360,
+            "referenceNumber": 35,
             "seeAlso": [
                 "http://www.affero.org/oagpl.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/AGPL-3.0.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "AGPL-3.0",
             "name": "GNU Affero General Public License v3.0",
             "reference": "https://spdx.org/licenses/AGPL-3.0.html",
-            "referenceNumber": 180,
+            "referenceNumber": 232,
             "seeAlso": [
                 "https://www.gnu.org/licenses/agpl.txt",
                 "https://opensource.org/licenses/AGPL-3.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/AGPL-3.0-only.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "AGPL-3.0-only",
             "name": "GNU Affero General Public License v3.0 only",
             "reference": "https://spdx.org/licenses/AGPL-3.0-only.html",
-            "referenceNumber": 404,
+            "referenceNumber": 34,
             "seeAlso": [
                 "https://www.gnu.org/licenses/agpl.txt",
                 "https://opensource.org/licenses/AGPL-3.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/AGPL-3.0-or-later.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "AGPL-3.0-or-later",
             "name": "GNU Affero General Public License v3.0 or later",
             "reference": "https://spdx.org/licenses/AGPL-3.0-or-later.html",
-            "referenceNumber": 306,
+            "referenceNumber": 217,
             "seeAlso": [
                 "https://www.gnu.org/licenses/agpl.txt",
                 "https://opensource.org/licenses/AGPL-3.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Aladdin.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": false,
             "licenseId": "Aladdin",
             "name": "Aladdin Free Public License",
             "reference": "https://spdx.org/licenses/Aladdin.html",
-            "referenceNumber": 80,
+            "referenceNumber": 63,
             "seeAlso": [
                 "http://pages.cs.wisc.edu/~ghost/doc/AFPL/6.01/Public.htm"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/AMDPLPA.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "AMDPLPA",
             "name": "AMD's plpa_map.c License",
             "reference": "https://spdx.org/licenses/AMDPLPA.html",
-            "referenceNumber": 74,
+            "referenceNumber": 386,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/AMD_plpa_map_License"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/AML.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "AML",
             "name": "Apple MIT License",
             "reference": "https://spdx.org/licenses/AML.html",
-            "referenceNumber": 204,
+            "referenceNumber": 147,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Apple_MIT_License"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/AMPAS.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "AMPAS",
             "name": "Academy of Motion Picture Arts and Sciences BSD",
             "reference": "https://spdx.org/licenses/AMPAS.html",
-            "referenceNumber": 250,
+            "referenceNumber": 90,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/BSD#AMPASBSD"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/ANTLR-PD.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "ANTLR-PD",
             "name": "ANTLR Software Rights Notice",
             "reference": "https://spdx.org/licenses/ANTLR-PD.html",
-            "referenceNumber": 326,
+            "referenceNumber": 448,
             "seeAlso": [
                 "http://www.antlr2.org/license.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/ANTLR-PD-fallback.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "ANTLR-PD-fallback",
             "name": "ANTLR Software Rights Notice with license fallback",
             "reference": "https://spdx.org/licenses/ANTLR-PD-fallback.html",
-            "referenceNumber": 72,
+            "referenceNumber": 201,
             "seeAlso": [
                 "http://www.antlr2.org/license.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Apache-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "Apache-1.0",
             "name": "Apache License 1.0",
             "reference": "https://spdx.org/licenses/Apache-1.0.html",
-            "referenceNumber": 238,
+            "referenceNumber": 434,
             "seeAlso": [
                 "http://www.apache.org/licenses/LICENSE-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Apache-1.1.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "Apache-1.1",
             "name": "Apache License 1.1",
             "reference": "https://spdx.org/licenses/Apache-1.1.html",
-            "referenceNumber": 202,
+            "referenceNumber": 524,
             "seeAlso": [
                 "http://apache.org/licenses/LICENSE-1.1",
                 "https://opensource.org/licenses/Apache-1.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Apache-2.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "Apache-2.0",
             "name": "Apache License 2.0",
             "reference": "https://spdx.org/licenses/Apache-2.0.html",
-            "referenceNumber": 347,
+            "referenceNumber": 264,
             "seeAlso": [
                 "https://www.apache.org/licenses/LICENSE-2.0",
                 "https://opensource.org/licenses/Apache-2.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/APAFML.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "APAFML",
             "name": "Adobe Postscript AFM License",
             "reference": "https://spdx.org/licenses/APAFML.html",
-            "referenceNumber": 4,
+            "referenceNumber": 184,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/AdobePostscriptAFM"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/APL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "APL-1.0",
             "name": "Adaptive Public License 1.0",
             "reference": "https://spdx.org/licenses/APL-1.0.html",
-            "referenceNumber": 483,
+            "referenceNumber": 410,
             "seeAlso": [
                 "https://opensource.org/licenses/APL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/App-s2p.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "App-s2p",
             "name": "App::s2p License",
             "reference": "https://spdx.org/licenses/App-s2p.html",
-            "referenceNumber": 334,
+            "referenceNumber": 150,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/App-s2p"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/APSL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": true,
             "licenseId": "APSL-1.0",
             "name": "Apple Public Source License 1.0",
             "reference": "https://spdx.org/licenses/APSL-1.0.html",
-            "referenceNumber": 244,
+            "referenceNumber": 177,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Apple_Public_Source_License_1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/APSL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "APSL-1.1",
             "name": "Apple Public Source License 1.1",
             "reference": "https://spdx.org/licenses/APSL-1.1.html",
-            "referenceNumber": 425,
+            "referenceNumber": 536,
             "seeAlso": [
                 "http://www.opensource.apple.com/source/IOSerialFamily/IOSerialFamily-7/APPLE_LICENSE"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/APSL-1.2.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "APSL-1.2",
             "name": "Apple Public Source License 1.2",
             "reference": "https://spdx.org/licenses/APSL-1.2.html",
-            "referenceNumber": 209,
+            "referenceNumber": 479,
             "seeAlso": [
                 "http://www.samurajdata.se/opensource/mirror/licenses/apsl.php"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/APSL-2.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "APSL-2.0",
             "name": "Apple Public Source License 2.0",
             "reference": "https://spdx.org/licenses/APSL-2.0.html",
-            "referenceNumber": 451,
+            "referenceNumber": 183,
             "seeAlso": [
                 "http://www.opensource.apple.com/license/apsl/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Arphic-1999.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Arphic-1999",
             "name": "Arphic Public License",
             "reference": "https://spdx.org/licenses/Arphic-1999.html",
-            "referenceNumber": 149,
+            "referenceNumber": 78,
             "seeAlso": [
                 "http://ftp.gnu.org/gnu/non-gnu/chinese-fonts-truetype/LICENSE"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Artistic-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": true,
             "licenseId": "Artistic-1.0",
             "name": "Artistic License 1.0",
             "reference": "https://spdx.org/licenses/Artistic-1.0.html",
-            "referenceNumber": 213,
+            "referenceNumber": 282,
             "seeAlso": [
                 "https://opensource.org/licenses/Artistic-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Artistic-1.0-cl8.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "Artistic-1.0-cl8",
             "name": "Artistic License 1.0 w/clause 8",
             "reference": "https://spdx.org/licenses/Artistic-1.0-cl8.html",
-            "referenceNumber": 227,
+            "referenceNumber": 210,
             "seeAlso": [
                 "https://opensource.org/licenses/Artistic-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Artistic-1.0-Perl.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "Artistic-1.0-Perl",
             "name": "Artistic License 1.0 (Perl)",
             "reference": "https://spdx.org/licenses/Artistic-1.0-Perl.html",
-            "referenceNumber": 459,
+            "referenceNumber": 550,
             "seeAlso": [
                 "http://dev.perl.org/licenses/artistic.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Artistic-2.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "Artistic-2.0",
             "name": "Artistic License 2.0",
             "reference": "https://spdx.org/licenses/Artistic-2.0.html",
-            "referenceNumber": 452,
+            "referenceNumber": 148,
             "seeAlso": [
                 "http://www.perlfoundation.org/artistic_license_2_0",
                 "https://www.perlfoundation.org/artistic-license-20.html",
                 "https://opensource.org/licenses/artistic-license-2.0"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/ASWF-Digital-Assets-1.0.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "ASWF-Digital-Assets-1.0",
+            "name": "ASWF Digital Assets License version 1.0",
+            "reference": "https://spdx.org/licenses/ASWF-Digital-Assets-1.0.html",
+            "referenceNumber": 277,
+            "seeAlso": [
+                "https://github.com/AcademySoftwareFoundation/foundation/blob/main/digital_assets/aswf_digital_assets_license_v1.0.txt"
+            ]
+        },
+        {
+            "detailsUrl": "https://spdx.org/licenses/ASWF-Digital-Assets-1.1.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "ASWF-Digital-Assets-1.1",
+            "name": "ASWF Digital Assets License 1.1",
+            "reference": "https://spdx.org/licenses/ASWF-Digital-Assets-1.1.html",
+            "referenceNumber": 266,
+            "seeAlso": [
+                "https://github.com/AcademySoftwareFoundation/foundation/blob/main/digital_assets/aswf_digital_assets_license_v1.1.txt"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Baekmuk.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Baekmuk",
             "name": "Baekmuk License",
             "reference": "https://spdx.org/licenses/Baekmuk.html",
-            "referenceNumber": 81,
+            "referenceNumber": 76,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing:Baekmuk?rd=Licensing/Baekmuk"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Bahyph.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Bahyph",
             "name": "Bahyph License",
             "reference": "https://spdx.org/licenses/Bahyph.html",
-            "referenceNumber": 417,
+            "referenceNumber": 4,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Bahyph"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Barr.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Barr",
             "name": "Barr License",
             "reference": "https://spdx.org/licenses/Barr.html",
-            "referenceNumber": 156,
+            "referenceNumber": 401,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Barr"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Beerware.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Beerware",
             "name": "Beerware License",
             "reference": "https://spdx.org/licenses/Beerware.html",
-            "referenceNumber": 76,
+            "referenceNumber": 487,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Beerware",
                 "https://people.freebsd.org/~phk/"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/Bitstream-Charter.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Bitstream-Charter",
+            "name": "Bitstream Charter Font License",
+            "reference": "https://spdx.org/licenses/Bitstream-Charter.html",
+            "referenceNumber": 175,
+            "seeAlso": [
+                "https://fedoraproject.org/wiki/Licensing/Charter#License_Text",
+                "https://raw.githubusercontent.com/blackhole89/notekit/master/data/fonts/Charter%20license.txt"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Bitstream-Vera.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Bitstream-Vera",
             "name": "Bitstream Vera Font License",
             "reference": "https://spdx.org/licenses/Bitstream-Vera.html",
-            "referenceNumber": 31,
+            "referenceNumber": 505,
             "seeAlso": [
                 "https://web.archive.org/web/20080207013128/http://www.gnome.org/fonts/",
                 "https://docubrain.com/sites/default/files/licenses/bitstream-vera.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BitTorrent-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "BitTorrent-1.0",
             "name": "BitTorrent Open Source License v1.0",
             "reference": "https://spdx.org/licenses/BitTorrent-1.0.html",
-            "referenceNumber": 442,
+            "referenceNumber": 500,
             "seeAlso": [
                 "http://sources.gentoo.org/cgi-bin/viewvc.cgi/gentoo-x86/licenses/BitTorrent?r1=1.1&r2=1.1.1.1&diff_format=s"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BitTorrent-1.1.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "BitTorrent-1.1",
             "name": "BitTorrent Open Source License v1.1",
             "reference": "https://spdx.org/licenses/BitTorrent-1.1.html",
-            "referenceNumber": 393,
+            "referenceNumber": 77,
             "seeAlso": [
                 "http://directory.fsf.org/wiki/License:BitTorrentOSL1.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/blessing.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "blessing",
             "name": "SQLite Blessing",
             "reference": "https://spdx.org/licenses/blessing.html",
-            "referenceNumber": 433,
+            "referenceNumber": 444,
             "seeAlso": [
                 "https://www.sqlite.org/src/artifact/e33a4df7e32d742a?ln=4-9",
                 "https://sqlite.org/src/artifact/df5091916dbb40e6"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BlueOak-1.0.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "BlueOak-1.0.0",
             "name": "Blue Oak Model License 1.0.0",
             "reference": "https://spdx.org/licenses/BlueOak-1.0.0.html",
-            "referenceNumber": 485,
+            "referenceNumber": 428,
             "seeAlso": [
                 "https://blueoakcouncil.org/license/1.0.0"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/Boehm-GC.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Boehm-GC",
+            "name": "Boehm-Demers-Weiser GC License",
+            "reference": "https://spdx.org/licenses/Boehm-GC.html",
+            "referenceNumber": 314,
+            "seeAlso": [
+                "https://fedoraproject.org/wiki/Licensing:MIT#Another_Minimal_variant_(found_in_libatomic_ops)",
+                "https://github.com/uim/libgcroots/blob/master/COPYING",
+                "https://github.com/ivmai/libatomic_ops/blob/master/LICENSE"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Borceux.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Borceux",
             "name": "Borceux license",
             "reference": "https://spdx.org/licenses/Borceux.html",
-            "referenceNumber": 130,
+            "referenceNumber": 327,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Borceux"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/Brian-Gladman-3-Clause.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Brian-Gladman-3-Clause",
+            "name": "Brian Gladman 3-Clause License",
+            "reference": "https://spdx.org/licenses/Brian-Gladman-3-Clause.html",
+            "referenceNumber": 131,
+            "seeAlso": [
+                "https://github.com/SWI-Prolog/packages-clib/blob/master/sha1/brg_endian.h"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/BSD-1-Clause.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "BSD-1-Clause",
             "name": "BSD 1-Clause License",
             "reference": "https://spdx.org/licenses/BSD-1-Clause.html",
-            "referenceNumber": 186,
+            "referenceNumber": 200,
             "seeAlso": [
                 "https://svnweb.freebsd.org/base/head/include/ifaddrs.h?revision=326823"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-2-Clause.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "BSD-2-Clause",
             "name": "BSD 2-Clause \"Simplified\" License",
             "reference": "https://spdx.org/licenses/BSD-2-Clause.html",
-            "referenceNumber": 408,
+            "referenceNumber": 269,
             "seeAlso": [
                 "https://opensource.org/licenses/BSD-2-Clause"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-2-Clause-FreeBSD.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "BSD-2-Clause-FreeBSD",
             "name": "BSD 2-Clause FreeBSD License",
             "reference": "https://spdx.org/licenses/BSD-2-Clause-FreeBSD.html",
-            "referenceNumber": 82,
+            "referenceNumber": 22,
             "seeAlso": [
                 "http://www.freebsd.org/copyright/freebsd-license.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-2-Clause-NetBSD.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "BSD-2-Clause-NetBSD",
             "name": "BSD 2-Clause NetBSD License",
             "reference": "https://spdx.org/licenses/BSD-2-Clause-NetBSD.html",
-            "referenceNumber": 464,
+            "referenceNumber": 365,
             "seeAlso": [
                 "http://www.netbsd.org/about/redistribution.html#default"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-2-Clause-Patent.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "BSD-2-Clause-Patent",
             "name": "BSD-2-Clause Plus Patent License",
             "reference": "https://spdx.org/licenses/BSD-2-Clause-Patent.html",
-            "referenceNumber": 236,
+            "referenceNumber": 494,
             "seeAlso": [
                 "https://opensource.org/licenses/BSDplusPatent"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-2-Clause-Views.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "BSD-2-Clause-Views",
             "name": "BSD 2-Clause with views sentence",
             "reference": "https://spdx.org/licenses/BSD-2-Clause-Views.html",
-            "referenceNumber": 184,
+            "referenceNumber": 552,
             "seeAlso": [
                 "http://www.freebsd.org/copyright/freebsd-license.html",
                 "https://people.freebsd.org/~ivoras/wine/patch-wine-nvidia.sh",
                 "https://github.com/protegeproject/protege/blob/master/license.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-3-Clause.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "BSD-3-Clause",
             "name": "BSD 3-Clause \"New\" or \"Revised\" License",
             "reference": "https://spdx.org/licenses/BSD-3-Clause.html",
-            "referenceNumber": 303,
+            "referenceNumber": 320,
             "seeAlso": [
                 "https://opensource.org/licenses/BSD-3-Clause",
                 "https://www.eclipse.org/org/documents/edl-v10.php"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-3-Clause-Attribution.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "BSD-3-Clause-Attribution",
             "name": "BSD with attribution",
             "reference": "https://spdx.org/licenses/BSD-3-Clause-Attribution.html",
-            "referenceNumber": 111,
+            "referenceNumber": 195,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/BSD_with_Attribution"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-3-Clause-Clear.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "BSD-3-Clause-Clear",
             "name": "BSD 3-Clause Clear License",
             "reference": "https://spdx.org/licenses/BSD-3-Clause-Clear.html",
-            "referenceNumber": 490,
+            "referenceNumber": 233,
             "seeAlso": [
                 "http://labs.metacarta.com/license-explanation.html#license"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-3-Clause-LBNL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "BSD-3-Clause-LBNL",
             "name": "Lawrence Berkeley National Labs BSD variant license",
             "reference": "https://spdx.org/licenses/BSD-3-Clause-LBNL.html",
-            "referenceNumber": 489,
+            "referenceNumber": 45,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/LBNLBSD"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-3-Clause-Modification.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "BSD-3-Clause-Modification",
             "name": "BSD 3-Clause Modification",
             "reference": "https://spdx.org/licenses/BSD-3-Clause-Modification.html",
-            "referenceNumber": 88,
+            "referenceNumber": 202,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing:BSD#Modification_Variant"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-3-Clause-No-Military-License.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "BSD-3-Clause-No-Military-License",
             "name": "BSD 3-Clause No Military License",
             "reference": "https://spdx.org/licenses/BSD-3-Clause-No-Military-License.html",
-            "referenceNumber": 270,
+            "referenceNumber": 341,
             "seeAlso": [
                 "https://gitlab.syncad.com/hive/dhive/-/blob/master/LICENSE",
                 "https://github.com/greymass/swift-eosio/blob/master/LICENSE"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-3-Clause-No-Nuclear-License.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "BSD-3-Clause-No-Nuclear-License",
             "name": "BSD 3-Clause No Nuclear License",
             "reference": "https://spdx.org/licenses/BSD-3-Clause-No-Nuclear-License.html",
-            "referenceNumber": 466,
+            "referenceNumber": 331,
             "seeAlso": [
                 "http://download.oracle.com/otn-pub/java/licenses/bsd.txt?AuthParam=1467140197_43d516ce1776bd08a58235a7785be1cc"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-3-Clause-No-Nuclear-License-2014.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "BSD-3-Clause-No-Nuclear-License-2014",
             "name": "BSD 3-Clause No Nuclear License 2014",
             "reference": "https://spdx.org/licenses/BSD-3-Clause-No-Nuclear-License-2014.html",
-            "referenceNumber": 256,
+            "referenceNumber": 442,
             "seeAlso": [
                 "https://java.net/projects/javaeetutorial/pages/BerkeleyLicense"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-3-Clause-No-Nuclear-Warranty.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "BSD-3-Clause-No-Nuclear-Warranty",
             "name": "BSD 3-Clause No Nuclear Warranty",
             "reference": "https://spdx.org/licenses/BSD-3-Clause-No-Nuclear-Warranty.html",
-            "referenceNumber": 472,
+            "referenceNumber": 79,
             "seeAlso": [
                 "https://jogamp.org/git/?p=gluegen.git;a=blob_plain;f=LICENSE.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-3-Clause-Open-MPI.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "BSD-3-Clause-Open-MPI",
             "name": "BSD 3-Clause Open MPI variant",
             "reference": "https://spdx.org/licenses/BSD-3-Clause-Open-MPI.html",
-            "referenceNumber": 435,
+            "referenceNumber": 483,
             "seeAlso": [
                 "https://www.open-mpi.org/community/license.php",
                 "http://www.netlib.org/lapack/LICENSE.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-4-Clause.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "BSD-4-Clause",
             "name": "BSD 4-Clause \"Original\" or \"Old\" License",
             "reference": "https://spdx.org/licenses/BSD-4-Clause.html",
-            "referenceNumber": 498,
+            "referenceNumber": 471,
             "seeAlso": [
                 "http://directory.fsf.org/wiki/License:BSD_4Clause"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-4-Clause-Shortened.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "BSD-4-Clause-Shortened",
             "name": "BSD 4 Clause Shortened",
             "reference": "https://spdx.org/licenses/BSD-4-Clause-Shortened.html",
-            "referenceNumber": 190,
+            "referenceNumber": 41,
             "seeAlso": [
                 "https://metadata.ftp-master.debian.org/changelogs//main/a/arpwatch/arpwatch_2.1a15-7_copyright"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-4-Clause-UC.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "BSD-4-Clause-UC",
             "name": "BSD-4-Clause (University of California-Specific)",
             "reference": "https://spdx.org/licenses/BSD-4-Clause-UC.html",
-            "referenceNumber": 344,
+            "referenceNumber": 160,
             "seeAlso": [
                 "http://www.freebsd.org/copyright/license.html"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/BSD-4.3RENO.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "BSD-4.3RENO",
+            "name": "BSD 4.3 RENO License",
+            "reference": "https://spdx.org/licenses/BSD-4.3RENO.html",
+            "referenceNumber": 130,
+            "seeAlso": [
+                "https://sourceware.org/git/?p=binutils-gdb.git;a=blob;f=libiberty/strcasecmp.c;h=131d81c2ce7881fa48c363dc5bf5fb302c61ce0b;hb=HEAD"
+            ]
+        },
+        {
+            "detailsUrl": "https://spdx.org/licenses/BSD-4.3TAHOE.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "BSD-4.3TAHOE",
+            "name": "BSD 4.3 TAHOE License",
+            "reference": "https://spdx.org/licenses/BSD-4.3TAHOE.html",
+            "referenceNumber": 507,
+            "seeAlso": [
+                "https://github.com/389ds/389-ds-base/blob/main/ldap/include/sysexits-compat.h#L15",
+                "https://git.savannah.gnu.org/cgit/indent.git/tree/doc/indent.texi?id=a74c6b4ee49397cf330b333da1042bffa60ed14f#n1788"
+            ]
+        },
+        {
+            "detailsUrl": "https://spdx.org/licenses/BSD-Advertising-Acknowledgement.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "BSD-Advertising-Acknowledgement",
+            "name": "BSD Advertising Acknowledgement License",
+            "reference": "https://spdx.org/licenses/BSD-Advertising-Acknowledgement.html",
+            "referenceNumber": 367,
+            "seeAlso": [
+                "https://github.com/python-excel/xlrd/blob/master/LICENSE#L33"
+            ]
+        },
+        {
+            "detailsUrl": "https://spdx.org/licenses/BSD-Attribution-HPND-disclaimer.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "BSD-Attribution-HPND-disclaimer",
+            "name": "BSD with Attribution and HPND disclaimer",
+            "reference": "https://spdx.org/licenses/BSD-Attribution-HPND-disclaimer.html",
+            "referenceNumber": 280,
+            "seeAlso": [
+                "https://github.com/cyrusimap/cyrus-sasl/blob/master/COPYING"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/BSD-Protection.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "BSD-Protection",
             "name": "BSD Protection License",
             "reference": "https://spdx.org/licenses/BSD-Protection.html",
-            "referenceNumber": 364,
+            "referenceNumber": 126,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/BSD_Protection_License"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSD-Source-Code.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "BSD-Source-Code",
             "name": "BSD Source Code Attribution",
             "reference": "https://spdx.org/licenses/BSD-Source-Code.html",
-            "referenceNumber": 266,
+            "referenceNumber": 397,
             "seeAlso": [
                 "https://github.com/robbiehanson/CocoaHTTPServer/blob/master/LICENSE.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BSL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "BSL-1.0",
             "name": "Boost Software License 1.0",
             "reference": "https://spdx.org/licenses/BSL-1.0.html",
-            "referenceNumber": 203,
+            "referenceNumber": 467,
             "seeAlso": [
                 "http://www.boost.org/LICENSE_1_0.txt",
                 "https://opensource.org/licenses/BSL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/BUSL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "BUSL-1.1",
             "name": "Business Source License 1.1",
             "reference": "https://spdx.org/licenses/BUSL-1.1.html",
-            "referenceNumber": 165,
+            "referenceNumber": 255,
             "seeAlso": [
                 "https://mariadb.com/bsl11/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/bzip2-1.0.5.json",
             "isDeprecatedLicenseId": true,
             "isOsiApproved": false,
             "licenseId": "bzip2-1.0.5",
             "name": "bzip2 and libbzip2 License v1.0.5",
             "reference": "https://spdx.org/licenses/bzip2-1.0.5.html",
-            "referenceNumber": 15,
+            "referenceNumber": 245,
             "seeAlso": [
                 "https://sourceware.org/bzip2/1.0.5/bzip2-manual-1.0.5.html",
                 "http://bzip.org/1.0.5/bzip2-manual-1.0.5.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/bzip2-1.0.6.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "bzip2-1.0.6",
             "name": "bzip2 and libbzip2 License v1.0.6",
             "reference": "https://spdx.org/licenses/bzip2-1.0.6.html",
-            "referenceNumber": 37,
+            "referenceNumber": 392,
             "seeAlso": [
                 "https://sourceware.org/git/?p=bzip2.git;a=blob;f=LICENSE;hb=bzip2-1.0.6",
                 "http://bzip.org/1.0.5/bzip2-manual-1.0.5.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/C-UDA-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "C-UDA-1.0",
             "name": "Computational Use of Data Agreement v1.0",
             "reference": "https://spdx.org/licenses/C-UDA-1.0.html",
-            "referenceNumber": 212,
+            "referenceNumber": 191,
             "seeAlso": [
                 "https://github.com/microsoft/Computational-Use-of-Data-Agreement/blob/master/C-UDA-1.0.md",
                 "https://cdla.dev/computational-use-of-data-agreement-v1-0/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CAL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "CAL-1.0",
             "name": "Cryptographic Autonomy License 1.0",
             "reference": "https://spdx.org/licenses/CAL-1.0.html",
-            "referenceNumber": 499,
+            "referenceNumber": 551,
             "seeAlso": [
                 "http://cryptographicautonomylicense.com/license-text.html",
                 "https://opensource.org/licenses/CAL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CAL-1.0-Combined-Work-Exception.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "CAL-1.0-Combined-Work-Exception",
             "name": "Cryptographic Autonomy License 1.0 (Combined Work Exception)",
             "reference": "https://spdx.org/licenses/CAL-1.0-Combined-Work-Exception.html",
-            "referenceNumber": 429,
+            "referenceNumber": 316,
             "seeAlso": [
                 "http://cryptographicautonomylicense.com/license-text.html",
                 "https://opensource.org/licenses/CAL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Caldera.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Caldera",
             "name": "Caldera License",
             "reference": "https://spdx.org/licenses/Caldera.html",
-            "referenceNumber": 123,
+            "referenceNumber": 178,
             "seeAlso": [
                 "http://www.lemis.com/grog/UNIX/ancient-source-all.pdf"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CATOSL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "CATOSL-1.1",
             "name": "Computer Associates Trusted Open Source License 1.1",
             "reference": "https://spdx.org/licenses/CATOSL-1.1.html",
-            "referenceNumber": 122,
+            "referenceNumber": 253,
             "seeAlso": [
                 "https://opensource.org/licenses/CATOSL-1.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-1.0",
             "name": "Creative Commons Attribution 1.0 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-1.0.html",
-            "referenceNumber": 21,
+            "referenceNumber": 205,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by/1.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-2.0",
             "name": "Creative Commons Attribution 2.0 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-2.0.html",
-            "referenceNumber": 383,
+            "referenceNumber": 61,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by/2.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-2.5.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-2.5",
             "name": "Creative Commons Attribution 2.5 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-2.5.html",
-            "referenceNumber": 372,
+            "referenceNumber": 171,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by/2.5/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-2.5-AU.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-2.5-AU",
             "name": "Creative Commons Attribution 2.5 Australia",
             "reference": "https://spdx.org/licenses/CC-BY-2.5-AU.html",
-            "referenceNumber": 49,
+            "referenceNumber": 128,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by/2.5/au/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-3.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-3.0",
             "name": "Creative Commons Attribution 3.0 Unported",
             "reference": "https://spdx.org/licenses/CC-BY-3.0.html",
-            "referenceNumber": 394,
+            "referenceNumber": 433,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by/3.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-3.0-AT.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-3.0-AT",
             "name": "Creative Commons Attribution 3.0 Austria",
             "reference": "https://spdx.org/licenses/CC-BY-3.0-AT.html",
-            "referenceNumber": 147,
+            "referenceNumber": 7,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by/3.0/at/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-3.0-DE.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-3.0-DE",
             "name": "Creative Commons Attribution 3.0 Germany",
             "reference": "https://spdx.org/licenses/CC-BY-3.0-DE.html",
-            "referenceNumber": 426,
+            "referenceNumber": 317,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by/3.0/de/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-3.0-IGO.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-3.0-IGO",
             "name": "Creative Commons Attribution 3.0 IGO",
             "reference": "https://spdx.org/licenses/CC-BY-3.0-IGO.html",
-            "referenceNumber": 70,
+            "referenceNumber": 141,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by/3.0/igo/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-3.0-NL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-3.0-NL",
             "name": "Creative Commons Attribution 3.0 Netherlands",
             "reference": "https://spdx.org/licenses/CC-BY-3.0-NL.html",
-            "referenceNumber": 313,
+            "referenceNumber": 193,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by/3.0/nl/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-3.0-US.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-3.0-US",
             "name": "Creative Commons Attribution 3.0 United States",
             "reference": "https://spdx.org/licenses/CC-BY-3.0-US.html",
-            "referenceNumber": 42,
+            "referenceNumber": 156,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by/3.0/us/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-4.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "CC-BY-4.0",
             "name": "Creative Commons Attribution 4.0 International",
             "reference": "https://spdx.org/licenses/CC-BY-4.0.html",
-            "referenceNumber": 309,
+            "referenceNumber": 499,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by/4.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-1.0",
             "name": "Creative Commons Attribution Non Commercial 1.0 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-NC-1.0.html",
-            "referenceNumber": 56,
+            "referenceNumber": 292,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc/1.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-2.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-2.0",
             "name": "Creative Commons Attribution Non Commercial 2.0 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-NC-2.0.html",
-            "referenceNumber": 355,
+            "referenceNumber": 143,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc/2.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-2.5.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-2.5",
             "name": "Creative Commons Attribution Non Commercial 2.5 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-NC-2.5.html",
-            "referenceNumber": 127,
+            "referenceNumber": 457,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc/2.5/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-3.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-3.0",
             "name": "Creative Commons Attribution Non Commercial 3.0 Unported",
             "reference": "https://spdx.org/licenses/CC-BY-NC-3.0.html",
-            "referenceNumber": 491,
+            "referenceNumber": 216,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc/3.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-3.0-DE.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-3.0-DE",
             "name": "Creative Commons Attribution Non Commercial 3.0 Germany",
             "reference": "https://spdx.org/licenses/CC-BY-NC-3.0-DE.html",
-            "referenceNumber": 172,
+            "referenceNumber": 196,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc/3.0/de/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-4.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-4.0",
             "name": "Creative Commons Attribution Non Commercial 4.0 International",
             "reference": "https://spdx.org/licenses/CC-BY-NC-4.0.html",
-            "referenceNumber": 443,
+            "referenceNumber": 248,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc/4.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-ND-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-ND-1.0",
             "name": "Creative Commons Attribution Non Commercial No Derivatives 1.0 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-NC-ND-1.0.html",
-            "referenceNumber": 201,
+            "referenceNumber": 368,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nd-nc/1.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-ND-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-ND-2.0",
             "name": "Creative Commons Attribution Non Commercial No Derivatives 2.0 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-NC-ND-2.0.html",
-            "referenceNumber": 456,
+            "referenceNumber": 462,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc-nd/2.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-ND-2.5.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-ND-2.5",
             "name": "Creative Commons Attribution Non Commercial No Derivatives 2.5 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-NC-ND-2.5.html",
-            "referenceNumber": 225,
+            "referenceNumber": 464,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc-nd/2.5/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-ND-3.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-ND-3.0",
             "name": "Creative Commons Attribution Non Commercial No Derivatives 3.0 Unported",
             "reference": "https://spdx.org/licenses/CC-BY-NC-ND-3.0.html",
-            "referenceNumber": 28,
+            "referenceNumber": 478,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc-nd/3.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-ND-3.0-DE.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-ND-3.0-DE",
             "name": "Creative Commons Attribution Non Commercial No Derivatives 3.0 Germany",
             "reference": "https://spdx.org/licenses/CC-BY-NC-ND-3.0-DE.html",
-            "referenceNumber": 415,
+            "referenceNumber": 384,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc-nd/3.0/de/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-ND-3.0-IGO.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-ND-3.0-IGO",
             "name": "Creative Commons Attribution Non Commercial No Derivatives 3.0 IGO",
             "reference": "https://spdx.org/licenses/CC-BY-NC-ND-3.0-IGO.html",
-            "referenceNumber": 216,
+            "referenceNumber": 211,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc-nd/3.0/igo/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-ND-4.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-ND-4.0",
             "name": "Creative Commons Attribution Non Commercial No Derivatives 4.0 International",
             "reference": "https://spdx.org/licenses/CC-BY-NC-ND-4.0.html",
-            "referenceNumber": 369,
+            "referenceNumber": 466,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc-nd/4.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-SA-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-SA-1.0",
             "name": "Creative Commons Attribution Non Commercial Share Alike 1.0 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-NC-SA-1.0.html",
-            "referenceNumber": 33,
+            "referenceNumber": 132,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc-sa/1.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-SA-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-SA-2.0",
             "name": "Creative Commons Attribution Non Commercial Share Alike 2.0 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-NC-SA-2.0.html",
-            "referenceNumber": 110,
+            "referenceNumber": 420,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc-sa/2.0/legalcode"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-SA-2.0-DE.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "CC-BY-NC-SA-2.0-DE",
+            "name": "Creative Commons Attribution Non Commercial Share Alike 2.0 Germany",
+            "reference": "https://spdx.org/licenses/CC-BY-NC-SA-2.0-DE.html",
+            "referenceNumber": 452,
+            "seeAlso": [
+                "https://creativecommons.org/licenses/by-nc-sa/2.0/de/legalcode"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-SA-2.0-FR.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-SA-2.0-FR",
             "name": "Creative Commons Attribution-NonCommercial-ShareAlike 2.0 France",
             "reference": "https://spdx.org/licenses/CC-BY-NC-SA-2.0-FR.html",
-            "referenceNumber": 382,
+            "referenceNumber": 29,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc-sa/2.0/fr/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-SA-2.0-UK.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-SA-2.0-UK",
             "name": "Creative Commons Attribution Non Commercial Share Alike 2.0 England and Wales",
             "reference": "https://spdx.org/licenses/CC-BY-NC-SA-2.0-UK.html",
-            "referenceNumber": 311,
+            "referenceNumber": 460,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc-sa/2.0/uk/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-SA-2.5.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-SA-2.5",
             "name": "Creative Commons Attribution Non Commercial Share Alike 2.5 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-NC-SA-2.5.html",
-            "referenceNumber": 354,
+            "referenceNumber": 8,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc-sa/2.5/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-SA-3.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-SA-3.0",
             "name": "Creative Commons Attribution Non Commercial Share Alike 3.0 Unported",
             "reference": "https://spdx.org/licenses/CC-BY-NC-SA-3.0.html",
-            "referenceNumber": 45,
+            "referenceNumber": 271,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc-sa/3.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-SA-3.0-DE.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-SA-3.0-DE",
             "name": "Creative Commons Attribution Non Commercial Share Alike 3.0 Germany",
             "reference": "https://spdx.org/licenses/CC-BY-NC-SA-3.0-DE.html",
-            "referenceNumber": 282,
+            "referenceNumber": 504,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc-sa/3.0/de/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-SA-3.0-IGO.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-SA-3.0-IGO",
             "name": "Creative Commons Attribution Non Commercial Share Alike 3.0 IGO",
             "reference": "https://spdx.org/licenses/CC-BY-NC-SA-3.0-IGO.html",
-            "referenceNumber": 337,
+            "referenceNumber": 14,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc-sa/3.0/igo/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-NC-SA-4.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-NC-SA-4.0",
             "name": "Creative Commons Attribution Non Commercial Share Alike 4.0 International",
             "reference": "https://spdx.org/licenses/CC-BY-NC-SA-4.0.html",
-            "referenceNumber": 254,
+            "referenceNumber": 338,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-ND-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-ND-1.0",
             "name": "Creative Commons Attribution No Derivatives 1.0 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-ND-1.0.html",
-            "referenceNumber": 219,
+            "referenceNumber": 115,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nd/1.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-ND-2.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-ND-2.0",
             "name": "Creative Commons Attribution No Derivatives 2.0 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-ND-2.0.html",
-            "referenceNumber": 187,
+            "referenceNumber": 116,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nd/2.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-ND-2.5.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-ND-2.5",
             "name": "Creative Commons Attribution No Derivatives 2.5 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-ND-2.5.html",
-            "referenceNumber": 100,
+            "referenceNumber": 13,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nd/2.5/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-ND-3.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-ND-3.0",
             "name": "Creative Commons Attribution No Derivatives 3.0 Unported",
             "reference": "https://spdx.org/licenses/CC-BY-ND-3.0.html",
-            "referenceNumber": 330,
+            "referenceNumber": 31,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nd/3.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-ND-3.0-DE.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-ND-3.0-DE",
             "name": "Creative Commons Attribution No Derivatives 3.0 Germany",
             "reference": "https://spdx.org/licenses/CC-BY-ND-3.0-DE.html",
-            "referenceNumber": 121,
+            "referenceNumber": 322,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nd/3.0/de/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-ND-4.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-ND-4.0",
             "name": "Creative Commons Attribution No Derivatives 4.0 International",
             "reference": "https://spdx.org/licenses/CC-BY-ND-4.0.html",
-            "referenceNumber": 467,
+            "referenceNumber": 44,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-nd/4.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-SA-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-SA-1.0",
             "name": "Creative Commons Attribution Share Alike 1.0 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-SA-1.0.html",
-            "referenceNumber": 160,
+            "referenceNumber": 71,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-sa/1.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-SA-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-SA-2.0",
             "name": "Creative Commons Attribution Share Alike 2.0 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-SA-2.0.html",
-            "referenceNumber": 305,
+            "referenceNumber": 252,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-sa/2.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-SA-2.0-UK.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-SA-2.0-UK",
             "name": "Creative Commons Attribution Share Alike 2.0 England and Wales",
             "reference": "https://spdx.org/licenses/CC-BY-SA-2.0-UK.html",
-            "referenceNumber": 285,
+            "referenceNumber": 72,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-sa/2.0/uk/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-SA-2.1-JP.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-SA-2.1-JP",
             "name": "Creative Commons Attribution Share Alike 2.1 Japan",
             "reference": "https://spdx.org/licenses/CC-BY-SA-2.1-JP.html",
-            "referenceNumber": 362,
+            "referenceNumber": 54,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-sa/2.1/jp/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-SA-2.5.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-SA-2.5",
             "name": "Creative Commons Attribution Share Alike 2.5 Generic",
             "reference": "https://spdx.org/licenses/CC-BY-SA-2.5.html",
-            "referenceNumber": 241,
+            "referenceNumber": 378,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-sa/2.5/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-SA-3.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-SA-3.0",
             "name": "Creative Commons Attribution Share Alike 3.0 Unported",
             "reference": "https://spdx.org/licenses/CC-BY-SA-3.0.html",
-            "referenceNumber": 385,
+            "referenceNumber": 139,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-sa/3.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-SA-3.0-AT.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-SA-3.0-AT",
             "name": "Creative Commons Attribution Share Alike 3.0 Austria",
             "reference": "https://spdx.org/licenses/CC-BY-SA-3.0-AT.html",
-            "referenceNumber": 153,
+            "referenceNumber": 189,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-sa/3.0/at/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-SA-3.0-DE.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-BY-SA-3.0-DE",
             "name": "Creative Commons Attribution Share Alike 3.0 Germany",
             "reference": "https://spdx.org/licenses/CC-BY-SA-3.0-DE.html",
-            "referenceNumber": 349,
+            "referenceNumber": 385,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-sa/3.0/de/legalcode"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/CC-BY-SA-3.0-IGO.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "CC-BY-SA-3.0-IGO",
+            "name": "Creative Commons Attribution-ShareAlike 3.0 IGO",
+            "reference": "https://spdx.org/licenses/CC-BY-SA-3.0-IGO.html",
+            "referenceNumber": 213,
+            "seeAlso": [
+                "https://creativecommons.org/licenses/by-sa/3.0/igo/legalcode"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/CC-BY-SA-4.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "CC-BY-SA-4.0",
             "name": "Creative Commons Attribution Share Alike 4.0 International",
             "reference": "https://spdx.org/licenses/CC-BY-SA-4.0.html",
-            "referenceNumber": 307,
+            "referenceNumber": 342,
             "seeAlso": [
                 "https://creativecommons.org/licenses/by-sa/4.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC-PDDC.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CC-PDDC",
             "name": "Creative Commons Public Domain Dedication and Certification",
             "reference": "https://spdx.org/licenses/CC-PDDC.html",
-            "referenceNumber": 129,
+            "referenceNumber": 240,
             "seeAlso": [
                 "https://creativecommons.org/licenses/publicdomain/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CC0-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "CC0-1.0",
             "name": "Creative Commons Zero v1.0 Universal",
             "reference": "https://spdx.org/licenses/CC0-1.0.html",
-            "referenceNumber": 191,
+            "referenceNumber": 279,
             "seeAlso": [
                 "https://creativecommons.org/publicdomain/zero/1.0/legalcode"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CDDL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "CDDL-1.0",
             "name": "Common Development and Distribution License 1.0",
             "reference": "https://spdx.org/licenses/CDDL-1.0.html",
-            "referenceNumber": 359,
+            "referenceNumber": 187,
             "seeAlso": [
                 "https://opensource.org/licenses/cddl1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CDDL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CDDL-1.1",
             "name": "Common Development and Distribution License 1.1",
             "reference": "https://spdx.org/licenses/CDDL-1.1.html",
-            "referenceNumber": 351,
+            "referenceNumber": 352,
             "seeAlso": [
                 "http://glassfish.java.net/public/CDDL+GPL_1_1.html",
                 "https://javaee.github.io/glassfish/LICENSE"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CDL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CDL-1.0",
             "name": "Common Documentation License 1.0",
             "reference": "https://spdx.org/licenses/CDL-1.0.html",
-            "referenceNumber": 269,
+            "referenceNumber": 12,
             "seeAlso": [
                 "http://www.opensource.apple.com/cdl/",
                 "https://fedoraproject.org/wiki/Licensing/Common_Documentation_License",
                 "https://www.gnu.org/licenses/license-list.html#ACDL"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CDLA-Permissive-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CDLA-Permissive-1.0",
             "name": "Community Data License Agreement Permissive 1.0",
             "reference": "https://spdx.org/licenses/CDLA-Permissive-1.0.html",
-            "referenceNumber": 154,
+            "referenceNumber": 238,
             "seeAlso": [
                 "https://cdla.io/permissive-1-0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CDLA-Permissive-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CDLA-Permissive-2.0",
             "name": "Community Data License Agreement Permissive 2.0",
             "reference": "https://spdx.org/licenses/CDLA-Permissive-2.0.html",
-            "referenceNumber": 109,
+            "referenceNumber": 270,
             "seeAlso": [
                 "https://cdla.dev/permissive-2-0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CDLA-Sharing-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CDLA-Sharing-1.0",
             "name": "Community Data License Agreement Sharing 1.0",
             "reference": "https://spdx.org/licenses/CDLA-Sharing-1.0.html",
-            "referenceNumber": 343,
+            "referenceNumber": 535,
             "seeAlso": [
                 "https://cdla.io/sharing-1-0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CECILL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CECILL-1.0",
             "name": "CeCILL Free Software License Agreement v1.0",
             "reference": "https://spdx.org/licenses/CECILL-1.0.html",
-            "referenceNumber": 10,
+            "referenceNumber": 376,
             "seeAlso": [
                 "http://www.cecill.info/licences/Licence_CeCILL_V1-fr.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CECILL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CECILL-1.1",
             "name": "CeCILL Free Software License Agreement v1.1",
             "reference": "https://spdx.org/licenses/CECILL-1.1.html",
-            "referenceNumber": 38,
+            "referenceNumber": 522,
             "seeAlso": [
                 "http://www.cecill.info/licences/Licence_CeCILL_V1.1-US.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CECILL-2.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "CECILL-2.0",
             "name": "CeCILL Free Software License Agreement v2.0",
             "reference": "https://spdx.org/licenses/CECILL-2.0.html",
-            "referenceNumber": 144,
+            "referenceNumber": 149,
             "seeAlso": [
                 "http://www.cecill.info/licences/Licence_CeCILL_V2-en.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CECILL-2.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "CECILL-2.1",
             "name": "CeCILL Free Software License Agreement v2.1",
             "reference": "https://spdx.org/licenses/CECILL-2.1.html",
-            "referenceNumber": 423,
+            "referenceNumber": 226,
             "seeAlso": [
                 "http://www.cecill.info/licences/Licence_CeCILL_V2.1-en.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CECILL-B.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "CECILL-B",
             "name": "CeCILL-B Free Software License Agreement",
             "reference": "https://spdx.org/licenses/CECILL-B.html",
-            "referenceNumber": 249,
+            "referenceNumber": 308,
             "seeAlso": [
                 "http://www.cecill.info/licences/Licence_CeCILL-B_V1-en.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CECILL-C.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "CECILL-C",
             "name": "CeCILL-C Free Software License Agreement",
             "reference": "https://spdx.org/licenses/CECILL-C.html",
-            "referenceNumber": 117,
+            "referenceNumber": 129,
             "seeAlso": [
                 "http://www.cecill.info/licences/Licence_CeCILL-C_V1-en.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CERN-OHL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CERN-OHL-1.1",
             "name": "CERN Open Hardware Licence v1.1",
             "reference": "https://spdx.org/licenses/CERN-OHL-1.1.html",
-            "referenceNumber": 302,
+            "referenceNumber": 348,
             "seeAlso": [
                 "https://www.ohwr.org/project/licenses/wikis/cern-ohl-v1.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CERN-OHL-1.2.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CERN-OHL-1.2",
             "name": "CERN Open Hardware Licence v1.2",
             "reference": "https://spdx.org/licenses/CERN-OHL-1.2.html",
-            "referenceNumber": 92,
+            "referenceNumber": 473,
             "seeAlso": [
                 "https://www.ohwr.org/project/licenses/wikis/cern-ohl-v1.2"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CERN-OHL-P-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "CERN-OHL-P-2.0",
             "name": "CERN Open Hardware Licence Version 2 - Permissive",
             "reference": "https://spdx.org/licenses/CERN-OHL-P-2.0.html",
-            "referenceNumber": 136,
+            "referenceNumber": 439,
             "seeAlso": [
                 "https://www.ohwr.org/project/cernohl/wikis/Documents/CERN-OHL-version-2"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CERN-OHL-S-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "CERN-OHL-S-2.0",
             "name": "CERN Open Hardware Licence Version 2 - Strongly Reciprocal",
             "reference": "https://spdx.org/licenses/CERN-OHL-S-2.0.html",
-            "referenceNumber": 342,
+            "referenceNumber": 497,
             "seeAlso": [
                 "https://www.ohwr.org/project/cernohl/wikis/Documents/CERN-OHL-version-2"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CERN-OHL-W-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "CERN-OHL-W-2.0",
             "name": "CERN Open Hardware Licence Version 2 - Weakly Reciprocal",
             "reference": "https://spdx.org/licenses/CERN-OHL-W-2.0.html",
-            "referenceNumber": 91,
+            "referenceNumber": 493,
             "seeAlso": [
                 "https://www.ohwr.org/project/cernohl/wikis/Documents/CERN-OHL-version-2"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/CFITSIO.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "CFITSIO",
+            "name": "CFITSIO License",
+            "reference": "https://spdx.org/licenses/CFITSIO.html",
+            "referenceNumber": 395,
+            "seeAlso": [
+                "https://heasarc.gsfc.nasa.gov/docs/software/fitsio/c/f_user/node9.html"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/checkmk.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "checkmk",
             "name": "Checkmk License",
             "reference": "https://spdx.org/licenses/checkmk.html",
-            "referenceNumber": 221,
+            "referenceNumber": 475,
             "seeAlso": [
                 "https://github.com/libcheck/check/blob/master/checkmk/checkmk.in"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/ClArtistic.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "ClArtistic",
             "name": "Clarified Artistic License",
             "reference": "https://spdx.org/licenses/ClArtistic.html",
-            "referenceNumber": 390,
+            "referenceNumber": 412,
             "seeAlso": [
                 "http://gianluca.dellavedova.org/2011/01/03/clarified-artistic-license/",
                 "http://www.ncftp.com/ncftp/doc/LICENSE.txt"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/Clips.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Clips",
+            "name": "Clips License",
+            "reference": "https://spdx.org/licenses/Clips.html",
+            "referenceNumber": 28,
+            "seeAlso": [
+                "https://github.com/DrItanium/maya/blob/master/LICENSE.CLIPS"
+            ]
+        },
+        {
+            "detailsUrl": "https://spdx.org/licenses/CMU-Mach.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "CMU-Mach",
+            "name": "CMU Mach License",
+            "reference": "https://spdx.org/licenses/CMU-Mach.html",
+            "referenceNumber": 355,
+            "seeAlso": [
+                "https://www.cs.cmu.edu/~410/licenses.html"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/CNRI-Jython.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CNRI-Jython",
             "name": "CNRI Jython License",
             "reference": "https://spdx.org/licenses/CNRI-Jython.html",
-            "referenceNumber": 234,
+            "referenceNumber": 491,
             "seeAlso": [
                 "http://www.jython.org/license.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CNRI-Python.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "CNRI-Python",
             "name": "CNRI Python License",
             "reference": "https://spdx.org/licenses/CNRI-Python.html",
-            "referenceNumber": 346,
+            "referenceNumber": 120,
             "seeAlso": [
                 "https://opensource.org/licenses/CNRI-Python"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CNRI-Python-GPL-Compatible.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CNRI-Python-GPL-Compatible",
             "name": "CNRI Python Open Source GPL Compatible License Agreement",
             "reference": "https://spdx.org/licenses/CNRI-Python-GPL-Compatible.html",
-            "referenceNumber": 263,
+            "referenceNumber": 404,
             "seeAlso": [
                 "http://www.python.org/download/releases/1.6.1/download_win/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/COIL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "COIL-1.0",
             "name": "Copyfree Open Innovation License",
             "reference": "https://spdx.org/licenses/COIL-1.0.html",
-            "referenceNumber": 492,
+            "referenceNumber": 203,
             "seeAlso": [
                 "https://coil.apotheon.org/plaintext/01.0.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Community-Spec-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Community-Spec-1.0",
             "name": "Community Specification License 1.0",
             "reference": "https://spdx.org/licenses/Community-Spec-1.0.html",
-            "referenceNumber": 107,
+            "referenceNumber": 347,
             "seeAlso": [
                 "https://github.com/CommunitySpecification/1.0/blob/master/1._Community_Specification_License-v1.md"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Condor-1.1.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "Condor-1.1",
             "name": "Condor Public License v1.1",
             "reference": "https://spdx.org/licenses/Condor-1.1.html",
-            "referenceNumber": 237,
+            "referenceNumber": 351,
             "seeAlso": [
                 "http://research.cs.wisc.edu/condor/license.html#condor",
                 "http://web.archive.org/web/20111123062036/http://research.cs.wisc.edu/condor/license.html#condor"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/copyleft-next-0.3.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "copyleft-next-0.3.0",
             "name": "copyleft-next 0.3.0",
             "reference": "https://spdx.org/licenses/copyleft-next-0.3.0.html",
-            "referenceNumber": 240,
+            "referenceNumber": 258,
             "seeAlso": [
                 "https://github.com/copyleft-next/copyleft-next/blob/master/Releases/copyleft-next-0.3.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/copyleft-next-0.3.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "copyleft-next-0.3.1",
             "name": "copyleft-next 0.3.1",
             "reference": "https://spdx.org/licenses/copyleft-next-0.3.1.html",
-            "referenceNumber": 198,
+            "referenceNumber": 265,
             "seeAlso": [
                 "https://github.com/copyleft-next/copyleft-next/blob/master/Releases/copyleft-next-0.3.1"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/Cornell-Lossless-JPEG.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Cornell-Lossless-JPEG",
+            "name": "Cornell Lossless JPEG License",
+            "reference": "https://spdx.org/licenses/Cornell-Lossless-JPEG.html",
+            "referenceNumber": 375,
+            "seeAlso": [
+                "https://android.googlesource.com/platform/external/dng_sdk/+/refs/heads/master/source/dng_lossless_jpeg.cpp#16",
+                "https://www.mssl.ucl.ac.uk/~mcrw/src/20050920/proto.h",
+                "https://gitlab.freedesktop.org/libopenraw/libopenraw/blob/master/lib/ljpegdecompressor.cpp#L32"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/CPAL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "CPAL-1.0",
             "name": "Common Public Attribution License 1.0",
             "reference": "https://spdx.org/licenses/CPAL-1.0.html",
-            "referenceNumber": 159,
+            "referenceNumber": 411,
             "seeAlso": [
                 "https://opensource.org/licenses/CPAL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CPL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "CPL-1.0",
             "name": "Common Public License 1.0",
             "reference": "https://spdx.org/licenses/CPL-1.0.html",
-            "referenceNumber": 432,
+            "referenceNumber": 488,
             "seeAlso": [
                 "https://opensource.org/licenses/CPL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CPOL-1.02.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": false,
             "licenseId": "CPOL-1.02",
             "name": "Code Project Open License 1.02",
             "reference": "https://spdx.org/licenses/CPOL-1.02.html",
-            "referenceNumber": 406,
+            "referenceNumber": 381,
             "seeAlso": [
                 "http://www.codeproject.com/info/cpol10.aspx"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Crossword.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Crossword",
             "name": "Crossword License",
             "reference": "https://spdx.org/licenses/Crossword.html",
-            "referenceNumber": 268,
+            "referenceNumber": 260,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Crossword"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CrystalStacker.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "CrystalStacker",
             "name": "CrystalStacker License",
             "reference": "https://spdx.org/licenses/CrystalStacker.html",
-            "referenceNumber": 169,
+            "referenceNumber": 105,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing:CrystalStacker?rd=Licensing/CrystalStacker"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/CUA-OPL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "CUA-OPL-1.0",
             "name": "CUA Office Public License v1.0",
             "reference": "https://spdx.org/licenses/CUA-OPL-1.0.html",
-            "referenceNumber": 341,
+            "referenceNumber": 108,
             "seeAlso": [
                 "https://opensource.org/licenses/CUA-OPL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Cube.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Cube",
             "name": "Cube License",
             "reference": "https://spdx.org/licenses/Cube.html",
-            "referenceNumber": 135,
+            "referenceNumber": 182,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Cube"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/curl.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "curl",
             "name": "curl License",
             "reference": "https://spdx.org/licenses/curl.html",
-            "referenceNumber": 60,
+            "referenceNumber": 332,
             "seeAlso": [
                 "https://github.com/bagder/curl/blob/master/COPYING"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/D-FSL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "D-FSL-1.0",
             "name": "Deutsche Freie Software Lizenz",
             "reference": "https://spdx.org/licenses/D-FSL-1.0.html",
-            "referenceNumber": 8,
+            "referenceNumber": 337,
             "seeAlso": [
                 "http://www.dipp.nrw.de/d-fsl/lizenzen/",
                 "http://www.dipp.nrw.de/d-fsl/index_html/lizenzen/de/D-FSL-1_0_de.txt",
                 "http://www.dipp.nrw.de/d-fsl/index_html/lizenzen/en/D-FSL-1_0_en.txt",
                 "https://www.hbz-nrw.de/produkte/open-access/lizenzen/dfsl",
                 "https://www.hbz-nrw.de/produkte/open-access/lizenzen/dfsl/deutsche-freie-software-lizenz",
                 "https://www.hbz-nrw.de/produkte/open-access/lizenzen/dfsl/german-free-software-license",
@@ -2068,311 +2268,323 @@
         {
             "detailsUrl": "https://spdx.org/licenses/diffmark.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "diffmark",
             "name": "diffmark license",
             "reference": "https://spdx.org/licenses/diffmark.html",
-            "referenceNumber": 171,
+            "referenceNumber": 302,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/diffmark"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/DL-DE-BY-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "DL-DE-BY-2.0",
             "name": "Data licence Germany \u2013 attribution \u2013 version 2.0",
             "reference": "https://spdx.org/licenses/DL-DE-BY-2.0.html",
-            "referenceNumber": 365,
+            "referenceNumber": 93,
             "seeAlso": [
                 "https://www.govdata.de/dl-de/by-2-0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/DOC.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "DOC",
             "name": "DOC License",
             "reference": "https://spdx.org/licenses/DOC.html",
-            "referenceNumber": 1,
+            "referenceNumber": 262,
             "seeAlso": [
                 "http://www.cs.wustl.edu/~schmidt/ACE-copying.html",
                 "https://www.dre.vanderbilt.edu/~schmidt/ACE-copying.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Dotseqn.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Dotseqn",
             "name": "Dotseqn License",
             "reference": "https://spdx.org/licenses/Dotseqn.html",
-            "referenceNumber": 20,
+            "referenceNumber": 95,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Dotseqn"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/DRL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "DRL-1.0",
             "name": "Detection Rule License 1.0",
             "reference": "https://spdx.org/licenses/DRL-1.0.html",
-            "referenceNumber": 345,
+            "referenceNumber": 325,
             "seeAlso": [
                 "https://github.com/Neo23x0/sigma/blob/master/LICENSE.Detection.Rules.md"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/DSDP.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "DSDP",
             "name": "DSDP License",
             "reference": "https://spdx.org/licenses/DSDP.html",
-            "referenceNumber": 25,
+            "referenceNumber": 379,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/DSDP"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/dtoa.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "dtoa",
+            "name": "David M. Gay dtoa License",
+            "reference": "https://spdx.org/licenses/dtoa.html",
+            "referenceNumber": 144,
+            "seeAlso": [
+                "https://github.com/SWI-Prolog/swipl-devel/blob/master/src/os/dtoa.c"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/dvipdfm.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "dvipdfm",
             "name": "dvipdfm License",
             "reference": "https://spdx.org/licenses/dvipdfm.html",
-            "referenceNumber": 134,
+            "referenceNumber": 289,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/dvipdfm"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/ECL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "ECL-1.0",
             "name": "Educational Community License v1.0",
             "reference": "https://spdx.org/licenses/ECL-1.0.html",
-            "referenceNumber": 375,
+            "referenceNumber": 242,
             "seeAlso": [
                 "https://opensource.org/licenses/ECL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/ECL-2.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "ECL-2.0",
             "name": "Educational Community License v2.0",
             "reference": "https://spdx.org/licenses/ECL-2.0.html",
-            "referenceNumber": 133,
+            "referenceNumber": 246,
             "seeAlso": [
                 "https://opensource.org/licenses/ECL-2.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/eCos-2.0.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "eCos-2.0",
             "name": "eCos license version 2.0",
             "reference": "https://spdx.org/licenses/eCos-2.0.html",
-            "referenceNumber": 115,
+            "referenceNumber": 40,
             "seeAlso": [
                 "https://www.gnu.org/licenses/ecos-license.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/EFL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "EFL-1.0",
             "name": "Eiffel Forum License v1.0",
             "reference": "https://spdx.org/licenses/EFL-1.0.html",
-            "referenceNumber": 189,
+            "referenceNumber": 485,
             "seeAlso": [
                 "http://www.eiffel-nice.org/license/forum.txt",
                 "https://opensource.org/licenses/EFL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/EFL-2.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "EFL-2.0",
             "name": "Eiffel Forum License v2.0",
             "reference": "https://spdx.org/licenses/EFL-2.0.html",
-            "referenceNumber": 416,
+            "referenceNumber": 437,
             "seeAlso": [
                 "http://www.eiffel-nice.org/license/eiffel-forum-license-2.html",
                 "https://opensource.org/licenses/EFL-2.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/eGenix.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "eGenix",
             "name": "eGenix.com Public License 1.1.0",
             "reference": "https://spdx.org/licenses/eGenix.html",
-            "referenceNumber": 13,
+            "referenceNumber": 170,
             "seeAlso": [
                 "http://www.egenix.com/products/eGenix.com-Public-License-1.1.0.pdf",
                 "https://fedoraproject.org/wiki/Licensing/eGenix.com_Public_License_1.1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Elastic-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Elastic-2.0",
             "name": "Elastic License 2.0",
             "reference": "https://spdx.org/licenses/Elastic-2.0.html",
-            "referenceNumber": 193,
+            "referenceNumber": 547,
             "seeAlso": [
                 "https://www.elastic.co/licensing/elastic-license",
                 "https://github.com/elastic/elasticsearch/blob/master/licenses/ELASTIC-LICENSE-2.0.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Entessa.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "Entessa",
             "name": "Entessa Public License v1.0",
             "reference": "https://spdx.org/licenses/Entessa.html",
-            "referenceNumber": 468,
+            "referenceNumber": 89,
             "seeAlso": [
                 "https://opensource.org/licenses/Entessa"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/EPICS.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "EPICS",
             "name": "EPICS Open License",
             "reference": "https://spdx.org/licenses/EPICS.html",
-            "referenceNumber": 271,
+            "referenceNumber": 508,
             "seeAlso": [
                 "https://epics.anl.gov/license/open.php"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/EPL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "EPL-1.0",
             "name": "Eclipse Public License 1.0",
             "reference": "https://spdx.org/licenses/EPL-1.0.html",
-            "referenceNumber": 207,
+            "referenceNumber": 388,
             "seeAlso": [
                 "http://www.eclipse.org/legal/epl-v10.html",
                 "https://opensource.org/licenses/EPL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/EPL-2.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "EPL-2.0",
             "name": "Eclipse Public License 2.0",
             "reference": "https://spdx.org/licenses/EPL-2.0.html",
-            "referenceNumber": 434,
+            "referenceNumber": 114,
             "seeAlso": [
                 "https://www.eclipse.org/legal/epl-2.0",
                 "https://www.opensource.org/licenses/EPL-2.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/ErlPL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "ErlPL-1.1",
             "name": "Erlang Public License v1.1",
             "reference": "https://spdx.org/licenses/ErlPL-1.1.html",
-            "referenceNumber": 41,
+            "referenceNumber": 228,
             "seeAlso": [
                 "http://www.erlang.org/EPLICENSE"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/etalab-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "etalab-2.0",
             "name": "Etalab Open License 2.0",
             "reference": "https://spdx.org/licenses/etalab-2.0.html",
-            "referenceNumber": 363,
+            "referenceNumber": 273,
             "seeAlso": [
                 "https://github.com/DISIC/politique-de-contribution-open-source/blob/master/LICENSE.pdf",
                 "https://raw.githubusercontent.com/DISIC/politique-de-contribution-open-source/master/LICENSE"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/EUDatagrid.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "EUDatagrid",
             "name": "EU DataGrid Software License",
             "reference": "https://spdx.org/licenses/EUDatagrid.html",
-            "referenceNumber": 419,
+            "referenceNumber": 30,
             "seeAlso": [
                 "http://eu-datagrid.web.cern.ch/eu-datagrid/license.html",
                 "https://opensource.org/licenses/EUDatagrid"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/EUPL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "EUPL-1.0",
             "name": "European Union Public License 1.0",
             "reference": "https://spdx.org/licenses/EUPL-1.0.html",
-            "referenceNumber": 232,
+            "referenceNumber": 361,
             "seeAlso": [
                 "http://ec.europa.eu/idabc/en/document/7330.html",
                 "http://ec.europa.eu/idabc/servlets/Doc027f.pdf?id=31096"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/EUPL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "EUPL-1.1",
             "name": "European Union Public License 1.1",
             "reference": "https://spdx.org/licenses/EUPL-1.1.html",
-            "referenceNumber": 410,
+            "referenceNumber": 109,
             "seeAlso": [
                 "https://joinup.ec.europa.eu/software/page/eupl/licence-eupl",
                 "https://joinup.ec.europa.eu/sites/default/files/custom-page/attachment/eupl1.1.-licence-en_0.pdf",
                 "https://opensource.org/licenses/EUPL-1.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/EUPL-1.2.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "EUPL-1.2",
             "name": "European Union Public License 1.2",
             "reference": "https://spdx.org/licenses/EUPL-1.2.html",
-            "referenceNumber": 286,
+            "referenceNumber": 166,
             "seeAlso": [
                 "https://joinup.ec.europa.eu/page/eupl-text-11-12",
                 "https://joinup.ec.europa.eu/sites/default/files/custom-page/attachment/eupl_v1.2_en.pdf",
                 "https://joinup.ec.europa.eu/sites/default/files/custom-page/attachment/2020-03/EUPL-1.2%20EN.txt",
                 "https://joinup.ec.europa.eu/sites/default/files/inline-files/EUPL%20v1_2%20EN(1).txt",
                 "http://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=CELEX:32017D0863",
                 "https://opensource.org/licenses/EUPL-1.2"
@@ -2381,1393 +2593,1583 @@
         {
             "detailsUrl": "https://spdx.org/licenses/Eurosym.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Eurosym",
             "name": "Eurosym License",
             "reference": "https://spdx.org/licenses/Eurosym.html",
-            "referenceNumber": 79,
+            "referenceNumber": 49,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Eurosym"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Fair.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "Fair",
             "name": "Fair License",
             "reference": "https://spdx.org/licenses/Fair.html",
-            "referenceNumber": 125,
+            "referenceNumber": 436,
             "seeAlso": [
                 "http://fairlicense.org/",
                 "https://opensource.org/licenses/Fair"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/FDK-AAC.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "FDK-AAC",
             "name": "Fraunhofer FDK AAC Codec Library",
             "reference": "https://spdx.org/licenses/FDK-AAC.html",
-            "referenceNumber": 296,
+            "referenceNumber": 159,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/FDK-AAC",
                 "https://directory.fsf.org/wiki/License:Fdk"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Frameworx-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "Frameworx-1.0",
             "name": "Frameworx Open License 1.0",
             "reference": "https://spdx.org/licenses/Frameworx-1.0.html",
-            "referenceNumber": 315,
+            "referenceNumber": 207,
             "seeAlso": [
                 "https://opensource.org/licenses/Frameworx-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/FreeBSD-DOC.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "FreeBSD-DOC",
             "name": "FreeBSD Documentation License",
             "reference": "https://spdx.org/licenses/FreeBSD-DOC.html",
-            "referenceNumber": 228,
+            "referenceNumber": 168,
             "seeAlso": [
                 "https://www.freebsd.org/copyright/freebsd-doc-license/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/FreeImage.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "FreeImage",
             "name": "FreeImage Public License v1.0",
             "reference": "https://spdx.org/licenses/FreeImage.html",
-            "referenceNumber": 377,
+            "referenceNumber": 533,
             "seeAlso": [
                 "http://freeimage.sourceforge.net/freeimage-license.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/FSFAP.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "FSFAP",
             "name": "FSF All Permissive License",
             "reference": "https://spdx.org/licenses/FSFAP.html",
-            "referenceNumber": 368,
+            "referenceNumber": 340,
             "seeAlso": [
                 "https://www.gnu.org/prep/maintain/html_node/License-Notices-for-Other-Files.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/FSFUL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "FSFUL",
             "name": "FSF Unlimited License",
             "reference": "https://spdx.org/licenses/FSFUL.html",
-            "referenceNumber": 327,
+            "referenceNumber": 393,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/FSF_Unlimited_License"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/FSFULLR.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "FSFULLR",
             "name": "FSF Unlimited License (with License Retention)",
             "reference": "https://spdx.org/licenses/FSFULLR.html",
-            "referenceNumber": 242,
+            "referenceNumber": 528,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/FSF_Unlimited_License#License_Retention_Variant"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/FSFULLRWD.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "FSFULLRWD",
-            "name": "FSF Unlimited License (With License Retention    and Warranty Disclaimer)",
+            "name": "FSF Unlimited License (With License Retention and Warranty Disclaimer)",
             "reference": "https://spdx.org/licenses/FSFULLRWD.html",
-            "referenceNumber": 448,
+            "referenceNumber": 512,
             "seeAlso": [
                 "https://lists.gnu.org/archive/html/autoconf/2012-04/msg00061.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/FTL.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "FTL",
             "name": "Freetype Project License",
             "reference": "https://spdx.org/licenses/FTL.html",
-            "referenceNumber": 199,
+            "referenceNumber": 209,
             "seeAlso": [
                 "http://freetype.fis.uniroma2.it/FTL.TXT",
                 "http://git.savannah.gnu.org/cgit/freetype/freetype2.git/tree/docs/FTL.TXT",
                 "http://gitlab.freedesktop.org/freetype/freetype/-/raw/master/docs/FTL.TXT"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GD.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GD",
             "name": "GD License",
             "reference": "https://spdx.org/licenses/GD.html",
-            "referenceNumber": 150,
+            "referenceNumber": 294,
             "seeAlso": [
                 "https://libgd.github.io/manuals/2.3.0/files/license-txt.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.1.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.1",
             "name": "GNU Free Documentation License v1.1",
             "reference": "https://spdx.org/licenses/GFDL-1.1.html",
-            "referenceNumber": 438,
+            "referenceNumber": 59,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/fdl-1.1.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.1-invariants-only.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.1-invariants-only",
             "name": "GNU Free Documentation License v1.1 only - invariants",
             "reference": "https://spdx.org/licenses/GFDL-1.1-invariants-only.html",
-            "referenceNumber": 58,
+            "referenceNumber": 521,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/fdl-1.1.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.1-invariants-or-later.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.1-invariants-or-later",
             "name": "GNU Free Documentation License v1.1 or later - invariants",
             "reference": "https://spdx.org/licenses/GFDL-1.1-invariants-or-later.html",
-            "referenceNumber": 284,
+            "referenceNumber": 275,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/fdl-1.1.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.1-no-invariants-only.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.1-no-invariants-only",
             "name": "GNU Free Documentation License v1.1 only - no invariants",
             "reference": "https://spdx.org/licenses/GFDL-1.1-no-invariants-only.html",
-            "referenceNumber": 34,
+            "referenceNumber": 124,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/fdl-1.1.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.1-no-invariants-or-later.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.1-no-invariants-or-later",
             "name": "GNU Free Documentation License v1.1 or later - no invariants",
             "reference": "https://spdx.org/licenses/GFDL-1.1-no-invariants-or-later.html",
-            "referenceNumber": 9,
+            "referenceNumber": 391,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/fdl-1.1.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.1-only.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.1-only",
             "name": "GNU Free Documentation License v1.1 only",
             "reference": "https://spdx.org/licenses/GFDL-1.1-only.html",
-            "referenceNumber": 2,
+            "referenceNumber": 11,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/fdl-1.1.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.1-or-later.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.1-or-later",
             "name": "GNU Free Documentation License v1.1 or later",
             "reference": "https://spdx.org/licenses/GFDL-1.1-or-later.html",
-            "referenceNumber": 96,
+            "referenceNumber": 197,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/fdl-1.1.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.2.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.2",
             "name": "GNU Free Documentation License v1.2",
             "reference": "https://spdx.org/licenses/GFDL-1.2.html",
-            "referenceNumber": 328,
+            "referenceNumber": 188,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/fdl-1.2.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.2-invariants-only.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.2-invariants-only",
             "name": "GNU Free Documentation License v1.2 only - invariants",
             "reference": "https://spdx.org/licenses/GFDL-1.2-invariants-only.html",
-            "referenceNumber": 463,
+            "referenceNumber": 194,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/fdl-1.2.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.2-invariants-or-later.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.2-invariants-or-later",
             "name": "GNU Free Documentation License v1.2 or later - invariants",
             "reference": "https://spdx.org/licenses/GFDL-1.2-invariants-or-later.html",
-            "referenceNumber": 381,
+            "referenceNumber": 313,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/fdl-1.2.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.2-no-invariants-only.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.2-no-invariants-only",
             "name": "GNU Free Documentation License v1.2 only - no invariants",
             "reference": "https://spdx.org/licenses/GFDL-1.2-no-invariants-only.html",
-            "referenceNumber": 361,
+            "referenceNumber": 427,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/fdl-1.2.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.2-no-invariants-or-later.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.2-no-invariants-or-later",
             "name": "GNU Free Documentation License v1.2 or later - no invariants",
             "reference": "https://spdx.org/licenses/GFDL-1.2-no-invariants-or-later.html",
-            "referenceNumber": 387,
+            "referenceNumber": 285,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/fdl-1.2.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.2-only.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.2-only",
             "name": "GNU Free Documentation License v1.2 only",
             "reference": "https://spdx.org/licenses/GFDL-1.2-only.html",
-            "referenceNumber": 379,
+            "referenceNumber": 244,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/fdl-1.2.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.2-or-later.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.2-or-later",
             "name": "GNU Free Documentation License v1.2 or later",
             "reference": "https://spdx.org/licenses/GFDL-1.2-or-later.html",
-            "referenceNumber": 332,
+            "referenceNumber": 349,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/fdl-1.2.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.3.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.3",
             "name": "GNU Free Documentation License v1.3",
             "reference": "https://spdx.org/licenses/GFDL-1.3.html",
-            "referenceNumber": 90,
+            "referenceNumber": 435,
             "seeAlso": [
                 "https://www.gnu.org/licenses/fdl-1.3.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.3-invariants-only.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.3-invariants-only",
             "name": "GNU Free Documentation License v1.3 only - invariants",
             "reference": "https://spdx.org/licenses/GFDL-1.3-invariants-only.html",
-            "referenceNumber": 206,
+            "referenceNumber": 37,
             "seeAlso": [
                 "https://www.gnu.org/licenses/fdl-1.3.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.3-invariants-or-later.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.3-invariants-or-later",
             "name": "GNU Free Documentation License v1.3 or later - invariants",
             "reference": "https://spdx.org/licenses/GFDL-1.3-invariants-or-later.html",
-            "referenceNumber": 97,
+            "referenceNumber": 406,
             "seeAlso": [
                 "https://www.gnu.org/licenses/fdl-1.3.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.3-no-invariants-only.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.3-no-invariants-only",
             "name": "GNU Free Documentation License v1.3 only - no invariants",
             "reference": "https://spdx.org/licenses/GFDL-1.3-no-invariants-only.html",
-            "referenceNumber": 176,
+            "referenceNumber": 249,
             "seeAlso": [
                 "https://www.gnu.org/licenses/fdl-1.3.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.3-no-invariants-or-later.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.3-no-invariants-or-later",
             "name": "GNU Free Documentation License v1.3 or later - no invariants",
             "reference": "https://spdx.org/licenses/GFDL-1.3-no-invariants-or-later.html",
-            "referenceNumber": 420,
+            "referenceNumber": 523,
             "seeAlso": [
                 "https://www.gnu.org/licenses/fdl-1.3.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.3-only.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.3-only",
             "name": "GNU Free Documentation License v1.3 only",
             "reference": "https://spdx.org/licenses/GFDL-1.3-only.html",
-            "referenceNumber": 214,
+            "referenceNumber": 283,
             "seeAlso": [
                 "https://www.gnu.org/licenses/fdl-1.3.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GFDL-1.3-or-later.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "GFDL-1.3-or-later",
             "name": "GNU Free Documentation License v1.3 or later",
             "reference": "https://spdx.org/licenses/GFDL-1.3-or-later.html",
-            "referenceNumber": 486,
+            "referenceNumber": 336,
             "seeAlso": [
                 "https://www.gnu.org/licenses/fdl-1.3.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Giftware.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Giftware",
             "name": "Giftware License",
             "reference": "https://spdx.org/licenses/Giftware.html",
-            "referenceNumber": 336,
+            "referenceNumber": 329,
             "seeAlso": [
                 "http://liballeg.org/license.html#allegro-4-the-giftware-license"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GL2PS.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GL2PS",
             "name": "GL2PS License",
             "reference": "https://spdx.org/licenses/GL2PS.html",
-            "referenceNumber": 297,
+            "referenceNumber": 461,
             "seeAlso": [
                 "http://www.geuz.org/gl2ps/COPYING.GL2PS"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Glide.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Glide",
             "name": "3dfx Glide License",
             "reference": "https://spdx.org/licenses/Glide.html",
-            "referenceNumber": 146,
+            "referenceNumber": 353,
             "seeAlso": [
                 "http://www.users.on.net/~triforce/glidexp/COPYING.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Glulxe.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Glulxe",
             "name": "Glulxe License",
             "reference": "https://spdx.org/licenses/Glulxe.html",
-            "referenceNumber": 14,
+            "referenceNumber": 530,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Glulxe"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GLWTPL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GLWTPL",
             "name": "Good Luck With That Public License",
             "reference": "https://spdx.org/licenses/GLWTPL.html",
-            "referenceNumber": 396,
+            "referenceNumber": 318,
             "seeAlso": [
                 "https://github.com/me-shaon/GLWTPL/commit/da5f6bc734095efbacb442c0b31e33a65b9d6e85"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/gnuplot.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "gnuplot",
             "name": "gnuplot License",
             "reference": "https://spdx.org/licenses/gnuplot.html",
-            "referenceNumber": 289,
+            "referenceNumber": 455,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Gnuplot"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-1.0.json",
             "isDeprecatedLicenseId": true,
             "isOsiApproved": false,
             "licenseId": "GPL-1.0",
             "name": "GNU General Public License v1.0 only",
             "reference": "https://spdx.org/licenses/GPL-1.0.html",
-            "referenceNumber": 402,
+            "referenceNumber": 212,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/gpl-1.0-standalone.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-1.0+.json",
             "isDeprecatedLicenseId": true,
             "isOsiApproved": false,
             "licenseId": "GPL-1.0+",
             "name": "GNU General Public License v1.0 or later",
             "reference": "https://spdx.org/licenses/GPL-1.0+.html",
-            "referenceNumber": 430,
+            "referenceNumber": 219,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/gpl-1.0-standalone.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-1.0-only.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GPL-1.0-only",
             "name": "GNU General Public License v1.0 only",
             "reference": "https://spdx.org/licenses/GPL-1.0-only.html",
-            "referenceNumber": 299,
+            "referenceNumber": 235,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/gpl-1.0-standalone.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-1.0-or-later.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "GPL-1.0-or-later",
             "name": "GNU General Public License v1.0 or later",
             "reference": "https://spdx.org/licenses/GPL-1.0-or-later.html",
-            "referenceNumber": 275,
+            "referenceNumber": 85,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/gpl-1.0-standalone.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-2.0.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "GPL-2.0",
             "name": "GNU General Public License v2.0 only",
             "reference": "https://spdx.org/licenses/GPL-2.0.html",
-            "referenceNumber": 283,
+            "referenceNumber": 1,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/gpl-2.0-standalone.html",
                 "https://opensource.org/licenses/GPL-2.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-2.0+.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "GPL-2.0+",
             "name": "GNU General Public License v2.0 or later",
             "reference": "https://spdx.org/licenses/GPL-2.0+.html",
-            "referenceNumber": 166,
+            "referenceNumber": 509,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/gpl-2.0-standalone.html",
                 "https://opensource.org/licenses/GPL-2.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-2.0-only.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "GPL-2.0-only",
             "name": "GNU General Public License v2.0 only",
             "reference": "https://spdx.org/licenses/GPL-2.0-only.html",
-            "referenceNumber": 318,
+            "referenceNumber": 438,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/gpl-2.0-standalone.html",
                 "https://opensource.org/licenses/GPL-2.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-2.0-or-later.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "GPL-2.0-or-later",
             "name": "GNU General Public License v2.0 or later",
             "reference": "https://spdx.org/licenses/GPL-2.0-or-later.html",
-            "referenceNumber": 392,
+            "referenceNumber": 17,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/gpl-2.0-standalone.html",
                 "https://opensource.org/licenses/GPL-2.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-2.0-with-autoconf-exception.json",
             "isDeprecatedLicenseId": true,
             "isOsiApproved": false,
             "licenseId": "GPL-2.0-with-autoconf-exception",
             "name": "GNU General Public License v2.0 w/Autoconf exception",
             "reference": "https://spdx.org/licenses/GPL-2.0-with-autoconf-exception.html",
-            "referenceNumber": 183,
+            "referenceNumber": 296,
             "seeAlso": [
                 "http://ac-archive.sourceforge.net/doc/copyright.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-2.0-with-bison-exception.json",
             "isDeprecatedLicenseId": true,
             "isOsiApproved": false,
             "licenseId": "GPL-2.0-with-bison-exception",
             "name": "GNU General Public License v2.0 w/Bison exception",
             "reference": "https://spdx.org/licenses/GPL-2.0-with-bison-exception.html",
-            "referenceNumber": 316,
+            "referenceNumber": 68,
             "seeAlso": [
                 "http://git.savannah.gnu.org/cgit/bison.git/tree/data/yacc.c?id=193d7c7054ba7197b0789e14965b739162319b5e#n141"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-2.0-with-classpath-exception.json",
             "isDeprecatedLicenseId": true,
             "isOsiApproved": false,
             "licenseId": "GPL-2.0-with-classpath-exception",
             "name": "GNU General Public License v2.0 w/Classpath exception",
             "reference": "https://spdx.org/licenses/GPL-2.0-with-classpath-exception.html",
-            "referenceNumber": 295,
+            "referenceNumber": 261,
             "seeAlso": [
                 "https://www.gnu.org/software/classpath/license.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-2.0-with-font-exception.json",
             "isDeprecatedLicenseId": true,
             "isOsiApproved": false,
             "licenseId": "GPL-2.0-with-font-exception",
             "name": "GNU General Public License v2.0 w/Font exception",
             "reference": "https://spdx.org/licenses/GPL-2.0-with-font-exception.html",
-            "referenceNumber": 226,
+            "referenceNumber": 87,
             "seeAlso": [
                 "https://www.gnu.org/licenses/gpl-faq.html#FontException"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-2.0-with-GCC-exception.json",
             "isDeprecatedLicenseId": true,
             "isOsiApproved": false,
             "licenseId": "GPL-2.0-with-GCC-exception",
             "name": "GNU General Public License v2.0 w/GCC Runtime Library exception",
             "reference": "https://spdx.org/licenses/GPL-2.0-with-GCC-exception.html",
-            "referenceNumber": 473,
+            "referenceNumber": 468,
             "seeAlso": [
                 "https://gcc.gnu.org/git/?p=gcc.git;a=blob;f=gcc/libgcc1.c;h=762f5143fc6eed57b6797c82710f3538aa52b40b;hb=cb143a3ce4fb417c68f5fa2691a1b1b1053dfba9#l10"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-3.0.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "GPL-3.0",
             "name": "GNU General Public License v3.0 only",
             "reference": "https://spdx.org/licenses/GPL-3.0.html",
-            "referenceNumber": 458,
+            "referenceNumber": 55,
             "seeAlso": [
                 "https://www.gnu.org/licenses/gpl-3.0-standalone.html",
                 "https://opensource.org/licenses/GPL-3.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-3.0+.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "GPL-3.0+",
             "name": "GNU General Public License v3.0 or later",
             "reference": "https://spdx.org/licenses/GPL-3.0+.html",
-            "referenceNumber": 376,
+            "referenceNumber": 146,
             "seeAlso": [
                 "https://www.gnu.org/licenses/gpl-3.0-standalone.html",
                 "https://opensource.org/licenses/GPL-3.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-3.0-only.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "GPL-3.0-only",
             "name": "GNU General Public License v3.0 only",
             "reference": "https://spdx.org/licenses/GPL-3.0-only.html",
-            "referenceNumber": 16,
+            "referenceNumber": 174,
             "seeAlso": [
                 "https://www.gnu.org/licenses/gpl-3.0-standalone.html",
                 "https://opensource.org/licenses/GPL-3.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-3.0-or-later.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "GPL-3.0-or-later",
             "name": "GNU General Public License v3.0 or later",
             "reference": "https://spdx.org/licenses/GPL-3.0-or-later.html",
-            "referenceNumber": 321,
+            "referenceNumber": 425,
             "seeAlso": [
                 "https://www.gnu.org/licenses/gpl-3.0-standalone.html",
                 "https://opensource.org/licenses/GPL-3.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-3.0-with-autoconf-exception.json",
             "isDeprecatedLicenseId": true,
             "isOsiApproved": false,
             "licenseId": "GPL-3.0-with-autoconf-exception",
             "name": "GNU General Public License v3.0 w/Autoconf exception",
             "reference": "https://spdx.org/licenses/GPL-3.0-with-autoconf-exception.html",
-            "referenceNumber": 357,
+            "referenceNumber": 484,
             "seeAlso": [
                 "https://www.gnu.org/licenses/autoconf-exception-3.0.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/GPL-3.0-with-GCC-exception.json",
             "isDeprecatedLicenseId": true,
             "isOsiApproved": true,
             "licenseId": "GPL-3.0-with-GCC-exception",
             "name": "GNU General Public License v3.0 w/GCC Runtime Library exception",
             "reference": "https://spdx.org/licenses/GPL-3.0-with-GCC-exception.html",
-            "referenceNumber": 319,
+            "referenceNumber": 446,
             "seeAlso": [
                 "https://www.gnu.org/licenses/gcc-exception-3.1.html"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/Graphics-Gems.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Graphics-Gems",
+            "name": "Graphics Gems License",
+            "reference": "https://spdx.org/licenses/Graphics-Gems.html",
+            "referenceNumber": 315,
+            "seeAlso": [
+                "https://github.com/erich666/GraphicsGems/blob/master/LICENSE.md"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/gSOAP-1.3b.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "gSOAP-1.3b",
             "name": "gSOAP Public License v1.3b",
             "reference": "https://spdx.org/licenses/gSOAP-1.3b.html",
-            "referenceNumber": 230,
+            "referenceNumber": 556,
             "seeAlso": [
                 "http://www.cs.fsu.edu/~engelen/license.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/HaskellReport.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "HaskellReport",
             "name": "Haskell Language Report License",
             "reference": "https://spdx.org/licenses/HaskellReport.html",
-            "referenceNumber": 437,
+            "referenceNumber": 135,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Haskell_Language_Report_License"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Hippocratic-2.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Hippocratic-2.1",
             "name": "Hippocratic License 2.1",
             "reference": "https://spdx.org/licenses/Hippocratic-2.1.html",
-            "referenceNumber": 53,
+            "referenceNumber": 5,
             "seeAlso": [
                 "https://firstdonoharm.dev/version/2/1/license.html",
                 "https://github.com/EthicalSource/hippocratic-license/blob/58c0e646d64ff6fbee275bfe2b9492f914e3ab2a/LICENSE.txt"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/HP-1986.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "HP-1986",
+            "name": "Hewlett-Packard 1986 License",
+            "reference": "https://spdx.org/licenses/HP-1986.html",
+            "referenceNumber": 98,
+            "seeAlso": [
+                "https://sourceware.org/git/?p=newlib-cygwin.git;a=blob;f=newlib/libc/machine/hppa/memchr.S;h=1cca3e5e8867aa4bffef1f75a5c1bba25c0c441e;hb=HEAD#l2"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/HPND.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "HPND",
             "name": "Historical Permission Notice and Disclaimer",
             "reference": "https://spdx.org/licenses/HPND.html",
-            "referenceNumber": 163,
+            "referenceNumber": 172,
             "seeAlso": [
                 "https://opensource.org/licenses/HPND"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/HPND-export-US.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "HPND-export-US",
+            "name": "HPND with US Government export control warning",
+            "reference": "https://spdx.org/licenses/HPND-export-US.html",
+            "referenceNumber": 272,
+            "seeAlso": [
+                "https://www.kermitproject.org/ck90.html#source"
+            ]
+        },
+        {
+            "detailsUrl": "https://spdx.org/licenses/HPND-Markus-Kuhn.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "HPND-Markus-Kuhn",
+            "name": "Historical Permission Notice and Disclaimer - Markus Kuhn variant",
+            "reference": "https://spdx.org/licenses/HPND-Markus-Kuhn.html",
+            "referenceNumber": 118,
+            "seeAlso": [
+                "https://www.cl.cam.ac.uk/~mgk25/ucs/wcwidth.c",
+                "https://sourceware.org/git/?p=binutils-gdb.git;a=blob;f=readline/readline/support/wcwidth.c;h=0f5ec995796f4813abbcf4972aec0378ab74722a;hb=HEAD#l55"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/HPND-sell-variant.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "HPND-sell-variant",
             "name": "Historical Permission Notice and Disclaimer - sell variant",
             "reference": "https://spdx.org/licenses/HPND-sell-variant.html",
-            "referenceNumber": 143,
+            "referenceNumber": 424,
             "seeAlso": [
                 "https://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux.git/tree/net/sunrpc/auth_gss/gss_generic_token.c?h=v4.19"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/HPND-sell-variant-MIT-disclaimer.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "HPND-sell-variant-MIT-disclaimer",
+            "name": "HPND sell variant with MIT disclaimer",
+            "reference": "https://spdx.org/licenses/HPND-sell-variant-MIT-disclaimer.html",
+            "referenceNumber": 103,
+            "seeAlso": [
+                "https://github.com/sigmavirus24/x11-ssh-askpass/blob/master/README"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/HTMLTIDY.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "HTMLTIDY",
             "name": "HTML Tidy License",
             "reference": "https://spdx.org/licenses/HTMLTIDY.html",
-            "referenceNumber": 427,
+            "referenceNumber": 538,
             "seeAlso": [
                 "https://github.com/htacg/tidy-html5/blob/next/README/LICENSE.md"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/IBM-pibs.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "IBM-pibs",
             "name": "IBM PowerPC Initialization and Boot Software",
             "reference": "https://spdx.org/licenses/IBM-pibs.html",
-            "referenceNumber": 119,
+            "referenceNumber": 96,
             "seeAlso": [
                 "http://git.denx.de/?p=u-boot.git;a=blob;f=arch/powerpc/cpu/ppc4xx/miiphy.c;h=297155fdafa064b955e53e9832de93bfb0cfb85b;hb=9fab4bf4cc077c21e43941866f3f2c196f28670d"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/ICU.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "ICU",
             "name": "ICU License",
             "reference": "https://spdx.org/licenses/ICU.html",
-            "referenceNumber": 374,
+            "referenceNumber": 254,
             "seeAlso": [
                 "http://source.icu-project.org/repos/icu/icu/trunk/license.html"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/IEC-Code-Components-EULA.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "IEC-Code-Components-EULA",
+            "name": "IEC    Code Components End-user licence agreement",
+            "reference": "https://spdx.org/licenses/IEC-Code-Components-EULA.html",
+            "referenceNumber": 546,
+            "seeAlso": [
+                "https://www.iec.ch/webstore/custserv/pdf/CC-EULA.pdf",
+                "https://www.iec.ch/CCv1",
+                "https://www.iec.ch/copyright"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/IJG.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "IJG",
             "name": "Independent JPEG Group License",
             "reference": "https://spdx.org/licenses/IJG.html",
-            "referenceNumber": 211,
+            "referenceNumber": 110,
             "seeAlso": [
                 "http://dev.w3.org/cvsweb/Amaya/libjpeg/Attic/README?rev=1.2"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/IJG-short.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "IJG-short",
+            "name": "Independent JPEG Group License - short",
+            "reference": "https://spdx.org/licenses/IJG-short.html",
+            "referenceNumber": 373,
+            "seeAlso": [
+                "https://sourceforge.net/p/xmedcon/code/ci/master/tree/libs/ljpg/"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/ImageMagick.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "ImageMagick",
             "name": "ImageMagick License",
             "reference": "https://spdx.org/licenses/ImageMagick.html",
-            "referenceNumber": 407,
+            "referenceNumber": 287,
             "seeAlso": [
                 "http://www.imagemagick.org/script/license.php"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/iMatix.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "iMatix",
             "name": "iMatix Standard Function Library Agreement",
             "reference": "https://spdx.org/licenses/iMatix.html",
-            "referenceNumber": 7,
+            "referenceNumber": 430,
             "seeAlso": [
                 "http://legacy.imatix.com/html/sfl/sfl4.htm#license"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Imlib2.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "Imlib2",
             "name": "Imlib2 License",
             "reference": "https://spdx.org/licenses/Imlib2.html",
-            "referenceNumber": 167,
+            "referenceNumber": 477,
             "seeAlso": [
                 "http://trac.enlightenment.org/e/browser/trunk/imlib2/COPYING",
                 "https://git.enlightenment.org/legacy/imlib2.git/tree/COPYING"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Info-ZIP.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Info-ZIP",
             "name": "Info-ZIP License",
             "reference": "https://spdx.org/licenses/Info-ZIP.html",
-            "referenceNumber": 132,
+            "referenceNumber": 366,
             "seeAlso": [
                 "http://www.info-zip.org/license.html"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/Inner-Net-2.0.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Inner-Net-2.0",
+            "name": "Inner Net License v2.0",
+            "reference": "https://spdx.org/licenses/Inner-Net-2.0.html",
+            "referenceNumber": 241,
+            "seeAlso": [
+                "https://fedoraproject.org/wiki/Licensing/Inner_Net_License",
+                "https://sourceware.org/git/?p=glibc.git;a=blob;f=LICENSES;h=530893b1dc9ea00755603c68fb36bd4fc38a7be8;hb=HEAD#l207"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Intel.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "Intel",
             "name": "Intel Open Source License",
             "reference": "https://spdx.org/licenses/Intel.html",
-            "referenceNumber": 395,
+            "referenceNumber": 486,
             "seeAlso": [
                 "https://opensource.org/licenses/Intel"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Intel-ACPI.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Intel-ACPI",
             "name": "Intel ACPI Software License Agreement",
             "reference": "https://spdx.org/licenses/Intel-ACPI.html",
-            "referenceNumber": 87,
+            "referenceNumber": 65,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Intel_ACPI_Software_License_Agreement"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Interbase-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Interbase-1.0",
             "name": "Interbase Public License v1.0",
             "reference": "https://spdx.org/licenses/Interbase-1.0.html",
-            "referenceNumber": 494,
+            "referenceNumber": 553,
             "seeAlso": [
                 "https://web.archive.org/web/20060319014854/http://info.borland.com/devsupport/interbase/opensource/IPL.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/IPA.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "IPA",
             "name": "IPA Font License",
             "reference": "https://spdx.org/licenses/IPA.html",
-            "referenceNumber": 177,
+            "referenceNumber": 383,
             "seeAlso": [
                 "https://opensource.org/licenses/IPA"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/IPL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "IPL-1.0",
             "name": "IBM Public License v1.0",
             "reference": "https://spdx.org/licenses/IPL-1.0.html",
-            "referenceNumber": 480,
+            "referenceNumber": 220,
             "seeAlso": [
                 "https://opensource.org/licenses/IPL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/ISC.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "ISC",
             "name": "ISC License",
             "reference": "https://spdx.org/licenses/ISC.html",
-            "referenceNumber": 323,
+            "referenceNumber": 263,
             "seeAlso": [
                 "https://www.isc.org/licenses/",
                 "https://www.isc.org/downloads/software-support-policy/isc-license/",
                 "https://opensource.org/licenses/ISC"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Jam.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "Jam",
             "name": "Jam License",
             "reference": "https://spdx.org/licenses/Jam.html",
-            "referenceNumber": 71,
+            "referenceNumber": 445,
             "seeAlso": [
                 "https://www.boost.org/doc/libs/1_35_0/doc/html/jam.html",
                 "https://web.archive.org/web/20160330173339/https://swarm.workshop.perforce.com/files/guest/perforce_software/jam/src/README"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/JasPer-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "JasPer-2.0",
             "name": "JasPer License",
             "reference": "https://spdx.org/licenses/JasPer-2.0.html",
-            "referenceNumber": 43,
+            "referenceNumber": 537,
             "seeAlso": [
                 "http://www.ece.uvic.ca/~mdadams/jasper/LICENSE"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/JPL-image.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "JPL-image",
+            "name": "JPL Image Use Policy",
+            "reference": "https://spdx.org/licenses/JPL-image.html",
+            "referenceNumber": 81,
+            "seeAlso": [
+                "https://www.jpl.nasa.gov/jpl-image-use-policy"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/JPNIC.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "JPNIC",
             "name": "Japan Network Information Center License",
             "reference": "https://spdx.org/licenses/JPNIC.html",
-            "referenceNumber": 488,
+            "referenceNumber": 50,
             "seeAlso": [
                 "https://gitlab.isc.org/isc-projects/bind9/blob/master/COPYRIGHT#L366"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/JSON.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": false,
             "licenseId": "JSON",
             "name": "JSON License",
             "reference": "https://spdx.org/licenses/JSON.html",
-            "referenceNumber": 152,
+            "referenceNumber": 543,
             "seeAlso": [
                 "http://www.json.org/license.html"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/Kazlib.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Kazlib",
+            "name": "Kazlib License",
+            "reference": "https://spdx.org/licenses/Kazlib.html",
+            "referenceNumber": 229,
+            "seeAlso": [
+                "http://git.savannah.gnu.org/cgit/kazlib.git/tree/except.c?id=0062df360c2d17d57f6af19b0e444c51feb99036"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Knuth-CTAN.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Knuth-CTAN",
             "name": "Knuth CTAN License",
             "reference": "https://spdx.org/licenses/Knuth-CTAN.html",
-            "referenceNumber": 450,
+            "referenceNumber": 222,
             "seeAlso": [
                 "https://ctan.org/license/knuth"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LAL-1.2.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "LAL-1.2",
             "name": "Licence Art Libre 1.2",
             "reference": "https://spdx.org/licenses/LAL-1.2.html",
-            "referenceNumber": 208,
+            "referenceNumber": 176,
             "seeAlso": [
                 "http://artlibre.org/licence/lal/licence-art-libre-12/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LAL-1.3.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "LAL-1.3",
             "name": "Licence Art Libre 1.3",
             "reference": "https://spdx.org/licenses/LAL-1.3.html",
-            "referenceNumber": 30,
+            "referenceNumber": 515,
             "seeAlso": [
                 "https://artlibre.org/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Latex2e.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Latex2e",
             "name": "Latex2e License",
             "reference": "https://spdx.org/licenses/Latex2e.html",
-            "referenceNumber": 86,
+            "referenceNumber": 303,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Latex2e"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/Latex2e-translated-notice.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Latex2e-translated-notice",
+            "name": "Latex2e with translated notice permission",
+            "reference": "https://spdx.org/licenses/Latex2e-translated-notice.html",
+            "referenceNumber": 26,
+            "seeAlso": [
+                "https://git.savannah.gnu.org/cgit/indent.git/tree/doc/indent.texi?id=a74c6b4ee49397cf330b333da1042bffa60ed14f#n74"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Leptonica.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Leptonica",
             "name": "Leptonica License",
             "reference": "https://spdx.org/licenses/Leptonica.html",
-            "referenceNumber": 104,
+            "referenceNumber": 206,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Leptonica"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LGPL-2.0.json",
             "isDeprecatedLicenseId": true,
             "isOsiApproved": true,
             "licenseId": "LGPL-2.0",
             "name": "GNU Library General Public License v2 only",
             "reference": "https://spdx.org/licenses/LGPL-2.0.html",
-            "referenceNumber": 320,
+            "referenceNumber": 470,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/lgpl-2.0-standalone.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LGPL-2.0+.json",
             "isDeprecatedLicenseId": true,
             "isOsiApproved": true,
             "licenseId": "LGPL-2.0+",
             "name": "GNU Library General Public License v2 or later",
             "reference": "https://spdx.org/licenses/LGPL-2.0+.html",
-            "referenceNumber": 188,
+            "referenceNumber": 82,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/lgpl-2.0-standalone.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LGPL-2.0-only.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "LGPL-2.0-only",
             "name": "GNU Library General Public License v2 only",
             "reference": "https://spdx.org/licenses/LGPL-2.0-only.html",
-            "referenceNumber": 57,
+            "referenceNumber": 19,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/lgpl-2.0-standalone.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LGPL-2.0-or-later.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "LGPL-2.0-or-later",
             "name": "GNU Library General Public License v2 or later",
             "reference": "https://spdx.org/licenses/LGPL-2.0-or-later.html",
-            "referenceNumber": 287,
+            "referenceNumber": 350,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/lgpl-2.0-standalone.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LGPL-2.1.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "LGPL-2.1",
             "name": "GNU Lesser General Public License v2.1 only",
             "reference": "https://spdx.org/licenses/LGPL-2.1.html",
-            "referenceNumber": 496,
+            "referenceNumber": 554,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/lgpl-2.1-standalone.html",
                 "https://opensource.org/licenses/LGPL-2.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LGPL-2.1+.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "LGPL-2.1+",
-            "name": "GNU Library General Public License v2.1 or later",
+            "name": "GNU Lesser General Public License v2.1 or later",
             "reference": "https://spdx.org/licenses/LGPL-2.1+.html",
-            "referenceNumber": 411,
+            "referenceNumber": 198,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/lgpl-2.1-standalone.html",
                 "https://opensource.org/licenses/LGPL-2.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LGPL-2.1-only.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "LGPL-2.1-only",
             "name": "GNU Lesser General Public License v2.1 only",
             "reference": "https://spdx.org/licenses/LGPL-2.1-only.html",
-            "referenceNumber": 371,
+            "referenceNumber": 359,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/lgpl-2.1-standalone.html",
                 "https://opensource.org/licenses/LGPL-2.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LGPL-2.1-or-later.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "LGPL-2.1-or-later",
             "name": "GNU Lesser General Public License v2.1 or later",
             "reference": "https://spdx.org/licenses/LGPL-2.1-or-later.html",
-            "referenceNumber": 139,
+            "referenceNumber": 66,
             "seeAlso": [
                 "https://www.gnu.org/licenses/old-licenses/lgpl-2.1-standalone.html",
                 "https://opensource.org/licenses/LGPL-2.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LGPL-3.0.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "LGPL-3.0",
             "name": "GNU Lesser General Public License v3.0 only",
             "reference": "https://spdx.org/licenses/LGPL-3.0.html",
-            "referenceNumber": 247,
+            "referenceNumber": 298,
             "seeAlso": [
                 "https://www.gnu.org/licenses/lgpl-3.0-standalone.html",
                 "https://www.gnu.org/licenses/lgpl+gpl-3.0.txt",
                 "https://opensource.org/licenses/LGPL-3.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LGPL-3.0+.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "LGPL-3.0+",
             "name": "GNU Lesser General Public License v3.0 or later",
             "reference": "https://spdx.org/licenses/LGPL-3.0+.html",
-            "referenceNumber": 258,
+            "referenceNumber": 231,
             "seeAlso": [
                 "https://www.gnu.org/licenses/lgpl-3.0-standalone.html",
                 "https://www.gnu.org/licenses/lgpl+gpl-3.0.txt",
                 "https://opensource.org/licenses/LGPL-3.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LGPL-3.0-only.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "LGPL-3.0-only",
             "name": "GNU Lesser General Public License v3.0 only",
             "reference": "https://spdx.org/licenses/LGPL-3.0-only.html",
-            "referenceNumber": 65,
+            "referenceNumber": 10,
             "seeAlso": [
                 "https://www.gnu.org/licenses/lgpl-3.0-standalone.html",
                 "https://www.gnu.org/licenses/lgpl+gpl-3.0.txt",
                 "https://opensource.org/licenses/LGPL-3.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LGPL-3.0-or-later.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "LGPL-3.0-or-later",
             "name": "GNU Lesser General Public License v3.0 or later",
             "reference": "https://spdx.org/licenses/LGPL-3.0-or-later.html",
-            "referenceNumber": 195,
+            "referenceNumber": 293,
             "seeAlso": [
                 "https://www.gnu.org/licenses/lgpl-3.0-standalone.html",
                 "https://www.gnu.org/licenses/lgpl+gpl-3.0.txt",
                 "https://opensource.org/licenses/LGPL-3.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LGPLLR.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "LGPLLR",
             "name": "Lesser General Public License For Linguistic Resources",
             "reference": "https://spdx.org/licenses/LGPLLR.html",
-            "referenceNumber": 224,
+            "referenceNumber": 56,
             "seeAlso": [
                 "http://www-igm.univ-mlv.fr/~unitex/lgpllr.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Libpng.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Libpng",
             "name": "libpng License",
             "reference": "https://spdx.org/licenses/Libpng.html",
-            "referenceNumber": 446,
+            "referenceNumber": 21,
             "seeAlso": [
                 "http://www.libpng.org/pub/png/src/libpng-LICENSE.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/libpng-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "libpng-2.0",
             "name": "PNG Reference Library version 2",
             "reference": "https://spdx.org/licenses/libpng-2.0.html",
-            "referenceNumber": 322,
+            "referenceNumber": 453,
             "seeAlso": [
                 "http://www.libpng.org/pub/png/src/libpng-LICENSE.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/libselinux-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "libselinux-1.0",
             "name": "libselinux public domain notice",
             "reference": "https://spdx.org/licenses/libselinux-1.0.html",
-            "referenceNumber": 67,
+            "referenceNumber": 501,
             "seeAlso": [
                 "https://github.com/SELinuxProject/selinux/blob/master/libselinux/LICENSE"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/libtiff.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "libtiff",
             "name": "libtiff License",
             "reference": "https://spdx.org/licenses/libtiff.html",
-            "referenceNumber": 348,
+            "referenceNumber": 227,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/libtiff"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/libutil-David-Nugent.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "libutil-David-Nugent",
             "name": "libutil David Nugent License",
             "reference": "https://spdx.org/licenses/libutil-David-Nugent.html",
-            "referenceNumber": 248,
+            "referenceNumber": 531,
             "seeAlso": [
                 "http://web.mit.edu/freebsd/head/lib/libutil/login_ok.3",
                 "https://cgit.freedesktop.org/libbsd/tree/man/setproctitle.3bsd"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LiLiQ-P-1.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "LiLiQ-P-1.1",
             "name": "Licence Libre du Qu\u00e9bec \u2013 Permissive version 1.1",
             "reference": "https://spdx.org/licenses/LiLiQ-P-1.1.html",
-            "referenceNumber": 6,
+            "referenceNumber": 48,
             "seeAlso": [
                 "https://forge.gouv.qc.ca/licence/fr/liliq-v1-1/",
                 "http://opensource.org/licenses/LiLiQ-P-1.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LiLiQ-R-1.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "LiLiQ-R-1.1",
             "name": "Licence Libre du Qu\u00e9bec \u2013 R\u00e9ciprocit\u00e9 version 1.1",
             "reference": "https://spdx.org/licenses/LiLiQ-R-1.1.html",
-            "referenceNumber": 52,
+            "referenceNumber": 418,
             "seeAlso": [
                 "https://www.forge.gouv.qc.ca/participez/licence-logicielle/licence-libre-du-quebec-liliq-en-francais/licence-libre-du-quebec-reciprocite-liliq-r-v1-1/",
                 "http://opensource.org/licenses/LiLiQ-R-1.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LiLiQ-Rplus-1.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "LiLiQ-Rplus-1.1",
             "name": "Licence Libre du Qu\u00e9bec \u2013 R\u00e9ciprocit\u00e9 forte version 1.1",
             "reference": "https://spdx.org/licenses/LiLiQ-Rplus-1.1.html",
-            "referenceNumber": 231,
+            "referenceNumber": 286,
             "seeAlso": [
                 "https://www.forge.gouv.qc.ca/participez/licence-logicielle/licence-libre-du-quebec-liliq-en-francais/licence-libre-du-quebec-reciprocite-forte-liliq-r-v1-1/",
                 "http://opensource.org/licenses/LiLiQ-Rplus-1.1"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/Linux-man-pages-1-para.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Linux-man-pages-1-para",
+            "name": "Linux man-pages - 1 paragraph",
+            "reference": "https://spdx.org/licenses/Linux-man-pages-1-para.html",
+            "referenceNumber": 409,
+            "seeAlso": [
+                "https://git.kernel.org/pub/scm/docs/man-pages/man-pages.git/tree/man2/getcpu.2#n4"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Linux-man-pages-copyleft.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Linux-man-pages-copyleft",
             "name": "Linux man-pages Copyleft",
             "reference": "https://spdx.org/licenses/Linux-man-pages-copyleft.html",
-            "referenceNumber": 403,
+            "referenceNumber": 469,
             "seeAlso": [
                 "https://www.kernel.org/doc/man-pages/licenses.html"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/Linux-man-pages-copyleft-2-para.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Linux-man-pages-copyleft-2-para",
+            "name": "Linux man-pages Copyleft - 2 paragraphs",
+            "reference": "https://spdx.org/licenses/Linux-man-pages-copyleft-2-para.html",
+            "referenceNumber": 167,
+            "seeAlso": [
+                "https://git.kernel.org/pub/scm/docs/man-pages/man-pages.git/tree/man2/move_pages.2#n5",
+                "https://git.kernel.org/pub/scm/docs/man-pages/man-pages.git/tree/man2/migrate_pages.2#n8"
+            ]
+        },
+        {
+            "detailsUrl": "https://spdx.org/licenses/Linux-man-pages-copyleft-var.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Linux-man-pages-copyleft-var",
+            "name": "Linux man-pages Copyleft Variant",
+            "reference": "https://spdx.org/licenses/Linux-man-pages-copyleft-var.html",
+            "referenceNumber": 400,
+            "seeAlso": [
+                "https://git.kernel.org/pub/scm/docs/man-pages/man-pages.git/tree/man2/set_mempolicy.2#n5"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Linux-OpenIB.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Linux-OpenIB",
             "name": "Linux Kernel Variant of OpenIB.org license",
             "reference": "https://spdx.org/licenses/Linux-OpenIB.html",
-            "referenceNumber": 399,
+            "referenceNumber": 25,
             "seeAlso": [
                 "https://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux.git/tree/drivers/infiniband/core/sa.h"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/LOOP.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "LOOP",
+            "name": "Common Lisp LOOP License",
+            "reference": "https://spdx.org/licenses/LOOP.html",
+            "referenceNumber": 357,
+            "seeAlso": [
+                "https://gitlab.com/embeddable-common-lisp/ecl/-/blob/develop/src/lsp/loop.lsp",
+                "http://git.savannah.gnu.org/cgit/gcl.git/tree/gcl/lsp/gcl_loop.lsp?h=Version_2_6_13pre",
+                "https://sourceforge.net/p/sbcl/sbcl/ci/master/tree/src/code/loop.lisp",
+                "https://github.com/cl-adams/adams/blob/master/LICENSE.md",
+                "https://github.com/blakemcbride/eclipse-lisp/blob/master/lisp/loop.lisp",
+                "https://gitlab.common-lisp.net/cmucl/cmucl/-/blob/master/src/code/loop.lisp"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/LPL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "LPL-1.0",
             "name": "Lucent Public License Version 1.0",
             "reference": "https://spdx.org/licenses/LPL-1.0.html",
-            "referenceNumber": 292,
+            "referenceNumber": 102,
             "seeAlso": [
                 "https://opensource.org/licenses/LPL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LPL-1.02.json",
             "isDeprecatedLicenseId": false,
@@ -3785,78 +4187,78 @@
         {
             "detailsUrl": "https://spdx.org/licenses/LPPL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "LPPL-1.0",
             "name": "LaTeX Project Public License v1.0",
             "reference": "https://spdx.org/licenses/LPPL-1.0.html",
-            "referenceNumber": 462,
+            "referenceNumber": 541,
             "seeAlso": [
                 "http://www.latex-project.org/lppl/lppl-1-0.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LPPL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "LPPL-1.1",
             "name": "LaTeX Project Public License v1.1",
             "reference": "https://spdx.org/licenses/LPPL-1.1.html",
-            "referenceNumber": 239,
+            "referenceNumber": 99,
             "seeAlso": [
                 "http://www.latex-project.org/lppl/lppl-1-1.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LPPL-1.2.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "LPPL-1.2",
             "name": "LaTeX Project Public License v1.2",
             "reference": "https://spdx.org/licenses/LPPL-1.2.html",
-            "referenceNumber": 424,
+            "referenceNumber": 429,
             "seeAlso": [
                 "http://www.latex-project.org/lppl/lppl-1-2.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LPPL-1.3a.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "LPPL-1.3a",
             "name": "LaTeX Project Public License v1.3a",
             "reference": "https://spdx.org/licenses/LPPL-1.3a.html",
-            "referenceNumber": 218,
+            "referenceNumber": 516,
             "seeAlso": [
                 "http://www.latex-project.org/lppl/lppl-1-3a.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LPPL-1.3c.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "LPPL-1.3c",
             "name": "LaTeX Project Public License v1.3c",
             "reference": "https://spdx.org/licenses/LPPL-1.3c.html",
-            "referenceNumber": 145,
+            "referenceNumber": 237,
             "seeAlso": [
                 "http://www.latex-project.org/lppl/lppl-1-3c.txt",
                 "https://opensource.org/licenses/LPPL-1.3c"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LZMA-SDK-9.11-to-9.20.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "LZMA-SDK-9.11-to-9.20",
             "name": "LZMA SDK License (versions 9.11 to 9.20)",
             "reference": "https://spdx.org/licenses/LZMA-SDK-9.11-to-9.20.html",
-            "referenceNumber": 370,
+            "referenceNumber": 431,
             "seeAlso": [
                 "https://www.7-zip.org/sdk.html",
                 "https://sourceforge.net/projects/sevenzip/files/LZMA%20SDK/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/LZMA-SDK-9.22.json",
@@ -3874,2423 +4276,2736 @@
         {
             "detailsUrl": "https://spdx.org/licenses/MakeIndex.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "MakeIndex",
             "name": "MakeIndex License",
             "reference": "https://spdx.org/licenses/MakeIndex.html",
-            "referenceNumber": 356,
+            "referenceNumber": 123,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/MakeIndex"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/Martin-Birgmeier.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Martin-Birgmeier",
+            "name": "Martin Birgmeier License",
+            "reference": "https://spdx.org/licenses/Martin-Birgmeier.html",
+            "referenceNumber": 380,
+            "seeAlso": [
+                "https://github.com/Perl/perl5/blob/blead/util.c#L6136"
+            ]
+        },
+        {
+            "detailsUrl": "https://spdx.org/licenses/metamail.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "metamail",
+            "name": "metamail License",
+            "reference": "https://spdx.org/licenses/metamail.html",
+            "referenceNumber": 474,
+            "seeAlso": [
+                "https://github.com/Dual-Life/mime-base64/blob/master/Base64.xs#L12"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Minpack.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Minpack",
             "name": "Minpack License",
             "reference": "https://spdx.org/licenses/Minpack.html",
-            "referenceNumber": 495,
+            "referenceNumber": 300,
             "seeAlso": [
                 "http://www.netlib.org/minpack/disclaimer",
                 "https://gitlab.com/libeigen/eigen/-/blob/master/COPYING.MINPACK"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MirOS.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "MirOS",
             "name": "The MirOS Licence",
             "reference": "https://spdx.org/licenses/MirOS.html",
-            "referenceNumber": 391,
+            "referenceNumber": 443,
             "seeAlso": [
                 "https://opensource.org/licenses/MirOS"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MIT.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "MIT",
             "name": "MIT License",
             "reference": "https://spdx.org/licenses/MIT.html",
-            "referenceNumber": 141,
+            "referenceNumber": 223,
             "seeAlso": [
                 "https://opensource.org/licenses/MIT"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MIT-0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "MIT-0",
             "name": "MIT No Attribution",
             "reference": "https://spdx.org/licenses/MIT-0.html",
-            "referenceNumber": 487,
+            "referenceNumber": 369,
             "seeAlso": [
                 "https://github.com/aws/mit-0",
                 "https://romanrm.net/mit-zero",
                 "https://github.com/awsdocs/aws-cloud9-user-guide/blob/master/LICENSE-SAMPLECODE"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MIT-advertising.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "MIT-advertising",
             "name": "Enlightenment License (e16)",
             "reference": "https://spdx.org/licenses/MIT-advertising.html",
-            "referenceNumber": 44,
+            "referenceNumber": 382,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/MIT_With_Advertising"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MIT-CMU.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "MIT-CMU",
             "name": "CMU License",
             "reference": "https://spdx.org/licenses/MIT-CMU.html",
-            "referenceNumber": 84,
+            "referenceNumber": 24,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing:MIT?rd=Licensing/MIT#CMU_Style",
                 "https://github.com/python-pillow/Pillow/blob/fffb426092c8db24a5f4b6df243a8a3c01fb63cd/LICENSE"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MIT-enna.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "MIT-enna",
             "name": "enna License",
             "reference": "https://spdx.org/licenses/MIT-enna.html",
-            "referenceNumber": 401,
+            "referenceNumber": 465,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/MIT#enna"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MIT-feh.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "MIT-feh",
             "name": "feh License",
             "reference": "https://spdx.org/licenses/MIT-feh.html",
-            "referenceNumber": 55,
+            "referenceNumber": 234,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/MIT#feh"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/MIT-Festival.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "MIT-Festival",
+            "name": "MIT Festival Variant",
+            "reference": "https://spdx.org/licenses/MIT-Festival.html",
+            "referenceNumber": 423,
+            "seeAlso": [
+                "https://github.com/festvox/flite/blob/master/COPYING",
+                "https://github.com/festvox/speech_tools/blob/master/COPYING"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/MIT-Modern-Variant.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "MIT-Modern-Variant",
             "name": "MIT License Modern Variant",
             "reference": "https://spdx.org/licenses/MIT-Modern-Variant.html",
-            "referenceNumber": 475,
+            "referenceNumber": 548,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing:MIT#Modern_Variants",
                 "https://ptolemy.berkeley.edu/copyright.htm",
                 "https://pirlwww.lpl.arizona.edu/resources/guide/software/PerlTk/Tixlic.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MIT-open-group.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "MIT-open-group",
             "name": "MIT Open Group variant",
             "reference": "https://spdx.org/licenses/MIT-open-group.html",
-            "referenceNumber": 481,
+            "referenceNumber": 46,
             "seeAlso": [
                 "https://gitlab.freedesktop.org/xorg/app/iceauth/-/blob/master/COPYING",
                 "https://gitlab.freedesktop.org/xorg/app/xvinfo/-/blob/master/COPYING",
                 "https://gitlab.freedesktop.org/xorg/app/xsetroot/-/blob/master/COPYING",
                 "https://gitlab.freedesktop.org/xorg/app/xauth/-/blob/master/COPYING"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/MIT-Wu.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "MIT-Wu",
+            "name": "MIT Tom Wu Variant",
+            "reference": "https://spdx.org/licenses/MIT-Wu.html",
+            "referenceNumber": 421,
+            "seeAlso": [
+                "https://github.com/chromium/octane/blob/master/crypto.js"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/MITNFA.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "MITNFA",
             "name": "MIT +no-false-attribs license",
             "reference": "https://spdx.org/licenses/MITNFA.html",
-            "referenceNumber": 62,
+            "referenceNumber": 145,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/MITNFA"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Motosoto.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "Motosoto",
             "name": "Motosoto License",
             "reference": "https://spdx.org/licenses/Motosoto.html",
-            "referenceNumber": 386,
+            "referenceNumber": 358,
             "seeAlso": [
                 "https://opensource.org/licenses/Motosoto"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/mpi-permissive.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "mpi-permissive",
             "name": "mpi Permissive License",
             "reference": "https://spdx.org/licenses/mpi-permissive.html",
-            "referenceNumber": 35,
+            "referenceNumber": 295,
             "seeAlso": [
                 "https://sources.debian.org/src/openmpi/4.1.0-10/ompi/debuggers/msgq_interface.h/?hl=19#L19"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/mpich2.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "mpich2",
             "name": "mpich2 License",
             "reference": "https://spdx.org/licenses/mpich2.html",
-            "referenceNumber": 421,
+            "referenceNumber": 281,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/MIT"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MPL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "MPL-1.0",
             "name": "Mozilla Public License 1.0",
             "reference": "https://spdx.org/licenses/MPL-1.0.html",
-            "referenceNumber": 210,
+            "referenceNumber": 94,
             "seeAlso": [
                 "http://www.mozilla.org/MPL/MPL-1.0.html",
                 "https://opensource.org/licenses/MPL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MPL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "MPL-1.1",
             "name": "Mozilla Public License 1.1",
             "reference": "https://spdx.org/licenses/MPL-1.1.html",
-            "referenceNumber": 83,
+            "referenceNumber": 192,
             "seeAlso": [
                 "http://www.mozilla.org/MPL/MPL-1.1.html",
                 "https://opensource.org/licenses/MPL-1.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MPL-2.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "MPL-2.0",
             "name": "Mozilla Public License 2.0",
             "reference": "https://spdx.org/licenses/MPL-2.0.html",
-            "referenceNumber": 331,
+            "referenceNumber": 236,
             "seeAlso": [
                 "https://www.mozilla.org/MPL/2.0/",
                 "https://opensource.org/licenses/MPL-2.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MPL-2.0-no-copyleft-exception.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "MPL-2.0-no-copyleft-exception",
             "name": "Mozilla Public License 2.0 (no copyleft exception)",
             "reference": "https://spdx.org/licenses/MPL-2.0-no-copyleft-exception.html",
-            "referenceNumber": 108,
+            "referenceNumber": 67,
             "seeAlso": [
                 "https://www.mozilla.org/MPL/2.0/",
                 "https://opensource.org/licenses/MPL-2.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/mplus.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "mplus",
             "name": "mplus Font License",
             "reference": "https://spdx.org/licenses/mplus.html",
-            "referenceNumber": 335,
+            "referenceNumber": 157,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing:Mplus?rd=Licensing/mplus"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MS-LPL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "MS-LPL",
             "name": "Microsoft Limited Public License",
             "reference": "https://spdx.org/licenses/MS-LPL.html",
-            "referenceNumber": 148,
+            "referenceNumber": 181,
             "seeAlso": [
                 "https://www.openhub.net/licenses/mslpl",
                 "https://github.com/gabegundy/atlserver/blob/master/License.txt",
                 "https://en.wikipedia.org/wiki/Shared_Source_Initiative#Microsoft_Limited_Public_License_(Ms-LPL)"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MS-PL.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "MS-PL",
             "name": "Microsoft Public License",
             "reference": "https://spdx.org/licenses/MS-PL.html",
-            "referenceNumber": 293,
+            "referenceNumber": 345,
             "seeAlso": [
                 "http://www.microsoft.com/opensource/licenses.mspx",
                 "https://opensource.org/licenses/MS-PL"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MS-RL.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "MS-RL",
             "name": "Microsoft Reciprocal License",
             "reference": "https://spdx.org/licenses/MS-RL.html",
-            "referenceNumber": 267,
+            "referenceNumber": 23,
             "seeAlso": [
                 "http://www.microsoft.com/opensource/licenses.mspx",
                 "https://opensource.org/licenses/MS-RL"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MTLL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "MTLL",
             "name": "Matrix Template Library License",
             "reference": "https://spdx.org/licenses/MTLL.html",
-            "referenceNumber": 194,
+            "referenceNumber": 80,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Matrix_Template_Library_License"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MulanPSL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "MulanPSL-1.0",
             "name": "Mulan Permissive Software License, Version 1",
             "reference": "https://spdx.org/licenses/MulanPSL-1.0.html",
-            "referenceNumber": 235,
+            "referenceNumber": 290,
             "seeAlso": [
                 "https://license.coscl.org.cn/MulanPSL/",
                 "https://github.com/yuwenlong/longphp/blob/25dfb70cc2a466dc4bb55ba30901cbce08d164b5/LICENSE"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/MulanPSL-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "MulanPSL-2.0",
             "name": "Mulan Permissive Software License, Version 2",
             "reference": "https://spdx.org/licenses/MulanPSL-2.0.html",
-            "referenceNumber": 23,
+            "referenceNumber": 490,
             "seeAlso": [
                 "https://license.coscl.org.cn/MulanPSL2/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Multics.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "Multics",
             "name": "Multics License",
             "reference": "https://spdx.org/licenses/Multics.html",
-            "referenceNumber": 215,
+            "referenceNumber": 247,
             "seeAlso": [
                 "https://opensource.org/licenses/Multics"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Mup.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Mup",
             "name": "Mup License",
             "reference": "https://spdx.org/licenses/Mup.html",
-            "referenceNumber": 63,
+            "referenceNumber": 480,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Mup"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NAIST-2003.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "NAIST-2003",
             "name": "Nara Institute of Science and Technology License (2003)",
             "reference": "https://spdx.org/licenses/NAIST-2003.html",
-            "referenceNumber": 471,
+            "referenceNumber": 39,
             "seeAlso": [
                 "https://enterprise.dejacode.com/licenses/public/naist-2003/#license-text",
                 "https://github.com/nodejs/node/blob/4a19cc8947b1bba2b2d27816ec3d0edf9b28e503/LICENSE#L343"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NASA-1.3.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": true,
             "licenseId": "NASA-1.3",
             "name": "NASA Open Source Agreement 1.3",
             "reference": "https://spdx.org/licenses/NASA-1.3.html",
-            "referenceNumber": 380,
+            "referenceNumber": 360,
             "seeAlso": [
                 "http://ti.arc.nasa.gov/opensource/nosa/",
                 "https://opensource.org/licenses/NASA-1.3"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Naumen.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "Naumen",
             "name": "Naumen Public License",
             "reference": "https://spdx.org/licenses/Naumen.html",
-            "referenceNumber": 233,
+            "referenceNumber": 339,
             "seeAlso": [
                 "https://opensource.org/licenses/Naumen"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NBPL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "NBPL-1.0",
             "name": "Net Boolean Public License v1",
             "reference": "https://spdx.org/licenses/NBPL-1.0.html",
-            "referenceNumber": 373,
+            "referenceNumber": 517,
             "seeAlso": [
                 "http://www.openldap.org/devel/gitweb.cgi?p=openldap.git;a=blob;f=LICENSE;hb=37b4b3f6cc4bf34e1d3dec61e69914b9819d8894"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NCGL-UK-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "NCGL-UK-2.0",
             "name": "Non-Commercial Government Licence",
             "reference": "https://spdx.org/licenses/NCGL-UK-2.0.html",
-            "referenceNumber": 140,
+            "referenceNumber": 113,
             "seeAlso": [
                 "http://www.nationalarchives.gov.uk/doc/non-commercial-government-licence/version/2/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NCSA.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "NCSA",
             "name": "University of Illinois/NCSA Open Source License",
             "reference": "https://spdx.org/licenses/NCSA.html",
-            "referenceNumber": 229,
+            "referenceNumber": 199,
             "seeAlso": [
                 "http://otm.illinois.edu/uiuc_openSource",
                 "https://opensource.org/licenses/NCSA"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Net-SNMP.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Net-SNMP",
             "name": "Net-SNMP License",
             "reference": "https://spdx.org/licenses/Net-SNMP.html",
-            "referenceNumber": 101,
+            "referenceNumber": 74,
             "seeAlso": [
                 "http://net-snmp.sourceforge.net/about/license.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NetCDF.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "NetCDF",
             "name": "NetCDF license",
             "reference": "https://spdx.org/licenses/NetCDF.html",
-            "referenceNumber": 304,
+            "referenceNumber": 321,
             "seeAlso": [
                 "http://www.unidata.ucar.edu/software/netcdf/copyright.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Newsletr.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Newsletr",
             "name": "Newsletr License",
             "reference": "https://spdx.org/licenses/Newsletr.html",
-            "referenceNumber": 66,
+            "referenceNumber": 539,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Newsletr"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NGPL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "NGPL",
             "name": "Nethack General Public License",
             "reference": "https://spdx.org/licenses/NGPL.html",
-            "referenceNumber": 200,
+            "referenceNumber": 301,
             "seeAlso": [
                 "https://opensource.org/licenses/NGPL"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NICTA-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "NICTA-1.0",
             "name": "NICTA Public Software License, Version 1.0",
             "reference": "https://spdx.org/licenses/NICTA-1.0.html",
-            "referenceNumber": 120,
+            "referenceNumber": 545,
             "seeAlso": [
                 "https://opensource.apple.com/source/mDNSResponder/mDNSResponder-320.10/mDNSPosix/nss_ReadMe.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NIST-PD.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "NIST-PD",
             "name": "NIST Public Domain Notice",
             "reference": "https://spdx.org/licenses/NIST-PD.html",
-            "referenceNumber": 142,
+            "referenceNumber": 346,
             "seeAlso": [
                 "https://github.com/tcheneau/simpleRPL/blob/e645e69e38dd4e3ccfeceb2db8cba05b7c2e0cd3/LICENSE.txt",
                 "https://github.com/tcheneau/Routing/blob/f09f46fcfe636107f22f2c98348188a65a135d98/README.md"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NIST-PD-fallback.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "NIST-PD-fallback",
             "name": "NIST Public Domain Notice with license fallback",
             "reference": "https://spdx.org/licenses/NIST-PD-fallback.html",
-            "referenceNumber": 24,
+            "referenceNumber": 319,
             "seeAlso": [
                 "https://github.com/usnistgov/jsip/blob/59700e6926cbe96c5cdae897d9a7d2656b42abe3/LICENSE",
                 "https://github.com/usnistgov/fipy/blob/86aaa5c2ba2c6f1be19593c5986071cf6568cc34/LICENSE.rst"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/NIST-Software.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "NIST-Software",
+            "name": "NIST Software License",
+            "reference": "https://spdx.org/licenses/NIST-Software.html",
+            "referenceNumber": 413,
+            "seeAlso": [
+                "https://github.com/open-quantum-safe/liboqs/blob/40b01fdbb270f8614fde30e65d30e9da18c02393/src/common/rand/rand_nist.c#L1-L15"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/NLOD-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "NLOD-1.0",
             "name": "Norwegian Licence for Open Government Data (NLOD) 1.0",
             "reference": "https://spdx.org/licenses/NLOD-1.0.html",
-            "referenceNumber": 412,
+            "referenceNumber": 525,
             "seeAlso": [
                 "http://data.norge.no/nlod/en/1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NLOD-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "NLOD-2.0",
             "name": "Norwegian Licence for Open Government Data (NLOD) 2.0",
             "reference": "https://spdx.org/licenses/NLOD-2.0.html",
-            "referenceNumber": 113,
+            "referenceNumber": 52,
             "seeAlso": [
                 "http://data.norge.no/nlod/en/2.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NLPL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "NLPL",
             "name": "No Limit Public License",
             "reference": "https://spdx.org/licenses/NLPL.html",
-            "referenceNumber": 162,
+            "referenceNumber": 529,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/NLPL"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Nokia.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "Nokia",
             "name": "Nokia Open Source License",
             "reference": "https://spdx.org/licenses/Nokia.html",
-            "referenceNumber": 378,
+            "referenceNumber": 88,
             "seeAlso": [
                 "https://opensource.org/licenses/nokia"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NOSL.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "NOSL",
             "name": "Netizen Open Source License",
             "reference": "https://spdx.org/licenses/NOSL.html",
-            "referenceNumber": 291,
+            "referenceNumber": 417,
             "seeAlso": [
                 "http://bits.netizen.com.au/licenses/NOSL/nosl.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Noweb.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Noweb",
             "name": "Noweb License",
             "reference": "https://spdx.org/licenses/Noweb.html",
-            "referenceNumber": 428,
+            "referenceNumber": 398,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Noweb"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NPL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "NPL-1.0",
             "name": "Netscape Public License v1.0",
             "reference": "https://spdx.org/licenses/NPL-1.0.html",
-            "referenceNumber": 222,
+            "referenceNumber": 53,
             "seeAlso": [
                 "http://www.mozilla.org/MPL/NPL/1.0/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NPL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "NPL-1.1",
             "name": "Netscape Public License v1.1",
             "reference": "https://spdx.org/licenses/NPL-1.1.html",
-            "referenceNumber": 50,
+            "referenceNumber": 51,
             "seeAlso": [
                 "http://www.mozilla.org/MPL/NPL/1.1/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NPOSL-3.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "NPOSL-3.0",
             "name": "Non-Profit Open Software License 3.0",
             "reference": "https://spdx.org/licenses/NPOSL-3.0.html",
-            "referenceNumber": 493,
+            "referenceNumber": 555,
             "seeAlso": [
                 "https://opensource.org/licenses/NOSL3.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NRL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "NRL",
             "name": "NRL License",
             "reference": "https://spdx.org/licenses/NRL.html",
-            "referenceNumber": 217,
+            "referenceNumber": 458,
             "seeAlso": [
                 "http://web.mit.edu/network/isakmp/nrllicense.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NTP.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "NTP",
             "name": "NTP License",
             "reference": "https://spdx.org/licenses/NTP.html",
-            "referenceNumber": 179,
+            "referenceNumber": 2,
             "seeAlso": [
                 "https://opensource.org/licenses/NTP"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/NTP-0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "NTP-0",
             "name": "NTP No Attribution",
             "reference": "https://spdx.org/licenses/NTP-0.html",
-            "referenceNumber": 274,
+            "referenceNumber": 476,
             "seeAlso": [
                 "https://github.com/tytso/e2fsprogs/blob/master/lib/et/et_name.c"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Nunit.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "Nunit",
             "name": "Nunit License",
             "reference": "https://spdx.org/licenses/Nunit.html",
-            "referenceNumber": 441,
+            "referenceNumber": 456,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Nunit"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/O-UDA-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "O-UDA-1.0",
             "name": "Open Use of Data Agreement v1.0",
             "reference": "https://spdx.org/licenses/O-UDA-1.0.html",
-            "referenceNumber": 89,
+            "referenceNumber": 542,
             "seeAlso": [
                 "https://github.com/microsoft/Open-Use-of-Data-Agreement/blob/v1.0/O-UDA-1.0.md",
                 "https://cdla.dev/open-use-of-data-agreement-v1-0/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OCCT-PL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OCCT-PL",
             "name": "Open CASCADE Technology Public License",
             "reference": "https://spdx.org/licenses/OCCT-PL.html",
-            "referenceNumber": 260,
+            "referenceNumber": 309,
             "seeAlso": [
                 "http://www.opencascade.com/content/occt-public-license"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OCLC-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "OCLC-2.0",
             "name": "OCLC Research Public License 2.0",
             "reference": "https://spdx.org/licenses/OCLC-2.0.html",
-            "referenceNumber": 436,
+            "referenceNumber": 370,
             "seeAlso": [
                 "http://www.oclc.org/research/activities/software/license/v2final.htm",
                 "https://opensource.org/licenses/OCLC-2.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/ODbL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "ODbL-1.0",
             "name": "Open Data Commons Open Database License v1.0",
             "reference": "https://spdx.org/licenses/ODbL-1.0.html",
-            "referenceNumber": 223,
+            "referenceNumber": 356,
             "seeAlso": [
                 "http://www.opendatacommons.org/licenses/odbl/1.0/",
                 "https://opendatacommons.org/licenses/odbl/1-0/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/ODC-By-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "ODC-By-1.0",
             "name": "Open Data Commons Attribution License v1.0",
             "reference": "https://spdx.org/licenses/ODC-By-1.0.html",
-            "referenceNumber": 116,
+            "referenceNumber": 64,
             "seeAlso": [
                 "https://opendatacommons.org/licenses/by/1.0/"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/OFFIS.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "OFFIS",
+            "name": "OFFIS License",
+            "reference": "https://spdx.org/licenses/OFFIS.html",
+            "referenceNumber": 104,
+            "seeAlso": [
+                "https://sourceforge.net/p/xmedcon/code/ci/master/tree/libs/dicom/README"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/OFL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "OFL-1.0",
             "name": "SIL Open Font License 1.0",
             "reference": "https://spdx.org/licenses/OFL-1.0.html",
-            "referenceNumber": 137,
+            "referenceNumber": 419,
             "seeAlso": [
                 "http://scripts.sil.org/cms/scripts/page.php?item_id=OFL10_web"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OFL-1.0-no-RFN.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OFL-1.0-no-RFN",
             "name": "SIL Open Font License 1.0 with no Reserved Font Name",
             "reference": "https://spdx.org/licenses/OFL-1.0-no-RFN.html",
-            "referenceNumber": 455,
+            "referenceNumber": 354,
             "seeAlso": [
                 "http://scripts.sil.org/cms/scripts/page.php?item_id=OFL10_web"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OFL-1.0-RFN.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OFL-1.0-RFN",
             "name": "SIL Open Font License 1.0 with Reserved Font Name",
             "reference": "https://spdx.org/licenses/OFL-1.0-RFN.html",
-            "referenceNumber": 252,
+            "referenceNumber": 250,
             "seeAlso": [
                 "http://scripts.sil.org/cms/scripts/page.php?item_id=OFL10_web"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OFL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "OFL-1.1",
             "name": "SIL Open Font License 1.1",
             "reference": "https://spdx.org/licenses/OFL-1.1.html",
-            "referenceNumber": 300,
+            "referenceNumber": 3,
             "seeAlso": [
                 "http://scripts.sil.org/cms/scripts/page.php?item_id=OFL_web",
                 "https://opensource.org/licenses/OFL-1.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OFL-1.1-no-RFN.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "OFL-1.1-no-RFN",
             "name": "SIL Open Font License 1.1 with no Reserved Font Name",
             "reference": "https://spdx.org/licenses/OFL-1.1-no-RFN.html",
-            "referenceNumber": 73,
+            "referenceNumber": 117,
             "seeAlso": [
                 "http://scripts.sil.org/cms/scripts/page.php?item_id=OFL_web",
                 "https://opensource.org/licenses/OFL-1.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OFL-1.1-RFN.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "OFL-1.1-RFN",
             "name": "SIL Open Font License 1.1 with Reserved Font Name",
             "reference": "https://spdx.org/licenses/OFL-1.1-RFN.html",
-            "referenceNumber": 3,
+            "referenceNumber": 518,
             "seeAlso": [
                 "http://scripts.sil.org/cms/scripts/page.php?item_id=OFL_web",
                 "https://opensource.org/licenses/OFL-1.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OGC-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OGC-1.0",
             "name": "OGC Software License, Version 1.0",
             "reference": "https://spdx.org/licenses/OGC-1.0.html",
-            "referenceNumber": 64,
+            "referenceNumber": 15,
             "seeAlso": [
                 "https://www.ogc.org/ogc/software/1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OGDL-Taiwan-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OGDL-Taiwan-1.0",
             "name": "Taiwan Open Government Data License, version 1.0",
             "reference": "https://spdx.org/licenses/OGDL-Taiwan-1.0.html",
-            "referenceNumber": 288,
+            "referenceNumber": 284,
             "seeAlso": [
                 "https://data.gov.tw/license"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OGL-Canada-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OGL-Canada-2.0",
             "name": "Open Government Licence - Canada",
             "reference": "https://spdx.org/licenses/OGL-Canada-2.0.html",
-            "referenceNumber": 196,
+            "referenceNumber": 214,
             "seeAlso": [
                 "https://open.canada.ca/en/open-government-licence-canada"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OGL-UK-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OGL-UK-1.0",
             "name": "Open Government Licence v1.0",
             "reference": "https://spdx.org/licenses/OGL-UK-1.0.html",
-            "referenceNumber": 26,
+            "referenceNumber": 165,
             "seeAlso": [
                 "http://www.nationalarchives.gov.uk/doc/open-government-licence/version/1/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OGL-UK-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OGL-UK-2.0",
             "name": "Open Government Licence v2.0",
             "reference": "https://spdx.org/licenses/OGL-UK-2.0.html",
-            "referenceNumber": 118,
+            "referenceNumber": 304,
             "seeAlso": [
                 "http://www.nationalarchives.gov.uk/doc/open-government-licence/version/2/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OGL-UK-3.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OGL-UK-3.0",
             "name": "Open Government Licence v3.0",
             "reference": "https://spdx.org/licenses/OGL-UK-3.0.html",
-            "referenceNumber": 192,
+            "referenceNumber": 415,
             "seeAlso": [
                 "http://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OGTSL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "OGTSL",
             "name": "Open Group Test Suite License",
             "reference": "https://spdx.org/licenses/OGTSL.html",
-            "referenceNumber": 99,
+            "referenceNumber": 133,
             "seeAlso": [
                 "http://www.opengroup.org/testing/downloads/The_Open_Group_TSL.txt",
                 "https://opensource.org/licenses/OGTSL"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OLDAP-1.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OLDAP-1.1",
             "name": "Open LDAP Public License v1.1",
             "reference": "https://spdx.org/licenses/OLDAP-1.1.html",
-            "referenceNumber": 366,
+            "referenceNumber": 208,
             "seeAlso": [
                 "http://www.openldap.org/devel/gitweb.cgi?p=openldap.git;a=blob;f=LICENSE;hb=806557a5ad59804ef3a44d5abfbe91d706b0791f"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OLDAP-1.2.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OLDAP-1.2",
             "name": "Open LDAP Public License v1.2",
             "reference": "https://spdx.org/licenses/OLDAP-1.2.html",
-            "referenceNumber": 388,
+            "referenceNumber": 100,
             "seeAlso": [
                 "http://www.openldap.org/devel/gitweb.cgi?p=openldap.git;a=blob;f=LICENSE;hb=42b0383c50c299977b5893ee695cf4e486fb0dc7"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OLDAP-1.3.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OLDAP-1.3",
             "name": "Open LDAP Public License v1.3",
             "reference": "https://spdx.org/licenses/OLDAP-1.3.html",
-            "referenceNumber": 460,
+            "referenceNumber": 328,
             "seeAlso": [
                 "http://www.openldap.org/devel/gitweb.cgi?p=openldap.git;a=blob;f=LICENSE;hb=e5f8117f0ce088d0bd7a8e18ddf37eaa40eb09b1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OLDAP-1.4.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OLDAP-1.4",
             "name": "Open LDAP Public License v1.4",
             "reference": "https://spdx.org/licenses/OLDAP-1.4.html",
-            "referenceNumber": 477,
+            "referenceNumber": 333,
             "seeAlso": [
                 "http://www.openldap.org/devel/gitweb.cgi?p=openldap.git;a=blob;f=LICENSE;hb=c9f95c2f3f2ffb5e0ae55fe7388af75547660941"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OLDAP-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OLDAP-2.0",
             "name": "Open LDAP Public License v2.0 (or possibly 2.0A and 2.0B)",
             "reference": "https://spdx.org/licenses/OLDAP-2.0.html",
-            "referenceNumber": 414,
+            "referenceNumber": 519,
             "seeAlso": [
                 "http://www.openldap.org/devel/gitweb.cgi?p=openldap.git;a=blob;f=LICENSE;hb=cbf50f4e1185a21abd4c0a54d3f4341fe28f36ea"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OLDAP-2.0.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OLDAP-2.0.1",
             "name": "Open LDAP Public License v2.0.1",
             "reference": "https://spdx.org/licenses/OLDAP-2.0.1.html",
-            "referenceNumber": 40,
+            "referenceNumber": 324,
             "seeAlso": [
                 "http://www.openldap.org/devel/gitweb.cgi?p=openldap.git;a=blob;f=LICENSE;hb=b6d68acd14e51ca3aab4428bf26522aa74873f0e"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OLDAP-2.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OLDAP-2.1",
             "name": "Open LDAP Public License v2.1",
             "reference": "https://spdx.org/licenses/OLDAP-2.1.html",
-            "referenceNumber": 479,
+            "referenceNumber": 402,
             "seeAlso": [
                 "http://www.openldap.org/devel/gitweb.cgi?p=openldap.git;a=blob;f=LICENSE;hb=b0d176738e96a0d3b9f85cb51e140a86f21be715"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OLDAP-2.2.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OLDAP-2.2",
             "name": "Open LDAP Public License v2.2",
             "reference": "https://spdx.org/licenses/OLDAP-2.2.html",
-            "referenceNumber": 413,
+            "referenceNumber": 163,
             "seeAlso": [
                 "http://www.openldap.org/devel/gitweb.cgi?p=openldap.git;a=blob;f=LICENSE;hb=470b0c18ec67621c85881b2733057fecf4a1acc3"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OLDAP-2.2.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OLDAP-2.2.1",
             "name": "Open LDAP Public License v2.2.1",
             "reference": "https://spdx.org/licenses/OLDAP-2.2.1.html",
-            "referenceNumber": 353,
+            "referenceNumber": 451,
             "seeAlso": [
                 "http://www.openldap.org/devel/gitweb.cgi?p=openldap.git;a=blob;f=LICENSE;hb=4bc786f34b50aa301be6f5600f58a980070f481e"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OLDAP-2.2.2.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OLDAP-2.2.2",
             "name": "Open LDAP Public License 2.2.2",
             "reference": "https://spdx.org/licenses/OLDAP-2.2.2.html",
-            "referenceNumber": 279,
+            "referenceNumber": 140,
             "seeAlso": [
                 "http://www.openldap.org/devel/gitweb.cgi?p=openldap.git;a=blob;f=LICENSE;hb=df2cc1e21eb7c160695f5b7cffd6296c151ba188"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OLDAP-2.3.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "OLDAP-2.3",
             "name": "Open LDAP Public License v2.3",
             "reference": "https://spdx.org/licenses/OLDAP-2.3.html",
-            "referenceNumber": 338,
+            "referenceNumber": 33,
             "seeAlso": [
                 "http://www.openldap.org/devel/gitweb.cgi?p=openldap.git;a=blob;f=LICENSE;hb=d32cf54a32d581ab475d23c810b0a7fbaf8d63c3"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OLDAP-2.4.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OLDAP-2.4",
             "name": "Open LDAP Public License v2.4",
             "reference": "https://spdx.org/licenses/OLDAP-2.4.html",
-            "referenceNumber": 174,
+            "referenceNumber": 447,
             "seeAlso": [
                 "http://www.openldap.org/devel/gitweb.cgi?p=openldap.git;a=blob;f=LICENSE;hb=cd1284c4a91a8a380d904eee68d1583f989ed386"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OLDAP-2.5.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OLDAP-2.5",
             "name": "Open LDAP Public License v2.5",
             "reference": "https://spdx.org/licenses/OLDAP-2.5.html",
-            "referenceNumber": 185,
+            "referenceNumber": 549,
             "seeAlso": [
                 "http://www.openldap.org/devel/gitweb.cgi?p=openldap.git;a=blob;f=LICENSE;hb=6852b9d90022e8593c98205413380536b1b5a7cf"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OLDAP-2.6.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OLDAP-2.6",
             "name": "Open LDAP Public License v2.6",
             "reference": "https://spdx.org/licenses/OLDAP-2.6.html",
-            "referenceNumber": 445,
+            "referenceNumber": 297,
             "seeAlso": [
                 "http://www.openldap.org/devel/gitweb.cgi?p=openldap.git;a=blob;f=LICENSE;hb=1cae062821881f41b73012ba816434897abf4205"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OLDAP-2.7.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "OLDAP-2.7",
             "name": "Open LDAP Public License v2.7",
             "reference": "https://spdx.org/licenses/OLDAP-2.7.html",
-            "referenceNumber": 151,
+            "referenceNumber": 134,
             "seeAlso": [
                 "http://www.openldap.org/devel/gitweb.cgi?p=openldap.git;a=blob;f=LICENSE;hb=47c2415c1df81556eeb39be6cad458ef87c534a2"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OLDAP-2.8.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "OLDAP-2.8",
             "name": "Open LDAP Public License v2.8",
             "reference": "https://spdx.org/licenses/OLDAP-2.8.html",
-            "referenceNumber": 440,
+            "referenceNumber": 540,
             "seeAlso": [
                 "http://www.openldap.org/software/release/license.html"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/OLFL-1.3.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": true,
+            "licenseId": "OLFL-1.3",
+            "name": "Open Logistics Foundation License Version 1.3",
+            "reference": "https://spdx.org/licenses/OLFL-1.3.html",
+            "referenceNumber": 482,
+            "seeAlso": [
+                "https://openlogisticsfoundation.org/licenses/",
+                "https://opensource.org/license/olfl-1-3/"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/OML.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OML",
             "name": "Open Market License",
             "reference": "https://spdx.org/licenses/OML.html",
-            "referenceNumber": 298,
+            "referenceNumber": 155,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Open_Market_License"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/OpenPBS-2.3.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "OpenPBS-2.3",
+            "name": "OpenPBS v2.3 Software License",
+            "reference": "https://spdx.org/licenses/OpenPBS-2.3.html",
+            "referenceNumber": 377,
+            "seeAlso": [
+                "https://github.com/adaptivecomputing/torque/blob/master/PBS_License.txt",
+                "https://www.mcs.anl.gov/research/projects/openpbs/PBS_License.txt"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/OpenSSL.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "OpenSSL",
             "name": "OpenSSL License",
             "reference": "https://spdx.org/licenses/OpenSSL.html",
-            "referenceNumber": 105,
+            "referenceNumber": 276,
             "seeAlso": [
                 "http://www.openssl.org/source/license.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OPL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": false,
             "licenseId": "OPL-1.0",
             "name": "Open Public License v1.0",
             "reference": "https://spdx.org/licenses/OPL-1.0.html",
-            "referenceNumber": 36,
+            "referenceNumber": 510,
             "seeAlso": [
                 "http://old.koalateam.com/jackaroo/OPL_1_0.TXT",
                 "https://fedoraproject.org/wiki/Licensing/Open_Public_License"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/OPL-UK-3.0.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "OPL-UK-3.0",
+            "name": "United    Kingdom Open Parliament Licence v3.0",
+            "reference": "https://spdx.org/licenses/OPL-UK-3.0.html",
+            "referenceNumber": 257,
+            "seeAlso": [
+                "https://www.parliament.uk/site-information/copyright-parliament/open-parliament-licence/"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/OPUBL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "OPUBL-1.0",
             "name": "Open Publication License v1.0",
             "reference": "https://spdx.org/licenses/OPUBL-1.0.html",
-            "referenceNumber": 161,
+            "referenceNumber": 514,
             "seeAlso": [
                 "http://opencontent.org/openpub/",
                 "https://www.debian.org/opl",
                 "https://www.ctan.org/license/opl"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OSET-PL-2.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "OSET-PL-2.1",
             "name": "OSET Public License version 2.1",
             "reference": "https://spdx.org/licenses/OSET-PL-2.1.html",
-            "referenceNumber": 294,
+            "referenceNumber": 274,
             "seeAlso": [
                 "http://www.osetfoundation.org/public-license",
                 "https://opensource.org/licenses/OPL-2.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OSL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "OSL-1.0",
             "name": "Open Software License 1.0",
             "reference": "https://spdx.org/licenses/OSL-1.0.html",
-            "referenceNumber": 478,
+            "referenceNumber": 371,
             "seeAlso": [
                 "https://opensource.org/licenses/OSL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OSL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "OSL-1.1",
             "name": "Open Software License 1.1",
             "reference": "https://spdx.org/licenses/OSL-1.1.html",
-            "referenceNumber": 325,
+            "referenceNumber": 310,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/OSL1.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OSL-2.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "OSL-2.0",
             "name": "Open Software License 2.0",
             "reference": "https://spdx.org/licenses/OSL-2.0.html",
-            "referenceNumber": 389,
+            "referenceNumber": 405,
             "seeAlso": [
                 "http://web.archive.org/web/20041020171434/http://www.rosenlaw.com/osl2.0.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OSL-2.1.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "OSL-2.1",
             "name": "Open Software License 2.1",
             "reference": "https://spdx.org/licenses/OSL-2.1.html",
-            "referenceNumber": 405,
+            "referenceNumber": 251,
             "seeAlso": [
                 "http://web.archive.org/web/20050212003940/http://www.rosenlaw.com/osl21.htm",
                 "https://opensource.org/licenses/OSL-2.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/OSL-3.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "OSL-3.0",
             "name": "Open Software License 3.0",
             "reference": "https://spdx.org/licenses/OSL-3.0.html",
-            "referenceNumber": 474,
+            "referenceNumber": 20,
             "seeAlso": [
                 "https://web.archive.org/web/20120101081418/http://rosenlaw.com:80/OSL3.0.htm",
                 "https://opensource.org/licenses/OSL-3.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Parity-6.0.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Parity-6.0.0",
             "name": "The Parity Public License 6.0.0",
             "reference": "https://spdx.org/licenses/Parity-6.0.0.html",
-            "referenceNumber": 333,
+            "referenceNumber": 69,
             "seeAlso": [
                 "https://paritylicense.com/versions/6.0.0.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Parity-7.0.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Parity-7.0.0",
             "name": "The Parity Public License 7.0.0",
             "reference": "https://spdx.org/licenses/Parity-7.0.0.html",
-            "referenceNumber": 168,
+            "referenceNumber": 323,
             "seeAlso": [
                 "https://paritylicense.com/versions/7.0.0.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/PDDL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "PDDL-1.0",
             "name": "Open Data Commons Public Domain Dedication & License 1.0",
             "reference": "https://spdx.org/licenses/PDDL-1.0.html",
-            "referenceNumber": 75,
+            "referenceNumber": 42,
             "seeAlso": [
                 "http://opendatacommons.org/licenses/pddl/1.0/",
                 "https://opendatacommons.org/licenses/pddl/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/PHP-3.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "PHP-3.0",
             "name": "PHP License v3.0",
             "reference": "https://spdx.org/licenses/PHP-3.0.html",
-            "referenceNumber": 265,
+            "referenceNumber": 450,
             "seeAlso": [
                 "http://www.php.net/license/3_0.txt",
                 "https://opensource.org/licenses/PHP-3.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/PHP-3.01.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "PHP-3.01",
             "name": "PHP License v3.01",
             "reference": "https://spdx.org/licenses/PHP-3.01.html",
-            "referenceNumber": 126,
+            "referenceNumber": 58,
             "seeAlso": [
                 "http://www.php.net/license/3_01.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Plexus.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Plexus",
             "name": "Plexus Classworlds License",
             "reference": "https://spdx.org/licenses/Plexus.html",
-            "referenceNumber": 94,
+            "referenceNumber": 97,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Plexus_Classworlds_License"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/PolyForm-Noncommercial-1.0.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "PolyForm-Noncommercial-1.0.0",
             "name": "PolyForm Noncommercial License 1.0.0",
             "reference": "https://spdx.org/licenses/PolyForm-Noncommercial-1.0.0.html",
-            "referenceNumber": 98,
+            "referenceNumber": 112,
             "seeAlso": [
                 "https://polyformproject.org/licenses/noncommercial/1.0.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/PolyForm-Small-Business-1.0.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "PolyForm-Small-Business-1.0.0",
             "name": "PolyForm Small Business License 1.0.0",
             "reference": "https://spdx.org/licenses/PolyForm-Small-Business-1.0.0.html",
-            "referenceNumber": 157,
+            "referenceNumber": 161,
             "seeAlso": [
                 "https://polyformproject.org/licenses/small-business/1.0.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/PostgreSQL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "PostgreSQL",
             "name": "PostgreSQL License",
             "reference": "https://spdx.org/licenses/PostgreSQL.html",
-            "referenceNumber": 106,
+            "referenceNumber": 527,
             "seeAlso": [
                 "http://www.postgresql.org/about/licence",
                 "https://opensource.org/licenses/PostgreSQL"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/PSF-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "PSF-2.0",
             "name": "Python Software Foundation License 2.0",
             "reference": "https://spdx.org/licenses/PSF-2.0.html",
-            "referenceNumber": 272,
+            "referenceNumber": 86,
             "seeAlso": [
                 "https://opensource.org/licenses/Python-2.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/psfrag.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "psfrag",
             "name": "psfrag License",
             "reference": "https://spdx.org/licenses/psfrag.html",
-            "referenceNumber": 255,
+            "referenceNumber": 190,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/psfrag"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/psutils.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "psutils",
             "name": "psutils License",
             "reference": "https://spdx.org/licenses/psutils.html",
-            "referenceNumber": 22,
+            "referenceNumber": 27,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/psutils"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Python-2.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "Python-2.0",
             "name": "Python License 2.0",
             "reference": "https://spdx.org/licenses/Python-2.0.html",
-            "referenceNumber": 253,
+            "referenceNumber": 459,
             "seeAlso": [
                 "https://opensource.org/licenses/Python-2.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Python-2.0.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Python-2.0.1",
             "name": "Python License 2.0.1",
             "reference": "https://spdx.org/licenses/Python-2.0.1.html",
-            "referenceNumber": 329,
+            "referenceNumber": 307,
             "seeAlso": [
                 "https://www.python.org/download/releases/2.0.1/license/",
                 "https://docs.python.org/3/license.html",
                 "https://github.com/python/cpython/blob/main/LICENSE"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Qhull.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Qhull",
             "name": "Qhull License",
             "reference": "https://spdx.org/licenses/Qhull.html",
-            "referenceNumber": 18,
+            "referenceNumber": 158,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Qhull"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/QPL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "QPL-1.0",
             "name": "Q Public License 1.0",
             "reference": "https://spdx.org/licenses/QPL-1.0.html",
-            "referenceNumber": 46,
+            "referenceNumber": 472,
             "seeAlso": [
                 "http://doc.qt.nokia.com/3.3/license.html",
                 "https://opensource.org/licenses/QPL-1.0",
                 "https://doc.qt.io/archives/3.3/license.html"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/QPL-1.0-INRIA-2004.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "QPL-1.0-INRIA-2004",
+            "name": "Q Public License 1.0 - INRIA 2004 variant",
+            "reference": "https://spdx.org/licenses/QPL-1.0-INRIA-2004.html",
+            "referenceNumber": 62,
+            "seeAlso": [
+                "https://github.com/maranget/hevea/blob/master/LICENSE"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Rdisc.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Rdisc",
             "name": "Rdisc License",
             "reference": "https://spdx.org/licenses/Rdisc.html",
-            "referenceNumber": 178,
+            "referenceNumber": 224,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Rdisc_License"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/RHeCos-1.1.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": false,
             "licenseId": "RHeCos-1.1",
             "name": "Red Hat eCos Public License v1.1",
             "reference": "https://spdx.org/licenses/RHeCos-1.1.html",
-            "referenceNumber": 12,
+            "referenceNumber": 422,
             "seeAlso": [
                 "http://ecos.sourceware.org/old-license.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/RPL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "RPL-1.1",
             "name": "Reciprocal Public License 1.1",
             "reference": "https://spdx.org/licenses/RPL-1.1.html",
-            "referenceNumber": 262,
+            "referenceNumber": 16,
             "seeAlso": [
                 "https://opensource.org/licenses/RPL-1.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/RPL-1.5.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "RPL-1.5",
             "name": "Reciprocal Public License 1.5",
             "reference": "https://spdx.org/licenses/RPL-1.5.html",
-            "referenceNumber": 69,
+            "referenceNumber": 136,
             "seeAlso": [
                 "https://opensource.org/licenses/RPL-1.5"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/RPSL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "RPSL-1.0",
             "name": "RealNetworks Public Source License v1.0",
             "reference": "https://spdx.org/licenses/RPSL-1.0.html",
-            "referenceNumber": 422,
+            "referenceNumber": 230,
             "seeAlso": [
                 "https://helixcommunity.org/content/rpsl",
                 "https://opensource.org/licenses/RPSL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/RSA-MD.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "RSA-MD",
             "name": "RSA Message-Digest License",
             "reference": "https://spdx.org/licenses/RSA-MD.html",
-            "referenceNumber": 398,
+            "referenceNumber": 506,
             "seeAlso": [
                 "http://www.faqs.org/rfcs/rfc1321.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/RSCPL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "RSCPL",
             "name": "Ricoh Source Code Public License",
             "reference": "https://spdx.org/licenses/RSCPL.html",
-            "referenceNumber": 431,
+            "referenceNumber": 169,
             "seeAlso": [
                 "http://wayback.archive.org/web/20060715140826/http://www.risource.org/RPL/RPL-1.0A.shtml",
                 "https://opensource.org/licenses/RSCPL"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Ruby.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "Ruby",
             "name": "Ruby License",
             "reference": "https://spdx.org/licenses/Ruby.html",
-            "referenceNumber": 276,
+            "referenceNumber": 60,
             "seeAlso": [
                 "http://www.ruby-lang.org/en/LICENSE.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SAX-PD.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "SAX-PD",
             "name": "Sax Public Domain Notice",
             "reference": "https://spdx.org/licenses/SAX-PD.html",
-            "referenceNumber": 251,
+            "referenceNumber": 390,
             "seeAlso": [
                 "http://www.saxproject.org/copying.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Saxpath.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Saxpath",
             "name": "Saxpath License",
             "reference": "https://spdx.org/licenses/Saxpath.html",
-            "referenceNumber": 164,
+            "referenceNumber": 372,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Saxpath_License"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SCEA.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "SCEA",
             "name": "SCEA Shared Source License",
             "reference": "https://spdx.org/licenses/SCEA.html",
-            "referenceNumber": 205,
+            "referenceNumber": 173,
             "seeAlso": [
                 "http://research.scea.com/scea_shared_source_license.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SchemeReport.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "SchemeReport",
             "name": "Scheme Language Report License",
             "reference": "https://spdx.org/licenses/SchemeReport.html",
-            "referenceNumber": 220,
+            "referenceNumber": 38,
             "seeAlso": []
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Sendmail.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Sendmail",
             "name": "Sendmail License",
             "reference": "https://spdx.org/licenses/Sendmail.html",
-            "referenceNumber": 281,
+            "referenceNumber": 18,
             "seeAlso": [
                 "http://www.sendmail.com/pdfs/open_source/sendmail_license.pdf",
                 "https://web.archive.org/web/20160322142305/https://www.sendmail.com/pdfs/open_source/sendmail_license.pdf"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Sendmail-8.23.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Sendmail-8.23",
             "name": "Sendmail License 8.23",
             "reference": "https://spdx.org/licenses/Sendmail-8.23.html",
-            "referenceNumber": 261,
+            "referenceNumber": 344,
             "seeAlso": [
                 "https://www.proofpoint.com/sites/default/files/sendmail-license.pdf",
                 "https://web.archive.org/web/20181003101040/https://www.proofpoint.com/sites/default/files/sendmail-license.pdf"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SGI-B-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "SGI-B-1.0",
             "name": "SGI Free Software License B v1.0",
             "reference": "https://spdx.org/licenses/SGI-B-1.0.html",
-            "referenceNumber": 301,
+            "referenceNumber": 122,
             "seeAlso": [
                 "http://oss.sgi.com/projects/FreeB/SGIFreeSWLicB.1.0.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SGI-B-1.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "SGI-B-1.1",
             "name": "SGI Free Software License B v1.1",
             "reference": "https://spdx.org/licenses/SGI-B-1.1.html",
-            "referenceNumber": 114,
+            "referenceNumber": 330,
             "seeAlso": [
                 "http://oss.sgi.com/projects/FreeB/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SGI-B-2.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "SGI-B-2.0",
             "name": "SGI Free Software License B v2.0",
             "reference": "https://spdx.org/licenses/SGI-B-2.0.html",
-            "referenceNumber": 59,
+            "referenceNumber": 278,
             "seeAlso": [
                 "http://oss.sgi.com/projects/FreeB/SGIFreeSWLicB.2.0.pdf"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/SGP4.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "SGP4",
+            "name": "SGP4 Permission Notice",
+            "reference": "https://spdx.org/licenses/SGP4.html",
+            "referenceNumber": 520,
+            "seeAlso": [
+                "https://celestrak.org/publications/AIAA/2006-6753/faq.php"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/SHL-0.5.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "SHL-0.5",
             "name": "Solderpad Hardware License v0.5",
             "reference": "https://spdx.org/licenses/SHL-0.5.html",
-            "referenceNumber": 102,
+            "referenceNumber": 511,
             "seeAlso": [
                 "https://solderpad.org/licenses/SHL-0.5/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SHL-0.51.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "SHL-0.51",
             "name": "Solderpad Hardware License, Version 0.51",
             "reference": "https://spdx.org/licenses/SHL-0.51.html",
-            "referenceNumber": 317,
+            "referenceNumber": 492,
             "seeAlso": [
                 "https://solderpad.org/licenses/SHL-0.51/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SimPL-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "SimPL-2.0",
             "name": "Simple Public License 2.0",
             "reference": "https://spdx.org/licenses/SimPL-2.0.html",
-            "referenceNumber": 85,
+            "referenceNumber": 387,
             "seeAlso": [
                 "https://opensource.org/licenses/SimPL-2.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SISSL.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "SISSL",
             "name": "Sun Industry Standards Source License v1.1",
             "reference": "https://spdx.org/licenses/SISSL.html",
-            "referenceNumber": 290,
+            "referenceNumber": 186,
             "seeAlso": [
                 "http://www.openoffice.org/licenses/sissl_license.html",
                 "https://opensource.org/licenses/SISSL"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SISSL-1.2.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "SISSL-1.2",
             "name": "Sun Industry Standards Source License v1.2",
             "reference": "https://spdx.org/licenses/SISSL-1.2.html",
-            "referenceNumber": 257,
+            "referenceNumber": 267,
             "seeAlso": [
                 "http://gridscheduler.sourceforge.net/Gridengine_SISSL_license.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Sleepycat.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "Sleepycat",
             "name": "Sleepycat License",
             "reference": "https://spdx.org/licenses/Sleepycat.html",
-            "referenceNumber": 259,
+            "referenceNumber": 162,
             "seeAlso": [
                 "https://opensource.org/licenses/Sleepycat"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SMLNJ.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "SMLNJ",
             "name": "Standard ML of New Jersey License",
             "reference": "https://spdx.org/licenses/SMLNJ.html",
-            "referenceNumber": 454,
+            "referenceNumber": 243,
             "seeAlso": [
                 "https://www.smlnj.org/license.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SMPPL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "SMPPL",
             "name": "Secure Messaging Protocol Public License",
             "reference": "https://spdx.org/licenses/SMPPL.html",
-            "referenceNumber": 68,
+            "referenceNumber": 399,
             "seeAlso": [
                 "https://github.com/dcblake/SMP/blob/master/Documentation/License.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SNIA.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "SNIA",
             "name": "SNIA Public License 1.1",
             "reference": "https://spdx.org/licenses/SNIA.html",
-            "referenceNumber": 131,
+            "referenceNumber": 334,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/SNIA_Public_License"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/snprintf.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "snprintf",
+            "name": "snprintf License",
+            "reference": "https://spdx.org/licenses/snprintf.html",
+            "referenceNumber": 142,
+            "seeAlso": [
+                "https://github.com/openssh/openssh-portable/blob/master/openbsd-compat/bsd-snprintf.c#L2"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Spencer-86.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Spencer-86",
             "name": "Spencer License 86",
             "reference": "https://spdx.org/licenses/Spencer-86.html",
-            "referenceNumber": 470,
+            "referenceNumber": 311,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Henry_Spencer_Reg-Ex_Library_License"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Spencer-94.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Spencer-94",
             "name": "Spencer License 94",
             "reference": "https://spdx.org/licenses/Spencer-94.html",
-            "referenceNumber": 482,
+            "referenceNumber": 394,
             "seeAlso": [
-                "https://fedoraproject.org/wiki/Licensing/Henry_Spencer_Reg-Ex_Library_License"
+                "https://fedoraproject.org/wiki/Licensing/Henry_Spencer_Reg-Ex_Library_License",
+                "https://metacpan.org/release/KNOK/File-MMagic-1.30/source/COPYING#L28"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Spencer-99.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Spencer-99",
             "name": "Spencer License 99",
             "reference": "https://spdx.org/licenses/Spencer-99.html",
-            "referenceNumber": 453,
+            "referenceNumber": 164,
             "seeAlso": [
                 "http://www.opensource.apple.com/source/tcl/tcl-5/tcl/generic/regfronts.c"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SPL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "SPL-1.0",
             "name": "Sun Public License v1.0",
             "reference": "https://spdx.org/licenses/SPL-1.0.html",
-            "referenceNumber": 400,
+            "referenceNumber": 441,
             "seeAlso": [
                 "https://opensource.org/licenses/SPL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SSH-OpenSSH.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "SSH-OpenSSH",
             "name": "SSH OpenSSH license",
             "reference": "https://spdx.org/licenses/SSH-OpenSSH.html",
-            "referenceNumber": 367,
+            "referenceNumber": 481,
             "seeAlso": [
                 "https://github.com/openssh/openssh-portable/blob/1b11ea7c58cd5c59838b5fa574cd456d6047b2d4/LICENCE#L10"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SSH-short.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "SSH-short",
             "name": "SSH short notice",
             "reference": "https://spdx.org/licenses/SSH-short.html",
-            "referenceNumber": 308,
+            "referenceNumber": 151,
             "seeAlso": [
                 "https://github.com/openssh/openssh-portable/blob/1b11ea7c58cd5c59838b5fa574cd456d6047b2d4/pathnames.h",
                 "http://web.mit.edu/kolya/.f/root/athena.mit.edu/sipb.mit.edu/project/openssh/OldFiles/src/openssh-2.9.9p2/ssh-add.1",
                 "https://joinup.ec.europa.eu/svn/lesoll/trunk/italc/lib/src/dsa_key.cpp"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SSPL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "SSPL-1.0",
             "name": "Server Side Public License, v 1",
             "reference": "https://spdx.org/licenses/SSPL-1.0.html",
-            "referenceNumber": 93,
+            "referenceNumber": 218,
             "seeAlso": [
                 "https://www.mongodb.com/licensing/server-side-public-license"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/StandardML-NJ.json",
             "isDeprecatedLicenseId": true,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "StandardML-NJ",
             "name": "Standard ML of New Jersey License",
             "reference": "https://spdx.org/licenses/StandardML-NJ.html",
-            "referenceNumber": 497,
+            "referenceNumber": 299,
             "seeAlso": [
-                "http://www.smlnj.org//license.html"
+                "https://www.smlnj.org/license.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/SugarCRM-1.1.3.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "SugarCRM-1.1.3",
             "name": "SugarCRM Public License v1.1.3",
             "reference": "https://spdx.org/licenses/SugarCRM-1.1.3.html",
-            "referenceNumber": 51,
+            "referenceNumber": 363,
             "seeAlso": [
                 "http://www.sugarcrm.com/crm/SPL"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/SunPro.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "SunPro",
+            "name": "SunPro License",
+            "reference": "https://spdx.org/licenses/SunPro.html",
+            "referenceNumber": 495,
+            "seeAlso": [
+                "https://github.com/freebsd/freebsd-src/blob/main/lib/msun/src/e_acosh.c",
+                "https://github.com/freebsd/freebsd-src/blob/main/lib/msun/src/e_lgammal.c"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/SWL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "SWL",
             "name": "Scheme Widget Library (SWL) Software License Agreement",
             "reference": "https://spdx.org/licenses/SWL.html",
-            "referenceNumber": 47,
+            "referenceNumber": 180,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/SWL"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/Symlinks.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Symlinks",
+            "name": "Symlinks License",
+            "reference": "https://spdx.org/licenses/Symlinks.html",
+            "referenceNumber": 259,
+            "seeAlso": [
+                "https://www.mail-archive.com/debian-bugs-rc@lists.debian.org/msg11494.html"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/TAPR-OHL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "TAPR-OHL-1.0",
             "name": "TAPR Open Hardware License v1.0",
             "reference": "https://spdx.org/licenses/TAPR-OHL-1.0.html",
-            "referenceNumber": 465,
+            "referenceNumber": 496,
             "seeAlso": [
                 "https://www.tapr.org/OHL"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/TCL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "TCL",
             "name": "TCL/TK License",
             "reference": "https://spdx.org/licenses/TCL.html",
-            "referenceNumber": 170,
+            "referenceNumber": 125,
             "seeAlso": [
                 "http://www.tcl.tk/software/tcltk/license.html",
                 "https://fedoraproject.org/wiki/Licensing/TCL"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/TCP-wrappers.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "TCP-wrappers",
             "name": "TCP Wrappers License",
             "reference": "https://spdx.org/licenses/TCP-wrappers.html",
-            "referenceNumber": 39,
+            "referenceNumber": 84,
             "seeAlso": [
                 "http://rc.quest.com/topics/openssh/license.php#tcpwrappers"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/TermReadKey.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "TermReadKey",
+            "name": "TermReadKey License",
+            "reference": "https://spdx.org/licenses/TermReadKey.html",
+            "referenceNumber": 489,
+            "seeAlso": [
+                "https://github.com/jonathanstowe/TermReadKey/blob/master/README#L9-L10"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/TMate.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "TMate",
             "name": "TMate Open Source License",
             "reference": "https://spdx.org/licenses/TMate.html",
-            "referenceNumber": 469,
+            "referenceNumber": 36,
             "seeAlso": [
                 "http://svnkit.com/license.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/TORQUE-1.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "TORQUE-1.1",
             "name": "TORQUE v2.5+ Software License v1.1",
             "reference": "https://spdx.org/licenses/TORQUE-1.1.html",
-            "referenceNumber": 182,
+            "referenceNumber": 416,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/TORQUEv1.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/TOSL.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "TOSL",
             "name": "Trusster Open Source License",
             "reference": "https://spdx.org/licenses/TOSL.html",
-            "referenceNumber": 484,
+            "referenceNumber": 426,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/TOSL"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/TPDL.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "TPDL",
+            "name": "Time::ParseDate License",
+            "reference": "https://spdx.org/licenses/TPDL.html",
+            "referenceNumber": 432,
+            "seeAlso": [
+                "https://metacpan.org/pod/Time::ParseDate#LICENSE"
+            ]
+        },
+        {
+            "detailsUrl": "https://spdx.org/licenses/TPL-1.0.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "TPL-1.0",
+            "name": "THOR Public License 1.0",
+            "reference": "https://spdx.org/licenses/TPL-1.0.html",
+            "referenceNumber": 221,
+            "seeAlso": [
+                "https://fedoraproject.org/wiki/Licensing:ThorPublicLicense"
+            ]
+        },
+        {
+            "detailsUrl": "https://spdx.org/licenses/TTWL.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "TTWL",
+            "name": "Text-Tabs+Wrap License",
+            "reference": "https://spdx.org/licenses/TTWL.html",
+            "referenceNumber": 403,
+            "seeAlso": [
+                "https://fedoraproject.org/wiki/Licensing/TTWL",
+                "https://github.com/ap/Text-Tabs/blob/master/lib.modern/Text/Tabs.pm#L148"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/TU-Berlin-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "TU-Berlin-1.0",
             "name": "Technische Universitaet Berlin License 1.0",
             "reference": "https://spdx.org/licenses/TU-Berlin-1.0.html",
-            "referenceNumber": 103,
+            "referenceNumber": 91,
             "seeAlso": [
                 "https://github.com/swh/ladspa/blob/7bf6f3799fdba70fda297c2d8fd9f526803d9680/gsm/COPYRIGHT"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/TU-Berlin-2.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "TU-Berlin-2.0",
             "name": "Technische Universitaet Berlin License 2.0",
             "reference": "https://spdx.org/licenses/TU-Berlin-2.0.html",
-            "referenceNumber": 158,
+            "referenceNumber": 326,
             "seeAlso": [
                 "https://github.com/CorsixTH/deps/blob/fd339a9f526d1d9c9f01ccf39e438a015da50035/licences/libgsm.txt"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/UCAR.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "UCAR",
+            "name": "UCAR License",
+            "reference": "https://spdx.org/licenses/UCAR.html",
+            "referenceNumber": 454,
+            "seeAlso": [
+                "https://github.com/Unidata/UDUNITS-2/blob/master/COPYRIGHT"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/UCL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "UCL-1.0",
             "name": "Upstream Compatibility License v1.0",
             "reference": "https://spdx.org/licenses/UCL-1.0.html",
-            "referenceNumber": 19,
+            "referenceNumber": 414,
             "seeAlso": [
                 "https://opensource.org/licenses/UCL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Unicode-DFS-2015.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Unicode-DFS-2015",
             "name": "Unicode License Agreement - Data Files and Software (2015)",
             "reference": "https://spdx.org/licenses/Unicode-DFS-2015.html",
-            "referenceNumber": 77,
+            "referenceNumber": 291,
             "seeAlso": [
                 "https://web.archive.org/web/20151224134844/http://unicode.org/copyright.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Unicode-DFS-2016.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "Unicode-DFS-2016",
             "name": "Unicode License Agreement - Data Files and Software (2016)",
             "reference": "https://spdx.org/licenses/Unicode-DFS-2016.html",
-            "referenceNumber": 461,
+            "referenceNumber": 544,
             "seeAlso": [
+                "https://www.unicode.org/license.txt",
+                "http://web.archive.org/web/20160823201924/http://www.unicode.org/copyright.html#License",
                 "http://www.unicode.org/copyright.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Unicode-TOU.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Unicode-TOU",
             "name": "Unicode Terms of Use",
             "reference": "https://spdx.org/licenses/Unicode-TOU.html",
-            "referenceNumber": 197,
+            "referenceNumber": 268,
             "seeAlso": [
+                "http://web.archive.org/web/20140704074106/http://www.unicode.org/copyright.html",
                 "http://www.unicode.org/copyright.html"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/UnixCrypt.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "UnixCrypt",
+            "name": "UnixCrypt License",
+            "reference": "https://spdx.org/licenses/UnixCrypt.html",
+            "referenceNumber": 47,
+            "seeAlso": [
+                "https://foss.heptapod.net/python-libs/passlib/-/blob/branch/stable/LICENSE#L70",
+                "https://opensource.apple.com/source/JBoss/JBoss-737/jboss-all/jetty/src/main/org/mortbay/util/UnixCrypt.java.auto.html",
+                "https://archive.eclipse.org/jetty/8.0.1.v20110908/xref/org/eclipse/jetty/http/security/UnixCrypt.html"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Unlicense.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "Unlicense",
             "name": "The Unlicense",
             "reference": "https://spdx.org/licenses/Unlicense.html",
-            "referenceNumber": 5,
+            "referenceNumber": 137,
             "seeAlso": [
                 "https://unlicense.org/"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/UPL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "UPL-1.0",
             "name": "Universal Permissive License v1.0",
             "reference": "https://spdx.org/licenses/UPL-1.0.html",
-            "referenceNumber": 128,
+            "referenceNumber": 204,
             "seeAlso": [
                 "https://opensource.org/licenses/UPL"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Vim.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "Vim",
             "name": "Vim License",
             "reference": "https://spdx.org/licenses/Vim.html",
-            "referenceNumber": 155,
+            "referenceNumber": 526,
             "seeAlso": [
                 "http://vimdoc.sourceforge.net/htmldoc/uganda.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/VOSTROM.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "VOSTROM",
             "name": "VOSTROM Public License for Open Source",
             "reference": "https://spdx.org/licenses/VOSTROM.html",
-            "referenceNumber": 61,
+            "referenceNumber": 6,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/VOSTROM"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/VSL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "VSL-1.0",
             "name": "Vovida Software License v1.0",
             "reference": "https://spdx.org/licenses/VSL-1.0.html",
-            "referenceNumber": 384,
+            "referenceNumber": 153,
             "seeAlso": [
                 "https://opensource.org/licenses/VSL-1.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/W3C.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "W3C",
             "name": "W3C Software Notice and License (2002-12-31)",
             "reference": "https://spdx.org/licenses/W3C.html",
-            "referenceNumber": 339,
+            "referenceNumber": 335,
             "seeAlso": [
                 "http://www.w3.org/Consortium/Legal/2002/copyright-software-20021231.html",
                 "https://opensource.org/licenses/W3C"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/W3C-19980720.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "W3C-19980720",
             "name": "W3C Software Notice and License (1998-07-20)",
             "reference": "https://spdx.org/licenses/W3C-19980720.html",
-            "referenceNumber": 273,
+            "referenceNumber": 408,
             "seeAlso": [
                 "http://www.w3.org/Consortium/Legal/copyright-software-19980720.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/W3C-20150513.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "W3C-20150513",
             "name": "W3C Software Notice and Document License (2015-05-13)",
             "reference": "https://spdx.org/licenses/W3C-20150513.html",
-            "referenceNumber": 95,
+            "referenceNumber": 9,
             "seeAlso": [
                 "https://www.w3.org/Consortium/Legal/2015/copyright-software-and-document"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/w3m.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "w3m",
+            "name": "w3m License",
+            "reference": "https://spdx.org/licenses/w3m.html",
+            "referenceNumber": 32,
+            "seeAlso": [
+                "https://github.com/tats/w3m/blob/master/COPYING"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Watcom-1.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": false,
             "isOsiApproved": true,
             "licenseId": "Watcom-1.0",
             "name": "Sybase Open Watcom Public License 1.0",
             "reference": "https://spdx.org/licenses/Watcom-1.0.html",
-            "referenceNumber": 112,
+            "referenceNumber": 185,
             "seeAlso": [
                 "https://opensource.org/licenses/Watcom-1.0"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/Widget-Workshop.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Widget-Workshop",
+            "name": "Widget Workshop License",
+            "reference": "https://spdx.org/licenses/Widget-Workshop.html",
+            "referenceNumber": 364,
+            "seeAlso": [
+                "https://github.com/novnc/noVNC/blob/master/core/crypto/des.js#L24"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Wsuipa.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Wsuipa",
             "name": "Wsuipa License",
             "reference": "https://spdx.org/licenses/Wsuipa.html",
-            "referenceNumber": 48,
+            "referenceNumber": 440,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Wsuipa"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/WTFPL.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "WTFPL",
             "name": "Do What The F*ck You Want To Public License",
             "reference": "https://spdx.org/licenses/WTFPL.html",
-            "referenceNumber": 181,
+            "referenceNumber": 513,
             "seeAlso": [
                 "http://www.wtfpl.net/about/",
                 "http://sam.zoy.org/wtfpl/COPYING"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/wxWindows.json",
             "isDeprecatedLicenseId": true,
             "isOsiApproved": true,
             "licenseId": "wxWindows",
             "name": "wxWindows Library License",
             "reference": "https://spdx.org/licenses/wxWindows.html",
-            "referenceNumber": 124,
+            "referenceNumber": 57,
             "seeAlso": [
                 "https://opensource.org/licenses/WXwindows"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/X11.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "X11",
             "name": "X11 License",
             "reference": "https://spdx.org/licenses/X11.html",
-            "referenceNumber": 312,
+            "referenceNumber": 503,
             "seeAlso": [
                 "http://www.xfree86.org/3.3.6/COPYRIGHT2.html#3"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/X11-distribute-modifications-variant.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "X11-distribute-modifications-variant",
             "name": "X11 License Distribution Modification Variant",
             "reference": "https://spdx.org/licenses/X11-distribute-modifications-variant.html",
-            "referenceNumber": 352,
+            "referenceNumber": 288,
             "seeAlso": [
                 "https://github.com/mirror/ncurses/blob/master/COPYING"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/Xdebug-1.03.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Xdebug-1.03",
+            "name": "Xdebug License v 1.03",
+            "reference": "https://spdx.org/licenses/Xdebug-1.03.html",
+            "referenceNumber": 127,
+            "seeAlso": [
+                "https://github.com/xdebug/xdebug/blob/master/LICENSE"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Xerox.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Xerox",
             "name": "Xerox License",
             "reference": "https://spdx.org/licenses/Xerox.html",
-            "referenceNumber": 409,
+            "referenceNumber": 179,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Xerox"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/Xfig.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "Xfig",
+            "name": "Xfig License",
+            "reference": "https://spdx.org/licenses/Xfig.html",
+            "referenceNumber": 239,
+            "seeAlso": [
+                "https://github.com/Distrotech/transfig/blob/master/transfig/transfig.c",
+                "https://fedoraproject.org/wiki/Licensing:MIT#Xfig_Variant",
+                "https://sourceforge.net/p/mcj/xfig/ci/master/tree/src/Makefile.am"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/XFree86-1.1.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "XFree86-1.1",
             "name": "XFree86 License 1.1",
             "reference": "https://spdx.org/licenses/XFree86-1.1.html",
-            "referenceNumber": 27,
+            "referenceNumber": 138,
             "seeAlso": [
                 "http://www.xfree86.org/current/LICENSE4.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/xinetd.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "xinetd",
             "name": "xinetd License",
             "reference": "https://spdx.org/licenses/xinetd.html",
-            "referenceNumber": 17,
+            "referenceNumber": 312,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Xinetd_License"
             ]
         },
         {
+            "detailsUrl": "https://spdx.org/licenses/xlock.json",
+            "isDeprecatedLicenseId": false,
+            "isOsiApproved": false,
+            "licenseId": "xlock",
+            "name": "xlock License",
+            "reference": "https://spdx.org/licenses/xlock.html",
+            "referenceNumber": 343,
+            "seeAlso": [
+                "https://fossies.org/linux/tiff/contrib/ras/ras2tif.c"
+            ]
+        },
+        {
             "detailsUrl": "https://spdx.org/licenses/Xnet.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": true,
             "licenseId": "Xnet",
             "name": "X.Net License",
             "reference": "https://spdx.org/licenses/Xnet.html",
-            "referenceNumber": 439,
+            "referenceNumber": 119,
             "seeAlso": [
                 "https://opensource.org/licenses/Xnet"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/xpp.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "xpp",
             "name": "XPP License",
             "reference": "https://spdx.org/licenses/xpp.html",
-            "referenceNumber": 29,
+            "referenceNumber": 407,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/xpp"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/XSkat.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "XSkat",
             "name": "XSkat License",
             "reference": "https://spdx.org/licenses/XSkat.html",
-            "referenceNumber": 54,
+            "referenceNumber": 43,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/XSkat_License"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/YPL-1.0.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "YPL-1.0",
             "name": "Yahoo! Public License v1.0",
             "reference": "https://spdx.org/licenses/YPL-1.0.html",
-            "referenceNumber": 264,
+            "referenceNumber": 75,
             "seeAlso": [
                 "http://www.zimbra.com/license/yahoo_public_license_1.0.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/YPL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "YPL-1.1",
             "name": "Yahoo! Public License v1.1",
             "reference": "https://spdx.org/licenses/YPL-1.1.html",
-            "referenceNumber": 324,
+            "referenceNumber": 215,
             "seeAlso": [
                 "http://www.zimbra.com/license/yahoo_public_license_1.1.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Zed.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Zed",
             "name": "Zed License",
             "reference": "https://spdx.org/licenses/Zed.html",
-            "referenceNumber": 11,
+            "referenceNumber": 532,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/Zed"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Zend-2.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "Zend-2.0",
             "name": "Zend License v2.0",
             "reference": "https://spdx.org/licenses/Zend-2.0.html",
-            "referenceNumber": 32,
+            "referenceNumber": 374,
             "seeAlso": [
                 "https://web.archive.org/web/20130517195954/http://www.zend.com/license/2_00.txt"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Zimbra-1.3.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": false,
             "licenseId": "Zimbra-1.3",
             "name": "Zimbra Public License v1.3",
             "reference": "https://spdx.org/licenses/Zimbra-1.3.html",
-            "referenceNumber": 277,
+            "referenceNumber": 107,
             "seeAlso": [
                 "http://web.archive.org/web/20100302225219/http://www.zimbra.com/license/zimbra-public-license-1-3.html"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Zimbra-1.4.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "Zimbra-1.4",
             "name": "Zimbra Public License v1.4",
             "reference": "https://spdx.org/licenses/Zimbra-1.4.html",
-            "referenceNumber": 175,
+            "referenceNumber": 121,
             "seeAlso": [
                 "http://www.zimbra.com/legal/zimbra-public-license-1-4"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/Zlib.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "Zlib",
             "name": "zlib License",
             "reference": "https://spdx.org/licenses/Zlib.html",
-            "referenceNumber": 457,
+            "referenceNumber": 70,
             "seeAlso": [
                 "http://www.zlib.net/zlib_license.html",
                 "https://opensource.org/licenses/Zlib"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/zlib-acknowledgement.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "zlib-acknowledgement",
             "name": "zlib/libpng License with Acknowledgement",
             "reference": "https://spdx.org/licenses/zlib-acknowledgement.html",
-            "referenceNumber": 314,
+            "referenceNumber": 362,
             "seeAlso": [
                 "https://fedoraproject.org/wiki/Licensing/ZlibWithAcknowledgement"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/ZPL-1.1.json",
             "isDeprecatedLicenseId": false,
             "isOsiApproved": false,
             "licenseId": "ZPL-1.1",
             "name": "Zope Public License 1.1",
             "reference": "https://spdx.org/licenses/ZPL-1.1.html",
-            "referenceNumber": 397,
+            "referenceNumber": 498,
             "seeAlso": [
                 "http://old.zope.org/Resources/License/ZPL-1.1"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/ZPL-2.0.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "ZPL-2.0",
             "name": "Zope Public License 2.0",
             "reference": "https://spdx.org/licenses/ZPL-2.0.html",
-            "referenceNumber": 138,
+            "referenceNumber": 83,
             "seeAlso": [
                 "http://old.zope.org/Resources/License/ZPL-2.0",
                 "https://opensource.org/licenses/ZPL-2.0"
             ]
         },
         {
             "detailsUrl": "https://spdx.org/licenses/ZPL-2.1.json",
             "isDeprecatedLicenseId": false,
             "isFsfLibre": true,
             "isOsiApproved": true,
             "licenseId": "ZPL-2.1",
             "name": "Zope Public License 2.1",
             "reference": "https://spdx.org/licenses/ZPL-2.1.html",
-            "referenceNumber": 278,
+            "referenceNumber": 101,
             "seeAlso": [
                 "http://old.zope.org/Resources/ZPL/"
             ]
         }
     ],
-    "releaseDate": "2022-11-30"
+    "releaseDate": "2023-06-18"
 }
```

### Comparing `reuse-1.1.2/src/reuse/supported_licenses.py` & `reuse-2.0.0/src/reuse/supported_licenses.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 # SPDX-FileCopyrightText: 2022 Florian Snow <florian@familysnow.net>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """supported-licenses command handler"""
 
 import sys
+from argparse import ArgumentParser, Namespace
+from typing import IO
 
 from ._licenses import _LICENSES, _load_license_list
 from .project import Project
 
 
 # pylint: disable=unused-argument
-def add_arguments(parser) -> None:
+def add_arguments(parser: ArgumentParser) -> None:
     """Add arguments to the parser."""
 
 
 # pylint: disable=unused-argument
-def run(args, project: Project, out=sys.stdout):
+def run(args: Namespace, project: Project, out: IO[str] = sys.stdout) -> int:
     """Print the supported SPDX licenses list"""
 
     licenses = _load_license_list(_LICENSES)[1]
 
     for license_id, license_info in licenses.items():
         license_name = license_info["name"]
         license_reference = license_info["reference"]
```

### Comparing `reuse-1.1.2/src/reuse/vcs.py` & `reuse-2.0.0/src/reuse/vcs.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,89 +2,93 @@
 # SPDX-FileCopyrightText: © 2020 Liferay, Inc. <https://liferay.com>
 # SPDX-FileCopyrightText: 2020 John Mulligan <jmulligan@redhat.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """This module deals with version control systems."""
 
+from __future__ import annotations
+
 import logging
 import os
 from abc import ABC, abstractmethod
-from os import PathLike
 from pathlib import Path
-from typing import Optional, Set
+from typing import TYPE_CHECKING, Optional, Set
+
+from ._util import GIT_EXE, HG_EXE, StrPath, execute_command
 
-from ._util import GIT_EXE, HG_EXE, execute_command
+if TYPE_CHECKING:
+    from .project import Project
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class VCSStrategy(ABC):
     """Strategy pattern for version control systems."""
 
     @abstractmethod
-    def __init__(self, project: "Project"):
+    def __init__(self, project: Project):
         self.project = project
 
     @abstractmethod
-    def is_ignored(self, path: PathLike) -> bool:
+    def is_ignored(self, path: StrPath) -> bool:
         """Is *path* ignored by the VCS?"""
 
     @classmethod
     @abstractmethod
-    def in_repo(cls, directory: PathLike) -> bool:
+    def in_repo(cls, directory: StrPath) -> bool:
         """Is *directory* inside of the VCS repository?
 
         :raises NotADirectoryError: if directory is not a directory.
         """
 
     @classmethod
     @abstractmethod
-    def find_root(cls, cwd: PathLike = None) -> Optional[Path]:
+    def find_root(cls, cwd: Optional[StrPath] = None) -> Optional[Path]:
         """Try to find the root of the project from *cwd*. If none is found,
         return None.
 
         :raises NotADirectoryError: if directory is not a directory.
         """
 
 
 class VCSStrategyNone(VCSStrategy):
     """Strategy that is used when there is no VCS."""
 
-    def __init__(self, project: "Project"):
+    def __init__(self, project: Project):
         # pylint: disable=useless-super-delegation
         super().__init__(project)
 
-    def is_ignored(self, path: PathLike) -> bool:
+    def is_ignored(self, path: StrPath) -> bool:
         return False
 
     @classmethod
-    def in_repo(cls, directory: PathLike) -> bool:
+    def in_repo(cls, directory: StrPath) -> bool:
         return False
 
     @classmethod
-    def find_root(cls, cwd: PathLike = None) -> Optional[Path]:
+    def find_root(cls, cwd: Optional[StrPath] = None) -> Optional[Path]:
         return None
 
 
 class VCSStrategyGit(VCSStrategy):
     """Strategy that is used for Git."""
 
-    def __init__(self, project):
+    def __init__(self, project: Project):
         super().__init__(project)
         if not GIT_EXE:
             raise FileNotFoundError("Could not find binary for Git")
         self._all_ignored_files = self._find_all_ignored_files()
 
     def _find_all_ignored_files(self) -> Set[Path]:
         """Return a set of all files ignored by git. If a whole directory is
         ignored, don't return all files inside of it.
         """
         command = [
-            GIT_EXE,
+            str(GIT_EXE),
             "ls-files",
             "--exclude-standard",
             "--ignored",
             "--others",
             "--directory",
             # TODO: This flag is unexpected.  I reported it as a bug in Git.
             # This flag---counter-intuitively---lists untracked directories
@@ -93,114 +97,114 @@
             # Separate output with \0 instead of \n.
             "-z",
         ]
         result = execute_command(command, _LOGGER, cwd=self.project.root)
         all_files = result.stdout.decode("utf-8").split("\0")
         return {Path(file_) for file_ in all_files}
 
-    def is_ignored(self, path: PathLike) -> bool:
+    def is_ignored(self, path: StrPath) -> bool:
         path = self.project.relative_from_root(path)
         return path in self._all_ignored_files
 
     @classmethod
-    def in_repo(cls, directory: PathLike) -> bool:
+    def in_repo(cls, directory: StrPath) -> bool:
         if directory is None:
             directory = Path.cwd()
 
         if not Path(directory).is_dir():
             raise NotADirectoryError()
 
-        command = [GIT_EXE, "status"]
+        command = [str(GIT_EXE), "status"]
         result = execute_command(command, _LOGGER, cwd=directory)
 
         return not result.returncode
 
     @classmethod
-    def find_root(cls, cwd: PathLike = None) -> Optional[Path]:
+    def find_root(cls, cwd: Optional[StrPath] = None) -> Optional[Path]:
         if cwd is None:
             cwd = Path.cwd()
 
         if not Path(cwd).is_dir():
             raise NotADirectoryError()
 
-        command = [GIT_EXE, "rev-parse", "--show-toplevel"]
+        command = [str(GIT_EXE), "rev-parse", "--show-toplevel"]
         result = execute_command(command, _LOGGER, cwd=cwd)
 
         if not result.returncode:
             path = result.stdout.decode("utf-8")[:-1]
             return Path(os.path.relpath(path, cwd))
 
         return None
 
 
 class VCSStrategyHg(VCSStrategy):
     """Strategy that is used for Mercurial."""
 
-    def __init__(self, project: "Project"):
+    def __init__(self, project: Project):
         super().__init__(project)
         if not HG_EXE:
             raise FileNotFoundError("Could not find binary for Mercurial")
         self._all_ignored_files = self._find_all_ignored_files()
 
     def _find_all_ignored_files(self) -> Set[Path]:
         """Return a set of all files ignored by mercurial. If a whole directory
         is ignored, don't return all files inside of it.
         """
         command = [
-            HG_EXE,
+            str(HG_EXE),
             "status",
             "--ignored",
             # terse is marked 'experimental' in the hg help but is documented
             # in the man page. It collapses the output of a dir containing only
             # ignored files to the ignored name like the git command does.
             # TODO: Re-enable this flag in the future.
             # "--terse=i",
             "--no-status",
             "--print0",
         ]
         result = execute_command(command, _LOGGER, cwd=self.project.root)
         all_files = result.stdout.decode("utf-8").split("\0")
         return {Path(file_) for file_ in all_files}
 
-    def is_ignored(self, path: PathLike) -> bool:
+    def is_ignored(self, path: StrPath) -> bool:
         path = self.project.relative_from_root(path)
         return path in self._all_ignored_files
 
     @classmethod
-    def in_repo(cls, directory: PathLike) -> bool:
+    def in_repo(cls, directory: StrPath) -> bool:
         if directory is None:
             directory = Path.cwd()
 
         if not Path(directory).is_dir():
             raise NotADirectoryError()
 
-        command = [HG_EXE, "root"]
+        command = [str(HG_EXE), "root"]
         result = execute_command(command, _LOGGER, cwd=directory)
 
         return not result.returncode
 
     @classmethod
-    def find_root(cls, cwd: PathLike = None) -> Optional[Path]:
+    def find_root(cls, cwd: Optional[StrPath] = None) -> Optional[Path]:
         if cwd is None:
             cwd = Path.cwd()
 
         if not Path(cwd).is_dir():
             raise NotADirectoryError()
 
-        command = [HG_EXE, "root"]
+        command = [str(HG_EXE), "root"]
         result = execute_command(command, _LOGGER, cwd=cwd)
 
         if not result.returncode:
             path = result.stdout.decode("utf-8")[:-1]
             return Path(os.path.relpath(path, cwd))
 
         return None
 
 
-def find_root(cwd: PathLike = None) -> Optional[Path]:
+def find_root(cwd: Optional[StrPath] = None) -> Optional[Path]:
     """Try to find the root of the project from *cwd*. If none is found,
     return None.
 
     :raises NotADirectoryError: if directory is not a directory.
     """
     if GIT_EXE:
         root = VCSStrategyGit.find_root(cwd=cwd)
```

### Comparing `reuse-1.1.2/tests/conftest.py` & `reuse-2.0.0/tests/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import os
 import shutil
 import subprocess
 import sys
 from inspect import cleandoc
 from io import StringIO
 from pathlib import Path
-from typing import Optional
+from typing import Generator
 from unittest.mock import create_autospec
 
 import pytest
 from debian.copyright import Copyright
 from jinja2 import Environment
 
 os.environ["LC_ALL"] = "C"
@@ -39,55 +39,67 @@
     from reuse._util import GIT_EXE, HG_EXE, setup_logging
 
 CWD = Path.cwd()
 
 TESTS_DIRECTORY = Path(__file__).parent.resolve()
 RESOURCES_DIRECTORY = TESTS_DIRECTORY / "resources"
 
+
 # REUSE-IgnoreStart
 
 
-def pytest_configure():
+def pytest_addoption(parser):
+    """Allows specification of additional commandline options to parse"""
+    parser.addoption("--loglevel", action="store", default="DEBUG")
+
+
+def pytest_configure(config):
     """Called after command line options have been parsed and all plugins and
     initial conftest files been loaded.
     """
-    setup_logging(level=logging.DEBUG)
+    loglevel = config.getoption("loglevel")
+    setup_logging(level=logging.getLevelName(loglevel))
 
 
 def pytest_runtest_setup(item):
     """Called before running a test."""
     # pylint: disable=unused-argument
     # Make sure to restore CWD
     os.chdir(CWD)
 
 
 @pytest.fixture()
 def git_exe() -> str:
     """Run the test with git."""
     if not GIT_EXE:
         pytest.skip("cannot run this test without git")
-    yield GIT_EXE
+    return str(GIT_EXE)
 
 
 @pytest.fixture()
 def hg_exe() -> str:
     """Run the test with mercurial (hg)."""
     if not HG_EXE:
         pytest.skip("cannot run this test without mercurial")
-    yield HG_EXE
+    return str(HG_EXE)
 
 
 @pytest.fixture(params=[True, False])
-def multiprocessing(request, monkeypatch) -> bool:
+def multiprocessing(request, monkeypatch) -> Generator[bool, None, None]:
     """Run the test with or without multiprocessing."""
     if not request.param:
         monkeypatch.delattr(mp, "Pool")
     yield request.param
 
 
+@pytest.fixture(params=[True, False])
+def add_license_concluded(request) -> Generator[bool, None, None]:
+    yield request
+
+
 @pytest.fixture()
 def empty_directory(tmpdir_factory) -> Path:
     """Create a temporary empty directory."""
     directory = Path(str(tmpdir_factory.mktemp("empty_directory")))
 
     os.chdir(str(directory))
     return directory
@@ -113,14 +125,21 @@
         encoding="utf-8",
     )
     (directory / "src/custom.py").write_text(
         "SPDX-FileCopyrightText: 2017 Jane Doe\n"
         "SPDX-License-Identifier: LicenseRef-custom",
         encoding="utf-8",
     )
+    (directory / "src/multiple_licenses.rs").write_text(
+        "SPDX-FileCopyrightText: 2022 Jane Doe\n"
+        "SPDX-License-Identifier: GPL-3.0-or-later\n"
+        "SPDX-License-Identifier: Apache-2.0 OR CC0-1.0"
+        " WITH Autoconf-exception-3.0\n",
+        encoding="utf-8",
+    )
 
     os.chdir(directory)
     return directory
 
 
 def _repo_contents(
     fake_repository, ignore_filename=".gitignore", ignore_prefix=""
@@ -146,24 +165,26 @@
 
     build_dir = fake_repository / "build"
     build_dir.mkdir()
     (build_dir / "hello.py").write_text("foo")
 
 
 @pytest.fixture()
-def git_repository(fake_repository: Path, git_exe: Optional[str]) -> Path:
+def git_repository(fake_repository: Path, git_exe: str) -> Path:
     """Create a git repository with ignored files."""
     os.chdir(fake_repository)
     _repo_contents(fake_repository)
 
+    # TODO: To speed this up, maybe directly write to '.gitconfig' instead.
     subprocess.run([git_exe, "init", str(fake_repository)], check=True)
     subprocess.run([git_exe, "config", "user.name", "Example"], check=True)
     subprocess.run(
         [git_exe, "config", "user.email", "example@example.com"], check=True
     )
+    subprocess.run([git_exe, "config", "commit.gpgSign", "false"], check=True)
 
     subprocess.run([git_exe, "add", str(fake_repository)], check=True)
     subprocess.run(
         [
             git_exe,
             "commit",
             "-m",
@@ -172,15 +193,15 @@
         check=True,
     )
 
     return fake_repository
 
 
 @pytest.fixture()
-def hg_repository(fake_repository: Path, hg_exe: Optional[str]) -> Path:
+def hg_repository(fake_repository: Path, hg_exe: str) -> Path:
     """Create a mercurial repository with ignored files."""
     os.chdir(fake_repository)
     _repo_contents(
         fake_repository,
         ignore_filename=".hgignore",
         ignore_prefix="syntax:glob",
     )
@@ -200,15 +221,15 @@
     )
 
     return fake_repository
 
 
 @pytest.fixture()
 def submodule_repository(
-    git_repository: Path, git_exe: Optional[str], tmpdir_factory
+    git_repository: Path, git_exe: str, tmpdir_factory
 ) -> Path:
     """Create a git repository that contains a submodule."""
     header = cleandoc(
         """
             SPDX-FileCopyrightText: 2019 Jane Doe
 
             SPDX-License-Identifier: CC0-1.0
@@ -363,8 +384,17 @@
 def mock_date_today(monkeypatch):
     """Mock away datetime.date.today to always return 2018."""
     date = create_autospec(datetime.date)
     date.today.return_value = datetime.date(2018, 1, 1)
     monkeypatch.setattr(datetime, "date", date)
 
 
+@pytest.fixture(
+    params=[[], ["John Doe"], ["John Doe", "Alice Doe"]],
+    ids=["None", "John", "John and Alice"],
+)
+def contributors(request):
+    """Provide contributors for SPDX-FileContributor field generation"""
+    yield request.param
+
+
 # REUSE-IgnoreEnd
```

### Comparing `reuse-1.1.2/tests/resources/fsfe.png` & `reuse-2.0.0/tests/resources/fsfe.png`

 * *Files identical despite different names*

### Comparing `reuse-1.1.2/tests/test_comment.py` & `reuse-2.0.0/tests/test_comment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # SPDX-FileCopyrightText: 2019 Free Software Foundation Europe e.V. <https://fsfe.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
-"""All tests for reuse._comment"""
+"""All tests for reuse.comment"""
 
 # pylint: disable=protected-access,invalid-name,redefined-outer-name
 
 from inspect import cleandoc
 from textwrap import dedent
 
 import pytest
 
-from reuse._comment import (
+from reuse.comment import (
     CCommentStyle,
     CommentCreateError,
     CommentParseError,
     CommentStyle,
     HtmlCommentStyle,
     PythonCommentStyle,
     _all_style_classes,
```

### Comparing `reuse-1.1.2/tests/test_download.py` & `reuse-2.0.0/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `reuse-1.1.2/tests/test_header.py` & `reuse-2.0.0/tests/test_header.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,109 +1,112 @@
 # SPDX-FileCopyrightText: 2019 Free Software Foundation Europe e.V. <https://fsfe.org>
 # SPDX-FileCopyrightText: 2022 Florian Snow <florian@familysnow.net>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """All tests for reuse.header"""
 
-# pylint: disable=implicit-str-concat-in-sequence
-
 from inspect import cleandoc
 
 import pytest
 
-from reuse import SpdxInfo
-from reuse._comment import CCommentStyle, CommentCreateError
+from reuse import ReuseInfo
+from reuse.comment import CCommentStyle, CommentCreateError
 from reuse.header import (
-    MissingSpdxInfo,
+    MissingReuseInfo,
     add_new_header,
     create_header,
     find_and_replace_header,
 )
 
 # REUSE-IgnoreStart
 
 
 def test_create_header_simple():
     """Create a super simple header."""
-    spdx_info = SpdxInfo(
-        {"GPL-3.0-or-later"}, {"SPDX-FileCopyrightText: Jane Doe"}
+    info = ReuseInfo({"GPL-3.0-or-later"}, {"SPDX-FileCopyrightText: Jane Doe"})
+    expected = cleandoc(
+        """
+        # SPDX-FileCopyrightText: Jane Doe
+        #
+        # SPDX-License-Identifier: GPL-3.0-or-later
+        """
+    )
+
+    assert create_header(info).strip() == expected
+
+
+def test_create_header_simple_with_contributor():
+    """Create a super simple header."""
+    info = ReuseInfo(
+        {"GPL-3.0-or-later"}, {"SPDX-FileCopyrightText: Jane Doe"}, {"John Doe"}
     )
     expected = cleandoc(
         """
         # SPDX-FileCopyrightText: Jane Doe
+        # SPDX-FileContributor: John Doe
         #
         # SPDX-License-Identifier: GPL-3.0-or-later
         """
     )
 
-    assert create_header(spdx_info).strip() == expected
+    assert create_header(info).strip() == expected
 
 
 def test_create_header_template_simple(template_simple):
     """Create a header with a simple template."""
-    spdx_info = SpdxInfo(
-        {"GPL-3.0-or-later"}, {"SPDX-FileCopyrightText: Jane Doe"}
-    )
+    info = ReuseInfo({"GPL-3.0-or-later"}, {"SPDX-FileCopyrightText: Jane Doe"})
     expected = cleandoc(
         """
         # Hello, world!
         #
         # SPDX-FileCopyrightText: Jane Doe
         #
         # SPDX-License-Identifier: GPL-3.0-or-later
         """
     )
 
-    assert (
-        create_header(spdx_info, template=template_simple).strip() == expected
-    )
+    assert create_header(info, template=template_simple).strip() == expected
 
 
 def test_create_header_template_no_spdx(template_no_spdx):
-    """Create a header with a template that does not have all SPDX info."""
-    spdx_info = SpdxInfo(
-        {"GPL-3.0-or-later"}, {"SPDX-FileCopyrightText: Jane Doe"}
-    )
+    """Create a header with a template that does not have all REUSE info."""
+    info = ReuseInfo({"GPL-3.0-or-later"}, {"SPDX-FileCopyrightText: Jane Doe"})
 
-    with pytest.raises(MissingSpdxInfo):
-        create_header(spdx_info, template=template_no_spdx)
+    with pytest.raises(MissingReuseInfo):
+        create_header(info, template=template_no_spdx)
 
 
 def test_create_header_template_commented(template_commented):
     """Create a header with an already-commented template."""
-    spdx_info = SpdxInfo(
-        {"GPL-3.0-or-later"}, {"SPDX-FileCopyrightText: Jane Doe"}
-    )
+    info = ReuseInfo({"GPL-3.0-or-later"}, {"SPDX-FileCopyrightText: Jane Doe"})
     expected = cleandoc(
         """
         # Hello, world!
         #
         # SPDX-FileCopyrightText: Jane Doe
         #
         # SPDX-License-Identifier: GPL-3.0-or-later
         """
     )
 
     assert (
         create_header(
-            spdx_info,
+            info,
             template=template_commented,
             template_is_commented=True,
             style=CCommentStyle,
         ).strip()
         == expected
     )
 
 
 def test_create_header_already_contains_spdx():
-    """Create a new header from a header that already contains SPDX info."""
-    spdx_info = SpdxInfo(
-        {"GPL-3.0-or-later"}, {"SPDX-FileCopyrightText: Jane Doe"}
-    )
+    """Create a new header from a header that already contains REUSE info."""
+    info = ReuseInfo({"GPL-3.0-or-later"}, {"SPDX-FileCopyrightText: Jane Doe"})
     existing = cleandoc(
         """
         # SPDX-FileCopyrightText: John Doe
         #
         # SPDX-License-Identifier: MIT
         """
     )
@@ -113,56 +116,54 @@
         # SPDX-FileCopyrightText: John Doe
         #
         # SPDX-License-Identifier: GPL-3.0-or-later
         # SPDX-License-Identifier: MIT
         """
     )
 
-    assert create_header(spdx_info, header=existing).strip() == expected
+    assert create_header(info, header=existing).strip() == expected
 
 
 def test_create_header_existing_is_wrong():
     """If the existing header contains errors, raise a CommentCreateError."""
-    spdx_info = SpdxInfo(
-        {"GPL-3.0-or-later"}, {"SPDX-FileCopyrightText: Jane Doe"}
-    )
+    info = ReuseInfo({"GPL-3.0-or-later"}, {"SPDX-FileCopyrightText: Jane Doe"})
     existing = cleandoc(
         """
         # SPDX-FileCopyrightText: John Doe
         #
         # SPDX-License-Identifier: MIT AND OR 0BSD
         """
     )
 
     with pytest.raises(CommentCreateError):
-        create_header(spdx_info, header=existing)
+        create_header(info, header=existing)
 
 
 def test_create_header_old_syntax():
     """Old copyright syntax is preserved when creating a new header."""
-    spdx_info = SpdxInfo({"GPL-3.0-or-later"}, set())
+    info = ReuseInfo({"GPL-3.0-or-later"})
     existing = cleandoc(
         """
         # Copyright John Doe
         """
     )
     expected = cleandoc(
         """
         # Copyright John Doe
         #
         # SPDX-License-Identifier: GPL-3.0-or-later
         """
     )
 
-    assert create_header(spdx_info, header=existing).strip() == expected
+    assert create_header(info, header=existing).strip() == expected
 
 
 def test_create_header_remove_fluff():
-    """Any stuff that isn't SPDX info is removed when using create_header."""
-    spdx_info = SpdxInfo({"GPL-3.0-or-later"}, set())
+    """Any stuff that isn't REUSE info is removed when using create_header."""
+    info = ReuseInfo({"GPL-3.0-or-later"})
     existing = cleandoc(
         """
         # SPDX-FileCopyrightText: John Doe
         #
         # Hello, world!
 
         pass
@@ -172,24 +173,22 @@
         """
         # SPDX-FileCopyrightText: John Doe
         #
         # SPDX-License-Identifier: GPL-3.0-or-later
         """
     )
 
-    assert create_header(spdx_info, header=existing).strip() == expected
+    assert create_header(info, header=existing).strip() == expected
 
 
 def test_add_new_header_simple():
     """Given text that already contains a header, create a new one, and preserve
     the old one.
     """
-    spdx_info = SpdxInfo(
-        {"GPL-3.0-or-later"}, {"SPDX-FileCopyrightText: Jane Doe"}
-    )
+    info = ReuseInfo({"GPL-3.0-or-later"}, {"SPDX-FileCopyrightText: Jane Doe"})
     text = cleandoc(
         """
         # SPDX-FileCopyrightText: John Doe
         #
         # SPDX-License-Identifier: MIT
 
         pass
@@ -204,63 +203,59 @@
         # SPDX-FileCopyrightText: John Doe
         #
         # SPDX-License-Identifier: MIT
 
         pass
         """
     )
-    assert add_new_header(text, spdx_info) == expected
+    assert add_new_header(text, info) == expected
 
 
 def test_find_and_replace_no_header():
     """Given text without header, add a header."""
-    spdx_info = SpdxInfo(
-        {"GPL-3.0-or-later"}, {"SPDX-FileCopyrightText: Jane Doe"}
-    )
+    info = ReuseInfo({"GPL-3.0-or-later"}, {"SPDX-FileCopyrightText: Jane Doe"})
     text = "pass"
     expected = cleandoc(
         """
         # SPDX-FileCopyrightText: Jane Doe
         #
         # SPDX-License-Identifier: GPL-3.0-or-later
 
         pass
         """
     )
 
     assert (
-        find_and_replace_header(text, spdx_info)
-        == add_new_header(text, spdx_info)
+        find_and_replace_header(text, info)
+        == add_new_header(text, info)
         == expected
     )
 
 
 def test_find_and_replace_verbatim():
     """Replace a header with itself."""
-    spdx_info = SpdxInfo(set(), set())
+    info = ReuseInfo()
     text = cleandoc(
         """
         # SPDX-FileCopyrightText: Jane Doe
         #
         # SPDX-License-Identifier: GPL-3.0-or-later
 
         pass
         """
     )
 
-    assert find_and_replace_header(text, spdx_info) == text
+    assert find_and_replace_header(text, info) == text
 
 
 def test_find_and_replace_newline_before_header():
     """In a scenario where the header is preceded by whitespace, remove the
     preceding whitespace.
     """
-    spdx_info = SpdxInfo(
-        {"GPL-3.0-or-later"}, {"SPDX-FileCopyrightText: John Doe"}
-    )
+    info = ReuseInfo({"GPL-3.0-or-later"}, {"SPDX-FileCopyrightText: John Doe"})
     text = cleandoc(
         """
         # SPDX-FileCopyrightText: Jane Doe
 
         pass
         """
     )
@@ -272,22 +267,20 @@
         #
         # SPDX-License-Identifier: GPL-3.0-or-later
 
         pass
         """
     )
 
-    assert find_and_replace_header(text, spdx_info) == expected
+    assert find_and_replace_header(text, info) == expected
 
 
 def test_find_and_replace_preserve_preceding():
     """When the SPDX header is in the middle of the file, keep it there."""
-    spdx_info = SpdxInfo(
-        {"GPL-3.0-or-later"}, {"SPDX-FileCopyrightText: John Doe"}
-    )
+    info = ReuseInfo({"GPL-3.0-or-later"}, {"SPDX-FileCopyrightText: John Doe"})
     text = cleandoc(
         """
         # Hello, world!
 
         def foo(bar):
             return bar
 
@@ -308,24 +301,22 @@
         #
         # SPDX-License-Identifier: GPL-3.0-or-later
 
         pass
         """
     )
 
-    assert find_and_replace_header(text, spdx_info) == expected
+    assert find_and_replace_header(text, info) == expected
 
 
 def test_find_and_replace_keep_shebang():
     """When encountering a shebang, keep it and put the REUSE header beneath
     it.
     """
-    spdx_info = SpdxInfo(
-        {"GPL-3.0-or-later"}, {"SPDX-FileCopyrightText: John Doe"}
-    )
+    info = ReuseInfo({"GPL-3.0-or-later"}, {"SPDX-FileCopyrightText: John Doe"})
     text = cleandoc(
         """
         #!/usr/bin/env python3
 
         # SPDX-FileCopyrightText: Jane Doe
 
         pass
@@ -340,22 +331,22 @@
         #
         # SPDX-License-Identifier: GPL-3.0-or-later
 
         pass
         """
     )
 
-    assert find_and_replace_header(text, spdx_info) == expected
+    assert find_and_replace_header(text, info) == expected
 
 
 def test_find_and_replace_separate_shebang():
     """When the shebang is part of the same comment as the SPDX comment,
     separate the two.
     """
-    spdx_info = SpdxInfo({"GPL-3.0-or-later"}, set())
+    info = ReuseInfo({"GPL-3.0-or-later"})
     text = cleandoc(
         """
         #!/usr/bin/env python3
         #!nix-shell -p python3
         # SPDX-FileCopyrightText: Jane Doe
 
         pass
@@ -370,20 +361,20 @@
         #
         # SPDX-License-Identifier: GPL-3.0-or-later
 
         pass
         """
     )
 
-    assert find_and_replace_header(text, spdx_info) == expected
+    assert find_and_replace_header(text, info) == expected
 
 
 def test_find_and_replace_only_shebang():
     """When the file only contains a shebang, keep it at the top of the file."""
-    spdx_info = SpdxInfo({"GPL-3.0-or-later"}, set())
+    info = ReuseInfo({"GPL-3.0-or-later"})
     text = cleandoc(
         """
         #!/usr/bin/env python3
 
         # Hello, world!
 
         pass
@@ -397,24 +388,22 @@
 
         # Hello, world!
 
         pass
         """
     )
 
-    assert find_and_replace_header(text, spdx_info) == expected
+    assert find_and_replace_header(text, info) == expected
 
 
 def test_find_and_replace_keep_old_comment():
     """When encountering a comment that does not contain copyright and
     licensing information, preserve it below the REUSE header.
     """
-    spdx_info = SpdxInfo(
-        {"GPL-3.0-or-later"}, {"SPDX-FileCopyrightText: Jane Doe"}
-    )
+    info = ReuseInfo({"GPL-3.0-or-later"}, {"SPDX-FileCopyrightText: Jane Doe"})
     text = cleandoc(
         """
         # Hello, world!
 
         pass
         """
     )
@@ -426,31 +415,31 @@
 
         # Hello, world!
 
         pass
         """
     )
 
-    assert find_and_replace_header(text, spdx_info) == expected
+    assert find_and_replace_header(text, info) == expected
 
 
 def test_find_and_replace_preserve_newline():
     """If the file content ends with a newline, don't remove it."""
 
-    spdx_info = SpdxInfo(set(), set())
+    info = ReuseInfo()
     text = (
         cleandoc(
             """
             # SPDX-FileCopyrightText: Jane Doe
             #
             # SPDX-License-Identifier: GPL-3.0-or-later
 
             pass
             """
         )
         + "\n"
     )
 
-    assert find_and_replace_header(text, spdx_info) == text
+    assert find_and_replace_header(text, info) == text
 
 
 # REUSE-IgnoreEnd
```

### Comparing `reuse-1.1.2/tests/test_main.py` & `reuse-2.0.0/tests/test_main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,54 @@
 # SPDX-FileCopyrightText: 2019 Free Software Foundation Europe e.V. <https://fsfe.org>
 # SPDX-FileCopyrightText: 2019 Stefan Bakker <s.bakker777@gmail.com>
 # SPDX-FileCopyrightText: © 2020 Liferay, Inc. <https://liferay.com>
 # SPDX-FileCopyrightText: 2022 Florian Snow <florian@familysnow.net>
+# SPDX-FileCopyrightText: 2022 Pietro Albini <pietro.albini@ferrous-systems.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Tests for reuse._main: lint, spdx, download"""
 
 # pylint: disable=redefined-outer-name,unused-argument
 
 import errno
+import json
 import os
 import re
 from inspect import cleandoc
 from pathlib import Path
-from typing import Optional
+from typing import Generator, Optional
 from unittest.mock import create_autospec
 from urllib.error import URLError
 
 import pytest
 
 from reuse import download
 from reuse._main import main
 from reuse._util import GIT_EXE, HG_EXE
+from reuse.report import LINT_VERSION
 
 # REUSE-IgnoreStart
 
 
 @pytest.fixture(params=[True, False])
-def optional_git_exe(request, monkeypatch) -> Optional[str]:
+def optional_git_exe(
+    request, monkeypatch
+) -> Generator[Optional[str], None, None]:
     """Run the test with or without git."""
     exe = GIT_EXE if request.param else ""
     monkeypatch.setattr("reuse.project.GIT_EXE", exe)
     monkeypatch.setattr("reuse._util.GIT_EXE", exe)
     yield exe
 
 
 @pytest.fixture(params=[True, False])
-def optional_hg_exe(request, monkeypatch) -> Optional[str]:
+def optional_hg_exe(
+    request, monkeypatch
+) -> Generator[Optional[str], None, None]:
     """Run the test with or without mercurial."""
     exe = HG_EXE if request.param else ""
     monkeypatch.setattr("reuse.project.HG_EXE", exe)
     monkeypatch.setattr("reuse._util.HG_EXE", exe)
     yield exe
 
 
@@ -210,14 +217,37 @@
     (fake_repository / "foo.py").write_text("foo")
     result = main(["lint", "--quiet"], out=stringio)
 
     assert result > 0
     assert stringio.getvalue() == ""
 
 
+def test_lint_json(fake_repository, stringio):
+    """Run a failed lint."""
+    result = main(["lint", "--json"], out=stringio)
+    output = json.loads(stringio.getvalue())
+
+    assert result == 0
+    assert output["lint_version"] == LINT_VERSION
+    assert len(output["files"]) == 8
+
+
+def test_lint_json_fail(fake_repository, stringio):
+    """Run a failed lint."""
+    (fake_repository / "foo.py").write_text("foo")
+    result = main(["lint", "--json"], out=stringio)
+    output = json.loads(stringio.getvalue())
+
+    assert result > 0
+    assert output["lint_version"] == LINT_VERSION
+    assert len(output["non_compliant"]["missing_licensing_info"]) == 1
+    assert len(output["non_compliant"]["missing_copyright_info"]) == 1
+    assert len(output["files"]) == 9
+
+
 def test_lint_no_file_extension(fake_repository, stringio):
     """If a license has no file extension, the lint fails."""
     (fake_repository / "LICENSES/CC0-1.0.txt").rename(
         fake_repository / "LICENSES/CC0-1.0"
     )
     result = main(["lint"], out=stringio)
 
@@ -273,18 +303,74 @@
     assert ":-)" in stringio.getvalue()
 
 
 def test_spdx(fake_repository, stringio):
     """Compile to an SPDX document."""
     os.chdir(str(fake_repository))
     result = main(["spdx"], out=stringio)
+    output = stringio.getvalue()
+
+    # Ensure no LicenseConcluded is included without the flag
+    assert "\nLicenseConcluded: NOASSERTION\n" in output
+    assert "\nLicenseConcluded: GPL-3.0-or-later\n" not in output
+    assert "\nCreator: Person: Anonymous ()\n" in output
+    assert "\nCreator: Organization: Anonymous ()\n" in output
 
     # TODO: This test is rubbish.
     assert result == 0
-    assert stringio.getvalue()
+    assert output
+
+
+def test_spdx_creator_info(fake_repository, stringio):
+    """Ensure the --creator-* flags are properly formatted"""
+    os.chdir(str(fake_repository))
+    result = main(
+        [
+            "spdx",
+            "--creator-person=Jane Doe (jane.doe@example.org)",
+            "--creator-organization=FSFE",
+        ],
+        out=stringio,
+    )
+    output = stringio.getvalue()
+
+    assert result == 0
+    assert "\nCreator: Person: Jane Doe (jane.doe@example.org)\n" in output
+    assert "\nCreator: Organization: FSFE ()\n" in output
+
+
+def test_spdx_add_license_concluded(fake_repository, stringio):
+    """Compile to an SPDX document with the LicenseConcluded field."""
+    os.chdir(str(fake_repository))
+    result = main(
+        [
+            "spdx",
+            "--add-license-concluded",
+            "--creator-person=Jane Doe",
+            "--creator-organization=FSFE",
+        ],
+        out=stringio,
+    )
+    output = stringio.getvalue()
+
+    # Ensure no LicenseConcluded is included without the flag
+    assert result == 0
+    assert "\nLicenseConcluded: NOASSERTION\n" not in output
+    assert "\nLicenseConcluded: GPL-3.0-or-later\n" in output
+    assert "\nCreator: Person: Jane Doe ()\n" in output
+    assert "\nCreator: Organization: FSFE ()\n" in output
+
+
+def test_spdx_add_license_concluded_without_creator_info(
+    fake_repository, stringio
+):
+    """Adding LicenseConcluded should require creator information"""
+    os.chdir(str(fake_repository))
+    with pytest.raises(SystemExit):
+        main(["spdx", "--add-license-concluded"], out=stringio)
 
 
 def test_spdx_no_multiprocessing(fake_repository, stringio, multiprocessing):
     """--no-multiprocessing works."""
     os.chdir(str(fake_repository))
     result = main(["--no-multiprocessing", "spdx"], out=stringio)
```

### Comparing `reuse-1.1.2/tests/test_main_annotate.py` & `reuse-2.0.0/tests/test_main_annotate.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 # SPDX-FileCopyrightText: © 2020 Liferay, Inc. <https://liferay.com>
 # SPDX-FileCopyrightText: 2022 Florian Snow <florian@familysnow.net>
 # SPDX-FileCopyrightText: 2022 Carmen Bianca Bakker <carmenbianca@fsfe.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Tests for reuse._main: annotate"""
-
-# pylint: disable=too-many-lines,unused-argument
-
+import logging
 import stat
 from inspect import cleandoc
 
 import pytest
 
 from reuse._main import main
 
+# pylint: disable=too-many-lines,unused-argument
+
+
 # REUSE-IgnoreStart
 
+
 # TODO: Replace this test with a monkeypatched test
 def test_annotate_simple(fake_repository, stringio, mock_date_today):
     """Add a header to a file that does not have one."""
     simple_file = fake_repository / "foo.py"
     simple_file.write_text("pass")
     expected = cleandoc(
         """
@@ -260,14 +262,83 @@
         out=stringio,
     )
 
     assert result == 0
     assert simple_file.read_text() == expected
 
 
+def test_annotate_contributors_only(
+    fake_repository, stringio, mock_date_today, contributors
+):
+    """Add a header with only contributor information."""
+
+    if not contributors:
+        pytest.skip("No contributors to add")
+
+    simple_file = fake_repository / "foo.py"
+    simple_file.write_text("pass")
+    content = []
+
+    for contributor in sorted(contributors):
+        content.append(f"# SPDX-FileContributor: {contributor}")
+
+    content += ["", "pass"]
+    expected = cleandoc("\n".join(content))
+
+    args = [
+        "annotate",
+    ]
+    for contributor in contributors:
+        args += ["--contributor", contributor]
+    args += ["foo.py"]
+
+    result = main(
+        args,
+        out=stringio,
+    )
+
+    assert result == 0
+    assert simple_file.read_text() == expected
+
+
+def test_annotate_contributors(
+    fake_repository, stringio, mock_date_today, contributors
+):
+    """Add a header with contributor information."""
+    simple_file = fake_repository / "foo.py"
+    simple_file.write_text("pass")
+    content = ["# SPDX-FileCopyrightText: 2018 Jane Doe"]
+
+    if contributors:
+        for contributor in sorted(contributors):
+            content.append(f"# SPDX-FileContributor: {contributor}")
+
+    content += ["#", "# SPDX-License-Identifier: GPL-3.0-or-later", "", "pass"]
+    expected = cleandoc("\n".join(content))
+
+    args = [
+        "annotate",
+        "--license",
+        "GPL-3.0-or-later",
+        "--copyright",
+        "Jane Doe",
+    ]
+    for contributor in contributors:
+        args += ["--contributor", contributor]
+    args += ["foo.py"]
+
+    result = main(
+        args,
+        out=stringio,
+    )
+
+    assert result == 0
+    assert simple_file.read_text() == expected
+
+
 def test_annotate_specify_style(fake_repository, stringio, mock_date_today):
     """Add a header to a file that does not have one, using a custom style."""
     simple_file = fake_repository / "foo.py"
     simple_file.write_text("pass")
     expected = cleandoc(
         """
         // SPDX-FileCopyrightText: 2018 Jane Doe
@@ -416,15 +487,21 @@
             "--skip-unrecognised",
             "foo.foo",
         ],
         out=stringio,
     )
 
     assert result == 0
-    assert "no effect" in caplog.text
+    loglevel = logging.getLogger("reuse").level
+    if loglevel > logging.WARNING:
+        pytest.skip(
+            "Test needs LogLevel <= WARNING (e.g. WARNING, INFO, DEBUG)."
+        )
+    else:
+        assert "no effect" in caplog.text
 
 
 def test_annotate_no_copyright_or_license(fake_repository):
     """Add a header, but supply no copyright or license."""
     simple_file = fake_repository / "foo.py"
     simple_file.write_text("pass")
 
@@ -511,15 +588,15 @@
         )
         assert simple_file.read_text() == expected
 
 
 def test_annotate_template_no_spdx(
     fake_repository, stringio, template_no_spdx_source
 ):
-    """Add a header with a template that lacks SPDX info."""
+    """Add a header with a template that lacks REUSE info."""
     simple_file = fake_repository / "foo.py"
     simple_file.write_text("pass")
     template_file = fake_repository / ".reuse/templates/mytemplate.jinja2"
     template_file.parent.mkdir(parents=True, exist_ok=True)
     template_file.write_text(template_no_spdx_source)
 
     result = main(
@@ -600,15 +677,14 @@
             ]
         )
 
 
 def test_annotate_template_without_extension(
     fake_repository, stringio, mock_date_today, template_simple_source
 ):
-
     """Find the correct header even when not using an extension."""
     simple_file = fake_repository / "foo.py"
     simple_file.write_text("pass")
     template_file = fake_repository / ".reuse/templates/mytemplate.jinja2"
     template_file.parent.mkdir(parents=True, exist_ok=True)
     template_file.write_text(template_simple_source)
     expected = cleandoc(
@@ -1152,15 +1228,15 @@
     with open(simple_file, newline="", encoding="utf-8") as fp:
         contents = fp.read()
 
     assert contents == expected
 
 
 def test_annotate_skip_existing(fake_repository, stringio, mock_date_today):
-    """When annotate --skip-existing on a file that already contains SPDX info,
+    """When annotate --skip-existing on a file that already contains REUSE info,
     don't write additional information to it.
     """
     for path in ("foo.py", "bar.py"):
         (fake_repository / path).write_text("pass")
     expected_foo = cleandoc(
         """
         # SPDX-FileCopyrightText: 2018 Jane Doe
```

### Comparing `reuse-1.1.2/tests/test_main_annotate_merge.py` & `reuse-2.0.0/tests/test_main_annotate_merge.py`

 * *Files identical despite different names*

### Comparing `reuse-1.1.2/tests/test_project.py` & `reuse-2.0.0/tests/test_project.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,29 +4,30 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Tests for reuse.project."""
 
 import os
 import shutil
+from importlib import import_module
 from inspect import cleandoc
 from pathlib import Path
 from textwrap import dedent
 
 import pytest
 from license_expression import LicenseSymbol
 
 from reuse.project import Project
 
 try:
-    import posix as is_posix
+    IS_POSIX = bool(import_module("posix"))
 except ImportError:
-    is_posix = False
+    IS_POSIX = False
 
-posix = pytest.mark.skipif(not is_posix, reason="Windows not supported")
+posix = pytest.mark.skipif(not IS_POSIX, reason="Windows not supported")
 
 TESTS_DIRECTORY = Path(__file__).parent.resolve()
 RESOURCES_DIRECTORY = TESTS_DIRECTORY / "resources"
 
 
 # REUSE-IgnoreStart
 
@@ -197,139 +198,139 @@
 def test_all_files_hg_ignored_contains_newline(hg_repository):
     """File names that contain newlines are also ignored."""
     (hg_repository / "hello\nworld.pyc").touch()
     project = Project(hg_repository)
     assert Path("hello\nworld.pyc").absolute() not in project.all_files()
 
 
-def test_spdx_info_of_file_does_not_exist(fake_repository):
-    """Raise FileNotFoundError when asking for the SPDX info of a file that
+def test_reuse_info_of_file_does_not_exist(fake_repository):
+    """Raise FileNotFoundError when asking for the REUSE info of a file that
     does not exist.
     """
     project = Project(fake_repository)
     with pytest.raises(FileNotFoundError):
-        project.spdx_info_of(fake_repository / "does_not_exist")
+        project.reuse_info_of(fake_repository / "does_not_exist")
 
 
-def test_spdx_info_of_directory(empty_directory):
-    """Raise IsADirectoryError when calling spdx_info_of on a directory."""
+def test_reuse_info_of_directory(empty_directory):
+    """Raise IsADirectoryError when calling reuse_info_of on a directory."""
     (empty_directory / "src").mkdir()
 
     project = Project(empty_directory)
     with pytest.raises((IsADirectoryError, PermissionError)):
-        project.spdx_info_of(empty_directory / "src")
+        project.reuse_info_of(empty_directory / "src")
 
 
-def test_spdx_info_of_unlicensed_file(fake_repository):
-    """Return an empty SpdxInfo object when asking for the SPDX information
-    of a file that has no SPDX information.
+def test_reuse_info_of_unlicensed_file(fake_repository):
+    """Return an empty ReuseInfo object when asking for the REUSE information
+    of a file that has no REUSE information.
     """
     (fake_repository / "foo.py").write_text("foo")
     project = Project(fake_repository)
-    assert not any(project.spdx_info_of("foo.py"))
+    assert not bool(project.reuse_info_of("foo.py"))
 
 
-def test_spdx_info_of_only_copyright(fake_repository):
+def test_reuse_info_of_only_copyright(fake_repository):
     """A file contains only a copyright line. Test whether it correctly picks
     up on that.
     """
     (fake_repository / "foo.py").write_text(
         "SPDX-FileCopyrightText: 2017 Jane Doe"
     )
     project = Project(fake_repository)
-    spdx_info = project.spdx_info_of("foo.py")
-    assert not any(spdx_info.spdx_expressions)
-    assert len(spdx_info.copyright_lines) == 1
+    reuse_info = project.reuse_info_of("foo.py")
+    assert not any(reuse_info.spdx_expressions)
+    assert len(reuse_info.copyright_lines) == 1
     assert (
-        spdx_info.copyright_lines.pop()
+        reuse_info.copyright_lines.pop()
         == "SPDX-FileCopyrightText: 2017 Jane Doe"
     )
 
 
-def test_spdx_info_of_only_copyright_also_covered_by_debian(fake_repository):
+def test_reuse_info_of_only_copyright_also_covered_by_debian(fake_repository):
     """A file contains only a copyright line, but debian/copyright also has
-    information on this file. Use both.
+    information on this file. Use only the information from file header.
     """
     (fake_repository / "doc/foo.py").write_text(
         "SPDX-FileCopyrightText: in file"
     )
     project = Project(fake_repository)
-    spdx_info = project.spdx_info_of("doc/foo.py")
-    assert any(spdx_info.spdx_expressions)
-    assert len(spdx_info.copyright_lines) == 2
-    assert "SPDX-FileCopyrightText: in file" in spdx_info.copyright_lines
-    assert "2017 Jane Doe" in spdx_info.copyright_lines
+    reuse_info = project.reuse_info_of("doc/foo.py")
 
+    assert len(reuse_info.copyright_lines) == 1
+    assert "SPDX-FileCopyrightText: in file" in reuse_info.copyright_lines
 
-def test_spdx_info_of_also_covered_by_dep5(fake_repository):
-    """A file contains all SPDX information, but .reuse/dep5 also
-    provides information on this file. Use both.
+
+def test_reuse_info_of_also_covered_by_dep5(fake_repository):
+    """A file contains all REUSE information, but .reuse/dep5 also
+    provides information on this file. Use only the information
+    from the file header.
     """
     (fake_repository / "doc/foo.py").write_text(
         dedent(
             """
             SPDX-License-Identifier: MIT
             SPDX-FileCopyrightText: in file"""
         )
     )
     project = Project(fake_repository)
-    spdx_info = project.spdx_info_of("doc/foo.py")
-    assert LicenseSymbol("MIT") in spdx_info.spdx_expressions
-    assert LicenseSymbol("CC0-1.0") in spdx_info.spdx_expressions
-    assert "SPDX-FileCopyrightText: in file" in spdx_info.copyright_lines
-    assert "2017 Jane Doe" in spdx_info.copyright_lines
+    reuse_info = project.reuse_info_of("doc/foo.py")
+    assert LicenseSymbol("MIT") in reuse_info.spdx_expressions
+    assert LicenseSymbol("CC0-1.0") not in reuse_info.spdx_expressions
+    assert "SPDX-FileCopyrightText: in file" in reuse_info.copyright_lines
+    assert "2017 Jane Doe" not in reuse_info.copyright_lines
 
 
-def test_spdx_info_of_no_duplicates(empty_directory):
-    """A file contains the same lines twice. The SpdxInfo only contains those
+def test_reuse_info_of_no_duplicates(empty_directory):
+    """A file contains the same lines twice. The ReuseInfo only contains those
     lines once.
     """
     spdx_line = "SPDX-License-Identifier: GPL-3.0-or-later\n"
     copyright_line = (
         "SPDX-FileCopyrightText: 2017 Free Software Foundation Europe\n"
     )
     text = spdx_line + copyright_line
 
     (empty_directory / "foo.py").write_text(text * 2)
     project = Project(empty_directory)
-    spdx_info = project.spdx_info_of("foo.py")
-    assert len(spdx_info.spdx_expressions) == 1
-    assert LicenseSymbol("GPL-3.0-or-later") in spdx_info.spdx_expressions
-    assert len(spdx_info.copyright_lines) == 1
+    reuse_info = project.reuse_info_of("foo.py")
+    assert len(reuse_info.spdx_expressions) == 1
+    assert LicenseSymbol("GPL-3.0-or-later") in reuse_info.spdx_expressions
+    assert len(reuse_info.copyright_lines) == 1
     assert (
         "SPDX-FileCopyrightText: 2017 Free Software Foundation Europe"
-        in spdx_info.copyright_lines
+        in reuse_info.copyright_lines
     )
 
 
-def test_spdx_info_of_binary_succeeds(fake_repository):
-    """spdx_info_of succeeds when the target is covered by dep5."""
+def test_reuse_info_of_binary_succeeds(fake_repository):
+    """reuse_info_of succeeds when the target is covered by dep5."""
     shutil.copy(
         RESOURCES_DIRECTORY / "fsfe.png", fake_repository / "doc/fsfe.png"
     )
 
     project = Project(fake_repository)
-    spdx_info = project.spdx_info_of("doc/fsfe.png")
-    assert LicenseSymbol("CC0-1.0") in spdx_info.spdx_expressions
+    reuse_info = project.reuse_info_of("doc/fsfe.png")
+    assert LicenseSymbol("CC0-1.0") in reuse_info.spdx_expressions
 
 
 def test_license_file_detected(empty_directory):
     """Test whether---when given a file and a license file---the license file
     is detected and read.
     """
     (empty_directory / "foo.py").write_text("foo")
     (empty_directory / "foo.py.license").write_text(
         "SPDX-FileCopyrightText: 2017 Jane Doe\nSPDX-License-Identifier: MIT\n"
     )
 
     project = Project(empty_directory)
-    spdx_info = project.spdx_info_of("foo.py")
+    reuse_info = project.reuse_info_of("foo.py")
 
-    assert "SPDX-FileCopyrightText: 2017 Jane Doe" in spdx_info.copyright_lines
-    assert LicenseSymbol("MIT") in spdx_info.spdx_expressions
+    assert "SPDX-FileCopyrightText: 2017 Jane Doe" in reuse_info.copyright_lines
+    assert LicenseSymbol("MIT") in reuse_info.spdx_expressions
 
 
 def test_licenses_filename(empty_directory):
     """Detect the license identifier of a license from its stem."""
     (empty_directory / "LICENSES").mkdir()
     (empty_directory / "LICENSES/foo.txt").write_text("foo")
     project = Project(empty_directory)
```

### Comparing `reuse-1.1.2/tests/test_report.py` & `reuse-2.0.0/tests/test_report.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,117 +1,229 @@
 # SPDX-FileCopyrightText: 2017 Free Software Foundation Europe e.V. <https://fsfe.org>
 # SPDX-FileCopyrightText: 2022 Florian Snow <florian@familysnow.net>
+# SPDX-FileCopyrightText: 2022 Pietro Albini <pietro.albini@ferrous-systems.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Tests for reuse.report"""
 
 
 import os
 import sys
+from importlib import import_module
 
 import pytest
 
 from reuse.project import Project
 from reuse.report import FileReport, ProjectReport
 
 try:
-    import posix as is_posix
+    IS_POSIX = bool(import_module("posix"))
 except ImportError:
-    is_posix = False
+    IS_POSIX = False
 
 cpython = pytest.mark.skipif(
     sys.implementation.name != "cpython", reason="only CPython supported"
 )
-posix = pytest.mark.skipif(not is_posix, reason="Windows not supported")
+posix = pytest.mark.skipif(not IS_POSIX, reason="Windows not supported")
 
 
 # REUSE-IgnoreStart
 
 
-def test_generate_file_report_file_simple(fake_repository):
+def test_generate_file_report_file_simple(
+    fake_repository, add_license_concluded
+):
     """An extremely simple generate test, just to see if the function doesn't
     crash.
     """
     project = Project(fake_repository)
-    result = FileReport.generate(project, "src/source_code.py")
+    result = FileReport.generate(
+        project,
+        "src/source_code.py",
+        add_license_concluded=add_license_concluded,
+    )
+
     assert result.spdxfile.licenses_in_file == ["GPL-3.0-or-later"]
+    assert (
+        result.spdxfile.license_concluded == "GPL-3.0-or-later"
+        if add_license_concluded
+        else "NOASSERTION"
+    )
     assert result.spdxfile.copyright == "SPDX-FileCopyrightText: 2017 Jane Doe"
     assert not result.bad_licenses
     assert not result.missing_licenses
 
 
-def test_generate_file_report_file_from_different_cwd(fake_repository):
+def test_generate_file_report_file_from_different_cwd(
+    fake_repository, add_license_concluded
+):
     """Another simple generate test, but from a different CWD."""
     os.chdir("/")
     project = Project(fake_repository)
     result = FileReport.generate(
-        project, fake_repository / "src/source_code.py"
+        project,
+        fake_repository / "src/source_code.py",
+        add_license_concluded=add_license_concluded,
     )
     assert result.spdxfile.licenses_in_file == ["GPL-3.0-or-later"]
+    assert (
+        result.spdxfile.license_concluded == "GPL-3.0-or-later"
+        if add_license_concluded
+        else "NOASSERTION"
+    )
     assert result.spdxfile.copyright == "SPDX-FileCopyrightText: 2017 Jane Doe"
     assert not result.bad_licenses
     assert not result.missing_licenses
 
 
-def test_generate_file_report_file_missing_license(fake_repository):
+def test_generate_file_report_file_missing_license(
+    fake_repository, add_license_concluded
+):
     """Simple generate test with a missing license."""
     (fake_repository / "foo.py").write_text(
         "SPDX-License-Identifier: BSD-3-Clause"
     )
     project = Project(fake_repository)
-    result = FileReport.generate(project, "foo.py")
+    result = FileReport.generate(
+        project, "foo.py", add_license_concluded=add_license_concluded
+    )
 
     assert result.spdxfile.copyright == ""
+    assert result.spdxfile.licenses_in_file == ["BSD-3-Clause"]
+    assert (
+        result.spdxfile.license_concluded == "BSD-3-Clause"
+        if add_license_concluded
+        else "NOASSERTION"
+    )
     assert result.missing_licenses == {"BSD-3-Clause"}
     assert not result.bad_licenses
 
 
-def test_generate_file_report_file_bad_license(fake_repository):
+def test_generate_file_report_file_bad_license(
+    fake_repository, add_license_concluded
+):
     """Simple generate test with a bad license."""
     (fake_repository / "foo.py").write_text(
         "SPDX-License-Identifier: fakelicense"
     )
     project = Project(fake_repository)
-    result = FileReport.generate(project, "foo.py")
+    result = FileReport.generate(
+        project, "foo.py", add_license_concluded=add_license_concluded
+    )
 
     assert result.spdxfile.copyright == ""
+    assert result.spdxfile.licenses_in_file == ["fakelicense"]
+    assert (
+        result.spdxfile.license_concluded == "fakelicense"
+        if add_license_concluded
+        else "NOASSERTION"
+    )
     assert result.bad_licenses == {"fakelicense"}
     assert result.missing_licenses == {"fakelicense"}
 
 
-def test_generate_file_report_license_contains_plus(fake_repository):
+def test_generate_file_report_license_contains_plus(
+    fake_repository, add_license_concluded
+):
     """Given a license expression akin to Apache-1.0+, LICENSES/Apache-1.0.txt
     should be an appropriate license file.
     """
     (fake_repository / "foo.py").write_text(
         "SPDX-License-Identifier: Apache-1.0+"
     )
     (fake_repository / "LICENSES/Apache-1.0.txt").touch()
     project = Project(fake_repository)
-    result = FileReport.generate(project, "foo.py")
+    result = FileReport.generate(
+        project, "foo.py", add_license_concluded=add_license_concluded
+    )
 
     assert result.spdxfile.copyright == ""
+    assert result.spdxfile.licenses_in_file == ["Apache-1.0+"]
+    assert (
+        result.spdxfile.license_concluded == "Apache-1.0+"
+        if add_license_concluded
+        else "NOASSERTION"
+    )
     assert not result.bad_licenses
     assert not result.missing_licenses
 
 
-def test_generate_file_report_exception(fake_repository):
+def test_generate_file_report_exception(fake_repository, add_license_concluded):
     """Simple generate test to test if the exception is detected."""
     project = Project(fake_repository)
-    result = FileReport.generate(project, "src/exception.py")
+    result = FileReport.generate(
+        project, "src/exception.py", add_license_concluded=add_license_concluded
+    )
+
     assert set(result.spdxfile.licenses_in_file) == {
         "GPL-3.0-or-later",
         "Autoconf-exception-3.0",
     }
+    assert (
+        result.spdxfile.license_concluded
+        == "GPL-3.0-or-later WITH Autoconf-exception-3.0"
+        if add_license_concluded
+        else "NOASSERTION"
+    )
     assert result.spdxfile.copyright == "SPDX-FileCopyrightText: 2017 Jane Doe"
     assert not result.bad_licenses
     assert not result.missing_licenses
 
 
+def test_generate_file_report_no_licenses(
+    fake_repository, add_license_concluded
+):
+    """Test behavior when no license information is present in the file"""
+    (fake_repository / "foo.py").write_text("")
+    project = Project(fake_repository)
+    result = FileReport.generate(
+        project, "foo.py", add_license_concluded=add_license_concluded
+    )
+
+    assert result.spdxfile.copyright == ""
+    assert not result.spdxfile.licenses_in_file
+    assert (
+        result.spdxfile.license_concluded == "NONE"
+        if add_license_concluded
+        else "NOASSERTION"
+    )
+    assert not result.bad_licenses
+    assert not result.missing_licenses
+
+
+def test_generate_file_report_multiple_licenses(
+    fake_repository, add_license_concluded
+):
+    """Test that all licenses are included in LicenseConcluded"""
+    project = Project(fake_repository)
+    result = FileReport.generate(
+        project,
+        "src/multiple_licenses.rs",
+        add_license_concluded=add_license_concluded,
+    )
+
+    assert result.spdxfile.copyright == "SPDX-FileCopyrightText: 2022 Jane Doe"
+    assert set(result.spdxfile.licenses_in_file) == {
+        "GPL-3.0-or-later",
+        "Apache-2.0",
+        "CC0-1.0",
+        "Autoconf-exception-3.0",
+    }
+    assert (
+        result.spdxfile.license_concluded
+        == "GPL-3.0-or-later AND (Apache-2.0 OR CC0-1.0"
+        " WITH Autoconf-exception-3.0)"
+        if add_license_concluded
+        else "NOASSERTION"
+    )
+    assert not result.bad_licenses
+    assert not result.missing_licenses
+
+
 def test_generate_project_report_simple(fake_repository, multiprocessing):
     """Simple generate test, just to see if it sort of works."""
     project = Project(fake_repository)
     result = ProjectReport.generate(project, multiprocessing=multiprocessing)
 
     assert not result.bad_licenses
     assert not result.licenses_without_extension
@@ -263,20 +375,29 @@
     project = Project(fake_repository)
     result = ProjectReport.generate(project, multiprocessing=multiprocessing)
 
     # pylint: disable=superfluous-parens
     assert (fake_repository / "bad") in result.read_errors
 
 
-def test_generate_project_report_to_dict(fake_repository, multiprocessing):
-    """Extremely simple test for ProjectReport.to_dict."""
+def test_generate_project_report_to_dict_lint(fake_repository, multiprocessing):
+    """Generate dictionary output and verify correct ordering."""
     project = Project(fake_repository)
     report = ProjectReport.generate(project, multiprocessing=multiprocessing)
-    # TODO: Actually do something
-    report.to_dict()
+    result = report.to_dict_lint()
+
+    # Check if the top three keys are at the beginning of the dictionary
+    assert list(result.keys())[:3] == [
+        "lint_version",
+        "reuse_spec_version",
+        "reuse_tool_version",
+    ]
+
+    # Check if the rest of the keys are sorted alphabetically
+    assert list(result.keys())[3:] == sorted(list(result.keys())[3:])
 
 
 def test_bill_of_materials(fake_repository, multiprocessing):
     """Generate a bill of materials."""
     project = Project(fake_repository)
     report = ProjectReport.generate(project, multiprocessing=multiprocessing)
     # TODO: Actually do something
```

### Comparing `reuse-1.1.2/tests/test_util.py` & `reuse-2.0.0/tests/test_util.py`

 * *Files 15% similar despite different names*

```diff
@@ -42,23 +42,23 @@
 # REUSE-IgnoreStart
 
 
 def test_extract_expression():
     """Parse various expressions."""
     expressions = ["GPL-3.0+", "GPL-3.0 AND CC0-1.0", "nonsense"]
     for expression in expressions:
-        result = _util.extract_spdx_info(
+        result = _util.extract_reuse_info(
             f"SPDX-License-Identifier: {expression}"
         )
         assert result.spdx_expressions == {_LICENSING.parse(expression)}
 
 
 def test_extract_expression_from_ascii_art_frame():
     """Parse an expression from an ASCII art frame"""
-    result = _util.extract_spdx_info(
+    result = _util.extract_reuse_info(
         cleandoc(
             """
              /**********************************\\
              |*  SPDX-License-Identifier: MIT  *|
              \\**********************************/
             """
         )
@@ -66,77 +66,77 @@
     assert result.spdx_expressions == {_LICENSING.parse("MIT")}
 
 
 def test_extract_erroneous_expression():
     """Parse an incorrect expression."""
     expression = "SPDX-License-Identifier: GPL-3.0-or-later AND (MIT OR)"
     with pytest.raises(ParseError):
-        _util.extract_spdx_info(expression)
+        _util.extract_reuse_info(expression)
 
 
 def test_extract_no_info():
-    """Given a file without SPDX information, return an empty SpdxInfo
+    """Given a string without REUSE information, return an empty ReuseInfo
     object.
     """
-    result = _util.extract_spdx_info("")
-    assert result == _util.SpdxInfo(set(), set())
+    result = _util.extract_reuse_info("")
+    assert result == _util.ReuseInfo()
 
 
 def test_extract_tab():
     """A tag followed by a tab is also valid."""
-    result = _util.extract_spdx_info("SPDX-License-Identifier:\tMIT")
+    result = _util.extract_reuse_info("SPDX-License-Identifier:\tMIT")
     assert result.spdx_expressions == {_LICENSING.parse("MIT")}
 
 
 def test_extract_many_whitespace():
     """When a tag is followed by a lot of whitespace, the whitespace should be
     filtered out.
     """
-    result = _util.extract_spdx_info("SPDX-License-Identifier:    MIT")
+    result = _util.extract_reuse_info("SPDX-License-Identifier:    MIT")
     assert result.spdx_expressions == {_LICENSING.parse("MIT")}
 
 
 def test_extract_bibtex_comment():
     """A special case for BibTex comments."""
     expression = "@Comment{SPDX-License-Identifier: GPL-3.0-or-later}"
-    result = _util.extract_spdx_info(expression)
+    result = _util.extract_reuse_info(expression)
     assert str(list(result.spdx_expressions)[0]) == "GPL-3.0-or-later"
 
 
 def test_extract_copyright():
     """Given a file with copyright information, have it return that copyright
     information.
     """
     copyright_line = "SPDX-FileCopyrightText: 2019 Jane Doe"
-    result = _util.extract_spdx_info(copyright_line)
+    result = _util.extract_reuse_info(copyright_line)
     assert result.copyright_lines == {copyright_line}
 
 
 def test_extract_copyright_duplicate():
     """When a copyright line is duplicated, only yield one."""
     copyright_line = "SPDX-FileCopyrightText: 2019 Jane Doe"
-    result = _util.extract_spdx_info(
+    result = _util.extract_reuse_info(
         "\n".join((copyright_line, copyright_line))
     )
     assert result.copyright_lines == {copyright_line}
 
 
 def test_extract_copyright_tab():
     """A tag followed by a tab is also valid."""
     copyright_line = "SPDX-FileCopyrightText:\t2019 Jane Doe"
-    result = _util.extract_spdx_info(copyright_line)
+    result = _util.extract_reuse_info(copyright_line)
     assert result.copyright_lines == {copyright_line}
 
 
 def test_extract_copyright_many_whitespace():
     """When a tag is followed by a lot of whitespace, that is also valid. The
     whitespace is not filtered out.
     """
     copyright_line = "SPDX-FileCopyrightText:    2019 Jane Doe"
-    result = _util.extract_spdx_info(copyright_line)
+    result = _util.extract_reuse_info(copyright_line)
     assert result.copyright_lines == {copyright_line}
 
 
 def test_extract_copyright_variations():
     """There are multiple ways to declare copyright. All should be detected."""
     text = cleandoc(
         """
@@ -145,15 +145,15 @@
         © 2019 Jane Doe
         Copyright © 2019 Jane Doe
         Copyright 2019 Jane Doe
         Copyright (C) 2019 Jane Doe
         """
     )
 
-    result = _util.extract_spdx_info(text)
+    result = _util.extract_reuse_info(text)
     lines = text.splitlines()
     for line in lines:
         assert line in result.copyright_lines
     assert len(lines) == len(result.copyright_lines)
 
 
 def test_extract_with_ignore_block():
@@ -167,25 +167,25 @@
         REUSE-IgnoreStart
         SPDX-FileCopyrightText: 2019 John Doe
         SPDX-License-Identifier: GPL-3.0-or-later
         REUSE-IgnoreEnd
         SPDX-FileCopyrightText: 2019 Eve
         """
     )
-    result = _util.extract_spdx_info(text)
+    result = _util.extract_reuse_info(text)
     assert len(result.copyright_lines) == 2
     assert len(result.spdx_expressions) == 1
 
 
 def test_extract_sameline_multiline():
     """When a copyright line is in a multi-line style comment on a single line,
     do not include the comment end pattern as part of the copyright.
     """
     text = "<!-- SPDX-FileCopyrightText: Jane Doe -->"
-    result = _util.extract_spdx_info(text)
+    result = _util.extract_reuse_info(text)
     assert len(result.copyright_lines) == 1
     assert result.copyright_lines == {"SPDX-FileCopyrightText: Jane Doe"}
 
 
 def test_extract_special_endings():
     """Strip some non-comment-style endings from the end of copyright and
     licensing information.
@@ -197,20 +197,31 @@
         <tag value="Copyright 2019 Joe Somebody" />
         <tag value='Copyright 2019 Alice'>
         <tag value='Copyright 2019 Bob' >
         <tag value='Copyright 2019 Eve' />
         [Copyright 2019 Ajnulo] ::
         """
     )
-    result = _util.extract_spdx_info(text)
+    result = _util.extract_reuse_info(text)
     for item in result.copyright_lines:
         assert ">" not in item
         assert "] ::" not in item
 
 
+def test_extract_contributors():
+    """Correctly extract SPDX-FileContributor information from text."""
+    text = cleandoc(
+        """
+        # SPDX-FileContributor: Jane Doe
+        """
+    )
+    result = _util.extract_reuse_info(text)
+    assert result.contributor_lines == {"Jane Doe"}
+
+
 def test_filter_ignore_block_with_comment_style():
     """Test that the ignore block is properly removed if start and end markers
     are in comment style.
     """
     text = cleandoc(
         """
         Relevant text
@@ -404,14 +415,22 @@
     """Given a simple statement, style and a year, make it a copyright line."""
     statement = _util.make_copyright_line(
         "hello", year=2019, copyright_style="spdx"
     )
     assert statement == "SPDX-FileCopyrightText: 2019 hello"
 
 
+def test_make_copyright_line_style_spdx_c_year():
+    """Given a simple statement, style and a year, make it a copyright line."""
+    statement = _util.make_copyright_line(
+        "hello", year=2019, copyright_style="spdx-c"
+    )
+    assert statement == "SPDX-FileCopyrightText: (C) 2019 hello"
+
+
 def test_make_copyright_line_style_spdx_symbol_year():
     """Given a simple statement, style and a year, make it a copyright line."""
     statement = _util.make_copyright_line(
         "hello", year=2019, copyright_style="spdx-symbol"
     )
     assert statement == "SPDX-FileCopyrightText: © 2019 hello"
```

### Comparing `reuse-1.1.2/tests/test_vcs.py` & `reuse-2.0.0/tests/test_vcs.py`

 * *Files identical despite different names*

### Comparing `reuse-1.1.2/PKG-INFO` & `reuse-2.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 Metadata-Version: 2.1
 Name: reuse
-Version: 1.1.2
+Version: 2.0.0
 Summary: reuse is a tool for compliance with the REUSE recommendations.
 Home-page: https://reuse.software/
-License: Apache-2.0 AND CC0-1.0 AND GPL-3.0-or-later
+License: Apache-2.0 AND CC0-1.0 AND CC-BY-SA-4.0 AND GPL-3.0-or-later
 Author: Free Software Foundation Europe
 Author-email: contact@fsfe.org
 Maintainer: Carmen Bianca Bakker
 Maintainer-email: carmenbianca@fsfe.org
-Requires-Python: >=3.6.2,<4.0.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
+Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
+Classifier: License :: DFSG approved
+Classifier: License :: OSI Approved
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.0.0,<4.0.0)
 Requires-Dist: binaryornot (>=0.4.4,<0.5.0)
 Requires-Dist: boolean.py (>=3.8)
 Requires-Dist: license-expression (>=1.0)
 Requires-Dist: python-debian (>=0.1.38,<0.2.0,!=0.1.45,!=0.1.46,!=0.1.47)
-Requires-Dist: setuptools
 Project-URL: Documentation, https://reuse.readthedocs.org/
 Project-URL: Repository, https://github.com/fsfe/reuse-tool
 Description-Content-Type: text/markdown
 
 <!--
 SPDX-FileCopyrightText: 2017 Free Software Foundation Europe e.V. <https://fsfe.org>
 
@@ -34,37 +38,51 @@
 -->
 
 # reuse
 
 [![The latest version of reuse can be found on PyPI.](https://img.shields.io/pypi/v/reuse.svg)](https://pypi.python.org/pypi/reuse)
 [![Information on what versions of Python reuse supports can be found on PyPI.](https://img.shields.io/pypi/pyversions/reuse.svg)](https://pypi.python.org/pypi/reuse)
 [![REUSE status](https://api.reuse.software/badge/github.com/fsfe/reuse-tool)](https://api.reuse.software/info/github.com/fsfe/reuse-tool)
-[![readme style standard](https://img.shields.io/badge/readme_style-standard-brightgreen.svg)](https://github.com/RichardLitt/standard-readme)
+[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg)](https://github.com/RichardLitt/standard-readme)
 [![Packaging status](https://repology.org/badge/tiny-repos/reuse.svg?header=in%20distro%20repos)](https://repology.org/project/reuse/versions)
+[![Translation status](https://hosted.weblate.org/widgets/fsfe/-/reuse-tool/svg-badge.svg)](https://hosted.weblate.org/projects/fsfe/reuse-tool/)
 
-> reuse is a tool for compliance with the [REUSE](https://reuse.software/)
-> recommendations.
+reuse is a tool for compliance with the [REUSE](https://reuse.software/)
+recommendations.
 
 - Documentation: <https://reuse.readthedocs.io> and <https://reuse.software>
 - Source code: <https://github.com/fsfe/reuse-tool>
 - PyPI: <https://pypi.python.org/pypi/reuse>
 - REUSE: 3.0
-- Python: 3.6+
+- Python: 3.8+
+
+## Table of contents
+
+- [Background](#background)
+- [Install](#install)
+- [Usage](#usage)
+- [Maintainers](#maintainers)
+- [Contributing](#contributing)
+- [License](#license)
 
 ## Background
 
+<!-- REUSE-IgnoreStart -->
+
 Copyright and licensing is difficult, especially when reusing software from
 different projects that are released under various different licenses.
 [REUSE](https://reuse.software) was started by the
 [Free Software Foundation Europe](https://fsfe.org) (FSFE) to provide a set of
 recommendations to make licensing your Free Software projects easier. Not only
 do these recommendations make it easier for you to declare the licenses under
 which your works are released, but they also make it easier for a computer to
 understand how your project is licensed.
 
+<!-- REUSE-IgnoreEnd -->
+
 As a short summary, the recommendations are threefold:
 
 1. Choose and provide licenses
 2. Add copyright and licensing information to each file
 3. Confirm REUSE compliance
 
 You are recommended to read [our tutorial](https://reuse.software/tutorial) for
@@ -78,39 +96,21 @@
 
 There are [other tools](https://reuse.software/comparison) that have a lot more
 features and functionality surrounding the analysis and inspection of copyright
 and licenses in software projects. The REUSE helper tool, on the other hand, is
 solely designed to be a simple tool to assist in compliance with the REUSE
 recommendations.
 
-## Example demo
-
-In this screencast, we are going to follow the
-[tutorial](https://reuse.software/tutorial), making the
-[REUSE example repository](https://github.com/fsfe/reuse-example/) compliant.
-
-![Demo of some basic REUSE tool commands](https://download.fsfe.org/videos/reuse/screencasts/reuse-tool.gif)
-
 ## Install
 
-### Installation via package managers (Recommended)
+### Installation via package manager (Recommended)
 
-There are packages available for easy install on some operating systems. You are
+There are packages available for easy install on many operating systems. You are
 welcome to help us package this tool for more distributions!
 
-- Alpine Linux: [reuse](https://pkgs.alpinelinux.org/packages?name=reuse)
-- Arch Linux: [reuse](https://archlinux.org/packages/community/any/reuse/)
-- Debian: [reuse](https://packages.debian.org/search?keywords=reuse&exact=1)
-- GNU Guix: [reuse](https://guix.gnu.org/en/packages/reuse-1.0.0/)
-- Fedora: [reuse](https://packages.fedoraproject.org/pkgs/reuse/reuse/)
-- MacPorts: [reuse](https://ports.macports.org/port/reuse/)
-- NixOS: [reuse](https://search.nixos.org/packages?show=reuse)
-- openSUSE: [reuse](https://software.opensuse.org/package/reuse)
-- VoidLinux: [reuse](https://voidlinux.org/packages/?arch=x86_64&q=reuse)
-
 An automatically generated list can be found at
 [repology.org](https://repology.org/project/reuse/versions), without any
 guarantee for completeness.
 
 ### Install and run via pipx (Recommended)
 
 The following one-liner both installs and runs this tool from
@@ -131,44 +131,47 @@
 ```bash
 pipx install reuse
 ```
 
 reuse will then be available in `~/.local/bin`, which must be added to your
 `$PATH`.
 
-### Installation via pip
-
-To install reuse, you need to have the following pieces of software on your
-computer:
-
-- Python 3.6+
-- pip
-
-You then only need to run the following command:
-
-```bash
-pip3 install --user reuse
-```
-
 After this, make sure that `~/.local/bin` is in your `$PATH`. On Windows, the
 required path for your environment may look like
 `%USERPROFILE%\AppData\Roaming\Python\Python39\Scripts`, depending on the Python
 version you have installed.
 
-To update reuse, run this command:
+To upgrade reuse, run this command:
 
 ```bash
-pip3 install --user --upgrade reuse
+pipx upgrade reuse
 ```
 
 For full functionality, the following pieces of software are recommended:
 
 - Git
 - Mercurial 4.3+
 
+### Installation via pip
+
+To install reuse into `~/.local/bin`, run:
+
+```bash
+pip3 install --user reuse
+```
+
+Subsequently, make sure that `~/.local/bin` is in your `$PATH` like described in
+the previous section.
+
+To upgrade reuse, run this command:
+
+```bash
+pip3 install --user --upgrade reuse
+```
+
 ### Installation from source
 
 You can also install this tool from the source code, but we recommend the
 methods above for easier and more stable updates. Please make sure the
 requirements for the installation via pip are present on your machine.
 
 ```bash
@@ -176,14 +179,16 @@
 ```
 
 ## Usage
 
 First, read the [REUSE tutorial](https://reuse.software/tutorial/). In a
 nutshell:
 
+<!-- REUSE-IgnoreStart -->
+
 1. Put your licenses in the `LICENSES/` directory.
 2. Add a comment header to each file that says
    `SPDX-License-Identifier: GPL-3.0-or-later`, and
    `SPDX-FileCopyrightText: $YEAR $NAME`. You can be flexible with the format,
    just make sure that the line starts with `SPDX-FileCopyrightText:`.
 3. Verify your work using this tool.
 
@@ -191,39 +196,46 @@
 
 ```
 # SPDX-FileCopyrightText: 2017 Free Software Foundation Europe e.V. <https://fsfe.org>
 #
 # SPDX-License-Identifier: CC-BY-SA-4.0
 ```
 
+<!-- REUSE-IgnoreEnd -->
+
+### CLI
+
 To check against the recommendations, use `reuse lint`:
 
 ```
 ~/Projects/reuse-tool $ reuse lint
 [...]
 
 Congratulations! Your project is compliant with version 3.0 of the REUSE Specification :-)
 ```
 
 This tool can do various more things, detailed in the documentation. Here a
 short summary:
 
 - `annotate` --- Add copyright and/or licensing information to the header of a
   file.
-
 - `download` --- Download the specified license into the `LICENSES/` directory.
-
 - `init` --- Set up the project for REUSE compliance.
-
 - `lint` --- Verify the project for REUSE compliance.
-
 - `spdx` --- Generate an SPDX Document of all files in the project.
-
 - `supported-licenses` --- Prints all licenses supported by REUSE.
 
+### Example demo
+
+In this screencast, we are going to follow the
+[tutorial](https://reuse.software/tutorial), making the
+[REUSE example repository](https://github.com/fsfe/reuse-example/) compliant.
+
+![Demo of some basic REUSE tool commands](https://download.fsfe.org/videos/reuse/screencasts/reuse-tool.gif)
+
 ### Run in Docker
 
 The `fsfe/reuse` Docker image is available on
 [Docker Hub](https://hub.docker.com/r/fsfe/reuse). With it, you can easily
 include REUSE in CI/CD processes. This way, you can check for REUSE compliance
 for each build. In our [resources for developers](https://reuse.software/dev/)
 you can learn how to integrate the REUSE tool in Drone, Travis, GitHub, or
@@ -260,60 +272,51 @@
 Git. This uses [pre-commit](https://pre-commit.com/). Once you
 [have it installed](https://pre-commit.com/#install), add this to the
 `.pre-commit-config.yaml` in your repository:
 
 ```yaml
 repos:
   - repo: https://github.com/fsfe/reuse-tool
-    rev: v1.1.2
+    rev: v2.0.0
     hooks:
       - id: reuse
 ```
 
 Then run `pre-commit install`. Now, every time you commit, `reuse lint` is run
 in the background, and will prevent your commit from going through if there was
 an error.
 
 ## Maintainers
 
-- Carmen Bianca Bakker - <carmenbianca@fsfe.org>
-- Max Mehl - <max.mehl@fsfe.org>
-
-## Contribute
-
-Any pull requests or suggestions are welcome at
-<https://github.com/fsfe/reuse-tool> or via e-mail to one of the maintainers.
-General inquiries can be sent to <reuse@lists.fsfe.org>.
-
-Interaction within this project is covered by the
-[FSFE's Code of Conduct](https://fsfe.org/about/codeofconduct).
+- Carmen Bianca Bakker <carmenbianca@fsfe.org>
+- Max Mehl <max.mehl@fsfe.org>
+- Linus Sehn <linus@fsfe.org>
+
+## Contributing
+
+If you're interested in contributing to the reuse project, there are several
+ways to get involved. Development of the project takes place on GitHub at
+<https://github.com/fsfe/reuse-tool>. There, you can submit bug reports, feature
+requests, and pull requests. Even and especially when in doubt, feel free to
+open an issue with a question. Contributions of all types are welcome, and the
+development team is happy to provide guidance and support for new contributors.
 
-Starting local development is very simple, just execute the following commands:
-
-```bash
-git clone git@github.com:fsfe/reuse-tool.git
-cd reuse-tool/
-poetry install  # You may need to install poetry using your package manager.
-poetry run pre-commit install  # Using poetry is optional here if you already have pre-commit.
-```
+Additionally, the <reuse@lists.fsfe.org> mailing list is available for
+discussion and support related to the project.
 
-Next, you'll find the following commands handy:
-
-- `poetry run reuse`
-- `poetry run pytest`
-- `poetry run pylint src`
-- `make docs`
+You can find the full contribution guidelines at
+<https://reuse.readthedocs.io/en/latest/contributing.html>.
 
 ## License
 
 This work is licensed under multiple licences. Because keeping this section
-up-to-date is challenging, here is a brief summary as of April 2020:
+up-to-date is challenging, here is a brief summary as of February 2023:
 
 - All original source code is licensed under GPL-3.0-or-later.
 - All documentation is licensed under CC-BY-SA-4.0.
 - Some configuration and data files are licensed under CC0-1.0.
 - Some code borrowed from
-  [spdx/tool-python](https://github.com/spdx/tools-python) is licensed under
+  [spdx/tools-python](https://github.com/spdx/tools-python) is licensed under
   Apache-2.0.
 
 For more accurate information, check the individual files.
```

