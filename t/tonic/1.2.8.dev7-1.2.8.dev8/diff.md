# Comparing `tmp/tonic-1.2.8.dev7.tar.gz` & `tmp/tonic-1.2.8.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonic-1.2.8.dev7.tar", last modified: Tue Jun 20 23:24:32 2023, max compression
+gzip compressed data, was "tonic-1.2.8.dev8.tar", last modified: Wed Jun 21 10:38:20 2023, max compression
```

## Comparing `tonic-1.2.8.dev7.tar` & `tonic-1.2.8.dev8.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.847335 tonic-1.2.8.dev7/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.827335 tonic-1.2.8.dev7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.827335 tonic-1.2.8.dev7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/.github/workflows/ci-pipeline.yml
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-20 23:24:32.000000 tonic-1.2.8.dev7/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    39687 2023-06-20 23:24:32.000000 tonic-1.2.8.dev7/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-06-20 23:24:32.847335 tonic-1.2.8.dev7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.827335 tonic-1.2.8.dev7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.831335 tonic-1.2.8.dev7/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.831335 tonic-1.2.8.dev7/docs/_static/event-cameras/
--rw-r--r--   0 runner    (1001) docker     (123)   460683 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/_static/event-cameras/eventstream.png
--rw-r--r--   0 runner    (1001) docker     (123)   209036 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/_static/event-cameras/framestream.png
--rw-r--r--   0 runner    (1001) docker     (123)    28336 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/_static/event-cameras/receptive-fields.png
--rw-r--r--   0 runner    (1001) docker     (123)    18392 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/_static/event-cameras/sampling-theorems.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.831335 tonic-1.2.8.dev7/docs/_static/snn/
--rw-r--r--   0 runner    (1001) docker     (123)   119778 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/_static/snn/neuron-models.png
--rw-r--r--   0 runner    (1001) docker     (123)    62505 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/_static/snn/surrogates.png
--rw-r--r--   0 runner    (1001) docker     (123)   196968 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/_static/tonic-logo-black.png
--rw-r--r--   0 runner    (1001) docker     (123)   193807 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/_static/tonic-logo-white.png
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/_static/tonic_favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.831335 tonic-1.2.8.dev7/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/_templates/class_dataset.rst
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/_templates/class_transform.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.831335 tonic-1.2.8.dev7/docs/about/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/about/about.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/about/info.rst
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/about/prototype.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/about/release_notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/datasets.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.831335 tonic-1.2.8.dev7/docs/gallery/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.831335 tonic-1.2.8.dev7/docs/gallery/representations/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/representations/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/representations/plot_tobinarep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/representations/plot_toframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/representations/plot_toimage.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/representations/plot_totimesurface.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/representations/plot_tovoxelgrid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.835335 tonic-1.2.8.dev7/docs/gallery/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_centercrop.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_crop_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_decimation.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_denoise.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_downsample.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_drop_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_drop_event_by_area.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_drop_event_by_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_drop_pixel.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_merge_polarities.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_random_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_random_flip_lr.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_random_flip_ud.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_random_time_reversal.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_refractory_period.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_spatial_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_time_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_uniform_noise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.835335 tonic-1.2.8.dev7/docs/getting_involved/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/getting_involved/communication_channels.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/getting_involved/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/getting_involved/getting_involved.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.835335 tonic-1.2.8.dev7/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/getting_started/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/getting_started/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/getting_started/nmnist.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.835335 tonic-1.2.8.dev7/docs/how-tos/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/how-tos/how-tos.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/how-tos/loading-raw-events.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/how-tos/visualizing-data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/how-tos/wrapping_own_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.835335 tonic-1.2.8.dev7/docs/reading_material/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/reading_material/design_choices.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11178 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/reading_material/intro-event-cameras.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/reading_material/intro-snns.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/reading_material/reading_material.rst
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/reading_material/training-snns.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/transformations.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.835335 tonic-1.2.8.dev7/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/tutorials/batching.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/tutorials/davis_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/tutorials/fast_dataloading.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/tutorials/large_datasets.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/tutorials/slicing.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/tutorials/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-20 23:24:32.847335 tonic-1.2.8.dev7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.835335 tonic-1.2.8.dev7/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/prototype_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/test_audio_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/test_chained_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.839335 tonic-1.2.8.dev7/test/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)   949253 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/test_data/sample.aedat4
--rw-r--r--   0 runner    (1001) docker     (123)    16165 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/test_data/sample_ncars.dat
--rw-r--r--   0 runner    (1001) docker     (123)    21625 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/test_data/sample_nmnist.bin
--rw-r--r--   0 runner    (1001) docker     (123)    38132 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/test_data/sample_stmnist.mat
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/test_dsec.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    10029 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/test_prototype_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/test_representations.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/test_sliced_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/test_slicers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/test_tonic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18669 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.839335 tonic-1.2.8.dev7/tonic/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/audio_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/cached_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/collation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.843335 tonic-1.2.8.dev7/tonic/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/datasets/asl_dvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/datasets/cifar10dvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/datasets/davisdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14707 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/datasets/dsec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/datasets/dvs_lips.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/datasets/dvsgesture.py
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/datasets/hsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/datasets/mvsec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/datasets/ncaltech101.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/datasets/nmnist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/datasets/pokerdvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/datasets/s_mnist.py
--rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/datasets/tum_vie.py
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/datasets/visual_place_recognition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/download_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.843335 tonic-1.2.8.dev7/tonic/functional/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/functional/crop.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/functional/decimate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/functional/denoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/functional/drop_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/functional/drop_pixel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/functional/refractory_period.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/functional/spatial_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/functional/time_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/functional/time_skew.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/functional/to_averaged_timesurface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/functional/to_bina_rep.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/functional/to_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/functional/to_timesurface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/functional/to_voxel_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/functional/uniform_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.843335 tonic-1.2.8.dev7/tonic/prototype/
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/prototype/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/prototype/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.843335 tonic-1.2.8.dev7/tonic/prototype/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/prototype/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/prototype/datasets/ncars.py
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/prototype/datasets/nmnist.py
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/prototype/datasets/prophesee.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/prototype/datasets/stmnist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.847335 tonic-1.2.8.dev7/tonic/prototype/datasets/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/prototype/datasets/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/prototype/datasets/utils/_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/prototype/datasets/utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/prototype/slicers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/sliced_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/slicers.py
--rw-r--r--   0 runner    (1001) docker     (123)    38208 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   212526 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic-logo-padded.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.843335 tonic-1.2.8.dev7/tonic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-06-20 23:24:32.000000 tonic-1.2.8.dev7/tonic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-06-20 23:24:32.000000 tonic-1.2.8.dev7/tonic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 23:24:32.000000 tonic-1.2.8.dev7/tonic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 23:24:32.000000 tonic-1.2.8.dev7/tonic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-20 23:24:32.000000 tonic-1.2.8.dev7/tonic.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-20 23:24:32.000000 tonic-1.2.8.dev7/tonic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 23:24:32.000000 tonic-1.2.8.dev7/tonic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.996976 tonic-1.2.8.dev8/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.980976 tonic-1.2.8.dev8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.980976 tonic-1.2.8.dev8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/.github/workflows/ci-pipeline.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-21 10:38:19.000000 tonic-1.2.8.dev8/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    39739 2023-06-21 10:38:19.000000 tonic-1.2.8.dev8/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-06-21 10:38:19.996976 tonic-1.2.8.dev8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.984976 tonic-1.2.8.dev8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.984976 tonic-1.2.8.dev8/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.984976 tonic-1.2.8.dev8/docs/_static/event-cameras/
+-rw-r--r--   0 runner    (1001) docker     (123)   460683 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/_static/event-cameras/eventstream.png
+-rw-r--r--   0 runner    (1001) docker     (123)   209036 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/_static/event-cameras/framestream.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28336 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/_static/event-cameras/receptive-fields.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18392 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/_static/event-cameras/sampling-theorems.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.984976 tonic-1.2.8.dev8/docs/_static/snn/
+-rw-r--r--   0 runner    (1001) docker     (123)   119778 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/_static/snn/neuron-models.png
+-rw-r--r--   0 runner    (1001) docker     (123)    62505 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/_static/snn/surrogates.png
+-rw-r--r--   0 runner    (1001) docker     (123)   196968 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/_static/tonic-logo-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)   193807 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/_static/tonic-logo-white.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/_static/tonic_favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.984976 tonic-1.2.8.dev8/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/_templates/class_dataset.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/_templates/class_transform.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.984976 tonic-1.2.8.dev8/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/about/about.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/about/info.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/about/prototype.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/about/release_notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/datasets.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.984976 tonic-1.2.8.dev8/docs/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.984976 tonic-1.2.8.dev8/docs/gallery/representations/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/representations/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/representations/plot_tobinarep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/representations/plot_toframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/representations/plot_toimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/representations/plot_totimesurface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/representations/plot_tovoxelgrid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.988976 tonic-1.2.8.dev8/docs/gallery/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_centercrop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_crop_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_decimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_denoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_downsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_drop_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_drop_event_by_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_drop_event_by_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_drop_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_merge_polarities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_random_flip_lr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_random_flip_ud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_random_time_reversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_refractory_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_spatial_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_time_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/gallery/transformations/plot_uniform_noise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.988976 tonic-1.2.8.dev8/docs/getting_involved/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/getting_involved/communication_channels.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/getting_involved/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/getting_involved/getting_involved.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.988976 tonic-1.2.8.dev8/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/getting_started/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/getting_started/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/getting_started/nmnist.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.988976 tonic-1.2.8.dev8/docs/how-tos/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/how-tos/how-tos.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/how-tos/loading-raw-events.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/how-tos/visualizing-data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/how-tos/wrapping_own_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.988976 tonic-1.2.8.dev8/docs/reading_material/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/reading_material/design_choices.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11178 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/reading_material/intro-event-cameras.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/reading_material/intro-snns.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/reading_material/reading_material.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/reading_material/training-snns.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/transformations.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.988976 tonic-1.2.8.dev8/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/tutorials/batching.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/tutorials/davis_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/tutorials/fast_dataloading.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/tutorials/large_datasets.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/tutorials/slicing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/docs/tutorials/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-21 10:38:19.996976 tonic-1.2.8.dev8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.992976 tonic-1.2.8.dev8/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/prototype_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/test_audio_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/test_chained_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.992976 tonic-1.2.8.dev8/test/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   949253 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/test_data/sample.aedat4
+-rw-r--r--   0 runner    (1001) docker     (123)    16165 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/test_data/sample_ncars.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    21625 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/test_data/sample_nmnist.bin
+-rw-r--r--   0 runner    (1001) docker     (123)    38132 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/test_data/sample_stmnist.mat
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/test_dsec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10029 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/test_prototype_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/test_representations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/test_sliced_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/test_slicers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/test_tonic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18669 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.992976 tonic-1.2.8.dev8/tonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/audio_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/cached_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/collation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.996976 tonic-1.2.8.dev8/tonic/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/datasets/asl_dvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/datasets/cifar10dvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/datasets/davisdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14707 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/datasets/dsec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/datasets/dvs_lips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/datasets/dvsgesture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/datasets/hsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/datasets/mvsec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/datasets/ncaltech101.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/datasets/nmnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/datasets/pokerdvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/datasets/s_mnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/datasets/tum_vie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/datasets/visual_place_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/download_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.996976 tonic-1.2.8.dev8/tonic/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/functional/crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/functional/decimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/functional/denoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/functional/drop_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/functional/drop_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/functional/refractory_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/functional/spatial_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/functional/time_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/functional/time_skew.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/functional/to_averaged_timesurface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/functional/to_bina_rep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/functional/to_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/functional/to_timesurface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/functional/to_voxel_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/functional/uniform_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.996976 tonic-1.2.8.dev8/tonic/prototype/
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/prototype/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/prototype/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.996976 tonic-1.2.8.dev8/tonic/prototype/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/prototype/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/prototype/datasets/ncars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/prototype/datasets/nmnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/prototype/datasets/prophesee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/prototype/datasets/stmnist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.996976 tonic-1.2.8.dev8/tonic/prototype/datasets/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/prototype/datasets/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/prototype/datasets/utils/_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/prototype/datasets/utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/prototype/slicers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/sliced_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/slicers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38250 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   212526 2023-06-21 10:38:03.000000 tonic-1.2.8.dev8/tonic-logo-padded.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:38:19.992976 tonic-1.2.8.dev8/tonic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-06-21 10:38:19.000000 tonic-1.2.8.dev8/tonic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-06-21 10:38:19.000000 tonic-1.2.8.dev8/tonic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 10:38:19.000000 tonic-1.2.8.dev8/tonic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 10:38:19.000000 tonic-1.2.8.dev8/tonic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-21 10:38:19.000000 tonic-1.2.8.dev8/tonic.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-21 10:38:19.000000 tonic-1.2.8.dev8/tonic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 10:38:19.000000 tonic-1.2.8.dev8/tonic.egg-info/top_level.txt
```

### Comparing `tonic-1.2.8.dev7/.github/workflows/ci-pipeline.yml` & `tonic-1.2.8.dev8/.github/workflows/ci-pipeline.yml`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/AUTHORS` & `tonic-1.2.8.dev8/AUTHORS`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/ChangeLog` & `tonic-1.2.8.dev8/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 CHANGES
 =======
 
