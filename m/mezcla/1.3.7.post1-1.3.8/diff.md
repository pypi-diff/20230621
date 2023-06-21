# Comparing `tmp/mezcla-1.3.7.post1.tar.gz` & `tmp/mezcla-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mezcla-1.3.7.post1.tar", last modified: Thu Jun  1 23:52:41 2023, max compression
+gzip compressed data, was "mezcla-1.3.8.tar", last modified: Wed Jun 21 08:36:51 2023, max compression
```

## Comparing `mezcla-1.3.7.post1.tar` & `mezcla-1.3.8.tar`

### file list

```diff
@@ -1,159 +1,161 @@
--rw-r--r--   0        0        0      542 2023-04-30 22:44:00.934589 mezcla-1.3.7.post1/.coveragerc
--rw-r--r--   0        0        0     1042 2023-06-01 22:36:35.337702 mezcla-1.3.7.post1/.github/workflows/tests.yml
--rw-r--r--   0        0        0     1870 2023-06-01 22:36:35.337702 mezcla-1.3.7.post1/.gitignore
--rw-r--r--   0        0        0     2621 2023-06-01 22:36:35.341703 mezcla-1.3.7.post1/Dockerfile
--rw-r--r--   0        0        0     7370 2022-06-03 04:33:57.175684 mezcla-1.3.7.post1/LICENSE.txt
--rw-r--r--   0        0        0      777 2022-06-03 04:33:57.175684 mezcla-1.3.7.post1/README.txt
--rw-r--r--   0        0        0      380 2023-06-01 22:36:35.341703 mezcla-1.3.7.post1/TODO.txt
--rw-r--r--   0        0        0      130 2023-06-01 22:36:35.341703 mezcla-1.3.7.post1/mezcla/TODO.md
--rwxr-xr-x   0        0        0     1933 2023-06-01 23:42:22.938105 mezcla-1.3.7.post1/mezcla/__init__.py
--rwxr-xr-x   0        0        0    10860 2022-06-02 23:46:45.000000 mezcla-1.3.7.post1/mezcla/analyze_tfidf.py
--rwxr-xr-x   0        0        0    13029 2023-04-30 22:44:00.938590 mezcla-1.3.7.post1/mezcla/audio.py
--rwxr-xr-x   0        0        0     4707 2023-06-01 22:36:35.341703 mezcla-1.3.7.post1/mezcla/bash_ast.py
--rwxr-xr-x   0        0        0    16055 2022-06-16 07:59:25.588655 mezcla-1.3.7.post1/mezcla/bert_multi_classification.py
--rwxr-xr-x   0        0        0    25702 2022-06-03 05:22:44.104859 mezcla-1.3.7.post1/mezcla/bert_text_classification.py
--rwxr-xr-x   0        0        0     7625 2023-04-30 22:44:00.938590 mezcla-1.3.7.post1/mezcla/bing_search.py
--rwxr-xr-x   0        0        0     8925 2022-02-01 06:41:33.000000 mezcla-1.3.7.post1/mezcla/check_html_javascript.py
--rwxr-xr-x   0        0        0    14338 2023-04-30 22:44:00.938590 mezcla-1.3.7.post1/mezcla/compute_tfidf.py
--rwxr-xr-x   0        0        0    22279 2023-04-30 22:44:00.938590 mezcla-1.3.7.post1/mezcla/cut.py
--rwxr-xr-x   0        0        0     4307 2023-04-30 22:47:21.042725 mezcla-1.3.7.post1/mezcla/data_utils.py
--rwxr-xr-x   0        0        0    47548 2023-06-01 22:36:35.341703 mezcla-1.3.7.post1/mezcla/debug.py
--rw-r--r--   0        0        0    25047 2023-04-30 22:44:00.942590 mezcla-1.3.7.post1/mezcla/docs/audio_uml.svg
--rwxr-xr-x   0        0        0        0 2023-04-30 22:44:00.942590 mezcla-1.3.7.post1/mezcla/examples/__init__.py
--rwxr-xr-x   0        0        0    12834 2021-10-26 07:06:23.000000 mezcla-1.3.7.post1/mezcla/examples/alt_sklearn_plot_precision_recall.py
--rwxr-xr-x   0        0        0     3608 2022-06-16 07:59:25.588655 mezcla-1.3.7.post1/mezcla/examples/brownlee_ml_metrics.py
--rwxr-xr-x   0        0        0     2419 2023-04-30 22:44:00.942590 mezcla-1.3.7.post1/mezcla/examples/consume_all_memory.py
--rwxr-xr-x   0        0        0     5008 2023-04-30 22:44:00.942590 mezcla-1.3.7.post1/mezcla/examples/download_user_gist.py
--rwxr-xr-x   0        0        0     6477 2022-06-09 02:23:07.119975 mezcla-1.3.7.post1/mezcla/examples/dump_checkpoints.py
--rw-r--r--   0        0        0     2738 2022-02-20 02:05:16.229030 mezcla-1.3.7.post1/mezcla/examples/encoded-iris.csv
--rwxr-xr-x   0        0        0     8779 2022-02-21 09:16:29.886156 mezcla-1.3.7.post1/mezcla/examples/feature_importance.py
--rw-r--r--   0        0        0    40044 2023-04-30 22:44:00.946590 mezcla-1.3.7.post1/mezcla/examples/fuzzy-testing-1-2-3.wav
--rwxr-xr-x   0        0        0     3338 2023-04-30 22:44:00.946590 mezcla-1.3.7.post1/mezcla/examples/hugging_face_speechrec.py
--rwxr-xr-x   0        0        0     3922 2023-04-30 22:44:00.946590 mezcla-1.3.7.post1/mezcla/examples/hugging_face_translation.py
--rwxr-xr-x   0        0        0    10347 2023-04-30 22:44:00.946590 mezcla-1.3.7.post1/mezcla/examples/inspect_checkpoint.py
--rw-r--r--   0        0        0     4607 2020-04-12 09:44:23.000000 mezcla-1.3.7.post1/mezcla/examples/iris.csv
--rw-r--r--   0        0        0    23345 2020-05-01 07:18:00.000000 mezcla-1.3.7.post1/mezcla/examples/pima-indians-diabetes.csv
--rwxr-xr-x   0        0        0     8279 2022-06-09 02:26:58.076477 mezcla-1.3.7.post1/mezcla/examples/plot_forest_importances.py
--rwxr-xr-x   0        0        0    12989 2021-10-16 04:41:00.000000 mezcla-1.3.7.post1/mezcla/examples/sklearn_plot_precision_recall.py
--rwxr-xr-x   0        0        0     1685 2023-06-01 22:36:35.341703 mezcla-1.3.7.post1/mezcla/examples/template.py
--rwxr-xr-x   0        0        0     3155 2023-04-30 22:44:00.946590 mezcla-1.3.7.post1/mezcla/examples/tensorflow_matrix_multiply.py
--rwxr-xr-x   0        0        0     3607 2023-04-30 22:44:00.946590 mezcla-1.3.7.post1/mezcla/examples/tracemalloc_display.py
--rwxr-xr-x   0        0        0     4031 2023-04-30 22:44:00.946590 mezcla-1.3.7.post1/mezcla/extract_document_text.py
--rwxr-xr-x   0        0        0     7708 2023-06-01 22:36:35.341703 mezcla-1.3.7.post1/mezcla/file_utils.py
--rwxr-xr-x   0        0        0     3071 2022-03-01 08:46:55.000000 mezcla-1.3.7.post1/mezcla/filter_random.py
--rwxr-xr-x   0        0        0     2998 2021-09-30 12:02:57.000000 mezcla-1.3.7.post1/mezcla/format_profile.py
--rwxr-xr-x   0        0        0    32894 2022-06-02 07:16:58.000000 mezcla-1.3.7.post1/mezcla/gensim_test.py
--rwxr-xr-x   0        0        0    32727 2023-06-01 22:36:35.345703 mezcla-1.3.7.post1/mezcla/glue_helpers.py
--rwxr-xr-x   0        0        0    32492 2023-04-30 22:44:00.950590 mezcla-1.3.7.post1/mezcla/html_utils.py
--rwxr-xr-x   0        0        0     4708 2021-09-30 12:02:57.000000 mezcla-1.3.7.post1/mezcla/kenlm_example.py
--rwxr-xr-x   0        0        0    17916 2023-04-30 22:44:00.950590 mezcla-1.3.7.post1/mezcla/keras_param_search.py
--rwxr-xr-x   0        0        0    42934 2023-06-01 22:36:35.345703 mezcla-1.3.7.post1/mezcla/main.py
--rwxr-xr-x   0        0        0     9307 2023-06-01 22:36:35.345703 mezcla-1.3.7.post1/mezcla/merge_files.py
--rwxr-xr-x   0        0        0    11717 2023-04-30 22:44:00.954590 mezcla-1.3.7.post1/mezcla/merge_notes.py
--rwxr-xr-x   0        0        0    11641 2023-04-30 22:47:21.046725 mezcla-1.3.7.post1/mezcla/misc_utils.py
--rwxr-xr-x   0        0        0     9779 2023-06-01 22:36:35.345703 mezcla-1.3.7.post1/mezcla/my_regex.py
--rwxr-xr-x   0        0        0    13776 2023-04-30 22:44:00.954590 mezcla-1.3.7.post1/mezcla/ngram_tfidf.py
--rwxr-xr-x   0        0        0      737 2023-06-01 22:36:35.345703 mezcla-1.3.7.post1/mezcla/os_utils.py
--rwxr-xr-x   0        0        0    31436 2023-04-30 22:44:00.958590 mezcla-1.3.7.post1/mezcla/pandas_sklearn.py
--rwxr-xr-x   0        0        0      828 2023-04-30 22:44:00.958590 mezcla-1.3.7.post1/mezcla/plot_utils.py
--rwxr-xr-x   0        0        0     7053 2023-04-30 22:44:00.958590 mezcla-1.3.7.post1/mezcla/randomize_lines.py
--rwxr-xr-x   0        0        0     7012 2023-04-30 22:44:00.958590 mezcla-1.3.7.post1/mezcla/rgb_color_name.py
--rwxr-xr-x   0        0        0    40529 2022-03-01 08:46:55.000000 mezcla-1.3.7.post1/mezcla/run_albert_classifier.py
--rwxr-xr-x   0        0        0    39613 2022-06-16 07:59:25.592656 mezcla-1.3.7.post1/mezcla/run_bert_classifier.py
--rwxr-xr-x   0        0        0    17400 2023-04-30 22:44:00.962590 mezcla-1.3.7.post1/mezcla/show_bert_representation.py
--rwxr-xr-x   0        0        0     1508 2021-09-30 12:02:57.000000 mezcla-1.3.7.post1/mezcla/simple_main_example.py
--rwxr-xr-x   0        0        0    19931 2023-04-30 22:44:00.962590 mezcla-1.3.7.post1/mezcla/spacy_nlp.py
--rwxr-xr-x   0        0        0     3011 2023-04-30 22:44:00.962590 mezcla-1.3.7.post1/mezcla/spell.py
--rwxr-xr-x   0        0        0     2416 2021-09-30 11:10:06.000000 mezcla-1.3.7.post1/mezcla/sys_version_info_hack.py
--rwxr-xr-x   0        0        0    50228 2023-06-01 22:36:35.345703 mezcla-1.3.7.post1/mezcla/system.py
--rwxr-xr-x   0        0        0    45776 2023-04-30 22:44:00.966590 mezcla-1.3.7.post1/mezcla/temp/simple_batspp.py
--rwxr-xr-x   0        0        0     5594 2023-06-01 22:36:35.345703 mezcla-1.3.7.post1/mezcla/template.py
--rw-r--r--   0        0        0     7370 2022-06-03 04:33:57.199684 mezcla-1.3.7.post1/mezcla/tests/LICENSE.txt
--rw-r--r--   0        0        0      462 2023-06-01 22:36:35.349704 mezcla-1.3.7.post1/mezcla/tests/TODO.md
--rw-r--r--   0        0        0     1082 2023-06-01 22:36:35.349704 mezcla-1.3.7.post1/mezcla/tests/adhoc-tests.batspp
--rw-r--r--   0        0        0      204 2023-06-01 22:36:35.349704 mezcla-1.3.7.post1/mezcla/tests/misc-tests.batspp
--rwxr-xr-x   0        0        0     3905 2022-06-03 04:33:57.199684 mezcla-1.3.7.post1/mezcla/tests/misc_doctests.py
--rw-r--r--   0        0        0      810 2023-04-30 22:47:21.046725 mezcla-1.3.7.post1/mezcla/tests/resources/cars-csv-len-3.txt
--rw-r--r--   0        0        0      113 2023-04-30 22:44:00.966590 mezcla-1.3.7.post1/mezcla/tests/resources/cars-fields-2-3-4.txt
--rw-r--r--   0        0        0      602 2023-04-30 22:47:21.046725 mezcla-1.3.7.post1/mezcla/tests/resources/cars-tsv-len-3.txt
--rw-r--r--   0        0        0      659 2023-04-30 22:44:00.966590 mezcla-1.3.7.post1/mezcla/tests/resources/cars.csv
--rw-r--r--   0        0        0      655 2023-04-30 22:47:21.046725 mezcla-1.3.7.post1/mezcla/tests/resources/cars.tsv
--rw-r--r--   0        0        0      603 2023-04-30 22:44:00.966590 mezcla-1.3.7.post1/mezcla/tests/resources/example_text.txt
--rw-r--r--   0        0        0     2573 2023-04-30 22:44:00.966590 mezcla-1.3.7.post1/mezcla/tests/resources/example_text_tags.txt
--rw-r--r--   0        0        0     2440 2023-04-30 22:44:00.966590 mezcla-1.3.7.post1/mezcla/tests/resources/iris_output.txt
--rw-r--r--   0        0        0     1152 2023-04-30 22:44:00.966590 mezcla-1.3.7.post1/mezcla/tests/resources/simple-window-dimensions.html
--rw-r--r--   0        0        0     5577 2023-04-30 22:44:00.966590 mezcla-1.3.7.post1/mezcla/tests/resources/spanish-accents.docx
--rw-r--r--   0        0        0    12530 2023-04-30 22:44:00.966590 mezcla-1.3.7.post1/mezcla/tests/resources/spanish-accents.pdf
--rw-r--r--   0        0        0      141 2023-04-30 22:44:00.966590 mezcla-1.3.7.post1/mezcla/tests/resources/spanish-accents.txt
--rw-r--r--   0        0        0       65 2023-04-30 22:44:00.966590 mezcla-1.3.7.post1/mezcla/tests/resources/word-POS.freq
--rw-r--r--   0        0        0      254 2023-04-30 22:44:00.966590 mezcla-1.3.7.post1/mezcla/tests/simple-script-tests.test
--rwxr-xr-x   0        0        0     4379 2023-06-01 22:36:35.349704 mezcla-1.3.7.post1/mezcla/tests/template.py
--rw-r--r--   0        0        0     2489 2023-06-01 22:36:35.349704 mezcla-1.3.7.post1/mezcla/tests/test___init__.py
--rwxr-xr-x   0        0        0     4736 2023-06-01 22:36:35.349704 mezcla-1.3.7.post1/mezcla/tests/test_audio.py
--rwxr-xr-x   0        0        0      969 2023-04-30 22:44:00.966590 mezcla-1.3.7.post1/mezcla/tests/test_bert_multi_classification.py
--rwxr-xr-x   0        0        0      834 2023-04-30 22:44:00.966590 mezcla-1.3.7.post1/mezcla/tests/test_bing_search.py
--rwxr-xr-x   0        0        0     1974 2023-04-30 22:44:00.966590 mezcla-1.3.7.post1/mezcla/tests/test_compute_tfidf.py
--rwxr-xr-x   0        0        0     2905 2023-04-30 22:47:21.046725 mezcla-1.3.7.post1/mezcla/tests/test_cut.py
--rwxr-xr-x   0        0        0     2464 2023-04-30 22:47:21.046725 mezcla-1.3.7.post1/mezcla/tests/test_data_utils.py
--rwxr-xr-x   0        0        0    15032 2023-06-01 22:36:35.349704 mezcla-1.3.7.post1/mezcla/tests/test_debug.py
--rwxr-xr-x   0        0        0     1030 2023-04-30 22:44:00.970590 mezcla-1.3.7.post1/mezcla/tests/test_extract_document_text.py
--rwxr-xr-x   0        0        0     4429 2023-06-01 22:36:35.349704 mezcla-1.3.7.post1/mezcla/tests/test_file_utils.py
--rwxr-xr-x   0        0        0     2939 2023-06-01 22:36:35.349704 mezcla-1.3.7.post1/mezcla/tests/test_filter_random.py
--rwxr-xr-x   0        0        0     2562 2023-04-30 22:44:00.970590 mezcla-1.3.7.post1/mezcla/tests/test_gensim_test.py
--rwxr-xr-x   0        0        0    15711 2023-06-01 22:36:35.349704 mezcla-1.3.7.post1/mezcla/tests/test_glue_helpers.py
--rwxr-xr-x   0        0        0    13008 2023-04-30 22:44:00.970590 mezcla-1.3.7.post1/mezcla/tests/test_html_utils.py
--rwxr-xr-x   0        0        0      892 2023-04-30 22:44:00.970590 mezcla-1.3.7.post1/mezcla/tests/test_kenlm_example.py
--rwxr-xr-x   0        0        0     2114 2023-06-01 22:36:35.349704 mezcla-1.3.7.post1/mezcla/tests/test_keras_param_search.py
--rwxr-xr-x   0        0        0     8972 2023-06-01 22:36:35.349704 mezcla-1.3.7.post1/mezcla/tests/test_main.py
--rwxr-xr-x   0        0        0     2725 2023-06-01 22:36:35.349704 mezcla-1.3.7.post1/mezcla/tests/test_merge_files.py
--rwxr-xr-x   0        0        0     1291 2023-04-30 22:44:00.970590 mezcla-1.3.7.post1/mezcla/tests/test_merge_notes.py
--rwxr-xr-x   0        0        0     6565 2023-04-30 22:44:00.970590 mezcla-1.3.7.post1/mezcla/tests/test_misc_utils.py
--rwxr-xr-x   0        0        0     2882 2023-04-30 22:44:00.970590 mezcla-1.3.7.post1/mezcla/tests/test_my_regex.py
--rwxr-xr-x   0        0        0      916 2023-04-30 22:44:00.970590 mezcla-1.3.7.post1/mezcla/tests/test_ngram_tfidf.py
--rwxr-xr-x   0        0        0      931 2023-06-01 22:36:35.349704 mezcla-1.3.7.post1/mezcla/tests/test_os_utils.py
--rwxr-xr-x   0        0        0     8323 2023-06-01 22:36:35.353705 mezcla-1.3.7.post1/mezcla/tests/test_pandas_sklearn.py
--rwxr-xr-x   0        0        0     1215 2023-06-01 22:36:35.353705 mezcla-1.3.7.post1/mezcla/tests/test_plot_utils.py
--rwxr-xr-x   0        0        0      854 2023-04-30 22:44:00.970590 mezcla-1.3.7.post1/mezcla/tests/test_randomize_lines.py
--rwxr-xr-x   0        0        0     2869 2023-04-30 22:47:21.050725 mezcla-1.3.7.post1/mezcla/tests/test_rgb_color_name.py
--rwxr-xr-x   0        0        0      895 2023-04-30 22:44:00.974590 mezcla-1.3.7.post1/mezcla/tests/test_run_albert_classifier.py
--rwxr-xr-x   0        0        0      930 2023-04-30 22:44:00.974590 mezcla-1.3.7.post1/mezcla/tests/test_run_bert_classifier.py
--rwxr-xr-x   0        0        0     1602 2023-04-30 22:44:00.974590 mezcla-1.3.7.post1/mezcla/tests/test_show_bert_representation.py
--rwxr-xr-x   0        0        0      916 2023-06-01 22:36:35.353705 mezcla-1.3.7.post1/mezcla/tests/test_simple_main_example.py
--rwxr-xr-x   0        0        0     2083 2023-06-01 22:36:35.353705 mezcla-1.3.7.post1/mezcla/tests/test_spacy_nlp.py
--rwxr-xr-x   0        0        0      882 2023-04-30 22:44:00.974590 mezcla-1.3.7.post1/mezcla/tests/test_sys_version_info_hack.py
--rwxr-xr-x   0        0        0    33402 2023-06-01 22:36:35.353705 mezcla-1.3.7.post1/mezcla/tests/test_system.py
--rwxr-xr-x   0        0        0     1769 2023-04-30 22:44:00.974590 mezcla-1.3.7.post1/mezcla/tests/test_template.py
--rwxr-xr-x   0        0        0     3714 2023-04-30 22:47:21.050725 mezcla-1.3.7.post1/mezcla/tests/test_text_categorizer.py
--rwxr-xr-x   0        0        0     7264 2023-04-30 22:47:21.050725 mezcla-1.3.7.post1/mezcla/tests/test_text_processing.py
--rwxr-xr-x   0        0        0     7362 2023-04-30 22:44:00.974590 mezcla-1.3.7.post1/mezcla/tests/test_text_utils.py
--rwxr-xr-x   0        0        0    21785 2023-04-30 22:44:00.974590 mezcla-1.3.7.post1/mezcla/tests/test_tpo_common.py
--rwxr-xr-x   0        0        0      715 2023-04-30 22:44:00.974590 mezcla-1.3.7.post1/mezcla/tests/test_train_language_model.py
--rwxr-xr-x   0        0        0      725 2023-04-30 22:44:00.974590 mezcla-1.3.7.post1/mezcla/tests/test_train_text_categorizer.py
--rwxr-xr-x   0        0        0      686 2023-04-30 22:44:00.974590 mezcla-1.3.7.post1/mezcla/tests/test_transpose_data.py
--rwxr-xr-x   0        0        0     2859 2023-04-30 22:44:00.974590 mezcla-1.3.7.post1/mezcla/tests/test_xml_utils.py
--rw-r--r--   0        0        0      676 2023-04-30 22:44:00.974590 mezcla-1.3.7.post1/mezcla/tests/tfidf/test_corpus.py
--rw-r--r--   0        0        0      697 2023-04-30 22:44:00.974590 mezcla-1.3.7.post1/mezcla/tests/tfidf/test_dockeyword.py
--rw-r--r--   0        0        0      688 2023-04-30 22:44:00.978591 mezcla-1.3.7.post1/mezcla/tests/tfidf/test_document.py
--rw-r--r--   0        0        0      697 2023-04-30 22:44:00.978591 mezcla-1.3.7.post1/mezcla/tests/tfidf/test_preprocess.py
--rwxr-xr-x   0        0        0    33807 2023-04-30 22:44:00.978591 mezcla-1.3.7.post1/mezcla/text_categorizer.py
--rwxr-xr-x   0        0        0    23204 2023-06-01 22:36:35.353705 mezcla-1.3.7.post1/mezcla/text_processing.py
--rwxr-xr-x   0        0        0    16223 2023-04-30 22:44:00.978591 mezcla-1.3.7.post1/mezcla/text_utils.py
--rwxr-xr-x   0        0        0      375 2022-07-10 04:39:58.387124 mezcla-1.3.7.post1/mezcla/tfidf/__init__.py
--rwxr-xr-x   0        0        0    18423 2023-04-30 22:44:00.978591 mezcla-1.3.7.post1/mezcla/tfidf/corpus.py
--rwxr-xr-x   0        0        0     2282 2023-04-30 22:44:00.978591 mezcla-1.3.7.post1/mezcla/tfidf/dockeyword.py
--rwxr-xr-x   0        0        0     7983 2023-04-30 22:44:00.978591 mezcla-1.3.7.post1/mezcla/tfidf/document.py
-lrwxr-xr-x   0        0        0        0 2022-06-03 04:33:57.207684 mezcla-1.3.7.post1/mezcla/tfidf/old-version -> /home/tomohara/python/tfidf
--rwxr-xr-x   0        0        0    16163 2023-04-30 22:44:00.982591 mezcla-1.3.7.post1/mezcla/tfidf/preprocess.py
--rwxr-xr-x   0        0        0    59862 2023-04-30 22:44:00.982591 mezcla-1.3.7.post1/mezcla/tpo_common.py
--rwxr-xr-x   0        0        0     5267 2022-04-12 04:31:30.000000 mezcla-1.3.7.post1/mezcla/train_language_model.py
--rwxr-xr-x   0        0        0     5098 2021-10-22 05:45:54.000000 mezcla-1.3.7.post1/mezcla/train_text_categorizer.py
--rwxr-xr-x   0        0        0     6778 2021-09-30 12:02:57.000000 mezcla-1.3.7.post1/mezcla/transpose_data.py
--rw-r--r--   0        0        0    12935 2023-06-01 22:36:35.353705 mezcla-1.3.7.post1/mezcla/unittest_wrapper.py
--rwxr-xr-x   0        0        0     3543 2022-04-12 04:50:46.000000 mezcla-1.3.7.post1/mezcla/xml_utils.py
--rw-r--r--   0        0        0      958 2022-06-03 04:33:57.211684 mezcla-1.3.7.post1/pyproject.toml
--rw-r--r--   0        0        0     2335 2023-06-01 22:36:35.353705 mezcla-1.3.7.post1/requirements.txt
--rw-r--r--   0        0        0     1168 2023-06-01 23:40:23.173757 mezcla-1.3.7.post1/setup.py
--rwxr-xr-x   0        0        0    45023 2022-07-16 02:44:46.791484 mezcla-1.3.7.post1/temp/simple_batspp.py
--rwxr-xr-x   0        0        0      862 2023-06-01 22:36:35.353705 mezcla-1.3.7.post1/tools/run_tests.bash
--rw-r--r--   0        0        0      612 2023-06-01 22:36:35.353705 mezcla-1.3.7.post1/tox.ini
--rw-r--r--   0        0        0     1091 1970-01-01 00:00:00.000000 mezcla-1.3.7.post1/PKG-INFO
+-rw-r--r--   0        0        0      542 2023-06-18 00:28:36.095854 mezcla-1.3.8/.coveragerc
+-rw-r--r--   0        0        0     1042 2023-06-18 00:28:36.095854 mezcla-1.3.8/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     1937 2023-06-18 00:29:02.178395 mezcla-1.3.8/.gitignore
+-rw-r--r--   0        0        0     2621 2023-06-18 00:28:36.095854 mezcla-1.3.8/Dockerfile
+-rw-r--r--   0        0        0     7370 2023-06-18 00:28:36.095854 mezcla-1.3.8/LICENSE.txt
+-rw-r--r--   0        0        0      777 2023-06-18 00:28:36.095854 mezcla-1.3.8/README.txt
+-rw-r--r--   0        0        0      380 2023-06-18 00:28:36.095854 mezcla-1.3.8/TODO.txt
+-rw-r--r--   0        0        0      130 2023-06-18 00:28:36.095854 mezcla-1.3.8/mezcla/TODO.md
+-rwxr-xr-x   0        0        0     1927 2023-06-21 08:32:51.710523 mezcla-1.3.8/mezcla/__init__.py
+-rwxr-xr-x   0        0        0    10860 2023-06-18 00:28:36.095854 mezcla-1.3.8/mezcla/analyze_tfidf.py
+-rwxr-xr-x   0        0        0    13025 2023-06-18 00:36:41.989782 mezcla-1.3.8/mezcla/audio.py
+-rwxr-xr-x   0        0        0     4707 2023-06-18 00:28:36.099855 mezcla-1.3.8/mezcla/bash_ast.py
+-rwxr-xr-x   0        0        0    16055 2023-06-18 00:28:36.099855 mezcla-1.3.8/mezcla/bert_multi_classification.py
+-rwxr-xr-x   0        0        0    25702 2023-06-18 00:28:36.099855 mezcla-1.3.8/mezcla/bert_text_classification.py
+-rwxr-xr-x   0        0        0     7625 2023-06-18 00:28:36.099855 mezcla-1.3.8/mezcla/bing_search.py
+-rwxr-xr-x   0        0        0     8925 2023-06-18 00:28:36.099855 mezcla-1.3.8/mezcla/check_html_javascript.py
+-rwxr-xr-x   0        0        0    14338 2023-06-18 00:28:36.099855 mezcla-1.3.8/mezcla/compute_tfidf.py
+-rwxr-xr-x   0        0        0    22279 2023-06-18 00:28:36.099855 mezcla-1.3.8/mezcla/cut.py
+-rwxr-xr-x   0        0        0     4307 2023-06-18 00:28:36.099855 mezcla-1.3.8/mezcla/data_utils.py
+-rwxr-xr-x   0        0        0    47920 2023-06-18 00:29:02.182396 mezcla-1.3.8/mezcla/debug.py
+-rw-r--r--   0        0        0    25047 2023-06-18 00:28:36.103855 mezcla-1.3.8/mezcla/docs/audio_uml.svg
+-rwxr-xr-x   0        0        0        0 2023-06-18 00:28:36.103855 mezcla-1.3.8/mezcla/examples/__init__.py
+-rwxr-xr-x   0        0        0    12834 2023-06-18 00:28:36.103855 mezcla-1.3.8/mezcla/examples/alt_sklearn_plot_precision_recall.py
+-rwxr-xr-x   0        0        0     3608 2023-06-18 00:28:36.103855 mezcla-1.3.8/mezcla/examples/brownlee_ml_metrics.py
+-rwxr-xr-x   0        0        0     2419 2023-06-18 00:28:36.103855 mezcla-1.3.8/mezcla/examples/consume_all_memory.py
+-rwxr-xr-x   0        0        0     5008 2023-06-18 00:28:36.103855 mezcla-1.3.8/mezcla/examples/download_user_gist.py
+-rwxr-xr-x   0        0        0     6477 2023-06-18 00:28:36.103855 mezcla-1.3.8/mezcla/examples/dump_checkpoints.py
+-rw-r--r--   0        0        0     2738 2023-06-18 00:28:36.103855 mezcla-1.3.8/mezcla/examples/encoded-iris.csv
+-rwxr-xr-x   0        0        0     8779 2023-06-18 00:28:36.103855 mezcla-1.3.8/mezcla/examples/feature_importance.py
+-rw-r--r--   0        0        0    40044 2023-06-18 00:28:36.107855 mezcla-1.3.8/mezcla/examples/fuzzy-testing-1-2-3.wav
+-rwxr-xr-x   0        0        0    28364 2023-06-21 06:10:44.430553 mezcla-1.3.8/mezcla/examples/hf_stable_diffusion.py
+-rwxr-xr-x   0        0        0     3338 2023-06-18 00:28:36.107855 mezcla-1.3.8/mezcla/examples/hugging_face_speechrec.py
+-rwxr-xr-x   0        0        0     3922 2023-06-18 00:28:36.107855 mezcla-1.3.8/mezcla/examples/hugging_face_translation.py
+-rwxr-xr-x   0        0        0    10347 2023-06-18 00:28:36.107855 mezcla-1.3.8/mezcla/examples/inspect_checkpoint.py
+-rw-r--r--   0        0        0     4607 2023-06-18 00:28:36.107855 mezcla-1.3.8/mezcla/examples/iris.csv
+-rw-r--r--   0        0        0    23345 2023-06-18 00:28:36.107855 mezcla-1.3.8/mezcla/examples/pima-indians-diabetes.csv
+-rwxr-xr-x   0        0        0     8279 2023-06-18 00:28:36.107855 mezcla-1.3.8/mezcla/examples/plot_forest_importances.py
+-rwxr-xr-x   0        0        0    12989 2023-06-18 00:28:36.107855 mezcla-1.3.8/mezcla/examples/sklearn_plot_precision_recall.py
+-rwxr-xr-x   0        0        0     1938 2023-06-21 06:10:44.430553 mezcla-1.3.8/mezcla/examples/template.py
+-rwxr-xr-x   0        0        0     3155 2023-06-18 00:28:36.107855 mezcla-1.3.8/mezcla/examples/tensorflow_matrix_multiply.py
+-rwxr-xr-x   0        0        0     5006 2023-06-21 06:10:44.430553 mezcla-1.3.8/mezcla/examples/tests/test_hf_stable_diffusion.py
+-rwxr-xr-x   0        0        0     3607 2023-06-18 00:28:36.107855 mezcla-1.3.8/mezcla/examples/tracemalloc_display.py
+-rwxr-xr-x   0        0        0     4031 2023-06-18 00:28:36.107855 mezcla-1.3.8/mezcla/extract_document_text.py
+-rwxr-xr-x   0        0        0     7708 2023-06-18 00:28:36.107855 mezcla-1.3.8/mezcla/file_utils.py
+-rwxr-xr-x   0        0        0     3071 2023-06-18 00:28:36.107855 mezcla-1.3.8/mezcla/filter_random.py
+-rwxr-xr-x   0        0        0     2998 2023-06-18 00:28:36.111856 mezcla-1.3.8/mezcla/format_profile.py
+-rwxr-xr-x   0        0        0    32894 2023-06-18 00:28:36.111856 mezcla-1.3.8/mezcla/gensim_test.py
+-rwxr-xr-x   0        0        0    32756 2023-06-21 06:10:44.430553 mezcla-1.3.8/mezcla/glue_helpers.py
+-rwxr-xr-x   0        0        0    32492 2023-06-18 00:28:36.111856 mezcla-1.3.8/mezcla/html_utils.py
+-rwxr-xr-x   0        0        0     4708 2023-06-18 00:28:36.111856 mezcla-1.3.8/mezcla/kenlm_example.py
+-rwxr-xr-x   0        0        0    17916 2023-06-18 00:28:36.111856 mezcla-1.3.8/mezcla/keras_param_search.py
+-rwxr-xr-x   0        0        0    45741 2023-06-21 08:32:51.714523 mezcla-1.3.8/mezcla/main.py
+-rwxr-xr-x   0        0        0     9307 2023-06-18 00:28:36.115856 mezcla-1.3.8/mezcla/merge_files.py
+-rwxr-xr-x   0        0        0    11717 2023-06-18 00:28:36.115856 mezcla-1.3.8/mezcla/merge_notes.py
+-rwxr-xr-x   0        0        0    11641 2023-06-18 00:28:36.115856 mezcla-1.3.8/mezcla/misc_utils.py
+-rwxr-xr-x   0        0        0     9779 2023-06-18 00:28:36.115856 mezcla-1.3.8/mezcla/my_regex.py
+-rwxr-xr-x   0        0        0    13776 2023-06-18 00:28:36.115856 mezcla-1.3.8/mezcla/ngram_tfidf.py
+-rwxr-xr-x   0        0        0      737 2023-06-18 00:28:36.115856 mezcla-1.3.8/mezcla/os_utils.py
+-rwxr-xr-x   0        0        0    31436 2023-06-18 00:28:36.115856 mezcla-1.3.8/mezcla/pandas_sklearn.py
+-rwxr-xr-x   0        0        0      828 2023-06-18 00:28:36.115856 mezcla-1.3.8/mezcla/plot_utils.py
+-rwxr-xr-x   0        0        0     7053 2023-06-18 00:28:36.115856 mezcla-1.3.8/mezcla/randomize_lines.py
+-rwxr-xr-x   0        0        0     7604 2023-06-18 00:29:02.182396 mezcla-1.3.8/mezcla/rgb_color_name.py
+-rwxr-xr-x   0        0        0    40529 2023-06-18 00:28:36.115856 mezcla-1.3.8/mezcla/run_albert_classifier.py
+-rwxr-xr-x   0        0        0    39613 2023-06-18 00:28:36.119856 mezcla-1.3.8/mezcla/run_bert_classifier.py
+-rwxr-xr-x   0        0        0    17400 2023-06-18 00:28:36.119856 mezcla-1.3.8/mezcla/show_bert_representation.py
+-rwxr-xr-x   0        0        0     1508 2023-06-18 00:28:36.119856 mezcla-1.3.8/mezcla/simple_main_example.py
+-rwxr-xr-x   0        0        0    19931 2023-06-18 00:28:36.119856 mezcla-1.3.8/mezcla/spacy_nlp.py
+-rwxr-xr-x   0        0        0     3011 2023-06-18 00:28:36.119856 mezcla-1.3.8/mezcla/spell.py
+-rwxr-xr-x   0        0        0     2416 2023-06-18 00:28:36.119856 mezcla-1.3.8/mezcla/sys_version_info_hack.py
+-rwxr-xr-x   0        0        0    50554 2023-06-21 06:10:44.434553 mezcla-1.3.8/mezcla/system.py
+-rwxr-xr-x   0        0        0    45776 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/temp/simple_batspp.py
+-rwxr-xr-x   0        0        0     5594 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/template.py
+-rw-r--r--   0        0        0     7370 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/LICENSE.txt
+-rw-r--r--   0        0        0      462 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/TODO.md
+-rw-r--r--   0        0        0     1082 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/adhoc-tests.batspp
+-rw-r--r--   0        0        0      204 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/misc-tests.batspp
+-rwxr-xr-x   0        0        0     3905 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/misc_doctests.py
+-rw-r--r--   0        0        0      810 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/resources/cars-csv-len-3.txt
+-rw-r--r--   0        0        0      113 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/resources/cars-fields-2-3-4.txt
+-rw-r--r--   0        0        0      602 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/resources/cars-tsv-len-3.txt
+-rw-r--r--   0        0        0      659 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/resources/cars.csv
+-rw-r--r--   0        0        0      655 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/resources/cars.tsv
+-rw-r--r--   0        0        0      603 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/resources/example_text.txt
+-rw-r--r--   0        0        0     2573 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/resources/example_text_tags.txt
+-rw-r--r--   0        0        0     2440 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/resources/iris_output.txt
+-rw-r--r--   0        0        0     1152 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/resources/simple-window-dimensions.html
+-rw-r--r--   0        0        0     5577 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/resources/spanish-accents.docx
+-rw-r--r--   0        0        0    12530 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/resources/spanish-accents.pdf
+-rw-r--r--   0        0        0      141 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/resources/spanish-accents.txt
+-rw-r--r--   0        0        0       65 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/resources/word-POS.freq
+-rw-r--r--   0        0        0      254 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/simple-script-tests.test
+-rwxr-xr-x   0        0        0     4816 2023-06-18 00:29:02.182396 mezcla-1.3.8/mezcla/tests/template.py
+-rwxr-xr-x   0        0        0     2489 2023-06-18 00:29:02.182396 mezcla-1.3.8/mezcla/tests/test___init__.py
+-rwxr-xr-x   0        0        0     4736 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/test_audio.py
+-rwxr-xr-x   0        0        0      969 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/test_bert_multi_classification.py
+-rwxr-xr-x   0        0        0      834 2023-06-18 00:28:36.123857 mezcla-1.3.8/mezcla/tests/test_bing_search.py
+-rwxr-xr-x   0        0        0     1974 2023-06-18 00:28:36.127857 mezcla-1.3.8/mezcla/tests/test_compute_tfidf.py
+-rwxr-xr-x   0        0        0     2905 2023-06-18 00:28:36.127857 mezcla-1.3.8/mezcla/tests/test_cut.py
+-rwxr-xr-x   0        0        0     2464 2023-06-18 00:28:36.127857 mezcla-1.3.8/mezcla/tests/test_data_utils.py
+-rwxr-xr-x   0        0        0    15032 2023-06-18 00:28:36.127857 mezcla-1.3.8/mezcla/tests/test_debug.py
+-rwxr-xr-x   0        0        0     1030 2023-06-18 00:28:36.127857 mezcla-1.3.8/mezcla/tests/test_extract_document_text.py
+-rwxr-xr-x   0        0        0     4429 2023-06-18 00:28:36.127857 mezcla-1.3.8/mezcla/tests/test_file_utils.py
+-rwxr-xr-x   0        0        0     2939 2023-06-18 00:28:36.127857 mezcla-1.3.8/mezcla/tests/test_filter_random.py
+-rwxr-xr-x   0        0        0     2562 2023-06-18 00:28:36.127857 mezcla-1.3.8/mezcla/tests/test_gensim_test.py
+-rwxr-xr-x   0        0        0    15711 2023-06-18 00:28:36.127857 mezcla-1.3.8/mezcla/tests/test_glue_helpers.py
+-rwxr-xr-x   0        0        0    13008 2023-06-18 00:28:36.127857 mezcla-1.3.8/mezcla/tests/test_html_utils.py
+-rwxr-xr-x   0        0        0      892 2023-06-18 00:28:36.127857 mezcla-1.3.8/mezcla/tests/test_kenlm_example.py
+-rwxr-xr-x   0        0        0     2114 2023-06-18 00:28:36.127857 mezcla-1.3.8/mezcla/tests/test_keras_param_search.py
+-rwxr-xr-x   0        0        0     8972 2023-06-18 00:28:36.127857 mezcla-1.3.8/mezcla/tests/test_main.py
+-rwxr-xr-x   0        0        0     2725 2023-06-18 00:28:36.127857 mezcla-1.3.8/mezcla/tests/test_merge_files.py
+-rwxr-xr-x   0        0        0     1291 2023-06-18 00:28:36.127857 mezcla-1.3.8/mezcla/tests/test_merge_notes.py
+-rwxr-xr-x   0        0        0     6565 2023-06-18 00:28:36.127857 mezcla-1.3.8/mezcla/tests/test_misc_utils.py
+-rwxr-xr-x   0        0        0     2882 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_my_regex.py
+-rwxr-xr-x   0        0        0      916 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_ngram_tfidf.py
+-rwxr-xr-x   0        0        0      931 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_os_utils.py
+-rwxr-xr-x   0        0        0     8323 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_pandas_sklearn.py
+-rwxr-xr-x   0        0        0     1215 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_plot_utils.py
+-rwxr-xr-x   0        0        0      854 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_randomize_lines.py
+-rwxr-xr-x   0        0        0     2869 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_rgb_color_name.py
+-rwxr-xr-x   0        0        0      895 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_run_albert_classifier.py
+-rwxr-xr-x   0        0        0      930 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_run_bert_classifier.py
+-rwxr-xr-x   0        0        0     1602 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_show_bert_representation.py
+-rwxr-xr-x   0        0        0      916 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_simple_main_example.py
+-rwxr-xr-x   0        0        0     2083 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_spacy_nlp.py
+-rwxr-xr-x   0        0        0      882 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_sys_version_info_hack.py
+-rwxr-xr-x   0        0        0    33402 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_system.py
+-rwxr-xr-x   0        0        0     1769 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_template.py
+-rwxr-xr-x   0        0        0     3714 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_text_categorizer.py
+-rwxr-xr-x   0        0        0     7264 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_text_processing.py
+-rwxr-xr-x   0        0        0     7362 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_text_utils.py
+-rwxr-xr-x   0        0        0    21785 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_tpo_common.py
+-rwxr-xr-x   0        0        0      715 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_train_language_model.py
+-rwxr-xr-x   0        0        0      725 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_train_text_categorizer.py
+-rwxr-xr-x   0        0        0      686 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_transpose_data.py
+-rwxr-xr-x   0        0        0     2859 2023-06-18 00:28:36.131858 mezcla-1.3.8/mezcla/tests/test_xml_utils.py
+-rwxr-xr-x   0        0        0      676 2023-06-18 00:29:02.186396 mezcla-1.3.8/mezcla/tests/tfidf/test_corpus.py
+-rwxr-xr-x   0        0        0      697 2023-06-18 00:29:02.186396 mezcla-1.3.8/mezcla/tests/tfidf/test_dockeyword.py
+-rwxr-xr-x   0        0        0      688 2023-06-18 00:29:02.186396 mezcla-1.3.8/mezcla/tests/tfidf/test_document.py
+-rwxr-xr-x   0        0        0      697 2023-06-18 00:29:02.186396 mezcla-1.3.8/mezcla/tests/tfidf/test_preprocess.py
+-rwxr-xr-x   0        0        0    33807 2023-06-18 00:28:36.135858 mezcla-1.3.8/mezcla/text_categorizer.py
+-rwxr-xr-x   0        0        0    23204 2023-06-18 00:28:36.135858 mezcla-1.3.8/mezcla/text_processing.py
+-rwxr-xr-x   0        0        0    16223 2023-06-18 00:28:36.135858 mezcla-1.3.8/mezcla/text_utils.py
+-rwxr-xr-x   0        0        0      375 2023-06-18 00:28:36.135858 mezcla-1.3.8/mezcla/tfidf/__init__.py
+-rwxr-xr-x   0        0        0    18423 2023-06-18 00:28:36.135858 mezcla-1.3.8/mezcla/tfidf/corpus.py
+-rwxr-xr-x   0        0        0     2282 2023-06-18 00:28:36.135858 mezcla-1.3.8/mezcla/tfidf/dockeyword.py
+-rwxr-xr-x   0        0        0     7983 2023-06-18 00:28:36.135858 mezcla-1.3.8/mezcla/tfidf/document.py
+lrwxr-xr-x   0        0        0        0 2023-06-18 00:28:36.135858 mezcla-1.3.8/mezcla/tfidf/old-version -> /home/tomohara/python/tfidf
+-rwxr-xr-x   0        0        0    16163 2023-06-18 00:28:36.135858 mezcla-1.3.8/mezcla/tfidf/preprocess.py
+-rwxr-xr-x   0        0        0    59862 2023-06-18 00:28:36.139858 mezcla-1.3.8/mezcla/tpo_common.py
+-rwxr-xr-x   0        0        0     5267 2023-06-18 00:28:36.139858 mezcla-1.3.8/mezcla/train_language_model.py
+-rwxr-xr-x   0        0        0     5098 2023-06-18 00:28:36.139858 mezcla-1.3.8/mezcla/train_text_categorizer.py
+-rwxr-xr-x   0        0        0     6778 2023-06-18 00:28:36.139858 mezcla-1.3.8/mezcla/transpose_data.py
+-rwxr-xr-x   0        0        0    13361 2023-06-18 00:29:02.186396 mezcla-1.3.8/mezcla/unittest_wrapper.py
+-rwxr-xr-x   0        0        0     3543 2023-06-18 00:28:36.139858 mezcla-1.3.8/mezcla/xml_utils.py
+-rw-r--r--   0        0        0      958 2023-06-18 00:28:36.139858 mezcla-1.3.8/pyproject.toml
+-rw-r--r--   0        0        0     2432 2023-06-18 00:29:02.186396 mezcla-1.3.8/requirements.txt
+-rwxr-xr-x   0        0        0     1162 2023-06-21 08:32:51.714523 mezcla-1.3.8/setup.py
+-rwxr-xr-x   0        0        0    45023 2023-06-18 00:28:36.139858 mezcla-1.3.8/temp/simple_batspp.py
+-rwxr-xr-x   0        0        0      862 2023-06-18 00:28:36.139858 mezcla-1.3.8/tools/run_tests.bash
+-rw-r--r--   0        0        0      612 2023-06-18 00:28:36.139858 mezcla-1.3.8/tox.ini
+-rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 mezcla-1.3.8/PKG-INFO
```

### Comparing `mezcla-1.3.7.post1/.coveragerc` & `mezcla-1.3.8/.coveragerc`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/.github/workflows/tests.yml` & `mezcla-1.3.8/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/.gitignore` & `mezcla-1.3.8/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Rules for telling git which untracked files to ignore, mainly based on
 # file extension but also accounting for some idiosyncratic usages.
 #
 # Note:
 # - *** Please add examples when adding exclusions.
-# - ** Also explain if used for non standard Python (e.g., tox.ini)
+# - ** Also explain if used for non standard stuff (e.g., tox.ini with Python).
 # - This is shared across projects, so there might seem to be
 #   some apparently extraneous patterns included.
 # - Used to pruned 'git status' output, which gets
 #   shown during check-in's (as a sanity check).
 # - The patterns are glob-like with the extension that **/GLOB
 #   matches the glob pattern in any subdirectory.
 # - See 'man gitignore' for details.
@@ -20,15 +20,15 @@
 # TODO: figure out how to apply to subdirs
 **/*.log
 **/*.list
 
 # Any files with leading _, except specified cases
 **/_*
 !**/*__init__.py
-# Likewise for trailing _'s (e.g., requirements.link_)
+# Likewise for trailing _'s (e.g., master-dir-link_)
 **/*_
 
 # Special cases
 # TODO: see why excluded by the rules
 # Workflow files (e.g., .github/workflows/tests.yml).
 !.github/**
 
@@ -47,14 +47,20 @@
 
 # Top level distribution dir and related
 # Note: tox support PyPi packaging
 # TODO: dist created by tox utiility???
 dist
 .tox
 
+# Jupyter
+.ipynb_checkpoints
+
+# (maldito) Mac
+.DS_Store
+
 #...............................................................................
 # Idiosyncratic stuff for Tom
 #
 
 # Personal note files
 # ex: reempl-notes.txt
 **/*notes*txt
```

