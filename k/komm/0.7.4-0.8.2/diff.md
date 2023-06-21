# Comparing `tmp/komm-0.7.4.tar.gz` & `tmp/komm-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "komm-0.7.4.tar", last modified: Wed May 24 20:32:30 2023, max compression
+gzip compressed data, was "komm-0.8.2.tar", last modified: Wed Jun 21 01:32:33 2023, max compression
```

## Comparing `komm-0.7.4.tar` & `komm-0.8.2.tar`

### file list

```diff
@@ -1,40 +1,112 @@
-drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-05-24 20:32:30.483378 komm-0.7.4/
--rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    35147 2022-07-22 15:17:50.000000 komm-0.7.4/LICENSE
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1372 2023-05-24 20:32:30.483378 komm-0.7.4/PKG-INFO
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1757 2023-05-13 23:19:40.000000 komm-0.7.4/README.rst
-drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-05-24 20:32:30.473378 komm-0.7.4/komm/
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      620 2023-05-13 23:18:38.000000 komm-0.7.4/komm/__init__.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    32335 2023-05-13 23:09:56.000000 komm-0.7.4/komm/_algebra.py
--rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      189 2022-07-22 15:17:50.000000 komm-0.7.4/komm/_aux.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    15361 2023-05-24 18:32:24.000000 komm-0.7.4/komm/_channels.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    67646 2023-05-13 23:12:00.000000 komm-0.7.4/komm/_error_control_block.py
--rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      123 2022-07-22 15:17:50.000000 komm-0.7.4/komm/_error_control_checksum.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    20369 2023-05-13 23:09:56.000000 komm-0.7.4/komm/_error_control_convolutional.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    18086 2023-05-13 23:08:37.000000 komm-0.7.4/komm/_finite_state_machine.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    30566 2023-05-13 23:11:52.000000 komm-0.7.4/komm/_modulation.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    14874 2023-05-13 23:08:37.000000 komm-0.7.4/komm/_pulses.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     8251 2023-05-13 23:08:37.000000 komm-0.7.4/komm/_quantization.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    19729 2023-05-13 23:08:28.000000 komm-0.7.4/komm/_sequences.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    19050 2022-07-22 15:17:50.000000 komm-0.7.4/komm/_source_coding.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2484 2023-05-24 18:32:24.000000 komm-0.7.4/komm/_sources.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     5469 2023-05-24 18:32:24.000000 komm-0.7.4/komm/_util.py
-drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-05-24 20:32:30.473378 komm-0.7.4/komm.egg-info/
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1372 2023-05-24 20:32:30.000000 komm-0.7.4/komm.egg-info/PKG-INFO
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      791 2023-05-24 20:32:30.000000 komm-0.7.4/komm.egg-info/SOURCES.txt
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        1 2023-05-24 20:32:30.000000 komm-0.7.4/komm.egg-info/dependency_links.txt
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)       12 2023-05-24 20:32:30.000000 komm-0.7.4/komm.egg-info/requires.txt
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        5 2023-05-24 20:32:30.000000 komm-0.7.4/komm.egg-info/top_level.txt
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)       38 2023-05-24 20:32:30.483378 komm-0.7.4/setup.cfg
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1623 2023-05-24 20:31:35.000000 komm-0.7.4/setup.py
-drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-05-24 20:32:30.483378 komm-0.7.4/tests/
--rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     7141 2022-07-22 15:17:50.000000 komm-0.7.4/tests/test_algebra.py
--rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      509 2022-07-22 15:17:50.000000 komm-0.7.4/tests/test_channels.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    14875 2023-05-13 23:08:28.000000 komm-0.7.4/tests/test_error_control_block.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     8605 2023-05-13 23:08:28.000000 komm-0.7.4/tests/test_error_control_convolutional.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2661 2022-07-22 15:17:50.000000 komm-0.7.4/tests/test_finite_state_machine.py
--rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1860 2022-07-22 15:17:50.000000 komm-0.7.4/tests/test_modulation.py
--rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1802 2022-07-22 15:17:50.000000 komm-0.7.4/tests/test_quantization.py
--rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      976 2023-05-13 23:08:28.000000 komm-0.7.4/tests/test_sequences.py
--rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     3028 2022-07-22 15:17:50.000000 komm-0.7.4/tests/test_source_coding.py
--rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      289 2023-05-13 23:08:28.000000 komm-0.7.4/tests/test_sources.py
--rw-------   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      509 2022-07-22 15:17:50.000000 komm-0.7.4/tests/test_util.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:32:33.418661 komm-0.8.2/
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    35147 2023-05-13 23:05:18.000000 komm-0.8.2/LICENSE
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2076 2023-06-21 01:32:33.418661 komm-0.8.2/PKG-INFO
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1612 2023-06-20 12:29:42.000000 komm-0.8.2/README.md
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      835 2023-06-21 01:31:54.000000 komm-0.8.2/pyproject.toml
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)       38 2023-06-21 01:32:33.418661 komm-0.8.2/setup.cfg
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:32:33.395328 komm-0.8.2/src/
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:32:33.398661 komm-0.8.2/src/komm/
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      418 2023-06-17 03:53:41.000000 komm-0.8.2/src/komm/__init__.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:32:33.401995 komm-0.8.2/src/komm/_algebra/
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     7114 2023-06-17 03:53:41.000000 komm-0.8.2/src/komm/_algebra/BinaryPolynomial.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2678 2023-06-13 13:41:29.000000 komm-0.8.2/src/komm/_algebra/BinaryPolynomialFraction.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     9049 2023-06-13 13:41:29.000000 komm-0.8.2/src/komm/_algebra/FiniteBifield.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     7463 2023-06-13 13:41:29.000000 komm-0.8.2/src/komm/_algebra/RationalPolynomial.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     3577 2023-06-13 13:41:29.000000 komm-0.8.2/src/komm/_algebra/RationalPolynomialFraction.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      269 2023-06-01 00:49:38.000000 komm-0.8.2/src/komm/_algebra/__init__.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     4028 2023-06-13 13:41:29.000000 komm-0.8.2/src/komm/_algebra/util.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      192 2023-06-06 01:42:18.000000 komm-0.8.2/src/komm/_aux.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:32:33.401995 komm-0.8.2/src/komm/_channels/
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     3469 2023-06-20 02:19:25.000000 komm-0.8.2/src/komm/_channels/AWGNChannel.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2580 2023-06-20 02:20:49.000000 komm-0.8.2/src/komm/_channels/BinaryErasureChannel.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2716 2023-06-20 02:20:05.000000 komm-0.8.2/src/komm/_channels/BinarySymmetricChannel.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     5967 2023-06-20 17:22:46.000000 komm-0.8.2/src/komm/_channels/DiscreteMemorylessChannel.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      216 2023-06-01 00:48:34.000000 komm-0.8.2/src/komm/_channels/__init__.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:32:33.405328 komm-0.8.2/src/komm/_error_control_block/
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     7276 2023-06-16 01:34:25.000000 komm-0.8.2/src/komm/_error_control_block/BCHCode.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    19826 2023-06-17 03:53:41.000000 komm-0.8.2/src/komm/_error_control_block/BlockCode.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1915 2023-06-16 00:23:48.000000 komm-0.8.2/src/komm/_error_control_block/CordaroWagnerCode.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     9304 2023-06-16 00:53:27.000000 komm-0.8.2/src/komm/_error_control_block/CyclicCode.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2612 2023-06-16 00:21:22.000000 komm-0.8.2/src/komm/_error_control_block/GolayCode.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     3499 2023-06-16 00:23:33.000000 komm-0.8.2/src/komm/_error_control_block/HammingCode.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     7132 2023-06-16 00:23:41.000000 komm-0.8.2/src/komm/_error_control_block/ReedMullerCode.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2435 2023-06-16 00:23:37.000000 komm-0.8.2/src/komm/_error_control_block/RepetitionCode.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2073 2023-06-16 00:24:47.000000 komm-0.8.2/src/komm/_error_control_block/SimplexCode.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2408 2023-06-16 00:23:35.000000 komm-0.8.2/src/komm/_error_control_block/SingleParityCheckCode.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      396 2023-06-01 00:49:32.000000 komm-0.8.2/src/komm/_error_control_block/__init__.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:32:33.405328 komm-0.8.2/src/komm/_error_control_checksum/
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      102 2023-06-01 00:49:44.000000 komm-0.8.2/src/komm/_error_control_checksum/CyclicRedundancyCheck.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)       57 2023-06-01 00:49:46.000000 komm-0.8.2/src/komm/_error_control_checksum/__init__.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:32:33.405328 komm-0.8.2/src/komm/_error_control_convolutional/
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    14843 2023-06-17 03:53:41.000000 komm-0.8.2/src/komm/_error_control_convolutional/ConvolutionalCode.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     3043 2023-06-17 03:53:41.000000 komm-0.8.2/src/komm/_error_control_convolutional/ConvolutionalStreamDecoder.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1554 2023-06-17 03:53:36.000000 komm-0.8.2/src/komm/_error_control_convolutional/ConvolutionalStreamEncoder.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    11569 2023-06-17 03:53:41.000000 komm-0.8.2/src/komm/_error_control_convolutional/TerminatedConvolutionalCode.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      252 2023-06-01 00:49:57.000000 komm-0.8.2/src/komm/_error_control_convolutional/__init__.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:32:33.405328 komm-0.8.2/src/komm/_finite_state_machine/
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    16691 2023-06-13 13:41:29.000000 komm-0.8.2/src/komm/_finite_state_machine/FiniteStateMachine.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)       51 2023-06-01 00:50:36.000000 komm-0.8.2/src/komm/_finite_state_machine/__init__.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:32:33.408661 komm-0.8.2/src/komm/_modulation/
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     4066 2023-06-20 02:11:47.000000 komm-0.8.2/src/komm/_modulation/APSKModulation.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2736 2023-06-20 01:44:54.000000 komm-0.8.2/src/komm/_modulation/ASKModulation.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    12099 2023-06-20 18:39:44.000000 komm-0.8.2/src/komm/_modulation/Modulation.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2287 2023-06-20 01:45:29.000000 komm-0.8.2/src/komm/_modulation/PAModulation.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2853 2023-06-20 01:45:02.000000 komm-0.8.2/src/komm/_modulation/PSKModulation.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     5530 2023-06-20 01:45:12.000000 komm-0.8.2/src/komm/_modulation/QAModulation.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      238 2023-06-20 01:16:54.000000 komm-0.8.2/src/komm/_modulation/__init__.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1294 2023-06-01 00:51:22.000000 komm-0.8.2/src/komm/_modulation/util.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:32:33.408661 komm-0.8.2/src/komm/_pulses/
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1274 2023-06-21 00:07:43.000000 komm-0.8.2/src/komm/_pulses/FormattingPulse.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2316 2023-06-21 00:07:43.000000 komm-0.8.2/src/komm/_pulses/GaussianPulse.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      951 2023-06-21 00:07:43.000000 komm-0.8.2/src/komm/_pulses/ManchesterPulse.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2460 2023-06-21 00:07:43.000000 komm-0.8.2/src/komm/_pulses/RaisedCosinePulse.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)       90 2023-06-06 01:42:18.000000 komm-0.8.2/src/komm/_pulses/ReceiveFilter.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1617 2023-06-21 00:07:43.000000 komm-0.8.2/src/komm/_pulses/RectangularPulse.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2528 2023-06-21 00:07:43.000000 komm-0.8.2/src/komm/_pulses/RootRaisedCosinePulse.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1226 2023-06-21 00:07:43.000000 komm-0.8.2/src/komm/_pulses/SincPulse.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1365 2023-06-21 00:07:43.000000 komm-0.8.2/src/komm/_pulses/TransmitFilter.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      356 2023-06-21 00:07:43.000000 komm-0.8.2/src/komm/_pulses/__init__.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:32:33.411995 komm-0.8.2/src/komm/_quantization/
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      172 2023-06-13 13:41:29.000000 komm-0.8.2/src/komm/_quantization/LloydMaxQuantizer.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     3601 2023-06-13 13:41:29.000000 komm-0.8.2/src/komm/_quantization/ScalarQuantizer.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     4514 2023-06-13 13:41:29.000000 komm-0.8.2/src/komm/_quantization/UniformQuantizer.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      141 2023-06-01 00:52:43.000000 komm-0.8.2/src/komm/_quantization/__init__.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:32:33.415328 komm-0.8.2/src/komm/_sequences/
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1895 2023-06-13 13:41:29.000000 komm-0.8.2/src/komm/_sequences/BarkerSequence.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     4483 2023-06-18 23:40:21.000000 komm-0.8.2/src/komm/_sequences/BinarySequence.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     3047 2023-06-18 23:41:15.000000 komm-0.8.2/src/komm/_sequences/ComplexSequence.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      149 2023-06-06 01:42:18.000000 komm-0.8.2/src/komm/_sequences/GoldSequence.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      153 2023-06-06 01:42:18.000000 komm-0.8.2/src/komm/_sequences/KasamiSequence.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     6920 2023-06-19 02:08:59.000000 komm-0.8.2/src/komm/_sequences/LFSRSequence.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     4923 2023-06-19 00:06:38.000000 komm-0.8.2/src/komm/_sequences/WalshHadamardSequence.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2865 2023-06-19 23:56:43.000000 komm-0.8.2/src/komm/_sequences/ZadoffChuSequence.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      358 2023-06-17 16:09:32.000000 komm-0.8.2/src/komm/_sequences/__init__.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:32:33.415328 komm-0.8.2/src/komm/_source_coding/
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     6572 2023-06-15 18:52:28.000000 komm-0.8.2/src/komm/_source_coding/FixedToVariableCode.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     3895 2023-06-15 20:06:05.000000 komm-0.8.2/src/komm/_source_coding/HuffmanCode.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2788 2023-06-15 20:06:05.000000 komm-0.8.2/src/komm/_source_coding/TunstallCode.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     6017 2023-06-15 20:06:05.000000 komm-0.8.2/src/komm/_source_coding/VariableToFixedCode.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      182 2023-06-01 00:53:25.000000 komm-0.8.2/src/komm/_source_coding/__init__.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      424 2023-06-01 00:53:27.000000 komm-0.8.2/src/komm/_source_coding/util.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:32:33.415328 komm-0.8.2/src/komm/_sources/
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2253 2023-06-20 02:23:08.000000 komm-0.8.2/src/komm/_sources/DiscreteMemorylessSource.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)       63 2023-06-01 00:53:36.000000 komm-0.8.2/src/komm/_sources/__init__.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:32:33.418661 komm-0.8.2/src/komm/_util/
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1046 2023-06-18 23:05:20.000000 komm-0.8.2/src/komm/_util/__init__.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2037 2023-06-17 03:57:16.000000 komm-0.8.2/src/komm/_util/bit_operations.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     3214 2023-06-18 23:36:30.000000 komm-0.8.2/src/komm/_util/correlation.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2415 2023-06-20 17:22:17.000000 komm-0.8.2/src/komm/_util/information_theory.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1140 2023-06-17 03:55:28.000000 komm-0.8.2/src/komm/_util/special_functions.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:32:33.401995 komm-0.8.2/src/komm.egg-info/
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2076 2023-06-21 01:32:33.000000 komm-0.8.2/src/komm.egg-info/PKG-INFO
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     3506 2023-06-21 01:32:33.000000 komm-0.8.2/src/komm.egg-info/SOURCES.txt
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        1 2023-06-21 01:32:33.000000 komm-0.8.2/src/komm.egg-info/dependency_links.txt
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)       74 2023-06-21 01:32:33.000000 komm-0.8.2/src/komm.egg-info/requires.txt
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        5 2023-06-21 01:32:33.000000 komm-0.8.2/src/komm.egg-info/top_level.txt
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:32:33.418661 komm-0.8.2/tests/
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     7158 2023-06-06 01:42:18.000000 komm-0.8.2/tests/test_algebra.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      510 2023-06-01 00:55:24.000000 komm-0.8.2/tests/test_channels.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     9462 2023-06-01 00:55:29.000000 komm-0.8.2/tests/test_error_control_convolutional.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2781 2023-06-01 00:55:31.000000 komm-0.8.2/tests/test_finite_state_machine.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1802 2023-06-01 00:55:36.000000 komm-0.8.2/tests/test_quantization.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      290 2023-06-01 00:55:44.000000 komm-0.8.2/tests/test_sources.py
```

### Comparing `komm-0.7.4/LICENSE` & `komm-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `komm-0.7.4/komm/_error_control_convolutional.py` & `komm-0.8.2/src/komm/_error_control_convolutional/ConvolutionalCode.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,179 +1,160 @@
 import numpy as np
 
-from ._algebra import \
-    BinaryPolynomial, BinaryPolynomialFraction
-
-from ._finite_state_machine import \
-    FiniteStateMachine
-
-from ._util import \
-    int2binlist, binlist2int, pack, unpack
-
-
-__all__ = ['ConvolutionalCode', 'ConvolutionalStreamEncoder', 'ConvolutionalStreamDecoder']
+from .._algebra import BinaryPolynomial, BinaryPolynomialFraction
+from .._finite_state_machine import FiniteStateMachine
+from .._util import binlist2int, int2binlist
 
 
 class ConvolutionalCode:
-    """
-    Binary convolutional code. It is characterized by a *matrix of feedforward polynomials* :math:`P(D)`, of shape :math:`k \\times n`, and (optionally) by a *vector of feedback polynomials* :math:`q(D)`, of length :math:`k`. The element in row :math:`i` and column :math:`j` of :math:`P(D)` is denoted by :math:`p_{i,j}(D)`, and the element in position :math:`i` of :math:`q(D)` is denoted by :math:`q_i(D)`; they are binary polynomials (:class:`BinaryPolynomial`) in :math:`D`. The parameters :math:`k` and :math:`n` are the number of input and output bits per block, respectively.
+    r"""
+    Binary convolutional code. It is characterized by a *matrix of feedforward polynomials* $P(D)$, of shape $k \times n$, and (optionally) by a *vector of feedback polynomials* $q(D)$, of length $k$. The element in row $i$ and column $j$ of $P(D)$ is denoted by $p_{i,j}(D)$, and the element in position $i$ of $q(D)$ is denoted by $q_i(D)$; they are [binary polynomials](/ref/BinaryPolynomial) in $D$. The parameters $k$ and $n$ are the number of input and output bits per block, respectively.
 
-    The *transfer function matrix* (also known as *transform-domain generator matrix*) :math:`G(D)` of the convolutional code, of shape :math:`k \\times n`, is such that the element in row :math:`i` and column :math:`j` is given by
+    The *transfer function matrix* (also known as *transform-domain generator matrix*) $G(D)$ of the convolutional code, of shape $k \times n$, is such that the element in row $i$ and column $j$ is given by
+    $$
+        g_{i,j}(D) = \frac{p_{i,j}(D)}{q_{i}(D)},
+    $$
+    for $i \in [0 : k)$ and $j \in [0 : n)$.
 
-    .. math::
-       g_{i,j}(D) = \\frac{p_{i,j}(D)}{q_{i}(D)},
-
-    for :math:`i \\in [0 : k)` and :math:`j \\in [0 : n)`.
-
-    .. rubric:: Constraint lenghts and related parameters
+    <h2>Constraint lengths and related parameters</h2>
 
     The *constraint lengths* of the code are defined by
-
-    .. math::
-       \\nu_i = \\max \\{ \\deg p_{i,0}(D), \\deg p_{i,1}(D), \\ldots, \\deg p_{i,n-1}(D), \\deg q_i(D) \\},
-
-    for :math:`i \\in [0 : k)`.
+    $$
+        \nu_i = \max \\{ \deg p_{i,0}(D), \deg p_{i,1}(D), \ldots, \deg p_{i,n-1}(D), \deg q_i(D) \\},
+    $$
+    for $i \in [0 : k)$.
 
     The *overall constraint length* of the code is defined by
-
-    .. math::
-       \\nu = \\sum_{0 \\leq i < k} \\nu_i.
+    $$
+        \nu = \sum_{0 \leq i < k} \nu_i.
+    $$
 
     The *memory order* of the code is defined by
+    $$
+        \mu = \max_{0 \leq i < k} \nu_i.
+    $$
+
+    <h2>Space-state representation</h2>
+
+    A convolutional code may also be described via the *space-state representation*. Let $\mathbf{u}_t = (u_t^{(0)}, u_t^{(1)}, \ldots, u_t^{(k-1)})$ be the input block, $\mathbf{v}_t = (v_t^{(0)}, v_t^{(1)}, \ldots, v_t^{(n-1)})$ be the output block, and $\mathbf{s}_t = (s_t^{(0)}, s_t^{(1)}, \ldots, s_t^{(\nu-1)})$ be the state, all defined at time instant $t$. Then,
+    $$
+    \begin{aligned}
+        \mathbf{s}\_{t+1} & = \mathbf{s}_t A + \mathbf{u}_t B, \\\\
+        \mathbf{v}\_{t} & = \mathbf{s}_t C + \mathbf{u}\_t D,
+    \end{aligned}
+    $$
+    where $A$ is the $\nu \times \nu$ *state matrix*, $B$ is the $k \times \nu$ *control matrix*, $C$ is the $\nu \times n$ *observation matrix*, and $D$ is the $k \times n$ *transition matrix*.
+
+    <h2>Tables of convolutional codes</h2>
+
+    The tables below <cite>LC04, Sec. 12.3</cite> lists optimal convolutional codes with parameters $(n,k) = (2,1)$ and $(n,k) = (3,1)$, for small values of the overall constraint length $\nu$.
+
+    | Parameters $(n, k, \nu)$ | Transfer function matrix $G(D)$ |
+    | :----------------------: | ------------------------------- |
+    | $(2, 1, 1)$              | `[[0o1, 0o3]]`                  |
+    | $(2, 1, 2)$              | `[[0o5, 0o7]]`                  |
+    | $(2, 1, 3)$              | `[[0o13, 0o17]]`                |
+    | $(2, 1, 4)$              | `[[0o27, 0o31]]`                |
+    | $(2, 1, 5)$              | `[[0o53, 0o75]]`                |
+    | $(2, 1, 6)$              | `[[0o117, 0o155]]`              |
+    | $(2, 1, 7)$              | `[[0o247, 0o371]]`              |
+    | $(2, 1, 8)$              | `[[0o561, 0o753]]`              |
+
+    | Parameters $(n, k, \nu)$ | Transfer function matrix $G(D)$ |
+    | :----------------------: | ------------------------------- |
+    | $(3, 1, 1)$              | `[[0o1, 0o3, 0o3]]`             |
+    | $(3, 1, 2)$              | `[[0o5, 0o7, 0o7]]`             |
+    | $(3, 1, 3)$              | `[[0o13, 0o15, 0o17]]`          |
+    | $(3, 1, 4)$              | `[[0o25, 0o33, 0o37]]`          |
+    | $(3, 1, 5)$              | `[[0o47, 0o53, 0o75]]`          |
+    | $(3, 1, 6)$              | `[[0o117, 0o127, 0o155]]`       |
+    | $(3, 1, 7)$              | `[[0o255, 0o331, 0o367]]`       |
+    | $(3, 1, 8)$              | `[[0o575, 0o623, 0o727]]`       |
 
-    .. math::
-        \\mu = \\max_{0 \\leq i < k} \\nu_i.
-
-    .. rubric:: Space-state representation
-
-    A convolutional code may also be described via the *space-state representation*. Let :math:`\\mathbf{u}_t = (u_t^{(0)}, u_t^{(1)}, \\ldots, u_t^{(k-1)})` be the input block, :math:`\\mathbf{v}_t = (v_t^{(0)}, v_t^{(1)}, \\ldots, v_t^{(n-1)})` be the output block, and :math:`\\mathbf{s}_t = (s_t^{(0)}, s_t^{(1)}, \\ldots, s_t^{(\\nu-1)})` be the state, all defined at time instant :math:`t`. Then,
-
-    .. math::
-       \\mathbf{s}_{t+1} & = \\mathbf{s}_t A + \\mathbf{u}_t B, \\\\
-       \\mathbf{v}_{t} & = \\mathbf{s}_t C + \\mathbf{u}_t D,
-
-    where :math:`A` is the :math:`\\nu \\times \\nu` *state matrix*, :math:`B` is the :math:`k \\times \\nu` *control matrix*, :math:`C` is the :math:`\\nu \\times n` *observation matrix*, and :math:`D` is the :math:`k \\times n` *transition matrix*.
-
-    .. rubric:: Table of convolutional code
-
-    The table below lists optimal convolutional codes with parameters :math:`(n,k) = (2,1)` and :math:`(n,k) = (3,1)`, for small values of the overall constraint length :math:`\\nu`. For more details, see :cite:`Lin.Costello.04` (Sec. 12.3).
-
-    =================================  ======================================
-     Parameters :math:`(n, k, \\nu)`    Transfer function matrix :math:`G(D)`
-    =================================  ======================================
-     :math:`(2, 1, 1)`                  :code:`[[0o1, 0o3]]`
-     :math:`(2, 1, 2)`                  :code:`[[0o5, 0o7]]`
-     :math:`(2, 1, 3)`                  :code:`[[0o13, 0o17]]`
-     :math:`(2, 1, 4)`                  :code:`[[0o27, 0o31]]`
-     :math:`(2, 1, 5)`                  :code:`[[0o53, 0o75]]`
-     :math:`(2, 1, 6)`                  :code:`[[0o117, 0o155]]`
-     :math:`(2, 1, 7)`                  :code:`[[0o247, 0o371]]`
-     :math:`(2, 1, 8)`                  :code:`[[0o561, 0o753]]`
-    =================================  ======================================
-
-    =================================  ======================================
-     Parameters :math:`(n, k, \\nu)`    Transfer function matrix :math:`G(D)`
-    =================================  ======================================
-     :math:`(3, 1, 1)`                  :code:`[[0o1, 0o3, 0o3]]`
-     :math:`(3, 1, 2)`                  :code:`[[0o5, 0o7, 0o7]]`
-     :math:`(3, 1, 3)`                  :code:`[[0o13, 0o15, 0o17]]`
-     :math:`(3, 1, 4)`                  :code:`[[0o25, 0o33, 0o37]]`
-     :math:`(3, 1, 5)`                  :code:`[[0o47, 0o53, 0o75]]`
-     :math:`(3, 1, 6)`                  :code:`[[0o117, 0o127, 0o155]]`
-     :math:`(3, 1, 7)`                  :code:`[[0o255, 0o331, 0o367]]`
-     :math:`(3, 1, 8)`                  :code:`[[0o575, 0o623, 0o727]]`
-    =================================  ======================================
-
-    References: :cite:`Johannesson.Zigangirov.15`, :cite:`Lin.Costello.04`, :cite:`Weiss.01`
+    For more details, see <cite>JZ15</cite> and <cite>LC04, Chs. 11, 12</cite>.
     """
 
     def __init__(self, feedforward_polynomials, feedback_polynomials=None):
-        """
-        Constructor for the class. It expects the following parameters:
-
-        :code:`feedforward_polynomials` : 2D-array of (:obj:`BinaryPolynomial` or :obj:`int`)
-            The matrix of feedforward polynomials :math:`P(D)`, which is a :math:`k \\times n` matrix whose entries are either binary polynomials (:obj:`BinaryPolynomial`) or integers to be converted to the former.
-
-        :code:`feedback_polynomials` : 1D-array of  (:obj:`BinaryPolynomial` or :obj:`int`), optional
-            The vector of feedback polynomials :math:`q(D)`, which is a :math:`k`-vector whose entries are either binary polynomials (:obj:`BinaryPolynomial`) or integers to be converted to the former. The default value corresponds to no feedback, that is, :math:`q_i(D) = 1` for all :math:`i \\in [0 : k)`.
-
-        .. rubric:: Examples
-
-        The convolutional code with encoder depicted in the figure below has parameters :math:`(n, k, \\nu) = (2, 1, 6)`; its transfer function matrix is given by
+        r"""
+        Constructor for the class.
 
-        .. math::
+        Parameters:
 
-           G(D) =
-           \\begin{bmatrix}
-              D^6 + D^3 + D^2 + D + 1  &  D^6 + D^5 + D^3 + D^2 + 1
-           \\end{bmatrix},
+            feedforward_polynomials (Array2D[BinaryPolynomial, int]): The matrix of feedforward polynomials $P(D)$, which is a $k \times n$ matrix whose entries are either [binary polynomials](/ref/BinaryPolynomial) or integers to be converted to the former.
 
-        yielding :code:`feedforward_polynomials = [[0b1001111, 0b1101101]] = [[0o117, 0o155]] = [[79, 109]]`.
+            feedback_polynomials (Optional[Array1D[BinaryPolynomial, int]]): The vector of feedback polynomials $q(D)$, which is a $k$-vector whose entries are either [binary polynomials](/ref/BinaryPolynomial) or integers to be converted to the former. The default value corresponds to no feedback, that is, $q_i(D) = 1$ for all $i \in [0 : k)$.
 
-        .. image:: figures/cc_2_1_6.png
-           :alt: Convolutional encoder example.
-           :align: center
-
-        >>> code = komm.ConvolutionalCode(feedforward_polynomials=[[0o117, 0o155]])
-        >>> (code.num_output_bits, code.num_input_bits, code.overall_constraint_length)
-        (2, 1, 6)
-
-        The convolutional code with encoder depicted in the figure below has parameters :math:`(n, k, \\nu) = (3, 2, 7)`; its transfer function matrix is given by
-
-        .. math::
-
-           G(D) =
-           \\begin{bmatrix}
-               D^4 + D^3 + 1  &  D^4 + D^2 + D + 1  &  0 \\\\
-               0  &  D^3 + D  &  D^3 + D^2 + 1 \\\\
-           \\end{bmatrix},
-
-        yielding :code:`feedforward_polynomials = [[0b11001, 0b10111, 0b00000], [0b0000, 0b1010, 0b1101]] = [[0o31, 0o27, 0o00], [0o00, 0o12, 0o15]] = [[25, 23, 0], [0, 10, 13]]`.
-
-        .. image:: figures/cc_3_2_7.png
-           :alt: Convolutional encoder example.
-           :align: center
-
-        >>> code = komm.ConvolutionalCode(feedforward_polynomials=[[0o31, 0o27, 0o00], [0o00, 0o12, 0o15]])
-        >>> (code.num_output_bits, code.num_input_bits, code.overall_constraint_length)
-        (3, 2, 7)
-
-        The convolutional code with feedback encoder depicted in the figure below has parameters :math:`(n, k, \\nu) = (2, 1, 4)`; its transfer function matrix is given by
-
-        .. math::
-
-           G(D) =
-           \\begin{bmatrix}
-               1  &  \\dfrac{D^4 + D^3 + 1}{D^4 + D^2 + D + 1}
-           \\end{bmatrix},
-
-        yielding :code:`feedforward_polynomials = [[0b10111, 0b11001]] = [[0o27, 0o31]] = [[23, 25]]` and :code:`feedback_polynomials = [0o27]`.
-
-        .. image:: figures/cc_2_1_4_fb.png
-           :alt: Convolutional feedback encoder example.
-           :align: center
-
-        >>> code = komm.ConvolutionalCode(feedforward_polynomials=[[0o27, 0o31]], feedback_polynomials=[0o27])
-        >>> (code.num_output_bits, code.num_input_bits, code.overall_constraint_length)
-        (2, 1, 4)
+        Examples:
+
+            The convolutional code with encoder depicted in the figure below has parameters $(n, k, \nu) = (2, 1, 6)$; its transfer function matrix is given by
+            $$
+                G(D) =
+                \begin{bmatrix}
+                    D^6 + D^3 + D^2 + D + 1  &  D^6 + D^5 + D^3 + D^2 + 1
+                \end{bmatrix},
+            $$
+            yielding `feedforward_polynomials = [[0b1001111, 0b1101101]] = [[0o117, 0o155]] = [[79, 109]]`.
+
+            <figure markdown>
+              ![Convolutional encoder for (2, 1, 6) code.](/figures/cc_2_1_6.svg)
+            </figure>
+
+            >>> code = komm.ConvolutionalCode(feedforward_polynomials=[[0o117, 0o155]])
+            >>> (code.num_output_bits, code.num_input_bits, code.overall_constraint_length)
+            (2, 1, 6)
+
+            The convolutional code with encoder depicted in the figure below has parameters $(n, k, \nu) = (3, 2, 7)$; its transfer function matrix is given by
+            $$
+                G(D) =
+                \begin{bmatrix}
+                    D^4 + D^3 + 1  &  D^4 + D^2 + D + 1  &  0 \\\\
+                    0  &  D^3 + D  &  D^3 + D^2 + 1
+                \end{bmatrix},
+            $$
+            yielding `feedforward_polynomials = [[0b11001, 0b10111, 0b00000], [0b0000, 0b1010, 0b1101]] = [[0o31, 0o27, 0o00], [0o00, 0o12, 0o15]] = [[25, 23, 0], [0, 10, 13]]`.
+
+            <figure markdown>
+              ![Convolutional encoder for (3, 2, 7) code.](/figures/cc_3_2_7.svg)
+            </figure>
+
+            >>> code = komm.ConvolutionalCode(feedforward_polynomials=[[0o31, 0o27, 0o00], [0o00, 0o12, 0o15]])
+            >>> (code.num_output_bits, code.num_input_bits, code.overall_constraint_length)
+            (3, 2, 7)
+
+            The convolutional code with feedback encoder depicted in the figure below has parameters $(n, k, \nu) = (2, 1, 4)$; its transfer function matrix is given by
+            $$
+                G(D) =
+                \begin{bmatrix}
+                    1  &  \dfrac{D^4 + D^3 + 1}{D^4 + D^2 + D + 1}
+                \end{bmatrix},
+            $$
+            yielding `feedforward_polynomials = [[0b10111, 0b11001]] = [[0o27, 0o31]] = [[23, 25]]` and `feedback_polynomials = [0o27]`.
+
+            <figure markdown>
+              ![Convolutional encoder for (2, 1, 4) feedback code.](/figures/cc_2_1_4_fb.svg)
+            </figure>
+
+            >>> code = komm.ConvolutionalCode(feedforward_polynomials=[[0o27, 0o31]], feedback_polynomials=[0o27])
+            >>> (code.num_output_bits, code.num_input_bits, code.overall_constraint_length)
+            (2, 1, 4)
         """
         self._feedforward_polynomials = np.empty_like(feedforward_polynomials, dtype=BinaryPolynomial)
         for (i, j), p in np.ndenumerate(feedforward_polynomials):
             self._feedforward_polynomials[i, j] = BinaryPolynomial(p)
 
         k, n = self._feedforward_polynomials.shape
 
         if feedback_polynomials is None:
             self._feedback_polynomials = np.array([BinaryPolynomial(0b1) for _ in range(k)], dtype=object)
-            self._constructed_from = 'no_feedback_polynomials'
+            self._constructed_from = "no_feedback_polynomials"
         else:
             self._feedback_polynomials = np.empty_like(feedback_polynomials, dtype=object)
             for i, q in np.ndenumerate(feedback_polynomials):
                 self._feedback_polynomials[i] = BinaryPolynomial(q)
-            self._constructed_from = 'feedback_polynomials'
+            self._constructed_from = "feedback_polynomials"
 
         nus = np.empty(k, dtype=int)
         for i, (ps, q) in enumerate(zip(self._feedforward_polynomials, self._feedback_polynomials)):
             nus[i] = max(np.amax([p.degree for p in ps]), q.degree)
 
         self._num_input_bits = k
         self._num_output_bits = n
@@ -187,19 +168,19 @@
             self._transfer_function_matrix[i, j] = BinaryPolynomialFraction(p) / BinaryPolynomialFraction(q)
 
         self._setup_finite_state_machine_direct_form()
         self._setup_space_state_representation()
 
     def __repr__(self):
         feedforward_polynomials_str = str(np.vectorize(str)(self._feedforward_polynomials).tolist()).replace("'", "")
-        args = 'feedforward_polynomials={}'.format(feedforward_polynomials_str)
-        if self._constructed_from == 'feedback_polynomials':
+        args = "feedforward_polynomials={}".format(feedforward_polynomials_str)
+        if self._constructed_from == "feedback_polynomials":
             feedback_polynomials_str = str(np.vectorize(str)(self._feedback_polynomials).tolist()).replace("'", "")
-            args = '{}, feedback_polynomials={}'.format(args, feedback_polynomials_str)
-        return '{}({})'.format(self.__class__.__name__, args)
+            args = "{}, feedback_polynomials={}".format(args, feedback_polynomials_str)
+        return "{}({})".format(self.__class__.__name__, args)
 
     def _setup_finite_state_machine_direct_form(self):
         n, k, nu = self._num_output_bits, self._num_input_bits, self._overall_constraint_length
 
         x_indices = np.concatenate(([0], np.cumsum(self._constraint_lengths + 1)[:-1]))
         s_indices = np.setdiff1d(np.arange(k + nu), x_indices)
 
@@ -252,187 +233,95 @@
             s1 = self._finite_state_machine.next_states[0, x]
             y = self._finite_state_machine.outputs[0, x]
             self._control_matrix[i, :] = int2binlist(s1, width=nu)
             self._transition_matrix[i, :] = int2binlist(y, width=n)
 
     @property
     def num_input_bits(self):
-        """
-        The number of input bits per block, :math:`k`. This property is read-only.
+        r"""
+        The number of input bits per block, $k$.
         """
         return self._num_input_bits
 
     @property
     def num_output_bits(self):
-        """
-        The number of output bits per block, :math:`n`. This property is read-only.
+        r"""
+        The number of output bits per block, $n$.
         """
         return self._num_output_bits
 
     @property
     def constraint_lengths(self):
-        """
-        The constraint lengths :math:`\\nu_i` of the code, for :math:`i \\in [0 : k)`. This is a 1D-array of :obj:`int`. This property is read-only.
+        r"""
+        The constraint lengths $\nu_i$ of the code, for $i \in [0 : k)$. This is a $k$-array of integers.
         """
         return self._constraint_lengths
 
     @property
     def overall_constraint_length(self):
-        """
-        The overall constraint length :math:`\\nu` of the code. This property is read-only.
+        r"""
+        The overall constraint length $\nu$ of the code.
         """
         return self._overall_constraint_length
 
     @property
     def memory_order(self):
+        r"""
+        The memory order $\mu$ of the code.
         """
-        The memory order :math:`\\mu` of the code. This property is read-only.
-        """
-        return  self._memory_order
+        return self._memory_order
 
     @property
     def feedforward_polynomials(self):
-        """
-        The matrix of feedforward polynomials :math:`P(D)` of the code. This is a :math:`k \\times n` array of :obj:`BinaryPolynomial`. This property is read-only.
+        r"""
+        The matrix of feedforward polynomials $P(D)$ of the code. This is a $k \times n$ array of [binary polynomials](/ref/BinaryPolynomial).
         """
         return self._feedforward_polynomials
 
     @property
     def feedback_polynomials(self):
-        """
-        The vector of feedback polynomials :math:`q(D)` of the code. This is a :math:`k`-array of :obj:`BinaryPolynomial`. This property is read-only.
+        r"""
+        The vector of feedback polynomials $q(D)$ of the code. This is a $k$-array of [binary polynomials](/ref/BinaryPolynomial).
         """
         return self._feedback_polynomials
 
     @property
     def transfer_function_matrix(self):
-        """
-        The transfer function matrix :math:`G(D)` of the code. This is a :math:`k \\times n` array of :obj:`BinaryPolynomialFraction`. This property is read-only.
+        r"""
+        The transfer function matrix $G(D)$ of the code. This is a $k \times n$ array of [binary polynomial fractions](/ref/BinaryPolynomialFraction).
         """
         return self._transfer_function_matrix
 
     @property
     def finite_state_machine(self):
-        """
+        r"""
         The finite-state machine of the code.
         """
         return self._finite_state_machine
 
     @property
     def state_matrix(self):
-        """
-        The state matrix :math:`A` of the state-space representation. This is a :math:`\\nu \\times \\nu` array of integers in :math:`\\{ 0, 1 \\}`. This property is read-only.
+        r"""
+        The state matrix $A$ of the state-space representation. This is a $\nu \times \nu$ array of integers in $\\{ 0, 1 \\}$.
         """
         return self._state_matrix
 
     @property
     def control_matrix(self):
-        """
-        The control matrix :math:`B` of the state-space representation. This is a :math:`k \\times \\nu` array of integers in :math:`\\{ 0, 1 \\}`. This property is read-only.
+        r"""
+        The control matrix $B$ of the state-space representation. This is a $k \times \nu$ array of integers in $\\{ 0, 1 \\}$.
         """
         return self._control_matrix
 
     @property
     def observation_matrix(self):
-        """
-        The observation matrix :math:`C` of the state-space representation. This is a :math:`\\nu \\times n` array of integers in :math:`\\{ 0, 1 \\}`. This property is read-only.
+        r"""
+        The observation matrix $C$ of the state-space representation. This is a $\nu \times n$ array of integers in $\\{ 0, 1 \\}$.
         """
         return self._observation_matrix
 
     @property
     def transition_matrix(self):
-        """
-        The transition matrix :math:`D` of the state-space representation. This is a :math:`k \\times n` array of integers in :math:`\\{ 0, 1 \\}`. This property is read-only.
+        r"""
+        The transition matrix $D$ of the state-space representation. This is a $k \times n$ array of integers in $\\{ 0, 1 \\}$.
         """
         return self._transition_matrix
-
-
-class ConvolutionalStreamEncoder:
-    """
-    Convolutional stream encoder. Encode a bit stream using a given convolutional code (:class:`ConvolutionalCode`). The internal state of the encoder is maintained across each call.
-
-    .. rubric:: Examples
-
-    >>> convolutional_code = komm.ConvolutionalCode([[0o7, 0o5]])
-    >>> convolutional_encoder = komm.ConvolutionalStreamEncoder(convolutional_code)
-    >>> convolutional_encoder([1, 1, 1, 1])
-    array([1, 1, 0, 1, 1, 0, 1, 0])
-    >>> convolutional_encoder([1, 1, 1, 1])
-    array([1, 0, 1, 0, 1, 0, 1, 0])
-    """
-    def __init__(self, convolutional_code, initial_state=0):
-        """
-        Constructor for the class. It expects the following parameters:
-
-        :code:`convolutional_code` : :class:`ConvolutionalCode`
-            The convolutional code.
-
-        :code:`initial_state` : :obj:`int`, optional
-            Initial state of the encoder. The default value is :code:`0`.
-        """
-        self._convolutional_code = convolutional_code
-        self._state = int(initial_state)
-
-    def __call__(self, inp):
-        n, k = self._convolutional_code.num_output_bits, self._convolutional_code.num_input_bits
-
-        output_sequence, self._state = self._convolutional_code.finite_state_machine.process(
-            input_sequence=pack(inp, width=k),
-            initial_state=self._state)
-
-        outp = unpack(output_sequence, width=n)
-        return outp
-
-
-class ConvolutionalStreamDecoder:
-    """
-    Convolutional stream decoder using Viterbi algorithm. Decode a (hard or soft) bit stream given a convolutional code (:class:`ConvolutionalCode`), assuming a traceback length (path memory) of :math:`\\tau`. At time :math:`t`, the decoder chooses the path survivor with best metric at time :math:`t - \\tau` and outputs the corresponding information bits. The output stream has a delay equal to :math:`k \\tau`, where :math:`k` is the number of input bits of the convolutional code. As a rule of thumb, the traceback length is choosen as :math:`\\tau = 5\\mu`, where :math:`\\mu` is the memory order of the convolutional code.
-
-    .. rubric:: Examples
-
-    >>> convolutional_code = komm.ConvolutionalCode([[0o7, 0o5]])
-    >>> convolutional_decoder = komm.ConvolutionalStreamDecoder(convolutional_code, traceback_length=10)
-    >>> convolutional_decoder([1, 1, 1, 0, 0, 0, 0, 1, 1, 0, 0, 1, 0, 0, 0, 1, 0, 1, 1, 1])
-    array([0, 0, 0, 0, 0, 0, 0, 0, 0, 0])
-    >>> convolutional_decoder(np.zeros(2*10, dtype=int))
-    array([1, 0, 1, 1, 1, 0, 1, 1, 0, 0])
-    """
-    def __init__(self, convolutional_code, traceback_length, initial_state=0, input_type='hard'):
-        """
-        Constructor for the class. It expects the following parameters:
-
-        :code:`convolutional_code` : :class:`ConvolutionalCode`
-            The convolutional code.
-
-        :code:`traceback_length` : :obj:`int`
-            The traceback length (path memory) :math:`\\tau` of the decoder.
-
-        :code:`initial_state` : :obj:`int`, optional
-            Initial state of the encoder. The default value is :code:`0`.
-        """
-        self._convolutional_code = convolutional_code
-        self._traceback_length = int(traceback_length)
-        self._initial_state = int(initial_state)
-        self._input_type = input_type
-
-        n = convolutional_code.num_output_bits
-        num_states = convolutional_code.finite_state_machine.num_states
-
-        self._memory = {}
-        self._memory['metrics'] = np.full((num_states, traceback_length + 1), fill_value=np.inf)
-        self._memory['metrics'][initial_state, -1] = 0.0
-        self._memory['paths'] = np.zeros((num_states, traceback_length + 1), dtype=int)
-
-        cache_bit = np.array([int2binlist(y, width=n) for y in range(2**n)])
-        self._metric_function_hard = lambda y, z: np.count_nonzero(cache_bit[y] != z)
-        self._metric_function_soft = lambda y, z: np.dot(cache_bit[y], z)
-
-    def __call__(self, inp):
-        n, k = self._convolutional_code.num_output_bits, self._convolutional_code.num_input_bits
-
-        input_sequence_hat = self._convolutional_code.finite_state_machine.viterbi_streaming(
-            observed_sequence=np.reshape(inp, newshape=(-1, n)),
-            metric_function=getattr(self, '_metric_function_' + self._input_type),
-            memory=self._memory)
-
-        outp = unpack(input_sequence_hat, width=k)
-        return outp
```

