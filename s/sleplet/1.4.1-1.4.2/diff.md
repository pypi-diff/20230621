# Comparing `tmp/sleplet-1.4.1.tar.gz` & `tmp/sleplet-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleplet-1.4.1.tar", last modified: Wed May  3 13:58:27 2023, max compression
+gzip compressed data, was "sleplet-1.4.2.tar", last modified: Wed Jun 21 14:25:30 2023, max compression
```

## Comparing `sleplet-1.4.1.tar` & `sleplet-1.4.2.tar`

### file list

```diff
@@ -1,211 +1,210 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.286598 sleplet-1.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.250598 sleplet-1.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.258598 sleplet-1.4.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-03 13:58:16.000000 sleplet-1.4.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-03 13:58:16.000000 sleplet-1.4.1/.github/ISSUE_TEMPLATE/documentation.md
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-03 13:58:16.000000 sleplet-1.4.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-03 13:58:16.000000 sleplet-1.4.1/.github/ISSUE_TEMPLATE/question.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.262598 sleplet-1.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-03 13:58:16.000000 sleplet-1.4.1/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-03 13:58:16.000000 sleplet-1.4.1/.github/workflows/documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-03 13:58:16.000000 sleplet-1.4.1/.github/workflows/examples.yml
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-03 13:58:16.000000 sleplet-1.4.1/.github/workflows/licence.yml
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-03 13:58:16.000000 sleplet-1.4.1/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-03 13:58:16.000000 sleplet-1.4.1/.github/workflows/paper.yml
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-03 13:58:16.000000 sleplet-1.4.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-03 13:58:16.000000 sleplet-1.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-03 13:58:16.000000 sleplet-1.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-03 13:58:16.000000 sleplet-1.4.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-05-03 13:58:16.000000 sleplet-1.4.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-03 13:58:16.000000 sleplet-1.4.1/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-05-03 13:58:27.282598 sleplet-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-03 13:58:16.000000 sleplet-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.262598 sleplet-1.4.1/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)    22029 2023-05-03 13:58:16.000000 sleplet-1.4.1/documentation/DOCUMENTATION.md
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-03 13:58:16.000000 sleplet-1.4.1/documentation/config.mako
--rw-r--r--   0 runner    (1001) docker     (123)   254768 2023-05-03 13:58:16.000000 sleplet-1.4.1/documentation/slepian_wavelet_coefficients_homer_3B_2jmin_2j_zoom.png
--rw-r--r--   0 runner    (1001) docker     (123)   226721 2023-05-03 13:58:16.000000 sleplet-1.4.1/documentation/slepian_wavelets_south_america_3B_2jmin_2j_L128_res512_real.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.254598 sleplet-1.4.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.266598 sleplet-1.4.1/examples/arbitrary/
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/_denoising_slepian_wavelet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/_slepian_wavelet_covariance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.266598 sleplet-1.4.1/examples/arbitrary/africa/
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/africa/denoising_slepian_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/africa/eigenvalues_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/africa/progressive_wavelet_reconstruction_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/africa/slepian_reconstruction_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/africa/slepian_wavelet_covariance_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/africa/sparsity_wavelet_slepian_comparison_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/africa/tiling_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/africa/wavelet_reconstruction_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/eigenvalues_combined.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.266598 sleplet-1.4.1/examples/arbitrary/south_america/
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/south_america/denoising_slepian_functions_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/south_america/denoising_slepian_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/south_america/eigenvalues_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/south_america/progressive_wavelet_reconstruction_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/south_america/slepian_reconstruction_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/south_america/slepian_wavelet_covariance_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/south_america/sparsity_wavelet_slepian_comparison_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/south_america/tiling_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/arbitrary/south_america/wavelet_reconstruction_south_america.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.266598 sleplet-1.4.1/examples/mesh/
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/mesh/denoising_slepian_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/mesh/mesh_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/mesh/mesh_slepian_eigenvalues.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/mesh/mesh_tiling.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/mesh/produce_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.266598 sleplet-1.4.1/examples/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/misc/_denoising_axisym.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/misc/denoising_axisym_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/misc/denoising_axisym_earth.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/misc/denoising_axisym_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/misc/translation_normalisation.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/misc/wavelet_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.270598 sleplet-1.4.1/examples/polar_cap/
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/polar_cap/eigenfunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/polar_cap/eigenvalues.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/polar_cap/fried_egg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/polar_cap/simons_5_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/polar_cap/simons_5_3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/polar_cap/slepian_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/polar_cap/slepian_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.270598 sleplet-1.4.1/examples/wavelets/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/wavelets/axisymmetric_tiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-03 13:58:16.000000 sleplet-1.4.1/examples/wavelets/axisymmetric_wavelet_covariance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.270598 sleplet-1.4.1/paper/
--rw-r--r--   0 runner    (1001) docker     (123)    15349 2023-05-03 13:58:16.000000 sleplet-1.4.1/paper/arxiv.tex
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-05-03 13:58:16.000000 sleplet-1.4.1/paper/paper.bib
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-05-03 13:58:16.000000 sleplet-1.4.1/paper/paper.md
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-03 13:58:16.000000 sleplet-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-03 13:58:16.000000 sleplet-1.4.1/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 13:58:27.286598 sleplet-1.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.254598 sleplet-1.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.270598 sleplet-1.4.1/src/sleplet/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_array_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_bool_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_class_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_convolution_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.274598 sleplet-1.4.1/src/sleplet/_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_data/create_earth_flm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_data/create_wmap_flm.py
--rw-r--r--   0 runner    (1001) docker     (123)    39339 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_data/meshes_polygons_bird.off
--rw-r--r--   0 runner    (1001) docker     (123)   111621 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_data/meshes_polygons_cheetah.off
--rw-r--r--   0 runner    (1001) docker     (123)   321932 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_data/meshes_polygons_cube.off
--rw-r--r--   0 runner    (1001) docker     (123)    65194 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_data/meshes_polygons_dragon.off
--rw-r--r--   0 runner    (1001) docker     (123)   329591 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_data/meshes_polygons_homer.off
--rw-r--r--   0 runner    (1001) docker     (123)    36961 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_data/meshes_polygons_teapot.off
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_data/meshes_regions_bird.toml
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_data/meshes_regions_cheetah.toml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_data/meshes_regions_cube.toml
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_data/meshes_regions_dragon.toml
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_data/meshes_regions_homer.toml
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_data/meshes_regions_teapot.toml
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_data/setup_pooch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_integration_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_mask_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_mesh_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_parallel_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_plotly_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.274598 sleplet-1.4.1/src/sleplet/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_scripts/plotting_on_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    10988 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_scripts/plotting_on_sphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_slepian_arbitrary_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_string_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-03 13:58:27.000000 sleplet-1.4.1/src/sleplet/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.278598 sleplet-1.4.1/src/sleplet/functions/
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/axisymmetric_wavelet_coefficients_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/axisymmetric_wavelet_coefficients_earth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/axisymmetric_wavelet_coefficients_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/axisymmetric_wavelets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/coefficients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/dirac_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/directional_spin_wavelets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/earth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/elongated_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/flm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/fp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/harmonic_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/noise_earth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/ridgelets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/slepian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/slepian_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/slepian_dirac_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/slepian_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/slepian_noise_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/slepian_noise_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/slepian_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/slepian_wavelet_coefficients_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/slepian_wavelet_coefficients_south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/slepian_wavelets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/south_america.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/spherical_harmonic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/squashed_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/functions/wmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/harmonic_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.282598 sleplet-1.4.1/src/sleplet/meshes/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/meshes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/meshes/_mesh_slepian_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/meshes/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/meshes/mesh_basis_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/meshes/mesh_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/meshes/mesh_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/meshes/mesh_harmonic_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/meshes/mesh_noise_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/meshes/mesh_slepian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/meshes/mesh_slepian_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/meshes/mesh_slepian_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/meshes/mesh_slepian_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/meshes/mesh_slepian_noise_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/meshes/mesh_slepian_wavelet_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/meshes/mesh_slepian_wavelets.py
--rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/plot_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.282598 sleplet-1.4.1/src/sleplet/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/plotting/_create_plot_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/plotting/_create_plot_sphere.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.282598 sleplet-1.4.1/src/sleplet/slepian/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/slepian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/slepian/_slepian_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/slepian/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/slepian/slepian_arbitrary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/slepian/slepian_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/slepian/slepian_limit_lat_lon.py
--rw-r--r--   0 runner    (1001) docker     (123)    13590 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/slepian/slepian_polar_cap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6955 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/slepian_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-05-03 13:58:16.000000 sleplet-1.4.1/src/sleplet/wavelet_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.274598 sleplet-1.4.1/src/sleplet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-05-03 13:58:27.000000 sleplet-1.4.1/src/sleplet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-05-03 13:58:27.000000 sleplet-1.4.1/src/sleplet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 13:58:27.000000 sleplet-1.4.1/src/sleplet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-03 13:58:27.000000 sleplet-1.4.1/src/sleplet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-03 13:58:27.000000 sleplet-1.4.1/src/sleplet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 13:58:27.000000 sleplet-1.4.1/src/sleplet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:58:27.282598 sleplet-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_arbitrary_region.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_harmonic.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_loading_pooch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_slepian_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_translation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-05-03 13:58:16.000000 sleplet-1.4.1/tests/test_wavelets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:30.075563 sleplet-1.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:30.043563 sleplet-1.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:30.047563 sleplet-1.4.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-21 14:25:16.000000 sleplet-1.4.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-21 14:25:16.000000 sleplet-1.4.2/.github/ISSUE_TEMPLATE/documentation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-21 14:25:16.000000 sleplet-1.4.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-21 14:25:16.000000 sleplet-1.4.2/.github/ISSUE_TEMPLATE/question.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:30.047563 sleplet-1.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-21 14:25:16.000000 sleplet-1.4.2/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-21 14:25:16.000000 sleplet-1.4.2/.github/workflows/documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-21 14:25:16.000000 sleplet-1.4.2/.github/workflows/examples.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-21 14:25:16.000000 sleplet-1.4.2/.github/workflows/licence.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-21 14:25:16.000000 sleplet-1.4.2/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-21 14:25:16.000000 sleplet-1.4.2/.github/workflows/paper.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-21 14:25:16.000000 sleplet-1.4.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-21 14:25:16.000000 sleplet-1.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-21 14:25:16.000000 sleplet-1.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-21 14:25:16.000000 sleplet-1.4.2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-06-21 14:25:16.000000 sleplet-1.4.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-21 14:25:16.000000 sleplet-1.4.2/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-06-21 14:25:30.075563 sleplet-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-06-21 14:25:16.000000 sleplet-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:30.047563 sleplet-1.4.2/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)    22029 2023-06-21 14:25:16.000000 sleplet-1.4.2/documentation/DOCUMENTATION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-21 14:25:16.000000 sleplet-1.4.2/documentation/config.mako
+-rw-r--r--   0 runner    (1001) docker     (123)   254768 2023-06-21 14:25:16.000000 sleplet-1.4.2/documentation/slepian_wavelet_coefficients_homer_3B_2jmin_2j_zoom.png
+-rw-r--r--   0 runner    (1001) docker     (123)   226721 2023-06-21 14:25:16.000000 sleplet-1.4.2/documentation/slepian_wavelets_south_america_3B_2jmin_2j_L128_res512_real.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:30.043563 sleplet-1.4.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:30.051563 sleplet-1.4.2/examples/arbitrary/
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/arbitrary/_denoising_slepian_wavelet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/arbitrary/_slepian_wavelet_covariance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:30.051563 sleplet-1.4.2/examples/arbitrary/africa/
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/arbitrary/africa/denoising_slepian_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/arbitrary/africa/eigenvalues_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/arbitrary/africa/progressive_wavelet_reconstruction_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/arbitrary/africa/slepian_reconstruction_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/arbitrary/africa/slepian_wavelet_covariance_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/arbitrary/africa/sparsity_wavelet_slepian_comparison_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/arbitrary/africa/tiling_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/arbitrary/africa/wavelet_reconstruction_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/arbitrary/eigenvalues_combined.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:30.055563 sleplet-1.4.2/examples/arbitrary/south_america/
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/arbitrary/south_america/denoising_slepian_functions_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/arbitrary/south_america/denoising_slepian_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/arbitrary/south_america/eigenvalues_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/arbitrary/south_america/progressive_wavelet_reconstruction_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/arbitrary/south_america/slepian_reconstruction_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/arbitrary/south_america/slepian_wavelet_covariance_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/arbitrary/south_america/sparsity_wavelet_slepian_comparison_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/arbitrary/south_america/tiling_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/arbitrary/south_america/wavelet_reconstruction_south_america.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:30.055563 sleplet-1.4.2/examples/mesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/mesh/denoising_slepian_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/mesh/mesh_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/mesh/mesh_slepian_eigenvalues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/mesh/mesh_tiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/mesh/produce_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:30.055563 sleplet-1.4.2/examples/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/misc/_denoising_axisym.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/misc/denoising_axisym_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/misc/denoising_axisym_earth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/misc/denoising_axisym_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/misc/translation_normalisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/misc/wavelet_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:30.059563 sleplet-1.4.2/examples/polar_cap/
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/polar_cap/eigenfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/polar_cap/eigenvalues.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/polar_cap/fried_egg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/polar_cap/simons_5_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/polar_cap/simons_5_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/polar_cap/slepian_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/polar_cap/slepian_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:30.059563 sleplet-1.4.2/examples/wavelets/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/wavelets/axisymmetric_tiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-06-21 14:25:16.000000 sleplet-1.4.2/examples/wavelets/axisymmetric_wavelet_covariance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:30.059563 sleplet-1.4.2/paper/
+-rw-r--r--   0 runner    (1001) docker     (123)    15349 2023-06-21 14:25:16.000000 sleplet-1.4.2/paper/arxiv.tex
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-06-21 14:25:16.000000 sleplet-1.4.2/paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-21 14:25:16.000000 sleplet-1.4.2/paper/paper.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-06-21 14:25:16.000000 sleplet-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-21 14:25:16.000000 sleplet-1.4.2/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 14:25:30.075563 sleplet-1.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:30.043563 sleplet-1.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:30.059563 sleplet-1.4.2/src/sleplet/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/_array_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/_bool_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/_class_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/_convolution_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:30.067563 sleplet-1.4.2/src/sleplet/_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/_data/create_earth_flm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/_data/create_wmap_flm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39339 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/_data/meshes_polygons_bird.off
+-rw-r--r--   0 runner    (1001) docker     (123)   111621 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/_data/meshes_polygons_cheetah.off
+-rw-r--r--   0 runner    (1001) docker     (123)   321932 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/_data/meshes_polygons_cube.off
+-rw-r--r--   0 runner    (1001) docker     (123)    65194 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/_data/meshes_polygons_dragon.off
+-rw-r--r--   0 runner    (1001) docker     (123)   329591 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/_data/meshes_polygons_homer.off
+-rw-r--r--   0 runner    (1001) docker     (123)    36961 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/_data/meshes_polygons_teapot.off
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/_data/meshes_regions_bird.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/_data/meshes_regions_cheetah.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/_data/meshes_regions_cube.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/_data/meshes_regions_dragon.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/_data/meshes_regions_homer.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/_data/meshes_regions_teapot.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/_data/setup_pooch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/_integration_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/_mask_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/_mesh_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/_parallel_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/_plotly_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:30.067563 sleplet-1.4.2/src/sleplet/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/_scripts/plotting_on_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11005 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/_scripts/plotting_on_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/_slepian_arbitrary_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/_string_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 14:25:29.000000 sleplet-1.4.2/src/sleplet/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:30.071563 sleplet-1.4.2/src/sleplet/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/functions/africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/functions/axisymmetric_wavelet_coefficients_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/functions/axisymmetric_wavelet_coefficients_earth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/functions/axisymmetric_wavelet_coefficients_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/functions/axisymmetric_wavelets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/functions/coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/functions/dirac_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/functions/directional_spin_wavelets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/functions/earth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/functions/elongated_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/functions/flm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/functions/fp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/functions/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/functions/harmonic_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/functions/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/functions/noise_earth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/functions/ridgelets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/functions/slepian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/functions/slepian_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/functions/slepian_dirac_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/functions/slepian_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/functions/slepian_noise_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/functions/slepian_noise_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/functions/slepian_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/functions/slepian_wavelet_coefficients_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/functions/slepian_wavelet_coefficients_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/functions/slepian_wavelets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/functions/south_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/functions/spherical_harmonic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/functions/squashed_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/functions/wmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/harmonic_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:30.071563 sleplet-1.4.2/src/sleplet/meshes/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/meshes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/meshes/_mesh_slepian_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/meshes/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/meshes/mesh_basis_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/meshes/mesh_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/meshes/mesh_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/meshes/mesh_harmonic_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/meshes/mesh_noise_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/meshes/mesh_slepian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/meshes/mesh_slepian_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/meshes/mesh_slepian_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/meshes/mesh_slepian_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/meshes/mesh_slepian_noise_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/meshes/mesh_slepian_wavelet_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/meshes/mesh_slepian_wavelets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/plot_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:30.071563 sleplet-1.4.2/src/sleplet/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/plotting/_create_plot_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/plotting/_create_plot_sphere.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:30.075563 sleplet-1.4.2/src/sleplet/slepian/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/slepian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/slepian/_slepian_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/slepian/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/slepian/slepian_arbitrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/slepian/slepian_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/slepian/slepian_limit_lat_lon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/slepian/slepian_polar_cap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/slepian_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-06-21 14:25:16.000000 sleplet-1.4.2/src/sleplet/wavelet_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:30.063563 sleplet-1.4.2/src/sleplet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-06-21 14:25:29.000000 sleplet-1.4.2/src/sleplet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-06-21 14:25:30.000000 sleplet-1.4.2/src/sleplet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:25:29.000000 sleplet-1.4.2/src/sleplet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-21 14:25:29.000000 sleplet-1.4.2/src/sleplet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-21 14:25:29.000000 sleplet-1.4.2/src/sleplet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 14:25:29.000000 sleplet-1.4.2/src/sleplet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:25:30.075563 sleplet-1.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-06-21 14:25:16.000000 sleplet-1.4.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-21 14:25:16.000000 sleplet-1.4.2/tests/test_arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-21 14:25:16.000000 sleplet-1.4.2/tests/test_bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-21 14:25:16.000000 sleplet-1.4.2/tests/test_convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-06-21 14:25:16.000000 sleplet-1.4.2/tests/test_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-21 14:25:16.000000 sleplet-1.4.2/tests/test_harmonic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-21 14:25:16.000000 sleplet-1.4.2/tests/test_loading_pooch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-21 14:25:16.000000 sleplet-1.4.2/tests/test_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-21 14:25:16.000000 sleplet-1.4.2/tests/test_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-21 14:25:16.000000 sleplet-1.4.2/tests/test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-21 14:25:16.000000 sleplet-1.4.2/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-21 14:25:16.000000 sleplet-1.4.2/tests/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-21 14:25:16.000000 sleplet-1.4.2/tests/test_slepian_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-21 14:25:16.000000 sleplet-1.4.2/tests/test_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-21 14:25:16.000000 sleplet-1.4.2/tests/test_strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-06-21 14:25:16.000000 sleplet-1.4.2/tests/test_translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-21 14:25:16.000000 sleplet-1.4.2/tests/test_wavelets.py
```

### Comparing `sleplet-1.4.1/.github/ISSUE_TEMPLATE/bug_report.md` & `sleplet-1.4.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/.github/ISSUE_TEMPLATE/feature_request.md` & `sleplet-1.4.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/.github/workflows/deploy.yml` & `sleplet-1.4.2/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/.github/workflows/documentation.yml` & `sleplet-1.4.2/.github/workflows/documentation.yml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     steps:
       - name: checkout source
         uses: actions/checkout@v3
 
       - name: Set up python
         uses: actions/setup-python@v4
         with:
-          python-version: "3.10"
+          python-version: "3.x"
           cache: "pip"
           cache-dependency-path: "pyproject.toml"
 
       - name: Install dependencies
         run: python -m pip install -e .[docs]
 
       - name: Create documentation
```

### Comparing `sleplet-1.4.1/.github/workflows/examples.yml` & `sleplet-1.4.2/.github/workflows/examples.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 name: Examples
 
 on:
+  push:
+    branches:
+      - main
   workflow_dispatch:
 
 jobs:
   codeblocks:
     runs-on: ubuntu-latest
     steps:
       - name: Checkout source
         uses: actions/checkout@v3
 
       - name: Set up python
         uses: actions/setup-python@v4
         with:
-          python-version: "3.10"
+          python-version: "3.11"
           cache: "pip"
           cache-dependency-path: "pyproject.toml"
 
       - name: Cache pooch
         uses: actions/cache@v3
         with:
           path: ~/.cache/sleplet
@@ -34,15 +37,15 @@
     steps:
       - name: Checkout source
         uses: actions/checkout@v3
 
       - name: Set up python
         uses: actions/setup-python@v4
         with:
-          python-version: "3.10"
+          python-version: "3.11"
           cache: "pip"
           cache-dependency-path: "pyproject.toml"
 
       - name: Cache pooch
         uses: actions/cache@v3
         with:
           path: ~/.cache/sleplet
