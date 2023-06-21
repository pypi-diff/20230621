# Comparing `tmp/CUQIpy-0.4.0.post0.dev19.tar.gz` & `tmp/CUQIpy-0.4.0.post0.dev21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CUQIpy-0.4.0.post0.dev19.tar", last modified: Fri Jun  9 08:18:05 2023, max compression
+gzip compressed data, was "CUQIpy-0.4.0.post0.dev21.tar", last modified: Wed Jun 21 19:37:10 2023, max compression
```

## Comparing `CUQIpy-0.4.0.post0.dev19.tar` & `CUQIpy-0.4.0.post0.dev21.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.956735 CUQIpy-0.4.0.post0.dev19/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.920735 CUQIpy-0.4.0.post0.dev19/CUQIpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16388 2023-06-09 08:18:05.000000 CUQIpy-0.4.0.post0.dev19/CUQIpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-09 08:18:05.000000 CUQIpy-0.4.0.post0.dev19/CUQIpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 08:18:05.000000 CUQIpy-0.4.0.post0.dev19/CUQIpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-09 08:18:05.000000 CUQIpy-0.4.0.post0.dev19/CUQIpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-09 08:18:05.000000 CUQIpy-0.4.0.post0.dev19/CUQIpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16388 2023-06-09 08:18:05.952736 CUQIpy-0.4.0.post0.dev19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.956735 CUQIpy-0.4.0.post0.dev19/cuqi/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-09 08:18:05.956735 CUQIpy-0.4.0.post0.dev19/cuqi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.924735 CUQIpy-0.4.0.post0.dev19/cuqi/array/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/array/_array.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.928735 CUQIpy-0.4.0.post0.dev19/cuqi/data/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/data/_data.py
--rw-r--r--   0 runner    (1001) docker     (123)   786696 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/data/astronaut.npz
--rw-r--r--   0 runner    (1001) docker     (123)   262408 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/data/camera.npz
--rw-r--r--   0 runner    (1001) docker     (123)   406164 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/data/cat.npz
--rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/data/satellite.mat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.928735 CUQIpy-0.4.0.post0.dev19/cuqi/density/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/density/_density.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/diagnostics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.932735 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_beta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_cauchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_cmrf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    15873 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)    32903 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_gmrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_inverse_gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)    15039 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_joint_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_laplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_lmrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_lognormal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_normal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_posterior.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_uniform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.932735 CUQIpy-0.4.0.post0.dev19/cuqi/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39613 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/geometry/_geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.932735 CUQIpy-0.4.0.post0.dev19/cuqi/likelihood/
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/likelihood/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/likelihood/_likelihood.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.932735 CUQIpy-0.4.0.post0.dev19/cuqi/model/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24201 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/model/_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.932735 CUQIpy-0.4.0.post0.dev19/cuqi/operator/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/operator/_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.936735 CUQIpy-0.4.0.post0.dev19/cuqi/pde/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/pde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12572 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/pde/_pde.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.936735 CUQIpy-0.4.0.post0.dev19/cuqi/problem/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/problem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28944 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/problem/_problem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.940735 CUQIpy-0.4.0.post0.dev19/cuqi/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_conjugate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_conjugate_approx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_cwmh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_gibbs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_hmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_langevin_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_laplace_approximation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_mh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_pcn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_rto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.940735 CUQIpy-0.4.0.post0.dev19/cuqi/samples/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27128 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/samples/_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.940735 CUQIpy-0.4.0.post0.dev19/cuqi/solver/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19377 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/solver/_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.940735 CUQIpy-0.4.0.post0.dev19/cuqi/testproblem/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/testproblem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52242 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/testproblem/_testproblem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.944735 CUQIpy-0.4.0.post0.dev19/cuqi/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/utilities/_get_python_variable_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/utilities/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 08:18:05.956735 CUQIpy-0.4.0.post0.dev19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.952736 CUQIpy-0.4.0.post0.dev19/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/tests/test_abstract_distribution_density.py
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/tests/test_bayesian_inversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/tests/test_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    29794 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/tests/test_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    14728 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/tests/test_joint_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/tests/test_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)    21330 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/tests/test_pde.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/tests/test_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    16757 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/tests/test_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/tests/test_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/tests/test_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/tests/test_testproblem.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:37:10.482885 CUQIpy-0.4.0.post0.dev21/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:37:10.474886 CUQIpy-0.4.0.post0.dev21/CUQIpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16388 2023-06-21 19:37:10.000000 CUQIpy-0.4.0.post0.dev21/CUQIpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-21 19:37:10.000000 CUQIpy-0.4.0.post0.dev21/CUQIpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:37:10.000000 CUQIpy-0.4.0.post0.dev21/CUQIpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-21 19:37:10.000000 CUQIpy-0.4.0.post0.dev21/CUQIpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 19:37:10.000000 CUQIpy-0.4.0.post0.dev21/CUQIpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16388 2023-06-21 19:37:10.482885 CUQIpy-0.4.0.post0.dev21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:37:10.482885 CUQIpy-0.4.0.post0.dev21/cuqi/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-21 19:37:10.482885 CUQIpy-0.4.0.post0.dev21/cuqi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:37:10.474886 CUQIpy-0.4.0.post0.dev21/cuqi/array/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/array/_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:37:10.474886 CUQIpy-0.4.0.post0.dev21/cuqi/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/data/_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)   786696 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/data/astronaut.npz
+-rw-r--r--   0 runner    (1001) docker     (123)   262408 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/data/camera.npz
+-rw-r--r--   0 runner    (1001) docker     (123)   406164 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/data/cat.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/data/satellite.mat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:37:10.474886 CUQIpy-0.4.0.post0.dev21/cuqi/density/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/density/_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/diagnostics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:37:10.478886 CUQIpy-0.4.0.post0.dev21/cuqi/distribution/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/distribution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/distribution/_beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/distribution/_cauchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/distribution/_cmrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/distribution/_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15873 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/distribution/_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/distribution/_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32903 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/distribution/_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/distribution/_gmrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/distribution/_inverse_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15039 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/distribution/_joint_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/distribution/_laplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/distribution/_lmrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/distribution/_lognormal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/distribution/_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/distribution/_posterior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/distribution/_uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:37:10.478886 CUQIpy-0.4.0.post0.dev21/cuqi/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39613 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/geometry/_geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:37:10.478886 CUQIpy-0.4.0.post0.dev21/cuqi/likelihood/
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/likelihood/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/likelihood/_likelihood.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:37:10.478886 CUQIpy-0.4.0.post0.dev21/cuqi/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24201 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/model/_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:37:10.478886 CUQIpy-0.4.0.post0.dev21/cuqi/operator/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/operator/_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:37:10.478886 CUQIpy-0.4.0.post0.dev21/cuqi/pde/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/pde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12572 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/pde/_pde.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:37:10.478886 CUQIpy-0.4.0.post0.dev21/cuqi/problem/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/problem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28944 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/problem/_problem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:37:10.482885 CUQIpy-0.4.0.post0.dev21/cuqi/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/sampler/_conjugate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/sampler/_conjugate_approx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/sampler/_cwmh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/sampler/_gibbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/sampler/_hmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/sampler/_langevin_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/sampler/_laplace_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/sampler/_mh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/sampler/_pcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/sampler/_rto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/sampler/_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:37:10.482885 CUQIpy-0.4.0.post0.dev21/cuqi/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27128 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/samples/_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:37:10.482885 CUQIpy-0.4.0.post0.dev21/cuqi/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19377 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/solver/_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:37:10.482885 CUQIpy-0.4.0.post0.dev21/cuqi/testproblem/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/testproblem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52242 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/testproblem/_testproblem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:37:10.482885 CUQIpy-0.4.0.post0.dev21/cuqi/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/utilities/_get_python_variable_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/cuqi/utilities/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 19:37:10.482885 CUQIpy-0.4.0.post0.dev21/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:37:10.482885 CUQIpy-0.4.0.post0.dev21/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/tests/test_abstract_distribution_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/tests/test_bayesian_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/tests/test_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29794 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/tests/test_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14728 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/tests/test_joint_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/tests/test_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21330 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15166 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/tests/test_pde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/tests/test_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16757 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/tests/test_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/tests/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/tests/test_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/tests/test_testproblem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-21 19:37:00.000000 CUQIpy-0.4.0.post0.dev21/tests/test_utilities.py
```

### Comparing `CUQIpy-0.4.0.post0.dev19/CUQIpy.egg-info/PKG-INFO` & `CUQIpy-0.4.0.post0.dev21/CUQIpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CUQIpy
-Version: 0.4.0.post0.dev19
+Version: 0.4.0.post0.dev21
 Summary: Computational Uncertainty Quantification for Inverse problems in Python
 Maintainer-email: "Nicolai A. B. Riis" <nabr@dtu.dk>, "Jakob S. Jørgensen" <jakj@dtu.dk>, "Amal M. Alghamdi" <amaal@dtu.dk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `CUQIpy-0.4.0.post0.dev19/CUQIpy.egg-info/SOURCES.txt` & `CUQIpy-0.4.0.post0.dev21/CUQIpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/LICENSE` & `CUQIpy-0.4.0.post0.dev21/LICENSE`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/PKG-INFO` & `CUQIpy-0.4.0.post0.dev21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CUQIpy
