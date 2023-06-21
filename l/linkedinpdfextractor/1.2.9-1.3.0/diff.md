# Comparing `tmp/linkedinpdfextractor-1.2.9.tar.gz` & `tmp/linkedinpdfextractor-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkedinpdfextractor-1.2.9.tar", last modified: Fri May 26 11:51:09 2023, max compression
+gzip compressed data, was "linkedinpdfextractor-1.3.0.tar", last modified: Wed Jun 21 07:07:03 2023, max compression
```

## Comparing `linkedinpdfextractor-1.2.9.tar` & `linkedinpdfextractor-1.3.0.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-26 11:51:09.958694 linkedinpdfextractor-1.2.9/
--rw-r--r--   0 seshivitakula   (501) staff       (20)     8196 2023-05-05 08:33:17.000000 linkedinpdfextractor-1.2.9/.DS_Store
--rw-r--r--   0 seshivitakula   (501) staff       (20)     1829 2023-05-25 06:34:04.000000 linkedinpdfextractor-1.2.9/.gitignore
--rw-r--r--   0 seshivitakula   (501) staff       (20)       82 2023-04-21 07:18:22.000000 linkedinpdfextractor-1.2.9/AUTHORS.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)      128 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.9/CHANGELOG.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)    14010 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.9/CONTRIBUTING.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)     1078 2023-04-19 16:57:33.000000 linkedinpdfextractor-1.2.9/LICENSE.txt
--rw-r--r--   0 seshivitakula   (501) staff       (20)     1350 2023-05-26 11:51:09.958860 linkedinpdfextractor-1.2.9/PKG-INFO
--rw-r--r--   0 seshivitakula   (501) staff       (20)     1770 2023-05-16 12:16:16.000000 linkedinpdfextractor-1.2.9/README.md
--rw-r--r--   0 seshivitakula   (501) staff       (20)      840 2023-05-16 12:33:10.000000 linkedinpdfextractor-1.2.9/README.rst
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-26 11:51:09.936048 linkedinpdfextractor-1.2.9/docs/
--rw-r--r--   0 seshivitakula   (501) staff       (20)     1154 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.9/docs/Makefile
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-26 11:51:09.936407 linkedinpdfextractor-1.2.9/docs/_static/
--rw-r--r--   0 seshivitakula   (501) staff       (20)       18 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.9/docs/_static/.gitignore
--rw-r--r--   0 seshivitakula   (501) staff       (20)       41 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.9/docs/authors.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)       43 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.9/docs/changelog.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)     9807 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.9/docs/conf.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)       33 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.9/docs/contributing.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2373 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.9/docs/index.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)       67 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.9/docs/license.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)       39 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.9/docs/readme.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)      233 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.9/docs/requirements.txt
--rw-r--r--   0 seshivitakula   (501) staff       (20)      346 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.9/pyproject.toml
--rw-r--r--   0 seshivitakula   (501) staff       (20)       46 2023-04-21 06:26:32.000000 linkedinpdfextractor-1.2.9/requirements.txt
--rw-r--r--   0 seshivitakula   (501) staff       (20)     1249 2023-05-26 11:51:09.959650 linkedinpdfextractor-1.2.9/setup.cfg
--rw-r--r--   0 seshivitakula   (501) staff       (20)      723 2023-05-05 10:18:51.000000 linkedinpdfextractor-1.2.9/setup.py
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-26 11:51:09.937147 linkedinpdfextractor-1.2.9/src/
--rw-r--r--   0 seshivitakula   (501) staff       (20)     6148 2023-04-19 11:25:51.000000 linkedinpdfextractor-1.2.9/src/.DS_Store
--rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-05-26 07:31:17.000000 linkedinpdfextractor-1.2.9/src/__init__.py
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-26 11:51:09.938526 linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/
--rw-r--r--   0 seshivitakula   (501) staff       (20)     6148 2023-04-19 11:27:25.000000 linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/.DS_Store
--rw-r--r--   0 seshivitakula   (501) staff       (20)      577 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/__init__.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     5962 2023-05-26 11:49:27.000000 linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/extractor.py
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-26 11:51:09.939875 linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/pdfstructure/
--rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/pdfstructure/__init__.py
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-26 11:51:09.941355 linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/pdfstructure/analysis/
--rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/pdfstructure/analysis/__init__.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2916 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/pdfstructure/analysis/annotate.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     3691 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/pdfstructure/analysis/sizemapper.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     5496 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/pdfstructure/analysis/styledistribution.py
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-26 11:51:09.942901 linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/pdfstructure/hierarchy/
--rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/pdfstructure/hierarchy/__init__.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     1593 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/pdfstructure/hierarchy/detectheader.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2985 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/pdfstructure/hierarchy/headercompare.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     7296 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/pdfstructure/hierarchy/parser.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2608 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/pdfstructure/hierarchy/traversal.py
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-26 11:51:09.943685 linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/pdfstructure/model/
--rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/pdfstructure/model/__init__.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     4497 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/pdfstructure/model/document.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2108 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/pdfstructure/model/style.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     4155 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/pdfstructure/printer.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     4983 2023-04-21 06:26:32.000000 linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/pdfstructure/source.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     4253 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/pdfstructure/utils.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     4310 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/skeleton.py
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-26 11:51:09.945340 linkedinpdfextractor-1.2.9/src/linkedinpdfextractor.egg-info/
--rw-r--r--   0 seshivitakula   (501) staff       (20)     1350 2023-05-26 11:51:09.000000 linkedinpdfextractor-1.2.9/src/linkedinpdfextractor.egg-info/PKG-INFO
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2574 2023-05-26 11:51:09.000000 linkedinpdfextractor-1.2.9/src/linkedinpdfextractor.egg-info/SOURCES.txt
--rw-r--r--   0 seshivitakula   (501) staff       (20)        1 2023-05-26 11:51:09.000000 linkedinpdfextractor-1.2.9/src/linkedinpdfextractor.egg-info/dependency_links.txt
--rw-r--r--   0 seshivitakula   (501) staff       (20)        1 2023-04-21 07:55:27.000000 linkedinpdfextractor-1.2.9/src/linkedinpdfextractor.egg-info/not-zip-safe
--rw-r--r--   0 seshivitakula   (501) staff       (20)      101 2023-05-26 11:51:09.000000 linkedinpdfextractor-1.2.9/src/linkedinpdfextractor.egg-info/requires.txt
--rw-r--r--   0 seshivitakula   (501) staff       (20)       23 2023-05-26 11:51:09.000000 linkedinpdfextractor-1.2.9/src/linkedinpdfextractor.egg-info/top_level.txt
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-26 11:51:09.950049 linkedinpdfextractor-1.2.9/tests/
--rw-r--r--   0 seshivitakula   (501) staff       (20)     8196 2023-05-05 08:33:17.000000 linkedinpdfextractor-1.2.9/tests/.DS_Store
--rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.9/tests/__init__.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)      290 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.9/tests/conftest.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)      820 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.9/tests/helper.py
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-26 11:51:09.956796 linkedinpdfextractor-1.2.9/tests/resources/
--rw-r--r--   0 seshivitakula   (501) staff       (20)   143869 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.9/tests/resources/5648.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)   401628 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.9/tests/resources/IE00BM67HT60-ATB-FS-DE-2020-2-28.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)    18836 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.9/tests/resources/SameSize_BoldTitle.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)    12108 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.9/tests/resources/SameSize_EnumeratedTitle.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)    12178 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.9/tests/resources/SameStyleOnly.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)    45965 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.9/tests/resources/interview_cheatsheet-excerpt.png
--rwxr-xr-x   0 seshivitakula   (501) staff       (20)   230787 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.9/tests/resources/interview_cheatsheet.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)    32674 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.9/tests/resources/lorem.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)   383508 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.9/tests/resources/paper.pdf
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-26 11:51:09.958414 linkedinpdfextractor-1.2.9/tests/resources/parsed/
--rw-r--r--   0 seshivitakula   (501) staff       (20)   215280 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.9/tests/resources/parsed/interview_cheatsheet.json
--rw-r--r--   0 seshivitakula   (501) staff       (20)    15753 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.9/tests/resources/parsed/interview_cheatsheet_pretty.txt
--rw-r--r--   0 seshivitakula   (501) staff       (20)    62812 2023-04-19 12:12:39.000000 linkedinpdfextractor-1.2.9/tests/resources/profile.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)   251982 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.9/tests/resources/samplepptx.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)     1398 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.9/tests/test_custom_use_cases.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)      656 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.9/tests/test_document.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2304 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.9/tests/test_headercompare.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     4709 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.9/tests/test_hierarchy.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)      199 2023-05-26 07:31:17.000000 linkedinpdfextractor-1.2.9/tests/test_linkedin_parser.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     3202 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.9/tests/test_printer.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)      597 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.9/tests/test_skeleton.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     4276 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.9/tests/test_style_analyser.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     3865 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.9/tests/test_traversal.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)      804 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.9/tests/test_utils.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2690 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.9/tox.ini
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-06-21 07:07:03.865832 linkedinpdfextractor-1.3.0/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     8196 2023-05-05 08:33:17.000000 linkedinpdfextractor-1.3.0/.DS_Store
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     1829 2023-05-25 06:34:04.000000 linkedinpdfextractor-1.3.0/.gitignore
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       82 2023-04-21 07:18:22.000000 linkedinpdfextractor-1.3.0/AUTHORS.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      128 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.3.0/CHANGELOG.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)    14010 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     1078 2023-04-19 16:57:33.000000 linkedinpdfextractor-1.3.0/LICENSE.txt
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     1350 2023-06-21 07:07:03.866031 linkedinpdfextractor-1.3.0/PKG-INFO
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     1770 2023-05-16 12:16:16.000000 linkedinpdfextractor-1.3.0/README.md
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      840 2023-05-16 12:33:10.000000 linkedinpdfextractor-1.3.0/README.rst
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-06-21 07:07:03.831381 linkedinpdfextractor-1.3.0/docs/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     1154 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.3.0/docs/Makefile
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-06-21 07:07:03.831625 linkedinpdfextractor-1.3.0/docs/_static/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       18 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.3.0/docs/_static/.gitignore
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       41 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.3.0/docs/authors.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       43 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.3.0/docs/changelog.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     9807 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.3.0/docs/conf.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       33 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.3.0/docs/contributing.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2373 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.3.0/docs/index.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       67 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.3.0/docs/license.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       39 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.3.0/docs/readme.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      233 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.3.0/docs/requirements.txt
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      346 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.3.0/pyproject.toml
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       46 2023-04-21 06:26:32.000000 linkedinpdfextractor-1.3.0/requirements.txt
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     1249 2023-06-21 07:07:03.867646 linkedinpdfextractor-1.3.0/setup.cfg
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      723 2023-05-05 10:18:51.000000 linkedinpdfextractor-1.3.0/setup.py
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-06-21 07:07:03.832387 linkedinpdfextractor-1.3.0/src/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     6148 2023-04-19 11:25:51.000000 linkedinpdfextractor-1.3.0/src/.DS_Store
+-rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-05-26 07:31:17.000000 linkedinpdfextractor-1.3.0/src/__init__.py
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-06-21 07:07:03.833803 linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     6148 2023-04-19 11:27:25.000000 linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/.DS_Store
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      577 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/__init__.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     6214 2023-06-21 07:04:34.000000 linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/extractor.py
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-06-21 07:07:03.835859 linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/pdfstructure/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/pdfstructure/__init__.py
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-06-21 07:07:03.838835 linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/pdfstructure/analysis/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/pdfstructure/analysis/__init__.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2916 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/pdfstructure/analysis/annotate.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     3691 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/pdfstructure/analysis/sizemapper.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     5496 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/pdfstructure/analysis/styledistribution.py
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-06-21 07:07:03.840279 linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/pdfstructure/hierarchy/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/pdfstructure/hierarchy/__init__.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     1593 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/pdfstructure/hierarchy/detectheader.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2985 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/pdfstructure/hierarchy/headercompare.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     7296 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/pdfstructure/hierarchy/parser.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2608 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/pdfstructure/hierarchy/traversal.py
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-06-21 07:07:03.843472 linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/pdfstructure/model/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/pdfstructure/model/__init__.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     4497 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/pdfstructure/model/document.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2108 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/pdfstructure/model/style.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     4155 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/pdfstructure/printer.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     4983 2023-04-21 06:26:32.000000 linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/pdfstructure/source.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     4253 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/pdfstructure/utils.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     4310 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/skeleton.py
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-06-21 07:07:03.847077 linkedinpdfextractor-1.3.0/src/linkedinpdfextractor.egg-info/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     1350 2023-06-21 07:07:03.000000 linkedinpdfextractor-1.3.0/src/linkedinpdfextractor.egg-info/PKG-INFO
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2574 2023-06-21 07:07:03.000000 linkedinpdfextractor-1.3.0/src/linkedinpdfextractor.egg-info/SOURCES.txt
+-rw-r--r--   0 seshivitakula   (501) staff       (20)        1 2023-06-21 07:07:03.000000 linkedinpdfextractor-1.3.0/src/linkedinpdfextractor.egg-info/dependency_links.txt
+-rw-r--r--   0 seshivitakula   (501) staff       (20)        1 2023-04-21 07:55:27.000000 linkedinpdfextractor-1.3.0/src/linkedinpdfextractor.egg-info/not-zip-safe
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      101 2023-06-21 07:07:03.000000 linkedinpdfextractor-1.3.0/src/linkedinpdfextractor.egg-info/requires.txt
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       23 2023-06-21 07:07:03.000000 linkedinpdfextractor-1.3.0/src/linkedinpdfextractor.egg-info/top_level.txt
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-06-21 07:07:03.853067 linkedinpdfextractor-1.3.0/tests/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     8196 2023-05-05 08:33:17.000000 linkedinpdfextractor-1.3.0/tests/.DS_Store
+-rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.3.0/tests/__init__.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      290 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.3.0/tests/conftest.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      820 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.3.0/tests/helper.py
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-06-21 07:07:03.862357 linkedinpdfextractor-1.3.0/tests/resources/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)   143869 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.3.0/tests/resources/5648.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)   401628 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.3.0/tests/resources/IE00BM67HT60-ATB-FS-DE-2020-2-28.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)    18836 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.3.0/tests/resources/SameSize_BoldTitle.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)    12108 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.3.0/tests/resources/SameSize_EnumeratedTitle.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)    12178 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.3.0/tests/resources/SameStyleOnly.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)    45965 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.3.0/tests/resources/interview_cheatsheet-excerpt.png
+-rwxr-xr-x   0 seshivitakula   (501) staff       (20)   230787 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.3.0/tests/resources/interview_cheatsheet.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)    32674 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.3.0/tests/resources/lorem.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)   383508 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.3.0/tests/resources/paper.pdf
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-06-21 07:07:03.865452 linkedinpdfextractor-1.3.0/tests/resources/parsed/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)   215280 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.3.0/tests/resources/parsed/interview_cheatsheet.json
+-rw-r--r--   0 seshivitakula   (501) staff       (20)    15753 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.3.0/tests/resources/parsed/interview_cheatsheet_pretty.txt
+-rw-r--r--   0 seshivitakula   (501) staff       (20)    62812 2023-04-19 12:12:39.000000 linkedinpdfextractor-1.3.0/tests/resources/profile.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)   251982 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.3.0/tests/resources/samplepptx.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     1398 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.3.0/tests/test_custom_use_cases.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      656 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.3.0/tests/test_document.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2304 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.3.0/tests/test_headercompare.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     4709 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.3.0/tests/test_hierarchy.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      199 2023-05-26 07:31:17.000000 linkedinpdfextractor-1.3.0/tests/test_linkedin_parser.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     3202 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.3.0/tests/test_printer.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      597 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.3.0/tests/test_skeleton.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     4276 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.3.0/tests/test_style_analyser.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     3865 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.3.0/tests/test_traversal.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      804 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.3.0/tests/test_utils.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2690 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.3.0/tox.ini
```

### Comparing `linkedinpdfextractor-1.2.9/.DS_Store` & `linkedinpdfextractor-1.3.0/.DS_Store`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/.gitignore` & `linkedinpdfextractor-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/CONTRIBUTING.rst` & `linkedinpdfextractor-1.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/LICENSE.txt` & `linkedinpdfextractor-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/PKG-INFO` & `linkedinpdfextractor-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkedinpdfextractor
-Version: 1.2.9
+Version: 1.3.0
 Summary: Add a short description here!
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Ketan Prabhu
 Author-email: ketan.prabhu@gigvistas.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `linkedinpdfextractor-1.2.9/README.md` & `linkedinpdfextractor-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/README.rst` & `linkedinpdfextractor-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/docs/Makefile` & `linkedinpdfextractor-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/docs/conf.py` & `linkedinpdfextractor-1.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/docs/index.rst` & `linkedinpdfextractor-1.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/setup.cfg` & `linkedinpdfextractor-1.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/setup.py` & `linkedinpdfextractor-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/src/.DS_Store` & `linkedinpdfextractor-1.3.0/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/.DS_Store` & `linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/.DS_Store`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/__init__.py` & `linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/__init__.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/extractor.py` & `linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/extractor.py`

 * *Files 5% similar despite different names*

