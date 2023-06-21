# Comparing `tmp/pyprecice-2.5.0.2.tar.gz` & `tmp/pyprecice-3.0.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprecice-2.5.0.2.tar", last modified: Tue Feb 21 12:38:05 2023, max compression
+gzip compressed data, was "pyprecice-3.0.0.0.dev0.tar", last modified: Wed Jun 21 08:35:58 2023, max compression
```

## Comparing `pyprecice-2.5.0.2.tar` & `pyprecice-3.0.0.0.dev0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:38:05.450372 pyprecice-2.5.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-02-21 12:37:50.000000 pyprecice-2.5.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-02-21 12:37:50.000000 pyprecice-2.5.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-02-21 12:37:50.000000 pyprecice-2.5.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13605 2023-02-21 12:38:05.450372 pyprecice-2.5.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13261 2023-02-21 12:37:50.000000 pyprecice-2.5.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:38:05.446372 pyprecice-2.5.0.2/cyprecice/
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-02-21 12:37:50.000000 pyprecice-2.5.0.2/cyprecice/SolverInterface.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-02-21 12:37:50.000000 pyprecice-2.5.0.2/cyprecice/cyprecice.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    61672 2023-02-21 12:37:50.000000 pyprecice-2.5.0.2/cyprecice/cyprecice.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:38:05.450372 pyprecice-2.5.0.2/precice/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-02-21 12:37:50.000000 pyprecice-2.5.0.2/precice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-02-21 12:38:05.450372 pyprecice-2.5.0.2/precice/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:38:05.446372 pyprecice-2.5.0.2/pyprecice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13605 2023-02-21 12:38:05.000000 pyprecice-2.5.0.2/pyprecice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-02-21 12:38:05.000000 pyprecice-2.5.0.2/pyprecice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 12:38:05.000000 pyprecice-2.5.0.2/pyprecice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 12:38:05.000000 pyprecice-2.5.0.2/pyprecice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-21 12:38:05.000000 pyprecice-2.5.0.2/pyprecice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-21 12:38:05.000000 pyprecice-2.5.0.2/pyprecice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-02-21 12:37:50.000000 pyprecice-2.5.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-02-21 12:38:05.450372 pyprecice-2.5.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-02-21 12:37:50.000000 pyprecice-2.5.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:38:05.450372 pyprecice-2.5.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)    30685 2023-02-21 12:37:50.000000 pyprecice-2.5.0.2/test/test_bindings_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    70208 2023-02-21 12:37:50.000000 pyprecice-2.5.0.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:35:58.861335 pyprecice-3.0.0.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-21 08:35:43.000000 pyprecice-3.0.0.0.dev0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-21 08:35:43.000000 pyprecice-3.0.0.0.dev0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-21 08:35:43.000000 pyprecice-3.0.0.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14245 2023-06-21 08:35:58.861335 pyprecice-3.0.0.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13896 2023-06-21 08:35:43.000000 pyprecice-3.0.0.0.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:35:58.861335 pyprecice-3.0.0.0.dev0/cyprecice/
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-06-21 08:35:43.000000 pyprecice-3.0.0.0.dev0/cyprecice/Participant.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-21 08:35:43.000000 pyprecice-3.0.0.0.dev0/cyprecice/cyprecice.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    40061 2023-06-21 08:35:43.000000 pyprecice-3.0.0.0.dev0/cyprecice/cyprecice.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:35:58.865335 pyprecice-3.0.0.0.dev0/precice/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-21 08:35:43.000000 pyprecice-3.0.0.0.dev0/precice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-21 08:35:58.865335 pyprecice-3.0.0.0.dev0/precice/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:35:58.861335 pyprecice-3.0.0.0.dev0/pyprecice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14245 2023-06-21 08:35:58.000000 pyprecice-3.0.0.0.dev0/pyprecice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-21 08:35:58.000000 pyprecice-3.0.0.0.dev0/pyprecice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 08:35:58.000000 pyprecice-3.0.0.0.dev0/pyprecice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 08:35:58.000000 pyprecice-3.0.0.0.dev0/pyprecice.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-21 08:35:58.000000 pyprecice-3.0.0.0.dev0/pyprecice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 08:35:58.000000 pyprecice-3.0.0.0.dev0/pyprecice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-21 08:35:43.000000 pyprecice-3.0.0.0.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-21 08:35:58.865335 pyprecice-3.0.0.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-06-21 08:35:43.000000 pyprecice-3.0.0.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:35:58.861335 pyprecice-3.0.0.0.dev0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    27225 2023-06-21 08:35:43.000000 pyprecice-3.0.0.0.dev0/test/test_bindings_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70208 2023-06-21 08:35:43.000000 pyprecice-3.0.0.0.dev0/versioneer.py
```

### Comparing `pyprecice-2.5.0.2/CHANGELOG.md` & `pyprecice-3.0.0.0.dev0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Changelog of Python language bindings for preCICE
 
 All notable changes to this project will be documented in this file.
 
-## latest
+## 3.0.0.0dev0
+
+* Update to API introduced in preCICE v3.0.0. https://github.com/precice/python-bindings/pull/169 https://github.com/precice/python-bindings/pull/174 https://github.com/precice/python-bindings/pull/179
 
 ## 2.5.0.2
 
 * Add Waveform API introduced in preCICE v2.4.0.
 
 ## 2.5.0.1
```

### Comparing `pyprecice-2.5.0.2/LICENSE.txt` & `pyprecice-3.0.0.0.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyprecice-2.5.0.2/PKG-INFO` & `pyprecice-3.0.0.0.dev0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,177 +1,201 @@
 Metadata-Version: 2.1
 Name: pyprecice