```

### Comparing `sleplet-1.4.1/.github/workflows/linting.yml` & `sleplet-1.4.2/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/.github/workflows/test.yml` & `sleplet-1.4.2/.github/workflows/test.yml`

 * *Files 9% similar despite different names*

```diff
@@ -7,38 +7,43 @@
   pull_request:
     paths-ignore:
       - "**.md"
       - "paper/**"
 
 jobs:
   test:
+    name: ${{ matrix.os }} py${{ matrix.python-version }}
+    runs-on: ${{ matrix.os }}
     strategy:
+      fail-fast: false
       matrix:
-        os: [ubuntu-latest, macos-latest]
-    runs-on: ${{ matrix.os }}
+        os: [macos-latest, ubuntu-latest]
+        python-version: ["3.10", "3.11"]
     steps:
       - name: Checkout source
         uses: actions/checkout@v3
 
       - name: Cache tox/pooch
         uses: actions/cache@v3
         with:
           path: |-
             .tox
             ~/.cache/sleplet
           key: test-${{ hashFiles('pyproject.toml') }}
 
-      - name: Set up python
+      - name: Set up python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
-          python-version: "3.10"
+          python-version: ${{ matrix.python-version }}
           cache: "pip"
           cache-dependency-path: "pyproject.toml"
 
       - name: Install dependencies
         run: python -m pip install tox tox-gh-actions
 
       - name: Test with tox
-        run: tox
+        run: tox run
+        env:
+          OS: ${{ matrix.os }}
 
       - name: Coverage
         uses: coverallsapp/github-action@v2
```

### Comparing `sleplet-1.4.1/.pre-commit-config.yaml` & `sleplet-1.4.2/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 repos:
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.264
+    rev: v0.0.274
     hooks:
       - id: ruff
   - repo: https://github.com/Lucas-C/pre-commit-hooks
     rev: v1.5.1
     hooks:
       - id: forbid-tabs
   - repo: https://github.com/pappasam/toml-sort
