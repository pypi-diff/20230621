# Comparing `tmp/pyspk-1.5.tar.gz` & `tmp/pyspk-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspk-1.5.tar", last modified: Fri Jun  9 17:01:36 2023, max compression
+gzip compressed data, was "pyspk-1.6.tar", last modified: Wed Jun 21 12:49:58 2023, max compression
```

## Comparing `pyspk-1.5.tar` & `pyspk-1.6.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-06-09 17:01:36.912228 pyspk-1.5/
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     7326 2023-06-09 16:28:12.000000 pyspk-1.5/LICENSE.md
--rw-r--r--   0 jaimesalcido   (501) staff       (20)       25 2023-06-09 16:28:12.000000 pyspk-1.5/MANIFEST.in
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     9188 2023-06-09 17:01:36.912026 pyspk-1.5/PKG-INFO
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     8667 2023-06-09 16:28:12.000000 pyspk-1.5/README.md
-drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-06-09 17:01:36.910767 pyspk-1.5/pyspk/
--rw-r--r--   0 jaimesalcido   (501) staff       (20)       20 2023-06-09 16:28:12.000000 pyspk-1.5/pyspk/__init__.py
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     4114 2023-06-09 16:28:12.000000 pyspk-1.5/pyspk/fit_vals.py
--rw-r--r--   0 jaimesalcido   (501) staff       (20)    16276 2023-06-09 16:47:49.000000 pyspk-1.5/pyspk/model.py
--rw-r--r--   0 jaimesalcido   (501) staff       (20)   180588 2023-06-09 16:28:12.000000 pyspk-1.5/pyspk/stat_errors_200.csv
--rw-r--r--   0 jaimesalcido   (501) staff       (20)   179036 2023-06-09 16:28:12.000000 pyspk-1.5/pyspk/stat_errors_500.csv
-drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-06-09 17:01:36.911880 pyspk-1.5/pyspk.egg-info/
--rw-r--r--   0 jaimesalcido   (501) staff       (20)     9188 2023-06-09 17:01:36.000000 pyspk-1.5/pyspk.egg-info/PKG-INFO
--rw-r--r--   0 jaimesalcido   (501) staff       (20)      288 2023-06-09 17:01:36.000000 pyspk-1.5/pyspk.egg-info/SOURCES.txt
--rw-r--r--   0 jaimesalcido   (501) staff       (20)        1 2023-06-09 17:01:36.000000 pyspk-1.5/pyspk.egg-info/dependency_links.txt
--rw-r--r--   0 jaimesalcido   (501) staff       (20)       12 2023-06-09 17:01:36.000000 pyspk-1.5/pyspk.egg-info/requires.txt
--rw-r--r--   0 jaimesalcido   (501) staff       (20)        6 2023-06-09 17:01:36.000000 pyspk-1.5/pyspk.egg-info/top_level.txt
--rw-r--r--   0 jaimesalcido   (501) staff       (20)       38 2023-06-09 17:01:36.912266 pyspk-1.5/setup.cfg
--rw-r--r--   0 jaimesalcido   (501) staff       (20)      807 2023-06-09 17:01:19.000000 pyspk-1.5/setup.py
+drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-06-21 12:49:58.363867 pyspk-1.6/
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)     7326 2023-06-09 16:28:12.000000 pyspk-1.6/LICENSE.md
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)       25 2023-06-09 16:28:12.000000 pyspk-1.6/MANIFEST.in
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)     9188 2023-06-21 12:49:58.363703 pyspk-1.6/PKG-INFO
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)     8667 2023-06-09 16:28:12.000000 pyspk-1.6/README.md
+drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-06-21 12:49:58.361849 pyspk-1.6/pyspk/
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)       20 2023-06-09 16:28:12.000000 pyspk-1.6/pyspk/__init__.py
+drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-06-21 12:49:58.363451 pyspk-1.6/pyspk/__pycache__/
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)      156 2023-06-21 11:12:32.000000 pyspk-1.6/pyspk/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)     2169 2023-06-21 11:12:32.000000 pyspk-1.6/pyspk/__pycache__/fit_vals.cpython-38.pyc
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)    14959 2023-06-21 11:12:32.000000 pyspk-1.6/pyspk/__pycache__/model.cpython-38.pyc
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)     4114 2023-06-09 16:28:12.000000 pyspk-1.6/pyspk/fit_vals.py
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)    16579 2023-06-21 11:54:52.000000 pyspk-1.6/pyspk/model.py
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)   180588 2023-06-09 16:28:12.000000 pyspk-1.6/pyspk/stat_errors_200.csv
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)   179036 2023-06-09 16:28:12.000000 pyspk-1.6/pyspk/stat_errors_500.csv
+drwxr-xr-x   0 jaimesalcido   (501) staff       (20)        0 2023-06-21 12:49:58.362954 pyspk-1.6/pyspk.egg-info/
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)     9188 2023-06-21 12:49:58.000000 pyspk-1.6/pyspk.egg-info/PKG-INFO
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)      411 2023-06-21 12:49:58.000000 pyspk-1.6/pyspk.egg-info/SOURCES.txt
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)        1 2023-06-21 12:49:58.000000 pyspk-1.6/pyspk.egg-info/dependency_links.txt
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)       12 2023-06-21 12:49:58.000000 pyspk-1.6/pyspk.egg-info/requires.txt
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)        6 2023-06-21 12:49:58.000000 pyspk-1.6/pyspk.egg-info/top_level.txt
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)       38 2023-06-21 12:49:58.363903 pyspk-1.6/setup.cfg
+-rw-r--r--   0 jaimesalcido   (501) staff       (20)      807 2023-06-21 12:46:36.000000 pyspk-1.6/setup.py
```

### Comparing `pyspk-1.5/LICENSE.md` & `pyspk-1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyspk-1.5/PKG-INFO` & `pyspk-1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspk
-Version: 1.5
+Version: 1.6
 Summary: Python package to predict the suppression of the total matter power spectrum due to baryonic physics
 Home-page: https://github.com/jemme07/pyspk
 Author: Jaime Salcido
 Author-email: j.salcidonegrete@ljmu.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `pyspk-1.5/README.md` & `pyspk-1.6/README.md`

 * *Files identical despite different names*

