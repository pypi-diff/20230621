# Comparing `tmp/airfrans-0.1.4.tar.gz` & `tmp/airfrans-0.1.5.tar.gz`

## Comparing `airfrans-0.1.4.tar` & `airfrans-0.1.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 airfrans-0.1.4/.readthedocs.yaml
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 airfrans-0.1.4/airfrans.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/Makefile
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/make.bat
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/requirements.txt
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/source/conf.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/source/index.rst
--rw-r--r--   0        0        0   119172 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/source/_figures/boundary_layer.png
--rw-r--r--   0        0        0  2300738 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/source/_figures/fields.png
--rw-r--r--   0        0        0  2317524 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/source/_figures/sampling.png
--rw-r--r--   0        0        0    71716 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/source/_figures/surface.png
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/source/modules/dataset.rst
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/source/modules/naca.rst
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/source/modules/root.rst
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/source/modules/sampling.rst
--rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/source/notes/dataset.rst
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/source/notes/installation.rst
--rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/source/notes/introduction.rst
--rw-r--r--   0        0        0     9547 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/source/notes/simulation.rst
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 airfrans-0.1.4/docs/source/notes/visualization.rst
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 airfrans-0.1.4/src/airfrans/__init__.py
--rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 airfrans-0.1.4/src/airfrans/dataset.py
--rw-r--r--   0        0        0     5175 2020-02-02 00:00:00.000000 airfrans-0.1.4/src/airfrans/naca_generator.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 airfrans-0.1.4/src/airfrans/reorganize.py
--rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 airfrans-0.1.4/src/airfrans/sampling.py
--rw-r--r--   0        0        0    22518 2020-02-02 00:00:00.000000 airfrans-0.1.4/src/airfrans/simulation.py
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 airfrans-0.1.4/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 airfrans-0.1.4/LICENSE
--rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 airfrans-0.1.4/README.md
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 airfrans-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 airfrans-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 airfrans-0.1.5/.readthedocs.yaml
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 airfrans-0.1.5/airfrans.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/Makefile
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/make.bat
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/requirements.txt
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/source/conf.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/source/index.rst
+-rw-r--r--   0        0        0   119172 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/source/_figures/boundary_layer.png
+-rw-r--r--   0        0        0  2300738 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/source/_figures/fields.png
+-rw-r--r--   0        0        0  2317524 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/source/_figures/sampling.png
+-rw-r--r--   0        0        0    71716 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/source/_figures/surface.png
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/source/modules/dataset.rst
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/source/modules/naca.rst
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/source/modules/root.rst
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/source/modules/sampling.rst
+-rw-r--r--   0        0        0     5962 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/source/notes/dataset.rst
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/source/notes/installation.rst
+-rw-r--r--   0        0        0     5041 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/source/notes/introduction.rst
+-rw-r--r--   0        0        0     9590 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/source/notes/simulation.rst
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 airfrans-0.1.5/docs/source/notes/visualization.rst
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 airfrans-0.1.5/src/airfrans/__init__.py
+-rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 airfrans-0.1.5/src/airfrans/dataset.py
+-rw-r--r--   0        0        0     5175 2020-02-02 00:00:00.000000 airfrans-0.1.5/src/airfrans/naca_generator.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 airfrans-0.1.5/src/airfrans/reorganize.py
+-rw-r--r--   0        0        0     4054 2020-02-02 00:00:00.000000 airfrans-0.1.5/src/airfrans/sampling.py
+-rw-r--r--   0        0        0    23110 2020-02-02 00:00:00.000000 airfrans-0.1.5/src/airfrans/simulation.py
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 airfrans-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 airfrans-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 airfrans-0.1.5/README.md
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 airfrans-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4736 2020-02-02 00:00:00.000000 airfrans-0.1.5/PKG-INFO
```

### Comparing `airfrans-0.1.4/.readthedocs.yaml` & `airfrans-0.1.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.4/docs/Makefile` & `airfrans-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.4/docs/make.bat` & `airfrans-0.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.4/docs/source/conf.py` & `airfrans-0.1.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.4/docs/source/index.rst` & `airfrans-0.1.5/docs/source/index.rst`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 AirfRANS documentation
 ======================
 
 **AirfRANS** is a Python library for handling simulations coming from the AirfRANS dataset which makes available numerical resolutions of the incompressible Reynolds-Averaged Navier–Stokes (RANS) equations over the NACA 4 and 5 digits series of airfoils and in a subsonic flight regime setup.
 
 It consists of a utility for downloading and loading the dataset under a NumPy format and a class to manipulate and execute some basic operations on the simulations. In particular, it allows to compute the force coefficent straightforwardly and it includes a method to visualize boundary layers and trails. Moreover, it allows to sample uniformly or with respect to the mesh density and to get rid of the mesh points constraint for training.
 
+The original paper accepted at the 36th Conference on Neural Information Processing Systems (NeurIPS 2022) Track on Datasets and Benchmarks can be found `here <https://openreview.net/forum?id=Zp8YmiQ_bDC>`_ and the preprint `here <https://arxiv.org/abs/2212.07564>`_. **Disclaimer: An important update correcting an inconsistency in the Machine Learning experiments proposed in the main part of the NeurIPS version of the paper has been done. Please refer to the** `ArXiv version <https://arxiv.org/abs/2212.07564>`_ **for the up to date version.**
+
 .. toctree::
    :glob:
    :maxdepth: 1
    :caption: Notes
 
    notes/introduction
    notes/installation