### Comparing `komm-0.7.4/komm/_finite_state_machine.py` & `komm-0.8.2/src/komm/_finite_state_machine/FiniteStateMachine.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,213 +1,195 @@
 import numpy as np
-
 from scipy import special
 
 
-__all__ = ['FiniteStateMachine']
-
-
 class FiniteStateMachine:
-    """
-    Finite-state machine (Mealy machine). It is defined by a *set of states* :math:`\\mathcal{S}`, an *input alphabet* :math:`\\mathcal{X}`, an *output alphabet* :math:`\\mathcal{Y}`, and a *transition function* :math:`T : \\mathcal{S} \\times \\mathcal{X} \\to \\mathcal{S} \\times \\mathcal{Y}`. Here, for simplicity, the set of states, the input alphabet, and the output alphabet are always taken as :math:`\\mathcal{S} = \\{ 0, 1, \\ldots, |\\mathcal{S}| - 1 \\}`, :math:`\\mathcal{X} = \\{ 0, 1, \\ldots, |\\mathcal{X}| - 1 \\}`, and :math:`\\mathcal{Y} = \\{ 0, 1, \\ldots, |\\mathcal{Y}| - 1 \\}`, respectively.
+    r"""
+    Finite-state machine (Mealy machine). It is defined by a *set of states* $\mathcal{S}$, an *input alphabet* $\mathcal{X}$, an *output alphabet* $\mathcal{Y}$, and a *transition function* $T : \mathcal{S} \times \mathcal{X} \to \mathcal{S} \times \mathcal{Y}$. Here, for simplicity, the set of states, the input alphabet, and the output alphabet are always taken as $\mathcal{S} = \\{ 0, 1, \ldots, |\mathcal{S}| - 1 \\}$, $\mathcal{X} = \\{ 0, 1, \ldots, |\mathcal{X}| - 1 \\}$, and $\mathcal{Y} = \\{ 0, 1, \ldots, |\mathcal{Y}| - 1 \\}$, respectively.
 
     For example, consider the finite-state machine whose state diagram depicted in the figure below.
 
