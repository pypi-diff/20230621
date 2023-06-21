# Comparing `tmp/damona-0.8.3.tar.gz` & `tmp/damona-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damona-0.8.3.tar", last modified: Fri Apr 14 09:55:16 2023, max compression
+gzip compressed data, was "damona-0.9.0.tar", last modified: Wed Jun 21 07:35:48 2023, max compression
```

## Comparing `damona-0.8.3.tar` & `damona-0.9.0.tar`

### file list

```diff
@@ -1,267 +1,315 @@
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.297055 damona-0.8.3/
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.245055 damona-0.8.3/.github/
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.251055 damona-0.8.3/.github/workflows/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1748 2023-02-21 22:05:28.000000 damona-0.8.3/.github/workflows/bash_test.yml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1875 2023-02-21 22:06:16.000000 damona-0.8.3/.github/workflows/fish_test.yml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1594 2023-02-21 22:03:27.000000 damona-0.8.3/.github/workflows/main.yml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      961 2023-01-10 21:16:10.000000 damona-0.8.3/.github/workflows/pypi.yml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      976 2021-12-30 10:11:24.000000 damona-0.8.3/.gitignore
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      340 2023-04-11 13:45:36.000000 damona-0.8.3/.readthedocs.yml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1574 2020-08-25 18:37:15.000000 damona-0.8.3/CONTRIBUTING.rst
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1532 2020-08-10 11:26:10.000000 damona-0.8.3/LICENSE
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      244 2022-01-19 17:14:01.000000 damona-0.8.3/MANIFEST.in
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    17299 2023-04-14 09:55:16.297055 damona-0.8.3/PKG-INFO
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    16010 2023-04-12 15:49:38.000000 damona-0.8.3/README.rst
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.254055 damona-0.8.3/damona/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1481 2022-01-19 10:34:27.000000 damona-0.8.3/damona/__init__.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3114 2022-01-19 11:46:01.000000 damona-0.8.3/damona/admin.py
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.255055 damona-0.8.3/damona/biocontainers/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2022-01-18 11:56:04.000000 damona-0.8.3/damona/biocontainers/__init__.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)  3790743 2022-01-19 12:13:06.000000 damona-0.8.3/damona/biocontainers/registry.yaml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     6105 2021-12-31 09:42:03.000000 damona-0.8.3/damona/builders.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    13000 2022-01-19 11:00:41.000000 damona-0.8.3/damona/common.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5315 2021-12-31 10:56:58.000000 damona-0.8.3/damona/config.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    15657 2021-12-31 15:14:31.000000 damona-0.8.3/damona/environ.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    22582 2022-01-19 12:09:57.000000 damona-0.8.3/damona/install.py
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.259055 damona-0.8.3/damona/library/
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.260055 damona-0.8.3/damona/library/R/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      119 2020-08-04 13:32:55.000000 damona-0.8.3/damona/library/R/Makefile
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     1588 2020-08-11 20:17:37.000000 damona-0.8.3/damona/library/R/Singularity.R_3.6.3
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     1589 2021-03-19 12:22:16.000000 damona-0.8.3/damona/library/R/Singularity.R_4.0.2
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      144 2021-03-19 12:18:31.000000 damona-0.8.3/damona/library/R/registry.yaml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2021-12-29 10:11:19.000000 damona-0.8.3/damona/library/__init__.py
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.261055 damona-0.8.3/damona/library/conda/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      521 2021-12-22 14:56:38.000000 damona-0.8.3/damona/library/conda/README.rst
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3358 2021-02-22 19:31:08.000000 damona-0.8.3/damona/library/conda/Singularity.conda_4.7.12
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2621 2022-11-08 16:04:03.000000 damona-0.8.3/damona/library/conda/Singularity.conda_4.9.2
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      212 2021-12-22 14:55:56.000000 damona-0.8.3/damona/library/conda/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.261055 damona-0.8.3/damona/library/rust/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      272 2022-08-26 07:32:05.000000 damona-0.8.3/damona/library/rust/Singularity.rust
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.262055 damona-0.8.3/damona/library/ubuntu/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      724 2021-09-02 15:44:16.000000 damona-0.8.3/damona/library/ubuntu/Singularity.ubuntu_16.04
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3391 2021-09-02 15:44:16.000000 damona-0.8.3/damona/library/ubuntu/Singularity.ubuntu_18.04
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      166 2021-09-02 15:44:16.000000 damona-0.8.3/damona/library/ubuntu/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.262055 damona-0.8.3/damona/papers/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2022-01-19 11:53:53.000000 damona-0.8.3/damona/papers/__init__.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    16088 2023-04-10 17:45:28.000000 damona-0.8.3/damona/registry.py
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)    26465 2023-02-21 11:15:46.000000 damona-0.8.3/damona/script.py
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.262055 damona-0.8.3/damona/shell/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2021-09-01 19:41:28.000000 damona-0.8.3/damona/shell/__init__.py
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.263055 damona-0.8.3/damona/shell/bash/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2021-12-30 11:40:38.000000 damona-0.8.3/damona/shell/bash/__init__.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5636 2021-12-30 10:08:08.000000 damona-0.8.3/damona/shell/bash/damona.sh
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      809 2021-09-02 15:44:17.000000 damona-0.8.3/damona/shell/damona_comp.sh
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.263055 damona-0.8.3/damona/shell/fish/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3320 2021-12-30 10:03:26.000000 damona-0.8.3/damona/shell/fish/damona.fish
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.263055 damona-0.8.3/damona/software/
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.263055 damona-0.8.3/damona/software/RIPseeker/
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      983 2023-03-27 15:34:19.000000 damona-0.8.3/damona/software/RIPseeker/Singularity.RIPseeker_1.0.0
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      668 2023-03-22 09:02:18.000000 damona-0.8.3/damona/software/RIPseeker/registry.yaml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2020-08-04 13:32:55.000000 damona-0.8.3/damona/software/__init__.py
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.264055 damona-0.8.3/damona/software/art/
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      296 2021-11-13 18:22:59.000000 damona-0.8.3/damona/software/art/Singularity.art_2.5.8
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      293 2021-11-13 18:23:34.000000 damona-0.8.3/damona/software/art/Singularity.art_3.11.14
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      530 2022-02-22 14:07:33.000000 damona-0.8.3/damona/software/art/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.265055 damona-0.8.3/damona/software/bamtools/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      977 2023-02-17 16:03:17.000000 damona-0.8.3/damona/software/bamtools/Singularity.bamtools_2.5.2
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      286 2022-11-22 08:10:42.000000 damona-0.8.3/damona/software/bamtools/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.265055 damona-0.8.3/damona/software/bbtools/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      439 2021-12-31 14:51:14.000000 damona-0.8.3/damona/software/bbtools/Singularity.bbtools_38.94.0
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3102 2021-12-31 14:58:24.000000 damona-0.8.3/damona/software/bbtools/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.266055 damona-0.8.3/damona/software/bcl2fastq/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      160 2020-08-12 08:05:20.000000 damona-0.8.3/damona/software/bcl2fastq/Makefile
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1140 2021-12-08 13:09:00.000000 damona-0.8.3/damona/software/bcl2fastq/README.rst
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      289 2020-08-11 20:07:37.000000 damona-0.8.3/damona/software/bcl2fastq/Singularity.bcl2fastq_2.20.0
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      298 2021-09-02 16:37:43.000000 damona-0.8.3/damona/software/bcl2fastq/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.267055 damona-0.8.3/damona/software/bedtools/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      955 2022-11-22 09:58:55.000000 damona-0.8.3/damona/software/bedtools/Singularity.bedtools_2.30.0
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      289 2022-11-22 09:54:23.000000 damona-0.8.3/damona/software/bedtools/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.268055 damona-0.8.3/damona/software/bioconvert/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1858 2022-08-30 12:01:29.000000 damona-0.8.3/damona/software/bioconvert/Singularity.bioconvert_0.6.1
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1753 2022-12-21 19:41:04.000000 damona-0.8.3/damona/software/bioconvert/Singularity.bioconvert_0.6.2
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1769 2023-03-07 09:19:34.000000 damona-0.8.3/damona/software/bioconvert/Singularity.bioconvert_0.6.3
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1770 2023-03-07 09:58:04.000000 damona-0.8.3/damona/software/bioconvert/Singularity.bioconvert_1.0.0
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      880 2023-03-07 11:48:52.000000 damona-0.8.3/damona/software/bioconvert/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.268055 damona-0.8.3/damona/software/bowtie/
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      956 2022-11-22 15:10:01.000000 damona-0.8.3/damona/software/bowtie/Singularity.bowtie_1.3.1
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      402 2021-12-30 14:16:40.000000 damona-0.8.3/damona/software/bowtie/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.269055 damona-0.8.3/damona/software/bowtie2/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      918 2021-12-07 22:46:55.000000 damona-0.8.3/damona/software/bowtie2/Singularity.bowtie2_2.3.4
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      912 2021-12-22 18:04:18.000000 damona-0.8.3/damona/software/bowtie2/Singularity.bowtie2_2.4.2
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      606 2021-12-08 13:33:41.000000 damona-0.8.3/damona/software/bowtie2/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.269055 damona-0.8.3/damona/software/busco/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2706 2023-04-06 14:03:40.000000 damona-0.8.3/damona/software/busco/Singularity.busco_5.4.6
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      279 2023-04-06 14:03:40.000000 damona-0.8.3/damona/software/busco/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.270055 damona-0.8.3/damona/software/bwa/
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     1162 2023-03-15 10:44:53.000000 damona-0.8.3/damona/software/bwa/Singularity.bwa_0.7.17
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      256 2023-03-15 10:45:44.000000 damona-0.8.3/damona/software/bwa/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.271055 damona-0.8.3/damona/software/canu/
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      322 2023-04-06 14:05:13.000000 damona-0.8.3/damona/software/canu/Singularity.canu_1.6.0
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      322 2021-12-07 22:29:23.000000 damona-0.8.3/damona/software/canu/Singularity.canu_1.8.0
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      753 2023-04-07 10:00:30.000000 damona-0.8.3/damona/software/canu/Singularity.canu_2.1.1
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      652 2023-04-07 10:04:55.000000 damona-0.8.3/damona/software/canu/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.271055 damona-0.8.3/damona/software/ccs/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      334 2023-04-11 10:33:31.000000 damona-0.8.3/damona/software/ccs/Singularity.ccs_6.4.0
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      271 2023-04-11 10:35:40.000000 damona-0.8.3/damona/software/ccs/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.272055 damona-0.8.3/damona/software/circlator/
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     2779 2023-04-12 13:41:45.000000 damona-0.8.3/damona/software/circlator/Singularity.circlator_1.5.5
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      268 2023-04-12 13:48:17.000000 damona-0.8.3/damona/software/circlator/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.272055 damona-0.8.3/damona/software/falco/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      531 2022-08-22 09:04:26.000000 damona-0.8.3/damona/software/falco/Singularity.falco_0.2.1
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      778 2022-08-22 10:14:18.000000 damona-0.8.3/damona/software/falco/Singularity.falco_1.0.0
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      497 2022-08-22 14:26:58.000000 damona-0.8.3/damona/software/falco/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.273055 damona-0.8.3/damona/software/fastp/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      445 2022-11-14 16:32:09.000000 damona-0.8.3/damona/software/fastp/Singularity.fastp_0.23.2
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      462 2022-11-16 13:29:53.000000 damona-0.8.3/damona/software/fastp/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.274055 damona-0.8.3/damona/software/fastqc/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      522 2020-08-11 20:13:30.000000 damona-0.8.3/damona/software/fastqc/Singularity.fastqc_0.11.8
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      492 2021-02-12 14:59:23.000000 damona-0.8.3/damona/software/fastqc/Singularity.fastqc_0.11.9
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      705 2022-11-22 13:28:06.000000 damona-0.8.3/damona/software/fastqc/Singularity.fastqc_0.11.9_py3
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      658 2022-12-16 09:49:55.000000 damona-0.8.3/damona/software/fastqc/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.274055 damona-0.8.3/damona/software/flye/
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      388 2021-11-26 14:49:41.000000 damona-0.8.3/damona/software/flye/Singularity.flye_2.9.0
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      357 2023-03-14 16:03:34.000000 damona-0.8.3/damona/software/flye/Singularity.flye_2.9.1
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      464 2023-03-15 08:43:07.000000 damona-0.8.3/damona/software/flye/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.275055 damona-0.8.3/damona/software/gffread/
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      601 2020-08-11 20:15:32.000000 damona-0.8.3/damona/software/gffread/Singularity.gffread_0.12.1
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      266 2021-12-22 17:57:32.000000 damona-0.8.3/damona/software/gffread/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.276055 damona-0.8.3/damona/software/graphviz/
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      279 2023-04-11 20:29:23.000000 damona-0.8.3/damona/software/graphviz/Singularity.graphviz_2.43.0
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      289 2021-12-08 13:44:16.000000 damona-0.8.3/damona/software/graphviz/registry.yaml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      183 2021-12-08 13:41:34.000000 damona-0.8.3/damona/software/graphviz/test.dot
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      192 2021-12-22 20:51:22.000000 damona-0.8.3/damona/software/graphviz/test.sh
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.276055 damona-0.8.3/damona/software/gzip/
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      180 2022-08-30 09:44:02.000000 damona-0.8.3/damona/software/gzip/Singularity.gzip_1.9.0
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      280 2022-08-30 09:51:19.000000 damona-0.8.3/damona/software/gzip/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.277055 damona-0.8.3/damona/software/hifiasm/
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      695 2023-03-15 11:04:46.000000 damona-0.8.3/damona/software/hifiasm/Singularity.hifiasm_0.19.1
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      265 2023-03-15 13:49:27.000000 damona-0.8.3/damona/software/hifiasm/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.277055 damona-0.8.3/damona/software/hisat2/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      127 2021-12-22 15:20:09.000000 damona-0.8.3/damona/software/hisat2/README.rst
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      188 2022-01-14 16:44:28.000000 damona-0.8.3/damona/software/hisat2/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.278055 damona-0.8.3/damona/software/homer/
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      482 2022-11-08 20:13:27.000000 damona-0.8.3/damona/software/homer/Singularity.homer_4.11.0
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      297 2022-11-08 20:26:09.000000 damona-0.8.3/damona/software/homer/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.278055 damona-0.8.3/damona/software/idr/
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      699 2022-12-07 21:29:04.000000 damona-0.8.3/damona/software/idr/Singularity.idr_2.0.3
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      272 2022-11-08 19:56:00.000000 damona-0.8.3/damona/software/idr/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.278055 damona-0.8.3/damona/software/igvtools/
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     1367 2022-08-25 09:41:44.000000 damona-0.8.3/damona/software/igvtools/Singularity.igvtools_2.12.0
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      293 2022-08-25 15:40:00.000000 damona-0.8.3/damona/software/igvtools/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.279055 damona-0.8.3/damona/software/kraken/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      140 2020-08-04 13:32:55.000000 damona-0.8.3/damona/software/kraken/Makefile
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      638 2020-08-11 20:16:50.000000 damona-0.8.3/damona/software/kraken/Singularity.kraken_1.1.0
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      904 2020-08-11 20:16:44.000000 damona-0.8.3/damona/software/kraken/Singularity.kraken_2.0.9
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      604 2021-12-23 10:47:17.000000 damona-0.8.3/damona/software/kraken/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.280055 damona-0.8.3/damona/software/mergegi/
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      448 2022-12-09 10:41:16.000000 damona-0.8.3/damona/software/mergegi/Singularity.mergegi_0.0.1
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      291 2022-12-09 10:43:14.000000 damona-0.8.3/damona/software/mergegi/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.281055 damona-0.8.3/damona/software/minimap2/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      681 2021-12-22 17:36:12.000000 damona-0.8.3/damona/software/minimap2/Singularity.minimap2_2.17.0
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      589 2023-04-07 15:31:23.000000 damona-0.8.3/damona/software/minimap2/Singularity.minimap2_2.23.0
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      478 2023-04-11 20:17:17.000000 damona-0.8.3/damona/software/minimap2/Singularity.minimap2_2.24.0
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      675 2023-04-11 13:46:34.000000 damona-0.8.3/damona/software/minimap2/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.281055 damona-0.8.3/damona/software/pbbam/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1062 2023-04-11 10:14:40.000000 damona-0.8.3/damona/software/pbbam/Singularity.pbbam_2.1.0
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1297 2023-04-11 10:14:58.000000 damona-0.8.3/damona/software/pbbam/Singularity.pbbam_2.3.0
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      495 2023-04-11 10:35:46.000000 damona-0.8.3/damona/software/pbbam/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.282055 damona-0.8.3/damona/software/phantompeakqualtools/
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      942 2022-11-07 19:50:54.000000 damona-0.8.3/damona/software/phantompeakqualtools/Singularity.phantompeakqualtools_1.2.2
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      522 2022-11-10 20:11:13.000000 damona-0.8.3/damona/software/phantompeakqualtools/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.282055 damona-0.8.3/damona/software/picard/
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      523 2022-09-20 21:09:49.000000 damona-0.8.3/damona/software/picard/Singularity.picard_2.26
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.282055 damona-0.8.3/damona/software/pigz/
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      185 2022-11-22 10:01:11.000000 damona-0.8.3/damona/software/pigz/Singularity.pigz_2.4.0
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      280 2022-11-22 10:03:15.000000 damona-0.8.3/damona/software/pigz/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.283055 damona-0.8.3/damona/software/polypolish/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      630 2023-03-07 09:07:51.000000 damona-0.8.3/damona/software/polypolish/Singularity.polypolish_0.5.0
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      269 2023-03-07 09:14:59.000000 damona-0.8.3/damona/software/polypolish/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.283055 damona-0.8.3/damona/software/prokka/
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      617 2021-05-05 09:12:20.000000 damona-0.8.3/damona/software/prokka/Singularity.prokka_1.14.5
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      238 2021-11-21 15:26:58.000000 damona-0.8.3/damona/software/prokka/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.284055 damona-0.8.3/damona/software/pycoqc/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      103 2023-03-17 16:01:16.000000 damona-0.8.3/damona/software/pycoqc/Singularity.pycoqc_2.5.2
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      281 2023-03-17 21:36:36.000000 damona-0.8.3/damona/software/pycoqc/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.284055 damona-0.8.3/damona/software/quast/
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      638 2021-11-17 23:21:58.000000 damona-0.8.3/damona/software/quast/Singularity.quast_5.0.2
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      261 2021-12-22 18:38:46.000000 damona-0.8.3/damona/software/quast/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.285055 damona-0.8.3/damona/software/rnadiff/
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      930 2022-12-20 12:52:53.000000 damona-0.8.3/damona/software/rnadiff/Singularity.rnadiff_1.7.1
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      264 2022-12-20 12:53:05.000000 damona-0.8.3/damona/software/rnadiff/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.285055 damona-0.8.3/damona/software/rnaseqc/
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      531 2020-08-25 09:13:07.000000 damona-0.8.3/damona/software/rnaseqc/Singularity.rnaseqc_2.35.0
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      266 2021-12-22 18:39:26.000000 damona-0.8.3/damona/software/rnaseqc/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.286055 damona-0.8.3/damona/software/rtools/
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      406 2021-03-19 14:03:02.000000 damona-0.8.3/damona/software/rtools/Singularity.rtools_1.0.0
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      509 2023-02-17 14:08:13.000000 damona-0.8.3/damona/software/rtools/Singularity.rtools_1.1.0
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      791 2023-02-20 09:57:39.000000 damona-0.8.3/damona/software/rtools/Singularity.rtools_1.2.0
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      668 2023-02-21 22:55:12.000000 damona-0.8.3/damona/software/rtools/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.287055 damona-0.8.3/damona/software/salmon/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      179 2020-08-04 13:32:55.000000 damona-0.8.3/damona/software/salmon/Makefile
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      594 2022-08-30 09:55:04.000000 damona-0.8.3/damona/software/salmon/Singularity.salmon_1.3.0
--rw-rw----   0 cokelaer  (1000) cokelaer  (1000)      281 2022-08-25 15:43:58.000000 damona-0.8.3/damona/software/salmon/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.288055 damona-0.8.3/damona/software/samtools/
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      805 2022-12-14 13:49:36.000000 damona-0.8.3/damona/software/samtools/Singularity.samtools_1.15.0
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      818 2023-04-08 20:18:25.000000 damona-0.8.3/damona/software/samtools/Singularity.samtools_1.16.1
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      482 2022-12-14 14:46:18.000000 damona-0.8.3/damona/software/samtools/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.288055 damona-0.8.3/damona/software/samtools_minimap2/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      906 2023-04-11 13:29:17.000000 damona-0.8.3/damona/software/samtools_minimap2/Singularity.samtools_1.17_minimap2_2.24.0
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      296 2023-04-12 15:46:15.000000 damona-0.8.3/damona/software/samtools_minimap2/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.289055 damona-0.8.3/damona/software/seqkit/
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      548 2023-04-12 13:51:51.000000 damona-0.8.3/damona/software/seqkit/Singularity.seqkit_2.1.0
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      389 2023-04-12 13:51:58.000000 damona-0.8.3/damona/software/seqkit/Singularity.seqkit_2.4.0
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      451 2023-04-12 13:55:18.000000 damona-0.8.3/damona/software/seqkit/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.289055 damona-0.8.3/damona/software/seqtk/
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      498 2021-11-26 14:19:46.000000 damona-0.8.3/damona/software/seqtk/Singularity.seqtk_1.3.0
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      259 2021-11-26 14:07:18.000000 damona-0.8.3/damona/software/seqtk/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.290055 damona-0.8.3/damona/software/sequana/
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     1022 2023-04-06 14:09:18.000000 damona-0.8.3/damona/software/sequana/Singularity.sequana_0.12.6
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     1037 2023-03-14 19:53:08.000000 damona-0.8.3/damona/software/sequana/Singularity.sequana_0.14.6
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      514 2023-03-15 08:42:48.000000 damona-0.8.3/damona/software/sequana/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.291055 damona-0.8.3/damona/software/sequana_denovo/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5201 2023-04-12 14:04:40.000000 damona-0.8.3/damona/software/sequana_denovo/Singularity.sequana_denovo_0.0.2
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      342 2022-11-18 20:00:11.000000 damona-0.8.3/damona/software/sequana_denovo/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.292055 damona-0.8.3/damona/software/sequana_perl_tools/
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      637 2021-05-05 09:13:25.000000 damona-0.8.3/damona/software/sequana_perl_tools/Singularity.sequana_perl_tools_0.1.0
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      644 2022-11-18 15:12:46.000000 damona-0.8.3/damona/software/sequana_perl_tools/Singularity.sequana_perl_tools_0.2.0
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5197 2022-11-18 15:39:03.000000 damona-0.8.3/damona/software/sequana_perl_tools/Singularity.sequana_perl_tools_0.3.0
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      689 2022-11-08 20:04:09.000000 damona-0.8.3/damona/software/sequana_perl_tools/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.292055 damona-0.8.3/damona/software/sequana_ribofinder/
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     1484 2022-11-22 16:28:40.000000 damona-0.8.3/damona/software/sequana_ribofinder/Singularity.sequana_ribofinder_0.12.0
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      288 2022-11-22 16:27:58.000000 damona-0.8.3/damona/software/sequana_ribofinder/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.294055 damona-0.8.3/damona/software/sequana_tools/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      427 2022-11-14 15:42:49.000000 damona-0.8.3/damona/software/sequana_tools/README.txt
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     2156 2021-03-29 14:32:32.000000 damona-0.8.3/damona/software/sequana_tools/Singularity.sequana_tools_0.10.0
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     2242 2021-07-24 20:18:11.000000 damona-0.8.3/damona/software/sequana_tools/Singularity.sequana_tools_0.11.0
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     2241 2022-08-30 09:52:49.000000 damona-0.8.3/damona/software/sequana_tools/Singularity.sequana_tools_0.12.0
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     2338 2022-12-20 15:01:03.000000 damona-0.8.3/damona/software/sequana_tools/Singularity.sequana_tools_0.14.1
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      695 2022-09-21 07:48:13.000000 damona-0.8.3/damona/software/sequana_tools/Singularity.sequana_tools_0.14.2
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      640 2022-09-21 07:45:54.000000 damona-0.8.3/damona/software/sequana_tools/Singularity.sequana_tools_0.14.3
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      366 2023-02-06 10:24:17.000000 damona-0.8.3/damona/software/sequana_tools/Singularity.sequana_tools_0.14.5
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      391 2023-02-06 10:23:27.000000 damona-0.8.3/damona/software/sequana_tools/Singularity.sequana_tools_0.14.6
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     2641 2021-03-19 12:11:02.000000 damona-0.8.3/damona/software/sequana_tools/Singularity.sequana_tools_0.9.0
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5990 2023-04-11 14:46:53.000000 damona-0.8.3/damona/software/sequana_tools/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.295055 damona-0.8.3/damona/software/shustring/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      463 2023-02-21 11:04:27.000000 damona-0.8.3/damona/software/shustring/Singularity.shustring_2.6.0
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      289 2023-02-21 11:44:36.000000 damona-0.8.3/damona/software/shustring/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.295055 damona-0.8.3/damona/software/snpeff/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1185 2022-11-18 20:58:56.000000 damona-0.8.3/damona/software/snpeff/Singularity.snpeff_5.1.0
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.296055 damona-0.8.3/damona/software/trf/
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      891 2021-03-08 19:58:50.000000 damona-0.8.3/damona/software/trf/Singularity.trf_4.10.0
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      198 2021-11-17 22:03:28.000000 damona-0.8.3/damona/software/trf/registry.yaml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.296055 damona-0.8.3/damona/software/ucsc/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       88 2021-12-23 14:08:59.000000 damona-0.8.3/damona/software/ucsc/README.rst
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      521 2022-12-13 15:40:07.000000 damona-0.8.3/damona/software/ucsc/Singularity.ucsc_3.7.7
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      356 2022-12-13 15:23:14.000000 damona-0.8.3/damona/software/ucsc/registry.yaml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    13985 2023-04-10 20:57:40.000000 damona-0.8.3/damona/zenodo.py
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.254055 damona-0.8.3/damona.egg-info/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    17299 2023-04-14 09:55:16.000000 damona-0.8.3/damona.egg-info/PKG-INFO
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     8019 2023-04-14 09:55:16.000000 damona-0.8.3/damona.egg-info/SOURCES.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2023-04-14 09:55:16.000000 damona-0.8.3/damona.egg-info/dependency_links.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       46 2023-04-14 09:55:16.000000 damona-0.8.3/damona.egg-info/entry_points.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2021-09-02 15:44:05.000000 damona-0.8.3/damona.egg-info/not-zip-safe
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      222 2023-04-14 09:55:16.000000 damona-0.8.3/damona.egg-info/requires.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        7 2023-04-14 09:55:16.000000 damona-0.8.3/damona.egg-info/top_level.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       78 2021-12-23 15:50:31.000000 damona-0.8.3/requirements.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      312 2023-04-14 09:55:16.297055 damona-0.8.3/setup.cfg
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4822 2023-04-11 13:45:20.000000 damona-0.8.3/setup.py
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.523929 damona-0.9.0/
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.452928 damona-0.9.0/.github/
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.458928 damona-0.9.0/.github/workflows/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1742 2023-06-19 17:57:20.000000 damona-0.9.0/.github/workflows/bash_test.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1869 2023-06-19 17:57:26.000000 damona-0.9.0/.github/workflows/fish_test.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1591 2023-06-19 17:57:03.000000 damona-0.9.0/.github/workflows/main.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      961 2023-01-10 21:16:10.000000 damona-0.9.0/.github/workflows/pypi.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      976 2021-12-30 10:11:24.000000 damona-0.9.0/.gitignore
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      340 2023-04-11 13:45:36.000000 damona-0.9.0/.readthedocs.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1574 2020-08-25 18:37:15.000000 damona-0.9.0/CONTRIBUTING.rst
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1532 2020-08-10 11:26:10.000000 damona-0.9.0/LICENSE
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      244 2022-01-19 17:14:01.000000 damona-0.9.0/MANIFEST.in
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    17988 2023-06-21 07:35:48.523929 damona-0.9.0/PKG-INFO
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    16749 2023-06-19 17:44:53.000000 damona-0.9.0/README.rst
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.460928 damona-0.9.0/damona/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1481 2022-01-19 10:34:27.000000 damona-0.9.0/damona/__init__.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3217 2023-06-19 17:28:00.000000 damona-0.9.0/damona/admin.py
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.461928 damona-0.9.0/damona/biocontainers/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2022-01-18 11:56:04.000000 damona-0.9.0/damona/biocontainers/__init__.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)  3790743 2023-06-19 16:59:36.000000 damona-0.9.0/damona/biocontainers/registry.yaml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     6105 2021-12-31 09:42:03.000000 damona-0.9.0/damona/builders.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    12881 2023-06-19 17:30:07.000000 damona-0.9.0/damona/common.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5312 2023-06-19 17:25:29.000000 damona-0.9.0/damona/config.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    18858 2023-06-19 17:31:53.000000 damona-0.9.0/damona/environ.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    22745 2023-06-19 17:35:39.000000 damona-0.9.0/damona/install.py
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.467929 damona-0.9.0/damona/library/
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.468928 damona-0.9.0/damona/library/R/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      119 2020-08-04 13:32:55.000000 damona-0.9.0/damona/library/R/Makefile
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     1588 2020-08-11 20:17:37.000000 damona-0.9.0/damona/library/R/Singularity.R_3.6.3
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     1589 2021-03-19 12:22:16.000000 damona-0.9.0/damona/library/R/Singularity.R_4.0.2
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      144 2021-03-19 12:18:31.000000 damona-0.9.0/damona/library/R/registry.yaml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2021-12-29 10:11:19.000000 damona-0.9.0/damona/library/__init__.py
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.469929 damona-0.9.0/damona/library/conda/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      521 2021-12-22 14:56:38.000000 damona-0.9.0/damona/library/conda/README.rst
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2523 2023-06-13 14:09:52.000000 damona-0.9.0/damona/library/conda/Singularity.conda_23.5.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3358 2021-02-22 19:31:08.000000 damona-0.9.0/damona/library/conda/Singularity.conda_4.7.12
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2621 2022-11-08 16:04:03.000000 damona-0.9.0/damona/library/conda/Singularity.conda_4.9.2
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2523 2023-06-13 14:09:13.000000 damona-0.9.0/damona/library/conda/Singularity.conda_4.9.3
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      212 2021-12-22 14:55:56.000000 damona-0.9.0/damona/library/conda/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.470929 damona-0.9.0/damona/library/micromamba/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      593 2023-06-13 21:38:30.000000 damona-0.9.0/damona/library/micromamba/Singularity.micromamba_1.4.3
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      269 2023-06-13 21:39:02.000000 damona-0.9.0/damona/library/micromamba/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.470929 damona-0.9.0/damona/library/rust/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      272 2022-08-26 07:32:05.000000 damona-0.9.0/damona/library/rust/Singularity.rust
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.471928 damona-0.9.0/damona/library/ubuntu/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      724 2021-09-02 15:44:16.000000 damona-0.9.0/damona/library/ubuntu/Singularity.ubuntu_16.04
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3391 2021-09-02 15:44:16.000000 damona-0.9.0/damona/library/ubuntu/Singularity.ubuntu_18.04
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      166 2021-09-02 15:44:16.000000 damona-0.9.0/damona/library/ubuntu/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.471928 damona-0.9.0/damona/papers/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2022-01-19 11:53:53.000000 damona-0.9.0/damona/papers/__init__.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    16085 2023-06-19 17:25:29.000000 damona-0.9.0/damona/registry.py
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)    28038 2023-06-19 17:48:45.000000 damona-0.9.0/damona/script.py
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.471928 damona-0.9.0/damona/shell/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2021-09-01 19:41:28.000000 damona-0.9.0/damona/shell/__init__.py
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.472929 damona-0.9.0/damona/shell/bash/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2021-12-30 11:40:38.000000 damona-0.9.0/damona/shell/bash/__init__.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5636 2021-12-30 10:08:08.000000 damona-0.9.0/damona/shell/bash/damona.sh
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      809 2021-09-02 15:44:17.000000 damona-0.9.0/damona/shell/damona_comp.sh
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.472929 damona-0.9.0/damona/shell/fish/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3320 2021-12-30 10:03:26.000000 damona-0.9.0/damona/shell/fish/damona.fish
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.472929 damona-0.9.0/damona/software/
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.473929 damona-0.9.0/damona/software/RIPseeker/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      983 2023-03-27 15:34:19.000000 damona-0.9.0/damona/software/RIPseeker/Singularity.RIPseeker_1.0.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      668 2023-03-22 09:02:18.000000 damona-0.9.0/damona/software/RIPseeker/registry.yaml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2020-08-04 13:32:55.000000 damona-0.9.0/damona/software/__init__.py
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.473929 damona-0.9.0/damona/software/art/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      296 2021-11-13 18:22:59.000000 damona-0.9.0/damona/software/art/Singularity.art_2.5.8
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      293 2021-11-13 18:23:34.000000 damona-0.9.0/damona/software/art/Singularity.art_3.11.14
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      530 2022-02-22 14:07:33.000000 damona-0.9.0/damona/software/art/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.474928 damona-0.9.0/damona/software/bamtools/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      977 2023-02-17 16:03:17.000000 damona-0.9.0/damona/software/bamtools/Singularity.bamtools_2.5.2
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      286 2022-11-22 08:10:42.000000 damona-0.9.0/damona/software/bamtools/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.474928 damona-0.9.0/damona/software/bbtools/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      439 2021-12-31 14:51:14.000000 damona-0.9.0/damona/software/bbtools/Singularity.bbtools_38.94.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3102 2021-12-31 14:58:24.000000 damona-0.9.0/damona/software/bbtools/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.475929 damona-0.9.0/damona/software/bcl2fastq/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1139 2023-05-17 11:26:53.000000 damona-0.9.0/damona/software/bcl2fastq/README.rst
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      289 2020-08-11 20:07:37.000000 damona-0.9.0/damona/software/bcl2fastq/Singularity.bcl2fastq_2.20.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      298 2021-09-02 16:37:43.000000 damona-0.9.0/damona/software/bcl2fastq/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.476929 damona-0.9.0/damona/software/bedtools/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      955 2022-11-22 09:58:55.000000 damona-0.9.0/damona/software/bedtools/Singularity.bedtools_2.30.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      289 2022-11-22 09:54:23.000000 damona-0.9.0/damona/software/bedtools/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.477928 damona-0.9.0/damona/software/bioconvert/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1858 2022-08-30 12:01:29.000000 damona-0.9.0/damona/software/bioconvert/Singularity.bioconvert_0.6.1
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1753 2022-12-21 19:41:04.000000 damona-0.9.0/damona/software/bioconvert/Singularity.bioconvert_0.6.2
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1769 2023-03-07 09:19:34.000000 damona-0.9.0/damona/software/bioconvert/Singularity.bioconvert_0.6.3
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1770 2023-03-07 09:58:04.000000 damona-0.9.0/damona/software/bioconvert/Singularity.bioconvert_1.0.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      880 2023-03-07 11:48:52.000000 damona-0.9.0/damona/software/bioconvert/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.478929 damona-0.9.0/damona/software/blast/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      120 2023-04-17 18:12:34.000000 damona-0.9.0/damona/software/blast/Singularity.blast_2.12.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      261 2023-04-21 08:53:43.000000 damona-0.9.0/damona/software/blast/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.478929 damona-0.9.0/damona/software/bowtie/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      956 2022-11-22 15:10:01.000000 damona-0.9.0/damona/software/bowtie/Singularity.bowtie_1.3.1
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      402 2021-12-30 14:16:40.000000 damona-0.9.0/damona/software/bowtie/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.479929 damona-0.9.0/damona/software/bowtie2/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      918 2021-12-07 22:46:55.000000 damona-0.9.0/damona/software/bowtie2/Singularity.bowtie2_2.3.4
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      912 2021-12-22 18:04:18.000000 damona-0.9.0/damona/software/bowtie2/Singularity.bowtie2_2.4.2
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      606 2021-12-08 13:33:41.000000 damona-0.9.0/damona/software/bowtie2/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.479929 damona-0.9.0/damona/software/busco/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2706 2023-06-12 12:53:00.000000 damona-0.9.0/damona/software/busco/Singularity.busco_5.4.6
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      279 2023-04-06 14:03:40.000000 damona-0.9.0/damona/software/busco/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.480929 damona-0.9.0/damona/software/bwa/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     1167 2023-05-25 10:26:00.000000 damona-0.9.0/damona/software/bwa/Singularity.bwa_0.7.17
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      617 2023-06-14 12:11:50.000000 damona-0.9.0/damona/software/bwa/Singularity.bwa_mamba_0.7.17
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      256 2023-05-25 10:28:05.000000 damona-0.9.0/damona/software/bwa/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.481929 damona-0.9.0/damona/software/canu/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      322 2023-04-06 14:05:13.000000 damona-0.9.0/damona/software/canu/Singularity.canu_1.6.0
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      322 2021-12-07 22:29:23.000000 damona-0.9.0/damona/software/canu/Singularity.canu_1.8.0
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      765 2023-04-24 20:10:11.000000 damona-0.9.0/damona/software/canu/Singularity.canu_2.1.1
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      653 2023-04-26 10:13:04.000000 damona-0.9.0/damona/software/canu/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.482929 damona-0.9.0/damona/software/ccs/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      334 2023-04-11 10:33:31.000000 damona-0.9.0/damona/software/ccs/Singularity.ccs_6.4.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      271 2023-04-11 10:35:40.000000 damona-0.9.0/damona/software/ccs/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.482929 damona-0.9.0/damona/software/cellranger/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1220 2023-06-09 21:44:26.000000 damona-0.9.0/damona/software/cellranger/Singularity.cellranger_7.1.0
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.483929 damona-0.9.0/damona/software/circlator/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     2779 2023-04-12 13:41:45.000000 damona-0.9.0/damona/software/circlator/Singularity.circlator_1.5.5
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      268 2023-04-12 13:48:17.000000 damona-0.9.0/damona/software/circlator/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.483929 damona-0.9.0/damona/software/falco/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      531 2022-08-22 09:04:26.000000 damona-0.9.0/damona/software/falco/Singularity.falco_0.2.1
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      778 2022-08-22 10:14:18.000000 damona-0.9.0/damona/software/falco/Singularity.falco_1.0.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      497 2022-08-22 14:26:58.000000 damona-0.9.0/damona/software/falco/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.484929 damona-0.9.0/damona/software/fastp/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      445 2022-11-14 16:32:09.000000 damona-0.9.0/damona/software/fastp/Singularity.fastp_0.23.2
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      445 2023-05-29 21:59:06.000000 damona-0.9.0/damona/software/fastp/Singularity.fastp_0.23.3
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      470 2023-06-14 07:53:48.000000 damona-0.9.0/damona/software/fastp/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.486929 damona-0.9.0/damona/software/fastqc/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      522 2020-08-11 20:13:30.000000 damona-0.9.0/damona/software/fastqc/Singularity.fastqc_0.11.8
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      492 2021-02-12 14:59:23.000000 damona-0.9.0/damona/software/fastqc/Singularity.fastqc_0.11.9
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      705 2023-05-11 07:15:16.000000 damona-0.9.0/damona/software/fastqc/Singularity.fastqc_0.11.9_py3
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      728 2023-05-11 08:00:01.000000 damona-0.9.0/damona/software/fastqc/Singularity.fastqc_0.12.1
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      850 2023-05-11 08:02:49.000000 damona-0.9.0/damona/software/fastqc/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.487929 damona-0.9.0/damona/software/flye/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      388 2021-11-26 14:49:41.000000 damona-0.9.0/damona/software/flye/Singularity.flye_2.9.0
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      357 2023-03-14 16:03:34.000000 damona-0.9.0/damona/software/flye/Singularity.flye_2.9.1
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      464 2023-03-15 08:43:07.000000 damona-0.9.0/damona/software/flye/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.487929 damona-0.9.0/damona/software/gffread/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      601 2020-08-11 20:15:32.000000 damona-0.9.0/damona/software/gffread/Singularity.gffread_0.12.1
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      625 2023-06-14 09:27:12.000000 damona-0.9.0/damona/software/gffread/Singularity.gffread_0.12.7
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      480 2023-06-14 09:56:44.000000 damona-0.9.0/damona/software/gffread/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.489929 damona-0.9.0/damona/software/graphviz/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      279 2023-05-11 20:09:49.000000 damona-0.9.0/damona/software/graphviz/Singularity.graphviz_2.43.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       98 2023-05-12 07:59:37.000000 damona-0.9.0/damona/software/graphviz/Singularity.graphviz_7.0.5
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      679 2023-05-12 08:00:47.000000 damona-0.9.0/damona/software/graphviz/registry.yaml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      183 2021-12-08 13:41:34.000000 damona-0.9.0/damona/software/graphviz/test.dot
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      192 2021-12-22 20:51:22.000000 damona-0.9.0/damona/software/graphviz/test.sh
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.489929 damona-0.9.0/damona/software/gzip/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      180 2022-08-30 09:44:02.000000 damona-0.9.0/damona/software/gzip/Singularity.gzip_1.9.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      280 2022-08-30 09:51:19.000000 damona-0.9.0/damona/software/gzip/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.490929 damona-0.9.0/damona/software/hifiasm/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      695 2023-03-15 11:04:46.000000 damona-0.9.0/damona/software/hifiasm/Singularity.hifiasm_0.19.1
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      265 2023-03-15 13:49:27.000000 damona-0.9.0/damona/software/hifiasm/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.490929 damona-0.9.0/damona/software/hisat2/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      127 2021-12-22 15:20:09.000000 damona-0.9.0/damona/software/hisat2/README.rst
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      188 2022-01-14 16:44:28.000000 damona-0.9.0/damona/software/hisat2/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.491929 damona-0.9.0/damona/software/homer/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      482 2022-11-08 20:13:27.000000 damona-0.9.0/damona/software/homer/Singularity.homer_4.11.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      297 2022-11-08 20:26:09.000000 damona-0.9.0/damona/software/homer/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.492929 damona-0.9.0/damona/software/idr/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      699 2022-12-07 21:29:04.000000 damona-0.9.0/damona/software/idr/Singularity.idr_2.0.3
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      272 2022-11-08 19:56:00.000000 damona-0.9.0/damona/software/idr/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.494929 damona-0.9.0/damona/software/igvtools/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     1367 2022-08-25 09:41:44.000000 damona-0.9.0/damona/software/igvtools/Singularity.igvtools_2.12.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      293 2022-08-25 15:40:00.000000 damona-0.9.0/damona/software/igvtools/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.495929 damona-0.9.0/damona/software/ivar/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     1323 2023-06-13 11:41:32.000000 damona-0.9.0/damona/software/ivar/Singularity.ivar_1.3.1
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      275 2023-06-14 09:58:11.000000 damona-0.9.0/damona/software/ivar/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.498929 damona-0.9.0/damona/software/kraken/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      140 2020-08-04 13:32:55.000000 damona-0.9.0/damona/software/kraken/Makefile
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      638 2020-08-11 20:16:50.000000 damona-0.9.0/damona/software/kraken/Singularity.kraken_1.1.0
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      904 2023-06-14 09:40:06.000000 damona-0.9.0/damona/software/kraken/Singularity.kraken_2.0.9
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      604 2021-12-23 10:47:17.000000 damona-0.9.0/damona/software/kraken/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.499929 damona-0.9.0/damona/software/mafft/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      623 2023-06-14 09:43:00.000000 damona-0.9.0/damona/software/mafft/Singularity.mafft_7.520.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      282 2023-06-14 09:52:45.000000 damona-0.9.0/damona/software/mafft/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.500929 damona-0.9.0/damona/software/medaka/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1800 2023-04-17 18:12:34.000000 damona-0.9.0/damona/software/medaka/Singularity.medaka_1.7.3
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      263 2023-04-21 08:53:43.000000 damona-0.9.0/damona/software/medaka/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.501929 damona-0.9.0/damona/software/mergegi/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      448 2022-12-09 10:41:16.000000 damona-0.9.0/damona/software/mergegi/Singularity.mergegi_0.0.1
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      291 2022-12-09 10:43:14.000000 damona-0.9.0/damona/software/mergegi/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.503929 damona-0.9.0/damona/software/minimap2/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      681 2021-12-22 17:36:12.000000 damona-0.9.0/damona/software/minimap2/Singularity.minimap2_2.17.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      589 2023-04-07 15:31:23.000000 damona-0.9.0/damona/software/minimap2/Singularity.minimap2_2.23.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      478 2023-04-11 20:17:17.000000 damona-0.9.0/damona/software/minimap2/Singularity.minimap2_2.24.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      675 2023-04-11 13:46:34.000000 damona-0.9.0/damona/software/minimap2/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.504929 damona-0.9.0/damona/software/nextclade/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      720 2023-06-13 15:34:30.000000 damona-0.9.0/damona/software/nextclade/Singularity.nextclade_2.15.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      292 2023-06-14 09:58:00.000000 damona-0.9.0/damona/software/nextclade/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.505929 damona-0.9.0/damona/software/pangolin/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      534 2023-06-14 09:57:32.000000 damona-0.9.0/damona/software/pangolin/Singularity.pangolin_4.3.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      287 2023-06-14 09:57:39.000000 damona-0.9.0/damona/software/pangolin/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.505929 damona-0.9.0/damona/software/pbbam/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1062 2023-04-11 10:14:40.000000 damona-0.9.0/damona/software/pbbam/Singularity.pbbam_2.1.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1297 2023-04-11 10:14:58.000000 damona-0.9.0/damona/software/pbbam/Singularity.pbbam_2.3.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      495 2023-04-11 10:35:46.000000 damona-0.9.0/damona/software/pbbam/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.505929 damona-0.9.0/damona/software/phantompeakqualtools/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      942 2022-11-07 19:50:54.000000 damona-0.9.0/damona/software/phantompeakqualtools/Singularity.phantompeakqualtools_1.2.2
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      522 2022-11-10 20:11:13.000000 damona-0.9.0/damona/software/phantompeakqualtools/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.506929 damona-0.9.0/damona/software/picard/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      523 2022-09-20 21:09:49.000000 damona-0.9.0/damona/software/picard/Singularity.picard_2.26
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.506929 damona-0.9.0/damona/software/pigz/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      185 2022-11-22 10:01:11.000000 damona-0.9.0/damona/software/pigz/Singularity.pigz_2.4.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      280 2022-11-22 10:03:15.000000 damona-0.9.0/damona/software/pigz/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.507929 damona-0.9.0/damona/software/polypolish/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      630 2023-03-07 09:07:51.000000 damona-0.9.0/damona/software/polypolish/Singularity.polypolish_0.5.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      269 2023-03-07 09:14:59.000000 damona-0.9.0/damona/software/polypolish/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.507929 damona-0.9.0/damona/software/prokka/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      617 2021-05-05 09:12:20.000000 damona-0.9.0/damona/software/prokka/Singularity.prokka_1.14.5
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2099 2023-05-17 20:41:38.000000 damona-0.9.0/damona/software/prokka/Singularity.prokka_1.14.6
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      684 2023-05-17 20:57:00.000000 damona-0.9.0/damona/software/prokka/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.508929 damona-0.9.0/damona/software/pycoqc/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      103 2023-03-17 16:01:16.000000 damona-0.9.0/damona/software/pycoqc/Singularity.pycoqc_2.5.2
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      281 2023-03-17 21:36:36.000000 damona-0.9.0/damona/software/pycoqc/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.508929 damona-0.9.0/damona/software/quast/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      638 2023-04-19 20:15:13.000000 damona-0.9.0/damona/software/quast/Singularity.quast_5.0.2
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1797 2023-04-21 08:53:43.000000 damona-0.9.0/damona/software/quast/Singularity.quast_5.2.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      450 2023-04-21 08:53:43.000000 damona-0.9.0/damona/software/quast/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.509929 damona-0.9.0/damona/software/raxml/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      648 2023-05-24 13:57:04.000000 damona-0.9.0/damona/software/raxml/Singularity.raxml_8.2.12
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      375 2023-05-24 20:47:42.000000 damona-0.9.0/damona/software/raxml/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.509929 damona-0.9.0/damona/software/rnadiff/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      930 2022-12-20 12:52:53.000000 damona-0.9.0/damona/software/rnadiff/Singularity.rnadiff_1.7.1
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      264 2022-12-20 12:53:05.000000 damona-0.9.0/damona/software/rnadiff/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.510929 damona-0.9.0/damona/software/rnaseqc/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      531 2020-08-25 09:13:07.000000 damona-0.9.0/damona/software/rnaseqc/Singularity.rnaseqc_2.35.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      266 2021-12-22 18:39:26.000000 damona-0.9.0/damona/software/rnaseqc/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.511929 damona-0.9.0/damona/software/rtools/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      406 2021-03-19 14:03:02.000000 damona-0.9.0/damona/software/rtools/Singularity.rtools_1.0.0
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      509 2023-02-17 14:08:13.000000 damona-0.9.0/damona/software/rtools/Singularity.rtools_1.1.0
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      791 2023-02-20 09:57:39.000000 damona-0.9.0/damona/software/rtools/Singularity.rtools_1.2.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      668 2023-02-21 22:55:12.000000 damona-0.9.0/damona/software/rtools/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.512929 damona-0.9.0/damona/software/salmon/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      179 2020-08-04 13:32:55.000000 damona-0.9.0/damona/software/salmon/Makefile
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      594 2022-08-30 09:55:04.000000 damona-0.9.0/damona/software/salmon/Singularity.salmon_1.3.0
+-rw-rw----   0 cokelaer  (1000) cokelaer  (1000)      281 2022-08-25 15:43:58.000000 damona-0.9.0/damona/software/salmon/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.512929 damona-0.9.0/damona/software/samtools/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      805 2022-12-14 13:49:36.000000 damona-0.9.0/damona/software/samtools/Singularity.samtools_1.15.0
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      818 2023-04-08 20:18:25.000000 damona-0.9.0/damona/software/samtools/Singularity.samtools_1.16.1
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      482 2022-12-14 14:46:18.000000 damona-0.9.0/damona/software/samtools/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.513929 damona-0.9.0/damona/software/samtools_minimap2/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      916 2023-05-30 22:01:36.000000 damona-0.9.0/damona/software/samtools_minimap2/Singularity.samtools_1.17_minimap2_2.24.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      296 2023-05-30 22:06:01.000000 damona-0.9.0/damona/software/samtools_minimap2/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.514929 damona-0.9.0/damona/software/seqkit/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      548 2023-06-13 12:56:43.000000 damona-0.9.0/damona/software/seqkit/Singularity.seqkit_2.1.0
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      389 2023-05-17 13:57:14.000000 damona-0.9.0/damona/software/seqkit/Singularity.seqkit_2.4.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      451 2023-04-12 13:55:18.000000 damona-0.9.0/damona/software/seqkit/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.514929 damona-0.9.0/damona/software/seqtk/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      498 2021-11-26 14:19:46.000000 damona-0.9.0/damona/software/seqtk/Singularity.seqtk_1.3.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      259 2021-11-26 14:07:18.000000 damona-0.9.0/damona/software/seqtk/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.515929 damona-0.9.0/damona/software/sequana/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     1022 2023-04-06 14:09:18.000000 damona-0.9.0/damona/software/sequana/Singularity.sequana_0.12.6
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     1037 2023-03-14 19:53:08.000000 damona-0.9.0/damona/software/sequana/Singularity.sequana_0.14.6
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      977 2023-04-25 14:31:48.000000 damona-0.9.0/damona/software/sequana/Singularity.sequana_0.15.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      708 2023-04-25 14:40:41.000000 damona-0.9.0/damona/software/sequana/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.515929 damona-0.9.0/damona/software/sequana_denovo/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5201 2023-05-17 12:54:13.000000 damona-0.9.0/damona/software/sequana_denovo/Singularity.sequana_denovo_0.0.2
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      342 2022-11-18 20:00:11.000000 damona-0.9.0/damona/software/sequana_denovo/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.516929 damona-0.9.0/damona/software/sequana_minimal/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      931 2023-06-14 10:00:41.000000 damona-0.9.0/damona/software/sequana_minimal/Singularity.sequana_minimal_23.6.13
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      855 2023-06-14 10:20:01.000000 damona-0.9.0/damona/software/sequana_minimal/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.517929 damona-0.9.0/damona/software/sequana_perl_tools/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      637 2021-05-05 09:13:25.000000 damona-0.9.0/damona/software/sequana_perl_tools/Singularity.sequana_perl_tools_0.1.0
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      644 2022-11-18 15:12:46.000000 damona-0.9.0/damona/software/sequana_perl_tools/Singularity.sequana_perl_tools_0.2.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5197 2022-11-18 15:39:03.000000 damona-0.9.0/damona/software/sequana_perl_tools/Singularity.sequana_perl_tools_0.3.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      689 2022-11-08 20:04:09.000000 damona-0.9.0/damona/software/sequana_perl_tools/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.517929 damona-0.9.0/damona/software/sequana_ribofinder/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     1484 2023-05-25 07:41:58.000000 damona-0.9.0/damona/software/sequana_ribofinder/Singularity.sequana_ribofinder_0.12.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      288 2022-11-22 16:27:58.000000 damona-0.9.0/damona/software/sequana_ribofinder/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.520929 damona-0.9.0/damona/software/sequana_tools/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      620 2023-05-23 19:57:44.000000 damona-0.9.0/damona/software/sequana_tools/README.txt
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     2156 2023-06-14 08:25:31.000000 damona-0.9.0/damona/software/sequana_tools/Singularity.sequana_tools_0.10.0
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     2242 2021-07-24 20:18:11.000000 damona-0.9.0/damona/software/sequana_tools/Singularity.sequana_tools_0.11.0
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     2241 2022-08-30 09:52:49.000000 damona-0.9.0/damona/software/sequana_tools/Singularity.sequana_tools_0.12.0
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     2338 2022-12-20 15:01:03.000000 damona-0.9.0/damona/software/sequana_tools/Singularity.sequana_tools_0.14.1
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      695 2022-09-21 07:48:13.000000 damona-0.9.0/damona/software/sequana_tools/Singularity.sequana_tools_0.14.2
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      640 2023-05-23 18:05:09.000000 damona-0.9.0/damona/software/sequana_tools/Singularity.sequana_tools_0.14.3
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      366 2023-05-23 18:00:44.000000 damona-0.9.0/damona/software/sequana_tools/Singularity.sequana_tools_0.14.5
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      428 2023-05-23 19:57:57.000000 damona-0.9.0/damona/software/sequana_tools/Singularity.sequana_tools_0.15.1
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     2641 2021-03-19 12:11:02.000000 damona-0.9.0/damona/software/sequana_tools/Singularity.sequana_tools_0.9.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2021 2023-06-14 09:14:17.000000 damona-0.9.0/damona/software/sequana_tools/Singularity.sequana_tools_23.6.13
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     6190 2023-05-23 20:01:46.000000 damona-0.9.0/damona/software/sequana_tools/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.520929 damona-0.9.0/damona/software/shustring/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      463 2023-06-14 09:56:11.000000 damona-0.9.0/damona/software/shustring/Singularity.shustring_2.6.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      289 2023-06-14 09:56:09.000000 damona-0.9.0/damona/software/shustring/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.521929 damona-0.9.0/damona/software/snpeff/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1188 2023-05-23 15:04:07.000000 damona-0.9.0/damona/software/snpeff/Singularity.snpeff_5.0.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1189 2023-05-23 14:58:11.000000 damona-0.9.0/damona/software/snpeff/Singularity.snpeff_5.1.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      452 2023-05-23 16:13:17.000000 damona-0.9.0/damona/software/snpeff/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.521929 damona-0.9.0/damona/software/subread/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      632 2023-06-14 09:53:36.000000 damona-0.9.0/damona/software/subread/Singularity.subread_2.0.3
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      341 2023-06-14 09:55:49.000000 damona-0.9.0/damona/software/subread/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.522929 damona-0.9.0/damona/software/trf/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      891 2021-03-08 19:58:50.000000 damona-0.9.0/damona/software/trf/Singularity.trf_4.10.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      198 2021-11-17 22:03:28.000000 damona-0.9.0/damona/software/trf/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.522929 damona-0.9.0/damona/software/ucsc/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       88 2021-12-23 14:08:59.000000 damona-0.9.0/damona/software/ucsc/README.rst
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      521 2022-12-13 15:40:07.000000 damona-0.9.0/damona/software/ucsc/Singularity.ucsc_3.7.7
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      356 2022-12-13 15:23:14.000000 damona-0.9.0/damona/software/ucsc/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.523929 damona-0.9.0/damona/software/vt/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      630 2023-06-14 09:58:58.000000 damona-0.9.0/damona/software/vt/Singularity.vt_0.57721.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      277 2023-05-25 09:29:38.000000 damona-0.9.0/damona/software/vt/registry.yaml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1353 2023-06-19 17:35:31.000000 damona-0.9.0/damona/utils.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    14927 2023-06-19 17:25:29.000000 damona-0.9.0/damona/zenodo.py
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-06-21 07:35:48.461928 damona-0.9.0/damona.egg-info/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    17988 2023-06-21 07:35:48.000000 damona-0.9.0/damona.egg-info/PKG-INFO
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     9664 2023-06-21 07:35:48.000000 damona-0.9.0/damona.egg-info/SOURCES.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2023-06-21 07:35:48.000000 damona-0.9.0/damona.egg-info/dependency_links.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       46 2023-06-21 07:35:48.000000 damona-0.9.0/damona.egg-info/entry_points.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2021-09-02 15:44:05.000000 damona-0.9.0/damona.egg-info/not-zip-safe
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      236 2023-06-21 07:35:48.000000 damona-0.9.0/damona.egg-info/requires.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        7 2023-06-21 07:35:48.000000 damona-0.9.0/damona.egg-info/top_level.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       92 2023-06-19 17:52:20.000000 damona-0.9.0/requirements.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      312 2023-06-21 07:35:48.523929 damona-0.9.0/setup.cfg
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4771 2023-06-19 17:41:04.000000 damona-0.9.0/setup.py
```

### Comparing `damona-0.8.3/.github/workflows/bash_test.yml` & `damona-0.9.0/.github/workflows/bash_test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
       run: |
         bash
         damona 
         echo " source ~/.config/damona/damona.sh" >> ~/.bashrc
     - name: Test installation hisat2
       run: |
         #source /home/runner/.config/damona/damona.sh