```

### Comparing `airfrans-0.1.4/docs/source/_figures/boundary_layer.png` & `airfrans-0.1.5/docs/source/_figures/boundary_layer.png`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.4/docs/source/_figures/fields.png` & `airfrans-0.1.5/docs/source/_figures/fields.png`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.4/docs/source/_figures/sampling.png` & `airfrans-0.1.5/docs/source/_figures/sampling.png`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.4/docs/source/_figures/surface.png` & `airfrans-0.1.5/docs/source/_figures/surface.png`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.4/docs/source/notes/dataset.rst` & `airfrans-0.1.5/docs/source/notes/dataset.rst`

 * *Files 0% similar despite different names*

```diff
@@ -54,18 +54,19 @@
 The raw dataset contains the simulations of the AirfRANS dataset as they were outputed by OpenFOAM. The pre-processed version differs from the raw version as it only includes a processed version of the ``.vtu`` / ``.vtp`` files of the simulations.
 
 For the internal field given in the file ending by ``internal.vtu``, we followed:
 
 - **Clipping**: Clip to a box of size ``[(-2, 4), (-1.5, 1.5), (0, 1)]`` where each tuple represents an axis in the order x, y, and z. We did it with the PyVista `clip filter  <https://docs.pyvista.org/version/stable/api/core/_autosummary/pyvista.DataSetFilters.clip_box.html>`_ and we set ``crinkle = True`` in the parameters to leave the cells untouched.
 - **Slicing**:  Take a slice at :math:`z = 0.5` to go from a 3D mesh to a 2D mesh. We did it with the PyVista `slice filter <https://docs.pyvista.org/version/stable/api/core/_autosummary/pyvista.DataSetFilters.slice.html>`_ and we set ``generate_triangles = False``.
 - **Distance function**: Compute the distance function with the PyVista `compute_implicit_distance filter <https://docs.pyvista.org/version/stable/api/core/_autosummary/pyvista.DataSetFilters.compute_implicit_distance.html>`_.
