# Comparing `tmp/ligo-followup-advocate-1.2.3.tar.gz` & `tmp/ligo-followup-advocate-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ligo-followup-advocate-1.2.3.tar", last modified: Wed May 24 17:47:56 2023, max compression
+gzip compressed data, was "ligo-followup-advocate-1.2.4.tar", last modified: Tue Jun 20 23:10:47 2023, max compression
```

## Comparing `ligo-followup-advocate-1.2.3.tar` & `ligo-followup-advocate-1.2.4.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.911851 ligo-followup-advocate-1.2.3/
--rw-rw-rw-   0 root         (0) root         (0)    17895 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/COPYING.md
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      880 2023-05-24 17:47:56.912850 ligo-followup-advocate-1.2.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2855 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.779846 ligo-followup-advocate-1.2.3/ligo/
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.914851 ligo-followup-advocate-1.2.3/ligo/followup_advocate/
--rw-rw-rw-   0 root         (0) root         (0)    24955 2023-05-23 23:25:10.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-05-24 17:47:56.914851 ligo-followup-advocate-1.2.3/ligo/followup_advocate/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     1244 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/jinja.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.788847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2973 2023-05-23 23:25:10.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/RAVEN_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      944 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/RAVEN_subject.jinja2
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 17:47:46.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/authors.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      376 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/compare_skymaps.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1032 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/em_bright.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     2699 2023-05-23 23:25:10.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/initial_body.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      425 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/initial_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1581 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/llama_alert_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      436 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/llama_subject.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     2303 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/llama_track_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     9888 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/macros.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      567 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/medium_latency_grb_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1786 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/medium_latency_grb_detection_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1504 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/medium_latency_grb_exclusion_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      344 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/medium_latency_grb_subject.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/numbered_pipeline_citations.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      461 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/p_astro.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      419 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/retraction.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1122 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/skymap_info.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      310 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/subject.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1350 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/update_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      223 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/userguide_conclusion.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.788847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 17:47:46.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.777846 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.789847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1122/
--rw-rw-rw-   0 root         (0) root         (0)     1880 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1122/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.790847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1122/files/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1122/files/distances_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1122/files/distances_x.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1122/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1122/files/false_alarm_probability_x.json
--rw-rw-rw-   0 root         (0) root         (0)      987 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1122/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.791847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1133/
--rw-rw-rw-   0 root         (0) root         (0)     1877 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1133/event.json
--rw-rw-rw-   0 root         (0) root         (0)        4 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1133/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.792847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1134/
--rw-rw-rw-   0 root         (0) root         (0)     1904 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1134/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.793847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1134/files/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1134/files/distances_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1134/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)      515 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1134/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.793847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1234/
--rw-rw-rw-   0 root         (0) root         (0)     1881 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1234/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.795847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1234/files/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1234/files/distances_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1234/files/distances_x.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1234/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1234/files/false_alarm_probability_x.json
--rw-rw-rw-   0 root         (0) root         (0)      714 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1234/files/initial.data
--rw-rw-rw-   0 root         (0) root         (0)     1086 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1234/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.795847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1235/
--rw-rw-rw-   0 root         (0) root         (0)     1876 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1235/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.796847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1235/files/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1235/files/distances_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1235/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)      714 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1235/files/initial.data
--rw-rw-rw-   0 root         (0) root         (0)      610 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1235/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.797847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E2244/
--rw-rw-rw-   0 root         (0) root         (0)     1904 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E2244/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.798847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E2244/files/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E2244/files/distances_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E2244/files/distances_x.json
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E2244/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E2244/files/false_alarm_probability_x.json
--rw-rw-rw-   0 root         (0) root         (0)      991 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E2244/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.799847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E5678/
--rw-rw-rw-   0 root         (0) root         (0)     1918 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E5678/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.799847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E5678/files/
--rw-rw-rw-   0 root         (0) root         (0)     5761 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E5678/files/initial.data
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E5678/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.800847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M1122/
--rw-rw-rw-   0 root         (0) root         (0)     1936 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M1122/event.json
--rw-rw-rw-   0 root         (0) root         (0)      633 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M1122/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.801847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M1234/
--rw-rw-rw-   0 root         (0) root         (0)     3958 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M1234/event.json
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M1234/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.801847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M1235/
--rw-rw-rw-   0 root         (0) root         (0)     3982 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M1235/event.json
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M1235/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.802847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M2468/
--rw-rw-rw-   0 root         (0) root         (0)     3956 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M2468/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.802847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M2468/files/
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M2468/files/p_astro.json
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M2468/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.803847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M2469/
--rw-rw-rw-   0 root         (0) root         (0)     3979 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M2469/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.803847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M2469/files/
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M2469/files/p_astro.json
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M2469/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.805847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M5566/
--rw-rw-rw-   0 root         (0) root         (0)     3958 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M5566/event.json
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M5566/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.805847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M5678/
--rw-rw-rw-   0 root         (0) root         (0)     3955 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M5678/event.json
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M5678/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.806847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M5679/
--rw-rw-rw-   0 root         (0) root         (0)     3979 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M5679/event.json
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M5679/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.807847 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.831848 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files/
--rw-rw-rw-   0 root         (0) root         (0)     4609 2023-05-23 23:25:10.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files/S1234-1-EarlyWarning.xml
--rw-rw-rw-   0 root         (0) root         (0)     4607 2023-05-23 23:25:10.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files/S1234-2-Initial.xml
--rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files/bayestar-ext.fits.gz
--rw-rw-rw-   0 root         (0) root         (0)   777600 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files/bayestar.fits.gz
--rw-rw-rw-   0 root         (0) root         (0)   777600 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files/bayestar.multiorder.fits
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files/coincidence_far.json
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files/em_bright.json
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files/p_astro.json
--rw-rw-rw-   0 root         (0) root         (0)     1832 2023-05-23 23:25:10.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files.json
--rw-rw-rw-   0 root         (0) root         (0)     7997 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/logs.json
--rw-rw-rw-   0 root         (0) root         (0)     5897 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/superevent.json
--rw-rw-rw-   0 root         (0) root         (0)     1612 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/voevents.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.833848 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S2468/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.840848 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S2468/files/
--rw-rw-rw-   0 root         (0) root         (0)     4476 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml
--rw-rw-rw-   0 root         (0) root         (0)  1065600 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S2468/files/cwb.multiorder.fits
--rw-rw-rw-   0 root         (0) root         (0)     4047 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S2468/files/significance_subthreshold_lvc-i3.json
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S2468/files.json
--rw-rw-rw-   0 root         (0) root         (0)     4911 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S2468/logs.json
--rw-rw-rw-   0 root         (0) root         (0)     3397 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S2468/superevent.json
--rw-rw-rw-   0 root         (0) root         (0)      966 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S2468/voevents.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.842848 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.908851 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/
--rw-rw-rw-   0 root         (0) root         (0)  1540117 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/LALInference.fits.gz,0
--rw-rw-rw-   0 root         (0) root         (0)     6731 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml
--rw-rw-rw-   0 root         (0) root         (0)     6716 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml
--rw-rw-rw-   0 root         (0) root         (0)   777600 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/bayestar.multiorder.fits
--rw-rw-rw-   0 root         (0) root         (0)  1540117 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/bilby.fits.gz,0
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/coincidence_far.json
--rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz
--rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,0
--rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,1
--rw-rw-rw-   0 root         (0) root         (0)   777600 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/combined-ext.multiorder.fits
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/em_bright.json
--rw-rw-rw-   0 root         (0) root         (0)       52 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/em_bright.json,0
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/p_astro.json
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/p_astro.json,0
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files.json
--rw-rw-rw-   0 root         (0) root         (0)     7678 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/logs.json
--rw-rw-rw-   0 root         (0) root         (0)     5616 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/superevent.json
--rw-rw-rw-   0 root         (0) root         (0)     1585 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/voevents.json
--rw-rw-rw-   0 root         (0) root         (0)     5123 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/test_tool.py
--rw-rw-rw-   0 root         (0) root         (0)     2576 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/ligo/followup_advocate/tool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 17:47:56.911851 ligo-followup-advocate-1.2.3/ligo_followup_advocate.egg-info/
--rw-r--r--   0 root         (0) root         (0)      880 2023-05-24 17:47:56.000000 ligo-followup-advocate-1.2.3/ligo_followup_advocate.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7102 2023-05-24 17:47:56.000000 ligo-followup-advocate-1.2.3/ligo_followup_advocate.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 17:47:56.000000 ligo-followup-advocate-1.2.3/ligo_followup_advocate.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       76 2023-05-24 17:47:56.000000 ligo-followup-advocate-1.2.3/ligo_followup_advocate.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-05-24 17:47:56.000000 ligo-followup-advocate-1.2.3/ligo_followup_advocate.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-24 17:47:56.000000 ligo-followup-advocate-1.2.3/ligo_followup_advocate.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1793 2023-05-24 17:47:56.914851 ligo-followup-advocate-1.2.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      539 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    68611 2023-05-23 20:35:54.000000 ligo-followup-advocate-1.2.3/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.441718 ligo-followup-advocate-1.2.4/
+-rw-rw-rw-   0 root         (0) root         (0)    17895 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/COPYING.md
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      880 2023-06-20 23:10:47.441718 ligo-followup-advocate-1.2.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2855 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.406717 ligo-followup-advocate-1.2.4/ligo/
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.442718 ligo-followup-advocate-1.2.4/ligo/followup_advocate/
+-rw-rw-rw-   0 root         (0) root         (0)    25817 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-06-20 23:10:47.442718 ligo-followup-advocate-1.2.4/ligo/followup_advocate/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1244 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/jinja.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.410717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2960 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/RAVEN_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      944 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/RAVEN_subject.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 23:10:35.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/authors.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      376 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/compare_skymaps.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1036 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/em_bright.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     2614 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/initial_body.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      425 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/initial_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1439 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/llama_alert_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      436 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/llama_subject.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     2447 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/llama_track_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     9889 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/macros.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      567 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/medium_latency_grb_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1682 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/medium_latency_grb_detection_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1496 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/medium_latency_grb_exclusion_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      344 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/medium_latency_grb_subject.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/numbered_pipeline_citations.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      461 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/p_astro.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/retraction.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1122 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/skymap_info.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      310 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/subject.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1350 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/update_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      221 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/userguide_conclusion.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.411717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 23:10:35.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.405717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.411717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1122/
+-rw-rw-rw-   0 root         (0) root         (0)     1880 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1122/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.412717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1122/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1122/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1122/files/distances_x.json
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1122/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1122/files/false_alarm_probability_x.json
+-rw-rw-rw-   0 root         (0) root         (0)      987 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1122/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.412717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1133/
+-rw-rw-rw-   0 root         (0) root         (0)     1877 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1133/event.json
+-rw-rw-rw-   0 root         (0) root         (0)        4 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1133/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.412717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1134/
+-rw-rw-rw-   0 root         (0) root         (0)     1904 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1134/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.412717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1134/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1134/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1134/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)      515 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1134/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.413717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1234/
+-rw-rw-rw-   0 root         (0) root         (0)     1881 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1234/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.413717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1234/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1234/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1234/files/distances_x.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1234/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1234/files/false_alarm_probability_x.json
+-rw-rw-rw-   0 root         (0) root         (0)      714 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1234/files/initial.data
+-rw-rw-rw-   0 root         (0) root         (0)     1086 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1234/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.414717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1235/
+-rw-rw-rw-   0 root         (0) root         (0)     1876 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1235/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.414717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1235/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1235/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1235/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)      714 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1235/files/initial.data
+-rw-rw-rw-   0 root         (0) root         (0)      610 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1235/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.414717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E2244/
+-rw-rw-rw-   0 root         (0) root         (0)     1904 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E2244/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.415717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E2244/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E2244/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E2244/files/distances_x.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E2244/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E2244/files/false_alarm_probability_x.json
+-rw-rw-rw-   0 root         (0) root         (0)      991 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E2244/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.415717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E5678/
+-rw-rw-rw-   0 root         (0) root         (0)     1918 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E5678/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.415717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E5678/files/
+-rw-rw-rw-   0 root         (0) root         (0)     5761 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E5678/files/initial.data
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E5678/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.416717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M1122/
+-rw-rw-rw-   0 root         (0) root         (0)     1936 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M1122/event.json
+-rw-rw-rw-   0 root         (0) root         (0)      633 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M1122/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.416717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M1234/
+-rw-rw-rw-   0 root         (0) root         (0)     3958 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M1234/event.json
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M1234/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.416717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M1235/
+-rw-rw-rw-   0 root         (0) root         (0)     3982 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M1235/event.json
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M1235/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.417717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M2468/
+-rw-rw-rw-   0 root         (0) root         (0)     3956 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M2468/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.417717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M2468/files/
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M2468/files/p_astro.json
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M2468/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.417717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M2469/
+-rw-rw-rw-   0 root         (0) root         (0)     3979 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M2469/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.417717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M2469/files/
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M2469/files/p_astro.json
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M2469/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.417717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M5566/
+-rw-rw-rw-   0 root         (0) root         (0)     3958 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M5566/event.json
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M5566/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.418717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M5678/
+-rw-rw-rw-   0 root         (0) root         (0)     3955 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M5678/event.json
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M5678/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.418717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M5679/
+-rw-rw-rw-   0 root         (0) root         (0)     3979 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M5679/event.json
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M5679/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.419717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.424717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files/
+-rw-rw-rw-   0 root         (0) root         (0)     4609 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files/S1234-1-EarlyWarning.xml
+-rw-rw-rw-   0 root         (0) root         (0)     4607 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files/S1234-2-Initial.xml
+-rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files/bayestar-ext.fits.gz
+-rw-rw-rw-   0 root         (0) root         (0)   777600 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files/bayestar.fits.gz
+-rw-rw-rw-   0 root         (0) root         (0)   777600 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files/bayestar.multiorder.fits
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files/coincidence_far.json
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files/em_bright.json
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files/p_astro.json
+-rw-rw-rw-   0 root         (0) root         (0)     1832 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files.json
+-rw-rw-rw-   0 root         (0) root         (0)     7997 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/logs.json
+-rw-rw-rw-   0 root         (0) root         (0)     5897 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/superevent.json
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/voevents.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.424717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S2468/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.426717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S2468/files/
+-rw-rw-rw-   0 root         (0) root         (0)     4476 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml
+-rw-rw-rw-   0 root         (0) root         (0)  1065600 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S2468/files/cwb.multiorder.fits
+-rw-rw-rw-   0 root         (0) root         (0)     4047 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S2468/files/significance_subthreshold_lvc-i3.json
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S2468/files.json
+-rw-rw-rw-   0 root         (0) root         (0)     4911 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S2468/logs.json
+-rw-rw-rw-   0 root         (0) root         (0)     3397 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S2468/superevent.json
+-rw-rw-rw-   0 root         (0) root         (0)      966 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S2468/voevents.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.426717 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.440718 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/
+-rw-rw-rw-   0 root         (0) root         (0)  1540117 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/LALInference.fits.gz,0
+-rw-rw-rw-   0 root         (0) root         (0)     6731 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml
+-rw-rw-rw-   0 root         (0) root         (0)     6716 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml
+-rw-rw-rw-   0 root         (0) root         (0)   777600 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/bayestar.multiorder.fits
+-rw-rw-rw-   0 root         (0) root         (0)  1540117 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/bilby.fits.gz,0
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/coincidence_far.json
+-rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz
+-rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,0
+-rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,1
+-rw-rw-rw-   0 root         (0) root         (0)   777600 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/combined-ext.multiorder.fits
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/em_bright.json
+-rw-rw-rw-   0 root         (0) root         (0)       52 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/em_bright.json,0
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/p_astro.json
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/p_astro.json,0
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files.json
+-rw-rw-rw-   0 root         (0) root         (0)     7678 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/logs.json
+-rw-rw-rw-   0 root         (0) root         (0)     5616 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/superevent.json
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/voevents.json
+-rw-rw-rw-   0 root         (0) root         (0)     5199 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/test_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)     2957 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/ligo/followup_advocate/tool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 23:10:47.441718 ligo-followup-advocate-1.2.4/ligo_followup_advocate.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      880 2023-06-20 23:10:47.000000 ligo-followup-advocate-1.2.4/ligo_followup_advocate.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7102 2023-06-20 23:10:47.000000 ligo-followup-advocate-1.2.4/ligo_followup_advocate.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 23:10:47.000000 ligo-followup-advocate-1.2.4/ligo_followup_advocate.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       76 2023-06-20 23:10:47.000000 ligo-followup-advocate-1.2.4/ligo_followup_advocate.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-06-20 23:10:47.000000 ligo-followup-advocate-1.2.4/ligo_followup_advocate.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-20 23:10:47.000000 ligo-followup-advocate-1.2.4/ligo_followup_advocate.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1793 2023-06-20 23:10:47.442718 ligo-followup-advocate-1.2.4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      539 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)    68611 2023-06-20 23:08:27.000000 ligo-followup-advocate-1.2.4/versioneer.py
```

### Comparing `ligo-followup-advocate-1.2.3/COPYING.md` & `ligo-followup-advocate-1.2.4/COPYING.md`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/PKG-INFO` & `ligo-followup-advocate-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ligo-followup-advocate
-Version: 1.2.3
+Version: 1.2.4
 Summary: LIGO/Virgo/KAGRA Follow-up Advocate Tools
 Home-page: https://git.ligo.org/emfollow/ligo-followup-advocate
 Author: Leo Singer
 Author-email: leo.singer@ligo.org
 Maintainer: Brandon Piotrzkowski
 Maintainer-email: brandon.piotrzkowski@ligo.org
 License: GPL-2+
```

