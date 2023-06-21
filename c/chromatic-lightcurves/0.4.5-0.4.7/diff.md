# Comparing `tmp/chromatic-lightcurves-0.4.5.tar.gz` & `tmp/chromatic-lightcurves-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromatic-lightcurves-0.4.5.tar", last modified: Wed Nov 16 23:53:41 2022, max compression
+gzip compressed data, was "chromatic-lightcurves-0.4.7.tar", last modified: Wed Jun 21 14:35:11 2023, max compression
```

## Comparing `chromatic-lightcurves-0.4.5.tar` & `chromatic-lightcurves-0.4.7.tar`

### file list

```diff
@@ -1,200 +1,204 @@
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2022-11-16 23:53:41.151028 chromatic-lightcurves-0.4.5/
--rwxr-xr-x   0 zach       (502) staff       (20)     2226 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/.gitignore
--rwxr-xr-x   0 zach       (502) staff       (20)      329 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/.pre-commit-config.yaml
--rwxr-xr-x   0 zach       (502) staff       (20)     1076 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/LICENSE
--rw-r--r--   0 zach       (502) staff       (20)      641 2022-11-16 23:53:41.150834 chromatic-lightcurves-0.4.5/PKG-INFO
--rwxr-xr-x   0 zach       (502) staff       (20)     2776 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/README.md
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2022-11-16 23:53:41.051174 chromatic-lightcurves-0.4.5/chromatic/
--rwxr-xr-x   0 zach       (502) staff       (20)      119 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/__init__.py
--rwxr-xr-x   0 zach       (502) staff       (20)     5005 2022-11-08 03:57:51.000000 chromatic-lightcurves-0.4.5/chromatic/imports.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2022-11-16 23:53:41.055345 chromatic-lightcurves-0.4.5/chromatic/rainbows/
--rwxr-xr-x   0 zach       (502) staff       (20)      890 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/__init__.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2022-11-16 23:53:41.067623 chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/
--rwxr-xr-x   0 zach       (502) staff       (20)      444 2022-10-07 04:08:11.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/__init__.py
--rwxr-xr-x   0 zach       (502) staff       (20)     8191 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/align_wavelengths.py
--rwxr-xr-x   0 zach       (502) staff       (20)     1955 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/attach_model.py
--rwxr-xr-x   0 zach       (502) staff       (20)    27690 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/binning.py
--rwxr-xr-x   0 zach       (502) staff       (20)      832 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/compare.py
--rwxr-xr-x   0 zach       (502) staff       (20)     1336 2022-10-10 12:57:27.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/descriptions.txt
--rwxr-xr-x   0 zach       (502) staff       (20)     3542 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/flag_outliers.py
--rwxr-xr-x   0 zach       (502) staff       (20)     3399 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/fold.py
--rwxr-xr-x   0 zach       (502) staff       (20)     3414 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/inflate_uncertainty.py
--rwxr-xr-x   0 zach       (502) staff       (20)     3856 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/inject_noise.py
--rw-r--r--   0 zach       (502) staff       (20)     1699 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/inject_outliers.py
--rwxr-xr-x   0 zach       (502) staff       (20)     2612 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/inject_spectrum.py
--rwxr-xr-x   0 zach       (502) staff       (20)    10376 2022-11-08 03:57:51.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/inject_systematics.py
--rwxr-xr-x   0 zach       (502) staff       (20)    18525 2022-11-15 00:30:54.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/inject_transit.py
--rwxr-xr-x   0 zach       (502) staff       (20)     3653 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/normalization.py
--rwxr-xr-x   0 zach       (502) staff       (20)    11422 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/operations.py
--rwxr-xr-x   0 zach       (502) staff       (20)     6730 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/remove_trends.py
--rwxr-xr-x   0 zach       (502) staff       (20)     1227 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/shift.py
--rwxr-xr-x   0 zach       (502) staff       (20)     7549 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/trim.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2022-11-16 23:53:41.069244 chromatic-lightcurves-0.4.5/chromatic/rainbows/converters/
--rwxr-xr-x   0 zach       (502) staff       (20)       26 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/converters/__init__.py
--rwxr-xr-x   0 zach       (502) staff       (20)     3135 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/converters/for_altair.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2022-11-16 23:53:41.069968 chromatic-lightcurves-0.4.5/chromatic/rainbows/get/
--rwxr-xr-x   0 zach       (502) staff       (20)       48 2022-10-06 03:41:04.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/get/__init__.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2022-11-16 23:53:41.073862 chromatic-lightcurves-0.4.5/chromatic/rainbows/get/timelike/
--rwxr-xr-x   0 zach       (502) staff       (20)      109 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/get/timelike/__init__.py
--rwxr-xr-x   0 zach       (502) staff       (20)      503 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/get/timelike/average_lightcurve.py
--rwxr-xr-x   0 zach       (502) staff       (20)      508 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/get/timelike/descriptions.txt
--rwxr-xr-x   0 zach       (502) staff       (20)      394 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/get/timelike/median_lightcurve.py
--rwxr-xr-x   0 zach       (502) staff       (20)     2897 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/get/timelike/subset.py
--rwxr-xr-x   0 zach       (502) staff       (20)     6052 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/get/timelike/time.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2022-11-16 23:53:41.079632 chromatic-lightcurves-0.4.5/chromatic/rainbows/get/wavelike/
--rwxr-xr-x   0 zach       (502) staff       (20)      228 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/get/wavelike/__init__.py
--rwxr-xr-x   0 zach       (502) staff       (20)      513 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/get/wavelike/average_spectrum.py
--rwxr-xr-x   0 zach       (502) staff       (20)      618 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/get/wavelike/descriptions.txt
--rwxr-xr-x   0 zach       (502) staff       (20)      929 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/get/wavelike/expected_uncertainty.py
--rwxr-xr-x   0 zach       (502) staff       (20)     1875 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/get/wavelike/measured_scatter.py
--rwxr-xr-x   0 zach       (502) staff       (20)     2801 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/get/wavelike/measured_scatter_in_bins.py
--rwxr-xr-x   0 zach       (502) staff       (20)      380 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/get/wavelike/median_spectrum.py
--rwxr-xr-x   0 zach       (502) staff       (20)     1082 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/get/wavelike/spectral_resolution.py
--rwxr-xr-x   0 zach       (502) staff       (20)     2966 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/get/wavelike/subset.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2022-11-16 23:53:41.082796 chromatic-lightcurves-0.4.5/chromatic/rainbows/helpers/
--rwxr-xr-x   0 zach       (502) staff       (20)       82 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/helpers/__init__.py
--rwxr-xr-x   0 zach       (502) staff       (20)      238 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/helpers/descriptions.txt
--rw-r--r--   0 zach       (502) staff       (20)      927 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/helpers/get.py
--rwxr-xr-x   0 zach       (502) staff       (20)     1566 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/helpers/help.py
--rwxr-xr-x   0 zach       (502) staff       (20)     3784 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/helpers/history.py
--rw-r--r--   0 zach       (502) staff       (20)      713 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/helpers/save.py
--rwxr-xr-x   0 zach       (502) staff       (20)    21121 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/multi.py
--rwxr-xr-x   0 zach       (502) staff       (20)    37249 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/rainbow.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2022-11-16 23:53:41.097069 chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/
--rwxr-xr-x   0 zach       (502) staff       (20)     3948 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/__init__.py
--rwxr-xr-x   0 zach       (502) staff       (20)     5245 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/atoca.py
--rwxr-xr-x   0 zach       (502) staff       (20)     4541 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/coulombe.py
--rwxr-xr-x   0 zach       (502) staff       (20)     3901 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/dossantos.py
--rwxr-xr-x   0 zach       (502) staff       (20)     1638 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/espinoza.py
--rwxr-xr-x   0 zach       (502) staff       (20)     1594 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/eureka_channels.py
--rwxr-xr-x   0 zach       (502) staff       (20)     4183 2022-11-16 23:46:37.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/eureka_lcdata.py
--rwxr-xr-x   0 zach       (502) staff       (20)     4794 2022-11-16 23:46:37.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/eureka_specdata.py
--rwxr-xr-x   0 zach       (502) staff       (20)     1961 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/eureka_txt.py
--rwxr-xr-x   0 zach       (502) staff       (20)     2125 2022-11-15 00:24:17.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/feinstein.py
--rwxr-xr-x   0 zach       (502) staff       (20)     4948 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/kirk.py
--rwxr-xr-x   0 zach       (502) staff       (20)     3276 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/nres.py
--rwxr-xr-x   0 zach       (502) staff       (20)     1253 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/radica.py
--rwxr-xr-x   0 zach       (502) staff       (20)     1178 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/rainbow_FITS.py
--rwxr-xr-x   0 zach       (502) staff       (20)      774 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/rainbow_npy.py
--rwxr-xr-x   0 zach       (502) staff       (20)     1430 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/schlawin.py
--rwxr-xr-x   0 zach       (502) staff       (20)     3709 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/template.py
--rwxr-xr-x   0 zach       (502) staff       (20)     1896 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/text.py
--rwxr-xr-x   0 zach       (502) staff       (20)    15533 2022-11-16 23:46:37.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/x1dints.py
--rwxr-xr-x   0 zach       (502) staff       (20)     7472 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/x1dints_kludge.py
--rwxr-xr-x   0 zach       (502) staff       (20)     3567 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/xarray_fitted_light_curves.py
--rwxr-xr-x   0 zach       (502) staff       (20)     3209 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/xarray_raw_light_curves.py
--rwxr-xr-x   0 zach       (502) staff       (20)     3122 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/xarray_stellar_spectra.py
--rwxr-xr-x   0 zach       (502) staff       (20)     8463 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/simulated.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2022-11-16 23:53:41.101371 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/
--rwxr-xr-x   0 zach       (502) staff       (20)      324 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/__init__.py
--rwxr-xr-x   0 zach       (502) staff       (20)    15989 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/animate.py
--rwxr-xr-x   0 zach       (502) staff       (20)     3282 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/colors.py
--rwxr-xr-x   0 zach       (502) staff       (20)      620 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/descriptions.txt
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2022-11-16 23:53:41.103177 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/diagnostics/
--rwxr-xr-x   0 zach       (502) staff       (20)       89 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/diagnostics/__init__.py
--rwxr-xr-x   0 zach       (502) staff       (20)      311 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/diagnostics/descriptions.txt
--rwxr-xr-x   0 zach       (502) staff       (20)     3698 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/diagnostics/histogram.py
--rwxr-xr-x   0 zach       (502) staff       (20)     2426 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/diagnostics/imshow_quantities.py
--rwxr-xr-x   0 zach       (502) staff       (20)     3303 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/diagnostics/plot_quantities.py
--rwxr-xr-x   0 zach       (502) staff       (20)     7408 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/imshow.py
--rwxr-xr-x   0 zach       (502) staff       (20)     6882 2022-11-16 23:46:37.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/interactive.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2022-11-16 23:53:41.105895 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/models/
--rwxr-xr-x   0 zach       (502) staff       (20)      112 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/models/__init__.py
--rwxr-xr-x   0 zach       (502) staff       (20)      393 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/models/descriptions.txt
--rwxr-xr-x   0 zach       (502) staff       (20)     5261 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/models/imshow_with_models.py
--rwxr-xr-x   0 zach       (502) staff       (20)    13439 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/models/plot_one_wavelength_with_models.py
--rwxr-xr-x   0 zach       (502) staff       (20)     4737 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/models/plot_with_model.py
--rwxr-xr-x   0 zach       (502) staff       (20)     4769 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/pcolormesh.py
--rwxr-xr-x   0 zach       (502) staff       (20)     1023 2022-10-06 04:04:01.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/plot.py
--rwxr-xr-x   0 zach       (502) staff       (20)     7356 2022-11-16 23:46:37.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/plot_lightcurves.py
--rwxr-xr-x   0 zach       (502) staff       (20)     6821 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/plot_spectra.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2022-11-16 23:53:41.107976 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/timelike/
--rwxr-xr-x   0 zach       (502) staff       (20)       67 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/timelike/__init__.py
--rwxr-xr-x   0 zach       (502) staff       (20)      711 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/timelike/average_lightcurve.py
--rwxr-xr-x   0 zach       (502) staff       (20)      184 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/timelike/descriptions.txt
--rwxr-xr-x   0 zach       (502) staff       (20)      707 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/timelike/median_lightcurve.py
--rwxr-xr-x   0 zach       (502) staff       (20)     6387 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/utilities.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2022-11-16 23:53:41.111635 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/wavelike/
--rwxr-xr-x   0 zach       (502) staff       (20)      170 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/wavelike/__init__.py
--rwxr-xr-x   0 zach       (502) staff       (20)      715 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/wavelike/average_spectrum.py
--rwxr-xr-x   0 zach       (502) staff       (20)      408 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/wavelike/descriptions.txt
--rwxr-xr-x   0 zach       (502) staff       (20)      711 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/wavelike/median_spectrum.py
--rwxr-xr-x   0 zach       (502) staff       (20)     4810 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/wavelike/noise_comparison.py
--rwxr-xr-x   0 zach       (502) staff       (20)     2124 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/wavelike/noise_comparison_in_bins.py
--rwxr-xr-x   0 zach       (502) staff       (20)     1012 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/wavelike/spectral_resolution.py
--rwxr-xr-x   0 zach       (502) staff       (20)     2996 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/withmodel.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2022-11-16 23:53:41.116265 chromatic-lightcurves-0.4.5/chromatic/rainbows/writers/
--rwxr-xr-x   0 zach       (502) staff       (20)     1868 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/writers/__init__.py
--rwxr-xr-x   0 zach       (502) staff       (20)     1558 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/writers/rainbow_FITS.py
--rwxr-xr-x   0 zach       (502) staff       (20)      767 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/writers/rainbow_npy.py
--rwxr-xr-x   0 zach       (502) staff       (20)     2438 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/writers/template.py
--rwxr-xr-x   0 zach       (502) staff       (20)     1689 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/writers/text.py
--rwxr-xr-x   0 zach       (502) staff       (20)     4488 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/writers/xarray_fitted_light_curves.py
--rwxr-xr-x   0 zach       (502) staff       (20)     3946 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/writers/xarray_raw_light_curves.py
--rwxr-xr-x   0 zach       (502) staff       (20)     3700 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/rainbows/writers/xarray_stellar_spectra.py
--rwxr-xr-x   0 zach       (502) staff       (20)    25293 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/resampling.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2022-11-16 23:53:41.119201 chromatic-lightcurves-0.4.5/chromatic/spectra/
--rwxr-xr-x   0 zach       (502) staff       (20)       45 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/spectra/__init__.py
--rwxr-xr-x   0 zach       (502) staff       (20)    38477 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/spectra/phoenix.py
--rwxr-xr-x   0 zach       (502) staff       (20)     3196 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/spectra/planck.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2022-11-16 23:53:41.135181 chromatic-lightcurves-0.4.5/chromatic/tests/
--rwxr-xr-x   0 zach       (502) staff       (20)      637 2022-10-01 13:31:56.000000 chromatic-lightcurves-0.4.5/chromatic/tests/__init__.py
--rwxr-xr-x   0 zach       (502) staff       (20)      148 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/tests/setup_tests.py
--rwxr-xr-x   0 zach       (502) staff       (20)     3639 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/tests/test_align_wavelengths.py
--rwxr-xr-x   0 zach       (502) staff       (20)     3649 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/tests/test_basics.py
--rwxr-xr-x   0 zach       (502) staff       (20)     9879 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/tests/test_binning.py
--rwxr-xr-x   0 zach       (502) staff       (20)     2298 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/tests/test_conversions.py
--rwxr-xr-x   0 zach       (502) staff       (20)      939 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/chromatic/tests/test_fold.py
--rwxr-xr-x   0 zach       (502) staff       (20)     1001 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/tests/test_history.py
--rwxr-xr-x   0 zach       (502) staff       (20)     2750 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/tests/test_io.py
--rwxr-xr-x   0 zach       (502) staff       (20)     1186 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/tests/test_multi.py
--rwxr-xr-x   0 zach       (502) staff       (20)     1445 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/tests/test_normalize.py
--rwxr-xr-x   0 zach       (502) staff       (20)     2621 2022-10-03 20:05:27.000000 chromatic-lightcurves-0.4.5/chromatic/tests/test_ok.py
--rwxr-xr-x   0 zach       (502) staff       (20)     2914 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/tests/test_operations.py
--rw-r--r--   0 zach       (502) staff       (20)     1033 2022-10-01 13:31:56.000000 chromatic-lightcurves-0.4.5/chromatic/tests/test_outliers.py
--rwxr-xr-x   0 zach       (502) staff       (20)     1611 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/tests/test_remove_trends.py
--rwxr-xr-x   0 zach       (502) staff       (20)     4635 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/tests/test_resampling.py
--rwxr-xr-x   0 zach       (502) staff       (20)     1622 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/tests/test_shift.py
--rwxr-xr-x   0 zach       (502) staff       (20)     3637 2022-11-15 00:30:54.000000 chromatic-lightcurves-0.4.5/chromatic/tests/test_simulations.py
--rwxr-xr-x   0 zach       (502) staff       (20)     2989 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/tests/test_spectra.py
--rwxr-xr-x   0 zach       (502) staff       (20)     2559 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/tests/test_summaries.py
--rwxr-xr-x   0 zach       (502) staff       (20)      496 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/tests/test_time.py
--rwxr-xr-x   0 zach       (502) staff       (20)      376 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/tests/test_trimming.py
--rwxr-xr-x   0 zach       (502) staff       (20)      173 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/tests/test_units.py
--rwxr-xr-x   0 zach       (502) staff       (20)    10687 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/tests/test_visualizations.py
--rwxr-xr-x   0 zach       (502) staff       (20)     3472 2022-11-08 03:50:16.000000 chromatic-lightcurves-0.4.5/chromatic/tests/test_withmodel.py
--rwxr-xr-x   0 zach       (502) staff       (20)      847 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/chromatic/units.py
--rwxr-xr-x   0 zach       (502) staff       (20)       62 2022-11-16 23:53:19.000000 chromatic-lightcurves-0.4.5/chromatic/version.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2022-11-16 23:53:41.138166 chromatic-lightcurves-0.4.5/chromatic_lightcurves.egg-info/
--rw-r--r--   0 zach       (502) staff       (20)      641 2022-11-16 23:53:40.000000 chromatic-lightcurves-0.4.5/chromatic_lightcurves.egg-info/PKG-INFO
--rw-r--r--   0 zach       (502) staff       (20)     6996 2022-11-16 23:53:40.000000 chromatic-lightcurves-0.4.5/chromatic_lightcurves.egg-info/SOURCES.txt
--rw-r--r--   0 zach       (502) staff       (20)        1 2022-11-16 23:53:40.000000 chromatic-lightcurves-0.4.5/chromatic_lightcurves.egg-info/dependency_links.txt
--rw-r--r--   0 zach       (502) staff       (20)        1 2021-07-30 14:17:57.000000 chromatic-lightcurves-0.4.5/chromatic_lightcurves.egg-info/not-zip-safe
--rw-r--r--   0 zach       (502) staff       (20)      333 2022-11-16 23:53:40.000000 chromatic-lightcurves-0.4.5/chromatic_lightcurves.egg-info/requires.txt
--rw-r--r--   0 zach       (502) staff       (20)       10 2022-11-16 23:53:40.000000 chromatic-lightcurves-0.4.5/chromatic_lightcurves.egg-info/top_level.txt
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2022-11-16 23:53:41.147765 chromatic-lightcurves-0.4.5/docs/
--rwxr-xr-x   0 zach       (502) staff       (20)    20910 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/docs/actions.ipynb
--rw-r--r--   0 zach       (502) staff       (20)     3492 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/docs/api.md
--rwxr-xr-x   0 zach       (502) staff       (20)     8185 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/docs/basics.ipynb
--rwxr-xr-x   0 zach       (502) staff       (20)    14863 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/docs/creating.ipynb
--rwxr-xr-x   0 zach       (502) staff       (20)    11038 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/docs/designing.ipynb
--rwxr-xr-x   0 zach       (502) staff       (20)     2713 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/docs/documentation.ipynb
--rwxr-xr-x   0 zach       (502) staff       (20)    16372 2022-11-16 23:46:37.000000 chromatic-lightcurves-0.4.5/docs/example-timeseries-spectra.ipynb
--rwxr-xr-x   0 zach       (502) staff       (20)    10634 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/docs/github.ipynb
--rwxr-xr-x   0 zach       (502) staff       (20)      715 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/docs/index.md
--rwxr-xr-x   0 zach       (502) staff       (20)     5401 2022-11-16 23:46:37.000000 chromatic-lightcurves-0.4.5/docs/installation.ipynb
--rwxr-xr-x   0 zach       (502) staff       (20)    17965 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/docs/io.ipynb
--rwxr-xr-x   0 zach       (502) staff       (20)     9495 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/docs/models.ipynb
--rwxr-xr-x   0 zach       (502) staff       (20)     2567 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/docs/multi.ipynb.ignore
--rwxr-xr-x   0 zach       (502) staff       (20)     9810 2022-11-16 23:46:37.000000 chromatic-lightcurves-0.4.5/docs/quickstart.ipynb
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2022-11-16 23:53:41.149318 chromatic-lightcurves-0.4.5/docs/tools/
--rwxr-xr-x   0 zach       (502) staff       (20)    10868 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/docs/tools/binning.ipynb
--rwxr-xr-x   0 zach       (502) staff       (20)     3073 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/docs/tools/colormaps.ipynb
--rwxr-xr-x   0 zach       (502) staff       (20)    13016 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/docs/tools/spectra.ipynb
--rwxr-xr-x   0 zach       (502) staff       (20)     8909 2022-11-06 21:35:42.000000 chromatic-lightcurves-0.4.5/docs/visualizing.ipynb
--rwxr-xr-x   0 zach       (502) staff       (20)     1650 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/mkdocs.yml
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2022-11-16 23:53:41.150406 chromatic-lightcurves-0.4.5/notes/
--rwxr-xr-x   0 zach       (502) staff       (20)     1432 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.5/notes/how-to-do-pre-commit.md
--rwxr-xr-x   0 zach       (502) staff       (20)     1935 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.5/notes/how-to-do-the-docs.md
--rw-r--r--   0 zach       (502) staff       (20)       38 2022-11-16 23:53:41.151078 chromatic-lightcurves-0.4.5/setup.cfg
--rw-r--r--   0 zach       (502) staff       (20)     4141 2022-11-16 23:52:56.000000 chromatic-lightcurves-0.4.5/setup.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-21 14:35:11.560904 chromatic-lightcurves-0.4.7/
+-rwxr-xr-x   0 zach       (502) staff       (20)     2248 2023-06-21 14:34:54.000000 chromatic-lightcurves-0.4.7/.gitignore
+-rwxr-xr-x   0 zach       (502) staff       (20)      329 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/.pre-commit-config.yaml
+-rwxr-xr-x   0 zach       (502) staff       (20)     1076 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/LICENSE
+-rw-r--r--   0 zach       (502) staff       (20)      641 2023-06-21 14:35:11.560629 chromatic-lightcurves-0.4.7/PKG-INFO
+-rwxr-xr-x   0 zach       (502) staff       (20)     2597 2023-06-21 14:34:54.000000 chromatic-lightcurves-0.4.7/README.md
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-21 14:35:11.516781 chromatic-lightcurves-0.4.7/chromatic/
+-rwxr-xr-x   0 zach       (502) staff       (20)      119 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/__init__.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     5005 2022-11-08 03:57:51.000000 chromatic-lightcurves-0.4.7/chromatic/imports.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-21 14:35:11.517970 chromatic-lightcurves-0.4.7/chromatic/rainbows/
+-rwxr-xr-x   0 zach       (502) staff       (20)      890 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/__init__.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-21 14:35:11.522587 chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/
+-rwxr-xr-x   0 zach       (502) staff       (20)      444 2022-10-07 04:08:11.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/__init__.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     8427 2023-06-21 14:34:54.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/align_wavelengths.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     1955 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/attach_model.py
+-rwxr-xr-x   0 zach       (502) staff       (20)    27690 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/binning.py
+-rwxr-xr-x   0 zach       (502) staff       (20)      832 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/compare.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     1310 2023-06-21 14:34:54.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/descriptions.txt
+-rwxr-xr-x   0 zach       (502) staff       (20)     3542 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/flag_outliers.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     3399 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/fold.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     3414 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/inflate_uncertainty.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     3856 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/inject_noise.py
+-rw-r--r--   0 zach       (502) staff       (20)     1699 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/inject_outliers.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     2630 2023-06-21 14:34:54.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/inject_spectrum.py
+-rwxr-xr-x   0 zach       (502) staff       (20)    10376 2022-11-08 03:57:51.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/inject_systematics.py
+-rwxr-xr-x   0 zach       (502) staff       (20)    18525 2022-11-15 00:30:54.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/inject_transit.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     4807 2023-06-21 14:34:54.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/normalization.py
+-rwxr-xr-x   0 zach       (502) staff       (20)    11422 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/operations.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     6730 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/remove_trends.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     1227 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/shift.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     8789 2023-06-21 14:34:54.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/trim.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-21 14:35:11.522995 chromatic-lightcurves-0.4.7/chromatic/rainbows/converters/
+-rwxr-xr-x   0 zach       (502) staff       (20)       26 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/converters/__init__.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     3135 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/converters/for_altair.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-21 14:35:11.523178 chromatic-lightcurves-0.4.7/chromatic/rainbows/get/
+-rwxr-xr-x   0 zach       (502) staff       (20)       72 2023-06-21 14:34:54.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/get/__init__.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-21 14:35:11.523614 chromatic-lightcurves-0.4.7/chromatic/rainbows/get/fluxlike/
+-rw-r--r--   0 zach       (502) staff       (20)       22 2023-06-21 14:34:54.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/get/fluxlike/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)      926 2023-06-21 14:34:54.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/get/fluxlike/subset.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-21 14:35:11.525490 chromatic-lightcurves-0.4.7/chromatic/rainbows/get/timelike/
+-rwxr-xr-x   0 zach       (502) staff       (20)      109 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/get/timelike/__init__.py
+-rwxr-xr-x   0 zach       (502) staff       (20)      503 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/get/timelike/average_lightcurve.py
+-rwxr-xr-x   0 zach       (502) staff       (20)      508 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/get/timelike/descriptions.txt
+-rwxr-xr-x   0 zach       (502) staff       (20)      403 2023-06-21 14:34:54.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/get/timelike/median_lightcurve.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     2897 2023-04-12 21:35:28.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/get/timelike/subset.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     6052 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/get/timelike/time.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-21 14:35:11.527477 chromatic-lightcurves-0.4.7/chromatic/rainbows/get/wavelike/
+-rwxr-xr-x   0 zach       (502) staff       (20)      228 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/get/wavelike/__init__.py
+-rwxr-xr-x   0 zach       (502) staff       (20)      513 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/get/wavelike/average_spectrum.py
+-rwxr-xr-x   0 zach       (502) staff       (20)      618 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/get/wavelike/descriptions.txt
+-rwxr-xr-x   0 zach       (502) staff       (20)      929 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/get/wavelike/expected_uncertainty.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     1875 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/get/wavelike/measured_scatter.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     2801 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/get/wavelike/measured_scatter_in_bins.py
+-rwxr-xr-x   0 zach       (502) staff       (20)      389 2023-06-21 14:34:54.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/get/wavelike/median_spectrum.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     1082 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/get/wavelike/spectral_resolution.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     2966 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/get/wavelike/subset.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-21 14:35:11.528909 chromatic-lightcurves-0.4.7/chromatic/rainbows/helpers/
+-rwxr-xr-x   0 zach       (502) staff       (20)       82 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/helpers/__init__.py
+-rwxr-xr-x   0 zach       (502) staff       (20)      236 2023-06-21 14:34:54.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/helpers/descriptions.txt
+-rw-r--r--   0 zach       (502) staff       (20)      927 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/helpers/get.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     1566 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/helpers/help.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     3784 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/helpers/history.py
+-rw-r--r--   0 zach       (502) staff       (20)      713 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/helpers/save.py
+-rwxr-xr-x   0 zach       (502) staff       (20)    21121 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/multi.py
+-rwxr-xr-x   0 zach       (502) staff       (20)    37349 2023-06-21 14:34:54.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/rainbow.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-21 14:35:11.534521 chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/
+-rwxr-xr-x   0 zach       (502) staff       (20)     4042 2023-06-21 14:34:54.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/__init__.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     5245 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/atoca.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     3972 2023-06-21 14:34:54.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/aylin.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     4541 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/coulombe.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     3901 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/dossantos.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     1638 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/espinoza.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     1594 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/eureka_channels.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     4183 2022-11-16 23:46:37.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/eureka_lcdata.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     4826 2023-06-21 14:34:54.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/eureka_specdata.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     1961 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/eureka_txt.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     2125 2022-11-15 00:24:17.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/feinstein.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     4948 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/kirk.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     3276 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/nres.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     1253 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/radica.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     1178 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/rainbow_FITS.py
+-rwxr-xr-x   0 zach       (502) staff       (20)      774 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/rainbow_npy.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     1430 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/schlawin.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     3709 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/template.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     1896 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/text.py
+-rwxr-xr-x   0 zach       (502) staff       (20)    15534 2023-06-21 14:34:54.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/x1dints.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     7472 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/x1dints_kludge.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     3567 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/xarray_fitted_light_curves.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     3209 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/xarray_raw_light_curves.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     3122 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/xarray_stellar_spectra.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     8463 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/simulated.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-21 14:35:11.537676 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/
+-rwxr-xr-x   0 zach       (502) staff       (20)      324 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/__init__.py
+-rwxr-xr-x   0 zach       (502) staff       (20)    15989 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/animate.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     3282 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/colors.py
+-rwxr-xr-x   0 zach       (502) staff       (20)      620 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/descriptions.txt
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-21 14:35:11.539256 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/diagnostics/
+-rwxr-xr-x   0 zach       (502) staff       (20)       89 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/diagnostics/__init__.py
+-rwxr-xr-x   0 zach       (502) staff       (20)      311 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/diagnostics/descriptions.txt
+-rwxr-xr-x   0 zach       (502) staff       (20)     3698 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/diagnostics/histogram.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     2426 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/diagnostics/imshow_quantities.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     3303 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/diagnostics/plot_quantities.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     7902 2023-06-21 14:34:54.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/imshow.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     6882 2022-11-16 23:46:37.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/interactive.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-21 14:35:11.540864 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/models/
+-rwxr-xr-x   0 zach       (502) staff       (20)      112 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/models/__init__.py
+-rwxr-xr-x   0 zach       (502) staff       (20)      393 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/models/descriptions.txt
+-rwxr-xr-x   0 zach       (502) staff       (20)     5261 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/models/imshow_with_models.py
+-rwxr-xr-x   0 zach       (502) staff       (20)    13439 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/models/plot_one_wavelength_with_models.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     4737 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/models/plot_with_model.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     4769 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/pcolormesh.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     1023 2022-10-06 04:04:01.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/plot.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     7356 2022-11-16 23:46:37.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/plot_lightcurves.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     6821 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/plot_spectra.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-21 14:35:11.541924 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/timelike/
+-rwxr-xr-x   0 zach       (502) staff       (20)       67 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/timelike/__init__.py
+-rwxr-xr-x   0 zach       (502) staff       (20)      711 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/timelike/average_lightcurve.py
+-rwxr-xr-x   0 zach       (502) staff       (20)      184 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/timelike/descriptions.txt
+-rwxr-xr-x   0 zach       (502) staff       (20)      707 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/timelike/median_lightcurve.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     6387 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/utilities.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-21 14:35:11.543589 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/wavelike/
+-rwxr-xr-x   0 zach       (502) staff       (20)      170 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/wavelike/__init__.py
+-rwxr-xr-x   0 zach       (502) staff       (20)      715 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/wavelike/average_spectrum.py
+-rwxr-xr-x   0 zach       (502) staff       (20)      408 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/wavelike/descriptions.txt
+-rwxr-xr-x   0 zach       (502) staff       (20)      711 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/wavelike/median_spectrum.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     4810 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/wavelike/noise_comparison.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     2124 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/wavelike/noise_comparison_in_bins.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     1012 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/wavelike/spectral_resolution.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     2996 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/withmodel.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-21 14:35:11.545618 chromatic-lightcurves-0.4.7/chromatic/rainbows/writers/
+-rwxr-xr-x   0 zach       (502) staff       (20)     1868 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/writers/__init__.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     1558 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/writers/rainbow_FITS.py
+-rwxr-xr-x   0 zach       (502) staff       (20)      767 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/writers/rainbow_npy.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     2438 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/writers/template.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     1689 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/writers/text.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     4488 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/writers/xarray_fitted_light_curves.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     3946 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/writers/xarray_raw_light_curves.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     3700 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/rainbows/writers/xarray_stellar_spectra.py
+-rwxr-xr-x   0 zach       (502) staff       (20)    25293 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/resampling.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-21 14:35:11.546470 chromatic-lightcurves-0.4.7/chromatic/spectra/
+-rwxr-xr-x   0 zach       (502) staff       (20)       45 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/spectra/__init__.py
+-rwxr-xr-x   0 zach       (502) staff       (20)    38477 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/spectra/phoenix.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     3196 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/spectra/planck.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-21 14:35:11.552931 chromatic-lightcurves-0.4.7/chromatic/tests/
+-rwxr-xr-x   0 zach       (502) staff       (20)      637 2022-10-01 13:31:56.000000 chromatic-lightcurves-0.4.7/chromatic/tests/__init__.py
+-rwxr-xr-x   0 zach       (502) staff       (20)      148 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/tests/setup_tests.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     3639 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/tests/test_align_wavelengths.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     3649 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/tests/test_basics.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     9879 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/tests/test_binning.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     2298 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/tests/test_conversions.py
+-rwxr-xr-x   0 zach       (502) staff       (20)      939 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/chromatic/tests/test_fold.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     1001 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/tests/test_history.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     2750 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/tests/test_io.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     1186 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/tests/test_multi.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     2200 2023-06-21 14:34:54.000000 chromatic-lightcurves-0.4.7/chromatic/tests/test_normalize.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     2621 2022-10-03 20:05:27.000000 chromatic-lightcurves-0.4.7/chromatic/tests/test_ok.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     2914 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/tests/test_operations.py
+-rw-r--r--   0 zach       (502) staff       (20)     1033 2022-10-01 13:31:56.000000 chromatic-lightcurves-0.4.7/chromatic/tests/test_outliers.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     1611 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/tests/test_remove_trends.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     4635 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/tests/test_resampling.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     1622 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/tests/test_shift.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     3637 2022-11-15 00:30:54.000000 chromatic-lightcurves-0.4.7/chromatic/tests/test_simulations.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     2989 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/tests/test_spectra.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     2559 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/tests/test_summaries.py
+-rwxr-xr-x   0 zach       (502) staff       (20)      496 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/tests/test_time.py
+-rwxr-xr-x   0 zach       (502) staff       (20)      376 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/tests/test_trimming.py
+-rwxr-xr-x   0 zach       (502) staff       (20)      173 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/tests/test_units.py
+-rwxr-xr-x   0 zach       (502) staff       (20)    10687 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/tests/test_visualizations.py
+-rwxr-xr-x   0 zach       (502) staff       (20)     3472 2022-11-08 03:50:16.000000 chromatic-lightcurves-0.4.7/chromatic/tests/test_withmodel.py
+-rwxr-xr-x   0 zach       (502) staff       (20)      847 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/chromatic/units.py
+-rwxr-xr-x   0 zach       (502) staff       (20)       62 2023-06-21 14:34:54.000000 chromatic-lightcurves-0.4.7/chromatic/version.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-21 14:35:11.554263 chromatic-lightcurves-0.4.7/chromatic_lightcurves.egg-info/
+-rw-r--r--   0 zach       (502) staff       (20)      641 2023-06-21 14:35:11.000000 chromatic-lightcurves-0.4.7/chromatic_lightcurves.egg-info/PKG-INFO
+-rw-r--r--   0 zach       (502) staff       (20)     7118 2023-06-21 14:35:11.000000 chromatic-lightcurves-0.4.7/chromatic_lightcurves.egg-info/SOURCES.txt
+-rw-r--r--   0 zach       (502) staff       (20)        1 2023-06-21 14:35:11.000000 chromatic-lightcurves-0.4.7/chromatic_lightcurves.egg-info/dependency_links.txt
+-rw-r--r--   0 zach       (502) staff       (20)        1 2021-07-30 14:17:57.000000 chromatic-lightcurves-0.4.7/chromatic_lightcurves.egg-info/not-zip-safe
+-rw-r--r--   0 zach       (502) staff       (20)      333 2023-06-21 14:35:11.000000 chromatic-lightcurves-0.4.7/chromatic_lightcurves.egg-info/requires.txt
+-rw-r--r--   0 zach       (502) staff       (20)       10 2023-06-21 14:35:11.000000 chromatic-lightcurves-0.4.7/chromatic_lightcurves.egg-info/top_level.txt
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-21 14:35:11.558806 chromatic-lightcurves-0.4.7/docs/
+-rwxr-xr-x   0 zach       (502) staff       (20)    20910 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/docs/actions.ipynb
+-rw-r--r--   0 zach       (502) staff       (20)     3492 2022-11-06 22:17:46.000000 chromatic-lightcurves-0.4.7/docs/api.md
+-rwxr-xr-x   0 zach       (502) staff       (20)     8185 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/docs/basics.ipynb
+-rwxr-xr-x   0 zach       (502) staff       (20)    14863 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/docs/creating.ipynb
+-rwxr-xr-x   0 zach       (502) staff       (20)    11038 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/docs/designing.ipynb
+-rwxr-xr-x   0 zach       (502) staff       (20)     2713 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/docs/documentation.ipynb
+-rwxr-xr-x   0 zach       (502) staff       (20)    16372 2022-11-16 23:46:37.000000 chromatic-lightcurves-0.4.7/docs/example-timeseries-spectra.ipynb
+-rwxr-xr-x   0 zach       (502) staff       (20)    10634 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/docs/github.ipynb
+-rwxr-xr-x   0 zach       (502) staff       (20)      715 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/docs/index.md
+-rwxr-xr-x   0 zach       (502) staff       (20)     5401 2022-11-16 23:46:37.000000 chromatic-lightcurves-0.4.7/docs/installation.ipynb
+-rwxr-xr-x   0 zach       (502) staff       (20)    17965 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/docs/io.ipynb
+-rwxr-xr-x   0 zach       (502) staff       (20)     9495 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/docs/models.ipynb
+-rwxr-xr-x   0 zach       (502) staff       (20)     2567 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/docs/multi.ipynb.ignore
+-rwxr-xr-x   0 zach       (502) staff       (20)     9761 2023-06-21 14:34:54.000000 chromatic-lightcurves-0.4.7/docs/quickstart.ipynb
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-21 14:35:11.559556 chromatic-lightcurves-0.4.7/docs/tools/
+-rwxr-xr-x   0 zach       (502) staff       (20)    10868 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/docs/tools/binning.ipynb
+-rwxr-xr-x   0 zach       (502) staff       (20)     3073 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/docs/tools/colormaps.ipynb
+-rwxr-xr-x   0 zach       (502) staff       (20)    13016 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/docs/tools/spectra.ipynb
+-rwxr-xr-x   0 zach       (502) staff       (20)     8909 2022-11-06 21:35:42.000000 chromatic-lightcurves-0.4.7/docs/visualizing.ipynb
+-rwxr-xr-x   0 zach       (502) staff       (20)     1687 2023-06-21 14:34:54.000000 chromatic-lightcurves-0.4.7/mkdocs.yml
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-21 14:35:11.560228 chromatic-lightcurves-0.4.7/notes/
+-rwxr-xr-x   0 zach       (502) staff       (20)     1432 2022-09-26 22:07:42.000000 chromatic-lightcurves-0.4.7/notes/how-to-do-pre-commit.md
+-rwxr-xr-x   0 zach       (502) staff       (20)     1935 2023-03-19 19:26:32.000000 chromatic-lightcurves-0.4.7/notes/how-to-do-the-docs.md
+-rw-r--r--   0 zach       (502) staff       (20)       38 2023-06-21 14:35:11.560989 chromatic-lightcurves-0.4.7/setup.cfg
+-rw-r--r--   0 zach       (502) staff       (20)     4141 2022-11-16 23:55:30.000000 chromatic-lightcurves-0.4.7/setup.py
```

### Comparing `chromatic-lightcurves-0.4.5/.gitignore` & `chromatic-lightcurves-0.4.7/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # a few extra things to watch out for
+.vscode/settings.json
 .DS_Store
 *.mp4
 *.gif
 *.png
 *.pdf
 *.dat
 *.npy