-        damona env --create TEST
+        damona create TEST
         damona activate TEST
         damona install hisat2  # a docker file
         damona install fastqc  # a zenodo/damona file
         damona install minimap2  # a zenodo/damona file
         damona deactivate
       env:
         DAMONA_EXE: /usr/share/miniconda/bin/damona
```

### Comparing `damona-0.8.3/.github/workflows/fish_test.yml` & `damona-0.9.0/.github/workflows/fish_test.yml`

 * *Files 6% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         mkdir -p ~/.config/fish
         echo "source ~/.config/damona/damona.fish" >> ~/.config/fish/config.fish
     - name: Test installation hisat2
       run: |
         which fish
         cat << EOF > test.fish
         #!/usr/bin/fish
-        damona env --create TEST
+        damona create TEST
         damona activate TEST
         damona install hisat2
         damona install fastqc
         damona deactivate
         EOF
         cat test.fish
         `(fish test.fish)`
```

### Comparing `damona-0.8.3/.github/workflows/main.yml` & `damona-0.9.0/.github/workflows/main.yml`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 jobs:
   build-linux:
     runs-on: ubuntu-20.04
     strategy:
       max-parallel: 5
       matrix:
-        python: [3.7, 3.8, 3.9]
+        python: [3.8, 3.9, '3.10']
       fail-fast: false
 
     steps:
 
     - name: precleanup
       run: |
         sudo rm -rf /usr/share/dotnet