+* Compose takes into account empty event arrays now
 * update NMNIST prototype dataset and tests to make compatible with Python 3.11
 * test Python 3.11
 * simplify STMNIST prototype dataset, broke keep\_compressed option though
 * Add delta\_t as a parameter to time surface test
 * Remove print statements to evaluate correctness
 * Time surface returns time surfaces at interval
```

### Comparing `tonic-1.2.8.dev7/LICENSE.txt` & `tonic-1.2.8.dev8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/PKG-INFO` & `tonic-1.2.8.dev8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonic
-Version: 1.2.8.dev7
+Version: 1.2.8.dev8
 Summary: Neuromorphic datasets and transformations.
 Home-page: UNKNOWN
 Author: The Neuromorphs of Telluride
 Author-email: mail@lenzgregor.com
 License: GNU GPLv3
 Project-URL: Source code, https://github.com/neuromorphs/tonic
 Project-URL: Documentation, https://tonic.readthedocs.org
```

### Comparing `tonic-1.2.8.dev7/README.md` & `tonic-1.2.8.dev8/README.md`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/Makefile` & `tonic-1.2.8.dev8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/_static/event-cameras/eventstream.png` & `tonic-1.2.8.dev8/docs/_static/event-cameras/eventstream.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/_static/event-cameras/framestream.png` & `tonic-1.2.8.dev8/docs/_static/event-cameras/framestream.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/_static/event-cameras/receptive-fields.png` & `tonic-1.2.8.dev8/docs/_static/event-cameras/receptive-fields.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/_static/event-cameras/sampling-theorems.png` & `tonic-1.2.8.dev8/docs/_static/event-cameras/sampling-theorems.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/_static/snn/neuron-models.png` & `tonic-1.2.8.dev8/docs/_static/snn/neuron-models.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/_static/snn/surrogates.png` & `tonic-1.2.8.dev8/docs/_static/snn/surrogates.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/_static/tonic-logo-black.png` & `tonic-1.2.8.dev8/docs/_static/tonic-logo-black.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/_static/tonic-logo-white.png` & `tonic-1.2.8.dev8/docs/_static/tonic-logo-white.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/_static/tonic_favicon.png` & `tonic-1.2.8.dev8/docs/_static/tonic_favicon.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/about/info.rst` & `tonic-1.2.8.dev8/docs/about/info.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/about/prototype.rst` & `tonic-1.2.8.dev8/docs/about/prototype.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/about/release_notes.rst` & `tonic-1.2.8.dev8/docs/about/release_notes.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/conf.py` & `tonic-1.2.8.dev8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/datasets.rst` & `tonic-1.2.8.dev8/docs/datasets.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/gallery/representations/plot_tobinarep.py` & `tonic-1.2.8.dev8/docs/gallery/representations/plot_tobinarep.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/gallery/representations/plot_toframe.py` & `tonic-1.2.8.dev8/docs/gallery/representations/plot_toframe.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/gallery/representations/plot_toimage.py` & `tonic-1.2.8.dev8/docs/gallery/representations/plot_toimage.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/gallery/representations/plot_totimesurface.py` & `tonic-1.2.8.dev8/docs/gallery/representations/plot_totimesurface.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/gallery/transformations/plot_centercrop.py` & `tonic-1.2.8.dev8/docs/gallery/transformations/plot_centercrop.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/gallery/transformations/plot_crop_time.py` & `tonic-1.2.8.dev8/docs/gallery/transformations/plot_crop_time.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/gallery/transformations/plot_decimation.py` & `tonic-1.2.8.dev8/docs/gallery/transformations/plot_decimation.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/gallery/transformations/plot_denoise.py` & `tonic-1.2.8.dev8/docs/gallery/transformations/plot_denoise.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/gallery/transformations/plot_downsample.py` & `tonic-1.2.8.dev8/docs/gallery/transformations/plot_downsample.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/gallery/transformations/plot_drop_event.py` & `tonic-1.2.8.dev8/docs/gallery/transformations/plot_drop_event.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/gallery/transformations/plot_drop_event_by_area.py` & `tonic-1.2.8.dev8/docs/gallery/transformations/plot_drop_event_by_area.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/gallery/transformations/plot_drop_event_by_time.py` & `tonic-1.2.8.dev8/docs/gallery/transformations/plot_drop_event_by_time.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/gallery/transformations/plot_drop_pixel.py` & `tonic-1.2.8.dev8/docs/gallery/transformations/plot_drop_pixel.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/gallery/transformations/plot_merge_polarities.py` & `tonic-1.2.8.dev8/docs/gallery/transformations/plot_merge_polarities.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/gallery/transformations/plot_random_crop.py` & `tonic-1.2.8.dev8/docs/gallery/transformations/plot_random_crop.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/gallery/transformations/plot_random_flip_lr.py` & `tonic-1.2.8.dev8/docs/gallery/transformations/plot_random_flip_lr.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/gallery/transformations/plot_random_flip_ud.py` & `tonic-1.2.8.dev8/docs/gallery/transformations/plot_random_flip_ud.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/gallery/transformations/plot_random_time_reversal.py` & `tonic-1.2.8.dev8/docs/gallery/transformations/plot_random_time_reversal.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/gallery/transformations/plot_refractory_period.py` & `tonic-1.2.8.dev8/docs/gallery/transformations/plot_refractory_period.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/gallery/transformations/plot_spatial_jitter.py` & `tonic-1.2.8.dev8/docs/gallery/transformations/plot_spatial_jitter.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/gallery/transformations/plot_time_jitter.py` & `tonic-1.2.8.dev8/docs/gallery/transformations/plot_time_jitter.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/gallery/transformations/plot_uniform_noise.py` & `tonic-1.2.8.dev8/docs/gallery/transformations/plot_uniform_noise.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/getting_involved/communication_channels.rst` & `tonic-1.2.8.dev8/docs/getting_involved/communication_channels.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/getting_involved/contribute.rst` & `tonic-1.2.8.dev8/docs/getting_involved/contribute.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/getting_started/install.rst` & `tonic-1.2.8.dev8/docs/getting_started/install.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/getting_started/nmnist.ipynb` & `tonic-1.2.8.dev8/docs/getting_started/nmnist.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/how-tos/loading-raw-events.ipynb` & `tonic-1.2.8.dev8/docs/how-tos/loading-raw-events.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/how-tos/visualizing-data.ipynb` & `tonic-1.2.8.dev8/docs/how-tos/visualizing-data.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/how-tos/wrapping_own_data.ipynb` & `tonic-1.2.8.dev8/docs/how-tos/wrapping_own_data.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/index.md` & `tonic-1.2.8.dev8/docs/index.md`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/make.bat` & `tonic-1.2.8.dev8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/reading_material/design_choices.rst` & `tonic-1.2.8.dev8/docs/reading_material/design_choices.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/reading_material/intro-event-cameras.rst` & `tonic-1.2.8.dev8/docs/reading_material/intro-event-cameras.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/reading_material/intro-snns.rst` & `tonic-1.2.8.dev8/docs/reading_material/intro-snns.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/reading_material/training-snns.rst` & `tonic-1.2.8.dev8/docs/reading_material/training-snns.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/transformations.rst` & `tonic-1.2.8.dev8/docs/transformations.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/tutorials/batching.ipynb` & `tonic-1.2.8.dev8/docs/tutorials/batching.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/tutorials/davis_data.ipynb` & `tonic-1.2.8.dev8/docs/tutorials/davis_data.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/tutorials/fast_dataloading.ipynb` & `tonic-1.2.8.dev8/docs/tutorials/fast_dataloading.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/tutorials/large_datasets.ipynb` & `tonic-1.2.8.dev8/docs/tutorials/large_datasets.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/docs/tutorials/slicing.ipynb` & `tonic-1.2.8.dev8/docs/tutorials/slicing.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/setup.cfg` & `tonic-1.2.8.dev8/setup.cfg`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/test/dataset_utils.py` & `tonic-1.2.8.dev8/test/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/test/prototype_dataset_utils.py` & `tonic-1.2.8.dev8/test/prototype_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/test/test_audio_transforms.py` & `tonic-1.2.8.dev8/test/test_audio_transforms.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/test/test_caching.py` & `tonic-1.2.8.dev8/test/test_caching.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/test/test_chained_transforms.py` & `tonic-1.2.8.dev8/test/test_chained_transforms.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/test/test_data/sample.aedat4` & `tonic-1.2.8.dev8/test/test_data/sample.aedat4`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/test/test_data/sample_ncars.dat` & `tonic-1.2.8.dev8/test/test_data/sample_ncars.dat`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/test/test_data/sample_nmnist.bin` & `tonic-1.2.8.dev8/test/test_data/sample_nmnist.bin`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/test/test_data/sample_stmnist.mat` & `tonic-1.2.8.dev8/test/test_data/sample_stmnist.mat`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/test/test_datasets.py` & `tonic-1.2.8.dev8/test/test_datasets.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/test/test_dsec.py` & `tonic-1.2.8.dev8/test/test_dsec.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/test/test_io.py` & `tonic-1.2.8.dev8/test/test_io.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/test/test_prototype_datasets.py` & `tonic-1.2.8.dev8/test/test_prototype_datasets.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/test/test_representations.py` & `tonic-1.2.8.dev8/test/test_representations.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/test/test_sliced_dataset.py` & `tonic-1.2.8.dev8/test/test_sliced_dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/test/test_slicers.py` & `tonic-1.2.8.dev8/test/test_slicers.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/test/test_tonic_utils.py` & `tonic-1.2.8.dev8/test/test_tonic_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/test/test_transforms.py` & `tonic-1.2.8.dev8/test/test_transforms.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/test/utils.py` & `tonic-1.2.8.dev8/test/utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/audio_transforms.py` & `tonic-1.2.8.dev8/tonic/audio_transforms.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/cached_dataset.py` & `tonic-1.2.8.dev8/tonic/cached_dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/collation.py` & `tonic-1.2.8.dev8/tonic/collation.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/dataset.py` & `tonic-1.2.8.dev8/tonic/dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/datasets/__init__.py` & `tonic-1.2.8.dev8/tonic/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/datasets/asl_dvs.py` & `tonic-1.2.8.dev8/tonic/datasets/asl_dvs.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/datasets/cifar10dvs.py` & `tonic-1.2.8.dev8/tonic/datasets/cifar10dvs.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/datasets/davisdataset.py` & `tonic-1.2.8.dev8/tonic/datasets/davisdataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/datasets/dsec.py` & `tonic-1.2.8.dev8/tonic/datasets/dsec.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/datasets/dvs_lips.py` & `tonic-1.2.8.dev8/tonic/datasets/dvs_lips.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/datasets/dvsgesture.py` & `tonic-1.2.8.dev8/tonic/datasets/dvsgesture.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/datasets/hsd.py` & `tonic-1.2.8.dev8/tonic/datasets/hsd.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/datasets/mvsec.py` & `tonic-1.2.8.dev8/tonic/datasets/mvsec.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/datasets/ncaltech101.py` & `tonic-1.2.8.dev8/tonic/datasets/ncaltech101.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/datasets/nmnist.py` & `tonic-1.2.8.dev8/tonic/datasets/nmnist.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/datasets/pokerdvs.py` & `tonic-1.2.8.dev8/tonic/datasets/pokerdvs.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/datasets/s_mnist.py` & `tonic-1.2.8.dev8/tonic/datasets/s_mnist.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/datasets/tum_vie.py` & `tonic-1.2.8.dev8/tonic/datasets/tum_vie.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/datasets/visual_place_recognition.py` & `tonic-1.2.8.dev8/tonic/datasets/visual_place_recognition.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/download_utils.py` & `tonic-1.2.8.dev8/tonic/download_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/functional/__init__.py` & `tonic-1.2.8.dev8/tonic/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/functional/crop.py` & `tonic-1.2.8.dev8/tonic/functional/crop.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/functional/decimate.py` & `tonic-1.2.8.dev8/tonic/functional/decimate.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/functional/denoise.py` & `tonic-1.2.8.dev8/tonic/functional/denoise.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/functional/drop_event.py` & `tonic-1.2.8.dev8/tonic/functional/drop_event.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/functional/drop_pixel.py` & `tonic-1.2.8.dev8/tonic/functional/drop_pixel.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/functional/refractory_period.py` & `tonic-1.2.8.dev8/tonic/functional/refractory_period.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/functional/spatial_jitter.py` & `tonic-1.2.8.dev8/tonic/functional/spatial_jitter.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/functional/time_jitter.py` & `tonic-1.2.8.dev8/tonic/functional/time_jitter.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/functional/time_skew.py` & `tonic-1.2.8.dev8/tonic/functional/time_skew.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/functional/to_averaged_timesurface.py` & `tonic-1.2.8.dev8/tonic/functional/to_averaged_timesurface.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/functional/to_bina_rep.py` & `tonic-1.2.8.dev8/tonic/functional/to_bina_rep.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/functional/to_frame.py` & `tonic-1.2.8.dev8/tonic/functional/to_frame.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/functional/to_timesurface.py` & `tonic-1.2.8.dev8/tonic/functional/to_timesurface.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/functional/to_voxel_grid.py` & `tonic-1.2.8.dev8/tonic/functional/to_voxel_grid.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/functional/uniform_noise.py` & `tonic-1.2.8.dev8/tonic/functional/uniform_noise.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/io.py` & `tonic-1.2.8.dev8/tonic/io.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/prototype/README.md` & `tonic-1.2.8.dev8/tonic/prototype/README.md`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/prototype/datasets/ncars.py` & `tonic-1.2.8.dev8/tonic/prototype/datasets/ncars.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/prototype/datasets/nmnist.py` & `tonic-1.2.8.dev8/tonic/prototype/datasets/nmnist.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/prototype/datasets/prophesee.py` & `tonic-1.2.8.dev8/tonic/prototype/datasets/prophesee.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/prototype/datasets/stmnist.py` & `tonic-1.2.8.dev8/tonic/prototype/datasets/stmnist.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/prototype/datasets/utils/_dataset.py` & `tonic-1.2.8.dev8/tonic/prototype/datasets/utils/_dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/prototype/datasets/utils/_utils.py` & `tonic-1.2.8.dev8/tonic/prototype/datasets/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/prototype/slicers.py` & `tonic-1.2.8.dev8/tonic/prototype/slicers.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/sliced_dataset.py` & `tonic-1.2.8.dev8/tonic/sliced_dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/slicers.py` & `tonic-1.2.8.dev8/tonic/slicers.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic/transforms.py` & `tonic-1.2.8.dev8/tonic/transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     """
 
     def __init__(self, transforms: Callable):
         self.transforms = transforms
 
     def __call__(self, events):
         for t in self.transforms:
+            if len(events) == 0:
+                break
             events = t(events)
         return events
 
     def __repr__(self):
         format_string = self.__class__.__name__ + "("
         for t in self.transforms:
             format_string += "\n"
@@ -174,15 +176,14 @@
     Example:
         >>> transform = tonic.transforms.DropEventByTime(duration_ratio=(0.1, 0.8))
     """
 
     duration_ratio: Union[float, Tuple[float, float]] = 0.2
 
     def __call__(self, events):