```

### Comparing `chromatic-lightcurves-0.4.5/LICENSE` & `chromatic-lightcurves-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/PKG-INFO` & `chromatic-lightcurves-0.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromatic-lightcurves
-Version: 0.4.5
+Version: 0.4.7
 Summary: Tools for working with spectroscopic light curves (of transiting exoplanets).
 Home-page: https://github.com/zkbt/chromatic
 Author: Zach Berta-Thompson
 Author-email: zach.bertathompson@colorado.edu
 License: MIT
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `chromatic-lightcurves-0.4.5/README.md` & `chromatic-lightcurves-0.4.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -32,8 +32,8 @@
 
 We welcome contributions from anyone who agrees to follow the `ers-transit` [Code of Conduct](https://ers-transit.github.io/code-of-conduct.html#ers-transit). If you're on the `ers-transit` slack, please join the #hack-chromatic channel there and say hello; otherwise, please contact Zach directly or just dive right in!
 
 A great initial way to contribute would be to [submit an Issue](https://github.com/zkbt/chromatic/issues) about a bug, question, or suggestion you might have. If you want to contribute code, the [Developer Guide](https://zkbt.github.io/chromatic/designing/) is probably the best place to start. We know it can feel a little scary to try to contribute to a shared code package, so we try our best to be friendly and helpful to new contributors trying to learn how!
 
 *And for context, Zach is a little new to trying to manage a big collaborative code project, so if there are things we could be doing better, please let him know!*
 
-The approximate goal is currently (as of May 2022) to have the code ready and the documentation complete enough to submit `chromatic-lightcurves` to the [Journal of Open Source Software](https://joss.theoj.org/) early enough to be a documented tool in support of the real ERS data (so, like, early late June 2022). If you contribute before then, you'll be included on the paper!
+The goal is to submit `chromatic-lightcurves` to the [Journal of Open Source Software](https://joss.theoj.org/) before the end of 2022. If you contribute before then, you'll be included on the paper!
```