### Comparing `ligo-followup-advocate-1.2.3/README.md` & `ligo-followup-advocate-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/__init__.py` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -159,20 +159,20 @@
         prob_has_massgap=source_classification.get('HasMassGap'),
         include_ellipse=None,
         classifications=classifications,
         citation_index=citation_index)
 
     if skymaps:
         preferred_skymap = skymaps[-1]['filename']
-        cl = 90
+        cls = [50, 90]
         include_ellipse, ra, dec, a, b, pa, area, greedy_area = \
-            uncertainty_ellipse(gracedb_id, preferred_skymap, client, cl=cl)
+            uncertainty_ellipse(gracedb_id, preferred_skymap, client, cls=cls)
         kwargs.update(
             preferred_skymap=preferred_skymap,
-            cl=cl,
+            cl=cls[-1],
             include_ellipse=include_ellipse,
             ra=coord.Longitude(ra*u.deg),
             dec=coord.Latitude(dec*u.deg),
             a=coord.Angle(a*u.deg),
             b=coord.Angle(b*u.deg),
             pa=coord.Angle(pa*u.deg),
             ellipse_area=area,
@@ -254,15 +254,15 @@
                       tl, format='gps').isot).replace('T', ' ')
     th_datetime = str(astropy.time.Time(
                       th, format='gps').isot).replace('T', ' ')
 
     o = urllib.parse.urlparse(client.service_url)
     kwargs = dict(
         gracedb_service_url=urllib.parse.urlunsplit(
-            (o.scheme, o.netloc, '/events/', '', '')),
+            (o.scheme, o.netloc, '/superevents/', '', '')),
         gracedb_id=gracedb_id,
         llama=True,
         icecube_alert=icecube_alert,
         event_time=event_time,
         tl_datetime=tl_datetime,
         th_datetime=th_datetime,
         authors=authors)