-    rev: v0.23.0
+    rev: v0.23.1
     hooks:
       - id: toml-sort-fix
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.1.1
+    rev: v1.4.0
     hooks:
       - id: mypy
         additional_dependencies: [numpy, pydantic]
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v3.0.0-alpha.9-for-vscode
     hooks:
       - id: prettier
@@ -32,12 +32,16 @@
         args: [--fix=lf]
       - id: trailing-whitespace
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/adamchainz/blacken-docs
-    rev: "1.13.0"
+    rev: "1.14.0"
     hooks:
       - id: blacken-docs
         additional_dependencies:
           - black==23.3.0
+  - repo: https://github.com/codespell-project/codespell
+    rev: v2.2.5
+    hooks:
+      - id: codespell
```

### Comparing `sleplet-1.4.1/CITATION.cff` & `sleplet-1.4.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/CONTRIBUTING.md` & `sleplet-1.4.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/LICENCE.md` & `sleplet-1.4.2/LICENCE.md`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/PKG-INFO` & `sleplet-1.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleplet
-Version: 1.4.1
+Version: 1.4.2
 Summary: Slepian Scale-Discretised Wavelets in Python
 Author-email: "Patrick J. Roddy" <patrickjamesroddy@gmail.com>
 License: BSD 3-Clause Licence
         
         Copyright (c) 2017-2023, Patrick Roddy
         All rights reserved.
         
@@ -40,14 +40,15 @@
 Project-URL: Issues, https://github.com/astro-informatics/sleplet/issues
 Keywords: manifolds,python,slepian-functions,sphere,wavelets
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `sleplet-1.4.1/README.md` & `sleplet-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/documentation/DOCUMENTATION.md` & `sleplet-1.4.2/documentation/DOCUMENTATION.md`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/documentation/config.mako` & `sleplet-1.4.2/documentation/config.mako`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/documentation/slepian_wavelet_coefficients_homer_3B_2jmin_2j_zoom.png` & `sleplet-1.4.2/documentation/slepian_wavelet_coefficients_homer_3B_2jmin_2j_zoom.png`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/documentation/slepian_wavelets_south_america_3B_2jmin_2j_L128_res512_real.png` & `sleplet-1.4.2/documentation/slepian_wavelets_south_america_3B_2jmin_2j_L128_res512_real.png`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/arbitrary/_denoising_slepian_wavelet.py` & `sleplet-1.4.2/examples/arbitrary/_denoising_slepian_wavelet.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/arbitrary/_slepian_wavelet_covariance.py` & `sleplet-1.4.2/examples/arbitrary/_slepian_wavelet_covariance.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/arbitrary/africa/denoising_slepian_africa.py` & `sleplet-1.4.2/examples/arbitrary/africa/denoising_slepian_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/arbitrary/africa/eigenvalues_africa.py` & `sleplet-1.4.2/examples/arbitrary/africa/eigenvalues_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/arbitrary/africa/progressive_wavelet_reconstruction_africa.py` & `sleplet-1.4.2/examples/arbitrary/africa/progressive_wavelet_reconstruction_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/arbitrary/africa/slepian_reconstruction_africa.py` & `sleplet-1.4.2/examples/arbitrary/africa/slepian_reconstruction_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/arbitrary/africa/slepian_wavelet_covariance_africa.py` & `sleplet-1.4.2/examples/arbitrary/africa/slepian_wavelet_covariance_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/arbitrary/africa/sparsity_wavelet_slepian_comparison_africa.py` & `sleplet-1.4.2/examples/arbitrary/africa/sparsity_wavelet_slepian_comparison_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/arbitrary/africa/tiling_africa.py` & `sleplet-1.4.2/examples/arbitrary/africa/tiling_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/arbitrary/africa/wavelet_reconstruction_africa.py` & `sleplet-1.4.2/examples/arbitrary/africa/wavelet_reconstruction_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/arbitrary/eigenvalues_combined.py` & `sleplet-1.4.2/examples/arbitrary/eigenvalues_combined.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/arbitrary/south_america/denoising_slepian_functions_south_america.py` & `sleplet-1.4.2/examples/arbitrary/south_america/denoising_slepian_functions_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/arbitrary/south_america/denoising_slepian_south_america.py` & `sleplet-1.4.2/examples/arbitrary/south_america/denoising_slepian_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/arbitrary/south_america/eigenvalues_south_america.py` & `sleplet-1.4.2/examples/arbitrary/south_america/eigenvalues_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/arbitrary/south_america/progressive_wavelet_reconstruction_south_america.py` & `sleplet-1.4.2/examples/arbitrary/south_america/progressive_wavelet_reconstruction_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/arbitrary/south_america/slepian_reconstruction_south_america.py` & `sleplet-1.4.2/examples/arbitrary/south_america/slepian_reconstruction_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/arbitrary/south_america/slepian_wavelet_covariance_south_america.py` & `sleplet-1.4.2/examples/arbitrary/south_america/slepian_wavelet_covariance_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/arbitrary/south_america/sparsity_wavelet_slepian_comparison_south_america.py` & `sleplet-1.4.2/examples/arbitrary/south_america/sparsity_wavelet_slepian_comparison_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/arbitrary/south_america/tiling_south_america.py` & `sleplet-1.4.2/examples/arbitrary/south_america/tiling_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/arbitrary/south_america/wavelet_reconstruction_south_america.py` & `sleplet-1.4.2/examples/arbitrary/south_america/wavelet_reconstruction_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/mesh/denoising_slepian_mesh.py` & `sleplet-1.4.2/examples/mesh/denoising_slepian_mesh.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/mesh/mesh_region.py` & `sleplet-1.4.2/examples/mesh/mesh_region.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     mesh = Mesh(mesh_name)
 
     # create region masking
     field = np.zeros(mesh.vertices.shape[0])
     field[mesh.region] = 1
 
     name = f"{mesh_name}_region"
-    PlotMesh(mesh, name, field, colour=cmocean.cm.haline, region=True).execute()
+    PlotMesh(mesh, name, field, region=True).execute(cmocean.cm.haline)
 
 
 if __name__ == "__main__":
     parser = ArgumentParser(description="mesh tiling")
     parser.add_argument(
         "function",
         type=str,
```

### Comparing `sleplet-1.4.1/examples/mesh/mesh_slepian_eigenvalues.py` & `sleplet-1.4.2/examples/mesh/mesh_slepian_eigenvalues.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/mesh/mesh_tiling.py` & `sleplet-1.4.2/examples/mesh/mesh_tiling.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/misc/_denoising_axisym.py` & `sleplet-1.4.2/examples/misc/_denoising_axisym.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     axisymmetric_wavelet_forward,
     axisymmetric_wavelet_inverse,
 )
 
 SAMPLING_SCHEME = "MWSS"
 
 
