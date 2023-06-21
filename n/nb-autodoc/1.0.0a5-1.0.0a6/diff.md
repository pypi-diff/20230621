# Comparing `tmp/nb-autodoc-1.0.0a5.tar.gz` & `tmp/nb-autodoc-1.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb-autodoc-1.0.0a5.tar", last modified: Wed Feb  1 17:48:43 2023, max compression
+gzip compressed data, was "nb-autodoc-1.0.0a6.tar", last modified: Wed Jun 21 14:20:57 2023, max compression
```

## Comparing `nb-autodoc-1.0.0a5.tar` & `nb-autodoc-1.0.0a6.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0 iyume     (1000) iyume     (1000)     1064 2021-11-24 06:50:23.530000 nb-autodoc-1.0.0a5/LICENSE
--rw-r--r--   0 iyume     (1000) iyume     (1000)     1064 2023-02-01 13:34:50.380077 nb-autodoc-1.0.0a5/README.md
--rw-r--r--   0 iyume     (1000) iyume     (1000)       86 2023-02-01 17:41:51.554292 nb-autodoc-1.0.0a5/nb_autodoc/__init__.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)     1318 2023-02-01 17:39:46.544340 nb-autodoc-1.0.0a5/nb_autodoc/__main__.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)        0 2023-02-01 10:11:10.514858 nb-autodoc-1.0.0a5/nb_autodoc/analyzers/__init__.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)     2791 2023-02-01 10:11:10.514858 nb-autodoc-1.0.0a5/nb_autodoc/analyzers/analyzer.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)      484 2023-02-01 10:11:10.514858 nb-autodoc-1.0.0a5/nb_autodoc/analyzers/base.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)    12841 2023-02-01 13:16:50.320506 nb-autodoc-1.0.0a5/nb_autodoc/analyzers/definitionfinder.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)     5697 2023-02-01 10:11:10.514858 nb-autodoc-1.0.0a5/nb_autodoc/analyzers/unparse_ann.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)    10475 2023-02-01 13:06:20.800752 nb-autodoc-1.0.0a5/nb_autodoc/analyzers/utils.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)    15029 2023-02-01 11:06:15.663561 nb-autodoc-1.0.0a5/nb_autodoc/annotation.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)     7597 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/nb_autodoc/builders/__init__.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)      406 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/nb_autodoc/builders/helpers.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)    25431 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/nb_autodoc/builders/markdown.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)     2478 2023-02-01 17:08:56.235063 nb-autodoc-1.0.0a5/nb_autodoc/config.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)       83 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/nb_autodoc/docstringparser/__init__.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)    14680 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/nb_autodoc/docstringparser/google.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)     1991 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/nb_autodoc/log.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)    33403 2023-02-01 13:06:35.790746 nb-autodoc-1.0.0a5/nb_autodoc/manager.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)    15796 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/nb_autodoc/modulefinder.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)     4512 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/nb_autodoc/nodes.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)        0 2022-10-10 09:23:09.200000 nb-autodoc-1.0.0a5/nb_autodoc/py.typed
--rw-r--r--   0 iyume     (1000) iyume     (1000)     1396 2023-02-01 11:12:36.513422 nb-autodoc-1.0.0a5/nb_autodoc/typing.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)     8599 2023-02-01 13:15:01.210550 nb-autodoc-1.0.0a5/nb_autodoc/utils.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)     1214 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/pyproject.toml
--rw-r--r--   0 iyume     (1000) iyume     (1000)       29 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/__init__.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)      189 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/analyzerdata/assigndata-override-ast.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)      203 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/analyzerdata/exec_type_checking.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)      169 2023-02-01 12:17:59.641886 nb-autodoc-1.0.0a5/tests/analyzerdata/extract-docstring.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)      380 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/analyzerdata/overload.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)     1286 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/analyzerdata/simple-definition-ast.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)      342 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/analyzerdata/type-checking-ast.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/data/__init__.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)     9335 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/data/example_google_docstring.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)      362 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/data/stuff1.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)      121 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/managerdata/class_bases/__init__.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)       20 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/managerdata/class_bases/base.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)      169 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/managerdata/class_instvar_combination.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/managerdata/class_prepare/__init__.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)      355 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/managerdata/class_prepare/instvar.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)       89 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/managerdata/get_canonical_member/Foo.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)       21 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/managerdata/get_canonical_member/__init__.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)       75 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/managerdata/get_canonical_member/a.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)       27 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/managerdata/get_canonical_member/b.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)       37 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/managerdata/single.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)      217 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/managerdata/variable_is_typealias.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/modulefinderdata/simplepkg/__init__.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/modulefinderdata/simplepkg/foo.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/modulefinderdata/simplepkg/foo.pyi
--rw-r--r--   0 iyume     (1000) iyume     (1000)        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/modulefinderdata/simplepkg/simplenamespace/portion1.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/modulefinderdata/simplepkg/simplenamespace/portion1.pyi
--rw-r--r--   0 iyume     (1000) iyume     (1000)        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/modulefinderdata/simplepkg/simplenamespace/portion2/__init__.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/modulefinderdata/simplepkg/stubalone.pyi
--rw-r--r--   0 iyume     (1000) iyume     (1000)        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/modulefinderdata/simplepkg/sub/__init__.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/modulefinderdata/simplepkg/sub/__init__.pyi
--rw-r--r--   0 iyume     (1000) iyume     (1000)        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/modulefinderdata/simplepkg/sub/a.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/modulefinderdata/simplepkg/sub/a.pyi
--rw-r--r--   0 iyume     (1000) iyume     (1000)        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/modulefinderdata/simplepkg/sub/stubalone.pyi
--rw-r--r--   0 iyume     (1000) iyume     (1000)        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/modulefinderdata/simplepkg/sub.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/modulefinderdata/simplepkg/sub.pyi
--rw-r--r--   0 iyume     (1000) iyume     (1000)     2232 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/simple_pkg/__init__.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)       41 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/simple_pkg/api.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)       66 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/simple_pkg/namespace/foo.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)      132 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/simple_pkg/overload/__init__.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)      630 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/simple_pkg/overload/__init__.pyi
--rw-r--r--   0 iyume     (1000) iyume     (1000)      888 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a5/tests/simple_pkg/overload/nopyi.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)      478 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a5/tests/simple_pkg/overload/relative.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)       80 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a5/tests/simple_pkg/overload/typing.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)       19 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a5/tests/simple_pkg/pyi/__init__.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)      780 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a5/tests/simple_pkg/pyi/fuzz.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)      867 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a5/tests/simple_pkg/pyi/fuzz.pyi
--rw-r--r--   0 iyume     (1000) iyume     (1000)       92 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a5/tests/simple_pkg/pyi/util.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)      458 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a5/tests/simple_pkg/reexport/__init__.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)      757 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a5/tests/simple_pkg/reexport/_sample.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)       34 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a5/tests/simple_pkg/reexport/inter.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)      161 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a5/tests/simple_pkg/typing.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)       33 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a5/tests/test_analyzers/__init__.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)     1606 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a5/tests/test_analyzers/test_analyzer.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)     9140 2023-02-01 12:19:26.981853 nb-autodoc-1.0.0a5/tests/test_analyzers/test_definitionfinder.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)      665 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a5/tests/test_analyzers/test_unparse_ann.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)     2266 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a5/tests/test_analyzers/test_utils.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)     5306 2023-02-01 11:03:36.803631 nb-autodoc-1.0.0a5/tests/test_annotation.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)        0 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a5/tests/test_docstringparser/__init__.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)     5328 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a5/tests/test_docstringparser/test_google.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)     8952 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a5/tests/test_manager.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)     2102 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a5/tests/test_modulefinder.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)     6607 2023-02-01 11:26:22.073091 nb-autodoc-1.0.0a5/tests/test_utils.py
--rw-r--r--   0 iyume     (1000) iyume     (1000)      738 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a5/tests/utils.py
--rw-------   0 iyume     (1000) iyume     (1000)     1484 2023-02-01 17:48:43.114128 nb-autodoc-1.0.0a5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2021-11-24 06:50:23.530000 nb-autodoc-1.0.0a6/LICENSE
+-rw-r--r--   0        0        0     1743 2023-02-02 07:55:37.114382 nb-autodoc-1.0.0a6/README.md
+-rw-r--r--   0        0        0       86 2023-06-21 14:18:00.713881 nb-autodoc-1.0.0a6/nb_autodoc/__init__.py
+-rw-r--r--   0        0        0     1318 2023-02-02 07:55:37.114382 nb-autodoc-1.0.0a6/nb_autodoc/__main__.py
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.514858 nb-autodoc-1.0.0a6/nb_autodoc/analyzers/__init__.py
+-rw-r--r--   0        0        0     2791 2023-02-01 10:11:10.514858 nb-autodoc-1.0.0a6/nb_autodoc/analyzers/analyzer.py
+-rw-r--r--   0        0        0      484 2023-02-01 10:11:10.514858 nb-autodoc-1.0.0a6/nb_autodoc/analyzers/base.py
+-rw-r--r--   0        0        0    12841 2023-02-02 07:55:37.114382 nb-autodoc-1.0.0a6/nb_autodoc/analyzers/definitionfinder.py
+-rw-r--r--   0        0        0     5697 2023-02-01 10:11:10.514858 nb-autodoc-1.0.0a6/nb_autodoc/analyzers/unparse_ann.py
+-rw-r--r--   0        0        0    10475 2023-02-02 07:55:37.114382 nb-autodoc-1.0.0a6/nb_autodoc/analyzers/utils.py
+-rw-r--r--   0        0        0    15331 2023-03-22 10:11:28.688069 nb-autodoc-1.0.0a6/nb_autodoc/annotation.py
+-rw-r--r--   0        0        0     7597 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/nb_autodoc/builders/__init__.py
+-rw-r--r--   0        0        0      406 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/nb_autodoc/builders/helpers.py
+-rw-r--r--   0        0        0    26266 2023-05-05 09:04:38.574920 nb-autodoc-1.0.0a6/nb_autodoc/builders/markdown.py
+-rw-r--r--   0        0        0     2478 2023-02-02 07:55:37.124382 nb-autodoc-1.0.0a6/nb_autodoc/config.py
+-rw-r--r--   0        0        0       83 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/nb_autodoc/docstringparser/__init__.py
+-rw-r--r--   0        0        0    15112 2023-06-21 14:14:36.863882 nb-autodoc-1.0.0a6/nb_autodoc/docstringparser/google.py
+-rw-r--r--   0        0        0     1991 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/nb_autodoc/log.py
+-rw-r--r--   0        0        0    33670 2023-05-05 09:07:44.174879 nb-autodoc-1.0.0a6/nb_autodoc/manager.py
+-rw-r--r--   0        0        0    15796 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/nb_autodoc/modulefinder.py
+-rw-r--r--   0        0        0     4512 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/nb_autodoc/nodes.py
+-rw-r--r--   0        0        0        0 2022-10-10 09:23:09.200000 nb-autodoc-1.0.0a6/nb_autodoc/py.typed
+-rw-r--r--   0        0        0     1396 2023-02-02 07:55:37.124382 nb-autodoc-1.0.0a6/nb_autodoc/typing.py
+-rw-r--r--   0        0        0     8599 2023-03-22 10:06:52.428169 nb-autodoc-1.0.0a6/nb_autodoc/utils.py
+-rw-r--r--   0        0        0     1228 2023-03-22 08:53:54.029767 nb-autodoc-1.0.0a6/pyproject.toml
+-rw-r--r--   0        0        0       29 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/__init__.py
+-rw-r--r--   0        0        0      189 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/analyzerdata/assigndata-override-ast.py
+-rw-r--r--   0        0        0      203 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/analyzerdata/exec_type_checking.py
+-rw-r--r--   0        0        0      169 2023-02-02 07:55:37.124382 nb-autodoc-1.0.0a6/tests/analyzerdata/extract-docstring.py
+-rw-r--r--   0        0        0      380 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/analyzerdata/overload.py
+-rw-r--r--   0        0        0     1286 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/analyzerdata/simple-definition-ast.py
+-rw-r--r--   0        0        0      342 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/analyzerdata/type-checking-ast.py
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/data/__init__.py
+-rw-r--r--   0        0        0     9335 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/data/example_google_docstring.py
+-rw-r--r--   0        0        0      362 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/data/stuff1.py
+-rw-r--r--   0        0        0      121 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/managerdata/class_bases/__init__.py
+-rw-r--r--   0        0        0       20 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/managerdata/class_bases/base.py
+-rw-r--r--   0        0        0      169 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/managerdata/class_instvar_combination.py
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/managerdata/class_prepare/__init__.py
+-rw-r--r--   0        0        0      355 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/managerdata/class_prepare/instvar.py
+-rw-r--r--   0        0        0       89 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/managerdata/get_canonical_member/Foo.py
+-rw-r--r--   0        0        0       21 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/managerdata/get_canonical_member/__init__.py
+-rw-r--r--   0        0        0       75 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/managerdata/get_canonical_member/a.py
+-rw-r--r--   0        0        0       27 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/managerdata/get_canonical_member/b.py
+-rw-r--r--   0        0        0       37 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/managerdata/single.py
+-rw-r--r--   0        0        0      217 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/managerdata/variable_is_typealias.py
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/modulefinderdata/simplepkg/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/modulefinderdata/simplepkg/foo.py
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/modulefinderdata/simplepkg/foo.pyi
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/modulefinderdata/simplepkg/simplenamespace/portion1.py
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/modulefinderdata/simplepkg/simplenamespace/portion1.pyi
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/modulefinderdata/simplepkg/simplenamespace/portion2/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/modulefinderdata/simplepkg/stubalone.pyi
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/modulefinderdata/simplepkg/sub/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/modulefinderdata/simplepkg/sub/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/modulefinderdata/simplepkg/sub/a.py
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/modulefinderdata/simplepkg/sub/a.pyi
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/modulefinderdata/simplepkg/sub/stubalone.pyi
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/modulefinderdata/simplepkg/sub.py
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/modulefinderdata/simplepkg/sub.pyi
+-rw-r--r--   0        0        0     2232 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/simple_pkg/__init__.py
+-rw-r--r--   0        0        0       41 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/simple_pkg/api.py
+-rw-r--r--   0        0        0       66 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/simple_pkg/namespace/foo.py
+-rw-r--r--   0        0        0      132 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/simple_pkg/overload/__init__.py
+-rw-r--r--   0        0        0      630 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/simple_pkg/overload/__init__.pyi
+-rw-r--r--   0        0        0      888 2023-02-01 10:11:10.524858 nb-autodoc-1.0.0a6/tests/simple_pkg/overload/nopyi.py
+-rw-r--r--   0        0        0      478 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/simple_pkg/overload/relative.py
+-rw-r--r--   0        0        0       80 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/simple_pkg/overload/typing.py
+-rw-r--r--   0        0        0       19 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/simple_pkg/pyi/__init__.py
+-rw-r--r--   0        0        0      780 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/simple_pkg/pyi/fuzz.py
+-rw-r--r--   0        0        0      867 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/simple_pkg/pyi/fuzz.pyi
+-rw-r--r--   0        0        0       92 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/simple_pkg/pyi/util.py
+-rw-r--r--   0        0        0      458 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/simple_pkg/reexport/__init__.py
+-rw-r--r--   0        0        0      757 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/simple_pkg/reexport/_sample.py
+-rw-r--r--   0        0        0       34 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/simple_pkg/reexport/inter.py
+-rw-r--r--   0        0        0      161 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/simple_pkg/typing.py
+-rw-r--r--   0        0        0       33 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/test_analyzers/__init__.py
+-rw-r--r--   0        0        0     1606 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/test_analyzers/test_analyzer.py
+-rw-r--r--   0        0        0     9140 2023-02-02 07:55:37.124382 nb-autodoc-1.0.0a6/tests/test_analyzers/test_definitionfinder.py
+-rw-r--r--   0        0        0      665 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/test_analyzers/test_unparse_ann.py
+-rw-r--r--   0        0        0     2266 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/test_analyzers/test_utils.py
+-rw-r--r--   0        0        0     5306 2023-02-04 07:42:44.759251 nb-autodoc-1.0.0a6/tests/test_annotation.py
+-rw-r--r--   0        0        0        0 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/test_docstringparser/__init__.py
+-rw-r--r--   0        0        0     5330 2023-06-21 14:08:14.903902 nb-autodoc-1.0.0a6/tests/test_docstringparser/test_google.py
+-rw-r--r--   0        0        0     8952 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/test_manager.py
+-rw-r--r--   0        0        0     2102 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/test_modulefinder.py
+-rw-r--r--   0        0        0     6607 2023-02-02 07:55:37.124382 nb-autodoc-1.0.0a6/tests/test_utils.py
+-rw-r--r--   0        0        0      738 2023-02-01 10:11:10.534858 nb-autodoc-1.0.0a6/tests/utils.py
+-rw-r--r--   0        0        0     2191 1970-01-01 00:00:00.000000 nb-autodoc-1.0.0a6/PKG-INFO
```

### Comparing `nb-autodoc-1.0.0a5/LICENSE` & `nb-autodoc-1.0.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a5/nb_autodoc/__main__.py` & `nb-autodoc-1.0.0a6/nb_autodoc/__main__.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a5/nb_autodoc/analyzers/analyzer.py` & `nb-autodoc-1.0.0a6/nb_autodoc/analyzers/analyzer.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a5/nb_autodoc/analyzers/definitionfinder.py` & `nb-autodoc-1.0.0a6/nb_autodoc/analyzers/definitionfinder.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a5/nb_autodoc/analyzers/unparse_ann.py` & `nb-autodoc-1.0.0a6/nb_autodoc/analyzers/unparse_ann.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a5/nb_autodoc/analyzers/utils.py` & `nb-autodoc-1.0.0a6/nb_autodoc/analyzers/utils.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a5/nb_autodoc/annotation.py` & `nb-autodoc-1.0.0a6/nb_autodoc/annotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,18 +294,21 @@
 
     def __init__(
         self,
         *,
         globalns: dict[str, T_Definition] = frozendict(),
         add_link: t.Callable[[T_Definition], str] = _add_link_empty,
         eval_refname: t.Callable[[str], t.Optional[T_Definition]] = lambda x: None,
+        escape_impl: t.Callable[[str], str] = lambda x: x,
     ) -> None:
         self.globalns = globalns
         self.add_link = add_link
         self.eval_refname = eval_refname
