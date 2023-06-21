# Comparing `tmp/pyoptgra-0.1.8.tar.gz` & `tmp/pyoptgra-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoptgra-0.1.8.tar", last modified: Fri Feb 10 14:11:36 2023, max compression
+gzip compressed data, was "pyoptgra-0.1.9.tar", last modified: Wed Jun 21 13:32:53 2023, max compression
```

## Comparing `pyoptgra-0.1.8.tar` & `pyoptgra-0.1.9.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 14:11:36.280259 pyoptgra-0.1.8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 14:11:36.266257 pyoptgra-0.1.8/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 14:11:36.269258 pyoptgra-0.1.8/.github/workflows/
--rw-rw-rw-   0 root         (0) root         (0)      689 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/.github/workflows/deployment.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2461 2023-02-10 14:10:37.000000 pyoptgra-0.1.8/.github/workflows/workflow.yaml
--rw-rw-rw-   0 root         (0) root         (0)      205 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     4106 2023-02-10 14:10:37.000000 pyoptgra-0.1.8/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/.gitmodules
--rw-rw-rw-   0 root         (0) root         (0)     3989 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)    17060 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/ESA Software Community Licence Weak Copyleft - v2.4
--rw-rw-rw-   0 root         (0) root         (0)    35150 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/GNU GENERAL PUBLIC LICENSE 3
--rw-rw-rw-   0 root         (0) root         (0)      615 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/LEGAL
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2423 2023-02-10 14:11:36.280259 pyoptgra-0.1.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2073 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 14:11:36.269258 pyoptgra-0.1.8/ThirdPartyLicenses/
--rw-rw-rw-   0 root         (0) root         (0)     1338 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/ThirdPartyLicenses/CATCH2_LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)     5366 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/ThirdPartyLicenses/CMAKE_LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)     1676 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/ThirdPartyLicenses/PYBIND11_LICENSE.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 14:11:36.266257 pyoptgra-0.1.8/cmake/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 14:11:36.270258 pyoptgra-0.1.8/cmake/modules/
--rw-rw-rw-   0 root         (0) root         (0)      526 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/cmake/modules/Pybind11.cmake
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/cmake/modules/Update_submodules.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 14:11:36.266257 pyoptgra-0.1.8/doc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 14:11:36.270258 pyoptgra-0.1.8/doc/doxygen/
--rw-rw-rw-   0 root         (0) root         (0)   112588 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/doc/doxygen/Doxyfile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 14:11:36.271258 pyoptgra-0.1.8/doc/sphinx/
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/doc/sphinx/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 14:11:36.271258 pyoptgra-0.1.8/doc/sphinx/_static/
--rw-rw-rw-   0 root         (0) root         (0)   423563 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/doc/sphinx/_static/Earth_Mars_SEP_Pyoptgra.html
--rw-rw-rw-   0 root         (0) root         (0)      729 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/doc/sphinx/api.rst
--rw-rw-rw-   0 root         (0) root         (0)     4523 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/doc/sphinx/changes-from-fortran.rst
--rw-rw-rw-   0 root         (0) root         (0)     2324 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/doc/sphinx/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      122 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/doc/sphinx/example-notebook.rst
--rw-rw-rw-   0 root         (0) root         (0)     1210 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/doc/sphinx/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1843 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/doc/sphinx/scaling-and-tolerances.rst
--rw-rw-rw-   0 root         (0) root         (0)     5792 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/doc/sphinx/sensitivity.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 14:11:36.272258 pyoptgra-0.1.8/pyoptgra/
--rw-rw-rw-   0 root         (0) root         (0)      899 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/_about.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 14:11:36.279259 pyoptgra-0.1.8/pyoptgra/core/
--rw-rw-rw-   0 root         (0) root         (0)      858 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4232 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/bindings.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1865 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/mul2m.F
--rw-rw-rw-   0 root         (0) root         (0)      820 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/mulvs.F
--rw-rw-rw-   0 root         (0) root         (0)     1106 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/ogcdel.F
--rw-rw-rw-   0 root         (0) root         (0)     2095 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/ogclos.F
--rw-rw-rw-   0 root         (0) root         (0)    27579 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/ogcorr.F
--rw-rw-rw-   0 root         (0) root         (0)     1123 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/ogcpri.F
--rw-rw-rw-   0 root         (0) root         (0)     1193 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/ogcsca.F
--rw-rw-rw-   0 root         (0) root         (0)     1327 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/ogcstr.F
--rw-rw-rw-   0 root         (0) root         (0)     1270 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/ogctyp.F
--rw-rw-rw-   0 root         (0) root         (0)     5244 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/ogdata.inc
--rw-rw-rw-   0 root         (0) root         (0)     1605 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/ogderi.F
--rw-rw-rw-   0 root         (0) root         (0)     1389 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/ogdist.F
--rw-rw-rw-   0 root         (0) root         (0)    14266 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/ogeval.F
--rw-rw-rw-   0 root         (0) root         (0)     3023 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/ogexcl.F
--rw-rw-rw-   0 root         (0) root         (0)    17620 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/ogexec.F
--rw-rw-rw-   0 root         (0) root         (0)     3124 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/oggsst.F
--rw-rw-rw-   0 root         (0) root         (0)     4721 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/ogincl.F
--rw-rw-rw-   0 root         (0) root         (0)     5674 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/oginit.F
--rw-rw-rw-   0 root         (0) root         (0)     1757 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/ogiter.F
--rw-rw-rw-   0 root         (0) root         (0)     1584 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/ogleft.F
--rw-rw-rw-   0 root         (0) root         (0)     1174 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/ogomet.F
--rw-rw-rw-   0 root         (0) root         (0)    31825 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/ogopti.F
--rw-rw-rw-   0 root         (0) root         (0)     1615 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/ogplog.F
--rw-rw-rw-   0 root         (0) root         (0)     2659 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/ogpwri.F
--rw-rw-rw-   0 root         (0) root         (0)     2250 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/ogpwri_end.F
--rw-rw-rw-   0 root         (0) root         (0)     2306 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/ogpwri_start.F
--rw-rw-rw-   0 root         (0) root         (0)     1627 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/ogrigt.F
--rw-rw-rw-   0 root         (0) root         (0)     5359 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/ogsens.F
--rw-rw-rw-   0 root         (0) root         (0)     1297 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/ogsopt.F
--rw-rw-rw-   0 root         (0) root         (0)     3202 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/ogssst.F
--rw-rw-rw-   0 root         (0) root         (0)     1077 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/ogvsca.F
--rw-rw-rw-   0 root         (0) root         (0)     1309 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/ogvstr.F
--rw-rw-rw-   0 root         (0) root         (0)     1177 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/ogvtyp.F
--rw-rw-rw-   0 root         (0) root         (0)     1192 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/ogwlog.F
--rw-rw-rw-   0 root         (0) root         (0)     1007 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/ogwmat.F
--rw-rw-rw-   0 root         (0) root         (0)      764 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/ogwrit.F
--rw-rw-rw-   0 root         (0) root         (0)     1196 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/ogwtab.F
--rw-rw-rw-   0 root         (0) root         (0)      633 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/sum2v.F
--rw-rw-rw-   0 root         (0) root         (0)    54108 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/core/wrapper.hpp
--rw-rw-rw-   0 root         (0) root         (0)    30520 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyoptgra/optgra.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 14:11:36.273258 pyoptgra-0.1.8/pyoptgra.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2423 2023-02-10 14:11:36.000000 pyoptgra-0.1.8/pyoptgra.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2093 2023-02-10 14:11:36.000000 pyoptgra-0.1.8/pyoptgra.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-10 14:11:36.000000 pyoptgra-0.1.8/pyoptgra.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-02-10 14:11:36.000000 pyoptgra-0.1.8/pyoptgra.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-02-10 14:11:36.000000 pyoptgra-0.1.8/pyoptgra.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      570 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      396 2023-02-10 14:11:36.282259 pyoptgra-0.1.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1032 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 14:11:36.267257 pyoptgra-0.1.8/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 14:11:36.279259 pyoptgra-0.1.8/tests/cpp/
--rw-rw-rw-   0 root         (0) root         (0)     8990 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/tests/cpp/bare-test.cpp
--rw-rw-rw-   0 root         (0) root         (0)    10659 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/tests/cpp/raiitest.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2113 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/tests/cpp/test-callables.hpp
--rw-rw-rw-   0 root         (0) root         (0)     5478 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/tests/cpp/wrappertest.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 14:11:36.280259 pyoptgra-0.1.8/tests/python/
--rw-rw-rw-   0 root         (0) root         (0)    22690 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/tests/python/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 14:11:36.280259 pyoptgra-0.1.8/tools/
--rwxrwxrwx   0 root         (0) root         (0)      457 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/tools/build-manylinux-wheels.sh
--rwxrwxrwx   0 root         (0) root         (0)      788 2023-02-10 13:33:51.000000 pyoptgra-0.1.8/tools/deploy-docs-to-gh-pages.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:53.797590 pyoptgra-0.1.9/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:53.785588 pyoptgra-0.1.9/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:53.789589 pyoptgra-0.1.9/.github/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)      689 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/.github/workflows/deployment.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2461 2023-06-21 13:32:18.000000 pyoptgra-0.1.9/.github/workflows/workflow.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      205 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     4105 2023-06-21 13:32:18.000000 pyoptgra-0.1.9/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/.gitmodules
+-rw-rw-rw-   0 root         (0) root         (0)     3989 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) root         (0)    17060 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/ESA Software Community Licence Weak Copyleft - v2.4
+-rw-rw-rw-   0 root         (0) root         (0)    35150 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/GNU GENERAL PUBLIC LICENSE 3
+-rw-rw-rw-   0 root         (0) root         (0)      615 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/LEGAL
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2423 2023-06-21 13:32:53.797590 pyoptgra-0.1.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2073 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:53.789589 pyoptgra-0.1.9/ThirdPartyLicenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1338 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/ThirdPartyLicenses/CATCH2_LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)     5366 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/ThirdPartyLicenses/CMAKE_LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1676 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/ThirdPartyLicenses/PYBIND11_LICENSE.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:53.785588 pyoptgra-0.1.9/cmake/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:53.789589 pyoptgra-0.1.9/cmake/modules/
+-rw-rw-rw-   0 root         (0) root         (0)      526 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/cmake/modules/Pybind11.cmake
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/cmake/modules/Update_submodules.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:53.785588 pyoptgra-0.1.9/doc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:53.789589 pyoptgra-0.1.9/doc/doxygen/
+-rw-rw-rw-   0 root         (0) root         (0)   112588 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/doc/doxygen/Doxyfile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:53.789589 pyoptgra-0.1.9/doc/sphinx/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/doc/sphinx/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:53.789589 pyoptgra-0.1.9/doc/sphinx/_static/
+-rw-rw-rw-   0 root         (0) root         (0)   423563 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/doc/sphinx/_static/Earth_Mars_SEP_Pyoptgra.html
+-rw-rw-rw-   0 root         (0) root         (0)      729 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/doc/sphinx/api.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4523 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/doc/sphinx/changes-from-fortran.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2324 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/doc/sphinx/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      122 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/doc/sphinx/example-notebook.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1210 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/doc/sphinx/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1843 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/doc/sphinx/scaling-and-tolerances.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5792 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/doc/sphinx/sensitivity.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:53.793589 pyoptgra-0.1.9/pyoptgra/
+-rw-rw-rw-   0 root         (0) root         (0)      899 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-21 13:32:18.000000 pyoptgra-0.1.9/pyoptgra/_about.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:53.797590 pyoptgra-0.1.9/pyoptgra/core/
+-rw-rw-rw-   0 root         (0) root         (0)      858 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4232 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/bindings.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     1865 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/mul2m.F
+-rw-rw-rw-   0 root         (0) root         (0)      820 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/mulvs.F
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/ogcdel.F
+-rw-rw-rw-   0 root         (0) root         (0)     2095 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/ogclos.F
+-rw-rw-rw-   0 root         (0) root         (0)    27579 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/ogcorr.F
+-rw-rw-rw-   0 root         (0) root         (0)     1123 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/ogcpri.F
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/ogcsca.F
+-rw-rw-rw-   0 root         (0) root         (0)     1327 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/ogcstr.F
+-rw-rw-rw-   0 root         (0) root         (0)     1270 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/ogctyp.F
+-rw-rw-rw-   0 root         (0) root         (0)     5244 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/ogdata.inc
+-rw-rw-rw-   0 root         (0) root         (0)     1605 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/ogderi.F
+-rw-rw-rw-   0 root         (0) root         (0)     1389 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/ogdist.F
+-rw-rw-rw-   0 root         (0) root         (0)    14266 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/ogeval.F
+-rw-rw-rw-   0 root         (0) root         (0)     3023 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/ogexcl.F
+-rw-rw-rw-   0 root         (0) root         (0)    17620 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/ogexec.F
+-rw-rw-rw-   0 root         (0) root         (0)     3124 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/oggsst.F
+-rw-rw-rw-   0 root         (0) root         (0)     4721 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/ogincl.F
+-rw-rw-rw-   0 root         (0) root         (0)     5674 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/oginit.F
+-rw-rw-rw-   0 root         (0) root         (0)     1757 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/ogiter.F
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/ogleft.F
+-rw-rw-rw-   0 root         (0) root         (0)     1174 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/ogomet.F
+-rw-rw-rw-   0 root         (0) root         (0)    31825 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/ogopti.F
+-rw-rw-rw-   0 root         (0) root         (0)     1615 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/ogplog.F
+-rw-rw-rw-   0 root         (0) root         (0)     2659 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/ogpwri.F
+-rw-rw-rw-   0 root         (0) root         (0)     2250 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/ogpwri_end.F
+-rw-rw-rw-   0 root         (0) root         (0)     2306 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/ogpwri_start.F
+-rw-rw-rw-   0 root         (0) root         (0)     1627 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/ogrigt.F
+-rw-rw-rw-   0 root         (0) root         (0)     5359 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/ogsens.F
+-rw-rw-rw-   0 root         (0) root         (0)     1297 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/ogsopt.F
+-rw-rw-rw-   0 root         (0) root         (0)     3202 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/ogssst.F
+-rw-rw-rw-   0 root         (0) root         (0)     1077 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/ogvsca.F
+-rw-rw-rw-   0 root         (0) root         (0)     1309 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/ogvstr.F
+-rw-rw-rw-   0 root         (0) root         (0)     1177 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/ogvtyp.F
+-rw-rw-rw-   0 root         (0) root         (0)     1192 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/ogwlog.F
+-rw-rw-rw-   0 root         (0) root         (0)     1007 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/ogwmat.F
+-rw-rw-rw-   0 root         (0) root         (0)      764 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/ogwrit.F
+-rw-rw-rw-   0 root         (0) root         (0)     1196 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/ogwtab.F
+-rw-rw-rw-   0 root         (0) root         (0)      633 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/sum2v.F
+-rw-rw-rw-   0 root         (0) root         (0)    54108 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/core/wrapper.hpp
+-rw-rw-rw-   0 root         (0) root         (0)    30520 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/pyoptgra/optgra.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:53.793589 pyoptgra-0.1.9/pyoptgra.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2423 2023-06-21 13:32:53.000000 pyoptgra-0.1.9/pyoptgra.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2093 2023-06-21 13:32:53.000000 pyoptgra-0.1.9/pyoptgra.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 13:32:53.000000 pyoptgra-0.1.9/pyoptgra.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-21 13:32:53.000000 pyoptgra-0.1.9/pyoptgra.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-21 13:32:53.000000 pyoptgra-0.1.9/pyoptgra.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      570 2023-06-21 13:32:18.000000 pyoptgra-0.1.9/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      396 2023-06-21 13:32:53.797590 pyoptgra-0.1.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1032 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:53.785588 pyoptgra-0.1.9/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:53.797590 pyoptgra-0.1.9/tests/cpp/
+-rw-rw-rw-   0 root         (0) root         (0)     8990 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/tests/cpp/bare-test.cpp
+-rw-rw-rw-   0 root         (0) root         (0)    10659 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/tests/cpp/raiitest.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     2113 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/tests/cpp/test-callables.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     5478 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/tests/cpp/wrappertest.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:53.797590 pyoptgra-0.1.9/tests/python/
+-rw-rw-rw-   0 root         (0) root         (0)    22690 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/tests/python/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:32:53.797590 pyoptgra-0.1.9/tools/
+-rwxrwxrwx   0 root         (0) root         (0)      457 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/tools/build-manylinux-wheels.sh
+-rwxrwxrwx   0 root         (0) root         (0)      788 2023-06-21 13:06:08.000000 pyoptgra-0.1.9/tools/deploy-docs-to-gh-pages.sh
```

### Comparing `pyoptgra-0.1.8/.github/workflows/deployment.yaml` & `pyoptgra-0.1.9/.github/workflows/deployment.yaml`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/.github/workflows/workflow.yaml` & `pyoptgra-0.1.9/.github/workflows/workflow.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
   python-test:
     runs-on: ubuntu-latest
     steps:
       - name: Set up Python
         uses: actions/setup-python@v2
         with:
-          python-version: 3.8
+          python-version: 3.9
       - uses: actions/checkout@v2
       - run: sudo apt update && sudo apt install gfortran --yes
       - run: python -m pip install .
       - run: pip install pytest-cov coverage
       - run: pytest --cov pyoptgra --cov-report term-missing test.py
         working-directory: tests/python
       - run: coverage report --fail-under=95
@@ -48,29 +48,29 @@
 
   doctest:
     runs-on: ubuntu-latest
     steps:
     - name: Set up Python
       uses: actions/setup-python@v2
       with:
-        python-version: 3.8
+        python-version: 3.9
     - uses: actions/checkout@v2
     - run: sudo apt update && sudo apt install gfortran --yes
     - run: pip install sphinx breathe
     - run: python -m pip install .
     - run: make doctest
       working-directory: doc/sphinx
 
   documentation:
     runs-on: ubuntu-latest
     steps:
     - name: Set up Python
       uses: actions/setup-python@v2
       with:
-        python-version: 3.8
+        python-version: 3.9
     - uses: actions/checkout@v2
     - run: sudo apt update && sudo apt install gfortran doxygen --yes
     - run: pip install sphinx breathe sphinx-rtd-theme
     - run: python -m pip install .
     - run: cd doc/doxygen
     - run: doxygen Doxyfile
       working-directory: doc/doxygen
```

