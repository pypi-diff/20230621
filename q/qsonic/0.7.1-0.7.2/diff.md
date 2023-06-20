# Comparing `tmp/qsonic-0.7.1.tar.gz` & `tmp/qsonic-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsonic-0.7.1.tar", last modified: Sun Jun 18 01:03:31 2023, max compression
+gzip compressed data, was "qsonic-0.7.2.tar", last modified: Tue Jun 20 22:08:28 2023, max compression
```

## Comparing `qsonic-0.7.1.tar` & `qsonic-0.7.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:03:31.121441 qsonic-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-18 01:03:12.000000 qsonic-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-18 01:03:31.121441 qsonic-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-18 01:03:12.000000 qsonic-0.7.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:03:31.117441 qsonic-0.7.1/py/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:03:31.121441 qsonic-0.7.1/py/qsonic/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-18 01:03:12.000000 qsonic-0.7.1/py/qsonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-06-18 01:03:12.000000 qsonic-0.7.1/py/qsonic/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-06-18 01:03:12.000000 qsonic-0.7.1/py/qsonic/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    18264 2023-06-18 01:03:12.000000 qsonic-0.7.1/py/qsonic/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    13560 2023-06-18 01:03:12.000000 qsonic-0.7.1/py/qsonic/masks.py
--rw-r--r--   0 runner    (1001) docker     (123)    17279 2023-06-18 01:03:12.000000 qsonic-0.7.1/py/qsonic/mathtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-06-18 01:03:12.000000 qsonic-0.7.1/py/qsonic/mpi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    52012 2023-06-18 01:03:12.000000 qsonic-0.7.1/py/qsonic/picca_continuum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:03:31.121441 qsonic-0.7.1/py/qsonic/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-06-18 01:03:12.000000 qsonic-0.7.1/py/qsonic/scripts/qsonic_calib.py
--rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-06-18 01:03:12.000000 qsonic-0.7.1/py/qsonic/scripts/qsonic_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)    30001 2023-06-18 01:03:12.000000 qsonic-0.7.1/py/qsonic/spectrum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:03:31.121441 qsonic-0.7.1/py/qsonic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-18 01:03:31.000000 qsonic-0.7.1/py/qsonic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-18 01:03:31.000000 qsonic-0.7.1/py/qsonic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 01:03:31.000000 qsonic-0.7.1/py/qsonic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-18 01:03:31.000000 qsonic-0.7.1/py/qsonic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-18 01:03:31.000000 qsonic-0.7.1/py/qsonic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-18 01:03:31.000000 qsonic-0.7.1/py/qsonic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-18 01:03:12.000000 qsonic-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-18 01:03:12.000000 qsonic-0.7.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-18 01:03:31.121441 qsonic-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 01:03:12.000000 qsonic-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:03:31.121441 qsonic-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-18 01:03:12.000000 qsonic-0.7.1/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-06-18 01:03:12.000000 qsonic-0.7.1/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-18 01:03:12.000000 qsonic-0.7.1/tests/test_masks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-18 01:03:12.000000 qsonic-0.7.1/tests/test_mathtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-06-18 01:03:12.000000 qsonic-0.7.1/tests/test_mpi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-06-18 01:03:12.000000 qsonic-0.7.1/tests/test_picca_continuum.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-18 01:03:12.000000 qsonic-0.7.1/tests/test_qsonic_calib.py
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-18 01:03:12.000000 qsonic-0.7.1/tests/test_spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:08:28.300312 qsonic-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-20 22:08:04.000000 qsonic-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-20 22:08:28.300312 qsonic-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-20 22:08:04.000000 qsonic-0.7.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:08:28.296312 qsonic-0.7.2/py/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:08:28.296312 qsonic-0.7.2/py/qsonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-20 22:08:04.000000 qsonic-0.7.2/py/qsonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-06-20 22:08:04.000000 qsonic-0.7.2/py/qsonic/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-06-20 22:08:04.000000 qsonic-0.7.2/py/qsonic/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18264 2023-06-20 22:08:04.000000 qsonic-0.7.2/py/qsonic/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13560 2023-06-20 22:08:04.000000 qsonic-0.7.2/py/qsonic/masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17279 2023-06-20 22:08:04.000000 qsonic-0.7.2/py/qsonic/mathtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-06-20 22:08:04.000000 qsonic-0.7.2/py/qsonic/mpi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52579 2023-06-20 22:08:04.000000 qsonic-0.7.2/py/qsonic/picca_continuum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:08:28.296312 qsonic-0.7.2/py/qsonic/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-06-20 22:08:04.000000 qsonic-0.7.2/py/qsonic/scripts/qsonic_calib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-06-20 22:08:04.000000 qsonic-0.7.2/py/qsonic/scripts/qsonic_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29973 2023-06-20 22:08:04.000000 qsonic-0.7.2/py/qsonic/spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:08:28.296312 qsonic-0.7.2/py/qsonic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-20 22:08:28.000000 qsonic-0.7.2/py/qsonic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-20 22:08:28.000000 qsonic-0.7.2/py/qsonic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 22:08:28.000000 qsonic-0.7.2/py/qsonic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-20 22:08:28.000000 qsonic-0.7.2/py/qsonic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-20 22:08:28.000000 qsonic-0.7.2/py/qsonic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 22:08:28.000000 qsonic-0.7.2/py/qsonic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-20 22:08:04.000000 qsonic-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-20 22:08:04.000000 qsonic-0.7.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-20 22:08:28.300312 qsonic-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 22:08:04.000000 qsonic-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:08:28.300312 qsonic-0.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-20 22:08:04.000000 qsonic-0.7.2/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-06-20 22:08:04.000000 qsonic-0.7.2/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-20 22:08:04.000000 qsonic-0.7.2/tests/test_masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-20 22:08:04.000000 qsonic-0.7.2/tests/test_mathtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-06-20 22:08:04.000000 qsonic-0.7.2/tests/test_mpi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-06-20 22:08:04.000000 qsonic-0.7.2/tests/test_picca_continuum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-20 22:08:04.000000 qsonic-0.7.2/tests/test_qsonic_calib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-20 22:08:04.000000 qsonic-0.7.2/tests/test_spectrum.py
```

### Comparing `qsonic-0.7.1/LICENSE` & `qsonic-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.1/PKG-INFO` & `qsonic-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsonic
-Version: 0.7.1
+Version: 0.7.2
 Summary: Quasar continuum fitter for DESI
 Author: Naim Goksel Karacayli
 Author-email: ngokselk@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/p-slash/qsonic/issues
 Project-URL: Documentation, http://qsonic.readthedocs.io/
 Project-URL: Source, https://github.com/p-slash/qsonic