```diff
@@ -91,16 +91,16 @@
     return jsonStr
 
 
 def traverse(elements: List[Section], level, parent=None):
     # print(len(elements))
     i=0
     for e in elements:
-        if (e.heading.text == "Summary" or e.heading.text == "Contact" or
-           e.heading.text == "Top Skills" or e.heading.text == "Experience" or e.heading.text == "Education"):
+        if (e.heading.text == "Summary" or e.heading.text == "Contact" or e.heading.text == "Top Skills" or 
+            e.heading.text == "Experience" or e.heading.text == "Education" or e.heading.text == "Certifications" or e.heading.text == "Languages"):
             parent = e.heading.text
         # print(e.heading)
         
         Data.append({"level": level+1, "text": e.heading.text, "type": parent,
                     "mean_size": e.heading.style.mean_size, "max_size": e.heading.style.max_size, "index": i})
         i=i+1
         # print("Level: ", level, element)
@@ -112,37 +112,36 @@
     summary = Summary()
     contact = Contact()
     i = 0
     for index, row in data.iterrows():
         if (row['level'] == 1 and row["mean_size"] == 26.0 and row["max_size"] == 26.0):
             user.name = row["text"]
         elif (row['level'] == 1 and row["mean_size"] == 12.0 and row["max_size"] == 12.0):
-            user.title = ' '.join(map(str, row["text"].split('\n')[0:-1]))
+            user.title = ' '.join(map(str,  decode( row["text"] ).split('\n')[0:-1]))
         elif ((row['level'] == 2 or row['level'] == 3) and 11.8 < row["max_size"] < 12.5 and row["type"] == "Summary"):
-            summary.description.append(row["text"])
+            summary.description.append( decode( row["text"] ).replace("\n", " "))
         elif (row['level'] == 3 and 10.4 < row["max_size"] < 10.6 and row["type"] == "Contact"):
-            contact.description = row["text"]
+            contact.description =  decode( row["text"] )
         elif ((row['level'] == 3 or row['level'] == 1) and 10.4 < row["max_size"] < 10.6 and row["type"] == "Top Skills"):
             user.skills.append(row["text"])
         elif(row["type"] == "Experience"):
-            # if()
             parseExperience(row, user)
         elif (row["type"] == "Education"):
             parseEducation(row, user)
     
     user.summary = ' '.join(map(str, summary.description))
     
     return user
 
 def parseExperience(row, user):
     expLength = len(user.experience)
     exp = Experience() if expLength == 0 else user.experience[expLength-1]
     if (row["max_size"] <= 12.9 and row["max_size"] >= 11.9):
         exp = Experience()
-        expElements = row['text'].split('\n')
+        expElements =  decode( row["text"] ).split('\n')
         if(len(expElements) == 1):
             exp.companyName = expElements[0]
         elif(len(expElements) == 2):
             exp.companyName = expElements[0]
             exp.date = expElements[1].replace('\xa0','')
         elif(len(expElements) == 3):
             exp.companyName = expElements[0]
@@ -151,22 +150,25 @@
         elif(len(expElements) == 4 ):
             exp.companyName = expElements[0]
             exp.position = expElements[1]
             exp.date = expElements[2].replace('\xa0','')
             exp.location = expElements[3]
         user.experience.append(exp)
     elif(row["max_size"] > 9.0 and row["max_size"] < 11.5):
-        user.experience[expLength-1].description += row["text"]
+        user.experience[expLength-1].description += " " + decode( row["text"] )
 
 def parseEducation(row, user):
     eduLength = len(user.education)
     edu = Education() if eduLength == 0 else user.education[eduLength-1]
-    
     if (row["max_size"] <= 12.9 and row["max_size"] >= 11.9):
         edu = Education()
-        edu.university = row['text']
+        edu.university = decode(row["text"])
         user.education.append(edu)
     elif(row["max_size"] < 10.6 and row["max_size"] > 10.2 ):
-        user.education[eduLength-1].course += row["text"]
+        user.education[eduLength-1].course += decode(row["text"])
+
+def decode(str):
+    string_encode = str.encode("ascii", "ignore")
+    return string_encode.decode().strip()
 
-# pdf_to_json("/home/pk/Documents/gig-banking/test_linkdin_package/rashmi.pdf")
-#pdf_to_json("/Users/rishav/Downloads/rashmi_linkedin.pdf")
+# pdf_to_json("/home/pk/Documents/gig-banking/test_linkdin_package/raj.pdf")
+# pdf_to_json("/Users/rishav/Downloads/rashmi_linkedin.pdf")
```

