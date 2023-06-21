# Comparing `tmp/eradiate-0.23.2rc1.tar.gz` & `tmp/eradiate-0.23.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eradiate-0.23.2rc1.tar", last modified: Tue May 16 13:35:25 2023, max compression
+gzip compressed data, was "eradiate-0.23.2rc2.tar", last modified: Wed Jun 21 16:12:21 2023, max compression
```

## Comparing `eradiate-0.23.2rc1.tar` & `eradiate-0.23.2rc2.tar`

### file list

```diff
@@ -1,604 +1,631 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.943456 eradiate-0.23.2rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.883456 eradiate-0.23.2rc1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.887456 eradiate-0.23.2rc1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.887456 eradiate-0.23.2rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/.github/workflows/cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    18002 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-05-16 13:35:25.943456 eradiate-0.23.2rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.887456 eradiate-0.23.2rc1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.887456 eradiate-0.23.2rc1/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/_ext/exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/_ext/pluginparameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.887456 eradiate-0.23.2rc1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/_static/.keep
--rw-r--r--   0 runner    (1001) docker     (123)    17013 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/_static/eradiate-logo-typo-black.png
--rw-r--r--   0 runner    (1001) docker     (123)    32795 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/_static/eradiate-logo-typo-black.svg
--rw-r--r--   0 runner    (1001) docker     (123)    25531 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/_static/eradiate-logo-typo-darkgrey.png
--rw-r--r--   0 runner    (1001) docker     (123)    34059 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/_static/eradiate-logo-typo-darkgrey.svg
--rw-r--r--   0 runner    (1001) docker     (123)    18587 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/_static/eradiate-logo-typo-white.png
--rw-r--r--   0 runner    (1001) docker     (123)    34061 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/_static/eradiate-logo-typo-white.svg
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/_static/theme_overrides.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.879456 eradiate-0.23.2rc1/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.887456 eradiate-0.23.2rc1/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/_templates/autosummary/module.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.887456 eradiate-0.23.2rc1/docs/_templates/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/_templates/sections/footer-content.html
--rw-r--r--   0 runner    (1001) docker     (123)    10525 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/convert_figures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.895456 eradiate-0.23.2rc1/docs/fig/
--rw-r--r--   0 runner    (1001) docker     (123)    20540 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/atmosphere_attributes.png
--rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/atmosphere_attributes.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28149 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/azimuth-east_left.png
--rw-r--r--   0 runner    (1001) docker     (123)    32937 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/azimuth-east_left.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28852 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/azimuth-east_right.png
--rw-r--r--   0 runner    (1001) docker     (123)    35278 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/azimuth-east_right.svg
--rw-r--r--   0 runner    (1001) docker     (123)    30666 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/azimuth-north_left.png
--rw-r--r--   0 runner    (1001) docker     (123)    32862 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/azimuth-north_left.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28115 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/azimuth-north_right.png
--rw-r--r--   0 runner    (1001) docker     (123)    32455 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/azimuth-north_right.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28153 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/azimuth-south_left.png
--rw-r--r--   0 runner    (1001) docker     (123)    32939 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/azimuth-south_left.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28118 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/azimuth-south_right.png
--rw-r--r--   0 runner    (1001) docker     (123)    32455 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/azimuth-south_right.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28178 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/azimuth-west_left.png
--rw-r--r--   0 runner    (1001) docker     (123)    32935 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/azimuth-west_left.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28067 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/azimuth-west_right.png
--rw-r--r--   0 runner    (1001) docker     (123)    32437 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/azimuth-west_right.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/cartesian-coordinate-system.png
--rw-r--r--   0 runner    (1001) docker     (123)    15939 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/cartesian-coordinate-system.svg
--rw-r--r--   0 runner    (1001) docker     (123)    25301 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/cuboid_leaf_cloud_params.png
--rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/cuboid_leaf_cloud_params.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.895456 eradiate-0.23.2rc1/docs/fig/diagrams/
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/diagrams/class_diagram_biosphere.drawio
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/diagrams/cuboid_leaf_cloud_params.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    20990 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/diagrams/package.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    40438 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/eradiate-logo-typo-black.png
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/eradiate-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/icon_eradiate.png
--rw-r--r--   0 runner    (1001) docker     (123)    38873 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/package.png
--rw-r--r--   0 runner    (1001) docker     (123)    57417 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/package.svg
--rw-r--r--   0 runner    (1001) docker     (123)    32384 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/radiancemeter_hsphere.png
--rw-r--r--   0 runner    (1001) docker     (123)    43351 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/radiancemeter_hsphere.svg
--rw-r--r--   0 runner    (1001) docker     (123)    36773 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/radiancemeter_plane.png
--rw-r--r--   0 runner    (1001) docker     (123)    31853 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/radiancemeter_plane.svg
--rw-r--r--   0 runner    (1001) docker     (123)    17583 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/requirement_layers.png
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/requirement_layers.svg
--rw-r--r--   0 runner    (1001) docker     (123)    21451 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/solid_2017.png
--rw-r--r--   0 runner    (1001) docker     (123)    24994 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/spectral_discretization_ckd_atm_interval.png
--rw-r--r--   0 runner    (1001) docker     (123)    16459 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/spectral_discretization_ckd_atm_isolated.png
--rw-r--r--   0 runner    (1001) docker     (123)    28519 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/spectral_discretization_ckd_noatm_interval.png
--rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/spectral_discretization_ckd_noatm_isolated.png
--rw-r--r--   0 runner    (1001) docker     (123)    27127 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/spectral_discretization_mono_atm_interval.png
--rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/spectral_discretization_mono_atm_isolated.png
--rw-r--r--   0 runner    (1001) docker     (123)    46208 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/spectral_discretization_mono_noatm_interval1.png
--rw-r--r--   0 runner    (1001) docker     (123)    14036 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/spectral_discretization_mono_noatm_interval2.png
--rw-r--r--   0 runner    (1001) docker     (123)    21975 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/spectral_discretization_mono_noatm_isolated.png
--rw-r--r--   0 runner    (1001) docker     (123)    10036 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/spherical-coordinate-system.png
--rw-r--r--   0 runner    (1001) docker     (123)    19861 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/spherical-coordinate-system.svg
--rw-r--r--   0 runner    (1001) docker     (123)    20660 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/thuillier_2003.png
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/generate_md_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/generate_rst_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/generate_rst_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/index_latex.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)    16528 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/references.bib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.895456 eradiate-0.23.2rc1/docs/rst/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/bibliography.rst
--rw-r--r--   0 runner    (1001) docker     (123)    22779 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/dependencies.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.895456 eradiate-0.23.2rc1/docs/rst/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/developer_guide/design_atmosphere.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/developer_guide/factory_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/developer_guide/lazy_loading.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/developer_guide/radiometric_kernel_interface.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/developer_guide/scene_generator.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.895456 eradiate-0.23.2rc1/docs/rst/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12492 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/getting_started/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/getting_started/update.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13682 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/maintainer_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.899456 eradiate-0.23.2rc1/docs/rst/reference_api/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/attrs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/config.rst
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/constants.rst
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/contexts.rst
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/converters.rst
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/data.rst
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/eradiate_core.rst
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/experiments.rst
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/factory.rst
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/frame.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/kernel.rst
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/mode.rst
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/notebook.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/pipelines.rst
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/plot.rst
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/quad.rst
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/radprops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/rng.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/scenes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/spectral.rst
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/srf_tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/test_tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/thermoprops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/units.rst
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/util.rst
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/validators.rst
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/warp.rst
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/xarray.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.899456 eradiate-0.23.2rc1/docs/rst/reference_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_plugins/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.899456 eradiate-0.23.2rc1/docs/rst/user_guide/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.903456 eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/absorption.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.903456 eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/fig/
--rw-r--r--   0 runner    (1001) docker     (123)    25171 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/fig/bad_resolution.png
--rw-r--r--   0 runner    (1001) docker     (123)    26889 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/fig/good_resolution.png
--rw-r--r--   0 runner    (1001) docker     (123)    24938 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/fig/line.png
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/heterogeneous.rst
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/homogeneous.rst
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/molecular.rst
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/particle_layer.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/rayleigh_scattering.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/basic_concepts.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/conventions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.903456 eradiate-0.23.2rc1/docs/rst/user_guide/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/data/absorption.rst
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/data/atmosphere_radprops.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/data/atmosphere_thermoprops.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/data/ckd.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.903456 eradiate-0.23.2rc1/docs/rst/user_guide/data/fig/
--rw-r--r--   0 runner    (1001) docker     (123)    30117 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/data/fig/p_interp_rerr_histo_65349.png
--rw-r--r--   0 runner    (1001) docker     (123)    59107 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/data/fig/pt_points.png
--rw-r--r--   0 runner    (1001) docker     (123)    28580 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/data/fig/w_interp_rerr_histo_101325.png
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/data/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/data/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/data/particle_radprops.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/data/solar_irradiance.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/data/spectra-us76_u86_4.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/data/srf.rst
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/onedim_experiment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/package_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13015 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/spectral_discretization.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/unit_guide_user.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.903456 eradiate-0.23.2rc1/docs/src/
--rw-r--r--   0 runner    (1001) docker     (123)    18002 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/src/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/src/reference_cli.md
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.907456 eradiate-0.23.2rc1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/check_conda_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/copy_envvars.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (123)    13404 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/environment-dev.yml
--rw-r--r--   0 runner    (1001) docker     (123)    39893 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/environment-linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/environment-minimal.yml
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/environment-optional.yml
--rw-r--r--   0 runner    (1001) docker     (123)    30957 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/environment-osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/environment-production.yml
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/environment-recommended.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/environment.in
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/layered.yml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/main.in
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/main.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/make_conda_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/make_pip_in_files.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/optional.in
--rw-r--r--   0 runner    (1001) docker     (123)    20920 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/optional.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/production.in
--rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/production.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/recommended.in
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/tests.in
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/setpath.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:35:25.943456 eradiate-0.23.2rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.879456 eradiate-0.23.2rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.911456 eradiate-0.23.2rc1/src/eradiate/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9411 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/attrs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.911456 eradiate-0.23.2rc1/src/eradiate/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/cli/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/cli/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/cli/srf.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.911456 eradiate-0.23.2rc1/src/eradiate/data/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/data/_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/data/_blind_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/data/_blind_online.py
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/data/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/data/_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/data/_safe_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/data/_safe_online.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/data/_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    16343 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/data/downloads.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/data/downloads_development.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.911456 eradiate-0.23.2rc1/src/eradiate/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/experiments/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/experiments/_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/experiments/_canopy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12113 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/experiments/_canopy_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)    20760 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/experiments/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/experiments/_dem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/experiments/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12531 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/frame.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.915456 eradiate-0.23.2rc1/src/eradiate/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/kernel/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/kernel/_bitmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/kernel/_bsdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/kernel/_kernel_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/kernel/_render.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/kernel/gridvolume.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/kernel/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/kernel/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.915456 eradiate-0.23.2rc1/src/eradiate/notebook/
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/notebook/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/notebook/tutorials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.915456 eradiate-0.23.2rc1/src/eradiate/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/pipelines/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/pipelines/_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11488 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/pipelines/_assemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/pipelines/_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/pipelines/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/pipelines/_gather.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/quad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.915456 eradiate-0.23.2rc1/src/eradiate/radprops/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/radprops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/radprops/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/radprops/_afgl1986.py
--rw-r--r--   0 runner    (1001) docker     (123)    14982 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/radprops/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10705 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/radprops/_us76_approx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/radprops/_util_mono.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/radprops/absorption.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/radprops/rayleigh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/rng.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.915456 eradiate-0.23.2rc1/src/eradiate/scenes/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.919456 eradiate-0.23.2rc1/src/eradiate/scenes/atmosphere/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/atmosphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/atmosphere/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23375 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/atmosphere/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/atmosphere/_heterogeneous.py
--rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/atmosphere/_homogeneous.py
--rw-r--r--   0 runner    (1001) docker     (123)    14639 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/atmosphere/_molecular_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/atmosphere/_particle_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/atmosphere/_particle_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.919456 eradiate-0.23.2rc1/src/eradiate/scenes/biosphere/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/biosphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/biosphere/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/biosphere/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    12392 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/biosphere/_discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)    38992 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/biosphere/_leaf_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    17136 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/biosphere/_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.919456 eradiate-0.23.2rc1/src/eradiate/scenes/bsdfs/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/bsdfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/bsdfs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/bsdfs/_black.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/bsdfs/_checkerboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/bsdfs/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/bsdfs/_lambertian.py
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/bsdfs/_mqdiffuse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/bsdfs/_rpv.py
--rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.919456 eradiate-0.23.2rc1/src/eradiate/scenes/illumination/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/illumination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/illumination/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/illumination/_constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/illumination/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/illumination/_directional.py
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/illumination/_spot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.919456 eradiate-0.23.2rc1/src/eradiate/scenes/integrators/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/integrators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/integrators/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/integrators/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/integrators/_path_tracers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.923456 eradiate-0.23.2rc1/src/eradiate/scenes/measure/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/measure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/measure/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9555 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/measure/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/measure/_distant.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/measure/_distant_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/measure/_hemispherical_distant.py
--rw-r--r--   0 runner    (1001) docker     (123)    20874 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/measure/_multi_distant.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/measure/_multi_radiancemeter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/measure/_perspective.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/measure/_radiancemeter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.923456 eradiate-0.23.2rc1/src/eradiate/scenes/phase/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/phase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/phase/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12138 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/phase/_blend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/phase/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/phase/_hg.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/phase/_isotropic.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/phase/_rayleigh.py
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/phase/_tabulated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.923456 eradiate-0.23.2rc1/src/eradiate/scenes/shapes/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/shapes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/shapes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/shapes/_buffermesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/shapes/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/shapes/_cuboid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/shapes/_filemesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/shapes/_rectangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/shapes/_sphere.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.923456 eradiate-0.23.2rc1/src/eradiate/scenes/spectra/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/spectra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/spectra/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/spectra/_air_scattering_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/spectra/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    11869 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/spectra/_interpolated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/spectra/_multi_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/spectra/_solar_irradiance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/spectra/_uniform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.923456 eradiate-0.23.2rc1/src/eradiate/scenes/surface/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/surface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/surface/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/surface/_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/surface/_central_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/surface/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10526 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/surface/_dem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.927456 eradiate-0.23.2rc1/src/eradiate/spectral/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/spectral/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/spectral/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/spectral/ckd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/spectral/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/spectral/mono.py
--rw-r--r--   0 runner    (1001) docker     (123)    26485 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/srf_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.927456 eradiate-0.23.2rc1/src/eradiate/test_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/test_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/test_tools/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/test_tools/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/test_tools/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/test_tools/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.927456 eradiate-0.23.2rc1/src/eradiate/thermoprops/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/thermoprops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/thermoprops/afgl_1986.py
--rw-r--r--   0 runner    (1001) docker     (123)    42061 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/thermoprops/us76.py
--rw-r--r--   0 runner    (1001) docker     (123)    22124 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/thermoprops/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.927456 eradiate-0.23.2rc1/src/eradiate/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/util/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15100 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/util/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/util/numpydoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/util/sys_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/warp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.927456 eradiate-0.23.2rc1/src/eradiate/xarray/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/xarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/xarray/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/xarray/_accessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/xarray/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/xarray/interp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.911456 eradiate-0.23.2rc1/src/eradiate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-05-16 13:35:25.000000 eradiate-0.23.2rc1/src/eradiate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21002 2023-05-16 13:35:25.000000 eradiate-0.23.2rc1/src/eradiate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:35:25.000000 eradiate-0.23.2rc1/src/eradiate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-16 13:35:25.000000 eradiate-0.23.2rc1/src/eradiate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-16 13:35:25.000000 eradiate-0.23.2rc1/src/eradiate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 13:35:25.000000 eradiate-0.23.2rc1/src/eradiate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.927456 eradiate-0.23.2rc1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.927456 eradiate-0.23.2rc1/tests/01_eradiate/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.927456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.931456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/test_blind_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/test_blind_online.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/test_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/test_open.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/test_safe_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/test_safe_online.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.931456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/experiments/test_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/experiments/test_canopy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/experiments/test_canopy_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/experiments/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/experiments/test_dem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/experiments/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.931456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/kernel/test_gridvolume.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/kernel/test_kernel_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/kernel/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/kernel/test_render.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/kernel/test_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.931456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/pipelines/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/pipelines/test_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/pipelines/test_assemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/pipelines/test_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/pipelines/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/pipelines/test_gather.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.931456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/radprops/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/radprops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/radprops/test_absorption.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/radprops/test_afgl_1986.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/radprops/test_rayleigh_scattering.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/radprops/test_us76_approx.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/radprops/test_zgrid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.931456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.935456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_heterogeneous.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_homogeneous.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_molecular_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.935456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)    10746 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_leaf_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.935456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_black.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_checkerboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_lambertian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_mqdiffuse.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_rpv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.935456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/illumination/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/illumination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/illumination/test_constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/illumination/test_directional.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/illumination/test_spot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.935456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/integrators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/integrators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/integrators/test_path_tracers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.935456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/measure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/measure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_distant_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_hemispherical_distant.py
--rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_multi_distant.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_multi_radiancemeter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_perspective.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_radiancemeter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.935456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/phase/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/phase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/phase/test_blend.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/phase/test_hg.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/phase/test_isotropic.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/phase/test_rayleigh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/phase/test_tabulated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.939456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/shapes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/shapes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/shapes/test_buffermesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/shapes/test_cuboid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/shapes/test_filemesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/shapes/test_rectangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/shapes/test_sphere.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.939456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/spectra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/spectra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/spectra/test_air_scattering_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/spectra/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/spectra/test_interpolated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/spectra/test_solar_irradiance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/spectra/test_uniform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.939456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/surface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/surface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/surface/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/surface/test_central_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/surface/test_dem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/test_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.939456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/spectral/
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/spectral/test_ckd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/spectral/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/spectral/test_mono.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_quad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_rng.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_srf_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.939456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_tools/test_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_units.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_warp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.939456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/thermoprops/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/thermoprops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/thermoprops/test_afgl1986.py
--rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/thermoprops/test_us76.py
--rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/thermoprops/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.939456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/util/test_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/util/test_misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.939456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/xarray/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/xarray/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/xarray/test_interp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.943456 eradiate-0.23.2rc1/tests/01_eradiate/02_system/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_albedo.py
--rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_atmosphere_ckd_vs_mono.py
--rw-r--r--   0 runner    (1001) docker     (123)    25312 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_atmosphere_rpv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_ckd_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_compare_canopy_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_expansion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_parameter_id_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_irradiance_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_kernel_render_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_maximum_scene_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_mdistant_insitu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_onedim_lambertian_brf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_onedim_phase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_onedim_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_spectral_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.943456 eradiate-0.23.2rc1/tests/01_eradiate/03_regression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/03_regression/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.943456 eradiate-0.23.2rc1/tests/01_eradiate/03_regression/atmospheres/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/03_regression/atmospheres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986_continental.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.943456 eradiate-0.23.2rc1/tests/01_eradiate/03_regression/rami4atm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/03_regression/rami4atm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/03_regression/rami4atm/test_rami4atm_hom00_bla_sd2s_m03_z30a000_brfpp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.943456 eradiate-0.23.2rc1/tests/01_eradiate/03_regression/romc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/03_regression/romc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/03_regression/romc/test_het01.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/03_regression/romc/test_het04.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/03_regression/romc/test_het06.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.430173 eradiate-0.23.2rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.338165 eradiate-0.23.2rc2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.338165 eradiate-0.23.2rc2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.338165 eradiate-0.23.2rc2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/.github/workflows/cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    18287 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7263 2023-06-21 16:12:21.430173 eradiate-0.23.2rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.338165 eradiate-0.23.2rc2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.338165 eradiate-0.23.2rc2/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/_ext/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/_ext/pluginparameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.342166 eradiate-0.23.2rc2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/_static/.keep
+-rw-r--r--   0 runner    (1001) docker     (123)    17013 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/_static/eradiate-logo-typo-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32795 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/_static/eradiate-logo-typo-black.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25531 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/_static/eradiate-logo-typo-darkgrey.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34059 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/_static/eradiate-logo-typo-darkgrey.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    18587 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/_static/eradiate-logo-typo-white.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34061 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/_static/eradiate-logo-typo-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/_static/theme_overrides.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.326164 eradiate-0.23.2rc2/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.342166 eradiate-0.23.2rc2/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/_templates/autosummary/module.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.342166 eradiate-0.23.2rc2/docs/_templates/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/_templates/sections/footer-content.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10467 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/convert_figures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.350166 eradiate-0.23.2rc2/docs/fig/
+-rw-r--r--   0 runner    (1001) docker     (123)    20540 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/atmosphere_attributes.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/atmosphere_attributes.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28149 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/azimuth-east_left.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32937 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/azimuth-east_left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28852 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/azimuth-east_right.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35278 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/azimuth-east_right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    30666 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/azimuth-north_left.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32862 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/azimuth-north_left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28115 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/azimuth-north_right.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32455 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/azimuth-north_right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28153 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/azimuth-south_left.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32939 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/azimuth-south_left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28118 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/azimuth-south_right.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32455 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/azimuth-south_right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28178 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/azimuth-west_left.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32935 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/azimuth-west_left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28067 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/azimuth-west_right.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32437 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/azimuth-west_right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/cartesian-coordinate-system.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15939 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/cartesian-coordinate-system.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25301 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/cuboid_leaf_cloud_params.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/cuboid_leaf_cloud_params.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.350166 eradiate-0.23.2rc2/docs/fig/diagrams/
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/diagrams/class_diagram_biosphere.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/diagrams/cuboid_leaf_cloud_params.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    20990 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/diagrams/package.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    40438 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/eradiate-logo-typo-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/eradiate-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/icon_eradiate.png
+-rw-r--r--   0 runner    (1001) docker     (123)    38873 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/package.png
+-rw-r--r--   0 runner    (1001) docker     (123)    57417 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/package.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    32384 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/radiancemeter_hsphere.png
+-rw-r--r--   0 runner    (1001) docker     (123)    43351 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/radiancemeter_hsphere.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    36773 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/radiancemeter_plane.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31853 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/radiancemeter_plane.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    31276 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/requirement_layers.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/requirement_layers.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    21451 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/solid_2017.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24994 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/spectral_discretization_ckd_atm_interval.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16459 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/spectral_discretization_ckd_atm_isolated.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28519 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/spectral_discretization_ckd_noatm_interval.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/spectral_discretization_ckd_noatm_isolated.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27127 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/spectral_discretization_mono_atm_interval.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/spectral_discretization_mono_atm_isolated.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46208 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/spectral_discretization_mono_noatm_interval1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14036 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/spectral_discretization_mono_noatm_interval2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21975 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/spectral_discretization_mono_noatm_isolated.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10036 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/spherical-coordinate-system.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19861 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/spherical-coordinate-system.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    20660 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/fig/thuillier_2003.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/generate_md_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/generate_rst_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/generate_rst_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/index_latex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    16528 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/references.bib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.350166 eradiate-0.23.2rc2/docs/rst/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/bibliography.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    22779 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/dependencies.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.350166 eradiate-0.23.2rc2/docs/rst/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/developer_guide/design_atmosphere.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/developer_guide/factory_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/developer_guide/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/developer_guide/lazy_loading.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/developer_guide/radiometric_kernel_interface.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/developer_guide/scene_generator.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/developer_guide/update.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14549 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/maintainer_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.354167 eradiate-0.23.2rc2/docs/rst/reference_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/attrs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/constants.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/contexts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/converters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/eradiate_core.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/experiments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/factory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/frame.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/kernel.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/mode.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/notebook.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/pipelines.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/plot.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/quad.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/radprops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/rng.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/scenes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/spectral.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/srf_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/test_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/thermoprops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/units.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/validators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/warp.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_api/xarray.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.354167 eradiate-0.23.2rc2/docs/rst/reference_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/reference_plugins/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.358167 eradiate-0.23.2rc2/docs/rst/user_guide/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.358167 eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/absorption.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.358167 eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/fig/
+-rw-r--r--   0 runner    (1001) docker     (123)    25171 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/fig/bad_resolution.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26889 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/fig/good_resolution.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24938 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/fig/line.png
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/heterogeneous.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/homogeneous.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/molecular.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/particle_layer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/rayleigh_scattering.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/basic_concepts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/conventions.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.362167 eradiate-0.23.2rc2/docs/rst/user_guide/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/data/absorption.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/data/atmosphere_radprops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/data/atmosphere_thermoprops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/data/ckd.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.362167 eradiate-0.23.2rc2/docs/rst/user_guide/data/fig/
+-rw-r--r--   0 runner    (1001) docker     (123)    30117 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/data/fig/p_interp_rerr_histo_65349.png
+-rw-r--r--   0 runner    (1001) docker     (123)    59107 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/data/fig/pt_points.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28580 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/data/fig/w_interp_rerr_histo_101325.png
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/data/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/data/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/data/particle_radprops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/data/solar_irradiance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/data/spectra-us76_u86_4.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/data/srf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/onedim_experiment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/package_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13015 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/spectral_discretization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/rst/user_guide/unit_guide_user.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.362167 eradiate-0.23.2rc2/docs/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    18287 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/src/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/docs/src/reference_cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.362167 eradiate-0.23.2rc2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/check_conda_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.366168 eradiate-0.23.2rc2/requirements/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)    22312 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-dependencies-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-dependencies-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-dependencies.dot
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-dependencies.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    41340 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-dev-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    32328 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-dev-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-dev.dot
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-dev.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    29544 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-docs-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    20325 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-docs-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-docs.dot
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    22312 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-main-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-main-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-main.dot
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    41340 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-optional-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    32328 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-optional-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-optional.dot
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-optional.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    20158 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-recommended-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    19689 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-recommended-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-recommended.dot
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-recommended.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    23014 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-tests-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    14040 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-tests-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-tests.dot
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/environment-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/conda/layer_graph.dot
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/copy_envvars.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/environment.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/layered.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/make_conda_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/make_pip_in_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.370168 eradiate-0.23.2rc2/requirements/pip/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/pip/dependencies.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/pip/dependencies.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/pip/dev.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/pip/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/pip/docs.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/pip/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/pip/main.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/pip/main.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/pip/optional.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20980 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/pip/optional.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/pip/recommended.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/pip/recommended.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/pip/tests.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/requirements/pip/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/setpath.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 16:12:21.430173 eradiate-0.23.2rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.330164 eradiate-0.23.2rc2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.374168 eradiate-0.23.2rc2/src/eradiate/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/attrs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.374168 eradiate-0.23.2rc2/src/eradiate/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/cli/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/cli/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/cli/srf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.378169 eradiate-0.23.2rc2/src/eradiate/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/data/_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/data/_blind_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/data/_blind_online.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/data/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/data/_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/data/_safe_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/data/_safe_online.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/data/_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16343 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/data/downloads.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/data/downloads_development.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.378169 eradiate-0.23.2rc2/src/eradiate/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/experiments/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/experiments/_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/experiments/_canopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12113 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/experiments/_canopy_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20760 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/experiments/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7795 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/experiments/_dem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/experiments/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12531 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/frame.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.382169 eradiate-0.23.2rc2/src/eradiate/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/kernel/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/kernel/_bitmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/kernel/_bsdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/kernel/_kernel_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/kernel/_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/kernel/gridvolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/kernel/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/kernel/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.382169 eradiate-0.23.2rc2/src/eradiate/notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/notebook/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/notebook/tutorials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.382169 eradiate-0.23.2rc2/src/eradiate/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/pipelines/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/pipelines/_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11488 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/pipelines/_assemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/pipelines/_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/pipelines/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/pipelines/_gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/quad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.382169 eradiate-0.23.2rc2/src/eradiate/radprops/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/radprops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/radprops/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/radprops/_afgl1986.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14982 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/radprops/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10705 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/radprops/_us76_approx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/radprops/_util_mono.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/radprops/absorption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/radprops/rayleigh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/rng.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.386170 eradiate-0.23.2rc2/src/eradiate/scenes/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.386170 eradiate-0.23.2rc2/src/eradiate/scenes/atmosphere/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/atmosphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/atmosphere/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23375 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/atmosphere/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/atmosphere/_heterogeneous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/atmosphere/_homogeneous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14639 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/atmosphere/_molecular_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/atmosphere/_particle_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/atmosphere/_particle_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.386170 eradiate-0.23.2rc2/src/eradiate/scenes/biosphere/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/biosphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/biosphere/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/biosphere/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12392 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/biosphere/_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38992 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/biosphere/_leaf_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17136 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/biosphere/_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.390170 eradiate-0.23.2rc2/src/eradiate/scenes/bsdfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/bsdfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/bsdfs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/bsdfs/_black.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/bsdfs/_checkerboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/bsdfs/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/bsdfs/_lambertian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/bsdfs/_mqdiffuse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/bsdfs/_opacity_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/bsdfs/_rpv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.390170 eradiate-0.23.2rc2/src/eradiate/scenes/illumination/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/illumination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/illumination/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/illumination/_astroobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/illumination/_constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/illumination/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/illumination/_directional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/illumination/_spot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.390170 eradiate-0.23.2rc2/src/eradiate/scenes/integrators/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/integrators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/integrators/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/integrators/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/integrators/_path_tracers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.394170 eradiate-0.23.2rc2/src/eradiate/scenes/measure/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/measure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/measure/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9555 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/measure/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/measure/_distant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/measure/_distant_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/measure/_hemispherical_distant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20874 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/measure/_multi_distant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/measure/_multi_radiancemeter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/measure/_perspective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/measure/_radiancemeter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.394170 eradiate-0.23.2rc2/src/eradiate/scenes/phase/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/phase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/phase/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12138 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/phase/_blend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/phase/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/phase/_hg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/phase/_isotropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/phase/_rayleigh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/phase/_tabulated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.394170 eradiate-0.23.2rc2/src/eradiate/scenes/shapes/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/shapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/shapes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/shapes/_buffermesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/shapes/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/shapes/_cuboid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/shapes/_filemesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/shapes/_rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/shapes/_sphere.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.398171 eradiate-0.23.2rc2/src/eradiate/scenes/spectra/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/spectra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/spectra/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/spectra/_air_scattering_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9743 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/spectra/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12948 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/spectra/_interpolated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/spectra/_multi_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/spectra/_solar_irradiance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/spectra/_uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.398171 eradiate-0.23.2rc2/src/eradiate/scenes/surface/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/surface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/surface/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/surface/_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/surface/_central_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/surface/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18023 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/scenes/surface/_dem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.398171 eradiate-0.23.2rc2/src/eradiate/spectral/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/spectral/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/spectral/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/spectral/ckd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/spectral/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/spectral/mono.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26485 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/srf_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.398171 eradiate-0.23.2rc2/src/eradiate/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/test_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/test_tools/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/test_tools/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/test_tools/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/test_tools/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.402171 eradiate-0.23.2rc2/src/eradiate/thermoprops/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/thermoprops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/thermoprops/afgl_1986.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42061 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/thermoprops/us76.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22124 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/thermoprops/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.402171 eradiate-0.23.2rc2/src/eradiate/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/util/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15100 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/util/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/util/numpydoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/util/sys_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/warp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.402171 eradiate-0.23.2rc2/src/eradiate/xarray/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/xarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/xarray/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/xarray/_accessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/xarray/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/src/eradiate/xarray/interp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.374168 eradiate-0.23.2rc2/src/eradiate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7263 2023-06-21 16:12:21.000000 eradiate-0.23.2rc2/src/eradiate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22346 2023-06-21 16:12:21.000000 eradiate-0.23.2rc2/src/eradiate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:12:21.000000 eradiate-0.23.2rc2/src/eradiate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-21 16:12:21.000000 eradiate-0.23.2rc2/src/eradiate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-21 16:12:21.000000 eradiate-0.23.2rc2/src/eradiate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 16:12:21.000000 eradiate-0.23.2rc2/src/eradiate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.402171 eradiate-0.23.2rc2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.402171 eradiate-0.23.2rc2/tests/01_eradiate/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.406171 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.406171 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/test_blind_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/test_blind_online.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/test_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/test_safe_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/test_safe_online.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.406171 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8354 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/experiments/test_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/experiments/test_canopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/experiments/test_canopy_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/experiments/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/experiments/test_dem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/experiments/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.410172 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/kernel/test_gridvolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/kernel/test_kernel_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/kernel/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/kernel/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/kernel/test_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.410172 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/pipelines/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/pipelines/test_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/pipelines/test_assemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/pipelines/test_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/pipelines/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/pipelines/test_gather.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.410172 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/radprops/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/radprops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/radprops/test_absorption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/radprops/test_afgl_1986.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/radprops/test_rayleigh_scattering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/radprops/test_us76_approx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/radprops/test_zgrid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.410172 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.414172 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/atmosphere/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/atmosphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/atmosphere/test_heterogeneous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/atmosphere/test_homogeneous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/atmosphere/test_molecular_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.414172 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/biosphere/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/biosphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/biosphere/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/biosphere/test_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10746 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/biosphere/test_leaf_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.414172 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/bsdfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/bsdfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/bsdfs/test_black.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/bsdfs/test_checkerboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/bsdfs/test_lambertian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/bsdfs/test_mqdiffuse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/bsdfs/test_rpv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.414172 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/illumination/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/illumination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/illumination/test_astroobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/illumination/test_constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/illumination/test_directional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/illumination/test_spot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.418172 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/integrators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/integrators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/integrators/test_path_tracers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.418172 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/measure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/measure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/measure/test_distant_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/measure/test_hemispherical_distant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/measure/test_multi_distant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/measure/test_multi_radiancemeter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/measure/test_perspective.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/measure/test_radiancemeter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/measure/test_target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.418172 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/phase/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/phase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/phase/test_blend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/phase/test_hg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/phase/test_isotropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/phase/test_rayleigh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/phase/test_tabulated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.418172 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/shapes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/shapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/shapes/test_buffermesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/shapes/test_cuboid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/shapes/test_filemesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/shapes/test_rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/shapes/test_sphere.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.422173 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/spectra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/spectra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/spectra/test_air_scattering_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/spectra/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/spectra/test_interpolated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/spectra/test_solar_irradiance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/spectra/test_uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.422173 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/surface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/surface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/surface/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/surface/test_central_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/surface/test_dem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.422173 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/spectral/
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/spectral/test_ckd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/spectral/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/spectral/test_mono.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_rng.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_srf_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.422173 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_tools/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_warp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.422173 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/thermoprops/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/thermoprops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/thermoprops/test_afgl1986.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/thermoprops/test_us76.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/thermoprops/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.422173 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/util/test_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/util/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.422173 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/xarray/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/xarray/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/01_unit/xarray/test_interp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.426173 eradiate-0.23.2rc2/tests/01_eradiate/02_system/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_albedo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_atmosphere_ckd_vs_mono.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25312 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_atmosphere_rpv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_ckd_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_compare_canopy_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_parameter_id_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_irradiance_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_kernel_render_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_maximum_scene_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_mdistant_insitu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_onedim_lambertian_brf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_onedim_phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_onedim_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_spectral_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.426173 eradiate-0.23.2rc2/tests/01_eradiate/03_regression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/03_regression/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.430173 eradiate-0.23.2rc2/tests/01_eradiate/03_regression/atmospheres/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/03_regression/atmospheres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986_continental.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.430173 eradiate-0.23.2rc2/tests/01_eradiate/03_regression/rami4atm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/03_regression/rami4atm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/03_regression/rami4atm/test_rami4atm_hom00_bla_sd2s_m03_z30a000_brfpp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:21.430173 eradiate-0.23.2rc2/tests/01_eradiate/03_regression/romc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/03_regression/romc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/03_regression/romc/test_het01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/03_regression/romc/test_het04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/03_regression/romc/test_het06.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/01_eradiate/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-21 16:12:07.000000 eradiate-0.23.2rc2/tests/conftest.py
```

### Comparing `eradiate-0.23.2rc1/.clang-format` & `eradiate-0.23.2rc2/.clang-format`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/.github/ISSUE_TEMPLATE/bug_report.md` & `eradiate-0.23.2rc2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/.github/ISSUE_TEMPLATE/feature_request.md` & `eradiate-0.23.2rc2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/.github/pull_request_template.md` & `eradiate-0.23.2rc2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/.github/workflows/cd.yml` & `eradiate-0.23.2rc2/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/.github/workflows/ci.yml` & `eradiate-0.23.2rc2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/.pre-commit-config.yaml` & `eradiate-0.23.2rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/.readthedocs.yml` & `eradiate-0.23.2rc2/.readthedocs.yml`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   os: ubuntu-22.04
   tools:
     # Use Mamba for quicker setup
     python: mambaforge-4.10
 
 conda:
   # Setup Conda env with dev dependencies
-  environment: requirements/environment-dev.yml
+  environment: requirements/conda/environment-dev.yml
 
 python:
   # Install Eradiate package in Conda env
   install:
     - method: pip
       path: .
 
@@ -24,8 +24,9 @@
   builder: html
   configuration: docs/conf.py
 
 submodules:
   include:
     - resources/data
     - tutorials
+    - ext/mitsuba
   recursive: true
```

### Comparing `eradiate-0.23.2rc1/CHANGELOG.md` & `eradiate-0.23.2rc2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,21 @@
 ### Improvements and fixes
 
 * Added {class}`.MultiDeltaSpectrum` spectrum type ({ghpr}`311`).
 * Exposed several API members in the top-level namespace ({ghpr}`324`).
 * Exposed the ``eradiate.spectral.*`` subpackage members in the
   {mod}`eradiate.spectral` namespace ({ghpr}`324`).
 * Fixed incorrect Mitsuba scene parameter drop and lookup ({ghpr}`329`).
-* Provide an Eradiate Pypi package ({ghpr}`328`)
+* Added spherical-shell geometry support to DEM components
+  {ghpr}`320`.
+* Fixed broken symmetry between {class}`.Spectrum` dictionary and object
+  conversion protocols ({ghpr}`336`).
+* Provide an Eradiate Pypi package ({ghpr}`328`).
+* Implement the Astronomical Object Illumination, its tests and its
+  documentation ({ghpr}`331`).
 
 ### Documentation
 
 * Added a user guide page on spectral discretization.
 
 ### Internal changes
```

### Comparing `eradiate-0.23.2rc1/CONTRIBUTING.md` & `eradiate-0.23.2rc2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/LICENSE` & `eradiate-0.23.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/Makefile` & `eradiate-0.23.2rc2/Makefile`

 * *Files 22% similar despite different names*

```diff
@@ -26,75 +26,85 @@
 pip-update-in-files:
 	python3 requirements/make_pip_in_files.py --quiet
 
 # Lock pip dependencies
 # Dev must be compiled first because it constrains the others
 # No hashes: doesn't play nicely with RTD when running pip-compile on macOS
 pip-compile: pip-update-in-files
-	rm requirements/dev.txt
-	touch requirements/dev.txt
+	rm requirements/pip/dev.txt
+	touch requirements/pip/dev.txt
 
-	@for LAYER in dev main docs tests production optional; do \
-		echo "Compiling requirements/$${LAYER}.in to requirements/$${LAYER}.txt"; \
+	@for LAYER in dev dependencies main recommended tests docs optional; do \
+		echo "Compiling requirements/pip/$${LAYER}.in to requirements/pip/$${LAYER}.txt"; \
 		pip-compile --upgrade --resolver=backtracking --build-isolation --allow-unsafe \
-			--output-file requirements/$${LAYER}.txt \
-			requirements/$${LAYER}.in; \
+			--output-file requirements/pip/$${LAYER}.txt \
+			requirements/pip/$${LAYER}.in; \
 	done
 
 # Lock dependencies
 pip-lock: pip-update-tools pip-compile
 
 # Initialise development environment
 pip-init:
-	pip install --upgrade -r requirements/dev.txt
+	pip install --upgrade -r requirements/pip/dev.txt
 	pip install --editable . --no-deps
 
 pip-update: pip-lock pip-init
 
 .PHONY: pip-compile pip-update-tools pip-update-deps pip-init pip-update-in-files
 
 # -- Dependency management with Conda ------------------------------------------
 
-# Generate environment files from pyproject.toml
+# Generate environment files
 conda-env:
-	python3 requirements/make_conda_env.py \
-	    -s "main" \
-	    -o requirements/environment-minimal.yml --quiet
-	python3 requirements/make_conda_env.py \
-	    -s "main,recommended" \
-	    -o requirements/environment-recommended.yml --quiet
-	python3 requirements/make_conda_env.py \
-		-s "main,recommended,docs,dev" \
-	    -o requirements/environment-dev.yml --quiet
-	python3 requirements/make_conda_env.py \
-		-s "main,recommended,docs,dev,optional" \
-	    -o requirements/environment-optional.yml --quiet
-	python3 requirements/make_conda_env.py \
-		-s "main,recommended,production" \
-	    -o requirements/environment-production.yml --quiet
+	python3 requirements/make_conda_env.py --quiet;
 
 # Lock conda dependencies
 conda-lock: conda-env
-	conda-lock --kind explicit --no-mamba --file requirements/environment-dev.yml \
-	    --filename-template "requirements/environment-{platform}.lock" \
-	    -p $(PLATFORM)
+	@for LAYER in dev dependencies main recommended tests docs optional; do \
+		conda-lock --kind explicit --no-mamba --file requirements/conda/environment-$${LAYER}.yml \
+			--filename-template "requirements/conda/environment-$${LAYER}-{platform}.lock" \
+			-p $(PLATFORM); \
+	done
 
 conda-lock-all: conda-env
-	conda-lock --kind explicit --no-mamba --file requirements/environment-dev.yml \
-	    --filename-template "requirements/environment-{platform}.lock" \
-	    -p osx-64 -p linux-64
+	@for LAYER in dev dependencies main recommended tests docs optional; do \
+		conda-lock --kind explicit --no-mamba --file requirements/conda/environment-$${LAYER}.yml \
+			--filename-template "requirements/conda/environment-$${LAYER}-{platform}.lock" \
+			-p osx-64 -p linux-64; \
+	done
 
-# Initialise development environment
-conda-init:
+conda-prepare:
 	python3 requirements/check_conda_env.py
 	conda config --env --add channels conda-forge --add channels eradiate
-	conda update --file requirements/environment-$(PLATFORM).lock
+
+install-no-deps:
 	python3 requirements/copy_envvars.py
 	pip install --editable . --no-deps
 
+# Initialise development environment
+conda-init: conda-prepare
+	conda update --file requirements/conda/environment-dev-$(PLATFORM).lock
+	$(MAKE) no-deps-install
+
+# Initialise docs building environment
+conda-init-docs: conda-prepare
+	conda update --file requirements/conda/environment-docs-$(PLATFORM).lock
+	$(MAKE) no-deps-install
+
+# Initialise tests environment
+conda-init-tests: conda-prepare
+	conda update --file requirements/conda/environment-tests-$(PLATFORM).lock
+	$(MAKE) no-deps-install
+
+# Initialise production environment
+conda-init-prod: conda-prepare
+	conda update --file requirements/conda/environment-dependencies-$(PLATFORM).lock
+	$(MAKE) no-deps-install
+
 conda-update: conda-lock-all conda-init
 
 .PHONY: conda-env conda-lock conda-lock-all conda-init conda-update
 
 # -- Build the Eradiate Mitsuba kernel -----------------------------------------
 
 kernel:
```

### Comparing `eradiate-0.23.2rc1/PKG-INFO` & `eradiate-0.23.2rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 Metadata-Version: 2.1
 Name: eradiate
-Version: 0.23.2rc1
+Version: 0.23.2rc2
 Summary: A radiative transfer model for the Earth observation community
 Author: The Eradiate Team
 Maintainer: The Eradiate Team
 License: LGPLv3
 Project-URL: changelog, https://github.com/eradiate/eradiate/CHANGELOG.md
 Project-URL: documentation, https://eradiate.readthedocs.io
 Project-URL: repository, https://github.com/eradiate/eradiate
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: docs
 Provides-Extra: recommended
-Provides-Extra: tests
-Provides-Extra: optional
-Provides-Extra: production
 License-File: LICENSE
 
 ![Eradiate logo](docs/fig/eradiate-logo.svg "Eradiate — A new-generation radiative transfer simulation package")
 
 # Eradiate Radiative Transfer Model
 
 [![docs][rtd-badge]][rtd-url]
```

### Comparing `eradiate-0.23.2rc1/README.md` & `eradiate-0.23.2rc2/README.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/Makefile` & `eradiate-0.23.2rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/_ext/exec.py` & `eradiate-0.23.2rc2/docs/_ext/exec.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/_ext/pluginparameters.py` & `eradiate-0.23.2rc2/docs/_ext/pluginparameters.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/_static/eradiate-logo-typo-black.png` & `eradiate-0.23.2rc2/docs/_static/eradiate-logo-typo-black.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/_static/eradiate-logo-typo-black.svg` & `eradiate-0.23.2rc2/docs/_static/eradiate-logo-typo-black.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/_static/eradiate-logo-typo-darkgrey.png` & `eradiate-0.23.2rc2/docs/_static/eradiate-logo-typo-darkgrey.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/_static/eradiate-logo-typo-darkgrey.svg` & `eradiate-0.23.2rc2/docs/_static/eradiate-logo-typo-darkgrey.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/_static/eradiate-logo-typo-white.png` & `eradiate-0.23.2rc2/docs/_static/eradiate-logo-typo-white.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/_static/eradiate-logo-typo-white.svg` & `eradiate-0.23.2rc2/docs/_static/eradiate-logo-typo-white.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/_templates/autosummary/module.rst` & `eradiate-0.23.2rc2/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/_templates/sections/footer-content.html` & `eradiate-0.23.2rc2/docs/_templates/sections/footer-content.html`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/conf.py` & `eradiate-0.23.2rc2/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import sys
 import unittest.mock as mock
 from importlib.metadata import version
 
 # -- Mock Mitsuba modules (required to render CLI reference on RTD) ------------
 
-MOCK_MODULES = ["mitsuba", "mitsuba.scalar_rgb", "drjit"]
+MOCK_MODULES = []
 for mod_name in MOCK_MODULES:
     sys.modules[mod_name] = mock.Mock()
 
 # -- Path setup ----------------------------------------------------------------
 
 # sys.path.insert(0, os.path.abspath('.'))
 sys.path.append(os.path.abspath("./_ext"))
@@ -124,15 +124,15 @@
 ]
 autodoc_typehints = "none"
 autodoc_member_order = "groupwise"
 autodoc_preserve_defaults = False
 
 # Mitsuba modules must be mocked in order to allow compiling docs even if they're not here;
 # this mocking is also done in the ertdocs extension
-autodoc_mock_imports = ["drjit", "mitsuba"]
+autodoc_mock_imports = []
 
 # Autosummary tables in autodoc
 # https://autodocsumm.readthedocs.io/en/latest
 autodoc_default_options = {
     # "autosummary": False,
 }
```

### Comparing `eradiate-0.23.2rc1/docs/fig/atmosphere_attributes.png` & `eradiate-0.23.2rc2/docs/fig/atmosphere_attributes.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/atmosphere_attributes.svg` & `eradiate-0.23.2rc2/docs/fig/atmosphere_attributes.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/azimuth-east_left.png` & `eradiate-0.23.2rc2/docs/fig/azimuth-east_left.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/azimuth-east_left.svg` & `eradiate-0.23.2rc2/docs/fig/azimuth-east_left.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/azimuth-east_right.png` & `eradiate-0.23.2rc2/docs/fig/azimuth-east_right.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/azimuth-east_right.svg` & `eradiate-0.23.2rc2/docs/fig/azimuth-east_right.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/azimuth-north_left.png` & `eradiate-0.23.2rc2/docs/fig/azimuth-north_left.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/azimuth-north_left.svg` & `eradiate-0.23.2rc2/docs/fig/azimuth-north_left.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/azimuth-north_right.png` & `eradiate-0.23.2rc2/docs/fig/azimuth-north_right.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/azimuth-north_right.svg` & `eradiate-0.23.2rc2/docs/fig/azimuth-north_right.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/azimuth-south_left.png` & `eradiate-0.23.2rc2/docs/fig/azimuth-south_left.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/azimuth-south_left.svg` & `eradiate-0.23.2rc2/docs/fig/azimuth-south_left.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/azimuth-south_right.png` & `eradiate-0.23.2rc2/docs/fig/azimuth-south_right.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/azimuth-south_right.svg` & `eradiate-0.23.2rc2/docs/fig/azimuth-south_right.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/azimuth-west_left.png` & `eradiate-0.23.2rc2/docs/fig/azimuth-west_left.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/azimuth-west_left.svg` & `eradiate-0.23.2rc2/docs/fig/azimuth-west_left.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/azimuth-west_right.png` & `eradiate-0.23.2rc2/docs/fig/azimuth-west_right.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/azimuth-west_right.svg` & `eradiate-0.23.2rc2/docs/fig/azimuth-west_right.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/cartesian-coordinate-system.png` & `eradiate-0.23.2rc2/docs/fig/cartesian-coordinate-system.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/cartesian-coordinate-system.svg` & `eradiate-0.23.2rc2/docs/fig/cartesian-coordinate-system.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/cuboid_leaf_cloud_params.png` & `eradiate-0.23.2rc2/docs/fig/cuboid_leaf_cloud_params.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/cuboid_leaf_cloud_params.svg` & `eradiate-0.23.2rc2/docs/fig/cuboid_leaf_cloud_params.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/diagrams/class_diagram_biosphere.drawio` & `eradiate-0.23.2rc2/docs/fig/diagrams/class_diagram_biosphere.drawio`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/diagrams/cuboid_leaf_cloud_params.drawio` & `eradiate-0.23.2rc2/docs/fig/diagrams/cuboid_leaf_cloud_params.drawio`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/diagrams/package.drawio` & `eradiate-0.23.2rc2/docs/fig/diagrams/package.drawio`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/eradiate-logo-typo-black.png` & `eradiate-0.23.2rc2/docs/fig/eradiate-logo-typo-black.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/eradiate-logo.svg` & `eradiate-0.23.2rc2/docs/fig/eradiate-logo.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/icon_eradiate.png` & `eradiate-0.23.2rc2/docs/fig/icon_eradiate.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/package.png` & `eradiate-0.23.2rc2/docs/fig/package.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/package.svg` & `eradiate-0.23.2rc2/docs/fig/package.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/radiancemeter_hsphere.png` & `eradiate-0.23.2rc2/docs/fig/radiancemeter_hsphere.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/radiancemeter_hsphere.svg` & `eradiate-0.23.2rc2/docs/fig/radiancemeter_hsphere.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/radiancemeter_plane.png` & `eradiate-0.23.2rc2/docs/fig/radiancemeter_plane.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/radiancemeter_plane.svg` & `eradiate-0.23.2rc2/docs/fig/radiancemeter_plane.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/solid_2017.png` & `eradiate-0.23.2rc2/docs/fig/solid_2017.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/spectral_discretization_ckd_atm_interval.png` & `eradiate-0.23.2rc2/docs/fig/spectral_discretization_ckd_atm_interval.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/spectral_discretization_ckd_atm_isolated.png` & `eradiate-0.23.2rc2/docs/fig/spectral_discretization_ckd_atm_isolated.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/spectral_discretization_ckd_noatm_interval.png` & `eradiate-0.23.2rc2/docs/fig/spectral_discretization_ckd_noatm_interval.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/spectral_discretization_ckd_noatm_isolated.png` & `eradiate-0.23.2rc2/docs/fig/spectral_discretization_ckd_noatm_isolated.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/spectral_discretization_mono_atm_interval.png` & `eradiate-0.23.2rc2/docs/fig/spectral_discretization_mono_atm_interval.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/spectral_discretization_mono_atm_isolated.png` & `eradiate-0.23.2rc2/docs/fig/spectral_discretization_mono_atm_isolated.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/spectral_discretization_mono_noatm_interval1.png` & `eradiate-0.23.2rc2/docs/fig/spectral_discretization_mono_noatm_interval1.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/spectral_discretization_mono_noatm_interval2.png` & `eradiate-0.23.2rc2/docs/fig/spectral_discretization_mono_noatm_interval2.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/spectral_discretization_mono_noatm_isolated.png` & `eradiate-0.23.2rc2/docs/fig/spectral_discretization_mono_noatm_isolated.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/spherical-coordinate-system.png` & `eradiate-0.23.2rc2/docs/fig/spherical-coordinate-system.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/spherical-coordinate-system.svg` & `eradiate-0.23.2rc2/docs/fig/spherical-coordinate-system.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/fig/thuillier_2003.png` & `eradiate-0.23.2rc2/docs/fig/thuillier_2003.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/generate_md_cli.py` & `eradiate-0.23.2rc2/docs/generate_md_cli.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/generate_rst_api.py` & `eradiate-0.23.2rc2/docs/generate_rst_api.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/generate_rst_plugins.py` & `eradiate-0.23.2rc2/docs/generate_rst_plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,17 @@
     ],
     "sensors": [
         "distantflux",
         "hdistant",
         "mdistant",
         "mradiancemeter",
     ],
+    "emitters": [
+        "astroobject",
+    ],
 }
 
 
 def write_if_modified(filename, content):
     filename.parent.mkdir(parents=True, exist_ok=True)
 
     try:
@@ -86,30 +89,30 @@
     return ("\n".join(result)).lstrip()
 
 
 def make_toc(section, title) -> str:
     return dedent(
         rf"""
         .. _sec-reference_plugins-{section}:
-        
+
         {title}
         {underline(title)}
-        
+
         .. toctree::
            :maxdepth: 1
            :glob:
-        
+
            ../plugins/{section}/*
         """
     )
 
 
 def generate():
     root_dir = Path(__file__).absolute().parent.parent
-    plugin_dir = root_dir / "src/plugins/src"
+    plugin_dir = root_dir / "ext/mitsuba/src/eradiate_plugins"
     out_dir = root_dir / "docs/rst/reference_plugins/generated"
     print(f"Generating plugin docs in '{out_dir}'")
 
     for section, section_title in SECTIONS.items():
         try:
             plugin_order = PLUGIN_ORDERS[section]
         except KeyError:
```

### Comparing `eradiate-0.23.2rc1/docs/index.rst` & `eradiate-0.23.2rc2/docs/index.rst`

 * *Files 13% similar despite different names*

```diff
@@ -19,45 +19,38 @@
 Python and C++17. It relies on a radiometric kernel based on the
 `Mitsuba 3 <https://github.com/mitsuba-renderer/mitsuba3>`_ rendering system
 :cite:`Jakob2022DrJit,Jakob2022Mitsuba3`.
 
 .. grid:: 1 2 auto auto
    :gutter: 3
 
-   .. grid-item-card:: :fas:`download` Getting started
-      :link: sec-getting_started
+   .. grid-item-card:: :fas:`download` User Guide
+      :link: sec-user_guide
       :link-type: ref
 
-      Learn about Eradiate, how to get it and how to compile it.
+      Learn about Eradiate, how to get it and how to use it.
 
    .. grid-item-card:: :fas:`graduation-cap` Tutorials
       :link: sec-tutorials
       :link-type: ref
 
       A practical introduction to Eradiate.
 
-   .. grid-item-card:: :fas:`book` User guide
-      :link: sec-user_guide
-      :link-type: ref
-
-      Learn how to use Eradiate.
-
    .. grid-item-card:: :fas:`file-code` Reference
       :link: sec-reference_api
       :link-type: ref
 
       The complete reference.
 
 .. toctree::
    :maxdepth: 3
    :hidden:
    :titlesonly:
    :caption: Users
 
-   rst/getting_started/index
    rst/user_guide/index
    tutorials/index
 
 .. toctree::
    :maxdepth: 3
    :hidden:
    :titlesonly:
```

### Comparing `eradiate-0.23.2rc1/docs/make.bat` & `eradiate-0.23.2rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/references.bib` & `eradiate-0.23.2rc2/docs/references.bib`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/contributing.rst` & `eradiate-0.23.2rc2/docs/rst/contributing.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/dependencies.rst` & `eradiate-0.23.2rc2/docs/rst/dependencies.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/developer_guide/design_atmosphere.rst` & `eradiate-0.23.2rc2/docs/rst/developer_guide/design_atmosphere.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/developer_guide/factory_guide.rst` & `eradiate-0.23.2rc2/docs/rst/developer_guide/factory_guide.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/developer_guide/lazy_loading.rst` & `eradiate-0.23.2rc2/docs/rst/developer_guide/lazy_loading.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/developer_guide/radiometric_kernel_interface.rst` & `eradiate-0.23.2rc2/docs/rst/developer_guide/radiometric_kernel_interface.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/developer_guide/scene_generator.rst` & `eradiate-0.23.2rc2/docs/rst/developer_guide/scene_generator.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/getting_started/index.rst` & `eradiate-0.23.2rc2/docs/rst/user_guide/index.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,23 @@
-.. _sec-getting_started:
+.. _sec-user_guide:
 
-Getting started
-===============
+User guides
+===========
 
 .. toctree::
    :maxdepth: 1
-   :hidden:
 
    install
-   update
+   basic_concepts
+   conventions
+   package_structure
+   onedim_experiment
+   spectral_discretization
+   unit_guide_user
+   data/index
 
 What is Eradiate?
 -----------------
 
 Eradiate is a modern radiative transfer model for Earth observation
 applications. It primarily targets calibration/validation applications and
 focuses on delivering highly accurate results.
@@ -44,8 +49,8 @@
     Eradiate can simulate top-of-canopy/atmosphere radiance on 3D scenes
     consisting of a vegetated ground patch with or without atmosphere above it
     (plane parallel geometry only).
 
 .. seealso::
 
    For a full list of features, head to
-   `our website <https://www.eradiate.eu/>`_.
+   `our website <https://www.eradiate.eu/>`_.
```

### Comparing `eradiate-0.23.2rc1/docs/rst/getting_started/install.rst` & `eradiate-0.23.2rc2/docs/rst/developer_guide/getting_started.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,17 @@
-.. _sec-getting_started-install:
+.. _sec-getting_started-development:
 
-Installation guide
-==================
+Development installation
+========================
 
-This guide covers all steps necessary to get Eradiate running on your machine.
-
-.. warning::
-
-   Eradiate currently requires a development setup, even for end-users. This has
-   a few consequences which we hope to overcome in the future:
-
-   * installing and running Eradiate requires to use the Conda package and
-     environment manager;
-   * installation requires many dependencies not necessarily useful to
-     end-users;
-   * integrating Eradiate in your workflow can be a bit constraining if you have
-     specific requirements on package versions.
+This guide covers all steps necessary to get Eradiate running on your machine in
+development mode. This mode allows for easy code modifications and testing, as
+well as for developing on the kernel code. It requires to compile the C++ code
+of the Mitsuba renderer, using the Eradiate specific plugins and the appropriate
+variants.
 
 Prerequisites
 -------------
 
 Before cloning the Git repository and compiling the code, ensure that your
 machine meets the requirements listed below.
 
@@ -228,19 +220,19 @@
    conda deactivate && conda activate eradiate
 
 .. _sec-getting_started-install-compiling:
 
 Compiling the radiometric kernel
 --------------------------------
 
-Configure CMake for compilation:
+Using the Makefile rule to build the kernel is the recommended way to compile.
 
 .. code:: bash
 
-   cmake --preset default
+   make kernel
 
 .. dropdown:: CMake Error: The source directory "..." does not exist
    :color: info
    :icon: info
 
    This most probably means that your CMake version is too old
    (see `Prerequisites`_). At this stage, you might also install CMake in your
@@ -283,34 +275,14 @@
          :sync: macos
 
          .. code:: bash
 
             export CC=clang
             export CXX=clang++
 
-   You might want to add these commands to your environment profile loading
-   script. If you don't want to modify your environment variables, you can
-   alternatively specify compilers during CMake configuration using CMake
-   variables:
-
-   .. tab-set::
-
-      .. tab-item:: Linux
-         :sync: linux
-
-          .. code:: bash
-
-             cmake --preset default -DCMAKE_C_COMPILER=clang-11 -DCMAKE_CXX_COMPILER=clang++-11
-
-      .. tab-item:: macOS
-         :sync: macos
-
-          .. code:: bash
-
-             cmake --preset default -DCMAKE_C_COMPILER=clang -DCMAKE_CXX_COMPILER=clang++
 
 Inspect CMake's output to check if your Conda environment Python is used by
 CMake. Search for a line starting with:
 
 .. tab-set::
 
       .. tab-item:: Linux
@@ -347,20 +319,14 @@
 
        *Created a default 'mitsuba.conf' configuration file.  You will
        probably want to edit this file to specify the desired configurations
        before starting to compile.*
 
    This is expected: do not worry about it.
 
-When CMake is successfully configured, you can compile the code:
-
-.. code:: bash
-
-   cmake --build build
-
 The compilation process can last for up to around half an hour on old machines.
 It completes within a few minutes on modern workstations.
 
 .. _sec-getting_started-install-verify_installation:
 
 Verifying the installation
 --------------------------
```

### Comparing `eradiate-0.23.2rc1/docs/rst/getting_started/update.rst` & `eradiate-0.23.2rc2/docs/rst/developer_guide/update.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/maintainer_guide.rst` & `eradiate-0.23.2rc2/docs/rst/maintainer_guide.rst`

 * *Files 6% similar despite different names*

```diff
@@ -183,70 +183,80 @@
 
 * `conda-lock <https://github.com/conda-incubator/conda-lock>`_
 * `pip-tools <https://github.com/jazzband/pip-tools>`_
 
 Basic principles
 ^^^^^^^^^^^^^^^^
 
-We categorise our dependencies in five sets:
+We categorize our dependencies in five layers:
 
-* ``main``: dependencies strictly required to run Eradiate as a user;
-* ``recommended``: dependencies recommended to run Eradiate as a user;
-* ``docs``: dependencies required to compile the documentation;
-* ``tests``: dependencies required to run tests;
+* ``main``: minimal requirements for eradiate to run in development mode
+* ``recommended``: convenient optional dependencies included in the production package. Installable through PyPI.
+* ``docs``: dependencies required to compile the docs in development mode
+* ``tests``: dependencies required for testing eradiate in development mode
 * ``dev``: dependencies specific to a development setup.
+* ``dependencies``: dependency list used by default by Setuptools in production packages. Includes the ``eradiate-mitsuba`` package. Used by users who install Eradiate through PyPI.
+* ``optional``: convenience development dependencies, including the ``eradiate-mitsuba`` package.
 
-``main``, ``recommended`` and ``docs`` and ``tests`` are subsets of ``dev``:
+Layers can include other layers. As a result, we have the following layer Directed Acyclic Graph (DAG):
 
-- ``recommended`` includes ``main``;
 - ``docs`` includes ``main``;
 - ``tests`` includes ``main``;
 - ``dev`` includes ``recommended``, ``docs`` and ``tests``.
+- ``dependencies`` includes ``main``;
+- ``optional`` includes ``dev``;
+
+The following figure illustrates the layer DAG:
 
 .. only:: latex
 
    .. figure:: ../fig/requirement_layers.png
 
 .. only:: not latex
 
    .. figure:: ../fig/requirement_layers.svg
 
-The sets are defined in ``pyproject.toml``, where direct dependencies are
+The sets are defined in ``requirements/layered.yml``, where direct dependencies are
 specified with minimal constraint.
 
 .. warning:: This is the location from which all dependencies are sourced.
-   Dependencies shoud all be specified only in ``pyproject.toml``.
+   Dependencies shoud all be specified only in ``requirements/layered.yml``.
 
 We then have processes which will compile these dependencies into transitively
 pinned dependencies and write them as requirement (lock) files. The Conda and
 Pip pinning processes are different.
 
 The generated lock files are versioned and come along the source code they were
 used to write. Thus, a developer cloning the codebase will also get the
 information they need to reproduce the same environment as the other developers.
 
+The project's ``pyproject.toml`` file defines the metadata used by the Eradiate wheels.
+It thus includes the necessary pip lock files for production/users setups. These are
+the ``dependencies`` layer pip lock file, which includes the eradiate-mitsuba package, and
+the ``recommended`` layer pip lock file, as an optional dependency set.
+
 Lock files
 ^^^^^^^^^^
 
 Lock files are stored in the ``requirements`` directory, alongside a series of
 utility scripts.
 
 * **Conda** dependencies are pinned using conda-lock. It uses a regular
   environment YAML file as input. It can compile requirements for multiple
   platforms, but cannot be used to extract subsets of an existing requirement
   specification. The ``environment-dev.yml`` file is created by the
   ``make_conda_env.py`` script, from a header ``environment.in`` and the data
-  found in ``pyproject.toml``. Our Conda lock files use the extension ``.lock``.
+  found in ``requirements/layered.yml``. Our Conda lock files use the extension ``.lock``.
 * **Pip** dependencies are pinned using pip-tools. It uses a series of ``*.in``
-  files as input (one per requirement set) which can be configured to define
+  files as input (one per requirement layer) which can be configured to define
   subsets of each other, but cannot compile requirements for multiple platforms,
   which basically means that we cannot use hashes to pin requirements with it.
   The ``*.in`` input files are created by the ``make_pip_in_files.py`` script
-  from the data found in ``pyproject.toml`` and the requirement layer relations
-  defined in the ``layered.yml`` file. Our Pip lock files use the extension
+  from the data found in ``requirements/layered.yml`` and the requirement layer relations
+  defined in the ``requirements/layered.yml`` file. Our Pip lock files use the extension
   ``.txt``.
 
 We can already see at this point that neither tool will perfectly fulfill our
 requirements, but the limitations we have observed so far have not (yet)
 proven to be critical.
 
 Initialising or updating an environment
```

### Comparing `eradiate-0.23.2rc1/docs/rst/reference_api/data.rst` & `eradiate-0.23.2rc2/docs/rst/reference_api/data.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/reference_api/eradiate_core.rst` & `eradiate-0.23.2rc2/docs/rst/reference_api/eradiate_core.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/reference_api/experiments.rst` & `eradiate-0.23.2rc2/docs/rst/reference_api/experiments.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/reference_api/factory.rst` & `eradiate-0.23.2rc2/docs/rst/reference_api/factory.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/reference_api/index.rst` & `eradiate-0.23.2rc2/docs/rst/reference_api/index.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/reference_api/kernel.rst` & `eradiate-0.23.2rc2/docs/rst/reference_api/kernel.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/reference_api/pipelines.rst` & `eradiate-0.23.2rc2/docs/rst/reference_api/pipelines.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/reference_api/scenes.rst` & `eradiate-0.23.2rc2/docs/rst/reference_api/scenes.rst`

 * *Files 1% similar despite different names*

```diff
@@ -182,237 +182,247 @@
 00000b50: 6374 6f72 7960 0a0a 2a2a 5363 656e 6520  ctory`..**Scene 
 00000b60: 656c 656d 656e 7473 2a2a 0a0a 2e2e 2061  elements**.... a
 00000b70: 7574 6f73 756d 6d61 7279 3a3a 0a20 2020  utosummary::.   
 00000b80: 3a74 6f63 7472 6565 3a20 6765 6e65 7261  :toctree: genera
 00000b90: 7465 642f 6175 746f 7375 6d6d 6172 792f  ted/autosummary/
 00000ba0: 0a0a 2020 2042 6173 6963 5375 7266 6163  ..   BasicSurfac
 00000bb0: 650a 2020 2043 656e 7472 616c 5061 7463  e.   CentralPatc
-00000bc0: 6853 7572 6661 6365 0a0a 6060 6572 6164  hSurface..``erad
-00000bd0: 6961 7465 2e73 6365 6e65 732e 6273 6466  iate.scenes.bsdf
-00000be0: 7360 600a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  s``.------------
-00000bf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a2e  -------------...
-00000c00: 2e20 6175 746f 6d6f 6475 6c65 3a3a 2065  . automodule:: e
-00000c10: 7261 6469 6174 652e 7363 656e 6573 2e62  radiate.scenes.b
-00000c20: 7364 6673 0a0a 2e2e 2070 793a 6375 7272  sdfs.... py:curr
-00000c30: 656e 746d 6f64 756c 653a 3a20 6572 6164  entmodule:: erad
-00000c40: 6961 7465 2e73 6365 6e65 732e 6273 6466  iate.scenes.bsdf
-00000c50: 730a 0a2a 2a49 6e74 6572 6661 6365 732a  s..**Interfaces*
-00000c60: 2a0a 0a2e 2e20 6175 746f 7375 6d6d 6172  *.... autosummar
-00000c70: 793a 3a0a 2020 203a 746f 6374 7265 653a  y::.   :toctree:
-00000c80: 2067 656e 6572 6174 6564 2f61 7574 6f73   generated/autos
-00000c90: 756d 6d61 7279 2f0a 0a20 2020 4253 4446  ummary/..   BSDF
-00000ca0: 0a0a 2a2a 4661 6374 6f72 6965 732a 2a0a  ..**Factories**.
-00000cb0: 0a2a 203a 6461 7461 3a60 6273 6466 5f66  .* :data:`bsdf_f
-00000cc0: 6163 746f 7279 600a 0a2a 2a53 6365 6e65  actory`..**Scene
-00000cd0: 2065 6c65 6d65 6e74 732a 2a0a 0a2e 2e20   elements**.... 
-00000ce0: 6175 746f 7375 6d6d 6172 793a 3a0a 2020  autosummary::.  
-00000cf0: 203a 746f 6374 7265 653a 2067 656e 6572   :toctree: gener
-00000d00: 6174 6564 2f61 7574 6f73 756d 6d61 7279  ated/autosummary
-00000d10: 2f0a 0a20 2020 426c 6163 6b42 5344 460a  /..   BlackBSDF.
-00000d20: 2020 2043 6865 636b 6572 626f 6172 6442     CheckerboardB
-00000d30: 5344 460a 2020 204c 616d 6265 7274 6961  SDF.   Lambertia
-00000d40: 6e42 5344 460a 2020 204d 5144 6966 6675  nBSDF.   MQDiffu
-00000d50: 7365 4253 4446 0a20 2020 5250 5642 5344  seBSDF.   RPVBSD
-00000d60: 460a 0a60 6065 7261 6469 6174 652e 7363  F..``eradiate.sc
-00000d70: 656e 6573 2e73 6861 7065 7360 600a 2d2d  enes.shapes``.--
-00000d80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000d90: 2d2d 2d2d 2d2d 2d2d 0a0a 2e2e 2061 7574  --------.... aut
-00000da0: 6f6d 6f64 756c 653a 3a20 6572 6164 6961  omodule:: eradia
-00000db0: 7465 2e73 6365 6e65 732e 7368 6170 6573  te.scenes.shapes
-00000dc0: 0a0a 2e2e 2070 793a 6375 7272 656e 746d  .... py:currentm
-00000dd0: 6f64 756c 653a 3a20 6572 6164 6961 7465  odule:: eradiate
-00000de0: 2e73 6365 6e65 732e 7368 6170 6573 0a0a  .scenes.shapes..
-00000df0: 2a2a 496e 7465 7266 6163 6573 2a2a 0a0a  **Interfaces**..
-00000e00: 2e2e 2061 7574 6f73 756d 6d61 7279 3a3a  .. autosummary::
-00000e10: 0a20 2020 3a74 6f63 7472 6565 3a20 6765  .   :toctree: ge
-00000e20: 6e65 7261 7465 642f 6175 746f 7375 6d6d  nerated/autosumm
-00000e30: 6172 792f 0a0a 2020 2053 6861 7065 0a20  ary/..   Shape. 
-00000e40: 2020 5368 6170 654e 6f64 650a 2020 2053    ShapeNode.   S
-00000e50: 6861 7065 496e 7374 616e 6365 0a0a 2a2a  hapeInstance..**
-00000e60: 4661 6374 6f72 6965 732a 2a0a 0a2a 203a  Factories**..* :
-00000e70: 6461 7461 3a60 7368 6170 655f 6661 6374  data:`shape_fact
-00000e80: 6f72 7960 0a0a 2a2a 5363 656e 6520 656c  ory`..**Scene el
-00000e90: 656d 656e 7473 2a2a 0a0a 2e2e 2061 7574  ements**.... aut
-00000ea0: 6f73 756d 6d61 7279 3a3a 0a20 2020 3a74  osummary::.   :t
-00000eb0: 6f63 7472 6565 3a20 6765 6e65 7261 7465  octree: generate
-00000ec0: 642f 6175 746f 7375 6d6d 6172 792f 0a0a  d/autosummary/..
-00000ed0: 2020 2043 7562 6f69 6453 6861 7065 0a20     CuboidShape. 
-00000ee0: 2020 5265 6374 616e 676c 6553 6861 7065    RectangleShape
-00000ef0: 0a20 2020 5370 6865 7265 5368 6170 650a  .   SphereShape.
-00000f00: 0a60 6065 7261 6469 6174 652e 7363 656e  .``eradiate.scen
-00000f10: 6573 2e69 6c6c 756d 696e 6174 696f 6e60  es.illumination`
-00000f20: 600a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  `.--------------
-00000f30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000f40: 2d2d 0a0a 2e2e 2061 7574 6f6d 6f64 756c  --.... automodul
-00000f50: 653a 3a20 6572 6164 6961 7465 2e73 6365  e:: eradiate.sce
-00000f60: 6e65 732e 696c 6c75 6d69 6e61 7469 6f6e  nes.illumination
-00000f70: 0a0a 2e2e 2070 793a 6375 7272 656e 746d  .... py:currentm
-00000f80: 6f64 756c 653a 3a20 6572 6164 6961 7465  odule:: eradiate
-00000f90: 2e73 6365 6e65 732e 696c 6c75 6d69 6e61  .scenes.illumina
-00000fa0: 7469 6f6e 0a0a 2a2a 496e 7465 7266 6163  tion..**Interfac
-00000fb0: 6573 2a2a 0a0a 2e2e 2061 7574 6f73 756d  es**.... autosum
-00000fc0: 6d61 7279 3a3a 0a20 2020 3a74 6f63 7472  mary::.   :toctr
-00000fd0: 6565 3a20 6765 6e65 7261 7465 642f 6175  ee: generated/au
-00000fe0: 746f 7375 6d6d 6172 792f 0a0a 2020 2049  tosummary/..   I
-00000ff0: 6c6c 756d 696e 6174 696f 6e0a 0a2a 2a46  llumination..**F
-00001000: 6163 746f 7269 6573 2a2a 0a0a 2a20 3a64  actories**..* :d
-00001010: 6174 613a 6069 6c6c 756d 696e 6174 696f  ata:`illuminatio
-00001020: 6e5f 6661 6374 6f72 7960 0a0a 2a2a 5363  n_factory`..**Sc
-00001030: 656e 6520 656c 656d 656e 7473 2a2a 0a0a  ene elements**..
-00001040: 2e2e 2061 7574 6f73 756d 6d61 7279 3a3a  .. autosummary::
-00001050: 0a20 2020 3a74 6f63 7472 6565 3a20 6765  .   :toctree: ge
-00001060: 6e65 7261 7465 642f 6175 746f 7375 6d6d  nerated/autosumm
-00001070: 6172 792f 0a0a 2020 2044 6972 6563 7469  ary/..   Directi
-00001080: 6f6e 616c 496c 6c75 6d69 6e61 7469 6f6e  onalIllumination
-00001090: 0a20 2020 436f 6e73 7461 6e74 496c 6c75  .   ConstantIllu
-000010a0: 6d69 6e61 7469 6f6e 0a20 2020 5370 6f74  mination.   Spot
-000010b0: 496c 6c75 6d69 6e61 7469 6f6e 0a0a 6060  Illumination..``
-000010c0: 6572 6164 6961 7465 2e73 6365 6e65 732e  eradiate.scenes.
-000010d0: 6d65 6173 7572 6560 600a 2d2d 2d2d 2d2d  measure``.------
-000010e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000010f0: 2d2d 2d2d 2d0a 0a2e 2e20 6175 746f 6d6f  -----.... automo
-00001100: 6475 6c65 3a3a 2065 7261 6469 6174 652e  dule:: eradiate.
-00001110: 7363 656e 6573 2e6d 6561 7375 7265 0a0a  scenes.measure..
-00001120: 2e2e 2070 793a 6375 7272 656e 746d 6f64  .. py:currentmod
-00001130: 756c 653a 3a20 6572 6164 6961 7465 2e73  ule:: eradiate.s
-00001140: 6365 6e65 732e 6d65 6173 7572 650a 0a2a  cenes.measure..*
-00001150: 2a49 6e74 6572 6661 6365 732a 2a0a 0a2e  *Interfaces**...
-00001160: 2e20 6175 746f 7375 6d6d 6172 793a 3a0a  . autosummary::.
-00001170: 2020 203a 746f 6374 7265 653a 2067 656e     :toctree: gen
-00001180: 6572 6174 6564 2f61 7574 6f73 756d 6d61  erated/autosumma
-00001190: 7279 2f0a 0a20 2020 4d65 6173 7572 650a  ry/..   Measure.
-000011a0: 2020 2054 6172 6765 740a 0a2a 2a46 6163     Target..**Fac
-000011b0: 746f 7269 6573 2a2a 0a0a 2a20 3a64 6174  tories**..* :dat
-000011c0: 613a 606d 6561 7375 7265 5f66 6163 746f  a:`measure_facto
-000011d0: 7279 600a 0a2a 2a53 6365 6e65 2065 6c65  ry`..**Scene ele
-000011e0: 6d65 6e74 732a 2a0a 0a2e 2e20 6175 746f  ments**.... auto
-000011f0: 7375 6d6d 6172 793a 3a0a 2020 203a 746f  summary::.   :to
-00001200: 6374 7265 653a 2067 656e 6572 6174 6564  ctree: generated
-00001210: 2f61 7574 6f73 756d 6d61 7279 2f0a 0a20  /autosummary/.. 
-00001220: 2020 4d75 6c74 6944 6973 7461 6e74 4d65    MultiDistantMe
-00001230: 6173 7572 650a 2020 2044 6973 7461 6e74  asure.   Distant
-00001240: 466c 7578 4d65 6173 7572 650a 2020 2048  FluxMeasure.   H
-00001250: 656d 6973 7068 6572 6963 616c 4469 7374  emisphericalDist
-00001260: 616e 744d 6561 7375 7265 0a20 2020 5261  antMeasure.   Ra
-00001270: 6469 616e 6365 6d65 7465 724d 6561 7375  diancemeterMeasu
-00001280: 7265 0a20 2020 4d75 6c74 6952 6164 6961  re.   MultiRadia
-00001290: 6e63 656d 6574 6572 4d65 6173 7572 650a  ncemeterMeasure.
-000012a0: 2020 2050 6572 7370 6563 7469 7665 4361     PerspectiveCa
-000012b0: 6d65 7261 4d65 6173 7572 650a 0a2a 2a44  meraMeasure..**D
-000012c0: 6973 7461 6e74 206d 6561 7375 7265 2074  istant measure t
-000012d0: 6172 6765 7420 6465 6669 6e69 7469 6f6e  arget definition
-000012e0: 2a2a 0a0a 2e2e 2061 7574 6f73 756d 6d61  **.... autosumma
-000012f0: 7279 3a3a 0a20 203a 746f 6374 7265 653a  ry::.  :toctree:
-00001300: 2067 656e 6572 6174 6564 2f61 7574 6f73   generated/autos
-00001310: 756d 6d61 7279 2f0a 0a20 2054 6172 6765  ummary/..  Targe
-00001320: 7450 6f69 6e74 0a20 2054 6172 6765 7452  tPoint.  TargetR
-00001330: 6563 7461 6e67 6c65 0a0a 2a2a 5669 6577  ectangle..**View
-00001340: 696e 6720 6469 7265 6374 696f 6e20 6c61  ing direction la
-00001350: 796f 7574 732a 2a0a 0a2a 5573 6564 2061  youts**..*Used a
-00001360: 7320 696e 7075 7420 746f 2074 6865 2a20  s input to the* 
-00001370: 3a63 6c61 7373 3a60 2e4d 756c 7469 4469  :class:`.MultiDi
-00001380: 7374 616e 744d 6561 7375 7265 605c 2060  stantMeasure`\ `
-00001390: 602e 6c61 796f 7574 6060 202a 6669 656c  `.layout`` *fiel
-000013a0: 642e 2a0a 0a2e 2e20 6175 746f 7375 6d6d  d.*.... autosumm
-000013b0: 6172 793a 3a0a 2020 203a 746f 6374 7265  ary::.   :toctre
-000013c0: 653a 2067 656e 6572 6174 6564 2f61 7574  e: generated/aut
-000013d0: 6f73 756d 6d61 7279 2f0a 0a20 2020 4c61  osummary/..   La
-000013e0: 796f 7574 0a20 2020 416e 676c 654c 6179  yout.   AngleLay
-000013f0: 6f75 740a 2020 2041 7a69 6d75 7468 5269  out.   AzimuthRi
-00001400: 6e67 4c61 796f 7574 0a20 2020 4469 7265  ngLayout.   Dire
-00001410: 6374 696f 6e4c 6179 6f75 740a 2020 2047  ctionLayout.   G
-00001420: 7269 644c 6179 6f75 740a 2020 2048 656d  ridLayout.   Hem
-00001430: 6973 7068 6572 6550 6c61 6e65 4c61 796f  ispherePlaneLayo
-00001440: 7574 0a0a 6060 6572 6164 6961 7465 2e73  ut..``eradiate.s
-00001450: 6365 6e65 732e 7068 6173 6560 600a 2d2d  cenes.phase``.--
-00001460: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001470: 2d2d 2d2d 2d2d 2d0a 0a2e 2e20 6175 746f  -------.... auto
-00001480: 6d6f 6475 6c65 3a3a 2065 7261 6469 6174  module:: eradiat
-00001490: 652e 7363 656e 6573 2e70 6861 7365 0a0a  e.scenes.phase..
-000014a0: 2e2e 2070 793a 6375 7272 656e 746d 6f64  .. py:currentmod
-000014b0: 756c 653a 3a20 6572 6164 6961 7465 2e73  ule:: eradiate.s
-000014c0: 6365 6e65 732e 7068 6173 650a 0a2a 2a49  cenes.phase..**I
-000014d0: 6e74 6572 6661 6365 732a 2a0a 0a2e 2e20  nterfaces**.... 
-000014e0: 6175 746f 7375 6d6d 6172 793a 3a0a 2020  autosummary::.  
-000014f0: 203a 746f 6374 7265 653a 2067 656e 6572   :toctree: gener
-00001500: 6174 6564 2f61 7574 6f73 756d 6d61 7279  ated/autosummary
-00001510: 2f0a 0a20 2020 5068 6173 6546 756e 6374  /..   PhaseFunct
-00001520: 696f 6e0a 0a2a 2a46 6163 746f 7269 6573  ion..**Factories
-00001530: 2a2a 0a0a 2a20 3a64 6174 613a 6070 6861  **..* :data:`pha
-00001540: 7365 5f66 756e 6374 696f 6e5f 6661 6374  se_function_fact
-00001550: 6f72 7960 0a0a 2a2a 5363 656e 6520 656c  ory`..**Scene el
-00001560: 656d 656e 7473 2a2a 0a0a 2e2e 2061 7574  ements**.... aut
-00001570: 6f73 756d 6d61 7279 3a3a 0a20 2020 3a74  osummary::.   :t
-00001580: 6f63 7472 6565 3a20 6765 6e65 7261 7465  octree: generate
-00001590: 642f 6175 746f 7375 6d6d 6172 792f 0a0a  d/autosummary/..
-000015a0: 2020 2049 736f 7472 6f70 6963 5068 6173     IsotropicPhas
-000015b0: 6546 756e 6374 696f 6e0a 2020 2052 6179  eFunction.   Ray
-000015c0: 6c65 6967 6850 6861 7365 4675 6e63 7469  leighPhaseFuncti
-000015d0: 6f6e 0a20 2020 4865 6e79 6579 4772 6565  on.   HenyeyGree
-000015e0: 6e73 7465 696e 5068 6173 6546 756e 6374  nsteinPhaseFunct
-000015f0: 696f 6e0a 2020 2042 6c65 6e64 5068 6173  ion.   BlendPhas
-00001600: 6546 756e 6374 696f 6e0a 2020 2054 6162  eFunction.   Tab
-00001610: 756c 6174 6564 5068 6173 6546 756e 6374  ulatedPhaseFunct
-00001620: 696f 6e0a 0a60 6065 7261 6469 6174 652e  ion..``eradiate.
-00001630: 7363 656e 6573 2e69 6e74 6567 7261 746f  scenes.integrato
-00001640: 7273 6060 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  rs``.-----------
-00001650: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001660: 2d2d 2d2d 0a0a 2e2e 2061 7574 6f6d 6f64  ----.... automod
-00001670: 756c 653a 3a20 6572 6164 6961 7465 2e73  ule:: eradiate.s
-00001680: 6365 6e65 732e 696e 7465 6772 6174 6f72  cenes.integrator
-00001690: 730a 0a2e 2e20 7079 3a63 7572 7265 6e74  s.... py:current
-000016a0: 6d6f 6475 6c65 3a3a 2065 7261 6469 6174  module:: eradiat
-000016b0: 652e 7363 656e 6573 2e69 6e74 6567 7261  e.scenes.integra
-000016c0: 746f 7273 0a0a 2a2a 496e 7465 7266 6163  tors..**Interfac
-000016d0: 6573 2a2a 0a0a 2e2e 2061 7574 6f73 756d  es**.... autosum
-000016e0: 6d61 7279 3a3a 0a20 2020 3a74 6f63 7472  mary::.   :toctr
-000016f0: 6565 3a20 6765 6e65 7261 7465 642f 6175  ee: generated/au
-00001700: 746f 7375 6d6d 6172 792f 0a0a 2020 2049  tosummary/..   I
-00001710: 6e74 6567 7261 746f 720a 0a2a 2a46 6163  ntegrator..**Fac
-00001720: 746f 7269 6573 2a2a 0a0a 2a20 3a64 6174  tories**..* :dat
-00001730: 613a 6069 6e74 6567 7261 746f 725f 6661  a:`integrator_fa
-00001740: 6374 6f72 7960 0a0a 2a2a 5363 656e 6520  ctory`..**Scene 
-00001750: 656c 656d 656e 7473 2a2a 0a0a 2e2e 2061  elements**.... a
-00001760: 7574 6f73 756d 6d61 7279 3a3a 0a20 2020  utosummary::.   
-00001770: 3a74 6f63 7472 6565 3a20 6765 6e65 7261  :toctree: genera
-00001780: 7465 642f 6175 746f 7375 6d6d 6172 792f  ted/autosummary/
-00001790: 0a0a 2020 2050 6174 6849 6e74 6567 7261  ..   PathIntegra
-000017a0: 746f 720a 2020 2056 6f6c 5061 7468 496e  tor.   VolPathIn
-000017b0: 7465 6772 6174 6f72 0a20 2020 566f 6c50  tegrator.   VolP
-000017c0: 6174 684d 4953 496e 7465 6772 6174 6f72  athMISIntegrator
-000017d0: 0a0a 6060 6572 6164 6961 7465 2e73 6365  ..``eradiate.sce
-000017e0: 6e65 732e 7370 6563 7472 6160 600a 2d2d  nes.spectra``.--
-000017f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001800: 2d2d 2d2d 2d2d 2d2d 2d0a 0a2e 2e20 6175  ---------.... au
-00001810: 746f 6d6f 6475 6c65 3a3a 2065 7261 6469  tomodule:: eradi
-00001820: 6174 652e 7363 656e 6573 2e73 7065 6374  ate.scenes.spect
-00001830: 7261 0a0a 2e2e 2070 793a 6375 7272 656e  ra.... py:curren
-00001840: 746d 6f64 756c 653a 3a20 6572 6164 6961  tmodule:: eradia
-00001850: 7465 2e73 6365 6e65 732e 7370 6563 7472  te.scenes.spectr
-00001860: 610a 0a2a 2a49 6e74 6572 6661 6365 732a  a..**Interfaces*
-00001870: 2a0a 0a2e 2e20 6175 746f 7375 6d6d 6172  *.... autosummar
-00001880: 793a 3a0a 2020 203a 746f 6374 7265 653a  y::.   :toctree:
-00001890: 2067 656e 6572 6174 6564 2f61 7574 6f73   generated/autos
-000018a0: 756d 6d61 7279 2f0a 0a20 2020 5370 6563  ummary/..   Spec
-000018b0: 7472 756d 0a0a 2a2a 4661 6374 6f72 6965  trum..**Factorie
-000018c0: 732a 2a0a 0a2a 203a 6461 7461 3a60 7370  s**..* :data:`sp
-000018d0: 6563 7472 756d 5f66 6163 746f 7279 600a  ectrum_factory`.
-000018e0: 0a2e 2e20 6472 6f70 646f 776e 3a3a 2050  ... dropdown:: P
-000018f0: 7269 7661 7465 0a0a 2020 202e 2e20 6175  rivate..   .. au
-00001900: 746f 7375 6d6d 6172 793a 3a0a 2020 2020  tosummary::.    
-00001910: 2020 3a74 6f63 7472 6565 3a20 6765 6e65    :toctree: gene
-00001920: 7261 7465 642f 6175 746f 7375 6d6d 6172  rated/autosummar
-00001930: 792f 0a0a 2020 2020 2020 5f63 6f72 652e  y/..      _core.
-00001940: 5370 6563 7472 756d 4661 6374 6f72 790a  SpectrumFactory.
-00001950: 0a2a 2a53 6365 6e65 2065 6c65 6d65 6e74  .**Scene element
-00001960: 732a 2a0a 0a2e 2e20 6175 746f 7375 6d6d  s**.... autosumm
-00001970: 6172 793a 3a0a 2020 203a 746f 6374 7265  ary::.   :toctre
-00001980: 653a 2067 656e 6572 6174 6564 2f61 7574  e: generated/aut
-00001990: 6f73 756d 6d61 7279 2f0a 0a20 2020 556e  osummary/..   Un
-000019a0: 6966 6f72 6d53 7065 6374 7275 6d0a 2020  iformSpectrum.  
-000019b0: 2049 6e74 6572 706f 6c61 7465 6453 7065   InterpolatedSpe
-000019c0: 6374 7275 6d0a 2020 204d 756c 7469 4465  ctrum.   MultiDe
-000019d0: 6c74 6153 7065 6374 7275 6d0a 2020 2053  ltaSpectrum.   S
-000019e0: 6f6c 6172 4972 7261 6469 616e 6365 5370  olarIrradianceSp
-000019f0: 6563 7472 756d 0a20 2020 4169 7253 6361  ectrum.   AirSca
-00001a00: 7474 6572 696e 6743 6f65 6666 6963 6965  tteringCoefficie
-00001a10: 6e74 5370 6563 7472 756d 0a              ntSpectrum.
+00000bc0: 6853 7572 6661 6365 0a20 2020 4445 4d53  hSurface.   DEMS
+00000bd0: 7572 6661 6365 0a0a 2a2a 4865 6c70 6572  urface..**Helper
+00000be0: 732a 2a0a 0a2e 2e20 6175 746f 7375 6d6d  s**.... autosumm
+00000bf0: 6172 793a 3a0a 2020 203a 746f 6374 7265  ary::.   :toctre
+00000c00: 653a 2067 656e 6572 6174 6564 2f61 7574  e: generated/aut
+00000c10: 6f73 756d 6d61 7279 2f0a 0a20 2020 6d65  osummary/..   me
+00000c20: 7368 5f66 726f 6d5f 6465 6d0a 0a60 6065  sh_from_dem..``e
+00000c30: 7261 6469 6174 652e 7363 656e 6573 2e62  radiate.scenes.b
+00000c40: 7364 6673 6060 0a2d 2d2d 2d2d 2d2d 2d2d  sdfs``.---------
+00000c50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000c60: 0a0a 2e2e 2061 7574 6f6d 6f64 756c 653a  .... automodule:
+00000c70: 3a20 6572 6164 6961 7465 2e73 6365 6e65  : eradiate.scene
+00000c80: 732e 6273 6466 730a 0a2e 2e20 7079 3a63  s.bsdfs.... py:c
+00000c90: 7572 7265 6e74 6d6f 6475 6c65 3a3a 2065  urrentmodule:: e
+00000ca0: 7261 6469 6174 652e 7363 656e 6573 2e62  radiate.scenes.b
+00000cb0: 7364 6673 0a0a 2a2a 496e 7465 7266 6163  sdfs..**Interfac
+00000cc0: 6573 2a2a 0a0a 2e2e 2061 7574 6f73 756d  es**.... autosum
+00000cd0: 6d61 7279 3a3a 0a20 2020 3a74 6f63 7472  mary::.   :toctr
+00000ce0: 6565 3a20 6765 6e65 7261 7465 642f 6175  ee: generated/au
+00000cf0: 746f 7375 6d6d 6172 792f 0a0a 2020 2042  tosummary/..   B
+00000d00: 5344 460a 0a2a 2a46 6163 746f 7269 6573  SDF..**Factories
+00000d10: 2a2a 0a0a 2a20 3a64 6174 613a 6062 7364  **..* :data:`bsd
+00000d20: 665f 6661 6374 6f72 7960 0a0a 2a2a 5363  f_factory`..**Sc
+00000d30: 656e 6520 656c 656d 656e 7473 2a2a 0a0a  ene elements**..
+00000d40: 2e2e 2061 7574 6f73 756d 6d61 7279 3a3a  .. autosummary::
+00000d50: 0a20 2020 3a74 6f63 7472 6565 3a20 6765  .   :toctree: ge
+00000d60: 6e65 7261 7465 642f 6175 746f 7375 6d6d  nerated/autosumm
+00000d70: 6172 792f 0a0a 2020 2042 6c61 636b 4253  ary/..   BlackBS
+00000d80: 4446 0a20 2020 4368 6563 6b65 7262 6f61  DF.   Checkerboa
+00000d90: 7264 4253 4446 0a20 2020 4c61 6d62 6572  rdBSDF.   Lamber
+00000da0: 7469 616e 4253 4446 0a20 2020 4d51 4469  tianBSDF.   MQDi
+00000db0: 6666 7573 6542 5344 460a 2020 204f 7061  ffuseBSDF.   Opa
+00000dc0: 6369 7479 4d61 736b 4253 4446 0a20 2020  cityMaskBSDF.   
+00000dd0: 5250 5642 5344 460a 0a60 6065 7261 6469  RPVBSDF..``eradi
+00000de0: 6174 652e 7363 656e 6573 2e73 6861 7065  ate.scenes.shape
+00000df0: 7360 600a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  s``.------------
+00000e00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  --------------..
+00000e10: 2e2e 2061 7574 6f6d 6f64 756c 653a 3a20  .. automodule:: 
+00000e20: 6572 6164 6961 7465 2e73 6365 6e65 732e  eradiate.scenes.
+00000e30: 7368 6170 6573 0a0a 2e2e 2070 793a 6375  shapes.... py:cu
+00000e40: 7272 656e 746d 6f64 756c 653a 3a20 6572  rrentmodule:: er
+00000e50: 6164 6961 7465 2e73 6365 6e65 732e 7368  adiate.scenes.sh
+00000e60: 6170 6573 0a0a 2a2a 496e 7465 7266 6163  apes..**Interfac
+00000e70: 6573 2a2a 0a0a 2e2e 2061 7574 6f73 756d  es**.... autosum
+00000e80: 6d61 7279 3a3a 0a20 2020 3a74 6f63 7472  mary::.   :toctr
+00000e90: 6565 3a20 6765 6e65 7261 7465 642f 6175  ee: generated/au
+00000ea0: 746f 7375 6d6d 6172 792f 0a0a 2020 2053  tosummary/..   S
+00000eb0: 6861 7065 0a20 2020 5368 6170 654e 6f64  hape.   ShapeNod
+00000ec0: 650a 2020 2053 6861 7065 496e 7374 616e  e.   ShapeInstan
+00000ed0: 6365 0a0a 2a2a 4661 6374 6f72 6965 732a  ce..**Factories*
+00000ee0: 2a0a 0a2a 203a 6461 7461 3a60 7368 6170  *..* :data:`shap
+00000ef0: 655f 6661 6374 6f72 7960 0a0a 2a2a 5363  e_factory`..**Sc
+00000f00: 656e 6520 656c 656d 656e 7473 2a2a 0a0a  ene elements**..
+00000f10: 2e2e 2061 7574 6f73 756d 6d61 7279 3a3a  .. autosummary::
+00000f20: 0a20 2020 3a74 6f63 7472 6565 3a20 6765  .   :toctree: ge
+00000f30: 6e65 7261 7465 642f 6175 746f 7375 6d6d  nerated/autosumm
+00000f40: 6172 792f 0a0a 2020 2042 7566 6665 724d  ary/..   BufferM
+00000f50: 6573 6853 6861 7065 0a20 2020 4375 626f  eshShape.   Cubo
+00000f60: 6964 5368 6170 650a 2020 2046 696c 654d  idShape.   FileM
+00000f70: 6573 6853 6861 7065 0a20 2020 5265 6374  eshShape.   Rect
+00000f80: 616e 676c 6553 6861 7065 0a20 2020 5370  angleShape.   Sp
+00000f90: 6865 7265 5368 6170 650a 0a60 6065 7261  hereShape..``era
+00000fa0: 6469 6174 652e 7363 656e 6573 2e69 6c6c  diate.scenes.ill
+00000fb0: 756d 696e 6174 696f 6e60 600a 2d2d 2d2d  umination``.----
+00000fc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000fd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 2e2e  ------------....
+00000fe0: 2061 7574 6f6d 6f64 756c 653a 3a20 6572   automodule:: er
+00000ff0: 6164 6961 7465 2e73 6365 6e65 732e 696c  adiate.scenes.il
+00001000: 6c75 6d69 6e61 7469 6f6e 0a0a 2e2e 2070  lumination.... p
+00001010: 793a 6375 7272 656e 746d 6f64 756c 653a  y:currentmodule:
+00001020: 3a20 6572 6164 6961 7465 2e73 6365 6e65  : eradiate.scene
+00001030: 732e 696c 6c75 6d69 6e61 7469 6f6e 0a0a  s.illumination..
+00001040: 2a2a 496e 7465 7266 6163 6573 2a2a 0a0a  **Interfaces**..
+00001050: 2e2e 2061 7574 6f73 756d 6d61 7279 3a3a  .. autosummary::
+00001060: 0a20 2020 3a74 6f63 7472 6565 3a20 6765  .   :toctree: ge
+00001070: 6e65 7261 7465 642f 6175 746f 7375 6d6d  nerated/autosumm
+00001080: 6172 792f 0a0a 2020 2049 6c6c 756d 696e  ary/..   Illumin
+00001090: 6174 696f 6e0a 0a2a 2a46 6163 746f 7269  ation..**Factori
+000010a0: 6573 2a2a 0a0a 2a20 3a64 6174 613a 6069  es**..* :data:`i
+000010b0: 6c6c 756d 696e 6174 696f 6e5f 6661 6374  llumination_fact
+000010c0: 6f72 7960 0a0a 2a2a 5363 656e 6520 656c  ory`..**Scene el
+000010d0: 656d 656e 7473 2a2a 0a0a 2e2e 2061 7574  ements**.... aut
+000010e0: 6f73 756d 6d61 7279 3a3a 0a20 2020 3a74  osummary::.   :t
+000010f0: 6f63 7472 6565 3a20 6765 6e65 7261 7465  octree: generate
+00001100: 642f 6175 746f 7375 6d6d 6172 792f 0a0a  d/autosummary/..
+00001110: 2020 2044 6972 6563 7469 6f6e 616c 496c     DirectionalIl
+00001120: 6c75 6d69 6e61 7469 6f6e 0a20 2020 436f  lumination.   Co
+00001130: 6e73 7461 6e74 496c 6c75 6d69 6e61 7469  nstantIlluminati
+00001140: 6f6e 0a20 2020 5370 6f74 496c 6c75 6d69  on.   SpotIllumi
+00001150: 6e61 7469 6f6e 0a0a 6060 6572 6164 6961  nation..``eradia
+00001160: 7465 2e73 6365 6e65 732e 6d65 6173 7572  te.scenes.measur
+00001170: 6560 600a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  e``.------------
+00001180: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
+00001190: 0a2e 2e20 6175 746f 6d6f 6475 6c65 3a3a  ... automodule::
+000011a0: 2065 7261 6469 6174 652e 7363 656e 6573   eradiate.scenes
+000011b0: 2e6d 6561 7375 7265 0a0a 2e2e 2070 793a  .measure.... py:
+000011c0: 6375 7272 656e 746d 6f64 756c 653a 3a20  currentmodule:: 
+000011d0: 6572 6164 6961 7465 2e73 6365 6e65 732e  eradiate.scenes.
+000011e0: 6d65 6173 7572 650a 0a2a 2a49 6e74 6572  measure..**Inter
+000011f0: 6661 6365 732a 2a0a 0a2e 2e20 6175 746f  faces**.... auto
+00001200: 7375 6d6d 6172 793a 3a0a 2020 203a 746f  summary::.   :to
+00001210: 6374 7265 653a 2067 656e 6572 6174 6564  ctree: generated
+00001220: 2f61 7574 6f73 756d 6d61 7279 2f0a 0a20  /autosummary/.. 
+00001230: 2020 4d65 6173 7572 650a 2020 2054 6172    Measure.   Tar
+00001240: 6765 740a 0a2a 2a46 6163 746f 7269 6573  get..**Factories
+00001250: 2a2a 0a0a 2a20 3a64 6174 613a 606d 6561  **..* :data:`mea
+00001260: 7375 7265 5f66 6163 746f 7279 600a 0a2a  sure_factory`..*
+00001270: 2a53 6365 6e65 2065 6c65 6d65 6e74 732a  *Scene elements*
+00001280: 2a0a 0a2e 2e20 6175 746f 7375 6d6d 6172  *.... autosummar
+00001290: 793a 3a0a 2020 203a 746f 6374 7265 653a  y::.   :toctree:
+000012a0: 2067 656e 6572 6174 6564 2f61 7574 6f73   generated/autos
+000012b0: 756d 6d61 7279 2f0a 0a20 2020 4d75 6c74  ummary/..   Mult
+000012c0: 6944 6973 7461 6e74 4d65 6173 7572 650a  iDistantMeasure.
+000012d0: 2020 2044 6973 7461 6e74 466c 7578 4d65     DistantFluxMe
+000012e0: 6173 7572 650a 2020 2048 656d 6973 7068  asure.   Hemisph
+000012f0: 6572 6963 616c 4469 7374 616e 744d 6561  ericalDistantMea
+00001300: 7375 7265 0a20 2020 5261 6469 616e 6365  sure.   Radiance
+00001310: 6d65 7465 724d 6561 7375 7265 0a20 2020  meterMeasure.   
+00001320: 4d75 6c74 6952 6164 6961 6e63 656d 6574  MultiRadiancemet
+00001330: 6572 4d65 6173 7572 650a 2020 2050 6572  erMeasure.   Per
+00001340: 7370 6563 7469 7665 4361 6d65 7261 4d65  spectiveCameraMe
+00001350: 6173 7572 650a 0a2a 2a44 6973 7461 6e74  asure..**Distant
+00001360: 206d 6561 7375 7265 2074 6172 6765 7420   measure target 
+00001370: 6465 6669 6e69 7469 6f6e 2a2a 0a0a 2e2e  definition**....
+00001380: 2061 7574 6f73 756d 6d61 7279 3a3a 0a20   autosummary::. 
+00001390: 203a 746f 6374 7265 653a 2067 656e 6572   :toctree: gener
+000013a0: 6174 6564 2f61 7574 6f73 756d 6d61 7279  ated/autosummary
+000013b0: 2f0a 0a20 2054 6172 6765 7450 6f69 6e74  /..  TargetPoint
+000013c0: 0a20 2054 6172 6765 7452 6563 7461 6e67  .  TargetRectang
+000013d0: 6c65 0a0a 2a2a 5669 6577 696e 6720 6469  le..**Viewing di
+000013e0: 7265 6374 696f 6e20 6c61 796f 7574 732a  rection layouts*
+000013f0: 2a0a 0a2a 5573 6564 2061 7320 696e 7075  *..*Used as inpu
+00001400: 7420 746f 2074 6865 2a20 3a63 6c61 7373  t to the* :class
+00001410: 3a60 2e4d 756c 7469 4469 7374 616e 744d  :`.MultiDistantM
+00001420: 6561 7375 7265 605c 2060 602e 6c61 796f  easure`\ ``.layo
+00001430: 7574 6060 202a 6669 656c 642e 2a0a 0a2e  ut`` *field.*...
+00001440: 2e20 6175 746f 7375 6d6d 6172 793a 3a0a  . autosummary::.
+00001450: 2020 203a 746f 6374 7265 653a 2067 656e     :toctree: gen
+00001460: 6572 6174 6564 2f61 7574 6f73 756d 6d61  erated/autosumma
+00001470: 7279 2f0a 0a20 2020 4c61 796f 7574 0a20  ry/..   Layout. 
+00001480: 2020 416e 676c 654c 6179 6f75 740a 2020    AngleLayout.  
+00001490: 2041 7a69 6d75 7468 5269 6e67 4c61 796f   AzimuthRingLayo
+000014a0: 7574 0a20 2020 4469 7265 6374 696f 6e4c  ut.   DirectionL
+000014b0: 6179 6f75 740a 2020 2047 7269 644c 6179  ayout.   GridLay
+000014c0: 6f75 740a 2020 2048 656d 6973 7068 6572  out.   Hemispher
+000014d0: 6550 6c61 6e65 4c61 796f 7574 0a0a 6060  ePlaneLayout..``
+000014e0: 6572 6164 6961 7465 2e73 6365 6e65 732e  eradiate.scenes.
+000014f0: 7068 6173 6560 600a 2d2d 2d2d 2d2d 2d2d  phase``.--------
+00001500: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001510: 2d0a 0a2e 2e20 6175 746f 6d6f 6475 6c65  -.... automodule
+00001520: 3a3a 2065 7261 6469 6174 652e 7363 656e  :: eradiate.scen
+00001530: 6573 2e70 6861 7365 0a0a 2e2e 2070 793a  es.phase.... py:
+00001540: 6375 7272 656e 746d 6f64 756c 653a 3a20  currentmodule:: 
+00001550: 6572 6164 6961 7465 2e73 6365 6e65 732e  eradiate.scenes.
+00001560: 7068 6173 650a 0a2a 2a49 6e74 6572 6661  phase..**Interfa
+00001570: 6365 732a 2a0a 0a2e 2e20 6175 746f 7375  ces**.... autosu
+00001580: 6d6d 6172 793a 3a0a 2020 203a 746f 6374  mmary::.   :toct
+00001590: 7265 653a 2067 656e 6572 6174 6564 2f61  ree: generated/a
+000015a0: 7574 6f73 756d 6d61 7279 2f0a 0a20 2020  utosummary/..   
+000015b0: 5068 6173 6546 756e 6374 696f 6e0a 0a2a  PhaseFunction..*
+000015c0: 2a46 6163 746f 7269 6573 2a2a 0a0a 2a20  *Factories**..* 
+000015d0: 3a64 6174 613a 6070 6861 7365 5f66 756e  :data:`phase_fun
+000015e0: 6374 696f 6e5f 6661 6374 6f72 7960 0a0a  ction_factory`..
+000015f0: 2a2a 5363 656e 6520 656c 656d 656e 7473  **Scene elements
+00001600: 2a2a 0a0a 2e2e 2061 7574 6f73 756d 6d61  **.... autosumma
+00001610: 7279 3a3a 0a20 2020 3a74 6f63 7472 6565  ry::.   :toctree
+00001620: 3a20 6765 6e65 7261 7465 642f 6175 746f  : generated/auto
+00001630: 7375 6d6d 6172 792f 0a0a 2020 2049 736f  summary/..   Iso
+00001640: 7472 6f70 6963 5068 6173 6546 756e 6374  tropicPhaseFunct
+00001650: 696f 6e0a 2020 2052 6179 6c65 6967 6850  ion.   RayleighP
+00001660: 6861 7365 4675 6e63 7469 6f6e 0a20 2020  haseFunction.   
+00001670: 4865 6e79 6579 4772 6565 6e73 7465 696e  HenyeyGreenstein
+00001680: 5068 6173 6546 756e 6374 696f 6e0a 2020  PhaseFunction.  
+00001690: 2042 6c65 6e64 5068 6173 6546 756e 6374   BlendPhaseFunct
+000016a0: 696f 6e0a 2020 2054 6162 756c 6174 6564  ion.   Tabulated
+000016b0: 5068 6173 6546 756e 6374 696f 6e0a 0a60  PhaseFunction..`
+000016c0: 6065 7261 6469 6174 652e 7363 656e 6573  `eradiate.scenes
+000016d0: 2e69 6e74 6567 7261 746f 7273 6060 0a2d  .integrators``.-
+000016e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000016f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  --------------..
+00001700: 2e2e 2061 7574 6f6d 6f64 756c 653a 3a20  .. automodule:: 
+00001710: 6572 6164 6961 7465 2e73 6365 6e65 732e  eradiate.scenes.
+00001720: 696e 7465 6772 6174 6f72 730a 0a2e 2e20  integrators.... 
+00001730: 7079 3a63 7572 7265 6e74 6d6f 6475 6c65  py:currentmodule
+00001740: 3a3a 2065 7261 6469 6174 652e 7363 656e  :: eradiate.scen
+00001750: 6573 2e69 6e74 6567 7261 746f 7273 0a0a  es.integrators..
+00001760: 2a2a 496e 7465 7266 6163 6573 2a2a 0a0a  **Interfaces**..
+00001770: 2e2e 2061 7574 6f73 756d 6d61 7279 3a3a  .. autosummary::
+00001780: 0a20 2020 3a74 6f63 7472 6565 3a20 6765  .   :toctree: ge
+00001790: 6e65 7261 7465 642f 6175 746f 7375 6d6d  nerated/autosumm
+000017a0: 6172 792f 0a0a 2020 2049 6e74 6567 7261  ary/..   Integra
+000017b0: 746f 720a 0a2a 2a46 6163 746f 7269 6573  tor..**Factories
+000017c0: 2a2a 0a0a 2a20 3a64 6174 613a 6069 6e74  **..* :data:`int
+000017d0: 6567 7261 746f 725f 6661 6374 6f72 7960  egrator_factory`
+000017e0: 0a0a 2a2a 5363 656e 6520 656c 656d 656e  ..**Scene elemen
+000017f0: 7473 2a2a 0a0a 2e2e 2061 7574 6f73 756d  ts**.... autosum
+00001800: 6d61 7279 3a3a 0a20 2020 3a74 6f63 7472  mary::.   :toctr
+00001810: 6565 3a20 6765 6e65 7261 7465 642f 6175  ee: generated/au
+00001820: 746f 7375 6d6d 6172 792f 0a0a 2020 2050  tosummary/..   P
+00001830: 6174 6849 6e74 6567 7261 746f 720a 2020  athIntegrator.  
+00001840: 2056 6f6c 5061 7468 496e 7465 6772 6174   VolPathIntegrat
+00001850: 6f72 0a20 2020 566f 6c50 6174 684d 4953  or.   VolPathMIS
+00001860: 496e 7465 6772 6174 6f72 0a0a 6060 6572  Integrator..``er
+00001870: 6164 6961 7465 2e73 6365 6e65 732e 7370  adiate.scenes.sp
+00001880: 6563 7472 6160 600a 2d2d 2d2d 2d2d 2d2d  ectra``.--------
+00001890: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000018a0: 2d2d 2d0a 0a2e 2e20 6175 746f 6d6f 6475  ---.... automodu
+000018b0: 6c65 3a3a 2065 7261 6469 6174 652e 7363  le:: eradiate.sc
+000018c0: 656e 6573 2e73 7065 6374 7261 0a0a 2e2e  enes.spectra....
+000018d0: 2070 793a 6375 7272 656e 746d 6f64 756c   py:currentmodul
+000018e0: 653a 3a20 6572 6164 6961 7465 2e73 6365  e:: eradiate.sce
+000018f0: 6e65 732e 7370 6563 7472 610a 0a2a 2a49  nes.spectra..**I
+00001900: 6e74 6572 6661 6365 732a 2a0a 0a2e 2e20  nterfaces**.... 
+00001910: 6175 746f 7375 6d6d 6172 793a 3a0a 2020  autosummary::.  
+00001920: 203a 746f 6374 7265 653a 2067 656e 6572   :toctree: gener
+00001930: 6174 6564 2f61 7574 6f73 756d 6d61 7279  ated/autosummary
+00001940: 2f0a 0a20 2020 5370 6563 7472 756d 0a0a  /..   Spectrum..
+00001950: 2a2a 4661 6374 6f72 6965 732a 2a0a 0a2a  **Factories**..*
+00001960: 203a 6461 7461 3a60 7370 6563 7472 756d   :data:`spectrum
+00001970: 5f66 6163 746f 7279 600a 0a2e 2e20 6472  _factory`.... dr
+00001980: 6f70 646f 776e 3a3a 2050 7269 7661 7465  opdown:: Private
+00001990: 0a0a 2020 202e 2e20 6175 746f 7375 6d6d  ..   .. autosumm
+000019a0: 6172 793a 3a0a 2020 2020 2020 3a74 6f63  ary::.      :toc
+000019b0: 7472 6565 3a20 6765 6e65 7261 7465 642f  tree: generated/
+000019c0: 6175 746f 7375 6d6d 6172 792f 0a0a 2020  autosummary/..  
+000019d0: 2020 2020 5f63 6f72 652e 5370 6563 7472      _core.Spectr
+000019e0: 756d 4661 6374 6f72 790a 0a2a 2a53 6365  umFactory..**Sce
+000019f0: 6e65 2065 6c65 6d65 6e74 732a 2a0a 0a2e  ne elements**...
+00001a00: 2e20 6175 746f 7375 6d6d 6172 793a 3a0a  . autosummary::.
+00001a10: 2020 203a 746f 6374 7265 653a 2067 656e     :toctree: gen
+00001a20: 6572 6174 6564 2f61 7574 6f73 756d 6d61  erated/autosumma
+00001a30: 7279 2f0a 0a20 2020 556e 6966 6f72 6d53  ry/..   UniformS
+00001a40: 7065 6374 7275 6d0a 2020 2049 6e74 6572  pectrum.   Inter
+00001a50: 706f 6c61 7465 6453 7065 6374 7275 6d0a  polatedSpectrum.
+00001a60: 2020 204d 756c 7469 4465 6c74 6153 7065     MultiDeltaSpe
+00001a70: 6374 7275 6d0a 2020 2053 6f6c 6172 4972  ctrum.   SolarIr
+00001a80: 7261 6469 616e 6365 5370 6563 7472 756d  radianceSpectrum
+00001a90: 0a20 2020 4169 7253 6361 7474 6572 696e  .   AirScatterin
+00001aa0: 6743 6f65 6666 6963 6965 6e74 5370 6563  gCoefficientSpec
+00001ab0: 7472 756d 0a                             trum.
```

### Comparing `eradiate-0.23.2rc1/docs/rst/reference_api/srf_tools.rst` & `eradiate-0.23.2rc2/docs/rst/reference_api/srf_tools.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/reference_api/test_tools.rst` & `eradiate-0.23.2rc2/docs/rst/reference_api/test_tools.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/reference_api/xarray.rst` & `eradiate-0.23.2rc2/docs/rst/reference_api/xarray.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/absorption.rst` & `eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/absorption.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/fig/bad_resolution.png` & `eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/fig/bad_resolution.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/fig/good_resolution.png` & `eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/fig/good_resolution.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/fig/line.png` & `eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/fig/line.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/heterogeneous.rst` & `eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/heterogeneous.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/intro.rst` & `eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/intro.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/molecular.rst` & `eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/molecular.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/rayleigh_scattering.rst` & `eradiate-0.23.2rc2/docs/rst/user_guide/atmosphere/rayleigh_scattering.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/user_guide/basic_concepts.rst` & `eradiate-0.23.2rc2/docs/rst/user_guide/basic_concepts.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/user_guide/conventions.rst` & `eradiate-0.23.2rc2/docs/rst/user_guide/conventions.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/user_guide/data/absorption.rst` & `eradiate-0.23.2rc2/docs/rst/user_guide/data/absorption.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/user_guide/data/atmosphere_radprops.rst` & `eradiate-0.23.2rc2/docs/rst/user_guide/data/atmosphere_radprops.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/user_guide/data/atmosphere_thermoprops.rst` & `eradiate-0.23.2rc2/docs/rst/user_guide/data/atmosphere_thermoprops.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/user_guide/data/ckd.rst` & `eradiate-0.23.2rc2/docs/rst/user_guide/data/ckd.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/user_guide/data/fig/p_interp_rerr_histo_65349.png` & `eradiate-0.23.2rc2/docs/rst/user_guide/data/fig/p_interp_rerr_histo_65349.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/user_guide/data/fig/pt_points.png` & `eradiate-0.23.2rc2/docs/rst/user_guide/data/fig/pt_points.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/user_guide/data/fig/w_interp_rerr_histo_101325.png` & `eradiate-0.23.2rc2/docs/rst/user_guide/data/fig/w_interp_rerr_histo_101325.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/user_guide/data/intro.rst` & `eradiate-0.23.2rc2/docs/rst/user_guide/data/intro.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/user_guide/data/particle_radprops.rst` & `eradiate-0.23.2rc2/docs/rst/user_guide/data/particle_radprops.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/user_guide/data/solar_irradiance.rst` & `eradiate-0.23.2rc2/docs/rst/user_guide/data/solar_irradiance.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/user_guide/data/spectra-us76_u86_4.rst` & `eradiate-0.23.2rc2/docs/rst/user_guide/data/spectra-us76_u86_4.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/user_guide/data/srf.rst` & `eradiate-0.23.2rc2/docs/rst/user_guide/data/srf.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/user_guide/onedim_experiment.rst` & `eradiate-0.23.2rc2/docs/rst/user_guide/onedim_experiment.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/user_guide/package_structure.rst` & `eradiate-0.23.2rc2/docs/rst/user_guide/package_structure.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/user_guide/spectral_discretization.rst` & `eradiate-0.23.2rc2/docs/rst/user_guide/spectral_discretization.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/rst/user_guide/unit_guide_user.rst` & `eradiate-0.23.2rc2/docs/rst/user_guide/unit_guide_user.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/docs/src/CHANGELOG.md` & `eradiate-0.23.2rc2/docs/src/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,21 @@
 ### Improvements and fixes
 
 * Added {class}`.MultiDeltaSpectrum` spectrum type ({ghpr}`311`).
 * Exposed several API members in the top-level namespace ({ghpr}`324`).
 * Exposed the ``eradiate.spectral.*`` subpackage members in the
   {mod}`eradiate.spectral` namespace ({ghpr}`324`).
 * Fixed incorrect Mitsuba scene parameter drop and lookup ({ghpr}`329`).
-* Provide an Eradiate Pypi package ({ghpr}`328`)
+* Added spherical-shell geometry support to DEM components
+  {ghpr}`320`.
+* Fixed broken symmetry between {class}`.Spectrum` dictionary and object
+  conversion protocols ({ghpr}`336`).
+* Provide an Eradiate Pypi package ({ghpr}`328`).
+* Implement the Astronomical Object Illumination, its tests and its
+  documentation ({ghpr}`331`).
 
 ### Documentation
 
 * Added a user guide page on spectral discretization.
 
 ### Internal changes
```

### Comparing `eradiate-0.23.2rc1/docs/src/reference_cli.md` & `eradiate-0.23.2rc2/docs/src/reference_cli.md`

 * *Files 7% similar despite different names*

```diff
@@ -51,20 +51,20 @@
 #### `eradiate data fetch`
 
 Fetch files from the Eradiate data store.
 
 **Usage**:
 
 ```console
-$ eradiate data fetch [OPTIONS] [FILES]...
+$ eradiate data fetch [OPTIONS] [FILE_LIST]...
 ```
 
 **Arguments**:
 
-* `[FILES]...`: An arbitrary number of relative paths to files to be retrieved from the data store. If unset, the list of files is read from a YAML file which can be specified by using the ``--from-file`` option and defaults to ``$ERADIATE_SOURCE_DIR/resources/downloads.yml``.
+* `[FILE_LIST]...`: An arbitrary number of relative paths to files to be retrieved from the data store. If unset, the list of files is read from a YAML file which can be specified by using the ``--from-file`` option and defaults to ``$ERADIATE_SOURCE_DIR/data/downloads.yml`` a production environment and ``$ERADIATE_SOURCE_DIR/data/downloads_development.yml`` in a development environment.
 
 **Options**:
 
 * `-f, --from-file TEXT`: Optional path to a file list (YAML format). If this option is set, the FILES argument(s) will be ignored.
 * `--help`: Show this message and exit.
 
 #### `eradiate data info`
```

### Comparing `eradiate-0.23.2rc1/pyproject.toml` & `eradiate-0.23.2rc2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -2,85 +2,25 @@
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=61", "setuptools_scm>=6.2"]
 
 [project]
 authors = [
   {name = "The Eradiate Team"}
 ]
-dependencies = [
-  "aenum",
-  "attrs>=22.2",
-  "click",
-  "dessinemoi>=23.1.0",
-  "environ-config",
-  "lazy_loader>=0.1",
-  "matplotlib>=3.3",
-  "netcdf4",
-  "numpy",
-  "pint",
-  "pinttrs>=23.2.0",
-  "portion",
-  "pooch",
-  "rich",
-  "ruamel.yaml",
-  "scipy",
-  "shellingham!=1.5.1",  # Typer dependency; exclude this version which raises while previous don't
-  "tqdm",
-  "typer>=0.9.0",
-  "xarray>=0.19,!=0.20.*"
-]
+
 description = "A radiative transfer model for the Earth observation community"
-dynamic = ["version"]
+dynamic = ["version", "dependencies", "optional-dependencies"]
 license = {text = "LGPLv3"}
 maintainers = [
   {name = "The Eradiate Team"}
 ]
 name = "eradiate"
 readme = "README.md"
 requires-python = ">=3.8"
 
-[project.optional-dependencies]
-dev = [
-  "conda-lock>=1.4",  # Required by dependency management scripts
-  "pip>=22",  # Required by dependency management scripts
-  "pip-tools>=6.5",  # Required by dependency management scripts
-  "setuptools>=61"  # Required by dependency management scripts
-]
-docs = [
-  "autodocsumm",
-  "myst-parser",
-  "nbsphinx>=0.9.0",
-  "sphinx-book-theme>=1.0",
-  "sphinx",
-  "sphinxcontrib-bibtex>=2.0",
-  "sphinx-autobuild",
-  "sphinx-copybutton",
-  "sphinx-design"
-]
-recommended = [
-  "aabbtree",  # Used by the leaf collision detection feature
-  "astropy",  # Used by the solar irradiance spectrum date-based scaling feature
-  "iapws",  # Used by thermophysical property utilities
-  "ipython",
-  "ipywidgets",
-  "jupyterlab",
-  "python-dateutil",  # Used by the Solar irradiance spectrum date-based scaling feature
-  "seaborn"  # Used to define the Eradiate plotting style
-]
-tests = [
-  "pytest",
-  "pytest-json-report"
-]
-optional = [
-  "eradiate_mitsuba==0.0.1rc10"
-]
-production = [
-  "eradiate_mitsuba==0.0.1rc10"
-]
-
 [project.scripts]
 eradiate = "eradiate.cli:main"
 
 [project.urls]
 changelog = "https://github.com/eradiate/eradiate/CHANGELOG.md"
 documentation = "https://eradiate.readthedocs.io"
 repository = "https://github.com/eradiate/eradiate"
@@ -116,14 +56,20 @@
 
 [tool.ruff.isort]
 relative-imports-order = "closest-to-furthest"
 
 [tool.setuptools]
 include-package-data = true # Required because of package data
 
+[tool.setuptools.dynamic]
+dependencies = {file = ["requirements/pip/dependencies.txt"]}
+
+[tool.setuptools.dynamic.optional-dependencies]
+recommended = {file = ['requirements/pip/recommended.txt']}
+
 [tool.setuptools.package-data]
 # Required by PEP 561
 # https://mypy.readthedocs.io/en/stable/installed_packages.html#creating-pep-561-compatible-packages
 eradiate = ["py.typed", "*.pyi"]
 
 [tool.setuptools.packages.find]
 exclude = ["plugins"]
```

### Comparing `eradiate-0.23.2rc1/requirements/copy_envvars.py` & `eradiate-0.23.2rc2/requirements/copy_envvars.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/requirements/dev.txt` & `eradiate-0.23.2rc2/requirements/pip/dev.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,51 +1,46 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --allow-unsafe --output-file=requirements/dev.txt --resolver=backtracking requirements/dev.in
+#    pip-compile --allow-unsafe --output-file=requirements/pip/dev.txt --resolver=backtracking requirements/pip/dev.in
 #
 aabbtree==2.8.1
-    # via -r requirements/recommended.in
+    # via -r requirements/pip/recommended.in
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
 aenum==3.1.12
-    # via -r requirements/main.in
-aiofiles==22.1.0
-    # via ypy-websocket
-aiosqlite==0.19.0
-    # via ypy-websocket
+    # via -r requirements/pip/main.in
 alabaster==0.7.13
     # via sphinx
-anyio==3.6.2
+anyio==3.7.0
     # via jupyter-server
 appdirs==1.4.4
     # via ensureconda
 argon2-cffi==21.3.0
-    # via
-    #   jupyter-server
-    #   nbclassic
-    #   notebook
+    # via jupyter-server
 argon2-cffi-bindings==21.2.0
     # via argon2-cffi
 arrow==1.2.3
     # via isoduration
 astropy==5.2.2
-    # via -r requirements/recommended.in
+    # via -r requirements/pip/recommended.in
 asttokens==2.2.1
     # via stack-data
+async-lru==2.0.2
+    # via jupyterlab
 attrs==23.1.0
     # via
-    #   -r requirements/main.in
+    #   -r requirements/pip/main.in
     #   dessinemoi
     #   environ-config
     #   jsonschema
     #   pinttrs
 autodocsumm==0.2.11
-    # via -r requirements/docs.in
+    # via -r requirements/pip/docs.in
 babel==2.12.1
     # via
     #   jupyterlab-server
     #   pydata-sphinx-theme
     #   sphinx
 backcall==0.2.0
     # via ipython
@@ -53,137 +48,142 @@
     # via
     #   nbconvert
     #   pydata-sphinx-theme
 bleach==6.0.0
     # via nbconvert
 build==0.10.0
     # via pip-tools
-cachecontrol[filecache]==0.12.11
+cachecontrol[filecache]==0.13.1
     # via conda-lock
 cachy==0.3.0
     # via conda-lock
 certifi==2023.5.7
-    # via requests
+    # via
+    #   netcdf4
+    #   requests
 cffi==1.15.1
     # via
     #   argon2-cffi-bindings
     #   cryptography
 cftime==1.6.2
     # via netcdf4
 charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via
-    #   -r requirements/main.in
+    #   -r requirements/pip/main.in
     #   click-default-group
     #   conda-lock
     #   ensureconda
     #   pip-tools
     #   typer
 click-default-group==1.2.2
     # via conda-lock
 clikit==0.6.2
     # via conda-lock
 colorama==0.4.6
     # via sphinx-autobuild
 comm==0.1.3
     # via ipykernel
-conda-lock==1.4.0
-    # via -r requirements/dev.in
-contourpy==1.0.7
+conda-lock==2.1.0
+    # via -r requirements/pip/dev.in
+contourpy==1.1.0
     # via matplotlib
 crashtest==0.3.1
     # via
     #   clikit
     #   conda-lock
-cryptography==40.0.2
+cryptography==41.0.1
     # via secretstorage
 cycler==0.11.0
     # via matplotlib
 debugpy==1.6.7
     # via ipykernel
 decorator==5.1.1
     # via ipython
 defusedxml==0.7.1
     # via nbconvert
 dessinemoi==23.1.0
-    # via -r requirements/main.in
+    # via -r requirements/pip/main.in
 distlib==0.3.6
     # via virtualenv
 docutils==0.19
     # via
     #   myst-parser
     #   nbsphinx
     #   pybtex-docutils
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinxcontrib-bibtex
 ensureconda==1.4.3
     # via conda-lock
 environ-config==23.2.0
-    # via -r requirements/main.in
+    # via -r requirements/pip/main.in
 exceptiongroup==1.1.1
-    # via pytest
+    # via
+    #   anyio
+    #   pytest
 executing==1.2.0
     # via stack-data
-fastjsonschema==2.16.3
+fastjsonschema==2.17.1
     # via nbformat
-filelock==3.12.0
+filelock==3.12.2
     # via
+    #   cachecontrol
     #   conda-lock
     #   ensureconda
     #   virtualenv
-fonttools==4.39.3
+fonttools==4.40.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
+gitdb==4.0.10
+    # via gitpython
+gitpython==3.1.31
+    # via conda-lock
 html5lib==1.1
     # via conda-lock
 iapws==1.5.3
-    # via -r requirements/recommended.in
+    # via -r requirements/pip/recommended.in
 idna==3.4
     # via
     #   anyio
     #   jsonschema
     #   requests
 imagesize==1.4.1
     # via sphinx
-importlib-metadata==6.6.0
+importlib-metadata==6.7.0
     # via
     #   jupyter-client
-    #   jupyter-ydoc
+    #   jupyter-lsp
+    #   jupyterlab
     #   jupyterlab-server
     #   keyring
     #   nbconvert
     #   sphinx
     #   sphinxcontrib-bibtex
 importlib-resources==5.12.0
     # via
     #   jsonschema
+    #   jupyterlab
     #   keyring
     #   matplotlib
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.23.0
+ipykernel==6.23.2
     # via
     #   ipywidgets
-    #   nbclassic
-    #   notebook
+    #   jupyterlab
 ipython==8.12.2
     # via
-    #   -r requirements/recommended.in
+    #   -r requirements/pip/recommended.in
     #   ipykernel
     #   ipywidgets
-    #   jupyterlab
-ipython-genutils==0.2.0
-    # via
-    #   nbclassic
-    #   notebook
 ipywidgets==8.0.6
-    # via -r requirements/recommended.in
+    # via -r requirements/pip/recommended.in
 isoduration==20.11.0
     # via jsonschema
 jaraco-classes==3.2.3
     # via keyring
 jedi==0.18.2
     # via ipython
 jeepney==0.8.0
@@ -193,162 +193,136 @@
 jinja2==3.1.2
     # via
     #   conda-lock
     #   jupyter-server
     #   jupyterlab
     #   jupyterlab-server
     #   myst-parser
-    #   nbclassic
     #   nbconvert
     #   nbsphinx
-    #   notebook
     #   sphinx
-json5==0.9.11
+json5==0.9.14
     # via jupyterlab-server
-jsonpointer==2.3
+jsonpointer==2.4
     # via jsonschema
 jsonschema[format-nongpl]==4.17.3
     # via
     #   jupyter-events
     #   jupyterlab-server
     #   nbformat
 jupyter-client==8.2.0
     # via
     #   ipykernel
     #   jupyter-server
-    #   nbclassic
     #   nbclient
-    #   notebook
-jupyter-core==5.3.0
+jupyter-core==5.3.1
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   jupyterlab
-    #   nbclassic
     #   nbclient
     #   nbconvert
     #   nbformat
-    #   notebook
 jupyter-events==0.6.3
+    # via jupyter-server
+jupyter-lsp==2.2.0
+    # via jupyterlab
+jupyter-server==2.6.0
     # via
-    #   jupyter-server
-    #   jupyter-server-fileid
-jupyter-server==2.5.0
-    # via
-    #   jupyter-server-fileid
+    #   jupyter-lsp
     #   jupyterlab
     #   jupyterlab-server
-    #   nbclassic
     #   notebook-shim
-jupyter-server-fileid==0.9.0
-    # via jupyter-server-ydoc
 jupyter-server-terminals==0.4.4
     # via jupyter-server
-jupyter-server-ydoc==0.8.0
-    # via jupyterlab
-jupyter-ydoc==0.2.4
-    # via
-    #   jupyter-server-ydoc
-    #   jupyterlab
-jupyterlab==3.6.3
-    # via -r requirements/recommended.in
+jupyterlab==4.0.2
+    # via -r requirements/pip/recommended.in
 jupyterlab-pygments==0.2.2
     # via nbconvert
-jupyterlab-server==2.22.1
+jupyterlab-server==2.23.0
     # via jupyterlab
 jupyterlab-widgets==3.0.7
     # via ipywidgets
-keyring==23.13.1
+keyring==24.0.0
     # via conda-lock
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 lazy-loader==0.2
-    # via -r requirements/main.in
+    # via -r requirements/pip/main.in
 livereload==2.6.3
     # via sphinx-autobuild
-lockfile==0.12.2
-    # via cachecontrol
-markdown-it-py==2.2.0
+markdown-it-py==3.0.0
     # via
     #   mdit-py-plugins
     #   myst-parser
     #   rich
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   jinja2
     #   nbconvert
 matplotlib==3.7.1
     # via
-    #   -r requirements/main.in
+    #   -r requirements/pip/main.in
     #   seaborn
 matplotlib-inline==0.1.6
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.3.5
+mdit-py-plugins==0.4.0
     # via myst-parser
 mdurl==0.1.2
     # via markdown-it-py
-mistune==2.0.5
+mistune==3.0.1
     # via nbconvert
 more-itertools==9.1.0
     # via jaraco-classes
 msgpack==1.0.5
     # via cachecontrol
-myst-parser==1.0.0
-    # via -r requirements/docs.in
-nbclassic==1.0.0
-    # via
-    #   jupyterlab
-    #   notebook
-nbclient==0.7.4
+myst-parser==2.0.0
+    # via -r requirements/pip/docs.in
+nbclient==0.8.0
     # via nbconvert
-nbconvert==7.4.0
+nbconvert==7.6.0
     # via
     #   jupyter-server
-    #   nbclassic
     #   nbsphinx
-    #   notebook
-nbformat==5.8.0
+nbformat==5.9.0
     # via
     #   jupyter-server
-    #   nbclassic
     #   nbclient
     #   nbconvert
     #   nbsphinx
-    #   notebook
-nbsphinx==0.9.1
-    # via -r requirements/docs.in
+nbsphinx==0.9.2
+    # via -r requirements/pip/docs.in
 nest-asyncio==1.5.6
-    # via
-    #   ipykernel
-    #   nbclassic
-    #   notebook
-netcdf4==1.6.3
-    # via -r requirements/main.in
-notebook==6.5.4
-    # via jupyterlab
+    # via ipykernel
+netcdf4==1.6.4
+    # via -r requirements/pip/main.in
+networkx==3.1
+    # via -r requirements/pip/dev.in
 notebook-shim==0.2.3
-    # via nbclassic
+    # via jupyterlab
 numpy==1.24.3
     # via
-    #   -r requirements/main.in
+    #   -r requirements/pip/main.in
     #   astropy
     #   cftime
     #   contourpy
     #   matplotlib
     #   netcdf4
     #   pandas
     #   pyerfa
     #   scipy
     #   seaborn
     #   xarray
+overrides==7.3.1
+    # via jupyter-server
 packaging==23.1
     # via
     #   astropy
     #   build
     #   conda-lock
     #   ipykernel
     #   jupyter-server
@@ -357,15 +331,15 @@
     #   matplotlib
     #   nbconvert
     #   pooch
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
     #   xarray
-pandas==2.0.1
+pandas==2.0.2
     # via
     #   seaborn
     #   xarray
 pandocfilters==1.5.0
     # via nbconvert
 parso==0.8.3
     # via jedi
@@ -373,42 +347,39 @@
     # via clikit
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
 pillow==9.5.0
     # via matplotlib
-pint==0.21
+pint==0.21.1
     # via
-    #   -r requirements/main.in
+    #   -r requirements/pip/main.in
     #   pinttrs
 pinttrs==23.2.0
-    # via -r requirements/main.in
+    # via -r requirements/pip/main.in
 pip-tools==6.13.0
-    # via -r requirements/dev.in
+    # via -r requirements/pip/dev.in
 pkginfo==1.9.6
     # via conda-lock
 pkgutil-resolve-name==1.3.10
     # via jsonschema
-platformdirs==3.5.0
+platformdirs==3.6.0
     # via
     #   jupyter-core
     #   pooch
     #   virtualenv
 pluggy==1.0.0
     # via pytest
 pooch==1.7.0
-    # via -r requirements/main.in
+    # via -r requirements/pip/main.in
 portion==2.4.0
-    # via -r requirements/main.in
-prometheus-client==0.16.0
-    # via
-    #   jupyter-server
-    #   nbclassic
-    #   notebook
+    # via -r requirements/pip/main.in
+prometheus-client==0.17.0
+    # via jupyter-server
 prompt-toolkit==3.0.38
     # via ipython
 psutil==5.9.5
     # via ipykernel
 ptyprocess==0.7.0
     # via
     #   pexpect
@@ -419,15 +390,15 @@
     # via
     #   pybtex-docutils
     #   sphinxcontrib-bibtex
 pybtex-docutils==1.0.2
     # via sphinxcontrib-bibtex
 pycparser==2.21
     # via cffi
-pydantic==1.10.7
+pydantic==1.10.9
     # via conda-lock
 pydata-sphinx-theme==0.13.3
     # via sphinx-book-theme
 pyerfa==2.0.0.3
     # via astropy
 pygments==2.15.1
     # via
@@ -435,32 +406,32 @@
     #   ipython
     #   nbconvert
     #   pydata-sphinx-theme
     #   rich
     #   sphinx
 pylev==1.4.0
     # via clikit
-pyparsing==3.0.9
+pyparsing==3.1.0
     # via matplotlib
 pyproject-hooks==1.0.0
     # via build
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.3.1
+pytest==7.3.2
     # via
-    #   -r requirements/tests.in
+    #   -r requirements/pip/tests.in
     #   pytest-json-report
     #   pytest-metadata
 pytest-json-report==1.5.0
-    # via -r requirements/tests.in
-pytest-metadata==2.0.4
+    # via -r requirements/pip/tests.in
+pytest-metadata==3.0.0
     # via pytest-json-report
 python-dateutil==2.8.2
     # via
-    #   -r requirements/recommended.in
+    #   -r requirements/pip/recommended.in
     #   arrow
     #   jupyter-client
     #   matplotlib
     #   pandas
 python-json-logger==2.0.7
     # via jupyter-events
 pytz==2023.3
@@ -470,22 +441,20 @@
 pyyaml==6.0
     # via
     #   astropy
     #   conda-lock
     #   jupyter-events
     #   myst-parser
     #   pybtex
-pyzmq==25.0.2
+pyzmq==25.1.0
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
-    #   nbclassic
-    #   notebook
-requests==2.30.0
+requests==2.31.0
     # via
     #   cachecontrol
     #   conda-lock
     #   ensureconda
     #   jupyterlab-server
     #   pooch
     #   sphinx
@@ -493,79 +462,78 @@
     # via
     #   jsonschema
     #   jupyter-events
 rfc3986-validator==0.1.1
     # via
     #   jsonschema
     #   jupyter-events
-rich==13.3.5
-    # via -r requirements/main.in
-ruamel-yaml==0.17.24
+rich==13.4.2
+    # via -r requirements/pip/main.in
+ruamel-yaml==0.17.32
     # via
-    #   -r requirements/main.in
+    #   -r requirements/pip/main.in
     #   conda-lock
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.10.1
     # via
-    #   -r requirements/main.in
+    #   -r requirements/pip/main.in
     #   iapws
 seaborn==0.12.2
-    # via -r requirements/recommended.in
+    # via -r requirements/pip/recommended.in
 secretstorage==3.3.3
     # via keyring
 send2trash==1.8.2
-    # via
-    #   jupyter-server
-    #   nbclassic
-    #   notebook
+    # via jupyter-server
 shellingham==1.5.0.post1
-    # via -r requirements/main.in
+    # via -r requirements/pip/main.in
 six==1.16.0
     # via
     #   asttokens
     #   bleach
     #   html5lib
     #   latexcodec
     #   livereload
     #   pybtex
     #   python-dateutil
     #   rfc3339-validator
+smmap==5.0.0
+    # via gitdb
 sniffio==1.3.0
     # via anyio
 snowballstemmer==2.2.0
     # via sphinx
 sortedcontainers==2.4.0
     # via portion
 soupsieve==2.4.1
     # via beautifulsoup4
 sphinx==6.2.1
     # via
-    #   -r requirements/docs.in
+    #   -r requirements/pip/docs.in
     #   autodocsumm
     #   myst-parser
     #   nbsphinx
     #   pydata-sphinx-theme
     #   sphinx-autobuild
     #   sphinx-book-theme
     #   sphinx-copybutton
     #   sphinx-design
     #   sphinxcontrib-bibtex
 sphinx-autobuild==2021.3.14
-    # via -r requirements/docs.in
+    # via -r requirements/pip/docs.in
 sphinx-book-theme==1.0.1
-    # via -r requirements/docs.in
+    # via -r requirements/pip/docs.in
 sphinx-copybutton==0.5.2
-    # via -r requirements/docs.in
+    # via -r requirements/pip/docs.in
 sphinx-design==0.4.1
-    # via -r requirements/docs.in
+    # via -r requirements/pip/docs.in
 sphinxcontrib-applehelp==1.0.4
     # via sphinx
 sphinxcontrib-bibtex==2.5.0
-    # via -r requirements/docs.in
+    # via -r requirements/pip/docs.in
 sphinxcontrib-devhelp==1.0.2
     # via sphinx
 sphinxcontrib-htmlhelp==2.0.1
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.3
@@ -574,106 +542,98 @@
     # via sphinx
 stack-data==0.6.2
     # via ipython
 terminado==0.17.1
     # via
     #   jupyter-server
     #   jupyter-server-terminals
-    #   nbclassic
-    #   notebook
 tinycss2==1.2.1
     # via nbconvert
 tomli==2.0.1
     # via
     #   build
     #   conda-lock
     #   jupyterlab
     #   pyproject-hooks
     #   pytest
 tomlkit==0.11.8
     # via conda-lock
 toolz==0.12.0
     # via conda-lock
-tornado==6.3.1
+tornado==6.3.2
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   jupyterlab
     #   livereload
-    #   nbclassic
-    #   notebook
     #   terminado
 tqdm==4.65.0
-    # via -r requirements/main.in
+    # via -r requirements/pip/main.in
 traitlets==5.9.0
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   jupyter-events
     #   jupyter-server
+    #   jupyterlab
     #   matplotlib-inline
-    #   nbclassic
     #   nbclient
     #   nbconvert
     #   nbformat
     #   nbsphinx
-    #   notebook
 typer==0.9.0
-    # via -r requirements/main.in
-typing-extensions==4.5.0
+    # via -r requirements/pip/main.in
+typing-extensions==4.6.3
     # via
+    #   async-lru
     #   conda-lock
     #   ipython
     #   pydantic
     #   pydata-sphinx-theme
     #   rich
     #   typer
 tzdata==2023.3
     # via pandas
 uri-template==1.2.0
     # via jsonschema
-urllib3==2.0.2
-    # via requests
-virtualenv==20.23.0
+urllib3==1.26.16
+    # via
+    #   conda-lock
+    #   requests
+virtualenv==20.23.1
     # via conda-lock
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
 webencodings==0.5.1
     # via
     #   bleach
     #   html5lib
     #   tinycss2
-websocket-client==1.5.1
+websocket-client==1.6.0
     # via jupyter-server
 wheel==0.40.0
     # via pip-tools
 widgetsnbextension==4.0.7
     # via ipywidgets
 xarray==2023.1.0
-    # via -r requirements/main.in
-y-py==0.5.9
-    # via
-    #   jupyter-ydoc
-    #   ypy-websocket
-ypy-websocket==0.8.2
-    # via jupyter-server-ydoc
+    # via -r requirements/pip/main.in
 zipp==3.15.0
     # via
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 pip==23.1.2
     # via
-    #   -r requirements/dev.in
+    #   -r requirements/pip/dev.in
     #   pip-tools
-setuptools==67.7.2
+setuptools==68.0.0
     # via
-    #   -r requirements/dev.in
+    #   -r requirements/pip/dev.in
     #   pip-tools
```

### Comparing `eradiate-0.23.2rc1/requirements/docs.txt` & `eradiate-0.23.2rc2/requirements/pip/docs.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,463 +1,464 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --allow-unsafe --output-file=requirements/docs.txt --resolver=backtracking requirements/docs.in
+#    pip-compile --allow-unsafe --output-file=requirements/pip/docs.txt --resolver=backtracking requirements/pip/docs.in
 #
 accessible-pygments==0.0.4
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   pydata-sphinx-theme
 aenum==3.1.12
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
 alabaster==0.7.13
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   sphinx
 attrs==23.1.0
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
     #   dessinemoi
     #   environ-config
     #   jsonschema
     #   pinttrs
 autodocsumm==0.2.11
-    # via -r requirements/docs.in
+    # via -r requirements/pip/docs.in
 babel==2.12.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   nbconvert
     #   pydata-sphinx-theme
 bleach==6.0.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   nbconvert
 certifi==2023.5.7
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
+    #   netcdf4
     #   requests
 cftime==1.6.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   netcdf4
 charset-normalizer==3.1.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   requests
 click==8.1.3
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
     #   typer
 colorama==0.4.6
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   sphinx-autobuild
-contourpy==1.0.7
+contourpy==1.1.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   matplotlib
 cycler==0.11.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   matplotlib
 defusedxml==0.7.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   nbconvert
 dessinemoi==23.1.0
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
 docutils==0.19
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   myst-parser
     #   nbsphinx
     #   pybtex-docutils
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinxcontrib-bibtex
 environ-config==23.2.0
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
-fastjsonschema==2.16.3
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
+fastjsonschema==2.17.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   nbformat
-fonttools==4.39.3
+fonttools==4.40.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   matplotlib
 idna==3.4
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   requests
 imagesize==1.4.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   sphinx
-importlib-metadata==6.6.0
+importlib-metadata==6.7.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jupyter-client
     #   nbconvert
     #   sphinx
     #   sphinxcontrib-bibtex
 importlib-resources==5.12.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jsonschema
     #   matplotlib
 jinja2==3.1.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   myst-parser
     #   nbconvert
     #   nbsphinx
     #   sphinx
 jsonschema==4.17.3
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   nbformat
 jupyter-client==8.2.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   nbclient
-jupyter-core==5.3.0
+jupyter-core==5.3.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jupyter-client
     #   nbclient
     #   nbconvert
     #   nbformat
 jupyterlab-pygments==0.2.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   nbconvert
 kiwisolver==1.4.4
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   matplotlib
 latexcodec==2.0.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   pybtex
 lazy-loader==0.2
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
 livereload==2.6.3
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   sphinx-autobuild
-markdown-it-py==2.2.0
+markdown-it-py==3.0.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   mdit-py-plugins
     #   myst-parser
     #   rich
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jinja2
     #   nbconvert
 matplotlib==3.7.1
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
-mdit-py-plugins==0.3.5
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
+mdit-py-plugins==0.4.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   myst-parser
 mdurl==0.1.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   markdown-it-py
-mistune==2.0.5
+mistune==3.0.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   nbconvert
-myst-parser==1.0.0
-    # via -r requirements/docs.in
-nbclient==0.7.4
+myst-parser==2.0.0
+    # via -r requirements/pip/docs.in
+nbclient==0.8.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   nbconvert
-nbconvert==7.4.0
+nbconvert==7.6.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   nbsphinx
-nbformat==5.8.0
+nbformat==5.9.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   nbclient
     #   nbconvert
     #   nbsphinx
-nbsphinx==0.9.1
-    # via -r requirements/docs.in
-netcdf4==1.6.3
+nbsphinx==0.9.2
+    # via -r requirements/pip/docs.in
+netcdf4==1.6.4
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
 numpy==1.24.3
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
     #   cftime
     #   contourpy
     #   matplotlib
     #   netcdf4
     #   pandas
     #   scipy
     #   xarray
 packaging==23.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   matplotlib
     #   nbconvert
     #   pooch
     #   pydata-sphinx-theme
     #   sphinx
     #   xarray
-pandas==2.0.1
+pandas==2.0.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   xarray
 pandocfilters==1.5.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   nbconvert
 pillow==9.5.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   matplotlib
-pint==0.21
+pint==0.21.1
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
     #   pinttrs
 pinttrs==23.2.0
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
 pkgutil-resolve-name==1.3.10
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jsonschema
-platformdirs==3.5.0
+platformdirs==3.6.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jupyter-core
     #   pooch
 pooch==1.7.0
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
 portion==2.4.0
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
 pybtex==0.24.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   pybtex-docutils
     #   sphinxcontrib-bibtex
 pybtex-docutils==1.0.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   sphinxcontrib-bibtex
 pydata-sphinx-theme==0.13.3
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   sphinx-book-theme
 pygments==2.15.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   accessible-pygments
     #   nbconvert
     #   pydata-sphinx-theme
     #   rich
     #   sphinx
-pyparsing==3.0.9
+pyparsing==3.1.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   matplotlib
 pyrsistent==0.19.3
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jsonschema
 python-dateutil==2.8.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jupyter-client
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   babel
     #   pandas
 pyyaml==6.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   myst-parser
     #   pybtex
-pyzmq==25.0.2
+pyzmq==25.1.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jupyter-client
-requests==2.30.0
+requests==2.31.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   pooch
     #   sphinx
-rich==13.3.5
+rich==13.4.2
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
-ruamel-yaml==0.17.24
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
+ruamel-yaml==0.17.32
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
 ruamel-yaml-clib==0.2.7
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   ruamel-yaml
 scipy==1.10.1
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
 shellingham==1.5.0.post1
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
 six==1.16.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   bleach
     #   latexcodec
     #   livereload
     #   pybtex
     #   python-dateutil
 snowballstemmer==2.2.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   sphinx
 sortedcontainers==2.4.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   portion
 soupsieve==2.4.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   beautifulsoup4
 sphinx==6.2.1
     # via
-    #   -r requirements/docs.in
+    #   -r requirements/pip/docs.in
     #   autodocsumm
     #   myst-parser
     #   nbsphinx
     #   pydata-sphinx-theme
     #   sphinx-autobuild
     #   sphinx-book-theme
     #   sphinx-copybutton
     #   sphinx-design
     #   sphinxcontrib-bibtex
 sphinx-autobuild==2021.3.14
-    # via -r requirements/docs.in
+    # via -r requirements/pip/docs.in
 sphinx-book-theme==1.0.1
-    # via -r requirements/docs.in
+    # via -r requirements/pip/docs.in
 sphinx-copybutton==0.5.2
-    # via -r requirements/docs.in
+    # via -r requirements/pip/docs.in
 sphinx-design==0.4.1
-    # via -r requirements/docs.in
+    # via -r requirements/pip/docs.in
 sphinxcontrib-applehelp==1.0.4
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   sphinx
 sphinxcontrib-bibtex==2.5.0
-    # via -r requirements/docs.in
+    # via -r requirements/pip/docs.in
 sphinxcontrib-devhelp==1.0.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   sphinx
 sphinxcontrib-htmlhelp==2.0.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   sphinx
 sphinxcontrib-jsmath==1.0.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   sphinx
 sphinxcontrib-qthelp==1.0.3
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   sphinx
 tinycss2==1.2.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   nbconvert
-tornado==6.3.1
+tornado==6.3.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jupyter-client
     #   livereload
 tqdm==4.65.0
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
 traitlets==5.9.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jupyter-client
     #   jupyter-core
     #   nbclient
     #   nbconvert
     #   nbformat
     #   nbsphinx
 typer==0.9.0
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
-typing-extensions==4.5.0
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
+typing-extensions==4.6.3
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   pydata-sphinx-theme
     #   rich
     #   typer
 tzdata==2023.3
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   pandas
-urllib3==2.0.2
+urllib3==1.26.16
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   requests
 webencodings==0.5.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   bleach
     #   tinycss2
 xarray==2023.1.0
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
 zipp==3.15.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   importlib-metadata
     #   importlib-resources
```

### Comparing `eradiate-0.23.2rc1/requirements/environment-dev.yml` & `eradiate-0.23.2rc2/requirements/conda/environment-dev.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,44 @@
 channels:
   - eradiate
   - conda-forge
   - defaults
 dependencies:
+  # default
   - python=3.8
+  # dev
+  - conda-lock>=1.4
+  - networkx>=3.1
+  - pip-tools>=6.5
+  - pip>=22
+  - setuptools>=61
+  # docs
+  - autodocsumm
+  - myst-parser
+  - nbsphinx>=0.9.0
+  - sphinx
+  - sphinx-autobuild
+  - sphinx-book-theme>=1.0
+  - sphinx-copybutton
+  - sphinx-design
+  - sphinxcontrib-bibtex>=2.0
   # main
   - aenum
   - attrs>=22.2
   - click
   - dessinemoi>=23.1.0
   - environ-config
   - lazy_loader>=0.1
   - matplotlib>=3.3
   - netcdf4
   - numpy
   - pint
   - pinttrs>=23.2.0
-  - portion
   - pooch
+  - portion
   - rich
   - ruamel.yaml
   - scipy
   - shellingham!=1.5.1
   - tqdm
   - typer>=0.9.0
   - xarray>=0.19,!=0.20.*
@@ -30,22 +47,10 @@
   - astropy
   - iapws
   - ipython
   - ipywidgets
   - jupyterlab
   - python-dateutil
   - seaborn
-  # docs
-  - autodocsumm
-  - myst-parser
-  - nbsphinx>=0.9.0
-  - sphinx-book-theme>=1.0
-  - sphinx
-  - sphinxcontrib-bibtex>=2.0
-  - sphinx-autobuild
-  - sphinx-copybutton
-  - sphinx-design
-  # dev
-  - conda-lock>=1.4
-  - pip>=22
-  - pip-tools>=6.5
-  - setuptools>=61
+  # tests
+  - pytest
+  - pytest-json-report
```

### Comparing `eradiate-0.23.2rc1/requirements/environment-linux-64.lock` & `eradiate-0.23.2rc2/requirements/conda/environment-dev-linux-64.lock`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # Generated by conda-lock.
 # platform: linux-64
-# input_hash: 922343b773c5cdc6056bd3a0d516a9b971595f509375033c9ca82e60a9716e7f
+# input_hash: 9dcecc3b104941efb0fda739f479016fbf6654d5f0596f31fc7e8f13170c7d08
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
 https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2023.5.7-hbcca054_0.conda#f5c65075fc34438d5b456c7f3f5ab695
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-dejavu-sans-mono-2.37-hab24e00_0.tar.bz2#0c96522c6bdaed4b1566d11387caaf45
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-inconsolata-3.000-h77eed37_0.tar.bz2#34893075a5c9e55cdafac56607368fc6
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-source-code-pro-2.038-h77eed37_0.tar.bz2#4d59c254e01d9cde7957100457e2d5fb
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-ubuntu-0.83-hab24e00_0.tar.bz2#19410c3df09dfb12d1206132a1d357c5
 https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda#7aca3059a1729aa76c597603f10b0dd3
-https://conda.anaconda.org/conda-forge/linux-64/libgfortran5-12.2.0-h337968e_19.tar.bz2#164b4b1acaedc47ee7e658ae6b308ca3
-https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-12.2.0-h46fd767_19.tar.bz2#1030b1f38c129f2634eae026f704fe60
+https://conda.anaconda.org/conda-forge/linux-64/libgfortran5-13.1.0-h15d22d2_0.conda#afb656a334c409dd9805508af1c89c7a
+https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.1.0-hfd8a6a1_0.conda#067bcc23164642f4c226da631f2a2e1d
 https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.8-3_cp38.conda#2f3f7af062b42d664117662612022204
 https://conda.anaconda.org/conda-forge/noarch/fonts-conda-forge-1-0.tar.bz2#f766549260d6815b0c52253f1fb1bb29
-https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-12.2.0-h69a702a_19.tar.bz2#cd7a806282c16e1f2d39a7e80d3a3e0d
-https://conda.anaconda.org/conda-forge/linux-64/libgomp-12.2.0-h65d4601_19.tar.bz2#cedcee7c064c01c403f962c9e8d3c373
+https://conda.anaconda.org/conda-forge/linux-64/libgfortran-ng-13.1.0-h69a702a_0.conda#506dc07710dd5b0ba63cbf134897fc10
+https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.1.0-he5830b7_0.conda#56ca14d57ac29a75d23a39eb3ee0ddeb
 https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
 https://conda.anaconda.org/conda-forge/noarch/fonts-conda-ecosystem-1-0.tar.bz2#fee5683a3f04bd15cbd8318b096a27ab
-https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-12.2.0-h65d4601_19.tar.bz2#e4c94f80aef025c17ab0828cd85ef535
+https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.1.0-he5830b7_0.conda#cd93f779ff018dd85c7544c015c9db3c
 https://conda.anaconda.org/conda-forge/linux-64/alsa-lib-1.2.8-h166bdaf_0.tar.bz2#be733e69048951df1e4b4b7bb8c7666f
 https://conda.anaconda.org/conda-forge/linux-64/attr-2.5.1-h166bdaf_1.tar.bz2#d9c69a24ad678ffce24c6543a0176b00
 https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-h7f98852_4.tar.bz2#a1fd65c7ccbf10880423d82bca54eb54
-https://conda.anaconda.org/conda-forge/linux-64/c-ares-1.18.1-h7f98852_0.tar.bz2#f26ef8098fab1f719c91eb760d63381a
+https://conda.anaconda.org/conda-forge/linux-64/c-ares-1.19.1-hd590300_0.conda#e8c18d865be43e2fb3f7a145b6adf1f5
 https://conda.anaconda.org/conda-forge/linux-64/gettext-0.21.1-h27087fc_0.tar.bz2#14947d8770185e5153fdd04d4673ed37
+https://conda.anaconda.org/conda-forge/linux-64/gmp-6.2.1-h58526e2_0.tar.bz2#b94cf2db16066b242ebd26db2facbd56
 https://conda.anaconda.org/conda-forge/linux-64/graphite2-1.3.13-h58526e2_1001.tar.bz2#8c54672728e8ec6aa6db90cf2806d220
 https://conda.anaconda.org/conda-forge/linux-64/icu-72.1-hcb278e6_0.conda#7c8d20d847bb45f56bd941578fcfa146
 https://conda.anaconda.org/conda-forge/linux-64/keyutils-1.6.1-h166bdaf_0.tar.bz2#30186d27e2c9fa62b45fb1476b7200e3
 https://conda.anaconda.org/conda-forge/linux-64/lame-3.100-h166bdaf_1003.tar.bz2#a8832b479f93521a9e7b5b743803be51
 https://conda.anaconda.org/conda-forge/linux-64/lerc-4.0.0-h27087fc_0.tar.bz2#76bbff344f0134279f225174e9064c8f
 https://conda.anaconda.org/conda-forge/linux-64/libaec-1.0.6-hcb278e6_1.conda#0f683578378cddb223e7fd24f785ab2a
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.0.9-h166bdaf_8.tar.bz2#9194c9bf9428035a05352d031462eae4
@@ -34,86 +35,84 @@
 https://conda.anaconda.org/conda-forge/linux-64/libev-4.33-h516909a_1.tar.bz2#6f8720dff19e17ce5d48cfe7f3d2f0a3
 https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.5.0-hcb278e6_1.conda#6305a3dd2752c76335295da4e581f2fd
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
 https://conda.anaconda.org/conda-forge/linux-64/libiconv-1.17-h166bdaf_0.tar.bz2#b62b52da46c39ee2bc3c162ac7f1804d
 https://conda.anaconda.org/conda-forge/linux-64/libjpeg-turbo-2.1.5.1-h0b41bf4_0.conda#1edd9e67bdb90d78cea97733ff6b54e6
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2#39b1328babf85c7c3a61636d9cd50206
 https://conda.anaconda.org/conda-forge/linux-64/libogg-1.3.4-h7f98852_1.tar.bz2#6e8cc2173440d77708196c5b93771680
-https://conda.anaconda.org/conda-forge/linux-64/libopenblas-0.3.21-pthreads_h78a6416_3.tar.bz2#8c5963a49b6035c40646a763293fbb35
+https://conda.anaconda.org/conda-forge/linux-64/libopenblas-0.3.23-pthreads_h80387f5_0.conda#9c5ea51ccb8ffae7d06c645869d24ce6
 https://conda.anaconda.org/conda-forge/linux-64/libopus-1.3.1-h7f98852_1.tar.bz2#15345e56d527b330e1cacbdf58676e8f
 https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2#c3788462a6fbddafdb413a9f9053e58d
 https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
 https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.3.0-h0b41bf4_0.conda#0d4a7508d8c6c65314f2b9c1f56ad408
-https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-h166bdaf_4.tar.bz2#f3f9de449d32ca9b9c66a22863c96f41
+https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda#f36c115f1ee199da648e0597ec2047ad
 https://conda.anaconda.org/conda-forge/linux-64/lz4-c-1.9.4-hcb278e6_0.conda#318b08df404f9c9be5712aaa5a6f0bb0
 https://conda.anaconda.org/conda-forge/linux-64/mpg123-1.31.3-hcb278e6_0.conda#141a126675b6d1a4eabb111a4a353898
-https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.3-h27087fc_1.tar.bz2#4acfc691e64342b9dae57cf2adc63238
+https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4-hcb278e6_0.conda#681105bccc2a3f7f1a837d47d39c9179
 https://conda.anaconda.org/conda-forge/linux-64/nspr-4.35-h27087fc_0.conda#da0ec11a6454ae19bff5b02ed881a2b1
-https://conda.anaconda.org/conda-forge/linux-64/openssl-3.1.0-hd590300_3.conda#8f24d371ed9efb3f0b0de383fb81d51c
+https://conda.anaconda.org/conda-forge/linux-64/openssl-3.1.1-hd590300_1.conda#2e1d7b458ac8f1e3ca4e18b77add6277
 https://conda.anaconda.org/conda-forge/linux-64/pixman-0.40.0-h36c2ea0_0.tar.bz2#660e72c82f2e75a6b3fe6a6e75c79f19
 https://conda.anaconda.org/conda-forge/linux-64/pthread-stubs-0.4-h36c2ea0_1001.tar.bz2#22dad4df6e8630e8dff2428f6f6a7036
 https://conda.anaconda.org/conda-forge/linux-64/snappy-1.1.10-h9fff704_0.conda#e6d228cd0bb74a51dd18f5bfce0b4115
-https://conda.anaconda.org/conda-forge/linux-64/xkeyboard-config-2.38-h0b41bf4_0.conda#9ac34337e5101a87e5d91da05d84aa48
 https://conda.anaconda.org/conda-forge/linux-64/xorg-kbproto-1.0.7-h7f98852_1002.tar.bz2#4b230e8381279d76131116660f5a241a
-https://conda.anaconda.org/conda-forge/linux-64/xorg-libice-1.0.10-h7f98852_0.tar.bz2#d6b0b50b49eccfe0be0373be628be0f3
-https://conda.anaconda.org/conda-forge/linux-64/xorg-libxau-1.0.9-h7f98852_0.tar.bz2#bf6f803a544f26ebbdc3bfff272eb179
+https://conda.anaconda.org/conda-forge/linux-64/xorg-libice-1.1.1-hd590300_0.conda#b462a33c0be1421532f28bfe8f4a7514
+https://conda.anaconda.org/conda-forge/linux-64/xorg-libxau-1.0.11-hd590300_0.conda#2c80dc38fface310c9bd81b17037fee5
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxdmcp-1.1.3-h7f98852_0.tar.bz2#be93aabceefa2fac576e971aef407908
 https://conda.anaconda.org/conda-forge/linux-64/xorg-renderproto-0.11.1-h7f98852_1002.tar.bz2#06feff3d2634e3097ce2fe681474b534
 https://conda.anaconda.org/conda-forge/linux-64/xorg-xextproto-7.3.0-h0b41bf4_1003.conda#bce9f945da8ad2ae9b1d7165a64d0f87
 https://conda.anaconda.org/conda-forge/linux-64/xorg-xf86vidmodeproto-2.3.1-h7f98852_1002.tar.bz2#3ceea9668625c18f19530de98b15d5b0
 https://conda.anaconda.org/conda-forge/linux-64/xorg-xproto-7.0.31-h7f98852_1007.tar.bz2#b4a4381d54784606820704f7b5f05a15
 https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2#2161070d867d1b1204ea749c8eec4ef0
 https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2#4cb3ad778ec2d5a7acbdf254eb1c42ae
 https://conda.anaconda.org/conda-forge/linux-64/expat-2.5.0-hcb278e6_1.conda#8b9b5aca60558d02ddaa09d599e55920
 https://conda.anaconda.org/conda-forge/linux-64/hdf4-4.2.15-h501b40f_6.conda#c3e9338e15d90106f467377017352b97
-https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-16_linux64_openblas.tar.bz2#d9b7a8639171f6c6fa0a983edabcfe2b
+https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-17_linux64_openblas.conda#57fb44770b1bc832fb2dbefa1bd502de
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.0.9-h166bdaf_8.tar.bz2#4ae4d7795d33e02bd20f6b23d91caf82
 https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.0.9-h166bdaf_8.tar.bz2#04bac51ba35ea023dc48af73c1c88c25
 https://conda.anaconda.org/conda-forge/linux-64/libcap-2.67-he9d0100_0.conda#d05556c80caffff164d17bdea0105a1a
 https://conda.anaconda.org/conda-forge/linux-64/libedit-3.1.20191231-he28a2e2_2.tar.bz2#4d331e44109e3f0e19b4cb8f9b82f3e1
-https://conda.anaconda.org/conda-forge/linux-64/libevent-2.1.10-h28343ad_4.tar.bz2#4a049fc560e00e43151dc51368915fdd
+https://conda.anaconda.org/conda-forge/linux-64/libevent-2.1.12-hf998b51_1.conda#a1cfcc585f0c42bf8d5546bb1dfb668d
 https://conda.anaconda.org/conda-forge/linux-64/libflac-1.4.2-h27087fc_0.tar.bz2#7daf72d8e2a8e848e11d63ed6d1026e0
-https://conda.anaconda.org/conda-forge/linux-64/libgpg-error-1.46-h620e276_0.conda#27e745f6f2e4b757e95dd7225fbe6bdb
+https://conda.anaconda.org/conda-forge/linux-64/libgpg-error-1.47-h71f35ed_0.conda#c2097d0b46367996f09b4e8e4920384a
 https://conda.anaconda.org/conda-forge/linux-64/libnghttp2-1.52.0-h61bc06f_0.conda#613955a50485812985c059e7b269f42e
 https://conda.anaconda.org/conda-forge/linux-64/libpng-1.6.39-h753d276_0.conda#e1c890aebdebbfbf87e2c917187b4416
-https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.41.2-h2797004_1.conda#1d002bf709048f8021c32abfd0e0d395
-https://conda.anaconda.org/conda-forge/linux-64/libssh2-1.10.0-hf14f497_3.tar.bz2#d85acad4b47dff4e3def14a769a97906
+https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.42.0-h2797004_0.conda#fdaae20a1cf7cd62130a0973190a31b7
+https://conda.anaconda.org/conda-forge/linux-64/libssh2-1.11.0-h0841786_0.conda#1f5a58e686b13bcfde88b93f547d23fe
 https://conda.anaconda.org/conda-forge/linux-64/libvorbis-1.3.7-h9c3ff4c_0.tar.bz2#309dec04b70a3cc0f1e84a4013683bc0
-https://conda.anaconda.org/conda-forge/linux-64/libxcb-1.13-h7f98852_1004.tar.bz2#b3653fdc58d03face9724f602218a904
-https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.10.4-hfdac1af_0.conda#241845899caff54ac1d2b3102ad988cf
+https://conda.anaconda.org/conda-forge/linux-64/libxcb-1.15-h0b41bf4_0.conda#33277193f5b92bad9fdd230eb700929c
+https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.11.4-h0d562d8_0.conda#e46fad17d5fb57316b956f88dca765e4
 https://conda.anaconda.org/conda-forge/linux-64/libzip-1.9.2-hc929e4a_1.tar.bz2#5b122b50e738c4be5c3f2899f010d7cf
-https://conda.anaconda.org/conda-forge/linux-64/mysql-common-8.0.32-hf1915f5_2.conda#cf4a8f520fdad3a63bb2bce74576cd2d
-https://conda.anaconda.org/conda-forge/linux-64/pandoc-2.19.2-h32600fe_2.conda#326f46f36d15c44cff5f81d505cb717f
+https://conda.anaconda.org/conda-forge/linux-64/mysql-common-8.0.33-hf1915f5_0.conda#aa8b86066614c4573f6db62c91978fa9
 https://conda.anaconda.org/conda-forge/linux-64/pcre2-10.40-hc3806b6_0.tar.bz2#69e2c796349cd9b273890bee0febfe1b
 https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
 https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
-https://conda.anaconda.org/conda-forge/linux-64/xorg-libsm-1.2.3-hd9c2040_1000.tar.bz2#9e856f78d5c80d5a78f61e72d1d473a3
+https://conda.anaconda.org/conda-forge/linux-64/xorg-libsm-1.2.4-h7391055_0.conda#93ee23f12bc2e684548181256edd2cf6
 https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.4-h9c3ff4c_1.tar.bz2#21743a8d2ea0c8cfbbf8fe489b0347df
-https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-h166bdaf_4.tar.bz2#4b11e365c0275b808be78b30f904e295
+https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda#68c34ec6149623be41a1933ab996a209
 https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.2-h3eb15da_6.conda#6b63daed8feeca47be78f323e793d555
-https://conda.anaconda.org/conda-forge/linux-64/blosc-1.21.3-hafa529b_0.conda#bcf0664a2dbbbb86cbd4c1e6ff10ddd6
+https://conda.anaconda.org/conda-forge/linux-64/blosc-1.21.4-h0f2a231_0.conda#876286b5941933a0f558777e57d883cc
 https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.0.9-h166bdaf_8.tar.bz2#e5613f2bc717e9945840ff474419b8e4
 https://conda.anaconda.org/conda-forge/linux-64/freetype-2.12.1-hca18f0e_1.conda#e1232042de76d24539a436d37597eb06
 https://conda.anaconda.org/conda-forge/linux-64/krb5-1.20.1-h81ceb04_0.conda#89a41adce7106749573d883b2f657d78
-https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-16_linux64_openblas.tar.bz2#20bae26d0a1db73f758fc3754cab4719
+https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-17_linux64_openblas.conda#7ef0969b00fe3d6eef56a8151d3afb29
 https://conda.anaconda.org/conda-forge/linux-64/libgcrypt-1.10.1-h166bdaf_0.tar.bz2#f967fc95089cd247ceed56eda31de3a9
-https://conda.anaconda.org/conda-forge/linux-64/libglib-2.76.2-hebfc3b9_0.conda#db1d4a1dfc04f3eab50d97551850759a
-https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-16_linux64_openblas.tar.bz2#955d993f41f9354bf753d29864ea20ad
-https://conda.anaconda.org/conda-forge/linux-64/libllvm16-16.0.3-hbf9e925_1.conda#3d942f062d7656168bb42b3439bdfede
+https://conda.anaconda.org/conda-forge/linux-64/libglib-2.76.3-hebfc3b9_0.conda#a64f11b244b2c112cd3fa1cbe9493999
+https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-17_linux64_openblas.conda#a2103882c46492e26500fcb56c03de8b
+https://conda.anaconda.org/conda-forge/linux-64/libllvm16-16.0.6-h5cf9203_0.conda#753e078cccad40fe4b396bdcf27a3c15
 https://conda.anaconda.org/conda-forge/linux-64/libsndfile-1.2.0-hb75c966_0.conda#c648d19cd9c8625898d5d370414de7c7
-https://conda.anaconda.org/conda-forge/linux-64/libtiff-4.5.0-ha587672_6.conda#4e5ee4b062c21519efbee7e2ae608748
-https://conda.anaconda.org/conda-forge/linux-64/libxkbcommon-1.5.0-h79f4944_1.conda#04a39cdd663f295653fc143851830563
-https://conda.anaconda.org/conda-forge/linux-64/mysql-libs-8.0.32-hca2cd23_2.conda#20b4708cd04bdc8138d03314ddd97885
+https://conda.anaconda.org/conda-forge/linux-64/libtiff-4.5.1-h8b53f26_0.conda#8ad377fb60abab446a9f02c62b3c2190
+https://conda.anaconda.org/conda-forge/linux-64/mysql-libs-8.0.33-hca2cd23_0.conda#276339b0115d92c6e0793dcdc7afe308
 https://conda.anaconda.org/conda-forge/linux-64/nss-3.89-he45b914_0.conda#2745719a58eeaab6657256a3f142f099
-https://conda.anaconda.org/conda-forge/linux-64/python-3.8.16-he550d4f_1_cpython.conda#9de84cccfbc5f8350a3667bb6ef6fc30
-https://conda.anaconda.org/conda-forge/linux-64/xcb-util-0.4.0-h166bdaf_0.tar.bz2#384e7fcb3cd162ba3e4aed4b687df566
-https://conda.anaconda.org/conda-forge/linux-64/xcb-util-keysyms-0.4.0-h166bdaf_0.tar.bz2#637054603bb7594302e3bf83f0a99879
-https://conda.anaconda.org/conda-forge/linux-64/xcb-util-renderutil-0.3.9-h166bdaf_0.tar.bz2#732e22f1741bccea861f5668cf7342a7
-https://conda.anaconda.org/conda-forge/linux-64/xcb-util-wm-0.4.1-h166bdaf_0.tar.bz2#0a8e20a8aef954390b9481a527421a8c
-https://conda.anaconda.org/conda-forge/linux-64/xorg-libx11-1.8.4-h0b41bf4_0.conda#ea8fbfeb976ac49cbeb594e985393514
+https://conda.anaconda.org/conda-forge/linux-64/pandoc-3.1.3-h32600fe_0.conda#8287aeb8462e2d4b235eff788e75919d
+https://conda.anaconda.org/conda-forge/linux-64/python-3.8.17-he550d4f_0_cpython.conda#72d038de0a228e4f0ef4011940641293
+https://conda.anaconda.org/conda-forge/linux-64/xcb-util-0.4.0-hd590300_1.conda#9bfac7ccd94d54fd21a0501296d60424
+https://conda.anaconda.org/conda-forge/linux-64/xcb-util-keysyms-0.4.0-h8ee46fc_1.conda#632413adcd8bc16b515cab87a2932913
+https://conda.anaconda.org/conda-forge/linux-64/xcb-util-renderutil-0.3.9-hd590300_1.conda#e995b155d938b6779da6ace6c6b13816
+https://conda.anaconda.org/conda-forge/linux-64/xcb-util-wm-0.4.1-h8ee46fc_1.conda#90108a432fb5c6150ccfee3f03388656
+https://conda.anaconda.org/conda-forge/linux-64/xorg-libx11-1.8.6-h8ee46fc_0.conda#7590b76c3d11d21caa44f3fc38ac584a
 https://conda.anaconda.org/eradiate/noarch/aabbtree-2.8.0-py_0.tar.bz2#647bcce5f0af4974e507591d5420486b
 https://conda.anaconda.org/conda-forge/noarch/aenum-3.1.12-pyhd8ed1ab_0.conda#602716538da00b2ca3cc85c4d35c0245
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.13-pyhd8ed1ab_0.conda#06006184e203b61d3525f90de394471e
 https://conda.anaconda.org/conda-forge/noarch/appdirs-1.4.4-pyh9f0ad1d_0.tar.bz2#5f095bc6454094e96f146491fd03633b
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
@@ -129,217 +128,231 @@
 https://conda.anaconda.org/conda-forge/linux-64/dbus-1.13.6-h5008d03_3.tar.bz2#ecfff944ba3960ecb334b9a2663d708d
 https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.6.7-py38h8dc9893_0.conda#e3c2cc835cf3223d585d1d25d56fd3de
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.6-pyhd8ed1ab_0.tar.bz2#b65b4d50dbd2d50fa0aeac367ec9eed7
 https://conda.anaconda.org/conda-forge/linux-64/docutils-0.16-py38h578d9bd_3.tar.bz2#a7866449fb9e5e4008a02df276549d34
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
-https://conda.anaconda.org/conda-forge/noarch/filelock-3.12.0-pyhd8ed1ab_0.conda#650f18a56f366dbf419c15b543592c2d
-https://conda.anaconda.org/conda-forge/noarch/flit-core-3.8.0-pyhd8ed1ab_0.tar.bz2#6d5e56de2e65da7aa35fd10131226efa
+https://conda.anaconda.org/conda-forge/noarch/filelock-3.12.2-pyhd8ed1ab_0.conda#53522ec72e6adae42bd373ef58357230
+https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/linux-64/fontconfig-2.14.2-h14ed4e7_0.conda#0f69b688f52ff6da70bccb7ff7001d1d
-https://conda.anaconda.org/conda-forge/linux-64/glib-tools-2.76.2-hfc55251_0.conda#7147b242b00aff73d95259ff318d14a0
+https://conda.anaconda.org/conda-forge/linux-64/glib-tools-2.76.3-hfc55251_0.conda#8951eedf3cdf94dd733c1b5eee1f4880
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
-https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
+https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/noarch/jeepney-0.8.0-pyhd8ed1ab_0.tar.bz2#9800ad1699b42612478755a2d26c722d
 https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_0.conda#1f39269ab88d1342c3e32935759e606a
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
 https://conda.anaconda.org/conda-forge/linux-64/kiwisolver-1.4.4-py38h43d8883_1.tar.bz2#41ca56d5cac7bfc7eb4fcdbee878eb84
 https://conda.anaconda.org/conda-forge/noarch/lazy_loader-0.2-pyhd8ed1ab_0.conda#d060d017720c9882c4eca0544a4a0592
 https://conda.anaconda.org/conda-forge/linux-64/lcms2-2.15-haa2dc70_1.conda#980d8aca0bc23ca73fa8caa3e7c84c28
-https://conda.anaconda.org/conda-forge/linux-64/libclang13-16.0.3-default_hd781213_0.conda#e0f95087543b73c7bc2689f0aeb86a6d
+https://conda.anaconda.org/conda-forge/linux-64/libclang13-16.0.6-default_h4d60ac6_0.conda#b10174a063ec195f8fe1b278282c3149
 https://conda.anaconda.org/conda-forge/linux-64/libcups-2.3.3-h36d4200_3.conda#c9f4416a34bc91e0eb029f912c68f81f
-https://conda.anaconda.org/conda-forge/linux-64/libcurl-8.0.1-h588be90_0.conda#b635278a73eb67edcfba7d01a6b48a03
-https://conda.anaconda.org/conda-forge/linux-64/libpq-15.2-hb675445_0.conda#4654b17eccaba55b8581d6b9c77f53cc
+https://conda.anaconda.org/conda-forge/linux-64/libcurl-8.1.2-h409715c_0.conda#50c873c9660ed116707ae15b663928d8
+https://conda.anaconda.org/conda-forge/linux-64/libpq-15.3-hbcd7760_1.conda#8afb2a97d256ffde95b91a6283bc598c
 https://conda.anaconda.org/conda-forge/linux-64/libsystemd0-253-h8c4010b_1.conda#9176b1e2cb8beca37a7510b0e801e38f
 https://conda.anaconda.org/conda-forge/noarch/lockfile-0.12.2-py_1.tar.bz2#c104d98e09c47519950cffb8dd5b4f10
-https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.2-py38h1de0b5d_0.conda#6d97b5d6f06933ab653f1862ddf6e33e
+https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.3-py38h01eb140_0.conda#17d2a5314adf0f25220eeebb312d00a4
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
-https://conda.anaconda.org/conda-forge/noarch/mistune-2.0.5-pyhd8ed1ab_0.conda#61a07195cfc935f1c1901d8ecf4af441
+https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
 https://conda.anaconda.org/conda-forge/noarch/more-itertools-9.1.0-pyhd8ed1ab_0.conda#1698a717f83cfecf644a877c174c84bd
 https://conda.anaconda.org/conda-forge/linux-64/msgpack-python-1.0.5-py38hfbd4bf9_0.conda#5401b83c1007f408d0c74e23fa9b5eff
 https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2#2ba8498c1018c1e9c61eb99b973dfe19
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
+https://conda.anaconda.org/conda-forge/noarch/networkx-3.1-pyhd8ed1ab_0.conda#254f787d5068bc89f578bf63893ce8b4
 https://conda.anaconda.org/conda-forge/linux-64/numpy-1.24.3-py38h59b608b_0.conda#5836e4ab0399136ede58446a4776b2ff
 https://conda.anaconda.org/conda-forge/linux-64/openjpeg-2.5.0-hfec8fc6_2.conda#5ce6a42505c6e9e6151c54c3ec8d68ea
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
 https://conda.anaconda.org/conda-forge/noarch/pastel-0.2.1-pyhd8ed1ab_0.tar.bz2#a4eea5bff523f26442405bc5d1f52adb
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pint-0.21-pyhd8ed1ab_0.conda#8d7b829e37d78447569c180f9d827005
 https://conda.anaconda.org/conda-forge/noarch/pkginfo-1.9.6-pyhd8ed1ab_0.conda#be1e9f1c65a1ed0f2ae9352fec99db64
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
+https://conda.anaconda.org/conda-forge/noarch/pluggy-1.0.0-pyhd8ed1ab_5.tar.bz2#7d301a0d25f424d96175f810935f0da9
 https://conda.anaconda.org/conda-forge/noarch/ply-3.11-py_1.tar.bz2#7205635cd71531943440fbfe3b6b5727
-https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.16.0-pyhd8ed1ab_0.conda#8efaddc1c8b8ce262c4d1a7c6571c799
+https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda#95c5be3c7cbd872509d16c216617fdab
 https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.5-py38h1de0b5d_0.conda#92e899e7b0ed27c793014d1fa54f9b7b
 https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
 https://conda.anaconda.org/conda-forge/noarch/pylev-1.4.0-pyhd8ed1ab_0.tar.bz2#edf8651c4379d9d1495ad6229622d150
-https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.0.9-pyhd8ed1ab_0.tar.bz2#e8fbc1b54b25f4b08281467bc13b70cc
+https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.0-pyhd8ed1ab_0.conda#d3ed087d1f7f8f5590e8e87b57a8ce64
 https://conda.anaconda.org/conda-forge/linux-64/pyrsistent-0.19.3-py38h1de0b5d_0.conda#a33157288d499397a2a56da4d724948d
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
-https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.16.3-pyhd8ed1ab_0.conda#7aa330a4d88b7ab891a42c39d5d2e742
+https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
 https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py38h0a891b7_5.tar.bz2#0856c59f9ddb710c640dc0428d66b1b7
-https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.0.2-py38he24dcef_0.conda#2809c142d8afb750687432f64da8a0a9
+https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.0-py38h509eb50_0.conda#33872b6650886eba869408b76c96994c
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml.clib-0.2.7-py38h1de0b5d_1.conda#9afa2fc3c51cc4e7d1589c38e4e00d5c
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyh41d4057_0.conda#ada5a17adcd10be4fc7e37e4166ba0e2
 https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
 https://conda.anaconda.org/conda-forge/noarch/shellingham-1.4.0-pyh44b312d_0.tar.bz2#437655338696f9d0dfdb0a024e66b255
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
+https://conda.anaconda.org/conda-forge/noarch/smmap-3.0.5-pyh44b312d_0.tar.bz2#3a8dc70789709aa315325d5df06fb7e4
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.4-pyhd8ed1ab_0.conda#5a31a7d564f551d0e6dff52fd8cb5b16
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.2-py_0.tar.bz2#68e01cac9d38d0e717cd5c87bc3d2cc9
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-htmlhelp-2.0.1-pyhd8ed1ab_0.conda#6c8c4d6eb2325e59290ac6dbbeacd5f0
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jsmath-1.0.1-py_0.tar.bz2#67cd9d9c0382d37479b4d306c369a2d4
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-qthelp-1.0.3-py_0.tar.bz2#d01180388e6d1838c3e1ad029590aa7a
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-serializinghtml-1.1.5-pyhd8ed1ab_2.tar.bz2#9ff55a0901cf952f05c654394de76bf7
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.11.8-pyha770c72_0.conda#75838e8556166263a82038b51d01d5f1
 https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.0-pyhd8ed1ab_0.tar.bz2#92facfec94bc02d6ccf42e7173831a36
-https://conda.anaconda.org/conda-forge/linux-64/tornado-6.3-py38h1de0b5d_0.conda#1371a9ace5486b295a373924803acaba
+https://conda.anaconda.org/conda-forge/linux-64/tornado-6.3.2-py38h01eb140_0.conda#3db869202b0e523d606d13e81ca79ab6
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.5.0-pyha770c72_0.conda#43e7d9e50261fb11deb76e17d8431aac
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.3-pyha770c72_0.conda#4a3014a4d107d15475d106b751c4e352
+https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/linux-64/unicodedata2-15.0.0-py38h0a891b7_0.tar.bz2#44421904760e9f5ae2035193e04360f0
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.5.1-pyhd8ed1ab_0.conda#2a914654b9ade742049dab13e29571c6
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.0-pyhd8ed1ab_0.conda#1dd6387a73d84e16b6f73de676bb4c36
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
 https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
-https://conda.anaconda.org/conda-forge/linux-64/xcb-util-image-0.4.0-h166bdaf_0.tar.bz2#c9b568bd804cb2903c6be6f5f68182e4
+https://conda.anaconda.org/conda-forge/linux-64/xcb-util-image-0.4.0-h8ee46fc_1.conda#9d7bcddf49cbf727730af10e71022c73
+https://conda.anaconda.org/conda-forge/linux-64/xkeyboard-config-2.39-hd590300_0.conda#d88c7fc8a11858fb14761832e4da1954
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxext-1.3.4-h0b41bf4_2.conda#82b6df12252e6f32402b96dacc656fec
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxrender-0.9.10-h7f98852_1003.tar.bz2#f59c1242cc1dd93e72c2ee2b360979eb
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
-https://conda.anaconda.org/conda-forge/noarch/anyio-3.6.2-pyhd8ed1ab_0.tar.bz2#8ada050fa88f26916fc1e76e368a49fd
+https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.0-pyhd8ed1ab_1.conda#2b35a85d654a47aac8f34c1bb6de7142
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
+https://conda.anaconda.org/conda-forge/noarch/async-lru-2.0.2-pyhd8ed1ab_0.conda#41221f97a0c82e5a60b21716a3d7469c
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
 https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
-https://conda.anaconda.org/conda-forge/linux-64/cairo-1.16.0-h35add3b_1015.conda#0c944213e40c9e4aa32292776b9c6903
+https://conda.anaconda.org/conda-forge/linux-64/cairo-1.16.0-hbbf8b49_1016.conda#c1dd96500b9b1a75e9e511931f415cbc
 https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py38h4a40e3a_3.conda#3ac112151c6b6cfe457e976de41af0c5
 https://conda.anaconda.org/conda-forge/linux-64/cftime-1.6.2-py38h26c90d9_1.tar.bz2#dcc025a7bb54374979c500c2e161fac9
 https://conda.anaconda.org/conda-forge/noarch/click-default-group-1.2.2-pyhd8ed1ab_1.tar.bz2#72a46ffc25701c173932fd55cf0965d3
 https://conda.anaconda.org/conda-forge/noarch/clikit-0.6.2-pyhd8ed1ab_2.conda#02abb7b66b02e8b9f5a9b05454400087
 https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
-https://conda.anaconda.org/conda-forge/linux-64/contourpy-1.0.7-py38hfbd4bf9_0.conda#638537863b298151635c05c762a997ab
-https://conda.anaconda.org/conda-forge/linux-64/curl-8.0.1-h588be90_0.conda#69691e828381dd12df671c26b680f1b0
+https://conda.anaconda.org/conda-forge/linux-64/contourpy-1.1.0-py38h7f3f72f_0.conda#0fdf3cc879156e0234e05962d55b6502
+https://conda.anaconda.org/conda-forge/linux-64/curl-8.1.2-h409715c_0.conda#9f88cfb15b7d08b25880b138f91e0eb4
 https://conda.anaconda.org/eradiate/noarch/dessinemoi-23.1.0-py_0.tar.bz2#490780e63e113a7dc444bd068e049bfe
 https://conda.anaconda.org/conda-forge/noarch/environ-config-22.1.0-pyhd8ed1ab_0.tar.bz2#a1103faffa0a877313c1fba776aa0fc0
-https://conda.anaconda.org/conda-forge/linux-64/fonttools-4.39.3-py38h1de0b5d_0.conda#34449fe6e3949956fac2236c9a9a3d3b
-https://conda.anaconda.org/conda-forge/linux-64/glib-2.76.2-hfc55251_0.conda#00c19ae01a69fb4e1a3fb3e83094dedf
+https://conda.anaconda.org/conda-forge/linux-64/fonttools-4.40.0-py38h01eb140_0.conda#f893b6bac56c477dd71498569b4a9022
+https://conda.anaconda.org/conda-forge/noarch/gitdb-4.0.10-pyhd8ed1ab_0.conda#3706d2f3d7cb5dae600c833345a76132
+https://conda.anaconda.org/conda-forge/linux-64/glib-2.76.3-hfc55251_0.conda#950e02f5665f5f4ff0437a6acba58798
 https://conda.anaconda.org/conda-forge/linux-64/hdf5-1.14.0-nompi_hb72d44e_103.conda#975973a4350ab45ff1981fe535a12af5
 https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2#b2355343d6315c892543200231d7154a
-https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.6.0-pyha770c72_0.conda#f91a5d5175fb7ff2a91952ec7da59cb9
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.7.0-pyha770c72_0.conda#ba3786c6846e46038fe60c785d46dc81
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.2.3-pyhd8ed1ab_0.tar.bz2#31e4a1506968d017229bdb64695013a1
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
+https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-4.12.0-py38h578d9bd_0.conda#e7f204764ab3683174c1707240368b84
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
 https://conda.anaconda.org/conda-forge/noarch/latexcodec-2.0.1-pyh9f0ad1d_0.tar.bz2#8d67904973263afd2985ba56aa2d6bb4
-https://conda.anaconda.org/conda-forge/linux-64/libclang-16.0.3-default_h83cc7fd_0.conda#5b597bfd98734dd4d0d907656a7ea9d1
+https://conda.anaconda.org/conda-forge/linux-64/libclang-16.0.6-default_h1cdf331_0.conda#e976871e132fe506da52c1240229246a
+https://conda.anaconda.org/conda-forge/linux-64/libxkbcommon-1.5.0-h5d7e998_3.conda#c91ea308d7bf70b62ddda568478aa03b
 https://conda.anaconda.org/conda-forge/noarch/livereload-2.6.3-pyh9f0ad1d_0.tar.bz2#b7190e3ec3eff52839434bf4698e2d62
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
 https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
-https://conda.anaconda.org/conda-forge/noarch/pep517-0.13.0-pyhd8ed1ab_0.tar.bz2#d94aa03d99d8adc9898f783eba0d84d2
+https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
 https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
-https://conda.anaconda.org/conda-forge/linux-64/pillow-9.5.0-py38h961100d_0.conda#3d5804d43c160c35d4eb04036f1f23b7
+https://conda.anaconda.org/conda-forge/linux-64/pillow-9.5.0-py38h885162f_1.conda#0eec8a20a17f17ec9e0b6839be466866
 https://conda.anaconda.org/eradiate/noarch/pinttrs-23.2.0-py_0.tar.bz2#1aebe9fa813278f719fa8e31d8000452
 https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/noarch/portion-2.4.0-pyhd8ed1ab_0.conda#9d34bac22e169b41f4e34525a140c13b
-https://conda.anaconda.org/conda-forge/linux-64/pulseaudio-client-16.1-h5195f5e_3.conda#caeb3302ef1dc8b342b20c710a86f8a9
+https://conda.anaconda.org/conda-forge/linux-64/pulseaudio-client-16.1-hb77b528_4.conda#8f349ca16d30950aa00870484d9d30c4
 https://conda.anaconda.org/conda-forge/linux-64/pyerfa-2.0.0.3-py38h7e4f40d_0.conda#631de6b5c8aec9c8ae2dcc596f8d2f72
+https://conda.anaconda.org/conda-forge/noarch/pyproject_hooks-1.0.0-pyhd8ed1ab_0.conda#21de50391d584eb7f4441b9de1ad773f
+https://conda.anaconda.org/conda-forge/noarch/pytest-7.3.2-pyhd8ed1ab_1.conda#f2465696f4396245eca4613f6e924796
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
-https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.17.24-py38h01eb140_0.conda#f9325f82900208075ad1f940e16652d9
+https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.17.32-py38h01eb140_0.conda#c92cc8efb1341f90ea5f51f576480580
 https://conda.anaconda.org/conda-forge/linux-64/sip-6.7.9-py38h17151c0_0.conda#6a54fd42b71a8b1c5f9c4a691270cdf1
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyh41d4057_0.conda#3788984d535770cad699efaeb6cb3037
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.65.0-pyhd8ed1ab_1.conda#ed792aff3acb977d09c7013358097f83
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.5.0-hd8ed1ab_0.conda#b3c594fde1a80a1fc3eb9cc4a5dfe392
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.3-hd8ed1ab_0.conda#3876f650ed7d0f95d70fa4b647621909
 https://conda.anaconda.org/conda-forge/linux-64/argon2-cffi-bindings-21.2.0-py38h0a891b7_3.tar.bz2#efcaa056d265a3138d2038a4b6b68791
-https://conda.anaconda.org/conda-forge/linux-64/astropy-5.2.2-py38h07e1bb6_0.conda#9cc8abe77be2118eb5b0c5c5d745f187
+https://conda.anaconda.org/conda-forge/linux-64/astropy-5.0.6-py38h07e1bb6_0.conda#0fcc655ae90038f1f66db3e3046d6c51
 https://conda.anaconda.org/conda-forge/linux-64/brotlipy-0.7.0-py38h0a891b7_1005.tar.bz2#e99e08812dfff30fdd17b3f8838e2759
-https://conda.anaconda.org/conda-forge/noarch/build-0.7.0-pyhd8ed1ab_0.tar.bz2#add7f31586d03678695b32b78a1337a1
-https://conda.anaconda.org/conda-forge/linux-64/cryptography-40.0.2-py38h3d167d9_0.conda#5443d5da3591c818482757981424c5b4
-https://conda.anaconda.org/conda-forge/linux-64/gstreamer-1.22.0-h25f0c4b_2.conda#461541cb1b387c2a28ab6217f3d38502
-https://conda.anaconda.org/conda-forge/linux-64/harfbuzz-6.0.0-h3ff4399_1.conda#73d2c2d25fdcec40c24929bab9f44831
+https://conda.anaconda.org/conda-forge/linux-64/cryptography-41.0.1-py38hcdda232_0.conda#8dc6f3a9342a870c3c927927e86aa4ad
+https://conda.anaconda.org/conda-forge/noarch/gitpython-3.1.31-pyhd8ed1ab_0.conda#f6e6b482110246a81c3f03e81c68752d
+https://conda.anaconda.org/conda-forge/linux-64/gstreamer-1.22.3-h977cf35_1.conda#410ed3b168e5a139d12ebaf4143072cd
+https://conda.anaconda.org/conda-forge/linux-64/harfbuzz-7.3.0-hdb3a94d_0.conda#765bc76c0dfaf24ff9d8a2935b2510df
 https://conda.anaconda.org/conda-forge/noarch/importlib-resources-5.12.0-pyhd8ed1ab_0.conda#3544c818f0720c89eb16ae6940ab440b
-https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.6.0-hd8ed1ab_0.conda#3cbc9615f10a3d471532b83e4250b971
+https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.7.0-hd8ed1ab_0.conda#27a4cec373ec84d1c1aa02a1e37f8eaf
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
-https://conda.anaconda.org/conda-forge/linux-64/libnetcdf-4.9.2-nompi_hdf9a29f_104.conda#283aeeef04e2a01445156c9c2d5c4fa0
-https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.3.5-pyhd8ed1ab_0.conda#9eeb66a24c8f6d950eb55a9f1128da20
+https://conda.anaconda.org/conda-forge/linux-64/libnetcdf-4.9.2-nompi_h0f3d0bb_105.conda#b5d412441b84305460e9df8a016a3392
+https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.4.0-pyhd8ed1ab_0.conda#6c5358a10873a15398b6f15f60cb5e1f
 https://conda.anaconda.org/conda-forge/linux-64/pandas-1.5.3-py38hdc8b05c_1.conda#c944b033a2126e7f714a7ecaecb22011
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.5.0-pyhd8ed1ab_0.conda#6c36f1c42dd0069b7f23acc74f19be46
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.6.0-pyhd8ed1ab_0.conda#741384b21c1b512617f4ee4ea8457c5d
 https://conda.anaconda.org/conda-forge/noarch/pybtex-0.24.0-pyhd8ed1ab_2.tar.bz2#2099b86a7399c44c0c61cdb6de6915ba
-https://conda.anaconda.org/conda-forge/linux-64/pydantic-1.10.7-py38h1de0b5d_0.conda#a373b13bc8a7336148a073e1de3d16d4
+https://conda.anaconda.org/conda-forge/linux-64/pydantic-1.10.9-py38h01eb140_0.conda#2d8a27b52507d0ba49c938005465b5e3
 https://conda.anaconda.org/conda-forge/linux-64/pyqt5-sip-12.11.0-py38h8dc9893_3.conda#7bb0328b4a0f857aeb432426b9a5f908
-https://conda.anaconda.org/conda-forge/noarch/rich-13.3.5-pyhd8ed1ab_0.conda#2e40a02ad28e34f26cee2a72042843db
+https://conda.anaconda.org/conda-forge/noarch/pytest-metadata-3.0.0-pyhd8ed1ab_1.conda#8bdcc0f401561213821bf67513abeeff
+https://conda.anaconda.org/conda-forge/noarch/python-build-0.10.0-pyhd8ed1ab_1.conda#0ab47ce574f6a8bcb9f2076436e7fedb
+https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda#f993baacc175e83fafd6b846e9c4c8a2
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
-https://conda.anaconda.org/conda-forge/linux-64/gst-plugins-base-1.22.0-h4243ec0_2.conda#0d0c6604c8ac4ad5e51efa7bb58da05c
-https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.3.0-py38h578d9bd_0.conda#d75b783a348cf33c6d3d75480300fecd
+https://conda.anaconda.org/conda-forge/linux-64/gst-plugins-base-1.22.3-h938bd60_1.conda#1f317eb7f00db75f4112a07476345376
+https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda#58ca2d50c3b27b86fd7df62eaadbf9a9
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
 https://conda.anaconda.org/conda-forge/linux-64/matplotlib-base-3.7.1-py38hd6c3c57_0.conda#3b8ba76acae09fbd4b2247c4ee4c0324
-https://conda.anaconda.org/conda-forge/linux-64/netcdf4-1.6.3-nompi_py38hd31e641_102.conda#1631559ac87f3f0742a8abd0ecd32e2d
-https://conda.anaconda.org/conda-forge/noarch/pip-tools-6.13.0-pyhd8ed1ab_0.conda#e05241917486ee034d848522161790b3
+https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
+https://conda.anaconda.org/conda-forge/linux-64/netcdf4-1.6.4-nompi_py38hdfa7aa7_100.conda#ce30178fb90d4509c3fda5b572124200
+https://conda.anaconda.org/conda-forge/noarch/pip-tools-6.13.0-pyhd8ed1ab_1.conda#566e41c99730f1124d6948ab8fe1c18d
 https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
 https://conda.anaconda.org/conda-forge/linux-64/pybtex-docutils-1.0.2-py38h578d9bd_2.tar.bz2#178c840a19be1a4c809798a73b285d27
-https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.1.1-pyhd8ed1ab_0.conda#0b34aa3ab7e7ccb1765a03dd9ed29938
+https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.2.0-pyhd8ed1ab_1.conda#34f7d568bf59d18e3fef8c405cbece21
+https://conda.anaconda.org/conda-forge/noarch/pytest-json-report-1.5.0-pyhd8ed1ab_0.tar.bz2#837e335fa428cf7c784ee2e80594506c
 https://conda.anaconda.org/conda-forge/linux-64/secretstorage-3.3.3-py38h578d9bd_1.tar.bz2#7ff0f00ee67fcbccbae548be59bfae77
 https://conda.anaconda.org/conda-forge/noarch/typer-0.9.0-pyhd8ed1ab_0.conda#5030a13b2fe5e143d5956d4943d3018f
-https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.23.0-pyhd8ed1ab_0.conda#a920e114c4c2ced2280e266da65ab5e6
+https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.23.1-pyhd8ed1ab_0.conda#838b85f656b078bdd882ef97978e7f40
 https://conda.anaconda.org/conda-forge/noarch/xarray-2023.1.0-pyhd8ed1ab_0.conda#c11eb03b6f77a0d22ae88c454c940f55
-https://conda.anaconda.org/conda-forge/linux-64/ipython-8.4.0-py38h578d9bd_0.tar.bz2#45164b6fd0616b2ed5217970c39865da
-https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda#58ca2d50c3b27b86fd7df62eaadbf9a9
 https://conda.anaconda.org/conda-forge/linux-64/keyring-23.13.1-py38h578d9bd_0.conda#713b14390d450db02fea6b0c0535d67a
-https://conda.anaconda.org/conda-forge/noarch/nbformat-5.8.0-pyhd8ed1ab_0.conda#1ca43103a08456b19222d93fd9d119ac
-https://conda.anaconda.org/conda-forge/linux-64/qt-main-5.15.8-h5c52f38_10.conda#0e898d8654a422310fe37bdf97a67a21
+https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
+https://conda.anaconda.org/conda-forge/linux-64/qt-main-5.15.8-h01ceb2d_12.conda#60fd4bdf187f88bac57cdc1a052f2811
 https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.15-pyhd8ed1ab_0.conda#27db656619a55d727eaf5a6ece3d2fd6
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.0-pyh210e3f2_0.conda#a9d13f9aee96fd4650928ac0302b0bf8
-https://conda.anaconda.org/conda-forge/noarch/nbclient-0.7.4-pyhd8ed1ab_0.conda#f7aa15f77d29b11caa1df1eb15383c59
+https://conda.anaconda.org/conda-forge/noarch/ipython-8.12.0-pyh41d4057_0.conda#e89d0c5836e45f9e6a66c5c24fc9ef35
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.6.0-pyhd8ed1ab_0.conda#879782bde4bbdb4c7b5d4054504a20d5
 https://conda.anaconda.org/conda-forge/linux-64/pyqt-5.15.7-py38ha0d8c90_3.conda#e965dc172d67920d058ac2b3a0e27565
-https://conda.anaconda.org/conda-forge/noarch/requests-2.29.0-pyhd8ed1ab_0.conda#5fa992d972fbccfc069161805122cb8d
-https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.12.11-pyhd8ed1ab_1.conda#e8f0410e0aa03342304357c5cc3bb75d
+https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
+https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.13.0-pyhd8ed1ab_0.conda#9f0b2eb5f5dd2cec36d5342a80adfec0
 https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.3-pyhd8ed1ab_0.tar.bz2#c99ae3abf501990769047b4b40a98f17
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.1-pyh210e3f2_0.conda#4b57b688e22d094d1479a35543c18e93
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.6.0-pyhd8ed1ab_0.conda#39fd52b0fcb2fb52bac47a1419bf09bd
 https://conda.anaconda.org/conda-forge/linux-64/matplotlib-3.7.1-py38h578d9bd_0.conda#50ff9e0a3dd459a0ca365741072bf9a2
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.4.0-pyhd8ed1ab_0.conda#4456e6030a8309bdad57569b0170b6a3
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.6.0-pyhd8ed1ab_0.conda#e8172ca42f2869bb90185c9356899e81
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.7.0-pyha770c72_3.conda#5936894aade8240c867d292aa0d980c6
 https://conda.anaconda.org/conda-forge/noarch/sphinx-5.0.0-pyh6c4a22f_1.tar.bz2#a7cc4b9c94548ff9a19b368f975e5404
 https://conda.anaconda.org/conda-forge/noarch/autodocsumm-0.2.11-pyhd8ed1ab_0.conda#547c48372c97c463c93af86d7f2c868c
-https://conda.anaconda.org/conda-forge/noarch/cachecontrol-with-filecache-0.12.11-pyhd8ed1ab_1.conda#9df660456c0076d27b802448f7ede78f
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.5.0-pyhd8ed1ab_0.conda#7fa3bd3d8dee42934f63711e9fbe959a
-https://conda.anaconda.org/conda-forge/noarch/myst-parser-1.0.0-pyhd8ed1ab_0.conda#e559708feb0aed1ae24c518e569ea3eb
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.4.0-pyhd8ed1ab_0.conda#127c702e1b1eff595be82bc6a78cfce0
+https://conda.anaconda.org/conda-forge/noarch/cachecontrol-with-filecache-0.13.0-pyhd8ed1ab_0.conda#3fd3d55ea862cc0736ac1cce6f44c2d1
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
+https://conda.anaconda.org/conda-forge/noarch/jupyter-lsp-2.2.0-pyhd8ed1ab_0.conda#38589f4104d11f2a59ff01a9f4e3bfb3
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.23.0-pyhd8ed1ab_0.conda#942aa06b962c7e507884c6fbeb4d1f7d
+https://conda.anaconda.org/conda-forge/noarch/myst-parser-0.18.1-pyhd8ed1ab_0.tar.bz2#bcfdf5c7d8bf5c6f6be7b4c66fff2eca
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.6.0-pyhd8ed1ab_0.conda#59976ee8df1c6f82c4aa94b5fd6b745e
+https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
 https://conda.anaconda.org/conda-forge/noarch/pydata-sphinx-theme-0.13.3-pyhd8ed1ab_0.conda#07aca5f2dea315dcc16680d6891e9056
-https://conda.anaconda.org/conda-forge/linux-64/scipy-1.10.1-py38h59f1b5f_1.conda#402ed4afcc5b82b8cebc9120fa523015
+https://conda.anaconda.org/conda-forge/linux-64/scipy-1.10.1-py38h59b608b_3.conda#2f2a57462fcfbc67dfdbb0de6f7484c2
 https://conda.anaconda.org/conda-forge/noarch/sphinx-autobuild-2021.3.14-pyhd8ed1ab_0.tar.bz2#1909f784dc37b4ab97afe2c95aeeabaa
 https://conda.anaconda.org/conda-forge/noarch/sphinx-copybutton-0.5.2-pyhd8ed1ab_0.conda#ac832cc43adc79118cf6e23f1f9b8995
-https://conda.anaconda.org/conda-forge/noarch/sphinx-design-0.4.1-pyhd8ed1ab_0.conda#14a64286fe896fe7e1a485fc91ccd022
+https://conda.anaconda.org/conda-forge/noarch/sphinx-design-0.4.1-pyhd8ed1ab_1.conda#c6b2e7903121c3210462a0866a561993
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-bibtex-2.5.0-pyhd8ed1ab_0.tar.bz2#b2e5c9aece936ebf9f26abdf71ddd74b
-https://conda.anaconda.org/conda-forge/noarch/conda-lock-1.4.0-pyhd8ed1ab_2.conda#e9ecdfe3e7d4f76d67afd65b02a621a0
+https://conda.anaconda.org/conda-forge/noarch/conda-lock-2.1.0-pyhd8ed1ab_0.conda#1e07afcf3d3e371fc3a3681fe9b78e90
 https://conda.anaconda.org/conda-forge/noarch/iapws-1.5.3-pyhd8ed1ab_0.tar.bz2#c5cad28f7c667df1910c3e9f8213c5eb
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.22.1-pyhd8ed1ab_0.conda#fc7172a6742a7c3c4331ddd7ed463ffc
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.4.0-pyhd8ed1ab_0.conda#a86727968b41c20dd3d73b91632e77dc
-https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.0.2-pyhd8ed1ab_0.conda#8e102bf37f10dd49c248910450242a19
+https://conda.anaconda.org/conda-forge/noarch/nbsphinx-0.9.2-pyhd8ed1ab_0.conda#d1212b423fdd10d2da59601385561ff7
 https://conda.anaconda.org/conda-forge/noarch/patsy-0.5.3-pyhd8ed1ab_0.tar.bz2#50ef6b29b1fb0768ca82c5aeb4fb2d96
 https://conda.anaconda.org/conda-forge/noarch/seaborn-base-0.12.2-pyhd8ed1ab_0.conda#cf88f3a1c11536bc3c10c14ad00ccc42
 https://conda.anaconda.org/conda-forge/noarch/sphinx-book-theme-1.0.1-pyhd8ed1ab_0.conda#1ef419576de2c51b6e3a5a393eb35cda
-https://conda.anaconda.org/conda-forge/noarch/nbclassic-1.0.0-pyhb4ecaf3_1.conda#a0be31e9bd84d6eae87cdbf74c56b90b
-https://conda.anaconda.org/conda-forge/noarch/nbsphinx-0.9.1-pyhd8ed1ab_0.conda#a0b8b3d9eb22da29279a90883dcd5962
 https://conda.anaconda.org/conda-forge/linux-64/statsmodels-0.14.0-py38h31356c5_1.conda#46fdc57a392e7e494ba579eed5e153a0
-https://conda.anaconda.org/conda-forge/noarch/notebook-6.5.4-pyha770c72_0.conda#ec4ce3ce0a55ce21b6f5b86049b97af9
 https://conda.anaconda.org/conda-forge/noarch/seaborn-0.12.2-hd8ed1ab_0.conda#50847a47c07812f88581081c620f5160
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab-3.5.3-pyhd8ed1ab_0.conda#69f71bc3d176b3ad3d9564a32bd049b8
```

### Comparing `eradiate-0.23.2rc1/requirements/environment-optional.yml` & `eradiate-0.23.2rc2/requirements/conda/environment-docs.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,38 @@
 channels:
   - eradiate
   - conda-forge
   - defaults
 dependencies:
+  # default
   - python=3.8
+  # docs
+  - autodocsumm
+  - myst-parser
+  - nbsphinx>=0.9.0
+  - sphinx
+  - sphinx-autobuild
+  - sphinx-book-theme>=1.0
+  - sphinx-copybutton
+  - sphinx-design
+  - sphinxcontrib-bibtex>=2.0
   # main
   - aenum
   - attrs>=22.2
   - click
   - dessinemoi>=23.1.0
   - environ-config
   - lazy_loader>=0.1
   - matplotlib>=3.3
   - netcdf4
   - numpy
   - pint
   - pinttrs>=23.2.0
-  - portion
   - pooch
+  - portion
   - rich
   - ruamel.yaml
   - scipy
   - shellingham!=1.5.1
   - tqdm
   - typer>=0.9.0
   - xarray>=0.19,!=0.20.*
-  # recommended
-  - aabbtree
-  - astropy
-  - iapws
-  - ipython
-  - ipywidgets
-  - jupyterlab
-  - python-dateutil
-  - seaborn
-  # docs
-  - autodocsumm
-  - myst-parser
-  - nbsphinx>=0.9.0
-  - sphinx-book-theme>=1.0
-  - sphinx
-  - sphinxcontrib-bibtex>=2.0
-  - sphinx-autobuild
-  - sphinx-copybutton
-  - sphinx-design
-  # dev
-  - conda-lock>=1.4
-  - pip>=22
-  - pip-tools>=6.5
-  - setuptools>=61
-  # optional
-  - pip
-  - pip:
-    - eradiate_mitsuba==0.0.1rc10
```

### Comparing `eradiate-0.23.2rc1/requirements/environment-osx-64.lock` & `eradiate-0.23.2rc2/requirements/conda/environment-dev-osx-64.lock`

 * *Files 3% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 # Generated by conda-lock.
 # platform: osx-64
-# input_hash: d9247051d05316398f35c8ce4621ac229570f18ff5cd48d8edcae2ab4587ce46
+# input_hash: bf11f624e722c74ec0e342583ae0fcb21524c22ae8ca653349f3b25602fab72a
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h0d85af4_4.tar.bz2#37edc4e6304ca87316e160f5ca0bd1b5
-https://conda.anaconda.org/conda-forge/osx-64/c-ares-1.18.1-h0d85af4_0.tar.bz2#00b3e98a61e6430808fe7a2534681f28
+https://conda.anaconda.org/conda-forge/osx-64/c-ares-1.19.1-h0dc2134_0.conda#b3e62631b4e1b9801477523ce1d6f355
 https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2023.5.7-h8857fd0_0.conda#b704e4b79ba0d887c4870b7b09d6a4df
 https://conda.anaconda.org/conda-forge/osx-64/icu-72.1-h7336db1_0.conda#c9689510a50a4bb2ae978421671a125e
 https://conda.anaconda.org/conda-forge/osx-64/libbrotlicommon-1.0.9-hb7f2c08_8.tar.bz2#37157d273eaf3bc7d6862104161d9ec9
-https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.3-hd57cbcb_0.conda#a18d8a09f5f3037723862e5ffd3d8efa
+https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.6-hd57cbcb_0.conda#7d6972792161077908b62971802f289a
 https://conda.anaconda.org/conda-forge/osx-64/libdeflate-1.18-hac1461d_0.conda#3d131584456b277ce0871e6481fde49b
 https://conda.anaconda.org/conda-forge/osx-64/libev-4.33-haf1e3a3_1.tar.bz2#79dc2be110b2a3d1e97ec21f691c50ad
 https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2#ccb34fb14960ad8b125962d3d79b31a9
 https://conda.anaconda.org/conda-forge/osx-64/libiconv-1.17-hac89ed1_0.tar.bz2#691d103d11180486154af49c037b7ed9
 https://conda.anaconda.org/conda-forge/osx-64/libjpeg-turbo-2.1.5.1-hb7f2c08_0.conda#d7309a152b9b79799063b8bb47e34a3a
 https://conda.anaconda.org/conda-forge/osx-64/libsodium-1.0.18-hbcb3906_1.tar.bz2#24632c09ed931af617fe6d5292919cab
 https://conda.anaconda.org/conda-forge/osx-64/libwebp-base-1.3.0-hb7f2c08_0.conda#18981e4c840126d6118d8952485fea51
-https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-hfd90126_4.tar.bz2#35eb3fce8d51ed3c1fd4122bad48250b
-https://conda.anaconda.org/conda-forge/osx-64/llvm-openmp-16.0.3-hff08bdf_0.conda#4493294698b915041f100126923769e3
-https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.3-h96cf925_1.tar.bz2#76217ebfbb163ff2770a261f955a5861
-https://conda.anaconda.org/conda-forge/osx-64/pandoc-2.19.2-h694c41f_2.conda#de3014568ff5004048dd09ba73990430
+https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda#4a3ad23f6e16f99c04e166767193d700
+https://conda.anaconda.org/conda-forge/osx-64/llvm-openmp-16.0.6-hff08bdf_0.conda#39a5227d906f75102bf8586741690128
+https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4-hf0c8a7f_0.conda#c3dbae2411164d9b02c69090a9a91857
 https://conda.anaconda.org/conda-forge/osx-64/pthread-stubs-0.4-hc929b4f_1001.tar.bz2#addd19059de62181cd11ae8f4ef26084
 https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.8-3_cp38.conda#ff192f59f7fe23555612030493a079f8
-https://conda.anaconda.org/conda-forge/osx-64/xorg-libxau-1.0.9-h35c211d_0.tar.bz2#c5049997b2e98edfbcdd294582f66281
+https://conda.anaconda.org/conda-forge/osx-64/xorg-libxau-1.0.11-h0dc2134_0.conda#9566b4c29274125b0266d0177b5eb97b
 https://conda.anaconda.org/conda-forge/osx-64/xorg-libxdmcp-1.1.3-h35c211d_0.tar.bz2#86ac76d6bf1cbb9621943eb3bd9ae36e
 https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2#a72f9d4ea13d55d745ff1ed594747f10
 https://conda.anaconda.org/conda-forge/osx-64/yaml-0.2.5-h0d85af4_2.tar.bz2#d7e08fcf8259d742156188e8762b4d20
 https://conda.anaconda.org/conda-forge/osx-64/hdf4-4.2.15-h9804679_6.conda#c13d8841112ba7f5931d1d60631394f3
 https://conda.anaconda.org/conda-forge/osx-64/lerc-4.0.0-hb486fe8_0.tar.bz2#f9d6a4c82889d5ecedec1d90eb673c55
 https://conda.anaconda.org/conda-forge/osx-64/libaec-1.0.6-hf0c8a7f_1.conda#7c0f82f435ab4c48d65dc9b28db2ad9e
 https://conda.anaconda.org/conda-forge/osx-64/libbrotlidec-1.0.9-hb7f2c08_8.tar.bz2#7f952a036d9014b4dab96c6ea0f8c2a7
 https://conda.anaconda.org/conda-forge/osx-64/libbrotlienc-1.0.9-hb7f2c08_8.tar.bz2#b36a3bfe866d9127f25f286506982166
 https://conda.anaconda.org/conda-forge/osx-64/libedit-3.1.20191231-h0678c8f_2.tar.bz2#6016a8a1d0e63cac3de2c352cd40208b
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran5-12.2.0-he409387_31.conda#5a544130e584b1f204ac896ff071d5b3
 https://conda.anaconda.org/conda-forge/osx-64/libpng-1.6.39-ha978bb4_0.conda#35e4928794c5391aec14ffdf1deaaee5
-https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.41.2-h58db7d2_1.conda#208f91c5db1ba9f80d32cffde56f4a8f
-https://conda.anaconda.org/conda-forge/osx-64/libxcb-1.13-h0d85af4_1004.tar.bz2#eb7860935e14aec936065cbc21a1a962
-https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.10.4-h554bb67_0.conda#003fef825b16c26c44d97e115bf8840e
+https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.42.0-h58db7d2_0.conda#a7d3b44b7b0c9901ac7813b7a0462893
+https://conda.anaconda.org/conda-forge/osx-64/libxcb-1.15-hb7f2c08_0.conda#5513f57e0238c87c12dffedbcc9c1a4a
+https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.11.4-hd95e348_0.conda#681f8dda25e73a830d774a37b9839c85
 https://conda.anaconda.org/conda-forge/osx-64/lz4-c-1.9.4-hf0c8a7f_0.conda#aa04f7143228308662696ac24023f991
-https://conda.anaconda.org/conda-forge/osx-64/openssl-3.1.0-h8a1eda9_3.conda#3761d72a2a68de6fd1c0a2d038864785
+https://conda.anaconda.org/conda-forge/osx-64/openssl-3.1.1-h8a1eda9_1.conda#c7822d6ee74e34af1fd74365cfd18983
+https://conda.anaconda.org/conda-forge/osx-64/pandoc-3.1.3-h9d075a6_0.conda#e86a3d5c966a09b6129354114483f7a7
 https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda#f17f77f2acf4d344734bda76829ce14e
 https://conda.anaconda.org/conda-forge/osx-64/snappy-1.1.10-h225ccf5_0.conda#4320a8781f14cd959689b86e349f3b73
 https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.12-h5dbffcc_0.tar.bz2#8e9480d9c47061db2ed1b4ecce519a7f
 https://conda.anaconda.org/conda-forge/osx-64/zeromq-4.3.4-he49afe7_1.tar.bz2#1972d732b123ed04b60fd21e94f0b178
 https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.2-hbc0c0cd_6.conda#40a188783d3c425bdccc9ae9104acbb8
-https://conda.anaconda.org/conda-forge/osx-64/blosc-1.21.2-hebb52c4_0.conda#2e726e782e57ba3e70f2e85891377cd5
+https://conda.anaconda.org/conda-forge/osx-64/blosc-1.21.4-heccf04b_0.conda#02e92eb72b9ae4c1745b95d03a9c949e
 https://conda.anaconda.org/conda-forge/osx-64/brotli-bin-1.0.9-hb7f2c08_8.tar.bz2#aac5ad0d8f747ef7f871508146df75d9
 https://conda.anaconda.org/conda-forge/osx-64/freetype-2.12.1-h3f81eb7_1.conda#852224ea3e8991a8342228eab274840e
 https://conda.anaconda.org/conda-forge/osx-64/krb5-1.20.1-h049b76e_0.conda#db11fa2968ef0837288fe2d7f5b77a50
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran-5.0.0-11_3_0_h97931a8_31.conda#97451338600bd9c5b535eb224ef6c471
 https://conda.anaconda.org/conda-forge/osx-64/libnghttp2-1.52.0-he2ab024_0.conda#12ac7d100bf260263e30a019517f42a2
-https://conda.anaconda.org/conda-forge/osx-64/libssh2-1.10.0-h47af595_3.tar.bz2#5a28624eeb7812b585b9e2d75f846ba2
-https://conda.anaconda.org/conda-forge/osx-64/libtiff-4.5.0-hedf67fa_6.conda#800b810c1aa3eb4a08106698441871bb
+https://conda.anaconda.org/conda-forge/osx-64/libssh2-1.11.0-hd019ec5_0.conda#ca3a72efba692c59a90d4b9fc0dfe774
+https://conda.anaconda.org/conda-forge/osx-64/libtiff-4.5.1-hf955e92_0.conda#56523ed556e3a44c0fd55bcf17045892
 https://conda.anaconda.org/conda-forge/osx-64/libzip-1.9.2-h6db710c_1.tar.bz2#ce732d37e479919f3d22b1ccdeb858ac
-https://conda.anaconda.org/conda-forge/osx-64/python-3.8.16-hf9b03c3_1_cpython.conda#96d23d997c18a90efde924d9ca6dd5b3
+https://conda.anaconda.org/conda-forge/osx-64/python-3.8.17-hf9b03c3_0_cpython.conda#f613b663d3829f325b4ffb626bf612b6
 https://conda.anaconda.org/eradiate/noarch/aabbtree-2.8.0-py_0.tar.bz2#647bcce5f0af4974e507591d5420486b
 https://conda.anaconda.org/conda-forge/noarch/aenum-3.1.12-pyhd8ed1ab_0.conda#602716538da00b2ca3cc85c4d35c0245
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.13-pyhd8ed1ab_0.conda#06006184e203b61d3525f90de394471e
 https://conda.anaconda.org/conda-forge/noarch/appdirs-1.4.4-pyh9f0ad1d_0.tar.bz2#5f095bc6454094e96f146491fd03633b
 https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.3-pyhd8ed1ab_0.tar.bz2#54ac328d703bff191256ffa1183126d1
 https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
@@ -72,199 +72,211 @@
 https://conda.anaconda.org/conda-forge/noarch/dataclasses-0.8-pyhc8e2a94_3.tar.bz2#a362b2124b06aad102e2ee4581acee7d
 https://conda.anaconda.org/conda-forge/osx-64/debugpy-1.6.7-py38h4cd09af_0.conda#32626ffd5cd7eaad3036d7dca808ddc7
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.6-pyhd8ed1ab_0.tar.bz2#b65b4d50dbd2d50fa0aeac367ec9eed7
 https://conda.anaconda.org/conda-forge/osx-64/docutils-0.16-py38h50d1736_3.tar.bz2#935f17c6604af240ea1c31c1d3292293
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
-https://conda.anaconda.org/conda-forge/noarch/filelock-3.12.0-pyhd8ed1ab_0.conda#650f18a56f366dbf419c15b543592c2d
-https://conda.anaconda.org/conda-forge/noarch/flit-core-3.8.0-pyhd8ed1ab_0.tar.bz2#6d5e56de2e65da7aa35fd10131226efa
+https://conda.anaconda.org/conda-forge/noarch/filelock-3.12.2-pyhd8ed1ab_0.conda#53522ec72e6adae42bd373ef58357230
+https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
-https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
+https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_0.conda#1f39269ab88d1342c3e32935759e606a
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
 https://conda.anaconda.org/conda-forge/osx-64/kiwisolver-1.4.4-py38h98b9b1b_1.tar.bz2#c11eff21a36bc5809b8e23a05ee71df8
 https://conda.anaconda.org/conda-forge/noarch/lazy_loader-0.2-pyhd8ed1ab_0.conda#d060d017720c9882c4eca0544a4a0592
 https://conda.anaconda.org/conda-forge/osx-64/lcms2-2.15-h2dcdeff_1.conda#f1df9b0c2d9fbe985e62f4b24773a9e4
-https://conda.anaconda.org/conda-forge/osx-64/libcurl-8.0.1-h1fead75_0.conda#8f9160d09c01592c4654be05fff5b9cc
-https://conda.anaconda.org/conda-forge/osx-64/libopenblas-0.3.21-openmp_h429af6e_3.tar.bz2#968c46aa7f4032c3f3873f3452ed4c34
+https://conda.anaconda.org/conda-forge/osx-64/libcurl-8.1.2-hbee3ae8_0.conda#d51e337da844262f9033c9a26452520f
+https://conda.anaconda.org/conda-forge/osx-64/libopenblas-0.3.23-openmp_h429af6e_0.conda#7000a828e29608e4f57e662b5502d2c9
 https://conda.anaconda.org/conda-forge/noarch/lockfile-0.12.2-py_1.tar.bz2#c104d98e09c47519950cffb8dd5b4f10
-https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.2-py38hef030d1_0.conda#011ae40b08362bc2b0b549f4fc0bd79f
+https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.3-py38hcafd530_0.conda#e8ee9933dc3749c889baccb1c4b4f014
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
-https://conda.anaconda.org/conda-forge/noarch/mistune-2.0.5-pyhd8ed1ab_0.conda#61a07195cfc935f1c1901d8ecf4af441
+https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
 https://conda.anaconda.org/conda-forge/noarch/more-itertools-9.1.0-pyhd8ed1ab_0.conda#1698a717f83cfecf644a877c174c84bd
 https://conda.anaconda.org/conda-forge/osx-64/msgpack-python-1.0.5-py38h98b9b1b_0.conda#c8dc8bd685921ea63ba672f4ae018f06
 https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2#2ba8498c1018c1e9c61eb99b973dfe19
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
+https://conda.anaconda.org/conda-forge/noarch/networkx-3.1-pyhd8ed1ab_0.conda#254f787d5068bc89f578bf63893ce8b4
 https://conda.anaconda.org/conda-forge/osx-64/openjpeg-2.5.0-h13ac156_2.conda#299a29af9ac9f550ad459d655739280b
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
 https://conda.anaconda.org/conda-forge/noarch/pastel-0.2.1-pyhd8ed1ab_0.tar.bz2#a4eea5bff523f26442405bc5d1f52adb
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pint-0.21-pyhd8ed1ab_0.conda#8d7b829e37d78447569c180f9d827005
 https://conda.anaconda.org/conda-forge/noarch/pkginfo-1.9.6-pyhd8ed1ab_0.conda#be1e9f1c65a1ed0f2ae9352fec99db64
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
-https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.16.0-pyhd8ed1ab_0.conda#8efaddc1c8b8ce262c4d1a7c6571c799
+https://conda.anaconda.org/conda-forge/noarch/pluggy-1.0.0-pyhd8ed1ab_5.tar.bz2#7d301a0d25f424d96175f810935f0da9
+https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda#95c5be3c7cbd872509d16c216617fdab
 https://conda.anaconda.org/conda-forge/osx-64/psutil-5.9.5-py38hef030d1_0.conda#20b4cc7adae881327b943c883be6335e
 https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
 https://conda.anaconda.org/conda-forge/noarch/pylev-1.4.0-pyhd8ed1ab_0.tar.bz2#edf8651c4379d9d1495ad6229622d150
-https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.0.9-pyhd8ed1ab_0.tar.bz2#e8fbc1b54b25f4b08281467bc13b70cc
+https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.0-pyhd8ed1ab_0.conda#d3ed087d1f7f8f5590e8e87b57a8ce64
 https://conda.anaconda.org/conda-forge/osx-64/pyrsistent-0.19.3-py38hef030d1_0.conda#01ca11f08679d88fc881a19902a0a008
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
-https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.16.3-pyhd8ed1ab_0.conda#7aa330a4d88b7ab891a42c39d5d2e742
+https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
 https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0-py38hef030d1_5.tar.bz2#e27d698dc29c6d5b49f1385bcd1d50f9
-https://conda.anaconda.org/conda-forge/osx-64/pyzmq-25.0.2-py38h0b711fd_0.conda#6aafe8de24c304eabdacbabfe290d9c7
+https://conda.anaconda.org/conda-forge/osx-64/pyzmq-25.1.0-py38h3b70857_0.conda#a48761bc98b3bc22d209e9bb2f3dc5c1
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
 https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml.clib-0.2.7-py38hef030d1_1.conda#9a8e866b0680b61b2e988b18a1eaecae
 https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
 https://conda.anaconda.org/conda-forge/noarch/shellingham-1.4.0-pyh44b312d_0.tar.bz2#437655338696f9d0dfdb0a024e66b255
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
+https://conda.anaconda.org/conda-forge/noarch/smmap-3.0.5-pyh44b312d_0.tar.bz2#3a8dc70789709aa315325d5df06fb7e4
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/sortedcontainers-2.4.0-pyhd8ed1ab_0.tar.bz2#6d6552722448103793743dabfbda532d
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.4-pyhd8ed1ab_0.conda#5a31a7d564f551d0e6dff52fd8cb5b16
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.2-py_0.tar.bz2#68e01cac9d38d0e717cd5c87bc3d2cc9
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-htmlhelp-2.0.1-pyhd8ed1ab_0.conda#6c8c4d6eb2325e59290ac6dbbeacd5f0
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jsmath-1.0.1-py_0.tar.bz2#67cd9d9c0382d37479b4d306c369a2d4
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-qthelp-1.0.3-py_0.tar.bz2#d01180388e6d1838c3e1ad029590aa7a
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-serializinghtml-1.1.5-pyhd8ed1ab_2.tar.bz2#9ff55a0901cf952f05c654394de76bf7
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.11.8-pyha770c72_0.conda#75838e8556166263a82038b51d01d5f1
 https://conda.anaconda.org/conda-forge/noarch/toolz-0.12.0-pyhd8ed1ab_0.tar.bz2#92facfec94bc02d6ccf42e7173831a36
-https://conda.anaconda.org/conda-forge/osx-64/tornado-6.3-py38hef030d1_0.conda#dd70b29d191a538848c095bf49535d58
+https://conda.anaconda.org/conda-forge/osx-64/tornado-6.3.2-py38hcafd530_0.conda#afefcf665a5049b030efb084a51e3935
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.5.0-pyha770c72_0.conda#43e7d9e50261fb11deb76e17d8431aac
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.3-pyha770c72_0.conda#4a3014a4d107d15475d106b751c4e352
+https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/osx-64/unicodedata2-15.0.0-py38hef030d1_0.tar.bz2#51020c740c53f14657f6307b9eb23f85
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.5.1-pyhd8ed1ab_0.conda#2a914654b9ade742049dab13e29571c6
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.0-pyhd8ed1ab_0.conda#1dd6387a73d84e16b6f73de676bb4c36
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
 https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
 https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
 https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
-https://conda.anaconda.org/conda-forge/noarch/anyio-3.6.2-pyhd8ed1ab_0.tar.bz2#8ada050fa88f26916fc1e76e368a49fd
+https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.0-pyhd8ed1ab_1.conda#2b35a85d654a47aac8f34c1bb6de7142
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
+https://conda.anaconda.org/conda-forge/noarch/async-lru-2.0.2-pyhd8ed1ab_0.conda#41221f97a0c82e5a60b21716a3d7469c
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
 https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
 https://conda.anaconda.org/conda-forge/osx-64/cffi-1.15.1-py38hb368cf1_3.conda#a2b3ae2a1fd2aea0b4433d9e7fff8cf3
 https://conda.anaconda.org/conda-forge/noarch/click-default-group-1.2.2-pyhd8ed1ab_1.tar.bz2#72a46ffc25701c173932fd55cf0965d3
 https://conda.anaconda.org/conda-forge/noarch/clikit-0.6.2-pyhd8ed1ab_2.conda#02abb7b66b02e8b9f5a9b05454400087
 https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
-https://conda.anaconda.org/conda-forge/osx-64/curl-8.0.1-h1fead75_0.conda#bd841ebfa6236b55a0dce27c2f5e6171
+https://conda.anaconda.org/conda-forge/osx-64/curl-8.1.2-hbee3ae8_0.conda#6cc301a6c2ba26e29949818efdc133ca
 https://conda.anaconda.org/eradiate/noarch/dessinemoi-23.1.0-py_0.tar.bz2#490780e63e113a7dc444bd068e049bfe
 https://conda.anaconda.org/conda-forge/noarch/environ-config-22.1.0-pyhd8ed1ab_0.tar.bz2#a1103faffa0a877313c1fba776aa0fc0
-https://conda.anaconda.org/conda-forge/osx-64/fonttools-4.39.3-py38hef030d1_0.conda#5bf00768c337532c03aaf42239c008d2
+https://conda.anaconda.org/conda-forge/osx-64/fonttools-4.40.0-py38hcafd530_0.conda#b26b38c5f75e03e86cecf860ca9fb1cd
+https://conda.anaconda.org/conda-forge/noarch/gitdb-4.0.10-pyhd8ed1ab_0.conda#3706d2f3d7cb5dae600c833345a76132
 https://conda.anaconda.org/conda-forge/osx-64/hdf5-1.14.0-nompi_hbf0aa07_103.conda#90f50d124606a4e62628823b614a2f4c
 https://conda.anaconda.org/conda-forge/noarch/html5lib-1.1-pyh9f0ad1d_0.tar.bz2#b2355343d6315c892543200231d7154a
-https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.6.0-pyha770c72_0.conda#f91a5d5175fb7ff2a91952ec7da59cb9
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.7.0-pyha770c72_0.conda#ba3786c6846e46038fe60c785d46dc81
 https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
 https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.2.3-pyhd8ed1ab_0.tar.bz2#31e4a1506968d017229bdb64695013a1
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
 https://conda.anaconda.org/conda-forge/noarch/latexcodec-2.0.1-pyh9f0ad1d_0.tar.bz2#8d67904973263afd2985ba56aa2d6bb4
-https://conda.anaconda.org/conda-forge/osx-64/libblas-3.9.0-16_osx64_openblas.tar.bz2#644d63e9379867490b67bace400b2a0f
+https://conda.anaconda.org/conda-forge/osx-64/libblas-3.9.0-17_osx64_openblas.conda#65299527582e2449b05d27fcf8352125
 https://conda.anaconda.org/conda-forge/noarch/livereload-2.6.3-pyh9f0ad1d_0.tar.bz2#b7190e3ec3eff52839434bf4698e2d62
 https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-2.2.0-pyhd8ed1ab_0.conda#b2928a6c6d52d7e3562b4a59c3214e3a
 https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
-https://conda.anaconda.org/conda-forge/noarch/pep517-0.13.0-pyhd8ed1ab_0.tar.bz2#d94aa03d99d8adc9898f783eba0d84d2
+https://conda.anaconda.org/conda-forge/noarch/overrides-7.3.1-pyhd8ed1ab_0.tar.bz2#a5745ced46e69aa9754053ba061974ab
 https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
-https://conda.anaconda.org/conda-forge/osx-64/pillow-9.5.0-py38h3c5639a_0.conda#e0bac463141a239a8b6624d927aed567
+https://conda.anaconda.org/conda-forge/osx-64/pillow-9.5.0-py38h16710f9_1.conda#c5bf174a033ef668679cc80918422515
 https://conda.anaconda.org/eradiate/noarch/pinttrs-23.2.0-py_0.tar.bz2#1aebe9fa813278f719fa8e31d8000452
 https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
 https://conda.anaconda.org/conda-forge/noarch/portion-2.4.0-pyhd8ed1ab_0.conda#9d34bac22e169b41f4e34525a140c13b
-https://conda.anaconda.org/conda-forge/osx-64/pyobjc-core-9.1.1-py38h8f2a8f7_0.conda#e8cdf74d4a128a7bdd574d6c06b3b994
+https://conda.anaconda.org/conda-forge/osx-64/pyobjc-core-9.2-py38h095c2e5_0.conda#8dbb4798b2066b678d8da47734d1c763
+https://conda.anaconda.org/conda-forge/noarch/pyproject_hooks-1.0.0-pyhd8ed1ab_0.conda#21de50391d584eb7f4441b9de1ad773f
+https://conda.anaconda.org/conda-forge/noarch/pytest-7.3.2-pyhd8ed1ab_1.conda#f2465696f4396245eca4613f6e924796
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
-https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml-0.17.24-py38hcafd530_0.conda#6740db2ae9383c1cabb2da0a74dbd3f9
+https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml-0.17.32-py38hcafd530_0.conda#cb301e0b2b162330bc3b03fe51ea0d15
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyhd1c38e8_0.conda#046120b71d8896cb7faef78bfdbfee1e
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.65.0-pyhd8ed1ab_1.conda#ed792aff3acb977d09c7013358097f83
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.5.0-hd8ed1ab_0.conda#b3c594fde1a80a1fc3eb9cc4a5dfe392
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.3-hd8ed1ab_0.conda#3876f650ed7d0f95d70fa4b647621909
 https://conda.anaconda.org/conda-forge/osx-64/argon2-cffi-bindings-21.2.0-py38hef030d1_3.tar.bz2#fc1bc20add8eff07c367973bba25e8eb
 https://conda.anaconda.org/conda-forge/osx-64/brotlipy-0.7.0-py38hef030d1_1005.tar.bz2#2fa6826f6f94c847bf26709f2162a09c
-https://conda.anaconda.org/conda-forge/noarch/build-0.7.0-pyhd8ed1ab_0.tar.bz2#add7f31586d03678695b32b78a1337a1
-https://conda.anaconda.org/conda-forge/osx-64/cryptography-40.0.2-py38h4257468_0.conda#e60e91caecdb7719724e6e2124e4cffc
+https://conda.anaconda.org/conda-forge/osx-64/cryptography-41.0.1-py38he13da33_0.conda#845f16b2278f26769e23796d04636e06
+https://conda.anaconda.org/conda-forge/noarch/gitpython-3.1.31-pyhd8ed1ab_0.conda#f6e6b482110246a81c3f03e81c68752d
 https://conda.anaconda.org/conda-forge/noarch/importlib-resources-5.12.0-pyhd8ed1ab_0.conda#3544c818f0720c89eb16ae6940ab440b
-https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.6.0-hd8ed1ab_0.conda#3cbc9615f10a3d471532b83e4250b971
+https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.7.0-hd8ed1ab_0.conda#27a4cec373ec84d1c1aa02a1e37f8eaf
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
-https://conda.anaconda.org/conda-forge/osx-64/libcblas-3.9.0-16_osx64_openblas.tar.bz2#28592eab0f05bcf9969789e87f754e11
-https://conda.anaconda.org/conda-forge/osx-64/liblapack-3.9.0-16_osx64_openblas.tar.bz2#406ad426aade5578b90544cc2ed4a79b
-https://conda.anaconda.org/conda-forge/osx-64/libnetcdf-4.9.2-nompi_h4ab8a84_104.conda#36f19c95e1a5034b3b5a0b2b98676c50
-https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.3.5-pyhd8ed1ab_0.conda#9eeb66a24c8f6d950eb55a9f1128da20
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.5.0-pyhd8ed1ab_0.conda#6c36f1c42dd0069b7f23acc74f19be46
+https://conda.anaconda.org/conda-forge/osx-64/libcblas-3.9.0-17_osx64_openblas.conda#380151ca00704172b242a63701b7bf8a
+https://conda.anaconda.org/conda-forge/osx-64/liblapack-3.9.0-17_osx64_openblas.conda#6ab83532872bf3659613638589dd10af
+https://conda.anaconda.org/conda-forge/osx-64/libnetcdf-4.9.2-nompi_hf077d52_105.conda#64d626e024a284777458e2b315e9eb56
+https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.4.0-pyhd8ed1ab_0.conda#6c5358a10873a15398b6f15f60cb5e1f
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.6.0-pyhd8ed1ab_0.conda#741384b21c1b512617f4ee4ea8457c5d
 https://conda.anaconda.org/conda-forge/noarch/pybtex-0.24.0-pyhd8ed1ab_2.tar.bz2#2099b86a7399c44c0c61cdb6de6915ba
-https://conda.anaconda.org/conda-forge/osx-64/pydantic-1.10.7-py38hef030d1_0.conda#85de1c7f80b6614f1a96a5614d9e2da2
-https://conda.anaconda.org/conda-forge/osx-64/pyobjc-framework-cocoa-9.1.1-py38h8f2a8f7_0.conda#eaea41f1de16d95ce4de1fdd1b4bb295
-https://conda.anaconda.org/conda-forge/noarch/rich-13.3.5-pyhd8ed1ab_0.conda#2e40a02ad28e34f26cee2a72042843db
+https://conda.anaconda.org/conda-forge/osx-64/pydantic-1.10.9-py38hcafd530_0.conda#253819655b95aedbeddf0ff7fa26cf16
+https://conda.anaconda.org/conda-forge/osx-64/pyobjc-framework-cocoa-9.2-py38h095c2e5_0.conda#fa3e3307ff143e7a9e823ce7bbc916ad
+https://conda.anaconda.org/conda-forge/noarch/pytest-metadata-3.0.0-pyhd8ed1ab_1.conda#8bdcc0f401561213821bf67513abeeff
+https://conda.anaconda.org/conda-forge/noarch/python-build-0.10.0-pyhd8ed1ab_1.conda#0ab47ce574f6a8bcb9f2076436e7fedb
+https://conda.anaconda.org/conda-forge/noarch/rich-13.4.2-pyhd8ed1ab_0.conda#f993baacc175e83fafd6b846e9c4c8a2
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
-https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.3.0-py38h50d1736_0.conda#c342b82641ef032fa8b256eb4f0a5649
+https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.3.1-py38h50d1736_0.conda#03a3619e222793567b29b5966c2a821d
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
 https://conda.anaconda.org/conda-forge/osx-64/keyring-23.13.1-py38h50d1736_0.conda#7ba9ac4c5edbaddcffe213189e679b13
 https://conda.anaconda.org/conda-forge/osx-64/numpy-1.24.3-py38h9a4a08f_0.conda#5ff64b8133dea66865fe1bd35fb1d6d6
-https://conda.anaconda.org/conda-forge/noarch/pip-tools-6.13.0-pyhd8ed1ab_0.conda#e05241917486ee034d848522161790b3
+https://conda.anaconda.org/conda-forge/noarch/pip-tools-6.13.0-pyhd8ed1ab_1.conda#566e41c99730f1124d6948ab8fe1c18d
 https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
 https://conda.anaconda.org/conda-forge/osx-64/pybtex-docutils-1.0.2-py38h50d1736_2.tar.bz2#5650c819d7ae44ff91c456370f175706
-https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.1.1-pyhd8ed1ab_0.conda#0b34aa3ab7e7ccb1765a03dd9ed29938
+https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.2.0-pyhd8ed1ab_1.conda#34f7d568bf59d18e3fef8c405cbece21
+https://conda.anaconda.org/conda-forge/noarch/pytest-json-report-1.5.0-pyhd8ed1ab_0.tar.bz2#837e335fa428cf7c784ee2e80594506c
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyhd1c38e8_0.conda#2657c3de5371c571aef6678afb4aaadd
 https://conda.anaconda.org/conda-forge/noarch/typer-0.9.0-pyhd8ed1ab_0.conda#5030a13b2fe5e143d5956d4943d3018f
-https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.23.0-pyhd8ed1ab_0.conda#a920e114c4c2ced2280e266da65ab5e6
+https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.23.1-pyhd8ed1ab_0.conda#838b85f656b078bdd882ef97978e7f40
 https://conda.anaconda.org/conda-forge/osx-64/cftime-1.6.2-py38hbd87e4b_1.tar.bz2#6b61efa56393b9655334192cc5423659
-https://conda.anaconda.org/conda-forge/osx-64/contourpy-1.0.7-py38h98b9b1b_0.conda#c3d26ebf025c7b9c9ff2fbcaee1f7646
-https://conda.anaconda.org/conda-forge/osx-64/ipython-8.4.0-py38h50d1736_0.tar.bz2#01aa6e4355138850ed06c972926cc153
+https://conda.anaconda.org/conda-forge/osx-64/contourpy-1.1.0-py38h15a1a5b_0.conda#30d645ffb3572a3875e6fc8687857182
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda#58ca2d50c3b27b86fd7df62eaadbf9a9
-https://conda.anaconda.org/conda-forge/noarch/nbformat-5.8.0-pyhd8ed1ab_0.conda#1ca43103a08456b19222d93fd9d119ac
+https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
 https://conda.anaconda.org/conda-forge/osx-64/pandas-1.5.3-py38hec72209_1.conda#a8f001ab0a7c6312cea020bd20689765
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
 https://conda.anaconda.org/conda-forge/osx-64/pyerfa-2.0.0.3-py38hbd87e4b_0.conda#48a43c20176ae9fba912e9142bc066ad
 https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.15-pyhd8ed1ab_0.conda#27db656619a55d727eaf5a6ece3d2fd6
-https://conda.anaconda.org/conda-forge/osx-64/astropy-5.2.2-py38h073b4c8_0.conda#1b1da5798eae4db8e187844ac782db0f
-https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.0-pyh736e0ef_0.conda#6568402ca7540ad5b352fb51ffe17b51
+https://conda.anaconda.org/conda-forge/osx-64/astropy-5.0.6-py38h073b4c8_0.conda#d2955fea4da9c60ab73746c1d7e588bb
+https://conda.anaconda.org/conda-forge/noarch/ipython-8.12.0-pyhd1c38e8_0.conda#4b25de6cd2891e6bce87de8c5d85e27c
 https://conda.anaconda.org/conda-forge/osx-64/matplotlib-base-3.7.1-py38hcb346ec_0.conda#1f1eea98c232c8ef720175e12b00d0c4
-https://conda.anaconda.org/conda-forge/noarch/nbclient-0.7.4-pyhd8ed1ab_0.conda#f7aa15f77d29b11caa1df1eb15383c59
-https://conda.anaconda.org/conda-forge/osx-64/netcdf4-1.6.3-nompi_py38hfcbbda9_102.conda#cf4cec7ac00ee3f2d230dbb655fbc28b
-https://conda.anaconda.org/conda-forge/noarch/requests-2.29.0-pyhd8ed1ab_0.conda#5fa992d972fbccfc069161805122cb8d
+https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
+https://conda.anaconda.org/conda-forge/osx-64/netcdf4-1.6.4-nompi_py38h47ac6a0_100.conda#f86d4df9f8f46ae6d0c29bb87fe093b0
+https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/noarch/xarray-2023.1.0-pyhd8ed1ab_0.conda#c11eb03b6f77a0d22ae88c454c940f55
-https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.12.11-pyhd8ed1ab_1.conda#e8f0410e0aa03342304357c5cc3bb75d
+https://conda.anaconda.org/conda-forge/noarch/cachecontrol-0.13.0-pyhd8ed1ab_0.conda#9f0b2eb5f5dd2cec36d5342a80adfec0
 https://conda.anaconda.org/conda-forge/noarch/ensureconda-1.4.3-pyhd8ed1ab_0.tar.bz2#c99ae3abf501990769047b4b40a98f17
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.1-pyh736e0ef_0.conda#d5aa7d2cc9fe03f62cf6e7bcc8e1a8df
 https://conda.anaconda.org/conda-forge/osx-64/matplotlib-3.7.1-py38h50d1736_0.conda#14bce132d8a4546246b131c4289b480f
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.4.0-pyhd8ed1ab_0.conda#4456e6030a8309bdad57569b0170b6a3
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.6.0-pyhd8ed1ab_0.conda#879782bde4bbdb4c7b5d4054504a20d5
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.7.0-pyha770c72_3.conda#5936894aade8240c867d292aa0d980c6
 https://conda.anaconda.org/conda-forge/noarch/sphinx-5.0.0-pyh6c4a22f_1.tar.bz2#a7cc4b9c94548ff9a19b368f975e5404
 https://conda.anaconda.org/conda-forge/noarch/autodocsumm-0.2.11-pyhd8ed1ab_0.conda#547c48372c97c463c93af86d7f2c868c
-https://conda.anaconda.org/conda-forge/noarch/cachecontrol-with-filecache-0.12.11-pyhd8ed1ab_1.conda#9df660456c0076d27b802448f7ede78f
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.5.0-pyhd8ed1ab_0.conda#7fa3bd3d8dee42934f63711e9fbe959a
-https://conda.anaconda.org/conda-forge/noarch/myst-parser-1.0.0-pyhd8ed1ab_0.conda#e559708feb0aed1ae24c518e569ea3eb
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.4.0-pyhd8ed1ab_0.conda#127c702e1b1eff595be82bc6a78cfce0
+https://conda.anaconda.org/conda-forge/noarch/cachecontrol-with-filecache-0.13.0-pyhd8ed1ab_0.conda#3fd3d55ea862cc0736ac1cce6f44c2d1
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.6.0-pyhd8ed1ab_0.conda#39fd52b0fcb2fb52bac47a1419bf09bd
+https://conda.anaconda.org/conda-forge/noarch/myst-parser-0.18.1-pyhd8ed1ab_0.tar.bz2#bcfdf5c7d8bf5c6f6be7b4c66fff2eca
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.6.0-pyhd8ed1ab_0.conda#e8172ca42f2869bb90185c9356899e81
 https://conda.anaconda.org/conda-forge/noarch/pydata-sphinx-theme-0.13.3-pyhd8ed1ab_0.conda#07aca5f2dea315dcc16680d6891e9056
-https://conda.anaconda.org/conda-forge/osx-64/scipy-1.10.1-py38h1a492ef_1.conda#537c446eab40b1c7d34886dc72a52c5e
+https://conda.anaconda.org/conda-forge/osx-64/scipy-1.10.1-py38h9cf86d3_3.conda#5e20c77455e815704b008ab8f42f6169
 https://conda.anaconda.org/conda-forge/noarch/sphinx-autobuild-2021.3.14-pyhd8ed1ab_0.tar.bz2#1909f784dc37b4ab97afe2c95aeeabaa
 https://conda.anaconda.org/conda-forge/noarch/sphinx-copybutton-0.5.2-pyhd8ed1ab_0.conda#ac832cc43adc79118cf6e23f1f9b8995
-https://conda.anaconda.org/conda-forge/noarch/sphinx-design-0.4.1-pyhd8ed1ab_0.conda#14a64286fe896fe7e1a485fc91ccd022
+https://conda.anaconda.org/conda-forge/noarch/sphinx-design-0.4.1-pyhd8ed1ab_1.conda#c6b2e7903121c3210462a0866a561993
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-bibtex-2.5.0-pyhd8ed1ab_0.tar.bz2#b2e5c9aece936ebf9f26abdf71ddd74b
-https://conda.anaconda.org/conda-forge/noarch/conda-lock-1.4.0-pyhd8ed1ab_2.conda#e9ecdfe3e7d4f76d67afd65b02a621a0
+https://conda.anaconda.org/conda-forge/noarch/conda-lock-2.1.0-pyhd8ed1ab_0.conda#1e07afcf3d3e371fc3a3681fe9b78e90
 https://conda.anaconda.org/conda-forge/noarch/iapws-1.5.3-pyhd8ed1ab_0.tar.bz2#c5cad28f7c667df1910c3e9f8213c5eb
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.22.1-pyhd8ed1ab_0.conda#fc7172a6742a7c3c4331ddd7ed463ffc
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.4.0-pyhd8ed1ab_0.conda#a86727968b41c20dd3d73b91632e77dc
+https://conda.anaconda.org/conda-forge/noarch/jupyter-lsp-2.2.0-pyhd8ed1ab_0.conda#38589f4104d11f2a59ff01a9f4e3bfb3
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.23.0-pyhd8ed1ab_0.conda#942aa06b962c7e507884c6fbeb4d1f7d
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.6.0-pyhd8ed1ab_0.conda#59976ee8df1c6f82c4aa94b5fd6b745e
 https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
 https://conda.anaconda.org/conda-forge/noarch/patsy-0.5.3-pyhd8ed1ab_0.tar.bz2#50ef6b29b1fb0768ca82c5aeb4fb2d96
 https://conda.anaconda.org/conda-forge/noarch/seaborn-base-0.12.2-pyhd8ed1ab_0.conda#cf88f3a1c11536bc3c10c14ad00ccc42
 https://conda.anaconda.org/conda-forge/noarch/sphinx-book-theme-1.0.1-pyhd8ed1ab_0.conda#1ef419576de2c51b6e3a5a393eb35cda
-https://conda.anaconda.org/conda-forge/noarch/nbclassic-1.0.0-pyhb4ecaf3_1.conda#a0be31e9bd84d6eae87cdbf74c56b90b
-https://conda.anaconda.org/conda-forge/noarch/nbsphinx-0.9.1-pyhd8ed1ab_0.conda#a0b8b3d9eb22da29279a90883dcd5962
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab-4.0.2-pyhd8ed1ab_0.conda#8e102bf37f10dd49c248910450242a19
+https://conda.anaconda.org/conda-forge/noarch/nbsphinx-0.9.2-pyhd8ed1ab_0.conda#d1212b423fdd10d2da59601385561ff7
 https://conda.anaconda.org/conda-forge/osx-64/statsmodels-0.14.0-py38hd2faf92_1.conda#9367d8a5adfd7425b91ef0cf112d552e
-https://conda.anaconda.org/conda-forge/noarch/notebook-6.5.4-pyha770c72_0.conda#ec4ce3ce0a55ce21b6f5b86049b97af9
 https://conda.anaconda.org/conda-forge/noarch/seaborn-0.12.2-hd8ed1ab_0.conda#50847a47c07812f88581081c620f5160
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab-3.5.3-pyhd8ed1ab_0.conda#69f71bc3d176b3ad3d9564a32bd049b8
```

### Comparing `eradiate-0.23.2rc1/requirements/main.txt` & `eradiate-0.23.2rc2/requirements/pip/main.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,174 +1,175 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --allow-unsafe --output-file=requirements/main.txt --resolver=backtracking requirements/main.in
+#    pip-compile --allow-unsafe --output-file=requirements/pip/main.txt --resolver=backtracking requirements/pip/main.in
 #
 aenum==3.1.12
-    # via -r requirements/main.in
+    # via -r requirements/pip/main.in
 attrs==23.1.0
     # via
-    #   -r requirements/main.in
+    #   -r requirements/pip/main.in
     #   dessinemoi
     #   environ-config
     #   pinttrs
 certifi==2023.5.7
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
+    #   netcdf4
     #   requests
 cftime==1.6.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   netcdf4
 charset-normalizer==3.1.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   requests
 click==8.1.3
     # via
-    #   -r requirements/main.in
+    #   -r requirements/pip/main.in
     #   typer
-contourpy==1.0.7
+contourpy==1.1.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   matplotlib
 cycler==0.11.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   matplotlib
 dessinemoi==23.1.0
-    # via -r requirements/main.in
+    # via -r requirements/pip/main.in
 environ-config==23.2.0
-    # via -r requirements/main.in
-fonttools==4.39.3
+    # via -r requirements/pip/main.in
+fonttools==4.40.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   matplotlib
 idna==3.4
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   requests
 importlib-resources==5.12.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   matplotlib
 kiwisolver==1.4.4
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   matplotlib
 lazy-loader==0.2
-    # via -r requirements/main.in
-markdown-it-py==2.2.0
+    # via -r requirements/pip/main.in
+markdown-it-py==3.0.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   rich
 matplotlib==3.7.1
-    # via -r requirements/main.in
+    # via -r requirements/pip/main.in
 mdurl==0.1.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   markdown-it-py
-netcdf4==1.6.3
-    # via -r requirements/main.in
+netcdf4==1.6.4
+    # via -r requirements/pip/main.in
 numpy==1.24.3
     # via
-    #   -r requirements/main.in
+    #   -r requirements/pip/main.in
     #   cftime
     #   contourpy
     #   matplotlib
     #   netcdf4
     #   pandas
     #   scipy
     #   xarray
 packaging==23.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   matplotlib
     #   pooch
     #   xarray
-pandas==2.0.1
+pandas==2.0.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   xarray
 pillow==9.5.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   matplotlib
-pint==0.21
+pint==0.21.1
     # via
-    #   -r requirements/main.in
+    #   -r requirements/pip/main.in
     #   pinttrs
 pinttrs==23.2.0
-    # via -r requirements/main.in
-platformdirs==3.5.0
+    # via -r requirements/pip/main.in
+platformdirs==3.6.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   pooch
 pooch==1.7.0
-    # via -r requirements/main.in
+    # via -r requirements/pip/main.in
 portion==2.4.0
-    # via -r requirements/main.in
+    # via -r requirements/pip/main.in
 pygments==2.15.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   rich
-pyparsing==3.0.9
+pyparsing==3.1.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   matplotlib
 python-dateutil==2.8.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   pandas
-requests==2.30.0
+requests==2.31.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   pooch
-rich==13.3.5
-    # via -r requirements/main.in
-ruamel-yaml==0.17.24
-    # via -r requirements/main.in
+rich==13.4.2
+    # via -r requirements/pip/main.in
+ruamel-yaml==0.17.32
+    # via -r requirements/pip/main.in
 ruamel-yaml-clib==0.2.7
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   ruamel-yaml
 scipy==1.10.1
-    # via -r requirements/main.in
+    # via -r requirements/pip/main.in
 shellingham==1.5.0.post1
-    # via -r requirements/main.in
+    # via -r requirements/pip/main.in
 six==1.16.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   python-dateutil
 sortedcontainers==2.4.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   portion
 tqdm==4.65.0
-    # via -r requirements/main.in
+    # via -r requirements/pip/main.in
 typer==0.9.0
-    # via -r requirements/main.in
-typing-extensions==4.5.0
+    # via -r requirements/pip/main.in
+typing-extensions==4.6.3
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   rich
     #   typer
 tzdata==2023.3
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   pandas
-urllib3==2.0.2
+urllib3==1.26.16
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   requests
 xarray==2023.1.0
-    # via -r requirements/main.in
+    # via -r requirements/pip/main.in
 zipp==3.15.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   importlib-resources
```

### Comparing `eradiate-0.23.2rc1/requirements/make_conda_env.py` & `eradiate-0.23.2rc2/requirements/make_pip_in_files.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,99 +1,64 @@
 import os
-import sys
-from copy import deepcopy
 
 import click
 from ruamel.yaml import YAML
-from ruamel.yaml.comments import CommentedSeq as CS
-from setuptools.config.pyprojecttoml import read_configuration
 
 
 @click.command()
 @click.option(
     "-s",
     "--sections",
-    default="main,recommended,tests,dev,docs,production,optional",
+    default="dependencies,main,recommended,tests,dev,docs,optional",
     help="Dependency sections to include in the produced environment.yml file. "
-    "Default: 'main,recommended,tests,dev,docs,production,optional'",
+    "Default: 'dependencies,main,recommended,tests,dev,docs,optional'",
 )
 @click.option(
-    "-i", "--input", default="pyproject.toml", help="Path to pyproject.toml file."
+    "-o",
+    "--output-dir",
+    default="./requirements/pip",
+    help="Path to output directory. Default: ./requirements/pip",
+)
+@click.option(
+    "-l",
+    "--layered-config",
+    default="./requirements/layered.yml",
+    help="Path to layered requirement dependency configuration file. "
+    "Default: ./requirements/layered.yml",
 )
-@click.option("-o", "--output", default=None, help="Path to output file.")
 @click.option("-q", "--quiet", is_flag=True, help="Suppress terminal output.")
-def cli(sections, input, output, quiet):
-    """
-    Create a Conda environment file from a pyproject.toml.
-    """
-
-    # Set YAML parameters
-    yaml = YAML(typ="rt")  # Round-trip mode allows for comment insertion
-    indent_offset = 2
-    yaml.indent(offset=indent_offset)
-
-    # Load environment file template
-    with open(os.path.join("requirements", "environment.in")) as f:
-        env_yml = yaml.load(f.read())
-
-    # Extract dependency section contents
-    if not quiet:
-        print(f"Reading dependencies from {input}")
+def cli(sections, output_dir, layered_config, quiet):
+    # Load dependency list
 
-    setup_config = read_configuration(input)
     sections = [x.strip() for x in sections.split(",")]
-    section_indices = dict()
-    dep_list = deepcopy(env_yml["dependencies"]) if "dependencies" in env_yml else []
-    i = len(dep_list)
+
+    # Load layered dependency dependencies
+    yaml = YAML(typ="safe")
+    with open(layered_config) as f:
+        layered_yml = yaml.load(f.read())
 
     for section in sections:
-        section_indices[section] = i
+        if not quiet:
+            print(f"Processing section '{section}'")
+
+        packages = layered_yml[section].get("packages", [])
+
+        if not quiet:
+            print(f"Writing to {os.path.join(output_dir, f'{section}.in')}")
+
+        # Create .in file
+        with open(os.path.join(output_dir, f"{section}.in"), "w") as f:
+            # Prepend layered requirement includes
+            includes = layered_yml[section].get("includes", [])
+            for include in includes:
+                f.write(f"-r {include}.in\n")
+
+            constraints = layered_yml[section].get("constraints", [])
+            for constraint in constraints:
+                f.write(f"-c {constraint}.txt\n")
 
-        try:
-            packages = (
-                setup_config["project"]["dependencies"]
-                if section == "main"
-                else setup_config["project"]["optional-dependencies"][section]
-            )
-        except KeyError:
-            raise RuntimeError(f"Cannot fetch dependencies from {input}")
-
-        mitsuba_pkg = None
-
-        for package in packages:
-            if package in dep_list:  # Do not duplicate
-                continue
-            # Temporary fix until an eradiate_mitsuba conda package is made available
-            if "eradiate_mitsuba" in set(package.split("==") + package.split(">=") + package.split("<=") + package.split("!=")):
-                mitsuba_pkg = package
-                continue
-            dep_list.append(package)
-            i += 1
-
-        if mitsuba_pkg:
-            if "pip" not in dep_list:
-                dep_list.append("pip")
-            dep_list.append({"pip": [mitsuba_pkg]})
-
-    # Format dependency list
-    lst = CS(dep_list)
-
-    for section, i in section_indices.items():
-        lst.yaml_set_comment_before_after_key(i, section, indent_offset)
-
-    env_yml["dependencies"] = lst
-
-    # Output to terminal
-    if not quiet:
-        yaml.dump(env_yml, sys.stdout)
-
-    # Output to file
-    if output is not None:
-        with open(output, "w") as outfile:
-            if not quiet:
-                print()
-            print(f"Saving to {output}")
-            yaml.dump(env_yml, outfile)
+            f.write("\n".join(packages))
+            f.write("\n")
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `eradiate-0.23.2rc1/requirements/optional.txt` & `eradiate-0.23.2rc2/requirements/pip/optional.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,1017 +1,973 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --allow-unsafe --output-file=requirements/optional.txt --resolver=backtracking requirements/optional.in
+#    pip-compile --allow-unsafe --output-file=requirements/pip/optional.txt --resolver=backtracking requirements/pip/optional.in
 #
 aabbtree==2.8.1
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/recommended.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/recommended.in
 accessible-pygments==0.0.4
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   pydata-sphinx-theme
 aenum==3.1.12
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
-aiofiles==22.1.0
-    # via
-    #   -c requirements/dev.txt
-    #   ypy-websocket
-aiosqlite==0.19.0
-    # via
-    #   -c requirements/dev.txt
-    #   ypy-websocket
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
 alabaster==0.7.13
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   sphinx
-anyio==3.6.2
+anyio==3.7.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jupyter-server
 appdirs==1.4.4
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   ensureconda
 argon2-cffi==21.3.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jupyter-server
-    #   nbclassic
-    #   notebook
 argon2-cffi-bindings==21.2.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   argon2-cffi
 arrow==1.2.3
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   isoduration
 astropy==5.2.2
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/recommended.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/recommended.in
 asttokens==2.2.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   stack-data
+async-lru==2.0.2
+    # via
+    #   -c requirements/pip/dev.txt
+    #   jupyterlab
 attrs==23.1.0
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
     #   dessinemoi
     #   environ-config
     #   jsonschema
     #   pinttrs
 autodocsumm==0.2.11
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/docs.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/docs.in
 babel==2.12.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jupyterlab-server
     #   pydata-sphinx-theme
     #   sphinx
 backcall==0.2.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   ipython
 beautifulsoup4==4.12.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   nbconvert
     #   pydata-sphinx-theme
 bleach==6.0.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   nbconvert
 build==0.10.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   pip-tools
-cachecontrol[filecache]==0.12.11
+cachecontrol[filecache]==0.13.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   conda-lock
 cachy==0.3.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   conda-lock
 certifi==2023.5.7
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
+    #   netcdf4
     #   requests
 cffi==1.15.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   argon2-cffi-bindings
     #   cryptography
 cftime==1.6.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   netcdf4
 charset-normalizer==3.1.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   requests
 click==8.1.3
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
     #   click-default-group
     #   conda-lock
     #   ensureconda
     #   pip-tools
     #   typer
 click-default-group==1.2.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   conda-lock
 clikit==0.6.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   conda-lock
 colorama==0.4.6
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   sphinx-autobuild
 comm==0.1.3
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   ipykernel
-conda-lock==1.4.0
-    # via -r requirements/dev.in
-contourpy==1.0.7
+conda-lock==2.1.0
+    # via -r requirements/pip/dev.in
+contourpy==1.1.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   matplotlib
 crashtest==0.3.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   clikit
     #   conda-lock
-cryptography==40.0.2
+cryptography==41.0.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   secretstorage
 cycler==0.11.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   matplotlib
 debugpy==1.6.7
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   ipykernel
 decorator==5.1.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   ipython
 defusedxml==0.7.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   nbconvert
 dessinemoi==23.1.0
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
 distlib==0.3.6
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   virtualenv
 docutils==0.19
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   myst-parser
     #   nbsphinx
     #   pybtex-docutils
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinxcontrib-bibtex
 drjit==0.4.1
     # via eradiate-mitsuba
 ensureconda==1.4.3
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   conda-lock
 environ-config==23.2.0
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
-eradiate-mitsuba==0.0.1rc10
-    # via -r requirements/optional.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
+eradiate-mitsuba==0.0.1
+    # via -r requirements/pip/optional.in
 exceptiongroup==1.1.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
+    #   anyio
     #   pytest
 executing==1.2.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   stack-data
-fastjsonschema==2.16.3
+fastjsonschema==2.17.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   nbformat
-filelock==3.12.0
+filelock==3.12.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
+    #   cachecontrol
     #   conda-lock
     #   ensureconda
     #   virtualenv
-fonttools==4.39.3
+fonttools==4.40.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   matplotlib
 fqdn==1.5.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jsonschema
+gitdb==4.0.10
+    # via
+    #   -c requirements/pip/dev.txt
+    #   gitpython
+gitpython==3.1.31
+    # via
+    #   -c requirements/pip/dev.txt
+    #   conda-lock
 html5lib==1.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   conda-lock
 iapws==1.5.3
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/recommended.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/recommended.in
 idna==3.4
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   anyio
     #   jsonschema
     #   requests
 imagesize==1.4.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   sphinx
-importlib-metadata==6.6.0
+importlib-metadata==6.7.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jupyter-client
-    #   jupyter-ydoc
+    #   jupyter-lsp
+    #   jupyterlab
     #   jupyterlab-server
     #   keyring
     #   nbconvert
     #   sphinx
     #   sphinxcontrib-bibtex
 importlib-resources==5.12.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jsonschema
+    #   jupyterlab
     #   keyring
     #   matplotlib
 iniconfig==2.0.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   pytest
-ipykernel==6.23.0
+ipykernel==6.23.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   ipywidgets
-    #   nbclassic
-    #   notebook
+    #   jupyterlab
 ipython==8.12.2
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/recommended.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/recommended.in
     #   ipykernel
     #   ipywidgets
-    #   jupyterlab
-ipython-genutils==0.2.0
-    # via
-    #   -c requirements/dev.txt
-    #   nbclassic
-    #   notebook
 ipywidgets==8.0.6
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/recommended.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/recommended.in
 isoduration==20.11.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jsonschema
 jaraco-classes==3.2.3
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   keyring
 jedi==0.18.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   ipython
 jeepney==0.8.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   keyring
     #   secretstorage
 jinja2==3.1.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   conda-lock
     #   jupyter-server
     #   jupyterlab
     #   jupyterlab-server
     #   myst-parser
-    #   nbclassic
     #   nbconvert
     #   nbsphinx
-    #   notebook
     #   sphinx
-json5==0.9.11
+json5==0.9.14
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jupyterlab-server
-jsonpointer==2.3
+jsonpointer==2.4
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jsonschema
 jsonschema[format-nongpl]==4.17.3
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jupyter-events
     #   jupyterlab-server
     #   nbformat
 jupyter-client==8.2.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   ipykernel
     #   jupyter-server
-    #   nbclassic
     #   nbclient
-    #   notebook
-jupyter-core==5.3.0
+jupyter-core==5.3.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   jupyterlab
-    #   nbclassic
     #   nbclient
     #   nbconvert
     #   nbformat
-    #   notebook
 jupyter-events==0.6.3
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jupyter-server
-    #   jupyter-server-fileid
-jupyter-server==2.5.0
+jupyter-lsp==2.2.0
+    # via
+    #   -c requirements/pip/dev.txt
+    #   jupyterlab
+jupyter-server==2.6.0
     # via
-    #   -c requirements/dev.txt
-    #   jupyter-server-fileid
+    #   -c requirements/pip/dev.txt
+    #   jupyter-lsp
     #   jupyterlab
     #   jupyterlab-server
-    #   nbclassic
     #   notebook-shim
-jupyter-server-fileid==0.9.0
-    # via
-    #   -c requirements/dev.txt
-    #   jupyter-server-ydoc
 jupyter-server-terminals==0.4.4
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jupyter-server
-jupyter-server-ydoc==0.8.0
+jupyterlab==4.0.2
     # via
-    #   -c requirements/dev.txt
-    #   jupyterlab
-jupyter-ydoc==0.2.4
-    # via
-    #   -c requirements/dev.txt
-    #   jupyter-server-ydoc
-    #   jupyterlab
-jupyterlab==3.6.3
-    # via
-    #   -c requirements/dev.txt
-    #   -r requirements/recommended.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/recommended.in
 jupyterlab-pygments==0.2.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   nbconvert
-jupyterlab-server==2.22.1
+jupyterlab-server==2.23.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jupyterlab
 jupyterlab-widgets==3.0.7
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   ipywidgets
-keyring==23.13.1
+keyring==24.0.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   conda-lock
 kiwisolver==1.4.4
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   matplotlib
 latexcodec==2.0.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   pybtex
 lazy-loader==0.2
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
 livereload==2.6.3
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   sphinx-autobuild
-lockfile==0.12.2
+markdown-it-py==3.0.0
     # via
-    #   -c requirements/dev.txt
-    #   cachecontrol
-markdown-it-py==2.2.0
-    # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   mdit-py-plugins
     #   myst-parser
     #   rich
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jinja2
     #   nbconvert
 matplotlib==3.7.1
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
     #   seaborn
 matplotlib-inline==0.1.6
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.3.5
+mdit-py-plugins==0.4.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   myst-parser
 mdurl==0.1.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   markdown-it-py
-mistune==2.0.5
+mistune==3.0.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   nbconvert
 more-itertools==9.1.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jaraco-classes
 msgpack==1.0.5
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   cachecontrol
-myst-parser==1.0.0
-    # via
-    #   -c requirements/dev.txt
-    #   -r requirements/docs.in
-nbclassic==1.0.0
+myst-parser==2.0.0
     # via
-    #   -c requirements/dev.txt
-    #   jupyterlab
-    #   notebook
-nbclient==0.7.4
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/docs.in
+nbclient==0.8.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   nbconvert
-nbconvert==7.4.0
+nbconvert==7.6.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jupyter-server
-    #   nbclassic
     #   nbsphinx
-    #   notebook
-nbformat==5.8.0
+nbformat==5.9.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jupyter-server
-    #   nbclassic
     #   nbclient
     #   nbconvert
     #   nbsphinx
-    #   notebook
-nbsphinx==0.9.1
+nbsphinx==0.9.2
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/docs.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/docs.in
 nest-asyncio==1.5.6
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   ipykernel
-    #   nbclassic
-    #   notebook
-netcdf4==1.6.3
-    # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
-notebook==6.5.4
+netcdf4==1.6.4
     # via
-    #   -c requirements/dev.txt
-    #   jupyterlab
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
+networkx==3.1
+    # via -r requirements/pip/dev.in
 notebook-shim==0.2.3
     # via
-    #   -c requirements/dev.txt
-    #   nbclassic
+    #   -c requirements/pip/dev.txt
+    #   jupyterlab
 numpy==1.24.3
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
     #   astropy
     #   cftime
     #   contourpy
     #   matplotlib
     #   netcdf4
     #   pandas
     #   pyerfa
     #   scipy
     #   seaborn
     #   xarray
+overrides==7.3.1
+    # via
+    #   -c requirements/pip/dev.txt
+    #   jupyter-server
 packaging==23.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   astropy
     #   build
     #   conda-lock
     #   ipykernel
     #   jupyter-server
     #   jupyterlab
     #   jupyterlab-server
     #   matplotlib
     #   nbconvert
     #   pooch
     #   pydata-sphinx-theme
     #   pytest
     #   sphinx
     #   xarray
-pandas==2.0.1
+pandas==2.0.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   seaborn
     #   xarray
 pandocfilters==1.5.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   nbconvert
 parso==0.8.3
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jedi
 pastel==0.2.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   clikit
 pexpect==4.8.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   ipython
 pickleshare==0.7.5
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   ipython
 pillow==9.5.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   matplotlib
-pint==0.21
+pint==0.21.1
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
     #   pinttrs
 pinttrs==23.2.0
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
 pip-tools==6.13.0
-    # via -r requirements/dev.in
+    # via -r requirements/pip/dev.in
 pkginfo==1.9.6
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   conda-lock
 pkgutil-resolve-name==1.3.10
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jsonschema
-platformdirs==3.5.0
+platformdirs==3.6.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jupyter-core
     #   pooch
     #   virtualenv
 pluggy==1.0.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   pytest
 pooch==1.7.0
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
 portion==2.4.0
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
-prometheus-client==0.16.0
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
+prometheus-client==0.17.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jupyter-server
-    #   nbclassic
-    #   notebook
 prompt-toolkit==3.0.38
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   ipython
 psutil==5.9.5
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   ipykernel
 ptyprocess==0.7.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   pexpect
     #   terminado
 pure-eval==0.2.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   stack-data
 pybtex==0.24.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   pybtex-docutils
     #   sphinxcontrib-bibtex
 pybtex-docutils==1.0.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   sphinxcontrib-bibtex
 pycparser==2.21
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   cffi
-pydantic==1.10.7
+pydantic==1.10.9
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   conda-lock
 pydata-sphinx-theme==0.13.3
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   sphinx-book-theme
 pyerfa==2.0.0.3
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   astropy
 pygments==2.15.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   accessible-pygments
     #   ipython
     #   nbconvert
     #   pydata-sphinx-theme
     #   rich
     #   sphinx
 pylev==1.4.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   clikit
-pyparsing==3.0.9
+pyparsing==3.1.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   matplotlib
 pyproject-hooks==1.0.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   build
 pyrsistent==0.19.3
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jsonschema
-pytest==7.3.1
+pytest==7.3.2
     # via
-    #   -r requirements/tests.in
+    #   -r requirements/pip/tests.in
     #   pytest-json-report
     #   pytest-metadata
 pytest-json-report==1.5.0
-    # via -r requirements/tests.in
-pytest-metadata==2.0.4
+    # via -r requirements/pip/tests.in
+pytest-metadata==3.0.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   pytest-json-report
 python-dateutil==2.8.2
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/recommended.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/recommended.in
     #   arrow
     #   jupyter-client
     #   matplotlib
     #   pandas
 python-json-logger==2.0.7
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jupyter-events
 pytz==2023.3
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   babel
     #   pandas
 pyyaml==6.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   astropy
     #   conda-lock
     #   jupyter-events
     #   myst-parser
     #   pybtex
-pyzmq==25.0.2
+pyzmq==25.1.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
-    #   nbclassic
-    #   notebook
-requests==2.30.0
+requests==2.31.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   cachecontrol
     #   conda-lock
     #   ensureconda
     #   jupyterlab-server
     #   pooch
     #   sphinx
 rfc3339-validator==0.1.4
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jsonschema
     #   jupyter-events
 rfc3986-validator==0.1.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jsonschema
     #   jupyter-events
-rich==13.3.5
+rich==13.4.2
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
-ruamel-yaml==0.17.24
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
+ruamel-yaml==0.17.32
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
     #   conda-lock
 ruamel-yaml-clib==0.2.7
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   ruamel-yaml
 scipy==1.10.1
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
     #   iapws
 seaborn==0.12.2
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/recommended.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/recommended.in
 secretstorage==3.3.3
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   keyring
 send2trash==1.8.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jupyter-server
-    #   nbclassic
-    #   notebook
 shellingham==1.5.0.post1
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
 six==1.16.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   asttokens
     #   bleach
     #   html5lib
     #   latexcodec
     #   livereload
     #   pybtex
     #   python-dateutil
     #   rfc3339-validator
+smmap==5.0.0
+    # via
+    #   -c requirements/pip/dev.txt
+    #   gitdb
 sniffio==1.3.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   anyio
 snowballstemmer==2.2.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   sphinx
 sortedcontainers==2.4.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   portion
 soupsieve==2.4.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   beautifulsoup4
 sphinx==6.2.1
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/docs.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/docs.in
     #   autodocsumm
     #   myst-parser
     #   nbsphinx
     #   pydata-sphinx-theme
     #   sphinx-autobuild
     #   sphinx-book-theme
     #   sphinx-copybutton
     #   sphinx-design
     #   sphinxcontrib-bibtex
 sphinx-autobuild==2021.3.14
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/docs.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/docs.in
 sphinx-book-theme==1.0.1
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/docs.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/docs.in
 sphinx-copybutton==0.5.2
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/docs.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/docs.in
 sphinx-design==0.4.1
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/docs.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/docs.in
 sphinxcontrib-applehelp==1.0.4
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   sphinx
 sphinxcontrib-bibtex==2.5.0
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/docs.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/docs.in
 sphinxcontrib-devhelp==1.0.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   sphinx
 sphinxcontrib-htmlhelp==2.0.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   sphinx
 sphinxcontrib-jsmath==1.0.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   sphinx
 sphinxcontrib-qthelp==1.0.3
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   sphinx
 stack-data==0.6.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   ipython
 terminado==0.17.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jupyter-server
     #   jupyter-server-terminals
-    #   nbclassic
-    #   notebook
 tinycss2==1.2.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   nbconvert
 tomli==2.0.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   build
     #   conda-lock
     #   jupyterlab
     #   pyproject-hooks
     #   pytest
 tomlkit==0.11.8
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   conda-lock
 toolz==0.12.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   conda-lock
-tornado==6.3.1
+tornado==6.3.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   jupyterlab
     #   livereload
-    #   nbclassic
-    #   notebook
     #   terminado
 tqdm==4.65.0
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
 traitlets==5.9.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   jupyter-events
     #   jupyter-server
+    #   jupyterlab
     #   matplotlib-inline
-    #   nbclassic
     #   nbclient
     #   nbconvert
     #   nbformat
     #   nbsphinx
-    #   notebook
 typer==0.9.0
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
-typing-extensions==4.5.0
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
+typing-extensions==4.6.3
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
+    #   async-lru
     #   conda-lock
     #   ipython
     #   pydantic
     #   pydata-sphinx-theme
     #   rich
     #   typer
 tzdata==2023.3
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   pandas
 uri-template==1.2.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jsonschema
-urllib3==2.0.2
+urllib3==1.26.16
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
+    #   conda-lock
     #   requests
-virtualenv==20.23.0
+virtualenv==20.23.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   conda-lock
 wcwidth==0.2.6
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   prompt-toolkit
 webcolors==1.13
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jsonschema
 webencodings==0.5.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   bleach
     #   html5lib
     #   tinycss2
-websocket-client==1.5.1
+websocket-client==1.6.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   jupyter-server
 wheel==0.40.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   pip-tools
 widgetsnbextension==4.0.7
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   ipywidgets
 xarray==2023.1.0
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
-y-py==0.5.9
-    # via
-    #   -c requirements/dev.txt
-    #   jupyter-ydoc
-    #   ypy-websocket
-ypy-websocket==0.8.2
-    # via
-    #   -c requirements/dev.txt
-    #   jupyter-server-ydoc
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
 zipp==3.15.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 pip==23.1.2
     # via
-    #   -r requirements/dev.in
+    #   -r requirements/pip/dev.in
     #   pip-tools
-setuptools==67.7.2
+setuptools==68.0.0
     # via
-    #   -r requirements/dev.in
+    #   -r requirements/pip/dev.in
     #   pip-tools
```

### Comparing `eradiate-0.23.2rc1/requirements/tests.txt` & `eradiate-0.23.2rc2/requirements/pip/tests.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,238 +1,239 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --allow-unsafe --output-file=requirements/tests.txt --resolver=backtracking requirements/tests.in
+#    pip-compile --allow-unsafe --output-file=requirements/pip/tests.txt --resolver=backtracking requirements/pip/tests.in
 #
 aenum==3.1.12
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
 attrs==23.1.0
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
     #   dessinemoi
     #   environ-config
     #   pinttrs
 certifi==2023.5.7
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
+    #   netcdf4
     #   requests
 cftime==1.6.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   netcdf4
 charset-normalizer==3.1.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   requests
 click==8.1.3
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
     #   typer
-contourpy==1.0.7
+contourpy==1.1.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   matplotlib
 cycler==0.11.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   matplotlib
 dessinemoi==23.1.0
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
 environ-config==23.2.0
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
 exceptiongroup==1.1.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   pytest
-fonttools==4.39.3
+fonttools==4.40.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   matplotlib
 idna==3.4
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   requests
 importlib-resources==5.12.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   matplotlib
 iniconfig==2.0.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   pytest
 kiwisolver==1.4.4
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   matplotlib
 lazy-loader==0.2
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
-markdown-it-py==2.2.0
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
+markdown-it-py==3.0.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   rich
 matplotlib==3.7.1
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
 mdurl==0.1.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   markdown-it-py
-netcdf4==1.6.3
+netcdf4==1.6.4
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
 numpy==1.24.3
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
     #   cftime
     #   contourpy
     #   matplotlib
     #   netcdf4
     #   pandas
     #   scipy
     #   xarray
 packaging==23.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   matplotlib
     #   pooch
     #   pytest
     #   xarray
-pandas==2.0.1
+pandas==2.0.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   xarray
 pillow==9.5.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   matplotlib
-pint==0.21
+pint==0.21.1
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
     #   pinttrs
 pinttrs==23.2.0
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
-platformdirs==3.5.0
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
+platformdirs==3.6.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   pooch
 pluggy==1.0.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   pytest
 pooch==1.7.0
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
 portion==2.4.0
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
 pygments==2.15.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   rich
-pyparsing==3.0.9
+pyparsing==3.1.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   matplotlib
-pytest==7.3.1
+pytest==7.3.2
     # via
-    #   -r requirements/tests.in
+    #   -r requirements/pip/tests.in
     #   pytest-json-report
     #   pytest-metadata
 pytest-json-report==1.5.0
-    # via -r requirements/tests.in
-pytest-metadata==2.0.4
+    # via -r requirements/pip/tests.in
+pytest-metadata==3.0.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   pytest-json-report
 python-dateutil==2.8.2
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   pandas
-requests==2.30.0
+requests==2.31.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   pooch
-rich==13.3.5
+rich==13.4.2
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
-ruamel-yaml==0.17.24
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
+ruamel-yaml==0.17.32
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
 ruamel-yaml-clib==0.2.7
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   ruamel-yaml
 scipy==1.10.1
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
 shellingham==1.5.0.post1
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
 six==1.16.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   python-dateutil
 sortedcontainers==2.4.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   portion
 tomli==2.0.1
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   pytest
 tqdm==4.65.0
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
 typer==0.9.0
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
-typing-extensions==4.5.0
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
+typing-extensions==4.6.3
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   rich
     #   typer
 tzdata==2023.3
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   pandas
-urllib3==2.0.2
+urllib3==1.26.16
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   requests
 xarray==2023.1.0
     # via
-    #   -c requirements/dev.txt
-    #   -r requirements/main.in
+    #   -c requirements/pip/dev.txt
+    #   -r requirements/pip/main.in
 zipp==3.15.0
     # via
-    #   -c requirements/dev.txt
+    #   -c requirements/pip/dev.txt
     #   importlib-resources
```

### Comparing `eradiate-0.23.2rc1/setpath.sh` & `eradiate-0.23.2rc2/setpath.sh`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/__init__.pyi` & `eradiate-0.23.2rc2/src/eradiate/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/_config.py` & `eradiate-0.23.2rc2/src/eradiate/_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 variables. A single instance :data:`.config` is aliased in the top-level module
 for convenience.
 """
 
 import enum
 import os.path
 import pathlib
-from importlib.metadata import version, PackageNotFoundError
 
 import attrs
 import environ
 from environ._environ_config import CNF_KEY, RAISE, _ConfigEntry
 from environ.exceptions import ConfigError
 
 from .frame import AzimuthConvention
@@ -130,30 +129,28 @@
         default=None,
     )
 
     @source_dir.validator
     def _dir_validator(self, var, dir):
 
         if dir is None:
-            try:
-                version("eradiate-mitsuba")
-                return
-            except PackageNotFoundError as pkg_error:
+            if not __import__("eradiate").kernel.ERADIATE_MITSUBA_PACKAGE:
                 raise ConfigError(
                     "Could not find a suitable production installation for the "
                     "Eradiate kernel. This is either because you are using Eradiate "
                     "in a production environment without having the eradiate-mitsuba "
                     "package installed, or because you are using Eradiate directly "
                     "from the sources. In the latter case, please make sure the "
                     "'ERADIATE_SOURCE_DIR' environment variable is correctly set to "
                     "the Eradiate installation directory. If you are using Eradiate "
                     "directly from the sources, you can alternatively source the "
                     "provided setpath.sh script. You can install the eradiate-mitsuba "
                     "package using 'pip install eradiate-mitsuba'."
-                ) from pkg_error
+                )
+            return
 
         eradiate_init = dir / "src" / "eradiate" / "__init__.py"
 
         if not eradiate_init.is_file():
             raise ConfigError(
                 f"While configuring Eradiate: could not find {eradiate_init} file. "
                 "Please make sure the 'ERADIATE_SOURCE_DIR' environment variable is "
```

### Comparing `eradiate-0.23.2rc1/src/eradiate/_factory.py` & `eradiate-0.23.2rc2/src/eradiate/_factory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/_mode.py` & `eradiate-0.23.2rc2/src/eradiate/_mode.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/attrs.py` & `eradiate-0.23.2rc2/src/eradiate/attrs.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/cli/__init__.py` & `eradiate-0.23.2rc2/src/eradiate/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/cli/data.py` & `eradiate-0.23.2rc2/src/eradiate/cli/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,18 @@
     file_list: Annotated[
         Optional[List[str]],
         typer.Argument(
             help="An arbitrary number of relative paths to files to be "
             "retrieved from the data store. If unset, the list of "
             "files is read from a YAML file which can be specified by "
             "using the ``--from-file`` option and defaults to "
-            "``$ERADIATE_SOURCE_DIR/resources/downloads.yml``."
+            "``$ERADIATE_SOURCE_DIR/data/downloads.yml`` a production "
+            "environment and "
+            "``$ERADIATE_SOURCE_DIR/data/downloads_development.yml`` in a "
+            "development environment."
         ),
     ] = None,
     from_file: Annotated[
         Optional[str],
         typer.Option(
             "--from-file",
             "-f",
```

### Comparing `eradiate-0.23.2rc1/src/eradiate/cli/show.py` & `eradiate-0.23.2rc2/src/eradiate/cli/show.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/cli/srf.py` & `eradiate-0.23.2rc2/src/eradiate/cli/srf.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/contexts.py` & `eradiate-0.23.2rc2/src/eradiate/contexts.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/converters.py` & `eradiate-0.23.2rc2/src/eradiate/converters.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,16 @@
     "on_quantity",
     "to_dataset",
 ]
 
 import os
 import typing as t
 
+import mitsuba as mi
+import numpy as np
 import pint
 import xarray as xr
 
 from . import data
 from .attrs import AUTO
 from .typing import PathLike
 
@@ -111,15 +113,14 @@
 
     A converter without dataset identifier interpretation:
 
     >>> aerosol_converter = to_dataset()
     """
 
     def converter(value: xr.Dataset | PathLike) -> xr.Dataset:
-
         if isinstance(value, xr.Dataset):
             return value
 
         # Path (local or remote)
         if str(value).endswith(".nc"):
             # Try and open a file if it is directly referenced
             if os.path.isfile(value):
@@ -133,7 +134,25 @@
             return load_from_id(value)
 
         # Abnormal state
         # Reference must be provided as a Dataset, a path-like or a str
         raise ValueError(f"Cannot convert value '{value}'")
 
     return converter
+
+
+def to_mi_scalar_transform(value):
+    """
+    Convert an array-like value to a :class:`mitsuba.ScalarTransform4f`.
+    If `value` is a Numpy array, it is used to initialize a
+    :class:`mitsuba.ScalarTransform4f` without copy; if it is a list, a Numpy
+    array is first created from it. Otherwise, `value` is forwarded without
+    change.
+    """
+    if isinstance(value, np.ndarray):
+        return mi.ScalarTransform4f(value)
+
+    elif isinstance(value, list):
+        return mi.ScalarTransform4f(np.array(value))
+
+    else:
+        return value
```

### Comparing `eradiate-0.23.2rc1/src/eradiate/data/__init__.pyi` & `eradiate-0.23.2rc2/src/eradiate/data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/data/_access.py` & `eradiate-0.23.2rc2/src/eradiate/data/_access.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/data/_blind_directory.py` & `eradiate-0.23.2rc2/src/eradiate/data/_blind_directory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/data/_blind_online.py` & `eradiate-0.23.2rc2/src/eradiate/data/_blind_online.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/data/_core.py` & `eradiate-0.23.2rc2/src/eradiate/data/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/data/_multi.py` & `eradiate-0.23.2rc2/src/eradiate/data/_multi.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/data/_safe_directory.py` & `eradiate-0.23.2rc2/src/eradiate/data/_safe_directory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/data/_safe_online.py` & `eradiate-0.23.2rc2/src/eradiate/data/_safe_online.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/data/_store.py` & `eradiate-0.23.2rc2/src/eradiate/data/_store.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,21 @@
 
     Parameters
     ----------
     offline : bool, optional
         If ``True``, replace all online data stores with blind directory data
         stores. If unset, the global offline configuration is used.
 
+    production : bool, optional
+        If ``True``, replace all development data stores providing files from
+        the current local source folder with online safe data stores. If set to
+        ``True`` with ``offline`` flag set to ``True``, then the data must be
+        provided by the user before accessing it. If unset, the global
+        production configuration is used.
+
     Notes
     -----
     This function is called automatically when the ``eradiate.data`` package is
     imported.
     """
     global data_store
```

### Comparing `eradiate-0.23.2rc1/src/eradiate/data/downloads.yml` & `eradiate-0.23.2rc2/src/eradiate/data/downloads.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/data/downloads_development.yml` & `eradiate-0.23.2rc2/src/eradiate/data/downloads_development.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/exceptions.py` & `eradiate-0.23.2rc2/src/eradiate/exceptions.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/experiments/_atmosphere.py` & `eradiate-0.23.2rc2/src/eradiate/experiments/_atmosphere.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,15 @@
 
 from ._core import EarthObservationExperiment, Experiment
 from ._helpers import (
     measure_inside_atmosphere,
     surface_converter,
 )
 from ..attrs import documented, get_doc, parse_docs
-from ..scenes.atmosphere import (
-    Atmosphere,
-    HomogeneousAtmosphere,
-    atmosphere_factory,
-)
+from ..scenes.atmosphere import Atmosphere, HomogeneousAtmosphere, atmosphere_factory
 from ..scenes.bsdfs import LambertianBSDF
 from ..scenes.core import SceneElement
 from ..scenes.geometry import (
     PlaneParallelGeometry,
     SceneGeometry,
     SphericalShellGeometry,
 )
```

### Comparing `eradiate-0.23.2rc1/src/eradiate/experiments/_canopy.py` & `eradiate-0.23.2rc2/src/eradiate/experiments/_canopy.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/experiments/_canopy_atmosphere.py` & `eradiate-0.23.2rc2/src/eradiate/experiments/_canopy_atmosphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/experiments/_core.py` & `eradiate-0.23.2rc2/src/eradiate/experiments/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/experiments/_dem.py` & `eradiate-0.23.2rc2/src/eradiate/experiments/_dem.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,68 +1,72 @@
 from __future__ import annotations
 
 import typing as t
 import warnings
 
 import attrs
 
-from ._core import EarthObservationExperiment, Experiment
-from ._helpers import (
-    measure_inside_atmosphere,
-    surface_converter,
-)
-from ..attrs import documented, get_doc, parse_docs
-from ..scenes.atmosphere import (
-    Atmosphere,
-    HomogeneousAtmosphere,
-    atmosphere_factory,
-)
+from ._core import EarthObservationExperiment
+from ._helpers import measure_inside_atmosphere, surface_converter
+from ..attrs import documented, parse_docs
+from ..scenes.atmosphere import Atmosphere, HomogeneousAtmosphere, atmosphere_factory
 from ..scenes.bsdfs import LambertianBSDF
 from ..scenes.core import SceneElement
-from ..scenes.geometry import PlaneParallelGeometry, SceneGeometry
+from ..scenes.geometry import (
+    PlaneParallelGeometry,
+    SceneGeometry,
+    SphericalShellGeometry,
+)
 from ..scenes.integrators import Integrator, VolPathIntegrator, integrator_factory
 from ..scenes.measure import DistantMeasure, Measure, TargetPoint
-from ..scenes.shapes import RectangleShape
-from ..scenes.surface import BasicSurface, DEMSurface, surface_factory
-from ..units import unit_registry as ureg
+from ..scenes.surface import BasicSurface, DEMSurface
 
 
 @parse_docs
 @attrs.define
 class DEMExperiment(EarthObservationExperiment):
     """
-    Simulate radiation in a scene with a digital elevation model (DEM)
-    under a 1D atmosphere.
+    Simulate radiation in a scene with a digital elevation model (DEM) under a
+    1D atmosphere.
+
+    Warnings
+    --------
+    * Although technically supported, DEMs extending below 0 elevation may be
+      a tricky case because atmospheric profile behaviour below sea level is
+      undefined. This will be addressed in a future release.
 
     Notes
     -----
     * When using distant measures, setting a target is highly recommended. This
       experiment will issue a warning during configuration if it detects that a
       distant measure is used with no or an inappropriate target. If a distant
       measure is used and no target is set, it defaults to [0, 0, 0].
 
     * This experiment supports arbitrary measure positioning, except for
       :class:`.MultiRadiancemeterMeasure`, for which subsensor origins are
       required to be either all inside or all outside of the atmosphere. If an
       unsuitable configuration is detected, a :class:`ValueError` will be raised
       during initialization.
 
-    * Currently this experiment is limited to the plane-parallel geometry.
+    * Even without an atmosphere, this experiment requries using a volumetric
+      path tracing integrator.
     """
 
-    # Currently, only the plane parallel geometry is supported
-    geometry: PlaneParallelGeometry = documented(
+    geometry: SceneGeometry = documented(
         attrs.field(
             default="plane_parallel",
             converter=SceneGeometry.convert,
-            validator=attrs.validators.instance_of(PlaneParallelGeometry),
+            validator=attrs.validators.instance_of(
+                (PlaneParallelGeometry, SphericalShellGeometry)
+            ),
         ),
         doc="Problem geometry.",
-        type=".PlaneParallelGeometry",
-        init_type="str or dict or .PlaneParallelGeometry",
+        type=".SceneGeometry",
+        init_type='{"plane_parallel", "spherical_shell"} or dict or '
+        ".PlaneParallelGeometry or .SphericalShellGeometry",
         default='"plane_parallel"',
     )
 
     atmosphere: Atmosphere | None = documented(
         attrs.field(
             factory=HomogeneousAtmosphere,
             converter=attrs.converters.optional(atmosphere_factory.convert),
@@ -70,60 +74,47 @@
                 attrs.validators.instance_of(Atmosphere)
             ),
         ),
         doc="Atmosphere specification. If set to ``None``, no atmosphere will "
         "be added. "
         "This parameter can be specified as a dictionary which will be "
         "interpreted by :data:`.atmosphere_factory`.",
-        type=":class:`.Atmosphere` or None",
-        init_type=":class:`.Atmosphere` or dict or None",
+        type=".Atmosphere or None",
+        init_type=".Atmosphere or dict or None",
         default=":class:`HomogeneousAtmosphere() <.HomogeneousAtmosphere>`",
     )
 
-    surface: BasicSurface | None = documented(
+    surface: BasicSurface | DEMSurface | None = documented(
         attrs.field(
             factory=lambda: BasicSurface(bsdf=LambertianBSDF()),
             converter=attrs.converters.optional(surface_converter),
             validator=attrs.validators.optional(
-                attrs.validators.instance_of(BasicSurface)
+                attrs.validators.instance_of((BasicSurface, DEMSurface))
             ),
         ),
         doc="Surface specification. If set to ``None``, no surface will be "
         "added. This parameter can be specified as a dictionary which will be "
         "interpreted by :data:`.surface_factory` and :data:`.bsdf_factory`.",
-        type=".BasicSurface or None",
-        init_type=".BasicSurface or .BSDF or dict, optional",
+        type=".Surface or None",
+        init_type=".BasicSurface or .DEMSurface or .BSDF or dict, optional",
         default=":class:`BasicSurface(bsdf=LambertianBSDF()) <.BasicSurface>`",
     )
 
-    dem: DEMSurface | None = documented(
-        attrs.field(
-            default=None,
-            converter=attrs.converters.optional(surface_factory.convert),
-            validator=attrs.validators.optional(
-                attrs.validators.instance_of(DEMSurface)
-            ),
-        ),
-        doc="Digital elevation model (DEM) specification. If set to ``None``, no DEM will be "
-        "added. This parameter can be specified as a dictionary which will be "
-        "interpreted by :data:`.surface_factory`",
-        type=".DEMSurface or None",
-        init_type=".DEMSurface or dict, optional",
-        default="None",
-    )
-
     _integrator: Integrator = documented(
         attrs.field(
             factory=VolPathIntegrator,
             converter=integrator_factory.convert,
-            validator=attrs.validators.instance_of(Integrator),
+            validator=attrs.validators.instance_of(VolPathIntegrator),
         ),
-        doc=get_doc(Experiment, attrib="_integrator", field="doc"),
-        type=get_doc(Experiment, attrib="_integrator", field="type"),
-        init_type=get_doc(Experiment, attrib="_integrator", field="init_type"),
+        doc="Monte Carlo integration algorithm specification. "
+        "This parameter can be specified as a dictionary which will be "
+        "interpreted by :data:`.integrator_factory`. The DEMExperiment requires"
+        "the use of a .VolPathIntegrator.",
+        type=".VolPathIntegrator",
+        init_type=".VolPathIntegrator or dict",
         default=":class:`VolPathIntegrator() <.VolPathIntegrator>`",
     )
 
     def __attrs_post_init__(self):
         self._normalize_spectral()
         self._normalize_atmosphere()
         self._normalize_measures()
@@ -140,15 +131,15 @@
         Ensure that distant measure targets are set to appropriate values.
         Processed measures will have their ray target and origin parameters
         overridden if relevant.
         """
         for measure in self.measures:
             # Override ray target location if relevant
             if isinstance(measure, DistantMeasure):
-                if self.dem is not None:
+                if isinstance(self.surface, DEMSurface):
                     if measure.target is None:
                         msg = (
                             f"Measure '{measure.id}' has its target unset "
                             "and the DEM is set. This is not recommended."
                         )
 
                     elif isinstance(measure.target, TargetPoint):
@@ -164,18 +155,14 @@
                         measure.target = {"type": "point", "xyz": [0, 0, 0]}
 
                     msg = None
 
                 if msg is not None:
                     warnings.warn(UserWarning(msg))
 
-    @property
-    def _default_surface_width(self):
-        return 1.0 * ureg.km
-
     def _dataset_metadata(self, measure: Measure) -> dict[str, str]:
         result = super()._dataset_metadata(measure)
 
         if measure.is_distant():
             result["title"] = "Top-of-atmosphere simulation results"
 
         return result
@@ -196,35 +183,26 @@
     def scene_objects(self) -> dict[str, SceneElement]:
         # Inherit docstring
 
         objects = {}
 
         # Process atmosphere
         if self.atmosphere is not None:
-            objects["atmosphere"] = self.atmosphere
+            objects["atmosphere"] = attrs.evolve(
+                self.atmosphere, geometry=self.geometry
+            )
 
         # Process surface
-        if self.surface is not None:
-            if self.atmosphere is not None:
-                surface_width = self.atmosphere.geometry.width
-                surface_altitude = self.atmosphere.bottom_altitude
-            else:
-                surface_width = self._default_surface_width
-                surface_altitude = 0.0 * ureg.km
-
+        if self.surface is not None and isinstance(self.surface, BasicSurface):
             objects["surface"] = attrs.evolve(
                 self.surface,
-                shape=RectangleShape.surface(
-                    altitude=surface_altitude, width=surface_width
-                ),
+                shape=self.geometry.surface_shape,
             )
-
-        # Process DEM
-        if self.dem is not None:
-            objects["surface"] = self.dem
+        else:
+            objects["surface"] = self.surface
 
         objects.update(
             {
                 "illumination": self.illumination,
                 **{measure.id: measure for measure in self.measures},
                 "integrator": self.integrator,
             }
```

### Comparing `eradiate-0.23.2rc1/src/eradiate/experiments/_helpers.py` & `eradiate-0.23.2rc2/src/eradiate/experiments/_helpers.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/frame.py` & `eradiate-0.23.2rc2/src/eradiate/frame.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/kernel/__init__.pyi` & `eradiate-0.23.2rc2/src/eradiate/kernel/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/kernel/_bitmap.py` & `eradiate-0.23.2rc2/src/eradiate/kernel/_bitmap.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/kernel/_bsdf.py` & `eradiate-0.23.2rc2/src/eradiate/kernel/_bsdf.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/kernel/_kernel_dict.py` & `eradiate-0.23.2rc2/src/eradiate/kernel/_kernel_dict.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/kernel/_render.py` & `eradiate-0.23.2rc2/src/eradiate/kernel/_render.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/kernel/gridvolume.py` & `eradiate-0.23.2rc2/src/eradiate/kernel/gridvolume.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/kernel/logging.py` & `eradiate-0.23.2rc2/src/eradiate/kernel/logging.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/kernel/transform.py` & `eradiate-0.23.2rc2/src/eradiate/kernel/transform.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/notebook/__init__.py` & `eradiate-0.23.2rc2/src/eradiate/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/notebook/tutorials.py` & `eradiate-0.23.2rc2/src/eradiate/notebook/tutorials.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/pipelines/__init__.pyi` & `eradiate-0.23.2rc2/src/eradiate/pipelines/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/pipelines/_aggregate.py` & `eradiate-0.23.2rc2/src/eradiate/pipelines/_aggregate.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/pipelines/_assemble.py` & `eradiate-0.23.2rc2/src/eradiate/pipelines/_assemble.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/pipelines/_compute.py` & `eradiate-0.23.2rc2/src/eradiate/pipelines/_compute.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/pipelines/_core.py` & `eradiate-0.23.2rc2/src/eradiate/pipelines/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/pipelines/_gather.py` & `eradiate-0.23.2rc2/src/eradiate/pipelines/_gather.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/plot.py` & `eradiate-0.23.2rc2/src/eradiate/plot.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/quad.py` & `eradiate-0.23.2rc2/src/eradiate/quad.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/radprops/_afgl1986.py` & `eradiate-0.23.2rc2/src/eradiate/radprops/_afgl1986.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/radprops/_core.py` & `eradiate-0.23.2rc2/src/eradiate/radprops/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/radprops/_us76_approx.py` & `eradiate-0.23.2rc2/src/eradiate/radprops/_us76_approx.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/radprops/_util_mono.py` & `eradiate-0.23.2rc2/src/eradiate/radprops/_util_mono.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/radprops/absorption.py` & `eradiate-0.23.2rc2/src/eradiate/radprops/absorption.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/radprops/rayleigh.py` & `eradiate-0.23.2rc2/src/eradiate/radprops/rayleigh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/rng.py` & `eradiate-0.23.2rc2/src/eradiate/rng.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/atmosphere/__init__.pyi` & `eradiate-0.23.2rc2/src/eradiate/scenes/atmosphere/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/atmosphere/_core.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/atmosphere/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/atmosphere/_heterogeneous.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/atmosphere/_heterogeneous.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/atmosphere/_homogeneous.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/atmosphere/_homogeneous.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/atmosphere/_molecular_atmosphere.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/atmosphere/_molecular_atmosphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/atmosphere/_particle_dist.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/atmosphere/_particle_dist.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/atmosphere/_particle_layer.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/atmosphere/_particle_layer.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/biosphere/_core.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/biosphere/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/biosphere/_discrete.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/biosphere/_discrete.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/biosphere/_leaf_cloud.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/biosphere/_leaf_cloud.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/biosphere/_tree.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/biosphere/_tree.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/bsdfs/_black.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/bsdfs/_black.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/bsdfs/_checkerboard.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/bsdfs/_checkerboard.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/bsdfs/_core.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/bsdfs/_core.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 bsdf_factory = Factory()
 bsdf_factory.register_lazy_batch(
     [
         ("_black.BlackBSDF", "black", {}),
         ("_checkerboard.CheckerboardBSDF", "checkerboard", {}),
         ("_lambertian.LambertianBSDF", "lambertian", {}),
         ("_mqdiffuse.MQDiffuseBSDF", "mqdiffuse", {}),
+        ("_opacity_mask.OpacityMaskBSDF", "opacity_mask", {}),
         ("_rpv.RPVBSDF", "rpv", {}),
     ],
     cls_prefix="eradiate.scenes.bsdfs",
 )
 
 
 @parse_docs
```

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/bsdfs/_lambertian.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/bsdfs/_lambertian.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/bsdfs/_mqdiffuse.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/bsdfs/_mqdiffuse.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/bsdfs/_rpv.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/bsdfs/_rpv.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/core.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,15 @@
 import pint
 import pinttr
 from pinttr.util import ensure_units
 
 from .._factory import Factory
 from ..attrs import documented, parse_docs
 from ..exceptions import TraversalError
-from ..kernel import (
-    KernelDictTemplate,
-    UpdateMapTemplate,
-    UpdateParameter,
-)
+from ..kernel import KernelDictTemplate, UpdateMapTemplate, UpdateParameter
 from ..units import unit_context_config as ucc
 from ..units import unit_registry as ureg
 
 # ------------------------------------------------------------------------------
 #                           Scene element interface
 # ------------------------------------------------------------------------------
```

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/geometry.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/geometry.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/illumination/_constant.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/illumination/_constant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/illumination/_core.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/illumination/_core.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from ...attrs import documented, get_doc, parse_docs
 
 illumination_factory = Factory()
 illumination_factory.register_lazy_batch(
     [
         ("_constant.ConstantIllumination", "constant", {}),
         ("_directional.DirectionalIllumination", "directional", {}),
+        ("_astroobject.AstroObjectIllumination", "astro_object", {}),
         ("_spot.SpotIllumination", "spot", {}),
     ],
     cls_prefix="eradiate.scenes.illumination",
 )
 
 
 @parse_docs
```

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/illumination/_directional.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/illumination/_directional.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/illumination/_spot.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/illumination/_spot.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/integrators/_core.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/integrators/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/integrators/_path_tracers.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/integrators/_path_tracers.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/measure/__init__.pyi` & `eradiate-0.23.2rc2/src/eradiate/scenes/measure/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/measure/_core.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/measure/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/measure/_distant.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/measure/_distant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/measure/_distant_flux.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/measure/_distant_flux.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/measure/_hemispherical_distant.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/measure/_hemispherical_distant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/measure/_multi_distant.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/measure/_multi_distant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/measure/_multi_radiancemeter.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/measure/_multi_radiancemeter.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/measure/_perspective.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/measure/_perspective.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/measure/_radiancemeter.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/measure/_radiancemeter.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/phase/_blend.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/phase/_blend.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/phase/_core.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/phase/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/phase/_hg.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/phase/_hg.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/phase/_rayleigh.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/phase/_rayleigh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/phase/_tabulated.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/phase/_tabulated.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/shapes/_buffermesh.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/shapes/_buffermesh.py`

 * *Files 24% similar despite different names*

```diff
@@ -27,27 +27,29 @@
 
     vertices: pint.Quantity = documented(
         pinttr.field(
             validator=pinttr.validators.has_compatible_units,
             units=ucc.deferred("length"),
             kw_only=True,
         ),
-        doc="List of vertex positions. The passed list must contain a (n, 3) list"
-        "of three dimensional points.\n\nUnit-enabled field (default: ucc['length']).",
+        doc="List of vertex coordinates, specified either as a (n, 3) NumPy "
+        "array or a list of triplets.\n"
+        "\n"
+        "Unit-enabled field (default: ucc['length']).",
         type="quantity",
         init_type="array-like",
     )
 
     faces: np.ndarray = documented(
         attrs.field(
             kw_only=True,
             converter=np.array,
         ),
-        doc="List of face definitions. The passed list must contain a (n, 3) list"
-        "of three vertex indices defining triangles.",
+        doc="List of face definitions. specified either as a (n, 3) NumPy "
+        "array or a list of triplets of vertex indices.",
         type="ndarray",
         init_type="array-like",
     )
 
     @vertices.validator
     @faces.validator
     def _vertex_face_validator(self, attribute, value):
@@ -87,14 +89,33 @@
         mesh_params = mi.traverse(mesh)
         mesh_params["vertex_positions"] = vertices.ravel()
         mesh_params["faces"] = self.faces.ravel()
         mesh_params.update()
 
         return mesh
 
+    def write_ply(self, filename: str) -> None:
+        """
+        Write the mesh data to a PLY file.
+
+        Parameters
+        ----------
+        filename : str
+            Path and filename to write the mesh file into. No directories
+            are created.
+
+        Notes
+        -----
+        Vertex coordinates are expressed in kernel units and accordingly prior
+        to writing to disk. See the documentation of
+        :data:`eradiate.unit_context_kernel` and the
+        :ref:`sec-user_guide-unit_guide_user`.
+        """
+        self.instance.write_ply(filename)
+
     @property
     def params(self) -> dict[str, UpdateParameter] | None:
         if self.bsdf is None:
             return None
 
         _, params = traverse(attrs.evolve(self.bsdf, id=self._bsdf_id))
         return {f"bsdf.{k}": v for k, v in params.items()}
```

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/shapes/_core.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/shapes/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/shapes/_cuboid.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/shapes/_cuboid.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/shapes/_filemesh.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/shapes/_filemesh.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,48 +11,52 @@
 
 @parse_docs
 @attrs.define(eq=False, slots=False)
 class FileMeshShape(ShapeNode):
     """
     File based mesh shape [``file_mesh``].
 
-    This shape represents a triangulated mesh defined in a file
-    in either the PLY or OBJ format.
-    The vertex positions are assumed to be defined in kernel units.
+    This shape represents a triangulated mesh defined in a file. The OBJ and PLY
+    formats are supported.
+
+    Warnings
+    --------
+    Vertex coordinates are assumed to be defined in kernel units.
     """
 
     filename: Path = documented(
         attrs.field(converter=Path, kw_only=True),
         type="Path",
         init_type="path-like",
         doc="Path to the mesh file.",
     )
 
     @filename.validator
     def _filename_validator(self, attribute, value):
-        if value.suffix not in [".obj", ".ply"]:
+        if value.suffix not in {".obj", ".ply"}:
             raise ValueError(
                 f"while validating {attribute.name}:"
                 f"Eradiate supports mesh files only in PLY or OBJ format."
             )
 
-    @property
-    def _kernel_type(self) -> str:
-        if self.filename.suffix == ".obj":
-            return "obj"
-        elif self.filename.suffix == ".ply":
-            return "ply"
-        else:
-            raise ValueError(f"unknown mesh file type '{self.filename.suffix}'")
-
     def bbox(self) -> BoundingBox:
         # Inherit docstring
         raise NotImplementedError
 
     @property
     def template(self) -> dict:
         # Inherit docstring
+
+        if self.filename.suffix == ".obj":
+            mi_plugin = "obj"
+        elif self.filename.suffix == ".ply":
+            mi_plugin = "ply"
+        else:
+            raise ValueError(
+                f"unsupported mesh file extension '{self.filename.suffix}'"
+            )
+
         return {
-            "type": self._kernel_type,
+            "type": mi_plugin,
             "filename": str(self.filename),
             "face_normals": True,
         }
```

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/shapes/_rectangle.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/shapes/_rectangle.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/shapes/_sphere.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/shapes/_sphere.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from __future__ import annotations
 
 import attrs
+import mitsuba as mi
 import numpy as np
 import pint
 import pinttr
 from pinttr.util import ensure_units
 
 from ._core import ShapeNode
 from ..bsdfs import BSDF
 from ..core import BoundingBox
+from ... import converters
 from ...attrs import documented, parse_docs
 from ...constants import EARTH_RADIUS
 from ...units import unit_context_config as ucc
 from ...units import unit_context_kernel as uck
 from ...units import unit_registry as ureg
 
 
@@ -44,29 +46,56 @@
         ),
         doc="Sphere radius. Unit-enabled field (default: ``ucc['length']``).",
         type="quantity",
         init_type="quantity or float, optional",
         default="1.0",
     )
 
+    to_world: "mitsuba.ScalarTransform4f" = documented(
+        attrs.field(
+            converter=converters.to_mi_scalar_transform,
+            default=None,
+        ),
+        doc="Transform to scale, shift and rotate the sphere. "
+        "This transform will be prepended to the transform derived "
+        "from the center position and radius of the sphere. If, for example, a "
+        "scaling is provided here, it will multiply the sphere's radius.",
+        type="mitsuba.ScalarTransform4f or None",
+        init_type="mitsuba.ScalarTransform4f or array-like, optional",
+        default=None,
+    )
+
+    @to_world.validator
+    def to_world_validator(self, attribute, value):
+        if value is not None:
+            if not isinstance(value, mi.ScalarTransform4f):
+                raise TypeError(
+                    f"while validating '{attribute.name}': "
+                    f"'{attribute.name}' must be a mitsuba.ScalarTransform4f; "
+                    f"found: {type(value)}",
+                )
+
     @property
     def bbox(self) -> BoundingBox:
         length_units = ucc.get("length")
         offset = (
             np.full_like(self.center, self.radius.m_as(length_units)) * length_units
         )
         return BoundingBox(self.center - offset, self.center + offset)
 
     @property
     def template(self) -> dict:
-        return {
+        result = {
             "type": "sphere",
             "center": self.center.m_as(uck.get("length")),
             "radius": self.radius.m_as(uck.get("length")),
         }
+        if self.to_world is not None:
+            result["to_world"] = self.to_world
+        return result
 
     def contains(self, p: np.typing.ArrayLike, strict: bool = False) -> bool:
         """
         Test whether a point lies within the sphere.
 
         Parameters
         ----------
```

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/spectra/_air_scattering_coefficient.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/spectra/_air_scattering_coefficient.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/spectra/_core.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/spectra/_core.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,33 +48,37 @@
         -------
         callable
             Generated converter.
         """
 
         def f(value):
             if isinstance(value, (int, float, pint.Quantity)):
-                # Convert quantity-less values with dict wrapping and recursive call
+                # Convert unitless values with dict wrapping and recursive call
                 return f({"type": "uniform", "quantity": quantity, "value": value})
 
             if isinstance(value, dict):
                 # If generic spectrum is requested without a specified
                 # "quantity" field, add pre-configured quantity and attempt
                 # conversion using regular conversion protocol
                 try:
                     if (
-                        value["type"] in {"uniform", "interpolated"}
+                        value["type"] in {"uniform", "interpolated", "multi_delta"}
                         and "quantity" not in value
                     ):
                         return self.convert({**value, "quantity": quantity})
                 except KeyError:
                     # Note: A missing "type" field will also run this case, and
                     # the ill-formed dict will be correctly reported upon
                     # regular conversion
                     pass
 
+            if isinstance(value, Spectrum) and value.quantity is None:
+                # If quantity is unspecified, apply the expected quantity
+                return self.convert(attrs.evolve(value, quantity=quantity))
+
             # Regular conversion (happens if value is neither int, float nor
             # dict without "quantity" field)
             return self.convert(value)
 
         return f
 
 
@@ -118,35 +122,44 @@
     Spectrum interface.
 
     Notes
     -----
     * This class is to be used as a mixin.
     * Subclasses must implement :meth:`eval_mono`, :meth:`eval_ckd` and
       :meth:`integral`.
+
+    Warnings
+    --------
+    Leaving the ``quantity`` field unset is discouraged and permitted only to
+    allow for more convenience in some parts of the code (*e.g.* to increase the
+    flexibility of spectrum conversion protocols).
     """
 
-    quantity: PhysicalQuantity = documented(
+    quantity: PhysicalQuantity | None = documented(
         attrs.field(
-            default="dimensionless",
-            converter=PhysicalQuantity,
-            repr=lambda x: x.value.upper(),
+            default=None,
+            converter=attrs.converters.optional(PhysicalQuantity),
+            repr=lambda x: "None" if x is None else x.value.upper(),
         ),
         doc="Physical quantity which the spectrum represents. The specified "
         "quantity must be one which varies with wavelength. "
         "See :meth:`.PhysicalQuantity.spectrum` for allowed values.\n"
         "\n"
         "Child classes should implement value units validation and conversion "
         "based on ``quantity``.",
-        type=":class:`.PhysicalQuantity`",
-        init_type=":class:`.PhysicalQuantity` or str",
-        default="dimensionless",
+        type=".PhysicalQuantity or None",
+        init_type=".PhysicalQuantity or str, optional",
+        default="None",
     )
 
     @quantity.validator
     def _quantity_validator(self, attribute, value):
+        if value is None:
+            return
+
         if value not in PhysicalQuantity.spectrum():
             raise ValueError(
                 f"while validating {attribute.name}: "
                 f"got value '{value}', expected one of {str(PhysicalQuantity.spectrum())}"
             )
 
     @singledispatchmethod
@@ -233,16 +246,25 @@
             Integration interval's lower bound.
 
         wmax : quantity
             Integration interval's upper bound.
 
         Returns
         -------
-        value : quantity
-            Computed integral value.
+        value : quantity or ndarray
+            Computed integral value, in units consistent with the specified
+            quantity.
+
+        Warnings
+        --------
+        If the ``quantity`` field is unset (*i.e.* left to its default value
+        ``None``), the output of this method will inherit the units of value
+        fields (the actual policy depends on the implementation, and unitless
+        values are intepreted as dimnesionless). Note that leaving the
+        ``quantity`` field unset is discouraged.
         """
         raise NotImplementedError
 
     @singledispatchmethod
     def select_in(self, spectral_set) -> BinSet | WavelengthSet:
         """
         Select a subset of a spectral set.
```

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/spectra/_interpolated.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/spectra/_interpolated.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,19 +15,20 @@
 from ...attrs import documented, parse_docs
 from ...kernel import InitParameter, UpdateParameter
 from ...spectral.ckd import BinSet
 from ...spectral.mono import WavelengthSet
 from ...units import PhysicalQuantity, to_quantity
 from ...units import unit_context_config as ucc
 from ...units import unit_context_kernel as uck
+from ...units import unit_registry as ureg
 from ...util.misc import where_consecutive_zeros, where_non_significant_zeros
 
 
 @parse_docs
-@attrs.define(eq=False, slots=False)
+@attrs.define(eq=False, slots=False, init=False)
 class InterpolatedSpectrum(Spectrum):
     """
     Linearly interpolated spectrum [``interpolated``].
 
     .. admonition:: Class method constructors
 
        .. autosummary::
@@ -66,27 +67,34 @@
             raise ValueError("wavelengths must be monotonically increasing")
 
     values: pint.Quantity = documented(
         attrs.field(
             converter=converters.on_quantity(np.atleast_1d),
             kw_only=True,
         ),
-        doc="Uniform spectrum value. If a float is passed, it is automatically "
-        "converted to appropriate default configuration units. "
-        "If a :class:`~pint.Quantity` is passed, units are checked for "
-        "consistency.",
+        doc="Spectrum values. If a quantity is passed, units are "
+        "checked for consistency. If a unitless array is passed, it is "
+        "automatically converted to appropriate default configuration units, "
+        "depending on the value of the ``quantity`` field. If no quantity is "
+        "specified, this field can be a unitless value.",
         type="quantity",
         init_type="array-like",
     )
 
     @values.validator
     def _values_validator(self, attribute, value):
-        if isinstance(value, pint.Quantity):
-            expected_units = ucc.get(self.quantity)
+        if self.quantity is not None:
+            if not isinstance(self.values, pint.Quantity):
+                raise ValueError(
+                    f"while validating '{attribute.name}': expected a Pint "
+                    "quantity compatible with quantity field value "
+                    f"'{self.quantity}', got a unitless value instead"
+                )
 
+            expected_units = ucc.get(self.quantity)
             if not pinttr.util.units_compatible(expected_units, value.units):
                 raise pinttr.exceptions.UnitsError(
                     value.units,
                     expected_units,
                     extra_msg=f"while validating '{attribute.name}', got units "
                     f"'{value.units}' incompatible with quantity {self.quantity} "
                     f"(expected '{expected_units}')",
@@ -113,21 +121,32 @@
         if self.wavelengths.shape != self.values.shape:
             raise ValueError(
                 f"while validating '{attribute.name}': 'wavelengths' and 'values' "
                 f"must have the same shape, got {self.wavelengths.shape} and "
                 f"{self.values.shape}"
             )
 
-    def __attrs_post_init__(self):
-        self.update()
+    def __init__(
+        self,
+        id: str | None = None,
+        quantity: PhysicalQuantity | str | None = None,
+        *,
+        wavelengths: np.typing.ArrayLike,
+        values: np.typing.ArrayLike,
+    ):
+        # If a quantity is set and a unitless value is passed, it is
+        # automatically applied appropriate units
+        if quantity is not None and not isinstance(values, pint.Quantity):
+            values = pinttr.util.ensure_units(values, ucc.get(quantity))
 
-    def update(self):
-        # Apply appropriate units to values field
-        self.values = pinttr.util.ensure_units(self.values, ucc.get(self.quantity))
+        self.__attrs_init__(
+            id=id, quantity=quantity, wavelengths=wavelengths, values=values
+        )
 
+    def update(self):
         # Sort by increasing wavelength (required by numpy.interp in eval_mono)
         idx = np.argsort(self.wavelengths)
         self.wavelengths = self.wavelengths[idx]
         self.values = self.values[idx]
 
     @classmethod
     def from_dataarray(
@@ -157,15 +176,15 @@
         Notes
         -----
 
         * Expected data format:
 
           **Coordinates (\\* means also dimension)**
 
-          * ``*w`` (float): wavelength in nm.
+          * ``*w`` (float): wavelength (units specified as a ``units`` attribute).
 
           **Metadata**
 
           * ``quantity`` (str): physical quantity which the data describes (see
             :meth:`.PhysicalQuantity.spectrum` for allowed values), optional.
           * ``units`` (str): units of spectrum values (must be consistent with
             ``quantity``).
@@ -191,14 +210,16 @@
     def eval_mono(self, w: pint.Quantity) -> pint.Quantity:
         return np.interp(w, self.wavelengths, self.values, left=0.0, right=0.0)
 
     def eval_ckd(self, w: pint.Quantity, g: float) -> pint.Quantity:
         return self.eval_mono(w=w)
 
     def integral(self, wmin: pint.Quantity, wmax: pint.Quantity) -> pint.Quantity:
+        # Inherit docstring
+
         # Collect spectral coordinates
         wavelength_units = self.wavelengths.units
         s_w = self.wavelengths.m
         s_wmin = s_w.min()
         s_wmax = s_w.max()
 
         # Select all spectral mesh vertices between wmin and wmax, as well as
@@ -219,19 +240,21 @@
 
         try:
             w.insert(w.index(s_wmax) + 1, s_wmax + eps)
         except ValueError:
             pass
 
         # Evaluate spectrum at wavelengths
-        w *= wavelength_units
-        interp = self.eval_mono(w)
+        interp = self.eval_mono(w * wavelength_units)
 
         # Compute integral
-        return np.trapz(interp, w)
+        integral = np.trapz(interp, w)
+
+        # Apply units
+        return integral * ureg.dimensionless * wavelength_units
 
     @property
     def template(self) -> dict:
         # Inherit docstring
 
         return {
             "type": "uniform",
@@ -263,15 +286,15 @@
         Returns
         -------
         Interval
             Wavelength interval.
         """
         wunits = self.wavelengths.units
         wm = self.wavelengths.m
-        vm = self.values.m
+        vm = self.values.m if isinstance(self.values, pint.Quantity) else self.values
 
         # 1. strip non significant zeros
         nsz = where_non_significant_zeros(vm)
         values = vm[~nsz]
         wavelengths = wm[~nsz]
 
         # 2. split where consecutive zeros are located
@@ -287,30 +310,29 @@
             nsz = where_non_significant_zeros(v)
             values_cleaned.append(v[~nsz])
             wavelengths_cleaned.append(w[~nsz])
 
         # 4. Determine interval
         intervals = []
         for w in wavelengths_cleaned:
-
             # lower and upper bound of current sub-interval
             wlower = w[0]
             wupper = w[-1]
 
             # corresponding indices
             ilower = np.where(wm == wlower)
             iupper = np.where(wm == wupper)
 
             # create sub-interval
             interval = P.open(wlower * wunits, wupper * wunits)
 
             # update left and right boundaries if necessary
-            if self.values.m[ilower] != 0:
+            if vm[ilower] != 0:
                 interval = interval.replace(left=P.CLOSED)
-            if self.values.m[iupper] != 0:
+            if vm[iupper] != 0:
                 interval = interval.replace(right=P.CLOSED)
 
             intervals.append(interval)
 
         # union of all intervals
         interval = reduce(lambda i1, i2: i1 | i2, intervals[0:], intervals[0])
```

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/spectra/_multi_delta.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/spectra/_multi_delta.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/spectra/_solar_irradiance.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/spectra/_solar_irradiance.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/spectra/_uniform.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/spectra/_uniform.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,65 +4,96 @@
 import numpy as np
 import pint
 import pinttr
 
 from ._core import Spectrum
 from ...attrs import documented, parse_docs
 from ...kernel import InitParameter, UpdateParameter
+from ...units import PhysicalQuantity
 from ...units import unit_context_config as ucc
 from ...units import unit_context_kernel as uck
+from ...units import unit_registry as ureg
 
 
 @parse_docs
-@attrs.define(eq=False, slots=False)
+@attrs.define(eq=False, slots=False, init=False)
 class UniformSpectrum(Spectrum):
     """
     Uniform spectrum [``uniform``] (*i.e.* constant vs wavelength).
     """
 
     value: pint.Quantity = documented(
         attrs.field(
             converter=lambda x: float(x) if isinstance(x, int) else x,
             repr=lambda x: f"{x:~P}",
             kw_only=True,
         ),
-        doc="Uniform spectrum value. If a float is passed, it is automatically "
-        "converted to appropriate configuration default units. Integer values "
-        "are also converted to float.",
-        type=":class:`~pint.Quantity`",
-        init_type="float or :class:`~pint.Quantity` or int",
+        doc="Uniform spectrum value. If a quantity is passed, units are "
+        "checked for consistency. If a unitless value is passed, it is "
+        "automatically converted to appropriate configuration default units, "
+        "depending on the value of the ``quantity`` field. Integer values "
+        "are converted to float. If no quantity is specified, this field must be"
+        "a unitless value.",
+        type="quantity",
+        init_type="quantity or float or int",
     )
 
     @value.validator
     def _value_validator(self, attribute, value):
+        # If a quantity is passed, it must match the quantity field
         if isinstance(value, pint.Quantity):
-            expected_units = ucc.get(self.quantity)
-
-            if not pinttr.util.units_compatible(expected_units, value.units):
-                raise pinttr.exceptions.UnitsError(
-                    value.units,
-                    expected_units,
-                    extra_msg=f"while validating {attribute.name}, got units "
-                    f"'{value.units}' incompatible with quantity {self.quantity} "
-                    f"(expected '{expected_units}')",
+            if self.quantity is None:
+                raise ValueError(
+                    f"while validating {attribute.name}, got a Pint quantity, "
+                    "incompatible with 'quantity' field set to None; "
+                    "please provide a unitless value"
                 )
+            else:
+                expected_units = ucc.get(self.quantity)
+
+                if not pinttr.util.units_compatible(expected_units, value.units):
+                    raise pinttr.exceptions.UnitsError(
+                        value.units,
+                        expected_units,
+                        extra_msg=f"while validating {attribute.name}, got units "
+                        f"'{value.units}' incompatible with quantity {self.quantity} "
+                        f"(expected '{expected_units}')",
+                    )
+
+    def __init__(
+        self,
+        id: str | None = None,
+        quantity: PhysicalQuantity | str | None = None,
+        *,
+        value: int | float | pint.Quantity,
+    ):
+        # If a quantity is set and a unitless value is passed, it is
+        # automatically applied appropriate units
+        if quantity is not None and not isinstance(value, pint.Quantity):
+            value = pinttr.util.ensure_units(value, ucc.get(quantity))
 
-    def update(self):
-        self.value = pinttr.util.ensure_units(self.value, ucc.get(self.quantity))
+        self.__attrs_init__(id=id, quantity=quantity, value=value)
 
     def eval_mono(self, w: pint.Quantity) -> pint.Quantity:
         return np.full_like(w, self.value.m) * self.value.units
 
     def eval_ckd(self, w: pint.Quantity, g: float) -> pint.Quantity:
         return self.eval_mono(w=w)
 
     def integral(self, wmin: pint.Quantity, wmax: pint.Quantity) -> pint.Quantity:
-        wmin = pinttr.util.ensure_units(wmin, ucc.get("wavelength"))
-        wmax = pinttr.util.ensure_units(wmax, ucc.get("wavelength"))
-        return self.value * (wmax - wmin)
+        # Convert bounds to unitless values
+        wavelength_units = wmin.units
+        wmin = wmin.magnitude
+        wmax = wmax.m_as(wavelength_units)
+
+        # Compute integral
+        integral = self.value * (wmax - wmin)
+
+        # Apply units
+        return integral * ureg.dimensionless * wavelength_units
 
     @property
     def template(self) -> dict:
         # Inherit docstring
 
         return {
             "type": "uniform",
```

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/surface/_basic.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/surface/_basic.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/surface/_central_patch.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/surface/_central_patch.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/scenes/surface/_core.py` & `eradiate-0.23.2rc2/src/eradiate/scenes/surface/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/spectral/ckd.py` & `eradiate-0.23.2rc2/src/eradiate/spectral/ckd.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/spectral/index.py` & `eradiate-0.23.2rc2/src/eradiate/spectral/index.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/spectral/mono.py` & `eradiate-0.23.2rc2/src/eradiate/spectral/mono.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/srf_tools.py` & `eradiate-0.23.2rc2/src/eradiate/srf_tools.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/test_tools/plugin.py` & `eradiate-0.23.2rc2/src/eradiate/test_tools/plugin.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/test_tools/regression.py` & `eradiate-0.23.2rc2/src/eradiate/test_tools/regression.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/test_tools/types.py` & `eradiate-0.23.2rc2/src/eradiate/test_tools/types.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from ..scenes.core import CompositeSceneElement, NodeSceneElement, Scene, traverse
 
 
 def check_scene_element(
     instance: NodeSceneElement | CompositeSceneElement,
     mi_cls=None,
     ctx: KernelContext = None,
+    drop_parameters: bool = True,
 ) -> MitsubaObjectWrapper:
     """
     Perform kernel dictionary checks on a scene element.
 
     This function checks if the scene element can produce a valid kernel
     dictionary template, as well as an appropriate parameter table.
 
@@ -31,14 +32,18 @@
         Mitsuba class the node scene element expands to. Must be set if
         `instance` is a :class:`.NodeSceneElement`; ignored otherwise.
 
     ctx : .KernelContext, optional
         If provided, the kernel dictionary context to use. Otherwise, a default
         context is created.
 
+    drop_parameters : bool, default: True
+        If ``True``, the Mitsuba scene parameter table will be stripped off from
+        untracked parameters.
+
     Returns
     -------
     mi_obj : :class:`mitsuba.Object`
         Mitsuba object the scene element was expanded to. See notes for details.
 
     mi_params : dict
         Parameter table of the Mitsuba objects generated by the tested scene
@@ -90,8 +95,12 @@
         except KeyError as e:
             pytest.fail(
                 reason=f"could not set parameter, got KeyError: {e}\n{mi_params = }"
             )
 
     mi_params.update()
 
+    # Drop untracked parameters (this will detect param lookup failures)
+    if drop_parameters:
+        mi_wrapper.drop_parameters()
+
     return mi_wrapper
```

### Comparing `eradiate-0.23.2rc1/src/eradiate/test_tools/util.py` & `eradiate-0.23.2rc2/src/eradiate/test_tools/util.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/thermoprops/afgl_1986.py` & `eradiate-0.23.2rc2/src/eradiate/thermoprops/afgl_1986.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/thermoprops/us76.py` & `eradiate-0.23.2rc2/src/eradiate/thermoprops/us76.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/thermoprops/util.py` & `eradiate-0.23.2rc2/src/eradiate/thermoprops/util.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/units.py` & `eradiate-0.23.2rc2/src/eradiate/units.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/util/deprecation.py` & `eradiate-0.23.2rc2/src/eradiate/util/deprecation.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/util/misc.py` & `eradiate-0.23.2rc2/src/eradiate/util/misc.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/util/numpydoc.py` & `eradiate-0.23.2rc2/src/eradiate/util/numpydoc.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/util/sys_info.py` & `eradiate-0.23.2rc2/src/eradiate/util/sys_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,12 +92,11 @@
     print("System")
     print(f"  CPU: {sys_info['cpu_info']}")
     print(f"  OS: {sys_info['os']}")
     print(f"  Python: {sys_info['python']}")
 
     print("\nVersions")
     print(f"  drjit {sys_info['drjit_version']}")
-    print(f"  mitsuba {sys_info['mitsuba_version']}")
-    print(f"  eradiate-mitsuba {sys_info['eradiate_mitsuba_version']}")
+    print(f"  eradiate-mitsuba {sys_info['eradiate_mitsuba_version']} (based on mitsuba {sys_info['mitsuba_version']})")
 
     print("\nMitsuba variants")
     print("\n".join([f"  {variant}" for variant in mi.variants()]))
```

### Comparing `eradiate-0.23.2rc1/src/eradiate/validators.py` & `eradiate-0.23.2rc2/src/eradiate/validators.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/warp.py` & `eradiate-0.23.2rc2/src/eradiate/warp.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/xarray/_accessors.py` & `eradiate-0.23.2rc2/src/eradiate/xarray/_accessors.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/xarray/_helpers.py` & `eradiate-0.23.2rc2/src/eradiate/xarray/_helpers.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate/xarray/interp.py` & `eradiate-0.23.2rc2/src/eradiate/xarray/interp.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/src/eradiate.egg-info/PKG-INFO` & `eradiate-0.23.2rc2/src/eradiate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 Metadata-Version: 2.1
 Name: eradiate
-Version: 0.23.2rc1
+Version: 0.23.2rc2
 Summary: A radiative transfer model for the Earth observation community
 Author: The Eradiate Team
 Maintainer: The Eradiate Team
 License: LGPLv3
 Project-URL: changelog, https://github.com/eradiate/eradiate/CHANGELOG.md
 Project-URL: documentation, https://eradiate.readthedocs.io
 Project-URL: repository, https://github.com/eradiate/eradiate
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: docs
 Provides-Extra: recommended
-Provides-Extra: tests
-Provides-Extra: optional
-Provides-Extra: production
 License-File: LICENSE
 
 ![Eradiate logo](docs/fig/eradiate-logo.svg "Eradiate — A new-generation radiative transfer simulation package")
 
 # Eradiate Radiative Transfer Model
 
 [![docs][rtd-badge]][rtd-url]
```

### Comparing `eradiate-0.23.2rc1/src/eradiate.egg-info/SOURCES.txt` & `eradiate-0.23.2rc2/src/eradiate.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -94,21 +94,20 @@
 docs/fig/diagrams/package.drawio
 docs/rst/bibliography.rst
 docs/rst/contributing.rst
 docs/rst/dependencies.rst
 docs/rst/maintainer_guide.rst
 docs/rst/developer_guide/design_atmosphere.rst
 docs/rst/developer_guide/factory_guide.rst
+docs/rst/developer_guide/getting_started.rst
 docs/rst/developer_guide/index.rst
 docs/rst/developer_guide/lazy_loading.rst
 docs/rst/developer_guide/radiometric_kernel_interface.rst
 docs/rst/developer_guide/scene_generator.rst
-docs/rst/getting_started/index.rst
-docs/rst/getting_started/install.rst
-docs/rst/getting_started/update.rst
+docs/rst/developer_guide/update.rst
 docs/rst/reference_api/attrs.rst
 docs/rst/reference_api/config.rst
 docs/rst/reference_api/constants.rst
 docs/rst/reference_api/contexts.rst
 docs/rst/reference_api/converters.rst
 docs/rst/reference_api/data.rst
 docs/rst/reference_api/eradiate_core.rst
@@ -135,14 +134,15 @@
 docs/rst/reference_api/validators.rst
 docs/rst/reference_api/warp.rst
 docs/rst/reference_api/xarray.rst
 docs/rst/reference_plugins/index.rst
 docs/rst/user_guide/basic_concepts.rst
 docs/rst/user_guide/conventions.rst
 docs/rst/user_guide/index.rst
+docs/rst/user_guide/install.rst
 docs/rst/user_guide/onedim_experiment.rst
 docs/rst/user_guide/package_structure.rst
 docs/rst/user_guide/spectral_discretization.rst
 docs/rst/user_guide/unit_guide_user.rst
 docs/rst/user_guide/atmosphere/absorption.rst
 docs/rst/user_guide/atmosphere/heterogeneous.rst
 docs/rst/user_guide/atmosphere/homogeneous.rst
@@ -167,38 +167,61 @@
 docs/rst/user_guide/data/fig/p_interp_rerr_histo_65349.png
 docs/rst/user_guide/data/fig/pt_points.png
 docs/rst/user_guide/data/fig/w_interp_rerr_histo_101325.png
 docs/src/CHANGELOG.md
 docs/src/reference_cli.md
 requirements/check_conda_env.py
 requirements/copy_envvars.py
-requirements/dev.in
-requirements/dev.txt
-requirements/docs.in
-requirements/docs.txt
-requirements/environment-dev.yml
-requirements/environment-linux-64.lock
-requirements/environment-minimal.yml
-requirements/environment-optional.yml
-requirements/environment-osx-64.lock
-requirements/environment-production.yml
-requirements/environment-recommended.yml
 requirements/environment.in
 requirements/layered.yml
-requirements/main.in
-requirements/main.txt
 requirements/make_conda_env.py
 requirements/make_pip_in_files.py
-requirements/optional.in
-requirements/optional.txt
-requirements/production.in
-requirements/production.txt
-requirements/recommended.in
-requirements/tests.in
-requirements/tests.txt
+requirements/conda/environment-dependencies-linux-64.lock
+requirements/conda/environment-dependencies-osx-64.lock
+requirements/conda/environment-dependencies.dot
+requirements/conda/environment-dependencies.yml
+requirements/conda/environment-dev-linux-64.lock
+requirements/conda/environment-dev-osx-64.lock
+requirements/conda/environment-dev.dot
+requirements/conda/environment-dev.yml
+requirements/conda/environment-docs-linux-64.lock
+requirements/conda/environment-docs-osx-64.lock
+requirements/conda/environment-docs.dot
+requirements/conda/environment-docs.yml
+requirements/conda/environment-main-linux-64.lock
+requirements/conda/environment-main-osx-64.lock
+requirements/conda/environment-main.dot
+requirements/conda/environment-main.yml
+requirements/conda/environment-optional-linux-64.lock
+requirements/conda/environment-optional-osx-64.lock
+requirements/conda/environment-optional.dot
+requirements/conda/environment-optional.yml
+requirements/conda/environment-recommended-linux-64.lock
+requirements/conda/environment-recommended-osx-64.lock
+requirements/conda/environment-recommended.dot
+requirements/conda/environment-recommended.yml
+requirements/conda/environment-tests-linux-64.lock
+requirements/conda/environment-tests-osx-64.lock
+requirements/conda/environment-tests.dot
+requirements/conda/environment-tests.yml
+requirements/conda/layer_graph.dot
+requirements/pip/dependencies.in
+requirements/pip/dependencies.txt
+requirements/pip/dev.in
+requirements/pip/dev.txt
+requirements/pip/docs.in
+requirements/pip/docs.txt
+requirements/pip/main.in
+requirements/pip/main.txt
+requirements/pip/optional.in
+requirements/pip/optional.txt
+requirements/pip/recommended.in
+requirements/pip/recommended.txt
+requirements/pip/tests.in
+requirements/pip/tests.txt
 src/eradiate/__init__.py
 src/eradiate/__init__.pyi
 src/eradiate/_config.py
 src/eradiate/_factory.py
 src/eradiate/_mode.py
 src/eradiate/_version.py
 src/eradiate/attrs.py
@@ -294,17 +317,19 @@
 src/eradiate/scenes/bsdfs/__init__.py
 src/eradiate/scenes/bsdfs/__init__.pyi
 src/eradiate/scenes/bsdfs/_black.py
 src/eradiate/scenes/bsdfs/_checkerboard.py
 src/eradiate/scenes/bsdfs/_core.py
 src/eradiate/scenes/bsdfs/_lambertian.py
 src/eradiate/scenes/bsdfs/_mqdiffuse.py
+src/eradiate/scenes/bsdfs/_opacity_mask.py
 src/eradiate/scenes/bsdfs/_rpv.py
 src/eradiate/scenes/illumination/__init__.py
 src/eradiate/scenes/illumination/__init__.pyi
+src/eradiate/scenes/illumination/_astroobject.py
 src/eradiate/scenes/illumination/_constant.py
 src/eradiate/scenes/illumination/_core.py
 src/eradiate/scenes/illumination/_directional.py
 src/eradiate/scenes/illumination/_spot.py
 src/eradiate/scenes/integrators/__init__.py
 src/eradiate/scenes/integrators/__init__.pyi
 src/eradiate/scenes/integrators/_core.py
@@ -440,14 +465,15 @@
 tests/01_eradiate/01_unit/scenes/bsdfs/__init__.py
 tests/01_eradiate/01_unit/scenes/bsdfs/test_black.py
 tests/01_eradiate/01_unit/scenes/bsdfs/test_checkerboard.py
 tests/01_eradiate/01_unit/scenes/bsdfs/test_lambertian.py
 tests/01_eradiate/01_unit/scenes/bsdfs/test_mqdiffuse.py
 tests/01_eradiate/01_unit/scenes/bsdfs/test_rpv.py
 tests/01_eradiate/01_unit/scenes/illumination/__init__.py
+tests/01_eradiate/01_unit/scenes/illumination/test_astroobject.py
 tests/01_eradiate/01_unit/scenes/illumination/test_constant.py
 tests/01_eradiate/01_unit/scenes/illumination/test_directional.py
 tests/01_eradiate/01_unit/scenes/illumination/test_spot.py
 tests/01_eradiate/01_unit/scenes/integrators/__init__.py
 tests/01_eradiate/01_unit/scenes/integrators/test_path_tracers.py
 tests/01_eradiate/01_unit/scenes/measure/__init__.py
 tests/01_eradiate/01_unit/scenes/measure/test_distant_flux.py
```

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/test_blind_directory.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/test_blind_directory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/test_blind_online.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/test_blind_online.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/test_core.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/test_datasets.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/test_datasets.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/test_multi.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/test_multi.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/test_safe_directory.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/test_safe_directory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/test_safe_online.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/data/test_safe_online.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/experiments/test_atmosphere.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/experiments/test_atmosphere.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,17 @@
 
     # With an atmosphere
     exp = AtmosphereExperiment(
         geometry={"type": "plane_parallel", "width": 42.0, "width_units": "km"},
         atmosphere=HomogeneousAtmosphere(),
         measures={"type": "distant"},
     )
-    mi_wrapper = check_scene_element(exp.scene, mi.Scene)
+    mi_wrapper = check_scene_element(
+        exp.scene, mi.Scene, drop_parameters=False
+    )  # Do not drop untracked parameters: we want to check the `to_world` transform
     # -- Surface width is inherited from geometry
     assert np.allclose(
         mi_wrapper.parameters["surface_shape.to_world"].matrix,
         mi.ScalarTransform4f.scale([21000, 21000, 1]).matrix,
     )
     # -- Atmosphere is part of the scene
     assert "shape_atmosphere" in set(shape.id() for shape in mi_wrapper.obj.shapes())
@@ -106,15 +108,15 @@
         surface={"type": "lambertian"},
         measures=[
             {"type": "distant", "id": "distant_measure"},
             {"type": "radiancemeter", "origin": [1, 0, 0], "id": "radiancemeter"},
         ],
     )
     # -- Surface width has default value
-    mi_wrapper = check_scene_element(exp.scene, mi.Scene)
+    mi_wrapper = check_scene_element(exp.scene, mi.Scene, drop_parameters=False)
     assert np.allclose(
         mi_wrapper.parameters["surface_shape.to_world"].matrix,
         mi.ScalarTransform4f.scale([5e8, 5e8, 1]).matrix,
     )
     # -- Atmosphere is not part of the scene
     assert "shape_atmosphere" not in set(
         shape.id() for shape in mi_wrapper.obj.shapes()
```

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/experiments/test_canopy.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/experiments/test_canopy.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,17 @@
             lai=0.5,  # This very low value ensures fast object initialization
             leaf_radius=0.1 * ureg.m,
             l_horizontal=10.0 * ureg.m,
             l_vertical=2.0 * ureg.m,
             padding=padding,
         )
     )
-    mi_wrapper = check_scene_element(exp.scene, mi.Scene)
+    mi_wrapper = check_scene_element(
+        exp.scene, mi.Scene, drop_parameters=False
+    )  # Don't drop untracked params at this stage: we want to check the surface transform
 
     assert np.allclose(
         mi_wrapper.parameters["surface_shape.to_world"].transform_affine(
             mi.Point3f(1, -1, 0)
         ),
         [5 * (2 * padding + 1), -5 * (2 * padding + 1), 0],
     )
```

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/experiments/test_canopy_atmosphere.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/experiments/test_canopy_atmosphere.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,15 +96,17 @@
         ),
         measures=[
             {"type": "distant", "id": "distant_measure"},
             {"type": "radiancemeter", "origin": [1, 0, 0], "id": "radiancemeter"},
         ],
     )
 
-    mi_wrapper = check_scene_element(exp.scene, mi.Scene)
+    mi_wrapper = check_scene_element(
+        exp.scene, mi.Scene, drop_parameters=False
+    )  # Do not drop untracked parameters: we want to check the surface transform
     assert np.allclose(
         mi_wrapper.parameters["surface_shape.to_world"].transform_affine(
             mi.Point3f(1, -1, 0)
         ),
         [5 * (2 * padding + 1), -5 * (2 * padding + 1), 0],
     )
 
@@ -120,15 +122,17 @@
             leaf_radius=0.1 * ureg.m,
             l_horizontal=10.0 * ureg.m,
             l_vertical=2.0 * ureg.m,
             padding=padding,
         ),
     )
 
-    mi_wrapper = check_scene_element(exp.scene, mi.Scene)
+    mi_wrapper = check_scene_element(
+        exp.scene, mi.Scene, drop_parameters=False
+    )  # Do not drop untracked parameters: we want to check the surface transform
     assert np.allclose(
         mi_wrapper.parameters["surface_shape.to_world"].matrix,
         mi.ScalarTransform4f.scale([21000, 21000, 1]).matrix,
     )
 
 
 @pytest.mark.slow
@@ -154,15 +158,17 @@
     )
 
     expected = (
         mi.ScalarTransform3f.scale([1400, 1400])
         @ mi.ScalarTransform3f.translate([-0.499642857, -0.499642857])
     ).matrix
 
-    mi_wrapper = check_scene_element(exp.scene, mi.Scene)
+    mi_wrapper = check_scene_element(
+        exp.scene, mi.Scene, drop_parameters=False
+    )  # Do not drop untracked parameters: we want to check the surface texture's uv transform
     result = mi_wrapper.parameters["surface_bsdf.weight.to_uv"].matrix
 
     np.testing.assert_allclose(expected, result)
 
 
 @pytest.mark.slow
 def test_canopy_atmosphere_experiment_real_life(mode_mono):
```

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/experiments/test_core.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/experiments/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/experiments/test_dem.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/experiments/test_dem.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import mitsuba as mi
 import numpy as np
 import pytest
+import xarray as xr
 
 import eradiate
 from eradiate import unit_registry as ureg
+from eradiate.constants import EARTH_RADIUS
 from eradiate.experiments import DEMExperiment
 from eradiate.scenes.atmosphere import (
     HeterogeneousAtmosphere,
     HomogeneousAtmosphere,
     MolecularAtmosphere,
 )
-from eradiate.scenes.bsdfs import LambertianBSDF
+from eradiate.scenes.geometry import PlaneParallelGeometry
 from eradiate.scenes.measure import MultiDistantMeasure
 from eradiate.scenes.spectra import MultiDeltaSpectrum
-from eradiate.scenes.surface import DEMSurface
+from eradiate.scenes.surface import DEMSurface, mesh_from_dem
 from eradiate.test_tools.types import check_scene_element
 
 
 def test_dem_experiment_construct_default(modes_all_double):
     """
     DEMExperiment initialises with default params in all modes
     """
@@ -77,18 +79,20 @@
         surface={"type": "lambertian"},
         measures=[
             {"type": "distant", "id": "distant_measure"},
             {"type": "radiancemeter", "origin": [1, 0, 0], "id": "radiancemeter"},
         ],
     )
     # -- Surface has default value
-    mi_wrapper = check_scene_element(exp.scene, mi.Scene, ctx=exp.context_init)
+    mi_wrapper = check_scene_element(
+        exp.scene, mi.Scene, ctx=exp.context_init, drop_parameters=False
+    )  # Do not drop untracked parameters: we want to check the surface transform
     np.testing.assert_allclose(
         mi_wrapper.parameters["surface_shape.to_world"].matrix,
-        mi.ScalarTransform4f.scale([500, 500, 1]).matrix,
+        mi.ScalarTransform4f.scale([5e8, 5e8, 1]).matrix,
     )
     # -- Atmosphere is not in kernel dictionary
     assert {shape.id() for shape in mi_wrapper.obj.shapes()} == {"surface_shape"}
 
     # -- Measures get no external medium assigned
     assert all(sensor.medium() is None for sensor in mi_wrapper.obj.sensors())
 
@@ -211,28 +215,42 @@
         expected_coords |= {"bin", "bin_wmin", "bin_wmax"}
     assert set(results["irradiance"].coords) == expected_coords
 
     # We just check that we record something as expected
     assert np.all(results["radiance"].data > 0.0)
 
 
-def test_dem_experiment_warn_targeting_dem(modes_all_double):
+def test_dem_experiment_warn_targeting_dem(modes_all_double, tmpdir):
     """
-    Test that Eradiate raises a warning, when the measure target is a point and a DEM is defined in the scene.
+    Test that the DEMExperiment constructor raises a warning when the measure
+    target is a point and a DEM is defined in the scene.
     """
 
+    da = xr.DataArray(
+        data=np.zeros((10, 10)),
+        dims=["x", "y"],
+        coords={
+            "x": (["x"], np.linspace(-10, 20, 10), {"units": "kilometer"}),
+            "y": (["y"], np.linspace(-30, 40, 10), {"units": "kilometer"}),
+        },
+        attrs={"units": "meter"},
+    )
+
+    mesh, lat, lon = mesh_from_dem(
+        da, geometry="plane_parallel", planet_radius=EARTH_RADIUS
+    )
+
     with pytest.warns(UserWarning, match="uses a point target"):
         DEMExperiment(
-            dem=DEMSurface.from_analytical(
-                elevation_function=lambda x, y: 1,
-                x_length=1 * ureg.m,
-                x_steps=10,
-                y_length=1 * ureg.m,
-                y_steps=10,
-                bsdf=LambertianBSDF(),
+            surface=DEMSurface.from_mesh(
+                id="terrain",
+                mesh=mesh,
+                lat=lat,
+                lon=lon,
+                geometry=PlaneParallelGeometry(),
             ),
             measures=[
                 {
                     "type": "distant",
                     "id": "distant_measure",
                     "target": {"type": "point", "xyz": [1, 1, 0]},
                 },
```

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/experiments/test_helpers.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/experiments/test_helpers.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/kernel/test_gridvolume.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/kernel/test_gridvolume.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/kernel/test_kernel_dict.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/kernel/test_kernel_dict.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/kernel/test_logging.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/kernel/test_logging.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/kernel/test_render.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/kernel/test_render.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/kernel/test_transform.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/kernel/test_transform.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/pipelines/conftest.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/pipelines/conftest.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/pipelines/test_aggregate.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/pipelines/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/pipelines/test_assemble.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/pipelines/test_assemble.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/pipelines/test_compute.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/pipelines/test_compute.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/pipelines/test_core.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/pipelines/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/pipelines/test_gather.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/pipelines/test_gather.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/radprops/test_absorption.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/radprops/test_absorption.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/radprops/test_afgl_1986.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/radprops/test_afgl_1986.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/radprops/test_rayleigh_scattering.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/radprops/test_rayleigh_scattering.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/radprops/test_us76_approx.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/radprops/test_us76_approx.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/radprops/test_zgrid.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/radprops/test_zgrid.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_heterogeneous.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/atmosphere/test_heterogeneous.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_homogeneous.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/atmosphere/test_homogeneous.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_molecular_atmosphere.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/atmosphere/test_molecular_atmosphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_dist.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_dist.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_layer.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_layer.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_core.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/biosphere/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_discrete.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/biosphere/test_discrete.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_leaf_cloud.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/biosphere/test_leaf_cloud.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_abstract.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_abstract.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_mesh.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_mesh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_checkerboard.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/bsdfs/test_checkerboard.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_lambertian.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/bsdfs/test_lambertian.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_mqdiffuse.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/bsdfs/test_mqdiffuse.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_rpv.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/bsdfs/test_rpv.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/illumination/test_constant.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/illumination/test_constant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/illumination/test_directional.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/illumination/test_directional.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/illumination/test_spot.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/illumination/test_spot.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/integrators/test_path_tracers.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/integrators/test_path_tracers.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_distant_flux.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/measure/test_distant_flux.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_hemispherical_distant.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/measure/test_hemispherical_distant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_multi_distant.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/measure/test_multi_distant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_multi_radiancemeter.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/measure/test_multi_radiancemeter.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_perspective.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/measure/test_perspective.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_radiancemeter.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/measure/test_radiancemeter.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_target.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/measure/test_target.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/phase/test_blend.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/phase/test_blend.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/phase/test_tabulated.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/phase/test_tabulated.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/shapes/test_buffermesh.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/shapes/test_buffermesh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/shapes/test_cuboid.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/shapes/test_cuboid.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from eradiate.scenes.core import traverse
 from eradiate.scenes.shapes import CuboidShape
 from eradiate.test_tools.types import check_scene_element
 
 
 @pytest.mark.parametrize(
     "kwargs, expected_reflectance",
-    [({}, None), ({"bsdf": {"type": "black"}}, 0.0)],
+    [({}, None), ({"bsdf": {"type": "lambertian", "reflectance": 0.0}}, 0.0)],
     ids=["noargs", "args"],
 )
 def test_cuboid_construct_kernel_dict(modes_all, kwargs, expected_reflectance):
     cuboid = CuboidShape(**kwargs)
 
     mi_wrapper = check_scene_element(cuboid, mi.Shape)
```

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/shapes/test_filemesh.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/shapes/test_filemesh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/shapes/test_rectangle.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/shapes/test_rectangle.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from eradiate.scenes.core import traverse
 from eradiate.scenes.shapes import RectangleShape
 from eradiate.test_tools.types import check_scene_element
 
 
 @pytest.mark.parametrize(
     "kwargs, expected_reflectance",
-    [({}, None), ({"bsdf": {"type": "black"}}, 0.0)],
+    [({}, None), ({"bsdf": {"type": "lambertian", "reflectance": 0.0}}, 0.0)],
     ids=["noargs", "args"],
 )
 def test_rectangle_construct_kernel_dict(modes_all, kwargs, expected_reflectance):
     rectangle = RectangleShape(**kwargs)
     mi_wrapper = check_scene_element(rectangle, mi.Shape)
 
     if expected_reflectance is not None:
```

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/shapes/test_sphere.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/shapes/test_sphere.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from eradiate import unit_registry as ureg
 from eradiate.scenes.shapes import SphereShape
 from eradiate.test_tools.types import check_scene_element
 
 
 @pytest.mark.parametrize(
     "kwargs, expected_reflectance",
-    [({}, None), ({"bsdf": {"type": "black"}}, 0.0)],
+    [({}, None), ({"bsdf": {"type": "lambertian", "reflectance": 0.0}}, 0.0)],
     ids=["noargs", "args"],
 )
 def test_sphere_construct_kernel_dict(modes_all, kwargs, expected_reflectance):
     sphere = SphereShape(**kwargs)
     mi_wrapper = check_scene_element(sphere, mi.Shape)
 
     if expected_reflectance is not None:
```

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/spectra/test_air_scattering_coefficient.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/spectra/test_air_scattering_coefficient.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/spectra/test_core.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/spectra/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/spectra/test_interpolated.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/spectra/test_interpolated.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,19 +32,18 @@
             {"wavelengths": [500.0, 600.0], "values": [0.0, 1.0, 2.0]},
             ValueError,
             None,
         ),
         (
             {"wavelengths": [500.0, 600.0], "values": [0.0, 1.0]},
             InterpolatedSpectrum(
-                quantity=PhysicalQuantity.DIMENSIONLESS,
                 wavelengths=[500.0, 600.0] * ureg.nm,
-                values=[0.0, 1.0] * ureg.dimensionless,
+                values=[0.0, 1.0],
             ),
-            "dimensionless",
+            None,
         ),
         (
             {
                 "quantity": "irradiance",
                 "wavelengths": [500.0, 600.0],
                 "values": [0.0, 1.0],
             },
@@ -69,42 +68,60 @@
                 "quantity": "irradiance",
                 "wavelengths": [500.0, 600.0] * ureg.s,
                 "values": [0.0, 1.0],
             },
             UnitsError,
             None,
         ),
+        (
+            {
+                "wavelengths": [500.0, 600.0],
+                "values": [0.0, 1.0] * ureg.dimensionless,
+            },
+            InterpolatedSpectrum(
+                quantity=None,
+                wavelengths=[500.0, 600.0] * ureg.nm,
+                values=[0.0, 1.0] * ureg.dimensionless,
+            ),
+            None,
+        ),
     ],
     ids=[
         "no_args",
         "missing_args_1",
         "missing_args_2",
         "array_shape_mismatch",
         "no_quantity",
         "no_units",
         "inconsistent_units_1",
         "inconsistent_units_2",
+        "quantity_values_but_no_quantity",
     ],
 )
 def test_interpolated_construct(modes_all, tested, expected, units):
     if isinstance(expected, InterpolatedSpectrum):
         s = InterpolatedSpectrum(**tested)
+
         assert s.quantity is expected.quantity
-        assert isinstance(s.values, pint.Quantity)
-        assert isinstance(s.values.magnitude, np.ndarray)
         assert np.all(s.values == expected.values)
 
+        if isinstance(s.values, pint.Quantity):
+            assert isinstance(s.values.magnitude, np.ndarray)
+        else:
+            assert isinstance(s.values, np.ndarray)
+
     elif issubclass(expected, Exception):
         with pytest.raises(expected):
             InterpolatedSpectrum(**tested)
 
     else:
         raise RuntimeError
 
 
+@pytest.mark.parametrize("quantity", ["dimensionless", None])
 @pytest.mark.parametrize(
     "wmin, wmax, expected, isclose_kwargs",
     [
         # Easy case: integrate over full interval
         (500.0 * ureg.nm, 600.0 * ureg.nm, 50.0 * ureg.nm, {"rtol": 1e-10}),
         # Min or max falls in-between two coordinate values
         (540.0 * ureg.nm, 600.0 * ureg.nm, 42.0 * ureg.nm, {"rtol": 1e-10}),
@@ -119,21 +136,25 @@
         # Integrating on an interval covering the whole support yields correct
         # integral values
         (450.0 * ureg.nm, 650.0 * ureg.nm, 50.0 * ureg.nm, {"rtol": 1e-10}),
         (500.0 * ureg.nm, 650.0 * ureg.nm, 50.0 * ureg.nm, {"rtol": 1e-10}),
         (450.0 * ureg.nm, 600.0 * ureg.nm, 50.0 * ureg.nm, {"rtol": 1e-10}),
     ],
 )
-def test_interpolated_integral(mode_mono, wmin, wmax, expected, isclose_kwargs):
+def test_interpolated_integral(
+    mode_mono, quantity, wmin, wmax, expected, isclose_kwargs
+):
     s = InterpolatedSpectrum(
         wavelengths=[500.0, 525.0, 550.0, 575.0, 600.0],
         values=[0.0, 0.25, 0.5, 0.75, 1.0],
+        quantity=quantity,
     )
 
     integral = s.integral(wmin, wmax)
+
     np.testing.assert_allclose(
         integral.m_as(ureg.nm), expected.m_as(ureg.nm), **isclose_kwargs
     )
 
 
 @pytest.mark.parametrize(
     "quantity, values, w, expected",
@@ -177,27 +198,41 @@
         expected = 0.5
 
     elif eradiate.mode().is_ckd:
         si = SpectralIndex.new(w=550.0 * ureg.nm, g=0)
         expected = 0.5
 
     else:
-        assert False
+        raise NotImplementedError
 
     # Spectrum performs linear interpolation and yields units consistent with
     # quantity
-    spectrum = InterpolatedSpectrum(wavelengths=[500.0, 600.0], values=[0.0, 1.0])
+    spectrum = InterpolatedSpectrum(
+        quantity="dimensionless",
+        wavelengths=[500.0, 600.0],
+        values=[0.0, 1.0],
+    )
     assert spectrum.eval(si) == expected * spectrum.values.units
 
     spectrum = InterpolatedSpectrum(
         quantity="irradiance", wavelengths=[500.0, 600.0], values=[0.0, 1.0]
     )
-    # Interpolation returns quantity
     assert spectrum.eval(si) == expected * spectrum.values.units
 
+    # If no quantity is specified, the evaluation routine returns a
+    # unitless value
+    spectrum = InterpolatedSpectrum(
+        quantity=None,
+        wavelengths=[500.0, 600.0],
+        values=[0.0, 1.0],
+    )
+    actual = spectrum.eval(si)
+    assert actual == expected
+    assert not isinstance(actual, pint.Quantity)
+
 
 def test_interpolated_kernel_dict(modes_all_mono):
     # Instantiate from factory
     with ucc.override({"radiance": "W/m^2/sr/nm"}):
         spectrum = spectrum_factory.convert(
             {
                 "type": "interpolated",
@@ -215,10 +250,10 @@
         assert np.isclose(mi_wrapper.parameters["value"], 5e-4)
 
 
 def test_interpolated_from_dataarray(mode_mono):
     da = eradiate.data.load_dataset(
         "spectra/reflectance/lambertian_soil.nc"
     ).reflectance.sel(brightness="darkest")
-    spectrum = InterpolatedSpectrum.from_dataarray(dataarray=da)
+    spectrum = InterpolatedSpectrum.from_dataarray(quantity="reflectance", dataarray=da)
     assert np.all(spectrum.wavelengths.m_as(da.w.attrs["units"]) == da.w.values)
     assert np.all(spectrum.values.m_as(da.attrs["units"]) == da.values)
```

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/spectra/test_solar_irradiance.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/spectra/test_solar_irradiance.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/spectra/test_uniform.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/spectra/test_uniform.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 
 
 @pytest.mark.parametrize(
     "tested, expected",
     [
         (
             {"value": 1.0},
-            UniformSpectrum(quantity=PhysicalQuantity.DIMENSIONLESS, value=1.0),
+            UniformSpectrum(quantity=None, value=1.0),
         ),
         (
             {"value": 1},
-            UniformSpectrum(quantity=PhysicalQuantity.DIMENSIONLESS, value=1.0),
+            UniformSpectrum(quantity=None, value=1.0),
         ),
         (
             {
                 "value": 1.0 * ureg.m**-1,
                 "quantity": PhysicalQuantity.COLLISION_COEFFICIENT,
             },
             UniformSpectrum(
@@ -38,36 +38,46 @@
             UniformSpectrum(
                 quantity=PhysicalQuantity.COLLISION_COEFFICIENT,
                 value=1.0 * ureg.m**-1,
             ),
         ),
         (
             {"value": 1.0, "quantity": "speed"},
-            ValueError,
+            KeyError,
         ),
         (
             {"quantity": "collision_coefficient", "value": ureg.Quantity(1.0, "")},
             UnitsError,
         ),
+        (
+            {"value": 1.0 * ureg.dimensionless},
+            ValueError,
+        ),
     ],
     ids=[
         "float",
         "int",
         "quantity",
         "quantity_convert",
         "unsupported_quantity",
         "inconsistent_units",
+        "unitless_value_but_no_quantity",
     ],
 )
-def test_uniform_construct(modes_all, tested, expected):
+def test_uniform_construct_basic(modes_all, tested, expected):
     if isinstance(expected, UniformSpectrum):
         s = UniformSpectrum(**tested)
+
         assert s.quantity is expected.quantity
         assert np.all(s.value == expected.value)
-        assert isinstance(s.value.magnitude, float)
+
+        if isinstance(s.value, pint.Quantity):
+            assert isinstance(s.value.magnitude, float)
+        else:
+            assert isinstance(s.value, float)
 
     elif issubclass(expected, Exception):
         with pytest.raises(expected):
             UniformSpectrum(**tested)
 
     else:
         raise RuntimeError
@@ -107,11 +117,12 @@
     eval = UniformSpectrum(quantity=quantity, value=value).eval_mono(w)
     assert np.all(expected == eval)
     assert isinstance(eval, pint.Quantity)
 
 
 def test_integral(mode_mono):
     s = UniformSpectrum(value=0.5)
-    assert s.integral(300.0, 400.0) == 50.0 * ureg.nm
+    # Unitless value is interpreted as dimensionless
+    assert s.integral(300.0 * ureg.nm, 400.0 * ureg.nm) == 50.0 * ureg.nm
 
     s = UniformSpectrum(quantity="collision_coefficient", value=0.5)
-    assert s.integral(300.0, 400.0) == 50.0 * ureg("nm / m")
+    assert s.integral(300.0 * ureg.nm, 400.0 * ureg.nm) == 50.0 * ureg("nm / m")
```

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/surface/test_basic.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/surface/test_basic.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/surface/test_central_patch.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/surface/test_central_patch.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/test_core.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/scenes/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/spectral/test_ckd.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/spectral/test_ckd.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/spectral/test_index.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/spectral/test_index.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/spectral/test_mono.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/spectral/test_mono.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_config.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     # Otherwise it raises
     with pytest.raises(ConfigError):
         EradiateConfig.from_environ({"ERADIATE_SOURCE_DIR": tmpdir_path})
 
 
 
 @pytest.mark.skipif(eradiate_mitsuba_status(), reason='This is not a production environment: eradiate-mitsuba is not installed')
-def test_production_config():
+def test_production_config(tmpdir):
     # Create an appropriate file tree for tests
     tmpdir_path = Path(tmpdir)
     (tmpdir_path / "eradiate/src/eradiate").mkdir(parents=True)
     (tmpdir_path / "eradiate/src/eradiate/__init__.py").touch()
 
 
     # Should not fail, should detect eradiate-mitsuba instead
```

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_factory.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_factory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_frame.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_frame.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_mode.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_mode.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_quad.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_quad.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_rng.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_rng.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_srf_tools.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_srf_tools.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_tools/test_regression.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_tools/test_regression.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_units.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_units.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_validators.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_validators.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_warp.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/test_warp.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/thermoprops/test_afgl1986.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/thermoprops/test_afgl1986.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/thermoprops/test_us76.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/thermoprops/test_us76.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/thermoprops/test_util.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/thermoprops/test_util.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/util/test_deprecation.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/util/test_deprecation.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/util/test_misc.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/util/test_misc.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/xarray/conftest.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/xarray/conftest.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/xarray/test_interp.py` & `eradiate-0.23.2rc2/tests/01_eradiate/01_unit/xarray/test_interp.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/02_system/conftest.py` & `eradiate-0.23.2rc2/tests/01_eradiate/02_system/conftest.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_albedo.py` & `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_albedo.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_atmosphere_ckd_vs_mono.py` & `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_atmosphere_ckd_vs_mono.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_atmosphere_rpv.py` & `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_atmosphere_rpv.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_basic.py` & `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_basic.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 
 import eradiate
 from eradiate import KernelContext
 from eradiate import unit_registry as ureg
 from eradiate.kernel import mi_render
 from eradiate.scenes.bsdfs import LambertianBSDF
 from eradiate.scenes.core import Scene
-from eradiate.scenes.illumination import ConstantIllumination, DirectionalIllumination
+from eradiate.scenes.illumination import ConstantIllumination, DirectionalIllumination, AstroObjectIllumination
 from eradiate.scenes.integrators import PathIntegrator
 from eradiate.scenes.measure import MultiDistantMeasure
 from eradiate.scenes.shapes import RectangleShape
 from eradiate.scenes.surface import BasicSurface
 from eradiate.test_tools.types import check_scene_element
 
 
-@pytest.mark.parametrize("illumination, spp", [("directional", 1), ("constant", 5e5)])
+@pytest.mark.parametrize("illumination, spp", [("directional", 1), ("constant", 5e5), ("astroobject", 5e5)])
 @pytest.mark.parametrize("li", [0.1, 1.0, 10.0])
 @pytest.mark.slow
 def test_radiometric_accuracy(modes_all_mono, illumination, spp, li, ert_seed_state):
     r"""
     Radiometric check (``path``)
     ============================
 
@@ -78,20 +78,28 @@
         "measure": measure,
         "integrator": PathIntegrator(),
     }
 
     if illumination == "directional":
         objects["illumination"] = DirectionalIllumination(zenith=0.0, irradiance=li)
         theoretical_solution = np.full_like(vza, rho * li / np.pi)
+        rtol=1e-3
 
     elif illumination == "constant":
         objects["illumination"] = ConstantIllumination(radiance=li)
         theoretical_solution = np.full_like(vza, rho * li)
+        rtol=1e-3
+
+    elif illumination == "astroobject":
+        objects["illumination"] = AstroObjectIllumination(zenith=0.0, irradiance=li, angular_diameter=0.03)
+        theoretical_solution = np.full_like(vza, rho * li / np.pi)
+        # The angular diameter is not taken into account in the theoretical solution
+        rtol=1e-2
 
     else:
         raise ValueError(f"unsupported illumination '{illumination}'")
 
     scene = Scene(objects=objects)
     mi_wrapper = check_scene_element(scene, mi.Scene)
 
     result = np.squeeze(mi_render(mi_wrapper, ctxs=[KernelContext()])[550.0]["measure"])
-    np.testing.assert_allclose(result, theoretical_solution, rtol=1e-3)
+    np.testing.assert_allclose(result, theoretical_solution, rtol=rtol)
```

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_ckd_basic.py` & `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_ckd_basic.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_compare_canopy_atmosphere.py` & `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_compare_canopy_atmosphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_expansion.py` & `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_expansion.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_flags.py` & `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_flags.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_parameter_id_lookup.py` & `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_parameter_id_lookup.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_irradiance_scaling.py` & `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_irradiance_scaling.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_kernel_render_benchmark.py` & `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_kernel_render_benchmark.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_maximum_scene_size.py` & `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_maximum_scene_size.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_mdistant_insitu.py` & `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_mdistant_insitu.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_onedim_lambertian_brf.py` & `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_onedim_lambertian_brf.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_onedim_phase.py` & `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_onedim_phase.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_onedim_symmetry.py` & `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_onedim_symmetry.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_spectral_loop.py` & `eradiate-0.23.2rc2/tests/01_eradiate/02_system/test_spectral_loop.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986.py` & `eradiate-0.23.2rc2/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986_continental.py` & `eradiate-0.23.2rc2/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986_continental.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/03_regression/rami4atm/test_rami4atm_hom00_bla_sd2s_m03_z30a000_brfpp.py` & `eradiate-0.23.2rc2/tests/01_eradiate/03_regression/rami4atm/test_rami4atm_hom00_bla_sd2s_m03_z30a000_brfpp.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/03_regression/romc/test_het01.py` & `eradiate-0.23.2rc2/tests/01_eradiate/03_regression/romc/test_het01.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/03_regression/romc/test_het04.py` & `eradiate-0.23.2rc2/tests/01_eradiate/03_regression/romc/test_het04.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/03_regression/romc/test_het06.py` & `eradiate-0.23.2rc2/tests/01_eradiate/03_regression/romc/test_het06.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/01_eradiate/conftest.py` & `eradiate-0.23.2rc2/tests/01_eradiate/conftest.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc1/tests/conftest.py` & `eradiate-0.23.2rc2/tests/conftest.py`

 * *Files identical despite different names*

