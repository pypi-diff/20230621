# Comparing `tmp/tristan-0.2.1.tar.gz` & `tmp/tristan-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tristan-0.2.1.tar", last modified: Thu Dec 15 09:42:37 2022, max compression
+gzip compressed data, was "tristan-0.2.2.tar", last modified: Wed Jun 21 13:28:37 2023, max compression
```

## Comparing `tristan-0.2.1.tar` & `tristan-0.2.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-12-15 09:42:37.765415 tristan-0.2.1/
--rw-r--r--   0 vsts      (1001) docker     (122)     1081 2022-12-15 09:42:22.000000 tristan-0.2.1/LICENCE
--rw-r--r--   0 vsts      (1001) docker     (122)     1120 2022-12-15 09:42:37.765415 tristan-0.2.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      194 2022-12-15 09:42:22.000000 tristan-0.2.1/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      193 2022-12-15 09:42:22.000000 tristan-0.2.1/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     1599 2022-12-15 09:42:37.765415 tristan-0.2.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      128 2022-12-15 09:42:22.000000 tristan-0.2.1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-12-15 09:42:37.761415 tristan-0.2.1/src/
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-12-15 09:42:37.765415 tristan-0.2.1/src/tristan/
--rw-r--r--   0 vsts      (1001) docker     (122)     1285 2022-12-15 09:42:22.000000 tristan-0.2.1/src/tristan/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8516 2022-12-15 09:42:22.000000 tristan-0.2.1/src/tristan/binning.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-12-15 09:42:37.765415 tristan-0.2.1/src/tristan/command_line/
--rw-r--r--   0 vsts      (1001) docker     (122)    13967 2022-12-15 09:42:22.000000 tristan-0.2.1/src/tristan/command_line/__init__.py
--rwxr-xr-x   0 vsts      (1001) docker     (122)     3657 2022-12-15 09:42:22.000000 tristan-0.2.1/src/tristan/command_line/apply_flat_field.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1991 2022-12-15 09:42:22.000000 tristan-0.2.1/src/tristan/command_line/cues.py
--rw-r--r--   0 vsts      (1001) docker     (122)    23091 2022-12-15 09:42:22.000000 tristan-0.2.1/src/tristan/command_line/images.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1626 2022-12-15 09:42:22.000000 tristan-0.2.1/src/tristan/command_line/vds.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8898 2022-12-15 09:42:22.000000 tristan-0.2.1/src/tristan/data.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-12-15 09:42:37.765415 tristan-0.2.1/src/tristan/diagnostics/
--rw-r--r--   0 vsts      (1001) docker     (122)     1357 2022-12-15 09:42:22.000000 tristan-0.2.1/src/tristan/diagnostics/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3864 2022-12-15 09:42:22.000000 tristan-0.2.1/src/tristan/diagnostics/check_files.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5930 2022-12-15 09:42:22.000000 tristan-0.2.1/src/tristan/diagnostics/check_valid_events.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1187 2022-12-15 09:42:22.000000 tristan-0.2.1/src/tristan/diagnostics/diagnostics_log.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13829 2022-12-15 09:42:22.000000 tristan-0.2.1/src/tristan/diagnostics/find_trigger_intervals.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8937 2022-12-15 09:42:22.000000 tristan-0.2.1/src/tristan/vds.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-12-15 09:42:37.765415 tristan-0.2.1/src/tristan.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1120 2022-12-15 09:42:37.000000 tristan-0.2.1/src/tristan.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      779 2022-12-15 09:42:37.000000 tristan-0.2.1/src/tristan.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2022-12-15 09:42:37.000000 tristan-0.2.1/src/tristan.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      384 2022-12-15 09:42:37.000000 tristan-0.2.1/src/tristan.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2022-12-15 09:42:37.000000 tristan-0.2.1/src/tristan.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)       99 2022-12-15 09:42:37.000000 tristan-0.2.1/src/tristan.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        8 2022-12-15 09:42:37.000000 tristan-0.2.1/src/tristan.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-21 13:28:37.599331 tristan-0.2.2/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1081 2023-06-21 13:28:29.000000 tristan-0.2.2/LICENCE
+-rw-r--r--   0 vsts      (1001) docker     (122)     1191 2023-06-21 13:28:37.599331 tristan-0.2.2/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      194 2023-06-21 13:28:29.000000 tristan-0.2.2/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      194 2023-06-21 13:28:29.000000 tristan-0.2.2/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1874 2023-06-21 13:28:37.599331 tristan-0.2.2/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      128 2023-06-21 13:28:29.000000 tristan-0.2.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-21 13:28:37.595331 tristan-0.2.2/src/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-21 13:28:37.599331 tristan-0.2.2/src/tristan/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1285 2023-06-21 13:28:29.000000 tristan-0.2.2/src/tristan/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8516 2023-06-21 13:28:29.000000 tristan-0.2.2/src/tristan/binning.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-21 13:28:37.599331 tristan-0.2.2/src/tristan/command_line/
+-rw-r--r--   0 vsts      (1001) docker     (122)    14689 2023-06-21 13:28:29.000000 tristan-0.2.2/src/tristan/command_line/__init__.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     3657 2023-06-21 13:28:29.000000 tristan-0.2.2/src/tristan/command_line/apply_flat_field.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1991 2023-06-21 13:28:29.000000 tristan-0.2.2/src/tristan/command_line/cues.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    29995 2023-06-21 13:28:29.000000 tristan-0.2.2/src/tristan/command_line/images.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1626 2023-06-21 13:28:29.000000 tristan-0.2.2/src/tristan/command_line/vds.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9005 2023-06-21 13:28:29.000000 tristan-0.2.2/src/tristan/data.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-21 13:28:37.599331 tristan-0.2.2/src/tristan/diagnostics/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1357 2023-06-21 13:28:29.000000 tristan-0.2.2/src/tristan/diagnostics/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3864 2023-06-21 13:28:29.000000 tristan-0.2.2/src/tristan/diagnostics/check_files.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5930 2023-06-21 13:28:29.000000 tristan-0.2.2/src/tristan/diagnostics/check_valid_events.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1458 2023-06-21 13:28:29.000000 tristan-0.2.2/src/tristan/diagnostics/diagnostics_log.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14922 2023-06-21 13:28:29.000000 tristan-0.2.2/src/tristan/diagnostics/find_trigger_intervals.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8937 2023-06-21 13:28:29.000000 tristan-0.2.2/src/tristan/vds.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-21 13:28:37.599331 tristan-0.2.2/src/tristan.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1191 2023-06-21 13:28:37.000000 tristan-0.2.2/src/tristan.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      779 2023-06-21 13:28:37.000000 tristan-0.2.2/src/tristan.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-21 13:28:37.000000 tristan-0.2.2/src/tristan.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      384 2023-06-21 13:28:37.000000 tristan-0.2.2/src/tristan.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-21 13:28:37.000000 tristan-0.2.2/src/tristan.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      180 2023-06-21 13:28:37.000000 tristan-0.2.2/src/tristan.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        8 2023-06-21 13:28:37.000000 tristan-0.2.2/src/tristan.egg-info/top_level.txt
```

### Comparing `tristan-0.2.1/LICENCE` & `tristan-0.2.2/LICENCE`

 * *Files identical despite different names*

### Comparing `tristan-0.2.1/PKG-INFO` & `tristan-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tristan
-Version: 0.2.1
+Version: 0.2.2
 Summary: Tools for processing event-mode X-ray data
 Author: Diamond Light Source — Data Analysis
 Author-email: scientificsoftware@diamond.ac.uk
 License: MIT
 Project-URL: Documentation, https://tristan.readthedocs.io/
 Project-URL: GitHub, https://github.com/DiamondLightSource/python-tristan
 Project-URL: Bug-Tracker, https://github.com/DiamondLightSource/python-tristan/issues
