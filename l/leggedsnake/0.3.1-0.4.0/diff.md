# Comparing `tmp/leggedsnake-0.3.1.tar.gz` & `tmp/leggedsnake-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leggedsnake-0.3.1.tar", last modified: Wed Jun 14 07:18:29 2023, max compression
+gzip compressed data, was "leggedsnake-0.4.0.tar", last modified: Wed Jun 21 08:01:59 2023, max compression
```

## Comparing `leggedsnake-0.3.1.tar` & `leggedsnake-0.4.0.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:18:29.311823 leggedsnake-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18995 2023-06-14 07:18:29.311823 leggedsnake-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9930 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:18:29.307823 leggedsnake-0.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/docs/.buildinfo
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/docs/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)    28583 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/docs/changeloglink.html
--rw-r--r--   0 runner    (1001) docker     (123)    25259 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/docs/genindex.html
--rw-r--r--   0 runner    (1001) docker     (123)    30647 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/docs/objects.inv
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/docs/py-modindex.html
--rw-r--r--   0 runner    (1001) docker     (123)    27009 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/docs/readmelink.html
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/docs/search.html
--rw-r--r--   0 runner    (1001) docker     (123)    16337 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/docs/searchindex.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:18:29.311823 leggedsnake-0.3.1/leggedsnake/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/leggedsnake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22721 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/leggedsnake/dynamiclinkage.py
--rw-r--r--   0 runner    (1001) docker     (123)    14809 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/leggedsnake/geneticoptimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17294 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/leggedsnake/physicsengine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/leggedsnake/show_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/leggedsnake/utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/leggedsnake/walker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:18:29.311823 leggedsnake-0.3.1/leggedsnake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18995 2023-06-14 07:18:29.000000 leggedsnake-0.3.1/leggedsnake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-14 07:18:29.000000 leggedsnake-0.3.1/leggedsnake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 07:18:29.000000 leggedsnake-0.3.1/leggedsnake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-14 07:18:29.000000 leggedsnake-0.3.1/leggedsnake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 07:18:29.000000 leggedsnake-0.3.1/leggedsnake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-14 07:18:29.311823 leggedsnake-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:18:29.311823 leggedsnake-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-14 07:18:19.000000 leggedsnake-0.3.1/tests/test_utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:01:59.389962 leggedsnake-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-06-21 08:01:48.000000 leggedsnake-0.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-06-21 08:01:48.000000 leggedsnake-0.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-21 08:01:48.000000 leggedsnake-0.4.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-21 08:01:48.000000 leggedsnake-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10557 2023-06-21 08:01:59.389962 leggedsnake-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9070 2023-06-21 08:01:48.000000 leggedsnake-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:01:59.385962 leggedsnake-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-21 08:01:48.000000 leggedsnake-0.4.0/docs/.buildinfo
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:01:48.000000 leggedsnake-0.4.0/docs/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)    28583 2023-06-21 08:01:48.000000 leggedsnake-0.4.0/docs/changeloglink.html
+-rw-r--r--   0 runner    (1001) docker     (123)    25259 2023-06-21 08:01:48.000000 leggedsnake-0.4.0/docs/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)    30647 2023-06-21 08:01:48.000000 leggedsnake-0.4.0/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-21 08:01:48.000000 leggedsnake-0.4.0/docs/objects.inv
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-06-21 08:01:48.000000 leggedsnake-0.4.0/docs/py-modindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)    27009 2023-06-21 08:01:48.000000 leggedsnake-0.4.0/docs/readmelink.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-06-21 08:01:48.000000 leggedsnake-0.4.0/docs/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16337 2023-06-21 08:01:48.000000 leggedsnake-0.4.0/docs/searchindex.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:01:59.385962 leggedsnake-0.4.0/leggedsnake/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-21 08:01:48.000000 leggedsnake-0.4.0/leggedsnake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22742 2023-06-21 08:01:48.000000 leggedsnake-0.4.0/leggedsnake/dynamiclinkage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12828 2023-06-21 08:01:48.000000 leggedsnake-0.4.0/leggedsnake/geneticoptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-06-21 08:01:48.000000 leggedsnake-0.4.0/leggedsnake/physicsengine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-21 08:01:48.000000 leggedsnake-0.4.0/leggedsnake/show_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-21 08:01:48.000000 leggedsnake-0.4.0/leggedsnake/utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-06-21 08:01:48.000000 leggedsnake-0.4.0/leggedsnake/walker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13467 2023-06-21 08:01:48.000000 leggedsnake-0.4.0/leggedsnake/worldvisualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:01:59.389962 leggedsnake-0.4.0/leggedsnake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10557 2023-06-21 08:01:59.000000 leggedsnake-0.4.0/leggedsnake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-21 08:01:59.000000 leggedsnake-0.4.0/leggedsnake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 08:01:59.000000 leggedsnake-0.4.0/leggedsnake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-21 08:01:59.000000 leggedsnake-0.4.0/leggedsnake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 08:01:59.000000 leggedsnake-0.4.0/leggedsnake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 08:01:59.000000 leggedsnake-0.4.0/leggedsnake.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-21 08:01:48.000000 leggedsnake-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-21 08:01:59.389962 leggedsnake-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-21 08:01:48.000000 leggedsnake-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:01:59.389962 leggedsnake-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-21 08:01:48.000000 leggedsnake-0.4.0/tests/test_utility.py
```

### Comparing `leggedsnake-0.3.1/CHANGELOG.md` & `leggedsnake-0.4.0/CHANGELOG.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,67 @@
 # Changelog
 
 All notable changes to the LeggedSnake will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.4.0] - 2023-06-21
+
+### Added in 0.4.0
+
+- View all walkers!
+  - ``show_all_walkers`` in ``docs/examples/strider.py`` let you see all walkers in one simulation!
+  - You can set the color of walkers during display.
+- Genetic optimization:
+  - ``GeneticOptimization`` class in ``geneticoptimizer.py`` that will replace the previous functional paradigm.
+  - The average score is now displayed.
+- ``VisualWorld`` has a new method called ``reload_visuals``.
+- ``show_evolution.py`` is a new script plotting various data about the Walkers population's evolution during 
+genetic optimization.
+- In ``docs/examples/strider.py`` we recommend to use ``total_distance`` as the fitness function.
+
+### Changed in 0.4.0
+
+- Genetic optimization:
+  - During genetic optimization, population is now stable at max_pop (it used to fluctuate a lot).
+  - Genetic optimization do no longer display all dimensions in the progress bar.
+  - ``startnstop`` argument may now be the name of the file to use (a string).
+  - ``max_genetic_distance`` was changed from 0.7 to 10. Results are much better now!
+- Visuals:
+  - ``update`` method of ``VisualWorld`` replaced by ``visual_update``. It clearly separates physics and display time.
+  - Frame rate and physics speed are now independent parameters.
+  - Visuals go to a new file ``worldvisualizer.py``.
+  - Camera parameters should now be accessed from ``CAMERA`` instead of ``params["camera"]``.
+  - The camera feels more cinematic.
+- You can define a custom load when using ``World.add_linkage`` or ``VisualWorld.add_linkage``. The default is 0.
+- ``pyproject.toml`` updated with the data of ``setup.cfg``. This is now the recommended metadata for the project. 
+- In ``docs/example/strider.py``, simulation time was increased from 30 seconds to 40. It was just not enough.
+
+### Fixed in 0.4.0
+
+- Documentation of ``evolutionary_optimization_builtin`` was wrong: returned data were in order (fitness, dimensions, position),
+but (fitness, position, dimensions) was indicated.
+- After a genetic optimization, the example script was assigning wrong data to the demo walker.
+- ``kwargs_switcher`` from ``geneticoptimizer.py`` do no longer pop (destroy) argument from the input dictionary.
+
+### Deprecated in 0.4.0
+
+- ``setup.cfg`` should no longer be used, as it is replaced by ``pyproject.toml``. 
+
+### Removed in 0.4.0
+
+- ``evolutionary_optimization`` function is removed. Use  ``GeneticOptimization`` class instead.
+  - You can no longer use the argument "init_pop" to change the size of the initial population. 
+  It now always set to max_pop.
+- ``time_coef``, ``calc_rate`` and ``max_sub`` parameters of ``params["simul"]`` replaced by a unique 
+``physics_period`` set to 0.02 (s).
+- ``leggedsnake/Population evolution.json`` removed. 
+It contained data about an evolution run and is not relevant for users.
+
 ## [0.3.1] - 2023-06-14
 
 Starting from 0.3.1, we won't include "-alpha" or "-beta" in the naming scheme,
 as it is considered irrelevant.
 
 ### Added in 0.3.1