### Comparing `linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/pdfstructure/analysis/annotate.py` & `linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/pdfstructure/analysis/annotate.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/pdfstructure/analysis/sizemapper.py` & `linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/pdfstructure/analysis/sizemapper.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/pdfstructure/analysis/styledistribution.py` & `linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/pdfstructure/analysis/styledistribution.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/pdfstructure/hierarchy/detectheader.py` & `linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/pdfstructure/hierarchy/detectheader.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/pdfstructure/hierarchy/headercompare.py` & `linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/pdfstructure/hierarchy/headercompare.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/pdfstructure/hierarchy/parser.py` & `linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/pdfstructure/hierarchy/parser.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/pdfstructure/hierarchy/traversal.py` & `linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/pdfstructure/hierarchy/traversal.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/pdfstructure/model/document.py` & `linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/pdfstructure/model/document.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/pdfstructure/model/style.py` & `linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/pdfstructure/model/style.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/pdfstructure/printer.py` & `linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/pdfstructure/printer.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/pdfstructure/source.py` & `linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/pdfstructure/source.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/pdfstructure/utils.py` & `linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/pdfstructure/utils.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/src/linkedin_pdf_extractor/skeleton.py` & `linkedinpdfextractor-1.3.0/src/linkedin_pdf_extractor/skeleton.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/src/linkedinpdfextractor.egg-info/PKG-INFO` & `linkedinpdfextractor-1.3.0/src/linkedinpdfextractor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkedinpdfextractor
-Version: 1.2.9
+Version: 1.3.0
 Summary: Add a short description here!
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Ketan Prabhu
 Author-email: ketan.prabhu@gigvistas.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `linkedinpdfextractor-1.2.9/src/linkedinpdfextractor.egg-info/SOURCES.txt` & `linkedinpdfextractor-1.3.0/src/linkedinpdfextractor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/tests/.DS_Store` & `linkedinpdfextractor-1.3.0/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/tests/helper.py` & `linkedinpdfextractor-1.3.0/tests/helper.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/tests/resources/5648.pdf` & `linkedinpdfextractor-1.3.0/tests/resources/5648.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/tests/resources/IE00BM67HT60-ATB-FS-DE-2020-2-28.pdf` & `linkedinpdfextractor-1.3.0/tests/resources/IE00BM67HT60-ATB-FS-DE-2020-2-28.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/tests/resources/SameSize_BoldTitle.pdf` & `linkedinpdfextractor-1.3.0/tests/resources/SameSize_BoldTitle.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/tests/resources/SameSize_EnumeratedTitle.pdf` & `linkedinpdfextractor-1.3.0/tests/resources/SameSize_EnumeratedTitle.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/tests/resources/SameStyleOnly.pdf` & `linkedinpdfextractor-1.3.0/tests/resources/SameStyleOnly.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/tests/resources/interview_cheatsheet-excerpt.png` & `linkedinpdfextractor-1.3.0/tests/resources/interview_cheatsheet-excerpt.png`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/tests/resources/interview_cheatsheet.pdf` & `linkedinpdfextractor-1.3.0/tests/resources/interview_cheatsheet.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/tests/resources/lorem.pdf` & `linkedinpdfextractor-1.3.0/tests/resources/lorem.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/tests/resources/paper.pdf` & `linkedinpdfextractor-1.3.0/tests/resources/paper.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/tests/resources/parsed/interview_cheatsheet.json` & `linkedinpdfextractor-1.3.0/tests/resources/parsed/interview_cheatsheet.json`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/tests/resources/parsed/interview_cheatsheet_pretty.txt` & `linkedinpdfextractor-1.3.0/tests/resources/parsed/interview_cheatsheet_pretty.txt`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/tests/resources/profile.pdf` & `linkedinpdfextractor-1.3.0/tests/resources/profile.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/tests/resources/samplepptx.pdf` & `linkedinpdfextractor-1.3.0/tests/resources/samplepptx.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/tests/test_custom_use_cases.py` & `linkedinpdfextractor-1.3.0/tests/test_custom_use_cases.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/tests/test_document.py` & `linkedinpdfextractor-1.3.0/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/tests/test_headercompare.py` & `linkedinpdfextractor-1.3.0/tests/test_headercompare.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/tests/test_hierarchy.py` & `linkedinpdfextractor-1.3.0/tests/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/tests/test_printer.py` & `linkedinpdfextractor-1.3.0/tests/test_printer.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/tests/test_skeleton.py` & `linkedinpdfextractor-1.3.0/tests/test_skeleton.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/tests/test_style_analyser.py` & `linkedinpdfextractor-1.3.0/tests/test_style_analyser.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/tests/test_traversal.py` & `linkedinpdfextractor-1.3.0/tests/test_traversal.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/tests/test_utils.py` & `linkedinpdfextractor-1.3.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.9/tox.ini` & `linkedinpdfextractor-1.3.0/tox.ini`

 * *Files identical despite different names*