### Comparing `mezcla-1.3.7.post1/Dockerfile` & `mezcla-1.3.8/Dockerfile`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/LICENSE.txt` & `mezcla-1.3.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/README.txt` & `mezcla-1.3.8/README.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/__init__.py` & `mezcla-1.3.8/mezcla/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     from mezcla import *
     debug.trace(TL.DEFAULT, "Hey")
     debug.trace(TL.DETAILED, "Joe")
 
 Tom O'Hara
 Feb 2022
 """
-__VERSION__ = '1.3.7.post1'
+__VERSION__ = '1.3.8'
 __version__ = __VERSION__
 
 # Standard module(s)
 import sys
 
 # Note: requires python 3 or higher
 PYTHON3_PLUS = (sys.version_info[0] >= 3)
```

### Comparing `mezcla-1.3.7.post1/mezcla/analyze_tfidf.py` & `mezcla-1.3.8/mezcla/analyze_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/audio.py` & `mezcla-1.3.8/mezcla/audio.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,16 +100,16 @@
 
     def setup(self):
         """Process arguments"""
         debug.trace(7, f'AudioArgumentProcessing.setup({self})')
 
         # Check the command-line options
         source       = self.get_parsed_argument(SOURCE, "")
-        self.output  = self.get_parsed_argument(OUTPUT, self.output)
-        self.speech  = self.get_parsed_argument(SPEECH, self.speech)
+        self.output  = self.get_parsed_option(OUTPUT, self.output)
+        self.speech  = self.get_parsed_option(SPEECH, self.speech)
         self.verbose = self.get_parsed_option(VERBOSE)
 
         # Process source
         source_match = re.search(r'(?P<path>[\w\-\/]+)\.*(?P<ext>[a-zA-Z0-9]+)* *$', source)
         extension = source_match.group('ext') if source_match else ''
         path      = source_match.group('path') if source_match else ''
```

### Comparing `mezcla-1.3.7.post1/mezcla/bash_ast.py` & `mezcla-1.3.8/mezcla/bash_ast.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/bert_multi_classification.py` & `mezcla-1.3.8/mezcla/bert_multi_classification.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/bert_text_classification.py` & `mezcla-1.3.8/mezcla/bert_text_classification.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/bing_search.py` & `mezcla-1.3.8/mezcla/bing_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/check_html_javascript.py` & `mezcla-1.3.8/mezcla/check_html_javascript.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/compute_tfidf.py` & `mezcla-1.3.8/mezcla/compute_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/cut.py` & `mezcla-1.3.8/mezcla/cut.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/data_utils.py` & `mezcla-1.3.8/mezcla/data_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/debug.py` & `mezcla-1.3.8/mezcla/debug.py`

 * *Files 1% similar despite different names*

```diff
@@ -581,23 +581,25 @@
     def assertion(expression, message=None, assert_level=None):
         """Issue warning if EXPRESSION doesn't hold, along with optional MESSAGE
         Note:
         - This is a "soft assertion" that doesn't raise an exception (n.b., provided the test doesn't do so).
         - Currently, the expression text is not resolved properly under ipython (or Jupyter).
         - The optional ASSERT_LEVEL overrides use of ALWAYS.
         - Uses introspection to derive text for assertion expression.
