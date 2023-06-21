# Comparing `tmp/airfrans-0.1.5.tar.gz` & `tmp/airfrans-0.1.5.1.tar.gz`

## Comparing `airfrans-0.1.5.tar` & `airfrans-0.1.5.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 airfrans-0.1.5/.readthedocs.yaml
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 airfrans-0.1.5/airfrans.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/Makefile
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/make.bat
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/requirements.txt
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/source/conf.py
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/source/index.rst
--rw-r--r--   0        0        0   119172 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/source/_figures/boundary_layer.png
--rw-r--r--   0        0        0  2300738 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/source/_figures/fields.png
--rw-r--r--   0        0        0  2317524 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/source/_figures/sampling.png
--rw-r--r--   0        0        0    71716 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/source/_figures/surface.png
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/source/modules/dataset.rst
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/source/modules/naca.rst
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/source/modules/root.rst
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/source/modules/sampling.rst
--rw-r--r--   0        0        0     5962 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/source/notes/dataset.rst
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/source/notes/installation.rst
--rw-r--r--   0        0        0     5041 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/source/notes/introduction.rst
--rw-r--r--   0        0        0     9590 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/source/notes/simulation.rst
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/source/notes/visualization.rst
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 airfrans-0.1.5/src/airfrans/__init__.py
--rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 airfrans-0.1.5/src/airfrans/dataset.py
--rw-r--r--   0        0        0     5175 2020-02-02 00:00:00.000000 airfrans-0.1.5/src/airfrans/naca_generator.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 airfrans-0.1.5/src/airfrans/reorganize.py
--rw-r--r--   0        0        0     4054 2020-02-02 00:00:00.000000 airfrans-0.1.5/src/airfrans/sampling.py
--rw-r--r--   0        0        0    23110 2020-02-02 00:00:00.000000 airfrans-0.1.5/src/airfrans/simulation.py
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 airfrans-0.1.5/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 airfrans-0.1.5/LICENSE
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 airfrans-0.1.5/README.md
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 airfrans-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     4736 2020-02-02 00:00:00.000000 airfrans-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 airfrans-0.1.5.1/.readthedocs.yaml
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 airfrans-0.1.5.1/airfrans.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 airfrans-0.1.5.1/docs/Makefile
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 airfrans-0.1.5.1/docs/make.bat
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 airfrans-0.1.5.1/docs/requirements.txt
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 airfrans-0.1.5.1/docs/source/conf.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 airfrans-0.1.5.1/docs/source/index.rst
+-rw-r--r--   0        0        0   119172 2020-02-02 00:00:00.000000 airfrans-0.1.5.1/docs/source/_figures/boundary_layer.png
+-rw-r--r--   0        0        0  2300738 2020-02-02 00:00:00.000000 airfrans-0.1.5.1/docs/source/_figures/fields.png
+-rw-r--r--   0        0        0  2317524 2020-02-02 00:00:00.000000 airfrans-0.1.5.1/docs/source/_figures/sampling.png
+-rw-r--r--   0        0        0    71716 2020-02-02 00:00:00.000000 airfrans-0.1.5.1/docs/source/_figures/surface.png
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 airfrans-0.1.5.1/docs/source/modules/dataset.rst
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 airfrans-0.1.5.1/docs/source/modules/naca.rst
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 airfrans-0.1.5.1/docs/source/modules/root.rst
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 airfrans-0.1.5.1/docs/source/modules/sampling.rst
+-rw-r--r--   0        0        0     5962 2020-02-02 00:00:00.000000 airfrans-0.1.5.1/docs/source/notes/dataset.rst
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 airfrans-0.1.5.1/docs/source/notes/installation.rst
+-rw-r--r--   0        0        0     5041 2020-02-02 00:00:00.000000 airfrans-0.1.5.1/docs/source/notes/introduction.rst
+-rw-r--r--   0        0        0     9590 2020-02-02 00:00:00.000000 airfrans-0.1.5.1/docs/source/notes/simulation.rst
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 airfrans-0.1.5.1/docs/source/notes/visualization.rst
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 airfrans-0.1.5.1/src/airfrans/__init__.py
+-rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 airfrans-0.1.5.1/src/airfrans/dataset.py
+-rw-r--r--   0        0        0     5175 2020-02-02 00:00:00.000000 airfrans-0.1.5.1/src/airfrans/naca_generator.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 airfrans-0.1.5.1/src/airfrans/reorganize.py
+-rw-r--r--   0        0        0     4054 2020-02-02 00:00:00.000000 airfrans-0.1.5.1/src/airfrans/sampling.py
+-rw-r--r--   0        0        0    24286 2020-02-02 00:00:00.000000 airfrans-0.1.5.1/src/airfrans/simulation.py
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 airfrans-0.1.5.1/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 airfrans-0.1.5.1/LICENSE
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 airfrans-0.1.5.1/README.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 airfrans-0.1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 airfrans-0.1.5.1/PKG-INFO
```

### Comparing `airfrans-0.1.5/.readthedocs.yaml` & `airfrans-0.1.5.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.5/docs/Makefile` & `airfrans-0.1.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.5/docs/make.bat` & `airfrans-0.1.5.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.5/docs/source/conf.py` & `airfrans-0.1.5.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.5/docs/source/index.rst` & `airfrans-0.1.5.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.5/docs/source/_figures/boundary_layer.png` & `airfrans-0.1.5.1/docs/source/_figures/boundary_layer.png`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.5/docs/source/_figures/fields.png` & `airfrans-0.1.5.1/docs/source/_figures/fields.png`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.5/docs/source/_figures/sampling.png` & `airfrans-0.1.5.1/docs/source/_figures/sampling.png`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.5/docs/source/_figures/surface.png` & `airfrans-0.1.5.1/docs/source/_figures/surface.png`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.5/docs/source/notes/dataset.rst` & `airfrans-0.1.5.1/docs/source/notes/dataset.rst`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.5/docs/source/notes/introduction.rst` & `airfrans-0.1.5.1/docs/source/notes/introduction.rst`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.5/docs/source/notes/simulation.rst` & `airfrans-0.1.5.1/docs/source/notes/simulation.rst`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.5/docs/source/notes/visualization.rst` & `airfrans-0.1.5.1/docs/source/notes/visualization.rst`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.5/src/airfrans/dataset.py` & `airfrans-0.1.5.1/src/airfrans/dataset.py`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.5/src/airfrans/naca_generator.py` & `airfrans-0.1.5.1/src/airfrans/naca_generator.py`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.5/src/airfrans/reorganize.py` & `airfrans-0.1.5.1/src/airfrans/reorganize.py`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.5/src/airfrans/sampling.py` & `airfrans-0.1.5.1/src/airfrans/sampling.py`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.5/src/airfrans/simulation.py` & `airfrans-0.1.5.1/src/airfrans/simulation.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,17 @@
         # Targets
         self.velocity = np.array(self.internal.point_data['U'][:, :2]).astype('float64')
         self.pressure = np.array(self.internal.point_data['p'][:, None]).astype('float64')
         self.nu_t = np.array(self.internal.point_data['nut'][:, None]).astype('float64')
 
     def sampling_volume(self, seed, n, density = 'uniform', targets = True):
         """
-        Sample points in the internal mesh following the given density.
+        Sample points in the internal mesh following the given density. The outputs is a ndarray of shape (n, 2 + 1) or (n, 2 + 1 + 4)
+        if targets is ``True``. The two first columns are the position of the sampled points, followed by the distance to the airfoil
+        and the targets (in the order x-velocity, y-velocity, pressure, and turbulent viscosity) if called.
 
         Args:
             seed (int): Seed for the random number generator.
             n (int): Number of sampled points.
             density (str, optional): Density from which the sampling is done. Choose between ``'uniform'`` and ``'mesh_density'``. Default: ``'uniform'``
             targets (bool, optional): If ``True``, velocity, pressure and kinematic turbulent viscosity will be returned in the output ndarray. Default: ``True``
         """
