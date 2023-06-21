# Comparing `tmp/alphapulldown-0.30.6.tar.gz` & `tmp/alphapulldown-0.30.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphapulldown-0.30.6.tar", last modified: Wed May 24 14:18:11 2023, max compression
+gzip compressed data, was "alphapulldown-0.30.7.tar", last modified: Wed Jun 21 12:14:42 2023, max compression
```

## Comparing `alphapulldown-0.30.6.tar` & `alphapulldown-0.30.7.tar`

### file list

```diff
@@ -1,177 +1,176 @@
-drwxr-xr-x   0    24600      721        0 2023-05-24 14:18:10.000000 alphapulldown-0.30.6/
--rw-r--r--   0    24600      721    35149 2022-08-09 10:02:13.000000 alphapulldown-0.30.6/LICENSE
--rw-r--r--   0    24600      721       70 2023-04-18 11:12:17.000000 alphapulldown-0.30.6/MANIFEST.in
--rw-r--r--   0    24600      721      428 2023-05-24 14:18:10.000000 alphapulldown-0.30.6/PKG-INFO
--rw-r--r--   0    24600      721     5483 2023-05-24 13:23:45.000000 alphapulldown-0.30.6/README.md
-drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:17.000000 alphapulldown-0.30.6/alphafold/
-drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:18.000000 alphapulldown-0.30.6/alphafold/alphafold/
--rw-r--r--   0    24600      721      663 2023-05-16 14:00:32.000000 alphapulldown-0.30.6/alphafold/alphafold/__init__.py
-drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:20.000000 alphapulldown-0.30.6/alphafold/alphafold/common/
--rw-r--r--   0    24600      721      655 2023-05-16 14:00:32.000000 alphapulldown-0.30.6/alphafold/alphafold/common/__init__.py
--rw-r--r--   0    24600      721     6066 2023-05-16 14:00:33.000000 alphapulldown-0.30.6/alphafold/alphafold/common/confidence.py
--rw-r--r--   0    24600      721     9959 2023-05-16 14:00:33.000000 alphapulldown-0.30.6/alphafold/alphafold/common/protein.py
--rw-r--r--   0    24600      721     4594 2023-05-16 14:00:33.000000 alphapulldown-0.30.6/alphafold/alphafold/common/protein_test.py
--rw-r--r--   0    24600      721    34974 2023-05-16 14:00:33.000000 alphapulldown-0.30.6/alphafold/alphafold/common/residue_constants.py
--rw-r--r--   0    24600      721     9256 2023-05-16 14:00:33.000000 alphapulldown-0.30.6/alphafold/alphafold/common/residue_constants_test.py
-drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:23.000000 alphapulldown-0.30.6/alphafold/alphafold/data/
--rw-r--r--   0    24600      721      634 2023-05-16 14:00:34.000000 alphapulldown-0.30.6/alphafold/alphafold/data/__init__.py
--rw-r--r--   0    24600      721     8575 2023-05-16 14:00:35.000000 alphapulldown-0.30.6/alphafold/alphafold/data/feature_processing.py
--rw-r--r--   0    24600      721    14182 2023-05-16 14:00:35.000000 alphapulldown-0.30.6/alphafold/alphafold/data/mmcif_parsing.py
--rw-r--r--   0    24600      721     3229 2023-05-16 14:00:35.000000 alphapulldown-0.30.6/alphafold/alphafold/data/msa_identifiers.py
--rw-r--r--   0    24600      721    17220 2023-05-16 14:00:35.000000 alphapulldown-0.30.6/alphafold/alphafold/data/msa_pairing.py
--rw-r--r--   0    24600      721    21397 2023-05-16 14:00:35.000000 alphapulldown-0.30.6/alphafold/alphafold/data/parsers.py
--rw-r--r--   0    24600      721    10419 2023-05-16 14:00:35.000000 alphapulldown-0.30.6/alphafold/alphafold/data/pipeline.py
--rw-r--r--   0    24600      721    11126 2023-05-16 14:00:36.000000 alphapulldown-0.30.6/alphafold/alphafold/data/pipeline_multimer.py
--rw-r--r--   0    24600      721    40677 2023-05-16 14:00:36.000000 alphapulldown-0.30.6/alphafold/alphafold/data/templates.py
-drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:26.000000 alphapulldown-0.30.6/alphafold/alphafold/data/tools/
--rw-r--r--   0    24600      721      639 2023-05-16 14:00:36.000000 alphapulldown-0.30.6/alphafold/alphafold/data/tools/__init__.py
--rw-r--r--   0    24600      721     5504 2023-05-16 14:00:36.000000 alphapulldown-0.30.6/alphafold/alphafold/data/tools/hhblits.py
--rw-r--r--   0    24600      721     3601 2023-05-16 14:00:36.000000 alphapulldown-0.30.6/alphafold/alphafold/data/tools/hhsearch.py
--rw-r--r--   0    24600      721     4576 2023-05-16 14:00:37.000000 alphapulldown-0.30.6/alphafold/alphafold/data/tools/hmmbuild.py
--rw-r--r--   0    24600      721     4556 2023-05-16 14:00:37.000000 alphapulldown-0.30.6/alphafold/alphafold/data/tools/hmmsearch.py
--rw-r--r--   0    24600      721     8386 2023-05-16 14:00:37.000000 alphapulldown-0.30.6/alphafold/alphafold/data/tools/jackhmmer.py
--rw-r--r--   0    24600      721     3387 2023-05-16 14:00:37.000000 alphapulldown-0.30.6/alphafold/alphafold/data/tools/kalign.py
--rw-r--r--   0    24600      721     1223 2023-05-16 14:00:37.000000 alphapulldown-0.30.6/alphafold/alphafold/data/tools/utils.py
-drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:35.000000 alphapulldown-0.30.6/alphafold/alphafold/model/
--rw-r--r--   0    24600      721      617 2023-05-16 14:00:37.000000 alphapulldown-0.30.6/alphafold/alphafold/model/__init__.py
--rw-r--r--   0    24600      721    47028 2023-05-16 14:00:38.000000 alphapulldown-0.30.6/alphafold/alphafold/model/all_atom.py
--rw-r--r--   0    24600      721    40145 2023-05-16 14:00:38.000000 alphapulldown-0.30.6/alphafold/alphafold/model/all_atom_multimer.py
--rw-r--r--   0    24600      721     4706 2023-05-16 14:00:38.000000 alphapulldown-0.30.6/alphafold/alphafold/model/all_atom_test.py
--rw-r--r--   0    24600      721     5957 2023-05-16 14:00:38.000000 alphapulldown-0.30.6/alphafold/alphafold/model/common_modules.py
--rw-r--r--   0    24600      721    26814 2023-05-16 14:00:38.000000 alphapulldown-0.30.6/alphafold/alphafold/model/config.py
--rw-r--r--   0    24600      721     1097 2023-05-16 14:00:39.000000 alphapulldown-0.30.6/alphafold/alphafold/model/data.py
--rw-r--r--   0    24600      721     3692 2023-05-16 14:00:39.000000 alphapulldown-0.30.6/alphafold/alphafold/model/features.py
--rw-r--r--   0    24600      721    37264 2023-05-16 14:00:39.000000 alphapulldown-0.30.6/alphafold/alphafold/model/folding.py
--rw-r--r--   0    24600      721    42498 2023-05-16 14:00:39.000000 alphapulldown-0.30.6/alphafold/alphafold/model/folding_multimer.py
-drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:38.000000 alphapulldown-0.30.6/alphafold/alphafold/model/geometry/
--rw-r--r--   0    24600      721     1172 2023-05-16 14:00:40.000000 alphapulldown-0.30.6/alphafold/alphafold/model/geometry/__init__.py
--rw-r--r--   0    24600      721     4148 2023-05-16 14:00:40.000000 alphapulldown-0.30.6/alphafold/alphafold/model/geometry/rigid_matrix_vector.py
--rw-r--r--   0    24600      721     5751 2023-05-16 14:00:40.000000 alphapulldown-0.30.6/alphafold/alphafold/model/geometry/rotation_matrix.py
--rw-r--r--   0    24600      721     7745 2023-05-16 14:00:40.000000 alphapulldown-0.30.6/alphafold/alphafold/model/geometry/struct_of_array.py
--rw-r--r--   0    24600      721     4166 2023-05-16 14:00:40.000000 alphapulldown-0.30.6/alphafold/alphafold/model/geometry/test_utils.py
--rw-r--r--   0    24600      721      853 2023-05-16 14:00:40.000000 alphapulldown-0.30.6/alphafold/alphafold/model/geometry/utils.py
--rw-r--r--   0    24600      721     6896 2023-05-16 14:00:40.000000 alphapulldown-0.30.6/alphafold/alphafold/model/geometry/vector.py
--rw-r--r--   0    24600      721     9134 2023-05-16 14:00:41.000000 alphapulldown-0.30.6/alphafold/alphafold/model/layer_stack.py
--rw-r--r--   0    24600      721    10315 2023-05-16 14:00:41.000000 alphapulldown-0.30.6/alphafold/alphafold/model/layer_stack_test.py
--rw-r--r--   0    24600      721     3505 2023-05-16 14:00:41.000000 alphapulldown-0.30.6/alphafold/alphafold/model/lddt.py
--rw-r--r--   0    24600      721     2384 2023-05-16 14:00:41.000000 alphapulldown-0.30.6/alphafold/alphafold/model/lddt_test.py
--rw-r--r--   0    24600      721     7963 2023-05-16 14:00:41.000000 alphapulldown-0.30.6/alphafold/alphafold/model/mapping.py
--rw-r--r--   0    24600      721     6613 2023-05-16 14:00:41.000000 alphapulldown-0.30.6/alphafold/alphafold/model/model.py
--rw-r--r--   0    24600      721    74120 2023-05-16 14:00:42.000000 alphapulldown-0.30.6/alphafold/alphafold/model/modules.py
--rw-r--r--   0    24600      721    42228 2023-05-16 14:00:42.000000 alphapulldown-0.30.6/alphafold/alphafold/model/modules_multimer.py
--rw-r--r--   0    24600      721     1978 2023-05-16 14:00:42.000000 alphapulldown-0.30.6/alphafold/alphafold/model/prng.py
--rw-r--r--   0    24600      721     1250 2023-05-16 14:00:42.000000 alphapulldown-0.30.6/alphafold/alphafold/model/prng_test.py
--rw-r--r--   0    24600      721    17388 2023-05-16 14:00:42.000000 alphapulldown-0.30.6/alphafold/alphafold/model/quat_affine.py
--rw-r--r--   0    24600      721     5038 2023-05-16 14:00:42.000000 alphapulldown-0.30.6/alphafold/alphafold/model/quat_affine_test.py
--rw-r--r--   0    24600      721    10935 2023-05-16 14:00:43.000000 alphapulldown-0.30.6/alphafold/alphafold/model/r3.py
-drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:42.000000 alphapulldown-0.30.6/alphafold/alphafold/model/tf/
--rw-r--r--   0    24600      721      633 2023-05-16 14:00:43.000000 alphapulldown-0.30.6/alphafold/alphafold/model/tf/__init__.py
--rw-r--r--   0    24600      721    21428 2023-05-16 14:00:43.000000 alphapulldown-0.30.6/alphafold/alphafold/model/tf/data_transforms.py
--rw-r--r--   0    24600      721     5357 2023-05-16 14:00:43.000000 alphapulldown-0.30.6/alphafold/alphafold/model/tf/input_pipeline.py
--rw-r--r--   0    24600      721     5051 2023-05-16 14:00:43.000000 alphapulldown-0.30.6/alphafold/alphafold/model/tf/protein_features.py
--rw-r--r--   0    24600      721     1822 2023-05-16 14:00:43.000000 alphapulldown-0.30.6/alphafold/alphafold/model/tf/protein_features_test.py
--rw-r--r--   0    24600      721     6344 2023-05-16 14:00:44.000000 alphapulldown-0.30.6/alphafold/alphafold/model/tf/proteins_dataset.py
--rw-r--r--   0    24600      721     1415 2023-05-16 14:00:44.000000 alphapulldown-0.30.6/alphafold/alphafold/model/tf/shape_helpers.py
--rw-r--r--   0    24600      721     1318 2023-05-16 14:00:44.000000 alphapulldown-0.30.6/alphafold/alphafold/model/tf/shape_helpers_test.py
--rw-r--r--   0    24600      721      812 2023-05-16 14:00:44.000000 alphapulldown-0.30.6/alphafold/alphafold/model/tf/shape_placeholders.py
--rw-r--r--   0    24600      721     1276 2023-05-16 14:00:44.000000 alphapulldown-0.30.6/alphafold/alphafold/model/tf/utils.py
--rw-r--r--   0    24600      721     5328 2023-05-16 14:00:44.000000 alphapulldown-0.30.6/alphafold/alphafold/model/utils.py
-drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:43.000000 alphapulldown-0.30.6/alphafold/alphafold/notebooks/
--rw-r--r--   0    24600      721      626 2023-05-16 14:00:45.000000 alphapulldown-0.30.6/alphafold/alphafold/notebooks/__init__.py
--rw-r--r--   0    24600      721     7520 2023-05-16 14:00:45.000000 alphapulldown-0.30.6/alphafold/alphafold/notebooks/notebook_utils.py
--rw-r--r--   0    24600      721     9571 2023-05-16 14:00:45.000000 alphapulldown-0.30.6/alphafold/alphafold/notebooks/notebook_utils_test.py
-drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:46.000000 alphapulldown-0.30.6/alphafold/alphafold/relax/
--rw-r--r--   0    24600      721      618 2023-05-16 14:00:45.000000 alphapulldown-0.30.6/alphafold/alphafold/relax/__init__.py
--rw-r--r--   0    24600      721    19061 2023-05-16 14:00:45.000000 alphapulldown-0.30.6/alphafold/alphafold/relax/amber_minimize.py
--rw-r--r--   0    24600      721     4348 2023-05-16 14:00:46.000000 alphapulldown-0.30.6/alphafold/alphafold/relax/amber_minimize_test.py
--rw-r--r--   0    24600      721     4832 2023-05-16 14:00:46.000000 alphapulldown-0.30.6/alphafold/alphafold/relax/cleanup.py
--rw-r--r--   0    24600      721     6170 2023-05-16 14:00:46.000000 alphapulldown-0.30.6/alphafold/alphafold/relax/cleanup_test.py
--rw-r--r--   0    24600      721     3288 2023-05-16 14:00:46.000000 alphapulldown-0.30.6/alphafold/alphafold/relax/relax.py
--rw-r--r--   0    24600      721     3827 2023-05-16 14:00:46.000000 alphapulldown-0.30.6/alphafold/alphafold/relax/relax_test.py
--rw-r--r--   0    24600      721     2501 2023-05-16 14:00:48.000000 alphapulldown-0.30.6/alphafold/alphafold/relax/utils.py
--rw-r--r--   0    24600      721     1996 2023-05-16 14:00:48.000000 alphapulldown-0.30.6/alphafold/alphafold/relax/utils_test.py
--rw-r--r--   0    24600      721    19606 2023-05-19 10:39:58.000000 alphapulldown-0.30.6/alphafold/run_alphafold.py
--rw-r--r--   0    24600      721     3814 2023-05-16 14:00:59.000000 alphapulldown-0.30.6/alphafold/run_alphafold_test.py
--rw-r--r--   0    24600      721     2064 2023-05-16 14:01:01.000000 alphapulldown-0.30.6/alphafold/setup.py
-drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:49.000000 alphapulldown-0.30.6/alphapulldown/
-drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:12.000000 alphapulldown-0.30.6/alphapulldown/ColabFold/
-drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:55.000000 alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/
--rw-r--r--   0    24600      721        0 2023-05-16 09:15:18.000000 alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/__init__.py
--rw-r--r--   0    24600      721    65347 2023-05-16 11:20:06.000000 alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/batch.py
--rw-r--r--   0    24600      721     5988 2023-05-16 11:20:07.000000 alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/citations.py
--rw-r--r--   0    24600      721    24980 2023-05-16 11:20:07.000000 alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/colabfold.py
--rw-r--r--   0    24600      721    32656 2023-05-16 11:20:07.000000 alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/colabfold_alphafold.py
--rw-r--r--   0    24600      721     1982 2023-05-16 11:20:07.000000 alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/download.py
--rw-r--r--   0    24600      721     2120 2023-05-16 09:15:21.000000 alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/pdb.py
--rw-r--r--   0    24600      721     3419 2023-05-16 11:20:07.000000 alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/plot.py
--rw-r--r--   0    24600      721     9954 2023-05-16 11:20:08.000000 alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/utils.py
--rw-r--r--   0    24600      721        0 2023-01-27 13:02:50.000000 alphapulldown-0.30.6/alphapulldown/__init__.py
-drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:57.000000 alphapulldown-0.30.6/alphapulldown/analysis_pipeline/
--rw-r--r--   0    24600      721     7268 2023-03-14 10:54:09.000000 alphapulldown-0.30.6/alphapulldown/analysis_pipeline/af2_3dmol.py
-drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:57.000000 alphapulldown-0.30.6/alphapulldown/analysis_pipeline/af2_plots/
-drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:58.000000 alphapulldown-0.30.6/alphapulldown/analysis_pipeline/af2_plots/af2plots/
--rw-r--r--   0    24600      721        0 2023-05-16 12:08:43.000000 alphapulldown-0.30.6/alphapulldown/analysis_pipeline/af2_plots/af2plots/__init__.py
--rw-r--r--   0    24600      721     3745 2023-05-16 11:50:17.000000 alphapulldown-0.30.6/alphapulldown/analysis_pipeline/af2_plots/af2plots/__main__.py
--rw-r--r--   0    24600      721    15555 2023-05-16 11:50:17.000000 alphapulldown-0.30.6/alphapulldown/analysis_pipeline/af2_plots/af2plots/plotter.py
--rw-r--r--   0    24600      721       21 2023-05-16 11:50:18.000000 alphapulldown-0.30.6/alphapulldown/analysis_pipeline/af2_plots/af2plots/version.py
--rw-r--r--   0    24600      721      851 2023-05-16 11:51:00.000000 alphapulldown-0.30.6/alphapulldown/analysis_pipeline/af2_plots/setup.py
--rw-rw-r--   0    24600      721     6028 2023-01-27 13:24:19.000000 alphapulldown-0.30.6/alphapulldown/analysis_pipeline/calculate_mpdockq.py
--rw-r--r--   0    24600      721     5510 2023-01-27 13:03:03.000000 alphapulldown-0.30.6/alphapulldown/analysis_pipeline/create_notebook.py
--rw-r--r--   0    24600      721     6520 2023-01-27 13:24:19.000000 alphapulldown-0.30.6/alphapulldown/analysis_pipeline/get_good_inter_pae.py
--rw-r--r--   0    24600      721      962 2023-01-27 13:03:03.000000 alphapulldown-0.30.6/alphapulldown/analysis_pipeline/utils.py
--rwxr-xr-x   0    24600      721    10571 2023-04-19 11:33:53.000000 alphapulldown-0.30.6/alphapulldown/create_individual_features.py
--rw-r--r--   0    24600      721    22205 2023-04-19 11:33:53.000000 alphapulldown-0.30.6/alphapulldown/objects.py
--rw-r--r--   0    24600      721     1822 2023-03-14 16:09:43.000000 alphapulldown-0.30.6/alphapulldown/plot_pae.py
--rw-r--r--   0    24600      721     8878 2023-04-18 11:12:23.000000 alphapulldown-0.30.6/alphapulldown/predict_structure.py
--rwxr-xr-x   0    24600      721     1166 2023-03-14 16:09:44.000000 alphapulldown-0.30.6/alphapulldown/prepare_seq_names.py
--rwxr-xr-x   0    24600      721     1261 2023-03-14 16:09:44.000000 alphapulldown-0.30.6/alphapulldown/rename_colab_search_a3m.py
--rw-r--r--   0    24600      721    11611 2023-05-24 13:19:32.000000 alphapulldown-0.30.6/alphapulldown/run_multimer_jobs.py
--rw-r--r--   0    24600      721    11546 2023-05-24 14:16:37.000000 alphapulldown-0.30.6/alphapulldown/utils.py
-drwxr-xr-x   0    24600      721        0 2023-05-24 14:18:09.000000 alphapulldown-0.30.6/alphapulldown.egg-info/
--rw-r--r--   0    24600      721     4096 2023-05-19 09:47:48.000000 alphapulldown-0.30.6/alphapulldown.egg-info/._PKG-INFO
--rw-r--r--   0    24600      721     4096 2023-05-19 09:47:58.000000 alphapulldown-0.30.6/alphapulldown.egg-info/._SOURCES.txt
--rw-r--r--   0    24600      721     4096 2023-05-19 09:47:49.000000 alphapulldown-0.30.6/alphapulldown.egg-info/._dependency_links.txt
--rw-r--r--   0    24600      721     4096 2023-05-19 09:47:50.000000 alphapulldown-0.30.6/alphapulldown.egg-info/._requires.txt
--rw-r--r--   0    24600      721     4096 2023-05-19 09:47:50.000000 alphapulldown-0.30.6/alphapulldown.egg-info/._top_level.txt
--rw-r--r--   0    24600      721      428 2023-05-24 14:17:09.000000 alphapulldown-0.30.6/alphapulldown.egg-info/PKG-INFO
--rw-r--r--   0    24600      721     6248 2023-05-24 14:17:10.000000 alphapulldown-0.30.6/alphapulldown.egg-info/SOURCES.txt
--rw-r--r--   0    24600      721        1 2023-05-24 14:17:09.000000 alphapulldown-0.30.6/alphapulldown.egg-info/dependency_links.txt
--rw-r--r--   0    24600      721      262 2023-05-24 14:17:10.000000 alphapulldown-0.30.6/alphapulldown.egg-info/requires.txt
--rw-r--r--   0    24600      721       61 2023-05-24 14:17:10.000000 alphapulldown-0.30.6/alphapulldown.egg-info/top_level.txt
-drwxr-xr-x   0    24600      721        0 2023-05-24 14:18:02.000000 alphapulldown-0.30.6/colabfold/
--rw-r--r--   0    24600      721        0 2023-04-06 09:21:34.000000 alphapulldown-0.30.6/colabfold/__init__.py
-drwxr-xr-x   0    24600      721        0 2023-05-24 14:18:03.000000 alphapulldown-0.30.6/colabfold/alphafold/
--rw-r--r--   0    24600      721        0 2023-04-06 09:21:34.000000 alphapulldown-0.30.6/colabfold/alphafold/__init__.py
--rw-r--r--   0    24600      721     5923 2023-04-06 09:21:34.000000 alphapulldown-0.30.6/colabfold/alphafold/models.py
--rw-r--r--   0    24600      721     1565 2023-04-06 09:21:34.000000 alphapulldown-0.30.6/colabfold/alphafold/msa.py
--rw-r--r--   0    24600      721    65347 2023-04-06 09:21:34.000000 alphapulldown-0.30.6/colabfold/batch.py
--rw-r--r--   0    24600      721     5988 2023-04-06 09:21:34.000000 alphapulldown-0.30.6/colabfold/citations.py
--rw-r--r--   0    24600      721    24980 2023-04-06 09:21:34.000000 alphapulldown-0.30.6/colabfold/colabfold.py
--rw-r--r--   0    24600      721    32656 2023-04-06 09:21:34.000000 alphapulldown-0.30.6/colabfold/colabfold_alphafold.py
--rw-r--r--   0    24600      721     1982 2023-04-06 09:21:34.000000 alphapulldown-0.30.6/colabfold/download.py
-drwxr-xr-x   0    24600      721        0 2023-05-24 14:18:04.000000 alphapulldown-0.30.6/colabfold/mmseqs/
--rw-r--r--   0    24600      721        0 2023-04-06 09:21:34.000000 alphapulldown-0.30.6/colabfold/mmseqs/__init__.py
--rw-r--r--   0    24600      721     1933 2023-04-06 09:21:34.000000 alphapulldown-0.30.6/colabfold/mmseqs/merge_and_split_msas.py
--rw-r--r--   0    24600      721    18799 2023-04-06 09:21:34.000000 alphapulldown-0.30.6/colabfold/mmseqs/search.py
--rw-r--r--   0    24600      721     1429 2023-04-06 09:21:34.000000 alphapulldown-0.30.6/colabfold/mmseqs/split_msas.py
--rw-r--r--   0    24600      721     2120 2023-04-06 09:21:34.000000 alphapulldown-0.30.6/colabfold/pdb.py
--rw-r--r--   0    24600      721     3419 2023-04-06 09:21:35.000000 alphapulldown-0.30.6/colabfold/plot.py
--rw-r--r--   0    24600      721     9954 2023-04-06 09:21:35.000000 alphapulldown-0.30.6/colabfold/utils.py
--rw-r--r--   0    24600      721      140 2023-04-05 11:02:03.000000 alphapulldown-0.30.6/pyproject.toml
--rw-r--r--   0    24600      721     1470 2023-05-24 14:18:10.000000 alphapulldown-0.30.6/setup.cfg
--rwxr-xr-x   0    24600      721       67 2023-04-18 11:12:27.000000 alphapulldown-0.30.6/setup.py
--rw-r--r--   0    24600      721     9119 2023-04-18 11:12:28.000000 alphapulldown-0.30.6/stereo_chemical_props.txt
-drwxr-xr-x   0    24600      721        0 2023-05-24 14:18:10.000000 alphapulldown-0.30.6/test/
--rw-r--r--   0    24600      721     4546 2023-04-19 11:33:54.000000 alphapulldown-0.30.6/test/test_create_objects.py
--rwxr-xr-x   0    24600      721    12809 2023-05-19 10:38:44.000000 alphapulldown-0.30.6/test/test_predict_structure.py
-drwxr-xr-x   0    24600      721        0 2023-05-24 14:17:13.000000 alphapulldown-0.30.6/unifold/
-drwxr-xr-x   0    24600      721        0 2023-05-24 14:18:07.000000 alphapulldown-0.30.6/unifold/unifold/
--rw-r--r--   0    24600      721       72 2023-05-19 11:17:04.000000 alphapulldown-0.30.6/unifold/unifold/__init__.py
--rw-r--r--   0    24600      721    25459 2023-05-24 12:02:28.000000 alphapulldown-0.30.6/unifold/unifold/config.py
--rw-r--r--   0    24600      721    21165 2023-05-24 12:02:54.000000 alphapulldown-0.30.6/unifold/unifold/dataset.py
--rw-r--r--   0    24600      721    10412 2023-05-19 11:17:20.000000 alphapulldown-0.30.6/unifold/unifold/homo_search.py
--rw-r--r--   0    24600      721    16351 2023-05-24 12:02:55.000000 alphapulldown-0.30.6/unifold/unifold/inference.py
--rw-r--r--   0    24600      721     7587 2023-05-19 11:17:22.000000 alphapulldown-0.30.6/unifold/unifold/inference_symmetry.py
--rw-r--r--   0    24600      721     9457 2023-05-19 11:17:23.000000 alphapulldown-0.30.6/unifold/unifold/loss.py
--rw-r--r--   0    24600      721     1453 2023-05-19 11:17:30.000000 alphapulldown-0.30.6/unifold/unifold/model.py
--rw-r--r--   0    24600      721     2445 2023-05-19 11:18:12.000000 alphapulldown-0.30.6/unifold/unifold/task.py
+drwxr-xr-x   0    24600      721        0 2023-06-21 12:14:41.000000 alphapulldown-0.30.7/
+-rw-r--r--   0    24600      721    35149 2022-08-09 10:02:13.000000 alphapulldown-0.30.7/LICENSE
+-rw-r--r--   0    24600      721       80 2023-06-21 11:54:50.000000 alphapulldown-0.30.7/MANIFEST.in
+-rw-r--r--   0    24600      721      428 2023-06-21 12:14:41.000000 alphapulldown-0.30.7/PKG-INFO
+-rw-r--r--   0    24600      721     5771 2023-06-02 12:21:35.000000 alphapulldown-0.30.7/README.md
+drwxr-xr-x   0    24600      721        0 2023-06-21 12:13:45.000000 alphapulldown-0.30.7/alphafold/
+drwxr-xr-x   0    24600      721        0 2023-06-21 12:13:46.000000 alphapulldown-0.30.7/alphafold/alphafold/
+-rw-r--r--   0    24600      721      663 2023-05-16 14:00:32.000000 alphapulldown-0.30.7/alphafold/alphafold/__init__.py
+drwxr-xr-x   0    24600      721        0 2023-06-21 12:13:48.000000 alphapulldown-0.30.7/alphafold/alphafold/common/
+-rw-r--r--   0    24600      721      655 2023-05-16 14:00:32.000000 alphapulldown-0.30.7/alphafold/alphafold/common/__init__.py
+-rw-r--r--   0    24600      721     6066 2023-05-16 14:00:33.000000 alphapulldown-0.30.7/alphafold/alphafold/common/confidence.py
+-rw-r--r--   0    24600      721     9959 2023-05-16 14:00:33.000000 alphapulldown-0.30.7/alphafold/alphafold/common/protein.py
+-rw-r--r--   0    24600      721     4594 2023-05-16 14:00:33.000000 alphapulldown-0.30.7/alphafold/alphafold/common/protein_test.py
+-rw-r--r--   0    24600      721    34974 2023-05-16 14:00:33.000000 alphapulldown-0.30.7/alphafold/alphafold/common/residue_constants.py
+-rw-r--r--   0    24600      721     9256 2023-05-16 14:00:33.000000 alphapulldown-0.30.7/alphafold/alphafold/common/residue_constants_test.py
+drwxr-xr-x   0    24600      721        0 2023-06-21 12:13:51.000000 alphapulldown-0.30.7/alphafold/alphafold/data/
+-rw-r--r--   0    24600      721      634 2023-05-16 14:00:34.000000 alphapulldown-0.30.7/alphafold/alphafold/data/__init__.py
+-rw-r--r--   0    24600      721     8575 2023-05-16 14:00:35.000000 alphapulldown-0.30.7/alphafold/alphafold/data/feature_processing.py
+-rw-r--r--   0    24600      721    14182 2023-05-16 14:00:35.000000 alphapulldown-0.30.7/alphafold/alphafold/data/mmcif_parsing.py
+-rw-r--r--   0    24600      721     3229 2023-05-16 14:00:35.000000 alphapulldown-0.30.7/alphafold/alphafold/data/msa_identifiers.py
+-rw-r--r--   0    24600      721    17220 2023-05-16 14:00:35.000000 alphapulldown-0.30.7/alphafold/alphafold/data/msa_pairing.py
+-rw-r--r--   0    24600      721    21397 2023-05-16 14:00:35.000000 alphapulldown-0.30.7/alphafold/alphafold/data/parsers.py
+-rw-r--r--   0    24600      721    10419 2023-05-16 14:00:35.000000 alphapulldown-0.30.7/alphafold/alphafold/data/pipeline.py
+-rw-r--r--   0    24600      721    11126 2023-05-16 14:00:36.000000 alphapulldown-0.30.7/alphafold/alphafold/data/pipeline_multimer.py
+-rw-r--r--   0    24600      721    40677 2023-05-16 14:00:36.000000 alphapulldown-0.30.7/alphafold/alphafold/data/templates.py
+drwxr-xr-x   0    24600      721        0 2023-06-21 12:13:55.000000 alphapulldown-0.30.7/alphafold/alphafold/data/tools/
+-rw-r--r--   0    24600      721      639 2023-05-16 14:00:36.000000 alphapulldown-0.30.7/alphafold/alphafold/data/tools/__init__.py
+-rw-r--r--   0    24600      721     5504 2023-05-16 14:00:36.000000 alphapulldown-0.30.7/alphafold/alphafold/data/tools/hhblits.py
+-rw-r--r--   0    24600      721     3601 2023-05-16 14:00:36.000000 alphapulldown-0.30.7/alphafold/alphafold/data/tools/hhsearch.py
+-rw-r--r--   0    24600      721     4576 2023-05-16 14:00:37.000000 alphapulldown-0.30.7/alphafold/alphafold/data/tools/hmmbuild.py
+-rw-r--r--   0    24600      721     4556 2023-05-16 14:00:37.000000 alphapulldown-0.30.7/alphafold/alphafold/data/tools/hmmsearch.py
+-rw-r--r--   0    24600      721     8386 2023-05-16 14:00:37.000000 alphapulldown-0.30.7/alphafold/alphafold/data/tools/jackhmmer.py
+-rw-r--r--   0    24600      721     3387 2023-05-16 14:00:37.000000 alphapulldown-0.30.7/alphafold/alphafold/data/tools/kalign.py
+-rw-r--r--   0    24600      721     1223 2023-05-16 14:00:37.000000 alphapulldown-0.30.7/alphafold/alphafold/data/tools/utils.py
+drwxr-xr-x   0    24600      721        0 2023-06-21 12:14:05.000000 alphapulldown-0.30.7/alphafold/alphafold/model/
+-rw-r--r--   0    24600      721      617 2023-05-16 14:00:37.000000 alphapulldown-0.30.7/alphafold/alphafold/model/__init__.py
+-rw-r--r--   0    24600      721    47028 2023-05-16 14:00:38.000000 alphapulldown-0.30.7/alphafold/alphafold/model/all_atom.py
+-rw-r--r--   0    24600      721    40145 2023-05-16 14:00:38.000000 alphapulldown-0.30.7/alphafold/alphafold/model/all_atom_multimer.py
+-rw-r--r--   0    24600      721     4706 2023-05-16 14:00:38.000000 alphapulldown-0.30.7/alphafold/alphafold/model/all_atom_test.py
+-rw-r--r--   0    24600      721     5957 2023-05-16 14:00:38.000000 alphapulldown-0.30.7/alphafold/alphafold/model/common_modules.py
+-rw-r--r--   0    24600      721    26814 2023-05-16 14:00:38.000000 alphapulldown-0.30.7/alphafold/alphafold/model/config.py
+-rw-r--r--   0    24600      721     1097 2023-05-16 14:00:39.000000 alphapulldown-0.30.7/alphafold/alphafold/model/data.py
+-rw-r--r--   0    24600      721     3692 2023-05-16 14:00:39.000000 alphapulldown-0.30.7/alphafold/alphafold/model/features.py
+-rw-r--r--   0    24600      721    37264 2023-05-16 14:00:39.000000 alphapulldown-0.30.7/alphafold/alphafold/model/folding.py
+-rw-r--r--   0    24600      721    42498 2023-05-16 14:00:39.000000 alphapulldown-0.30.7/alphafold/alphafold/model/folding_multimer.py
+drwxr-xr-x   0    24600      721        0 2023-06-21 12:14:07.000000 alphapulldown-0.30.7/alphafold/alphafold/model/geometry/
+-rw-r--r--   0    24600      721     1172 2023-05-16 14:00:40.000000 alphapulldown-0.30.7/alphafold/alphafold/model/geometry/__init__.py
+-rw-r--r--   0    24600      721     4148 2023-05-16 14:00:40.000000 alphapulldown-0.30.7/alphafold/alphafold/model/geometry/rigid_matrix_vector.py
+-rw-r--r--   0    24600      721     5751 2023-05-16 14:00:40.000000 alphapulldown-0.30.7/alphafold/alphafold/model/geometry/rotation_matrix.py
+-rw-r--r--   0    24600      721     7745 2023-05-16 14:00:40.000000 alphapulldown-0.30.7/alphafold/alphafold/model/geometry/struct_of_array.py
+-rw-r--r--   0    24600      721     4166 2023-05-16 14:00:40.000000 alphapulldown-0.30.7/alphafold/alphafold/model/geometry/test_utils.py
+-rw-r--r--   0    24600      721      853 2023-05-16 14:00:40.000000 alphapulldown-0.30.7/alphafold/alphafold/model/geometry/utils.py
+-rw-r--r--   0    24600      721     6896 2023-05-16 14:00:40.000000 alphapulldown-0.30.7/alphafold/alphafold/model/geometry/vector.py
+-rw-r--r--   0    24600      721     9134 2023-05-16 14:00:41.000000 alphapulldown-0.30.7/alphafold/alphafold/model/layer_stack.py
+-rw-r--r--   0    24600      721    10315 2023-05-16 14:00:41.000000 alphapulldown-0.30.7/alphafold/alphafold/model/layer_stack_test.py
+-rw-r--r--   0    24600      721     3505 2023-05-16 14:00:41.000000 alphapulldown-0.30.7/alphafold/alphafold/model/lddt.py
+-rw-r--r--   0    24600      721     2384 2023-05-16 14:00:41.000000 alphapulldown-0.30.7/alphafold/alphafold/model/lddt_test.py
+-rw-r--r--   0    24600      721     7963 2023-05-16 14:00:41.000000 alphapulldown-0.30.7/alphafold/alphafold/model/mapping.py
+-rw-r--r--   0    24600      721     6613 2023-05-16 14:00:41.000000 alphapulldown-0.30.7/alphafold/alphafold/model/model.py
+-rw-r--r--   0    24600      721    74120 2023-05-16 14:00:42.000000 alphapulldown-0.30.7/alphafold/alphafold/model/modules.py
+-rw-r--r--   0    24600      721    42228 2023-05-16 14:00:42.000000 alphapulldown-0.30.7/alphafold/alphafold/model/modules_multimer.py
+-rw-r--r--   0    24600      721     1978 2023-05-16 14:00:42.000000 alphapulldown-0.30.7/alphafold/alphafold/model/prng.py
+-rw-r--r--   0    24600      721     1250 2023-05-16 14:00:42.000000 alphapulldown-0.30.7/alphafold/alphafold/model/prng_test.py
+-rw-r--r--   0    24600      721    17388 2023-05-16 14:00:42.000000 alphapulldown-0.30.7/alphafold/alphafold/model/quat_affine.py
+-rw-r--r--   0    24600      721     5038 2023-05-16 14:00:42.000000 alphapulldown-0.30.7/alphafold/alphafold/model/quat_affine_test.py
+-rw-r--r--   0    24600      721    10935 2023-05-16 14:00:43.000000 alphapulldown-0.30.7/alphafold/alphafold/model/r3.py
+drwxr-xr-x   0    24600      721        0 2023-06-21 12:14:11.000000 alphapulldown-0.30.7/alphafold/alphafold/model/tf/
+-rw-r--r--   0    24600      721      633 2023-05-16 14:00:43.000000 alphapulldown-0.30.7/alphafold/alphafold/model/tf/__init__.py
+-rw-r--r--   0    24600      721    21428 2023-05-16 14:00:43.000000 alphapulldown-0.30.7/alphafold/alphafold/model/tf/data_transforms.py
+-rw-r--r--   0    24600      721     5357 2023-05-16 14:00:43.000000 alphapulldown-0.30.7/alphafold/alphafold/model/tf/input_pipeline.py
+-rw-r--r--   0    24600      721     5051 2023-05-16 14:00:43.000000 alphapulldown-0.30.7/alphafold/alphafold/model/tf/protein_features.py
+-rw-r--r--   0    24600      721     1822 2023-05-16 14:00:43.000000 alphapulldown-0.30.7/alphafold/alphafold/model/tf/protein_features_test.py
+-rw-r--r--   0    24600      721     6344 2023-05-16 14:00:44.000000 alphapulldown-0.30.7/alphafold/alphafold/model/tf/proteins_dataset.py
+-rw-r--r--   0    24600      721     1415 2023-05-16 14:00:44.000000 alphapulldown-0.30.7/alphafold/alphafold/model/tf/shape_helpers.py
+-rw-r--r--   0    24600      721     1318 2023-05-16 14:00:44.000000 alphapulldown-0.30.7/alphafold/alphafold/model/tf/shape_helpers_test.py
+-rw-r--r--   0    24600      721      812 2023-05-16 14:00:44.000000 alphapulldown-0.30.7/alphafold/alphafold/model/tf/shape_placeholders.py
+-rw-r--r--   0    24600      721     1276 2023-05-16 14:00:44.000000 alphapulldown-0.30.7/alphafold/alphafold/model/tf/utils.py
+-rw-r--r--   0    24600      721     5328 2023-06-21 12:01:54.000000 alphapulldown-0.30.7/alphafold/alphafold/model/utils.py
+drwxr-xr-x   0    24600      721        0 2023-06-21 12:14:13.000000 alphapulldown-0.30.7/alphafold/alphafold/notebooks/
+-rw-r--r--   0    24600      721      626 2023-05-16 14:00:45.000000 alphapulldown-0.30.7/alphafold/alphafold/notebooks/__init__.py
+-rw-r--r--   0    24600      721     7520 2023-05-16 14:00:45.000000 alphapulldown-0.30.7/alphafold/alphafold/notebooks/notebook_utils.py
+-rw-r--r--   0    24600      721     9571 2023-05-16 14:00:45.000000 alphapulldown-0.30.7/alphafold/alphafold/notebooks/notebook_utils_test.py
+drwxr-xr-x   0    24600      721        0 2023-06-21 12:14:16.000000 alphapulldown-0.30.7/alphafold/alphafold/relax/
+-rw-r--r--   0    24600      721      618 2023-05-16 14:00:45.000000 alphapulldown-0.30.7/alphafold/alphafold/relax/__init__.py
+-rw-r--r--   0    24600      721    19061 2023-05-16 14:00:45.000000 alphapulldown-0.30.7/alphafold/alphafold/relax/amber_minimize.py
+-rw-r--r--   0    24600      721     4348 2023-05-16 14:00:46.000000 alphapulldown-0.30.7/alphafold/alphafold/relax/amber_minimize_test.py
+-rw-r--r--   0    24600      721     4832 2023-05-16 14:00:46.000000 alphapulldown-0.30.7/alphafold/alphafold/relax/cleanup.py
+-rw-r--r--   0    24600      721     6170 2023-05-16 14:00:46.000000 alphapulldown-0.30.7/alphafold/alphafold/relax/cleanup_test.py
+-rw-r--r--   0    24600      721     3288 2023-05-16 14:00:46.000000 alphapulldown-0.30.7/alphafold/alphafold/relax/relax.py
+-rw-r--r--   0    24600      721     3827 2023-05-16 14:00:46.000000 alphapulldown-0.30.7/alphafold/alphafold/relax/relax_test.py
+-rw-r--r--   0    24600      721     2501 2023-05-16 14:00:48.000000 alphapulldown-0.30.7/alphafold/alphafold/relax/utils.py
+-rw-r--r--   0    24600      721     1996 2023-05-16 14:00:48.000000 alphapulldown-0.30.7/alphafold/alphafold/relax/utils_test.py
+-rw-r--r--   0    24600      721    19606 2023-06-06 10:25:24.000000 alphapulldown-0.30.7/alphafold/alphafold/run_alphafold.py
+-rw-r--r--   0    24600      721     2064 2023-05-16 14:01:01.000000 alphapulldown-0.30.7/alphafold/setup.py
+drwxr-xr-x   0    24600      721        0 2023-06-21 12:14:20.000000 alphapulldown-0.30.7/alphapulldown/
+drwxr-xr-x   0    24600      721        0 2023-06-21 12:13:41.000000 alphapulldown-0.30.7/alphapulldown/ColabFold/
+drwxr-xr-x   0    24600      721        0 2023-06-21 12:14:25.000000 alphapulldown-0.30.7/alphapulldown/ColabFold/colabfold/
+-rw-r--r--   0    24600      721        0 2023-05-16 09:15:18.000000 alphapulldown-0.30.7/alphapulldown/ColabFold/colabfold/__init__.py
+-rw-r--r--   0    24600      721    65347 2023-05-16 11:20:06.000000 alphapulldown-0.30.7/alphapulldown/ColabFold/colabfold/batch.py
+-rw-r--r--   0    24600      721     5988 2023-05-16 11:20:07.000000 alphapulldown-0.30.7/alphapulldown/ColabFold/colabfold/citations.py
+-rw-r--r--   0    24600      721    24980 2023-05-16 11:20:07.000000 alphapulldown-0.30.7/alphapulldown/ColabFold/colabfold/colabfold.py
+-rw-r--r--   0    24600      721    32656 2023-05-16 11:20:07.000000 alphapulldown-0.30.7/alphapulldown/ColabFold/colabfold/colabfold_alphafold.py
+-rw-r--r--   0    24600      721     1982 2023-05-16 11:20:07.000000 alphapulldown-0.30.7/alphapulldown/ColabFold/colabfold/download.py
+-rw-r--r--   0    24600      721     2120 2023-05-16 09:15:21.000000 alphapulldown-0.30.7/alphapulldown/ColabFold/colabfold/pdb.py
+-rw-r--r--   0    24600      721     3419 2023-05-16 11:20:07.000000 alphapulldown-0.30.7/alphapulldown/ColabFold/colabfold/plot.py
+-rw-r--r--   0    24600      721     9954 2023-05-16 11:20:08.000000 alphapulldown-0.30.7/alphapulldown/ColabFold/colabfold/utils.py
+-rw-r--r--   0    24600      721       81 2023-06-21 12:08:49.000000 alphapulldown-0.30.7/alphapulldown/__init__.py
+drwxr-xr-x   0    24600      721        0 2023-06-21 12:14:27.000000 alphapulldown-0.30.7/alphapulldown/analysis_pipeline/
+-rw-r--r--   0    24600      721     7268 2023-03-14 10:54:09.000000 alphapulldown-0.30.7/alphapulldown/analysis_pipeline/af2_3dmol.py
+drwxr-xr-x   0    24600      721        0 2023-06-21 12:14:27.000000 alphapulldown-0.30.7/alphapulldown/analysis_pipeline/af2_plots/
+drwxr-xr-x   0    24600      721        0 2023-06-21 12:14:29.000000 alphapulldown-0.30.7/alphapulldown/analysis_pipeline/af2_plots/af2plots/
+-rw-r--r--   0    24600      721        0 2023-05-16 12:08:43.000000 alphapulldown-0.30.7/alphapulldown/analysis_pipeline/af2_plots/af2plots/__init__.py
+-rw-r--r--   0    24600      721     3745 2023-05-16 11:50:17.000000 alphapulldown-0.30.7/alphapulldown/analysis_pipeline/af2_plots/af2plots/__main__.py
+-rw-r--r--   0    24600      721    15555 2023-05-16 11:50:17.000000 alphapulldown-0.30.7/alphapulldown/analysis_pipeline/af2_plots/af2plots/plotter.py
+-rw-r--r--   0    24600      721       21 2023-05-16 11:50:18.000000 alphapulldown-0.30.7/alphapulldown/analysis_pipeline/af2_plots/af2plots/version.py
+-rw-r--r--   0    24600      721      851 2023-05-16 11:51:00.000000 alphapulldown-0.30.7/alphapulldown/analysis_pipeline/af2_plots/setup.py
+-rw-rw-r--   0    24600      721     6028 2023-01-27 13:24:19.000000 alphapulldown-0.30.7/alphapulldown/analysis_pipeline/calculate_mpdockq.py
+-rw-r--r--   0    24600      721     5510 2023-01-27 13:03:03.000000 alphapulldown-0.30.7/alphapulldown/analysis_pipeline/create_notebook.py
+-rw-r--r--   0    24600      721     6520 2023-01-27 13:24:19.000000 alphapulldown-0.30.7/alphapulldown/analysis_pipeline/get_good_inter_pae.py
+-rw-r--r--   0    24600      721      962 2023-01-27 13:03:03.000000 alphapulldown-0.30.7/alphapulldown/analysis_pipeline/utils.py
+-rwxr-xr-x   0    24600      721    10571 2023-04-19 11:33:53.000000 alphapulldown-0.30.7/alphapulldown/create_individual_features.py
+-rw-r--r--   0    24600      721    22205 2023-06-21 11:51:34.000000 alphapulldown-0.30.7/alphapulldown/objects.py
+-rw-r--r--   0    24600      721     1822 2023-03-14 16:09:43.000000 alphapulldown-0.30.7/alphapulldown/plot_pae.py
+-rw-r--r--   0    24600      721     8913 2023-06-21 11:51:34.000000 alphapulldown-0.30.7/alphapulldown/predict_structure.py
+-rwxr-xr-x   0    24600      721     1166 2023-03-14 16:09:44.000000 alphapulldown-0.30.7/alphapulldown/prepare_seq_names.py
+-rwxr-xr-x   0    24600      721     1261 2023-03-14 16:09:44.000000 alphapulldown-0.30.7/alphapulldown/rename_colab_search_a3m.py
+-rw-r--r--   0    24600      721    11611 2023-06-06 10:29:09.000000 alphapulldown-0.30.7/alphapulldown/run_multimer_jobs.py
+-rw-r--r--   0    24600      721    11546 2023-05-24 14:31:29.000000 alphapulldown-0.30.7/alphapulldown/utils.py
+drwxr-xr-x   0    24600      721        0 2023-06-21 12:14:40.000000 alphapulldown-0.30.7/alphapulldown.egg-info/
+-rw-r--r--   0    24600      721     4096 2023-05-19 09:47:48.000000 alphapulldown-0.30.7/alphapulldown.egg-info/._PKG-INFO
+-rw-r--r--   0    24600      721     4096 2023-05-19 09:47:58.000000 alphapulldown-0.30.7/alphapulldown.egg-info/._SOURCES.txt
+-rw-r--r--   0    24600      721     4096 2023-05-19 09:47:49.000000 alphapulldown-0.30.7/alphapulldown.egg-info/._dependency_links.txt
+-rw-r--r--   0    24600      721     4096 2023-05-19 09:47:50.000000 alphapulldown-0.30.7/alphapulldown.egg-info/._requires.txt
+-rw-r--r--   0    24600      721     4096 2023-05-19 09:47:50.000000 alphapulldown-0.30.7/alphapulldown.egg-info/._top_level.txt
+-rw-r--r--   0    24600      721      428 2023-06-21 12:13:38.000000 alphapulldown-0.30.7/alphapulldown.egg-info/PKG-INFO
+-rw-r--r--   0    24600      721     6224 2023-06-21 12:13:39.000000 alphapulldown-0.30.7/alphapulldown.egg-info/SOURCES.txt
+-rw-r--r--   0    24600      721        1 2023-06-21 12:13:38.000000 alphapulldown-0.30.7/alphapulldown.egg-info/dependency_links.txt
+-rw-r--r--   0    24600      721      262 2023-06-21 12:13:38.000000 alphapulldown-0.30.7/alphapulldown.egg-info/requires.txt
+-rw-r--r--   0    24600      721       61 2023-06-21 12:13:38.000000 alphapulldown-0.30.7/alphapulldown.egg-info/top_level.txt
+drwxr-xr-x   0    24600      721        0 2023-06-21 12:14:32.000000 alphapulldown-0.30.7/colabfold/
+-rw-r--r--   0    24600      721        0 2023-04-06 09:21:34.000000 alphapulldown-0.30.7/colabfold/__init__.py
+drwxr-xr-x   0    24600      721        0 2023-06-21 12:14:33.000000 alphapulldown-0.30.7/colabfold/alphafold/
+-rw-r--r--   0    24600      721        0 2023-04-06 09:21:34.000000 alphapulldown-0.30.7/colabfold/alphafold/__init__.py
+-rw-r--r--   0    24600      721     5923 2023-04-06 09:21:34.000000 alphapulldown-0.30.7/colabfold/alphafold/models.py
+-rw-r--r--   0    24600      721     1565 2023-04-06 09:21:34.000000 alphapulldown-0.30.7/colabfold/alphafold/msa.py
+-rw-r--r--   0    24600      721    65347 2023-04-06 09:21:34.000000 alphapulldown-0.30.7/colabfold/batch.py
+-rw-r--r--   0    24600      721     5988 2023-04-06 09:21:34.000000 alphapulldown-0.30.7/colabfold/citations.py
+-rw-r--r--   0    24600      721    24980 2023-04-06 09:21:34.000000 alphapulldown-0.30.7/colabfold/colabfold.py
+-rw-r--r--   0    24600      721    32656 2023-04-06 09:21:34.000000 alphapulldown-0.30.7/colabfold/colabfold_alphafold.py
+-rw-r--r--   0    24600      721     1982 2023-04-06 09:21:34.000000 alphapulldown-0.30.7/colabfold/download.py
+drwxr-xr-x   0    24600      721        0 2023-06-21 12:14:35.000000 alphapulldown-0.30.7/colabfold/mmseqs/
+-rw-r--r--   0    24600      721        0 2023-04-06 09:21:34.000000 alphapulldown-0.30.7/colabfold/mmseqs/__init__.py
+-rw-r--r--   0    24600      721     1933 2023-04-06 09:21:34.000000 alphapulldown-0.30.7/colabfold/mmseqs/merge_and_split_msas.py
+-rw-r--r--   0    24600      721    18799 2023-04-06 09:21:34.000000 alphapulldown-0.30.7/colabfold/mmseqs/search.py
+-rw-r--r--   0    24600      721     1429 2023-04-06 09:21:34.000000 alphapulldown-0.30.7/colabfold/mmseqs/split_msas.py
+-rw-r--r--   0    24600      721     2120 2023-04-06 09:21:34.000000 alphapulldown-0.30.7/colabfold/pdb.py
+-rw-r--r--   0    24600      721     3419 2023-04-06 09:21:35.000000 alphapulldown-0.30.7/colabfold/plot.py
+-rw-r--r--   0    24600      721     9954 2023-04-06 09:21:35.000000 alphapulldown-0.30.7/colabfold/utils.py
+-rw-r--r--   0    24600      721      140 2023-04-05 11:02:03.000000 alphapulldown-0.30.7/pyproject.toml
+-rw-r--r--   0    24600      721     1470 2023-06-21 12:14:42.000000 alphapulldown-0.30.7/setup.cfg
+-rwxr-xr-x   0    24600      721       67 2023-04-18 11:12:27.000000 alphapulldown-0.30.7/setup.py
+-rw-r--r--   0    24600      721     9119 2023-04-18 11:12:28.000000 alphapulldown-0.30.7/stereo_chemical_props.txt
+drwxr-xr-x   0    24600      721        0 2023-06-21 12:14:41.000000 alphapulldown-0.30.7/test/
+-rw-r--r--   0    24600      721     4546 2023-04-19 11:33:54.000000 alphapulldown-0.30.7/test/test_create_objects.py
+-rwxr-xr-x   0    24600      721    12809 2023-05-19 10:38:44.000000 alphapulldown-0.30.7/test/test_predict_structure.py
+drwxr-xr-x   0    24600      721        0 2023-06-21 12:13:42.000000 alphapulldown-0.30.7/unifold/
+drwxr-xr-x   0    24600      721        0 2023-06-21 12:14:38.000000 alphapulldown-0.30.7/unifold/unifold/
+-rw-r--r--   0    24600      721       72 2023-05-19 11:17:04.000000 alphapulldown-0.30.7/unifold/unifold/__init__.py
+-rw-r--r--   0    24600      721    25459 2023-05-24 12:02:28.000000 alphapulldown-0.30.7/unifold/unifold/config.py
+-rw-r--r--   0    24600      721    21165 2023-05-24 12:02:54.000000 alphapulldown-0.30.7/unifold/unifold/dataset.py
+-rw-r--r--   0    24600      721    10412 2023-05-19 11:17:20.000000 alphapulldown-0.30.7/unifold/unifold/homo_search.py
+-rw-r--r--   0    24600      721    16351 2023-05-24 12:02:55.000000 alphapulldown-0.30.7/unifold/unifold/inference.py
+-rw-r--r--   0    24600      721     7587 2023-05-19 11:17:22.000000 alphapulldown-0.30.7/unifold/unifold/inference_symmetry.py
+-rw-r--r--   0    24600      721     9457 2023-05-19 11:17:23.000000 alphapulldown-0.30.7/unifold/unifold/loss.py
+-rw-r--r--   0    24600      721     1453 2023-05-19 11:17:30.000000 alphapulldown-0.30.7/unifold/unifold/model.py
+-rw-r--r--   0    24600      721     2445 2023-05-19 11:18:12.000000 alphapulldown-0.30.7/unifold/unifold/task.py
```

### Comparing `alphapulldown-0.30.6/LICENSE` & `alphapulldown-0.30.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/README.md` & `alphapulldown-0.30.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # AlphaPulldown
+[![Downloads](https://static.pepy.tech/badge/alphapulldown)](https://pepy.tech/project/alphapulldown)  [![python3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-360/) ![GPL3 license](https://img.shields.io/badge/license-GPLv3-green)
 
 AlphaPulldown is a Python package that streamlines protein-protein interaction screens and high-throughput modelling of higher-order oligomers using AlphaFold-Multimer:
 * provides a convenient command line interface to screen a bait protein against many candidates, calculate all-versus-all pairwise comparisons, test alternative homo-oligomeric states, and model various parts of a larger complex
 * separates the CPU stages (MSA and template feature generation) from GPU stages (the actual modeling)
 * allows modeling fragments of proteins without recalculation of MSAs and keeping the original full-length residue numbering in the models
 * summarizes the results in a CSV table with AlphaFold scores, pDockQ and mpDockQ, PI-score, and various physical parameters of the interface
 * provides a Jupyter notebook for an interactive analysis of PAE plots and models
@@ -54,15 +55,15 @@
 ```bash
 conda create -n AlphaPulldown -c omnia -c bioconda -c conda-forge python==3.8 openmm=7.5.1 pdbfixer=1.6 kalign2=2.04 cctbx-base
 ```
 
 **Secondly**, activate the AlphaPulldown environment and install AlphaPulldown
 ```bash
 source activate AlphaPulldown
-python3 -m pip install alphapulldown==0.30.5
+python3 -m pip install alphapulldown==0.30.6
 pip install -q "jax[cuda]==0.3.25" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
 ```
 
 **Optionally**, if you do not have these software yet on your system, install [HMMER](http://hmmer.org/documentation.html), [HH-suite](https://github.com/soedinglab/hh-suite) from Anaconda
 ```bash
 source activate AlphaPulldown
 conda install -c bioconda hmmer hhsuite
```

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/__init__.py` & `alphapulldown-0.30.7/alphafold/alphafold/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/common/__init__.py` & `alphapulldown-0.30.7/alphafold/alphafold/common/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/common/confidence.py` & `alphapulldown-0.30.7/alphafold/alphafold/common/confidence.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/common/protein.py` & `alphapulldown-0.30.7/alphafold/alphafold/common/protein.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/common/protein_test.py` & `alphapulldown-0.30.7/alphafold/alphafold/common/protein_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/common/residue_constants.py` & `alphapulldown-0.30.7/alphafold/alphafold/common/residue_constants.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/common/residue_constants_test.py` & `alphapulldown-0.30.7/alphafold/alphafold/common/residue_constants_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/data/__init__.py` & `alphapulldown-0.30.7/alphafold/alphafold/data/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/data/feature_processing.py` & `alphapulldown-0.30.7/alphafold/alphafold/data/feature_processing.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/data/mmcif_parsing.py` & `alphapulldown-0.30.7/alphafold/alphafold/data/mmcif_parsing.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/data/msa_identifiers.py` & `alphapulldown-0.30.7/alphafold/alphafold/data/msa_identifiers.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/data/msa_pairing.py` & `alphapulldown-0.30.7/alphafold/alphafold/data/msa_pairing.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/data/parsers.py` & `alphapulldown-0.30.7/alphafold/alphafold/data/parsers.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/data/pipeline.py` & `alphapulldown-0.30.7/alphafold/alphafold/data/pipeline.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/data/pipeline_multimer.py` & `alphapulldown-0.30.7/alphafold/alphafold/data/pipeline_multimer.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/data/templates.py` & `alphapulldown-0.30.7/alphafold/alphafold/data/templates.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/data/tools/__init__.py` & `alphapulldown-0.30.7/alphafold/alphafold/data/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/data/tools/hhblits.py` & `alphapulldown-0.30.7/alphafold/alphafold/data/tools/hhblits.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/data/tools/hhsearch.py` & `alphapulldown-0.30.7/alphafold/alphafold/data/tools/hhsearch.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/data/tools/hmmbuild.py` & `alphapulldown-0.30.7/alphafold/alphafold/data/tools/hmmbuild.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/data/tools/hmmsearch.py` & `alphapulldown-0.30.7/alphafold/alphafold/data/tools/hmmsearch.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/data/tools/jackhmmer.py` & `alphapulldown-0.30.7/alphafold/alphafold/data/tools/jackhmmer.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/data/tools/kalign.py` & `alphapulldown-0.30.7/alphafold/alphafold/data/tools/kalign.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/data/tools/utils.py` & `alphapulldown-0.30.7/alphafold/alphafold/data/tools/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/__init__.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/all_atom.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/all_atom.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/all_atom_multimer.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/all_atom_multimer.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/all_atom_test.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/all_atom_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/common_modules.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/common_modules.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/config.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/config.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/data.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/data.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/features.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/features.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/folding.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/folding.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/folding_multimer.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/folding_multimer.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/geometry/__init__.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/geometry/rigid_matrix_vector.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/geometry/rigid_matrix_vector.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/geometry/rotation_matrix.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/geometry/rotation_matrix.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/geometry/struct_of_array.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/geometry/struct_of_array.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/geometry/test_utils.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/geometry/test_utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/geometry/utils.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/geometry/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/geometry/vector.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/geometry/vector.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/layer_stack.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/layer_stack.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/layer_stack_test.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/layer_stack_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/lddt.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/lddt.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/lddt_test.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/lddt_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/mapping.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/mapping.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/model.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/model.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/modules.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/modules.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/modules_multimer.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/modules_multimer.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/prng.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/prng.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/prng_test.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/prng_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/quat_affine.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/quat_affine.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/quat_affine_test.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/quat_affine_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/r3.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/r3.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/tf/__init__.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/tf/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/tf/data_transforms.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/tf/data_transforms.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/tf/input_pipeline.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/tf/input_pipeline.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/tf/protein_features.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/tf/protein_features.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/tf/protein_features_test.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/tf/protein_features_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/tf/proteins_dataset.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/tf/proteins_dataset.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/tf/shape_helpers.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/tf/shape_helpers.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/tf/shape_helpers_test.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/tf/shape_helpers_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/tf/shape_placeholders.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/tf/shape_placeholders.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/tf/utils.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/tf/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/model/utils.py` & `alphapulldown-0.30.7/alphafold/alphafold/model/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/notebooks/__init__.py` & `alphapulldown-0.30.7/alphafold/alphafold/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/notebooks/notebook_utils.py` & `alphapulldown-0.30.7/alphafold/alphafold/notebooks/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/notebooks/notebook_utils_test.py` & `alphapulldown-0.30.7/alphafold/alphafold/notebooks/notebook_utils_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/relax/__init__.py` & `alphapulldown-0.30.7/alphafold/alphafold/relax/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/relax/amber_minimize.py` & `alphapulldown-0.30.7/alphafold/alphafold/relax/amber_minimize.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/relax/amber_minimize_test.py` & `alphapulldown-0.30.7/alphafold/alphafold/relax/amber_minimize_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/relax/cleanup.py` & `alphapulldown-0.30.7/alphafold/alphafold/relax/cleanup.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/relax/cleanup_test.py` & `alphapulldown-0.30.7/alphafold/alphafold/relax/cleanup_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/relax/relax.py` & `alphapulldown-0.30.7/alphafold/alphafold/relax/relax.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/relax/relax_test.py` & `alphapulldown-0.30.7/alphafold/alphafold/relax/relax_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/relax/utils.py` & `alphapulldown-0.30.7/alphafold/alphafold/relax/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/alphafold/relax/utils_test.py` & `alphapulldown-0.30.7/alphafold/alphafold/relax/utils_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/run_alphafold.py` & `alphapulldown-0.30.7/alphafold/alphafold/run_alphafold.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphafold/setup.py` & `alphapulldown-0.30.7/alphafold/setup.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/batch.py` & `alphapulldown-0.30.7/alphapulldown/ColabFold/colabfold/batch.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/citations.py` & `alphapulldown-0.30.7/alphapulldown/ColabFold/colabfold/citations.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/colabfold.py` & `alphapulldown-0.30.7/alphapulldown/ColabFold/colabfold/colabfold.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/colabfold_alphafold.py` & `alphapulldown-0.30.7/alphapulldown/ColabFold/colabfold/colabfold_alphafold.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/download.py` & `alphapulldown-0.30.7/alphapulldown/ColabFold/colabfold/download.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/pdb.py` & `alphapulldown-0.30.7/alphapulldown/ColabFold/colabfold/pdb.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/plot.py` & `alphapulldown-0.30.7/alphapulldown/ColabFold/colabfold/plot.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphapulldown/ColabFold/colabfold/utils.py` & `alphapulldown-0.30.7/alphapulldown/ColabFold/colabfold/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphapulldown/analysis_pipeline/af2_3dmol.py` & `alphapulldown-0.30.7/alphapulldown/analysis_pipeline/af2_3dmol.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphapulldown/analysis_pipeline/af2_plots/af2plots/__main__.py` & `alphapulldown-0.30.7/alphapulldown/analysis_pipeline/af2_plots/af2plots/__main__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphapulldown/analysis_pipeline/af2_plots/af2plots/plotter.py` & `alphapulldown-0.30.7/alphapulldown/analysis_pipeline/af2_plots/af2plots/plotter.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphapulldown/analysis_pipeline/af2_plots/setup.py` & `alphapulldown-0.30.7/alphapulldown/analysis_pipeline/af2_plots/setup.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphapulldown/analysis_pipeline/calculate_mpdockq.py` & `alphapulldown-0.30.7/alphapulldown/analysis_pipeline/calculate_mpdockq.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphapulldown/analysis_pipeline/create_notebook.py` & `alphapulldown-0.30.7/alphapulldown/analysis_pipeline/create_notebook.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphapulldown/analysis_pipeline/get_good_inter_pae.py` & `alphapulldown-0.30.7/alphapulldown/analysis_pipeline/get_good_inter_pae.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphapulldown/analysis_pipeline/utils.py` & `alphapulldown-0.30.7/alphapulldown/analysis_pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphapulldown/create_individual_features.py` & `alphapulldown-0.30.7/alphapulldown/create_individual_features.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphapulldown/objects.py` & `alphapulldown-0.30.7/alphapulldown/objects.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphapulldown/plot_pae.py` & `alphapulldown-0.30.7/alphapulldown/plot_pae.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphapulldown/predict_structure.py` & `alphapulldown-0.30.7/alphapulldown/predict_structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     with open(pkl_path, "rb") as f:
         result = pickle.load(f)
     if "iptm" in result:
         score_type = "iptm+ptm"
         score = 0.8 * result["iptm"] + 0.2 * result["ptm"]
     else:
         score_type = "plddt"
-        score = result["plddt"]
+        score = np.mean(result["plddt"])
 
     return score_type, score
 
 def get_existing_model_info(output_dir, model_runners):
     ranking_confidences = {}
     unrelaxed_proteins = {}
     unrelaxed_pdbs = {}
@@ -83,14 +83,15 @@
 ):
     timings = {}
     unrelaxed_pdbs = {}
     relaxed_pdbs = {}
     relax_metrics = {}
     ranking_confidences = {}
     unrelaxed_proteins = {}
+    prediction_result = {}
     START = 0
     ranking_output_path = os.path.join(output_dir, "ranking_debug.json")
     temp_timings_output_path = os.path.join(output_dir, "timings_temp.json") #To keep track of timings in case of crash and resume
 
     if allow_resume:
         logging.info("Checking for existing results")
         ranking_confidences, unrelaxed_proteins, unrelaxed_pdbs, START = get_existing_model_info(output_dir, model_runners)
@@ -168,15 +169,14 @@
         unrelaxed_pdb_path = os.path.join(output_dir, f"unrelaxed_{model_name}.pdb")
         with open(unrelaxed_pdb_path, "w") as f:
             f.write(unrelaxed_pdbs[model_name])
 
         with open(temp_timings_output_path, "w") as f:
             f.write(json.dumps(timings, indent=4))
 
-
     # Rank by model confidence.
     ranked_order = [
         model_name for model_name, confidence in
         sorted(ranking_confidences.items(), key=lambda x: x[1], reverse=True)]
 
     # Relax predictions.
     amber_relaxer = relax.AmberRelaxation(
```

### Comparing `alphapulldown-0.30.6/alphapulldown/prepare_seq_names.py` & `alphapulldown-0.30.7/alphapulldown/prepare_seq_names.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphapulldown/rename_colab_search_a3m.py` & `alphapulldown-0.30.7/alphapulldown/rename_colab_search_a3m.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphapulldown/run_multimer_jobs.py` & `alphapulldown-0.30.7/alphapulldown/run_multimer_jobs.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphapulldown/utils.py` & `alphapulldown-0.30.7/alphapulldown/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphapulldown.egg-info/._PKG-INFO` & `alphapulldown-0.30.7/alphapulldown.egg-info/._PKG-INFO`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphapulldown.egg-info/._SOURCES.txt` & `alphapulldown-0.30.7/alphapulldown.egg-info/._SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphapulldown.egg-info/._dependency_links.txt` & `alphapulldown-0.30.7/alphapulldown.egg-info/._dependency_links.txt`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphapulldown.egg-info/._requires.txt` & `alphapulldown-0.30.7/alphapulldown.egg-info/._requires.txt`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphapulldown.egg-info/._top_level.txt` & `alphapulldown-0.30.7/alphapulldown.egg-info/._top_level.txt`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/alphapulldown.egg-info/SOURCES.txt` & `alphapulldown-0.30.7/alphapulldown.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 stereo_chemical_props.txt
-./alphafold/run_alphafold.py
-./alphafold/run_alphafold_test.py
 ./alphafold/setup.py
 ./alphafold/alphafold/__init__.py
+./alphafold/alphafold/run_alphafold.py
 ./alphafold/alphafold/common/__init__.py
 ./alphafold/alphafold/common/confidence.py
 ./alphafold/alphafold/common/protein.py
 ./alphafold/alphafold/common/protein_test.py
 ./alphafold/alphafold/common/residue_constants.py
 ./alphafold/alphafold/common/residue_constants_test.py
 ./alphafold/alphafold/data/__init__.py
```

### Comparing `alphapulldown-0.30.6/colabfold/alphafold/models.py` & `alphapulldown-0.30.7/colabfold/alphafold/models.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/colabfold/alphafold/msa.py` & `alphapulldown-0.30.7/colabfold/alphafold/msa.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/colabfold/batch.py` & `alphapulldown-0.30.7/colabfold/batch.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/colabfold/citations.py` & `alphapulldown-0.30.7/colabfold/citations.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/colabfold/colabfold.py` & `alphapulldown-0.30.7/colabfold/colabfold.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/colabfold/colabfold_alphafold.py` & `alphapulldown-0.30.7/colabfold/colabfold_alphafold.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/colabfold/download.py` & `alphapulldown-0.30.7/colabfold/download.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/colabfold/mmseqs/merge_and_split_msas.py` & `alphapulldown-0.30.7/colabfold/mmseqs/merge_and_split_msas.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/colabfold/mmseqs/search.py` & `alphapulldown-0.30.7/colabfold/mmseqs/search.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/colabfold/mmseqs/split_msas.py` & `alphapulldown-0.30.7/colabfold/mmseqs/split_msas.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/colabfold/pdb.py` & `alphapulldown-0.30.7/colabfold/pdb.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/colabfold/plot.py` & `alphapulldown-0.30.7/colabfold/plot.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/colabfold/utils.py` & `alphapulldown-0.30.7/colabfold/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/setup.cfg` & `alphapulldown-0.30.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = alphapulldown
-version = 0.30.6
+version = 0.30.7
 author = Dingquan Yu
 author_email = dingquan.yu@embl-hamburg.de
 description = Pipeline allows massive screening using alphafold
 url = https://github.com/KosinskiLab/AlphaPulldown
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
```

### Comparing `alphapulldown-0.30.6/stereo_chemical_props.txt` & `alphapulldown-0.30.7/stereo_chemical_props.txt`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/test/test_create_objects.py` & `alphapulldown-0.30.7/test/test_create_objects.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/test/test_predict_structure.py` & `alphapulldown-0.30.7/test/test_predict_structure.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/unifold/unifold/config.py` & `alphapulldown-0.30.7/unifold/unifold/config.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/unifold/unifold/dataset.py` & `alphapulldown-0.30.7/unifold/unifold/dataset.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/unifold/unifold/homo_search.py` & `alphapulldown-0.30.7/unifold/unifold/homo_search.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/unifold/unifold/inference.py` & `alphapulldown-0.30.7/unifold/unifold/inference.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/unifold/unifold/inference_symmetry.py` & `alphapulldown-0.30.7/unifold/unifold/inference_symmetry.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/unifold/unifold/loss.py` & `alphapulldown-0.30.7/unifold/unifold/loss.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/unifold/unifold/model.py` & `alphapulldown-0.30.7/unifold/unifold/model.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.6/unifold/unifold/task.py` & `alphapulldown-0.30.7/unifold/unifold/task.py`

 * *Files identical despite different names*