@@ -305,15 +305,16 @@
         body = (
             env.get_template('llama_track_circular.jinja2').render(**kwargs)
             .strip())
     return '{0}\n\n{1}'.format(subject, body)
 
 
 def compose_grb_medium_latency(
-        gracedb_id, authors=(), service=rest.DEFAULT_SERVICE_URL, client=None):
+        gracedb_id, authors=(), service=rest.DEFAULT_SERVICE_URL,
+        use_detection_template=None, client=None):
     """Compose GRB Medium Latency GCN Circular draft.
     Here, gracedb_id will be a GRB external trigger ID in GraceDb."""
 
     if client is None:
         client = rest.GraceDb(service)
 
     event = client.event(gracedb_id).json()
@@ -342,15 +343,19 @@
 
     citation_index = {}
     index = 1
     xpipeline_fap_file = 'false_alarm_probability_x.json'
     if xpipeline_fap_file in files:
         xpipeline_fap = client.files(gracedb_id, xpipeline_fap_file).json()
         online_xpipeline_fap = xpipeline_fap.get('Online Xpipeline')
-        if online_xpipeline_fap < 0.001:
+        # Create detection/exclusion circular based on given argument
+        # Use default cutoff if not provided
+        xpipeline_detection = (use_detection_template if use_detection_template
+                               is not None else online_xpipeline_fap < 0.001)
+        if xpipeline_detection:
             kwargs['detections'].append('xpipeline')
             kwargs.update(online_xpipeline_fap=online_xpipeline_fap)
         else:
             kwargs['exclusions'].append('xpipeline')
             xpipeline_distances_file = 'distances_x.json'
             xpipeline_distances = client.files(gracedb_id,
                                                xpipeline_distances_file).json()