-    .. image:: figures/mealy.png
-       :alt: Finite-state machine (Mealy machine) example.
-       :align: center
-
-    It has set of states :math:`\\mathcal{S} = \\{ 0, 1, 2, 3 \\}`, input alphabet :math:`\\mathcal{X} = \\{ 0, 1 \\}`, output alphabet :math:`\\mathcal{Y} = \\{ 0, 1, 2, 3 \\}`, and transition function :math:`T` given by the table below.
-
-    .. csv-table:: Transition function
-       :align: center
-       :header: State, Input, Next state, Output
-
-       0, 0, 0, 0
-       0, 1, 1, 3
-       1, 0, 2, 1
-       1, 1, 3, 2
-       2, 0, 0, 3
-       2, 1, 1, 0
-       3, 0, 2, 2
-       3, 1, 3, 1
-
-    |
+    <figure markdown>
+      ![Finite-state machine (Mealy machine) example.](/figures/mealy.svg)
+    </figure>
+
+    It has set of states $\mathcal{S} = \\{ 0, 1, 2, 3 \\}$, input alphabet $\mathcal{X} = \\{ 0, 1 \\}$, output alphabet $\mathcal{Y} = \\{ 0, 1, 2, 3 \\}$, and transition function $T$ given by the table below.
+
+    | State | Input | Next state | Output |
+    | :---: | :---: | :--------: | :----: |
+    | $0$   | $0$   | $0$        | $0$    |
+    | $0$   | $1$   | $1$        | $3$    |
+    | $1$   | $0$   | $2$        | $1$    |
+    | $1$   | $1$   | $3$        | $2$    |
+    | $2$   | $0$   | $0$        | $3$    |
+    | $2$   | $1$   | $1$        | $0$    |
+    | $3$   | $0$   | $2$        | $2$    |
+    | $3$   | $1$   | $3$        | $1$    |
     """
+
     def __init__(self, next_states, outputs):
-        """
-        Constructor for the class. It expects the following parameters:
+        r"""
+        Constructor for the class.
+
+        Parameters:
 
-        :code:`next_states` : 2D-array of :obj:`int`
-            The matrix of next states of the machine, of shape :math:`|\\mathcal{S}| \\times |\\mathcal{X}|`. The element in row :math:`s` and column :math:`x` should be the next state of the machine (an element in :math:`\\mathcal{S}`), given that the current state is :math:`s \\in \\mathcal{S}` and the input is :math:`x \\in \\mathcal{X}`.
+            next_states (Array2D[int]): The matrix of next states of the machine, of shape $|\mathcal{S}| \times |\mathcal{X}|$. The element in row $s$ and column $x$ should be the next state of the machine (an element in $\mathcal{S}$), given that the current state is $s \in \mathcal{S}$ and the input is $x \in \mathcal{X}$.
 
-        :code:`outputs` : 2D-array of :obj:`int`
-            The matrix of outputs of the machine, of shape :math:`|\\mathcal{S}| \\times |\\mathcal{X}|`. The element in row :math:`s` and column :math:`x` should be the output of the machine (an element in :math:`\\mathcal{Y}`), given that the current state is :math:`s \\in \\mathcal{S}` and the input is :math:`x \\in \\mathcal{X}`.
+            outputs (Array2D[int]): The matrix of outputs of the machine, of shape $|\mathcal{S}| \times |\mathcal{X}|$. The element in row $s$ and column $x$ should be the output of the machine (an element in $\mathcal{Y}$), given that the current state is $s \in \mathcal{S}$ and the input is $x \in \mathcal{X}$.
 
-        .. rubric:: Examples
+        Examples:
 
-        >>> fsm = komm.FiniteStateMachine(next_states=[[0,1], [2,3], [0,1], [2,3]], outputs=[[0,3], [1,2], [3,0], [2,1]])
+            >>> fsm = komm.FiniteStateMachine(next_states=[[0,1], [2,3], [0,1], [2,3]], outputs=[[0,3], [1,2], [3,0], [2,1]])
         """
         self._next_states = np.array(next_states, dtype=int)
         self._outputs = np.array(outputs, dtype=int)
         self._num_states, self._num_input_symbols = self._next_states.shape
         self._num_output_symbols = np.amax(self._outputs)
 
         self._input_edges = np.full((self._num_states, self._num_states), fill_value=-1)
         self._output_edges = np.full((self._num_states, self._num_states), fill_value=-1)
         for state_from in range(self._num_states):
             for x, state_to in enumerate(self._next_states[state_from, :]):
                 self._input_edges[state_from, state_to] = x
                 self._output_edges[state_from, state_to] = self._outputs[state_from, x]
 
     def __repr__(self):
-        args = 'next_states={}, outputs={}'.format(self._next_states.tolist(), self._outputs.tolist())
-        return '{}({})'.format(self.__class__.__name__, args)
+        args = "next_states={}, outputs={}".format(self._next_states.tolist(), self._outputs.tolist())
+        return "{}({})".format(self.__class__.__name__, args)
 
     @property
     def num_states(self):
-        """
-        The number of states of the machine. This property is read-only.
+        r"""
+        The number of states of the machine.
         """
         return self._num_states
 
     @property
     def num_input_symbols(self):
-        """
-        The size (cardinality) of the input alphabet :math:`\\mathcal{X}`. This property is read-only.
+        r"""
+        The size (cardinality) of the input alphabet $\mathcal{X}$.
         """
         return self._num_input_symbols
 
     @property
     def num_output_symbols(self):
-        """
-        The size (cardinality) of the output alphabet :math:`\\mathcal{Y}`. This property is read-only.
+        r"""
+        The size (cardinality) of the output alphabet $\mathcal{Y}$.
         """
         return self._num_output_symbols
 
     @property
     def next_states(self):
-        """
-        The matrix of next states of the machine. It has shape :math:`|\\mathcal{S}| \\times |\\mathcal{X}|`. The element in row :math:`s` and column :math:`x` is the next state of the machine (an element in :math:`\\mathcal{S}`), given that the current state is :math:`s \\in \\mathcal{S}` and the input is :math:`x \\in \\mathcal{X}`. This property is read-only.
+        r"""
+        The matrix of next states of the machine. It has shape $|\mathcal{S}| \times |\mathcal{X}|$. The element in row $s$ and column $x$ is the next state of the machine (an element in $\mathcal{S}$), given that the current state is $s \in \mathcal{S}$ and the input is $x \in \mathcal{X}$.
         """
         return self._next_states
 
     @property
     def outputs(self):
-        """
-        The matrix of outputs of the machine. It has shape :math:`|\\mathcal{S}| \\times |\\mathcal{X}|`. The element in row :math:`s` and column :math:`x` is the output of the machine (an element in :math:`\\mathcal{Y}`), given that the current state is :math:`s \\in \\mathcal{S}` and the input is :math:`x \\in \\mathcal{X}`. This property is read-only.
+        r"""
+        The matrix of outputs of the machine. It has shape $|\mathcal{S}| \times |\mathcal{X}|$. The element in row $s$ and column $x$ is the output of the machine (an element in $\mathcal{Y}$), given that the current state is $s \in \mathcal{S}$ and the input is $x \in \mathcal{X}$.
         """
         return self._outputs
 
     @property
     def input_edges(self):
-        """
-        The matrix of input edges of the machine. It has shape :math:`|\\mathcal{S}| \\times |\\mathcal{S}|`. If there is an edge from :math:`s_0 \\in \\mathcal{S}` to :math:`s_1 \\in \\mathcal{S}`, then the element in row :math:`s_0` and column :math:`s_1` is the input associated with that edge (an element of :math:`\\mathcal{X}`); if there is no such edge, then the element is :math:`-1`. This property is read-only.
+        r"""
+        The matrix of input edges of the machine. It has shape $|\mathcal{S}| \times |\mathcal{S}|$. If there is an edge from $s_0 \in \mathcal{S}$ to $s_1 \in \mathcal{S}$, then the element in row $s_0$ and column $s_1$ is the input associated with that edge (an element of $\mathcal{X}$); if there is no such edge, then the element is $-1$.
 
-        .. rubric:: Examples
+        Examples:
 
-        >>> fsm = komm.FiniteStateMachine(next_states=[[0,1], [2,3], [0,1], [2,3]], outputs=[[0,3], [1,2], [3,0], [2,1]])
-        >>> fsm.input_edges
-        array([[ 0,  1, -1, -1],
-               [-1, -1,  0,  1],
-               [ 0,  1, -1, -1],
-               [-1, -1,  0,  1]])
+            >>> fsm = komm.FiniteStateMachine(next_states=[[0,1], [2,3], [0,1], [2,3]], outputs=[[0,3], [1,2], [3,0], [2,1]])
+            >>> fsm.input_edges
+            array([[ 0,  1, -1, -1],
+                   [-1, -1,  0,  1],
+                   [ 0,  1, -1, -1],
+                   [-1, -1,  0,  1]])
         """
         return self._input_edges
 
     @property
     def output_edges(self):