+        - Returns expression text or None if not triggered.
         """
         # EX: assertion((2 + 2) != 5)
         # TODO: have streamlined version using sys.write that can be used for trace and trace_fmtd sanity checks about {}'s
         # TODO: trace out local and globals to aid in diagnosing assertion failures; ex: add automatic tarcing of variables used in the assertion expression)
+        expression_text = None
         if (assert_level is None):
             assert_level = ALWAYS
         if (trace_level < assert_level):
             # note: Short-circuits processing to avoid extraneous warnings (e.g., trace_expr under ipython)
-            return
+            return expression_text
         if (not expression):
             try:
                 # Get source information for failed assertion
                 trace_fmtd(MOST_VERBOSE, "Call stack: {st}", st=inspect.stack())
                 caller = inspect.stack()[1]
                 ## OLD: (_frame, filename, line_number, _function, _context, _index) = caller
                 (_frame, filename, line_number, _function, context, _index) = caller
@@ -609,24 +611,25 @@
                     ## OLD: statement = str(context).replace(")\\n']", "")
                     statement = str(context).replace("\\n']", "")
                 # Format expression and message
                 # note: removes comments, along with the assertion call prefix and suffix
                 statement = re.sub("#.*$", "", statement)
                 statement = re.sub(r"^(\S*)assertion\(", "", statement)
                 expression = re.sub(r"\);?\s*$", "", statement)
+                expression_text = expression
                 qualification_spec = (": " + message) if message else ""
                 # Output information
                 # TODO: omit subsequent warnings
                 trace_fmtd(ALWAYS, "Assertion failed: {expr} (at {file}:{line}){qual}",
                            expr=expression, file=filename, line=line_number, qual=qualification_spec)
             except:
                 trace_fmtd(ALWAYS, "Exception formatting assertion: {exc}",
                            exc=sys.exc_info())
                 trace_object(ALWAYS, inspect.currentframe(), "caller frame", pretty_print=True)
-        return
+        return expression_text
 
     def val(level, value):
         """Returns VALUE if at trace LEVEL or higher otherwise None
         Note: inspired by Lisp's convenient IF form without an explicit else: (if test value-if-true)"""
         # EX: (101 if ((get_level() == 1) and val(1, 101)) else None) => 101
         # EX: ((not __debug__) and val(trace_level, 101))) => None
         # TODO: rename as cond_value???