### Comparing `chromatic-lightcurves-0.4.5/chromatic/imports.py` & `chromatic-lightcurves-0.4.7/chromatic/imports.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/__init__.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/__init__.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/align_wavelengths.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/align_wavelengths.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     Parameters
     ----------
     wscale : str
         What kind of a new wavelength axis should be created?
         Options include:
             'linear' = constant d[wavelength] between grid points
             'log' = constant d[wavelength]/[wavelength] between grid points
+            'nonlinear' = the median wavelength grid for all time points
 
     supersampling : float
         By how many times should we increase or decrease the wavelength sampling?
         In general, values >1 will split each input wavelength grid point into
         multiple supersampled wavelength grid points, values close to 1 will
         produce approximately one output wavelength for each input wavelength,
         and values <1 will average multiple input wavelengths into a single output
@@ -33,15 +34,15 @@
 
         (FIXME = add a way to estimate a covariance matrix when binning?)
 
     visualize : bool
         Should we make some plots showing how the shared wavelength
         axis compares to the original input wavelength axes?
     """
-    w = rainbow.fluxlike["wavelength_2d"] * 1
+    w = (rainbow.fluxlike["wavelength_2d"] * 1).to(u.micron)
     w[rainbow.ok == False] = np.nan
     dw_per_time = np.gradient(w, axis=rainbow.waveaxis)
     R_per_time = w / dw_per_time
 
     if visualize:
         fi, ax = plt.subplots(1, 2, figsize=(8, 3), dpi=300)
         plt.sca(ax[0])
@@ -61,14 +62,16 @@
     min_w, max_w = np.nanmin(w).to("micron").value, np.nanmax(w).to("micron").value
     if wscale == "linear":
         dw = np.nanmedian(dw_per_time).to("micron").value / supersampling
         shared_w = np.arange(min_w, max_w + dw, dw) * u.micron
     elif wscale == "log":
         R = np.nanmedian(w / dw_per_time) * supersampling
         shared_w = np.exp(np.arange(np.log(min_w), np.log(max_w) + 1 / R, 1 / R))
+    elif wscale == "nonlinear":
+        shared_w = np.nanmedian(w, axis=1)
     shared_dw = np.gradient(shared_w)
     shared_R = shared_w / shared_dw
 
     if visualize:
         fi, ax = plt.subplots(1, 2, figsize=(8, 3), dpi=300)
         plt.sca(ax[0])
         plt.plot(w, dw_per_time, alpha=0.2)
@@ -144,14 +147,15 @@
                   All data points will be included in the bin.
                   The OK-ness will propagate onward.
     wscale : str, optional
         What kind of a new wavelength axis should be created?
         Options include:
             'linear' = constant d[wavelength] between grid points
             'log' = constant d[wavelength]/[wavelength] between grid points
+            'nonlinear' = the median wavelength grid for all time points
     supersampling : float, optional
         By how many times should we increase or decrease the wavelength sampling?
         In general, values >1 will split each input wavelength grid point into
         multiple supersampled wavelength grid points, values close to 1 will
         produce approximately one output wavelength for each input wavelength,
         and values <1 will average multiple input wavelengths into a single output
         wavelength bin.
```

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/attach_model.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/attach_model.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/binning.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/binning.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/compare.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/compare.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/descriptions.txt` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/descriptions.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 🌈🎧🎲 | inject_noise| Inject (uncorrelated, simple) random noise.
 🌈🎧🎹 | inject_systematics| Inject (correlated, wobbly) systematic noise.
 🌈⭐️👻 | inject_spectrum | Inject a static stellar spectrum.
 🌈🪐🚞 | inject_transit | Inject a transit signal.
 🌈🫓😑 | normalize | Normalize by dividing through by a typical spectrum (and/or light curve).
 🌈🏴‍☠️🛁 | remove_trends | Remove smooth trends in time and/or wavelength.
 🌈🚇🌊 | shift | Doppler shift wavelengths.
-🌈🍱💇 | trim | Trim away wavelengths or times that contain no good data.
+🌈🍱💇 | trim | Trim away wavelengths or times.
```

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/flag_outliers.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/flag_outliers.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/fold.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/fold.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/inflate_uncertainty.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/inflate_uncertainty.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/inject_noise.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/inject_noise.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/inject_outliers.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/inject_outliers.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/inject_spectrum.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/inject_spectrum.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     # create a history entry for this action (before other variables are defined)
     h = self._create_history_entry("inject_spectrum", locals())
 
     # create a copy of the existing Rainbow
     new = self._create_copy()
 
     # warn if maybe we shouldn't inject anything
-    if np.all(self.flux != 1):
+    if np.all(u.Quantity(self.flux).value != 1):
         cheerfully_suggest(
             f"""
         None of the pre-existing flux values were 1,
         which hints at the possibility that there
         might already be a spectrum in them. Please
         watch out for weird units or values!
         """
```

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/inject_systematics.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/inject_systematics.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/inject_transit.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/inject_transit.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/normalization.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/normalization.py`

 * *Files 18% similar despite different names*

```diff
@@ -40,39 +40,77 @@
 
     # create a history entry for this action (before other variables are defined)
     h = self._create_history_entry("normalize", locals())
 
     # create an empty copy
     new = self._create_copy()
 
+    # shortcut for the first letter of the axis
+    a = axis.lower()[0]
+
     # (ignore nan warnings)
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
 
-        if axis.lower()[0] == "w":
-            normalization = np.nanpercentile(new.flux, percentile, axis=self.timeaxis)
+        # get fluxes, with not-OK replaced with nans
+        flux_for_normalizing = new.get_ok_data()
+        negative_normalization_message = ""
+        if a == "w":
+            normalization = np.nanpercentile(
+                flux_for_normalizing, percentile, axis=self.timeaxis
+            )
             for k in self._keys_that_respond_to_math:
                 new.fluxlike[k] = new.get(k) / normalization[:, np.newaxis]
             try:
                 new.fluxlike["uncertainty"] = (
                     self.uncertainty / normalization[:, np.newaxis]
                 )
             except ValueError:
                 pass
-        elif axis.lower()[0] == "t":
-            normalization = np.nanpercentile(self.flux, percentile, axis=self.waveaxis)
+
+        elif a == "t":
+            normalization = np.nanpercentile(
+                flux_for_normalizing, percentile, axis=self.waveaxis
+            )
             for k in self._keys_that_respond_to_math:
                 new.fluxlike[k] = new.get(k) / normalization[np.newaxis, :]
             try:
                 new.fluxlike["uncertainty"] = (
                     self.uncertainty / normalization[np.newaxis, :]
                 )
             except ValueError:
                 pass
 
+    if a in "wt":
+        thing = {"w": "wavelengths", "t": "times"}[a]
+        fix = {
+            "w": """
+                ok = rainbow.get_median_spectrum() > 0
+                rainbow[ok, :].normalize()
+        """,
+            "t": """
+                ok = rainbow.get_median_lightcurve() > 0
+                rainbow[:, ok].normalize()
+        """,
+        }[a]
+        if np.any(normalization < 0):
+            cheerfully_suggest(
+                f"""
+            There are {np.sum(normalization < 0)} negative {thing} that
+            are going into the normalization of this Rainbow. If you're
+            not expecting negative fluxes, it may be useful to trim them
+            away with something like:
+
+            {fix}
+
+            Otherwise, watch out that your fluxes and uncertainties may
+            potentially have flipped sign!
+            """
+            )
+
     # append the history entry to the new Rainbow
     new._record_history_entry(h)
 
     # return the new Rainbow
     return new
```

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/operations.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/operations.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/remove_trends.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/remove_trends.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/shift.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/shift.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/actions/trim.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/actions/trim.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,32 @@
 from ...imports import *
 
 __all__ = ["trim", "trim_times", "trim_wavelengths"]
 
 
-def trim_times(self, just_edges=True, when_to_give_up=1, minimum_acceptable_ok=1):
+def trim_times(
+    self,
+    t_min=None,
+    t_max=None,
+    just_edges=True,
+    when_to_give_up=1,
+    minimum_acceptable_ok=1,
+):
     """