-def denoising_axisym(
+def denoising_axisym(  # noqa: PLR0913
     signal: Africa | Earth | SouthAmerica,
     noised_signal: Africa | Earth | SouthAmerica,
     axisymmetric_wavelets: AxisymmetricWavelets,
     snr_in: float,
     n_sigma: int,
     *,
     rotate_to_south_america: bool = False,
```

### Comparing `sleplet-1.4.1/examples/misc/denoising_axisym_africa.py` & `sleplet-1.4.2/examples/misc/denoising_axisym_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/misc/denoising_axisym_earth.py` & `sleplet-1.4.2/examples/misc/denoising_axisym_earth.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/misc/denoising_axisym_south_america.py` & `sleplet-1.4.2/examples/misc/denoising_axisym_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/misc/translation_normalisation.py` & `sleplet-1.4.2/examples/misc/translation_normalisation.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/misc/wavelet_transform.py` & `sleplet-1.4.2/examples/misc/wavelet_transform.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/polar_cap/eigenfunctions.py` & `sleplet-1.4.2/examples/polar_cap/eigenfunctions.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/polar_cap/eigenvalues.py` & `sleplet-1.4.2/examples/polar_cap/eigenvalues.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/polar_cap/fried_egg.py` & `sleplet-1.4.2/examples/polar_cap/fried_egg.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/polar_cap/simons_5_1.py` & `sleplet-1.4.2/examples/polar_cap/simons_5_1.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/polar_cap/simons_5_3.py` & `sleplet-1.4.2/examples/polar_cap/simons_5_3.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/polar_cap/slepian_coefficients.py` & `sleplet-1.4.2/examples/polar_cap/slepian_coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/polar_cap/slepian_error.py` & `sleplet-1.4.2/examples/polar_cap/slepian_error.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/wavelets/axisymmetric_tiling.py` & `sleplet-1.4.2/examples/wavelets/axisymmetric_tiling.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/examples/wavelets/axisymmetric_wavelet_covariance.py` & `sleplet-1.4.2/examples/wavelets/axisymmetric_wavelet_covariance.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/paper/arxiv.tex` & `sleplet-1.4.2/paper/arxiv.tex`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/paper/paper.bib` & `sleplet-1.4.2/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/paper/paper.md` & `sleplet-1.4.2/paper/paper.md`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/pyproject.toml` & `sleplet-1.4.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 ]
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Operating System :: POSIX",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: Image Processing",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Scientific/Engineering :: Visualization",
     "Typing :: Typed",
 ]
 dependencies = [
@@ -178,19 +179,24 @@
 overrides."tool.coverage.paths.source".inline_arrays = false
 
 [tool.tox]
 legacy_tox_ini = """
     [gh-actions]
     python =
         3.10: py310
+        3.11: py311
+
+    [gh-actions:env]
+    OS =
+        ubuntu-latest: linux
+        macos-latest: macos
 
     [testenv]
     commands =
         pytest --cov --cov-report=lcov --slow
     deps =
         pytest-cov
         pytest-skip-slow
 
     [tox]
-    env_list =
-        py310
+    env_list = py{310,311}-{linux,macos}
 """
```

### Comparing `sleplet-1.4.1/src/sleplet/__init__.py` & `sleplet-1.4.2/src/sleplet/__init__.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/_bool_methods.py` & `sleplet-1.4.2/src/sleplet/_bool_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/_class_lists.py` & `sleplet-1.4.2/src/sleplet/_class_lists.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/_convolution_methods.py` & `sleplet-1.4.2/src/sleplet/_convolution_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/_data/create_earth_flm.py` & `sleplet-1.4.2/src/sleplet/_data/create_earth_flm.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/_data/create_wmap_flm.py` & `sleplet-1.4.2/src/sleplet/_data/create_wmap_flm.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/_data/meshes_polygons_bird.off` & `sleplet-1.4.2/src/sleplet/_data/meshes_polygons_bird.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/_data/meshes_polygons_cheetah.off` & `sleplet-1.4.2/src/sleplet/_data/meshes_polygons_cheetah.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/_data/meshes_polygons_cube.off` & `sleplet-1.4.2/src/sleplet/_data/meshes_polygons_cube.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/_data/meshes_polygons_dragon.off` & `sleplet-1.4.2/src/sleplet/_data/meshes_polygons_dragon.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/_data/meshes_polygons_homer.off` & `sleplet-1.4.2/src/sleplet/_data/meshes_polygons_homer.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/_data/meshes_polygons_teapot.off` & `sleplet-1.4.2/src/sleplet/_data/meshes_polygons_teapot.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/_data/setup_pooch.py` & `sleplet-1.4.2/src/sleplet/_data/setup_pooch.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/_integration_methods.py` & `sleplet-1.4.2/src/sleplet/_integration_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/_mask_methods.py` & `sleplet-1.4.2/src/sleplet/_mask_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/_mesh_methods.py` & `sleplet-1.4.2/src/sleplet/_mesh_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/_parallel_methods.py` & `sleplet-1.4.2/src/sleplet/_parallel_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/_plotly_methods.py` & `sleplet-1.4.2/src/sleplet/_plotly_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "zeroline": False,
     "ticks": "",
     "showticklabels": False,
     "showbackground": False,
 }
 
 