@@ -980,15 +983,15 @@
         trace_fmtd(VERBOSE, "debug_filename={fn} debug_file={f}",
                    fn=debug_filename, f=debug_file)
         return
 
     def reopen_debug_file():
         """Re-open debug file to work around concurrent access issues
         Note: The debug file is mainly used with pytest to work around stderr tracing issues"""
-        trace(5, "open_debug_file()")
+        trace(5, "reopen_debug_file()")
         global debug_file
         assertion(debug_file is not None)
 
         # Close file if opened
         if debug_file:
             debug_file.close()
             debug_file = None
@@ -998,15 +1001,19 @@
         return
                         
 
     def debug_init():
         """Debug-only initialization"""
         time_start = time.time()
         trace(DETAILED, f"in debug_init(); {timestamp()}")
-        trace(USUAL, " ".join(sys.argv))
+        # note: shows command invocation unless invoked via "python -c ..."
+        command_line = " ".join(sys.argv)
+        assertion(command_line)
+        if (command_line and (command_line != "-c")):
+            trace(USUAL, command_line)
         trace_expr(DETAILED, sys.argv)
         open_debug_file()
 
         # Determine whether tracing include time and date
         global output_timestamps
         ## OLD
         ## output_timestamps = (str(os.environ.get("OUTPUT_DEBUG_TIMESTAMPS", False)).upper()
```

### Comparing `mezcla-1.3.7.post1/mezcla/docs/audio_uml.svg` & `mezcla-1.3.8/mezcla/docs/audio_uml.svg`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/examples/alt_sklearn_plot_precision_recall.py` & `mezcla-1.3.8/mezcla/examples/alt_sklearn_plot_precision_recall.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/examples/brownlee_ml_metrics.py` & `mezcla-1.3.8/mezcla/examples/brownlee_ml_metrics.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/examples/consume_all_memory.py` & `mezcla-1.3.8/mezcla/examples/consume_all_memory.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/examples/download_user_gist.py` & `mezcla-1.3.8/mezcla/examples/download_user_gist.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/examples/dump_checkpoints.py` & `mezcla-1.3.8/mezcla/examples/dump_checkpoints.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/examples/encoded-iris.csv` & `mezcla-1.3.8/mezcla/examples/encoded-iris.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/examples/feature_importance.py` & `mezcla-1.3.8/mezcla/examples/feature_importance.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/examples/fuzzy-testing-1-2-3.wav` & `mezcla-1.3.8/mezcla/examples/fuzzy-testing-1-2-3.wav`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/examples/hugging_face_speechrec.py` & `mezcla-1.3.8/mezcla/examples/hugging_face_speechrec.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/examples/hugging_face_translation.py` & `mezcla-1.3.8/mezcla/examples/hugging_face_translation.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/examples/inspect_checkpoint.py` & `mezcla-1.3.8/mezcla/examples/inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/examples/iris.csv` & `mezcla-1.3.8/mezcla/examples/iris.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/examples/pima-indians-diabetes.csv` & `mezcla-1.3.8/mezcla/examples/pima-indians-diabetes.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/examples/plot_forest_importances.py` & `mezcla-1.3.8/mezcla/examples/plot_forest_importances.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/examples/sklearn_plot_precision_recall.py` & `mezcla-1.3.8/mezcla/examples/sklearn_plot_precision_recall.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/examples/template.py` & `mezcla-1.3.8/mezcla/examples/template.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,28 +8,30 @@
 TODO: what module does (brief)
 
 Sample usage:
    echo $'TODO:task1\\nDONE:task2' | {script} --TODO-arg --
 """
 
 # Standard modules
-# TODO: import re
+## TODO: import json
 
 # Intalled module
 # TODO: import numpy as np
 
 # Local modules
 from mezcla import debug
 from mezcla import glue_helpers as gh
 from mezcla.main import Main
+## TODO: from mezcla.my_regex import my_re
 from mezcla import system
 ## TODO2: streamline imports by exposing common functions, etc. in mezcla
 
 # Constants
 TL = debug.TL
+## TODO: TODO_OPT1 = "todo-option1"
 
 ## TODO:
 ## # Environment options
 ## # Notes:
 ## # - These are just intended for internal options, not for end users.
 ## # - They also allow for enabling options in one place rather than four
 ## #   when using main.Main (e.g., [Main member] initialization, run-time
@@ -40,18 +42,21 @@
 
 #-------------------------------------------------------------------------------
 
 def main():
     """Entry point"""
     debug.trace(TL.USUAL, f"main(): script={system.real_path(__file__)}")
 
-    # Show simple usage if --help given
-    dummy_main_app = Main(description=__doc__.format(script=gh.basename(__file__)),
-                          skip_input=False, manual_input=False)
-    debug.assertion(dummy_main_app.parsed_args)
+    # Parse command line options, show usage if --help given
+    # TODO: manual_input=True; short_options=True
+    main_app = Main(description=__doc__.format(script=gh.basename(__file__)),
+                    ## TODO: boolean_boolean_options=[(TODO_OPT1, "TODO desc1")]
+                    skip_input=False)
+    debug.assertion(main_app.parsed_args)
+    ## TODO_OPT1 = main_app.get_parsed_option(TODO_OPT1)
 
     ## TODO:
     system.print_error("Error: Implement me!")
     return
 
 #-------------------------------------------------------------------------------
```

### Comparing `mezcla-1.3.7.post1/mezcla/examples/tensorflow_matrix_multiply.py` & `mezcla-1.3.8/mezcla/examples/tensorflow_matrix_multiply.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/examples/tracemalloc_display.py` & `mezcla-1.3.8/mezcla/examples/tracemalloc_display.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/extract_document_text.py` & `mezcla-1.3.8/mezcla/extract_document_text.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/file_utils.py` & `mezcla-1.3.8/mezcla/file_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/filter_random.py` & `mezcla-1.3.8/mezcla/filter_random.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/format_profile.py` & `mezcla-1.3.8/mezcla/format_profile.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/gensim_test.py` & `mezcla-1.3.8/mezcla/gensim_test.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/glue_helpers.py` & `mezcla-1.3.8/mezcla/glue_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,18 +80,18 @@
     return temp_file_name
 #
 TEMP_LOG_FILE = tpo.getenv_text("TEMP_LOG_FILE", get_temp_file() + "-log",
                                 "Log file for stderr such as for issue function")
 TEMP_SCRIPT_FILE = tpo.getenv_text("TEMP_SCRIPT_FILE", get_temp_file() + "-script",
                                    "File for command invocation")
 
-def create_temp_file(contents):
+def create_temp_file(contents, binary=False):
     """Create temporary file with CONTENTS and return full path"""
     temp_filename = get_temp_file()
-    system.write_file(temp_filename, contents)
+    system.write_file(temp_filename, contents, binary=binary)
     debug.trace(6, "create_temp_file({contents!r}) => {temp_filename}")
     return temp_filename
 
 
 def basename(filename, extension=None):
     """Remove directory from FILENAME along with optional EXTENSION, as with Unix basename command. Note: the period in the extension must be explicitly supplied (e.g., '.data' not 'data')"""
     # EX: basename("fubar.py", ".py") => "fubar"
```

### Comparing `mezcla-1.3.7.post1/mezcla/html_utils.py` & `mezcla-1.3.8/mezcla/html_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/kenlm_example.py` & `mezcla-1.3.8/mezcla/kenlm_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/keras_param_search.py` & `mezcla-1.3.8/mezcla/keras_param_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/main.py` & `mezcla-1.3.8/mezcla/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #    from main import Main
 #
 #    class MyMain(Main):
 #       def process_line(self, line):
 #           if "funny" in line:
 #               print("Funny looking line: %s" % line)
 #
-#    if __name__ == '__main__':
+#    if __name__ == "__main__":
 #        MyMain().run()
 #    
 # Notes:
 # - See simple_main_example.py for a non-trivial example.
 # - To add command-line arguments, pass corresponding arguments to Main's
 #   initialization. For example,
 #      Main(boolean_options=["fubar"], 
@@ -52,16 +52,17 @@
 #   was added to facilitate porting Perl scripts, especially those used in aliases. See
 #      https://github.com/tomasohara/shell-scripts/blob/main/tomohara-aliases.bash
 #   For example, https://github.com/tomasohara/shell-scripts/blob/main/check_errors.py.
 # - This requires a workaround due to an argparse limitation:
 #      https://github.com/spotify/luigi/issues/193 [boolean as command-line arg]
 #
 # TODO:
-# - *** Convert tpo_common calls (i.e., tpo.xyz) to debug!'
+# - *** Convert tpo_common calls (i.e., tpo.xyz) to debug!
 # - * Clarify TEMP_BASE vs. TEMP_FILE usage.
+# - ** Create cheatsheet for argparse tricks (e.,g., using argparse.SUPPRESS to hide).
 # - Specify argument via input dicts, such as in 
 #      options=[{"name": "fubar", "type": bool}, 
 #               {"name": "count", type: int, default: 10}]
 # - Add support for perl-style paragraph mode in input processing.
 # - Add support for multple input files (e.g., via fileinput module).
 # - Add support for csv.csv_reader (see usage in cut.py).
 # - Add support for argument aliases (e.g., --input-delim for --delim).
@@ -118,14 +119,16 @@
 BRIEF_USAGE = system.getenv_bool("BRIEF_USAGE", False,
                                  "Show brief usage with autohelp")
 PERL_SWITCH_PARSING = system.getenv_bool("PERL_SWITCH_PARSING", False,
                                          "Preprocess args to expand Perl-style -var[=[val=1]] to --var=val")
 ## HACK: This is needed if boolean options default to true based on run-time initialization
 NEGATIVE_BOOL_ARGS = system.getenv_bool("NEGATIVE_BOOL_ARGS", False,
                                         "Add negation option for each boolean option")
+SHORT_OPTIONS = system.getenv_bool("SHORT_OPTIONS", False,
+                                   "Automatically derive short options")
 
 #-------------------------------------------------------------------------------
 
 class Main(object):
     """Class encompassing common script processing"""
     argument_parser = None
     force_unicode = False
@@ -140,29 +143,30 @@
                  multiple_files=False,
                  use_temp_base_dir=None,
                  usage_notes=None,
                  program=None,
                  paragraph_mode=None, track_pages=None, file_input_mode=None, newlines=None,
                  boolean_options=None, text_options=None, int_options=None,
                  float_options=None, positional_options=None, positional_arguments=None,
-                 skip_input=None, manual_input=None, auto_help=None, brief_usage=None, **kwargs):
+                 skip_input=None, manual_input=None, auto_help=None, brief_usage=None,
+                 short_options=None, **kwargs):
         """Class constructor: parses RUNTIME_ARGS (or command line), with specifications
         for BOOLEAN_OPTIONS, TEXT_OPTIONS, INT_OPTIONS, FLOAT_OPTIONS, and POSITIONAL_OPTIONS
