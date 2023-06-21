# Comparing `tmp/blond-2.1.8.tar.gz` & `tmp/blond-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blond-2.1.8.tar", last modified: Thu Jun 15 14:48:02 2023, max compression
+gzip compressed data, was "blond-2.1.9.tar", last modified: Mon Jun 19 10:46:20 2023, max compression
```

## Comparing `blond-2.1.8.tar` & `blond-2.1.9.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:48:02.348000 blond-2.1.8/
--rw-r--r--   0 root         (0) root         (0)      399 2023-06-15 14:47:35.000000 blond-2.1.8/.coveragerc
--rw-r--r--   0 root         (0) root         (0)     6235 2023-06-15 14:47:35.000000 blond-2.1.8/.gitignore
--rw-r--r--   0 root         (0) root         (0)     3411 2023-06-15 14:47:35.000000 blond-2.1.8/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)     1887 2023-06-15 14:47:35.000000 blond-2.1.8/CHANGELOG
--rw-r--r--   0 root         (0) root         (0)    35797 2023-06-15 14:47:35.000000 blond-2.1.8/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      208 2023-06-15 14:47:35.000000 blond-2.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    14287 2023-06-15 14:48:02.348000 blond-2.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13525 2023-06-15 14:47:35.000000 blond-2.1.8/README.md
--rw-r--r--   0 root         (0) root         (0)      794 2023-06-15 14:47:35.000000 blond-2.1.8/WARNINGS.txt
--rw-r--r--   0 root         (0) root         (0)     1380 2023-06-15 14:47:35.000000 blond-2.1.8/appveyor.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:48:02.328000 blond-2.1.8/blond/
--rw-r--r--   0 root         (0) root         (0)     2407 2023-06-15 14:47:35.000000 blond-2.1.8/blond/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-06-15 14:48:02.000000 blond-2.1.8/blond/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:48:02.332000 blond-2.1.8/blond/beam/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 14:47:35.000000 blond-2.1.8/blond/beam/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20226 2023-06-15 14:47:35.000000 blond-2.1.8/blond/beam/beam.py
--rw-r--r--   0 root         (0) root         (0)     4424 2023-06-15 14:47:35.000000 blond-2.1.8/blond/beam/coasting_beam.py
--rw-r--r--   0 root         (0) root         (0)    44819 2023-06-15 14:47:35.000000 blond-2.1.8/blond/beam/distributions.py
--rw-r--r--   0 root         (0) root         (0)    40049 2023-06-15 14:47:35.000000 blond-2.1.8/blond/beam/distributions_multibunch.py
--rw-r--r--   0 root         (0) root         (0)    23708 2023-06-15 14:47:35.000000 blond-2.1.8/blond/beam/profile.py
--rw-r--r--   0 root         (0) root         (0)     5740 2023-06-15 14:47:35.000000 blond-2.1.8/blond/beam/sparse_histogram.cpp
--rw-r--r--   0 root         (0) root         (0)     4796 2023-06-15 14:47:35.000000 blond-2.1.8/blond/beam/sparse_slices.py
--rw-r--r--   0 root         (0) root         (0)    12857 2023-06-15 14:47:35.000000 blond-2.1.8/blond/compile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:48:02.336000 blond-2.1.8/blond/cpp_routines/
--rw-r--r--   0 root         (0) root         (0)     3088 2023-06-15 14:47:35.000000 blond-2.1.8/blond/cpp_routines/beam_phase.cpp
--rw-r--r--   0 root         (0) root         (0)    29022 2023-06-15 14:47:35.000000 blond-2.1.8/blond/cpp_routines/blondmath.cpp
--rw-r--r--   0 root         (0) root         (0)    13334 2023-06-15 14:47:35.000000 blond-2.1.8/blond/cpp_routines/blondmath.h
--rw-r--r--   0 root         (0) root         (0)     1316 2023-06-15 14:47:35.000000 blond-2.1.8/blond/cpp_routines/cos.h
--rw-r--r--   0 root         (0) root         (0)     5747 2023-06-15 14:47:35.000000 blond-2.1.8/blond/cpp_routines/drift.cpp
--rw-r--r--   0 root         (0) root         (0)     4376 2023-06-15 14:47:35.000000 blond-2.1.8/blond/cpp_routines/exp.h
--rw-r--r--   0 root         (0) root         (0)     4661 2023-06-15 14:47:35.000000 blond-2.1.8/blond/cpp_routines/fast_resonator.cpp
--rw-r--r--   0 root         (0) root         (0)    29481 2023-06-15 14:47:35.000000 blond-2.1.8/blond/cpp_routines/fft.cpp
--rw-r--r--   0 root         (0) root         (0)     4419 2023-06-15 14:47:35.000000 blond-2.1.8/blond/cpp_routines/fft.h
--rw-r--r--   0 root         (0) root         (0)    10031 2023-06-15 14:47:35.000000 blond-2.1.8/blond/cpp_routines/histogram.cpp
--rw-r--r--   0 root         (0) root         (0)     3493 2023-06-15 14:47:35.000000 blond-2.1.8/blond/cpp_routines/kick.cpp
--rw-r--r--   0 root         (0) root         (0)     6406 2023-06-15 14:47:35.000000 blond-2.1.8/blond/cpp_routines/linear_interp_kick.cpp
--rw-r--r--   0 root         (0) root         (0)    15181 2023-06-15 14:47:35.000000 blond-2.1.8/blond/cpp_routines/music_track.cpp
--rw-r--r--   0 root         (0) root         (0)      169 2023-06-15 14:47:35.000000 blond-2.1.8/blond/cpp_routines/openmp.cpp
--rw-r--r--   0 root         (0) root         (0)      245 2023-06-15 14:47:35.000000 blond-2.1.8/blond/cpp_routines/openmp.h
--rw-r--r--   0 root         (0) root         (0)     1960 2023-06-15 14:47:35.000000 blond-2.1.8/blond/cpp_routines/sin.h
--rw-r--r--   0 root         (0) root         (0)     5871 2023-06-15 14:47:35.000000 blond-2.1.8/blond/cpp_routines/sincos.h
--rw-r--r--   0 root         (0) root         (0)     7480 2023-06-15 14:47:35.000000 blond-2.1.8/blond/cpp_routines/vdtcore_common.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:48:02.336000 blond-2.1.8/blond/gpu/
--rw-r--r--   0 root         (0) root         (0)     2561 2023-06-15 14:47:35.000000 blond-2.1.8/blond/gpu/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11763 2023-06-15 14:47:35.000000 blond-2.1.8/blond/gpu/butils_wrap_cupy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:48:02.336000 blond-2.1.8/blond/gpu/cuda_kernels/
--rw-r--r--   0 root         (0) root         (0)    14390 2023-06-15 14:47:35.000000 blond-2.1.8/blond/gpu/cuda_kernels/kernels_double.cu
--rw-r--r--   0 root         (0) root         (0)    14135 2023-06-15 14:47:35.000000 blond-2.1.8/blond/gpu/cuda_kernels/kernels_single.cu
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:48:02.336000 blond-2.1.8/blond/impedances/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 14:47:35.000000 blond-2.1.8/blond/impedances/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39010 2023-06-15 14:47:35.000000 blond-2.1.8/blond/impedances/impedance.py
--rw-r--r--   0 root         (0) root         (0)    46781 2023-06-15 14:47:35.000000 blond-2.1.8/blond/impedances/impedance_sources.py
--rw-r--r--   0 root         (0) root         (0)     3458 2023-06-15 14:47:35.000000 blond-2.1.8/blond/impedances/induced_voltage_analytical.py
--rw-r--r--   0 root         (0) root         (0)    12030 2023-06-15 14:47:35.000000 blond-2.1.8/blond/impedances/music.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:48:02.340000 blond-2.1.8/blond/input_parameters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 14:47:35.000000 blond-2.1.8/blond/input_parameters/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24756 2023-06-15 14:47:35.000000 blond-2.1.8/blond/input_parameters/rf_parameters.py
--rw-r--r--   0 root         (0) root         (0)    19840 2023-06-15 14:47:35.000000 blond-2.1.8/blond/input_parameters/rf_parameters_options.py
--rw-r--r--   0 root         (0) root         (0)    17888 2023-06-15 14:47:35.000000 blond-2.1.8/blond/input_parameters/ring.py
--rw-r--r--   0 root         (0) root         (0)    22411 2023-06-15 14:47:35.000000 blond-2.1.8/blond/input_parameters/ring_options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:48:02.340000 blond-2.1.8/blond/llrf/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 14:47:35.000000 blond-2.1.8/blond/llrf/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21064 2023-06-15 14:47:35.000000 blond-2.1.8/blond/llrf/beam_feedback.py
--rw-r--r--   0 root         (0) root         (0)    37188 2023-06-15 14:47:35.000000 blond-2.1.8/blond/llrf/cavity_feedback.py
--rw-r--r--   0 root         (0) root         (0)    14013 2023-06-15 14:47:35.000000 blond-2.1.8/blond/llrf/impulse_response.py
--rw-r--r--   0 root         (0) root         (0)     2464 2023-06-15 14:47:35.000000 blond-2.1.8/blond/llrf/notch_filter.py
--rw-r--r--   0 root         (0) root         (0)     7117 2023-06-15 14:47:35.000000 blond-2.1.8/blond/llrf/offset_frequency.py
--rw-r--r--   0 root         (0) root         (0)     4157 2023-06-15 14:47:35.000000 blond-2.1.8/blond/llrf/rf_modulation.py
--rw-r--r--   0 root         (0) root         (0)    15492 2023-06-15 14:47:35.000000 blond-2.1.8/blond/llrf/rf_noise.py
--rw-r--r--   0 root         (0) root         (0)    18443 2023-06-15 14:47:35.000000 blond-2.1.8/blond/llrf/signal_processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:48:02.340000 blond-2.1.8/blond/monitors/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 14:47:35.000000 blond-2.1.8/blond/monitors/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21309 2023-06-15 14:47:35.000000 blond-2.1.8/blond/monitors/monitors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:48:02.344000 blond-2.1.8/blond/plots/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 14:47:35.000000 blond-2.1.8/blond/plots/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12199 2023-06-15 14:47:35.000000 blond-2.1.8/blond/plots/plot.py
--rw-r--r--   0 root         (0) root         (0)    10475 2023-06-15 14:47:35.000000 blond-2.1.8/blond/plots/plot_beams.py
--rw-r--r--   0 root         (0) root         (0)    13429 2023-06-15 14:47:35.000000 blond-2.1.8/blond/plots/plot_impedance.py
--rw-r--r--   0 root         (0) root         (0)    14720 2023-06-15 14:47:35.000000 blond-2.1.8/blond/plots/plot_llrf.py
--rw-r--r--   0 root         (0) root         (0)     1153 2023-06-15 14:47:35.000000 blond-2.1.8/blond/plots/plot_parameters.py
--rw-r--r--   0 root         (0) root         (0)     2912 2023-06-15 14:47:35.000000 blond-2.1.8/blond/plots/plot_slices.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:48:02.344000 blond-2.1.8/blond/synchrotron_radiation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 14:47:35.000000 blond-2.1.8/blond/synchrotron_radiation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5364 2023-06-15 14:47:35.000000 blond-2.1.8/blond/synchrotron_radiation/synchrotron_radiation.cpp
--rw-r--r--   0 root         (0) root         (0)     8043 2023-06-15 14:47:35.000000 blond-2.1.8/blond/synchrotron_radiation/synchrotron_radiation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:48:02.344000 blond-2.1.8/blond/toolbox/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 14:47:35.000000 blond-2.1.8/blond/toolbox/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5002 2023-06-15 14:47:35.000000 blond-2.1.8/blond/toolbox/action.py
--rw-r--r--   0 root         (0) root         (0)     7742 2023-06-15 14:47:35.000000 blond-2.1.8/blond/toolbox/diffusion.py
--rw-r--r--   0 root         (0) root         (0)     7514 2023-06-15 14:47:35.000000 blond-2.1.8/blond/toolbox/filters_and_fitting.py
--rw-r--r--   0 root         (0) root         (0)     1961 2023-06-15 14:47:35.000000 blond-2.1.8/blond/toolbox/logger.py
--rw-r--r--   0 root         (0) root         (0)     3311 2023-06-15 14:47:35.000000 blond-2.1.8/blond/toolbox/next_regular.py
--rw-r--r--   0 root         (0) root         (0)    20662 2023-06-15 14:47:35.000000 blond-2.1.8/blond/toolbox/parameter_scaling.py
--rw-r--r--   0 root         (0) root         (0)     2358 2023-06-15 14:47:35.000000 blond-2.1.8/blond/toolbox/tomoscope.cpp
--rw-r--r--   0 root         (0) root         (0)     4174 2023-06-15 14:47:35.000000 blond-2.1.8/blond/toolbox/tomoscope.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:48:02.344000 blond-2.1.8/blond/trackers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 14:47:35.000000 blond-2.1.8/blond/trackers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25355 2023-06-15 14:47:35.000000 blond-2.1.8/blond/trackers/tracker.py
--rw-r--r--   0 root         (0) root         (0)    30773 2023-06-15 14:47:35.000000 blond-2.1.8/blond/trackers/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:48:02.348000 blond-2.1.8/blond/utils/
--rw-r--r--   0 root         (0) root         (0)     3326 2023-06-15 14:47:35.000000 blond-2.1.8/blond/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8515 2023-06-15 14:47:35.000000 blond-2.1.8/blond/utils/bmath.py
--rw-r--r--   0 root         (0) root         (0)    47038 2023-06-15 14:47:35.000000 blond-2.1.8/blond/utils/butils_wrap_cpp.py
--rw-r--r--   0 root         (0) root         (0)    17329 2023-06-15 14:47:35.000000 blond-2.1.8/blond/utils/butils_wrap_python.py
--rw-r--r--   0 root         (0) root         (0)     3889 2023-06-15 14:47:35.000000 blond-2.1.8/blond/utils/data_check.py
--rw-r--r--   0 root         (0) root         (0)     2009 2023-06-15 14:47:35.000000 blond-2.1.8/blond/utils/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    14499 2023-06-15 14:47:35.000000 blond-2.1.8/blond/utils/mpi_config.py
--rw-r--r--   0 root         (0) root         (0)     3740 2023-06-15 14:47:35.000000 blond-2.1.8/blond/utils/track_iteration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:48:02.332000 blond-2.1.8/blond.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14287 2023-06-15 14:48:02.000000 blond-2.1.8/blond.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2834 2023-06-15 14:48:02.000000 blond-2.1.8/blond.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 14:48:02.000000 blond-2.1.8/blond.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      277 2023-06-15 14:48:02.000000 blond-2.1.8/blond.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-15 14:48:02.000000 blond-2.1.8/blond.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      338 2023-06-15 14:47:35.000000 blond-2.1.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       35 2023-06-15 14:47:35.000000 blond-2.1.8/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     8883 2023-06-15 14:47:35.000000 blond-2.1.8/sanity_check.py
--rw-r--r--   0 root         (0) root         (0)     1008 2023-06-15 14:48:02.348000 blond-2.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      169 2023-06-15 14:47:35.000000 blond-2.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:46:20.612000 blond-2.1.9/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-06-19 10:45:53.000000 blond-2.1.9/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)     6235 2023-06-19 10:45:53.000000 blond-2.1.9/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     3394 2023-06-19 10:45:53.000000 blond-2.1.9/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)     1887 2023-06-19 10:45:53.000000 blond-2.1.9/CHANGELOG
+-rw-r--r--   0 root         (0) root         (0)    35797 2023-06-19 10:45:53.000000 blond-2.1.9/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      208 2023-06-19 10:45:53.000000 blond-2.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    14287 2023-06-19 10:46:20.612000 blond-2.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13525 2023-06-19 10:45:53.000000 blond-2.1.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      794 2023-06-19 10:45:53.000000 blond-2.1.9/WARNINGS.txt
+-rw-r--r--   0 root         (0) root         (0)     1382 2023-06-19 10:45:53.000000 blond-2.1.9/appveyor.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:46:20.596000 blond-2.1.9/blond/
+-rw-r--r--   0 root         (0) root         (0)     2407 2023-06-19 10:45:53.000000 blond-2.1.9/blond/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-06-19 10:46:20.000000 blond-2.1.9/blond/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:46:20.600000 blond-2.1.9/blond/beam/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 10:45:53.000000 blond-2.1.9/blond/beam/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20226 2023-06-19 10:45:53.000000 blond-2.1.9/blond/beam/beam.py
+-rw-r--r--   0 root         (0) root         (0)     4424 2023-06-19 10:45:53.000000 blond-2.1.9/blond/beam/coasting_beam.py
+-rw-r--r--   0 root         (0) root         (0)    44819 2023-06-19 10:45:53.000000 blond-2.1.9/blond/beam/distributions.py
+-rw-r--r--   0 root         (0) root         (0)    40049 2023-06-19 10:45:53.000000 blond-2.1.9/blond/beam/distributions_multibunch.py
+-rw-r--r--   0 root         (0) root         (0)    23708 2023-06-19 10:45:53.000000 blond-2.1.9/blond/beam/profile.py
+-rw-r--r--   0 root         (0) root         (0)     5740 2023-06-19 10:45:53.000000 blond-2.1.9/blond/beam/sparse_histogram.cpp
+-rw-r--r--   0 root         (0) root         (0)     4796 2023-06-19 10:45:53.000000 blond-2.1.9/blond/beam/sparse_slices.py
+-rw-r--r--   0 root         (0) root         (0)    12857 2023-06-19 10:45:53.000000 blond-2.1.9/blond/compile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:46:20.604000 blond-2.1.9/blond/cpp_routines/
+-rw-r--r--   0 root         (0) root         (0)     3088 2023-06-19 10:45:53.000000 blond-2.1.9/blond/cpp_routines/beam_phase.cpp
+-rw-r--r--   0 root         (0) root         (0)    29022 2023-06-19 10:45:53.000000 blond-2.1.9/blond/cpp_routines/blondmath.cpp
+-rw-r--r--   0 root         (0) root         (0)    13334 2023-06-19 10:45:53.000000 blond-2.1.9/blond/cpp_routines/blondmath.h
+-rw-r--r--   0 root         (0) root         (0)     1316 2023-06-19 10:45:53.000000 blond-2.1.9/blond/cpp_routines/cos.h
+-rw-r--r--   0 root         (0) root         (0)     5747 2023-06-19 10:45:53.000000 blond-2.1.9/blond/cpp_routines/drift.cpp
+-rw-r--r--   0 root         (0) root         (0)     4376 2023-06-19 10:45:53.000000 blond-2.1.9/blond/cpp_routines/exp.h
+-rw-r--r--   0 root         (0) root         (0)     4661 2023-06-19 10:45:53.000000 blond-2.1.9/blond/cpp_routines/fast_resonator.cpp
+-rw-r--r--   0 root         (0) root         (0)    29481 2023-06-19 10:45:53.000000 blond-2.1.9/blond/cpp_routines/fft.cpp
+-rw-r--r--   0 root         (0) root         (0)     4419 2023-06-19 10:45:53.000000 blond-2.1.9/blond/cpp_routines/fft.h
+-rw-r--r--   0 root         (0) root         (0)    10031 2023-06-19 10:45:53.000000 blond-2.1.9/blond/cpp_routines/histogram.cpp
+-rw-r--r--   0 root         (0) root         (0)     3493 2023-06-19 10:45:53.000000 blond-2.1.9/blond/cpp_routines/kick.cpp
+-rw-r--r--   0 root         (0) root         (0)     6406 2023-06-19 10:45:53.000000 blond-2.1.9/blond/cpp_routines/linear_interp_kick.cpp
+-rw-r--r--   0 root         (0) root         (0)    15181 2023-06-19 10:45:53.000000 blond-2.1.9/blond/cpp_routines/music_track.cpp
+-rw-r--r--   0 root         (0) root         (0)      169 2023-06-19 10:45:53.000000 blond-2.1.9/blond/cpp_routines/openmp.cpp
+-rw-r--r--   0 root         (0) root         (0)      245 2023-06-19 10:45:53.000000 blond-2.1.9/blond/cpp_routines/openmp.h
+-rw-r--r--   0 root         (0) root         (0)     1960 2023-06-19 10:45:53.000000 blond-2.1.9/blond/cpp_routines/sin.h
+-rw-r--r--   0 root         (0) root         (0)     5871 2023-06-19 10:45:53.000000 blond-2.1.9/blond/cpp_routines/sincos.h
+-rw-r--r--   0 root         (0) root         (0)     7480 2023-06-19 10:45:53.000000 blond-2.1.9/blond/cpp_routines/vdtcore_common.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:46:20.604000 blond-2.1.9/blond/gpu/
+-rw-r--r--   0 root         (0) root         (0)     2561 2023-06-19 10:45:53.000000 blond-2.1.9/blond/gpu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11763 2023-06-19 10:45:53.000000 blond-2.1.9/blond/gpu/butils_wrap_cupy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:46:20.604000 blond-2.1.9/blond/gpu/cuda_kernels/
+-rw-r--r--   0 root         (0) root         (0)    14390 2023-06-19 10:45:53.000000 blond-2.1.9/blond/gpu/cuda_kernels/kernels_double.cu
+-rw-r--r--   0 root         (0) root         (0)    14135 2023-06-19 10:45:53.000000 blond-2.1.9/blond/gpu/cuda_kernels/kernels_single.cu
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:46:20.604000 blond-2.1.9/blond/impedances/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 10:45:53.000000 blond-2.1.9/blond/impedances/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39010 2023-06-19 10:45:53.000000 blond-2.1.9/blond/impedances/impedance.py
+-rw-r--r--   0 root         (0) root         (0)    46781 2023-06-19 10:45:53.000000 blond-2.1.9/blond/impedances/impedance_sources.py
+-rw-r--r--   0 root         (0) root         (0)     3458 2023-06-19 10:45:53.000000 blond-2.1.9/blond/impedances/induced_voltage_analytical.py
+-rw-r--r--   0 root         (0) root         (0)    12030 2023-06-19 10:45:53.000000 blond-2.1.9/blond/impedances/music.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:46:20.604000 blond-2.1.9/blond/input_parameters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 10:45:53.000000 blond-2.1.9/blond/input_parameters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24756 2023-06-19 10:45:53.000000 blond-2.1.9/blond/input_parameters/rf_parameters.py
+-rw-r--r--   0 root         (0) root         (0)    19840 2023-06-19 10:45:53.000000 blond-2.1.9/blond/input_parameters/rf_parameters_options.py
+-rw-r--r--   0 root         (0) root         (0)    17888 2023-06-19 10:45:53.000000 blond-2.1.9/blond/input_parameters/ring.py
+-rw-r--r--   0 root         (0) root         (0)    22411 2023-06-19 10:45:53.000000 blond-2.1.9/blond/input_parameters/ring_options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:46:20.604000 blond-2.1.9/blond/llrf/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 10:45:53.000000 blond-2.1.9/blond/llrf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21064 2023-06-19 10:45:53.000000 blond-2.1.9/blond/llrf/beam_feedback.py
+-rw-r--r--   0 root         (0) root         (0)    37188 2023-06-19 10:45:53.000000 blond-2.1.9/blond/llrf/cavity_feedback.py
+-rw-r--r--   0 root         (0) root         (0)    14013 2023-06-19 10:45:53.000000 blond-2.1.9/blond/llrf/impulse_response.py
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-06-19 10:45:53.000000 blond-2.1.9/blond/llrf/notch_filter.py
+-rw-r--r--   0 root         (0) root         (0)     7117 2023-06-19 10:45:53.000000 blond-2.1.9/blond/llrf/offset_frequency.py
+-rw-r--r--   0 root         (0) root         (0)     4157 2023-06-19 10:45:53.000000 blond-2.1.9/blond/llrf/rf_modulation.py
+-rw-r--r--   0 root         (0) root         (0)    15492 2023-06-19 10:45:53.000000 blond-2.1.9/blond/llrf/rf_noise.py
+-rw-r--r--   0 root         (0) root         (0)    18443 2023-06-19 10:45:53.000000 blond-2.1.9/blond/llrf/signal_processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:46:20.604000 blond-2.1.9/blond/monitors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 10:45:53.000000 blond-2.1.9/blond/monitors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21309 2023-06-19 10:45:53.000000 blond-2.1.9/blond/monitors/monitors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:46:20.608000 blond-2.1.9/blond/plots/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 10:45:53.000000 blond-2.1.9/blond/plots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12199 2023-06-19 10:45:53.000000 blond-2.1.9/blond/plots/plot.py
+-rw-r--r--   0 root         (0) root         (0)    10475 2023-06-19 10:45:53.000000 blond-2.1.9/blond/plots/plot_beams.py
+-rw-r--r--   0 root         (0) root         (0)    13429 2023-06-19 10:45:53.000000 blond-2.1.9/blond/plots/plot_impedance.py
+-rw-r--r--   0 root         (0) root         (0)    14720 2023-06-19 10:45:53.000000 blond-2.1.9/blond/plots/plot_llrf.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-06-19 10:45:53.000000 blond-2.1.9/blond/plots/plot_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-06-19 10:45:53.000000 blond-2.1.9/blond/plots/plot_slices.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:46:20.608000 blond-2.1.9/blond/synchrotron_radiation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 10:45:53.000000 blond-2.1.9/blond/synchrotron_radiation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5364 2023-06-19 10:45:53.000000 blond-2.1.9/blond/synchrotron_radiation/synchrotron_radiation.cpp
+-rw-r--r--   0 root         (0) root         (0)     8043 2023-06-19 10:45:53.000000 blond-2.1.9/blond/synchrotron_radiation/synchrotron_radiation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:46:20.608000 blond-2.1.9/blond/toolbox/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 10:45:53.000000 blond-2.1.9/blond/toolbox/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5002 2023-06-19 10:45:53.000000 blond-2.1.9/blond/toolbox/action.py
+-rw-r--r--   0 root         (0) root         (0)     7742 2023-06-19 10:45:53.000000 blond-2.1.9/blond/toolbox/diffusion.py
+-rw-r--r--   0 root         (0) root         (0)     7514 2023-06-19 10:45:53.000000 blond-2.1.9/blond/toolbox/filters_and_fitting.py
+-rw-r--r--   0 root         (0) root         (0)     1961 2023-06-19 10:45:53.000000 blond-2.1.9/blond/toolbox/logger.py
+-rw-r--r--   0 root         (0) root         (0)     3311 2023-06-19 10:45:53.000000 blond-2.1.9/blond/toolbox/next_regular.py
+-rw-r--r--   0 root         (0) root         (0)    20662 2023-06-19 10:45:53.000000 blond-2.1.9/blond/toolbox/parameter_scaling.py
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-06-19 10:45:53.000000 blond-2.1.9/blond/toolbox/tomoscope.cpp
+-rw-r--r--   0 root         (0) root         (0)     4174 2023-06-19 10:45:53.000000 blond-2.1.9/blond/toolbox/tomoscope.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:46:20.608000 blond-2.1.9/blond/trackers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 10:45:53.000000 blond-2.1.9/blond/trackers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25355 2023-06-19 10:45:53.000000 blond-2.1.9/blond/trackers/tracker.py
+-rw-r--r--   0 root         (0) root         (0)    30773 2023-06-19 10:45:53.000000 blond-2.1.9/blond/trackers/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:46:20.612000 blond-2.1.9/blond/utils/
+-rw-r--r--   0 root         (0) root         (0)     3326 2023-06-19 10:45:53.000000 blond-2.1.9/blond/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8515 2023-06-19 10:45:53.000000 blond-2.1.9/blond/utils/bmath.py
+-rw-r--r--   0 root         (0) root         (0)    47038 2023-06-19 10:45:53.000000 blond-2.1.9/blond/utils/butils_wrap_cpp.py
+-rw-r--r--   0 root         (0) root         (0)    17329 2023-06-19 10:45:53.000000 blond-2.1.9/blond/utils/butils_wrap_python.py
+-rw-r--r--   0 root         (0) root         (0)     3889 2023-06-19 10:45:53.000000 blond-2.1.9/blond/utils/data_check.py
+-rw-r--r--   0 root         (0) root         (0)     2009 2023-06-19 10:45:53.000000 blond-2.1.9/blond/utils/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    14499 2023-06-19 10:45:53.000000 blond-2.1.9/blond/utils/mpi_config.py
+-rw-r--r--   0 root         (0) root         (0)     3740 2023-06-19 10:45:53.000000 blond-2.1.9/blond/utils/track_iteration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:46:20.600000 blond-2.1.9/blond.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14287 2023-06-19 10:46:20.000000 blond-2.1.9/blond.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2834 2023-06-19 10:46:20.000000 blond-2.1.9/blond.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 10:46:20.000000 blond-2.1.9/blond.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      284 2023-06-19 10:46:20.000000 blond-2.1.9/blond.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-19 10:46:20.000000 blond-2.1.9/blond.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      338 2023-06-19 10:45:53.000000 blond-2.1.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       35 2023-06-19 10:45:53.000000 blond-2.1.9/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     8883 2023-06-19 10:45:53.000000 blond-2.1.9/sanity_check.py
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-06-19 10:46:20.612000 blond-2.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      169 2023-06-19 10:45:53.000000 blond-2.1.9/setup.py
```

### Comparing `blond-2.1.8/.gitignore` & `blond-2.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/.gitlab-ci.yml` & `blond-2.1.9/.gitlab-ci.yml`

 * *Files 3% similar despite different names*

```diff
@@ -54,40 +54,40 @@
       junit: ${project_root}junit-report.xml
     paths:
       - ${project_root}coverage-html/*
     # reports:
     #   junit: ${project_root}/coverage-report.xml
 
 
-# test_py_37:
-#   variables:  
-#     PY_VERSION: "3.7"
-#   image: python:${PY_VERSION}
-#   stage: test
-#   extends:
-#     - .before
-#     - .main
-#     - .after
-#     # - .publish
+test_py_38:
+  variables:  
+    PY_VERSION: "3.8"
+  image: python:${PY_VERSION}
+  stage: test
+  extends:
+    - .before
+    - .main
+    - .after
+    - .publish
 
-test_py_39:
+test_py_310:
   variables:
-    PY_VERSION: "3.9"
+    PY_VERSION: "3.10"
   image: python:${PY_VERSION}
   stage: test
   extends:
     - .before
     - .main
     - .after
-    - .publish
+    # - .publish
 
 
-release_sdist_39:
+release_sdist_38:
   variables:
-    PY_VERSION: "3.9"
+    PY_VERSION: "3.8"
   image: python:${PY_VERSION}
   stage: deploy
   extends:
     - .on_tag
   before_script:
    - apt-get update
    - apt-get install -y git
@@ -105,21 +105,21 @@
         --username="${PYPI_USERNAME}"
         --password="${PYPI_PASSWORD}"
         dist/*.tar.gz
 
 
 pages:
   variables:
-    PY_VERSION: "3.9"
+    PY_VERSION: "3.8"
   image: python:${PY_VERSION}
   script:
    - cd ${project_root}
    - mkdir public
    - python3 -m pip install --upgrade pip
    - python3 -m pip install -v ${project_root}[doc]
    - make -C __doc html
    - cp -r __doc/_build/html/* public/
   artifacts:
     paths:
      - ${project_root}public
   only:
-   - master
+   - master
```

### Comparing `blond-2.1.8/CHANGELOG` & `blond-2.1.9/CHANGELOG`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/LICENSE.txt` & `blond-2.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/PKG-INFO` & `blond-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: blond
-Version: 2.1.8
+Version: 2.1.9
 Summary: CERN code for simulating longitudinal beam dynamics in synchrotrons.
 Home-page: https://gitlab.cern.ch/blond/BLonD
 Author: Helga Timko
 Author-email: helga.timko@cern.ch
 Maintainer: Konstantinos Iliakis
 License: GPL
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: all
 License-File: LICENSE.txt
```

### Comparing `blond-2.1.8/README.md` & `blond-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/WARNINGS.txt` & `blond-2.1.9/WARNINGS.txt`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/appveyor.yml` & `blond-2.1.9/appveyor.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 image:
   - Visual Studio 2017
 environment:
   matrix:
     # - PATH: C:\Python36-x64;C:\mingw-w64\x86_64-7.2.0-posix-seh-rt_v5-rev1\mingw64\bin;%PATH%
-    - PATH: C:\Python37-x64;C:\mingw-w64\x86_64-7.2.0-posix-seh-rt_v5-rev1\mingw64\bin;%PATH%
+    # - PATH: C:\Python37-x64;C:\mingw-w64\x86_64-7.2.0-posix-seh-rt_v5-rev1\mingw64\bin;%PATH%
     - PATH: C:\Python38-x64;C:\mingw-w64\x86_64-7.2.0-posix-seh-rt_v5-rev1\mingw64\bin;%PATH%
   # matrix:
     # - VSVER: Visual Studio 14 2015
     # - VSVER: Visual Studio 14 2015 Win64
 
 # cache: 
 #   - C:\ProgramData\chocolatey\bin -> appveyor.yml
```

### Comparing `blond-2.1.8/blond/__init__.py` & `blond-2.1.9/blond/__init__.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/beam/beam.py` & `blond-2.1.9/blond/beam/beam.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/beam/coasting_beam.py` & `blond-2.1.9/blond/beam/coasting_beam.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/beam/distributions.py` & `blond-2.1.9/blond/beam/distributions.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/beam/distributions_multibunch.py` & `blond-2.1.9/blond/beam/distributions_multibunch.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/beam/profile.py` & `blond-2.1.9/blond/beam/profile.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/beam/sparse_histogram.cpp` & `blond-2.1.9/blond/beam/sparse_histogram.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/beam/sparse_slices.py` & `blond-2.1.9/blond/beam/sparse_slices.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/compile.py` & `blond-2.1.9/blond/compile.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/cpp_routines/beam_phase.cpp` & `blond-2.1.9/blond/cpp_routines/beam_phase.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/cpp_routines/blondmath.cpp` & `blond-2.1.9/blond/cpp_routines/blondmath.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/cpp_routines/blondmath.h` & `blond-2.1.9/blond/cpp_routines/blondmath.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/cpp_routines/cos.h` & `blond-2.1.9/blond/cpp_routines/cos.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/cpp_routines/drift.cpp` & `blond-2.1.9/blond/cpp_routines/drift.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/cpp_routines/exp.h` & `blond-2.1.9/blond/cpp_routines/exp.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/cpp_routines/fast_resonator.cpp` & `blond-2.1.9/blond/cpp_routines/fast_resonator.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/cpp_routines/fft.cpp` & `blond-2.1.9/blond/cpp_routines/fft.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/cpp_routines/fft.h` & `blond-2.1.9/blond/cpp_routines/fft.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/cpp_routines/histogram.cpp` & `blond-2.1.9/blond/cpp_routines/histogram.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/cpp_routines/kick.cpp` & `blond-2.1.9/blond/cpp_routines/kick.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/cpp_routines/linear_interp_kick.cpp` & `blond-2.1.9/blond/cpp_routines/linear_interp_kick.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/cpp_routines/music_track.cpp` & `blond-2.1.9/blond/cpp_routines/music_track.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/cpp_routines/sin.h` & `blond-2.1.9/blond/cpp_routines/sin.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/cpp_routines/sincos.h` & `blond-2.1.9/blond/cpp_routines/sincos.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/cpp_routines/vdtcore_common.h` & `blond-2.1.9/blond/cpp_routines/vdtcore_common.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/gpu/__init__.py` & `blond-2.1.9/blond/gpu/__init__.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/gpu/butils_wrap_cupy.py` & `blond-2.1.9/blond/gpu/butils_wrap_cupy.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/gpu/cuda_kernels/kernels_double.cu` & `blond-2.1.9/blond/gpu/cuda_kernels/kernels_double.cu`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/gpu/cuda_kernels/kernels_single.cu` & `blond-2.1.9/blond/gpu/cuda_kernels/kernels_single.cu`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/impedances/impedance.py` & `blond-2.1.9/blond/impedances/impedance.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/impedances/impedance_sources.py` & `blond-2.1.9/blond/impedances/impedance_sources.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/impedances/induced_voltage_analytical.py` & `blond-2.1.9/blond/impedances/induced_voltage_analytical.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/impedances/music.py` & `blond-2.1.9/blond/impedances/music.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/input_parameters/rf_parameters.py` & `blond-2.1.9/blond/input_parameters/rf_parameters.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/input_parameters/rf_parameters_options.py` & `blond-2.1.9/blond/input_parameters/rf_parameters_options.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/input_parameters/ring.py` & `blond-2.1.9/blond/input_parameters/ring.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/input_parameters/ring_options.py` & `blond-2.1.9/blond/input_parameters/ring_options.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/llrf/beam_feedback.py` & `blond-2.1.9/blond/llrf/beam_feedback.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/llrf/cavity_feedback.py` & `blond-2.1.9/blond/llrf/cavity_feedback.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/llrf/impulse_response.py` & `blond-2.1.9/blond/llrf/impulse_response.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/llrf/notch_filter.py` & `blond-2.1.9/blond/llrf/notch_filter.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/llrf/offset_frequency.py` & `blond-2.1.9/blond/llrf/offset_frequency.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/llrf/rf_modulation.py` & `blond-2.1.9/blond/llrf/rf_modulation.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/llrf/rf_noise.py` & `blond-2.1.9/blond/llrf/rf_noise.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/llrf/signal_processing.py` & `blond-2.1.9/blond/llrf/signal_processing.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/monitors/monitors.py` & `blond-2.1.9/blond/monitors/monitors.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/plots/plot.py` & `blond-2.1.9/blond/plots/plot.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/plots/plot_beams.py` & `blond-2.1.9/blond/plots/plot_beams.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/plots/plot_impedance.py` & `blond-2.1.9/blond/plots/plot_impedance.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/plots/plot_llrf.py` & `blond-2.1.9/blond/plots/plot_llrf.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/plots/plot_parameters.py` & `blond-2.1.9/blond/plots/plot_parameters.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/plots/plot_slices.py` & `blond-2.1.9/blond/plots/plot_slices.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/synchrotron_radiation/synchrotron_radiation.cpp` & `blond-2.1.9/blond/synchrotron_radiation/synchrotron_radiation.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/synchrotron_radiation/synchrotron_radiation.py` & `blond-2.1.9/blond/synchrotron_radiation/synchrotron_radiation.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/toolbox/action.py` & `blond-2.1.9/blond/toolbox/action.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/toolbox/diffusion.py` & `blond-2.1.9/blond/toolbox/diffusion.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/toolbox/filters_and_fitting.py` & `blond-2.1.9/blond/toolbox/filters_and_fitting.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/toolbox/logger.py` & `blond-2.1.9/blond/toolbox/logger.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/toolbox/next_regular.py` & `blond-2.1.9/blond/toolbox/next_regular.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/toolbox/parameter_scaling.py` & `blond-2.1.9/blond/toolbox/parameter_scaling.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/toolbox/tomoscope.cpp` & `blond-2.1.9/blond/toolbox/tomoscope.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/toolbox/tomoscope.py` & `blond-2.1.9/blond/toolbox/tomoscope.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/trackers/tracker.py` & `blond-2.1.9/blond/trackers/tracker.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/trackers/utilities.py` & `blond-2.1.9/blond/trackers/utilities.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/utils/__init__.py` & `blond-2.1.9/blond/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/utils/bmath.py` & `blond-2.1.9/blond/utils/bmath.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/utils/butils_wrap_cpp.py` & `blond-2.1.9/blond/utils/butils_wrap_cpp.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/utils/butils_wrap_python.py` & `blond-2.1.9/blond/utils/butils_wrap_python.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/utils/data_check.py` & `blond-2.1.9/blond/utils/data_check.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/utils/exceptions.py` & `blond-2.1.9/blond/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/utils/mpi_config.py` & `blond-2.1.9/blond/utils/mpi_config.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond/utils/track_iteration.py` & `blond-2.1.9/blond/utils/track_iteration.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/blond.egg-info/PKG-INFO` & `blond-2.1.9/blond.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: blond
-Version: 2.1.8
+Version: 2.1.9
 Summary: CERN code for simulating longitudinal beam dynamics in synchrotrons.
 Home-page: https://gitlab.cern.ch/blond/BLonD
 Author: Helga Timko
 Author-email: helga.timko@cern.ch
 Maintainer: Konstantinos Iliakis
 License: GPL
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: all
 License-File: LICENSE.txt
```

### Comparing `blond-2.1.8/blond.egg-info/SOURCES.txt` & `blond-2.1.9/blond.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/sanity_check.py` & `blond-2.1.9/sanity_check.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.8/setup.cfg` & `blond-2.1.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 	Operating System :: OS Independent
 	Intended Audience :: Science/Research
 	Natural Language :: English
 	Topic :: Scientific/Engineering :: Physics
 
 [options]
 packages = find:
-python_requires = >=3.6
+python_requires = >=3.8
 install_requires = 
 	numpy
 	scipy
 	h5py
-	matplotlib
+	matplotlib>=3.7.1
 	mpmath
 include_package_data = True
 
 [options.extras_require]
 test = 
 	pytest
 lint =
```