-def create_camera(
+def create_camera(  # noqa: PLR0913
     x_eye: float,
     y_eye: float,
     z_eye: float,
     zoom: float,
     *,
     x_center: float = 0,
     y_center: float = 0,
```

### Comparing `sleplet-1.4.1/src/sleplet/_scripts/plotting_on_mesh.py` & `sleplet-1.4.2/src/sleplet/_scripts/plotting_on_mesh.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/_scripts/plotting_on_sphere.py` & `sleplet-1.4.2/src/sleplet/_scripts/plotting_on_sphere.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,15 @@
         "-v",
         action="version",
         version=sleplet.__version__,
     )
     return parser.parse_args()
 
 
-def plot(
+def plot(  # noqa: PLR0913
     f: sleplet.functions.coefficients.Coefficients,
     g: sleplet.functions.coefficients.Coefficients | None,
     *,
     alpha_pi_frac: float,
     beta_pi_frac: float,
     gamma_pi_frac: float,
     annotations: bool,
```

### Comparing `sleplet-1.4.1/src/sleplet/_slepian_arbitrary_methods.py` & `sleplet-1.4.2/src/sleplet/_slepian_arbitrary_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/_smoothing.py` & `sleplet-1.4.2/src/sleplet/_smoothing.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/_string_methods.py` & `sleplet-1.4.2/src/sleplet/_string_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/functions/__init__.py` & `sleplet-1.4.2/src/sleplet/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/functions/africa.py` & `sleplet-1.4.2/src/sleplet/functions/africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/functions/axisymmetric_wavelet_coefficients_africa.py` & `sleplet-1.4.2/src/sleplet/functions/axisymmetric_wavelet_coefficients_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/functions/axisymmetric_wavelet_coefficients_earth.py` & `sleplet-1.4.2/src/sleplet/functions/axisymmetric_wavelet_coefficients_earth.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/functions/axisymmetric_wavelet_coefficients_south_america.py` & `sleplet-1.4.2/src/sleplet/functions/axisymmetric_wavelet_coefficients_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/functions/axisymmetric_wavelets.py` & `sleplet-1.4.2/src/sleplet/functions/axisymmetric_wavelets.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/functions/coefficients.py` & `sleplet-1.4.2/src/sleplet/functions/coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/functions/dirac_delta.py` & `sleplet-1.4.2/src/sleplet/functions/dirac_delta.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/functions/directional_spin_wavelets.py` & `sleplet-1.4.2/src/sleplet/functions/directional_spin_wavelets.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/functions/earth.py` & `sleplet-1.4.2/src/sleplet/functions/earth.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/functions/elongated_gaussian.py` & `sleplet-1.4.2/src/sleplet/functions/elongated_gaussian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/functions/flm.py` & `sleplet-1.4.2/src/sleplet/functions/flm.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/functions/fp.py` & `sleplet-1.4.2/src/sleplet/functions/fp.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/functions/gaussian.py` & `sleplet-1.4.2/src/sleplet/functions/gaussian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/functions/harmonic_gaussian.py` & `sleplet-1.4.2/src/sleplet/functions/harmonic_gaussian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/functions/identity.py` & `sleplet-1.4.2/src/sleplet/functions/identity.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/functions/noise_earth.py` & `sleplet-1.4.2/src/sleplet/functions/noise_earth.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/functions/ridgelets.py` & `sleplet-1.4.2/src/sleplet/functions/ridgelets.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/functions/slepian.py` & `sleplet-1.4.2/src/sleplet/functions/slepian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/functions/slepian_africa.py` & `sleplet-1.4.2/src/sleplet/functions/slepian_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/functions/slepian_dirac_delta.py` & `sleplet-1.4.2/src/sleplet/functions/slepian_dirac_delta.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from sleplet.functions.fp import Fp
 
 _logger = logging.getLogger(__name__)
 
 
 @dataclass(config=sleplet._validation.Validation)
 class SlepianDiracDelta(Fp):
-    """Createa a Dirac delta of the Slepian coefficients."""
+    """Creates a Dirac delta of the Slepian coefficients."""
 
     def __post_init_post_parse__(self) -> None:
         super().__post_init_post_parse__()
 
     def _create_coefficients(self) -> npt.NDArray[np.complex_ | np.float_]:
         self._compute_angles()
         return sleplet.slepian_methods._compute_s_p_omega_prime(
```

### Comparing `sleplet-1.4.1/src/sleplet/functions/slepian_identity.py` & `sleplet-1.4.2/src/sleplet/functions/slepian_identity.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/functions/slepian_noise_africa.py` & `sleplet-1.4.2/src/sleplet/functions/slepian_noise_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/functions/slepian_noise_south_america.py` & `sleplet-1.4.2/src/sleplet/functions/slepian_noise_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/functions/slepian_south_america.py` & `sleplet-1.4.2/src/sleplet/functions/slepian_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/functions/slepian_wavelet_coefficients_africa.py` & `sleplet-1.4.2/src/sleplet/functions/slepian_wavelet_coefficients_africa.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/functions/slepian_wavelet_coefficients_south_america.py` & `sleplet-1.4.2/src/sleplet/functions/slepian_wavelet_coefficients_south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/functions/slepian_wavelets.py` & `sleplet-1.4.2/src/sleplet/functions/slepian_wavelets.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from sleplet.functions.fp import Fp
 
 _logger = logging.getLogger(__name__)
 
 
 @dataclass(config=sleplet._validation.Validation, kw_only=True)
 class SlepianWavelets(Fp):
-    """Creats the Slepian wavelets."""
+    """Creates the Slepian wavelets."""
 
     B: int = 3
     r"""The wavelet parameter. Represented as \(\lambda\) in the papers."""
     j_min: int = 2
     r"""The minimum wavelet scale. Represented as \(J_{0}\) in the papers."""
     j: int | None = None
     """Option to select a given wavelet. `None` indicates the scaling function,
```

### Comparing `sleplet-1.4.1/src/sleplet/functions/south_america.py` & `sleplet-1.4.2/src/sleplet/functions/south_america.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/functions/spherical_harmonic.py` & `sleplet-1.4.2/src/sleplet/functions/spherical_harmonic.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/functions/squashed_gaussian.py` & `sleplet-1.4.2/src/sleplet/functions/squashed_gaussian.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/functions/wmap.py` & `sleplet-1.4.2/src/sleplet/functions/wmap.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/harmonic_methods.py` & `sleplet-1.4.2/src/sleplet/harmonic_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/meshes/__init__.py` & `sleplet-1.4.2/src/sleplet/meshes/__init__.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/meshes/_mesh_slepian_decomposition.py` & `sleplet-1.4.2/src/sleplet/meshes/_mesh_slepian_decomposition.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/meshes/mesh.py` & `sleplet-1.4.2/src/sleplet/meshes/mesh.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/meshes/mesh_basis_functions.py` & `sleplet-1.4.2/src/sleplet/meshes/mesh_basis_functions.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/meshes/mesh_coefficients.py` & `sleplet-1.4.2/src/sleplet/meshes/mesh_coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/meshes/mesh_field.py` & `sleplet-1.4.2/src/sleplet/meshes/mesh_field.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/meshes/mesh_harmonic_coefficients.py` & `sleplet-1.4.2/src/sleplet/meshes/mesh_harmonic_coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/meshes/mesh_noise_field.py` & `sleplet-1.4.2/src/sleplet/meshes/mesh_noise_field.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/meshes/mesh_slepian.py` & `sleplet-1.4.2/src/sleplet/meshes/mesh_slepian.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
             for i in chunk:
                 _logger.info(f"start basis function: {i}")
                 self._fill_D_elements(D_int, i)
                 _logger.info(f"finish basis function: {i}")
 
             sleplet._parallel_methods.free_shared_memory(shm_int)
 
-        # split up L range to maximise effiency
+        # split up L range to maximise efficiency
         ncpu = int(os.getenv("NCPU", "4"))
         _logger.info(f"Number of CPU={ncpu}")
         chunks = sleplet._parallel_methods.split_arr_into_chunks(
             self.mesh.mesh_eigenvalues.shape[0],
             ncpu,
         )
```

### Comparing `sleplet-1.4.1/src/sleplet/meshes/mesh_slepian_coefficients.py` & `sleplet-1.4.2/src/sleplet/meshes/mesh_slepian_coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/meshes/mesh_slepian_field.py` & `sleplet-1.4.2/src/sleplet/meshes/mesh_slepian_field.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/meshes/mesh_slepian_functions.py` & `sleplet-1.4.2/src/sleplet/meshes/mesh_slepian_functions.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/meshes/mesh_slepian_noise_field.py` & `sleplet-1.4.2/src/sleplet/meshes/mesh_slepian_noise_field.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/meshes/mesh_slepian_wavelet_coefficients.py` & `sleplet-1.4.2/src/sleplet/meshes/mesh_slepian_wavelet_coefficients.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/meshes/mesh_slepian_wavelets.py` & `sleplet-1.4.2/src/sleplet/meshes/mesh_slepian_wavelets.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/noise.py` & `sleplet-1.4.2/src/sleplet/noise.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/plot_methods.py` & `sleplet-1.4.2/src/sleplet/plot_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
 
 def _set_outside_region_to_minimum(
     f_plot: npt.NDArray[np.float_],
     L: int,
     region: sleplet.slepian.region.Region,
 ) -> npt.NDArray[np.float_]:
     """
-    For the Slepian region set the outisde area to negative infinity
+    For the Slepian region set the outside area to negative infinity
     hence it is clear we are only interested in the coloured region.
     """
     # create mask of interest
     mask = sleplet._mask_methods.create_mask_region(L, region)
 
     # adapt for closed plot
     _, n_phi = ssht.sample_shape(L, Method=sleplet._vars.SAMPLING_SCHEME)
@@ -169,15 +169,15 @@
     if (f == 0).all():
         # if all 0, set to 0
         return f + 0.5
     # if all non-zero, set to 1 otherwise scale from [0, 1]
     return f / f.max() if np.allclose(f, f.max()) else (f - f.min()) / f.ptp()
 
 
-def _boost_field(
+def _boost_field(  # noqa: PLR0913
     field: npt.NDArray[np.complex_ | np.float_],
     L: int,
     resolution: int,
     *,
     reality: bool,
     spin: int,
     upsample: bool,
```

### Comparing `sleplet-1.4.1/src/sleplet/plotting/_create_plot_mesh.py` & `sleplet-1.4.2/src/sleplet/plotting/_create_plot_mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,27 +32,30 @@
     filename: str
     """The output filename of the plot."""
     f: npt.NDArray[np.complex_ | np.float_]
     """The field value sampled on the mesh."""
     _: KW_ONLY
     amplitude: float | None = None
     """Whether to customise the amplitude range of the colour bar."""
-    colour: LinearSegmentedColormap = cmocean.cm.ice
-    """The colour of the field on the mesh."""
     normalise: bool = True
     """Whether to normalise the plot or not."""
     region: bool = False
     """Whether to set the field values outside of the region to zero."""
 
     def __post_init_post_parse__(self) -> None:
         if self.normalise:
             self.filename += "_norm"
 
-    def execute(self) -> None:
-        """Performs the plot."""
+    def execute(self, colour: LinearSegmentedColormap = cmocean.cm.ice) -> None:
+        """
+        Performs the plot.
+
+        Args:
+            colour: From the `cmocean.cm` module
+        """
         vmin, vmax = self.f.min(), self.f.max()
         f = self._prepare_field(self.f)
 
         if self.region:
             # make plot area clearer
             f = self._set_outside_region_to_minimum(f)
 
@@ -79,15 +82,15 @@
                 colorbar=sleplet._plotly_methods.create_colour_bar(
                     tick_mark,
                     normalise=self.normalise,
                     bar_len=_MESH_CBAR_LEN,
                     bar_pos=self.mesh.colourbar_pos,
                     font_size=_MESH_CBAR_FONT_SIZE,
                 ),
-                colorscale=sleplet.plot_methods._convert_colourscale(self.colour),
+                colorscale=sleplet.plot_methods._convert_colourscale(colour),
                 lighting=go.mesh3d.Lighting(ambient=1),
                 reversescale=True,
             ),
         ]
 
         layout = sleplet._plotly_methods.create_layout(self.mesh.camera_view)
 
@@ -110,14 +113,14 @@
         )
 
     def _set_outside_region_to_minimum(
         self,
         f: npt.NDArray[np.float_],
     ) -> npt.NDArray[np.float_]:
         """
-        For the Slepian region set the outisde area to negative infinity
+        For the Slepian region set the outside area to negative infinity
         hence it is clear we are only interested in the coloured region.
         """
         region_on_faces = sleplet._mask_methods.convert_region_on_vertices_to_faces(
             self.mesh,
         )
         return np.where(region_on_faces, f, _MESH_UNSEEN)
```

### Comparing `sleplet-1.4.1/src/sleplet/plotting/_create_plot_sphere.py` & `sleplet-1.4.2/src/sleplet/plotting/_create_plot_sphere.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 
         fig = go.Figure(data=data, layout=layout)
 
         _logger.info(f"Opening: {self.filename}")
         pio.show(fig, config={"toImageButtonOptions": {"filename": self.filename}})
 
     @staticmethod
-    def _setup_plot(
+    def _setup_plot(  # noqa: PLR0913
         f: npt.NDArray[np.float_],
         resolution: int,
         *,
         method: str = "MW",
         close: bool = True,
         parametric: bool = False,
         parametric_scaling: list[float] | None = None,
```

### Comparing `sleplet-1.4.1/src/sleplet/slepian/_slepian_decomposition.py` & `sleplet-1.4.2/src/sleplet/slepian/_slepian_decomposition.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/slepian/region.py` & `sleplet-1.4.2/src/sleplet/slepian/region.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,25 +17,25 @@
     """Identifies and creates the appropriate Slepian region for the sphere."""
 
     gap: bool = False
     """Whether to enable a double ended polar cap, set by the `POLAR_GAP`
     environment variable. Only relevant if `theta_max` is not `180` and the
     other angles are at their default values."""
     mask_name: str = ""
-    """The name of the mask of the arbirary region, set by the `SLEPIAN_MASK`
+    """The name of the mask of the arbitrary region, set by the `SLEPIAN_MASK`
     environment variable. Current options are `africa` and `south_america`."""
     phi_max: float = sleplet._vars.PHI_MAX_DEFAULT
     """For a limited latitude longitude region, set by the `PHI_MAX` environment
     variable."""
     phi_min: float = sleplet._vars.PHI_MIN_DEFAULT
     """For a limited latitude longitude region, set by the `PHI_MIN` environment
     variable."""
     theta_max: float = sleplet._vars.THETA_MAX_DEFAULT
     """Set by the `THETA_MAX` environment variable. When set without the
-    other angles it controls a polar cap region. When in conjuction with the
+    other angles it controls a polar cap region. When in conjunction with the
     others it is for a limited latitude longitude region."""
     theta_min: float = sleplet._vars.THETA_MIN_DEFAULT
     """For a limited latitude longitude region, set by the `THETA_MIN` environment
     variable."""
 
     def __post_init_post_parse__(self) -> None:
         self._identify_region()
```

### Comparing `sleplet-1.4.1/src/sleplet/slepian/slepian_arbitrary.py` & `sleplet-1.4.2/src/sleplet/slepian/slepian_arbitrary.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 
 @dataclass(config=sleplet._validation.Validation)
 class SlepianArbitrary(SlepianFunctions):
     """Class to create an arbitrary Slepian region on the sphere."""
 
     mask_name: str
-    """The name of the mask of the arbirary region."""
+    """The name of the mask of the arbitrary region."""
     _: KW_ONLY
 
     def __post_init_post_parse__(self) -> None:
         self.resolution = _SAMPLES * self.L
         super().__post_init_post_parse__()
 
     def _create_fn_name(self) -> str:
@@ -60,19 +60,23 @@
     def _solve_eigenproblem(
         self,
     ) -> tuple[npt.NDArray[np.float_], npt.NDArray[np.complex_]]:
         eval_loc = f"{self.matrix_location}_eigenvalues.npy"
         evec_loc = f"{self.matrix_location}_eigenvectors.npy"
 
         try:
-            return np.load(
+            eigenvalues = np.load(
                 sleplet._data.setup_pooch.find_on_pooch_then_local(eval_loc),
-            ), np.load(sleplet._data.setup_pooch.find_on_pooch_then_local(evec_loc))
+            )
+            eigenvectors = np.load(
+                sleplet._data.setup_pooch.find_on_pooch_then_local(evec_loc),
+            )
         except TypeError:
-            return self._solve_D_matrix(eval_loc, evec_loc)
+            eigenvalues, eigenvectors = self._solve_D_matrix(eval_loc, evec_loc)
+        return eigenvalues, eigenvectors
 
     def _solve_D_matrix(  # noqa: N802
         self,
         eval_loc,
         evec_loc,
     ) -> tuple[npt.NDArray[np.float_], npt.NDArray[np.complex_]]:
         D = self._create_D_matrix()
@@ -115,15 +119,15 @@
             for i in chunk:
                 _logger.info(f"start ell: {i}")
                 self._matrix_helper(D_r_int, D_i_int, i)
                 _logger.info(f"finish ell: {i}")
 
             sleplet._parallel_methods.free_shared_memory(shm_r_int, shm_i_int)
 
-        # split up L range to maximise effiency
+        # split up L range to maximise efficiency
         ncpu = int(os.getenv("NCPU", "4"))
         _logger.info(f"Number of CPU={ncpu}")
         chunks = sleplet._parallel_methods.split_arr_into_chunks(
             self.L**2,
             ncpu,
         )
```

### Comparing `sleplet-1.4.1/src/sleplet/slepian/slepian_functions.py` & `sleplet-1.4.2/src/sleplet/slepian/slepian_functions.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet/slepian/slepian_limit_lat_lon.py` & `sleplet-1.4.2/src/sleplet/slepian/slepian_limit_lat_lon.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,23 +58,26 @@
 
     def _solve_eigenproblem(
         self,
     ) -> tuple[npt.NDArray[np.float_], npt.NDArray[np.complex_]]:
         eval_loc = f"{self.matrix_location}_eigenvalues.npy"
         evec_loc = f"{self.matrix_location}_eigenvectors.npy"
         try:
-            return np.load(
+            eigenvalues = np.load(
                 sleplet._data.setup_pooch.find_on_pooch_then_local(eval_loc),
-            ), np.load(sleplet._data.setup_pooch.find_on_pooch_then_local(evec_loc))
+            )
+            eigenvectors = np.load(
+                sleplet._data.setup_pooch.find_on_pooch_then_local(evec_loc),
+            )
         except TypeError:
             K = self._create_K_matrix()
             eigenvalues, eigenvectors = self._clean_evals_and_evecs(LA.eigh(K))
             np.save(user_data_path() / eval_loc, eigenvalues)
             np.save(user_data_path() / evec_loc, eigenvectors[: self.N])
-            return eigenvalues, eigenvectors
+        return eigenvalues, eigenvectors
 
     def _create_K_matrix(self) -> npt.NDArray[np.complex_]:  # noqa: N802
         """Computes the K matrix."""
         # Compute sub-integral matrix
         G = self._slepian_integral()
 
         # Compute Slepian matrix
```

### Comparing `sleplet-1.4.1/src/sleplet/slepian/slepian_polar_cap.py` & `sleplet-1.4.2/src/sleplet/slepian/slepian_polar_cap.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,17 +63,26 @@
     def _solve_eigenproblem(
         self,
     ) -> tuple[npt.NDArray[np.float_], npt.NDArray[np.complex_]]:
         eval_loc = f"{self.matrix_location}_eigenvalues.npy"
         evec_loc = f"{self.matrix_location}_eigenvectors.npy"
         order_loc = f"{self.matrix_location}_orders.npy"
         try:
-            return self._solve_eigenproblem_from_files(eval_loc, evec_loc, order_loc)
+            eigenvalues, eigenvectors = self._solve_eigenproblem_from_files(
+                eval_loc,
+                evec_loc,
+                order_loc,
+            )
         except TypeError:
-            return self._solve_eigenproblem_from_scratch(eval_loc, evec_loc, order_loc)
+            eigenvalues, eigenvectors = self._solve_eigenproblem_from_scratch(
+                eval_loc,
+                evec_loc,
+                order_loc,
+            )
+        return eigenvalues, eigenvectors
 
     def _solve_eigenproblem_from_files(
         self,
         eval_loc: str,
         evec_loc: str,
         order_loc: str,
     ) -> tuple[npt.NDArray[np.float_], npt.NDArray[np.complex_]]:
@@ -184,15 +193,15 @@
             for i in chunk:
                 _logger.info(f"start ell: {i}")
                 self._dm_matrix_helper(Dm_int, i, m, lvec, Pl, ell)
                 _logger.info(f"finish ell: {i}")
 
             sleplet._parallel_methods.free_shared_memory(shm_int)
 
-        # split up L range to maximise effiency
+        # split up L range to maximise efficiency
         ncpu = int(os.getenv("NCPU", "4"))
         _logger.info(f"Number of CPU={ncpu}")
         chunks = sleplet._parallel_methods.split_arr_into_chunks(
             self.L - m,
             ncpu,
         )
 
@@ -297,16 +306,16 @@
         else:
             t1 = l2 - l3 - m1
             t2 = l1 - l3 + m2
             t3 = l1 + l2 - l3
             t4 = l1 - m1
             t5 = l2 + m2
 
-            tmin = max(0, max(t1, t2))
-            tmax = min(t3, min(t4, t5))
+            tmin = max(0, t1, t2)
+            tmax = min(t3, t4, t5)
 
             # sum is over all those t for which the
             # following factorials have non-zero arguments
             s = sum(
                 (-1) ** t
                 / (
                     gp.factorial(t)
```

### Comparing `sleplet-1.4.1/src/sleplet/slepian_methods.py` & `sleplet-1.4.2/src/sleplet/slepian_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         The values on the sphere in pixel space.
     """
     f_p_reshape = f_p[: slepian.N, np.newaxis, np.newaxis]
     s_p = compute_s_p_omega(L, slepian)
     return (f_p_reshape * s_p).sum(axis=0)
 
 
-def slepian_forward(
+def slepian_forward(  # noqa: PLR0913
     L: int,
     slepian: SlepianFunctions,
     *,
     f: npt.NDArray[np.complex_] | None = None,
     flm: npt.NDArray[np.complex_ | np.float_] | None = None,
     mask: npt.NDArray[np.float_] | None = None,
     n_coeffs: int | None = None,
```

### Comparing `sleplet-1.4.1/src/sleplet/wavelet_methods.py` & `sleplet-1.4.2/src/sleplet/wavelet_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/src/sleplet.egg-info/PKG-INFO` & `sleplet-1.4.2/src/sleplet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleplet
-Version: 1.4.1
+Version: 1.4.2
 Summary: Slepian Scale-Discretised Wavelets in Python
 Author-email: "Patrick J. Roddy" <patrickjamesroddy@gmail.com>
 License: BSD 3-Clause Licence
         
         Copyright (c) 2017-2023, Patrick Roddy
         All rights reserved.
         
@@ -40,14 +40,15 @@
 Project-URL: Issues, https://github.com/astro-informatics/sleplet/issues
 Keywords: manifolds,python,slepian-functions,sphere,wavelets
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `sleplet-1.4.1/src/sleplet.egg-info/SOURCES.txt` & `sleplet-1.4.2/src/sleplet.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,14 @@
 src/sleplet/slepian/_slepian_decomposition.py
 src/sleplet/slepian/region.py
 src/sleplet/slepian/slepian_arbitrary.py
 src/sleplet/slepian/slepian_functions.py
 src/sleplet/slepian/slepian_limit_lat_lon.py
 src/sleplet/slepian/slepian_polar_cap.py
 tests/conftest.py
-tests/test_arbitrary_region.py
 tests/test_arrays.py
 tests/test_bool.py
 tests/test_convolution.py
 tests/test_decomposition.py
 tests/test_harmonic.py
 tests/test_loading_pooch.py
 tests/test_mesh.py
```

### Comparing `sleplet-1.4.1/tests/conftest.py` & `sleplet-1.4.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/tests/test_arrays.py` & `sleplet-1.4.2/tests/test_arrays.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/tests/test_bool.py` & `sleplet-1.4.2/tests/test_bool.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/tests/test_convolution.py` & `sleplet-1.4.2/tests/test_convolution.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     flm_conv = f.convolve(flm, g.coefficients)
     assert_array_equal(flm, flm_conv)
 
 
 def test_earth_harmonic_gaussian_convolution() -> None:
     """
     Test to ensure that convolving the Earth with the harmonic
-    Gausian does not change significantly change the map.
+    Gaussian does not change significantly change the map.
     """
     f = sleplet.functions.Earth(L)
     g = sleplet.functions.HarmonicGaussian(L)
     flm = f.coefficients
     flm_conv = f.convolve(flm, g.coefficients)
     assert_allclose(np.abs(flm_conv - flm).mean(), 0, atol=7)
```

### Comparing `sleplet-1.4.1/tests/test_decomposition.py` & `sleplet-1.4.2/tests/test_decomposition.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/tests/test_harmonic.py` & `sleplet-1.4.2/tests/test_harmonic.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/tests/test_loading_pooch.py` & `sleplet-1.4.2/tests/test_loading_pooch.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/tests/test_mesh.py` & `sleplet-1.4.2/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/tests/test_plot.py` & `sleplet-1.4.2/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/tests/test_region.py` & `sleplet-1.4.2/tests/test_region.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,21 +30,21 @@
 
 def test_arbitrary_region() -> None:
     """Tests that an arbitrary region is created."""
     region = sleplet.slepian.Region(mask_name=MASK)
     assert_equal(region.region_type, "arbitrary")
 
 
-def test_polar_hierarchy_over_arbirary() -> None:
+def test_polar_hierarchy_over_arbitrary() -> None:
     """Ensures polar cap is made instead of arbitrary."""
     region = sleplet.slepian.Region(theta_max=THETA_MAX, mask_name=MASK)
     assert_equal(region.region_type, "polar")
 
 
-def test_lim_lat_lon_hierarchy_over_arbirary() -> None:
+def test_lim_lat_lon_hierarchy_over_arbitrary() -> None:
     """Ensures limited latitude longitude region is made instead of arbitrary."""
     region = sleplet.slepian.Region(
         theta_min=THETA_0,
         theta_max=THETA_1,
         phi_min=PHI_0,
         phi_max=PHI_1,
         mask_name=MASK,
```

### Comparing `sleplet-1.4.1/tests/test_slepian_mesh.py` & `sleplet-1.4.2/tests/test_slepian_mesh.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/tests/test_strings.py` & `sleplet-1.4.2/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/tests/test_translation.py` & `sleplet-1.4.2/tests/test_translation.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.1/tests/test_wavelets.py` & `sleplet-1.4.2/tests/test_wavelets.py`

 * *Files identical despite different names*

