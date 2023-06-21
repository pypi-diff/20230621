# Comparing `tmp/brnet-0.0.2.tar.gz` & `tmp/brnet-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brnet-0.0.2.tar", last modified: Wed Jun 21 20:46:55 2023, max compression
+gzip compressed data, was "brnet-0.0.3.tar", last modified: Wed Jun 21 21:10:41 2023, max compression
```

## Comparing `brnet-0.0.2.tar` & `brnet-0.0.3.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:46:55.748987 brnet-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:46:55.748987 brnet-0.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-21 20:46:45.000000 brnet-0.0.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:46:55.748987 brnet-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-21 20:46:45.000000 brnet-0.0.2/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-21 20:46:45.000000 brnet-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-21 20:46:45.000000 brnet-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-21 20:46:45.000000 brnet-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-21 20:46:45.000000 brnet-0.0.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-06-21 20:46:55.748987 brnet-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-21 20:46:45.000000 brnet-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-21 20:46:45.000000 brnet-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:46:55.748987 brnet-0.0.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 20:46:45.000000 brnet-0.0.2/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-06-21 20:46:45.000000 brnet-0.0.2/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 20:46:45.000000 brnet-0.0.2/requirements/main.in
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-21 20:46:45.000000 brnet-0.0.2/requirements/main.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 20:46:55.748987 brnet-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:46:55.748987 brnet-0.0.2/sh/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-21 20:46:45.000000 brnet-0.0.2/sh/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     5758 2023-06-21 20:46:45.000000 brnet-0.0.2/sh/brnet
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-21 20:46:45.000000 brnet-0.0.2/sh/pidp11.sh.diff
--rwxr-xr-x   0 runner    (1001) docker     (123)      304 2023-06-21 20:46:45.000000 brnet-0.0.2/sh/wait_for_if
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:46:55.744987 brnet-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:46:55.748987 brnet-0.0.2/src/brnet/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-21 20:46:45.000000 brnet-0.0.2/src/brnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-06-21 20:46:45.000000 brnet-0.0.2/src/brnet/bridger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2853 2023-06-21 20:46:45.000000 brnet-0.0.2/src/brnet/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-21 20:46:45.000000 brnet-0.0.2/src/brnet/external.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:46:55.748987 brnet-0.0.2/src/brnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-06-21 20:46:55.000000 brnet-0.0.2/src/brnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-21 20:46:55.000000 brnet-0.0.2/src/brnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 20:46:55.000000 brnet-0.0.2/src/brnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-21 20:46:55.000000 brnet-0.0.2/src/brnet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 20:46:55.000000 brnet-0.0.2/src/brnet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:46:55.748987 brnet-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 20:46:45.000000 brnet-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-21 20:46:45.000000 brnet-0.0.2/tests/object_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-21 20:46:45.000000 brnet-0.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:10:41.527262 brnet-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:10:41.523262 brnet-0.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-21 21:10:22.000000 brnet-0.0.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:10:41.523262 brnet-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-21 21:10:22.000000 brnet-0.0.3/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-21 21:10:22.000000 brnet-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-21 21:10:22.000000 brnet-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-21 21:10:22.000000 brnet-0.0.3/01-phys-to-bridge
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-21 21:10:22.000000 brnet-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-21 21:10:22.000000 brnet-0.0.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-06-21 21:10:41.527262 brnet-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-21 21:10:22.000000 brnet-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-06-21 21:10:22.000000 brnet-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:10:41.523262 brnet-0.0.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 21:10:22.000000 brnet-0.0.3/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-06-21 21:10:22.000000 brnet-0.0.3/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 21:10:22.000000 brnet-0.0.3/requirements/main.in
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-21 21:10:22.000000 brnet-0.0.3/requirements/main.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 21:10:41.527262 brnet-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:10:41.523262 brnet-0.0.3/sh/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-21 21:10:22.000000 brnet-0.0.3/sh/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5758 2023-06-21 21:10:22.000000 brnet-0.0.3/sh/brnet
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-21 21:10:22.000000 brnet-0.0.3/sh/pidp11.sh.diff
+-rwxr-xr-x   0 runner    (1001) docker     (123)      304 2023-06-21 21:10:22.000000 brnet-0.0.3/sh/wait_for_if
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:10:41.519262 brnet-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:10:41.523262 brnet-0.0.3/src/brnet/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-21 21:10:22.000000 brnet-0.0.3/src/brnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-06-21 21:10:22.000000 brnet-0.0.3/src/brnet/bridger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2853 2023-06-21 21:10:22.000000 brnet-0.0.3/src/brnet/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-21 21:10:22.000000 brnet-0.0.3/src/brnet/external.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:10:41.523262 brnet-0.0.3/src/brnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-06-21 21:10:41.000000 brnet-0.0.3/src/brnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-21 21:10:41.000000 brnet-0.0.3/src/brnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 21:10:41.000000 brnet-0.0.3/src/brnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-21 21:10:41.000000 brnet-0.0.3/src/brnet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 21:10:41.000000 brnet-0.0.3/src/brnet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:10:41.523262 brnet-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 21:10:22.000000 brnet-0.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-21 21:10:22.000000 brnet-0.0.3/tests/object_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-21 21:10:22.000000 brnet-0.0.3/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-21 21:10:22.000000 brnet-0.0.3/wrapper.sh
```

### Comparing `brnet-0.0.2/.github/workflows/ci.yaml` & `brnet-0.0.3/.github/workflows/ci.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -20,35 +20,43 @@
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
-          python-version: "3.11"
+          python-version: "3.9"
 
       - name: Run pre-commit
         uses: pre-commit/action@v3.0.0
 
   test:
     runs-on: ubuntu-latest
 
     strategy:
       matrix:
         python:
+          - "3.9"
+          - "3.10"
           - "3.11"
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
 
+      - name: Regen dependencies
+        run: |
+          rm -f requirements/main.txt requirements/dev.txt
+          make update-deps
+          make init
+
       - name: Run pre-commit
         uses: pre-commit/action@v3.0.0
 
       - name: Install tox
         run: pip install tox
 
       - name: Cache tox environments
@@ -70,14 +78,19 @@
     environment:
       name: pypi
       url: https://pypi.org/p/brnet
     permissions:
       id-token: write
     steps:
       - uses: actions/checkout@v3
+      - name: Set up Python
+        uses: actions/setup-python@v4
+        with:
+          python-version: "3.9"
+
       - name: Build
         run: |
           python3 -m pip install twine build
           python3 -m build
           twine check dist/*
 
       - name: Publish
```

### Comparing `brnet-0.0.2/.gitignore` & `brnet-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `brnet-0.0.2/LICENSE` & `brnet-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `brnet-0.0.2/Makefile` & `brnet-0.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `brnet-0.0.2/PKG-INFO` & `brnet-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brnet
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tool to convert ethernet interface to bridge for emulation
 License: MIT License
         
         Copyright (c) 2020-2023 Adam Thornton
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -26,20 +26,22 @@
         
 Project-URL: Source, https://github.com/athornton/brnet
 Keywords: brnet,pi,emulation
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Typing :: Typed
-Requires-Python: >=3.11
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # brnet
 
 These is a networking tool to make running emulated systems under Linux
 a little easier and more secure.
@@ -68,27 +70,19 @@
 # Installing
 
 `pip install brnet`, or check out the repository and do a `pip install
 -e .`  You probably want to do this in a virtualenv, and if you do that,
 you probably want to install a wrapper script as `/usr/local/bin/brnet`
 to activate the appropriate virtualenv and then run the `brnet` command
 (virtualenv activation will put the new stuff at the head of your
-`$PATH`).
+`$PATH`).  One approach to this is [here](./wrapper.sh).
 
 Then you want to drop the following into `/etc/network/interfaces.d` to
 start the network after the physical interface comes up.  I called my
-file `01-eth0-and-bridge` and it contains:
-
-```
-auto eth0
-iface eth0 inet dhcp
-
-post-up  /usr/local/bin/brnet start
-pre-down /usr/local/bin/brnet stop
-```
+file [`01-phys-to-bridge`](./01-phys-to-bridge).
 
 # Examples
 
 To run using the defaults, which should work for a Raspberry Pi running
 the PiDP-11 software: `brnet start`.
 
 To run with a different user and group and more tap devices:
```

### Comparing `brnet-0.0.2/README.md` & `brnet-0.0.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -27,27 +27,19 @@
 # Installing
 
 `pip install brnet`, or check out the repository and do a `pip install
 -e .`  You probably want to do this in a virtualenv, and if you do that,
 you probably want to install a wrapper script as `/usr/local/bin/brnet`
 to activate the appropriate virtualenv and then run the `brnet` command
 (virtualenv activation will put the new stuff at the head of your
-`$PATH`).
+`$PATH`).  One approach to this is [here](./wrapper.sh).
 
 Then you want to drop the following into `/etc/network/interfaces.d` to
 start the network after the physical interface comes up.  I called my
-file `01-eth0-and-bridge` and it contains:
-
-```
-auto eth0
-iface eth0 inet dhcp
-
-post-up  /usr/local/bin/brnet start
-pre-down /usr/local/bin/brnet stop
-```
+file [`01-phys-to-bridge`](./01-phys-to-bridge).
 
 # Examples
 
 To run using the defaults, which should work for a Raspberry Pi running
 the PiDP-11 software: `brnet start`.
 
 To run with a different user and group and more tap devices:
```

### Comparing `brnet-0.0.2/pyproject.toml` & `brnet-0.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 keywords = ["brnet","pi","emulation"]
 # https://pypi.org/classifiers/
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Operating System :: POSIX",
     "Typing :: Typed",
 ]
-requires-python = ">=3.11"
+requires-python = ">=3.9"
 # Use requirements/main.in for runtime dependencies instead.
 dependencies = []
 dynamic = ["version"]
 
 [project.scripts]
 brnet = "brnet.cli:main"
 
@@ -54,15 +56,15 @@
     "if 0:",
     "if __name__ == .__main__.:",
     "if TYPE_CHECKING:",
 ]
 
 [tool.black]
 line-length = 79
-target-version = ["py311"]
+target-version = ["py39"]
 exclude = '''
 /(
     \.eggs
   | \.git
   | \.mypy_cache
   | \.tox
   | \.venv
@@ -103,10 +105,7 @@
 local_partial_types = true
 no_implicit_reexport = true
 show_error_codes = true
 strict_equality = true
 warn_redundant_casts = true
 warn_unreachable = true
 warn_unused_ignores = true
-
-[tool.distutils.bdist_wheel]
-universal=true
```

### Comparing `brnet-0.0.2/requirements/dev.txt` & `brnet-0.0.3/requirements/dev.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile --generate-hashes --output-file=requirements/dev.txt --resolver=backtracking requirements/dev.in
 #
 coverage[toml]==7.2.7 \
     --hash=sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f \
     --hash=sha256:06fb182e69f33f6cd1d39a6c597294cff3143554b64b9825d1dc69d18cc2fff2 \
@@ -64,14 +64,18 @@
     --hash=sha256:f2f67fe12b22cd130d34d0ef79206061bfb5eda52feb6ce0dba0644e20a03cf4 \
     --hash=sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e \
     --hash=sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850 \
     --hash=sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3
     # via
     #   -r requirements/dev.in
     #   pytest-cov
+exceptiongroup==1.1.1 \
+    --hash=sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e \
+    --hash=sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785
+    # via pytest
 iniconfig==2.0.0 \
     --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
     --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
     # via pytest
 mypy==1.4.0 \
     --hash=sha256:0cf0ca95e4b8adeaf07815a78b4096b65adf64ea7871b39a2116c19497fcd0dd \
     --hash=sha256:0f98973e39e4a98709546a9afd82e1ffcc50c6ec9ce6f7870f33ebbf0bd4f26d \
@@ -104,25 +108,32 @@
     --hash=sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d \
     --hash=sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782
     # via mypy
 packaging==23.1 \
     --hash=sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61 \
     --hash=sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f
     # via pytest
-pluggy==1.0.0 \
-    --hash=sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159 \
-    --hash=sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3
+pluggy==1.2.0 \
+    --hash=sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849 \
+    --hash=sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3
     # via pytest
 pytest==7.3.2 \
     --hash=sha256:cdcbd012c9312258922f8cd3f1b62a6580fdced17db6014896053d47cddf9295 \
     --hash=sha256:ee990a3cc55ba808b80795a79944756f315c67c12b56abd3ac993a7b8c17030b
     # via
     #   -r requirements/dev.in
     #   pytest-cov
 pytest-cov==4.1.0 \
     --hash=sha256:3904b13dfbfec47f003b8e77fd5b589cd11904a21ddf1ab38a64f204d6a10ef6 \
     --hash=sha256:6ba70b9e97e69fcc3fb45bfeab2d0a138fb65c4d0d6a41ef33983ad114be8c3a
     # via -r requirements/dev.in
+tomli==2.0.1 \
+    --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
+    --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
+    # via
+    #   coverage
+    #   mypy
+    #   pytest
 typing-extensions==4.6.3 \
     --hash=sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26 \
     --hash=sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5
     # via mypy
```

### Comparing `brnet-0.0.2/sh/README.md` & `brnet-0.0.3/sh/README.md`

 * *Files identical despite different names*

### Comparing `brnet-0.0.2/sh/brnet` & `brnet-0.0.3/sh/brnet`

 * *Files identical despite different names*

### Comparing `brnet-0.0.2/src/brnet/bridger.py` & `brnet-0.0.3/src/brnet/bridger.py`

 * *Files identical despite different names*

### Comparing `brnet-0.0.2/src/brnet/cli.py` & `brnet-0.0.3/src/brnet/cli.py`

 * *Files identical despite different names*

### Comparing `brnet-0.0.2/src/brnet/external.py` & `brnet-0.0.3/src/brnet/external.py`

 * *Files identical despite different names*

### Comparing `brnet-0.0.2/src/brnet.egg-info/PKG-INFO` & `brnet-0.0.3/src/brnet.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brnet
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tool to convert ethernet interface to bridge for emulation
 License: MIT License
         
         Copyright (c) 2020-2023 Adam Thornton
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -26,20 +26,22 @@
         
 Project-URL: Source, https://github.com/athornton/brnet
 Keywords: brnet,pi,emulation
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Typing :: Typed
-Requires-Python: >=3.11
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # brnet
 
 These is a networking tool to make running emulated systems under Linux
 a little easier and more secure.
@@ -68,27 +70,19 @@
 # Installing
 
 `pip install brnet`, or check out the repository and do a `pip install
 -e .`  You probably want to do this in a virtualenv, and if you do that,
 you probably want to install a wrapper script as `/usr/local/bin/brnet`
 to activate the appropriate virtualenv and then run the `brnet` command
 (virtualenv activation will put the new stuff at the head of your
-`$PATH`).
+`$PATH`).  One approach to this is [here](./wrapper.sh).
 
 Then you want to drop the following into `/etc/network/interfaces.d` to
 start the network after the physical interface comes up.  I called my
-file `01-eth0-and-bridge` and it contains:
-
-```
-auto eth0
-iface eth0 inet dhcp
-
-post-up  /usr/local/bin/brnet start
-pre-down /usr/local/bin/brnet stop
-```
+file [`01-phys-to-bridge`](./01-phys-to-bridge).
 
 # Examples
 
 To run using the defaults, which should work for a Raspberry Pi running
 the PiDP-11 software: `brnet start`.
 
 To run with a different user and group and more tap devices:
```

### Comparing `brnet-0.0.2/src/brnet.egg-info/SOURCES.txt` & `brnet-0.0.3/src/brnet.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 .gitignore
 .pre-commit-config.yaml
+01-phys-to-bridge
 LICENSE
 Makefile
 README.md
 pyproject.toml
 tox.ini
+wrapper.sh
 .github/dependabot.yml
 .github/workflows/ci.yaml
 requirements/dev.in
 requirements/dev.txt
 requirements/main.in
 requirements/main.txt
 sh/README.md
```

### Comparing `brnet-0.0.2/tox.ini` & `brnet-0.0.3/tox.ini`

 * *Files identical despite different names*