-- **Keep only the required fields**: Only keep the pressure, the velocity, the turbulent viscosity, and the distance function in the data.
+- **Keeping only the required fields**: Only keep the pressure, the velocity, the turbulent viscosity, and the distance function in the data.
 
 For the aerofoil patch (internal boundary) given in the file ending by ``aerofoil.vtp``, we followed:
 
 - **Normals**: Compute the normals with the PyVista `compute_normals filter <https://docs.pyvista.org/version/stable/api/core/_autosummary/pyvista.PolyDataFilters.compute_normals.html>`_. We set ``flip_normals = False`` leading to inward-pointing normals.
 - **Slicing**: Take a slice at :math:`z = 0.5` to go from a 2D mesh to a 1D mesh. We did it with the PyVista `slice filter <https://docs.pyvista.org/version/stable/api/core/_autosummary/pyvista.DataSetFilters.slice.html>`_ and we set ``generate_triangles = False``.
-- **Keep only the required fields**: Only keep the pressure, the velocity, the turbulent velocity, and the normals in the data.
+- **Keeping only the required fields**: Only keep the pressure, the velocity, the turbulent velocity, and the normals in the data.
 
 For the freestream patch (external boundary) given in the file ending by ``freestream.vtp``, we followed:
+
 - **Slicing**: Take a slice at :math:`z = 0.5` to go from a 2D mesh to a 1D mesh. We did it with the PyVista `slice filter <https://docs.pyvista.org/version/stable/api/core/_autosummary/pyvista.DataSetFilters.slice.html>`_ and we set ``generate_triangles = False``.
-- **Keep only the required fields**: Only keep the pressure, the velocity, and the turbulent velocity in the data.
+- **Keeping only the required fields**: Only keep the pressure, the velocity, and the turbulent velocity in the data.
```

### Comparing `airfrans-0.1.4/docs/source/notes/introduction.rst` & `airfrans-0.1.5/docs/source/notes/introduction.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Introduction
 ============
 
-The AirfRANS dataset is a collection of numerical simulations solving the incompressible Reynolds-Averaged Navier-Stokes equations over two dimensional airfoils in a subsonic flight regime. The associated `paper https://arxiv.org/abs/2212.07564`_ has been accepted at the 36th Conference on Neural Information Processing Systems (NeurIPS 2022) Track on Datasets and Benchmarks. In addition to this library two GitHub repositories have been proposed to reconduct the paper `experiments <https://github.com/Extrality/AirfRANS>`_ and to generate new `compressible or incompressible simulations over NACA airfoils <https://github.com/Extrality/NACA_simulation>`_. The setup to generate those simulations have been confronted to the Langley Research Center experiments available in the `Turbulence Modeling Resource <https://turbmodels.larc.nasa.gov/>`_ for the NACA 0012 and 4412.
+The AirfRANS dataset is a collection of numerical simulations solving the incompressible Reynolds-Averaged Navier-Stokes equations over two dimensional airfoils in a subsonic flight regime. The associated `paper <https://arxiv.org/abs/2212.07564>`_ has been accepted at the 36th Conference on Neural Information Processing Systems (NeurIPS 2022) Track on Datasets and Benchmarks. In addition to this library two GitHub repositories have been proposed to reconduct the paper `experiments <https://github.com/Extrality/AirfRANS>`_ and to generate new `compressible or incompressible simulations over NACA airfoils <https://github.com/Extrality/NACA_simulation>`_. The setup to generate those simulations have been confronted to the Langley Research Center experiments available in the `Turbulence Modeling Resource <https://turbmodels.larc.nasa.gov/>`_ for the NACA 0012 and 4412.
 
 This dataset has been built to lower the potential barrier between Machine Learning and Physics research communities. It proposes data on a simple but realistic case which already includes some of the major challenges of Machine Learning for solving Fluid Dynamics, namely:
 
 - working with unstructured data coming from raw numerical simulations,
 - being able to deal with the number of nodes required in simulation meshes (from hundreds of thousands to hundreds of million in 3D cases),
 - treating cases with a realistic Reynolds number,
 - regressing the entire velocity, pressure and turbulent viscosity fields from a geometry and the boundary conditions,