-        (see convert_option). Includes options to SKIP_INPUT, or to have MANUAL_INPUT, or to use AUTO_HELP invocation (i.e., assuming {ha} if no args)."""
+        (see convert_option). Includes options to SKIP_INPUT, or to have MANUAL_INPUT, or to use AUTO_HELP invocation (i.e., assuming {ha} if no args). Also allows for SHORT_OPTIONS"""
         tpo.debug_format("Main.__init__({args}, d={desc}, b={bools}, t={texts},"
                          + " i={ints}, f={floats}, po={posns}, pa={pargs}, si={skip}, m={mi}, ah={auto}, bu={usage},"
                          + " pm={para}, tp={page}, fim={file}, nl={nl}, prog={prog}, sa={skip_args},"
-                         + " mult={mf}, temp_base={utbd} notes={us} kw={kw})", 5,
+                         + " mult={mf}, temp_base={utbd} notes={us} short={so} kw={kw})", 5,
                          args=runtime_args, desc=description, bools=boolean_options,
                          texts=text_options, ints=int_options, floats=float_options,
                          mf=multiple_files, utbd=use_temp_base_dir,
                          posns=positional_options, pargs=positional_arguments, skip=skip_input, mi=manual_input,
                          auto=auto_help, usage=brief_usage, us=usage_notes,
                          para=paragraph_mode, page=track_pages, file=file_input_mode, nl=newlines,
-                         prog=program, ha=HELP_ARG, skip_args=skip_args, kw=kwargs)
+                         prog=program, ha=HELP_ARG, skip_args=skip_args, so=short_options, kw=kwargs)
         self.description = "TODO: what the script does"   # *** DONT'T MODIFY: default TODO note for client
         self.boolean_options = []
         self.text_options = []
         self.int_options = []
         self.float_options = []
         self.positional_options = []
         self.process_line_warning = False
@@ -178,15 +182,15 @@
         self.char_offset = -1
         self.raw_line = None
         # Note: manual_input was introduced after skip_input to allow for input processing
         # in bulk (e.g., via read_input generator). By default, neither is specified
         # (see template.py), and both should be assumed false.
         # TODO: *** Add better sanity checking (such as a filename on command line).
         if manual_input is None:
-            # NOTE: skip_input=>manual_input: T=>T  F=>F  None=>F
+            # NOTE: skip_input=>manual_input: T=>T  F=>F  None=>F (i.e., bool(skip_input))
             manual_input = False if (skip_input is None) else skip_input
             debug.trace_fmt(7, "inferred manual_input: {mi}", mi=manual_input)
         self.manual_input = manual_input
         if skip_input is None:
             skip_input = self.manual_input
             debug.trace_fmt(7, "inferred skip_input: {si}", si=skip_input)
         self.skip_input = skip_input
@@ -195,38 +199,45 @@
         if brief_usage is None:
             brief_usage = BRIEF_USAGE
         self.brief_usage = brief_usage  # show brief usage instead of full --help
         if auto_help is None:
             ## TODO: rework to be default if none specified for both skip_input and manual_input
             ## OLD: auto_help = self.skip_input
             auto_help = self.skip_input or not self.manual_input
+            debug.trace(7, f"inferred auto_help: {auto_help}")
         self.auto_help = auto_help      # adds --help to command line if no arguments
         if usage_notes is None:
             usage_notes = ""
         self.notes = usage_notes
         if paragraph_mode is None:
             paragraph_mode = USE_PARAGRAPH_MODE
         self.paragraph_mode = paragraph_mode
         if file_input_mode is None:
             file_input_mode = FILE_INPUT_MODE
         self.file_input_mode = file_input_mode
         self.newlines = newlines
         if track_pages is None:
             track_pages = TRACK_PAGES
         self.track_pages = track_pages
-        self.binary_input = kwargs.get("binary_input", False)
+        self.short_options = (short_options if (short_options is not None) else SHORT_OPTIONS)
+
+        # Check miscellaneous options
+        BINARY_INPUT_OPTION = "binary_input"
+        PERL_SWITCH_PARSING_OPTION = "perl_switch_parsing"
+        debug.assertion(not (system.difference(kwargs.keys(), [BINARY_INPUT_OPTION, PERL_SWITCH_PARSING_OPTION])))
+        self.binary_input = kwargs.get(BINARY_INPUT_OPTION, False)
 
         # Setup temporary file and/or base directory
         # Note: Uses NamedTemporaryFile (hence ntf_args)
         # TODO: allow temp_base handling to be overridable by constructor options
         # TODO: reconcile with unittest_wrapper.py.get_temp_dir
         prefix = (FILE_BASE + "-")