### Comparing `pyoptgra-0.1.8/.gitlab-ci.yml` & `pyoptgra-0.1.9/.gitlab-ci.yml`

 * *Files 7% similar despite different names*

```diff
@@ -3,27 +3,27 @@
   - package
   - test-package
   - deploy
   
 # check the code adheres to the coding standards
 static:
   stage: test
-  image: python:3.8
+  image: python:3.9
   allow_failure: false
   script:
     - pip install black==22.8.0 flake8==5.0.4 isort mypy
     - mypy --ignore-missing-imports pyoptgra/*.py
     - black --check pyoptgra/*.py
     - flake8 --max-line-length 125 --ignore='E203','W503','E123','E704','W504','E126','E226','E121','E24' pyoptgra/*.py
     - isort --profile black --check pyoptgra
 
 # check the C++ part compiles and the test runs
 c++-test:
   stage: test
-  image: python:3.8
+  image: python:3.9
   allow_failure: false
   before_script:  # install this project's dependencies
     - apt update && apt install gfortran g++ cmake --yes
   script:
     - mkdir build && cd build
     - cmake ..
     - make optgra-test raii-test bare-test
@@ -31,42 +31,42 @@
     - ./bare-test
     - ./raii-test
     - ./optgra-test
 
 # check the python code compiles and the tests run
 test:
   stage: test
-  image: python:3.8
+  image: python:3.9
   allow_failure: false
   before_script:  # install this project's dependencies
     - apt update && apt install gfortran --yes
   script:
     - python -m pip install .
     - pip install pytest-cov coverage
     - cd tests/python # move into test directory to ensure that the installed package is tested, not the source
     - pytest --cov pyoptgra --cov-report term-missing test.py
     - coverage report --fail-under=95
 
 # check the documentation examples work
 doctest:
   stage: test
-  image: python:3.8
+  image: python:3.9
   allow_failure: false
   before_script:  # install this project's dependencies
     - apt update && apt install gfortran --yes
     - pip install sphinx breathe
   script:
     - python -m pip install .
     - cd doc/sphinx
     - make doctest
 
 # build the documentation
 documentation:
   stage: test
-  image: python:3.8
+  image: python:3.9
   allow_failure: false
   before_script:  # install this project's dependencies
     - apt update && apt install gfortran doxygen --yes
     - pip install sphinx breathe sphinx-rtd-theme
   script:
     - python -m pip install .
     - cd doc/doxygen
@@ -75,15 +75,15 @@
     - make html
   artifacts:
      paths:
        - doc/sphinx/_build
 
 python-sdist:
   stage: package
-  image: python:3.8
+  image: python:3.9
   needs: []
   before_script:
     - apt update && apt install gfortran doxygen --yes
     - pip install --upgrade pip
     - pip install scikit-build setuptools-scm ninja cmake
   script:
     - git submodule update --init --recursive
@@ -106,27 +106,27 @@
   artifacts:
     name: python-wheels-manylinux2010
     paths:
       - pyoptgra-*.whl
 
 test-wheels:
   stage: test-package
-  image: python:3.6
+  image: python:3.9
   script:
-    - pip install pyoptgra*cp36-cp36m*manylinux2010_x86_64.whl
+    - pip install pyoptgra*cp39-cp39*manylinux2010_x86_64.whl
     - mkdir test-install
     - cd test-install
     - python -c "import pyoptgra"
     - cd ..
   needs:
     - python-wheels:manylinux2010
 
 publish:
   stage: deploy
-  image: python:3.8
+  image: python:3.9
   script:
     - pip install twine
     # upload to the project pypi (whl) (change testpypi to pypi to upload to PyPi)
     - twine upload --non-interactive --disable-progress-bar --verbose --repository testpypi -u __token__ -p $TEST_PYPI_TOKEN pyoptgra-*.whl
     # upload to the project pypi (sdist)
     - twine upload --non-interactive --disable-progress-bar --verbose --repository testpypi -u __token__ -p $TEST_PYPI_TOKEN pyoptgra-*.tar.gz
   needs:
@@ -136,15 +136,15 @@
   only:
     refs:
         - master
   when: manual
 
 pages:
   stage: deploy
-  image: python:3.8
+  image: python:3.9
   needs:
     - documentation
     - test-wheels
   script:
   - mkdir -p ./public/html/
   - mv ./doc/sphinx/_build/html/* ./public/
   artifacts:
```