@@ -13,14 +13,16 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENCE
 
 # tristan
 
 A set of prototype data processing tools for Tristan, the experimental [Timepix3-based](https://doi.org/10.1016/j.nima.2016.04.075) event-mode X-ray detector at Diamond Light Source.
```

### Comparing `tristan-0.2.1/setup.cfg` & `tristan-0.2.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tristan
-version = 0.2.1
+version = 0.2.2
 description = Tools for processing event-mode X-ray data
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Diamond Light Source — Data Analysis
 author_email = scientificsoftware@diamond.ac.uk
 license = MIT
 license_file = LICENCE
@@ -13,43 +13,61 @@
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Natural Language :: English
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 keywords = 
 	x-ray
 	tristan
 	timepix
 project-urls = 
 	Documentation = https://tristan.readthedocs.io/
 	GitHub = https://github.com/DiamondLightSource/python-tristan
 	Bug-Tracker = https://github.com/DiamondLightSource/python-tristan/issues
 
 [options]
 include_package_data = True
 install_requires = 
 	dask[array,diagnostics,distributed] != 2021.3.*
-	h5py
-	hdf5plugin
-	nexgen >= 0.6.8
+	h5py>=3.8
+	hdf5plugin>=4.0.1
+	nexgen >= 0.6.20
 	numpy
 	pandas
 	pint
 	zarr
 packages = find:
 package_dir = 
 	=src
 python_requires = >=3.8
 zip_safe = False
 
+[options.extras_require]
+dev = 
+	black
+	pytest-cov
+	pytest-random-order
+	pre-commit
+	flake8
+	build
+
 [options.packages.find]
 where = src
 
+[isort]
+profile = black
+float_to_top = true
+
+[flake8]
+max-line-length = 88
+extend-ignore = E203,E266,E402,E501,W503,E741
+
 [options.entry_points]
 console_scripts = 
 	apply-flat-field = tristan.command_line.apply_flat_field:main
 	check-tristan-files = tristan.diagnostics.check_files:cli
 	cues = tristan.command_line.cues:main
 	find-trigger-intervals = tristan.diagnostics.find_trigger_intervals:cli
 	images = tristan.command_line.images:main
```

### Comparing `tristan-0.2.1/src/tristan/__init__.py` & `tristan-0.2.2/src/tristan/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Source.
 """
 
 from __future__ import annotations
 
 __author__ = "Diamond Light Source — Data Analysis Group"
 __email__ = "dataanalysis@diamond.ac.uk"
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 __version_tuple__ = tuple(int(x) for x in __version__.split("."))
 
 import dask
 import pint
 from dask.distributed import progress, wait
 
 ureg = pint.UnitRegistry()
```

### Comparing `tristan-0.2.1/src/tristan/binning.py` & `tristan-0.2.2/src/tristan/binning.py`

 * *Files identical despite different names*

### Comparing `tristan-0.2.1/src/tristan/command_line/__init__.py` & `tristan-0.2.2/src/tristan/command_line/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -417,7 +417,26 @@
     "'--exposure-time .5ms', '-e 500µs' or '-e 500us'.  Unspecified units default to "
     "seconds.",
     type=units_of_time,
 )
 group.add_argument(
     "-x", "--num-sequences", help="Number of image sequences.", type=positive_int
 )
+
+# A parser for specifying a pair of trigger signals with which to gate event processing.
+gate_parser = argparse.ArgumentParser(add_help=False)
+gate_parser.add_argument(
+    "-g",
+    "--gate-open",
+    help="Trigger signal denoting the start of each gate period.",
+    choices=triggers.keys(),
+    required=True,
+)
+gate_parser.add_argument(
+    "-c",
+    "--gate-close",
+    help="Trigger signal denoting the end of each gate period (optional).  If not "
+    "provided, this will default to the complementary signal to the '--gate-open' "
+    "value.  For example, if the '--gate-open' signal is 'TTL-rising', "
+    "the --gate-close signal will default to 'TTL-falling', and vice versa.",
+    choices=triggers.keys(),
+)
```

### Comparing `tristan-0.2.1/src/tristan/command_line/apply_flat_field.py` & `tristan-0.2.2/src/tristan/command_line/apply_flat_field.py`

 * *Files identical despite different names*

### Comparing `tristan-0.2.1/src/tristan/command_line/cues.py` & `tristan-0.2.2/src/tristan/command_line/cues.py`

 * *Files identical despite different names*

### Comparing `tristan-0.2.1/src/tristan/command_line/images.py` & `tristan-0.2.2/src/tristan/command_line/images.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,32 +25,33 @@
 from ..binning import (
     align_bins,
     create_cache,
     events_to_images,
     find_start_end,
     find_time_bins,
     make_images,
-    valid_events,
 )
 from ..data import (
     cue_keys,
     cue_times,
     cues,
     event_location_key,
     event_time_key,
     first_cue_time,
     latrd_data,
     pixel_index,
     seconds,
+    valid_events,
 )
 from . import (
     check_multiple_output_files,
     check_output_file,
     data_files,
     exposure_parser,
+    gate_parser,
     image_output_parser,
     input_parser,
     interval_parser,
     trigger_parser,
     triggers,
     version_parser,
 )
@@ -272,29 +273,15 @@
     aggregated, providing a single stack of images that captures the evolution of the
     response of the measurement to a pump signal.
     """
     write_mode = "w" if args.force else "x"
     output_file = check_output_file(args.output_file, args.stem, "images", args.force)
 
     input_nexus = args.data_dir / f"{args.stem}.nxs"
-    if input_nexus.exists():
-        try:
-            # Write output NeXus file if we have an input NeXus file.
-            output_nexus = CopyTristanNexus.single_image_nexus(
-                output_file, input_nexus, write_mode=write_mode
-            )
-        except FileExistsError:
-            sys.exit(
-                f"This output file already exists:\n\t"
-                f"{output_file.with_suffix('.nxs')}\n"
-                "Use '-f' to override, "
-                "or specify a different output file path with '-o'."
-            )
-    else:
-        output_nexus = None
+    if not input_nexus.exists():
         print(
             "Could not find a NeXus file containing experiment metadata.\n"
             "Resorting to writing raw image data without accompanying metadata."
         )
 
     image_size = args.image_size or determine_image_size(input_nexus)
 
@@ -315,14 +302,33 @@
         sys.exit(f"Only one '{cues[trigger_type]}' signal found.  Two or more needed.")
 
     end = da.diff(trigger_times).min()
     exposure_time, num_images = args.exposure_time, args.num_images
     exposure_time, _, num_images = exposure(0, end, exposure_time, num_images)
     bins = np.linspace(0, end, num_images + 1, dtype=np.uint64)
 
+    if input_nexus.exists():
+        try:
+            # Write output NeXus file if we have an input NeXus file.
+            output_nexus = CopyTristanNexus.single_image_nexus(
+                output_file,
+                input_nexus,
+                write_mode=write_mode,
+                pump_probe_bins=num_images,
+            )
+        except FileExistsError:
+            sys.exit(
+                f"This output file already exists:\n\t"
+                f"{output_file.with_suffix('.nxs')}\n"
+                "Use '-f' to override, "
+                "or specify a different output file path with '-o'."
+            )
+    else:
+        output_nexus = None
+
     print(
         f"Binning events into {num_images} images with an exposure time of "
         f"{exposure_time:.3g~#P} according to the time elapsed since the most "
         f"recent '{cues[trigger_type]}' signal."
     )
 
     # Make a cache for the images.
@@ -525,14 +531,162 @@
 
     # Delete the Zarr store.
     store.clear()
 
     print(f"Images written to\n\t{output_nexus_pattern or out_file_pattern}")
 
 
+def gated_images_cli(args):
+    """Utility to bin events into a sequence of images according to a gating signal."""
+    write_mode = "w" if args.force else "x"
+    output_file = check_output_file(args.output_file, args.stem, "images", args.force)
+
+    input_nexus = args.data_dir / f"{args.stem}.nxs"
+    if not input_nexus.exists():
+        print(
+            "Could not find a NeXus file containing experiment metadata.\n"
+            "Resorting to writing raw image data without accompanying metadata."
+        )
+
+    image_size = args.image_size or determine_image_size(input_nexus)
+
+    raw_files, _ = data_files(args.data_dir, args.stem)
+
+    # If gate_close isn't specified, default to the complementary signal to gate_open.
+    gate_open = triggers.get(args.gate_open)
+    gate_close = triggers.get(args.gate_close) or gate_open ^ (1 << 5)
+
+    with latrd_data(raw_files, keys=cue_keys) as cues_data:
+        print("Finding detector shutter open and close times.")
+        with ProgressBar():
+            start, end = find_start_end(cues_data)
+
+        print("Finding gate signal times.")
+        # Here we assume no synchronization issues:
+        # falling edges always recorded after rising edges.
+        open_times = cue_times(cues_data, gate_open, after=start)
+        close_times = cue_times(cues_data, gate_close, before=end)
+        with ProgressBar():
+            open_times, close_times = dask.compute(open_times, close_times)
+
+    if not open_times.size:
+        sys.exit(f"Could not find a '{cues[gate_open]}' signal.")
+    if not close_times.size:
+        sys.exit(f"Could not find a '{cues[gate_close]}' signal.")
+
+    open_times = np.sort(open_times)
+    close_times = np.sort(close_times)
+
+    if not open_times.size == close_times.size:
+        # If size difference is just one, look for missing one right before/after
+        # shutters and use shutter open/close timestamp as first/last gate
+        if abs(open_times.size - close_times.size) > 1:
+            sys.exit(
+                "Found a non-matching number of gate open and close signals:\n\t"
+                f"Number of '{cues[gate_open]}' signals: {open_times.size}\n\t"
+                f"Number of '{cues[gate_close]}' signals: {close_times.size}\n"
+                f"Note that signals before the shutter open time are ignored."
+            )
+        else:
+            if open_times[-1] > close_times[-1]:
+                print(
+                    "WARNING! \n\t"
+                    f"Missing last '{cues[gate_close]}' signal.\n\t"
+                    f"Shutter close timestamp will be used instead for last image."
+                )
+                # Append shutter close to close_times
+                close_times = np.append(close_times, end)
+            elif open_times[0] > close_times[0]:
+                print(
+                    "WARNING! \n\t"
+                    f"Missing first '{cues[gate_open]}' signal.\n\t"
+                    f"Shutter open timestamp will be used instead for first image."
+                )
+                # Insert shutter open to open times
+                open_times = np.insert(open_times, 0, start)
+            else:
+                sys.exit(
+                    "Found a non-matching number of gate open and close signals:\n\t"
+                    f"Number of '{cues[gate_open]}' signals: {open_times.size}\n\t"
+                    f"Number of '{cues[gate_close]}' signals: {close_times.size}\n"
+                )
+
+    num_images = open_times.size
+    bins = np.linspace(0, num_images, num_images + 1, dtype=np.uint64)
+
+    if input_nexus.exists():
+        try:
+            # Write output NeXus file if we have an input NeXus file.
+            output_nexus = CopyTristanNexus.serial_images_nexus(
+                output_file,
+                input_nexus,
+                nbins=num_images,
+                write_mode=write_mode,
+            )
+        except FileExistsError:
+            sys.exit(
+                f"This output file already exists:\n\t"
+                f"{output_file.with_suffix('.nxs')}\n"
+                "Use '-f' to override, "
+                "or specify a different output file path with '-o'."
+            )
+    else:
+        output_nexus = None
+
+    print(f"Binning events into {num_images} images.")
+
+    # Make a cache for the images.
+    images = create_cache(output_file, num_images, image_size)
+
+    with latrd_data(raw_files, keys=(event_location_key, event_time_key)) as data:
+        # Consider only those events that occur between the start and end times.
+        data = valid_events(data, start, end)
+
+        # Gate the events.
+        event_times = data[event_time_key].astype(np.int64).values
+        open_index = da.digitize(event_times, open_times) - 1
+        close_index = da.digitize(event_times, close_times)
+        # Look for events that happen after gate open and before gate close
+        # Eliminate invalid events by looking at the open and close index
+        valid = open_index == close_index
+        valid = dd.from_dask_array(valid, index=data.index)
+
+        # Convert the event IDs to a form that is suitable for a NumPy bincount.
+        data[event_location_key] = pixel_index(data[event_location_key], image_size)
+
+        columns = event_location_key, "time_bin"
+        dtypes = data.dtypes
+        dtypes["time_bin"] = dtypes.pop(event_time_key)
+
+        meta = pd.DataFrame(columns=columns).astype(dtype=dtypes)
+        # Enumerate the image in the stack to which each event belongs
+        data = data.map_partitions(find_time_bins, bins=bins, meta=meta)
+        data["time_bin"] = open_index
+        data = data[valid]
+
+        # Bin to images, partition by partition.
+        data = dd.map_partitions(
+            make_images, data, image_size, images, meta=meta, enforce_metadata=False
+        )
+
+        print("Computing the binned images.")
+        # Use multi-threading, rather than multi-processing.
+        with Client(processes=False):
+            compute_with_progress(data)
+
+    print("Transferring the images to the output file.")
+    with h5py.File(output_file, write_mode) as f:
+        zarr.copy_all(zarr.open(images.store), f, **Bitshuffle())
+
+    # Delete the Zarr store.
+    images.store.clear()
+
+    print(f"Images written to\n\t{output_nexus or output_file}")
+
+
 parser = argparse.ArgumentParser(description=__doc__, parents=[version_parser])
 subparsers = parser.add_subparsers(
     help="Choose the manner in which to create images.",
     required=True,
     dest="sub-command",
 )
 
@@ -599,12 +753,22 @@
         trigger_parser,
         exposure_parser,
         interval_parser,
     ],
 )
 parser_multiple_sequences.set_defaults(func=multiple_sequences_cli)
 