@@ -359,15 +364,19 @@
         citation_index['xpipeline'] = index
         index += 1
 
     pygrb_fap_file = 'false_alarm_probability_pygrb.json'
     if pygrb_fap_file in files:
         pygrb_fap = client.files(gracedb_id, pygrb_fap_file).json()
         online_pygrb_fap = pygrb_fap.get('Online PyGRB')
-        if online_pygrb_fap < 0.01:
+        # Create detection/exclusion circular based on given argument
+        # Use default cutoff if not provided
+        pygrb_detection = (use_detection_template if use_detection_template
+                           is not None else online_pygrb_fap < 0.01)
+        if pygrb_detection:
             kwargs['detections'].append('pygrb')
             kwargs.update(online_pygrb_fap=online_pygrb_fap)
         else:
             kwargs['exclusions'].append('pygrb')
             pygrb_distances_file = 'distances_pygrb.json'
             pygrb_distances = client.files(gracedb_id,
                                            pygrb_distances_file).json()
@@ -514,46 +523,50 @@
     joint_areas = [(mask & masks[-1]).sum() * deg2perpix for mask in masks]
 
     kwargs = dict(params=zip(filenames, pipelines, areas, joint_areas))
 
     return env.get_template('compare_skymaps.jinja2').render(**kwargs)
 
 
-def uncertainty_ellipse(graceid, filename, client, cl=90,
+def uncertainty_ellipse(graceid, filename, client, cls=[50, 90],
                         ratio_ellipse_cl_areas=1.35):
     """Compute uncertainty ellipses for a given sky map
 
     Parameters
     ----------
     graceid: str
         ID of the trigger used by GraceDB
     filename: str
         File name of sky map
     client: class
         REST API client for HTTP connection
-    cl: float
-        Percentage of minimal credible area
+    cls: list
+        List of percentage of minimal credible area used to check whether the
+        areas are close to an ellipse, returning the values of the final item
     ratio_ellipse_cl_areas: float
         Ratio between ellipse area and minimal credible area from cl
     """
     if filename.endswith('.gz'):
         # Try using the multi-res sky map if it exists
         try:
             new_filename = filename.replace('.fits.gz', '.multiorder.fits')
             skymap = read_map_gracedb(graceid, new_filename, client)
         except (IOError, rest.HTTPError):
             skymap = read_map_gracedb(graceid, filename, client)
     else:
         skymap = read_map_gracedb(graceid, filename, client)
 
-    result = crossmatch(skymap, contours=[cl / 100])
-    greedy_area = result.contour_areas[0]
-    ra, dec, a, b, pa, ellipse_area = find_ellipse(skymap, cl=cl)
-    return ellipse_area <= ratio_ellipse_cl_areas*greedy_area, ra, dec, a, b, \
-        pa, ellipse_area, greedy_area
+    use_ellipse = True
+    for cl in cls:
+        result = crossmatch(skymap, contours=[cl / 100])
+        greedy_area = result.contour_areas[0]
+        ra, dec, a, b, pa, ellipse_area = find_ellipse(skymap, cl=cl)
+        use_ellipse = (ellipse_area <= ratio_ellipse_cl_areas * greedy_area and
+                       use_ellipse)
+    return use_ellipse, ra, dec, a, b, pa, ellipse_area, greedy_area
 
 
 def _update_raven_parameters(gracedb_id, kwargs, client):
     """Update kwargs with parameters for RAVEN coincidence"""
 
     event = client.superevent(gracedb_id).json()
 
@@ -640,21 +653,22 @@
                     alert_type=alert_type,
                     filename=filename,
                     latency=issued_time-event_time.gps)
 
         if combined_skymaps:
             combined_skymaps = list(combined_skymaps.values())
             combined_skymap = combined_skymaps[-1]['filename']
-            cl = 90
+            cls = [50, 90]
             include_ellipse, ra, dec, a, b, pa, area, greedy_area = \