@@ -31,15 +31,15 @@
     :target: https://qsonic.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 **QSOnic** is an MPI-parallelized, highly optimized quasar continuum fitting package for DESI built on the same algorithm as `picca <https://github.com/igmhub/picca>`_, but *faster*. It also provides an efficient API to read DESI quasar spectra.
 
 The key differences
 -------------------
-- Coadding of spectrograph arms is optional and performed after continuum fitting.
+- Coadding of spectrograph arms can be performed after continuum fitting or disabled entirely.
 - Continuum is multiplied by a fiducial mean flux when provided.
 - You can pass fiducial var_lss (column **VAR_LSS**) and mean flux (column **MEANFLUX**) for observed wavelength **LAMBDA** in **STATS** extention of a FITS file. Wavelength should be linearly and equally spaced. This is the same format as rawio output from picca, except **VAR** column in picca is the variance on flux not deltas. We break away from that convention by explicitly requiring variance on deltas in a new column.
 - If no fiducial is passed, we fit only for var_lss (no eta fitting by default). Eta fitting can be enabled, but is not recommended for Lya forest.
 - Internal weights for continuum fitting and coadding are based on smoothed ``IVAR``, and output ``WEIGHT`` is based on this smoothed ivar. This smoothing can be turned off.
 - Chi2 information as well as best fits are saved in continuum_chi2_catalog.fits. Chi2 is calculated using smooth ivar and var_lss, and does not subtract sum of ln(weights).
 
 Similarities
```

### Comparing `qsonic-0.7.1/README.rst` & `qsonic-0.7.2/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     :target: https://qsonic.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 **QSOnic** is an MPI-parallelized, highly optimized quasar continuum fitting package for DESI built on the same algorithm as `picca <https://github.com/igmhub/picca>`_, but *faster*. It also provides an efficient API to read DESI quasar spectra.
 
 The key differences
 -------------------