+parser_serial = subparsers.add_parser(
+    "serial",
+    description="Bin events into images, gated with trigger signals.\n\n"
+    "Events will be binned into as many images as there are gate signals, one image "
+    "per gate.  Each 'gate-open' signal is taken as the start of an exposure and the "
+    "next 'gate-close' signal is taken as the end of the exposure.",
+    parents=[version_parser, input_parser, image_output_parser, gate_parser],
+)
+parser_serial.set_defaults(func=gated_images_cli)
+
 
 def main(args=None):
     """Perform the image binning with a user-specified sub-command."""
     args = parser.parse_args(args)
     args.func(args)
```

### Comparing `tristan-0.2.1/src/tristan/command_line/vds.py` & `tristan-0.2.2/src/tristan/command_line/vds.py`

 * *Files identical despite different names*

### Comparing `tristan-0.2.1/src/tristan/data.py` & `tristan-0.2.2/src/tristan/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,20 @@
     if after:
         message_incidences &= data[cue_time_key] >= after
     first_index = message_incidences.idxmax().compute()
     if first_index or data[cue_id_key].loc[0].compute().values == message:
         return data[cue_time_key].loc[first_index]
 
 
-def cue_times(data: dd.DataFrame, message: int, after: int | None = None) -> da.Array:
+def cue_times(
+    data: dd.DataFrame,
+    message: int,
+    after: int | None = None,
+    before: int | None = None,
+) -> da.Array:
     """
     Find the timestamps of all instances of a cue message in a Tristan data set.
 
     The found timestamps are de-duplicated.
 
     Args:
         data:     A DataFrame of LATRD data.  Must contain one column for cue id
@@ -161,14 +166,16 @@
     Returns:
         The timestamps, measured in clock cycles from the global synchronisation
         signal, de-duplicated.
     """
     index = data[cue_id_key] == message
     if after:
         index &= data[cue_time_key] >= after
