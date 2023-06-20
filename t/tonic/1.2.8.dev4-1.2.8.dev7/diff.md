# Comparing `tmp/tonic-1.2.8.dev4.tar.gz` & `tmp/tonic-1.2.8.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonic-1.2.8.dev4.tar", last modified: Tue Jun 20 10:37:25 2023, max compression
+gzip compressed data, was "tonic-1.2.8.dev7.tar", last modified: Tue Jun 20 23:24:32 2023, max compression
```

## Comparing `tonic-1.2.8.dev4.tar` & `tonic-1.2.8.dev7.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.778264 tonic-1.2.8.dev4/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.754264 tonic-1.2.8.dev4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.758264 tonic-1.2.8.dev4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/.github/workflows/ci-pipeline.yml
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-20 10:37:25.000000 tonic-1.2.8.dev4/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    39513 2023-06-20 10:37:25.000000 tonic-1.2.8.dev4/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-06-20 10:37:25.778264 tonic-1.2.8.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.762264 tonic-1.2.8.dev4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.762264 tonic-1.2.8.dev4/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.762264 tonic-1.2.8.dev4/docs/_static/event-cameras/
--rw-r--r--   0 runner    (1001) docker     (123)   460683 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/_static/event-cameras/eventstream.png
--rw-r--r--   0 runner    (1001) docker     (123)   209036 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/_static/event-cameras/framestream.png
--rw-r--r--   0 runner    (1001) docker     (123)    28336 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/_static/event-cameras/receptive-fields.png
--rw-r--r--   0 runner    (1001) docker     (123)    18392 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/_static/event-cameras/sampling-theorems.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.762264 tonic-1.2.8.dev4/docs/_static/snn/
--rw-r--r--   0 runner    (1001) docker     (123)   119778 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/_static/snn/neuron-models.png
--rw-r--r--   0 runner    (1001) docker     (123)    62505 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/_static/snn/surrogates.png
--rw-r--r--   0 runner    (1001) docker     (123)   196968 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/_static/tonic-logo-black.png
--rw-r--r--   0 runner    (1001) docker     (123)   193807 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/_static/tonic-logo-white.png
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/_static/tonic_favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.762264 tonic-1.2.8.dev4/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/_templates/class_dataset.rst
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/_templates/class_transform.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.762264 tonic-1.2.8.dev4/docs/about/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/about/about.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/about/info.rst
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/about/prototype.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/about/release_notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/datasets.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.762264 tonic-1.2.8.dev4/docs/gallery/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.766264 tonic-1.2.8.dev4/docs/gallery/representations/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/representations/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/representations/plot_tobinarep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/representations/plot_toframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/representations/plot_toimage.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/representations/plot_totimesurface.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/representations/plot_tovoxelgrid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.766264 tonic-1.2.8.dev4/docs/gallery/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_centercrop.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_crop_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_decimation.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_denoise.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_downsample.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_drop_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_drop_event_by_area.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_drop_event_by_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_drop_pixel.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_merge_polarities.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_random_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_random_flip_lr.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_random_flip_ud.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_random_time_reversal.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_refractory_period.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_spatial_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_time_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_uniform_noise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.766264 tonic-1.2.8.dev4/docs/getting_involved/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/getting_involved/communication_channels.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/getting_involved/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/getting_involved/getting_involved.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.766264 tonic-1.2.8.dev4/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/getting_started/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/getting_started/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/getting_started/nmnist.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.766264 tonic-1.2.8.dev4/docs/how-tos/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/how-tos/how-tos.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/how-tos/loading-raw-events.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/how-tos/visualizing-data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/how-tos/wrapping_own_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.766264 tonic-1.2.8.dev4/docs/reading_material/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/reading_material/design_choices.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11178 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/reading_material/intro-event-cameras.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/reading_material/intro-snns.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/reading_material/reading_material.rst
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/reading_material/training-snns.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/transformations.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.770264 tonic-1.2.8.dev4/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/tutorials/batching.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/tutorials/davis_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/tutorials/fast_dataloading.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/tutorials/large_datasets.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/tutorials/slicing.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/tutorials/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-20 10:37:25.778264 tonic-1.2.8.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.770264 tonic-1.2.8.dev4/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/prototype_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/test_audio_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/test_chained_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.770264 tonic-1.2.8.dev4/test/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)   949253 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/test_data/sample.aedat4
--rw-r--r--   0 runner    (1001) docker     (123)    16165 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/test_data/sample_ncars.dat
--rw-r--r--   0 runner    (1001) docker     (123)    21625 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/test_data/sample_nmnist.bin
--rw-r--r--   0 runner    (1001) docker     (123)    38132 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/test_data/sample_stmnist.mat
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/test_dsec.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/test_prototype_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/test_representations.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/test_sliced_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/test_slicers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/test_tonic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18669 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.774264 tonic-1.2.8.dev4/tonic/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/audio_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/cached_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/collation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.774264 tonic-1.2.8.dev4/tonic/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/datasets/asl_dvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/datasets/cifar10dvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/datasets/davisdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14707 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/datasets/dsec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/datasets/dvs_lips.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/datasets/dvsgesture.py
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/datasets/hsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/datasets/mvsec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/datasets/ncaltech101.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/datasets/nmnist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/datasets/pokerdvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/datasets/s_mnist.py
--rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/datasets/tum_vie.py
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/datasets/visual_place_recognition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/download_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.778264 tonic-1.2.8.dev4/tonic/functional/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/functional/crop.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/functional/decimate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/functional/denoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/functional/drop_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/functional/drop_pixel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/functional/refractory_period.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/functional/spatial_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/functional/time_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/functional/time_skew.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/functional/to_averaged_timesurface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/functional/to_bina_rep.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/functional/to_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/functional/to_timesurface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/functional/to_voxel_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/functional/uniform_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.778264 tonic-1.2.8.dev4/tonic/prototype/
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/prototype/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/prototype/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.778264 tonic-1.2.8.dev4/tonic/prototype/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/prototype/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/prototype/datasets/ncars.py
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/prototype/datasets/nmnist.py
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/prototype/datasets/prophesee.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/prototype/datasets/stmnist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.778264 tonic-1.2.8.dev4/tonic/prototype/datasets/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/prototype/datasets/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/prototype/datasets/utils/_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/prototype/datasets/utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/prototype/slicers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/sliced_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/slicers.py
--rw-r--r--   0 runner    (1001) docker     (123)    38208 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   212526 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic-logo-padded.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.774264 tonic-1.2.8.dev4/tonic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-06-20 10:37:25.000000 tonic-1.2.8.dev4/tonic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-06-20 10:37:25.000000 tonic-1.2.8.dev4/tonic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 10:37:25.000000 tonic-1.2.8.dev4/tonic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 10:37:25.000000 tonic-1.2.8.dev4/tonic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-20 10:37:25.000000 tonic-1.2.8.dev4/tonic.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-20 10:37:25.000000 tonic-1.2.8.dev4/tonic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 10:37:25.000000 tonic-1.2.8.dev4/tonic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.847335 tonic-1.2.8.dev7/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.827335 tonic-1.2.8.dev7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.827335 tonic-1.2.8.dev7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/.github/workflows/ci-pipeline.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-20 23:24:32.000000 tonic-1.2.8.dev7/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    39687 2023-06-20 23:24:32.000000 tonic-1.2.8.dev7/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-06-20 23:24:32.847335 tonic-1.2.8.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.827335 tonic-1.2.8.dev7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.831335 tonic-1.2.8.dev7/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.831335 tonic-1.2.8.dev7/docs/_static/event-cameras/
+-rw-r--r--   0 runner    (1001) docker     (123)   460683 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/_static/event-cameras/eventstream.png
+-rw-r--r--   0 runner    (1001) docker     (123)   209036 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/_static/event-cameras/framestream.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28336 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/_static/event-cameras/receptive-fields.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18392 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/_static/event-cameras/sampling-theorems.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.831335 tonic-1.2.8.dev7/docs/_static/snn/
+-rw-r--r--   0 runner    (1001) docker     (123)   119778 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/_static/snn/neuron-models.png
+-rw-r--r--   0 runner    (1001) docker     (123)    62505 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/_static/snn/surrogates.png
+-rw-r--r--   0 runner    (1001) docker     (123)   196968 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/_static/tonic-logo-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)   193807 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/_static/tonic-logo-white.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/_static/tonic_favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.831335 tonic-1.2.8.dev7/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/_templates/class_dataset.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/_templates/class_transform.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.831335 tonic-1.2.8.dev7/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/about/about.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/about/info.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/about/prototype.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/about/release_notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/datasets.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.831335 tonic-1.2.8.dev7/docs/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.831335 tonic-1.2.8.dev7/docs/gallery/representations/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/representations/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/representations/plot_tobinarep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/representations/plot_toframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/representations/plot_toimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/representations/plot_totimesurface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/representations/plot_tovoxelgrid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.835335 tonic-1.2.8.dev7/docs/gallery/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_centercrop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_crop_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_decimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_denoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_downsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_drop_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_drop_event_by_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_drop_event_by_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_drop_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_merge_polarities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_random_flip_lr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_random_flip_ud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_random_time_reversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_refractory_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_spatial_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_time_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/gallery/transformations/plot_uniform_noise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.835335 tonic-1.2.8.dev7/docs/getting_involved/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/getting_involved/communication_channels.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/getting_involved/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/getting_involved/getting_involved.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.835335 tonic-1.2.8.dev7/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/getting_started/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/getting_started/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/getting_started/nmnist.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.835335 tonic-1.2.8.dev7/docs/how-tos/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/how-tos/how-tos.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/how-tos/loading-raw-events.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/how-tos/visualizing-data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/how-tos/wrapping_own_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.835335 tonic-1.2.8.dev7/docs/reading_material/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/reading_material/design_choices.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11178 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/reading_material/intro-event-cameras.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/reading_material/intro-snns.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/reading_material/reading_material.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/reading_material/training-snns.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/transformations.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.835335 tonic-1.2.8.dev7/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/tutorials/batching.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/tutorials/davis_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/tutorials/fast_dataloading.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/tutorials/large_datasets.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/tutorials/slicing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/docs/tutorials/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-20 23:24:32.847335 tonic-1.2.8.dev7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.835335 tonic-1.2.8.dev7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/prototype_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/test_audio_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/test_chained_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.839335 tonic-1.2.8.dev7/test/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   949253 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/test_data/sample.aedat4
+-rw-r--r--   0 runner    (1001) docker     (123)    16165 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/test_data/sample_ncars.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    21625 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/test_data/sample_nmnist.bin
+-rw-r--r--   0 runner    (1001) docker     (123)    38132 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/test_data/sample_stmnist.mat
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/test_dsec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10029 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/test_prototype_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/test_representations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/test_sliced_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/test_slicers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/test_tonic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18669 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.839335 tonic-1.2.8.dev7/tonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/audio_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/cached_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/collation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.843335 tonic-1.2.8.dev7/tonic/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/datasets/asl_dvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/datasets/cifar10dvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/datasets/davisdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14707 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/datasets/dsec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/datasets/dvs_lips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/datasets/dvsgesture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/datasets/hsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/datasets/mvsec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/datasets/ncaltech101.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/datasets/nmnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/datasets/pokerdvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/datasets/s_mnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/datasets/tum_vie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/datasets/visual_place_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/download_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.843335 tonic-1.2.8.dev7/tonic/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/functional/crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/functional/decimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/functional/denoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/functional/drop_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/functional/drop_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/functional/refractory_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/functional/spatial_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/functional/time_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/functional/time_skew.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/functional/to_averaged_timesurface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/functional/to_bina_rep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/functional/to_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/functional/to_timesurface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/functional/to_voxel_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/functional/uniform_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.843335 tonic-1.2.8.dev7/tonic/prototype/
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/prototype/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/prototype/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.843335 tonic-1.2.8.dev7/tonic/prototype/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/prototype/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/prototype/datasets/ncars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/prototype/datasets/nmnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/prototype/datasets/prophesee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/prototype/datasets/stmnist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.847335 tonic-1.2.8.dev7/tonic/prototype/datasets/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/prototype/datasets/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/prototype/datasets/utils/_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/prototype/datasets/utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/prototype/slicers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/sliced_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/slicers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38208 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   212526 2023-06-20 23:24:07.000000 tonic-1.2.8.dev7/tonic-logo-padded.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:24:32.843335 tonic-1.2.8.dev7/tonic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-06-20 23:24:32.000000 tonic-1.2.8.dev7/tonic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-06-20 23:24:32.000000 tonic-1.2.8.dev7/tonic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 23:24:32.000000 tonic-1.2.8.dev7/tonic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 23:24:32.000000 tonic-1.2.8.dev7/tonic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-20 23:24:32.000000 tonic-1.2.8.dev7/tonic.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-20 23:24:32.000000 tonic-1.2.8.dev7/tonic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 23:24:32.000000 tonic-1.2.8.dev7/tonic.egg-info/top_level.txt
```

### Comparing `tonic-1.2.8.dev4/.github/workflows/ci-pipeline.yml` & `tonic-1.2.8.dev7/.github/workflows/ci-pipeline.yml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 jobs:
   multitest:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, windows-2022]