-        """
-        The matrix of output edges of the machine. It has shape :math:`|\\mathcal{S}| \\times |\\mathcal{S}|`. If there is an edge from :math:`s_0 \\in \\mathcal{S}` to :math:`s_1 \\in \\mathcal{S}`, then the element in row :math:`s_0` and column :math:`s_1` is the output associated with that edge (an element of :math:`\\mathcal{Y}`); if there is no such edge, then the element is :math:`-1`. This property is read-only.
+        r"""
+        The matrix of output edges of the machine. It has shape $|\mathcal{S}| \times |\mathcal{S}|$. If there is an edge from $s_0 \in \mathcal{S}$ to $s_1 \in \mathcal{S}$, then the element in row $s_0$ and column $s_1$ is the output associated with that edge (an element of $\mathcal{Y}$); if there is no such edge, then the element is $-1$.
 
-        .. rubric:: Examples
+        Examples:
 
-        >>> fsm = komm.FiniteStateMachine(next_states=[[0,1], [2,3], [0,1], [2,3]], outputs=[[0,3], [1,2], [3,0], [2,1]])
-        >>> fsm.output_edges
-        array([[ 0,  3, -1, -1],
-               [-1, -1,  1,  2],
-               [ 3,  0, -1, -1],
-               [-1, -1,  2,  1]])
+            >>> fsm = komm.FiniteStateMachine(next_states=[[0,1], [2,3], [0,1], [2,3]], outputs=[[0,3], [1,2], [3,0], [2,1]])
+            >>> fsm.output_edges
+            array([[ 0,  3, -1, -1],
+                   [-1, -1,  1,  2],
+                   [ 3,  0, -1, -1],
+                   [-1, -1,  2,  1]])
         """
         return self._output_edges
 
     def process(self, input_sequence, initial_state):
-        """
-        Returns the output sequence corresponding to a given input sequence. It assumes the machine starts at a given initial state :math:`s_\\mathrm{i}`. The input sequence and the output sequence are denoted by :math:`\\mathbf{x} = (x_0, x_1, \\ldots, x_{L-1}) \\in \\mathcal{X}^L` and :math:`\\mathbf{y} = (y_0, y_1, \\ldots, y_{L-1}) \\in \\mathcal{Y}^L`, respectively.
+        r"""
+        Returns the output sequence corresponding to a given input sequence. It assumes the machine starts at a given initial state $s_\mathrm{i}$. The input sequence and the output sequence are denoted by $\mathbf{x} = (x_0, x_1, \ldots, x_{L-1}) \in \mathcal{X}^L$ and $\mathbf{y} = (y_0, y_1, \ldots, y_{L-1}) \in \mathcal{Y}^L$, respectively.
 
-        .. rubric:: Input
+        Parameters:
 
-        :code:`input_sequence` : 1D-array of :obj:`int`
-            The input sequence :math:`\\mathbf{x} \\in \\mathcal{X}^L`. It should be a 1D-array with elements in :math:`\\mathcal{X}`.
+            input_sequence (Array1D[int]): The input sequence $\mathbf{x} \in \mathcal{X}^L$. It should be a 1D-array with elements in $\mathcal{X}$.
 
-        :code:`initial_state` : :obj:`int`
-            The initial state :math:`s_\\mathrm{i}` of the machine. Should be an integer in :math:`\\mathcal{S}`.
+            initial_state (int): The initial state $s_\mathrm{i}$ of the machine. Should be an integer in $\mathcal{S}$.
 
-        .. rubric:: Output
+        Returns:
 
-        :code:`output_sequence` : 1D-array of :obj:`int`
-            The output sequence :math:`\\mathbf{y} \\in \\mathcal{Y}^L` corresponding to :code:`input_sequence`, assuming the machine starts at the state given by :code:`initial_state`. It is a 1D-array with elements in :math:`\\mathcal{Y}`.
+            output_sequence (Array1D[int]): The output sequence $\mathbf{y} \in \mathcal{Y}^L$ corresponding to `input_sequence`, assuming the machine starts at the state given by `initial_state`. It is a 1D-array with elements in $\mathcal{Y}$.
 
-        :code:`final_state` : :obj:`int`
-            The final state :math:`s_\\mathrm{f}` of the machine. It is an integer in :math:`\\mathcal{S}`.
+            final_state (int): The final state $s_\mathrm{f}$ of the machine. It is an integer in $\mathcal{S}$.
 
-        .. rubric:: Examples
+        Examples:
 
-        >>> fsm = komm.FiniteStateMachine(next_states=[[0,1], [2,3], [0,1], [2,3]], outputs=[[0,3], [1,2], [3,0], [2,1]])
-        >>> input_sequence, initial_state = [1, 1, 0, 1, 0], 0
-        >>> output_sequence, final_state = fsm.process(input_sequence, initial_state)
-        >>> output_sequence
-        array([3, 2, 2, 0, 1])
-        >>> final_state
-        2
+            >>> fsm = komm.FiniteStateMachine(next_states=[[0,1], [2,3], [0,1], [2,3]], outputs=[[0,3], [1,2], [3,0], [2,1]])
+            >>> input_sequence, initial_state = [1, 1, 0, 1, 0], 0
+            >>> output_sequence, final_state = fsm.process(input_sequence, initial_state)
+            >>> output_sequence
+            array([3, 2, 2, 0, 1])
+            >>> final_state
+            2
         """
         output_sequence = np.empty_like(input_sequence, dtype=int)
         s = initial_state
         for t, x in np.ndenumerate(input_sequence):
             y = self._outputs[s, x]
             s = self._next_states[s, x]
             output_sequence[t] = y
         final_state = s
         return output_sequence, final_state
 
     def viterbi(self, observed_sequence, metric_function, initial_metrics=None):
-        """
-        Applies the Viterbi algorithm on a given observed sequence. The Viterbi algorithm finds the most probable input sequence :math:`\\hat{\\mathbf{x}}(s) \\in \\mathcal{X}^L` ending in state :math:`s`, for all :math:`s \\in \\mathcal{S}`, given an observed sequence :math:`\\mathbf{z} \\in \\mathcal{Z}^L`. It is assumed uniform input priors.
-
-        References: :cite:`Lin.Costello.04` (Sec. 12.1).
+        r"""
+        Applies the Viterbi algorithm on a given observed sequence. The Viterbi algorithm finds the most probable input sequence $\hat{\mathbf{x}}(s) \in \mathcal{X}^L$ ending in state $s$, for all $s \in \mathcal{S}$, given an observed sequence $\mathbf{z} \in \mathcal{Z}^L$. It is assumed uniform input priors. See <cite>LC04, Sec. 12.1</cite>.
 
-        .. rubric:: Input
+        Parameters:
 
-        :code:`observed_sequence` : 1D-array
-            The observed sequence :math:`\\mathbf{z} \\in \\mathcal{Z}^L`.
+            observed_sequence (Array1D): The observed sequence $\mathbf{z} \in \mathcal{Z}^L$.
 
-        :code:`metric_function` : function
-            The metric function :math:`\\mathcal{Y} \\times \\mathcal{Z} \\to \\mathbb{R}`.
+            metric_function (function): The metric function $\mathcal{Y} \times \mathcal{Z} \to \mathbb{R}$.
 
-        :code:`initial_metrics` : 1D-array of :obj:`float`, optional
-            The initial metrics for each state. It must be a 1D-array of length :math:`|\\mathcal{S}|`. The default value is :code:`0.0` for all states.
+            initial_metrics (Optional[Array1D[float]]): The initial metrics for each state. It must be a 1D-array of length $|\mathcal{S}|$. The default value is `0.0` for all states.
 
-        .. rubric:: Output
+        Returns:
 
-        :code:`input_sequences_hat` : 2D-array of :obj:`int`
-            The most probable input sequence :math:`\\hat{\\mathbf{x}}(s) \\in \\mathcal{X}^L` ending in state :math:`s`, for all :math:`s \\in \\mathcal{S}`. It is a 2D-array of shape :math:`L \\times |\\mathcal{S}|`, in which column :math:`s` is equal to :math:`\\hat{\\mathbf{x}}(s)`.
+            input_sequences_hat (Array2D[int]): The most probable input sequence $\hat{\mathbf{x}}(s) \in \mathcal{X}^L$ ending in state $s$, for all $s \in \mathcal{S}$. It is a 2D-array of shape $L \times |\mathcal{S}|$, in which column $s$ is equal to $\hat{\mathbf{x}}(s)$.
 
-        :code:`final_metrics` : 1D-array of :obj:`float`
-            The final metrics for each state. It is a 1D-array of length :math:`|\\mathcal{S}|`.
+            final_metrics (Array1D[float]): The final metrics for each state. It is a 1D-array of length $|\mathcal{S}|$.
         """
         L, num_states = len(observed_sequence), self._num_states
         choices = np.empty((L, num_states), dtype=int)
         metrics = np.full((L + 1, num_states), fill_value=np.inf)
         if initial_metrics is None:
             metrics[0, :] = np.zeros(num_states, dtype=float)
         else:
             metrics[0, :] = initial_metrics
         for t, z in enumerate(observed_sequence):
             for s0 in range(num_states):
-                for (s1, y) in zip(self._next_states[s0], self._outputs[s0]):
+                for s1, y in zip(self._next_states[s0], self._outputs[s0]):
                     candidate_metrics = metrics[t, s0] + metric_function(y, z)
                     if candidate_metrics < metrics[t + 1, s1]:
                         metrics[t + 1, s1] = candidate_metrics
                         choices[t, s1] = s0
 
         # Backtrack
         input_sequences_hat = np.empty((L, num_states), dtype=int)
@@ -217,106 +199,97 @@
                 s0 = choices[t, s1]
                 input_sequences_hat[t, final_state] = self._input_edges[s0, s1]
                 s1 = s0
 
         return input_sequences_hat, metrics[L, :]
 
     def viterbi_streaming(self, observed_sequence, metric_function, memory):
-        """
-        Applies the streaming version of the Viterbi algorithm on a given observed sequence. The path memory (or traceback length) is denoted by :math:`\\tau`. It chooses the survivor with best metric and selects the information block on this path.
-
-        References: :cite:`Lin.Costello.04` (Sec. 12.3).
-
-        .. rubric:: Input
+        r"""
+        Applies the streaming version of the Viterbi algorithm on a given observed sequence. The path memory (or traceback length) is denoted by $\tau$. It chooses the survivor with best metric and selects the information block on this path. See <cite>LC04, Sec. 12.3</cite>.
 
-        :code:`observed_sequence` : 1D-array
-            The observed sequence :math:`\\mathbf{z} \\in \\mathcal{Z}^L`.
+        Parameters:
 
-        :code:`metric_function` : function
-            The metric function :math:`\\mathcal{Y} \\times \\mathcal{Z} \\to \\mathbb{R}`.
+            observed_sequence (Array1D): The observed sequence $\mathbf{z} \in \mathcal{Z}^L$.
 
-        .. rubric:: Output
+            metric_function (function): The metric function $\mathcal{Y} \times \mathcal{Z} \to \mathbb{R}$.
 
-        :code:`input_sequence_hat` : 1D-array of :obj:`int`
-            The most probable input sequence :math:`\\hat{\\mathbf{x}} \\in \\mathcal{X}^L`
+            memory (dict): The metrics for each state. It must be a dictionary containing two keys: `'paths'`, a 2D-array of integers of shape $|\mathcal{S}| \times (\tau + 1)$; and `'metrics'`, a 2D-array of floats of shape $|\mathcal{S}| \times (\tau + 1)$. This dictionary is updated in-place by this method.
 
-        .. rubric:: Input and Output
+        Returns:
 
-        :code:`memory` : :obj:`dict`
-            The metrics for each state. It must be a dictionary containing two keys: :code:`'paths'`, a 2D-array of :obj:`int` of shape :math:`|\\mathcal{S}| \\times (\\tau + 1)`; and :code:`'metrics'`, a 2D-array of :obj:`float` of shape :math:`|\\mathcal{S}| \\times (\\tau + 1)`.
+            input_sequence_hat (Array1D[int]): The most probable input sequence $\hat{\mathbf{x}} \in \mathcal{X}^L$
         """
         num_states = self._num_states
         input_sequences_hat = np.empty(len(observed_sequence), dtype=int)
         for t, z in enumerate(observed_sequence):
             new_metrics = np.full(num_states, fill_value=np.inf)
             choices = np.zeros(num_states, dtype=int)
             for s0 in range(num_states):
-                for (s1, y) in zip(self._next_states[s0], self._outputs[s0]):
-                    candidate_metric = memory['metrics'][s0, -1] + metric_function(y, z)
+                for s1, y in zip(self._next_states[s0], self._outputs[s0]):
+                    candidate_metric = memory["metrics"][s0, -1] + metric_function(y, z)
                     if candidate_metric < new_metrics[s1]:
                         new_metrics[s1] = candidate_metric
                         choices[s1] = s0
 
             s_star = np.argmin(new_metrics)
-            s0, s1 = memory['paths'][s_star, :2]
+            s0, s1 = memory["paths"][s_star, :2]
             input_sequences_hat[t] = self._input_edges[s0, s1]
 
-            memory['metrics'] = np.roll(memory['metrics'], shift=-1, axis=1)
-            memory['metrics'][:, -1] = new_metrics
-            memory['paths'] = np.roll(memory['paths'], shift=-1, axis=1)
+            memory["metrics"] = np.roll(memory["metrics"], shift=-1, axis=1)
+            memory["metrics"][:, -1] = new_metrics
+            memory["paths"] = np.roll(memory["paths"], shift=-1, axis=1)
 
-            paths_copy = np.copy(memory['paths'])
+            paths_copy = np.copy(memory["paths"])
             for s1, s0 in enumerate(choices):
-                memory['paths'][s1, :-1] = paths_copy[s0, :-1]
-                memory['paths'][s1, -1] = s1
+                memory["paths"][s1, :-1] = paths_copy[s0, :-1]
+                memory["paths"][s1, -1] = s1
 
         return input_sequences_hat
 
-    def forward_backward(self, observed_sequence, metric_function, input_priors=None, initial_state_distribution=None, final_state_distribution=None):
-        """
-        Applies the forward-backward algorithm on a given observed sequence. The forward-backward algorithm computes the posterior :term:`pmf` of each input :math:`x_0, x_1, \\ldots, x_{L-1} \\in \\mathcal{X}` given an observed sequence :math:`\\mathbf{z} = (z_0, z_1, \\ldots, z_{L-1}) \\in \\mathcal{Z}^L`. The prior :term:`pmf` of each input may also be provided.
-
-        References: :cite:`Lin.Costello.04` (Sec. 12.6).
+    def forward_backward(
+        self,
+        observed_sequence,
+        metric_function,
+        input_priors=None,
+        initial_state_distribution=None,
+        final_state_distribution=None,
+    ):
+        r"""
+        Applies the forward-backward algorithm on a given observed sequence. The forward-backward algorithm computes the posterior pmf of each input $x_0, x_1, \ldots, x_{L-1} \in \mathcal{X}$ given an observed sequence $\mathbf{z} = (z_0, z_1, \ldots, z_{L-1}) \in \mathcal{Z}^L$. The prior pmf of each input may also be provided. See <cite>LC04, 12.6</cite>.
 
-        .. rubric:: Input
+        Parameters:
 
-        :code:`observed_sequence` : 1D-array
-            The observed sequence :math:`\\mathbf{z} \\in \\mathcal{Z}^L`.
+            observed_sequence (Array1D): The observed sequence $\mathbf{z} \in \mathcal{Z}^L$.
 
-        :code:`metric_function` : function
-            The metric function :math:`\\mathcal{Y} \\times \\mathcal{Z} \\to \\mathbb{R}`.
+            metric_function (function): The metric function $\mathcal{Y} \times \mathcal{Z} \to \mathbb{R}$.
 
-        :code:`input_priors` : 2D-array of :obj:`float`, optional
-            The prior :term:`pmf` of each input, of shape :math:`L \\times |\\mathcal{X}|`. The element in row :math:`t \\in [0 : L)` and column :math:`x \\in \\mathcal{X}` should be :math:`p(x_t = x)`. The default value considers uniform priors.
+            input_priors (Optional[Array2D[float]]): The prior pmf of each input, of shape $L \times |\mathcal{X}|$. The element in row $t \in [0 : L)$ and column $x \in \mathcal{X}$ should be $p(x_t = x)$. The default value yields uniform priors.
 
-        :code:`initial_state_distribution` : 1D-array of :obj:`float`, optional
-            The :term:`pmf` of the initial state of the machine. It must be a 1D-array of length :math:`|\\mathcal{S}|`. The default value is uniform over all states.
+            initial_state_distribution (Optional[Array1D[float]]): The pmf of the initial state of the machine. It must be a 1D-array of length $|\mathcal{S}|$. The default value is uniform over all states.
 
-        :code:`final_state_distribution` : 1D-array of :obj:`float`, optional
-            The :term:`pmf` of the final state of the machine. It must be a 1D-array of length :math:`|\\mathcal{S}|`. The default value is uniform over all states.
+            final_state_distribution (Optional[Array1D[float]]): The pmf of the final state of the machine. It must be a 1D-array of length $|\mathcal{S}|$. The default value is uniform over all states.
 
-        .. rubric:: Output
+        Returns:
 