```

### Comparing `airfrans-0.1.4/docs/source/notes/simulation.rst` & `airfrans-0.1.5/docs/source/notes/simulation.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .. note::
 	
-	Since version ``0.1.4``, the normals in the ``airfrans.Simulation`` class are inward-pointing instead ouf outward-pointing previsouly. This for consistency with the normals given in the AirfRANS dataset.
+	Since version ``0.1.4``, the normals in the ``airfrans.Simulation`` class are inward-pointing instead of outward-pointing as previously. This for consistency with the normals given in the AirfRANS dataset.
 
 Simulation
 ==========
 
 Each simulation is defined via boundary conditions (inlet velocity and angle of attack) and a geometry (NACA 4 or 5 digits). We recall that in an incompressible setup and when neglecting gravity, the only parameter of Navier-Stokes equations (and also of RANS equations) is the Reynolds number. If we fix the kinematic viscosity (`i.e.` if we fix the temperature of air one for all), the Reynolds number is completely defined by the inlet velocity (as the characteristic length of airfoil is chosen to be 1 meter). In this dataset, we chose to arbitrarily fix the temperature to 298.15K and to work with properties of air at that temperature, at a pressure of 1013.25 hPa.
 
 You can run new simulation with the help of `OpenFOAM v2112 <https://www.openfoam.com/>`_ and the `NACA simulation GitHub <https://github.com/Extrality/NACA_simulation>`_.
@@ -103,21 +103,23 @@
 
 - :obj:`airfrans.Simulation.sampling_volume` allows sampling from two different densities on the internal mesh domain
 - :obj:`airfrans.Simulation.sampling_surface` allows sampling from two different densities on the airfoil mesh domain
 - :obj:`airfrans.Simulation.sampling_mesh` allows the sampling of nodes in the internal mesh
 
 .. code-block:: python
 
-	sampling_volume_uniform = simulation.sampling_volume(50000, density = 'uniform')
-	sampling_volume_mesh = simulation.sampling_volume(50000, density = 'mesh_density')
+	seed = 0
+
+	sampling_volume_uniform = simulation.sampling_volume(seed, 50000, density = 'uniform')
+	sampling_volume_mesh = simulation.sampling_volume(seed, 50000, density = 'mesh_density')
 	
-	sampling_surface_uniform = simulation.sampling_surface(500, density = 'uniform')
-	sampling_surface_mesh = simulation.sampling_surface(500, density = 'mesh_density')
+	sampling_surface_uniform = simulation.sampling_surface(seed, 500, density = 'uniform')
+	sampling_surface_mesh = simulation.sampling_surface(seed, 500, density = 'mesh_density')
 	
-	sampling_mesh = simulation.sampling_mesh(50000)
+	sampling_mesh = simulation.sampling_mesh(seed, 50000)
 	sampling_mesh_surface = sampling_mesh[sampling_mesh[:, 2].astype('bool')]
 	
 	fig, ax = plt.subplots(2, 3, figsize = (36, 12))
 	ax[0, 0].scatter(sampling_volume_uniform[:, 0], sampling_volume_uniform[:, 1], c = sampling_volume_uniform[:, 3], s = 0.75)
 	ax[0, 1].scatter(sampling_volume_mesh[:, 0], sampling_volume_mesh[:, 1], c = sampling_volume_mesh[:, 3], s = 0.75)
 	ax[0, 2].scatter(sampling_mesh[:, 0], sampling_mesh[:, 1], c = sampling_mesh[:, 8], s = 0.75)
 	ax[1, 0].scatter(sampling_surface_uniform[:, 0], sampling_surface_uniform[:, 1], s = 0.75)