-- Coadding of spectrograph arms is optional and performed after continuum fitting.
+- Coadding of spectrograph arms can be performed after continuum fitting or disabled entirely.
 - Continuum is multiplied by a fiducial mean flux when provided.
 - You can pass fiducial var_lss (column **VAR_LSS**) and mean flux (column **MEANFLUX**) for observed wavelength **LAMBDA** in **STATS** extention of a FITS file. Wavelength should be linearly and equally spaced. This is the same format as rawio output from picca, except **VAR** column in picca is the variance on flux not deltas. We break away from that convention by explicitly requiring variance on deltas in a new column.
 - If no fiducial is passed, we fit only for var_lss (no eta fitting by default). Eta fitting can be enabled, but is not recommended for Lya forest.
 - Internal weights for continuum fitting and coadding are based on smoothed ``IVAR``, and output ``WEIGHT`` is based on this smoothed ivar. This smoothing can be turned off.
 - Chi2 information as well as best fits are saved in continuum_chi2_catalog.fits. Chi2 is calculated using smooth ivar and var_lss, and does not subtract sum of ln(weights).
 
 Similarities
```

### Comparing `qsonic-0.7.1/py/qsonic/calibration.py` & `qsonic-0.7.2/py/qsonic/calibration.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.1/py/qsonic/catalog.py` & `qsonic-0.7.2/py/qsonic/catalog.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.1/py/qsonic/io.py` & `qsonic-0.7.2/py/qsonic/io.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.1/py/qsonic/masks.py` & `qsonic-0.7.2/py/qsonic/masks.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.1/py/qsonic/mathtools.py` & `qsonic-0.7.2/py/qsonic/mathtools.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.1/py/qsonic/mpi_utils.py` & `qsonic-0.7.2/py/qsonic/mpi_utils.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.1/py/qsonic/picca_continuum.py` & `qsonic-0.7.2/py/qsonic/picca_continuum.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,18 @@
         "--var-fit-eta", action="store_true",
         help="Fit for noise calibration (eta).")
     cont_group.add_argument(
         "--var-use-cov", action="store_true",
         help="Use covariance in varlss-eta fitting.")
     cont_group.add_argument(
         "--normalize-stacked-flux", action="store_true",
-        help="NOT IMPLEMENTED: Force stacked flux to be one at the end.")
+        help=("Force stacked flux to be one at the end."
+              "Note this does not change STACKED_FLUX in attributes. "
+              "It only updates CONT of each delta.")
+    )
     cont_group.add_argument(
         "--rfdwave", type=float, default=0.8,
         help="Rest-frame wave steps. Complies with forest limits")
     cont_group.add_argument(
         "--minimizer", default="iminuit", choices=["iminuit", "l_bfgs_b"],
         help="Minimizer to fit the continuum.")
 
@@ -121,14 +124,16 @@
         Number of iterations from ``args.num_iterations``.
     cont_order: int
         Order of continuum polynomial from ``args.cont_order``.
     outdir: str or None
         Directory to save catalogs. If None or empty, does not save.
     fit_eta: bool
         True if fitting eta and fiducial var_lss is not set.
+    normalize_stacked_flux: bool
+        Normalizes observed flux to be 1 if True.
     """
 
     def _get_fiducial_interp(self, fname, col2read):
         """ Return an interpolator for mean flux or var_lss.
 
         FITS file must have a **STATS** extention, which must have **LAMBDA**,
         **MEANFLUX** and **VAR_LSS** columns. This is the same format as rawio
@@ -232,14 +237,15 @@
             np.ones_like(self.varlss_interp.fp),
             ep=np.zeros_like(self.varlss_interp.fp))
 
         self.niterations = args.num_iterations
         self.cont_order = args.cont_order
         self.outdir = args.outdir
         self.fit_eta = args.var_fit_eta
