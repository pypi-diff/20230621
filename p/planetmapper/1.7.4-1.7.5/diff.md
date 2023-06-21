# Comparing `tmp/planetmapper-1.7.4.tar.gz` & `tmp/planetmapper-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planetmapper-1.7.4.tar", last modified: Tue Jun 20 10:50:27 2023, max compression
+gzip compressed data, was "planetmapper-1.7.5.tar", last modified: Wed Jun 21 20:40:38 2023, max compression
```

## Comparing `planetmapper-1.7.4.tar` & `planetmapper-1.7.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:50:27.166611 planetmapper-1.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-20 10:50:15.000000 planetmapper-1.7.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-06-20 10:50:27.166611 planetmapper-1.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-20 10:50:15.000000 planetmapper-1.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:50:27.162611 planetmapper-1.7.4/planetmapper/
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-06-20 10:50:15.000000 planetmapper-1.7.4/planetmapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28536 2023-06-20 10:50:15.000000 planetmapper-1.7.4/planetmapper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-06-20 10:50:15.000000 planetmapper-1.7.4/planetmapper/basic_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    81538 2023-06-20 10:50:15.000000 planetmapper-1.7.4/planetmapper/body.py
--rw-r--r--   0 runner    (1001) docker     (123)   112154 2023-06-20 10:50:15.000000 planetmapper-1.7.4/planetmapper/body_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-20 10:50:15.000000 planetmapper-1.7.4/planetmapper/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:50:27.162611 planetmapper-1.7.4/planetmapper/data/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-20 10:50:15.000000 planetmapper-1.7.4/planetmapper/data/ring_aliases.json
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-20 10:50:15.000000 planetmapper-1.7.4/planetmapper/data/rings.json
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-20 10:50:15.000000 planetmapper-1.7.4/planetmapper/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)   118682 2023-06-20 10:50:15.000000 planetmapper-1.7.4/planetmapper/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-06-20 10:50:15.000000 planetmapper-1.7.4/planetmapper/kernel_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    46604 2023-06-20 10:50:15.000000 planetmapper-1.7.4/planetmapper/observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-06-20 10:50:15.000000 planetmapper-1.7.4/planetmapper/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-06-20 10:50:15.000000 planetmapper-1.7.4/planetmapper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:50:27.162611 planetmapper-1.7.4/planetmapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-06-20 10:50:27.000000 planetmapper-1.7.4/planetmapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-20 10:50:27.000000 planetmapper-1.7.4/planetmapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 10:50:27.000000 planetmapper-1.7.4/planetmapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-20 10:50:27.000000 planetmapper-1.7.4/planetmapper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-20 10:50:27.000000 planetmapper-1.7.4/planetmapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 10:50:27.000000 planetmapper-1.7.4/planetmapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-20 10:50:15.000000 planetmapper-1.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 10:50:27.166611 planetmapper-1.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-20 10:50:15.000000 planetmapper-1.7.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:50:27.162611 planetmapper-1.7.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    25552 2023-06-20 10:50:15.000000 planetmapper-1.7.4/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-20 10:50:15.000000 planetmapper-1.7.4/tests/test_basic_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    34896 2023-06-20 10:50:15.000000 planetmapper-1.7.4/tests/test_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    39958 2023-06-20 10:50:15.000000 planetmapper-1.7.4/tests/test_body_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 10:50:15.000000 planetmapper-1.7.4/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-20 10:50:15.000000 planetmapper-1.7.4/tests/test_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-20 10:50:15.000000 planetmapper-1.7.4/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-20 10:50:15.000000 planetmapper-1.7.4/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-06-20 10:50:15.000000 planetmapper-1.7.4/tests/test_kernel_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    28477 2023-06-20 10:50:15.000000 planetmapper-1.7.4/tests/test_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-20 10:50:15.000000 planetmapper-1.7.4/tests/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-06-20 10:50:15.000000 planetmapper-1.7.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:40:38.400402 planetmapper-1.7.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-21 20:40:28.000000 planetmapper-1.7.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-06-21 20:40:38.400402 planetmapper-1.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-21 20:40:28.000000 planetmapper-1.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:40:38.396402 planetmapper-1.7.5/planetmapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-06-21 20:40:28.000000 planetmapper-1.7.5/planetmapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28542 2023-06-21 20:40:28.000000 planetmapper-1.7.5/planetmapper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-06-21 20:40:28.000000 planetmapper-1.7.5/planetmapper/basic_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81538 2023-06-21 20:40:28.000000 planetmapper-1.7.5/planetmapper/body.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112285 2023-06-21 20:40:28.000000 planetmapper-1.7.5/planetmapper/body_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-21 20:40:28.000000 planetmapper-1.7.5/planetmapper/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:40:38.400402 planetmapper-1.7.5/planetmapper/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-21 20:40:28.000000 planetmapper-1.7.5/planetmapper/data/ring_aliases.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-21 20:40:28.000000 planetmapper-1.7.5/planetmapper/data/rings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-21 20:40:28.000000 planetmapper-1.7.5/planetmapper/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118682 2023-06-21 20:40:28.000000 planetmapper-1.7.5/planetmapper/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-06-21 20:40:28.000000 planetmapper-1.7.5/planetmapper/kernel_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46604 2023-06-21 20:40:28.000000 planetmapper-1.7.5/planetmapper/observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-06-21 20:40:28.000000 planetmapper-1.7.5/planetmapper/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-06-21 20:40:28.000000 planetmapper-1.7.5/planetmapper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:40:38.400402 planetmapper-1.7.5/planetmapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-06-21 20:40:38.000000 planetmapper-1.7.5/planetmapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-21 20:40:38.000000 planetmapper-1.7.5/planetmapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 20:40:38.000000 planetmapper-1.7.5/planetmapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-21 20:40:38.000000 planetmapper-1.7.5/planetmapper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-21 20:40:38.000000 planetmapper-1.7.5/planetmapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-21 20:40:38.000000 planetmapper-1.7.5/planetmapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-21 20:40:28.000000 planetmapper-1.7.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 20:40:38.400402 planetmapper-1.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-21 20:40:28.000000 planetmapper-1.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:40:38.400402 planetmapper-1.7.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    25552 2023-06-21 20:40:28.000000 planetmapper-1.7.5/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-21 20:40:28.000000 planetmapper-1.7.5/tests/test_basic_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35990 2023-06-21 20:40:28.000000 planetmapper-1.7.5/tests/test_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41788 2023-06-21 20:40:28.000000 planetmapper-1.7.5/tests/test_body_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-21 20:40:28.000000 planetmapper-1.7.5/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-21 20:40:28.000000 planetmapper-1.7.5/tests/test_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-21 20:40:28.000000 planetmapper-1.7.5/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-21 20:40:28.000000 planetmapper-1.7.5/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-06-21 20:40:28.000000 planetmapper-1.7.5/tests/test_kernel_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28477 2023-06-21 20:40:28.000000 planetmapper-1.7.5/tests/test_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-21 20:40:28.000000 planetmapper-1.7.5/tests/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-06-21 20:40:28.000000 planetmapper-1.7.5/tests/test_utils.py
```

### Comparing `planetmapper-1.7.4/LICENSE.txt` & `planetmapper-1.7.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.4/PKG-INFO` & `planetmapper-1.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetmapper
-Version: 1.7.4
+Version: 1.7.5
 Summary: PlanetMapper: A Python module for visualising, navigating and mapping Solar System observations
 Home-page: https://github.com/ortk95/planetmapper
 Download-URL: https://pypi.org/project/planetmapper/
 Author: Oliver King
 Author-email: oliver.king95@gmail.com
 License: MIT
 Project-URL: Documentation, https://planetmapper.readthedocs.io/