```

### Comparing `airfrans-0.1.4/docs/source/notes/visualization.rst` & `airfrans-0.1.5/docs/source/notes/visualization.rst`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.4/src/airfrans/dataset.py` & `airfrans-0.1.5/src/airfrans/dataset.py`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.4/src/airfrans/naca_generator.py` & `airfrans-0.1.5/src/airfrans/naca_generator.py`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.4/src/airfrans/reorganize.py` & `airfrans-0.1.5/src/airfrans/reorganize.py`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.4/src/airfrans/sampling.py` & `airfrans-0.1.5/src/airfrans/sampling.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import numpy as np
 
-def cell_sampling_2d(cell_points, cell_attr = None):
+def cell_sampling_2d(seed, cell_points, cell_attr = None):
     '''
     Sample points in a two dimensional cell via parallelogram sampling and triangle interpolation via barycentric coordinates.
     The vertices have to be ordered in a certain way.
 
     Args:
+        seed (int): Seed for the random number generator.
         cell_points (np.ndarray): Vertices of the 2 dimensional cells. Shape `(N, 4)` for N cells with 4 vertices.
         cell_attr (np.ndarray, optional): Features of the vertices of the 2 dimensional cells. Shape `(N, 4, k)` for N cells with 4 edges and k features. 
             If given shape `(N, 4)` it will resize it automatically in a `(N, 4, 1)` tensor. Default: ``None``
     '''
+    rng = np.random.default_rng(seed = seed)
+
     # Sampling via triangulation of the cell and parallelogram sampling
     v0, v1 = cell_points[:, 1] - cell_points[:, 0], cell_points[:, 3] - cell_points[:, 0]
     v2, v3 = cell_points[:, 3] - cell_points[:, 2], cell_points[:, 1] - cell_points[:, 2]  
     a0, a1 = np.abs(np.linalg.det(np.hstack([v0[:, :2], v1[:, :2]]).reshape(-1, 2, 2))), \
                 np.abs(np.linalg.det(np.hstack([v2[:, :2], v3[:, :2]]).reshape(-1, 2, 2)))
     p = a0/(a0 + a1)
-    index_triangle = np.random.binomial(1, p)[:, None]
-    u = np.random.uniform(size = (len(p), 2))
+    index_triangle = rng.binomial(1, p)[:, None]
+    u = rng.uniform(size = (len(p), 2))
     sampled_point = index_triangle*(u[:, 0:1]*v0 + u[:, 1:2]*v1) + (1 - index_triangle)*(u[:, 0:1]*v2 + u[:, 1:2]*v3)
     sampled_point_mirror = index_triangle*((1 - u[:, 0:1])*v0 + (1 - u[:, 1:2])*v1) + (1 - index_triangle)*((1 - u[:, 0:1])*v2 + (1 - u[:, 1:2])*v3)
     reflex = (u.sum(axis = 1) > 1)
     sampled_point[reflex] = sampled_point_mirror[reflex]
 
     # Interpolation on a triangle via barycentric coordinates
     if cell_attr is not None:
@@ -39,25 +42,28 @@
         attr2 = index_triangle*cell_attr[:, 3] + (1 - index_triangle)*cell_attr[:, 3]
         sampled_attr = w0[:, None]*attr0 + w1[:, None]*attr1 + w2[:, None]*attr2
 
     sampled_point += index_triangle*cell_points[:, 0] + (1 - index_triangle)*cell_points[:, 2]    
 
     return np.hstack([sampled_point[:, :2], sampled_attr]) if cell_attr is not None else sampled_point[:, :2]
 
-def cell_sampling_1d(line_points, line_attr = None):
+def cell_sampling_1d(seed, line_points, line_attr = None):
     '''
     Sample points in a one dimensional cell via linear sampling and interpolation.
 
     Args:
+        seed (int): Seed for the random number generator.
         line_points (np.ndarray): Edges of the 1 dimensional cells. Shape `(N, 2)` for N cells with 2 edges.
         line_attr (np.ndarray, optional): Features of the edges of the 1 dimensional cells. Shape `(N, 2, k)` for N cells with 2 edges and k features.
             If given shape `(N, 2)` it will resize it automatically in a `(N, 2, 1)` tensor. Default: ``None``
     '''