-                uncertainty_ellipse(gracedb_id, combined_skymap, client, cl=cl)
+                uncertainty_ellipse(gracedb_id, combined_skymap, client,
+                                    cls=cls)
             kwargs.update(
                 combined_skymap=combined_skymap,
                 combined_skymaps=combined_skymaps,
-                cl=cl,
+                cl=cls[-1],
                 combined_skymap_include_ellipse=include_ellipse,
                 combined_skymap_ra=coord.Longitude(ra*u.deg),
                 combined_skymap_dec=coord.Latitude(dec*u.deg),
                 combined_skymap_a=coord.Angle(a*u.deg),
                 combined_skymap_b=coord.Angle(b*u.deg),
                 combined_skymap_pa=coord.Angle(pa*u.deg),
                 combined_skymap_ellipse_area=area,
```

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/jinja.py` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/jinja.py`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/RAVEN_circular.jinja2` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/RAVEN_circular.jinja2`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 {% from 'macros.jinja2' import naturalfar, grbmission, grbmission_targeted, naturalotherexternalpipelines, propername %}
 {% if not update_alert %}{% include 'authors.jinja2' %}
 
 {% include 'initial_body.jinja2' %}
 {% endif %}
 {% filter rewrap %}
 A search performed by the RAVEN pipeline found a temporal coincidence between
-{{gracedb_id}} and a {% if snews %}SNEWS supernova{% elif grb %}{% if subthreshold %}sub-threshold {% endif %}{{grbmission(external_pipeline)}}{% endif %} {{propername(external_trigger)}} **CITE ORIGINAL GCN FOR THE EXTERNAL TRIGGER FROM https://gcn.gsfc.nasa.gov/gcn3_archive.html, e.g., (Bhalerao et al., GCN Circular XXXXX)**.
+{{gracedb_id}} and a {% if snews %}SNEWS supernova{% elif grb %}{% if subthreshold %}sub-threshold {% endif %}{{grbmission(external_pipeline)}}{% endif %} {{propername(external_trigger)}} **CITE ORIGINAL GCN FOR THE EXTERNAL TRIGGER FROM https://gcn.nasa.gov/circulars, e.g., (Bhalerao et al., GCN Circular XXXXX)**.
 The {% if snews %}neutrino{% elif grb %}GRB{% endif %} trigger time is {{latency}} seconds {{beforeafter}} the GW candidate event.
 {% if grb %}
 The estimated joint false alarm rate for the coincidence using just timing info is {{naturalfar(time_coinc_far)}}.
 {% if subthreshold_targeted %}The GRB candidate was found during a joint targeted search between the LIGO/Virgo/KAGRA collaboration and {{grbmission_targeted(external_pipeline)}}, and has a false alarm rate of {{naturalfar(far_grb)}}. {% endif %}
 {% if other_ext_pipelines %}RAVEN has also identified {% if other_ext_pipelines|length == 1 %}an additional detection{% elif other_ext_pipelines|length > 1%}additional detections{% endif %} from {{naturalotherexternalpipelines(other_ext_pipelines)}}.{% endif %}
 {% endif %}
 
 {% if combined_skymap %}
 {% if combined_skymaps|length == 1 %}A combined sky map is{% else %}Combined sky maps are{% endif %} also available:
 {% for skymap in combined_skymaps %}
- * {{skymap.filename}}, an {% if skymap.alert_type in ['preliminary','initial'] %}initial{% elif skymap.alert_type == 'earlywarning' %}early warning{% else %}updated{% endif %} localization, distributed via GCN notice about {{skymap.latency|abs|naturaldelta}} {% if skymap.latency < 0 %}before {% else %}after {% endif %}the candidate event time.
+ * {{skymap.filename}}, an {% if skymap.alert_type in ['preliminary','initial'] %}initial{% elif skymap.alert_type == 'earlywarning' %}early-warning{% else %}updated{% endif %} localization, distributed via GCN notice about {{skymap.latency|abs|naturaldelta}} {% if skymap.latency < 0 %}before {% else %}after {% endif %}the candidate event time.
 {% endfor %}
 
 For the {{combined_skymap}} sky map, the {{cl}}% credible region is {{combined_skymap_greedy_area|round|int}} deg2.
 {% endif %}
 {% if external_pipeline|lower == 'swift'%}
 The joint localization is dominated by the {{grbmission(external_pipeline)}} candidate, which was identified with right ascension, declination of {{'%0.3f' % ext_ra|float}}, {{'%0.3f' % ext_dec|float}}{% if ext_error %} and 90% containment error radius of {{'%0.3f' % ext_error|float}} deg{% endif %}.
 {% endif %}
```

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/RAVEN_subject.jinja2` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/RAVEN_subject.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/authors.jinja2` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/authors.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/em_bright.jinja2` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/em_bright.jinja2`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 {% from 'macros.jinja2' import evidence_for, probability,
                                citeskymap_number %}
 {% filter rewrap %}
 {% if subject == 'Update' %}Based on posterior support from parameter
 estimation {{citeskymap_number(updated_skymap.pipeline, citation_index)}},
 under the assumption that the candidate {{gracedb_id}} is astrophysical in
-origin,{% else %}Assuming the candidate is astrophysical in origin, {% endif %}
+origin, {% else %}Assuming the candidate is astrophysical in origin, {% endif %}
 the probability that the lighter compact object is consistent with a neutron star mass
 (HasNS) is {{probability(prob_has_ns)}}.
 [{{citation_index['em_bright']}}] Using the masses and spins inferred from the signal, the
 probability of matter outside the final compact object (HasRemnant) is
 {{probability(prob_has_remnant)}}. [{{citation_index['em_bright']}}]
 Both HasNS and HasRemnant consider the support of several neutron star
-equations of state. The probability that any one of the binary components
-lie between 3 to 5 solar mass (HasMassgap) is {{probability(prob_has_massgap)}}.
+equations of state. The probability that either of the binary components
+lies between 3 and 5 solar masses (HasMassgap) is {{probability(prob_has_massgap)}}.
 
 {% endfilter %}
```

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/initial_body.jinja2` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/initial_body.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
                             renamegroup, citeskymap %}
 {% filter rewrap %}
 We identified the {{renamegroup(group)}} candidate {{gracedb_id}} during real-time processing of data from
 {{naturalinstruments(instruments, )}} at {{utctime}} UTC (GPS time: {{gpstime}}).
 The candidate was found by the {{naturalpipelines(all_pipelines, citation_index)}}
 analysis pipeline{% if all_pipelines|length > 1 %}s{% endif %}.
 {% if early_warning_alert and early_warning_pipelines %}
-An early-warning alert was issued for this candidate, with {% if early_warning_pipelines|length > 1 %}detections{% else %} a detection{% endif %} from the {{naturalearlywarningpipelines(early_warning_pipelines, citation_index)}} early-warning pipeline{% if early_warning_pipelines|length > 1 %}s{% endif %}.
+An early-warning alert was issued for this candidate, detected by the {{naturalearlywarningpipelines(early_warning_pipelines, citation_index)}} early-warning pipeline{% if early_warning_pipelines|length > 1 %}s{% endif %}.
 {% endif %}
 
 {% if change_significance_statement %}
 Based on the analysis of gravitational-wave data alone, this candidate does not meet our criteria for a high-significance public alert.
 However, a search performed by the RAVEN pipeline found a significant coincidence between this candidate and {{external_trigger}}.
 {% else %}
 {{gracedb_id}} is an event of interest because its false alarm rate, as
@@ -30,13 +30,13 @@
 {% if prob_has_ns is not none %}
 {%- include 'em_bright.jinja2' -%}
 {% endif %}
 {% if skymaps|length == 0 %}
 No{% else %}{{ skymaps|length|apnumber|capitalize }}{% endif %} {% if combined_skymap is not defined %}sky map{% else %}GW-only sky map{% endif %}{% if skymaps|length == 1 %} is{% else %}s are{% endif %} available at this time{% if skymaps|length > 0 %} and can be retrieved from the GraceDB event page:{% else %}.{% endif %}
 
 {% for skymap in skymaps %}