@@ -55,15 +55,15 @@
         python-version: ${{ matrix.python }}
 
     - name: Install Damona using pip
       run: |
         pip install .[testing]
     - name: Test with pytest
       run: |
-        damona env --create damona__testing__
+        damona create damona__testing__
         pytest --cov-report term --cov=damona
       env:
         DAMONA_EXE: /usr/share/miniconda/bin/damona
         DAMONA_PATH: /home/runner/.config/damona
     - name: coveralls
       run: |
         coveralls --service=github
```

### Comparing `damona-0.8.3/.github/workflows/pypi.yml` & `damona-0.9.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/.gitignore` & `damona-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/CONTRIBUTING.rst` & `damona-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/LICENSE` & `damona-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/PKG-INFO` & `damona-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: damona
-Version: 0.8.3
+Version: 0.9.0
 Summary: A set of NGS singularity recipes, built for you and easily downlable
 Home-page: http://github.com/sequana/sequana
-Download-URL: https://github.com/sequana/sequana/archive/0.8.3.tar.gz
+Download-URL: https://github.com/sequana/sequana/archive/0.9.0.tar.gz
 Author: Thomas Cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: Thomas Cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
 Keywords: NGS,singularity
 Platform: Linux
 Platform: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
@@ -48,15 +47,15 @@
     :target: http://damona.readthedocs.org/en/latest/?badge=latest
     :alt: Documentation Status
 
 .. image:: https://zenodo.org/badge/282275608.svg
    :target: https://zenodo.org/badge/latestdoi/282275608
 
 