-
         return functional.drop_by_time_numpy(events, self.duration_ratio)
 
 
 @dataclass(frozen=True)
 class DropEventByArea:
     """Drops events located in a randomly chosen box area. The size of the box area is defined by a
     specified ratio of the sensor size.
@@ -198,15 +199,14 @@
         >>> transform = tonic.transforms.DropEventByArea(sensor_size=(128,128,2), area_ratio=(0.1, 0.8))
     """
 
     sensor_size: Tuple[int, int, int]
     area_ratio: Union[float, Tuple[float, float]] = 0.2
 
     def __call__(self, events):
-
         return functional.drop_by_area_numpy(events, self.sensor_size, self.area_ratio)
 
 
 @dataclass
 class DropPixel:
     """Drops events for individual pixels. If the locations of pixels to be dropped is known, a
     list of x/y coordinates can be passed directly. Alternatively, a cutoff frequency for each
@@ -346,15 +346,14 @@
         >>> transform = tonic.transforms.RandomCrop(sensor_size=(340, 240, 2), target_size=(50, 50))
     """
 
     sensor_size: Tuple[int, int, int]
     target_size: Tuple[int, int]
 
     def __call__(self, events):
-
         return functional.crop_numpy(
             events=events, sensor_size=self.sensor_size, target_size=self.target_size
         )
 
 
 @dataclass
 class RandomDropPixel:
@@ -757,18 +756,18 @@
         )
 
 
 @dataclass(frozen=True)
 class ToFrame:
     """Accumulate events to frames by slicing along constant time (time_window), constant number of
     events (spike_count) or constant number of frames (n_time_bins / n_event_bins). All the events
-    in one slice are added up in a frame for each polarity.  If you want binary frames, you can 
-    manually clamp them to 1 afterwards. You can set one of the first 4 parameters to choose the 
-    slicing method. Depending on which method you choose, overlap will be defined differently.
-    As a rule of thumb, here are some considerations if you are unsure which slicing method to choose:
+    in one slice are added up in a frame for each polarity.  If you want binary frames, you can
+    manually clamp them to 1 afterwards. You can set one of the first 4 parameters to choose the
+    slicing method. Depending on which method you choose, overlap will be defined differently. As a
+    rule of thumb, here are some considerations if you are unsure which slicing method to choose:
 
     * If your recordings are of roughly the same length, a safe option is to set time_window. Bare in mind
       that the number of events can vary greatly from slice to slice, but will give you some consistency when
       training RNNs or other algorithms that have time steps.
 
     * If your recordings have roughly the same amount of activity / number of events and you are more interested
       in the spatial composition, then setting spike_count will give you frames that are visually more consistent.
@@ -789,16 +788,16 @@
                              for every frame if the recording's activity is not consistent.
         spike_count (int): Number of events per frame. Good for training CNNs which do not care about temporal consistency.
         n_time_bins (int): Fixed number of frames, sliced along time axis. Good for generating a pre-determined number of
                            frames which might help with batching.
         n_event_bins (int): Fixed number of frames, sliced along number of events in the recording. Good for generating a
                             pre-determined number of frames which might help with batching.
         overlap (float): Overlap between frames. The definition of overlap depends on the slicing method.
-                         For slicing by time_window, the overlap is defined in microseconds. For slicing by spike_count, 
-                         the overlap is defined by number of events. For slicing by n_time_bins or n_event_bins, the 
+                         For slicing by time_window, the overlap is defined in microseconds. For slicing by spike_count,
+                         the overlap is defined by number of events. For slicing by n_time_bins or n_event_bins, the
                          overlap is defined by the fraction of a bin between 0 and 1.
         include_incomplete (bool): If True, includes overhang slice when time_window or spike_count is specified.
                                    Not valid for bin_count methods.
 
     Example:
         >>> from tonic.transforms import ToFrame
         >>> transform1 = ToFrame(time_window=10000, overlap=1000, include_incomplete=True)
@@ -811,15 +810,14 @@
     event_count: Optional[int] = None
     n_time_bins: Optional[int] = None
     n_event_bins: Optional[int] = None
     overlap: float = 0
     include_incomplete: bool = False
 
     def __call__(self, events):
-
         return functional.to_frame_numpy(
             events=events,
             sensor_size=self.sensor_size,
             time_window=self.time_window,
             event_count=self.event_count,
             n_time_bins=self.n_time_bins,
             n_event_bins=self.n_event_bins,
@@ -893,15 +891,14 @@
     ToImage will typically be used in combination with SlicedDataset to cut a recording into
     smaller chunks that are then individually binned to frames.
     """
 
     sensor_size: Tuple[int, int, int]
 
     def __call__(self, events):