+    rng = np.random.default_rng(seed = seed)
+
     # Linear sampling
-    u = np.random.uniform(size = (len(line_points), 1))
+    u = rng.uniform(size = (len(line_points), 1))
     sampled_point = u*line_points[:, 0] + (1 - u)*line_points[:, 1]
 
     # Linear interpolation
     if line_attr is not None:   
         if len(line_attr.shape) == 2:
             line_attr = line_attr[:, :, None]
         sampled_attr = u*line_attr[:, 0] + (1 - u)*line_attr[:, 1]
```

### Comparing `airfrans-0.1.4/src/airfrans/simulation.py` & `airfrans-0.1.5/src/airfrans/simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,80 +62,92 @@
             )
 
         # Targets
         self.velocity = np.array(self.internal.point_data['U'][:, :2]).astype('float64')
         self.pressure = np.array(self.internal.point_data['p'][:, None]).astype('float64')
         self.nu_t = np.array(self.internal.point_data['nut'][:, None]).astype('float64')
 
-    def sampling_volume(self, n, density = 'uniform', targets = True):
+    def sampling_volume(self, seed, n, density = 'uniform', targets = True):
         """
         Sample points in the internal mesh following the given density.
 
         Args:
+            seed (int): Seed for the random number generator.
             n (int): Number of sampled points.
             density (str, optional): Density from which the sampling is done. Choose between ``'uniform'`` and ``'mesh_density'``. Default: ``'uniform'``
             targets (bool, optional): If ``True``, velocity, pressure and kinematic turbulent viscosity will be returned in the output ndarray. Default: ``True``
         """
+        rng = np.random.default_rng(seed = seed)
+
         if density == 'uniform': # Uniform sampling strategy
             p = np.array(self.internal.cell_data['Area']/self.internal.cell_data['Area'].sum())
-            sampled_cell_indices = np.random.choice(self.internal.n_cells, size = n, replace = True, p = p)
+            sampled_cell_indices = rng.choice(self.internal.n_cells, size = n, replace = True, p = p)
         elif density == 'mesh_density': # Sample via mesh density
-            sampled_cell_indices = np.random.choice(self.internal.n_cells, size = n, replace = True)
+            sampled_cell_indices = rng.choice(self.internal.n_cells, size = n, replace = True)
 
         cell_dict = np.array(self.internal.cells).reshape(-1, 5)[sampled_cell_indices, 1:]
         cell_points = self.position[cell_dict]
 
         if targets:
             cell_attr = np.concatenate([self.sdf[cell_dict], self.velocity[cell_dict], self.pressure[cell_dict], self.nu_t[cell_dict]], axis = -1)
         else:
-            cell_attr = self.sdf[cell_dict]            
+            cell_attr = self.sdf[cell_dict]   
+
+        seed_sampling = rng.integers(10000)         
 
-        return sampling.cell_sampling_2d(cell_points, cell_attr)
+        return sampling.cell_sampling_2d(seed_sampling, cell_points, cell_attr)
     
-    def sampling_surface(self, n, density = 'uniform', targets = True):
+    def sampling_surface(self, seed, n, density = 'uniform', targets = True):
         """
         Sample points in the airfoil mesh following the given density.
 
         Args:
+            seed (int): Seed for the random number generator.
             n (int): Number of sampled points.
             density (str, optional): Density from which the sampling is done. Choose between ``'uniform'`` and ``'mesh_density'``. Default: ``'uniform'``
             targets (bool, optional): If ``True``, velocity, pressure and kinematic turbulent viscosity will be returned in the output ndarray. Default: ``True``
         """
+        rng = np.random.default_rng(seed = seed)
+
         if density == 'uniform': # Uniform sampling strategy
             p = np.array(self.airfoil.cell_data['Length']/self.airfoil.cell_data['Length'].sum())