-:Python version: Python 3.7, 3.8, 3.9
+:Python version: Python 3.8, 3.9, 3.10
 :Source: See  `http://github.com/cokelaer/damona <https://github.com/cokelaer/damona/>`__.
 :Issues: Please fill a report on `github <https://github.com/cokelaer/damona/issues>`__
 :Platform: This is currently only available for Linux distribution with bash shell (contributions are welcome to port the tool on MacOSX and other platforms)
 
 Overview
 ========
 
@@ -68,14 +67,15 @@
 Damona is now used in production to create reproducible environments where singularity images and their associated binaries are installed altogether.
 
 In a nutshell, Damona combines the logic of Conda environments with the
 reproducibility of singularity containers. We believe that it could be useful for
 other projects and therefore decided to release it as an independent tool.
 
 As of 30th Dec 2021, **Damona** contains 26 software, 38 releases, 105 binaries.
+As of 12th May 2023, **Damona** contains 54 software, 88 releases, 359 binaries.
 
 Installation
 ============
 
 If you are in a hurry, just type::
 
     pip install damona --upgrade
@@ -246,15 +246,15 @@
 
     damona env
 
 2. *create* environments
 ------------------------
 All environments are stored in *~/.config/damona/envs/*. You can create a new one as follows::
 
-    damona env --create TEST
+    damona create TEST
 
 There, you have a *bin* directory where binaries are going to be installed.
 
 You can check that it has been created::
 
     damona env
 
@@ -345,15 +345,15 @@
 
 7. combine two different environments
 --------------------------------------
 
 In damona, you can have sereral environments in parallel and later activate the
 one you wish to use. Let us create a new one::
 
-    damone env --create test1
+    damone create test1
 
 and check that you now have one more environment::
 
     damona env
 
 We want to create an alias to the previously downloaded image of fastqc tool but
 in the *test1* environment. First we activate the newly create environment::
@@ -378,14 +378,24 @@
 
 Changelog
 =========
 
 ========= ========================================================================
 Version   Description
 ========= ========================================================================
+0.9.0     * refactorise the command 'env' by splitting into dedicated subcommands
+            create, delete, rename. add progress bar when downloading container
+          * NEW micromamba image to work as a localimage
+          * NEW sequana_minimal package to hold common tools (bwa, samtools,
+            kraken, etc)
+          * NEW ivarm pangolin, nextclade, subread, mafft packages
+          * UPDATE fastp to 0.23.3, gffread to 0.12.7 (3 times lighter).
+          * UPDATE sequana_tools to use micromamba (30% lighter)
+0.8.4     * fix damona stats command to return unique binaries
+          * more recipes and version (e.g. fastqc 0.12.1, graphviz update, etc)
 0.8.3     * create registry specifically for the sandbox (for testing)
           * add damona community in the uploads
           * add pbbam, bioconvert, busco, canu, ccs
           * add polypolish, samtools 1.16.1, sequana 0.14.6, flye 2.9, canu 2.1.1
             circlator 1.5.5, hifiasm
 0.8.2     * add idr, samtools, homer, bamtools, bedtools, sequana_denovo
           * add seqkit recipe and container
```

### Comparing `damona-0.8.3/README.rst` & `damona-0.9.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     :target: http://damona.readthedocs.org/en/latest/?badge=latest
     :alt: Documentation Status
 
 .. image:: https://zenodo.org/badge/282275608.svg
    :target: https://zenodo.org/badge/latestdoi/282275608
 
 
-:Python version: Python 3.7, 3.8, 3.9
+:Python version: Python 3.8, 3.9, 3.10
 :Source: See  `http://github.com/cokelaer/damona <https://github.com/cokelaer/damona/>`__.
 :Issues: Please fill a report on `github <https://github.com/cokelaer/damona/issues>`__
 :Platform: This is currently only available for Linux distribution with bash shell (contributions are welcome to port the tool on MacOSX and other platforms)
 
 Overview
 ========
 
@@ -36,14 +36,15 @@
 Damona is now used in production to create reproducible environments where singularity images and their associated binaries are installed altogether.
 
 In a nutshell, Damona combines the logic of Conda environments with the
 reproducibility of singularity containers. We believe that it could be useful for
 other projects and therefore decided to release it as an independent tool.
 
 As of 30th Dec 2021, **Damona** contains 26 software, 38 releases, 105 binaries.
+As of 12th May 2023, **Damona** contains 54 software, 88 releases, 359 binaries.
 
 Installation
 ============
 
 If you are in a hurry, just type::
 
     pip install damona --upgrade
@@ -214,15 +215,15 @@
 
     damona env
 
 2. *create* environments
 ------------------------
 All environments are stored in *~/.config/damona/envs/*. You can create a new one as follows::
 
-    damona env --create TEST
+    damona create TEST
 
 There, you have a *bin* directory where binaries are going to be installed.
 
 You can check that it has been created::
 
     damona env
 
@@ -313,15 +314,15 @@
 
 7. combine two different environments
 --------------------------------------
 
 In damona, you can have sereral environments in parallel and later activate the
 one you wish to use. Let us create a new one::
 
-    damone env --create test1
+    damone create test1
 
 and check that you now have one more environment::
 
     damona env
 
 We want to create an alias to the previously downloaded image of fastqc tool but
 in the *test1* environment. First we activate the newly create environment::
@@ -346,14 +347,24 @@
 
 Changelog
 =========
 
 ========= ========================================================================
 Version   Description
 ========= ========================================================================
+0.9.0     * refactorise the command 'env' by splitting into dedicated subcommands
+            create, delete, rename. add progress bar when downloading container
+          * NEW micromamba image to work as a localimage
+          * NEW sequana_minimal package to hold common tools (bwa, samtools,
+            kraken, etc)
+          * NEW ivarm pangolin, nextclade, subread, mafft packages
+          * UPDATE fastp to 0.23.3, gffread to 0.12.7 (3 times lighter).
+          * UPDATE sequana_tools to use micromamba (30% lighter)
+0.8.4     * fix damona stats command to return unique binaries
+          * more recipes and version (e.g. fastqc 0.12.1, graphviz update, etc)
 0.8.3     * create registry specifically for the sandbox (for testing)
           * add damona community in the uploads
           * add pbbam, bioconvert, busco, canu, ccs
           * add polypolish, samtools 1.16.1, sequana 0.14.6, flye 2.9, canu 2.1.1
             circlator 1.5.5, hifiasm
 0.8.2     * add idr, samtools, homer, bamtools, bedtools, sequana_denovo
           * add seqkit recipe and container
```

### Comparing `damona-0.8.3/damona/__init__.py` & `damona-0.9.0/damona/__init__.py`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/admin.py` & `damona-0.9.0/damona/admin.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 #
 ##############################################################################
 """Provide some stats for admin"""
 import os
 import sys
 
 from damona import Registry
-from damona.registry import Software
-from damona.registry import ImageName
 from damona import version
 
 import colorlog
 
 logger = colorlog.getLogger(__name__)
 
 
@@ -44,53 +42,62 @@
     """
 
     data = {}
     print(f"Damona version : {version}")
     r = Registry(biocontainers=biocontainers)
 
     Nv = len(r.get_list())
-    Nb = sum([len(x) for x in r.get_binaries().values()])
+    Nb = len(set([y for x in r.get_binaries().values() for y in x]))
     Ns = len(set([x.split(":")[0] for x in r.get_list()]))
     if biocontainers:
         print("From biocontainers, in theory*, we also have:")
     print(f"- number of software:  {Ns}")
     print(f"- version: {Nv}")
     print(f"- unique binaries: {Nb}")
     data["version"] = Nv
     data["software"] = Ns
     data["unique_binaries"] = Nb
     if biocontainers:
-        print("""*: not all software provided in the biocontainers registry are actually on Docker.
-There is nothing we can do about that in Damona. Actual number is more around 1000 public software""")
+        print(
+            """*: not all software provided in the biocontainers registry are actually on Docker.
+There is nothing we can do about that in Damona. Actual number is more around 1000 public software"""
+        )
 
     return data
 
 
-def build_biocontainers_registry(output="biocontainers.yml", force=False, limit=20000): #pragma: no cover
+def get_software_names():
+
+    r = Registry(biocontainers=False)
+    return set([x.split(":")[0] for x in r.get_list()])
+
+
+def build_biocontainers_registry(output="biocontainers.yml", force=False, limit=20000):  # pragma: no cover
     """Create the list of software and their versions available in Biocontainer"""
     logger.info("Retrieve all information from Biocontainers")
     try:
         from bioservices import Biocontainers
     except (ModuleNotFoundError, ImportError) as err:
-        logger.error("This function is for admin only. You may use but you mut install bioservices first (pip install bioservices). ")
-        return 
+        logger.error(
+            "This function is for admin only. You may use but you mut install bioservices first (pip install bioservices). "
+        )
+        return
 
     b = Biocontainers()
     info = b.get_tools(limit=limit)
     if len(info) > limit:
         logger.warning(f"Looks like you reached the limit of {limit} tool. Use limit argument to get more")
     tools = {}
-    for name, versions in zip(info['name'], info['versions']):
-        tools[name] = [x['meta_version'] for x in versions]
+    for name, versions in zip(info["name"], info["versions"]):
+        tools[name] = [x["meta_version"] for x in versions]
 
     # Create the registry
     if os.path.exists(output) and not force:
         logger.error(f"Output file {output} exists already. Please rename or remove the target file")
         sys.exit(1)
 
     with open(output, "w") as fout:
         for name, versions in tools.items():
             fout.write(f"{name}:\n  releases:\n")
             for version in versions:
                 fout.write(f"    {version}:\n")
                 fout.write(f"      download: docker://biocontainers/{name}:{version}\n")
-
```

### Comparing `damona-0.8.3/damona/biocontainers/registry.yaml` & `damona-0.9.0/damona/biocontainers/registry.yaml`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/builders.py` & `damona-0.9.0/damona/builders.py`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/common.py` & `damona-0.9.0/damona/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,18 +50,14 @@
     This class simply create the *~/.config/damona/envs* and images directories.
     It also checks whether **DAMONA_PATH** and **DAMONA_SINGULARITY_OPTIONS** variables
     are defined in the environment.
     """
 
     def __init__(self):
         if "DAMONA_PATH" not in os.environ:
-            try:
-                HOME = os.path.expanduser("~")
-            except Exception:  # pragma: no cover
-                HOME = "/home/user/"
             logger.critical(
                 """DAMONA_PATH was not found in your environment.
 
 Before using Damona, you have to copy/paste the following code in
 your ~/.bashrc file once for all (start a new shell afterwards):
 
     if [ ! -f  "~/.config/damona/damona.sh" ] ; then
@@ -153,15 +149,15 @@
         used_images = []
         for binary in binaries:
             br = BinaryReader(binary)
             used_images.append(pathlib.Path(br.image))
 
         used_images = set(used_images)
         Nu = len(used_images)
-        No = Ni - Nu
+        #No = Ni - Nu
         # keep print to make sure it is seen
         print(f"{Nu} images is/are used. ")
         orphans = []
 
         for image in sorted(images):
             if image not in used_images:  # pragma: no cover
                 logger.info(f"{image} image not used.")
@@ -214,15 +210,15 @@
             >>> print(ir.version)
             '0.11.9'
 
         """
         self.filename = pathlib.Path(name)
 
         if self.is_valid_name() is False:
-            logger.error("Invalid image name. Your input image must end in .img or .sif")
+            logger.error("Invalid image name. Your input image must end in .img or .sif ; version must be X.Y.Z")
             sys.exit(1)
 
     def delete(self):
         if self.is_orphan():
             logger.warning(f"deleting {self.filename} since it is not used anymore by any environments")
             self.filename.unlink()
         else:
@@ -307,15 +303,15 @@
 
 class BinaryReader:
     """Manage a single binary
 
     ::
 
         >>> from damona.common import BinaryReader
-        >>> br = BinaryReader("~/.config/damona/envs/base/fastqc")
+        >>> br = BinaryReader("~/.config/damona/envs/base/bin/fastqc")
         >>> br.get_image()
         'fastqc:0.11.9'
         >>> br.is_image_available()
         True
     """
 
     def __init__(self, filename):
@@ -372,15 +368,18 @@
         image = [x for x in command[0].split() if "/images/" in x]
         image = image[0].split()
         container = image[0].split("/")[-1]
         container = container.replace(".img", "")
         container = ":".join(container.rsplit("_", 1))
         return container
 
+
 import functools
+
+
 def requires_singularity(func):
     """A decorator to check presence of singularity"""
 
     @functools.wraps(func)
     def wrapper(ref, *args, **kwargs):
         if cmd_exists("singularity"):
             return func(ref, *args, **kwargs)
```

### Comparing `damona-0.8.3/damona/config.py` & `damona-0.9.0/damona/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 
 class Config:
     """A place holder to store our configuration file and shell scripts
 
 
     This class is called each time damona is started. The config file, if not present
-    is created, otherwise nothing happens. Same for the bash and fish shell configuration 
+    is created, otherwise nothing happens. Same for the bash and fish shell configuration
     files
 
     The damona configuration file looks like::
 
         [general]
         quiet=False
 
@@ -58,15 +58,15 @@
 
         [sandbox.zenodo]
         token=FFmbAEhQbb...
         orcid=0000-0001
         name='Cokelaer, Thomas'
         affiliation='Institut Pasteur'
 
-    Where the urls section can be used to store aliases to external registry. When 
+    Where the urls section can be used to store aliases to external registry. When
     installing software using::
 
         damona install example --from url damona
 
     if the alias damona is in the [urls] section, it is replaced by its real value (https://...)
     the URL must end with the expected registry name **registry.txt**
 
@@ -141,15 +141,15 @@
                     fout.write(fin.read())
             return True
         else:
             return False
 
 
 def get_damona_commands():
-    """Print commands available in Damona if not hidden. 
+    """Print commands available in Damona if not hidden.
 
     This function is used for the fish completion"""
     from damona import script
 
     commands = [x for x in dir(script) if "allow_interspersed_args" in dir(getattr(script, x))]
     commands = [x for x in commands if not getattr(script, x).hidden]
     commands = [x for x in commands if x != "main"]
```

### Comparing `damona-0.8.3/damona/environ.py` & `damona-0.9.0/damona/environ.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 """Environments manager"""
 import os
 import shutil
 import sys
 import pathlib
 import math
 import tarfile
+from tqdm import tqdm
 
 from damona.common import Damona
 from damona.common import BinaryReader
 
 
 manager = Damona()
 
@@ -40,14 +41,15 @@
     """Class to handle a specific environment given its name
 
     ::
 
         from damona import Environment
         ee = Environment("test1")
         ee.create_bundle("test.tar")
+        ee.create_yaml("test.yaml")
 
     """
 
     def __init__(self, name):
         """.. rubric:: **Constructor**
 
         :param str name: the name of the environment
@@ -73,15 +75,14 @@
     def __contains__(self, name):
         binaries = [x.name for x in self.get_installed_binaries()]
         return name in binaries
 
     def get_disk_usage(self):
         """Return virtual size of the environment if we were to
         copy/export all images"""
-        binaries = self.get_installed_binaries()
         S = 0
         images = self.get_images()
         for image in images:
             try:
                 if "DAMONA_PATH" not in os.environ:  # pragma: no cover
                     logger.error("You must define a DAMONA_PATH")
                     sys.exit(1)
@@ -113,15 +114,15 @@
 
         env_size = math.ceil(disk / 1e6)
 
         txt += f" Disk usage is {env_size}Mb"
         return txt
 
     def rename(self, newname, force=False):
-        """Rename an environment. 
+        """Rename an environment.
 
         Note that the *base* environment cannot be renamed
         """
         if self.name == "base":
             logger.error("You cannot rename the 'base' environment")
             sys.exit(1)
 
@@ -137,16 +138,16 @@
         ff.rename(self.path.parent / newname)
         # reset the path
         self._init(newname)
         logger.warning("Please restart a new shell if this is an active environment.")
 
     def get_current_state(self):
         """Return dictionary with statistics about the environment
-        
-        It includes the number of binariesm images and name of the 
+
+        It includes the number of binariesm images and name of the
         environment for now.
         """
         images = set()
         binaries = {}
         for filename in self.get_installed_binaries():
             br = BinaryReader(filename)
             image = br.get_image()
@@ -182,14 +183,58 @@
             logger.info(f"Adding {filename}")
             archive.add(filename, arcname=f"images/{filename.name}")
         archive.close()
 
         logger.info(f"Saved environment {self.name} into {output_name}")
         return output_name
 
+    def create_yaml(self, output_name=None):
+        if output_name is None:
+            output_name = f"damona_{self.name}.yaml"
+
+        images = [pathlib.Path(x) for x in self.get_images()]
+
+        with open(output_name, "w") as fout:
+
+            fout.write(f"name: {self.name}\n")
+            fout.write(f"\nimages:\n")
+
+            for image in images:
+                fout.write(f"- {image.name}\n")
+
+            fout.write(f"\nbinaries:\n")
+
+            binaries = self.get_installed_binaries()
+            binaries = [x.absolute() for x in binaries]
+            binaries = sorted(binaries)
+
+            for binary in binaries:
+                bininst = BinaryReader(binary)
+                fout.write(f"- {binary.name} from {bininst.get_image()}\n")
+
+
+class YamlEnv:
+    def __init__(self, filename):
+
+        self.name = None
+        self.binaries = []
+        self.images = []
+
+        with open(filename, "r") as fin:
+            for line in fin.readlines():
+                if line.startswith("name:"):
+                    self.name = line.split(":")[1].strip()
+
+                elif line.startswith("-") and " from " in line:
+                    line = line.replace("- ", "").strip()
+                    self.binaries.append(line)
+                elif line.startswith("-") and "from" not in line:
+                    line = line.replace("- ", "").strip()
+                    self.images.append(line)
+
 
 class Images:
     def __init__(self):
         self.images_dir = manager.images_directory
 
     def __len__(self):
         return len(list(self.files))
@@ -252,35 +297,40 @@
     def _get_env_names(self):
         envs = os.listdir(manager.environments_path)
         envs = sorted([Environment(x).name for x in envs])
         return envs
 
     environment_names = property(_get_env_names)
 
-    def delete(self, env_name):
+    def delete(self, env_name, force=False):
 
         if env_name == "base":
             logger.error("Environment 'base' is reserved and cannot not be created or deleted")
             sys.exit(1)
 
         env_path = manager.environments_path / env_name
         if os.path.exists(env_path) is False:
             logger.error("{} does not exists".format(env_path))
         else:
             try:
                 os.rmdir(env_path)
             except OSError:
-                logger.warning(
-                    "Will delete all contents of {}. Although this concerns only aliases you will lose your environement".format(
-                        env_path
+                if not force:
+                    logger.warning(
+                        f"Will delete all contents of {env_path}. Although this concerns only aliases you will lose your environement"
                     )
-                )
-                ret = input("Are you sure you want to proceed ? (N/y)")
-                if ret == "y":
+                else:
+                    logger.warning(f"Deleting environment {env_path} since you used --force")
+
+                if force:
                     shutil.rmtree(env_path)
+                else:
+                    ret = input("Are you sure you want to proceed ? (N/y)")
+                    if ret == "y":
+                        shutil.rmtree(env_path)
 
     def _env_in_path(self, env_name):
         PATH = os.environ["PATH"]
         paths = PATH.split(":")
         for x in paths:
             if str(manager.damona_path / "envs" / env_name / "bin") == x:
                 return True
@@ -327,15 +377,15 @@
         found = False  # this one is the one to deactivate (to ignore)
         newPATH = []
         for path in paths:
             # if deactivate without name, we remove the last one only
             if env_name and str(manager.damona_path / "envs" / env_name / "bin") == path:
                 logger.info(f"# Found damona path ({path}), to be removed from your PATH")
                 found = True
-            elif not env_name and f"/damona/envs/" in str(path) and not found:
+            elif not env_name and "/damona/envs/" in str(path) and not found:
                 logger.info(f"# Found a damona path ({path}), to be removed from your PATH")
                 found = True
             else:  # keep track of other paths.
                 newPATH.append(path)
 
         if found is False:
             logger.info("# no more active damona environment in your path. Use 'damona activate ENVNAME'")
@@ -381,22 +431,64 @@
                 os.mkdir(env_path)
                 os.mkdir(env_path / "bin")
                 logger.info(f"Created {env_name} in {env_directory}")
                 logger.info(f"Type 'damona activate {env_name}' to activate it")
             except:  # pragma: no cover
                 pass  # if already created, error are caught here
 
+    def create_from_yaml(self, env_name, yaml, force=False):
+        if env_name in self.environment_names:
+            logger.warning(f"{env_name} exists already.")
+            if force is False:
+                logger.critical(f"To recreate, you must delete it using 'damona delete {env_name}'")
+                sys.exit(0)
+            else:
+                logger.warning("You used --force, so overwritting existing environment")
+
+        env_directory = pathlib.Path(manager.damona_path / "envs" / env_name)
+
+        from damona.environ import YamlEnv
+
+        ye = YamlEnv(yaml)
+        # ye.name is not used for now, supposibly, it already exists, so we require a user input
+
+        self.create(env_name, force=force)
+
+        for image in tqdm(ye.images):
+            # local import to avoid circular import
+            from damona.install import RemoteImageInstaller
+
+            # replace all _ with :
+            image = image.rsplit(".", 1)[0].replace("_", ":")
+
+            # and replace : with _ except last one
+            image = image.replace(":", "_", image.count(":") - 1)
+
+            rii = RemoteImageInstaller(image)
+            rii.pull_image(force=True)
+
+        for binary in tqdm(ye.binaries):
+            # local import to avoid circular import
+            from damona.install import BinaryInstaller
+
+            binary, image = binary.split(" from ")
+            binary = binary.strip()
+            image = image.strip()
+            image += ".img"
+            bi = BinaryInstaller([binary], image, env_name)
+            bi.install_binaries()
+
     def create_from_bundle(self, env_name, bundle, force=False):
         if env_name in self.environment_names:
             logger.warning(f"{env_name} exists already.")
             if force is False:
-                logger.critical(f"To recreate, you must delete it using 'damona env --delete {env_name}'")
+                logger.critical(f"To recreate, you must delete it using 'damona delete {env_name}'")
                 sys.exit(0)
             else:
-                logger.warning(f"You used --force, so overwritting existing environment")
+                logger.warning("You used --force, so overwritting existing environment")
 
         # if it does not exsits or force is True
         self.create(env_name, force=force)
 
         env_directory = pathlib.Path(manager.damona_path / "envs" / env_name)
 
         archive = tarfile.open(bundle)
```

### Comparing `damona-0.8.3/damona/install.py` & `damona-0.9.0/damona/install.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,30 +13,29 @@
 #  documentation: http://damona.readthedocs.io
 #
 ##############################################################################
 """Tools to install images/binaries"""
 import os
 import sys
 import pathlib
-
 import shutil
 import time
 import subprocess
 
-from urllib.request import urlretrieve
 
 from easydev import md5
 
 
 from spython.main import Client
 from damona import Registry
 from damona import Environ
 from damona.common import ImageReader, requires_singularity
 from damona.registry import Software
 from damona import version as damona_version
+from damona.utils import download_with_progress
 
 
 DAMONA_PATH = os.environ["DAMONA_PATH"]
 
 
 import colorlog
 
@@ -129,14 +128,15 @@
     This is not recommended but very useful for developers::
 
         damona install fastqc_0.11.9.img --binaries fastqc
 
     Since there is no registry, you can set the list of binaries.
 
     """
+
     def __init__(self, image_name, cmd=None, binaries=None):
         """.. rubric:: **Constructor**
 
         :param str image_name: The location of the singularity image to be installed.
         :param cmd: internal place holder to fill the history log with the calling command.
         :param list binaries: The list of binaries to be installed and expected to be
             found in the :attr:`image_name`
@@ -261,17 +261,15 @@
 
     def is_valid(self):
 
         return True
 
     @requires_singularity
     def pull_image(self, output_name=None, force=False):
-        """Pull and Install a singularity image from the web.
-
-        """
+        """Pull and Install a singularity image from the web."""
 
         self.image_installed = False
 
         # the name must be valid. we use _ to separate name and version for the
         # singularity filemane but the image have a tag (version) and name
         # separated by a :
 
@@ -369,18 +367,17 @@
                 cmd += " --force "
             cmd += f"{self.from_url}/{download_name}"
             print(cmd)
             subprocess.call(cmd.split())
         else:
 
             if download_name.startswith("https://"):
-                print(f"downloading into {pull_folder} {output_name}")
+                logger.info(f"downloading into {pull_folder} {output_name}")
 
-                urlretrieve(download_name, filename=str(pull_folder / output_name))
-                # wget.download(download_name, str(pull_folder / output_name))
+                download_with_progress(download_name, filename=str(pull_folder / output_name))
 
             else:  # use singularity
                 Client.pull(str(download_name), name=output_name, pull_folder=pull_folder, force=force)
         logger.info(f"File {self.image_name} uploaded to {pull_folder}")
 
         # Read the image, checking everything is correct
 
@@ -421,15 +418,14 @@
             tools[name] = [x['meta_version'] for x in versions]
 
     """
 
     def __init__(self, image_name, binaries=None, cmd=None):
         super(BiocontainersInstaller, self).__init__()
 
-
         # get the biocontainers prefix and the name:version suffix
         prefix, suffix = image_name.split("/")
 
         if prefix != "biocontainers":
             logger.error(f"Biocontainers name must start with 'biocontainers/' ({prefix} provided")
             sys.exit(1)
 
@@ -440,32 +436,32 @@
         except ValueError as err:
             logger.error(f"Biocontainers name must be formatted as NAME:VERSION ({suffix} provided)")
             sys.exit(1)
 
         self.registry = Registry(biocontainers=True)
 
         if suffix not in self.registry.registry:
-            logger.error(f"{name} not found in the biocontainers registry. Use damona search PATTERN --include-biocontainers")
+            logger.error(
+                f"{name} not found in the biocontainers registry. Use damona search PATTERN --include-biocontainers"
+            )
             sys.exit(1)
 
         self.image_name = image_name
         self.images_directory = pathlib.Path(DAMONA_PATH) / "images"
 
         self.cmd = cmd
         self.binaries = binaries
         self.image_installed = False
 
     def is_valid(self):
         return True
 
     @requires_singularity
     def pull_image(self, output_name=None, force=False):
-        """Pull and Install a biocontainer image.
-
-        """
+        """Pull and Install a biocontainer image."""
         self.image_installed = False
 
         download_name = self.image_name
 
         # now that we have the registry name, we can download the image
         logger.info("Downloading {}".format(self.image_name))
 
@@ -490,37 +486,39 @@
             logger.warning("File not installed properly. Stopping")
             self.image_installed = False
 
         # for the install_binaries to work, we need to set the binaries
         prefix, suffix = self.image_name.split("/")
         self.binaries = self.registry.registry[suffix].binaries
 
-
-
         self.image_installed = True
 
 
-
-
 class BinaryInstaller:
-    """Install a binary in the bin/ directory of the current environment given its image
-
+    """Install a binary in the bin/ directory of the current environment given its image"""
 
-    """
-    def __init__(self, binaries, parent_image_path):
+    def __init__(self, binaries, parent_image_path, env_name=None):
         """.. rubric:: **Constructor**
 
         :param list binaries: list of binaries to install
         :param str parent_image_path: the location of the images where binaries are to be found
 
         """
         #: instance of :class:`damona.common.ImageReader`
         self.image = ImageReader(parent_image_path)
         self.binaries = binaries
 
+        if env_name:
+            from damona.common import get_damona_path
+
+            self.env_name = get_damona_path() / "envs" / env_name
+        else:
+            env = Environ()
+            self.env_name = env.get_current_env()
+
     @requires_singularity
     def install_binaries(self, force=False):
         """Install an image and its binaries
 
         Given the :attr:`~damona.install.BinaryInstaller.image`, we install a set of :attr:`~damona.install.BinaryInstaller.binaries` to be found in the
         image registry. If we install a binary again, no need to rewrite the command. For example,
         imagine that you installed fastqc.0.11.9 for the first time, then in the commands
@@ -530,20 +528,19 @@
             damona install fastqc:0.11.9 --force
 
         the second command has no effect. If we now install a new version::
 
             damona install fastqc:0.11.8
 
         The previous binary (v0.11.9) will be replaced by the new one (v0.11.8).
-        The old image is kept in the images directory (it may be used in another 
+        The old image is kept in the images directory (it may be used in another
         environment indeed).
         """
 
-        env = Environ()
-        bin_directory = env.get_current_env() / "bin"
+        bin_directory = self.env_name / "bin"
         logger.info(bin_directory)
 
         for binary in sorted(self.binaries):
             bin_path = pathlib.Path(bin_directory) / binary
 
             CMD = """singularity -s exec ${{DAMONA_SINGULARITY_OPTIONS}} {} {} ${{1+"$@"}}"""
             CMD = CMD.format(f"${{DAMONA_PATH}}/images/{self.image.shortname}", binary)
```

### Comparing `damona-0.8.3/damona/library/R/Singularity.R_3.6.3` & `damona-0.9.0/damona/library/R/Singularity.R_3.6.3`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/library/R/Singularity.R_4.0.2` & `damona-0.9.0/damona/library/R/Singularity.R_4.0.2`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/library/conda/README.rst` & `damona-0.9.0/damona/library/conda/README.rst`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/library/conda/Singularity.conda_4.7.12` & `damona-0.9.0/damona/library/conda/Singularity.conda_4.7.12`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/library/conda/Singularity.conda_4.9.2` & `damona-0.9.0/damona/library/conda/Singularity.conda_4.9.2`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/library/ubuntu/Singularity.ubuntu_16.04` & `damona-0.9.0/damona/library/ubuntu/Singularity.ubuntu_16.04`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/library/ubuntu/Singularity.ubuntu_18.04` & `damona-0.9.0/damona/library/ubuntu/Singularity.ubuntu_18.04`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/registry.py` & `damona-0.9.0/damona/registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from damona.config import Config
 
 import colorlog
 
 logger = colorlog.getLogger(__name__)
 
 
-__all__ = ["Releases", "Software", "Registry", "Release", "ImageName", "RemoteRegistry" ]
+__all__ = ["Releases", "Software", "Registry", "Release", "ImageName", "RemoteRegistry"]
 
 
 class ImageName:
     """Check image name
 
     An image name must have the following convention::
 
@@ -97,20 +97,19 @@
                 # strings for e.g x.y.z
                 self[str(version)] = Release(version, data)
 
     def _get_last_release(self):
         from packaging import version
 
         # split on - for the special cases 0.11.9-py3
-        return max(list(self.keys()), key=lambda x: version.parse(x.split('-')[0]))
+        return max(list(self.keys()), key=lambda x: version.parse(x.split("-")[0]))
 
     last_release = property(_get_last_release, doc="return the last version")
 
 
-
 class Release:
     """A Release class
 
     This class populates information found in the release section of a
     registry.
 
     A regitry looks like::
@@ -219,21 +218,19 @@
         html = response.read()
         self.rawdata = html.decode("utf-8")
         remote_registry = yaml.load(self.rawdata, Loader=Loader)
         self.data = remote_registry
 
 
 class BiocontainersRegistry:
-
     def __init__(self, filename=None):
         from damona import __path__
 
-
         if filename in [True, None]:
-            self.filename = pathlib.Path(__path__[0]) / "biocontainers" /  "registry.yaml"
+            self.filename = pathlib.Path(__path__[0]) / "biocontainers" / "registry.yaml"
         elif os.path.exists(filename):
             self.filename = filename
         else:
             raise ValueError(f"Expected a valid input filename. you provided {filename}")
         self._read_registry()
 
     def _read_registry(self):
@@ -387,15 +384,15 @@
         self.from_biocontainers = biocontainers
         self.from_url = from_url
         self.registry = {}
         self.discovery()
 
     def find_candidate(self, pattern):
         """Find a unique recipe within the registry."""
-        candidates = [x for x in self.registry.keys() if pattern==x or pattern in x.split(":")]
+        candidates = [x for x in self.registry.keys() if pattern == x or pattern in x.split(":")]
 
         if len(candidates) == 0:  # pragma: no cover
             logger.critical(
                 f"No image found for {pattern}. Make sure it is correct. You can use 'damona search' command"
             )
             return None
 
@@ -421,15 +418,15 @@
             self._url_discovery()
         elif self.from_biocontainers:
             self._biocontainers_discovery()
         else:
             self._damona_discovery()
 
     def _populate(self, data):
-        #Used by _url_discovery, _biocontainers_discovery, _damona_discovery 
+        # Used by _url_discovery, _biocontainers_discovery, _damona_discovery
 
         self.registry = {}
 
         for name, content in data.items():
             software = Software({name: content})
             software.check()
             # we may have several releases
@@ -460,23 +457,23 @@
         ext_reg = BiocontainersRegistry(self.from_biocontainers)
         self._populate(ext_reg.data)
 
     def _damona_discovery(self):
 
         # read all damona registry and store in expected dictionary structure
         from damona.software import __path__
+
         _registry_files = glob.glob(__path__[0] + "/*/registry.yaml")
         data = {}
         for registry in _registry_files:
             software = Software(registry)
             data[software.name] = software._yaml[software.name]
 
         self._populate(data)
 