-        python-version: ["3.7", "3.8", "3.9"]
+        python-version: ["3.7", "3.9", "3.11"]
     steps:
       - uses: actions/checkout@v2
       - if: matrix.os == 'ubuntu-latest'
         name: install audio library libsndfile
         run: sudo apt-get -y update && sudo apt-get install -y libsndfile1
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
```

### Comparing `tonic-1.2.8.dev4/AUTHORS` & `tonic-1.2.8.dev7/AUTHORS`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/ChangeLog` & `tonic-1.2.8.dev7/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 CHANGES
 =======
 
+* update NMNIST prototype dataset and tests to make compatible with Python 3.11
+* test Python 3.11
+* simplify STMNIST prototype dataset, broke keep\_compressed option though
 * Add delta\_t as a parameter to time surface test
 * Remove print statements to evaluate correctness
 * Time surface returns time surfaces at interval
 
 v1.2.7
 ------
```

### Comparing `tonic-1.2.8.dev4/LICENSE.txt` & `tonic-1.2.8.dev7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/PKG-INFO` & `tonic-1.2.8.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonic
-Version: 1.2.8.dev4
+Version: 1.2.8.dev7
 Summary: Neuromorphic datasets and transformations.
 Home-page: UNKNOWN
 Author: The Neuromorphs of Telluride
 Author-email: mail@lenzgregor.com
 License: GNU GPLv3
 Project-URL: Source code, https://github.com/neuromorphs/tonic
 Project-URL: Documentation, https://tonic.readthedocs.org