-
         frames = functional.to_frame_numpy(
             events=events, sensor_size=self.sensor_size, event_count=len(events)
         )
 
         return frames.squeeze(0)
 
 
@@ -913,26 +910,25 @@
 
     Parameters:
         sensor_size: a 3-tuple of x,y,p for sensor_size
         surface_dimensions (int, int): width does not have to be equal to height, however both numbers have to be odd.
             if surface_dimensions is None: the time surface is defined globally, on the whole sensor grid.
         tau (float): time constant to decay events around occuring event with.
         delta_t (float): the interval at which the time-surfaces are accumulated, if set 0 number of time-surfaces will
-            equal to the number of events. (defaults to 0.0) 
+            equal to the number of events. (defaults to 0.0)
         decay (str): can be either 'lin' or 'exp', corresponding to linear or exponential decay.
     """
 
     sensor_size: Tuple[int, int, int]
     surface_dimensions: Union[None, Tuple[int, int]] = None
     tau: float = 5e3
     delta_t: float = 0.0
     decay: str = "lin"
 
     def __call__(self, events):
-
         return functional.to_timesurface_numpy(
             events=events,
             sensor_size=self.sensor_size,
             surface_dimensions=self.surface_dimensions,
             tau=self.tau,
             delta_t=self.delta_t,
             decay=self.decay,
@@ -950,15 +946,14 @@
         n_time_bins (int): fixed number of time bins to slice the event sample into.
     """
 
     sensor_size: Tuple[int, int, int]
     n_time_bins: int
 
     def __call__(self, events):