-
     def get_list(self, pattern=None):
         """Return list of :class:`Software` found in the registry"""
         software = {}
         for name, info in self.registry.items():
             if pattern:
                 if pattern.lower() in name.lower():
                     software[name] = info.download
```

### Comparing `damona-0.8.3/damona/script.py` & `damona-0.9.0/damona/script.py`

 * *Files 14% similar despite different names*

```diff
@@ -58,16 +58,16 @@
     """Damona is an environment manager for singularity containers.
 
     It is to singularity container what conda is to packaging.
 
     The default environment is called 'base'. You can create and activate
     a new environment as follows:
 
-    \b 
-        damona env --create TEST
+    \b
+        damona create --name TEST
         damona activate TEST
 
     Once an environment is activated, you can install a Damona-registered image
     (and its registered binaries):
 
         damona install fastqc:0.11.9
 
@@ -81,84 +81,108 @@
     ######################## !!!!!!!!!!!! ####################
     # this function cannot print anything because the damona
     # activate command prints bash commands read by damona.sh
     ######################## !!!!!!!!!!!! ####################
     logger.setLevel(level)
 
 
-# =================================================================== env
 @main.command()
-@click.option("--create", type=click.STRING, help="""create a new environment""")
-@click.option("--delete", type=click.STRING, help="""Delete an existing environment""")
-@click.option("--rename", type=click.STRING, help="""Rename an existing environment""")
-@click.option("--new-name", type=click.STRING, default="", help="""The new environment name (use with --rename) only""")
-@click.option("--disk-usage", is_flag=True, help="Prints disk usage of each Damona environments")
-@click.option("--from-bundle", type=click.STRING, help="a bundle file create with 'damona export' command")
+@click.argument("environment", required=True, type=click.STRING)
+@click.option("--from-bundle", type=click.STRING, help="a bundle file create with 'damona export --bundle' command")
+@click.option("--from-yaml", type=click.STRING, help="a yaml file create with 'damona export --yaml' command")
 @click.option(
     "--force",
     is_flag=True,
     help="""When creating an environment with --from-bundle, rewrite binaries and
 images even though the environment exists.""",
 )
+def create(**kwargs):
+    """Create a new environment
+
+    Here we create an environment called TEST:
+
+    \b
+        damona create TEST
+
+    You can then activate it:
+
+    \b
+        damona activate TEST
+
+    You can create an environment from a environment.yaml file that was created with the 'export --yaml' command
+    or manually built using the following syntax:
+
+    \b
+        name: sequana_rnaseq
+    \b
+        images:
+            - sequana_tools_0.14.5.img
+    \b
+        binaries:
+            - bwa
+            - samtools
+            - bamtools
+
+    """
+    envs = Environ()
+    if kwargs["from_bundle"]:
+        envs.create_from_bundle(kwargs["environment"], bundle=kwargs["from_bundle"], force=kwargs["force"])
+    elif kwargs["from_yaml"]:
+        envs.create_from_yaml(kwargs["environment"], yaml=kwargs["from_yaml"], force=kwargs["force"])
+    else:
+        envs.create(kwargs["environment"])
+
+
+@main.command()
+@click.argument("environment", required=True, type=click.STRING)
+@click.option("--force", is_flag=True, help="""When creating an environment with --from-bundle, rewrite binaries and""")
+def delete(**kwargs):
+    """Remove an environment"""
+    env = Environ()
+    env.delete(kwargs["environment"], force=kwargs['force'])
+
+
+@main.command()
+@click.argument("environment", required=True, type=click.STRING)
+@click.option("--new-name", required=True, type=click.STRING, help="""new name of the environments""")
+def rename(**kwargs):
+    """Rename an existing environment"""
+    env = Environment(kwargs["environment"])
+    env.rename(kwargs["new_name"])
+
+
+# =================================================================== env
+@main.command()
 def env(**kwargs):
-    """Create/Delete/Rename environments here.
+    """Delete/Rename environments here.
 
-    Print information about current environments::
+    To create an environment, use ::
 
-        damona env
+        damona create --name TEST
 
-    Check the disk usage of each environments::
+    Print information about current environments::
 
-        damona env --disk-usage
+        damona env
 
     You can also create an environment and install a saved on in it::
 
     \b
         damona export test1
         damona env --create copy_test1 --from-bundle damona_test1.tar
 
     """
     envs = Environ()
 