+    if before:
+        index &= data[cue_time_key] <= before
     return da.unique(data[cue_time_key][index].values)
 
 
 def seconds(timestamp: int, reference: int = 0) -> Quantity:
     """
     Convert a Tristan timestamp to seconds, measured from a given reference timestamp.
```

### Comparing `tristan-0.2.1/src/tristan/diagnostics/__init__.py` & `tristan-0.2.2/src/tristan/diagnostics/__init__.py`

 * *Files identical despite different names*

### Comparing `tristan-0.2.1/src/tristan/diagnostics/check_files.py` & `tristan-0.2.2/src/tristan/diagnostics/check_files.py`

 * *Files identical despite different names*

### Comparing `tristan-0.2.1/src/tristan/diagnostics/check_valid_events.py` & `tristan-0.2.2/src/tristan/diagnostics/check_valid_events.py`

 * *Files identical despite different names*

### Comparing `tristan-0.2.1/src/tristan/diagnostics/diagnostics_log.py` & `tristan-0.2.2/src/tristan/diagnostics/diagnostics_log.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Logging configuration for diagnostics.
+Logging configuration for Tristan diagnostics.
 """
 
 import logging
 import logging.config
 
 logging_config = {
     "version": 1,
@@ -31,14 +31,20 @@
     },
 }
 
 logging.config.dictConfig(logging_config)
 
 
 def config(logfile: str = None, write_mode: str = "a"):