+        # escape for name contains md chars; or Literal string
+        self.escape_impl = escape_impl
         self._builder: list[str] = []
 
     def write(self, s: str) -> None:
         self._builder.append(s)
 
     @contextmanager
     def delimit(self, start: str, end: str) -> t.Generator[None, None, None]:
@@ -338,15 +341,15 @@
 
     def visit_Name(self, annexpr: Name) -> None:
         name = annexpr.name
         dobj = self.globalns.get(name) or self.eval_refname(name)
         if dobj:
             self.write(self.add_link(dobj))
         else:
-            self.write(name)
+            self.write(self.escape_impl(name))
 
     def visit_TypingName(self, annexpr: TypingName) -> None:
         if annexpr.tp_name in _py310_ga_tpname:
             self.write(annexpr.tp_name.lower())
         else:
             self.write(annexpr.tp_name)
 
@@ -355,15 +358,15 @@
 
     def visit_Literal(self, annexpr: Literal) -> None:
         with self.delimit("Literal[", "]"):
             interleave(
                 lambda: self.write(", "),
                 lambda arg: self.visit_Name(arg)
                 if isinstance(arg, Name)
-                else self.write(repr(arg)),
+                else self.write(self.escape_impl(repr(arg))),
                 annexpr.args,
             )
 
     def visit_Annotated(self, annexpr: Annotated) -> None:
         self.visit(annexpr.origin)
 
     def visit_GASubscript(self, annexpr: GASubscript) -> None:
@@ -427,21 +430,26 @@
 
     @property
     def is_classvar(self) -> bool:
         if isinstance(self.ann, _annexpr):
             return _ga_subst_outer_check(self.ann, "ClassVar")
         return False
 
-    def get_doc_linkify(self, add_link: t.Callable[[T_Definition], str]) -> str:
+    def get_doc_linkify(
+        self,
+        add_link: t.Callable[[T_Definition], str],
+        escape_impl: t.Callable[[str], str],
+    ) -> str:
         return AnnExprVisitor(
             globalns=self.globalns,
             add_link=add_link,
             eval_refname=self.manager.get_definition_dotted
             if self.manager
             else lambda x: None,
+            escape_impl=escape_impl,
         ).render(self.ann)
 
     def __str__(self) -> str:
         return _type_str(self.ann)
 
     # @property
     # def is_callable(self) -> bool:
```

### Comparing `nb-autodoc-1.0.0a5/nb_autodoc/builders/__init__.py` & `nb-autodoc-1.0.0a6/nb_autodoc/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a5/nb_autodoc/builders/markdown.py` & `nb-autodoc-1.0.0a6/nb_autodoc/builders/markdown.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,27 @@
 from .helpers import vuepress_slugify
 
 _descr_role_re = re.compile(
     r"{(?P<name>\w+?)}`(?:(?P<text>[^{}]+?) <)?(?P<content>[\w\.\+\-]+)(?(text)>)`"
 )
 
 