-    if kwargs["disk_usage"]:
-        envs = Environ()
-        N = len(envs.images)
-        usage = envs.images.get_disk_usage()
-        click.echo(f"Found {N} images: Images usage: {usage}.Mb")
-    elif kwargs["create"] is None and kwargs["delete"] is None and kwargs["rename"] is None:
-        click.secho(f"There are currently {envs.N} Damona environments:\n", bold=True)
-        if envs.N != 0:
-            for this in envs.environments:
-                name = this.name
-                click.echo(click.style(f"{name}", bold=True) + click.style(f" -  {this}"))
-        current_env = envs.get_current_env_name()
-        click.secho(f"\nYour current env is '{current_env}'.", bold=True)
-    elif kwargs["create"] and kwargs["delete"]:  # mutually exclusive
-        logger.error("you cannot use --delete and --create together")
-        sys.exit(1)
-    elif kwargs["create"] and kwargs["rename"]:  # mutually exclusive
-        logger.error("you cannot use --delete and --rename together")
-        sys.exit(1)
-    elif kwargs["rename"] and kwargs["delete"]:  # mutually exclusive
-        logger.error("you cannot use --delete and --rename together")
-        sys.exyyit(1)
-
-    elif kwargs["delete"]:
-        envs.delete(kwargs["delete"])
-    elif kwargs["create"]:
-        if kwargs["from_bundle"]:
-            envs.create_from_bundle(kwargs["create"], bundle=kwargs["from_bundle"], force=kwargs["force"])
-        else:
-            envs.create(kwargs["create"])
-    elif kwargs["rename"]:
-        if kwargs["new_name"] == "":
-            logger.error("If you use --rename, you must provide a new name with --new-name")
-            sys.exit(1)
-        env = Environment(kwargs["rename"])
-        env.rename(kwargs["new_name"], force=kwargs["force"])
+    click.secho(f"There are currently {envs.N} Damona environments:\n", bold=True)
+    if envs.N != 0:
+        for this in envs.environments:
+            name = this.name
+            click.echo(click.style(f"{name}", bold=True) + click.style(f" -  {this}"))
+    current_env = envs.get_current_env_name()
+    click.secho(f"\nYour current env is '{current_env}'.", bold=True)
 
 
 # =================================================================== activate
 @main.command()
 @click.argument("name", required=True, type=click.STRING)
 def activate(**kwargs):
     """Activate a damona environment.
@@ -241,18 +265,20 @@
     Images are installed in the ~/.config/damona/images directory. It is the
     DAMONA_PATH environment variable. Therefore, you can redefine this variable
     to install images elsewhere.
 
     You may have images online on a website. To install such images, use
     the --url (see developer guide for details).
 
-    Or wish to use a biocontainers docker file::
+    Or wish to use an existing docker file::
 
         damona install biocontainers/hisat2:v2.0.5-1-deb
 
+    Note (June 2023) biocontainers do not work anymore...
+
     """
     logger.debug(kwargs)
 
     env = Environ()
     cenv = env.get_current_env()
 
     # url
@@ -270,19 +296,17 @@
         if "," in kwargs["binaries"]:
             binaries = kwargs["binaries"].split(",")
         else:
             binaries = [kwargs["binaries"]]
     else:
         binaries = None
 
-
-    if kwargs['image'].startswith("biocontainers/"):
-        p = BiocontainersInstaller(kwargs['image'], binaries=binaries)
+    if kwargs["image"].startswith("biocontainers/"):
+        p = BiocontainersInstaller(kwargs["image"], binaries=binaries)
         p.pull_image(force=force_image)
-
         p.install_binaries(force=force_binaries)
 
     elif os.path.exists(image_path) is False:
         if kwargs["url"]:
             url = kwargs["url"]
             logger.info(f"Installing from online registry  (url: {url})")
         else:
@@ -320,35 +344,35 @@
 @click.argument("name", required=True, type=click.STRING)
 @click.option("--environment", type=click.STRING, default=None)
 # @click.option("--force", is_flag=True, help="force the removal of binaries or images")
 def remove(**kwargs):
     """Remove binaries or image from an environment.
 
     You can remove a binary from an environment given its path. It will not be removed
-    if used by an executable if an environment.::
+    if used by an executable in an environment.::
 
         damona remove /home/cokelaer/.config/damona/images/fastqc_0.11.8.img
 
     if you have the name of the image, it works as well::
 
         damona remove fastqc_0.11.8.img
 
     You must give the .img extension in both cases otherwise it is considered
     to be a binary that you want to remove.
 
     If you suppress a binary like here::
 
         damona remove fastqc
 
-    it removes the binary from the activate environnt only. Then, it the image is now orpha,
-    it is also removed.
+    it removes the binary from the activate environment only. Then, if the image is now an
+    orphan, it is also removed.
 
 
     You can also remove an image (and its binaries) from an environment. Note, however,
-    that the image is not deleted if usde in other environments.
+    that the image is not deleted if used in other environments.
     """
     # First, let us figure out the current or user-defined environment
     envs = Environ()
     env_name = kwargs["environment"]
     if not env_name:
         env_name = envs.get_current_env_name(warning=False)
         if env_name is None:
@@ -435,29 +459,28 @@
         logger.info("No orphan images found")
     else:
         logger.info(f"Found {len(orphans)} orphans.")
 
     if kwargs["remove"]:  # pragma: no cover
         for x in orphans:
             answer = input(f"You are going to delete this image: {x}. Are you sure ? (yes/no)")
-            if answer in [ "yes", 'y']:
+            if answer in ["yes", "y"]:
                 os.remove(os.path.expanduser(x))
                 logger.info(f"Removed {x}")
             else:
                 logger.info(f"skipped deletion of {x}")
     else:
         logger.warning("Please use --remove to confirm that you want to remove the orphans")
 
 
 # =================================================================== search
 @main.command()
 @click.argument("pattern", required=True, type=click.STRING)
 @click.option("--images-only", is_flag=True, default=False, help="Show images only")
-@click.option("--include-biocontainers", is_flag=True, default=False, 
-    help="include also biocontainers hits")
+@click.option("--include-biocontainers", is_flag=True, default=False, help="include also biocontainers hits")
 @click.option("--binaries-only", is_flag=True, default=False, help="Show binaries only")
 @click.option(
     "--url",
     help="""Set the online registry file to search for a
 given container. See damona.readthedocs.io for in formation on how to write this
 file . Example is available on https://biomics.pasteur.fr/salsa/damona/registry.txt""",
 )
@@ -481,16 +504,16 @@
         damona search fastqc --url https://biomics.pasteur.fr/salsa/damona/registry.txt
 
     You may define aliases to URLs in your ~/.config/damona/damona.cfg file to
     make it easier::
 
         damona search fastqc --url damona
 
-    Although not recommended (not curated by Damona), you can also 
-    install any container available on biocontainer. To do som you first 
+    Although not recommended (not curated by Damona), you can also
+    install any container available on biocontainer. To do som you first
     need to know the name and version:
 
         damona search fastqc --include-biocontainers
 
 
     """
 
@@ -513,18 +536,18 @@
         for k in sorted(modules.keys()):
             v = modules[k]
             click.echo(f" - {k}: {v} (damona install {k})")
 
     if kwargs["include_biocontainers"]:
         click.echo("Searching biocontainers:")
         br = BiocontainersRegistry()
-        for k,data in br.data.items():
+        for k, data in br.data.items():
             if pattern in k:
                 click.echo(f" - {k}: ")
-                for version, location in data['releases'].items():
+                for version, location in data["releases"].items():
                     install = f"(damona install biocontainers/{k}:{version})"
                     click.echo(f" -     {version}: {install} ")
             elif pattern == "*":
                 click.echo(f" - {k}: {v}")
 
 
 # ============================================================  export
@@ -548,76 +571,119 @@
 
     x = [ee for ee in manager.environments if ee.name == envname]
     if len(x) == 0:
         logger.error(f"Environment '{envname}' does not exist. Use 'damona env' to get the list")
         sys.exit(1)
     else:
         environ = x[0]
-        click.echo(environ)
-        click.echo("Images:")
+        click.echo(f"name: {envname}")
+        click.echo("\nimages:")
         for item in sorted(environ.get_images()):
             click.echo(" - " + pathlib.Path(item).name)
-        click.echo("Binaries:")
+        click.echo("\nbinaries:")
         for item in sorted(environ.get_installed_binaries()):
             click.echo(" - " + pathlib.Path(item).name)
 
 
 # ============================================================  export
 @main.command()
 @click.argument("environment", required=True, type=click.STRING)
-@click.option("--output", default=None, help="name of output file")
+@click.option("--yaml", help="name of output file")
+@click.option("--bundle", default=None, help="name of output file")
 def export(**kwargs):
     """Create a bundle of a given environment.
 
     the following command copies all binaries from an environment and their
     associated images into a tar ball file named after the
-    environment.::
+    environment.
 
-        damona export test1
+    \b
+        damona export TEST --yaml   test_env.yaml
+        damona export TEST --bundle test_bundle.tar
+
+    We do not compress the tar file. The images are already compressed.
 
     This create a bundle named damona_test1.tar. You can then create a new
-    environment starting from this bundle::
+    environment starting from this bundle:
+
+    \b
+        damona env --create TEST1 --from-bundle test_bundle.tar
+        damona env --create TEST1 --from-yaml   test_env.yaml
 
-        damona env --create TEST1 --from-bundle damona_test1.tar
 
     """
     from damona import Environment
 
     logger.debug(kwargs)
 
     environment = kwargs["environment"]
     envname = kwargs["environment"]
 
     # TODO This should be based on the binaries of the environment, not the images
     # to do so, we'll need an installed.txt file
 
     env = Environment(envname)
-    output = env.create_bundle(output_name=kwargs["output"])
-    logger.info(f"Use this command to create a new environment: \n\n\tdamona env --create test --from-bundle {output}")
+    if kwargs["bundle"]:
+        bundle_file = kwargs["bundle"]
+        output = env.create_bundle(output_name=kwargs["bundle"])
+        logger.info(
+            f"Use this command to create a new environment: \n\n\tdamona create test1 --from-bundle {bundle_file}"
+        )
+    elif kwargs["yaml"]:
+        yaml_file = kwargs["yaml"]
+        env.create_yaml(output_name=yaml_file)
+        logger.info(f"Use this command to create a new environment: \n\n\tdamona create test1 --from-yaml {yaml_file}")
 
 
 # ============================================================  stats
 
 
 @main.command()
 @click.option("--include-biocontainers", is_flag=True, help="include also biocontainers (experimental)")
+@click.option("--include-downloads", is_flag=True, help="include downloads")
 def stats(**kwargs):
     """Get information about Damona images and binaries
 
     Just type::
 
         damona stats
 