```

### Comparing `tonic-1.2.8.dev4/README.md` & `tonic-1.2.8.dev7/README.md`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/Makefile` & `tonic-1.2.8.dev7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/_static/event-cameras/eventstream.png` & `tonic-1.2.8.dev7/docs/_static/event-cameras/eventstream.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/_static/event-cameras/framestream.png` & `tonic-1.2.8.dev7/docs/_static/event-cameras/framestream.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/_static/event-cameras/receptive-fields.png` & `tonic-1.2.8.dev7/docs/_static/event-cameras/receptive-fields.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/_static/event-cameras/sampling-theorems.png` & `tonic-1.2.8.dev7/docs/_static/event-cameras/sampling-theorems.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/_static/snn/neuron-models.png` & `tonic-1.2.8.dev7/docs/_static/snn/neuron-models.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/_static/snn/surrogates.png` & `tonic-1.2.8.dev7/docs/_static/snn/surrogates.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/_static/tonic-logo-black.png` & `tonic-1.2.8.dev7/docs/_static/tonic-logo-black.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/_static/tonic-logo-white.png` & `tonic-1.2.8.dev7/docs/_static/tonic-logo-white.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/_static/tonic_favicon.png` & `tonic-1.2.8.dev7/docs/_static/tonic_favicon.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/about/info.rst` & `tonic-1.2.8.dev7/docs/about/info.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/about/prototype.rst` & `tonic-1.2.8.dev7/docs/about/prototype.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/about/release_notes.rst` & `tonic-1.2.8.dev7/docs/about/release_notes.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/conf.py` & `tonic-1.2.8.dev7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/datasets.rst` & `tonic-1.2.8.dev7/docs/datasets.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/gallery/representations/plot_tobinarep.py` & `tonic-1.2.8.dev7/docs/gallery/representations/plot_tobinarep.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/gallery/representations/plot_toframe.py` & `tonic-1.2.8.dev7/docs/gallery/representations/plot_toframe.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/gallery/representations/plot_toimage.py` & `tonic-1.2.8.dev7/docs/gallery/representations/plot_toimage.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/gallery/representations/plot_totimesurface.py` & `tonic-1.2.8.dev7/docs/gallery/representations/plot_totimesurface.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/gallery/transformations/plot_centercrop.py` & `tonic-1.2.8.dev7/docs/gallery/transformations/plot_centercrop.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/gallery/transformations/plot_crop_time.py` & `tonic-1.2.8.dev7/docs/gallery/transformations/plot_crop_time.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/gallery/transformations/plot_decimation.py` & `tonic-1.2.8.dev7/docs/gallery/transformations/plot_decimation.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/gallery/transformations/plot_denoise.py` & `tonic-1.2.8.dev7/docs/gallery/transformations/plot_denoise.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/gallery/transformations/plot_downsample.py` & `tonic-1.2.8.dev7/docs/gallery/transformations/plot_downsample.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/gallery/transformations/plot_drop_event.py` & `tonic-1.2.8.dev7/docs/gallery/transformations/plot_drop_event.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/gallery/transformations/plot_drop_event_by_area.py` & `tonic-1.2.8.dev7/docs/gallery/transformations/plot_drop_event_by_area.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/gallery/transformations/plot_drop_event_by_time.py` & `tonic-1.2.8.dev7/docs/gallery/transformations/plot_drop_event_by_time.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/gallery/transformations/plot_drop_pixel.py` & `tonic-1.2.8.dev7/docs/gallery/transformations/plot_drop_pixel.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/gallery/transformations/plot_merge_polarities.py` & `tonic-1.2.8.dev7/docs/gallery/transformations/plot_merge_polarities.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/gallery/transformations/plot_random_crop.py` & `tonic-1.2.8.dev7/docs/gallery/transformations/plot_random_crop.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/gallery/transformations/plot_random_flip_lr.py` & `tonic-1.2.8.dev7/docs/gallery/transformations/plot_random_flip_lr.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/gallery/transformations/plot_random_flip_ud.py` & `tonic-1.2.8.dev7/docs/gallery/transformations/plot_random_flip_ud.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/gallery/transformations/plot_random_time_reversal.py` & `tonic-1.2.8.dev7/docs/gallery/transformations/plot_random_time_reversal.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/gallery/transformations/plot_refractory_period.py` & `tonic-1.2.8.dev7/docs/gallery/transformations/plot_refractory_period.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/gallery/transformations/plot_spatial_jitter.py` & `tonic-1.2.8.dev7/docs/gallery/transformations/plot_spatial_jitter.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/gallery/transformations/plot_time_jitter.py` & `tonic-1.2.8.dev7/docs/gallery/transformations/plot_time_jitter.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/gallery/transformations/plot_uniform_noise.py` & `tonic-1.2.8.dev7/docs/gallery/transformations/plot_uniform_noise.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/getting_involved/communication_channels.rst` & `tonic-1.2.8.dev7/docs/getting_involved/communication_channels.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/getting_involved/contribute.rst` & `tonic-1.2.8.dev7/docs/getting_involved/contribute.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/getting_started/install.rst` & `tonic-1.2.8.dev7/docs/getting_started/install.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/getting_started/nmnist.ipynb` & `tonic-1.2.8.dev7/docs/getting_started/nmnist.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/how-tos/loading-raw-events.ipynb` & `tonic-1.2.8.dev7/docs/how-tos/loading-raw-events.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/how-tos/visualizing-data.ipynb` & `tonic-1.2.8.dev7/docs/how-tos/visualizing-data.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/how-tos/wrapping_own_data.ipynb` & `tonic-1.2.8.dev7/docs/how-tos/wrapping_own_data.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/index.md` & `tonic-1.2.8.dev7/docs/index.md`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/make.bat` & `tonic-1.2.8.dev7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/reading_material/design_choices.rst` & `tonic-1.2.8.dev7/docs/reading_material/design_choices.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/reading_material/intro-event-cameras.rst` & `tonic-1.2.8.dev7/docs/reading_material/intro-event-cameras.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/reading_material/intro-snns.rst` & `tonic-1.2.8.dev7/docs/reading_material/intro-snns.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/reading_material/training-snns.rst` & `tonic-1.2.8.dev7/docs/reading_material/training-snns.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/transformations.rst` & `tonic-1.2.8.dev7/docs/transformations.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/tutorials/batching.ipynb` & `tonic-1.2.8.dev7/docs/tutorials/batching.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/tutorials/davis_data.ipynb` & `tonic-1.2.8.dev7/docs/tutorials/davis_data.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/tutorials/fast_dataloading.ipynb` & `tonic-1.2.8.dev7/docs/tutorials/fast_dataloading.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/tutorials/large_datasets.ipynb` & `tonic-1.2.8.dev7/docs/tutorials/large_datasets.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/docs/tutorials/slicing.ipynb` & `tonic-1.2.8.dev7/docs/tutorials/slicing.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/setup.cfg` & `tonic-1.2.8.dev7/setup.cfg`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/test/dataset_utils.py` & `tonic-1.2.8.dev7/test/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/test/prototype_dataset_utils.py` & `tonic-1.2.8.dev7/test/prototype_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/test/test_audio_transforms.py` & `tonic-1.2.8.dev7/test/test_audio_transforms.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/test/test_caching.py` & `tonic-1.2.8.dev7/test/test_caching.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/test/test_chained_transforms.py` & `tonic-1.2.8.dev7/test/test_chained_transforms.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/test/test_data/sample.aedat4` & `tonic-1.2.8.dev7/test/test_data/sample.aedat4`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/test/test_data/sample_ncars.dat` & `tonic-1.2.8.dev7/test/test_data/sample_ncars.dat`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/test/test_data/sample_nmnist.bin` & `tonic-1.2.8.dev7/test/test_data/sample_nmnist.bin`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/test/test_data/sample_stmnist.mat` & `tonic-1.2.8.dev7/test/test_data/sample_stmnist.mat`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/test/test_datasets.py` & `tonic-1.2.8.dev7/test/test_datasets.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/test/test_dsec.py` & `tonic-1.2.8.dev7/test/test_dsec.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/test/test_io.py` & `tonic-1.2.8.dev7/test/test_io.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/test/test_prototype_datasets.py` & `tonic-1.2.8.dev7/test/test_prototype_datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,16 @@
             PATH_TO_TEST_DATA / "sample_nmnist.bin",
             destination_path / "sample_nmnist.bin",
         )
     # We compress the archive.
     shutil.make_archive(
         base_name=Path(tmpdir, "NMNIST", filename),
         format="zip",
-        base_dir=folder_path,
-        root_dir=folder_path,
+        root_dir=folder_path.parent,
+        base_dir=folder,
     )
     # We remove the folder previously created.
     shutil.rmtree(folder_path)
 
 
 class NMNISTTestCase_Train_Uncompressed_AllSaccades(dataset_utils.DatasetTestCase):
     DATASET_CLASS = datasets.NMNIST
@@ -135,16 +135,14 @@
     # We compress the archive.
     shutil.make_archive(
         base_name=Path(tmpdir, "STMNIST", filename),
         format="zip",
         base_dir=folder_path,
         root_dir=folder_path,
     )
-    # We remove the folder previously created.
-    shutil.rmtree(folder_path)
 
 
 class STMNISTTestCase_Uncompressed(dataset_utils.DatasetTestCase):
     DATASET_CLASS = datasets.STMNIST
     FEATURE_TYPES = (datasets.STMNIST._DTYPE,)
     TARGET_TYPES = (int,)
     KWARGS = {"keep_compressed": False}
```