-        ntf_args = {'prefix': prefix,
-                    'delete': not debug.detailed_debugging(),
-                    ## TODO: 'suffix': "-"
+        ntf_args = {"prefix": prefix,
+                    "delete": not debug.detailed_debugging(),
+                    ## TODO: "suffix": "-"
                     }
         self.temp_base = system.getenv_text("TEMP_BASE",
                                             tempfile.NamedTemporaryFile(**ntf_args).name)
         # TODO: self.use_temp_base_dir = gh.dir_exists(gh.basename(self.temp_base))
         # -or-: temp_base_dir = system.getenv_text("TEMP_BASE_DIR", " "); self.use_temp_base_dir = bool(temp_base_dir.strip()); ...
         if use_temp_base_dir is None:
             use_temp_base_dir = system.getenv_bool("USE_TEMP_BASE_DIR", False)
@@ -262,15 +273,14 @@
             debug.trace(4, "FYI: Enabling Perl-style options")
             debug.assertion(not re.search(r"--\w+", " ".join(runtime_args)),
                             "Shouldn't use Python arguments with PERL_SWITCH_PARSING")
             for i, arg in enumerate(runtime_args):
                 if arg in ["-", "--"]:
                     break
                 if my_re.search(r"^-([a-z0-9_]+\w*)=?(.*)$", arg, flags=re.IGNORECASE):
-                    ## OLD: new_arg = "-" + arg
                     option = my_re.group(1)
                     value = (my_re.group(2) if len(my_re.group(2)) else "1")
                     new_arg = f"--{option}={value}"
                     debug.trace(4, f"Converted Perl-style arg {i} from {arg!r} to {new_arg}")
                     debug.assertion(not system.file_exists(arg))
                     runtime_args[i] = new_arg
                     
@@ -289,15 +299,15 @@
         if text_options:
             self.text_options = text_options
         if int_options:
             self.int_options = int_options
         if float_options:
             self.float_options = float_options
         if positional_options or positional_arguments:
-            # TODO: mark positional_options as decprecated
+            # TODO: mark positional_options as deprecated
             debug.assertion(not (positional_options and positional_arguments))
             self.positional_options = positional_options or positional_arguments
         self.multiple_files = multiple_files      # sets other_filenames if multiple w/ nargs=+ 
         # Set defaults
         self.parsed_args = None
         self.filename = None
         self.other_filenames = []
@@ -310,16 +320,20 @@
         debug.trace_fmt(tpo.QUITE_DETAILED, "end of Main.__init__(); self={s}",
                         s=self)
         return
 
     def convert_option(self, option_spec, default_value=None, positional=False):
         """Convert OPTION_SPEC to (label, description, default) tuple. 
         Notes: The description and default of the specification are optional,
-        and the parentheses can be omitted if just the label is given. Also,
-        if POSITIONAL the option prefix (--) is omitted."""
+        and the parentheses can be omitted if just the label is given. For example,
+             ("--num-eggs", "Number of eggs", 2)
+        If POSITIONAL, the option prefix (--) is omitted and the option_SPEC
+        includes an optional nargs component, such as"
+             ("other-files", "Other file names", ["f1", "f2", "f3"], "+")
+        """
         # EX: label, _desc, _default = Main.convert_option("--mucho-backflips"); label => "--mucho-backflips"
         ## TEST: result = ["", "", ""]
         opt_label = None
         opt_desc = None
         opt_default = default_value
         opt_nargs = None
         opt_prefix = "--" if not positional else ""
@@ -328,14 +342,15 @@
             option_components = list(option_spec)
             opt_label = opt_prefix + option_components[0]
             if len(option_components) > 1:
                 opt_desc = option_components[1]
             if len(option_components) > 2:
                 opt_default = option_components[2]
             if len(option_components) > 3:
+                debug.assertion(positional)
                 opt_nargs = option_components[3]
                 debug.assertion(positional)
         else:
             opt_label = opt_prefix + tpo.to_string(option_spec)
         debug.assertion(not " " in opt_label)
         result_list = [opt_label, opt_desc, opt_default]
         if positional:
@@ -345,41 +360,41 @@
                          o=option_spec, d=default_value, p=positional,
                          s=self, r=result)
         return result
 
     def convert_argument(self, argument_spec, default_value=None):
         """Convert ARGUMENT_SPEC to (label, description, default) tuple. 
         Note: This is a wrapper around convert_option for positional arguments."""
-        debug.trace(6, f"convert_option({argument_spec}, {default_value}")
+        debug.trace(6, f"convert_argument({argument_spec}, {default_value}")
         return self.convert_option(argument_spec, default_value, positional=True)
 
     def get_option_name(self, label):
         """Return internal name for parser options (e.g. dashes converted to underscores)"""
         # EX: dummy_app.get_option_name("mucho-backflips") => "mucho_backflips"
         name = label.replace("-", "_")
         tpo.debug_format("get_option_name({l}) => {n}; self={s}", 6,
                          l=label, n=name, s=self)
         return name
 
     def has_parsed_option_old(self, label):
         """Whether option for LABEL specified (i.e., non-null value)
         Note: OLD version that checks for non-null value)
         """
-        # EX: self.parsed_args = {'it': False}; self.has_parsed_option_old('nonit') => False
+        # EX: self.parsed_args = {"it": False}; self.has_parsed_option_old("nonit") => False
         name = self.get_option_name(label)
         has_option = (name in self.parsed_args and (self.parsed_args[name] is not None))
         tpo.debug_format("has_parsed_option_old({l}) => {r}", 6,
                          l=label, r=has_option)
         return has_option
 
     def has_parsed_option(self, label):
         """Value for LABEL specified or None if not applicable
         Note: This is a deprecated method (use get_parsed_option instead)
         """
-        # EX: self.parsed_args = {'it': False}; self.has_parsed_option('notit') => None
+        # EX: self.parsed_args = {"it": False}; self.has_parsed_option("notit") => None
         ## TEMP HACK: if called by a subclass, treate as alias to get_parsed_option
         if (self.__class__ != "__main__.Script"):
             debug.trace(4, "Warning: deprecated method: has_parsed_option => get_parsed_option")
             return self.get_parsed_option(label)
         # Return parsed-arg entry for the option
         name = self.get_option_name(label)
         ## TEMP HACK: has_parsed_option returns args.get(opt)
@@ -395,30 +410,33 @@
         if not self.parsed_args:
             debug.trace(5, "Error: Unexpected condition in get_parsed_option")
             return default
         value = self.parsed_args.get(opt_label)
         # Override null value with default
         if value is None:
             value = default
+            under_label = label.replace("-", "_")
             # Do sanity check for positional argument being checked by mistake
             # TODO: do automatic correction?
             if opt_label != label:
-                if positional:
-                    debug.assertion(opt_label not in self.parsed_args)
-                else:
-                    debug.assertion(label not in self.parsed_args)
+                debug.assertion(label not in self.parsed_args)
+            elif under_label != label:
+                debug.assertion(under_label not in self.parsed_args,
+                                "potential option/argument mismatch")
+            debug.trace_expr(6, label, opt_label, under_label)
         # Return result, after tracing invocation
         tpo.debug_format("get_parsed_option({l}, [{d}], [{p}]) => {v}", 5,
                          l=label, d=default, p=positional, v=value)
         return value
 
     def get_parsed_argument(self, label, default=None):
         """Get value for positional argument LABEL using DEFAULT value"""
         tpo.debug_format("get_parsed_agument({l}, [{d}])", 6,
                          l=label, d=default)
+        ## TODO2: debug.assertion(label in ((l[0] if isinstance(l, list) else l)) for l in self.positional_options)
         return self.get_parsed_option(label, default, positional=True)
 
     def check_arguments(self, runtime_args):
         """Check command-line arguments
         Note: This uses argparse, which might exit the process
         """
         # Note: Shows env. options when debugging as these are backdoor settings.
@@ -434,62 +452,74 @@
                 env_opts = system.formatted_environment_option_descriptions(sort=True, indent=INDENT)
                 env_opt_spec = f"- Available env. options:\n{INDENT}{env_opts}"
             elided_path = re.sub(r"^.*/", ".../", sys.argv[0])
             # note: A dash ("-") is used to indicate stdin with filename arg or to bypass usage w/o one
             # TODO1: get dash put in usage to make more explicit, such as in following:
             #     usage: main.py [-h] [--verbose] [filename] [-]
             usage_notes = ("Notes: \n"
-                           + ("- Use - for filename to skip usage (i.e., a la stdin).\n" if (not self.skip_input) else "")
+                           + ("- Use - for filename to skip usage (i.e., a la stdin).\n" if (not self.skip_input)
+                              else "- Use - to skip usage if no arguments needed.\n" if self.auto_help else "")
                            + ("- Use --non-... for any boolean arg\n" if NEGATIVE_BOOL_ARGS else "")
                            + (f"- Use \"ENV1='v1' ENV2='v2' python {elided_path} ...\" for environment options.\n")
                            + env_opt_spec)
         parser = self.argument_parser(description=self.description,
                                       epilog=usage_notes, prog=self.program,
                                       formatter_class=argparse.RawDescriptionHelpFormatter)
         # TODO: use capitalized script description but lowercase argument help
 
+        def add_argument(opt_label, add_short=None, **kwargs):   # pylint: disable=redefined-builtin
+            """Wrapper around argparse.ArgumentParser.add_argument
+            Note: adds short options string if ADD_SHORT (see self.short_options)"""
+            debug.trace(6, f"add_argument{(opt_label, add_short, kwargs)}")
+            if add_short is None:
+                add_short = self.short_options
+            if self.short_options and my_re.search(r"-(-[a-z])[a-z]+", opt_label):
+                short_label = my_re.group(1)
+                parser.add_argument(short_label, opt_label, **kwargs)
+            else:
+                parser.add_argument(opt_label, **kwargs)
+    
         # Check for options of specific types
         # TODO: consolidate processing for the groups; add option for environment-based default; resolve stupid pylint false positive about unbalanced-tuple-unpacking
         for opt_spec in self.boolean_options:
             (opt_label, opt_desc, opt_default) = self.convert_option(opt_spec, None)    # pylint: disable=unbalanced-tuple-unpacking
             if self.perl_switch_parsing:
                 # note: With Perl argument support, booleans treated as integers due to argparse quirk.
-                ## TEST: parser.add_argument(opt_label, type=int, nargs='?', default=opt_default, help=opt_desc)
+                ## TEST: parser.add_argument(opt_label, type=int, nargs="?", default=opt_default, help=opt_desc)
                 numeric_default = 1 if opt_default else 0
-                parser.add_argument(opt_label, type=int, default=numeric_default, help=opt_desc)
+                add_argument(opt_label, type=int, default=numeric_default, help=opt_desc)
             else:
-                parser.add_argument(opt_label, default=opt_default, action='store_true', help=opt_desc)
+                add_argument(opt_label, default=opt_default, action="store_true", help=opt_desc)
                 if NEGATIVE_BOOL_ARGS:
                     # BAD: label = f"non-{opt_label}"
                     under_label = my_re.sub(r"^__", "", opt_label.replace("-", "_"))
                     label = "--non-" + under_label
                     ## SO-SO
                     ## # note: converts "Description ..." into "Do not description ..."
                     ## opt_desc_uncapitalized = ((opt_desc[:1].lower() + opt_desc[1:]) if opt_desc else "")
                     ## desc = f"Non {opt_desc_uncapitalized}"
                     # note: the argument is not shown in help to avoid clutter
                     desc = argparse.SUPPRESS
                     debug.trace(4, f"Adding negative-boolean: label={label} dest={under_label}")
-                    parser.add_argument(label, default=opt_default, dest=under_label, action='store_false', help=desc)
+                    parser.add_argument(label, default=opt_default, dest=under_label, action="store_false", help=desc, add_short=False)
         for opt_spec in self.int_options:
             (opt_label, opt_desc, opt_default) = self.convert_option(opt_spec, None)    # pylint: disable=unbalanced-tuple-unpacking
-            parser.add_argument(opt_label, type=int, default=opt_default, help=opt_desc)
+            add_argument(opt_label, type=int, default=opt_default, help=opt_desc)
         for opt_spec in self.float_options:
             (opt_label, opt_desc, opt_default) = self.convert_option(opt_spec, None)    # pylint: disable=unbalanced-tuple-unpacking
-            parser.add_argument(opt_label, type=float, default=opt_default,
-                                help=opt_desc)
+            add_argument(opt_label, type=float, default=opt_default, help=opt_desc)
         for opt_spec in self.text_options:
             (opt_label, opt_desc, opt_default) = self.convert_option(opt_spec, None)    # pylint: disable=unbalanced-tuple-unpacking
-            parser.add_argument(opt_label, default=opt_default, help=opt_desc)
+            add_argument(opt_label, default=opt_default, help=opt_desc)
 
         # Add dummy arguments
         # Note: These are used as reminders on how to flesh out the initialization
         if tpo.detailed_debugging():
             if not self.boolean_options:
-                parser.add_argument("--TODO-bool-arg", default=False, action='store_true',
+                parser.add_argument("--TODO-bool-arg", default=False, action="store_true",
                                     help="Add via boolean_options keyword")
             if not self.text_options:
                 parser.add_argument("--TODO-text-arg", default="",
                                     help="Add via text_options keyword")
             if not self.int_options:
                 parser.add_argument("--TODO-int-arg", type=int, default=0,
                                     help="Add via int_options keyword")
@@ -507,18 +537,33 @@
             # TODO: add default to opt_desc if not mentioned
             parser.add_argument(opt_label, default=opt_default, nargs=nargs, 
                                 help=opt_desc)
 
         # Add filename last and make optional with "-" default (i.e., for stdin)
         # Note: with nargs=+, the result is a list of filenames (even if one file [WTH?]!)
         if not self.skip_input:
-            filename_nargs = ('?' if (not self.multiple_files) else "+")
+            filename_nargs = ("?" if (not self.multiple_files) else "+")
             tpo.debug_format("filename_nargs={nargs}", 6, nargs=filename_nargs)
-            parser.add_argument("filename", nargs=filename_nargs, default='-',
+            parser.add_argument("filename", nargs=filename_nargs, default="-",
                                 help="Input filename")
+        elif self.auto_help:
+            dash_nargs = "?"
+            debug.trace_expr(6, dash_nargs)
+            ## TAKE1:
+            ## TODO2: hide [dash] from usage (maldito argparse)
+            ## parser.add_argument("dash", nargs=dash_nargs, default="-",
+            ##                     help="Use - to bypass usage statement")
+            parser.add_argument("-", dest="_", help=argparse.SUPPRESS,
+                                default="-", action="store_true")
+            ## TODO3
+            ## parser.add_argument("--", dest="_", help=argparse.SUPPRESS,
+            ##                     default="-", action="store_true")
+            ## NOTE: currently leads to "error: unrecognized arguments: --" unlike when - used
+        else:
+            debug.trace(6, "Not adding filename nor dash argument")
 
         # Optionally, show brief usage and exit
         # note: print_usage just prints command line synopsis (not individual descriptions)
         if (self.brief_usage and (runtime_args == [USAGE_ARG])):
             debug.trace(4, "Just showing (brief) usage and then exiting")
             debug.trace(5, "warning: self.setup won't be invoked")
             parser.print_usage()
@@ -531,15 +576,15 @@
         self.parsed_args = vars(parser.parse_args(runtime_args))
         debug.trace(5, f"parsed_args = {self.parsed_args}")
         self.verbose = self.get_parsed_option("verbose")
 
         # Get filename unless input ignored and fixup if returned as list
         # TODO: add an option to retain self.filename as is
         if not self.skip_input:
-            self.filename = self.parsed_args['filename']
+            self.filename = self.parsed_args["filename"]
             if (isinstance(self.filename, list)):
                 if not self.multiple_files:
                     debug.trace(3, "Warning: Making (list) self.filename a string & setting self.other_filenames to remainder")
                 file_list = self.filename
                 self.other_filenames = file_list[1:]
                 self.filename = file_list[0] if len(file_list) else "-"
         debug.trace(6, "end Main.check_arguments()")
@@ -617,21 +662,21 @@
                 debug.trace(2, "Processing input")
                 self.process_input()
         except BrokenPipeError:
             ## TODO: exit gracefully (e.g., after wrap_up)
             ## debug.trace_fmt(6, "Silly exception processing input: {exc}", 
             ##                 exc=system.get_exception)
             ##
-            ## exit("Note: you can Ignore any silly BrokenPipeError's thrown by Python!")
+            ## exit("Note: you can Ignore any silly BrokenPipeError"s thrown by Python!")
             ##
             ## pass
             ##
             ## take 3+:
             ## Based on https://stackoverflow.com/questions/26692284/how-to-prevent-brokenpipeerror-when-doing-a-flush-in-python
-            ## sys.stderr.close()                       [doesn't work for Python 3]
+            ## sys.stderr.close()                       [doesn"t work for Python 3]
             ##
             ## take 4 [gotta hate Python!]:
             # Python flushes standard streams on exit; redirect remaining output
             # to devnull to avoid another BrokenPipeError at shutdown
             devnull = os.open(os.devnull, os.O_WRONLY)
             os.dup2(devnull, sys.stdout.fileno())
             sys.exit(1)  # Python exits with error code 1 on EPIPE
@@ -659,15 +704,15 @@
     
     def read_input(self):
         """Generator for producing lines of text from the input (without newlines).
         Notes:
         0. Use read_entire_input for method to return all text at once (i.e., non-generator).
         1. This is called automatically via process_input.
         2. When page mode is in effect, 
-           a. lines don't include form feeds
+           a. lines don"t include form feeds
            b. pages are not buffered: the page number is just tracked.
         3. Paragraph end at empty lines or form feeds (i.e., implicit).
         """
         # TODO: add special page-input mode
         # Note: para_num reset here and updated by process_input
         tpo.debug_format("Main.read_input(): {input}", 5,
                          input=self.input_stream)
@@ -829,13 +874,13 @@
 
 dummy_app = Main([])
 
 debug.trace_current_context(8, "main.py context")
 
 #------------------------------------------------------------------------
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     system.print_stderr(f"Warning: {__file__} is not intended to be run standalone\n")
     # note: Follwing used for argument parsing
     main = Main(description=__doc__)
     main.run()
```

### Comparing `mezcla-1.3.7.post1/mezcla/merge_files.py` & `mezcla-1.3.8/mezcla/merge_files.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/merge_notes.py` & `mezcla-1.3.8/mezcla/merge_notes.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/misc_utils.py` & `mezcla-1.3.8/mezcla/misc_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/my_regex.py` & `mezcla-1.3.8/mezcla/my_regex.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/ngram_tfidf.py` & `mezcla-1.3.8/mezcla/ngram_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/os_utils.py` & `mezcla-1.3.8/mezcla/os_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/pandas_sklearn.py` & `mezcla-1.3.8/mezcla/pandas_sklearn.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/plot_utils.py` & `mezcla-1.3.8/mezcla/plot_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/randomize_lines.py` & `mezcla-1.3.8/mezcla/randomize_lines.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/rgb_color_name.py` & `mezcla-1.3.8/mezcla/rgb_color_name.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,56 +32,64 @@
 #................................................................................
 # TODO:
 # - Add example usage with extcolors:
 #   extcolors self.filename | self.program -
 # - Add option to invoke extcolors automatically.
 #
 
-"""Convert RGB tuples into color names"""
+"""Convert RGB tuples into color names
+
+Sample usage:
+   extcolors tests/resources/orange-gradient.png | {script} -
+"""
 
 # Standard packages
 import re
 
 # Installed packages
 import webcolors
 from scipy.spatial import KDTree
 
 # Local packages
 from mezcla import debug
+from mezcla import glue_helpers as gh
 from mezcla.main import Main
 from mezcla import system
 from mezcla.my_regex import my_re
 
 # Constants for switches omitting leading dashes (e.g., DEBUG_MODE = "debug-mode")
 
 ## TODO: REPLACEMENT = "regex-replacement"
 RGB_REGEX = "rgb-regex"
 HEX = "hex"
 SKIP_DIRECT = "skip-direct"
+SHOW_HEX = "show-hex"
 
 class Script(Main):
     """Input processing class: convert RGB tuples to <RGB, label> pairs"""
     rgb_regex = r"\((0?x?[0-9A-F]+), (0?x?[0-9A-F]+), (0?x?[0-9A-F]+)\)"
     ## TODO: replacement = r"<COLOR, \1>"
     space_color_db = None
     color_names = []
     hex = False
     skip_direct = False
+    show_hex = False
     check_direct_match = None
 
     def setup(self):
         """Check results of command line processing"""
         debug.trace_fmtd(5, "Script.setup(): self={s}", s=self)
         # Extract argument values
         ## TODO: self.REPLACEMENT = self.get_parsed_option(REPLACEMENT, self.REPLACEMENT)
         self.rgb_regex = self.get_parsed_option(RGB_REGEX, self.rgb_regex)
         spec_regex = r"\([^\(\)]+\).*" * 3
         debug.assertion(re.search(spec_regex, self.rgb_regex, re.IGNORECASE))
         self.hex = self.get_parsed_option(HEX, self.hex)
         self.skip_direct = self.get_parsed_option(SKIP_DIRECT, self.skip_direct)
+        self.show_hex = self.get_parsed_option(SHOW_HEX, self.show_hex)
         self.check_direct_match = not self.skip_direct
 
         # Populate color names into spatial name database
         hexnames = webcolors.CSS3_HEX_TO_NAMES
         self.color_names = []
         color_positions = []
         #
@@ -140,38 +148,46 @@
                     debug.trace_fmtd(5, f"{rgb} => {index}; dist={dist}")
                     color_name = self.color_names[index]
             except:
                 system.print_stderr(f"Exception in color decoding: {system.get_exception()}")
                 continue
 
             rgb_spec = rgb
-            color_spec = f"<{rgb_spec}, {color_name}>"
+            hex_spec = ""
+            if self.show_hex:
+                # https://stackoverflow.com/questions/2269827/how-to-convert-an-int-to-a-hex-string
+                hex_spec = " 0x" + "".join(f"{c:0>2X}" for c in query_color)
+            color_spec = f"<{rgb_spec}, {color_name}{hex_spec}>"
             processed_text += text[0: my_re.start()] + color_spec
             text = text[my_re.end():]
             debug.trace_fmtd(4, "match: {m}; new text: {new}",
                              m=my_re.group(0), new=text)
         debug.assertion(num_tries <= MAX_TRIES)
 
         # Print revised line
         print(processed_text + text)
 
-#-------------------------------------------------------------------------------
-
-if __name__ == '__main__':
-    debug.trace_current_context(level=debug.QUITE_DETAILED)
+def main():
+    """Entry point"""
     app = Script(
-        description=__doc__,
+        description=__doc__.format(script=gh.basename(__file__)),
         usage_notes="Note: Input is not an image (e.g., use extcolors)",
         # Note: skip_input controls the line-by-line processing, which is inefficient but simple to
         # understand; in contrast, manual_input controls iterator-based input (the opposite of both).
-        skip_input=False,
-        manual_input=False,
         boolean_options=[(HEX, "RGB triple specified in hex (not decimal)"),
+                         (SHOW_HEX, "Show hex-style specification XXXXXX"),
                          (SKIP_DIRECT, "Don't include direct match (for nearest neighbor test")],
         # Note: FILENAME is default argument unless skip_input
         text_options=[
             ## TODO: (REPLACEMENT, "Regex-like replacement using \\1 for RGB tuple and COLOR for color name"),
             (RGB_REGEX, "Regex for finding RGB color specifications with \\1, \\2, and \\3 for reg, green, and blue")
         ],
         # Note: Following added for indentation: float options are not common
         float_options=None)
     app.run()
+    
+        
+#-------------------------------------------------------------------------------
+
+if __name__ == '__main__':
+    debug.trace_current_context(level=debug.QUITE_DETAILED)
+    main()
```

### Comparing `mezcla-1.3.7.post1/mezcla/run_albert_classifier.py` & `mezcla-1.3.8/mezcla/run_albert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/run_bert_classifier.py` & `mezcla-1.3.8/mezcla/run_bert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/show_bert_representation.py` & `mezcla-1.3.8/mezcla/show_bert_representation.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/simple_main_example.py` & `mezcla-1.3.8/mezcla/simple_main_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/spacy_nlp.py` & `mezcla-1.3.8/mezcla/spacy_nlp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/spell.py` & `mezcla-1.3.8/mezcla/spell.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/sys_version_info_hack.py` & `mezcla-1.3.8/mezcla/sys_version_info_hack.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/system.py` & `mezcla-1.3.8/mezcla/system.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,14 +75,16 @@
     env_defaults[var] = default
     return
 
 
 def get_registered_env_options():
     """Returns list of environment options registered via register_env_option"""
     ## OLD: option_names = [k for k in env_options if (env_options[k] and env_options[k].strip())]
+    ## TEMP
+    # pylint: disable=consider-using-dict-items
     option_names = [k for k in env_options if (env_options[k] is not None)]
     debug.trace_fmt(5, "get_registered_env_options() => {on}", on=option_names)
     return option_names
 
 
 def get_environment_option_descriptions(include_all=None, include_default=None, indent=" "):
     """