- * {{skymap.filename}}, an {% if skymap.alert_type in ['preliminary','initial'] %}initial{% elif skymap.alert_type == 'earlywarning' %}early warning{% else %}updated{% endif %} localization generated by {{citeskymap(skymap.pipeline, citation_index)}}, distributed via GCN notice about {{skymap.latency|abs|naturaldelta}} {% if skymap.latency < 0 %}before {% else %}after {% endif %}the candidate event time.
+ * {{skymap.filename}}, an {% if skymap.alert_type in ['preliminary','initial'] %}initial{% elif skymap.alert_type == 'earlywarning' %}early-warning{% else %}updated{% endif %} localization generated by {{citeskymap(skymap.pipeline, citation_index)}}, distributed via GCN notice about {{skymap.latency|abs|naturaldelta}} {% if skymap.latency < 0 %}before {% else %}after {% endif %}the candidate event time.
 {% endfor %}
 
 {% if skymaps|length != 0 %}{%- include 'skymap_info.jinja2' -%}{% endif %}
 {% endif %}
 {% endfilter %}
```

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/llama_alert_circular.jinja2` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/llama_alert_circular.jinja2`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 {% from 'macros.jinja2' import citeskymap_number %}
 
 {% filter rewrap %}
 {% include 'authors.jinja2' %}
 
-A LLAMA search for LIGO-Virgo-KAGRA gravitational-wave candidate consistent
-with the sky localization of IceCube alert {{icecube_alert}} (<link to notice>)
-in a time range of 1000 seconds {{citeskymap_number('llama', citation_index)}}
-centered on the alert event time
-({{tl_datetime}} UTC to {{tl_datetime}} UTC) have been performed.
-The hypothesis test employed by LLAMA uses a Bayesian approach to quantify
-the joint GW + neutrino event significance. {{citeskymap_number('llama_stat', citation_index)}}
-
-Gravitational-wave candidate {{gracedb_id}} is found to be in spatial and temporal
-coincidence with {{icecube_alert}} public alert. The properties of the candidate
-event, which based on the analysis of gravitational-wave data alone does not
-meet the LIGO/Virgo/KAGRA criteria for a high-significance public alert and can
-be found at this URL:
+A LLAMA search has been performed for LIGO/Virgo/KAGRA
+gravitational-wave candidates consistent with the sky localization of
+IceCube alert {{icecube_alert}} (** <add link to notice> **) in a
+time range of 1000 seconds {{citeskymap_number('llama', citation_index)}} centered on the alert event time
+({{tl_datetime}} UTC to {{th_datetime}} UTC).
+
+Gravitational-wave candidate {{gracedb_id}} has been identified by this
+search. This candidate does not meet the LIGO/Virgo/KAGRA public alert
+criteria based on analysis of the gravitational-wave data alone, but
+it is found to be in spatial and temporal coincidence with
+{{icecube_alert}} public alert. The properties of the GW
+candidate can be found at this URL:
 
 {{ gracedb_service_url }}{{ gracedb_id }}
 
 The neutrino trigger time is xxx.xx seconds before(after) the gravitational-wave
 candidate event. The p-value associated with the joint observation is {{'%.4g'|format(llama_fap)}}.
 We encourage further observation of the localization area of {{icecube_alert}}
 and we provide a joint localization probability map at:
 
 <gracedb link here>
 
 Further information about analysis methodology can be found at
-<https://multimessenger.science/>.
+https://multimessenger.science/.
 {% endfilter %}
 {% include 'userguide_conclusion.jinja2' %}
 {% filter rewrap %}
 {% include 'numbered_pipeline_citations.jinja2' %}
 {% endfilter %}
```

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/llama_track_circular.jinja2` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/llama_track_circular.jinja2`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 {% from 'macros.jinja2' import citeskymap_number %}
 
 {% filter rewrap %}
 {% include 'authors.jinja2' %}
 
-Searches for track-like muon neutrino events detected by IceCube consistent
-with the sky localization of gravitational-wave candidate {{gracedb_id}} in a time range
-of 1000 seconds {{citeskymap_number('llama', citation_index)}} centered on the alert event time
-({{tl_datetime}} UTC to {{th_datetime}} UTC) have been performed.
-During this time period IceCube was collecting good quality data. The hypothesis
-test employed by LLAMA uses a Bayesian approach to quantify the joint GW + neutrino
-event significance. {{citeskymap_number('llama_stat', citation_index)}}
-
-{{neutrinos|length|int}} track-like event{% if neutrinos|length > 1 %}s were{% else %} was{% endif %} found in spatial and temporal coincidence with the
-gravitational-wave candidate {{gracedb_id}}. The event’s properties can be found at
-this URL:
+Searches have been performed for {% if neutrinos|length == 1 %}a {% endif %}track-like muon neutrino event{% if neutrinos|length > 1 %}s{% endif %} 
+detected by IceCube consistent with the the time and sky localization
+of the gravitational-wave (GW) candidate {{gracedb_id}}. The GW candidate's
+properties can be found at this URL:
 
 {{ gracedb_service_url }}{{ gracedb_id }}
 
-Based on the analysis of gravitational-wave data alone, this candidate does not
-meet our criteria for a high-significance public alert.
+Based on the analysis of gravitational-wave data alone, this candidate
+does not meet LIGO/Virgo/KAGRA criteria for a public alert.
+
+IceCube data was searched in a time range of 1000 seconds {{citeskymap_number('llama', citation_index)}} centered
+on the GW event time ({{tl_datetime}} UTC to {{th_datetime}} UTC).
+During this time period IceCube was collecting
+good quality data. The hypothesis test employed by LLAMA uses a
+Bayesian approach to quantify the joint GW + neutrino event
+significance. {{citeskymap_number('llama_stat', citation_index)}}
+From this analysis, {{neutrinos|length|int}} track-like event{% if neutrinos|length > 1 %}s were{% else %} was{% endif %} found
+in spatial and temporal coincidence with the gravitational-wave
+candidate {{gracedb_id}}.
 
 Properties of the coincident neutrino{% if neutrinos|length > 1 %}s{% endif %} together with the p-value{% if neutrinos|length > 1 %}s{% endif %} associated
 with the joint observation {% if neutrinos|length > 1 %}are{% else %}is{% endif %} shown below. 
 
 {% endfilter %}
 dt         ra        dec      Angular Uncertainty(deg)     p-value
 ------------------------------------------------------------------
@@ -37,14 +40,14 @@
 p-value = the p-value for this specific track event from each search.
 {% filter rewrap %}
 
 The IceCube Neutrino Observatory is a cubic-kilometer neutrino detector
 operating at the geographic South Pole, Antarctica. The IceCube realtime alert
 point of contact can be reached at roc@icecube.wisc.edu
 