-    Trim times that are all (or mostly) useless.
+    Trim in time.
+
+    This removes times that either (a) fall outside of a desired time range
+    or (b) are mostly useless.
 
     Parameters
     ----------
+    t_min : u.Quantity
+        The minimum time to keep.
+    t_max : u.Quantity
+        The maximum time to keep.
     just_edges : bool, optional
         Should we only trim the outermost bad time bins?
             `True` = Just trim off the bad edges and keep
             interior bad values. Keeping interior data, even if
             they're all bad, often helps to make for more
             intuititive imshow plots.
             `False` = Trim off every bad time, whether it's on
@@ -45,14 +59,20 @@
 
     # figure out which times should be considered bad
     is_nan = np.isnan(self.flux)
     isnt_ok = self.ok < minimum_acceptable_ok
     fraction_bad = np.sum(is_nan | isnt_ok, axis=self.waveaxis) / self.nwave
     should_be_kept = fraction_bad < when_to_give_up
 
+    # trim in time
+    if t_min is not None:
+        should_be_kept = should_be_kept * (self.time >= t_min)
+    if t_max is not None:
+        should_be_kept = should_be_kept * (self.time <= t_max)
+
     # only make cuts on the edges (if desired)
     if just_edges:
         isnt_before_first = np.cumsum(should_be_kept) > 0
         isnt_after_last = (np.cumsum(should_be_kept[::-1]) > 0)[::-1]
         isnt_edge = isnt_before_first & isnt_after_last
         should_be_kept = should_be_kept | isnt_edge
 