-            sampled_line_indices = np.random.choice(self.airfoil.n_cells, size = n, replace = True, p = p)
+            sampled_line_indices = rng.choice(self.airfoil.n_cells, size = n, replace = True, p = p)
         elif density == 'mesh_density': # Sample via mesh density
-            sampled_line_indices = np.random.choice(self.airfoil.n_cells, size = n, replace = True)
+            sampled_line_indices = rng.choice(self.airfoil.n_cells, size = n, replace = True)
 
         line_dict = np.array(self.airfoil.lines).reshape(-1, 3)[sampled_line_indices, 1:]
         line_points = np.array(self.airfoil.points)[line_dict]
 
         normal = np.array(self.airfoil.point_data['Normals'][line_dict, :2]) 
 
         if targets:
             line_attr = np.concatenate([
                 normal, 
                 np.array(self.airfoil.point_data['U'][line_dict, :2]), 
                 np.array(self.airfoil.point_data['p'][line_dict, None]), 
                 np.array(self.airfoil.point_data['nut'][line_dict, None])
                 ], axis = -1)
         else:
-            line_attr = normal     
+            line_attr = normal  
 
-        return sampling.cell_sampling_1d(line_points, line_attr)
+        seed_sampling = rng.integers(10000)
 
-    def sampling_mesh(self, n, targets = True):
+        return sampling.cell_sampling_1d(seed_sampling, line_points, line_attr)
+
+    def sampling_mesh(self, seed, n, targets = True):
         """
         Sample points over the simulation mesh without replacement.
 
         Args:
+            seed (int): Seed for the random number generator.
             n (int): Number of sampled points, this number has to be lower than the total number of points in the mesh.
             targets (bool, optional): If ``True``, velocity, pressure and kinematic turbulent viscosity will be returned in the output ndarray. Default: ``True``
         """
-        idx = np.random.choice(self.position.shape[0], size = n, replace = False)
+        rng = np.random.default_rng(seed = seed)
+        idx = rng.choice(self.position.shape[0], size = n, replace = False)
 
         # Position
         position = self.position[idx]
 
         # Inputs
         surface = self.surface[idx]
         sdf = self.sdf[idx]
@@ -226,14 +238,15 @@
     def force_coefficient(self, compressible = False, reference = False):
         """
         Compute the force coefficients for the simulation. The output is a tuple of the form `((cd, cdp, cdv), (cl, clp, clv))`,
         where `cd` is the drag coefficient, `cdp` the pressure contribution of the drag coefficient and `cdv` the viscous
         contribution of the drag coefficient. Same for the lift coefficient `cl`.
 
         Args:
+            compressible (bool, optional): If ``False``, multiply the force computed with the simulation field by the specific mass. Default: ``False``
             reference (bool, optional): If ``True``, return the force coefficients computed with the reference fields.
                 If ``False``, compute the force coefficients with the fields attribute of the class. Default: ``False``   
         """
         f, fp, fv = self.force(compressible = compressible, reference = reference)
 
         basis = np.array([[np.cos(self.angle_of_attack), np.sin(self.angle_of_attack)], [-np.sin(self.angle_of_attack), np.cos(self.angle_of_attack)]])
         fp_rot, fv_rot = np.matmul(basis, fp), np.matmul(basis, fv)
