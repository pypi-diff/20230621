# Comparing `tmp/smmregrid-0.0.1.tar.gz` & `tmp/smmregrid-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smmregrid-0.0.1.tar", last modified: Sat May 13 14:08:49 2023, max compression
+gzip compressed data, was "smmregrid-0.0.2.tar", last modified: Wed Jun 21 13:40:10 2023, max compression
```

## Comparing `smmregrid-0.0.1.tar` & `smmregrid-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 paolo     (1028) paolo     (1028)        0 2023-05-13 14:08:49.212745 smmregrid-0.0.1/
--rw-rw-r--   0 paolo     (1028) paolo     (1028)    11357 2023-01-30 09:30:49.000000 smmregrid-0.0.1/LICENSE
--rw-rw-r--   0 paolo     (1028) paolo     (1028)     2996 2023-05-13 14:08:49.212745 smmregrid-0.0.1/PKG-INFO
--rw-rw-r--   0 paolo     (1028) paolo     (1028)     2206 2023-05-13 14:08:16.000000 smmregrid-0.0.1/README.md
--rw-rw-r--   0 paolo     (1028) paolo     (1028)     1234 2023-05-13 14:08:16.000000 smmregrid-0.0.1/pyproject.toml
--rw-rw-r--   0 paolo     (1028) paolo     (1028)       38 2023-05-13 14:08:49.212745 smmregrid-0.0.1/setup.cfg
-drwxrwxr-x   0 paolo     (1028) paolo     (1028)        0 2023-05-13 14:08:49.212745 smmregrid-0.0.1/smmregrid/
--rw-rw-r--   0 paolo     (1028) paolo     (1028)      165 2023-05-13 14:08:16.000000 smmregrid-0.0.1/smmregrid/__init__.py
--rw-rw-r--   0 paolo     (1028) paolo     (1028)     9406 2023-05-13 14:08:16.000000 smmregrid-0.0.1/smmregrid/cdo_weights.py
--rw-rw-r--   0 paolo     (1028) paolo     (1028)     2198 2023-05-13 14:08:16.000000 smmregrid-0.0.1/smmregrid/checker.py
--rw-rw-r--   0 paolo     (1028) paolo     (1028)     2920 2023-02-23 22:03:32.000000 smmregrid-0.0.1/smmregrid/dimension.py
--rw-rw-r--   0 paolo     (1028) paolo     (1028)     2985 2023-05-13 14:08:16.000000 smmregrid-0.0.1/smmregrid/esmf_weights.py
--rw-rw-r--   0 paolo     (1028) paolo     (1028)    17232 2023-05-13 14:08:16.000000 smmregrid-0.0.1/smmregrid/regrid.py
--rw-rw-r--   0 paolo     (1028) paolo     (1028)      415 2023-05-13 14:08:16.000000 smmregrid-0.0.1/smmregrid/util.py
--rw-rw-r--   0 paolo     (1028) paolo     (1028)     3692 2023-05-13 14:08:16.000000 smmregrid-0.0.1/smmregrid/weights.py
-drwxrwxr-x   0 paolo     (1028) paolo     (1028)        0 2023-05-13 14:08:49.212745 smmregrid-0.0.1/smmregrid.egg-info/
--rw-rw-r--   0 paolo     (1028) paolo     (1028)     2996 2023-05-13 14:08:49.000000 smmregrid-0.0.1/smmregrid.egg-info/PKG-INFO
--rw-rw-r--   0 paolo     (1028) paolo     (1028)      372 2023-05-13 14:08:49.000000 smmregrid-0.0.1/smmregrid.egg-info/SOURCES.txt
--rw-rw-r--   0 paolo     (1028) paolo     (1028)        1 2023-05-13 14:08:49.000000 smmregrid-0.0.1/smmregrid.egg-info/dependency_links.txt
--rw-rw-r--   0 paolo     (1028) paolo     (1028)      111 2023-05-13 14:08:49.000000 smmregrid-0.0.1/smmregrid.egg-info/requires.txt
--rw-rw-r--   0 paolo     (1028) paolo     (1028)       10 2023-05-13 14:08:49.000000 smmregrid-0.0.1/smmregrid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:40:10.900054 smmregrid-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 13:39:45.000000 smmregrid-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-21 13:40:10.900054 smmregrid-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-21 13:39:45.000000 smmregrid-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-21 13:39:45.000000 smmregrid-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 13:40:10.900054 smmregrid-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:40:10.900054 smmregrid-0.0.2/smmregrid/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-21 13:39:45.000000 smmregrid-0.0.2/smmregrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9471 2023-06-21 13:39:45.000000 smmregrid-0.0.2/smmregrid/cdo_weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-21 13:39:45.000000 smmregrid-0.0.2/smmregrid/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-06-21 13:39:45.000000 smmregrid-0.0.2/smmregrid/dimension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-21 13:39:45.000000 smmregrid-0.0.2/smmregrid/esmf_weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-21 13:39:45.000000 smmregrid-0.0.2/smmregrid/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17373 2023-06-21 13:39:45.000000 smmregrid-0.0.2/smmregrid/regrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-21 13:39:45.000000 smmregrid-0.0.2/smmregrid/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-06-21 13:39:45.000000 smmregrid-0.0.2/smmregrid/weights.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:40:10.900054 smmregrid-0.0.2/smmregrid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-21 13:40:10.000000 smmregrid-0.0.2/smmregrid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-21 13:40:10.000000 smmregrid-0.0.2/smmregrid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 13:40:10.000000 smmregrid-0.0.2/smmregrid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-21 13:40:10.000000 smmregrid-0.0.2/smmregrid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 13:40:10.000000 smmregrid-0.0.2/smmregrid.egg-info/top_level.txt
```

### Comparing `smmregrid-0.0.1/LICENSE` & `smmregrid-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `smmregrid-0.0.1/PKG-INFO` & `smmregrid-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: smmregrid
-Version: 0.0.1
+Version: 0.0.2
 Summary: Regridding based on sparse matrix multiplication
 Author-email: Jost von Hardenberg <jost.hardenberg@polito.it>, Paolo Davini <p.davini@isac.cnr.it>, Scott Wales <scott.wales@unimelb.edu.au>
 Project-URL: Homepage, https://github.com/jhardenberg/smmregrid
 Project-URL: Bug Tracker, https://github.com/jhardenberg/smmregrid/issues
-Project-URL: Repository, https://github.com/oloapinivad/ECmean4
+Project-URL: Repository, https://github.com/jhardenberg/smmregrid
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
+Provides-Extra: notebooks
 Provides-Extra: all
 License-File: LICENSE
 
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/jhardenberg/smmregrid/graphs/commit-activity)
 [![PyTest](https://github.com/jhardenberg/smmregrid/actions/workflows/mambatest.yml/badge.svg)](https://github.com/jhardenberg/smmregrid/actions/workflows/mambatest.yml)
 [![Coverage Status](https://coveralls.io/repos/github/jhardenberg/smmregrid/badge.svg?branch=main)](https://coveralls.io/github/jhardenberg/smmregrid?branch=main)
 [![PyPI version](https://badge.fury.io/py/smmregrid.svg)](https://badge.fury.io/py/smmregrid)
```