### Comparing `tonic-1.2.8.dev4/test/test_representations.py` & `tonic-1.2.8.dev7/test/test_representations.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/test/test_sliced_dataset.py` & `tonic-1.2.8.dev7/test/test_sliced_dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/test/test_slicers.py` & `tonic-1.2.8.dev7/test/test_slicers.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/test/test_tonic_utils.py` & `tonic-1.2.8.dev7/test/test_tonic_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/test/test_transforms.py` & `tonic-1.2.8.dev7/test/test_transforms.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/test/utils.py` & `tonic-1.2.8.dev7/test/utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/audio_transforms.py` & `tonic-1.2.8.dev7/tonic/audio_transforms.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/cached_dataset.py` & `tonic-1.2.8.dev7/tonic/cached_dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/collation.py` & `tonic-1.2.8.dev7/tonic/collation.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/dataset.py` & `tonic-1.2.8.dev7/tonic/dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/datasets/__init__.py` & `tonic-1.2.8.dev7/tonic/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/datasets/asl_dvs.py` & `tonic-1.2.8.dev7/tonic/datasets/asl_dvs.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/datasets/cifar10dvs.py` & `tonic-1.2.8.dev7/tonic/datasets/cifar10dvs.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/datasets/davisdataset.py` & `tonic-1.2.8.dev7/tonic/datasets/davisdataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/datasets/dsec.py` & `tonic-1.2.8.dev7/tonic/datasets/dsec.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/datasets/dvs_lips.py` & `tonic-1.2.8.dev7/tonic/datasets/dvs_lips.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/datasets/dvsgesture.py` & `tonic-1.2.8.dev7/tonic/datasets/dvsgesture.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/datasets/hsd.py` & `tonic-1.2.8.dev7/tonic/datasets/hsd.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/datasets/mvsec.py` & `tonic-1.2.8.dev7/tonic/datasets/mvsec.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/datasets/ncaltech101.py` & `tonic-1.2.8.dev7/tonic/datasets/ncaltech101.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/datasets/nmnist.py` & `tonic-1.2.8.dev7/tonic/datasets/nmnist.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/datasets/pokerdvs.py` & `tonic-1.2.8.dev7/tonic/datasets/pokerdvs.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/datasets/s_mnist.py` & `tonic-1.2.8.dev7/tonic/datasets/s_mnist.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/datasets/tum_vie.py` & `tonic-1.2.8.dev7/tonic/datasets/tum_vie.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/datasets/visual_place_recognition.py` & `tonic-1.2.8.dev7/tonic/datasets/visual_place_recognition.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/download_utils.py` & `tonic-1.2.8.dev7/tonic/download_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/functional/__init__.py` & `tonic-1.2.8.dev7/tonic/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/functional/crop.py` & `tonic-1.2.8.dev7/tonic/functional/crop.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/functional/decimate.py` & `tonic-1.2.8.dev7/tonic/functional/decimate.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/functional/denoise.py` & `tonic-1.2.8.dev7/tonic/functional/denoise.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/functional/drop_event.py` & `tonic-1.2.8.dev7/tonic/functional/drop_event.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/functional/drop_pixel.py` & `tonic-1.2.8.dev7/tonic/functional/drop_pixel.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/functional/refractory_period.py` & `tonic-1.2.8.dev7/tonic/functional/refractory_period.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/functional/spatial_jitter.py` & `tonic-1.2.8.dev7/tonic/functional/spatial_jitter.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/functional/time_jitter.py` & `tonic-1.2.8.dev7/tonic/functional/time_jitter.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/functional/time_skew.py` & `tonic-1.2.8.dev7/tonic/functional/time_skew.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/functional/to_averaged_timesurface.py` & `tonic-1.2.8.dev7/tonic/functional/to_averaged_timesurface.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/functional/to_bina_rep.py` & `tonic-1.2.8.dev7/tonic/functional/to_bina_rep.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/functional/to_frame.py` & `tonic-1.2.8.dev7/tonic/functional/to_frame.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/functional/to_timesurface.py` & `tonic-1.2.8.dev7/tonic/functional/to_timesurface.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/functional/to_voxel_grid.py` & `tonic-1.2.8.dev7/tonic/functional/to_voxel_grid.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/functional/uniform_noise.py` & `tonic-1.2.8.dev7/tonic/functional/uniform_noise.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/io.py` & `tonic-1.2.8.dev7/tonic/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import numpy as np
 from numpy.lib import recfunctions
 
 events_struct = np.dtype(
     [("x", np.int16), ("y", np.int16), ("t", np.int64), ("p", bool)]
 )
 