+    """Configure the logger.
+
+    Args:
+        logfile (str, optional): If passed, create a file handle for the logger to write a logfile output. Defaults to None.
+        write_mode (str, optional): Writing mode for the logfile output. Defaults to "a".
+    """
     diag_logger = logging.getLogger("TristanDiagnostics")
     if logfile:
         fileFormatter = logging.Formatter(
             "%(asctime)s - %(levelname)s -- %(message)s",
             datefmt="%d-%m-%Y %I:%M:%S",
         )
         FH = logging.FileHandler(logfile, mode=write_mode, encoding="utf-8")
```

### Comparing `tristan-0.2.1/src/tristan/diagnostics/find_trigger_intervals.py` & `tristan-0.2.2/src/tristan/diagnostics/find_trigger_intervals.py`

 * *Files 6% similar despite different names*

```diff
@@ -233,27 +233,27 @@
     logger.info("----- SUMMARY -----")
     for el in res:
         for k, v in el.items():
             shutters = [v["Shutter open"], v["Shutter close"]]
             logger.info(f"--- {k} ---")
             logger.info("SHUTTERS")
             if len(shutters[0]) > 0 and len(shutters[1]) > 0:
-                logger.info(f"Shutter open timestamp: {shutters[0][0]:.4f}")
-                logger.info(f"Shutter close timestamp: {shutters[1][0]:.4f}")
+                logger.info(f"Shutter open timestamp: {shutters[0][0]:.4f}.")
+                logger.info(f"Shutter close timestamp: {shutters[1][0]:.4f}.")
                 diff0 = shutters[1][0] - shutters[0][0]
                 logger.info(
                     f"Total time between shutter opening and closing: {diff0:.4f} s."
                 )
             elif len(shutters[0]) == 0 or len(shutters[1]) == 0:
                 logger.warning("Missing shutter information!")
                 logger.warning(
-                    f"Number of shutter open timestamps found: {len(shutters[0])}"
+                    f"Number of shutter open timestamps found: {len(shutters[0])}."
                 )
                 logger.warning(
-                    f"Number of shutter close timestamps found: {len(shutters[1])}"
+                    f"Number of shutter close timestamps found: {len(shutters[1])}."
                 )
             logger.info("LVDS")
             if len(v["LVDS re"]) > 0 and len(v["LVDS fe"]) > 0:
                 logger.info(
                     f"Found {len(v['LVDS re'])} rising edges and {len(v['LVDS fe'])} falling edges."
                 )
                 logger.info(f"LVDS rising edge timestamp: {v['LVDS re'][0]:.4f}.")