+        self.normalize_stacked_flux = args.normalize_stacked_flux
 
     def _continuum_costfn(self, x, wave, flux, ivar_sm, z_qso):
         """ Cost function to minimize for each quasar.
 
         This is a modified chi2 where amplitude is also part of minimization.
         Cost of each arm is simply added to the total cost.
 
@@ -477,32 +483,29 @@
 
         # normalize
         mean = np.trapz(new_meancont, x=x)
         new_meancont /= mean
 
         return new_meancont, mean
 
-    def update_mean_cont(self, spectra_list, noupdate):
+    def update_mean_cont(self, spectra_list):
         """ Update the global mean continuum and stacked flux.
 
         Uses :attr:`forestivar_sm <qsonic.spectrum.Spectrum.forestivar_sm>`
         in inverse variance, but must be set beforehand.
         Raw mean continuum estimates are smoothed with a weighted
         :external+scipy:py:class:`scipy.interpolate.UnivariateSpline`. The mean
         continuum is removed from higher Legendre polynomials and normalized by
         the mean. This function updates
-        :attr:`meancont_interp.fp <.meancont_interp>` if noupdate is False.
+        :attr:`meancont_interp.fp <.meancont_interp>`.
 
         Arguments
         ---------
         spectra_list: list(Spectrum)
             Spectrum objects to fit.
-        noupdate: bool
-            Does not update :attr:`meancont_interp.fp <.meancont_interp>` if
-            True (last iteration).
 
         Returns
         ---------
         has_converged: bool
             True if all continuum updates on every point are less than 0.33
             times the error estimates.
         """
@@ -552,16 +555,15 @@
 
         # remove tilt and higher orders and normalize
         new_meancont, mean_ = self._project_normalize_meancont(new_meancont)
 
         norm_flux = new_meancont / self.meancont_interp.fp - 1
         std_flux /= mean_
 
-        if not noupdate:
-            self.meancont_interp.reset(new_meancont, ep=std_flux)
+        self.meancont_interp.reset(new_meancont, ep=std_flux)
 
         all_pt_test = np.all(np.abs(norm_flux) < 0.33 * std_flux)
         chi2_change = np.sum((norm_flux / std_flux)**2) / self.nbins
         has_converged = (chi2_change < 1e-3) | all_pt_test
 
         if self.mpi_rank != 0:
             return has_converged
@@ -573,24 +575,22 @@
             text += f"{w:7.2f}\t| {n:7.2e}\t| +- {e:7.2e}\n"
 
         text += f"Change in chi2: {chi2_change*100:.4e}%"
         logging_mpi(text, 0)
 
         return has_converged
 
-    def update_var_lss_eta(self, spectra_list, noupdate):
+    def update_var_lss_eta(self, spectra_list):
         """ Fit and update var_lss and eta if enabled. See
         :class:`VarLSSFitter` for fitting details.
 
         Arguments
         ---------
         spectra_list: list(Spectrum)
             Spectrum objects to fit.
-        noupdate: bool
-            Does not update `self.varlss_interp.fp` if True (last iteration).
         """
         if self.varlss_fitter is None:
             return
 
         self.varlss_fitter.reset()
 
         for spec in valid_spectra(spectra_list):
@@ -609,17 +609,17 @@
         else:
             text = "Fitting var_lss"
             initial_guess = self.varlss_interp.fp
 
         logging_mpi(text, self.mpi_rank)
         y, ep = self.varlss_fitter.fit(initial_guess)
 
-        if not noupdate and not self.fit_eta:
+        if not self.fit_eta:
             self.varlss_interp.reset(y, ep=ep)
-        if not noupdate and self.fit_eta:
+        else:
             self.varlss_interp.reset(y[:, 0], ep=ep[:, 0])
             self.eta_interp.reset(y[:, 1], ep=ep[:, 1])
 
         if self.mpi_rank != 0:
             return
 
         step = max(1, self.varlss_fitter.nwbins // 10)
@@ -633,14 +633,33 @@
             n = self.eta_interp.fp[i]
             ne = self.eta_interp.ep[i]
             text += \
                 f"{w:7.2f}\t| {v:7.2e} +- {ve:7.2e}\t| {n:7.2e} +- {ne:7.2e}\n"
         text += "------------------------------"
         logging_mpi(text, 0)
 
+    def _normalize_flux(self, spectra_list):
+        """Multiplies continuum estimates with stacked values in order to
+        normalize flux in the observed grid to be 1 if
+        ``--normalize-stacked-flux`` is passed.
+
+        Arguments
+        ---------
+        spectra_list: list(Spectrum)
+            Spectrum objects.
+        """
+        if not self.normalize_stacked_flux:
+            return
+
+        logging_mpi("Forcing stacked flux to be one.", self.mpi_rank)
+
+        for spec in valid_spectra(spectra_list):
+            for arm, wave_arm in spec.forestwave.items():
+                spec.cont_params['cont'][arm] *= self.flux_stacker(wave_arm)
+
     def iterate(self, spectra_list):
         """Main function to fit continua and iterate.
 
         Consists of three major steps: initializing, fitting, updating global
         variables. The initialization sets ``cont_params`` variable of every
         Spectrum object. Continuum polynomial order is carried by setting
         ``cont_params[x]``. At each iteration:
@@ -669,35 +688,36 @@
             spec.cont_params['dof'] = \
                 spec.get_real_size() - self.cont_order - 1
 
         fname = f"{self.outdir}/attributes.fits" if self.outdir else ""
         fattr = MPISaver(fname, self.mpi_rank)
 
         for it in range(self.niterations):
-            is_last_it = it == self.niterations - 1
             logging_mpi(
                 f"Fitting iteration {it+1}/{self.niterations}", self.mpi_rank)
 
             self.save(fattr, f"-{it + 1}")
 
             # Fit all continua one by one
             self.fit_continua(spectra_list)
             # Stack all spectra in each process
             # Broadcast and recalculate global functions
-            has_converged = self.update_mean_cont(spectra_list, is_last_it)
+            has_converged = self.update_mean_cont(spectra_list)
 
-            self.update_var_lss_eta(spectra_list, is_last_it)
+            self.update_var_lss_eta(spectra_list)
 
             if has_converged:
                 logging_mpi("Iteration has converged.", self.mpi_rank)
                 break
 
         if not has_converged:
             warn_mpi("Iteration has NOT converged.", self.mpi_rank)
 
+        self._normalize_flux(spectra_list)
+
         self.save(fattr)
         if self.varlss_fitter:
             self.varlss_fitter.write(fattr)
         fattr.close()
         logging_mpi("All continua are fit.", self.mpi_rank)
 
     def true_continuum(self, spectra_list):
@@ -733,16 +753,18 @@
                 cont_est = tcont_interp(wave_arm)
                 cont_est *= self.meanflux_interp(wave_arm)
                 spec.cont_params['cont'][arm] = cont_est
 
             spec.set_forest_weight(self.varlss_interp)
             spec.calc_continuum_chi2()
 
-        self.update_mean_cont(spectra_list, False)
-        self.update_var_lss_eta(spectra_list, False)
+        self.update_mean_cont(spectra_list)
+        self.update_var_lss_eta(spectra_list)
+        self._normalize_flux(spectra_list)
+
         fname = f"{self.outdir}/attributes.fits" if self.outdir else ""
         fattr = MPISaver(fname, self.mpi_rank)
         self.save(fattr)
         if self.varlss_fitter:
             self.varlss_fitter.write(fattr)
         fattr.close()
```

### Comparing `qsonic-0.7.1/py/qsonic/scripts/qsonic_calib.py` & `qsonic-0.7.2/py/qsonic/scripts/qsonic_calib.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.1/py/qsonic/scripts/qsonic_fit.py` & `qsonic-0.7.2/py/qsonic/scripts/qsonic_fit.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.1/py/qsonic/spectrum.py` & `qsonic-0.7.2/py/qsonic/spectrum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import argparse
 
 import numpy as np
 
-from qsonic import QsonicException
 from qsonic.mathtools import _zero_function, _one_function, get_smooth_ivar
 
 
 def add_wave_region_parser(parser=None):
     """ Adds wavelength analysis related arguments to parser. These
     arguments are grouped under 'Wavelength analysis region'. All of them
     come with defaults, none are required.
@@ -366,17 +365,18 @@
 
         return size
 
     def is_long(self, dforest_wave, skip_ratio):
         """Determine if spectrum is long enough to be accepted.
 
         The condition is :meth:`get_real_size` > ``skip_ratio * npixels``,
-        where ``npixels`` :math:`=(1 + z_\\mathrm{qso}) \\times` ``dforest_wave``
-        :math:`/ \\mathrm{d}\\lambda` and :math:`\\mathrm{d}\\lambda` is
-        wavelength spacing in the observed frame in A. 
+        where ``npixels`` :math:`=(1 + z_\\mathrm{qso}) \\times`
+        ``dforest_wave`` :math:`/ \\mathrm{d}\\lambda` and
+        :math:`\\mathrm{d}\\lambda` is wavelength spacing in the observed frame
+        in A.
 
         Arguments
         ---------
         dforest_wave: float
             Length of the forest in the rest-frame in A.
         skip_ratio: float
             Minimum ratio that needs to be present and unmasked to keep the