+def escape_md_chars(s: str) -> str:
+    return (
+        s.replace("*", r"\*")
+        .replace("#", r"\#")
+        .replace("(", r"\(")
+        .replace(")", r"\)")
+        .replace("<", r"\<")
+        .replace(">", r"\>")
+        .replace("_", r"\_")
+        .replace("`", r"\`")
+    )
+
+
 # renderer utils
 def _find_kind_from_roles(roles: List[nodes.Role]) -> Optional[str]:
     for role in roles:
         if role.name == "kind":
             return role.content
 
 
@@ -238,22 +251,29 @@
         if version:
             self.write(" ")
             self.write(get_version_badge(version))
         if self.add_heading_id:
             self.write(f" {{#{heading_id_slugify_impl(dobj)}}}")
 
     def add_link(
-        self, dobj: T_Definition, *, warn_notfound: str = "", text: Optional[str] = None
+        self,
+        dobj: T_Definition,
+        *,
+        warn_notfound: str = "",
+        text: Optional[str] = None,
+        autoescape: bool = True,
     ) -> str:
         modulename, anchor = self.builder.get_anchor_ref(dobj)
         if not anchor:
             if warn_notfound:
                 logger.warning(warn_notfound)
             return dobj.qualname
         text = text or dobj.qualname
+        if autoescape:
+            text = escape_md_chars(text)
         if modulename == self.current_module.name:
             return f"[{text}](#{anchor})"
         path = self.builder.paths[modulename]
         current_path = self.builder.paths[self.current_module.name]
         relpath = calculate_relpath(path, current_path.parent)
         return f"[{text}]({relpath}#{anchor})"
 
