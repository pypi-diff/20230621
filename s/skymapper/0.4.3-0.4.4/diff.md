# Comparing `tmp/skymapper-0.4.3.tar.gz` & `tmp/skymapper-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skymapper-0.4.3.tar", last modified: Thu Nov 10 16:43:18 2022, max compression
+gzip compressed data, was "skymapper-0.4.4.tar", last modified: Wed Jun 21 18:44:08 2023, max compression
```

## Comparing `skymapper-0.4.3.tar` & `skymapper-0.4.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2022-11-10 16:43:18.644539 skymapper-0.4.3/
--rw-r--r--   0 pmelchior   (501) staff       (20)     1071 2018-09-13 22:02:16.000000 skymapper-0.4.3/LICENSE.md
--rw-r--r--   0 pmelchior   (501) staff       (20)     8723 2022-11-10 16:43:18.644375 skymapper-0.4.3/PKG-INFO
--rw-r--r--   0 pmelchior   (501) staff       (20)     7964 2020-03-18 16:33:44.000000 skymapper-0.4.3/README.md
--rw-r--r--   0 pmelchior   (501) staff       (20)     2599 2018-02-08 20:25:16.000000 skymapper-0.4.3/aea_vs_lc_south_pole.py
--rw-r--r--   0 pmelchior   (501) staff       (20)    18190 2016-03-11 04:44:18.000000 skymapper-0.4.3/custom_projection_example.py
--rw-r--r--   0 pmelchior   (501) staff       (20)     2168 2016-03-14 19:10:36.000000 skymapper-0.4.3/example.py
--rw-r--r--   0 pmelchior   (501) staff       (20)     1625 2016-04-13 05:06:14.000000 skymapper-0.4.3/example2.py
--rw-r--r--   0 pmelchior   (501) staff       (20)     2795 2016-03-19 20:40:32.000000 skymapper-0.4.3/example3.py
--rw-r--r--   0 pmelchior   (501) staff       (20)       38 2022-11-10 16:43:18.644580 skymapper-0.4.3/setup.cfg
--rw-r--r--   0 pmelchior   (501) staff       (20)     1057 2022-11-10 16:42:50.000000 skymapper-0.4.3/setup.py
-drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2022-11-10 16:43:18.642281 skymapper-0.4.3/skymapper/
--rw-r--r--   0 pmelchior   (501) staff       (20)     1334 2019-08-01 21:33:10.000000 skymapper-0.4.3/skymapper/__init__.py
--rw-r--r--   0 pmelchior   (501) staff       (20)     4356 2020-03-26 03:40:46.000000 skymapper-0.4.3/skymapper/healpix.py
--rw-r--r--   0 pmelchior   (501) staff       (20)    51117 2022-11-10 16:40:13.000000 skymapper-0.4.3/skymapper/map.py
--rw-r--r--   0 pmelchior   (501) staff       (20)    36292 2019-08-09 21:14:23.000000 skymapper-0.4.3/skymapper/projection.py
-drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2022-11-10 16:43:18.644124 skymapper-0.4.3/skymapper/survey/
--rw-r--r--   0 pmelchior   (501) staff       (20)     1598 2019-08-01 21:33:10.000000 skymapper-0.4.3/skymapper/survey/__init__.py
--rw-r--r--   0 pmelchior   (501) staff       (20)    11571 2019-08-01 21:33:10.000000 skymapper-0.4.3/skymapper/survey/boss_survey.ply
--rw-r--r--   0 pmelchior   (501) staff       (20)    36480 2019-08-01 21:33:10.000000 skymapper-0.4.3/skymapper/survey/des-round17-poly_tidy.ply
-drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2022-11-10 16:43:18.643469 skymapper-0.4.3/skymapper.egg-info/
--rw-r--r--   0 pmelchior   (501) staff       (20)     8723 2022-11-10 16:43:18.000000 skymapper-0.4.3/skymapper.egg-info/PKG-INFO
--rw-r--r--   0 pmelchior   (501) staff       (20)      470 2022-11-10 16:43:18.000000 skymapper-0.4.3/skymapper.egg-info/SOURCES.txt
--rw-r--r--   0 pmelchior   (501) staff       (20)        1 2022-11-10 16:43:18.000000 skymapper-0.4.3/skymapper.egg-info/dependency_links.txt
--rw-r--r--   0 pmelchior   (501) staff       (20)       30 2022-11-10 16:43:18.000000 skymapper-0.4.3/skymapper.egg-info/requires.txt
--rw-r--r--   0 pmelchior   (501) staff       (20)       10 2022-11-10 16:43:18.000000 skymapper-0.4.3/skymapper.egg-info/top_level.txt
+drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2023-06-21 18:44:08.034407 skymapper-0.4.4/
+-rw-r--r--   0 pmelchior   (501) staff       (20)     1071 2018-09-13 22:02:16.000000 skymapper-0.4.4/LICENSE.md
+-rw-r--r--   0 pmelchior   (501) staff       (20)     8723 2023-06-21 18:44:08.034166 skymapper-0.4.4/PKG-INFO
+-rw-r--r--   0 pmelchior   (501) staff       (20)     7984 2023-06-21 18:42:38.000000 skymapper-0.4.4/README.md
+-rw-r--r--   0 pmelchior   (501) staff       (20)     2599 2018-02-08 20:25:16.000000 skymapper-0.4.4/aea_vs_lc_south_pole.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)    18190 2016-03-11 04:44:18.000000 skymapper-0.4.4/custom_projection_example.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)     2168 2016-03-14 19:10:36.000000 skymapper-0.4.4/example.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)     1625 2016-04-13 05:06:14.000000 skymapper-0.4.4/example2.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)     2795 2016-03-19 20:40:32.000000 skymapper-0.4.4/example3.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)       38 2023-06-21 18:44:08.034460 skymapper-0.4.4/setup.cfg
+-rw-r--r--   0 pmelchior   (501) staff       (20)     1057 2023-06-21 18:42:38.000000 skymapper-0.4.4/setup.py
+drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2023-06-21 18:44:08.032006 skymapper-0.4.4/skymapper/
+-rw-r--r--   0 pmelchior   (501) staff       (20)     1334 2019-08-01 21:33:10.000000 skymapper-0.4.4/skymapper/__init__.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)     4356 2020-03-26 03:40:46.000000 skymapper-0.4.4/skymapper/healpix.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)    51939 2023-06-21 18:42:31.000000 skymapper-0.4.4/skymapper/map.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)    36292 2019-08-09 21:14:23.000000 skymapper-0.4.4/skymapper/projection.py
+drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2023-06-21 18:44:08.033825 skymapper-0.4.4/skymapper/survey/
+-rw-r--r--   0 pmelchior   (501) staff       (20)     1598 2019-08-01 21:33:10.000000 skymapper-0.4.4/skymapper/survey/__init__.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)    11571 2019-08-01 21:33:10.000000 skymapper-0.4.4/skymapper/survey/boss_survey.ply
+-rw-r--r--   0 pmelchior   (501) staff       (20)    36480 2019-08-01 21:33:10.000000 skymapper-0.4.4/skymapper/survey/des-round17-poly_tidy.ply
+drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2023-06-21 18:44:08.033195 skymapper-0.4.4/skymapper.egg-info/
+-rw-r--r--   0 pmelchior   (501) staff       (20)     8723 2023-06-21 18:44:07.000000 skymapper-0.4.4/skymapper.egg-info/PKG-INFO
+-rw-r--r--   0 pmelchior   (501) staff       (20)      470 2023-06-21 18:44:07.000000 skymapper-0.4.4/skymapper.egg-info/SOURCES.txt
+-rw-r--r--   0 pmelchior   (501) staff       (20)        1 2023-06-21 18:44:07.000000 skymapper-0.4.4/skymapper.egg-info/dependency_links.txt
+-rw-r--r--   0 pmelchior   (501) staff       (20)       30 2023-06-21 18:44:07.000000 skymapper-0.4.4/skymapper.egg-info/requires.txt
+-rw-r--r--   0 pmelchior   (501) staff       (20)       10 2023-06-21 18:44:07.000000 skymapper-0.4.4/skymapper.egg-info/top_level.txt
```

### Comparing `skymapper-0.4.3/LICENSE.md` & `skymapper-0.4.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `skymapper-0.4.3/PKG-INFO` & `skymapper-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: skymapper
-Version: 0.4.3
+Version: 0.4.4
 Summary: Mapping astronomical survey data on the sky, handsomely
 Home-page: https://github.com/pmelchior/skymapper
 Author: Peter Melchior
 Author-email: peter.m.melchior@gmail.com
 License: MIT
 Keywords: visualization,map projection,matplotlib
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -63,15 +62,15 @@
 # add scatter plot
 map.scatter(ra_scatter, dec_scatter, s=size_scatter, edgecolor='k', facecolor='None')
 
 # focus on relevant region
 map.focus(ra, dec)
 ```
 