@@ -269,14 +269,16 @@
                 )
                 logger.warning(
                     f"Number of LVDS fe timestamps found: {len(v['LVDS fe'])}"
                 )
             logger.info("TTL")
             logger.info(f"Found {len(v['TTL re'])} rising edges.\n")
             if len(v["TTL re"]) > 0:
+                logger.info(f"First TTL rising edge timestamp: {v['TTL re'][0]:.4f} .")
+                logger.info(f"Last TTL rising edge timestamp: {v['TTL re'][-1]:.4f} .")
                 d = [i - v["TTL re"][n - 1] for n, i in enumerate(v["TTL re"])][1:]
                 d_avg = np.average(d) if len(d) else np.nan
                 logger.info(
                     f"Average time interval between one TTL re and the next: {d_avg:.4} s"
                 )
                 if len(v["LVDS re"]) > 0:
                     diff2 = v["TTL re"][0] - v["LVDS re"][0]
@@ -317,24 +319,40 @@
             # If SSX, print out SYNC info.
             if args.expt == "ssx":
                 logger.info("SYNC")
                 if len(v["SYNC re"]) > 0 and len(v["SYNC fe"]) > 0:
                     logger.info(
                         f"Found {len(v['SYNC re'])} rising edges and {len(v['SYNC fe'])} falling edges."
                     )