@@ -272,14 +292,15 @@
                 dobj = manager.get_definition_dotted(content)
             if dobj:
                 return self.add_link(
                     dobj,
                     warn_notfound=f"ref {matchtext!r} found {dobj.fullname!r} "
                     "which is unlinkable",
                     text=text,
+                    autoescape=False,
                 )
             else:
                 logger.warning(f"ref {matchtext!r} is not a member")
         else:
             logger.warning(f"role {matchtext!r} is invalid")
         return text or content
 
@@ -312,17 +333,19 @@
                 if doc_args_dict:
                     doc_arg = doc_args_dict.get(p.name)
                 annotation = None
                 # doc overridden annotation or parameter annotation
                 if doc_arg and doc_arg.annotation:
                     annotation = bind_module.build_static_ann(
                         ast.parse(doc_arg.annotation, mode="eval").body
-                    ).get_doc_linkify(self.add_link)
+                    ).get_doc_linkify(self.add_link, escape_md_chars)
                 elif p.annotation is not Parameter.empty:
-                    annotation = p.annotation.get_doc_linkify(self.add_link)
+                    annotation = p.annotation.get_doc_linkify(
+                        self.add_link, escape_md_chars
+                    )
                 arg = nodes.ColonArg(p.name, annotation, [], "", "")
                 if doc_arg:
                     arg.descr = doc_arg.descr
                     arg.long_descr = doc_arg.long_descr
                 if p.kind in (
                     Parameter.POSITIONAL_ONLY,
                     Parameter.POSITIONAL_OR_KEYWORD,
@@ -341,15 +364,15 @@
                 if sig and name in sig.parameters:  # keep order
                     continue
                 doc_arg = doc_args_dict[name]
                 annotation = None
                 if doc_arg.annotation:
                     annotation = bind_module.build_static_ann(
                         ast.parse(doc_arg.annotation, mode="eval").body
-                    ).get_doc_linkify(self.add_link)
+                    ).get_doc_linkify(self.add_link, escape_md_chars)
                 new_args.kwonlyargs.append(
                     nodes.ColonArg(
                         name, annotation, [], doc_arg.descr, doc_arg.long_descr
                     )
                 )
         return new_args
 