```

### Comparing `planetmapper-1.7.4/README.md` & `planetmapper-1.7.5/README.md`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.4/planetmapper/__init__.py` & `planetmapper-1.7.5/planetmapper/__init__.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.4/planetmapper/base.py` & `planetmapper-1.7.5/planetmapper/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,15 +328,15 @@
         Args:
             mjd: Float representing MJD.
 
         Returns:
             Python datetime object corresponding to `mjd`. This datetime is timezone
             aware and set to the UTC timezone.
         """
-        dtm: datetime.datetime = astropy.time.Time(mjd, format='mjd').datetime
+        dtm = cast(datetime.datetime, astropy.time.Time(mjd, format='mjd').datetime)
         return dtm.replace(tzinfo=datetime.timezone.utc)
 
     def speed_of_light(self) -> float:
         """
         Return the speed of light in km/s. This is a convenience function to call
         `spice.clight()`.
```

### Comparing `planetmapper-1.7.4/planetmapper/basic_body.py` & `planetmapper-1.7.5/planetmapper/basic_body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.4/planetmapper/body.py` & `planetmapper-1.7.5/planetmapper/body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.4/planetmapper/body_xy.py` & `planetmapper-1.7.5/planetmapper/body_xy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1253,26 +1253,28 @@
 
     def plot_map(
         self,
         map_img: np.ndarray,
         ax: Axes | None = None,
         *,
         wireframe_kwargs: dict[str, Any] | None = None,
+        add_wireframe: bool = True,
         **kwargs,
     ) -> QuadMesh:
         """
         Utility function to easily plot a mapped image using `plt.imshow` with
         appropriate extents, axis labels, gridlines etc.
 
         Args:
             map_img: Image to plot.
             ax: Matplotlib axis to use for plotting. If `ax` is None (the default), then
                 a new figure and axis is created.
             wireframe_kwargs: Dictionary of arguments passed to
                 :func:`plot_map_wireframe`.
+            add_wireframe: Enable/disable plotting of wireframe.
             **kwargs: Additional arguments are passed to
                 :func:`generate_map_coordinates` to specify the map projection used, and
                 to Matplotlib's `pcolormesh` to customise the plot. For example, can be
                 used to set the colormap of the plot using e.g.
                 `body.plot_map(..., projection='orthographic', cmap='Greys')`.
 
         Returns:
@@ -1285,15 +1287,16 @@
         # pylint: disable-next=no-member
         for k in set(_MapKwargs.__optional_keys__) | set(_MapKwargs.__required_keys__):
             if k in kwargs:
                 map_kwargs[k] = kwargs.pop(k)
 
         _, _, xx, yy, _, _ = self.generate_map_coordinates(**map_kwargs)
         h = ax.pcolormesh(xx, yy, map_img, **kwargs)
-        self.plot_map_wireframe(ax=ax, **(wireframe_kwargs or {}), **map_kwargs)
+        if add_wireframe:
+            self.plot_map_wireframe(ax=ax, **(wireframe_kwargs or {}), **map_kwargs)
         return h
 
     def imshow_map(self, *args, **kwargs):
         """
         Alias for `plot_map` for backwards compatibility.
 
         :meta private:
```

### Comparing `planetmapper-1.7.4/planetmapper/data/rings.json` & `planetmapper-1.7.5/planetmapper/data/rings.json`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.4/planetmapper/data_loader.py` & `planetmapper-1.7.5/planetmapper/data_loader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.4/planetmapper/gui.py` & `planetmapper-1.7.5/planetmapper/gui.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.4/planetmapper/kernel_downloader.py` & `planetmapper-1.7.5/planetmapper/kernel_downloader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.4/planetmapper/observation.py` & `planetmapper-1.7.5/planetmapper/observation.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.4/planetmapper/progress.py` & `planetmapper-1.7.5/planetmapper/progress.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.4/planetmapper/utils.py` & `planetmapper-1.7.5/planetmapper/utils.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.4/planetmapper.egg-info/PKG-INFO` & `planetmapper-1.7.5/planetmapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetmapper
-Version: 1.7.4
+Version: 1.7.5
 Summary: PlanetMapper: A Python module for visualising, navigating and mapping Solar System observations
 Home-page: https://github.com/ortk95/planetmapper
 Download-URL: https://pypi.org/project/planetmapper/
 Author: Oliver King
 Author-email: oliver.king95@gmail.com
 License: MIT
 Project-URL: Documentation, https://planetmapper.readthedocs.io/
```

### Comparing `planetmapper-1.7.4/planetmapper.egg-info/SOURCES.txt` & `planetmapper-1.7.5/planetmapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.4/pyproject.toml` & `planetmapper-1.7.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.4/setup.py` & `planetmapper-1.7.5/setup.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.4/tests/test_base.py` & `planetmapper-1.7.5/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.4/tests/test_basic_body.py` & `planetmapper-1.7.5/tests/test_basic_body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.4/tests/test_body.py` & `planetmapper-1.7.5/tests/test_body.py`

 * *Files 3% similar despite different names*

