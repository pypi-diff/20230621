# Comparing `tmp/komm-0.8.0.tar.gz` & `tmp/komm-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "komm-0.8.0.tar", last modified: Wed Jun 21 00:53:39 2023, max compression
+gzip compressed data, was "komm-0.8.1.tar", last modified: Wed Jun 21 01:03:46 2023, max compression
```

## Comparing `komm-0.8.0.tar` & `komm-0.8.1.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 00:53:39.107094 komm-0.8.0/
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    35147 2023-05-13 23:05:18.000000 komm-0.8.0/LICENSE
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    42583 2023-06-21 00:53:39.107094 komm-0.8.0/PKG-INFO
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1612 2023-06-20 12:29:42.000000 komm-0.8.0/README.md
-drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 00:53:39.090427 komm-0.8.0/komm/
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      418 2023-06-17 03:53:41.000000 komm-0.8.0/komm/__init__.py
-drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 00:53:39.090427 komm-0.8.0/komm/_algebra/
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     7114 2023-06-17 03:53:41.000000 komm-0.8.0/komm/_algebra/BinaryPolynomial.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2678 2023-06-13 13:41:29.000000 komm-0.8.0/komm/_algebra/BinaryPolynomialFraction.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     9049 2023-06-13 13:41:29.000000 komm-0.8.0/komm/_algebra/FiniteBifield.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     7463 2023-06-13 13:41:29.000000 komm-0.8.0/komm/_algebra/RationalPolynomial.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     3577 2023-06-13 13:41:29.000000 komm-0.8.0/komm/_algebra/RationalPolynomialFraction.py
--rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      269 2023-06-01 00:49:38.000000 komm-0.8.0/komm/_algebra/__init__.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     4028 2023-06-13 13:41:29.000000 komm-0.8.0/komm/_algebra/util.py
--rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      192 2023-06-06 01:42:18.000000 komm-0.8.0/komm/_aux.py
-drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 00:53:39.093760 komm-0.8.0/komm/_channels/
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     3469 2023-06-20 02:19:25.000000 komm-0.8.0/komm/_channels/AWGNChannel.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2580 2023-06-20 02:20:49.000000 komm-0.8.0/komm/_channels/BinaryErasureChannel.py
--rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2716 2023-06-20 02:20:05.000000 komm-0.8.0/komm/_channels/BinarySymmetricChannel.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     5967 2023-06-20 17:22:46.000000 komm-0.8.0/komm/_channels/DiscreteMemorylessChannel.py
--rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      216 2023-06-01 00:48:34.000000 komm-0.8.0/komm/_channels/__init__.py
-drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 00:53:39.097094 komm-0.8.0/komm/_error_control_block/
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     7276 2023-06-16 01:34:25.000000 komm-0.8.0/komm/_error_control_block/BCHCode.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    19826 2023-06-17 03:53:41.000000 komm-0.8.0/komm/_error_control_block/BlockCode.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1915 2023-06-16 00:23:48.000000 komm-0.8.0/komm/_error_control_block/CordaroWagnerCode.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     9304 2023-06-16 00:53:27.000000 komm-0.8.0/komm/_error_control_block/CyclicCode.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2612 2023-06-16 00:21:22.000000 komm-0.8.0/komm/_error_control_block/GolayCode.py
--rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     3499 2023-06-16 00:23:33.000000 komm-0.8.0/komm/_error_control_block/HammingCode.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     7132 2023-06-16 00:23:41.000000 komm-0.8.0/komm/_error_control_block/ReedMullerCode.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2435 2023-06-16 00:23:37.000000 komm-0.8.0/komm/_error_control_block/RepetitionCode.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2073 2023-06-16 00:24:47.000000 komm-0.8.0/komm/_error_control_block/SimplexCode.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2408 2023-06-16 00:23:35.000000 komm-0.8.0/komm/_error_control_block/SingleParityCheckCode.py
--rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      396 2023-06-01 00:49:32.000000 komm-0.8.0/komm/_error_control_block/__init__.py
-drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 00:53:39.097094 komm-0.8.0/komm/_error_control_checksum/
--rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      102 2023-06-01 00:49:44.000000 komm-0.8.0/komm/_error_control_checksum/CyclicRedundancyCheck.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)       57 2023-06-01 00:49:46.000000 komm-0.8.0/komm/_error_control_checksum/__init__.py
-drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 00:53:39.097094 komm-0.8.0/komm/_error_control_convolutional/
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    14843 2023-06-17 03:53:41.000000 komm-0.8.0/komm/_error_control_convolutional/ConvolutionalCode.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     3043 2023-06-17 03:53:41.000000 komm-0.8.0/komm/_error_control_convolutional/ConvolutionalStreamDecoder.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1554 2023-06-17 03:53:36.000000 komm-0.8.0/komm/_error_control_convolutional/ConvolutionalStreamEncoder.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    11569 2023-06-17 03:53:41.000000 komm-0.8.0/komm/_error_control_convolutional/TerminatedConvolutionalCode.py
--rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      252 2023-06-01 00:49:57.000000 komm-0.8.0/komm/_error_control_convolutional/__init__.py
-drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 00:53:39.097094 komm-0.8.0/komm/_finite_state_machine/
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    16691 2023-06-13 13:41:29.000000 komm-0.8.0/komm/_finite_state_machine/FiniteStateMachine.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)       51 2023-06-01 00:50:36.000000 komm-0.8.0/komm/_finite_state_machine/__init__.py
-drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 00:53:39.100427 komm-0.8.0/komm/_modulation/
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     4066 2023-06-20 02:11:47.000000 komm-0.8.0/komm/_modulation/APSKModulation.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2736 2023-06-20 01:44:54.000000 komm-0.8.0/komm/_modulation/ASKModulation.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    12099 2023-06-20 18:39:44.000000 komm-0.8.0/komm/_modulation/Modulation.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2287 2023-06-20 01:45:29.000000 komm-0.8.0/komm/_modulation/PAModulation.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2853 2023-06-20 01:45:02.000000 komm-0.8.0/komm/_modulation/PSKModulation.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     5530 2023-06-20 01:45:12.000000 komm-0.8.0/komm/_modulation/QAModulation.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      238 2023-06-20 01:16:54.000000 komm-0.8.0/komm/_modulation/__init__.py
--rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1294 2023-06-01 00:51:22.000000 komm-0.8.0/komm/_modulation/util.py
-drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 00:53:39.100427 komm-0.8.0/komm/_pulses/
--rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1274 2023-06-21 00:07:43.000000 komm-0.8.0/komm/_pulses/FormattingPulse.py
--rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2316 2023-06-21 00:07:43.000000 komm-0.8.0/komm/_pulses/GaussianPulse.py
--rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      951 2023-06-21 00:07:43.000000 komm-0.8.0/komm/_pulses/ManchesterPulse.py
--rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2460 2023-06-21 00:07:43.000000 komm-0.8.0/komm/_pulses/RaisedCosinePulse.py
--rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)       90 2023-06-06 01:42:18.000000 komm-0.8.0/komm/_pulses/ReceiveFilter.py
--rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1617 2023-06-21 00:07:43.000000 komm-0.8.0/komm/_pulses/RectangularPulse.py
--rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2528 2023-06-21 00:07:43.000000 komm-0.8.0/komm/_pulses/RootRaisedCosinePulse.py
--rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1226 2023-06-21 00:07:43.000000 komm-0.8.0/komm/_pulses/SincPulse.py
--rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1365 2023-06-21 00:07:43.000000 komm-0.8.0/komm/_pulses/TransmitFilter.py
--rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      356 2023-06-21 00:07:43.000000 komm-0.8.0/komm/_pulses/__init__.py
-drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 00:53:39.103761 komm-0.8.0/komm/_quantization/
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      172 2023-06-13 13:41:29.000000 komm-0.8.0/komm/_quantization/LloydMaxQuantizer.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     3601 2023-06-13 13:41:29.000000 komm-0.8.0/komm/_quantization/ScalarQuantizer.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     4514 2023-06-13 13:41:29.000000 komm-0.8.0/komm/_quantization/UniformQuantizer.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      141 2023-06-01 00:52:43.000000 komm-0.8.0/komm/_quantization/__init__.py
-drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 00:53:39.103761 komm-0.8.0/komm/_sequences/
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1895 2023-06-13 13:41:29.000000 komm-0.8.0/komm/_sequences/BarkerSequence.py
--rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     4483 2023-06-18 23:40:21.000000 komm-0.8.0/komm/_sequences/BinarySequence.py
--rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      149 2023-06-06 01:42:18.000000 komm-0.8.0/komm/_sequences/GoldSequence.py
--rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      153 2023-06-06 01:42:18.000000 komm-0.8.0/komm/_sequences/KasamiSequence.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     6920 2023-06-19 02:08:59.000000 komm-0.8.0/komm/_sequences/LFSRSequence.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     4923 2023-06-19 00:06:38.000000 komm-0.8.0/komm/_sequences/WalshHadamardSequence.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2865 2023-06-19 23:56:43.000000 komm-0.8.0/komm/_sequences/ZadoffChuSequence.py
--rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      358 2023-06-17 16:09:32.000000 komm-0.8.0/komm/_sequences/__init__.py
-drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 00:53:39.103761 komm-0.8.0/komm/_source_coding/
--rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     6572 2023-06-15 18:52:28.000000 komm-0.8.0/komm/_source_coding/FixedToVariableCode.py
--rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     3895 2023-06-15 20:06:05.000000 komm-0.8.0/komm/_source_coding/HuffmanCode.py
--rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2788 2023-06-15 20:06:05.000000 komm-0.8.0/komm/_source_coding/TunstallCode.py
--rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     6017 2023-06-15 20:06:05.000000 komm-0.8.0/komm/_source_coding/VariableToFixedCode.py
--rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      182 2023-06-01 00:53:25.000000 komm-0.8.0/komm/_source_coding/__init__.py
--rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      424 2023-06-01 00:53:27.000000 komm-0.8.0/komm/_source_coding/util.py
-drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 00:53:39.107094 komm-0.8.0/komm/_sources/
--rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2253 2023-06-20 02:23:08.000000 komm-0.8.0/komm/_sources/DiscreteMemorylessSource.py
--rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)       63 2023-06-01 00:53:36.000000 komm-0.8.0/komm/_sources/__init__.py
-drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 00:53:39.090427 komm-0.8.0/komm.egg-info/
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    42583 2023-06-21 00:53:39.000000 komm-0.8.0/komm.egg-info/PKG-INFO
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2969 2023-06-21 00:53:39.000000 komm-0.8.0/komm.egg-info/SOURCES.txt
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        1 2023-06-21 00:53:39.000000 komm-0.8.0/komm.egg-info/dependency_links.txt
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        1 2023-06-21 00:53:39.000000 komm-0.8.0/komm.egg-info/top_level.txt
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      688 2023-06-21 00:44:17.000000 komm-0.8.0/pyproject.toml
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)       38 2023-06-21 00:53:39.107094 komm-0.8.0/setup.cfg
-drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 00:53:39.107094 komm-0.8.0/tests/
--rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     7158 2023-06-06 01:42:18.000000 komm-0.8.0/tests/test_algebra.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      510 2023-06-01 00:55:24.000000 komm-0.8.0/tests/test_channels.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     9462 2023-06-01 00:55:29.000000 komm-0.8.0/tests/test_error_control_convolutional.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2781 2023-06-01 00:55:31.000000 komm-0.8.0/tests/test_finite_state_machine.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1802 2023-06-01 00:55:36.000000 komm-0.8.0/tests/test_quantization.py
--rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      290 2023-06-01 00:55:44.000000 komm-0.8.0/tests/test_sources.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:03:46.431523 komm-0.8.1/
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    35147 2023-05-13 23:05:18.000000 komm-0.8.1/LICENSE
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    42583 2023-06-21 01:03:46.431523 komm-0.8.1/PKG-INFO
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1612 2023-06-20 12:29:42.000000 komm-0.8.1/README.md
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:03:46.414857 komm-0.8.1/komm/
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      418 2023-06-17 03:53:41.000000 komm-0.8.1/komm/__init__.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:03:46.418190 komm-0.8.1/komm/_algebra/
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     7114 2023-06-17 03:53:41.000000 komm-0.8.1/komm/_algebra/BinaryPolynomial.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2678 2023-06-13 13:41:29.000000 komm-0.8.1/komm/_algebra/BinaryPolynomialFraction.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     9049 2023-06-13 13:41:29.000000 komm-0.8.1/komm/_algebra/FiniteBifield.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     7463 2023-06-13 13:41:29.000000 komm-0.8.1/komm/_algebra/RationalPolynomial.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     3577 2023-06-13 13:41:29.000000 komm-0.8.1/komm/_algebra/RationalPolynomialFraction.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      269 2023-06-01 00:49:38.000000 komm-0.8.1/komm/_algebra/__init__.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     4028 2023-06-13 13:41:29.000000 komm-0.8.1/komm/_algebra/util.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      192 2023-06-06 01:42:18.000000 komm-0.8.1/komm/_aux.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:03:46.418190 komm-0.8.1/komm/_channels/
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     3469 2023-06-20 02:19:25.000000 komm-0.8.1/komm/_channels/AWGNChannel.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2580 2023-06-20 02:20:49.000000 komm-0.8.1/komm/_channels/BinaryErasureChannel.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2716 2023-06-20 02:20:05.000000 komm-0.8.1/komm/_channels/BinarySymmetricChannel.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     5967 2023-06-20 17:22:46.000000 komm-0.8.1/komm/_channels/DiscreteMemorylessChannel.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      216 2023-06-01 00:48:34.000000 komm-0.8.1/komm/_channels/__init__.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:03:46.421523 komm-0.8.1/komm/_error_control_block/
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     7276 2023-06-16 01:34:25.000000 komm-0.8.1/komm/_error_control_block/BCHCode.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    19826 2023-06-17 03:53:41.000000 komm-0.8.1/komm/_error_control_block/BlockCode.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1915 2023-06-16 00:23:48.000000 komm-0.8.1/komm/_error_control_block/CordaroWagnerCode.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     9304 2023-06-16 00:53:27.000000 komm-0.8.1/komm/_error_control_block/CyclicCode.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2612 2023-06-16 00:21:22.000000 komm-0.8.1/komm/_error_control_block/GolayCode.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     3499 2023-06-16 00:23:33.000000 komm-0.8.1/komm/_error_control_block/HammingCode.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     7132 2023-06-16 00:23:41.000000 komm-0.8.1/komm/_error_control_block/ReedMullerCode.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2435 2023-06-16 00:23:37.000000 komm-0.8.1/komm/_error_control_block/RepetitionCode.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2073 2023-06-16 00:24:47.000000 komm-0.8.1/komm/_error_control_block/SimplexCode.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2408 2023-06-16 00:23:35.000000 komm-0.8.1/komm/_error_control_block/SingleParityCheckCode.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      396 2023-06-01 00:49:32.000000 komm-0.8.1/komm/_error_control_block/__init__.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:03:46.421523 komm-0.8.1/komm/_error_control_checksum/
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      102 2023-06-01 00:49:44.000000 komm-0.8.1/komm/_error_control_checksum/CyclicRedundancyCheck.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)       57 2023-06-01 00:49:46.000000 komm-0.8.1/komm/_error_control_checksum/__init__.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:03:46.421523 komm-0.8.1/komm/_error_control_convolutional/
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    14843 2023-06-17 03:53:41.000000 komm-0.8.1/komm/_error_control_convolutional/ConvolutionalCode.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     3043 2023-06-17 03:53:41.000000 komm-0.8.1/komm/_error_control_convolutional/ConvolutionalStreamDecoder.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1554 2023-06-17 03:53:36.000000 komm-0.8.1/komm/_error_control_convolutional/ConvolutionalStreamEncoder.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    11569 2023-06-17 03:53:41.000000 komm-0.8.1/komm/_error_control_convolutional/TerminatedConvolutionalCode.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      252 2023-06-01 00:49:57.000000 komm-0.8.1/komm/_error_control_convolutional/__init__.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:03:46.421523 komm-0.8.1/komm/_finite_state_machine/
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    16691 2023-06-13 13:41:29.000000 komm-0.8.1/komm/_finite_state_machine/FiniteStateMachine.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)       51 2023-06-01 00:50:36.000000 komm-0.8.1/komm/_finite_state_machine/__init__.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:03:46.424857 komm-0.8.1/komm/_modulation/
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     4066 2023-06-20 02:11:47.000000 komm-0.8.1/komm/_modulation/APSKModulation.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2736 2023-06-20 01:44:54.000000 komm-0.8.1/komm/_modulation/ASKModulation.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    12099 2023-06-20 18:39:44.000000 komm-0.8.1/komm/_modulation/Modulation.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2287 2023-06-20 01:45:29.000000 komm-0.8.1/komm/_modulation/PAModulation.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2853 2023-06-20 01:45:02.000000 komm-0.8.1/komm/_modulation/PSKModulation.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     5530 2023-06-20 01:45:12.000000 komm-0.8.1/komm/_modulation/QAModulation.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      238 2023-06-20 01:16:54.000000 komm-0.8.1/komm/_modulation/__init__.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1294 2023-06-01 00:51:22.000000 komm-0.8.1/komm/_modulation/util.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:03:46.428190 komm-0.8.1/komm/_pulses/
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1274 2023-06-21 00:07:43.000000 komm-0.8.1/komm/_pulses/FormattingPulse.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2316 2023-06-21 00:07:43.000000 komm-0.8.1/komm/_pulses/GaussianPulse.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      951 2023-06-21 00:07:43.000000 komm-0.8.1/komm/_pulses/ManchesterPulse.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2460 2023-06-21 00:07:43.000000 komm-0.8.1/komm/_pulses/RaisedCosinePulse.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)       90 2023-06-06 01:42:18.000000 komm-0.8.1/komm/_pulses/ReceiveFilter.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1617 2023-06-21 00:07:43.000000 komm-0.8.1/komm/_pulses/RectangularPulse.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2528 2023-06-21 00:07:43.000000 komm-0.8.1/komm/_pulses/RootRaisedCosinePulse.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1226 2023-06-21 00:07:43.000000 komm-0.8.1/komm/_pulses/SincPulse.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1365 2023-06-21 00:07:43.000000 komm-0.8.1/komm/_pulses/TransmitFilter.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      356 2023-06-21 00:07:43.000000 komm-0.8.1/komm/_pulses/__init__.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:03:46.428190 komm-0.8.1/komm/_quantization/
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      172 2023-06-13 13:41:29.000000 komm-0.8.1/komm/_quantization/LloydMaxQuantizer.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     3601 2023-06-13 13:41:29.000000 komm-0.8.1/komm/_quantization/ScalarQuantizer.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     4514 2023-06-13 13:41:29.000000 komm-0.8.1/komm/_quantization/UniformQuantizer.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      141 2023-06-01 00:52:43.000000 komm-0.8.1/komm/_quantization/__init__.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:03:46.428190 komm-0.8.1/komm/_sequences/
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1895 2023-06-13 13:41:29.000000 komm-0.8.1/komm/_sequences/BarkerSequence.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     4483 2023-06-18 23:40:21.000000 komm-0.8.1/komm/_sequences/BinarySequence.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      149 2023-06-06 01:42:18.000000 komm-0.8.1/komm/_sequences/GoldSequence.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      153 2023-06-06 01:42:18.000000 komm-0.8.1/komm/_sequences/KasamiSequence.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     6920 2023-06-19 02:08:59.000000 komm-0.8.1/komm/_sequences/LFSRSequence.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     4923 2023-06-19 00:06:38.000000 komm-0.8.1/komm/_sequences/WalshHadamardSequence.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2865 2023-06-19 23:56:43.000000 komm-0.8.1/komm/_sequences/ZadoffChuSequence.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      358 2023-06-17 16:09:32.000000 komm-0.8.1/komm/_sequences/__init__.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:03:46.431523 komm-0.8.1/komm/_source_coding/
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     6572 2023-06-15 18:52:28.000000 komm-0.8.1/komm/_source_coding/FixedToVariableCode.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     3895 2023-06-15 20:06:05.000000 komm-0.8.1/komm/_source_coding/HuffmanCode.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2788 2023-06-15 20:06:05.000000 komm-0.8.1/komm/_source_coding/TunstallCode.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     6017 2023-06-15 20:06:05.000000 komm-0.8.1/komm/_source_coding/VariableToFixedCode.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      182 2023-06-01 00:53:25.000000 komm-0.8.1/komm/_source_coding/__init__.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      424 2023-06-01 00:53:27.000000 komm-0.8.1/komm/_source_coding/util.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:03:46.431523 komm-0.8.1/komm/_sources/
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2253 2023-06-20 02:23:08.000000 komm-0.8.1/komm/_sources/DiscreteMemorylessSource.py
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)       63 2023-06-01 00:53:36.000000 komm-0.8.1/komm/_sources/__init__.py
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:03:46.414857 komm-0.8.1/komm.egg-info/
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)    42583 2023-06-21 01:03:46.000000 komm-0.8.1/komm.egg-info/PKG-INFO
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2969 2023-06-21 01:03:46.000000 komm-0.8.1/komm.egg-info/SOURCES.txt
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        1 2023-06-21 01:03:46.000000 komm-0.8.1/komm.egg-info/dependency_links.txt
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        5 2023-06-21 01:03:46.000000 komm-0.8.1/komm.egg-info/top_level.txt
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      694 2023-06-21 01:01:26.000000 komm-0.8.1/pyproject.toml
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)       38 2023-06-21 01:03:46.431523 komm-0.8.1/setup.cfg
+drwxr-x---   0 roberto.nobrega  (1000) roberto.nobrega  (1000)        0 2023-06-21 01:03:46.431523 komm-0.8.1/tests/
+-rw-r--r--   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     7158 2023-06-06 01:42:18.000000 komm-0.8.1/tests/test_algebra.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      510 2023-06-01 00:55:24.000000 komm-0.8.1/tests/test_channels.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     9462 2023-06-01 00:55:29.000000 komm-0.8.1/tests/test_error_control_convolutional.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     2781 2023-06-01 00:55:31.000000 komm-0.8.1/tests/test_finite_state_machine.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)     1802 2023-06-01 00:55:36.000000 komm-0.8.1/tests/test_quantization.py
+-rw-r-----   0 roberto.nobrega  (1000) roberto.nobrega  (1000)      290 2023-06-01 00:55:44.000000 komm-0.8.1/tests/test_sources.py
```

### Comparing `komm-0.8.0/LICENSE` & `komm-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/PKG-INFO` & `komm-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: komm
-Version: 0.8.0
+Version: 0.8.1
 Summary: An open-source library for Python 3 providing tools for analysis and simulation of analog and digital communication systems.
 Author-email: "Roberto W. Nobrega" <rwnobrega@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `komm-0.8.0/README.md` & `komm-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_algebra/BinaryPolynomial.py` & `komm-0.8.1/komm/_algebra/BinaryPolynomial.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_algebra/BinaryPolynomialFraction.py` & `komm-0.8.1/komm/_algebra/BinaryPolynomialFraction.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_algebra/FiniteBifield.py` & `komm-0.8.1/komm/_algebra/FiniteBifield.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_algebra/RationalPolynomial.py` & `komm-0.8.1/komm/_algebra/RationalPolynomial.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_algebra/RationalPolynomialFraction.py` & `komm-0.8.1/komm/_algebra/RationalPolynomialFraction.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_algebra/util.py` & `komm-0.8.1/komm/_algebra/util.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_channels/AWGNChannel.py` & `komm-0.8.1/komm/_channels/AWGNChannel.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_channels/BinaryErasureChannel.py` & `komm-0.8.1/komm/_channels/BinaryErasureChannel.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_channels/BinarySymmetricChannel.py` & `komm-0.8.1/komm/_channels/BinarySymmetricChannel.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_channels/DiscreteMemorylessChannel.py` & `komm-0.8.1/komm/_channels/DiscreteMemorylessChannel.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_error_control_block/BCHCode.py` & `komm-0.8.1/komm/_error_control_block/BCHCode.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_error_control_block/BlockCode.py` & `komm-0.8.1/komm/_error_control_block/BlockCode.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_error_control_block/CordaroWagnerCode.py` & `komm-0.8.1/komm/_error_control_block/CordaroWagnerCode.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_error_control_block/CyclicCode.py` & `komm-0.8.1/komm/_error_control_block/CyclicCode.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_error_control_block/GolayCode.py` & `komm-0.8.1/komm/_error_control_block/GolayCode.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_error_control_block/HammingCode.py` & `komm-0.8.1/komm/_error_control_block/HammingCode.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_error_control_block/ReedMullerCode.py` & `komm-0.8.1/komm/_error_control_block/ReedMullerCode.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_error_control_block/RepetitionCode.py` & `komm-0.8.1/komm/_error_control_block/RepetitionCode.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_error_control_block/SimplexCode.py` & `komm-0.8.1/komm/_error_control_block/SimplexCode.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_error_control_block/SingleParityCheckCode.py` & `komm-0.8.1/komm/_error_control_block/SingleParityCheckCode.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_error_control_convolutional/ConvolutionalCode.py` & `komm-0.8.1/komm/_error_control_convolutional/ConvolutionalCode.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_error_control_convolutional/ConvolutionalStreamDecoder.py` & `komm-0.8.1/komm/_error_control_convolutional/ConvolutionalStreamDecoder.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_error_control_convolutional/ConvolutionalStreamEncoder.py` & `komm-0.8.1/komm/_error_control_convolutional/ConvolutionalStreamEncoder.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_error_control_convolutional/TerminatedConvolutionalCode.py` & `komm-0.8.1/komm/_error_control_convolutional/TerminatedConvolutionalCode.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_finite_state_machine/FiniteStateMachine.py` & `komm-0.8.1/komm/_finite_state_machine/FiniteStateMachine.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_modulation/APSKModulation.py` & `komm-0.8.1/komm/_modulation/APSKModulation.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_modulation/ASKModulation.py` & `komm-0.8.1/komm/_modulation/ASKModulation.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_modulation/Modulation.py` & `komm-0.8.1/komm/_modulation/Modulation.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_modulation/PAModulation.py` & `komm-0.8.1/komm/_modulation/PAModulation.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_modulation/PSKModulation.py` & `komm-0.8.1/komm/_modulation/PSKModulation.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_modulation/QAModulation.py` & `komm-0.8.1/komm/_modulation/QAModulation.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_modulation/util.py` & `komm-0.8.1/komm/_modulation/util.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_pulses/FormattingPulse.py` & `komm-0.8.1/komm/_pulses/FormattingPulse.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_pulses/GaussianPulse.py` & `komm-0.8.1/komm/_pulses/GaussianPulse.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_pulses/ManchesterPulse.py` & `komm-0.8.1/komm/_pulses/ManchesterPulse.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_pulses/RaisedCosinePulse.py` & `komm-0.8.1/komm/_pulses/RaisedCosinePulse.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_pulses/RectangularPulse.py` & `komm-0.8.1/komm/_pulses/RectangularPulse.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_pulses/RootRaisedCosinePulse.py` & `komm-0.8.1/komm/_pulses/RootRaisedCosinePulse.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_pulses/SincPulse.py` & `komm-0.8.1/komm/_pulses/SincPulse.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_pulses/TransmitFilter.py` & `komm-0.8.1/komm/_pulses/TransmitFilter.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_quantization/ScalarQuantizer.py` & `komm-0.8.1/komm/_quantization/ScalarQuantizer.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_quantization/UniformQuantizer.py` & `komm-0.8.1/komm/_quantization/UniformQuantizer.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_sequences/BarkerSequence.py` & `komm-0.8.1/komm/_sequences/BarkerSequence.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_sequences/BinarySequence.py` & `komm-0.8.1/komm/_sequences/BinarySequence.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_sequences/LFSRSequence.py` & `komm-0.8.1/komm/_sequences/LFSRSequence.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_sequences/WalshHadamardSequence.py` & `komm-0.8.1/komm/_sequences/WalshHadamardSequence.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_sequences/ZadoffChuSequence.py` & `komm-0.8.1/komm/_sequences/ZadoffChuSequence.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_source_coding/FixedToVariableCode.py` & `komm-0.8.1/komm/_source_coding/FixedToVariableCode.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_source_coding/HuffmanCode.py` & `komm-0.8.1/komm/_source_coding/HuffmanCode.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_source_coding/TunstallCode.py` & `komm-0.8.1/komm/_source_coding/TunstallCode.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_source_coding/VariableToFixedCode.py` & `komm-0.8.1/komm/_source_coding/VariableToFixedCode.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm/_sources/DiscreteMemorylessSource.py` & `komm-0.8.1/komm/_sources/DiscreteMemorylessSource.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/komm.egg-info/PKG-INFO` & `komm-0.8.1/komm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: komm
-Version: 0.8.0
+Version: 0.8.1
 Summary: An open-source library for Python 3 providing tools for analysis and simulation of analog and digital communication systems.
 Author-email: "Roberto W. Nobrega" <rwnobrega@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `komm-0.8.0/komm.egg-info/SOURCES.txt` & `komm-0.8.1/komm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/pyproject.toml` & `komm-0.8.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [project]
 name = "komm"
 authors = [{ name = "Roberto W. Nobrega", email = "rwnobrega@gmail.com" }]
 description = "An open-source library for Python 3 providing tools for analysis and simulation of analog and digital communication systems."
 readme = "README.md"
 urls = { home = "https://komm.dev/", repository = "https://github.com/rwnobrega/komm/" }
 license = { file = "LICENSE" }
-version = "0.8.0"
+version = "0.8.1"
 requires-python = ">=3.8"
 
 [build-system]
 requires = ["setuptools", "wheel", "numpy", "scipy"]
 
 [tool.setuptools]
-py-modules = []
+py-modules = ["komm"]
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules"
 python_files = "test_*.py"
 python_functions = "test_*"
 pythonpath = "."
 testpaths = ["komm", "tests"]
```

### Comparing `komm-0.8.0/tests/test_algebra.py` & `komm-0.8.1/tests/test_algebra.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/tests/test_error_control_convolutional.py` & `komm-0.8.1/tests/test_error_control_convolutional.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/tests/test_finite_state_machine.py` & `komm-0.8.1/tests/test_finite_state_machine.py`

 * *Files identical despite different names*

### Comparing `komm-0.8.0/tests/test_quantization.py` & `komm-0.8.1/tests/test_quantization.py`

 * *Files identical despite different names*