@@ -366,25 +389,27 @@
         new_rets.value = nodes.ColonArg(None, None, [], "", "")
         annotation = None
         if rets:
             if isinstance(rets.value, nodes.ColonArg):
                 assert rets.value.annotation, "Returns ColonArg annotation must be str"
                 annotation = bind_module.build_static_ann(
                     ast.parse(rets.value.annotation, mode="eval").body
-                ).get_doc_linkify(self.add_link)
+                ).get_doc_linkify(self.add_link, escape_md_chars)
                 descr = rets.value.descr
                 long_descr = rets.value.long_descr
             else:
                 descr, _, long_descr = rets.value.partition("\n")  # type: ignore  # mypy
                 descr = descr.strip()
                 long_descr = long_descr.strip()
             new_rets.value.descr = descr
             new_rets.value.long_descr = long_descr
         if annotation is None and sig and sig.return_annotation is not Parameter.empty:
-            annotation = sig.return_annotation.get_doc_linkify(self.add_link)
+            annotation = sig.return_annotation.get_doc_linkify(
+                self.add_link, escape_md_chars
+            )
         elif annotation is None:
             annotation = "untyped"
         new_rets.value.annotation = annotation
         return new_rets
 
     def _resolve_doc_from_sig(self, dobj: Union[Function, Class]) -> None:
         if not dobj.doctree:
@@ -459,22 +484,25 @@
         self.title(dobj)
         _extract_inlinevalue(dobj.doctree)
         self.newline()
         self.visit_Docstring(dobj.doctree)
 
     def visit_Variable(self, dobj: Variable) -> None:
         self.title(dobj)
-        self.newline("- **类型:**")
+        self.newline("- **类型:** ")
         if dobj.annotation:
-            self.write(" ")
-            self.write(dobj.annotation.get_doc_linkify(self.add_link))
+            self.write(dobj.annotation.get_doc_linkify(self.add_link, escape_md_chars))
         elif dobj.doctree and dobj.doctree.annotation:
-            dobj.module.build_static_ann(
-                ast.parse(dobj.doctree.annotation, mode="eval").body
-            ).get_doc_linkify(self.add_link)
+            self.write(
+                dobj.module.build_static_ann(
+                    ast.parse(dobj.doctree.annotation, mode="eval").body
+                ).get_doc_linkify(self.add_link, escape_md_chars)
+            )
+        else:
+            self.write("untyped")
         inlinevalue = {}
         if dobj.doctree:
             inlinevalue = _extract_inlinevalue(dobj.doctree)
         if inlinevalue.get("typeversion"):
             self.write(" ")
             self.write(get_version_badge(inlinevalue["typeversion"]))
         if dobj.doctree:
@@ -571,15 +599,15 @@
         isvar: bool = False,
         iskw: bool = False,
         link_ann: bool = False,
     ) -> None:
         if link_ann and dsobj.annotation:
             dsobj.annotation = self.current_module.build_static_ann(
                 ast.parse(dsobj.annotation, mode="eval").body
-            ).get_doc_linkify(self.add_link)
+            ).get_doc_linkify(self.add_link, escape_md_chars)
         self.fill("- ")
         if dsobj.name:
             with self.delimit("`", "`"):
                 if isvar:
                     self.write("*")
                 if iskw:
                     self.write("**")
@@ -685,16 +713,17 @@
             self.write(get_version_badge(dsobj.version))
         with self.block():
             self.newline(dsobj.value)
 
 
 def heading_id_slugify_impl(dobj: T_Definition) -> str:
     # EnumMember is unlinkable and expect None, but we skipped