-Version: 0.4.0.post0.dev19
+Version: 0.4.0.post0.dev21
 Summary: Computational Uncertainty Quantification for Inverse problems in Python
 Maintainer-email: "Nicolai A. B. Riis" <nabr@dtu.dk>, "Jakob S. Jørgensen" <jakj@dtu.dk>, "Amal M. Alghamdi" <amaal@dtu.dk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `CUQIpy-0.4.0.post0.dev19/README.md` & `CUQIpy-0.4.0.post0.dev21/README.md`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/array/_array.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/array/_array.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/config.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/config.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/data/_data.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/data/_data.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/data/astronaut.npz` & `CUQIpy-0.4.0.post0.dev21/cuqi/data/astronaut.npz`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/data/camera.npz` & `CUQIpy-0.4.0.post0.dev21/cuqi/data/camera.npz`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/data/cat.npz` & `CUQIpy-0.4.0.post0.dev21/cuqi/data/cat.npz`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/data/satellite.mat` & `CUQIpy-0.4.0.post0.dev21/cuqi/data/satellite.mat`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/density/_density.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/density/_density.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/diagnostics.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/diagnostics.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/__init__.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_beta.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/distribution/_beta.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_cauchy.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/distribution/_cauchy.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_cmrf.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/distribution/_cmrf.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_custom.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/distribution/_custom.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_distribution.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/distribution/_distribution.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_gamma.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/distribution/_gamma.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_gaussian.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/distribution/_gaussian.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_gmrf.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/distribution/_gmrf.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_inverse_gamma.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/distribution/_inverse_gamma.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_joint_distribution.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/distribution/_joint_distribution.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_laplace.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/distribution/_laplace.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_lmrf.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/distribution/_lmrf.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_lognormal.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/distribution/_lognormal.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_normal.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/distribution/_normal.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_posterior.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/distribution/_posterior.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_uniform.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/distribution/_uniform.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/geometry/__init__.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/geometry/_geometry.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/geometry/_geometry.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/likelihood/__init__.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/likelihood/__init__.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/likelihood/_likelihood.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/likelihood/_likelihood.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/model/_model.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/model/_model.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/operator/_operator.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/operator/_operator.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/pde/_pde.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/pde/_pde.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/problem/_problem.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/problem/_problem.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_conjugate.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/sampler/_conjugate.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_conjugate_approx.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/sampler/_conjugate_approx.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_cwmh.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/sampler/_cwmh.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_gibbs.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/sampler/_gibbs.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_hmc.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/sampler/_hmc.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_langevin_algorithm.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/sampler/_langevin_algorithm.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_laplace_approximation.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/sampler/_laplace_approximation.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_mh.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/sampler/_mh.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_pcn.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/sampler/_pcn.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_rto.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/sampler/_rto.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_sampler.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/sampler/_sampler.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/samples/_samples.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/samples/_samples.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/solver/_solver.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/solver/_solver.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/testproblem/_testproblem.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/testproblem/_testproblem.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/utilities/_get_python_variable_name.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/utilities/_get_python_variable_name.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/cuqi/utilities/_utilities.py` & `CUQIpy-0.4.0.post0.dev21/cuqi/utilities/_utilities.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/pyproject.toml` & `CUQIpy-0.4.0.post0.dev21/pyproject.toml`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/tests/test_abstract_distribution_density.py` & `CUQIpy-0.4.0.post0.dev21/tests/test_abstract_distribution_density.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/tests/test_bayesian_inversion.py` & `CUQIpy-0.4.0.post0.dev21/tests/test_bayesian_inversion.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/tests/test_density.py` & `CUQIpy-0.4.0.post0.dev21/tests/test_density.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/tests/test_distribution.py` & `CUQIpy-0.4.0.post0.dev21/tests/test_distribution.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/tests/test_geometry.py` & `CUQIpy-0.4.0.post0.dev21/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/tests/test_joint_distribution.py` & `CUQIpy-0.4.0.post0.dev21/tests/test_joint_distribution.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/tests/test_likelihood.py` & `CUQIpy-0.4.0.post0.dev21/tests/test_likelihood.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/tests/test_model.py` & `CUQIpy-0.4.0.post0.dev21/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/tests/test_pde.py` & `CUQIpy-0.4.0.post0.dev21/tests/test_pde.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,18 +244,18 @@
             Dxx, source_term, np.ones(dim))
         if parametrization == 'source_term1':
             parameters = np.zeros(dim)
         elif parametrization == 'source_term2':
             parameters = np.ones(dim)
 
     # 4. Set up the observation parameters
-    if grid_obs == 'half_grid':
+    if isinstance(grid_obs, str) and grid_obs == 'half_grid':
         grid_obs = grid_sol[int(dim/2):]
 
-    if time_obs == 'every_5':
+    if isinstance(time_obs, str) and time_obs == 'every_5':
         time_obs = time_steps[::5]
 
     # 5. Create a PDE object
     PDE = cuqi.pde.TimeDependentLinearPDE(
         PDE_form, time_steps, method=method,
         grid_sol=grid_sol,
         grid_obs=grid_obs, time_obs=time_obs,
```

### Comparing `CUQIpy-0.4.0.post0.dev19/tests/test_problem.py` & `CUQIpy-0.4.0.post0.dev21/tests/test_problem.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/tests/test_sampler.py` & `CUQIpy-0.4.0.post0.dev21/tests/test_sampler.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/tests/test_samples.py` & `CUQIpy-0.4.0.post0.dev21/tests/test_samples.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/tests/test_solver.py` & `CUQIpy-0.4.0.post0.dev21/tests/test_solver.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/tests/test_testproblem.py` & `CUQIpy-0.4.0.post0.dev21/tests/test_testproblem.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0.post0.dev19/tests/test_utilities.py` & `CUQIpy-0.4.0.post0.dev21/tests/test_utilities.py`

 * *Files identical despite different names*