```

### Comparing `qsonic-0.7.1/py/qsonic.egg-info/PKG-INFO` & `qsonic-0.7.2/py/qsonic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsonic
-Version: 0.7.1
+Version: 0.7.2
 Summary: Quasar continuum fitter for DESI
 Author: Naim Goksel Karacayli
 Author-email: ngokselk@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/p-slash/qsonic/issues
 Project-URL: Documentation, http://qsonic.readthedocs.io/
 Project-URL: Source, https://github.com/p-slash/qsonic
@@ -31,15 +31,15 @@
     :target: https://qsonic.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 **QSOnic** is an MPI-parallelized, highly optimized quasar continuum fitting package for DESI built on the same algorithm as `picca <https://github.com/igmhub/picca>`_, but *faster*. It also provides an efficient API to read DESI quasar spectra.
 
 The key differences
 -------------------
-- Coadding of spectrograph arms is optional and performed after continuum fitting.
+- Coadding of spectrograph arms can be performed after continuum fitting or disabled entirely.
 - Continuum is multiplied by a fiducial mean flux when provided.
 - You can pass fiducial var_lss (column **VAR_LSS**) and mean flux (column **MEANFLUX**) for observed wavelength **LAMBDA** in **STATS** extention of a FITS file. Wavelength should be linearly and equally spaced. This is the same format as rawio output from picca, except **VAR** column in picca is the variance on flux not deltas. We break away from that convention by explicitly requiring variance on deltas in a new column.
 - If no fiducial is passed, we fit only for var_lss (no eta fitting by default). Eta fitting can be enabled, but is not recommended for Lya forest.
 - Internal weights for continuum fitting and coadding are based on smoothed ``IVAR``, and output ``WEIGHT`` is based on this smoothed ivar. This smoothing can be turned off.
 - Chi2 information as well as best fits are saved in continuum_chi2_catalog.fits. Chi2 is calculated using smooth ivar and var_lss, and does not subtract sum of ln(weights).
 
 Similarities
```

### Comparing `qsonic-0.7.1/py/qsonic.egg-info/SOURCES.txt` & `qsonic-0.7.2/py/qsonic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.1/setup.cfg` & `qsonic-0.7.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.7.1
+current_version = 0.7.2
 commit = True
 tag = True
 
 [bumpversion:file:py/qsonic/__init__.py]
 search = __version__ = '{current_version}'
 replace = __version__ = '{new_version}'
```

### Comparing `qsonic-0.7.1/tests/test_catalog.py` & `qsonic-0.7.2/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.1/tests/test_io.py` & `qsonic-0.7.2/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.1/tests/test_masks.py` & `qsonic-0.7.2/tests/test_masks.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.1/tests/test_mathtools.py` & `qsonic-0.7.2/tests/test_mathtools.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.1/tests/test_mpi_utils.py` & `qsonic-0.7.2/tests/test_mpi_utils.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.1/tests/test_picca_continuum.py` & `qsonic-0.7.2/tests/test_picca_continuum.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,15 @@
             spec.set_forest_region(
                 3600., 6000., args.forest_w1, args.forest_w2)
             spec.cont_params['valid'] = True
             spec.cont_params['cont'] = {}
             for arm, wave_arm in spec.forestwave.items():
                 spec.cont_params['cont'][arm] = np.ones_like(wave_arm)
 
-        qcfit.update_mean_cont(spectra_list, False)
+        qcfit.update_mean_cont(spectra_list)
         npt.assert_allclose(qcfit.meancont_interp.fp, 1, rtol=1e-3)
         npt.assert_almost_equal(qcfit.meancont_interp.fp.mean(), 1)
 
 
 class TestVarLSSFitter(object):
     def test_add(self, setup_data):
         nwbins = 4
```

### Comparing `qsonic-0.7.1/tests/test_qsonic_calib.py` & `qsonic-0.7.2/tests/test_qsonic_calib.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.1/tests/test_spectrum.py` & `qsonic-0.7.2/tests/test_spectrum.py`

 * *Files identical despite different names*