```diff
@@ -828,19 +828,36 @@
         self.assertEqual(self.body.get_poles_to_plot(), [(0, -90, 'S')])
 
         moon = Body('moon', utc='2000-01-08 03:00:00')
         self.assertEqual(moon.get_poles_to_plot(), [(0, 90, '(N)'), (0, -90, '(S)')])
 
     @patch('matplotlib.pyplot.show')
     def test_plot_wireframe(self, mock_show: MagicMock):
+        # TODO improve these tests by mocking the various matplotlib functions and
+        # checking that they are called with the correct arguments (also applies to
+        # other plotting tests elsewhere)
+
         fig, ax = plt.subplots()
         self.body.plot_wireframe_radec(ax, color='red')
+        self.assertEqual(len(ax.get_lines()), 21)
+        self.assertEqual(len(ax.get_images()), 0)
+        self.assertEqual(len(ax.get_children()), 32)
+        plt.close(fig)
+
+        fig, ax = plt.subplots()
+        self.body.plot_wireframe_radec(ax, label_poles=False)
+        self.assertEqual(len(ax.get_lines()), 21)
+        self.assertEqual(len(ax.get_images()), 0)
+        self.assertEqual(len(ax.get_children()), 31)
         plt.close(fig)
 
         ax = self.body.plot_wireframe_km()
+        self.assertEqual(len(ax.get_lines()), 21)
+        self.assertEqual(len(ax.get_images()), 0)
+        self.assertEqual(len(ax.get_children()), 32)
         plt.close(ax.figure)
 
         self.body.add_named_rings()
         self.body.coordinates_of_interest_lonlat.extend(
             [(0, 0), (90, 0), (180, 0), (270, 0)]
         )
         self.body.coordinates_of_interest_radec.append(
@@ -850,29 +867,35 @@
         fig, ax = plt.subplots()
         self.body.plot_wireframe_km(
             ax,
             label_poles=False,
             add_axis_labels=False,
             aspect_adjustable='box',
             add_title=False,
-            grid_interval=43,
+            grid_interval=45,
             indicate_equator=True,
             indicate_prime_meridian=True,
         )
+        self.assertEqual(len(ax.get_lines()), 21)
+        self.assertEqual(len(ax.get_images()), 0)
+        self.assertEqual(len(ax.get_children()), 36)
         plt.close(fig)
         self.body.ring_radii.clear()
         self.body.coordinates_of_interest_lonlat.clear()
         self.body.coordinates_of_interest_radec.clear()
         self.body.other_bodies_of_interest.clear()
 
         # Test hidden other bodies
         jupiter = planetmapper.Body('jupiter', utc='2005-01-01T04:00')
         jupiter.add_other_bodies_of_interest('thebe', 'metis', 'amalthea', 'adrastea')
         fig, ax = plt.subplots()
         jupiter.plot_wireframe_radec(ax)
+        self.assertEqual(len(ax.get_lines()), 21)
+        self.assertEqual(len(ax.get_images()), 0)
+        self.assertEqual(len(ax.get_children()), 40)
         plt.close(fig)
 
         # Test show
         fig, ax = plt.subplots()
         jupiter.plot_wireframe_radec(ax, show=True)
         plt.close(fig)
         mock_show.assert_called_once()
```

### Comparing `planetmapper-1.7.4/tests/test_body_xy.py` & `planetmapper-1.7.5/tests/test_body_xy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import unittest
 from unittest.mock import MagicMock, patch
 
 import common_testing
 import matplotlib.pyplot as plt
 import numpy as np
+from matplotlib.collections import QuadMesh
 from numpy import array, nan
 
 import planetmapper
 import planetmapper.base
 import planetmapper.progress
 from planetmapper import BodyXY
 from planetmapper.body_xy import Backplane, BackplaneNotFoundError
@@ -531,50 +532,67 @@
             )
         )
 
     @patch('matplotlib.pyplot.show')
     def test_plot_wireframe(self, mock_show: MagicMock):
         fig, ax = plt.subplots()
         self.body.plot_wireframe_xy(ax=ax)
+        self.assertEqual(len(ax.get_lines()), 21)
+        self.assertEqual(len(ax.get_images()), 0)
+        self.assertEqual(len(ax.get_children()), 32)
         plt.close(fig)
 
         fig, ax = plt.subplots()
         self.body.plot_wireframe_xy(ax=ax, show=True)
         plt.close(fig)
         mock_show.assert_called_once()
         mock_show.reset_mock()
 
         fig, ax = plt.subplots()
         self.body_zero_size.plot_wireframe_xy(ax=ax)
         plt.close(fig)
 
         ax = self.body.plot_map_wireframe()
         self.assertEqual(ax.get_xlim(), (360, 0))
+        self.assertEqual(len(ax.get_lines()), 16)
+        self.assertEqual(len(ax.get_images()), 0)
+        self.assertEqual(len(ax.get_children()), 26)
         plt.close('all')
 
         uranus = BodyXY('uranus', utc='2000-01-01', sz=5)  # Uranus is +ve E
         ax = uranus.plot_map_wireframe(ax=ax)
         self.assertEqual(ax.get_xlim(), (0, 360))
         plt.close('all')
 
         fig, ax = plt.subplots()
         self.body.plot_map_wireframe(ax=ax, projection='orthographic', lat=56)