-For further information about analysis methodology can be found at
-<https://multimessenger.science/>.
+Further information about analysis methodology can be found at
+https://multimessenger.science/.
 {% endfilter %}
 {% include 'userguide_conclusion.jinja2' %}
 {% filter rewrap %}
 {% include 'numbered_pipeline_citations.jinja2' %}
 {% endfilter %}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/macros.jinja2` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/macros.jinja2`

 * *Files 0% similar despite different names*

```diff
@@ -252,15 +252,15 @@
                     'spiir': 'Chu et al. PRD 105, 024023 (2022)',
                     'pycbc_earlywarning': 'Nitz A. H., Schäfer M., Dal Canton T. ApJL 902, 2 (2020)',
                     'gstlal_earlywarning': 'Sachdev et al. ApJL 905, 2 (2020)',
                     'spiir_earlywarning': 'Kovalam et al. ApJL 927, 1 (2022)',
                     'cwb': 'Klimenko et al. PRD 93, 042004 (2016)',
                     'olib': 'Lynch et al. PRD 95, 104046 (2017)',
                     'mly': 'Skliris et al. arXiv:2009.14611 (2020)',
-                    'em_bright': 'Chatterjee et al. ApJ 896, 1 (2020)',
+                    'em_bright': 'Chatterjee et al. ApJ 896, 54 (2020)',
                     'pygrb': 'Williamson et al. PRD 90, 122004 (2014)',
                     'xpipeline': 'Was et al. PRD 86, 022003 (2012)',
                     'llama': 'Baret et al., Astroparticle Physics 35, 1 (2011)',
                     'llama_stat': 'Bartos et al. arXiv:1810.11467 (2018) and Countryman et al.\n arXiv:1901.05486 (2019)',
                     'bayestar': 'Singer & Price PRD 93, 024013 (2016)',
                     'bilby': 'Ashton et al. ApJS 241, 27 (2019)',
                     'lalinference': 'Veitch et al. PRD 91, 042003 (2015)',
```

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/medium_latency_grb_circular.jinja2` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/medium_latency_grb_circular.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/medium_latency_grb_detection_circular.jinja2` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/medium_latency_grb_detection_circular.jinja2`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 {% from 'macros.jinja2' import naturalgrbmediumlatencypipelines,
                                naturalfap, grbmission, propername %}
 {% filter rewrap %}
-The {{naturalgrbmediumlatencypipelines(detections, citation_index)}} made{% if detections|length == 1 %} a{% endif %} preliminary identification of {% if detections|length == 1 %}a {% endif %}gravitational wave (GW) candidate{% if detections|length == 2 %}s{% endif %} associated with the time and sky position of GRB {{grbmission(pipeline)}} {{propername(external_trigger)}} **CITE ORIGINAL GCN FOR THE EXTERNAL TRIGGER FROM https://gcn.gsfc.nasa.gov/gcn3_archive.html, e.g., (Bhalerao et al., GCN Circular XXXXX)**.
+The {{naturalgrbmediumlatencypipelines(detections, citation_index)}} made{% if detections|length == 1 %} a{% endif %} preliminary identification of {% if detections|length == 1 %}a {% endif %}gravitational wave (GW) candidate{% if detections|length == 2 %}s{% endif %} associated with the time and sky position of GRB {{grbmission(pipeline)}} {{propername(external_trigger)}} **CITE ORIGINAL GCN FOR THE EXTERNAL TRIGGER FROM https://gcn.nasa.gov/circulars, e.g., (Bhalerao et al., GCN Circular XXXXX)**.
 
 {% if detections|length == 2 %}
 In PyGRB, the candidate is consistent with a binary coalescence with False Alarm Probability of {{naturalfap(online_pygrb_fap)}}.
 
 In X-Pipeline, the candidate is an unmodeled GW transient with False Alarm Probability of {{naturalfap(online_xpipeline_fap)}}.
 {% elif detections| length == 1%}
 The candidate is {% if 'Burst' in detections %}an unmodeled GW transient{% else %}consistent with a binary coalescence{% endif %} with False Alarm Probability of {% if 'Burst' in detections %}{{online_xpipeline_fap}}{% else %}{{online_pygrb_fap}}{% endif %}.
 {% endif %}
 
 The False Alarm Probability is calculated by counting the fraction of background trials containing an event with a greater detection statistic than the loudest on-source event. The off-source trials are of {% if detections|length == 2 %}6 s duration for CBC and 660 s duration for Burst{% elif detections| length == 1%}{% if 'Burst' in detections %}660 s duration{% else %}6 s duration{% endif %}{% endif %}.
-
-Offline analyses are ongoing. Any significant updates will be provided by a new circular.
 {% endfilter %}
```

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/medium_latency_grb_exclusion_circular.jinja2` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/medium_latency_grb_exclusion_circular.jinja2`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 {% from 'macros.jinja2' import naturalgrbmediumlatencypipelines,
                                grbmission, propername %}
 {% filter rewrap %}
-The {{naturalgrbmediumlatencypipelines(exclusions, citation_index)}} did not find a candidate gravitational wave (GW) event associated with GRB {{grbmission(pipeline)}} {{propername(external_trigger)}} **CITE ORIGINAL GCN FOR THE EXTERNAL TRIGGER FROM https://gcn.gsfc.nasa.gov/gcn3_archive.html, e.g., (Bhalerao et al., GCN Circular XXXXX)**.
+The {{naturalgrbmediumlatencypipelines(exclusions, citation_index)}} did not find a candidate gravitational wave (GW) event associated with GRB {{grbmission(pipeline)}} {{propername(external_trigger)}} **CITE ORIGINAL GCN FOR THE EXTERNAL TRIGGER FROM https://gcn.nasa.gov/circulars, e.g., (Bhalerao et al., GCN Circular XXXXX)**.
 
-Preliminary exclusion distances with the below assumptions:
+Preliminary exclusion distances with the assumptions given below:
 
 {% if 'pygrb' in exclusions %}
 NS-NS: {{nsns_exclusion}} Mpc, 90% CL {{'\n'}}
 NS-BH: {{nsbh_exclusion}} Mpc, 90% CL {{'\n'}}
 {% endif %}
 {% if 'xpipeline' in exclusions %}
 Rotational model: {{burst_exclusion}} Mpc, 90% CL {{'\n'}} 
 {% endif %}
 
 {% if 'pygrb' in exclusions %}
 Exclusion distance from a Gaussian distribution of mass, uniform distribution of spin and inclination. NS-NS: a Gaussian distribution of component masses 1-3 M_sun, uniform distributions of spin 0-0.4, and inclination angle up to a maximum of 30 deg. NS-BH: as above for NS; BH mass and spin distributions 3-15 M_sun, 0-0.98.
 {% endif %}
 {% if 'xpipeline' in exclusions %}