### Comparing `smmregrid-0.0.1/README.md` & `smmregrid-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `smmregrid-0.0.1/pyproject.toml` & `smmregrid-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -23,33 +23,41 @@
     'numpy',
     'xarray',
     'dask',
     'netcdf4',
     'cfgrib',
     'dask',
     'sparse',
-    'cdo'
+    'cdo',
+    'numba',
+    'cfunits'
 ]
 
 [project.optional-dependencies]
 tests = [
     "coverage",
     "coveralls",
     "pytest"
 ]
 
+notebooks = [
+    "ipykernel",
+    "matplotlib",
+    "jinja2"
+]
+
 #docs = [
 #    "sphinx",
 #    "sphinx-rtd-theme"
 #]
 
 all = [
-    "scriptengine[tests]"
+    "smmregrid[tests,notebooks]"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/jhardenberg/smmregrid"
 "Bug Tracker" = "https://github.com/jhardenberg/smmregrid/issues"
-"Repository" = "https://github.com/oloapinivad/ECmean4"
+"Repository" = "https://github.com/jhardenberg/smmregrid"
 
 [tool.setuptools.dynamic]
 version = {attr = "smmregrid.__version__"}
```

### Comparing `smmregrid-0.0.1/smmregrid/cdo_weights.py` & `smmregrid-0.0.2/smmregrid/cdo_weights.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 """CDO-based generation of weights"""
 
 import os
 import sys
-import logging
 import tempfile
 import subprocess
 from multiprocessing import Process, Manager
 import numpy
 import xarray
-from .util import find_vert_coord
+from .util import find_vert_coords
 from .weights import compute_weights_matrix3d, compute_weights_matrix, mask_weights, check_mask
+import logging
+
+# set up logger
+loggy = logging.getLogger(__name__)
 
 
 def worker(wlist, nnn, *args, **kwargs):
     """Run a worker process"""
     wlist[nnn] = cdo_generate_weights2d(*args, **kwargs).compute()
 
+
 def cdo_generate_weights(source_grid, target_grid, method="con", extrapolate=True,
                          remap_norm="fracarea", remap_area_min=0.0, icongridpath=None,
                          gridpath=None, extra=None, vert_coord=None, cdo="cdo", nproc=1):
     """Generate the weights using CDO, handling both 2D and 3D cases"""
 
     # Check if there is a vertical coordinate for 3d oceanic data
     if not vert_coord:
-        vert_coord = find_vert_coord(source_grid)
-        logging.warning('vert_coord is %s',str(vert_coord))
+        vert_coord = find_vert_coords(source_grid)
+        loggy.info('vert_coord is %s', str(vert_coord))
 
-    if not vert_coord: # Are we 2D? Use default method
-        weights =cdo_generate_weights2d(
+    if not vert_coord:  # Are we 2D? Use default method
+        weights = cdo_generate_weights2d(
             source_grid,
             target_grid,
             method=method,
             extrapolate=extrapolate,
             remap_norm=remap_norm,
             remap_area_min=remap_area_min,
             icongridpath=icongridpath,
@@ -46,54 +50,54 @@
         masked = int(check_mask(weights, vert_coord))
         masked_xa = xarray.DataArray(masked, name="dst_grid_masked")
 
         return xarray.merge([weights, masked_xa])
 
     else:  # we are 3D
         if extra:
-        # make sure extra is a flat list if it is not already
+            # make sure extra is a flat list if it is not already
             if not isinstance(extra, list):
                 extra = [extra]
         else:
             extra = []
 
         if isinstance(source_grid, str):
             sgrid = xarray.open_dataset(source_grid)
         else:
             sgrid = source_grid
 
         nvert = sgrid[vert_coord].values.size
-        #print(nvert)
+        # print(nvert)
 
         # for lev in range(0, nvert):
         mgr = Manager()
 
         # dictionaries are shared, so they have to be passed as functions
-        wlist= mgr.list(range(nvert))
+        wlist = mgr.list(range(nvert))
 
         num_blocks, remainder = divmod(nvert, nproc)
         num_blocks = num_blocks + (0 if remainder == 0 else 1)
 
         blocks = numpy.array_split(numpy.arange(nvert), num_blocks)
         for block in blocks:
             processes = []
             for lev in block:
-                logging.info("Generating level: %s", str(lev))
+                loggy.info("Generating level: %s", str(lev))
                 extra2 = [f"-sellevidx,{lev+1}"]
                 ppp = Process(target=worker,
-                            args=(wlist, lev, source_grid, target_grid),
-                            kwargs=dict(method=method,
-                                        extrapolate=extrapolate,
-                                        remap_norm=remap_norm,
-                                        remap_area_min=remap_area_min,
-                                        icongridpath=icongridpath,
-                                        gridpath=gridpath,
-                                        extra=extra + extra2,
-                                        cdo=cdo,
-                                        nproc=nproc))
+                              args=(wlist, lev, source_grid, target_grid),
+                              kwargs=dict(method=method,
+                                          extrapolate=extrapolate,
+                                          remap_norm=remap_norm,
+                                          remap_area_min=remap_area_min,
+                                          icongridpath=icongridpath,
+                                          gridpath=gridpath,
+                                          extra=extra + extra2,
+                                          cdo=cdo,
+                                          nproc=nproc))
                 ppp.start()
                 processes.append(ppp)
 
             for proc in processes:
                 proc.join()
 
         weights = weightslist_to_3d(wlist, vert_coord)
@@ -190,42 +194,42 @@
             # make sure extra is a flat list if it is not already
             if not isinstance(extra, list):
                 extra = [extra]
 
             subprocess.check_output(
                 [
                     cdo,
-                    "gen%s,%s" % (method, tgrid)
+                    f"gen{method},{tgrid}"
                 ] + extra +
                 [
                     sgrid,
                     weight_file.name,
                 ],
                 stderr=subprocess.PIPE,
                 env=env,
             )
         else:
             subprocess.check_output(
                 [
                     cdo,
-                    "gen%s,%s" % (method, tgrid),
+                    f"gen{method},{tgrid}",
                     sgrid,
                     weight_file.name,
                 ],
                 stderr=subprocess.PIPE,
                 env=env,
             )
 
         # Grab the weights file it outputs as a xarray.Dataset
         weights = xarray.open_dataset(weight_file.name, engine="netcdf4")
         return weights
 
     except subprocess.CalledProcessError as err:
         # Print the CDO error message
-        logging.error(err.output.decode(), file=sys.stderr)
+        print(err.output.decode(), file=sys.stderr)
         raise
 
     finally:
         # Clean up the temporary files
         if not isinstance(source_grid, str):
             source_grid_file.close()
         if not isinstance(target_grid, str):
@@ -238,23 +242,23 @@
     Function to combine a list of 2D cdo weights into a 3D one adding a vertical coordinate lev
     """
     # CDO 2.2.0 fix
     if "numLinks" in ds_list[0].dims:
         links_dim = "numLinks"
     else:
         links_dim = "num_links"
-    
+
     dim_values = range(len(ds_list))
     nl = [ds.src_address.size for ds in ds_list]
     nl0 = max(nl)
     nlda = xarray.DataArray(nl, coords={vert_coord: range(0, len(nl))}, name="link_length")
     new_array = []
     varlist = ["src_address", "dst_address", "remap_matrix", "src_grid_imask", "dst_grid_imask"]
     ds0 = ds_list[0].drop_vars(varlist)
     for x, d in zip(ds_list, dim_values):
         nl1 = x.src_address.size
 #        xplist = [x[vname].pad(num_links=(0, nl0-nl1), mode='constant', constant_values=0)
-        xplist = [x[vname].pad(**{links_dim: (0, nl0-nl1), "mode": 'constant', "constant_values": 0})
-                  for vname in varlist ]
-        xp = xarray.merge(xplist)
-        new_array.append(xp.assign_coords({vert_coord: d}))
+        xplist = [x[vname].pad(**{links_dim: (0, nl0 - nl1), "mode": 'constant', "constant_values": 0})
+                  for vname in varlist]
+        xmerged = xarray.merge(xplist)
+        new_array.append(xmerged.assign_coords({vert_coord: d}))
     return xarray.merge([nlda, ds0, xarray.concat(new_array, vert_coord)])
```

### Comparing `smmregrid-0.0.1/smmregrid/checker.py` & `smmregrid-0.0.2/smmregrid/checker.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Module for cdo-smmregrid comparison"""
 
 import numpy as np
 import xarray as xr
 from cdo import Cdo
-import xarray as xr
-from smmregrid import cdo_generate_weights, Regridder
+from smmregrid import Regridder, cdo_generate_weights
 
 
 cdo = Cdo()
 
 
 def find_var(xfield):
     """Find them most likely set of vars that needs to be interpolated"""
@@ -20,46 +19,53 @@
     # if find none otherwise, pick what you have
     if not myvar:
         myvar = list(xfield.data_vars)
 
     return myvar
 
 
-def check_cdo_regrid(finput, ftarget, method='con', access='Dataset', vert_coord=None):
+def check_cdo_regrid(finput, ftarget, remap_method='con', access='Dataset',
+                     init_method='grids', vert_coord=None):
     """Given a file to be interpolated finput over the ftarget grid,
     check if the output of the last variable is the same as produced
     by CDO remap command. This function is used for tests."""
 
     # define files and open input file
     xfield = xr.open_mfdataset(finput)
 
     # var as the last available
     # myvar = list(xfield.data_vars)[-1]
 
     # interpolation with pure CDO
-    cdo_interpolator = getattr(cdo,  'remap' + method)
+    cdo_interpolator = getattr(cdo, 'remap' + remap_method)
     cdofield = cdo_interpolator(ftarget, input=finput, returnXDataset=True)
     # print(cdofield)
 
     # var as the one which have time and not have bnds (could work)
     smmvar = find_var(xfield)
     cdovar = find_var(cdofield)
 
     if len(smmvar) == 1 and access == 'DataArray':
         xfield = xfield[smmvar[0]]
     if len(cdovar) == 1 and access == 'DataArray':
         cdofield = cdofield[cdovar[0]]
 
     # interpolation with smmregrid (CDO-based)
     # method with creation of weights
-    #wfield = cdo_generate_weights(finput, ftarget, method=method)
-    #interpolator = Regridder(weights=wfield)
+    # wfield = cdo_generate_weights(finput, ftarget, method=method)
+    # interpolator = Regridder(weights=wfield)
 
     # method with automatic creation of weights
-    interpolator = Regridder(source_grid=finput, target_grid=ftarget, method=method, vert_coord=vert_coord)
+    if init_method == 'grids':
+        interpolator = Regridder(source_grid=finput, target_grid=ftarget,
+                                 method=remap_method, vert_coord=vert_coord)
+    if init_method == 'weights':
+        wfield = cdo_generate_weights(finput, ftarget,
+                                      method=remap_method, vert_coord=vert_coord)
+        interpolator = Regridder(weights=wfield, vert_coord=vert_coord)
     rfield = interpolator.regrid(xfield)
 
     if access == 'Dataset':
         rfield = rfield[smmvar].to_array()
         cdofield = cdofield[cdovar].to_array()
 
     # check if arrays are equal with numerical tolerance
```

### Comparing `smmregrid-0.0.1/smmregrid/dimension.py` & `smmregrid-0.0.2/smmregrid/dimension.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import print_function
 
-#from cfunits import Units
+# from cfunits import Units
 import numpy
 
 
 def remove_degenerate_axes(coord):
     """
     Remove any degenerate axes from the coordinate, where all the values along a dimension are identical
```

### Comparing `smmregrid-0.0.1/smmregrid/esmf_weights.py` & `smmregrid-0.0.2/smmregrid/esmf_weights.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """ESMF-based generation of weights"""
 
 import tempfile
 import subprocess
 import xarray
 
+
 def esmf_generate_weights(
     source_grid,
     target_grid,
     method="bilinear",
     extrap_method="nearestidavg",
     norm_type="dstarea",
     line_type=None,
```

### Comparing `smmregrid-0.0.1/smmregrid/regrid.py` & `smmregrid-0.0.2/smmregrid/regrid.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,28 +32,29 @@
 :class:`Regrid` can create basic weights and store them to apply the weights to
 multiple datasets.
 """
 
 
 import math
 import sys
-import logging
 import xarray
 import numpy
-import sparse
 import dask.array
 from .dimension import remove_degenerate_axes
 from .cdo_weights import cdo_generate_weights
-from .util import find_vert_coord
+from .util import find_vert_coords
 from .weights import compute_weights_matrix3d, compute_weights_matrix, mask_weights, check_mask
+import logging
 
+# set up logger
+loggy = logging.getLogger(__name__)
 
 # default spatial dimensions and vertical coordinates
 default_space_dims = ['i', 'j', 'x', 'y', 'lon', 'lat', 'longitude', 'latitude',
-                     'cell', 'cells', 'ncells', 'values', 'value', 'nod2', 'pix']
+                     'cell', 'cells', 'ncells', 'values', 'value', 'nod2', 'pix', 'elem']
 
 
 def apply_weights(source_data, weights, weights_matrix=None, masked=True, space_dims=None):
     """
     Apply the CDO weights ``weights`` to ``source_data``, performing a regridding operation
 
     Args:
@@ -64,101 +65,100 @@
 
     Returns:
         xarray.DataArray: Regridded version of the source dataset
     """
 
     # Understand immediately if we need to return something or not
     # This is done if we have bounds variables
-    if ("bnds" in source_data.name or "bounds" in source_data.name):
+    if any(substring in source_data.name for substring in ["bnds", "bounds", "vertices"]):
 
         # we keep time bounds, and we ignore all the rest
         if 'time' in source_data.name:
-            logging.info('original %s', source_data.name)
+            loggy.info('%s will not be interpolated in the output', source_data.name)
             return source_data
         else:
-            logging.info('empty %s', source_data.name)
+            loggy.info('%s will be excluded from the output', source_data.name)
             return xarray.DataArray(data=None)
 
     # Alias the weights dataset from CDO
     w = weights
 
     # The weights file contains a sparse matrix, that we need to multiply the
     # source data's horizontal grid with to get the regridded data.
     #
     # A bit of messing about with `.stack()` is needed in order to get the
     # dimensions to conform - the horizontal grid needs to be converted to a 1d
     # array, multiplied by the weights matrix, then unstacked back into a 2d
     # array
 
-    #if w.title.startswith("ESMF"):
+    # if w.title.startswith("ESMF"):
     if "S" in w.variables:
         # ESMF style weights
-        #src_address = w.col - 1
-        #dst_address = w.row - 1
-        #remap_matrix = w.S
-        #w_shape = (w.sizes["n_a"], w.sizes["n_b"])
+        # src_address = w.col - 1
+        # dst_address = w.row - 1
+        # remap_matrix = w.S
+        # w_shape = (w.sizes["n_a"], w.sizes["n_b"])
 
         dst_grid_shape = w.dst_grid_dims.values
         dst_grid_center_lat = w.yc_b.data.reshape(dst_grid_shape[::-1])
         dst_grid_center_lon = w.xc_b.data.reshape(dst_grid_shape[::-1])
 
         dst_mask = w.mask_b
 
         axis_scale = 1  # Weight lat/lon in degrees
 
     else:
         # CDO style weights
-        #src_address = w.src_address - 1
-        #dst_address = w.dst_address - 1
-        #remap_matrix = w.remap_matrix[:, 0]
-        #w_shape = (w.sizes["src_grid_size"], w.sizes["dst_grid_size"])
+        # src_address = w.src_address - 1
+        # dst_address = w.dst_address - 1
+        # remap_matrix = w.remap_matrix[:, 0]
+        # w_shape = (w.sizes["src_grid_size"], w.sizes["dst_grid_size"])
 
         dst_grid_shape = w.dst_grid_dims.values
         dst_grid_center_lat = w.dst_grid_center_lat.data.reshape(
             # dst_grid_shape[::-1], order="C"
             dst_grid_shape[::-1]
         )
         dst_grid_center_lon = w.dst_grid_center_lon.data.reshape(
             # dst_grid_shape[::-1], order="C"
             dst_grid_shape[::-1]
         )
 
         dst_mask = w.dst_grid_imask
-        #src_mask = w.src_grid_imask
+        # src_mask = w.src_grid_imask
 
         axis_scale = 180.0 / math.pi  # Weight lat/lon in radians
 
     # Dimension on which we can produce the interpolation
     if space_dims is None:
         space_dims = default_space_dims
-    
+
     if not any(x in source_data.dims for x in space_dims):
-        logging.error("None of dimensions on which we can interpolate is found in the DataArray. Does your DataArray include any of these?")
-        logging.error(space_dims)
+        loggy.error("None of dimensions on which we can interpolate is found in the DataArray. Does your DataArray include any of these?")
+        loggy.error(space_dims)
         sys.exit('Dimensions mismatch')
 
     # Find dimensions to keep
     nd = sum([(d not in space_dims) for d in source_data.dims])
 
     kept_shape = list(source_data.shape[0:nd])
     kept_dims = list(source_data.dims[0:nd])
-    logging.info('Dimension kept:')
-    logging.info(kept_dims)
+    loggy.info('Dimension kept: %s', kept_dims)
+    #loggy.info(kept_dims)
 
     if weights_matrix is None:
         weights_matrix = compute_weights_matrix(weights)
 
     # Remove the spatial axes, apply the weights, add the spatial axes back
     source_array = source_data.data
     if isinstance(source_array, dask.array.Array):
         source_array = dask.array.reshape(source_array, kept_shape + [-1])
     else:
         source_array = numpy.reshape(source_array, kept_shape + [-1])
 
-
     # Handle input mask
     dask.array.ma.set_fill_value(source_array, 1e20)
     source_array = dask.array.ma.fix_invalid(source_array)
     source_array = dask.array.ma.filled(source_array)
 
     target_dask = dask.array.tensordot(source_array, weights_matrix, axes=1)
 
@@ -224,14 +224,15 @@
         del target_da.attrs['CDI_grid_type']
 
     # Now rename to the original coordinate names
     # target_da = target_da.rename({"lat": source_lat.name, "lon": source_lon.name})
 
     return target_da
 
+
 class Regridder(object):
     """Set up the regridding operation
 
     Supply either both ``source_grid`` and ``dest_grid`` or just ``weights``.
 
     For large grids you may wish to pre-calculate the weights using
     ESMF_RegridWeightGen, if not supplied ``weights`` will be calculated from
@@ -240,72 +241,71 @@
     Weights may be pre-computed by an external program, or created using
     :func:`cdo_generate_weights` or :func:`esmf_generate_weights`
 
     Args:
         source_grid (:class:`coecms.grid.Grid` or :class:`xarray.DataArray`): Source grid / sample dataset
         target_grid (:class:`coecms.grid.Grid` or :class:`xarray.DataArray`): Target grid / sample dataset
         weights (:class:`xarray.Dataset`): Pre-computed interpolation weights
-        vert_coord (str): Name of the vertical coordinate. 
+        vert_coord (str): Name of the vertical coordinate.
                           If provided, 3D weights are generated (default: None)
         method (str): Method to use for interpolation (default: 'con')
         space_dims (list): list of dimensions to interpolate (default: None)
-        transpose (bool): transpose the output so that the vertical coordinate is 
+        transpose (bool): transpose the output so that the vertical coordinate is
                           just before other spatial coords (dafault: True)
     """
 
     def __init__(self, source_grid=None, target_grid=None, weights=None,
                  method='con', space_dims=None, vert_coord=None, transpose=True,
                  cdo='cdo'):
-        
+
         if (source_grid is None or target_grid is None) and (weights is None):
             raise ValueError(
                 "Either weights or source_grid/target_grid must be supplied"
             )
-        
+
         self.transpose = transpose
-    
+
         # Is there already a weights file?
         if weights is not None:
             if not isinstance(weights, xarray.Dataset):
                 self.weights = xarray.open_mfdataset(weights)
             else:
                 self.weights = weights
-            
+
             if not vert_coord:
-                self.vert_coord = find_vert_coord(self.weights)
+                self.vert_coord = find_vert_coords(self.weights)
             else:
                 self.vert_coord = vert_coord
         else:
 
             # Check if there is a vertical coordinate for 3d oceanic data
             if not vert_coord:
-                self.vert_coord = find_vert_coord(source_grid)
+                self.vert_coord = find_vert_coords(source_grid)
             else:
                 self.vert_coord = vert_coord
 
             # Generate the weights with CDO
             self.weights = cdo_generate_weights(source_grid, target_grid, method=method,
                                                 vert_coord=self.vert_coord, cdo=cdo)
 
         if self.vert_coord:
             self.weights_matrix = compute_weights_matrix3d(self.weights, self.vert_coord)
-        else: 
+        else:
             self.weights_matrix = compute_weights_matrix(self.weights)
 
         # this section is used to create a target mask initializing the CDO weights (both 2d and 3d)
         if "dst_grid_masked" in self.weights.variables:  # has a destination mask been precomputed?
             self.masked = self.weights.dst_grid_masked.data  # ok, let's use it
         else:
             # compute the destination mask now
             self.weights = mask_weights(self.weights, self.weights_matrix, self.vert_coord)
             self.masked = check_mask(self.weights, self.vert_coord)
 
         self.space_dims = space_dims
 
-
     def regrid(self, source_data):
         """Regrid ``source_data`` to match the target grid
 
         Args:
             source_data (:class:`xarray.DataArray` or xarray.Dataset): Source
             variable
 
@@ -318,26 +318,25 @@
 
             # apply the regridder on each DataArray
             out = source_data.map(self.regrid_array, keep_attrs=True)
 
             # clean from degenerated variables
             degen_vars = [var for var in out.data_vars if out[var].dims == ()]
             return out.drop_vars(degen_vars)
-        
+
         elif isinstance(source_data, xarray.DataArray):
 
             return self.regrid_array(source_data)
 
         else:
             sys.exit('The object provided is not a Xarray object!')
 
     def regrid_array(self, source_data):
-
         """Regridding selection through 2d and 3d arrays"""
-        
+
         if (self.vert_coord and self.vert_coord in source_data.coords):
             # if this is a 3D we specified the vertical coord and it has it
             return self.regrid3d(source_data)
         else:
             return self.regrid2d(source_data)
 
     def regrid3d(self, source_data):
@@ -348,22 +347,22 @@
             variable
 
         Returns:
             :class:`xarray.DataArray` with a regridded
             version of the source variable
         """
 
-        logging.info('3D DataArray access!')
+        loggy.debug('3D DataArray access: variable is %s', source_data.name)
 
         # CDO 2.2.0 fix
         if "numLinks" in self.weights.dims:
             links_dim = "numLinks"
         else:
             links_dim = "num_links"
-        
+
         # this is necessary to remove lev-bounds, temporary hack since they should
         # be treated in a smarter way
         if ("bnds" in source_data.name or "bounds" in source_data.name):
             return source_data
 
         data3d_list = []
         for lev in range(0, source_data.coords[self.vert_coord].values.size):
@@ -383,15 +382,15 @@
             # Make sure that the vertical dimension is just before the spatial ones
             if self.space_dims is None:
                 space_dims = default_space_dims
             else:
                 space_dims = self.space_dims
             dims = list(data3d.dims)
             index = min([i for i, s in enumerate(dims) if s in space_dims])
-            dimst= dims[1:index] + [dims[0]] + dims[index:]
+            dimst = dims[1:index] + [dims[0]] + dims[index:]
             data3d = data3d.transpose(*dimst)
 
             return data3d
         else:
             sys.exit('Cannot process this source data, are you sure it is an xarray?')
 
     def regrid2d(self, source_data):
@@ -401,15 +400,15 @@
             source_data (:class:`xarray.DataArray`): Source
             variable
 
         Returns:
             :class:`xarray.DataArray` with a regridded
             version of the source variable
         """
-        logging.info('2D DataArray access!')
+        loggy.debug('2D DataArray access: variables is %s', source_data.name)
         return apply_weights(
             source_data, self.weights, weights_matrix=self.weights_matrix,
             masked=self.masked, space_dims=self.space_dims
         )
 
 
 def regrid(source_data, target_grid=None, weights=None, vert_coord=None, transpose=True, cdo='cdo'):
@@ -419,29 +418,29 @@
     the function.
 
     To save the weights use :class:`Regridder`.
 
     Args:
         source_data (:class:`xarray.DataArray`): Source variable
         target_grid (:class:`coecms.grid.Grid` or :class:`xarray.DataArray`): Target grid / sample variable
-        vert_coord (str): Name of the vertical coordinate. 
+        vert_coord (str): Name of the vertical coordinate.
                           If provided, 3D weights are generated (default: None)
         weights (:class:`xarray.Dataset`): Pre-computed interpolation weights
         transpose (bool): If True, transpose the output so that the vertical
                           coordinate is just before the other spatial coordinates (default: True)
 
         cdo (path): path of cdo executable ["cdo"]
     Returns:
         :class:`xarray.DataArray` with a regridded version of the source variable
     """
 
-    regridder = Regridder(source_data, target_grid=target_grid, weights=weights, 
+    regridder = Regridder(source_data, target_grid=target_grid, weights=weights,
                           vert_coord=vert_coord, cdo=cdo, transpose=transpose)
     return regridder.regrid(source_data)
 
 
 # def combine_2d_to_3d(array_list, dim_name, dim_values):
 #     """
 #     Function to combine a list of 2D xarrays into a 3D one adding a vertical coordinate lev
 #     """
 #     new_array = [x.assign_coords({dim_name: d}) for x, d in zip(array_list, dim_values)]
-#     return xarray.concat(new_array, dim_name)
+#     return xarray.concat(new_array, dim_name)
```

### Comparing `smmregrid-0.0.1/smmregrid/weights.py` & `smmregrid-0.0.2/smmregrid/weights.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Weight calculation utilities"""
 
 import dask.array
 import sparse
+import logging
 
+loggy = logging.getLogger(__name__)
 
 def compute_weights_matrix3d(weights, vert_coord='lev'):
     """
     Convert the weights from CDO to a list of numpy arrays
     """
 
     # CDO 2.2.0 fix
@@ -18,51 +20,50 @@
     sparse_weights = []
     nvert = weights[vert_coord].values.size
     for i in range(0, nvert):
         w = weights.loc[{vert_coord: i}]
         nl = w.link_length.values
         w = w.isel(**{links_dim: slice(0, nl)})
         sparse_weights.append(compute_weights_matrix(w))
-    
+
     return sparse_weights
 
 
 def compute_weights_matrix(weights):
     """
     Convert the weights from CDO/ESMF to a numpy array
     """
     w = weights
-    #if w.title.startswith("ESMF"):
+    # if w.title.startswith("ESMF"):
     if "S" in w.variables:
         # ESMF style weights
         src_address = w.col - 1
         dst_address = w.row - 1
         remap_matrix = w.S
         w_shape = (w.sizes["n_a"], w.sizes["n_b"])
 
     else:
         # CDO style weights
         src_address = w.src_address - 1
         dst_address = w.dst_address - 1
         remap_matrix = w.remap_matrix[:, 0]
         w_shape = (w.sizes["src_grid_size"], w.sizes["dst_grid_size"])
-   
+
     # Create a sparse array from the weights
     sparse_weights_delayed = dask.delayed(sparse.COO)(
         [src_address.data, dst_address.data], remap_matrix.data, shape=w_shape
     )
     sparse_weights = dask.array.from_delayed(
         sparse_weights_delayed, shape=w_shape, dtype=remap_matrix.dtype
     )
 
     return sparse_weights
 
 
 def mask_tensordot(src_mask, weights_matrix):
-
     """Apply tensor dot product to source mask to return destination mask"""
 
     target_mask = dask.array.tensordot(src_mask, weights_matrix, axes=1)
     target_mask = dask.array.where(target_mask < 0.5, 0, 1)
     return target_mask
 
 
@@ -95,29 +96,29 @@
     else:
         check = wdst.mean()
         out = (check != 1).data
 
     return out
 
 
-def check_mask_old(weights, vert_coord=None):
-    """Old version: check if the target mask is empty or full and
-    return a bool to be passed to the regridder.
-    Handle the 3d case"""
-
-    if vert_coord is not None:
-        result = []
-        for nlev in range(len(weights[vert_coord])):
-            w = weights['dst_grid_imask'].loc[{vert_coord: nlev}]
-            v = w.sum()/len(w)
-            if v == 1:
-                result.append(False)
-            else:
-                result.append(True)
-        return result
-    else:
-        w = weights['dst_grid_imask']
-        v = w.sum()/len(w)
-        if v == 1:
-            return False
-        else:
-            return True
+# def check_mask_old(weights, vert_coord=None):
+#     """Old version: check if the target mask is empty or full and
+#     return a bool to be passed to the regridder.
+#     Handle the 3d case"""
+
+#     if vert_coord is not None:
+#         result = []
+#         for nlev in range(len(weights[vert_coord])):
+#             w = weights['dst_grid_imask'].loc[{vert_coord: nlev}]
+#             v = w.sum() / len(w)
+#             if v == 1:
+#                 result.append(False)
+#             else:
+#                 result.append(True)
+#         return result
+#     else:
+#         w = weights['dst_grid_imask']
+#         v = w.sum() / len(w)
+#         if v == 1:
+#             return False
+#         else:
+#             return True
```

### Comparing `smmregrid-0.0.1/smmregrid.egg-info/PKG-INFO` & `smmregrid-0.0.2/smmregrid.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: smmregrid
-Version: 0.0.1
+Version: 0.0.2
 Summary: Regridding based on sparse matrix multiplication
 Author-email: Jost von Hardenberg <jost.hardenberg@polito.it>, Paolo Davini <p.davini@isac.cnr.it>, Scott Wales <scott.wales@unimelb.edu.au>
 Project-URL: Homepage, https://github.com/jhardenberg/smmregrid
 Project-URL: Bug Tracker, https://github.com/jhardenberg/smmregrid/issues
-Project-URL: Repository, https://github.com/oloapinivad/ECmean4
+Project-URL: Repository, https://github.com/jhardenberg/smmregrid
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
+Provides-Extra: notebooks
 Provides-Extra: all
 License-File: LICENSE
 
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/jhardenberg/smmregrid/graphs/commit-activity)
 [![PyTest](https://github.com/jhardenberg/smmregrid/actions/workflows/mambatest.yml/badge.svg)](https://github.com/jhardenberg/smmregrid/actions/workflows/mambatest.yml)
 [![Coverage Status](https://coveralls.io/repos/github/jhardenberg/smmregrid/badge.svg?branch=main)](https://coveralls.io/github/jhardenberg/smmregrid?branch=main)
 [![PyPI version](https://badge.fury.io/py/smmregrid.svg)](https://badge.fury.io/py/smmregrid)
```