### Comparing `pyspk-1.5/pyspk/fit_vals.py` & `pyspk-1.6/pyspk/fit_vals.py`

 * *Files identical despite different names*

### Comparing `pyspk-1.5/pyspk/model.py` & `pyspk-1.6/pyspk/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,15 +266,15 @@
     C = _np.power(m_halo / 1e14, beta - 1)
     D = _np.power(cosmo.efunc(z) / cosmo.efunc(0.3), gamma)
 
     return A * B * C * D
 
 
 def sup_model(SO, z, fb_a=None, fb_pow=None, fb_pivot=1, M_halo=None, fb=None, extrapolate=False,
-              alpha=None, beta=None, gamma=None, cosmo=None, k_min=0.1, k_max=8, n=100, 
+              alpha=None, beta=None, gamma=None, cosmo=None, k_array=None, k_min=0.1, k_max=8, n=100, 
               errors=False, verbose=False):
     """
     Returns the suppression of the total matter power spectrum as a function of scale 'k' using the SP(k) model.
     Automatically selects the required optimal mass as a function of scale and redshift. Requires the baryon 
     fraction - halo mass relation, either by specifying power-law fitting parameters, or non-parametric 
     proving arrays with fb and M_halo at a specific redshift. The function accepts a simple power law form 
     or an Akino et al 2022 fucntional form. If a non-parametric relation is given, an 
@@ -304,14 +304,16 @@
         sets the Akino power law constant
     beta : float, optional
         sets the Akino power law exponent
     gamma : float, optional
         sets the Akino power law redshift dependence. 
     cosmo: astropy cosmology object, optional
         astropy cosmology object with the desired cosmology
+    k_array : array of float, optional
+        array containing the desired co-moving wavenumber in units [h/Mpc]. If given, k_min, k_max and n are ignored.
     k_min : float, default 0.1
         minimum co-moving wavenumber in units [h/Mpc]
     k_max : float, default 8, max 12
         maximum co-moving wavenumber in units [h/Mpc]. Default is set to the Nyquist frequency of the Antilles
         simulations (see Salcido et al. 2023). 
     n : int, default 100
         number of equally spaced co-moving wavenumber in log-spaced between k_min and k_max.
@@ -338,40 +340,51 @@
     Notes
     ----------
     The maximum co-moving wavenumber in units [h/Mpc] is set to the Nyquist frequency of the Antilles simulations 
     (see Salcido et al. 2023). Although SP(k) was fitted up to k = 12 [h/Mpc], we caution the user that setting 
     𝑘 > 𝑘Ny (8 [h/Mpc]) might not be representative of the true uncertainties in the data. 
     """
 