-    return dobj.qualname.replace(".", "-")
-    # return dobj.qualname  # docusauras cannot recognize "."
+    # replace . because docusaurus 2.0.0 not support (2.3.0 work)
+    # replace _ for: https://github.com/facebook/docusaurus/issues/8617
+    return dobj.qualname.replace(".", "-").replace("_", "-")
 
 
 def vuepress_slugify_impl(dobj: T_Definition) -> Optional[str]:
     title = get_bare_title(dobj)
     if title is None:
         return None
     return vuepress_slugify(title)
```

### Comparing `nb-autodoc-1.0.0a5/nb_autodoc/config.py` & `nb-autodoc-1.0.0a6/nb_autodoc/config.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a5/nb_autodoc/docstringparser/google.py` & `nb-autodoc-1.0.0a6/nb_autodoc/docstringparser/google.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,19 +370,27 @@
             # have description before first section
             match = self._firstline_re.match(self.line)
             if match:
                 annotation, descr = match.groups()
                 descr = descr.strip()
             else:
                 descr = self.line.strip()
-            self.lineno += 1
-            self.col = 0  # descr may behind roles, so set to zero
-            descr_chunk = self.lines[self.lineno : partition_lineno]
-            self.lineno += len(descr_chunk)  # maybe zero
-            long_descr = "\n".join(descr_chunk).strip()
+            # collect long descr if there has any rest content
+            if self.lineno < len(self.lines) - 1:
+                self.lineno += 1
+                self.col = 0  # descr may behind roles, so set to zero
+                # join following text line into short descr
+                while (l := self.line.strip()) and (
+                    partition_lineno is None or self.lineno < partition_lineno
+                ):
+                    self.lineno += 1
+                    descr = f"{descr} {l.strip()}"
+                descr_chunk = self.lines[self.lineno : partition_lineno]
+                self.lineno += len(descr_chunk)  # maybe zero
+                long_descr = "\n".join(descr_chunk).strip()
         sections = []
         text_chunk: list[str] = []
 
         def save_text_chunk_if() -> None:
             if text_chunk:
                 text = "\n".join(text_chunk).strip()
                 if text:
```

### Comparing `nb-autodoc-1.0.0a5/nb_autodoc/log.py` & `nb-autodoc-1.0.0a6/nb_autodoc/log.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a5/nb_autodoc/manager.py` & `nb-autodoc-1.0.0a6/nb_autodoc/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations as _
 
 import ast
 import dataclasses
 from inspect import Parameter, Signature, getsource, unwrap
 from types import FunctionType, MappingProxyType, ModuleType
 from typing import Any, Dict, NamedTuple, TypeVar, cast