@@ -117,14 +119,16 @@
             # Note: add quotes to distinguish "None" from None (i.e., str vs. NoneType)
             default_spec = (("(%r)" % default_value) if has_default else "(None)")
         default_spec = default_spec.replace("\n", "\\n")
         result = (opt, desc_spec + indent + default_spec)
         debug.trace_fmt(9, "_format_env_option() => {r}", r=result)
         return result
     #
+    ## TEMP
+    # pylint: disable=consider-using-dict-items
     option_descriptions = [_format_env_option(opt) for opt in env_options if (env_options[opt] or include_all)]
     debug.trace_fmt(5, "get_environment_option_descriptions() => {od}",
                     od=option_descriptions)
     return option_descriptions
 
 
 def formatted_environment_option_descriptions(sort=False, include_all=None, indent="\t"):
@@ -686,25 +690,29 @@
     key = entry if retain_case else entry.lower()
     result = hash_table[key]
     debug.trace_fmt(6, "lookup_entry(_, {e}, [case={rc}) => {r}",
                     e=entry, rc=retain_case, r=result)
     return result
 
                 
-def write_file(filename, text, skip_newline=False, append=False):
+def write_file(filename, text, skip_newline=False, append=False, binary=False):
     """Create FILENAME with TEXT and optionally for APPEND.
-    Note: A newline is added at the end if missing unless SKIP_NEWLINE"""
+    Note: A newline is added at the end if missing unless SKIP_NEWLINE.
+    A binary file is created if BINARY (n.b., incompatible with APPEND).
+    """
     debug.trace_fmt(7, "write_file({f}, {t})", f=filename, t=text)
     # EX: f = "/tmp/_it.list"; write_file(f, "it"); read_file(f) => "it\n"
     # EX: write_file(f, "it", skip_newline=True); read_file(f) => "it"
     debug.assertion(isinstance(text, str))
     try:
         if not isinstance(text, STRING_TYPES):
             text = to_string(text)
-        mode = 'a' if append else 'w'
+        ## OLD: mode = 'a' if append else 'w'
+        debug.assertion(not binary and append)
+        mode = "wb" if binary else "a" if append else "w"
         with open(filename, encoding="UTF-8", mode=mode) as f:
             f.write(to_utf8(text))
             if not text.endswith("\n"):
                 if not skip_newline:
                     f.write("\n")
     except (IOError, ValueError):
         debug.trace_fmtd(1, "Error: Problem writing file '{f}': {exc}",
```

### Comparing `mezcla-1.3.7.post1/mezcla/temp/simple_batspp.py` & `mezcla-1.3.8/mezcla/temp/simple_batspp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/template.py` & `mezcla-1.3.8/mezcla/template.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/LICENSE.txt` & `mezcla-1.3.8/mezcla/tests/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/adhoc-tests.batspp` & `mezcla-1.3.8/mezcla/tests/adhoc-tests.batspp`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/misc_doctests.py` & `mezcla-1.3.8/mezcla/tests/misc_doctests.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/resources/cars-csv-len-3.txt` & `mezcla-1.3.8/mezcla/tests/resources/cars-csv-len-3.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/resources/cars-tsv-len-3.txt` & `mezcla-1.3.8/mezcla/tests/resources/cars-tsv-len-3.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/resources/cars.csv` & `mezcla-1.3.8/mezcla/tests/resources/cars.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/resources/cars.tsv` & `mezcla-1.3.8/mezcla/tests/resources/cars.tsv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/resources/example_text.txt` & `mezcla-1.3.8/mezcla/tests/resources/example_text.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/resources/example_text_tags.txt` & `mezcla-1.3.8/mezcla/tests/resources/example_text_tags.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/resources/iris_output.txt` & `mezcla-1.3.8/mezcla/tests/resources/iris_output.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/resources/simple-window-dimensions.html` & `mezcla-1.3.8/mezcla/tests/resources/simple-window-dimensions.html`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/resources/spanish-accents.docx` & `mezcla-1.3.8/mezcla/tests/resources/spanish-accents.docx`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/resources/spanish-accents.pdf` & `mezcla-1.3.8/mezcla/tests/resources/spanish-accents.pdf`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/template.py` & `mezcla-1.3.8/mezcla/tests/template.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,48 +11,48 @@
 # - This can be run as follows:
 #   $ PYTHONPATH=".:$PYTHONPATH" python ./mezcla/tests/test_<module>.py
 #
 
 """TODO: Tests for <module> module"""
 
 # Standard packages
-import re
+## TODO: from collections import defaultdict
 
 # Installed packages
 import pytest
 
 # Local packages
 from mezcla.unittest_wrapper import TestWrapper
 from mezcla import debug
-## TODO: from mezcla import system
+from mezcla.my_regex import my_re
 from mezcla import glue_helpers as gh
 
 # Note: Two references are used for the module to be tested:
 #    THE_MODULE:                  global module object
 #    TestTemplate.script_module:  path to file
-## TODO: change template to new name
+## TODO (vvv): change template to new name; *** use commented out template below ***
 THE_MODULE = None           ## TODO: remove this line (n.b., used just to avoid syntax problems with <module> in following)
-## TODO: import mezcla.<module> as THE_MODULE
+## TODO (^^^): import mezcla.<module> as THE_MODULE
 #
 # Note: sanity test for customization (TODO: remove if desired)
-if not re.search(__file__, r"\btemplate.py$"):
+if not my_re.search(__file__, r"\btemplate.py$"):
     debug.assertion("mezcla.template" not in str(THE_MODULE))
 
 ## TODO:
 ## # Environment options
 ## # Note: These are just intended for internal options, not for end users.
 ## # It also allows for enabling options in one place.
 ## #
 ## FUBAR = system.getenv_bool("FUBAR", False,
 ##                            description="Fouled Up Beyond All Recognition processing")
 
 
 class TestIt(TestWrapper):
     """Class for testcase definition"""
-    script_module = TestWrapper.get_testing_module_name(__file__)
+    script_module = TestWrapper.get_testing_module_name(__file__, THE_MODULE)
     # -or- non-mezcla: script_module = TestWrapper.get_testing_module_name(__file__, THE_MODULE)
     #
     # TODO: use_temp_base_dir = True            # treat TEMP_BASE as directory
     # note: temp_file defined by parent (along with script_module, temp_base, and test_num)
 
     ## TODO: optional setup methods
     ##
@@ -76,25 +76,25 @@
 
     @pytest.mark.xfail                   # TODO: remove xfail
     def test_data_file(self):
         """Makes sure TODO works as expected"""
         debug.trace(4, f"TestIt.test_data_file(); self={self}")
         data = ["TODO1", "TODO2"]
         gh.write_lines(self.temp_file, data)
-        output = self.run_script("", self.temp_file)
-        assert(re.search(r"TODO-pattern", 
-                         output.strip()))
+        ## TODO: add use_stdin=True to following if no file argument
+        output = self.run_script(options="", data_file=self.temp_file)
+        assert my_re.search(r"TODO-pattern", output.strip())
         return
 
     @pytest.mark.xfail                   # TODO: remove xfail
     def test_something_else(self):
         """TODO: flesh out test for something else"""
         debug.trace(4, f"TestIt.test_something_else(); self={self}")
         self.fail("TODO: code test")
-        ## ex: assert(THE_MODULE.TODO_function() == TODO_value)
+        ## ex: assert (THE_MODULE.TODO_function() == TODO_value)
         return
 
 
     ## TODO: optional cleanup methods
     ##
     ## def tearDown(self):
     ##     debug.trace(6, f"TestIt.tearDown(); self={self}")
@@ -111,15 +111,21 @@
 
 ## TODO:
 ## #...............................................................................
 ##
 ## class TestIt2:
 ##     """Another class for testcase definition
 ##     Note: Needed to avoid error with pytest due to inheritance with unittest.TestCase via TestWrapper"""
-##     pass
+##
+##    def test_whatever(self):
+##        """TODO: flesh out test for whatever"""
+##        debug.trace(4, f"TestIt2.test_whatever(); self={self}")
+##        assert False, "TODO: code test"
+##        ## ex: assert THE_MODULE.fast_sort() == THE_MODULE.slow_sort()
+##        return
 ##
 
 #------------------------------------------------------------------------
 
 if __name__ == '__main__':
     debug.trace_current_context()
     pytest.main([__file__])