```

### Comparing `leggedsnake-0.3.1/CODE_OF_CONDUCT.md` & `leggedsnake-0.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `leggedsnake-0.3.1/LICENSE.rst` & `leggedsnake-0.4.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `leggedsnake-0.3.1/README.md` & `leggedsnake-0.4.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,194 +1,230 @@
+Metadata-Version: 2.1
+Name: leggedsnake
+Version: 0.4.0
+Summary: Simulate and optimize planar leg mechanisms using PSO and GA
+Home-page: https://hugofara.github.io/leggedsnake/
+Author: Hugo Farajallah
+Author-email: Hugo Farajallah <leggedsnake@hugofara.net>
+License: MIT License
+Project-URL: Homepage, https://hugofara.net/leggedsnake-retro-ingeneering-evolution/
+Project-URL: Documentation, https://github.com/HugoFara/leggedsnake/blob/main/CHANGELOG.md
+Project-URL: Repository, https://github.com/HugoFara/leggedsnake
+Project-URL: Changelog, https://github.com/me/spam/blob/master/CHANGELOG.md
+Keywords: linkage,leg mechanism,optimization,leggedsnake,walking linkage
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Artificial Life
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Legal Industry
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.rst
+
 # leggedsnake
 
 [![PyPI version fury.io](https://badge.fury.io/py/leggedsnake.svg)](https://pypi.python.org/pypi/leggedsnake/)
 [![Downloads](https://static.pepy.tech/personalized-badge/leggedsnake?period=total&units=international_system&left_color=grey&right_color=green&left_text=downloads)](https://pepy.tech/project/leggedsnake)
-[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg )](https://raw.githubusercontent.com/HugoFara/leggedsnake/master/LICENSE.rst)
+[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg )](https://raw.githubusercontent.com/HugoFara/leggedsnake/main/LICENSE.rst)
 
-LeggedSnake is a project intended to make the simulation of walking linkages fast and easy. 
+LeggedSnake makes the simulation of walking linkages fast and easy.
 We believe that building walking linkages is fun and could be useful.
 Our philosophy is to provide a quick way of building, optimizing and testing walking linkages.
 
-We handle planar [leg mechanisms](https://en.wikipedia.org/wiki/Leg_mechanism) in three main parts:
+## Overview
 
-* Linkage conception in simple Python relying on [pylinkage](https://github.com/HugoFara/pylinkage).
-* Kinematic optimization with ``Walker`` class, inheriting from pylinkage's ``Linkage`` class.
-* Dynamic simulation and its optimization using genetic algorithms.
+First, you will define a linkage to be optimized. 
+Here we use the [strider linkage](https://www.diywalkers.com/strider-linkage-plans.html) by [Wade Wagle and Team Trotbot](https://www.diywalkers.com/).
 
-## Quick links
 
-* For the documentation, check the docs at [hugofara.github.io/leggedsnake](https://hugofara.github.io/leggedsnake/)!
-* Source code is hosted on GitHub as [HugoFara/leggedsnake](https://github.com/HugoFara/leggedsnake)
-* We also provide a Python package on PyPi, test [leggedsnake](https://pypi.org/project/leggedsnake/).
-* If you just want to chill out looking at walking linkages striving to survive, join the [discussions](https://github.com/HugoFara/leggedsnake/discussions).
-
-Contributors are welcome!
+![Dynamic four-leg-pair unoptimized Strider](https://github.com/HugoFara/leggedsnake/raw/main/docs/examples/images/Dynamic%20unoptimized%20strider.gif)
 
-## Installation
+*Dimensions are intentionally wrong, so that the robots fails to walk properly.*
 
-### Using pip
+Let's take several identical linkages, and make them reproduce and evolve through many generations.
+Here is how it looks:
 
-The package is hosted on PyPi as [leggedsnake](https://pypi.org/project/leggedsnake/), use:
+![10 optimized striders](https://github.com/HugoFara/leggedsnake/raw/main/docs/examples/images/Striders%20run.gif)
 
-```bash
-pip install leggedsnake
-```
+Finally, we will extract the best linkage, and here is our optimized model that do not fall.
 
-### Setting up Virtual Environment
+![Dynamic optimized Strider](https://github.com/HugoFara/leggedsnake/raw/main/docs/examples/images/Dynamic%20optimized%20strider.gif)
 
-We provide an [environment.yml](https://github.com/HugoFara/leggedsnake/blob/master/environment.yml) file for conda. 
-Use ``conda env update --file environment.yml --name leggedsnake-env`` to install the requirements in a separate environment.
 
-If you are looking for a development version, check the GitHub repo under 
-[HugoFara/leggedsnake](https://github.com/HugoFara/leggedsnake).
+## Installation
 
+The package is hosted on PyPi as [leggedsnake](https://pypi.org/project/leggedsnake/), use:
 
-## Contribute
+```bash
+pip install leggedsnake
+```
 
-Download the latest GitHub version, then install the dev requirements in ``requirements-dev.txt``.
+## Build from source
 
-In a nutshell
+Download this repository.
 
-```bash
-git clone https://github.com/HugoFara/leggedsnake.git
-cd leggedsnake
-pip install -r requirements-dev.txt
+```shell
+git clone https://github.com/hugofara/leggedsnake
 ```
 
-### Testing
+### Conda Virtual Environment
 
-We use unittest. Just run ``python3 -m unittest discover .`` from the main folder.
+We provide an [environment.yml](https://github.com/HugoFara/leggedsnake/blob/main/environment.yml) file for conda.
 
-### Release
+```shell
+conda env update --file environment.yml --name leggedsnake-env
+``` 
+It will install the requirements in a separate environment.
 
-This section is mainly intended for maintainers. 
-Fell free to use the tools described here, but they are not necessary in any way.
+### Other installation
 
-* To publish a new version, use ``bump2version``. For instance ``bump2version minor``.
-* Regenerate the documentation with ``make html`` (uses Sphinx).
+If you are looking for a development version, check the GitHub repo under
+[HugoFara/leggedsnake](https://github.com/HugoFara/leggedsnake).
 
 ## Usage
 
-The demo script is [strider.py](https://github.com/HugoFara/leggedsnake/blob/master/docs/examples/strider.py), which
+First, you define the linkage you want to use. 
+The demo script is [strider.py](https://github.com/HugoFara/leggedsnake/blob/main/docs/examples/strider.py), which
 demonstrates all the techniques about the [Strider linkage](https://www.diywalkers.com/strider-linkage-plans.html).
 
-### Defining a ``Walker``
+In a nutshell, the two main parts are:
+
+1. Define a Linkage.
+2. Run the optimization. 
 
-First, you need to define joints for your ``Walker`` as described in [pylinkage](https://github.com/HugoFara/pylinkage)
-documentation. Once your joints (let's say they are in a joint object), you should have something like that:
 
+### Defining a ``Walker``
+you need to define joints for your ``Walker`` as described in [pylinkage](https://github.com/HugoFara/pylinkage)
+documentation. 
+You may use a dictionary, that looks like that:
 ```python3
 import leggedsnake as ls
 
-# Center of the Walker
+# Quick definition of a linkage as a dict of joints
 linkage = {
     "A": ls.Static(x=0, y=0, name="A"),
     "B": ls.Crank(1, 0, distance=1, angle=0.31, name="Crank")
     # etc...
 }
+# Conversion to a dynamic linkage
 my_walker = ls.Walker(
     joints=linkage.values(),
     name="My Walker"
 )
-```
+# It is often faster to add pairs of legs this way
+my_walker.add_legs(3)
 
-``Walker`` is just an inherited class of ``Linkage``, with some useful methods, and behaves quite the same way.
 
-### Kinematic optimization using Particle Swarm Optimization (PSO)
+# Then, run launch a GUI simulation with
+ls.video(my_walker)
+```
+It should display something like the following.
 
-No change compared to a classic linkage optimization. You should use the ``step`` and ``stride`` method from the 
-[utility module](https://github.com/HugoFara/leggedsnake/blob/master/leggedsnake/utility.py) as fitness functions.
-This set of rules should work well for a stride **maximisation** problem:
+![Dynamic four-leg-pair unoptimized Strider](https://github.com/HugoFara/leggedsnake/raw/main/docs/examples/images/Dynamic%20unoptimized%20strider.gif)
 
-1. Rebuild the Walker with the provided set of dimensions, and do a complete turn.
-2. If the Walker raises an UnbuildableError, its score is 0 (or ``-float('inf')`` if you use other evaluation functions).
-3. Verify if it can pass a certain obstacle using ``step`` function. If not, its score is 0.
-4. Eventually measure the length of its stride with the ``stride`` function. Return this length as its score.
 
-### Dynamic Optimization using Genetic Algorithm (GA)
+### Optimization using Genetic Algorithm (GA)
 
-Kinematic optimization is fast, but it can return weird results, and it has no sense of gravity while walking heavily
-relies on gravity. This is why you may need to use dynamic optimization thanks to
-[Pymunk](http://www.pymunk.org/en/latest/index.html). However, the calculation is much slower, and you can no
-longer test millions of linkages as in PSO (or you will need time). This is why we
-use [genetic algorithm](https://en.wikipedia.org/wiki/Genetic_algorithm), because it can provide good results with
-fewer parents.
-
-We handle everything almost everything world definition to linkage conversion. Apart from the GA parameters, you just
-have to define a fitness function. Here are the main steps for a **maximisation problem**:
-
-1. Create a function of two arguments, the first one should be the parameters of the linkage, the second the initial positions for the joints.
-2. Try to do a revolution in **kinematic simulation**. If the Walker raises an ``UnbuildableError`` set its score to ``-float('inf')``.
-3. Otherwise, use the following procedure:
+The next step is to optimize your linkage. We use a genetic algorithm here.
 
-```python3
-import leggedsnake as ls
+```python
+# Definition of an individual as (fitness, dimensions, initial coordinates)
+dna = [0, list(my_walker.get_num.constraints()), list(my_walker.get_coords())]
+population = 10
 
-def dynamic_linkage_fitness(walker):
+def total_distance(walker):
     """
-    Make the dynamic evaluation of a Walker.
+    Evaluates the final horizontal position of the input linkage.
     
-    Return yield and initial position of joints.
+    Return final distance and initial position of joints.
     """
+    pos = tuple(walker.step())[-1]
     world = ls.World()
     # We handle all the conversions
     world.add_linkage(walker)
     # Simulation duration (in seconds)
     duration = 40
-    # Somme of yields
-    tot = 0
-    # Motor turned on duration
-    dur = 0
-    n = duration * ls.params["camera"]["fps"]
-    n /= ls.params["simul"]["time_coef"]
-    pos = tuple(walker.step())[-1]
-    for j in range(int(n)):
-        efficiency, energy = world.update(j)
-        tot += efficiency
-        dur += energy
-    if dur == 0:
-        return - float('inf'), list()
-    print("Score:", tot / dur)
-    # Return 100 times average yield, and initial positions as the final score
-    return tot / dur, pos
-```
-
-And now, relax while your computer creates a civilization of walking machines!
+    steps = int(duration / ls.params["simul"]["physics_period"])
+    for _ in range(steps):
+        world.update()
+    return world.linkages[0].body.position.x, pos
 
-### Visualization
 
-For this part we will focus on the [Strider linkage](https://www.diywalkers.com/strider-linkage-plans.html), 
-an example file is provided at ``docs/examples/strider.py``.
+# Prepare the optimization, with any fitness_function(dna) -> score 
+optimizer = ls.GeneticOptimization(
+        dna=dna, 
+        fitness=total_distance,
+        max_pop=population,
+)
+# Run for 100 iterations, on 4 processes
+optimized_walkers = optimizer.run(iters=100, processes=4)
 
-The linkage looks like this:
-![A Kinematic representation of Strider linkage](https://github.com/HugoFara/leggedsnake/raw/master/docs/examples/images/Kinematic%20unoptimized%20Strider.gif)
+# The following line will display the results
+ls.all_linkages_video(optimized_walkers)
+```
+For 100 iterations, 10 linkages will be simulated and evaluated by fitness_function.
+The fittest individuals are kept and will propagate their genes (with mutations).
 
-Looks cool? Let's simulate it dynamically!
+Now you should see something like the following.
 
-![Dynamic one-leg-pair Strider being tested](https://github.com/HugoFara/leggedsnake/raw/master/docs/examples/images/Dynamic%20unoptimized%20one-legged%20Strider.gif)
+![10 optimized striders](https://github.com/HugoFara/leggedsnake/raw/main/docs/examples/images/Striders%20run.gif)
 
-Oops! Here is what you get when you forget to add more legs! There is **real danger here**, because your walker crawls
-well, you will be able to optimize efficiently the "crawler", *which may be not your goal*.
+This is a simulation from the last generation of 10 linkages. 
+Most of them cover a larger distance (this is the target of our ``fitness_function``).
 
-Let's add three more leg pairs. Why three? Many legs mean more mass and constraints, so less yield and more intensive
-computations. On the other hand, we always want the center of mass over the
-[support line](https://en.wikipedia.org/wiki/Support_polygon), which means that if the walker begins to lift a foot
-(let's say a front foot), and another doesn't come on the ground ahead of it, the linkage will fall nose to the
-ground. With more feet, we make the "snooping" time shorter, and a total of four leg pairs is a minimum for this
-*unoptimized* version.
+### Results
 
-A simple way to do it is:
+Finally, only the best linkage at index 0 may be kept.
 
 ```python
-my_linkage.add_legs(3) # Replace "my_linkage" with your Walker object
+# Results are sorted by best fitness first, 
+# so we use the walker with the best score
+best_dna = optimized_walkers[0]
+
+# Change the dimensions
+my_walker.set_num_constraints(best_dna[1])
+my_walker.set_coords(best_dna[2])
+
+# Once again launch the video
+ls.video(my_walker)
 ```
 
-Let's have a look at the artist:
+![Dynamic optimized Strider](https://github.com/HugoFara/leggedsnake/raw/main/docs/examples/images/Dynamic%20optimized%20strider.gif)
+
+So now it has a small ski pole, does not fall and goes much farther away!
+
+### Kinematic optimization using Particle Swarm Optimization (PSO)
+
+You may need a kinematic optimization, depending solely on pylinkage. 
+You should use the ``step`` and ``stride`` method from the
+[utility module](https://github.com/HugoFara/leggedsnake/blob/main/leggedsnake/utility.py) as fitness functions.
+This set of rules should work well for a stride **maximisation** problem:
+
+1. Rebuild the Walker with the provided set of dimensions, and do a complete turn.
+2. If the Walker raises an UnbuildableError, its score is 0 (or ``-float('inf')`` if you use other evaluation functions).
+3. Verify if it can pass a certain obstacle using ``step`` function. If not, its score is 0.
+4. Eventually measure the length of its stride with the ``stride`` function. Return this length as its score.
 
-![Dynamic four-leg-pair unoptimized Strider](https://github.com/HugoFara/leggedsnake/raw/master/docs/examples/images/Dynamic%20unoptimized%20strider.gif)
+## Main features
+
+We handle planar [leg mechanisms](https://en.wikipedia.org/wiki/Leg_mechanism) in three main parts:
+
+* Linkage conception in simple Python relies on [pylinkage](https://github.com/HugoFara/pylinkage).
+* *Optional* kinematic optimization with ``Walker`` class, inherits from pylinkage's ``Linkage`` class.
+* Dynamic simulation and its optimization use genetic algorithms.
 
 ## Advice
 
 Use the visualisation tools provided! The optimization tools should always give you a score with a better fitness,
 but it might not be what you expected. Tailor your optimization and *then* go for a long run will make you save a lot
 of time.
 
@@ -196,24 +232,33 @@
 several mechanisms to prevent that (starting from random position), but it can always have an impact on the rest of
 the optimization.
 
 Try to minimize the number of elements in the optimizations! You can often use some linkage properties to reduce the
 number of simulation parameters. For instance, the Strider linkage has axial symmetry. While it is irrelevant to use
 this property in dynamic simulation, you can use "half" your Strider in a kinematic optimization, which is much faster.
 
-![A Kinematic half Strider](https://github.com/HugoFara/leggedsnake/raw/master/docs/examples/images/Kinematic%20half-Strider.gif)
+![A Kinematic half Strider](https://github.com/HugoFara/leggedsnake/raw/main/docs/examples/images/Kinematic%20half-Strider.gif)
+
+## Contribute
+
+This project is open to contribution and actively looking for contributors.
+You can help making it better!
+
+### For everyone
+
+You can [drop a star](https://github.com/HugoFara/leggedsnake/stargazers),
+[fork this project](https://github.com/HugoFara/leggedsnake/forks) or simply share the link to your best media.
+
+The more people get engaged into this project, the better it will develop!
 
-## Requirements
+### For developers
 
-Python 3, numpy for calculation, matplotlib for drawing, and standard libraries.
+You can follow the guide at [CONTRIBUTING.md](CONTRIBUTING.md). Feel free to me any pull request.
 
-For kinematic optimization, you can either use the built-in algorithm, or
-[PySwarms](https://pyswarms.readthedocs.io/en/latest/), under MIT license. 
-PySwarms is a much more complex package which provides quick calculations, 
-however, with modern laptops the built-in swarm optimization should be quick enough
-to fit your needs.
-
-Dynamic optimization relies on multiple packages.
-First of all, it uses [Pymunk](http://www.pymunk.org/en/latest/index.html),
-made by Victor Blomqvist, as its physics engine. 
-The genetic algorithm optimizer is home-made, 
-but feel free to use any external tool suiting your needs!
+## Quick links
+
+* For the documentation, check the docs at [hugofara.github.io/leggedsnake](https://hugofara.github.io/leggedsnake/)!
+* Source code is hosted on GitHub as [HugoFara/leggedsnake](https://github.com/HugoFara/leggedsnake)
+* We also provide a Python package on PyPi, test [leggedsnake](https://pypi.org/project/leggedsnake/).
+* If you just want to chill out looking at walking linkages striving to survive, join the [discussions](https://github.com/HugoFara/leggedsnake/discussions).
+
+Contributors are welcome!
```

### Comparing `leggedsnake-0.3.1/docs/changeloglink.html` & `leggedsnake-0.4.0/docs/changeloglink.html`

 * *Files identical despite different names*

### Comparing `leggedsnake-0.3.1/docs/genindex.html` & `leggedsnake-0.4.0/docs/genindex.html`

 * *Files identical despite different names*

### Comparing `leggedsnake-0.3.1/docs/index.html` & `leggedsnake-0.4.0/docs/index.html`

 * *Files identical despite different names*

### Comparing `leggedsnake-0.3.1/docs/objects.inv` & `leggedsnake-0.4.0/docs/objects.inv`

 * *Files identical despite different names*

### Comparing `leggedsnake-0.3.1/docs/py-modindex.html` & `leggedsnake-0.4.0/docs/py-modindex.html`

 * *Files identical despite different names*

### Comparing `leggedsnake-0.3.1/docs/readmelink.html` & `leggedsnake-0.4.0/docs/readmelink.html`

 * *Files identical despite different names*

### Comparing `leggedsnake-0.3.1/docs/search.html` & `leggedsnake-0.4.0/docs/search.html`

 * *Files identical despite different names*

### Comparing `leggedsnake-0.3.1/docs/searchindex.js` & `leggedsnake-0.4.0/docs/searchindex.js`

 * *Files identical despite different names*

### Comparing `leggedsnake-0.3.1/leggedsnake/__init__.py` & `leggedsnake-0.4.0/leggedsnake/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,20 +20,27 @@
     kinematic_minimization, kinematic_maximization,
     UnbuildableError, HypostaticError,
     show_linkage,
 )
 
 from .utility import step, stride
 from .walker import Walker
-from .geneticoptimizer import evolutionary_optimization
+from .geneticoptimizer import GeneticOptimization
 from .dynamiclinkage import (
     Nail, PinUp, DynamicPivot, Motor,
     DynamicLinkage,
     convert_to_dynamic_linkage,
 )
 from .physicsengine import (
-    video, video_debug,
     params,
-    World, VisualWorld
+    World,
 )
+from .worldvisualizer import (
+    all_linkages_video,
+    video,
+    video_debug,
+    VisualWorld,
+    CAMERA
+)
+from .show_evolution import load_data, show_genetic_optimization
 
-__version__ = "0.3.1"
+__version__ = "0.4.0"
```

### Comparing `leggedsnake-0.3.1/leggedsnake/dynamiclinkage.py` & `leggedsnake-0.4.0/leggedsnake/dynamiclinkage.py`

 * *Files 1% similar despite different names*

```diff
@@ -508,20 +508,24 @@
     empty shell in the ways you will use it.
 
     Please note that it carries a load, which is relevant with real-world
     simulation where the weight of legs is small compared to the weight of the
     frame.
     """
 
-    __slots__ = ['joint_to_rigidbodies', 'rigidbodies', 'body', 'height',
-                 'mechanical_energy', 'mass', 'space', 'density',
-                 '_thickness', 'filter']
-
-    def __init__(self, joints, space, density=1, load=0, name=None,
-                 thickness=.1):
+    __slots__ = [
+        'joint_to_rigidbodies', 'rigidbodies', 'body', 'height',
+        'mechanical_energy', 'mass', 'space', 'density',
+        '_thickness', 'filter'
+    ]
+
+    def __init__(
+            self, joints, space, density=1, load=0, name=None,
+            thickness=.1
+    ):
         """
         Instanciate a new DynamicLinkage.
 
         Parameters
         ----------
         joints : linkage.Joint
             Joints to be part of the linkage. Kinematic joints will be
@@ -585,32 +589,34 @@
             if isinstance(joint, DynamicJoint):
                 djoint = joint
             elif isinstance(joint, linkage.Static):
                 djoint = Nail(body=self.body, **common)
             # Joints with at least one reference
             else:
                 """
-                Useless while qe don't support quick joint definition
+                Useless while we don't support quick joint definition
                 if (
                         isinstance(joint.joint0, linkage.Static)
                         and joint.joint0 not in conversion_dict
                 ):
                     conversion_dict[joint.joint0] = joint.joint0
                 if (
                         hasattr(joint, "joint1")
                         and isinstance(joint.joint1, linkage.Static)
                         and joint.joint1 not in conversion_dict
                 ):
                     conversion_dict[joint.joint1] = joint.joint1
                 """
                 if isinstance(joint, linkage.Fixed):
-                    djoint = PinUp(distance=joint.r, angle=joint.angle,
-                                   joint0=conversion_dict[joint.joint0],
-                                   joint1=conversion_dict[joint.joint1],
-                                   **common)
+                    djoint = PinUp(
+                        distance=joint.r, angle=joint.angle,
+                        joint0=conversion_dict[joint.joint0],
+                        joint1=conversion_dict[joint.joint1],
+                        **common
+                    )
                 elif isinstance(joint, linkage.Crank):
                     djoint = Motor(
                         joint0=conversion_dict[joint.joint0],
                         distance=joint.r, angle=joint.angle,
                         **common
                     )
                 elif isinstance(joint, linkage.Pivot):
@@ -621,28 +627,32 @@
                         **common
                     )
             dynajoints.append(djoint)
             conversion_dict[joint] = djoint
         self.joints = tuple(dynajoints)
 
     def build_load(self, position, load_mass):
-        """Create the load this linkage have to carry."""
+        """Create the load this linkage has to carry."""
         load = pm.Body(load_mass)
         load.position = position
         vertices = (-.5, -.5), (-.5, .5), (.5, .5), (.5, -.5)
         segs = []
         for i, vertex in enumerate(vertices):
-            segs.append(pm.Segment(load, vertex,
-                                   vertices[(i + 1) % len(vertices)],
-                                   self._thickness))
-            segs[-1].density = self.density
+            segment = pm.Segment(
+                load, vertex, vertices[(i + 1) % len(vertices)],
+                self._thickness
+            )
+            segment.density = self.density
             # Rigidbodies in this group won't collide
-            segs[-1].filter = self.filter
+            segment.filter = self.filter
+            segs.append(segment)
         self.space.add(load, *segs)
         return load
 
 
 def convert_to_dynamic_linkage(kinematic_linkage, space, density=1,
                                load=1):
     """Convert a classic Linkage to its dynamic counterpart."""
-    return DynamicLinkage(kinematic_linkage.joints, space, density=density,
-                          load=load, name=kinematic_linkage.name)
+    return DynamicLinkage(
+        kinematic_linkage.joints, space, density=density,
+        load=load, name=kinematic_linkage.name
+    )
```

### Comparing `leggedsnake-0.3.1/leggedsnake/physicsengine.py` & `leggedsnake-0.4.0/leggedsnake/worldvisualizer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,470 +1,360 @@
-# -*- coding: utf-8 -*-
 """
-The physicsengine module gives a dynamic behavior to legged mechanism.
-
-It uses the 2D physics engine chipmunk, this is why it can only be used on
-planar mechanisms.
-In theory, you can use any type of mechanism, and not only planar mechanisms.
-In practice, we do generate the road and some other parameters as the gravity,
-so it can be difficult to test something other than a walker.
-
-Created on Sat May 25 2019 14:56:01.
-
-@author: HugoFara
+This file contains class and method to see the walkers in action.
 """
+from functools import partial
+import matplotlib.pyplot as plt
 import numpy as np
-import pymunk as pm
 import pymunk.matplotlib_util
-import matplotlib.pyplot as plt
-import matplotlib.animation as anim
-from pylinkage.geometry import norm, cyl_to_cart, bounding_box
-from pylinkage.linkage import Static, Crank, Fixed, Pivot
-
-from . import dynamiclinkage as dlink
-
-# Simulation parameters
-params = {
-    # Ground parameters
-    "ground": {
-        # Nominal slope (radian)
-        "slope": 10 * np.pi / 180,
-        # Maximal step height
-        "max_step": .5,
-        # Steps frequency
-        "step_freq": .1,
-        # Terrain variations should not be above 1
-        "noise": .9,
-        # Road trunks length
-        "section_len": 1,
-        # Ground friction coefficient root
-        "friction": .5 ** .5
-    },
-    # Studied system parameters
-    "linkage": {
-        # Maximal torque (N.m)
-        "torque": 1e3,
-        # Crank length (m) (unused for now)
-        "crank_len": .05,
-        # Linear mass of bars (kg/m)
-        "masses": 1,
-        # Load mass (kg)
-        "load": 10,
-    },
-    # Physics engine parameters
-    "physics": {
-        "gravity": (0, -9.80665),
-        # Maximal value of forces (N)
-        "max_force": 1e10,
-    },
-    # Study hypothesis
-    "simul": {
-        # Multiply time by this coefficient
-        "time_coef": 1,
-        # Number of calculations for each frame
-        "calc_rate": 300,
-        # Maximal number of subcalculations
-        "max_sub": 50,
-    },
-    # Display parameters
-    "camera": {
-        # Do you want to follow a system of view whole scene?
-        "dynamic_camera": True,
-        # Required frames per second
-        "fps": 20,
-    },
-}
+import matplotlib.animation as animation
+from pymunk import Space
 
+from . import physicsengine as pe
+from . import dynamiclinkage
 
-def set_space_constraints(space):
-    """Set the solver if they are many constraints."""
-    constraints = space.constraints
-    len_c = len(space.constraints)
-    # Number of iteration can be adapted
-    space.iterations = int(10 * np.exp(len_c / 60))
-    for constraint in constraints:
-        if not isinstance(constraint, pm.SimpleMotor) and False:
-            constraint.max_force = params["physics"]["max_force"] * (np.exp(
-                - len_c / 25) / 2 + .5)
-        constraint.error_bias = (1 - .1 * np.exp(-len_c / 60)) ** 60
+# Display settings
+CAMERA = {
+    # Do you want to follow a system of view whole scene?
+    "dynamic_camera": False,
+    # Required frames per second
+    "fps": 20,
+}
 
 
-class World:
+def smooth_transition(target, prev_view, dampers=((-10, -5), (10, 5))):
     """
-    A world contains a space of simulation, at least one linkage, and a road.
+    Create a smooth transition between a camera view (prev_view) and a target view.
 
-    It is not intended to be rendered visually per se, see VisualWorld for
-    this purpose.
+    Parameters
+    ----------
+    target : tuple of tuple of float
+        Target camera bounds.
+    prev_view : tuple of tuple of float
+        Current camera bounds
+    dampers : tuple of tuple of float
+        Absolute values to stay in
+
+    Returns
+    -------
+        New bounds : tuple of tuple of float
     """
-
-    def __init__(self, space=None, road_y=-5):
-        """
-        Initiate rigidbodies and simulation.
-
-        Add rigidbodies in linkage.
-
-        Parameters
-        ----------
-        space : pymunk.space.Space, optional
-            Space of simulation. The default is None.
-        road_y : float, optional
-            The ordinate of the ground. Useful when linkages have long legs.
-            The default is -5.
-        """
-        if isinstance(space, pm.Space):
-            self.space = space
-        else:
-            self.space = pm.Space()
-            self.space.gravity = params["physics"]["gravity"]
-
-        set_space_constraints(self.space)
-
-        # The road which will be built
-        self.road = [(-15, road_y), (15, road_y)]
-        # First road parts
-        seg = pm.Segment(self.space.static_body, self.road[0], self.road[-1],
-                         .1)
-        seg.friction = params["ground"]["friction"]
-        self.space.add(seg)
-        self.linkages = []
-
-    def add_linkage(self, linkage):
-        """Add a DynamicLinkage to the simulation."""
-        if isinstance(linkage, dlink.DynamicLinkage):
-            dynamiclinkage = linkage
-        else:
-            dynamiclinkage = dlink.convert_to_dynamic_linkage(
-                linkage, self.space)
-        for crank in dynamiclinkage._cranks:
-            crank.actuator.max_force = 0
-        self.linkages.append(dynamiclinkage)
-        for s in self.space.shapes:
-            s.friction = params["ground"]["friction"]
-        set_space_constraints(self.space)
-
-    def __update_linkage__(self, linkage, power):
-        """Update a specific linkage."""
-        linkage_crank = next(j for j in linkage.joints if isinstance(j, Crank))
-        if (
-                linkage_crank.actuator.max_force == 0
-                and norm(linkage.body.velocity) < .1):
-            linkage_crank.actuator.max_force = params["linkage"]["torque"]
-            linkage.height = linkage.body.position.y
-            linkage.mechanical_energy = (.5 * linkage.mass
-                                         * norm(linkage.body.velocity) ** 2)
-
-        # Energy from the motor in this step
-        energy = power * params["simul"]["time_coef"] / params["camera"]["fps"]
-        if hasattr(linkage, 'height') and energy != 0.:
-            v = norm(linkage.body.velocity)
-            g = norm(params["physics"]["gravity"])
-            m = linkage.mass
-            new_mechanical_energy = (m
-                                     * (.5 * v ** 2
-                                        + g * (linkage.body.position.y
-                                               - linkage.height))
-                                     )
-            efficiency = (new_mechanical_energy
-                          - linkage.mechanical_energy) / energy
-            linkage.mechanical_energy = new_mechanical_energy
-            return energy, efficiency
-        return 0, 0
-
-    def update(self, t):
-        """Update simulation."""
-        # Simulation step
-        dt = (params["simul"]["time_coef"] / params["simul"]["calc_rate"]
-              / params["camera"]["fps"])
-        # Motor power in this simulation step
-        powers = [[0 for j in lin.joints
-                   if isinstance(j, Crank)] for lin in self.linkages]
-        for _ in range(params["simul"]["calc_rate"]):
-            self.space.step(dt)
-            for i, linkage in enumerate(self.linkages):
-                index = -1
-                for crank in linkage.joints:
-                    if not isinstance(crank, Crank):
-                        continue
-                    index += 1
-                    # Get offset for crank rotation speed
-                    w = crank._b.angular_velocity
-                    w -= linkage.body.angular_velocity
-                    powers[i][index] += abs(w) * crank.actuator.impulse / dt
-
-        bounds = (0, 0)
-        energies = [0] * len(self.linkages)
-        efficiencies = [0] * len(self.linkages)
-        for i, linkage, power in zip(
-                range(len(self.linkages)), self.linkages, powers):
-            recalc_linkage(linkage)
-            energies[i], efficiencies[i] = self.__update_linkage__(linkage,
-                                                                   power[0])
-            bounds = (min(bounds[0], *(i.x for i in linkage.joints)),
-                      max(bounds[1], *(i.x for i in linkage.joints)))
-        while self.road[-1][0] < bounds[1] + 10:
-            self.build_road(True)
-        while self.road[0][0] > bounds[0] - 10:
-            self.build_road(False)
-
-        # Without animation, we return 100 times motor yield
-        # with duration step
-        for linkage, energy, efficiency in zip(self.linkages, energies,
-                                               efficiencies):
-            return efficiency, energy * dt
-            #if hasattr(linkage, 'height') and energy != 0:
-            #    return (1e2 * efficiency,
-            #            params["simul"]["time_coef"] /params["camera"]["fps"])
-
-    def __build_road_step__(self, ground, index):
-        """Add a step (two points)."""
-        high = np.random.rand() * ground["max_step"]
-        a = self.road[index][0], self.road[index][1] + high
-        b = (self.road[index][0] + ground["section_len"] * (1 - index),
-             self.road[index][1] + high)
-
-        s = pm.Segment(self.space.static_body, a, b, .1)
-        s.friction = ground["friction"]
-        self.space.add(s)
-        s = pm.Segment(self.space.static_body, a, self.road[index], .1)
-        s.friction = ground["friction"]
-        self.space.add(s)
-        # Add the elements in the end or the beginning
-        self.road.insert(-index * len(self.road), a)
-        self.road.insert(-index * len(self.road), b)
-
-    def __build_road_segment__(self, ground, index):
-        """Add a segment (one point)."""
-        # Add noise for more chaotic terrain."""
-        angle = np.random.normal(ground["slope"] / 2,
-                                 ground["noise"] * ground["slope"] / 2)
-        # Adding a point to the left is increasing angle by pi/2
-        if not index:
-            angle = np.pi - angle
-        a = pm.Vec2d(*cyl_to_cart(ground["section_len"], angle,
-                                  self.road[index]))
-        s = pm.Segment(self.space.static_body, a, self.road[index], .1)
-        s.friction = ground["friction"]
-        self.space.add(s)
-        self.road.insert(-index * len(self.road), a)
-
-    def build_road(self, positive=False):
-        """
-        Build a road part.
-
-        Arguments
-        ---------
-        positive: if False (default), the road part will be added on the left.
-        """
-        # Ground parameters
-        ground = params["ground"]
-        if np.random.rand() < ground["step_freq"] and False:
-            self.__build_road_step__(ground, -positive)
-        else:
-            self.__build_road_segment__(ground, -positive)
+    new_bounds = [list(target[0]), list(target[1])]
+    # Below this reactivity, we won't resize the window. Does not seem to work.
+    reactivity_threshold = 0.5
+    reactivity = [[0, 0], [0, 0]]
+    for i in range(2):
+        for j in range(2):
+            operator = max if j else min
+            if operator(target[i][j], prev_view[i][j]) == prev_view[i][j]:
+                # We are in-bounds
+                # do not change anything
+                if operator(target[i][j] - dampers[i][j], prev_view[i][j]) == prev_view[i][j]:
+                    reactivity[i][j] = np.interp(
+                        target[i][j],
+                        (prev_view[i][j], prev_view[i][j] + dampers[i][j]),
+                        [0, 1]
+                    )
+                else:
+                    reactivity[i][j] = 0
+            elif operator(target[i][j] + dampers[i][j], prev_view[i][j]) == prev_view[i][j]:
+                # Damper zone, initiate a smooth transition
+                reactivity[i][j] = np.interp(
+                    target[i][j],
+                    (prev_view[i][j], prev_view[i][j] - dampers[i][j]),
+                    [0, 1]
+                )
+            else:
+                # Out-of-bounds, move a quick as possible
+                reactivity[i][j] = 1
+    if any(reac[0] > reactivity_threshold or reac[1] > reactivity_threshold for reac in reactivity):
+        for i in range(2):
+            for j in range(2):
+                new_bounds[i][j] = target[i][j] * reactivity[i][j] + prev_view[i][j] * (1 - reactivity[i][j])
+    return new_bounds
 
 
-class VisualWorld(World):
+class VisualWorld(pe.World):
     """Same as parent class World, but with matplotlib objects."""
 
     def __init__(self, space=None, road_y=-5):
         """
         Instantiate the world and objects to be displayed.
 
         Parameters
         ----------
         space : pymunk.space.Space, optional
             Space of simulation. The default is None.
         road_y : float, optional
-            The ordinate of the ground. Useful when likages have long legs.
+            The ordinate of the ground. Useful when linkages have long legs.
             The default is -5.
         """
         super().__init__(space=space, road_y=road_y)
         self.fig, self.ax = plt.subplots()
         self.ax.set_aspect('equal')
         self.linkage_im = []
-        # Same for road
+        # Same for the road
         self.road_im = self.ax.plot([], [], 'k-', animated=False)
 
-    def add_linkage(self, linkage):
+    def add_linkage(self, linkage, load=0):
         """
-        Add a linkage to the world, and create the appropriate Artist objects.
+        Add a linkage to the simulation, and create the appropriate Artist objects.
 
         Parameters
         ----------
-        linkage : pylinkage.linkage.Linkage
-            The linkage you want to add, can be a Walker.
-
+        linkage : pylinkage.Linkage or leggedsnake.DynamicLinkage
+            Linkage to add.
+            We use the linkage's space if it is a DynamicLinkage.
+        load : float, optional
+            Load to add the center of the linkage.
+            Has no effect when using a DynamicLinkage.
+            The default is 0.
         Returns
         -------
         None.
 
         """
-        super().add_linkage(linkage)
+        super().add_linkage(linkage, load)
         # Objects that will allow display
         linkage_im = []
-        ax = self.ax
         for j in self.linkages[-1].joints:
             if (
-                    isinstance(j, Static)
+                    isinstance(j, pe.Static)
                     and hasattr(j, 'joint0')
-                    and j.joint0 is not None):
-                linkage_im.append(ax.plot([], [], 'k-', animated=False)[0])
+                    and j.joint0 is not None
+            ):
+                linkage_im.append(self.ax.plot([], [], 'k-', animated=False)[0])
                 if hasattr(j, 'joint1') and j.joint1 is not None:
-                    linkage_im.append(ax.plot([], [], 'k-', animated=False)[0])
-            elif isinstance(j, Crank):
-                linkage_im.append(ax.plot([], [], 'g-', animated=False)[0])
-            elif isinstance(j, Fixed):
-                linkage_im.append(ax.plot([], [], 'r-', animated=False)[0])
-                linkage_im.append(ax.plot([], [], 'r-', animated=False)[0])
-            elif isinstance(j, Pivot):
-                linkage_im.append(ax.plot([], [], 'b-', animated=False)[0])
-                linkage_im.append(ax.plot([], [], 'b-', animated=False)[0])
-        self.linkage_im.extend(linkage_im)
+                    linkage_im.append(self.ax.plot([], [], 'k-', animated=False)[0])
+            elif isinstance(j, pe.Crank):
+                linkage_im.append(self.ax.plot([], [], 'g-', animated=False)[0])
+            elif isinstance(j, pe.Fixed):
+                linkage_im.append(self.ax.plot([], [], 'r-', animated=False)[0])
+                linkage_im.append(self.ax.plot([], [], 'r-', animated=False)[0])
+            elif isinstance(j, pe.Pivot):
+                linkage_im.append(self.ax.plot([], [], 'b-', animated=False)[0])
+                linkage_im.append(self.ax.plot([], [], 'b-', animated=False)[0])
+        self.linkage_im.append(linkage_im)
 
-    def draw_linkage(self, joints):
+    def draw_linkage(self, linkage_im, joints):
         """Draw the linkage at his current state."""
         a = 0
         for j in joints:
             if hasattr(j, 'joint0') and j.joint0 is not None:
-                self.linkage_im[a].set_data([j.x, j.joint0.x],
-                                            [j.y, j.joint0.y])
+                linkage_im[a].set_data(
+                    [j.x, j.joint0.x], [j.y, j.joint0.y]
+                )
                 a += 1
             if hasattr(j, 'joint1') and j.joint1 is not None:
-                self.linkage_im[a].set_data([j.x, j.joint1.x],
-                                            [j.y, j.joint1.y])
+                linkage_im[a].set_data(
+                    [j.x, j.joint1.x], [j.y, j.joint1.y]
+                )
                 a += 1
-        return self.linkage_im
-
-    def update(self, t):
-        """Update simulation and draw it."""
-        super().update(t)
-        center = self.linkages[0].joints[0].coord()
-        self.fig.suptitle("Position: {}".format(tuple(map(int, center))))
-
-        self.road_im[0].set_data([i[0] for i in self.road],
-                                 [i[1] for i in self.road])
-        ax = self.ax
-        for linkage in self.linkages:
-            if params["camera"]["dynamic_camera"]:
-                ax.set_xlim(center[0] - 10, center[0] + 10)
-                ax.set_ylim(center[1] - 10, center[1] + 10)
-            else:
-                ax.set_ylim(min([0] + [i.y for i in linkage.joints]) - 5,
-                            max([0] + [i.y for i in linkage.joints]) + 5)
-
-        # Return modified objects for animation optimisation
-        return (
-            [self.draw_linkage(linkage.joints) for linkage in self.linkages]
-            + self.road_im)
+        return linkage_im
 
+    def init_visuals(self, colors=None):
+        if colors is not None:
+            for im, color in zip(self.linkage_im, colors):
+                for line in im:
+                    if np.isscalar(color):
+                        line.set_alpha(color)
+                    else:
+                        line.set_color(color)
+
+        return self.road_im + [im for im in self.linkage_im]
+
+    def reload_visuals(self):
+        """Reload the visual components only."""
+        center = np.mean([linkage.joints[0].coord() for linkage in self.linkages], axis=0)
+        self.fig.suptitle(f"Position: {tuple(map(int, center))}")
+
+        self.road_im[0].set_data(
+            [i[0] for i in self.road],
+            [i[1] for i in self.road]
+        )
+        prev_view = self.ax.get_xlim(), self.ax.get_ylim()
+        if CAMERA["dynamic_camera"]:
+            target = (center[0] - 10, center[0] + 10), (center[1] - 10, center[1] + 10)
+        else:
+            target = (
+                min([0] + [min(i.x for i in linkage.joints) for linkage in self.linkages]) - 10,
+                max([0] + [max(i.x for i in linkage.joints) for linkage in self.linkages]) + 10
+            ), (
+                min([0] + [min(i.y for i in linkage.joints) for linkage in self.linkages]) - 5,
+                max([0] + [max(i.y for i in linkage.joints) for linkage in self.linkages]) + 5
+            )
+        target = smooth_transition(target, prev_view)
+        self.ax.set_xlim(*target[0])
+        self.ax.set_ylim(*target[1])
+        # Return modified objects for animation optimization
+        visual_objects = []
+        for linkage, im in zip(self.linkages, self.linkage_im):
+            visual_objects += self.draw_linkage(im, linkage.joints)
+        visual_objects += self.road_im
+        return visual_objects
 
-def recalc_linkage(linkage):
-    """Assign a good position to all joints."""
-    for j in linkage.joints:
-        j.reload()
-
-
-def linkage_bb(linkage):
-    """
-    Return the bounding box for this linkage.
-
-    The bounding box is in form (min_y, max_x, max_y, min_x).
+    def visual_update(self, time=None):
+        """
+        Update simulation and draw it.
 
-    Parameters
-    ----------
-    linkage : pylinkage.linkage.Linkage
-        The linkage from which to get the bounding box.
-    """
-    data = [i.coord() for i in linkage.joints]
-    if isinstance(linkage, dlink.DynamicLinkage):
-        data.extend(tuple(i.position) for i in linkage.rigidbodies)
-    return bounding_box(data)
+        Parameters
+        ----------
+        time : list | float | None
+            When a list, delta-time for physics and display (respectively)
+            Using a float, only delta-time for physics, fps is set with CAMERA_SETTINGS["fps"]
+            Setting to None set physics dt to pe.params["simul"]["physics_period"] and fps to CAMERA_SETTINGS["fps"]
+        """
+        if time is None:
+            dt = pe.params["simul"]["physics_period"]
+            fps = CAMERA["fps"]
+        elif isinstance(time, int) or isinstance(time, float):
+            dt = time
+            fps = CAMERA["fps"]
+        else:
+            dt, fps = time
+        div = 1 // (dt * fps)
+        if div >= 1:
+            update_ret = [0, 0]
+            for _ in range(int(div)):
+                for i, step_update in enumerate(self.update(dt)):
+                    update_ret[i] += step_update
+            for i, step_update in enumerate(self.update(1 / fps - dt * div)):
+                update_ret[i] += step_update
+        else:
+            update_ret = self.update(dt)
+        self.reload_visuals()
+        return update_ret
 
 
 def im_debug(world, linkage):
     """Use pymunk debugging for visual debugging."""
-    bbox = linkage_bb(linkage)
+    bbox = pe.linkage_bb(linkage)
     world.ax.clear()
     world.ax.set_xlim(int(bbox[3]) - 5, int(bbox[1]) + 5)
     world.ax.set_ylim(int(bbox[2]) - 5, int(bbox[0]) + 5)
-    world.ax.scatter([i.x for i in linkage.joints],
-                     [i.y for i in linkage.joints], c='r')
+    world.ax.scatter(
+        [i.x for i in linkage.joints],
+        [i.y for i in linkage.joints],
+        c='r'
+    )
     for j in linkage.joints:
         for shape in j._a.shapes:
             begin = j._a.local_to_world(shape.a)
             end = j._a.local_to_world(shape.b)
             world.ax.plot([begin[0], end[0]], [begin[1], end[1]])
     options = pymunk.matplotlib_util.DrawOptions(world.ax)
     options.constraint_color = (.1, .1, .1, .0)
     world.space.debug_draw(options)
 
 
 def video_debug(linkage):
     """Launch the simulation frame by frame, useful for debug."""
-    road_y = linkage_bb(linkage)[0] - 1
-    if isinstance(linkage, dlink.DynamicLinkage):
+    road_y = pe.linkage_bb(linkage)[0] - 1
+    if isinstance(linkage, dynamiclinkage.DynamicLinkage):
         world = VisualWorld(linkage.space, road_y=road_y)
     else:
         world = VisualWorld(road_y=road_y)
     world.add_linkage(linkage)
-    dynamiclinkage = world.linkages[-1]
+    dynamic_linkage = world.linkages[-1]
     for _ in range(1, int(1e3)):
-        dt = (params["simul"]["time_coef"] / params["simul"]["calc_rate"]
-              / params["camera"]["fps"])
-        for i in range(params["simul"]["calc_rate"]):
-            world.space.step(dt)
-        recalc_linkage(dynamiclinkage)
-        im_debug(world, dynamiclinkage)
+        dt = pe.params["simul"]["physics_period"]
+        world.space.step(dt)
+        pe.recalc_linkage(dynamic_linkage)
+        im_debug(world, dynamic_linkage)
         plt.pause(.2)
 
 
-def video(linkage, duration=30, save=False):
+def all_linkages_video(linkages, duration=30, save=False, colors=None, dynamic_camera=False):
     """
     Give the rigidbody a dynamic model and launch simulation with video.
 
     Parameters
     ----------
-    linkage : Union[pylinkage.linkage.Linkage,
-    leggedsnake.dynamiclinkage.DynamicLinkage]
+    linkages : Union[
+        list of pylinkage.linkage.Linkage,
+        list of leggedsnake.dynamiclinkage.DynamicLinkage
+    ]
         The Linkage you want to simulate.
     duration : float, optional
         Duration (in seconds) of the simulation. The default is 40.
     save : bool, optional
         If you want to save it as a .mp4 file.
+    colors : list of float or list of list of float
+        * If a list of float, it is the list of opacities
+        * If a list of list of float, it is the list of colors
+        * If None, opacities are set randomly
+    dynamic_camera : bool, optional
+        Type of visualization. True follows one strider, False gives a larger view.
+        The default is False.
     """
-    road_y = linkage_bb(linkage)[0] - 1
-    if isinstance(linkage, dlink.DynamicLinkage):
-        world = VisualWorld(linkage.space, road_y=road_y)
+    road_y = min(pe.linkage_bb(linkage)[0] for linkage in linkages) - 1
+    if isinstance(linkages[0], dynamiclinkage.DynamicLinkage):
+        world = VisualWorld(linkages[0].space, road_y=road_y)
     else:
         world = VisualWorld(road_y=road_y)
-    world.add_linkage(linkage)
+    for linkage in linkages:
+        world.add_linkage(linkage)
     # Number of frames for the selected duration
-    n = int(params["camera"]["fps"] * duration
-            / params["simul"]["time_coef"])
+    n_frames = int(CAMERA["fps"] * duration)
 
-    animation = anim.FuncAnimation(
-        world.fig, world.update, frames=range(1, n),
-        interval=int(1000 / params["camera"]["fps"]),
+    dt = pe.params["simul"]["physics_period"]
+    fps = CAMERA["fps"]
+    if dt * fps > 1:
+        print(
+            f"Warning: Physics is computed every {dt}s ({1 / dt} times/s)",
+            f"but display is {fps} times/s."
+        )
+
+    if colors is None:
+        colors = np.logspace(0, -1, num=len(linkages))
+    previous_camera = CAMERA["dynamic_camera"]
+    CAMERA["dynamic_camera"] = dynamic_camera
+    ani = animation.FuncAnimation(
+        world.fig, world.visual_update,
+        frames=[None] * (n_frames - 1),
+        init_func=partial(world.init_visuals, colors),
+        interval=int(1000 / CAMERA["fps"]),
         repeat=False, blit=False
     )
     if save:
-        writer = anim.FFMpegWriter(fps=params["camera"]["fps"], bitrate=2500)
-        animation.save(f"Dynamic {linkage.name}.mp4", writer=writer)
+        writer = animation.FFMpegWriter(fps=CAMERA["fps"], bitrate=2500)
+        ani.save(f"Dynamic {linkages[0].name}.mp4", writer=writer)
     else:
         plt.show()
-        if animation:
+        if ani:
             pass
+    CAMERA["dynamic_camera"] = previous_camera
+
+
+def video(linkage, duration=30, save=False, dynamic_camera=True):
+    """
+    Give the rigidbody a dynamic model and launch simulation with video.
+
+    Parameters
+    ----------
+    linkage : Union[pylinkage.linkage.Linkage,
+    leggedsnake.dynamiclinkage.DynamicLinkage]
+        The Linkage you want to simulate.
+    duration : float, optional
+        Duration (in seconds) of the simulation. The default is 40.
+    save : bool, optional
+        If you want to save it as a .mp4 file.
+    dynamic_camera : bool, optional
+        Type of visualization. True follows one strider, False gives a larger view.
+        The default is True.
+    """
+    all_linkages_video([linkage], duration, save, dynamic_camera=dynamic_camera)
 
 
 if __name__ == "__main__":
-    base = Static(0, 0, name="Main trick")
-    crank = Crank(1, 0, name="The crank", angle=1, joint0=base)
-    follower = Pivot(0, 2, joint0=base, joint1=crank, distance0=2,
-                     distance1=1)
-    frame = Fixed(joint0=crank, joint1=follower, distance=1, angle=-np.pi/2)
-    demo_linkage = dlink.DynamicLinkage(
+    base = pe.Static(0, 0, name="Main trick")
+    crank = pe.Crank(1, 0, name="The crank", angle=1, joint0=base)
+    follower = pe.Pivot(
+        0, 2, joint0=base, joint1=crank, distance0=2, distance1=1
+    )
+    frame = pe.Fixed(joint0=crank, joint1=follower, distance=1, angle=-np.pi/2)
+    demo_linkage = pe.dynamiclinkage.DynamicLinkage(
         name='Some tricky linkage',
         joints=(base, crank, follower, frame),
-        space=pm.Space()
+        space=Space()
     )
-    demo_linkage.space.gravity = params["physics"]["gravity"]
+    demo_linkage.space.gravity = pe.params["physics"]["gravity"]
     video_debug(demo_linkage)
```

### Comparing `leggedsnake-0.3.1/leggedsnake/show_evolution.py` & `leggedsnake-0.4.0/leggedsnake/show_evolution.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,27 +19,27 @@
     vector = tuple(map(func, scores))
     axis.plot(vector)
 
 
 def draw_median_score(axis, scores):
     """Compute a median vector from a score matrix and draw it."""
     median = tuple(map(np.nanmedian, scores))
-    axis.plot(median, c='g', label="Median score")
+    axis.plot(median, label="Median score")
 
 
 def draw_best_score(axis, scores):
     """Compute the best score vector form a score matrix and draw it."""
     best = tuple(map(np.nanmax, scores))
-    axis.plot(best, c='r', label="Best score")
+    axis.plot(best, label="Best score")
 
 
 def draw_standard_deviation(axis, scores):
     """Draw the standard deviation of scores from a score matrix."""
     std = tuple(map(np.nanstd, scores))
-    axis.plot(std, c='b', label="Standard deviation")
+    axis.plot(std, label="Standard deviation")
 
 
 def draw_population(axis, populations):
     """Just draw the number of individuals in the population."""
     pop_vector = tuple(map(len, populations))
     axis.plot(pop_vector, label="Population")
     axis.set_ylabel("Total population")
@@ -48,14 +48,21 @@
 
 def draw_diversity(axis, dimensions):
     """Draw the standard deviation in the dimensions."""
     diversity_vector = tuple(map(np.nanstd, dimensions))
     axis.plot(diversity_vector, label="Genetic diversity")
 
 
+def load_data(json_file):
+    """Load the population from a JSON file, and return it."""
+    with open(json_file) as file:
+        data = json.load(file)
+        return data
+
+
 def show_genetic_optimization(data=DATA):
     """
     Show a graph representing an optimization with a genetic algorithm.
 
     Parameters
     ----------
     data : Any, default=None
@@ -90,11 +97,9 @@
     draw_population(pop_axis, scores)
     fig.suptitle("Evolution of linkages using a genetic algorithm")
     fig.legend()
     plt.show()
 
 
 if __name__ == "__main__":
-    with open("Population evolution.json") as file:
-        DATA.extend(json.load(file))
-
-    show_genetic_optimization()
+    data = load_data("Population evolution.json")
+    show_genetic_optimization(data)
```

### Comparing `leggedsnake-0.3.1/leggedsnake/utility.py` & `leggedsnake-0.4.0/leggedsnake/utility.py`

 * *Files identical despite different names*

### Comparing `leggedsnake-0.3.1/leggedsnake/walker.py` & `leggedsnake-0.4.0/leggedsnake/walker.py`

 * *Files identical despite different names*

### Comparing `leggedsnake-0.3.1/leggedsnake.egg-info/SOURCES.txt` & `leggedsnake-0.4.0/leggedsnake.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -19,13 +19,15 @@
 leggedsnake/__init__.py
 leggedsnake/dynamiclinkage.py
 leggedsnake/geneticoptimizer.py
 leggedsnake/physicsengine.py
 leggedsnake/show_evolution.py
 leggedsnake/utility.py
 leggedsnake/walker.py
+leggedsnake/worldvisualizer.py
 leggedsnake.egg-info/PKG-INFO
 leggedsnake.egg-info/SOURCES.txt
 leggedsnake.egg-info/dependency_links.txt
 leggedsnake.egg-info/requires.txt
 leggedsnake.egg-info/top_level.txt
+leggedsnake.egg-info/zip-safe
 tests/test_utility.py
```

### Comparing `leggedsnake-0.3.1/setup.cfg` & `leggedsnake-0.4.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 [bumpversion]
-current_version = 0.3.1
+current_version = 0.4.0
 commit = False
 tag = False
 
 [metadata]
 name = leggedsnake
 version = attr: leggedsnake.__version__
 author = Hugo Farajallah
+author_email = leggedsnake@hugofara.net
 description = Simulate and optimize planar leg mechanisms using PSO and GA
+long_description = file: README.md, CHANGELOG.md
+long_description_content_type = text/markdown
+keywords = linkage, leg mechanism, optimization, leggedsnake, walking linkage
 license = MIT License
 url = https://hugofara.github.io/leggedsnake/
 project_urls = 
 	Changelog=https://hugofara.github.io/leggedsnake/changeloglink.html
 	Source=https://github.com/HugoFara/leggedsnake
-long_description = file: README.md, CHANGELOG.md
-long_description_content_type = text/markdown
-license_file = LICENSE.rst
+license_files = LICENSE.rst
 classifiers = 
-	Development Status :: 3 - Alpha
+	Development Status :: 4 - Beta
 	Topic :: Scientific/Engineering
 	Topic :: Scientific/Engineering :: Artificial Life
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Environment :: Console
 	Intended Audience :: Science/Research
 	Intended Audience :: Legal Industry
 	Intended Audience :: End Users/Desktop
 	Operating System :: OS Independent
-keywords = linkage, leg mechanism, optimization, leggedsnake, walking linkage
-zip_safe = true
 
 [options]
+zip_safe = True
 packages = leggedsnake
 install_requires = 
 	numpy
 	tqdm
 	matplotlib
 	pylinkage
 test_suite = tests
+python_requires = >=3.7
 
 [bumpversion:file:leggedsnake/__init__.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
 
 [bumpversion:file:source/conf.py]
 search = release = '{current_version}'
```

### Comparing `leggedsnake-0.3.1/tests/test_utility.py` & `leggedsnake-0.4.0/tests/test_utility.py`

 * *Files identical despite different names*