@@ -63,20 +83,31 @@
     # append the history entry to the new Rainbow
     new._record_history_entry(h)
 
     # return the new Rainbow
     return new
 
 
-def trim_wavelengths(self, just_edges=True, when_to_give_up=1, minimum_acceptable_ok=1):
+def trim_wavelengths(
+    self,
+    w_min=None,
+    w_max=None,
+    just_edges=True,
+    when_to_give_up=1,
+    minimum_acceptable_ok=1,
+):
     """
     Trim wavelengths that are all (or mostly) useless.
 
     Parameters
     ----------
+    w_min : u.Quantity
+        The minimum wavelength to keep.
+    w_max : u.Quantity
+        The maximum wavelength to keep.
     just_edges : bool, optional
         Should we only trim the outermost bad wavelength bins?
             `True` = Just trim off the bad edges and keep
             interior bad values. Keeping interior data, even if
             they're all bad, often helps to make for more
             intuititive imshow plots.
             `False` = Trim off every bad wavelength, whether it's on
@@ -109,14 +140,20 @@
 
     # figure out which wavelengths should be considered bad
     is_nan = np.isnan(self.flux)
     isnt_ok = self.ok < minimum_acceptable_ok
     fraction_bad = np.sum(is_nan | isnt_ok, axis=self.timeaxis) / self.ntime
     should_be_kept = fraction_bad < when_to_give_up
 
+    # trim in wavelength
+    if w_min is not None:
+        should_be_kept = should_be_kept * (self.wavelength >= w_min)
+    if w_max is not None:
+        should_be_kept = should_be_kept * (self.wavelength <= w_max)
+
     # only make cuts on the edges (if desired)
     if just_edges:
         isnt_before_first = np.cumsum(should_be_kept) > 0
         isnt_after_last = (np.cumsum(should_be_kept[::-1]) > 0)[::-1]
         isnt_edge = isnt_before_first & isnt_after_last
         should_be_kept = should_be_kept | isnt_edge
 
@@ -127,26 +164,43 @@
     # append the history entry to the new Rainbow
     new._record_history_entry(h)
 
     # return the new Rainbow
     return new
 
 
-def trim(self, just_edges=True, when_to_give_up=1, minimum_acceptable_ok=1):
+def trim(
+    self,
+    t_min=None,
+    t_max=None,
+    w_min=None,
+    w_max=None,
+    just_edges=True,
+    when_to_give_up=1,
+    minimum_acceptable_ok=1,
+):
     """
     Trim away bad wavelengths and/or times.
 
     If entire wavelengths or times are marked as not `ok`,
     we can probably remove them to simplify calculations
     and visualizations. This function will trim those away,
     by default only removing problem rows/columns on the ends,
     to maintain a contiguous block.
 
     Parameters
     ----------