-Unmodeled transient exclusion distance from an ad hoc rotational model with a circularly polarized, sine-Gaussian waveform with Q-factor = 9 and center frequency = 150 Hz, assuming E_GW = 10^-2 M_sun c^2 of energy emitted as GWs. Exclusion distance scales roughly as sqrt(E_GW).
+Unmodeled transient exclusion distance from an ad hoc rotational model with a circularly polarized, sine-Gaussian waveform with Q-factor = 9 and center frequency = 150 Hz, assuming E_GW = 0.01 M_sun c^2 of energy emitted as GWs. Exclusion distance scales roughly as sqrt(E_GW).
 {% endif %}
 {% endfilter %}
```

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/skymap_info.jinja2` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/skymap_info.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/templates/update_circular.jinja2` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/templates/update_circular.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1122/event.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1122/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1122/files.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1122/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1133/event.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1133/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1134/event.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1134/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1134/files.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1134/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1234/event.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1234/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1234/files/initial.data` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1234/files/initial.data`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1234/files.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1234/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1235/event.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1235/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1235/files/initial.data` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1235/files/initial.data`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E1235/files.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E1235/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E2244/event.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E2244/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E2244/files.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E2244/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E5678/event.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E5678/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/E5678/files/initial.data` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/E5678/files/initial.data`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M1122/event.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M1122/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M1122/files.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M1122/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M1234/event.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M1234/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M1234/files.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M1234/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M1235/event.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M1235/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M1235/files.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M1235/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M2468/event.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M2468/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M2468/files.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M2468/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M2469/event.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M2469/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M2469/files.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M2469/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M5566/event.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M5566/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M5566/files.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M5566/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M5678/event.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M5678/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M5678/files.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M5678/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M5679/event.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M5679/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/M5679/files.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/M5679/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files/S1234-1-EarlyWarning.xml` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files/S1234-1-EarlyWarning.xml`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files/S1234-2-Initial.xml` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files/S1234-2-Initial.xml`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files/bayestar-ext.fits.gz` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files/bayestar-ext.fits.gz`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files/bayestar.fits.gz` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files/bayestar.fits.gz`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files/bayestar.multiorder.fits` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files/bayestar.multiorder.fits`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/files.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/logs.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/logs.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/superevent.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/superevent.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S1234/voevents.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S1234/voevents.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S2468/files/cwb.multiorder.fits` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S2468/files/cwb.multiorder.fits`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S2468/files/significance_subthreshold_lvc-i3.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S2468/files/significance_subthreshold_lvc-i3.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S2468/files.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S2468/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S2468/logs.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S2468/logs.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S2468/superevent.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S2468/superevent.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S2468/voevents.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S2468/voevents.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/LALInference.fits.gz,0` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/LALInference.fits.gz,0`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/bayestar.multiorder.fits` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/bayestar.multiorder.fits`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/bilby.fits.gz,0` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/bilby.fits.gz,0`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,0` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,0`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,1` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,1`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files/combined-ext.multiorder.fits` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files/combined-ext.multiorder.fits`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/files.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/logs.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/logs.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/superevent.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/superevent.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/data/S5678/voevents.json` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/data/S5678/voevents.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/test/test_tool.py` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/test/test_tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,25 +130,27 @@
 def test_medium_latency_cbc_detection(mock_gracedb):
     main(['--service', 'https://gracedb.invalid/api/',
           'compose_grb_medium_latency', 'E1234'])
 
 
 def test_medium_latency_cbc_burst_detection(mock_gracedb):
     main(['--service', 'https://gracedb.invalid/api/',
-          'compose_grb_medium_latency', 'E1122'])
+          'compose_grb_medium_latency', 'E1122',
+          '--use_detection_template'])
 
 
 def test_medium_latency_cbc_exclusion(mock_gracedb):
     main(['--service', 'https://gracedb.invalid/api/',
           'compose_grb_medium_latency', 'E1134'])
 
 
 def test_medium_latency_cbc_burst_exclusion(mock_gracedb):
     main(['--service', 'https://gracedb.invalid/api/',
-          'compose_grb_medium_latency', 'E2244'])
+          'compose_grb_medium_latency', 'E2244',
+          '--use_exclusion_template'])
 
 
 def test_llama_neutrino_track(mock_gracedb):
     main(['--service', 'https://gracedb.invalid/api/',
           'compose_llama', 'S2468'])
```

### Comparing `ligo-followup-advocate-1.2.3/ligo/followup_advocate/tool.py` & `ligo-followup-advocate-1.2.4/ligo/followup_advocate/tool.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,14 +41,20 @@
     cmd.add_argument('--icecube_alert', metavar='IceCube-230501',
                      required=False,
                      default=None, help='IceCube alert ID')
 
     cmd = add_command(followup_advocate.compose_grb_medium_latency,
                       parents=[authors])
     cmd.add_argument('gracedb_id', metavar='E123456', help='GraceDB ID of GRB')
+    cmd.add_argument('--use_detection_template', action='store_true',
+                     help='If given, always use detection template')
+    cmd.add_argument('--use_exclusion_template', dest='use_detection_template',
+                     action='store_false',
+                     help='If given, always use exclusion template')
+    cmd.set_defaults(use_detection_template=None)
 
     cmd = add_command(followup_advocate.compose_update, parents=[authors])
     cmd.add_argument('gracedb_id', metavar='S123456', help='GraceDB ID')
     cmd.add_argument('update_types', metavar='[sky_localization]',
                      help='List of Update types')
 
     cmd = add_command(followup_advocate.compose_retraction, parents=[authors])
```

### Comparing `ligo-followup-advocate-1.2.3/ligo_followup_advocate.egg-info/PKG-INFO` & `ligo-followup-advocate-1.2.4/ligo_followup_advocate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ligo-followup-advocate
-Version: 1.2.3
+Version: 1.2.4
 Summary: LIGO/Virgo/KAGRA Follow-up Advocate Tools
 Home-page: https://git.ligo.org/emfollow/ligo-followup-advocate
 Author: Leo Singer
 Author-email: leo.singer@ligo.org
 Maintainer: Brandon Piotrzkowski
 Maintainer-email: brandon.piotrzkowski@ligo.org
 License: GPL-2+
```

### Comparing `ligo-followup-advocate-1.2.3/ligo_followup_advocate.egg-info/SOURCES.txt` & `ligo-followup-advocate-1.2.4/ligo_followup_advocate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/setup.cfg` & `ligo-followup-advocate-1.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/setup.py` & `ligo-followup-advocate-1.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.3/versioneer.py` & `ligo-followup-advocate-1.2.4/versioneer.py`

 * *Files identical despite different names*