```

### Comparing `airfrans-0.1.4/.gitignore` & `airfrans-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.4/LICENSE` & `airfrans-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `airfrans-0.1.4/README.md` & `airfrans-0.1.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -46,18 +46,20 @@
 ```
 See the documentation for more details about this object.
 
 ## License
 This project is licensed under the [ODbL-1.0 License](https://opendatacommons.org/licenses/odbl/1-0/).
 
 ## Reference
-The original paper accepted at the 36th Conference on Neural Information Processing Systems (NeurIPS 2022) Track on Datasets and Benchmarks can be found [here](https://openreview.net/forum?id=Zp8YmiQ_bDC) and the preprint [here](https://arxiv.org/abs/2212.07564). Please cite this paper if you use this dataset in your own work.
+The original paper accepted at the 36th Conference on Neural Information Processing Systems (NeurIPS 2022) Track on Datasets and Benchmarks can be found [here](https://openreview.net/forum?id=Zp8YmiQ_bDC) and the preprint [here](https://arxiv.org/abs/2212.07564). **Disclaimer: An important update correcting an inconsistency in the Machine Learning experiments proposed in the main part of the NeurIPS version of the paper has been done. Please refer to the [ArXiv version](https://arxiv.org/abs/2212.07564) for the up to date version.** 
+
+Please cite this paper if you use this dataset in your own work.
 ```
 @inproceedings{
 bonnet2022airfrans,
 title={Airf{RANS}: High Fidelity Computational Fluid Dynamics Dataset for Approximating Reynolds-Averaged Navier{\textendash}Stokes Solutions},
 author={Florent Bonnet and Jocelyn Ahmed Mazari and Paola Cinnella and Patrick Gallinari},
 booktitle={Thirty-sixth Conference on Neural Information Processing Systems Datasets and Benchmarks Track},
 year={2022},
-url={https://openreview.net/forum?id=Zp8YmiQ_bDC}
+url={https://arxiv.org/abs/2212.07564}
   }
 ```
```

### Comparing `airfrans-0.1.4/pyproject.toml` & `airfrans-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "airfrans"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Florent Bonnet", email="bonnet@isir.upmc.fr" },
 ]
 description = "A package to facilitate the manipulation of the AirfRANS dataset simulations."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `airfrans-0.1.4/PKG-INFO` & `airfrans-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airfrans
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package to facilitate the manipulation of the AirfRANS dataset simulations.
 Project-URL: Homepage, https://github.com/Extrality/airfrans_lib
 Project-URL: Bug Tracker, https://github.com/Extrality/airfrans_lib/issues
 Author-email: Florent Bonnet <bonnet@isir.upmc.fr>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -65,18 +65,20 @@
 ```
 See the documentation for more details about this object.
 
 ## License
 This project is licensed under the [ODbL-1.0 License](https://opendatacommons.org/licenses/odbl/1-0/).
 
 ## Reference
-The original paper accepted at the 36th Conference on Neural Information Processing Systems (NeurIPS 2022) Track on Datasets and Benchmarks can be found [here](https://openreview.net/forum?id=Zp8YmiQ_bDC) and the preprint [here](https://arxiv.org/abs/2212.07564). Please cite this paper if you use this dataset in your own work.
+The original paper accepted at the 36th Conference on Neural Information Processing Systems (NeurIPS 2022) Track on Datasets and Benchmarks can be found [here](https://openreview.net/forum?id=Zp8YmiQ_bDC) and the preprint [here](https://arxiv.org/abs/2212.07564). **Disclaimer: An important update correcting an inconsistency in the Machine Learning experiments proposed in the main part of the NeurIPS version of the paper has been done. Please refer to the [ArXiv version](https://arxiv.org/abs/2212.07564) for the up to date version.** 
+
+Please cite this paper if you use this dataset in your own work.
 ```
 @inproceedings{
 bonnet2022airfrans,
 title={Airf{RANS}: High Fidelity Computational Fluid Dynamics Dataset for Approximating Reynolds-Averaged Navier{\textendash}Stokes Solutions},
 author={Florent Bonnet and Jocelyn Ahmed Mazari and Paola Cinnella and Patrick Gallinari},
 booktitle={Thirty-sixth Conference on Neural Information Processing Systems Datasets and Benchmarks Track},
 year={2022},
-url={https://openreview.net/forum?id=Zp8YmiQ_bDC}
+url={https://arxiv.org/abs/2212.07564}
   }
 ```
```

