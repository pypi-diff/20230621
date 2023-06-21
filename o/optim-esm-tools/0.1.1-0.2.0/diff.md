# Comparing `tmp/optim_esm_tools-0.1.1.tar.gz` & `tmp/optim_esm_tools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optim_esm_tools-0.1.1.tar", last modified: Tue Jun 13 14:34:50 2023, max compression
+gzip compressed data, was "optim_esm_tools-0.2.0.tar", last modified: Wed Jun 21 09:03:42 2023, max compression
```

## Comparing `optim_esm_tools-0.1.1.tar` & `optim_esm_tools-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:34:50.392854 optim_esm_tools-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-13 14:34:50.392854 optim_esm_tools-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:34:50.388853 optim_esm_tools-0.1.1/extra_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/extra_requirements/requirements-tests.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:34:50.392854 optim_esm_tools-0.1.1/optim_esm_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/optim_esm_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/optim_esm_tools/_test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:34:50.392854 optim_esm_tools-0.1.1/optim_esm_tools/analyze/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/optim_esm_tools/analyze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/optim_esm_tools/analyze/analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/optim_esm_tools/analyze/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)    25487 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/optim_esm_tools/analyze/cmip_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/optim_esm_tools/analyze/xarray_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:34:50.392854 optim_esm_tools-0.1.1/optim_esm_tools/synda_files/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/optim_esm_tools/synda_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/optim_esm_tools/synda_files/format_synda.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/optim_esm_tools/synda_files/synda_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/optim_esm_tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:34:50.392854 optim_esm_tools-0.1.1/optim_esm_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-13 14:34:50.000000 optim_esm_tools-0.1.1/optim_esm_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-13 14:34:50.000000 optim_esm_tools-0.1.1/optim_esm_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:34:50.000000 optim_esm_tools-0.1.1/optim_esm_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:34:50.000000 optim_esm_tools-0.1.1/optim_esm_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-13 14:34:50.000000 optim_esm_tools-0.1.1/optim_esm_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-13 14:34:50.000000 optim_esm_tools-0.1.1/optim_esm_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-13 14:34:50.392854 optim_esm_tools-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:34:50.392854 optim_esm_tools-0.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/test/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/test/test_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/test/test_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/test/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/test/test_xarray_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:42.070011 optim_esm_tools-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-06-21 09:03:42.070011 optim_esm_tools-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:42.066011 optim_esm_tools-0.2.0/extra_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/extra_requirements/requirements-tests.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:42.066011 optim_esm_tools-0.2.0/optim_esm_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/optim_esm_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/optim_esm_tools/_test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:42.066011 optim_esm_tools-0.2.0/optim_esm_tools/analyze/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/optim_esm_tools/analyze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/optim_esm_tools/analyze/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/optim_esm_tools/analyze/cmip_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/optim_esm_tools/analyze/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15510 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/optim_esm_tools/analyze/region_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/optim_esm_tools/analyze/tipping_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/optim_esm_tools/analyze/xarray_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:42.066011 optim_esm_tools-0.2.0/optim_esm_tools/cmip_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/optim_esm_tools/cmip_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/optim_esm_tools/cmip_files/find_matches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/optim_esm_tools/cmip_files/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/optim_esm_tools/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:42.066011 optim_esm_tools-0.2.0/optim_esm_tools/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/optim_esm_tools/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10868 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/optim_esm_tools/plotting/map_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/optim_esm_tools/plotting/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:42.066011 optim_esm_tools-0.2.0/optim_esm_tools/synda_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/optim_esm_tools/synda_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/optim_esm_tools/synda_files/format_synda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/optim_esm_tools/synda_files/synda_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10868 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/optim_esm_tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:42.066011 optim_esm_tools-0.2.0/optim_esm_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-06-21 09:03:41.000000 optim_esm_tools-0.2.0/optim_esm_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-21 09:03:42.000000 optim_esm_tools-0.2.0/optim_esm_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 09:03:41.000000 optim_esm_tools-0.2.0/optim_esm_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 09:03:41.000000 optim_esm_tools-0.2.0/optim_esm_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-21 09:03:41.000000 optim_esm_tools-0.2.0/optim_esm_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-21 09:03:41.000000 optim_esm_tools-0.2.0/optim_esm_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-21 09:03:42.070011 optim_esm_tools-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:42.070011 optim_esm_tools-0.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/test/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/test/test_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/test/test_find_matches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/test/test_pangeo_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/test/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/test/test_region_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/test/test_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/test/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-21 09:03:36.000000 optim_esm_tools-0.2.0/test/test_xarray_tools.py
```

### Comparing `optim_esm_tools-0.1.1/optim_esm_tools/synda_files/synda_files.py` & `optim_esm_tools-0.2.0/optim_esm_tools/synda_files/synda_files.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 class SyndaViewer:
     """Visualize synda downloads as a tree structure"""
 
     def __init__(
         self,
-        base: str = '/nobackup/users/angevaar/synda/data',
+        base: str = os.path.join(os.environ.get('ST_HOME', 'NO ST HOME?'), 'data'),
         max_depth: typing.Optional[int] = None,
         show_files: bool = False,
         concatenate_folders: bool = True,
         count_files: bool = False,
     ):
         """
         Viewer for Synda Folder structure
```

### Comparing `optim_esm_tools-0.1.1/optim_esm_tools.egg-info/SOURCES.txt` & `optim_esm_tools-0.2.0/optim_esm_tools.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,41 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 extra_requirements/requirements-tests.txt
 optim_esm_tools/__init__.py
 optim_esm_tools/_test_utils.py
+optim_esm_tools/config.py
 optim_esm_tools/utils.py
 optim_esm_tools.egg-info/PKG-INFO
 optim_esm_tools.egg-info/SOURCES.txt
 optim_esm_tools.egg-info/dependency_links.txt
 optim_esm_tools.egg-info/not-zip-safe
 optim_esm_tools.egg-info/requires.txt
 optim_esm_tools.egg-info/top_level.txt
 optim_esm_tools/analyze/__init__.py
-optim_esm_tools/analyze/analyze.py
 optim_esm_tools/analyze/clustering.py
 optim_esm_tools/analyze/cmip_handler.py
+optim_esm_tools/analyze/globals.py
+optim_esm_tools/analyze/region_finding.py
+optim_esm_tools/analyze/tipping_criteria.py
 optim_esm_tools/analyze/xarray_tools.py
+optim_esm_tools/cmip_files/__init__.py
+optim_esm_tools/cmip_files/find_matches.py
+optim_esm_tools/cmip_files/io.py
+optim_esm_tools/plotting/__init__.py
+optim_esm_tools/plotting/map_maker.py
+optim_esm_tools/plotting/plot.py
 optim_esm_tools/synda_files/__init__.py
 optim_esm_tools/synda_files/format_synda.py
 optim_esm_tools/synda_files/synda_files.py
 test/test_basics.py
 test/test_clustering.py
+test/test_find_matches.py
+test/test_pangeo_download.py
+test/test_plotting.py
+test/test_region_finding.py
 test/test_utils.py
 test/test_viewer.py
 test/test_workflow.py
 test/test_xarray_tools.py
```

### Comparing `optim_esm_tools-0.1.1/setup.py` & `optim_esm_tools-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 readme = open('README.md').read()
 history = open('HISTORY.md').read()
 requirements = open_requirements('requirements.txt')
 
 setuptools.setup(
     name='optim_esm_tools',
-    version='0.1.1',
+    version='0.2.0',
     description='Tools for OptimESM',
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/markdown',
     author='Joran R. Angevaare',
     url='https://github.com/JoranAngevaare/optim_esm_tools',
     packages=setuptools.find_packages() + ['extra_requirements'],
     package_dir={
```

### Comparing `optim_esm_tools-0.1.1/test/test_clustering.py` & `optim_esm_tools-0.2.0/test/test_clustering.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     ds = ds.isel(time=0)
     assert np.all(np.shape(ds['var']) > np.array([2, 2]))
 
     clusters, masks = clustering.build_cluster_mask(ds['var'] > 0, ds['x'], ds['y'])
     assert len(clusters) == len(masks) == 0
 
 
-def test_clustering_double_blob(npoints=100, res_x=5, res_y=5):
+def test_clustering_double_blob(npoints=100, res_x=3, res_y=3):
     ds = optim_esm_tools._test_utils.minimal_xr_ds().copy()
     ds = ds.isel(time=0)
 
     arr = np.zeros_like(ds['var'])
     len_x, len_y = arr.shape[0:]
     x0, y0, x1, y1 = len_x // 4, len_y // 4, len_x // 2, len_y // 2
 
@@ -34,10 +34,23 @@
     assert np.all(np.shape(ds['var']) > np.array([2, 2]))
 
     clusters, masks = clustering.build_cluster_mask(
         ds['var'] > 1,
         ds['x'],
         ds['y'],
         max_distance_km=1000,
-        cluster_opts=dict(min_samples=2),
+        min_samples=2,
+    )
+    assert len(clusters) == len(masks)
+    assert len(clusters) == 2
+
+
+def test_geopy_alternative():
+    xs, ys = np.random.rand(1, 4).reshape(2, 2)
+    xs *= 360
+    ys = ys * 180 - 90
+    # LAT:LON!
+    coords = np.array([ys, xs]).T
+    print(coords)
+    assert np.isclose(
+        clustering._distance_bf(coords), clustering._distance(coords), rtol=0.1
     )
-    assert len(clusters) == len(masks) == 2
```

### Comparing `optim_esm_tools-0.1.1/test/test_workflow.py` & `optim_esm_tools-0.2.0/test/test_workflow.py`

 * *Files 15% similar despite different names*

```diff
@@ -39,21 +39,35 @@
         data_set = oet.synda_files.format_synda.load_glob(self.ayear_file)
 
     def test_make_map(self):
         data_set = oet.analyze.cmip_handler.read_ds(os.path.split(self.ayear_file)[0])
         oet.analyze.cmip_handler.MapMaker(data_set=data_set).plot_all(2)
         plt.clf()
 
-    def test_example_time_series(self):
-        data_set = oet.analyze.cmip_handler.read_ds(os.path.split(self.ayear_file)[0])
-        oet.analyze.cmip_handler.example_time_series(data_set)
-        plt.clf()
-
     def test_map_maker_time_series(self):
         data_set = oet.analyze.cmip_handler.read_ds(os.path.split(self.ayear_file)[0])
         oet.analyze.cmip_handler.MapMaker(data_set=data_set).time_series()
         plt.clf()
 
     @classmethod
     def tearDownClass(cls) -> None:
         os.remove(cls.ayear_file)
         return super().tearDownClass()
+
+
+class Units(unittest.TestCase):
+    def test_apply_relative_units(self, unit='relative', refresh=False):
+        from optim_esm_tools._test_utils import year_means, get_file_from_pangeo
+
+        data_set = oet.analyze.cmip_handler.read_ds(
+            os.path.split(
+                year_means(
+                    get_file_from_pangeo('ssp585', refresh=refresh), refresh=refresh
+                )
+            )[0],
+            condition_kwargs=dict(unit=unit),
+            _file_name='test_merged.nc',
+        )
+        mm = oet.analyze.cmip_handler.MapMaker(data_set=data_set)
+
+    def test_apply_std_unit(self):
+        self.test_apply_relative_units(unit='std')
```