+    t_min : u.Quantity
+        The minimum time to keep.
+    t_max : u.Quantity
+        The maximum time to keep.
+    w_min : u.Quantity
+        The minimum wavelength to keep.
+    w_max : u.Quantity
+        The maximum wavelength to keep.
     just_edges : bool, optional
         Should we only trim the outermost bad wavelength bins?
             `True` = Just trim off the bad edges and keep
             interior bad values. Keeping interior data, even if
             they're all bad, often helps to make for more
             intuititive imshow plots.
             `False` = Trim off every bad wavelength, whether it's on
@@ -171,18 +225,22 @@
     Returns
     -------
     trimmed : Rainbow
         The trimmed `Rainbow`.
     """
 
     trimmed = self.trim_times(
+        t_min=t_min,
+        t_max=t_max,
         when_to_give_up=when_to_give_up,
         just_edges=just_edges,
         minimum_acceptable_ok=minimum_acceptable_ok,
     )
     trimmed = trimmed.trim_wavelengths(
+        w_min=w_min,
+        w_max=w_max,
         when_to_give_up=when_to_give_up,
         just_edges=just_edges,
         minimum_acceptable_ok=minimum_acceptable_ok,
     )
 
     return trimmed
```

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/converters/for_altair.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/converters/for_altair.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/get/timelike/subset.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/get/timelike/subset.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/get/timelike/time.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/get/timelike/time.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/get/wavelike/average_spectrum.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/get/wavelike/average_spectrum.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/get/wavelike/descriptions.txt` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/get/wavelike/descriptions.txt`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/get/wavelike/expected_uncertainty.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/get/wavelike/expected_uncertainty.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/get/wavelike/measured_scatter.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/get/wavelike/measured_scatter.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/get/wavelike/measured_scatter_in_bins.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/get/wavelike/measured_scatter_in_bins.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/get/wavelike/spectral_resolution.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/get/wavelike/spectral_resolution.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/get/wavelike/subset.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/get/wavelike/subset.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/helpers/get.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/helpers/get.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/helpers/help.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/helpers/help.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/helpers/history.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/helpers/history.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/helpers/save.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/helpers/save.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/multi.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/multi.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/rainbow.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/rainbow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1001,24 +1001,29 @@
         get_expected_uncertainty,
         get_measured_scatter,
         get_measured_scatter_in_bins,
         get_for_wavelength,
         get_ok_data_for_wavelength,
     )
 
-    # import summary statistics for each wavelength
+    # import summary statistics for each time
     from .get.timelike import (
         get_average_lightcurve,
         get_median_lightcurve,
         get_for_time,
         get_ok_data_for_time,
         get_times_as_astropy,
         set_times_from_astropy,
     )
 
+    # import summary statistics for each time
+    from .get.fluxlike import (
+        get_ok_data,
+    )
+
     # import visualizations that can act on Rainbows
     from .visualizations import (
         imshow,
         pcolormesh,
         plot_lightcurves,
         _setup_animate_lightcurves,
         animate_lightcurves,
```

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/__init__.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from .espinoza import *
 from .dossantos import *
 from .feinstein import *
 from .schlawin import *
 from .coulombe import *
 from .kirk import *
 from .radica import *
+from .aylin import *
 
 
 # construct a dictionary of available readers
 available_readers = {k: globals()[k] for k in globals() if k[0:5] == "from_"}
 
 
 def guess_reader(filepath, format=None):
@@ -103,14 +104,16 @@
         return from_kirk_stellar_spectra
     elif fnmatch(f, "*.txt") or fnmatch(f, "*.csv"):
         return from_text
     elif fnmatch(f, "*e92-1d.fits") or fnmatch(f, "*e92-1d.fits.fz"):
         return from_nres
     elif fnmatch(f, "*spec_*.fits"):
         return from_schlawin
+    elif fnmatch(f, "*Original_Spectrum.csv"):
+        return from_aylin
     else:
         raise ValueError(
             f"""
         We're having trouble guessing the input format from the filename
         {f}
         Please try specifying a `format=` keyword to your call.
         """
```

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/atoca.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/atoca.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/coulombe.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/coulombe.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/dossantos.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/dossantos.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/espinoza.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/espinoza.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/eureka_channels.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/eureka_channels.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/eureka_lcdata.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/eureka_lcdata.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/eureka_specdata.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/eureka_specdata.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,18 +55,19 @@
     w_without_unit = dataset[k].data
     w_unit = u.Unit(dataset[k].attrs["wave_units"])
     rainbow.wavelike["wavelength"] = w_without_unit * w_unit
     keys_used.append(k)
 
     # populate a 1D array of times (with astropy units of time)
     k = "time"
-    if dataset[k].attrs["time_units"] == "BMJD_TDB":
+
+    if dataset[k].attrs.get("time_units", None) == "BMJD_TDB":
         astropy_times = Time(dataset[k].data, format="mjd", scale="tdb")
         rainbow.set_times_from_astropy(astropy_times, is_barycentric=True)
-    elif dataset[k].attrs["time_units"] == "BJD_TDB":
+    elif dataset[k].attrs.get("time_units", None) == "BJD_TDB":
         astropy_times = Time(dataset[k].data, format="mjd", scale="tdb")
         rainbow.set_times_from_astropy(astropy_times, is_barycentric=True)
         cheerfully_suggest(
             f"""
         Times are being estimated from the 'BJD_TDB'
         keyword but being interpreted as "modified"
         BJD_TDB ("modified" = BJD_TDB - 2400000.5).