-        :code:`input_posteriors` : 2D-array of :obj:`float`
-            The posterior :term:`pmf` of each input, given the observed sequence, of shape :math:`L \\times |\\mathcal{X}|`. The element in row :math:`t \\in [0 : L)` and column :math:`x \\in \\mathcal{X}` is :math:`p(x_t = x \\mid \\mathbf{z})`.
+            input_posteriors (Array2D[float]): The posterior pmf of each input, given the observed sequence, of shape $L \times |\mathcal{X}|$. The element in row $t \in [0 : L)$ and column $x \in \mathcal{X}$ is $p(x_t = x \mid \mathbf{z})$.
         """
         L, num_states, num_input_symbols = len(observed_sequence), self._num_states, self._num_input_symbols
 
         if input_priors is None:
             input_priors = np.ones((L, num_input_symbols)) / num_input_symbols
         if initial_state_distribution is None:
             initial_state_distribution = np.ones(num_states) / num_states
-        if initial_state_distribution is None:
+        if final_state_distribution is None:
             final_state_distribution = np.ones(num_states) / num_states
 
         log_gamma = np.full((L, num_states, num_states), fill_value=-np.inf)
         log_alpha = np.full((L + 1, num_states), fill_value=-np.inf)
         log_beta = np.full((L + 1, num_states), fill_value=-np.inf)
 
-        with np.errstate(divide='ignore'):
+        with np.errstate(divide="ignore"):
             log_input_priors = np.log(input_priors)
             log_alpha[0, :] = np.log(initial_state_distribution)
             log_beta[L, :] = np.log(final_state_distribution)
 
         for t, z in enumerate(observed_sequence):
             for x, s0 in np.ndindex(num_input_symbols, num_states):
                 y, s1 = self._outputs[s0, x], self._next_states[s0, x]
```

### Comparing `komm-0.7.4/komm/_source_coding.py` & `komm-0.8.2/src/komm/_error_control_block/BlockCode.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,480 +1,498 @@
-import heapq
+import functools
 import itertools
 
 import numpy as np
 
-__all__ = ['FixedToVariableCode', 'VariableToFixedCode',
-           'HuffmanCode', 'TunstallCode']
+from .._algebra.util import null_matrix, right_inverse
+from .._aux import tag
+from .._util import binlist2int, int2binlist
 
 
-class FixedToVariableCode:
+class BlockCode:
+    r"""
+    General binary linear block code. It is characterized by its *generator matrix* $G$, a binary $k \times n$ matrix, and by its *parity-check matrix* $H$, a binary $m \times n$ matrix. Those matrix are related by $G H^\top = 0$. The parameters $k$, $m$, and $n$ are called the code *dimension*, *redundancy*, and *length*, respectively, and are related by $k + m = n$. For more details, see <cite>LC04, Ch. 3</cite>.
     """
-    Binary (prefix-free) fixed-to-variable length code. Let :math:`\\mathcal{X}` be the alphabet of some discrete source. A *binary fixed-to-variable length code* of source block size :math:`k` is defined by an encoding mapping :math:`\\mathrm{Enc} : \\mathcal{X}^k \\to \\{ 0, 1 \\}^+`, where :math:`\\{ 0, 1 \\}^+` denotes the set of all finite-length, non-empty binary strings. Here, for simplicity, the source alphabet is always taken as :math:`\\mathcal{X} = \\{0, 1, \\ldots, |\\mathcal{X} - 1| \\}`. The elements in the image of :math:`\\mathrm{Enc}` are called *codewords*.
 
-    Also, we only consider *prefix-free* codes, in which no codeword is a prefix of any other codeword.
-    """
-    def __init__(self, codewords, source_cardinality=None):
-        """
-        Constructor for the class. It expects the following parameters:
-
-        :code:`codewords` : :obj:`list` of :obj:`tuple` of :obj:`int`
-            The codewords of the code. Must be a list of length :math:`|\\mathcal{X}|^k` containing tuples of integers in :math:`\\{ 0, 1 \\}`. The tuple in position :math:`i` of :code:`codewords` should be equal to :math:`\\mathrm{Enc}(u)`, where :math:`u` is the :math:`i`-th element in the lexicographic ordering of :math:`\\mathcal{X}^k`.
+    def __init__(self):
+        self._generator_matrix = None
+        self._parity_check_matrix = None
+        self._parity_submatrix = None
+        self._information_set = None
+        self._parity_set = None
+        self._length = None
+        self._dimension = None
+        self._redundancy = None
+        self._constructed_from = None
+        self._minimum_distance = None
+        self._codeword_weight_distribution = None
+        self._coset_leader_weight_distribution = None
+
+    def _init_from_generator_matrix(self, generator_matrix):
+        self._generator_matrix = np.array(generator_matrix, dtype=int) % 2
+        self._dimension, self._length = self._generator_matrix.shape
+        self._redundancy = self._length - self._dimension
+        self._constructed_from = "generator_matrix"
+
+    def _init_from_parity_check_matrix(self, parity_check_matrix):
+        self._parity_check_matrix = np.array(parity_check_matrix, dtype=int) % 2
+        self._redundancy, self._length = self._parity_check_matrix.shape
+        self._dimension = self._length - self._redundancy
+        self._constructed_from = "parity_check_matrix"
+
+    def _init_from_parity_submatrix(self, parity_submatrix, information_set="left"):
+        self._parity_submatrix = np.array(parity_submatrix, dtype=int) % 2
+        self._dimension, self._redundancy = self._parity_submatrix.shape
+        self._length = self._dimension + self._redundancy
+        if information_set == "left":
+            self._information_set = np.arange(self._dimension)
+        elif information_set == "right":
+            self._information_set = np.arange(self._redundancy, self._length)
+        else:
+            self._information_set = np.array(information_set, dtype=int)
+        if (
+            self._information_set.size != self._dimension
+            or self._information_set.min() < 0
+            or self._information_set.max() > self._length
+        ):
+            raise ValueError("Parameter 'information_set' must be a 'k'-subset of 'range(n)'")
+        self._parity_set = np.setdiff1d(np.arange(self._length), self._information_set)
+        self._generator_matrix = np.empty((self._dimension, self._length), dtype=int)
+        self._generator_matrix[:, self._information_set] = np.eye(self._dimension, dtype=int)
+        self._generator_matrix[:, self._parity_set] = self._parity_submatrix
+        self._parity_check_matrix = np.empty((self._redundancy, self._length), dtype=int)
+        self._parity_check_matrix[:, self._information_set] = self._parity_submatrix.T
+        self._parity_check_matrix[:, self._parity_set] = np.eye(self._redundancy, dtype=int)
+        self._constructed_from = "parity_submatrix"
+
+    @classmethod
+    def from_generator_matrix(cls, generator_matrix):
+        r"""
+        Constructs a binary linear block code from its generator matrix.
+
+        Parameters:
+
+            generator_matrix (Array2D[int]): Generator matrix $G$ for the code, which is a $k \times n$ binary matrix.
+
+        Examples:
+
+            >>> komm.BlockCode().from_generator_matrix([[1, 0, 0, 0, 1, 1], [0, 1, 0, 1, 0, 1], [0, 0, 1, 1, 1, 0]])
+            BlockCode.from_generator_matrix([[1, 0, 0, 0, 1, 1], [0, 1, 0, 1, 0, 1], [0, 0, 1, 1, 1, 0]])
+        """
+        obj = cls()
+        obj._init_from_generator_matrix(generator_matrix)
+        return obj
+
+    @classmethod
+    def from_parity_check_matrix(cls, parity_check_matrix):
+        r"""
+        Constructs a binary linear block code from its parity-check matrix.
+
+        Parameters:
+
+            parity_check_matrix (Array2D[int]): Parity-check matrix $H$ for the code, which is an $m \times n$ binary matrix.
+
+        Examples:
+
+            >>> komm.BlockCode().from_parity_check_matrix([[0, 1, 1, 1, 0, 0], [1, 0, 1, 0, 1, 0], [1, 1, 0, 0, 0, 1]])
+            BlockCode.from_parity_check_matrix([[0, 1, 1, 1, 0, 0], [1, 0, 1, 0, 1, 0], [1, 1, 0, 0, 0, 1]])
+        """
+        obj = cls()
+        obj._init_from_parity_check_matrix(parity_check_matrix)
+        return obj
+
+    @classmethod
+    def from_parity_submatrix(cls, parity_submatrix, information_set="left"):
+        r"""
+        Constructs a binary linear block code from its parity submatrix and information set.
+
+        Parameters:
+
+            parity_submatrix (Array2D[int]): Parity submatrix $P$ for the code, which is a $k \times m$ binary matrix.
+
+            information_set (Optional[Array1D[int] | str]): Either an array containing the indices of the information positions, which must be a $k$-sublist of $[0 : n)$, or one of the strings `'left'` or `'right'`. The default value is `'left'`.
+
+        Examples:
+
+            >>> komm.BlockCode().from_parity_submatrix([[0, 1, 1], [1, 0, 1], [1, 1, 0]])
+            BlockCode.from_parity_submatrix([[0, 1, 1], [1, 0, 1], [1, 1, 0]], information_set=[0, 1, 2])
+        """
+        obj = cls()
+        obj._init_from_parity_submatrix(parity_submatrix, information_set)
+        return obj
 
-        :code:`source_cardinality` : :obj:`int`, optional
-            The cardinality :math:`|\\mathcal{X}|` of the source alphabet. The default value is :code:`len(codewords)`, yielding a source block size :math:`k = 1`.
-
-        *Note:* The source block size :math:`k` is inferred from :code:`len(codewords)` and :code:`source_cardinality`.
-
-        .. rubric:: Examples
-
-        >>> code = komm.FixedToVariableCode(codewords=[(0,), (1,0), (1,1)])
-        >>> pprint(code.enc_mapping)
-        {(0,): (0,), (1,): (1, 0), (2,): (1, 1)}
-        >>> pprint(code.dec_mapping)
-        {(0,): (0,), (1, 0): (1,), (1, 1): (2,)}
-
-        >>> code = komm.FixedToVariableCode(codewords=[(0,), (1,0,0), (1,1), (1,0,1)], source_cardinality=2)
-        >>> pprint(code.enc_mapping)
-        {(0, 0): (0,), (0, 1): (1, 0, 0), (1, 0): (1, 1), (1, 1): (1, 0, 1)}
-        >>> pprint(code.dec_mapping)
-        {(0,): (0, 0), (1, 0, 0): (0, 1), (1, 0, 1): (1, 1), (1, 1): (1, 0)}
-        """
-        # TODO: Assert prefix-free
-        self._codewords = codewords
-        self._source_cardinality = len(codewords) if source_cardinality is None else int(source_cardinality)
-        self._source_block_size = 1
-        while self._source_cardinality ** self._source_block_size < len(codewords):
-            self._source_block_size += 1
-
-        if self._source_cardinality ** self._source_block_size != len(codewords):
-            raise ValueError("Invalid number of codewords")
-
-        self._enc_mapping = {}
-        self._dec_mapping = {}
-        for symbols, bits in zip(itertools.product(range(self._source_cardinality), repeat=self._source_block_size), codewords):
-            self._enc_mapping[symbols] = tuple(bits)
-            self._dec_mapping[tuple(bits)] = symbols
+    def __repr__(self):
+        if self._constructed_from == "generator_matrix":
+            args = f"{self._generator_matrix.tolist()}"
+        elif self._constructed_from == "parity_check_matrix":
+            args = f"{self._parity_check_matrix.tolist()}"
+        elif self._constructed_from == "parity_submatrix":
+            args = f"{self._parity_submatrix.tolist()}, information_set={self._information_set.tolist()}"
+        return f"{self.__class__.__name__}.from_{self._constructed_from}({args})"
 
     @property
-    def source_cardinality(self):
-        """
-        The cardinality :math:`|\\mathcal{X}|` of the source alphabet.
-        """
-        return self._source_cardinality
+    def length(self):
+        r"""
+        The length $n$ of the code.
 
-    @property
-    def source_block_size(self):
-        """
-        The source block size :math:`k`.
-        """
-        return self._source_block_size
+        Examples:
 
-    @property
-    def enc_mapping(self):
-        """
-        The encoding mapping :math:`\\mathrm{Enc}` of the code.
+            >>> code = komm.BlockCode.from_parity_submatrix([[0, 1, 1], [1, 0, 1], [1, 1, 0]])
+            >>> code.length
+            6
         """
-        return self._enc_mapping
+        return self._length
 
     @property
-    def dec_mapping(self):
-        """
-        The decoding mapping :math:`\\mathrm{Dec}` of the code.
-        """
-        return self._dec_mapping
+    def dimension(self):
+        r"""
+        The dimension $k$ of the code.
 
-    def rate(self, pmf):
-        """
-        Computes the expected rate :math:`R` of the code, assuming a given :term:`pmf`. It is given in bits per source symbol.
+        Examples:
 
-        .. rubric:: Input
+            >>> code = komm.BlockCode.from_parity_submatrix([[0, 1, 1], [1, 0, 1], [1, 1, 0]])
+            >>> code.dimension
+            3
+        """
+        return self._dimension
 
-        :code:`pmf` : 1D-array of :obj:`float`
-            The (first-order) probability mass function :math:`p_X(x)` to be assumed.
+    @property
+    def redundancy(self):
+        r"""
+        The redundancy $m$ of the code.
 
-        .. rubric:: Output
+        Examples:
 
-        :code:`rate` : :obj:`float`
-            The expected rate :math:`R` of the code.
+            >>> code = komm.BlockCode.from_parity_submatrix([[0, 1, 1], [1, 0, 1], [1, 1, 0]])
+            >>> code.redundancy
+            3
+        """
+        return self._redundancy
 
-        .. rubric:: Examples
+    @property
+    def rate(self):
+        r"""
+        The rate $R = k/n$ of the code.
 
-        >>> code = komm.FixedToVariableCode([(0,), (1,0), (1,1)])
-        >>> code.rate([0.5, 0.25, 0.25])
-        1.5
-        """
-        probabilities = np.array([np.prod(ps) for ps in itertools.product(pmf, repeat=self._source_block_size)])
-        lengths = [len(bits) for bits in self._codewords]
-        return np.dot(lengths, probabilities) / self._source_block_size
+        Examples:
 
-    def encode(self, symbol_sequence):
+            >>> code = komm.BlockCode.from_parity_submatrix([[0, 1, 1], [1, 0, 1], [1, 1, 0]])
+            >>> code.rate
+            0.5
         """
-        Encodes a given sequence of symbols to its corresponding sequence of bits.
-
-        .. rubric:: Input
+        return self._dimension / self._length
 
-        :code:`symbol_sequence` : 1D-array of :obj:`int`
-            The sequence of symbols to be encoded. Must be a 1D-array with elements in :math:`\\mathcal{X} = \\{0, 1, \\ldots, |\\mathcal{X} - 1| \\}`. Its length must be a multiple of :math:`k`.
+    @functools.cached_property
+    def minimum_distance(self):
+        r"""
+        The minimum distance $d$ of the code. This is equal to the minimum Hamming weight of the non-zero codewords.
 
-        .. rubric:: Output
+        Examples:
 
-        :code:`bit_sequence` : 1D-array of :obj:`int`
-            The sequence of bits corresponding to :code:`symbol_sequence`.
+            >>> code = komm.BlockCode.from_parity_submatrix([[0, 1, 1], [1, 0, 1], [1, 1, 0]])
+            >>> code.minimum_distance
+            3
+        """
+        if self._minimum_distance is None:
+            return np.flatnonzero(self.codeword_weight_distribution)[1]
+        return self._minimum_distance
 
-        .. rubric:: Examples
+    @functools.cached_property
+    def packing_radius(self):
+        r"""
+        The packing radius of the code. This is also called the *error-correcting capability* of the code, and is equal to $\lfloor (d - 1) / 2 \rfloor$.
 
-        >>> code = komm.FixedToVariableCode([(0,), (1,0), (1,1)])
-        >>> code.encode([1, 0, 1, 0, 2, 0])
-        array([1, 0, 0, 1, 0, 0, 1, 1, 0])
-        """
-        symbols_reshaped = np.reshape(symbol_sequence, newshape=(-1, self._source_block_size))
-        return np.concatenate([self._enc_mapping[tuple(symbols)] for symbols in symbols_reshaped])
+        Examples:
 
-    def decode(self, bit_sequence):
+            >>> code = komm.BlockCode.from_parity_submatrix([[0, 1, 1], [1, 0, 1], [1, 1, 0]])
+            >>> code.packing_radius
+            1
         """
-        Decodes a given sequence of bits to its corresponding sequence of symbols.
+        return (self.minimum_distance - 1) // 2
 
-        .. rubric:: Input
+    @functools.cached_property
+    def covering_radius(self):
+        r"""
+        The covering radius of the code. This is equal to the maximum Hamming weight of the coset leaders.
 
-        :code:`bit_sequence` : 1D-array of :obj:`int`
-            The sequence of bits to be decoded. Must be a 1D-array with elements in :math:`\\{ 0, 1 \\}`.
+        Examples:
 
-        .. rubric:: Output
+            >>> code = komm.BlockCode.from_parity_submatrix([[0, 1, 1], [1, 0, 1], [1, 1, 0]])
+            >>> code.covering_radius
+            2
+        """
+        return np.flatnonzero(self.coset_leader_weight_distribution)[-1]
 
-        :code:`symbol_sequence` : 1D-array of :obj:`int`
-            The sequence of symbols corresponding to :code:`bits`.
+    @functools.cached_property
+    def generator_matrix(self):
+        r"""
+        The generator matrix $G$ of the code. It as a $k \times n$ binary matrix, where $k$ is the code dimension, and $n$ is the code length.
 
-        .. rubric:: Examples
+        Examples:
 
-        >>> code = komm.FixedToVariableCode([(0,), (1,0), (1,1)])
-        >>> code.decode([1, 0, 0, 1, 0, 0, 1, 1, 0])
-        array([1, 0, 1, 0, 2, 0])
+            >>> code = komm.BlockCode.from_parity_submatrix([[0, 1, 1], [1, 0, 1], [1, 1, 0]])
+            >>> code.generator_matrix
+            array([[1, 0, 0, 0, 1, 1],
+                   [0, 1, 0, 1, 0, 1],
+                   [0, 0, 1, 1, 1, 0]])
         """
-        return np.array(_parse_prefix_free(bit_sequence, self._dec_mapping))
-
-    def __repr__(self):
-        args = 'codewords={}'.format(self._codewords)
-        return '{}({})'.format(self.__class__.__name__, args)
+        if self._generator_matrix is None:
+            return null_matrix(self._parity_check_matrix)
+        return self._generator_matrix
 
+    @functools.cached_property
+    def parity_check_matrix(self):
+        r"""
+        The parity-check matrix $H$ of the code. It as an $m \times n$ binary matrix, where $m$ is the code redundancy, and $n$ is the code length.
 
-class HuffmanCode(FixedToVariableCode):
-    """
-    Huffman code. It is an optimal (minimal expected rate) fixed-to-variable length code (:class:`FixedToVariableCode`) for a given probability mass function.
+        Examples:
 
-    .. rubric:: Examples
-
-    >>> code = komm.HuffmanCode([0.7, 0.15, 0.15])
-    >>> pprint(code.enc_mapping)
-    {(0,): (0,), (1,): (1, 1), (2,): (1, 0)}
-
-    >>> code = komm.HuffmanCode([0.7, 0.15, 0.15], source_block_size=2)
-    >>> pprint(code.enc_mapping)
-    {(0, 0): (1,),
-     (0, 1): (0, 0, 0, 0),
-     (0, 2): (0, 1, 1),
-     (1, 0): (0, 1, 0),
-     (1, 1): (0, 0, 0, 1, 1, 1),
-     (1, 2): (0, 0, 0, 1, 1, 0),
-     (2, 0): (0, 0, 1),
-     (2, 1): (0, 0, 0, 1, 0, 1),
-     (2, 2): (0, 0, 0, 1, 0, 0)}
-    """
-    def __init__(self, pmf, source_block_size=1, policy='high'):
+            >>> code = komm.BlockCode.from_parity_submatrix([[0, 1, 1], [1, 0, 1], [1, 1, 0]])
+            >>> code.parity_check_matrix
+            array([[0, 1, 1, 1, 0, 0],
+                   [1, 0, 1, 0, 1, 0],
+                   [1, 1, 0, 0, 0, 1]])
         """
-        Constructor for the class. It expects the following parameters:
+        if self._parity_check_matrix is None:
+            return null_matrix(self._generator_matrix)
+        return self._parity_check_matrix
 