+    This will print the actual status of Damona with number of binaries/images.
+    This will also give local information
+
     """
     from damona import admin
 
     admin.stats()
-    if kwargs['include_biocontainers']:
+    if kwargs["include_biocontainers"]:
         admin.stats(True)
 
+    if kwargs["include_downloads"]:
+        click.echo("Detailled summary of downloads for each container:")
+        from damona import admin
+        from damona import zenodo
+
+        all_software = admin.get_software_names()
+        N = 0
+        for software in sorted(all_software):
+            downloads = zenodo.get_stats_software(software)
+            click.echo(f"{software}: {downloads}")
+            try:
+                N += downloads.replace(",", "")
+            except AttributeError:
+                N += downloads
+        click.echo(f"Total: {N}")
+
+    envs = Environ()
+    N = len(envs.images)
+    usage = envs.images.get_disk_usage()
+    click.echo(
+        f"\n--\nLocal installation. In your local environment, we found {N} images. This account for a total of: {usage}.Mb"
+    )
+
 
 # ===================================================================  list
 
 
 @main.command()
 def list(**kwargs):
     """List all packages that can be installed"""
```

### Comparing `damona-0.8.3/damona/shell/bash/damona.sh` & `damona-0.9.0/damona/shell/bash/damona.sh`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/shell/damona_comp.sh` & `damona-0.9.0/damona/shell/damona_comp.sh`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/shell/fish/damona.fish` & `damona-0.9.0/damona/shell/fish/damona.fish`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/RIPseeker/Singularity.RIPseeker_1.0.0` & `damona-0.9.0/damona/software/RIPseeker/Singularity.RIPseeker_1.0.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/RIPseeker/registry.yaml` & `damona-0.9.0/damona/software/RIPseeker/registry.yaml`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/art/registry.yaml` & `damona-0.9.0/damona/software/art/registry.yaml`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/bamtools/Singularity.bamtools_2.5.2` & `damona-0.9.0/damona/software/bamtools/Singularity.bamtools_2.5.2`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/bbtools/registry.yaml` & `damona-0.9.0/damona/software/bbtools/registry.yaml`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/bcl2fastq/README.rst` & `damona-0.9.0/damona/software/bcl2fastq/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 In order to build this recipes, you must have your own license of bcl2fastq by
 downloading and agreeing to the terms for your user license. We cannot provide
-the RPM or source even though they are available for free. 
+the RPM or source even though they are available for free.
 
 This can be done on Illumina website in the download section you should find the
 RPM link to download bcl2fastq2.20 RPM file.
 
 Once you have the RPM, copy it in this directory and call it *bcl2fastq.rpm*
 
 To build this singularity container yourself::
```

### Comparing `damona-0.8.3/damona/software/bedtools/Singularity.bedtools_2.30.0` & `damona-0.9.0/damona/software/bedtools/Singularity.bedtools_2.30.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/bioconvert/Singularity.bioconvert_0.6.1` & `damona-0.9.0/damona/software/bioconvert/Singularity.bioconvert_0.6.1`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/bioconvert/Singularity.bioconvert_0.6.2` & `damona-0.9.0/damona/software/bioconvert/Singularity.bioconvert_0.6.2`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/bioconvert/Singularity.bioconvert_0.6.3` & `damona-0.9.0/damona/software/bioconvert/Singularity.bioconvert_0.6.3`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/bioconvert/Singularity.bioconvert_1.0.0` & `damona-0.9.0/damona/software/bioconvert/Singularity.bioconvert_1.0.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/bioconvert/registry.yaml` & `damona-0.9.0/damona/software/bioconvert/registry.yaml`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/bowtie/Singularity.bowtie_1.3.1` & `damona-0.9.0/damona/software/bowtie/Singularity.bowtie_1.3.1`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/bowtie2/Singularity.bowtie2_2.3.4` & `damona-0.9.0/damona/software/bowtie2/Singularity.bowtie2_2.3.4`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/bowtie2/Singularity.bowtie2_2.4.2` & `damona-0.9.0/damona/software/bowtie2/Singularity.bowtie2_2.4.2`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/bowtie2/registry.yaml` & `damona-0.9.0/damona/software/bowtie2/registry.yaml`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/busco/Singularity.busco_5.4.6` & `damona-0.9.0/damona/software/busco/Singularity.busco_5.4.6`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/bwa/Singularity.bwa_0.7.17` & `damona-0.9.0/damona/software/bwa/Singularity.bwa_0.7.17`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 %labels
     Author thomas cokelaer
 
 %post
 
     apk update
-    apk add unzip
+    apk add unzip bash
 
     apk add ca-certificates
     update-ca-certificates
     apk add --update --no-cache ncurses --force-non-repository
 
     apk add --no-cache wget g++ make zlib-dev bzip2 bzip2-dev patch
```

### Comparing `damona-0.8.3/damona/software/canu/Singularity.canu_2.1.1` & `damona-0.9.0/damona/software/canu/Singularity.canu_2.1.1`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 %labels
     Author thomas cokelaer
 
 %post
     export CANU_VERSION=2.1.1
 
     apt update -y && apt upgrade -y && apt install -y git build-essential zlib1g-dev wget && \
-        apt install -y autoconf automake  pkg-config libtool-bin yaggo perl 
+        apt install -y autoconf automake  pkg-config libtool-bin yaggo perl default-jre 
 
     wget https://github.com/marbl/canu/releases/download/v${CANU_VERSION}/canu-${CANU_VERSION}.Linux-amd64.tar.xz && \
         tar -xvf canu-${CANU_VERSION}.Linux-amd64.tar.xz  &&
         rm canu-${CANU_VERSION}.Linux-amd64.tar.xz
 
     apt-get autoremove -y
     apt-get autoclean -y
```

### Comparing `damona-0.8.3/damona/software/canu/registry.yaml` & `damona-0.9.0/damona/software/canu/registry.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -10,11 +10,11 @@
       filesize: 848314368
     1.8.0:
       download: https://zenodo.org/record/5765679/files/canu_1.8.0.img
       md5sum: 7de1e567c6102f572f760e1f08855013
       doi: 10.5281/zenodo.5765679
       filesize: 798138368
     2.1.1:
-      download: https://zenodo.org/record/7808153/files/canu_2.1.1.img
-      md5sum: 483122e00fa0f3d7611fa2e170308296
-      doi: 10.5281/zenodo.7808153
-      filesize: 233267200
+      download: https://zenodo.org/record/7866415/files/canu_2.1.1.img
+      md5sum: 191b8eca9c40945fb975c6a6e69970f2
+      doi: 10.5281/zenodo.7866415
+      filesize: 363024384
```

### Comparing `damona-0.8.3/damona/software/circlator/Singularity.circlator_1.5.5` & `damona-0.9.0/damona/software/circlator/Singularity.circlator_1.5.5`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/falco/Singularity.falco_0.2.1` & `damona-0.9.0/damona/software/falco/Singularity.falco_0.2.1`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/falco/Singularity.falco_1.0.0` & `damona-0.9.0/damona/software/falco/Singularity.falco_1.0.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/fastqc/Singularity.fastqc_0.11.8` & `damona-0.9.0/damona/software/fastqc/Singularity.fastqc_0.11.8`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/fastqc/Singularity.fastqc_0.11.9_py3` & `damona-0.9.0/damona/software/fastqc/Singularity.fastqc_0.11.9_py3`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/fastqc/registry.yaml` & `damona-0.9.0/damona/software/fastqc/registry.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -13,7 +13,12 @@
       doi: 10.5281/zenodo.5708811
       filesize: 198116894
     0.11.9-py3:
       download: https://zenodo.org/record/7015004/files/fastqc_0.11.9-py3.img
       md5sum: 10d09a5d67f8a93bd1d1b7cba46db883
       doi: 10.5281/zenodo.7015004
       filesize: 138665984
+    0.12.1:
+      download: https://zenodo.org/record/7923780/files/fastqc_0.12.1.img
+      md5sum: 5a1b3f8c6a9fbe54cc600be44699d228
+      doi: 10.5281/zenodo.7923780
+      filesize: 138809344
```

### Comparing `damona-0.8.3/damona/software/gffread/Singularity.gffread_0.12.1` & `damona-0.9.0/damona/software/gffread/Singularity.gffread_0.12.1`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/hifiasm/Singularity.hifiasm_0.19.1` & `damona-0.9.0/damona/software/hifiasm/Singularity.hifiasm_0.19.1`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/idr/Singularity.idr_2.0.3` & `damona-0.9.0/damona/software/idr/Singularity.idr_2.0.3`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/igvtools/Singularity.igvtools_2.12.0` & `damona-0.9.0/damona/software/igvtools/Singularity.igvtools_2.12.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/kraken/Singularity.kraken_1.1.0` & `damona-0.9.0/damona/software/kraken/Singularity.kraken_1.1.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/kraken/Singularity.kraken_2.0.9` & `damona-0.9.0/damona/software/kraken/Singularity.kraken_2.0.9`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/kraken/registry.yaml` & `damona-0.9.0/damona/software/kraken/registry.yaml`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/minimap2/Singularity.minimap2_2.17.0` & `damona-0.9.0/damona/software/minimap2/Singularity.minimap2_2.17.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/minimap2/Singularity.minimap2_2.23.0` & `damona-0.9.0/damona/software/minimap2/Singularity.minimap2_2.23.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/minimap2/registry.yaml` & `damona-0.9.0/damona/software/minimap2/registry.yaml`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/pbbam/Singularity.pbbam_2.1.0` & `damona-0.9.0/damona/software/pbbam/Singularity.pbbam_2.1.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/pbbam/Singularity.pbbam_2.3.0` & `damona-0.9.0/damona/software/pbbam/Singularity.pbbam_2.3.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/phantompeakqualtools/Singularity.phantompeakqualtools_1.2.2` & `damona-0.9.0/damona/software/phantompeakqualtools/Singularity.phantompeakqualtools_1.2.2`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/phantompeakqualtools/registry.yaml` & `damona-0.9.0/damona/software/phantompeakqualtools/registry.yaml`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/picard/Singularity.picard_2.26` & `damona-0.9.0/damona/software/picard/Singularity.picard_2.26`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/polypolish/Singularity.polypolish_0.5.0` & `damona-0.9.0/damona/software/polypolish/Singularity.polypolish_0.5.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/prokka/Singularity.prokka_1.14.5` & `damona-0.9.0/damona/software/prokka/Singularity.prokka_1.14.5`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/quast/Singularity.quast_5.0.2` & `damona-0.9.0/damona/software/quast/Singularity.quast_5.0.2`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/rnadiff/Singularity.rnadiff_1.7.1` & `damona-0.9.0/damona/software/rnadiff/Singularity.rnadiff_1.7.1`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/rnaseqc/Singularity.rnaseqc_2.35.0` & `damona-0.9.0/damona/software/rnaseqc/Singularity.rnaseqc_2.35.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/rtools/Singularity.rtools_1.2.0` & `damona-0.9.0/damona/software/rtools/Singularity.rtools_1.2.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/rtools/registry.yaml` & `damona-0.9.0/damona/software/rtools/registry.yaml`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/salmon/Singularity.salmon_1.3.0` & `damona-0.9.0/damona/software/salmon/Singularity.salmon_1.3.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/samtools/Singularity.samtools_1.15.0` & `damona-0.9.0/damona/software/samtools/Singularity.samtools_1.15.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/samtools/Singularity.samtools_1.16.1` & `damona-0.9.0/damona/software/samtools/Singularity.samtools_1.16.1`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/samtools_minimap2/Singularity.samtools_1.17_minimap2_2.24.0` & `damona-0.9.0/damona/software/samtools_minimap2/Singularity.samtools_1.17_minimap2_2.24.0`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Bootstrap: docker
 From: alpine:3.17
 
+
 %labels
   Author Sequana Team
 
 %post
   SAMTOOLS_VERSION=1.17
   MINIMAP2_VERSION=2.24
 
-  apk update && apk upgrade && apk add bash libc6-compat curl
+  apk update && apk upgrade && apk add bash libc6-compat curl python3
   # samtools deps
   apk add autoconf automake make gcc musl-dev perl zlib-dev bzip2-dev xz-dev curl-dev ncurses-dev
 
   curl -L https://github.com/lh3/minimap2/releases/download/v${MINIMAP2_VERSION}/minimap2-${MINIMAP2_VERSION}_x64-linux.tar.bz2 | tar -jxf - minimap2-${MINIMAP2_VERSION}_x64-linux/minimap2 \
     && mv ./minimap2-${MINIMAP2_VERSION}_x64-linux/minimap2 /usr/local/bin
   curl -L https://github.com/samtools/samtools/releases/download/${SAMTOOLS_VERSION}/samtools-${SAMTOOLS_VERSION}.tar.bz2 | tar -jxf - \
     && cd samtools-${SAMTOOLS_VERSION} \
     && ./configure && make all all-htslib && make install
   rm -rf samtools-${SAMTOOLS_VERSION}
 
-  apk del curl autoconf automake make gcc musl-dev ncurses-dev
+  apk del curl autoconf automake make gcc musl-dev ncurses-dev
```

### Comparing `damona-0.8.3/damona/software/seqkit/Singularity.seqkit_2.1.0` & `damona-0.9.0/damona/software/seqkit/Singularity.seqkit_2.1.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/sequana/Singularity.sequana_0.12.6` & `damona-0.9.0/damona/software/sequana/Singularity.sequana_0.12.6`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/sequana/Singularity.sequana_0.14.6` & `damona-0.9.0/damona/software/sequana/Singularity.sequana_0.14.6`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/sequana/registry.yaml` & `damona-0.9.0/damona/software/sequana/registry.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -9,7 +9,12 @@
       doi: 10.5281/zenodo.5799539
       filesize: 528461824
     0.14.6:
       download: https://zenodo.org/record/7734816/files/sequana_0.14.6.img
       md5sum: 574d01ea3b43868b2fe1f61c3b1005ae
       doi: 10.5281/zenodo.7734816
       filesize: 695410688
+    0.15.0:
+      download: https://zenodo.org/record/7863732/files/sequana_0.15.0.img
+      md5sum: 34854a9b59121b92896fb1b9f2e81fd2
+      doi: 10.5281/zenodo.7863732
+      filesize: 636309504
```

### Comparing `damona-0.8.3/damona/software/sequana_denovo/Singularity.sequana_denovo_0.0.2` & `damona-0.9.0/damona/software/sequana_denovo/Singularity.sequana_denovo_0.0.2`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/sequana_perl_tools/Singularity.sequana_perl_tools_0.1.0` & `damona-0.9.0/damona/software/sequana_perl_tools/Singularity.sequana_perl_tools_0.1.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/sequana_perl_tools/Singularity.sequana_perl_tools_0.2.0` & `damona-0.9.0/damona/software/sequana_perl_tools/Singularity.sequana_perl_tools_0.2.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/sequana_perl_tools/Singularity.sequana_perl_tools_0.3.0` & `damona-0.9.0/damona/software/sequana_perl_tools/Singularity.sequana_perl_tools_0.3.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/sequana_perl_tools/registry.yaml` & `damona-0.9.0/damona/software/sequana_perl_tools/registry.yaml`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/sequana_ribofinder/Singularity.sequana_ribofinder_0.12.0` & `damona-0.9.0/damona/software/sequana_ribofinder/Singularity.sequana_ribofinder_0.12.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/sequana_tools/Singularity.sequana_tools_0.10.0` & `damona-0.9.0/damona/software/sequana_tools/Singularity.sequana_tools_0.10.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/sequana_tools/Singularity.sequana_tools_0.11.0` & `damona-0.9.0/damona/software/sequana_tools/Singularity.sequana_tools_0.11.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/sequana_tools/Singularity.sequana_tools_0.12.0` & `damona-0.9.0/damona/software/sequana_tools/Singularity.sequana_tools_0.12.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/sequana_tools/Singularity.sequana_tools_0.14.1` & `damona-0.9.0/damona/software/sequana_tools/Singularity.sequana_tools_0.14.1`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/sequana_tools/Singularity.sequana_tools_0.14.2` & `damona-0.9.0/damona/software/sequana_tools/Singularity.sequana_tools_0.14.2`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/sequana_tools/Singularity.sequana_tools_0.14.3` & `damona-0.9.0/damona/software/sequana_tools/Singularity.sequana_tools_0.14.3`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/sequana_tools/Singularity.sequana_tools_0.9.0` & `damona-0.9.0/damona/software/sequana_tools/Singularity.sequana_tools_0.9.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/sequana_tools/registry.yaml` & `damona-0.9.0/damona/software/sequana_tools/registry.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -60,7 +60,12 @@
 
     0.14.5:
       download: https://zenodo.org/record/7341710/files/sequana_tools_0.14.5.img
       md5sum: 0b486ed2050459e469cde9eca3fd00bc
       doi: 10.5281/zenodo.7341710
       filesize: 2002989056
       binaries:  bcftools falco fastp kraken2-inspect mafft vcfutils.pl bamCoverage rnaseqc salmon inner_distance.py read_GC.py geneBody_coverage.py geneBody_coverage2.py clipping_profile.py read_duplication.py junction_annotation.py junction_saturation.py infer_experiment.py bam_stat.py dot genomeCoverageBed plotFingerprint intersectBed shustring hmmalign hmmconvert hmmfetch hmmpgmd hmmpress hmmsearch hmmstat hmmbuild hmmemit hmmlogo hmmpgmd_shard hmmscan hmmsim trinotate_report_summary.pl kallisto Build_Trinotate_Boilerplate_SQLite_db.pl Trinity seqkit seqtk sequana sequana_taxonomy nanopolish
+    0.15.1:
+      download: https://zenodo.org/record/7963917/files/sequana_tools_0.15.1.img
+      md5sum: 0e20654cecb7c70d9eba6e11571f45b7
+      doi: 10.5281/zenodo.7963917
+      filesize: 2007072768
```

### Comparing `damona-0.8.3/damona/software/snpeff/Singularity.snpeff_5.1.0` & `damona-0.9.0/damona/software/snpeff/Singularity.snpeff_5.0.0`

 * *Files 11% similar despite different names*

```diff
@@ -5,27 +5,27 @@
     Author thomas cokelaer
 
 %post
 
     apk update && apk upgrade
 
     #Add here what kind of dependencies you need in general
-    apk add --no-cache wget curl build-base git ca-certificates unzip bash openjdk11
+    apk add --no-cache wget curl build-base git ca-certificates unzip bash openjdk11 bash
 
     # Temp dir for downloading and building stuff
     TMPDIR=/build
     mkdir $TMPDIR
     cd $TMPDIR
 
     # the installation directory of snpEff
     INSTALLDIR=/usr/local/lib
     BINDIR=/usr/local/bin
 
     # at the time
-    wget https://snpeff.blob.core.windows.net/versions/snpEff_latest_core.zip
+    wget https://snpeff.blob.core.windows.net/versions/snpEff_v5_0_core.zip
 
     # Unzip snpEff archive
     ls $TMPDIR | xargs -i unzip "$TMPDIR/{}" -d $INSTALLDIR
 
     echo "#!/bin/sh" > $BINDIR/snpEff
     echo "java -jar $INSTALLDIR/snpEff/snpEff.jar \$*" >> $BINDIR/snpEff
```

### Comparing `damona-0.8.3/damona/software/trf/Singularity.trf_4.10.0` & `damona-0.9.0/damona/software/trf/Singularity.trf_4.10.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/software/ucsc/Singularity.ucsc_3.7.7` & `damona-0.9.0/damona/software/ucsc/Singularity.ucsc_3.7.7`

 * *Files identical despite different names*

### Comparing `damona-0.8.3/damona/zenodo.py` & `damona-0.9.0/damona/zenodo.py`

 * *Files 15% similar despite different names*

```diff
@@ -70,19 +70,39 @@
         published = z.publish(deposit)
 
     # if we want an update, we must create a new version from a published deposit::
 
         new_version = z.create_new_deposit_version(deposit)
 
 
+    A damona registry looks like::
+
+        ivar:
+          doi: 10.5281/zenodo.8033025
+          zenodo_id: 8033026
+          releases:
+            1.3.1:
+              download: https://zenodo.org/record/8033026/files/ivar_1.3.1.img
+              md5sum: 213e286c708e12d6423b0bd8fa723327
+              doi: 10.5281/zenodo.8033026
+              filesize: 139108352
+
+    This is create when using::
+
+        damona zenodo-upload file.img --mode zenodo
+
+    The zenodo_id is the record on the main page. e.g https://zenodo.org/record/8033026
+    The zenodo_id is also related to the main DOI to be shared in papers.
+    To cite all versions, this is the field zenodo_doi here above (8033026), which is also
+    the latest doi of the latests release. If there is a new release, the zenodo_id is therefore updated.
+
     """
 
     def __init__(self, mode="sandbox.zenodo", token=None, author=None, affiliation=None, orcid=None):
 
-
         assert mode in ["zenodo", "sandbox.zenodo"]
         self.mode = mode
         self.headers = {"Content-Type": "application/json"}
         self.last_requests = []
 
         cfg = Config()
 
@@ -177,15 +197,14 @@
         url = f"https://{self.mode}.org/api/deposit/depositions/{ID}"
         r = requests.delete(url, params=self.params, json={})
         self._status(r, [201])
         return r
 
     def upload(self, filename, json_deposit):  # pragma: no cover
 
-
         try:
             bucket_url = json_deposit["links"]["bucket"]
         except:
             bucket_url = json_deposit.json()["links"]["bucket"]
 
         jsons = {}
 