+        self.assertEqual(len(ax.get_lines()), 18)
+        self.assertEqual(len(ax.get_images()), 0)
+        self.assertEqual(len(ax.get_children()), 29)
         plt.close(fig)
 
         fig, ax = plt.subplots()
-        self.body.plot_map_wireframe(ax=ax, projection='azimuthal', lat=-90)
+        self.body.plot_map_wireframe(
+            ax=ax, projection='azimuthal', lat=-90, label_poles=False, grid_interval=45
+        )
+        self.assertEqual(len(ax.get_lines()), 20)
+        self.assertEqual(len(ax.get_images()), 0)
+        self.assertEqual(len(ax.get_children()), 30)
         plt.close(fig)
 
         fig, ax = plt.subplots()
         self.body.plot_map_wireframe(
             ax=ax,
             projection='manual',
             lon_coords=np.linspace(-180, 180, 5),
             lat_coords=np.linspace(0, 90, 3),
         )
+        self.assertEqual(len(ax.get_lines()), 17)
+        self.assertEqual(len(ax.get_images()), 0)
+        self.assertEqual(len(ax.get_children()), 29)
         plt.close(fig)
 
     def test_get_wireframe_overlay(self):
         img = self.body.get_wireframe_overlay_img(output_size=100)
         self.assertEqual(max(img.shape), 100)
         self.assertEqual(len(img.shape), 2)
 
@@ -884,34 +902,55 @@
         )
         self.body.set_img_size(15, 10)
 
     @patch('matplotlib.pyplot.show')
     def test_plot_backplane(self, mock_show: MagicMock):
         fig, ax = plt.subplots()
         self.body.plot_backplane_img(' emission ', ax=ax)
+        self.assertEqual(len(ax.get_lines()), 21)
+        self.assertEqual(len(ax.get_images()), 1)
+        self.assertEqual(len(ax.get_children()), 33)
         plt.close(fig)
 
         fig, ax = plt.subplots()
         self.body.plot_backplane_img(' EmissioN ', ax=ax, show=True)
         plt.close(fig)
         mock_show.assert_called_once()
         mock_show.reset_mock()
 
         fig, ax = plt.subplots()
         self.body.plot_backplane_map(' emission ', ax=ax, show=True)
         plt.close(fig)
         mock_show.assert_called_once()
         mock_show.reset_mock()
 
-        self.body.plot_backplane_map(' emission ', degree_interval=90)
+        ax = self.body.plot_backplane_map(' emission ', degree_interval=90)
+        self.assertEqual(len(ax.get_lines()), 16)
+        self.assertEqual(len(ax.get_images()), 0)
+        self.assertEqual(len(ax.get_children()), 27)
         plt.close('all')
 
     def test_plot_map(self):
         fig, ax = plt.subplots()
-        self.body.plot_map(np.ones((180, 360)), ax=ax)
+        h = self.body.plot_map(np.ones((180, 360)), ax=ax)
+        self.assertIsInstance(h, QuadMesh)
+        children = ax.get_children()
+        self.assertIn(h, ax.get_children())
+        self.assertEqual(len(ax.get_lines()), 16)
+        self.assertEqual(len(ax.get_images()), 0)
+        self.assertEqual(len(ax.get_children()), 27)
+        plt.close(fig)
+
+        fig, ax = plt.subplots()
+        h = self.body.plot_map(np.ones((180, 360)), ax=ax, add_wireframe=False)
+        children = ax.get_children()
+        self.assertIn(h, ax.get_children())
+        self.assertEqual(len(ax.get_lines()), 0)
+        self.assertEqual(len(ax.get_images()), 0)
+        self.assertEqual(len(ax.get_children()), 11)
         plt.close(fig)
 
         self.body.imshow_map(np.ones((180, 360)))
         plt.close('all')
 
     def test_matplotlib_transforms(self):
         self.body.set_disc_params(2, 1, 3.5, 45.678)
```

### Comparing `planetmapper-1.7.4/tests/test_common.py` & `planetmapper-1.7.5/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.4/tests/test_data_loader.py` & `planetmapper-1.7.5/tests/test_data_loader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.4/tests/test_init.py` & `planetmapper-1.7.5/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.4/tests/test_kernel_downloader.py` & `planetmapper-1.7.5/tests/test_kernel_downloader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.4/tests/test_observation.py` & `planetmapper-1.7.5/tests/test_observation.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.4/tests/test_progress.py` & `planetmapper-1.7.5/tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.4/tests/test_utils.py` & `planetmapper-1.7.5/tests/test_utils.py`

 * *Files identical despite different names*