### Comparing `pyoptgra-0.1.8/CMakeLists.txt` & `pyoptgra-0.1.9/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/ESA Software Community Licence Weak Copyleft - v2.4` & `pyoptgra-0.1.9/ESA Software Community Licence Weak Copyleft - v2.4`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/GNU GENERAL PUBLIC LICENSE 3` & `pyoptgra-0.1.9/GNU GENERAL PUBLIC LICENSE 3`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/LEGAL` & `pyoptgra-0.1.9/LEGAL`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/PKG-INFO` & `pyoptgra-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyoptgra
-Version: 0.1.8
+Version: 0.1.9
 Summary: A python-wrapped optimizer for near-linear constrained problems
 Home-page: https://github.com/esa/pyoptgra
 Author: Moritz von Looz
 Author-email: moritz.von.looz@esa.int
 License: GPL 3 OR ESCL 2.4
 Keywords: optimization,constraints
 Platform: UNKNOWN
```

### Comparing `pyoptgra-0.1.8/README.rst` & `pyoptgra-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/ThirdPartyLicenses/CATCH2_LICENSE.txt` & `pyoptgra-0.1.9/ThirdPartyLicenses/CATCH2_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/ThirdPartyLicenses/CMAKE_LICENSE.txt` & `pyoptgra-0.1.9/ThirdPartyLicenses/CMAKE_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/ThirdPartyLicenses/PYBIND11_LICENSE.txt` & `pyoptgra-0.1.9/ThirdPartyLicenses/PYBIND11_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/cmake/modules/Pybind11.cmake` & `pyoptgra-0.1.9/cmake/modules/Pybind11.cmake`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/doc/doxygen/Doxyfile` & `pyoptgra-0.1.9/doc/doxygen/Doxyfile`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/doc/sphinx/Makefile` & `pyoptgra-0.1.9/doc/sphinx/Makefile`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/doc/sphinx/_static/Earth_Mars_SEP_Pyoptgra.html` & `pyoptgra-0.1.9/doc/sphinx/_static/Earth_Mars_SEP_Pyoptgra.html`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/doc/sphinx/api.rst` & `pyoptgra-0.1.9/doc/sphinx/api.rst`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/doc/sphinx/changes-from-fortran.rst` & `pyoptgra-0.1.9/doc/sphinx/changes-from-fortran.rst`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/doc/sphinx/conf.py` & `pyoptgra-0.1.9/doc/sphinx/conf.py`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/doc/sphinx/index.rst` & `pyoptgra-0.1.9/doc/sphinx/index.rst`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/doc/sphinx/scaling-and-tolerances.rst` & `pyoptgra-0.1.9/doc/sphinx/scaling-and-tolerances.rst`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/doc/sphinx/sensitivity.rst` & `pyoptgra-0.1.9/doc/sphinx/sensitivity.rst`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/__init__.py` & `pyoptgra-0.1.9/pyoptgra/__init__.py`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/__init__.py` & `pyoptgra-0.1.9/pyoptgra/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/bindings.cpp` & `pyoptgra-0.1.9/pyoptgra/core/bindings.cpp`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/mul2m.F` & `pyoptgra-0.1.9/pyoptgra/core/mul2m.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/mulvs.F` & `pyoptgra-0.1.9/pyoptgra/core/mulvs.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/ogcdel.F` & `pyoptgra-0.1.9/pyoptgra/core/ogcdel.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/ogclos.F` & `pyoptgra-0.1.9/pyoptgra/core/ogclos.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/ogcorr.F` & `pyoptgra-0.1.9/pyoptgra/core/ogcorr.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/ogcpri.F` & `pyoptgra-0.1.9/pyoptgra/core/ogcpri.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/ogcsca.F` & `pyoptgra-0.1.9/pyoptgra/core/ogcsca.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/ogcstr.F` & `pyoptgra-0.1.9/pyoptgra/core/ogcstr.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/ogctyp.F` & `pyoptgra-0.1.9/pyoptgra/core/ogctyp.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/ogdata.inc` & `pyoptgra-0.1.9/pyoptgra/core/ogdata.inc`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/ogderi.F` & `pyoptgra-0.1.9/pyoptgra/core/ogderi.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/ogdist.F` & `pyoptgra-0.1.9/pyoptgra/core/ogdist.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/ogeval.F` & `pyoptgra-0.1.9/pyoptgra/core/ogeval.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/ogexcl.F` & `pyoptgra-0.1.9/pyoptgra/core/ogexcl.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/ogexec.F` & `pyoptgra-0.1.9/pyoptgra/core/ogexec.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/oggsst.F` & `pyoptgra-0.1.9/pyoptgra/core/oggsst.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/ogincl.F` & `pyoptgra-0.1.9/pyoptgra/core/ogincl.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/oginit.F` & `pyoptgra-0.1.9/pyoptgra/core/oginit.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/ogiter.F` & `pyoptgra-0.1.9/pyoptgra/core/ogiter.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/ogleft.F` & `pyoptgra-0.1.9/pyoptgra/core/ogleft.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/ogomet.F` & `pyoptgra-0.1.9/pyoptgra/core/ogomet.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/ogopti.F` & `pyoptgra-0.1.9/pyoptgra/core/ogopti.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/ogplog.F` & `pyoptgra-0.1.9/pyoptgra/core/ogplog.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/ogpwri.F` & `pyoptgra-0.1.9/pyoptgra/core/ogpwri.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/ogpwri_end.F` & `pyoptgra-0.1.9/pyoptgra/core/ogpwri_end.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/ogpwri_start.F` & `pyoptgra-0.1.9/pyoptgra/core/ogpwri_start.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/ogrigt.F` & `pyoptgra-0.1.9/pyoptgra/core/ogrigt.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/ogsens.F` & `pyoptgra-0.1.9/pyoptgra/core/ogsens.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/ogsopt.F` & `pyoptgra-0.1.9/pyoptgra/core/ogsopt.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/ogssst.F` & `pyoptgra-0.1.9/pyoptgra/core/ogssst.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/ogvsca.F` & `pyoptgra-0.1.9/pyoptgra/core/ogvsca.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/ogvstr.F` & `pyoptgra-0.1.9/pyoptgra/core/ogvstr.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/ogvtyp.F` & `pyoptgra-0.1.9/pyoptgra/core/ogvtyp.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/ogwlog.F` & `pyoptgra-0.1.9/pyoptgra/core/ogwlog.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/ogwmat.F` & `pyoptgra-0.1.9/pyoptgra/core/ogwmat.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/ogwrit.F` & `pyoptgra-0.1.9/pyoptgra/core/ogwrit.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/ogwtab.F` & `pyoptgra-0.1.9/pyoptgra/core/ogwtab.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/sum2v.F` & `pyoptgra-0.1.9/pyoptgra/core/sum2v.F`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/core/wrapper.hpp` & `pyoptgra-0.1.9/pyoptgra/core/wrapper.hpp`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra/optgra.py` & `pyoptgra-0.1.9/pyoptgra/optgra.py`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyoptgra.egg-info/PKG-INFO` & `pyoptgra-0.1.9/pyoptgra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyoptgra
-Version: 0.1.8
+Version: 0.1.9
 Summary: A python-wrapped optimizer for near-linear constrained problems
 Home-page: https://github.com/esa/pyoptgra
 Author: Moritz von Looz
 Author-email: moritz.von.looz@esa.int
 License: GPL 3 OR ESCL 2.4
 Keywords: optimization,constraints
 Platform: UNKNOWN