+
 # many functions in this file have been copied from https://gitlab.com/synsense/aermanager/-/blob/master/aermanager/parsers.py
 def make_structured_array(*args, dtype=events_struct):
     """Make a structured array given a variable number of argument values.
 
     Parameters:
         *args: Values in the form of nested lists or tuples or numpy arrays.
                Every except the first argument can be of a primitive data type like int or float.
@@ -164,15 +165,15 @@
 
     xytp = make_structured_array(x, y, t, p)
     shape = (132, 104)
     return shape, xytp
 
 
 def read_mnist_file(
-    bin_file: Union[str, BinaryIO], dtype: np.dtype, is_stream: Optional[bool] = False
+    bin_file: Union[str, BinaryIO], dtype: np.dtype, is_stream: bool = False
 ):
     """Reads the events contained in N-MNIST/N-CALTECH101 datasets.
 
     Code adapted from https://github.com/gorchard/event-Python/blob/master/eventvision.py
     """
     if is_stream:
         raw_data = np.frombuffer(bin_file.read(), dtype=np.uint8).astype(np.uint32)
```

### Comparing `tonic-1.2.8.dev4/tonic/prototype/README.md` & `tonic-1.2.8.dev7/tonic/prototype/README.md`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/prototype/datasets/ncars.py` & `tonic-1.2.8.dev7/tonic/prototype/datasets/ncars.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/prototype/datasets/nmnist.py` & `tonic-1.2.8.dev7/tonic/prototype/datasets/nmnist.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import zipfile
 from pathlib import Path
 from typing import Any, BinaryIO, Callable, Iterator, Optional, Tuple, Union
 
 import numpy as np
 from torchdata.datapipes.iter import (
     FileLister,
     FileOpener,
@@ -92,89 +93,63 @@
 
     def __init__(
         self,
         root: os.PathLike,
         train: Optional[bool] = True,
         first_saccade_only: Optional[bool] = False,
         keep_compressed: Optional[bool] = False,
-        skip_sha256_check: Optional[bool] = True,
     ) -> None:
         self.train = train
         self.first_saccade_only = first_saccade_only
+        self.filename = self._TRAIN_FILENAME if self.train else self._TEST_FILENAME
+        self.subfolder = self._TRAIN_FOLDER if self.train else self._TEST_FOLDER
+        sha256 = self._TRAIN_SHA256 if self.train else self._TEST_SHA256
+        root = Path(root, self.__class__.__name__)
+        if not self._check_exists(root / self.filename):
+            self._download(root, self.filename, sha256)
         super().__init__(
-            root=Path(root, self.__class__.__name__),
+            root=root,
             keep_compressed=keep_compressed,
-            skip_sha256_check=skip_sha256_check,
         )
-        self._download()
 
     def __len__(self) -> int:
         return 60_000 if self.train else 10_000
 
     def _filter(self, fname: str) -> bool:
         return fname.endswith(".bin")
 
     def _saccade_filter(self, events: np.ndarray):
-        return events[events["t"] > int(1e5)]
+        return events[events["t"] <= int(1e5)]
 
-    def _download(self) -> None:
-        # Setting file path depending on train value.
+    def _download(self, root, filename, sha256) -> None:
         url = self._TRAIN_URL if self.train else self._TEST_URL
-        sha256 = self._TRAIN_SHA256 if self.train else self._TEST_SHA256
-        filename = self._TRAIN_FILENAME if self.train else self._TEST_FILENAME
-        # Downloading and SHA256 check.
-        if not self._check_exists():
-            download_url(url=url, root=self._root, filename=filename)
-            check_sha256(os.path.join(self._root, filename), sha256)
-        elif not self.skip_sha256:
-            check_sha256(os.path.join(self._root, filename), sha256)
-
-    def _check_exists(self) -> bool:
-        filename = self._TRAIN_FILENAME if self.train else self._TEST_FILENAME
-        return os.path.isfile(os.path.join(self._root, filename))
-
-    def _uncompress(
-        self, dp: IterDataPipe[Tuple[Any, BinaryIO]]
-    ) -> IterDataPipe[Tuple[str, BinaryIO]]:
-        folder = self._TRAIN_FOLDER if self.train else self._TEST_FOLDER
-        # Joining root with a folder to contain the data.
-        filepath = os.path.join(self._root, folder)
-        if (not os.path.isdir(filepath)) or (not os.listdir(filepath)):
-            os.makedirs(filepath, exist_ok=True)
-
-            # Decompressing in root.
-            def read_bin(fdata):
-                return fdata.read()
-
-            dp = Mapper(dp, read_bin, input_col=1)
-
-            def filepath_fn(fpath):
-                fpath_i = fpath.split(os.sep)
-                start = fpath_i.index(folder) + len(os.sep)
-                fpath_i = os.sep.join(fpath_i[start:])
-                return os.path.join(filepath, fpath_i)
-
-            dp = Saver(dp, mode="wb", filepath_fn=filepath_fn)
-            # Saving data to file.
-            for x in dp:
-                pass
-        dp = FileLister(filepath, recursive=True)
-        return dp
+        download_url(url=url, root=root, filename=filename)
+        check_sha256(root / filename, sha256)
+
+    def _check_exists(self, folder) -> bool:
+        return not folder.is_file()
+
+    def _is_unzipped(self, folder) -> bool:
+        if not folder.is_dir():
+            return False
+        dp = FileLister(str(folder), recursive=True).filter(self._filter)
+        return len(list(dp)) >= 60_000 if self.train else 10_000
 
     def _datapipe(self) -> IterDataPipe[Sample]:
-        filename = self._TRAIN_FILENAME if self.train else self._TEST_FILENAME
-        filepath = os.path.join(self._root, filename)
-        dp = FileLister(str(filepath))
-        dp = FileOpener(dp, mode="b")
-        # Unzipping.
-        dp = ZipArchiveLoader(dp)
         if not self.keep_cmp:
-            dp = self._uncompress(dp).filter(self._filter)
+            folder = self._root / self.subfolder
+            if not self._is_unzipped(folder):
+                with zipfile.ZipFile(self._root / self.filename, "r") as zip_file:
+                    zip_file.extractall(self._root)
+            dp = FileLister(str(folder), recursive=True)
+            dp = dp.filter(self._filter)
         else:
-            # Filtering the non-bin files.
-            dp = Filter(dp, self._filter, input_col=0)
+            zip_filepath = self._root / self.filename
+            dp = FileLister(str(zip_filepath))
+            dp = FileOpener(dp, mode="rb")
+            dp = ZipArchiveLoader(dp)
         # Reading data to structured NumPy array and integer target.
         dp = NMNISTFileReader(dp, keep_compressed=self.keep_cmp)
         # Filtering the first saccade.
         if self.first_saccade_only:
             dp = Mapper(dp, self._saccade_filter, input_col=0)
         return dp
```

### Comparing `tonic-1.2.8.dev4/tonic/prototype/datasets/prophesee.py` & `tonic-1.2.8.dev7/tonic/prototype/datasets/prophesee.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/prototype/datasets/stmnist.py` & `tonic-1.2.8.dev7/tonic/prototype/datasets/stmnist.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import zipfile
 from pathlib import Path
 from typing import Any, BinaryIO, Callable, Iterator, Optional, Tuple, Union
 
 import numpy as np
 from scipy.io import loadmat
 from torchdata.datapipes.iter import (
     FileLister,
@@ -28,17 +29,17 @@
         ),
     ) -> None:
         self.dp = dp
         self.dtype = dtype
         self.sensor_size = sensor_size
 
     def __iter__(self) -> Iterator[Sample]:
-        for fname, fdata in self.dp:
+        for fname in self.dp:
             yield (
-                self._mat_to_array(fdata),
+                self._mat_to_array(fname),
                 self._get_target(fname),
             )
 
     def _get_target(self, fname: str) -> int:
         return int(fname.split(os.sep)[-2])
 
     def _mat_to_array(self, f):
@@ -63,96 +64,71 @@
         events["p"] = np.maximum(spikes[(events_nums, events_addrs)], 0).astype(int)
         return events
 
 
 class STMNIST(Dataset):
     """`ST-MNIST <https://arxiv.org/abs/2005.04319>`_
 