@@ -94,15 +96,17 @@
 
         seed_sampling = rng.integers(10000)         
 
         return sampling.cell_sampling_2d(seed_sampling, cell_points, cell_attr)
     
     def sampling_surface(self, seed, n, density = 'uniform', targets = True):
         """
-        Sample points in the airfoil mesh following the given density.
+        Sample points in the airfoil mesh following the given density. The outputs is a ndarray of shape (n, 2 + 2) or (n, 2 + 2 + 4)
+        if targets is ``True``. The two first columns are the position of the sampled points, followed by the x and y components of
+        the inward-pointing normals and the targets (in the order x-velocity, y-velocity, pressure, and turbulent viscosity) if called.
 
         Args:
             seed (int): Seed for the random number generator.
             n (int): Number of sampled points.
             density (str, optional): Density from which the sampling is done. Choose between ``'uniform'`` and ``'mesh_density'``. Default: ``'uniform'``
             targets (bool, optional): If ``True``, velocity, pressure and kinematic turbulent viscosity will be returned in the output ndarray. Default: ``True``
         """
@@ -131,15 +135,19 @@
 
         seed_sampling = rng.integers(10000)
 
         return sampling.cell_sampling_1d(seed_sampling, line_points, line_attr)
 
     def sampling_mesh(self, seed, n, targets = True):
         """
-        Sample points over the simulation mesh without replacement.
+        Sample points over the simulation mesh without replacement. The outputs is a ndarray of shape (n, 2 + 6) or (n, 2 + 6 + 4)
+        if targets is ``True``. The two first columns are the position of the sampled points, followed by a boolean set to ``True``
+        if the sample points belongs to the surface, the distance to the airfoil, the x and y components of the normals (set to 0
+        if the sample points does not belong to the surface), the x and y components of the input velocity and the targets (in the
+        order x-velocity, y-velocity, pressure, and turbulent viscosity) if called.
 
         Args:
             seed (int): Seed for the random number generator.
             n (int): Number of sampled points, this number has to be lower than the total number of points in the mesh.
             targets (bool, optional): If ``True``, velocity, pressure and kinematic turbulent viscosity will be returned in the output ndarray. Default: ``True``
         """
         rng = np.random.default_rng(seed = seed)
```

### Comparing `airfrans-0.1.5/.gitignore` & `airfrans-0.1.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.5/LICENSE` & `airfrans-0.1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.5/README.md` & `airfrans-0.1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.5/pyproject.toml` & `airfrans-0.1.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "airfrans"
-version = "0.1.5"
+version = "0.1.5.1"
 authors = [
   { name="Florent Bonnet", email="bonnet@isir.upmc.fr" },
 ]
 description = "A package to facilitate the manipulation of the AirfRANS dataset simulations."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `airfrans-0.1.5/PKG-INFO` & `airfrans-0.1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airfrans
-Version: 0.1.5
+Version: 0.1.5.1
 Summary: A package to facilitate the manipulation of the AirfRANS dataset simulations.
 Project-URL: Homepage, https://github.com/Extrality/airfrans_lib
 Project-URL: Bug Tracker, https://github.com/Extrality/airfrans_lib/issues
 Author-email: Florent Bonnet <bonnet@isir.upmc.fr>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