-        :code:`pmf` : 1D-array of :obj:`float`
-            The probability mass function used to construct the code.
+    @functools.cached_property
+    def codeword_table(self):
+        r"""
+        The codeword table of the code. This is a $2^k \times n$ matrix whose rows are all the codewords. The codeword in row $i$ corresponds to the message whose binary representation (MSB in the right) is $i$.
 
-        :code:`source_block_size` : :obj:`int`, optional
-            The source block size :math:`k`. The default value is :math:`k = 1`.
+        Examples:
 
-        :code:`policy` : :obj:`str`, optional
-            The policy to be used when constructing the code. It must be either :code:`'high'` (move combined symbols as high as possible) or :code:`'low'` (move combined symbols as low as possible). The default value is :code:`'high'`.
+            >>> code = komm.BlockCode.from_parity_submatrix([[0, 1, 1], [1, 0, 1], [1, 1, 0]])
+            >>> code.codeword_table
+            array([[0, 0, 0, 0, 0, 0],
+                   [1, 0, 0, 0, 1, 1],
+                   [0, 1, 0, 1, 0, 1],
+                   [1, 1, 0, 1, 1, 0],
+                   [0, 0, 1, 1, 1, 0],
+                   [1, 0, 1, 1, 0, 1],
+                   [0, 1, 1, 0, 1, 1],
+                   [1, 1, 1, 0, 0, 0]])
         """
-        self._pmf = np.array(pmf)
-        self._policy = policy
+        codeword_table = np.empty([2**self._dimension, self._length], dtype=int)
+        for i in range(2**self._dimension):
+            message = int2binlist(i, width=self._dimension)
+            codeword_table[i] = self.encode(message)
+        return codeword_table
 
-        if policy not in ['high', 'low']:
-            raise ValueError("Parameter 'policy' must be in {'high', 'low'}")
+    @functools.cached_property
+    def codeword_weight_distribution(self):
+        r"""
+        The codeword weight distribution of the code. This is an array of shape $(n + 1)$ in which element in position $w$ is equal to the number of codewords of Hamming weight $w$, for $w \in [0 : n]$.
 
-        super().__init__(codewords=HuffmanCode._huffman_algorithm(pmf, source_block_size, policy),
-                         source_cardinality=self._pmf.size)
+        Examples:
 
-    @property
-    def pmf(self):
-        """
-        The probability mass function used to construct the code. This property is read-only.
+            >>> code = komm.BlockCode.from_parity_submatrix([[0, 1, 1], [1, 0, 1], [1, 1, 0]])
+            >>> code.codeword_weight_distribution
+            array([1, 0, 0, 4, 3, 0, 0])
         """
-        return self._pmf
+        if self._codeword_weight_distribution is None:
+            return np.bincount(np.sum(self.codeword_table, axis=1), minlength=self._length + 1)
+        return self._codeword_weight_distribution
 
-    @staticmethod
-    def _huffman_algorithm(pmf, source_block_size, policy):
-        class Node:
-            def __init__(self, index, probability):
-                self.index = index
-                self.probability = probability
-                self.parent = None
-                self.bit = None
-            def __lt__(self, other):
-                if policy == 'high':
-                    return (self.probability, self.index) < (other.probability, other.index)
-                elif policy == 'low':
-                    return (self.probability, -self.index) < (other.probability, -other.index)
-
-        tree = [Node(i, np.prod(probs)) for (i, probs) in enumerate(itertools.product(pmf, repeat=source_block_size))]
-        queue = [node for node in tree]
-        heapq.heapify(queue)
-        while len(queue) > 1:
-            node1 = heapq.heappop(queue)
-            node0 = heapq.heappop(queue)
-            node1.bit = 1
-            node0.bit = 0
-            node = Node(index=len(tree), probability=node0.probability + node1.probability)
-            node0.parent = node1.parent = node.index
-            heapq.heappush(queue, node)
-            tree.append(node)
-
-        codewords = []
-        for symbol in range(len(pmf)**source_block_size):
-            node = tree[symbol]
-            bits = []
-            while node.parent is not None:
-                bits.insert(0, node.bit)
-                node = tree[node.parent]
-            codewords.append(tuple(bits))
+    @functools.cached_property
+    def coset_leader_table(self):
+        r"""
+        The coset leader table of the code. This is a $2^m \times n$ matrix whose rows are all the coset leaders. The coset leader in row $i$ corresponds to the syndrome whose binary representation (MSB in the right) is $i$. This may be used as a LUT for syndrome-based decoding.
 
-        return codewords
+        Examples:
 
-    def __repr__(self):
-        args = 'pmf={}, source_block_size={}'.format(self._pmf.tolist(), self._source_block_size)
-        return '{}({})'.format(self.__class__.__name__, args)
+            >>> code = komm.BlockCode.from_parity_submatrix([[0, 1, 1], [1, 0, 1], [1, 1, 0]])
+            >>> code.coset_leader_table
+            array([[0, 0, 0, 0, 0, 0],
+                   [0, 0, 0, 1, 0, 0],
+                   [0, 0, 0, 0, 1, 0],
+                   [0, 0, 1, 0, 0, 0],
+                   [0, 0, 0, 0, 0, 1],
+                   [0, 1, 0, 0, 0, 0],
+                   [1, 0, 0, 0, 0, 0],
+                   [1, 0, 0, 1, 0, 0]])
+        """
+        coset_leader_table = np.empty([2**self._redundancy, self._length], dtype=int)
+        taken = []
+        for w in range(self._length + 1):
+            for idx in itertools.combinations(range(self._length), w):
+                errorword = np.zeros(self._length, dtype=int)
+                errorword[list(idx)] = 1
+                syndrome = np.dot(errorword, self.parity_check_matrix.T) % 2
+                syndrome_int = binlist2int(syndrome)
+                if syndrome_int not in taken:
+                    coset_leader_table[syndrome_int] = np.array(errorword)
+                    taken.append(syndrome_int)
+                if len(taken) == 2**self.redundancy:
+                    break
+        return coset_leader_table
 
+    @functools.cached_property
+    def coset_leader_weight_distribution(self):
+        r"""
+        The coset leader weight distribution of the code. This is an array of shape $(n + 1)$ in which element in position $w$ is equal to the number of coset leaders of weight $w$, for $w \in [0 : n]$.
 
-class VariableToFixedCode:
-    """
-    Binary (prefix-free) variable-to-fixed length code. Let :math:`\\mathcal{X}` be the alphabet of some discrete source. A *binary variable-to-fixed length code* of code block size :math:`n` is defined by a (possibly partial) decoding mapping :math:`\\mathrm{Dec} : \\{ 0, 1 \\}^n \\to \\mathcal{X}^+`, where :math:`\\mathcal{X}^+` denotes the set of all finite-length, non-empty strings from the source alphabet. Here, for simplicity, the source alphabet is always taken as :math:`\\mathcal{X} = \\{0, 1, \\ldots, |\\mathcal{X} - 1| \\}`. The elements in the image of :math:`\\mathrm{Dec}` are called *sourcewords*.
+        Examples:
 
-    Also, we only consider *prefix-free* codes, in which no sourceword is a prefix of any other sourceword.
-    """
-    def __init__(self, sourcewords):
+            >>> code = komm.BlockCode.from_parity_submatrix([[0, 1, 1], [1, 0, 1], [1, 1, 0]])
+            >>> code.coset_leader_weight_distribution
+            array([1, 6, 1, 0, 0, 0, 0])
         """
-        Constructor for the class. It expects the following parameters:
+        if self._coset_leader_weight_distribution is None:
+            return np.bincount(np.sum(self.coset_leader_table, axis=1), minlength=self._length + 1)
+        return self._coset_leader_weight_distribution
 
-        :code:`sourcewords` : :obj:`list` of :obj:`tuple` of :obj:`int`
-            The sourcewords of the code. Must be a list of length at most :math:`2^n` containing tuples of integers in :math:`\\mathcal{X}`. The tuple in position :math:`i` of :code:`sourcewords` should be equal to :math:`\\mathrm{Dec}(v)`, where :math:`v` is the :math:`i`-th element in the lexicographic ordering of :math:`\\{ 0, 1 \\}^n`.
+    @functools.cached_property
+    def _generator_matrix_right_inverse(self):
+        return right_inverse(self.generator_matrix)
 
-        *Note:* The code block size :math:`n` is inferred from :code:`len(sourcewords)`.
+    def encode(self, message, method=None):
+        r"""
+        Encodes a given message to its corresponding codeword.
 
-        .. rubric:: Examples
-
-        >>> code = komm.VariableToFixedCode(sourcewords=[(1,), (2,), (0,1), (0,2), (0,0,0), (0,0,1), (0,0,2)])
-        >>> pprint(code.enc_mapping)
-        {(0, 0, 0): (1, 0, 0),
-         (0, 0, 1): (1, 0, 1),
-         (0, 0, 2): (1, 1, 0),
-         (0, 1): (0, 1, 0),
-         (0, 2): (0, 1, 1),
-         (1,): (0, 0, 0),
-         (2,): (0, 0, 1)}
-        >>> pprint(code.dec_mapping)
-        {(0, 0, 0): (1,),
-         (0, 0, 1): (2,),
-         (0, 1, 0): (0, 1),
-         (0, 1, 1): (0, 2),
-         (1, 0, 0): (0, 0, 0),
-         (1, 0, 1): (0, 0, 1),
-         (1, 1, 0): (0, 0, 2)}
-        """
-        # TODO: Assert prefix-free
-        self._sourcewords = sourcewords
-        self._source_cardinality = max(itertools.chain(*sourcewords)) + 1
-        self._code_block_size = (len(sourcewords) - 1).bit_length()
-        self._enc_mapping = {}
-        self._dec_mapping = {}
-        for symbols, bits in zip(itertools.product(range(2), repeat=self._code_block_size), sourcewords):
-            self._enc_mapping[bits] = tuple(symbols)
-            self._dec_mapping[tuple(symbols)] = bits
+        Parameters:
 
-    @property
-    def source_cardinality(self):
-        """
-        The cardinality :math:`|\\mathcal{X}|` of the source alphabet.
-        """
-        return self._source_cardinality
+            message (Array1D[int]): The message to be encoded. Its length must be $k$.
 
-    @property
-    def code_block_size(self):
-        """
-        The code block size :math:`n`.
-        """
-        return self._code_block_size
+            method (Optional[str]): The encoding method to be used.
 
-    @property
-    def enc_mapping(self):
-        """
-        The encoding mapping :math:`\\mathrm{Enc}` of the code.
-        """
-        return self._enc_mapping
-
-    @property
-    def dec_mapping(self):
-        """
-        The decoding mapping :math:`\\mathrm{Dec}` of the code.
-        """
-        return self._dec_mapping
+        Returns:
 
-    def rate(self, pmf):
+            codeword (Array1D[int]): The codeword corresponding to `message`. Its length is equal to $n$.
         """
-        Computes the expected rate :math:`R` of the code, assuming a given :term:`pmf`. It is given in bits per source symbol.
-
-        .. rubric:: Input
+        message = np.array(message)
 
-        :code:`pmf` : 1D-array of :obj:`float`
-            The (first-order) probability mass function :math:`p_X(x)` to be assumed.
+        if message.size != self._dimension:
+            raise ValueError("Length of 'message' must be equal to the code dimension")
 
-        .. rubric:: Output
+        if method is None:
+            method = self._default_encoder()
 
-        :code:`rate` : :obj:`float`
-            The expected rate :math:`R` of the code.
+        encoder = getattr(self, "_encode_" + method)
+        codeword = encoder(message)
 
-        .. rubric:: Examples
+        return codeword
 
-        >>> code = komm.VariableToFixedCode([(0,0,0), (0,0,1), (0,1), (1,)])
-        >>> code.rate([2/3, 1/3])
-        0.9473684210526315
-        """
-        probabilities = np.array([np.prod([pmf[x] for x in symbols]) for symbols in self._sourcewords])
-        lengths = [len(symbols) for symbols in self._sourcewords]
-        return self._code_block_size / np.dot(lengths, probabilities)
+    def _encode_generator_matrix(self, message):
+        codeword = np.dot(message, self.generator_matrix) % 2
+        return codeword
 
-    def encode(self, symbol_sequence):
-        """
-        Encodes a given sequence of symbols to its corresponding sequence of bits.
+    def _encode_systematic_generator_matrix(self, message):
+        codeword = np.empty(self._length, dtype=int)
+        codeword[self._information_set] = message
+        codeword[self._parity_set] = np.dot(message, self._parity_submatrix) % 2
+        return codeword
 
-        .. rubric:: Input
+    def _default_encoder(self):
+        if self._constructed_from == "parity_submatrix":
+            return "systematic_generator_matrix"
+        else:
+            return "generator_matrix"
 
-        :code:`symbol_sequence` : 1D-array of :obj:`int`
-            The sequence of symbols to be encoded. Must be a 1D-array with elements in :math:`\\mathcal{X} = \\{0, 1, \\ldots, |\\mathcal{X} - 1| \\}`.
+    def message_from_codeword(self, codeword):
+        r"""
+        Returns the message corresponding to a given codeword. In other words, applies the inverse encoding map.
 
-        .. rubric:: Output
+        Parameters:
 
-        :code:`bit_sequence` : 1D-array of :obj:`int`
-            The sequence of bits corresponding to :code:`symbol_sequence`.
+            codeword (Array1D[int]): A codeword from the code. Its length must be $n$.
 
-        .. rubric:: Examples
+        Returns:
 
-        >>> code = komm.VariableToFixedCode([(0,0,0), (0,0,1), (0,1), (1,)])
-        >>> code.encode([0, 0, 0, 1, 0, 0, 1, 0, 0, 1, 0, 0, 1, 0, 0, 0])
-        array([0, 0, 1, 1, 0, 1, 0, 1, 0, 1, 0, 0])
+            message (Array1D[int]): The message corresponding to `codeword`. Its length is equal to $k$.
         """
-        return np.array(_parse_prefix_free(symbol_sequence, self._enc_mapping))
+        if self._constructed_from == "parity_submatrix":
+            return codeword[self._information_set]
+        else:
+            return np.dot(codeword, self._generator_matrix_right_inverse) % 2
 
-    def decode(self, bit_sequence):
-        """
-        Decodes a given sequence of bits to its corresponding sequence of symbols.
+    def decode(self, recvword, method=None, **kwargs):
+        r"""
+        Decodes a received word to a message.
 
-        .. rubric:: Input
+        Parameters:
 
-        :code:`bit_sequence` : 1D-array of :obj:`int`
-            The sequence of bits to be decoded. Must be a 1D-array with elements in :math:`\\{ 0, 1 \\}`.  Its length must be a multiple of :math:`n`.
+            recvword (Array1D[int] | Array1D[float]): The word to be decoded. If using a hard-decision decoding method, then the elements of the array must be bits (integers in $\\{ 0, 1 \\}$). If using a soft-decision decoding method, then the elements of the array must be soft-bits (floats standing for log-probability ratios, in which positive values represent bit $0$ and negative values represent bit $1$). Its length must be $n$.
 
-        .. rubric:: Output
+            method (Optional[str]): The decoding method to be used.
 
-        :code:`symbol_sequence` : 1D-array of :obj:`int`
-            The sequence of symbols corresponding to :code:`bits`.
+            kwargs (): Keyword arguments to be passed to the decoding method.
 
-        .. rubric:: Examples
+        Returns:
 
-        >>> code = komm.VariableToFixedCode([(0,0,0), (0,0,1), (0,1), (1,)])
-        >>> code.decode([0, 0, 1, 1, 0, 1, 0, 1, 0, 1, 0, 0])
-        array([0, 0, 0, 1, 0, 0, 1, 0, 0, 1, 0, 0, 1, 0, 0, 0])
+            message_hat (Array1D[int]): The message decoded from `recvword`. Its length is equal to $k$.
         """
-        bits_reshaped = np.reshape(bit_sequence, newshape=(-1, self._code_block_size))
-        return np.concatenate([self._dec_mapping[tuple(bits)] for bits in bits_reshaped])
-
-    def __repr__(self):
-        args = 'sourcewords={}'.format(self._sourcewords)
-        return '{}({})'.format(self.__class__.__name__, args)
+        recvword = np.array(recvword)
 
+        if recvword.size != self._length:
+            raise ValueError("Length of 'recvword' must be equal to the code length")
 
-class TunstallCode(VariableToFixedCode):
-    """
-    Tunstall code. It is an optimal (minimal expected rate) variable-to-fixed length code (:class:`VariableToFixedCode`) for a given probability mass function.
+        if method is None:
+            method = self._default_decoder(recvword.dtype)
 
-    .. rubric:: Examples
+        decoder = getattr(self, "_decode_" + method)
 
-    >>> code = komm.TunstallCode([0.6, 0.3, 0.1], code_block_size=3)
-    >>> pprint(code.enc_mapping)
-    {(0, 0, 0): (0, 0, 0),
-     (0, 0, 1): (0, 0, 1),
-     (0, 0, 2): (0, 1, 0),
-     (0, 1): (0, 1, 1),
-     (0, 2): (1, 0, 0),
-     (1,): (1, 0, 1),
-     (2,): (1, 1, 0)}
-    """
-    def __init__(self, pmf, code_block_size):
-        """
-        Constructor for the class. It expects the following parameters:
+        if decoder.target == "codeword":
+            message_hat = self.message_from_codeword(decoder(recvword, **kwargs))
+        elif decoder.target == "message":
+            message_hat = decoder(recvword, **kwargs)
 
-        :code:`pmf` : 1D-array of :obj:`float`
-            The probability mass function used to construct the code.
+        return message_hat
 
-        :code:`code_block_size` : :obj:`int`, optional
-            The code block size :math:`n`. Must satisfy :math:`2^n \geq |\\mathcal{X}|`, where :math:`|\\mathcal{X}|` is the cardinality of the source alphabet, given by :code:`len(pmf)`.
+    @tag(name="Exhaustive search (hard-decision)", input_type="hard", target="codeword")
+    def _decode_exhaustive_search_hard(self, recvword):
+        r"""
+        Exhaustive search minimum distance hard decoder. Hamming distance.
         """
-        self._pmf = np.array(pmf)
-
-        if 2**code_block_size < len(pmf):
-            raise ValueError("Code block size is too low")
-
-        super().__init__(sourcewords=TunstallCode._tunstall_algorithm(pmf, code_block_size))
+        codewords = self.codeword_table
+        metrics = np.count_nonzero(recvword != codewords, axis=1)
+        codeword_hat = codewords[np.argmin(metrics)]
+        return codeword_hat
 