```

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test___init__.py` & `mezcla-1.3.8/mezcla/tests/test___init__.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_audio.py` & `mezcla-1.3.8/mezcla/tests/test_audio.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_bert_multi_classification.py` & `mezcla-1.3.8/mezcla/tests/test_bert_multi_classification.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_bing_search.py` & `mezcla-1.3.8/mezcla/tests/test_bing_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_compute_tfidf.py` & `mezcla-1.3.8/mezcla/tests/test_compute_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_cut.py` & `mezcla-1.3.8/mezcla/tests/test_cut.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_data_utils.py` & `mezcla-1.3.8/mezcla/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_debug.py` & `mezcla-1.3.8/mezcla/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_extract_document_text.py` & `mezcla-1.3.8/mezcla/tests/test_extract_document_text.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_file_utils.py` & `mezcla-1.3.8/mezcla/tests/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_filter_random.py` & `mezcla-1.3.8/mezcla/tests/test_filter_random.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_gensim_test.py` & `mezcla-1.3.8/mezcla/tests/test_gensim_test.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_glue_helpers.py` & `mezcla-1.3.8/mezcla/tests/test_glue_helpers.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_html_utils.py` & `mezcla-1.3.8/mezcla/tests/test_html_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_kenlm_example.py` & `mezcla-1.3.8/mezcla/tests/test_kenlm_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_keras_param_search.py` & `mezcla-1.3.8/mezcla/tests/test_keras_param_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_main.py` & `mezcla-1.3.8/mezcla/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_merge_files.py` & `mezcla-1.3.8/mezcla/tests/test_merge_files.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_merge_notes.py` & `mezcla-1.3.8/mezcla/tests/test_merge_notes.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_misc_utils.py` & `mezcla-1.3.8/mezcla/tests/test_misc_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_my_regex.py` & `mezcla-1.3.8/mezcla/tests/test_my_regex.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_ngram_tfidf.py` & `mezcla-1.3.8/mezcla/tests/test_ngram_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_os_utils.py` & `mezcla-1.3.8/mezcla/tests/test_os_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_pandas_sklearn.py` & `mezcla-1.3.8/mezcla/tests/test_pandas_sklearn.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_plot_utils.py` & `mezcla-1.3.8/mezcla/tests/test_plot_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_randomize_lines.py` & `mezcla-1.3.8/mezcla/tests/test_randomize_lines.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_rgb_color_name.py` & `mezcla-1.3.8/mezcla/tests/test_rgb_color_name.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_run_albert_classifier.py` & `mezcla-1.3.8/mezcla/tests/test_run_albert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_run_bert_classifier.py` & `mezcla-1.3.8/mezcla/tests/test_run_bert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_show_bert_representation.py` & `mezcla-1.3.8/mezcla/tests/test_show_bert_representation.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_simple_main_example.py` & `mezcla-1.3.8/mezcla/tests/test_simple_main_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_spacy_nlp.py` & `mezcla-1.3.8/mezcla/tests/test_spacy_nlp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_sys_version_info_hack.py` & `mezcla-1.3.8/mezcla/tests/test_sys_version_info_hack.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_system.py` & `mezcla-1.3.8/mezcla/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_template.py` & `mezcla-1.3.8/mezcla/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_text_categorizer.py` & `mezcla-1.3.8/mezcla/tests/test_text_categorizer.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_text_processing.py` & `mezcla-1.3.8/mezcla/tests/test_text_processing.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_text_utils.py` & `mezcla-1.3.8/mezcla/tests/test_text_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_tpo_common.py` & `mezcla-1.3.8/mezcla/tests/test_tpo_common.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_train_language_model.py` & `mezcla-1.3.8/mezcla/tests/test_train_language_model.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_train_text_categorizer.py` & `mezcla-1.3.8/mezcla/tests/test_train_text_categorizer.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_transpose_data.py` & `mezcla-1.3.8/mezcla/tests/test_transpose_data.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/test_xml_utils.py` & `mezcla-1.3.8/mezcla/tests/test_xml_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/tfidf/test_corpus.py` & `mezcla-1.3.8/mezcla/tests/tfidf/test_corpus.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/tfidf/test_dockeyword.py` & `mezcla-1.3.8/mezcla/tests/tfidf/test_dockeyword.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/tfidf/test_document.py` & `mezcla-1.3.8/mezcla/tests/tfidf/test_document.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tests/tfidf/test_preprocess.py` & `mezcla-1.3.8/mezcla/tests/tfidf/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/text_categorizer.py` & `mezcla-1.3.8/mezcla/text_categorizer.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/text_processing.py` & `mezcla-1.3.8/mezcla/text_processing.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/text_utils.py` & `mezcla-1.3.8/mezcla/text_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tfidf/corpus.py` & `mezcla-1.3.8/mezcla/tfidf/corpus.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tfidf/dockeyword.py` & `mezcla-1.3.8/mezcla/tfidf/dockeyword.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tfidf/document.py` & `mezcla-1.3.8/mezcla/tfidf/document.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tfidf/preprocess.py` & `mezcla-1.3.8/mezcla/tfidf/preprocess.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/tpo_common.py` & `mezcla-1.3.8/mezcla/tpo_common.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/train_language_model.py` & `mezcla-1.3.8/mezcla/train_language_model.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/train_text_categorizer.py` & `mezcla-1.3.8/mezcla/train_text_categorizer.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/transpose_data.py` & `mezcla-1.3.8/mezcla/transpose_data.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/mezcla/unittest_wrapper.py` & `mezcla-1.3.8/mezcla/unittest_wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,50 +38,56 @@
 # TODO:
 # - Add method to invoke unittest.main(), so clients don't need to import unittest.
 # - Clarify how ALLOW_SUBCOMMAND_TRACING affects tests that invoke external scripts.
 #
 
 """Unit test support class"""
 
+# Standard modules
+
 import os
 import re
 import tempfile
 import unittest
 
+# Installed modules
+## TODO: import pytest
+
+# Local modules
+
 import mezcla
 from mezcla import debug
 from mezcla import glue_helpers as gh
 from mezcla import system
-from mezcla import tpo_common as tpo
 
+# Constants (e.g., environment options)
 
-KEEP_TEMP = system.getenv_bool("KEEP_TEMP", tpo.detailed_debugging(),
+TL = debug.TL
+KEEP_TEMP = system.getenv_bool("KEEP_TEMP", debug.detailed_debugging(),
                                "keep temporary files")
 TODO_FILE = "TODO FILE"
 TODO_MODULE = "TODO MODULE"
 
 # Note: the following is for transparent resolution of dotted module names
 # for invocation of scripts via 'python -m package.module'. This is in support
 # of transitioning from the old way of importing packages via 'import module'
 # instead of 'import package.module'. (The former required that package be
 # explicitly specified in the python path, such as via 'PYTHONPATH=package-dir:...'.)
 THIS_PACKAGE = getattr(mezcla.debug, "__package__", None)
 debug.assertion(THIS_PACKAGE == "mezcla")
 
-
 def get_temp_dir(keep=False):
     """Get temporary directory, omitting later deletion if KEEP"""
     if keep is None:
         keep = KEEP_TEMP
     dir_path = tempfile.NamedTemporaryFile(delete=(not keep)).name
     gh.full_mkdir(dir_path)
     debug.trace(5, "get_temp_dir() => {dir_path}")
     return dir_path
 
-
 class TestWrapper(unittest.TestCase):
     """Class for testcase definition"""
     script_file = TODO_FILE             # path for invocation via 'python -m coverage run ...' (n.b., usually set via get_module_file_path)
     script_module = TODO_MODULE         # name for invocation via 'python -m' (n.b., usuually set via derive_tested_module_name)
     temp_base = system.getenv_text("TEMP_BASE",
                                    tempfile.NamedTemporaryFile().name)
     check_coverage = system.getenv_bool("CHECK_COVERAGE", False,
@@ -103,15 +109,15 @@
     ##    debug.trace_object(5, self, label="TestWrapper instance")
     ##
     ## __test__ = False                 # make sure not assumed test
         
     @classmethod
     def setUpClass(cls):
         """Per-class initialization: make sure script_module set properly"""
-        tpo.debug_format("TestWrapper.setupClass(): cls={c}", 5, c=cls)
+        debug.trace_fmtd(5, "TestWrapper.setupClass(): cls={c}", c=cls)
         super(TestWrapper, cls).setUpClass()
         debug.trace_object(5, cls, "TestWrapper class")
         debug.assertion(cls.script_module != TODO_MODULE)
         if cls.script_module:
             # Try to pull up usage via python -m mezcla.xyz --help
             help_usage = gh.run("python -m '{mod}' --help", mod=cls.script_module)
             debug.assertion("No module named" not in help_usage,
@@ -135,42 +141,43 @@
 
         return
 
     @staticmethod
     def derive_tested_module_name(test_filename):
         """Derive the name of the module being tested from TEST_FILENAME. Used as follows:
               script_module = TestWrapper.derive_tested_module_name(__file__)
-        Note: Deprecated method (see get_testing_module_name)
+        Note: *** Deprecated method *** (see get_testing_module_name)
         """
-        tpo.debug_format("Warning: in deprecrated derive_tested_module_name", 5)
+        debug.trace(3, "Warning: in deprecrated derive_tested_module_name")
         module = os.path.split(test_filename)[-1]
         module = re.sub(r".py[oc]?$", "", module)
         module = re.sub(r"^test_", "", module)
-        tpo.debug_format("derive_tested_module_name({f}) => {m}", 5,
+        debug.trace_fmtd(5, "derive_tested_module_name({f}) => {m}",
                          f=test_filename, m=module)
         return (module)
 
     @staticmethod
     def get_testing_module_name(test_filename, module_object=None):
-        """Derive the name of the module being tested from TEST_FILENAME and MODULE_OBJECT"""
-        # TODO: used as follows (see tests/test_template.py):
-        #    script_module = TestWrapper.get_testing_module_name(__file__)
+        """Derive the name of the module being tested from TEST_FILENAME and MODULE_OBJECT
+        Note: used as follows (see tests/test_template.py):
+            script_module = TestWrapper.get_testing_module_name(__file__)
+        """
         module_name = os.path.split(test_filename)[-1]
         module_name = re.sub(r".py[oc]?$", "", module_name)
         module_name = re.sub(r"^test_", "", module_name)
         package_name = THIS_PACKAGE
         if module_object is not None:
            package_name = getattr(module_object, "__package__", "")
            debug.trace_expr(4, package_name)
         if package_name:
             full_module_name = package_name + "." + module_name
         else:
             full_module_name = module_name
-        tpo.debug_format("get_testing_module_name({f}) => {m}", 4,
-                         f=test_filename, m=full_module_name)
+        debug.trace_fmtd(4, "get_testing_module_name({f}, [{mo}]) => {m}",
+                         f=test_filename, m=full_module_name, mo=module_object)
         return (full_module_name)
 
     @staticmethod
     def get_module_file_path(test_filename):
         """Return absolute path of module being tested"""
         result = system.absolute_path(test_filename)
         result = re.sub(r'tests\/test_(.*\.py)', r'\1', result)
@@ -180,50 +187,51 @@
 
     def setUp(self):
         """Per-test initializations
         Notes:
         - Disables tracing scripts invoked via run() unless ALLOW_SUBCOMMAND_TRACING
         - Initializes temp file name (With override from environment)."""
         # Note: By default, each test gets its own temp file.
-        tpo.debug_print("TestWrapper.setUp()", 4)
+        debug.trace(4, "TestWrapper.setUp()")
         if not gh.ALLOW_SUBCOMMAND_TRACING:
             gh.disable_subcommand_tracing()
         # The temp file is an extension of temp-base file by default.
         # Opitonally, if can be a file in temp-base subdrectory.
         if self.use_temp_base_dir:
             default_temp_file = gh.form_path(self.temp_base, "test-")
         else:
             default_temp_file = self.temp_base + "-test-"
         default_temp_file += str(TestWrapper.test_num)
         self.temp_file = system.getenv_text("TEMP_FILE", default_temp_file)
         gh.delete_existing_file(self.temp_file)
         TestWrapper.test_num += 1
 
-        ## OLD: tpo.trace_object(self, 5, "TestWrapper instance")
         debug.trace_object(5, self, "TestWrapper instance")
         return
 
     def run_script(self, options=None, data_file=None, log_file=None, trace_level=4,
                    out_file=None, env_options=None, uses_stdin=False):
         """Runs the script over the DATA_FILE (optional), passing (positional)
         OPTIONS and optional setting ENV_OPTIONS. If OUT_FILE and LOG_FILE are
         not specifed, they  are derived from self.temp_file.
         Notes:
         - issues warning if script invocation leads to error
         - if USES_STDIN, requires explicit empty string for DATA_FILE to avoid use of - (n.b., as a precaution against hangups)"""
-        tpo.debug_format("TestWrapper.run_script({opts}, {df}, {lf}, {of}, {env})", trace_level + 1,
+        debug.trace_fmtd(trace_level + 1,
+                         "TestWrapper.run_script({env}, {opts}, {df}, {lf}, {of}",
                          opts=options, df=data_file, lf=log_file, 
                          of=out_file, env=env_options)
         if options is None:
             options = ""
         if env_options is None:
             env_options = ""
 
         # Derive the full paths for data file and log, and then invoke script.
         # TODO: derive from temp base and data file name?;
+        # TODO1: derive default for uses_stdin based use of filename argment (e.g., from usage)
         data_path = ("" if uses_stdin else "-")
         if data_file is not None:
             data_path = (gh.resolve_path(data_file) if len(data_file) else data_file)
         if not log_file:
             log_file = self.temp_file + ".log"
         if not out_file:
             out_file = self.temp_file + ".out"
@@ -241,44 +249,50 @@
         gh.issue("{env} python -m {cov_spec} {module}  {opts}  {path} 1> {out} 2> {log}",
                  env=env_options, cov_spec=coverage_spec, module=self.script_module,
                  opts=options, path=data_path, out=out_file, log=log_file)
         output = gh.read_file(out_file)
         # note; trailing newline removed as with shell output
         if output.endswith("\n"):
             output = output[:-1]
-        tpo.debug_format("output: {{\n{out}\n}}", trace_level,
+        debug.trace_fmtd(trace_level, "output: {{\n{out}\n}}",
                          out=gh.indent_lines(output))
 
         # Make sure no python or bash errors. For example,
         #   "SyntaxError: invalid syntax" and "bash: python: command not found"
         log_contents = gh.read_file(log_file)
         error_found = re.search(r"(\S+error:)|(no module)|(command not found)",
                                 log_contents.lower())
         gh.assertion(not error_found)
-        tpo.debug_format("log contents: {{\n{log}\n}}", trace_level + 1,
-                         log=gh.indent_lines(log_contents))
+        debug.trace_fmt(trace_level + 1, "log contents: {{\n{log}\n}}",
+                        log=gh.indent_lines(log_contents))
 
         # Do sanity check for python exceptions
         traceback_found = re.search("Traceback.*most recent call", log_contents)
         gh.assertion(not traceback_found)
 
         return output
 
     def tearDown(self):
         """Per-test cleanup: deletes temp file unless detailed debugging"""
-        tpo.debug_print("TestWrapper.tearDown()", 4)
+        debug.trace(4, "TestWrapper.tearDown()")
         if not KEEP_TEMP:
             gh.run("rm -vf {file}*", file=self.temp_file)
         return
 
     @classmethod
     def tearDownClass(cls):
         """Per-class cleanup: stub for tracing purposes"""
-        tpo.debug_format("TestWrapper.tearDownClass(); cls={c}", 5, c=cls)
+        debug.trace_fmtd(5, "TestWrapper.tearDownClass(); cls={c}", c=cls)
         if not KEEP_TEMP:
             ## TODO: use shutil
             if cls.use_temp_base_dir:
                 gh.run("rm -rvf {dir}", dir=cls.temp_base)
             else:
                 gh.run("rm -vf {base}*", base=cls.temp_base)
         super(TestWrapper, cls).tearDownClass()
         return
+    
+#-------------------------------------------------------------------------------
+    
+if __name__ == '__main__':
+    debug.trace_current_context(level=TL.QUITE_DETAILED)
+    debug.trace(TL.USUAL, "Warning: not intended for command-line use\n")
```

### Comparing `mezcla-1.3.7.post1/mezcla/xml_utils.py` & `mezcla-1.3.8/mezcla/xml_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/pyproject.toml` & `mezcla-1.3.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/requirements.txt` & `mezcla-1.3.8/requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -45,15 +45,16 @@
 ibm_cloud_sdk_core==3.15.3
 pysbd==0.3.4
 scikit-learn==1.1.2
 scispacy==0.5.0
 stop_words==2018.7.23
 tensorflow_hub==0.12.0
 vaderSentiment==3.3.2
-extcolors==1.0.0
+## OLD: extcolors==1.0.0
+extcolors>=1.0.0
 #
 #...............................................................................
 # Optional requirements
 #
 ## TODO:
 # - download Spacy model(s):
 #   python -m spacy download en_core_web_lg
@@ -92,7 +93,12 @@
 #opt# coverage
 #opt# ipython
 #opt# pylint
 #opt# gradio
 #full# sentencepiece
 #full# sacremoses
 #opt# transformers
+#opt# torch
+#opt# accelerate
+#opt# datasets
+#opt# diffusers
+#opt# flask
```

### Comparing `mezcla-1.3.7.post1/setup.py` & `mezcla-1.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 """Simple installer"""
 
 from distutils.core import setup
 
 setup(name='Mezcla',
       packages=['mezcla'],
       module="mezcla",
-      version='1.3.7.post1',
+      version='1.3.8',
       description-file="README.txt",
       dist-name="Mezcla",
       ## OLD: py_modules=PYTHON_MODULE_NAMES,
       author="Tom O'Hara",
       # TODO: find out which email key is preferred
       email="tomasohara@gmail.com",
       author-email="tomasohara@gmail.com"
```

### Comparing `mezcla-1.3.7.post1/temp/simple_batspp.py` & `mezcla-1.3.8/temp/simple_batspp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/tools/run_tests.bash` & `mezcla-1.3.8/tools/run_tests.bash`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/tox.ini` & `mezcla-1.3.8/tox.ini`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.7.post1/PKG-INFO` & `mezcla-1.3.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mezcla
-Version: 1.3.7.post1
+Version: 1.3.8
 Summary: Mezcla is Spanish for mixture, and this repository contains a variety of Python scripts.
 Home-page: https://github.com/tomasohara/mezcla
 License: LGPLv3
 Author: Tomás O'Hara
 Author-email: tomasohara@gmail.com
 Description-Content-Type: text/plain
```