```

### Comparing `pyoptgra-0.1.8/pyoptgra.egg-info/SOURCES.txt` & `pyoptgra-0.1.9/pyoptgra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/pyproject.toml` & `pyoptgra-0.1.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [project]
 name = "pyoptgra"
-version = "0.1.8"
+version = "0.1.9"
 description = "A python-wrapped version of OPTGRA, an algorithm for constrained optimization"
 authors = [
     {name="Johannes Schoenmaekers", email="johannes.schoenmaekers@esa.int"},
     {name="Moritz von Looz", email="moritz.von.looz@esa.int"}
 ]
 license = {text = "GPL-3.0 or ESCL-2.4"} 
 readme = "README.rst"
 
 dependencies = [
-"pygmo == 2.16.0"
+"pygmo >= 2.16.0"
 ]
 
 [build-system]
 requires = ["setuptools", "wheel", "scikit-build", "cmake", "ninja", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
```

### Comparing `pyoptgra-0.1.8/setup.py` & `pyoptgra-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,10 +22,10 @@
 version = about["__version__"]
 
 setup(
     name="pyoptgra",
     version=version,
     packages=["pyoptgra"],
     setup_requires=["cmake", "ninja"],
-    install_requires=["pygmo==2.16"],
+    install_requires=["pygmo>=2.16"],
     cmake_install_dir="pyoptgra/core",
 )
```

### Comparing `pyoptgra-0.1.8/tests/cpp/bare-test.cpp` & `pyoptgra-0.1.9/tests/cpp/bare-test.cpp`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/tests/cpp/raiitest.cpp` & `pyoptgra-0.1.9/tests/cpp/raiitest.cpp`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/tests/cpp/test-callables.hpp` & `pyoptgra-0.1.9/tests/cpp/test-callables.hpp`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/tests/cpp/wrappertest.cpp` & `pyoptgra-0.1.9/tests/cpp/wrappertest.cpp`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/tests/python/test.py` & `pyoptgra-0.1.9/tests/python/test.py`

 * *Files identical despite different names*

### Comparing `pyoptgra-0.1.8/tools/deploy-docs-to-gh-pages.sh` & `pyoptgra-0.1.9/tools/deploy-docs-to-gh-pages.sh`

 * *Files identical despite different names*