@@ -76,15 +77,15 @@
         the fact that they're modified.
 
         If we're interpreting times wrongly, please
         raise an issue on the chromatic github!
         """
         )
     else:
-        t_unit = u.Unit(dataset[k].attrs["time_units"])
+        t_unit = u.Unit(dataset[k].attrs.get("time_units", "day"))
         t_without_unit = dataset[k].data
         rainbow.timelike["time"] = t_without_unit * t_unit
     keys_used.append(k)
 
     # populate a 2D (row = wavelength, col = time) array of fluxes
     for k in dataset.data_vars.keys():
         shape = dataset[k].shape
```

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/eureka_txt.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/eureka_txt.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/feinstein.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/feinstein.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/kirk.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/kirk.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/nres.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/nres.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/radica.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/radica.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/rainbow_FITS.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/rainbow_FITS.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/rainbow_npy.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/rainbow_npy.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/schlawin.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/schlawin.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/template.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/template.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/text.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/text.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/x1dints.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/x1dints.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,15 +232,15 @@
                     n_orders = 1
 
                 if order is None:
                     order = 1
                     if n_orders > 1:
                         cheerfully_suggest(
                             f"""
-                        This file contains data for {n_orders} spectrosopic orders. Because no
+                        This file contains data for {n_orders} spectroscopic orders. Because no
                         `order=` keyword was supplied, we're defaulting to first order. You can
                         hide this warning by expliciting stating which order you want to load.
                         For this file, the options include {np.arange(n_orders) + 1}.
                         """
                         )
                 assert (order >= 1) and (order <= n_orders)
```

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/x1dints_kludge.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/x1dints_kludge.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/xarray_fitted_light_curves.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/xarray_fitted_light_curves.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/xarray_raw_light_curves.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/xarray_raw_light_curves.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/readers/xarray_stellar_spectra.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/readers/xarray_stellar_spectra.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/simulated.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/simulated.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/animate.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/animate.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/colors.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/colors.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/descriptions.txt` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/descriptions.txt`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/diagnostics/histogram.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/diagnostics/histogram.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/diagnostics/imshow_quantities.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/diagnostics/imshow_quantities.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/diagnostics/plot_quantities.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/diagnostics/plot_quantities.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/imshow.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/imshow.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,18 +87,23 @@
         {len(self.wavelike.get('wavelength_lower', []))} wavelength edges defined.
 
         It's hard to imshow something with a wavelength axis
         that isn't linearly or logarithmically uniform, or doesn't
         at least have its wavelength edges defined. We're giving up
         and just using the wavelength index as the wavelength axis.
 
-        If you want a real wavelength axis, one solution would
-        be to bin your wavelengths to a more uniform grid with
-        `rainbow.bin(R=...)` (for logarithmic wavelengths) or
-        `rainbow.bin(dw=...)` (for linear wavelengths)
+        If you want a real wavelength axis, one solution would be
+        to use `rainbow.pcolormesh()` instead of `rainbow.imshow()`.
+        It takes basically the same inputs but can handle non-uniform
+        grids.
+
+        Or, you could bin your wavelengths to a more uniform grid with
+        `binned = rainbow.bin(R=...)` (for logarithmic wavelengths)
+        or `binned = rainbow.bin(dw=...)` (for linear wavelengths)
+        and then `binned.imshow()` will give more informative axes.
         """
         cheerfully_suggest(message)
         wlower, wupper = -0.5, self.nwave - 0.5
         wlabel = "Wavelength Index"
 
     # set up the time extent
     try:
@@ -121,17 +126,22 @@
         {len(self.timelike.get('time_lower', []))} time edges defined.
 
         It's hard to imshow something with a time axis
         that isn't linearly or logarithmically uniform, or doesn't
         at least have its time edges defined. We're giving up
         and just using the time index as the time axis.
 
-        If you want a real time axis, one solution would
-        be to bin your times to a more uniform grid with
-        `rainbow.bin(dt=...)` (for linear times).
+        If you want a real time axis, one solution would be
+        to use `rainbow.pcolormesh()` instead of `rainbow.imshow()`.
+        It takes basically the same inputs but can handle non-uniform
+        grids.
+
+        Or, you could bin your times to a more uniform grid with
+        `binned = rainbow.bin(dt=...)` (for linear times) and then
+        `binned.imshow()` will give more informative axes.
         """
         cheerfully_suggest(message)
         tlower, tupper = -0.5, self.ntime - 0.5
         tlabel = "Time Index"
 
     def get_2D(k):
         """
```

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/interactive.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/interactive.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/models/imshow_with_models.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/models/imshow_with_models.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/models/plot_one_wavelength_with_models.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/models/plot_one_wavelength_with_models.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/models/plot_with_model.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/models/plot_with_model.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/pcolormesh.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/pcolormesh.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/plot.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/plot.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/plot_lightcurves.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/plot_lightcurves.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/plot_spectra.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/plot_spectra.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/timelike/average_lightcurve.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/timelike/average_lightcurve.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/timelike/median_lightcurve.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/timelike/median_lightcurve.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/utilities.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/utilities.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/wavelike/average_spectrum.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/wavelike/average_spectrum.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/wavelike/median_spectrum.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/wavelike/median_spectrum.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/wavelike/noise_comparison.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/wavelike/noise_comparison.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/wavelike/noise_comparison_in_bins.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/wavelike/noise_comparison_in_bins.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/visualizations/wavelike/spectral_resolution.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/visualizations/wavelike/spectral_resolution.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/withmodel.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/withmodel.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/writers/__init__.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/writers/__init__.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/writers/rainbow_FITS.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/writers/rainbow_FITS.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/writers/rainbow_npy.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/writers/rainbow_npy.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/writers/template.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/writers/template.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/writers/text.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/writers/text.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/writers/xarray_fitted_light_curves.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/writers/xarray_fitted_light_curves.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/writers/xarray_raw_light_curves.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/writers/xarray_raw_light_curves.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/rainbows/writers/xarray_stellar_spectra.py` & `chromatic-lightcurves-0.4.7/chromatic/rainbows/writers/xarray_stellar_spectra.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/resampling.py` & `chromatic-lightcurves-0.4.7/chromatic/resampling.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/spectra/phoenix.py` & `chromatic-lightcurves-0.4.7/chromatic/spectra/phoenix.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/spectra/planck.py` & `chromatic-lightcurves-0.4.7/chromatic/spectra/planck.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/tests/__init__.py` & `chromatic-lightcurves-0.4.7/chromatic/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/tests/test_align_wavelengths.py` & `chromatic-lightcurves-0.4.7/chromatic/tests/test_align_wavelengths.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/tests/test_basics.py` & `chromatic-lightcurves-0.4.7/chromatic/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/tests/test_binning.py` & `chromatic-lightcurves-0.4.7/chromatic/tests/test_binning.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/tests/test_conversions.py` & `chromatic-lightcurves-0.4.7/chromatic/tests/test_conversions.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/tests/test_fold.py` & `chromatic-lightcurves-0.4.7/chromatic/tests/test_fold.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/tests/test_history.py` & `chromatic-lightcurves-0.4.7/chromatic/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/tests/test_io.py` & `chromatic-lightcurves-0.4.7/chromatic/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/tests/test_multi.py` & `chromatic-lightcurves-0.4.7/chromatic/tests/test_multi.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/tests/test_normalize.py` & `chromatic-lightcurves-0.4.7/chromatic/tests/test_normalize.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,38 @@
             r.fluxlike["relative-uncertainty"] = r.uncertainty / r.flux
             assert np.all(np.isclose(r.uncertainty / r.flux, 1 / snr, rtol=0.1))
             if plot:
                 r.imshow_quantities(maxcol=4)
     plt.close("all")
 
 
+def test_normalization_negative_warnings():
+    snr = 0.1
+    rainbow = SimulatedRainbow().inject_noise(signal_to_noise=0.1)
+
+    with pytest.warns(match="get_median_spectrum"):
+        rainbow.normalize(axis="wavelength")
+    ok = rainbow.get_median_spectrum() > 0
+    rainbow[ok, :].normalize(axis="wavelength")
+
+    with pytest.warns(match="get_median_lightcurve"):
+        rainbow.normalize(axis="time")
+    ok = rainbow.get_median_lightcurve() > 0
+    rainbow[:, ok].normalize(axis="time")
+
+
+def test_normalization_with_not_ok():
+    snr = 0.1
+    rainbow = SimulatedRainbow().inject_noise(signal_to_noise=0.1)
+    rainbow.ok = rainbow.flux > 0
+    with warnings.catch_warnings():
+        warnings.simplefilter("error")
+        rainbow.normalize()
+
+
 def test_is_probably_normalized():
     f = [2] * u.W / u.m**2
     kw = dict(star_flux=f, R=10, dt=10 * u.minute)
     assert SimulatedRainbow(**kw)._is_probably_normalized() == False
     assert SimulatedRainbow(**kw).normalize()._is_probably_normalized() == True
     assert SimulatedRainbow(**kw).inject_noise()._is_probably_normalized() == False
     assert (
```