-    @property
-    def pmf(self):
-        """
-        The probability mass function used to construct the code. This property is read-only.
+    @tag(name="Exhaustive search (soft-decision)", input_type="soft", target="codeword")
+    def _decode_exhaustive_search_soft(self, recvword):
+        r"""
+        Exhaustive search minimum distance soft decoder. Euclidean distance.
         """
-        return self._pmf
-
-    @staticmethod
-    def _tunstall_algorithm(pmf, code_block_size):
-        class Node:
-            def __init__(self, symbols, probability):
-                self.symbols = symbols
-                self.probability = probability
-            def __lt__(self, other):
-                return -self.probability < -other.probability
-
-        queue = [Node((symbol,), probability) for (symbol, probability) in enumerate(pmf)]
-        heapq.heapify(queue)
-
-        while len(queue) + len(pmf) - 1 < 2**code_block_size:
-            node = heapq.heappop(queue)
-            for (symbol, probability) in enumerate(pmf):
-                new_node = Node(node.symbols + (symbol,), node.probability * probability)
-                heapq.heappush(queue, new_node)
-        sourcewords = sorted(node.symbols for node in queue)
+        codewords = self.codeword_table
+        metrics = np.dot(recvword, codewords.T)
+        codeword_hat = codewords[np.argmin(metrics)]
+        return codeword_hat
 
-        return sourcewords
-
-    def __repr__(self):
-        args = 'pmf={}, code_block_size={}'.format(self._pmf.tolist(), self._code_block_size)
-        return '{}({})'.format(self.__class__.__name__, args)
+    @tag(name="Syndrome table", input_type="hard", target="codeword")
+    def _decode_syndrome_table(self, recvword):
+        r"""
+        Syndrome table decoder.
+        """
+        coset_leader_table = self.coset_leader_table
+        syndrome = np.dot(recvword, self.parity_check_matrix.T) % 2
+        syndrome_int = binlist2int(syndrome)
+        errorword_hat = coset_leader_table[syndrome_int]
+        codeword_hat = np.bitwise_xor(recvword, errorword_hat)
+        return codeword_hat
 
+    def _default_decoder(self, dtype):
+        if dtype == int:
+            if self._dimension >= self._redundancy:
+                return "syndrome_table"
+            else:
+                return "exhaustive_search_hard"
+        elif dtype == float:
+            return "exhaustive_search_soft"
 
-def _parse_prefix_free(input_sequence, dictionary):
-    output_sequence = []
-    i = 0
-    while i < len(input_sequence):
-        j = 1
-        while i + j <= len(input_sequence):
-            try:
-                key = tuple(input_sequence[i : i + j])
-                output_sequence.extend(dictionary[key])
-                break
-            except KeyError:
-                j += 1
-        i += j
-    return output_sequence
+    @staticmethod
+    def _extended_parity_submatrix(parity_submatrix):
+        last_column = (1 + np.sum(parity_submatrix, axis=1)) % 2
+        extended_parity_submatrix = np.hstack([parity_submatrix, last_column[np.newaxis].T])
+        return extended_parity_submatrix
+
+    @classmethod
+    def _available_decoding_methods(cls):
+        table = []
+        for name in dir(cls):
+            if name.startswith("_decode_"):
+                identifier = name[8:]
+                method = getattr(cls, name)
+                table.append([method.name, "`{}`".format(identifier), method.input_type])
+        return table
```

### Comparing `komm-0.7.4/komm/_sources.py` & `komm-0.8.2/src/komm/_sources/DiscreteMemorylessSource.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,72 @@
 import numpy as np
 
-from ._util import \
-    _entropy
-
-
-__all__ = ['DiscreteMemorylessSource']
+from .._util import _entropy
 
 
 class DiscreteMemorylessSource:
-    """
-    Discrete memoryless source (DMS). It is defined by an *alphabet* :math:`\\mathcal{X}` and a *probability mass function* (:term:`pmf`) :math:`p_X`. Here, for simplicity, the alphabet is always taken as :math:`\\mathcal{X} = \\{ 0, 1, \\ldots, |\\mathcal{X}| - 1 \\}`. The :term:`pmf` :math:`p_X` gives the probability of the source emitting the symbol :math:`X = x`.
+    r"""
+    Discrete memoryless source (DMS). It is defined by an *alphabet* $\mathcal{X}$ and a *probability mass function* (pmf) $p_X$. Here, for simplicity, the alphabet is always taken as $\mathcal{X} = \\{ 0, 1, \ldots, |\mathcal{X}| - 1 \\}$. The pmf $p_X$ gives the probability of the source emitting the symbol $X = x$.
 
-    To invoke the source, call the object giving the number of symbols to be emitted as parameter (see example below).
+    To invoke the source, call the object giving the number of symbols to be emitted as parameter (see example in the constructor below).
     """
+
     def __init__(self, pmf):
-        """
-        Constructor for the class. It expects the following parameter:
+        r"""
+        Constructor for the class.
 
-        :code:`pmf` : 1D-array of :obj:`float`
-            The source probability mass function :math:`p_X`. The element in position :math:`x \\in \\mathcal{X}` must be equal to :math:`p_X(x)`.
+        Parameters:
 
-        .. rubric:: Examples
+            pmf (Array1D[float]): The source probability mass function $p_X$. The element in position $x \in \mathcal{X}$ must be equal to $p_X(x)$.
 
-        >>> dms = komm.DiscreteMemorylessSource([0.5, 0.4, 0.1])
-        >>> dms(10)  #doctest:+SKIP
-        array([1, 2, 1, 0, 0, 1, 1, 0, 1, 1])
+        Examples:
+
+            >>> np.random.seed(42)
+            >>> dms = komm.DiscreteMemorylessSource([0.5, 0.4, 0.1])
+            >>> dms(10)
+            array([0, 2, 1, 1, 0, 0, 0, 1, 1, 1])
         """
         self.pmf = pmf
 
     @property
     def pmf(self):
-        """
-        The source probability mass function :math:`p_X`. This is a read-and-write property.
+        r"""
+        The source probability mass function $p_X$.
         """
         return self._pmf
 
     @pmf.setter
     def pmf(self, value):
         self._pmf = np.array(value, dtype=float)
         self._cardinality = self._pmf.size
 
     @property
     def cardinality(self):
-        """
-        The cardinality :math:`|\\mathcal{X}|` of the source alphabet. This property is read-only.
+        r"""
+        The cardinality $|\mathcal{X}|$ of the source alphabet.
         """
         return self._cardinality
 
     def entropy(self, base=2.0):
-        """
-        Returns the source entropy :math:`\\mathrm{H}(X)`.
+        r"""
+        Returns the source entropy $\mathrm{H}(X)$. See [`komm.entropy`](/ref/entropy) for more details.
 
-        .. rubric:: Input
+        Parameters:
 
-        :code:`base` : :obj:`float` or :obj:`str`, optional
-            The base of the logarithm to be used. It must be a positive float or the string :code:`'e'`. The default value is :code:`2.0`.
+            base (Optional[float | str]): See [`komm.entropy`](/ref/entropy). The default value is $2.0$.
 
-        .. rubric:: Examples
+        Examples:
 
-        >>> dms = komm.DiscreteMemorylessSource([1/2, 1/4, 1/8, 1/8])
-        >>> dms.entropy()
-        1.75
-        >>> dms.entropy(base=4)
-        0.875
+            >>> dms = komm.DiscreteMemorylessSource([1/2, 1/4, 1/8, 1/8])
+            >>> dms.entropy()
+            1.75
+            >>> dms.entropy(base=4)
+            0.875
         """
         return _entropy(self._pmf, base=base)
 
     def __call__(self, size):
         return np.random.choice(self._cardinality, p=self._pmf, size=size)
 
     def __repr__(self):
-        args = 'pmf={}'.format(self._pmf.tolist())
-        return '{}({})'.format(self.__class__.__name__, args)
+        args = "pmf={}".format(self._pmf.tolist())
+        return "{}({})".format(self.__class__.__name__, args)
```

### Comparing `komm-0.7.4/tests/test_algebra.py` & `komm-0.8.2/tests/test_algebra.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
+import numpy as np
 import pytest
 
-import numpy as np
 import komm
 
 
 def test_binary_polynomial():
     poly = komm.BinaryPolynomial(0b10100110111)
     assert komm.BinaryPolynomial.from_coefficients([1, 1, 1, 0, 1, 1, 0, 0, 1, 0, 1]) == poly
     assert komm.BinaryPolynomial.from_exponents([0, 1, 2, 4, 5, 8, 10]) == poly
     assert poly.degree == 10
     assert np.array_equal(poly.coefficients(), [1, 1, 1, 0, 1, 1, 0, 0, 1, 0, 1])
     assert np.array_equal(poly.exponents(), [0, 1, 2, 4, 5, 8, 10])
     assert poly == komm.BinaryPolynomial(0b10100110111)
     assert poly >> 2 == komm.BinaryPolynomial(0b101001101)
     assert poly << 2 == komm.BinaryPolynomial(0b1010011011100)
-    assert poly ** 2 == komm.BinaryPolynomial(0b100010000010100010101)
+    assert poly**2 == komm.BinaryPolynomial(0b100010000010100010101)
     assert poly.evaluate(2) == 0b10100110111
     assert poly.evaluate(10) == 10100110111
     assert poly.evaluate(16) == 0x10100110111
 
     poly0 = komm.BinaryPolynomial(0b101011)
     poly1 = komm.BinaryPolynomial(0b10011101)
     assert poly0 + poly1 == komm.BinaryPolynomial(0b10110110)
@@ -40,65 +40,67 @@
     poly_lcm = komm.BinaryPolynomial(0b111000111)
 
     assert komm.BinaryPolynomial.gcd(poly0, poly1) == poly_gcd
     assert komm.BinaryPolynomial.lcm(poly0, poly1) == poly_lcm
 
 
 def test_finite_bifield():
-    """
+    r"""
     Lin--Costello, Example 2.7,  p. 46.
     """
     field = komm.FiniteBifield(4, 0b10011)
     alpha = field.primitive_element
     one = field(1)
     assert alpha**4 == one + alpha == field(0b0011)
     assert alpha**5 == alpha + alpha**2 == field(0b0110)
     assert alpha**6 == alpha**2 + alpha**3 == field(0b1100)
-    assert alpha**7 == one + alpha + alpha**3 == alpha**4 / alpha**12 == alpha**12 / alpha**5 == field(0b1011)
+    assert (
+        alpha**7 == one + alpha + alpha**3 == alpha**4 / alpha**12 == alpha**12 / alpha**5 == field(0b1011)
+    )
     assert alpha**13 == alpha**5 + alpha**7 == field(0b1101)
     assert one + alpha**5 + alpha**10 == field(0)
 
 
 def test_conjugates():
-    """
+    r"""
     Lin--Costello, Table 2.9,  p. 52.
     """
     field = komm.FiniteBifield(4, 0b10011)
     alpha = field.primitive_element
     assert set(field(0).conjugates()) == {field(0)}
     assert set(field(1).conjugates()) == {field(1)}
     assert set(field(alpha).conjugates()) == {alpha, alpha**2, alpha**4, alpha**8}
     assert set(field(alpha**3).conjugates()) == {alpha**3, alpha**6, alpha**9, alpha**12}
     assert set(field(alpha**5).conjugates()) == {alpha**5, alpha**10}
     assert set(field(alpha**7).conjugates()) == {alpha**7, alpha**11, alpha**13, alpha**14}
 
 
 def test_minimal_polynomial():