-Version: 2.5.0.2
+Version: 3.0.0.0.dev0
 Summary: Python language bindings for the preCICE coupling library
 Home-page: https://github.com/precice/python-bindings
 Author: the preCICE developers
 Author-email: info@precice.org
 License: LGPL-3.0
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-⚠️ The latest version of the documentation for the python bindings can be found on [precice.org](https://precice.org/installation-bindings-python.html). The information from this `README` is currently under revision and will be moved ⚠️
+# Python language bindings for the C++ library preCICE
 
-Python language bindings for the C++ library preCICE
-----------------------------------------------------
+⚠️ The latest version of the documentation for the python bindings can be found on [precice.org](https://precice.org/installation-bindings-python.html). The information from this `README` is currently under revision and will be moved ⚠️
 
 [![Upload Python Package](https://github.com/precice/python-bindings/workflows/Upload%20Python%20Package/badge.svg?branch=master)](https://pypi.org/project/pyprecice/)
 
 This package provides python language bindings for the C++ library [preCICE](https://github.com/precice/precice). Note that the first three digits of the version number of the bindings indicate the preCICE version that the bindings support. The last digit represents the version of the bindings. Example: `v2.0.0.1` and `v2.0.0.2` of the bindings represent versions `1` and `2` of the bindings that are compatible with preCICE `v2.0.0`.
 
-# User documentation
+## User documentation
 
 Please refer to [the preCICE documentation](https://www.precice.org/installation-bindings-python.html) for information on how to install and use the python bindings. Information below is intended for advanced users and developers.
 
-# Required dependencies
+## Required dependencies
 
 **preCICE**: Refer to [the preCICE documentation](https://precice.org/installation-overview.html) for information on building and installation.
 
 **C++**: A working C++ compiler, e.g., `g++`.
 
 **MPI**: `mpi4py` requires MPI to be installed on your system.
 
-# Installing the package
+## Installing the package
 
 We recommend using pip3 (version 19.0.0 or newer required) for the sake of simplicity. You can check your pip3 version via `pip3 --version`. To update pip3, use the following line:
 
-```
+```bash
 $ pip3 install --user --upgrade pip
 ```
 
-## Using pip3
+### Using pip3
 
-### preCICE system installs
+#### preCICE system installs
 
 For system installs of preCICE, installation works out of the box. There are different ways how pip can be used to install pyprecice. pip will fetch cython and other build-time dependencies, compile the bindings and finally install the package pyprecice.
 
 * (recommended) install [pyprecice from PyPI](https://pypi.org/project/pyprecice/)
 
-  ```
+  ```bash
   $ pip3 install --user pyprecice
   ```
 
 * provide the link to this repository to pip (replace `<branch>` with the branch you want to use, preferably `master` or `develop`)
 
-  ```
+  ```bash
   $ pip3 install --user https://github.com/precice/python-bindings/archive/<branch>.zip
   ```
 
 * if you already cloned this repository, execute the following command from this directory:
 
-  ```
+  ```bash
   $ pip3 install --user .
   ```
+
   *note the dot at the end of the line*
 
-### preCICE at custom location (setting PATHS)
+#### preCICE at custom location (setting PATHS)
 
 If preCICE (the C++ library) was installed in a custom prefix, or only built but not installed at all, you have to extend the following environment variables:
 
-- `LIBRARY_PATH`, `LD_LIBRARY_PATH` to the library location, or `$prefix/lib`
-- `CPATH` either to the `src` directory or the `$prefix/include`
+* `LIBRARY_PATH`, `LD_LIBRARY_PATH` to the library location, or `$prefix/lib`
+* `CPATH` either to the `src` directory or the `$prefix/include`
 
 The preCICE documentation provides more informaiton on [linking preCICE](https://precice.org/installation-linking.html).
 
-## Using Spack
+### Using Spack
 
 You can also install the python language bindings for preCICE via Spack by installing the Spack package `py-pyprecice`. Refer to [our installation guide for preCICE via Spack](https://precice.org/installation-spack.html) for getting started with Spack.
 
-## Using setup.py
+### Using setup.py
 
-### preCICE system installs
+#### preCICE system installs
 
 In this directory, execute:
-```
+
+```bash
 $ python3 setup.py install --user
 ```
 
-### preCICE at custom location (setting PATHS)
+#### preCICE at custom location (setting PATHS)
 
 see above. Then run
-```
+
+```bash
 $ python3 setup.py install --user
 ```
 
-### preCICE at custom location (explicit include path, library path)
+#### preCICE at custom location (explicit include path, library path)
 
 1. Install cython and other dependencies via pip3
-   ```
+
+   ```bash
    $ pip3 install --user setuptools wheel cython packaging numpy
    ```
+
 2. Open terminal in this folder.
 3. Build the bindings
-   ```
+
+   ```bash
    $ python3 setup.py build_ext --include-dirs=$PRECICE_ROOT/src --library-dirs=$PRECICE_ROOT/build/last
    ```
 
-  **Options:**
-  - `--include-dirs=`, default: `''` 
-    Path to the headers of preCICE, point to the sources `$PRECICE_ROOT/src`, or the your custom install prefix `$prefix/include`.
-  
-  **NOTES:**
-  
-  - If you have built preCICE using CMake, you can pass the path to the CMake binary directory using `--library-dirs`.
-  - It is recommended to use preCICE as a shared library here.
+   **Options:**
+   * `--include-dirs=`, default: `''`
+     Path to the headers of preCICE, point to the sources `$PRECICE_ROOT/src`, or the your custom install prefix `$prefix/include`.
+
+   **NOTES:**
+
+   * If you have built preCICE using CMake, you can pass the path to the CMake binary directory using `--library-dirs`.
+   * It is recommended to use preCICE as a shared library here.
 
 4. Install the bindings
-   ```
+
+   ```bash
    $ python3 setup.py install --user
    ```
 
-5. Clean-up _optional_
-   ```
+5. Clean-up *optional*
+
+   ```bash
    $ python3 setup.py clean --all
    ```
 
-# Test the installation
+## Test the installation
 
 Update `LD_LIBRARY_PATH` such that python can find `precice.so`
 
-```
+```bash
 $ export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:$PRECICE_ROOT/build/last
 ```
 
 Run the following to test the installation:
 
-```
+```bash
 $ python3 -c "import precice"
 ```
 
-## Unit tests
+### Unit tests
 
-1. Clean-up __mandatory__ (because we must not link against the real `precice.so`, but we use a mocked version)
-   ```
+1. Clean-up **mandatory** (because we must not link against the real `precice.so`, but we use a mocked version)
+
+   ```bash
    $ python3 setup.py clean --all
    ```
 
 2. Set `CPLUS_INCLUDE_PATH` (we cannot use `build_ext` and the `--include-dirs` option here)
-   ```
+
+   ```bash
    $ export CPLUS_INCLUDE_PATH=$CPLUS_INCLUDE_PATH:$PRECICE_ROOT/src
    ```
 
 3. Run tests with
-   ```
+
+   ```bash
    $ python3 setup.py test
    ```
 
-# Usage
+## Usage
 
-You can find the documentation of the implemented interface in the file `precice.pyx`. For an example of how `pyprecice` can be used please refer to the [1D elastic tube example](https://precice.org/tutorials-elastic-tube-1d.html#python). 
+You can find the documentation of the implemented interface in the file `precice.pyx`. For an example of how `pyprecice` can be used please refer to the [1D elastic tube example](https://precice.org/tutorials-elastic-tube-1d.html#python).
 
 **Note** The python package that is installed is called `pyprecice`. It provides the python module `precice` that can be use in your code via `import precice`, for example.
 
-# Troubleshooting & miscellaneous
+## Troubleshooting & miscellaneous
 
 ### preCICE is not found
 
 The following error shows up during installation, if preCICE is not found:
 
+```bash
+  /tmp/pip-install-d_fjyo1h/pyprecice/precice.cpp:643:10: fatal error: precice/Participant.hpp: No such file or directory
+    643 | #include "precice/Participant.hpp"
+        |          ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+  compilation terminated.
+  error: command 'x86_64-linux-gnu-gcc' failed with exit status 1
+  ----------------------------------------
+  ERROR: Failed building wheel for pyprecice
+Failed to build pyprecice
+ERROR: Could not build wheels for pyprecice which use PEP 517 and cannot be installed directly
 ```
+
+Or, for preCICE v2:
+
+```bash
   /tmp/pip-install-d_fjyo1h/pyprecice/precice.cpp:643:10: fatal error: precice/SolverInterface.hpp: No such file or directory
     643 | #include "precice/SolverInterface.hpp"
         |          ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~
   compilation terminated.
   error: command 'x86_64-linux-gnu-gcc' failed with exit status 1
   ----------------------------------------
   ERROR: Failed building wheel for pyprecice
@@ -186,31 +210,31 @@
 
 ### Version of Cython is too old
 
 In case the compilation fails with `shared_ptr.pxd not found` messages, check if you use the latest version of Cython.
 
 ### `Python.h` missing
 
-```
+```bash
 $ python3 -m pip install pyprecice
 Collecting pyprecice
 ...
   /tmp/pip-build-7rj4_h93/pyprecice/precice.cpp:25:20: fatal error: Python.h: No such file or directory
   compilation terminated.
   error: command 'x86_64-linux-gnu-gcc' failed with exit status 1
 
   ----------------------------------------
-  Failed building wheel for pyprecice 
+  Failed building wheel for pyprecice
 ```
 
 Please try to install `python3-dev`. E.g. via `apt install python3-dev`. Please make sure that you use the correct version (e.g. `python3.5-dev` or `python3.6-dev`). You can check your version via `python3 --version`.
 
 ### `libprecice.so` is not found at runtime
 
-```
+```bash
 $ python3 -c "import precice"
 Traceback (most recent call last):
   File "<stdin>", line 1, in <module>
 ImportError: libprecice.so.2: cannot open shared object file: No such file or directory
 ```
 
 Make sure that your `LD_LIBRARY_PATH` includes the directory that contains `libprecice.so`. The actual path depends on how you installed preCICE. Example: If preCICE was installed using `sudo make install` and you did not define a `CMAKE_INSTALL_PREFIX` the library path is `/usr/local/lib`. This means you have to `export LD_LIBRARY_PATH=/usr/local/lib:$LD_LIBRARY_PATH`.
@@ -224,81 +248,94 @@
 *Note that the instructions in this section are outdated and refer to the deprecated python bindings. Until we have updated information on the installation procedure for the python bindings under this use-case, we will keep these instructions, since they might still be very useful* (Originally contributed by [huangq1234553](https://github.com/huangq1234553) to the precice wiki in [`precice/precice/wiki:8bb74b7`](https://github.com/precice/precice/wiki/Dependencies/8bb74b78a7ebc54983f4822af82fb3d638021faa).)
 
 <details><summary>show details</summary>
 
 This guide provides steps to install python bindings for precice-1.6.1 for a conda environment Python 2.7.17 on the CoolMUC. Note that preCICE no longer supports Python 2 after v1.4.0. Hence, some modifications to the python setup code was necessary. Most steps are similar if not identical to the basic guide without petsc or python above. This guide assumes that the Eigen dependencies have already been installed.
 
 Load the prerequisite libraries:
-```
+
+```bash
 module load gcc/7
 module unload mpi.intel
 module load mpi.intel/2018_gcc
 module load cmake/3.12.1
 ```
+
 At the time of this writing `module load boost/1.68.0` is no longer available. Instead
-boost 1.65.1 was installed per the `boost and yaml-cpp` guide above. 
+boost 1.65.1 was installed per the `boost and yaml-cpp` guide above.
 
 In order to have the right python dependencies, a packaged conda environment was transferred to
 SuperMUC. The following dependencies were installed:
-- numpy
-- mpi4py
+
+* numpy
+* mpi4py
 
 With the python environment active, we have to feed the right python file directories to the cmake command.
 Note that -DPYTHON_LIBRARY expects a python shared library. You can likely modify the version to fit what is required.
-```
+
+```bash
 mkdir build && cd build
 cmake -DBUILD_SHARED_LIBS=ON -DPRECICE_PETScMapping=OFF -DPRECICE_PythonActions=ON -DCMAKE_INSTALL_PREFIX=/path/to/precice -DCMAKE_BUILD_TYPE=Debug .. -DPYTHON_INCLUDE_DIR=$(python -c "from distutils.sysconfig import get_python_inc; print(get_python_inc())")  -DPYTHON_LIBRARY=$(python -c "import distutils.sysconfig as sysconfig; print(sysconfig.get_config_var('LIBDIR')+'/libpython2.7.so')") -DNumPy_INCLUDE_DIR=$(python -c "import numpy; print(numpy.get_include())")
 make -j 12
 make install
 ```
+
 After installing, make sure you add the preCICE installation paths to your `.bashrc`, so that other programs can find it:
-```
+
+```bash
 export PRECICE_ROOT="path/to/precice_install"
 export PKG_CONFIG_PATH="path/to/precice_install/lib/pkgconfig:${PKG_CONFIG_PATH}"
 export CPLUS_INCLUDE_PATH="path/to/precice_install/include:${CPLUS_INCLUDE_PATH}"
 export LD_LIBRARY_PATH="path/to/precice_install/lib:${LD_LIBRARY_PATH}"
 ```
+
 Then, navigate to the python_future bindings script.
-```
+
+```bash
 cd /path/to/precice/src/precice/bindings/python_future
 ```
+
 Append the following to the head of the file to allow Python2 to run Python3 code. Note that
-importing `unicode_literals` from `future` will cause errors in `setuptools` methods as string literals 
+importing `unicode_literals` from `future` will cause errors in `setuptools` methods as string literals
 in code are interpreted as `unicode` with this import.
-```
+
+```python
 from __future__ import (absolute_import, division,
                         print_function)
 from builtins import (
          bytes, dict, int, list, object, range, str,
          ascii, chr, hex, input, next, oct, open,
          pow, round, super,
          filter, map, zip)
 ```
+
 Modify `mpicompiler_default = "mpic++"` to `mpicompiler_default = "mpicxx"` in line 100.
 Run the setup file using the default Python 2.7.17.
-```
+
+```bash
 python setup.py install --user
 ```
+
 </details>
 
 ### ValueError while importing preCICE
+
 If you face the error:
 
 ```bash
 ValueError: numpy.ndarray size changed, may indicate binary incompatibility. Expected 88 from C header, got 80 from PyObject
 ```
 
 make sure that you are using an up-to-date version of NumPy. You can update NumPy with
 
 ```bash
 pip3 install numpy --upgrade
 ```
 
-
-# Contributors
+## Contributors
 
 * [Benjamin Rodenberg](https://github.com/BenjaminRodenberg)
 * [Ishaan Desai](https://github.com/IshaanDesai)
 * [Saumitra Vinay Joshi](https://github.com/saumiJ) contributed first working prototype in [`3db9c9` on `precice/precice`](https://github.com/precice/precice/commit/3db9c95e527db1e1cacb2fd116a5ce13ee877513)
 * [Frédéric Simonis](https://github.com/fsimonis)
 * [Florian Lindner](https://github.com/floli)
 * [Benjamin Uekermann](https://github.com/uekerman)
```

### Comparing `pyprecice-2.5.0.2/README.md` & `pyprecice-3.0.0.0.dev0/pyprecice.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,165 +1,201 @@
-⚠️ The latest version of the documentation for the python bindings can be found on [precice.org](https://precice.org/installation-bindings-python.html). The information from this `README` is currently under revision and will be moved ⚠️
+Metadata-Version: 2.1
+Name: pyprecice
+Version: 3.0.0.0.dev0
+Summary: Python language bindings for the preCICE coupling library
+Home-page: https://github.com/precice/python-bindings
+Author: the preCICE developers
+Author-email: info@precice.org
+License: LGPL-3.0
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Python language bindings for the C++ library preCICE
 
-Python language bindings for the C++ library preCICE
-----------------------------------------------------
+⚠️ The latest version of the documentation for the python bindings can be found on [precice.org](https://precice.org/installation-bindings-python.html). The information from this `README` is currently under revision and will be moved ⚠️
 
 [![Upload Python Package](https://github.com/precice/python-bindings/workflows/Upload%20Python%20Package/badge.svg?branch=master)](https://pypi.org/project/pyprecice/)
 
 This package provides python language bindings for the C++ library [preCICE](https://github.com/precice/precice). Note that the first three digits of the version number of the bindings indicate the preCICE version that the bindings support. The last digit represents the version of the bindings. Example: `v2.0.0.1` and `v2.0.0.2` of the bindings represent versions `1` and `2` of the bindings that are compatible with preCICE `v2.0.0`.
 
-# User documentation
+## User documentation
 
 Please refer to [the preCICE documentation](https://www.precice.org/installation-bindings-python.html) for information on how to install and use the python bindings. Information below is intended for advanced users and developers.
 
-# Required dependencies
+## Required dependencies
 
 **preCICE**: Refer to [the preCICE documentation](https://precice.org/installation-overview.html) for information on building and installation.
 
 **C++**: A working C++ compiler, e.g., `g++`.
 
 **MPI**: `mpi4py` requires MPI to be installed on your system.
 
-# Installing the package
+## Installing the package
 
 We recommend using pip3 (version 19.0.0 or newer required) for the sake of simplicity. You can check your pip3 version via `pip3 --version`. To update pip3, use the following line:
 
-```
+```bash
 $ pip3 install --user --upgrade pip
 ```
 
-## Using pip3
+### Using pip3
 
-### preCICE system installs
+#### preCICE system installs
 
 For system installs of preCICE, installation works out of the box. There are different ways how pip can be used to install pyprecice. pip will fetch cython and other build-time dependencies, compile the bindings and finally install the package pyprecice.
 
 * (recommended) install [pyprecice from PyPI](https://pypi.org/project/pyprecice/)
 
-  ```
+  ```bash
   $ pip3 install --user pyprecice
   ```
 
 * provide the link to this repository to pip (replace `<branch>` with the branch you want to use, preferably `master` or `develop`)
 
-  ```
+  ```bash
   $ pip3 install --user https://github.com/precice/python-bindings/archive/<branch>.zip
   ```
 
 * if you already cloned this repository, execute the following command from this directory:
 
-  ```
+  ```bash
   $ pip3 install --user .
   ```
+
   *note the dot at the end of the line*
 
-### preCICE at custom location (setting PATHS)
+#### preCICE at custom location (setting PATHS)
 
 If preCICE (the C++ library) was installed in a custom prefix, or only built but not installed at all, you have to extend the following environment variables:
 
-- `LIBRARY_PATH`, `LD_LIBRARY_PATH` to the library location, or `$prefix/lib`
-- `CPATH` either to the `src` directory or the `$prefix/include`
+* `LIBRARY_PATH`, `LD_LIBRARY_PATH` to the library location, or `$prefix/lib`
+* `CPATH` either to the `src` directory or the `$prefix/include`
 
 The preCICE documentation provides more informaiton on [linking preCICE](https://precice.org/installation-linking.html).
 
-## Using Spack
+### Using Spack
 
 You can also install the python language bindings for preCICE via Spack by installing the Spack package `py-pyprecice`. Refer to [our installation guide for preCICE via Spack](https://precice.org/installation-spack.html) for getting started with Spack.
 
-## Using setup.py
+### Using setup.py
 
-### preCICE system installs
+#### preCICE system installs
 
 In this directory, execute:
-```
+
+```bash
 $ python3 setup.py install --user
 ```
 
-### preCICE at custom location (setting PATHS)
+#### preCICE at custom location (setting PATHS)
 
 see above. Then run
-```
+
+```bash
 $ python3 setup.py install --user
 ```
 
-### preCICE at custom location (explicit include path, library path)
+#### preCICE at custom location (explicit include path, library path)
 
 1. Install cython and other dependencies via pip3
-   ```
+
+   ```bash
    $ pip3 install --user setuptools wheel cython packaging numpy
    ```
+
 2. Open terminal in this folder.
 3. Build the bindings
-   ```
+
+   ```bash
    $ python3 setup.py build_ext --include-dirs=$PRECICE_ROOT/src --library-dirs=$PRECICE_ROOT/build/last
    ```
 
-  **Options:**
-  - `--include-dirs=`, default: `''` 
-    Path to the headers of preCICE, point to the sources `$PRECICE_ROOT/src`, or the your custom install prefix `$prefix/include`.
-  
-  **NOTES:**
-  
-  - If you have built preCICE using CMake, you can pass the path to the CMake binary directory using `--library-dirs`.
-  - It is recommended to use preCICE as a shared library here.
+   **Options:**
+   * `--include-dirs=`, default: `''`
+     Path to the headers of preCICE, point to the sources `$PRECICE_ROOT/src`, or the your custom install prefix `$prefix/include`.
+
+   **NOTES:**
+
+   * If you have built preCICE using CMake, you can pass the path to the CMake binary directory using `--library-dirs`.
+   * It is recommended to use preCICE as a shared library here.
 
 4. Install the bindings
-   ```
+
+   ```bash
    $ python3 setup.py install --user
    ```
 
-5. Clean-up _optional_
-   ```
+5. Clean-up *optional*
+
+   ```bash
    $ python3 setup.py clean --all
    ```
 
-# Test the installation
+## Test the installation
 
 Update `LD_LIBRARY_PATH` such that python can find `precice.so`
 
-```
+```bash
 $ export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:$PRECICE_ROOT/build/last
 ```
 
 Run the following to test the installation:
 
-```
+```bash
 $ python3 -c "import precice"
 ```
 
-## Unit tests
+### Unit tests
 
-1. Clean-up __mandatory__ (because we must not link against the real `precice.so`, but we use a mocked version)
-   ```
+1. Clean-up **mandatory** (because we must not link against the real `precice.so`, but we use a mocked version)
+
+   ```bash
    $ python3 setup.py clean --all
    ```
 
 2. Set `CPLUS_INCLUDE_PATH` (we cannot use `build_ext` and the `--include-dirs` option here)
-   ```
+
+   ```bash
    $ export CPLUS_INCLUDE_PATH=$CPLUS_INCLUDE_PATH:$PRECICE_ROOT/src
    ```
 
 3. Run tests with
-   ```
+
+   ```bash
    $ python3 setup.py test
    ```
 
-# Usage
+## Usage
 
-You can find the documentation of the implemented interface in the file `precice.pyx`. For an example of how `pyprecice` can be used please refer to the [1D elastic tube example](https://precice.org/tutorials-elastic-tube-1d.html#python). 
+You can find the documentation of the implemented interface in the file `precice.pyx`. For an example of how `pyprecice` can be used please refer to the [1D elastic tube example](https://precice.org/tutorials-elastic-tube-1d.html#python).
 
 **Note** The python package that is installed is called `pyprecice`. It provides the python module `precice` that can be use in your code via `import precice`, for example.
 
-# Troubleshooting & miscellaneous
+## Troubleshooting & miscellaneous
 
 ### preCICE is not found
 
 The following error shows up during installation, if preCICE is not found:
 
+```bash
+  /tmp/pip-install-d_fjyo1h/pyprecice/precice.cpp:643:10: fatal error: precice/Participant.hpp: No such file or directory
+    643 | #include "precice/Participant.hpp"
+        |          ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+  compilation terminated.
+  error: command 'x86_64-linux-gnu-gcc' failed with exit status 1
+  ----------------------------------------
+  ERROR: Failed building wheel for pyprecice
+Failed to build pyprecice
+ERROR: Could not build wheels for pyprecice which use PEP 517 and cannot be installed directly
 ```
+
+Or, for preCICE v2:
+
+```bash
   /tmp/pip-install-d_fjyo1h/pyprecice/precice.cpp:643:10: fatal error: precice/SolverInterface.hpp: No such file or directory
     643 | #include "precice/SolverInterface.hpp"
         |          ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~
   compilation terminated.
   error: command 'x86_64-linux-gnu-gcc' failed with exit status 1
   ----------------------------------------
   ERROR: Failed building wheel for pyprecice
@@ -174,31 +210,31 @@
 
 ### Version of Cython is too old
 
 In case the compilation fails with `shared_ptr.pxd not found` messages, check if you use the latest version of Cython.
 
 ### `Python.h` missing
 
-```
+```bash
 $ python3 -m pip install pyprecice
 Collecting pyprecice
 ...
   /tmp/pip-build-7rj4_h93/pyprecice/precice.cpp:25:20: fatal error: Python.h: No such file or directory
   compilation terminated.
   error: command 'x86_64-linux-gnu-gcc' failed with exit status 1
 
   ----------------------------------------
-  Failed building wheel for pyprecice 
+  Failed building wheel for pyprecice
 ```
 
 Please try to install `python3-dev`. E.g. via `apt install python3-dev`. Please make sure that you use the correct version (e.g. `python3.5-dev` or `python3.6-dev`). You can check your version via `python3 --version`.
 
 ### `libprecice.so` is not found at runtime
 
-```
+```bash
 $ python3 -c "import precice"
 Traceback (most recent call last):
   File "<stdin>", line 1, in <module>
 ImportError: libprecice.so.2: cannot open shared object file: No such file or directory
 ```
 
 Make sure that your `LD_LIBRARY_PATH` includes the directory that contains `libprecice.so`. The actual path depends on how you installed preCICE. Example: If preCICE was installed using `sudo make install` and you did not define a `CMAKE_INSTALL_PREFIX` the library path is `/usr/local/lib`. This means you have to `export LD_LIBRARY_PATH=/usr/local/lib:$LD_LIBRARY_PATH`.
@@ -212,81 +248,94 @@
 *Note that the instructions in this section are outdated and refer to the deprecated python bindings. Until we have updated information on the installation procedure for the python bindings under this use-case, we will keep these instructions, since they might still be very useful* (Originally contributed by [huangq1234553](https://github.com/huangq1234553) to the precice wiki in [`precice/precice/wiki:8bb74b7`](https://github.com/precice/precice/wiki/Dependencies/8bb74b78a7ebc54983f4822af82fb3d638021faa).)
 
 <details><summary>show details</summary>
 
 This guide provides steps to install python bindings for precice-1.6.1 for a conda environment Python 2.7.17 on the CoolMUC. Note that preCICE no longer supports Python 2 after v1.4.0. Hence, some modifications to the python setup code was necessary. Most steps are similar if not identical to the basic guide without petsc or python above. This guide assumes that the Eigen dependencies have already been installed.
 
 Load the prerequisite libraries:
-```
+
+```bash
 module load gcc/7
 module unload mpi.intel
 module load mpi.intel/2018_gcc
 module load cmake/3.12.1
 ```
+
 At the time of this writing `module load boost/1.68.0` is no longer available. Instead
-boost 1.65.1 was installed per the `boost and yaml-cpp` guide above. 
+boost 1.65.1 was installed per the `boost and yaml-cpp` guide above.
 
 In order to have the right python dependencies, a packaged conda environment was transferred to
 SuperMUC. The following dependencies were installed:
-- numpy
-- mpi4py
+
+* numpy
+* mpi4py
 
 With the python environment active, we have to feed the right python file directories to the cmake command.
 Note that -DPYTHON_LIBRARY expects a python shared library. You can likely modify the version to fit what is required.
-```
+
+```bash
 mkdir build && cd build
 cmake -DBUILD_SHARED_LIBS=ON -DPRECICE_PETScMapping=OFF -DPRECICE_PythonActions=ON -DCMAKE_INSTALL_PREFIX=/path/to/precice -DCMAKE_BUILD_TYPE=Debug .. -DPYTHON_INCLUDE_DIR=$(python -c "from distutils.sysconfig import get_python_inc; print(get_python_inc())")  -DPYTHON_LIBRARY=$(python -c "import distutils.sysconfig as sysconfig; print(sysconfig.get_config_var('LIBDIR')+'/libpython2.7.so')") -DNumPy_INCLUDE_DIR=$(python -c "import numpy; print(numpy.get_include())")
 make -j 12
 make install
 ```
+
 After installing, make sure you add the preCICE installation paths to your `.bashrc`, so that other programs can find it:
-```
+
+```bash
 export PRECICE_ROOT="path/to/precice_install"
 export PKG_CONFIG_PATH="path/to/precice_install/lib/pkgconfig:${PKG_CONFIG_PATH}"
 export CPLUS_INCLUDE_PATH="path/to/precice_install/include:${CPLUS_INCLUDE_PATH}"
 export LD_LIBRARY_PATH="path/to/precice_install/lib:${LD_LIBRARY_PATH}"
 ```
+
 Then, navigate to the python_future bindings script.
-```
+
+```bash
 cd /path/to/precice/src/precice/bindings/python_future
 ```
+
 Append the following to the head of the file to allow Python2 to run Python3 code. Note that
-importing `unicode_literals` from `future` will cause errors in `setuptools` methods as string literals 
+importing `unicode_literals` from `future` will cause errors in `setuptools` methods as string literals
 in code are interpreted as `unicode` with this import.
-```
+
+```python
 from __future__ import (absolute_import, division,
                         print_function)
 from builtins import (
          bytes, dict, int, list, object, range, str,
          ascii, chr, hex, input, next, oct, open,
          pow, round, super,
          filter, map, zip)
 ```
+
 Modify `mpicompiler_default = "mpic++"` to `mpicompiler_default = "mpicxx"` in line 100.
 Run the setup file using the default Python 2.7.17.
-```
+
+```bash
 python setup.py install --user
 ```
+
 </details>
 
 ### ValueError while importing preCICE
+
 If you face the error:
 
 ```bash
 ValueError: numpy.ndarray size changed, may indicate binary incompatibility. Expected 88 from C header, got 80 from PyObject
 ```
 
 make sure that you are using an up-to-date version of NumPy. You can update NumPy with
 
 ```bash
 pip3 install numpy --upgrade
 ```
 
-
-# Contributors
+## Contributors
 
 * [Benjamin Rodenberg](https://github.com/BenjaminRodenberg)
 * [Ishaan Desai](https://github.com/IshaanDesai)
 * [Saumitra Vinay Joshi](https://github.com/saumiJ) contributed first working prototype in [`3db9c9` on `precice/precice`](https://github.com/precice/precice/commit/3db9c95e527db1e1cacb2fd116a5ce13ee877513)
 * [Frédéric Simonis](https://github.com/fsimonis)
 * [Florian Lindner](https://github.com/floli)
 * [Benjamin Uekermann](https://github.com/uekerman)
```

### Comparing `pyprecice-2.5.0.2/pyprecice.egg-info/PKG-INFO` & `pyprecice-3.0.0.0.dev0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,177 +1,189 @@
-Metadata-Version: 2.1
-Name: pyprecice
-Version: 2.5.0.2
-Summary: Python language bindings for the preCICE coupling library
-Home-page: https://github.com/precice/python-bindings
-Author: the preCICE developers
-Author-email: info@precice.org
-License: LGPL-3.0
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+# Python language bindings for the C++ library preCICE
 
 ⚠️ The latest version of the documentation for the python bindings can be found on [precice.org](https://precice.org/installation-bindings-python.html). The information from this `README` is currently under revision and will be moved ⚠️
 
-Python language bindings for the C++ library preCICE
-----------------------------------------------------
-
 [![Upload Python Package](https://github.com/precice/python-bindings/workflows/Upload%20Python%20Package/badge.svg?branch=master)](https://pypi.org/project/pyprecice/)
 
 This package provides python language bindings for the C++ library [preCICE](https://github.com/precice/precice). Note that the first three digits of the version number of the bindings indicate the preCICE version that the bindings support. The last digit represents the version of the bindings. Example: `v2.0.0.1` and `v2.0.0.2` of the bindings represent versions `1` and `2` of the bindings that are compatible with preCICE `v2.0.0`.
 
-# User documentation
+## User documentation
 
 Please refer to [the preCICE documentation](https://www.precice.org/installation-bindings-python.html) for information on how to install and use the python bindings. Information below is intended for advanced users and developers.
 
-# Required dependencies
+## Required dependencies
 
 **preCICE**: Refer to [the preCICE documentation](https://precice.org/installation-overview.html) for information on building and installation.
 
 **C++**: A working C++ compiler, e.g., `g++`.
 
 **MPI**: `mpi4py` requires MPI to be installed on your system.
 
-# Installing the package
+## Installing the package
 
 We recommend using pip3 (version 19.0.0 or newer required) for the sake of simplicity. You can check your pip3 version via `pip3 --version`. To update pip3, use the following line:
 
-```
+```bash
 $ pip3 install --user --upgrade pip
 ```
 
-## Using pip3
+### Using pip3
 
-### preCICE system installs
+#### preCICE system installs
 
 For system installs of preCICE, installation works out of the box. There are different ways how pip can be used to install pyprecice. pip will fetch cython and other build-time dependencies, compile the bindings and finally install the package pyprecice.
 
 * (recommended) install [pyprecice from PyPI](https://pypi.org/project/pyprecice/)
 
-  ```
+  ```bash
   $ pip3 install --user pyprecice
   ```
 
 * provide the link to this repository to pip (replace `<branch>` with the branch you want to use, preferably `master` or `develop`)
 
-  ```
+  ```bash
   $ pip3 install --user https://github.com/precice/python-bindings/archive/<branch>.zip
   ```
 
 * if you already cloned this repository, execute the following command from this directory:
 
-  ```
+  ```bash
   $ pip3 install --user .
   ```
+
   *note the dot at the end of the line*
 
-### preCICE at custom location (setting PATHS)
+#### preCICE at custom location (setting PATHS)
 
 If preCICE (the C++ library) was installed in a custom prefix, or only built but not installed at all, you have to extend the following environment variables:
 
-- `LIBRARY_PATH`, `LD_LIBRARY_PATH` to the library location, or `$prefix/lib`
-- `CPATH` either to the `src` directory or the `$prefix/include`
+* `LIBRARY_PATH`, `LD_LIBRARY_PATH` to the library location, or `$prefix/lib`
+* `CPATH` either to the `src` directory or the `$prefix/include`
 
 The preCICE documentation provides more informaiton on [linking preCICE](https://precice.org/installation-linking.html).
 
-## Using Spack
+### Using Spack
 
 You can also install the python language bindings for preCICE via Spack by installing the Spack package `py-pyprecice`. Refer to [our installation guide for preCICE via Spack](https://precice.org/installation-spack.html) for getting started with Spack.
 
-## Using setup.py
+### Using setup.py
 
-### preCICE system installs
+#### preCICE system installs
 
 In this directory, execute:
-```
+
+```bash
 $ python3 setup.py install --user
 ```
 
-### preCICE at custom location (setting PATHS)
+#### preCICE at custom location (setting PATHS)
 
 see above. Then run
-```
+
+```bash
 $ python3 setup.py install --user
 ```
 
-### preCICE at custom location (explicit include path, library path)
+#### preCICE at custom location (explicit include path, library path)
 
 1. Install cython and other dependencies via pip3
-   ```
+
+   ```bash
    $ pip3 install --user setuptools wheel cython packaging numpy
    ```
+
 2. Open terminal in this folder.
 3. Build the bindings
-   ```
+
+   ```bash
    $ python3 setup.py build_ext --include-dirs=$PRECICE_ROOT/src --library-dirs=$PRECICE_ROOT/build/last
    ```
 
-  **Options:**
-  - `--include-dirs=`, default: `''` 
-    Path to the headers of preCICE, point to the sources `$PRECICE_ROOT/src`, or the your custom install prefix `$prefix/include`.
-  
-  **NOTES:**
-  
-  - If you have built preCICE using CMake, you can pass the path to the CMake binary directory using `--library-dirs`.
-  - It is recommended to use preCICE as a shared library here.
+   **Options:**
+   * `--include-dirs=`, default: `''`
+     Path to the headers of preCICE, point to the sources `$PRECICE_ROOT/src`, or the your custom install prefix `$prefix/include`.
+
+   **NOTES:**
+
+   * If you have built preCICE using CMake, you can pass the path to the CMake binary directory using `--library-dirs`.
+   * It is recommended to use preCICE as a shared library here.
 
 4. Install the bindings
-   ```
+
+   ```bash
    $ python3 setup.py install --user
    ```
 
-5. Clean-up _optional_
-   ```
+5. Clean-up *optional*
+
+   ```bash
    $ python3 setup.py clean --all
    ```
 
-# Test the installation
+## Test the installation
 
 Update `LD_LIBRARY_PATH` such that python can find `precice.so`
 
-```
+```bash
 $ export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:$PRECICE_ROOT/build/last
 ```
 
 Run the following to test the installation:
 
-```
+```bash
 $ python3 -c "import precice"
 ```
 
-## Unit tests
+### Unit tests
 
-1. Clean-up __mandatory__ (because we must not link against the real `precice.so`, but we use a mocked version)
-   ```
+1. Clean-up **mandatory** (because we must not link against the real `precice.so`, but we use a mocked version)
+
+   ```bash
    $ python3 setup.py clean --all
    ```
 
 2. Set `CPLUS_INCLUDE_PATH` (we cannot use `build_ext` and the `--include-dirs` option here)
-   ```
+
+   ```bash
    $ export CPLUS_INCLUDE_PATH=$CPLUS_INCLUDE_PATH:$PRECICE_ROOT/src
    ```
 
 3. Run tests with
-   ```
+
+   ```bash
    $ python3 setup.py test
    ```
 
-# Usage
+## Usage
 
-You can find the documentation of the implemented interface in the file `precice.pyx`. For an example of how `pyprecice` can be used please refer to the [1D elastic tube example](https://precice.org/tutorials-elastic-tube-1d.html#python). 
+You can find the documentation of the implemented interface in the file `precice.pyx`. For an example of how `pyprecice` can be used please refer to the [1D elastic tube example](https://precice.org/tutorials-elastic-tube-1d.html#python).
 
 **Note** The python package that is installed is called `pyprecice`. It provides the python module `precice` that can be use in your code via `import precice`, for example.
 
-# Troubleshooting & miscellaneous
+## Troubleshooting & miscellaneous
 
 ### preCICE is not found
 
 The following error shows up during installation, if preCICE is not found:
 
+```bash
+  /tmp/pip-install-d_fjyo1h/pyprecice/precice.cpp:643:10: fatal error: precice/Participant.hpp: No such file or directory
+    643 | #include "precice/Participant.hpp"
+        |          ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+  compilation terminated.
+  error: command 'x86_64-linux-gnu-gcc' failed with exit status 1
+  ----------------------------------------
+  ERROR: Failed building wheel for pyprecice
+Failed to build pyprecice
+ERROR: Could not build wheels for pyprecice which use PEP 517 and cannot be installed directly
 ```
+
+Or, for preCICE v2:
+
+```bash
   /tmp/pip-install-d_fjyo1h/pyprecice/precice.cpp:643:10: fatal error: precice/SolverInterface.hpp: No such file or directory
     643 | #include "precice/SolverInterface.hpp"
         |          ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~
   compilation terminated.
   error: command 'x86_64-linux-gnu-gcc' failed with exit status 1
   ----------------------------------------
   ERROR: Failed building wheel for pyprecice
@@ -186,31 +198,31 @@
 
 ### Version of Cython is too old
 
 In case the compilation fails with `shared_ptr.pxd not found` messages, check if you use the latest version of Cython.
 
 ### `Python.h` missing
 
-```
+```bash
 $ python3 -m pip install pyprecice
 Collecting pyprecice
 ...
   /tmp/pip-build-7rj4_h93/pyprecice/precice.cpp:25:20: fatal error: Python.h: No such file or directory
   compilation terminated.
   error: command 'x86_64-linux-gnu-gcc' failed with exit status 1
 
   ----------------------------------------
-  Failed building wheel for pyprecice 
+  Failed building wheel for pyprecice
 ```
 
 Please try to install `python3-dev`. E.g. via `apt install python3-dev`. Please make sure that you use the correct version (e.g. `python3.5-dev` or `python3.6-dev`). You can check your version via `python3 --version`.
 
 ### `libprecice.so` is not found at runtime
 
-```
+```bash
 $ python3 -c "import precice"
 Traceback (most recent call last):
   File "<stdin>", line 1, in <module>
 ImportError: libprecice.so.2: cannot open shared object file: No such file or directory
 ```
 
 Make sure that your `LD_LIBRARY_PATH` includes the directory that contains `libprecice.so`. The actual path depends on how you installed preCICE. Example: If preCICE was installed using `sudo make install` and you did not define a `CMAKE_INSTALL_PREFIX` the library path is `/usr/local/lib`. This means you have to `export LD_LIBRARY_PATH=/usr/local/lib:$LD_LIBRARY_PATH`.
@@ -224,81 +236,94 @@
 *Note that the instructions in this section are outdated and refer to the deprecated python bindings. Until we have updated information on the installation procedure for the python bindings under this use-case, we will keep these instructions, since they might still be very useful* (Originally contributed by [huangq1234553](https://github.com/huangq1234553) to the precice wiki in [`precice/precice/wiki:8bb74b7`](https://github.com/precice/precice/wiki/Dependencies/8bb74b78a7ebc54983f4822af82fb3d638021faa).)
 
 <details><summary>show details</summary>
 
 This guide provides steps to install python bindings for precice-1.6.1 for a conda environment Python 2.7.17 on the CoolMUC. Note that preCICE no longer supports Python 2 after v1.4.0. Hence, some modifications to the python setup code was necessary. Most steps are similar if not identical to the basic guide without petsc or python above. This guide assumes that the Eigen dependencies have already been installed.
 
 Load the prerequisite libraries:
-```
+
+```bash
 module load gcc/7
 module unload mpi.intel
 module load mpi.intel/2018_gcc
 module load cmake/3.12.1
 ```
+
 At the time of this writing `module load boost/1.68.0` is no longer available. Instead
-boost 1.65.1 was installed per the `boost and yaml-cpp` guide above. 
+boost 1.65.1 was installed per the `boost and yaml-cpp` guide above.
 
 In order to have the right python dependencies, a packaged conda environment was transferred to
 SuperMUC. The following dependencies were installed:
-- numpy
-- mpi4py
+
+* numpy
+* mpi4py
 
 With the python environment active, we have to feed the right python file directories to the cmake command.
 Note that -DPYTHON_LIBRARY expects a python shared library. You can likely modify the version to fit what is required.
-```
+
+```bash
 mkdir build && cd build
 cmake -DBUILD_SHARED_LIBS=ON -DPRECICE_PETScMapping=OFF -DPRECICE_PythonActions=ON -DCMAKE_INSTALL_PREFIX=/path/to/precice -DCMAKE_BUILD_TYPE=Debug .. -DPYTHON_INCLUDE_DIR=$(python -c "from distutils.sysconfig import get_python_inc; print(get_python_inc())")  -DPYTHON_LIBRARY=$(python -c "import distutils.sysconfig as sysconfig; print(sysconfig.get_config_var('LIBDIR')+'/libpython2.7.so')") -DNumPy_INCLUDE_DIR=$(python -c "import numpy; print(numpy.get_include())")
 make -j 12
 make install
 ```
+
 After installing, make sure you add the preCICE installation paths to your `.bashrc`, so that other programs can find it:
-```
+
+```bash
 export PRECICE_ROOT="path/to/precice_install"
 export PKG_CONFIG_PATH="path/to/precice_install/lib/pkgconfig:${PKG_CONFIG_PATH}"
 export CPLUS_INCLUDE_PATH="path/to/precice_install/include:${CPLUS_INCLUDE_PATH}"
 export LD_LIBRARY_PATH="path/to/precice_install/lib:${LD_LIBRARY_PATH}"
 ```
+
 Then, navigate to the python_future bindings script.
-```
+
+```bash
 cd /path/to/precice/src/precice/bindings/python_future
 ```
+
 Append the following to the head of the file to allow Python2 to run Python3 code. Note that
-importing `unicode_literals` from `future` will cause errors in `setuptools` methods as string literals 
+importing `unicode_literals` from `future` will cause errors in `setuptools` methods as string literals
 in code are interpreted as `unicode` with this import.
-```
+
+```python
 from __future__ import (absolute_import, division,
                         print_function)
 from builtins import (
          bytes, dict, int, list, object, range, str,
          ascii, chr, hex, input, next, oct, open,
          pow, round, super,
          filter, map, zip)
 ```
+
 Modify `mpicompiler_default = "mpic++"` to `mpicompiler_default = "mpicxx"` in line 100.
 Run the setup file using the default Python 2.7.17.
-```
+
+```bash
 python setup.py install --user
 ```
+
 </details>
 
 ### ValueError while importing preCICE
+
 If you face the error:
 
 ```bash
 ValueError: numpy.ndarray size changed, may indicate binary incompatibility. Expected 88 from C header, got 80 from PyObject
 ```
 
 make sure that you are using an up-to-date version of NumPy. You can update NumPy with
 
 ```bash
 pip3 install numpy --upgrade
 ```
 
-
-# Contributors
+## Contributors
 
 * [Benjamin Rodenberg](https://github.com/BenjaminRodenberg)
 * [Ishaan Desai](https://github.com/IshaanDesai)
 * [Saumitra Vinay Joshi](https://github.com/saumiJ) contributed first working prototype in [`3db9c9` on `precice/precice`](https://github.com/precice/precice/commit/3db9c95e527db1e1cacb2fd116a5ce13ee877513)
 * [Frédéric Simonis](https://github.com/fsimonis)
 * [Florian Lindner](https://github.com/floli)
 * [Benjamin Uekermann](https://github.com/uekerman)
```

### Comparing `pyprecice-2.5.0.2/setup.py` & `pyprecice-3.0.0.0.dev0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,27 +60,27 @@
 
 PYTHON_BINDINGS_PATH = os.path.dirname(os.path.abspath(__file__))
 
 
 def get_extensions(is_test):
     compile_args = []
     link_args = []
-    compile_args.append("-std=c++11")
+    compile_args.append("-std=c++17")
     compile_args.append("-I{}".format(numpy.get_include()))
 
     bindings_sources = [os.path.join(PYTHON_BINDINGS_PATH, "cyprecice",
                                      "cyprecice" + ".pyx")]
 
     compile_args += pkgconfig.cflags('libprecice').split()
 
     if not is_test:
         link_args += pkgconfig.libs('libprecice').split()
     if is_test:
         bindings_sources.append(os.path.join(PYTHON_BINDINGS_PATH, "test",
-                                             "SolverInterface.cpp"))
+                                             "Participant.cpp"))
 
     return [
         Extension(
             "cyprecice",
             sources=bindings_sources,
             libraries=[],
             language="c++",
```

### Comparing `pyprecice-2.5.0.2/versioneer.py` & `pyprecice-3.0.0.0.dev0/versioneer.py`

 * *Files identical despite different names*