### Comparing `chromatic-lightcurves-0.4.5/chromatic/tests/test_ok.py` & `chromatic-lightcurves-0.4.7/chromatic/tests/test_ok.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/tests/test_operations.py` & `chromatic-lightcurves-0.4.7/chromatic/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/tests/test_outliers.py` & `chromatic-lightcurves-0.4.7/chromatic/tests/test_outliers.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/tests/test_remove_trends.py` & `chromatic-lightcurves-0.4.7/chromatic/tests/test_remove_trends.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/tests/test_resampling.py` & `chromatic-lightcurves-0.4.7/chromatic/tests/test_resampling.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/tests/test_shift.py` & `chromatic-lightcurves-0.4.7/chromatic/tests/test_shift.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/tests/test_simulations.py` & `chromatic-lightcurves-0.4.7/chromatic/tests/test_simulations.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/tests/test_spectra.py` & `chromatic-lightcurves-0.4.7/chromatic/tests/test_spectra.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/tests/test_summaries.py` & `chromatic-lightcurves-0.4.7/chromatic/tests/test_summaries.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/tests/test_visualizations.py` & `chromatic-lightcurves-0.4.7/chromatic/tests/test_visualizations.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/tests/test_withmodel.py` & `chromatic-lightcurves-0.4.7/chromatic/tests/test_withmodel.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic/units.py` & `chromatic-lightcurves-0.4.7/chromatic/units.py`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/chromatic_lightcurves.egg-info/PKG-INFO` & `chromatic-lightcurves-0.4.7/chromatic_lightcurves.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromatic-lightcurves
-Version: 0.4.5
+Version: 0.4.7
 Summary: Tools for working with spectroscopic light curves (of transiting exoplanets).
 Home-page: https://github.com/zkbt/chromatic
 Author: Zach Berta-Thompson
 Author-email: zach.bertathompson@colorado.edu
 License: MIT
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `chromatic-lightcurves-0.4.5/chromatic_lightcurves.egg-info/SOURCES.txt` & `chromatic-lightcurves-0.4.7/chromatic_lightcurves.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 chromatic/rainbows/actions/operations.py
 chromatic/rainbows/actions/remove_trends.py
 chromatic/rainbows/actions/shift.py
 chromatic/rainbows/actions/trim.py
 chromatic/rainbows/converters/__init__.py
 chromatic/rainbows/converters/for_altair.py
 chromatic/rainbows/get/__init__.py
+chromatic/rainbows/get/fluxlike/__init__.py
+chromatic/rainbows/get/fluxlike/subset.py
 chromatic/rainbows/get/timelike/__init__.py
 chromatic/rainbows/get/timelike/average_lightcurve.py
 chromatic/rainbows/get/timelike/descriptions.txt
 chromatic/rainbows/get/timelike/median_lightcurve.py
 chromatic/rainbows/get/timelike/subset.py
 chromatic/rainbows/get/timelike/time.py
 chromatic/rainbows/get/wavelike/__init__.py
@@ -55,14 +57,15 @@
 chromatic/rainbows/helpers/descriptions.txt
 chromatic/rainbows/helpers/get.py
 chromatic/rainbows/helpers/help.py
 chromatic/rainbows/helpers/history.py
 chromatic/rainbows/helpers/save.py
 chromatic/rainbows/readers/__init__.py
 chromatic/rainbows/readers/atoca.py
+chromatic/rainbows/readers/aylin.py
 chromatic/rainbows/readers/coulombe.py
 chromatic/rainbows/readers/dossantos.py
 chromatic/rainbows/readers/espinoza.py
 chromatic/rainbows/readers/eureka_channels.py
 chromatic/rainbows/readers/eureka_lcdata.py
 chromatic/rainbows/readers/eureka_specdata.py
 chromatic/rainbows/readers/eureka_txt.py
```

### Comparing `chromatic-lightcurves-0.4.5/docs/actions.ipynb` & `chromatic-lightcurves-0.4.7/docs/actions.ipynb`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/docs/api.md` & `chromatic-lightcurves-0.4.7/docs/api.md`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/docs/basics.ipynb` & `chromatic-lightcurves-0.4.7/docs/basics.ipynb`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/docs/creating.ipynb` & `chromatic-lightcurves-0.4.7/docs/creating.ipynb`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/docs/designing.ipynb` & `chromatic-lightcurves-0.4.7/docs/designing.ipynb`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/docs/documentation.ipynb` & `chromatic-lightcurves-0.4.7/docs/documentation.ipynb`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/docs/example-timeseries-spectra.ipynb` & `chromatic-lightcurves-0.4.7/docs/example-timeseries-spectra.ipynb`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/docs/github.ipynb` & `chromatic-lightcurves-0.4.7/docs/github.ipynb`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/docs/index.md` & `chromatic-lightcurves-0.4.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/docs/installation.ipynb` & `chromatic-lightcurves-0.4.7/docs/installation.ipynb`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/docs/io.ipynb` & `chromatic-lightcurves-0.4.7/docs/io.ipynb`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/docs/models.ipynb` & `chromatic-lightcurves-0.4.7/docs/models.ipynb`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/docs/multi.ipynb.ignore` & `chromatic-lightcurves-0.4.7/docs/multi.ipynb.ignore`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/docs/quickstart.ipynb` & `chromatic-lightcurves-0.4.7/docs/quickstart.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9976310483870967%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(0, '## 💾 Download\\n')], delete: [0]}}, 5: {'source': "*

 * *            "{insert: [(0, '## 🧑\\u200d💻 Read\\n')], delete: [0]}}, 12: {'source': ['## 🧮 "*

 * *            'Calculate\']}, 24: {\'source\': ["What a dataset! It looks like there\'s something a '*

 * *            'little odd happening at about 2 microns (probably [contamination from another star or '*

 * *            'spectrograph '*

 * *            'order](https://jwst-docs.stsci.edu/jwst-near-infrared-imager-and-slitless-spectrogr […]*

```diff
@@ -33,15 +33,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "7a3ce2f3",
             "metadata": {},
             "source": [
-                "## \ud83d\udcbe Download Data\n",
+                "## \ud83d\udcbe Download\n",
                 "Let's download the [JWST Early Release Observation of HAT-P-18b](https://www.stsci.edu/jwst/science-execution/approved-programs/webb-first-image-observations), one of first exoplanet transit datasets to be gathered by the telescope. We'll get the default pipeline `x1dints` (Stage 3) outputs; there are lots of reasons why we shouldn't use these particular pipeline files for science, but they're useful for a quick initial look."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "5e9439e7",
@@ -54,15 +54,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "2e0b64f2",
             "metadata": {},
             "source": [
-                "## \ud83e\uddd1\u200d\ud83d\udcbb Load Data\n",
+                "## \ud83e\uddd1\u200d\ud83d\udcbb Read\n",
                 "Next, let's load that transit dataset into a `Rainbow` (\ud83c\udf08) object. These `chromatic` \ud83c\udf08 objects keep track of how the brightness of source changes across both wavelength and time."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e6f42847",
@@ -123,15 +123,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "030ad243",
             "metadata": {},
             "source": [
-                "## \ud83e\uddee Do Basic Calculations"
+                "## \ud83e\uddee Calculate"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "a9760f54",
             "metadata": {},
             "source": [
@@ -229,23 +229,23 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "5cf32700",
             "metadata": {},
             "source": [
-                "What a dataset! It looks like there's something a little odd happening at about 2 microns (probably [contamination from another star or spectrograph order](https://jwst-docs.stsci.edu/jwst-near-infrared-imager-and-slitless-spectrograph/niriss-features-and-caveats) and a starspot crossing just after mid-transit, but otherwise it's a remarkably beautiful transit from a very impressive telescope!"
+                "What a dataset! It looks like there's something a little odd happening at about 2 microns (probably [contamination from another star or spectrograph order](https://jwst-docs.stsci.edu/jwst-near-infrared-imager-and-slitless-spectrograph/niriss-features-and-caveats)) and a starspot crossing just after mid-transit, but otherwise it's a remarkably beautiful transit from a very impressive telescope!"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "4e55a26d",
             "metadata": {},
             "source": [
-                "## \ud83e\uddf6 String Actions Together\n",
+                "## \ud83e\uddf6 Build\n",
                 "Because many of the actions possible with \ud83c\udf08 objects return other \ud83c\udf08 objects, it's possible to connect multiple steps into a single command, building up complicated analysis stories with relatively succinct code."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "7cfe9a49",
@@ -262,15 +262,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "143156f5",
             "metadata": {},
             "source": [
-                "## \ud83d\udcbe Save Data\n",
+                "## \ud83d\udcbe Save\n",
                 "\n",
                 "Let's convert these data into a different format by saving it as a new file, which we might send around to share with our colleagues or publish along with a paper. `chromatic` can read and save \ud83c\udf08 datasets with a variety of formats, to try to ease collaboration across different pipelines and toolkits."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -282,15 +282,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "23aa7da8",
             "metadata": {},
             "source": [
-                "## \ud83d\udcda Learn More\n",
+                "## \ud83d\udcda Learn\n",
                 "\n",
                 "That's it! This quick tutorial highlighted `chromatic`'s abilities to...\n",
                 "- load in time-series spectra or multiwavelength light curves from formats like `x1dints`\n",
                 "- access core data variables like `wavelength`, `time`, `flux`, `uncertainty`\n",
                 "- perform calculations like `.normalize`, `.bin`, `.fold` \n",
                 "- visualize the data with `.imshow`, `.imshow_interact`, `.plot`\n",
                 "\n",
```

### Comparing `chromatic-lightcurves-0.4.5/docs/tools/binning.ipynb` & `chromatic-lightcurves-0.4.7/docs/tools/binning.ipynb`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/docs/tools/colormaps.ipynb` & `chromatic-lightcurves-0.4.7/docs/tools/colormaps.ipynb`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/docs/tools/spectra.ipynb` & `chromatic-lightcurves-0.4.7/docs/tools/spectra.ipynb`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/docs/visualizing.ipynb` & `chromatic-lightcurves-0.4.7/docs/visualizing.ipynb`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/mkdocs.yml` & `chromatic-lightcurves-0.4.7/mkdocs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -53,13 +53,15 @@
       custom_templates: templates
       watch:
         - chromatic
   - exclude:
       glob:
         - "example-datasets/*"
         - "*.pdf"
+        - "*.fits"
+        - "*.npy"
 markdown_extensions:
     - toc:
         permalink: "#"
 
 # this is super borrowed from Christina Hedges' fabulous
 # https://christinahedges.github.io/astronomy_workflow/
```

### Comparing `chromatic-lightcurves-0.4.5/notes/how-to-do-pre-commit.md` & `chromatic-lightcurves-0.4.7/notes/how-to-do-pre-commit.md`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/notes/how-to-do-the-docs.md` & `chromatic-lightcurves-0.4.7/notes/how-to-do-the-docs.md`

 * *Files identical despite different names*

### Comparing `chromatic-lightcurves-0.4.5/setup.py` & `chromatic-lightcurves-0.4.7/setup.py`

 * *Files identical despite different names*