-
         return functional.to_voxel_grid_numpy(
             events.copy(), self.sensor_size, self.n_time_bins
         )
 
 
 @dataclass(frozen=True)
 class ToBinaRep:
@@ -987,15 +982,14 @@
         >>> ])
     """
 
     n_frames: Optional[int] = 1
     n_bits: Optional[int] = 8
 
     def __call__(self, event_frames):
-
         return functional.to_bina_rep_numpy(event_frames, self.n_frames, self.n_bits)
 
 
 @dataclass(frozen=True)
 class Repeat:
     """Copies target n times.
```

### Comparing `tonic-1.2.8.dev7/tonic/utils.py` & `tonic-1.2.8.dev8/tonic/utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic-logo-padded.png` & `tonic-1.2.8.dev8/tonic-logo-padded.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev7/tonic.egg-info/PKG-INFO` & `tonic-1.2.8.dev8/tonic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonic
-Version: 1.2.8.dev7
+Version: 1.2.8.dev8
 Summary: Neuromorphic datasets and transformations.
 Home-page: UNKNOWN
 Author: The Neuromorphs of Telluride
 Author-email: mail@lenzgregor.com
 License: GNU GPLv3
 Project-URL: Source code, https://github.com/neuromorphs/tonic
 Project-URL: Documentation, https://tonic.readthedocs.org
```

### Comparing `tonic-1.2.8.dev7/tonic.egg-info/SOURCES.txt` & `tonic-1.2.8.dev8/tonic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