+
     if z < 0:
         raise Exception('\033[91mIncorrect redshift.\033[0m') from None
         
     if z > 3:
         raise Exception('\033[91mpy-spk was calibrated up to z = 3.0. '
                         'Please specify z <= 3.0 \033[0m') from None
 
     if z < 0.125:
         _warnings.warn('\033[33mpy-spk was calibrated down to z = 0.125. Redshifts '
                        'z < 0.125 may not be accurately reproduced by the model. \033[0m', stacklevel=2)
 
+    if cosmo is not None:
+        if not cosmo.Ob0:
+            raise Exception('\033[91mIncorrect cosmology. Please specify Omega_baryon.\033[0m') from None
+
+
+    if k_array is not None:
+        k_max = k_array.max()
+        k_min = k_array.min()
+        k = k_array
+
+    else:
+        k = _np.round(_np.logspace(_np.log10(k_min), _np.log10(k_max), n), 6)
+    
+    logk = _np.log10(k)
+
     if k_max > 12:
         raise Exception('\033[91mpy-spk was calibrated up to k_max = 12 [h/Mpc] '
                         'Please specify k_max <= 12 [h/Mpc] \033[0m') from None
         
     if k_max > 8:
         _warnings.warn('\033[33mScales with k_max > k_ny = 8 [h/Mpc] '
                        'may not be accurately reproduced by the model. \033[0m', stacklevel=2)
 
-    if cosmo is not None:
-        if not cosmo.Ob0:
-            raise Exception('\033[91mIncorrect cosmology. Please specify Omega_baryon.\033[0m') from None
 
     params = _get_params(SO, z)
-    k = _np.round(_np.logspace(_np.log10(k_min), _np.log10(k_max), n), 6)
-    logk = _np.log10(k)
 
     best_mass = _optimal_mass_funct(k, params)
 
     if (fb_a is not None) or (fb_pow is not None):
         if verbose:
             print('\033[36mUsing power-law fit for fb - M_halo at z=%.3f, ' 
                   'normalised at M_halo = %.2e [M_sun] \033[0m' % (z, fb_pivot))
```

### Comparing `pyspk-1.5/pyspk/stat_errors_200.csv` & `pyspk-1.6/pyspk/stat_errors_200.csv`

 * *Files identical despite different names*

### Comparing `pyspk-1.5/pyspk/stat_errors_500.csv` & `pyspk-1.6/pyspk/stat_errors_500.csv`

 * *Files identical despite different names*

### Comparing `pyspk-1.5/pyspk.egg-info/PKG-INFO` & `pyspk-1.6/pyspk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspk
-Version: 1.5
+Version: 1.6
 Summary: Python package to predict the suppression of the total matter power spectrum due to baryonic physics
 Home-page: https://github.com/jemme07/pyspk
 Author: Jaime Salcido
 Author-email: j.salcidonegrete@ljmu.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `pyspk-1.5/setup.py` & `pyspk-1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     print(long_description)
 
 setuptools.setup(
     name="pyspk",
-    version=1.5,
+    version=1.6,
     description="Python package to predict the suppression of the total matter power spectrum due to baryonic physics",
     url="https://github.com/jemme07/pyspk",
     author="Jaime Salcido",
     author_email="j.salcidonegrete@ljmu.ac.uk",
     packages=['pyspk'],
     long_description=long_description,
     long_description_content_type="text/markdown",
```