-![Random density in DES footprint](https://github.com/pmelchior/skymapper/raw/master/examples/example1.png)
+![Random density in DES footprint](https://github.com/pmelchior/skymapper/assets/1463403/fa1528f4-2ed0-4945-a342-17bddd64d73d)
 
 The `map` instance has several members, most notably
 
 *  `fig`: the `matplotlib.Figure` that holds the map
 * `ax`: the `matplotlib.Axes` that holds the map
 
 The syntax mimics `matplotlib` as closely as possible. Currently supported are canonical plotting functions
@@ -156,8 +155,7 @@
 If this looks like the [`pymangle`](https://github.com/esheldon/pymangle) interface: it should. That means that you can avoid the overhead of having to define a survey and e.g. pass a `pymangle.Mangle` object directly to `footprint()`.
 
 ### Limitation(s)
 
 The combination of `Map` and `Projection` is *not* a [matplotlib transformation](http://matplotlib.org/users/transforms_tutorial.html). Among several reasons, it is very difficult (maybe impossible) to work with the `matplotlib.Axes` that are not rectangles or ellipses. So, we decided to split the problem: making use of matplotlib for lower-level graphics primitive and layering the map-making on top of it. This way, we can control e.g. the interpolation method on the sphere or the location of the tick labels in a way consistent with visual expectations from hundreds of years of cartography. While `skymapper` tries to follow matplotlib conventions very closely, some methods may not work as expected. Open an issue if you think you found such a case.
 
 In particular, we'd appreciate help to make sure that the interactive features work well on all matplotlib backends.
-
```

### Comparing `skymapper-0.4.3/README.md` & `skymapper-0.4.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 # add scatter plot
 map.scatter(ra_scatter, dec_scatter, s=size_scatter, edgecolor='k', facecolor='None')
 
 # focus on relevant region
 map.focus(ra, dec)
 ```
 
-![Random density in DES footprint](https://github.com/pmelchior/skymapper/raw/master/examples/example1.png)
+![Random density in DES footprint](https://github.com/pmelchior/skymapper/assets/1463403/fa1528f4-2ed0-4945-a342-17bddd64d73d)
 
 The `map` instance has several members, most notably
 
 *  `fig`: the `matplotlib.Figure` that holds the map
 * `ax`: the `matplotlib.Axes` that holds the map
 
 The syntax mimics `matplotlib` as closely as possible. Currently supported are canonical plotting functions
@@ -134,8 +134,8 @@
 
 If this looks like the [`pymangle`](https://github.com/esheldon/pymangle) interface: it should. That means that you can avoid the overhead of having to define a survey and e.g. pass a `pymangle.Mangle` object directly to `footprint()`.
 
 ### Limitation(s)
 
 The combination of `Map` and `Projection` is *not* a [matplotlib transformation](http://matplotlib.org/users/transforms_tutorial.html). Among several reasons, it is very difficult (maybe impossible) to work with the `matplotlib.Axes` that are not rectangles or ellipses. So, we decided to split the problem: making use of matplotlib for lower-level graphics primitive and layering the map-making on top of it. This way, we can control e.g. the interpolation method on the sphere or the location of the tick labels in a way consistent with visual expectations from hundreds of years of cartography. While `skymapper` tries to follow matplotlib conventions very closely, some methods may not work as expected. Open an issue if you think you found such a case.
 
-In particular, we'd appreciate help to make sure that the interactive features work well on all matplotlib backends.
+In particular, we'd appreciate help to make sure that the interactive features work well on all matplotlib backends.
```

### Comparing `skymapper-0.4.3/aea_vs_lc_south_pole.py` & `skymapper-0.4.4/aea_vs_lc_south_pole.py`

 * *Files identical despite different names*

### Comparing `skymapper-0.4.3/custom_projection_example.py` & `skymapper-0.4.4/custom_projection_example.py`

 * *Files identical despite different names*

### Comparing `skymapper-0.4.3/example.py` & `skymapper-0.4.4/example.py`

 * *Files identical despite different names*

### Comparing `skymapper-0.4.3/example2.py` & `skymapper-0.4.4/example2.py`

 * *Files identical despite different names*

### Comparing `skymapper-0.4.3/example3.py` & `skymapper-0.4.4/example3.py`

 * *Files identical despite different names*

### Comparing `skymapper-0.4.3/setup.py` & `skymapper-0.4.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 long_description = open('README.md').read()
 
 setup(
     name="skymapper",
     description="Mapping astronomical survey data on the sky, handsomely",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version="0.4.3",
+    version="0.4.4",
     license="MIT",
     author="Peter Melchior",
     author_email="peter.m.melchior@gmail.com",
     url="https://github.com/pmelchior/skymapper",
     packages=["skymapper", "skymapper.survey"],
     package_data={"skymapper.survey": ['*.ply']},
     classifiers=[
```

### Comparing `skymapper-0.4.3/skymapper/__init__.py` & `skymapper-0.4.4/skymapper/__init__.py`

 * *Files identical despite different names*

### Comparing `skymapper-0.4.3/skymapper/healpix.py` & `skymapper-0.4.4/skymapper/healpix.py`

 * *Files identical despite different names*

### Comparing `skymapper-0.4.3/skymapper/map.py` & `skymapper-0.4.4/skymapper/map.py`

 * *Files 1% similar despite different names*

```diff
@@ -469,37 +469,47 @@
         if loc == "top":
             return "bottom"
         if loc == "left":
             return "right"
         if loc == "right":
             return "left"
 
-    def labelMeridiansAtParallel(self, p, loc=None, meridians=None, pad=None, direction='parallel', fmt=None, **kwargs):
+    def labelMeridiansAtParallel(self, p, loc=None, meridians=None, pad=None, direction='parallel', fmt=None, 
+                                 clear_existing_labels=False, **kwargs):
         """Label the meridians intersecting a given parallel
 
         The method is called by `grid()` but can be used to overwrite the defaults.
 
         Args:
             p: parallel in deg
             loc: location of the label with respect to `p`, from `['top', 'bottom']`
             meridians: list of meridians to label, if None labels all of them
             pad: padding of annotation, in units of fontsize
             direction: tangent of the label, from `['parallel', 'meridian']`
             fmt: formatter for labels, if `None` use default
+            clear_existing_labels : bool (default=False)
             **kwargs: styling of `matplotlib` annotations for the graticule labels
         """
         arguments = _parseArgs(locals())
 
         if p in self.proj.poleIsPoint.keys() and self.proj.poleIsPoint[p]:
             return
 
         myname = 'labelMeridiansAtParallel'
         if myname not in self._config.keys():
             self._config[myname] = dict()
 
+        # remove all existing labels:
+        if clear_existing_labels:
+            for _p in self._config[myname].keys():
+                gid = 'meridian-label-%r' % _p 
+                artists = self.artists(gid)
+                for artist in artists:
+                    artist.remove() 
+
         # remove exisiting labels at p
         gid = 'meridian-label-%r' % p
         if p in self._config[myname].keys():
             artists = self.artists(gid)
             for artist in artists:
                 artist.remove()
 
@@ -551,34 +561,44 @@
                 dxy_ = self.proj.gradient(m, p, direction=direction)
                 angle = rot_base - np.arctan2(*dxy_) / DEG2RAD
             else:
                 angle = rotation
 
             self.ax.annotate(fmt(m), (xp, yp), xytext=dxy, textcoords='offset points', rotation=angle, rotation_mode='anchor', horizontalalignment=horizontalalignment, verticalalignment=verticalalignment, size=size, color=color, alpha=alpha, zorder=zorder, gid=gid, in_layout=False, **kwargs)
 
-    def labelParallelsAtMeridian(self, m, loc=None, parallels=None, pad=None, direction='parallel', fmt=None, **kwargs):
+    def labelParallelsAtMeridian(self, m, loc=None, parallels=None, pad=None, direction='parallel', fmt=None, 
+                                 clear_existing_labels=False, **kwargs):
         """Label the parallel intersecting a given meridian
 
         The method is called by `grid()` but can be used to overwrite the defaults.
 
         Args:
             m: meridian in deg
             loc: location of the label with respect to `m`, from `['left', 'right']`
             parallel: list of parallels to label, if None labels all of them
             pad: padding of annotation, in units of fontsize
             direction: tangent of the label, from `['parallel', 'meridian']`
             fmt: formatter for label, if `None` use default
+            clear_existing_labels : bool (default=False)
             **kwargs: styling of `matplotlib` annotations for the graticule labels
         """
         arguments = _parseArgs(locals())
 
         myname = 'labelParallelsAtMeridian'
         if myname not in self._config.keys():
             self._config[myname] = dict()
 
+        # remove all existing labels
+        if clear_existing_labels:
+            for _m in self._config[myname].keys():
+                gid = 'parallel-label-%r' % _m
+                artists = self.artists(gid)
+                for artist in artists:
+                    artist.remove() 
+
         # remove exisiting labels at m
         gid = 'parallel-label-%r' % m
         if m in self._config[myname].keys():
             artists = self.artists(gid)
             for artist in artists:
                 artist.remove()
```

### Comparing `skymapper-0.4.3/skymapper/projection.py` & `skymapper-0.4.4/skymapper/projection.py`

 * *Files identical despite different names*

### Comparing `skymapper-0.4.3/skymapper/survey/__init__.py` & `skymapper-0.4.4/skymapper/survey/__init__.py`

 * *Files identical despite different names*

### Comparing `skymapper-0.4.3/skymapper/survey/boss_survey.ply` & `skymapper-0.4.4/skymapper/survey/boss_survey.ply`

 * *Files identical despite different names*

### Comparing `skymapper-0.4.3/skymapper/survey/des-round17-poly_tidy.ply` & `skymapper-0.4.4/skymapper/survey/des-round17-poly_tidy.ply`

 * *Files identical despite different names*

### Comparing `skymapper-0.4.3/skymapper.egg-info/PKG-INFO` & `skymapper-0.4.4/skymapper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: skymapper
-Version: 0.4.3
+Version: 0.4.4
 Summary: Mapping astronomical survey data on the sky, handsomely
 Home-page: https://github.com/pmelchior/skymapper
 Author: Peter Melchior
 Author-email: peter.m.melchior@gmail.com
 License: MIT
 Keywords: visualization,map projection,matplotlib
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -63,15 +62,15 @@
 # add scatter plot
 map.scatter(ra_scatter, dec_scatter, s=size_scatter, edgecolor='k', facecolor='None')
 
 # focus on relevant region
 map.focus(ra, dec)
 ```
 
-![Random density in DES footprint](https://github.com/pmelchior/skymapper/raw/master/examples/example1.png)
+![Random density in DES footprint](https://github.com/pmelchior/skymapper/assets/1463403/fa1528f4-2ed0-4945-a342-17bddd64d73d)
 
 The `map` instance has several members, most notably
 
 *  `fig`: the `matplotlib.Figure` that holds the map
 * `ax`: the `matplotlib.Axes` that holds the map
 
 The syntax mimics `matplotlib` as closely as possible. Currently supported are canonical plotting functions
@@ -156,8 +155,7 @@
 If this looks like the [`pymangle`](https://github.com/esheldon/pymangle) interface: it should. That means that you can avoid the overhead of having to define a survey and e.g. pass a `pymangle.Mangle` object directly to `footprint()`.
 
 ### Limitation(s)
 
 The combination of `Map` and `Projection` is *not* a [matplotlib transformation](http://matplotlib.org/users/transforms_tutorial.html). Among several reasons, it is very difficult (maybe impossible) to work with the `matplotlib.Axes` that are not rectangles or ellipses. So, we decided to split the problem: making use of matplotlib for lower-level graphics primitive and layering the map-making on top of it. This way, we can control e.g. the interpolation method on the sphere or the location of the tick labels in a way consistent with visual expectations from hundreds of years of cartography. While `skymapper` tries to follow matplotlib conventions very closely, some methods may not work as expected. Open an issue if you think you found such a case.
 
 In particular, we'd appreciate help to make sure that the interactive features work well on all matplotlib backends.
-
```