+from typing_extensions import TypeAlias
 
 from nb_autodoc.analyzers.analyzer import Analyzer
 from nb_autodoc.analyzers.definitionfinder import (
     AssignData,
     ClassDefData,
     FunctionDefData,
     ImportFromData,
@@ -672,15 +673,15 @@
     like `{module: {qualname: {firstlineno: func}}}`, so stub evaluation will cover
     the potential overloads. We do not take care of this implementation.
     """
 
     def __init__(
         self,
         name: str,
-        pyobj: FunctionType | staticmethod[Any] | classmethod[Any],
+        pyobj: FunctionType | staticmethod[Any, Any] | classmethod[Any, Any, Any],
         astobj: FunctionDefData | None,
         *,
         module: Module,
         cls: Class | None = None,
         assign_doc: str | None = None,
     ) -> None:
         self.name = name
@@ -731,25 +732,29 @@
         sig = Function._get_signature(self.func, self.module.manager.modules)
         if sig and self.cls and isinstance(self.pyobj, (FunctionType, classmethod)):
             return _skip_signature_bound_arg(sig)
         return sig
 
     @cached_property
     def overloads(self) -> list[tuple[FunctionSignature, Docstring | None]] | None:
-        overloads = None
+        overloads: list[tuple[FunctionSignature, Docstring | None]] | None = None
         if isinstance(self.astobj, FunctionDefData) and self.astobj.overloads:
             overloads = []
             for overload in self.astobj.overloads:
                 doc = overload.docstring and cleandoc(overload.docstring)
                 overloads.append(
                     (
                         self.module._transform_ast_signature(overload.signature),
                         self.module.manager.parse_doc(doc) if doc else None,
                     )
                 )
+        if overloads and self.cls:
+            overloads = [
+                (_skip_signature_bound_arg(sig), doc) for sig, doc in overloads
+            ]
         return overloads
 
     @staticmethod
     def _get_signature(
         obj: Any, modules: dict[str, Module]
     ) -> FunctionSignature | None:
         func = get_signable_func(obj)
```

### Comparing `nb-autodoc-1.0.0a5/nb_autodoc/modulefinder.py` & `nb-autodoc-1.0.0a6/nb_autodoc/modulefinder.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a5/nb_autodoc/nodes.py` & `nb-autodoc-1.0.0a6/nb_autodoc/nodes.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a5/nb_autodoc/typing.py` & `nb-autodoc-1.0.0a6/nb_autodoc/typing.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a5/nb_autodoc/utils.py` & `nb-autodoc-1.0.0a6/nb_autodoc/utils.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a5/pyproject.toml` & `nb-autodoc-1.0.0a6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 [project]
 name = "nb-autodoc"
-description = "Powerful API Documentation Generator."
+description = "Python API documentation tool supporting the modern PEPs and typing features."
 authors = [
     { name = "iyume", email = "iyumelive@gmail.com" },
 ]
 requires-python = ">=3.8"
 dynamic = []
 readme = "README.md"
 keywords = [
     "nonebot",
     "autodoc",
-    "ast",
-    "inspect",
     "apidoc",
     "documentation-tool",
     "markdown",
 ]
 dependencies = [
     "typing-extensions>=4.0",
     "click==8.*",
 ]
-version = "1.0.0a5"
+version = "1.0.0a6"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 
 [project.urls]
```

### Comparing `nb-autodoc-1.0.0a5/tests/analyzerdata/simple-definition-ast.py` & `nb-autodoc-1.0.0a6/tests/analyzerdata/simple-definition-ast.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a5/tests/data/example_google_docstring.py` & `nb-autodoc-1.0.0a6/tests/data/example_google_docstring.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a5/tests/simple_pkg/__init__.py` & `nb-autodoc-1.0.0a6/tests/simple_pkg/__init__.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a5/tests/simple_pkg/overload/__init__.pyi` & `nb-autodoc-1.0.0a6/tests/simple_pkg/overload/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a5/tests/simple_pkg/overload/nopyi.py` & `nb-autodoc-1.0.0a6/tests/simple_pkg/overload/nopyi.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a5/tests/simple_pkg/pyi/fuzz.py` & `nb-autodoc-1.0.0a6/tests/simple_pkg/pyi/fuzz.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a5/tests/simple_pkg/pyi/fuzz.pyi` & `nb-autodoc-1.0.0a6/tests/simple_pkg/pyi/fuzz.pyi`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a5/tests/simple_pkg/reexport/_sample.py` & `nb-autodoc-1.0.0a6/tests/simple_pkg/reexport/_sample.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a5/tests/test_analyzers/test_analyzer.py` & `nb-autodoc-1.0.0a6/tests/test_analyzers/test_analyzer.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a5/tests/test_analyzers/test_definitionfinder.py` & `nb-autodoc-1.0.0a6/tests/test_analyzers/test_definitionfinder.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a5/tests/test_analyzers/test_unparse_ann.py` & `nb-autodoc-1.0.0a6/tests/test_analyzers/test_unparse_ann.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a5/tests/test_analyzers/test_utils.py` & `nb-autodoc-1.0.0a6/tests/test_analyzers/test_utils.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a5/tests/test_annotation.py` & `nb-autodoc-1.0.0a6/tests/test_annotation.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a5/tests/test_docstringparser/test_google.py` & `nb-autodoc-1.0.0a6/tests/test_docstringparser/test_google.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
             descr="description",
             long_descr="",
             sections=[],
         )
         assert parse("int: descr\nlong descr") == Docstring(
             roles=[],
             annotation="int",
-            descr="descr",
-            long_descr="long descr",
+            descr="descr long descr",
+            long_descr="",
             sections=[],
         )
         assert parse("{ver}`1.1.0+` descr") == Docstring(
             roles=[Role("ver", None, "1.1.0+")],
             annotation=None,
             descr="descr",
             long_descr="",
@@ -46,16 +46,16 @@
             descr="descr",
             long_descr="",
             sections=[],
         )
         assert parse("{ver}`1.1.0+` Union[int, str]: descr\nlong descr") == Docstring(
             roles=[Role("ver", None, "1.1.0+")],
             annotation="Union[int, str]",
-            descr="descr",
-            long_descr="long descr",
+            descr="descr long descr",
+            long_descr="",
             sections=[],
         )
         assert parse(
             "{ver}`1.1.0+` Union[int, str]: descr\n\nlong descr\n\nlong long descr"
         ) == Docstring(
             roles=[Role("ver", None, "1.1.0+")],
             annotation="Union[int, str]",
```

### Comparing `nb-autodoc-1.0.0a5/tests/test_manager.py` & `nb-autodoc-1.0.0a6/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a5/tests/test_modulefinder.py` & `nb-autodoc-1.0.0a6/tests/test_modulefinder.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a5/tests/test_utils.py` & `nb-autodoc-1.0.0a6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `nb-autodoc-1.0.0a5/tests/utils.py` & `nb-autodoc-1.0.0a6/tests/utils.py`

 * *Files identical despite different names*