-    """
+    r"""
     Lin--Costello, Table 2.9,  p. 52.
     """
     field = komm.FiniteBifield(4, 0b10011)
     alpha = field.primitive_element
     assert field(0).minimal_polynomial() == komm.BinaryPolynomial(0b10)
     assert field(1).minimal_polynomial() == komm.BinaryPolynomial(0b11)
     assert field(alpha).minimal_polynomial() == komm.BinaryPolynomial(0b10011)
     assert field(alpha**3).minimal_polynomial() == komm.BinaryPolynomial(0b11111)
     assert field(alpha**5).minimal_polynomial() == komm.BinaryPolynomial(0b111)
     assert field(alpha**7).minimal_polynomial() == komm.BinaryPolynomial(0b11001)
 
 
-@pytest.mark.parametrize('m', list(range(2, 8)))
+@pytest.mark.parametrize("m", list(range(2, 8)))
 def test_inverse(m):
     field = komm.FiniteBifield(m)
     for i in range(1, field.order):
         a = field(i)
         assert a * a.inverse() == field(1)
 
 
-@pytest.mark.parametrize('m', list(range(2, 8)))
+@pytest.mark.parametrize("m", list(range(2, 8)))
 def test_logarithm(m):
     field = komm.FiniteBifield(m)
     alpha = field.primitive_element
     for i in range(1, field.order - 1):
         assert (alpha**i).logarithm() == i
 
 
@@ -130,16 +132,16 @@
     poly_divisor = komm.RationalPolynomial([0, 0, 0, 0, 0, 1])
     poly_quotient = komm.RationalPolynomial([])
     poly_remainder = komm.RationalPolynomial([1, 0, 2])
     assert divmod(poly_dividend, poly_divisor) == (poly_quotient, poly_remainder)
 
     poly_dividend = komm.RationalPolynomial([0, 0, 0, 0, 0, 1])
     poly_divisor = komm.RationalPolynomial([1, 0, 2])
-    poly_quotient = komm.RationalPolynomial([0, '-1/4', 0, '1/2'])
-    poly_remainder = komm.RationalPolynomial([0, '1/4'])
+    poly_quotient = komm.RationalPolynomial([0, "-1/4", 0, "1/2"])
+    poly_remainder = komm.RationalPolynomial([0, "1/4"])
     assert divmod(poly_dividend, poly_divisor) == (poly_quotient, poly_remainder)
 
     poly_dividend = komm.RationalPolynomial([12, -26, 21, -9, 2])
     poly_divisor = komm.RationalPolynomial([-3, 2])
     poly_quotient = komm.RationalPolynomial([-4, 6, -3, 1])
     poly_remainder = komm.RationalPolynomial([])
     assert poly_dividend // poly_divisor == poly_quotient
@@ -159,10 +161,10 @@
 
 
 def test_rational_polynomial_fractions():
     fraction = komm.RationalPolynomialFraction([0, 1, 2], [0, 0, 0, 1])
     assert fraction.numerator == komm.RationalPolynomial([1, 2])
     assert fraction.denominator == komm.RationalPolynomial([0, 0, 1])
 
-    fraction = komm.RationalPolynomialFraction([0, '5/14'], [0, 0, 0, '55/21'])
+    fraction = komm.RationalPolynomialFraction([0, "5/14"], [0, 0, 0, "55/21"])
     assert fraction.numerator == komm.RationalPolynomial([3])
     assert fraction.denominator == komm.RationalPolynomial([0, 0, 22])
```

### Comparing `komm-0.7.4/tests/test_error_control_convolutional.py` & `komm-0.8.2/tests/test_error_control_convolutional.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+import numpy as np
 import pytest
 
-import numpy as np
 import komm
 
 
 def test_convolutional_code():
     # Lin.Costello.04, p. 454--456.
     code = komm.ConvolutionalCode(feedforward_polynomials=[[0b1101, 0b1111]])
     assert (code.num_output_bits, code.num_input_bits) == (2, 1)
@@ -53,121 +53,171 @@
     D = code.transition_matrix
     assert np.array_equal(A, [[0, 1, 0], [0, 0, 1], [0, 0, 0]])
     assert np.array_equal(B, [[1, 0, 0]])
     assert np.array_equal(C, [[1, 0], [1, 1], [1, 1]])
     assert np.array_equal(D, [[1, 1]])
 
 
-@pytest.mark.parametrize('feedforward_polynomials, feedback_polynomials', [
-    ([[0o7, 0o5]], None),
-    ([[0o117, 0o155]], None),
-    ([[0o31, 0o27, 0o00], [0o00, 0o12, 0o15]], None),
-    ([[0o27, 0o31]], [0o27]),
-])
+@pytest.mark.parametrize(
+    "feedforward_polynomials, feedback_polynomials",
+    [
+        ([[0o7, 0o5]], None),
+        ([[0o117, 0o155]], None),
+        ([[0o31, 0o27, 0o00], [0o00, 0o12, 0o15]], None),
+        ([[0o27, 0o31]], [0o27]),
+    ],
+)
 def test_convolutional_space_state_representation_2(feedforward_polynomials, feedback_polynomials):
     code = komm.ConvolutionalCode(feedforward_polynomials, feedback_polynomials)
     n, k, nu = code.num_output_bits, code.num_input_bits, code.overall_constraint_length
 
     A = code.state_matrix
     B = code.control_matrix
     C = code.observation_matrix
     D = code.transition_matrix
 
-    input_bits = np.random.randint(2, size=100*k)
+    input_bits = np.random.randint(2, size=100 * k)
     output_bits = np.empty(n * input_bits.size // k, dtype=int)
 
     s = np.zeros(nu, dtype=int)
 
     for t, u in enumerate(np.reshape(input_bits, newshape=(-1, k))):
         s, v = (np.dot(s, A) + np.dot(u, B)) % 2, (np.dot(s, C) + np.dot(u, D)) % 2
-        output_bits[t*n : (t+1)*n] = v
+        output_bits[t * n : (t + 1) * n] = v
 
     convolutional_encoder = komm.ConvolutionalStreamEncoder(code)
     assert np.array_equal(output_bits, convolutional_encoder(input_bits))
 
 
 def test_convolutional_stream_encoder():
     # Abrantes.10, p. 307.
     code = komm.ConvolutionalCode(feedforward_polynomials=[[0b111, 0b101]])
     convolutional_encoder = komm.ConvolutionalStreamEncoder(code)
-    assert np.array_equal(convolutional_encoder([1, 0, 1, 1, 1, 0, 1, 1, 0, 0]), [1,1, 1,0, 0,0, 0,1, 1,0, 0,1, 0,0, 0,1, 0,1, 1,1])
+    assert np.array_equal(
+        convolutional_encoder([1, 0, 1, 1, 1, 0, 1, 1, 0, 0]),
+        [1, 1, 1, 0, 0, 0, 0, 1, 1, 0, 0, 1, 0, 0, 0, 1, 0, 1, 1, 1],
+    )
 
     # Lin.Costello.04, p. 454--456.
     code = komm.ConvolutionalCode(feedforward_polynomials=[[0b1101, 0b1111]])
     convolutional_encoder = komm.ConvolutionalStreamEncoder(code)
-    assert np.array_equal(convolutional_encoder([1, 0, 1, 1, 1, 0, 0, 0]), [1,1, 0,1, 0,0, 0,1, 0,1, 0,1, 0,0, 1,1])
+    assert np.array_equal(
+        convolutional_encoder([1, 0, 1, 1, 1, 0, 0, 0]), [1, 1, 0, 1, 0, 0, 0, 1, 0, 1, 0, 1, 0, 0, 1, 1]
+    )
 
     # Lin.Costello.04, p. 456--458.
     code = komm.ConvolutionalCode(feedforward_polynomials=[[0b11, 0b10, 0b11], [0b10, 0b1, 0b1]])
     convolutional_encoder = komm.ConvolutionalStreamEncoder(code)
-    assert np.array_equal(convolutional_encoder([1,1, 0,1, 1,0, 0,0]), [1,1,0, 0,0,0, 0,0,1, 1,1,1])
+    assert np.array_equal(convolutional_encoder([1, 1, 0, 1, 1, 0, 0, 0]), [1, 1, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1])
 
     # Ryan.Lin.09, p. 154.
     code = komm.ConvolutionalCode(feedforward_polynomials=[[0b111, 0b101]])
     convolutional_encoder = komm.ConvolutionalStreamEncoder(code)
-    assert np.array_equal(convolutional_encoder([1, 0, 0, 0]), [1,1, 1,0, 1,1, 0,0])
+    assert np.array_equal(convolutional_encoder([1, 0, 0, 0]), [1, 1, 1, 0, 1, 1, 0, 0])
 
     # Ibid.
     code = komm.ConvolutionalCode(feedforward_polynomials=[[0b111, 0b101]], feedback_polynomials=[0b111])
     convolutional_encoder = komm.ConvolutionalStreamEncoder(code)
-    assert np.array_equal(convolutional_encoder([1, 1, 1, 0]), [1,1, 1,0, 1,1, 0,0])
+    assert np.array_equal(convolutional_encoder([1, 1, 1, 0]), [1, 1, 1, 0, 1, 1, 0, 0])
 
 
 def test_convolutional_stream_decoder():
     # Abrantes.10, p. 307.
     code = komm.ConvolutionalCode(feedforward_polynomials=[[0b111, 0b101]])
     traceback_length = 12
-    convolutional_decoder = komm.ConvolutionalStreamDecoder(code, traceback_length, input_type='hard')
-    recvword = np.array([1,1, 0,0, 0,0, 0,0, 1,0, 0,1, 0,0, 0,1, 0,1, 1,1])
-    recvword_ = np.concatenate([recvword, np.zeros(traceback_length*code.num_output_bits, dtype=int)])
+    convolutional_decoder = komm.ConvolutionalStreamDecoder(code, traceback_length, input_type="hard")
+    recvword = np.array([1, 1, 0, 0, 0, 0, 0, 0, 1, 0, 0, 1, 0, 0, 0, 1, 0, 1, 1, 1])
+    recvword_ = np.concatenate([recvword, np.zeros(traceback_length * code.num_output_bits, dtype=int)])
     message_hat = convolutional_decoder(recvword_)
-    message_hat_ = message_hat[traceback_length :]
+    message_hat_ = message_hat[traceback_length:]
     assert np.array_equal(message_hat_, [1, 0, 1, 1, 1, 0, 1, 1, 0, 0])
 
 
-@pytest.mark.parametrize('feedforward_polynomials, feedback_polynomials, message, codeword', [
-    ([[0o7, 0o5]], None,
-     komm.int2binlist(0xcd698970bd55fe82a5e2bdd4dc8e3ff01c3f713e33eb2c9200, 200),
-     komm.int2binlist(0xbe84a1facdf49b0d258444495561c0d11f496cd12589847e89bdce6ce5555b0039b0e5589b37e56cebe5612bd2bdf7dc0000, 400)),
-
-    ([[0o117, 0o155]], None,
-     komm.int2binlist(0xcd698970bd55fe82a5e2bdd4dc8e3ff01c3f713e33eb2c9200, 200),
-     komm.int2binlist(0x3925a704c66355eb62f33de3c4512d01a6d681376ccec5f7fb8091ba4ff29b35456641cf63217ab7fd748a0560b5d4dc0000, 400)),
-
-    ([[0o31, 0o27, 0o00], [0o00, 0o12, 0o15]], None,
-     komm.int2binlist(0xcd698970bd55fe82a5e2bdd4dc8e3ff01c3f713e33eb2c9200, 200),
-     komm.int2binlist(0x6c889449f6801e93daf4e498ccf75404897d7459ce571f1581a4d05b2011986c0c8501d4000, 300)),
-
-    ([[0o27, 0o31]], [0o27],
-     komm.int2binlist(0xcd698970bd55fe82a5e2bdd4dc8e3ff01c3f713e33eb2c9200, 200),
-     komm.int2binlist(0x525114c160c91f2ac5511933f5d6ea2eceb9f48cc779f998d9d86a762d57df2a23daa7551f298d762d85d6e70e526b2c0000, 400)),
-])
+@pytest.mark.parametrize(
+    "feedforward_polynomials, feedback_polynomials, message, codeword",
+    [
+        (
+            [[0o7, 0o5]],
+            None,
+            komm.int2binlist(0xCD698970BD55FE82A5E2BDD4DC8E3FF01C3F713E33EB2C9200, 200),
+            komm.int2binlist(
+                0xBE84A1FACDF49B0D258444495561C0D11F496CD12589847E89BDCE6CE5555B0039B0E5589B37E56CEBE5612BD2BDF7DC0000,
+                400,
+            ),
+        ),
+        (
+            [[0o117, 0o155]],
+            None,
+            komm.int2binlist(0xCD698970BD55FE82A5E2BDD4DC8E3FF01C3F713E33EB2C9200, 200),
+            komm.int2binlist(
+                0x3925A704C66355EB62F33DE3C4512D01A6D681376CCEC5F7FB8091BA4FF29B35456641CF63217AB7FD748A0560B5D4DC0000,
+                400,
+            ),
+        ),
+        (
+            [[0o31, 0o27, 0o00], [0o00, 0o12, 0o15]],
+            None,
+            komm.int2binlist(0xCD698970BD55FE82A5E2BDD4DC8E3FF01C3F713E33EB2C9200, 200),
+            komm.int2binlist(0x6C889449F6801E93DAF4E498CCF75404897D7459CE571F1581A4D05B2011986C0C8501D4000, 300),
+        ),
+        (
+            [[0o27, 0o31]],
+            [0o27],
+            komm.int2binlist(0xCD698970BD55FE82A5E2BDD4DC8E3FF01C3F713E33EB2C9200, 200),
+            komm.int2binlist(
+                0x525114C160C91F2AC5511933F5D6EA2ECEB9F48CC779F998D9D86A762D57DF2A23DAA7551F298D762D85D6E70E526B2C0000,
+                400,
+            ),
+        ),
+    ],
+)
 def test_convolutional_stream_encoder_2(feedforward_polynomials, feedback_polynomials, message, codeword):
     code = komm.ConvolutionalCode(feedforward_polynomials, feedback_polynomials)
     convolutional_encoder = komm.ConvolutionalStreamEncoder(code)
     assert np.array_equal(convolutional_encoder(message), codeword)
 
 
-@pytest.mark.parametrize('feedforward_polynomials, feedback_polynomials, recvword, message_hat', [
-    ([[0o7, 0o5]], None,
-     komm.int2binlist(0x974b4459a5230ede0b95ceee67577b289b10e5f299954fcc6bcd698970bd55fe82a5e2bdd4dc8e3ff01c3f713e33eb2c9200, 400),
-     komm.int2binlist(0x1055cb0f07d8e51b703c77e5589dc1fcdbec820c9a12a130c0, 200)),
-
-    ([[0o117, 0o155]], None,
-     komm.int2binlist(0x974b4459a5230ede0b95ceee67577b289b10e5f299954fcc6bcd698970bd55fe82a5e2bdd4dc8e3ff01c3f713e33eb2c9200, 400),
-     komm.int2binlist(0x1ca9300a1f7524061b0ada89ec7e72d5906920081222bedf0, 200)),
-
-    ([[0o31, 0o27, 0o00], [0o00, 0o12, 0o15]], None,
-     komm.int2binlist(0x7577b289b10e5f299954fcc6bcd698970bd55fe82a5e2bdd4dc8e3ff01c3f713e33eb2c9200, 300),
-     komm.int2binlist(0x4b592f74786e69c9e75cfa836cffa14f917d51aae2c9ed60, 200)),
-
-    ([[0o27, 0o31]], [0o27],
-     komm.int2binlist(0x974b4459a5230ede0b95ceee67577b289b10e5f299954fcc6bcd698970bd55fe82a5e2bdd4dc8e3ff01c3f713e33eb2c9200, 400),
-     komm.int2binlist(0x192f33ae3eba2f9050b8577adb33477613a7ea67cc7965da40, 200)),
-])
+@pytest.mark.parametrize(
+    "feedforward_polynomials, feedback_polynomials, recvword, message_hat",
+    [
+        (
+            [[0o7, 0o5]],
+            None,
+            komm.int2binlist(
+                0x974B4459A5230EDE0B95CEEE67577B289B10E5F299954FCC6BCD698970BD55FE82A5E2BDD4DC8E3FF01C3F713E33EB2C9200,
+                400,
+            ),
+            komm.int2binlist(0x1055CB0F07D8E51B703C77E5589DC1FCDBEC820C9A12A130C0, 200),
+        ),
+        (
+            [[0o117, 0o155]],
+            None,
+            komm.int2binlist(
+                0x974B4459A5230EDE0B95CEEE67577B289B10E5F299954FCC6BCD698970BD55FE82A5E2BDD4DC8E3FF01C3F713E33EB2C9200,
+                400,
+            ),
+            komm.int2binlist(0x1CA9300A1F7524061B0ADA89EC7E72D5906920081222BEDF0, 200),
+        ),
+        (
+            [[0o31, 0o27, 0o00], [0o00, 0o12, 0o15]],
+            None,
+            komm.int2binlist(0x7577B289B10E5F299954FCC6BCD698970BD55FE82A5E2BDD4DC8E3FF01C3F713E33EB2C9200, 300),
+            komm.int2binlist(0x4B592F74786E69C9E75CFA836CFFA14F917D51AAE2C9ED60, 200),
+        ),
+        (
+            [[0o27, 0o31]],
+            [0o27],
+            komm.int2binlist(
+                0x974B4459A5230EDE0B95CEEE67577B289B10E5F299954FCC6BCD698970BD55FE82A5E2BDD4DC8E3FF01C3F713E33EB2C9200,
+                400,
+            ),
+            komm.int2binlist(0x192F33AE3EBA2F9050B8577ADB33477613A7EA67CC7965DA40, 200),
+        ),
+    ],
+)
 def test_convolutional_stream_decoder_2(feedforward_polynomials, feedback_polynomials, recvword, message_hat):
     code = komm.ConvolutionalCode(feedforward_polynomials, feedback_polynomials)
     L = len(message_hat) // code.num_input_bits
-    recvword = np.concatenate([recvword, np.zeros(code.num_output_bits*L)])
-    convolutional_decoder = komm.ConvolutionalStreamDecoder(code, traceback_length=L, input_type='hard')
-    message_hat = np.pad(message_hat, (len(message_hat), 0), mode='constant')
+    recvword = np.concatenate([recvword, np.zeros(code.num_output_bits * L)])
+    convolutional_decoder = komm.ConvolutionalStreamDecoder(code, traceback_length=L, input_type="hard")
+    message_hat = np.pad(message_hat, (len(message_hat), 0), mode="constant")
     assert np.array_equal(message_hat, convolutional_decoder(recvword))
```

### Comparing `komm-0.7.4/tests/test_finite_state_machine.py` & `komm-0.8.2/tests/test_finite_state_machine.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,62 @@
+import numpy as np
 import pytest
 
-import numpy as np
 import komm
 
 
 def test_fsm_viterbi():
     # Sklar.01, p. 401-405.
     def metric_function(y, z):
         s = komm.int2binlist(y, width=len(z))
         return np.count_nonzero(z != s)
-    fsm = komm.FiniteStateMachine(next_states=[[0,1], [2,3], [0,1], [2,3]], outputs=[[0,3], [1,2], [3,0], [2,1]])
+
+    fsm = komm.FiniteStateMachine(
+        next_states=[[0, 1], [2, 3], [0, 1], [2, 3]], outputs=[[0, 3], [1, 2], [3, 0], [2, 1]]
+    )
     z = np.array([(1, 1), (0, 1), (0, 1), (1, 0), (0, 1)])
     initial_metrics = [0.0, np.inf, np.inf, np.inf]
     input_sequences_hat, final_metrics = fsm.viterbi(z, metric_function, initial_metrics)
     assert np.allclose(final_metrics, [2.0, 2.0, 2.0, 1.0])
-    assert np.array_equal(input_sequences_hat.T, [[1,1,0,0,0], [1,1,0,0,1], [1,1,1,1,0], [1,1,0,1,1]])
+    assert np.array_equal(input_sequences_hat.T, [[1, 1, 0, 0, 0], [1, 1, 0, 0, 1], [1, 1, 1, 1, 0], [1, 1, 0, 1, 1]])
 
     # Ryan.Lin.09, p. 176-177
     def metric_function(y, z):
-        y = (-1)**komm.int2binlist(y, width=len(z))
+        y = (-1) ** komm.int2binlist(y, width=len(z))
         return -np.dot(z, y)
-    fsm = komm.FiniteStateMachine(next_states=[[0,1], [2,3], [0,1], [2,3]], outputs=[[0,3], [1,2], [3,0], [2,1]])
+
+    fsm = komm.FiniteStateMachine(
+        next_states=[[0, 1], [2, 3], [0, 1], [2, 3]], outputs=[[0, 3], [1, 2], [3, 0], [2, 1]]
+    )
     z = np.array([(-0.7, -0.5), (-0.8, -0.6), (-1.1, +0.4), (+0.9, +0.8)])
     initial_metrics = [0.0, np.inf, np.inf, np.inf]
     input_sequences_hat, final_metrics = fsm.viterbi(z, metric_function, initial_metrics)
     assert np.allclose(final_metrics, [-3.8, -3.4, -2.6, -2.4])
-    assert np.array_equal(input_sequences_hat.T, [[1,0,0,0], [0,1,0,1], [1,1,1,0], [1,1,1,1]])
+    assert np.array_equal(input_sequences_hat.T, [[1, 0, 0, 0], [0, 1, 0, 1], [1, 1, 1, 0], [1, 1, 1, 1]])
 
 
 def test_fsm_forward_backward():
     # Lin.Costello.04, p. 572-575.
-    fsm = komm.FiniteStateMachine(next_states=[[0,1], [1,0]], outputs=[[0,3], [2,1]])
+    fsm = komm.FiniteStateMachine(next_states=[[0, 1], [1, 0]], outputs=[[0, 3], [2, 1]])
     input_posteriors = fsm.forward_backward(
         observed_sequence=-np.array([(0.8, 0.1), (1.0, -0.5), (-1.8, 1.1), (1.6, -1.6)]),
-        metric_function=lambda y, z: 0.5 * np.dot(z, (-1)**komm.int2binlist(y, width=len(z))),
+        metric_function=lambda y, z: 0.5 * np.dot(z, (-1) ** komm.int2binlist(y, width=len(z))),
         initial_state_distribution=[1, 0],
-        final_state_distribution=[1, 0])
-    with np.errstate(divide='ignore'):
+        final_state_distribution=[1, 0],
+    )
+    with np.errstate(divide="ignore"):
         llr = np.log(input_posteriors[:, 0] / input_posteriors[:, 1])
     assert np.allclose(-llr, [0.48, 0.62, -1.02, 2.08], atol=0.05)
 
     # Abrantes.10, p.434-437
-    fsm = komm.FiniteStateMachine(next_states=[[0,2], [0,2], [1,3], [1,3]], outputs=[[0,3], [3,0], [1,2], [2,1]])
+    fsm = komm.FiniteStateMachine(
+        next_states=[[0, 2], [0, 2], [1, 3], [1, 3]], outputs=[[0, 3], [3, 0], [1, 2], [2, 1]]
+    )
     input_posteriors = fsm.forward_backward(
         observed_sequence=-np.array([(0.3, 0.1), (-0.5, 0.2), (0.8, 0.5), (-0.5, 0.3), (0.1, -0.7), (1.5, -0.4)]),
-        metric_function=lambda y, z: 2.5 * np.dot(z, (-1)**komm.int2binlist(y, width=len(z))),
+        metric_function=lambda y, z: 2.5 * np.dot(z, (-1) ** komm.int2binlist(y, width=len(z))),
         initial_state_distribution=[1, 0, 0, 0],
-        final_state_distribution=[1, 0, 0, 0])
-    with np.errstate(divide='ignore'):
-        llr = np.log(input_posteriors[:,0] / input_posteriors[:,1])
+        final_state_distribution=[1, 0, 0, 0],
+    )
+    with np.errstate(divide="ignore"):
+        llr = np.log(input_posteriors[:, 0] / input_posteriors[:, 1])
     assert np.allclose(-llr, [1.78, 0.24, -1.97, 5.52, -np.inf, -np.inf], atol=0.05)
```

### Comparing `komm-0.7.4/tests/test_quantization.py` & `komm-0.8.2/tests/test_quantization.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,36 @@
+import numpy as np
 import pytest
 
-import numpy as np
 import komm
 
 
 def test_scalar_quantizer():
     quantizer = komm.ScalarQuantizer(levels=[-1.0, 0.0, 1.2], thresholds=[-0.5, 0.8])
     assert np.allclose(quantizer([-1.01, -1.0, -0.99, -0.51, -0.5, -0.49]), [-1, -1, -1, -1, 0, 0])
     assert np.allclose(quantizer([0.8, -0.5]), [1.2, 0.0])
     assert np.allclose(quantizer([-1.0, 0.0, 1.2]), [-1.0, 0.0, 1.2])
     assert np.allclose(quantizer([-np.inf, np.inf]), [-1.0, 1.2])
 
 
 def test_uniform_quantizer_1():
-    quantizer = komm.UniformQuantizer(num_levels=8, input_peak=4.0, choice='unsigned')
+    quantizer = komm.UniformQuantizer(num_levels=8, input_peak=4.0, choice="unsigned")
     assert np.allclose(quantizer.levels, [0.0, 0.5, 1.0, 1.5, 2.0, 2.5, 3.0, 3.5])
     assert np.allclose(quantizer.thresholds, [0.25, 0.75, 1.25, 1.75, 2.25, 2.75, 3.25])
 
-    quantizer = komm.UniformQuantizer(num_levels=8, input_peak=4.0, choice='mid-riser')
+    quantizer = komm.UniformQuantizer(num_levels=8, input_peak=4.0, choice="mid-riser")
     assert np.allclose(quantizer.levels, [-3.5, -2.5, -1.5, -0.5, 0.5, 1.5, 2.5, 3.5])
     assert np.allclose(quantizer.thresholds, [-3.0, -2.0, -1.0, 0.0, 1.0, 2.0, 3.0])
 
-    quantizer = komm.UniformQuantizer(num_levels=8, input_peak=4.0, choice='mid-tread')
+    quantizer = komm.UniformQuantizer(num_levels=8, input_peak=4.0, choice="mid-tread")
     assert np.allclose(quantizer.levels, [-4.0, -3.0, -2.0, -1.0, 0.0, 1.0, 2.0, 3.0])
     assert np.allclose(quantizer.thresholds, [-3.5, -2.5, -1.5, -0.5, 0.5, 1.5, 2.5])
 
 
-@pytest.mark.parametrize('choice', ['unsigned', 'mid-riser', 'mid-tread'])
-@pytest.mark.parametrize('input_peak', [1.0, 0.3, 0.5, 1.0, 2.0, 3.0, 10.0])
-@pytest.mark.parametrize('num_levels', [2, 4, 8, 16, 32])
+@pytest.mark.parametrize("choice", ["unsigned", "mid-riser", "mid-tread"])
+@pytest.mark.parametrize("input_peak", [1.0, 0.3, 0.5, 1.0, 2.0, 3.0, 10.0])
+@pytest.mark.parametrize("num_levels", [2, 4, 8, 16, 32])
 def test_uniform_quantizer_2(num_levels, input_peak, choice):
     quantizer_1 = komm.UniformQuantizer(num_levels, input_peak, choice)
     quantizer_2 = komm.ScalarQuantizer(quantizer_1.levels, quantizer_1.thresholds)
     x = np.linspace(-20.0, 20.0, num=10000)
     assert np.allclose(quantizer_1(x), quantizer_2(x))
```