@@ -209,15 +228,15 @@
                 "title": f"Damona singularity image of {software} software",
                 "upload_type": "physicalobject",
                 "description": f"""Singularity image(s) of {software} software to be used and installed with damona
 (<a href="https://damona.readthedocs.org">See https://damona.readthedocs.org</a>) for reproducible bioinformatics
 analysis.""",
                 "keywords": ["apptainer", "singularity", "damona", "bioinformatics", "reproducibility", "container"],
                 "version": f"{version}",
-                "communities": [{"identifier": "damona"}]
+                "communities": [{"identifier": "damona"}],
             }
         }
 
         if self.orcid:
             data["metadata"]["creators"] = [{"orcid": self.orcid, "name": self.author, "affiliation": self.affiliation}]
         else:
             data["metadata"]["creators"] = [{"name": self.author, "affiliation": self.affiliation}]
@@ -273,14 +292,15 @@
     def _get_registry(self):
         print(self.mode)
 
         if self.mode == "zenodo":
             return "registry.yaml"
         elif self.mode == "sandbox.zenodo":
             return "registry_sandbox.yaml"
+
     registry_name = property(_get_registry)
 
     def _upload(self, filename):
         data = ImageName(filename)
         software = Software(data.name)
 
         if software.name:
@@ -388,25 +408,38 @@
         msg += f"      download: {record_html}/files/{basename}\n"
         msg += f"      md5sum: {md5sum}\n"
         msg += f"      doi: {this_doi}\n"
         msg += f"      filesize: {filesize}"  # no EOF
         return msg
 
 
+def get_stats_software(software):
+    from damona.registry import Software
+
+    s = Software(software)
+    try:
+        return get_stats_id(s.zenodo_id)
+    except AttributeError:
+        return 0
+
+
 def get_stats_id(ID):
-    """Returns number of downloads"""
+    """Returns number of downloads
+
+
+    For instance, for this link: https://zenodo.org/record/7319782
+    you should provide the ID 7319782
+
+
+
+    """
     from bs4 import BeautifulSoup
 
     r = requests.get(f"https://zenodo.org/record/{ID}")
     bs = BeautifulSoup(r.content, features="html.parser")
 
-    for x in bs.find(id="collapse-stats").find_all("tr"):
-        entries = []
-        for xx in x.find_all("td"):
-            entries.append(xx)
-        if len(entries):
-            if entries[0].contents[0].strip() == "Downloads":
-                stats = entries[2].contents[0]
-                return int(stats)
-
-    # if could not find the info, return -1
-    return -1
+    try:
+        data = list(bs.find(id="accordion").div.children)[3].span.contents[0]
+        data = int(data.replace(",", ""))
+        return data
+    except Exception:
+        return 1
```

### Comparing `damona-0.8.3/damona.egg-info/PKG-INFO` & `damona-0.9.0/damona.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: damona
-Version: 0.8.3
+Version: 0.9.0
 Summary: A set of NGS singularity recipes, built for you and easily downlable
 Home-page: http://github.com/sequana/sequana
-Download-URL: https://github.com/sequana/sequana/archive/0.8.3.tar.gz
+Download-URL: https://github.com/sequana/sequana/archive/0.9.0.tar.gz
 Author: Thomas Cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: Thomas Cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
 Keywords: NGS,singularity
 Platform: Linux
 Platform: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
@@ -48,15 +47,15 @@
     :target: http://damona.readthedocs.org/en/latest/?badge=latest
     :alt: Documentation Status
 
 .. image:: https://zenodo.org/badge/282275608.svg
    :target: https://zenodo.org/badge/latestdoi/282275608
 
 
-:Python version: Python 3.7, 3.8, 3.9
+:Python version: Python 3.8, 3.9, 3.10
 :Source: See  `http://github.com/cokelaer/damona <https://github.com/cokelaer/damona/>`__.
 :Issues: Please fill a report on `github <https://github.com/cokelaer/damona/issues>`__
 :Platform: This is currently only available for Linux distribution with bash shell (contributions are welcome to port the tool on MacOSX and other platforms)
 
 Overview
 ========
 
@@ -68,14 +67,15 @@
 Damona is now used in production to create reproducible environments where singularity images and their associated binaries are installed altogether.
 
 In a nutshell, Damona combines the logic of Conda environments with the
 reproducibility of singularity containers. We believe that it could be useful for
 other projects and therefore decided to release it as an independent tool.
 
 As of 30th Dec 2021, **Damona** contains 26 software, 38 releases, 105 binaries.
+As of 12th May 2023, **Damona** contains 54 software, 88 releases, 359 binaries.
 
 Installation
 ============
 
 If you are in a hurry, just type::
 
     pip install damona --upgrade
@@ -246,15 +246,15 @@
 
     damona env
 
 2. *create* environments
 ------------------------
 All environments are stored in *~/.config/damona/envs/*. You can create a new one as follows::
 
-    damona env --create TEST
+    damona create TEST
 
 There, you have a *bin* directory where binaries are going to be installed.
 
 You can check that it has been created::
 
     damona env
 
@@ -345,15 +345,15 @@
 
 7. combine two different environments
 --------------------------------------
 
 In damona, you can have sereral environments in parallel and later activate the
 one you wish to use. Let us create a new one::
 
-    damone env --create test1
+    damone create test1
 
 and check that you now have one more environment::
 
     damona env
 
 We want to create an alias to the previously downloaded image of fastqc tool but
 in the *test1* environment. First we activate the newly create environment::
@@ -378,14 +378,24 @@
 
 Changelog
 =========
 
 ========= ========================================================================
 Version   Description
 ========= ========================================================================
+0.9.0     * refactorise the command 'env' by splitting into dedicated subcommands
+            create, delete, rename. add progress bar when downloading container
+          * NEW micromamba image to work as a localimage
+          * NEW sequana_minimal package to hold common tools (bwa, samtools,
+            kraken, etc)
+          * NEW ivarm pangolin, nextclade, subread, mafft packages
+          * UPDATE fastp to 0.23.3, gffread to 0.12.7 (3 times lighter).
+          * UPDATE sequana_tools to use micromamba (30% lighter)
+0.8.4     * fix damona stats command to return unique binaries
+          * more recipes and version (e.g. fastqc 0.12.1, graphviz update, etc)
 0.8.3     * create registry specifically for the sandbox (for testing)
           * add damona community in the uploads
           * add pbbam, bioconvert, busco, canu, ccs
           * add polypolish, samtools 1.16.1, sequana 0.14.6, flye 2.9, canu 2.1.1
             circlator 1.5.5, hifiasm
 0.8.2     * add idr, samtools, homer, bamtools, bedtools, sequana_denovo
           * add seqkit recipe and container
```

### Comparing `damona-0.8.3/damona.egg-info/SOURCES.txt` & `damona-0.9.0/damona.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 damona/builders.py
 damona/common.py
 damona/config.py
 damona/environ.py
 damona/install.py
 damona/registry.py
 damona/script.py
+damona/utils.py
 damona/zenodo.py
 damona.egg-info/PKG-INFO
 damona.egg-info/SOURCES.txt
 damona.egg-info/dependency_links.txt
 damona.egg-info/entry_points.txt
 damona.egg-info/not-zip-safe
 damona.egg-info/requires.txt
@@ -32,17 +33,21 @@
 damona/biocontainers/registry.yaml
 damona/library/__init__.py
 damona/library/R/Makefile
 damona/library/R/Singularity.R_3.6.3
 damona/library/R/Singularity.R_4.0.2
 damona/library/R/registry.yaml
 damona/library/conda/README.rst
+damona/library/conda/Singularity.conda_23.5.0
 damona/library/conda/Singularity.conda_4.7.12
 damona/library/conda/Singularity.conda_4.9.2
+damona/library/conda/Singularity.conda_4.9.3
 damona/library/conda/registry.yaml
+damona/library/micromamba/Singularity.micromamba_1.4.3
+damona/library/micromamba/registry.yaml
 damona/library/rust/Singularity.rust
 damona/library/ubuntu/Singularity.ubuntu_16.04
 damona/library/ubuntu/Singularity.ubuntu_18.04
 damona/library/ubuntu/registry.yaml
 damona/papers/__init__.py
 damona/shell/__init__.py
 damona/shell/damona_comp.sh
@@ -55,57 +60,64 @@
 damona/software/art/Singularity.art_2.5.8
 damona/software/art/Singularity.art_3.11.14
 damona/software/art/registry.yaml
 damona/software/bamtools/Singularity.bamtools_2.5.2
 damona/software/bamtools/registry.yaml
 damona/software/bbtools/Singularity.bbtools_38.94.0
 damona/software/bbtools/registry.yaml
-damona/software/bcl2fastq/Makefile
 damona/software/bcl2fastq/README.rst
 damona/software/bcl2fastq/Singularity.bcl2fastq_2.20.0
 damona/software/bcl2fastq/registry.yaml
 damona/software/bedtools/Singularity.bedtools_2.30.0
 damona/software/bedtools/registry.yaml
 damona/software/bioconvert/Singularity.bioconvert_0.6.1
 damona/software/bioconvert/Singularity.bioconvert_0.6.2
 damona/software/bioconvert/Singularity.bioconvert_0.6.3
 damona/software/bioconvert/Singularity.bioconvert_1.0.0
 damona/software/bioconvert/registry.yaml
+damona/software/blast/Singularity.blast_2.12.0
+damona/software/blast/registry.yaml
 damona/software/bowtie/Singularity.bowtie_1.3.1
 damona/software/bowtie/registry.yaml
 damona/software/bowtie2/Singularity.bowtie2_2.3.4
 damona/software/bowtie2/Singularity.bowtie2_2.4.2
 damona/software/bowtie2/registry.yaml
 damona/software/busco/Singularity.busco_5.4.6
 damona/software/busco/registry.yaml
 damona/software/bwa/Singularity.bwa_0.7.17
+damona/software/bwa/Singularity.bwa_mamba_0.7.17
 damona/software/bwa/registry.yaml
 damona/software/canu/Singularity.canu_1.6.0
 damona/software/canu/Singularity.canu_1.8.0
 damona/software/canu/Singularity.canu_2.1.1
 damona/software/canu/registry.yaml
 damona/software/ccs/Singularity.ccs_6.4.0
 damona/software/ccs/registry.yaml
+damona/software/cellranger/Singularity.cellranger_7.1.0
 damona/software/circlator/Singularity.circlator_1.5.5
 damona/software/circlator/registry.yaml
 damona/software/falco/Singularity.falco_0.2.1
 damona/software/falco/Singularity.falco_1.0.0
 damona/software/falco/registry.yaml
 damona/software/fastp/Singularity.fastp_0.23.2
+damona/software/fastp/Singularity.fastp_0.23.3
 damona/software/fastp/registry.yaml
 damona/software/fastqc/Singularity.fastqc_0.11.8
 damona/software/fastqc/Singularity.fastqc_0.11.9
 damona/software/fastqc/Singularity.fastqc_0.11.9_py3
+damona/software/fastqc/Singularity.fastqc_0.12.1
 damona/software/fastqc/registry.yaml
 damona/software/flye/Singularity.flye_2.9.0
 damona/software/flye/Singularity.flye_2.9.1
 damona/software/flye/registry.yaml
 damona/software/gffread/Singularity.gffread_0.12.1
+damona/software/gffread/Singularity.gffread_0.12.7
 damona/software/gffread/registry.yaml
 damona/software/graphviz/Singularity.graphviz_2.43.0
+damona/software/graphviz/Singularity.graphviz_7.0.5
 damona/software/graphviz/registry.yaml
 damona/software/graphviz/test.dot
 damona/software/graphviz/test.sh
 damona/software/gzip/Singularity.gzip_1.9.0
 damona/software/gzip/registry.yaml
 damona/software/hifiasm/Singularity.hifiasm_0.19.1
 damona/software/hifiasm/registry.yaml
@@ -113,40 +125,54 @@
 damona/software/hisat2/registry.yaml
 damona/software/homer/Singularity.homer_4.11.0
 damona/software/homer/registry.yaml
 damona/software/idr/Singularity.idr_2.0.3
 damona/software/idr/registry.yaml
 damona/software/igvtools/Singularity.igvtools_2.12.0
 damona/software/igvtools/registry.yaml
+damona/software/ivar/Singularity.ivar_1.3.1
+damona/software/ivar/registry.yaml
 damona/software/kraken/Makefile
 damona/software/kraken/Singularity.kraken_1.1.0
 damona/software/kraken/Singularity.kraken_2.0.9
 damona/software/kraken/registry.yaml
+damona/software/mafft/Singularity.mafft_7.520.0
+damona/software/mafft/registry.yaml
+damona/software/medaka/Singularity.medaka_1.7.3
+damona/software/medaka/registry.yaml
 damona/software/mergegi/Singularity.mergegi_0.0.1
 damona/software/mergegi/registry.yaml
 damona/software/minimap2/Singularity.minimap2_2.17.0
 damona/software/minimap2/Singularity.minimap2_2.23.0
 damona/software/minimap2/Singularity.minimap2_2.24.0
 damona/software/minimap2/registry.yaml
+damona/software/nextclade/Singularity.nextclade_2.15.0
+damona/software/nextclade/registry.yaml
+damona/software/pangolin/Singularity.pangolin_4.3.0
+damona/software/pangolin/registry.yaml
 damona/software/pbbam/Singularity.pbbam_2.1.0
 damona/software/pbbam/Singularity.pbbam_2.3.0
 damona/software/pbbam/registry.yaml
 damona/software/phantompeakqualtools/Singularity.phantompeakqualtools_1.2.2
 damona/software/phantompeakqualtools/registry.yaml
 damona/software/picard/Singularity.picard_2.26
 damona/software/pigz/Singularity.pigz_2.4.0
 damona/software/pigz/registry.yaml
 damona/software/polypolish/Singularity.polypolish_0.5.0
 damona/software/polypolish/registry.yaml
 damona/software/prokka/Singularity.prokka_1.14.5
+damona/software/prokka/Singularity.prokka_1.14.6
 damona/software/prokka/registry.yaml
 damona/software/pycoqc/Singularity.pycoqc_2.5.2
 damona/software/pycoqc/registry.yaml
 damona/software/quast/Singularity.quast_5.0.2
+damona/software/quast/Singularity.quast_5.2.0
 damona/software/quast/registry.yaml
+damona/software/raxml/Singularity.raxml_8.2.12
+damona/software/raxml/registry.yaml
 damona/software/rnadiff/Singularity.rnadiff_1.7.1
 damona/software/rnadiff/registry.yaml
 damona/software/rnaseqc/Singularity.rnaseqc_2.35.0
 damona/software/rnaseqc/registry.yaml
 damona/software/rtools/Singularity.rtools_1.0.0
 damona/software/rtools/Singularity.rtools_1.1.0
 damona/software/rtools/Singularity.rtools_1.2.0
@@ -162,35 +188,45 @@
 damona/software/seqkit/Singularity.seqkit_2.1.0
 damona/software/seqkit/Singularity.seqkit_2.4.0
 damona/software/seqkit/registry.yaml
 damona/software/seqtk/Singularity.seqtk_1.3.0
 damona/software/seqtk/registry.yaml
 damona/software/sequana/Singularity.sequana_0.12.6
 damona/software/sequana/Singularity.sequana_0.14.6
+damona/software/sequana/Singularity.sequana_0.15.0
 damona/software/sequana/registry.yaml
 damona/software/sequana_denovo/Singularity.sequana_denovo_0.0.2
 damona/software/sequana_denovo/registry.yaml
+damona/software/sequana_minimal/Singularity.sequana_minimal_23.6.13
+damona/software/sequana_minimal/registry.yaml
 damona/software/sequana_perl_tools/Singularity.sequana_perl_tools_0.1.0
 damona/software/sequana_perl_tools/Singularity.sequana_perl_tools_0.2.0
 damona/software/sequana_perl_tools/Singularity.sequana_perl_tools_0.3.0
 damona/software/sequana_perl_tools/registry.yaml
 damona/software/sequana_ribofinder/Singularity.sequana_ribofinder_0.12.0
 damona/software/sequana_ribofinder/registry.yaml
 damona/software/sequana_tools/README.txt
 damona/software/sequana_tools/Singularity.sequana_tools_0.10.0
 damona/software/sequana_tools/Singularity.sequana_tools_0.11.0
 damona/software/sequana_tools/Singularity.sequana_tools_0.12.0
 damona/software/sequana_tools/Singularity.sequana_tools_0.14.1
 damona/software/sequana_tools/Singularity.sequana_tools_0.14.2
 damona/software/sequana_tools/Singularity.sequana_tools_0.14.3
 damona/software/sequana_tools/Singularity.sequana_tools_0.14.5
-damona/software/sequana_tools/Singularity.sequana_tools_0.14.6
+damona/software/sequana_tools/Singularity.sequana_tools_0.15.1
 damona/software/sequana_tools/Singularity.sequana_tools_0.9.0
+damona/software/sequana_tools/Singularity.sequana_tools_23.6.13
 damona/software/sequana_tools/registry.yaml
 damona/software/shustring/Singularity.shustring_2.6.0
 damona/software/shustring/registry.yaml
+damona/software/snpeff/Singularity.snpeff_5.0.0
 damona/software/snpeff/Singularity.snpeff_5.1.0
+damona/software/snpeff/registry.yaml
+damona/software/subread/Singularity.subread_2.0.3
+damona/software/subread/registry.yaml
 damona/software/trf/Singularity.trf_4.10.0
 damona/software/trf/registry.yaml
 damona/software/ucsc/README.rst
 damona/software/ucsc/Singularity.ucsc_3.7.7
-damona/software/ucsc/registry.yaml
+damona/software/ucsc/registry.yaml
+damona/software/vt/Singularity.vt_0.57721.0
+damona/software/vt/registry.yaml
```

### Comparing `damona-0.8.3/setup.py` & `damona-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 import os
 from setuptools import setup, find_packages
 import glob
 
 _MAJOR               = 0
-_MINOR               = 8
-_MICRO               = 3
+_MINOR               = 9
+_MICRO               = 0
 version              = '%d.%d.%d' % (_MAJOR, _MINOR, _MICRO)
 release              = '%d.%d' % (_MAJOR, _MINOR)
 
 
 metainfo = {
     'authors': {"main": ("Thomas Cokelaer", "thomas.cokelaer@pasteur.fr")},
     'maintainer': {"main": ("Thomas Cokelaer", "thomas.cokelaer@pasteur.fr")},
@@ -22,15 +22,14 @@
     'keywords' : ['NGS', 'singularity'],
     'classifiers' : [
           'Development Status :: 5 - Production/Stable',
           'Intended Audience :: Developers',
           'Intended Audience :: Science/Research',
           'License :: OSI Approved :: BSD License',
           'Operating System :: OS Independent',
-          'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
           'Topic :: Software Development :: Libraries :: Python Modules',
           'Topic :: Scientific/Engineering :: Bio-Informatics',
           'Topic :: Scientific/Engineering :: Information Analysis',
           'Topic :: Scientific/Engineering :: Mathematics',
```