-    Novel neuromorphic Spiking Tactile MNIST (ST-MNIST) dataset, which comprises handwritten
+    Neuromorphic Spiking Tactile MNIST (ST-MNIST) dataset, which comprises handwritten
     digits obtained by human participants writing on a neuromorphic tactile sensor array. The
     original paper can be found at https://arxiv.org/abs/2005.04319. Data is provided with the MAT
     format. Download of the compressed dataset has to be done by the user by accessing https://scho
     larbank.nus.edu.sg/bitstream/10635/168106/2/STMNIST%20dataset%20NUS%20Tee%20Research%20Group.zi
-    p, where a form has to be compiled. Then, the path to the ZIP archive has to be provided to the
-    stmnist() function root argument.
+    p, where a form has to be completed. Then, the path to the ZIP archive has to be provided to the
+    STMNIST constructor root argument.
 
     Events have (xytp) ordering.
     Parameters:
-        root (string): path to the ZIP archive downloaded by the user (e.g. "./STMNIST.zip").
-        transform (callable, optional): a callable of transforms to be applied to events data.
-        target_transform (callable, optional): a callable of transform to be applied to target data.
-        transforms (callable, optional): a callable of transforms to be applied to both events and target data.
+        root (string): Parent folder of 'STMNIST/STMNIST dataset NUS Tee Research Group.zip'. The STMNIST folder is related to the Tonic class name and is needed currently.
+        shuffle (bool): Whether to shuffle the dataset. More efficient if done based on file paths.
 
     Returns:
         dp (IterDataPipe[Sample]): Torchdata data pipe that yields a tuple of events (or transformed events) and target.
     """
 
     _DTYPE = np.dtype([("x", int), ("y", int), ("t", int), ("p", int)])
     _SHA256 = "825bb5a64753fff4a2a2c32e3497fa8a951d9c94993e03ba25a057e17d83b884"
+    _FILENAME = "STMNIST dataset NUS Tee Research Group.zip"
     sensor_size = dict(x=10, y=10, p=2)
 
     def __init__(
         self,
         root: os.PathLike,
         keep_compressed: Optional[bool] = False,
         skip_sha256_check: Optional[bool] = True,
+        shuffle: bool = False,
     ) -> None:
         super().__init__(
             Path(root, self.__class__.__name__),
             keep_compressed,
             skip_sha256_check,
         )
-        assert self._check_exists(), "Error: the archive is not present."
-        if not self.skip_sha256:
-            check_sha256(fpath=self._root, sha256_provided=self._SHA256)
+        if not skip_sha256_check:
+            check_sha256(
+                fpath=self._root / self._FILENAME, sha256_provided=self._SHA256
+            )
+        if not self._check_exists():
+            assert os.path.isfile(
+                self._root / self._FILENAME
+            ), "Error: root must point to parent folder of STMNIST/STMNIST dataset NUS Tee Research Group.zip."
+            if not keep_compressed:
+                with zipfile.ZipFile(self._root / self._FILENAME, "r") as zip_file:
+                    zip_file.extractall(self._root)
+        self.shuffle = shuffle
 
     def _check_exists(self):
-        return os.path.isfile(self._root)
+        dp = FileLister(str(self._root), recursive=True).filter(self._filter)
+        return len(list(dp)) >= 6953
 
     def __len__(self) -> int:
         return 6_953
 
     def _filter(self, fname: str) -> bool:
         return fname.endswith(".mat") and ("LUT" not in fname)
 
-    def _uncompress(
-        self, dp: IterDataPipe[Tuple[Any, BinaryIO]]
-    ) -> IterDataPipe[Tuple[str, BinaryIO]]:
-        # Stripping the archive from self._root.
-        root = os.sep.join(str(self._root).split(os.sep)[:-1])
-        # Joining root with a folder to contain the data.
-        root = os.path.join(root, "data_uncompressed")
-        if not os.path.isdir(root):
-            os.mkdir(root)
-
-            # Decompressing in root.
-            def read_bin(fdata):
-                return fdata.read()
-
-            def filepath_fn(fpath):
-                fpath_i = fpath.split(os.sep)
-                start = fpath_i.index("data_submission") + len(os.sep)
-                fpath_i = os.sep.join(fpath_i[start:])
-                return os.path.join(
-                    root,
-                    fpath_i,
-                )
-
-            dp = Mapper(dp, read_bin, input_col=1)
-            dp = Saver(dp, mode="wb", filepath_fn=filepath_fn)
-            # Saving data to file.
-            for x in dp:
-                pass
-        dp = FileLister(root, recursive=True)
-        dp = FileOpener(dp, mode="rb")
-        return dp
-
     def _datapipe(self) -> IterDataPipe[Sample]:
-        dp = FileLister(str(self._root))
-        dp = FileOpener(dp, mode="b")
-        # Unzipping.
-        dp = ZipArchiveLoader(dp)
-        if not self.keep_cmp:
-            dp = self._uncompress(dp)
-        dp = Filter(dp, self._filter, input_col=0)
+        dp = FileLister(str(self._root), recursive=True)
+        if self.shuffle:
+            dp = dp.shuffle(buffer_size=10_000)
+        dp = Filter(dp, self._filter)
         dp = STMNISTFileReader(dp)
         return dp
```

### Comparing `tonic-1.2.8.dev4/tonic/prototype/datasets/utils/_dataset.py` & `tonic-1.2.8.dev7/tonic/prototype/datasets/utils/_dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/prototype/datasets/utils/_utils.py` & `tonic-1.2.8.dev7/tonic/prototype/datasets/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/prototype/slicers.py` & `tonic-1.2.8.dev7/tonic/prototype/slicers.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/sliced_dataset.py` & `tonic-1.2.8.dev7/tonic/sliced_dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/slicers.py` & `tonic-1.2.8.dev7/tonic/slicers.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/transforms.py` & `tonic-1.2.8.dev7/tonic/transforms.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic/utils.py` & `tonic-1.2.8.dev7/tonic/utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic-logo-padded.png` & `tonic-1.2.8.dev7/tonic-logo-padded.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.8.dev4/tonic.egg-info/PKG-INFO` & `tonic-1.2.8.dev7/tonic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonic
-Version: 1.2.8.dev4
+Version: 1.2.8.dev7
 Summary: Neuromorphic datasets and transformations.
 Home-page: UNKNOWN
 Author: The Neuromorphs of Telluride
 Author-email: mail@lenzgregor.com
 License: GNU GPLv3
 Project-URL: Source code, https://github.com/neuromorphs/tonic
 Project-URL: Documentation, https://tonic.readthedocs.org
```

### Comparing `tonic-1.2.8.dev4/tonic.egg-info/SOURCES.txt` & `tonic-1.2.8.dev7/tonic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