+                    logger.info(
+                        f"First SYNC rising edge timestamp: {v['SYNC re'][0]:.4f}."
+                    )
+                    logger.info(
+                        f"Last SYNC falling edge timestamp: {v['SYNC fe'][-1]:.4f}."
+                    )
+                    if v["SYNC re"][0] < shutters[0][0]:
+                        logger.warning(
+                            "First SYNC rising edge was recorded before the shutter open signal! \n"
+                            f"Timestamp difference: {shutters[0][0] - v['SYNC re'][0]} s."
+                        )
+                    if v["SYNC fe"][-1] > shutters[1][0]:
+                        logger.warning(
+                            "Last SYNC falling edge was recorded after the shutter close signal! \n"
+                            f"Timestamp difference: {v['SYNC fe'][-1] - shutters[1][0]} s."
+                        )
                     diff4 = [b - a for a, b in zip(v["SYNC re"], v["SYNC fe"])]
                     avg4 = np.average(diff4) if len(diff4) else np.nan
                     logger.info(
-                        f"Average time interval between SYNC re and fe: {avg4:.4f} s"
+                        f"Average time interval between SYNC re and fe: {avg4:.4f} s."
                     )
                     if len(v["TTL re"]) == len(v["SYNC re"]):
                         diff5 = [b - a for a, b in zip(v["TTL re"], v["SYNC re"])]
                         avg5 = np.average(diff5) if len(diff5) else np.nan
                         logger.info(
-                            f"Average time interval between TTL re and SYNC re: {avg5:.4f} s"
+                            f"Average time interval between TTL re and SYNC re: {avg5:.4f} s."
                         )
                     else:
                         logger.error(
                             "The number of TTL re and SYNC re doesn't match. Impossible to accurately calculate time difference."
                         )
                 elif len(v["SYNC re"]) == 0:
                     logger.warning("No SYNC rising edges found!")
```

### Comparing `tristan-0.2.1/src/tristan/vds.py` & `tristan-0.2.2/src/tristan/vds.py`

 * *Files identical despite different names*

### Comparing `tristan-0.2.1/src/tristan.egg-info/PKG-INFO` & `tristan-0.2.2/src/tristan.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tristan
-Version: 0.2.1
+Version: 0.2.2
 Summary: Tools for processing event-mode X-ray data
 Author: Diamond Light Source — Data Analysis
 Author-email: scientificsoftware@diamond.ac.uk
 License: MIT
 Project-URL: Documentation, https://tristan.readthedocs.io/
 Project-URL: GitHub, https://github.com/DiamondLightSource/python-tristan
 Project-URL: Bug-Tracker, https://github.com/DiamondLightSource/python-tristan/issues
@@ -13,14 +13,16 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENCE
 
 # tristan
 
 A set of prototype data processing tools for Tristan, the experimental [Timepix3-based](https://doi.org/10.1016/j.nima.2016.04.075) event-mode X-ray detector at Diamond Light Source.
```

### Comparing `tristan-0.2.1/src/tristan.egg-info/SOURCES.txt` & `tristan-0.2.2/src/tristan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

